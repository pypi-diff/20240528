# Comparing `tmp/mb_pytorch-1.0.52.tar.gz` & `tmp/mb_pytorch-1.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mb_pytorch-1.0.52.tar", last modified: Mon May 27 21:21:12 2024, max compression
+gzip compressed data, was "mb_pytorch-1.0.53.tar", last modified: Mon May 27 21:31:28 2024, max compression
```

## Comparing `mb_pytorch-1.0.52.tar` & `mb_pytorch-1.0.53.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:21:12.645662 mb_pytorch-1.0.52/
--rw-r--r--   0 malav     (1000) malav     (1000)      206 2024-05-27 21:21:12.645662 mb_pytorch-1.0.52/PKG-INFO
--rw-rw-r--   0 malav     (1000) malav     (1000)      742 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/README.md
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:21:12.641662 mb_pytorch-1.0.52/mb_pytorch/
--rw-rw-r--   0 malav     (1000) malav     (1000)       97 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/__init__.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:21:12.641662 mb_pytorch-1.0.52/mb_pytorch/classification/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:38:04.000000 mb_pytorch-1.0.52/mb_pytorch/classification/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     7166 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/classification/training.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:21:12.641662 mb_pytorch-1.0.52/mb_pytorch/dataloader/
--rw-rw-r--   0 malav     (1000) malav     (1000)       44 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/dataloader/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)    19206 2024-05-27 21:20:59.000000 mb_pytorch-1.0.52/mb_pytorch/dataloader/loader.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:21:12.641662 mb_pytorch-1.0.52/mb_pytorch/detection/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:38:14.000000 mb_pytorch-1.0.52/mb_pytorch/detection/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     6567 2024-05-27 20:31:19.000000 mb_pytorch-1.0.52/mb_pytorch/detection/training.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:21:12.641662 mb_pytorch-1.0.52/mb_pytorch/metalearning/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/metalearning/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1385 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/metalearning/meta_utils.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1030 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/metalearning/proto_dataloader.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     2861 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/metalearning/prototypical.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:21:12.641662 mb_pytorch-1.0.52/mb_pytorch/models/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/models/__init__.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:21:12.641662 mb_pytorch-1.0.52/mb_pytorch/models/blocks/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/models/blocks/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     2801 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/models/blocks/attention_block.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     3629 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/models/blocks/cnn.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     4783 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/models/blocks/conv_block.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      920 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/models/blocks/conv_with_relu.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     2256 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/models/blocks/model_out.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1184 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/models/blocks/rnn.py
--rw-rw-r--   0 malav     (1000) malav     (1000)    21087 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/models/extra_models.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      920 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/models/lenet.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     3921 2024-05-17 14:58:48.000000 mb_pytorch-1.0.52/mb_pytorch/models/modelloader.py
--rw-rw-r--   0 malav     (1000) malav     (1000)    10784 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/models/unet_models.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:21:12.641662 mb_pytorch-1.0.52/mb_pytorch/segmentation/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:59:50.000000 mb_pytorch-1.0.52/mb_pytorch/segmentation/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     4800 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/segmentation/training.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:21:12.641662 mb_pytorch-1.0.52/mb_pytorch/training/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:59:41.000000 mb_pytorch-1.0.52/mb_pytorch/training/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1630 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/training/accelerate_train.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1454 2024-05-17 23:03:52.000000 mb_pytorch-1.0.52/mb_pytorch/training/train_params.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      144 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/training/training.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:21:12.645662 mb_pytorch-1.0.52/mb_pytorch/utils/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/utils/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1055 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/utils/compiler.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      257 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/utils/dist.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     3391 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/utils/extra_utils.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     7097 2024-05-13 00:29:33.000000 mb_pytorch-1.0.52/mb_pytorch/utils/generate_emb.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     2582 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/utils/losses.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1199 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/utils/metrics.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      207 2024-05-27 21:21:01.000000 mb_pytorch-1.0.52/mb_pytorch/utils/version.py
--rw-rw-r--   0 malav     (1000) malav     (1000)    10620 2024-05-23 19:25:11.000000 mb_pytorch-1.0.52/mb_pytorch/utils/viewer.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      994 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/mb_pytorch/utils/yaml_reader.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:21:12.645662 mb_pytorch-1.0.52/mb_pytorch.egg-info/
--rw-r--r--   0 malav     (1000) malav     (1000)      206 2024-05-27 21:21:12.000000 mb_pytorch-1.0.52/mb_pytorch.egg-info/PKG-INFO
--rw-rw-r--   0 malav     (1000) malav     (1000)     1607 2024-05-27 21:21:12.000000 mb_pytorch-1.0.52/mb_pytorch.egg-info/SOURCES.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)        1 2024-05-27 21:21:12.000000 mb_pytorch-1.0.52/mb_pytorch.egg-info/dependency_links.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       27 2024-05-27 21:21:12.000000 mb_pytorch-1.0.52/mb_pytorch.egg-info/requires.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       19 2024-05-27 21:21:12.000000 mb_pytorch-1.0.52/mb_pytorch.egg-info/top_level.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       81 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/pyproject.toml
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:21:12.645662 mb_pytorch-1.0.52/scripts/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/scripts/__init__.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:21:12.645662 mb_pytorch-1.0.52/scripts/extra_utils/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/scripts/extra_utils/__init__.py
--rwxrwxr-x   0 malav     (1000) malav     (1000)     1314 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/scripts/extra_utils/dataload_results.py
--rw-rw-r--   0 malav     (1000) malav     (1000)       38 2024-05-27 21:21:12.645662 mb_pytorch-1.0.52/setup.cfg
--rw-rw-r--   0 malav     (1000) malav     (1000)      818 2024-05-06 17:42:04.000000 mb_pytorch-1.0.52/setup.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:31:28.587258 mb_pytorch-1.0.53/
+-rw-r--r--   0 malav     (1000) malav     (1000)      206 2024-05-27 21:31:28.587258 mb_pytorch-1.0.53/PKG-INFO
+-rw-rw-r--   0 malav     (1000) malav     (1000)      742 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/README.md
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:31:28.579258 mb_pytorch-1.0.53/mb_pytorch/
+-rw-rw-r--   0 malav     (1000) malav     (1000)       97 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/__init__.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:31:28.583258 mb_pytorch-1.0.53/mb_pytorch/classification/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:38:04.000000 mb_pytorch-1.0.53/mb_pytorch/classification/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     7166 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/classification/training.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:31:28.583258 mb_pytorch-1.0.53/mb_pytorch/dataloader/
+-rw-rw-r--   0 malav     (1000) malav     (1000)       44 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/dataloader/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)    19206 2024-05-27 21:31:06.000000 mb_pytorch-1.0.53/mb_pytorch/dataloader/loader.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:31:28.583258 mb_pytorch-1.0.53/mb_pytorch/detection/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:38:14.000000 mb_pytorch-1.0.53/mb_pytorch/detection/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     6567 2024-05-27 20:31:19.000000 mb_pytorch-1.0.53/mb_pytorch/detection/training.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:31:28.583258 mb_pytorch-1.0.53/mb_pytorch/metalearning/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/metalearning/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1385 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/metalearning/meta_utils.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1030 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/metalearning/proto_dataloader.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     2861 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/metalearning/prototypical.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:31:28.583258 mb_pytorch-1.0.53/mb_pytorch/models/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/models/__init__.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:31:28.583258 mb_pytorch-1.0.53/mb_pytorch/models/blocks/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/models/blocks/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     2801 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/models/blocks/attention_block.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     3629 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/models/blocks/cnn.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     4783 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/models/blocks/conv_block.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      920 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/models/blocks/conv_with_relu.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     2256 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/models/blocks/model_out.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1184 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/models/blocks/rnn.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)    21087 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/models/extra_models.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      920 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/models/lenet.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     3921 2024-05-17 14:58:48.000000 mb_pytorch-1.0.53/mb_pytorch/models/modelloader.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)    10784 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/models/unet_models.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:31:28.583258 mb_pytorch-1.0.53/mb_pytorch/segmentation/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:59:50.000000 mb_pytorch-1.0.53/mb_pytorch/segmentation/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     4800 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/segmentation/training.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:31:28.583258 mb_pytorch-1.0.53/mb_pytorch/training/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-15 16:59:41.000000 mb_pytorch-1.0.53/mb_pytorch/training/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1630 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/training/accelerate_train.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1454 2024-05-17 23:03:52.000000 mb_pytorch-1.0.53/mb_pytorch/training/train_params.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      144 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/training/training.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:31:28.583258 mb_pytorch-1.0.53/mb_pytorch/utils/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/utils/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1055 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/utils/compiler.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      257 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/utils/dist.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     3391 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/utils/extra_utils.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     7097 2024-05-13 00:29:33.000000 mb_pytorch-1.0.53/mb_pytorch/utils/generate_emb.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     2582 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/utils/losses.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1199 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/utils/metrics.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      207 2024-05-27 21:31:23.000000 mb_pytorch-1.0.53/mb_pytorch/utils/version.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)    10620 2024-05-23 19:25:11.000000 mb_pytorch-1.0.53/mb_pytorch/utils/viewer.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      994 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/mb_pytorch/utils/yaml_reader.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:31:28.587258 mb_pytorch-1.0.53/mb_pytorch.egg-info/
+-rw-r--r--   0 malav     (1000) malav     (1000)      206 2024-05-27 21:31:28.000000 mb_pytorch-1.0.53/mb_pytorch.egg-info/PKG-INFO
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1607 2024-05-27 21:31:28.000000 mb_pytorch-1.0.53/mb_pytorch.egg-info/SOURCES.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)        1 2024-05-27 21:31:28.000000 mb_pytorch-1.0.53/mb_pytorch.egg-info/dependency_links.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       27 2024-05-27 21:31:28.000000 mb_pytorch-1.0.53/mb_pytorch.egg-info/requires.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       19 2024-05-27 21:31:28.000000 mb_pytorch-1.0.53/mb_pytorch.egg-info/top_level.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       81 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/pyproject.toml
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:31:28.583258 mb_pytorch-1.0.53/scripts/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/scripts/__init__.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-27 21:31:28.583258 mb_pytorch-1.0.53/scripts/extra_utils/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/scripts/extra_utils/__init__.py
+-rwxrwxr-x   0 malav     (1000) malav     (1000)     1314 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/scripts/extra_utils/dataload_results.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)       38 2024-05-27 21:31:28.587258 mb_pytorch-1.0.53/setup.cfg
+-rw-rw-r--   0 malav     (1000) malav     (1000)      818 2024-05-06 17:42:04.000000 mb_pytorch-1.0.53/setup.py
```

### Comparing `mb_pytorch-1.0.52/README.md` & `mb_pytorch-1.0.53/README.md`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/classification/training.py` & `mb_pytorch-1.0.53/mb_pytorch/classification/training.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/dataloader/loader.py` & `mb_pytorch-1.0.53/mb_pytorch/dataloader/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
     def __call__(self,img,mask=None,bbox=None):
         if self.transform_data['to_tensor']['val']:
             img = transforms.ToTensor()(img)
             if mask is not None:
                 mask = transforms.ToTensor()(mask)
             if bbox is not None:
-                bbox = torch.tensor([[bbox[0],bbox[1],bbox[2],bbox[3]]],dtype=torch.float32)
+                bbox = torch.tensor([[bbox[0],bbox[1],bbox[2],bbox[3]]],dtype=torch.int32)
 
         if self.transform_data['normalize']['val']:
             img = transforms.Normalize(self.transform_data['normalize']['args']['mean'],self.transform_data['normalize']['args']['std'])(img)
 
         if self.transform_data['resize']['val']:
             img = transforms.Resize(self.transform_data['resize']['args']['size'])(img)
             if mask is not None:
@@ -316,15 +316,15 @@
         
         if self.data_type == 'detection':
             if self.transform:
                 img,bbox = self.transform(img,bbox)
             bbox_dict={}
             bbox_dict['boxes'] = torch.tensor([[self.bbox.iloc[idx][0],self.bbox.iloc[idx][1],self.bbox.iloc[idx][2],self.bbox.iloc[idx][3]] 
                                              for x in len(self.bbox.iloc[idx])],dtype=torch.int32)  ## should be list in a list.
-            bbox_dict['label'] = self.label.iloc[idx]
+            bbox_dict['label'] = [self.label.iloc[idx]]
 
             return img,bbox_dict
 
 class DataLoader(data_fetcher):
     """
     Basic dataloader for pytorch1.0
     """
```

### Comparing `mb_pytorch-1.0.52/mb_pytorch/detection/training.py` & `mb_pytorch-1.0.53/mb_pytorch/detection/training.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/metalearning/meta_utils.py` & `mb_pytorch-1.0.53/mb_pytorch/metalearning/meta_utils.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/metalearning/proto_dataloader.py` & `mb_pytorch-1.0.53/mb_pytorch/metalearning/proto_dataloader.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/metalearning/prototypical.py` & `mb_pytorch-1.0.53/mb_pytorch/metalearning/prototypical.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/models/blocks/attention_block.py` & `mb_pytorch-1.0.53/mb_pytorch/models/blocks/attention_block.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/models/blocks/cnn.py` & `mb_pytorch-1.0.53/mb_pytorch/models/blocks/cnn.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/models/blocks/conv_block.py` & `mb_pytorch-1.0.53/mb_pytorch/models/blocks/conv_block.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/models/blocks/conv_with_relu.py` & `mb_pytorch-1.0.53/mb_pytorch/models/blocks/conv_with_relu.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/models/blocks/model_out.py` & `mb_pytorch-1.0.53/mb_pytorch/models/blocks/model_out.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/models/blocks/rnn.py` & `mb_pytorch-1.0.53/mb_pytorch/models/blocks/rnn.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/models/extra_models.py` & `mb_pytorch-1.0.53/mb_pytorch/models/extra_models.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/models/lenet.py` & `mb_pytorch-1.0.53/mb_pytorch/models/lenet.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/models/modelloader.py` & `mb_pytorch-1.0.53/mb_pytorch/models/modelloader.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/models/unet_models.py` & `mb_pytorch-1.0.53/mb_pytorch/models/unet_models.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/segmentation/training.py` & `mb_pytorch-1.0.53/mb_pytorch/segmentation/training.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/training/accelerate_train.py` & `mb_pytorch-1.0.53/mb_pytorch/training/accelerate_train.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/training/train_params.py` & `mb_pytorch-1.0.53/mb_pytorch/training/train_params.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/utils/compiler.py` & `mb_pytorch-1.0.53/mb_pytorch/utils/compiler.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/utils/extra_utils.py` & `mb_pytorch-1.0.53/mb_pytorch/utils/extra_utils.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/utils/generate_emb.py` & `mb_pytorch-1.0.53/mb_pytorch/utils/generate_emb.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/utils/losses.py` & `mb_pytorch-1.0.53/mb_pytorch/utils/losses.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/utils/metrics.py` & `mb_pytorch-1.0.53/mb_pytorch/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/utils/viewer.py` & `mb_pytorch-1.0.53/mb_pytorch/utils/viewer.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch/utils/yaml_reader.py` & `mb_pytorch-1.0.53/mb_pytorch/utils/yaml_reader.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/mb_pytorch.egg-info/SOURCES.txt` & `mb_pytorch-1.0.53/mb_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/scripts/extra_utils/dataload_results.py` & `mb_pytorch-1.0.53/scripts/extra_utils/dataload_results.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.52/setup.py` & `mb_pytorch-1.0.53/setup.py`

 * *Files identical despite different names*

