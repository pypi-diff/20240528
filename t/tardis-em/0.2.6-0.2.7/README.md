# Comparing `tmp/tardis_em-0.2.6.tar.gz` & `tmp/tardis_em-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tardis_em-0.2.6.tar", last modified: Fri May 24 08:27:36 2024, max compression
+gzip compressed data, was "tardis_em-0.2.7.tar", last modified: Tue May 28 16:44:16 2024, max compression
```

## Comparing `tardis_em-0.2.6.tar` & `tardis_em-0.2.7.tar`

### file list

```diff
@@ -1,129 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.661870 tardis_em-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-24 08:27:31.000000 tardis_em-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-24 08:27:31.000000 tardis_em-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-24 08:27:36.661870 tardis_em-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-05-24 08:27:31.000000 tardis_em-0.2.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-24 08:27:32.000000 tardis_em-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-24 08:27:32.000000 tardis_em-0.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-24 08:27:36.661870 tardis_em-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-24 08:27:32.000000 tardis_em-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.645870 tardis_em-0.2.6/tardis_em/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.645870 tardis_em-0.2.6/tardis_em/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/benchmarks/benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/benchmarks/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.645870 tardis_em-0.2.6/tardis_em/cnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/cnn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.645870 tardis_em-0.2.6/tardis_em/cnn/data_processing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/data_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12073 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/data_processing/draw_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/data_processing/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12894 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/data_processing/stitch.py
--rw-r--r--   0 runner    (1001) docker     (127)    13470 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/data_processing/trim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.649870 tardis_em-0.2.6/tardis_em/cnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/datasets/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    15300 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/datasets/build_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/datasets/dataloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.649870 tardis_em-0.2.6/tardis_em/cnn/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13542 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/model/convolution.py
--rw-r--r--   0 runner    (1001) docker     (127)    14686 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/model/decoder_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/model/encoder_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/model/init_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.649870 tardis_em-0.2.6/tardis_em/cnn/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18740 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/utils/build_cnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14593 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/cnn/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/compare_spatial_graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.649870 tardis_em-0.2.6/tardis_em/dist_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.649870 tardis_em-0.2.6/tardis_em/dist_pytorch/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/datasets/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    32154 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/datasets/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    20479 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/datasets/patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/dist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.649870 tardis_em-0.2.6/tardis_em/dist_pytorch/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/model/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    12217 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/model/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    30389 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/model/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/sparse_dist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.653870 tardis_em-0.2.6/tardis_em/dist_pytorch/sparse_model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/sparse_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/sparse_model/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/sparse_model/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/sparse_model/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     9399 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    29804 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.653870 tardis_em-0.2.6/tardis_em/dist_pytorch/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16498 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/utils/build_point_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    18487 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/utils/segment_point_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/dist_pytorch/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/predict_actin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/predict_mem.py
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/predict_mem_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/predict_mt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.653870 tardis_em-0.2.6/tardis_em/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16330 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/scripts/czi_predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/scripts/visualize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/tardis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.653870 tardis_em-0.2.6/tardis_em/tardis_helper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/tardis_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/tardis_helper/helper_func.py
--rw-r--r--   0 runner    (1001) docker     (127)    11061 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/train_DIST.py
--rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/train_cnn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.657870 tardis_em-0.2.6/tardis_em/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    20802 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/export_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    29405 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/logo.py
--rw-r--r--   0 runner    (1001) docker     (127)    20740 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/ota_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    53242 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/setup_envir.py
--rw-r--r--   0 runner    (1001) docker     (127)    38169 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/spline_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12260 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tardis_em/utils/visualize_pc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.661870 tardis_em-0.2.6/tardis_em.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-24 08:27:36.000000 tardis_em-0.2.6/tardis_em.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-24 08:27:36.000000 tardis_em-0.2.6/tardis_em.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 08:27:36.000000 tardis_em-0.2.6/tardis_em.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-24 08:27:36.000000 tardis_em-0.2.6/tardis_em.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-24 08:27:36.000000 tardis_em-0.2.6/tardis_em.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 08:27:36.000000 tardis_em-0.2.6/tardis_em.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:27:36.657870 tardis_em-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_cnn_build_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_cnn_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_cnn_draw_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_cnn_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7744 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_cnn_nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_cnn_trim_stitch.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_cnn_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_dist_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_dist_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_dist_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_dist_graph_cut.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_dist_img_to_pc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_dist_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_dist_nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_dist_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11123 2024-05-24 08:27:32.000000 tardis_em-0.2.6/tests/test_utils.py
+drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-28 16:44:16.343094 tardis_em-0.2.7/
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     1108 2022-10-24 14:55:09.000000 tardis_em-0.2.7/LICENSE
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)      103 2023-11-22 08:39:36.000000 tardis_em-0.2.7/MANIFEST.in
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     2859 2024-05-28 16:44:16.343010 tardis_em-0.2.7/PKG-INFO
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     5671 2024-05-27 06:52:31.000000 tardis_em-0.2.7/README.rst
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)      200 2023-11-22 08:39:31.000000 tardis_em-0.2.7/pyproject.toml
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)      454 2024-05-17 13:09:26.000000 tardis_em-0.2.7/requirements.txt
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     1851 2024-05-28 16:44:16.343508 tardis_em-0.2.7/setup.cfg
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)      686 2024-01-05 09:11:55.000000 tardis_em-0.2.7/setup.py
+drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-28 16:44:16.314134 tardis_em-0.2.7/tardis_em/
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)      239 2024-05-09 09:38:12.000000 tardis_em-0.2.7/tardis_em/__init__.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)      667 2024-05-28 16:43:58.000000 tardis_em-0.2.7/tardis_em/_version.py
+drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-28 16:44:16.315842 tardis_em-0.2.7/tardis_em/benchmarks/
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)        0 2023-03-22 15:14:45.000000 tardis_em-0.2.7/tardis_em/benchmarks/__init__.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     8279 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tardis_em/benchmarks/benchmarks.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    12326 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tardis_em/benchmarks/predictor.py
+drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-28 16:44:16.317074 tardis_em-0.2.7/tardis_em/cnn/
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)        0 2023-01-04 16:06:13.000000 tardis_em-0.2.7/tardis_em/cnn/__init__.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     4927 2024-01-10 08:08:53.000000 tardis_em-0.2.7/tardis_em/cnn/cnn.py
+drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-28 16:44:16.318415 tardis_em-0.2.7/tardis_em/cnn/data_processing/
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)        0 2023-01-04 16:07:43.000000 tardis_em-0.2.7/tardis_em/cnn/data_processing/__init__.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    12073 2024-05-07 15:06:01.000000 tardis_em-0.2.7/tardis_em/cnn/data_processing/draw_mask.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     5445 2024-02-15 16:58:53.000000 tardis_em-0.2.7/tardis_em/cnn/data_processing/interpolation.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    12894 2024-02-06 10:54:05.000000 tardis_em-0.2.7/tardis_em/cnn/data_processing/stitch.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    13470 2024-02-26 19:54:52.000000 tardis_em-0.2.7/tardis_em/cnn/data_processing/trim.py
+drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-28 16:44:16.319673 tardis_em-0.2.7/tardis_em/cnn/datasets/
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)        0 2023-01-04 16:07:24.000000 tardis_em-0.2.7/tardis_em/cnn/datasets/__init__.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     9105 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tardis_em/cnn/datasets/augmentation.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    15300 2024-01-18 14:25:52.000000 tardis_em-0.2.7/tardis_em/cnn/datasets/build_dataset.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     5450 2024-01-16 12:33:40.000000 tardis_em-0.2.7/tardis_em/cnn/datasets/dataloader.py
+drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-28 16:44:16.320978 tardis_em-0.2.7/tardis_em/cnn/model/
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)        0 2023-01-04 16:07:20.000000 tardis_em-0.2.7/tardis_em/cnn/model/__init__.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    13542 2024-01-17 08:23:39.000000 tardis_em-0.2.7/tardis_em/cnn/model/convolution.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    14686 2024-02-06 10:54:05.000000 tardis_em-0.2.7/tardis_em/cnn/model/decoder_blocks.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     6302 2024-02-06 10:54:05.000000 tardis_em-0.2.7/tardis_em/cnn/model/encoder_blocks.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     1897 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tardis_em/cnn/model/init_weights.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     5930 2024-01-07 16:42:10.000000 tardis_em-0.2.7/tardis_em/cnn/train.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     4398 2024-02-06 10:54:05.000000 tardis_em-0.2.7/tardis_em/cnn/trainer.py
+drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-28 16:44:16.321980 tardis_em-0.2.7/tardis_em/cnn/utils/
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)        0 2023-01-04 16:06:33.000000 tardis_em-0.2.7/tardis_em/cnn/utils/__init__.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    18740 2024-01-18 15:47:53.000000 tardis_em-0.2.7/tardis_em/cnn/utils/build_cnn.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    14593 2024-05-14 07:07:32.000000 tardis_em-0.2.7/tardis_em/cnn/utils/utils.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     8828 2024-05-09 09:14:43.000000 tardis_em-0.2.7/tardis_em/compare_spatial_graphs.py
+drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-28 16:44:16.323343 tardis_em-0.2.7/tardis_em/dist_pytorch/
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)        0 2023-01-04 16:08:56.000000 tardis_em-0.2.7/tardis_em/dist_pytorch/__init__.py
+drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-28 16:44:16.324952 tardis_em-0.2.7/tardis_em/dist_pytorch/datasets/
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)        0 2023-01-04 16:10:04.000000 tardis_em-0.2.7/tardis_em/dist_pytorch/datasets/__init__.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    13939 2024-02-15 16:58:53.000000 tardis_em-0.2.7/tardis_em/dist_pytorch/datasets/augmentation.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    32154 2024-02-21 13:01:04.000000 tardis_em-0.2.7/tardis_em/dist_pytorch/datasets/dataloader.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    20479 2024-02-15 16:58:53.000000 tardis_em-0.2.7/tardis_em/dist_pytorch/datasets/patches.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     9281 2024-05-03 07:51:14.000000 tardis_em-0.2.7/tardis_em/dist_pytorch/dist.py
+drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-28 16:44:16.325953 tardis_em-0.2.7/tardis_em/dist_pytorch/model/
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)        0 2023-01-04 16:09:41.000000 tardis_em-0.2.7/tardis_em/dist_pytorch/model/__init__.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     4993 2024-02-24 14:27:36.000000 tardis_em-0.2.7/tardis_em/dist_pytorch/model/embedding.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    12217 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tardis_em/dist_pytorch/model/layers.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    30389 2024-02-15 16:58:54.000000 tardis_em-0.2.7/tardis_em/dist_pytorch/model/modules.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     4076 2024-02-15 16:58:53.000000 tardis_em-0.2.7/tardis_em/dist_pytorch/sparse_dist.py
+drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-28 16:44:16.326931 tardis_em-0.2.7/tardis_em/dist_pytorch/sparse_model/
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)        0 2023-08-12 17:42:31.000000 tardis_em-0.2.7/tardis_em/dist_pytorch/sparse_model/__init__.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     7048 2024-02-15 16:58:53.000000 tardis_em-0.2.7/tardis_em/dist_pytorch/sparse_model/embedding.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     6224 2024-02-15 16:58:53.000000 tardis_em-0.2.7/tardis_em/dist_pytorch/sparse_model/layers.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     3627 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tardis_em/dist_pytorch/sparse_model/modules.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     9399 2024-02-06 10:54:05.000000 tardis_em-0.2.7/tardis_em/dist_pytorch/train.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    29804 2024-02-15 16:58:54.000000 tardis_em-0.2.7/tardis_em/dist_pytorch/trainer.py
+drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-28 16:44:16.328259 tardis_em-0.2.7/tardis_em/dist_pytorch/utils/
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)      648 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tardis_em/dist_pytorch/utils/__init__.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    16498 2024-05-17 13:19:03.000000 tardis_em-0.2.7/tardis_em/dist_pytorch/utils/build_point_cloud.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    18487 2024-02-26 19:54:52.000000 tardis_em-0.2.7/tardis_em/dist_pytorch/utils/segment_point_cloud.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    13528 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tardis_em/dist_pytorch/utils/utils.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     7095 2024-05-22 15:09:37.000000 tardis_em-0.2.7/tardis_em/predict_actin.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     5458 2024-05-09 09:38:12.000000 tardis_em-0.2.7/tardis_em/predict_mem.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     6741 2024-05-09 09:38:12.000000 tardis_em-0.2.7/tardis_em/predict_mem_2d.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     8476 2024-05-09 09:38:12.000000 tardis_em-0.2.7/tardis_em/predict_mt.py
+drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-28 16:44:16.329058 tardis_em-0.2.7/tardis_em/scripts/
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)       62 2024-02-23 10:17:26.000000 tardis_em-0.2.7/tardis_em/scripts/__init__.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    16330 2024-05-17 13:19:03.000000 tardis_em-0.2.7/tardis_em/scripts/czi_predict.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     3506 2024-05-10 09:01:02.000000 tardis_em-0.2.7/tardis_em/scripts/visualize.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     2909 2024-05-09 13:54:14.000000 tardis_em-0.2.7/tardis_em/tardis.py
+drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-28 16:44:16.329489 tardis_em-0.2.7/tardis_em/tardis_helper/
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)        0 2023-08-13 14:46:27.000000 tardis_em-0.2.7/tardis_em/tardis_helper/__init__.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     2220 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tardis_em/tardis_helper/helper_func.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    11061 2024-05-10 13:40:41.000000 tardis_em-0.2.7/tardis_em/train_DIST.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    10248 2024-05-03 07:47:21.000000 tardis_em-0.2.7/tardis_em/train_cnn.py
+drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-28 16:44:16.335666 tardis_em-0.2.7/tardis_em/utils/
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     1192 2023-04-12 16:41:09.000000 tardis_em-0.2.7/tardis_em/utils/__init__.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    11401 2024-05-22 09:25:56.000000 tardis_em-0.2.7/tardis_em/utils/aws.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     5934 2024-01-20 14:47:45.000000 tardis_em-0.2.7/tardis_em/utils/dataset.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     2137 2024-02-21 11:14:53.000000 tardis_em-0.2.7/tardis_em/utils/device.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     5812 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tardis_em/utils/errors.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    20802 2024-05-07 14:01:05.000000 tardis_em-0.2.7/tardis_em/utils/export_data.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    29405 2024-05-07 14:01:05.000000 tardis_em-0.2.7/tardis_em/utils/load_data.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     9423 2024-02-21 11:14:53.000000 tardis_em-0.2.7/tardis_em/utils/logo.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    20740 2024-02-15 16:58:54.000000 tardis_em-0.2.7/tardis_em/utils/losses.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    12729 2024-05-07 14:01:05.000000 tardis_em-0.2.7/tardis_em/utils/metrics.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     9473 2024-02-06 10:54:05.000000 tardis_em-0.2.7/tardis_em/utils/normalization.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     4830 2024-05-03 07:34:22.000000 tardis_em-0.2.7/tardis_em/utils/ota_update.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    53058 2024-05-28 16:37:19.000000 tardis_em-0.2.7/tardis_em/utils/predictor.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     5756 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tardis_em/utils/setup_envir.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    38169 2024-05-17 13:19:03.000000 tardis_em-0.2.7/tardis_em/utils/spline_metric.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    12177 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tardis_em/utils/trainer.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     3628 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tardis_em/utils/utils.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    12260 2024-01-18 07:34:07.000000 tardis_em-0.2.7/tardis_em/utils/visualize_pc.py
+drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-28 16:44:16.342334 tardis_em-0.2.7/tardis_em.egg-info/
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     2859 2024-05-28 16:44:16.000000 tardis_em-0.2.7/tardis_em.egg-info/PKG-INFO
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     3453 2024-05-28 16:44:16.000000 tardis_em-0.2.7/tardis_em.egg-info/SOURCES.txt
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)        1 2024-05-28 16:44:16.000000 tardis_em-0.2.7/tardis_em.egg-info/dependency_links.txt
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)      559 2024-05-28 16:44:16.000000 tardis_em-0.2.7/tardis_em.egg-info/entry_points.txt
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)      426 2024-05-28 16:44:16.000000 tardis_em-0.2.7/tardis_em.egg-info/requires.txt
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)       10 2024-05-28 16:44:16.000000 tardis_em-0.2.7/tardis_em.egg-info/top_level.txt
+drwxr-xr-x   0 robertkiewisz   (501) staff       (20)        0 2024-05-28 16:44:16.341929 tardis_em-0.2.7/tests/
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     3863 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tests/run_all_tests.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     2209 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tests/test_cnn_build_dataset.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     3223 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tests/test_cnn_dataset.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    10136 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tests/test_cnn_draw_mask.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     1384 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tests/test_cnn_interpolation.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     7744 2024-05-08 08:58:34.000000 tardis_em-0.2.7/tests/test_cnn_nn.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     4851 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tests/test_cnn_trim_stitch.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)      648 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tests/test_cnn_utils.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     8411 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tests/test_dist_augmentation.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     7653 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tests/test_dist_data_loader.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     2828 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tests/test_dist_embedding.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     4636 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tests/test_dist_graph_cut.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     1583 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tests/test_dist_img_to_pc.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     3112 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tests/test_dist_modules.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     3412 2024-05-08 08:39:51.000000 tardis_em-0.2.7/tests/test_dist_nn.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     5233 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tests/test_dist_trainer.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     1525 2024-05-17 13:19:03.000000 tardis_em-0.2.7/tests/test_dist_utils.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     3744 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tests/test_losses.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)     2971 2024-01-05 09:11:55.000000 tardis_em-0.2.7/tests/test_trainer.py
+-rw-r--r--   0 robertkiewisz   (501) staff       (20)    11123 2024-05-08 08:44:15.000000 tardis_em-0.2.7/tests/test_utils.py
```

### Comparing `tardis_em-0.2.6/LICENSE` & `tardis_em-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/PKG-INFO` & `tardis_em-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tardis_em
-Version: 0.2.6
+Version: 0.2.7
 Summary: PyTorch segmentation of 2D/3D images such as electron tomography (ET),Cryo-EM or fluorescent microscopy data into 3D segmented point cloud.
 Home-page: https://github.com/SMLC-NYSBC/TARDIS
 Author: Robert Kiewisz, Tristan Bepler
 Author-email: rkiewisz@nysbc.org
 License: MIT
 Keywords: semantic segmentation,instance segmentation,MT segmentation,membrane segmentation,CNN,FNet,DIST
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tardis_em-0.2.6/README.rst` & `tardis_em-0.2.7/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 Kiewisz R., Bepler T. 2022. Membrane and microtubule rapid instance segmentation with dimensionless instance segmentation by learning graph representations of point clouds. Neurips 2022 - Machine Learning for Structural Biology Workshop.
 
 What's new?
 ===========
 
 `Full History <https://smlc-nysbc.github.io/TARDIS/HISTORY.html>`__
 
-TARDIS-em v0.2.5 (2024-05-22):
+TARDIS-em v0.2.6 (2024-05-22):
     * Added actin segmentation
     * Improvement from Microtubule and Membrane prediction with updated models
     * Added option for scripting TARDIS predictions
     * Added visualization for semantic and instance predictions
     * TARDIS build in results visualization
     * Bug fixes
     * Documentation tutorials
```

### Comparing `tardis_em-0.2.6/setup.cfg` & `tardis_em-0.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/setup.py` & `tardis_em-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/_version.py` & `tardis_em-0.2.7/tests/test_cnn_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,9 +3,7 @@
 #                                                                     #
 #  New York Structural Biology Center                                 #
 #  Simons Machine Learning Center                                     #
 #                                                                     #
 #  Robert Kiewisz, Tristan Bepler                                     #
 #  MIT License 2021 - 2024                                            #
 # #####################################################################
-
-version = "0.2.6"
```

### Comparing `tardis_em-0.2.6/tardis_em/benchmarks/benchmarks.py` & `tardis_em-0.2.7/tardis_em/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/benchmarks/predictor.py` & `tardis_em-0.2.7/tardis_em/benchmarks/predictor.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/cnn/cnn.py` & `tardis_em-0.2.7/tardis_em/cnn/cnn.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/cnn/data_processing/draw_mask.py` & `tardis_em-0.2.7/tardis_em/cnn/data_processing/draw_mask.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/cnn/data_processing/interpolation.py` & `tardis_em-0.2.7/tardis_em/cnn/data_processing/interpolation.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/cnn/data_processing/stitch.py` & `tardis_em-0.2.7/tardis_em/cnn/data_processing/stitch.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/cnn/data_processing/trim.py` & `tardis_em-0.2.7/tardis_em/cnn/data_processing/trim.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/cnn/datasets/augmentation.py` & `tardis_em-0.2.7/tardis_em/cnn/datasets/augmentation.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/cnn/datasets/build_dataset.py` & `tardis_em-0.2.7/tardis_em/cnn/datasets/build_dataset.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/cnn/datasets/dataloader.py` & `tardis_em-0.2.7/tardis_em/cnn/datasets/dataloader.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,168 +1,168 @@
-#######################################################################
-#  TARDIS - Transformer And Rapid Dimensionless Instance Segmentation #
-#                                                                     #
-#  New York Structural Biology Center                                 #
-#  Simons Machine Learning Center                                     #
-#                                                                     #
-#  Robert Kiewisz, Tristan Bepler                                     #
-#  MIT License 2021 - 2024                                            #
-#######################################################################
-
-import os
-from os import listdir
-from os.path import join, splitext
-from typing import Tuple
-
-import numpy as np
-import torch
-from torch.utils.data import Dataset
-
-from tardis_em.cnn.datasets.augmentation import preprocess
-from tardis_em.utils.errors import TardisError
-from tardis_em.utils.load_data import load_image
-from tardis_em.utils.normalization import MinMaxNormalize
-
-
-class CNNDataset(Dataset):
-    """
-    DATASET BUILDER FOR IMAGES AND SEMANTIC LABEL MASKS FOR TRAINING
-
-    Args:
-        img_dir (str): Source of the 2D/3D .tif file.
-        mask_dir (str): Source of the 2D/3D .tif  images masks.
-        size (int): Output patch size for image and mask.
-        mask_suffix (str): Suffix name for mask images.
-        transform (bool): Call for random transformation on img and mask.
-        out_channels (int): Number of output channels.
-    """
-
-    def __init__(
-        self,
-        img_dir: str,
-        mask_dir: str,
-        size=64,
-        mask_suffix="_mask",
-        transform=True,
-        out_channels=1,
-    ):
-        self.img_dir = img_dir
-        self.mask_dir = mask_dir
-        self.size = size
-        self.mask_suffix = mask_suffix
-        self.transform = transform
-        self.out_channels = out_channels
-        self.minmax = MinMaxNormalize()
-
-        self.ids = [
-            splitext(file)[0] for file in listdir(img_dir) if not file.startswith(".")
-        ]
-        self.format = [
-            splitext(file)[1]
-            for file in listdir(img_dir)[:5]
-            if not file.startswith(".")
-        ][1]
-
-    def __len__(self):
-        return len(self.ids)
-
-    def __getitem__(self, i: int) -> Tuple[torch.Tensor, torch.Tensor]:
-        """
-        Select and process dataset for CNN.
-
-        Args:
-            i (int): Image ID number.
-
-        Returns:
-            torch.Tensor, torch.Tensor: Tensor of processed image and mask.
-        """
-        # Find next image and corresponding label mask image
-        idx = self.ids[i]
-        mask_file = os.path.join(self.mask_dir, str(idx) + "_mask" + self.format)
-        img_file = os.path.join(self.img_dir, str(idx) + self.format)
-
-        # Load image and corresponding label mask
-        img, _ = load_image(img_file)
-        mask, _ = load_image(mask_file)
-
-        if mask.dtype != np.uint8:
-            TardisError(
-                "147",
-                "tardis_em/cnn/dataset/dataloader.py",
-                f"Mask should be of np.uint8 dtype but is {mask.dtype}!",
-            )
-
-        # Process image and mask
-        img, mask = preprocess(
-            image=img,
-            mask=mask,
-            size=self.size,
-            transformation=self.transform,
-            output_dim_mask=self.out_channels,
-        )
-
-        if img.dtype != np.float32 and mask.dtype != np.uint8:
-            TardisError(
-                "147",
-                "tardis_em/cnn/dataset/dataloader.py",
-                f"Mask {mask.dtype} and image  {img.dtype} has wrong dtype!",
-            )
-        if not img.min() >= -1 and not img.max() <= 1:
-            TardisError(
-                "147",
-                "tardis_em/cnn/dataset/dataloader.py",
-                "Image file is not binary!",
-            )
-
-        return torch.from_numpy(img.copy()).type(torch.float32), torch.from_numpy(
-            mask.copy()
-        ).type(torch.float32)
-
-
-class PredictionDataset(Dataset):
-    """
-    DATASET BUILDER FOR IMAGES AND SEMANTIC LABEL MASKS FOR PREDICTION
-
-    Module has turn off all transformations.
-
-    Args:
-        img_dir (str): Source of the 2D/3D .tif file.
-        out_channels (int): Number of output channels.
-    """
-
-    def __init__(self, img_dir: str, out_channels=1):
-        self.img_dir = img_dir
-        self.out_channels = out_channels
-
-        self.ids = [
-            splitext(file)[0] for file in listdir(img_dir) if not file.startswith(".")
-        ]
-
-    def __len__(self):
-        return len(self.ids)
-
-    def __getitem__(self, i: int):
-        """
-        Select and process dataset for CNN.
-
-        Args:
-            i (int): Image ID number.
-
-        Returns:
-            torch.Tensor, str: Tensor of processed image and image file name.
-        """
-        idx = self.ids[i]
-        img_file = join(self.img_dir, str(idx) + ".tif")
-
-        # Load image
-        img, _ = load_image(img_file)
-        img = img.astype(np.float32)
-
-        # Process image and mask
-        img = preprocess(
-            image=img,
-            size=img.shape,
-            transformation=False,
-            output_dim_mask=self.out_channels,
-        )
-
-        return torch.from_numpy(img).type(torch.float32), idx
+#######################################################################
+#  TARDIS - Transformer And Rapid Dimensionless Instance Segmentation #
+#                                                                     #
+#  New York Structural Biology Center                                 #
+#  Simons Machine Learning Center                                     #
+#                                                                     #
+#  Robert Kiewisz, Tristan Bepler                                     #
+#  MIT License 2021 - 2024                                            #
+#######################################################################
+
+import os
+from os import listdir
+from os.path import join, splitext
+from typing import Tuple
+
+import numpy as np
+import torch
+from torch.utils.data import Dataset
+
+from tardis_em.cnn.datasets.augmentation import preprocess
+from tardis_em.utils.errors import TardisError
+from tardis_em.utils.load_data import load_image
+from tardis_em.utils.normalization import MinMaxNormalize
+
+
+class CNNDataset(Dataset):
+    """
+    DATASET BUILDER FOR IMAGES AND SEMANTIC LABEL MASKS FOR TRAINING
+
+    Args:
+        img_dir (str): Source of the 2D/3D .tif file.
+        mask_dir (str): Source of the 2D/3D .tif  images masks.
+        size (int): Output patch size for image and mask.
+        mask_suffix (str): Suffix name for mask images.
+        transform (bool): Call for random transformation on img and mask.
+        out_channels (int): Number of output channels.
+    """
+
+    def __init__(
+        self,
+        img_dir: str,
+        mask_dir: str,
+        size=64,
+        mask_suffix="_mask",
+        transform=True,
+        out_channels=1,
+    ):
+        self.img_dir = img_dir
+        self.mask_dir = mask_dir
+        self.size = size
+        self.mask_suffix = mask_suffix
+        self.transform = transform
+        self.out_channels = out_channels
+        self.minmax = MinMaxNormalize()
+
+        self.ids = [
+            splitext(file)[0] for file in listdir(img_dir) if not file.startswith(".")
+        ]
+        self.format = [
+            splitext(file)[1]
+            for file in listdir(img_dir)[:5]
+            if not file.startswith(".")
+        ][1]
+
+    def __len__(self):
+        return len(self.ids)
+
+    def __getitem__(self, i: int) -> Tuple[torch.Tensor, torch.Tensor]:
+        """
+        Select and process dataset for CNN.
+
+        Args:
+            i (int): Image ID number.
+
+        Returns:
+            torch.Tensor, torch.Tensor: Tensor of processed image and mask.
+        """
+        # Find next image and corresponding label mask image
+        idx = self.ids[i]
+        mask_file = os.path.join(self.mask_dir, str(idx) + "_mask" + self.format)
+        img_file = os.path.join(self.img_dir, str(idx) + self.format)
+
+        # Load image and corresponding label mask
+        img, _ = load_image(img_file)
+        mask, _ = load_image(mask_file)
+
+        if mask.dtype != np.uint8:
+            TardisError(
+                "147",
+                "tardis_em/cnn/dataset/dataloader.py",
+                f"Mask should be of np.uint8 dtype but is {mask.dtype}!",
+            )
+
+        # Process image and mask
+        img, mask = preprocess(
+            image=img,
+            mask=mask,
+            size=self.size,
+            transformation=self.transform,
+            output_dim_mask=self.out_channels,
+        )
+
+        if img.dtype != np.float32 and mask.dtype != np.uint8:
+            TardisError(
+                "147",
+                "tardis_em/cnn/dataset/dataloader.py",
+                f"Mask {mask.dtype} and image  {img.dtype} has wrong dtype!",
+            )
+        if not img.min() >= -1 and not img.max() <= 1:
+            TardisError(
+                "147",
+                "tardis_em/cnn/dataset/dataloader.py",
+                "Image file is not binary!",
+            )
+
+        return torch.from_numpy(img.copy()).type(torch.float32), torch.from_numpy(
+            mask.copy()
+        ).type(torch.float32)
+
+
+class PredictionDataset(Dataset):
+    """
+    DATASET BUILDER FOR IMAGES AND SEMANTIC LABEL MASKS FOR PREDICTION
+
+    Module has turn off all transformations.
+
+    Args:
+        img_dir (str): Source of the 2D/3D .tif file.
+        out_channels (int): Number of output channels.
+    """
+
+    def __init__(self, img_dir: str, out_channels=1):
+        self.img_dir = img_dir
+        self.out_channels = out_channels
+
+        self.ids = [
+            splitext(file)[0] for file in listdir(img_dir) if not file.startswith(".")
+        ]
+
+    def __len__(self):
+        return len(self.ids)
+
+    def __getitem__(self, i: int):
+        """
+        Select and process dataset for CNN.
+
+        Args:
+            i (int): Image ID number.
+
+        Returns:
+            torch.Tensor, str: Tensor of processed image and image file name.
+        """
+        idx = self.ids[i]
+        img_file = join(self.img_dir, str(idx) + ".tif")
+
+        # Load image
+        img, _ = load_image(img_file)
+        img = img.astype(np.float32)
+
+        # Process image and mask
+        img = preprocess(
+            image=img,
+            size=img.shape,
+            transformation=False,
+            output_dim_mask=self.out_channels,
+        )
+
+        return torch.from_numpy(img).type(torch.float32), idx
```

### Comparing `tardis_em-0.2.6/tardis_em/cnn/model/convolution.py` & `tardis_em-0.2.7/tardis_em/cnn/model/convolution.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/cnn/model/decoder_blocks.py` & `tardis_em-0.2.7/tardis_em/cnn/model/decoder_blocks.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/cnn/model/encoder_blocks.py` & `tardis_em-0.2.7/tardis_em/cnn/model/encoder_blocks.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/cnn/model/init_weights.py` & `tardis_em-0.2.7/tardis_em/cnn/model/init_weights.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/cnn/train.py` & `tardis_em-0.2.7/tardis_em/cnn/train.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/cnn/trainer.py` & `tardis_em-0.2.7/tardis_em/cnn/trainer.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/cnn/utils/build_cnn.py` & `tardis_em-0.2.7/tardis_em/cnn/utils/build_cnn.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/cnn/utils/utils.py` & `tardis_em-0.2.7/tardis_em/cnn/utils/utils.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/compare_spatial_graphs.py` & `tardis_em-0.2.7/tardis_em/compare_spatial_graphs.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/dist_pytorch/datasets/augmentation.py` & `tardis_em-0.2.7/tardis_em/dist_pytorch/datasets/augmentation.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/dist_pytorch/datasets/dataloader.py` & `tardis_em-0.2.7/tardis_em/dist_pytorch/datasets/dataloader.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/dist_pytorch/datasets/patches.py` & `tardis_em-0.2.7/tardis_em/dist_pytorch/datasets/patches.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/dist_pytorch/dist.py` & `tardis_em-0.2.7/tardis_em/dist_pytorch/dist.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/dist_pytorch/model/embedding.py` & `tardis_em-0.2.7/tardis_em/dist_pytorch/model/embedding.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/dist_pytorch/model/layers.py` & `tardis_em-0.2.7/tardis_em/dist_pytorch/model/layers.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/dist_pytorch/model/modules.py` & `tardis_em-0.2.7/tardis_em/dist_pytorch/model/modules.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/dist_pytorch/sparse_dist.py` & `tardis_em-0.2.7/tardis_em/dist_pytorch/sparse_dist.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/dist_pytorch/sparse_model/embedding.py` & `tardis_em-0.2.7/tardis_em/dist_pytorch/sparse_model/embedding.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/dist_pytorch/sparse_model/layers.py` & `tardis_em-0.2.7/tardis_em/dist_pytorch/sparse_model/layers.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/dist_pytorch/sparse_model/modules.py` & `tardis_em-0.2.7/tardis_em/dist_pytorch/sparse_model/modules.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/dist_pytorch/train.py` & `tardis_em-0.2.7/tardis_em/dist_pytorch/train.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/dist_pytorch/trainer.py` & `tardis_em-0.2.7/tardis_em/dist_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/dist_pytorch/utils/__init__.py` & `tardis_em-0.2.7/tardis_em/dist_pytorch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/dist_pytorch/utils/build_point_cloud.py` & `tardis_em-0.2.7/tardis_em/dist_pytorch/utils/build_point_cloud.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/dist_pytorch/utils/segment_point_cloud.py` & `tardis_em-0.2.7/tardis_em/dist_pytorch/utils/segment_point_cloud.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/dist_pytorch/utils/utils.py` & `tardis_em-0.2.7/tardis_em/dist_pytorch/utils/utils.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/predict_actin.py` & `tardis_em-0.2.7/tardis_em/predict_actin.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/predict_mem.py` & `tardis_em-0.2.7/tardis_em/predict_mem.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/predict_mem_2d.py` & `tardis_em-0.2.7/tardis_em/predict_mem_2d.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/predict_mt.py` & `tardis_em-0.2.7/tardis_em/predict_mt.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/scripts/czi_predict.py` & `tardis_em-0.2.7/tardis_em/scripts/czi_predict.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/scripts/visualize.py` & `tardis_em-0.2.7/tardis_em/scripts/visualize.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/tardis.py` & `tardis_em-0.2.7/tardis_em/tardis.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/tardis_helper/helper_func.py` & `tardis_em-0.2.7/tardis_em/tardis_helper/helper_func.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/train_DIST.py` & `tardis_em-0.2.7/tardis_em/train_DIST.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/train_cnn.py` & `tardis_em-0.2.7/tardis_em/train_cnn.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/utils/__init__.py` & `tardis_em-0.2.7/tardis_em/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/utils/aws.py` & `tardis_em-0.2.7/tardis_em/utils/aws.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/utils/dataset.py` & `tardis_em-0.2.7/tardis_em/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/utils/device.py` & `tardis_em-0.2.7/tardis_em/utils/device.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/utils/errors.py` & `tardis_em-0.2.7/tardis_em/utils/errors.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/utils/export_data.py` & `tardis_em-0.2.7/tardis_em/utils/export_data.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/utils/load_data.py` & `tardis_em-0.2.7/tardis_em/utils/load_data.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/utils/logo.py` & `tardis_em-0.2.7/tardis_em/utils/logo.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/utils/losses.py` & `tardis_em-0.2.7/tardis_em/utils/losses.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/utils/metrics.py` & `tardis_em-0.2.7/tardis_em/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/utils/normalization.py` & `tardis_em-0.2.7/tardis_em/utils/normalization.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/utils/ota_update.py` & `tardis_em-0.2.7/tardis_em/utils/ota_update.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/utils/predictor.py` & `tardis_em-0.2.7/tardis_em/utils/predictor.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,15 @@
         if NN in ["Microtubule", "Actin"]:
             self.normalize_px = 25
         else:
             self.normalize_px = 15
 
         if NN in ["Actin", "Microtubule"]:
             # Build CNN network with loaded pre-trained weights
-            if not self.output_format.startswith("None") and not self.binary_mask:
+            if not self.binary_mask:
                 self.cnn = Predictor(
                     checkpoint=self.checkpoint[0],
                     network=self.convolution_nn,
                     subtype="32",
                     model_type="microtubules_3d" if NN == "Microtubule" else "actin_3d",
                     img_size=self.patch_size,
                     sigmoid=False,
@@ -334,15 +334,15 @@
                     subtype="triang",
                     model_type="2d",
                     device=self.device,
                 )
         elif NN in ["Membrane2D", "Membrane"]:
             # Build CNN network with loaded pre-trained weights
             if NN == "Membrane2D":
-                if not self.output_format.startswith("None") and not self.binary_mask:
+                if not self.binary_mask:
                     self.cnn = Predictor(
                         checkpoint=self.checkpoint[0],
                         network=self.convolution_nn,
                         subtype="32",
                         model_type="membrane_2d",
                         img_size=self.patch_size,
                         sigmoid=False,
@@ -356,15 +356,15 @@
                         checkpoint=self.checkpoint[1],
                         network="dist",
                         subtype="triang",
                         model_type="2d",
                         device=self.device,
                     )
             else:
-                if not self.output_format.startswith("None") and not self.binary_mask:
+                if not self.binary_mask:
                     self.cnn = Predictor(
                         checkpoint=self.checkpoint[0],
                         network=self.convolution_nn,
                         subtype="32",
                         model_type="membrane_3d",
                         img_size=self.patch_size,
                         sigmoid=False,
@@ -1067,15 +1067,15 @@
                 else:
                     assert not assert_, msg
 
             # Tardis progress bar update
             self.log_tardis(id_, i, log_id=1)
 
             """Semantic Segmentation"""
-            if not self.output_format.startswith("None") and not self.binary_mask:
+            if not self.binary_mask:
                 # Cut image for fix patch size and normalizing image pixel size
                 trim_with_stride(
                     image=self.image,
                     scale=self.scale_shape,
                     trim_size_xy=self.patch_size,
                     trim_size_z=self.patch_size,
                     output=join(self.dir, "temp", "Patches"),
```

### Comparing `tardis_em-0.2.6/tardis_em/utils/setup_envir.py` & `tardis_em-0.2.7/tardis_em/utils/setup_envir.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/utils/spline_metric.py` & `tardis_em-0.2.7/tardis_em/utils/spline_metric.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/utils/trainer.py` & `tardis_em-0.2.7/tardis_em/utils/trainer.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/utils/utils.py` & `tardis_em-0.2.7/tardis_em/utils/utils.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em/utils/visualize_pc.py` & `tardis_em-0.2.7/tardis_em/utils/visualize_pc.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tardis_em.egg-info/PKG-INFO` & `tardis_em-0.2.7/tardis_em.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tardis_em
-Version: 0.2.6
+Version: 0.2.7
 Summary: PyTorch segmentation of 2D/3D images such as electron tomography (ET),Cryo-EM or fluorescent microscopy data into 3D segmented point cloud.
 Home-page: https://github.com/SMLC-NYSBC/TARDIS
 Author: Robert Kiewisz, Tristan Bepler
 Author-email: rkiewisz@nysbc.org
 License: MIT
 Keywords: semantic segmentation,instance segmentation,MT segmentation,membrane segmentation,CNN,FNet,DIST
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tardis_em-0.2.6/tardis_em.egg-info/SOURCES.txt` & `tardis_em-0.2.7/tardis_em.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 tardis_em/utils/ota_update.py
 tardis_em/utils/predictor.py
 tardis_em/utils/setup_envir.py
 tardis_em/utils/spline_metric.py
 tardis_em/utils/trainer.py
 tardis_em/utils/utils.py
 tardis_em/utils/visualize_pc.py
+tests/run_all_tests.py
 tests/test_cnn_build_dataset.py
 tests/test_cnn_dataset.py
 tests/test_cnn_draw_mask.py
 tests/test_cnn_interpolation.py
 tests/test_cnn_nn.py
 tests/test_cnn_trim_stitch.py
 tests/test_cnn_utils.py
```

### Comparing `tardis_em-0.2.6/tardis_em.egg-info/entry_points.txt` & `tardis_em-0.2.7/tardis_em.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tests/test_cnn_build_dataset.py` & `tardis_em-0.2.7/tests/test_cnn_build_dataset.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tests/test_cnn_dataset.py` & `tardis_em-0.2.7/tests/test_cnn_dataset.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tests/test_cnn_draw_mask.py` & `tardis_em-0.2.7/tests/test_cnn_draw_mask.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tests/test_cnn_interpolation.py` & `tardis_em-0.2.7/tests/test_cnn_interpolation.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tests/test_cnn_nn.py` & `tardis_em-0.2.7/tests/test_cnn_nn.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tests/test_cnn_trim_stitch.py` & `tardis_em-0.2.7/tests/test_cnn_trim_stitch.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tests/test_cnn_utils.py` & `tardis_em-0.2.7/tardis_em/_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,7 +3,9 @@
 #                                                                     #
 #  New York Structural Biology Center                                 #
 #  Simons Machine Learning Center                                     #
 #                                                                     #
 #  Robert Kiewisz, Tristan Bepler                                     #
 #  MIT License 2021 - 2024                                            #
 # #####################################################################
+
+version = "0.2.7"
```

### Comparing `tardis_em-0.2.6/tests/test_dist_augmentation.py` & `tardis_em-0.2.7/tests/test_dist_augmentation.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tests/test_dist_data_loader.py` & `tardis_em-0.2.7/tests/test_dist_data_loader.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tests/test_dist_embedding.py` & `tardis_em-0.2.7/tests/test_dist_embedding.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tests/test_dist_graph_cut.py` & `tardis_em-0.2.7/tests/test_dist_graph_cut.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tests/test_dist_img_to_pc.py` & `tardis_em-0.2.7/tests/test_dist_img_to_pc.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tests/test_dist_modules.py` & `tardis_em-0.2.7/tests/test_dist_modules.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tests/test_dist_nn.py` & `tardis_em-0.2.7/tests/test_dist_nn.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tests/test_dist_trainer.py` & `tardis_em-0.2.7/tests/test_dist_trainer.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tests/test_dist_utils.py` & `tardis_em-0.2.7/tests/test_dist_utils.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tests/test_losses.py` & `tardis_em-0.2.7/tests/test_losses.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tests/test_trainer.py` & `tardis_em-0.2.7/tests/test_trainer.py`

 * *Files identical despite different names*

### Comparing `tardis_em-0.2.6/tests/test_utils.py` & `tardis_em-0.2.7/tests/test_utils.py`

 * *Files identical despite different names*

