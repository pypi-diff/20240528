# Comparing `tmp/dcnum-0.20.0.tar.gz` & `tmp/dcnum-0.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcnum-0.20.0.tar", last modified: Mon May 27 12:51:47 2024, max compression
+gzip compressed data, was "dcnum-0.20.1.tar", last modified: Tue May 28 05:41:05 2024, max compression
```

## Comparing `dcnum-0.20.0.tar` & `dcnum-0.20.1.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.634594 dcnum-0.20.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.614594 dcnum-0.20.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.614594 dcnum-0.20.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-27 12:51:42.000000 dcnum-0.20.0/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-27 12:51:42.000000 dcnum-0.20.0/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-27 12:51:42.000000 dcnum-0.20.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-27 12:51:42.000000 dcnum-0.20.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-05-27 12:51:42.000000 dcnum-0.20.0/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-27 12:51:42.000000 dcnum-0.20.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-27 12:51:47.634594 dcnum-0.20.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-27 12:51:42.000000 dcnum-0.20.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.618594 dcnum-0.20.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-27 12:51:42.000000 dcnum-0.20.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.618594 dcnum-0.20.0/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-27 12:51:42.000000 dcnum-0.20.0/docs/extensions/github_changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-27 12:51:42.000000 dcnum-0.20.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-27 12:51:42.000000 dcnum-0.20.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-27 12:51:42.000000 dcnum-0.20.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 12:51:47.634594 dcnum-0.20.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.614594 dcnum-0.20.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.618594 dcnum-0.20.0/src/dcnum/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-27 12:51:47.000000 dcnum-0.20.0/src/dcnum/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.618594 dcnum-0.20.0/src/dcnum/feat/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/event_extractor_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.618594 dcnum-0.20.0/src/dcnum/feat/feat_background/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_background/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_background/bg_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13175 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_background/bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (127)    20709 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_background/bg_sparse_median.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.618594 dcnum-0.20.0/src/dcnum/feat/feat_brightness/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_brightness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_brightness/bright_all.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_brightness/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.622594 dcnum-0.20.0/src/dcnum/feat/feat_contour/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_contour/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_contour/contour.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_contour/moments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_contour/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.622594 dcnum-0.20.0/src/dcnum/feat/feat_texture/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_texture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_texture/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/feat_texture/tex_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/gate.py
--rw-r--r--   0 runner    (1001) docker     (127)    15644 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/feat/queue_event_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.622594 dcnum-0.20.0/src/dcnum/logic/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34405 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/logic/ctrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/logic/job.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/logic/json_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.622594 dcnum-0.20.0/src/dcnum/meta/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/meta/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/meta/ppid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.622594 dcnum-0.20.0/src/dcnum/read/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/read/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/read/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    23489 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/read/hdf5_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/read/mapped.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.622594 dcnum-0.20.0/src/dcnum/segm/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/segm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/segm/segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (127)    12220 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/segm/segmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10690 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/segm/segmenter_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/segm/segmenter_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/segm/segmenter_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.626594 dcnum-0.20.0/src/dcnum/write/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/write/deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/write/queue_collector_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)    15601 2024-05-27 12:51:42.000000 dcnum-0.20.0/src/dcnum/write/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.634594 dcnum-0.20.0/src/dcnum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-27 12:51:47.000000 dcnum-0.20.0/src/dcnum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-27 12:51:47.000000 dcnum-0.20.0/src/dcnum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 12:51:47.000000 dcnum-0.20.0/src/dcnum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-27 12:51:47.000000 dcnum-0.20.0/src/dcnum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 12:51:47.000000 dcnum-0.20.0/src/dcnum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.630594 dcnum-0.20.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 12:51:47.634594 dcnum-0.20.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip
--rw-r--r--   0 runner    (1001) docker     (127)   650653 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
--rw-r--r--   0 runner    (1001) docker     (127)   284743 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/data/fmt-hdf5_cytoshot_full-features_2024.zip
--rw-r--r--   0 runner    (1001) docker     (127)   154010 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/data/fmt-hdf5_shapein_empty.zip
--rw-r--r--   0 runner    (1001) docker     (127)   275920 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_feat_background_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_feat_background_bg_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_feat_background_bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_feat_background_bg_sparsemed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_feat_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_feat_event_extractor_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_feat_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_feat_haralick.py
--rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_feat_moments_based.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_feat_moments_based_extended.py
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_feat_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_logic_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_logic_join.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_logic_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    35480 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_logic_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_meta_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_meta_ppid_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_meta_ppid_bg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_meta_ppid_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_meta_ppid_feat.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_meta_ppid_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_meta_ppid_segm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_read_basin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_read_concat_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)    11771 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_read_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_read_hdf5_basins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_read_hdf5_index_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    14336 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_segm_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_segm_no_mask_proc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_write_deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_write_queue_collector_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-05-27 12:51:42.000000 dcnum-0.20.0/tests/test_write_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:41:05.180303 dcnum-0.20.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:41:05.160302 dcnum-0.20.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:41:05.164302 dcnum-0.20.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-28 05:40:59.000000 dcnum-0.20.1/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-28 05:40:59.000000 dcnum-0.20.1/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-28 05:40:59.000000 dcnum-0.20.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-28 05:40:59.000000 dcnum-0.20.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    12486 2024-05-28 05:40:59.000000 dcnum-0.20.1/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-28 05:40:59.000000 dcnum-0.20.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-28 05:41:05.180303 dcnum-0.20.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-28 05:40:59.000000 dcnum-0.20.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:41:05.164302 dcnum-0.20.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-28 05:40:59.000000 dcnum-0.20.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:41:05.164302 dcnum-0.20.1/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-28 05:40:59.000000 dcnum-0.20.1/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-28 05:40:59.000000 dcnum-0.20.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 05:40:59.000000 dcnum-0.20.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-28 05:40:59.000000 dcnum-0.20.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 05:41:05.180303 dcnum-0.20.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:41:05.160302 dcnum-0.20.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:41:05.164302 dcnum-0.20.1/src/dcnum/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-28 05:41:05.000000 dcnum-0.20.1/src/dcnum/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:41:05.164302 dcnum-0.20.1/src/dcnum/feat/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/feat/event_extractor_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:41:05.164302 dcnum-0.20.1/src/dcnum/feat/feat_background/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/feat/feat_background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/feat/feat_background/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/feat/feat_background/bg_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13175 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/feat/feat_background/bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20709 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/feat/feat_background/bg_sparse_median.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:41:05.164302 dcnum-0.20.1/src/dcnum/feat/feat_brightness/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/feat/feat_brightness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/feat/feat_brightness/bright_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/feat/feat_brightness/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:41:05.168302 dcnum-0.20.1/src/dcnum/feat/feat_contour/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/feat/feat_contour/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/feat/feat_contour/contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/feat/feat_contour/moments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/feat/feat_contour/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:41:05.168302 dcnum-0.20.1/src/dcnum/feat/feat_texture/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/feat/feat_texture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/feat/feat_texture/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/feat/feat_texture/tex_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/feat/gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15644 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/feat/queue_event_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:41:05.168302 dcnum-0.20.1/src/dcnum/logic/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34412 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/logic/ctrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/logic/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/logic/json_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:41:05.168302 dcnum-0.20.1/src/dcnum/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/meta/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/meta/ppid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:41:05.168302 dcnum-0.20.1/src/dcnum/read/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/read/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/read/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23489 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/read/hdf5_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/read/mapped.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:41:05.168302 dcnum-0.20.1/src/dcnum/segm/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/segm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/segm/segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12220 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/segm/segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10690 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/segm/segmenter_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/segm/segmenter_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/segm/segmenter_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:41:05.168302 dcnum-0.20.1/src/dcnum/write/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/write/deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/write/queue_collector_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15601 2024-05-28 05:40:59.000000 dcnum-0.20.1/src/dcnum/write/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:41:05.176303 dcnum-0.20.1/src/dcnum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-28 05:41:05.000000 dcnum-0.20.1/src/dcnum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-28 05:41:05.000000 dcnum-0.20.1/src/dcnum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 05:41:05.000000 dcnum-0.20.1/src/dcnum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-28 05:41:05.000000 dcnum-0.20.1/src/dcnum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 05:41:05.000000 dcnum-0.20.1/src/dcnum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:41:05.176303 dcnum-0.20.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:41:05.176303 dcnum-0.20.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   650653 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   284743 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/data/fmt-hdf5_cytoshot_full-features_2024.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   154010 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/data/fmt-hdf5_shapein_empty.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   275920 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_feat_background_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_feat_background_bg_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_feat_background_bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_feat_background_bg_sparsemed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_feat_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_feat_event_extractor_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_feat_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_feat_haralick.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_feat_moments_based.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_feat_moments_based_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_feat_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_logic_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_logic_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_logic_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37009 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_logic_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_meta_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_meta_ppid_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_meta_ppid_bg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_meta_ppid_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_meta_ppid_feat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_meta_ppid_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_meta_ppid_segm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_read_basin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_read_concat_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11771 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_read_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_read_hdf5_basins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_read_hdf5_index_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14336 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_segm_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_segm_no_mask_proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_write_deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_write_queue_collector_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-05-28 05:40:59.000000 dcnum-0.20.1/tests/test_write_writer.py
```

### Comparing `dcnum-0.20.0/.github/workflows/check.yml` & `dcnum-0.20.1/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/.github/workflows/deploy_pypi.yml` & `dcnum-0.20.1/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/.gitignore` & `dcnum-0.20.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/CHANGELOG` & `dcnum-0.20.1/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+0.20.1
+ - fix: relative basin locations not written correctly
+ - enh: increase deque size threshold for waiting for writer
 0.20.0
  - feat: support reading mapped basins
  - feat: support writing mapped-basin-based output files
  - fix: copy "bg_off" data to output file when copying background data
  - enh: allow to slice BaseImageChunkCache
  - enh: sort logs, tables and basins for reproducible access
  - enh: add more timing information in logs
```

### Comparing `dcnum-0.20.0/LICENSE` & `dcnum-0.20.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/PKG-INFO` & `dcnum-0.20.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.20.0
+Version: 0.20.1
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Maximilian Schlögel, Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.20.0/README.rst` & `dcnum-0.20.1/README.rst`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/docs/conf.py` & `dcnum-0.20.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/docs/extensions/github_changelog.py` & `dcnum-0.20.1/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/pyproject.toml` & `dcnum-0.20.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/feat/event_extractor_manager_thread.py` & `dcnum-0.20.1/src/dcnum/feat/event_extractor_manager_thread.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,16 +92,16 @@
         num_slots = len(self.slot_states)
         chunks_processed = 0
         frames_processed = 0
         while True:
             # If the writer_dq starts filling up, then this could lead to
             # an oom-kill signal. Stall for the writer to prevent this.
             ldq = len(self.writer_dq)
-            if ldq > 100:
-                stallsec = ldq / 100
+            if ldq > 1000:
+                stallsec = ldq / 1000
                 self.logger.warning(
                     f"Stalling {stallsec:.1f}s for slow writer")
                 time.sleep(stallsec)
 
             cur_slot = 0
             unavailable_slots = 0
             # Check all slots for segmented labels
```

### Comparing `dcnum-0.20.0/src/dcnum/feat/feat_background/base.py` & `dcnum-0.20.1/src/dcnum/feat/feat_background/base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/feat/feat_background/bg_copy.py` & `dcnum-0.20.1/src/dcnum/feat/feat_background/bg_copy.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/feat/feat_background/bg_roll_median.py` & `dcnum-0.20.1/src/dcnum/feat/feat_background/bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/feat/feat_background/bg_sparse_median.py` & `dcnum-0.20.1/src/dcnum/feat/feat_background/bg_sparse_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/feat/feat_brightness/bright_all.py` & `dcnum-0.20.1/src/dcnum/feat/feat_brightness/bright_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/feat/feat_contour/moments.py` & `dcnum-0.20.1/src/dcnum/feat/feat_contour/moments.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/feat/feat_contour/volume.py` & `dcnum-0.20.1/src/dcnum/feat/feat_contour/volume.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/feat/feat_texture/tex_all.py` & `dcnum-0.20.1/src/dcnum/feat/feat_texture/tex_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/feat/gate.py` & `dcnum-0.20.1/src/dcnum/feat/gate.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/feat/queue_event_extractor.py` & `dcnum-0.20.1/src/dcnum/feat/queue_event_extractor.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/logic/ctrl.py` & `dcnum-0.20.1/src/dcnum/logic/ctrl.py`

 * *Files 1% similar despite different names*

```diff
@@ -609,15 +609,15 @@
                 else:
                     # TAP: Create basins for the "optional" features in the
                     # output file. Note that the "critical" features never
                     # reach this case.
                     self.logger.debug(f"Creating basin for {feats}")
                     # Relative and absolute paths.
                     pin = pathlib.Path(hin.filename).resolve()
-                    pout = pathlib.Path(hout.filename).resolve()
+                    pout = pathlib.Path(hout.filename).resolve().parent
                     paths = [pin, os.path.relpath(pin, pout)]
                     hw.store_basin(name="dcnum basin",
                                    features=feats,
                                    mapping=basinmap,
                                    paths=paths,
                                    description=f"Created with dcnum {version}",
                                    )
```

### Comparing `dcnum-0.20.0/src/dcnum/logic/job.py` & `dcnum-0.20.1/src/dcnum/logic/job.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/logic/json_encoder.py` & `dcnum-0.20.1/src/dcnum/logic/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/meta/paths.py` & `dcnum-0.20.1/src/dcnum/meta/paths.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/meta/ppid.py` & `dcnum-0.20.1/src/dcnum/meta/ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/read/cache.py` & `dcnum-0.20.1/src/dcnum/read/cache.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/read/hdf5_data.py` & `dcnum-0.20.1/src/dcnum/read/hdf5_data.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/read/mapped.py` & `dcnum-0.20.1/src/dcnum/read/mapped.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/segm/segm_thresh.py` & `dcnum-0.20.1/src/dcnum/segm/segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/segm/segmenter.py` & `dcnum-0.20.1/src/dcnum/segm/segmenter.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/segm/segmenter_cpu.py` & `dcnum-0.20.1/src/dcnum/segm/segmenter_cpu.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/segm/segmenter_gpu.py` & `dcnum-0.20.1/src/dcnum/segm/segmenter_gpu.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/segm/segmenter_manager_thread.py` & `dcnum-0.20.1/src/dcnum/segm/segmenter_manager_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/write/deque_writer_thread.py` & `dcnum-0.20.1/src/dcnum/write/deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/write/queue_collector_thread.py` & `dcnum-0.20.1/src/dcnum/write/queue_collector_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum/write/writer.py` & `dcnum-0.20.1/src/dcnum/write/writer.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/src/dcnum.egg-info/PKG-INFO` & `dcnum-0.20.1/src/dcnum.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.20.0
+Version: 0.20.1
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Maximilian Schlögel, Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.20.0/src/dcnum.egg-info/SOURCES.txt` & `dcnum-0.20.1/src/dcnum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/conftest.py` & `dcnum-0.20.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip` & `dcnum-0.20.1/tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip` & `dcnum-0.20.1/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/data/fmt-hdf5_cytoshot_full-features_2024.zip` & `dcnum-0.20.1/tests/data/fmt-hdf5_cytoshot_full-features_2024.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip` & `dcnum-0.20.1/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/data/fmt-hdf5_shapein_empty.zip` & `dcnum-0.20.1/tests/data/fmt-hdf5_shapein_empty.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip` & `dcnum-0.20.1/tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/helper_methods.py` & `dcnum-0.20.1/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_feat_background_base.py` & `dcnum-0.20.1/tests/test_feat_background_base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_feat_background_bg_copy.py` & `dcnum-0.20.1/tests/test_feat_background_bg_copy.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_feat_background_bg_roll_median.py` & `dcnum-0.20.1/tests/test_feat_background_bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_feat_background_bg_sparsemed.py` & `dcnum-0.20.1/tests/test_feat_background_bg_sparsemed.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_feat_brightness.py` & `dcnum-0.20.1/tests/test_feat_brightness.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_feat_event_extractor_manager.py` & `dcnum-0.20.1/tests/test_feat_event_extractor_manager.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_feat_gate.py` & `dcnum-0.20.1/tests/test_feat_gate.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_feat_haralick.py` & `dcnum-0.20.1/tests/test_feat_haralick.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_feat_moments_based.py` & `dcnum-0.20.1/tests/test_feat_moments_based.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_feat_moments_based_extended.py` & `dcnum-0.20.1/tests/test_feat_moments_based_extended.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_feat_volume.py` & `dcnum-0.20.1/tests/test_feat_volume.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_logic_job.py` & `dcnum-0.20.1/tests/test_logic_job.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_logic_join.py` & `dcnum-0.20.1/tests/test_logic_join.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_logic_pipeline.py` & `dcnum-0.20.1/tests/test_logic_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,53 @@
         for feat in h5["events"]:
             assert len(h5["events"][feat]) == 275
         # The other features are accessed via basins
         hd = read.HDF5Data(h5)
         assert "image" in hd
 
 
+def test_basin_relative_path():
+    path_orig = retrieve_data("fmt-hdf5_cytoshot_full-features_2023.zip")
+    path = path_orig.with_name("input.rtdc")
+    path_out = path_orig.with_name("out.rtdc")
+    with read.concatenated_hdf5_data(5 * [path_orig], path_out=path):
+        pass
+
+    job = logic.DCNumPipelineJob(path_in=path,
+                                 path_out=path_out,
+                                 background_kwargs={"kernel_size": 150},
+                                 basin_strategy="tap",
+                                 debug=True)
+    with logic.DCNumJobRunner(job=job) as runner:
+        runner.run()
+
+    dir_new = path_orig.parent / "another_directory"
+    dir_new.mkdir()
+    path_new = dir_new / path.name
+    path_out_new = dir_new / path_out.name
+    path.rename(path_new)
+    path_out.rename(path_out_new)
+
+    # Everything should just work, because we have relative paths in the basin.
+    with h5py.File(path_out_new) as h5:
+        assert h5.attrs["pipeline:dcnum background"] \
+               == "sparsemed:k=150^s=1^t=0^f=0.8^o=1"
+        assert "image_bg" in h5["events"]
+        assert "bg_off" in h5["events"]
+        assert "deform" in h5["events"]
+        # the rest of the original features are basins!
+        assert "time" not in h5["events"]
+        assert "image" not in h5["events"]
+        for feat in h5["events"]:
+            assert len(h5["events"][feat]) == 275
+        # The other features are accessed via basins
+        hd = read.HDF5Data(h5)
+        assert "image" in hd
+
+
 def test_chained_pipeline():
     """Test running two pipelines consecutively"""
     path_orig = retrieve_data("fmt-hdf5_cytoshot_full-features_2023.zip")
     path = path_orig.with_name("input.rtdc")
     path2 = path.with_name("path_intermediate.rtdc")
     with read.concatenated_hdf5_data(5 * [path_orig], path_out=path):
         pass
```

### Comparing `dcnum-0.20.0/tests/test_meta_paths.py` & `dcnum-0.20.1/tests/test_meta_paths.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_meta_ppid_base.py` & `dcnum-0.20.1/tests/test_meta_ppid_base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_meta_ppid_bg.py` & `dcnum-0.20.1/tests/test_meta_ppid_bg.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_meta_ppid_data.py` & `dcnum-0.20.1/tests/test_meta_ppid_data.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_meta_ppid_feat.py` & `dcnum-0.20.1/tests/test_meta_ppid_feat.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_meta_ppid_gate.py` & `dcnum-0.20.1/tests/test_meta_ppid_gate.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_meta_ppid_segm.py` & `dcnum-0.20.1/tests/test_meta_ppid_segm.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_read_basin.py` & `dcnum-0.20.1/tests/test_read_basin.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_read_concat_hdf5.py` & `dcnum-0.20.1/tests/test_read_concat_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_read_hdf5.py` & `dcnum-0.20.1/tests/test_read_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_read_hdf5_basins.py` & `dcnum-0.20.1/tests/test_read_hdf5_basins.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_read_hdf5_index_mapping.py` & `dcnum-0.20.1/tests/test_read_hdf5_index_mapping.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_segm_base.py` & `dcnum-0.20.1/tests/test_segm_base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_segm_no_mask_proc.py` & `dcnum-0.20.1/tests/test_segm_no_mask_proc.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_segm_thresh.py` & `dcnum-0.20.1/tests/test_segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_write_deque_writer_thread.py` & `dcnum-0.20.1/tests/test_write_deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_write_queue_collector_thread.py` & `dcnum-0.20.1/tests/test_write_queue_collector_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.20.0/tests/test_write_writer.py` & `dcnum-0.20.1/tests/test_write_writer.py`

 * *Files identical despite different names*

