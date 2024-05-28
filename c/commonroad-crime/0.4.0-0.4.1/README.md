# Comparing `tmp/commonroad_crime-0.4.0.tar.gz` & `tmp/commonroad_crime-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonroad_crime-0.4.0.tar", last modified: Fri May 10 15:30:48 2024, max compression
+gzip compressed data, was "commonroad_crime-0.4.1.tar", last modified: Tue May 28 04:14:22 2024, max compression
```

## Comparing `commonroad_crime-0.4.0.tar` & `commonroad_crime-0.4.1.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.724271 commonroad_crime-0.4.0/
--rw-rw-rw-   0 root         (0) root         (0)     1570 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6805 2024-05-10 15:30:48.724271 commonroad_crime-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5386 2024-05-10 15:23:42.000000 commonroad_crime-0.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.632274 commonroad_crime-0.4.0/commonroad_crime/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:29:55.000000 commonroad_crime-0.4.0/commonroad_crime/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-10 14:43:51.000000 commonroad_crime-0.4.0/commonroad_crime/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.640273 commonroad_crime-0.4.0/commonroad_crime/data_structure/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:29:55.000000 commonroad_crime-0.4.0/commonroad_crime/data_structure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11885 2024-04-23 13:52:54.000000 commonroad_crime-0.4.0/commonroad_crime/data_structure/base.py
--rw-rw-rw-   0 root         (0) root         (0)    16249 2024-03-22 09:23:05.000000 commonroad_crime-0.4.0/commonroad_crime/data_structure/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     7182 2024-05-09 05:22:09.000000 commonroad_crime-0.4.0/commonroad_crime/data_structure/crime_interface.py
--rw-rw-rw-   0 root         (0) root         (0)     1965 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/data_structure/scene.py
--rw-rw-rw-   0 root         (0) root         (0)     2692 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/data_structure/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.644273 commonroad_crime-0.4.0/commonroad_crime/measure/
--rw-rw-rw-   0 root         (0) root         (0)     1273 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.648273 commonroad_crime-0.4.0/commonroad_crime/measure/acceleration/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:29:55.000000 commonroad_crime-0.4.0/commonroad_crime/measure/acceleration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5873 2024-04-08 15:17:55.000000 commonroad_crime-0.4.0/commonroad_crime/measure/acceleration/a_lat_req.py
--rw-rw-rw-   0 root         (0) root         (0)     5015 2024-04-08 15:17:55.000000 commonroad_crime-0.4.0/commonroad_crime/measure/acceleration/a_long_req.py
--rw-rw-rw-   0 root         (0) root         (0)     1945 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/acceleration/a_req.py
--rw-rw-rw-   0 root         (0) root         (0)     2731 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/acceleration/dst.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.652273 commonroad_crime-0.4.0/commonroad_crime/measure/distance/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:29:55.000000 commonroad_crime-0.4.0/commonroad_crime/measure/distance/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4732 2024-05-10 14:43:51.000000 commonroad_crime-0.4.0/commonroad_crime/measure/distance/dce.py
--rw-rw-rw-   0 root         (0) root         (0)     3882 2024-05-10 14:43:51.000000 commonroad_crime-0.4.0/commonroad_crime/measure/distance/hw.py
--rw-rw-rw-   0 root         (0) root         (0)     4444 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/distance/msd.py
--rw-rw-rw-   0 root         (0) root         (0)     6952 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/distance/psd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.664273 commonroad_crime-0.4.0/commonroad_crime/measure/index/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:29:55.000000 commonroad_crime-0.4.0/commonroad_crime/measure/index/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/index/aci.py
--rw-rw-rw-   0 root         (0) root         (0)     2100 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/index/btn.py
--rw-rw-rw-   0 root         (0) root         (0)     8272 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/index/ci.py
--rw-rw-rw-   0 root         (0) root         (0)     5110 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/index/cpi.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/index/pri.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/index/rss.py
--rw-rw-rw-   0 root         (0) root         (0)    10267 2024-04-28 15:00:45.000000 commonroad_crime-0.4.0/commonroad_crime/measure/index/soi.py
--rw-rw-rw-   0 root         (0) root         (0)     1983 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/index/stn.py
--rw-rw-rw-   0 root         (0) root         (0)     2779 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/index/tci.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.664273 commonroad_crime-0.4.0/commonroad_crime/measure/jerk/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:29:55.000000 commonroad_crime-0.4.0/commonroad_crime/measure/jerk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1853 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/jerk/lat_j.py
--rw-rw-rw-   0 root         (0) root         (0)     1966 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/jerk/long_j.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.668273 commonroad_crime-0.4.0/commonroad_crime/measure/potential/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:29:55.000000 commonroad_crime-0.4.0/commonroad_crime/measure/potential/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16293 2024-04-15 08:47:41.000000 commonroad_crime-0.4.0/commonroad_crime/measure/potential/pf.py
--rw-rw-rw-   0 root         (0) root         (0)      984 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/potential/sp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.672273 commonroad_crime-0.4.0/commonroad_crime/measure/probability/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:29:55.000000 commonroad_crime-0.4.0/commonroad_crime/measure/probability/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7488 2024-05-10 14:43:51.000000 commonroad_crime-0.4.0/commonroad_crime/measure/probability/p_mc.py
--rw-rw-rw-   0 root         (0) root         (0)      997 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/probability/p_smh.py
--rw-rw-rw-   0 root         (0) root         (0)      997 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/probability/p_srs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.676272 commonroad_crime-0.4.0/commonroad_crime/measure/reachable_set/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:29:55.000000 commonroad_crime-0.4.0/commonroad_crime/measure/reachable_set/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4945 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/reachable_set/drivable_area.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.696272 commonroad_crime-0.4.0/commonroad_crime/measure/time/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:29:55.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/ags.py
--rw-rw-rw-   0 root         (0) root         (0)    16262 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/et.py
--rw-rw-rw-   0 root         (0) root         (0)    11178 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/pet.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/pttc.py
--rw-rw-rw-   0 root         (0) root         (0)      974 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/tc.py
--rw-rw-rw-   0 root         (0) root         (0)     1926 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/tet.py
--rw-rw-rw-   0 root         (0) root         (0)     5928 2024-05-08 22:38:38.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/thw.py
--rw-rw-rw-   0 root         (0) root         (0)     3798 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/tit.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/ttb.py
--rw-rw-rw-   0 root         (0) root         (0)     6677 2024-04-08 15:29:07.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/ttc.py
--rw-rw-rw-   0 root         (0) root         (0)     6490 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/ttc_star.py
--rw-rw-rw-   0 root         (0) root         (0)     2550 2024-04-28 15:03:44.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/ttce.py
--rw-rw-rw-   0 root         (0) root         (0)      693 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/ttk.py
--rw-rw-rw-   0 root         (0) root         (0)     7121 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/ttm.py
--rw-rw-rw-   0 root         (0) root         (0)     2777 2024-03-19 15:06:10.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/ttr.py
--rw-rw-rw-   0 root         (0) root         (0)     2630 2024-03-19 15:06:10.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/tts.py
--rw-rw-rw-   0 root         (0) root         (0)     6606 2024-05-08 22:38:38.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/ttz.py
--rw-rw-rw-   0 root         (0) root         (0)      974 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/tv.py
--rw-rw-rw-   0 root         (0) root         (0)     5479 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/wttc.py
--rw-rw-rw-   0 root         (0) root         (0)     6475 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/time/wttr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.700272 commonroad_crime-0.4.0/commonroad_crime/measure/velocity/
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/velocity/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      987 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/measure/velocity/cs.py
--rw-rw-rw-   0 root         (0) root         (0)     3009 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/measure/velocity/delta_v.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.708272 commonroad_crime-0.4.0/commonroad_crime/utility/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:29:55.000000 commonroad_crime-0.4.0/commonroad_crime/utility/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10350 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/utility/batch_evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)     8463 2024-03-19 12:50:18.000000 commonroad_crime-0.4.0/commonroad_crime/utility/general.py
--rw-rw-rw-   0 root         (0) root         (0)     1843 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/utility/logger.py
--rw-rw-rw-   0 root         (0) root         (0)    10662 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/commonroad_crime/utility/optimization.py
--rw-rw-rw-   0 root         (0) root         (0)    34806 2024-03-16 09:37:51.000000 commonroad_crime-0.4.0/commonroad_crime/utility/simulation.py
--rw-rw-rw-   0 root         (0) root         (0)    14569 2024-05-08 22:38:38.000000 commonroad_crime-0.4.0/commonroad_crime/utility/solver.py
--rw-rw-rw-   0 root         (0) root         (0)    11746 2024-03-19 14:56:29.000000 commonroad_crime-0.4.0/commonroad_crime/utility/visualization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.720271 commonroad_crime-0.4.0/commonroad_crime.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6805 2024-05-10 15:30:48.000000 commonroad_crime-0.4.0/commonroad_crime.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3538 2024-05-10 15:30:48.000000 commonroad_crime-0.4.0/commonroad_crime.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 15:30:48.000000 commonroad_crime-0.4.0/commonroad_crime.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      296 2024-05-10 15:30:48.000000 commonroad_crime-0.4.0/commonroad_crime.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-10 15:30:48.000000 commonroad_crime-0.4.0/commonroad_crime.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-10 15:30:48.724271 commonroad_crime-0.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1926 2024-05-10 15:12:38.000000 commonroad_crime-0.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 15:30:48.720271 commonroad_crime-0.4.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 15:29:55.000000 commonroad_crime-0.4.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1811 2024-04-29 15:24:25.000000 commonroad_crime-0.4.0/tests/test_acceleration_domain.py
--rw-rw-rw-   0 root         (0) root         (0)     3614 2024-05-09 05:22:09.000000 commonroad_crime-0.4.0/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1915 2024-03-14 18:08:10.000000 commonroad_crime-0.4.0/tests/test_distance_domain.py
--rw-rw-rw-   0 root         (0) root         (0)     3794 2024-04-29 15:24:25.000000 commonroad_crime-0.4.0/tests/test_index_domain.py
--rw-rw-rw-   0 root         (0) root         (0)     1531 2024-04-29 15:24:25.000000 commonroad_crime-0.4.0/tests/test_jerk_domain.py
--rw-rw-rw-   0 root         (0) root         (0)      936 2024-04-29 15:24:25.000000 commonroad_crime-0.4.0/tests/test_potential_domain.py
--rw-rw-rw-   0 root         (0) root         (0)      992 2024-04-29 15:24:25.000000 commonroad_crime-0.4.0/tests/test_probability_domain.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/tests/test_reachable_set_domain.py
--rw-rw-rw-   0 root         (0) root         (0)     9902 2024-03-16 09:37:51.000000 commonroad_crime-0.4.0/tests/test_time_domain.py
--rw-rw-rw-   0 root         (0) root         (0)     6816 2024-03-14 17:14:19.000000 commonroad_crime-0.4.0/tests/test_utils_simulation.py
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-29 15:24:25.000000 commonroad_crime-0.4.0/tests/test_velocity_domain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:14:22.859714 commonroad_crime-0.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6810 2024-05-28 04:14:22.859714 commonroad_crime-0.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5386 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:14:22.851714 commonroad_crime-0.4.1/commonroad_crime/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 04:13:30.000000 commonroad_crime-0.4.1/commonroad_crime/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-28 03:58:43.000000 commonroad_crime-0.4.1/commonroad_crime/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:14:22.851714 commonroad_crime-0.4.1/commonroad_crime/data_structure/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 04:13:30.000000 commonroad_crime-0.4.1/commonroad_crime/data_structure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11885 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/data_structure/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    16249 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/data_structure/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     7355 2024-05-28 03:58:43.000000 commonroad_crime-0.4.1/commonroad_crime/data_structure/crime_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)     1965 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/data_structure/scene.py
+-rw-rw-rw-   0 root         (0) root         (0)     2692 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/data_structure/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:14:22.851714 commonroad_crime-0.4.1/commonroad_crime/measure/
+-rw-rw-rw-   0 root         (0) root         (0)     1273 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:14:22.851714 commonroad_crime-0.4.1/commonroad_crime/measure/acceleration/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 04:13:30.000000 commonroad_crime-0.4.1/commonroad_crime/measure/acceleration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5898 2024-05-28 03:58:43.000000 commonroad_crime-0.4.1/commonroad_crime/measure/acceleration/a_lat_req.py
+-rw-rw-rw-   0 root         (0) root         (0)     5040 2024-05-28 03:58:43.000000 commonroad_crime-0.4.1/commonroad_crime/measure/acceleration/a_long_req.py
+-rw-rw-rw-   0 root         (0) root         (0)     1945 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/acceleration/a_req.py
+-rw-rw-rw-   0 root         (0) root         (0)     2748 2024-05-28 03:58:43.000000 commonroad_crime-0.4.1/commonroad_crime/measure/acceleration/dst.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:14:22.851714 commonroad_crime-0.4.1/commonroad_crime/measure/distance/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 04:13:30.000000 commonroad_crime-0.4.1/commonroad_crime/measure/distance/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4732 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/distance/dce.py
+-rw-rw-rw-   0 root         (0) root         (0)     3905 2024-05-28 03:58:43.000000 commonroad_crime-0.4.1/commonroad_crime/measure/distance/hw.py
+-rw-rw-rw-   0 root         (0) root         (0)     4444 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/distance/msd.py
+-rw-rw-rw-   0 root         (0) root         (0)     6952 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/distance/psd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:14:22.855714 commonroad_crime-0.4.1/commonroad_crime/measure/index/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 04:13:30.000000 commonroad_crime-0.4.1/commonroad_crime/measure/index/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/index/aci.py
+-rw-rw-rw-   0 root         (0) root         (0)     2100 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/index/btn.py
+-rw-rw-rw-   0 root         (0) root         (0)     8289 2024-05-28 03:58:43.000000 commonroad_crime-0.4.1/commonroad_crime/measure/index/ci.py
+-rw-rw-rw-   0 root         (0) root         (0)     5165 2024-05-28 03:58:43.000000 commonroad_crime-0.4.1/commonroad_crime/measure/index/cpi.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/index/pri.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/index/rss.py
+-rw-rw-rw-   0 root         (0) root         (0)    10267 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/index/soi.py
+-rw-rw-rw-   0 root         (0) root         (0)     1983 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/index/stn.py
+-rw-rw-rw-   0 root         (0) root         (0)     2779 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/index/tci.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:14:22.855714 commonroad_crime-0.4.1/commonroad_crime/measure/jerk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 04:13:30.000000 commonroad_crime-0.4.1/commonroad_crime/measure/jerk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1853 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/jerk/lat_j.py
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/jerk/long_j.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:14:22.855714 commonroad_crime-0.4.1/commonroad_crime/measure/potential/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 04:13:30.000000 commonroad_crime-0.4.1/commonroad_crime/measure/potential/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16293 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/potential/pf.py
+-rw-rw-rw-   0 root         (0) root         (0)      984 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/potential/sp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:14:22.855714 commonroad_crime-0.4.1/commonroad_crime/measure/probability/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 04:13:30.000000 commonroad_crime-0.4.1/commonroad_crime/measure/probability/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7488 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/probability/p_mc.py
+-rw-rw-rw-   0 root         (0) root         (0)      997 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/probability/p_smh.py
+-rw-rw-rw-   0 root         (0) root         (0)      997 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/probability/p_srs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:14:22.855714 commonroad_crime-0.4.1/commonroad_crime/measure/reachable_set/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 04:13:30.000000 commonroad_crime-0.4.1/commonroad_crime/measure/reachable_set/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4945 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/reachable_set/drivable_area.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:14:22.855714 commonroad_crime-0.4.1/commonroad_crime/measure/time/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 04:13:30.000000 commonroad_crime-0.4.1/commonroad_crime/measure/time/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/time/ags.py
+-rw-rw-rw-   0 root         (0) root         (0)    16262 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/time/et.py
+-rw-rw-rw-   0 root         (0) root         (0)    11178 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/time/pet.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/time/pttc.py
+-rw-rw-rw-   0 root         (0) root         (0)      974 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/time/tc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1926 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/time/tet.py
+-rw-rw-rw-   0 root         (0) root         (0)     6007 2024-05-28 03:58:43.000000 commonroad_crime-0.4.1/commonroad_crime/measure/time/thw.py
+-rw-rw-rw-   0 root         (0) root         (0)     3798 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/time/tit.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/time/ttb.py
+-rw-rw-rw-   0 root         (0) root         (0)     6677 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/time/ttc.py
+-rw-rw-rw-   0 root         (0) root         (0)     6490 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/time/ttc_star.py
+-rw-rw-rw-   0 root         (0) root         (0)     2567 2024-05-28 03:58:43.000000 commonroad_crime-0.4.1/commonroad_crime/measure/time/ttce.py
+-rw-rw-rw-   0 root         (0) root         (0)      693 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/time/ttk.py
+-rw-rw-rw-   0 root         (0) root         (0)     7121 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/time/ttm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/time/ttr.py
+-rw-rw-rw-   0 root         (0) root         (0)     2630 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/time/tts.py
+-rw-rw-rw-   0 root         (0) root         (0)     6606 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/time/ttz.py
+-rw-rw-rw-   0 root         (0) root         (0)      974 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/time/tv.py
+-rw-rw-rw-   0 root         (0) root         (0)     5479 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/time/wttc.py
+-rw-rw-rw-   0 root         (0) root         (0)     6725 2024-05-28 03:51:13.000000 commonroad_crime-0.4.1/commonroad_crime/measure/time/wttr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:14:22.855714 commonroad_crime-0.4.1/commonroad_crime/measure/velocity/
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/velocity/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      987 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/velocity/cs.py
+-rw-rw-rw-   0 root         (0) root         (0)     3009 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/measure/velocity/delta_v.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:14:22.855714 commonroad_crime-0.4.1/commonroad_crime/utility/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 04:13:30.000000 commonroad_crime-0.4.1/commonroad_crime/utility/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10350 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/utility/batch_evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)     8463 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/utility/general.py
+-rw-rw-rw-   0 root         (0) root         (0)     1843 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/utility/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)    10662 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/utility/optimization.py
+-rw-rw-rw-   0 root         (0) root         (0)    34806 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/utility/simulation.py
+-rw-rw-rw-   0 root         (0) root         (0)    14569 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/utility/solver.py
+-rw-rw-rw-   0 root         (0) root         (0)    11746 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/commonroad_crime/utility/visualization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:14:22.859714 commonroad_crime-0.4.1/commonroad_crime.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6810 2024-05-28 04:14:22.000000 commonroad_crime-0.4.1/commonroad_crime.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3538 2024-05-28 04:14:22.000000 commonroad_crime-0.4.1/commonroad_crime.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 04:14:22.000000 commonroad_crime-0.4.1/commonroad_crime.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      301 2024-05-28 04:14:22.000000 commonroad_crime-0.4.1/commonroad_crime.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-28 04:14:22.000000 commonroad_crime-0.4.1/commonroad_crime.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 04:14:22.859714 commonroad_crime-0.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1931 2024-05-28 03:35:32.000000 commonroad_crime-0.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 04:14:22.859714 commonroad_crime-0.4.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 04:13:30.000000 commonroad_crime-0.4.1/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1811 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/tests/test_acceleration_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     3614 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1915 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/tests/test_distance_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     3794 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/tests/test_index_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/tests/test_jerk_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)      936 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/tests/test_potential_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)      992 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/tests/test_probability_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/tests/test_reachable_set_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     9917 2024-05-28 03:51:13.000000 commonroad_crime-0.4.1/tests/test_time_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     6816 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/tests/test_utils_simulation.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-05-28 03:28:42.000000 commonroad_crime-0.4.1/tests/test_velocity_domain.py
```

### Comparing `commonroad_crime-0.4.0/LICENSE` & `commonroad_crime-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/PKG-INFO` & `commonroad_crime-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonroad-crime
-Version: 0.4.0
+Version: 0.4.1
 Summary: criticality measures of automated vehicles
 Home-page: https://commonroad.in.tum.de/tools/commonroad-crime
 Author: Technical University of Munich
 Author-email: commonroad@lists.lrz.de
 License: BSD 3-Clause
 Project-URL: Documentation, https://cps.pages.gitlab.lrz.de/commonroad/commonroad-criticality-measures/
 Project-URL: Forum, https://github.com/CommonRoad/commonroad-crime/issues
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: commonroad-io>=2023.4
 Requires-Dist: commonroad-vehicle-models>=3.0.0
 Requires-Dist: commonroad-route-planner>=2024.2.0
 Requires-Dist: commonroad-drivability-checker>=2023.1
 Requires-Dist: commonroad-reach>=2024.1.2
-Requires-Dist: matplotlib>=3.5.2
+Requires-Dist: matplotlib<3.9,>=3.5.2
 Requires-Dist: numpy>=1.19.0
 Requires-Dist: scipy>=1.7.3
 Requires-Dist: shapely<3.0.0,>=2.0.1
 Requires-Dist: omegaconf>=2.1.1
 Requires-Dist: casadi>=3.6.3
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: imageio>=2.9.0
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: commonroad-crime Version: 0.4.0 Summary:
+Metadata-Version: 2.1 Name: commonroad-crime Version: 0.4.1 Summary:
 criticality measures of automated vehicles Home-page: https://
 commonroad.in.tum.de/tools/commonroad-crime Author: Technical University of
 Munich Author-email: commonroad@lists.lrz.de License: BSD 3-Clause Project-URL:
 Documentation, https://cps.pages.gitlab.lrz.de/commonroad/commonroad-
 criticality-measures/ Project-URL: Forum, https://github.com/CommonRoad/
 commonroad-crime/issues Project-URL: Source, https://github.com/CommonRoad/
 commonroad-crime Keywords: criticality,autonomous driving Classifier:
 Programming Language :: C++ Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: commonroad-io>=2023.4 Requires-
 Dist: commonroad-vehicle-models>=3.0.0 Requires-Dist: commonroad-route-
 planner>=2024.2.0 Requires-Dist: commonroad-drivability-checker>=2023.1
-Requires-Dist: commonroad-reach>=2024.1.2 Requires-Dist: matplotlib>=3.5.2
+Requires-Dist: commonroad-reach>=2024.1.2 Requires-Dist: matplotlib<3.9,>=3.5.2
 Requires-Dist: numpy>=1.19.0 Requires-Dist: scipy>=1.7.3 Requires-Dist:
 shapely<3.0.0,>=2.0.1 Requires-Dist: omegaconf>=2.1.1 Requires-Dist:
 casadi>=3.6.3 Requires-Dist: tqdm>=4.65.0 Requires-Dist: imageio>=2.9.0
 Requires-Dist: pytest>=7.4.0 # CommonRoad-CriMe ![image info](https://
 raw.githubusercontent.com/CommonRoad/commonroad-crime/develop/docs/figures/
 CriMe-banner.png) [![Linux](https://img.shields.io/badge/os-
 linux?&logo=Linux&logoColor=white&labelColor=gray)](https://pypi.python.org/
```

### Comparing `commonroad_crime-0.4.0/README.md` & `commonroad_crime-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/data_structure/base.py` & `commonroad_crime-0.4.1/commonroad_crime/data_structure/base.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/data_structure/configuration.py` & `commonroad_crime-0.4.1/commonroad_crime/data_structure/configuration.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/data_structure/crime_interface.py` & `commonroad_crime-0.4.1/commonroad_crime/data_structure/crime_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Yuanfei Lin, Marius Erath"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import os
 import logging
 from typing import List, Type
@@ -125,28 +125,30 @@
         for m_evaluator in self.measure_evaluators:
             if time_step is None:
                 m_evaluator.visualize()
             else:
                 if m_evaluator.time_step == time_step:
                     m_evaluator.visualize()
 
-    def safe_to_file(self, output_dir: str):
+    def save_to_file(self, output_dir: str):
         """
         Saves the criticality measures of a scenario to an XML file.
 
         This method serializes the scenario information along with the related
         criticality measures into an XML structure and saves it to a file. The
         XML file is structured with a root element and child elements that include
         the scenario details, parameters, and measures listed over all timesteps.
 
         Parameters:
         output_dir (str): The directory where the XML file will be saved.
 
-        The XML file is named using the scenario ID and prefixed with 'CriMe-'. The
-        file will include pretty-printed XML for better readability.
+        The XML file is named using the scenario ID with the prefix 'CriMe-'
+        and the suffix '_veh_123' where 123 is the ID of the vehicle with respect
+        to which the criticality was computed (ego vehicle).
+        The file will include pretty-printed XML for better readability.
         """
         # Ensure the output directory exists
         if not os.path.exists(output_dir):
             os.makedirs(output_dir)  # Create the directory if it does not exist
 
         scenario = self.config.scenario
         root = etree.Element("commonroad-criticality-measures")
@@ -185,12 +187,12 @@
                     "measure_value",
                     {"name": measure_name, "value": str(value)},
                 )
 
         # Save to file
         tree = etree.ElementTree(root)
         tree.write(
-            f"{output_dir}/CriMe-{scenario.scenario_id}.xml",
+            f"{output_dir}/CriMe-{scenario.scenario_id}_veh_{self.config.vehicle.ego_id}.xml",
             pretty_print=True,
             xml_declaration=True,
             encoding="utf-8",
         )
```

### Comparing `commonroad_crime-0.4.0/commonroad_crime/data_structure/scene.py` & `commonroad_crime-0.4.1/commonroad_crime/data_structure/scene.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/data_structure/type.py` & `commonroad_crime-0.4.1/commonroad_crime/data_structure/type.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/__init__.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/acceleration/a_lat_req.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/acceleration/a_lat_req.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import math
 import logging
 import numpy as np
@@ -96,14 +96,15 @@
                 self.other_vehicle.state_at_time(time_step).position,
             )[1]
         except ValueError as e:
             utils_log.print_and_log_warning(
                 logger,
                 f"* <A_LAT_REQ> During the projection of the vehicle {self.other_vehicle.obstacle_id} "
                 f"at time step {self.time_step}: {e}",
+                verbose,
             )
             # out of projection domain: the other vehicle is far away
             self.value = 0.0
         else:
             ttc = self._ttc_object.compute(vehicle_id, time_step, verbose=verbose)
             utils_log.print_and_log_info(
                 logger, f"*\t\t TTC is equal to {ttc}", verbose
```

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/acceleration/a_long_req.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/acceleration/a_long_req.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import math
 import numpy as np
 import logging
@@ -60,14 +60,15 @@
                 self.other_vehicle.state_at_time(time_step).position,
             )[1]
         except ValueError as e:
             utils_log.print_and_log_warning(
                 logger,
                 f"* <A_LONG_REQ> During the projection of the vehicle {self.other_vehicle.obstacle_id} "
                 f"at time step {self.time_step}: {e}",
+                verbose,
             )
             # out of projection domain: the other vehicle is far away
             a_req = 0.0
         else:
             # acceleration of the other vehicle along the lanelet
             a_obj = math.sqrt(
                 self.other_vehicle.state_at_time(time_step).acceleration ** 2
```

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/acceleration/a_req.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/acceleration/a_req.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/acceleration/dst.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/acceleration/dst.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import math
 import numpy as np
 import matplotlib.pyplot as plt
@@ -36,15 +36,15 @@
         super(DST, self).__init__(config)
         self._hw_solver = HW(config)
 
     def compute(self, vehicle_id: int, time_step: int = 0, verbose: bool = True):
         if not self.validate_update_states_log(vehicle_id, time_step, verbose):
             return np.nan
         # under the assumption that the velocity of the other object remains constant
-        headway = self._hw_solver.compute(vehicle_id, time_step)
+        headway = self._hw_solver.compute(vehicle_id, time_step, verbose=verbose)
         if headway < 0:
             return -math.inf
         v_ego = self.ego_vehicle.state_at_time(time_step).velocity
         v_otr = self.other_vehicle.state_at_time(time_step).velocity
         # from (17) in Schubert, Robin, Karsten Schulze, and Gerd Wanielik. "Situation assessment for automatic
         # lane-change maneuvers." IEEE Transactions on Intelligent Transportation Systems 11.3 (2010): 607-616.
         dst = (
```

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/distance/dce.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/distance/dce.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/distance/hw.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/distance/hw.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import matplotlib.pyplot as plt
 import logging
 import math
@@ -34,15 +34,15 @@
 
     measure_name = TypeDistance.HW
     monotone = TypeMonotone.NEG
 
     def __init__(self, config: CriMeConfiguration):
         super(HW, self).__init__(config)
 
-    def cal_headway(self):
+    def cal_headway(self, verbose=True):
         if isinstance(self.other_vehicle.obstacle_shape, Polygon):
             other_position = self.other_vehicle.state_at_time(self.time_step).position
         else:
             if isinstance(self.other_vehicle.obstacle_shape, Circle):
                 other_position = (
                     self.other_vehicle.state_at_time(self.time_step).position
                     - self.other_vehicle.obstacle_shape.radius
@@ -58,15 +58,15 @@
         )
         try:
             headway = utils_sol.compute_clcs_distance(
                 self.clcs, ego_position, other_position
             )[0]
         except ValueError as e:
             utils_log.print_and_log_warning(
-                logger, f"<HW> During the projection of the other vehicle: {e}"
+                logger, f"<HW> During the projection of the other vehicle: {e}", verbose
             )
             headway = math.inf
         if headway < 0:
             return math.inf
         else:
             return headway
```

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/distance/msd.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/distance/msd.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/distance/psd.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/distance/psd.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/index/aci.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/index/aci.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/index/btn.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/index/btn.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/index/ci.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/index/ci.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Yuanfei Lin and Kun Qian"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import logging
 import matplotlib.pyplot as plt
 import math
@@ -77,15 +77,15 @@
         if self.ci_config.m_b:
             m2 = self.ci_config.m_b
         else:
             # assume that the vehicle b has the same mass as the ego vehicle
             m2 = m1
 
         # Use PET object
-        pet = self._pet_object.compute(vehicle_id, time_step)
+        pet = self._pet_object.compute(vehicle_id, time_step, verbose=verbose)
 
         # Threshold of 5.0 as standard configuration in the paper
         threshold = self.ci_config.pet_threshold
 
         # As PET = math.inf in case of no conflict area for PET, no separate check is needed
         if pet >= threshold:
             utils_log.print_and_log_info(
```

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/index/cpi.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/index/cpi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Yuanfei Lin, Sicheng Wang"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import logging
 import math
 
@@ -61,15 +61,17 @@
             return np.nan
 
         self.end_time_step = self.ego_vehicle.prediction.final_time_step
         self.value = 0.0
 
         for ts in range(self.time_step, self.end_time_step):
             try:
-                dr_lon_req = -self._a_lon_req_object.compute(vehicle_id, ts)
+                dr_lon_req = -self._a_lon_req_object.compute(
+                    vehicle_id, ts, verbose=verbose
+                )
                 self.dr_lon_req_list.append(dr_lon_req)
             except ValueError:
                 utils_log.print_and_log_info(
                     logger,
                     f"*\t\t vehicle {vehicle_id} is no longer in the lanelets.",
                     verbose,
                 )
```

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/index/pri.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/index/pri.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/index/rss.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/index/rss.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/index/soi.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/index/soi.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/index/stn.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/index/stn.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/index/tci.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/index/tci.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/jerk/lat_j.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/jerk/lat_j.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/jerk/long_j.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/jerk/long_j.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/potential/pf.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/potential/pf.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/potential/sp.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/potential/sp.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/probability/p_mc.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/probability/p_mc.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/probability/p_smh.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/probability/p_smh.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/probability/p_srs.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/probability/p_srs.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/reachable_set/drivable_area.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/reachable_set/drivable_area.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/time/ags.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/time/ags.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/time/et.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/time/et.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/time/pet.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/time/pet.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/time/pttc.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/time/pttc.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/time/tc.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/time/tc.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/time/tet.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/time/tet.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/time/thw.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/time/thw.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import matplotlib.pyplot as plt
 import logging
 import math
@@ -43,38 +43,40 @@
             add_on = vehicle.obstacle_shape.radius
         else:
             raise ValueError(
                 f"<{self.measure_name}>: obstacle shape {type(vehicle.obstacle_shape).__name__} not supported."
             )
         return add_on
 
-    def cal_headway(self):
+    def cal_headway(self, verbose=True):
         try:
             other_position = self.other_vehicle.state_at_time(self.time_step).position
             other_s, _ = self.clcs.convert_to_curvilinear_coords(
                 other_position[0], other_position[1]
             )
         except ValueError as e:
             utils_log.print_and_log_warning(
                 logger,
                 f"* <THW> During the projection of the vehicle {self.other_vehicle.obstacle_id} "
                 f"at time step {self.time_step}: {e}",
+                verbose,
             )
             # out of projection domain: the other vehicle is far away
             return math.inf
         try:
             ego_position = self.ego_vehicle.state_at_time(self.time_step).position
             ego_s, _ = self.clcs.convert_to_curvilinear_coords(
                 ego_position[0], ego_position[1]
             )
         except ValueError as e:
             utils_log.print_and_log_warning(
                 logger,
                 f"* <THW> During the projection of the ego vehicle with id {self.ego_vehicle.obstacle_id} "
                 f"at time step {self.time_step}: {e}",
+                verbose,
             )
             # out of projection domain: the ref path should be problematic
             return math.nan
 
         # additional position for the vehicles
         ego_s += self._compute_vehicle_add_on(self.ego_vehicle)
         other_s -= self._compute_vehicle_add_on(self.other_vehicle)
@@ -101,15 +103,15 @@
         if not self.validate_update_states_log(vehicle_id, time_step, verbose):
             return np.nan
 
         if self._except_obstacle_in_same_lanelet(
             expected_value=math.inf, verbose=verbose
         ):
             return self.value
-        self.value = self.cal_headway()
+        self.value = self.cal_headway(verbose=verbose)
         if self.value is not math.inf:
             self.value = utils_gen.int_round(self.value, 2)
         utils_log.print_and_log_info(
             logger,
             f"*\t\t {self.measure_name} with vehicle id {vehicle_id} = {self.value}",
             verbose,
         )
```

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/time/tit.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/time/tit.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/time/ttb.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/time/ttb.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/time/ttc.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/time/ttc.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/time/ttc_star.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/time/ttc_star.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/time/ttce.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/time/ttce.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Oliver Specht, Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 __maintainer__ = "beta"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "Pre-alpha"
 
 import matplotlib.pyplot as plt
 import numpy as np
 import logging
@@ -40,15 +40,15 @@
     def compute(self, vehicle_id: int, time_step: int = 0, verbose: bool = True):
         """
         Using DCE to calculate the TTCE value. DCE marks the time step when the minimal distance is reached.
         """
         if not self.validate_update_states_log(vehicle_id, time_step, verbose):
             return np.nan
 
-        self._dce_object.compute(vehicle_id, self.time_step)
+        self._dce_object.compute(vehicle_id, self.time_step, verbose=verbose)
         if self._dce_object.time_dce is not math.inf:
             self.value = utils_gen.int_round(
                 (self._dce_object.time_dce - self.time_step) * self.dt, 3
             )
         else:
             self.value = self._dce_object.time_dce
         utils_log.print_and_log_info(
```

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/time/ttk.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/time/ttk.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/time/ttm.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/time/ttm.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/time/ttr.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/time/ttr.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/time/tts.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/time/tts.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/time/ttz.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/time/ttz.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/time/tv.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/time/tv.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/time/wttc.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/time/wttc.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/time/wttr.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/time/wttr.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Yuanfei Lin"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["KoSi"]
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 __maintainer__ = "Yuanfei Lin"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "beta"
 
 import math
 import copy
 import logging
@@ -60,15 +60,14 @@
         self.reach_config.vehicle.ego.a_lat_max = (
             self.configuration.vehicle.curvilinear.a_lat_max
         )
         self.reach_config.planning.dt = self.sce.dt
         # self.reach_config.planning.coordinate_system = "CART"
         self.reach_config.update()
         self.reach_interface = ReachableSetInterface(self.reach_config)
-        self._end_sim = None
 
     def _update_initial_state(self, target_state: State):
         self.reach_config.planning_problem.initial_state.position = (
             target_state.position
         )
         self.reach_config.planning_problem.initial_state.velocity = (
             target_state.velocity
@@ -79,33 +78,33 @@
         self.reach_config.planning_problem.initial_state.time_step = (
             target_state.time_step
         )
 
     def compute(self, time_step: int = 0, vehicle_id=None, verbose: bool = True):
         if not self.validate_update_states_log(vehicle_id, time_step, verbose):
             return np.nan
-        self.ttc = self.ttc_object.compute(time_step)
+        self.ttc = self.ttc_object.compute(time_step, verbose=verbose)
         if self.ttc == 0:
             self.value = -math.inf
         elif self.ttc == math.inf:
             self.value = math.inf
         else:
-            self.value = self.binary_search(time_step)
+            self.value = self.binary_search(time_step, verbose=verbose)
         if self.value in [math.inf, -math.inf]:
             utils_log.print_and_log_info(
                 logger, f"*\t\t {self.measure_name} = {self.value}"
             )
             return self.value
         self.value = utils_gen.int_round(self.value, str(self.dt)[::-1].find("."))
         utils_log.print_and_log_info(
             logger, f"*\t\t {self.measure_name} = {self.value}"
         )
         return self.value
 
-    def binary_search(self, initial_step: int):
+    def binary_search(self, initial_step: int, verbose=False):
         """
         Binary search to find the last time to execute the maneuver.
         """
         wttr = -math.inf
         low = initial_step
         tstc = int(
             utils_gen.int_round(
@@ -114,23 +113,30 @@
         )
         high = tstc + initial_step
         time_end = self.ego_vehicle.prediction.final_time_step
         while low < high:
             mid = int((low + high) / 2)
             mid_state = copy.deepcopy(self.ego_vehicle.state_at_time(mid))
             self._update_initial_state(mid_state)
+
+            # update configurations
             self.reach_config.update(
                 planning_problem=self.reach_config.planning_problem
             )
+            self.reach_config.planning.steps_computation = (
+                time_end - mid_state.time_step
+            )
             self.reach_config.scenario.remove_obstacle(
                 self.reach_config.scenario.obstacle_by_id(self.ego_vehicle.obstacle_id)
             )
+            self.reach_config.debug.save_config = verbose
+
+            # reset the interface and compute the reachable sets
             self.reach_interface.reset(self.reach_config)
-            self._end_sim = time_end - mid
-            self.reach_interface.compute_reachable_sets(0, time_end, verbose=True)
+            self.reach_interface.compute_reachable_sets(verbose=verbose)
             if self.reach_interface.reachable_set_at_step(time_end):
                 # the final step is still reachable without causing the collision
                 low = mid + 1
             else:
                 high = mid
         if low != initial_step:
             # no -1 (differs from the binary search for TTM)
@@ -146,15 +152,15 @@
             self._update_initial_state(mid_state)
             self.reach_config.update(
                 planning_problem=self.reach_config.planning_problem
             )
             self.reach_config.scenario.remove_obstacle(
                 self.reach_config.scenario.obstacle_by_id(self.ego_vehicle.obstacle_id)
             )
+            self.reach_config.planning.steps_computation = (
+                self.ego_vehicle.prediction.final_time_step - mid_state.time_step
+            )
             self.reach_interface.reset(self.reach_config)
-            self._end_sim = self.ego_vehicle.prediction.final_time_step
 
-            self.reach_interface.compute_reachable_sets(0, self._end_sim, verbose=True)
-            util_visual.plot_scenario_with_reachable_sets(
-                self.reach_interface, step_start=0, step_end=self._end_sim
-            )
+            self.reach_interface.compute_reachable_sets(verbose=False)
+            util_visual.plot_scenario_with_reachable_sets(self.reach_interface)
             # util_visual.plot_collision_checker(self.reach_interface)
```

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/velocity/cs.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/velocity/cs.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/measure/velocity/delta_v.py` & `commonroad_crime-0.4.1/commonroad_crime/measure/velocity/delta_v.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/utility/batch_evaluation.py` & `commonroad_crime-0.4.1/commonroad_crime/utility/batch_evaluation.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/utility/general.py` & `commonroad_crime-0.4.1/commonroad_crime/utility/general.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/utility/logger.py` & `commonroad_crime-0.4.1/commonroad_crime/utility/logger.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/utility/optimization.py` & `commonroad_crime-0.4.1/commonroad_crime/utility/optimization.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/utility/simulation.py` & `commonroad_crime-0.4.1/commonroad_crime/utility/simulation.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/utility/solver.py` & `commonroad_crime-0.4.1/commonroad_crime/utility/solver.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime/utility/visualization.py` & `commonroad_crime-0.4.1/commonroad_crime/utility/visualization.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/commonroad_crime.egg-info/PKG-INFO` & `commonroad_crime-0.4.1/commonroad_crime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonroad-crime
-Version: 0.4.0
+Version: 0.4.1
 Summary: criticality measures of automated vehicles
 Home-page: https://commonroad.in.tum.de/tools/commonroad-crime
 Author: Technical University of Munich
 Author-email: commonroad@lists.lrz.de
 License: BSD 3-Clause
 Project-URL: Documentation, https://cps.pages.gitlab.lrz.de/commonroad/commonroad-criticality-measures/
 Project-URL: Forum, https://github.com/CommonRoad/commonroad-crime/issues
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: commonroad-io>=2023.4
 Requires-Dist: commonroad-vehicle-models>=3.0.0
 Requires-Dist: commonroad-route-planner>=2024.2.0
 Requires-Dist: commonroad-drivability-checker>=2023.1
 Requires-Dist: commonroad-reach>=2024.1.2
-Requires-Dist: matplotlib>=3.5.2
+Requires-Dist: matplotlib<3.9,>=3.5.2
 Requires-Dist: numpy>=1.19.0
 Requires-Dist: scipy>=1.7.3
 Requires-Dist: shapely<3.0.0,>=2.0.1
 Requires-Dist: omegaconf>=2.1.1
 Requires-Dist: casadi>=3.6.3
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: imageio>=2.9.0
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: commonroad-crime Version: 0.4.0 Summary:
+Metadata-Version: 2.1 Name: commonroad-crime Version: 0.4.1 Summary:
 criticality measures of automated vehicles Home-page: https://
 commonroad.in.tum.de/tools/commonroad-crime Author: Technical University of
 Munich Author-email: commonroad@lists.lrz.de License: BSD 3-Clause Project-URL:
 Documentation, https://cps.pages.gitlab.lrz.de/commonroad/commonroad-
 criticality-measures/ Project-URL: Forum, https://github.com/CommonRoad/
 commonroad-crime/issues Project-URL: Source, https://github.com/CommonRoad/
 commonroad-crime Keywords: criticality,autonomous driving Classifier:
 Programming Language :: C++ Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: commonroad-io>=2023.4 Requires-
 Dist: commonroad-vehicle-models>=3.0.0 Requires-Dist: commonroad-route-
 planner>=2024.2.0 Requires-Dist: commonroad-drivability-checker>=2023.1
-Requires-Dist: commonroad-reach>=2024.1.2 Requires-Dist: matplotlib>=3.5.2
+Requires-Dist: commonroad-reach>=2024.1.2 Requires-Dist: matplotlib<3.9,>=3.5.2
 Requires-Dist: numpy>=1.19.0 Requires-Dist: scipy>=1.7.3 Requires-Dist:
 shapely<3.0.0,>=2.0.1 Requires-Dist: omegaconf>=2.1.1 Requires-Dist:
 casadi>=3.6.3 Requires-Dist: tqdm>=4.65.0 Requires-Dist: imageio>=2.9.0
 Requires-Dist: pytest>=7.4.0 # CommonRoad-CriMe ![image info](https://
 raw.githubusercontent.com/CommonRoad/commonroad-crime/develop/docs/figures/
 CriMe-banner.png) [![Linux](https://img.shields.io/badge/os-
 linux?&logo=Linux&logoColor=white&labelColor=gray)](https://pypi.python.org/
```

### Comparing `commonroad_crime-0.4.0/commonroad_crime.egg-info/SOURCES.txt` & `commonroad_crime-0.4.1/commonroad_crime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/setup.py` & `commonroad_crime-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     data_files=[(".", ["LICENSE"])],
     install_requires=[
         "commonroad-io>=2023.4",
         "commonroad-vehicle-models>=3.0.0",
         "commonroad-route-planner>=2024.2.0",
         "commonroad-drivability-checker>=2023.1",
         "commonroad-reach>=2024.1.2",
-        "matplotlib>=3.5.2",
+        "matplotlib>=3.5.2,<3.9",
         "numpy>=1.19.0",
         "scipy>=1.7.3",
         "shapely<3.0.0,>=2.0.1",
         "omegaconf>=2.1.1",
         "casadi>=3.6.3",
         "tqdm>=4.65.0",
         "imageio>=2.9.0",
```

### Comparing `commonroad_crime-0.4.0/tests/test_acceleration_domain.py` & `commonroad_crime-0.4.1/tests/test_acceleration_domain.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/tests/test_base.py` & `commonroad_crime-0.4.1/tests/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,8 +100,8 @@
 
         crime_interface.evaluate_scene([TTC], time_step=35)
         self.assertTrue(
             np.isnan(crime_interface.criticality_dict[35][TTC.measure_name]),
             "The result should be NaN.",
         )
 
-        crime_interface.safe_to_file(config.general.path_output)
+        crime_interface.save_to_file(config.general.path_output)
```

### Comparing `commonroad_crime-0.4.0/tests/test_distance_domain.py` & `commonroad_crime-0.4.1/tests/test_distance_domain.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/tests/test_index_domain.py` & `commonroad_crime-0.4.1/tests/test_index_domain.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/tests/test_jerk_domain.py` & `commonroad_crime-0.4.1/tests/test_jerk_domain.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/tests/test_potential_domain.py` & `commonroad_crime-0.4.1/tests/test_potential_domain.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/tests/test_probability_domain.py` & `commonroad_crime-0.4.1/tests/test_probability_domain.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/tests/test_reachable_set_domain.py` & `commonroad_crime-0.4.1/tests/test_reachable_set_domain.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/tests/test_time_domain.py` & `commonroad_crime-0.4.1/tests/test_time_domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
 
         ttc_object = TTCStar(self.config)
         ttc = ttc_object.compute()
         self.assertGreater(ttc, wttc)
 
     def test_wttr(self):
         wttr_object = WTTR(self.config)
-        wttr = wttr_object.compute(10)
+        wttr = wttr_object.compute(10, verbose=False)
         wttr_object.visualize()
         self.assertEqual(wttr, 1.3)
         wttr2 = wttr_object.compute()
         self.assertAlmostEqual(wttr, wttr2 - 1.0)
 
     def test_ttz(self):
         self.config.general.name_scenario = "ZAM_Zip-2_1_T-1"
```

### Comparing `commonroad_crime-0.4.0/tests/test_utils_simulation.py` & `commonroad_crime-0.4.1/tests/test_utils_simulation.py`

 * *Files identical despite different names*

### Comparing `commonroad_crime-0.4.0/tests/test_velocity_domain.py` & `commonroad_crime-0.4.1/tests/test_velocity_domain.py`

 * *Files identical despite different names*

