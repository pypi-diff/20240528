# Comparing `tmp/alabamaencoder-0.4.2.tar.gz` & `tmp/alabamaencoder-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alabamaencoder-0.4.2.tar", last modified: Sat May 25 14:13:37 2024, max compression
+gzip compressed data, was "alabamaencoder-0.4.3.tar", last modified: Tue May 28 14:27:46 2024, max compression
```

## Comparing `alabamaencoder-0.4.2.tar` & `alabamaencoder-0.4.3.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.158367 alabamaencoder-0.4.2/
--rw-r--r--   0 kokoniara  (1000) kokoniara  (1000)      377 2024-05-25 14:13:37.158367 alabamaencoder-0.4.2/PKG-INFO
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.142367 alabamaencoder-0.4.2/alabamaEncode/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2021-04-17 09:55:33.000000 alabamaencoder-0.4.2/alabamaEncode/__init__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.142367 alabamaencoder-0.4.2/alabamaEncode/ai_vmaf/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-03 08:49:47.000000 alabamaencoder-0.4.2/alabamaEncode/ai_vmaf/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1554 2023-12-13 17:07:22.000000 alabamaencoder-0.4.2/alabamaEncode/ai_vmaf/aom_firstpass.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1026 2023-12-18 07:05:43.000000 alabamaencoder-0.4.2/alabamaEncode/ai_vmaf/perdict.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.146367 alabamaencoder-0.4.2/alabamaEncode/ai_vmaf/train/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-03 10:35:40.000000 alabamaencoder-0.4.2/alabamaEncode/ai_vmaf/train/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    12402 2023-12-14 22:03:21.000000 alabamaencoder-0.4.2/alabamaEncode/ai_vmaf/train/train.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.146367 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:25:35.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/__init__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.146367 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:26:35.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/__init__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.146367 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-01-17 00:34:57.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      671 2024-01-17 00:37:48.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/capped_crf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1064 2024-01-17 00:37:48.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/manual_crf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3401 2024-03-05 22:28:46.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/multires_encode_candidates.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4061 2024-02-04 12:03:51.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/optimised_vbr.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    10661 2024-04-29 21:50:58.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/per_scene_grain.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      597 2024-01-17 00:37:48.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_crf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      606 2024-01-17 00:37:48.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_vbr.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5578 2024-05-03 21:10:20.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/target_vmaf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      448 2023-12-10 19:05:23.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/chunk_analyse_step.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      623 2023-12-05 14:54:46.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_step.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.146367 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-05 14:55:01.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      684 2024-01-17 00:37:48.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/ai_targeted_vmaf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1584 2024-01-17 00:37:48.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/capped_crf_encode.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11063 2024-04-22 19:10:58.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6476 2024-02-04 12:12:23.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf_vbr.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2292 2024-03-05 22:27:27.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/multires_encode_finals.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      859 2024-02-02 15:57:21.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/plain.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2362 2024-05-20 19:14:36.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/opinionated_vmaf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5927 2024-03-05 22:32:37.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/pipelines.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      133 2024-01-15 01:49:31.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/refine_step.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.146367 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/refine_steps/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-01-14 19:17:26.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/refine_steps/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4955 2024-03-05 20:43:08.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/refine_steps/multires_package.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7817 2024-01-20 18:40:41.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/refine_steps/multires_trellis.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.146367 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:26:49.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1563 2024-05-20 13:32:49.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/args_tune.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4687 2024-04-27 00:03:05.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/autocrop.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      552 2024-01-25 02:38:21.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/denoise_filtering.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2409 2024-05-04 17:38:16.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/encoding_tiles.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9823 2024-02-04 12:39:56.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/ideal_crf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7511 2024-02-12 05:33:32.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/scrape_hdr_meta.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5986 2024-03-05 22:00:10.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/sequence_autograin.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3119 2024-02-02 18:54:38.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/taget_ssimdb.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6920 2024-02-04 12:09:55.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/target_bitrate_optimisation.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2777 2024-02-04 12:09:55.000000 alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/x264_tune.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.150367 alabamaencoder-0.4.2/alabamaEncode/core/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-11-19 23:19:38.000000 alabamaencoder-0.4.2/alabamaEncode/core/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    10800 2024-05-04 17:37:43.000000 alabamaencoder-0.4.2/alabamaEncode/core/alabama.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2879 2024-02-21 15:17:46.000000 alabamaencoder-0.4.2/alabamaEncode/core/bin_utils.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3878 2024-05-02 23:47:10.000000 alabamaencoder-0.4.2/alabamaEncode/core/chunk_job.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4947 2024-01-31 09:31:42.000000 alabamaencoder-0.4.2/alabamaEncode/core/cli_executor.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.150367 alabamaencoder-0.4.2/alabamaEncode/core/extras/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-24 18:44:15.000000 alabamaencoder-0.4.2/alabamaEncode/core/extras/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11151 2024-05-25 13:48:52.000000 alabamaencoder-0.4.2/alabamaEncode/core/extras/auto_thumbnailer.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    13706 2024-03-22 06:24:59.000000 alabamaencoder-0.4.2/alabamaEncode/core/ffmpeg.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5661 2024-05-07 20:56:31.000000 alabamaencoder-0.4.2/alabamaEncode/core/final_touches.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    19276 2024-05-04 17:36:30.000000 alabamaencoder-0.4.2/alabamaEncode/core/job.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1877 2024-04-22 19:11:27.000000 alabamaencoder-0.4.2/alabamaEncode/core/kv.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      813 2023-11-25 00:35:54.000000 alabamaencoder-0.4.2/alabamaEncode/core/path.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      556 2023-11-12 21:29:16.000000 alabamaencoder-0.4.2/alabamaEncode/core/timer.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1776 2023-12-24 03:53:49.000000 alabamaencoder-0.4.2/alabamaEncode/core/ws_update.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.150367 alabamaencoder-0.4.2/alabamaEncode/encoder/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-09-27 12:09:43.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      748 2024-01-17 00:16:49.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/codec.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11438 2024-04-26 23:55:50.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/encoder.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1536 2024-02-12 05:37:04.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/encoder_factory.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.150367 alabamaencoder-0.4.2/alabamaEncode/encoder/impl/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4369 2024-02-12 05:35:10.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/impl/Aomenc.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2087 2024-02-12 05:35:10.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/impl/Nvenc.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1586 2024-01-28 06:23:47.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/impl/SvtAvif.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7642 2024-04-26 23:56:02.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/impl/Svtenc.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2172 2024-02-12 05:35:10.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/impl/VaapiH264.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2114 2024-03-23 06:39:42.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/impl/VaapiH265.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7238 2024-02-12 05:35:10.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/impl/X264.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4097 2024-02-12 05:35:10.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/impl/X265.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2022-12-05 03:43:14.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/impl/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2033 2024-02-12 05:35:10.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/impl/rav1e.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3557 2024-02-12 05:35:10.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/impl/vp9.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      269 2024-01-17 00:14:46.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/rate_dist.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2494 2024-02-04 12:07:28.000000 alabamaencoder-0.4.2/alabamaEncode/encoder/stats.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.154367 alabamaencoder-0.4.2/alabamaEncode/experiments/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3713 2023-12-11 23:14:15.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/Aq.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4337 2023-12-11 23:14:15.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/Overlays.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2950 2024-02-02 15:19:02.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/Svtav1Speed.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5719 2023-12-11 23:14:15.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/Svtav1Tunes.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3749 2023-12-11 23:14:15.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/TemporalFiltering.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-06 18:23:30.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2496 2023-12-02 16:35:17.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/ai_feature_extract.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      319 2023-12-10 22:37:13.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/aom_extract.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5812 2024-02-04 12:09:55.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/convexhull.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    16885 2024-02-04 12:09:55.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/crf_vmaf_relation.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4941 2024-02-04 12:09:55.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/denoise.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2210 2024-02-04 12:09:55.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/sequence_convex.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      254 2023-12-20 04:58:54.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/serialise_context.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      793 2023-12-31 13:08:11.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/streaming_output.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6592 2023-12-11 23:14:15.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/superres.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4106 2023-11-15 20:26:48.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/target_vmaf.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.154367 alabamaencoder-0.4.2/alabamaEncode/experiments/util/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11478 2024-02-04 12:09:55.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/util/ExperimentUtil.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-10-17 18:48:28.000000 alabamaencoder-0.4.2/alabamaEncode/experiments/util/__init__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.154367 alabamaencoder-0.4.2/alabamaEncode/ffmpeg_source/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-21 17:50:35.000000 alabamaencoder-0.4.2/alabamaEncode/ffmpeg_source/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      837 2024-05-24 18:46:29.000000 alabamaencoder-0.4.2/alabamaEncode/ffmpeg_source/ffmpeg_src.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3758 2024-05-22 16:28:12.000000 alabamaencoder-0.4.2/alabamaEncode/ffmpeg_source/yuv.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.154367 alabamaencoder-0.4.2/alabamaEncode/metrics/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-11-17 22:15:46.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5237 2024-02-04 12:44:56.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/calculate.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      911 2023-11-22 22:07:47.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/comparison_display.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      384 2024-01-26 03:01:39.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/exception.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3033 2023-11-19 23:24:09.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/image.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.154367 alabamaencoder-0.4.2/alabamaEncode/metrics/impl/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-02-04 12:02:29.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/impl/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      924 2023-11-19 23:28:00.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/impl/psnr.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1432 2023-11-25 03:14:34.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/impl/ssim.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3093 2024-02-05 00:20:43.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/impl/ssimu2.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9052 2024-02-05 00:40:43.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/impl/vmaf.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      117 2024-02-04 12:09:55.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/metric.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      373 2024-02-04 12:36:30.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/options.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      308 2024-02-02 14:53:33.000000 alabamaencoder-0.4.2/alabamaEncode/metrics/result.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.154367 alabamaencoder-0.4.2/alabamaEncode/parallelEncoding/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2357 2024-01-07 02:35:39.000000 alabamaencoder-0.4.2/alabamaEncode/parallelEncoding/CeleryApp.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3848 2023-11-19 23:24:09.000000 alabamaencoder-0.4.2/alabamaEncode/parallelEncoding/CeleryAutoscaler.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-16 16:38:33.000000 alabamaencoder-0.4.2/alabamaEncode/parallelEncoding/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      148 2023-11-05 09:04:10.000000 alabamaencoder-0.4.2/alabamaEncode/parallelEncoding/command.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    12819 2024-04-21 00:03:18.000000 alabamaencoder-0.4.2/alabamaEncode/parallelEncoding/execute_commands.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      581 2024-01-07 00:27:19.000000 alabamaencoder-0.4.2/alabamaEncode/parallelEncoding/worker.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.154367 alabamaencoder-0.4.2/alabamaEncode/scene/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-15 20:18:27.000000 alabamaencoder-0.4.2/alabamaEncode/scene/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1810 2024-03-29 15:35:11.000000 alabamaencoder-0.4.2/alabamaEncode/scene/annel.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9690 2024-05-04 17:06:53.000000 alabamaencoder-0.4.2/alabamaEncode/scene/chunk.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    13305 2024-05-13 18:43:21.000000 alabamaencoder-0.4.2/alabamaEncode/scene/concat.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4451 2024-05-04 17:06:53.000000 alabamaencoder-0.4.2/alabamaEncode/scene/sequence.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11219 2024-05-04 17:23:39.000000 alabamaencoder-0.4.2/alabamaEncode/scene/split.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.154367 alabamaencoder-0.4.2/alabamaEncode_frontends/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:32:46.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/__init__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.158367 alabamaencoder-0.4.2/alabamaEncode_frontends/cli/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:52:09.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/cli/__init__.py
--rwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)     4366 2024-03-22 06:30:36.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/cli/__main__.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.158367 alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 18:44:18.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4150 2024-03-05 20:36:01.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/autopaths.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    20157 2024-03-29 15:04:00.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/cli_args.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1162 2024-03-05 20:46:37.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/paths.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1088 2024-01-23 00:24:16.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/ratecontrol.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1130 2023-12-10 18:44:44.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/res_preset.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1987 2024-05-04 17:19:56.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/validate_files.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1177 2024-03-17 23:12:31.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/video_filters.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.158367 alabamaencoder-0.4.2/alabamaEncode_frontends/demon/
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:38:55.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/demon/__init__.py
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2289 2024-03-05 20:43:08.000000 alabamaencoder-0.4.2/alabamaEncode_frontends/demon/demon.py
-drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-25 14:13:37.158367 alabamaencoder-0.4.2/alabamaEncoder.egg-info/
--rw-r--r--   0 kokoniara  (1000) kokoniara  (1000)      377 2024-05-25 14:13:37.000000 alabamaencoder-0.4.2/alabamaEncoder.egg-info/PKG-INFO
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6166 2024-05-25 14:13:37.000000 alabamaencoder-0.4.2/alabamaEncoder.egg-info/SOURCES.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        1 2024-05-25 14:13:37.000000 alabamaencoder-0.4.2/alabamaEncoder.egg-info/dependency_links.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       77 2024-05-25 14:13:37.000000 alabamaencoder-0.4.2/alabamaEncoder.egg-info/entry_points.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      124 2024-05-25 14:13:37.000000 alabamaencoder-0.4.2/alabamaEncoder.egg-info/requires.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       38 2024-05-25 14:13:37.000000 alabamaencoder-0.4.2/alabamaEncoder.egg-info/top_level.txt
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       38 2024-05-25 14:13:37.158367 alabamaencoder-0.4.2/setup.cfg
--rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      548 2024-05-25 14:12:58.000000 alabamaencoder-0.4.2/setup.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.910324 alabamaencoder-0.4.3/
+-rw-r--r--   0 kokoniara  (1000) kokoniara  (1000)      407 2024-05-28 14:27:46.910324 alabamaencoder-0.4.3/PKG-INFO
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.882323 alabamaencoder-0.4.3/alabamaEncode/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2021-04-17 09:55:33.000000 alabamaencoder-0.4.3/alabamaEncode/__init__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.882323 alabamaencoder-0.4.3/alabamaEncode/ai_vmaf/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-03 08:49:47.000000 alabamaencoder-0.4.3/alabamaEncode/ai_vmaf/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1554 2023-12-13 17:07:22.000000 alabamaencoder-0.4.3/alabamaEncode/ai_vmaf/aom_firstpass.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1026 2023-12-18 07:05:43.000000 alabamaencoder-0.4.3/alabamaEncode/ai_vmaf/perdict.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.882323 alabamaencoder-0.4.3/alabamaEncode/ai_vmaf/train/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-03 10:35:40.000000 alabamaencoder-0.4.3/alabamaEncode/ai_vmaf/train/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    12402 2023-12-14 22:03:21.000000 alabamaencoder-0.4.3/alabamaEncode/ai_vmaf/train/train.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.882323 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:25:35.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/__init__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.886324 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:26:35.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/__init__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.886324 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-01-17 00:34:57.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      671 2024-01-17 00:37:48.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/capped_crf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1064 2024-01-17 00:37:48.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/manual_crf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3401 2024-03-05 22:28:46.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/multires_encode_candidates.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4061 2024-02-04 12:03:51.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/optimised_vbr.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    10661 2024-04-29 21:50:58.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/per_scene_grain.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      597 2024-01-17 00:37:48.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_crf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      606 2024-01-17 00:37:48.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_vbr.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5578 2024-05-03 21:10:20.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/target_vmaf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      448 2023-12-10 19:05:23.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/chunk_analyse_step.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      623 2023-12-05 14:54:46.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_step.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.890324 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-05 14:55:01.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      684 2024-01-17 00:37:48.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/ai_targeted_vmaf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1584 2024-01-17 00:37:48.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/capped_crf_encode.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11063 2024-04-22 19:10:58.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6476 2024-02-04 12:12:23.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf_vbr.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2292 2024-03-05 22:27:27.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/multires_encode_finals.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      850 2024-05-28 14:05:00.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/plain.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2362 2024-05-20 19:14:36.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/opinionated_vmaf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5927 2024-03-05 22:32:37.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/pipelines.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      133 2024-01-15 01:49:31.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/refine_step.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.890324 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/refine_steps/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-01-14 19:17:26.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/refine_steps/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4955 2024-03-05 20:43:08.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/refine_steps/multires_package.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7817 2024-01-20 18:40:41.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/refine_steps/multires_trellis.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.890324 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 16:26:49.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1563 2024-05-20 13:32:49.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/args_tune.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4687 2024-04-27 00:03:05.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/autocrop.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      552 2024-01-25 02:38:21.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/denoise_filtering.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2409 2024-05-04 17:38:16.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/encoding_tiles.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9823 2024-02-04 12:39:56.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/ideal_crf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7511 2024-02-12 05:33:32.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/scrape_hdr_meta.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5986 2024-03-05 22:00:10.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/sequence_autograin.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3119 2024-02-02 18:54:38.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/taget_ssimdb.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6920 2024-02-04 12:09:55.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/target_bitrate_optimisation.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3103 2024-05-27 06:22:04.000000 alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/x264_tune.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.894324 alabamaencoder-0.4.3/alabamaEncode/core/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-11-19 23:19:38.000000 alabamaencoder-0.4.3/alabamaEncode/core/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    10874 2024-05-28 14:05:00.000000 alabamaencoder-0.4.3/alabamaEncode/core/alabama.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2890 2024-05-25 18:25:00.000000 alabamaencoder-0.4.3/alabamaEncode/core/bin_utils.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3878 2024-05-02 23:47:10.000000 alabamaencoder-0.4.3/alabamaEncode/core/chunk_job.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4947 2024-01-31 09:31:42.000000 alabamaencoder-0.4.3/alabamaEncode/core/cli_executor.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.894324 alabamaencoder-0.4.3/alabamaEncode/core/extras/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-24 18:44:15.000000 alabamaencoder-0.4.3/alabamaEncode/core/extras/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    12734 2024-05-26 19:36:14.000000 alabamaencoder-0.4.3/alabamaEncode/core/extras/auto_thumbnailer.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    13706 2024-03-22 06:24:59.000000 alabamaencoder-0.4.3/alabamaEncode/core/ffmpeg.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5661 2024-05-07 20:56:31.000000 alabamaencoder-0.4.3/alabamaEncode/core/final_touches.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    19276 2024-05-04 17:36:30.000000 alabamaencoder-0.4.3/alabamaEncode/core/job.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1877 2024-04-22 19:11:27.000000 alabamaencoder-0.4.3/alabamaEncode/core/kv.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      813 2023-11-25 00:35:54.000000 alabamaencoder-0.4.3/alabamaEncode/core/path.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      556 2023-11-12 21:29:16.000000 alabamaencoder-0.4.3/alabamaEncode/core/timer.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1776 2023-12-24 03:53:49.000000 alabamaencoder-0.4.3/alabamaEncode/core/ws_update.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.894324 alabamaencoder-0.4.3/alabamaEncode/encoder/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-09-27 12:09:43.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      748 2024-01-17 00:16:49.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/codec.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11438 2024-04-26 23:55:50.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/encoder.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1536 2024-02-12 05:37:04.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/encoder_factory.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.898324 alabamaencoder-0.4.3/alabamaEncode/encoder/impl/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4369 2024-02-12 05:35:10.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/impl/Aomenc.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2087 2024-02-12 05:35:10.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/impl/Nvenc.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1586 2024-01-28 06:23:47.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/impl/SvtAvif.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7662 2024-05-25 18:25:47.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/impl/Svtenc.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2172 2024-02-12 05:35:10.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/impl/VaapiH264.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2114 2024-03-23 06:39:42.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/impl/VaapiH265.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     7238 2024-02-12 05:35:10.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/impl/X264.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4097 2024-02-12 05:35:10.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/impl/X265.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2022-12-05 03:43:14.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/impl/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2033 2024-02-12 05:35:10.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/impl/rav1e.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3557 2024-02-12 05:35:10.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/impl/vp9.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      269 2024-01-17 00:14:46.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/rate_dist.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2494 2024-02-04 12:07:28.000000 alabamaencoder-0.4.3/alabamaEncode/encoder/stats.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.902324 alabamaencoder-0.4.3/alabamaEncode/experiments/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3713 2023-12-11 23:14:15.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/Aq.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4337 2023-12-11 23:14:15.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/Overlays.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2950 2024-02-02 15:19:02.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/Svtav1Speed.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5719 2023-12-11 23:14:15.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/Svtav1Tunes.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3749 2023-12-11 23:14:15.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/TemporalFiltering.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-06 18:23:30.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2496 2023-12-02 16:35:17.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/ai_feature_extract.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      319 2023-12-10 22:37:13.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/aom_extract.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5812 2024-02-04 12:09:55.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/convexhull.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    16885 2024-02-04 12:09:55.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/crf_vmaf_relation.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4941 2024-02-04 12:09:55.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/denoise.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2210 2024-02-04 12:09:55.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/sequence_convex.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      254 2023-12-20 04:58:54.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/serialise_context.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      793 2023-12-31 13:08:11.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/streaming_output.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6592 2023-12-11 23:14:15.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/superres.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4106 2023-11-15 20:26:48.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/target_vmaf.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.902324 alabamaencoder-0.4.3/alabamaEncode/experiments/util/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11478 2024-02-04 12:09:55.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/util/ExperimentUtil.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-10-17 18:48:28.000000 alabamaencoder-0.4.3/alabamaEncode/experiments/util/__init__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.902324 alabamaencoder-0.4.3/alabamaEncode/ffmpeg_source/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-21 17:50:35.000000 alabamaencoder-0.4.3/alabamaEncode/ffmpeg_source/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      837 2024-05-26 19:36:20.000000 alabamaencoder-0.4.3/alabamaEncode/ffmpeg_source/ffmpeg_src.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3758 2024-05-25 22:57:08.000000 alabamaencoder-0.4.3/alabamaEncode/ffmpeg_source/yuv.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.906324 alabamaencoder-0.4.3/alabamaEncode/metrics/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-11-17 22:15:46.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     5237 2024-02-04 12:44:56.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/calculate.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      911 2023-11-22 22:07:47.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/comparison_display.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      384 2024-01-26 03:01:39.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/exception.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3033 2023-11-19 23:24:09.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/image.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.906324 alabamaencoder-0.4.3/alabamaEncode/metrics/impl/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2024-02-04 12:02:29.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/impl/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      924 2023-11-19 23:28:00.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/impl/psnr.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1432 2023-11-25 03:14:34.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/impl/ssim.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3093 2024-02-05 00:20:43.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/impl/ssimu2.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9078 2024-05-28 13:30:59.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/impl/vmaf.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      117 2024-02-04 12:09:55.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/metric.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      373 2024-02-04 12:36:30.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/options.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      308 2024-02-02 14:53:33.000000 alabamaencoder-0.4.3/alabamaEncode/metrics/result.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.906324 alabamaencoder-0.4.3/alabamaEncode/parallelEncoding/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2357 2024-01-07 02:35:39.000000 alabamaencoder-0.4.3/alabamaEncode/parallelEncoding/CeleryApp.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     3848 2023-11-19 23:24:09.000000 alabamaencoder-0.4.3/alabamaEncode/parallelEncoding/CeleryAutoscaler.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-16 16:38:33.000000 alabamaencoder-0.4.3/alabamaEncode/parallelEncoding/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      148 2023-11-05 09:04:10.000000 alabamaencoder-0.4.3/alabamaEncode/parallelEncoding/command.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    12819 2024-04-21 00:03:18.000000 alabamaencoder-0.4.3/alabamaEncode/parallelEncoding/execute_commands.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      581 2024-01-07 00:27:19.000000 alabamaencoder-0.4.3/alabamaEncode/parallelEncoding/worker.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.906324 alabamaencoder-0.4.3/alabamaEncode/scene/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-04-15 20:18:27.000000 alabamaencoder-0.4.3/alabamaEncode/scene/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1810 2024-03-29 15:35:11.000000 alabamaencoder-0.4.3/alabamaEncode/scene/annel.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     9690 2024-05-04 17:06:53.000000 alabamaencoder-0.4.3/alabamaEncode/scene/chunk.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    13428 2024-05-25 14:27:51.000000 alabamaencoder-0.4.3/alabamaEncode/scene/concat.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4451 2024-05-04 17:06:53.000000 alabamaencoder-0.4.3/alabamaEncode/scene/sequence.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    11219 2024-05-04 17:23:39.000000 alabamaencoder-0.4.3/alabamaEncode/scene/split.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.910324 alabamaencoder-0.4.3/alabamaEncode_frontends/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:32:46.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/__init__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.910324 alabamaencoder-0.4.3/alabamaEncode_frontends/cli/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:52:09.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/cli/__init__.py
+-rwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)     4705 2024-05-26 19:26:41.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/cli/__main__.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.910324 alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-10 18:44:18.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     4150 2024-03-05 20:36:01.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/autopaths.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)    20449 2024-05-28 14:05:00.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/cli_args.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1162 2024-03-05 20:46:37.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/paths.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1088 2024-01-23 00:24:16.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/ratecontrol.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1130 2023-12-10 18:44:44.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/res_preset.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1987 2024-05-04 17:19:56.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/validate_files.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     1177 2024-03-17 23:12:31.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/video_filters.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.910324 alabamaencoder-0.4.3/alabamaEncode_frontends/demon/
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        0 2023-12-23 05:38:55.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/demon/__init__.py
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     2289 2024-03-05 20:43:08.000000 alabamaencoder-0.4.3/alabamaEncode_frontends/demon/demon.py
+drwxrwxr-x   0 kokoniara  (1000) kokoniara  (1000)        0 2024-05-28 14:27:46.910324 alabamaencoder-0.4.3/alabamaEncoder.egg-info/
+-rw-r--r--   0 kokoniara  (1000) kokoniara  (1000)      407 2024-05-28 14:27:46.000000 alabamaencoder-0.4.3/alabamaEncoder.egg-info/PKG-INFO
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)     6166 2024-05-28 14:27:46.000000 alabamaencoder-0.4.3/alabamaEncoder.egg-info/SOURCES.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)        1 2024-05-28 14:27:46.000000 alabamaencoder-0.4.3/alabamaEncoder.egg-info/dependency_links.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       77 2024-05-28 14:27:46.000000 alabamaencoder-0.4.3/alabamaEncoder.egg-info/entry_points.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      139 2024-05-28 14:27:46.000000 alabamaencoder-0.4.3/alabamaEncoder.egg-info/requires.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       38 2024-05-28 14:27:46.000000 alabamaencoder-0.4.3/alabamaEncoder.egg-info/top_level.txt
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)       38 2024-05-28 14:27:46.910324 alabamaencoder-0.4.3/setup.cfg
+-rw-rw-r--   0 kokoniara  (1000) kokoniara  (1000)      574 2024-05-28 14:15:56.000000 alabamaencoder-0.4.3/setup.py
```

### Comparing `alabamaencoder-0.4.2/alabamaEncode/ai_vmaf/aom_firstpass.py` & `alabamaencoder-0.4.3/alabamaEncode/ai_vmaf/aom_firstpass.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/ai_vmaf/perdict.py` & `alabamaencoder-0.4.3/alabamaEncode/ai_vmaf/perdict.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/ai_vmaf/train/train.py` & `alabamaencoder-0.4.3/alabamaEncode/ai_vmaf/train/train.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/capped_crf.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/capped_crf.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/manual_crf.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/manual_crf.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/multires_encode_candidates.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/multires_encode_candidates.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/optimised_vbr.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/optimised_vbr.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/per_scene_grain.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/per_scene_grain.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_crf.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_crf.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_vbr.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/plain_vbr.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/analyze_steps/target_vmaf.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/analyze_steps/target_vmaf.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_step.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_step.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/ai_targeted_vmaf.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/ai_targeted_vmaf.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/capped_crf_encode.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/capped_crf_encode.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf_vbr.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/dynamic_target_vmaf_vbr.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/multires_encode_finals.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/multires_encode_finals.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/chunk/final_encode_steps/plain.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/chunk/final_encode_steps/plain.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class PlainFinalEncode(FinalEncodeStep):
     def run(
         self, enc: Encoder, chunk: ChunkObject, ctx: AlabamaContext, encoded_a_frame
     ) -> EncodeStats:
         metric, _ = ctx.get_metric_target()
         return enc.run(
-            metric_to_calculate=metric if not ctx.dont_calc_final_vmaf else None,
+            metric_to_calculate=metric if ctx.calc_final_vmaf else None,
             metric_params=ctx.get_vmaf_options(),
             on_frame_encoded=encoded_a_frame,
         )
 
     def dry_run(self, enc: Encoder, chunk: ChunkObject) -> str:
         joined = " && ".join(enc.get_encode_commands())
         return joined
```

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/opinionated_vmaf.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/opinionated_vmaf.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/pipelines.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/pipelines.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/refine_steps/multires_package.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/refine_steps/multires_package.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/refine_steps/multires_trellis.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/refine_steps/multires_trellis.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/args_tune.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/args_tune.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/autocrop.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/autocrop.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/denoise_filtering.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/denoise_filtering.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/encoding_tiles.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/encoding_tiles.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/ideal_crf.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/ideal_crf.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/scrape_hdr_meta.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/scrape_hdr_meta.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/sequence_autograin.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/sequence_autograin.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/taget_ssimdb.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/taget_ssimdb.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/target_bitrate_optimisation.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/target_bitrate_optimisation.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/conent_analysis/sequence/x264_tune.py` & `alabamaencoder-0.4.3/alabamaEncode/conent_analysis/sequence/x264_tune.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 from alabamaEncode.core.alabama import AlabamaContext
 from alabamaEncode.encoder.impl.X264 import EncoderX264
 from alabamaEncode.metrics.metric import Metric
 from alabamaEncode.scene.sequence import ChunkSequence
 
 
 def run_tune(a):
-    tune, enc, path = a
+    tune, enc, path, vmaf_options = a
     enc.x264_tune = tune
     enc.output_path = os.path.join(path, f"{tune}{enc.get_chunk_file_extension()}")
-    stats = enc.run(metric_to_calculate=Metric.VMAF)
+    stats = enc.run(metric_to_calculate=Metric.VMAF, metric_params=vmaf_options)
     print(f"{tune}: {stats.bitrate}kb/s {stats.metric_results.harmonic_mean}vmaf")
     return tune, stats.metric_results.harmonic_mean, stats.bitrate
 
 
 def get_ideal_x264_tune(ctx: AlabamaContext, sequence: ChunkSequence):
     """
     Picks the ideal x264 tune for the sequence, based on the vmaf per bitrate
@@ -47,27 +47,35 @@
                 random_pick_count=2
             ):
                 enc.chunk = test_chunk
 
                 # get (tune, stats) tuples in a parallel fashion
                 with Pool() as p:
                     runs = p.map(
-                        run_tune, [(tune, enc.clone(), path) for tune in tunes]
+                        run_tune,
+                        [
+                            (tune, enc.clone(), path, ctx.get_vmaf_options())
+                            for tune in tunes
+                        ],
                     )
                     # and close the pool
                     p.close()
                     p.join()
 
                 # pick the tune with the biggest vmaf per bitrate with a little bias towards vmaf
-                runs_calculated = [
-                    (tune, ((vmaf / bitrate) + (vmaf / 100)))
-                    for tune, vmaf, bitrate in runs
-                ]
-                runs_calculated.sort(key=lambda x: x[1])
-                best_tune = runs_calculated[-1][0]
+                # runs_calculated = [
+                #     (tune, ((vmaf / bitrate) + (vmaf / 100)))
+                #     for tune, vmaf, bitrate in runs
+                # ]
+                # runs_calculated.sort(key=lambda x: x[1])
+                # best_tune = runs_calculated[-1][0]
+
+                # pick the tune with the biggest vmaf
+                runs.sort(key=lambda x: x[1])
+                best_tune = runs[-1][0]
 
                 best.append(best_tune)
 
             # pick the most common tune from the best tunes
             ctx.prototype_encoder.x264_tune = max(set(best), key=best.count)
             print(f"picked {ctx.prototype_encoder.x264_tune} as x264 tune")
             ctx.get_kv().set("x264_tune", "value", ctx.prototype_encoder.x264_tune)
```

### Comparing `alabamaencoder-0.4.2/alabamaEncode/core/alabama.py` & `alabamaencoder-0.4.3/alabamaEncode/core/alabama.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,15 @@
             raise RuntimeError("Invalid JSON")
         self.__dict__ = parser_dict
         return self
 
     def __iter__(self):
         return self.dict().__iter__()
 
+    standalone_autothumbnailer = False
     use_celery: bool = False
     offload_server = ""
     multiprocess_workers: int = -1
     throughput_scaling = False
     log_level: int = 0
     print_analysis_logs = False
     dry_run: bool = False
@@ -145,15 +146,15 @@
     bitrate_undershoot: float = 0.90
     bitrate_overshoot: float = 2
     bitrate_adjust_mode: str = ""
     cutoff_bitrate: int = -1
     max_bitrate: int = 0
     simple_denoise = False
     args_tune = "balanced"
-    dont_calc_final_vmaf = False
+    calc_final_vmaf = False
 
     metric_to_target = "vmaf"
     vmaf: int = 96
     denoise_vmaf_ref = False
     probe_count = 3
     vmaf_reference_display = ""
     crf_based_vmaf_targeting = True
@@ -218,17 +219,19 @@
                 "Prototype encoder is not set, this should be impossible"
             )
 
     def get_vmaf_options(self) -> VmafOptions:
         return VmafOptions(
             uhd=self.vmaf_4k_model,
             phone=self.vmaf_phone_model,
-            ref=ComparisonDisplayResolution.from_string(self.vmaf_reference_display)
-            if self.vmaf_reference_display
-            else None,
+            ref=(
+                ComparisonDisplayResolution.from_string(self.vmaf_reference_display)
+                if self.vmaf_reference_display
+                else None
+            ),
             no_motion=self.vmaf_no_motion,
             denoise_refrence=self.denoise_vmaf_ref,
         )
 
     def get_metric_target(self) -> Tuple[Metric, float]:
         """
         Return what metric and to what degree to target based on config
```

### Comparing `alabamaencoder-0.4.2/alabamaEncode/core/bin_utils.py` & `alabamaencoder-0.4.3/alabamaEncode/core/bin_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 Provides a central place to get the path to the binaries, and checks if they exist.
 Also includes checks if the binaries are what we need (e.g., ffmpeg has been compiled with certain flags)
 """
 
 import os
 from shutil import which
 
-__all__ = ["get_binary", "register_bin", "verify_ffmpeg_library"]
+__all__ = ["get_binary", "register_bin", "verify_ffmpeg_library", "check_bin"]
 
 from typing import List
 
 from alabamaEncode.core.cli_executor import run_cli
 
 bins = []
 
 
-def _check_bin(path) -> bool:
+def check_bin(path) -> bool:
     if path is None:
         return False
     _which = which(path) is not None
     if _which:
         return True
     else:
         if os.path.exists(path):
@@ -96,11 +96,11 @@
 
 def get_binary(name):
     _bin = os.getenv(f"{name.upper()}_CLI_PATH", name)
     if _bin == name:
         for _name, _cli in bins:
             if _name == name:
                 _bin = _cli
-    if _check_bin(_bin):
+    if check_bin(_bin):
         return _bin
     else:
         raise BinaryNotFound(name)
```

### Comparing `alabamaencoder-0.4.2/alabamaEncode/core/chunk_job.py` & `alabamaencoder-0.4.3/alabamaEncode/core/chunk_job.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/core/cli_executor.py` & `alabamaencoder-0.4.3/alabamaEncode/core/cli_executor.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/core/extras/auto_thumbnailer.py` & `alabamaencoder-0.4.3/alabamaEncode/core/extras/auto_thumbnailer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import multiprocessing
-import os.path
 
 import cv2
 import numpy as np
 import scipy
 from skimage.metrics import structural_similarity as ssim
 from tqdm import tqdm
 
-from alabamaEncode.core.bin_utils import get_binary
+from alabamaEncode.core.bin_utils import get_binary, check_ffmpeg_libraries, check_bin
 from alabamaEncode.core.cli_executor import run_cli
 from alabamaEncode.core.ffmpeg import Ffmpeg
 from alabamaEncode.core.path import PathAlabama
 from alabamaEncode.ffmpeg_source.ffmpeg_src import get_yuv_frame_stream
 from alabamaEncode.scene.chunk import ChunkObject
 
 
@@ -128,33 +127,48 @@
         chunk = ChunkObject(path=input_file)
         total_length = Ffmpeg.get_frame_count(PathAlabama(chunk.path))
 
         self.pbar = tqdm(
             total=total_length, desc="Gathering thumbnail data", unit="frame"
         )
 
-        if not os.path.exists("frame_data.json"):
-            get_yuv_frame_stream(
-                chunk,
-                frame_callback=self.process_frame,
-                vf="\"scale=-2:min'(720,ih)':force_original_aspect_ratio=decrease\"",
-            )
+        get_yuv_frame_stream(
+            chunk,
+            frame_callback=self.process_frame,
+            vf="\"scale=-2:min'(720,ih)':force_original_aspect_ratio=decrease\"",
+        )
 
-            # await all the tasks in the pool to be finished
-            self.pool.close()
-            self.pool.join()
-            import json
+        # await all the tasks in the pool to be finished
+        self.pool.close()
+        self.pool.join()
+
+        # if not os.path.exists("frame_data.json"):
+        #     get_yuv_frame_stream(
+        #         chunk,
+        #         frame_callback=self.process_frame,
+        #         vf="\"scale=-2:min'(720,ih)':force_original_aspect_ratio=decrease\"",
+        #     )
+        #
+        #     # await all the tasks in the pool to be finished
+        #     self.pool.close()
+        #     self.pool.join()
+        #     import json
+        #
+        #     with open("frame_data.json", "w") as f:
+        #         json.dump(self.frame_data, f)
+        # else:
+        #     import json
+        #
+        #     with open("frame_data.json", "r") as f:
+        #         self.frame_data = json.load(f)
 
-            with open("frame_data.json", "w") as f:
-                json.dump(self.frame_data, f)
-        else:
-            import json
+        self.pbar.close()
 
-            with open("frame_data.json", "r") as f:
-                self.frame_data = json.load(f)
+        if len(self.frame_data) == 0:
+            raise Exception("No frames were processed")
 
         best_frames = self.get_top_frames(
             self.frame_data,
             num_peaks=9,
             feature_names=[
                 "blurriness",
                 "saliency",
@@ -162,22 +176,30 @@
                 "contrast",
                 # 'saturation',
                 "dof",
                 # 'symmetry'
             ],
             # feature_names=['contrast']
         )
-
-        for i, best_frame in tqdm(enumerate(best_frames), desc="Saving best frames"):
+        has_placebo = check_ffmpeg_libraries("libplacebo")
+        has_jpegli = check_bin("cjpeg")
+        for i, best_frame in tqdm(
+            enumerate(best_frames), desc="Saving best frames", total=len(best_frames)
+        ):
             chunk = ChunkObject(
                 first_frame_index=best_frame,
                 last_frame_index=best_frame + 1,
                 path=input_file,
             )
-            command = f"{get_binary('ffmpeg')} -init_hw_device vulkan -y {chunk.get_ss_ffmpeg_command_pair()} -frames:v 1 -vf 'hwupload,libplacebo=minimum_peak=2:percentile=99.6:tonemapping=spline:colorspace=bt709:color_primaries=bt709:gamut_mode=perceptual:color_trc=bt709:range=tv:gamma=1:format=yuv420p,hwdownload,format=yuv420p' -c:v png -f image2pipe - | {get_binary('cjpeg')} -q 95 -tune-psnr -optimize -progressive > {output_folder}/{i}.jpg"
+            if has_placebo and has_jpegli:
+                command = f"{get_binary('ffmpeg')} -init_hw_device vulkan -y {chunk.get_ss_ffmpeg_command_pair()} -frames:v 1 -vf 'hwupload,libplacebo=minimum_peak=2:percentile=99.6:tonemapping=spline:colorspace=bt709:color_primaries=bt709:gamut_mode=perceptual:color_trc=bt709:range=tv:gamma=1:format=yuv420p,hwdownload,format=yuv420p' -c:v png -f image2pipe - | {get_binary('cjpeg')} -q 95 -tune-psnr -optimize -progressive > {output_folder}/{i}.jpg"
+            elif has_placebo:
+                command = f"{get_binary('ffmpeg')} -init_hw_device vulkan -y {chunk.get_ss_ffmpeg_command_pair()} -frames:v 1 -vf 'hwupload,libplacebo=minimum_peak=2:percentile=99.6:tonemapping=spline:colorspace=bt709:color_primaries=bt709:gamut_mode=perceptual:color_trc=bt709:range=tv:gamma=1:format=yuv420p,hwdownload,format=yuv420p' {output_folder}/{i}.png"
+            else:
+                command = f"{get_binary('ffmpeg')} -y {chunk.get_ss_ffmpeg_command_pair()} -frames:v 1 {output_folder}/{i}.png"
             run_cli(command).verify()
 
     def process_frame(self, yuv_frame):
         self.pool.apply_async(
             process_frame_worker,
             args=(
                 yuv_frame.buffer,
@@ -247,48 +269,55 @@
         # smoothed_score = scipy.ndimage.gaussian_filter1d(combined_score, sigma=100)
         # alt mode where you increate the smoothing factor based on lenght up to a point
         smoothing_factor = min(100, len(combined_score) // 10)
         smoothed_score = scipy.ndimage.gaussian_filter1d(
             combined_score, sigma=smoothing_factor
         )
 
-        import matplotlib.pyplot as plt
-
-        plt.plot(combined_score, label="Combined Score")
-        plt.plot(smoothed_score, label="Smoothed Score")
-        plt.legend()
-        plt.show()
+        # import matplotlib.pyplot as plt
+        #
+        # plt.plot(combined_score, label="Combined Score")
+        # plt.plot(smoothed_score, label="Smoothed Score")
+        # plt.legend()
+        # plt.show()
 
         return smoothed_score
 
     # Step 3: Find peaks in the smoothed data
     def find_peaks(self, smoothed_score):
         peaks, _ = scipy.signal.find_peaks(
             smoothed_score, distance=len(smoothed_score) // 20
         )  # Adjust distance for peak spacing
 
         # print the data with peeks overlayed
-        import matplotlib.pyplot as plt
-
-        plt.plot(smoothed_score, label="Smoothed Score")
-        plt.plot(peaks, smoothed_score[peaks], "x", label="Peaks")
-        plt.legend()
-        plt.show()
+        # import matplotlib.pyplot as plt
+        #
+        # plt.plot(smoothed_score, label="Smoothed Score")
+        # plt.plot(peaks, smoothed_score[peaks], "x", label="Peaks")
+        # plt.legend()
+        # plt.show()
 
         return peaks
 
     # Step 4: Select evenly spaced peaks or fallback to highest scores
     def select_evenly_spaced_peaks(self, peaks, num_peaks, combined_score):
-        if len(peaks) >= num_peaks:
+
+        if not len(peaks) >= num_peaks:
+            print(f"Detection only found {num_peaks} good candidates, using them")
+            return peaks
+        else:
             step = len(peaks) // num_peaks
             evenly_spaced_peaks = peaks[::step][:num_peaks]
-        else:
-            # Fallback: select frames with the highest combined scores
-            top_indices = np.argsort(-combined_score)[:num_peaks]
-            evenly_spaced_peaks = sorted(top_indices)
+        # if len(peaks) >= num_peaks:
+        #     step = len(peaks) // num_peaks
+        #     evenly_spaced_peaks = peaks[::step][:num_peaks]
+        # else:
+        #     # Fallback: select frames with the highest combined scores
+        #     top_indices = np.argsort(-combined_score)[:num_peaks]
+        #     evenly_spaced_peaks = sorted(top_indices)
         return evenly_spaced_peaks
 
     # Main function to get top frame indices
     def get_top_frames(self, frame_data, feature_names, num_peaks=5):
         combined_score = self.normalize_and_combine(frame_data, feature_names)
         smoothed_score = self.smooth_data(combined_score)
         peaks = self.find_peaks(smoothed_score)
@@ -297,12 +326,15 @@
         )
         selected_indices = [frame_data[peak]["index"] for peak in selected_peaks]
 
         return selected_indices
 
 
 if __name__ == "__main__":
-    # AutoThumbnailer().generate_previews('/home/kokoniara/movieEncode/Coraline (2009)/Coraline.2009.1440p.AV1.OPUS.HDR10.SouAV1R.webm', '.')
     AutoThumbnailer().generate_previews(
-        "/home/kokoniara/showsEncode/Silo (2023)/s1/e9/Silo.2023.S01E09.OPUS.AV1.1080p.webm",
+        "/home/kokoniara/Downloads/I Bought 6 PC “Speed Up” Tools to See if They Work [-G-DByczbWA].webm",
         ".",
     )
+    # AutoThumbnailer().generate_previews(
+    #     "/home/kokoniara/showsEncode/Silo (2023)/s1/e9/Silo.2023.S01E09.OPUS.AV1.1080p.webm",
+    #     ".",
+    # )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alabamaencoder-0.4.2/alabamaEncode/core/ffmpeg.py` & `alabamaencoder-0.4.3/alabamaEncode/core/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/core/final_touches.py` & `alabamaencoder-0.4.3/alabamaEncode/core/final_touches.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/core/job.py` & `alabamaencoder-0.4.3/alabamaEncode/core/job.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/core/kv.py` & `alabamaencoder-0.4.3/alabamaEncode/core/kv.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/core/path.py` & `alabamaencoder-0.4.3/alabamaEncode/core/path.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/core/timer.py` & `alabamaencoder-0.4.3/alabamaEncode/core/timer.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/core/ws_update.py` & `alabamaencoder-0.4.3/alabamaEncode/core/ws_update.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/encoder/codec.py` & `alabamaencoder-0.4.3/alabamaEncode/encoder/codec.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/encoder/encoder.py` & `alabamaencoder-0.4.3/alabamaEncode/encoder/encoder.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/encoder/encoder_factory.py` & `alabamaencoder-0.4.3/alabamaEncode/encoder/encoder_factory.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/encoder/impl/Aomenc.py` & `alabamaencoder-0.4.3/alabamaEncode/encoder/impl/Aomenc.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/encoder/impl/Nvenc.py` & `alabamaencoder-0.4.3/alabamaEncode/encoder/impl/Nvenc.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/encoder/impl/SvtAvif.py` & `alabamaencoder-0.4.3/alabamaEncode/encoder/impl/SvtAvif.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/encoder/impl/Svtenc.py` & `alabamaencoder-0.4.3/alabamaEncode/encoder/impl/Svtenc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from typing import List
 
-from alabamaEncode.core.bin_utils import get_binary
+from alabamaEncode.core.bin_utils import get_binary, check_bin
 from alabamaEncode.core.cli_executor import run_cli
 from alabamaEncode.encoder.codec import Codec
 from alabamaEncode.encoder.encoder import Encoder
 from alabamaEncode.encoder.rate_dist import EncoderRateDistribution
 
 
 class EncoderSvt(Encoder):
@@ -23,16 +23,17 @@
             self.keyint == -1 or self.keyint == -2
         ) and self.rate_distribution == EncoderRateDistribution.VBR:
             print("WARNING: keyint must be set for VBR, setting to 240")
             self.keyint = 240
 
         kommand = ""
 
-        if self.pin_to_core != -1:
-            kommand += f"taskset -a -c {self.pin_to_core} "
+        if check_bin("taskset"):
+            if self.pin_to_core != -1:
+                kommand += f"taskset -a -c {self.pin_to_core} "
 
         kommand += (
             f"{self.get_ffmpeg_pipe_command()} | "
             f"{get_binary('SvtAv1EncApp')}"
             f" -i stdin"
             f" --input-depth {self.bit_override}"
             f" --progress 2 "
@@ -131,17 +132,15 @@
                 kommand += " --enable-qm 1"
             else:
                 kommand += " --enable-qm 0"
 
             kommand += f" --enable-tf {self.svt_tf}"
 
             kommand += f" --enable-variance-boost {self.svt_enable_variance_boost} "
-            kommand += (
-                f" --variance-boost-strength {self.svt_variance_boost_strength}"
-            )
+            kommand += f" --variance-boost-strength {self.svt_variance_boost_strength}"
             kommand += f" --variance-octile {self.svt_variance_octile}"
             if self.is_psy():
                 kommand += f" --sharpness {self.svt_sharpness}"
 
         else:
             kommand += self.override_flags
```

### Comparing `alabamaencoder-0.4.2/alabamaEncode/encoder/impl/VaapiH264.py` & `alabamaencoder-0.4.3/alabamaEncode/encoder/impl/VaapiH264.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/encoder/impl/VaapiH265.py` & `alabamaencoder-0.4.3/alabamaEncode/encoder/impl/VaapiH265.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/encoder/impl/X264.py` & `alabamaencoder-0.4.3/alabamaEncode/encoder/impl/X264.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/encoder/impl/X265.py` & `alabamaencoder-0.4.3/alabamaEncode/encoder/impl/X265.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/encoder/impl/rav1e.py` & `alabamaencoder-0.4.3/alabamaEncode/encoder/impl/rav1e.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/encoder/impl/vp9.py` & `alabamaencoder-0.4.3/alabamaEncode/encoder/impl/vp9.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/encoder/stats.py` & `alabamaencoder-0.4.3/alabamaEncode/encoder/stats.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/experiments/Aq.py` & `alabamaencoder-0.4.3/alabamaEncode/experiments/Aq.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/experiments/Overlays.py` & `alabamaencoder-0.4.3/alabamaEncode/experiments/Overlays.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/experiments/Svtav1Speed.py` & `alabamaencoder-0.4.3/alabamaEncode/experiments/Svtav1Speed.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/experiments/Svtav1Tunes.py` & `alabamaencoder-0.4.3/alabamaEncode/experiments/Svtav1Tunes.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/experiments/TemporalFiltering.py` & `alabamaencoder-0.4.3/alabamaEncode/experiments/TemporalFiltering.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/experiments/ai_feature_extract.py` & `alabamaencoder-0.4.3/alabamaEncode/experiments/ai_feature_extract.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/experiments/convexhull.py` & `alabamaencoder-0.4.3/alabamaEncode/experiments/convexhull.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/experiments/crf_vmaf_relation.py` & `alabamaencoder-0.4.3/alabamaEncode/experiments/crf_vmaf_relation.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/experiments/denoise.py` & `alabamaencoder-0.4.3/alabamaEncode/experiments/denoise.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/experiments/sequence_convex.py` & `alabamaencoder-0.4.3/alabamaEncode/experiments/sequence_convex.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/experiments/streaming_output.py` & `alabamaencoder-0.4.3/alabamaEncode/experiments/streaming_output.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/experiments/superres.py` & `alabamaencoder-0.4.3/alabamaEncode/experiments/superres.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/experiments/target_vmaf.py` & `alabamaencoder-0.4.3/alabamaEncode/experiments/target_vmaf.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/experiments/util/ExperimentUtil.py` & `alabamaencoder-0.4.3/alabamaEncode/experiments/util/ExperimentUtil.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/ffmpeg_source/ffmpeg_src.py` & `alabamaencoder-0.4.3/alabamaEncode/ffmpeg_source/ffmpeg_src.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/ffmpeg_source/yuv.py` & `alabamaencoder-0.4.3/alabamaEncode/ffmpeg_source/yuv.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/metrics/calculate.py` & `alabamaencoder-0.4.3/alabamaEncode/metrics/calculate.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/metrics/comparison_display.py` & `alabamaencoder-0.4.3/alabamaEncode/metrics/comparison_display.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/metrics/image.py` & `alabamaencoder-0.4.3/alabamaEncode/metrics/image.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/metrics/impl/psnr.py` & `alabamaencoder-0.4.3/alabamaEncode/metrics/impl/psnr.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/metrics/impl/ssim.py` & `alabamaencoder-0.4.3/alabamaEncode/metrics/impl/ssim.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/metrics/impl/ssimu2.py` & `alabamaencoder-0.4.3/alabamaEncode/metrics/impl/ssimu2.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/metrics/impl/vmaf.py` & `alabamaencoder-0.4.3/alabamaEncode/metrics/impl/vmaf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 from statistics import mean
 
 from alabamaEncode.core.bin_utils import get_binary
 from alabamaEncode.core.bin_utils import register_bin
-from alabamaEncode.core.cli_executor import run_cli, run_cli_parallel
+from alabamaEncode.core.cli_executor import run_cli_parallel
 from alabamaEncode.core.path import PathAlabama
 from alabamaEncode.metrics.exception import VmafException
 from alabamaEncode.metrics.metric import Metric
 from alabamaEncode.metrics.options import MetricOptions
 from alabamaEncode.metrics.result import MetricResult
 from alabamaEncode.scene.chunk import ChunkObject
 
@@ -250,20 +250,21 @@
     ]
 
     models_dir = os.path.expanduser("~/vmaf_models")
     if not os.path.exists(models_dir):
         os.makedirs(models_dir)
 
     try:
+        import requests
+
         for link in links:
             if not os.path.exists(os.path.join(models_dir, link[1])):
                 print("Downloading VMAF model")
-                run_cli(
-                    f"wget -O {models_dir}/{link[1]} {link[0]}"
-                )  # TsODO: WINDOWS SUPPORT
+                r = requests.get(link[0], allow_redirects=True)
+                open(os.path.join(models_dir, link[1]), "wb").write(r.content)
 
         for link in links:
             if not os.path.exists(os.path.join(models_dir, link[1])):
                 raise FileNotFoundError(f"Something went wrong accessing {link[1]}")
     except Exception as e:
         raise RuntimeError(f"Failed downloading VMAF models, {e}")
```

### Comparing `alabamaencoder-0.4.2/alabamaEncode/parallelEncoding/CeleryApp.py` & `alabamaencoder-0.4.3/alabamaEncode/parallelEncoding/CeleryApp.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/parallelEncoding/CeleryAutoscaler.py` & `alabamaencoder-0.4.3/alabamaEncode/parallelEncoding/CeleryAutoscaler.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/parallelEncoding/execute_commands.py` & `alabamaencoder-0.4.3/alabamaEncode/parallelEncoding/execute_commands.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/parallelEncoding/worker.py` & `alabamaencoder-0.4.3/alabamaEncode/parallelEncoding/worker.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/scene/annel.py` & `alabamaencoder-0.4.3/alabamaEncode/scene/annel.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/scene/chunk.py` & `alabamaencoder-0.4.3/alabamaEncode/scene/chunk.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/scene/concat.py` & `alabamaencoder-0.4.3/alabamaEncode/scene/concat.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         end_offset=-1,
         title="",
         encoder_name="TestHoeEncode",
         mux_audio=True,
         subs_file=None,
         audio_only=False,
         temp_dir="",
-        copy_included_subs=True
+        copy_included_subs=True,
     ):
         self.files = files
         self.output = output
         self.file_with_audio = file_with_audio
         self.audio_param_override = audio_param_override
         self.start_offset = start_offset
         self.end_offset = end_offset
@@ -75,30 +75,35 @@
         print(f"Concat took {end - start} seconds")
 
     def extract_subs(self, start_offset="", end_offset=""):
         og_file = PathAlabama(self.file_with_audio)
         tracks = Ffmpeg.get_tracks(og_file)
         extracted_subs = []
         sub_counter = 0
-        for track in tqdm([track for track in tracks if track['codec_type'] == "subtitle"], desc="Extracting Subs"):
+        for track in tqdm(
+            [track for track in tracks if track["codec_type"] == "subtitle"],
+            desc="Extracting Subs",
+        ):
             tag_lang = ""
-            if 'language' in track['tags']:
-                tag_lang = track['tags']['language']
+            if "language" in track["tags"]:
+                tag_lang = track["tags"]["language"]
             tag_title = ""
-            if 'title' in track['tags']:
-                tag_title = track['tags']['title']
+            if "title" in track["tags"]:
+                tag_title = track["tags"]["title"]
 
-            out_path = f'{self.temp_dir}{tag_lang}.vtt'
+            out_path = f"{self.temp_dir}{tag_lang}.vtt"
             counter = 1
             while os.path.exists(out_path):
-                out_path = f'{self.temp_dir}{tag_lang}_{counter}.vtt'
+                out_path = f"{self.temp_dir}{tag_lang}_{counter}.vtt"
                 counter += 1
             try:
-                a = (f'{get_binary("ffmpeg")} -v error -y -stats {start_offset} -i {og_file.get_safe()} {end_offset} '
-                     f'-map 0:s:{sub_counter} "{out_path}"')
+                a = (
+                    f'{get_binary("ffmpeg")} -v error -y -stats {start_offset} -i {og_file.get_safe()} {end_offset} '
+                    f'-map 0:s:{sub_counter} "{out_path}"'
+                )
                 run_cli(a)
             except Exception as e:
                 # print(e)
                 pass
 
             if os.path.exists(out_path):
                 extracted_subs.append((out_path, tag_lang, tag_title, sub_counter))
@@ -127,15 +132,14 @@
         if Ffmpeg.check_for_invalid(PathAlabama(self.vid_output)):
             raise Exception("Concating chunks failed")
 
         os.remove(concat_file_path)
 
         self.final_files += [f'-i "{self.vid_output}"']
 
-
     def encode_audio_tracks(self):
         print("Encoding a audio track")
         self.audio_output = f"{self.temp_dir}audio.mkv"
 
         vec = [
             get_binary("ffmpeg"),
             "-y",
@@ -243,14 +247,15 @@
             os.system(
                 f"{get_binary('ffmpeg')} -y -stats -v error -i {self.vid_output} -c copy {self.output}"
             )
             os.remove(self.vid_output)
             if Ffmpeg.check_for_invalid(PathAlabama(self.output)):
                 os.remove(self.output)
                 raise Exception("VIDEO CONCAT FAILED")
+            return
 
         self.encode_audio_tracks()
         print("Muxing audio into the output")
 
         title_bit = f' -metadata description="encoded by {self.encoder_name}" '
         if self.title:
             title_bit += f' -metadata title="{self.title}"'
@@ -258,20 +263,22 @@
         if self.subs_file is None or self.subs_file[0] == "":
             vec = [
                 get_binary("ffmpeg"),
                 "-y",
                 "-stats",
                 "-v error",
                 f'-i "{self.vid_output}"',
-                f'-i "{self.audio_output}"'
+                f'-i "{self.audio_output}"',
             ]
 
             sub_tracks = []
             if self.copy_included_subs:
-                sub_tracks = self.extract_subs(start_offset=start_offset_command, end_offset=end_offset_command)
+                sub_tracks = self.extract_subs(
+                    start_offset=start_offset_command, end_offset=end_offset_command
+                )
 
                 for out_path, tag_lang, tag_title, track_index in sub_tracks:
                     vec += [
                         f'-i "{out_path}"',
                     ]
 
             if self.encoder_name:
@@ -280,15 +287,15 @@
             if self.title:
                 vec += [f' -metadata title="{self.title}"']
 
             if self.copy_included_subs and len(sub_tracks) > 0:
                 stream_index = 2
                 for out_path, tag_lang, tag_title, track_index in sub_tracks:
                     vec += [
-                        f'-map {stream_index}:s',
+                        f"-map {stream_index}:s",
                         f'-metadata:s:s:{track_index} language="{tag_lang}"',
                         f'-metadata:s:s:{track_index} title="{tag_title}"',
                     ]
                     stream_index += 1
 
             vec += ["-map 0:v", "-map 1:a"]
 
@@ -307,16 +314,16 @@
             ]
 
             final_command = " ".join(vec)
             print(final_command)
             # print(f"running: {final_command}")
             out = run_cli(final_command).verify().get_output()
             if (
-                    "Subtitle encoding currently only possible from text to text or bitmap to bitmap"
-                    in str(out)
+                "Subtitle encoding currently only possible from text to text or bitmap to bitmap"
+                in str(out)
             ):
                 print("Subtitle encoding failed, trying again")
                 for a in vec:
                     if "mov_text" in a or "map 2:s" in a:
                         vec.remove(a)
                 final_command = " ".join(vec)
                 # print(f"running: {final_command}")
@@ -382,8 +389,8 @@
     create_fake_ivf_and_test(temp_dir)
 
     # remove temp dir
     os.system(f"rm -rf {temp_dir}")
 
 
 if __name__ == "__main__":
-    test()
+    test()
```

### Comparing `alabamaencoder-0.4.2/alabamaEncode/scene/sequence.py` & `alabamaencoder-0.4.3/alabamaEncode/scene/sequence.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode/scene/split.py` & `alabamaencoder-0.4.3/alabamaEncode/scene/split.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode_frontends/cli/__main__.py` & `alabamaencoder-0.4.3/alabamaEncode_frontends/cli/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import asyncio
 import atexit
 import os
 import sys
 import time
 
 from alabamaEncode.core.alabama import AlabamaContext
+from alabamaEncode.core.extras.auto_thumbnailer import AutoThumbnailer
 from alabamaEncode.core.job import AlabamaEncodingJob
 from alabamaEncode.parallelEncoding.CeleryApp import app
 from alabamaEncode.parallelEncoding.worker import worker
 from alabamaEncode_frontends.cli.cli_setup.autopaths import auto_output_paths
 from alabamaEncode_frontends.cli.cli_setup.cli_args import read_args
 from alabamaEncode_frontends.cli.cli_setup.paths import parse_paths
 from alabamaEncode_frontends.cli.cli_setup.ratecontrol import parse_rd
@@ -97,28 +98,28 @@
         ctx = setup_context_for_standalone_usage()
 
     global runtime_file
     global lock_file_path
     runtime_file = os.path.join(ctx.temp_folder, "runtime.txt")
     lock_file_path = os.path.join(ctx.output_folder, "alabama.lock")
 
-    if os.path.exists(lock_file_path):
+    if os.path.exists(lock_file_path) and not ctx.standalone_autothumbnailer:
         print(
             "Lock file exists, are you sure another instance is not encoding in this folder? "
             "if not delete the lock file and try again"
         )
         quit()
     else:
         open(lock_file_path, "w").close()
 
     output_lock = os.path.join(ctx.temp_folder, "output.lock")
     if not os.path.exists(output_lock):
         with open(output_lock, "w") as f:
             f.write(ctx.raw_input_file)
-    else:
+    elif not ctx.standalone_autothumbnailer:
         output_file_from_lock = open(output_lock).read()
         if output_file_from_lock != ctx.raw_input_file:
             print(
                 f"Output file from lock file {output_file_from_lock} does not match output file "
                 f"from ctx {ctx.raw_input_file}"
             )
             quit()
@@ -132,14 +133,21 @@
         import requests
         import json
 
         headers = {"Authorization": f"Bearer {auth_token}"}
         data = json.dumps(ctx.to_json())
         requests.post(f"{ctx.offload_server}/jobs", data=data, headers=headers)
 
+    if ctx.standalone_autothumbnailer:
+        AutoThumbnailer().generate_previews(
+            input_file=ctx.input_file,
+            output_folder=ctx.output_folder,
+        )
+        quit()
+
     job = AlabamaEncodingJob(ctx)
 
     asyncio.run(job.run_pipeline())  # this runs the whole encoding process
 
     quit()
```

### Comparing `alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/autopaths.py` & `alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/autopaths.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/cli_args.py` & `alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/cli_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -553,35 +553,41 @@
         "--denoise_vmaf_ref",
         action="store_true",
         help="Denoise the vmaf reference",
         dest="denoise_vmaf_ref",
     )
 
     parser.add_argument(
-        "--dont_calc_final_vmaf",
-        default=ctx.dont_calc_final_vmaf,
+        "--calc_final_vmaf",
+        default=ctx.calc_final_vmaf,
         action="store_true",
         help="Dont calculate final vmaf",
-        dest="dont_calc_final_vmaf",
+        dest="calc_final_vmaf",
     )
 
     parser.add_argument(
         "--multi_res_pipeline",
         action="store_true",
         help="Create a optimised multi bitrate tier stream",
         dest="multi_res_pipeline",
     )
 
     parser.add_argument(
-        '--throughput_scaling',
-        action='store_true',
-        help='Scale the multi-process workers based on throughput',
-        dest='throughput_scaling'
+        "--throughput_scaling",
+        action="store_true",
+        help="Scale the multi-process workers based on throughput",
+        dest="throughput_scaling",
     )
 
+    parser.add_argument(
+        "--standalone_autothumbnailer",
+        action="store_true",
+        help="dont encode, just generate thumbnails for the input file in the output's file directory",
+        dest="standalone_autothumbnailer",
+    )
 
     args = parser.parse_args()
 
     ctx.output_file = args.output
     ctx.output_folder = ctx.output_file
     ctx.raw_input_file = args.input
     ctx.prototype_encoder = get_encoder_from_string(args.encoder)
@@ -647,12 +653,13 @@
     ctx.dynamic_vmaf_target = args.dynamic_vmaf_target
     ctx.dynamic_vmaf_target_vbr = args.dynamic_vmaf_target_vbr
     ctx.statically_sized_scenes = args.statically_sized_scenes
     ctx.scene_merge = args.scene_merge
     ctx.args_tune = args.tune
     ctx.denoise_vmaf_ref = args.denoise_vmaf_ref
     ctx.multi_res_pipeline = args.multi_res_pipeline
-    ctx.dont_calc_final_vmaf = args.dont_calc_final_vmaf
+    ctx.calc_final_vmaf = args.calc_final_vmaf
     ctx.metric_to_target = args.metric_to_target
     ctx.throughput_scaling = args.throughput_scaling
+    ctx.standalone_autothumbnailer = args.standalone_autothumbnailer
 
     return ctx
```

### Comparing `alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/paths.py` & `alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/paths.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/ratecontrol.py` & `alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/ratecontrol.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/res_preset.py` & `alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/res_preset.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/validate_files.py` & `alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/validate_files.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode_frontends/cli/cli_setup/video_filters.py` & `alabamaencoder-0.4.3/alabamaEncode_frontends/cli/cli_setup/video_filters.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncode_frontends/demon/demon.py` & `alabamaencoder-0.4.3/alabamaEncode_frontends/demon/demon.py`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/alabamaEncoder.egg-info/SOURCES.txt` & `alabamaencoder-0.4.3/alabamaEncoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alabamaencoder-0.4.2/setup.py` & `alabamaencoder-0.4.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="alabamaEncoder",
-    version="0.4.2",
+    version="0.4.3",
     packages=find_packages(),
     install_requires=[
         "scenedetect",
         "tqdm",
         "celery",
         "redis",
         "psutil",
@@ -14,13 +14,14 @@
         "requests",
         "torf",
         "websockets",
         "argparse_range",
         "scipy",
         "numpy",
         "scikit-image",
+        "argparse-range",
     ],
     entry_points="""
       [console_scripts]
       alabamaEncoder=alabamaEncode_frontends.cli.__main__:main
       """,
 )
```

