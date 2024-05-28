# Comparing `tmp/castle_ai-0.0.4.tar.gz` & `tmp/castle_ai-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "castle_ai-0.0.4.tar", last modified: Mon May 27 07:33:56 2024, max compression
+gzip compressed data, was "castle_ai-0.0.5.tar", last modified: Mon May 27 10:07:51 2024, max compression
```

## Comparing `castle_ai-0.0.4.tar` & `castle_ai-0.0.5.tar`

### file list

```diff
@@ -1,125 +1,141 @@
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 07:33:56.275453 castle_ai-0.0.4/
--rw-r--r--   0 raiso     (1000) raiso     (1000)     1728 2024-05-27 07:33:56.275453 castle_ai-0.0.4/PKG-INFO
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      866 2024-05-23 10:10:57.000000 castle_ai-0.0.4/README.md
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 07:33:56.271453 castle_ai-0.0.4/castle/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)       20 2024-05-22 04:34:06.000000 castle_ai-0.0.4/castle/__init__.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 07:33:56.271453 castle_ai-0.0.4/castle/aot/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)       31 2024-05-22 04:48:14.000000 castle_ai-0.0.4/castle/aot/__init__.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 07:33:56.275453 castle_ai-0.0.4/castle/aot/configs/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-23 00:30:16.000000 castle_ai-0.0.4/castle/aot/configs/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     5566 2024-05-22 06:28:08.000000 castle_ai-0.0.4/castle/aot/configs/default.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 07:33:56.275453 castle_ai-0.0.4/castle/aot/configs/models/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-23 00:32:03.000000 castle_ai-0.0.4/castle/aot/configs/models/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      207 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/configs/models/aotb.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      289 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/configs/models/aotl.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      207 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/configs/models/aots.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      174 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/configs/models/aott.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      206 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/configs/models/deaotb.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      289 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/configs/models/deaotl.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      206 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/configs/models/deaots.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      173 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/configs/models/deaott.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      957 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/configs/models/default.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      420 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/configs/models/default_deaot.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      545 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/configs/models/r101_aotl.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      541 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/configs/models/r50_aotl.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      410 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/configs/models/r50_deaotl.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      585 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/configs/models/rs101_aotl.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      645 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/configs/models/swinb_aotl.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      451 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/configs/models/swinb_deaotl.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      513 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/configs/pre.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      690 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/configs/pre_dav.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      611 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/configs/pre_ytb.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      668 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/configs/pre_ytb_dav.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      251 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/configs/ytb.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 07:33:56.275453 castle_ai-0.0.4/castle/aot/dataloaders/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/dataloaders/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    14300 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/dataloaders/eval_datasets.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    19828 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/dataloaders/image_transforms.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    24642 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/dataloaders/train_datasets.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    23561 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/dataloaders/video_transforms.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 07:33:56.275453 castle_ai-0.0.4/castle/aot/networks/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 04:49:47.000000 castle_ai-0.0.4/castle/aot/networks/__init__.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 07:33:56.275453 castle_ai-0.0.4/castle/aot/networks/decoders/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      186 2024-05-22 05:12:26.000000 castle_ai-0.0.4/castle/aot/networks/decoders/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     2079 2024-05-22 05:13:06.000000 castle_ai-0.0.4/castle/aot/networks/decoders/fpn.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 07:33:56.275453 castle_ai-0.0.4/castle/aot/networks/encoders/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     1307 2024-05-22 05:08:31.000000 castle_ai-0.0.4/castle/aot/networks/encoders/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     8427 2024-05-22 05:06:53.000000 castle_ai-0.0.4/castle/aot/networks/encoders/mobilenetv2.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     7907 2024-05-22 05:07:00.000000 castle_ai-0.0.4/castle/aot/networks/encoders/mobilenetv3.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 07:33:56.275453 castle_ai-0.0.4/castle/aot/networks/encoders/resnest/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)       23 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/networks/encoders/resnest/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     3343 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/networks/encoders/resnest/resnest.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    16481 2024-05-22 05:10:30.000000 castle_ai-0.0.4/castle/aot/networks/encoders/resnest/resnet.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     4467 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/networks/encoders/resnest/splat.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     6699 2024-05-22 05:07:30.000000 castle_ai-0.0.4/castle/aot/networks/encoders/resnet.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 07:33:56.275453 castle_ai-0.0.4/castle/aot/networks/encoders/swin/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)       35 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/networks/encoders/swin/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      987 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/networks/encoders/swin/build.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    27369 2024-05-22 05:10:57.000000 castle_ai-0.0.4/castle/aot/networks/encoders/swin/swin_transformer.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 07:33:56.275453 castle_ai-0.0.4/castle/aot/networks/engines/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      653 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/networks/engines/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    25206 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/networks/engines/aot_engine.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     5978 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/networks/engines/deaot_engine.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 07:33:56.275453 castle_ai-0.0.4/castle/aot/networks/layers/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/networks/layers/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    32865 2024-05-22 05:11:50.000000 castle_ai-0.0.4/castle/aot/networks/layers/attention.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     5111 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/networks/layers/basic.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     6698 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/networks/layers/loss.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     1700 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/networks/layers/normalization.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     2834 2024-05-22 05:12:08.000000 castle_ai-0.0.4/castle/aot/networks/layers/position.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    24810 2024-05-22 05:11:35.000000 castle_ai-0.0.4/castle/aot/networks/layers/transformer.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 07:33:56.275453 castle_ai-0.0.4/castle/aot/networks/models/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      358 2024-05-22 04:45:04.000000 castle_ai-0.0.4/castle/aot/networks/models/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     4574 2024-05-22 05:03:48.000000 castle_ai-0.0.4/castle/aot/networks/models/aot.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     2109 2024-05-22 05:13:44.000000 castle_ai-0.0.4/castle/aot/networks/models/deaot.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 07:33:56.275453 castle_ai-0.0.4/castle/aot/utils/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/utils/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     6233 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/utils/checkpoint.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     1358 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/utils/cp_ckpt.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     3561 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/utils/ema.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      443 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/utils/eval.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     6075 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/utils/image.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     3454 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/utils/learning.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      829 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/utils/math.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      860 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/utils/meters.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     1102 2024-05-22 03:59:14.000000 castle_ai-0.0.4/castle/aot/utils/metric.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 07:33:56.275453 castle_ai-0.0.4/castle/sam/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 04:03:33.000000 castle_ai-0.0.4/castle/sam/__init__.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 07:33:56.275453 castle_ai-0.0.4/castle/sam/segment_anything/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      427 2024-05-22 04:03:33.000000 castle_ai-0.0.4/castle/sam/segment_anything/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    15132 2024-05-22 04:03:33.000000 castle_ai-0.0.4/castle/sam/segment_anything/automatic_mask_generator.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     2941 2024-05-22 04:03:33.000000 castle_ai-0.0.4/castle/sam/segment_anything/build_sam.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 07:33:56.275453 castle_ai-0.0.4/castle/sam/segment_anything/modeling/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      385 2024-05-22 04:03:33.000000 castle_ai-0.0.4/castle/sam/segment_anything/modeling/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     1479 2024-05-22 04:03:33.000000 castle_ai-0.0.4/castle/sam/segment_anything/modeling/common.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    14407 2024-05-22 04:03:33.000000 castle_ai-0.0.4/castle/sam/segment_anything/modeling/image_encoder.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     6614 2024-05-22 04:03:33.000000 castle_ai-0.0.4/castle/sam/segment_anything/modeling/mask_decoder.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     8594 2024-05-22 04:03:33.000000 castle_ai-0.0.4/castle/sam/segment_anything/modeling/prompt_encoder.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     7225 2024-05-22 04:03:33.000000 castle_ai-0.0.4/castle/sam/segment_anything/modeling/sam.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     8396 2024-05-22 04:03:33.000000 castle_ai-0.0.4/castle/sam/segment_anything/modeling/transformer.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    11818 2024-05-22 04:03:33.000000 castle_ai-0.0.4/castle/sam/segment_anything/predictor.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 07:33:56.275453 castle_ai-0.0.4/castle/sam/segment_anything/utils/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      197 2024-05-22 04:03:33.000000 castle_ai-0.0.4/castle/sam/segment_anything/utils/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)    12711 2024-05-22 04:03:33.000000 castle_ai-0.0.4/castle/sam/segment_anything/utils/amg.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     5790 2024-05-22 04:03:33.000000 castle_ai-0.0.4/castle/sam/segment_anything/utils/onnx.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     3968 2024-05-22 04:03:33.000000 castle_ai-0.0.4/castle/sam/segment_anything/utils/transforms.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      541 2024-05-22 04:03:33.000000 castle_ai-0.0.4/castle/sam/setup.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 07:33:56.275453 castle_ai-0.0.4/castle/utils/
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      137 2024-05-24 08:01:14.000000 castle_ai-0.0.4/castle/utils/__init__.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     1002 2024-05-23 07:41:10.000000 castle_ai-0.0.4/castle/utils/download.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     6382 2024-05-23 08:44:58.000000 castle_ai-0.0.4/castle/utils/image_segment.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     5009 2024-05-27 07:12:04.000000 castle_ai-0.0.4/castle/utils/latent_explorer.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)      881 2024-05-23 09:47:44.000000 castle_ai-0.0.4/castle/utils/plot.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     3448 2024-05-24 06:17:35.000000 castle_ai-0.0.4/castle/utils/video_align.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     2524 2024-05-22 04:09:41.000000 castle_ai-0.0.4/castle/utils/video_io.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     8545 2024-05-23 07:50:24.000000 castle_ai-0.0.4/castle/utils/video_object_segment.py
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     3505 2024-05-24 08:36:28.000000 castle_ai-0.0.4/castle/utils/visual_latent_extract.py
-drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 07:33:56.275453 castle_ai-0.0.4/castle_ai.egg-info/
--rw-r--r--   0 raiso     (1000) raiso     (1000)     1728 2024-05-27 07:33:56.000000 castle_ai-0.0.4/castle_ai.egg-info/PKG-INFO
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     3706 2024-05-27 07:33:56.000000 castle_ai-0.0.4/castle_ai.egg-info/SOURCES.txt
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        1 2024-05-27 07:33:56.000000 castle_ai-0.0.4/castle_ai.egg-info/dependency_links.txt
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        1 2024-05-23 00:05:44.000000 castle_ai-0.0.4/castle_ai.egg-info/not-zip-safe
--rw-rw-r--   0 raiso     (1000) raiso     (1000)       68 2024-05-27 07:33:56.000000 castle_ai-0.0.4/castle_ai.egg-info/requires.txt
--rw-rw-r--   0 raiso     (1000) raiso     (1000)        7 2024-05-27 07:33:56.000000 castle_ai-0.0.4/castle_ai.egg-info/top_level.txt
--rw-rw-r--   0 raiso     (1000) raiso     (1000)       38 2024-05-27 07:33:56.275453 castle_ai-0.0.4/setup.cfg
--rw-rw-r--   0 raiso     (1000) raiso     (1000)     2004 2024-05-27 07:33:17.000000 castle_ai-0.0.4/setup.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 10:07:51.028937 castle_ai-0.0.5/
+-rw-r--r--   0 raiso     (1000) raiso     (1000)     1728 2024-05-27 10:07:51.028937 castle_ai-0.0.5/PKG-INFO
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      866 2024-05-23 10:10:57.000000 castle_ai-0.0.5/README.md
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 10:07:51.024937 castle_ai-0.0.5/castle/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)       20 2024-05-22 04:34:06.000000 castle_ai-0.0.5/castle/__init__.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 10:07:51.024937 castle_ai-0.0.5/castle/aot/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)       31 2024-05-22 04:48:14.000000 castle_ai-0.0.5/castle/aot/__init__.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 10:07:51.024937 castle_ai-0.0.5/castle/aot/configs/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-23 00:30:16.000000 castle_ai-0.0.5/castle/aot/configs/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     5566 2024-05-22 06:28:08.000000 castle_ai-0.0.5/castle/aot/configs/default.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 10:07:51.024937 castle_ai-0.0.5/castle/aot/configs/models/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-23 00:32:03.000000 castle_ai-0.0.5/castle/aot/configs/models/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      207 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/configs/models/aotb.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      289 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/configs/models/aotl.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      207 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/configs/models/aots.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      174 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/configs/models/aott.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      206 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/configs/models/deaotb.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      289 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/configs/models/deaotl.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      206 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/configs/models/deaots.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      173 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/configs/models/deaott.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      957 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/configs/models/default.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      420 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/configs/models/default_deaot.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      545 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/configs/models/r101_aotl.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      541 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/configs/models/r50_aotl.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      410 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/configs/models/r50_deaotl.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      585 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/configs/models/rs101_aotl.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      645 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/configs/models/swinb_aotl.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      451 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/configs/models/swinb_deaotl.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      513 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/configs/pre.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      690 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/configs/pre_dav.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      611 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/configs/pre_ytb.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      668 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/configs/pre_ytb_dav.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      251 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/configs/ytb.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 10:07:51.024937 castle_ai-0.0.5/castle/aot/dataloaders/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/dataloaders/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    14300 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/dataloaders/eval_datasets.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    19828 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/dataloaders/image_transforms.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    24642 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/dataloaders/train_datasets.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    23561 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/dataloaders/video_transforms.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 10:07:51.024937 castle_ai-0.0.5/castle/aot/networks/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 04:49:47.000000 castle_ai-0.0.5/castle/aot/networks/__init__.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 10:07:51.024937 castle_ai-0.0.5/castle/aot/networks/decoders/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      186 2024-05-22 05:12:26.000000 castle_ai-0.0.5/castle/aot/networks/decoders/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     2079 2024-05-22 05:13:06.000000 castle_ai-0.0.5/castle/aot/networks/decoders/fpn.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 10:07:51.024937 castle_ai-0.0.5/castle/aot/networks/encoders/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1307 2024-05-22 05:08:31.000000 castle_ai-0.0.5/castle/aot/networks/encoders/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     8427 2024-05-22 05:06:53.000000 castle_ai-0.0.5/castle/aot/networks/encoders/mobilenetv2.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     7907 2024-05-22 05:07:00.000000 castle_ai-0.0.5/castle/aot/networks/encoders/mobilenetv3.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 10:07:51.024937 castle_ai-0.0.5/castle/aot/networks/encoders/resnest/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)       23 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/networks/encoders/resnest/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     3343 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/networks/encoders/resnest/resnest.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    16481 2024-05-22 05:10:30.000000 castle_ai-0.0.5/castle/aot/networks/encoders/resnest/resnet.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     4467 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/networks/encoders/resnest/splat.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     6699 2024-05-22 05:07:30.000000 castle_ai-0.0.5/castle/aot/networks/encoders/resnet.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 10:07:51.024937 castle_ai-0.0.5/castle/aot/networks/encoders/swin/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)       35 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/networks/encoders/swin/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      987 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/networks/encoders/swin/build.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    27369 2024-05-22 05:10:57.000000 castle_ai-0.0.5/castle/aot/networks/encoders/swin/swin_transformer.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 10:07:51.024937 castle_ai-0.0.5/castle/aot/networks/engines/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      653 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/networks/engines/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    25206 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/networks/engines/aot_engine.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     5978 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/networks/engines/deaot_engine.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 10:07:51.024937 castle_ai-0.0.5/castle/aot/networks/layers/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/networks/layers/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    32865 2024-05-22 05:11:50.000000 castle_ai-0.0.5/castle/aot/networks/layers/attention.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     5111 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/networks/layers/basic.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     6698 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/networks/layers/loss.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1700 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/networks/layers/normalization.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     2834 2024-05-22 05:12:08.000000 castle_ai-0.0.5/castle/aot/networks/layers/position.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    24810 2024-05-22 05:11:35.000000 castle_ai-0.0.5/castle/aot/networks/layers/transformer.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 10:07:51.024937 castle_ai-0.0.5/castle/aot/networks/models/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      358 2024-05-22 04:45:04.000000 castle_ai-0.0.5/castle/aot/networks/models/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     4574 2024-05-22 05:03:48.000000 castle_ai-0.0.5/castle/aot/networks/models/aot.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     2109 2024-05-22 05:13:44.000000 castle_ai-0.0.5/castle/aot/networks/models/deaot.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 10:07:51.024937 castle_ai-0.0.5/castle/aot/utils/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/utils/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     6233 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/utils/checkpoint.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1358 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/utils/cp_ckpt.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     3561 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/utils/ema.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      443 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/utils/eval.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     6075 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/utils/image.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     3454 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/utils/learning.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      829 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/utils/math.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      860 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/utils/meters.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1102 2024-05-22 03:59:14.000000 castle_ai-0.0.5/castle/aot/utils/metric.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 10:07:51.024937 castle_ai-0.0.5/castle/sam/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        0 2024-05-22 04:03:33.000000 castle_ai-0.0.5/castle/sam/__init__.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 10:07:51.024937 castle_ai-0.0.5/castle/sam/segment_anything/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      427 2024-05-22 04:03:33.000000 castle_ai-0.0.5/castle/sam/segment_anything/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    15132 2024-05-22 04:03:33.000000 castle_ai-0.0.5/castle/sam/segment_anything/automatic_mask_generator.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     2941 2024-05-22 04:03:33.000000 castle_ai-0.0.5/castle/sam/segment_anything/build_sam.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 10:07:51.028937 castle_ai-0.0.5/castle/sam/segment_anything/modeling/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      385 2024-05-22 04:03:33.000000 castle_ai-0.0.5/castle/sam/segment_anything/modeling/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1479 2024-05-22 04:03:33.000000 castle_ai-0.0.5/castle/sam/segment_anything/modeling/common.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    14407 2024-05-22 04:03:33.000000 castle_ai-0.0.5/castle/sam/segment_anything/modeling/image_encoder.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     6614 2024-05-22 04:03:33.000000 castle_ai-0.0.5/castle/sam/segment_anything/modeling/mask_decoder.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     8594 2024-05-22 04:03:33.000000 castle_ai-0.0.5/castle/sam/segment_anything/modeling/prompt_encoder.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     7225 2024-05-22 04:03:33.000000 castle_ai-0.0.5/castle/sam/segment_anything/modeling/sam.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     8396 2024-05-22 04:03:33.000000 castle_ai-0.0.5/castle/sam/segment_anything/modeling/transformer.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    11818 2024-05-22 04:03:33.000000 castle_ai-0.0.5/castle/sam/segment_anything/predictor.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 10:07:51.028937 castle_ai-0.0.5/castle/sam/segment_anything/utils/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      197 2024-05-22 04:03:33.000000 castle_ai-0.0.5/castle/sam/segment_anything/utils/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    12711 2024-05-22 04:03:33.000000 castle_ai-0.0.5/castle/sam/segment_anything/utils/amg.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     5790 2024-05-22 04:03:33.000000 castle_ai-0.0.5/castle/sam/segment_anything/utils/onnx.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     3968 2024-05-22 04:03:33.000000 castle_ai-0.0.5/castle/sam/segment_anything/utils/transforms.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      541 2024-05-22 04:03:33.000000 castle_ai-0.0.5/castle/sam/setup.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 10:07:51.028937 castle_ai-0.0.5/castle/ui/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)       30 2024-05-27 09:19:59.000000 castle_ai-0.0.5/castle/ui/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     4051 2024-05-27 09:19:59.000000 castle_ai-0.0.5/castle/ui/cluster_input_ui.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      793 2024-05-27 09:19:59.000000 castle_ai-0.0.5/castle/ui/cluster_page_ui.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1402 2024-05-27 09:19:59.000000 castle_ai-0.0.5/castle/ui/dbscan_ui.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     4597 2024-05-27 09:19:59.000000 castle_ai-0.0.5/castle/ui/dimension_reduction_ui.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     3919 2024-05-27 09:26:22.000000 castle_ai-0.0.5/castle/ui/edit_ui.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     6432 2024-05-27 09:51:00.000000 castle_ai-0.0.5/castle/ui/extract_ui.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     4055 2024-05-27 09:34:46.000000 castle_ai-0.0.5/castle/ui/label_ui.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     2498 2024-05-27 09:19:59.000000 castle_ai-0.0.5/castle/ui/main_ui.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     7595 2024-05-27 09:20:00.000000 castle_ai-0.0.5/castle/ui/post_track_ui.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     3780 2024-05-27 09:20:00.000000 castle_ai-0.0.5/castle/ui/project_ui.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     4048 2024-05-27 09:20:00.000000 castle_ai-0.0.5/castle/ui/source_ui.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)    10056 2024-05-27 09:20:00.000000 castle_ai-0.0.5/castle/ui/track_ui.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     2187 2024-05-27 09:20:00.000000 castle_ai-0.0.5/castle/ui/view_ui.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 10:07:51.028937 castle_ai-0.0.5/castle/utils/
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)      137 2024-05-24 08:01:14.000000 castle_ai-0.0.5/castle/utils/__init__.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1002 2024-05-23 07:41:10.000000 castle_ai-0.0.5/castle/utils/download.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1357 2024-05-27 09:37:28.000000 castle_ai-0.0.5/castle/utils/h5_io.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     6382 2024-05-23 08:44:58.000000 castle_ai-0.0.5/castle/utils/image_segment.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     5615 2024-05-27 09:44:44.000000 castle_ai-0.0.5/castle/utils/latent_explorer.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     1505 2024-05-27 09:34:27.000000 castle_ai-0.0.5/castle/utils/plot.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     3448 2024-05-24 06:17:35.000000 castle_ai-0.0.5/castle/utils/video_align.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     2524 2024-05-22 04:09:41.000000 castle_ai-0.0.5/castle/utils/video_io.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     8545 2024-05-23 07:50:24.000000 castle_ai-0.0.5/castle/utils/video_object_segment.py
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     3505 2024-05-24 08:36:28.000000 castle_ai-0.0.5/castle/utils/visual_latent_extract.py
+drwxrwxr-x   0 raiso     (1000) raiso     (1000)        0 2024-05-27 10:07:51.028937 castle_ai-0.0.5/castle_ai.egg-info/
+-rw-r--r--   0 raiso     (1000) raiso     (1000)     1728 2024-05-27 10:07:50.000000 castle_ai-0.0.5/castle_ai.egg-info/PKG-INFO
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     4073 2024-05-27 10:07:51.000000 castle_ai-0.0.5/castle_ai.egg-info/SOURCES.txt
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        1 2024-05-27 10:07:50.000000 castle_ai-0.0.5/castle_ai.egg-info/dependency_links.txt
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        1 2024-05-23 00:05:44.000000 castle_ai-0.0.5/castle_ai.egg-info/not-zip-safe
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)       68 2024-05-27 10:07:50.000000 castle_ai-0.0.5/castle_ai.egg-info/requires.txt
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)        7 2024-05-27 10:07:50.000000 castle_ai-0.0.5/castle_ai.egg-info/top_level.txt
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)       38 2024-05-27 10:07:51.028937 castle_ai-0.0.5/setup.cfg
+-rw-rw-r--   0 raiso     (1000) raiso     (1000)     2004 2024-05-27 10:07:49.000000 castle_ai-0.0.5/setup.py
```

### Comparing `castle_ai-0.0.4/PKG-INFO` & `castle_ai-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: castle-ai
-Version: 0.0.4
+Version: 0.0.5
 Summary: Distinguish behavioral clusters Toolbox
 Maintainer: Raiso Liu
 Maintainer-email: rainsoon717@gmail.com
 License: AGPL-3.0 license
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `castle_ai-0.0.4/README.md` & `castle_ai-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/configs/default.py` & `castle_ai-0.0.5/castle/aot/configs/default.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/configs/models/default.py` & `castle_ai-0.0.5/castle/aot/configs/models/default.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/configs/models/r101_aotl.py` & `castle_ai-0.0.5/castle/aot/configs/models/r101_aotl.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/configs/models/r50_aotl.py` & `castle_ai-0.0.5/castle/aot/configs/models/r50_aotl.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/configs/models/rs101_aotl.py` & `castle_ai-0.0.5/castle/aot/configs/models/rs101_aotl.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/configs/models/swinb_aotl.py` & `castle_ai-0.0.5/castle/aot/configs/models/swinb_aotl.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/configs/pre.py` & `castle_ai-0.0.5/castle/aot/configs/pre.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/configs/pre_dav.py` & `castle_ai-0.0.5/castle/aot/configs/pre_dav.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/configs/pre_ytb.py` & `castle_ai-0.0.5/castle/aot/configs/pre_ytb.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/configs/pre_ytb_dav.py` & `castle_ai-0.0.5/castle/aot/configs/pre_ytb_dav.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/dataloaders/eval_datasets.py` & `castle_ai-0.0.5/castle/aot/dataloaders/eval_datasets.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/dataloaders/image_transforms.py` & `castle_ai-0.0.5/castle/aot/dataloaders/image_transforms.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/dataloaders/train_datasets.py` & `castle_ai-0.0.5/castle/aot/dataloaders/train_datasets.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/dataloaders/video_transforms.py` & `castle_ai-0.0.5/castle/aot/dataloaders/video_transforms.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/networks/decoders/fpn.py` & `castle_ai-0.0.5/castle/aot/networks/decoders/fpn.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/networks/encoders/__init__.py` & `castle_ai-0.0.5/castle/aot/networks/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/networks/encoders/mobilenetv2.py` & `castle_ai-0.0.5/castle/aot/networks/encoders/mobilenetv2.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/networks/encoders/mobilenetv3.py` & `castle_ai-0.0.5/castle/aot/networks/encoders/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/networks/encoders/resnest/resnest.py` & `castle_ai-0.0.5/castle/aot/networks/encoders/resnest/resnest.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/networks/encoders/resnest/resnet.py` & `castle_ai-0.0.5/castle/aot/networks/encoders/resnest/resnet.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/networks/encoders/resnest/splat.py` & `castle_ai-0.0.5/castle/aot/networks/encoders/resnest/splat.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/networks/encoders/resnet.py` & `castle_ai-0.0.5/castle/aot/networks/encoders/resnet.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/networks/encoders/swin/build.py` & `castle_ai-0.0.5/castle/aot/networks/encoders/swin/build.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/networks/encoders/swin/swin_transformer.py` & `castle_ai-0.0.5/castle/aot/networks/encoders/swin/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/networks/engines/__init__.py` & `castle_ai-0.0.5/castle/aot/networks/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/networks/engines/aot_engine.py` & `castle_ai-0.0.5/castle/aot/networks/engines/aot_engine.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/networks/engines/deaot_engine.py` & `castle_ai-0.0.5/castle/aot/networks/engines/deaot_engine.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/networks/layers/attention.py` & `castle_ai-0.0.5/castle/aot/networks/layers/attention.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/networks/layers/basic.py` & `castle_ai-0.0.5/castle/aot/networks/layers/basic.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/networks/layers/loss.py` & `castle_ai-0.0.5/castle/aot/networks/layers/loss.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/networks/layers/normalization.py` & `castle_ai-0.0.5/castle/aot/networks/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/networks/layers/position.py` & `castle_ai-0.0.5/castle/aot/networks/layers/position.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/networks/layers/transformer.py` & `castle_ai-0.0.5/castle/aot/networks/layers/transformer.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/networks/models/aot.py` & `castle_ai-0.0.5/castle/aot/networks/models/aot.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/networks/models/deaot.py` & `castle_ai-0.0.5/castle/aot/networks/models/deaot.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/utils/checkpoint.py` & `castle_ai-0.0.5/castle/aot/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/utils/cp_ckpt.py` & `castle_ai-0.0.5/castle/aot/utils/cp_ckpt.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/utils/ema.py` & `castle_ai-0.0.5/castle/aot/utils/ema.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/utils/image.py` & `castle_ai-0.0.5/castle/aot/utils/image.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/utils/learning.py` & `castle_ai-0.0.5/castle/aot/utils/learning.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/utils/math.py` & `castle_ai-0.0.5/castle/aot/utils/math.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/utils/meters.py` & `castle_ai-0.0.5/castle/aot/utils/meters.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/aot/utils/metric.py` & `castle_ai-0.0.5/castle/aot/utils/metric.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/sam/segment_anything/automatic_mask_generator.py` & `castle_ai-0.0.5/castle/sam/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/sam/segment_anything/build_sam.py` & `castle_ai-0.0.5/castle/sam/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/sam/segment_anything/modeling/common.py` & `castle_ai-0.0.5/castle/sam/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/sam/segment_anything/modeling/image_encoder.py` & `castle_ai-0.0.5/castle/sam/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/sam/segment_anything/modeling/mask_decoder.py` & `castle_ai-0.0.5/castle/sam/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/sam/segment_anything/modeling/prompt_encoder.py` & `castle_ai-0.0.5/castle/sam/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/sam/segment_anything/modeling/sam.py` & `castle_ai-0.0.5/castle/sam/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/sam/segment_anything/modeling/transformer.py` & `castle_ai-0.0.5/castle/sam/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/sam/segment_anything/predictor.py` & `castle_ai-0.0.5/castle/sam/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/sam/segment_anything/utils/amg.py` & `castle_ai-0.0.5/castle/sam/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/sam/segment_anything/utils/onnx.py` & `castle_ai-0.0.5/castle/sam/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/sam/segment_anything/utils/transforms.py` & `castle_ai-0.0.5/castle/sam/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/sam/setup.py` & `castle_ai-0.0.5/castle/sam/setup.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/utils/download.py` & `castle_ai-0.0.5/castle/utils/download.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/utils/image_segment.py` & `castle_ai-0.0.5/castle/utils/image_segment.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/utils/latent_explorer.py` & `castle_ai-0.0.5/castle/utils/latent_explorer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from umap import UMAP
+
 from sklearn.cluster import DBSCAN, HDBSCAN
 
 
 import matplotlib.pyplot as plt
 from matplotlib.patches import Patch
 
 
@@ -14,26 +14,27 @@
 def palette(x):
     if x == -1:
         return '#DDDDDD'
     return _palette[x % len(_palette)]
 
 
 class Latent:
-    def __init__(self, raw, time_window=1):
+    def __init__(self, raw, time_window=1, device='cpu'):
         n = len(raw) // time_window
         num_feature = raw.shape[-1]
         self.time_window = time_window
         self.data = raw.reshape((-1,  num_feature * time_window))
         self.cluster = np.zeros(len(self.data)).astype(int)
         self.cluster[np.isnan(self.data.sum(axis=1))] = -1
         self.num_cluster = 1
         self.need_maintain_key_frames = True
+        self.device=device
 
     def select(self, cluster_id):
-        return LocalLatent(self.data[self.cluster == cluster_id], self.cluster == cluster_id)
+        return LocalLatent(self.data[self.cluster == cluster_id], self.cluster == cluster_id, device=self.device)
     
     def merge(self, cluster_ids):
         cluster_ids = np.array(cluster_ids)
         mi = cluster_ids.min()
 
         for it in cluster_ids:
             self.cluster[self.cluster == it] = mi
@@ -83,21 +84,27 @@
         self.need_maintain_key_frames = True
 
 
 
 
 
 class LocalLatent:
-    def __init__(self, data, index_mask):
+    def __init__(self, data, index_mask, device):
         self.data = data
         self.index_mask = index_mask
+        self.device = device
+
 
         
 
     def build_embedding(self, configs):
+        if self.device == 'cpu':
+            from umap import UMAP
+        elif self.device == 'gpu':
+            from cuml.manifold import UMAP
         Z = self.data
         if hasattr(self, 'embedding'):
             delattr(self, 'embedding')
 
         if not type(configs) == list:
             configs = [configs]
 
@@ -105,14 +112,19 @@
             Z = UMAP(**it).fit_transform(Z)
 
         self.embedding = Z
 
 
 
     def build_cluster(self, method, configs):
+        if self.device == 'cpu':
+            from sklearn.cluster import DBSCAN, HDBSCAN
+        elif self.device == 'gpu':
+            from cuml.cluster import DBSCAN, HDBSCAN
+
         assert hasattr(self, 'embedding')
         if hasattr(self, 'cluster'):
             delattr(self, 'cluster')
 
 
         if method == 'hdbscan':
             self.cluster = HDBSCAN(**configs).fit_predict(self.embedding)
@@ -137,12 +149,20 @@
                             c='grey',
                             label=f'-1')
             plt.legend()
         else:
             plt.scatter(x=self.embedding[:,dims[0]], 
                         y=self.embedding[:,dims[1]], 
                         c='grey')
+            
+    def merge(self, cluster_ids):
+        cluster_ids = np.array(cluster_ids)
+        mi = cluster_ids.min()
+
+        for it in cluster_ids:
+            self.cluster[self.cluster == it] = mi
+
```

### Comparing `castle_ai-0.0.4/castle/utils/video_align.py` & `castle_ai-0.0.5/castle/utils/video_align.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/utils/video_io.py` & `castle_ai-0.0.5/castle/utils/video_io.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/utils/video_object_segment.py` & `castle_ai-0.0.5/castle/utils/video_object_segment.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle/utils/visual_latent_extract.py` & `castle_ai-0.0.5/castle/utils/visual_latent_extract.py`

 * *Files identical despite different names*

### Comparing `castle_ai-0.0.4/castle_ai.egg-info/PKG-INFO` & `castle_ai-0.0.5/castle_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: castle-ai
-Version: 0.0.4
+Version: 0.0.5
 Summary: Distinguish behavioral clusters Toolbox
 Maintainer: Raiso Liu
 Maintainer-email: rainsoon717@gmail.com
 License: AGPL-3.0 license
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `castle_ai-0.0.4/castle_ai.egg-info/SOURCES.txt` & `castle_ai-0.0.5/castle_ai.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -81,16 +81,31 @@
 castle/sam/segment_anything/modeling/prompt_encoder.py
 castle/sam/segment_anything/modeling/sam.py
 castle/sam/segment_anything/modeling/transformer.py
 castle/sam/segment_anything/utils/__init__.py
 castle/sam/segment_anything/utils/amg.py
 castle/sam/segment_anything/utils/onnx.py
 castle/sam/segment_anything/utils/transforms.py
+castle/ui/__init__.py
+castle/ui/cluster_input_ui.py
+castle/ui/cluster_page_ui.py
+castle/ui/dbscan_ui.py
+castle/ui/dimension_reduction_ui.py
+castle/ui/edit_ui.py
+castle/ui/extract_ui.py
+castle/ui/label_ui.py
+castle/ui/main_ui.py
+castle/ui/post_track_ui.py
+castle/ui/project_ui.py
+castle/ui/source_ui.py
+castle/ui/track_ui.py
+castle/ui/view_ui.py
 castle/utils/__init__.py
 castle/utils/download.py
+castle/utils/h5_io.py
 castle/utils/image_segment.py
 castle/utils/latent_explorer.py
 castle/utils/plot.py
 castle/utils/video_align.py
 castle/utils/video_io.py
 castle/utils/video_object_segment.py
 castle/utils/visual_latent_extract.py
```

### Comparing `castle_ai-0.0.4/setup.py` & `castle_ai-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         with io.open("README.md", encoding="UTF-8") as readme_file:
             return readme_file.read()
 
 
 
 configuration = {
     "name": "castle-ai",
-    "version": "0.0.4",
+    "version": "0.0.5",
     "description": "Distinguish behavioral clusters Toolbox",
     "long_description": readme(),
     "long_description_content_type": "text/markdown",
     "classifiers": [
         "Development Status :: 1 - Planning",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
```

