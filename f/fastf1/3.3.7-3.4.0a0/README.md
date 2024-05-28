# Comparing `tmp/fastf1-3.3.7.tar.gz` & `tmp/fastf1-3.4.0a0.tar.gz`

## Comparing `fastf1-3.3.7.tar` & `fastf1-3.4.0a0.tar`

### file list

```diff
@@ -1,62 +1,76 @@
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastf1-3.3.7/examples/README.rst
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastf1-3.3.7/examples/example_fastf1_signalrclient.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 fastf1-3.3.7/examples/plot_annotate_corners.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 fastf1-3.3.7/examples/plot_annotate_speed_trace.py
--rwxr-xr-x   0        0        0     2014 2020-02-02 00:00:00.000000 fastf1-3.3.7/examples/plot_driver_laptimes.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 fastf1-3.3.7/examples/plot_gear_shifts_on_track.py
--rwxr-xr-x   0        0        0     3163 2020-02-02 00:00:00.000000 fastf1-3.3.7/examples/plot_laptimes_distribution.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 fastf1-3.3.7/examples/plot_position_changes.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 fastf1-3.3.7/examples/plot_qualifying_results.py
--rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 fastf1-3.3.7/examples/plot_results_tracker.py
--rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 fastf1-3.3.7/examples/plot_speed_on_track.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 fastf1-3.3.7/examples/plot_speed_traces.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 fastf1-3.3.7/examples/plot_strategy.py
--rwxr-xr-x   0        0        0     2034 2020-02-02 00:00:00.000000 fastf1-3.3.7/examples/plot_team_pace_ranking.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 fastf1-3.3.7/examples/plot_who_can_still_win_wdc.py
--rw-r--r--   0        0        0     5356 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/__init__.py
--rw-r--r--   0        0        0    75158 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/_api.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/_version.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/api.py
--rw-r--r--   0        0        0   155296 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/core.py
--rw-r--r--   0        0        0    41549 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/events.py
--rw-r--r--   0        0        0    10591 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/legacy.py
--rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/logger.py
--rw-r--r--   0        0        0    16355 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/plotting.py
--rw-r--r--   0        0        0    26173 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/req.py
--rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/utils.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/ergast/__init__.py
--rw-r--r--   0        0        0    61561 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/ergast/interface.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/ergast/legacy.py
--rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/ergast/sphinx.py
--rw-r--r--   0        0        0    18692 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/ergast/structure.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/internals/__init__.py
--rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/internals/pandas_base.py
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/internals/pandas_extensions.py
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/livetiming/__init__.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/livetiming/__main__.py
--rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/livetiming/client.py
--rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/livetiming/data.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/mvapi/__init__.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/mvapi/api.py
--rw-r--r--   0        0        0     5927 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/mvapi/data.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/mvapi/internals.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/signalr_aio/LICENSE
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/signalr_aio/README.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/signalr_aio/__init__.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/signalr_aio/_connection.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/signalr_aio/events/__init__.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/signalr_aio/events/_events.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/signalr_aio/hubs/__init__.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/signalr_aio/hubs/_hub.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/signalr_aio/transports/__init__.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/signalr_aio/transports/_exceptions.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/signalr_aio/transports/_parameters.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/signalr_aio/transports/_queue_events.py
--rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 fastf1-3.3.7/fastf1/signalr_aio/transports/_transport.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 fastf1-3.3.7/requirements/dev.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 fastf1-3.3.7/requirements/minver.txt
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastf1-3.3.7/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastf1-3.3.7/LICENSE
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 fastf1-3.3.7/README.md
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 fastf1-3.3.7/pyproject.toml
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 fastf1-3.3.7/PKG-INFO
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/README.rst
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/example_fastf1_signalrclient.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_annotate_corners.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_annotate_speed_trace.py
+-rwxr-xr-x   0        0        0     2135 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_driver_laptimes.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_driver_styling.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_gear_shifts_on_track.py
+-rwxr-xr-x   0        0        0     2837 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_laptimes_distribution.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_position_changes.py
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_qualifying_results.py
+-rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_results_tracker.py
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_speed_on_track.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_speed_traces.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_strategy.py
+-rwxr-xr-x   0        0        0     2091 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_team_pace_ranking.py
+-rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/examples/plot_who_can_still_win_wdc.py
+-rw-r--r--   0        0        0     5356 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/__init__.py
+-rw-r--r--   0        0        0    74642 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/_api.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/_version.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/api.py
+-rw-r--r--   0        0        0   154357 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/core.py
+-rw-r--r--   0        0        0    43127 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/events.py
+-rw-r--r--   0        0        0    10633 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/legacy.py
+-rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/logger.py
+-rw-r--r--   0        0        0    26173 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/req.py
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/utils.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/ergast/__init__.py
+-rw-r--r--   0        0        0    61561 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/ergast/interface.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/ergast/legacy.py
+-rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/ergast/sphinx.py
+-rw-r--r--   0        0        0    18692 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/ergast/structure.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/internals/__init__.py
+-rw-r--r--   0        0        0     5717 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/internals/pandas_base.py
+-rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/internals/pandas_extensions.py
+-rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/livetiming/__init__.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/livetiming/__main__.py
+-rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/livetiming/client.py
+-rw-r--r--   0        0        0    10468 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/livetiming/data.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/mvapi/__init__.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/mvapi/api.py
+-rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/mvapi/data.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/mvapi/internals.py
+-rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/__init__.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_backend.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_base.py
+-rw-r--r--   0        0        0    22757 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_interface.py
+-rw-r--r--   0        0        0    14085 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_plotting.py
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_constants/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_constants/base.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_constants/season2018.py
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_constants/season2019.py
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_constants/season2020.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_constants/season2021.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_constants/season2022.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_constants/season2023.py
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/plotting/_constants/season2024.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/LICENSE
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/README.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/__init__.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/_connection.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/events/__init__.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/events/_events.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/hubs/__init__.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/hubs/_hub.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/transports/__init__.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/transports/_exceptions.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/transports/_parameters.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/transports/_queue_events.py
+-rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/fastf1/signalr_aio/transports/_transport.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/requirements/dev.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/requirements/minver.txt
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/LICENSE
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/README.md
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/pyproject.toml
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 fastf1-3.4.0a0/PKG-INFO
```

### Comparing `fastf1-3.3.7/examples/plot_annotate_corners.py` & `fastf1-3.4.0a0/examples/plot_annotate_corners.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.7/examples/plot_annotate_speed_trace.py` & `fastf1-3.4.0a0/examples/plot_annotate_speed_trace.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 
 
 import matplotlib.pyplot as plt
 
 import fastf1.plotting
 
 
-# enable some matplotlib patches for plotting timedelta values and load
-# FastF1's default color scheme
-fastf1.plotting.setup_mpl(misc_mpl_mods=False)
+# Enable Matplotlib patches for plotting timedelta values and load
+# FastF1's dark color scheme
+fastf1.plotting.setup_mpl(mpl_timedelta_support=True, misc_mpl_mods=False,
+                          color_scheme='fastf1')
 
 # load a session and its telemetry data
 session = fastf1.get_session(2021, 'Spanish Grand Prix', 'Q')
 session.load()
 
 ##############################################################################
 # First, we select the fastest lap and get the car telemetry data for this
@@ -31,15 +32,16 @@
 
 circuit_info = session.get_circuit_info()
 
 ##############################################################################
 # Finally, we create a plot and plot the speed trace as well as the corner
 # markers.
 
-team_color = fastf1.plotting.team_color(fastest_lap['Team'])
+team_color = fastf1.plotting.get_team_color(fastest_lap['Team'],
+                                            session=session)
 
 fig, ax = plt.subplots()
 ax.plot(car_data['Distance'], car_data['Speed'],
         color=team_color, label=fastest_lap['Driver'])
 
 # Draw vertical dotted lines at each corner that range from slightly below the
 # minimum speed to slightly above the maximum speed.
```

### Comparing `fastf1-3.3.7/examples/plot_driver_laptimes.py` & `fastf1-3.4.0a0/examples/plot_driver_laptimes.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,19 @@
 import seaborn as sns
 from matplotlib import pyplot as plt
 
 import fastf1
 import fastf1.plotting
 
 
-# The misc_mpl_mods option enables minor grid lines which clutter the plot
-fastf1.plotting.setup_mpl(misc_mpl_mods=False)
+# Enable Matplotlib patches for plotting timedelta values and load
+# FastF1's dark color scheme
+fastf1.plotting.setup_mpl(mpl_timedelta_support=True, misc_mpl_mods=False,
+                          color_scheme='fastf1')
+
 
 ###############################################################################
 # Load the race session.
 
 race = fastf1.get_session(2023, "Azerbaijan", 'R')
 race.load()
 
@@ -35,15 +38,15 @@
 fig, ax = plt.subplots(figsize=(8, 8))
 
 sns.scatterplot(data=driver_laps,
                 x="LapNumber",
                 y="LapTime",
                 ax=ax,
                 hue="Compound",
-                palette=fastf1.plotting.COMPOUND_COLORS,
+                palette=fastf1.plotting.get_compound_mapping(session=race),
                 s=80,
                 linewidth=0,
                 legend='auto')
 # sphinx_gallery_defer_figures
 
 ###############################################################################
 # Make the plot more aesthetic.
```

### Comparing `fastf1-3.3.7/examples/plot_gear_shifts_on_track.py` & `fastf1-3.4.0a0/examples/plot_gear_shifts_on_track.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.7/examples/plot_laptimes_distribution.py` & `fastf1-3.4.0a0/examples/plot_laptimes_distribution.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,16 +6,19 @@
 import seaborn as sns
 from matplotlib import pyplot as plt
 
 import fastf1
 import fastf1.plotting
 
 
-# enabling misc_mpl_mods will turn on minor grid lines that clutters the plot
-fastf1.plotting.setup_mpl(mpl_timedelta_support=False, misc_mpl_mods=False)
+# Enable Matplotlib patches for plotting timedelta values and load
+# FastF1's dark color scheme
+fastf1.plotting.setup_mpl(mpl_timedelta_support=True, misc_mpl_mods=False,
+                          color_scheme='fastf1')
+
 
 ###############################################################################
 # Load the race session
 
 race = fastf1.get_session(2023, "Azerbaijan", 'R')
 race.load()
 
@@ -31,49 +34,40 @@
 ###############################################################################
 # To plot the drivers by finishing order,
 # we need to get their three-letter abbreviations in the finishing order.
 finishing_order = [race.get_driver(i)["Abbreviation"] for i in point_finishers]
 print(finishing_order)
 
 ###############################################################################
-# We need to modify the DRIVER_COLORS palette.
-# Its keys are the driver's full names but we need the keys to be the drivers'
-# three-letter abbreviations.
-# We can do this with the DRIVER_TRANSLATE mapping.
-driver_colors = {abv: fastf1.plotting.DRIVER_COLORS[driver] for abv,
-                 driver in fastf1.plotting.DRIVER_TRANSLATE.items()}
-print(driver_colors)
-
-###############################################################################
 # First create the violin plots to show the distributions.
 # Then use the swarm plot to show the actual laptimes.
 
 # create the figure
 fig, ax = plt.subplots(figsize=(10, 5))
 
-# Seaborn doesn't have proper timedelta support
+# Seaborn doesn't have proper timedelta support,
 # so we have to convert timedelta to float (in seconds)
 driver_laps["LapTime(s)"] = driver_laps["LapTime"].dt.total_seconds()
 
 sns.violinplot(data=driver_laps,
                x="Driver",
                y="LapTime(s)",
                hue="Driver",
                inner=None,
                density_norm="area",
                order=finishing_order,
-               palette=driver_colors
+               palette=fastf1.plotting.get_driver_color_mapping(session=race)
                )
 
 sns.swarmplot(data=driver_laps,
               x="Driver",
               y="LapTime(s)",
               order=finishing_order,
               hue="Compound",
-              palette=fastf1.plotting.COMPOUND_COLORS,
+              palette=fastf1.plotting.get_compound_mapping(session=race),
               hue_order=["SOFT", "MEDIUM", "HARD"],
               linewidth=0,
               size=4,
               )
 # sphinx_gallery_defer_figures
 
 ###############################################################################
```

### Comparing `fastf1-3.3.7/examples/plot_position_changes.py` & `fastf1-3.4.0a0/examples/plot_position_changes.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 """
 
 import matplotlib.pyplot as plt
 
 import fastf1.plotting
 
 
-fastf1.plotting.setup_mpl(misc_mpl_mods=False)
+# Load FastF1's dark color scheme
+fastf1.plotting.setup_mpl(mpl_timedelta_support=False, misc_mpl_mods=False,
+                          color_scheme='fastf1')
+
 
 ##############################################################################
 # Load the session and create the plot
 session = fastf1.get_session(2023, 1, 'R')
 session.load(telemetry=False, weather=False)
 
 fig, ax = plt.subplots(figsize=(8.0, 4.9))
@@ -24,18 +27,20 @@
 # For each driver, get their three letter abbreviation (e.g. 'HAM') by simply
 # using the value of the first lap, get their color and then plot their
 # position over the number of laps.
 for drv in session.drivers:
     drv_laps = session.laps.pick_driver(drv)
 
     abb = drv_laps['Driver'].iloc[0]
-    color = fastf1.plotting.driver_color(abb)
+    style = fastf1.plotting.get_driver_style(identifier=abb,
+                                             style=['color', 'linestyle'],
+                                             session=session)
 
     ax.plot(drv_laps['LapNumber'], drv_laps['Position'],
-            label=abb, color=color)
+            label=abb, **style)
 # sphinx_gallery_defer_figures
 
 ##############################################################################
 # Finalize the plot by setting y-limits that invert the y-axis so that position
 # one is at the top, set custom tick positions and axis labels.
 ax.set_ylim([20.5, 0.5])
 ax.set_yticks([1, 5, 10, 15, 20])
```

### Comparing `fastf1-3.3.7/examples/plot_qualifying_results.py` & `fastf1-3.4.0a0/examples/plot_qualifying_results.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,46 +10,47 @@
 from timple.timedelta import strftimedelta
 
 import fastf1
 import fastf1.plotting
 from fastf1.core import Laps
 
 
-# we only want support for timedelta plotting in this example
-fastf1.plotting.setup_mpl(mpl_timedelta_support=True, color_scheme=None,
-                          misc_mpl_mods=False)
+# Enable Matplotlib patches for plotting timedelta values
+fastf1.plotting.setup_mpl(mpl_timedelta_support=True, misc_mpl_mods=False,
+                          color_scheme=None)
+
 
 session = fastf1.get_session(2021, 'Spanish Grand Prix', 'Q')
 session.load()
 
 
 ##############################################################################
 # First, we need to get an array of all drivers.
 
 drivers = pd.unique(session.laps['Driver'])
 print(drivers)
 
 
 ##############################################################################
-# After that we'll get each drivers fastest lap, create a new laps object
+# After that we'll get each driver's fastest lap, create a new laps object
 # from these laps, sort them by lap time and have pandas reindex them to
 # number them nicely by starting position.
 
 list_fastest_laps = list()
 for drv in drivers:
     drvs_fastest_lap = session.laps.pick_driver(drv).pick_fastest()
     list_fastest_laps.append(drvs_fastest_lap)
 fastest_laps = Laps(list_fastest_laps) \
     .sort_values(by='LapTime') \
     .reset_index(drop=True)
 
 
 ##############################################################################
 # The plot is nicer to look at and more easily understandable if we just plot
-# the time differences. Therefore we subtract the fastest lap time from all
+# the time differences. Therefore, we subtract the fastest lap time from all
 # other lap times.
 
 pole_lap = fastest_laps.pick_fastest()
 fastest_laps['LapTimeDelta'] = fastest_laps['LapTime'] - pole_lap['LapTime']
 
 
 ##############################################################################
@@ -60,15 +61,15 @@
 print(fastest_laps[['Driver', 'LapTime', 'LapTimeDelta']])
 
 
 ##############################################################################
 # Finally, we'll create a list of team colors per lap to color our plot.
 team_colors = list()
 for index, lap in fastest_laps.iterlaps():
-    color = fastf1.plotting.team_color(lap['Team'])
+    color = fastf1.plotting.get_team_color(lap['Team'], session=session)
     team_colors.append(color)
 
 
 ##############################################################################
 # Now, we can plot all the data
 fig, ax = plt.subplots()
 ax.barh(fastest_laps.index, fastest_laps['LapTimeDelta'],
```

### Comparing `fastf1-3.3.7/examples/plot_results_tracker.py` & `fastf1-3.4.0a0/examples/plot_results_tracker.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.7/examples/plot_speed_on_track.py` & `fastf1-3.4.0a0/examples/plot_speed_on_track.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.7/examples/plot_speed_traces.py` & `fastf1-3.4.0a0/examples/plot_speed_traces.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 
 
 import matplotlib.pyplot as plt
 
 import fastf1.plotting
 
 
-# enable some matplotlib patches for plotting timedelta values and load
-# FastF1's default color scheme
-fastf1.plotting.setup_mpl(misc_mpl_mods=False)
+# Enable Matplotlib patches for plotting timedelta values and load
+# FastF1's dark color scheme
+fastf1.plotting.setup_mpl(mpl_timedelta_support=True, misc_mpl_mods=False,
+                          color_scheme='fastf1')
 
 # load a session and its telemetry data
 session = fastf1.get_session(2021, 'Spanish Grand Prix', 'Q')
 session.load()
 
 ##############################################################################
 # First, we select the two laps that we want to compare
@@ -31,16 +32,16 @@
 ver_tel = ver_lap.get_car_data().add_distance()
 ham_tel = ham_lap.get_car_data().add_distance()
 
 ##############################################################################
 # Finally, we create a plot and plot both speed traces.
 # We color the individual lines with the driver's team colors.
 
-rbr_color = fastf1.plotting.team_color('RBR')
-mer_color = fastf1.plotting.team_color('MER')
+rbr_color = fastf1.plotting.get_team_color(ver_lap['Team'], session=session)
+mer_color = fastf1.plotting.get_team_color(ham_lap['Team'], session=session)
 
 fig, ax = plt.subplots()
 ax.plot(ver_tel['Distance'], ver_tel['Speed'], color=rbr_color, label='VER')
 ax.plot(ham_tel['Distance'], ham_tel['Speed'], color=mer_color, label='HAM')
 
 ax.set_xlabel('Distance in m')
 ax.set_ylabel('Speed in km/h')
```

### Comparing `fastf1-3.3.7/examples/plot_strategy.py` & `fastf1-3.4.0a0/examples/plot_strategy.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,19 +51,21 @@
 for driver in drivers:
     driver_stints = stints.loc[stints["Driver"] == driver]
 
     previous_stint_end = 0
     for idx, row in driver_stints.iterrows():
         # each row contains the compound name and stint length
         # we can use these information to draw horizontal bars
+        compound_color = fastf1.plotting.get_compound_color(row["Compound"],
+                                                            session=session)
         plt.barh(
             y=driver,
             width=row["StintLength"],
             left=previous_stint_end,
-            color=fastf1.plotting.COMPOUND_COLORS[row["Compound"]],
+            color=compound_color,
             edgecolor="black",
             fill=True
         )
 
         previous_stint_end += row["StintLength"]
 
 # sphinx_gallery_defer_figures
```

### Comparing `fastf1-3.3.7/examples/plot_team_pace_ranking.py` & `fastf1-3.4.0a0/examples/plot_team_pace_ranking.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 import seaborn as sns
 from matplotlib import pyplot as plt
 
 import fastf1
 import fastf1.plotting
 
 
-# activate the fastf1 color scheme (and no other modifications)
-fastf1.plotting.setup_mpl(mpl_timedelta_support=False, misc_mpl_mods=False)
+# Load FastF1's dark color scheme
+fastf1.plotting.setup_mpl(mpl_timedelta_support=False, misc_mpl_mods=False,
+                          color_scheme='fastf1')
+
 
 ###############################################################################
 # Load the race session.
 # Pick all quick laps (within 107% of fastest lap).
 # For races with mixed conditions, pick_wo_box() is better.
 race = fastf1.get_session(2024, 1, 'R')
 race.load()
@@ -36,15 +38,16 @@
     .median()["LapTime (s)"]
     .sort_values()
     .index
 )
 print(team_order)
 
 # make a color palette associating team names to hex codes
-team_palette = {team: fastf1.plotting.team_color(team) for team in team_order}
+team_palette = {team: fastf1.plotting.get_team_color(team, session=race)
+                for team in team_order}
 
 ###############################################################################
 fig, ax = plt.subplots(figsize=(15, 10))
 sns.boxplot(
     data=transformed_laps,
     x="Team",
     y="LapTime (s)",
```

### Comparing `fastf1-3.3.7/examples/plot_who_can_still_win_wdc.py` & `fastf1-3.4.0a0/examples/plot_who_can_still_win_wdc.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 SEASON = 2023
 ROUND = 15
 
 
 ##############################################################################
 # Get the current driver standings from Ergast.
-# Reference https://theoehrly.github.io/Fast-F1-Pre-Release-Documentation/ergast.html#fastf1.ergast.Ergast.get_driver_standings
+# Reference https://docs.fastf1.dev/ergast.html#fastf1.ergast.Ergast.get_driver_standings
 def get_drivers_standings():
     ergast = Ergast()
     standings = ergast.get_driver_standings(season=SEASON, round=ROUND)
     return standings.content[0]
 
 
 ##############################################################################
```

### Comparing `fastf1-3.3.7/fastf1/__init__.py` & `fastf1-3.4.0a0/fastf1/__init__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.7/fastf1/_api.py` & `fastf1-3.4.0a0/fastf1/_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1158,3541 +1158,3509 @@
 00004850: 756d 6265 724f 664c 6170 7327 2069 6e20  umberOfLaps' in 
 00004860: 7265 7370 2061 6e64 2072 6573 705b 274e  resp and resp['N
 00004870: 756d 6265 724f 664c 6170 7327 5d20 3c20  umberOfLaps'] < 
 00004880: 6170 695f 6c61 7063 6e74 293a 0a20 2020  api_lapcnt):.   
 00004890: 2020 2020 2020 2020 2069 6e5f 7061 7374           in_past
 000048a0: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
 000048b0: 2020 2020 636f 6e74 696e 7565 0a0a 2020      continue..  
-000048c0: 2020 2020 2020 2320 7661 6c75 6573 2077        # values w
-000048d0: 6869 6368 2061 7265 2075 7020 746f 2066  hich are up to f
-000048e0: 6976 6520 7365 636f 6e64 7320 6c61 7465  ive seconds late
-000048f0: 2061 7265 2073 7469 6c6c 2063 6f75 6e74   are still count
-00004900: 6564 2074 6f77 6172 6473 2074 6865 2070  ed towards the p
-00004910: 7265 7669 6f75 7320 6c61 700a 2020 2020  revious lap.    
-00004920: 2020 2020 2320 2873 6563 746f 7220 7469      # (sector ti
-00004930: 6d65 732c 2073 7065 6564 2074 7261 7073  mes, speed traps
-00004940: 2061 6e64 206c 6170 2074 696d 6573 290a   and lap times).
-00004950: 2020 2020 2020 2020 6c61 705f 6f66 6673          lap_offs
-00004960: 6574 203d 2030 0a20 2020 2020 2020 2069  et = 0.        i
-00004970: 6620 286c 6170 636e 7420 3e20 3029 2061  f (lapcnt > 0) a
-00004980: 6e64 2028 746f 5f74 696d 6564 656c 7461  nd (to_timedelta
-00004990: 2874 696d 6529 202d 2064 7276 5f64 6174  (time) - drv_dat
-000049a0: 615b 2754 696d 6527 5d5b 6c61 7063 6e74  a['Time'][lapcnt
-000049b0: 202d 2031 5d20 3c20 7064 2e54 696d 6564   - 1] < pd.Timed
-000049c0: 656c 7461 2835 2c20 2773 2729 293a 0a20  elta(5, 's')):. 
-000049d0: 2020 2020 2020 2020 2020 206c 6170 5f6f             lap_o
-000049e0: 6666 7365 7420 3d20 310a 0a20 2020 2020  ffset = 1..     
-000049f0: 2020 2069 6620 2753 6563 746f 7273 2720     if 'Sectors' 
-00004a00: 696e 2072 6573 7020 616e 6420 6973 696e  in resp and isin
-00004a10: 7374 616e 6365 2872 6573 705b 2753 6563  stance(resp['Sec
-00004a20: 746f 7273 275d 2c20 6469 6374 293a 0a20  tors'], dict):. 
-00004a30: 2020 2020 2020 2020 2020 2023 2073 6f6d             # som
-00004a40: 6574 696d 6573 2069 7427 7320 6120 6c69  etimes it's a li
-00004a50: 7374 2062 7574 2074 6865 6e20 6974 206e  st but then it n
-00004a60: 6576 6572 2063 6f6e 7461 696e 7320 7661  ever contains va
-00004a70: 6c75 6573 2e2e 2e0a 2020 2020 2020 2020  lues....        
-00004a80: 2020 2020 666f 7220 736e 2c20 7365 6374      for sn, sect
-00004a90: 6f72 2c20 7365 7373 7420 696e 2028 2827  or, sesst in (('
-00004aa0: 3027 2c20 2753 6563 746f 7231 5469 6d65  0', 'Sector1Time
-00004ab0: 272c 2027 5365 6374 6f72 3153 6573 7369  ', 'Sector1Sessi
-00004ac0: 6f6e 5469 6d65 2729 2c0a 2020 2020 2020  onTime'),.      
-00004ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004af0: 2827 3127 2c20 2753 6563 746f 7232 5469  ('1', 'Sector2Ti
-00004b00: 6d65 272c 2027 5365 6374 6f72 3253 6573  me', 'Sector2Ses
-00004b10: 7369 6f6e 5469 6d65 2729 2c0a 2020 2020  sionTime'),.    
-00004b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b40: 2020 2827 3227 2c20 2753 6563 746f 7233    ('2', 'Sector3
-00004b50: 5469 6d65 272c 2027 5365 6374 6f72 3353  Time', 'Sector3S
-00004b60: 6573 7369 6f6e 5469 6d65 2729 293a 0a20  essionTime')):. 
-00004b70: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00004b80: 6620 7661 6c20 3a3d 2072 6563 7572 7369  f val := recursi
-00004b90: 7665 5f64 6963 745f 6765 7428 7265 7370  ve_dict_get(resp
-00004ba0: 2c20 2753 6563 746f 7273 272c 2073 6e2c  , 'Sectors', sn,
-00004bb0: 2027 5661 6c75 6527 293a 0a20 2020 2020   'Value'):.     
-00004bc0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00004bd0: 7276 5f64 6174 615b 7365 6374 6f72 5d5b  rv_data[sector][
-00004be0: 6c61 7063 6e74 202d 206c 6170 5f6f 6666  lapcnt - lap_off
-00004bf0: 7365 745d 203d 2074 6f5f 7469 6d65 6465  set] = to_timede
-00004c00: 6c74 6128 7661 6c29 0a20 2020 2020 2020  lta(val).       
-00004c10: 2020 2020 2020 2020 2020 2020 2064 7276               drv
-00004c20: 5f64 6174 615b 7365 7373 745d 5b6c 6170  _data[sesst][lap
-00004c30: 636e 7420 2d20 6c61 705f 6f66 6673 6574  cnt - lap_offset
-00004c40: 5d20 3d20 746f 5f74 696d 6564 656c 7461  ] = to_timedelta
-00004c50: 2874 696d 6529 0a0a 2020 2020 2020 2020  (time)..        
-00004c60: 6966 2076 616c 203a 3d20 7265 6375 7273  if val := recurs
-00004c70: 6976 655f 6469 6374 5f67 6574 2872 6573  ive_dict_get(res
-00004c80: 702c 2027 4c61 7374 4c61 7054 696d 6527  p, 'LastLapTime'
-00004c90: 2c20 2756 616c 7565 2729 3a0a 2020 2020  , 'Value'):.    
-00004ca0: 2020 2020 2020 2020 2320 6966 2027 4c61          # if 'La
-00004cb0: 7374 4c61 7054 696d 6527 2069 7320 7265  stLapTime' is re
-00004cc0: 6365 6976 6564 206c 6573 7320 7468 616e  ceived less than
-00004cd0: 2066 6976 6520 7365 636f 6e64 7320 6166   five seconds af
-00004ce0: 7465 7220 7468 6520 7374 6172 7420 6f66  ter the start of
-00004cf0: 2061 206e 6577 206c 6170 2c20 6974 2069   a new lap, it i
-00004d00: 7320 7374 696c 6c20 6164 6465 640a 2020  s still added.  
-00004d10: 2020 2020 2020 2020 2020 2320 746f 2074            # to t
-00004d20: 6865 206c 6173 7420 6c61 700a 2020 2020  he last lap.    
-00004d30: 2020 2020 2020 2020 7661 6c20 3d20 746f          val = to
-00004d40: 5f74 696d 6564 656c 7461 2876 616c 290a  _timedelta(val).
-00004d50: 2020 2020 2020 2020 2020 2020 6966 2076              if v
-00004d60: 616c 2e74 6f74 616c 5f73 6563 6f6e 6473  al.total_seconds
-00004d70: 2829 203c 2031 3530 3a0a 2020 2020 2020  () < 150:.      
-00004d80: 2020 2020 2020 2020 2020 2320 6c61 7073            # laps
-00004d90: 2077 6869 6368 2061 7265 206c 6f6e 6765   which are longe
-00004da0: 7220 7468 616e 2031 3530 2073 6563 6f6e  r than 150 secon
-00004db0: 6473 2061 7265 2069 676e 6f72 6564 3b20  ds are ignored; 
-00004dc0: 7573 7561 6c6c 7920 7468 6973 2069 7320  usually this is 
-00004dd0: 7468 6520 6361 7365 2062 6574 7765 656e  the case between
-00004de0: 2051 312c 2051 3220 616e 6420 5133 0a20   Q1, Q2 and Q3. 
-00004df0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00004e00: 2062 6563 6175 7365 2061 6c6c 2074 6872   because all thr
-00004e10: 6565 2071 7561 6c69 6679 696e 6720 7365  ee qualifying se
-00004e20: 7373 696f 6e73 2061 7265 206f 6e65 2073  ssions are one s
-00004e30: 6573 7369 6f6e 2068 6572 652e 2054 686f  ession here. Tho
-00004e40: 7365 2074 696d 6573 7461 6d70 7320 6172  se timestamps ar
-00004e50: 6520 6f66 7465 6e20 7772 6f6e 6720 616e  e often wrong an
-00004e60: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-00004e70: 2020 2320 736f 6d65 7469 6d65 7320 6173    # sometimes as
-00004e80: 736f 6369 6174 6564 2077 6974 6820 7468  sociated with th
-00004e90: 6520 7772 6f6e 6720 6c61 700a 2020 2020  e wrong lap.    
-00004ea0: 2020 2020 2020 2020 2020 2020 6472 765f              drv_
-00004eb0: 6461 7461 5b27 4c61 7054 696d 6527 5d5b  data['LapTime'][
-00004ec0: 6c61 7063 6e74 202d 206c 6170 5f6f 6666  lapcnt - lap_off
-00004ed0: 7365 745d 203d 2076 616c 0a0a 2020 2020  set] = val..    
-00004ee0: 2020 2020 6966 2027 5370 6565 6473 2720      if 'Speeds' 
-00004ef0: 696e 2072 6573 703a 0a20 2020 2020 2020  in resp:.       
-00004f00: 2020 2020 2066 6f72 2074 7261 706b 6579       for trapkey
-00004f10: 2c20 7472 6170 6e61 6d65 2069 6e20 2828  , trapname in ((
-00004f20: 2749 3127 2c20 2753 7065 6564 4931 2729  'I1', 'SpeedI1')
-00004f30: 2c20 2827 4932 272c 2027 5370 6565 6449  , ('I2', 'SpeedI
-00004f40: 3227 292c 2028 2746 4c27 2c20 2753 7065  2'), ('FL', 'Spe
-00004f50: 6564 464c 2729 2c20 2827 5354 272c 2027  edFL'), ('ST', '
-00004f60: 5370 6565 6453 5427 2929 3a0a 2020 2020  SpeedST')):.    
-00004f70: 2020 2020 2020 2020 2020 2020 6966 2076              if v
-00004f80: 616c 203a 3d20 7265 6375 7273 6976 655f  al := recursive_
-00004f90: 6469 6374 5f67 6574 2872 6573 702c 2027  dict_get(resp, '
-00004fa0: 5370 6565 6473 272c 2074 7261 706b 6579  Speeds', trapkey
-00004fb0: 2c20 2756 616c 7565 2729 3a0a 2020 2020  , 'Value'):.    
-00004fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fd0: 2320 7370 6565 6420 6861 7320 746f 2062  # speed has to b
-00004fe0: 6520 666c 6f61 7420 6265 6361 7573 6520  e float because 
-00004ff0: 696e 7420 646f 6573 206e 6f74 2073 7570  int does not sup
-00005000: 706f 7274 204e 614e 0a20 2020 2020 2020  port NaN.       
-00005010: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00005020: 7472 6170 6b65 7920 3d3d 2027 5354 273a  trapkey == 'ST':
-00005030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005040: 2020 2020 2020 2020 2023 2074 6865 2053           # the S
-00005050: 5420 7472 6170 2076 616c 7565 2063 616e  T trap value can
-00005060: 206f 6363 7572 2065 6172 6c79 2065 6e6f   occur early eno
-00005070: 7567 6820 696e 2061 206e 6577 206c 6170  ugh in a new lap
-00005080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005090: 2020 2020 2020 2020 2023 2074 6861 7420           # that 
-000050a0: 6974 206e 6565 6473 2074 6f20 6265 2065  it needs to be e
-000050b0: 7863 6c75 6465 6420 6672 6f6d 2074 6865  xcluded from the
-000050c0: 2075 7375 616c 206f 6666 7365 740a 2020   usual offset.  
-000050d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050e0: 2020 2020 2020 2320 6c6f 6769 632c 2074        # logic, t
-000050f0: 6865 7265 666f 7265 2074 6865 206f 6666  herefore the off
-00005100: 7365 7420 6973 2069 676e 6f72 6564 2068  set is ignored h
-00005110: 6572 650a 2020 2020 2020 2020 2020 2020  ere.            
-00005120: 2020 2020 2020 2020 2020 2020 6472 765f              drv_
-00005130: 6461 7461 5b74 7261 706e 616d 655d 5b6c  data[trapname][l
-00005140: 6170 636e 745d 203d 2066 6c6f 6174 2876  apcnt] = float(v
-00005150: 616c 290a 2020 2020 2020 2020 2020 2020  al).            
-00005160: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00005170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005180: 2020 2020 2020 6472 765f 6461 7461 5b74        drv_data[t
-00005190: 7261 706e 616d 655d 5b6c 6170 636e 7420  rapname][lapcnt 
-000051a0: 2d20 6c61 705f 6f66 6673 6574 5d20 3d20  - lap_offset] = 
-000051b0: 666c 6f61 7428 7661 6c29 0a0a 2020 2020  float(val)..    
-000051c0: 2020 2020 6966 2027 496e 5069 7427 2069      if 'InPit' i
-000051d0: 6e20 7265 7370 3a0a 2020 2020 2020 2020  n resp:.        
-000051e0: 2020 2020 2320 2749 6e50 6974 273a 2054      # 'InPit': T
-000051f0: 7275 6520 6973 2072 6563 6569 7665 6420  rue is received 
-00005200: 6f6e 6365 2077 6865 6e20 656e 7465 7269  once when enteri
-00005210: 6e67 2070 6974 732c 2046 616c 7365 2069  ng pits, False i
-00005220: 7320 7265 6365 6976 6564 206f 6e63 6520  s received once 
-00005230: 7768 656e 206c 6561 7669 6e67 0a20 2020  when leaving.   
-00005240: 2020 2020 2020 2020 2069 6620 7265 7370           if resp
-00005250: 5b27 496e 5069 7427 5d20 6973 2054 7275  ['InPit'] is Tru
-00005260: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00005270: 2020 2069 6620 7069 7473 746f 7073 203e     if pitstops >
-00005280: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-00005290: 2020 2020 2020 2020 2064 7276 5f64 6174           drv_dat
-000052a0: 615b 2750 6974 496e 5469 6d65 275d 5b6c  a['PitInTime'][l
-000052b0: 6170 636e 745d 203d 2074 6f5f 7469 6d65  apcnt] = to_time
-000052c0: 6465 6c74 6128 7469 6d65 290a 2020 2020  delta(time).    
-000052d0: 2020 2020 2020 2020 656c 6966 2028 2828          elif (((
-000052e0: 274e 756d 6265 724f 664c 6170 7327 2069  'NumberOfLaps' i
-000052f0: 6e20 7265 7370 2920 616e 6420 7265 7370  n resp) and resp
-00005300: 5b27 4e75 6d62 6572 4f66 4c61 7073 275d  ['NumberOfLaps']
-00005310: 203e 2061 7069 5f6c 6170 636e 7429 0a20   > api_lapcnt). 
-00005320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005330: 206f 7220 2864 7276 5f64 6174 615b 2754   or (drv_data['T
-00005340: 696d 6527 5d5b 6c61 7063 6e74 5d20 2d20  ime'][lapcnt] - 
-00005350: 746f 5f74 696d 6564 656c 7461 2874 696d  to_timedelta(tim
-00005360: 6529 290a 2020 2020 2020 2020 2020 2020  e)).            
-00005370: 2020 2020 2020 3c20 7064 2e54 696d 6564        < pd.Timed
-00005380: 656c 7461 2835 2c20 2773 2729 293a 0a20  elta(5, 's')):. 
-00005390: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000053a0: 2073 616d 6520 7265 7370 6f6e 7365 206c   same response l
-000053b0: 696e 6520 6173 2062 6567 696e 6e69 6e67  ine as beginning
-000053c0: 206f 6620 6e65 7874 206c 6170 0a20 2020   of next lap.   
-000053d0: 2020 2020 2020 2020 2020 2020 2023 206f               # o
-000053e0: 7220 6265 6769 6e6e 696e 6720 6f66 206e  r beginning of n
-000053f0: 6578 7420 6c61 7020 6c65 7373 2074 6861  ext lap less tha
-00005400: 6e20 3520 7365 636f 6e64 7320 6177 6179  n 5 seconds away
-00005410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005420: 2064 7276 5f64 6174 615b 2750 6974 4f75   drv_data['PitOu
-00005430: 7454 696d 6527 5d5b 6c61 7063 6e74 202b  tTime'][lapcnt +
-00005440: 2031 5d20 3d20 746f 5f74 696d 6564 656c   1] = to_timedel
-00005450: 7461 2874 696d 6529 2020 2320 6164 6420  ta(time)  # add 
-00005460: 746f 206e 6578 7420 6c61 700a 2020 2020  to next lap.    
-00005470: 2020 2020 2020 2020 2020 2020 7069 7473              pits
-00005480: 746f 7073 202b 3d20 310a 2020 2020 2020  tops += 1.      
-00005490: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000054a0: 2020 2020 2020 2020 2020 2020 6472 765f              drv_
-000054b0: 6461 7461 5b27 5069 744f 7574 5469 6d65  data['PitOutTime
-000054c0: 275d 5b6c 6170 636e 745d 203d 2074 6f5f  '][lapcnt] = to_
-000054d0: 7469 6d65 6465 6c74 6128 7469 6d65 2920  timedelta(time) 
-000054e0: 2023 2061 6464 2074 6f20 6375 7272 656e   # add to curren
-000054f0: 7420 6c61 700a 2020 2020 2020 2020 2020  t lap.          
-00005500: 2020 2020 2020 7069 7473 746f 7073 202b        pitstops +
-00005510: 3d20 310a 0a20 2020 2020 2020 2023 2047  = 1..        # G
-00005520: 6574 2073 6176 6520 696e 666f 726d 6174  et save informat
-00005530: 696f 6e20 6162 6f75 7420 7065 7273 6f6e  ion about person
-00005540: 616c 2062 6573 7420 6c61 7020 7469 6d65  al best lap time
-00005550: 7320 6174 2074 6865 2074 696d 6573 7461  s at the timesta
-00005560: 6d70 0a20 2020 2020 2020 2023 2061 7420  mp.        # at 
-00005570: 7768 6963 6820 7468 6973 2069 6e66 6f72  which this infor
-00005580: 6d61 7469 6f6e 2077 6173 2072 6563 6569  mation was recei
-00005590: 7665 642e 0a20 2020 2020 2020 2023 2057  ved..        # W
-000055a0: 6865 6e65 7665 7220 6120 6c61 7020 6973  henever a lap is
-000055b0: 2064 656c 6574 6564 2028 6966 2074 6861   deleted (if tha
-000055c0: 7420 6861 7070 656e 7320 7175 6963 6b6c  t happens quickl
-000055d0: 7920 6166 7465 7220 6974 2077 6173 2073  y after it was s
-000055e0: 6574 292c 0a20 2020 2020 2020 2023 2074  et),.        # t
-000055f0: 6865 2070 7265 7669 6f75 7320 2742 6573  he previous 'Bes
-00005600: 744c 6170 5469 6d65 2720 7661 6c75 6520  tLapTime' value 
-00005610: 6973 2073 656e 7420 6167 6169 6e2e 2054  is sent again. T
-00005620: 6865 7265 2069 7320 736f 6d65 2065 7874  here is some ext
-00005630: 7261 0a20 2020 2020 2020 2023 206c 6f67  ra.        # log
-00005640: 6963 2061 7420 7468 656e 2065 6e64 2074  ic at then end t
-00005650: 6861 7420 636f 7272 6563 746c 7920 6d61  hat correctly ma
-00005660: 726b 7320 7065 7273 6f6e 616c 2062 6573  rks personal bes
-00005670: 7420 6c61 7073 2062 6173 6564 206f 6e0a  t laps based on.
-00005680: 2020 2020 2020 2020 2320 7468 6520 6461          # the da
-00005690: 7461 2074 6861 7420 6973 2073 6176 6564  ta that is saved
-000056a0: 2068 6572 652e 0a20 2020 2020 2020 2069   here..        i
-000056b0: 6620 7661 6c20 3a3d 2072 6563 7572 7369  f val := recursi
-000056c0: 7665 5f64 6963 745f 6765 7428 7265 7370  ve_dict_get(resp
-000056d0: 2c20 2742 6573 744c 6170 5469 6d65 272c  , 'BestLapTime',
-000056e0: 2027 5661 6c75 6527 293a 0a20 2020 2020   'Value'):.     
-000056f0: 2020 2020 2020 2070 6572 736f 6e61 6c5f         personal_
-00005700: 6265 7374 5f6c 6170 5f74 696d 6573 2e61  best_lap_times.a
-00005710: 7070 656e 6428 0a20 2020 2020 2020 2020  ppend(.         
-00005720: 2020 2020 2020 2028 746f 5f74 696d 6564         (to_timed
-00005730: 656c 7461 2874 696d 6529 2c20 746f 5f74  elta(time), to_t
-00005740: 696d 6564 656c 7461 2876 616c 2929 0a20  imedelta(val)). 
-00005750: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00005760: 2020 2020 2020 2320 4372 6561 7465 2061        # Create a
-00005770: 7070 726f 7869 6d61 7465 2028 7375 6229  pproximate (sub)
-00005780: 7365 7373 696f 6e20 2869 2e65 2e20 7175  session (i.e. qu
-00005790: 616c 6929 2073 706c 6974 2074 696d 6573  ali) split times
-000057a0: 2062 790a 2020 2020 2020 2020 2320 286d   by.        # (m
-000057b0: 6973 2975 7369 6e67 2074 6865 2073 6573  is)using the ses
-000057c0: 7369 6f6e 206e 756d 6265 7220 636f 756e  sion number coun
-000057d0: 7465 7220 6672 6f6d 2027 4265 7374 4c61  ter from 'BestLa
-000057e0: 7054 696d 6573 272e 0a20 2020 2020 2020  pTimes'..       
-000057f0: 2023 2028 4e6f 7465 3a20 7468 6f73 6520   # (Note: those 
-00005800: 6c61 7020 7469 6d65 7320 6361 6e6e 6f74  lap times cannot
-00005810: 2062 6520 7573 6564 2066 6f72 2063 6f72   be used for cor
-00005820: 7265 6374 2070 6572 736f 6e61 6c20 6265  rect personal be
-00005830: 7374 0a20 2020 2020 2020 2023 2020 6465  st.        #  de
-00005840: 7465 6374 696f 6e2c 2062 6563 6175 7365  tection, because
-00005850: 2074 6865 2070 7265 7669 6f75 7320 7661   the previous va
-00005860: 6c75 6520 6973 206e 6f74 2072 6573 656e  lue is not resen
-00005870: 7420 6865 7265 2077 6865 6e20 6120 6c61  t here when a la
-00005880: 700a 2020 2020 2020 2020 2320 2069 7320  p.        #  is 
-00005890: 6465 6c65 7465 642e 290a 2020 2020 2020  deleted.).      
-000058a0: 2020 6966 2028 7661 6c20 3a3d 2072 6573    if (val := res
-000058b0: 702e 6765 7428 2742 6573 744c 6170 5469  p.get('BestLapTi
-000058c0: 6d65 7327 2929 2061 6e64 2069 7369 6e73  mes')) and isins
-000058d0: 7461 6e63 6528 7661 6c2c 2064 6963 7429  tance(val, dict)
-000058e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000058f0: 7373 696f 6e5f 6e20 3d20 696e 7428 6c69  ssion_n = int(li
-00005900: 7374 2876 616c 2e6b 6579 7328 2929 5b30  st(val.keys())[0
-00005910: 5d29 0a20 2020 2020 2020 2020 2020 2069  ]).            i
-00005920: 6620 2873 6573 7369 6f6e 5f6e 202b 2031  f (session_n + 1
-00005930: 2920 3e20 6c65 6e28 7365 7373 696f 6e5f  ) > len(session_
-00005940: 7370 6c69 745f 7469 6d65 7329 3a0a 2020  split_times):.  
-00005950: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00005960: 7373 696f 6e5f 7370 6c69 745f 7469 6d65  ssion_split_time
-00005970: 732e 6170 7065 6e64 2874 6f5f 7469 6d65  s.append(to_time
-00005980: 6465 6c74 6128 7469 6d65 2929 0a0a 2020  delta(time))..  
-00005990: 2020 2020 2020 2320 6e65 7720 6c61 703b        # new lap;
-000059a0: 2063 7265 6174 6520 6e65 7874 2072 6f77   create next row
-000059b0: 0a20 2020 2020 2020 2069 6620 274e 756d  .        if 'Num
-000059c0: 6265 724f 664c 6170 7327 2069 6e20 7265  berOfLaps' in re
-000059d0: 7370 2061 6e64 2072 6573 705b 274e 756d  sp and resp['Num
-000059e0: 6265 724f 664c 6170 7327 5d20 3e20 6170  berOfLaps'] > ap
-000059f0: 695f 6c61 7063 6e74 3a0a 2020 2020 2020  i_lapcnt:.      
-00005a00: 2020 2020 2020 6170 695f 6c61 7063 6e74        api_lapcnt
-00005a10: 202b 3d20 310a 2020 2020 2020 2020 2020   += 1.          
-00005a20: 2020 2320 6d61 6b65 2073 7572 6520 7468    # make sure th
-00005a30: 6520 6361 7220 6163 7475 616c 6c79 2064  e car actually d
-00005a40: 726f 7665 206f 7574 206f 6620 7468 6520  rove out of the 
-00005a50: 7069 7473 2061 6c72 6561 6479 3b20 6974  pits already; it
-00005a60: 2063 616e 2774 2062 6520 6120 6e65 7720   can't be a new 
-00005a70: 6c61 7020 6966 2069 7420 6469 646e 2774  lap if it didn't
-00005a80: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00005a90: 7069 7473 746f 7073 203e 3d20 303a 0a20  pitstops >= 0:. 
-00005aa0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00005ab0: 7276 5f64 6174 615b 2754 696d 6527 5d5b  rv_data['Time'][
-00005ac0: 6c61 7063 6e74 5d20 3d20 746f 5f74 696d  lapcnt] = to_tim
-00005ad0: 6564 656c 7461 2874 696d 6529 0a20 2020  edelta(time).   
-00005ae0: 2020 2020 2020 2020 2020 2020 2064 7276               drv
-00005af0: 5f64 6174 615b 274e 756d 6265 724f 664c  _data['NumberOfL
-00005b00: 6170 7327 5d5b 6c61 7063 6e74 5d20 3d20  aps'][lapcnt] = 
-00005b10: 6c61 7063 6e74 202b 2031 2020 2320 646f  lapcnt + 1  # do
-00005b20: 6e27 7420 7573 6520 4631 2773 206c 6170  n't use F1's lap
-00005b30: 2063 6f75 6e74 3b20 6f75 7273 2069 7320   count; ours is 
-00005b40: 6265 7474 6572 0a20 2020 2020 2020 2020  better.         
-00005b50: 2020 2020 2020 2064 7276 5f64 6174 615b         drv_data[
-00005b60: 274e 756d 6265 724f 6650 6974 5374 6f70  'NumberOfPitStop
-00005b70: 7327 5d5b 6c61 7063 6e74 5d20 3d20 7069  s'][lapcnt] = pi
-00005b80: 7473 746f 7073 0a20 2020 2020 2020 2020  tstops.         
-00005b90: 2020 2020 2020 2064 7276 5f64 6174 615b         drv_data[
-00005ba0: 2744 7269 7665 7227 5d5b 6c61 7063 6e74  'Driver'][lapcnt
-00005bb0: 5d20 3d20 6472 760a 2020 2020 2020 2020  ] = drv.        
-00005bc0: 2020 2020 2020 2020 6c61 7063 6e74 202b          lapcnt +
-00005bd0: 3d20 310a 0a20 2020 2069 6620 6c61 7063  = 1..    if lapc
-00005be0: 6e74 203d 3d20 303a 2020 2320 6e6f 2064  nt == 0:  # no d
-00005bf0: 6174 6120 6174 2061 6c6c 2066 6f72 2074  ata at all for t
-00005c00: 6869 7320 6472 6976 6572 0a20 2020 2020  his driver.     
-00005c10: 2020 2072 6574 7572 6e20 4e6f 6e65 2c20     return None, 
-00005c20: 4e6f 6e65 0a0a 2020 2020 2320 646f 6e65  None..    # done
-00005c30: 2072 6561 6469 6e67 2074 6865 2064 6174   reading the dat
-00005c40: 612c 2064 6f20 706f 7374 7072 6f63 6573  a, do postproces
-00005c50: 7369 6e67 0a0a 2020 2020 6465 6620 6461  sing..    def da
-00005c60: 7461 5f69 6e5f 6c61 7028 6c61 705f 6e29  ta_in_lap(lap_n)
-00005c70: 3a0a 2020 2020 2020 2020 7265 6c65 7661  :.        releva
-00005c80: 6e74 203d 2028 2753 6563 746f 7231 5469  nt = ('Sector1Ti
-00005c90: 6d65 272c 2027 5365 6374 6f72 3254 696d  me', 'Sector2Tim
-00005ca0: 6527 2c20 2753 6563 746f 7233 5469 6d65  e', 'Sector3Time
-00005cb0: 272c 2027 5370 6565 6449 3127 2c20 2753  ', 'SpeedI1', 'S
-00005cc0: 7065 6564 4932 272c 0a20 2020 2020 2020  peedI2',.       
-00005cd0: 2020 2020 2020 2020 2020 2020 2027 5370               'Sp
-00005ce0: 6565 6446 4c27 2c20 2753 7065 6564 5354  eedFL', 'SpeedST
-00005cf0: 272c 2027 4c61 7054 696d 6527 290a 2020  ', 'LapTime').  
-00005d00: 2020 2020 2020 666f 7220 636f 6c20 696e        for col in
-00005d10: 2072 656c 6576 616e 743a 0a20 2020 2020   relevant:.     
-00005d20: 2020 2020 2020 2069 6620 6e6f 7420 7064         if not pd
-00005d30: 2e69 736e 756c 6c28 6472 765f 6461 7461  .isnull(drv_data
-00005d40: 5b63 6f6c 5d5b 6c61 705f 6e5d 293a 0a20  [col][lap_n]):. 
-00005d50: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00005d60: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
-00005d70: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00005d80: 0a20 2020 2023 2027 4e75 6d62 6572 4f66  .    # 'NumberOf
-00005d90: 4c61 7073 2720 616c 7761 7973 2069 6e74  Laps' always int
-00005da0: 726f 6475 6365 7320 6120 6e65 7720 6c61  roduces a new la
-00005db0: 7020 2863 616e 2062 6520 6120 7072 6576  p (can be a prev
-00005dc0: 696f 7573 206f 6e65 2920 6275 7420 736f  ious one) but so
-00005dd0: 6d65 7469 6d65 7320 7468 6572 6520 6973  metimes there is
-00005de0: 206f 6e65 206d 6f72 6520 6c61 7020 6174   one more lap at
-00005df0: 2074 6865 2065 6e64 0a20 2020 2023 2069   the end.    # i
-00005e00: 6e20 7468 6973 2063 6173 6520 7468 6520  n this case the 
-00005e10: 6461 7461 2077 696c 6c20 6265 2061 6464  data will be add
-00005e20: 6564 2061 7320 7573 7561 6c20 6162 6f76  ed as usual abov
-00005e30: 652c 206c 6170 2063 6f75 6e74 2061 6e64  e, lap count and
-00005e40: 2070 6974 2073 746f 7073 2061 7265 2061   pit stops are a
-00005e50: 6464 6564 2068 6572 6520 616e 6420 7468  dded here and th
-00005e60: 6520 2754 696d 6527 2069 730a 2020 2020  e 'Time' is.    
-00005e70: 2320 6361 6c63 756c 6174 6564 2062 656c  # calculated bel
-00005e80: 6f77 2066 726f 6d20 7365 6374 6f72 2074  ow from sector t
-00005e90: 696d 6573 0a20 2020 2069 6620 6461 7461  imes.    if data
-00005ea0: 5f69 6e5f 6c61 7028 6c61 7063 6e74 293a  _in_lap(lapcnt):
-00005eb0: 0a20 2020 2020 2020 2064 7276 5f64 6174  .        drv_dat
-00005ec0: 615b 274e 756d 6265 724f 664c 6170 7327  a['NumberOfLaps'
-00005ed0: 5d5b 6c61 7063 6e74 5d20 3d20 6c61 7063  ][lapcnt] = lapc
-00005ee0: 6e74 202b 2031 0a20 2020 2020 2020 2064  nt + 1.        d
-00005ef0: 7276 5f64 6174 615b 274e 756d 6265 724f  rv_data['NumberO
-00005f00: 6650 6974 5374 6f70 7327 5d5b 6c61 7063  fPitStops'][lapc
-00005f10: 6e74 5d20 3d20 7069 7473 746f 7073 0a20  nt] = pitstops. 
-00005f20: 2020 2020 2020 2064 7276 5f64 6174 615b         drv_data[
-00005f30: 2744 7269 7665 7227 5d5b 6c61 7063 6e74  'Driver'][lapcnt
-00005f40: 5d20 3d20 6472 760a 2020 2020 656c 7365  ] = drv.    else
-00005f50: 3a20 2023 2069 6620 7468 6572 6520 7761  :  # if there wa
-00005f60: 7320 6e6f 206d 6f72 6520 6461 7461 2061  s no more data a
-00005f70: 6674 6572 2074 6865 206c 6173 7420 6c61  fter the last la
-00005f80: 7020 636f 756e 7420 696e 6372 6561 7365  p count increase
-00005f90: 2c0a 2020 2020 2020 2020 2320 6465 6c65  ,.        # dele
-00005fa0: 7465 2074 6865 206c 6173 7420 656d 7074  te the last empt
-00005fb0: 7920 7265 636f 7264 0a20 2020 2020 2020  y record.       
-00005fc0: 2066 6f72 206b 6579 2069 6e20 6472 765f   for key in drv_
-00005fd0: 6461 7461 2e6b 6579 7328 293a 0a20 2020  data.keys():.   
-00005fe0: 2020 2020 2020 2020 2064 7276 5f64 6174           drv_dat
-00005ff0: 615b 6b65 795d 203d 2064 7276 5f64 6174  a[key] = drv_dat
-00006000: 615b 6b65 795d 5b3a 2d31 5d0a 2020 2020  a[key][:-1].    
-00006010: 6966 206e 6f74 2064 6174 615f 696e 5f6c  if not data_in_l
-00006020: 6170 2830 293a 2020 2320 7265 6d6f 7665  ap(0):  # remove
-00006030: 2066 6972 7374 206c 6170 2069 6620 7468   first lap if th
-00006040: 6572 6527 7320 6e6f 2064 6174 613b 0a20  ere's no data;. 
-00006050: 2020 2020 2020 2023 2022 7073 6575 646f         # "pseudo
-00006060: 206f 7574 6c61 7022 2074 6861 7420 6469   outlap" that di
-00006070: 646e 2774 2065 7869 7374 0a20 2020 2020  dn't exist.     
-00006080: 2020 2066 6f72 206b 6579 2069 6e20 6472     for key in dr
-00006090: 765f 6461 7461 2e6b 6579 7328 293a 0a20  v_data.keys():. 
-000060a0: 2020 2020 2020 2020 2020 2064 7276 5f64             drv_d
-000060b0: 6174 615b 6b65 795d 203d 2064 7276 5f64  ata[key] = drv_d
-000060c0: 6174 615b 6b65 795d 5b31 3a5d 0a20 2020  ata[key][1:].   
-000060d0: 2020 2020 2064 7276 5f64 6174 615b 274e       drv_data['N
-000060e0: 756d 6265 724f 664c 6170 7327 5d20 3d20  umberOfLaps'] = 
-000060f0: 6c69 7374 286d 6170 286c 616d 6264 6120  list(map(lambda 
-00006100: 6e3a 206e 202d 2031 2c20 6472 765f 6461  n: n - 1, drv_da
-00006110: 7461 5b27 4e75 6d62 6572 4f66 4c61 7073  ta['NumberOfLaps
-00006120: 275d 2929 2020 2320 7265 6475 6365 2065  ']))  # reduce e
-00006130: 6163 6820 6c61 7020 636f 756e 7420 6279  ach lap count by
-00006140: 206f 6e65 0a0a 2020 2020 6966 206e 6f74   one..    if not
-00006150: 2064 7276 5f64 6174 615b 2754 696d 6527   drv_data['Time'
-00006160: 5d3a 0a20 2020 2020 2020 2023 2065 6e73  ]:.        # ens
-00006170: 7572 6520 7468 6174 2074 6865 7265 2069  ure that there i
-00006180: 7320 7374 696c 6c20 6461 7461 206c 6566  s still data lef
-00006190: 7420 6166 7465 7220 706f 7465 6e74 6961  t after potentia
-000061a0: 6c6c 7920 7265 6d6f 7669 6e67 2061 206c  lly removing a l
-000061b0: 6170 0a20 2020 2020 2020 2072 6574 7572  ap.        retur
-000061c0: 6e20 6472 765f 6461 7461 2c20 7365 7373  n drv_data, sess
-000061d0: 696f 6e5f 7370 6c69 745f 7469 6d65 730a  ion_split_times.
-000061e0: 0a20 2020 2066 6f72 2069 2069 6e20 7261  .    for i in ra
-000061f0: 6e67 6528 6c65 6e28 6472 765f 6461 7461  nge(len(drv_data
-00006200: 5b27 5469 6d65 275d 2929 3a0a 2020 2020  ['Time'])):.    
-00006210: 2020 2020 7365 6374 6f72 5f73 756d 203d      sector_sum =
-00006220: 2064 6174 6574 696d 652e 7469 6d65 6465   datetime.timede
-00006230: 6c74 6128 3029 0a20 2020 2020 2020 206e  lta(0).        n
-00006240: 615f 7365 6374 6f72 7320 3d20 6c69 7374  a_sectors = list
-00006250: 2829 2020 2320 6c69 7374 206f 6620 6b65  ()  # list of ke
-00006260: 7973 2066 6f72 206d 6973 7369 6e67 2073  ys for missing s
-00006270: 6563 746f 7220 7469 6d65 730a 2020 2020  ector times.    
-00006280: 2020 2020 666f 7220 6b65 7920 696e 2028      for key in (
-00006290: 2753 6563 746f 7231 5469 6d65 272c 2027  'Sector1Time', '
-000062a0: 5365 6374 6f72 3254 696d 6527 2c20 2753  Sector2Time', 'S
-000062b0: 6563 746f 7233 5469 6d65 2729 3a0a 2020  ector3Time'):.  
-000062c0: 2020 2020 2020 2020 2020 7374 203d 2064            st = d
-000062d0: 7276 5f64 6174 615b 6b65 795d 5b69 5d0a  rv_data[key][i].
-000062e0: 2020 2020 2020 2020 2020 2020 6966 2070              if p
-000062f0: 642e 6973 6e61 2873 7429 3a0a 2020 2020  d.isna(st):.    
-00006300: 2020 2020 2020 2020 2020 2020 6e61 5f73              na_s
-00006310: 6563 746f 7273 2e61 7070 656e 6428 6b65  ectors.append(ke
-00006320: 7929 0a20 2020 2020 2020 2020 2020 2020  y).             
-00006330: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
-00006340: 2020 2020 2020 2020 7365 6374 6f72 5f73          sector_s
-00006350: 756d 202b 3d20 7374 0a0a 2020 2020 2020  um += st..      
-00006360: 2020 2320 6368 6563 6b20 666f 7220 696e    # check for in
-00006370: 636f 7272 6563 7420 6c61 7020 7469 6d65  correct lap time
-00006380: 7320 616e 6420 7265 6d6f 7665 2074 6865  s and remove the
-00006390: 6d0a 2020 2020 2020 2020 2320 6669 7865  m.        # fixe
-000063a0: 7320 4748 2331 3637 2061 6d6f 6e67 206f  s GH#167 among o
-000063b0: 7468 6572 730a 2020 2020 2020 2020 6966  thers.        if
-000063c0: 2073 6563 746f 725f 7375 6d20 3e20 6472   sector_sum > dr
-000063d0: 765f 6461 7461 5b27 4c61 7054 696d 6527  v_data['LapTime'
-000063e0: 5d5b 695d 3a0a 2020 2020 2020 2020 2020  ][i]:.          
-000063f0: 2020 6472 765f 6461 7461 5b27 4c61 7054    drv_data['LapT
-00006400: 696d 6527 5d5b 695d 203d 2070 642e 4e61  ime'][i] = pd.Na
-00006410: 540a 2020 2020 2020 2020 2020 2020 696e  T.            in
-00006420: 7465 6772 6974 795f 6572 726f 7273 2e61  tegrity_errors.a
-00006430: 7070 656e 6428 6920 2b20 3129 0a0a 2020  ppend(i + 1)..  
-00006440: 2020 2020 2020 6966 2069 203d 3d20 303a        if i == 0:
-00006450: 0a20 2020 2020 2020 2020 2020 2023 206f  .            # o
-00006460: 6e6c 7920 646f 2066 6f6c 6c6f 7769 6e67  nly do following
-00006470: 2063 6f72 7265 6374 696f 6e73 2066 6f72   corrections for
-00006480: 2032 6e64 206c 6170 2061 6e64 206f 6e77   2nd lap and onw
-00006490: 6172 6473 0a20 2020 2020 2020 2020 2020  ards.           
-000064a0: 2063 6f6e 7469 6e75 650a 0a20 2020 2020   continue..     
-000064b0: 2020 2023 2054 6865 2041 5049 206f 6e6c     # The API onl
-000064c0: 7920 7365 6e64 7320 616e 6420 7570 6461  y sends and upda
-000064d0: 7465 2069 6620 6120 7374 6174 6520 6368  te if a state ch
-000064e0: 616e 6765 732c 2074 6865 7265 666f 7265  anges, therefore
-000064f0: 2c20 6966 2074 776f 0a20 2020 2020 2020  , if two.       
-00006500: 2023 206c 6170 2074 696d 6573 206f 7220   # lap times or 
-00006510: 7365 6374 6f72 2074 696d 6573 2061 7265  sector times are
-00006520: 2065 7861 6374 6c79 2065 7175 616c 2c20   exactly equal, 
-00006530: 7468 6520 7365 636f 6e64 2076 616c 7565  the second value
-00006540: 2077 696c 6c0a 2020 2020 2020 2020 2320   will.        # 
-00006550: 6265 206d 6973 7369 6e67 2e20 4d69 7373  be missing. Miss
-00006560: 696e 6720 7365 6374 6f72 2074 696d 6573  ing sector times
-00006570: 2061 6e64 206c 6170 2074 696d 6573 2061   and lap times a
-00006580: 7265 2063 616c 6375 6c61 7465 6420 6865  re calculated he
-00006590: 7265 0a20 2020 2020 2020 2023 2062 6173  re.        # bas
-000065a0: 6564 206f 6e20 7468 6520 6176 6169 6c61  ed on the availa
-000065b0: 626c 6520 7661 6c75 6573 2066 6f72 2061  ble values for a
-000065c0: 206c 6170 2028 6d61 7820 6f6e 6520 6d61   lap (max one ma
-000065d0: 7920 6265 206d 6973 7369 6e67 292e 2049  y be missing). I
-000065e0: 660a 2020 2020 2020 2020 2320 7468 6520  f.        # the 
-000065f0: 6361 6c63 756c 6174 6564 2076 616c 7565  calculated value
-00006600: 206d 6174 6368 6573 2074 6865 2070 7265   matches the pre
-00006610: 7669 6f75 7320 7661 6c75 652c 2069 7420  vious value, it 
-00006620: 7769 6c6c 2062 6520 7365 742e 0a0a 2020  will be set...  
-00006630: 2020 2020 2020 2320 6c61 7020 7469 6d65        # lap time
-00006640: 2069 7320 6d69 7373 696e 670a 2020 2020   is missing.    
-00006650: 2020 2020 6966 2028 6e6f 7420 6e61 5f73      if (not na_s
-00006660: 6563 746f 7273 2920 616e 6420 7064 2e69  ectors) and pd.i
-00006670: 736e 6128 6472 765f 6461 7461 5b27 4c61  sna(drv_data['La
-00006680: 7054 696d 6527 5d5b 695d 2920 5c0a 2020  pTime'][i]) \.  
-00006690: 2020 2020 2020 2020 2020 2020 2020 616e                an
-000066a0: 6420 2864 7276 5f64 6174 615b 274c 6170  d (drv_data['Lap
-000066b0: 5469 6d65 275d 5b69 202d 2031 5d20 3d3d  Time'][i - 1] ==
-000066c0: 2073 6563 746f 725f 7375 6d29 3a0a 0a20   sector_sum):.. 
-000066d0: 2020 2020 2020 2020 2020 2064 7276 5f64             drv_d
-000066e0: 6174 615b 274c 6170 5469 6d65 275d 5b69  ata['LapTime'][i
-000066f0: 5d20 3d20 7365 6374 6f72 5f73 756d 0a0a  ] = sector_sum..
-00006700: 2020 2020 2020 2020 2320 6f6e 6520 7365          # one se
-00006710: 6374 6f72 2074 696d 6520 6973 206d 6973  ctor time is mis
-00006720: 7369 6e67 0a20 2020 2020 2020 2065 6c69  sing.        eli
-00006730: 6620 286c 656e 286e 615f 7365 6374 6f72  f (len(na_sector
-00006740: 7329 203d 3d20 3129 2061 6e64 206e 6f74  s) == 1) and not
-00006750: 2070 642e 6973 6e61 2864 7276 5f64 6174   pd.isna(drv_dat
-00006760: 615b 274c 6170 5469 6d65 275d 5b69 5d29  a['LapTime'][i])
-00006770: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00006780: 6372 6561 7465 2061 206c 6973 7420 7769  create a list wi
-00006790: 7468 2074 6865 2074 776f 206b 6579 7320  th the two keys 
-000067a0: 666f 7220 6176 6169 6c61 626c 6520 7365  for available se
-000067b0: 6374 6f72 2074 696d 6573 0a20 2020 2020  ctor times.     
-000067c0: 2020 2020 2020 2072 6566 5f73 6563 203d         ref_sec =
-000067d0: 205b 2753 6563 746f 7231 5469 6d65 272c   ['Sector1Time',
-000067e0: 2027 5365 6374 6f72 3254 696d 6527 2c20   'Sector2Time', 
-000067f0: 2753 6563 746f 7233 5469 6d65 275d 0a20  'Sector3Time']. 
-00006800: 2020 2020 2020 2020 2020 2072 6566 5f73             ref_s
-00006810: 6563 2e72 656d 6f76 6528 6e61 5f73 6563  ec.remove(na_sec
-00006820: 746f 7273 5b30 5d29 0a0a 2020 2020 2020  tors[0])..      
-00006830: 2020 2020 2020 6966 2028 7365 6331 203a        if (sec1 :
-00006840: 3d20 2864 7276 5f64 6174 615b 274c 6170  = (drv_data['Lap
-00006850: 5469 6d65 275d 5b69 5d0a 2020 2020 2020  Time'][i].      
-00006860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006870: 2020 202d 2064 7276 5f64 6174 615b 7265     - drv_data[re
-00006880: 665f 7365 635b 305d 5d5b 695d 0a20 2020  f_sec[0]][i].   
-00006890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068a0: 2020 2020 2020 2d20 6472 765f 6461 7461        - drv_data
-000068b0: 5b72 6566 5f73 6563 5b31 5d5d 5b69 5d29  [ref_sec[1]][i])
-000068c0: 2920 5c0a 2020 2020 2020 2020 2020 2020  ) \.            
-000068d0: 2020 2020 2020 2020 3d3d 2064 7276 5f64          == drv_d
-000068e0: 6174 615b 6e61 5f73 6563 746f 7273 5b30  ata[na_sectors[0
-000068f0: 5d5d 5b69 202d 2031 5d3a 0a0a 2020 2020  ]][i - 1]:..    
-00006900: 2020 2020 2020 2020 2020 2020 6472 765f              drv_
-00006910: 6461 7461 5b6e 615f 7365 6374 6f72 735b  data[na_sectors[
-00006920: 305d 5d5b 695d 203d 2073 6563 310a 0a20  0]][i] = sec1.. 
-00006930: 2020 2023 206c 6170 2074 696d 6520 7379     # lap time sy
-00006940: 6e63 3b20 6368 6563 6b20 7768 6963 6820  nc; check which 
-00006950: 7365 6374 6f72 2074 696d 6520 7761 7320  sector time was 
-00006960: 7472 6967 6765 7265 6420 7769 7468 2074  triggered with t
-00006970: 6865 206c 6f77 6573 7420 6c61 7465 6e63  he lowest latenc
-00006980: 790a 2020 2020 2320 5365 6374 6f72 3353  y.    # Sector3S
-00006990: 6573 7369 6f6e 5469 6d65 203d 3d20 656e  essionTime == en
-000069a0: 6420 6f66 206c 6170 0a20 2020 2023 2053  d of lap.    # S
-000069b0: 6563 746f 7232 5365 7373 696f 6e54 696d  ector2SessionTim
-000069c0: 6520 2b20 5365 6374 6f72 3354 696d 6520  e + Sector3Time 
-000069d0: 3d3d 2065 6e64 206f 6620 6c61 700a 2020  == end of lap.  
-000069e0: 2020 2320 5365 6374 6f72 3153 6573 7369    # Sector1Sessi
-000069f0: 6f6e 5469 6d65 202b 2053 6563 746f 7232  onTime + Sector2
-00006a00: 5469 6d65 202b 2053 6563 746f 7233 5469  Time + Sector3Ti
-00006a10: 6d65 203d 3d20 656e 6420 6f66 206c 6170  me == end of lap
-00006a20: 0a20 2020 2023 2061 6c6c 206f 6620 7468  .    # all of th
-00006a30: 6573 6520 7468 7265 6520 6861 7665 2073  ese three have s
-00006a40: 6c69 6768 746c 7920 6469 6666 6572 656e  lightly differen
-00006a50: 7420 7469 6d65 733b 2074 616b 6520 6561  t times; take ea
-00006a60: 726c 6965 7374 206f 6e65 202d 3e20 6d6f  rliest one -> mo
-00006a70: 7374 2065 7861 6374 2062 6563 6175 7365  st exact because
-00006a80: 2063 616e 2774 2074 7269 6767 6572 2074   can't trigger t
-00006a90: 6f6f 2065 6172 6c79 0a20 2020 2066 6f72  oo early.    for
-00006aa0: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
-00006ab0: 6472 765f 6461 7461 5b27 5469 6d65 275d  drv_data['Time']
-00006ac0: 2929 3a0a 2020 2020 2020 2020 7365 6374  )):.        sect
-00006ad0: 6f72 5f73 756d 203d 2070 642e 5469 6d65  or_sum = pd.Time
-00006ae0: 6465 6c74 6128 3029 0a20 2020 2020 2020  delta(0).       
-00006af0: 206d 696e 5f74 696d 6520 3d20 6472 765f   min_time = drv_
-00006b00: 6461 7461 5b27 5469 6d65 275d 5b69 5d0a  data['Time'][i].
-00006b10: 2020 2020 2020 2020 666f 7220 7365 6374          for sect
-00006b20: 6f72 5f74 696d 652c 2073 6573 7369 6f6e  or_time, session
-00006b30: 5f74 696d 6520 696e 2028 2870 642e 5469  _time in ((pd.Ti
-00006b40: 6d65 6465 6c74 6128 3029 2c20 6472 765f  medelta(0), drv_
-00006b50: 6461 7461 5b27 5365 6374 6f72 3353 6573  data['Sector3Ses
-00006b60: 7369 6f6e 5469 6d65 275d 5b69 5d29 2c0a  sionTime'][i]),.
-00006b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b90: 2020 2020 2020 2020 2020 2864 7276 5f64            (drv_d
-00006ba0: 6174 615b 2753 6563 746f 7233 5469 6d65  ata['Sector3Time
-00006bb0: 275d 5b69 5d2c 2064 7276 5f64 6174 615b  '][i], drv_data[
-00006bc0: 2753 6563 746f 7232 5365 7373 696f 6e54  'Sector2SessionT
-00006bd0: 696d 6527 5d5b 695d 292c 0a20 2020 2020  ime'][i]),.     
-00006be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c00: 2020 2020 2028 6472 765f 6461 7461 5b27       (drv_data['
-00006c10: 5365 6374 6f72 3254 696d 6527 5d5b 695d  Sector2Time'][i]
-00006c20: 2c20 6472 765f 6461 7461 5b27 5365 6374  , drv_data['Sect
-00006c30: 6f72 3153 6573 7369 6f6e 5469 6d65 275d  or1SessionTime']
-00006c40: 5b69 5d29 293a 0a20 2020 2020 2020 2020  [i])):.         
-00006c50: 2020 2069 6620 7064 2e69 736e 756c 6c28     if pd.isnull(
-00006c60: 7365 7373 696f 6e5f 7469 6d65 293a 0a20  session_time):. 
-00006c70: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00006c80: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
-00006c90: 2020 2020 6966 2070 642e 6973 6e75 6c6c      if pd.isnull
-00006ca0: 2873 6563 746f 725f 7469 6d65 293a 0a20  (sector_time):. 
-00006cb0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00006cc0: 7265 616b 2020 2320 6e65 6564 2074 6f20  reak  # need to 
-00006cd0: 7374 6f70 2068 6572 6520 6265 6361 7573  stop here becaus
-00006ce0: 6520 656c 7365 2074 6865 2073 6563 746f  e else the secto
-00006cf0: 7220 7375 6d20 7769 6c6c 2062 6520 696e  r sum will be in
-00006d00: 636f 7272 6563 740a 0a20 2020 2020 2020  correct..       
-00006d10: 2020 2020 2073 6563 746f 725f 7375 6d20       sector_sum 
-00006d20: 2b3d 2073 6563 746f 725f 7469 6d65 0a20  += sector_time. 
-00006d30: 2020 2020 2020 2020 2020 206e 6577 5f74             new_t
-00006d40: 696d 6520 3d20 7365 7373 696f 6e5f 7469  ime = session_ti
-00006d50: 6d65 202b 2073 6563 746f 725f 7375 6d0a  me + sector_sum.
-00006d60: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00006d70: 6f74 2070 642e 6973 6e75 6c6c 286e 6577  ot pd.isnull(new
-00006d80: 5f74 696d 6529 2061 6e64 2028 6e65 775f  _time) and (new_
-00006d90: 7469 6d65 203c 206d 696e 5f74 696d 6520  time < min_time 
-00006da0: 6f72 2070 642e 6973 6e75 6c6c 286d 696e  or pd.isnull(min
-00006db0: 5f74 696d 6529 293a 0a20 2020 2020 2020  _time)):.       
-00006dc0: 2020 2020 2020 2020 206d 696e 5f74 696d           min_tim
-00006dd0: 6520 3d20 6e65 775f 7469 6d65 0a20 2020  e = new_time.   
-00006de0: 2020 2020 2069 6620 6920 3e20 3020 616e       if i > 0 an
-00006df0: 6420 6d69 6e5f 7469 6d65 203c 2064 7276  d min_time < drv
-00006e00: 5f64 6174 615b 2754 696d 6527 5d5b 6920  _data['Time'][i 
-00006e10: 2d20 315d 3a0a 2020 2020 2020 2020 2020  - 1]:.          
-00006e20: 2020 696e 7465 6772 6974 795f 6572 726f    integrity_erro
-00006e30: 7273 2e61 7070 656e 6428 6920 2b20 3129  rs.append(i + 1)
-00006e40: 2020 2320 6e6f 7420 6265 2070 6f73 7369    # not be possi
-00006e50: 626c 6520 6966 2073 6563 746f 7220 7469  ble if sector ti
-00006e60: 6d65 7320 616e 6420 6c61 7020 7469 6d65  mes and lap time
-00006e70: 2061 7265 2063 6f72 7265 6374 0a20 2020   are correct.   
-00006e80: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00006e90: 650a 0a20 2020 2020 2020 2064 7276 5f64  e..        drv_d
-00006ea0: 6174 615b 2754 696d 6527 5d5b 695d 203d  ata['Time'][i] =
-00006eb0: 206d 696e 5f74 696d 650a 0a20 2020 2023   min_time..    #
-00006ec0: 206c 6173 7420 6c61 7020 6e65 6564 7320   last lap needs 
-00006ed0: 746f 2062 6520 7265 6d6f 7665 6420 6966  to be removed if
-00006ee0: 2069 7420 646f 6573 206e 6f74 2068 6176   it does not hav
-00006ef0: 6520 6120 2754 696d 6527 2061 6e64 2069  e a 'Time' and i
-00006f00: 7420 636f 756c 6420 6e6f 7420 6265 2063  t could not be c
-00006f10: 616c 6375 6c61 7465 6420 286c 696b 656c  alculated (likel
-00006f20: 7920 616e 2069 6e6c 6170 290a 2020 2020  y an inlap).    
-00006f30: 6966 2070 642e 6973 6e75 6c6c 2864 7276  if pd.isnull(drv
-00006f40: 5f64 6174 615b 2754 696d 6527 5d5b 2d31  _data['Time'][-1
-00006f50: 5d29 3a0a 2020 2020 2020 2020 6966 206e  ]):.        if n
-00006f60: 6f74 2070 642e 6973 6e75 6c6c 2864 7276  ot pd.isnull(drv
-00006f70: 5f64 6174 615b 2750 6974 496e 5469 6d65  _data['PitInTime
-00006f80: 275d 5b2d 315d 293a 0a20 2020 2020 2020  '][-1]):.       
-00006f90: 2020 2020 2064 7276 5f64 6174 615b 2754       drv_data['T
-00006fa0: 696d 6527 5d5b 2d31 5d20 3d20 6472 765f  ime'][-1] = drv_
-00006fb0: 6461 7461 5b27 5069 7449 6e54 696d 6527  data['PitInTime'
-00006fc0: 5d5b 2d31 5d0a 2020 2020 2020 2020 656c  ][-1].        el
-00006fd0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00006fe0: 666f 7220 6b65 7920 696e 2064 7276 5f64  for key in drv_d
-00006ff0: 6174 612e 6b65 7973 2829 3a0a 2020 2020  ata.keys():.    
-00007000: 2020 2020 2020 2020 2020 2020 6472 765f              drv_
-00007010: 6461 7461 5b6b 6579 5d20 3d20 6472 765f  data[key] = drv_
-00007020: 6461 7461 5b6b 6579 5d5b 3a2d 315d 0a0a  data[key][:-1]..
-00007030: 2020 2020 6966 206e 6f74 2064 7276 5f64      if not drv_d
-00007040: 6174 615b 2754 696d 6527 5d3a 0a20 2020  ata['Time']:.   
-00007050: 2020 2020 2023 2065 6e73 7572 6520 7468       # ensure th
-00007060: 6174 2074 6865 7265 2069 7320 7374 696c  at there is stil
-00007070: 6c20 6461 7461 206c 6566 7420 6166 7465  l data left afte
-00007080: 7220 706f 7465 6e74 6961 6c6c 7920 7265  r potentially re
-00007090: 6d6f 7669 6e67 2061 206c 6170 0a20 2020  moving a lap.   
-000070a0: 2020 2020 2072 6574 7572 6e20 6472 765f       return drv_
-000070b0: 6461 7461 2c20 7365 7373 696f 6e5f 7370  data, session_sp
-000070c0: 6c69 745f 7469 6d65 730a 0a20 2020 2023  lit_times..    #
-000070d0: 206d 6f72 6520 6c61 7020 7379 6e63 2c20   more lap sync, 
-000070e0: 7468 6973 2074 696d 6520 6368 6563 6b20  this time check 
-000070f0: 7768 6963 6820 6c61 7020 7472 6967 6765  which lap trigge
-00007100: 7265 6420 7769 7468 2074 6865 206c 6f77  red with the low
-00007110: 6573 7420 6c61 7465 6e63 790a 2020 2020  est latency.    
-00007120: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-00007130: 656e 2864 7276 5f64 6174 615b 2754 696d  en(drv_data['Tim
-00007140: 6527 5d29 202d 2031 2c20 302c 202d 3129  e']) - 1, 0, -1)
-00007150: 3a0a 2020 2020 2020 2020 6966 2028 6e65  :.        if (ne
-00007160: 775f 7469 6d65 203a 3d20 6472 765f 6461  w_time := drv_da
-00007170: 7461 5b27 5469 6d65 275d 5b69 5d20 2d20  ta['Time'][i] - 
-00007180: 6472 765f 6461 7461 5b27 4c61 7054 696d  drv_data['LapTim
-00007190: 6527 5d5b 695d 2920 3c20 5c0a 2020 2020  e'][i]) < \.    
-000071a0: 2020 2020 2020 2020 2020 2020 6472 765f              drv_
-000071b0: 6461 7461 5b27 5469 6d65 275d 5b69 202d  data['Time'][i -
-000071c0: 2031 5d3a 0a20 2020 2020 2020 2020 2020   1]:.           
-000071d0: 2069 6620 6920 3e20 3120 616e 6420 6e65   if i > 1 and ne
-000071e0: 775f 7469 6d65 203c 2064 7276 5f64 6174  w_time < drv_dat
-000071f0: 615b 2754 696d 6527 5d5b 6920 2d20 325d  a['Time'][i - 2]
-00007200: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00007210: 2020 696e 7465 6772 6974 795f 6572 726f    integrity_erro
-00007220: 7273 2e61 7070 656e 6428 6920 2b20 3129  rs.append(i + 1)
-00007230: 2020 2320 6e6f 7420 6265 2070 6f73 7369    # not be possi
-00007240: 626c 6520 6966 2073 6563 746f 7220 7469  ble if sector ti
-00007250: 6d65 7320 616e 6420 6c61 7020 7469 6d65  mes and lap time
-00007260: 2061 7265 2063 6f72 7265 6374 0a20 2020   are correct.   
-00007270: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00007280: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00007290: 7276 5f64 6174 615b 2754 696d 6527 5d5b  rv_data['Time'][
-000072a0: 6920 2d20 315d 203d 206e 6577 5f74 696d  i - 1] = new_tim
-000072b0: 650a 0a20 2020 2023 206e 6565 6420 746f  e..    # need to
-000072c0: 2067 6f20 626f 7468 2064 6972 6563 7469   go both directi
-000072d0: 6f6e 7320 6f6e 6365 2074 6f20 6d61 6b65  ons once to make
-000072e0: 2065 7665 7279 7468 696e 6720 6d61 7463   everything matc
-000072f0: 6820 7570 3b20 616c 736f 2072 6563 616c  h up; also recal
-00007300: 6375 6c61 7465 2073 6563 746f 7220 7469  culate sector ti
-00007310: 6d65 730a 2020 2020 666f 7220 6920 696e  mes.    for i in
-00007320: 2072 616e 6765 286c 656e 2864 7276 5f64   range(len(drv_d
-00007330: 6174 615b 2754 696d 6527 5d29 202d 2031  ata['Time']) - 1
-00007340: 293a 0a20 2020 2020 2020 2069 6620 616e  ):.        if an
-00007350: 7928 7064 2e69 736e 756c 6c28 7473 7429  y(pd.isnull(tst)
-00007360: 2066 6f72 2074 7374 2069 6e20 280a 2020   for tst in (.  
-00007370: 2020 2020 2020 2020 2020 2020 2020 6472                dr
-00007380: 765f 6461 7461 5b27 5469 6d65 275d 5b69  v_data['Time'][i
-00007390: 5d2c 2064 7276 5f64 6174 615b 274c 6170  ], drv_data['Lap
-000073a0: 5469 6d65 275d 5b69 202b 2031 5d2c 0a20  Time'][i + 1],. 
-000073b0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000073c0: 7276 5f64 6174 615b 2753 6563 746f 7231  rv_data['Sector1
-000073d0: 5469 6d65 275d 5b69 202b 2031 5d2c 0a20  Time'][i + 1],. 
-000073e0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000073f0: 7276 5f64 6174 615b 2753 6563 746f 7232  rv_data['Sector2
-00007400: 5469 6d65 275d 5b69 202b 2031 5d2c 0a20  Time'][i + 1],. 
-00007410: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00007420: 7276 5f64 6174 615b 2753 6563 746f 7233  rv_data['Sector3
-00007430: 5469 6d65 275d 5b69 202b 2031 5d29 293a  Time'][i + 1])):
-00007440: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-00007450: 7469 6e75 6520 2023 206c 6170 206e 6f74  tinue  # lap not
-00007460: 2075 7361 626c 652c 206d 6973 7369 6e67   usable, missing
-00007470: 2063 7269 7469 6361 6c20 7661 6c75 6573   critical values
-00007480: 0a0a 2020 2020 2020 2020 6966 2028 6e65  ..        if (ne
-00007490: 775f 7469 6d65 203a 3d20 6472 765f 6461  w_time := drv_da
-000074a0: 7461 5b27 5469 6d65 275d 5b69 5d20 2b20  ta['Time'][i] + 
-000074b0: 6472 765f 6461 7461 5b27 4c61 7054 696d  drv_data['LapTim
-000074c0: 6527 5d5b 692b 315d 2920 5c0a 2020 2020  e'][i+1]) \.    
-000074d0: 2020 2020 2020 2020 2020 2020 3c20 6472              < dr
-000074e0: 765f 6461 7461 5b27 5469 6d65 275d 5b69  v_data['Time'][i
-000074f0: 2b31 5d3a 0a20 2020 2020 2020 2020 2020  +1]:.           
-00007500: 2064 7276 5f64 6174 615b 2754 696d 6527   drv_data['Time'
-00007510: 5d5b 692b 315d 203d 206e 6577 5f74 696d  ][i+1] = new_tim
-00007520: 650a 2020 2020 2020 2020 6966 2028 6e65  e.        if (ne
-00007530: 775f 7331 5f74 696d 6520 3a3d 2064 7276  w_s1_time := drv
-00007540: 5f64 6174 615b 2754 696d 6527 5d5b 695d  _data['Time'][i]
-00007550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007560: 202b 2064 7276 5f64 6174 615b 2753 6563   + drv_data['Sec
-00007570: 746f 7231 5469 6d65 275d 5b69 2b31 5d29  tor1Time'][i+1])
-00007580: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
-00007590: 2020 203c 2064 7276 5f64 6174 615b 2753     < drv_data['S
-000075a0: 6563 746f 7231 5365 7373 696f 6e54 696d  ector1SessionTim
-000075b0: 6527 5d5b 692b 315d 3a0a 2020 2020 2020  e'][i+1]:.      
-000075c0: 2020 2020 2020 6472 765f 6461 7461 5b27        drv_data['
-000075d0: 5365 6374 6f72 3153 6573 7369 6f6e 5469  Sector1SessionTi
-000075e0: 6d65 275d 5b69 2b31 5d20 3d20 6e65 775f  me'][i+1] = new_
-000075f0: 7331 5f74 696d 650a 2020 2020 2020 2020  s1_time.        
-00007600: 6966 2028 6e65 775f 7332 5f74 696d 6520  if (new_s2_time 
-00007610: 3a3d 2064 7276 5f64 6174 615b 2754 696d  := drv_data['Tim
-00007620: 6527 5d5b 695d 202b 2064 7276 5f64 6174  e'][i] + drv_dat
-00007630: 615b 2753 6563 746f 7231 5469 6d65 275d  a['Sector1Time']
-00007640: 5b69 2b31 5d0a 2020 2020 2020 2020 2020  [i+1].          
-00007650: 2020 2020 2020 2b20 6472 765f 6461 7461        + drv_data
-00007660: 5b27 5365 6374 6f72 3254 696d 6527 5d5b  ['Sector2Time'][
-00007670: 692b 315d 2920 5c0a 2020 2020 2020 2020  i+1]) \.        
-00007680: 2020 2020 2020 2020 3c20 6472 765f 6461          < drv_da
-00007690: 7461 5b27 5365 6374 6f72 3253 6573 7369  ta['Sector2Sessi
-000076a0: 6f6e 5469 6d65 275d 5b69 2b31 5d3a 0a20  onTime'][i+1]:. 
-000076b0: 2020 2020 2020 2020 2020 2064 7276 5f64             drv_d
-000076c0: 6174 615b 2753 6563 746f 7232 5365 7373  ata['Sector2Sess
-000076d0: 696f 6e54 696d 6527 5d5b 692b 315d 203d  ionTime'][i+1] =
-000076e0: 206e 6577 5f73 325f 7469 6d65 0a20 2020   new_s2_time.   
-000076f0: 2020 2020 2069 6620 286e 6577 5f73 335f       if (new_s3_
-00007700: 7469 6d65 203a 3d20 6472 765f 6461 7461  time := drv_data
-00007710: 5b27 5469 6d65 275d 5b69 5d20 2b20 6472  ['Time'][i] + dr
-00007720: 765f 6461 7461 5b27 5365 6374 6f72 3154  v_data['Sector1T
-00007730: 696d 6527 5d5b 692b 315d 0a20 2020 2020  ime'][i+1].     
-00007740: 2020 2020 2020 2020 2020 202b 2064 7276             + drv
-00007750: 5f64 6174 615b 2753 6563 746f 7232 5469  _data['Sector2Ti
-00007760: 6d65 275d 5b69 2b31 5d0a 2020 2020 2020  me'][i+1].      
-00007770: 2020 2020 2020 2020 2020 2b20 6472 765f            + drv_
-00007780: 6461 7461 5b27 5365 6374 6f72 3354 696d  data['Sector3Tim
-00007790: 6527 5d5b 692b 315d 2920 5c0a 2020 2020  e'][i+1]) \.    
-000077a0: 2020 2020 2020 2020 2020 2020 3c20 6472              < dr
-000077b0: 765f 6461 7461 5b27 5365 6374 6f72 3353  v_data['Sector3S
-000077c0: 6573 7369 6f6e 5469 6d65 275d 5b69 2b31  essionTime'][i+1
-000077d0: 5d3a 0a20 2020 2020 2020 2020 2020 2064  ]:.            d
-000077e0: 7276 5f64 6174 615b 2753 6563 746f 7233  rv_data['Sector3
-000077f0: 5365 7373 696f 6e54 696d 6527 5d5b 692b  SessionTime'][i+
-00007800: 315d 203d 206e 6577 5f73 335f 7469 6d65  1] = new_s3_time
-00007810: 0a0a 2020 2020 2320 4974 6572 6174 6520  ..    # Iterate 
-00007820: 6f76 6572 206c 6973 7420 6f66 2070 6572  over list of per
-00007830: 736f 6e61 6c20 6c61 7020 7469 6d65 7320  sonal lap times 
-00007840: 7365 7420 2749 7350 6572 736f 6e61 6c42  set 'IsPersonalB
-00007850: 6573 7427 2e0a 2020 2020 2320 5768 656e  est'..    # When
-00007860: 2061 206c 6170 2069 7320 6465 6c65 7465   a lap is delete
-00007870: 642c 2074 6865 2041 5049 2072 6573 656e  d, the API resen
-00007880: 6473 2074 6865 2070 7265 7669 6f75 7320  ds the previous 
-00007890: 7065 7273 6f6e 616c 2062 6573 742e 0a20  personal best.. 
-000078a0: 2020 2023 2054 6865 7265 666f 7265 2c20     # Therefore, 
-000078b0: 6279 2069 7465 7261 7469 6e67 2069 6e20  by iterating in 
-000078c0: 7265 7665 7273 652c 2069 6620 616e 7920  reverse, if any 
-000078d0: 6c61 7020 6973 2065 6e63 6f75 6e74 6572  lap is encounter
-000078e0: 6564 2074 6861 7420 6973 0a20 2020 2023  ed that is.    #
-000078f0: 2071 7569 636b 6572 2074 6861 6e20 616c   quicker than al
-00007900: 7265 6164 7920 7072 6f63 6573 7365 6420  ready processed 
-00007910: 7065 7273 6f6e 616c 2062 6573 7420 6c61  personal best la
-00007920: 7020 7469 6d65 732c 2069 7420 6d75 7374  p times, it must
-00007930: 2068 6176 650a 2020 2020 2320 6265 656e   have.    # been
-00007940: 2064 656c 6574 6564 2e0a 2020 2020 2320   deleted..    # 
-00007950: 5468 6973 2069 7320 6a75 7374 2062 6573  This is just bes
-00007960: 7420 6566 666f 7274 2062 7574 206e 6f74  t effort but not
-00007970: 2065 7868 6175 7374 6976 6520 6173 2069   exhaustive as i
-00007980: 7420 6361 6e20 6f6e 6c79 2068 616e 646c  t can only handl
-00007990: 6520 6c61 700a 2020 2020 2320 7469 6d65  e lap.    # time
-000079a0: 7320 7468 6174 2077 6572 6520 6465 6c65  s that were dele
-000079b0: 7465 6420 7175 6963 6b6c 7920 2862 6566  ted quickly (bef
-000079c0: 6f72 6520 7468 6520 6e65 7874 2070 6572  ore the next per
-000079d0: 736f 6e61 6c20 6265 7374 2077 6173 2073  sonal best was s
-000079e0: 6574 292e 0a20 2020 205f 636f 7272 6563  et)..    _correc
-000079f0: 7465 645f 7065 7273 6f6e 616c 5f62 6573  ted_personal_bes
-00007a00: 745f 6c61 705f 7469 6d65 7320 3d20 6c69  t_lap_times = li
-00007a10: 7374 2829 0a20 2020 2023 206c 6973 7420  st().    # list 
-00007a20: 6973 206f 6e6c 7920 7573 6564 2066 6f72  is only used for
-00007a30: 2062 6163 6b72 6566 6572 656e 6365 2077   backreference w
-00007a40: 6974 6869 6e20 7468 6520 6c6f 6f70 0a20  ithin the loop. 
-00007a50: 2020 2063 7572 5f73 6e20 3d20 6c65 6e28     cur_sn = len(
-00007a60: 7365 7373 696f 6e5f 7370 6c69 745f 7469  session_split_ti
-00007a70: 6d65 7329 202d 2031 0a20 2020 2023 2063  mes) - 1.    # c
-00007a80: 7572 7265 6e74 2028 7375 6229 7365 7373  urrent (sub)sess
-00007a90: 696f 6e20 6e75 6d62 6572 2c20 7065 7273  ion number, pers
-00007aa0: 6f6e 616c 2062 6573 7420 6c61 7020 7469  onal best lap ti
-00007ab0: 6d65 7320 6e65 6564 2074 6f20 6265 0a20  mes need to be. 
-00007ac0: 2020 2023 2063 6f6e 7369 6465 7265 6420     # considered 
-00007ad0: 666f 7220 6561 6368 2028 7375 6229 7365  for each (sub)se
-00007ae0: 7373 696f 6e20 696e 6469 7669 6475 616c  ssion individual
-00007af0: 6c79 0a20 2020 2066 6f72 2074 696d 652c  ly.    for time,
-00007b00: 2070 625f 6c61 705f 7469 6d65 2069 6e20   pb_lap_time in 
-00007b10: 7265 7665 7273 6564 2870 6572 736f 6e61  reversed(persona
-00007b20: 6c5f 6265 7374 5f6c 6170 5f74 696d 6573  l_best_lap_times
-00007b30: 293a 0a20 2020 2020 2020 2069 6620 7469  ):.        if ti
-00007b40: 6d65 203c 2073 6573 7369 6f6e 5f73 706c  me < session_spl
-00007b50: 6974 5f74 696d 6573 5b63 7572 5f73 6e5d  it_times[cur_sn]
-00007b60: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00007b70: 7472 616e 7369 7469 6f6e 6564 2069 6e74  transitioned int
-00007b80: 6f20 7468 6520 7072 6576 696f 7573 2028  o the previous (
-00007b90: 7375 6229 7365 7373 696f 6e20 2872 6576  sub)session (rev
-00007ba0: 6572 7365 2069 7465 7261 7469 6f6e 2129  erse iteration!)
-00007bb0: 0a20 2020 2020 2020 2020 2020 2023 2072  .            # r
-00007bc0: 6573 6574 2074 6865 2072 6566 6572 656e  eset the referen
-00007bd0: 6365 206c 6973 742c 2073 6f20 7469 6d65  ce list, so time
-00007be0: 2061 7265 2063 6f6e 7369 6465 7265 6420   are considered 
-00007bf0: 696e 6469 7669 6475 616c 6c79 0a20 2020  individually.   
-00007c00: 2020 2020 2020 2020 2063 7572 5f73 6e20           cur_sn 
-00007c10: 2d3d 2031 0a20 2020 2020 2020 2020 2020  -= 1.           
-00007c20: 205f 636f 7272 6563 7465 645f 7065 7273   _corrected_pers
-00007c30: 6f6e 616c 5f62 6573 745f 6c61 705f 7469  onal_best_lap_ti
-00007c40: 6d65 7320 3d20 6c69 7374 2829 0a0a 2020  mes = list()..  
-00007c50: 2020 2020 2020 6966 205f 636f 7272 6563        if _correc
-00007c60: 7465 645f 7065 7273 6f6e 616c 5f62 6573  ted_personal_bes
-00007c70: 745f 6c61 705f 7469 6d65 733a 0a20 2020  t_lap_times:.   
-00007c80: 2020 2020 2020 2020 2069 6620 7062 5f6c           if pb_l
-00007c90: 6170 5f74 696d 6520 696e 205f 636f 7272  ap_time in _corr
-00007ca0: 6563 7465 645f 7065 7273 6f6e 616c 5f62  ected_personal_b
-00007cb0: 6573 745f 6c61 705f 7469 6d65 733a 0a20  est_lap_times:. 
-00007cc0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00007cd0: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
-00007ce0: 2020 2020 656c 6966 2070 625f 6c61 705f      elif pb_lap_
-00007cf0: 7469 6d65 203c 206d 696e 285f 636f 7272  time < min(_corr
-00007d00: 6563 7465 645f 7065 7273 6f6e 616c 5f62  ected_personal_b
-00007d10: 6573 745f 6c61 705f 7469 6d65 7329 3a0a  est_lap_times):.
-00007d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d30: 636f 6e74 696e 7565 0a0a 2020 2020 2020  continue..      
-00007d40: 2020 5f63 6f72 7265 6374 6564 5f70 6572    _corrected_per
-00007d50: 736f 6e61 6c5f 6265 7374 5f6c 6170 5f74  sonal_best_lap_t
-00007d60: 696d 6573 2e61 7070 656e 6428 7062 5f6c  imes.append(pb_l
-00007d70: 6170 5f74 696d 6529 0a0a 2020 2020 2020  ap_time)..      
-00007d80: 2020 2320 6669 6e64 2074 6865 2069 6e64    # find the ind
-00007d90: 6578 206f 6620 7468 6520 636f 7272 6573  ex of the corres
-00007da0: 706f 6e64 696e 6720 6c61 7020 6279 2063  ponding lap by c
-00007db0: 6f6d 7061 7269 6e67 2077 6974 6820 7468  omparing with th
-00007dc0: 6520 6c61 700a 2020 2020 2020 2020 2320  e lap.        # 
-00007dd0: 7469 6d65 7320 616e 6420 7365 7420 2749  times and set 'I
-00007de0: 7350 6572 736f 6e61 6c42 6573 7427 2074  sPersonalBest' t
-00007df0: 6f20 5472 7565 2066 6f72 2074 6861 7420  o True for that 
-00007e00: 6c61 700a 2020 2020 2020 2020 7472 793a  lap.        try:
-00007e10: 0a20 2020 2020 2020 2020 2020 2070 625f  .            pb_
-00007e20: 6964 7820 3d20 6472 765f 6461 7461 5b27  idx = drv_data['
-00007e30: 4c61 7054 696d 6527 5d2e 696e 6465 7828  LapTime'].index(
-00007e40: 7062 5f6c 6170 5f74 696d 6529 0a20 2020  pb_lap_time).   
-00007e50: 2020 2020 2065 7863 6570 7420 5661 6c75       except Valu
-00007e60: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
-00007e70: 2020 2020 2320 6f6e 6520 6578 616d 706c      # one exampl
-00007e80: 6520 6361 7365 2077 6865 7265 2074 6869  e case where thi
-00007e90: 7320 6572 726f 7220 6f63 6375 7273 2c20  s error occurs, 
-00007ea0: 6172 6520 7769 6c64 6c79 206f 6620 7065  are wildly of pe
-00007eb0: 7273 6f6e 616c 0a20 2020 2020 2020 2020  rsonal.         
-00007ec0: 2020 2023 2062 6573 7420 7469 6d65 7320     # best times 
-00007ed0: 283e 3220 6d69 6e20 6c61 7020 7469 6d65  (>2 min lap time
-00007ee0: 2920 7468 6174 2061 7265 2073 6f6d 6574  ) that are somet
-00007ef0: 696d 6573 2070 7265 7365 6e74 2061 6e64  imes present and
-00007f00: 0a20 2020 2020 2020 2020 2020 2023 2077  .            # w
-00007f10: 6869 6368 2068 6176 6520 6e6f 2063 6f72  hich have no cor
-00007f20: 7265 7370 6f6e 6469 6e67 206c 6170 2074  responding lap t
-00007f30: 696d 650a 2020 2020 2020 2020 2020 2020  ime.            
-00007f40: 7061 7373 0a20 2020 2020 2020 2065 6c73  pass.        els
-00007f50: 653a 0a20 2020 2020 2020 2020 2020 2064  e:.            d
-00007f60: 7276 5f64 6174 615b 2749 7350 6572 736f  rv_data['IsPerso
-00007f70: 6e61 6c42 6573 7427 5d5b 7062 5f69 6478  nalBest'][pb_idx
-00007f80: 5d20 3d20 5472 7565 0a0a 2020 2020 2320  ] = True..    # 
-00007f90: 6669 7820 7468 6520 6e75 6d62 6572 206f  fix the number o
-00007fa0: 6620 7069 7420 7374 6f70 733b 2064 7565  f pit stops; due
-00007fb0: 2074 6f20 706f 7465 6e74 6961 6c6c 7920   to potentially 
-00007fc0: 6d75 6c74 6970 6c65 206c 6170 7320 746f  multiple laps to
-00007fd0: 2074 6865 2067 7269 640a 2020 2020 2320   the grid.    # 
-00007fe0: 7768 6572 6520 6120 6361 7220 676f 6573  where a car goes
-00007ff0: 2074 6872 6f75 6768 2074 6865 2070 6974   through the pit
-00008000: 206c 616e 6520 6265 666f 7265 2066 696e   lane before fin
-00008010: 616c 6c79 2074 616b 696e 6720 6974 7320  ally taking its 
-00008020: 706c 6163 650a 2020 2020 2320 6f6e 2074  place.    # on t
-00008030: 6865 2067 7269 642c 2074 6865 206e 756d  he grid, the num
-00008040: 6265 7220 6f66 2070 6974 2073 746f 7073  ber of pit stops
-00008050: 206f 6e20 7468 6520 6669 7273 7420 6c61   on the first la
-00008060: 7020 6d61 7920 6265 2061 6c72 6561 6479  p may be already
-00008070: 0a20 2020 2023 2067 7265 6174 6572 2074  .    # greater t
-00008080: 6861 6e20 7a65 726f 3b20 7468 6572 6566  han zero; theref
-00008090: 6f72 652c 2061 7070 6c79 2063 6f72 7265  ore, apply corre
-000080a0: 6374 696f 6e20 736f 2074 6861 7420 7765  ction so that we
-000080b0: 2073 7461 7274 2077 6974 6820 7a65 726f   start with zero
-000080c0: 0a20 2020 2070 6974 7374 6f70 5f6f 6666  .    pitstop_off
-000080d0: 7365 7420 3d20 6472 765f 6461 7461 5b27  set = drv_data['
-000080e0: 4e75 6d62 6572 4f66 5069 7453 746f 7073  NumberOfPitStops
-000080f0: 275d 5b30 5d0a 2020 2020 666f 7220 6920  '][0].    for i 
-00008100: 696e 2072 616e 6765 286c 656e 2864 7276  in range(len(drv
-00008110: 5f64 6174 615b 274e 756d 6265 724f 6650  _data['NumberOfP
-00008120: 6974 5374 6f70 7327 5d29 293a 0a20 2020  itStops'])):.   
-00008130: 2020 2020 2064 7276 5f64 6174 615b 274e       drv_data['N
-00008140: 756d 6265 724f 6650 6974 5374 6f70 7327  umberOfPitStops'
-00008150: 5d5b 695d 202d 3d20 7069 7473 746f 705f  ][i] -= pitstop_
-00008160: 6f66 6673 6574 0a0a 2020 2020 2320 6669  offset..    # fi
-00008170: 7820 6669 7273 7420 6c61 7020 5069 7449  x first lap PitI
-00008180: 6e54 696d 653b 2073 616d 6520 7265 6173  nTime; same reas
-00008190: 6f6e 2061 7320 6162 6f76 6520 666f 7220  on as above for 
-000081a0: 7069 7420 7374 6f70 732c 2074 6865 7265  pit stops, there
-000081b0: 206d 6179 0a20 2020 2023 2062 6520 616e   may.    # be an
-000081c0: 2069 6e63 6f72 7265 6374 2050 6974 496e   incorrect PitIn
-000081d0: 5469 6d65 206f 6e20 7468 6520 6669 7273  Time on the firs
-000081e0: 7420 6c61 702e 2054 6865 7265 2061 6c77  t lap. There alw
-000081f0: 6179 7320 6973 2061 2050 6974 4f75 7454  ays is a PitOutT
-00008200: 696d 650a 2020 2020 2320 666f 7220 7768  ime.    # for wh
-00008210: 656e 2074 6865 2063 6172 206c 6561 7665  en the car leave
-00008220: 7320 7468 6520 626f 7820 666f 7220 7468  s the box for th
-00008230: 6520 6c61 7020 746f 2074 6865 2067 7269  e lap to the gri
-00008240: 642e 2054 6865 7265 2069 7320 610a 2020  d. There is a.  
-00008250: 2020 2320 5069 7449 6e54 696d 6520 6966    # PitInTime if
-00008260: 2074 6865 2063 6172 2064 7269 7665 7320   the car drives 
-00008270: 6d75 6c74 6970 6c65 206c 6170 7320 746f  multiple laps to
-00008280: 2074 6865 2067 7269 642c 2064 6973 6361   the grid, disca
-00008290: 7264 2074 6865 7365 2e0a 2020 2020 2320  rd these..    # 
-000082a0: 5468 6572 6520 6973 2061 6c73 6f20 6120  There is also a 
-000082b0: 5069 7449 6e54 696d 6520 6966 2074 6865  PitInTime if the
-000082c0: 2063 6172 2061 6374 7561 6c6c 7920 7069   car actually pi
-000082d0: 7473 2061 7420 7468 6520 656e 6420 6f66  ts at the end of
-000082e0: 2074 6865 0a20 2020 2023 2066 6972 7374   the.    # first
-000082f0: 206c 6170 2c20 7468 6f73 6520 6e65 6564   lap, those need
-00008300: 2074 6f20 6265 206b 6570 742e 0a20 2020   to be kept..   
-00008310: 2069 6620 6472 765f 6461 7461 5b27 5069   if drv_data['Pi
-00008320: 7449 6e54 696d 6527 5d5b 305d 203c 2064  tInTime'][0] < d
-00008330: 7276 5f64 6174 615b 2750 6974 4f75 7454  rv_data['PitOutT
-00008340: 696d 6527 5d5b 305d 3a0a 2020 2020 2020  ime'][0]:.      
-00008350: 2020 6472 765f 6461 7461 5b27 5069 7449    drv_data['PitI
-00008360: 6e54 696d 6527 5d5b 305d 203d 2070 642e  nTime'][0] = pd.
-00008370: 4e61 540a 0a20 2020 2069 6620 696e 7465  NaT..    if inte
-00008380: 6772 6974 795f 6572 726f 7273 3a0a 2020  grity_errors:.  
-00008390: 2020 2020 2020 5f6c 6f67 6765 722e 7761        _logger.wa
-000083a0: 726e 696e 6728 0a20 2020 2020 2020 2020  rning(.         
-000083b0: 2020 2066 2244 7269 7665 7220 7b64 7276     f"Driver {drv
-000083c0: 3a20 3e32 7d3a 2045 6e63 6f75 6e74 6572  : >2}: Encounter
-000083d0: 6564 207b 6c65 6e28 696e 7465 6772 6974  ed {len(integrit
-000083e0: 795f 6572 726f 7273 297d 2074 696d 696e  y_errors)} timin
-000083f0: 6720 220a 2020 2020 2020 2020 2020 2020  g ".            
-00008400: 6622 696e 7465 6772 6974 7920 6572 726f  f"integrity erro
-00008410: 7228 7329 206e 6561 7220 6c61 7028 7329  r(s) near lap(s)
-00008420: 3a20 7b69 6e74 6567 7269 7479 5f65 7272  : {integrity_err
-00008430: 6f72 737d 2e5c 6e22 0a20 2020 2020 2020  ors}.\n".       
-00008440: 2020 2020 2066 2254 6869 7320 6d69 6768       f"This migh
-00008450: 7420 6265 2061 2062 7567 2061 6e64 2073  t be a bug and s
-00008460: 686f 756c 6420 6265 2072 6570 6f72 7465  hould be reporte
-00008470: 642e 2229 0a0a 2020 2020 7265 7475 726e  d.")..    return
-00008480: 2064 7276 5f64 6174 612c 2073 6573 7369   drv_data, sessi
-00008490: 6f6e 5f73 706c 6974 5f74 696d 6573 0a0a  on_split_times..
-000084a0: 0a64 6566 205f 7374 7265 616d 5f64 6174  .def _stream_dat
-000084b0: 615f 6472 6976 6572 2864 7269 7665 725f  a_driver(driver_
-000084c0: 7261 772c 2065 6d70 7479 5f76 616c 732c  raw, empty_vals,
-000084d0: 2064 7276 293a 0a20 2020 2022 2222 0a20   drv):.    """. 
-000084e0: 2020 202e 2e20 7761 726e 696e 673a 3a0a     .. warning::.
-000084f0: 2020 2020 2020 2020 3a6d 6f64 3a60 6661          :mod:`fa
-00008500: 7374 6631 2e61 7069 6020 7769 6c6c 2062  stf1.api` will b
-00008510: 6520 636f 6e73 6964 6572 6564 2070 7269  e considered pri
-00008520: 7661 7465 2069 6e20 6675 7475 7265 2072  vate in future r
-00008530: 656c 6561 7365 7320 616e 640a 2020 2020  eleases and.    
-00008540: 2020 2020 706f 7465 6e74 6961 6c6c 7920      potentially 
-00008550: 6265 2072 656d 6f76 6564 206f 7220 6368  be removed or ch
-00008560: 616e 6765 642e 0a0a 2020 2020 4461 7461  anged...    Data
-00008570: 2069 7320 6f6e 2061 2074 696d 6573 7461   is on a timesta
-00008580: 6d70 2062 6173 6973 2e0a 0a20 2020 2050  mp basis...    P
-00008590: 6172 616d 733a 0a20 2020 2020 2020 2064  arams:.        d
-000085a0: 7269 7665 725f 7261 7720 286c 6973 7429  river_raw (list)
-000085b0: 3a20 7261 7720 6170 6920 7265 7370 6f6e  : raw api respon
-000085c0: 7365 2066 6f72 2074 6869 7320 6472 6976  se for this driv
-000085d0: 6572 206f 6e6c 7920 5b28 5469 6d65 7374  er only [(Timest
-000085e0: 616d 702c 2064 6174 6129 2c20 282e 2e2e  amp, data), (...
-000085f0: 292c 202e 2e2e 5d0a 2020 2020 2020 2020  ), ...].        
-00008600: 656d 7074 795f 7661 6c73 2028 6469 6374  empty_vals (dict
-00008610: 293a 2064 6963 7469 6f6e 6172 7920 6f66  ): dictionary of
-00008620: 2063 6f6c 756d 6e20 6e61 6d65 7320 616e   column names an
-00008630: 6420 656d 7074 7920 636f 6c75 6d6e 2076  d empty column v
-00008640: 616c 7565 730a 2020 2020 2020 2020 6472  alues.        dr
-00008650: 7620 2873 7472 293a 2064 7269 7665 7220  v (str): driver 
-00008660: 6964 656e 7469 6669 6572 0a0a 2020 2020  identifier..    
-00008670: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00008680: 2020 6469 6374 696f 6e61 7279 206f 6620    dictionary of 
-00008690: 7469 6d69 6e67 2073 7472 6561 6d20 6461  timing stream da
-000086a0: 7461 2066 6f72 2074 6869 7320 6472 6976  ta for this driv
-000086b0: 6572 0a20 2020 2022 2222 0a20 2020 2023  er.    """.    #
-000086c0: 2065 6e74 7269 6573 2061 7265 2070 7265   entries are pre
-000086d0: 6669 6c6c 6564 2077 6974 6820 656d 7074  filled with empt
-000086e0: 7920 6f72 2070 7265 7669 6f75 7320 7661  y or previous va
-000086f0: 6c75 6573 2061 6e64 206f 6e6c 7920 6f76  lues and only ov
-00008700: 6572 7772 6974 7465 6e20 6966 2074 6865  erwritten if the
-00008710: 7920 6578 6973 7420 696e 2074 6865 2072  y exist in the r
-00008720: 6573 706f 6e73 6520 6c69 6e65 0a20 2020  esponse line.   
-00008730: 2023 2062 6173 6963 616c 6c79 2069 6e74   # basically int
-00008740: 6572 706f 6c61 7469 6f6e 2062 7920 6669  erpolation by fi
-00008750: 6c6c 696e 6720 7570 2077 6974 6820 6c61  lling up with la
-00008760: 7374 206b 6e6f 776e 2076 616c 7565 2062  st known value b
-00008770: 6563 6175 7365 206e 6f74 2065 7665 7279  ecause not every
-00008780: 2076 616c 7565 2069 7320 696e 2065 7665   value is in eve
-00008790: 7279 2072 6573 706f 6e73 650a 2020 2020  ry response.    
-000087a0: 6472 765f 6461 7461 203d 207b 6b65 793a  drv_data = {key:
-000087b0: 205b 7661 6c2c 205d 2066 6f72 206b 6579   [val, ] for key
-000087c0: 2c20 7661 6c20 696e 2065 6d70 7479 5f76  , val in empty_v
-000087d0: 616c 732e 6974 656d 7328 297d 0a20 2020  als.items()}.   
-000087e0: 2069 203d 2030 0a0a 2020 2020 2320 6974   i = 0..    # it
-000087f0: 6572 6174 6520 7468 726f 7567 6820 7468  erate through th
-00008800: 6520 6461 7461 3b20 7469 6d65 7374 616d  e data; timestam
-00008810: 7020 2b20 616e 7920 6f66 2074 6865 2076  p + any of the v
-00008820: 616c 7565 7320 7472 6967 6765 7273 206e  alues triggers n
-00008830: 6577 2072 6f77 2069 6e20 6461 7461 0a20  ew row in data. 
-00008840: 2020 2066 6f72 2074 696d 652c 2072 6573     for time, res
-00008850: 7020 696e 2064 7269 7665 725f 7261 773a  p in driver_raw:
-00008860: 0a20 2020 2020 2020 206e 6577 5f65 6e74  .        new_ent
-00008870: 7279 203d 2046 616c 7365 0a20 2020 2020  ry = False.     
-00008880: 2020 2069 6620 7661 6c20 3a3d 2072 6563     if val := rec
-00008890: 7572 7369 7665 5f64 6963 745f 6765 7428  ursive_dict_get(
-000088a0: 7265 7370 2c20 2750 6f73 6974 696f 6e27  resp, 'Position'
-000088b0: 293a 0a20 2020 2020 2020 2020 2020 2064  ):.            d
-000088c0: 7276 5f64 6174 615b 2750 6f73 6974 696f  rv_data['Positio
-000088d0: 6e27 5d5b 695d 203d 2069 6e74 2876 616c  n'][i] = int(val
-000088e0: 290a 2020 2020 2020 2020 2020 2020 6e65  ).            ne
-000088f0: 775f 656e 7472 7920 3d20 5472 7565 0a20  w_entry = True. 
-00008900: 2020 2020 2020 2069 6620 7661 6c20 3a3d         if val :=
-00008910: 2072 6563 7572 7369 7665 5f64 6963 745f   recursive_dict_
-00008920: 6765 7428 7265 7370 2c20 2747 6170 546f  get(resp, 'GapTo
-00008930: 4c65 6164 6572 2729 3a0a 2020 2020 2020  Leader'):.      
-00008940: 2020 2020 2020 6472 765f 6461 7461 5b27        drv_data['
-00008950: 4761 7054 6f4c 6561 6465 7227 5d5b 695d  GapToLeader'][i]
-00008960: 203d 2076 616c 0a20 2020 2020 2020 2020   = val.         
-00008970: 2020 206e 6577 5f65 6e74 7279 203d 2054     new_entry = T
-00008980: 7275 650a 2020 2020 2020 2020 6966 2076  rue.        if v
-00008990: 616c 203a 3d20 7265 6375 7273 6976 655f  al := recursive_
-000089a0: 6469 6374 5f67 6574 2872 6573 702c 2027  dict_get(resp, '
-000089b0: 496e 7465 7276 616c 546f 506f 7369 7469  IntervalToPositi
-000089c0: 6f6e 4168 6561 6427 2c20 2756 616c 7565  onAhead', 'Value
-000089d0: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
-000089e0: 6472 765f 6461 7461 5b27 496e 7465 7276  drv_data['Interv
-000089f0: 616c 546f 506f 7369 7469 6f6e 4168 6561  alToPositionAhea
-00008a00: 6427 5d5b 695d 203d 2076 616c 0a20 2020  d'][i] = val.   
-00008a10: 2020 2020 2020 2020 206e 6577 5f65 6e74           new_ent
-00008a20: 7279 203d 2054 7275 650a 0a20 2020 2020  ry = True..     
-00008a30: 2020 2023 2061 7420 6c65 6173 7420 6f6e     # at least on
-00008a40: 6520 7661 6c75 6520 7761 7320 7072 6573  e value was pres
-00008a50: 656e 742c 2063 7265 6174 6520 6e65 7874  ent, create next
-00008a60: 2072 6f77 0a20 2020 2020 2020 2069 6620   row.        if 
-00008a70: 6e65 775f 656e 7472 793a 0a20 2020 2020  new_entry:.     
-00008a80: 2020 2020 2020 2064 7276 5f64 6174 615b         drv_data[
-00008a90: 2754 696d 6527 5d5b 695d 203d 2074 6f5f  'Time'][i] = to_
-00008aa0: 7469 6d65 6465 6c74 6128 7469 6d65 290a  timedelta(time).
-00008ab0: 2020 2020 2020 2020 2020 2020 6472 765f              drv_
-00008ac0: 6461 7461 5b27 4472 6976 6572 275d 5b69  data['Driver'][i
-00008ad0: 5d20 3d20 6472 760a 2020 2020 2020 2020  ] = drv.        
-00008ae0: 2020 2020 6920 2b3d 2031 0a0a 2020 2020      i += 1..    
-00008af0: 2020 2020 2020 2020 2320 6372 6561 7465          # create
-00008b00: 206e 6578 7420 726f 7720 6f66 2064 6174   next row of dat
-00008b10: 6120 6672 6f6d 2074 6865 206c 6173 7420  a from the last 
-00008b20: 7661 6c75 6573 3b20 7468 6572 6520 7769  values; there wi
-00008b30: 6c6c 2061 6c77 6179 7320 6265 206f 6e65  ll always be one
-00008b40: 2072 6f77 2074 6f6f 206d 7563 6820 6174   row too much at
-00008b50: 2074 6865 2065 6e64 2077 6869 6368 2069   the end which i
-00008b60: 730a 2020 2020 2020 2020 2020 2020 2320  s.            # 
-00008b70: 7265 6d6f 7665 6420 6167 6169 6e0a 2020  removed again.  
-00008b80: 2020 2020 2020 2020 2020 666f 7220 6b65            for ke
-00008b90: 792c 2076 616c 2069 6e20 656d 7074 795f  y, val in empty_
-00008ba0: 7661 6c73 2e69 7465 6d73 2829 3a0a 2020  vals.items():.  
-00008bb0: 2020 2020 2020 2020 2020 2020 2020 6472                dr
-00008bc0: 765f 6461 7461 5b6b 6579 5d2e 6170 7065  v_data[key].appe
-00008bd0: 6e64 2864 7276 5f64 6174 615b 6b65 795d  nd(drv_data[key]
-00008be0: 5b2d 315d 290a 0a20 2020 2066 6f72 206b  [-1])..    for k
-00008bf0: 6579 2069 6e20 6472 765f 6461 7461 2e6b  ey in drv_data.k
-00008c00: 6579 7328 293a 0a20 2020 2020 2020 2064  eys():.        d
-00008c10: 7276 5f64 6174 615b 6b65 795d 203d 2064  rv_data[key] = d
-00008c20: 7276 5f64 6174 615b 6b65 795d 5b3a 2d31  rv_data[key][:-1
-00008c30: 5d20 2023 2072 656d 6f76 6520 7665 7279  ]  # remove very
-00008c40: 206c 6173 7420 726f 7720 6167 6169 6e0a   last row again.
-00008c50: 0a20 2020 2072 6574 7572 6e20 6472 765f  .    return drv_
-00008c60: 6461 7461 0a0a 0a40 4361 6368 652e 6170  data...@Cache.ap
-00008c70: 695f 7265 7175 6573 745f 7772 6170 7065  i_request_wrappe
-00008c80: 720a 6465 6620 7469 6d69 6e67 5f61 7070  r.def timing_app
-00008c90: 5f64 6174 6128 7061 7468 2c20 7265 7370  _data(path, resp
-00008ca0: 6f6e 7365 3d4e 6f6e 652c 206c 6976 6564  onse=None, lived
-00008cb0: 6174 613d 4e6f 6e65 293a 0a20 2020 2022  ata=None):.    "
-00008cc0: 2222 0a20 2020 202e 2e20 7761 726e 696e  "".    .. warnin
-00008cd0: 673a 3a0a 2020 2020 2020 2020 3a6d 6f64  g::.        :mod
-00008ce0: 3a60 6661 7374 6631 2e61 7069 6020 7769  :`fastf1.api` wi
-00008cf0: 6c6c 2062 6520 636f 6e73 6964 6572 6564  ll be considered
-00008d00: 2070 7269 7661 7465 2069 6e20 6675 7475   private in futu
-00008d10: 7265 2072 656c 6561 7365 7320 616e 640a  re releases and.
-00008d20: 2020 2020 2020 2020 706f 7465 6e74 6961          potentia
-00008d30: 6c6c 7920 6265 2072 656d 6f76 6564 206f  lly be removed o
-00008d40: 7220 6368 616e 6765 642e 0a0a 2020 2020  r changed...    
-00008d50: 4665 7463 6820 616e 6420 7061 7273 6520  Fetch and parse 
-00008d60: 2774 696d 696e 6720 6170 7020 6461 7461  'timing app data
-00008d70: 272e 0a0a 2020 2020 5469 6d69 6e67 2061  '...    Timing a
-00008d80: 7070 2064 6174 6120 7072 6f76 6964 6573  pp data provides
-00008d90: 2074 6865 2066 6f6c 6c6f 7769 6e67 2064   the following d
-00008da0: 6174 6120 6368 616e 6e65 6c73 2070 6572  ata channels per
-00008db0: 2073 616d 706c 653a 0a20 2020 2020 2020   sample:.       
-00008dc0: 2d20 4c61 704e 756d 6265 7220 2866 6c6f  - LapNumber (flo
-00008dd0: 6174 206f 7220 6e61 6e29 3a20 4375 7272  at or nan): Curr
-00008de0: 656e 7420 6c61 7020 6e75 6d62 6572 0a20  ent lap number. 
-00008df0: 2020 2020 2020 2d20 4472 6976 6572 2028        - Driver (
-00008e00: 7374 7229 3a20 4472 6976 6572 206e 756d  str): Driver num
-00008e10: 6265 720a 2020 2020 2020 202d 204c 6170  ber.       - Lap
-00008e20: 5469 6d65 2028 7061 6e64 6173 2e54 696d  Time (pandas.Tim
-00008e30: 6564 656c 7461 206f 7220 4e6f 6e65 293a  edelta or None):
-00008e40: 204c 6170 2074 696d 6520 6f66 206c 6173   Lap time of las
-00008e50: 7420 6c61 700a 2020 2020 2020 202d 2053  t lap.       - S
-00008e60: 7469 6e74 2028 696e 7429 3a20 436f 756e  tint (int): Coun
-00008e70: 7465 7220 666f 7220 7468 6520 6e75 6d62  ter for the numb
-00008e80: 6572 206f 6620 6472 6976 656e 2073 7469  er of driven sti
-00008e90: 6e74 730a 2020 2020 2020 202d 2054 6f74  nts.       - Tot
-00008ea0: 616c 4c61 7073 2028 666c 6f61 7420 6f72  alLaps (float or
-00008eb0: 206e 616e 293a 2054 6f74 616c 206e 756d   nan): Total num
-00008ec0: 6265 7220 6f66 206c 6170 7320 6472 6976  ber of laps driv
-00008ed0: 656e 206f 6e20 7468 6973 2073 6574 206f  en on this set o
-00008ee0: 6620 7469 7265 7320 2869 6e63 6c75 6465  f tires (include
-00008ef0: 7320 6c61 7073 2064 7269 7665 6e20 696e  s laps driven in
-00008f00: 0a20 2020 2020 2020 2020 6f74 6865 7220  .         other 
-00008f10: 7365 7373 696f 6e73 2129 0a20 2020 2020  sessions!).     
-00008f20: 2020 2d20 436f 6d70 6f75 6e64 2028 7374    - Compound (st
-00008f30: 7220 6f72 204e 6f6e 6529 3a20 5469 7265  r or None): Tire
-00008f40: 2063 6f6d 706f 756e 640a 2020 2020 2020   compound.      
-00008f50: 202d 204e 6577 2028 626f 6f6c 206f 7220   - New (bool or 
-00008f60: 4e6f 6e65 293a 2057 6865 7468 6572 2074  None): Whether t
-00008f70: 6865 2074 6972 6520 7761 7320 6e65 7720  he tire was new 
-00008f80: 7768 656e 2066 6974 7465 640a 2020 2020  when fitted.    
-00008f90: 2020 202d 2054 7972 6573 4e6f 7443 6861     - TyresNotCha
-00008fa0: 6e67 6564 2028 696e 7420 6f72 204e 6f6e  nged (int or Non
-00008fb0: 6529 3a20 3f3f 3f20 5072 6f62 6162 6c79  e): ??? Probably
-00008fc0: 2061 2066 6c61 6720 746f 206d 6172 6b20   a flag to mark 
-00008fd0: 7069 7420 7374 6f70 7320 7769 7468 6f75  pit stops withou
-00008fe0: 7420 7469 7265 2063 6861 6e67 6573 0a20  t tire changes. 
-00008ff0: 2020 2020 2020 2d20 5469 6d65 2028 7061        - Time (pa
-00009000: 6e64 6173 2e54 696d 6564 656c 7461 293a  ndas.Timedelta):
-00009010: 2053 6573 7369 6f6e 2074 696d 650a 2020   Session time.  
-00009020: 2020 2020 202d 204c 6170 466c 6167 7320       - LapFlags 
-00009030: 2866 6c6f 6174 206f 7220 6e61 6e29 3a20  (float or nan): 
-00009040: 3f3f 3f20 756e 6b6e 6f77 6e0a 2020 2020  ??? unknown.    
-00009050: 2020 202d 204c 6170 436f 756e 7454 696d     - LapCountTim
-00009060: 6520 284e 6f6e 6520 6f72 203f 3f3f 293a  e (None or ???):
-00009070: 203f 3f3f 2075 6e6b 6e6f 776e 3b20 6e6f   ??? unknown; no
-00009080: 2064 6174 610a 2020 2020 2020 202d 2053   data.       - S
-00009090: 7461 7274 4c61 7073 2028 666c 6f61 7420  tartLaps (float 
-000090a0: 6f72 206e 616e 293a 203f 3f3f 2054 6972  or nan): ??? Tir
-000090b0: 6520 6167 6520 7768 656e 2066 6974 7465  e age when fitte
-000090c0: 6420 2873 616d 6520 6173 2027 546f 7461  d (same as 'Tota
-000090d0: 6c4c 6170 7327 2069 6e20 7468 6520 7361  lLaps' in the sa
-000090e0: 6d65 2073 616d 706c 653f 213f 290a 2020  me sample?!?).  
-000090f0: 2020 2020 202d 204f 7574 6c61 7020 284e       - Outlap (N
-00009100: 6f6e 6520 6f72 203f 3f3f 293a 203f 3f3f  one or ???): ???
-00009110: 2075 6e6b 6e6f 776e 3b20 6e6f 2064 6174   unknown; no dat
-00009120: 610a 0a20 2020 204f 6e6c 7920 6120 6665  a..    Only a fe
-00009130: 7720 7661 6c75 6573 2061 7265 2070 7265  w values are pre
-00009140: 7365 6e74 2070 6572 2074 696d 6573 7461  sent per timesta
-00009150: 6d70 2e20 536f 6d65 7768 6174 2063 6f6d  mp. Somewhat com
-00009160: 7072 6568 656e 7369 7665 2069 6e66 6f72  prehensive infor
-00009170: 6d61 7469 6f6e 2063 616e 2074 6865 7265  mation can there
-00009180: 666f 7265 206f 6e6c 7920 6265 206f 6274  fore only be obt
-00009190: 6169 6e65 6420 6279 0a20 2020 2061 6767  ained by.    agg
-000091a0: 7265 6761 7469 6e67 2064 6174 6120 2875  regating data (u
-000091b0: 7375 616c 6c79 206f 7665 7220 7468 6520  sually over the 
-000091c0: 636f 7572 7365 206f 6620 6f6e 6520 6c61  course of one la
-000091d0: 7029 2e20 536f 6d65 2076 616c 7565 7320  p). Some values 
-000091e0: 6172 6520 7365 6e74 2065 7665 6e20 6c65  are sent even le
-000091f0: 7373 0a20 2020 2066 7265 7175 656e 746c  ss.    frequentl
-00009200: 7920 2866 6f72 2065 7861 6d70 6c65 2027  y (for example '
-00009210: 436f 6d70 6f75 6e64 2720 6f6e 6c79 2061  Compound' only a
-00009220: 6674 6572 2074 6972 6520 6368 616e 6765  fter tire change
-00009230: 7329 2e0a 0a20 2020 2041 7267 733a 0a20  s)...    Args:. 
-00009240: 2020 2020 2020 2070 6174 6820 2873 7472         path (str
-00009250: 293a 2061 7069 2070 6174 6820 6261 7365  ): api path base
-00009260: 2073 7472 696e 6720 2875 7375 616c 6c79   string (usually
-00009270: 2060 6053 6573 7369 6f6e 2e61 7069 5f70   ``Session.api_p
-00009280: 6174 6860 6029 0a20 2020 2020 2020 2072  ath``).        r
-00009290: 6573 706f 6e73 653a 2052 6573 706f 6e73  esponse: Respons
-000092a0: 6520 6173 2072 6574 7572 6e65 6420 6279  e as returned by
-000092b0: 203a 6675 6e63 3a60 6665 7463 685f 7061   :func:`fetch_pa
-000092c0: 6765 6020 6361 6e20 6265 2070 6173 7365  ge` can be passe
-000092d0: 6420 6966 2069 7420 7761 7320 646f 776e  d if it was down
-000092e0: 6c6f 6164 6564 2061 6c72 6561 6479 2e0a  loaded already..
-000092f0: 2020 2020 2020 2020 6c69 7665 6461 7461          livedata
-00009300: 3a20 416e 2069 6e73 7461 6e63 6520 6f66  : An instance of
-00009310: 203a 636c 6173 733a 6066 6173 7466 312e   :class:`fastf1.
-00009320: 6c69 7665 7469 6d69 6e67 2e64 6174 612e  livetiming.data.
-00009330: 4c69 7665 5469 6d69 6e67 4461 7461 6020  LiveTimingData` 
-00009340: 746f 2075 7365 2061 7320 6120 736f 7572  to use as a sour
-00009350: 6365 2069 6e73 7465 6164 206f 6620 7468  ce instead of th
-00009360: 6520 6170 690a 0a20 2020 2052 6574 7572  e api..    Retur
-00009370: 6e73 3a0a 2020 2020 2020 2020 4120 4461  ns:.        A Da
-00009380: 7461 4672 616d 6520 636f 6e74 6169 6e69  taFrame containi
-00009390: 6e67 206f 6e65 2063 6f6c 756d 6e20 666f  ng one column fo
-000093a0: 7220 6561 6368 2064 6174 6120 6368 616e  r each data chan
-000093b0: 6e65 6c20 6c69 7374 6564 2061 626f 7665  nel listed above
-000093c0: 2e0a 0a20 2020 2052 6169 7365 733a 0a20  ...    Raises:. 
-000093d0: 2020 2020 2020 2053 6573 7369 6f6e 4e6f         SessionNo
-000093e0: 7441 7661 696c 6162 6c65 4572 726f 723a  tAvailableError:
-000093f0: 2069 6e20 6361 7365 2074 6865 2046 3120   in case the F1 
-00009400: 6c69 7665 7469 6d69 6e67 2061 7069 2072  livetiming api r
-00009410: 6574 7572 6e73 206e 6f20 6461 7461 0a20  eturns no data. 
-00009420: 2020 2022 2222 0a20 2020 2069 6620 6c69     """.    if li
-00009430: 7665 6461 7461 2069 7320 6e6f 7420 4e6f  vedata is not No
-00009440: 6e65 2061 6e64 206c 6976 6564 6174 612e  ne and livedata.
-00009450: 6861 7328 2754 696d 696e 6741 7070 4461  has('TimingAppDa
-00009460: 7461 2729 3a0a 2020 2020 2020 2020 7265  ta'):.        re
-00009470: 7370 6f6e 7365 203d 206c 6976 6564 6174  sponse = livedat
-00009480: 612e 6765 7428 2754 696d 696e 6741 7070  a.get('TimingApp
-00009490: 4461 7461 2729 0a20 2020 2065 6c69 6620  Data').    elif 
-000094a0: 7265 7370 6f6e 7365 2069 7320 4e6f 6e65  response is None
-000094b0: 3a20 2023 206e 6f20 7072 6576 696f 7573  :  # no previous
-000094c0: 2072 6573 706f 6e73 6520 7072 6f76 6964   response provid
-000094d0: 6564 0a20 2020 2020 2020 205f 6c6f 6767  ed.        _logg
-000094e0: 6572 2e69 6e66 6f28 2246 6574 6368 696e  er.info("Fetchin
-000094f0: 6720 7469 6d69 6e67 2061 7070 2064 6174  g timing app dat
-00009500: 612e 2e2e 2229 0a20 2020 2020 2020 2072  a...").        r
-00009510: 6573 706f 6e73 6520 3d20 6665 7463 685f  esponse = fetch_
-00009520: 7061 6765 2870 6174 682c 2027 7469 6d69  page(path, 'timi
-00009530: 6e67 5f61 7070 5f64 6174 6127 290a 2020  ng_app_data').  
-00009540: 2020 2020 2020 6966 2072 6573 706f 6e73        if respons
-00009550: 6520 6973 204e 6f6e 653a 2020 2320 6e6f  e is None:  # no
-00009560: 2072 6573 706f 6e73 6520 7265 6365 6976   response receiv
-00009570: 6564 0a20 2020 2020 2020 2020 2020 2072  ed.            r
-00009580: 6169 7365 2053 6573 7369 6f6e 4e6f 7441  aise SessionNotA
-00009590: 7661 696c 6162 6c65 4572 726f 7228 0a20  vailableError(. 
-000095a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000095b0: 4e6f 2064 6174 6120 666f 7220 7468 6973  No data for this
-000095c0: 2073 6573 7369 6f6e 2120 4966 2074 6869   session! If thi
-000095d0: 7320 7365 7373 696f 6e20 6f6e 6c79 2066  s session only f
-000095e0: 696e 6973 6865 6420 220a 2020 2020 2020  inished ".      
-000095f0: 2020 2020 2020 2020 2020 2272 6563 656e            "recen
-00009600: 746c 792c 2070 6c65 6173 6520 7472 7920  tly, please try 
-00009610: 6167 6169 6e20 696e 2061 2066 6577 206d  again in a few m
-00009620: 696e 7574 6573 2e22 0a20 2020 2020 2020  inutes.".       
-00009630: 2020 2020 2029 0a0a 2020 2020 6461 7461       )..    data
-00009640: 203d 207b 274c 6170 4e75 6d62 6572 273a   = {'LapNumber':
-00009650: 205b 5d2c 2027 4472 6976 6572 273a 205b   [], 'Driver': [
-00009660: 5d2c 2027 4c61 7054 696d 6527 3a20 5b5d  ], 'LapTime': []
-00009670: 2c20 2753 7469 6e74 273a 205b 5d2c 2027  , 'Stint': [], '
-00009680: 546f 7461 6c4c 6170 7327 3a20 5b5d 2c20  TotalLaps': [], 
-00009690: 2743 6f6d 706f 756e 6427 3a20 5b5d 2c20  'Compound': [], 
-000096a0: 274e 6577 273a 205b 5d2c 0a20 2020 2020  'New': [],.     
-000096b0: 2020 2020 2020 2027 5479 7265 734e 6f74         'TyresNot
-000096c0: 4368 616e 6765 6427 3a20 5b5d 2c20 2754  Changed': [], 'T
-000096d0: 696d 6527 3a20 5b5d 2c20 274c 6170 466c  ime': [], 'LapFl
-000096e0: 6167 7327 3a20 5b5d 2c20 274c 6170 436f  ags': [], 'LapCo
-000096f0: 756e 7454 696d 6527 3a20 5b5d 2c20 2753  untTime': [], 'S
-00009700: 7461 7274 4c61 7073 273a 205b 5d2c 2027  tartLaps': [], '
-00009710: 4f75 746c 6170 273a 205b 5d7d 0a0a 2020  Outlap': []}..  
-00009720: 2020 666f 7220 656e 7472 7920 696e 2072    for entry in r
-00009730: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
-00009740: 2069 6620 286c 656e 2865 6e74 7279 2920   if (len(entry) 
-00009750: 3c20 3229 206f 7220 274c 696e 6573 2720  < 2) or 'Lines' 
-00009760: 6e6f 7420 696e 2065 6e74 7279 5b31 5d3a  not in entry[1]:
-00009770: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-00009780: 7469 6e75 650a 0a20 2020 2020 2020 2074  tinue..        t
-00009790: 696d 6520 3d20 746f 5f74 696d 6564 656c  ime = to_timedel
-000097a0: 7461 2865 6e74 7279 5b30 5d29 0a20 2020  ta(entry[0]).   
-000097b0: 2020 2020 2072 6f77 203d 2065 6e74 7279       row = entry
-000097c0: 5b31 5d0a 2020 2020 2020 2020 666f 7220  [1].        for 
-000097d0: 6472 6976 6572 5f6e 756d 6265 7220 696e  driver_number in
-000097e0: 2072 6f77 5b27 4c69 6e65 7327 5d3a 0a20   row['Lines']:. 
-000097f0: 2020 2020 2020 2020 2020 2069 6620 7570             if up
-00009800: 6461 7465 203a 3d20 7265 6375 7273 6976  date := recursiv
-00009810: 655f 6469 6374 5f67 6574 2872 6f77 2c20  e_dict_get(row, 
-00009820: 274c 696e 6573 272c 2064 7269 7665 725f  'Lines', driver_
-00009830: 6e75 6d62 6572 2c20 2753 7469 6e74 7327  number, 'Stints'
-00009840: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00009850: 2020 2066 6f72 2073 7469 6e74 5f6e 756d     for stint_num
-00009860: 6265 722c 2073 7469 6e74 2069 6e20 656e  ber, stint in en
-00009870: 756d 6572 6174 6528 7570 6461 7465 293a  umerate(update):
-00009880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009890: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-000098a0: 6365 2875 7064 6174 652c 2064 6963 7429  ce(update, dict)
-000098b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000098c0: 2020 2020 2020 2020 2020 7374 696e 745f            stint_
-000098d0: 6e75 6d62 6572 203d 2069 6e74 2873 7469  number = int(sti
-000098e0: 6e74 290a 2020 2020 2020 2020 2020 2020  nt).            
-000098f0: 2020 2020 2020 2020 2020 2020 7374 696e              stin
-00009900: 7420 3d20 7570 6461 7465 5b73 7469 6e74  t = update[stint
-00009910: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00009920: 2020 2020 2020 666f 7220 6b65 7920 696e        for key in
-00009930: 2064 6174 613a 0a20 2020 2020 2020 2020   data:.         
-00009940: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00009950: 6620 6b65 7920 696e 2073 7469 6e74 3a0a  f key in stint:.
-00009960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009970: 2020 2020 2020 2020 2020 2020 7661 6c20              val 
-00009980: 3d20 7374 696e 745b 6b65 795d 0a20 2020  = stint[key].   
+000048c0: 2020 2020 2020 6966 2028 6c61 7063 6e74        if (lapcnt
+000048d0: 203d 3d20 3029 2061 6e64 2028 2864 7276   == 0) and ((drv
+000048e0: 5f64 6174 615b 2754 696d 6527 5d5b 6c61  _data['Time'][la
+000048f0: 7063 6e74 5d20 2d20 746f 5f74 696d 6564  pcnt] - to_timed
+00004900: 656c 7461 2874 696d 6529 2920 3e20 7064  elta(time)) > pd
+00004910: 2e54 696d 6564 656c 7461 2835 2c20 276d  .Timedelta(5, 'm
+00004920: 696e 2729 293a 0a20 2020 2020 2020 2020  in')):.         
+00004930: 2020 2023 2069 676e 6f72 6520 616e 7920     # ignore any 
+00004940: 6461 7461 2077 6869 6368 2061 7272 6976  data which arriv
+00004950: 6573 206d 6f72 6520 7468 616e 2035 206d  es more than 5 m
+00004960: 696e 7574 6573 2062 6566 6f72 6520 7468  inutes before th
+00004970: 6520 656e 6420 6f66 2074 6865 2066 6972  e end of the fir
+00004980: 7374 206c 6170 2c20 6578 6365 7074 2027  st lap, except '
+00004990: 5069 744f 7574 270a 2020 2020 2020 2020  PitOut'.        
+000049a0: 2020 2020 6966 2028 2749 6e50 6974 2720      if ('InPit' 
+000049b0: 696e 2072 6573 7029 2061 6e64 2028 7265  in resp) and (re
+000049c0: 7370 5b27 496e 5069 7427 5d20 6973 2046  sp['InPit'] is F
+000049d0: 616c 7365 293a 0a20 2020 2020 2020 2020  alse):.         
+000049e0: 2020 2020 2020 2064 7276 5f64 6174 615b         drv_data[
+000049f0: 2750 6974 4f75 7454 696d 6527 5d5b 6c61  'PitOutTime'][la
+00004a00: 7063 6e74 5d20 3d20 746f 5f74 696d 6564  pcnt] = to_timed
+00004a10: 656c 7461 2874 696d 6529 0a20 2020 2020  elta(time).     
+00004a20: 2020 2020 2020 2020 2020 2070 6974 7374             pitst
+00004a30: 6f70 7320 3d20 3020 2023 2073 7065 6369  ops = 0  # speci
+00004a40: 616c 2068 6572 652c 2063 616e 2062 6520  al here, can be 
+00004a50: 6d75 6c74 6970 6c65 2074 696d 6573 2066  multiple times f
+00004a60: 6f72 206e 6f20 7265 6173 6f6e 2074 6865  or no reason the
+00004a70: 7265 666f 7265 2073 6574 207a 6572 6f20  refore set zero 
+00004a80: 696e 7374 6561 6420 6f66 202b 3d31 0a20  instead of +=1. 
+00004a90: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+00004aa0: 6e75 650a 0a20 2020 2020 2020 2023 2076  nue..        # v
+00004ab0: 616c 7565 7320 7768 6963 6820 6172 6520  alues which are 
+00004ac0: 7570 2074 6f20 6669 7665 2073 6563 6f6e  up to five secon
+00004ad0: 6473 206c 6174 6520 6172 6520 7374 696c  ds late are stil
+00004ae0: 6c20 636f 756e 7465 6420 746f 7761 7264  l counted toward
+00004af0: 7320 7468 6520 7072 6576 696f 7573 206c  s the previous l
+00004b00: 6170 0a20 2020 2020 2020 2023 2028 7365  ap.        # (se
+00004b10: 6374 6f72 2074 696d 6573 2c20 7370 6565  ctor times, spee
+00004b20: 6420 7472 6170 7320 616e 6420 6c61 7020  d traps and lap 
+00004b30: 7469 6d65 7329 0a20 2020 2020 2020 206c  times).        l
+00004b40: 6170 5f6f 6666 7365 7420 3d20 300a 2020  ap_offset = 0.  
+00004b50: 2020 2020 2020 6966 2028 6c61 7063 6e74        if (lapcnt
+00004b60: 203e 2030 2920 616e 6420 2874 6f5f 7469   > 0) and (to_ti
+00004b70: 6d65 6465 6c74 6128 7469 6d65 2920 2d20  medelta(time) - 
+00004b80: 6472 765f 6461 7461 5b27 5469 6d65 275d  drv_data['Time']
+00004b90: 5b6c 6170 636e 7420 2d20 315d 203c 2070  [lapcnt - 1] < p
+00004ba0: 642e 5469 6d65 6465 6c74 6128 352c 2027  d.Timedelta(5, '
+00004bb0: 7327 2929 3a0a 2020 2020 2020 2020 2020  s')):.          
+00004bc0: 2020 6c61 705f 6f66 6673 6574 203d 2031    lap_offset = 1
+00004bd0: 0a0a 2020 2020 2020 2020 6966 2027 5365  ..        if 'Se
+00004be0: 6374 6f72 7327 2069 6e20 7265 7370 2061  ctors' in resp a
+00004bf0: 6e64 2069 7369 6e73 7461 6e63 6528 7265  nd isinstance(re
+00004c00: 7370 5b27 5365 6374 6f72 7327 5d2c 2064  sp['Sectors'], d
+00004c10: 6963 7429 3a0a 2020 2020 2020 2020 2020  ict):.          
+00004c20: 2020 2320 736f 6d65 7469 6d65 7320 6974    # sometimes it
+00004c30: 2773 2061 206c 6973 7420 6275 7420 7468  's a list but th
+00004c40: 656e 2069 7420 6e65 7665 7220 636f 6e74  en it never cont
+00004c50: 6169 6e73 2076 616c 7565 732e 2e2e 0a20  ains values.... 
+00004c60: 2020 2020 2020 2020 2020 2066 6f72 2073             for s
+00004c70: 6e2c 2073 6563 746f 722c 2073 6573 7374  n, sector, sesst
+00004c80: 2069 6e20 2828 2730 272c 2027 5365 6374   in (('0', 'Sect
+00004c90: 6f72 3154 696d 6527 2c20 2753 6563 746f  or1Time', 'Secto
+00004ca0: 7231 5365 7373 696f 6e54 696d 6527 292c  r1SessionTime'),
+00004cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cd0: 2020 2020 2020 2028 2731 272c 2027 5365         ('1', 'Se
+00004ce0: 6374 6f72 3254 696d 6527 2c20 2753 6563  ctor2Time', 'Sec
+00004cf0: 746f 7232 5365 7373 696f 6e54 696d 6527  tor2SessionTime'
+00004d00: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00004d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d20: 2020 2020 2020 2020 2028 2732 272c 2027           ('2', '
+00004d30: 5365 6374 6f72 3354 696d 6527 2c20 2753  Sector3Time', 'S
+00004d40: 6563 746f 7233 5365 7373 696f 6e54 696d  ector3SessionTim
+00004d50: 6527 2929 3a0a 2020 2020 2020 2020 2020  e')):.          
+00004d60: 2020 2020 2020 6966 2076 616c 203a 3d20        if val := 
+00004d70: 7265 6375 7273 6976 655f 6469 6374 5f67  recursive_dict_g
+00004d80: 6574 2872 6573 702c 2027 5365 6374 6f72  et(resp, 'Sector
+00004d90: 7327 2c20 736e 2c20 2756 616c 7565 2729  s', sn, 'Value')
+00004da0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004db0: 2020 2020 2020 6472 765f 6461 7461 5b73        drv_data[s
+00004dc0: 6563 746f 725d 5b6c 6170 636e 7420 2d20  ector][lapcnt - 
+00004dd0: 6c61 705f 6f66 6673 6574 5d20 3d20 746f  lap_offset] = to
+00004de0: 5f74 696d 6564 656c 7461 2876 616c 290a  _timedelta(val).
+00004df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e00: 2020 2020 6472 765f 6461 7461 5b73 6573      drv_data[ses
+00004e10: 7374 5d5b 6c61 7063 6e74 202d 206c 6170  st][lapcnt - lap
+00004e20: 5f6f 6666 7365 745d 203d 2074 6f5f 7469  _offset] = to_ti
+00004e30: 6d65 6465 6c74 6128 7469 6d65 290a 0a20  medelta(time).. 
+00004e40: 2020 2020 2020 2069 6620 7661 6c20 3a3d         if val :=
+00004e50: 2072 6563 7572 7369 7665 5f64 6963 745f   recursive_dict_
+00004e60: 6765 7428 7265 7370 2c20 274c 6173 744c  get(resp, 'LastL
+00004e70: 6170 5469 6d65 272c 2027 5661 6c75 6527  apTime', 'Value'
+00004e80: 293a 0a20 2020 2020 2020 2020 2020 2023  ):.            #
+00004e90: 2069 6620 274c 6173 744c 6170 5469 6d65   if 'LastLapTime
+00004ea0: 2720 6973 2072 6563 6569 7665 6420 6c65  ' is received le
+00004eb0: 7373 2074 6861 6e20 6669 7665 2073 6563  ss than five sec
+00004ec0: 6f6e 6473 2061 6674 6572 2074 6865 2073  onds after the s
+00004ed0: 7461 7274 206f 6620 6120 6e65 7720 6c61  tart of a new la
+00004ee0: 702c 2069 7420 6973 2073 7469 6c6c 2061  p, it is still a
+00004ef0: 6464 6564 0a20 2020 2020 2020 2020 2020  dded.           
+00004f00: 2023 2074 6f20 7468 6520 6c61 7374 206c   # to the last l
+00004f10: 6170 0a20 2020 2020 2020 2020 2020 2076  ap.            v
+00004f20: 616c 203d 2074 6f5f 7469 6d65 6465 6c74  al = to_timedelt
+00004f30: 6128 7661 6c29 0a20 2020 2020 2020 2020  a(val).         
+00004f40: 2020 2069 6620 7661 6c2e 746f 7461 6c5f     if val.total_
+00004f50: 7365 636f 6e64 7328 2920 3c20 3135 303a  seconds() < 150:
+00004f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004f70: 2023 206c 6170 7320 7768 6963 6820 6172   # laps which ar
+00004f80: 6520 6c6f 6e67 6572 2074 6861 6e20 3135  e longer than 15
+00004f90: 3020 7365 636f 6e64 7320 6172 6520 6967  0 seconds are ig
+00004fa0: 6e6f 7265 643b 2075 7375 616c 6c79 2074  nored; usually t
+00004fb0: 6869 7320 6973 2074 6865 2063 6173 6520  his is the case 
+00004fc0: 6265 7477 6565 6e20 5131 2c20 5132 2061  between Q1, Q2 a
+00004fd0: 6e64 2051 330a 2020 2020 2020 2020 2020  nd Q3.          
+00004fe0: 2020 2020 2020 2320 6265 6361 7573 6520        # because 
+00004ff0: 616c 6c20 7468 7265 6520 7175 616c 6966  all three qualif
+00005000: 7969 6e67 2073 6573 7369 6f6e 7320 6172  ying sessions ar
+00005010: 6520 6f6e 6520 7365 7373 696f 6e20 6865  e one session he
+00005020: 7265 2e20 5468 6f73 6520 7469 6d65 7374  re. Those timest
+00005030: 616d 7073 2061 7265 206f 6674 656e 2077  amps are often w
+00005040: 726f 6e67 2061 6e64 0a20 2020 2020 2020  rong and.       
+00005050: 2020 2020 2020 2020 2023 2073 6f6d 6574           # somet
+00005060: 696d 6573 2061 7373 6f63 6961 7465 6420  imes associated 
+00005070: 7769 7468 2074 6865 2077 726f 6e67 206c  with the wrong l
+00005080: 6170 0a20 2020 2020 2020 2020 2020 2020  ap.             
+00005090: 2020 2064 7276 5f64 6174 615b 274c 6170     drv_data['Lap
+000050a0: 5469 6d65 275d 5b6c 6170 636e 7420 2d20  Time'][lapcnt - 
+000050b0: 6c61 705f 6f66 6673 6574 5d20 3d20 7661  lap_offset] = va
+000050c0: 6c0a 0a20 2020 2020 2020 2069 6620 2753  l..        if 'S
+000050d0: 7065 6564 7327 2069 6e20 7265 7370 3a0a  peeds' in resp:.
+000050e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000050f0: 7472 6170 6b65 792c 2074 7261 706e 616d  trapkey, trapnam
+00005100: 6520 696e 2028 2827 4931 272c 2027 5370  e in (('I1', 'Sp
+00005110: 6565 6449 3127 292c 2028 2749 3227 2c20  eedI1'), ('I2', 
+00005120: 2753 7065 6564 4932 2729 2c20 2827 464c  'SpeedI2'), ('FL
+00005130: 272c 2027 5370 6565 6446 4c27 292c 2028  ', 'SpeedFL'), (
+00005140: 2753 5427 2c20 2753 7065 6564 5354 2729  'ST', 'SpeedST')
+00005150: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00005160: 2020 2069 6620 7661 6c20 3a3d 2072 6563     if val := rec
+00005170: 7572 7369 7665 5f64 6963 745f 6765 7428  ursive_dict_get(
+00005180: 7265 7370 2c20 2753 7065 6564 7327 2c20  resp, 'Speeds', 
+00005190: 7472 6170 6b65 792c 2027 5661 6c75 6527  trapkey, 'Value'
+000051a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000051b0: 2020 2020 2020 2023 2073 7065 6564 2068         # speed h
+000051c0: 6173 2074 6f20 6265 2066 6c6f 6174 2062  as to be float b
+000051d0: 6563 6175 7365 2069 6e74 2064 6f65 7320  ecause int does 
+000051e0: 6e6f 7420 7375 7070 6f72 7420 4e61 4e0a  not support NaN.
+000051f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005200: 2020 2020 6966 2074 7261 706b 6579 203d      if trapkey =
+00005210: 3d20 2753 5427 3a0a 2020 2020 2020 2020  = 'ST':.        
+00005220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005230: 2320 7468 6520 5354 2074 7261 7020 7661  # the ST trap va
+00005240: 6c75 6520 6361 6e20 6f63 6375 7220 6561  lue can occur ea
+00005250: 726c 7920 656e 6f75 6768 2069 6e20 6120  rly enough in a 
+00005260: 6e65 7720 6c61 700a 2020 2020 2020 2020  new lap.        
+00005270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005280: 2320 7468 6174 2069 7420 6e65 6564 7320  # that it needs 
+00005290: 746f 2062 6520 6578 636c 7564 6564 2066  to be excluded f
+000052a0: 726f 6d20 7468 6520 7573 7561 6c20 6f66  rom the usual of
+000052b0: 6673 6574 0a20 2020 2020 2020 2020 2020  fset.           
+000052c0: 2020 2020 2020 2020 2020 2020 2023 206c               # l
+000052d0: 6f67 6963 2c20 7468 6572 6566 6f72 6520  ogic, therefore 
+000052e0: 7468 6520 6f66 6673 6574 2069 7320 6967  the offset is ig
+000052f0: 6e6f 7265 6420 6865 7265 0a20 2020 2020  nored here.     
+00005300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005310: 2020 2064 7276 5f64 6174 615b 7472 6170     drv_data[trap
+00005320: 6e61 6d65 5d5b 6c61 7063 6e74 5d20 3d20  name][lapcnt] = 
+00005330: 666c 6f61 7428 7661 6c29 0a20 2020 2020  float(val).     
+00005340: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00005350: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00005360: 2020 2020 2020 2020 2020 2020 2064 7276               drv
+00005370: 5f64 6174 615b 7472 6170 6e61 6d65 5d5b  _data[trapname][
+00005380: 6c61 7063 6e74 202d 206c 6170 5f6f 6666  lapcnt - lap_off
+00005390: 7365 745d 203d 2066 6c6f 6174 2876 616c  set] = float(val
+000053a0: 290a 0a20 2020 2020 2020 2069 6620 2749  )..        if 'I
+000053b0: 6e50 6974 2720 696e 2072 6573 703a 0a20  nPit' in resp:. 
+000053c0: 2020 2020 2020 2020 2020 2023 2027 496e             # 'In
+000053d0: 5069 7427 3a20 5472 7565 2069 7320 7265  Pit': True is re
+000053e0: 6365 6976 6564 206f 6e63 6520 7768 656e  ceived once when
+000053f0: 2065 6e74 6572 696e 6720 7069 7473 2c20   entering pits, 
+00005400: 4661 6c73 6520 6973 2072 6563 6569 7665  False is receive
+00005410: 6420 6f6e 6365 2077 6865 6e20 6c65 6176  d once when leav
+00005420: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+00005430: 6966 2072 6573 705b 2749 6e50 6974 275d  if resp['InPit']
+00005440: 2069 7320 5472 7565 3a0a 2020 2020 2020   is True:.      
+00005450: 2020 2020 2020 2020 2020 6966 2070 6974            if pit
+00005460: 7374 6f70 7320 3e3d 2030 3a0a 2020 2020  stops >= 0:.    
+00005470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005480: 6472 765f 6461 7461 5b27 5069 7449 6e54  drv_data['PitInT
+00005490: 696d 6527 5d5b 6c61 7063 6e74 5d20 3d20  ime'][lapcnt] = 
+000054a0: 746f 5f74 696d 6564 656c 7461 2874 696d  to_timedelta(tim
+000054b0: 6529 0a20 2020 2020 2020 2020 2020 2065  e).            e
+000054c0: 6c69 6620 2828 2827 4e75 6d62 6572 4f66  lif ((('NumberOf
+000054d0: 4c61 7073 2720 696e 2072 6573 7029 2061  Laps' in resp) a
+000054e0: 6e64 2072 6573 705b 274e 756d 6265 724f  nd resp['NumberO
+000054f0: 664c 6170 7327 5d20 3e20 6170 695f 6c61  fLaps'] > api_la
+00005500: 7063 6e74 290a 2020 2020 2020 2020 2020  pcnt).          
+00005510: 2020 2020 2020 2020 6f72 2028 6472 765f          or (drv_
+00005520: 6461 7461 5b27 5469 6d65 275d 5b6c 6170  data['Time'][lap
+00005530: 636e 745d 202d 2074 6f5f 7469 6d65 6465  cnt] - to_timede
+00005540: 6c74 6128 7469 6d65 2929 0a20 2020 2020  lta(time)).     
+00005550: 2020 2020 2020 2020 2020 2020 203c 2070               < p
+00005560: 642e 5469 6d65 6465 6c74 6128 352c 2027  d.Timedelta(5, '
+00005570: 7327 2929 3a0a 2020 2020 2020 2020 2020  s')):.          
+00005580: 2020 2020 2020 2320 7361 6d65 2072 6573        # same res
+00005590: 706f 6e73 6520 6c69 6e65 2061 7320 6265  ponse line as be
+000055a0: 6769 6e6e 696e 6720 6f66 206e 6578 7420  ginning of next 
+000055b0: 6c61 700a 2020 2020 2020 2020 2020 2020  lap.            
+000055c0: 2020 2020 2320 6f72 2062 6567 696e 6e69      # or beginni
+000055d0: 6e67 206f 6620 6e65 7874 206c 6170 206c  ng of next lap l
+000055e0: 6573 7320 7468 616e 2035 2073 6563 6f6e  ess than 5 secon
+000055f0: 6473 2061 7761 790a 2020 2020 2020 2020  ds away.        
+00005600: 2020 2020 2020 2020 6472 765f 6461 7461          drv_data
+00005610: 5b27 5069 744f 7574 5469 6d65 275d 5b6c  ['PitOutTime'][l
+00005620: 6170 636e 7420 2b20 315d 203d 2074 6f5f  apcnt + 1] = to_
+00005630: 7469 6d65 6465 6c74 6128 7469 6d65 2920  timedelta(time) 
+00005640: 2023 2061 6464 2074 6f20 6e65 7874 206c   # add to next l
+00005650: 6170 0a20 2020 2020 2020 2020 2020 2020  ap.             
+00005660: 2020 2070 6974 7374 6f70 7320 2b3d 2031     pitstops += 1
+00005670: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00005680: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00005690: 2020 2064 7276 5f64 6174 615b 2750 6974     drv_data['Pit
+000056a0: 4f75 7454 696d 6527 5d5b 6c61 7063 6e74  OutTime'][lapcnt
+000056b0: 5d20 3d20 746f 5f74 696d 6564 656c 7461  ] = to_timedelta
+000056c0: 2874 696d 6529 2020 2320 6164 6420 746f  (time)  # add to
+000056d0: 2063 7572 7265 6e74 206c 6170 0a20 2020   current lap.   
+000056e0: 2020 2020 2020 2020 2020 2020 2070 6974               pit
+000056f0: 7374 6f70 7320 2b3d 2031 0a0a 2020 2020  stops += 1..    
+00005700: 2020 2020 2320 4765 7420 7361 7665 2069      # Get save i
+00005710: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
+00005720: 2070 6572 736f 6e61 6c20 6265 7374 206c   personal best l
+00005730: 6170 2074 696d 6573 2061 7420 7468 6520  ap times at the 
+00005740: 7469 6d65 7374 616d 700a 2020 2020 2020  timestamp.      
+00005750: 2020 2320 6174 2077 6869 6368 2074 6869    # at which thi
+00005760: 7320 696e 666f 726d 6174 696f 6e20 7761  s information wa
+00005770: 7320 7265 6365 6976 6564 2e0a 2020 2020  s received..    
+00005780: 2020 2020 2320 5768 656e 6576 6572 2061      # Whenever a
+00005790: 206c 6170 2069 7320 6465 6c65 7465 6420   lap is deleted 
+000057a0: 2869 6620 7468 6174 2068 6170 7065 6e73  (if that happens
+000057b0: 2071 7569 636b 6c79 2061 6674 6572 2069   quickly after i
+000057c0: 7420 7761 7320 7365 7429 2c0a 2020 2020  t was set),.    
+000057d0: 2020 2020 2320 7468 6520 7072 6576 696f      # the previo
+000057e0: 7573 2027 4265 7374 4c61 7054 696d 6527  us 'BestLapTime'
+000057f0: 2076 616c 7565 2069 7320 7365 6e74 2061   value is sent a
+00005800: 6761 696e 2e20 5468 6572 6520 6973 2073  gain. There is s
+00005810: 6f6d 6520 6578 7472 610a 2020 2020 2020  ome extra.      
+00005820: 2020 2320 6c6f 6769 6320 6174 2074 6865    # logic at the
+00005830: 6e20 656e 6420 7468 6174 2063 6f72 7265  n end that corre
+00005840: 6374 6c79 206d 6172 6b73 2070 6572 736f  ctly marks perso
+00005850: 6e61 6c20 6265 7374 206c 6170 7320 6261  nal best laps ba
+00005860: 7365 6420 6f6e 0a20 2020 2020 2020 2023  sed on.        #
+00005870: 2074 6865 2064 6174 6120 7468 6174 2069   the data that i
+00005880: 7320 7361 7665 6420 6865 7265 2e0a 2020  s saved here..  
+00005890: 2020 2020 2020 6966 2076 616c 203a 3d20        if val := 
+000058a0: 7265 6375 7273 6976 655f 6469 6374 5f67  recursive_dict_g
+000058b0: 6574 2872 6573 702c 2027 4265 7374 4c61  et(resp, 'BestLa
+000058c0: 7054 696d 6527 2c20 2756 616c 7565 2729  pTime', 'Value')
+000058d0: 3a0a 2020 2020 2020 2020 2020 2020 7065  :.            pe
+000058e0: 7273 6f6e 616c 5f62 6573 745f 6c61 705f  rsonal_best_lap_
+000058f0: 7469 6d65 732e 6170 7065 6e64 280a 2020  times.append(.  
+00005900: 2020 2020 2020 2020 2020 2020 2020 2874                (t
+00005910: 6f5f 7469 6d65 6465 6c74 6128 7469 6d65  o_timedelta(time
+00005920: 292c 2074 6f5f 7469 6d65 6465 6c74 6128  ), to_timedelta(
+00005930: 7661 6c29 290a 2020 2020 2020 2020 2020  val)).          
+00005940: 2020 290a 0a20 2020 2020 2020 2023 2043    )..        # C
+00005950: 7265 6174 6520 6170 7072 6f78 696d 6174  reate approximat
+00005960: 6520 2873 7562 2973 6573 7369 6f6e 2028  e (sub)session (
+00005970: 692e 652e 2071 7561 6c69 2920 7370 6c69  i.e. quali) spli
+00005980: 7420 7469 6d65 7320 6279 0a20 2020 2020  t times by.     
+00005990: 2020 2023 2028 6d69 7329 7573 696e 6720     # (mis)using 
+000059a0: 7468 6520 7365 7373 696f 6e20 6e75 6d62  the session numb
+000059b0: 6572 2063 6f75 6e74 6572 2066 726f 6d20  er counter from 
+000059c0: 2742 6573 744c 6170 5469 6d65 7327 2e0a  'BestLapTimes'..
+000059d0: 2020 2020 2020 2020 2320 284e 6f74 653a          # (Note:
+000059e0: 2074 686f 7365 206c 6170 2074 696d 6573   those lap times
+000059f0: 2063 616e 6e6f 7420 6265 2075 7365 6420   cannot be used 
+00005a00: 666f 7220 636f 7272 6563 7420 7065 7273  for correct pers
+00005a10: 6f6e 616c 2062 6573 740a 2020 2020 2020  onal best.      
+00005a20: 2020 2320 2064 6574 6563 7469 6f6e 2c20    #  detection, 
+00005a30: 6265 6361 7573 6520 7468 6520 7072 6576  because the prev
+00005a40: 696f 7573 2076 616c 7565 2069 7320 6e6f  ious value is no
+00005a50: 7420 7265 7365 6e74 2068 6572 6520 7768  t resent here wh
+00005a60: 656e 2061 206c 6170 0a20 2020 2020 2020  en a lap.       
+00005a70: 2023 2020 6973 2064 656c 6574 6564 2e29   #  is deleted.)
+00005a80: 0a20 2020 2020 2020 2069 6620 2876 616c  .        if (val
+00005a90: 203a 3d20 7265 7370 2e67 6574 2827 4265   := resp.get('Be
+00005aa0: 7374 4c61 7054 696d 6573 2729 2920 616e  stLapTimes')) an
+00005ab0: 6420 6973 696e 7374 616e 6365 2876 616c  d isinstance(val
+00005ac0: 2c20 6469 6374 293a 0a20 2020 2020 2020  , dict):.       
+00005ad0: 2020 2020 2073 6573 7369 6f6e 5f6e 203d       session_n =
+00005ae0: 2069 6e74 286c 6973 7428 7661 6c2e 6b65   int(list(val.ke
+00005af0: 7973 2829 295b 305d 290a 2020 2020 2020  ys())[0]).      
+00005b00: 2020 2020 2020 6966 2028 7365 7373 696f        if (sessio
+00005b10: 6e5f 6e20 2b20 3129 203e 206c 656e 2873  n_n + 1) > len(s
+00005b20: 6573 7369 6f6e 5f73 706c 6974 5f74 696d  ession_split_tim
+00005b30: 6573 293a 0a20 2020 2020 2020 2020 2020  es):.           
+00005b40: 2020 2020 2073 6573 7369 6f6e 5f73 706c       session_spl
+00005b50: 6974 5f74 696d 6573 2e61 7070 656e 6428  it_times.append(
+00005b60: 746f 5f74 696d 6564 656c 7461 2874 696d  to_timedelta(tim
+00005b70: 6529 290a 0a20 2020 2020 2020 2023 206e  e))..        # n
+00005b80: 6577 206c 6170 3b20 6372 6561 7465 206e  ew lap; create n
+00005b90: 6578 7420 726f 770a 2020 2020 2020 2020  ext row.        
+00005ba0: 6966 2027 4e75 6d62 6572 4f66 4c61 7073  if 'NumberOfLaps
+00005bb0: 2720 696e 2072 6573 7020 616e 6420 7265  ' in resp and re
+00005bc0: 7370 5b27 4e75 6d62 6572 4f66 4c61 7073  sp['NumberOfLaps
+00005bd0: 275d 203e 2061 7069 5f6c 6170 636e 743a  '] > api_lapcnt:
+00005be0: 0a20 2020 2020 2020 2020 2020 2061 7069  .            api
+00005bf0: 5f6c 6170 636e 7420 2b3d 2031 0a20 2020  _lapcnt += 1.   
+00005c00: 2020 2020 2020 2020 2023 206d 616b 6520           # make 
+00005c10: 7375 7265 2074 6865 2063 6172 2061 6374  sure the car act
+00005c20: 7561 6c6c 7920 6472 6f76 6520 6f75 7420  ually drove out 
+00005c30: 6f66 2074 6865 2070 6974 7320 616c 7265  of the pits alre
+00005c40: 6164 793b 2069 7420 6361 6e27 7420 6265  ady; it can't be
+00005c50: 2061 206e 6577 206c 6170 2069 6620 6974   a new lap if it
+00005c60: 2064 6964 6e27 740a 2020 2020 2020 2020   didn't.        
+00005c70: 2020 2020 6966 2070 6974 7374 6f70 7320      if pitstops 
+00005c80: 3e3d 2030 3a0a 2020 2020 2020 2020 2020  >= 0:.          
+00005c90: 2020 2020 2020 6472 765f 6461 7461 5b27        drv_data['
+00005ca0: 5469 6d65 275d 5b6c 6170 636e 745d 203d  Time'][lapcnt] =
+00005cb0: 2074 6f5f 7469 6d65 6465 6c74 6128 7469   to_timedelta(ti
+00005cc0: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
+00005cd0: 2020 2020 6472 765f 6461 7461 5b27 4e75      drv_data['Nu
+00005ce0: 6d62 6572 4f66 4c61 7073 275d 5b6c 6170  mberOfLaps'][lap
+00005cf0: 636e 745d 203d 206c 6170 636e 7420 2b20  cnt] = lapcnt + 
+00005d00: 3120 2023 2064 6f6e 2774 2075 7365 2046  1  # don't use F
+00005d10: 3127 7320 6c61 7020 636f 756e 743b 206f  1's lap count; o
+00005d20: 7572 7320 6973 2062 6574 7465 720a 2020  urs is better.  
+00005d30: 2020 2020 2020 2020 2020 2020 2020 6472                dr
+00005d40: 765f 6461 7461 5b27 4e75 6d62 6572 4f66  v_data['NumberOf
+00005d50: 5069 7453 746f 7073 275d 5b6c 6170 636e  PitStops'][lapcn
+00005d60: 745d 203d 2070 6974 7374 6f70 730a 2020  t] = pitstops.  
+00005d70: 2020 2020 2020 2020 2020 2020 2020 6472                dr
+00005d80: 765f 6461 7461 5b27 4472 6976 6572 275d  v_data['Driver']
+00005d90: 5b6c 6170 636e 745d 203d 2064 7276 0a20  [lapcnt] = drv. 
+00005da0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00005db0: 6170 636e 7420 2b3d 2031 0a0a 2020 2020  apcnt += 1..    
+00005dc0: 6966 206c 6170 636e 7420 3d3d 2030 3a20  if lapcnt == 0: 
+00005dd0: 2023 206e 6f20 6461 7461 2061 7420 616c   # no data at al
+00005de0: 6c20 666f 7220 7468 6973 2064 7269 7665  l for this drive
+00005df0: 720a 2020 2020 2020 2020 7265 7475 726e  r.        return
+00005e00: 204e 6f6e 652c 204e 6f6e 650a 0a20 2020   None, None..   
+00005e10: 2023 2064 6f6e 6520 7265 6164 696e 6720   # done reading 
+00005e20: 7468 6520 6461 7461 2c20 646f 2070 6f73  the data, do pos
+00005e30: 7470 726f 6365 7373 696e 670a 0a20 2020  tprocessing..   
+00005e40: 2064 6566 2064 6174 615f 696e 5f6c 6170   def data_in_lap
+00005e50: 286c 6170 5f6e 293a 0a20 2020 2020 2020  (lap_n):.       
+00005e60: 2072 656c 6576 616e 7420 3d20 2827 5365   relevant = ('Se
+00005e70: 6374 6f72 3154 696d 6527 2c20 2753 6563  ctor1Time', 'Sec
+00005e80: 746f 7232 5469 6d65 272c 2027 5365 6374  tor2Time', 'Sect
+00005e90: 6f72 3354 696d 6527 2c20 2753 7065 6564  or3Time', 'Speed
+00005ea0: 4931 272c 2027 5370 6565 6449 3227 2c0a  I1', 'SpeedI2',.
+00005eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ec0: 2020 2020 2753 7065 6564 464c 272c 2027      'SpeedFL', '
+00005ed0: 5370 6565 6453 5427 2c20 274c 6170 5469  SpeedST', 'LapTi
+00005ee0: 6d65 2729 0a20 2020 2020 2020 2066 6f72  me').        for
+00005ef0: 2063 6f6c 2069 6e20 7265 6c65 7661 6e74   col in relevant
+00005f00: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00005f10: 206e 6f74 2070 642e 6973 6e75 6c6c 2864   not pd.isnull(d
+00005f20: 7276 5f64 6174 615b 636f 6c5d 5b6c 6170  rv_data[col][lap
+00005f30: 5f6e 5d29 3a0a 2020 2020 2020 2020 2020  _n]):.          
+00005f40: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+00005f50: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+00005f60: 2046 616c 7365 0a0a 2020 2020 2320 274e   False..    # 'N
+00005f70: 756d 6265 724f 664c 6170 7327 2061 6c77  umberOfLaps' alw
+00005f80: 6179 7320 696e 7472 6f64 7563 6573 2061  ays introduces a
+00005f90: 206e 6577 206c 6170 2028 6361 6e20 6265   new lap (can be
+00005fa0: 2061 2070 7265 7669 6f75 7320 6f6e 6529   a previous one)
+00005fb0: 2062 7574 2073 6f6d 6574 696d 6573 2074   but sometimes t
+00005fc0: 6865 7265 2069 7320 6f6e 6520 6d6f 7265  here is one more
+00005fd0: 206c 6170 2061 7420 7468 6520 656e 640a   lap at the end.
+00005fe0: 2020 2020 2320 696e 2074 6869 7320 6361      # in this ca
+00005ff0: 7365 2074 6865 2064 6174 6120 7769 6c6c  se the data will
+00006000: 2062 6520 6164 6465 6420 6173 2075 7375   be added as usu
+00006010: 616c 2061 626f 7665 2c20 6c61 7020 636f  al above, lap co
+00006020: 756e 7420 616e 6420 7069 7420 7374 6f70  unt and pit stop
+00006030: 7320 6172 6520 6164 6465 6420 6865 7265  s are added here
+00006040: 2061 6e64 2074 6865 2027 5469 6d65 2720   and the 'Time' 
+00006050: 6973 0a20 2020 2023 2063 616c 6375 6c61  is.    # calcula
+00006060: 7465 6420 6265 6c6f 7720 6672 6f6d 2073  ted below from s
+00006070: 6563 746f 7220 7469 6d65 730a 2020 2020  ector times.    
+00006080: 6966 2064 6174 615f 696e 5f6c 6170 286c  if data_in_lap(l
+00006090: 6170 636e 7429 3a0a 2020 2020 2020 2020  apcnt):.        
+000060a0: 6472 765f 6461 7461 5b27 4e75 6d62 6572  drv_data['Number
+000060b0: 4f66 4c61 7073 275d 5b6c 6170 636e 745d  OfLaps'][lapcnt]
+000060c0: 203d 206c 6170 636e 7420 2b20 310a 2020   = lapcnt + 1.  
+000060d0: 2020 2020 2020 6472 765f 6461 7461 5b27        drv_data['
+000060e0: 4e75 6d62 6572 4f66 5069 7453 746f 7073  NumberOfPitStops
+000060f0: 275d 5b6c 6170 636e 745d 203d 2070 6974  '][lapcnt] = pit
+00006100: 7374 6f70 730a 2020 2020 2020 2020 6472  stops.        dr
+00006110: 765f 6461 7461 5b27 4472 6976 6572 275d  v_data['Driver']
+00006120: 5b6c 6170 636e 745d 203d 2064 7276 0a20  [lapcnt] = drv. 
+00006130: 2020 2065 6c73 653a 2020 2320 6966 2074     else:  # if t
+00006140: 6865 7265 2077 6173 206e 6f20 6d6f 7265  here was no more
+00006150: 2064 6174 6120 6166 7465 7220 7468 6520   data after the 
+00006160: 6c61 7374 206c 6170 2063 6f75 6e74 2069  last lap count i
+00006170: 6e63 7265 6173 652c 0a20 2020 2020 2020  ncrease,.       
+00006180: 2023 2064 656c 6574 6520 7468 6520 6c61   # delete the la
+00006190: 7374 2065 6d70 7479 2072 6563 6f72 640a  st empty record.
+000061a0: 2020 2020 2020 2020 666f 7220 6b65 7920          for key 
+000061b0: 696e 2064 7276 5f64 6174 612e 6b65 7973  in drv_data.keys
+000061c0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000061d0: 6472 765f 6461 7461 5b6b 6579 5d20 3d20  drv_data[key] = 
+000061e0: 6472 765f 6461 7461 5b6b 6579 5d5b 3a2d  drv_data[key][:-
+000061f0: 315d 0a20 2020 2069 6620 6e6f 7420 6461  1].    if not da
+00006200: 7461 5f69 6e5f 6c61 7028 3029 3a20 2023  ta_in_lap(0):  #
+00006210: 2072 656d 6f76 6520 6669 7273 7420 6c61   remove first la
+00006220: 7020 6966 2074 6865 7265 2773 206e 6f20  p if there's no 
+00006230: 6461 7461 3b0a 2020 2020 2020 2020 2320  data;.        # 
+00006240: 2270 7365 7564 6f20 6f75 746c 6170 2220  "pseudo outlap" 
+00006250: 7468 6174 2064 6964 6e27 7420 6578 6973  that didn't exis
+00006260: 740a 2020 2020 2020 2020 666f 7220 6b65  t.        for ke
+00006270: 7920 696e 2064 7276 5f64 6174 612e 6b65  y in drv_data.ke
+00006280: 7973 2829 3a0a 2020 2020 2020 2020 2020  ys():.          
+00006290: 2020 6472 765f 6461 7461 5b6b 6579 5d20    drv_data[key] 
+000062a0: 3d20 6472 765f 6461 7461 5b6b 6579 5d5b  = drv_data[key][
+000062b0: 313a 5d0a 2020 2020 2020 2020 6472 765f  1:].        drv_
+000062c0: 6461 7461 5b27 4e75 6d62 6572 4f66 4c61  data['NumberOfLa
+000062d0: 7073 275d 203d 206c 6973 7428 6d61 7028  ps'] = list(map(
+000062e0: 6c61 6d62 6461 206e 3a20 6e20 2d20 312c  lambda n: n - 1,
+000062f0: 2064 7276 5f64 6174 615b 274e 756d 6265   drv_data['Numbe
+00006300: 724f 664c 6170 7327 5d29 2920 2023 2072  rOfLaps']))  # r
+00006310: 6564 7563 6520 6561 6368 206c 6170 2063  educe each lap c
+00006320: 6f75 6e74 2062 7920 6f6e 650a 0a20 2020  ount by one..   
+00006330: 2069 6620 6e6f 7420 6472 765f 6461 7461   if not drv_data
+00006340: 5b27 5469 6d65 275d 3a0a 2020 2020 2020  ['Time']:.      
+00006350: 2020 2320 656e 7375 7265 2074 6861 7420    # ensure that 
+00006360: 7468 6572 6520 6973 2073 7469 6c6c 2064  there is still d
+00006370: 6174 6120 6c65 6674 2061 6674 6572 2070  ata left after p
+00006380: 6f74 656e 7469 616c 6c79 2072 656d 6f76  otentially remov
+00006390: 696e 6720 6120 6c61 700a 2020 2020 2020  ing a lap.      
+000063a0: 2020 7265 7475 726e 2064 7276 5f64 6174    return drv_dat
+000063b0: 612c 2073 6573 7369 6f6e 5f73 706c 6974  a, session_split
+000063c0: 5f74 696d 6573 0a0a 2020 2020 666f 7220  _times..    for 
+000063d0: 6920 696e 2072 616e 6765 286c 656e 2864  i in range(len(d
+000063e0: 7276 5f64 6174 615b 2754 696d 6527 5d29  rv_data['Time'])
+000063f0: 293a 0a20 2020 2020 2020 2073 6563 746f  ):.        secto
+00006400: 725f 7375 6d20 3d20 6461 7465 7469 6d65  r_sum = datetime
+00006410: 2e74 696d 6564 656c 7461 2830 290a 2020  .timedelta(0).  
+00006420: 2020 2020 2020 6e61 5f73 6563 746f 7273        na_sectors
+00006430: 203d 206c 6973 7428 2920 2023 206c 6973   = list()  # lis
+00006440: 7420 6f66 206b 6579 7320 666f 7220 6d69  t of keys for mi
+00006450: 7373 696e 6720 7365 6374 6f72 2074 696d  ssing sector tim
+00006460: 6573 0a20 2020 2020 2020 2066 6f72 206b  es.        for k
+00006470: 6579 2069 6e20 2827 5365 6374 6f72 3154  ey in ('Sector1T
+00006480: 696d 6527 2c20 2753 6563 746f 7232 5469  ime', 'Sector2Ti
+00006490: 6d65 272c 2027 5365 6374 6f72 3354 696d  me', 'Sector3Tim
+000064a0: 6527 293a 0a20 2020 2020 2020 2020 2020  e'):.           
+000064b0: 2073 7420 3d20 6472 765f 6461 7461 5b6b   st = drv_data[k
+000064c0: 6579 5d5b 695d 0a20 2020 2020 2020 2020  ey][i].         
+000064d0: 2020 2069 6620 7064 2e69 736e 6128 7374     if pd.isna(st
+000064e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000064f0: 2020 206e 615f 7365 6374 6f72 732e 6170     na_sectors.ap
+00006500: 7065 6e64 286b 6579 290a 2020 2020 2020  pend(key).      
+00006510: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+00006520: 7565 0a20 2020 2020 2020 2020 2020 2073  ue.            s
+00006530: 6563 746f 725f 7375 6d20 2b3d 2073 740a  ector_sum += st.
+00006540: 0a20 2020 2020 2020 2023 2063 6865 636b  .        # check
+00006550: 2066 6f72 2069 6e63 6f72 7265 6374 206c   for incorrect l
+00006560: 6170 2074 696d 6573 2061 6e64 2072 656d  ap times and rem
+00006570: 6f76 6520 7468 656d 0a20 2020 2020 2020  ove them.       
+00006580: 2023 2066 6978 6573 2047 4823 3136 3720   # fixes GH#167 
+00006590: 616d 6f6e 6720 6f74 6865 7273 0a20 2020  among others.   
+000065a0: 2020 2020 2069 6620 7365 6374 6f72 5f73       if sector_s
+000065b0: 756d 203e 2064 7276 5f64 6174 615b 274c  um > drv_data['L
+000065c0: 6170 5469 6d65 275d 5b69 5d3a 0a20 2020  apTime'][i]:.   
+000065d0: 2020 2020 2020 2020 2064 7276 5f64 6174           drv_dat
+000065e0: 615b 274c 6170 5469 6d65 275d 5b69 5d20  a['LapTime'][i] 
+000065f0: 3d20 7064 2e4e 6154 0a20 2020 2020 2020  = pd.NaT.       
+00006600: 2020 2020 2069 6e74 6567 7269 7479 5f65       integrity_e
+00006610: 7272 6f72 732e 6170 7065 6e64 2869 202b  rrors.append(i +
+00006620: 2031 290a 0a20 2020 2020 2020 2069 6620   1)..        if 
+00006630: 6920 3d3d 2030 3a0a 2020 2020 2020 2020  i == 0:.        
+00006640: 2020 2020 2320 6f6e 6c79 2064 6f20 666f      # only do fo
+00006650: 6c6c 6f77 696e 6720 636f 7272 6563 7469  llowing correcti
+00006660: 6f6e 7320 666f 7220 326e 6420 6c61 7020  ons for 2nd lap 
+00006670: 616e 6420 6f6e 7761 7264 730a 2020 2020  and onwards.    
+00006680: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+00006690: 0a0a 2020 2020 2020 2020 2320 5468 6520  ..        # The 
+000066a0: 4150 4920 6f6e 6c79 2073 656e 6473 2061  API only sends a
+000066b0: 6e64 2075 7064 6174 6520 6966 2061 2073  nd update if a s
+000066c0: 7461 7465 2063 6861 6e67 6573 2c20 7468  tate changes, th
+000066d0: 6572 6566 6f72 652c 2069 6620 7477 6f0a  erefore, if two.
+000066e0: 2020 2020 2020 2020 2320 6c61 7020 7469          # lap ti
+000066f0: 6d65 7320 6f72 2073 6563 746f 7220 7469  mes or sector ti
+00006700: 6d65 7320 6172 6520 6578 6163 746c 7920  mes are exactly 
+00006710: 6571 7561 6c2c 2074 6865 2073 6563 6f6e  equal, the secon
+00006720: 6420 7661 6c75 6520 7769 6c6c 0a20 2020  d value will.   
+00006730: 2020 2020 2023 2062 6520 6d69 7373 696e       # be missin
+00006740: 672e 204d 6973 7369 6e67 2073 6563 746f  g. Missing secto
+00006750: 7220 7469 6d65 7320 616e 6420 6c61 7020  r times and lap 
+00006760: 7469 6d65 7320 6172 6520 6361 6c63 756c  times are calcul
+00006770: 6174 6564 2068 6572 650a 2020 2020 2020  ated here.      
+00006780: 2020 2320 6261 7365 6420 6f6e 2074 6865    # based on the
+00006790: 2061 7661 696c 6162 6c65 2076 616c 7565   available value
+000067a0: 7320 666f 7220 6120 6c61 7020 286d 6178  s for a lap (max
+000067b0: 206f 6e65 206d 6179 2062 6520 6d69 7373   one may be miss
+000067c0: 696e 6729 2e20 4966 0a20 2020 2020 2020  ing). If.       
+000067d0: 2023 2074 6865 2063 616c 6375 6c61 7465   # the calculate
+000067e0: 6420 7661 6c75 6520 6d61 7463 6865 7320  d value matches 
+000067f0: 7468 6520 7072 6576 696f 7573 2076 616c  the previous val
+00006800: 7565 2c20 6974 2077 696c 6c20 6265 2073  ue, it will be s
+00006810: 6574 2e0a 0a20 2020 2020 2020 2023 206c  et...        # l
+00006820: 6170 2074 696d 6520 6973 206d 6973 7369  ap time is missi
+00006830: 6e67 0a20 2020 2020 2020 2069 6620 286e  ng.        if (n
+00006840: 6f74 206e 615f 7365 6374 6f72 7329 2061  ot na_sectors) a
+00006850: 6e64 2070 642e 6973 6e61 2864 7276 5f64  nd pd.isna(drv_d
+00006860: 6174 615b 274c 6170 5469 6d65 275d 5b69  ata['LapTime'][i
+00006870: 5d29 205c 0a20 2020 2020 2020 2020 2020  ]) \.           
+00006880: 2020 2020 2061 6e64 2028 6472 765f 6461       and (drv_da
+00006890: 7461 5b27 4c61 7054 696d 6527 5d5b 6920  ta['LapTime'][i 
+000068a0: 2d20 315d 203d 3d20 7365 6374 6f72 5f73  - 1] == sector_s
+000068b0: 756d 293a 0a0a 2020 2020 2020 2020 2020  um):..          
+000068c0: 2020 6472 765f 6461 7461 5b27 4c61 7054    drv_data['LapT
+000068d0: 696d 6527 5d5b 695d 203d 2073 6563 746f  ime'][i] = secto
+000068e0: 725f 7375 6d0a 0a20 2020 2020 2020 2023  r_sum..        #
+000068f0: 206f 6e65 2073 6563 746f 7220 7469 6d65   one sector time
+00006900: 2069 7320 6d69 7373 696e 670a 2020 2020   is missing.    
+00006910: 2020 2020 656c 6966 2028 6c65 6e28 6e61      elif (len(na
+00006920: 5f73 6563 746f 7273 2920 3d3d 2031 2920  _sectors) == 1) 
+00006930: 616e 6420 6e6f 7420 7064 2e69 736e 6128  and not pd.isna(
+00006940: 6472 765f 6461 7461 5b27 4c61 7054 696d  drv_data['LapTim
+00006950: 6527 5d5b 695d 293a 0a20 2020 2020 2020  e'][i]):.       
+00006960: 2020 2020 2023 2063 7265 6174 6520 6120       # create a 
+00006970: 6c69 7374 2077 6974 6820 7468 6520 7477  list with the tw
+00006980: 6f20 6b65 7973 2066 6f72 2061 7661 696c  o keys for avail
+00006990: 6162 6c65 2073 6563 746f 7220 7469 6d65  able sector time
+000069a0: 730a 2020 2020 2020 2020 2020 2020 7265  s.            re
+000069b0: 665f 7365 6320 3d20 5b27 5365 6374 6f72  f_sec = ['Sector
+000069c0: 3154 696d 6527 2c20 2753 6563 746f 7232  1Time', 'Sector2
+000069d0: 5469 6d65 272c 2027 5365 6374 6f72 3354  Time', 'Sector3T
+000069e0: 696d 6527 5d0a 2020 2020 2020 2020 2020  ime'].          
+000069f0: 2020 7265 665f 7365 632e 7265 6d6f 7665    ref_sec.remove
+00006a00: 286e 615f 7365 6374 6f72 735b 305d 290a  (na_sectors[0]).
+00006a10: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00006a20: 2873 6563 3120 3a3d 2028 6472 765f 6461  (sec1 := (drv_da
+00006a30: 7461 5b27 4c61 7054 696d 6527 5d5b 695d  ta['LapTime'][i]
+00006a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006a50: 2020 2020 2020 2020 2020 2d20 6472 765f            - drv_
+00006a60: 6461 7461 5b72 6566 5f73 6563 5b30 5d5d  data[ref_sec[0]]
+00006a70: 5b69 5d0a 2020 2020 2020 2020 2020 2020  [i].            
+00006a80: 2020 2020 2020 2020 2020 2020 202d 2064               - d
+00006a90: 7276 5f64 6174 615b 7265 665f 7365 635b  rv_data[ref_sec[
+00006aa0: 315d 5d5b 695d 2929 205c 0a20 2020 2020  1]][i])) \.     
+00006ab0: 2020 2020 2020 2020 2020 2020 2020 203d                 =
+00006ac0: 3d20 6472 765f 6461 7461 5b6e 615f 7365  = drv_data[na_se
+00006ad0: 6374 6f72 735b 305d 5d5b 6920 2d20 315d  ctors[0]][i - 1]
+00006ae0: 3a0a 0a20 2020 2020 2020 2020 2020 2020  :..             
+00006af0: 2020 2064 7276 5f64 6174 615b 6e61 5f73     drv_data[na_s
+00006b00: 6563 746f 7273 5b30 5d5d 5b69 5d20 3d20  ectors[0]][i] = 
+00006b10: 7365 6331 0a0a 2020 2020 2320 6c61 7020  sec1..    # lap 
+00006b20: 7469 6d65 2073 796e 633b 2063 6865 636b  time sync; check
+00006b30: 2077 6869 6368 2073 6563 746f 7220 7469   which sector ti
+00006b40: 6d65 2077 6173 2074 7269 6767 6572 6564  me was triggered
+00006b50: 2077 6974 6820 7468 6520 6c6f 7765 7374   with the lowest
+00006b60: 206c 6174 656e 6379 0a20 2020 2023 2053   latency.    # S
+00006b70: 6563 746f 7233 5365 7373 696f 6e54 696d  ector3SessionTim
+00006b80: 6520 3d3d 2065 6e64 206f 6620 6c61 700a  e == end of lap.
+00006b90: 2020 2020 2320 5365 6374 6f72 3253 6573      # Sector2Ses
+00006ba0: 7369 6f6e 5469 6d65 202b 2053 6563 746f  sionTime + Secto
+00006bb0: 7233 5469 6d65 203d 3d20 656e 6420 6f66  r3Time == end of
+00006bc0: 206c 6170 0a20 2020 2023 2053 6563 746f   lap.    # Secto
+00006bd0: 7231 5365 7373 696f 6e54 696d 6520 2b20  r1SessionTime + 
+00006be0: 5365 6374 6f72 3254 696d 6520 2b20 5365  Sector2Time + Se
+00006bf0: 6374 6f72 3354 696d 6520 3d3d 2065 6e64  ctor3Time == end
+00006c00: 206f 6620 6c61 700a 2020 2020 2320 616c   of lap.    # al
+00006c10: 6c20 6f66 2074 6865 7365 2074 6872 6565  l of these three
+00006c20: 2068 6176 6520 736c 6967 6874 6c79 2064   have slightly d
+00006c30: 6966 6665 7265 6e74 2074 696d 6573 3b20  ifferent times; 
+00006c40: 7461 6b65 2065 6172 6c69 6573 7420 6f6e  take earliest on
+00006c50: 6520 2d3e 206d 6f73 7420 6578 6163 7420  e -> most exact 
+00006c60: 6265 6361 7573 6520 6361 6e27 7420 7472  because can't tr
+00006c70: 6967 6765 7220 746f 6f20 6561 726c 790a  igger too early.
+00006c80: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00006c90: 6765 286c 656e 2864 7276 5f64 6174 615b  ge(len(drv_data[
+00006ca0: 2754 696d 6527 5d29 293a 0a20 2020 2020  'Time'])):.     
+00006cb0: 2020 2073 6563 746f 725f 7375 6d20 3d20     sector_sum = 
+00006cc0: 7064 2e54 696d 6564 656c 7461 2830 290a  pd.Timedelta(0).
+00006cd0: 2020 2020 2020 2020 6d69 6e5f 7469 6d65          min_time
+00006ce0: 203d 2064 7276 5f64 6174 615b 2754 696d   = drv_data['Tim
+00006cf0: 6527 5d5b 695d 0a20 2020 2020 2020 2066  e'][i].        f
+00006d00: 6f72 2073 6563 746f 725f 7469 6d65 2c20  or sector_time, 
+00006d10: 7365 7373 696f 6e5f 7469 6d65 2069 6e20  session_time in 
+00006d20: 2828 7064 2e54 696d 6564 656c 7461 2830  ((pd.Timedelta(0
+00006d30: 292c 2064 7276 5f64 6174 615b 2753 6563  ), drv_data['Sec
+00006d40: 746f 7233 5365 7373 696f 6e54 696d 6527  tor3SessionTime'
+00006d50: 5d5b 695d 292c 0a20 2020 2020 2020 2020  ][i]),.         
+00006d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d80: 2028 6472 765f 6461 7461 5b27 5365 6374   (drv_data['Sect
+00006d90: 6f72 3354 696d 6527 5d5b 695d 2c20 6472  or3Time'][i], dr
+00006da0: 765f 6461 7461 5b27 5365 6374 6f72 3253  v_data['Sector2S
+00006db0: 6573 7369 6f6e 5469 6d65 275d 5b69 5d29  essionTime'][i])
+00006dc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006de0: 2020 2020 2020 2020 2020 2020 2864 7276              (drv
+00006df0: 5f64 6174 615b 2753 6563 746f 7232 5469  _data['Sector2Ti
+00006e00: 6d65 275d 5b69 5d2c 2064 7276 5f64 6174  me'][i], drv_dat
+00006e10: 615b 2753 6563 746f 7231 5365 7373 696f  a['Sector1Sessio
+00006e20: 6e54 696d 6527 5d5b 695d 2929 3a0a 2020  nTime'][i])):.  
+00006e30: 2020 2020 2020 2020 2020 6966 2070 642e            if pd.
+00006e40: 6973 6e75 6c6c 2873 6573 7369 6f6e 5f74  isnull(session_t
+00006e50: 696d 6529 3a0a 2020 2020 2020 2020 2020  ime):.          
+00006e60: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+00006e70: 2020 2020 2020 2020 2020 2069 6620 7064             if pd
+00006e80: 2e69 736e 756c 6c28 7365 6374 6f72 5f74  .isnull(sector_t
+00006e90: 696d 6529 3a0a 2020 2020 2020 2020 2020  ime):.          
+00006ea0: 2020 2020 2020 6272 6561 6b20 2023 206e        break  # n
+00006eb0: 6565 6420 746f 2073 746f 7020 6865 7265  eed to stop here
+00006ec0: 2062 6563 6175 7365 2065 6c73 6520 7468   because else th
+00006ed0: 6520 7365 6374 6f72 2073 756d 2077 696c  e sector sum wil
+00006ee0: 6c20 6265 2069 6e63 6f72 7265 6374 0a0a  l be incorrect..
+00006ef0: 2020 2020 2020 2020 2020 2020 7365 6374              sect
+00006f00: 6f72 5f73 756d 202b 3d20 7365 6374 6f72  or_sum += sector
+00006f10: 5f74 696d 650a 2020 2020 2020 2020 2020  _time.          
+00006f20: 2020 6e65 775f 7469 6d65 203d 2073 6573    new_time = ses
+00006f30: 7369 6f6e 5f74 696d 6520 2b20 7365 6374  sion_time + sect
+00006f40: 6f72 5f73 756d 0a20 2020 2020 2020 2020  or_sum.         
+00006f50: 2020 2069 6620 6e6f 7420 7064 2e69 736e     if not pd.isn
+00006f60: 756c 6c28 6e65 775f 7469 6d65 2920 616e  ull(new_time) an
+00006f70: 6420 286e 6577 5f74 696d 6520 3c20 6d69  d (new_time < mi
+00006f80: 6e5f 7469 6d65 206f 7220 7064 2e69 736e  n_time or pd.isn
+00006f90: 756c 6c28 6d69 6e5f 7469 6d65 2929 3a0a  ull(min_time)):.
+00006fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fb0: 6d69 6e5f 7469 6d65 203d 206e 6577 5f74  min_time = new_t
+00006fc0: 696d 650a 2020 2020 2020 2020 6966 2069  ime.        if i
+00006fd0: 203e 2030 2061 6e64 206d 696e 5f74 696d   > 0 and min_tim
+00006fe0: 6520 3c20 6472 765f 6461 7461 5b27 5469  e < drv_data['Ti
+00006ff0: 6d65 275d 5b69 202d 2031 5d3a 0a20 2020  me'][i - 1]:.   
+00007000: 2020 2020 2020 2020 2069 6e74 6567 7269           integri
+00007010: 7479 5f65 7272 6f72 732e 6170 7065 6e64  ty_errors.append
+00007020: 2869 202b 2031 2920 2023 206e 6f74 2062  (i + 1)  # not b
+00007030: 6520 706f 7373 6962 6c65 2069 6620 7365  e possible if se
+00007040: 6374 6f72 2074 696d 6573 2061 6e64 206c  ctor times and l
+00007050: 6170 2074 696d 6520 6172 6520 636f 7272  ap time are corr
+00007060: 6563 740a 2020 2020 2020 2020 2020 2020  ect.            
+00007070: 636f 6e74 696e 7565 0a0a 2020 2020 2020  continue..      
+00007080: 2020 6472 765f 6461 7461 5b27 5469 6d65    drv_data['Time
+00007090: 275d 5b69 5d20 3d20 6d69 6e5f 7469 6d65  '][i] = min_time
+000070a0: 0a0a 2020 2020 2320 6c61 7374 206c 6170  ..    # last lap
+000070b0: 206e 6565 6473 2074 6f20 6265 2072 656d   needs to be rem
+000070c0: 6f76 6564 2069 6620 6974 2064 6f65 7320  oved if it does 
+000070d0: 6e6f 7420 6861 7665 2061 2027 5469 6d65  not have a 'Time
+000070e0: 2720 616e 6420 6974 2063 6f75 6c64 206e  ' and it could n
+000070f0: 6f74 2062 6520 6361 6c63 756c 6174 6564  ot be calculated
+00007100: 2028 6c69 6b65 6c79 2061 6e20 696e 6c61   (likely an inla
+00007110: 7029 0a20 2020 2069 6620 7064 2e69 736e  p).    if pd.isn
+00007120: 756c 6c28 6472 765f 6461 7461 5b27 5469  ull(drv_data['Ti
+00007130: 6d65 275d 5b2d 315d 293a 0a20 2020 2020  me'][-1]):.     
+00007140: 2020 2069 6620 6e6f 7420 7064 2e69 736e     if not pd.isn
+00007150: 756c 6c28 6472 765f 6461 7461 5b27 5069  ull(drv_data['Pi
+00007160: 7449 6e54 696d 6527 5d5b 2d31 5d29 3a0a  tInTime'][-1]):.
+00007170: 2020 2020 2020 2020 2020 2020 6472 765f              drv_
+00007180: 6461 7461 5b27 5469 6d65 275d 5b2d 315d  data['Time'][-1]
+00007190: 203d 2064 7276 5f64 6174 615b 2750 6974   = drv_data['Pit
+000071a0: 496e 5469 6d65 275d 5b2d 315d 0a20 2020  InTime'][-1].   
+000071b0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000071c0: 2020 2020 2020 2066 6f72 206b 6579 2069         for key i
+000071d0: 6e20 6472 765f 6461 7461 2e6b 6579 7328  n drv_data.keys(
+000071e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000071f0: 2020 2064 7276 5f64 6174 615b 6b65 795d     drv_data[key]
+00007200: 203d 2064 7276 5f64 6174 615b 6b65 795d   = drv_data[key]
+00007210: 5b3a 2d31 5d0a 0a20 2020 2069 6620 6e6f  [:-1]..    if no
+00007220: 7420 6472 765f 6461 7461 5b27 5469 6d65  t drv_data['Time
+00007230: 275d 3a0a 2020 2020 2020 2020 2320 656e  ']:.        # en
+00007240: 7375 7265 2074 6861 7420 7468 6572 6520  sure that there 
+00007250: 6973 2073 7469 6c6c 2064 6174 6120 6c65  is still data le
+00007260: 6674 2061 6674 6572 2070 6f74 656e 7469  ft after potenti
+00007270: 616c 6c79 2072 656d 6f76 696e 6720 6120  ally removing a 
+00007280: 6c61 700a 2020 2020 2020 2020 7265 7475  lap.        retu
+00007290: 726e 2064 7276 5f64 6174 612c 2073 6573  rn drv_data, ses
+000072a0: 7369 6f6e 5f73 706c 6974 5f74 696d 6573  sion_split_times
+000072b0: 0a0a 2020 2020 2320 6d6f 7265 206c 6170  ..    # more lap
+000072c0: 2073 796e 632c 2074 6869 7320 7469 6d65   sync, this time
+000072d0: 2063 6865 636b 2077 6869 6368 206c 6170   check which lap
+000072e0: 2074 7269 6767 6572 6564 2077 6974 6820   triggered with 
+000072f0: 7468 6520 6c6f 7765 7374 206c 6174 656e  the lowest laten
+00007300: 6379 0a20 2020 2066 6f72 2069 2069 6e20  cy.    for i in 
+00007310: 7261 6e67 6528 6c65 6e28 6472 765f 6461  range(len(drv_da
+00007320: 7461 5b27 5469 6d65 275d 2920 2d20 312c  ta['Time']) - 1,
+00007330: 2030 2c20 2d31 293a 0a20 2020 2020 2020   0, -1):.       
+00007340: 2069 6620 286e 6577 5f74 696d 6520 3a3d   if (new_time :=
+00007350: 2064 7276 5f64 6174 615b 2754 696d 6527   drv_data['Time'
+00007360: 5d5b 695d 202d 2064 7276 5f64 6174 615b  ][i] - drv_data[
+00007370: 274c 6170 5469 6d65 275d 5b69 5d29 203c  'LapTime'][i]) <
+00007380: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
+00007390: 2020 2064 7276 5f64 6174 615b 2754 696d     drv_data['Tim
+000073a0: 6527 5d5b 6920 2d20 315d 3a0a 2020 2020  e'][i - 1]:.    
+000073b0: 2020 2020 2020 2020 6966 2069 203e 2031          if i > 1
+000073c0: 2061 6e64 206e 6577 5f74 696d 6520 3c20   and new_time < 
+000073d0: 6472 765f 6461 7461 5b27 5469 6d65 275d  drv_data['Time']
+000073e0: 5b69 202d 2032 5d3a 0a20 2020 2020 2020  [i - 2]:.       
+000073f0: 2020 2020 2020 2020 2069 6e74 6567 7269           integri
+00007400: 7479 5f65 7272 6f72 732e 6170 7065 6e64  ty_errors.append
+00007410: 2869 202b 2031 2920 2023 206e 6f74 2062  (i + 1)  # not b
+00007420: 6520 706f 7373 6962 6c65 2069 6620 7365  e possible if se
+00007430: 6374 6f72 2074 696d 6573 2061 6e64 206c  ctor times and l
+00007440: 6170 2074 696d 6520 6172 6520 636f 7272  ap time are corr
+00007450: 6563 740a 2020 2020 2020 2020 2020 2020  ect.            
+00007460: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00007470: 2020 2020 2020 6472 765f 6461 7461 5b27        drv_data['
+00007480: 5469 6d65 275d 5b69 202d 2031 5d20 3d20  Time'][i - 1] = 
+00007490: 6e65 775f 7469 6d65 0a0a 2020 2020 2320  new_time..    # 
+000074a0: 6e65 6564 2074 6f20 676f 2062 6f74 6820  need to go both 
+000074b0: 6469 7265 6374 696f 6e73 206f 6e63 6520  directions once 
+000074c0: 746f 206d 616b 6520 6576 6572 7974 6869  to make everythi
+000074d0: 6e67 206d 6174 6368 2075 703b 2061 6c73  ng match up; als
+000074e0: 6f20 7265 6361 6c63 756c 6174 6520 7365  o recalculate se
+000074f0: 6374 6f72 2074 696d 6573 0a20 2020 2066  ctor times.    f
+00007500: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
+00007510: 6e28 6472 765f 6461 7461 5b27 5469 6d65  n(drv_data['Time
+00007520: 275d 2920 2d20 3129 3a0a 2020 2020 2020  ']) - 1):.      
+00007530: 2020 6966 2061 6e79 2870 642e 6973 6e75    if any(pd.isnu
+00007540: 6c6c 2874 7374 2920 666f 7220 7473 7420  ll(tst) for tst 
+00007550: 696e 2028 0a20 2020 2020 2020 2020 2020  in (.           
+00007560: 2020 2020 2064 7276 5f64 6174 615b 2754       drv_data['T
+00007570: 696d 6527 5d5b 695d 2c20 6472 765f 6461  ime'][i], drv_da
+00007580: 7461 5b27 4c61 7054 696d 6527 5d5b 6920  ta['LapTime'][i 
+00007590: 2b20 315d 2c0a 2020 2020 2020 2020 2020  + 1],.          
+000075a0: 2020 2020 2020 6472 765f 6461 7461 5b27        drv_data['
+000075b0: 5365 6374 6f72 3154 696d 6527 5d5b 6920  Sector1Time'][i 
+000075c0: 2b20 315d 2c0a 2020 2020 2020 2020 2020  + 1],.          
+000075d0: 2020 2020 2020 6472 765f 6461 7461 5b27        drv_data['
+000075e0: 5365 6374 6f72 3254 696d 6527 5d5b 6920  Sector2Time'][i 
+000075f0: 2b20 315d 2c0a 2020 2020 2020 2020 2020  + 1],.          
+00007600: 2020 2020 2020 6472 765f 6461 7461 5b27        drv_data['
+00007610: 5365 6374 6f72 3354 696d 6527 5d5b 6920  Sector3Time'][i 
+00007620: 2b20 315d 2929 3a0a 2020 2020 2020 2020  + 1])):.        
+00007630: 2020 2020 636f 6e74 696e 7565 2020 2320      continue  # 
+00007640: 6c61 7020 6e6f 7420 7573 6162 6c65 2c20  lap not usable, 
+00007650: 6d69 7373 696e 6720 6372 6974 6963 616c  missing critical
+00007660: 2076 616c 7565 730a 0a20 2020 2020 2020   values..       
+00007670: 2069 6620 286e 6577 5f74 696d 6520 3a3d   if (new_time :=
+00007680: 2064 7276 5f64 6174 615b 2754 696d 6527   drv_data['Time'
+00007690: 5d5b 695d 202b 2064 7276 5f64 6174 615b  ][i] + drv_data[
+000076a0: 274c 6170 5469 6d65 275d 5b69 2b31 5d29  'LapTime'][i+1])
+000076b0: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
+000076c0: 2020 203c 2064 7276 5f64 6174 615b 2754     < drv_data['T
+000076d0: 696d 6527 5d5b 692b 315d 3a0a 2020 2020  ime'][i+1]:.    
+000076e0: 2020 2020 2020 2020 6472 765f 6461 7461          drv_data
+000076f0: 5b27 5469 6d65 275d 5b69 2b31 5d20 3d20  ['Time'][i+1] = 
+00007700: 6e65 775f 7469 6d65 0a20 2020 2020 2020  new_time.       
+00007710: 2069 6620 286e 6577 5f73 315f 7469 6d65   if (new_s1_time
+00007720: 203a 3d20 6472 765f 6461 7461 5b27 5469   := drv_data['Ti
+00007730: 6d65 275d 5b69 5d0a 2020 2020 2020 2020  me'][i].        
+00007740: 2020 2020 2020 2020 2b20 6472 765f 6461          + drv_da
+00007750: 7461 5b27 5365 6374 6f72 3154 696d 6527  ta['Sector1Time'
+00007760: 5d5b 692b 315d 2920 5c0a 2020 2020 2020  ][i+1]) \.      
+00007770: 2020 2020 2020 2020 2020 3c20 6472 765f            < drv_
+00007780: 6461 7461 5b27 5365 6374 6f72 3153 6573  data['Sector1Ses
+00007790: 7369 6f6e 5469 6d65 275d 5b69 2b31 5d3a  sionTime'][i+1]:
+000077a0: 0a20 2020 2020 2020 2020 2020 2064 7276  .            drv
+000077b0: 5f64 6174 615b 2753 6563 746f 7231 5365  _data['Sector1Se
+000077c0: 7373 696f 6e54 696d 6527 5d5b 692b 315d  ssionTime'][i+1]
+000077d0: 203d 206e 6577 5f73 315f 7469 6d65 0a20   = new_s1_time. 
+000077e0: 2020 2020 2020 2069 6620 286e 6577 5f73         if (new_s
+000077f0: 325f 7469 6d65 203a 3d20 6472 765f 6461  2_time := drv_da
+00007800: 7461 5b27 5469 6d65 275d 5b69 5d20 2b20  ta['Time'][i] + 
+00007810: 6472 765f 6461 7461 5b27 5365 6374 6f72  drv_data['Sector
+00007820: 3154 696d 6527 5d5b 692b 315d 0a20 2020  1Time'][i+1].   
+00007830: 2020 2020 2020 2020 2020 2020 202b 2064               + d
+00007840: 7276 5f64 6174 615b 2753 6563 746f 7232  rv_data['Sector2
+00007850: 5469 6d65 275d 5b69 2b31 5d29 205c 0a20  Time'][i+1]) \. 
+00007860: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00007870: 2064 7276 5f64 6174 615b 2753 6563 746f   drv_data['Secto
+00007880: 7232 5365 7373 696f 6e54 696d 6527 5d5b  r2SessionTime'][
+00007890: 692b 315d 3a0a 2020 2020 2020 2020 2020  i+1]:.          
+000078a0: 2020 6472 765f 6461 7461 5b27 5365 6374    drv_data['Sect
+000078b0: 6f72 3253 6573 7369 6f6e 5469 6d65 275d  or2SessionTime']
+000078c0: 5b69 2b31 5d20 3d20 6e65 775f 7332 5f74  [i+1] = new_s2_t
+000078d0: 696d 650a 2020 2020 2020 2020 6966 2028  ime.        if (
+000078e0: 6e65 775f 7333 5f74 696d 6520 3a3d 2064  new_s3_time := d
+000078f0: 7276 5f64 6174 615b 2754 696d 6527 5d5b  rv_data['Time'][
+00007900: 695d 202b 2064 7276 5f64 6174 615b 2753  i] + drv_data['S
+00007910: 6563 746f 7231 5469 6d65 275d 5b69 2b31  ector1Time'][i+1
+00007920: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00007930: 2020 2b20 6472 765f 6461 7461 5b27 5365    + drv_data['Se
+00007940: 6374 6f72 3254 696d 6527 5d5b 692b 315d  ctor2Time'][i+1]
+00007950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007960: 202b 2064 7276 5f64 6174 615b 2753 6563   + drv_data['Sec
+00007970: 746f 7233 5469 6d65 275d 5b69 2b31 5d29  tor3Time'][i+1])
+00007980: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
+00007990: 2020 203c 2064 7276 5f64 6174 615b 2753     < drv_data['S
+000079a0: 6563 746f 7233 5365 7373 696f 6e54 696d  ector3SessionTim
+000079b0: 6527 5d5b 692b 315d 3a0a 2020 2020 2020  e'][i+1]:.      
+000079c0: 2020 2020 2020 6472 765f 6461 7461 5b27        drv_data['
+000079d0: 5365 6374 6f72 3353 6573 7369 6f6e 5469  Sector3SessionTi
+000079e0: 6d65 275d 5b69 2b31 5d20 3d20 6e65 775f  me'][i+1] = new_
+000079f0: 7333 5f74 696d 650a 0a20 2020 2023 2049  s3_time..    # I
+00007a00: 7465 7261 7465 206f 7665 7220 6c69 7374  terate over list
+00007a10: 206f 6620 7065 7273 6f6e 616c 206c 6170   of personal lap
+00007a20: 2074 696d 6573 2073 6574 2027 4973 5065   times set 'IsPe
+00007a30: 7273 6f6e 616c 4265 7374 272e 0a20 2020  rsonalBest'..   
+00007a40: 2023 2057 6865 6e20 6120 6c61 7020 6973   # When a lap is
+00007a50: 2064 656c 6574 6564 2c20 7468 6520 4150   deleted, the AP
+00007a60: 4920 7265 7365 6e64 7320 7468 6520 7072  I resends the pr
+00007a70: 6576 696f 7573 2070 6572 736f 6e61 6c20  evious personal 
+00007a80: 6265 7374 2e0a 2020 2020 2320 5468 6572  best..    # Ther
+00007a90: 6566 6f72 652c 2062 7920 6974 6572 6174  efore, by iterat
+00007aa0: 696e 6720 696e 2072 6576 6572 7365 2c20  ing in reverse, 
+00007ab0: 6966 2061 6e79 206c 6170 2069 7320 656e  if any lap is en
+00007ac0: 636f 756e 7465 7265 6420 7468 6174 2069  countered that i
+00007ad0: 730a 2020 2020 2320 7175 6963 6b65 7220  s.    # quicker 
+00007ae0: 7468 616e 2061 6c72 6561 6479 2070 726f  than already pro
+00007af0: 6365 7373 6564 2070 6572 736f 6e61 6c20  cessed personal 
+00007b00: 6265 7374 206c 6170 2074 696d 6573 2c20  best lap times, 
+00007b10: 6974 206d 7573 7420 6861 7665 0a20 2020  it must have.   
+00007b20: 2023 2062 6565 6e20 6465 6c65 7465 642e   # been deleted.
+00007b30: 0a20 2020 2023 2054 6869 7320 6973 206a  .    # This is j
+00007b40: 7573 7420 6265 7374 2065 6666 6f72 7420  ust best effort 
+00007b50: 6275 7420 6e6f 7420 6578 6861 7573 7469  but not exhausti
+00007b60: 7665 2061 7320 6974 2063 616e 206f 6e6c  ve as it can onl
+00007b70: 7920 6861 6e64 6c65 206c 6170 0a20 2020  y handle lap.   
+00007b80: 2023 2074 696d 6573 2074 6861 7420 7765   # times that we
+00007b90: 7265 2064 656c 6574 6564 2071 7569 636b  re deleted quick
+00007ba0: 6c79 2028 6265 666f 7265 2074 6865 206e  ly (before the n
+00007bb0: 6578 7420 7065 7273 6f6e 616c 2062 6573  ext personal bes
+00007bc0: 7420 7761 7320 7365 7429 2e0a 2020 2020  t was set)..    
+00007bd0: 5f63 6f72 7265 6374 6564 5f70 6572 736f  _corrected_perso
+00007be0: 6e61 6c5f 6265 7374 5f6c 6170 5f74 696d  nal_best_lap_tim
+00007bf0: 6573 203d 206c 6973 7428 290a 2020 2020  es = list().    
+00007c00: 2320 6c69 7374 2069 7320 6f6e 6c79 2075  # list is only u
+00007c10: 7365 6420 666f 7220 6261 636b 7265 6665  sed for backrefe
+00007c20: 7265 6e63 6520 7769 7468 696e 2074 6865  rence within the
+00007c30: 206c 6f6f 700a 2020 2020 6375 725f 736e   loop.    cur_sn
+00007c40: 203d 206c 656e 2873 6573 7369 6f6e 5f73   = len(session_s
+00007c50: 706c 6974 5f74 696d 6573 2920 2d20 310a  plit_times) - 1.
+00007c60: 2020 2020 2320 6375 7272 656e 7420 2873      # current (s
+00007c70: 7562 2973 6573 7369 6f6e 206e 756d 6265  ub)session numbe
+00007c80: 722c 2070 6572 736f 6e61 6c20 6265 7374  r, personal best
+00007c90: 206c 6170 2074 696d 6573 206e 6565 6420   lap times need 
+00007ca0: 746f 2062 650a 2020 2020 2320 636f 6e73  to be.    # cons
+00007cb0: 6964 6572 6564 2066 6f72 2065 6163 6820  idered for each 
+00007cc0: 2873 7562 2973 6573 7369 6f6e 2069 6e64  (sub)session ind
+00007cd0: 6976 6964 7561 6c6c 790a 2020 2020 666f  ividually.    fo
+00007ce0: 7220 7469 6d65 2c20 7062 5f6c 6170 5f74  r time, pb_lap_t
+00007cf0: 696d 6520 696e 2072 6576 6572 7365 6428  ime in reversed(
+00007d00: 7065 7273 6f6e 616c 5f62 6573 745f 6c61  personal_best_la
+00007d10: 705f 7469 6d65 7329 3a0a 2020 2020 2020  p_times):.      
+00007d20: 2020 6966 2074 696d 6520 3c20 7365 7373    if time < sess
+00007d30: 696f 6e5f 7370 6c69 745f 7469 6d65 735b  ion_split_times[
+00007d40: 6375 725f 736e 5d3a 0a20 2020 2020 2020  cur_sn]:.       
+00007d50: 2020 2020 2023 2074 7261 6e73 6974 696f       # transitio
+00007d60: 6e65 6420 696e 746f 2074 6865 2070 7265  ned into the pre
+00007d70: 7669 6f75 7320 2873 7562 2973 6573 7369  vious (sub)sessi
+00007d80: 6f6e 2028 7265 7665 7273 6520 6974 6572  on (reverse iter
+00007d90: 6174 696f 6e21 290a 2020 2020 2020 2020  ation!).        
+00007da0: 2020 2020 2320 7265 7365 7420 7468 6520      # reset the 
+00007db0: 7265 6665 7265 6e63 6520 6c69 7374 2c20  reference list, 
+00007dc0: 736f 2074 696d 6520 6172 6520 636f 6e73  so time are cons
+00007dd0: 6964 6572 6564 2069 6e64 6976 6964 7561  idered individua
+00007de0: 6c6c 790a 2020 2020 2020 2020 2020 2020  lly.            
+00007df0: 6375 725f 736e 202d 3d20 310a 2020 2020  cur_sn -= 1.    
+00007e00: 2020 2020 2020 2020 5f63 6f72 7265 6374          _correct
+00007e10: 6564 5f70 6572 736f 6e61 6c5f 6265 7374  ed_personal_best
+00007e20: 5f6c 6170 5f74 696d 6573 203d 206c 6973  _lap_times = lis
+00007e30: 7428 290a 0a20 2020 2020 2020 2069 6620  t()..        if 
+00007e40: 5f63 6f72 7265 6374 6564 5f70 6572 736f  _corrected_perso
+00007e50: 6e61 6c5f 6265 7374 5f6c 6170 5f74 696d  nal_best_lap_tim
+00007e60: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00007e70: 6966 2070 625f 6c61 705f 7469 6d65 2069  if pb_lap_time i
+00007e80: 6e20 5f63 6f72 7265 6374 6564 5f70 6572  n _corrected_per
+00007e90: 736f 6e61 6c5f 6265 7374 5f6c 6170 5f74  sonal_best_lap_t
+00007ea0: 696d 6573 3a0a 2020 2020 2020 2020 2020  imes:.          
+00007eb0: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+00007ec0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00007ed0: 7062 5f6c 6170 5f74 696d 6520 3c20 6d69  pb_lap_time < mi
+00007ee0: 6e28 5f63 6f72 7265 6374 6564 5f70 6572  n(_corrected_per
+00007ef0: 736f 6e61 6c5f 6265 7374 5f6c 6170 5f74  sonal_best_lap_t
+00007f00: 696d 6573 293a 0a20 2020 2020 2020 2020  imes):.         
+00007f10: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+00007f20: 0a20 2020 2020 2020 205f 636f 7272 6563  .        _correc
+00007f30: 7465 645f 7065 7273 6f6e 616c 5f62 6573  ted_personal_bes
+00007f40: 745f 6c61 705f 7469 6d65 732e 6170 7065  t_lap_times.appe
+00007f50: 6e64 2870 625f 6c61 705f 7469 6d65 290a  nd(pb_lap_time).
+00007f60: 0a20 2020 2020 2020 2023 2066 696e 6420  .        # find 
+00007f70: 7468 6520 696e 6465 7820 6f66 2074 6865  the index of the
+00007f80: 2063 6f72 7265 7370 6f6e 6469 6e67 206c   corresponding l
+00007f90: 6170 2062 7920 636f 6d70 6172 696e 6720  ap by comparing 
+00007fa0: 7769 7468 2074 6865 206c 6170 0a20 2020  with the lap.   
+00007fb0: 2020 2020 2023 2074 696d 6573 2061 6e64       # times and
+00007fc0: 2073 6574 2027 4973 5065 7273 6f6e 616c   set 'IsPersonal
+00007fd0: 4265 7374 2720 746f 2054 7275 6520 666f  Best' to True fo
+00007fe0: 7220 7468 6174 206c 6170 0a20 2020 2020  r that lap.     
+00007ff0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00008000: 2020 2020 7062 5f69 6478 203d 2064 7276      pb_idx = drv
+00008010: 5f64 6174 615b 274c 6170 5469 6d65 275d  _data['LapTime']
+00008020: 2e69 6e64 6578 2870 625f 6c61 705f 7469  .index(pb_lap_ti
+00008030: 6d65 290a 2020 2020 2020 2020 6578 6365  me).        exce
+00008040: 7074 2056 616c 7565 4572 726f 723a 0a20  pt ValueError:. 
+00008050: 2020 2020 2020 2020 2020 2023 206f 6e65             # one
+00008060: 2065 7861 6d70 6c65 2063 6173 6520 7768   example case wh
+00008070: 6572 6520 7468 6973 2065 7272 6f72 206f  ere this error o
+00008080: 6363 7572 732c 2061 7265 2077 696c 646c  ccurs, are wildl
+00008090: 7920 6f66 2070 6572 736f 6e61 6c0a 2020  y of personal.  
+000080a0: 2020 2020 2020 2020 2020 2320 6265 7374            # best
+000080b0: 2074 696d 6573 2028 3e32 206d 696e 206c   times (>2 min l
+000080c0: 6170 2074 696d 6529 2074 6861 7420 6172  ap time) that ar
+000080d0: 6520 736f 6d65 7469 6d65 7320 7072 6573  e sometimes pres
+000080e0: 656e 7420 616e 640a 2020 2020 2020 2020  ent and.        
+000080f0: 2020 2020 2320 7768 6963 6820 6861 7665      # which have
+00008100: 206e 6f20 636f 7272 6573 706f 6e64 696e   no correspondin
+00008110: 6720 6c61 7020 7469 6d65 0a20 2020 2020  g lap time.     
+00008120: 2020 2020 2020 2070 6173 730a 2020 2020         pass.    
+00008130: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00008140: 2020 2020 2020 6472 765f 6461 7461 5b27        drv_data['
+00008150: 4973 5065 7273 6f6e 616c 4265 7374 275d  IsPersonalBest']
+00008160: 5b70 625f 6964 785d 203d 2054 7275 650a  [pb_idx] = True.
+00008170: 0a20 2020 2069 6620 696e 7465 6772 6974  .    if integrit
+00008180: 795f 6572 726f 7273 3a0a 2020 2020 2020  y_errors:.      
+00008190: 2020 5f6c 6f67 6765 722e 7761 726e 696e    _logger.warnin
+000081a0: 6728 0a20 2020 2020 2020 2020 2020 2066  g(.            f
+000081b0: 2244 7269 7665 7220 7b64 7276 3a20 3e32  "Driver {drv: >2
+000081c0: 7d3a 2045 6e63 6f75 6e74 6572 6564 207b  }: Encountered {
+000081d0: 6c65 6e28 696e 7465 6772 6974 795f 6572  len(integrity_er
+000081e0: 726f 7273 297d 2074 696d 696e 6720 220a  rors)} timing ".
+000081f0: 2020 2020 2020 2020 2020 2020 6622 696e              f"in
+00008200: 7465 6772 6974 7920 6572 726f 7228 7329  tegrity error(s)
+00008210: 206e 6561 7220 6c61 7028 7329 3a20 7b69   near lap(s): {i
+00008220: 6e74 6567 7269 7479 5f65 7272 6f72 737d  ntegrity_errors}
+00008230: 2e5c 6e22 0a20 2020 2020 2020 2020 2020  .\n".           
+00008240: 2066 2254 6869 7320 6d69 6768 7420 6265   f"This might be
+00008250: 2061 2062 7567 2061 6e64 2073 686f 756c   a bug and shoul
+00008260: 6420 6265 2072 6570 6f72 7465 642e 2229  d be reported.")
+00008270: 0a0a 2020 2020 7265 7475 726e 2064 7276  ..    return drv
+00008280: 5f64 6174 612c 2073 6573 7369 6f6e 5f73  _data, session_s
+00008290: 706c 6974 5f74 696d 6573 0a0a 0a64 6566  plit_times...def
+000082a0: 205f 7374 7265 616d 5f64 6174 615f 6472   _stream_data_dr
+000082b0: 6976 6572 2864 7269 7665 725f 7261 772c  iver(driver_raw,
+000082c0: 2065 6d70 7479 5f76 616c 732c 2064 7276   empty_vals, drv
+000082d0: 293a 0a20 2020 2022 2222 0a20 2020 202e  ):.    """.    .
+000082e0: 2e20 7761 726e 696e 673a 3a0a 2020 2020  . warning::.    
+000082f0: 2020 2020 3a6d 6f64 3a60 6661 7374 6631      :mod:`fastf1
+00008300: 2e61 7069 6020 7769 6c6c 2062 6520 636f  .api` will be co
+00008310: 6e73 6964 6572 6564 2070 7269 7661 7465  nsidered private
+00008320: 2069 6e20 6675 7475 7265 2072 656c 6561   in future relea
+00008330: 7365 7320 616e 640a 2020 2020 2020 2020  ses and.        
+00008340: 706f 7465 6e74 6961 6c6c 7920 6265 2072  potentially be r
+00008350: 656d 6f76 6564 206f 7220 6368 616e 6765  emoved or change
+00008360: 642e 0a0a 2020 2020 4461 7461 2069 7320  d...    Data is 
+00008370: 6f6e 2061 2074 696d 6573 7461 6d70 2062  on a timestamp b
+00008380: 6173 6973 2e0a 0a20 2020 2050 6172 616d  asis...    Param
+00008390: 733a 0a20 2020 2020 2020 2064 7269 7665  s:.        drive
+000083a0: 725f 7261 7720 286c 6973 7429 3a20 7261  r_raw (list): ra
+000083b0: 7720 6170 6920 7265 7370 6f6e 7365 2066  w api response f
+000083c0: 6f72 2074 6869 7320 6472 6976 6572 206f  or this driver o
+000083d0: 6e6c 7920 5b28 5469 6d65 7374 616d 702c  nly [(Timestamp,
+000083e0: 2064 6174 6129 2c20 282e 2e2e 292c 202e   data), (...), .
+000083f0: 2e2e 5d0a 2020 2020 2020 2020 656d 7074  ..].        empt
+00008400: 795f 7661 6c73 2028 6469 6374 293a 2064  y_vals (dict): d
+00008410: 6963 7469 6f6e 6172 7920 6f66 2063 6f6c  ictionary of col
+00008420: 756d 6e20 6e61 6d65 7320 616e 6420 656d  umn names and em
+00008430: 7074 7920 636f 6c75 6d6e 2076 616c 7565  pty column value
+00008440: 730a 2020 2020 2020 2020 6472 7620 2873  s.        drv (s
+00008450: 7472 293a 2064 7269 7665 7220 6964 656e  tr): driver iden
+00008460: 7469 6669 6572 0a0a 2020 2020 5265 7475  tifier..    Retu
+00008470: 726e 733a 0a20 2020 2020 2020 2020 6469  rns:.         di
+00008480: 6374 696f 6e61 7279 206f 6620 7469 6d69  ctionary of timi
+00008490: 6e67 2073 7472 6561 6d20 6461 7461 2066  ng stream data f
+000084a0: 6f72 2074 6869 7320 6472 6976 6572 0a20  or this driver. 
+000084b0: 2020 2022 2222 0a20 2020 2023 2065 6e74     """.    # ent
+000084c0: 7269 6573 2061 7265 2070 7265 6669 6c6c  ries are prefill
+000084d0: 6564 2077 6974 6820 656d 7074 7920 6f72  ed with empty or
+000084e0: 2070 7265 7669 6f75 7320 7661 6c75 6573   previous values
+000084f0: 2061 6e64 206f 6e6c 7920 6f76 6572 7772   and only overwr
+00008500: 6974 7465 6e20 6966 2074 6865 7920 6578  itten if they ex
+00008510: 6973 7420 696e 2074 6865 2072 6573 706f  ist in the respo
+00008520: 6e73 6520 6c69 6e65 0a20 2020 2023 2062  nse line.    # b
+00008530: 6173 6963 616c 6c79 2069 6e74 6572 706f  asically interpo
+00008540: 6c61 7469 6f6e 2062 7920 6669 6c6c 696e  lation by fillin
+00008550: 6720 7570 2077 6974 6820 6c61 7374 206b  g up with last k
+00008560: 6e6f 776e 2076 616c 7565 2062 6563 6175  nown value becau
+00008570: 7365 206e 6f74 2065 7665 7279 2076 616c  se not every val
+00008580: 7565 2069 7320 696e 2065 7665 7279 2072  ue is in every r
+00008590: 6573 706f 6e73 650a 2020 2020 6472 765f  esponse.    drv_
+000085a0: 6461 7461 203d 207b 6b65 793a 205b 7661  data = {key: [va
+000085b0: 6c2c 205d 2066 6f72 206b 6579 2c20 7661  l, ] for key, va
+000085c0: 6c20 696e 2065 6d70 7479 5f76 616c 732e  l in empty_vals.
+000085d0: 6974 656d 7328 297d 0a20 2020 2069 203d  items()}.    i =
+000085e0: 2030 0a0a 2020 2020 2320 6974 6572 6174   0..    # iterat
+000085f0: 6520 7468 726f 7567 6820 7468 6520 6461  e through the da
+00008600: 7461 3b20 7469 6d65 7374 616d 7020 2b20  ta; timestamp + 
+00008610: 616e 7920 6f66 2074 6865 2076 616c 7565  any of the value
+00008620: 7320 7472 6967 6765 7273 206e 6577 2072  s triggers new r
+00008630: 6f77 2069 6e20 6461 7461 0a20 2020 2066  ow in data.    f
+00008640: 6f72 2074 696d 652c 2072 6573 7020 696e  or time, resp in
+00008650: 2064 7269 7665 725f 7261 773a 0a20 2020   driver_raw:.   
+00008660: 2020 2020 206e 6577 5f65 6e74 7279 203d       new_entry =
+00008670: 2046 616c 7365 0a20 2020 2020 2020 2069   False.        i
+00008680: 6620 7661 6c20 3a3d 2072 6563 7572 7369  f val := recursi
+00008690: 7665 5f64 6963 745f 6765 7428 7265 7370  ve_dict_get(resp
+000086a0: 2c20 2750 6f73 6974 696f 6e27 293a 0a20  , 'Position'):. 
+000086b0: 2020 2020 2020 2020 2020 2064 7276 5f64             drv_d
+000086c0: 6174 615b 2750 6f73 6974 696f 6e27 5d5b  ata['Position'][
+000086d0: 695d 203d 2069 6e74 2876 616c 290a 2020  i] = int(val).  
+000086e0: 2020 2020 2020 2020 2020 6e65 775f 656e            new_en
+000086f0: 7472 7920 3d20 5472 7565 0a20 2020 2020  try = True.     
+00008700: 2020 2069 6620 7661 6c20 3a3d 2072 6563     if val := rec
+00008710: 7572 7369 7665 5f64 6963 745f 6765 7428  ursive_dict_get(
+00008720: 7265 7370 2c20 2747 6170 546f 4c65 6164  resp, 'GapToLead
+00008730: 6572 2729 3a0a 2020 2020 2020 2020 2020  er'):.          
+00008740: 2020 6472 765f 6461 7461 5b27 4761 7054    drv_data['GapT
+00008750: 6f4c 6561 6465 7227 5d5b 695d 203d 2076  oLeader'][i] = v
+00008760: 616c 0a20 2020 2020 2020 2020 2020 206e  al.            n
+00008770: 6577 5f65 6e74 7279 203d 2054 7275 650a  ew_entry = True.
+00008780: 2020 2020 2020 2020 6966 2076 616c 203a          if val :
+00008790: 3d20 7265 6375 7273 6976 655f 6469 6374  = recursive_dict
+000087a0: 5f67 6574 2872 6573 702c 2027 496e 7465  _get(resp, 'Inte
+000087b0: 7276 616c 546f 506f 7369 7469 6f6e 4168  rvalToPositionAh
+000087c0: 6561 6427 2c20 2756 616c 7565 2729 3a0a  ead', 'Value'):.
+000087d0: 2020 2020 2020 2020 2020 2020 6472 765f              drv_
+000087e0: 6461 7461 5b27 496e 7465 7276 616c 546f  data['IntervalTo
+000087f0: 506f 7369 7469 6f6e 4168 6561 6427 5d5b  PositionAhead'][
+00008800: 695d 203d 2076 616c 0a20 2020 2020 2020  i] = val.       
+00008810: 2020 2020 206e 6577 5f65 6e74 7279 203d       new_entry =
+00008820: 2054 7275 650a 0a20 2020 2020 2020 2023   True..        #
+00008830: 2061 7420 6c65 6173 7420 6f6e 6520 7661   at least one va
+00008840: 6c75 6520 7761 7320 7072 6573 656e 742c  lue was present,
+00008850: 2063 7265 6174 6520 6e65 7874 2072 6f77   create next row
+00008860: 0a20 2020 2020 2020 2069 6620 6e65 775f  .        if new_
+00008870: 656e 7472 793a 0a20 2020 2020 2020 2020  entry:.         
+00008880: 2020 2064 7276 5f64 6174 615b 2754 696d     drv_data['Tim
+00008890: 6527 5d5b 695d 203d 2074 6f5f 7469 6d65  e'][i] = to_time
+000088a0: 6465 6c74 6128 7469 6d65 290a 2020 2020  delta(time).    
+000088b0: 2020 2020 2020 2020 6472 765f 6461 7461          drv_data
+000088c0: 5b27 4472 6976 6572 275d 5b69 5d20 3d20  ['Driver'][i] = 
+000088d0: 6472 760a 2020 2020 2020 2020 2020 2020  drv.            
+000088e0: 6920 2b3d 2031 0a0a 2020 2020 2020 2020  i += 1..        
+000088f0: 2020 2020 2320 6372 6561 7465 206e 6578      # create nex
+00008900: 7420 726f 7720 6f66 2064 6174 6120 6672  t row of data fr
+00008910: 6f6d 2074 6865 206c 6173 7420 7661 6c75  om the last valu
+00008920: 6573 3b20 7468 6572 6520 7769 6c6c 2061  es; there will a
+00008930: 6c77 6179 7320 6265 206f 6e65 2072 6f77  lways be one row
+00008940: 2074 6f6f 206d 7563 6820 6174 2074 6865   too much at the
+00008950: 2065 6e64 2077 6869 6368 2069 730a 2020   end which is.  
+00008960: 2020 2020 2020 2020 2020 2320 7265 6d6f            # remo
+00008970: 7665 6420 6167 6169 6e0a 2020 2020 2020  ved again.      
+00008980: 2020 2020 2020 666f 7220 6b65 792c 2076        for key, v
+00008990: 616c 2069 6e20 656d 7074 795f 7661 6c73  al in empty_vals
+000089a0: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+000089b0: 2020 2020 2020 2020 2020 6472 765f 6461            drv_da
+000089c0: 7461 5b6b 6579 5d2e 6170 7065 6e64 2864  ta[key].append(d
+000089d0: 7276 5f64 6174 615b 6b65 795d 5b2d 315d  rv_data[key][-1]
+000089e0: 290a 0a20 2020 2066 6f72 206b 6579 2069  )..    for key i
+000089f0: 6e20 6472 765f 6461 7461 2e6b 6579 7328  n drv_data.keys(
+00008a00: 293a 0a20 2020 2020 2020 2064 7276 5f64  ):.        drv_d
+00008a10: 6174 615b 6b65 795d 203d 2064 7276 5f64  ata[key] = drv_d
+00008a20: 6174 615b 6b65 795d 5b3a 2d31 5d20 2023  ata[key][:-1]  #
+00008a30: 2072 656d 6f76 6520 7665 7279 206c 6173   remove very las
+00008a40: 7420 726f 7720 6167 6169 6e0a 0a20 2020  t row again..   
+00008a50: 2072 6574 7572 6e20 6472 765f 6461 7461   return drv_data
+00008a60: 0a0a 0a40 4361 6368 652e 6170 695f 7265  ...@Cache.api_re
+00008a70: 7175 6573 745f 7772 6170 7065 720a 6465  quest_wrapper.de
+00008a80: 6620 7469 6d69 6e67 5f61 7070 5f64 6174  f timing_app_dat
+00008a90: 6128 7061 7468 2c20 7265 7370 6f6e 7365  a(path, response
+00008aa0: 3d4e 6f6e 652c 206c 6976 6564 6174 613d  =None, livedata=
+00008ab0: 4e6f 6e65 293a 0a20 2020 2022 2222 0a20  None):.    """. 
+00008ac0: 2020 202e 2e20 7761 726e 696e 673a 3a0a     .. warning::.
+00008ad0: 2020 2020 2020 2020 3a6d 6f64 3a60 6661          :mod:`fa
+00008ae0: 7374 6631 2e61 7069 6020 7769 6c6c 2062  stf1.api` will b
+00008af0: 6520 636f 6e73 6964 6572 6564 2070 7269  e considered pri
+00008b00: 7661 7465 2069 6e20 6675 7475 7265 2072  vate in future r
+00008b10: 656c 6561 7365 7320 616e 640a 2020 2020  eleases and.    
+00008b20: 2020 2020 706f 7465 6e74 6961 6c6c 7920      potentially 
+00008b30: 6265 2072 656d 6f76 6564 206f 7220 6368  be removed or ch
+00008b40: 616e 6765 642e 0a0a 2020 2020 4665 7463  anged...    Fetc
+00008b50: 6820 616e 6420 7061 7273 6520 2774 696d  h and parse 'tim
+00008b60: 696e 6720 6170 7020 6461 7461 272e 0a0a  ing app data'...
+00008b70: 2020 2020 5469 6d69 6e67 2061 7070 2064      Timing app d
+00008b80: 6174 6120 7072 6f76 6964 6573 2074 6865  ata provides the
+00008b90: 2066 6f6c 6c6f 7769 6e67 2064 6174 6120   following data 
+00008ba0: 6368 616e 6e65 6c73 2070 6572 2073 616d  channels per sam
+00008bb0: 706c 653a 0a20 2020 2020 2020 2d20 4c61  ple:.       - La
+00008bc0: 704e 756d 6265 7220 2866 6c6f 6174 206f  pNumber (float o
+00008bd0: 7220 6e61 6e29 3a20 4375 7272 656e 7420  r nan): Current 
+00008be0: 6c61 7020 6e75 6d62 6572 0a20 2020 2020  lap number.     
+00008bf0: 2020 2d20 4472 6976 6572 2028 7374 7229    - Driver (str)
+00008c00: 3a20 4472 6976 6572 206e 756d 6265 720a  : Driver number.
+00008c10: 2020 2020 2020 202d 204c 6170 5469 6d65         - LapTime
+00008c20: 2028 7061 6e64 6173 2e54 696d 6564 656c   (pandas.Timedel
+00008c30: 7461 206f 7220 4e6f 6e65 293a 204c 6170  ta or None): Lap
+00008c40: 2074 696d 6520 6f66 206c 6173 7420 6c61   time of last la
+00008c50: 700a 2020 2020 2020 202d 2053 7469 6e74  p.       - Stint
+00008c60: 2028 696e 7429 3a20 436f 756e 7465 7220   (int): Counter 
+00008c70: 666f 7220 7468 6520 6e75 6d62 6572 206f  for the number o
+00008c80: 6620 6472 6976 656e 2073 7469 6e74 730a  f driven stints.
+00008c90: 2020 2020 2020 202d 2054 6f74 616c 4c61         - TotalLa
+00008ca0: 7073 2028 666c 6f61 7420 6f72 206e 616e  ps (float or nan
+00008cb0: 293a 2054 6f74 616c 206e 756d 6265 7220  ): Total number 
+00008cc0: 6f66 206c 6170 7320 6472 6976 656e 206f  of laps driven o
+00008cd0: 6e20 7468 6973 2073 6574 206f 6620 7469  n this set of ti
+00008ce0: 7265 7320 2869 6e63 6c75 6465 7320 6c61  res (includes la
+00008cf0: 7073 2064 7269 7665 6e20 696e 0a20 2020  ps driven in.   
+00008d00: 2020 2020 2020 6f74 6865 7220 7365 7373        other sess
+00008d10: 696f 6e73 2129 0a20 2020 2020 2020 2d20  ions!).       - 
+00008d20: 436f 6d70 6f75 6e64 2028 7374 7220 6f72  Compound (str or
+00008d30: 204e 6f6e 6529 3a20 5469 7265 2063 6f6d   None): Tire com
+00008d40: 706f 756e 640a 2020 2020 2020 202d 204e  pound.       - N
+00008d50: 6577 2028 626f 6f6c 206f 7220 4e6f 6e65  ew (bool or None
+00008d60: 293a 2057 6865 7468 6572 2074 6865 2074  ): Whether the t
+00008d70: 6972 6520 7761 7320 6e65 7720 7768 656e  ire was new when
+00008d80: 2066 6974 7465 640a 2020 2020 2020 202d   fitted.       -
+00008d90: 2054 7972 6573 4e6f 7443 6861 6e67 6564   TyresNotChanged
+00008da0: 2028 696e 7420 6f72 204e 6f6e 6529 3a20   (int or None): 
+00008db0: 3f3f 3f20 5072 6f62 6162 6c79 2061 2066  ??? Probably a f
+00008dc0: 6c61 6720 746f 206d 6172 6b20 7069 7420  lag to mark pit 
+00008dd0: 7374 6f70 7320 7769 7468 6f75 7420 7469  stops without ti
+00008de0: 7265 2063 6861 6e67 6573 0a20 2020 2020  re changes.     
+00008df0: 2020 2d20 5469 6d65 2028 7061 6e64 6173    - Time (pandas
+00008e00: 2e54 696d 6564 656c 7461 293a 2053 6573  .Timedelta): Ses
+00008e10: 7369 6f6e 2074 696d 650a 2020 2020 2020  sion time.      
+00008e20: 202d 204c 6170 466c 6167 7320 2866 6c6f   - LapFlags (flo
+00008e30: 6174 206f 7220 6e61 6e29 3a20 3f3f 3f20  at or nan): ??? 
+00008e40: 756e 6b6e 6f77 6e0a 2020 2020 2020 202d  unknown.       -
+00008e50: 204c 6170 436f 756e 7454 696d 6520 284e   LapCountTime (N
+00008e60: 6f6e 6520 6f72 203f 3f3f 293a 203f 3f3f  one or ???): ???
+00008e70: 2075 6e6b 6e6f 776e 3b20 6e6f 2064 6174   unknown; no dat
+00008e80: 610a 2020 2020 2020 202d 2053 7461 7274  a.       - Start
+00008e90: 4c61 7073 2028 666c 6f61 7420 6f72 206e  Laps (float or n
+00008ea0: 616e 293a 203f 3f3f 2054 6972 6520 6167  an): ??? Tire ag
+00008eb0: 6520 7768 656e 2066 6974 7465 6420 2873  e when fitted (s
+00008ec0: 616d 6520 6173 2027 546f 7461 6c4c 6170  ame as 'TotalLap
+00008ed0: 7327 2069 6e20 7468 6520 7361 6d65 2073  s' in the same s
+00008ee0: 616d 706c 653f 213f 290a 2020 2020 2020  ample?!?).      
+00008ef0: 202d 204f 7574 6c61 7020 284e 6f6e 6520   - Outlap (None 
+00008f00: 6f72 203f 3f3f 293a 203f 3f3f 2075 6e6b  or ???): ??? unk
+00008f10: 6e6f 776e 3b20 6e6f 2064 6174 610a 0a20  nown; no data.. 
+00008f20: 2020 204f 6e6c 7920 6120 6665 7720 7661     Only a few va
+00008f30: 6c75 6573 2061 7265 2070 7265 7365 6e74  lues are present
+00008f40: 2070 6572 2074 696d 6573 7461 6d70 2e20   per timestamp. 
+00008f50: 536f 6d65 7768 6174 2063 6f6d 7072 6568  Somewhat compreh
+00008f60: 656e 7369 7665 2069 6e66 6f72 6d61 7469  ensive informati
+00008f70: 6f6e 2063 616e 2074 6865 7265 666f 7265  on can therefore
+00008f80: 206f 6e6c 7920 6265 206f 6274 6169 6e65   only be obtaine
+00008f90: 6420 6279 0a20 2020 2061 6767 7265 6761  d by.    aggrega
+00008fa0: 7469 6e67 2064 6174 6120 2875 7375 616c  ting data (usual
+00008fb0: 6c79 206f 7665 7220 7468 6520 636f 7572  ly over the cour
+00008fc0: 7365 206f 6620 6f6e 6520 6c61 7029 2e20  se of one lap). 
+00008fd0: 536f 6d65 2076 616c 7565 7320 6172 6520  Some values are 
+00008fe0: 7365 6e74 2065 7665 6e20 6c65 7373 0a20  sent even less. 
+00008ff0: 2020 2066 7265 7175 656e 746c 7920 2866     frequently (f
+00009000: 6f72 2065 7861 6d70 6c65 2027 436f 6d70  or example 'Comp
+00009010: 6f75 6e64 2720 6f6e 6c79 2061 6674 6572  ound' only after
+00009020: 2074 6972 6520 6368 616e 6765 7329 2e0a   tire changes)..
+00009030: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
+00009040: 2020 2070 6174 6820 2873 7472 293a 2061     path (str): a
+00009050: 7069 2070 6174 6820 6261 7365 2073 7472  pi path base str
+00009060: 696e 6720 2875 7375 616c 6c79 2060 6053  ing (usually ``S
+00009070: 6573 7369 6f6e 2e61 7069 5f70 6174 6860  ession.api_path`
+00009080: 6029 0a20 2020 2020 2020 2072 6573 706f  `).        respo
+00009090: 6e73 653a 2052 6573 706f 6e73 6520 6173  nse: Response as
+000090a0: 2072 6574 7572 6e65 6420 6279 203a 6675   returned by :fu
+000090b0: 6e63 3a60 6665 7463 685f 7061 6765 6020  nc:`fetch_page` 
+000090c0: 6361 6e20 6265 2070 6173 7365 6420 6966  can be passed if
+000090d0: 2069 7420 7761 7320 646f 776e 6c6f 6164   it was download
+000090e0: 6564 2061 6c72 6561 6479 2e0a 2020 2020  ed already..    
+000090f0: 2020 2020 6c69 7665 6461 7461 3a20 416e      livedata: An
+00009100: 2069 6e73 7461 6e63 6520 6f66 203a 636c   instance of :cl
+00009110: 6173 733a 6066 6173 7466 312e 6c69 7665  ass:`fastf1.live
+00009120: 7469 6d69 6e67 2e64 6174 612e 4c69 7665  timing.data.Live
+00009130: 5469 6d69 6e67 4461 7461 6020 746f 2075  TimingData` to u
+00009140: 7365 2061 7320 6120 736f 7572 6365 2069  se as a source i
+00009150: 6e73 7465 6164 206f 6620 7468 6520 6170  nstead of the ap
+00009160: 690a 0a20 2020 2052 6574 7572 6e73 3a0a  i..    Returns:.
+00009170: 2020 2020 2020 2020 4120 4461 7461 4672          A DataFr
+00009180: 616d 6520 636f 6e74 6169 6e69 6e67 206f  ame containing o
+00009190: 6e65 2063 6f6c 756d 6e20 666f 7220 6561  ne column for ea
+000091a0: 6368 2064 6174 6120 6368 616e 6e65 6c20  ch data channel 
+000091b0: 6c69 7374 6564 2061 626f 7665 2e0a 0a20  listed above... 
+000091c0: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
+000091d0: 2020 2053 6573 7369 6f6e 4e6f 7441 7661     SessionNotAva
+000091e0: 696c 6162 6c65 4572 726f 723a 2069 6e20  ilableError: in 
+000091f0: 6361 7365 2074 6865 2046 3120 6c69 7665  case the F1 live
+00009200: 7469 6d69 6e67 2061 7069 2072 6574 7572  timing api retur
+00009210: 6e73 206e 6f20 6461 7461 0a20 2020 2022  ns no data.    "
+00009220: 2222 0a20 2020 2069 6620 6c69 7665 6461  "".    if liveda
+00009230: 7461 2069 7320 6e6f 7420 4e6f 6e65 2061  ta is not None a
+00009240: 6e64 206c 6976 6564 6174 612e 6861 7328  nd livedata.has(
+00009250: 2754 696d 696e 6741 7070 4461 7461 2729  'TimingAppData')
+00009260: 3a0a 2020 2020 2020 2020 7265 7370 6f6e  :.        respon
+00009270: 7365 203d 206c 6976 6564 6174 612e 6765  se = livedata.ge
+00009280: 7428 2754 696d 696e 6741 7070 4461 7461  t('TimingAppData
+00009290: 2729 0a20 2020 2065 6c69 6620 7265 7370  ').    elif resp
+000092a0: 6f6e 7365 2069 7320 4e6f 6e65 3a20 2023  onse is None:  #
+000092b0: 206e 6f20 7072 6576 696f 7573 2072 6573   no previous res
+000092c0: 706f 6e73 6520 7072 6f76 6964 6564 0a20  ponse provided. 
+000092d0: 2020 2020 2020 205f 6c6f 6767 6572 2e69         _logger.i
+000092e0: 6e66 6f28 2246 6574 6368 696e 6720 7469  nfo("Fetching ti
+000092f0: 6d69 6e67 2061 7070 2064 6174 612e 2e2e  ming app data...
+00009300: 2229 0a20 2020 2020 2020 2072 6573 706f  ").        respo
+00009310: 6e73 6520 3d20 6665 7463 685f 7061 6765  nse = fetch_page
+00009320: 2870 6174 682c 2027 7469 6d69 6e67 5f61  (path, 'timing_a
+00009330: 7070 5f64 6174 6127 290a 2020 2020 2020  pp_data').      
+00009340: 2020 6966 2072 6573 706f 6e73 6520 6973    if response is
+00009350: 204e 6f6e 653a 2020 2320 6e6f 2072 6573   None:  # no res
+00009360: 706f 6e73 6520 7265 6365 6976 6564 0a20  ponse received. 
+00009370: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00009380: 2053 6573 7369 6f6e 4e6f 7441 7661 696c   SessionNotAvail
+00009390: 6162 6c65 4572 726f 7228 0a20 2020 2020  ableError(.     
+000093a0: 2020 2020 2020 2020 2020 2022 4e6f 2064             "No d
+000093b0: 6174 6120 666f 7220 7468 6973 2073 6573  ata for this ses
+000093c0: 7369 6f6e 2120 4966 2074 6869 7320 7365  sion! If this se
+000093d0: 7373 696f 6e20 6f6e 6c79 2066 696e 6973  ssion only finis
+000093e0: 6865 6420 220a 2020 2020 2020 2020 2020  hed ".          
+000093f0: 2020 2020 2020 2272 6563 656e 746c 792c        "recently,
+00009400: 2070 6c65 6173 6520 7472 7920 6167 6169   please try agai
+00009410: 6e20 696e 2061 2066 6577 206d 696e 7574  n in a few minut
+00009420: 6573 2e22 0a20 2020 2020 2020 2020 2020  es.".           
+00009430: 2029 0a0a 2020 2020 6461 7461 203d 207b   )..    data = {
+00009440: 274c 6170 4e75 6d62 6572 273a 205b 5d2c  'LapNumber': [],
+00009450: 2027 4472 6976 6572 273a 205b 5d2c 2027   'Driver': [], '
+00009460: 4c61 7054 696d 6527 3a20 5b5d 2c20 2753  LapTime': [], 'S
+00009470: 7469 6e74 273a 205b 5d2c 2027 546f 7461  tint': [], 'Tota
+00009480: 6c4c 6170 7327 3a20 5b5d 2c20 2743 6f6d  lLaps': [], 'Com
+00009490: 706f 756e 6427 3a20 5b5d 2c20 274e 6577  pound': [], 'New
+000094a0: 273a 205b 5d2c 0a20 2020 2020 2020 2020  ': [],.         
+000094b0: 2020 2027 5479 7265 734e 6f74 4368 616e     'TyresNotChan
+000094c0: 6765 6427 3a20 5b5d 2c20 2754 696d 6527  ged': [], 'Time'
+000094d0: 3a20 5b5d 2c20 274c 6170 466c 6167 7327  : [], 'LapFlags'
+000094e0: 3a20 5b5d 2c20 274c 6170 436f 756e 7454  : [], 'LapCountT
+000094f0: 696d 6527 3a20 5b5d 2c20 2753 7461 7274  ime': [], 'Start
+00009500: 4c61 7073 273a 205b 5d2c 2027 4f75 746c  Laps': [], 'Outl
+00009510: 6170 273a 205b 5d7d 0a0a 2020 2020 666f  ap': []}..    fo
+00009520: 7220 656e 7472 7920 696e 2072 6573 706f  r entry in respo
+00009530: 6e73 653a 0a20 2020 2020 2020 2069 6620  nse:.        if 
+00009540: 286c 656e 2865 6e74 7279 2920 3c20 3229  (len(entry) < 2)
+00009550: 206f 7220 274c 696e 6573 2720 6e6f 7420   or 'Lines' not 
+00009560: 696e 2065 6e74 7279 5b31 5d3a 0a20 2020  in entry[1]:.   
+00009570: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+00009580: 650a 0a20 2020 2020 2020 2074 696d 6520  e..        time 
+00009590: 3d20 746f 5f74 696d 6564 656c 7461 2865  = to_timedelta(e
+000095a0: 6e74 7279 5b30 5d29 0a20 2020 2020 2020  ntry[0]).       
+000095b0: 2072 6f77 203d 2065 6e74 7279 5b31 5d0a   row = entry[1].
+000095c0: 2020 2020 2020 2020 666f 7220 6472 6976          for driv
+000095d0: 6572 5f6e 756d 6265 7220 696e 2072 6f77  er_number in row
+000095e0: 5b27 4c69 6e65 7327 5d3a 0a20 2020 2020  ['Lines']:.     
+000095f0: 2020 2020 2020 2069 6620 7570 6461 7465         if update
+00009600: 203a 3d20 7265 6375 7273 6976 655f 6469   := recursive_di
+00009610: 6374 5f67 6574 2872 6f77 2c20 274c 696e  ct_get(row, 'Lin
+00009620: 6573 272c 2064 7269 7665 725f 6e75 6d62  es', driver_numb
+00009630: 6572 2c20 2753 7469 6e74 7327 293a 0a20  er, 'Stints'):. 
+00009640: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00009650: 6f72 2073 7469 6e74 5f6e 756d 6265 722c  or stint_number,
+00009660: 2073 7469 6e74 2069 6e20 656e 756d 6572   stint in enumer
+00009670: 6174 6528 7570 6461 7465 293a 0a20 2020  ate(update):.   
+00009680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009690: 2069 6620 6973 696e 7374 616e 6365 2875   if isinstance(u
+000096a0: 7064 6174 652c 2064 6963 7429 3a0a 2020  pdate, dict):.  
+000096b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096c0: 2020 2020 2020 7374 696e 745f 6e75 6d62        stint_numb
+000096d0: 6572 203d 2069 6e74 2873 7469 6e74 290a  er = int(stint).
+000096e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096f0: 2020 2020 2020 2020 7374 696e 7420 3d20          stint = 
+00009700: 7570 6461 7465 5b73 7469 6e74 5d0a 2020  update[stint].  
+00009710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009720: 2020 666f 7220 6b65 7920 696e 2064 6174    for key in dat
+00009730: 613a 0a20 2020 2020 2020 2020 2020 2020  a:.             
+00009740: 2020 2020 2020 2020 2020 2069 6620 6b65             if ke
+00009750: 7920 696e 2073 7469 6e74 3a0a 2020 2020  y in stint:.    
+00009760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009770: 2020 2020 2020 2020 7661 6c20 3d20 7374          val = st
+00009780: 696e 745b 6b65 795d 0a20 2020 2020 2020  int[key].       
+00009790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097a0: 2020 2020 2069 6620 6b65 7920 3d3d 2027       if key == '
+000097b0: 4c61 7054 696d 6527 3a0a 2020 2020 2020  LapTime':.      
+000097c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097d0: 2020 2020 2020 2020 2020 7661 6c20 3d20            val = 
+000097e0: 746f 5f74 696d 6564 656c 7461 2876 616c  to_timedelta(val
+000097f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00009800: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00009810: 6966 206b 6579 203d 3d20 274e 6577 273a  if key == 'New':
+00009820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009840: 2076 616c 203d 2054 7275 6520 6966 2076   val = True if v
+00009850: 616c 203d 3d20 2774 7275 6527 2065 6c73  al == 'true' els
+00009860: 6520 4661 6c73 650a 2020 2020 2020 2020  e False.        
+00009870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009880: 2020 2020 6461 7461 5b6b 6579 5d2e 6170      data[key].ap
+00009890: 7065 6e64 2876 616c 290a 2020 2020 2020  pend(val).      
+000098a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000098c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098d0: 2020 2020 6461 7461 5b6b 6579 5d2e 6170      data[key].ap
+000098e0: 7065 6e64 284e 6f6e 6529 0a20 2020 2020  pend(None).     
+000098f0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00009900: 6f72 206b 6579 2069 6e20 7374 696e 743a  or key in stint:
+00009910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009920: 2020 2020 2020 2020 2069 6620 6b65 7920           if key 
+00009930: 6e6f 7420 696e 2064 6174 613a 0a20 2020  not in data:.   
+00009940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009950: 2020 2020 2020 2020 205f 6c6f 6767 6572           _logger
+00009960: 2e64 6562 7567 2866 2246 6f75 6e64 2075  .debug(f"Found u
+00009970: 6e6b 6e6f 776e 206b 6579 2069 6e20 7469  nknown key in ti
+00009980: 6d69 6e67 2061 7070 2022 0a20 2020 2020  ming app ".     
 00009990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099a0: 2020 2020 2020 2020 2069 6620 6b65 7920           if key 
-000099b0: 3d3d 2027 4c61 7054 696d 6527 3a0a 2020  == 'LapTime':.  
-000099c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099d0: 2020 2020 2020 2020 2020 2020 2020 7661                va
-000099e0: 6c20 3d20 746f 5f74 696d 6564 656c 7461  l = to_timedelta
-000099f0: 2876 616c 290a 2020 2020 2020 2020 2020  (val).          
-00009a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a10: 2020 656c 6966 206b 6579 203d 3d20 274e    elif key == 'N
-00009a20: 6577 273a 0a20 2020 2020 2020 2020 2020  ew':.           
-00009a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a40: 2020 2020 2076 616c 203d 2054 7275 6520       val = True 
-00009a50: 6966 2076 616c 203d 3d20 2774 7275 6527  if val == 'true'
-00009a60: 2065 6c73 6520 4661 6c73 650a 2020 2020   else False.    
-00009a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a80: 2020 2020 2020 2020 6461 7461 5b6b 6579          data[key
-00009a90: 5d2e 6170 7065 6e64 2876 616c 290a 2020  ].append(val).  
-00009aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ab0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00009ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ad0: 2020 2020 2020 2020 6461 7461 5b6b 6579          data[key
-00009ae0: 5d2e 6170 7065 6e64 284e 6f6e 6529 0a20  ].append(None). 
-00009af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b00: 2020 2066 6f72 206b 6579 2069 6e20 7374     for key in st
-00009b10: 696e 743a 0a20 2020 2020 2020 2020 2020  int:.           
-00009b20: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00009b30: 6b65 7920 6e6f 7420 696e 2064 6174 613a  key not in data:
-00009b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009b50: 2020 2020 2020 2020 2020 2020 205f 6c6f               _lo
-00009b60: 6767 6572 2e64 6562 7567 2866 2246 6f75  gger.debug(f"Fou
-00009b70: 6e64 2075 6e6b 6e6f 776e 206b 6579 2069  nd unknown key i
-00009b80: 6e20 7469 6d69 6e67 2061 7070 2022 0a20  n timing app ". 
-00009b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bb0: 2020 2020 2020 2020 2066 2264 6174 613a           f"data:
-00009bc0: 207b 6b65 797d 2229 0a0a 2020 2020 2020   {key}")..      
-00009bd0: 2020 2020 2020 2020 2020 2020 2020 6461                da
-00009be0: 7461 5b27 5469 6d65 275d 5b2d 315d 203d  ta['Time'][-1] =
-00009bf0: 2074 696d 650a 2020 2020 2020 2020 2020   time.          
-00009c00: 2020 2020 2020 2020 2020 6461 7461 5b27            data['
-00009c10: 4472 6976 6572 275d 5b2d 315d 203d 2064  Driver'][-1] = d
-00009c20: 7269 7665 725f 6e75 6d62 6572 0a20 2020  river_number.   
-00009c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c40: 2064 6174 615b 2753 7469 6e74 275d 5b2d   data['Stint'][-
-00009c50: 315d 203d 2073 7469 6e74 5f6e 756d 6265  1] = stint_numbe
-00009c60: 720a 0a20 2020 2064 6620 3d20 7064 2e44  r..    df = pd.D
-00009c70: 6174 6146 7261 6d65 2864 6174 6129 0a20  ataFrame(data). 
-00009c80: 2020 2023 2070 616e 6461 7320 646f 6573     # pandas does
-00009c90: 6e27 7420 636f 7272 6563 746c 7920 696e  n't correctly in
-00009ca0: 6665 7220 626f 6f6c 2064 7479 7065 2063  fer bool dtype c
-00009cb0: 6f6c 756d 6e73 2c20 7365 7420 7479 7065  olumns, set type
-00009cc0: 2065 7870 6c69 6369 746c 790a 2020 2020   explicitly.    
-00009cd0: 6466 5b5b 274e 6577 272c 2027 5479 7265  df[['New', 'Tyre
-00009ce0: 734e 6f74 4368 616e 6765 6427 5d5d 205c  sNotChanged']] \
-00009cf0: 0a20 2020 2020 2020 203d 2064 665b 5b27  .        = df[['
-00009d00: 4e65 7727 2c20 2754 7972 6573 4e6f 7443  New', 'TyresNotC
-00009d10: 6861 6e67 6564 275d 5d2e 6173 7479 7065  hanged']].astype
-00009d20: 2862 6f6f 6c29 0a20 2020 2072 6574 7572  (bool).    retur
-00009d30: 6e20 6466 0a0a 0a40 4361 6368 652e 6170  n df...@Cache.ap
-00009d40: 695f 7265 7175 6573 745f 7772 6170 7065  i_request_wrappe
-00009d50: 720a 6465 6620 6361 725f 6461 7461 2870  r.def car_data(p
-00009d60: 6174 682c 2072 6573 706f 6e73 653d 4e6f  ath, response=No
-00009d70: 6e65 2c20 6c69 7665 6461 7461 3d4e 6f6e  ne, livedata=Non
-00009d80: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
-00009d90: 2e2e 2077 6172 6e69 6e67 3a3a 0a20 2020  .. warning::.   
-00009da0: 2020 2020 203a 6d6f 643a 6066 6173 7466       :mod:`fastf
-00009db0: 312e 6170 6960 2077 696c 6c20 6265 2063  1.api` will be c
-00009dc0: 6f6e 7369 6465 7265 6420 7072 6976 6174  onsidered privat
-00009dd0: 6520 696e 2066 7574 7572 6520 7265 6c65  e in future rele
-00009de0: 6173 6573 2061 6e64 0a20 2020 2020 2020  ases and.       
-00009df0: 2070 6f74 656e 7469 616c 6c79 2062 6520   potentially be 
-00009e00: 7265 6d6f 7665 6420 6f72 2063 6861 6e67  removed or chang
-00009e10: 6564 2e0a 0a20 2020 2046 6574 6368 2061  ed...    Fetch a
-00009e20: 6e64 2070 6172 7365 2063 6172 2064 6174  nd parse car dat
-00009e30: 612e 0a0a 2020 2020 4361 7220 6461 7461  a...    Car data
-00009e40: 2070 726f 7669 6465 7320 7468 6520 666f   provides the fo
-00009e50: 6c6c 6f77 696e 6720 6461 7461 2063 6861  llowing data cha
-00009e60: 6e6e 656c 7320 7065 7220 7361 6d70 6c65  nnels per sample
-00009e70: 3a0a 2020 2020 2020 2020 2d20 5469 6d65  :.        - Time
-00009e80: 2028 7061 6e64 6173 2e54 696d 6564 656c   (pandas.Timedel
-00009e90: 7461 293a 2073 6573 7369 6f6e 2074 696d  ta): session tim
-00009ea0: 6573 7461 6d70 2028 7469 6d65 206f 6e6c  estamp (time onl
-00009eb0: 7929 3b20 696e 6163 6375 7261 7465 2c20  y); inaccurate, 
-00009ec0: 6861 7320 6475 706c 6963 6174 6520 7661  has duplicate va
-00009ed0: 6c75 6573 3b20 7573 6520 4461 7465 2069  lues; use Date i
-00009ee0: 6e73 7465 6164 0a20 2020 2020 2020 202d  nstead.        -
-00009ef0: 2044 6174 6520 2870 616e 6461 732e 5469   Date (pandas.Ti
-00009f00: 6d65 7374 616d 7029 3a20 7469 6d65 7374  mestamp): timest
-00009f10: 616d 7020 666f 7220 7468 6973 2073 616d  amp for this sam
-00009f20: 706c 6520 6173 2044 6174 6520 2b20 5469  ple as Date + Ti
-00009f30: 6d65 3b20 6d6f 7265 206f 7220 6c65 7373  me; more or less
-00009f40: 2065 7861 6374 0a20 2020 2020 2020 202d   exact.        -
-00009f50: 2053 7065 6564 2028 696e 7429 3a20 4b6d   Speed (int): Km
-00009f60: 2f68 0a20 2020 2020 2020 202d 2052 504d  /h.        - RPM
-00009f70: 2028 696e 7429 0a20 2020 2020 2020 202d   (int).        -
-00009f80: 2047 6561 7220 2869 6e74 293a 205b 6361   Gear (int): [ca
-00009f90: 6c6c 6564 2027 6e47 6561 7227 2069 6e20  lled 'nGear' in 
-00009fa0: 7468 6520 6461 7461 215d 0a20 2020 2020  the data!].     
-00009fb0: 2020 202d 2054 6872 6f74 746c 6520 2869     - Throttle (i
-00009fc0: 6e74 293a 2030 2d31 3030 250a 2020 2020  nt): 0-100%.    
-00009fd0: 2020 2020 2d20 4272 616b 6520 2862 6f6f      - Brake (boo
-00009fe0: 6c29 0a20 2020 2020 2020 202d 2044 5253  l).        - DRS
-00009ff0: 2028 696e 7429 3a20 302d 3134 2028 4f64   (int): 0-14 (Od
-0000a000: 6420 4452 5320 6973 2044 6973 6162 6c65  d DRS is Disable
-0000a010: 642c 2045 7665 6e20 4452 5320 6973 2045  d, Even DRS is E
-0000a020: 6e61 626c 6564 3f29 0a20 2020 2020 2020  nabled?).       
-0000a030: 2020 2028 4d6f 7265 2052 6573 6561 7263     (More Researc
-0000a040: 6820 4e65 6564 6564 3f29 0a0a 2020 2020  h Needed?)..    
-0000a050: 2020 2020 2020 2d20 3020 3d20 204f 6666        - 0 =  Off
-0000a060: 0a20 2020 2020 2020 2020 202d 2031 203d  .          - 1 =
-0000a070: 2020 4f66 660a 2020 2020 2020 2020 2020    Off.          
-0000a080: 2d20 3220 3d20 2028 3f29 0a20 2020 2020  - 2 =  (?).     
-0000a090: 2020 2020 202d 2033 203d 2020 283f 290a       - 3 =  (?).
-0000a0a0: 2020 2020 2020 2020 2020 2d20 3820 3d20            - 8 = 
-0000a0b0: 2044 6574 6563 7465 642c 2045 6c69 6769   Detected, Eligi
-0000a0c0: 626c 6520 6f6e 6365 2069 6e20 4163 7469  ble once in Acti
-0000a0d0: 7661 7469 6f6e 205a 6f6e 6520 284e 6f74  vation Zone (Not
-0000a0e0: 6564 2053 6f6d 6574 696d 6573 290a 2020  ed Sometimes).  
-0000a0f0: 2020 2020 2020 2020 2d20 3130 203d 204f          - 10 = O
-0000a100: 6e20 2855 6e6b 6e6f 776e 2044 6973 7469  n (Unknown Disti
-0000a110: 6e63 7469 6f6e 290a 2020 2020 2020 2020  nction).        
-0000a120: 2020 2d20 3132 203d 204f 6e20 2855 6e6b    - 12 = On (Unk
-0000a130: 6e6f 776e 2044 6973 7469 6e63 7469 6f6e  nown Distinction
-0000a140: 290a 2020 2020 2020 2020 2020 2d20 3134  ).          - 14
-0000a150: 203d 204f 6e20 2855 6e6b 6e6f 776e 2044   = On (Unknown D
-0000a160: 6973 7469 6e63 7469 6f6e 290a 0a20 2020  istinction)..   
-0000a170: 2020 2020 202d 2053 6f75 7263 6520 2873       - Source (s
-0000a180: 7472 293a 2049 6e64 6963 6174 6573 2074  tr): Indicates t
-0000a190: 6865 2073 6f75 7263 6520 6f66 2061 2073  he source of a s
-0000a1a0: 616d 706c 653b 2027 6361 7227 2066 6f72  ample; 'car' for
-0000a1b0: 2061 6c6c 2076 616c 7565 7320 6865 7265   all values here
-0000a1c0: 0a0a 2020 2020 5468 6520 6461 7461 2073  ..    The data s
-0000a1d0: 7472 6561 6d20 6861 7320 6120 7361 6d70  tream has a samp
-0000a1e0: 6c65 2072 6174 6520 6f66 2028 7573 7561  le rate of (usua
-0000a1f0: 6c6c 7929 2032 3430 6d73 2e20 5468 6520  lly) 240ms. The 
-0000a200: 7361 6d70 6c65 7320 6672 6f6d 2074 6865  samples from the
-0000a210: 2064 6174 6120 7374 7265 616d 7320 666f   data streams fo
-0000a220: 7220 706f 7369 7469 6f6e 2064 6174 6120  r position data 
-0000a230: 616e 640a 2020 2020 6361 7220 6461 7461  and.    car data
-0000a240: 2064 6f20 6e6f 7420 6c69 6e65 2075 702e   do not line up.
-0000a250: 2052 6573 616d 706c 696e 672f 696e 7465   Resampling/inte
-0000a260: 7270 6f6c 6174 696f 6e20 6973 2072 6571  rpolation is req
-0000a270: 7569 7265 6420 746f 206d 6572 6765 2074  uired to merge t
-0000a280: 6865 6d2e 0a0a 2020 2020 4172 6773 3a0a  hem...    Args:.
-0000a290: 2020 2020 2020 2020 7061 7468 2028 7374          path (st
-0000a2a0: 7229 3a20 6170 6920 7061 7468 2062 6173  r): api path bas
-0000a2b0: 6520 7374 7269 6e67 2028 7573 7561 6c6c  e string (usuall
-0000a2c0: 7920 6060 5365 7373 696f 6e2e 6170 695f  y ``Session.api_
-0000a2d0: 7061 7468 6060 290a 2020 2020 2020 2020  path``).        
-0000a2e0: 7265 7370 6f6e 7365 3a20 5265 7370 6f6e  response: Respon
-0000a2f0: 7365 2061 7320 7265 7475 726e 6564 2062  se as returned b
-0000a300: 7920 3a66 756e 633a 6066 6574 6368 5f70  y :func:`fetch_p
-0000a310: 6167 6560 2063 616e 2062 6520 7061 7373  age` can be pass
-0000a320: 6564 2069 6620 6974 2077 6173 2064 6f77  ed if it was dow
-0000a330: 6e6c 6f61 6465 6420 616c 7265 6164 792e  nloaded already.
-0000a340: 0a20 2020 2020 2020 206c 6976 6564 6174  .        livedat
-0000a350: 613a 2041 6e20 696e 7374 616e 6365 206f  a: An instance o
-0000a360: 6620 3a63 6c61 7373 3a60 6661 7374 6631  f :class:`fastf1
-0000a370: 2e6c 6976 6574 696d 696e 672e 6461 7461  .livetiming.data
-0000a380: 2e4c 6976 6554 696d 696e 6744 6174 6160  .LiveTimingData`
-0000a390: 2074 6f20 7573 6520 6173 2061 2073 6f75   to use as a sou
-0000a3a0: 7263 6520 696e 7374 6561 6420 6f66 2074  rce instead of t
-0000a3b0: 6865 2061 7069 0a0a 2020 2020 5265 7475  he api..    Retu
-0000a3c0: 726e 733a 0a20 2020 2020 2020 207c 2041  rns:.        | A
-0000a3d0: 2064 6963 7469 6f6e 6172 7920 636f 6e74   dictionary cont
-0000a3e0: 6169 6e69 6e67 206f 6e65 2070 616e 6461  aining one panda
-0000a3f0: 7320 4461 7461 4672 616d 6520 7065 7220  s DataFrame per 
-0000a400: 6472 6976 6572 2e20 4469 6374 696f 6e61  driver. Dictiona
-0000a410: 7279 206b 6579 7320 6172 6520 7468 6520  ry keys are the 
-0000a420: 6472 6976 6572 2773 206e 756d 6265 7273  driver's numbers
-0000a430: 2061 730a 2020 2020 2020 2020 2020 7374   as.          st
-0000a440: 7269 6e67 2028 652e 672e 2027 3136 2729  ring (e.g. '16')
-0000a450: 2e20 596f 7520 7368 6f75 6c64 206e 6576  . You should nev
-0000a460: 6572 2061 7373 756d 6520 7468 6174 2061  er assume that a
-0000a470: 206e 756d 6265 7220 6578 6973 7473 210a   number exists!.
-0000a480: 2020 2020 2020 2020 7c20 4561 6368 2064          | Each d
-0000a490: 6174 6166 7261 6d65 2063 6f6e 7461 696e  ataframe contain
-0000a4a0: 7320 6f6e 6520 636f 6c75 6d6e 2066 6f72  s one column for
-0000a4b0: 2065 6163 6820 6461 7461 2063 6861 6e6e   each data chann
-0000a4c0: 656c 2061 7320 6c69 7374 6564 2061 626f  el as listed abo
-0000a4d0: 7665 0a0a 2020 2020 5261 6973 6573 3a0a  ve..    Raises:.
-0000a4e0: 2020 2020 2020 2020 5365 7373 696f 6e4e          SessionN
-0000a4f0: 6f74 4176 6169 6c61 626c 6545 7272 6f72  otAvailableError
-0000a500: 3a20 696e 2063 6173 6520 7468 6520 4631  : in case the F1
-0000a510: 206c 6976 6574 696d 696e 6720 6170 6920   livetiming api 
-0000a520: 7265 7475 726e 7320 6e6f 2064 6174 610a  returns no data.
-0000a530: 2020 2020 2222 220a 2020 2020 2320 6461      """.    # da
-0000a540: 7461 2072 6563 6f72 6465 6420 6672 6f6d  ta recorded from
-0000a550: 206c 6976 6520 7469 6d69 6e67 2068 6173   live timing has
-0000a560: 2061 2073 6c69 6768 746c 7920 6469 6666   a slightly diff
-0000a570: 6572 656e 7420 7374 7275 6374 7572 650a  erent structure.
-0000a580: 2020 2020 6973 5f6c 6976 6564 6174 6120      is_livedata 
-0000a590: 3d20 4661 6c73 6520 2023 2066 6c61 6720  = False  # flag 
-0000a5a0: 746f 2069 6e64 6963 6174 6520 6c69 7665  to indicate live
-0000a5b0: 2074 696d 696e 6720 6461 7461 0a0a 2020   timing data..  
-0000a5c0: 2020 6966 206c 6976 6564 6174 6120 6973    if livedata is
-0000a5d0: 206e 6f74 204e 6f6e 6520 616e 6420 6c69   not None and li
-0000a5e0: 7665 6461 7461 2e68 6173 2827 4361 7244  vedata.has('CarD
-0000a5f0: 6174 612e 7a27 293a 0a20 2020 2020 2020  ata.z'):.       
-0000a600: 2072 6573 706f 6e73 6520 3d20 6c69 7665   response = live
-0000a610: 6461 7461 2e67 6574 2827 4361 7244 6174  data.get('CarDat
-0000a620: 612e 7a27 290a 2020 2020 2020 2020 6973  a.z').        is
-0000a630: 5f6c 6976 6564 6174 6120 3d20 5472 7565  _livedata = True
-0000a640: 0a20 2020 2065 6c69 6620 7265 7370 6f6e  .    elif respon
-0000a650: 7365 2069 7320 4e6f 6e65 3a0a 2020 2020  se is None:.    
-0000a660: 2020 2020 5f6c 6f67 6765 722e 696e 666f      _logger.info
-0000a670: 2822 4665 7463 6869 6e67 2063 6172 2064  ("Fetching car d
-0000a680: 6174 612e 2e2e 2229 0a20 2020 2020 2020  ata...").       
-0000a690: 2072 6573 706f 6e73 6520 3d20 6665 7463   response = fetc
-0000a6a0: 685f 7061 6765 2870 6174 682c 2027 6361  h_page(path, 'ca
-0000a6b0: 725f 6461 7461 2729 0a20 2020 2020 2020  r_data').       
-0000a6c0: 2069 6620 7265 7370 6f6e 7365 2069 7320   if response is 
-0000a6d0: 4e6f 6e65 3a20 2023 206e 6f20 7265 7370  None:  # no resp
-0000a6e0: 6f6e 7365 2072 6563 6569 7665 640a 2020  onse received.  
-0000a6f0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000a700: 5365 7373 696f 6e4e 6f74 4176 6169 6c61  SessionNotAvaila
-0000a710: 626c 6545 7272 6f72 280a 2020 2020 2020  bleError(.      
-0000a720: 2020 2020 2020 2020 2020 224e 6f20 6461            "No da
-0000a730: 7461 2066 6f72 2074 6869 7320 7365 7373  ta for this sess
-0000a740: 696f 6e21 2049 6620 7468 6973 2073 6573  ion! If this ses
-0000a750: 7369 6f6e 206f 6e6c 7920 6669 6e69 7368  sion only finish
-0000a760: 6564 2022 0a20 2020 2020 2020 2020 2020  ed ".           
-0000a770: 2020 2020 2022 7265 6365 6e74 6c79 2c20       "recently, 
-0000a780: 706c 6561 7365 2074 7279 2061 6761 696e  please try again
-0000a790: 2069 6e20 6120 6665 7720 6d69 6e75 7465   in a few minute
-0000a7a0: 732e 220a 2020 2020 2020 2020 2020 2020  s.".            
-0000a7b0: 290a 0a20 2020 205f 6c6f 6767 6572 2e69  )..    _logger.i
-0000a7c0: 6e66 6f28 2250 6172 7369 6e67 2063 6172  nfo("Parsing car
-0000a7d0: 2064 6174 612e 2e2e 2229 0a0a 2020 2020   data...")..    
-0000a7e0: 6e75 6d65 7269 635f 6368 616e 6e65 6c73  numeric_channels
-0000a7f0: 203d 205b 2752 504d 272c 2027 5370 6565   = ['RPM', 'Spee
-0000a800: 6427 2c20 276e 4765 6172 272c 2027 5468  d', 'nGear', 'Th
-0000a810: 726f 7474 6c65 272c 2027 4452 5327 5d0a  rottle', 'DRS'].
-0000a820: 2020 2020 626f 6f6c 5f63 6861 6e6e 656c      bool_channel
-0000a830: 7320 3d20 5b27 4272 616b 6527 5d0a 2020  s = ['Brake'].  
-0000a840: 2020 636f 6c75 6d6e 7320 3d20 5b27 5469    columns = ['Ti
-0000a850: 6d65 272c 2027 4461 7465 272c 2027 5250  me', 'Date', 'RP
-0000a860: 4d27 2c20 2753 7065 6564 272c 2027 6e47  M', 'Speed', 'nG
-0000a870: 6561 7227 2c20 2754 6872 6f74 746c 6527  ear', 'Throttle'
-0000a880: 2c20 2742 7261 6b65 272c 0a20 2020 2020  , 'Brake',.     
-0000a890: 2020 2020 2020 2020 2020 2744 5253 272c            'DRS',
-0000a8a0: 2027 536f 7572 6365 275d 2020 2320 636f   'Source']  # co
-0000a8b0: 7272 6563 7420 6f72 6465 7220 7265 7175  rrect order requ
-0000a8c0: 6972 6564 210a 0a20 2020 2074 735f 6c65  ired!..    ts_le
-0000a8d0: 6e67 7468 203d 2031 3220 2023 206c 656e  ngth = 12  # len
-0000a8e0: 6774 6820 6f66 2074 696d 6573 7461 6d70  gth of timestamp
-0000a8f0: 3a20 6c65 6e28 2730 303a 3030 3a30 303a  : len('00:00:00:
-0000a900: 3030 3027 290a 0a20 2020 2064 6174 6120  000')..    data 
-0000a910: 3d20 6469 6374 2829 0a20 2020 2064 6563  = dict().    dec
-0000a920: 6f64 655f 6572 726f 725f 636f 756e 7420  ode_error_count 
-0000a930: 3d20 300a 0a20 2020 2066 6f72 2072 6563  = 0..    for rec
-0000a940: 6f72 6420 696e 2072 6573 706f 6e73 653a  ord in response:
-0000a950: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-0000a960: 2020 2020 2020 2020 2020 6966 2069 735f            if is_
-0000a970: 6c69 7665 6461 7461 3a0a 2020 2020 2020  livedata:.      
-0000a980: 2020 2020 2020 2020 2020 7469 6d65 203d            time =
-0000a990: 2074 6f5f 7469 6d65 6465 6c74 6128 7265   to_timedelta(re
-0000a9a0: 636f 7264 5b30 5d29 0a20 2020 2020 2020  cord[0]).       
-0000a9b0: 2020 2020 2020 2020 206a 7265 636f 7264           jrecord
-0000a9c0: 3a20 6469 6374 203d 2070 6172 7365 2872  : dict = parse(r
-0000a9d0: 6563 6f72 645b 315d 2c20 7a69 7070 6564  ecord[1], zipped
-0000a9e0: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-0000a9f0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000aa00: 2020 2020 2020 2020 2074 696d 6520 3d20           time = 
-0000aa10: 746f 5f74 696d 6564 656c 7461 2872 6563  to_timedelta(rec
-0000aa20: 6f72 645b 3a74 735f 6c65 6e67 7468 5d29  ord[:ts_length])
-0000aa30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000aa40: 206a 7265 636f 7264 3a20 6469 6374 203d   jrecord: dict =
-0000aa50: 2070 6172 7365 2872 6563 6f72 645b 7473   parse(record[ts
-0000aa60: 5f6c 656e 6774 683a 5d2c 207a 6970 7065  _length:], zippe
-0000aa70: 643d 5472 7565 290a 0a20 2020 2020 2020  d=True)..       
-0000aa80: 2020 2020 2066 6f72 2065 6e74 7279 2069       for entry i
-0000aa90: 6e20 6a72 6563 6f72 645b 2745 6e74 7269  n jrecord['Entri
-0000aaa0: 6573 275d 3a0a 2020 2020 2020 2020 2020  es']:.          
-0000aab0: 2020 2020 2020 2320 6461 7465 2066 6f72        # date for
-0000aac0: 6d61 7420 6973 2027 3230 3230 2d30 382d  mat is '2020-08-
-0000aad0: 3038 5430 393a 3435 3a30 332e 3036 3139  08T09:45:03.0619
-0000aae0: 3739 375a 2720 7769 7468 2061 2076 6172  797Z' with a var
-0000aaf0: 7969 6e67 0a20 2020 2020 2020 2020 2020  ying.           
-0000ab00: 2020 2020 2023 206e 756d 6265 7220 6f66       # number of
-0000ab10: 206d 696c 6c69 7365 636f 6e64 2064 6563   millisecond dec
-0000ab20: 696d 616c 2070 6f69 6e74 730a 2020 2020  imal points.    
-0000ab30: 2020 2020 2020 2020 2020 2020 2320 616c              # al
-0000ab40: 7761 7973 2072 656d 6f76 6520 6c61 7374  ways remove last
-0000ab50: 2063 6861 7220 2827 7a27 292c 206d 6178   char ('z'), max
-0000ab60: 206c 656e 2032 362c 2072 6967 6874 2070   len 26, right p
-0000ab70: 6164 2074 6f20 6c65 6e0a 2020 2020 2020  ad to len.      
-0000ab80: 2020 2020 2020 2020 2020 2320 3236 2077            # 26 w
-0000ab90: 6974 6820 7a65 726f 6573 2069 6620 7368  ith zeroes if sh
-0000aba0: 6f72 7465 720a 2020 2020 2020 2020 2020  orter.          
-0000abb0: 2020 2020 2020 6461 7465 203d 2074 6f5f        date = to_
-0000abc0: 6461 7465 7469 6d65 2865 6e74 7279 5b27  datetime(entry['
-0000abd0: 5574 6327 5d29 0a0a 2020 2020 2020 2020  Utc'])..        
-0000abe0: 2020 2020 2020 2020 666f 7220 6472 7620          for drv 
-0000abf0: 696e 2065 6e74 7279 5b27 4361 7273 275d  in entry['Cars']
-0000ac00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000ac10: 2020 2020 2020 6966 2064 7276 206e 6f74        if drv not
-0000ac20: 2069 6e20 6461 7461 3a0a 2020 2020 2020   in data:.      
-0000ac30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac40: 2020 2320 696e 6974 6961 6c69 7a65 2064    # initialize d
-0000ac50: 6963 7420 656e 7472 7920 666f 7220 7468  ict entry for th
-0000ac60: 6973 2064 7269 7665 720a 2020 2020 2020  is driver.      
+000099a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099b0: 2020 2020 2066 2264 6174 613a 207b 6b65       f"data: {ke
+000099c0: 797d 2229 0a0a 2020 2020 2020 2020 2020  y}")..          
+000099d0: 2020 2020 2020 2020 2020 6461 7461 5b27            data['
+000099e0: 5469 6d65 275d 5b2d 315d 203d 2074 696d  Time'][-1] = tim
+000099f0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00009a00: 2020 2020 2020 6461 7461 5b27 4472 6976        data['Driv
+00009a10: 6572 275d 5b2d 315d 203d 2064 7269 7665  er'][-1] = drive
+00009a20: 725f 6e75 6d62 6572 0a20 2020 2020 2020  r_number.       
+00009a30: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+00009a40: 615b 2753 7469 6e74 275d 5b2d 315d 203d  a['Stint'][-1] =
+00009a50: 2073 7469 6e74 5f6e 756d 6265 720a 0a20   stint_number.. 
+00009a60: 2020 2064 6620 3d20 7064 2e44 6174 6146     df = pd.DataF
+00009a70: 7261 6d65 2864 6174 6129 0a20 2020 2023  rame(data).    #
+00009a80: 2070 616e 6461 7320 646f 6573 6e27 7420   pandas doesn't 
+00009a90: 636f 7272 6563 746c 7920 696e 6665 7220  correctly infer 
+00009aa0: 626f 6f6c 2064 7479 7065 2063 6f6c 756d  bool dtype colum
+00009ab0: 6e73 2c20 7365 7420 7479 7065 2065 7870  ns, set type exp
+00009ac0: 6c69 6369 746c 790a 2020 2020 6466 5b5b  licitly.    df[[
+00009ad0: 274e 6577 272c 2027 5479 7265 734e 6f74  'New', 'TyresNot
+00009ae0: 4368 616e 6765 6427 5d5d 205c 0a20 2020  Changed']] \.   
+00009af0: 2020 2020 203d 2064 665b 5b27 4e65 7727       = df[['New'
+00009b00: 2c20 2754 7972 6573 4e6f 7443 6861 6e67  , 'TyresNotChang
+00009b10: 6564 275d 5d2e 6173 7479 7065 2862 6f6f  ed']].astype(boo
+00009b20: 6c29 0a20 2020 2072 6574 7572 6e20 6466  l).    return df
+00009b30: 0a0a 0a40 4361 6368 652e 6170 695f 7265  ...@Cache.api_re
+00009b40: 7175 6573 745f 7772 6170 7065 720a 6465  quest_wrapper.de
+00009b50: 6620 6361 725f 6461 7461 2870 6174 682c  f car_data(path,
+00009b60: 2072 6573 706f 6e73 653d 4e6f 6e65 2c20   response=None, 
+00009b70: 6c69 7665 6461 7461 3d4e 6f6e 6529 3a0a  livedata=None):.
+00009b80: 2020 2020 2222 220a 2020 2020 2e2e 2077      """.    .. w
+00009b90: 6172 6e69 6e67 3a3a 0a20 2020 2020 2020  arning::.       
+00009ba0: 203a 6d6f 643a 6066 6173 7466 312e 6170   :mod:`fastf1.ap
+00009bb0: 6960 2077 696c 6c20 6265 2063 6f6e 7369  i` will be consi
+00009bc0: 6465 7265 6420 7072 6976 6174 6520 696e  dered private in
+00009bd0: 2066 7574 7572 6520 7265 6c65 6173 6573   future releases
+00009be0: 2061 6e64 0a20 2020 2020 2020 2070 6f74   and.        pot
+00009bf0: 656e 7469 616c 6c79 2062 6520 7265 6d6f  entially be remo
+00009c00: 7665 6420 6f72 2063 6861 6e67 6564 2e0a  ved or changed..
+00009c10: 0a20 2020 2046 6574 6368 2061 6e64 2070  .    Fetch and p
+00009c20: 6172 7365 2063 6172 2064 6174 612e 0a0a  arse car data...
+00009c30: 2020 2020 4361 7220 6461 7461 2070 726f      Car data pro
+00009c40: 7669 6465 7320 7468 6520 666f 6c6c 6f77  vides the follow
+00009c50: 696e 6720 6461 7461 2063 6861 6e6e 656c  ing data channel
+00009c60: 7320 7065 7220 7361 6d70 6c65 3a0a 2020  s per sample:.  
+00009c70: 2020 2020 2020 2d20 5469 6d65 2028 7061        - Time (pa
+00009c80: 6e64 6173 2e54 696d 6564 656c 7461 293a  ndas.Timedelta):
+00009c90: 2073 6573 7369 6f6e 2074 696d 6573 7461   session timesta
+00009ca0: 6d70 2028 7469 6d65 206f 6e6c 7929 3b20  mp (time only); 
+00009cb0: 696e 6163 6375 7261 7465 2c20 6861 7320  inaccurate, has 
+00009cc0: 6475 706c 6963 6174 6520 7661 6c75 6573  duplicate values
+00009cd0: 3b20 7573 6520 4461 7465 2069 6e73 7465  ; use Date inste
+00009ce0: 6164 0a20 2020 2020 2020 202d 2044 6174  ad.        - Dat
+00009cf0: 6520 2870 616e 6461 732e 5469 6d65 7374  e (pandas.Timest
+00009d00: 616d 7029 3a20 7469 6d65 7374 616d 7020  amp): timestamp 
+00009d10: 666f 7220 7468 6973 2073 616d 706c 6520  for this sample 
+00009d20: 6173 2044 6174 6520 2b20 5469 6d65 3b20  as Date + Time; 
+00009d30: 6d6f 7265 206f 7220 6c65 7373 2065 7861  more or less exa
+00009d40: 6374 0a20 2020 2020 2020 202d 2053 7065  ct.        - Spe
+00009d50: 6564 2028 696e 7429 3a20 4b6d 2f68 0a20  ed (int): Km/h. 
+00009d60: 2020 2020 2020 202d 2052 504d 2028 696e         - RPM (in
+00009d70: 7429 0a20 2020 2020 2020 202d 2047 6561  t).        - Gea
+00009d80: 7220 2869 6e74 293a 205b 6361 6c6c 6564  r (int): [called
+00009d90: 2027 6e47 6561 7227 2069 6e20 7468 6520   'nGear' in the 
+00009da0: 6461 7461 215d 0a20 2020 2020 2020 202d  data!].        -
+00009db0: 2054 6872 6f74 746c 6520 2869 6e74 293a   Throttle (int):
+00009dc0: 2030 2d31 3030 250a 2020 2020 2020 2020   0-100%.        
+00009dd0: 2d20 4272 616b 6520 2862 6f6f 6c29 0a20  - Brake (bool). 
+00009de0: 2020 2020 2020 202d 2044 5253 2028 696e         - DRS (in
+00009df0: 7429 3a20 302d 3134 2028 4f64 6420 4452  t): 0-14 (Odd DR
+00009e00: 5320 6973 2044 6973 6162 6c65 642c 2045  S is Disabled, E
+00009e10: 7665 6e20 4452 5320 6973 2045 6e61 626c  ven DRS is Enabl
+00009e20: 6564 3f29 0a20 2020 2020 2020 2020 2028  ed?).          (
+00009e30: 4d6f 7265 2052 6573 6561 7263 6820 4e65  More Research Ne
+00009e40: 6564 6564 3f29 0a0a 2020 2020 2020 2020  eded?)..        
+00009e50: 2020 2d20 3020 3d20 204f 6666 0a20 2020    - 0 =  Off.   
+00009e60: 2020 2020 2020 202d 2031 203d 2020 4f66         - 1 =  Of
+00009e70: 660a 2020 2020 2020 2020 2020 2d20 3220  f.          - 2 
+00009e80: 3d20 2028 3f29 0a20 2020 2020 2020 2020  =  (?).         
+00009e90: 202d 2033 203d 2020 283f 290a 2020 2020   - 3 =  (?).    
+00009ea0: 2020 2020 2020 2d20 3820 3d20 2044 6574        - 8 =  Det
+00009eb0: 6563 7465 642c 2045 6c69 6769 626c 6520  ected, Eligible 
+00009ec0: 6f6e 6365 2069 6e20 4163 7469 7661 7469  once in Activati
+00009ed0: 6f6e 205a 6f6e 6520 284e 6f74 6564 2053  on Zone (Noted S
+00009ee0: 6f6d 6574 696d 6573 290a 2020 2020 2020  ometimes).      
+00009ef0: 2020 2020 2d20 3130 203d 204f 6e20 2855      - 10 = On (U
+00009f00: 6e6b 6e6f 776e 2044 6973 7469 6e63 7469  nknown Distincti
+00009f10: 6f6e 290a 2020 2020 2020 2020 2020 2d20  on).          - 
+00009f20: 3132 203d 204f 6e20 2855 6e6b 6e6f 776e  12 = On (Unknown
+00009f30: 2044 6973 7469 6e63 7469 6f6e 290a 2020   Distinction).  
+00009f40: 2020 2020 2020 2020 2d20 3134 203d 204f          - 14 = O
+00009f50: 6e20 2855 6e6b 6e6f 776e 2044 6973 7469  n (Unknown Disti
+00009f60: 6e63 7469 6f6e 290a 0a20 2020 2020 2020  nction)..       
+00009f70: 202d 2053 6f75 7263 6520 2873 7472 293a   - Source (str):
+00009f80: 2049 6e64 6963 6174 6573 2074 6865 2073   Indicates the s
+00009f90: 6f75 7263 6520 6f66 2061 2073 616d 706c  ource of a sampl
+00009fa0: 653b 2027 6361 7227 2066 6f72 2061 6c6c  e; 'car' for all
+00009fb0: 2076 616c 7565 7320 6865 7265 0a0a 2020   values here..  
+00009fc0: 2020 5468 6520 6461 7461 2073 7472 6561    The data strea
+00009fd0: 6d20 6861 7320 6120 7361 6d70 6c65 2072  m has a sample r
+00009fe0: 6174 6520 6f66 2028 7573 7561 6c6c 7929  ate of (usually)
+00009ff0: 2032 3430 6d73 2e20 5468 6520 7361 6d70   240ms. The samp
+0000a000: 6c65 7320 6672 6f6d 2074 6865 2064 6174  les from the dat
+0000a010: 6120 7374 7265 616d 7320 666f 7220 706f  a streams for po
+0000a020: 7369 7469 6f6e 2064 6174 6120 616e 640a  sition data and.
+0000a030: 2020 2020 6361 7220 6461 7461 2064 6f20      car data do 
+0000a040: 6e6f 7420 6c69 6e65 2075 702e 2052 6573  not line up. Res
+0000a050: 616d 706c 696e 672f 696e 7465 7270 6f6c  ampling/interpol
+0000a060: 6174 696f 6e20 6973 2072 6571 7569 7265  ation is require
+0000a070: 6420 746f 206d 6572 6765 2074 6865 6d2e  d to merge them.
+0000a080: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+0000a090: 2020 2020 7061 7468 2028 7374 7229 3a20      path (str): 
+0000a0a0: 6170 6920 7061 7468 2062 6173 6520 7374  api path base st
+0000a0b0: 7269 6e67 2028 7573 7561 6c6c 7920 6060  ring (usually ``
+0000a0c0: 5365 7373 696f 6e2e 6170 695f 7061 7468  Session.api_path
+0000a0d0: 6060 290a 2020 2020 2020 2020 7265 7370  ``).        resp
+0000a0e0: 6f6e 7365 3a20 5265 7370 6f6e 7365 2061  onse: Response a
+0000a0f0: 7320 7265 7475 726e 6564 2062 7920 3a66  s returned by :f
+0000a100: 756e 633a 6066 6574 6368 5f70 6167 6560  unc:`fetch_page`
+0000a110: 2063 616e 2062 6520 7061 7373 6564 2069   can be passed i
+0000a120: 6620 6974 2077 6173 2064 6f77 6e6c 6f61  f it was downloa
+0000a130: 6465 6420 616c 7265 6164 792e 0a20 2020  ded already..   
+0000a140: 2020 2020 206c 6976 6564 6174 613a 2041       livedata: A
+0000a150: 6e20 696e 7374 616e 6365 206f 6620 3a63  n instance of :c
+0000a160: 6c61 7373 3a60 6661 7374 6631 2e6c 6976  lass:`fastf1.liv
+0000a170: 6574 696d 696e 672e 6461 7461 2e4c 6976  etiming.data.Liv
+0000a180: 6554 696d 696e 6744 6174 6160 2074 6f20  eTimingData` to 
+0000a190: 7573 6520 6173 2061 2073 6f75 7263 6520  use as a source 
+0000a1a0: 696e 7374 6561 6420 6f66 2074 6865 2061  instead of the a
+0000a1b0: 7069 0a0a 2020 2020 5265 7475 726e 733a  pi..    Returns:
+0000a1c0: 0a20 2020 2020 2020 207c 2041 2064 6963  .        | A dic
+0000a1d0: 7469 6f6e 6172 7920 636f 6e74 6169 6e69  tionary containi
+0000a1e0: 6e67 206f 6e65 2070 616e 6461 7320 4461  ng one pandas Da
+0000a1f0: 7461 4672 616d 6520 7065 7220 6472 6976  taFrame per driv
+0000a200: 6572 2e20 4469 6374 696f 6e61 7279 206b  er. Dictionary k
+0000a210: 6579 7320 6172 6520 7468 6520 6472 6976  eys are the driv
+0000a220: 6572 2773 206e 756d 6265 7273 2061 730a  er's numbers as.
+0000a230: 2020 2020 2020 2020 2020 7374 7269 6e67            string
+0000a240: 2028 652e 672e 2027 3136 2729 2e20 596f   (e.g. '16'). Yo
+0000a250: 7520 7368 6f75 6c64 206e 6576 6572 2061  u should never a
+0000a260: 7373 756d 6520 7468 6174 2061 206e 756d  ssume that a num
+0000a270: 6265 7220 6578 6973 7473 210a 2020 2020  ber exists!.    
+0000a280: 2020 2020 7c20 4561 6368 2064 6174 6166      | Each dataf
+0000a290: 7261 6d65 2063 6f6e 7461 696e 7320 6f6e  rame contains on
+0000a2a0: 6520 636f 6c75 6d6e 2066 6f72 2065 6163  e column for eac
+0000a2b0: 6820 6461 7461 2063 6861 6e6e 656c 2061  h data channel a
+0000a2c0: 7320 6c69 7374 6564 2061 626f 7665 0a0a  s listed above..
+0000a2d0: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
+0000a2e0: 2020 2020 5365 7373 696f 6e4e 6f74 4176      SessionNotAv
+0000a2f0: 6169 6c61 626c 6545 7272 6f72 3a20 696e  ailableError: in
+0000a300: 2063 6173 6520 7468 6520 4631 206c 6976   case the F1 liv
+0000a310: 6574 696d 696e 6720 6170 6920 7265 7475  etiming api retu
+0000a320: 726e 7320 6e6f 2064 6174 610a 2020 2020  rns no data.    
+0000a330: 2222 220a 2020 2020 2320 6461 7461 2072  """.    # data r
+0000a340: 6563 6f72 6465 6420 6672 6f6d 206c 6976  ecorded from liv
+0000a350: 6520 7469 6d69 6e67 2068 6173 2061 2073  e timing has a s
+0000a360: 6c69 6768 746c 7920 6469 6666 6572 656e  lightly differen
+0000a370: 7420 7374 7275 6374 7572 650a 2020 2020  t structure.    
+0000a380: 6973 5f6c 6976 6564 6174 6120 3d20 4661  is_livedata = Fa
+0000a390: 6c73 6520 2023 2066 6c61 6720 746f 2069  lse  # flag to i
+0000a3a0: 6e64 6963 6174 6520 6c69 7665 2074 696d  ndicate live tim
+0000a3b0: 696e 6720 6461 7461 0a0a 2020 2020 6966  ing data..    if
+0000a3c0: 206c 6976 6564 6174 6120 6973 206e 6f74   livedata is not
+0000a3d0: 204e 6f6e 6520 616e 6420 6c69 7665 6461   None and liveda
+0000a3e0: 7461 2e68 6173 2827 4361 7244 6174 612e  ta.has('CarData.
+0000a3f0: 7a27 293a 0a20 2020 2020 2020 2072 6573  z'):.        res
+0000a400: 706f 6e73 6520 3d20 6c69 7665 6461 7461  ponse = livedata
+0000a410: 2e67 6574 2827 4361 7244 6174 612e 7a27  .get('CarData.z'
+0000a420: 290a 2020 2020 2020 2020 6973 5f6c 6976  ).        is_liv
+0000a430: 6564 6174 6120 3d20 5472 7565 0a20 2020  edata = True.   
+0000a440: 2065 6c69 6620 7265 7370 6f6e 7365 2069   elif response i
+0000a450: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+0000a460: 5f6c 6f67 6765 722e 696e 666f 2822 4665  _logger.info("Fe
+0000a470: 7463 6869 6e67 2063 6172 2064 6174 612e  tching car data.
+0000a480: 2e2e 2229 0a20 2020 2020 2020 2072 6573  ..").        res
+0000a490: 706f 6e73 6520 3d20 6665 7463 685f 7061  ponse = fetch_pa
+0000a4a0: 6765 2870 6174 682c 2027 6361 725f 6461  ge(path, 'car_da
+0000a4b0: 7461 2729 0a20 2020 2020 2020 2069 6620  ta').        if 
+0000a4c0: 7265 7370 6f6e 7365 2069 7320 4e6f 6e65  response is None
+0000a4d0: 3a20 2023 206e 6f20 7265 7370 6f6e 7365  :  # no response
+0000a4e0: 2072 6563 6569 7665 640a 2020 2020 2020   received.      
+0000a4f0: 2020 2020 2020 7261 6973 6520 5365 7373        raise Sess
+0000a500: 696f 6e4e 6f74 4176 6169 6c61 626c 6545  ionNotAvailableE
+0000a510: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+0000a520: 2020 2020 2020 224e 6f20 6461 7461 2066        "No data f
+0000a530: 6f72 2074 6869 7320 7365 7373 696f 6e21  or this session!
+0000a540: 2049 6620 7468 6973 2073 6573 7369 6f6e   If this session
+0000a550: 206f 6e6c 7920 6669 6e69 7368 6564 2022   only finished "
+0000a560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a570: 2022 7265 6365 6e74 6c79 2c20 706c 6561   "recently, plea
+0000a580: 7365 2074 7279 2061 6761 696e 2069 6e20  se try again in 
+0000a590: 6120 6665 7720 6d69 6e75 7465 732e 220a  a few minutes.".
+0000a5a0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+0000a5b0: 2020 205f 6c6f 6767 6572 2e69 6e66 6f28     _logger.info(
+0000a5c0: 2250 6172 7369 6e67 2063 6172 2064 6174  "Parsing car dat
+0000a5d0: 612e 2e2e 2229 0a0a 2020 2020 6e75 6d65  a...")..    nume
+0000a5e0: 7269 635f 6368 616e 6e65 6c73 203d 205b  ric_channels = [
+0000a5f0: 2752 504d 272c 2027 5370 6565 6427 2c20  'RPM', 'Speed', 
+0000a600: 276e 4765 6172 272c 2027 5468 726f 7474  'nGear', 'Thrott
+0000a610: 6c65 272c 2027 4452 5327 5d0a 2020 2020  le', 'DRS'].    
+0000a620: 626f 6f6c 5f63 6861 6e6e 656c 7320 3d20  bool_channels = 
+0000a630: 5b27 4272 616b 6527 5d0a 2020 2020 636f  ['Brake'].    co
+0000a640: 6c75 6d6e 7320 3d20 5b27 5469 6d65 272c  lumns = ['Time',
+0000a650: 2027 4461 7465 272c 2027 5250 4d27 2c20   'Date', 'RPM', 
+0000a660: 2753 7065 6564 272c 2027 6e47 6561 7227  'Speed', 'nGear'
+0000a670: 2c20 2754 6872 6f74 746c 6527 2c20 2742  , 'Throttle', 'B
+0000a680: 7261 6b65 272c 0a20 2020 2020 2020 2020  rake',.         
+0000a690: 2020 2020 2020 2744 5253 272c 2027 536f        'DRS', 'So
+0000a6a0: 7572 6365 275d 2020 2320 636f 7272 6563  urce']  # correc
+0000a6b0: 7420 6f72 6465 7220 7265 7175 6972 6564  t order required
+0000a6c0: 210a 0a20 2020 2074 735f 6c65 6e67 7468  !..    ts_length
+0000a6d0: 203d 2031 3220 2023 206c 656e 6774 6820   = 12  # length 
+0000a6e0: 6f66 2074 696d 6573 7461 6d70 3a20 6c65  of timestamp: le
+0000a6f0: 6e28 2730 303a 3030 3a30 303a 3030 3027  n('00:00:00:000'
+0000a700: 290a 0a20 2020 2064 6174 6120 3d20 6469  )..    data = di
+0000a710: 6374 2829 0a20 2020 2064 6563 6f64 655f  ct().    decode_
+0000a720: 6572 726f 725f 636f 756e 7420 3d20 300a  error_count = 0.
+0000a730: 0a20 2020 2066 6f72 2072 6563 6f72 6420  .    for record 
+0000a740: 696e 2072 6573 706f 6e73 653a 0a20 2020  in response:.   
+0000a750: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+0000a760: 2020 2020 2020 6966 2069 735f 6c69 7665        if is_live
+0000a770: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
+0000a780: 2020 2020 2020 7469 6d65 203d 2074 6f5f        time = to_
+0000a790: 7469 6d65 6465 6c74 6128 7265 636f 7264  timedelta(record
+0000a7a0: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
+0000a7b0: 2020 2020 206a 7265 636f 7264 3a20 6469       jrecord: di
+0000a7c0: 6374 203d 2070 6172 7365 2872 6563 6f72  ct = parse(recor
+0000a7d0: 645b 315d 2c20 7a69 7070 6564 3d54 7275  d[1], zipped=Tru
+0000a7e0: 6529 0a20 2020 2020 2020 2020 2020 2065  e).            e
+0000a7f0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000a800: 2020 2020 2074 696d 6520 3d20 746f 5f74       time = to_t
+0000a810: 696d 6564 656c 7461 2872 6563 6f72 645b  imedelta(record[
+0000a820: 3a74 735f 6c65 6e67 7468 5d29 0a20 2020  :ts_length]).   
+0000a830: 2020 2020 2020 2020 2020 2020 206a 7265               jre
+0000a840: 636f 7264 3a20 6469 6374 203d 2070 6172  cord: dict = par
+0000a850: 7365 2872 6563 6f72 645b 7473 5f6c 656e  se(record[ts_len
+0000a860: 6774 683a 5d2c 207a 6970 7065 643d 5472  gth:], zipped=Tr
+0000a870: 7565 290a 0a20 2020 2020 2020 2020 2020  ue)..           
+0000a880: 2066 6f72 2065 6e74 7279 2069 6e20 6a72   for entry in jr
+0000a890: 6563 6f72 645b 2745 6e74 7269 6573 275d  ecord['Entries']
+0000a8a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000a8b0: 2020 2320 6461 7465 2066 6f72 6d61 7420    # date format 
+0000a8c0: 6973 2027 3230 3230 2d30 382d 3038 5430  is '2020-08-08T0
+0000a8d0: 393a 3435 3a30 332e 3036 3139 3739 375a  9:45:03.0619797Z
+0000a8e0: 2720 7769 7468 2061 2076 6172 7969 6e67  ' with a varying
+0000a8f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a900: 2023 206e 756d 6265 7220 6f66 206d 696c   # number of mil
+0000a910: 6c69 7365 636f 6e64 2064 6563 696d 616c  lisecond decimal
+0000a920: 2070 6f69 6e74 730a 2020 2020 2020 2020   points.        
+0000a930: 2020 2020 2020 2020 2320 616c 7761 7973          # always
+0000a940: 2072 656d 6f76 6520 6c61 7374 2063 6861   remove last cha
+0000a950: 7220 2827 7a27 292c 206d 6178 206c 656e  r ('z'), max len
+0000a960: 2032 362c 2072 6967 6874 2070 6164 2074   26, right pad t
+0000a970: 6f20 6c65 6e0a 2020 2020 2020 2020 2020  o len.          
+0000a980: 2020 2020 2020 2320 3236 2077 6974 6820        # 26 with 
+0000a990: 7a65 726f 6573 2069 6620 7368 6f72 7465  zeroes if shorte
+0000a9a0: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+0000a9b0: 2020 6461 7465 203d 2074 6f5f 6461 7465    date = to_date
+0000a9c0: 7469 6d65 2865 6e74 7279 5b27 5574 6327  time(entry['Utc'
+0000a9d0: 5d29 0a0a 2020 2020 2020 2020 2020 2020  ])..            
+0000a9e0: 2020 2020 666f 7220 6472 7620 696e 2065      for drv in e
+0000a9f0: 6e74 7279 5b27 4361 7273 275d 3a0a 2020  ntry['Cars']:.  
+0000aa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa10: 2020 6966 2064 7276 206e 6f74 2069 6e20    if drv not in 
+0000aa20: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
+0000aa30: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000aa40: 696e 6974 6961 6c69 7a65 2064 6963 7420  initialize dict 
+0000aa50: 656e 7472 7920 666f 7220 7468 6973 2064  entry for this d
+0000aa60: 7269 7665 720a 2020 2020 2020 2020 2020  river.          
+0000aa70: 2020 2020 2020 2020 2020 2020 2020 6461                da
+0000aa80: 7461 5b64 7276 5d20 3d20 6c69 7374 2829  ta[drv] = list()
+0000aa90: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000aaa0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+0000aab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aac0: 2020 2072 706d 203d 2065 6e74 7279 5b27     rpm = entry['
+0000aad0: 4361 7273 275d 5b64 7276 5d5b 2743 6861  Cars'][drv]['Cha
+0000aae0: 6e6e 656c 7327 5d5b 2730 275d 0a20 2020  nnels']['0'].   
+0000aaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab00: 2020 2020 2073 7065 6564 203d 2065 6e74       speed = ent
+0000ab10: 7279 5b27 4361 7273 275d 5b64 7276 5d5b  ry['Cars'][drv][
+0000ab20: 2743 6861 6e6e 656c 7327 5d5b 2732 275d  'Channels']['2']
+0000ab30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ab40: 2020 2020 2020 2020 206e 6765 6172 203d           ngear =
+0000ab50: 2065 6e74 7279 5b27 4361 7273 275d 5b64   entry['Cars'][d
+0000ab60: 7276 5d5b 2743 6861 6e6e 656c 7327 5d5b  rv]['Channels'][
+0000ab70: 2733 275d 0a20 2020 2020 2020 2020 2020  '3'].           
+0000ab80: 2020 2020 2020 2020 2020 2020 2074 6872               thr
+0000ab90: 6f74 746c 6520 3d20 656e 7472 795b 2743  ottle = entry['C
+0000aba0: 6172 7327 5d5b 6472 765d 5b27 4368 616e  ars'][drv]['Chan
+0000abb0: 6e65 6c73 275d 5b27 3427 5d0a 2020 2020  nels']['4'].    
+0000abc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abd0: 2020 2020 6272 616b 6520 3d20 656e 7472      brake = entr
+0000abe0: 795b 2743 6172 7327 5d5b 6472 765d 5b27  y['Cars'][drv]['
+0000abf0: 4368 616e 6e65 6c73 275d 5b27 3527 5d0a  Channels']['5'].
+0000ac00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac10: 2020 2020 2020 2020 6472 7320 3d20 656e          drs = en
+0000ac20: 7472 795b 2743 6172 7327 5d5b 6472 765d  try['Cars'][drv]
+0000ac30: 5b27 4368 616e 6e65 6c73 275d 5b27 3435  ['Channels']['45
+0000ac40: 275d 0a0a 2020 2020 2020 2020 2020 2020  ']..            
+0000ac50: 2020 2020 2020 2020 6578 6365 7074 204b          except K
+0000ac60: 6579 4572 726f 723a 0a20 2020 2020 2020  eyError:.       
 0000ac70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac80: 2020 6461 7461 5b64 7276 5d20 3d20 6c69    data[drv] = li
-0000ac90: 7374 2829 0a0a 2020 2020 2020 2020 2020  st()..          
-0000aca0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
-0000acb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000acc0: 2020 2020 2020 2072 706d 203d 2065 6e74         rpm = ent
-0000acd0: 7279 5b27 4361 7273 275d 5b64 7276 5d5b  ry['Cars'][drv][
-0000ace0: 2743 6861 6e6e 656c 7327 5d5b 2730 275d  'Channels']['0']
-0000acf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ad00: 2020 2020 2020 2020 2073 7065 6564 203d           speed =
-0000ad10: 2065 6e74 7279 5b27 4361 7273 275d 5b64   entry['Cars'][d
-0000ad20: 7276 5d5b 2743 6861 6e6e 656c 7327 5d5b  rv]['Channels'][
-0000ad30: 2732 275d 0a20 2020 2020 2020 2020 2020  '2'].           
-0000ad40: 2020 2020 2020 2020 2020 2020 206e 6765               nge
-0000ad50: 6172 203d 2065 6e74 7279 5b27 4361 7273  ar = entry['Cars
-0000ad60: 275d 5b64 7276 5d5b 2743 6861 6e6e 656c  '][drv]['Channel
-0000ad70: 7327 5d5b 2733 275d 0a20 2020 2020 2020  s']['3'].       
-0000ad80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad90: 2074 6872 6f74 746c 6520 3d20 656e 7472   throttle = entr
-0000ada0: 795b 2743 6172 7327 5d5b 6472 765d 5b27  y['Cars'][drv]['
-0000adb0: 4368 616e 6e65 6c73 275d 5b27 3427 5d0a  Channels']['4'].
-0000adc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000add0: 2020 2020 2020 2020 6272 616b 6520 3d20          brake = 
-0000ade0: 656e 7472 795b 2743 6172 7327 5d5b 6472  entry['Cars'][dr
-0000adf0: 765d 5b27 4368 616e 6e65 6c73 275d 5b27  v]['Channels']['
-0000ae00: 3527 5d0a 2020 2020 2020 2020 2020 2020  5'].            
-0000ae10: 2020 2020 2020 2020 2020 2020 6472 7320              drs 
-0000ae20: 3d20 656e 7472 795b 2743 6172 7327 5d5b  = entry['Cars'][
-0000ae30: 6472 765d 5b27 4368 616e 6e65 6c73 275d  drv]['Channels']
-0000ae40: 5b27 3435 275d 0a0a 2020 2020 2020 2020  ['45']..        
-0000ae50: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-0000ae60: 7074 204b 6579 4572 726f 723a 0a20 2020  pt KeyError:.   
-0000ae70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae80: 2020 2020 2063 6f6e 7469 6e75 650a 0a20       continue.. 
-0000ae90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aea0: 2020 2064 6174 615b 6472 765d 2e61 7070     data[drv].app
-0000aeb0: 656e 6428 2874 696d 652c 2064 6174 652c  end((time, date,
-0000aec0: 2072 706d 2c20 7370 6565 642c 206e 6765   rpm, speed, nge
-0000aed0: 6172 2c20 7468 726f 7474 6c65 2c0a 2020  ar, throttle,.  
-0000aee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af00: 2020 2020 6272 616b 652c 2064 7273 2c20      brake, drs, 
-0000af10: 2763 6172 2729 290a 0a20 2020 2020 2020  'car'))..       
-0000af20: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-0000af30: 6e3a 0a20 2020 2020 2020 2020 2020 2023  n:.            #
-0000af40: 2074 6f6f 2072 6973 6b79 2074 6f20 7370   too risky to sp
-0000af50: 6563 6966 7920 616e 2065 7863 6570 7469  ecify an excepti
-0000af60: 6f6e 3a20 756e 6578 7065 6374 6564 2069  on: unexpected i
-0000af70: 6e76 616c 6964 2064 6174 6121 0a20 2020  nvalid data!.   
-0000af80: 2020 2020 2020 2020 2064 6563 6f64 655f           decode_
-0000af90: 6572 726f 725f 636f 756e 7420 2b3d 2031  error_count += 1
-0000afa0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-0000afb0: 7469 6e75 650a 0a20 2020 2069 6620 6465  tinue..    if de
-0000afc0: 636f 6465 5f65 7272 6f72 5f63 6f75 6e74  code_error_count
-0000afd0: 203e 2030 3a0a 2020 2020 2020 2020 5f6c   > 0:.        _l
-0000afe0: 6f67 6765 722e 7761 726e 696e 6728 6622  ogger.warning(f"
-0000aff0: 4361 7220 6461 7461 3a20 6661 696c 6564  Car data: failed
-0000b000: 2074 6f20 6465 636f 6465 207b 6465 636f   to decode {deco
-0000b010: 6465 5f65 7272 6f72 5f63 6f75 6e74 7d20  de_error_count} 
-0000b020: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000b030: 2020 2020 2020 2020 2020 6622 6d65 7373            f"mess
-0000b040: 6167 6573 2028 7b6c 656e 2872 6573 706f  ages ({len(respo
-0000b050: 6e73 6529 7d20 6d65 7373 6167 6573 2074  nse)} messages t
-0000b060: 6f74 616c 2922 290a 0a20 2020 2023 2063  otal)")..    # c
-0000b070: 7265 6174 6520 6f6e 6520 6461 7461 6672  reate one datafr
-0000b080: 616d 6520 7065 7220 6472 6976 6572 2061  ame per driver a
-0000b090: 6e64 2063 6865 636b 2066 6f72 2074 6865  nd check for the
-0000b0a0: 206c 6f6e 6765 7374 2064 6174 6166 7261   longest datafra
-0000b0b0: 6d65 0a20 2020 206d 6f73 745f 636f 6d70  me.    most_comp
-0000b0c0: 6c65 7465 5f72 6566 203d 204e 6f6e 650a  lete_ref = None.
-0000b0d0: 2020 2020 666f 7220 6472 7620 696e 2064      for drv in d
-0000b0e0: 6174 613a 0a20 2020 2020 2020 2061 7272  ata:.        arr
-0000b0f0: 5f61 6c6c 203d 206e 702e 6172 7261 7928  _all = np.array(
-0000b100: 6461 7461 5b64 7276 5d29 0a20 2020 2020  data[drv]).     
-0000b110: 2020 2074 696d 6520 3d20 6172 725f 616c     time = arr_al
-0000b120: 6c5b 3a2c 2030 5d2e 6173 7479 7065 2827  l[:, 0].astype('
-0000b130: 7469 6d65 6465 6c74 6136 345b 6e73 5d27  timedelta64[ns]'
-0000b140: 290a 2020 2020 2020 2020 6461 7465 203d  ).        date =
-0000b150: 2061 7272 5f61 6c6c 5b3a 2c20 315d 2e61   arr_all[:, 1].a
-0000b160: 7374 7970 6528 2764 6174 6574 696d 6536  stype('datetime6
-0000b170: 345b 6e73 5d27 290a 2020 2020 2020 2020  4[ns]').        
-0000b180: 7270 6d20 3d20 6172 725f 616c 6c5b 3a2c  rpm = arr_all[:,
-0000b190: 2032 5d2e 6173 7479 7065 2827 696e 7436   2].astype('int6
-0000b1a0: 3427 290a 2020 2020 2020 2020 7370 6565  4').        spee
-0000b1b0: 6420 3d20 6172 725f 616c 6c5b 3a2c 2033  d = arr_all[:, 3
-0000b1c0: 5d2e 6173 7479 7065 2827 696e 7436 3427  ].astype('int64'
-0000b1d0: 290a 2020 2020 2020 2020 6e67 6561 7220  ).        ngear 
-0000b1e0: 3d20 6172 725f 616c 6c5b 3a2c 2034 5d2e  = arr_all[:, 4].
-0000b1f0: 6173 7479 7065 2827 696e 7436 3427 290a  astype('int64').
-0000b200: 2020 2020 2020 2020 7468 726f 7474 6c65          throttle
-0000b210: 203d 2061 7272 5f61 6c6c 5b3a 2c20 355d   = arr_all[:, 5]
-0000b220: 2e61 7374 7970 6528 2769 6e74 3634 2729  .astype('int64')
-0000b230: 0a20 2020 2020 2020 2062 7261 6b65 203d  .        brake =
-0000b240: 2061 7272 5f61 6c6c 5b3a 2c20 365d 2e61   arr_all[:, 6].a
-0000b250: 7374 7970 6528 2769 6e74 3634 2729 2020  stype('int64')  
-0000b260: 2320 636f 6e76 6572 7465 6420 746f 2062  # converted to b
-0000b270: 6f6f 6c20 6c61 7465 720a 2020 2020 2020  ool later.      
-0000b280: 2020 6472 7320 3d20 6172 725f 616c 6c5b    drs = arr_all[
-0000b290: 3a2c 2037 5d2e 6173 7479 7065 2827 696e  :, 7].astype('in
-0000b2a0: 7436 3427 290a 2020 2020 2020 2020 736f  t64').        so
-0000b2b0: 7572 6365 203d 2061 7272 5f61 6c6c 5b3a  urce = arr_all[:
-0000b2c0: 2c20 385d 2e61 7374 7970 6528 276f 626a  , 8].astype('obj
-0000b2d0: 6563 7427 290a 0a20 2020 2020 2020 2064  ect')..        d
-0000b2e0: 6174 615b 6472 765d 203d 2063 7265 6174  ata[drv] = creat
-0000b2f0: 655f 6466 5f66 6173 7428 0a20 2020 2020  e_df_fast(.     
-0000b300: 2020 2020 2020 2061 7272 6179 733d 5b74         arrays=[t
-0000b310: 696d 652c 2064 6174 652c 0a20 2020 2020  ime, date,.     
-0000b320: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000b330: 706d 2c20 7370 6565 642c 206e 6765 6172  pm, speed, ngear
-0000b340: 2c20 7468 726f 7474 6c65 2c20 6272 616b  , throttle, brak
-0000b350: 652c 2064 7273 2c20 736f 7572 6365 5d2c  e, drs, source],
-0000b360: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
-0000b370: 756d 6e73 3d63 6f6c 756d 6e73 0a20 2020  umns=columns.   
-0000b380: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0000b390: 6966 2028 6d6f 7374 5f63 6f6d 706c 6574  if (most_complet
-0000b3a0: 655f 7265 6620 6973 204e 6f6e 6529 205c  e_ref is None) \
-0000b3b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b3c0: 206f 7220 286c 656e 2864 6174 615b 6472   or (len(data[dr
-0000b3d0: 765d 5b27 4461 7465 275d 2920 3e20 6c65  v]['Date']) > le
-0000b3e0: 6e28 6d6f 7374 5f63 6f6d 706c 6574 655f  n(most_complete_
-0000b3f0: 7265 6629 293a 0a20 2020 2020 2020 2020  ref)):.         
-0000b400: 2020 206d 6f73 745f 636f 6d70 6c65 7465     most_complete
-0000b410: 5f72 6566 203d 2064 6174 615b 6472 765d  _ref = data[drv]
-0000b420: 5b27 4461 7465 275d 0a0a 2020 2020 666f  ['Date']..    fo
-0000b430: 7220 6472 7620 696e 2064 6174 613a 0a20  r drv in data:. 
-0000b440: 2020 2020 2020 2023 2069 6620 6576 6572         # if ever
-0000b450: 7974 6869 6e67 2069 7320 7765 6c6c 2c20  ything is well, 
-0000b460: 616c 6c20 6461 7461 6672 616d 6573 2073  all dataframes s
-0000b470: 686f 756c 6420 6861 7665 2074 6865 2073  hould have the s
-0000b480: 616d 6520 6c65 6e67 7468 0a20 2020 2020  ame length.     
-0000b490: 2020 2023 2061 6e64 206e 6f20 706f 7374     # and no post
-0000b4a0: 7072 6f63 6573 7369 6e67 2069 7320 6e65  processing is ne
-0000b4b0: 6365 7373 6172 790a 2020 2020 2020 2020  cessary.        
-0000b4c0: 6966 206c 656e 2864 6174 615b 6472 765d  if len(data[drv]
-0000b4d0: 5b27 4461 7465 275d 2920 3c20 6c65 6e28  ['Date']) < len(
-0000b4e0: 6d6f 7374 5f63 6f6d 706c 6574 655f 7265  most_complete_re
-0000b4f0: 6629 3a0a 2020 2020 2020 2020 2020 2020  f):.            
-0000b500: 2320 7468 6572 6520 6973 206d 6973 7369  # there is missi
-0000b510: 6e67 2064 6174 6120 666f 7220 7468 6973  ng data for this
-0000b520: 2064 7269 7665 720a 2020 2020 2020 2020   driver.        
-0000b530: 2020 2020 2320 6578 7465 6e64 2074 6865      # extend the
-0000b540: 2044 6174 6520 636f 6c75 6d6e 2061 6e64   Date column and
-0000b550: 2066 696c 6c20 7570 206d 6973 7369 6e67   fill up missing
-0000b560: 2074 656c 656d 6574 7279 2076 616c 7565   telemetry value
-0000b570: 7320 7769 7468 0a20 2020 2020 2020 2020  s with.         
-0000b580: 2020 2023 207a 6572 6f2c 2065 7863 6570     # zero, excep
-0000b590: 7420 5469 6d65 2077 6869 6368 2069 7320  t Time which is 
-0000b5a0: 6c65 6674 2061 7320 4e61 5420 616e 6420  left as NaT and 
-0000b5b0: 7769 6c6c 2062 6520 6361 6c63 756c 6174  will be calculat
-0000b5c0: 6564 0a20 2020 2020 2020 2020 2020 2023  ed.            #
-0000b5d0: 2063 6f72 7265 6374 6c79 2062 6173 6564   correctly based
-0000b5e0: 206f 6e20 5365 7373 696f 6e2e 7430 5f64   on Session.t0_d
-0000b5f0: 6174 6520 616e 7977 6179 2077 6865 6e20  ate anyway when 
-0000b600: 6372 6561 7469 6e67 2054 656c 656d 6574  creating Telemet
-0000b610: 7279 0a20 2020 2020 2020 2020 2020 2023  ry.            #
-0000b620: 2069 6e73 7461 6e63 6573 2069 6e20 5365   instances in Se
-0000b630: 7373 696f 6e2e 6c6f 6164 5f74 656c 656d  ssion.load_telem
-0000b640: 6574 7279 0a20 2020 2020 2020 2020 2020  etry.           
-0000b650: 2064 6174 615b 6472 765d 203d 2064 6174   data[drv] = dat
-0000b660: 615b 6472 765d 205c 0a20 2020 2020 2020  a[drv] \.       
-0000b670: 2020 2020 2020 2020 202e 6d65 7267 6528           .merge(
-0000b680: 6d6f 7374 5f63 6f6d 706c 6574 655f 7265  most_complete_re
-0000b690: 662c 2068 6f77 3d27 6f75 7465 7227 2920  f, how='outer') 
-0000b6a0: 5c0a 2020 2020 2020 2020 2020 2020 2020  \.              
-0000b6b0: 2020 2e73 6f72 745f 7661 6c75 6573 2862    .sort_values(b
-0000b6c0: 793d 2744 6174 6527 2920 5c0a 2020 2020  y='Date') \.    
-0000b6d0: 2020 2020 2020 2020 2020 2020 2e72 6573              .res
-0000b6e0: 6574 5f69 6e64 6578 2864 726f 703d 5472  et_index(drop=Tr
-0000b6f0: 7565 290a 0a20 2020 2020 2020 2020 2020  ue)..           
-0000b700: 205f 6c6f 6767 6572 2e77 6172 6e69 6e67   _logger.warning
-0000b710: 2866 2244 7269 7665 7220 7b64 7276 3a20  (f"Driver {drv: 
-0000b720: 3e32 7d3a 2043 6172 2064 6174 6120 6973  >2}: Car data is
-0000b730: 2069 6e63 6f6d 706c 6574 6521 2229 0a0a   incomplete!")..
-0000b740: 2020 2020 2020 2020 2320 656e 7375 7265          # ensure
-0000b750: 2074 6861 7420 6272 616b 6520 6461 7461   that brake data
-0000b760: 2069 7320 2762 6f6f 6c65 616e 2d63 6f6d   is 'boolean-com
-0000b770: 7061 7469 626c 6527 2069 6e20 6361 7365  patible' in case
-0000b780: 2074 6861 7420 7468 6973 2069 730a 2020   that this is.  
-0000b790: 2020 2020 2020 2320 6576 6572 2063 6861        # ever cha
-0000b7a0: 6e67 6564 0a20 2020 2020 2020 205f 756e  nged.        _un
-0000b7b0: 6971 7565 5f62 7261 6b65 5f76 616c 7565  ique_brake_value
-0000b7c0: 7320 3d20 6461 7461 5b64 7276 5d2e 6c6f  s = data[drv].lo
-0000b7d0: 635b 3a2c 2027 4272 616b 6527 5d2e 756e  c[:, 'Brake'].un
-0000b7e0: 6971 7565 2829 0a20 2020 2020 2020 2069  ique().        i
-0000b7f0: 6620 2828 5f75 6e69 7175 655f 6272 616b  f ((_unique_brak
-0000b800: 655f 7661 6c75 6573 203e 2030 2920 2620  e_values > 0) & 
-0000b810: 285f 756e 6971 7565 5f62 7261 6b65 5f76  (_unique_brake_v
-0000b820: 616c 7565 7320 3c20 3130 3029 292e 616e  alues < 100)).an
-0000b830: 7928 293a 0a20 2020 2020 2020 2020 2020  y():.           
-0000b840: 205f 6c6f 6767 6572 2e77 6172 6e69 6e67   _logger.warning
-0000b850: 2866 2244 7269 7665 7220 7b64 7276 3a20  (f"Driver {drv: 
-0000b860: 3e32 7d3a 2052 6177 2062 7261 6b65 2064  >2}: Raw brake d
-0000b870: 6174 6120 636f 6e74 6169 6e73 2022 0a20  ata contains ". 
-0000b880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b890: 2020 2020 2020 2020 2020 2066 226e 6f6e             f"non
-0000b8a0: 2d62 6f6f 6c65 616e 2076 616c 7565 7321  -boolean values!
-0000b8b0: 2229 0a0a 2020 2020 2020 2020 2320 636f  ")..        # co
-0000b8c0: 6e76 6572 7420 746f 2063 6f72 7265 6374  nvert to correct
-0000b8d0: 2064 6174 6174 7970 6573 0a20 2020 2020   datatypes.     
-0000b8e0: 2020 2064 6174 615b 6472 765d 5b6e 756d     data[drv][num
-0000b8f0: 6572 6963 5f63 6861 6e6e 656c 735d 203d  eric_channels] =
-0000b900: 205c 0a20 2020 2020 2020 2020 2020 2064   \.            d
-0000b910: 6174 615b 6472 765d 2e6c 6f63 5b3a 2c20  ata[drv].loc[:, 
-0000b920: 6e75 6d65 7269 635f 6368 616e 6e65 6c73  numeric_channels
-0000b930: 5d20 5c0a 2020 2020 2020 2020 2020 2020  ] \.            
-0000b940: 2e66 696c 6c6e 6128 7661 6c75 653d 302c  .fillna(value=0,
-0000b950: 2069 6e70 6c61 6365 3d46 616c 7365 2920   inplace=False) 
-0000b960: 5c0a 2020 2020 2020 2020 2020 2020 2e61  \.            .a
-0000b970: 7374 7970 6528 2769 6e74 3634 2729 0a0a  stype('int64')..
-0000b980: 2020 2020 2020 2020 6461 7461 5b64 7276          data[drv
-0000b990: 5d5b 626f 6f6c 5f63 6861 6e6e 656c 735d  ][bool_channels]
-0000b9a0: 203d 205c 0a20 2020 2020 2020 2020 2020   = \.           
-0000b9b0: 2064 6174 615b 6472 765d 2e6c 6f63 5b3a   data[drv].loc[:
-0000b9c0: 2c20 626f 6f6c 5f63 6861 6e6e 656c 735d  , bool_channels]
-0000b9d0: 205c 0a20 2020 2020 2020 2020 2020 202e   \.            .
-0000b9e0: 6669 6c6c 6e61 2876 616c 7565 3d46 616c  fillna(value=Fal
-0000b9f0: 7365 2c20 696e 706c 6163 653d 4661 6c73  se, inplace=Fals
-0000ba00: 6529 205c 0a20 2020 2020 2020 2020 2020  e) \.           
-0000ba10: 202e 6173 7479 7065 2827 626f 6f6c 2729   .astype('bool')
-0000ba20: 0a0a 2020 2020 7265 7475 726e 2064 6174  ..    return dat
-0000ba30: 610a 0a0a 4043 6163 6865 2e61 7069 5f72  a...@Cache.api_r
-0000ba40: 6571 7565 7374 5f77 7261 7070 6572 0a64  equest_wrapper.d
-0000ba50: 6566 2070 6f73 6974 696f 6e5f 6461 7461  ef position_data
-0000ba60: 2870 6174 682c 2072 6573 706f 6e73 653d  (path, response=
-0000ba70: 4e6f 6e65 2c20 6c69 7665 6461 7461 3d4e  None, livedata=N
-0000ba80: 6f6e 6529 3a0a 2020 2020 2222 220a 2020  one):.    """.  
-0000ba90: 2020 2e2e 2077 6172 6e69 6e67 3a3a 0a20    .. warning::. 
-0000baa0: 2020 2020 2020 203a 6d6f 643a 6066 6173         :mod:`fas
-0000bab0: 7466 312e 6170 6960 2077 696c 6c20 6265  tf1.api` will be
-0000bac0: 2063 6f6e 7369 6465 7265 6420 7072 6976   considered priv
-0000bad0: 6174 6520 696e 2066 7574 7572 6520 7265  ate in future re
-0000bae0: 6c65 6173 6573 2061 6e64 0a20 2020 2020  leases and.     
-0000baf0: 2020 2070 6f74 656e 7469 616c 6c79 2062     potentially b
-0000bb00: 6520 7265 6d6f 7665 6420 6f72 2063 6861  e removed or cha
-0000bb10: 6e67 6564 2e0a 0a20 2020 2046 6574 6368  nged...    Fetch
-0000bb20: 2061 6e64 2070 6172 7365 2070 6f73 6974   and parse posit
-0000bb30: 696f 6e20 6461 7461 2e0a 0a20 2020 2050  ion data...    P
-0000bb40: 6f73 6974 696f 6e20 6461 7461 2070 726f  osition data pro
-0000bb50: 7669 6465 7320 7468 6520 666f 6c6c 6f77  vides the follow
-0000bb60: 696e 6720 6461 7461 2063 6861 6e6e 656c  ing data channel
-0000bb70: 7320 7065 7220 7361 6d70 6c65 3a0a 2020  s per sample:.  
-0000bb80: 2020 2020 2020 2d20 5469 6d65 2028 7061        - Time (pa
-0000bb90: 6e64 6173 2e54 696d 6564 656c 7461 293a  ndas.Timedelta):
-0000bba0: 2073 6573 7369 6f6e 2074 696d 6573 7461   session timesta
-0000bbb0: 6d70 2028 7469 6d65 206f 6e6c 7929 3b20  mp (time only); 
-0000bbc0: 696e 6163 6375 7261 7465 2c20 6861 7320  inaccurate, has 
-0000bbd0: 6475 706c 6963 6174 6520 7661 6c75 6573  duplicate values
-0000bbe0: 3b20 7573 6520 4461 7465 2069 6e73 7465  ; use Date inste
-0000bbf0: 6164 0a20 2020 2020 2020 202d 2044 6174  ad.        - Dat
-0000bc00: 6520 2870 616e 6461 732e 5469 6d65 7374  e (pandas.Timest
-0000bc10: 616d 7029 3a20 7469 6d65 7374 616d 7020  amp): timestamp 
-0000bc20: 666f 7220 7468 6973 2073 616d 706c 6520  for this sample 
-0000bc30: 6173 2044 6174 6520 2b20 5469 6d65 3b20  as Date + Time; 
-0000bc40: 6d6f 7265 206f 7220 6c65 7373 2065 7861  more or less exa
-0000bc50: 6374 0a20 2020 2020 2020 202d 2053 7461  ct.        - Sta
-0000bc60: 7475 7320 2873 7472 293a 2027 4f6e 5472  tus (str): 'OnTr
-0000bc70: 6163 6b27 206f 7220 274f 6666 5472 6163  ack' or 'OffTrac
-0000bc80: 6b27 0a20 2020 2020 2020 202d 2058 2c20  k'.        - X, 
-0000bc90: 592c 205a 2028 696e 7429 3a20 506f 7369  Y, Z (int): Posi
-0000bca0: 7469 6f6e 2063 6f6f 7264 696e 6174 6573  tion coordinates
-0000bcb0: 3b20 7374 6172 7469 6e67 2066 726f 6d20  ; starting from 
-0000bcc0: 3230 3230 2074 6865 2063 6f6f 7264 696e  2020 the coordin
-0000bcd0: 6174 6573 2061 7265 2067 6976 656e 2069  ates are given i
-0000bce0: 6e20 312f 3130 206d 6574 6572 0a20 2020  n 1/10 meter.   
-0000bcf0: 2020 2020 202d 2053 6f75 7263 6520 2873       - Source (s
-0000bd00: 7472 293a 2049 6e64 6963 6174 6573 2074  tr): Indicates t
-0000bd10: 6865 2073 6f75 7263 6520 6f66 2061 2073  he source of a s
-0000bd20: 616d 706c 653b 2027 706f 7327 2066 6f72  ample; 'pos' for
-0000bd30: 2061 6c6c 2076 616c 7565 7320 6865 7265   all values here
-0000bd40: 0a0a 2020 2020 5468 6520 6461 7461 2073  ..    The data s
-0000bd50: 7472 6561 6d20 6861 7320 6120 7361 6d70  tream has a samp
-0000bd60: 6c65 2072 6174 6520 6f66 2028 7573 7561  le rate of (usua
-0000bd70: 6c6c 7929 2032 3230 6d73 2e20 5468 6520  lly) 220ms. The 
-0000bd80: 7361 6d70 6c65 7320 6672 6f6d 2074 6865  samples from the
-0000bd90: 2064 6174 6120 7374 7265 616d 7320 666f   data streams fo
-0000bda0: 7220 706f 7369 7469 6f6e 2064 6174 6120  r position data 
-0000bdb0: 616e 640a 2020 2020 6361 7220 6461 7461  and.    car data
-0000bdc0: 2064 6f20 6e6f 7420 6c69 6e65 2075 702e   do not line up.
-0000bdd0: 2052 6573 616d 706c 696e 672f 696e 7465   Resampling/inte
-0000bde0: 7270 6f6c 6174 696f 6e20 6973 2072 6571  rpolation is req
-0000bdf0: 7569 7265 6420 746f 206d 6572 6765 2074  uired to merge t
-0000be00: 6865 6d2e 0a0a 2020 2020 4172 6773 3a0a  hem...    Args:.
-0000be10: 2020 2020 2020 2020 7061 7468 2028 7374          path (st
-0000be20: 7229 3a20 6170 6920 7061 7468 2062 6173  r): api path bas
-0000be30: 6520 7374 7269 6e67 2028 7573 7561 6c6c  e string (usuall
-0000be40: 7920 6060 5365 7373 696f 6e2e 6170 695f  y ``Session.api_
-0000be50: 7061 7468 6060 290a 2020 2020 2020 2020  path``).        
-0000be60: 7265 7370 6f6e 7365 3a20 5265 7370 6f6e  response: Respon
-0000be70: 7365 2061 7320 7265 7475 726e 6564 2062  se as returned b
-0000be80: 7920 3a66 756e 633a 6066 6574 6368 5f70  y :func:`fetch_p
-0000be90: 6167 6560 2063 616e 2062 6520 7061 7373  age` can be pass
-0000bea0: 6564 2069 6620 6974 2077 6173 2064 6f77  ed if it was dow
-0000beb0: 6e6c 6f61 6465 6420 616c 7265 6164 792e  nloaded already.
-0000bec0: 0a20 2020 2020 2020 206c 6976 6564 6174  .        livedat
-0000bed0: 613a 2041 6e20 696e 7374 616e 6365 206f  a: An instance o
-0000bee0: 6620 3a63 6c61 7373 3a60 6661 7374 6631  f :class:`fastf1
-0000bef0: 2e6c 6976 6574 696d 696e 672e 6461 7461  .livetiming.data
-0000bf00: 2e4c 6976 6554 696d 696e 6744 6174 6160  .LiveTimingData`
-0000bf10: 2074 6f20 7573 6520 6173 2061 2073 6f75   to use as a sou
-0000bf20: 7263 6520 696e 7374 6561 6420 6f66 2074  rce instead of t
-0000bf30: 6865 2061 7069 0a0a 2020 2020 5265 7475  he api..    Retu
-0000bf40: 726e 733a 0a20 2020 2020 2020 207c 2041  rns:.        | A
-0000bf50: 2064 6963 7469 6f6e 6172 7920 636f 6e74   dictionary cont
-0000bf60: 6169 6e69 6e67 206f 6e65 2070 616e 6461  aining one panda
-0000bf70: 7320 4461 7461 4672 616d 6520 7065 7220  s DataFrame per 
-0000bf80: 6472 6976 6572 2e20 4469 6374 696f 6e61  driver. Dictiona
-0000bf90: 7279 206b 6579 7320 6172 6520 7468 6520  ry keys are the 
-0000bfa0: 6472 6976 6572 2773 206e 756d 6265 7273  driver's numbers
-0000bfb0: 2061 730a 2020 2020 2020 2020 2020 7374   as.          st
-0000bfc0: 7269 6e67 2028 652e 672e 2027 3136 2729  ring (e.g. '16')
-0000bfd0: 2e20 596f 7520 7368 6f75 6c64 206e 6576  . You should nev
-0000bfe0: 6572 2061 7373 756d 6520 7468 6174 2061  er assume that a
-0000bff0: 206e 756d 6265 7220 6578 6973 7473 210a   number exists!.
-0000c000: 2020 2020 2020 2020 7c20 4561 6368 2064          | Each d
-0000c010: 6174 6166 7261 6d65 2063 6f6e 7461 696e  ataframe contain
-0000c020: 7320 6f6e 6520 636f 6c75 6d6e 2066 6f72  s one column for
-0000c030: 2065 6163 6820 6461 7461 2063 6861 6e6e   each data chann
-0000c040: 656c 2061 7320 6c69 7374 6564 2061 626f  el as listed abo
-0000c050: 7665 0a0a 2020 2020 5261 6973 6573 3a0a  ve..    Raises:.
-0000c060: 2020 2020 2020 2020 5365 7373 696f 6e4e          SessionN
-0000c070: 6f74 4176 6169 6c61 626c 6545 7272 6f72  otAvailableError
-0000c080: 3a20 696e 2063 6173 6520 7468 6520 4631  : in case the F1
-0000c090: 206c 6976 6574 696d 696e 6720 6170 6920   livetiming api 
-0000c0a0: 7265 7475 726e 7320 6e6f 2064 6174 610a  returns no data.
-0000c0b0: 2020 2020 2222 220a 2020 2020 2320 6461      """.    # da
-0000c0c0: 7461 2072 6563 6f72 6465 6420 6672 6f6d  ta recorded from
-0000c0d0: 206c 6976 6520 7469 6d69 6e67 2068 6173   live timing has
-0000c0e0: 2061 2073 6c69 6768 746c 7920 6469 6666   a slightly diff
-0000c0f0: 6572 656e 7420 7374 7275 6374 7572 650a  erent structure.
-0000c100: 2020 2020 6973 5f6c 6976 6564 6174 6120      is_livedata 
-0000c110: 3d20 4661 6c73 6520 2023 2066 6c61 6720  = False  # flag 
-0000c120: 746f 2069 6e64 6963 6174 6520 6c69 7665  to indicate live
-0000c130: 2074 696d 696e 6720 6461 7461 0a0a 2020   timing data..  
-0000c140: 2020 6966 206c 6976 6564 6174 6120 6973    if livedata is
-0000c150: 206e 6f74 204e 6f6e 6520 616e 6420 6c69   not None and li
-0000c160: 7665 6461 7461 2e68 6173 2827 506f 7369  vedata.has('Posi
-0000c170: 7469 6f6e 2e7a 2729 3a0a 2020 2020 2020  tion.z'):.      
-0000c180: 2020 7265 7370 6f6e 7365 203d 206c 6976    response = liv
-0000c190: 6564 6174 612e 6765 7428 2750 6f73 6974  edata.get('Posit
-0000c1a0: 696f 6e2e 7a27 290a 2020 2020 2020 2020  ion.z').        
-0000c1b0: 6973 5f6c 6976 6564 6174 6120 3d20 5472  is_livedata = Tr
-0000c1c0: 7565 0a20 2020 2065 6c69 6620 7265 7370  ue.    elif resp
-0000c1d0: 6f6e 7365 2069 7320 4e6f 6e65 3a0a 2020  onse is None:.  
-0000c1e0: 2020 2020 2020 5f6c 6f67 6765 722e 696e        _logger.in
-0000c1f0: 666f 2822 4665 7463 6869 6e67 2070 6f73  fo("Fetching pos
-0000c200: 6974 696f 6e20 6461 7461 2e2e 2e22 290a  ition data...").
-0000c210: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-0000c220: 203d 2066 6574 6368 5f70 6167 6528 7061   = fetch_page(pa
-0000c230: 7468 2c20 2770 6f73 6974 696f 6e27 290a  th, 'position').
-0000c240: 2020 2020 2020 2020 6966 2072 6573 706f          if respo
-0000c250: 6e73 6520 6973 204e 6f6e 653a 2020 2320  nse is None:  # 
-0000c260: 6e6f 2072 6573 706f 6e73 6520 7265 6365  no response rece
-0000c270: 6976 6564 0a20 2020 2020 2020 2020 2020  ived.           
-0000c280: 2072 6169 7365 2053 6573 7369 6f6e 4e6f   raise SessionNo
-0000c290: 7441 7661 696c 6162 6c65 4572 726f 7228  tAvailableError(
-0000c2a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c2b0: 2022 4e6f 2064 6174 6120 666f 7220 7468   "No data for th
-0000c2c0: 6973 2073 6573 7369 6f6e 2120 4966 2074  is session! If t
-0000c2d0: 6869 7320 7365 7373 696f 6e20 6f6e 6c79  his session only
-0000c2e0: 2066 696e 6973 6865 6420 220a 2020 2020   finished ".    
-0000c2f0: 2020 2020 2020 2020 2020 2020 2272 6563              "rec
-0000c300: 656e 746c 792c 2070 6c65 6173 6520 7472  ently, please tr
-0000c310: 7920 6167 6169 6e20 696e 2061 2066 6577  y again in a few
-0000c320: 206d 696e 7574 6573 2e22 0a20 2020 2020   minutes.".     
-0000c330: 2020 2020 2020 2029 0a0a 2020 2020 5f6c         )..    _l
-0000c340: 6f67 6765 722e 696e 666f 2822 5061 7273  ogger.info("Pars
-0000c350: 696e 6720 706f 7369 7469 6f6e 2064 6174  ing position dat
-0000c360: 612e 2e2e 2229 0a0a 2020 2020 6966 206e  a...")..    if n
-0000c370: 6f74 2072 6573 706f 6e73 653a 0a20 2020  ot response:.   
-0000c380: 2020 2020 2072 6574 7572 6e20 7b7d 0a0a       return {}..
-0000c390: 2020 2020 7473 5f6c 656e 6774 6820 3d20      ts_length = 
-0000c3a0: 3132 2020 2320 6c65 6e67 7468 206f 6620  12  # length of 
-0000c3b0: 7469 6d65 7374 616d 703a 206c 656e 2827  timestamp: len('
-0000c3c0: 3030 3a30 303a 3030 3a30 3030 2729 0a20  00:00:00:000'). 
-0000c3d0: 2020 2063 6f6c 756d 6e73 203d 205b 2754     columns = ['T
-0000c3e0: 696d 6527 2c20 2744 6174 6527 2c20 2753  ime', 'Date', 'S
-0000c3f0: 7461 7475 7327 2c20 2758 272c 2027 5927  tatus', 'X', 'Y'
-0000c400: 2c20 275a 272c 0a20 2020 2020 2020 2020  , 'Z',.         
-0000c410: 2020 2020 2020 2753 6f75 7263 6527 5d20        'Source'] 
-0000c420: 2023 2063 6f72 7265 6374 206f 7264 6572   # correct order
-0000c430: 2072 6571 7569 7265 6421 0a0a 2020 2020   required!..    
-0000c440: 6461 7461 203d 2064 6963 7428 290a 2020  data = dict().  
-0000c450: 2020 6465 636f 6465 5f65 7272 6f72 5f63    decode_error_c
-0000c460: 6f75 6e74 203d 2030 0a0a 2020 2020 666f  ount = 0..    fo
-0000c470: 7220 7265 636f 7264 2069 6e20 7265 7370  r record in resp
-0000c480: 6f6e 7365 3a0a 2020 2020 2020 2020 7472  onse:.        tr
-0000c490: 793a 0a20 2020 2020 2020 2020 2020 2069  y:.            i
-0000c4a0: 6620 6973 5f6c 6976 6564 6174 613a 0a20  f is_livedata:. 
-0000c4b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000c4c0: 696d 6520 3d20 7265 636f 7264 5b30 5d0a  ime = record[0].
-0000c4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4e0: 6a72 6563 6f72 643a 2064 6963 7420 3d20  jrecord: dict = 
-0000c4f0: 7061 7273 6528 7265 636f 7264 5b31 5d2c  parse(record[1],
-0000c500: 207a 6970 7065 643d 5472 7565 290a 2020   zipped=True).  
-0000c510: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0000c520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c530: 7469 6d65 203d 2074 6f5f 7469 6d65 6465  time = to_timede
-0000c540: 6c74 6128 7265 636f 7264 5b3a 7473 5f6c  lta(record[:ts_l
-0000c550: 656e 6774 685d 290a 2020 2020 2020 2020  ength]).        
-0000c560: 2020 2020 2020 2020 6a72 6563 6f72 643a          jrecord:
-0000c570: 2064 6963 7420 3d20 7061 7273 6528 7265   dict = parse(re
-0000c580: 636f 7264 5b74 735f 6c65 6e67 7468 3a5d  cord[ts_length:]
-0000c590: 2c20 7a69 7070 6564 3d54 7275 6529 0a0a  , zipped=True)..
-0000c5a0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000c5b0: 7361 6d70 6c65 2069 6e20 6a72 6563 6f72  sample in jrecor
-0000c5c0: 645b 2750 6f73 6974 696f 6e27 5d3a 0a20  d['Position']:. 
-0000c5d0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000c5e0: 2064 6174 6520 666f 726d 6174 2069 7320   date format is 
-0000c5f0: 2732 3032 302d 3038 2d30 3854 3039 3a34  '2020-08-08T09:4
-0000c600: 353a 3033 2e30 3631 3937 3937 5a27 2077  5:03.0619797Z' w
-0000c610: 6974 6820 6120 7661 7279 696e 670a 2020  ith a varying.  
-0000c620: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000c630: 6e75 6d62 6572 206f 6620 6d69 6c6c 6973  number of millis
-0000c640: 6563 6f6e 6420 6465 6369 6d61 6c20 706f  econd decimal po
-0000c650: 696e 7473 0a20 2020 2020 2020 2020 2020  ints.           
-0000c660: 2020 2020 2023 2061 6c77 6179 7320 7265       # always re
-0000c670: 6d6f 7665 206c 6173 7420 6368 6172 2028  move last char (
-0000c680: 277a 2729 2c20 6d61 7820 6c65 6e20 3236  'z'), max len 26
-0000c690: 2c20 7269 6768 7420 7061 6420 746f 206c  , right pad to l
-0000c6a0: 656e 0a20 2020 2020 2020 2020 2020 2020  en.             
-0000c6b0: 2020 2023 2032 3620 7769 7468 207a 6572     # 26 with zer
-0000c6c0: 6f65 7320 6966 2073 686f 7274 6572 0a20  oes if shorter. 
-0000c6d0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000c6e0: 6174 6520 3d20 746f 5f64 6174 6574 696d  ate = to_datetim
-0000c6f0: 6528 7361 6d70 6c65 5b27 5469 6d65 7374  e(sample['Timest
-0000c700: 616d 7027 5d29 0a0a 2020 2020 2020 2020  amp'])..        
-0000c710: 2020 2020 2020 2020 666f 7220 6472 7620          for drv 
-0000c720: 696e 2073 616d 706c 655b 2745 6e74 7269  in sample['Entri
-0000c730: 6573 275d 3a0a 2020 2020 2020 2020 2020  es']:.          
-0000c740: 2020 2020 2020 2020 2020 6966 2064 7276            if drv
-0000c750: 206e 6f74 2069 6e20 6461 7461 3a0a 2020   not in data:.  
-0000c760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c770: 2020 2020 2020 2320 696e 6974 6961 6c69        # initiali
-0000c780: 7a65 2064 6963 7420 656e 7472 7920 666f  ze dict entry fo
-0000c790: 7220 7468 6973 2064 7269 7665 720a 2020  r this driver.  
-0000c7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7b0: 2020 2020 2020 6461 7461 5b64 7276 5d20        data[drv] 
-0000c7c0: 3d20 6c69 7374 2829 0a0a 2020 2020 2020  = list()..      
-0000c7d0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-0000c7e0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-0000c7f0: 2020 2020 2020 2020 2020 2078 203d 2073             x = s
-0000c800: 616d 706c 655b 2745 6e74 7269 6573 275d  ample['Entries']
-0000c810: 5b64 7276 5d5b 2758 275d 0a20 2020 2020  [drv]['X'].     
-0000c820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c830: 2020 2079 203d 2073 616d 706c 655b 2745     y = sample['E
-0000c840: 6e74 7269 6573 275d 5b64 7276 5d5b 2759  ntries'][drv]['Y
-0000c850: 275d 0a20 2020 2020 2020 2020 2020 2020  '].             
-0000c860: 2020 2020 2020 2020 2020 207a 203d 2073             z = s
-0000c870: 616d 706c 655b 2745 6e74 7269 6573 275d  ample['Entries']
-0000c880: 5b64 7276 5d5b 275a 275d 0a20 2020 2020  [drv]['Z'].     
-0000c890: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000c8a0: 7863 6570 7420 4b65 7945 7272 6f72 3a0a  xcept KeyError:.
-0000c8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c8c0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-0000c8d0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000c8e0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-0000c8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c900: 2020 2073 7461 7475 7320 3d20 7361 6d70     status = samp
-0000c910: 6c65 5b27 456e 7472 6965 7327 5d5b 6472  le['Entries'][dr
-0000c920: 765d 5b27 5374 6174 7573 275d 0a20 2020  v]['Status'].   
-0000c930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c940: 2065 7863 6570 7420 4b65 7945 7272 6f72   except KeyError
-0000c950: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000c960: 2020 2020 2020 2020 2020 7374 6174 7573            status
-0000c970: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-0000c980: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000c990: 7472 2873 7461 7475 7329 2e69 7364 6967  tr(status).isdig
-0000c9a0: 6974 2829 3a0a 2020 2020 2020 2020 2020  it():.          
-0000c9b0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000c9c0: 4661 6c6c 6261 636b 206f 6e20 6f6c 6465  Fallback on olde
-0000c9d0: 7220 6170 6920 7374 6174 7573 206d 6170  r api status map
-0000c9e0: 7069 6e67 2061 6e64 2063 6f6e 7665 7274  ping and convert
-0000c9f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ca00: 2020 2020 2020 2020 2073 7461 7475 7320           status 
-0000ca10: 3d20 274f 6666 5472 6163 6b27 2069 6620  = 'OffTrack' if 
-0000ca20: 696e 7428 7374 6174 7573 2920 656c 7365  int(status) else
-0000ca30: 2027 4f6e 5472 6163 6b27 0a0a 2020 2020   'OnTrack'..    
-0000ca40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca50: 6461 7461 5b64 7276 5d2e 6170 7065 6e64  data[drv].append
-0000ca60: 2828 7469 6d65 2c20 6461 7465 2c20 7374  ((time, date, st
-0000ca70: 6174 7573 2c20 782c 2079 2c20 7a2c 2027  atus, x, y, z, '
-0000ca80: 706f 7327 2929 0a0a 2020 2020 2020 2020  pos'))..        
-0000ca90: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-0000caa0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-0000cab0: 746f 6f20 7269 736b 7920 746f 2073 7065  too risky to spe
-0000cac0: 6369 6679 2061 6e20 6578 6365 7074 696f  cify an exceptio
-0000cad0: 6e3a 2075 6e65 7870 6563 7465 6420 696e  n: unexpected in
-0000cae0: 7661 6c69 6420 6461 7461 210a 2020 2020  valid data!.    
-0000caf0: 2020 2020 2020 2020 6465 636f 6465 5f65          decode_e
-0000cb00: 7272 6f72 5f63 6f75 6e74 202b 3d20 310a  rror_count += 1.
-0000cb10: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-0000cb20: 696e 7565 0a0a 2020 2020 6966 2064 6563  inue..    if dec
-0000cb30: 6f64 655f 6572 726f 725f 636f 756e 7420  ode_error_count 
-0000cb40: 3e20 303a 0a20 2020 2020 2020 205f 6c6f  > 0:.        _lo
-0000cb50: 6767 6572 2e77 6172 6e69 6e67 280a 2020  gger.warning(.  
-0000cb60: 2020 2020 2020 2020 2020 6622 506f 7369            f"Posi
-0000cb70: 7469 6f6e 2064 6174 613a 2066 6169 6c65  tion data: faile
-0000cb80: 6420 746f 2064 6563 6f64 6520 7b64 6563  d to decode {dec
-0000cb90: 6f64 655f 6572 726f 725f 636f 756e 747d  ode_error_count}
-0000cba0: 2022 0a20 2020 2020 2020 2020 2020 2066   ".            f
-0000cbb0: 226d 6573 7361 6765 7320 287b 6c65 6e28  "messages ({len(
-0000cbc0: 7265 7370 6f6e 7365 297d 206d 6573 7361  response)} messa
-0000cbd0: 6765 7320 746f 7461 6c29 2229 0a0a 2020  ges total)")..  
-0000cbe0: 2020 2320 6372 6561 7465 206f 6e65 2064    # create one d
-0000cbf0: 6174 6166 7261 6d65 2070 6572 2064 7269  ataframe per dri
-0000cc00: 7665 7220 616e 6420 6368 6563 6b20 666f  ver and check fo
-0000cc10: 7220 7468 6520 6c6f 6e67 6573 7420 6461  r the longest da
-0000cc20: 7461 6672 616d 650a 2020 2020 6d6f 7374  taframe.    most
-0000cc30: 5f63 6f6d 706c 6574 655f 7265 6620 3d20  _complete_ref = 
-0000cc40: 4e6f 6e65 0a20 2020 2066 6f72 2064 7276  None.    for drv
-0000cc50: 2069 6e20 6461 7461 3a0a 2020 2020 2020   in data:.      
-0000cc60: 2020 6172 725f 616c 6c20 3d20 6e70 2e61    arr_all = np.a
-0000cc70: 7272 6179 2864 6174 615b 6472 765d 290a  rray(data[drv]).
-0000cc80: 2020 2020 2020 2020 7469 6d65 203d 2061          time = a
-0000cc90: 7272 5f61 6c6c 5b3a 2c20 305d 2e61 7374  rr_all[:, 0].ast
-0000cca0: 7970 6528 2774 696d 6564 656c 7461 3634  ype('timedelta64
-0000ccb0: 5b6e 735d 2729 0a20 2020 2020 2020 2064  [ns]').        d
-0000ccc0: 6174 6520 3d20 6172 725f 616c 6c5b 3a2c  ate = arr_all[:,
-0000ccd0: 2031 5d2e 6173 7479 7065 2827 6461 7465   1].astype('date
-0000cce0: 7469 6d65 3634 5b6e 735d 2729 0a20 2020  time64[ns]').   
-0000ccf0: 2020 2020 2073 7461 7475 7320 3d20 6172       status = ar
-0000cd00: 725f 616c 6c5b 3a2c 2032 5d2e 6173 7479  r_all[:, 2].asty
-0000cd10: 7065 2827 6f62 6a65 6374 2729 0a20 2020  pe('object').   
-0000cd20: 2020 2020 2078 203d 2061 7272 5f61 6c6c       x = arr_all
-0000cd30: 5b3a 2c20 335d 2e61 7374 7970 6528 2769  [:, 3].astype('i
-0000cd40: 6e74 3634 2729 0a20 2020 2020 2020 2079  nt64').        y
-0000cd50: 203d 2061 7272 5f61 6c6c 5b3a 2c20 345d   = arr_all[:, 4]
-0000cd60: 2e61 7374 7970 6528 2769 6e74 3634 2729  .astype('int64')
-0000cd70: 0a20 2020 2020 2020 207a 203d 2061 7272  .        z = arr
-0000cd80: 5f61 6c6c 5b3a 2c20 355d 2e61 7374 7970  _all[:, 5].astyp
-0000cd90: 6528 2769 6e74 3634 2729 0a20 2020 2020  e('int64').     
-0000cda0: 2020 2073 6f75 7263 6520 3d20 6172 725f     source = arr_
-0000cdb0: 616c 6c5b 3a2c 2036 5d2e 6173 7479 7065  all[:, 6].astype
-0000cdc0: 2827 6f62 6a65 6374 2729 0a0a 2020 2020  ('object')..    
-0000cdd0: 2020 2020 6461 7461 5b64 7276 5d20 3d20      data[drv] = 
-0000cde0: 6372 6561 7465 5f64 665f 6661 7374 280a  create_df_fast(.
-0000cdf0: 2020 2020 2020 2020 2020 2020 6172 7261              arra
-0000ce00: 7973 3d5b 7469 6d65 2c20 6461 7465 2c20  ys=[time, date, 
-0000ce10: 7374 6174 7573 2c20 782c 2079 2c20 7a2c  status, x, y, z,
-0000ce20: 2073 6f75 7263 655d 2c0a 2020 2020 2020   source],.      
-0000ce30: 2020 2020 2020 636f 6c75 6d6e 733d 636f        columns=co
-0000ce40: 6c75 6d6e 730a 2020 2020 2020 2020 290a  lumns.        ).
-0000ce50: 0a20 2020 2020 2020 2023 2063 6865 636b  .        # check
-0000ce60: 206c 656e 6774 6820 6f66 2064 6174 6166   length of dataf
-0000ce70: 7261 6d65 3b20 736f 6d65 7469 6d65 7320  rame; sometimes 
-0000ce80: 7468 6572 6520 6361 6e20 6265 206d 6973  there can be mis
-0000ce90: 7369 6e67 2064 6174 610a 2020 2020 2020  sing data.      
-0000cea0: 2020 6966 2028 6d6f 7374 5f63 6f6d 706c    if (most_compl
-0000ceb0: 6574 655f 7265 6620 6973 204e 6f6e 6529  ete_ref is None)
-0000cec0: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
-0000ced0: 2020 206f 7220 286c 656e 2864 6174 615b     or (len(data[
-0000cee0: 6472 765d 5b27 4461 7465 275d 2920 3e20  drv]['Date']) > 
-0000cef0: 6c65 6e28 6d6f 7374 5f63 6f6d 706c 6574  len(most_complet
-0000cf00: 655f 7265 6629 293a 0a20 2020 2020 2020  e_ref)):.       
-0000cf10: 2020 2020 206d 6f73 745f 636f 6d70 6c65       most_comple
-0000cf20: 7465 5f72 6566 203d 2064 6174 615b 6472  te_ref = data[dr
-0000cf30: 765d 5b27 4461 7465 275d 0a0a 2020 2020  v]['Date']..    
-0000cf40: 2320 6966 2065 7665 7279 7468 696e 6720  # if everything 
-0000cf50: 6973 2077 656c 6c2c 2061 6c6c 2064 6174  is well, all dat
-0000cf60: 6166 7261 6d65 7320 7368 6f75 6c64 2068  aframes should h
-0000cf70: 6176 6520 7468 6520 7361 6d65 206c 656e  ave the same len
-0000cf80: 6774 6820 616e 6420 6e6f 0a20 2020 2023  gth and no.    #
-0000cf90: 2070 6f73 7470 726f 6365 7373 696e 6720   postprocessing 
-0000cfa0: 6973 206e 6563 6573 7361 7279 0a20 2020  is necessary.   
-0000cfb0: 2066 6f72 2064 7276 2069 6e20 6461 7461   for drv in data
-0000cfc0: 3a0a 2020 2020 2020 2020 6966 206c 656e  :.        if len
-0000cfd0: 2864 6174 615b 6472 765d 5b27 4461 7465  (data[drv]['Date
-0000cfe0: 275d 2920 3c20 6c65 6e28 6d6f 7374 5f63  ']) < len(most_c
-0000cff0: 6f6d 706c 6574 655f 7265 6629 3a0a 2020  omplete_ref):.  
-0000d000: 2020 2020 2020 2020 2020 2320 7468 6572            # ther
-0000d010: 6520 6973 206d 6973 7369 6e67 2064 6174  e is missing dat
-0000d020: 6120 666f 7220 7468 6973 2064 7269 7665  a for this drive
-0000d030: 720a 2020 2020 2020 2020 2020 2020 2320  r.            # 
-0000d040: 6578 7465 6e64 2074 6865 2044 6174 6520  extend the Date 
-0000d050: 636f 6c75 6d6e 2061 6e64 2066 696c 6c20  column and fill 
-0000d060: 7570 206d 6973 7369 6e67 2074 656c 656d  up missing telem
-0000d070: 6574 7279 2076 616c 7565 7320 7769 7468  etry values with
-0000d080: 0a20 2020 2020 2020 2020 2020 2023 207a  .            # z
-0000d090: 6572 6f2c 2065 7863 6570 7420 5469 6d65  ero, except Time
-0000d0a0: 2077 6869 6368 2069 7320 6c65 6674 2061   which is left a
-0000d0b0: 7320 4e61 5420 616e 6420 7769 6c6c 2062  s NaT and will b
-0000d0c0: 6520 6361 6c63 756c 6174 6564 0a20 2020  e calculated.   
-0000d0d0: 2020 2020 2020 2020 2023 2063 6f72 7265           # corre
-0000d0e0: 6374 6c79 2062 6173 6564 206f 6e20 5365  ctly based on Se
-0000d0f0: 7373 696f 6e2e 7430 5f64 6174 6520 616e  ssion.t0_date an
-0000d100: 7977 6179 2077 6865 6e20 6372 6561 7469  yway when creati
-0000d110: 6e67 2054 656c 656d 6574 7279 0a20 2020  ng Telemetry.   
-0000d120: 2020 2020 2020 2020 2023 2069 6e73 7461           # insta
-0000d130: 6e63 6573 2069 6e20 5365 7373 696f 6e2e  nces in Session.
-0000d140: 6c6f 6164 5f74 656c 656d 6574 7279 0a20  load_telemetry. 
-0000d150: 2020 2020 2020 2020 2020 2023 2061 6e64             # and
-0000d160: 2065 7863 6570 7420 5374 6174 7573 2077   except Status w
-0000d170: 6869 6368 2073 686f 756c 6420 6265 2027  hich should be '
-0000d180: 4f66 6654 7261 636b 2720 666f 7220 6d69  OffTrack' for mi
-0000d190: 7373 696e 6720 6461 7461 0a20 2020 2020  ssing data.     
-0000d1a0: 2020 2020 2020 2064 6174 615b 6472 765d         data[drv]
-0000d1b0: 203d 2064 6174 615b 6472 765d 205c 0a20   = data[drv] \. 
-0000d1c0: 2020 2020 2020 2020 2020 2020 2020 202e                 .
-0000d1d0: 6d65 7267 6528 6d6f 7374 5f63 6f6d 706c  merge(most_compl
-0000d1e0: 6574 655f 7265 662c 2068 6f77 3d27 6f75  ete_ref, how='ou
-0000d1f0: 7465 7227 2920 5c0a 2020 2020 2020 2020  ter') \.        
-0000d200: 2020 2020 2020 2020 2e73 6f72 745f 7661          .sort_va
-0000d210: 6c75 6573 2862 793d 2744 6174 6527 2920  lues(by='Date') 
-0000d220: 5c0a 2020 2020 2020 2020 2020 2020 2020  \.              
-0000d230: 2020 2e72 6573 6574 5f69 6e64 6578 2864    .reset_index(d
-0000d240: 726f 703d 5472 7565 290a 2020 2020 2020  rop=True).      
-0000d250: 2020 2020 2020 6461 7461 5b64 7276 5d5b        data[drv][
-0000d260: 2753 7461 7475 7327 5d20 3d20 6461 7461  'Status'] = data
-0000d270: 5b64 7276 5d5b 2753 7461 7475 7327 5d20  [drv]['Status'] 
-0000d280: 5c0a 2020 2020 2020 2020 2020 2020 2020  \.              
-0000d290: 2020 2e66 696c 6c6e 6128 7661 6c75 653d    .fillna(value=
-0000d2a0: 274f 6666 5472 6163 6b27 2c20 696e 706c  'OffTrack', inpl
-0000d2b0: 6163 653d 4661 6c73 6529 0a20 2020 2020  ace=False).     
-0000d2c0: 2020 2020 2020 2064 6174 615b 6472 765d         data[drv]
-0000d2d0: 2e6c 6f63 5b3a 2c20 5b27 5827 2c20 2759  .loc[:, ['X', 'Y
-0000d2e0: 272c 2027 5a27 5d5d 203d 205c 0a20 2020  ', 'Z']] = \.   
-0000d2f0: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-0000d300: 615b 6472 765d 2e6c 6f63 5b3a 2c20 5b27  a[drv].loc[:, ['
-0000d310: 5827 2c20 2759 272c 2027 5a27 5d5d 5c0a  X', 'Y', 'Z']]\.
-0000d320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d330: 2e66 696c 6c6e 6128 7661 6c75 653d 302c  .fillna(value=0,
-0000d340: 2069 6e70 6c61 6365 3d46 616c 7365 290a   inplace=False).
-0000d350: 0a20 2020 2020 2020 2020 2020 205f 6c6f  .            _lo
-0000d360: 6767 6572 2e77 6172 6e69 6e67 2866 2244  gger.warning(f"D
-0000d370: 7269 7665 7220 7b64 7276 3a20 3e32 7d3a  river {drv: >2}:
-0000d380: 2050 6f73 6974 696f 6e20 6461 7461 2069   Position data i
-0000d390: 7320 220a 2020 2020 2020 2020 2020 2020  s ".            
-0000d3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3b0: 6622 696e 636f 6d70 6c65 7465 2122 290a  f"incomplete!").
-0000d3c0: 0a20 2020 2072 6574 7572 6e20 6461 7461  .    return data
-0000d3d0: 0a0a 0a40 4361 6368 652e 6170 695f 7265  ...@Cache.api_re
-0000d3e0: 7175 6573 745f 7772 6170 7065 720a 6465  quest_wrapper.de
-0000d3f0: 6620 7472 6163 6b5f 7374 6174 7573 5f64  f track_status_d
-0000d400: 6174 6128 7061 7468 2c20 7265 7370 6f6e  ata(path, respon
-0000d410: 7365 3d4e 6f6e 652c 206c 6976 6564 6174  se=None, livedat
-0000d420: 613d 4e6f 6e65 293a 0a20 2020 2022 2222  a=None):.    """
-0000d430: 0a20 2020 202e 2e20 7761 726e 696e 673a  .    .. warning:
-0000d440: 3a0a 2020 2020 2020 2020 3a6d 6f64 3a60  :.        :mod:`
-0000d450: 6661 7374 6631 2e61 7069 6020 7769 6c6c  fastf1.api` will
-0000d460: 2062 6520 636f 6e73 6964 6572 6564 2070   be considered p
-0000d470: 7269 7661 7465 2069 6e20 6675 7475 7265  rivate in future
-0000d480: 2072 656c 6561 7365 7320 616e 640a 2020   releases and.  
-0000d490: 2020 2020 2020 706f 7465 6e74 6961 6c6c        potentiall
-0000d4a0: 7920 6265 2072 656d 6f76 6564 206f 7220  y be removed or 
-0000d4b0: 6368 616e 6765 642e 0a0a 2020 2020 4665  changed...    Fe
-0000d4c0: 7463 6820 616e 6420 7061 7273 6520 7472  tch and parse tr
-0000d4d0: 6163 6b20 7374 6174 7573 2064 6174 612e  ack status data.
-0000d4e0: 0a0a 2020 2020 5472 6163 6b20 7374 6174  ..    Track stat
-0000d4f0: 7573 2063 6f6e 7461 696e 7320 696e 666f  us contains info
-0000d500: 726d 6174 696f 6e20 6f6e 2079 656c 6c6f  rmation on yello
-0000d510: 772f 7265 642f 6772 6565 6e20 666c 6167  w/red/green flag
-0000d520: 732c 2073 6166 6574 7920 6361 7220 616e  s, safety car an
-0000d530: 6420 7669 7274 7561 6c20 7361 6665 7479  d virtual safety
-0000d540: 2063 6172 2e20 4974 2070 726f 7669 6465   car. It provide
-0000d550: 7320 7468 650a 2020 2020 666f 6c6c 6f77  s the.    follow
-0000d560: 696e 6720 6461 7461 2063 6861 6e6e 656c  ing data channel
-0000d570: 7320 7065 7220 7361 6d70 6c65 3a0a 0a20  s per sample:.. 
-0000d580: 2020 2020 2020 202d 2054 696d 6520 2864         - Time (d
-0000d590: 6174 6574 696d 652e 7469 6d65 6465 6c74  atetime.timedelt
-0000d5a0: 6129 3a20 7365 7373 696f 6e20 7469 6d65  a): session time
-0000d5b0: 7374 616d 7020 2874 696d 6520 6f6e 6c79  stamp (time only
-0000d5c0: 290a 2020 2020 2020 2020 2d20 5374 6174  ).        - Stat
-0000d5d0: 7573 2028 7374 7229 3a20 636f 6e74 6169  us (str): contai
-0000d5e0: 6e73 2074 7261 636b 2073 7461 7475 7320  ns track status 
-0000d5f0: 6368 616e 6765 7320 6173 206e 756d 6572  changes as numer
-0000d600: 6963 2076 616c 7565 7320 2864 6573 6372  ic values (descr
-0000d610: 6962 6564 2062 656c 6f77 290a 2020 2020  ibed below).    
-0000d620: 2020 2020 2d20 4d65 7373 6167 6520 2873      - Message (s
-0000d630: 7472 293a 2063 6f6e 7461 696e 7320 7468  tr): contains th
-0000d640: 6520 7361 6d65 2069 6e66 6f72 6d61 7469  e same informati
-0000d650: 6f6e 2061 7320 7374 6174 7573 2062 7574  on as status but
-0000d660: 2069 6e20 6561 7369 6c79 2075 6e64 6572   in easily under
-0000d670: 7374 616e 6461 626c 650a 2020 2020 2020  standable.      
-0000d680: 2020 2020 776f 7264 7320 2827 5965 6c6c      words ('Yell
-0000d690: 6f77 272c 2027 416c 6c43 6c65 6172 272c  ow', 'AllClear',
-0000d6a0: 2e2e 2e29 0a0a 2020 2020 4120 6e65 7720  ...)..    A new 
-0000d6b0: 7661 6c75 6520 6973 2073 656e 7420 6576  value is sent ev
-0000d6c0: 6572 7920 7469 6d65 2074 6865 2074 7261  ery time the tra
-0000d6d0: 636b 2073 7461 7475 7320 6368 616e 6765  ck status change
-0000d6e0: 732e 0a0a 2020 2020 5472 6163 6b20 7374  s...    Track st
-0000d6f0: 6174 7573 2069 7320 696e 6469 6361 7465  atus is indicate
-0000d700: 6420 7573 696e 6720 7369 6e67 6c65 2064  d using single d
-0000d710: 6967 6974 2069 6e74 6567 6572 2073 7461  igit integer sta
-0000d720: 7475 7320 636f 6465 7320 2861 7320 7374  tus codes (as st
-0000d730: 7269 6e67 292e 204c 6973 7420 6f66 206b  ring). List of k
-0000d740: 6e6f 776e 2073 7461 7475 7365 733a 0a0a  nown statuses:..
-0000d750: 2020 2020 2020 2020 2d20 2731 273a 2054          - '1': T
-0000d760: 7261 636b 2063 6c65 6172 2028 6265 6769  rack clear (begi
-0000d770: 6e6e 696e 6720 6f66 2073 6573 7369 6f6e  nning of session
-0000d780: 206f 7220 746f 2069 6e64 6963 6174 6520   or to indicate 
-0000d790: 7468 6520 656e 640a 2020 2020 2020 2020  the end.        
-0000d7a0: 2020 206f 6620 616e 6f74 6865 7220 7374     of another st
-0000d7b0: 6174 7573 290a 2020 2020 2020 2020 2d20  atus).        - 
-0000d7c0: 2732 273a 2059 656c 6c6f 7720 666c 6167  '2': Yellow flag
-0000d7d0: 2028 7365 6374 6f72 7320 6172 6520 756e   (sectors are un
-0000d7e0: 6b6e 6f77 6e29 0a20 2020 2020 2020 202d  known).        -
-0000d7f0: 2027 3327 3a20 3f3f 3f20 4e65 7665 7220   '3': ??? Never 
-0000d800: 7365 656e 2073 6f20 6661 722c 2064 6f65  seen so far, doe
-0000d810: 7320 6e6f 7420 6578 6973 743f 0a20 2020  s not exist?.   
-0000d820: 2020 2020 202d 2027 3427 3a20 5361 6665       - '4': Safe
-0000d830: 7479 2043 6172 0a20 2020 2020 2020 202d  ty Car.        -
-0000d840: 2027 3527 3a20 5265 6420 466c 6167 0a20   '5': Red Flag. 
-0000d850: 2020 2020 2020 202d 2027 3627 3a20 5669         - '6': Vi
-0000d860: 7274 7561 6c20 5361 6665 7479 2043 6172  rtual Safety Car
-0000d870: 2064 6570 6c6f 7965 640a 2020 2020 2020   deployed.      
-0000d880: 2020 2d20 2737 273a 2056 6972 7475 616c    - '7': Virtual
-0000d890: 2053 6166 6574 7920 4361 7220 656e 6469   Safety Car endi
-0000d8a0: 6e67 2028 4173 2069 6e64 6963 6174 6564  ng (As indicated
-0000d8b0: 206f 6e20 7468 6520 6472 6976 6572 7320   on the drivers 
-0000d8c0: 7374 6565 7269 6e67 2077 6865 656c 2c20  steering wheel, 
-0000d8d0: 6f6e 2074 7620 616e 6420 736f 206f 6e3b  on tv and so on;
-0000d8e0: 2073 7461 7475 7320 2731 270a 2020 2020   status '1'.    
-0000d8f0: 2020 2020 2020 7769 6c6c 206d 6172 6b20        will mark 
-0000d900: 7468 6520 6163 7475 616c 2065 6e64 290a  the actual end).
-0000d910: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-0000d920: 2020 2070 6174 6820 2873 7472 293a 2061     path (str): a
-0000d930: 7069 2070 6174 6820 6261 7365 2073 7472  pi path base str
-0000d940: 696e 6720 2875 7375 616c 6c79 2060 6053  ing (usually ``S
-0000d950: 6573 7369 6f6e 2e61 7069 5f70 6174 6860  ession.api_path`
-0000d960: 6029 0a20 2020 2020 2020 2072 6573 706f  `).        respo
-0000d970: 6e73 653a 2052 6573 706f 6e73 6520 6173  nse: Response as
-0000d980: 2072 6574 7572 6e65 6420 6279 203a 6675   returned by :fu
-0000d990: 6e63 3a60 6665 7463 685f 7061 6765 6020  nc:`fetch_page` 
-0000d9a0: 6361 6e20 6265 2070 6173 7365 6420 6966  can be passed if
-0000d9b0: 2069 7420 7761 7320 646f 776e 6c6f 6164   it was download
-0000d9c0: 6564 2061 6c72 6561 6479 2e0a 2020 2020  ed already..    
-0000d9d0: 2020 2020 6c69 7665 6461 7461 3a20 416e      livedata: An
-0000d9e0: 2069 6e73 7461 6e63 6520 6f66 203a 636c   instance of :cl
-0000d9f0: 6173 733a 6066 6173 7466 312e 6c69 7665  ass:`fastf1.live
-0000da00: 7469 6d69 6e67 2e64 6174 612e 4c69 7665  timing.data.Live
-0000da10: 5469 6d69 6e67 4461 7461 6020 746f 2075  TimingData` to u
-0000da20: 7365 2061 7320 6120 736f 7572 6365 2069  se as a source i
-0000da30: 6e73 7465 6164 206f 6620 7468 6520 6170  nstead of the ap
-0000da40: 690a 0a20 2020 2052 6574 7572 6e73 3a0a  i..    Returns:.
-0000da50: 2020 2020 2020 2020 4120 6469 6374 696f          A dictio
-0000da60: 6e61 7279 2063 6f6e 7461 696e 696e 6720  nary containing 
-0000da70: 6f6e 6520 6b65 7920 666f 7220 6561 6368  one key for each
-0000da80: 2064 6174 6120 6368 616e 6e65 6c20 616e   data channel an
-0000da90: 6420 6120 6c69 7374 206f 6620 7661 6c75  d a list of valu
-0000daa0: 6573 2070 6572 206b 6579 2e0a 0a20 2020  es per key...   
-0000dab0: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
-0000dac0: 2053 6573 7369 6f6e 4e6f 7441 7661 696c   SessionNotAvail
-0000dad0: 6162 6c65 4572 726f 723a 2069 6e20 6361  ableError: in ca
-0000dae0: 7365 2074 6865 2046 3120 6c69 7665 7469  se the F1 liveti
-0000daf0: 6d69 6e67 2061 7069 2072 6574 7572 6e73  ming api returns
-0000db00: 206e 6f20 6461 7461 0a20 2020 2022 2222   no data.    """
-0000db10: 0a20 2020 2069 6620 6c69 7665 6461 7461  .    if livedata
-0000db20: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-0000db30: 206c 6976 6564 6174 612e 6861 7328 2754   livedata.has('T
-0000db40: 7261 636b 5374 6174 7573 2729 3a0a 2020  rackStatus'):.  
-0000db50: 2020 2020 2020 2320 646f 6573 206e 6f74        # does not
-0000db60: 206e 6565 6420 616e 7920 6675 7274 6865   need any furthe
-0000db70: 7220 7072 6f63 6573 7369 6e67 0a20 2020  r processing.   
-0000db80: 2020 2020 205f 6c6f 6767 6572 2e69 6e66       _logger.inf
-0000db90: 6f28 224c 6f61 6469 6e67 2074 7261 636b  o("Loading track
-0000dba0: 2073 7461 7475 7320 6461 7461 2229 0a20   status data"). 
-0000dbb0: 2020 2020 2020 2072 6574 7572 6e20 6c69         return li
-0000dbc0: 7665 6461 7461 2e67 6574 2827 5472 6163  vedata.get('Trac
-0000dbd0: 6b53 7461 7475 7327 290a 2020 2020 656c  kStatus').    el
-0000dbe0: 6966 2072 6573 706f 6e73 6520 6973 204e  if response is N
-0000dbf0: 6f6e 653a 0a20 2020 2020 2020 205f 6c6f  one:.        _lo
-0000dc00: 6767 6572 2e69 6e66 6f28 2246 6574 6368  gger.info("Fetch
-0000dc10: 696e 6720 7472 6163 6b20 7374 6174 7573  ing track status
-0000dc20: 2064 6174 612e 2e2e 2229 0a20 2020 2020   data...").     
-0000dc30: 2020 2072 6573 706f 6e73 6520 3d20 6665     response = fe
-0000dc40: 7463 685f 7061 6765 2870 6174 682c 2027  tch_page(path, '
-0000dc50: 7472 6163 6b5f 7374 6174 7573 2729 0a20  track_status'). 
-0000dc60: 2020 2020 2020 2069 6620 7265 7370 6f6e         if respon
-0000dc70: 7365 2069 7320 4e6f 6e65 3a20 2023 206e  se is None:  # n
-0000dc80: 6f20 7265 7370 6f6e 7365 2072 6563 6569  o response recei
-0000dc90: 7665 640a 2020 2020 2020 2020 2020 2020  ved.            
-0000dca0: 7261 6973 6520 5365 7373 696f 6e4e 6f74  raise SessionNot
-0000dcb0: 4176 6169 6c61 626c 6545 7272 6f72 280a  AvailableError(.
-0000dcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dcd0: 224e 6f20 6461 7461 2066 6f72 2074 6869  "No data for thi
-0000dce0: 7320 7365 7373 696f 6e21 2049 6620 7468  s session! If th
-0000dcf0: 6973 2073 6573 7369 6f6e 206f 6e6c 7920  is session only 
-0000dd00: 6669 6e69 7368 6564 2022 0a20 2020 2020  finished ".     
-0000dd10: 2020 2020 2020 2020 2020 2022 7265 6365             "rece
-0000dd20: 6e74 6c79 2c20 706c 6561 7365 2074 7279  ntly, please try
-0000dd30: 2061 6761 696e 2069 6e20 6120 6665 7720   again in a few 
-0000dd40: 6d69 6e75 7465 732e 220a 2020 2020 2020  minutes.".      
-0000dd50: 2020 2020 2020 290a 0a20 2020 2064 6174        )..    dat
-0000dd60: 6120 3d20 7b27 5469 6d65 273a 205b 5d2c  a = {'Time': [],
-0000dd70: 2027 5374 6174 7573 273a 205b 5d2c 2027   'Status': [], '
-0000dd80: 4d65 7373 6167 6527 3a20 5b5d 7d0a 0a20  Message': []}.. 
-0000dd90: 2020 2066 6f72 2065 6e74 7279 2069 6e20     for entry in 
-0000dda0: 7265 7370 6f6e 7365 3a0a 2020 2020 2020  response:.      
-0000ddb0: 2020 6966 206c 656e 2865 6e74 7279 2920    if len(entry) 
-0000ddc0: 3c20 323a 0a20 2020 2020 2020 2020 2020  < 2:.           
-0000ddd0: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
-0000dde0: 2020 726f 7720 3d20 656e 7472 795b 315d    row = entry[1]
-0000ddf0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-0000de00: 6973 696e 7374 616e 6365 2872 6f77 2c20  isinstance(row, 
-0000de10: 6469 6374 293a 0a20 2020 2020 2020 2020  dict):.         
-0000de20: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
-0000de30: 2020 2020 6461 7461 5b27 5469 6d65 275d      data['Time']
-0000de40: 2e61 7070 656e 6428 746f 5f74 696d 6564  .append(to_timed
-0000de50: 656c 7461 2865 6e74 7279 5b30 5d29 290a  elta(entry[0])).
-0000de60: 2020 2020 2020 2020 6461 7461 5b27 5374          data['St
-0000de70: 6174 7573 275d 2e61 7070 656e 6428 726f  atus'].append(ro
-0000de80: 772e 6765 7428 2753 7461 7475 7327 2c20  w.get('Status', 
-0000de90: 2727 2929 0a20 2020 2020 2020 2064 6174  '')).        dat
-0000dea0: 615b 274d 6573 7361 6765 275d 2e61 7070  a['Message'].app
-0000deb0: 656e 6428 726f 772e 6765 7428 274d 6573  end(row.get('Mes
-0000dec0: 7361 6765 272c 2027 2729 290a 0a20 2020  sage', ''))..   
-0000ded0: 2072 6574 7572 6e20 6461 7461 0a0a 0a40   return data...@
-0000dee0: 4361 6368 652e 6170 695f 7265 7175 6573  Cache.api_reques
-0000def0: 745f 7772 6170 7065 720a 6465 6620 7365  t_wrapper.def se
-0000df00: 7373 696f 6e5f 7374 6174 7573 5f64 6174  ssion_status_dat
-0000df10: 6128 7061 7468 2c20 7265 7370 6f6e 7365  a(path, response
-0000df20: 3d4e 6f6e 652c 206c 6976 6564 6174 613d  =None, livedata=
-0000df30: 4e6f 6e65 293a 0a20 2020 2022 2222 0a20  None):.    """. 
-0000df40: 2020 202e 2e20 7761 726e 696e 673a 3a0a     .. warning::.
-0000df50: 2020 2020 2020 2020 3a6d 6f64 3a60 6661          :mod:`fa
-0000df60: 7374 6631 2e61 7069 6020 7769 6c6c 2062  stf1.api` will b
-0000df70: 6520 636f 6e73 6964 6572 6564 2070 7269  e considered pri
-0000df80: 7661 7465 2069 6e20 6675 7475 7265 2072  vate in future r
-0000df90: 656c 6561 7365 7320 616e 640a 2020 2020  eleases and.    
-0000dfa0: 2020 2020 706f 7465 6e74 6961 6c6c 7920      potentially 
-0000dfb0: 6265 2072 656d 6f76 6564 206f 7220 6368  be removed or ch
-0000dfc0: 616e 6765 642e 0a0a 2020 2020 4665 7463  anged...    Fetc
-0000dfd0: 6820 616e 6420 7061 7273 6520 7365 7373  h and parse sess
-0000dfe0: 696f 6e20 7374 6174 7573 2064 6174 612e  ion status data.
-0000dff0: 0a0a 2020 2020 5365 7373 696f 6e20 7374  ..    Session st
-0000e000: 6174 7573 2063 6f6e 7461 696e 7320 696e  atus contains in
-0000e010: 666f 726d 6174 696f 6e20 6f6e 2077 6865  formation on whe
-0000e020: 6e20 6120 7365 7373 696f 6e20 7761 7320  n a session was 
-0000e030: 7374 6172 7465 6420 616e 6420 7768 656e  started and when
-0000e040: 2069 7420 656e 6465 6420 2861 6d6f 6e67   it ended (among
-0000e050: 7374 206f 7468 6572 7329 2e20 4974 0a20  st others). It. 
-0000e060: 2020 2070 726f 7669 6465 7320 7468 6520     provides the 
-0000e070: 666f 6c6c 6f77 696e 6720 6461 7461 2063  following data c
-0000e080: 6861 6e6e 656c 7320 7065 7220 7361 6d70  hannels per samp
-0000e090: 6c65 3a0a 0a20 2020 2020 2020 202d 2054  le:..        - T
-0000e0a0: 696d 6520 2864 6174 6574 696d 652e 7469  ime (datetime.ti
-0000e0b0: 6d65 6465 6c74 6129 3a20 7365 7373 696f  medelta): sessio
-0000e0c0: 6e20 7469 6d65 7374 616d 7020 2874 696d  n timestamp (tim
-0000e0d0: 6520 6f6e 6c79 290a 2020 2020 2020 2020  e only).        
-0000e0e0: 2d20 5374 6174 7573 2028 7374 7229 3a20  - Status (str): 
-0000e0f0: 7374 6174 7573 206d 6573 7361 6765 730a  status messages.
-0000e100: 0a20 2020 2041 206e 6577 2076 616c 7565  .    A new value
-0000e110: 2069 7320 7365 6e74 2065 7665 7279 2074   is sent every t
-0000e120: 696d 6520 7468 6520 7365 7373 696f 6e20  ime the session 
-0000e130: 7374 6174 7573 2063 6861 6e67 6573 2e0a  status changes..
-0000e140: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-0000e150: 2020 2070 6174 6820 2873 7472 293a 2061     path (str): a
-0000e160: 7069 2070 6174 6820 6261 7365 2073 7472  pi path base str
-0000e170: 696e 6720 2875 7375 616c 6c79 2060 6053  ing (usually ``S
-0000e180: 6573 7369 6f6e 2e61 7069 5f70 6174 6860  ession.api_path`
-0000e190: 6029 0a20 2020 2020 2020 2072 6573 706f  `).        respo
-0000e1a0: 6e73 653a 2052 6573 706f 6e73 6520 6173  nse: Response as
-0000e1b0: 2072 6574 7572 6e65 6420 6279 203a 6675   returned by :fu
-0000e1c0: 6e63 3a60 6665 7463 685f 7061 6765 6020  nc:`fetch_page` 
-0000e1d0: 6361 6e20 6265 2070 6173 7365 6420 6966  can be passed if
-0000e1e0: 2069 7420 7761 7320 646f 776e 6c6f 6164   it was download
-0000e1f0: 6564 2061 6c72 6561 6479 2e0a 2020 2020  ed already..    
-0000e200: 2020 2020 6c69 7665 6461 7461 3a20 416e      livedata: An
-0000e210: 2069 6e73 7461 6e63 6520 6f66 203a 636c   instance of :cl
-0000e220: 6173 733a 6066 6173 7466 312e 6c69 7665  ass:`fastf1.live
-0000e230: 7469 6d69 6e67 2e64 6174 612e 4c69 7665  timing.data.Live
-0000e240: 5469 6d69 6e67 4461 7461 6020 746f 2075  TimingData` to u
-0000e250: 7365 2061 7320 6120 736f 7572 6365 2069  se as a source i
-0000e260: 6e73 7465 6164 206f 6620 7468 6520 6170  nstead of the ap
-0000e270: 690a 0a20 2020 2052 6574 7572 6e73 3a0a  i..    Returns:.
-0000e280: 2020 2020 2020 2020 4120 6469 6374 696f          A dictio
-0000e290: 6e61 7279 2063 6f6e 7461 696e 696e 6720  nary containing 
-0000e2a0: 6f6e 6520 6b65 7920 666f 7220 6561 6368  one key for each
-0000e2b0: 2064 6174 6120 6368 616e 6e65 6c20 616e   data channel an
-0000e2c0: 6420 6120 6c69 7374 206f 6620 7661 6c75  d a list of valu
-0000e2d0: 6573 2070 6572 206b 6579 2e0a 0a20 2020  es per key...   
-0000e2e0: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
-0000e2f0: 2053 6573 7369 6f6e 4e6f 7441 7661 696c   SessionNotAvail
-0000e300: 6162 6c65 4572 726f 723a 2069 6e20 6361  ableError: in ca
-0000e310: 7365 2074 6865 2046 3120 6c69 7665 7469  se the F1 liveti
-0000e320: 6d69 6e67 2061 7069 2072 6574 7572 6e73  ming api returns
-0000e330: 206e 6f20 6461 7461 0a20 2020 2022 2222   no data.    """
-0000e340: 0a20 2020 2069 6620 6c69 7665 6461 7461  .    if livedata
-0000e350: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-0000e360: 206c 6976 6564 6174 612e 6861 7328 2753   livedata.has('S
-0000e370: 6573 7369 6f6e 5374 6174 7573 2729 3a0a  essionStatus'):.
-0000e380: 2020 2020 2020 2020 2320 646f 6573 206e          # does n
-0000e390: 6f74 206e 6565 6420 616e 7920 6675 7274  ot need any furt
-0000e3a0: 6865 7220 7072 6f63 6573 7369 6e67 0a20  her processing. 
-0000e3b0: 2020 2020 2020 205f 6c6f 6767 6572 2e69         _logger.i
-0000e3c0: 6e66 6f28 224c 6f61 6469 6e67 2073 6573  nfo("Loading ses
-0000e3d0: 7369 6f6e 2073 7461 7475 7320 6461 7461  sion status data
-0000e3e0: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
-0000e3f0: 6e20 6c69 7665 6461 7461 2e67 6574 2827  n livedata.get('
-0000e400: 5365 7373 696f 6e53 7461 7475 7327 290a  SessionStatus').
-0000e410: 2020 2020 656c 6966 2072 6573 706f 6e73      elif respons
-0000e420: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
-0000e430: 2020 205f 6c6f 6767 6572 2e69 6e66 6f28     _logger.info(
-0000e440: 2246 6574 6368 696e 6720 7365 7373 696f  "Fetching sessio
-0000e450: 6e20 7374 6174 7573 2064 6174 612e 2e2e  n status data...
-0000e460: 2229 0a20 2020 2020 2020 2072 6573 706f  ").        respo
-0000e470: 6e73 6520 3d20 6665 7463 685f 7061 6765  nse = fetch_page
-0000e480: 2870 6174 682c 2027 7365 7373 696f 6e5f  (path, 'session_
-0000e490: 7374 6174 7573 2729 0a20 2020 2020 2020  status').       
-0000e4a0: 2069 6620 7265 7370 6f6e 7365 2069 7320   if response is 
-0000e4b0: 4e6f 6e65 3a20 2023 206e 6f20 7265 7370  None:  # no resp
-0000e4c0: 6f6e 7365 2072 6563 6569 7665 640a 2020  onse received.  
-0000e4d0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000e4e0: 5365 7373 696f 6e4e 6f74 4176 6169 6c61  SessionNotAvaila
-0000e4f0: 626c 6545 7272 6f72 280a 2020 2020 2020  bleError(.      
-0000e500: 2020 2020 2020 2020 2020 224e 6f20 6461            "No da
-0000e510: 7461 2066 6f72 2074 6869 7320 7365 7373  ta for this sess
-0000e520: 696f 6e21 2049 6620 7468 6973 2073 6573  ion! If this ses
-0000e530: 7369 6f6e 206f 6e6c 7920 6669 6e69 7368  sion only finish
-0000e540: 6564 2022 0a20 2020 2020 2020 2020 2020  ed ".           
-0000e550: 2020 2020 2022 7265 6365 6e74 6c79 2c20       "recently, 
-0000e560: 706c 6561 7365 2074 7279 2061 6761 696e  please try again
-0000e570: 2069 6e20 6120 6665 7720 6d69 6e75 7465   in a few minute
-0000e580: 732e 220a 2020 2020 2020 2020 2020 2020  s.".            
-0000e590: 290a 0a20 2020 2064 6174 6120 3d20 7b27  )..    data = {'
-0000e5a0: 5469 6d65 273a 205b 5d2c 2027 5374 6174  Time': [], 'Stat
-0000e5b0: 7573 273a 205b 5d7d 0a0a 2020 2020 666f  us': []}..    fo
-0000e5c0: 7220 656e 7472 7920 696e 2072 6573 706f  r entry in respo
-0000e5d0: 6e73 653a 0a20 2020 2020 2020 2069 6620  nse:.        if 
-0000e5e0: 6c65 6e28 656e 7472 7929 203c 2032 3a0a  len(entry) < 2:.
-0000e5f0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-0000e600: 696e 7565 0a20 2020 2020 2020 2072 6f77  inue.        row
-0000e610: 203d 2065 6e74 7279 5b31 5d0a 2020 2020   = entry[1].    
-0000e620: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
-0000e630: 7461 6e63 6528 726f 772c 2064 6963 7429  tance(row, dict)
-0000e640: 206f 7220 2753 7461 7475 7327 206e 6f74   or 'Status' not
-0000e650: 2069 6e20 726f 773a 0a20 2020 2020 2020   in row:.       
-0000e660: 2020 2020 2063 6f6e 7469 6e75 650a 0a20       continue.. 
-0000e670: 2020 2020 2020 2064 6174 615b 2754 696d         data['Tim
-0000e680: 6527 5d2e 6170 7065 6e64 2874 6f5f 7469  e'].append(to_ti
-0000e690: 6d65 6465 6c74 6128 656e 7472 795b 305d  medelta(entry[0]
-0000e6a0: 2929 0a20 2020 2020 2020 2064 6174 615b  )).        data[
-0000e6b0: 2753 7461 7475 7327 5d2e 6170 7065 6e64  'Status'].append
-0000e6c0: 2872 6f77 5b27 5374 6174 7573 275d 290a  (row['Status']).
-0000e6d0: 0a20 2020 2072 6574 7572 6e20 6461 7461  .    return data
-0000e6e0: 0a0a 0a40 4361 6368 652e 6170 695f 7265  ...@Cache.api_re
-0000e6f0: 7175 6573 745f 7772 6170 7065 720a 6465  quest_wrapper.de
-0000e700: 6620 7261 6365 5f63 6f6e 7472 6f6c 5f6d  f race_control_m
-0000e710: 6573 7361 6765 7328 7061 7468 2c20 7265  essages(path, re
-0000e720: 7370 6f6e 7365 3d4e 6f6e 652c 206c 6976  sponse=None, liv
-0000e730: 6564 6174 613d 4e6f 6e65 293a 0a20 2020  edata=None):.   
-0000e740: 2022 2222 0a20 2020 202e 2e20 7761 726e   """.    .. warn
-0000e750: 696e 673a 3a0a 2020 2020 2020 2020 3a6d  ing::.        :m
-0000e760: 6f64 3a60 6661 7374 6631 2e61 7069 6020  od:`fastf1.api` 
-0000e770: 7769 6c6c 2062 6520 636f 6e73 6964 6572  will be consider
-0000e780: 6564 2070 7269 7661 7465 2069 6e20 6675  ed private in fu
-0000e790: 7475 7265 2072 656c 6561 7365 7320 616e  ture releases an
-0000e7a0: 640a 2020 2020 2020 2020 706f 7465 6e74  d.        potent
-0000e7b0: 6961 6c6c 7920 6265 2072 656d 6f76 6564  ially be removed
-0000e7c0: 206f 7220 6368 616e 6765 642e 0a0a 2020   or changed...  
-0000e7d0: 2020 4665 7463 6820 616e 6420 7061 7273    Fetch and pars
-0000e7e0: 6520 7261 6365 2063 6f6e 7472 6f6c 206d  e race control m
-0000e7f0: 6573 7361 6765 732e 0a0a 2020 2020 5261  essages...    Ra
-0000e800: 6365 2063 6f6e 7472 6f6c 206d 6573 7361  ce control messa
-0000e810: 6765 7320 6172 6520 7365 6e74 2062 7920  ges are sent by 
-0000e820: 7261 6365 2063 6f6e 7472 6f6c 2074 6f20  race control to 
-0000e830: 616c 6c20 7465 616d 7320 746f 206e 6f74  all teams to not
-0000e840: 6966 7920 6f66 0a20 2020 2064 6563 6973  ify of.    decis
-0000e850: 696f 6e73 2061 6e64 2073 7461 7475 7365  ions and statuse
-0000e860: 7320 6f66 2074 6865 2073 6573 7369 6f6e  s of the session
-0000e870: 2e0a 0a20 2020 2045 7665 7279 206d 6573  ...    Every mes
-0000e880: 7361 6765 2068 6173 2074 6865 2066 6f6c  sage has the fol
-0000e890: 6c6f 7769 6e67 2061 7474 7269 6275 7465  lowing attribute
-0000e8a0: 733a 0a0a 2020 2020 2020 2020 2d20 5574  s:..        - Ut
-0000e8b0: 633a 204d 6573 7361 6765 2074 696d 6573  c: Message times
-0000e8c0: 7461 6d70 0a20 2020 2020 2020 202d 2043  tamp.        - C
-0000e8d0: 6174 6567 6f72 7920 2873 7472 293a 2054  ategory (str): T
-0000e8e0: 7970 6520 6f66 206d 6573 7361 6765 2c20  ype of message, 
-0000e8f0: 224f 7468 6572 222c 2022 466c 6167 222c  "Other", "Flag",
-0000e900: 2022 4472 7322 2c20 2243 6172 4576 656e   "Drs", "CarEven
-0000e910: 7422 0a20 2020 2020 2020 202d 204d 6573  t".        - Mes
-0000e920: 7361 6765 2028 7374 7229 3a20 436f 6e74  sage (str): Cont
-0000e930: 656e 7420 6f66 206d 6573 7361 6765 0a0a  ent of message..
-0000e940: 2020 2020 4f74 6865 7220 706f 7373 6962      Other possib
-0000e950: 6c65 2061 7474 7269 6275 7465 7320 6172  le attributes ar
-0000e960: 653a 0a0a 2020 2020 2020 2020 2d20 5374  e:..        - St
-0000e970: 6174 7573 2028 7374 7229 3a20 5374 6174  atus (str): Stat
-0000e980: 7573 206f 6620 636f 6e74 6578 742c 2065  us of context, e
-0000e990: 2e67 2e20 2244 4953 4142 4c45 4422 2066  .g. "DISABLED" f
-0000e9a0: 6f72 2064 6973 6162 6c69 6e67 2044 5253  or disabling DRS
-0000e9b0: 0a20 2020 2020 2020 202d 2046 6c61 6720  .        - Flag 
-0000e9c0: 2873 7472 293a 2054 7970 6520 6f66 2066  (str): Type of f
-0000e9d0: 6c61 6720 6265 696e 6720 7761 7665 6420  lag being waved 
-0000e9e0: 2247 5245 454e 222c 2022 5245 4422 2c20  "GREEN", "RED", 
-0000e9f0: 2259 454c 4c4f 5722 2c0a 2020 2020 2020  "YELLOW",.      
-0000ea00: 2020 2020 2243 4c45 4152 222c 2022 4348      "CLEAR", "CH
-0000ea10: 4551 5545 5245 4422 0a20 2020 2020 2020  EQUERED".       
-0000ea20: 202d 2053 636f 7065 2028 7374 7229 3a20   - Scope (str): 
-0000ea30: 5363 6f70 6520 6f66 206d 6573 7361 6765  Scope of message
-0000ea40: 2022 5472 6163 6b22 2c20 2253 6563 746f   "Track", "Secto
-0000ea50: 7222 2c20 2244 7269 7665 7222 0a20 2020  r", "Driver".   
-0000ea60: 2020 2020 202d 2053 6563 746f 7220 2869       - Sector (i
-0000ea70: 6e74 293a 2041 6666 6563 7465 6420 7472  nt): Affected tr
-0000ea80: 6163 6b20 7365 6374 6f72 2066 6f72 2073  ack sector for s
-0000ea90: 6563 746f 722d 7363 6f70 6564 206d 6573  ector-scoped mes
-0000eaa0: 7361 6765 730a 2020 2020 2020 2020 2d20  sages.        - 
-0000eab0: 5261 6369 6e67 4e75 6d62 6572 2028 7374  RacingNumber (st
-0000eac0: 7229 3a20 4166 6665 6374 6564 2064 7269  r): Affected dri
-0000ead0: 7665 7220 666f 7220 4361 7245 7665 6e74  ver for CarEvent
-0000eae0: 206d 6573 7361 6765 730a 2020 2020 2020   messages.      
-0000eaf0: 2020 2d20 4c61 7020 2869 6e74 293a 204e    - Lap (int): N
-0000eb00: 756d 6265 7220 6f66 2074 6865 206c 6170  umber of the lap
-0000eb10: 2069 6e20 7768 6963 6820 7468 6520 6d65   in which the me
-0000eb20: 7373 6167 6520 7761 7320 6469 7370 6c61  ssage was displa
-0000eb30: 7965 640a 0a20 2020 2041 7267 733a 0a20  yed..    Args:. 
-0000eb40: 2020 2020 2020 2070 6174 6820 2873 7472         path (str
-0000eb50: 293a 2061 7069 2070 6174 6820 6261 7365  ): api path base
-0000eb60: 2073 7472 696e 6720 2875 7375 616c 6c79   string (usually
-0000eb70: 2060 6053 6573 7369 6f6e 2e61 7069 5f70   ``Session.api_p
-0000eb80: 6174 6860 6029 0a20 2020 2020 2020 2072  ath``).        r
-0000eb90: 6573 706f 6e73 653a 2052 6573 706f 6e73  esponse: Respons
-0000eba0: 6520 6173 2072 6574 7572 6e65 6420 6279  e as returned by
-0000ebb0: 203a 6675 6e63 3a60 6665 7463 685f 7061   :func:`fetch_pa
-0000ebc0: 6765 6020 6361 6e20 6265 2070 6173 7365  ge` can be passe
-0000ebd0: 6420 6966 0a20 2020 2020 2020 2020 2020  d if.           
-0000ebe0: 2069 7420 7761 7320 646f 776e 6c6f 6164   it was download
-0000ebf0: 6564 2061 6c72 6561 6479 2e0a 2020 2020  ed already..    
-0000ec00: 2020 2020 6c69 7665 6461 7461 3a20 416e      livedata: An
-0000ec10: 2069 6e73 7461 6e63 6520 6f66 0a20 2020   instance of.   
-0000ec20: 2020 2020 2020 2020 203a 636c 6173 733a           :class:
-0000ec30: 6066 6173 7466 312e 6c69 7665 7469 6d69  `fastf1.livetimi
-0000ec40: 6e67 2e64 6174 612e 4c69 7665 5469 6d69  ng.data.LiveTimi
-0000ec50: 6e67 4461 7461 6020 746f 2075 7365 2061  ngData` to use a
-0000ec60: 7320 6120 736f 7572 6365 0a20 2020 2020  s a source.     
-0000ec70: 2020 2020 2020 2069 6e73 7465 6164 206f         instead o
-0000ec80: 6620 7468 6520 6170 690a 0a20 2020 2052  f the api..    R
-0000ec90: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-0000eca0: 4120 6469 6374 696f 6e61 7279 2063 6f6e  A dictionary con
-0000ecb0: 7461 696e 696e 6720 6f6e 6520 6b65 7920  taining one key 
-0000ecc0: 666f 7220 6561 6368 2064 6174 6120 6368  for each data ch
-0000ecd0: 616e 6e65 6c20 616e 6420 6120 6c69 7374  annel and a list
-0000ece0: 206f 660a 2020 2020 2020 2020 7661 6c75   of.        valu
-0000ecf0: 6573 2070 6572 206b 6579 2e0a 0a20 2020  es per key...   
-0000ed00: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
-0000ed10: 2053 6573 7369 6f6e 4e6f 7441 7661 696c   SessionNotAvail
-0000ed20: 6162 6c65 4572 726f 723a 2069 6e20 6361  ableError: in ca
-0000ed30: 7365 2074 6865 2046 3120 6c69 7665 7469  se the F1 liveti
-0000ed40: 6d69 6e67 2061 7069 2072 6574 7572 6e73  ming api returns
-0000ed50: 206e 6f20 6461 7461 0a20 2020 2022 2222   no data.    """
-0000ed60: 0a20 2020 2069 6620 6c69 7665 6461 7461  .    if livedata
-0000ed70: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-0000ed80: 206c 6976 6564 6174 612e 6861 7328 2752   livedata.has('R
-0000ed90: 6163 6543 6f6e 7472 6f6c 4d65 7373 6167  aceControlMessag
-0000eda0: 6573 2729 3a0a 2020 2020 2020 2020 2320  es'):.        # 
-0000edb0: 646f 6573 206e 6f74 206e 6565 6420 616e  does not need an
-0000edc0: 7920 6675 7274 6865 7220 7072 6f63 6573  y further proces
-0000edd0: 7369 6e67 0a20 2020 2020 2020 205f 6c6f  sing.        _lo
-0000ede0: 6767 6572 2e69 6e66 6f28 224c 6f61 6469  gger.info("Loadi
-0000edf0: 6e67 2072 6163 6520 636f 6e74 726f 6c20  ng race control 
-0000ee00: 6d65 7373 6167 6573 2229 0a20 2020 2020  messages").     
-0000ee10: 2020 2072 6574 7572 6e20 6c69 7665 6461     return liveda
-0000ee20: 7461 2e67 6574 2827 5261 6365 436f 6e74  ta.get('RaceCont
-0000ee30: 726f 6c4d 6573 7361 6765 7327 290a 2020  rolMessages').  
-0000ee40: 2020 656c 6966 2072 6573 706f 6e73 6520    elif response 
-0000ee50: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0000ee60: 205f 6c6f 6767 6572 2e69 6e66 6f28 2246   _logger.info("F
-0000ee70: 6574 6368 696e 6720 7261 6365 2063 6f6e  etching race con
-0000ee80: 7472 6f6c 206d 6573 7361 6765 732e 2e2e  trol messages...
-0000ee90: 2229 0a20 2020 2020 2020 2072 6573 706f  ").        respo
-0000eea0: 6e73 6520 3d20 6665 7463 685f 7061 6765  nse = fetch_page
-0000eeb0: 2870 6174 682c 2027 7261 6365 5f63 6f6e  (path, 'race_con
-0000eec0: 7472 6f6c 5f6d 6573 7361 6765 7327 290a  trol_messages').
-0000eed0: 2020 2020 2020 2020 6966 2072 6573 706f          if respo
-0000eee0: 6e73 6520 6973 204e 6f6e 653a 2020 2320  nse is None:  # 
-0000eef0: 6e6f 2072 6573 706f 6e73 6520 7265 6365  no response rece
-0000ef00: 6976 6564 0a20 2020 2020 2020 2020 2020  ived.           
-0000ef10: 2072 6169 7365 2053 6573 7369 6f6e 4e6f   raise SessionNo
-0000ef20: 7441 7661 696c 6162 6c65 4572 726f 7228  tAvailableError(
-0000ef30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ef40: 2022 4e6f 2064 6174 6120 666f 7220 7468   "No data for th
-0000ef50: 6973 2073 6573 7369 6f6e 2120 4966 2074  is session! If t
-0000ef60: 6869 7320 7365 7373 696f 6e20 6f6e 6c79  his session only
-0000ef70: 2066 696e 6973 6865 6420 220a 2020 2020   finished ".    
-0000ef80: 2020 2020 2020 2020 2020 2020 2272 6563              "rec
-0000ef90: 656e 746c 792c 2070 6c65 6173 6520 7472  ently, please tr
-0000efa0: 7920 6167 6169 6e20 696e 2061 2066 6577  y again in a few
-0000efb0: 206d 696e 7574 6573 2e22 0a20 2020 2020   minutes.".     
-0000efc0: 2020 2020 2020 2029 0a0a 2020 2020 6461         )..    da
-0000efd0: 7461 203d 207b 0a20 2020 2020 2020 2027  ta = {.        '
-0000efe0: 5469 6d65 273a 205b 5d2c 2027 4361 7465  Time': [], 'Cate
-0000eff0: 676f 7279 273a 205b 5d2c 2027 4d65 7373  gory': [], 'Mess
-0000f000: 6167 6527 3a20 5b5d 2c20 2753 7461 7475  age': [], 'Statu
-0000f010: 7327 3a20 5b5d 2c0a 2020 2020 2020 2020  s': [],.        
-0000f020: 2746 6c61 6727 3a20 5b5d 2c20 2753 636f  'Flag': [], 'Sco
-0000f030: 7065 273a 205b 5d2c 2027 5365 6374 6f72  pe': [], 'Sector
-0000f040: 273a 205b 5d2c 2027 5261 6369 6e67 4e75  ': [], 'RacingNu
-0000f050: 6d62 6572 273a 205b 5d2c 2027 4c61 7027  mber': [], 'Lap'
-0000f060: 3a20 5b5d 0a20 2020 207d 0a20 2020 2064  : [].    }.    d
-0000f070: 6174 615f 6b65 7973 203d 2028 2743 6174  ata_keys = ('Cat
-0000f080: 6567 6f72 7927 2c20 274d 6573 7361 6765  egory', 'Message
-0000f090: 272c 2027 5374 6174 7573 272c 2027 466c  ', 'Status', 'Fl
-0000f0a0: 6167 272c 2027 5363 6f70 6527 2c20 2753  ag', 'Scope', 'S
-0000f0b0: 6563 746f 7227 2c0a 2020 2020 2020 2020  ector',.        
-0000f0c0: 2020 2020 2020 2020 2027 5261 6369 6e67           'Racing
-0000f0d0: 4e75 6d62 6572 272c 2027 4c61 7027 290a  Number', 'Lap').
-0000f0e0: 2020 2020 636f 6e76 6572 7465 7273 203d      converters =
-0000f0f0: 2028 7374 722c 2073 7472 2c20 7374 722c   (str, str, str,
-0000f100: 2073 7472 2c20 7374 722c 2069 6e74 2c20   str, str, int, 
-0000f110: 7374 722c 2069 6e74 290a 0a20 2020 2066  str, int)..    f
-0000f120: 6f72 206c 696e 6520 696e 2072 6573 706f  or line in respo
-0000f130: 6e73 653a 0a20 2020 2020 2020 206d 6573  nse:.        mes
-0000f140: 7361 6765 7320 3d20 6c69 6e65 5b31 5d5b  sages = line[1][
-0000f150: 274d 6573 7361 6765 7327 5d0a 2020 2020  'Messages'].    
-0000f160: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-0000f170: 6528 6d65 7373 6167 6573 2c20 6469 6374  e(messages, dict
-0000f180: 293a 0a20 2020 2020 2020 2020 2020 206d  ):.            m
-0000f190: 6573 7361 6765 7320 3d20 6c69 7374 286d  essages = list(m
-0000f1a0: 6573 7361 6765 732e 7661 6c75 6573 2829  essages.values()
-0000f1b0: 290a 2020 2020 2020 2020 666f 7220 656e  ).        for en
-0000f1c0: 7472 7920 696e 206d 6573 7361 6765 733a  try in messages:
-0000f1d0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-0000f1e0: 615b 2754 696d 6527 5d2e 6170 7065 6e64  a['Time'].append
-0000f1f0: 2874 6f5f 6461 7465 7469 6d65 2865 6e74  (to_datetime(ent
-0000f200: 7279 5b27 5574 6327 5d29 290a 0a20 2020  ry['Utc']))..   
-0000f210: 2020 2020 2020 2020 2066 6f72 206b 6579           for key
-0000f220: 2c20 636f 6e76 2069 6e20 7a69 7028 6461  , conv in zip(da
-0000f230: 7461 5f6b 6579 732c 2063 6f6e 7665 7274  ta_keys, convert
-0000f240: 6572 7329 3a0a 2020 2020 2020 2020 2020  ers):.          
-0000f250: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-0000f260: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000f270: 6174 615b 6b65 795d 2e61 7070 656e 6428  ata[key].append(
-0000f280: 636f 6e76 2865 6e74 7279 5b6b 6579 5d29  conv(entry[key])
-0000f290: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000f2a0: 2020 6578 6365 7074 2028 4b65 7945 7272    except (KeyErr
-0000f2b0: 6f72 2c20 5661 6c75 6545 7272 6f72 293a  or, ValueError):
-0000f2c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f2d0: 2020 2020 2023 2074 7970 6520 636f 6e76       # type conv
-0000f2e0: 6572 7369 6f6e 2066 6169 6c65 6420 6f72  ersion failed or
-0000f2f0: 206b 6579 2069 7320 6d69 7373 696e 670a   key is missing.
-0000f300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f310: 2020 2020 6461 7461 5b6b 6579 5d2e 6170      data[key].ap
-0000f320: 7065 6e64 284e 6f6e 6529 0a0a 2020 2020  pend(None)..    
-0000f330: 7265 7475 726e 2064 6174 610a 0a0a 4043  return data...@C
-0000f340: 6163 6865 2e61 7069 5f72 6571 7565 7374  ache.api_request
-0000f350: 5f77 7261 7070 6572 0a64 6566 206c 6170  _wrapper.def lap
-0000f360: 5f63 6f75 6e74 2870 6174 682c 2072 6573  _count(path, res
-0000f370: 706f 6e73 653d 4e6f 6e65 2c20 6c69 7665  ponse=None, live
-0000f380: 6461 7461 3d4e 6f6e 6529 3a0a 2020 2020  data=None):.    
-0000f390: 2222 220a 2020 2020 2e2e 2077 6172 6e69  """.    .. warni
-0000f3a0: 6e67 3a3a 0a20 2020 2020 2020 203a 6d6f  ng::.        :mo
-0000f3b0: 643a 6066 6173 7466 312e 6170 6960 2077  d:`fastf1.api` w
-0000f3c0: 696c 6c20 6265 2063 6f6e 7369 6465 7265  ill be considere
-0000f3d0: 6420 7072 6976 6174 6520 696e 2066 7574  d private in fut
-0000f3e0: 7572 6520 7265 6c65 6173 6573 2061 6e64  ure releases and
-0000f3f0: 0a20 2020 2020 2020 2070 6f74 656e 7469  .        potenti
-0000f400: 616c 6c79 2062 6520 7265 6d6f 7665 6420  ally be removed 
-0000f410: 6f72 2063 6861 6e67 6564 2e0a 0a20 2020  or changed...   
-0000f420: 2046 6574 6368 2061 6e64 2070 6172 7365   Fetch and parse
-0000f430: 206c 6170 2063 6f75 6e74 2064 6174 612e   lap count data.
-0000f440: 0a0a 2020 2020 4974 2070 726f 7669 6465  ..    It provide
-0000f450: 7320 7468 6520 666f 6c6c 6f77 696e 6720  s the following 
-0000f460: 6461 7461 2063 6861 6e6e 656c 7320 7065  data channels pe
-0000f470: 7220 7361 6d70 6c65 3a0a 2020 2020 2020  r sample:.      
-0000f480: 2020 2d20 5469 6d65 3a20 7365 7373 696f    - Time: sessio
-0000f490: 6e20 7469 6d65 7374 616d 7020 2874 696d  n timestamp (tim
-0000f4a0: 6520 6f6e 6c79 290a 2020 2020 2020 2020  e only).        
-0000f4b0: 2d20 546f 7461 6c4c 6170 7320 2869 6e74  - TotalLaps (int
-0000f4c0: 293a 2049 6e74 656e 6465 6420 6e75 6d62  ): Intended numb
-0000f4d0: 6572 206f 6620 746f 7461 6c20 6c61 7073  er of total laps
-0000f4e0: 0a20 2020 2020 2020 202d 2043 7572 7265  .        - Curre
-0000f4f0: 6e74 4c61 7020 2869 6e74 293a 2043 7572  ntLap (int): Cur
-0000f500: 7265 6e74 2072 6163 6520 6c61 700a 0a20  rent race lap.. 
-0000f510: 2020 2041 2076 616c 7565 2063 616e 2068     A value can h
-0000f520: 6176 6520 626f 7468 2027 546f 7461 6c4c  ave both 'TotalL
-0000f530: 6170 7327 2061 6e64 2027 4375 7272 656e  aps' and 'Curren
-0000f540: 744c 6170 2720 6f72 206f 6e6c 7920 6f6e  tLap' or only on
-0000f550: 6520 6f66 2074 6865 6d2e 0a0a 2020 2020  e of them...    
-0000f560: 4120 6e65 7720 7661 6c75 6520 6973 2073  A new value is s
-0000f570: 656e 7420 6576 6572 7920 7469 6d65 2061  ent every time a
-0000f580: 206c 6170 2069 7320 636f 6d70 6c65 7465   lap is complete
-0000f590: 6420 6f72 0a20 2020 2074 6865 2069 6e74  d or.    the int
-0000f5a0: 656e 6465 6420 6e75 6d62 6572 206f 6620  ended number of 
-0000f5b0: 6c61 7073 2063 6861 6e67 6573 2e0a 0a20  laps changes... 
-0000f5c0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-0000f5d0: 2070 6174 6820 2873 7472 293a 2061 7069   path (str): api
-0000f5e0: 2070 6174 6820 6261 7365 2073 7472 696e   path base strin
-0000f5f0: 6720 2875 7375 616c 6c79 2060 6053 6573  g (usually ``Ses
-0000f600: 7369 6f6e 2e61 7069 5f70 6174 6860 6029  sion.api_path``)
-0000f610: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
-0000f620: 653a 2052 6573 706f 6e73 6520 6173 2072  e: Response as r
-0000f630: 6574 7572 6e65 6420 6279 203a 6675 6e63  eturned by :func
-0000f640: 3a60 6665 7463 685f 7061 6765 6020 6361  :`fetch_page` ca
-0000f650: 6e20 6265 2070 6173 7365 6420 6966 0a20  n be passed if. 
-0000f660: 2020 2020 2020 2020 2020 2069 7420 7761             it wa
-0000f670: 7320 646f 776e 6c6f 6164 6564 2061 6c72  s downloaded alr
-0000f680: 6561 6479 2e0a 2020 2020 2020 2020 6c69  eady..        li
-0000f690: 7665 6461 7461 3a20 416e 2069 6e73 7461  vedata: An insta
-0000f6a0: 6e63 6520 6f66 0a20 2020 2020 2020 2020  nce of.         
-0000f6b0: 2020 203a 636c 6173 733a 6066 6173 7466     :class:`fastf
-0000f6c0: 312e 6c69 7665 7469 6d69 6e67 2e64 6174  1.livetiming.dat
-0000f6d0: 612e 4c69 7665 5469 6d69 6e67 4461 7461  a.LiveTimingData
-0000f6e0: 6020 746f 2075 7365 2061 7320 6120 736f  ` to use as a so
-0000f6f0: 7572 6365 0a20 2020 2020 2020 2020 2020  urce.           
-0000f700: 2069 6e73 7465 6164 206f 6620 7468 6520   instead of the 
-0000f710: 6170 690a 0a20 2020 2052 6574 7572 6e73  api..    Returns
-0000f720: 3a0a 2020 2020 2020 2020 4120 6469 6374  :.        A dict
-0000f730: 696f 6e61 7279 2063 6f6e 7461 696e 696e  ionary containin
-0000f740: 6720 6f6e 6520 6b65 7920 666f 7220 6561  g one key for ea
-0000f750: 6368 2064 6174 6120 6368 616e 6e65 6c20  ch data channel 
-0000f760: 616e 6420 6120 6c69 7374 206f 660a 2020  and a list of.  
-0000f770: 2020 2020 2020 7661 6c75 6573 2070 6572        values per
-0000f780: 206b 6579 2e0a 0a20 2020 2052 6169 7365   key...    Raise
-0000f790: 733a 0a20 2020 2020 2020 2053 6573 7369  s:.        Sessi
-0000f7a0: 6f6e 4e6f 7441 7661 696c 6162 6c65 4572  onNotAvailableEr
-0000f7b0: 726f 723a 2069 6e20 6361 7365 2074 6865  ror: in case the
-0000f7c0: 2046 3120 6c69 7665 7469 6d69 6e67 2061   F1 livetiming a
-0000f7d0: 7069 2072 6574 7572 6e73 206e 6f20 6461  pi returns no da
-0000f7e0: 7461 0a20 2020 2022 2222 0a20 2020 2069  ta.    """.    i
-0000f7f0: 6620 6c69 7665 6461 7461 2069 7320 6e6f  f livedata is no
-0000f800: 7420 4e6f 6e65 2061 6e64 206c 6976 6564  t None and lived
-0000f810: 6174 612e 6861 7328 274c 6170 436f 756e  ata.has('LapCoun
-0000f820: 7427 293a 0a20 2020 2020 2020 2023 2064  t'):.        # d
-0000f830: 6f65 7320 6e6f 7420 6e65 6564 2061 6e79  oes not need any
-0000f840: 2066 7572 7468 6572 2070 726f 6365 7373   further process
-0000f850: 696e 670a 2020 2020 2020 2020 5f6c 6f67  ing.        _log
-0000f860: 6765 722e 696e 666f 2822 4c6f 6164 696e  ger.info("Loadin
-0000f870: 6720 6c61 7020 636f 756e 7420 6461 7461  g lap count data
-0000f880: 2229 0a20 2020 2020 2020 2072 6573 706f  ").        respo
-0000f890: 6e73 6520 3d20 6c69 7665 6461 7461 2e67  nse = livedata.g
-0000f8a0: 6574 2827 4c61 7043 6f75 6e74 2729 0a20  et('LapCount'). 
-0000f8b0: 2020 2065 6c69 6620 7265 7370 6f6e 7365     elif response
-0000f8c0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0000f8d0: 2020 5f6c 6f67 6765 722e 696e 666f 2822    _logger.info("
-0000f8e0: 4665 7463 6869 6e67 206c 6170 2063 6f75  Fetching lap cou
-0000f8f0: 6e74 2064 6174 612e 2e2e 2229 0a20 2020  nt data...").   
-0000f900: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
-0000f910: 6665 7463 685f 7061 6765 2870 6174 682c  fetch_page(path,
-0000f920: 2027 6c61 705f 636f 756e 7427 290a 2020   'lap_count').  
-0000f930: 2020 2020 2020 6966 2072 6573 706f 6e73        if respons
-0000f940: 6520 6973 204e 6f6e 653a 2020 2320 6e6f  e is None:  # no
-0000f950: 2072 6573 706f 6e73 6520 7265 6365 6976   response receiv
-0000f960: 6564 0a20 2020 2020 2020 2020 2020 2072  ed.            r
-0000f970: 6169 7365 2053 6573 7369 6f6e 4e6f 7441  aise SessionNotA
-0000f980: 7661 696c 6162 6c65 4572 726f 7228 0a20  vailableError(. 
-0000f990: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000f9a0: 4e6f 2064 6174 6120 666f 7220 7468 6973  No data for this
-0000f9b0: 2073 6573 7369 6f6e 2120 4966 2074 6869   session! If thi
-0000f9c0: 7320 7365 7373 696f 6e20 6f6e 6c79 2066  s session only f
-0000f9d0: 696e 6973 6865 6420 220a 2020 2020 2020  inished ".      
-0000f9e0: 2020 2020 2020 2020 2020 2272 6563 656e            "recen
-0000f9f0: 746c 792c 2070 6c65 6173 6520 7472 7920  tly, please try 
-0000fa00: 6167 6169 6e20 696e 2061 2066 6577 206d  again in a few m
-0000fa10: 696e 7574 6573 2e22 0a20 2020 2020 2020  inutes.".       
-0000fa20: 2020 2020 2029 0a0a 2020 2020 6461 7461       )..    data
-0000fa30: 203d 207b 2754 696d 6527 3a20 5b5d 2c20   = {'Time': [], 
-0000fa40: 2754 6f74 616c 4c61 7073 273a 205b 5d2c  'TotalLaps': [],
-0000fa50: 2027 4375 7272 656e 744c 6170 273a 205b   'CurrentLap': [
-0000fa60: 5d7d 0a20 2020 2064 6174 615f 6b65 7973  ]}.    data_keys
-0000fa70: 203d 2028 2754 6f74 616c 4c61 7073 272c   = ('TotalLaps',
-0000fa80: 2027 4375 7272 656e 744c 6170 2729 0a20   'CurrentLap'). 
-0000fa90: 2020 2063 6f6e 7665 7274 6572 7320 3d20     converters = 
-0000faa0: 2869 6e74 2c20 696e 7429 0a0a 2020 2020  (int, int)..    
-0000fab0: 666f 7220 656e 7472 7920 696e 2072 6573  for entry in res
-0000fac0: 706f 6e73 653a 0a20 2020 2020 2020 2064  ponse:.        d
-0000fad0: 6174 615b 2754 696d 6527 5d2e 6170 7065  ata['Time'].appe
-0000fae0: 6e64 2874 6f5f 7469 6d65 6465 6c74 6128  nd(to_timedelta(
-0000faf0: 656e 7472 795b 305d 2929 0a0a 2020 2020  entry[0]))..    
-0000fb00: 2020 2020 666f 7220 6b65 792c 2063 6f6e      for key, con
-0000fb10: 7620 696e 207a 6970 2864 6174 615f 6b65  v in zip(data_ke
-0000fb20: 7973 2c20 636f 6e76 6572 7465 7273 293a  ys, converters):
-0000fb30: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
-0000fb40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000fb50: 2020 6461 7461 5b6b 6579 5d2e 6170 7065    data[key].appe
-0000fb60: 6e64 2863 6f6e 7628 656e 7472 795b 315d  nd(conv(entry[1]
-0000fb70: 5b6b 6579 5d29 290a 2020 2020 2020 2020  [key])).        
-0000fb80: 2020 2020 6578 6365 7074 2028 4b65 7945      except (KeyE
-0000fb90: 7272 6f72 2c20 5661 6c75 6545 7272 6f72  rror, ValueError
-0000fba0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000fbb0: 2020 2023 2074 7970 6520 636f 6e76 6572     # type conver
-0000fbc0: 7369 6f6e 2066 6169 6c65 6420 6f72 206b  sion failed or k
-0000fbd0: 6579 2069 7320 6d69 7373 696e 670a 2020  ey is missing.  
-0000fbe0: 2020 2020 2020 2020 2020 2020 2020 6461                da
-0000fbf0: 7461 5b6b 6579 5d2e 6170 7065 6e64 284e  ta[key].append(N
-0000fc00: 6f6e 6529 0a0a 2020 2020 7265 7475 726e  one)..    return
-0000fc10: 2064 6174 610a 0a0a 4043 6163 6865 2e61   data...@Cache.a
-0000fc20: 7069 5f72 6571 7565 7374 5f77 7261 7070  pi_request_wrapp
-0000fc30: 6572 0a64 6566 2064 7269 7665 725f 696e  er.def driver_in
-0000fc40: 666f 2870 6174 682c 2072 6573 706f 6e73  fo(path, respons
-0000fc50: 653d 4e6f 6e65 2c20 6c69 7665 6461 7461  e=None, livedata
-0000fc60: 3d4e 6f6e 6529 3a0a 2020 2020 2222 220a  =None):.    """.
-0000fc70: 2020 2020 2e2e 2077 6172 6e69 6e67 3a3a      .. warning::
-0000fc80: 0a20 2020 2020 2020 203a 6d6f 643a 6066  .        :mod:`f
-0000fc90: 6173 7466 312e 6170 6960 2077 696c 6c20  astf1.api` will 
-0000fca0: 6265 2063 6f6e 7369 6465 7265 6420 7072  be considered pr
-0000fcb0: 6976 6174 6520 696e 2066 7574 7572 6520  ivate in future 
-0000fcc0: 7265 6c65 6173 6573 2061 6e64 0a20 2020  releases and.   
-0000fcd0: 2020 2020 2070 6f74 656e 7469 616c 6c79       potentially
-0000fce0: 2062 6520 7265 6d6f 7665 6420 6f72 2063   be removed or c
-0000fcf0: 6861 6e67 6564 2e0a 0a20 2020 2046 6574  hanged...    Fet
-0000fd00: 6368 2064 7269 7665 7220 696e 666f 726d  ch driver inform
-0000fd10: 6174 696f 6e2e 0a0a 2020 2020 4472 6976  ation...    Driv
-0000fd20: 6572 2069 6e66 6f72 6d61 7469 6f6e 2063  er information c
-0000fd30: 6f6e 7461 696e 7320 7468 6520 666f 6c6c  ontains the foll
-0000fd40: 6f77 696e 6720 696e 666f 726d 6174 696f  owing informatio
-0000fd50: 6e20 6162 6f75 7420 6561 6368 2064 7269  n about each dri
-0000fd60: 7665 723a 0a0a 2020 2020 2020 2020 605b  ver:..        `[
-0000fd70: 2752 6163 696e 674e 756d 6265 7227 2c20  'RacingNumber', 
-0000fd80: 2742 726f 6164 6361 7374 4e61 6d65 272c  'BroadcastName',
-0000fd90: 2027 4675 6c6c 4e61 6d65 272c 2027 546c   'FullName', 'Tl
-0000fda0: 6127 2c20 274c 696e 6527 2c0a 2020 2020  a', 'Line',.    
-0000fdb0: 2020 2020 2754 6561 6d4e 616d 6527 2c20      'TeamName', 
-0000fdc0: 2754 6561 6d43 6f6c 6f75 7227 2c20 2746  'TeamColour', 'F
-0000fdd0: 6972 7374 4e61 6d65 272c 2027 4c61 7374  irstName', 'Last
-0000fde0: 4e61 6d65 272c 2027 5265 6665 7265 6e63  Name', 'Referenc
-0000fdf0: 6527 2c0a 2020 2020 2020 2020 2748 6561  e',.        'Hea
-0000fe00: 6473 686f 7455 726c 272c 2027 436f 756e  dshotUrl', 'Coun
-0000fe10: 7472 7943 6f64 6527 5d60 0a0a 2020 2020  tryCode']`..    
-0000fe20: 4172 6773 3a0a 2020 2020 2020 2020 7061  Args:.        pa
-0000fe30: 7468 2028 7374 7229 3a20 6170 6920 7061  th (str): api pa
-0000fe40: 7468 2062 6173 6520 7374 7269 6e67 2028  th base string (
-0000fe50: 7573 7561 6c6c 7920 6060 5365 7373 696f  usually ``Sessio
-0000fe60: 6e2e 6170 695f 7061 7468 6060 290a 2020  n.api_path``).  
-0000fe70: 2020 2020 2020 7265 7370 6f6e 7365 3a20        response: 
-0000fe80: 5265 7370 6f6e 7365 2061 7320 7265 7475  Response as retu
-0000fe90: 726e 6564 2062 7920 3a66 756e 633a 6066  rned by :func:`f
-0000fea0: 6574 6368 5f70 6167 6560 0a20 2020 2020  etch_page`.     
-0000feb0: 2020 2020 2020 2063 616e 2062 6520 7061         can be pa
-0000fec0: 7373 6564 2069 6620 6974 2077 6173 2064  ssed if it was d
-0000fed0: 6f77 6e6c 6f61 6465 6420 616c 7265 6164  ownloaded alread
-0000fee0: 792e 0a20 2020 2020 2020 206c 6976 6564  y..        lived
-0000fef0: 6174 613a 2041 6e20 696e 7374 616e 6365  ata: An instance
-0000ff00: 206f 6620 3a63 6c61 7373 3a60 6661 7374   of :class:`fast
-0000ff10: 6631 2e6c 6976 6574 696d 696e 672e 6461  f1.livetiming.da
-0000ff20: 7461 2e4c 6976 6554 696d 696e 6744 6174  ta.LiveTimingDat
-0000ff30: 6160 0a20 2020 2020 2020 2020 2020 2074  a`.            t
-0000ff40: 6f20 7573 6520 6173 2061 2073 6f75 7263  o use as a sourc
-0000ff50: 6520 696e 7374 6561 6420 6f66 2074 6865  e instead of the
-0000ff60: 2061 7069 0a0a 2020 2020 5265 7475 726e   api..    Return
-0000ff70: 733a 0a20 2020 2020 2020 2041 2064 6963  s:.        A dic
-0000ff80: 7469 6f6e 6172 7920 636f 6e74 6169 6e69  tionary containi
-0000ff90: 6e67 206f 6e65 2065 6e74 7279 2066 6f72  ng one entry for
-0000ffa0: 2065 6163 6820 6472 6976 6572 0a20 2020   each driver.   
-0000ffb0: 2020 2020 2077 6974 6820 7468 6520 6472       with the dr
-0000ffc0: 6976 6572 7320 7261 6369 6e67 206e 756d  ivers racing num
-0000ffd0: 6265 7220 6173 206b 6579 0a0a 2020 2020  ber as key..    
-0000ffe0: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
-0000fff0: 5365 7373 696f 6e4e 6f74 4176 6169 6c61  SessionNotAvaila
-00010000: 626c 6545 7272 6f72 3a20 696e 2063 6173  bleError: in cas
-00010010: 6520 7468 6520 4631 206c 6976 6574 696d  e the F1 livetim
-00010020: 696e 6720 6170 6920 7265 7475 726e 7320  ing api returns 
-00010030: 6e6f 2064 6174 610a 2020 2020 2222 220a  no data.    """.
-00010040: 2020 2020 6966 206c 6976 6564 6174 6120      if livedata 
-00010050: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
-00010060: 6c69 7665 6461 7461 2e68 6173 2827 4472  livedata.has('Dr
-00010070: 6976 6572 4c69 7374 2729 3a0a 2020 2020  iverList'):.    
-00010080: 2020 2020 2320 646f 6573 206e 6f74 206e      # does not n
-00010090: 6565 6420 616e 7920 6675 7274 6865 7220  eed any further 
-000100a0: 7072 6f63 6573 7369 6e67 0a20 2020 2020  processing.     
-000100b0: 2020 205f 6c6f 6767 6572 2e69 6e66 6f28     _logger.info(
-000100c0: 224c 6f61 6469 6e67 2064 7269 7665 7220  "Loading driver 
-000100d0: 6c69 7374 2229 0a20 2020 2020 2020 2072  list").        r
-000100e0: 6573 706f 6e73 6520 3d20 6c69 7665 6461  esponse = liveda
-000100f0: 7461 2e67 6574 2827 4472 6976 6572 4c69  ta.get('DriverLi
-00010100: 7374 2729 0a20 2020 2065 6c69 6620 7265  st').    elif re
-00010110: 7370 6f6e 7365 2069 7320 4e6f 6e65 3a0a  sponse is None:.
-00010120: 2020 2020 2020 2020 5f6c 6f67 6765 722e          _logger.
-00010130: 696e 666f 2822 4665 7463 6869 6e67 2064  info("Fetching d
-00010140: 7269 7665 7220 6c69 7374 2e2e 2e22 290a  river list...").
-00010150: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-00010160: 203d 2066 6574 6368 5f70 6167 6528 7061   = fetch_page(pa
-00010170: 7468 2c20 2764 7269 7665 725f 6c69 7374  th, 'driver_list
-00010180: 2729 0a20 2020 2020 2020 2069 6620 7265  ').        if re
-00010190: 7370 6f6e 7365 2069 7320 4e6f 6e65 3a20  sponse is None: 
-000101a0: 2023 206e 6f20 7265 7370 6f6e 7365 2072   # no response r
-000101b0: 6563 6569 7665 640a 2020 2020 2020 2020  eceived.        
-000101c0: 2020 2020 7261 6973 6520 5365 7373 696f      raise Sessio
-000101d0: 6e4e 6f74 4176 6169 6c61 626c 6545 7272  nNotAvailableErr
-000101e0: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-000101f0: 2020 2020 224e 6f20 6461 7461 2066 6f72      "No data for
-00010200: 2074 6869 7320 7365 7373 696f 6e21 2049   this session! I
-00010210: 6620 7468 6973 2073 6573 7369 6f6e 206f  f this session o
-00010220: 6e6c 7920 6669 6e69 7368 6564 2022 0a20  nly finished ". 
-00010230: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00010240: 7265 6365 6e74 6c79 2c20 706c 6561 7365  recently, please
-00010250: 2074 7279 2061 6761 696e 2069 6e20 6120   try again in a 
-00010260: 6665 7720 6d69 6e75 7465 732e 220a 2020  few minutes.".  
-00010270: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00010280: 2064 7269 7665 7273 203d 2063 6f6c 6c65   drivers = colle
-00010290: 6374 696f 6e73 2e64 6566 6175 6c74 6469  ctions.defaultdi
-000102a0: 6374 2864 6963 7429 0a0a 2020 2020 6465  ct(dict)..    de
-000102b0: 6661 756c 745f 6b65 7973 203d 205b 0a20  fault_keys = [. 
-000102c0: 2020 2020 2020 2027 5261 6369 6e67 4e75         'RacingNu
-000102d0: 6d62 6572 272c 2027 4272 6f61 6463 6173  mber', 'Broadcas
-000102e0: 744e 616d 6527 2c20 2746 756c 6c4e 616d  tName', 'FullNam
-000102f0: 6527 2c20 2754 6c61 272c 2027 4c69 6e65  e', 'Tla', 'Line
-00010300: 272c 0a20 2020 2020 2020 2027 5465 616d  ',.        'Team
-00010310: 4e61 6d65 272c 2027 5465 616d 436f 6c6f  Name', 'TeamColo
-00010320: 7572 272c 2027 4669 7273 744e 616d 6527  ur', 'FirstName'
-00010330: 2c20 274c 6173 744e 616d 6527 2c20 2752  , 'LastName', 'R
-00010340: 6566 6572 656e 6365 272c 0a20 2020 2020  eference',.     
-00010350: 2020 2027 4865 6164 7368 6f74 5572 6c27     'HeadshotUrl'
-00010360: 2c20 2743 6f75 6e74 7279 436f 6465 270a  , 'CountryCode'.
-00010370: 2020 2020 5d0a 0a20 2020 2066 6f72 206c      ]..    for l
-00010380: 696e 6520 696e 2072 6573 706f 6e73 653a  ine in response:
-00010390: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-000103a0: 2020 2020 2020 2020 2020 7473 2c20 636f            ts, co
-000103b0: 6e74 656e 7420 3d20 6c69 6e65 0a20 2020  ntent = line.   
-000103c0: 2020 2020 2065 7863 6570 7420 5661 6c75       except Valu
-000103d0: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
-000103e0: 2020 2020 2320 756e 6578 7065 6374 6564      # unexpected
-000103f0: 2064 6174 6120 666f 726d 6174 2c20 696e   data format, in
-00010400: 636f 7272 6563 7420 6e75 6d62 6572 206f  correct number o
-00010410: 6620 7661 6c75 6573 2074 6f20 756e 7061  f values to unpa
-00010420: 636b 0a20 2020 2020 2020 2020 2020 2063  ck.            c
-00010430: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
-00010440: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
-00010450: 6528 636f 6e74 656e 742c 2064 6963 7429  e(content, dict)
-00010460: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
-00010470: 6e74 696e 7565 2020 2320 756e 6578 7065  ntinue  # unexpe
-00010480: 6374 6564 2064 6174 6120 666f 726d 6174  cted data format
-00010490: 0a20 2020 2020 2020 2066 6f72 2064 7276  .        for drv
-000104a0: 5f6e 756d 2c20 7061 7463 6820 696e 2063  _num, patch in c
-000104b0: 6f6e 7465 6e74 2e69 7465 6d73 2829 3a0a  ontent.items():.
-000104c0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-000104d0: 6f74 2069 7369 6e73 7461 6e63 6528 7061  ot isinstance(pa
-000104e0: 7463 682c 2064 6963 7429 3a0a 2020 2020  tch, dict):.    
-000104f0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00010500: 696e 7565 2020 2320 756e 6578 7065 6374  inue  # unexpect
-00010510: 6564 2064 6174 6120 666f 726d 6174 0a20  ed data format. 
-00010520: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-00010530: 6579 2c20 7661 6c20 696e 2070 6174 6368  ey, val in patch
-00010540: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-00010550: 2020 2020 2020 2020 2020 6966 206b 6579            if key
-00010560: 206e 6f74 2069 6e20 6465 6661 756c 745f   not in default_
-00010570: 6b65 7973 3a0a 2020 2020 2020 2020 2020  keys:.          
-00010580: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-00010590: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
-000105a0: 2020 2064 7269 7665 7273 5b64 7276 5f6e     drivers[drv_n
-000105b0: 756d 5d5b 6b65 795d 203d 2076 616c 0a0a  um][key] = val..
-000105c0: 2020 2020 7265 7475 726e 2064 7269 7665      return drive
-000105d0: 7273 0a0a 0a40 4361 6368 652e 6170 695f  rs...@Cache.api_
-000105e0: 7265 7175 6573 745f 7772 6170 7065 720a  request_wrapper.
-000105f0: 6465 6620 7765 6174 6865 725f 6461 7461  def weather_data
-00010600: 2870 6174 682c 2072 6573 706f 6e73 653d  (path, response=
-00010610: 4e6f 6e65 2c20 6c69 7665 6461 7461 3d4e  None, livedata=N
-00010620: 6f6e 6529 3a0a 2020 2020 2222 220a 2020  one):.    """.  
-00010630: 2020 2e2e 2077 6172 6e69 6e67 3a3a 0a20    .. warning::. 
-00010640: 2020 2020 2020 203a 6d6f 643a 6066 6173         :mod:`fas
-00010650: 7466 312e 6170 6960 2077 696c 6c20 6265  tf1.api` will be
-00010660: 2063 6f6e 7369 6465 7265 6420 7072 6976   considered priv
-00010670: 6174 6520 696e 2066 7574 7572 6520 7265  ate in future re
-00010680: 6c65 6173 6573 2061 6e64 0a20 2020 2020  leases and.     
-00010690: 2020 2070 6f74 656e 7469 616c 6c79 2062     potentially b
-000106a0: 6520 7265 6d6f 7665 6420 6f72 2063 6861  e removed or cha
-000106b0: 6e67 6564 2e0a 0a20 2020 2046 6574 6368  nged...    Fetch
-000106c0: 2061 6e64 2070 6172 7365 2077 6561 7468   and parse weath
-000106d0: 6572 2064 6174 612e 0a0a 2020 2020 5765  er data...    We
-000106e0: 6174 6865 7220 6461 7461 2070 726f 7669  ather data provi
-000106f0: 6465 7320 7468 6520 666f 6c6c 6f77 696e  des the followin
-00010700: 6720 6461 7461 2063 6861 6e6e 656c 7320  g data channels 
-00010710: 7065 7220 7361 6d70 6c65 3a0a 0a20 2020  per sample:..   
-00010720: 2020 2020 202d 2054 696d 6520 2864 6174       - Time (dat
-00010730: 6574 696d 652e 7469 6d65 6465 6c74 6129  etime.timedelta)
-00010740: 3a20 7365 7373 696f 6e20 7469 6d65 7374  : session timest
-00010750: 616d 7020 2874 696d 6520 6f6e 6c79 290a  amp (time only).
-00010760: 2020 2020 2020 2020 2d20 4169 7254 656d          - AirTem
-00010770: 7020 2866 6c6f 6174 293a 2041 6972 2074  p (float): Air t
-00010780: 656d 7065 7261 7475 7265 205b c2b0 435d  emperature [..C]
-00010790: 0a20 2020 2020 2020 202d 2048 756d 6964  .        - Humid
-000107a0: 6974 7920 2866 6c6f 6174 293a 2052 656c  ity (float): Rel
-000107b0: 6174 6976 6520 6875 6d69 6469 7479 205b  ative humidity [
-000107c0: 255d 0a20 2020 2020 2020 202d 2050 7265  %].        - Pre
-000107d0: 7373 7572 6520 2866 6c6f 6174 293a 2041  ssure (float): A
-000107e0: 6972 2070 7265 7373 7572 6520 5b6d 6261  ir pressure [mba
-000107f0: 725d 0a20 2020 2020 2020 202d 2052 6169  r].        - Rai
-00010800: 6e66 616c 6c20 2862 6f6f 6c29 3a20 5368  nfall (bool): Sh
-00010810: 6f77 7320 6966 2074 6865 7265 2069 7320  ows if there is 
-00010820: 7261 696e 6661 6c6c 0a20 2020 2020 2020  rainfall.       
-00010830: 202d 2054 7261 636b 5465 6d70 2028 666c   - TrackTemp (fl
-00010840: 6f61 7429 3a20 5472 6163 6b20 7465 6d70  oat): Track temp
-00010850: 6572 6174 7572 6520 5bc2 b043 5d0a 2020  erature [..C].  
-00010860: 2020 2020 2020 2d20 5769 6e64 4469 7265        - WindDire
-00010870: 6374 696f 6e20 2869 6e74 293a 2057 696e  ction (int): Win
-00010880: 6420 6469 7265 6374 696f 6e20 5bc2 b05d  d direction [..]
-00010890: 2028 30c2 b02d 3335 39c2 b029 0a20 2020   (0..-359..).   
-000108a0: 2020 2020 202d 2057 696e 6453 7065 6564       - WindSpeed
-000108b0: 2028 666c 6f61 7429 3a20 5769 6e64 2073   (float): Wind s
-000108c0: 7065 6564 205b 6d2f 735d 0a0a 2020 2020  peed [m/s]..    
-000108d0: 5765 6174 6865 7220 6461 7461 2069 7320  Weather data is 
-000108e0: 7570 6461 7465 6420 6f6e 6365 2070 6572  updated once per
-000108f0: 206d 696e 7574 652e 0a0a 2020 2020 4172   minute...    Ar
-00010900: 6773 3a0a 2020 2020 2020 2020 7061 7468  gs:.        path
-00010910: 2028 7374 7229 3a20 6170 6920 7061 7468   (str): api path
-00010920: 2062 6173 6520 7374 7269 6e67 2028 7573   base string (us
-00010930: 7561 6c6c 7920 6060 5365 7373 696f 6e2e  ually ``Session.
-00010940: 6170 695f 7061 7468 6060 290a 2020 2020  api_path``).    
-00010950: 2020 2020 7265 7370 6f6e 7365 3a20 5265      response: Re
-00010960: 7370 6f6e 7365 2061 7320 7265 7475 726e  sponse as return
-00010970: 6564 2062 7920 3a66 756e 633a 6066 6574  ed by :func:`fet
-00010980: 6368 5f70 6167 6560 2063 616e 0a20 2020  ch_page` can.   
-00010990: 2020 2020 2020 2020 2062 6520 7061 7373           be pass
-000109a0: 6564 2069 6620 6974 2077 6173 2064 6f77  ed if it was dow
-000109b0: 6e6c 6f61 6465 6420 616c 7265 6164 792e  nloaded already.
-000109c0: 0a20 2020 2020 2020 206c 6976 6564 6174  .        livedat
-000109d0: 613a 2041 6e20 696e 7374 616e 6365 206f  a: An instance o
-000109e0: 660a 2020 2020 2020 2020 2020 2020 3a63  f.            :c
-000109f0: 6c61 7373 3a60 6661 7374 6631 2e6c 6976  lass:`fastf1.liv
-00010a00: 6574 696d 696e 672e 6461 7461 2e4c 6976  etiming.data.Liv
-00010a10: 6554 696d 696e 6744 6174 6160 0a20 2020  eTimingData`.   
-00010a20: 2020 2020 2020 2020 2074 6f20 7573 6520           to use 
-00010a30: 6173 2061 2073 6f75 7263 6520 696e 7374  as a source inst
-00010a40: 6561 6420 6f66 2074 6865 2061 7069 0a0a  ead of the api..
-00010a50: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00010a60: 2020 2020 2041 2064 6963 7469 6f6e 6172       A dictionar
-00010a70: 7920 636f 6e74 6169 6e69 6e67 206f 6e65  y containing one
-00010a80: 206b 6579 2066 6f72 2065 6163 6820 6461   key for each da
-00010a90: 7461 2063 6861 6e6e 656c 2061 6e64 2061  ta channel and a
-00010aa0: 206c 6973 740a 2020 2020 2020 2020 6f66   list.        of
-00010ab0: 2076 616c 7565 7320 7065 7220 6b65 792e   values per key.
-00010ac0: 0a0a 2020 2020 5261 6973 6573 3a0a 2020  ..    Raises:.  
-00010ad0: 2020 2020 2020 5365 7373 696f 6e4e 6f74        SessionNot
-00010ae0: 4176 6169 6c61 626c 6545 7272 6f72 3a20  AvailableError: 
-00010af0: 696e 2063 6173 6520 7468 6520 4631 206c  in case the F1 l
-00010b00: 6976 6520 7469 6d69 6e67 2061 7069 0a20  ive timing api. 
-00010b10: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00010b20: 6e73 206e 6f20 6461 7461 0a20 2020 2022  ns no data.    "
-00010b30: 2222 0a20 2020 2069 6620 6c69 7665 6461  "".    if liveda
-00010b40: 7461 2069 7320 6e6f 7420 4e6f 6e65 2061  ta is not None a
-00010b50: 6e64 206c 6976 6564 6174 612e 6861 7328  nd livedata.has(
-00010b60: 2757 6561 7468 6572 4461 7461 2729 3a0a  'WeatherData'):.
-00010b70: 2020 2020 2020 2020 2320 646f 6573 206e          # does n
-00010b80: 6f74 206e 6565 6420 616e 7920 6675 7274  ot need any furt
-00010b90: 6865 7220 7072 6f63 6573 7369 6e67 0a20  her processing. 
-00010ba0: 2020 2020 2020 205f 6c6f 6767 6572 2e69         _logger.i
-00010bb0: 6e66 6f28 224c 6f61 6469 6e67 2077 6561  nfo("Loading wea
-00010bc0: 7468 6572 2064 6174 6122 290a 2020 2020  ther data").    
-00010bd0: 2020 2020 7265 7370 6f6e 7365 203d 206c      response = l
-00010be0: 6976 6564 6174 612e 6765 7428 2757 6561  ivedata.get('Wea
-00010bf0: 7468 6572 4461 7461 2729 0a20 2020 2065  therData').    e
-00010c00: 6c69 6620 7265 7370 6f6e 7365 2069 7320  lif response is 
-00010c10: 4e6f 6e65 3a0a 2020 2020 2020 2020 5f6c  None:.        _l
-00010c20: 6f67 6765 722e 696e 666f 2822 4665 7463  ogger.info("Fetc
-00010c30: 6869 6e67 2077 6561 7468 6572 2064 6174  hing weather dat
-00010c40: 612e 2e2e 2229 0a20 2020 2020 2020 2072  a...").        r
-00010c50: 6573 706f 6e73 6520 3d20 6665 7463 685f  esponse = fetch_
-00010c60: 7061 6765 2870 6174 682c 2027 7765 6174  page(path, 'weat
-00010c70: 6865 725f 6461 7461 2729 0a20 2020 2020  her_data').     
-00010c80: 2020 2069 6620 7265 7370 6f6e 7365 2069     if response i
-00010c90: 7320 4e6f 6e65 3a20 2023 206e 6f20 7265  s None:  # no re
-00010ca0: 7370 6f6e 7365 2072 6563 6569 7665 640a  sponse received.
-00010cb0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00010cc0: 6520 5365 7373 696f 6e4e 6f74 4176 6169  e SessionNotAvai
-00010cd0: 6c61 626c 6545 7272 6f72 280a 2020 2020  lableError(.    
-00010ce0: 2020 2020 2020 2020 2020 2020 224e 6f20              "No 
-00010cf0: 6461 7461 2066 6f72 2074 6869 7320 7365  data for this se
-00010d00: 7373 696f 6e21 2049 6620 7468 6973 2073  ssion! If this s
-00010d10: 6573 7369 6f6e 206f 6e6c 7920 6669 6e69  ession only fini
-00010d20: 7368 6564 2022 0a20 2020 2020 2020 2020  shed ".         
-00010d30: 2020 2020 2020 2022 7265 6365 6e74 6c79         "recently
-00010d40: 2c20 706c 6561 7365 2074 7279 2061 6761  , please try aga
-00010d50: 696e 2069 6e20 6120 6665 7720 6d69 6e75  in in a few minu
-00010d60: 7465 732e 220a 2020 2020 2020 2020 2020  tes.".          
-00010d70: 2020 290a 0a20 2020 2064 6174 6120 3d20    )..    data = 
-00010d80: 7b0a 2020 2020 2020 2020 2754 696d 6527  {.        'Time'
-00010d90: 3a20 5b5d 2c20 2741 6972 5465 6d70 273a  : [], 'AirTemp':
-00010da0: 205b 5d2c 2027 4875 6d69 6469 7479 273a   [], 'Humidity':
-00010db0: 205b 5d2c 2027 5072 6573 7375 7265 273a   [], 'Pressure':
-00010dc0: 205b 5d2c 0a20 2020 2020 2020 2027 5261   [],.        'Ra
-00010dd0: 696e 6661 6c6c 273a 205b 5d2c 2027 5472  infall': [], 'Tr
-00010de0: 6163 6b54 656d 7027 3a20 5b5d 2c20 2757  ackTemp': [], 'W
-00010df0: 696e 6444 6972 6563 7469 6f6e 273a 205b  indDirection': [
-00010e00: 5d2c 2027 5769 6e64 5370 6565 6427 3a20  ], 'WindSpeed': 
-00010e10: 5b5d 0a20 2020 207d 0a0a 2020 2020 6461  [].    }..    da
-00010e20: 7461 5f6b 6579 7320 3d20 2827 4169 7254  ta_keys = ('AirT
-00010e30: 656d 7027 2c20 2748 756d 6964 6974 7927  emp', 'Humidity'
-00010e40: 2c20 2750 7265 7373 7572 6527 2c20 2752  , 'Pressure', 'R
-00010e50: 6169 6e66 616c 6c27 2c0a 2020 2020 2020  ainfall',.      
-00010e60: 2020 2020 2020 2020 2020 2027 5472 6163             'Trac
-00010e70: 6b54 656d 7027 2c20 2757 696e 6444 6972  kTemp', 'WindDir
-00010e80: 6563 7469 6f6e 272c 2027 5769 6e64 5370  ection', 'WindSp
-00010e90: 6565 6427 290a 2020 2020 636f 6e76 6572  eed').    conver
-00010ea0: 7465 7273 203d 2028 666c 6f61 742c 2066  ters = (float, f
-00010eb0: 6c6f 6174 2c20 666c 6f61 742c 0a20 2020  loat, float,.   
-00010ec0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00010ed0: 616d 6264 6120 763a 2054 7275 6520 6966  ambda v: True if
-00010ee0: 2076 203d 3d20 2731 2720 656c 7365 2046   v == '1' else F
-00010ef0: 616c 7365 2c20 2023 2072 6169 6e3a 2073  alse,  # rain: s
-00010f00: 7472 202d 3e20 626f 6f6c 0a20 2020 2020  tr -> bool.     
-00010f10: 2020 2020 2020 2020 2020 2020 2066 6c6f               flo
-00010f20: 6174 2c20 696e 742c 2066 6c6f 6174 290a  at, int, float).
-00010f30: 0a20 2020 2066 6f72 2065 6e74 7279 2069  .    for entry i
-00010f40: 6e20 7265 7370 6f6e 7365 3a0a 2020 2020  n response:.    
-00010f50: 2020 2020 6966 206c 656e 2865 6e74 7279      if len(entry
-00010f60: 2920 3c20 323a 0a20 2020 2020 2020 2020  ) < 2:.         
-00010f70: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
-00010f80: 2020 2020 726f 7720 3d20 656e 7472 795b      row = entry[
-00010f90: 315d 0a20 2020 2020 2020 2069 6620 6e6f  1].        if no
-00010fa0: 7420 6973 696e 7374 616e 6365 2872 6f77  t isinstance(row
-00010fb0: 2c20 6469 6374 293a 0a20 2020 2020 2020  , dict):.       
-00010fc0: 2020 2020 2063 6f6e 7469 6e75 650a 0a20       continue.. 
-00010fd0: 2020 2020 2020 2064 6174 615b 2754 696d         data['Tim
-00010fe0: 6527 5d2e 6170 7065 6e64 2874 6f5f 7469  e'].append(to_ti
-00010ff0: 6d65 6465 6c74 6128 656e 7472 795b 305d  medelta(entry[0]
-00011000: 2929 0a20 2020 2020 2020 2066 6f72 206b  )).        for k
-00011010: 6579 2c20 636f 6e76 2069 6e20 7a69 7028  ey, conv in zip(
-00011020: 6461 7461 5f6b 6579 732c 2063 6f6e 7665  data_keys, conve
-00011030: 7274 6572 7329 3a0a 2020 2020 2020 2020  rters):.        
-00011040: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00011050: 2020 2020 2020 2020 2064 6174 615b 6b65           data[ke
-00011060: 795d 2e61 7070 656e 6428 636f 6e76 2872  y].append(conv(r
-00011070: 6f77 5b6b 6579 5d29 290a 2020 2020 2020  ow[key])).      
-00011080: 2020 2020 2020 6578 6365 7074 2028 4b65        except (Ke
-00011090: 7945 7272 6f72 2c20 5661 6c75 6545 7272  yError, ValueErr
-000110a0: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
-000110b0: 2020 2020 2023 2074 7970 6520 636f 6e76       # type conv
-000110c0: 6572 7369 6f6e 2066 6169 6c65 6420 6f72  ersion failed or
-000110d0: 206b 6579 2069 7320 6d69 7373 696e 670a   key is missing.
-000110e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110f0: 6461 7461 5b6b 6579 5d2e 6170 7065 6e64  data[key].append
-00011100: 2863 6f6e 7628 3029 290a 0a20 2020 2072  (conv(0))..    r
-00011110: 6574 7572 6e20 6461 7461 0a0a 0a40 4361  eturn data...@Ca
-00011120: 6368 652e 6170 695f 7265 7175 6573 745f  che.api_request_
-00011130: 7772 6170 7065 720a 6465 6620 7365 6173  wrapper.def seas
-00011140: 6f6e 5f73 6368 6564 756c 6528 7061 7468  on_schedule(path
-00011150: 2c20 7265 7370 6f6e 7365 3d4e 6f6e 6529  , response=None)
-00011160: 3a0a 2020 2020 6966 2072 6573 706f 6e73  :.    if respons
-00011170: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
-00011180: 2020 205f 6c6f 6767 6572 2e69 6e66 6f28     _logger.info(
-00011190: 2246 6574 6368 696e 6720 7365 6173 6f6e  "Fetching season
-000111a0: 2073 6368 6564 756c 652e 2e2e 2229 0a20   schedule..."). 
-000111b0: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-000111c0: 3d20 6665 7463 685f 7061 6765 2870 6174  = fetch_page(pat
-000111d0: 682c 2027 696e 6465 7827 290a 2020 2020  h, 'index').    
-000111e0: 2020 2020 6966 2072 6573 706f 6e73 6520      if response 
-000111f0: 6973 204e 6f6e 653a 2020 2320 6e6f 2072  is None:  # no r
-00011200: 6573 706f 6e73 6520 7265 6365 6976 6564  esponse received
-00011210: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00011220: 7365 2053 6573 7369 6f6e 4e6f 7441 7661  se SessionNotAva
-00011230: 696c 6162 6c65 4572 726f 7228 0a20 2020  ilableError(.   
-00011240: 2020 2020 2020 2020 2020 2020 2022 4e6f               "No
-00011250: 2064 6174 6120 666f 7220 7468 6973 2073   data for this s
-00011260: 6573 7369 6f6e 2120 4966 2074 6869 7320  ession! If this 
-00011270: 7365 7373 696f 6e20 6f6e 6c79 2066 696e  session only fin
-00011280: 6973 6865 6420 220a 2020 2020 2020 2020  ished ".        
-00011290: 2020 2020 2020 2020 2272 6563 656e 746c          "recentl
-000112a0: 792c 2070 6c65 6173 6520 7472 7920 6167  y, please try ag
-000112b0: 6169 6e20 696e 2061 2066 6577 206d 696e  ain in a few min
-000112c0: 7574 6573 2e22 0a20 2020 2020 2020 2020  utes.".         
-000112d0: 2020 2029 0a0a 2020 2020 7265 7475 726e     )..    return
-000112e0: 2072 6573 706f 6e73 655b 274d 6565 7469   response['Meeti
-000112f0: 6e67 7327 5d0a 0a0a 4043 6163 6865 2e61  ngs']...@Cache.a
-00011300: 7069 5f72 6571 7565 7374 5f77 7261 7070  pi_request_wrapp
-00011310: 6572 0a64 6566 2073 6573 7369 6f6e 5f69  er.def session_i
-00011320: 6e66 6f28 7061 7468 2c20 7265 7370 6f6e  nfo(path, respon
-00011330: 7365 3d4e 6f6e 652c 206c 6976 6564 6174  se=None, livedat
-00011340: 613d 4e6f 6e65 293a 0a20 2020 2022 2222  a=None):.    """
-00011350: 0a20 2020 202e 2e20 7761 726e 696e 673a  .    .. warning:
-00011360: 3a0a 2020 2020 2020 2020 3a6d 6f64 3a60  :.        :mod:`
-00011370: 6661 7374 6631 2e61 7069 6020 7769 6c6c  fastf1.api` will
-00011380: 2062 6520 636f 6e73 6964 6572 6564 2070   be considered p
-00011390: 7269 7661 7465 2069 6e20 6675 7475 7265  rivate in future
-000113a0: 2072 656c 6561 7365 7320 616e 640a 2020   releases and.  
-000113b0: 2020 2020 2020 706f 7465 6e74 6961 6c6c        potentiall
-000113c0: 7920 6265 2072 656d 6f76 6564 206f 7220  y be removed or 
-000113d0: 6368 616e 6765 642e 0a0a 2020 2020 4665  changed...    Fe
-000113e0: 7463 6820 616e 6420 7061 7273 6520 7365  tch and parse se
-000113f0: 7373 696f 6e20 696e 666f 2064 6174 612e  ssion info data.
-00011400: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
-00011410: 2020 2020 2020 2041 2064 6963 7469 6f6e         A diction
-00011420: 6172 7920 636f 6e74 6169 6e69 6e67 2074  ary containing t
-00011430: 6865 206e 6573 7465 6420 7365 7373 696f  he nested sessio
-00011440: 6e20 696e 666f 2064 6174 612e 2054 696d  n info data. Tim
-00011450: 6573 7461 6d70 7320 616e 640a 2020 2020  estamps and.    
-00011460: 2020 2020 7469 6d65 6465 6c74 6173 2061      timedeltas a
-00011470: 7265 2063 6f6e 7665 7274 6564 2074 6f20  re converted to 
-00011480: 6060 6461 7465 7469 6d65 2e64 6174 6574  ``datetime.datet
-00011490: 696d 6560 6020 616e 640a 2020 2020 2020  ime`` and.      
-000114a0: 2020 6060 6461 7465 7469 6d65 2e74 696d    ``datetime.tim
-000114b0: 6564 656c 7461 6060 2072 6573 7065 6374  edelta`` respect
-000114c0: 6976 656c 792e 0a0a 2020 2020 5261 6973  ively...    Rais
-000114d0: 6573 3a0a 2020 2020 2020 2020 5365 7373  es:.        Sess
-000114e0: 696f 6e4e 6f74 4176 6169 6c61 626c 6545  ionNotAvailableE
-000114f0: 7272 6f72 3a20 696e 2063 6173 6520 7468  rror: in case th
-00011500: 6520 4631 206c 6976 6520 7469 6d69 6e67  e F1 live timing
-00011510: 2061 7069 0a20 2020 2020 2020 2020 2020   api.           
-00011520: 2072 6574 7572 6e73 206e 6f20 6461 7461   returns no data
-00011530: 0a20 2020 2022 2222 0a20 2020 2069 6620  .    """.    if 
-00011540: 6c69 7665 6461 7461 2069 7320 6e6f 7420  livedata is not 
-00011550: 4e6f 6e65 2061 6e64 206c 6976 6564 6174  None and livedat
-00011560: 612e 6861 7328 2753 6573 7369 6f6e 496e  a.has('SessionIn
-00011570: 666f 2729 3a0a 2020 2020 2020 2020 2320  fo'):.        # 
-00011580: 646f 6573 206e 6f74 206e 6565 6420 616e  does not need an
-00011590: 7920 6675 7274 6865 7220 7072 6f63 6573  y further proces
-000115a0: 7369 6e67 0a20 2020 2020 2020 205f 6c6f  sing.        _lo
-000115b0: 6767 6572 2e69 6e66 6f28 224c 6f61 6469  gger.info("Loadi
-000115c0: 6e67 2073 6573 7369 6f6e 2069 6e66 6f20  ng session info 
-000115d0: 6461 7461 2229 0a20 2020 2020 2020 2072  data").        r
-000115e0: 6573 706f 6e73 6520 3d20 6c69 7665 6461  esponse = liveda
-000115f0: 7461 2e67 6574 2827 5365 7373 696f 6e49  ta.get('SessionI
-00011600: 6e66 6f27 290a 2020 2020 656c 6966 2072  nfo').    elif r
-00011610: 6573 706f 6e73 6520 6973 204e 6f6e 653a  esponse is None:
-00011620: 0a20 2020 2020 2020 205f 6c6f 6767 6572  .        _logger
-00011630: 2e69 6e66 6f28 2246 6574 6368 696e 6720  .info("Fetching 
-00011640: 7365 7373 696f 6e20 696e 666f 2064 6174  session info dat
-00011650: 612e 2e2e 2229 0a20 2020 2020 2020 2072  a...").        r
-00011660: 6573 706f 6e73 6520 3d20 6665 7463 685f  esponse = fetch_
-00011670: 7061 6765 2870 6174 682c 2027 7365 7373  page(path, 'sess
-00011680: 696f 6e5f 696e 666f 2729 0a20 2020 2020  ion_info').     
-00011690: 2020 2069 6620 7265 7370 6f6e 7365 2069     if response i
-000116a0: 7320 4e6f 6e65 3a20 2023 206e 6f20 7265  s None:  # no re
-000116b0: 7370 6f6e 7365 2072 6563 6569 7665 640a  sponse received.
-000116c0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000116d0: 6520 5365 7373 696f 6e4e 6f74 4176 6169  e SessionNotAvai
-000116e0: 6c61 626c 6545 7272 6f72 280a 2020 2020  lableError(.    
-000116f0: 2020 2020 2020 2020 2020 2020 224e 6f20              "No 
-00011700: 6461 7461 2066 6f72 2074 6869 7320 7365  data for this se
-00011710: 7373 696f 6e21 2049 6620 7468 6973 2073  ssion! If this s
-00011720: 6573 7369 6f6e 206f 6e6c 7920 6669 6e69  ession only fini
-00011730: 7368 6564 2022 0a20 2020 2020 2020 2020  shed ".         
-00011740: 2020 2020 2020 2022 7265 6365 6e74 6c79         "recently
-00011750: 2c20 706c 6561 7365 2074 7279 2061 6761  , please try aga
-00011760: 696e 2069 6e20 6120 6665 7720 6d69 6e75  in in a few minu
-00011770: 7465 732e 220a 2020 2020 2020 2020 2020  tes.".          
-00011780: 2020 290a 0a20 2020 2074 732c 2064 6174    )..    ts, dat
-00011790: 6120 3d20 7265 7370 6f6e 7365 5b30 5d0a  a = response[0].
-000117a0: 0a20 2020 2064 6174 615b 2753 7461 7274  .    data['Start
-000117b0: 4461 7465 275d 203d 2074 6f5f 6461 7465  Date'] = to_date
-000117c0: 7469 6d65 2864 6174 615b 2753 7461 7274  time(data['Start
-000117d0: 4461 7465 275d 290a 2020 2020 6461 7461  Date']).    data
-000117e0: 5b27 456e 6444 6174 6527 5d20 3d20 746f  ['EndDate'] = to
-000117f0: 5f64 6174 6574 696d 6528 6461 7461 5b27  _datetime(data['
-00011800: 456e 6444 6174 6527 5d29 0a20 2020 2064  EndDate']).    d
-00011810: 6174 615b 2747 6d74 4f66 6673 6574 275d  ata['GmtOffset']
-00011820: 203d 2074 6f5f 7469 6d65 6465 6c74 6128   = to_timedelta(
-00011830: 6461 7461 5b27 476d 744f 6666 7365 7427  data['GmtOffset'
-00011840: 5d29 0a0a 2020 2020 7265 7475 726e 2064  ])..    return d
-00011850: 6174 610a 0a0a 6465 6620 6665 7463 685f  ata...def fetch_
-00011860: 7061 6765 2870 6174 682c 206e 616d 6529  page(path, name)
-00011870: 3a0a 2020 2020 2222 220a 2020 2020 2e2e  :.    """.    ..
-00011880: 2077 6172 6e69 6e67 3a3a 0a20 2020 2020   warning::.     
-00011890: 2020 203a 6d6f 643a 6066 6173 7466 312e     :mod:`fastf1.
-000118a0: 6170 6960 2077 696c 6c20 6265 2063 6f6e  api` will be con
-000118b0: 7369 6465 7265 6420 7072 6976 6174 6520  sidered private 
-000118c0: 696e 2066 7574 7572 6520 7265 6c65 6173  in future releas
-000118d0: 6573 2061 6e64 0a20 2020 2020 2020 2070  es and.        p
-000118e0: 6f74 656e 7469 616c 6c79 2062 6520 7265  otentially be re
-000118f0: 6d6f 7665 6420 6f72 2063 6861 6e67 6564  moved or changed
-00011900: 2e0a 0a20 2020 2046 6574 6368 2064 6174  ...    Fetch dat
-00011910: 6120 6672 6f6d 2074 6865 2066 6f72 6d75  a from the formu
-00011920: 6c61 3120 6c69 7665 7469 6d69 6e67 2077  la1 livetiming w
-00011930: 6562 2061 7069 2c20 6769 7665 6e20 7572  eb api, given ur
-00011940: 6c20 6261 7365 2070 6174 6820 616e 6420  l base path and 
-00011950: 7061 6765 206e 616d 652e 2041 6e20 6174  page name. An at
-00011960: 7465 6d70 740a 2020 2020 746f 2070 6172  tempt.    to par
-00011970: 7365 206a 736f 6e20 6f72 2064 6563 6f64  se json or decod
-00011980: 6520 6b6e 6f77 6e20 6d65 7373 6167 6573  e known messages
-00011990: 2069 7320 6d61 6465 2e0a 0a20 2020 2041   is made...    A
-000119a0: 7267 733a 0a20 2020 2020 2020 2070 6174  rgs:.        pat
-000119b0: 6820 2873 7472 293a 2061 7069 2070 6174  h (str): api pat
-000119c0: 6820 6261 7365 2073 7472 696e 6720 2875  h base string (u
-000119d0: 7375 616c 6c79 2060 6053 6573 7369 6f6e  sually ``Session
-000119e0: 2e61 7069 5f70 6174 6860 6029 0a20 2020  .api_path``).   
-000119f0: 2020 2020 206e 616d 6520 2873 7472 293a       name (str):
-00011a00: 2070 6167 6520 6e61 6d65 2028 7365 6520   page name (see 
-00011a10: 6060 6170 692e 7061 6765 7360 6020 666f  ``api.pages`` fo
-00011a20: 7220 616c 6c20 6b6e 6f77 6e20 7061 6765  r all known page
-00011a30: 7329 0a0a 2020 2020 5265 7475 726e 733a  s)..    Returns:
-00011a40: 0a20 2020 2020 2020 202d 2064 6963 7469  .        - dicti
-00011a50: 6f6e 6172 7920 6966 2063 6f6e 7465 6e74  onary if content
-00011a60: 2077 6173 206a 736f 6e0a 2020 2020 2020   was json.      
-00011a70: 2020 2d20 6c69 7374 206f 6620 656e 7472    - list of entr
-00011a80: 6965 7320 6966 206a 736f 6e53 7472 6561  ies if jsonStrea
-00011a90: 6d2c 2077 6865 7265 2065 6163 6820 656e  m, where each en
-00011aa0: 7472 7920 6167 6169 6e20 636f 6e74 6169  try again contai
-00011ab0: 6e73 2074 776f 2065 6c65 6d65 6e74 733a  ns two elements:
-00011ac0: 205b 7469 6d65 7374 616d 702c 2063 6f6e   [timestamp, con
-00011ad0: 7465 6e74 5d2e 2043 6f6e 7465 6e74 2069  tent]. Content i
-00011ae0: 730a 2020 2020 2020 2020 2020 7061 7273  s.          pars
-00011af0: 6564 2077 6974 6820 3a66 756e 633a 6070  ed with :func:`p
-00011b00: 6172 7365 6020 616e 6420 7769 6c6c 2075  arse` and will u
-00011b10: 7375 616c 6c79 2062 6520 6120 6469 6374  sually be a dict
-00011b20: 696f 6e61 7279 2063 7265 6174 6564 2066  ionary created f
-00011b30: 726f 6d20 6a73 6f6e 2064 6174 612e 0a20  rom json data.. 
-00011b40: 2020 2020 2020 202d 204e 6f6e 6520 6966         - None if
-00011b50: 2072 6571 7565 7374 2066 6169 6c65 640a   request failed.
-00011b60: 0a20 2020 2022 2222 0a20 2020 2070 6167  .    """.    pag
-00011b70: 6520 3d20 7061 6765 735b 6e61 6d65 5d0a  e = pages[name].
-00011b80: 2020 2020 6973 5f73 7472 6561 6d20 3d20      is_stream = 
-00011b90: 276a 736f 6e53 7472 6561 6d27 2069 6e20  'jsonStream' in 
-00011ba0: 7061 6765 0a20 2020 2069 735f 7a20 3d20  page.    is_z = 
-00011bb0: 272e 7a2e 2720 696e 2070 6167 650a 2020  '.z.' in page.  
-00011bc0: 2020 7220 3d20 4361 6368 652e 7265 7175    r = Cache.requ
-00011bd0: 6573 7473 5f67 6574 2862 6173 655f 7572  ests_get(base_ur
-00011be0: 6c20 2b20 7061 7468 202b 2070 6167 6573  l + path + pages
-00011bf0: 5b6e 616d 655d 2c20 6865 6164 6572 733d  [name], headers=
-00011c00: 6865 6164 6572 7329 0a20 2020 2069 6620  headers).    if 
-00011c10: 722e 7374 6174 7573 5f63 6f64 6520 3d3d  r.status_code ==
-00011c20: 2032 3030 3a0a 2020 2020 2020 2020 7261   200:.        ra
-00011c30: 7720 3d20 722e 636f 6e74 656e 742e 6465  w = r.content.de
-00011c40: 636f 6465 2827 7574 662d 382d 7369 6727  code('utf-8-sig'
-00011c50: 290a 2020 2020 2020 2020 6966 2069 735f  ).        if is_
-00011c60: 7374 7265 616d 3a0a 2020 2020 2020 2020  stream:.        
-00011c70: 2020 2020 7265 636f 7264 7320 3d20 7261      records = ra
-00011c80: 772e 7370 6c69 7428 275c 725c 6e27 295b  w.split('\r\n')[
-00011c90: 3a2d 315d 2020 2320 6c61 7374 2073 706c  :-1]  # last spl
-00011ca0: 6974 2069 7320 656d 7074 790a 2020 2020  it is empty.    
-00011cb0: 2020 2020 2020 2020 6966 206e 616d 6520          if name 
-00011cc0: 696e 2028 2770 6f73 6974 696f 6e27 2c20  in ('position', 
-00011cd0: 2763 6172 5f64 6174 6127 293a 0a20 2020  'car_data'):.   
-00011ce0: 2020 2020 2020 2020 2020 2020 2023 2053               # S
-00011cf0: 7065 6369 616c 2063 6173 6520 746f 2069  pecial case to i
-00011d00: 6d70 726f 7665 206d 656d 6f72 7920 6566  mprove memory ef
-00011d10: 6669 6369 656e 6379 0a20 2020 2020 2020  ficiency.       
-00011d20: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00011d30: 7265 636f 7264 730a 2020 2020 2020 2020  records.        
-00011d40: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00011d50: 2020 2020 2020 2020 2020 6465 636f 6465            decode
-00011d60: 5f65 7272 6f72 5f63 6f75 6e74 203d 2030  _error_count = 0
-00011d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011d80: 2074 6c20 3d20 3132 2020 2320 6c65 6e67   tl = 12  # leng
-00011d90: 7468 206f 6620 7469 6d65 7374 616d 703a  th of timestamp:
-00011da0: 206c 656e 2827 3030 3a30 303a 3030 3a30   len('00:00:00:0
-00011db0: 3030 2729 0a20 2020 2020 2020 2020 2020  00').           
-00011dc0: 2020 2020 2072 6574 203d 206c 6973 7428       ret = list(
-00011dd0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00011de0: 2020 666f 7220 6520 696e 2072 6563 6f72    for e in recor
-00011df0: 6473 3a0a 2020 2020 2020 2020 2020 2020  ds:.            
-00011e00: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00011e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e20: 2020 2020 2072 6574 2e61 7070 656e 6428       ret.append(
-00011e30: 5b65 5b3a 746c 5d2c 2070 6172 7365 2865  [e[:tl], parse(e
-00011e40: 5b74 6c3a 5d2c 207a 6970 7065 643d 6973  [tl:], zipped=is
-00011e50: 5f7a 295d 290a 2020 2020 2020 2020 2020  _z)]).          
-00011e60: 2020 2020 2020 2020 2020 6578 6365 7074            except
-00011e70: 206a 736f 6e2e 4a53 4f4e 4465 636f 6465   json.JSONDecode
-00011e80: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
-00011e90: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00011ea0: 6563 6f64 655f 6572 726f 725f 636f 756e  ecode_error_coun
-00011eb0: 7420 2b3d 2031 0a20 2020 2020 2020 2020  t += 1.         
-00011ec0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00011ed0: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
-00011ee0: 2020 2020 2020 2020 6966 2064 6563 6f64          if decod
-00011ef0: 655f 6572 726f 725f 636f 756e 7420 3e20  e_error_count > 
-00011f00: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
-00011f10: 2020 2020 2020 205f 6c6f 6767 6572 2e77         _logger.w
-00011f20: 6172 6e69 6e67 2866 2246 6169 6c65 6420  arning(f"Failed 
-00011f30: 746f 2064 6563 6f64 6520 7b64 6563 6f64  to decode {decod
-00011f40: 655f 6572 726f 725f 636f 756e 747d 220a  e_error_count}".
-00011f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f70: 2020 2020 6622 206d 6573 7361 6765 7320      f" messages 
-00011f80: 287b 6c65 6e28 7265 636f 7264 7329 7d20  ({len(records)} 
-00011f90: 6d65 7373 6167 6573 2022 0a20 2020 2020  messages ".     
-00011fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fb0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00011fc0: 2274 6f74 616c 2922 290a 2020 2020 2020  "total)").      
-00011fd0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00011fe0: 2072 6574 0a20 2020 2020 2020 2065 6c73   ret.        els
-00011ff0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00012000: 6574 7572 6e20 7061 7273 6528 7261 772c  eturn parse(raw,
-00012010: 2069 735f 7a29 0a20 2020 2065 6c73 653a   is_z).    else:
-00012020: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00012030: 4e6f 6e65 0a0a 0a64 6566 2070 6172 7365  None...def parse
-00012040: 2874 6578 743a 2073 7472 2c20 7a69 7070  (text: str, zipp
-00012050: 6564 3a20 626f 6f6c 203d 2046 616c 7365  ed: bool = False
-00012060: 2920 2d3e 2055 6e69 6f6e 5b73 7472 2c20  ) -> Union[str, 
-00012070: 6469 6374 5d3a 0a20 2020 2022 2222 0a20  dict]:.    """. 
-00012080: 2020 202e 2e20 7761 726e 696e 673a 3a0a     .. warning::.
-00012090: 2020 2020 2020 2020 3a6d 6f64 3a60 6661          :mod:`fa
-000120a0: 7374 6631 2e61 7069 6020 7769 6c6c 2062  stf1.api` will b
-000120b0: 6520 636f 6e73 6964 6572 6564 2070 7269  e considered pri
-000120c0: 7661 7465 2069 6e20 6675 7475 7265 2072  vate in future r
-000120d0: 656c 6561 7365 7320 616e 640a 2020 2020  eleases and.    
-000120e0: 2020 2020 706f 7465 6e74 6961 6c6c 7920      potentially 
-000120f0: 6265 2072 656d 6f76 6564 206f 7220 6368  be removed or ch
-00012100: 616e 6765 642e 0a0a 2020 2020 5061 7273  anged...    Pars
-00012110: 6520 6a73 6f6e 2061 6e64 206a 736f 6e53  e json and jsonS
-00012120: 7472 6561 6d20 6173 2072 6574 7572 6e65  tream as returne
-00012130: 6420 6279 206c 6976 6574 696d 696e 672e  d by livetiming.
-00012140: 666f 726d 756c 6131 2e63 6f6d 0a0a 2020  formula1.com..  
-00012150: 2020 5468 6973 2066 756e 6374 696f 6e20    This function 
-00012160: 6361 6e20 6f6e 6c79 2070 6173 7320 6f6e  can only pass on
-00012170: 6520 6461 7461 2065 6e74 7279 2061 7420  e data entry at 
-00012180: 6120 7469 6d65 2c20 6e6f 7420 6120 7768  a time, not a wh
-00012190: 6f6c 6520 7265 7370 6f6e 7365 2e0a 2020  ole response..  
-000121a0: 2020 5469 6d65 7374 616d 7073 2061 6e64    Timestamps and
-000121b0: 2064 6174 6120 6e65 6564 2074 6f20 6265   data need to be
-000121c0: 2073 6570 6172 6174 6564 2062 6566 6f72   separated befor
-000121d0: 6520 616e 6420 6f6e 6c79 2074 6865 2064  e and only the d
-000121e0: 6174 6120 6d75 7374 2062 6520 7061 7373  ata must be pass
-000121f0: 6564 2061 7320 6120 7374 7269 6e67 2074  ed as a string t
-00012200: 6f20 6265 2070 6172 7365 642e 0a0a 2020  o be parsed...  
-00012210: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00012220: 7465 7874 3a20 5468 6520 7374 7269 6e67  text: The string
-00012230: 2077 6869 6368 2073 686f 756c 6420 6265   which should be
-00012240: 2070 6172 7365 640a 2020 2020 2020 2020   parsed.        
-00012250: 7a69 7070 6564 3a20 5768 6574 6865 7220  zipped: Whether 
-00012260: 7468 6520 7465 7874 2069 7320 636f 6d70  the text is comp
-00012270: 7265 7373 6564 2e20 5468 6973 2069 7320  ressed. This is 
-00012280: 7468 6520 6361 7365 2066 6f72 2020 272e  the case for  '.
-00012290: 7a27 0a20 2020 2020 2020 2020 2020 2064  z'.            d
-000122a0: 6174 6120 2865 2e67 2e20 706f 7369 7469  ata (e.g. positi
-000122b0: 6f6e 2064 6174 6129 0a0a 2020 2020 5265  on data)..    Re
-000122c0: 7475 726e 733a 0a20 2020 2020 2020 2044  turns:.        D
-000122d0: 6570 656e 6469 6e67 206f 6e20 6461 7461  epending on data
-000122e0: 206f 6620 7768 6963 6820 7061 6765 2069   of which page i
-000122f0: 7320 7061 7273 6564 0a20 2020 2020 2020  s parsed.       
-00012300: 2020 2020 202d 2061 2064 6963 7469 6f6e       - a diction
-00012310: 6172 7920 6372 6561 7465 6420 6173 2061  ary created as a
-00012320: 2072 6573 756c 7420 6f66 206c 6f61 6469   result of loadi
-00012330: 6e67 206a 736f 6e20 6461 7461 0a20 2020  ng json data.   
-00012340: 2020 2020 2020 2020 202d 2061 2073 7472           - a str
-00012350: 696e 670a 2020 2020 2222 220a 2020 2020  ing.    """.    
-00012360: 6966 2074 6578 745b 305d 203d 3d20 277b  if text[0] == '{
-00012370: 273a 0a20 2020 2020 2020 2072 6574 7572  ':.        retur
-00012380: 6e20 6a73 6f6e 2e6c 6f61 6473 2874 6578  n json.loads(tex
-00012390: 7429 0a20 2020 2069 6620 7465 7874 5b30  t).    if text[0
-000123a0: 5d20 3d3d 2027 2227 3a0a 2020 2020 2020  ] == '"':.      
-000123b0: 2020 7465 7874 203d 2074 6578 742e 7374    text = text.st
-000123c0: 7269 7028 2722 2729 0a20 2020 2069 6620  rip('"').    if 
-000123d0: 7a69 7070 6564 3a0a 2020 2020 2020 2020  zipped:.        
-000123e0: 7465 7874 203d 207a 6c69 622e 6465 636f  text = zlib.deco
-000123f0: 6d70 7265 7373 2862 6173 6536 342e 6236  mpress(base64.b6
-00012400: 3464 6563 6f64 6528 7465 7874 292c 202d  4decode(text), -
-00012410: 7a6c 6962 2e4d 4158 5f57 4249 5453 290a  zlib.MAX_WBITS).
-00012420: 2020 2020 2020 2020 7265 7475 726e 2070          return p
-00012430: 6172 7365 2874 6578 742e 6465 636f 6465  arse(text.decode
-00012440: 2827 7574 662d 382d 7369 6727 2929 0a20  ('utf-8-sig')). 
-00012450: 2020 205f 6c6f 6767 6572 2e77 6172 6e69     _logger.warni
-00012460: 6e67 2822 436f 756c 646e 2774 2070 6172  ng("Couldn't par
-00012470: 7365 2074 6578 7422 290a 2020 2020 7265  se text").    re
-00012480: 7475 726e 2074 6578 740a 0a0a 636c 6173  turn text...clas
-00012490: 7320 5365 7373 696f 6e4e 6f74 4176 6169  s SessionNotAvai
-000124a0: 6c61 626c 6545 7272 6f72 2845 7863 6570  lableError(Excep
-000124b0: 7469 6f6e 293a 0a20 2020 2022 2222 5261  tion):.    """Ra
-000124c0: 6973 6564 2069 6620 616e 2061 7069 2072  ised if an api r
-000124d0: 6571 7565 7374 2072 6574 7572 6e65 6420  equest returned 
-000124e0: 6e6f 2064 6174 6120 666f 7220 7468 6520  no data for the 
-000124f0: 7265 7175 6573 7465 6420 7365 7373 696f  requested sessio
-00012500: 6e2e 0a20 2020 2041 206c 696b 656c 7920  n..    A likely 
-00012510: 6361 7573 6520 6973 2074 6861 7420 7468  cause is that th
-00012520: 6520 7365 7373 696f 6e20 646f 6573 206e  e session does n
-00012530: 6f74 2065 7869 7374 2062 6563 6175 7365  ot exist because
-00012540: 2069 7420 7761 7320 6361 6e63 656c 6c65   it was cancelle
-00012550: 642e 2222 220a 0a20 2020 2064 6566 205f  d."""..    def _
-00012560: 5f69 6e69 745f 5f28 7365 6c66 2c20 2a61  _init__(self, *a
-00012570: 7267 7329 3a0a 2020 2020 2020 2020 7375  rgs):.        su
-00012580: 7065 7228 292e 5f5f 696e 6974 5f5f 282a  per().__init__(*
-00012590: 6172 6773 290a                           args).
+0000ac80: 2063 6f6e 7469 6e75 650a 0a20 2020 2020   continue..     
+0000ac90: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0000aca0: 6174 615b 6472 765d 2e61 7070 656e 6428  ata[drv].append(
+0000acb0: 2874 696d 652c 2064 6174 652c 2072 706d  (time, date, rpm
+0000acc0: 2c20 7370 6565 642c 206e 6765 6172 2c20  , speed, ngear, 
+0000acd0: 7468 726f 7474 6c65 2c0a 2020 2020 2020  throttle,.      
+0000ace0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad00: 6272 616b 652c 2064 7273 2c20 2763 6172  brake, drs, 'car
+0000ad10: 2729 290a 0a20 2020 2020 2020 2065 7863  '))..        exc
+0000ad20: 6570 7420 4578 6365 7074 696f 6e3a 0a20  ept Exception:. 
+0000ad30: 2020 2020 2020 2020 2020 2023 2074 6f6f             # too
+0000ad40: 2072 6973 6b79 2074 6f20 7370 6563 6966   risky to specif
+0000ad50: 7920 616e 2065 7863 6570 7469 6f6e 3a20  y an exception: 
+0000ad60: 756e 6578 7065 6374 6564 2069 6e76 616c  unexpected inval
+0000ad70: 6964 2064 6174 6121 0a20 2020 2020 2020  id data!.       
+0000ad80: 2020 2020 2064 6563 6f64 655f 6572 726f       decode_erro
+0000ad90: 725f 636f 756e 7420 2b3d 2031 0a20 2020  r_count += 1.   
+0000ada0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+0000adb0: 650a 0a20 2020 2069 6620 6465 636f 6465  e..    if decode
+0000adc0: 5f65 7272 6f72 5f63 6f75 6e74 203e 2030  _error_count > 0
+0000add0: 3a0a 2020 2020 2020 2020 5f6c 6f67 6765  :.        _logge
+0000ade0: 722e 7761 726e 696e 6728 6622 4361 7220  r.warning(f"Car 
+0000adf0: 6461 7461 3a20 6661 696c 6564 2074 6f20  data: failed to 
+0000ae00: 6465 636f 6465 207b 6465 636f 6465 5f65  decode {decode_e
+0000ae10: 7272 6f72 5f63 6f75 6e74 7d20 220a 2020  rror_count} ".  
+0000ae20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae30: 2020 2020 2020 6622 6d65 7373 6167 6573        f"messages
+0000ae40: 2028 7b6c 656e 2872 6573 706f 6e73 6529   ({len(response)
+0000ae50: 7d20 6d65 7373 6167 6573 2074 6f74 616c  } messages total
+0000ae60: 2922 290a 0a20 2020 2023 2063 7265 6174  )")..    # creat
+0000ae70: 6520 6f6e 6520 6461 7461 6672 616d 6520  e one dataframe 
+0000ae80: 7065 7220 6472 6976 6572 2061 6e64 2063  per driver and c
+0000ae90: 6865 636b 2066 6f72 2074 6865 206c 6f6e  heck for the lon
+0000aea0: 6765 7374 2064 6174 6166 7261 6d65 0a20  gest dataframe. 
+0000aeb0: 2020 206d 6f73 745f 636f 6d70 6c65 7465     most_complete
+0000aec0: 5f72 6566 203d 204e 6f6e 650a 2020 2020  _ref = None.    
+0000aed0: 666f 7220 6472 7620 696e 2064 6174 613a  for drv in data:
+0000aee0: 0a20 2020 2020 2020 2061 7272 5f61 6c6c  .        arr_all
+0000aef0: 203d 206e 702e 6172 7261 7928 6461 7461   = np.array(data
+0000af00: 5b64 7276 5d29 0a20 2020 2020 2020 2074  [drv]).        t
+0000af10: 696d 6520 3d20 6172 725f 616c 6c5b 3a2c  ime = arr_all[:,
+0000af20: 2030 5d2e 6173 7479 7065 2827 7469 6d65   0].astype('time
+0000af30: 6465 6c74 6136 345b 6e73 5d27 290a 2020  delta64[ns]').  
+0000af40: 2020 2020 2020 6461 7465 203d 2061 7272        date = arr
+0000af50: 5f61 6c6c 5b3a 2c20 315d 2e61 7374 7970  _all[:, 1].astyp
+0000af60: 6528 2764 6174 6574 696d 6536 345b 6e73  e('datetime64[ns
+0000af70: 5d27 290a 2020 2020 2020 2020 7270 6d20  ]').        rpm 
+0000af80: 3d20 6172 725f 616c 6c5b 3a2c 2032 5d2e  = arr_all[:, 2].
+0000af90: 6173 7479 7065 2827 696e 7436 3427 290a  astype('int64').
+0000afa0: 2020 2020 2020 2020 7370 6565 6420 3d20          speed = 
+0000afb0: 6172 725f 616c 6c5b 3a2c 2033 5d2e 6173  arr_all[:, 3].as
+0000afc0: 7479 7065 2827 696e 7436 3427 290a 2020  type('int64').  
+0000afd0: 2020 2020 2020 6e67 6561 7220 3d20 6172        ngear = ar
+0000afe0: 725f 616c 6c5b 3a2c 2034 5d2e 6173 7479  r_all[:, 4].asty
+0000aff0: 7065 2827 696e 7436 3427 290a 2020 2020  pe('int64').    
+0000b000: 2020 2020 7468 726f 7474 6c65 203d 2061      throttle = a
+0000b010: 7272 5f61 6c6c 5b3a 2c20 355d 2e61 7374  rr_all[:, 5].ast
+0000b020: 7970 6528 2769 6e74 3634 2729 0a20 2020  ype('int64').   
+0000b030: 2020 2020 2062 7261 6b65 203d 2061 7272       brake = arr
+0000b040: 5f61 6c6c 5b3a 2c20 365d 2e61 7374 7970  _all[:, 6].astyp
+0000b050: 6528 2769 6e74 3634 2729 2020 2320 636f  e('int64')  # co
+0000b060: 6e76 6572 7465 6420 746f 2062 6f6f 6c20  nverted to bool 
+0000b070: 6c61 7465 720a 2020 2020 2020 2020 6472  later.        dr
+0000b080: 7320 3d20 6172 725f 616c 6c5b 3a2c 2037  s = arr_all[:, 7
+0000b090: 5d2e 6173 7479 7065 2827 696e 7436 3427  ].astype('int64'
+0000b0a0: 290a 2020 2020 2020 2020 736f 7572 6365  ).        source
+0000b0b0: 203d 2061 7272 5f61 6c6c 5b3a 2c20 385d   = arr_all[:, 8]
+0000b0c0: 2e61 7374 7970 6528 276f 626a 6563 7427  .astype('object'
+0000b0d0: 290a 0a20 2020 2020 2020 2064 6174 615b  )..        data[
+0000b0e0: 6472 765d 203d 2063 7265 6174 655f 6466  drv] = create_df
+0000b0f0: 5f66 6173 7428 0a20 2020 2020 2020 2020  _fast(.         
+0000b100: 2020 2061 7272 6179 733d 5b74 696d 652c     arrays=[time,
+0000b110: 2064 6174 652c 0a20 2020 2020 2020 2020   date,.         
+0000b120: 2020 2020 2020 2020 2020 2072 706d 2c20             rpm, 
+0000b130: 7370 6565 642c 206e 6765 6172 2c20 7468  speed, ngear, th
+0000b140: 726f 7474 6c65 2c20 6272 616b 652c 2064  rottle, brake, d
+0000b150: 7273 2c20 736f 7572 6365 5d2c 0a20 2020  rs, source],.   
+0000b160: 2020 2020 2020 2020 2063 6f6c 756d 6e73           columns
+0000b170: 3d63 6f6c 756d 6e73 0a20 2020 2020 2020  =columns.       
+0000b180: 2029 0a0a 2020 2020 2020 2020 6966 2028   )..        if (
+0000b190: 6d6f 7374 5f63 6f6d 706c 6574 655f 7265  most_complete_re
+0000b1a0: 6620 6973 204e 6f6e 6529 205c 0a20 2020  f is None) \.   
+0000b1b0: 2020 2020 2020 2020 2020 2020 206f 7220               or 
+0000b1c0: 286c 656e 2864 6174 615b 6472 765d 5b27  (len(data[drv]['
+0000b1d0: 4461 7465 275d 2920 3e20 6c65 6e28 6d6f  Date']) > len(mo
+0000b1e0: 7374 5f63 6f6d 706c 6574 655f 7265 6629  st_complete_ref)
+0000b1f0: 293a 0a20 2020 2020 2020 2020 2020 206d  ):.            m
+0000b200: 6f73 745f 636f 6d70 6c65 7465 5f72 6566  ost_complete_ref
+0000b210: 203d 2064 6174 615b 6472 765d 5b27 4461   = data[drv]['Da
+0000b220: 7465 275d 0a0a 2020 2020 666f 7220 6472  te']..    for dr
+0000b230: 7620 696e 2064 6174 613a 0a20 2020 2020  v in data:.     
+0000b240: 2020 2023 2069 6620 6576 6572 7974 6869     # if everythi
+0000b250: 6e67 2069 7320 7765 6c6c 2c20 616c 6c20  ng is well, all 
+0000b260: 6461 7461 6672 616d 6573 2073 686f 756c  dataframes shoul
+0000b270: 6420 6861 7665 2074 6865 2073 616d 6520  d have the same 
+0000b280: 6c65 6e67 7468 0a20 2020 2020 2020 2023  length.        #
+0000b290: 2061 6e64 206e 6f20 706f 7374 7072 6f63   and no postproc
+0000b2a0: 6573 7369 6e67 2069 7320 6e65 6365 7373  essing is necess
+0000b2b0: 6172 790a 2020 2020 2020 2020 6966 206c  ary.        if l
+0000b2c0: 656e 2864 6174 615b 6472 765d 5b27 4461  en(data[drv]['Da
+0000b2d0: 7465 275d 2920 3c20 6c65 6e28 6d6f 7374  te']) < len(most
+0000b2e0: 5f63 6f6d 706c 6574 655f 7265 6629 3a0a  _complete_ref):.
+0000b2f0: 2020 2020 2020 2020 2020 2020 2320 7468              # th
+0000b300: 6572 6520 6973 206d 6973 7369 6e67 2064  ere is missing d
+0000b310: 6174 6120 666f 7220 7468 6973 2064 7269  ata for this dri
+0000b320: 7665 720a 2020 2020 2020 2020 2020 2020  ver.            
+0000b330: 2320 6578 7465 6e64 2074 6865 2044 6174  # extend the Dat
+0000b340: 6520 636f 6c75 6d6e 2061 6e64 2066 696c  e column and fil
+0000b350: 6c20 7570 206d 6973 7369 6e67 2074 656c  l up missing tel
+0000b360: 656d 6574 7279 2076 616c 7565 7320 7769  emetry values wi
+0000b370: 7468 0a20 2020 2020 2020 2020 2020 2023  th.            #
+0000b380: 207a 6572 6f2c 2065 7863 6570 7420 5469   zero, except Ti
+0000b390: 6d65 2077 6869 6368 2069 7320 6c65 6674  me which is left
+0000b3a0: 2061 7320 4e61 5420 616e 6420 7769 6c6c   as NaT and will
+0000b3b0: 2062 6520 6361 6c63 756c 6174 6564 0a20   be calculated. 
+0000b3c0: 2020 2020 2020 2020 2020 2023 2063 6f72             # cor
+0000b3d0: 7265 6374 6c79 2062 6173 6564 206f 6e20  rectly based on 
+0000b3e0: 5365 7373 696f 6e2e 7430 5f64 6174 6520  Session.t0_date 
+0000b3f0: 616e 7977 6179 2077 6865 6e20 6372 6561  anyway when crea
+0000b400: 7469 6e67 2054 656c 656d 6574 7279 0a20  ting Telemetry. 
+0000b410: 2020 2020 2020 2020 2020 2023 2069 6e73             # ins
+0000b420: 7461 6e63 6573 2069 6e20 5365 7373 696f  tances in Sessio
+0000b430: 6e2e 6c6f 6164 5f74 656c 656d 6574 7279  n.load_telemetry
+0000b440: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+0000b450: 615b 6472 765d 203d 2064 6174 615b 6472  a[drv] = data[dr
+0000b460: 765d 205c 0a20 2020 2020 2020 2020 2020  v] \.           
+0000b470: 2020 2020 202e 6d65 7267 6528 6d6f 7374       .merge(most
+0000b480: 5f63 6f6d 706c 6574 655f 7265 662c 2068  _complete_ref, h
+0000b490: 6f77 3d27 6f75 7465 7227 2920 5c0a 2020  ow='outer') \.  
+0000b4a0: 2020 2020 2020 2020 2020 2020 2020 2e73                .s
+0000b4b0: 6f72 745f 7661 6c75 6573 2862 793d 2744  ort_values(by='D
+0000b4c0: 6174 6527 2920 5c0a 2020 2020 2020 2020  ate') \.        
+0000b4d0: 2020 2020 2020 2020 2e72 6573 6574 5f69          .reset_i
+0000b4e0: 6e64 6578 2864 726f 703d 5472 7565 290a  ndex(drop=True).
+0000b4f0: 0a20 2020 2020 2020 2020 2020 205f 6c6f  .            _lo
+0000b500: 6767 6572 2e77 6172 6e69 6e67 2866 2244  gger.warning(f"D
+0000b510: 7269 7665 7220 7b64 7276 3a20 3e32 7d3a  river {drv: >2}:
+0000b520: 2043 6172 2064 6174 6120 6973 2069 6e63   Car data is inc
+0000b530: 6f6d 706c 6574 6521 2229 0a0a 2020 2020  omplete!")..    
+0000b540: 2020 2020 2320 656e 7375 7265 2074 6861      # ensure tha
+0000b550: 7420 6272 616b 6520 6461 7461 2069 7320  t brake data is 
+0000b560: 2762 6f6f 6c65 616e 2d63 6f6d 7061 7469  'boolean-compati
+0000b570: 626c 6527 2069 6e20 6361 7365 2074 6861  ble' in case tha
+0000b580: 7420 7468 6973 2069 730a 2020 2020 2020  t this is.      
+0000b590: 2020 2320 6576 6572 2063 6861 6e67 6564    # ever changed
+0000b5a0: 0a20 2020 2020 2020 205f 756e 6971 7565  .        _unique
+0000b5b0: 5f62 7261 6b65 5f76 616c 7565 7320 3d20  _brake_values = 
+0000b5c0: 6461 7461 5b64 7276 5d2e 6c6f 635b 3a2c  data[drv].loc[:,
+0000b5d0: 2027 4272 616b 6527 5d2e 756e 6971 7565   'Brake'].unique
+0000b5e0: 2829 0a20 2020 2020 2020 2069 6620 2828  ().        if ((
+0000b5f0: 5f75 6e69 7175 655f 6272 616b 655f 7661  _unique_brake_va
+0000b600: 6c75 6573 203e 2030 2920 2620 285f 756e  lues > 0) & (_un
+0000b610: 6971 7565 5f62 7261 6b65 5f76 616c 7565  ique_brake_value
+0000b620: 7320 3c20 3130 3029 292e 616e 7928 293a  s < 100)).any():
+0000b630: 0a20 2020 2020 2020 2020 2020 205f 6c6f  .            _lo
+0000b640: 6767 6572 2e77 6172 6e69 6e67 2866 2244  gger.warning(f"D
+0000b650: 7269 7665 7220 7b64 7276 3a20 3e32 7d3a  river {drv: >2}:
+0000b660: 2052 6177 2062 7261 6b65 2064 6174 6120   Raw brake data 
+0000b670: 636f 6e74 6169 6e73 2022 0a20 2020 2020  contains ".     
+0000b680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b690: 2020 2020 2020 2066 226e 6f6e 2d62 6f6f         f"non-boo
+0000b6a0: 6c65 616e 2076 616c 7565 7321 2229 0a0a  lean values!")..
+0000b6b0: 2020 2020 2020 2020 2320 636f 6e76 6572          # conver
+0000b6c0: 7420 746f 2063 6f72 7265 6374 2064 6174  t to correct dat
+0000b6d0: 6174 7970 6573 0a20 2020 2020 2020 2064  atypes.        d
+0000b6e0: 6174 615b 6472 765d 5b6e 756d 6572 6963  ata[drv][numeric
+0000b6f0: 5f63 6861 6e6e 656c 735d 203d 205c 0a20  _channels] = \. 
+0000b700: 2020 2020 2020 2020 2020 2064 6174 615b             data[
+0000b710: 6472 765d 2e6c 6f63 5b3a 2c20 6e75 6d65  drv].loc[:, nume
+0000b720: 7269 635f 6368 616e 6e65 6c73 5d20 5c0a  ric_channels] \.
+0000b730: 2020 2020 2020 2020 2020 2020 2e66 696c              .fil
+0000b740: 6c6e 6128 7661 6c75 653d 302c 2069 6e70  lna(value=0, inp
+0000b750: 6c61 6365 3d46 616c 7365 2920 5c0a 2020  lace=False) \.  
+0000b760: 2020 2020 2020 2020 2020 2e61 7374 7970            .astyp
+0000b770: 6528 2769 6e74 3634 2729 0a0a 2020 2020  e('int64')..    
+0000b780: 2020 2020 6461 7461 5b64 7276 5d5b 626f      data[drv][bo
+0000b790: 6f6c 5f63 6861 6e6e 656c 735d 203d 205c  ol_channels] = \
+0000b7a0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+0000b7b0: 615b 6472 765d 2e6c 6f63 5b3a 2c20 626f  a[drv].loc[:, bo
+0000b7c0: 6f6c 5f63 6861 6e6e 656c 735d 205c 0a20  ol_channels] \. 
+0000b7d0: 2020 2020 2020 2020 2020 202e 6669 6c6c             .fill
+0000b7e0: 6e61 2876 616c 7565 3d46 616c 7365 2c20  na(value=False, 
+0000b7f0: 696e 706c 6163 653d 4661 6c73 6529 205c  inplace=False) \
+0000b800: 0a20 2020 2020 2020 2020 2020 202e 6173  .            .as
+0000b810: 7479 7065 2827 626f 6f6c 2729 0a0a 2020  type('bool')..  
+0000b820: 2020 7265 7475 726e 2064 6174 610a 0a0a    return data...
+0000b830: 4043 6163 6865 2e61 7069 5f72 6571 7565  @Cache.api_reque
+0000b840: 7374 5f77 7261 7070 6572 0a64 6566 2070  st_wrapper.def p
+0000b850: 6f73 6974 696f 6e5f 6461 7461 2870 6174  osition_data(pat
+0000b860: 682c 2072 6573 706f 6e73 653d 4e6f 6e65  h, response=None
+0000b870: 2c20 6c69 7665 6461 7461 3d4e 6f6e 6529  , livedata=None)
+0000b880: 3a0a 2020 2020 2222 220a 2020 2020 2e2e  :.    """.    ..
+0000b890: 2077 6172 6e69 6e67 3a3a 0a20 2020 2020   warning::.     
+0000b8a0: 2020 203a 6d6f 643a 6066 6173 7466 312e     :mod:`fastf1.
+0000b8b0: 6170 6960 2077 696c 6c20 6265 2063 6f6e  api` will be con
+0000b8c0: 7369 6465 7265 6420 7072 6976 6174 6520  sidered private 
+0000b8d0: 696e 2066 7574 7572 6520 7265 6c65 6173  in future releas
+0000b8e0: 6573 2061 6e64 0a20 2020 2020 2020 2070  es and.        p
+0000b8f0: 6f74 656e 7469 616c 6c79 2062 6520 7265  otentially be re
+0000b900: 6d6f 7665 6420 6f72 2063 6861 6e67 6564  moved or changed
+0000b910: 2e0a 0a20 2020 2046 6574 6368 2061 6e64  ...    Fetch and
+0000b920: 2070 6172 7365 2070 6f73 6974 696f 6e20   parse position 
+0000b930: 6461 7461 2e0a 0a20 2020 2050 6f73 6974  data...    Posit
+0000b940: 696f 6e20 6461 7461 2070 726f 7669 6465  ion data provide
+0000b950: 7320 7468 6520 666f 6c6c 6f77 696e 6720  s the following 
+0000b960: 6461 7461 2063 6861 6e6e 656c 7320 7065  data channels pe
+0000b970: 7220 7361 6d70 6c65 3a0a 2020 2020 2020  r sample:.      
+0000b980: 2020 2d20 5469 6d65 2028 7061 6e64 6173    - Time (pandas
+0000b990: 2e54 696d 6564 656c 7461 293a 2073 6573  .Timedelta): ses
+0000b9a0: 7369 6f6e 2074 696d 6573 7461 6d70 2028  sion timestamp (
+0000b9b0: 7469 6d65 206f 6e6c 7929 3b20 696e 6163  time only); inac
+0000b9c0: 6375 7261 7465 2c20 6861 7320 6475 706c  curate, has dupl
+0000b9d0: 6963 6174 6520 7661 6c75 6573 3b20 7573  icate values; us
+0000b9e0: 6520 4461 7465 2069 6e73 7465 6164 0a20  e Date instead. 
+0000b9f0: 2020 2020 2020 202d 2044 6174 6520 2870         - Date (p
+0000ba00: 616e 6461 732e 5469 6d65 7374 616d 7029  andas.Timestamp)
+0000ba10: 3a20 7469 6d65 7374 616d 7020 666f 7220  : timestamp for 
+0000ba20: 7468 6973 2073 616d 706c 6520 6173 2044  this sample as D
+0000ba30: 6174 6520 2b20 5469 6d65 3b20 6d6f 7265  ate + Time; more
+0000ba40: 206f 7220 6c65 7373 2065 7861 6374 0a20   or less exact. 
+0000ba50: 2020 2020 2020 202d 2053 7461 7475 7320         - Status 
+0000ba60: 2873 7472 293a 2027 4f6e 5472 6163 6b27  (str): 'OnTrack'
+0000ba70: 206f 7220 274f 6666 5472 6163 6b27 0a20   or 'OffTrack'. 
+0000ba80: 2020 2020 2020 202d 2058 2c20 592c 205a         - X, Y, Z
+0000ba90: 2028 696e 7429 3a20 506f 7369 7469 6f6e   (int): Position
+0000baa0: 2063 6f6f 7264 696e 6174 6573 3b20 7374   coordinates; st
+0000bab0: 6172 7469 6e67 2066 726f 6d20 3230 3230  arting from 2020
+0000bac0: 2074 6865 2063 6f6f 7264 696e 6174 6573   the coordinates
+0000bad0: 2061 7265 2067 6976 656e 2069 6e20 312f   are given in 1/
+0000bae0: 3130 206d 6574 6572 0a20 2020 2020 2020  10 meter.       
+0000baf0: 202d 2053 6f75 7263 6520 2873 7472 293a   - Source (str):
+0000bb00: 2049 6e64 6963 6174 6573 2074 6865 2073   Indicates the s
+0000bb10: 6f75 7263 6520 6f66 2061 2073 616d 706c  ource of a sampl
+0000bb20: 653b 2027 706f 7327 2066 6f72 2061 6c6c  e; 'pos' for all
+0000bb30: 2076 616c 7565 7320 6865 7265 0a0a 2020   values here..  
+0000bb40: 2020 5468 6520 6461 7461 2073 7472 6561    The data strea
+0000bb50: 6d20 6861 7320 6120 7361 6d70 6c65 2072  m has a sample r
+0000bb60: 6174 6520 6f66 2028 7573 7561 6c6c 7929  ate of (usually)
+0000bb70: 2032 3230 6d73 2e20 5468 6520 7361 6d70   220ms. The samp
+0000bb80: 6c65 7320 6672 6f6d 2074 6865 2064 6174  les from the dat
+0000bb90: 6120 7374 7265 616d 7320 666f 7220 706f  a streams for po
+0000bba0: 7369 7469 6f6e 2064 6174 6120 616e 640a  sition data and.
+0000bbb0: 2020 2020 6361 7220 6461 7461 2064 6f20      car data do 
+0000bbc0: 6e6f 7420 6c69 6e65 2075 702e 2052 6573  not line up. Res
+0000bbd0: 616d 706c 696e 672f 696e 7465 7270 6f6c  ampling/interpol
+0000bbe0: 6174 696f 6e20 6973 2072 6571 7569 7265  ation is require
+0000bbf0: 6420 746f 206d 6572 6765 2074 6865 6d2e  d to merge them.
+0000bc00: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+0000bc10: 2020 2020 7061 7468 2028 7374 7229 3a20      path (str): 
+0000bc20: 6170 6920 7061 7468 2062 6173 6520 7374  api path base st
+0000bc30: 7269 6e67 2028 7573 7561 6c6c 7920 6060  ring (usually ``
+0000bc40: 5365 7373 696f 6e2e 6170 695f 7061 7468  Session.api_path
+0000bc50: 6060 290a 2020 2020 2020 2020 7265 7370  ``).        resp
+0000bc60: 6f6e 7365 3a20 5265 7370 6f6e 7365 2061  onse: Response a
+0000bc70: 7320 7265 7475 726e 6564 2062 7920 3a66  s returned by :f
+0000bc80: 756e 633a 6066 6574 6368 5f70 6167 6560  unc:`fetch_page`
+0000bc90: 2063 616e 2062 6520 7061 7373 6564 2069   can be passed i
+0000bca0: 6620 6974 2077 6173 2064 6f77 6e6c 6f61  f it was downloa
+0000bcb0: 6465 6420 616c 7265 6164 792e 0a20 2020  ded already..   
+0000bcc0: 2020 2020 206c 6976 6564 6174 613a 2041       livedata: A
+0000bcd0: 6e20 696e 7374 616e 6365 206f 6620 3a63  n instance of :c
+0000bce0: 6c61 7373 3a60 6661 7374 6631 2e6c 6976  lass:`fastf1.liv
+0000bcf0: 6574 696d 696e 672e 6461 7461 2e4c 6976  etiming.data.Liv
+0000bd00: 6554 696d 696e 6744 6174 6160 2074 6f20  eTimingData` to 
+0000bd10: 7573 6520 6173 2061 2073 6f75 7263 6520  use as a source 
+0000bd20: 696e 7374 6561 6420 6f66 2074 6865 2061  instead of the a
+0000bd30: 7069 0a0a 2020 2020 5265 7475 726e 733a  pi..    Returns:
+0000bd40: 0a20 2020 2020 2020 207c 2041 2064 6963  .        | A dic
+0000bd50: 7469 6f6e 6172 7920 636f 6e74 6169 6e69  tionary containi
+0000bd60: 6e67 206f 6e65 2070 616e 6461 7320 4461  ng one pandas Da
+0000bd70: 7461 4672 616d 6520 7065 7220 6472 6976  taFrame per driv
+0000bd80: 6572 2e20 4469 6374 696f 6e61 7279 206b  er. Dictionary k
+0000bd90: 6579 7320 6172 6520 7468 6520 6472 6976  eys are the driv
+0000bda0: 6572 2773 206e 756d 6265 7273 2061 730a  er's numbers as.
+0000bdb0: 2020 2020 2020 2020 2020 7374 7269 6e67            string
+0000bdc0: 2028 652e 672e 2027 3136 2729 2e20 596f   (e.g. '16'). Yo
+0000bdd0: 7520 7368 6f75 6c64 206e 6576 6572 2061  u should never a
+0000bde0: 7373 756d 6520 7468 6174 2061 206e 756d  ssume that a num
+0000bdf0: 6265 7220 6578 6973 7473 210a 2020 2020  ber exists!.    
+0000be00: 2020 2020 7c20 4561 6368 2064 6174 6166      | Each dataf
+0000be10: 7261 6d65 2063 6f6e 7461 696e 7320 6f6e  rame contains on
+0000be20: 6520 636f 6c75 6d6e 2066 6f72 2065 6163  e column for eac
+0000be30: 6820 6461 7461 2063 6861 6e6e 656c 2061  h data channel a
+0000be40: 7320 6c69 7374 6564 2061 626f 7665 0a0a  s listed above..
+0000be50: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
+0000be60: 2020 2020 5365 7373 696f 6e4e 6f74 4176      SessionNotAv
+0000be70: 6169 6c61 626c 6545 7272 6f72 3a20 696e  ailableError: in
+0000be80: 2063 6173 6520 7468 6520 4631 206c 6976   case the F1 liv
+0000be90: 6574 696d 696e 6720 6170 6920 7265 7475  etiming api retu
+0000bea0: 726e 7320 6e6f 2064 6174 610a 2020 2020  rns no data.    
+0000beb0: 2222 220a 2020 2020 2320 6461 7461 2072  """.    # data r
+0000bec0: 6563 6f72 6465 6420 6672 6f6d 206c 6976  ecorded from liv
+0000bed0: 6520 7469 6d69 6e67 2068 6173 2061 2073  e timing has a s
+0000bee0: 6c69 6768 746c 7920 6469 6666 6572 656e  lightly differen
+0000bef0: 7420 7374 7275 6374 7572 650a 2020 2020  t structure.    
+0000bf00: 6973 5f6c 6976 6564 6174 6120 3d20 4661  is_livedata = Fa
+0000bf10: 6c73 6520 2023 2066 6c61 6720 746f 2069  lse  # flag to i
+0000bf20: 6e64 6963 6174 6520 6c69 7665 2074 696d  ndicate live tim
+0000bf30: 696e 6720 6461 7461 0a0a 2020 2020 6966  ing data..    if
+0000bf40: 206c 6976 6564 6174 6120 6973 206e 6f74   livedata is not
+0000bf50: 204e 6f6e 6520 616e 6420 6c69 7665 6461   None and liveda
+0000bf60: 7461 2e68 6173 2827 506f 7369 7469 6f6e  ta.has('Position
+0000bf70: 2e7a 2729 3a0a 2020 2020 2020 2020 7265  .z'):.        re
+0000bf80: 7370 6f6e 7365 203d 206c 6976 6564 6174  sponse = livedat
+0000bf90: 612e 6765 7428 2750 6f73 6974 696f 6e2e  a.get('Position.
+0000bfa0: 7a27 290a 2020 2020 2020 2020 6973 5f6c  z').        is_l
+0000bfb0: 6976 6564 6174 6120 3d20 5472 7565 0a20  ivedata = True. 
+0000bfc0: 2020 2065 6c69 6620 7265 7370 6f6e 7365     elif response
+0000bfd0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0000bfe0: 2020 5f6c 6f67 6765 722e 696e 666f 2822    _logger.info("
+0000bff0: 4665 7463 6869 6e67 2070 6f73 6974 696f  Fetching positio
+0000c000: 6e20 6461 7461 2e2e 2e22 290a 2020 2020  n data...").    
+0000c010: 2020 2020 7265 7370 6f6e 7365 203d 2066      response = f
+0000c020: 6574 6368 5f70 6167 6528 7061 7468 2c20  etch_page(path, 
+0000c030: 2770 6f73 6974 696f 6e27 290a 2020 2020  'position').    
+0000c040: 2020 2020 6966 2072 6573 706f 6e73 6520      if response 
+0000c050: 6973 204e 6f6e 653a 2020 2320 6e6f 2072  is None:  # no r
+0000c060: 6573 706f 6e73 6520 7265 6365 6976 6564  esponse received
+0000c070: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+0000c080: 7365 2053 6573 7369 6f6e 4e6f 7441 7661  se SessionNotAva
+0000c090: 696c 6162 6c65 4572 726f 7228 0a20 2020  ilableError(.   
+0000c0a0: 2020 2020 2020 2020 2020 2020 2022 4e6f               "No
+0000c0b0: 2064 6174 6120 666f 7220 7468 6973 2073   data for this s
+0000c0c0: 6573 7369 6f6e 2120 4966 2074 6869 7320  ession! If this 
+0000c0d0: 7365 7373 696f 6e20 6f6e 6c79 2066 696e  session only fin
+0000c0e0: 6973 6865 6420 220a 2020 2020 2020 2020  ished ".        
+0000c0f0: 2020 2020 2020 2020 2272 6563 656e 746c          "recentl
+0000c100: 792c 2070 6c65 6173 6520 7472 7920 6167  y, please try ag
+0000c110: 6169 6e20 696e 2061 2066 6577 206d 696e  ain in a few min
+0000c120: 7574 6573 2e22 0a20 2020 2020 2020 2020  utes.".         
+0000c130: 2020 2029 0a0a 2020 2020 5f6c 6f67 6765     )..    _logge
+0000c140: 722e 696e 666f 2822 5061 7273 696e 6720  r.info("Parsing 
+0000c150: 706f 7369 7469 6f6e 2064 6174 612e 2e2e  position data...
+0000c160: 2229 0a0a 2020 2020 6966 206e 6f74 2072  ")..    if not r
+0000c170: 6573 706f 6e73 653a 0a20 2020 2020 2020  esponse:.       
+0000c180: 2072 6574 7572 6e20 7b7d 0a0a 2020 2020   return {}..    
+0000c190: 7473 5f6c 656e 6774 6820 3d20 3132 2020  ts_length = 12  
+0000c1a0: 2320 6c65 6e67 7468 206f 6620 7469 6d65  # length of time
+0000c1b0: 7374 616d 703a 206c 656e 2827 3030 3a30  stamp: len('00:0
+0000c1c0: 303a 3030 3a30 3030 2729 0a20 2020 2063  0:00:000').    c
+0000c1d0: 6f6c 756d 6e73 203d 205b 2754 696d 6527  olumns = ['Time'
+0000c1e0: 2c20 2744 6174 6527 2c20 2753 7461 7475  , 'Date', 'Statu
+0000c1f0: 7327 2c20 2758 272c 2027 5927 2c20 275a  s', 'X', 'Y', 'Z
+0000c200: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+0000c210: 2020 2753 6f75 7263 6527 5d20 2023 2063    'Source']  # c
+0000c220: 6f72 7265 6374 206f 7264 6572 2072 6571  orrect order req
+0000c230: 7569 7265 6421 0a0a 2020 2020 6461 7461  uired!..    data
+0000c240: 203d 2064 6963 7428 290a 2020 2020 6465   = dict().    de
+0000c250: 636f 6465 5f65 7272 6f72 5f63 6f75 6e74  code_error_count
+0000c260: 203d 2030 0a0a 2020 2020 666f 7220 7265   = 0..    for re
+0000c270: 636f 7264 2069 6e20 7265 7370 6f6e 7365  cord in response
+0000c280: 3a0a 2020 2020 2020 2020 7472 793a 0a20  :.        try:. 
+0000c290: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+0000c2a0: 5f6c 6976 6564 6174 613a 0a20 2020 2020  _livedata:.     
+0000c2b0: 2020 2020 2020 2020 2020 2074 696d 6520             time 
+0000c2c0: 3d20 7265 636f 7264 5b30 5d0a 2020 2020  = record[0].    
+0000c2d0: 2020 2020 2020 2020 2020 2020 6a72 6563              jrec
+0000c2e0: 6f72 643a 2064 6963 7420 3d20 7061 7273  ord: dict = pars
+0000c2f0: 6528 7265 636f 7264 5b31 5d2c 207a 6970  e(record[1], zip
+0000c300: 7065 643d 5472 7565 290a 2020 2020 2020  ped=True).      
+0000c310: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000c320: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+0000c330: 203d 2074 6f5f 7469 6d65 6465 6c74 6128   = to_timedelta(
+0000c340: 7265 636f 7264 5b3a 7473 5f6c 656e 6774  record[:ts_lengt
+0000c350: 685d 290a 2020 2020 2020 2020 2020 2020  h]).            
+0000c360: 2020 2020 6a72 6563 6f72 643a 2064 6963      jrecord: dic
+0000c370: 7420 3d20 7061 7273 6528 7265 636f 7264  t = parse(record
+0000c380: 5b74 735f 6c65 6e67 7468 3a5d 2c20 7a69  [ts_length:], zi
+0000c390: 7070 6564 3d54 7275 6529 0a0a 2020 2020  pped=True)..    
+0000c3a0: 2020 2020 2020 2020 666f 7220 7361 6d70          for samp
+0000c3b0: 6c65 2069 6e20 6a72 6563 6f72 645b 2750  le in jrecord['P
+0000c3c0: 6f73 6974 696f 6e27 5d3a 0a20 2020 2020  osition']:.     
+0000c3d0: 2020 2020 2020 2020 2020 2023 2064 6174             # dat
+0000c3e0: 6520 666f 726d 6174 2069 7320 2732 3032  e format is '202
+0000c3f0: 302d 3038 2d30 3854 3039 3a34 353a 3033  0-08-08T09:45:03
+0000c400: 2e30 3631 3937 3937 5a27 2077 6974 6820  .0619797Z' with 
+0000c410: 6120 7661 7279 696e 670a 2020 2020 2020  a varying.      
+0000c420: 2020 2020 2020 2020 2020 2320 6e75 6d62            # numb
+0000c430: 6572 206f 6620 6d69 6c6c 6973 6563 6f6e  er of millisecon
+0000c440: 6420 6465 6369 6d61 6c20 706f 696e 7473  d decimal points
+0000c450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c460: 2023 2061 6c77 6179 7320 7265 6d6f 7665   # always remove
+0000c470: 206c 6173 7420 6368 6172 2028 277a 2729   last char ('z')
+0000c480: 2c20 6d61 7820 6c65 6e20 3236 2c20 7269  , max len 26, ri
+0000c490: 6768 7420 7061 6420 746f 206c 656e 0a20  ght pad to len. 
+0000c4a0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000c4b0: 2032 3620 7769 7468 207a 6572 6f65 7320   26 with zeroes 
+0000c4c0: 6966 2073 686f 7274 6572 0a20 2020 2020  if shorter.     
+0000c4d0: 2020 2020 2020 2020 2020 2064 6174 6520             date 
+0000c4e0: 3d20 746f 5f64 6174 6574 696d 6528 7361  = to_datetime(sa
+0000c4f0: 6d70 6c65 5b27 5469 6d65 7374 616d 7027  mple['Timestamp'
+0000c500: 5d29 0a0a 2020 2020 2020 2020 2020 2020  ])..            
+0000c510: 2020 2020 666f 7220 6472 7620 696e 2073      for drv in s
+0000c520: 616d 706c 655b 2745 6e74 7269 6573 275d  ample['Entries']
+0000c530: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000c540: 2020 2020 2020 6966 2064 7276 206e 6f74        if drv not
+0000c550: 2069 6e20 6461 7461 3a0a 2020 2020 2020   in data:.      
+0000c560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c570: 2020 2320 696e 6974 6961 6c69 7a65 2064    # initialize d
+0000c580: 6963 7420 656e 7472 7920 666f 7220 7468  ict entry for th
+0000c590: 6973 2064 7269 7665 720a 2020 2020 2020  is driver.      
+0000c5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5b0: 2020 6461 7461 5b64 7276 5d20 3d20 6c69    data[drv] = li
+0000c5c0: 7374 2829 0a0a 2020 2020 2020 2020 2020  st()..          
+0000c5d0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+0000c5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5f0: 2020 2020 2020 2078 203d 2073 616d 706c         x = sampl
+0000c600: 655b 2745 6e74 7269 6573 275d 5b64 7276  e['Entries'][drv
+0000c610: 5d5b 2758 275d 0a20 2020 2020 2020 2020  ]['X'].         
+0000c620: 2020 2020 2020 2020 2020 2020 2020 2079                 y
+0000c630: 203d 2073 616d 706c 655b 2745 6e74 7269   = sample['Entri
+0000c640: 6573 275d 5b64 7276 5d5b 2759 275d 0a20  es'][drv]['Y']. 
+0000c650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c660: 2020 2020 2020 207a 203d 2073 616d 706c         z = sampl
+0000c670: 655b 2745 6e74 7269 6573 275d 5b64 7276  e['Entries'][drv
+0000c680: 5d5b 275a 275d 0a20 2020 2020 2020 2020  ]['Z'].         
+0000c690: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+0000c6a0: 7420 4b65 7945 7272 6f72 3a0a 2020 2020  t KeyError:.    
+0000c6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6c0: 2020 2020 636f 6e74 696e 7565 0a0a 2020      continue..  
+0000c6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6e0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+0000c6f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000c700: 7461 7475 7320 3d20 7361 6d70 6c65 5b27  tatus = sample['
+0000c710: 456e 7472 6965 7327 5d5b 6472 765d 5b27  Entries'][drv]['
+0000c720: 5374 6174 7573 275d 0a20 2020 2020 2020  Status'].       
+0000c730: 2020 2020 2020 2020 2020 2020 2065 7863               exc
+0000c740: 6570 7420 4b65 7945 7272 6f72 3a0a 2020  ept KeyError:.  
+0000c750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c760: 2020 2020 2020 7374 6174 7573 203d 204e        status = N
+0000c770: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+0000c780: 2020 2020 2020 2020 6966 2073 7472 2873          if str(s
+0000c790: 7461 7475 7329 2e69 7364 6967 6974 2829  tatus).isdigit()
+0000c7a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000c7b0: 2020 2020 2020 2020 2020 2320 4661 6c6c            # Fall
+0000c7c0: 6261 636b 206f 6e20 6f6c 6465 7220 6170  back on older ap
+0000c7d0: 6920 7374 6174 7573 206d 6170 7069 6e67  i status mapping
+0000c7e0: 2061 6e64 2063 6f6e 7665 7274 0a20 2020   and convert.   
+0000c7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c800: 2020 2020 2073 7461 7475 7320 3d20 274f       status = 'O
+0000c810: 6666 5472 6163 6b27 2069 6620 696e 7428  ffTrack' if int(
+0000c820: 7374 6174 7573 2920 656c 7365 2027 4f6e  status) else 'On
+0000c830: 5472 6163 6b27 0a0a 2020 2020 2020 2020  Track'..        
+0000c840: 2020 2020 2020 2020 2020 2020 6461 7461              data
+0000c850: 5b64 7276 5d2e 6170 7065 6e64 2828 7469  [drv].append((ti
+0000c860: 6d65 2c20 6461 7465 2c20 7374 6174 7573  me, date, status
+0000c870: 2c20 782c 2079 2c20 7a2c 2027 706f 7327  , x, y, z, 'pos'
+0000c880: 2929 0a0a 2020 2020 2020 2020 6578 6365  ))..        exce
+0000c890: 7074 2045 7863 6570 7469 6f6e 3a0a 2020  pt Exception:.  
+0000c8a0: 2020 2020 2020 2020 2020 2320 746f 6f20            # too 
+0000c8b0: 7269 736b 7920 746f 2073 7065 6369 6679  risky to specify
+0000c8c0: 2061 6e20 6578 6365 7074 696f 6e3a 2075   an exception: u
+0000c8d0: 6e65 7870 6563 7465 6420 696e 7661 6c69  nexpected invali
+0000c8e0: 6420 6461 7461 210a 2020 2020 2020 2020  d data!.        
+0000c8f0: 2020 2020 6465 636f 6465 5f65 7272 6f72      decode_error
+0000c900: 5f63 6f75 6e74 202b 3d20 310a 2020 2020  _count += 1.    
+0000c910: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+0000c920: 0a0a 2020 2020 6966 2064 6563 6f64 655f  ..    if decode_
+0000c930: 6572 726f 725f 636f 756e 7420 3e20 303a  error_count > 0:
+0000c940: 0a20 2020 2020 2020 205f 6c6f 6767 6572  .        _logger
+0000c950: 2e77 6172 6e69 6e67 280a 2020 2020 2020  .warning(.      
+0000c960: 2020 2020 2020 6622 506f 7369 7469 6f6e        f"Position
+0000c970: 2064 6174 613a 2066 6169 6c65 6420 746f   data: failed to
+0000c980: 2064 6563 6f64 6520 7b64 6563 6f64 655f   decode {decode_
+0000c990: 6572 726f 725f 636f 756e 747d 2022 0a20  error_count} ". 
+0000c9a0: 2020 2020 2020 2020 2020 2066 226d 6573             f"mes
+0000c9b0: 7361 6765 7320 287b 6c65 6e28 7265 7370  sages ({len(resp
+0000c9c0: 6f6e 7365 297d 206d 6573 7361 6765 7320  onse)} messages 
+0000c9d0: 746f 7461 6c29 2229 0a0a 2020 2020 2320  total)")..    # 
+0000c9e0: 6372 6561 7465 206f 6e65 2064 6174 6166  create one dataf
+0000c9f0: 7261 6d65 2070 6572 2064 7269 7665 7220  rame per driver 
+0000ca00: 616e 6420 6368 6563 6b20 666f 7220 7468  and check for th
+0000ca10: 6520 6c6f 6e67 6573 7420 6461 7461 6672  e longest datafr
+0000ca20: 616d 650a 2020 2020 6d6f 7374 5f63 6f6d  ame.    most_com
+0000ca30: 706c 6574 655f 7265 6620 3d20 4e6f 6e65  plete_ref = None
+0000ca40: 0a20 2020 2066 6f72 2064 7276 2069 6e20  .    for drv in 
+0000ca50: 6461 7461 3a0a 2020 2020 2020 2020 6172  data:.        ar
+0000ca60: 725f 616c 6c20 3d20 6e70 2e61 7272 6179  r_all = np.array
+0000ca70: 2864 6174 615b 6472 765d 290a 2020 2020  (data[drv]).    
+0000ca80: 2020 2020 7469 6d65 203d 2061 7272 5f61      time = arr_a
+0000ca90: 6c6c 5b3a 2c20 305d 2e61 7374 7970 6528  ll[:, 0].astype(
+0000caa0: 2774 696d 6564 656c 7461 3634 5b6e 735d  'timedelta64[ns]
+0000cab0: 2729 0a20 2020 2020 2020 2064 6174 6520  ').        date 
+0000cac0: 3d20 6172 725f 616c 6c5b 3a2c 2031 5d2e  = arr_all[:, 1].
+0000cad0: 6173 7479 7065 2827 6461 7465 7469 6d65  astype('datetime
+0000cae0: 3634 5b6e 735d 2729 0a20 2020 2020 2020  64[ns]').       
+0000caf0: 2073 7461 7475 7320 3d20 6172 725f 616c   status = arr_al
+0000cb00: 6c5b 3a2c 2032 5d2e 6173 7479 7065 2827  l[:, 2].astype('
+0000cb10: 6f62 6a65 6374 2729 0a20 2020 2020 2020  object').       
+0000cb20: 2078 203d 2061 7272 5f61 6c6c 5b3a 2c20   x = arr_all[:, 
+0000cb30: 335d 2e61 7374 7970 6528 2769 6e74 3634  3].astype('int64
+0000cb40: 2729 0a20 2020 2020 2020 2079 203d 2061  ').        y = a
+0000cb50: 7272 5f61 6c6c 5b3a 2c20 345d 2e61 7374  rr_all[:, 4].ast
+0000cb60: 7970 6528 2769 6e74 3634 2729 0a20 2020  ype('int64').   
+0000cb70: 2020 2020 207a 203d 2061 7272 5f61 6c6c       z = arr_all
+0000cb80: 5b3a 2c20 355d 2e61 7374 7970 6528 2769  [:, 5].astype('i
+0000cb90: 6e74 3634 2729 0a20 2020 2020 2020 2073  nt64').        s
+0000cba0: 6f75 7263 6520 3d20 6172 725f 616c 6c5b  ource = arr_all[
+0000cbb0: 3a2c 2036 5d2e 6173 7479 7065 2827 6f62  :, 6].astype('ob
+0000cbc0: 6a65 6374 2729 0a0a 2020 2020 2020 2020  ject')..        
+0000cbd0: 6461 7461 5b64 7276 5d20 3d20 6372 6561  data[drv] = crea
+0000cbe0: 7465 5f64 665f 6661 7374 280a 2020 2020  te_df_fast(.    
+0000cbf0: 2020 2020 2020 2020 6172 7261 7973 3d5b          arrays=[
+0000cc00: 7469 6d65 2c20 6461 7465 2c20 7374 6174  time, date, stat
+0000cc10: 7573 2c20 782c 2079 2c20 7a2c 2073 6f75  us, x, y, z, sou
+0000cc20: 7263 655d 2c0a 2020 2020 2020 2020 2020  rce],.          
+0000cc30: 2020 636f 6c75 6d6e 733d 636f 6c75 6d6e    columns=column
+0000cc40: 730a 2020 2020 2020 2020 290a 0a20 2020  s.        )..   
+0000cc50: 2020 2020 2023 2063 6865 636b 206c 656e       # check len
+0000cc60: 6774 6820 6f66 2064 6174 6166 7261 6d65  gth of dataframe
+0000cc70: 3b20 736f 6d65 7469 6d65 7320 7468 6572  ; sometimes ther
+0000cc80: 6520 6361 6e20 6265 206d 6973 7369 6e67  e can be missing
+0000cc90: 2064 6174 610a 2020 2020 2020 2020 6966   data.        if
+0000cca0: 2028 6d6f 7374 5f63 6f6d 706c 6574 655f   (most_complete_
+0000ccb0: 7265 6620 6973 204e 6f6e 6529 205c 0a20  ref is None) \. 
+0000ccc0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0000ccd0: 7220 286c 656e 2864 6174 615b 6472 765d  r (len(data[drv]
+0000cce0: 5b27 4461 7465 275d 2920 3e20 6c65 6e28  ['Date']) > len(
+0000ccf0: 6d6f 7374 5f63 6f6d 706c 6574 655f 7265  most_complete_re
+0000cd00: 6629 293a 0a20 2020 2020 2020 2020 2020  f)):.           
+0000cd10: 206d 6f73 745f 636f 6d70 6c65 7465 5f72   most_complete_r
+0000cd20: 6566 203d 2064 6174 615b 6472 765d 5b27  ef = data[drv]['
+0000cd30: 4461 7465 275d 0a0a 2020 2020 2320 6966  Date']..    # if
+0000cd40: 2065 7665 7279 7468 696e 6720 6973 2077   everything is w
+0000cd50: 656c 6c2c 2061 6c6c 2064 6174 6166 7261  ell, all datafra
+0000cd60: 6d65 7320 7368 6f75 6c64 2068 6176 6520  mes should have 
+0000cd70: 7468 6520 7361 6d65 206c 656e 6774 6820  the same length 
+0000cd80: 616e 6420 6e6f 0a20 2020 2023 2070 6f73  and no.    # pos
+0000cd90: 7470 726f 6365 7373 696e 6720 6973 206e  tprocessing is n
+0000cda0: 6563 6573 7361 7279 0a20 2020 2066 6f72  ecessary.    for
+0000cdb0: 2064 7276 2069 6e20 6461 7461 3a0a 2020   drv in data:.  
+0000cdc0: 2020 2020 2020 6966 206c 656e 2864 6174        if len(dat
+0000cdd0: 615b 6472 765d 5b27 4461 7465 275d 2920  a[drv]['Date']) 
+0000cde0: 3c20 6c65 6e28 6d6f 7374 5f63 6f6d 706c  < len(most_compl
+0000cdf0: 6574 655f 7265 6629 3a0a 2020 2020 2020  ete_ref):.      
+0000ce00: 2020 2020 2020 2320 7468 6572 6520 6973        # there is
+0000ce10: 206d 6973 7369 6e67 2064 6174 6120 666f   missing data fo
+0000ce20: 7220 7468 6973 2064 7269 7665 720a 2020  r this driver.  
+0000ce30: 2020 2020 2020 2020 2020 2320 6578 7465            # exte
+0000ce40: 6e64 2074 6865 2044 6174 6520 636f 6c75  nd the Date colu
+0000ce50: 6d6e 2061 6e64 2066 696c 6c20 7570 206d  mn and fill up m
+0000ce60: 6973 7369 6e67 2074 656c 656d 6574 7279  issing telemetry
+0000ce70: 2076 616c 7565 7320 7769 7468 0a20 2020   values with.   
+0000ce80: 2020 2020 2020 2020 2023 207a 6572 6f2c           # zero,
+0000ce90: 2065 7863 6570 7420 5469 6d65 2077 6869   except Time whi
+0000cea0: 6368 2069 7320 6c65 6674 2061 7320 4e61  ch is left as Na
+0000ceb0: 5420 616e 6420 7769 6c6c 2062 6520 6361  T and will be ca
+0000cec0: 6c63 756c 6174 6564 0a20 2020 2020 2020  lculated.       
+0000ced0: 2020 2020 2023 2063 6f72 7265 6374 6c79       # correctly
+0000cee0: 2062 6173 6564 206f 6e20 5365 7373 696f   based on Sessio
+0000cef0: 6e2e 7430 5f64 6174 6520 616e 7977 6179  n.t0_date anyway
+0000cf00: 2077 6865 6e20 6372 6561 7469 6e67 2054   when creating T
+0000cf10: 656c 656d 6574 7279 0a20 2020 2020 2020  elemetry.       
+0000cf20: 2020 2020 2023 2069 6e73 7461 6e63 6573       # instances
+0000cf30: 2069 6e20 5365 7373 696f 6e2e 6c6f 6164   in Session.load
+0000cf40: 5f74 656c 656d 6574 7279 0a20 2020 2020  _telemetry.     
+0000cf50: 2020 2020 2020 2023 2061 6e64 2065 7863         # and exc
+0000cf60: 6570 7420 5374 6174 7573 2077 6869 6368  ept Status which
+0000cf70: 2073 686f 756c 6420 6265 2027 4f66 6654   should be 'OffT
+0000cf80: 7261 636b 2720 666f 7220 6d69 7373 696e  rack' for missin
+0000cf90: 6720 6461 7461 0a20 2020 2020 2020 2020  g data.         
+0000cfa0: 2020 2064 6174 615b 6472 765d 203d 2064     data[drv] = d
+0000cfb0: 6174 615b 6472 765d 205c 0a20 2020 2020  ata[drv] \.     
+0000cfc0: 2020 2020 2020 2020 2020 202e 6d65 7267             .merg
+0000cfd0: 6528 6d6f 7374 5f63 6f6d 706c 6574 655f  e(most_complete_
+0000cfe0: 7265 662c 2068 6f77 3d27 6f75 7465 7227  ref, how='outer'
+0000cff0: 2920 5c0a 2020 2020 2020 2020 2020 2020  ) \.            
+0000d000: 2020 2020 2e73 6f72 745f 7661 6c75 6573      .sort_values
+0000d010: 2862 793d 2744 6174 6527 2920 5c0a 2020  (by='Date') \.  
+0000d020: 2020 2020 2020 2020 2020 2020 2020 2e72                .r
+0000d030: 6573 6574 5f69 6e64 6578 2864 726f 703d  eset_index(drop=
+0000d040: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
+0000d050: 2020 6461 7461 5b64 7276 5d5b 2753 7461    data[drv]['Sta
+0000d060: 7475 7327 5d20 3d20 6461 7461 5b64 7276  tus'] = data[drv
+0000d070: 5d5b 2753 7461 7475 7327 5d20 5c0a 2020  ]['Status'] \.  
+0000d080: 2020 2020 2020 2020 2020 2020 2020 2e66                .f
+0000d090: 696c 6c6e 6128 7661 6c75 653d 274f 6666  illna(value='Off
+0000d0a0: 5472 6163 6b27 2c20 696e 706c 6163 653d  Track', inplace=
+0000d0b0: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
+0000d0c0: 2020 2064 6174 615b 6472 765d 2e6c 6f63     data[drv].loc
+0000d0d0: 5b3a 2c20 5b27 5827 2c20 2759 272c 2027  [:, ['X', 'Y', '
+0000d0e0: 5a27 5d5d 203d 205c 0a20 2020 2020 2020  Z']] = \.       
+0000d0f0: 2020 2020 2020 2020 2064 6174 615b 6472           data[dr
+0000d100: 765d 2e6c 6f63 5b3a 2c20 5b27 5827 2c20  v].loc[:, ['X', 
+0000d110: 2759 272c 2027 5a27 5d5d 5c0a 2020 2020  'Y', 'Z']]\.    
+0000d120: 2020 2020 2020 2020 2020 2020 2e66 696c              .fil
+0000d130: 6c6e 6128 7661 6c75 653d 302c 2069 6e70  lna(value=0, inp
+0000d140: 6c61 6365 3d46 616c 7365 290a 0a20 2020  lace=False)..   
+0000d150: 2020 2020 2020 2020 205f 6c6f 6767 6572           _logger
+0000d160: 2e77 6172 6e69 6e67 2866 2244 7269 7665  .warning(f"Drive
+0000d170: 7220 7b64 7276 3a20 3e32 7d3a 2050 6f73  r {drv: >2}: Pos
+0000d180: 6974 696f 6e20 6461 7461 2069 7320 220a  ition data is ".
+0000d190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1a0: 2020 2020 2020 2020 2020 2020 6622 696e              f"in
+0000d1b0: 636f 6d70 6c65 7465 2122 290a 0a20 2020  complete!")..   
+0000d1c0: 2072 6574 7572 6e20 6461 7461 0a0a 0a40   return data...@
+0000d1d0: 4361 6368 652e 6170 695f 7265 7175 6573  Cache.api_reques
+0000d1e0: 745f 7772 6170 7065 720a 6465 6620 7472  t_wrapper.def tr
+0000d1f0: 6163 6b5f 7374 6174 7573 5f64 6174 6128  ack_status_data(
+0000d200: 7061 7468 2c20 7265 7370 6f6e 7365 3d4e  path, response=N
+0000d210: 6f6e 652c 206c 6976 6564 6174 613d 4e6f  one, livedata=No
+0000d220: 6e65 293a 0a20 2020 2022 2222 0a20 2020  ne):.    """.   
+0000d230: 202e 2e20 7761 726e 696e 673a 3a0a 2020   .. warning::.  
+0000d240: 2020 2020 2020 3a6d 6f64 3a60 6661 7374        :mod:`fast
+0000d250: 6631 2e61 7069 6020 7769 6c6c 2062 6520  f1.api` will be 
+0000d260: 636f 6e73 6964 6572 6564 2070 7269 7661  considered priva
+0000d270: 7465 2069 6e20 6675 7475 7265 2072 656c  te in future rel
+0000d280: 6561 7365 7320 616e 640a 2020 2020 2020  eases and.      
+0000d290: 2020 706f 7465 6e74 6961 6c6c 7920 6265    potentially be
+0000d2a0: 2072 656d 6f76 6564 206f 7220 6368 616e   removed or chan
+0000d2b0: 6765 642e 0a0a 2020 2020 4665 7463 6820  ged...    Fetch 
+0000d2c0: 616e 6420 7061 7273 6520 7472 6163 6b20  and parse track 
+0000d2d0: 7374 6174 7573 2064 6174 612e 0a0a 2020  status data...  
+0000d2e0: 2020 5472 6163 6b20 7374 6174 7573 2063    Track status c
+0000d2f0: 6f6e 7461 696e 7320 696e 666f 726d 6174  ontains informat
+0000d300: 696f 6e20 6f6e 2079 656c 6c6f 772f 7265  ion on yellow/re
+0000d310: 642f 6772 6565 6e20 666c 6167 732c 2073  d/green flags, s
+0000d320: 6166 6574 7920 6361 7220 616e 6420 7669  afety car and vi
+0000d330: 7274 7561 6c20 7361 6665 7479 2063 6172  rtual safety car
+0000d340: 2e20 4974 2070 726f 7669 6465 7320 7468  . It provides th
+0000d350: 650a 2020 2020 666f 6c6c 6f77 696e 6720  e.    following 
+0000d360: 6461 7461 2063 6861 6e6e 656c 7320 7065  data channels pe
+0000d370: 7220 7361 6d70 6c65 3a0a 0a20 2020 2020  r sample:..     
+0000d380: 2020 202d 2054 696d 6520 2864 6174 6574     - Time (datet
+0000d390: 696d 652e 7469 6d65 6465 6c74 6129 3a20  ime.timedelta): 
+0000d3a0: 7365 7373 696f 6e20 7469 6d65 7374 616d  session timestam
+0000d3b0: 7020 2874 696d 6520 6f6e 6c79 290a 2020  p (time only).  
+0000d3c0: 2020 2020 2020 2d20 5374 6174 7573 2028        - Status (
+0000d3d0: 7374 7229 3a20 636f 6e74 6169 6e73 2074  str): contains t
+0000d3e0: 7261 636b 2073 7461 7475 7320 6368 616e  rack status chan
+0000d3f0: 6765 7320 6173 206e 756d 6572 6963 2076  ges as numeric v
+0000d400: 616c 7565 7320 2864 6573 6372 6962 6564  alues (described
+0000d410: 2062 656c 6f77 290a 2020 2020 2020 2020   below).        
+0000d420: 2d20 4d65 7373 6167 6520 2873 7472 293a  - Message (str):
+0000d430: 2063 6f6e 7461 696e 7320 7468 6520 7361   contains the sa
+0000d440: 6d65 2069 6e66 6f72 6d61 7469 6f6e 2061  me information a
+0000d450: 7320 7374 6174 7573 2062 7574 2069 6e20  s status but in 
+0000d460: 6561 7369 6c79 2075 6e64 6572 7374 616e  easily understan
+0000d470: 6461 626c 650a 2020 2020 2020 2020 2020  dable.          
+0000d480: 776f 7264 7320 2827 5965 6c6c 6f77 272c  words ('Yellow',
+0000d490: 2027 416c 6c43 6c65 6172 272c 2e2e 2e29   'AllClear',...)
+0000d4a0: 0a0a 2020 2020 4120 6e65 7720 7661 6c75  ..    A new valu
+0000d4b0: 6520 6973 2073 656e 7420 6576 6572 7920  e is sent every 
+0000d4c0: 7469 6d65 2074 6865 2074 7261 636b 2073  time the track s
+0000d4d0: 7461 7475 7320 6368 616e 6765 732e 0a0a  tatus changes...
+0000d4e0: 2020 2020 5472 6163 6b20 7374 6174 7573      Track status
+0000d4f0: 2069 7320 696e 6469 6361 7465 6420 7573   is indicated us
+0000d500: 696e 6720 7369 6e67 6c65 2064 6967 6974  ing single digit
+0000d510: 2069 6e74 6567 6572 2073 7461 7475 7320   integer status 
+0000d520: 636f 6465 7320 2861 7320 7374 7269 6e67  codes (as string
+0000d530: 292e 204c 6973 7420 6f66 206b 6e6f 776e  ). List of known
+0000d540: 2073 7461 7475 7365 733a 0a0a 2020 2020   statuses:..    
+0000d550: 2020 2020 2d20 2731 273a 2054 7261 636b      - '1': Track
+0000d560: 2063 6c65 6172 2028 6265 6769 6e6e 696e   clear (beginnin
+0000d570: 6720 6f66 2073 6573 7369 6f6e 206f 7220  g of session or 
+0000d580: 746f 2069 6e64 6963 6174 6520 7468 6520  to indicate the 
+0000d590: 656e 640a 2020 2020 2020 2020 2020 206f  end.           o
+0000d5a0: 6620 616e 6f74 6865 7220 7374 6174 7573  f another status
+0000d5b0: 290a 2020 2020 2020 2020 2d20 2732 273a  ).        - '2':
+0000d5c0: 2059 656c 6c6f 7720 666c 6167 2028 7365   Yellow flag (se
+0000d5d0: 6374 6f72 7320 6172 6520 756e 6b6e 6f77  ctors are unknow
+0000d5e0: 6e29 0a20 2020 2020 2020 202d 2027 3327  n).        - '3'
+0000d5f0: 3a20 3f3f 3f20 4e65 7665 7220 7365 656e  : ??? Never seen
+0000d600: 2073 6f20 6661 722c 2064 6f65 7320 6e6f   so far, does no
+0000d610: 7420 6578 6973 743f 0a20 2020 2020 2020  t exist?.       
+0000d620: 202d 2027 3427 3a20 5361 6665 7479 2043   - '4': Safety C
+0000d630: 6172 0a20 2020 2020 2020 202d 2027 3527  ar.        - '5'
+0000d640: 3a20 5265 6420 466c 6167 0a20 2020 2020  : Red Flag.     
+0000d650: 2020 202d 2027 3627 3a20 5669 7274 7561     - '6': Virtua
+0000d660: 6c20 5361 6665 7479 2043 6172 2064 6570  l Safety Car dep
+0000d670: 6c6f 7965 640a 2020 2020 2020 2020 2d20  loyed.        - 
+0000d680: 2737 273a 2056 6972 7475 616c 2053 6166  '7': Virtual Saf
+0000d690: 6574 7920 4361 7220 656e 6469 6e67 2028  ety Car ending (
+0000d6a0: 4173 2069 6e64 6963 6174 6564 206f 6e20  As indicated on 
+0000d6b0: 7468 6520 6472 6976 6572 7320 7374 6565  the drivers stee
+0000d6c0: 7269 6e67 2077 6865 656c 2c20 6f6e 2074  ring wheel, on t
+0000d6d0: 7620 616e 6420 736f 206f 6e3b 2073 7461  v and so on; sta
+0000d6e0: 7475 7320 2731 270a 2020 2020 2020 2020  tus '1'.        
+0000d6f0: 2020 7769 6c6c 206d 6172 6b20 7468 6520    will mark the 
+0000d700: 6163 7475 616c 2065 6e64 290a 0a20 2020  actual end)..   
+0000d710: 2041 7267 733a 0a20 2020 2020 2020 2070   Args:.        p
+0000d720: 6174 6820 2873 7472 293a 2061 7069 2070  ath (str): api p
+0000d730: 6174 6820 6261 7365 2073 7472 696e 6720  ath base string 
+0000d740: 2875 7375 616c 6c79 2060 6053 6573 7369  (usually ``Sessi
+0000d750: 6f6e 2e61 7069 5f70 6174 6860 6029 0a20  on.api_path``). 
+0000d760: 2020 2020 2020 2072 6573 706f 6e73 653a         response:
+0000d770: 2052 6573 706f 6e73 6520 6173 2072 6574   Response as ret
+0000d780: 7572 6e65 6420 6279 203a 6675 6e63 3a60  urned by :func:`
+0000d790: 6665 7463 685f 7061 6765 6020 6361 6e20  fetch_page` can 
+0000d7a0: 6265 2070 6173 7365 6420 6966 2069 7420  be passed if it 
+0000d7b0: 7761 7320 646f 776e 6c6f 6164 6564 2061  was downloaded a
+0000d7c0: 6c72 6561 6479 2e0a 2020 2020 2020 2020  lready..        
+0000d7d0: 6c69 7665 6461 7461 3a20 416e 2069 6e73  livedata: An ins
+0000d7e0: 7461 6e63 6520 6f66 203a 636c 6173 733a  tance of :class:
+0000d7f0: 6066 6173 7466 312e 6c69 7665 7469 6d69  `fastf1.livetimi
+0000d800: 6e67 2e64 6174 612e 4c69 7665 5469 6d69  ng.data.LiveTimi
+0000d810: 6e67 4461 7461 6020 746f 2075 7365 2061  ngData` to use a
+0000d820: 7320 6120 736f 7572 6365 2069 6e73 7465  s a source inste
+0000d830: 6164 206f 6620 7468 6520 6170 690a 0a20  ad of the api.. 
+0000d840: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+0000d850: 2020 2020 4120 6469 6374 696f 6e61 7279      A dictionary
+0000d860: 2063 6f6e 7461 696e 696e 6720 6f6e 6520   containing one 
+0000d870: 6b65 7920 666f 7220 6561 6368 2064 6174  key for each dat
+0000d880: 6120 6368 616e 6e65 6c20 616e 6420 6120  a channel and a 
+0000d890: 6c69 7374 206f 6620 7661 6c75 6573 2070  list of values p
+0000d8a0: 6572 206b 6579 2e0a 0a20 2020 2052 6169  er key...    Rai
+0000d8b0: 7365 733a 0a20 2020 2020 2020 2053 6573  ses:.        Ses
+0000d8c0: 7369 6f6e 4e6f 7441 7661 696c 6162 6c65  sionNotAvailable
+0000d8d0: 4572 726f 723a 2069 6e20 6361 7365 2074  Error: in case t
+0000d8e0: 6865 2046 3120 6c69 7665 7469 6d69 6e67  he F1 livetiming
+0000d8f0: 2061 7069 2072 6574 7572 6e73 206e 6f20   api returns no 
+0000d900: 6461 7461 0a20 2020 2022 2222 0a20 2020  data.    """.   
+0000d910: 2069 6620 6c69 7665 6461 7461 2069 7320   if livedata is 
+0000d920: 6e6f 7420 4e6f 6e65 2061 6e64 206c 6976  not None and liv
+0000d930: 6564 6174 612e 6861 7328 2754 7261 636b  edata.has('Track
+0000d940: 5374 6174 7573 2729 3a0a 2020 2020 2020  Status'):.      
+0000d950: 2020 2320 646f 6573 206e 6f74 206e 6565    # does not nee
+0000d960: 6420 616e 7920 6675 7274 6865 7220 7072  d any further pr
+0000d970: 6f63 6573 7369 6e67 0a20 2020 2020 2020  ocessing.       
+0000d980: 205f 6c6f 6767 6572 2e69 6e66 6f28 224c   _logger.info("L
+0000d990: 6f61 6469 6e67 2074 7261 636b 2073 7461  oading track sta
+0000d9a0: 7475 7320 6461 7461 2229 0a20 2020 2020  tus data").     
+0000d9b0: 2020 2072 6574 7572 6e20 6c69 7665 6461     return liveda
+0000d9c0: 7461 2e67 6574 2827 5472 6163 6b53 7461  ta.get('TrackSta
+0000d9d0: 7475 7327 290a 2020 2020 656c 6966 2072  tus').    elif r
+0000d9e0: 6573 706f 6e73 6520 6973 204e 6f6e 653a  esponse is None:
+0000d9f0: 0a20 2020 2020 2020 205f 6c6f 6767 6572  .        _logger
+0000da00: 2e69 6e66 6f28 2246 6574 6368 696e 6720  .info("Fetching 
+0000da10: 7472 6163 6b20 7374 6174 7573 2064 6174  track status dat
+0000da20: 612e 2e2e 2229 0a20 2020 2020 2020 2072  a...").        r
+0000da30: 6573 706f 6e73 6520 3d20 6665 7463 685f  esponse = fetch_
+0000da40: 7061 6765 2870 6174 682c 2027 7472 6163  page(path, 'trac
+0000da50: 6b5f 7374 6174 7573 2729 0a20 2020 2020  k_status').     
+0000da60: 2020 2069 6620 7265 7370 6f6e 7365 2069     if response i
+0000da70: 7320 4e6f 6e65 3a20 2023 206e 6f20 7265  s None:  # no re
+0000da80: 7370 6f6e 7365 2072 6563 6569 7665 640a  sponse received.
+0000da90: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0000daa0: 6520 5365 7373 696f 6e4e 6f74 4176 6169  e SessionNotAvai
+0000dab0: 6c61 626c 6545 7272 6f72 280a 2020 2020  lableError(.    
+0000dac0: 2020 2020 2020 2020 2020 2020 224e 6f20              "No 
+0000dad0: 6461 7461 2066 6f72 2074 6869 7320 7365  data for this se
+0000dae0: 7373 696f 6e21 2049 6620 7468 6973 2073  ssion! If this s
+0000daf0: 6573 7369 6f6e 206f 6e6c 7920 6669 6e69  ession only fini
+0000db00: 7368 6564 2022 0a20 2020 2020 2020 2020  shed ".         
+0000db10: 2020 2020 2020 2022 7265 6365 6e74 6c79         "recently
+0000db20: 2c20 706c 6561 7365 2074 7279 2061 6761  , please try aga
+0000db30: 696e 2069 6e20 6120 6665 7720 6d69 6e75  in in a few minu
+0000db40: 7465 732e 220a 2020 2020 2020 2020 2020  tes.".          
+0000db50: 2020 290a 0a20 2020 2064 6174 6120 3d20    )..    data = 
+0000db60: 7b27 5469 6d65 273a 205b 5d2c 2027 5374  {'Time': [], 'St
+0000db70: 6174 7573 273a 205b 5d2c 2027 4d65 7373  atus': [], 'Mess
+0000db80: 6167 6527 3a20 5b5d 7d0a 0a20 2020 2066  age': []}..    f
+0000db90: 6f72 2065 6e74 7279 2069 6e20 7265 7370  or entry in resp
+0000dba0: 6f6e 7365 3a0a 2020 2020 2020 2020 6966  onse:.        if
+0000dbb0: 206c 656e 2865 6e74 7279 2920 3c20 323a   len(entry) < 2:
+0000dbc0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+0000dbd0: 7469 6e75 650a 2020 2020 2020 2020 726f  tinue.        ro
+0000dbe0: 7720 3d20 656e 7472 795b 315d 0a20 2020  w = entry[1].   
+0000dbf0: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
+0000dc00: 7374 616e 6365 2872 6f77 2c20 6469 6374  stance(row, dict
+0000dc10: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
+0000dc20: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
+0000dc30: 6461 7461 5b27 5469 6d65 275d 2e61 7070  data['Time'].app
+0000dc40: 656e 6428 746f 5f74 696d 6564 656c 7461  end(to_timedelta
+0000dc50: 2865 6e74 7279 5b30 5d29 290a 2020 2020  (entry[0])).    
+0000dc60: 2020 2020 6461 7461 5b27 5374 6174 7573      data['Status
+0000dc70: 275d 2e61 7070 656e 6428 726f 772e 6765  '].append(row.ge
+0000dc80: 7428 2753 7461 7475 7327 2c20 2727 2929  t('Status', ''))
+0000dc90: 0a20 2020 2020 2020 2064 6174 615b 274d  .        data['M
+0000dca0: 6573 7361 6765 275d 2e61 7070 656e 6428  essage'].append(
+0000dcb0: 726f 772e 6765 7428 274d 6573 7361 6765  row.get('Message
+0000dcc0: 272c 2027 2729 290a 0a20 2020 2072 6574  ', ''))..    ret
+0000dcd0: 7572 6e20 6461 7461 0a0a 0a40 4361 6368  urn data...@Cach
+0000dce0: 652e 6170 695f 7265 7175 6573 745f 7772  e.api_request_wr
+0000dcf0: 6170 7065 720a 6465 6620 7365 7373 696f  apper.def sessio
+0000dd00: 6e5f 7374 6174 7573 5f64 6174 6128 7061  n_status_data(pa
+0000dd10: 7468 2c20 7265 7370 6f6e 7365 3d4e 6f6e  th, response=Non
+0000dd20: 652c 206c 6976 6564 6174 613d 4e6f 6e65  e, livedata=None
+0000dd30: 293a 0a20 2020 2022 2222 0a20 2020 202e  ):.    """.    .
+0000dd40: 2e20 7761 726e 696e 673a 3a0a 2020 2020  . warning::.    
+0000dd50: 2020 2020 3a6d 6f64 3a60 6661 7374 6631      :mod:`fastf1
+0000dd60: 2e61 7069 6020 7769 6c6c 2062 6520 636f  .api` will be co
+0000dd70: 6e73 6964 6572 6564 2070 7269 7661 7465  nsidered private
+0000dd80: 2069 6e20 6675 7475 7265 2072 656c 6561   in future relea
+0000dd90: 7365 7320 616e 640a 2020 2020 2020 2020  ses and.        
+0000dda0: 706f 7465 6e74 6961 6c6c 7920 6265 2072  potentially be r
+0000ddb0: 656d 6f76 6564 206f 7220 6368 616e 6765  emoved or change
+0000ddc0: 642e 0a0a 2020 2020 4665 7463 6820 616e  d...    Fetch an
+0000ddd0: 6420 7061 7273 6520 7365 7373 696f 6e20  d parse session 
+0000dde0: 7374 6174 7573 2064 6174 612e 0a0a 2020  status data...  
+0000ddf0: 2020 5365 7373 696f 6e20 7374 6174 7573    Session status
+0000de00: 2063 6f6e 7461 696e 7320 696e 666f 726d   contains inform
+0000de10: 6174 696f 6e20 6f6e 2077 6865 6e20 6120  ation on when a 
+0000de20: 7365 7373 696f 6e20 7761 7320 7374 6172  session was star
+0000de30: 7465 6420 616e 6420 7768 656e 2069 7420  ted and when it 
+0000de40: 656e 6465 6420 2861 6d6f 6e67 7374 206f  ended (amongst o
+0000de50: 7468 6572 7329 2e20 4974 0a20 2020 2070  thers). It.    p
+0000de60: 726f 7669 6465 7320 7468 6520 666f 6c6c  rovides the foll
+0000de70: 6f77 696e 6720 6461 7461 2063 6861 6e6e  owing data chann
+0000de80: 656c 7320 7065 7220 7361 6d70 6c65 3a0a  els per sample:.
+0000de90: 0a20 2020 2020 2020 202d 2054 696d 6520  .        - Time 
+0000dea0: 2864 6174 6574 696d 652e 7469 6d65 6465  (datetime.timede
+0000deb0: 6c74 6129 3a20 7365 7373 696f 6e20 7469  lta): session ti
+0000dec0: 6d65 7374 616d 7020 2874 696d 6520 6f6e  mestamp (time on
+0000ded0: 6c79 290a 2020 2020 2020 2020 2d20 5374  ly).        - St
+0000dee0: 6174 7573 2028 7374 7229 3a20 7374 6174  atus (str): stat
+0000def0: 7573 206d 6573 7361 6765 730a 0a20 2020  us messages..   
+0000df00: 2041 206e 6577 2076 616c 7565 2069 7320   A new value is 
+0000df10: 7365 6e74 2065 7665 7279 2074 696d 6520  sent every time 
+0000df20: 7468 6520 7365 7373 696f 6e20 7374 6174  the session stat
+0000df30: 7573 2063 6861 6e67 6573 2e0a 0a20 2020  us changes...   
+0000df40: 2041 7267 733a 0a20 2020 2020 2020 2070   Args:.        p
+0000df50: 6174 6820 2873 7472 293a 2061 7069 2070  ath (str): api p
+0000df60: 6174 6820 6261 7365 2073 7472 696e 6720  ath base string 
+0000df70: 2875 7375 616c 6c79 2060 6053 6573 7369  (usually ``Sessi
+0000df80: 6f6e 2e61 7069 5f70 6174 6860 6029 0a20  on.api_path``). 
+0000df90: 2020 2020 2020 2072 6573 706f 6e73 653a         response:
+0000dfa0: 2052 6573 706f 6e73 6520 6173 2072 6574   Response as ret
+0000dfb0: 7572 6e65 6420 6279 203a 6675 6e63 3a60  urned by :func:`
+0000dfc0: 6665 7463 685f 7061 6765 6020 6361 6e20  fetch_page` can 
+0000dfd0: 6265 2070 6173 7365 6420 6966 2069 7420  be passed if it 
+0000dfe0: 7761 7320 646f 776e 6c6f 6164 6564 2061  was downloaded a
+0000dff0: 6c72 6561 6479 2e0a 2020 2020 2020 2020  lready..        
+0000e000: 6c69 7665 6461 7461 3a20 416e 2069 6e73  livedata: An ins
+0000e010: 7461 6e63 6520 6f66 203a 636c 6173 733a  tance of :class:
+0000e020: 6066 6173 7466 312e 6c69 7665 7469 6d69  `fastf1.livetimi
+0000e030: 6e67 2e64 6174 612e 4c69 7665 5469 6d69  ng.data.LiveTimi
+0000e040: 6e67 4461 7461 6020 746f 2075 7365 2061  ngData` to use a
+0000e050: 7320 6120 736f 7572 6365 2069 6e73 7465  s a source inste
+0000e060: 6164 206f 6620 7468 6520 6170 690a 0a20  ad of the api.. 
+0000e070: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+0000e080: 2020 2020 4120 6469 6374 696f 6e61 7279      A dictionary
+0000e090: 2063 6f6e 7461 696e 696e 6720 6f6e 6520   containing one 
+0000e0a0: 6b65 7920 666f 7220 6561 6368 2064 6174  key for each dat
+0000e0b0: 6120 6368 616e 6e65 6c20 616e 6420 6120  a channel and a 
+0000e0c0: 6c69 7374 206f 6620 7661 6c75 6573 2070  list of values p
+0000e0d0: 6572 206b 6579 2e0a 0a20 2020 2052 6169  er key...    Rai
+0000e0e0: 7365 733a 0a20 2020 2020 2020 2053 6573  ses:.        Ses
+0000e0f0: 7369 6f6e 4e6f 7441 7661 696c 6162 6c65  sionNotAvailable
+0000e100: 4572 726f 723a 2069 6e20 6361 7365 2074  Error: in case t
+0000e110: 6865 2046 3120 6c69 7665 7469 6d69 6e67  he F1 livetiming
+0000e120: 2061 7069 2072 6574 7572 6e73 206e 6f20   api returns no 
+0000e130: 6461 7461 0a20 2020 2022 2222 0a20 2020  data.    """.   
+0000e140: 2069 6620 6c69 7665 6461 7461 2069 7320   if livedata is 
+0000e150: 6e6f 7420 4e6f 6e65 2061 6e64 206c 6976  not None and liv
+0000e160: 6564 6174 612e 6861 7328 2753 6573 7369  edata.has('Sessi
+0000e170: 6f6e 5374 6174 7573 2729 3a0a 2020 2020  onStatus'):.    
+0000e180: 2020 2020 2320 646f 6573 206e 6f74 206e      # does not n
+0000e190: 6565 6420 616e 7920 6675 7274 6865 7220  eed any further 
+0000e1a0: 7072 6f63 6573 7369 6e67 0a20 2020 2020  processing.     
+0000e1b0: 2020 205f 6c6f 6767 6572 2e69 6e66 6f28     _logger.info(
+0000e1c0: 224c 6f61 6469 6e67 2073 6573 7369 6f6e  "Loading session
+0000e1d0: 2073 7461 7475 7320 6461 7461 2229 0a20   status data"). 
+0000e1e0: 2020 2020 2020 2072 6574 7572 6e20 6c69         return li
+0000e1f0: 7665 6461 7461 2e67 6574 2827 5365 7373  vedata.get('Sess
+0000e200: 696f 6e53 7461 7475 7327 290a 2020 2020  ionStatus').    
+0000e210: 656c 6966 2072 6573 706f 6e73 6520 6973  elif response is
+0000e220: 204e 6f6e 653a 0a20 2020 2020 2020 205f   None:.        _
+0000e230: 6c6f 6767 6572 2e69 6e66 6f28 2246 6574  logger.info("Fet
+0000e240: 6368 696e 6720 7365 7373 696f 6e20 7374  ching session st
+0000e250: 6174 7573 2064 6174 612e 2e2e 2229 0a20  atus data..."). 
+0000e260: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+0000e270: 3d20 6665 7463 685f 7061 6765 2870 6174  = fetch_page(pat
+0000e280: 682c 2027 7365 7373 696f 6e5f 7374 6174  h, 'session_stat
+0000e290: 7573 2729 0a20 2020 2020 2020 2069 6620  us').        if 
+0000e2a0: 7265 7370 6f6e 7365 2069 7320 4e6f 6e65  response is None
+0000e2b0: 3a20 2023 206e 6f20 7265 7370 6f6e 7365  :  # no response
+0000e2c0: 2072 6563 6569 7665 640a 2020 2020 2020   received.      
+0000e2d0: 2020 2020 2020 7261 6973 6520 5365 7373        raise Sess
+0000e2e0: 696f 6e4e 6f74 4176 6169 6c61 626c 6545  ionNotAvailableE
+0000e2f0: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+0000e300: 2020 2020 2020 224e 6f20 6461 7461 2066        "No data f
+0000e310: 6f72 2074 6869 7320 7365 7373 696f 6e21  or this session!
+0000e320: 2049 6620 7468 6973 2073 6573 7369 6f6e   If this session
+0000e330: 206f 6e6c 7920 6669 6e69 7368 6564 2022   only finished "
+0000e340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e350: 2022 7265 6365 6e74 6c79 2c20 706c 6561   "recently, plea
+0000e360: 7365 2074 7279 2061 6761 696e 2069 6e20  se try again in 
+0000e370: 6120 6665 7720 6d69 6e75 7465 732e 220a  a few minutes.".
+0000e380: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+0000e390: 2020 2064 6174 6120 3d20 7b27 5469 6d65     data = {'Time
+0000e3a0: 273a 205b 5d2c 2027 5374 6174 7573 273a  ': [], 'Status':
+0000e3b0: 205b 5d7d 0a0a 2020 2020 666f 7220 656e   []}..    for en
+0000e3c0: 7472 7920 696e 2072 6573 706f 6e73 653a  try in response:
+0000e3d0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+0000e3e0: 656e 7472 7929 203c 2032 3a0a 2020 2020  entry) < 2:.    
+0000e3f0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+0000e400: 0a20 2020 2020 2020 2072 6f77 203d 2065  .        row = e
+0000e410: 6e74 7279 5b31 5d0a 2020 2020 2020 2020  ntry[1].        
+0000e420: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+0000e430: 6528 726f 772c 2064 6963 7429 206f 7220  e(row, dict) or 
+0000e440: 2753 7461 7475 7327 206e 6f74 2069 6e20  'Status' not in 
+0000e450: 726f 773a 0a20 2020 2020 2020 2020 2020  row:.           
+0000e460: 2063 6f6e 7469 6e75 650a 0a20 2020 2020   continue..     
+0000e470: 2020 2064 6174 615b 2754 696d 6527 5d2e     data['Time'].
+0000e480: 6170 7065 6e64 2874 6f5f 7469 6d65 6465  append(to_timede
+0000e490: 6c74 6128 656e 7472 795b 305d 2929 0a20  lta(entry[0])). 
+0000e4a0: 2020 2020 2020 2064 6174 615b 2753 7461         data['Sta
+0000e4b0: 7475 7327 5d2e 6170 7065 6e64 2872 6f77  tus'].append(row
+0000e4c0: 5b27 5374 6174 7573 275d 290a 0a20 2020  ['Status'])..   
+0000e4d0: 2072 6574 7572 6e20 6461 7461 0a0a 0a40   return data...@
+0000e4e0: 4361 6368 652e 6170 695f 7265 7175 6573  Cache.api_reques
+0000e4f0: 745f 7772 6170 7065 720a 6465 6620 7261  t_wrapper.def ra
+0000e500: 6365 5f63 6f6e 7472 6f6c 5f6d 6573 7361  ce_control_messa
+0000e510: 6765 7328 7061 7468 2c20 7265 7370 6f6e  ges(path, respon
+0000e520: 7365 3d4e 6f6e 652c 206c 6976 6564 6174  se=None, livedat
+0000e530: 613d 4e6f 6e65 293a 0a20 2020 2022 2222  a=None):.    """
+0000e540: 0a20 2020 202e 2e20 7761 726e 696e 673a  .    .. warning:
+0000e550: 3a0a 2020 2020 2020 2020 3a6d 6f64 3a60  :.        :mod:`
+0000e560: 6661 7374 6631 2e61 7069 6020 7769 6c6c  fastf1.api` will
+0000e570: 2062 6520 636f 6e73 6964 6572 6564 2070   be considered p
+0000e580: 7269 7661 7465 2069 6e20 6675 7475 7265  rivate in future
+0000e590: 2072 656c 6561 7365 7320 616e 640a 2020   releases and.  
+0000e5a0: 2020 2020 2020 706f 7465 6e74 6961 6c6c        potentiall
+0000e5b0: 7920 6265 2072 656d 6f76 6564 206f 7220  y be removed or 
+0000e5c0: 6368 616e 6765 642e 0a0a 2020 2020 4665  changed...    Fe
+0000e5d0: 7463 6820 616e 6420 7061 7273 6520 7261  tch and parse ra
+0000e5e0: 6365 2063 6f6e 7472 6f6c 206d 6573 7361  ce control messa
+0000e5f0: 6765 732e 0a0a 2020 2020 5261 6365 2063  ges...    Race c
+0000e600: 6f6e 7472 6f6c 206d 6573 7361 6765 7320  ontrol messages 
+0000e610: 6172 6520 7365 6e74 2062 7920 7261 6365  are sent by race
+0000e620: 2063 6f6e 7472 6f6c 2074 6f20 616c 6c20   control to all 
+0000e630: 7465 616d 7320 746f 206e 6f74 6966 7920  teams to notify 
+0000e640: 6f66 0a20 2020 2064 6563 6973 696f 6e73  of.    decisions
+0000e650: 2061 6e64 2073 7461 7475 7365 7320 6f66   and statuses of
+0000e660: 2074 6865 2073 6573 7369 6f6e 2e0a 0a20   the session... 
+0000e670: 2020 2045 7665 7279 206d 6573 7361 6765     Every message
+0000e680: 2068 6173 2074 6865 2066 6f6c 6c6f 7769   has the followi
+0000e690: 6e67 2061 7474 7269 6275 7465 733a 0a0a  ng attributes:..
+0000e6a0: 2020 2020 2020 2020 2d20 5574 633a 204d          - Utc: M
+0000e6b0: 6573 7361 6765 2074 696d 6573 7461 6d70  essage timestamp
+0000e6c0: 0a20 2020 2020 2020 202d 2043 6174 6567  .        - Categ
+0000e6d0: 6f72 7920 2873 7472 293a 2054 7970 6520  ory (str): Type 
+0000e6e0: 6f66 206d 6573 7361 6765 2c20 224f 7468  of message, "Oth
+0000e6f0: 6572 222c 2022 466c 6167 222c 2022 4472  er", "Flag", "Dr
+0000e700: 7322 2c20 2243 6172 4576 656e 7422 0a20  s", "CarEvent". 
+0000e710: 2020 2020 2020 202d 204d 6573 7361 6765         - Message
+0000e720: 2028 7374 7229 3a20 436f 6e74 656e 7420   (str): Content 
+0000e730: 6f66 206d 6573 7361 6765 0a0a 2020 2020  of message..    
+0000e740: 4f74 6865 7220 706f 7373 6962 6c65 2061  Other possible a
+0000e750: 7474 7269 6275 7465 7320 6172 653a 0a0a  ttributes are:..
+0000e760: 2020 2020 2020 2020 2d20 5374 6174 7573          - Status
+0000e770: 2028 7374 7229 3a20 5374 6174 7573 206f   (str): Status o
+0000e780: 6620 636f 6e74 6578 742c 2065 2e67 2e20  f context, e.g. 
+0000e790: 2244 4953 4142 4c45 4422 2066 6f72 2064  "DISABLED" for d
+0000e7a0: 6973 6162 6c69 6e67 2044 5253 0a20 2020  isabling DRS.   
+0000e7b0: 2020 2020 202d 2046 6c61 6720 2873 7472       - Flag (str
+0000e7c0: 293a 2054 7970 6520 6f66 2066 6c61 6720  ): Type of flag 
+0000e7d0: 6265 696e 6720 7761 7665 6420 2247 5245  being waved "GRE
+0000e7e0: 454e 222c 2022 5245 4422 2c20 2259 454c  EN", "RED", "YEL
+0000e7f0: 4c4f 5722 2c0a 2020 2020 2020 2020 2020  LOW",.          
+0000e800: 2243 4c45 4152 222c 2022 4348 4551 5545  "CLEAR", "CHEQUE
+0000e810: 5245 4422 0a20 2020 2020 2020 202d 2053  RED".        - S
+0000e820: 636f 7065 2028 7374 7229 3a20 5363 6f70  cope (str): Scop
+0000e830: 6520 6f66 206d 6573 7361 6765 2022 5472  e of message "Tr
+0000e840: 6163 6b22 2c20 2253 6563 746f 7222 2c20  ack", "Sector", 
+0000e850: 2244 7269 7665 7222 0a20 2020 2020 2020  "Driver".       
+0000e860: 202d 2053 6563 746f 7220 2869 6e74 293a   - Sector (int):
+0000e870: 2041 6666 6563 7465 6420 7472 6163 6b20   Affected track 
+0000e880: 7365 6374 6f72 2066 6f72 2073 6563 746f  sector for secto
+0000e890: 722d 7363 6f70 6564 206d 6573 7361 6765  r-scoped message
+0000e8a0: 730a 2020 2020 2020 2020 2d20 5261 6369  s.        - Raci
+0000e8b0: 6e67 4e75 6d62 6572 2028 7374 7229 3a20  ngNumber (str): 
+0000e8c0: 4166 6665 6374 6564 2064 7269 7665 7220  Affected driver 
+0000e8d0: 666f 7220 4361 7245 7665 6e74 206d 6573  for CarEvent mes
+0000e8e0: 7361 6765 730a 2020 2020 2020 2020 2d20  sages.        - 
+0000e8f0: 4c61 7020 2869 6e74 293a 204e 756d 6265  Lap (int): Numbe
+0000e900: 7220 6f66 2074 6865 206c 6170 2069 6e20  r of the lap in 
+0000e910: 7768 6963 6820 7468 6520 6d65 7373 6167  which the messag
+0000e920: 6520 7761 7320 6469 7370 6c61 7965 640a  e was displayed.
+0000e930: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
+0000e940: 2020 2070 6174 6820 2873 7472 293a 2061     path (str): a
+0000e950: 7069 2070 6174 6820 6261 7365 2073 7472  pi path base str
+0000e960: 696e 6720 2875 7375 616c 6c79 2060 6053  ing (usually ``S
+0000e970: 6573 7369 6f6e 2e61 7069 5f70 6174 6860  ession.api_path`
+0000e980: 6029 0a20 2020 2020 2020 2072 6573 706f  `).        respo
+0000e990: 6e73 653a 2052 6573 706f 6e73 6520 6173  nse: Response as
+0000e9a0: 2072 6574 7572 6e65 6420 6279 203a 6675   returned by :fu
+0000e9b0: 6e63 3a60 6665 7463 685f 7061 6765 6020  nc:`fetch_page` 
+0000e9c0: 6361 6e20 6265 2070 6173 7365 6420 6966  can be passed if
+0000e9d0: 0a20 2020 2020 2020 2020 2020 2069 7420  .            it 
+0000e9e0: 7761 7320 646f 776e 6c6f 6164 6564 2061  was downloaded a
+0000e9f0: 6c72 6561 6479 2e0a 2020 2020 2020 2020  lready..        
+0000ea00: 6c69 7665 6461 7461 3a20 416e 2069 6e73  livedata: An ins
+0000ea10: 7461 6e63 6520 6f66 0a20 2020 2020 2020  tance of.       
+0000ea20: 2020 2020 203a 636c 6173 733a 6066 6173       :class:`fas
+0000ea30: 7466 312e 6c69 7665 7469 6d69 6e67 2e64  tf1.livetiming.d
+0000ea40: 6174 612e 4c69 7665 5469 6d69 6e67 4461  ata.LiveTimingDa
+0000ea50: 7461 6020 746f 2075 7365 2061 7320 6120  ta` to use as a 
+0000ea60: 736f 7572 6365 0a20 2020 2020 2020 2020  source.         
+0000ea70: 2020 2069 6e73 7465 6164 206f 6620 7468     instead of th
+0000ea80: 6520 6170 690a 0a20 2020 2052 6574 7572  e api..    Retur
+0000ea90: 6e73 3a0a 2020 2020 2020 2020 4120 6469  ns:.        A di
+0000eaa0: 6374 696f 6e61 7279 2063 6f6e 7461 696e  ctionary contain
+0000eab0: 696e 6720 6f6e 6520 6b65 7920 666f 7220  ing one key for 
+0000eac0: 6561 6368 2064 6174 6120 6368 616e 6e65  each data channe
+0000ead0: 6c20 616e 6420 6120 6c69 7374 206f 660a  l and a list of.
+0000eae0: 2020 2020 2020 2020 7661 6c75 6573 2070          values p
+0000eaf0: 6572 206b 6579 2e0a 0a20 2020 2052 6169  er key...    Rai
+0000eb00: 7365 733a 0a20 2020 2020 2020 2053 6573  ses:.        Ses
+0000eb10: 7369 6f6e 4e6f 7441 7661 696c 6162 6c65  sionNotAvailable
+0000eb20: 4572 726f 723a 2069 6e20 6361 7365 2074  Error: in case t
+0000eb30: 6865 2046 3120 6c69 7665 7469 6d69 6e67  he F1 livetiming
+0000eb40: 2061 7069 2072 6574 7572 6e73 206e 6f20   api returns no 
+0000eb50: 6461 7461 0a20 2020 2022 2222 0a20 2020  data.    """.   
+0000eb60: 2069 6620 6c69 7665 6461 7461 2069 7320   if livedata is 
+0000eb70: 6e6f 7420 4e6f 6e65 2061 6e64 206c 6976  not None and liv
+0000eb80: 6564 6174 612e 6861 7328 2752 6163 6543  edata.has('RaceC
+0000eb90: 6f6e 7472 6f6c 4d65 7373 6167 6573 2729  ontrolMessages')
+0000eba0: 3a0a 2020 2020 2020 2020 2320 646f 6573  :.        # does
+0000ebb0: 206e 6f74 206e 6565 6420 616e 7920 6675   not need any fu
+0000ebc0: 7274 6865 7220 7072 6f63 6573 7369 6e67  rther processing
+0000ebd0: 0a20 2020 2020 2020 205f 6c6f 6767 6572  .        _logger
+0000ebe0: 2e69 6e66 6f28 224c 6f61 6469 6e67 2072  .info("Loading r
+0000ebf0: 6163 6520 636f 6e74 726f 6c20 6d65 7373  ace control mess
+0000ec00: 6167 6573 2229 0a20 2020 2020 2020 2072  ages").        r
+0000ec10: 6574 7572 6e20 6c69 7665 6461 7461 2e67  eturn livedata.g
+0000ec20: 6574 2827 5261 6365 436f 6e74 726f 6c4d  et('RaceControlM
+0000ec30: 6573 7361 6765 7327 290a 2020 2020 656c  essages').    el
+0000ec40: 6966 2072 6573 706f 6e73 6520 6973 204e  if response is N
+0000ec50: 6f6e 653a 0a20 2020 2020 2020 205f 6c6f  one:.        _lo
+0000ec60: 6767 6572 2e69 6e66 6f28 2246 6574 6368  gger.info("Fetch
+0000ec70: 696e 6720 7261 6365 2063 6f6e 7472 6f6c  ing race control
+0000ec80: 206d 6573 7361 6765 732e 2e2e 2229 0a20   messages..."). 
+0000ec90: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+0000eca0: 3d20 6665 7463 685f 7061 6765 2870 6174  = fetch_page(pat
+0000ecb0: 682c 2027 7261 6365 5f63 6f6e 7472 6f6c  h, 'race_control
+0000ecc0: 5f6d 6573 7361 6765 7327 290a 2020 2020  _messages').    
+0000ecd0: 2020 2020 6966 2072 6573 706f 6e73 6520      if response 
+0000ece0: 6973 204e 6f6e 653a 2020 2320 6e6f 2072  is None:  # no r
+0000ecf0: 6573 706f 6e73 6520 7265 6365 6976 6564  esponse received
+0000ed00: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+0000ed10: 7365 2053 6573 7369 6f6e 4e6f 7441 7661  se SessionNotAva
+0000ed20: 696c 6162 6c65 4572 726f 7228 0a20 2020  ilableError(.   
+0000ed30: 2020 2020 2020 2020 2020 2020 2022 4e6f               "No
+0000ed40: 2064 6174 6120 666f 7220 7468 6973 2073   data for this s
+0000ed50: 6573 7369 6f6e 2120 4966 2074 6869 7320  ession! If this 
+0000ed60: 7365 7373 696f 6e20 6f6e 6c79 2066 696e  session only fin
+0000ed70: 6973 6865 6420 220a 2020 2020 2020 2020  ished ".        
+0000ed80: 2020 2020 2020 2020 2272 6563 656e 746c          "recentl
+0000ed90: 792c 2070 6c65 6173 6520 7472 7920 6167  y, please try ag
+0000eda0: 6169 6e20 696e 2061 2066 6577 206d 696e  ain in a few min
+0000edb0: 7574 6573 2e22 0a20 2020 2020 2020 2020  utes.".         
+0000edc0: 2020 2029 0a0a 2020 2020 6461 7461 203d     )..    data =
+0000edd0: 207b 0a20 2020 2020 2020 2027 5469 6d65   {.        'Time
+0000ede0: 273a 205b 5d2c 2027 4361 7465 676f 7279  ': [], 'Category
+0000edf0: 273a 205b 5d2c 2027 4d65 7373 6167 6527  ': [], 'Message'
+0000ee00: 3a20 5b5d 2c20 2753 7461 7475 7327 3a20  : [], 'Status': 
+0000ee10: 5b5d 2c0a 2020 2020 2020 2020 2746 6c61  [],.        'Fla
+0000ee20: 6727 3a20 5b5d 2c20 2753 636f 7065 273a  g': [], 'Scope':
+0000ee30: 205b 5d2c 2027 5365 6374 6f72 273a 205b   [], 'Sector': [
+0000ee40: 5d2c 2027 5261 6369 6e67 4e75 6d62 6572  ], 'RacingNumber
+0000ee50: 273a 205b 5d2c 2027 4c61 7027 3a20 5b5d  ': [], 'Lap': []
+0000ee60: 0a20 2020 207d 0a20 2020 2064 6174 615f  .    }.    data_
+0000ee70: 6b65 7973 203d 2028 2743 6174 6567 6f72  keys = ('Categor
+0000ee80: 7927 2c20 274d 6573 7361 6765 272c 2027  y', 'Message', '
+0000ee90: 5374 6174 7573 272c 2027 466c 6167 272c  Status', 'Flag',
+0000eea0: 2027 5363 6f70 6527 2c20 2753 6563 746f   'Scope', 'Secto
+0000eeb0: 7227 2c0a 2020 2020 2020 2020 2020 2020  r',.            
+0000eec0: 2020 2020 2027 5261 6369 6e67 4e75 6d62       'RacingNumb
+0000eed0: 6572 272c 2027 4c61 7027 290a 2020 2020  er', 'Lap').    
+0000eee0: 636f 6e76 6572 7465 7273 203d 2028 7374  converters = (st
+0000eef0: 722c 2073 7472 2c20 7374 722c 2073 7472  r, str, str, str
+0000ef00: 2c20 7374 722c 2069 6e74 2c20 7374 722c  , str, int, str,
+0000ef10: 2069 6e74 290a 0a20 2020 2066 6f72 206c   int)..    for l
+0000ef20: 696e 6520 696e 2072 6573 706f 6e73 653a  ine in response:
+0000ef30: 0a20 2020 2020 2020 206d 6573 7361 6765  .        message
+0000ef40: 7320 3d20 6c69 6e65 5b31 5d5b 274d 6573  s = line[1]['Mes
+0000ef50: 7361 6765 7327 5d0a 2020 2020 2020 2020  sages'].        
+0000ef60: 6966 2069 7369 6e73 7461 6e63 6528 6d65  if isinstance(me
+0000ef70: 7373 6167 6573 2c20 6469 6374 293a 0a20  ssages, dict):. 
+0000ef80: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+0000ef90: 6765 7320 3d20 6c69 7374 286d 6573 7361  ges = list(messa
+0000efa0: 6765 732e 7661 6c75 6573 2829 290a 2020  ges.values()).  
+0000efb0: 2020 2020 2020 666f 7220 656e 7472 7920        for entry 
+0000efc0: 696e 206d 6573 7361 6765 733a 0a20 2020  in messages:.   
+0000efd0: 2020 2020 2020 2020 2064 6174 615b 2754           data['T
+0000efe0: 696d 6527 5d2e 6170 7065 6e64 2874 6f5f  ime'].append(to_
+0000eff0: 6461 7465 7469 6d65 2865 6e74 7279 5b27  datetime(entry['
+0000f000: 5574 6327 5d29 290a 0a20 2020 2020 2020  Utc']))..       
+0000f010: 2020 2020 2066 6f72 206b 6579 2c20 636f       for key, co
+0000f020: 6e76 2069 6e20 7a69 7028 6461 7461 5f6b  nv in zip(data_k
+0000f030: 6579 732c 2063 6f6e 7665 7274 6572 7329  eys, converters)
+0000f040: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000f050: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+0000f060: 2020 2020 2020 2020 2020 2064 6174 615b             data[
+0000f070: 6b65 795d 2e61 7070 656e 6428 636f 6e76  key].append(conv
+0000f080: 2865 6e74 7279 5b6b 6579 5d29 290a 2020  (entry[key])).  
+0000f090: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+0000f0a0: 6365 7074 2028 4b65 7945 7272 6f72 2c20  cept (KeyError, 
+0000f0b0: 5661 6c75 6545 7272 6f72 293a 0a20 2020  ValueError):.   
+0000f0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0d0: 2023 2074 7970 6520 636f 6e76 6572 7369   # type conversi
+0000f0e0: 6f6e 2066 6169 6c65 6420 6f72 206b 6579  on failed or key
+0000f0f0: 2069 7320 6d69 7373 696e 670a 2020 2020   is missing.    
+0000f100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f110: 6461 7461 5b6b 6579 5d2e 6170 7065 6e64  data[key].append
+0000f120: 284e 6f6e 6529 0a0a 2020 2020 7265 7475  (None)..    retu
+0000f130: 726e 2064 6174 610a 0a0a 4043 6163 6865  rn data...@Cache
+0000f140: 2e61 7069 5f72 6571 7565 7374 5f77 7261  .api_request_wra
+0000f150: 7070 6572 0a64 6566 206c 6170 5f63 6f75  pper.def lap_cou
+0000f160: 6e74 2870 6174 682c 2072 6573 706f 6e73  nt(path, respons
+0000f170: 653d 4e6f 6e65 2c20 6c69 7665 6461 7461  e=None, livedata
+0000f180: 3d4e 6f6e 6529 3a0a 2020 2020 2222 220a  =None):.    """.
+0000f190: 2020 2020 2e2e 2077 6172 6e69 6e67 3a3a      .. warning::
+0000f1a0: 0a20 2020 2020 2020 203a 6d6f 643a 6066  .        :mod:`f
+0000f1b0: 6173 7466 312e 6170 6960 2077 696c 6c20  astf1.api` will 
+0000f1c0: 6265 2063 6f6e 7369 6465 7265 6420 7072  be considered pr
+0000f1d0: 6976 6174 6520 696e 2066 7574 7572 6520  ivate in future 
+0000f1e0: 7265 6c65 6173 6573 2061 6e64 0a20 2020  releases and.   
+0000f1f0: 2020 2020 2070 6f74 656e 7469 616c 6c79       potentially
+0000f200: 2062 6520 7265 6d6f 7665 6420 6f72 2063   be removed or c
+0000f210: 6861 6e67 6564 2e0a 0a20 2020 2046 6574  hanged...    Fet
+0000f220: 6368 2061 6e64 2070 6172 7365 206c 6170  ch and parse lap
+0000f230: 2063 6f75 6e74 2064 6174 612e 0a0a 2020   count data...  
+0000f240: 2020 4974 2070 726f 7669 6465 7320 7468    It provides th
+0000f250: 6520 666f 6c6c 6f77 696e 6720 6461 7461  e following data
+0000f260: 2063 6861 6e6e 656c 7320 7065 7220 7361   channels per sa
+0000f270: 6d70 6c65 3a0a 2020 2020 2020 2020 2d20  mple:.        - 
+0000f280: 5469 6d65 3a20 7365 7373 696f 6e20 7469  Time: session ti
+0000f290: 6d65 7374 616d 7020 2874 696d 6520 6f6e  mestamp (time on
+0000f2a0: 6c79 290a 2020 2020 2020 2020 2d20 546f  ly).        - To
+0000f2b0: 7461 6c4c 6170 7320 2869 6e74 293a 2049  talLaps (int): I
+0000f2c0: 6e74 656e 6465 6420 6e75 6d62 6572 206f  ntended number o
+0000f2d0: 6620 746f 7461 6c20 6c61 7073 0a20 2020  f total laps.   
+0000f2e0: 2020 2020 202d 2043 7572 7265 6e74 4c61       - CurrentLa
+0000f2f0: 7020 2869 6e74 293a 2043 7572 7265 6e74  p (int): Current
+0000f300: 2072 6163 6520 6c61 700a 0a20 2020 2041   race lap..    A
+0000f310: 2076 616c 7565 2063 616e 2068 6176 6520   value can have 
+0000f320: 626f 7468 2027 546f 7461 6c4c 6170 7327  both 'TotalLaps'
+0000f330: 2061 6e64 2027 4375 7272 656e 744c 6170   and 'CurrentLap
+0000f340: 2720 6f72 206f 6e6c 7920 6f6e 6520 6f66  ' or only one of
+0000f350: 2074 6865 6d2e 0a0a 2020 2020 4120 6e65   them...    A ne
+0000f360: 7720 7661 6c75 6520 6973 2073 656e 7420  w value is sent 
+0000f370: 6576 6572 7920 7469 6d65 2061 206c 6170  every time a lap
+0000f380: 2069 7320 636f 6d70 6c65 7465 6420 6f72   is completed or
+0000f390: 0a20 2020 2074 6865 2069 6e74 656e 6465  .    the intende
+0000f3a0: 6420 6e75 6d62 6572 206f 6620 6c61 7073  d number of laps
+0000f3b0: 2063 6861 6e67 6573 2e0a 0a20 2020 2041   changes...    A
+0000f3c0: 7267 733a 0a20 2020 2020 2020 2070 6174  rgs:.        pat
+0000f3d0: 6820 2873 7472 293a 2061 7069 2070 6174  h (str): api pat
+0000f3e0: 6820 6261 7365 2073 7472 696e 6720 2875  h base string (u
+0000f3f0: 7375 616c 6c79 2060 6053 6573 7369 6f6e  sually ``Session
+0000f400: 2e61 7069 5f70 6174 6860 6029 0a20 2020  .api_path``).   
+0000f410: 2020 2020 2072 6573 706f 6e73 653a 2052       response: R
+0000f420: 6573 706f 6e73 6520 6173 2072 6574 7572  esponse as retur
+0000f430: 6e65 6420 6279 203a 6675 6e63 3a60 6665  ned by :func:`fe
+0000f440: 7463 685f 7061 6765 6020 6361 6e20 6265  tch_page` can be
+0000f450: 2070 6173 7365 6420 6966 0a20 2020 2020   passed if.     
+0000f460: 2020 2020 2020 2069 7420 7761 7320 646f         it was do
+0000f470: 776e 6c6f 6164 6564 2061 6c72 6561 6479  wnloaded already
+0000f480: 2e0a 2020 2020 2020 2020 6c69 7665 6461  ..        liveda
+0000f490: 7461 3a20 416e 2069 6e73 7461 6e63 6520  ta: An instance 
+0000f4a0: 6f66 0a20 2020 2020 2020 2020 2020 203a  of.            :
+0000f4b0: 636c 6173 733a 6066 6173 7466 312e 6c69  class:`fastf1.li
+0000f4c0: 7665 7469 6d69 6e67 2e64 6174 612e 4c69  vetiming.data.Li
+0000f4d0: 7665 5469 6d69 6e67 4461 7461 6020 746f  veTimingData` to
+0000f4e0: 2075 7365 2061 7320 6120 736f 7572 6365   use as a source
+0000f4f0: 0a20 2020 2020 2020 2020 2020 2069 6e73  .            ins
+0000f500: 7465 6164 206f 6620 7468 6520 6170 690a  tead of the api.
+0000f510: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
+0000f520: 2020 2020 2020 4120 6469 6374 696f 6e61        A dictiona
+0000f530: 7279 2063 6f6e 7461 696e 696e 6720 6f6e  ry containing on
+0000f540: 6520 6b65 7920 666f 7220 6561 6368 2064  e key for each d
+0000f550: 6174 6120 6368 616e 6e65 6c20 616e 6420  ata channel and 
+0000f560: 6120 6c69 7374 206f 660a 2020 2020 2020  a list of.      
+0000f570: 2020 7661 6c75 6573 2070 6572 206b 6579    values per key
+0000f580: 2e0a 0a20 2020 2052 6169 7365 733a 0a20  ...    Raises:. 
+0000f590: 2020 2020 2020 2053 6573 7369 6f6e 4e6f         SessionNo
+0000f5a0: 7441 7661 696c 6162 6c65 4572 726f 723a  tAvailableError:
+0000f5b0: 2069 6e20 6361 7365 2074 6865 2046 3120   in case the F1 
+0000f5c0: 6c69 7665 7469 6d69 6e67 2061 7069 2072  livetiming api r
+0000f5d0: 6574 7572 6e73 206e 6f20 6461 7461 0a20  eturns no data. 
+0000f5e0: 2020 2022 2222 0a20 2020 2069 6620 6c69     """.    if li
+0000f5f0: 7665 6461 7461 2069 7320 6e6f 7420 4e6f  vedata is not No
+0000f600: 6e65 2061 6e64 206c 6976 6564 6174 612e  ne and livedata.
+0000f610: 6861 7328 274c 6170 436f 756e 7427 293a  has('LapCount'):
+0000f620: 0a20 2020 2020 2020 2023 2064 6f65 7320  .        # does 
+0000f630: 6e6f 7420 6e65 6564 2061 6e79 2066 7572  not need any fur
+0000f640: 7468 6572 2070 726f 6365 7373 696e 670a  ther processing.
+0000f650: 2020 2020 2020 2020 5f6c 6f67 6765 722e          _logger.
+0000f660: 696e 666f 2822 4c6f 6164 696e 6720 6c61  info("Loading la
+0000f670: 7020 636f 756e 7420 6461 7461 2229 0a20  p count data"). 
+0000f680: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+0000f690: 3d20 6c69 7665 6461 7461 2e67 6574 2827  = livedata.get('
+0000f6a0: 4c61 7043 6f75 6e74 2729 0a20 2020 2065  LapCount').    e
+0000f6b0: 6c69 6620 7265 7370 6f6e 7365 2069 7320  lif response is 
+0000f6c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 5f6c  None:.        _l
+0000f6d0: 6f67 6765 722e 696e 666f 2822 4665 7463  ogger.info("Fetc
+0000f6e0: 6869 6e67 206c 6170 2063 6f75 6e74 2064  hing lap count d
+0000f6f0: 6174 612e 2e2e 2229 0a20 2020 2020 2020  ata...").       
+0000f700: 2072 6573 706f 6e73 6520 3d20 6665 7463   response = fetc
+0000f710: 685f 7061 6765 2870 6174 682c 2027 6c61  h_page(path, 'la
+0000f720: 705f 636f 756e 7427 290a 2020 2020 2020  p_count').      
+0000f730: 2020 6966 2072 6573 706f 6e73 6520 6973    if response is
+0000f740: 204e 6f6e 653a 2020 2320 6e6f 2072 6573   None:  # no res
+0000f750: 706f 6e73 6520 7265 6365 6976 6564 0a20  ponse received. 
+0000f760: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0000f770: 2053 6573 7369 6f6e 4e6f 7441 7661 696c   SessionNotAvail
+0000f780: 6162 6c65 4572 726f 7228 0a20 2020 2020  ableError(.     
+0000f790: 2020 2020 2020 2020 2020 2022 4e6f 2064             "No d
+0000f7a0: 6174 6120 666f 7220 7468 6973 2073 6573  ata for this ses
+0000f7b0: 7369 6f6e 2120 4966 2074 6869 7320 7365  sion! If this se
+0000f7c0: 7373 696f 6e20 6f6e 6c79 2066 696e 6973  ssion only finis
+0000f7d0: 6865 6420 220a 2020 2020 2020 2020 2020  hed ".          
+0000f7e0: 2020 2020 2020 2272 6563 656e 746c 792c        "recently,
+0000f7f0: 2070 6c65 6173 6520 7472 7920 6167 6169   please try agai
+0000f800: 6e20 696e 2061 2066 6577 206d 696e 7574  n in a few minut
+0000f810: 6573 2e22 0a20 2020 2020 2020 2020 2020  es.".           
+0000f820: 2029 0a0a 2020 2020 6461 7461 203d 207b   )..    data = {
+0000f830: 2754 696d 6527 3a20 5b5d 2c20 2754 6f74  'Time': [], 'Tot
+0000f840: 616c 4c61 7073 273a 205b 5d2c 2027 4375  alLaps': [], 'Cu
+0000f850: 7272 656e 744c 6170 273a 205b 5d7d 0a20  rrentLap': []}. 
+0000f860: 2020 2064 6174 615f 6b65 7973 203d 2028     data_keys = (
+0000f870: 2754 6f74 616c 4c61 7073 272c 2027 4375  'TotalLaps', 'Cu
+0000f880: 7272 656e 744c 6170 2729 0a20 2020 2063  rrentLap').    c
+0000f890: 6f6e 7665 7274 6572 7320 3d20 2869 6e74  onverters = (int
+0000f8a0: 2c20 696e 7429 0a0a 2020 2020 666f 7220  , int)..    for 
+0000f8b0: 656e 7472 7920 696e 2072 6573 706f 6e73  entry in respons
+0000f8c0: 653a 0a20 2020 2020 2020 2064 6174 615b  e:.        data[
+0000f8d0: 2754 696d 6527 5d2e 6170 7065 6e64 2874  'Time'].append(t
+0000f8e0: 6f5f 7469 6d65 6465 6c74 6128 656e 7472  o_timedelta(entr
+0000f8f0: 795b 305d 2929 0a0a 2020 2020 2020 2020  y[0]))..        
+0000f900: 666f 7220 6b65 792c 2063 6f6e 7620 696e  for key, conv in
+0000f910: 207a 6970 2864 6174 615f 6b65 7973 2c20   zip(data_keys, 
+0000f920: 636f 6e76 6572 7465 7273 293a 0a20 2020  converters):.   
+0000f930: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+0000f940: 2020 2020 2020 2020 2020 2020 2020 6461                da
+0000f950: 7461 5b6b 6579 5d2e 6170 7065 6e64 2863  ta[key].append(c
+0000f960: 6f6e 7628 656e 7472 795b 315d 5b6b 6579  onv(entry[1][key
+0000f970: 5d29 290a 2020 2020 2020 2020 2020 2020  ])).            
+0000f980: 6578 6365 7074 2028 4b65 7945 7272 6f72  except (KeyError
+0000f990: 2c20 5661 6c75 6545 7272 6f72 293a 0a20  , ValueError):. 
+0000f9a0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000f9b0: 2074 7970 6520 636f 6e76 6572 7369 6f6e   type conversion
+0000f9c0: 2066 6169 6c65 6420 6f72 206b 6579 2069   failed or key i
+0000f9d0: 7320 6d69 7373 696e 670a 2020 2020 2020  s missing.      
+0000f9e0: 2020 2020 2020 2020 2020 6461 7461 5b6b            data[k
+0000f9f0: 6579 5d2e 6170 7065 6e64 284e 6f6e 6529  ey].append(None)
+0000fa00: 0a0a 2020 2020 7265 7475 726e 2064 6174  ..    return dat
+0000fa10: 610a 0a0a 4043 6163 6865 2e61 7069 5f72  a...@Cache.api_r
+0000fa20: 6571 7565 7374 5f77 7261 7070 6572 0a64  equest_wrapper.d
+0000fa30: 6566 2064 7269 7665 725f 696e 666f 2870  ef driver_info(p
+0000fa40: 6174 682c 2072 6573 706f 6e73 653d 4e6f  ath, response=No
+0000fa50: 6e65 2c20 6c69 7665 6461 7461 3d4e 6f6e  ne, livedata=Non
+0000fa60: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
+0000fa70: 2e2e 2077 6172 6e69 6e67 3a3a 0a20 2020  .. warning::.   
+0000fa80: 2020 2020 203a 6d6f 643a 6066 6173 7466       :mod:`fastf
+0000fa90: 312e 6170 6960 2077 696c 6c20 6265 2063  1.api` will be c
+0000faa0: 6f6e 7369 6465 7265 6420 7072 6976 6174  onsidered privat
+0000fab0: 6520 696e 2066 7574 7572 6520 7265 6c65  e in future rele
+0000fac0: 6173 6573 2061 6e64 0a20 2020 2020 2020  ases and.       
+0000fad0: 2070 6f74 656e 7469 616c 6c79 2062 6520   potentially be 
+0000fae0: 7265 6d6f 7665 6420 6f72 2063 6861 6e67  removed or chang
+0000faf0: 6564 2e0a 0a20 2020 2046 6574 6368 2064  ed...    Fetch d
+0000fb00: 7269 7665 7220 696e 666f 726d 6174 696f  river informatio
+0000fb10: 6e2e 0a0a 2020 2020 4472 6976 6572 2069  n...    Driver i
+0000fb20: 6e66 6f72 6d61 7469 6f6e 2063 6f6e 7461  nformation conta
+0000fb30: 696e 7320 7468 6520 666f 6c6c 6f77 696e  ins the followin
+0000fb40: 6720 696e 666f 726d 6174 696f 6e20 6162  g information ab
+0000fb50: 6f75 7420 6561 6368 2064 7269 7665 723a  out each driver:
+0000fb60: 0a0a 2020 2020 2020 2020 605b 2752 6163  ..        `['Rac
+0000fb70: 696e 674e 756d 6265 7227 2c20 2742 726f  ingNumber', 'Bro
+0000fb80: 6164 6361 7374 4e61 6d65 272c 2027 4675  adcastName', 'Fu
+0000fb90: 6c6c 4e61 6d65 272c 2027 546c 6127 2c20  llName', 'Tla', 
+0000fba0: 274c 696e 6527 2c0a 2020 2020 2020 2020  'Line',.        
+0000fbb0: 2754 6561 6d4e 616d 6527 2c20 2754 6561  'TeamName', 'Tea
+0000fbc0: 6d43 6f6c 6f75 7227 2c20 2746 6972 7374  mColour', 'First
+0000fbd0: 4e61 6d65 272c 2027 4c61 7374 4e61 6d65  Name', 'LastName
+0000fbe0: 272c 2027 5265 6665 7265 6e63 6527 2c0a  ', 'Reference',.
+0000fbf0: 2020 2020 2020 2020 2748 6561 6473 686f          'Headsho
+0000fc00: 7455 726c 272c 2027 436f 756e 7472 7943  tUrl', 'CountryC
+0000fc10: 6f64 6527 5d60 0a0a 2020 2020 4172 6773  ode']`..    Args
+0000fc20: 3a0a 2020 2020 2020 2020 7061 7468 2028  :.        path (
+0000fc30: 7374 7229 3a20 6170 6920 7061 7468 2062  str): api path b
+0000fc40: 6173 6520 7374 7269 6e67 2028 7573 7561  ase string (usua
+0000fc50: 6c6c 7920 6060 5365 7373 696f 6e2e 6170  lly ``Session.ap
+0000fc60: 695f 7061 7468 6060 290a 2020 2020 2020  i_path``).      
+0000fc70: 2020 7265 7370 6f6e 7365 3a20 5265 7370    response: Resp
+0000fc80: 6f6e 7365 2061 7320 7265 7475 726e 6564  onse as returned
+0000fc90: 2062 7920 3a66 756e 633a 6066 6574 6368   by :func:`fetch
+0000fca0: 5f70 6167 6560 0a20 2020 2020 2020 2020  _page`.         
+0000fcb0: 2020 2063 616e 2062 6520 7061 7373 6564     can be passed
+0000fcc0: 2069 6620 6974 2077 6173 2064 6f77 6e6c   if it was downl
+0000fcd0: 6f61 6465 6420 616c 7265 6164 792e 0a20  oaded already.. 
+0000fce0: 2020 2020 2020 206c 6976 6564 6174 613a         livedata:
+0000fcf0: 2041 6e20 696e 7374 616e 6365 206f 6620   An instance of 
+0000fd00: 3a63 6c61 7373 3a60 6661 7374 6631 2e6c  :class:`fastf1.l
+0000fd10: 6976 6574 696d 696e 672e 6461 7461 2e4c  ivetiming.data.L
+0000fd20: 6976 6554 696d 696e 6744 6174 6160 0a20  iveTimingData`. 
+0000fd30: 2020 2020 2020 2020 2020 2074 6f20 7573             to us
+0000fd40: 6520 6173 2061 2073 6f75 7263 6520 696e  e as a source in
+0000fd50: 7374 6561 6420 6f66 2074 6865 2061 7069  stead of the api
+0000fd60: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
+0000fd70: 2020 2020 2020 2041 2064 6963 7469 6f6e         A diction
+0000fd80: 6172 7920 636f 6e74 6169 6e69 6e67 206f  ary containing o
+0000fd90: 6e65 2065 6e74 7279 2066 6f72 2065 6163  ne entry for eac
+0000fda0: 6820 6472 6976 6572 0a20 2020 2020 2020  h driver.       
+0000fdb0: 2077 6974 6820 7468 6520 6472 6976 6572   with the driver
+0000fdc0: 7320 7261 6369 6e67 206e 756d 6265 7220  s racing number 
+0000fdd0: 6173 206b 6579 0a0a 2020 2020 5261 6973  as key..    Rais
+0000fde0: 6573 3a0a 2020 2020 2020 2020 5365 7373  es:.        Sess
+0000fdf0: 696f 6e4e 6f74 4176 6169 6c61 626c 6545  ionNotAvailableE
+0000fe00: 7272 6f72 3a20 696e 2063 6173 6520 7468  rror: in case th
+0000fe10: 6520 4631 206c 6976 6574 696d 696e 6720  e F1 livetiming 
+0000fe20: 6170 6920 7265 7475 726e 7320 6e6f 2064  api returns no d
+0000fe30: 6174 610a 2020 2020 2222 220a 2020 2020  ata.    """.    
+0000fe40: 6966 206c 6976 6564 6174 6120 6973 206e  if livedata is n
+0000fe50: 6f74 204e 6f6e 6520 616e 6420 6c69 7665  ot None and live
+0000fe60: 6461 7461 2e68 6173 2827 4472 6976 6572  data.has('Driver
+0000fe70: 4c69 7374 2729 3a0a 2020 2020 2020 2020  List'):.        
+0000fe80: 2320 646f 6573 206e 6f74 206e 6565 6420  # does not need 
+0000fe90: 616e 7920 6675 7274 6865 7220 7072 6f63  any further proc
+0000fea0: 6573 7369 6e67 0a20 2020 2020 2020 205f  essing.        _
+0000feb0: 6c6f 6767 6572 2e69 6e66 6f28 224c 6f61  logger.info("Loa
+0000fec0: 6469 6e67 2064 7269 7665 7220 6c69 7374  ding driver list
+0000fed0: 2229 0a20 2020 2020 2020 2072 6573 706f  ").        respo
+0000fee0: 6e73 6520 3d20 6c69 7665 6461 7461 2e67  nse = livedata.g
+0000fef0: 6574 2827 4472 6976 6572 4c69 7374 2729  et('DriverList')
+0000ff00: 0a20 2020 2065 6c69 6620 7265 7370 6f6e  .    elif respon
+0000ff10: 7365 2069 7320 4e6f 6e65 3a0a 2020 2020  se is None:.    
+0000ff20: 2020 2020 5f6c 6f67 6765 722e 696e 666f      _logger.info
+0000ff30: 2822 4665 7463 6869 6e67 2064 7269 7665  ("Fetching drive
+0000ff40: 7220 6c69 7374 2e2e 2e22 290a 2020 2020  r list...").    
+0000ff50: 2020 2020 7265 7370 6f6e 7365 203d 2066      response = f
+0000ff60: 6574 6368 5f70 6167 6528 7061 7468 2c20  etch_page(path, 
+0000ff70: 2764 7269 7665 725f 6c69 7374 2729 0a20  'driver_list'). 
+0000ff80: 2020 2020 2020 2069 6620 7265 7370 6f6e         if respon
+0000ff90: 7365 2069 7320 4e6f 6e65 3a20 2023 206e  se is None:  # n
+0000ffa0: 6f20 7265 7370 6f6e 7365 2072 6563 6569  o response recei
+0000ffb0: 7665 640a 2020 2020 2020 2020 2020 2020  ved.            
+0000ffc0: 7261 6973 6520 5365 7373 696f 6e4e 6f74  raise SessionNot
+0000ffd0: 4176 6169 6c61 626c 6545 7272 6f72 280a  AvailableError(.
+0000ffe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fff0: 224e 6f20 6461 7461 2066 6f72 2074 6869  "No data for thi
+00010000: 7320 7365 7373 696f 6e21 2049 6620 7468  s session! If th
+00010010: 6973 2073 6573 7369 6f6e 206f 6e6c 7920  is session only 
+00010020: 6669 6e69 7368 6564 2022 0a20 2020 2020  finished ".     
+00010030: 2020 2020 2020 2020 2020 2022 7265 6365             "rece
+00010040: 6e74 6c79 2c20 706c 6561 7365 2074 7279  ntly, please try
+00010050: 2061 6761 696e 2069 6e20 6120 6665 7720   again in a few 
+00010060: 6d69 6e75 7465 732e 220a 2020 2020 2020  minutes.".      
+00010070: 2020 2020 2020 290a 0a20 2020 2064 7269        )..    dri
+00010080: 7665 7273 203d 2063 6f6c 6c65 6374 696f  vers = collectio
+00010090: 6e73 2e64 6566 6175 6c74 6469 6374 2864  ns.defaultdict(d
+000100a0: 6963 7429 0a0a 2020 2020 6465 6661 756c  ict)..    defaul
+000100b0: 745f 6b65 7973 203d 205b 0a20 2020 2020  t_keys = [.     
+000100c0: 2020 2027 5261 6369 6e67 4e75 6d62 6572     'RacingNumber
+000100d0: 272c 2027 4272 6f61 6463 6173 744e 616d  ', 'BroadcastNam
+000100e0: 6527 2c20 2746 756c 6c4e 616d 6527 2c20  e', 'FullName', 
+000100f0: 2754 6c61 272c 2027 4c69 6e65 272c 0a20  'Tla', 'Line',. 
+00010100: 2020 2020 2020 2027 5465 616d 4e61 6d65         'TeamName
+00010110: 272c 2027 5465 616d 436f 6c6f 7572 272c  ', 'TeamColour',
+00010120: 2027 4669 7273 744e 616d 6527 2c20 274c   'FirstName', 'L
+00010130: 6173 744e 616d 6527 2c20 2752 6566 6572  astName', 'Refer
+00010140: 656e 6365 272c 0a20 2020 2020 2020 2027  ence',.        '
+00010150: 4865 6164 7368 6f74 5572 6c27 2c20 2743  HeadshotUrl', 'C
+00010160: 6f75 6e74 7279 436f 6465 270a 2020 2020  ountryCode'.    
+00010170: 5d0a 0a20 2020 2066 6f72 206c 696e 6520  ]..    for line 
+00010180: 696e 2072 6573 706f 6e73 653a 0a20 2020  in response:.   
+00010190: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+000101a0: 2020 2020 2020 7473 2c20 636f 6e74 656e        ts, conten
+000101b0: 7420 3d20 6c69 6e65 0a20 2020 2020 2020  t = line.       
+000101c0: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
+000101d0: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
+000101e0: 2320 756e 6578 7065 6374 6564 2064 6174  # unexpected dat
+000101f0: 6120 666f 726d 6174 2c20 696e 636f 7272  a format, incorr
+00010200: 6563 7420 6e75 6d62 6572 206f 6620 7661  ect number of va
+00010210: 6c75 6573 2074 6f20 756e 7061 636b 0a20  lues to unpack. 
+00010220: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+00010230: 6e75 650a 2020 2020 2020 2020 6966 206e  nue.        if n
+00010240: 6f74 2069 7369 6e73 7461 6e63 6528 636f  ot isinstance(co
+00010250: 6e74 656e 742c 2064 6963 7429 3a0a 2020  ntent, dict):.  
+00010260: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+00010270: 7565 2020 2320 756e 6578 7065 6374 6564  ue  # unexpected
+00010280: 2064 6174 6120 666f 726d 6174 0a20 2020   data format.   
+00010290: 2020 2020 2066 6f72 2064 7276 5f6e 756d       for drv_num
+000102a0: 2c20 7061 7463 6820 696e 2063 6f6e 7465  , patch in conte
+000102b0: 6e74 2e69 7465 6d73 2829 3a0a 2020 2020  nt.items():.    
+000102c0: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+000102d0: 7369 6e73 7461 6e63 6528 7061 7463 682c  sinstance(patch,
+000102e0: 2064 6963 7429 3a0a 2020 2020 2020 2020   dict):.        
+000102f0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+00010300: 2020 2320 756e 6578 7065 6374 6564 2064    # unexpected d
+00010310: 6174 6120 666f 726d 6174 0a20 2020 2020  ata format.     
+00010320: 2020 2020 2020 2066 6f72 206b 6579 2c20         for key, 
+00010330: 7661 6c20 696e 2070 6174 6368 2e69 7465  val in patch.ite
+00010340: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
+00010350: 2020 2020 2020 6966 206b 6579 206e 6f74        if key not
+00010360: 2069 6e20 6465 6661 756c 745f 6b65 7973   in default_keys
+00010370: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00010380: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+00010390: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000103a0: 7269 7665 7273 5b64 7276 5f6e 756d 5d5b  rivers[drv_num][
+000103b0: 6b65 795d 203d 2076 616c 0a0a 2020 2020  key] = val..    
+000103c0: 7265 7475 726e 2064 7269 7665 7273 0a0a  return drivers..
+000103d0: 0a40 4361 6368 652e 6170 695f 7265 7175  .@Cache.api_requ
+000103e0: 6573 745f 7772 6170 7065 720a 6465 6620  est_wrapper.def 
+000103f0: 7765 6174 6865 725f 6461 7461 2870 6174  weather_data(pat
+00010400: 682c 2072 6573 706f 6e73 653d 4e6f 6e65  h, response=None
+00010410: 2c20 6c69 7665 6461 7461 3d4e 6f6e 6529  , livedata=None)
+00010420: 3a0a 2020 2020 2222 220a 2020 2020 2e2e  :.    """.    ..
+00010430: 2077 6172 6e69 6e67 3a3a 0a20 2020 2020   warning::.     
+00010440: 2020 203a 6d6f 643a 6066 6173 7466 312e     :mod:`fastf1.
+00010450: 6170 6960 2077 696c 6c20 6265 2063 6f6e  api` will be con
+00010460: 7369 6465 7265 6420 7072 6976 6174 6520  sidered private 
+00010470: 696e 2066 7574 7572 6520 7265 6c65 6173  in future releas
+00010480: 6573 2061 6e64 0a20 2020 2020 2020 2070  es and.        p
+00010490: 6f74 656e 7469 616c 6c79 2062 6520 7265  otentially be re
+000104a0: 6d6f 7665 6420 6f72 2063 6861 6e67 6564  moved or changed
+000104b0: 2e0a 0a20 2020 2046 6574 6368 2061 6e64  ...    Fetch and
+000104c0: 2070 6172 7365 2077 6561 7468 6572 2064   parse weather d
+000104d0: 6174 612e 0a0a 2020 2020 5765 6174 6865  ata...    Weathe
+000104e0: 7220 6461 7461 2070 726f 7669 6465 7320  r data provides 
+000104f0: 7468 6520 666f 6c6c 6f77 696e 6720 6461  the following da
+00010500: 7461 2063 6861 6e6e 656c 7320 7065 7220  ta channels per 
+00010510: 7361 6d70 6c65 3a0a 0a20 2020 2020 2020  sample:..       
+00010520: 202d 2054 696d 6520 2864 6174 6574 696d   - Time (datetim
+00010530: 652e 7469 6d65 6465 6c74 6129 3a20 7365  e.timedelta): se
+00010540: 7373 696f 6e20 7469 6d65 7374 616d 7020  ssion timestamp 
+00010550: 2874 696d 6520 6f6e 6c79 290a 2020 2020  (time only).    
+00010560: 2020 2020 2d20 4169 7254 656d 7020 2866      - AirTemp (f
+00010570: 6c6f 6174 293a 2041 6972 2074 656d 7065  loat): Air tempe
+00010580: 7261 7475 7265 205b c2b0 435d 0a20 2020  rature [..C].   
+00010590: 2020 2020 202d 2048 756d 6964 6974 7920       - Humidity 
+000105a0: 2866 6c6f 6174 293a 2052 656c 6174 6976  (float): Relativ
+000105b0: 6520 6875 6d69 6469 7479 205b 255d 0a20  e humidity [%]. 
+000105c0: 2020 2020 2020 202d 2050 7265 7373 7572         - Pressur
+000105d0: 6520 2866 6c6f 6174 293a 2041 6972 2070  e (float): Air p
+000105e0: 7265 7373 7572 6520 5b6d 6261 725d 0a20  ressure [mbar]. 
+000105f0: 2020 2020 2020 202d 2052 6169 6e66 616c         - Rainfal
+00010600: 6c20 2862 6f6f 6c29 3a20 5368 6f77 7320  l (bool): Shows 
+00010610: 6966 2074 6865 7265 2069 7320 7261 696e  if there is rain
+00010620: 6661 6c6c 0a20 2020 2020 2020 202d 2054  fall.        - T
+00010630: 7261 636b 5465 6d70 2028 666c 6f61 7429  rackTemp (float)
+00010640: 3a20 5472 6163 6b20 7465 6d70 6572 6174  : Track temperat
+00010650: 7572 6520 5bc2 b043 5d0a 2020 2020 2020  ure [..C].      
+00010660: 2020 2d20 5769 6e64 4469 7265 6374 696f    - WindDirectio
+00010670: 6e20 2869 6e74 293a 2057 696e 6420 6469  n (int): Wind di
+00010680: 7265 6374 696f 6e20 5bc2 b05d 2028 30c2  rection [..] (0.
+00010690: b02d 3335 39c2 b029 0a20 2020 2020 2020  .-359..).       
+000106a0: 202d 2057 696e 6453 7065 6564 2028 666c   - WindSpeed (fl
+000106b0: 6f61 7429 3a20 5769 6e64 2073 7065 6564  oat): Wind speed
+000106c0: 205b 6d2f 735d 0a0a 2020 2020 5765 6174   [m/s]..    Weat
+000106d0: 6865 7220 6461 7461 2069 7320 7570 6461  her data is upda
+000106e0: 7465 6420 6f6e 6365 2070 6572 206d 696e  ted once per min
+000106f0: 7574 652e 0a0a 2020 2020 4172 6773 3a0a  ute...    Args:.
+00010700: 2020 2020 2020 2020 7061 7468 2028 7374          path (st
+00010710: 7229 3a20 6170 6920 7061 7468 2062 6173  r): api path bas
+00010720: 6520 7374 7269 6e67 2028 7573 7561 6c6c  e string (usuall
+00010730: 7920 6060 5365 7373 696f 6e2e 6170 695f  y ``Session.api_
+00010740: 7061 7468 6060 290a 2020 2020 2020 2020  path``).        
+00010750: 7265 7370 6f6e 7365 3a20 5265 7370 6f6e  response: Respon
+00010760: 7365 2061 7320 7265 7475 726e 6564 2062  se as returned b
+00010770: 7920 3a66 756e 633a 6066 6574 6368 5f70  y :func:`fetch_p
+00010780: 6167 6560 2063 616e 0a20 2020 2020 2020  age` can.       
+00010790: 2020 2020 2062 6520 7061 7373 6564 2069       be passed i
+000107a0: 6620 6974 2077 6173 2064 6f77 6e6c 6f61  f it was downloa
+000107b0: 6465 6420 616c 7265 6164 792e 0a20 2020  ded already..   
+000107c0: 2020 2020 206c 6976 6564 6174 613a 2041       livedata: A
+000107d0: 6e20 696e 7374 616e 6365 206f 660a 2020  n instance of.  
+000107e0: 2020 2020 2020 2020 2020 3a63 6c61 7373            :class
+000107f0: 3a60 6661 7374 6631 2e6c 6976 6574 696d  :`fastf1.livetim
+00010800: 696e 672e 6461 7461 2e4c 6976 6554 696d  ing.data.LiveTim
+00010810: 696e 6744 6174 6160 0a20 2020 2020 2020  ingData`.       
+00010820: 2020 2020 2074 6f20 7573 6520 6173 2061       to use as a
+00010830: 2073 6f75 7263 6520 696e 7374 6561 6420   source instead 
+00010840: 6f66 2074 6865 2061 7069 0a0a 2020 2020  of the api..    
+00010850: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00010860: 2041 2064 6963 7469 6f6e 6172 7920 636f   A dictionary co
+00010870: 6e74 6169 6e69 6e67 206f 6e65 206b 6579  ntaining one key
+00010880: 2066 6f72 2065 6163 6820 6461 7461 2063   for each data c
+00010890: 6861 6e6e 656c 2061 6e64 2061 206c 6973  hannel and a lis
+000108a0: 740a 2020 2020 2020 2020 6f66 2076 616c  t.        of val
+000108b0: 7565 7320 7065 7220 6b65 792e 0a0a 2020  ues per key...  
+000108c0: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
+000108d0: 2020 5365 7373 696f 6e4e 6f74 4176 6169    SessionNotAvai
+000108e0: 6c61 626c 6545 7272 6f72 3a20 696e 2063  lableError: in c
+000108f0: 6173 6520 7468 6520 4631 206c 6976 6520  ase the F1 live 
+00010900: 7469 6d69 6e67 2061 7069 0a20 2020 2020  timing api.     
+00010910: 2020 2020 2020 2072 6574 7572 6e73 206e         returns n
+00010920: 6f20 6461 7461 0a20 2020 2022 2222 0a20  o data.    """. 
+00010930: 2020 2069 6620 6c69 7665 6461 7461 2069     if livedata i
+00010940: 7320 6e6f 7420 4e6f 6e65 2061 6e64 206c  s not None and l
+00010950: 6976 6564 6174 612e 6861 7328 2757 6561  ivedata.has('Wea
+00010960: 7468 6572 4461 7461 2729 3a0a 2020 2020  therData'):.    
+00010970: 2020 2020 2320 646f 6573 206e 6f74 206e      # does not n
+00010980: 6565 6420 616e 7920 6675 7274 6865 7220  eed any further 
+00010990: 7072 6f63 6573 7369 6e67 0a20 2020 2020  processing.     
+000109a0: 2020 205f 6c6f 6767 6572 2e69 6e66 6f28     _logger.info(
+000109b0: 224c 6f61 6469 6e67 2077 6561 7468 6572  "Loading weather
+000109c0: 2064 6174 6122 290a 2020 2020 2020 2020   data").        
+000109d0: 7265 7370 6f6e 7365 203d 206c 6976 6564  response = lived
+000109e0: 6174 612e 6765 7428 2757 6561 7468 6572  ata.get('Weather
+000109f0: 4461 7461 2729 0a20 2020 2065 6c69 6620  Data').    elif 
+00010a00: 7265 7370 6f6e 7365 2069 7320 4e6f 6e65  response is None
+00010a10: 3a0a 2020 2020 2020 2020 5f6c 6f67 6765  :.        _logge
+00010a20: 722e 696e 666f 2822 4665 7463 6869 6e67  r.info("Fetching
+00010a30: 2077 6561 7468 6572 2064 6174 612e 2e2e   weather data...
+00010a40: 2229 0a20 2020 2020 2020 2072 6573 706f  ").        respo
+00010a50: 6e73 6520 3d20 6665 7463 685f 7061 6765  nse = fetch_page
+00010a60: 2870 6174 682c 2027 7765 6174 6865 725f  (path, 'weather_
+00010a70: 6461 7461 2729 0a20 2020 2020 2020 2069  data').        i
+00010a80: 6620 7265 7370 6f6e 7365 2069 7320 4e6f  f response is No
+00010a90: 6e65 3a20 2023 206e 6f20 7265 7370 6f6e  ne:  # no respon
+00010aa0: 7365 2072 6563 6569 7665 640a 2020 2020  se received.    
+00010ab0: 2020 2020 2020 2020 7261 6973 6520 5365          raise Se
+00010ac0: 7373 696f 6e4e 6f74 4176 6169 6c61 626c  ssionNotAvailabl
+00010ad0: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+00010ae0: 2020 2020 2020 2020 224e 6f20 6461 7461          "No data
+00010af0: 2066 6f72 2074 6869 7320 7365 7373 696f   for this sessio
+00010b00: 6e21 2049 6620 7468 6973 2073 6573 7369  n! If this sessi
+00010b10: 6f6e 206f 6e6c 7920 6669 6e69 7368 6564  on only finished
+00010b20: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+00010b30: 2020 2022 7265 6365 6e74 6c79 2c20 706c     "recently, pl
+00010b40: 6561 7365 2074 7279 2061 6761 696e 2069  ease try again i
+00010b50: 6e20 6120 6665 7720 6d69 6e75 7465 732e  n a few minutes.
+00010b60: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
+00010b70: 0a20 2020 2064 6174 6120 3d20 7b0a 2020  .    data = {.  
+00010b80: 2020 2020 2020 2754 696d 6527 3a20 5b5d        'Time': []
+00010b90: 2c20 2741 6972 5465 6d70 273a 205b 5d2c  , 'AirTemp': [],
+00010ba0: 2027 4875 6d69 6469 7479 273a 205b 5d2c   'Humidity': [],
+00010bb0: 2027 5072 6573 7375 7265 273a 205b 5d2c   'Pressure': [],
+00010bc0: 0a20 2020 2020 2020 2027 5261 696e 6661  .        'Rainfa
+00010bd0: 6c6c 273a 205b 5d2c 2027 5472 6163 6b54  ll': [], 'TrackT
+00010be0: 656d 7027 3a20 5b5d 2c20 2757 696e 6444  emp': [], 'WindD
+00010bf0: 6972 6563 7469 6f6e 273a 205b 5d2c 2027  irection': [], '
+00010c00: 5769 6e64 5370 6565 6427 3a20 5b5d 0a20  WindSpeed': []. 
+00010c10: 2020 207d 0a0a 2020 2020 6461 7461 5f6b     }..    data_k
+00010c20: 6579 7320 3d20 2827 4169 7254 656d 7027  eys = ('AirTemp'
+00010c30: 2c20 2748 756d 6964 6974 7927 2c20 2750  , 'Humidity', 'P
+00010c40: 7265 7373 7572 6527 2c20 2752 6169 6e66  ressure', 'Rainf
+00010c50: 616c 6c27 2c0a 2020 2020 2020 2020 2020  all',.          
+00010c60: 2020 2020 2020 2027 5472 6163 6b54 656d         'TrackTem
+00010c70: 7027 2c20 2757 696e 6444 6972 6563 7469  p', 'WindDirecti
+00010c80: 6f6e 272c 2027 5769 6e64 5370 6565 6427  on', 'WindSpeed'
+00010c90: 290a 2020 2020 636f 6e76 6572 7465 7273  ).    converters
+00010ca0: 203d 2028 666c 6f61 742c 2066 6c6f 6174   = (float, float
+00010cb0: 2c20 666c 6f61 742c 0a20 2020 2020 2020  , float,.       
+00010cc0: 2020 2020 2020 2020 2020 206c 616d 6264             lambd
+00010cd0: 6120 763a 2054 7275 6520 6966 2076 203d  a v: True if v =
+00010ce0: 3d20 2731 2720 656c 7365 2046 616c 7365  = '1' else False
+00010cf0: 2c20 2023 2072 6169 6e3a 2073 7472 202d  ,  # rain: str -
+00010d00: 3e20 626f 6f6c 0a20 2020 2020 2020 2020  > bool.         
+00010d10: 2020 2020 2020 2020 2066 6c6f 6174 2c20           float, 
+00010d20: 696e 742c 2066 6c6f 6174 290a 0a20 2020  int, float)..   
+00010d30: 2066 6f72 2065 6e74 7279 2069 6e20 7265   for entry in re
+00010d40: 7370 6f6e 7365 3a0a 2020 2020 2020 2020  sponse:.        
+00010d50: 6966 206c 656e 2865 6e74 7279 2920 3c20  if len(entry) < 
+00010d60: 323a 0a20 2020 2020 2020 2020 2020 2063  2:.            c
+00010d70: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
+00010d80: 726f 7720 3d20 656e 7472 795b 315d 0a20  row = entry[1]. 
+00010d90: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
+00010da0: 696e 7374 616e 6365 2872 6f77 2c20 6469  instance(row, di
+00010db0: 6374 293a 0a20 2020 2020 2020 2020 2020  ct):.           
+00010dc0: 2063 6f6e 7469 6e75 650a 0a20 2020 2020   continue..     
+00010dd0: 2020 2064 6174 615b 2754 696d 6527 5d2e     data['Time'].
+00010de0: 6170 7065 6e64 2874 6f5f 7469 6d65 6465  append(to_timede
+00010df0: 6c74 6128 656e 7472 795b 305d 2929 0a20  lta(entry[0])). 
+00010e00: 2020 2020 2020 2066 6f72 206b 6579 2c20         for key, 
+00010e10: 636f 6e76 2069 6e20 7a69 7028 6461 7461  conv in zip(data
+00010e20: 5f6b 6579 732c 2063 6f6e 7665 7274 6572  _keys, converter
+00010e30: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00010e40: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00010e50: 2020 2020 2064 6174 615b 6b65 795d 2e61       data[key].a
+00010e60: 7070 656e 6428 636f 6e76 2872 6f77 5b6b  ppend(conv(row[k
+00010e70: 6579 5d29 290a 2020 2020 2020 2020 2020  ey])).          
+00010e80: 2020 6578 6365 7074 2028 4b65 7945 7272    except (KeyErr
+00010e90: 6f72 2c20 5661 6c75 6545 7272 6f72 293a  or, ValueError):
+00010ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010eb0: 2023 2074 7970 6520 636f 6e76 6572 7369   # type conversi
+00010ec0: 6f6e 2066 6169 6c65 6420 6f72 206b 6579  on failed or key
+00010ed0: 2069 7320 6d69 7373 696e 670a 2020 2020   is missing.    
+00010ee0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00010ef0: 5b6b 6579 5d2e 6170 7065 6e64 2863 6f6e  [key].append(con
+00010f00: 7628 3029 290a 0a20 2020 2072 6574 7572  v(0))..    retur
+00010f10: 6e20 6461 7461 0a0a 0a40 4361 6368 652e  n data...@Cache.
+00010f20: 6170 695f 7265 7175 6573 745f 7772 6170  api_request_wrap
+00010f30: 7065 720a 6465 6620 7365 6173 6f6e 5f73  per.def season_s
+00010f40: 6368 6564 756c 6528 7061 7468 2c20 7265  chedule(path, re
+00010f50: 7370 6f6e 7365 3d4e 6f6e 6529 3a0a 2020  sponse=None):.  
+00010f60: 2020 6966 2072 6573 706f 6e73 6520 6973    if response is
+00010f70: 204e 6f6e 653a 0a20 2020 2020 2020 205f   None:.        _
+00010f80: 6c6f 6767 6572 2e69 6e66 6f28 2246 6574  logger.info("Fet
+00010f90: 6368 696e 6720 7365 6173 6f6e 2073 6368  ching season sch
+00010fa0: 6564 756c 652e 2e2e 2229 0a20 2020 2020  edule...").     
+00010fb0: 2020 2072 6573 706f 6e73 6520 3d20 6665     response = fe
+00010fc0: 7463 685f 7061 6765 2870 6174 682c 2027  tch_page(path, '
+00010fd0: 696e 6465 7827 290a 2020 2020 2020 2020  index').        
+00010fe0: 6966 2072 6573 706f 6e73 6520 6973 204e  if response is N
+00010ff0: 6f6e 653a 2020 2320 6e6f 2072 6573 706f  one:  # no respo
+00011000: 6e73 6520 7265 6365 6976 6564 0a20 2020  nse received.   
+00011010: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
+00011020: 6573 7369 6f6e 4e6f 7441 7661 696c 6162  essionNotAvailab
+00011030: 6c65 4572 726f 7228 0a20 2020 2020 2020  leError(.       
+00011040: 2020 2020 2020 2020 2022 4e6f 2064 6174           "No dat
+00011050: 6120 666f 7220 7468 6973 2073 6573 7369  a for this sessi
+00011060: 6f6e 2120 4966 2074 6869 7320 7365 7373  on! If this sess
+00011070: 696f 6e20 6f6e 6c79 2066 696e 6973 6865  ion only finishe
+00011080: 6420 220a 2020 2020 2020 2020 2020 2020  d ".            
+00011090: 2020 2020 2272 6563 656e 746c 792c 2070      "recently, p
+000110a0: 6c65 6173 6520 7472 7920 6167 6169 6e20  lease try again 
+000110b0: 696e 2061 2066 6577 206d 696e 7574 6573  in a few minutes
+000110c0: 2e22 0a20 2020 2020 2020 2020 2020 2029  .".            )
+000110d0: 0a0a 2020 2020 7265 7475 726e 2072 6573  ..    return res
+000110e0: 706f 6e73 655b 274d 6565 7469 6e67 7327  ponse['Meetings'
+000110f0: 5d0a 0a0a 4043 6163 6865 2e61 7069 5f72  ]...@Cache.api_r
+00011100: 6571 7565 7374 5f77 7261 7070 6572 0a64  equest_wrapper.d
+00011110: 6566 2073 6573 7369 6f6e 5f69 6e66 6f28  ef session_info(
+00011120: 7061 7468 2c20 7265 7370 6f6e 7365 3d4e  path, response=N
+00011130: 6f6e 652c 206c 6976 6564 6174 613d 4e6f  one, livedata=No
+00011140: 6e65 293a 0a20 2020 2022 2222 0a20 2020  ne):.    """.   
+00011150: 202e 2e20 7761 726e 696e 673a 3a0a 2020   .. warning::.  
+00011160: 2020 2020 2020 3a6d 6f64 3a60 6661 7374        :mod:`fast
+00011170: 6631 2e61 7069 6020 7769 6c6c 2062 6520  f1.api` will be 
+00011180: 636f 6e73 6964 6572 6564 2070 7269 7661  considered priva
+00011190: 7465 2069 6e20 6675 7475 7265 2072 656c  te in future rel
+000111a0: 6561 7365 7320 616e 640a 2020 2020 2020  eases and.      
+000111b0: 2020 706f 7465 6e74 6961 6c6c 7920 6265    potentially be
+000111c0: 2072 656d 6f76 6564 206f 7220 6368 616e   removed or chan
+000111d0: 6765 642e 0a0a 2020 2020 4665 7463 6820  ged...    Fetch 
+000111e0: 616e 6420 7061 7273 6520 7365 7373 696f  and parse sessio
+000111f0: 6e20 696e 666f 2064 6174 612e 0a0a 2020  n info data...  
+00011200: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00011210: 2020 2041 2064 6963 7469 6f6e 6172 7920     A dictionary 
+00011220: 636f 6e74 6169 6e69 6e67 2074 6865 206e  containing the n
+00011230: 6573 7465 6420 7365 7373 696f 6e20 696e  ested session in
+00011240: 666f 2064 6174 612e 2054 696d 6573 7461  fo data. Timesta
+00011250: 6d70 7320 616e 640a 2020 2020 2020 2020  mps and.        
+00011260: 7469 6d65 6465 6c74 6173 2061 7265 2063  timedeltas are c
+00011270: 6f6e 7665 7274 6564 2074 6f20 6060 6461  onverted to ``da
+00011280: 7465 7469 6d65 2e64 6174 6574 696d 6560  tetime.datetime`
+00011290: 6020 616e 640a 2020 2020 2020 2020 6060  ` and.        ``
+000112a0: 6461 7465 7469 6d65 2e74 696d 6564 656c  datetime.timedel
+000112b0: 7461 6060 2072 6573 7065 6374 6976 656c  ta`` respectivel
+000112c0: 792e 0a0a 2020 2020 5261 6973 6573 3a0a  y...    Raises:.
+000112d0: 2020 2020 2020 2020 5365 7373 696f 6e4e          SessionN
+000112e0: 6f74 4176 6169 6c61 626c 6545 7272 6f72  otAvailableError
+000112f0: 3a20 696e 2063 6173 6520 7468 6520 4631  : in case the F1
+00011300: 206c 6976 6520 7469 6d69 6e67 2061 7069   live timing api
+00011310: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00011320: 7572 6e73 206e 6f20 6461 7461 0a20 2020  urns no data.   
+00011330: 2022 2222 0a20 2020 2069 6620 6c69 7665   """.    if live
+00011340: 6461 7461 2069 7320 6e6f 7420 4e6f 6e65  data is not None
+00011350: 2061 6e64 206c 6976 6564 6174 612e 6861   and livedata.ha
+00011360: 7328 2753 6573 7369 6f6e 496e 666f 2729  s('SessionInfo')
+00011370: 3a0a 2020 2020 2020 2020 2320 646f 6573  :.        # does
+00011380: 206e 6f74 206e 6565 6420 616e 7920 6675   not need any fu
+00011390: 7274 6865 7220 7072 6f63 6573 7369 6e67  rther processing
+000113a0: 0a20 2020 2020 2020 205f 6c6f 6767 6572  .        _logger
+000113b0: 2e69 6e66 6f28 224c 6f61 6469 6e67 2073  .info("Loading s
+000113c0: 6573 7369 6f6e 2069 6e66 6f20 6461 7461  ession info data
+000113d0: 2229 0a20 2020 2020 2020 2072 6573 706f  ").        respo
+000113e0: 6e73 6520 3d20 6c69 7665 6461 7461 2e67  nse = livedata.g
+000113f0: 6574 2827 5365 7373 696f 6e49 6e66 6f27  et('SessionInfo'
+00011400: 290a 2020 2020 656c 6966 2072 6573 706f  ).    elif respo
+00011410: 6e73 6520 6973 204e 6f6e 653a 0a20 2020  nse is None:.   
+00011420: 2020 2020 205f 6c6f 6767 6572 2e69 6e66       _logger.inf
+00011430: 6f28 2246 6574 6368 696e 6720 7365 7373  o("Fetching sess
+00011440: 696f 6e20 696e 666f 2064 6174 612e 2e2e  ion info data...
+00011450: 2229 0a20 2020 2020 2020 2072 6573 706f  ").        respo
+00011460: 6e73 6520 3d20 6665 7463 685f 7061 6765  nse = fetch_page
+00011470: 2870 6174 682c 2027 7365 7373 696f 6e5f  (path, 'session_
+00011480: 696e 666f 2729 0a20 2020 2020 2020 2069  info').        i
+00011490: 6620 7265 7370 6f6e 7365 2069 7320 4e6f  f response is No
+000114a0: 6e65 3a20 2023 206e 6f20 7265 7370 6f6e  ne:  # no respon
+000114b0: 7365 2072 6563 6569 7665 640a 2020 2020  se received.    
+000114c0: 2020 2020 2020 2020 7261 6973 6520 5365          raise Se
+000114d0: 7373 696f 6e4e 6f74 4176 6169 6c61 626c  ssionNotAvailabl
+000114e0: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+000114f0: 2020 2020 2020 2020 224e 6f20 6461 7461          "No data
+00011500: 2066 6f72 2074 6869 7320 7365 7373 696f   for this sessio
+00011510: 6e21 2049 6620 7468 6973 2073 6573 7369  n! If this sessi
+00011520: 6f6e 206f 6e6c 7920 6669 6e69 7368 6564  on only finished
+00011530: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+00011540: 2020 2022 7265 6365 6e74 6c79 2c20 706c     "recently, pl
+00011550: 6561 7365 2074 7279 2061 6761 696e 2069  ease try again i
+00011560: 6e20 6120 6665 7720 6d69 6e75 7465 732e  n a few minutes.
+00011570: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
+00011580: 0a20 2020 2074 732c 2064 6174 6120 3d20  .    ts, data = 
+00011590: 7265 7370 6f6e 7365 5b30 5d0a 0a20 2020  response[0]..   
+000115a0: 2064 6174 615b 2753 7461 7274 4461 7465   data['StartDate
+000115b0: 275d 203d 2074 6f5f 6461 7465 7469 6d65  '] = to_datetime
+000115c0: 2864 6174 615b 2753 7461 7274 4461 7465  (data['StartDate
+000115d0: 275d 290a 2020 2020 6461 7461 5b27 456e  ']).    data['En
+000115e0: 6444 6174 6527 5d20 3d20 746f 5f64 6174  dDate'] = to_dat
+000115f0: 6574 696d 6528 6461 7461 5b27 456e 6444  etime(data['EndD
+00011600: 6174 6527 5d29 0a20 2020 2064 6174 615b  ate']).    data[
+00011610: 2747 6d74 4f66 6673 6574 275d 203d 2074  'GmtOffset'] = t
+00011620: 6f5f 7469 6d65 6465 6c74 6128 6461 7461  o_timedelta(data
+00011630: 5b27 476d 744f 6666 7365 7427 5d29 0a0a  ['GmtOffset'])..
+00011640: 2020 2020 7265 7475 726e 2064 6174 610a      return data.
+00011650: 0a0a 6465 6620 6665 7463 685f 7061 6765  ..def fetch_page
+00011660: 2870 6174 682c 206e 616d 6529 3a0a 2020  (path, name):.  
+00011670: 2020 2222 220a 2020 2020 2e2e 2077 6172    """.    .. war
+00011680: 6e69 6e67 3a3a 0a20 2020 2020 2020 203a  ning::.        :
+00011690: 6d6f 643a 6066 6173 7466 312e 6170 6960  mod:`fastf1.api`
+000116a0: 2077 696c 6c20 6265 2063 6f6e 7369 6465   will be conside
+000116b0: 7265 6420 7072 6976 6174 6520 696e 2066  red private in f
+000116c0: 7574 7572 6520 7265 6c65 6173 6573 2061  uture releases a
+000116d0: 6e64 0a20 2020 2020 2020 2070 6f74 656e  nd.        poten
+000116e0: 7469 616c 6c79 2062 6520 7265 6d6f 7665  tially be remove
+000116f0: 6420 6f72 2063 6861 6e67 6564 2e0a 0a20  d or changed... 
+00011700: 2020 2046 6574 6368 2064 6174 6120 6672     Fetch data fr
+00011710: 6f6d 2074 6865 2066 6f72 6d75 6c61 3120  om the formula1 
+00011720: 6c69 7665 7469 6d69 6e67 2077 6562 2061  livetiming web a
+00011730: 7069 2c20 6769 7665 6e20 7572 6c20 6261  pi, given url ba
+00011740: 7365 2070 6174 6820 616e 6420 7061 6765  se path and page
+00011750: 206e 616d 652e 2041 6e20 6174 7465 6d70   name. An attemp
+00011760: 740a 2020 2020 746f 2070 6172 7365 206a  t.    to parse j
+00011770: 736f 6e20 6f72 2064 6563 6f64 6520 6b6e  son or decode kn
+00011780: 6f77 6e20 6d65 7373 6167 6573 2069 7320  own messages is 
+00011790: 6d61 6465 2e0a 0a20 2020 2041 7267 733a  made...    Args:
+000117a0: 0a20 2020 2020 2020 2070 6174 6820 2873  .        path (s
+000117b0: 7472 293a 2061 7069 2070 6174 6820 6261  tr): api path ba
+000117c0: 7365 2073 7472 696e 6720 2875 7375 616c  se string (usual
+000117d0: 6c79 2060 6053 6573 7369 6f6e 2e61 7069  ly ``Session.api
+000117e0: 5f70 6174 6860 6029 0a20 2020 2020 2020  _path``).       
+000117f0: 206e 616d 6520 2873 7472 293a 2070 6167   name (str): pag
+00011800: 6520 6e61 6d65 2028 7365 6520 6060 6170  e name (see ``ap
+00011810: 692e 7061 6765 7360 6020 666f 7220 616c  i.pages`` for al
+00011820: 6c20 6b6e 6f77 6e20 7061 6765 7329 0a0a  l known pages)..
+00011830: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00011840: 2020 2020 202d 2064 6963 7469 6f6e 6172       - dictionar
+00011850: 7920 6966 2063 6f6e 7465 6e74 2077 6173  y if content was
+00011860: 206a 736f 6e0a 2020 2020 2020 2020 2d20   json.        - 
+00011870: 6c69 7374 206f 6620 656e 7472 6965 7320  list of entries 
+00011880: 6966 206a 736f 6e53 7472 6561 6d2c 2077  if jsonStream, w
+00011890: 6865 7265 2065 6163 6820 656e 7472 7920  here each entry 
+000118a0: 6167 6169 6e20 636f 6e74 6169 6e73 2074  again contains t
+000118b0: 776f 2065 6c65 6d65 6e74 733a 205b 7469  wo elements: [ti
+000118c0: 6d65 7374 616d 702c 2063 6f6e 7465 6e74  mestamp, content
+000118d0: 5d2e 2043 6f6e 7465 6e74 2069 730a 2020  ]. Content is.  
+000118e0: 2020 2020 2020 2020 7061 7273 6564 2077          parsed w
+000118f0: 6974 6820 3a66 756e 633a 6070 6172 7365  ith :func:`parse
+00011900: 6020 616e 6420 7769 6c6c 2075 7375 616c  ` and will usual
+00011910: 6c79 2062 6520 6120 6469 6374 696f 6e61  ly be a dictiona
+00011920: 7279 2063 7265 6174 6564 2066 726f 6d20  ry created from 
+00011930: 6a73 6f6e 2064 6174 612e 0a20 2020 2020  json data..     
+00011940: 2020 202d 204e 6f6e 6520 6966 2072 6571     - None if req
+00011950: 7565 7374 2066 6169 6c65 640a 0a20 2020  uest failed..   
+00011960: 2022 2222 0a20 2020 2070 6167 6520 3d20   """.    page = 
+00011970: 7061 6765 735b 6e61 6d65 5d0a 2020 2020  pages[name].    
+00011980: 6973 5f73 7472 6561 6d20 3d20 276a 736f  is_stream = 'jso
+00011990: 6e53 7472 6561 6d27 2069 6e20 7061 6765  nStream' in page
+000119a0: 0a20 2020 2069 735f 7a20 3d20 272e 7a2e  .    is_z = '.z.
+000119b0: 2720 696e 2070 6167 650a 2020 2020 7220  ' in page.    r 
+000119c0: 3d20 4361 6368 652e 7265 7175 6573 7473  = Cache.requests
+000119d0: 5f67 6574 2862 6173 655f 7572 6c20 2b20  _get(base_url + 
+000119e0: 7061 7468 202b 2070 6167 6573 5b6e 616d  path + pages[nam
+000119f0: 655d 2c20 6865 6164 6572 733d 6865 6164  e], headers=head
+00011a00: 6572 7329 0a20 2020 2069 6620 722e 7374  ers).    if r.st
+00011a10: 6174 7573 5f63 6f64 6520 3d3d 2032 3030  atus_code == 200
+00011a20: 3a0a 2020 2020 2020 2020 7261 7720 3d20  :.        raw = 
+00011a30: 722e 636f 6e74 656e 742e 6465 636f 6465  r.content.decode
+00011a40: 2827 7574 662d 382d 7369 6727 290a 2020  ('utf-8-sig').  
+00011a50: 2020 2020 2020 6966 2069 735f 7374 7265        if is_stre
+00011a60: 616d 3a0a 2020 2020 2020 2020 2020 2020  am:.            
+00011a70: 7265 636f 7264 7320 3d20 7261 772e 7370  records = raw.sp
+00011a80: 6c69 7428 275c 725c 6e27 295b 3a2d 315d  lit('\r\n')[:-1]
+00011a90: 2020 2320 6c61 7374 2073 706c 6974 2069    # last split i
+00011aa0: 7320 656d 7074 790a 2020 2020 2020 2020  s empty.        
+00011ab0: 2020 2020 6966 206e 616d 6520 696e 2028      if name in (
+00011ac0: 2770 6f73 6974 696f 6e27 2c20 2763 6172  'position', 'car
+00011ad0: 5f64 6174 6127 293a 0a20 2020 2020 2020  _data'):.       
+00011ae0: 2020 2020 2020 2020 2023 2053 7065 6369           # Speci
+00011af0: 616c 2063 6173 6520 746f 2069 6d70 726f  al case to impro
+00011b00: 7665 206d 656d 6f72 7920 6566 6669 6369  ve memory effici
+00011b10: 656e 6379 0a20 2020 2020 2020 2020 2020  ency.           
+00011b20: 2020 2020 2072 6574 7572 6e20 7265 636f       return reco
+00011b30: 7264 730a 2020 2020 2020 2020 2020 2020  rds.            
+00011b40: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00011b50: 2020 2020 2020 6465 636f 6465 5f65 7272        decode_err
+00011b60: 6f72 5f63 6f75 6e74 203d 2030 0a20 2020  or_count = 0.   
+00011b70: 2020 2020 2020 2020 2020 2020 2074 6c20               tl 
+00011b80: 3d20 3132 2020 2320 6c65 6e67 7468 206f  = 12  # length o
+00011b90: 6620 7469 6d65 7374 616d 703a 206c 656e  f timestamp: len
+00011ba0: 2827 3030 3a30 303a 3030 3a30 3030 2729  ('00:00:00:000')
+00011bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011bc0: 2072 6574 203d 206c 6973 7428 290a 2020   ret = list().  
+00011bd0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00011be0: 7220 6520 696e 2072 6563 6f72 6473 3a0a  r e in records:.
+00011bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c00: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00011c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c20: 2072 6574 2e61 7070 656e 6428 5b65 5b3a   ret.append([e[:
+00011c30: 746c 5d2c 2070 6172 7365 2865 5b74 6c3a  tl], parse(e[tl:
+00011c40: 5d2c 207a 6970 7065 643d 6973 5f7a 295d  ], zipped=is_z)]
+00011c50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00011c60: 2020 2020 2020 6578 6365 7074 206a 736f        except jso
+00011c70: 6e2e 4a53 4f4e 4465 636f 6465 4572 726f  n.JSONDecodeErro
+00011c80: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
+00011c90: 2020 2020 2020 2020 2020 2064 6563 6f64             decod
+00011ca0: 655f 6572 726f 725f 636f 756e 7420 2b3d  e_error_count +=
+00011cb0: 2031 0a20 2020 2020 2020 2020 2020 2020   1.             
+00011cc0: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+00011cd0: 6e75 650a 2020 2020 2020 2020 2020 2020  nue.            
+00011ce0: 2020 2020 6966 2064 6563 6f64 655f 6572      if decode_er
+00011cf0: 726f 725f 636f 756e 7420 3e20 303a 0a20  ror_count > 0:. 
+00011d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d10: 2020 205f 6c6f 6767 6572 2e77 6172 6e69     _logger.warni
+00011d20: 6e67 2866 2246 6169 6c65 6420 746f 2064  ng(f"Failed to d
+00011d30: 6563 6f64 6520 7b64 6563 6f64 655f 6572  ecode {decode_er
+00011d40: 726f 725f 636f 756e 747d 220a 2020 2020  ror_count}".    
+00011d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d70: 6622 206d 6573 7361 6765 7320 287b 6c65  f" messages ({le
+00011d80: 6e28 7265 636f 7264 7329 7d20 6d65 7373  n(records)} mess
+00011d90: 6167 6573 2022 0a20 2020 2020 2020 2020  ages ".         
+00011da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011db0: 2020 2020 2020 2020 2020 2066 2274 6f74             f"tot
+00011dc0: 616c 2922 290a 2020 2020 2020 2020 2020  al)").          
+00011dd0: 2020 2020 2020 7265 7475 726e 2072 6574        return ret
+00011de0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00011df0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00011e00: 6e20 7061 7273 6528 7261 772c 2069 735f  n parse(raw, is_
+00011e10: 7a29 0a20 2020 2065 6c73 653a 0a20 2020  z).    else:.   
+00011e20: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+00011e30: 0a0a 0a64 6566 2070 6172 7365 2874 6578  ...def parse(tex
+00011e40: 743a 2073 7472 2c20 7a69 7070 6564 3a20  t: str, zipped: 
+00011e50: 626f 6f6c 203d 2046 616c 7365 2920 2d3e  bool = False) ->
+00011e60: 2055 6e69 6f6e 5b73 7472 2c20 6469 6374   Union[str, dict
+00011e70: 5d3a 0a20 2020 2022 2222 0a20 2020 202e  ]:.    """.    .
+00011e80: 2e20 7761 726e 696e 673a 3a0a 2020 2020  . warning::.    
+00011e90: 2020 2020 3a6d 6f64 3a60 6661 7374 6631      :mod:`fastf1
+00011ea0: 2e61 7069 6020 7769 6c6c 2062 6520 636f  .api` will be co
+00011eb0: 6e73 6964 6572 6564 2070 7269 7661 7465  nsidered private
+00011ec0: 2069 6e20 6675 7475 7265 2072 656c 6561   in future relea
+00011ed0: 7365 7320 616e 640a 2020 2020 2020 2020  ses and.        
+00011ee0: 706f 7465 6e74 6961 6c6c 7920 6265 2072  potentially be r
+00011ef0: 656d 6f76 6564 206f 7220 6368 616e 6765  emoved or change
+00011f00: 642e 0a0a 2020 2020 5061 7273 6520 6a73  d...    Parse js
+00011f10: 6f6e 2061 6e64 206a 736f 6e53 7472 6561  on and jsonStrea
+00011f20: 6d20 6173 2072 6574 7572 6e65 6420 6279  m as returned by
+00011f30: 206c 6976 6574 696d 696e 672e 666f 726d   livetiming.form
+00011f40: 756c 6131 2e63 6f6d 0a0a 2020 2020 5468  ula1.com..    Th
+00011f50: 6973 2066 756e 6374 696f 6e20 6361 6e20  is function can 
+00011f60: 6f6e 6c79 2070 6173 7320 6f6e 6520 6461  only pass one da
+00011f70: 7461 2065 6e74 7279 2061 7420 6120 7469  ta entry at a ti
+00011f80: 6d65 2c20 6e6f 7420 6120 7768 6f6c 6520  me, not a whole 
+00011f90: 7265 7370 6f6e 7365 2e0a 2020 2020 5469  response..    Ti
+00011fa0: 6d65 7374 616d 7073 2061 6e64 2064 6174  mestamps and dat
+00011fb0: 6120 6e65 6564 2074 6f20 6265 2073 6570  a need to be sep
+00011fc0: 6172 6174 6564 2062 6566 6f72 6520 616e  arated before an
+00011fd0: 6420 6f6e 6c79 2074 6865 2064 6174 6120  d only the data 
+00011fe0: 6d75 7374 2062 6520 7061 7373 6564 2061  must be passed a
+00011ff0: 7320 6120 7374 7269 6e67 2074 6f20 6265  s a string to be
+00012000: 2070 6172 7365 642e 0a0a 2020 2020 4172   parsed...    Ar
+00012010: 6773 3a0a 2020 2020 2020 2020 7465 7874  gs:.        text
+00012020: 3a20 5468 6520 7374 7269 6e67 2077 6869  : The string whi
+00012030: 6368 2073 686f 756c 6420 6265 2070 6172  ch should be par
+00012040: 7365 640a 2020 2020 2020 2020 7a69 7070  sed.        zipp
+00012050: 6564 3a20 5768 6574 6865 7220 7468 6520  ed: Whether the 
+00012060: 7465 7874 2069 7320 636f 6d70 7265 7373  text is compress
+00012070: 6564 2e20 5468 6973 2069 7320 7468 6520  ed. This is the 
+00012080: 6361 7365 2066 6f72 2020 272e 7a27 0a20  case for  '.z'. 
+00012090: 2020 2020 2020 2020 2020 2064 6174 6120             data 
+000120a0: 2865 2e67 2e20 706f 7369 7469 6f6e 2064  (e.g. position d
+000120b0: 6174 6129 0a0a 2020 2020 5265 7475 726e  ata)..    Return
+000120c0: 733a 0a20 2020 2020 2020 2044 6570 656e  s:.        Depen
+000120d0: 6469 6e67 206f 6e20 6461 7461 206f 6620  ding on data of 
+000120e0: 7768 6963 6820 7061 6765 2069 7320 7061  which page is pa
+000120f0: 7273 6564 0a20 2020 2020 2020 2020 2020  rsed.           
+00012100: 202d 2061 2064 6963 7469 6f6e 6172 7920   - a dictionary 
+00012110: 6372 6561 7465 6420 6173 2061 2072 6573  created as a res
+00012120: 756c 7420 6f66 206c 6f61 6469 6e67 206a  ult of loading j
+00012130: 736f 6e20 6461 7461 0a20 2020 2020 2020  son data.       
+00012140: 2020 2020 202d 2061 2073 7472 696e 670a       - a string.
+00012150: 2020 2020 2222 220a 2020 2020 6966 2074      """.    if t
+00012160: 6578 745b 305d 203d 3d20 277b 273a 0a20  ext[0] == '{':. 
+00012170: 2020 2020 2020 2072 6574 7572 6e20 6a73         return js
+00012180: 6f6e 2e6c 6f61 6473 2874 6578 7429 0a20  on.loads(text). 
+00012190: 2020 2069 6620 7465 7874 5b30 5d20 3d3d     if text[0] ==
+000121a0: 2027 2227 3a0a 2020 2020 2020 2020 7465   '"':.        te
+000121b0: 7874 203d 2074 6578 742e 7374 7269 7028  xt = text.strip(
+000121c0: 2722 2729 0a20 2020 2069 6620 7a69 7070  '"').    if zipp
+000121d0: 6564 3a0a 2020 2020 2020 2020 7465 7874  ed:.        text
+000121e0: 203d 207a 6c69 622e 6465 636f 6d70 7265   = zlib.decompre
+000121f0: 7373 2862 6173 6536 342e 6236 3464 6563  ss(base64.b64dec
+00012200: 6f64 6528 7465 7874 292c 202d 7a6c 6962  ode(text), -zlib
+00012210: 2e4d 4158 5f57 4249 5453 290a 2020 2020  .MAX_WBITS).    
+00012220: 2020 2020 7265 7475 726e 2070 6172 7365      return parse
+00012230: 2874 6578 742e 6465 636f 6465 2827 7574  (text.decode('ut
+00012240: 662d 382d 7369 6727 2929 0a20 2020 205f  f-8-sig')).    _
+00012250: 6c6f 6767 6572 2e77 6172 6e69 6e67 2822  logger.warning("
+00012260: 436f 756c 646e 2774 2070 6172 7365 2074  Couldn't parse t
+00012270: 6578 7422 290a 2020 2020 7265 7475 726e  ext").    return
+00012280: 2074 6578 740a 0a0a 636c 6173 7320 5365   text...class Se
+00012290: 7373 696f 6e4e 6f74 4176 6169 6c61 626c  ssionNotAvailabl
+000122a0: 6545 7272 6f72 2845 7863 6570 7469 6f6e  eError(Exception
+000122b0: 293a 0a20 2020 2022 2222 5261 6973 6564  ):.    """Raised
+000122c0: 2069 6620 616e 2061 7069 2072 6571 7565   if an api reque
+000122d0: 7374 2072 6574 7572 6e65 6420 6e6f 2064  st returned no d
+000122e0: 6174 6120 666f 7220 7468 6520 7265 7175  ata for the requ
+000122f0: 6573 7465 6420 7365 7373 696f 6e2e 0a20  ested session.. 
+00012300: 2020 2041 206c 696b 656c 7920 6361 7573     A likely caus
+00012310: 6520 6973 2074 6861 7420 7468 6520 7365  e is that the se
+00012320: 7373 696f 6e20 646f 6573 206e 6f74 2065  ssion does not e
+00012330: 7869 7374 2062 6563 6175 7365 2069 7420  xist because it 
+00012340: 7761 7320 6361 6e63 656c 6c65 642e 2222  was cancelled.""
+00012350: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
+00012360: 745f 5f28 7365 6c66 2c20 2a61 7267 7329  t__(self, *args)
+00012370: 3a0a 2020 2020 2020 2020 7375 7065 7228  :.        super(
+00012380: 292e 5f5f 696e 6974 5f5f 282a 6172 6773  ).__init__(*args
+00012390: 290a                                     ).
```

### Comparing `fastf1-3.3.7/fastf1/api.py` & `fastf1-3.4.0a0/fastf1/api.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.7/fastf1/core.py` & `fastf1-3.4.0a0/fastf1/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,26 +75,14 @@
     get_circuit_info
 )
 from fastf1.utils import to_timedelta
 
 
 _logger = get_logger(__name__)
 
-D_LOOKUP: List[List] = \
-    [[44, 'HAM', 'Mercedes'], [77, 'BOT', 'Mercedes'],
-     [55, 'SAI', 'Ferrari'], [16, 'LEC', 'Ferrari'],
-     [33, 'VER', 'Red Bull'], [11, 'PER', 'Red Bull'],
-     [3, 'RIC', 'McLaren'], [4, 'NOR', 'McLaren'],
-     [5, 'VET', 'Aston Martin'], [18, 'STR', 'Aston Martin'],
-     [14, 'ALO', 'Alpine'], [31, 'OCO', 'Alpine'],
-     [22, 'TSU', 'AlphaTauri'], [10, 'GAS', 'AlphaTauri'],
-     [47, 'MSC', 'Haas F1 Team'], [9, 'MAZ', 'Haas F1 Team'],
-     [7, 'RAI', 'Alfa Romeo'], [99, 'GIO', 'Alfa Romeo'],
-     [6, 'LAT', 'Williams'], [63, 'RUS', 'Williams']]
-
 
 class Telemetry(pd.DataFrame):
     """Multi-channel time series telemetry data
 
     The object can contain multiple telemetry channels. Multiple telemetry
     objects with different channels can be merged on time. Each telemetry
     channel is one dataframe column. Partial telemetry (e.g. for one lap only)
@@ -317,29 +305,29 @@
             pad_side: Where to pad the data; possible options:
                 'both', 'before', 'after
             interpolate_edges: Add an interpolated sample at the beginning
                 and end to exactly match the provided time window.
         """
         if isinstance(ref_laps, Laps) and len(ref_laps) > 1:
             if 'DriverNumber' not in ref_laps.columns:
-                ValueError("Laps is missing 'DriverNumber'. Cannot return "
-                           "telemetry for unknown driver.")
+                raise ValueError("Laps is missing 'DriverNumber'. "
+                           "Cannot return telemetry for unknown driver.")
             if not len(ref_laps['DriverNumber'].unique()) <= 1:
                 raise ValueError("Cannot create telemetry for multiple "
                                  "drivers at once!")
 
             end_time = ref_laps['Time'].max()
             start_time = ref_laps['LapStartTime'].min()
 
         elif isinstance(ref_laps, (Lap, Laps)):
             if isinstance(ref_laps, Laps):  # one lap in Laps
                 ref_laps = ref_laps.iloc[0]  # handle as a single lap
             if 'DriverNumber' not in ref_laps.index:
-                ValueError("Lap is missing 'DriverNumber'. Cannot return "
-                           "telemetry for unknown driver.")
+                raise ValueError("Lap is missing 'DriverNumber'. "
+                           "Cannot return telemetry for unknown driver.")
             end_time = ref_laps['Time']
             start_time = ref_laps['LapStartTime']
 
         else:
             raise TypeError("Attribute 'ref_laps' needs to be an instance of "
                             "`Lap` or `Laps`")
 
@@ -455,15 +443,15 @@
         # save dtypes before merging, so they can be restored after merging
         # necessary for example because merging produces NaN values which
         # would cause an int column to become float, but it can be converted
         # back to int after interpolating missing values
         dtype_map = dict()
         for df in data, other:
             for col in df.columns:
-                if col not in dtype_map.keys():
+                if col not in dtype_map:
                     dtype_map[col] = df[col].dtype
 
         # Exclude columns existing on both dataframes from one dataframe
         # before merging (cannot merge with duplicates)
         on_both_columns = set(other.columns).intersection(set(data.columns))
         merged = other.merge(
             data[data.columns.difference(on_both_columns, sort=False)],
@@ -497,15 +485,15 @@
             merged = merged.reset_index().rename(columns={'index': 'Date'})
 
         else:
             frq = pd.Timedelta(seconds=1/frequency)
 
             resampled_columns = dict()
 
-            for ch in self._CHANNELS.keys():
+            for ch in self._CHANNELS:
                 if ch not in merged.columns:
                     continue
                 sig_type = self._CHANNELS[ch]['type']
 
                 if sig_type == 'continuous':
                     method = self._CHANNELS[ch]['method']
                     if method in ('nearest', 'zero', 'slinear', 'quadratic',
@@ -562,15 +550,15 @@
             # recalculate the time columns
             merged['SessionTime'] \
                 = merged['Date'] - self.session.t0_date
             merged['Time'] \
                 = merged['SessionTime'] - merged['SessionTime'].iloc[0]
 
         # restore data types from before merging
-        for col in dtype_map.keys():
+        for col in dtype_map:
             try:
                 merged[col] = merged.loc[:, col].astype(dtype_map[col])
             except ValueError:
                 _logger.warning(f"Failed to preserve data type for column "
                                 f"'{col}' while merging telemetry.")
 
         return merged
@@ -641,15 +629,15 @@
         | Linear interpolation will be used for continuous values (Speed, RPM)
         | Forward-fill will be used for discrete values (Gear, DRS, ...)
 
         See :meth:`register_new_channel` for adding custom channels.
         """
         ret = self.copy()
 
-        for ch in self._CHANNELS.keys():
+        for ch in self._CHANNELS:
             if ch not in self.columns:
                 continue
             sig_type = self._CHANNELS[ch]['type']
             if sig_type == 'continuous':
                 if ret[ch].dtype == 'object':
                     warnings.warn("Interpolation not possible for telemetry "
                                   "channel because dtype is 'object'")
@@ -1492,15 +1480,15 @@
             self._results = SessionResults(_nums_df.join(_info_df),
                                            force_default_cols=True)
 
             _logger.warning("Generating minimal driver "
                             "list from timing data.")
 
         df = None
-        for i, driver in enumerate(drivers):
+        for _, driver in enumerate(drivers):
             d1 = data[data['Driver'] == driver]
             d2 = useful[useful['Driver'] == driver]
             if d2.shape[0] != len(d2['Stint'].unique()):
                 # tyre info includes correction messages that need to be
                 # applied before continuing
                 d2 = self.__fix_tyre_info(d2)
 
@@ -1757,16 +1745,14 @@
                 'TyreLife': [drv_laps['TyreLife'].iloc[-1] + 1],
                 'FreshTyre': [drv_laps['FreshTyre'].iloc[-1]],
                 'Position': [np.NaN],
                 'FastF1Generated': [True],
                 'IsAccurate': [False]
             })
 
-            self._add_track_status_to_laps(new_last)
-
             # add generated laps at the end and fix sorting at the end
             self._laps = (pd.concat([self._laps, new_last])
                           .__finalize__(self._laps))
             any_new = True
 
         if any_new:
             # re-sort and re-index to restore correct order of the laps
@@ -2116,15 +2102,15 @@
                         lap_integrity_ok = False
                 else:
                     check_2 = False  # data not available means fail
 
                 if prev_lap is not None:
                     # first lap after safety car often has timing issues
                     # (as do all laps under safety car)
-                    check_3 = (prev_lap['TrackStatus'] != '4')
+                    check_3 = prev_lap['TrackStatus'] != '4'
                 else:
                     check_3 = True  # no previous lap, no SC error
 
                 pre_check_4 = (((not pd.isnull(lap['Time']))
                                & (not pd.isnull(lap['LapTime'])))
                                and (prev_lap is not None)
                                and (not pd.isnull(prev_lap['Time'])))
@@ -2478,20 +2464,14 @@
         marshal sectors and the rotation of the track map. Note that the data
         is manually created and therefore not highly accurate, but it is useful
         for annotating data visualizations.
 
         See :class:`~fastf1.mvapi.CircuitInfo` for detailed information.
         """
         circuit_key = self.session_info['Meeting']['Circuit']['Key']
-
-        if ((circuit_key == 149)
-                and (self.session_info['Meeting']['Circuit']['ShortName']
-                     == 'Mugello')):
-            circuit_key = 146
-
         circuit_info = get_circuit_info(year=self.event.year,
                                         circuit_key=circuit_key)
         circuit_info.add_marker_distance(
             reference_lap=self.laps.pick_fastest()
         )
         return circuit_info
 
@@ -3040,17 +3020,14 @@
         .. deprecated:: 3.1.0
             pick_team is deprecated and will be removed in a future release.
             Use :func:`pick_teams` instead.
 
             mercedes = session_laps.pick_team('Mercedes')
             alfa_romeo = session_laps.pick_team('Alfa Romeo')
 
-        Have a look to :attr:`fastf1.plotting.TEAM_COLORS` for a quick
-        reference on team names.
-
         Args:
             name (str): Team name
 
         Returns:
             instance of :class:`Laps`
         """
         warnings.warn(("pick_team is deprecated and will be removed"
```

### Comparing `fastf1-3.3.7/fastf1/events.py` & `fastf1-3.4.0a0/fastf1/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,15 +203,15 @@
 
 with warnings.catch_warnings():
     warnings.filterwarnings(
         'ignore', message="Using slow pure-python SequenceMatcher"
     )
     # suppress that warning, it's confusing at best here, we don't need fast
     # sequence matching and the installation (on windows) requires some effort
-    from thefuzz import fuzz
+    from rapidfuzz import fuzz
 
 import pandas as pd
 
 import fastf1._api
 import fastf1.ergast
 from fastf1.core import Session
 from fastf1.internals.pandas_base import (
@@ -357,15 +357,16 @@
 
 def get_event(
         year: int,
         gp: Union[int, str],
         *,
         backend: Optional[Literal['fastf1', 'f1timing', 'ergast']] = None,
         force_ergast: bool = False,
-        strict_search: bool = False
+        strict_search: bool = False,
+        exact_match: bool = False
 ) -> "Event":
     """Create an :class:`~fastf1.events.Event` object for a specific
     season and gp.
 
     To get a testing event, use :func:`get_testing_event`.
 
     Args:
@@ -396,26 +397,30 @@
             is not available.
 
             For seasons older than 2018 ``'ergast'`` is always used.
 
         force_ergast: [Deprecated, use ``backend='ergast'``] Always use data
             from the ergast database to create the event schedule
 
-        strict_search: Match precisely the query, or default to
+        strict_search: This argument is deprecated and planned for removal,
+            use the equivalent ``exact_match`` instead
+
+        exact_match: Match precisely the query, or default to
             fuzzy search. If no event is found with
-            ``strict_search=True``, the function will return None
+            ``exact_match=True``, the function will return None
 
     .. versionadded:: 2.2
     """
     schedule = get_event_schedule(year=year, include_testing=False,
                                   force_ergast=force_ergast,
                                   backend=backend)
 
     if isinstance(gp, str):
-        event = schedule.get_event_by_name(gp, strict_search=strict_search)
+        event = schedule.get_event_by_name(
+            gp, strict_search=strict_search, exact_match=exact_match)
     else:
         event = schedule.get_event_by_round(gp)
 
     return event
 
 
 def get_testing_event(
@@ -923,46 +928,76 @@
                 if event['EventName'].lower() == query:
                     return self.loc[i]
         else:
             return None
 
     def _fuzzy_event_search(self, name: str) -> "Event":
 
+        def _remove_common_words(event_name):
+            common_words = ["formula 1", str(self.year), "grand prix", "gp"]
+            event_name = event_name.casefold()
+
+            for word in common_words:
+                event_name = event_name.replace(word, "")
+
+            return event_name.replace(" ", "")
+
         def _matcher_strings(ev):
             strings = list()
             if 'Location' in ev:
-                strings.append(ev['Location'])
+                strings.append(ev['Location'].casefold())
             if 'Country' in ev:
-                strings.append(ev['Country'])
+                strings.append(ev['Country'].casefold())
             if 'EventName' in ev:
-                strings.append(ev['EventName'].replace("Grand Prix", ""))
+                strings.append(_remove_common_words(ev["EventName"]))
             if 'OfficialEventName' in ev:
-                strings.append(ev['OfficialEventName']
-                               .replace("FORMULA 1", "")
-                               .replace(str(self.year), "")
-                               .replace("GRAND PRIX", ""))
+                strings.append(_remove_common_words(ev["OfficialEventName"]))
             return strings
 
-        max_ratio = 0
-        index = 0
+        user_input = name
+        name = _remove_common_words(name)
+        full_partial_match_indices = []
+
+        # check partial matches first
+        # if there is either zero or multiple 100% matches
+        # fall back to the full ratio
         for i, event in self.iterrows():
+            if any([name in val for val in _matcher_strings(event)]):
+                full_partial_match_indices.append(i)
+
+        if len(full_partial_match_indices) == 1:
+            return self.loc[full_partial_match_indices[0]]
+
+        max_ratio = 0
+        max_index = 0
+
+        for i, event in self.loc[full_partial_match_indices
+                                  or self.index].iterrows():
             ratio = max(
-                [fuzz.ratio(val.casefold(), name.casefold())
+                [fuzz.ratio(val, name)
                  for val in _matcher_strings(event)]
             )
             if ratio > max_ratio:
                 max_ratio = ratio
-                index = i
-        return self.loc[index]
+                max_index = i
+
+        if max_ratio != 100:
+            _logger.warning((
+                "Correcting user input "
+                f"'{user_input}' to'{self.loc[max_index].EventName}'"
+            )
+            )
+        return self.loc[max_index]
 
     def get_event_by_name(
             self,
             name: str,
             *,
-            strict_search: bool = False
+            strict_search: bool = False,
+            exact_match: bool = False
     ) -> "Event":
         """Get an :class:`Event` by its name.
 
         A fuzzy match is performed to find the event that best matches the
         given name. Fuzzy matching is performed using the country, location,
         name and officialName of each event. This is not guaranteed to return
         the correct result. You should therefore always check if the function
@@ -977,24 +1012,29 @@
             Grand Prix" as ``name``.
 
         Args:
             name: The name of the event. For example,
                 ``.get_event_by_name("british")`` and
                 ``.get_event_by_name("silverstone")`` will both return the
                 event for the British Grand Prix.
-            strict_search: Search only for exact query matches
+            strict_search: This argument is deprecated and planned for removal.
+                Use the equivalent ``exact_match`` instead
+            exact_match: Search only for exact query matches
                 instead of using fuzzy search. For example,
                 ``.get_event_by_name("British Grand Prix",
-                strict_search=True)``
+                exact_match=True)``
                 will return the event for the British Grand Prix, whereas
-                ``.get_event_by_name("British", strict_search=True)``
+                ``.get_event_by_name("British", exact_match=True)``
                 will return ``None``
         """
-
         if strict_search:
+            warnings.warn(("strict_search is deprecated and planned for "
+                           "removal, use the equivalent exact_match instead"),
+                          FutureWarning)
+        if strict_search or exact_match:
             return self._strict_event_search(name)
         else:
             return self._fuzzy_event_search(name)
 
 
 class Event(BaseSeries):
     """This class represents a single event (race weekend or testing event).
```

### Comparing `fastf1-3.3.7/fastf1/legacy.py` & `fastf1-3.4.0a0/fastf1/legacy.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     import fastf1
     import fastf1.plotting
     import fastf1.legacy
     import numpy as np
     import matplotlib.pyplot as plt
 
-    fastf1.plotting.setup_mpl()
+    fastf1.plotting.setup_mpl(misc_mpl_mods=False, color_scheme='fastf1')
 
     session = fastf1.get_session(2020, 'Italy', 'R')
     session.load()
 
     DRIVER = 'VER'  # which driver; need to specify number and abbreviation
     DRIVER_NUMBER = '33'
     LAP_N = 10  # which lap number to plot
```

### Comparing `fastf1-3.3.7/fastf1/logger.py` & `fastf1-3.4.0a0/fastf1/logger.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.7/fastf1/plotting.py` & `fastf1-3.4.0a0/fastf1/plotting/_plotting.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,206 +1,77 @@
-"""
-Helper functions for creating data plots.
-
-:mod:`fastf1.plotting` provides optional functionality with the intention of
-making it easy to create nice plots.
-
-This module offers mainly two things:
-    - team names and colors
-    - matplotlib mods and helper functions
-
-Fast-F1 focuses on plotting data with matplotlib. Of course, you are not
-required to use matplotlib and you can use any other tool you like.
-
-If you wish to use matplotlib, it is highly recommended to enable some
-helper functions by calling :func:`setup_mpl`.
-
-If you don't want to use matplotlib, you can still use the team names
-and colors which are provided below.
-
-
-.. note:: Plotting related functionality is likely to change in a future
-    release.
-"""
 import warnings
 from typing import (
-    Dict,
-    List
+    List,
+    Optional
 )
 
 import numpy as np
 import pandas as pd
 
 
 try:
     import matplotlib
     from matplotlib import cycler
     from matplotlib import pyplot as plt
 except ImportError:
     warnings.warn("Failed to import optional dependency 'matplotlib'!"
-                  "Plotting functionality will be unavailable!", UserWarning)
+                  "Plotting functionality will be unavailable!",
+                  RuntimeWarning)
 try:
     import timple
 except ImportError:
     warnings.warn("Failed to import optional dependency 'timple'!"
                   "Plotting of timedelta values will be restricted!",
-                  UserWarning)
+                  RuntimeWarning)
 
-import warnings
+from rapidfuzz import fuzz
+
+from fastf1.logger import get_logger
+from fastf1.plotting._constants import (
+    LEGACY_DRIVER_COLORS,
+    LEGACY_DRIVER_TRANSLATE,
+    LEGACY_TEAM_COLORS,
+    LEGACY_TEAM_TRANSLATE
+)
 
 
-with warnings.catch_warnings():
-    warnings.filterwarnings('ignore',
-                            message="Using slow pure-python SequenceMatcher")
-    # suppress that warning, it's confusing at best here, we don't need fast
-    # sequence matching and the installation (on windows) some effort
-    from thefuzz import fuzz
-
-
-class __TeamColorsWarnDict(dict):
-    """Implements userwarning on KeyError in :any:`TEAM_COLORS` after
-    changing team names."""
-
-    def get(self, key, default=None):
-        value = super().get(key, default)
-        if value is None:
-            self.warn_change()
-        return value
-
-    def __getitem__(self, item):
-        try:
-            return super().__getitem__(item)
-        except KeyError as err:
-            self.warn_change()
-            raise err
-        except Exception as err:
-            raise err
+_logger = get_logger(__package__)
+
+
+_COLOR_PALETTE: List[str] = ['#FF79C6', '#50FA7B', '#8BE9FD', '#BD93F9',
+                             '#FFB86C', '#FF5555', '#F1FA8C']
+# The default color palette for matplotlib plot lines in fastf1's color scheme
 
-    def warn_change(self):
-        warnings.warn(
-            "Team names in `TEAM_COLORS` are now lower-case and only contain "
-            "the most identifying part of the name. "
-            "Use function `.team_color` alternatively.", UserWarning
-        )
 
+class __DefaultStringArgType(str):
+    pass
 
-TEAM_COLORS = __TeamColorsWarnDict({
-    'mercedes': '#00d2be', 'ferrari': '#dc0000',
-    'red bull': '#fcd700', 'mclaren': '#ff8700',
-    'alpine': '#fe86bc', 'aston martin': '#006f62',
-    'sauber': '#00e701', 'visa rb': '#1634cb',
-    'haas': '#ffffff', 'williams': '#00a0dd'
-})
-"""Mapping of team names to team colors (hex color codes).
-(current season only)"""
-
-TEAM_TRANSLATE: Dict[str, str] = {
-    'MER': 'mercedes', 'FER': 'ferrari',
-    'RBR': 'red bull', 'MCL': 'mclaren',
-    'APN': 'alpine', 'AMR': 'aston martin',
-    'SAU': 'sauber', 'VRB': 'visa rb',
-    'HAA': 'haas', 'WIL': 'williams'}
-"""Mapping of team names to theirs respective abbreviations."""
-
-DRIVER_COLORS: Dict[str, str] = {
-    "valtteri bottas": "#00e701",
-    "zhou guanyu": "#008d01",
-    "theo pourchaire": "#004601",
-
-    "nyck de vries": "#1e3d61",
-    "yuki tsunoda": "#356cac",
-    "daniel ricciardo": "#2b4562",
-    "liam lawson": "#2b4562",
-    "isack hadjar": "#1e6176",
-    "ayumu iwasa": "#1e6176",
-
-    "pierre gasly": "#fe86bc",
-    "esteban ocon": "#ff117c",
-    "jack doohan": "#894667",
-
-    "fernando alonso": "#006f62",
-    "lance stroll": "#00413b",
-    "felipe drugovich": "#2f9b90",
-
-    "charles leclerc": "#dc0000",
-    "carlos sainz": "#ff8181",
-    "robert shwartzman": "#9c0000",
-    "oliver bearman": "#c40000",
-
-    "kevin magnussen": "#ffffff",
-    "nico hulkenberg": "#cacaca",
-
-    "oscar piastri": "#ff8700",
-    "lando norris": "#eeb370",
-    "pato oward": "#ee6d3a",
-
-    "lewis hamilton": "#00d2be",
-    "george russell": "#24ffff",
-    "frederik vesti": "#00a6ff",
-
-    "max verstappen": "#fcd700",
-    "sergio perez": "#ffec7b",
-    "jake dennis": "#907400",
-
-    "alexander albon": "#005aff",
-    "logan sargeant": "#012564",
-    "zak osullivan": "#1b3d97",
-}
-"""Mapping of driver names to driver colors (hex color codes).
-(current season only)"""
-
-DRIVER_TRANSLATE: Dict[str, str] = {
-    'LEC': 'charles leclerc', 'SAI': 'carlos sainz',
-    'SHW': 'robert shwartzman',
-    'VER': 'max verstappen', 'PER': 'sergio perez',
-    'DEN': 'jake dennis',
-    'PIA': 'oscar piastri', 'NOR': 'lando norris',
-    'OWA': 'pato oward',
-    'GAS': 'pierre gasly', 'OCO': 'esteban ocon',
-    'DOO': 'jack doohan',
-    'BOT': 'valtteri bottas', 'ZHO': 'zhou guanyu',
-    'POU': 'theo pourchaire',
-    'DEV': 'nyck de vries', 'TSU': 'yuki tsunoda',
-    'RIC': 'daniel ricciardo', 'LAW': 'liam lawson',
-    'HAD': 'isack hadjar', 'IWA': 'ayumu iwasa',
-    'MAG': 'kevin magnussen', 'HUL': 'nico hulkenberg',
-    'BEA': 'oliver bearman',
-    'ALO': 'fernando alonso', 'STR': 'lance stroll',
-    'DRU': 'felipe drugovich',
-    'HAM': 'lewis hamilton', 'RUS': 'george russell',
-    'VES': 'frederik vesti',
-    'ALB': 'alexander albon', 'SAR': 'logan sargeant',
-    'OSU': 'zak osullivan'}
-"""Mapping of driver names to theirs respective abbreviations."""
-
-COMPOUND_COLORS: Dict[str, str] = {
-    "SOFT": "#da291c",
-    "MEDIUM": "#ffd12e",
-    "HARD": "#f0f0ec",
-    "INTERMEDIATE": "#43b02a",
-    "WET": "#0067ad",
-    "UNKNOWN": "#00ffff",
-    "TEST-UNKNOWN": "#434649"
-}
-"""Mapping of tyre compound names to compound colors (hex color codes).
-(current season only)"""
-
-COLOR_PALETTE: List[str] = ['#FF79C6', '#50FA7B', '#8BE9FD', '#BD93F9',
-                            '#FFB86C', '#FF5555', '#F1FA8C']
-"""The default color palette for matplotlib plot lines in fastf1's color
-scheme."""
+
+__color_scheme_default_arg = __DefaultStringArgType('fastf1')
 
 
 def setup_mpl(
-        mpl_timedelta_support: bool = True, color_scheme: str = 'fastf1',
+        mpl_timedelta_support: bool = True,
+        color_scheme: Optional[str] = __color_scheme_default_arg,
         misc_mpl_mods: bool = True):
     """Setup matplotlib for use with fastf1.
 
     This is optional but, at least partly, highly recommended.
 
+    .. deprecated:: 3.4.0
+
+        The optional argument ``misc_mpls_mods`` is deprecated.
+
+    .. deprecated:: 3.4.0
+
+        The default value for ``color_scheme`` will change from ``'fastf1'``
+        to ``None``. You should explicitly set the desired value when calling
+        this function.
+
+
     Parameters:
         mpl_timedelta_support (bool):
             Matplotlib itself offers very limited functionality for plotting
             timedelta values. (Lap times, sector times and other kinds of time
             spans are represented as timedelta.)
 
             Enabling this option will patch some internal matplotlib functions
@@ -211,188 +82,208 @@
 
         color_scheme (str, None):
             This enables the Fast-F1 color scheme that you can see in all
             example images.
             Valid color scheme names are: ['fastf1', None]
 
         misc_mpl_mods (bool):
-            This enables a collection of patches for the following mpl
-            features:
-
-                - ``.savefig`` (saving of figures)
-                - ``.bar``/``.barh`` (plotting of bar graphs)
-                - ``plt.subplots`` (for creating a nice background grid)
+            This argument is deprecated since v3.4.0 and should no longer be
+            used.
     """
+    if color_scheme is __color_scheme_default_arg:
+        warnings.warn(
+            "FastF1 will no longer silently modify the default Matplotlib "
+            "colors in the future.\nTo remove this warning, explicitly set "
+            "`color_scheme=None` or `color_scheme='fastf1'` when calling "
+            "`.setup_mpl()`.", FutureWarning
+        )
+
+    if misc_mpl_mods:
+        warnings.warn(
+            "FastF1 will stop modifying the default Matplotlib settings in "
+            "the future.\nTo opt-in to the new behaviour and remove this "
+            "warning, explicitly set `misc_mpl_mods=False` when calling "
+            "`.setup_mpl()`.", FutureWarning
+        )
+
     if mpl_timedelta_support:
         _enable_timple()
     if color_scheme == 'fastf1':
         _enable_fastf1_color_scheme()
     if misc_mpl_mods:
         _enable_misc_mpl_mods()
 
 
 def driver_color(identifier: str) -> str:
-    """Get a driver's color from a driver name or abbreviation.
+    """
+    Get a driver's color from a driver name or abbreviation.
+
+    .. deprecated:: 3.4.0
+        This function is deprecated and will be removed in a future version.
+        Use :func:`~fastf1.plotting.get_driver_color` instead.
 
     This function will try to find a matching driver for any identifier string
-    that is passed to it. This involves case insensitive matching and partial
+    that is passed to it. This involves case-insensitive matching and partial
     string matching.
 
-    If you want exact string matching, you should use the
-    :any:`DRIVER_COLORS` dictionary directly, using :any:`DRIVER_TRANSLATE` to
-    convert abbreviations to team names if necessary.
-
     Example::
 
-        >>> driver_color('charles leclerc')
+        >>> driver_color('charles leclerc')  # doctest: +SKIP
         '#dc0000'
-        >>> driver_color('max verstappen')
+        >>> driver_color('max verstappen')  # doctest: +SKIP
         '#fcd700'
-        >>> driver_color('ver')
+        >>> driver_color('ver')  # doctest: +SKIP
         '#fcd700'
-        >>> driver_color('lec')
+        >>> driver_color('lec')  # doctest: +SKIP
         '#dc0000'
 
         shortened driver names and typos can be dealt with
         too (within reason)
 
-        >>> driver_color('Max Verst')
+        >>> driver_color('Max Verst')  # doctest: +SKIP
         '#fcd700'
-        >>> driver_color('Charles')
+        >>> driver_color('Charles')  # doctest: +SKIP
         '#dc0000'
 
     Args:
         identifier (str): Abbreviation or uniquely identifying name of the
             driver.
 
     Returns:
         str: hex color code
     """
+    warnings.warn("The function `driver_color` is deprecated and will be "
+                  "removed in a future version. Use "
+                  "`fastf1.plotting.get_driver_color` instead.",
+                  FutureWarning)
 
-    if identifier.upper() in DRIVER_TRANSLATE:
+    if identifier.upper() in LEGACY_DRIVER_TRANSLATE:
         # try short team abbreviations first
-        return DRIVER_COLORS[DRIVER_TRANSLATE[identifier.upper()]]
+        return LEGACY_DRIVER_COLORS[
+            LEGACY_DRIVER_TRANSLATE[identifier.upper()]
+        ]
     else:
         identifier = identifier.lower()
 
         # check for an exact team name match
-        if identifier in DRIVER_COLORS:
-            return DRIVER_COLORS[identifier]
+        if identifier in LEGACY_DRIVER_COLORS:
+            return LEGACY_DRIVER_COLORS[identifier]
 
         # check for exact partial string match
-        for team_name, color in DRIVER_COLORS.items():
+        for team_name, color in LEGACY_DRIVER_COLORS.items():
             if identifier in team_name:
                 return color
 
         # do fuzzy string matching
         key_ratios = list()
-        for existing_key in DRIVER_COLORS.keys():
+        for existing_key in LEGACY_DRIVER_COLORS:
             ratio = fuzz.ratio(identifier, existing_key)
             key_ratios.append((ratio, existing_key))
         key_ratios.sort(reverse=True)
+        if key_ratios[0][0] != 100:
+            _logger.warning(
+                ("Correcting invalid user input "
+                 f"'{identifier}' to '{key_ratios[0][1]}'."
+                 )
+            )
         if ((key_ratios[0][0] < 35)
                 or (key_ratios[0][0] / key_ratios[1][0] < 1.2)):
             # ensure that the best match has a minimum accuracy (35 out of
             # 100) and that it has a minimum confidence (at least 20% better
             # than second best)
             raise KeyError
         best_matched_key = key_ratios[0][1]
-        return DRIVER_COLORS[best_matched_key]
+        return LEGACY_DRIVER_COLORS[best_matched_key]
 
 
 def team_color(identifier: str) -> str:
-    """Get a team's color from a team name or abbreviation.
+    """
+    Get a team's color from a team name or abbreviation.
+
+    .. deprecated:: 3.4.0
+        This function is deprecated and will be removed in a future version.
+        Use :func:`~fastf1.plotting.get_team_color` instead.
 
     This function will try to find a matching team for any identifier string
-    that is passed to it. This involves case insensitive matching and partial
+    that is passed to it. This involves case-insensitive matching and partial
     string matching.
 
-    If you want exact string matching, you should use the
-    :any:`TEAM_COLORS` dictionary directly, using :any:`TEAM_TRANSLATE` to
-    convert abbreviations to team names if necessary.
-
     Example::
 
-        >>> team_color('Red Bull')
+        >>> team_color('Red Bull')  # doctest: +SKIP
         '#fcd700'
-        >>> team_color('redbull')
+        >>> team_color('redbull')  # doctest: +SKIP
         '#fcd700'
-        >>> team_color('Red')
+        >>> team_color('Red')  # doctest: +SKIP
         '#fcd700'
-        >>> team_color('RBR')
+        >>> team_color('RBR')  # doctest: +SKIP
         '#fcd700'
 
-        shortened team names, included sponsors and typos can be dealt with
-        too (within reason)
+        # shortened team names, included sponsors and typos can be dealt with
+        # too (within reason)
 
-        >>> team_color('Mercedes')
+        >>> team_color('Mercedes')  # doctest: +SKIP
         '#00d2be'
-        >>> team_color('Merc')
+        >>> team_color('Merc')  # doctest: +SKIP
         '#00d2be'
-        >>> team_color('Merecds')
+        >>> team_color('Merecds')  # doctest: +SKIP
         '#00d2be'
-        >>> team_color('Mercedes-AMG Petronas F1 Team')
+        >>> team_color('Mercedes-AMG Petronas F1 Team')  # doctest: +SKIP
         '#00d2be'
 
     Args:
         identifier (str): Abbreviation or uniquely identifying name of the
             team.
 
     Returns:
         str: hex color code
     """
-    if identifier.upper() in TEAM_TRANSLATE:
+    warnings.warn("The function `team_color` is deprecated and will be "
+                  "removed in a future version. Use "
+                  "`fastf1.plotting.get_team_color` instead.",
+                  FutureWarning)
+
+    if identifier.upper() in LEGACY_TEAM_TRANSLATE:
         # try short team abbreviations first
-        return TEAM_COLORS[TEAM_TRANSLATE[identifier.upper()]]
+        return LEGACY_TEAM_COLORS[LEGACY_TEAM_TRANSLATE[identifier.upper()]]
     else:
         identifier = identifier.lower()
         # remove common non-unique words
         for word in ('racing', 'team', 'f1', 'scuderia'):
             identifier = identifier.replace(word, "")
 
         # check for an exact team name match
-        if identifier in TEAM_COLORS:
-            return TEAM_COLORS[identifier]
+        if identifier in LEGACY_TEAM_COLORS:
+            return LEGACY_TEAM_COLORS[identifier]
 
         # check for exact partial string match
-        for team_name, color in TEAM_COLORS.items():
+        for team_name, color in LEGACY_TEAM_COLORS.items():
             if identifier in team_name:
                 return color
 
         # do fuzzy string matching
         key_ratios = list()
-        for existing_key in TEAM_COLORS.keys():
+        for existing_key in LEGACY_TEAM_COLORS.keys():
             ratio = fuzz.ratio(identifier, existing_key)
             key_ratios.append((ratio, existing_key))
         key_ratios.sort(reverse=True)
+        if key_ratios[0][0] != 100:
+            _logger.warning(
+                ("Correcting invalid user input "
+                 f"'{identifier}' to '{key_ratios[0][1]}'."
+                 )
+            )
         if ((key_ratios[0][0] < 35)
                 or (key_ratios[0][0] / key_ratios[1][0] < 1.2)):
             # ensure that the best match has a minimum accuracy (35 out of
             # 100) and that it has a minimum confidence (at least 20% better
             # than second best)
             raise KeyError
         best_matched_key = key_ratios[0][1]
-        return TEAM_COLORS[best_matched_key]
-
-
-def lapnumber_axis(ax, axis='xaxis'):
-    """Set axis to integer ticks only."
-
-    Args:
-        ax: matplotlib axis
-        axis: can be 'xaxis' or 'yaxis'
-
-    Returns:
-        the modified axis instance
-
-    """
-    getattr(ax, axis).get_major_locator().set_params(integer=True,
-                                                     min_n_ticks=0)
-
-    return ax
+        return LEGACY_TEAM_COLORS[best_matched_key]
 
 
 def _enable_timple():
     # use external package timple to patch matplotlib
     # this adds converters, locators and formatters for
     # plotting timedelta values
     tick_formats = [
@@ -483,13 +374,37 @@
     plt.rcParams['axes.titlesize'] = 'x-large'
     # plt.rcParams['font.family'] = 'Gravity'
     plt.rcParams['font.weight'] = 'medium'
     plt.rcParams['text.color'] = '#F1F1F3'
     plt.rcParams['axes.titlesize'] = '19'
     plt.rcParams['axes.titlepad'] = '12'
     plt.rcParams['axes.titleweight'] = 'light'
-    plt.rcParams['axes.prop_cycle'] = cycler('color', COLOR_PALETTE)
+    plt.rcParams['axes.prop_cycle'] = cycler('color', _COLOR_PALETTE)
     plt.rcParams['legend.fancybox'] = False
     plt.rcParams['legend.facecolor'] = (0.1, 0.1, 0.1, 0.7)
     plt.rcParams['legend.edgecolor'] = (0.1, 0.1, 0.1, 0.9)
     plt.rcParams['savefig.transparent'] = False
     plt.rcParams['axes.axisbelow'] = True
+
+
+def lapnumber_axis(ax, axis='xaxis'):
+    """
+    Set axis to integer ticks only.
+
+    .. deprecated:: 3.4.0
+        The function ``lapnumber_axis`` is deprecated and will ber removed in a
+        future version without replacement.
+
+    Args:
+        ax: matplotlib axis
+        axis: can be 'xaxis' or 'yaxis'
+
+    Returns:
+        the modified axis instance
+    """
+    warnings.warn("The function `lapnumber_axis` is deprecated and will be "
+                  "removed without replacement in a future version.",
+                  FutureWarning)
+    getattr(ax, axis).get_major_locator().set_params(integer=True,
+                                                     min_n_ticks=0)
+
+    return ax
```

### Comparing `fastf1-3.3.7/fastf1/req.py` & `fastf1-3.4.0a0/fastf1/req.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,15 @@
 
     Cached data can be deleted at any time to reclaim disk space. However,
     this also means you will have to redownload the same data again if you
     need which will lead to reduced performance.
     """
     _CACHE_DIR = None
     # version of the api parser code (unrelated to release version number)
-    _API_CORE_VERSION = 13
+    _API_CORE_VERSION = 12
     _IGNORE_VERSION = False
     _FORCE_RENEW = False
 
     _requests_session_cached: Optional[_CachedSessionWithRateLimiting] = None
     _requests_session: requests.Session = _SessionWithRateLimiting()
     _default_cache_enabled = False  # flag to ensure that warning about disabled cache is logged once only # noqa: E501
     _tmp_disabled = False
```

### Comparing `fastf1-3.3.7/fastf1/utils.py` & `fastf1-3.4.0a0/fastf1/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,31 +46,31 @@
         :include-source:
 
         import fastf1 as ff1
         from fastf1 import plotting
         from fastf1 import utils
         from matplotlib import pyplot as plt
 
-        plotting.setup_mpl()
+        plotting.setup_mpl(misc_mpl_mods=False, color_scheme='fastf1')
 
         session = ff1.get_session(2021, 'Emilia Romagna', 'Q')
         session.load()
         lec = session.laps.pick_driver('LEC').pick_fastest()
         ham = session.laps.pick_driver('HAM').pick_fastest()
 
         delta_time, ref_tel, compare_tel = utils.delta_time(ham, lec)
         # ham is reference, lec is compared
 
         fig, ax = plt.subplots()
         # use telemetry returned by .delta_time for best accuracy,
-        # this ensure the same applied interpolation and resampling
+        # this ensures the same applied interpolation and resampling
         ax.plot(ref_tel['Distance'], ref_tel['Speed'],
-                color=plotting.team_color(ham['Team']))
+                color=plotting.get_team_color(ham['Team'], session))
         ax.plot(compare_tel['Distance'], compare_tel['Speed'],
-                color=plotting.team_color(lec['Team']))
+                color=plotting.get_team_color(lec['Team'], session))
 
         twin = ax.twinx()
         twin.plot(ref_tel['Distance'], delta_time, '--', color='white')
         twin.set_ylabel("<-- Lec ahead | Ham ahead -->")
         plt.show()
 
     Args:
```

### Comparing `fastf1-3.3.7/fastf1/ergast/interface.py` & `fastf1-3.4.0a0/fastf1/ergast/interface.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.7/fastf1/ergast/legacy.py` & `fastf1-3.4.0a0/fastf1/ergast/legacy.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.7/fastf1/ergast/sphinx.py` & `fastf1-3.4.0a0/fastf1/ergast/sphinx.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.7/fastf1/ergast/structure.py` & `fastf1-3.4.0a0/fastf1/ergast/structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
     Transform to ::
 
         {'value' : [1, 2, 3, 4, 5, 6, ...], ...},
     """
     if len(data) <= 1:
         return data[0]
 
-    for i in range(len(data) - 1):
+    for _ in range(len(data) - 1):
         _tmp = data.pop(1)
         for key in data[0].keys():
             data[0][key].extend(_tmp.pop(key))
 
     return data[0]
```

### Comparing `fastf1-3.3.7/fastf1/internals/pandas_base.py` & `fastf1-3.4.0a0/fastf1/internals/pandas_base.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.7/fastf1/internals/pandas_extensions.py` & `fastf1-3.4.0a0/fastf1/internals/pandas_extensions.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.7/fastf1/livetiming/__init__.py` & `fastf1-3.4.0a0/fastf1/livetiming/__init__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.7/fastf1/livetiming/__main__.py` & `fastf1-3.4.0a0/fastf1/livetiming/__main__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.7/fastf1/livetiming/client.py` & `fastf1-3.4.0a0/fastf1/livetiming/client.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.7/fastf1/livetiming/data.py` & `fastf1-3.4.0a0/fastf1/livetiming/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,18 +159,18 @@
         if cat not in self.data:
             self.data[cat] = [entry, ]
         else:
             self.data[cat].append(entry)
 
     def _parse_session_data(self, msg):
         # make sure the categories exist as we want to append to them
-        if 'TrackStatus' not in self.data.keys():
+        if 'TrackStatus' not in self.data:
             self.data['TrackStatus'] = {'Time': [], 'Status': [],
                                         'Message': []}
-        if 'SessionStatus' not in self.data.keys():
+        if 'SessionStatus' not in self.data:
             self.data['SessionStatus'] = {'Time': [], 'Status': []}
 
         if ('StatusSeries' in msg) and isinstance(msg['StatusSeries'], dict):
             for entry in msg['StatusSeries'].values():
                 # convert timestamp to timedelta
                 try:
                     status_dt = to_datetime(entry['Utc'])
@@ -190,15 +190,15 @@
                     self.data['TrackStatus']['Message'].append("")
 
                 elif 'SessionStatus' in entry.keys():
                     self.data['SessionStatus']['Time'].append(status_timedelta)
                     self.data['SessionStatus']['Status'].append(entry['SessionStatus'])
 
     def _parse_race_control_message(self, msg):
-        if 'RaceControlMessages' not in self.data.keys():
+        if 'RaceControlMessages' not in self.data:
             self.data['RaceControlMessages'] = {
                 'Utc': [], 'Category': [], 'Message': [], 'Status': [],
                 'Flag': [], 'Scope': [], 'Sector': [], 'RacingNumber': []
             }
 
         if ('Messages' in msg) and isinstance(msg['Messages'], dict):
             for data in msg['Messages'].values():
```

### Comparing `fastf1-3.3.7/fastf1/mvapi/api.py` & `fastf1-3.4.0a0/fastf1/mvapi/api.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.7/fastf1/mvapi/data.py` & `fastf1-3.4.0a0/fastf1/mvapi/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,16 +131,15 @@
     if not data:
         _logger.warning("Failed to load circuit info")
         return None
 
     ret = list()
     for cat in ('corners', 'marshalLights', 'marshalSectors'):
         rows = list()
-        array = data.get(cat) or list()
-        for entry in array:
+        for entry in data[cat]:
             rows.append((
                 float(entry.get('trackPosition', {}).get('x', 0.0)),
                 float(entry.get('trackPosition', {}).get('y', 0.0)),
                 int(entry.get('number', 0)),
                 str(entry.get('letter', "")),
                 float(entry.get('angle', 0.0)),
                 np.nan
```

### Comparing `fastf1-3.3.7/fastf1/signalr_aio/LICENSE` & `fastf1-3.4.0a0/fastf1/signalr_aio/LICENSE`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.7/fastf1/signalr_aio/_connection.py` & `fastf1-3.4.0a0/fastf1/signalr_aio/_connection.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.7/fastf1/signalr_aio/hubs/_hub.py` & `fastf1-3.4.0a0/fastf1/signalr_aio/hubs/_hub.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.7/fastf1/signalr_aio/transports/_parameters.py` & `fastf1-3.4.0a0/fastf1/signalr_aio/transports/_parameters.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.7/fastf1/signalr_aio/transports/_transport.py` & `fastf1-3.4.0a0/fastf1/signalr_aio/transports/_transport.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.7/.gitignore` & `fastf1-3.4.0a0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # temporary testrun directories
 fastf1/tests/testenv/
 fastf1/tests/mpl-results/
 fastf1/tests/mpl-baseline-new/
 
 # documentation build directories
 docs/_build/
-docs/examples_gallery/
+docs/gen_modules/
 **/sg_execution_times.rst
 
 # all variations of cache directories
 *_cache/
 .DS_Store
 
 # other data directories
```

### Comparing `fastf1-3.3.7/LICENSE` & `fastf1-3.4.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.7/README.md` & `fastf1-3.4.0a0/README.md`

 * *Files identical despite different names*

### Comparing `fastf1-3.3.7/pyproject.toml` & `fastf1-3.4.0a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   "matplotlib>=3.5.1,<4.0.0",
   "numpy>=1.21.5,<2.0.0",
   "pandas>=1.4.1,<3.0.0",
   "python-dateutil",
   "requests>=2.28.1",
   "requests-cache>=1.0.0",
   "scipy>=1.7.3,<2.0.0",
-  "thefuzz",
+  "rapidfuzz",
   "timple>=0.1.6",
   "websockets>=10.3",
 ]
 
 [project.urls]
 "Source Code" = "https://github.com/theOehrly/Fast-F1"
 "Documentation" = "https://docs.fastf1.dev"
```

### Comparing `fastf1-3.3.7/PKG-INFO` & `fastf1-3.4.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fastf1
-Version: 3.3.7
+Version: 3.4.0a0
 Summary: Python package for accessing and analyzing Formula 1 results, schedules, timing data and telemetry.
 Project-URL: Source Code, https://github.com/theOehrly/Fast-F1
 Project-URL: Documentation, https://docs.fastf1.dev
 Author: Philipp Schaefer
 Author-email: oehrly@mailbox.org
 License: MIT License
         
@@ -29,18 +29,18 @@
         SOFTWARE.
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: matplotlib<4.0.0,>=3.5.1
 Requires-Dist: numpy<2.0.0,>=1.21.5
 Requires-Dist: pandas<3.0.0,>=1.4.1
 Requires-Dist: python-dateutil
+Requires-Dist: rapidfuzz
 Requires-Dist: requests-cache>=1.0.0
 Requires-Dist: requests>=2.28.1
 Requires-Dist: scipy<2.0.0,>=1.7.3
-Requires-Dist: thefuzz
 Requires-Dist: timple>=0.1.6
 Requires-Dist: websockets>=10.3
 Description-Content-Type: text/markdown
 
 # FastF1
 
 FastF1 is a python package for accessing and analyzing Formula 1 results,
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: fastf1 Version: 3.3.7 Summary: Python package for
+Metadata-Version: 2.3 Name: fastf1 Version: 3.4.0a0 Summary: Python package for
 accessing and analyzing Formula 1 results, schedules, timing data and
 telemetry. Project-URL: Source Code, https://github.com/theOehrly/Fast-F1
 Project-URL: Documentation, https://docs.fastf1.dev Author: Philipp Schaefer
 Author-email: oehrly@mailbox.org License: MIT License Copyright (c) 2024
 Philipp SchÃ¤fer Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
@@ -15,18 +15,18 @@
 LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
 AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
 CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. License-File: LICENSE
 Requires-Python: >=3.8 Requires-Dist: matplotlib<4.0.0,>=3.5.1 Requires-Dist:
 numpy<2.0.0,>=1.21.5 Requires-Dist: pandas<3.0.0,>=1.4.1 Requires-Dist: python-
-dateutil Requires-Dist: requests-cache>=1.0.0 Requires-Dist: requests>=2.28.1
-Requires-Dist: scipy<2.0.0,>=1.7.3 Requires-Dist: thefuzz Requires-Dist:
-timple>=0.1.6 Requires-Dist: websockets>=10.3 Description-Content-Type: text/
-markdown # FastF1 FastF1 is a python package for accessing and analyzing
+dateutil Requires-Dist: rapidfuzz Requires-Dist: requests-cache>=1.0.0
+Requires-Dist: requests>=2.28.1 Requires-Dist: scipy<2.0.0,>=1.7.3 Requires-
+Dist: timple>=0.1.6 Requires-Dist: websockets>=10.3 Description-Content-Type:
+text/markdown # FastF1 FastF1 is a python package for accessing and analyzing
 Formula 1 results, schedules, timing data and telemetry. ![](docs/_static/
 readme.png "banner") ## Main Features - Access to F1 timing data, telemetry,
 sessions results and more - Full support for [Ergast](http://ergast.com/mrd/
 ) to access current and historical F1 data - All data is provided in the form
 of extended Pandas DataFrames to make working with the data easy while having
 powerful tools available - Adds custom functions to the Pandas objects
 specifically to make working with F1 data quick and simple - Integration with
```

