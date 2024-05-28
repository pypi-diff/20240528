# Comparing `tmp/sounderpy-3.0.4.dev1.tar.gz` & `tmp/sounderpy-3.0.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sounderpy-3.0.4.dev1.tar", last modified: Sun May 26 11:06:33 2024, max compression
+gzip compressed data, was "sounderpy-3.0.4.dev2.tar", last modified: Tue May 28 14:14:28 2024, max compression
```

## Comparing `sounderpy-3.0.4.dev1.tar` & `sounderpy-3.0.4.dev2.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 11:06:33.166935 sounderpy-3.0.4.dev1/
--rw-rw-rw-   0        0        0     1094 2024-01-08 16:49:48.000000 sounderpy-3.0.4.dev1/LICENSE
--rw-rw-rw-   0        0        0    11192 2024-05-26 11:06:33.160955 sounderpy-3.0.4.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     9759 2024-05-26 00:48:06.000000 sounderpy-3.0.4.dev1/README.md
--rw-rw-rw-   0        0        0     1379 2024-05-26 10:51:07.000000 sounderpy-3.0.4.dev1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-26 11:06:33.167936 sounderpy-3.0.4.dev1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-26 11:06:32.362280 sounderpy-3.0.4.dev1/src/
-drwxrwxrwx   0        0        0        0 2024-05-26 11:06:32.418120 sounderpy-3.0.4.dev1/src/sounderpy/
-drwxrwxrwx   0        0        0        0 2024-05-26 11:06:32.451235 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/
--rw-rw-rw-   0        0        0       64 2023-06-15 13:50:54.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 11:06:32.462223 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/ci/
--rw-rw-rw-   0        0        0      439 2023-06-15 13:09:41.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/ci/check_artifact_dir.py
--rw-rw-rw-   0        0        0      337 2023-06-15 13:09:41.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/ci/screen.py
-drwxrwxrwx   0        0        0        0 2024-05-26 11:06:32.487212 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/datasources/
--rw-rw-rw-   0        0        0       41 2023-06-15 13:09:41.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/datasources/__init__.py
--rw-rw-rw-   0        0        0    22995 2023-06-15 13:09:42.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/datasources/available.py
--rw-rw-rw-   0        0        0    19870 2023-06-15 13:09:42.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/datasources/data_source.py
-drwxrwxrwx   0        0        0        0 2024-05-26 11:06:32.371672 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/
-drwxrwxrwx   0        0        0        0 2024-05-26 11:06:32.496533 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/io/
--rw-rw-rw-   0        0        0      115 2023-06-15 13:11:47.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/io/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 11:06:32.508751 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/plot/
--rw-rw-rw-   0        0        0       20 2023-06-15 13:11:48.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/plot/__init__.py
--rw-rw-rw-   0        0        0    13958 2023-12-20 17:12:24.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/plot/skew.py
-drwxrwxrwx   0        0        0        0 2024-05-26 11:06:32.708731 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/
--rw-rw-rw-   0        0        0       52 2023-06-15 13:35:03.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/__init__.py
--rw-rw-rw-   0        0        0     2524 2023-06-15 13:09:48.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/_sharppy_version.py
--rw-rw-rw-   0        0        0    18524 2023-06-15 13:09:48.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/_version.py
--rw-rw-rw-   0        0        0      891 2023-06-15 13:11:48.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/constants.py
--rw-rw-rw-   0        0        0     1054 2023-06-15 13:35:09.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/csv.py
--rw-rw-rw-   0        0        0     3433 2023-12-20 17:04:47.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/decoder.py
--rw-rw-rw-   0        0        0     7972 2023-12-20 17:09:41.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/fire.py
--rw-rw-rw-   0        0        0     3890 2023-12-20 17:12:22.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/gui.py
--rw-rw-rw-   0        0        0    12670 2023-12-20 17:09:40.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/interp.py
--rw-rw-rw-   0        0        0   120008 2024-01-01 01:57:39.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/params.py
--rw-rw-rw-   0        0        0    16042 2023-12-20 17:09:38.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/prof_collection.py
--rw-rw-rw-   0        0        0    49972 2023-12-20 16:52:49.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/profile.py
--rw-rw-rw-   0        0        0     8133 2023-12-20 17:09:36.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/pwv.py
--rw-rw-rw-   0        0        0     5849 2023-12-20 18:02:55.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/qc_tools.py
--rw-rw-rw-   0        0        0    17031 2023-06-15 13:35:02.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sars.py
--rw-rw-rw-   0        0        0     6846 2023-12-20 17:09:34.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sars_cal.py
--rw-rw-rw-   0        0        0    13328 2023-12-20 17:09:33.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sounding.py
--rw-rw-rw-   0        0        0    14047 2023-12-20 17:09:33.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/thermo.py
--rw-rw-rw-   0        0        0     8649 2023-12-20 17:09:32.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/utils.py
--rw-rw-rw-   0        0        0    22092 2023-12-20 17:09:32.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/watch_type.py
--rw-rw-rw-   0        0        0    16016 2023-12-20 17:22:10.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/winds.py
-drwxrwxrwx   0        0        0        0 2024-05-26 11:06:32.843838 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/
--rw-rw-rw-   0        0        0      925 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_binary.py
--rw-rw-rw-   0        0        0     2280 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_decoders.py
--rw-rw-rw-   0        0        0     4008 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_gui.py
--rw-rw-rw-   0        0        0     4168 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_interp.py
--rw-rw-rw-   0        0        0     1205 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_misc.py
--rw-rw-rw-   0        0        0     3896 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_params.py
--rw-rw-rw-   0        0        0     3532 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_plotting.py
--rw-rw-rw-   0        0        0    10918 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_profile.py
--rw-rw-rw-   0        0        0      529 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_sars.py
--rw-rw-rw-   0        0        0    13676 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_thermo.py
--rw-rw-rw-   0        0        0     1296 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_url.py
--rw-rw-rw-   0        0        0     9568 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_utils.py
--rw-rw-rw-   0        0        0     3558 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_winds.py
-drwxrwxrwx   0        0        0        0 2024-05-26 11:06:33.073306 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/
--rw-rw-rw-   0        0        0    40265 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/SPCWindow.py
--rw-rw-rw-   0        0        0      938 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/__init__.py
--rw-rw-rw-   0        0        0     7734 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/advection.py
--rw-rw-rw-   0        0        0    21293 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/analogues.py
--rw-rw-rw-   0        0        0     5589 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/barbs.py
--rw-rw-rw-   0        0        0     9080 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/draggable.py
--rw-rw-rw-   0        0        0    12439 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/ensemble.py
--rw-rw-rw-   0        0        0    15829 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/fire.py
--rw-rw-rw-   0        0        0    12108 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/generic.py
--rw-rw-rw-   0        0        0    52153 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/hodo.py
--rw-rw-rw-   0        0        0    23498 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/kinematics.py
--rw-rw-rw-   0        0        0    34524 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/map.py
--rw-rw-rw-   0        0        0    19031 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/preferences.py
--rw-rw-rw-   0        0        0    10173 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/ship.py
--rw-rw-rw-   0        0        0    65020 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/skew.py
--rw-rw-rw-   0        0        0    11895 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/slinky.py
--rw-rw-rw-   0        0        0    10152 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/speed.py
--rw-rw-rw-   0        0        0    15699 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/srwinds.py
--rw-rw-rw-   0        0        0    21968 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/stp.py
--rw-rw-rw-   0        0        0    11938 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/stpef.py
--rw-rw-rw-   0        0        0    32304 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/thermo.py
--rw-rw-rw-   0        0        0    10140 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/thetae.py
--rw-rw-rw-   0        0        0    12890 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/vrot.py
--rw-rw-rw-   0        0        0     7759 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/watch.py
--rw-rw-rw-   0        0        0    14588 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/winter.py
-drwxrwxrwx   0        0        0        0 2024-05-26 11:06:33.142500 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/
--rw-rw-rw-   0        0        0       65 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/__init__.py
--rw-rw-rw-   0        0        0     4236 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/async.py
--rw-rw-rw-   0        0        0     4147 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/async_threads.py
--rw-rw-rw-   0        0        0     2512 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/config.py
--rw-rw-rw-   0        0        0     1660 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/frozenutils.py
--rw-rw-rw-   0        0        0     1933 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/progress.py
--rw-rw-rw-   0        0        0      156 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/utils.py
--rw-rw-rw-   0        0        0     1329 2023-12-20 17:14:06.000000 sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/ver_updates.py
--rw-rw-rw-   0        0        0      743 2024-03-17 22:48:51.000000 sounderpy-3.0.4.dev1/src/sounderpy/__init__.py
--rw-rw-rw-   0        0        0    44655 2024-05-26 10:51:15.000000 sounderpy-3.0.4.dev1/src/sounderpy/calc.py
--rw-rw-rw-   0        0        0   193583 2024-05-26 11:04:56.000000 sounderpy-3.0.4.dev1/src/sounderpy/plot.py
--rw-rw-rw-   0        0        0    97993 2024-05-26 01:49:30.000000 sounderpy-3.0.4.dev1/src/sounderpy/sounderpy.py
-drwxrwxrwx   0        0        0        0 2024-05-26 11:06:33.149478 sounderpy-3.0.4.dev1/src/sounderpy.egg-info/
--rw-rw-rw-   0        0        0    11192 2024-05-26 11:06:32.000000 sounderpy-3.0.4.dev1/src/sounderpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4156 2024-05-26 11:06:32.000000 sounderpy-3.0.4.dev1/src/sounderpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 11:06:32.000000 sounderpy-3.0.4.dev1/src/sounderpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      167 2024-05-26 11:06:32.000000 sounderpy-3.0.4.dev1/src/sounderpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-26 11:06:32.000000 sounderpy-3.0.4.dev1/src/sounderpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 14:14:28.065001 sounderpy-3.0.4.dev2/
+-rw-rw-rw-   0        0        0     1094 2024-01-08 16:49:48.000000 sounderpy-3.0.4.dev2/LICENSE
+-rw-rw-rw-   0        0        0    11192 2024-05-28 14:14:28.054552 sounderpy-3.0.4.dev2/PKG-INFO
+-rw-rw-rw-   0        0        0     9759 2024-05-28 14:13:35.000000 sounderpy-3.0.4.dev2/README.md
+-rw-rw-rw-   0        0        0     1379 2024-05-28 14:13:36.000000 sounderpy-3.0.4.dev2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-28 14:14:28.066234 sounderpy-3.0.4.dev2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-28 14:14:27.123592 sounderpy-3.0.4.dev2/src/
+drwxrwxrwx   0        0        0        0 2024-05-28 14:14:27.188158 sounderpy-3.0.4.dev2/src/sounderpy/
+drwxrwxrwx   0        0        0        0 2024-05-28 14:14:27.240371 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/
+-rw-rw-rw-   0        0        0       64 2023-06-15 13:50:54.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:14:27.254929 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/ci/
+-rw-rw-rw-   0        0        0      439 2023-06-15 13:09:41.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/ci/check_artifact_dir.py
+-rw-rw-rw-   0        0        0      337 2023-06-15 13:09:41.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/ci/screen.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:14:27.281827 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/datasources/
+-rw-rw-rw-   0        0        0       41 2023-06-15 13:09:41.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/datasources/__init__.py
+-rw-rw-rw-   0        0        0    22995 2023-06-15 13:09:42.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/datasources/available.py
+-rw-rw-rw-   0        0        0    19870 2023-06-15 13:09:42.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/datasources/data_source.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:14:27.138060 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/
+drwxrwxrwx   0        0        0        0 2024-05-28 14:14:27.291702 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/io/
+-rw-rw-rw-   0        0        0      115 2023-06-15 13:11:47.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/io/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:14:27.304426 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/plot/
+-rw-rw-rw-   0        0        0       20 2023-06-15 13:11:48.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/plot/__init__.py
+-rw-rw-rw-   0        0        0    13958 2023-12-20 17:12:24.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/plot/skew.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:14:27.502780 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/
+-rw-rw-rw-   0        0        0       52 2023-06-15 13:35:03.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/__init__.py
+-rw-rw-rw-   0        0        0     2524 2023-06-15 13:09:48.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/_sharppy_version.py
+-rw-rw-rw-   0        0        0    18524 2023-06-15 13:09:48.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/_version.py
+-rw-rw-rw-   0        0        0      891 2023-06-15 13:11:48.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/constants.py
+-rw-rw-rw-   0        0        0     1054 2023-06-15 13:35:09.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/csv.py
+-rw-rw-rw-   0        0        0     3433 2023-12-20 17:04:47.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/decoder.py
+-rw-rw-rw-   0        0        0     7972 2023-12-20 17:09:41.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/fire.py
+-rw-rw-rw-   0        0        0     3890 2023-12-20 17:12:22.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/gui.py
+-rw-rw-rw-   0        0        0    12670 2023-12-20 17:09:40.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/interp.py
+-rw-rw-rw-   0        0        0   120008 2024-01-01 01:57:39.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/params.py
+-rw-rw-rw-   0        0        0    16042 2023-12-20 17:09:38.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/prof_collection.py
+-rw-rw-rw-   0        0        0    49972 2023-12-20 16:52:49.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/profile.py
+-rw-rw-rw-   0        0        0     8133 2023-12-20 17:09:36.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/pwv.py
+-rw-rw-rw-   0        0        0     5849 2023-12-20 18:02:55.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/qc_tools.py
+-rw-rw-rw-   0        0        0    17031 2023-06-15 13:35:02.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sars.py
+-rw-rw-rw-   0        0        0     6846 2023-12-20 17:09:34.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sars_cal.py
+-rw-rw-rw-   0        0        0    13328 2023-12-20 17:09:33.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sounding.py
+-rw-rw-rw-   0        0        0    14047 2023-12-20 17:09:33.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/thermo.py
+-rw-rw-rw-   0        0        0     8649 2023-12-20 17:09:32.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/utils.py
+-rw-rw-rw-   0        0        0    22092 2023-12-20 17:09:32.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/watch_type.py
+-rw-rw-rw-   0        0        0    16016 2023-12-20 17:22:10.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/winds.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:14:27.656453 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/
+-rw-rw-rw-   0        0        0      925 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_binary.py
+-rw-rw-rw-   0        0        0     2280 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_decoders.py
+-rw-rw-rw-   0        0        0     4008 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_gui.py
+-rw-rw-rw-   0        0        0     4168 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_interp.py
+-rw-rw-rw-   0        0        0     1205 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_misc.py
+-rw-rw-rw-   0        0        0     3896 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_params.py
+-rw-rw-rw-   0        0        0     3532 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_plotting.py
+-rw-rw-rw-   0        0        0    10918 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_profile.py
+-rw-rw-rw-   0        0        0      529 2023-06-15 13:11:49.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_sars.py
+-rw-rw-rw-   0        0        0    13676 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_thermo.py
+-rw-rw-rw-   0        0        0     1296 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_url.py
+-rw-rw-rw-   0        0        0     9568 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_utils.py
+-rw-rw-rw-   0        0        0     3558 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_winds.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:14:27.961491 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/
+-rw-rw-rw-   0        0        0    40265 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/SPCWindow.py
+-rw-rw-rw-   0        0        0      938 2023-06-15 13:11:50.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/__init__.py
+-rw-rw-rw-   0        0        0     7734 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/advection.py
+-rw-rw-rw-   0        0        0    21293 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/analogues.py
+-rw-rw-rw-   0        0        0     5589 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/barbs.py
+-rw-rw-rw-   0        0        0     9080 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/draggable.py
+-rw-rw-rw-   0        0        0    12439 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/ensemble.py
+-rw-rw-rw-   0        0        0    15829 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/fire.py
+-rw-rw-rw-   0        0        0    12108 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/generic.py
+-rw-rw-rw-   0        0        0    52153 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/hodo.py
+-rw-rw-rw-   0        0        0    23498 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/kinematics.py
+-rw-rw-rw-   0        0        0    34524 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/map.py
+-rw-rw-rw-   0        0        0    19031 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/preferences.py
+-rw-rw-rw-   0        0        0    10173 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/ship.py
+-rw-rw-rw-   0        0        0    65020 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/skew.py
+-rw-rw-rw-   0        0        0    11895 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/slinky.py
+-rw-rw-rw-   0        0        0    10152 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/speed.py
+-rw-rw-rw-   0        0        0    15699 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/srwinds.py
+-rw-rw-rw-   0        0        0    21968 2023-06-15 13:11:51.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/stp.py
+-rw-rw-rw-   0        0        0    11938 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/stpef.py
+-rw-rw-rw-   0        0        0    32304 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/thermo.py
+-rw-rw-rw-   0        0        0    10140 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/thetae.py
+-rw-rw-rw-   0        0        0    12890 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/vrot.py
+-rw-rw-rw-   0        0        0     7759 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/watch.py
+-rw-rw-rw-   0        0        0    14588 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/winter.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:14:28.034463 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sutils/
+-rw-rw-rw-   0        0        0       65 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sutils/__init__.py
+-rw-rw-rw-   0        0        0     4236 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sutils/async.py
+-rw-rw-rw-   0        0        0     4147 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sutils/async_threads.py
+-rw-rw-rw-   0        0        0     2512 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sutils/config.py
+-rw-rw-rw-   0        0        0     1660 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sutils/frozenutils.py
+-rw-rw-rw-   0        0        0     1933 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sutils/progress.py
+-rw-rw-rw-   0        0        0      156 2023-06-15 13:11:52.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sutils/utils.py
+-rw-rw-rw-   0        0        0     1329 2023-12-20 17:14:06.000000 sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sutils/ver_updates.py
+-rw-rw-rw-   0        0        0      743 2024-03-17 22:48:51.000000 sounderpy-3.0.4.dev2/src/sounderpy/__init__.py
+-rw-rw-rw-   0        0        0    44655 2024-05-26 10:51:15.000000 sounderpy-3.0.4.dev2/src/sounderpy/calc.py
+-rw-rw-rw-   0        0        0   193634 2024-05-28 14:13:39.000000 sounderpy-3.0.4.dev2/src/sounderpy/plot.py
+-rw-rw-rw-   0        0        0    97993 2024-05-28 14:13:37.000000 sounderpy-3.0.4.dev2/src/sounderpy/sounderpy.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:14:28.042917 sounderpy-3.0.4.dev2/src/sounderpy.egg-info/
+-rw-rw-rw-   0        0        0    11192 2024-05-28 14:14:26.000000 sounderpy-3.0.4.dev2/src/sounderpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4156 2024-05-28 14:14:27.000000 sounderpy-3.0.4.dev2/src/sounderpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 14:14:27.000000 sounderpy-3.0.4.dev2/src/sounderpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      167 2024-05-28 14:14:27.000000 sounderpy-3.0.4.dev2/src/sounderpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-28 14:14:27.000000 sounderpy-3.0.4.dev2/src/sounderpy.egg-info/top_level.txt
```

### Comparing `sounderpy-3.0.4.dev1/LICENSE` & `sounderpy-3.0.4.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/PKG-INFO` & `sounderpy-3.0.4.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sounderpy
-Version: 3.0.4.dev1
+Version: 3.0.4.dev2
 Summary: Vertical Profile Data Retrieval and Analysis Tool For Python
 Author-email: "Kyle J Gillett, University of North Dakota" <kjgillett10@gmail.com>
 Project-URL: Docs, https://kylejgillett.github.io/sounderpy/
 Project-URL: Code, https://github.com/kylejgillett/sounderpy
 Project-URL: Operational Site, https://sounderpysoundings.anvil.app/
 Project-URL: PyPi, https://pypi.org/project/sounderpy/
 Project-URL: My Website, https://kylegillettphoto.com
```

### Comparing `sounderpy-3.0.4.dev1/README.md` & `sounderpy-3.0.4.dev2/README.md`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/pyproject.toml` & `sounderpy-3.0.4.dev2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sounderpy"
-version = "3.0.4dev1"
+version = "3.0.4dev2"
 authors = [
   { name="Kyle J Gillett, University of North Dakota", email="kjgillett10@gmail.com" },
 ]
 description = "Vertical Profile Data Retrieval and Analysis Tool For Python"
 readme = "README.md"
 keywords = ["meteorology", "science", "data-analysis", "weather", "forecasting"]
 requires-python = ">=3.1"
```

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/datasources/available.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/datasources/available.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/datasources/data_source.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/datasources/data_source.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/plot/skew.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/plot/skew.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/_sharppy_version.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/_sharppy_version.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/_version.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/_version.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/constants.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/constants.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/csv.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/csv.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/decoder.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/decoder.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/fire.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/fire.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/gui.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/gui.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/interp.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/interp.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/params.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/params.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/prof_collection.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/prof_collection.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/profile.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/profile.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/pwv.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/pwv.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/qc_tools.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/qc_tools.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sars.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sars.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sars_cal.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sars_cal.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sounding.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/sounding.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/thermo.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/thermo.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/utils.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/utils.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/watch_type.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/watch_type.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/winds.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/sharptab/winds.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_binary.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_binary.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_decoders.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_decoders.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_gui.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_interp.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_interp.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_misc.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_params.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_plotting.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_profile.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_sars.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_sars.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_thermo.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_thermo.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_url.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_utils.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_winds.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/tests/test_winds.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/SPCWindow.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/SPCWindow.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/__init__.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/__init__.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/advection.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/advection.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/analogues.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/analogues.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/barbs.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/barbs.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/draggable.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/draggable.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/ensemble.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/ensemble.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/fire.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/fire.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/generic.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/generic.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/hodo.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/hodo.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/kinematics.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/kinematics.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/map.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/map.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/preferences.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/preferences.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/ship.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/ship.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/skew.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/skew.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/slinky.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/slinky.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/speed.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/speed.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/srwinds.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/srwinds.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/stp.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/stp.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/stpef.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/stpef.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/thermo.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/thermo.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/thetae.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/thetae.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/vrot.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/vrot.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/watch.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/watch.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sharppy/viz/winter.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sharppy/viz/winter.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/async.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sutils/async.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/async_threads.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sutils/async_threads.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/config.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sutils/config.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/frozenutils.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sutils/frozenutils.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/progress.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sutils/progress.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/SHARPPYMAIN/sutils/ver_updates.py` & `sounderpy-3.0.4.dev2/src/sounderpy/SHARPPYMAIN/sutils/ver_updates.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/__init__.py` & `sounderpy-3.0.4.dev2/src/sounderpy/__init__.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/calc.py` & `sounderpy-3.0.4.dev2/src/sounderpy/calc.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/plot.py` & `sounderpy-3.0.4.dev2/src/sounderpy/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -540,15 +540,15 @@
     Td_degF_label = '{}°F'.format(int(Td_degF[0].magnitude))                             
     plt.annotate(Td_degF_label,(Td[0], p[0]),textcoords="offset points",xytext=(-16,-15), 
                      fontsize=12, color=td_color, weight='bold', alpha=0.7, ha='center') 
     
     # if the sfc was modified by the user, plot a modified sfc flag
     if modify_sfc_txt == True: 
         plt.annotate("USER MODIFIED SFC →", (Td[0], p[0]),textcoords="offset points",xytext=(-50,0), 
-                     fontsize=10, color='black', weight='bold', alpha=0.5, ha='right')
+                     fontsize=10, color=gen_txt_clr, weight='bold', alpha=0.5, ha='right')
         
         
     # PARCEL HEIGHT ANNOTATIONS------------------------------------------------------------- 
     # plot the SBLCL and draw a line between the sfc and the lcl
     plt.text((0.82), (thermo['sb_lcl_p']), "←SBLCL", weight='bold',color='gray',
              alpha=0.9, fontsize=15, transform=skew.ax.get_yaxis_transform(), clip_on=True)
     lcl_line = plt.Line2D([0.86, 0.86], (p[0], thermo['sb_lcl_p']), 
@@ -592,20 +592,20 @@
         
         
         
         
     # T & WB FRREZING POINT ANNOTATION--------------------------------------------------------------
     if ma.is_masked(general['frz_pt_z']) == False:
         if general['frz_pt_z'] >= 50*units.m:
-            plt.text((0.76), (general['frz_pt_p']), "←FRZ", weight='bold',color='cornflowerblue',  
+            plt.text((0.765), (general['frz_pt_p']), "←FRZ", weight='bold',color='cornflowerblue',  
                      alpha=0.6, fontsize=12, transform=skew.ax.get_yaxis_transform(), clip_on=True)
     
     if ma.is_masked(general['wb_frz_pt_z']) == False:
         if general['wb_frz_pt_z'] >= 50*units.m:
-            plt.text((0.76), (general['wb_frz_pt_p']), "←WB0", weight='bold',color='darkblue',  
+            plt.text((0.765), (general['wb_frz_pt_p']), "←WB0", weight='bold',color='cornflowerblue',  
                      alpha=0.6, fontsize=12, transform=skew.ax.get_yaxis_transform(), clip_on=True)
 
             
     # PBL TOP POINT ANNOTATION---------------------------------------------------------------                   
     plt.text((0.78), (thermo['pbl_top']), "←PBL", weight='bold',color='gray', 
              alpha=0.9, fontsize=10, transform=skew.ax.get_yaxis_transform(), clip_on=True)
     pbl_line = plt.Line2D([0.80, 0.80], (p[0], thermo['pbl_top']), color='gray', 
@@ -674,15 +674,15 @@
 
     try:
         for hgt_idx in hgts:
             label = "{}% →".format(int(intrp['rhINTRP'][hgt_idx]))
             plt.annotate(label, (mpcalc.dewpoint_from_relative_humidity(intrp['tINTRP'][hgt_idx]*units.degC, 
                                                                     intrp['rhINTRP'][hgt_idx]/100),
                          intrp['pINTRP'][hgt_idx]*units.hPa), textcoords="offset points", xytext=(-40, 0), 
-                         color='green', alpha=0.4, fontsize=13.5, ha='center', clip_on=True) 
+                         color='green', alpha=0.6, fontsize=13.5, ha='center', clip_on=True) 
     except:
         pass
     #################################################################
     
     
     
     
@@ -1034,14 +1034,16 @@
         map_ax.set_box_aspect(1) 
 
         map_ax.add_feature(cfeature.STATES, color=bckgrnd_clr, zorder=1)
         map_ax.add_feature(cfeature.STATES, edgecolor=gen_txt_clr, alpha=0.7, 
                        linestyle='-', linewidth=2, zorder=6)
         map_ax.add_feature(USCOUNTIES, alpha=0.3, edgecolor=gen_txt_clr, 
                            linestyle='-', linewidth=0.2, zorder=5)
+        map_ax.add_feature(cfeature.LAKES, color=bckgrnd_clr)
+        map_ax.add_feature(cfeature.OCEAN, color=bckgrnd_clr)
 
         if show_radar == True:
             # BUILD COLOR MAP -----------------------------------------------------------------------------------------------------
             radar_cmap = LinearSegmentedColormap.from_list('custom_cmap',
                         ['#B0C4DE', '#4682B4', '#90EE90', '#228B22', '#FFFF4D', '#E6E600',
                         '#FFC34D', '#E69900', '#FF4D4D', '#E60000', '#FFCCEE', '#FF198C',
                         '#D400FF', '#550080'], N=256)
@@ -1370,54 +1372,54 @@
     ### KINEMATICS ###
     #################################################################   
     met_per_sec = (units.m*units.m)/(units.sec*units.sec)
 
     plt.figtext( 0.735, 0.07, 'BS         SRH       SRW    SWζ%    SWζ', color=gen_txt_clr, weight='bold', fontsize=15, alpha=0.8)
 
     plt.figtext( 0.689, 0.04, f"0-.5ₖₘ:", weight='bold', fontsize=15, color=gen_txt_clr, alpha=0.9)
-    plt.figtext( 0.732, 0.04, f"{mag(kinem['shear_0_to_500'])} kt", fontsize=15, color='deepskyblue', weight='bold')
-    plt.figtext( 0.769, 0.04, f"{mag(kinem['srh_0_to_500'])* met_per_sec:~P}", fontsize=15, color='deepskyblue', weight='bold')
-    plt.figtext( 0.828, 0.04, f"{mag(kinem['srw_0_to_500'])} kt", fontsize=15, color='deepskyblue', weight='bold')
-    plt.figtext( 0.870, 0.04, f"{mag(kinem['swv_perc_0_to_500'])}", fontsize=15, color='deepskyblue', weight='bold')
-    plt.figtext( 0.905, 0.04, f"{mag_round(kinem['swv_0_to_500'], 3)}", fontsize=15, color='deepskyblue', weight='bold')
+    plt.figtext( 0.732, 0.04, f"{mag(kinem['shear_0_to_500'])} kt", fontsize=15, color='#6495ED', weight='bold')
+    plt.figtext( 0.769, 0.04, f"{mag(kinem['srh_0_to_500'])* met_per_sec:~P}", fontsize=15, color='#6495ED', weight='bold')
+    plt.figtext( 0.828, 0.04, f"{mag(kinem['srw_0_to_500'])} kt", fontsize=15, color='#6495ED', weight='bold')
+    plt.figtext( 0.870, 0.04, f"{mag(kinem['swv_perc_0_to_500'])}", fontsize=15, color='#6495ED', weight='bold')
+    plt.figtext( 0.905, 0.04, f"{mag_round(kinem['swv_0_to_500'], 3)}", fontsize=15, color='#6495ED', weight='bold')
 
     plt.figtext( 0.689, 0.01, f"0-1ₖₘ:", weight='bold', fontsize=15, color=gen_txt_clr, alpha=0.9)
-    plt.figtext( 0.732, 0.01, f"{mag(kinem['shear_0_to_1000'])} kt", fontsize=15, color='mediumslateblue', weight='bold')
-    plt.figtext( 0.769, 0.01, f"{mag(kinem['srh_0_to_1000'])* met_per_sec:~P}", fontsize=15, color='mediumslateblue', weight='bold')
-    plt.figtext( 0.828, 0.01, f"{mag(kinem['srw_0_to_1000'])} kt", fontsize=15, color='mediumslateblue', weight='bold')
-    plt.figtext( 0.870, 0.01, f"{mag(kinem['swv_perc_0_to_1000'])}", fontsize=15, color='mediumslateblue', weight='bold')
-    plt.figtext( 0.905, 0.01, f"{mag_round(kinem['swv_0_to_1000'], 3)}", fontsize=15, color='mediumslateblue', weight='bold')
+    plt.figtext( 0.732, 0.01, f"{mag(kinem['shear_0_to_1000'])} kt", fontsize=15, color='#7B68EE', weight='bold')
+    plt.figtext( 0.769, 0.01, f"{mag(kinem['srh_0_to_1000'])* met_per_sec:~P}", fontsize=15, color='#7B68EE', weight='bold')
+    plt.figtext( 0.828, 0.01, f"{mag(kinem['srw_0_to_1000'])} kt", fontsize=15, color='#7B68EE', weight='bold')
+    plt.figtext( 0.870, 0.01, f"{mag(kinem['swv_perc_0_to_1000'])}", fontsize=15, color='#7B68EE', weight='bold')
+    plt.figtext( 0.905, 0.01, f"{mag_round(kinem['swv_0_to_1000'], 3)}", fontsize=15, color='#7B68EE', weight='bold')
 
     plt.figtext( 0.689, -0.02, f"1-3ₖₘ:", weight='bold', fontsize=15, color=gen_txt_clr, alpha=0.9)
-    plt.figtext( 0.732, -0.02, f"{mag(kinem['shear_1_to_3000'])} kt", fontsize=15, color='slateblue', weight='bold')
-    plt.figtext( 0.769, -0.02, f"{mag(kinem['srh_1_to_3000'])* met_per_sec:~P}", fontsize=15, color='slateblue', weight='bold')
-    plt.figtext( 0.828, -0.02, f"{mag(kinem['srw_1_to_3000'])} kt", fontsize=15, color='slateblue', weight='bold')
-    plt.figtext( 0.870, -0.02, f"{mag(kinem['swv_perc_1_to_3000'])}", fontsize=15, color='slateblue', weight='bold')
-    plt.figtext( 0.905, -0.02, f"{mag_round(kinem['swv_1_to_3000'], 3)}", fontsize=15, color='slateblue', weight='bold')
+    plt.figtext( 0.732, -0.02, f"{mag(kinem['shear_1_to_3000'])} kt", fontsize=15, color='#4169E1', weight='bold')
+    plt.figtext( 0.769, -0.02, f"{mag(kinem['srh_1_to_3000'])* met_per_sec:~P}", fontsize=15, color='#4169E1', weight='bold')
+    plt.figtext( 0.828, -0.02, f"{mag(kinem['srw_1_to_3000'])} kt", fontsize=15, color='#4169E1', weight='bold')
+    plt.figtext( 0.870, -0.02, f"{mag(kinem['swv_perc_1_to_3000'])}", fontsize=15, color='#4169E1', weight='bold')
+    plt.figtext( 0.905, -0.02, f"{mag_round(kinem['swv_1_to_3000'], 3)}", fontsize=15, color='#4169E1', weight='bold')
 
     plt.figtext( 0.689, -0.05, f"3-6ₖₘ:", weight='bold', fontsize=15, color=gen_txt_clr, alpha=0.9)
-    plt.figtext( 0.732, -0.05, f"{mag(kinem['shear_3_to_6000'])} kt", fontsize=15, color='darkslateblue', weight='bold')
-    plt.figtext( 0.769, -0.05, f"{mag(kinem['srh_3_to_6000'])* met_per_sec:~P}", fontsize=15, color='darkslateblue', weight='bold')
-    plt.figtext( 0.828, -0.05, f"{mag(kinem['srw_3_to_6000'])} kt", fontsize=15, color='darkslateblue', weight='bold')
-    plt.figtext( 0.870, -0.05, f"{mag(kinem['swv_perc_3_to_6000'])}", fontsize=15, color='darkslateblue', weight='bold')
-    plt.figtext( 0.905, -0.05, f"{mag_round(kinem['swv_3_to_6000'], 3)}", fontsize=15, color='darkslateblue', weight='bold')
+    plt.figtext( 0.732, -0.05, f"{mag(kinem['shear_3_to_6000'])} kt", fontsize=15, color='#0000CD', weight='bold')
+    plt.figtext( 0.769, -0.05, f"{mag(kinem['srh_3_to_6000'])* met_per_sec:~P}", fontsize=15, color='#0000CD', weight='bold')
+    plt.figtext( 0.828, -0.05, f"{mag(kinem['srw_3_to_6000'])} kt", fontsize=15, color='#0000CD', weight='bold')
+    plt.figtext( 0.870, -0.05, f"{mag(kinem['swv_perc_3_to_6000'])}", fontsize=15, color='#0000CD', weight='bold')
+    plt.figtext( 0.905, -0.05, f"{mag_round(kinem['swv_3_to_6000'], 3)}", fontsize=15, color='#0000CD', weight='bold')
     
     plt.figtext( 0.689, -0.08, f"6-9ₖₘ:", weight='bold', fontsize=15, color=gen_txt_clr, alpha=0.9)
-    plt.figtext( 0.732, -0.08, f"{mag(kinem['shear_6_to_9000'])} kt", fontsize=15, color='navy', weight='bold')
-    plt.figtext( 0.769, -0.08, f"{mag(kinem['srh_6_to_9000'])* met_per_sec:~P}", fontsize=15, color='navy', weight='bold')
-    plt.figtext( 0.828, -0.08, f"{mag(kinem['srw_6_to_9000'])} kt", fontsize=15, color='navy', weight='bold')
-    plt.figtext( 0.870, -0.08, f"{mag(kinem['swv_perc_6_to_9000'])}", fontsize=15, color='navy', weight='bold')
-    plt.figtext( 0.905, -0.08, f"{mag_round(kinem['swv_6_to_9000'], 3)}", fontsize=15, color='navy', weight='bold')
+    plt.figtext( 0.732, -0.08, f"{mag(kinem['shear_6_to_9000'])} kt", fontsize=15, color='#00008B', weight='bold')
+    plt.figtext( 0.769, -0.08, f"{mag(kinem['srh_6_to_9000'])* met_per_sec:~P}", fontsize=15, color='#00008B', weight='bold')
+    plt.figtext( 0.828, -0.08, f"{mag(kinem['srw_6_to_9000'])} kt", fontsize=15, color='#00008B', weight='bold')
+    plt.figtext( 0.870, -0.08, f"{mag(kinem['swv_perc_6_to_9000'])}", fontsize=15, color='#00008B', weight='bold')
+    plt.figtext( 0.905, -0.08, f"{mag_round(kinem['swv_6_to_9000'], 3)}", fontsize=15, color='#00008B', weight='bold')
     
     plt.figtext( 0.689, -0.11, f"EIL:", weight='bold', fontsize=15, color=gen_txt_clr, alpha=0.9)
-    plt.figtext( 0.732, -0.11, f"{mag(kinem['shear_eil'])} kt", fontsize=15, color='magenta', weight='bold')
-    plt.figtext( 0.769, -0.11, f"{mag(kinem['srh_eil'])* met_per_sec:~P}", fontsize=15, color='magenta', weight='bold')
-    plt.figtext( 0.828, -0.11, f"{mag(kinem['srw_eil'])} kt", fontsize=15, color='magenta', weight='bold')
-    plt.figtext( 0.870, -0.11, f"{mag(kinem['swv_perc_eil'])}", fontsize=15, color='magenta', weight='bold')
-    plt.figtext( 0.905, -0.11, f"{mag_round(kinem['swv_eil'], 3)}", fontsize=15, color='magenta', weight='bold')
+    plt.figtext( 0.732, -0.11, f"{mag(kinem['shear_eil'])} kt", fontsize=15, color='#000080', weight='bold')
+    plt.figtext( 0.769, -0.11, f"{mag(kinem['srh_eil'])* met_per_sec:~P}", fontsize=15, color='#000080', weight='bold')
+    plt.figtext( 0.828, -0.11, f"{mag(kinem['srw_eil'])} kt", fontsize=15, color='#000080', weight='bold')
+    plt.figtext( 0.870, -0.11, f"{mag(kinem['swv_perc_eil'])}", fontsize=15, color='#000080', weight='bold')
+    plt.figtext( 0.905, -0.11, f"{mag_round(kinem['swv_eil'], 3)}", fontsize=15, color='#000080', weight='bold')
     #################################################################
     
     
     
     #########################################################################
     ############################# PLOT EXTRAS ############################### 
     #########################################################################
```

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy/sounderpy.py` & `sounderpy-3.0.4.dev2/src/sounderpy/sounderpy.py`

 * *Files identical despite different names*

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy.egg-info/PKG-INFO` & `sounderpy-3.0.4.dev2/src/sounderpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sounderpy
-Version: 3.0.4.dev1
+Version: 3.0.4.dev2
 Summary: Vertical Profile Data Retrieval and Analysis Tool For Python
 Author-email: "Kyle J Gillett, University of North Dakota" <kjgillett10@gmail.com>
 Project-URL: Docs, https://kylejgillett.github.io/sounderpy/
 Project-URL: Code, https://github.com/kylejgillett/sounderpy
 Project-URL: Operational Site, https://sounderpysoundings.anvil.app/
 Project-URL: PyPi, https://pypi.org/project/sounderpy/
 Project-URL: My Website, https://kylegillettphoto.com
```

### Comparing `sounderpy-3.0.4.dev1/src/sounderpy.egg-info/SOURCES.txt` & `sounderpy-3.0.4.dev2/src/sounderpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

