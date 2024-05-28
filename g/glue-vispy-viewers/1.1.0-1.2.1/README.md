# Comparing `tmp/glue-vispy-viewers-1.1.0.tar.gz` & `tmp/glue_vispy_viewers-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue-vispy-viewers-1.1.0.tar", last modified: Mon Aug 21 21:46:50 2023, max compression
+gzip compressed data, was "glue_vispy_viewers-1.2.1.tar", last modified: Tue May 28 09:53:36 2024, max compression
```

## Comparing `glue-vispy-viewers-1.1.0.tar` & `glue_vispy_viewers-1.2.1.tar`

### file list

```diff
@@ -1,111 +1,146 @@
-drwxr-xr-x   0 tom        (504) staff       (20)        0 2023-08-21 21:46:50.094276 glue-vispy-viewers-1.1.0/
--rw-r--r--   0 tom        (504) staff       (20)       45 2017-02-15 13:47:26.000000 glue-vispy-viewers-1.1.0/.coveragerc
-drwxr-xr-x   0 tom        (504) staff       (20)        0 2023-08-21 21:46:50.077820 glue-vispy-viewers-1.1.0/.github/
--rw-r--r--   0 tom        (504) staff       (20)      374 2023-01-12 10:21:40.000000 glue-vispy-viewers-1.1.0/.github/release.yml
-drwxr-xr-x   0 tom        (504) staff       (20)        0 2023-08-21 21:46:50.078273 glue-vispy-viewers-1.1.0/.github/workflows/
--rw-r--r--   0 tom        (504) staff       (20)     1590 2023-02-11 07:11:53.000000 glue-vispy-viewers-1.1.0/.github/workflows/ci_workflows.yml
--rw-r--r--   0 tom        (504) staff       (20)      870 2023-01-12 10:21:40.000000 glue-vispy-viewers-1.1.0/.github/workflows/update-changelog.yaml
--rw-r--r--   0 tom        (504) staff       (20)      668 2015-10-19 13:17:47.000000 glue-vispy-viewers-1.1.0/.gitignore
--rw-r--r--   0 tom        (504) staff       (20)    18231 2023-08-15 09:57:17.000000 glue-vispy-viewers-1.1.0/CHANGES.md
--rw-r--r--   0 tom        (504) staff       (20)     1290 2015-08-13 16:09:59.000000 glue-vispy-viewers-1.1.0/LICENSE
--rw-r--r--   0 tom        (504) staff       (20)       77 2017-02-24 21:52:51.000000 glue-vispy-viewers-1.1.0/MANIFEST.in
--rw-r--r--   0 tom        (504) staff       (20)     2412 2023-08-21 21:46:50.094372 glue-vispy-viewers-1.1.0/PKG-INFO
--rw-r--r--   0 tom        (504) staff       (20)     2064 2023-01-12 11:37:37.000000 glue-vispy-viewers-1.1.0/README.rst
--rw-r--r--   0 tom        (504) staff       (20)      537 2023-01-12 10:21:40.000000 glue-vispy-viewers-1.1.0/RELEASE.rst
--rw-r--r--   0 tom        (504) staff       (20)      316 2023-01-12 11:15:09.000000 glue-vispy-viewers-1.1.0/codecov.yml
-drwxr-xr-x   0 tom        (504) staff       (20)        0 2023-08-21 21:46:50.078830 glue-vispy-viewers-1.1.0/glue_vispy_viewers/
--rw-r--r--   0 tom        (504) staff       (20)      237 2023-08-21 21:45:49.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/__init__.py
-drwxr-xr-x   0 tom        (504) staff       (20)        0 2023-08-21 21:46:50.083326 glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/
--rw-r--r--   0 tom        (504) staff       (20)        0 2019-11-08 10:35:33.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/__init__.py
--rw-r--r--   0 tom        (504) staff       (20)     4754 2023-08-15 09:57:17.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/axes.py
--rw-r--r--   0 tom        (504) staff       (20)     3896 2020-01-27 21:39:50.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/compat.py
--rw-r--r--   0 tom        (504) staff       (20)     4421 2019-11-08 10:35:33.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/glue_point.png
--rw-r--r--   0 tom        (504) staff       (20)     1094 2019-11-08 10:35:33.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/glue_record_start.png
--rw-r--r--   0 tom        (504) staff       (20)     5669 2019-11-08 10:35:33.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/glue_record_stop.png
--rw-r--r--   0 tom        (504) staff       (20)     3707 2019-11-08 10:35:33.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/glue_rotate.png
--rw-r--r--   0 tom        (504) staff       (20)      585 2019-11-08 10:35:33.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/layer_artist.py
--rw-r--r--   0 tom        (504) staff       (20)     1368 2021-07-27 06:25:59.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/layer_state.py
--rw-r--r--   0 tom        (504) staff       (20)     7288 2023-08-15 10:01:16.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/selection_tools.py
-drwxr-xr-x   0 tom        (504) staff       (20)        0 2023-08-21 21:46:50.084153 glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/tests/
--rw-r--r--   0 tom        (504) staff       (20)        0 2019-11-08 10:35:33.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/tests/__init__.py
--rw-r--r--   0 tom        (504) staff       (20)      702 2023-01-12 10:21:40.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/tests/test_3d_axis_visual.py
--rw-r--r--   0 tom        (504) staff       (20)     3604 2023-08-21 21:45:49.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/tests/test_vispy_toolbar.py
--rw-r--r--   0 tom        (504) staff       (20)     2800 2023-08-21 21:45:49.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/tests/test_vispy_viewer.py
--rw-r--r--   0 tom        (504) staff       (20)     1974 2023-01-12 10:21:40.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/tests/test_vispy_widget.py
--rw-r--r--   0 tom        (504) staff       (20)     1541 2023-08-21 21:45:49.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/toolbar.py
--rw-r--r--   0 tom        (504) staff       (20)     3653 2020-01-27 21:40:16.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/tools.py
--rw-r--r--   0 tom        (504) staff       (20)     1549 2023-08-21 21:45:49.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/viewer_options.py
--rw-r--r--   0 tom        (504) staff       (20)    10599 2023-01-12 10:22:20.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/viewer_options.ui
--rw-r--r--   0 tom        (504) staff       (20)     4611 2021-10-17 21:34:57.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/viewer_state.py
--rw-r--r--   0 tom        (504) staff       (20)     7255 2023-08-21 21:45:49.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/vispy_data_viewer.py
--rw-r--r--   0 tom        (504) staff       (20)     6264 2020-01-27 21:40:16.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/vispy_widget.py
-drwxr-xr-x   0 tom        (504) staff       (20)        0 2023-08-21 21:46:50.084964 glue-vispy-viewers-1.1.0/glue_vispy_viewers/compat/
--rw-r--r--   0 tom        (504) staff       (20)     1774 2019-11-08 16:39:56.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/compat/LICENSE.txt
--rw-r--r--   0 tom        (504) staff       (20)        0 2019-11-08 16:39:56.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/compat/__init__.py
--rw-r--r--   0 tom        (504) staff       (20)    22545 2020-01-27 21:38:38.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/compat/axis.py
--rw-r--r--   0 tom        (504) staff       (20)    25462 2023-01-12 10:21:40.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/compat/text.py
--rw-r--r--   0 tom        (504) staff       (20)     1992 2023-08-21 21:45:49.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/conftest.py
-drwxr-xr-x   0 tom        (504) staff       (20)        0 2023-08-21 21:46:50.087962 glue-vispy-viewers-1.1.0/glue_vispy_viewers/isosurface/
--rw-r--r--   0 tom        (504) staff       (20)      149 2019-11-08 10:35:33.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/isosurface/__init__.py
--rw-r--r--   0 tom        (504) staff       (20)      959 2020-01-27 21:40:16.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/isosurface/isosurface_viewer.py
--rw-r--r--   0 tom        (504) staff       (20)     6850 2020-01-27 21:40:16.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/isosurface/layer_artist.py
--rw-r--r--   0 tom        (504) staff       (20)     1568 2021-07-27 06:25:59.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/isosurface/layer_state.py
--rw-r--r--   0 tom        (504) staff       (20)     1862 2023-08-21 21:45:49.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/isosurface/layer_style_widget.py
--rw-r--r--   0 tom        (504) staff       (20)     3290 2023-08-21 21:45:49.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/isosurface/layer_style_widget.ui
--rw-r--r--   0 tom        (504) staff       (20)    13332 2023-01-12 10:21:40.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/isosurface/multi_iso_visual.py
-drwxr-xr-x   0 tom        (504) staff       (20)        0 2023-08-21 21:46:50.088246 glue-vispy-viewers-1.1.0/glue_vispy_viewers/isosurface/tests/
--rw-r--r--   0 tom        (504) staff       (20)        0 2019-11-08 10:35:33.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/isosurface/tests/__init__.py
--rw-r--r--   0 tom        (504) staff       (20)     3134 2023-08-21 21:45:49.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/isosurface/tests/test_isosurface_viewer.py
--rw-r--r--   0 tom        (504) staff       (20)      149 2019-11-08 10:35:33.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/isosurface/viewer_state.py
-drwxr-xr-x   0 tom        (504) staff       (20)        0 2023-08-21 21:46:50.089790 glue-vispy-viewers-1.1.0/glue_vispy_viewers/scatter/
--rw-r--r--   0 tom        (504) staff       (20)      140 2019-11-08 10:35:33.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/scatter/__init__.py
--rw-r--r--   0 tom        (504) staff       (20)    12883 2020-10-01 16:55:15.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/scatter/layer_artist.py
--rw-r--r--   0 tom        (504) staff       (20)     4946 2020-09-08 07:23:28.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/scatter/layer_state.py
--rw-r--r--   0 tom        (504) staff       (20)     3151 2023-08-21 21:45:49.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/scatter/layer_style_widget.py
--rw-r--r--   0 tom        (504) staff       (20)    23396 2023-08-21 21:45:49.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/scatter/layer_style_widget.ui
--rw-r--r--   0 tom        (504) staff       (20)     8440 2020-10-01 16:55:15.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/scatter/multi_scatter.py
--rw-r--r--   0 tom        (504) staff       (20)     1809 2020-01-27 21:40:16.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/scatter/scatter_toolbar.py
--rw-r--r--   0 tom        (504) staff       (20)     1343 2020-01-27 21:40:16.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/scatter/scatter_viewer.py
-drwxr-xr-x   0 tom        (504) staff       (20)        0 2023-08-21 21:46:50.090032 glue-vispy-viewers-1.1.0/glue_vispy_viewers/scatter/tests/
--rw-r--r--   0 tom        (504) staff       (20)        0 2019-11-08 10:35:33.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/scatter/tests/__init__.py
--rw-r--r--   0 tom        (504) staff       (20)    11930 2023-08-21 21:45:49.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/scatter/tests/test_scatter_viewer.py
--rw-r--r--   0 tom        (504) staff       (20)      964 2019-11-08 10:35:33.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/scatter/viewer_state.py
-drwxr-xr-x   0 tom        (504) staff       (20)        0 2023-08-21 21:46:50.090279 glue-vispy-viewers-1.1.0/glue_vispy_viewers/tests/
--rw-r--r--   0 tom        (504) staff       (20)        0 2019-11-08 10:35:33.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/tests/__init__.py
-drwxr-xr-x   0 tom        (504) staff       (20)        0 2023-08-21 21:46:50.091421 glue-vispy-viewers-1.1.0/glue_vispy_viewers/tests/data/
--rw-r--r--   0 tom        (504) staff       (20)        0 2019-11-08 10:35:33.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/tests/data/__init__.py
--rw-r--r--   0 tom        (504) staff       (20)    20124 2023-08-21 21:45:49.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/tests/data/multiple_volumes_v1.glu
--rw-r--r--   0 tom        (504) staff       (20)    22729 2023-08-21 21:45:49.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/tests/data/multiple_volumes_v2.glu
--rw-r--r--   0 tom        (504) staff       (20)    21818 2023-08-21 21:45:49.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/tests/data/scatter_volume_selection.glu
--rw-r--r--   0 tom        (504) staff       (20)    12879 2023-08-21 21:45:49.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/tests/data/scatter_volume_v0.glu
--rw-r--r--   0 tom        (504) staff       (20)    18668 2023-08-21 21:45:49.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/tests/data/scatter_volume_v1.glu
--rw-r--r--   0 tom        (504) staff       (20)     5667 2020-01-27 21:40:16.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/tests/test_session_back_compat.py
--rw-r--r--   0 tom        (504) staff       (20)     3472 2023-08-21 21:45:49.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/utils.py
-drwxr-xr-x   0 tom        (504) staff       (20)        0 2023-08-21 21:46:50.093499 glue-vispy-viewers-1.1.0/glue_vispy_viewers/volume/
--rw-r--r--   0 tom        (504) staff       (20)      137 2019-11-08 10:35:33.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/volume/__init__.py
--rw-r--r--   0 tom        (504) staff       (20)      293 2020-01-27 21:40:16.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/volume/colors.py
--rw-r--r--   0 tom        (504) staff       (20)     8239 2023-02-11 07:10:42.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/volume/layer_artist.py
--rw-r--r--   0 tom        (504) staff       (20)     1795 2021-10-17 21:34:57.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/volume/layer_state.py
--rw-r--r--   0 tom        (504) staff       (20)     1903 2023-08-21 21:45:49.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/volume/layer_style_widget.py
--rw-r--r--   0 tom        (504) staff       (20)     3204 2023-08-21 21:45:49.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/volume/layer_style_widget.ui
--rw-r--r--   0 tom        (504) staff       (20)    10862 2022-05-16 21:16:32.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/volume/shaders.py
-drwxr-xr-x   0 tom        (504) staff       (20)        0 2023-08-21 21:46:50.094168 glue-vispy-viewers-1.1.0/glue_vispy_viewers/volume/tests/
--rw-r--r--   0 tom        (504) staff       (20)        0 2019-11-08 10:35:33.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/volume/tests/__init__.py
--rw-r--r--   0 tom        (504) staff       (20)     2078 2019-11-08 10:35:33.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/volume/tests/test_volume_toolbar.py
--rw-r--r--   0 tom        (504) staff       (20)     6817 2023-08-21 21:45:49.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/volume/tests/test_volume_viewer.py
--rw-r--r--   0 tom        (504) staff       (20)     2776 2021-07-27 06:25:59.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/volume/viewer_state.py
--rw-r--r--   0 tom        (504) staff       (20)     7449 2020-01-27 21:40:16.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/volume/volume_toolbar.py
--rw-r--r--   0 tom        (504) staff       (20)    11371 2020-09-08 08:01:39.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/volume/volume_viewer.py
--rw-r--r--   0 tom        (504) staff       (20)    15255 2023-01-12 10:54:39.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers/volume/volume_visual.py
-drwxr-xr-x   0 tom        (504) staff       (20)        0 2023-08-21 21:46:50.079597 glue-vispy-viewers-1.1.0/glue_vispy_viewers.egg-info/
--rw-r--r--   0 tom        (504) staff       (20)     2412 2023-08-21 21:46:50.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers.egg-info/PKG-INFO
--rw-r--r--   0 tom        (504) staff       (20)     3723 2023-08-21 21:46:50.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (504) staff       (20)        1 2023-08-21 21:46:50.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (504) staff       (20)      111 2023-08-21 21:46:50.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers.egg-info/entry_points.txt
--rw-r--r--   0 tom        (504) staff       (20)      279 2023-08-21 21:46:50.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers.egg-info/requires.txt
--rw-r--r--   0 tom        (504) staff       (20)       19 2023-08-21 21:46:50.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers.egg-info/top_level.txt
--rw-r--r--   0 tom        (504) staff       (20)        1 2023-08-21 21:46:50.000000 glue-vispy-viewers-1.1.0/glue_vispy_viewers.egg-info/zip-safe
--rw-r--r--   0 tom        (504) staff       (20)       31 2018-03-10 18:43:14.000000 glue-vispy-viewers-1.1.0/pytest.ini
--rw-r--r--   0 tom        (504) staff       (20)     1910 2023-08-21 21:46:50.094716 glue-vispy-viewers-1.1.0/setup.cfg
--rwxr-xr-x   0 tom        (504) staff       (20)      398 2019-06-23 08:56:40.000000 glue-vispy-viewers-1.1.0/setup.py
--rw-r--r--   0 tom        (504) staff       (20)      629 2023-02-11 07:12:05.000000 glue-vispy-viewers-1.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.373900 glue_vispy_viewers-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.353900 glue_vispy_viewers-1.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.353900 glue_vispy_viewers-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/.github/workflows/update-changelog.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    19468 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-28 09:53:36.373900 glue_vispy_viewers-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/RELEASE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.357900 glue_vispy_viewers-1.2.1/glue_vispy_viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.357900 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/axes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/glue_point.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/glue_rotate.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.357900 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/jupyter/data_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/jupyter/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/layer_artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/layer_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.361900 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/qt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/qt/data_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/qt/glue_record_start.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/qt/glue_record_stop.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.361900 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/qt/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/qt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/qt/tests/test_vispy_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/qt/tests/test_vispy_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/qt/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/qt/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/qt/viewer_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/qt/viewer_options.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/selection_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.361900 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/tests/test_3d_axis_visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/tests/test_vispy_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/viewer_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/vispy_data_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/vispy_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.361900 glue_vispy_viewers-1.2.1/glue_vispy_viewers/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/compat/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22545 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/compat/axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25462 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/compat/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.361900 glue_vispy_viewers-1.2.1/glue_vispy_viewers/qt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/qt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.361900 glue_vispy_viewers-1.2.1/glue_vispy_viewers/qt/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/qt/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.365900 glue_vispy_viewers-1.2.1/glue_vispy_viewers/qt/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/qt/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20124 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/qt/tests/data/multiple_volumes_v1.glu
+-rw-r--r--   0 runner    (1001) docker     (127)    22729 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/qt/tests/data/multiple_volumes_v2.glu
+-rw-r--r--   0 runner    (1001) docker     (127)    21818 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/qt/tests/data/scatter_volume_selection.glu
+-rw-r--r--   0 runner    (1001) docker     (127)    12879 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/qt/tests/data/scatter_volume_v0.glu
+-rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/qt/tests/data/scatter_volume_v1.glu
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/qt/tests/test_session_back_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.365900 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.365900 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/jupyter/layer_state_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/jupyter/layer_state_widget.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/jupyter/scatter_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.365900 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/jupyter/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/jupyter/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/jupyter/tests/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/jupyter/viewer_state_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/jupyter/viewer_state_widget.vue
+-rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/layer_artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/layer_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/multi_scatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.365900 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/qt/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/qt/layer_style_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23396 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/qt/layer_style_widget.ui
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/qt/scatter_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.365900 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/qt/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/qt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11930 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/qt/tests/test_scatter_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/scatter_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/scatter_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.365900 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.365900 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/tests/data/state_widgets.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/viewer_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.369900 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/colors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.369900 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/jupyter/layer_state_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/jupyter/layer_state_widget.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.369900 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/jupyter/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/jupyter/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/jupyter/tests/test_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/jupyter/viewer_state_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/jupyter/viewer_state_widget.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/jupyter/volume_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/layer_artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/layer_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.369900 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/qt/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/qt/layer_style_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/qt/layer_style_widget.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.369900 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/qt/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/qt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/qt/tests/test_volume_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6817 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/qt/tests/test_volume_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/qt/volume_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10862 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/shaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.369900 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.369900 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/tests/data/state_widgets.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/viewer_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7531 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/volume_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/volume_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15143 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/volume_visual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:53:36.369900 glue_vispy_viewers-1.2.1/glue_vispy_viewers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-28 09:53:36.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-05-28 09:53:36.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:53:36.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-28 09:53:36.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-28 09:53:36.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 09:53:36.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:53:36.000000 glue_vispy_viewers-1.2.1/glue_vispy_viewers.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-28 09:53:36.373900 glue_vispy_viewers-1.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      398 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-28 09:52:53.000000 glue_vispy_viewers-1.2.1/tox.ini
```

### Comparing `glue-vispy-viewers-1.1.0/.github/workflows/ci_workflows.yml` & `glue_vispy_viewers-1.2.1/.github/workflows/ci_workflows.yml`

 * *Files 22% similar despite different names*

```diff
@@ -29,27 +29,42 @@
       libraries: |
         apt:
           - '^libxcb.*-dev'
           - libxkbcommon-x11-dev
           - libegl1-mesa
 
       envs: |
-        # Standard tests
+        # Tests without Qt. For now glfw can't run on MacOS runners in headless mode
+        # so we only run on Linux and Windows.
         - linux: py38-test
-        - linux: py39-test
-        - linux: py310-test-pyqt6
-        - linux: py311-test-dev-pyqt6
+        - windows: py39-test
+        - linux: py310-test
+        - windows: py311-test
+        - linux: py311-test-dev
 
-        - macos: py38-test
-        - macos: py39-test-dev
-        - macos: py310-test-pyqt6
+        # Tests with Jupyter
+        - linux: py38-test-jupyter
+        - windows: py39-test-jupyter
+        - linux: py310-test-jupyter
+        - windows: py311-test-jupyter
+
+        # Tests with Qt
+        - linux: py38-test-pyqt63
+        - linux: py39-test-pyside63
+        - linux: py310-test-pyqt64
+        - linux: py311-test-dev-pyqt64
+        # - macos: py38-test-pyqt63  # segfault
+        - macos: py39-test-pyside63
+        - macos: py310-test-pyqt64
+        - macos: py311-test-dev-pyqt64
+        - windows: py38-test-pyqt63
+        # - windows: py39-test-pyside63  # segfault
+        - windows: py310-test-pyqt64
+        - windows: py311-test-dev-pyqt64
 
-        - windows: py38-test
-        - windows: py39-test-dev
-        - windows: py310-test-pyqt6
 
   publish:
     needs: tests
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/publish_pure_python.yml@v1
     with:
       # Setup PyQt5 deps and headless X server as per pyvista/setup-headless-display-action@v1
       libraries: '^libxcb.*-dev libxkbcommon-x11-dev xvfb'
```

### Comparing `glue-vispy-viewers-1.1.0/.github/workflows/update-changelog.yaml` & `glue_vispy_viewers-1.2.1/.github/workflows/update-changelog.yaml`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/.gitignore` & `glue_vispy_viewers-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/CHANGES.md` & `glue_vispy_viewers-1.2.1/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,39 @@
 # Full changelog
 
+## v1.2.0 - 2024-05-24
+
+<!-- Release notes generated using configuration in .github/release.yml at main -->
+### What's Changed
+
+#### New Features
+
+* Refactor viewer classes to split out Qt from non-Qt part, and define Jupyter viewers by @astrofrog in https://github.com/glue-viz/glue-vispy-viewers/pull/381
+
+#### Bug Fixes
+
+* Fixes following Qt/Jupyter split by @astrofrog in https://github.com/glue-viz/glue-vispy-viewers/pull/383
+* Fix save/record tools in Qt and volume selection tools in Jupyter by @astrofrog in https://github.com/glue-viz/glue-vispy-viewers/pull/384
+* Fix tests by @astrofrog in https://github.com/glue-viz/glue-vispy-viewers/pull/385
+
+#### Other Changes
+
+* Remove isosurface sub-module as it has been broken for a long time by @astrofrog in https://github.com/glue-viz/glue-vispy-viewers/pull/382
+
+**Full Changelog**: https://github.com/glue-viz/glue-vispy-viewers/compare/v1.1.0...v1.2.0
+
+## v1.1.0 - 2023-08-21
+
+<!-- Release notes generated using configuration in .github/release.yml at main -->
+### What's Changed
+
+- Updated imports to glue_qt by @astrofrog in https://github.com/glue-viz/glue-vispy-viewers/pull/378
+
+**Full Changelog**: https://github.com/glue-viz/glue-vispy-viewers/compare/v1.0.7...v1.1.0
+
 ## v1.0.7 - 2023-02-11
 
 <!-- Release notes generated using configuration in .github/release.yml at main -->
 ### What's Changed
 
 #### Bug Fixes
```

### Comparing `glue-vispy-viewers-1.1.0/LICENSE` & `glue_vispy_viewers-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/RELEASE.rst` & `glue_vispy_viewers-1.2.1/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/axes.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/axes.py`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/compat.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/compat.py`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/glue_point.png` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/glue_point.png`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/glue_record_start.png` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/qt/glue_record_start.png`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/glue_record_stop.png` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/qt/glue_record_stop.png`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/glue_rotate.png` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/glue_rotate.png`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/layer_artist.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/layer_artist.py`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/layer_state.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/layer_state.py`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/selection_tools.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/selection_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,33 @@
 class VispyMouseMode(CheckableTool):
 
     # this will create an abstract selection mode class to handle mouse events
     # instanced by lasso, rectangle, circular and point mode
 
     def __init__(self, viewer):
         super(VispyMouseMode, self).__init__(viewer)
-        self._vispy_widget = viewer._vispy_widget
         self.current_visible_array = None
 
+    def activate(self):
+        if self.viewer is not None:
+            self.viewer.toolbar._enable_tool_interactions(self)
+        self.reset()
+
+    def deactivate(self):
+        if self.viewer is not None:
+            self.viewer.toolbar._disable_tool_interactions(self)
+        self.reset()
+
+    def reset(self):
+        pass
+
+    @property
+    def _vispy_widget(self):
+        return self.viewer._vispy_widget
+
     def get_visible_data(self):
         visible = []
         # Loop over visible layer artists
         for layer_artist in self.viewer._layer_artist_container:
             # Only extract Data objects, not subsets
             if isinstance(layer_artist.layer, Data):
                 visible.append(layer_artist.layer)
@@ -81,19 +97,15 @@
     icon = 'glue_lasso'
     tool_id = 'vispy:lasso'
     action_text = 'Select data using a lasso selection'
 
     def __init__(self, viewer):
         super(LassoSelectionMode, self).__init__(viewer)
         self.line = Line(color='purple',
-                         width=2, method='agg',
-                         parent=self._vispy_widget.canvas.scene)
-
-    def activate(self):
-        self.reset()
+                         width=2, method='agg')
 
     def reset(self):
         self.line_pos = []
         self.line.set_data(np.zeros((0, 2), dtype=float))
         self.line.parent = None
 
     def press(self, event):
@@ -129,17 +141,14 @@
     action_text = 'Select data using a rectangular selection'
 
     def __init__(self, viewer):
         super(RectangleSelectionMode, self).__init__(viewer)
         self.rectangle = Rectangle(center=(0, 0), width=1, height=1, border_width=2,
                                    color=(0, 0, 0, 0), border_color='purple')
 
-    def activate(self):
-        self.reset()
-
     def reset(self):
         self.corner1 = None
         self.corner2 = None
         self.rectangle.parent = None
 
     def press(self, event):
         if event.button == 1:
@@ -184,17 +193,14 @@
     action_text = 'Select data using a circular selection'
 
     def __init__(self, viewer):
         super(CircleSelectionMode, self).__init__(viewer)
         self.ellipse = Ellipse(center=(0, 0), radius=1, border_width=2,
                                color=(0, 0, 0, 0), border_color='purple')
 
-    def activate(self):
-        self.reset()
-
     def reset(self):
         self.center = None
         self.radius = 0
         self.ellipse.parent = None
 
     def press(self, event):
         if event.button == 1:
```

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/tests/test_3d_axis_visual.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/tests/test_3d_axis_visual.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,9 +13,10 @@
     canvas = scene.SceneCanvas(keys=None, size=(800, 600), show=True)
     view = canvas.central_widget.add_view()
     scene_transform = scene.STTransform()
     view.camera = scene.cameras.TurntableCamera(parent=view.scene,
                                                 fov=0., distance=4.0)
     AxesVisual3D(view=view, axis_color='red', transform=scene_transform)
 
-    canvas.native.show()
-    canvas.native.close()
+    if hasattr(canvas.native, 'show'):  # Qt
+        canvas.native.show()
+        canvas.native.close()
```

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/tests/test_vispy_toolbar.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/qt/tests/test_vispy_toolbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # pylint: disable=I0011,W0613,W0201,W0212,E1101,E1103
 
 import os
 import sys
 import pytest
-from mock import patch
+from unittest.mock import patch
 
 from glue_qt.app import GlueApplication
 from glue.core import Data
 
-from ...scatter.scatter_viewer import VispyScatterViewer
+from ....scatter.qt.scatter_viewer import VispyScatterViewer
 
-from .. import tools  # noqa:
+from ... import tools  # noqa:
 
 try:
     import imageio  # noqa
 except ImportError:
     IMAGEIO_INSTALLED = False
 else:
     IMAGEIO_INSTALLED = True
```

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/tests/test_vispy_viewer.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/qt/tests/test_vispy_viewer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # pylint: disable=I0011,W0613,W0201,W0212,E1101,E1103
 
 import numpy as np
 import pytest
 import sys
-from mock import patch
+from unittest.mock import patch
 
 from glue.core import Data, DataCollection
 from glue_qt.app import GlueApplication
 
 from glue.core.tests.util import simple_session
 
-from ..vispy_data_viewer import BaseVispyViewer
-from ...volume.volume_viewer import VispyVolumeViewer
-from ...scatter.scatter_viewer import VispyScatterViewer
-from ...isosurface.isosurface_viewer import VispyIsosurfaceViewer
+from ..data_viewer import BaseVispyViewer
+from ....volume.qt.volume_viewer import VispyVolumeViewer
+from ....scatter.qt.scatter_viewer import VispyScatterViewer
 
 IS_WIN = sys.platform == 'win32'
 
 
 def setup_function(func):
     import os
     os.environ['GLUE_TESTING'] = 'True'
@@ -34,16 +33,14 @@
         w.register_to_hub(hub)
         with patch.object(BaseVispyViewer, 'unregister') as unregister:
             w.close()
         unregister.assert_called_once_with(hub)
 
     @pytest.mark.skipif('IS_WIN', reason='Windows fatal exception: access violation')
     def test_add_viewer(self, tmpdir):
-        if self.widget_cls == VispyIsosurfaceViewer:
-            pytest.skip(reason='MultiIsoVisual broken')
 
         d1 = Data(x=np.random.random((2,) * self.ndim))
         d2 = Data(x=np.random.random((2,) * self.ndim))
         dc = DataCollection([d1, d2])
         app = GlueApplication(dc)
         w = app.new_data_viewer(self.widget_cls, data=d1)
         w.viewer_size = (300, 400)
@@ -57,16 +54,14 @@
         for viewer in app2.viewers:
             assert viewer[0].viewer_size == (300, 400)
 
         app.close()
         app2.close()
 
     def test_options_widget(self):
-        if self.widget_cls == VispyIsosurfaceViewer:
-            pytest.skip(reason='MultiIsoVisual broken')
 
         d1 = Data(x=np.random.random((2,) * self.ndim))
         d2 = Data(x=np.random.random((2,) * self.ndim))
         dc = DataCollection([d1, d2])
         app = GlueApplication(dc)
         w = app.new_data_viewer(self.widget_cls, data=d1)
 
@@ -88,11 +83,7 @@
 
 class TestDataViewerVolume(BaseTestDataViewer):
     widget_cls = VispyVolumeViewer
 
 
 class TestDataViewerScatter(BaseTestDataViewer):
     widget_cls = VispyScatterViewer
-
-
-class TestDataViewerIsosurface(BaseTestDataViewer):
-    widget_cls = VispyIsosurfaceViewer
```

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/tests/test_vispy_widget.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/tests/test_vispy_widget.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 @pytest.mark.skipif('IS_WIN', reason='Windows fatal exception: access violation')
 def test_vispy_widget():
 
     d = Vispy3DViewerState()
 
     w = VispyWidgetHelper(viewer_state=d)
 
-    w.canvas.native.show()
+    if hasattr(w.canvas.native, 'show'):  # Qt
+        w.canvas.native.show()
 
     # Try adding marker visuals to the scene
     positions = np.random.random((1000, 3))
     scat_visual = scene.visuals.Markers()
     scat_visual.set_data(positions, symbol='disc', edge_color=None, face_color='red')
     w.add_data_visual(scat_visual)
```

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/tools.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/qt/tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,32 +4,16 @@
 
 from glue.viewers.common.tool import Tool, CheckableTool
 
 from glue.config import viewer_tool
 
 from vispy import app, io
 
-
 RECORD_START_ICON = os.path.join(os.path.dirname(__file__), 'glue_record_start.png')
 RECORD_STOP_ICON = os.path.join(os.path.dirname(__file__), 'glue_record_stop.png')
-ROTATE_ICON = os.path.join(os.path.dirname(__file__), 'glue_rotate.png')
-
-
-@viewer_tool
-class ResetTool(Tool):
-
-    icon = 'glue_home'
-    tool_id = 'vispy:reset'
-    action_text = 'Reset the view'
-    tool_tip = 'Reset the view'
-
-    def activate(self):
-        self.viewer._vispy_widget.view.camera.reset()
-        self.viewer._vispy_widget._toggle_perspective()
-        self.viewer.state.reset_limits()
 
 
 @viewer_tool
 class SaveTool(Tool):
 
     icon = 'glue_filesave'
     tool_id = 'vispy:save'
@@ -93,29 +77,7 @@
 
     def set_icon(self, icon):
         self.viewer.toolbar.actions[self.tool_id].setIcon(QtGui.QIcon(icon))
 
     def record(self, event):
         im = self.viewer._vispy_widget.canvas.render()
         self.writer.append_data(im)
-
-
-@viewer_tool
-class RotateTool(CheckableTool):
-
-    icon = ROTATE_ICON
-    tool_id = 'vispy:rotate'
-    action_text = 'Continuously rotate view'
-    tool_tip = 'Start/Stop rotation'
-
-    timer = None
-
-    def activate(self):
-        if self.timer is None:
-            self.timer = app.Timer(connect=self.rotate)
-        self.timer.start(0.1)
-
-    def deactivate(self):
-        self.timer.stop()
-
-    def rotate(self, event):
-        self.viewer._vispy_widget.view.camera.azimuth -= 1.  # set speed as constant first
```

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/viewer_options.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/qt/viewer_options.py`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/viewer_options.ui` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/qt/viewer_options.ui`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/viewer_state.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/viewer_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,67 +32,67 @@
     perspective_view = CallbackProperty(False)
     clip_data = CallbackProperty(True)
     native_aspect = CallbackProperty(False)
     line_width = CallbackProperty(1.)
 
     layers = ListCallbackProperty()
 
-    limits_cache = CallbackProperty()
+    _limits_cache = CallbackProperty()
 
     def _update_priority(self, name):
         if name == 'layers':
             return 2
         elif name.endswith(('_min', '_max')):
             return 0
         else:
             return 1
 
     def __init__(self, **kwargs):
 
         super(Vispy3DViewerState, self).__init__(**kwargs)
 
-        if self.limits_cache is None:
-            self.limits_cache = {}
+        if self._limits_cache is None:
+            self._limits_cache = {}
 
         self.x_lim_helper = StateAttributeLimitsHelper(self, attribute='x_att',
                                                        lower='x_min', upper='x_max',
-                                                       cache=self.limits_cache)
+                                                       cache=self._limits_cache)
 
         self.y_lim_helper = StateAttributeLimitsHelper(self, attribute='y_att',
                                                        lower='y_min', upper='y_max',
-                                                       cache=self.limits_cache)
+                                                       cache=self._limits_cache)
 
         self.z_lim_helper = StateAttributeLimitsHelper(self, attribute='z_att',
                                                        lower='z_min', upper='z_max',
-                                                       cache=self.limits_cache)
+                                                       cache=self._limits_cache)
 
         # TODO: if limits_cache is re-assigned to a different object, we need to
         # update the attribute helpers. However if in future we make limits_cache
         # into a smart dictionary that can call callbacks when elements are
         # changed then we shouldn't always call this. It'd also be nice to
         # avoid this altogether and make it more clean.
-        self.add_callback('limits_cache', self._update_limits_cache)
+        self.add_callback('_limits_cache', self._update_limits_cache)
 
     def reset_limits(self):
         self.x_lim_helper.log = False
         self.x_lim_helper.percentile = 100.
         self.x_lim_helper.update_values(force=True)
         self.y_lim_helper.log = False
         self.y_lim_helper.percentile = 100.
         self.y_lim_helper.update_values(force=True)
         self.z_lim_helper.log = False
         self.z_lim_helper.percentile = 100.
         self.z_lim_helper.update_values(force=True)
 
     def _update_limits_cache(self, *args):
-        self.x_lim_helper._cache = self.limits_cache
+        self.x_lim_helper._cache = self._limits_cache
         self.x_lim_helper._update_attribute()
-        self.y_lim_helper._cache = self.limits_cache
+        self.y_lim_helper._cache = self._limits_cache
         self.y_lim_helper._update_attribute()
-        self.z_lim_helper._cache = self.limits_cache
+        self.z_lim_helper._cache = self._limits_cache
         self.z_lim_helper._update_attribute()
 
     @property
     def aspect(self):
         # TODO: this could be cached based on the limits, but is not urgent
         aspect = np.array([1, 1, 1], dtype=float)
         if self.native_aspect:
```

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/common/vispy_widget.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/common/vispy_widget.py`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/compat/LICENSE.txt` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/compat/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/compat/axis.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/compat/axis.py`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/compat/text.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/compat/text.py`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/isosurface/isosurface_viewer.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/scatter_viewer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,36 @@
-from ..common.vispy_data_viewer import BaseVispyViewer
-from .layer_artist import IsosurfaceLayerArtist
-from .layer_style_widget import IsosurfaceLayerStyleWidget
-from .viewer_state import Vispy3DIsosurfaceViewerState
+from ..common.vispy_data_viewer import BaseVispyViewerMixin
+from .layer_artist import ScatterLayerArtist
+from .viewer_state import Vispy3DScatterViewerState
 
 from ..common import tools as _tools, selection_tools  # noqa
+from . import scatter_toolbar  # noqa
 
 
-class VispyIsosurfaceViewer(BaseVispyViewer):
+class VispyScatterViewerMixin(BaseVispyViewerMixin):
 
-    LABEL = "3D Isosurface Rendering"
+    LABEL = "3D Scatter"
 
-    _state_cls = Vispy3DIsosurfaceViewerState
-    _layer_style_widget_cls = IsosurfaceLayerStyleWidget
+    _state_cls = Vispy3DScatterViewerState
 
-    tools = BaseVispyViewer.tools
+    tools = BaseVispyViewerMixin.tools + ['vispy:lasso', 'vispy:rectangle',
+                                          'vispy:circle', 'scatter3d:point']
 
-    _data_artist_cls = IsosurfaceLayerArtist
-    _subset_artist_cls = IsosurfaceLayerArtist
+    _data_artist_cls = ScatterLayerArtist
+    _subset_artist_cls = ScatterLayerArtist
 
     def add_data(self, data):
 
         first_layer_artist = len(self._layer_artist_container) == 0
 
-        added = super(VispyIsosurfaceViewer, self).add_data(data)
+        added = super().add_data(data)
 
         if added:
             if first_layer_artist:
-                self.state.set_limits(*self._layer_artist_container[0].bbox)
+                # The above call to add_data may have added subset layers, some
+                # of which may be incompatible with the data, so we need to now
+                # explicitly use the layer for the actual data object.
+                layer = self._layer_artist_container[data][0]
+                self.state.set_limits(*layer.default_limits)
                 self._ready_draw = True
 
         return added
```

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/isosurface/layer_artist.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/layer_artist.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,183 +1,207 @@
+import uuid
+import weakref
+
 import numpy as np
-from scipy.ndimage import gaussian_filter
 
-from glue.core.data import Subset
-from glue.core.exceptions import IncompatibleAttribute
+from matplotlib.colors import ColorConverter
 
-from .layer_state import IsosurfaceLayerState
+from glue.core.data import Subset, Data
+from glue.core.exceptions import IncompatibleAttribute
+from glue.core.fixed_resolution_buffer import ARRAY_CACHE, PIXEL_CACHE
+from .colors import get_translucent_cmap
+from .layer_state import VolumeLayerState
 from ..common.layer_artist import VispyLayerArtist
 
-from vispy.color import BaseColormap
 
-from .multi_iso_visual import MultiIsoVisual
+class DataProxy(object):
 
-DATA_PROPERTIES = set(['attribute', 'level_low', 'level_high'])
-LEVEL_PROPERTIES = set(['step_value'])
-COLOR_PROPERTIES = set(['color', 'alpha', 'cmap'])
-STEP_PROPERTIES = set(['step'])
-
-
-# TODO: create colormaps that is prettier
-class TransFire(BaseColormap):
-    glsl_map = """
-    vec4 translucent_grays(int l){
-    if (l==1)
-        {return $color_0;}
-    if (l==2)
-        {return $color_1;}
-    if (l==3)
-        {return $color_2;}
-    if (l==4)
-        {return $color_3;}
-    if (l==5)
-        {return $color_4;}
-    if (l==6)
-        {return $color_5;}
-    if (l==7)
-        {return $color_6;}
-    if (l==8)
-        {return $color_7;}
-    if (l==9)
-        {return $color_8;}
-    if (l==10)
-        {return $color_9;}
+    def __init__(self, viewer_state, layer_artist):
+        self._viewer_state = weakref.ref(viewer_state)
+        self._layer_artist = weakref.ref(layer_artist)
 
-    }
-    """
-# class AutoCmap(BaseColormap):
-#     colors =
-#     glsl_map = """
-#     vec4 translucent_grays(int l){
-#
-#     }
-#     """
-# vec4 translucent_fire(float t) {
-#         return vec4(pow(t, 0.5), t, t*t, max(0, t*1.05 - 0.05));
-#     }
+    @property
+    def layer_artist(self):
+        return self._layer_artist()
+
+    @property
+    def viewer_state(self):
+        return self._viewer_state()
+
+    @property
+    def shape(self):
+
+        x_axis = self.viewer_state.x_att.axis
+        y_axis = self.viewer_state.y_att.axis
+        z_axis = self.viewer_state.z_att.axis
+
+        if isinstance(self.layer_artist.layer, Subset):
+            full_shape = self.layer_artist.layer.data.shape
+        else:
+            full_shape = self.layer_artist.layer.shape
+
+        return full_shape[z_axis], full_shape[y_axis], full_shape[x_axis]
 
+    def compute_fixed_resolution_buffer(self, bounds=None):
 
-class IsosurfaceLayerArtist(VispyLayerArtist):
+        shape = [bound[2] for bound in bounds]
+
+        if self.layer_artist is None or self.viewer_state is None:
+            return np.broadcast_to(0, shape)
+
+        if isinstance(self.layer_artist.layer, Subset):
+            try:
+                subset_state = self.layer_artist.layer.subset_state
+                result = self.layer_artist.layer.data.compute_fixed_resolution_buffer(
+                    target_data=self.layer_artist._viewer_state.reference_data,
+                    bounds=bounds, subset_state=subset_state,
+                    cache_id=self.layer_artist.id)
+            except IncompatibleAttribute:
+                self.layer_artist.disable_incompatible_subset()
+                return np.broadcast_to(0, shape)
+            else:
+                self.layer_artist.enable()
+        else:
+            try:
+                result = self.layer_artist.layer.compute_fixed_resolution_buffer(
+                    target_data=self.layer_artist._viewer_state.reference_data,
+                    bounds=bounds, target_cid=self.layer_artist.state.attribute,
+                    cache_id=self.layer_artist.id)
+            except IncompatibleAttribute:
+                self.layer_artist.disable('Layer data is not fully linked to reference data')
+                return np.broadcast_to(0, shape)
+            else:
+                self.layer_artist.enable()
+
+        return result
+
+
+class VolumeLayerArtist(VispyLayerArtist):
     """
-    A layer artist to render isosurfaces.
+    A layer artist to render volumes.
+
+    This is more complex than for other visual types, because for volumes, we
+    need to manage all the volumes via a single MultiVolume visual class for
+    each data viewer.
     """
 
-    def __init__(self, vispy_viewer, layer=None, layer_state=None):
+    def __init__(self, vispy_viewer=None, layer=None, layer_state=None):
 
-        super(IsosurfaceLayerArtist, self).__init__(layer)
+        super(VolumeLayerArtist, self).__init__(layer)
 
         self._clip_limits = None
 
         self.layer = layer or layer_state.layer
         self.vispy_widget = vispy_viewer._vispy_widget
 
         # TODO: need to remove layers when layer artist is removed
         self._viewer_state = vispy_viewer.state
-        self.state = layer_state or IsosurfaceLayerState(layer=self.layer)
+        self.state = layer_state or VolumeLayerState(layer=self.layer)
         if self.state not in self._viewer_state.layers:
             self._viewer_state.layers.append(self.state)
 
-        # self._iso_visual = scene.Isosurface(np.ones((3, 3, 3)), level=0.5, shading='smooth')
-        # Create isosurface visual
-        self._iso_visual = MultiIsoVisual(np.ones((3, 3, 3)), step=4, relative_step_size=0.5)
-        # relative_step_size: ray casting performance, recommond 0.5~1.5)
-        self.vispy_widget.add_data_visual(self._iso_visual)
+        # We create a unique ID for this layer artist, that will be used to
+        # refer to the layer artist in the MultiVolume. We have to do this
+        # rather than use self.id because we can't guarantee the latter is
+        # unique.
+        self.id = str(uuid.uuid4())
+
+        self._multivol = self.vispy_widget._multivol
+        self._multivol.allocate(self.id)
 
         self._viewer_state.add_global_callback(self._update_volume)
         self.state.add_global_callback(self._update_volume)
 
         self.reset_cache()
 
+        self._data_proxy = None
+
     def reset_cache(self):
         self._last_viewer_state = {}
         self._last_layer_state = {}
 
     @property
+    def visual(self):
+        return self._multivol
+
+    @property
     def bbox(self):
         return (-0.5, self.layer.shape[2] - 0.5,
                 -0.5, self.layer.shape[1] - 0.5,
                 -0.5, self.layer.shape[0] - 0.5)
 
+    @property
+    def shape(self):
+        return self.layer.shape
+
     def redraw(self):
         """
         Redraw the Vispy canvas
         """
         self.vispy_widget.canvas.update()
 
     def clear(self):
         """
         Remove the layer artist from the visualization
         """
-        self._iso_visual.parent = None
+        # We don't want to deallocate here because this can be called if we
+        # disable the layer due to incompatible attributes
+        self._multivol.disable(self.id)
 
-    def _update_level(self):
-        # TODO: set iso clim
-        # self._iso_visual.set_data()
-        pass
-
-    def _update_step(self):
-        # TODO: generate a new color and transparancy scheme based on step num
-        self._iso_visual.step = self.state.step
-        self.redraw()
-        # self._update_color()
-
-    def _update_color(self):
-        cmap_data = self.state.cmap(np.linspace(0, 1, 10).tolist())  # self.cmap returns 10 colors
-        cmap_data = cmap_data.tolist()
-        t = TransFire(colors=cmap_data)
-        self._iso_visual.cmap = t
+    def remove(self):
+        """
+        Remove the layer artist for good
+        """
+        self._multivol.deallocate(self.id)
+        ARRAY_CACHE.pop(self.id, None)
+        PIXEL_CACHE.pop(self.id, None)
+
+    def _update_cmap_from_color(self):
+        cmap = get_translucent_cmap(*ColorConverter().to_rgb(self.state.color))
+        self._multivol.set_cmap(self.id, cmap)
         self.redraw()
 
-    def _update_data(self):
-
+    def _update_limits(self):
         if isinstance(self.layer, Subset):
-            try:
-                mask = self.layer.to_mask()
-            except IncompatibleAttribute:
-                mask = np.zeros(self.layer.data.shape, dtype=bool)
-            data = mask.astype(float)
+            self._multivol.set_clim(self.id, None)
         else:
-            data = self.layer[self.state.attribute]
+            self._multivol.set_clim(self.id, (self.state.vmin, self.state.vmax))
+        self.redraw()
 
-        if self._clip_limits is not None:
-            xmin, xmax, ymin, ymax, zmin, zmax = self._clip_limits
-            imin, imax = int(np.ceil(xmin)), int(np.ceil(xmax))
-            jmin, jmax = int(np.ceil(ymin)), int(np.ceil(ymax))
-            kmin, kmax = int(np.ceil(zmin)), int(np.ceil(zmax))
-            invalid = -np.inf
-            data = data.copy()
-            data[:, :, :imin] = invalid
-            data[:, :, imax:] = invalid
-            data[:, :jmin] = invalid
-            data[:, jmax:] = invalid
-            data[:kmin] = invalid
-            data[kmax:] = invalid
-
-        # self._iso_visual.set_data(np.nan_to_num(data).transpose())
-        gaussian_data = gaussian_filter(data/4, 1)
-
-        # TODO: the clim here conflict with set levels
-        # self._iso_visual.set_data(
-        # np.nan_to_num(gaussian_data),
-        # clim=(self.level_low, self.level_high))
-        # self._iso_visual.step = self.step
+    def _update_alpha(self):
+        self._multivol.set_weight(self.id, self.state.alpha)
+        self.redraw()
 
-        self._iso_visual.set_data(np.nan_to_num(gaussian_data))
+    def _update_subset_mode(self):
+        if isinstance(self.state.layer, Data) or self.state.subset_mode == 'outline':
+            self._multivol.set_multiply(self.id, None)
+        else:
+            label = self._multivol.label_for_layer(self.state.layer.data)
+            self._multivol.set_multiply(self.id, label)
         self.redraw()
 
+    def _update_data(self):
+
+        if self._data_proxy is None:
+            self._data_proxy = DataProxy(self._viewer_state, self)
+            self._multivol.set_data(self.id, self._data_proxy, layer=self.layer)
+        else:
+            self._multivol._update_scaled_data(self.id)
+
+        self._update_subset_mode()
+
     def _update_visibility(self):
-        # if self.visible:
-        #     self._iso_visual.parent =
-        # else:
-        #     self._multivol.disable(self.id)
+        if self.state.visible:
+            self._multivol.enable(self.id)
+        else:
+            self._multivol.disable(self.id)
         self.redraw()
 
     def set_clip(self, limits):
-        self._clip_limits = limits
-        self._update_data()
+        pass
 
     def _update_volume(self, force=False, **kwargs):
 
         if self.state.attribute is None or self.state.layer is None:
             return
 
         # Figure out which attributes are different from before. Ideally we shouldn't
@@ -198,22 +222,28 @@
             for key, value in self.state.as_dict().items():
                 if value != self._last_layer_state.get(key, None):
                     changed.add(key)
 
         self._last_viewer_state.update(self._viewer_state.as_dict())
         self._last_layer_state.update(self.state.as_dict())
 
-        if force or len(changed & DATA_PROPERTIES) > 0:
-            self._update_data()
+        if force or 'color' in changed:
+            self._update_cmap_from_color()
 
-        if force or len(changed & LEVEL_PROPERTIES) > 0:
-            self._update_level()
+        if force or 'vmin' in changed or 'vmax' in changed:
+            self._update_limits()
+
+        if force or 'alpha' in changed:
+            self._update_alpha()
+
+        if force or 'layer' in changed or 'attribute' in changed:
+            self._update_data()
 
-        if force or len(changed & COLOR_PROPERTIES) > 0:
-            self._update_color()
+        if force or 'subset_mode' in changed:
+            self._update_subset_mode()
 
-        if force or len(changed & STEP_PROPERTIES) > 0:
-            self._update_step()
+        if force or 'visible' in changed:
+            self._update_visibility()
 
     def update(self):
         self._update_volume(force=True)
         self.redraw()
```

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/isosurface/layer_style_widget.ui` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/qt/layer_style_widget.ui`

 * *Files 8% similar despite different names*

#### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/isosurface/layer_style_widget.ui` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/qt/layer_style_widget.ui`

```diff
@@ -2,111 +2,107 @@
 <ui version="4.0">
   <class>Form</class>
   <widget class="QWidget" name="Form">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>240</width>
-        <height>177</height>
+        <width>212</width>
+        <height>106</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>Form</string>
     </property>
     <layout class="QGridLayout" name="gridLayout">
       <property name="verticalSpacing">
         <number>5</number>
       </property>
       <property name="margin">
         <number>5</number>
       </property>
+      <item row="2" column="2">
+        <widget class="QSlider" name="value_alpha">
+          <property name="maximum">
+            <number>100</number>
+          </property>
+          <property name="orientation">
+            <enum>Qt::Horizontal</enum>
+          </property>
+        </widget>
+      </item>
+      <item row="3" column="1">
+        <widget class="QRadioButton" name="radio_subset_data">
+          <property name="text">
+            <string>Data</string>
+          </property>
+        </widget>
+      </item>
       <item row="0" column="0">
         <widget class="QLabel" name="label">
           <property name="text">
             <string>Attribute:</string>
           </property>
         </widget>
       </item>
-      <item row="2" column="0" colspan="4">
-        <layout class="QHBoxLayout" name="horizontalLayout">
-          <item>
-            <widget class="QLabel" name="label_3">
-              <property name="text">
-                <string>Limits:</string>
-              </property>
-            </widget>
-          </item>
-          <item>
-            <widget class="QLineEdit" name="valuetext_level_low"/>
-          </item>
-          <item>
-            <widget class="QLineEdit" name="valuetext_level_high">
-              <property name="text">
-                <string>2</string>
-              </property>
-            </widget>
-          </item>
-        </layout>
+      <item row="2" column="0">
+        <widget class="QLabel" name="label_2">
+          <property name="text">
+            <string>Color:</string>
+          </property>
+        </widget>
+      </item>
+      <item row="3" column="0">
+        <widget class="QLabel" name="label_subset_mode">
+          <property name="text">
+            <string>Subset:</string>
+          </property>
+        </widget>
+      </item>
+      <item row="1" column="1">
+        <widget class="QLineEdit" name="valuetext_vmin"/>
+      </item>
+      <item row="2" column="1">
+        <widget class="QColorBox" name="color_color">
+          <property name="sizePolicy">
+            <sizepolicy hsizetype="Preferred" vsizetype="Minimum">
+              <horstretch>0</horstretch>
+              <verstretch>0</verstretch>
+            </sizepolicy>
+          </property>
+          <property name="text">
+            <string/>
+          </property>
+        </widget>
       </item>
-      <item row="0" column="1" colspan="3">
+      <item row="1" column="0">
+        <widget class="QLabel" name="label_limits">
+          <property name="text">
+            <string>Limits:</string>
+          </property>
+        </widget>
+      </item>
+      <item row="1" column="2">
+        <widget class="QLineEdit" name="valuetext_vmax"/>
+      </item>
+      <item row="0" column="1" colspan="2">
         <widget class="QComboBox" name="combosel_attribute">
           <property name="sizeAdjustPolicy">
             <enum>QComboBox::AdjustToMinimumContentsLengthWithIcon</enum>
           </property>
         </widget>
       </item>
-      <item row="3" column="0" colspan="3">
-        <layout class="QHBoxLayout" name="horizontalLayout_3">
-          <item>
-            <widget class="QLabel" name="label_4">
-              <property name="text">
-                <string>Step:</string>
-              </property>
-            </widget>
-          </item>
-          <item>
-            <widget class="QSlider" name="value_step">
-              <property name="minimum">
-                <number>1</number>
-              </property>
-              <property name="maximum">
-                <number>10</number>
-              </property>
-              <property name="singleStep">
-                <number>1</number>
-              </property>
-              <property name="value">
-                <number>5</number>
-              </property>
-              <property name="orientation">
-                <enum>Qt::Horizontal</enum>
-              </property>
-            </widget>
-          </item>
-          <item>
-            <widget class="QLineEdit" name="valuetext_step"/>
-          </item>
-        </layout>
-      </item>
-      <item row="4" column="0" colspan="4">
-        <layout class="QHBoxLayout" name="horizontalLayout_2">
-          <item>
-            <widget class="QLabel" name="label_2">
-              <property name="text">
-                <string>Color:</string>
-              </property>
-            </widget>
-          </item>
-          <item>
-            <widget class="QColormapCombo" name="combodata_cmap"/>
-          </item>
-        </layout>
+      <item row="3" column="2">
+        <widget class="QRadioButton" name="radio_subset_outline">
+          <property name="text">
+            <string>Outline</string>
+          </property>
+        </widget>
       </item>
-      <item row="5" column="0">
+      <item row="4" column="1">
         <spacer name="verticalSpacer">
           <property name="orientation">
             <enum>Qt::Vertical</enum>
           </property>
           <property name="sizeHint" stdset="0">
             <size>
               <width>20</width>
@@ -115,15 +111,15 @@
           </property>
         </spacer>
       </item>
     </layout>
   </widget>
   <customwidgets>
     <customwidget>
-      <class>QColormapCombo</class>
-      <extends>QComboBox</extends>
+      <class>QColorBox</class>
+      <extends>QLabel</extends>
       <header>glue_qt.utils.colors</header>
     </customwidget>
   </customwidgets>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/scatter/layer_artist.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/layer_artist.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,16 +60,16 @@
             multiscat = MultiColorScatter()
             multiscat.set_gl_state(depth_test=False,
                                    blend=True,
                                    blend_func=('src_alpha', 'one_minus_src_alpha'))
 
             self.vispy_widget.add_data_visual(multiscat)
             self.vispy_widget._multiscat = multiscat
-            vispy_viewer.options.ui.label_line_width.show()
-            vispy_viewer.options.ui.value_line_width.show()
+            # vispy_viewer.options.ui.label_line_width.show()
+            # vispy_viewer.options.ui.value_line_width.show()
 
         self._multiscat = self.vispy_widget._multiscat
         self._multiscat.allocate(self.id)
         self._multiscat.set_zorder(self.id, self.get_zorder)
 
         # Watch for changes in the viewer state which would require the
         # layers to be redrawn
```

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/scatter/layer_state.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/layer_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 
 
 class ScatterLayerState(VispyLayerState):
     """
     A state object for volume layers
     """
 
-    size_mode = CallbackProperty('Fixed')
+    size_mode = SelectionCallbackProperty()
     size = CallbackProperty()
     size_attribute = SelectionCallbackProperty()
     size_vmin = CallbackProperty()
     size_vmax = CallbackProperty()
     size_scaling = CallbackProperty(1)
 
-    color_mode = CallbackProperty('Fixed')
+    color_mode = SelectionCallbackProperty()
     cmap_attribute = SelectionCallbackProperty()
     cmap_vmin = CallbackProperty()
     cmap_vmax = CallbackProperty()
     cmap = CallbackProperty()
 
     xerr_visible = CallbackProperty(False)
     xerr_attribute = SelectionCallbackProperty()
@@ -36,46 +36,49 @@
     vx_attribute = SelectionCallbackProperty()
     vy_attribute = SelectionCallbackProperty()
     vz_attribute = SelectionCallbackProperty()
     vector_scaling = CallbackProperty(1)
     vector_origin = SelectionCallbackProperty(default_index=1)
     vector_arrowhead = CallbackProperty()
 
-    size_limits_cache = CallbackProperty({})
-    cmap_limits_cache = CallbackProperty({})
+    _size_limits_cache = CallbackProperty({})
+    _cmap_limits_cache = CallbackProperty({})
 
     def __init__(self, layer=None, **kwargs):
 
         self._sync_markersize = None
 
         super(ScatterLayerState, self).__init__(layer=layer)
 
         if self.layer is not None:
 
             self.color = self.layer.style.color
             self.size = self.layer.style.markersize
             self.alpha = self.layer.style.alpha
 
+        ScatterLayerState.color_mode.set_choices(self, ['Fixed', 'Linear'])
+        ScatterLayerState.size_mode.set_choices(self, ['Fixed', 'Linear'])
+
         self.size_att_helper = ComponentIDComboHelper(self, 'size_attribute')
         self.cmap_att_helper = ComponentIDComboHelper(self, 'cmap_attribute')
         self.xerr_att_helper = ComponentIDComboHelper(self, 'xerr_attribute', categorical=False)
         self.yerr_att_helper = ComponentIDComboHelper(self, 'yerr_attribute', categorical=False)
         self.zerr_att_helper = ComponentIDComboHelper(self, 'zerr_attribute', categorical=False)
 
         self.vx_att_helper = ComponentIDComboHelper(self, 'vx_attribute', categorical=False)
         self.vy_att_helper = ComponentIDComboHelper(self, 'vy_attribute', categorical=False)
         self.vz_att_helper = ComponentIDComboHelper(self, 'vz_attribute', categorical=False)
 
         self.size_lim_helper = StateAttributeLimitsHelper(self, attribute='size_attribute',
                                                           lower='size_vmin', upper='size_vmax',
-                                                          cache=self.size_limits_cache)
+                                                          cache=self._size_limits_cache)
 
         self.cmap_lim_helper = StateAttributeLimitsHelper(self, attribute='cmap_attribute',
                                                           lower='cmap_vmin', upper='cmap_vmax',
-                                                          cache=self.cmap_limits_cache)
+                                                          cache=self._cmap_limits_cache)
 
         vector_origin_display = {'tail': 'Tail of vector',
                                  'middle': 'Middle of vector',
                                  'tip': 'Tip of vector'}
         ScatterLayerState.vector_origin.set_choices(self, ['tail', 'middle', 'tip'])
         ScatterLayerState.vector_origin.set_display_func(self, vector_origin_display.get)
```

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/scatter/layer_style_widget.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/qt/layer_style_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 from qtpy import QtWidgets
 
 from glue_qt.utils import load_ui
 from echo.qt import autoconnect_callbacks_to_qt
 
-from glue_vispy_viewers.utils import fix_tab_widget_fontsize
+from glue_qt.utils.app import fix_tab_widget_fontsize
 
 
 class ScatterLayerStyleWidget(QtWidgets.QWidget):
 
     def __init__(self, layer_artist):
 
         super(ScatterLayerStyleWidget, self).__init__()
```

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/scatter/layer_style_widget.ui` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/qt/layer_style_widget.ui`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/scatter/multi_scatter.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/multi_scatter.py`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/scatter/scatter_toolbar.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/scatter_toolbar.py`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/scatter/tests/test_scatter_viewer.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/qt/tests/test_scatter_viewer.py`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/scatter/viewer_state.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/scatter/viewer_state.py`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/tests/data/multiple_volumes_v1.glu` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/qt/tests/data/multiple_volumes_v1.glu`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/tests/data/multiple_volumes_v2.glu` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/qt/tests/data/multiple_volumes_v2.glu`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/tests/data/scatter_volume_selection.glu` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/qt/tests/data/scatter_volume_selection.glu`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/tests/data/scatter_volume_v0.glu` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/qt/tests/data/scatter_volume_v0.glu`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/tests/data/scatter_volume_v1.glu` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/qt/tests/data/scatter_volume_v1.glu`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/tests/test_session_back_compat.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/qt/tests/test_session_back_compat.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Make sure that session files can be read in a backward-compatible manner
 
 import os
 import pytest
-from mock import patch
+from unittest.mock import patch
 
 import numpy as np
 from numpy.testing import assert_equal
 
 from glue.core.state import GlueUnSerializer
 
-from ..volume.volume_viewer import QMessageBox
+from qtpy.QtWidgets import QMessageBox
 
 DATA = os.path.join(os.path.dirname(__file__), 'data')
 
 
 @pytest.mark.parametrize('protocol', [0, 1])
 def test_scatter_volume(protocol):
```

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/utils.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,33 +31,14 @@
         return transform.as_matrix()
     elif isinstance(transform, MatrixTransform):
         return transform
     else:
         raise TypeError("Could not simplify transform of type {0}".format(type(transform)))
 
 
-try:
-
-    from glue_qt.utils import fix_tab_widget_fontsize  # noqa
-
-except ImportError:
-
-    import platform
-    from glue_qt.utils import get_qapp
-
-    def fix_tab_widget_fontsize(tab_widget):
-        """
-        Because of a bug in Qt, tab titles on MacOS X don't have the right font size
-        """
-        if platform.system() == 'Darwin':
-            app = get_qapp()
-            app_font = app.font()
-            tab_widget.setStyleSheet('font-size: {0}px'.format(app_font.pointSize()))
-
-
 class NestedSTTransform(STTransform):
 
     glsl_map = """
         vec4 st_transform_map(vec4 pos) {
             return vec4((pos.xyz * $innerscale.xyz + $innertranslate.xyz * pos.w).xyz
                          * $scale.xyz + $translate.xyz * pos.w, pos.w);
         }
```

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/volume/layer_state.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/layer_state.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,30 +13,30 @@
     A state object for volume layers
     """
 
     attribute = SelectionCallbackProperty()
     vmin = CallbackProperty()
     vmax = CallbackProperty()
     subset_mode = CallbackProperty('data')
-    limits_cache = CallbackProperty({})
+    _limits_cache = CallbackProperty({})
 
     def __init__(self, layer=None, **kwargs):
 
         super(VolumeLayerState, self).__init__(layer=layer)
 
         if self.layer is not None:
 
             self.color = self.layer.style.color
             self.alpha = self.layer.style.alpha
 
         self.att_helper = ComponentIDComboHelper(self, 'attribute')
 
         self.lim_helper = StateAttributeLimitsHelper(self, attribute='attribute',
                                                      lower='vmin', upper='vmax',
-                                                     cache=self.limits_cache)
+                                                     cache=self._limits_cache)
 
         self.add_callback('layer', self._on_layer_change)
         if layer is not None:
             self._on_layer_change()
 
         if isinstance(self.layer, Subset):
             self.vmin = 0
```

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/volume/layer_style_widget.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/qt/layer_style_widget.py`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/volume/shaders.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/shaders.py`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/volume/tests/test_volume_toolbar.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/qt/tests/test_volume_toolbar.py`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/volume/tests/test_volume_viewer.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/qt/tests/test_volume_viewer.py`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/volume/viewer_state.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/viewer_state.py`

 * *Files identical despite different names*

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/volume/volume_toolbar.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/volume_toolbar.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,29 +21,32 @@
 
     icon = 'glue_point'
     tool_id = 'volume3d:floodfill'
     action_text = 'Select volume using a floodfill selection'
 
     def __init__(self, viewer):
         super(FloodFillSelectionMode, self).__init__(viewer)
-        self.markers = Markers(parent=self._vispy_widget.view.scene)
         self.subset_state = None
 
     def release(self, event):
         pass
 
-    def deactivate(self):
-        self.markers.visible = False
+    def reset(self):
+        if hasattr(self, 'markers'):
+            self.markers.visible = False
 
     def press(self, event):
         """
         Assign mouse position and do point selection.
         :param event:
         """
 
+        if not hasattr(self, 'markers'):
+            self.markers = Markers(parent=self._vispy_widget.view.scene)
+
         if event.button == 1:
 
             self.selection_origin = event.pos
 
             self.visible_data, self.visual = self.get_visible_data()
 
             # Get the values of the currently active layer artist - we
```

### Comparing `glue-vispy-viewers-1.1.0/glue_vispy_viewers/volume/volume_visual.py` & `glue_vispy_viewers-1.2.1/glue_vispy_viewers/volume/volume_visual.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,30 +32,27 @@
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 # ===========================================================================
 #
 # This modified version is released under the BSD license given in the LICENSE
 # file in this repository.
 
-from distutils.version import LooseVersion
 from collections import defaultdict
 
 import numpy as np
 from glue.utils import iterate_chunks
 
 from vispy.gloo import Texture3D, TextureEmulated3D, VertexBuffer, IndexBuffer
 from vispy.visuals import VolumeVisual, Visual
 from vispy.visuals.shaders import Function
 from vispy.color import get_colormap, Color
 from vispy.scene.visuals import create_visual_node
 
 from .shaders import get_frag_shader, VERT_SHADER
 
-NUMPY_LT_1_13 = LooseVersion(np.__version__) < LooseVersion('1.13')
-
 
 class NoFreeSlotsError(Exception):
     pass
 
 
 class MultiVolumeVisual(VolumeVisual):
     """
```

### Comparing `glue-vispy-viewers-1.1.0/setup.cfg` & `glue_vispy_viewers-1.2.1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,65 @@
 [metadata]
 name = glue-vispy-viewers
 url = https://github.com/glue-viz/glue-3d-viewer
 author = Thomas Robitaille, Penny Qian, and Maxwell Tsai
 author_email = glueviz@gmail.com
 description = Vispy-based viewers for Glue
 long_description = file: README.rst
+long_description_content_type = text/x-rst
 
 [options]
 zip_safe = True
 packages = find:
 setup_requires = setuptools_scm
 install_requires = 
 	numpy
 	pyopengl
 	glue-core>=1.13.1
-	glue-qt>=0.1.0
 	echo>=0.6
-	qtpy
 	scipy
 	matplotlib
 	vispy>=0.9.1
 	importlib_metadata>=3.6; python_version<'3.10'
+	glfw
+	imageio
 python_requires = >=3.8
 
 [options.entry_points]
 glue.plugins = 
-	vispy_volume = glue_vispy_viewers.volume:setup
-	vispy_scatter = glue_vispy_viewers.scatter:setup
+	vispy_volume = glue_vispy_viewers.volume.qt:setup
+	vispy_scatter = glue_vispy_viewers.scatter.qt:setup
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-cov
-	pytest-qt
 	pytest-faulthandler
 	objgraph;sys_platform!='win32'
 	mock
-qt = 
-	PyQt5>=5.9
-all = 
-	imageio
+pyqt = 
+	qtpy
+	glue-qt>=0.1.0
+	PyQt6
+pyside = 
+	qtpy
+	glue-qt>=0.1.0
+	PySide6
+jupyter = 
+	glue-jupyter
+	jupyter_rfb
 
 [options.package_data]
-glue_vispy_viewers.common = *.ui, *.png
-glue_vispy_viewers.isosurface = *.ui
-glue_vispy_viewers.scatter = *.ui
-glue_vispy_viewers.volume = *.ui
-glue_vispy_viewers.tests = data/*.glu
+glue_vispy_viewers.common = *.png
+glue_vispy_viewers.common.qt = *.ui, *.png
+glue_vispy_viewers.scatter.qt = *.ui
+glue_vispy_viewers.volume.qt = *.ui
+glue_vispy_viewers.scatter.jupyter = *.vue
+glue_vispy_viewers.volume.jupyter = *.vue
+glue_vispy_viewers.qt.tests = data/*.glu
 glue_vispy_viewers.extern = README.md, VISPY_LICENSE
 glue_vispy_viewers.extern.vispy = io/_data/*.npy, html/static/js/*.js, app/tests/*.ui
 glue_vispy_viewers.extern.vispy.glsl.antialias = *.vert, *.frag, *.glsl
 glue_vispy_viewers.extern.vispy.glsl.arrowheads = *.vert, *.frag, *.glsl
 glue_vispy_viewers.extern.vispy.glsl.arrows = *.vert, *.frag, *.glsl
 glue_vispy_viewers.extern.vispy.glsl.collections = *.vert, *.frag, *.glsl
 glue_vispy_viewers.extern.vispy.glsl.colormaps = *.vert, *.frag, *.glsl
```

### Comparing `glue-vispy-viewers-1.1.0/tox.ini` & `glue_vispy_viewers-1.2.1/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 [tox]
 envlist =
-    py{38,39,310,311}-{test}-{dev}{,-pyqt6}
+    py{38,39,310,311}-{test}-{dev}{,pyqt63,pyside63,pyqt64,pyside64,jupyter}
     codestyle
 requires = pip >= 18.0
            setuptools >= 30.3.0
 
 [testenv]
 passenv =
     DISPLAY
     HOME
 changedir =
     test: .tmp/{envname}
 deps =
-    !pyqt6: PyQt5==5.15.*
-    pyqt6: PyQt6==6.4.*
+    pyqt63: PyQt6==6.3.*
+    pyside63: PySide6==6.3.*
+    pyqt64: PyQt6==6.4.*
+    pyside64: PySide6==6.4.*
     dev: glue-core @ git+https://github.com/glue-viz/glue
     dev: vispy @ git+https://github.com/vispy/vispy
 extras =
     test: test
+    pyqt63,pyqt64: pyqt
+    pyside63,pyside64: pyside
+    jupyter: jupyter
 commands =
     test: pip freeze
     test: pytest --pyargs glue_vispy_viewers --cov glue_vispy_viewers {posargs}
 
 [testenv:codestyle]
 deps = flake8
 skip_install = true
```

