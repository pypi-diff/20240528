# Comparing `tmp/nvidia_dali_cuda120-1.37.1.tar.gz` & `tmp/nvidia_dali_cuda120-1.38.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia_dali_cuda120-1.37.1.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
+gzip compressed data, was "nvidia_dali_cuda120-1.38.0.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `nvidia_dali_cuda120-1.37.1.tar` & `nvidia_dali_cuda120-1.38.0.tar`

### PKG-INFO

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-cuda120
-Version: 1.37.1
-Summary: NVIDIA DALI  for CUDA 12.0. Git SHA: d1685acebd5c41743cab0e15890660130e0276ce
+Version: 1.38.0
+Summary: NVIDIA DALI  for CUDA 12.0. Git SHA: 8f2a43f3436cafeafa4774513f7daf68ebbffad8
 Home-page: https://github.com/NVIDIA/dali
 Author: NVIDIA Corporation
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

