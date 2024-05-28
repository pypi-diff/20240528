# Comparing `tmp/hqq-0.1.7.post2.tar.gz` & `tmp/hqq-0.1.7.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hqq-0.1.7.post2.tar", last modified: Mon May  6 16:38:05 2024, max compression
+gzip compressed data, was "hqq-0.1.7.post3.tar", last modified: Tue May 28 07:44:35 2024, max compression
```

## Comparing `hqq-0.1.7.post2.tar` & `hqq-0.1.7.post3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.731692 hqq-0.1.7.post2/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    11360 2023-12-02 17:25:57.000000 hqq-0.1.7.post2/LICENSE
--rw-r--r--   0 hicham    (1009) hicham    (1009)      438 2024-05-06 16:38:05.731692 hqq-0.1.7.post2/PKG-INFO
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.715691 hqq-0.1.7.post2/hqq/
--rwxrwxr-x   0 hicham    (1009) hicham    (1009)       93 2024-05-06 15:26:52.000000 hqq-0.1.7.post2/hqq/__init__.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.719691 hqq-0.1.7.post2/hqq/backends/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2024-04-16 10:04:12.000000 hqq-0.1.7.post2/hqq/backends/__init__.py
--rwxrwxr-x   0 hicham    (1009) hicham    (1009)     3351 2024-05-06 16:33:14.000000 hqq-0.1.7.post2/hqq/backends/marlin.py
--rwxrwxr-x   0 hicham    (1009) hicham    (1009)    11856 2024-05-06 16:33:14.000000 hqq-0.1.7.post2/hqq/backends/torchao.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.723691 hqq-0.1.7.post2/hqq/core/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-01 10:59:22.000000 hqq-0.1.7.post2/hqq/core/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     5195 2024-05-03 14:37:22.000000 hqq-0.1.7.post2/hqq/core/bitpack.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    14369 2024-05-03 14:37:54.000000 hqq-0.1.7.post2/hqq/core/optimize.py
--rwxrwxr-x   0 hicham    (1009) hicham    (1009)    17325 2024-05-06 15:26:52.000000 hqq-0.1.7.post2/hqq/core/peft.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    28621 2024-05-03 15:01:23.000000 hqq-0.1.7.post2/hqq/core/quantize.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)      670 2024-05-03 14:37:54.000000 hqq-0.1.7.post2/hqq/core/utils.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.723691 hqq-0.1.7.post2/hqq/engine/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7.post2/hqq/engine/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3159 2024-05-06 07:14:36.000000 hqq-0.1.7.post2/hqq/engine/base.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2568 2024-03-15 09:12:21.000000 hqq-0.1.7.post2/hqq/engine/hf.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2458 2024-03-15 09:09:35.000000 hqq-0.1.7.post2/hqq/engine/timm.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     5287 2024-03-15 12:03:22.000000 hqq-0.1.7.post2/hqq/engine/vllm.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.727692 hqq-0.1.7.post2/hqq/kernels/
--rwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 15:26:46.000000 hqq-0.1.7.post2/hqq/kernels/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2670 2024-03-25 10:15:39.000000 hqq-0.1.7.post2/hqq/kernels/hqq_aten_cuda.cpp
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    17933 2024-04-08 11:30:33.000000 hqq-0.1.7.post2/hqq/kernels/hqq_aten_cuda_kernel.cu
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3412 2024-02-21 11:27:07.000000 hqq-0.1.7.post2/hqq/kernels/hqq_aten_torch.cpp
--rwxrwxr-x   0 hicham    (1009) hicham    (1009)      473 2024-05-06 15:26:46.000000 hqq-0.1.7.post2/hqq/kernels/setup_cuda.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)      292 2024-03-14 16:26:18.000000 hqq-0.1.7.post2/hqq/kernels/setup_torch.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.727692 hqq-0.1.7.post2/hqq/models/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-01 10:59:32.000000 hqq-0.1.7.post2/hqq/models/__init__.py
--rwxrwxr-x   0 hicham    (1009) hicham    (1009)    18084 2024-05-06 15:26:52.000000 hqq-0.1.7.post2/hqq/models/base.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.727692 hqq-0.1.7.post2/hqq/models/hf/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7.post2/hqq/models/hf/__init__.py
--rwxrwxr-x   0 hicham    (1009) hicham    (1009)     1255 2024-05-06 16:33:14.000000 hqq-0.1.7.post2/hqq/models/hf/base.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2703 2024-03-14 15:51:30.000000 hqq-0.1.7.post2/hqq/models/hf/llama.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2703 2024-03-14 15:51:30.000000 hqq-0.1.7.post2/hqq/models/hf/mistral.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3464 2024-03-14 15:51:30.000000 hqq-0.1.7.post2/hqq/models/hf/mixtral.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2487 2024-03-14 15:51:30.000000 hqq-0.1.7.post2/hqq/models/hf/phi.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2361 2024-03-14 15:51:30.000000 hqq-0.1.7.post2/hqq/models/hf/phi_opt.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.727692 hqq-0.1.7.post2/hqq/models/timm/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7.post2/hqq/models/timm/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)      750 2024-03-14 15:52:37.000000 hqq-0.1.7.post2/hqq/models/timm/base.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2815 2024-03-14 15:53:15.000000 hqq-0.1.7.post2/hqq/models/timm/vit_clip.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.731692 hqq-0.1.7.post2/hqq/models/vllm/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7.post2/hqq/models/vllm/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     6114 2024-03-15 12:07:03.000000 hqq-0.1.7.post2/hqq/models/vllm/base.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    16480 2024-03-14 15:55:27.000000 hqq-0.1.7.post2/hqq/models/vllm/llama.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.731692 hqq-0.1.7.post2/hqq/utils/
--rw-rw-r--   0 hicham    (1009) hicham    (1009)        0 2024-05-06 15:26:46.000000 hqq-0.1.7.post2/hqq/utils/__init__.py
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)    10844 2024-04-23 16:50:10.000000 hqq-0.1.7.post2/hqq/utils/generation_hf.py
--rwxrwxr-x   0 hicham    (1009) hicham    (1009)     6319 2024-05-06 16:33:14.000000 hqq-0.1.7.post2/hqq/utils/patching.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.719691 hqq-0.1.7.post2/hqq.egg-info/
--rw-r--r--   0 hicham    (1009) hicham    (1009)      438 2024-05-06 16:37:56.000000 hqq-0.1.7.post2/hqq.egg-info/PKG-INFO
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     1109 2024-05-06 16:37:56.000000 hqq-0.1.7.post2/hqq.egg-info/SOURCES.txt
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        1 2024-05-06 16:37:56.000000 hqq-0.1.7.post2/hqq.egg-info/dependency_links.txt
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)       92 2024-05-06 16:37:56.000000 hqq-0.1.7.post2/hqq.egg-info/requires.txt
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)        4 2024-05-06 16:37:56.000000 hqq-0.1.7.post2/hqq.egg-info/top_level.txt
--rw-rw-r--   0 hicham    (1009) hicham    (1009)       38 2024-05-06 16:38:05.731692 hqq-0.1.7.post2/setup.cfg
--rwxrwxr-x   0 hicham    (1009) hicham    (1009)     1706 2024-05-06 15:26:52.000000 hqq-0.1.7.post2/setup.py
-drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-06 16:38:05.731692 hqq-0.1.7.post2/tests/
--rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3689 2024-03-25 10:44:50.000000 hqq-0.1.7.post2/tests/test_bitpack.py
--rw-rw-r--   0 hicham    (1009) hicham    (1009)    11302 2024-05-06 15:26:46.000000 hqq-0.1.7.post2/tests/test_quantize.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-28 07:44:35.572090 hqq-0.1.7.post3/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    11360 2023-12-02 17:25:57.000000 hqq-0.1.7.post3/LICENSE
+-rw-r--r--   0 hicham    (1009) hicham    (1009)      438 2024-05-28 07:44:35.572090 hqq-0.1.7.post3/PKG-INFO
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-28 07:44:35.568090 hqq-0.1.7.post3/hqq/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)       93 2024-05-28 07:43:23.000000 hqq-0.1.7.post3/hqq/__init__.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-28 07:44:35.568090 hqq-0.1.7.post3/hqq/backends/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2024-04-16 10:04:12.000000 hqq-0.1.7.post3/hqq/backends/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3351 2024-05-06 16:33:14.000000 hqq-0.1.7.post3/hqq/backends/marlin.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    11866 2024-05-09 08:24:37.000000 hqq-0.1.7.post3/hqq/backends/torchao.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-28 07:44:35.568090 hqq-0.1.7.post3/hqq/core/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-01 10:59:22.000000 hqq-0.1.7.post3/hqq/core/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     5195 2024-05-03 14:37:22.000000 hqq-0.1.7.post3/hqq/core/bitpack.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    14397 2024-05-13 09:35:53.000000 hqq-0.1.7.post3/hqq/core/optimize.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    17365 2024-05-09 08:26:30.000000 hqq-0.1.7.post3/hqq/core/peft.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    30679 2024-05-20 12:31:12.000000 hqq-0.1.7.post3/hqq/core/quantize.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)      718 2024-05-13 10:10:45.000000 hqq-0.1.7.post3/hqq/core/utils.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-28 07:44:35.568090 hqq-0.1.7.post3/hqq/engine/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7.post3/hqq/engine/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3189 2024-05-09 08:27:19.000000 hqq-0.1.7.post3/hqq/engine/base.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2568 2024-03-15 09:12:21.000000 hqq-0.1.7.post3/hqq/engine/hf.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2458 2024-03-15 09:09:35.000000 hqq-0.1.7.post3/hqq/engine/timm.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     5287 2024-03-15 12:03:22.000000 hqq-0.1.7.post3/hqq/engine/vllm.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-28 07:44:35.572090 hqq-0.1.7.post3/hqq/kernels/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2024-05-06 15:26:46.000000 hqq-0.1.7.post3/hqq/kernels/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2670 2024-03-25 10:15:39.000000 hqq-0.1.7.post3/hqq/kernels/hqq_aten_cuda.cpp
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    17933 2024-04-08 11:30:33.000000 hqq-0.1.7.post3/hqq/kernels/hqq_aten_cuda_kernel.cu
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3412 2024-02-21 11:27:07.000000 hqq-0.1.7.post3/hqq/kernels/hqq_aten_torch.cpp
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)      473 2024-05-06 15:26:46.000000 hqq-0.1.7.post3/hqq/kernels/setup_cuda.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)      292 2024-03-14 16:26:18.000000 hqq-0.1.7.post3/hqq/kernels/setup_torch.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-28 07:44:35.572090 hqq-0.1.7.post3/hqq/models/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-01 10:59:32.000000 hqq-0.1.7.post3/hqq/models/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    18020 2024-05-13 10:10:27.000000 hqq-0.1.7.post3/hqq/models/base.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-28 07:44:35.572090 hqq-0.1.7.post3/hqq/models/hf/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7.post3/hqq/models/hf/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     1255 2024-05-06 16:33:14.000000 hqq-0.1.7.post3/hqq/models/hf/base.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2703 2024-03-14 15:51:30.000000 hqq-0.1.7.post3/hqq/models/hf/llama.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2703 2024-03-14 15:51:30.000000 hqq-0.1.7.post3/hqq/models/hf/mistral.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3464 2024-03-14 15:51:30.000000 hqq-0.1.7.post3/hqq/models/hf/mixtral.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2487 2024-03-14 15:51:30.000000 hqq-0.1.7.post3/hqq/models/hf/phi.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2361 2024-03-14 15:51:30.000000 hqq-0.1.7.post3/hqq/models/hf/phi_opt.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-28 07:44:35.572090 hqq-0.1.7.post3/hqq/models/timm/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7.post3/hqq/models/timm/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)      758 2024-05-07 18:58:01.000000 hqq-0.1.7.post3/hqq/models/timm/base.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     2815 2024-03-14 15:53:15.000000 hqq-0.1.7.post3/hqq/models/timm/vit_clip.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-28 07:44:35.572090 hqq-0.1.7.post3/hqq/models/vllm/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2023-12-02 17:26:13.000000 hqq-0.1.7.post3/hqq/models/vllm/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     6114 2024-03-15 12:07:03.000000 hqq-0.1.7.post3/hqq/models/vllm/base.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    16480 2024-03-14 15:55:27.000000 hqq-0.1.7.post3/hqq/models/vllm/llama.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-28 07:44:35.572090 hqq-0.1.7.post3/hqq/utils/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        0 2024-05-06 15:26:46.000000 hqq-0.1.7.post3/hqq/utils/__init__.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)    10879 2024-05-09 08:22:38.000000 hqq-0.1.7.post3/hqq/utils/generation_hf.py
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     6319 2024-05-06 16:33:14.000000 hqq-0.1.7.post3/hqq/utils/patching.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-28 07:44:35.568090 hqq-0.1.7.post3/hqq.egg-info/
+-rw-r--r--   0 hicham    (1009) hicham    (1009)      438 2024-05-28 07:44:31.000000 hqq-0.1.7.post3/hqq.egg-info/PKG-INFO
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     1109 2024-05-28 07:44:31.000000 hqq-0.1.7.post3/hqq.egg-info/SOURCES.txt
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        1 2024-05-28 07:44:31.000000 hqq-0.1.7.post3/hqq.egg-info/dependency_links.txt
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)       92 2024-05-28 07:44:31.000000 hqq-0.1.7.post3/hqq.egg-info/requires.txt
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)        4 2024-05-28 07:44:31.000000 hqq-0.1.7.post3/hqq.egg-info/top_level.txt
+-rw-rw-r--   0 hicham    (1009) hicham    (1009)       38 2024-05-28 07:44:35.572090 hqq-0.1.7.post3/setup.cfg
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     1706 2024-05-28 07:43:02.000000 hqq-0.1.7.post3/setup.py
+drwxrwxr-x   0 hicham    (1009) hicham    (1009)        0 2024-05-28 07:44:35.572090 hqq-0.1.7.post3/tests/
+-rwxrwxrwx   0 hicham    (1009) hicham    (1009)     3689 2024-03-25 10:44:50.000000 hqq-0.1.7.post3/tests/test_bitpack.py
+-rw-rw-r--   0 hicham    (1009) hicham    (1009)    12177 2024-05-07 06:51:06.000000 hqq-0.1.7.post3/tests/test_quantize.py
```

### Comparing `hqq-0.1.7.post2/LICENSE` & `hqq-0.1.7.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post2/hqq/backends/marlin.py` & `hqq-0.1.7.post3/hqq/backends/marlin.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post2/hqq/backends/torchao.py` & `hqq-0.1.7.post3/hqq/backends/torchao.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,16 +127,16 @@
 
     ###################### Quantize/packing ######################
 
     def quantize(
         self,
         W: Tensor,
         weight_quant_params: dict,
-        scale_quant_params=dict | None,
-        zero_quant_params=dict | None,
+        scale_quant_params=Union[dict,None],
+        zero_quant_params=Union[dict,None],
         offload_meta=False,
     ):
         W_q, meta = Quantizer.quantize(
             W,
             **weight_quant_params,
             device=self.device,
             compute_dtype=self.compute_dtype,
```

### Comparing `hqq-0.1.7.post2/hqq/core/bitpack.py` & `hqq-0.1.7.post3/hqq/core/bitpack.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post2/hqq/core/optimize.py` & `hqq-0.1.7.post3/hqq/core/optimize.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,17 @@
     dtype = scale.dtype
     ###############################
     W_q = torch.round(W_f * scale + zero).clamp(min_max[0], min_max[1])
     n_clusters = max(W_q.shape[0], W_q.shape[1])
     rng = torch.abs(scale).mean() * rng_dump if (rng_dump < 1.0) else rng_dump
 
     scale_shifted = (
-        torch.linspace(-rng, rng, N)[:, None].to(dtype).to(device).repeat(1, n_clusters)
+        torch.linspace(-rng, rng, N)[:, None]
+        .to(dtype=dtype, device=device)
+        .repeat(1, n_clusters)
         + scale
     )
 
     # Safe inverse
     scale_shifted[
         torch.logical_and(scale_shifted >= 0, torch.abs(scale_shifted) <= z_val)
     ] = z_val
```

### Comparing `hqq-0.1.7.post2/hqq/core/peft.py` & `hqq-0.1.7.post3/hqq/core/peft.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #####################################################
 import torch
 from torch import float16, bfloat16, float32
 from torch import Tensor, nn
 import numpy as np
 from .quantize import HQQLinear, Quantizer
 from .utils import cleanup
+from typing import Union
 
 
 # Return trainable weight matrix
 def _get_dense_param(
     in_features: int,
     out_features: int,
     device="cuda",
@@ -363,38 +364,38 @@
 ##################################################################################################################
 def autoname_modules(model):
     for name, module in model.named_modules():
         module.name = name
 
 
 # Patching functions
-def patch_linear_add_peft(layer: nn.Module, patch_params: dict | None) -> nn.Module:
+def patch_linear_add_peft(layer: nn.Module, patch_params: Union[dict,None]) -> nn.Module:
     _peft_config = patch_params
     if _peft_config:
         lora_type = (
             _peft_config["lora_type"] if ("lora_type" in _peft_config) else "default"
         )
         new_layer = _HQQ_LORA_MAPPING[lora_type](layer, _peft_config)
     else:
         new_layer = layer
     return new_layer
 
 
-def patch_linear_merge_peft(layer: nn.Module, patch_params: dict | None) -> nn.Module:
+def patch_linear_merge_peft(layer: nn.Module, patch_params: Union[dict,None]) -> nn.Module:
     _quant_config = patch_params
     if _quant_config:
         new_layer = layer.merge_and_quantize(_quant_config)
         del layer
         cleanup()
     else:
         new_layer = layer
     return new_layer
 
 
-def patch_linear_cast_peft(layer: nn.Module, patch_params: dict | None) -> nn.Module:
+def patch_linear_cast_peft(layer: nn.Module, patch_params: Union[dict,None]) -> nn.Module:
     if is_hqq_lora_layer(layer):
         layer.cast(patch_params)
     return layer
 
 
 # Putting it all together
 class PeftUtils:
```

### Comparing `hqq-0.1.7.post2/hqq/core/quantize.py` & `hqq-0.1.7.post3/hqq/core/quantize.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,19 +9,21 @@
 from .utils import is_divisible
 from .optimize import optimize_weights_proximal
 from .bitpack import BitPack
 
 
 # Main HQQ Quantizer
 class Quantizer:
-    SUPPORTED_BITS = [8, 4, 3, 2, 1]
+    SUPPORTED_BITS = [8, 6, 5, 4, 3, 2, 1]
     optimize_weights = optimize_weights_proximal
 
     bit_to_packing = {
         8: "8bit_u8",
+        6: "8bit_u8", #todo: bitpacking
+        5: "8bit_u8", #todo: bitpacking
         4: "4bit_u8",
         3: "3bit_32",
         2: "2bit_u8",
         1: "1bit_u8",
     }
 
     pack = {
@@ -155,20 +157,20 @@
     @classmethod
     def dequantize(cls, W_q: Tensor, meta: dict) -> Tensor:
         compute_dtype = meta["compute_dtype"] if ("compute_dtype" in meta) else float16
         if meta["packing"]:
             if meta["view_as_float"]:
                 W_q = W_q.view(meta["unpack_view_dtype"])
             W_r = Quantizer.unpack[meta["packing"]](W_q, dtype=compute_dtype)
-            if (meta["group_size"] is not None) and (meta["nbits"] == 3):
-                W_r = (
-                    W_r[: meta["group_size"]]
-                    if (meta["axis"] == 0)
-                    else W_r[:, : meta["group_size"]]
-                )
+            if meta["nbits"] == 3:
+                W_r = W_r[
+                    : meta["group_size"]
+                    if meta["axis"] == 0
+                    else meta["shape"][0] * meta["shape"][1] // meta["group_size"]
+                ]
         else:
             W_r = W_q.to(compute_dtype)
         W_r = ((W_r - meta["zero"]) * meta["scale"]).reshape(meta["shape"])
         return W_r
 
     @classmethod
     def to_inplace(cls, W_q: Tensor, meta: dict, device) -> tuple:
@@ -345,18 +347,15 @@
 
         return grad_input, grad_weight, grad_bias
 
 
 # Main linear layer
 class HQQLinear(nn.Module):
     # Default backend
-    if hqq_aten_is_available:
-        backend = HQQBackend.ATEN
-    else:
-        backend = HQQBackend.PYTORCH
+    backend = HQQBackend.PYTORCH
 
     def __init__(
         self,
         linear_layer: Union[nn.Module, None],
         quant_config: dict,
         del_orig: bool = True,
         compute_dtype: torch.dtype = float16,
@@ -376,38 +375,55 @@
             if (self.quant_config is not None)
             else None
         )
 
         self.set_backend(HQQLinear.backend)
 
         self.linear_layer = linear_layer
-
-        # Create streams
-        self.stream_zero = torch.cuda.Stream()
-        self.stream_scale = torch.cuda.Stream()
+        self.W_q = None
+        self.meta = None
 
         if initialize:
             self.initialize()
 
     def initialize(self):
         if self.linear_layer is not None:
             self.quantize(self.linear_layer.weight.data, **self.quant_config)
             self.bias = (
                 None
                 if (self.linear_layer.bias is None)
-                else self.linear_layer.bias.to(self.compute_dtype).cuda(self.device)
+                else self.linear_layer.bias.to(
+                    device=self.device, dtype=self.compute_dtype
+                )
             )
 
         if self.del_orig:
             del self.linear_layer
         torch.cuda.empty_cache()
 
+    def extra_repr(self) -> str:
+        out = ""
+        if hasattr(self, "meta"):
+            if self.meta is not None:
+                in_features, out_features = self.meta["shape"][::-1]
+                out = f"in_features={in_features}, out_features={out_features}, bias={self.bias is not None}"
+        return out
+
     # Set backends
     @classmethod
     def set_backend(cls, backend: HQQBackend):
+        if "aten" in backend.value:
+            if hqq_aten_is_available is False:
+                print(
+                    "ATEN/CUDA backend not availabe. Make sure you install the hqq_aten library."
+                )
+                return
+            print(
+                "Warning: the ATEN/CUDA backend only supports axis=0 and GPU runtime."
+            )
         HQQLinear.backend = backend
         cls.forward = getattr(cls, backend.value)
 
     # TODO: rewrite this mess
     def cuda(self, device):
         self.meta["compute_dtype"] = self.compute_dtype
 
@@ -473,15 +489,15 @@
 
         return self
 
     def to(self, *args, **kwargs):
         # TODO: later
         return self
 
-    #TODO: later
+    # TODO: later
     # def to_empty(self, device, recurse=True):
     #     return self.cuda(device)
 
     def type(self, dst_type):
         # TODO: later
         return self
 
@@ -499,16 +515,49 @@
     def double(self, *args, **kwargs):
         return self
 
     def cpu(self):
         # TODO: later
         return self
 
-    def state_dict(self, *args, **kwargs):
-        return {"W_q": self.W_q, "meta": self.meta, "bias": self.bias}
+    def state_dict(self, *args, **kwargs):  # nn.Module override compatible
+        state = {"W_q": self.W_q, "meta": self.meta, "bias": self.bias}
+        if "destination" in kwargs and "prefix" in kwargs:
+            for key, value in state.items():
+                kwargs["destination"][kwargs["prefix"] + key] = value
+        return state
+
+    def _load_from_state_dict(
+        self,
+        state_dict,
+        prefix,
+        local_metadata,
+        strict,
+        missing_keys,
+        unexpected_keys,
+        error_msgs,
+    ):
+        W_q_key = prefix + "W_q"
+        meta_key = prefix + "meta"
+        bias_key = prefix + "bias"
+
+        if W_q_key not in state_dict:
+            missing_keys.append(W_q_key)
+        if meta_key not in state_dict:
+            missing_keys.append(meta_key)
+        if missing_keys:
+            return  # Can't load weights if either weight or meta is missing
+
+        W_q = nn.Parameter(state_dict.pop(W_q_key), requires_grad=False)
+        meta = state_dict.pop(meta_key)
+        bias = state_dict.pop(bias_key, None)
+
+        unexpected_keys += state_dict.keys()
+
+        self.load_state_dict({"W_q": W_q, "meta": meta, "bias": bias}, strict)
 
     def load_state_dict(self, state_dict, strict=True, assign=False):
         self.W_q = state_dict["W_q"]
         self.meta = state_dict["meta"]
         self.bias = state_dict["bias"] if ("bias" in state_dict) else None
 
         # Meta-data offloading
@@ -668,14 +717,18 @@
             meta["axis"],
             meta["packing"],
         )
 
     def dequantize_aten(self):
         # Dequantize
         assert self.ready, "model was not quantized"
+        assert (
+            self.meta["axis"] == 0
+        ), "only axis=0 is supported. Use HQQLinear.set_backend(HQQBackend.PYTORCH) instead."
+
         W_q, meta = self.W_q, self.meta
         device = W_q.device
         del_keys = set()
 
         # Zero/Scale packed together
         if "zero_scale" in meta:
             zero_scale = meta["zero_scale"].to(device=device, non_blocking=True)
@@ -716,14 +769,19 @@
         for key in del_keys:
             del meta[key]
 
         return W_est
 
     # Much faster with data-offloading zero_q/scale_q but takes more VRAM
     def dequantize_aten_with_streams(self):
+        # Create streams
+        if hasattr(self, "stream_zero") is False:
+            self.stream_zero = torch.cuda.Stream()
+            self.stream_scale = torch.cuda.Stream()
+
         # Dequantize
         assert self.ready, "model was not quantized"
         W_q, meta = self.W_q, self.meta
         device = W_q.device
         del_keys = set()
 
         # Zero/Scale packed together
```

### Comparing `hqq-0.1.7.post2/hqq/core/utils.py` & `hqq-0.1.7.post3/hqq/core/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 import torch
 import gc
 import numpy as np
 from typing import Union
 
 
 def cleanup() -> None:
-    torch.cuda.empty_cache()
+    try:
+        torch.cuda.empty_cache()
+    except Exception:
+        pass
     gc.collect()
 
 
 def is_divisible(val1: int, val2: int) -> bool:
     return int(val2 * np.ceil(val1 / val2)) == val1
```

### Comparing `hqq-0.1.7.post2/hqq/engine/base.py` & `hqq-0.1.7.post3/hqq/engine/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Written by Dr. Hicham Badri @Mobius Labs GmbH - 2023
 #####################################################
 from abc import abstractmethod
 from ..models.base import BaseHQQModel
 import torch
 from torch import float16
+from typing import Union
 
 # Wrapper that makes it easier to add quantization support to different engines (HF, VLLM, etc.)
 
 
 class HQQWrapper:
     @abstractmethod
     def _get_arch_key_from_save_dir(cls, save_dir: str):
@@ -71,15 +72,15 @@
 
     @classmethod
     def from_quantized(
         cls,
         save_dir_or_hub,
         compute_dtype: torch.dtype = float16,
         device="cuda",
-        cache_dir: str | None = "",
+        cache_dir: Union[str,None] = "",
         adapter: str = None,
     ):
         # Both local and hub-support
         save_dir = BaseHQQModel.try_snapshot_download(save_dir_or_hub, cache_dir=cache_dir)
         arch_key = cls._get_arch_key_from_save_dir(save_dir)
         cls._check_arch_support(arch_key)
```

### Comparing `hqq-0.1.7.post2/hqq/engine/hf.py` & `hqq-0.1.7.post3/hqq/engine/hf.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post2/hqq/engine/timm.py` & `hqq-0.1.7.post3/hqq/engine/timm.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post2/hqq/engine/vllm.py` & `hqq-0.1.7.post3/hqq/engine/vllm.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post2/hqq/kernels/hqq_aten_cuda.cpp` & `hqq-0.1.7.post3/hqq/kernels/hqq_aten_cuda.cpp`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post2/hqq/kernels/hqq_aten_cuda_kernel.cu` & `hqq-0.1.7.post3/hqq/kernels/hqq_aten_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post2/hqq/kernels/hqq_aten_torch.cpp` & `hqq-0.1.7.post3/hqq/kernels/hqq_aten_torch.cpp`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post2/hqq/models/base.py` & `hqq-0.1.7.post3/hqq/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,31 @@
 # Written by Dr. Hicham Badri @Mobius Labs GmbH - 2023
 #####################################################
 import os
-import gc
 import torch
 from torch import nn
 from torch import float16
 from os.path import join as pjoin
 from typing import Callable
 from tqdm import tqdm
 from abc import abstractmethod
 from functools import partial
 from typing import Union
 
 from huggingface_hub import snapshot_download
+from ..core.utils import cleanup
 from ..core.quantize import HQQLinear
 from ..core.peft import PeftUtils, _HQQ_LORA_CLASSES
 
 
 # Defined what is qualified as "linear layer"
 _QUANT_LAYERS = [nn.Linear, HQQLinear] + _HQQ_LORA_CLASSES
 _IGNORE_LINEAR = ["lm_head"]
 
 
-# Cleanup GPU vram
-def cleanup() -> None:
-    torch.cuda.empty_cache()
-    gc.collect()
-
-
 # Finds the parent of a node module named "name"
 def find_parent(model, name: str) -> nn.Module:
     module_tree = name.split(".")[:-1]
     parent = model
     for m in module_tree:
         parent = parent._modules[m]
     return parent
@@ -207,15 +201,15 @@
 
 
 class BaseHQQModel:
     # Override these
     ############################################
     # This method creates and empty model based on the specfied architecture
     @abstractmethod
-    def create_model(self):
+    def create_model(cls, save_dir, kwargs):
         pass
 
     # This method saves the model architecture only without inculding the weights (for example to a config.json)
     @abstractmethod
     def cache_model(cls, model, save_dir: str):
         pass
 
@@ -250,15 +244,16 @@
     def quantize_model(
         cls,
         model,
         quant_config: dict,
         compute_dtype: torch.dtype = float16,
         device: Union[str, list, dict] = "cuda",
     ):
-        if hasattr(model, "hqq_quantized"):
+        # Check if the model was already quantized
+        if getattr(model, "hqq_quantized", False):
             print("Model was already quantized")
             return
 
         # Set linear tags automatically
         cls.setup_model(model)
 
         # Use the same quantization config for all linear layers. Use None to skip quantizing a specfic layer.
@@ -376,17 +371,14 @@
                 )
 
         # Set base class
         model.base_class = cls
 
         model.hqq_quantized = True
 
-        # Sync
-        torch.cuda.synchronize()
-
         return model
 
     # Prepares model weights by iterating through modules. It might some parameters that are NOT modules like model.param1
     @classmethod
     def serialize_weights(cls, model, verbose: bool = False) -> dict:
         weights = {}
         ignore_keys = cls.get_ignore_layers(model)
@@ -446,20 +438,21 @@
     def from_quantized(
         cls,
         save_dir_or_hub,
         compute_dtype: torch.dtype = float16,
         device="cuda",
         cache_dir: Union[str, None] = "",
         adapter: str = None,
+        **kwargs,
     ):
         # Get directory path
         save_dir = cls.try_snapshot_download(save_dir_or_hub, cache_dir)
 
         # Load model from config
-        model = cls.create_model(save_dir)
+        model = cls.create_model(save_dir, kwargs)
 
         # Track save directory
         model.save_dir = save_dir
 
         # Name the layers
         cls.setup_model(model)
 
@@ -517,11 +510,8 @@
         if adapter is not None:
             try:
                 PeftUtils.load_lora_weights(model, filename=pjoin(save_dir, adapter))
                 PeftUtils.cast_lora_weights(model, dtype=compute_dtype)
             except Exception as e:
                 print("Skipping adapter loading...", str(e))
 
-        # Sync
-        torch.cuda.synchronize()
-
         return model
```

### Comparing `hqq-0.1.7.post2/hqq/models/hf/base.py` & `hqq-0.1.7.post3/hqq/models/hf/base.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post2/hqq/models/hf/llama.py` & `hqq-0.1.7.post3/hqq/models/hf/llama.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post2/hqq/models/hf/mistral.py` & `hqq-0.1.7.post3/hqq/models/hf/mistral.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post2/hqq/models/hf/mixtral.py` & `hqq-0.1.7.post3/hqq/models/hf/mixtral.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post2/hqq/models/hf/phi.py` & `hqq-0.1.7.post3/hqq/models/hf/phi.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post2/hqq/models/hf/phi_opt.py` & `hqq-0.1.7.post3/hqq/models/hf/phi_opt.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post2/hqq/models/timm/base.py` & `hqq-0.1.7.post3/hqq/models/timm/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 import timm
 
 
 class BaseHQQTimmModel(BaseHQQModel):
     # Save model architecture
     @classmethod
-    def cache_model(cls, model, save_dir):
+    def cache_model(cls, model, save_dir, kwargs):
         try:
             os.makedirs(save_dir, exist_ok=True)
         except Exception as error:
             print(error)
 
         with open(cls.get_config_file(save_dir), "w") as file:
             json.dump(model.default_cfg, file)
```

### Comparing `hqq-0.1.7.post2/hqq/models/timm/vit_clip.py` & `hqq-0.1.7.post3/hqq/models/timm/vit_clip.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post2/hqq/models/vllm/base.py` & `hqq-0.1.7.post3/hqq/models/vllm/base.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post2/hqq/models/vllm/llama.py` & `hqq-0.1.7.post3/hqq/models/vllm/llama.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post2/hqq/utils/generation_hf.py` & `hqq-0.1.7.post3/hqq/utils/generation_hf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # Written by Dr. Hicham Badri @Mobius Labs GmbH - 2024
 #####################################################
 
 # Rewrite generate() to support torch.compile fullgraph.
 # https://gist.github.com/ArthurZucker/5dc54a3fb443e979fac437e5df7c800b
 
 import torch
+from typing import Union
 from transformers import StaticCache
 from tqdm import tqdm
 
 
 class HFGenerator:
     def __init__(
         self,
         model,
         tokenizer,
         max_new_tokens: int = 1000,
-        cache_size: int | None = None,
+        cache_size: Union[int,None] = None,
         do_sample: bool = False,
         temperature: float = 0.6,
         top_k: int = 5,
-        compile: str | None = None, #None / "partial" / "full"
+        compile: Union[str,None] = None, #None / "partial" / "full"
     ):
         super().__init__()
 
         torch._dynamo.config.cache_size_limit = 32
         torch._dynamo.config.capture_scalar_outputs = True
 
         self.model = model
```

### Comparing `hqq-0.1.7.post2/hqq/utils/patching.py` & `hqq-0.1.7.post3/hqq/utils/patching.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post2/hqq.egg-info/SOURCES.txt` & `hqq-0.1.7.post3/hqq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post2/setup.py` & `hqq-0.1.7.post3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def run(self):
         egg_info.run(self)
         run_setup_cuda()
 
 
 setup(
     name="hqq",
-    version="0.1.7.post2",
+    version="0.1.7.post3",
     description="Half-Quadratic Quantization (HQQ)",
     url="https://github.com/mobiusml/hqq/",
     author="Dr. Hicham Badri",
     author_email="hicham@mobiuslabs.com",
     license="Apache 2",
     packages=find_packages(include=["hqq", "hqq.*"]),
     package_data={
```

### Comparing `hqq-0.1.7.post2/tests/test_bitpack.py` & `hqq-0.1.7.post3/tests/test_bitpack.py`

 * *Files identical despite different names*

### Comparing `hqq-0.1.7.post2/tests/test_quantize.py` & `hqq-0.1.7.post3/tests/test_quantize.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 import unittest, tempfile
 import torch
 from hqq.core.quantize import Quantizer, HQQLinear, BaseQuantizeConfig, HQQBackend
 from hqq.engine.hf import HQQModelForCausalLM
-from transformers import AutoModelForCausalLM, AutoConfig
+from transformers import AutoModelForCausalLM, AutoConfig, LlamaForCausalLM
+
+
+class CustomLlamaModel(LlamaForCausalLM):
+    def __init__(self, config):
+        super().__init__(config)
+        # replacing head with custom linear layer
+        qcfg = BaseQuantizeConfig(nbits=2, group_size=64)
+        linear = torch.nn.Linear(config.hidden_size, config.vocab_size, bias=False)
+        self.lm_head = HQQLinear(linear, qcfg)
+
 
 # python -m unittest tests.test_quantize.TestQuantizer.test_quantizer
 class TestQuantizer(unittest.TestCase):
 
     def setUp(self) -> None:
         # set seed
         torch.manual_seed(42)
@@ -147,49 +157,65 @@
 
                                 x = torch.randn([batch_size, context_size, self.m.weight.shape[1]], device='cuda').to(compute_dtype)
                                 with torch.no_grad():
                                     y_int   = hqq_linear_int.forward(x)
                                     y_float = hqq_linear_float.forward(x)
 
                                 assert torch.allclose(y_int, y_float, rtol=1e-5)
-                                
+
+    @staticmethod
+    def assert_equal_models(model, model_qt):
+        def assert_state_dict(v1, v2):
+            if isinstance(v1, torch.Tensor):
+                assert torch.isclose(v1, v2, rtol=1e-5).float().mean().item() > 0.99
+            if isinstance(v1, dict):
+                for _k, _v in v1.items():
+                    if isinstance(_v, torch.Tensor):
+                        assert torch.equal(_v, v2[_k])
+                    else:
+                        assert _v == v2[_k]
+
+        for n, p in model.named_parameters():
+            module_key, _, value_key = n.rpartition('.')
+            d1 = model.get_submodule(module_key).state_dict()
+            d2 = model_qt.get_submodule(module_key).state_dict()
+            for (k1, v1), (k2, v2) in zip(d1.items(), d2.items()):
+                assert k1 == k2
+                assert_state_dict(v1, v2)
+
     def test_save_and_load_model(self):
         compute_dtype = torch.bfloat16
         model_name = "meta-llama/Llama-2-7b-hf"
         cfg = AutoConfig.from_pretrained(model_name)
         cfg.num_hidden_layers = 2
 
         # load model on meta device without calling init and replace nn.Linear with Linear4bit
         model = AutoModelForCausalLM.from_config(cfg)
-        
+
         # quantize and save
         quant_config = BaseQuantizeConfig(nbits=4, group_size=64, view_as_float=True)
         HQQModelForCausalLM.quantize_model_(model, quant_config, compute_dtype=compute_dtype)
         model.save_quantized(f"{self.tmp_dir}/models")
-        
+
         # load model
-        model_qt = HQQModelForCausalLM.from_quantized(f"{self.tmp_dir}/models")
-        
+        model_qt = HQQModelForCausalLM.from_quantized(f"{self.tmp_dir}/models", compute_dtype=compute_dtype)
+
         # check if the state_dicts are equal
-        def assert_state_dict(v1,v2):
-            if isinstance(v1, torch.Tensor):
-                assert torch.isclose(v1,v2, rtol=1e-5).float().mean().item() > 0.99
-            if isinstance(v1, dict):
-                for _k,_v in v1.items():
-                    if isinstance(_v, torch.Tensor):
-                        assert torch.equal(_v, v2[_k])
-                    else:
-                        assert _v == v2[_k]
+        self.assert_equal_models(model, model_qt)
+
+    def test_create_and_load_custom_model_with_hqqlinear_from_state_dict(self):
+        model_name = "meta-llama/Llama-2-7b-hf"
+        cfg = AutoConfig.from_pretrained(model_name)
+        cfg.num_hidden_layers = 2
+
+        model = CustomLlamaModel(cfg)
+        state_dict = model.state_dict()
+
+        loaded_model = CustomLlamaModel(cfg)
+        loaded_model.load_state_dict(state_dict)
+
+        # check if the state_dicts are equal
+        self.assert_equal_models(model, loaded_model)
+
 
-        for n,p in model.named_parameters():
-            module_key, _, value_key = n.rpartition('.')
-            d1 = model.get_submodule(module_key).state_dict()
-            d2 = model_qt.get_submodule(module_key).state_dict()
-            for (k1,v1),(k2,v2) in zip(d1.items(), d2.items()):
-                assert k1 == k2
-                assert_state_dict(v1,v2)
-        
-        
-                        
-                                    
 if __name__ == '__main__':
     unittest.main()
```

