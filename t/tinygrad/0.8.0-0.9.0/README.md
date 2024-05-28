# Comparing `tmp/tinygrad-0.8.0.tar.gz` & `tmp/tinygrad-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinygrad-0.8.0.tar", last modified: Tue Jan  9 18:24:30 2024, max compression
+gzip compressed data, was "tinygrad-0.9.0.tar", last modified: Tue May 28 18:49:05 2024, max compression
```

## Comparing `tinygrad-0.8.0.tar` & `tinygrad-0.9.0.tar`

### file list

```diff
@@ -1,96 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 18:24:30.343506 tinygrad-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-01-09 18:24:22.000000 tinygrad-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-01-09 18:24:30.343506 tinygrad-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-01-09 18:24:22.000000 tinygrad-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-09 18:24:30.343506 tinygrad-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-01-09 18:24:22.000000 tinygrad-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 18:24:30.331506 tinygrad-0.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_conv_shapetracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_copy_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_custom_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    23997 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_dtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     8037 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_dtype_alu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_fusion_op.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_gc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_hip_rdna3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_image_dtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     9873 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_jit.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_kernel_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_lazybuffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_lazyop.py
--rw-r--r--   0 runner    (1001) docker     (127)    25338 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_linearizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23925 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_linearizer_failures.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_masked_st.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_method_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_multitensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_net_speed.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12398 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    84973 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_optim.py
--rw-r--r--   0 runner    (1001) docker     (127)     7353 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_randomness.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_specific_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    11620 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_speed_v_torch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_symbolic_jit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_symbolic_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_symbolic_shapetracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    17297 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_tensor_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_to_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_uops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_winograd.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-01-09 18:24:22.000000 tinygrad-0.8.0/test/test_zero_copy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 18:24:30.335506 tinygrad-0.8.0/tinygrad/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 18:24:30.335506 tinygrad-0.8.0/tinygrad/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)    35020 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/codegen/kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)    33166 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/codegen/linearizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    18438 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/dtype.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 18:24:30.335506 tinygrad-0.8.0/tinygrad/features/
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/features/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/features/multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/features/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    11771 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/jit.py
--rw-r--r--   0 runner    (1001) docker     (127)    16383 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8628 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/mlops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 18:24:30.335506 tinygrad-0.8.0/tinygrad/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/nn/optim.py
--rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/nn/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/realize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 18:24:30.335506 tinygrad-0.8.0/tinygrad/renderer/
--rw-r--r--   0 runner    (1001) docker     (127)    16951 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/renderer/cstyle.py
--rw-r--r--   0 runner    (1001) docker     (127)    10652 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/renderer/llvmir.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 18:24:30.339506 tinygrad-0.8.0/tinygrad/runtime/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 18:24:30.339506 tinygrad-0.8.0/tinygrad/runtime/graph/
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/runtime/graph/cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/runtime/graph/hip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/runtime/graph/metal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/runtime/ops_clang.py
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/runtime/ops_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/runtime/ops_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/runtime/ops_disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/runtime/ops_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/runtime/ops_hip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/runtime/ops_llvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/runtime/ops_metal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/runtime/ops_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 18:24:30.339506 tinygrad-0.8.0/tinygrad/shape/
--rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/shape/shapetracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    16565 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/shape/symbolic.py
--rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/shape/view.py
--rw-r--r--   0 runner    (1001) docker     (127)    58106 2024-01-09 18:24:22.000000 tinygrad-0.8.0/tinygrad/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 18:24:30.339506 tinygrad-0.8.0/tinygrad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-01-09 18:24:30.000000 tinygrad-0.8.0/tinygrad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-01-09 18:24:30.000000 tinygrad-0.8.0/tinygrad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 18:24:30.000000 tinygrad-0.8.0/tinygrad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-01-09 18:24:30.000000 tinygrad-0.8.0/tinygrad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-09 18:24:30.000000 tinygrad-0.8.0/tinygrad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:49:05.747423 tinygrad-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-28 18:48:56.000000 tinygrad-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-05-28 18:49:05.747423 tinygrad-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-05-28 18:48:56.000000 tinygrad-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 18:49:05.747423 tinygrad-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-28 18:48:56.000000 tinygrad-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:49:05.723423 tinygrad-0.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_arange.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12797 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10385 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_const_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_conv_shapetracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_copy_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_custom_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_device_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34630 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8303 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_dtype_alu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_fusion_op.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_fuzz_shape_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_gc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_image_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10912 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_jit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_kernel_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_lazybuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_lazyop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89185 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_linearizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70924 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_linearizer_failures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14889 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_linearizer_overflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_masked_st.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_method_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31384 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_multitensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_net_speed.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15424 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94808 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_optim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_pattern_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_randomness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27437 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_setitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_specific_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_speed_v_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_subbuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_symbolic_jit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_symbolic_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7554 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_symbolic_shapetracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21553 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_tensor_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_tensor_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_to_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_uop_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12860 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_uops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_uops_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_winograd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-28 18:48:56.000000 tinygrad-0.9.0/test/test_zero_copy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:49:05.727423 tinygrad-0.9.0/tinygrad/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:49:05.727423 tinygrad-0.9.0/tinygrad/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)    38169 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/codegen/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27622 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/codegen/linearizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21872 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/codegen/uops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/dtype.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:49:05.731423 tinygrad-0.9.0/tinygrad/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/engine/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11049 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/engine/jit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/engine/realize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18487 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/engine/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11289 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/engine/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12773 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13379 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/multi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:49:05.731423 tinygrad-0.9.0/tinygrad/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)    12932 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/nn/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/nn/optim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10138 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/nn/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:49:05.731423 tinygrad-0.9.0/tinygrad/renderer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/renderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17923 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/renderer/assembly.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24043 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/renderer/cstyle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/renderer/llvmir.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:49:05.735423 tinygrad-0.9.0/tinygrad/runtime/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:49:05.739423 tinygrad-0.9.0/tinygrad/runtime/autogen/
+-rw-r--r--   0 runner    (1001) docker     (127)    65022 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/runtime/autogen/amd_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38563 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/runtime/autogen/comgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)   250380 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/runtime/autogen/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)   245532 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/runtime/autogen/hip.py
+-rw-r--r--   0 runner    (1001) docker     (127)   270073 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/runtime/autogen/hsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29935 2024-05-28 18:48:56.000000 tinygrad-0.9.0/tinygrad/runtime/autogen/kfd.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1672024 2024-05-28 18:48:57.000000 tinygrad-0.9.0/tinygrad/runtime/autogen/nv_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82654 2024-05-28 18:48:57.000000 tinygrad-0.9.0/tinygrad/runtime/autogen/opencl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:49:05.739423 tinygrad-0.9.0/tinygrad/runtime/driver/
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-28 18:48:57.000000 tinygrad-0.9.0/tinygrad/runtime/driver/hip_comgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7218 2024-05-28 18:48:57.000000 tinygrad-0.9.0/tinygrad/runtime/driver/hsa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:49:05.743423 tinygrad-0.9.0/tinygrad/runtime/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-28 18:48:57.000000 tinygrad-0.9.0/tinygrad/runtime/graph/clang.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-28 18:48:57.000000 tinygrad-0.9.0/tinygrad/runtime/graph/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8089 2024-05-28 18:48:57.000000 tinygrad-0.9.0/tinygrad/runtime/graph/hcq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-05-28 18:48:57.000000 tinygrad-0.9.0/tinygrad/runtime/graph/hsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-05-28 18:48:57.000000 tinygrad-0.9.0/tinygrad/runtime/graph/metal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31811 2024-05-28 18:48:57.000000 tinygrad-0.9.0/tinygrad/runtime/ops_amd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-28 18:48:57.000000 tinygrad-0.9.0/tinygrad/runtime/ops_clang.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10840 2024-05-28 18:48:57.000000 tinygrad-0.9.0/tinygrad/runtime/ops_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-28 18:48:57.000000 tinygrad-0.9.0/tinygrad/runtime/ops_disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-05-28 18:48:57.000000 tinygrad-0.9.0/tinygrad/runtime/ops_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16188 2024-05-28 18:48:57.000000 tinygrad-0.9.0/tinygrad/runtime/ops_hsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-28 18:48:57.000000 tinygrad-0.9.0/tinygrad/runtime/ops_llvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-05-28 18:48:57.000000 tinygrad-0.9.0/tinygrad/runtime/ops_metal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-28 18:48:57.000000 tinygrad-0.9.0/tinygrad/runtime/ops_npy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37633 2024-05-28 18:48:57.000000 tinygrad-0.9.0/tinygrad/runtime/ops_nv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-05-28 18:48:57.000000 tinygrad-0.9.0/tinygrad/runtime/ops_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:49:05.743423 tinygrad-0.9.0/tinygrad/shape/
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-05-28 18:48:57.000000 tinygrad-0.9.0/tinygrad/shape/shapetracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16688 2024-05-28 18:48:57.000000 tinygrad-0.9.0/tinygrad/shape/symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17092 2024-05-28 18:48:57.000000 tinygrad-0.9.0/tinygrad/shape/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)   129223 2024-05-28 18:48:57.000000 tinygrad-0.9.0/tinygrad/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:49:05.743423 tinygrad-0.9.0/tinygrad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-05-28 18:49:05.000000 tinygrad-0.9.0/tinygrad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-28 18:49:05.000000 tinygrad-0.9.0/tinygrad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 18:49:05.000000 tinygrad-0.9.0/tinygrad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-28 18:49:05.000000 tinygrad-0.9.0/tinygrad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 18:49:05.000000 tinygrad-0.9.0/tinygrad.egg-info/top_level.txt
```

### Comparing `tinygrad-0.8.0/LICENSE` & `tinygrad-0.9.0/LICENSE`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright (c) 2023 George Hotz
+Copyright (c) 2024, the tiny corp
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `tinygrad-0.8.0/PKG-INFO` & `tinygrad-0.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: tinygrad
-Version: 0.8.0
+Version: 0.9.0
 Summary: You like pytorch? You like micrograd? You love tinygrad! <3
 Author: George Hotz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: tqdm
-Requires-Dist: gpuctypes
 Requires-Dist: pyobjc-framework-Metal; platform_system == "Darwin"
 Requires-Dist: pyobjc-framework-libdispatch; platform_system == "Darwin"
 Provides-Extra: llvm
 Requires-Dist: llvmlite; extra == "llvm"
 Provides-Extra: arm
 Requires-Dist: unicorn; extra == "arm"
 Provides-Extra: triton
@@ -28,29 +27,42 @@
 Requires-Dist: ruff; extra == "linting"
 Requires-Dist: types-tqdm; extra == "linting"
 Provides-Extra: testing
 Requires-Dist: torch; extra == "testing"
 Requires-Dist: pillow; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-xdist; extra == "testing"
-Requires-Dist: onnx==1.15.0; extra == "testing"
+Requires-Dist: onnx==1.16.0; extra == "testing"
 Requires-Dist: onnx2torch; extra == "testing"
 Requires-Dist: opencv-python; extra == "testing"
 Requires-Dist: tabulate; extra == "testing"
 Requires-Dist: safetensors; extra == "testing"
 Requires-Dist: transformers; extra == "testing"
 Requires-Dist: sentencepiece; extra == "testing"
 Requires-Dist: tiktoken; extra == "testing"
 Requires-Dist: librosa; extra == "testing"
 Requires-Dist: networkx; extra == "testing"
 Requires-Dist: hypothesis; extra == "testing"
+Requires-Dist: nibabel; extra == "testing"
+Provides-Extra: docs
+Requires-Dist: mkdocs-material; extra == "docs"
+Requires-Dist: mkdocstrings[python]; extra == "docs"
+Requires-Dist: markdown-callouts; extra == "docs"
+Requires-Dist: markdown-exec[ansi]; extra == "docs"
+Requires-Dist: black; extra == "docs"
+Provides-Extra: testing-tf
+Requires-Dist: tensorflow==2.15.1; extra == "testing-tf"
+Requires-Dist: tensorflow_addons; extra == "testing-tf"
 
 <div align="center">
 
-[![logo](https://raw.githubusercontent.com/tinygrad/tinygrad/master/docs/logo.png)](https://tinygrad.org)
+<picture>
+  <source media="(prefers-color-scheme: light)" srcset="/docs/logo_tiny_light.svg">
+  <img alt="tiny corp logo" src="/docs/logo_tiny_dark.svg" width="50%" height="50%">
+</picture>
 
 tinygrad: For something between [PyTorch](https://github.com/pytorch/pytorch) and [karpathy/micrograd](https://github.com/karpathy/micrograd). Maintained by [tiny corp](https://tinygrad.org).
 
 <h3>
 
 [Homepage](https://github.com/tinygrad/tinygrad) | [Documentation](/docs) | [Examples](/examples) | [Showcase](/docs/showcase.md) | [Discord](https://discord.gg/ZjZadyC7PK)
 
@@ -118,25 +130,22 @@
 
 See [examples/beautiful_mnist.py](examples/beautiful_mnist.py) for the full version that gets 98% in ~5 seconds
 
 ## Accelerators
 
 tinygrad already supports numerous accelerators, including:
 
-- [x] [CPU](tinygrad/runtime/ops_cpu.py)
 - [x] [GPU (OpenCL)](tinygrad/runtime/ops_gpu.py)
-- [x] [C Code (Clang)](tinygrad/runtime/ops_clang.py)
+- [x] [CLANG (C Code)](tinygrad/runtime/ops_clang.py)
 - [x] [LLVM](tinygrad/runtime/ops_llvm.py)
 - [x] [METAL](tinygrad/runtime/ops_metal.py)
 - [x] [CUDA](tinygrad/runtime/ops_cuda.py)
-- [x] [PyTorch](tinygrad/runtime/ops_torch.py)
-- [x] [HIP](tinygrad/runtime/ops_hip.py)
+- [x] [HSA](tinygrad/runtime/ops_hsa.py)
 
 And it is easy to add more! Your accelerator of choice only needs to support a total of ~25 low level ops.
-More information can be found in the [documentation for adding new accelerators](/docs/adding_new_accelerators.md).
 
 ## Installation
 
 The current recommended way to install tinygrad is from source.
 
 ### From source
 
@@ -189,14 +198,15 @@
 
 We'll start with what will get your PR closed with a pointer to this section:
 
 - No code golf! While low line count is a guiding light of this project, anything that remotely looks like code golf will be closed. The true goal is reducing complexity and increasing readability, and deleting `\n`s does nothing to help with that.
 - All docs and whitespace changes will be closed unless you are a well-known contributor. The people writing the docs should be those who know the codebase the absolute best. People who have not demonstrated that shouldn't be messing with docs. Whitespace changes are both useless *and* carry a risk of introducing bugs.
 - Anything you claim is a "speedup" must be benchmarked. In general, the goal is simplicity, so even if your PR makes things marginally faster, you have to consider the tradeoff with maintainablity and readablity.
 - In general, the code outside the core `tinygrad/` folder is not well tested, so unless the current code there is broken, you shouldn't be changing it.
+- If your PR looks "complex", is a big diff, or adds lots of lines, it won't be reviewed or merged. Consider breaking it up into smaller PRs that are individually clear wins. A common pattern I see is prerequisite refactors before adding new functionality. If you can (cleanly) refactor to the point that the feature is a 3 line change, this is great, and something easy for us to review.
 
 Now, what we want:
 
 - Bug fixes (with a regression test) are great! This library isn't 1.0 yet, so if you stumble upon a bug, fix it, write a test, and submit a PR, this is valuable work.
 - Solving bounties! tinygrad [offers cash bounties](https://docs.google.com/spreadsheets/d/1WKHbT-7KOgjEawq5h5Ic1qUWzpfAzuD_J06N1JwOCGs/edit?usp=sharing) for certain improvements to the library. All new code should be high quality and well tested.
 - Features. However, if you are adding a feature, consider the line tradeoff. If it's 3 lines, there's less of a bar of usefulness it has to meet over something that's 30 or 300 lines. All features must have regression tests. In general with no other constraints, your feature's API should match torch or numpy.
 - Refactors that are clear wins. In general, if your refactor isn't a clear win it will be closed. But some refactors are amazing! Think about readability in a deep core sense. A whitespace change or moving a few functions around is useless, but if you realize that two 100 line functions can actually use the same 110 line function with arguments while also improving readability, this is a big win.
```

### Comparing `tinygrad-0.8.0/README.md` & `tinygrad-0.9.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 <div align="center">
 
-[![logo](https://raw.githubusercontent.com/tinygrad/tinygrad/master/docs/logo.png)](https://tinygrad.org)
+<picture>
+  <source media="(prefers-color-scheme: light)" srcset="/docs/logo_tiny_light.svg">
+  <img alt="tiny corp logo" src="/docs/logo_tiny_dark.svg" width="50%" height="50%">
+</picture>
 
 tinygrad: For something between [PyTorch](https://github.com/pytorch/pytorch) and [karpathy/micrograd](https://github.com/karpathy/micrograd). Maintained by [tiny corp](https://tinygrad.org).
 
 <h3>
 
 [Homepage](https://github.com/tinygrad/tinygrad) | [Documentation](/docs) | [Examples](/examples) | [Showcase](/docs/showcase.md) | [Discord](https://discord.gg/ZjZadyC7PK)
 
@@ -72,25 +75,22 @@
 
 See [examples/beautiful_mnist.py](examples/beautiful_mnist.py) for the full version that gets 98% in ~5 seconds
 
 ## Accelerators
 
 tinygrad already supports numerous accelerators, including:
 
-- [x] [CPU](tinygrad/runtime/ops_cpu.py)
 - [x] [GPU (OpenCL)](tinygrad/runtime/ops_gpu.py)
-- [x] [C Code (Clang)](tinygrad/runtime/ops_clang.py)
+- [x] [CLANG (C Code)](tinygrad/runtime/ops_clang.py)
 - [x] [LLVM](tinygrad/runtime/ops_llvm.py)
 - [x] [METAL](tinygrad/runtime/ops_metal.py)
 - [x] [CUDA](tinygrad/runtime/ops_cuda.py)
-- [x] [PyTorch](tinygrad/runtime/ops_torch.py)
-- [x] [HIP](tinygrad/runtime/ops_hip.py)
+- [x] [HSA](tinygrad/runtime/ops_hsa.py)
 
 And it is easy to add more! Your accelerator of choice only needs to support a total of ~25 low level ops.
-More information can be found in the [documentation for adding new accelerators](/docs/adding_new_accelerators.md).
 
 ## Installation
 
 The current recommended way to install tinygrad is from source.
 
 ### From source
 
@@ -143,14 +143,15 @@
 
 We'll start with what will get your PR closed with a pointer to this section:
 
 - No code golf! While low line count is a guiding light of this project, anything that remotely looks like code golf will be closed. The true goal is reducing complexity and increasing readability, and deleting `\n`s does nothing to help with that.
 - All docs and whitespace changes will be closed unless you are a well-known contributor. The people writing the docs should be those who know the codebase the absolute best. People who have not demonstrated that shouldn't be messing with docs. Whitespace changes are both useless *and* carry a risk of introducing bugs.
 - Anything you claim is a "speedup" must be benchmarked. In general, the goal is simplicity, so even if your PR makes things marginally faster, you have to consider the tradeoff with maintainablity and readablity.
 - In general, the code outside the core `tinygrad/` folder is not well tested, so unless the current code there is broken, you shouldn't be changing it.
+- If your PR looks "complex", is a big diff, or adds lots of lines, it won't be reviewed or merged. Consider breaking it up into smaller PRs that are individually clear wins. A common pattern I see is prerequisite refactors before adding new functionality. If you can (cleanly) refactor to the point that the feature is a 3 line change, this is great, and something easy for us to review.
 
 Now, what we want:
 
 - Bug fixes (with a regression test) are great! This library isn't 1.0 yet, so if you stumble upon a bug, fix it, write a test, and submit a PR, this is valuable work.
 - Solving bounties! tinygrad [offers cash bounties](https://docs.google.com/spreadsheets/d/1WKHbT-7KOgjEawq5h5Ic1qUWzpfAzuD_J06N1JwOCGs/edit?usp=sharing) for certain improvements to the library. All new code should be high quality and well tested.
 - Features. However, if you are adding a feature, consider the line tradeoff. If it's 3 lines, there's less of a bar of usefulness it has to meet over something that's 30 or 300 lines. All features must have regression tests. In general with no other constraints, your feature's API should match torch or numpy.
 - Refactors that are clear wins. In general, if your refactor isn't a clear win it will be closed. But some refactors are amazing! Think about readability in a deep core sense. A whitespace change or moving a few functions around is useless, but if you realize that two 100 line functions can actually use the same 110 line function with arguments while also improving readability, this is a big win.
```

### Comparing `tinygrad-0.8.0/setup.py` & `tinygrad-0.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 from setuptools import setup
 
 directory = Path(__file__).resolve().parent
 with open(directory / 'README.md', encoding='utf-8') as f:
   long_description = f.read()
 
 setup(name='tinygrad',
-      version='0.8.0',
+      version='0.9.0',
       description='You like pytorch? You like micrograd? You love tinygrad! <3',
       author='George Hotz',
       license='MIT',
       long_description=long_description,
       long_description_content_type='text/markdown',
-      packages = ['tinygrad', 'tinygrad.codegen', 'tinygrad.nn', 'tinygrad.renderer',
-                  'tinygrad.runtime', 'tinygrad.runtime.graph', 'tinygrad.shape', 'tinygrad.features'],
+      packages = ['tinygrad', 'tinygrad.runtime.autogen', 'tinygrad.codegen', 'tinygrad.nn', 'tinygrad.renderer', 'tinygrad.engine',
+                  'tinygrad.runtime', 'tinygrad.runtime.driver', 'tinygrad.runtime.graph', 'tinygrad.shape'],
       classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License"
       ],
-      install_requires=["numpy", "tqdm", "gpuctypes",
+      install_requires=["numpy", "tqdm",
                         "pyobjc-framework-Metal; platform_system=='Darwin'",
                         "pyobjc-framework-libdispatch; platform_system=='Darwin'"],
       python_requires='>=3.8',
       extras_require={
         'llvm': ["llvmlite"],
         'arm': ["unicorn"],
         'triton': ["triton-nightly>=2.1.0.dev20231014192330"],
@@ -32,26 +32,39 @@
             "pylint",
             "mypy",
             "typing-extensions",
             "pre-commit",
             "ruff",
             "types-tqdm",
         ],
+        #'mlperf': ["mlperf-logging @ git+https://github.com/mlperf/logging.git@4.0.0-rc2"],
         'testing': [
             "torch",
             "pillow",
             "pytest",
             "pytest-xdist",
-            "onnx==1.15.0",
+            "onnx==1.16.0",
             "onnx2torch",
             "opencv-python",
             "tabulate",
             "safetensors",
             "transformers",
             "sentencepiece",
             "tiktoken",
             "librosa",
             "networkx",
             "hypothesis",
+            "nibabel",
+        ],
+        'docs': [
+            "mkdocs-material",
+            "mkdocstrings[python]",
+            "markdown-callouts",
+            "markdown-exec[ansi]",
+            "black"
+        ],
+        'testing_tf': [
+            "tensorflow==2.15.1",
+            "tensorflow_addons",
         ]
       },
       include_package_data=True)
```

### Comparing `tinygrad-0.8.0/test/test_conv.py` & `tinygrad-0.9.0/test/test_conv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import unittest
 import numpy as np
-from tinygrad.tensor import Tensor, Device
+from tinygrad.tensor import Tensor
+from tinygrad.helpers import Context
 
 class TestConv(unittest.TestCase):
   def test_simple(self):
     x = Tensor.ones(1,12,128,256).contiguous().realize()
     w = Tensor.ones(32,12,3,3).contiguous().realize()
     ret = x.conv2d(w, stride=(2,2), padding=(1,1)).numpy()
     # it's not 108 around the padding
@@ -57,26 +58,23 @@
     w = Tensor.randn(32,12,3,3)
     out = x.conv2d(w, stride=(2,2), padding=(1,1))
     r1, r2 = out.relu(), out.elu()
     np.testing.assert_allclose(r1.numpy(), np.maximum(out.numpy(), 0))
     np.testing.assert_allclose(r2.numpy(), np.where(out.numpy() > 0, out.numpy(), (np.exp(out.numpy()) - 1)), atol=1e-5)
     Tensor.no_grad = False
 
-  @unittest.skipIf(Device.DEFAULT != "TORCH", "Takes too long to compile for Compiled backends")
   def test_two_overlapping_binops_no_rerun_wino(self):
     Tensor.no_grad = True
-    old_wino = Tensor.wino
-    Tensor.wino = True
-    x = Tensor.randn(1,4,16,16)
-    w = Tensor.randn(6,4,3,3)
-    out = x.conv2d(w, padding=(1,1))
-    r1, r2 = out.relu(), out.elu()
-    np.testing.assert_allclose(r1.numpy(), np.maximum(out.numpy(), 0))
-    np.testing.assert_allclose(r2.numpy(), np.where(out.numpy() > 0, out.numpy(), (np.exp(out.numpy()) - 1)), atol=1e-5)
-    Tensor.wino = old_wino
+    with Context(WINO=1):
+      x = Tensor.randn(1,4,16,16)
+      w = Tensor.randn(6,4,3,3)
+      out = x.conv2d(w, padding=(1,1))
+      r1, r2 = out.relu(), out.elu()
+      np.testing.assert_allclose(r1.numpy(), np.maximum(out.numpy(), 0))
+      np.testing.assert_allclose(r2.numpy(), np.where(out.numpy() > 0, out.numpy(), (np.exp(out.numpy()) - 1)), atol=1e-5)
     Tensor.no_grad = False
 
   def test_first_three(self):
     Tensor.no_grad = True
     x = Tensor.rand(1,12,128,256)
 
     w = Tensor.rand(32,12,3,3)
@@ -137,8 +135,8 @@
     x = x.reshape((1, 12, 256, 128))
     x += 1
     x += 1
     x = x.reshape((1, 12, 128, 256))
     x.numpy()
 
 if __name__ == '__main__':
-  unittest.main()
+  unittest.main()
```

### Comparing `tinygrad-0.8.0/test/test_copy_speed.py` & `tinygrad-0.9.0/test/test_copy_speed.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,45 +20,45 @@
       with Timing("sync:  ", on_exit=lambda ns: f" @ {t.nbytes()/ns:.2f} GB/s"):
         with Timing("queue: "):
           t.to(Device.DEFAULT).realize()
         Device[Device.DEFAULT].synchronize()
     s.unlink()
 
   def testCopyCPUtoDefault(self):
-    t = Tensor.rand(N, N, device="cpu").realize()
+    t = Tensor.rand(N, N, device="clang").realize()
     print(f"buffer: {t.nbytes()*1e-9:.2f} GB")
     for _ in range(3):
       with Timing("sync:  ", on_exit=lambda ns: f" @ {t.nbytes()/ns:.2f} GB/s"):
         with Timing("queue: "):
           t.to(Device.DEFAULT).realize()
         Device[Device.DEFAULT].synchronize()
 
   def testCopyCPUtoDefaultFresh(self):
     print("fresh copy")
     for _ in range(3):
-      t = Tensor.rand(N, N, device="cpu").realize()
+      t = Tensor.rand(N, N, device="clang").realize()
       with Timing("sync:  ", on_exit=lambda ns: f" @ {t.nbytes()/ns:.2f} GB/s"): # noqa: F821
         with Timing("queue: "):
           t.to(Device.DEFAULT).realize()
         Device[Device.DEFAULT].synchronize()
       del t
 
   def testCopyDefaulttoCPU(self):
     t = Tensor.rand(N, N).realize()
     print(f"buffer: {t.nbytes()*1e-9:.2f} GB")
     for _ in range(3):
       with Timing("sync:  ", on_exit=lambda ns: f" @ {t.nbytes()/ns:.2f} GB/s"):
-        t.to('cpu').realize()
+        t.to('clang').realize()
 
   @unittest.skipIf(CI, "CI doesn't have 6 GPUs")
   @unittest.skipIf(Device.DEFAULT != "GPU", "only test this on GPU")
   def testCopyCPUto6GPUs(self):
     from tinygrad.runtime.ops_gpu import CLDevice
     if len(CLDevice.device_ids) != 6: raise unittest.SkipTest("computer doesn't have 6 GPUs")
-    t = Tensor.rand(N, N, device="cpu").realize()
+    t = Tensor.rand(N, N, device="clang").realize()
     print(f"buffer: {t.nbytes()*1e-9:.2f} GB")
     for _ in range(3):
       with Timing("sync:  ", on_exit=lambda ns: f" @ {t.nbytes()/ns:.2f} GB/s ({t.nbytes()*6/ns:.2f} GB/s total)"):
         with Timing("queue: "):
           for g in range(6):
             t.to(f"gpu:{g}").realize()
         Device["gpu"].synchronize()
```

### Comparing `tinygrad-0.8.0/test/test_custom_function.py` & `tinygrad-0.9.0/test/test_custom_function.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 from typing import Optional, Tuple
 from tinygrad.helpers import prod
 from tinygrad.dtype import dtypes
 
 # *** first, we implement the atan2 op at the lowest level ***
 # `atan2_gpu` for GPUBuffers and `atan2_cpu` for CPUBuffers
 from tinygrad.lazy import Buffer, create_lazybuffer
-from tinygrad.device import CompiledASTRunner, Device
+from tinygrad.device import Device
 from tinygrad.shape.shapetracker import ShapeTracker
+from tinygrad.engine.realize import CompiledRunner
+from tinygrad.renderer import Program
 
 # we don't always have GPU support, so the type signature is the abstract CompiledBuffer instead of GPUBuffer
 def atan2_gpu(ret:Buffer, a:Buffer, b:Buffer):
   assert a.dtype == b.dtype and a.dtype == dtypes.float32, "gpu function only supports float32"
   src = """
   __kernel void atan2_gpu(global float *c, global float *a, global float *b) {
     int idx = get_global_id(0);
     c[idx] = atan2(a[idx], b[idx]);
   }"""
-  lib = Device[ret.device].compiler(src)
-  CompiledASTRunner(None, "atan2_gpu", src, lib, global_size=[ret.size]).build(Device[ret.device].runtime).exec([ret, a, b])
+  CompiledRunner(Program("atan2_gpu", src, ret.device, global_size=[ret.size,1,1])).exec([ret, a, b])
 
 def atan2_cpu(ret:Buffer, a:Buffer, b:Buffer): ret.copyin(np.require(np.arctan2(a._buf, b._buf), requirements='C').data)
 
 # *** second, we write the ATan2 mlop ***
 # NOTE: The derivative of atan2 doesn't need a custom op! https://www.liquisearch.com/atan2/derivative
 # In general, it is also optional to write a backward function, just your backward pass won't work without it
 
@@ -84,15 +85,15 @@
     assert ta.grad is not None and tb.grad is not None, "torch didn't compute gradients"
     np.testing.assert_allclose(a.grad.numpy(), ta.grad.numpy(), atol=1e-5)
     np.testing.assert_allclose(b.grad.numpy(), tb.grad.numpy(), atol=1e-5)
 
   @unittest.skipIf(Device.DEFAULT in ["CPU"], "atan2_cpu not jittable")
   def test_atan2_jit(self):
     # custom ops even work in the JIT!
-    from tinygrad.jit import TinyJit
+    from tinygrad.engine.jit import TinyJit
 
     @TinyJit
     def jitted_atan2(a:Tensor, b:Tensor) -> Tensor:
       return ATan2.apply(a, b).realize()
 
     for _ in range(5):
       a = Tensor.randn(4,4,requires_grad=True).permute(1,0)
```

### Comparing `tinygrad-0.8.0/test/test_dtype.py` & `tinygrad-0.9.0/test/test_dtype.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,24 @@
-import unittest
+import unittest, operator, subprocess
 import numpy as np
 import torch
-import operator
-from tinygrad.helpers import CI, getenv, DEBUG, OSX, temp
-from tinygrad.dtype import DType, DTYPES_DICT, ImageDType, PtrDType, least_upper_float, least_upper_dtype
-from tinygrad import Device
-from tinygrad.tensor import Tensor, dtypes
 from typing import Any, List
-from hypothesis import given, settings, strategies as st
+from tinygrad.helpers import getenv, DEBUG, CI
+from tinygrad.dtype import DType, DTYPES_DICT, ImageDType, PtrDType, least_upper_float, least_upper_dtype
+from tinygrad import Device, Tensor, dtypes
+from hypothesis import given, settings, strategies as strat
+from test.helpers import is_dtype_supported, rand_for_dtype
+
+settings.register_profile("my_profile", max_examples=200, deadline=None)
+settings.load_profile("my_profile")
 
 core_dtypes = list(DTYPES_DICT.values())
-floats = [dt for dt in core_dtypes if dtypes.is_float(dt)]
-def is_dtype_supported(dtype: DType, device: str = Device.DEFAULT):
-  if dtype == dtypes.bfloat16: return False # numpy doesn't support bf16, tested separately in TestBFloat16DType
-  if device in ["WEBGPU", "WEBGL"]: return dtype in [dtypes.float, dtypes.int32, dtypes.uint32]
-  if device == "TORCH": return dtype not in [dtypes.uint16, dtypes.uint32, dtypes.uint64]
-  # for CI GPU, cl_khr_fp16 isn't supported
-  # for CI LLVM, it segfaults because it can't link to the casting function
-  # CUDA in CI uses CUDACPU that does not support half
-  if dtype == dtypes.half: return not (CI and device in ["GPU", "LLVM", "CUDA"])
-  if dtype == dtypes.float64: return device != "METAL" and not (OSX and device == "GPU")
-  return True
+if Device.DEFAULT == "CPU": core_dtypes.remove(dtypes.bfloat16)  # NOTE: this is for teenygrad, don't remove
+dtype_ints = [dt for dt in core_dtypes if dtypes.is_int(dt) and is_dtype_supported(dt)]
+dtype_floats = [dt for dt in core_dtypes if dtypes.is_float(dt) and is_dtype_supported(dt)]
 
 def get_available_cast_dtypes(dtype: DType) -> List[DType]:
   if not is_dtype_supported(dtype): return []
   return [v for k, v in DTYPES_DICT.items() if v != dtype and is_dtype_supported(v) and not k.startswith("_")] # dont cast internal dtypes
 
 def _test_to_np(a:Tensor, np_dtype, target):
   if DEBUG >= 2: print(a)
@@ -36,34 +30,43 @@
   except AssertionError as e:
     raise AssertionError(f"\ntensor {a.numpy()} does not match target {target} with np_dtype {np_dtype}") from e
 
 def _assert_eq(tensor:Tensor, target_dtype:DType, target):
   if DEBUG >= 2: print(tensor.numpy())
   try:
     assert tensor.dtype == target_dtype
-    np.testing.assert_allclose(tensor.numpy(), target)
+    np.testing.assert_allclose(tensor.numpy(), target, rtol={dtypes.float16:1e-3, dtypes.bfloat16:1e-2}.get(target_dtype, 1e-7))
   except AssertionError as e:
     raise AssertionError(f"\ntensor {tensor.numpy()} dtype {tensor.dtype} does not match target {target} with dtype {target_dtype}") from e
 
 def _test_op(fxn, target_dtype:DType, target):
   _assert_eq(fxn(), target_dtype, target)
 def _test_cast(a:Tensor, target_dtype:DType):
+  if a.is_floating_point() and dtypes.is_unsigned(target_dtype):
+    # converting negative float to unsigned integer is undefined
+    a = a.abs()
+  if target_dtype == dtypes.half and Device.DEFAULT == "PYTHON":
+    # TODO: struct.pack cannot pack value > 65504 (max of half) into e format
+    a = (a > 65504).where(65504, a)
+  if CI and Device.DEFAULT == "CLANG" and (target_dtype, a.dtype) in [(dtypes.double, dtypes.half), (dtypes.half, dtypes.double)]:
+    # TODO: cast between double and half are broken https://github.com/tinygrad/tinygrad/issues/4084
+    return
+
   _test_op(lambda: a.cast(target_dtype), target_dtype, list(a.numpy().astype(target_dtype.np)))
 def _test_bitcast(a:Tensor, target_dtype:DType, target=None):
+  if target_dtype == dtypes.bfloat16: raise unittest.SkipTest("no test for bf16 bitcast yet")
   _test_op(lambda: a.bitcast(target_dtype), target_dtype, target or a.numpy().view(target_dtype.np).tolist())
 
 class TestDType(unittest.TestCase):
   DTYPE: Any = None
   DATA: Any = None
   @classmethod
   def setUpClass(cls):
     if not cls.DTYPE or not is_dtype_supported(cls.DTYPE): raise unittest.SkipTest("dtype not supported")
-    if dtypes.is_int(cls.DTYPE): cls.DATA = np.random.randint(0, 100, size=10, dtype=cls.DTYPE.np).tolist()
-    elif cls.DTYPE == dtypes.bool: cls.DATA = np.random.choice([True, False], size=10).tolist()
-    else: cls.DATA = np.random.uniform(0, 1, size=10).tolist()
+    cls.DATA = rand_for_dtype(cls.DTYPE, 10)
   def setUp(self):
     if self.DTYPE is None: raise unittest.SkipTest("base class")
 
   def test_to_np(self): _test_to_np(Tensor(self.DATA, dtype=self.DTYPE), self.DTYPE.np, np.array(self.DATA, dtype=self.DTYPE.np))
 
   def test_casts_to(self): list(map(
     lambda dtype: _test_cast(Tensor(self.DATA, dtype=dtype), self.DTYPE),
@@ -99,98 +102,176 @@
     ))
 
   def test_dtypes_fields(self):
     fields = dtypes.fields()
     self.assertTrue(all(isinstance(value, DType) for value in fields.values()))
     self.assertTrue(all(issubclass(value.np, np.generic) for value in fields.values() if value.np is not None))
 
+  def test_resulting_and_init_dtypes_match(self):
+    dtypes = list(map(np.dtype, ["bool", "uint8", "int8", "int16", "int32", "int64", "float32", "float64"]))
+    data = [1., 2., 0., 0.5, -1.5, 5.25]
+    for dt in dtypes:
+      arr = np.asarray(data, dtype=dt)
+      tin = Tensor(arr).numpy()
+      tor = torch.as_tensor(arr).detach().numpy()
+      assert dt == tin.dtype == tor.dtype, f"dtype mismatch: expected={dt} | tinygrad={tin.dtype} | torch={tor.dtype}"
+      np.testing.assert_allclose(tin, tor, atol=1e-6, rtol=1e-3)
+
 def _test_ops(a_dtype:DType, b_dtype:DType, target_dtype=None):
   target_dtype = target_dtype or least_upper_dtype(a_dtype, b_dtype)
   if not is_dtype_supported(a_dtype) or not is_dtype_supported(b_dtype) or not is_dtype_supported(target_dtype): return
   if a_dtype == dtypes.bool or b_dtype == dtypes.bool: return
   _assert_eq(Tensor([1,2,3,4], dtype=a_dtype)+Tensor([1,2,3,4], dtype=b_dtype), target_dtype, [2,4,6,8])
+  _assert_eq((Tensor([1], dtype=a_dtype).cast(b_dtype)+Tensor([1], dtype=a_dtype).cast(b_dtype)).cast(a_dtype), a_dtype, [2])
   _assert_eq(Tensor([1,2,3,4], dtype=a_dtype)*Tensor([1,2,3,4], dtype=b_dtype), target_dtype, [1,4,9,16])
   _assert_eq(Tensor([[1,2],[3,4]], dtype=a_dtype)@Tensor.eye(2, dtype=b_dtype), target_dtype, [[1,2],[3,4]])
   _assert_eq(Tensor([1,1,1,1], dtype=a_dtype)+Tensor.ones((4,4), dtype=b_dtype), target_dtype, 2*Tensor.ones(4,4).numpy())
 
-@unittest.skipUnless(Device.DEFAULT in ["LLVM", "TORCH"], "bfloat16 not supported")
+@unittest.skipUnless(is_dtype_supported(dtypes.bfloat16), "bfloat16 not supported")
+class TestBFloat16(unittest.TestCase):
+  def test_bf16_creation_numpy(self):
+    data = [-1, 1, 2]
+    t = Tensor(data, dtype=dtypes.bfloat16)
+    assert t.dtype == dtypes.bfloat16
+    tnp = t.numpy()
+    assert tnp.dtype == np.float32
+    np.testing.assert_allclose(tnp, np.array(data))
+
+  def test_bf16_ones(self):
+    t = Tensor.ones(3, 5, dtype=dtypes.bfloat16)
+    assert t.dtype == dtypes.bfloat16
+    np.testing.assert_allclose(t.numpy(), np.ones((3, 5)))
+
+  def test_bf16_eye(self):
+    t = Tensor.eye(3, dtype=dtypes.bfloat16)
+    assert t.dtype == dtypes.bfloat16
+    np.testing.assert_allclose(t.numpy(), np.eye(3))
+
+@unittest.skipUnless(is_dtype_supported(dtypes.bfloat16), "bfloat16 not supported")
 class TestBFloat16DType(unittest.TestCase):
   def test_bf16_to_float(self):
-    with self.assertRaises(AssertionError):
-      _test_cast(Tensor([100000], dtype=dtypes.bfloat16), dtypes.float32)
+    _test_cast(Tensor([100000], dtype=dtypes.bfloat16), dtypes.float32)
 
   def test_float_to_bf16(self):
-    with self.assertRaises(AssertionError):
-      _test_cast(Tensor([100000], dtype=dtypes.float32), dtypes.bfloat16)
-
-  # torch.tensor([10000, -1, -1000, -10000, 20]).type(torch.bfloat16)
+    _test_cast(Tensor([100000], dtype=dtypes.float32), dtypes.bfloat16)
 
   def test_bf16(self):
     t = Tensor([10000, -1, -1000, -10000, 20]).cast(dtypes.bfloat16)
     t.realize()
     back = t.cast(dtypes.float32)
     assert tuple(back.numpy().tolist()) == (9984., -1, -1000, -9984, 20)
 
-  def test_bf16_disk_write_read(self):
-    t = Tensor([10000, -1, -1000, -10000, 20]).cast(dtypes.float32)
-    t.to(f"disk:{temp('f32')}").realize()
-
-    # hack to "cast" f32 -> bf16
-    with open(temp('f32'), "rb") as f: dat = f.read()
-    adat = b''.join([dat[i+2:i+4] for i in range(0, len(dat), 4)])
-    with open(temp('bf16'), "wb") as f: f.write(adat)
-
-    t = Tensor.empty(5, dtype=dtypes.bfloat16, device=f"disk:{temp('bf16')}").llvm().realize()
-    back = t.cast(dtypes.float32)
-    assert tuple(back.numpy().tolist()) == (9984., -1, -1000, -9984, 20)
-
-class TestHalfDtype(TestDType): DTYPE = dtypes.half
+@unittest.skipUnless(is_dtype_supported(dtypes.bfloat16), "bfloat16 not supported")
+class TestBFloat16DTypeCast(unittest.TestCase):
+  def test_f16_to_bf16_conversion(self):
+    original_tensor = Tensor([1.0, 2.0, 3.0], dtype=dtypes.float16)
+    converted_tensor = original_tensor.cast(dtypes.bfloat16)
+    self.assertEqual(converted_tensor.dtype, dtypes.bfloat16)
+    back_to_float32 = converted_tensor.cast(dtypes.float32)
+    original_to_float32 = original_tensor.cast(dtypes.float32)
+    np.testing.assert_allclose(back_to_float32.numpy(), original_to_float32.numpy(), rtol=1e-2, atol=1e-3)
+
+  def test_f16_to_bf16_edge_cases(self):
+    edge_cases = Tensor([0.0, -0.0, float('inf'), float('-inf'), float('nan')], dtype=dtypes.float16)
+    converted = edge_cases.cast(dtypes.bfloat16).cast(dtypes.float32)
+    np.testing.assert_equal(converted.numpy(), edge_cases.cast(dtypes.float32).numpy())
+
+  def test_f16_to_bf16_range_precision(self):
+    large_value = Tensor([65504.0], dtype=dtypes.float16)  # Max representable in float16
+    small_value = Tensor([6.1035e-5], dtype=dtypes.float16)  # Smallest positive normal float16
+    large_converted = large_value.cast(dtypes.bfloat16).cast(dtypes.float32)
+    small_converted = small_value.cast(dtypes.bfloat16).cast(dtypes.float32)
+    np.testing.assert_allclose(large_converted.numpy(), large_value.cast(dtypes.float32).numpy(), rtol=1e-2, atol=1e-3)
+    np.testing.assert_equal(small_converted.numpy(), small_value.cast(dtypes.float32).numpy())
+
+  def test_f16_to_bf16_randomized(self):
+    np.random.seed(42)  # For reproducibility
+    random_values = Tensor(np.random.uniform(-65504, 65504, 1000), dtype=dtypes.float16)
+    converted = random_values.cast(dtypes.bfloat16).cast(dtypes.float32)
+    np.testing.assert_allclose(converted.numpy(), random_values.cast(dtypes.float32).numpy(), rtol=1e-2, atol=1e-3)
+
+class TestHalfDType(TestDType): DTYPE = dtypes.half
+
+class TestFloatDType(TestDType):
+  DTYPE = dtypes.float
+
+  def test_float_to_uint(self):
+    _test_op(lambda: Tensor([-0.9, -0.3, 1.2], dtype=dtypes.float32).cast(dtypes.uint32), dtypes.uint32,
+             [0, 0, 1])
+
+class TestDoubleDType(TestDType):
+  DTYPE = dtypes.double
+  @unittest.skipIf((CI and Device.DEFAULT in {"CUDA", "NV"}) or getenv("PTX"), "conversion not supported on CUDACPU and PTX")  # TODO: why not?
+  def test_float64_increased_precision(self):
+    for func in [
+      lambda t: t.exp(),
+      lambda t: t.exp2(),
+      lambda t: t.log(),
+      lambda t: t.log2(),
+      lambda t: t.sqrt(),
+      lambda t: t.rsqrt(),
+      lambda t: t.sin(),
+      lambda t: t.cos(),
+      lambda t: t.tan(),
+      lambda t: t.sigmoid(),
+    ]:
+      a = [2, 3, 4]
+      np.testing.assert_allclose(func(Tensor(a, dtype=self.DTYPE)).numpy(), func(torch.tensor(a, dtype=torch.float64)), rtol=1e-12, atol=1e-12)
 
-class TestFloatDType(TestDType): DTYPE = dtypes.float
+  def test_float64_to_float32_cast_inf(self):
+    _test_op(lambda: Tensor([3.4e40, 3.4e38, 1, 0], dtype=dtypes.float64).cast(dtypes.float32),
+             dtypes.float32, [float('inf'), 3.4e38, 1, 0])
 
-class TestDoubleDtype(TestDType): DTYPE = dtypes.double
 
-class TestInt8Dtype(TestDType):
+class TestInt8DType(TestDType):
   DTYPE = dtypes.int8
   @unittest.skipIf(getenv("CUDA",0)==1 or getenv("PTX", 0)==1, "cuda saturation works differently")
   def test_int8_to_uint8_negative(self):
     _test_op(lambda: Tensor([-1, -2, -3, -4], dtype=dtypes.int8).cast(dtypes.uint8), dtypes.uint8, [255, 254, 253, 252])
 
-class TestUint8Dtype(TestDType):
+  def test_int8_to_uint16_negative(self):
+    _test_op(lambda: Tensor([-1, -2, -3, -4], dtype=dtypes.int8).cast(dtypes.uint16), dtypes.uint16, [2**16-1, 2**16-2, 2**16-3, 2**16-4])
+
+class TestUint8DType(TestDType):
   DTYPE = dtypes.uint8
   @unittest.skipIf(getenv("CUDA",0)==1 or getenv("PTX", 0)==1, "cuda saturation works differently")
   def test_uint8_to_int8_overflow(self):
     _test_op(lambda: Tensor([255, 254, 253, 252], dtype=dtypes.uint8).cast(dtypes.int8), dtypes.int8, [-1, -2, -3, -4])
 
 @unittest.skipIf(Device.DEFAULT == "WEBGL", "No bitcast on WebGL")
 class TestBitCast(unittest.TestCase):
   def test_shape_change_bitcast(self):
-    with self.assertRaises(AssertionError):
+    with self.assertRaises(RuntimeError):
       _test_bitcast(Tensor([100000], dtype=dtypes.float32), dtypes.uint8, [100000])
 
   def test_bitcast_float_to_int32(self):
     a = Tensor([1.,2,3])
     b = a.bitcast(dtypes.int32)
     assert b.numpy()[0] == 0x3f800000
 
   def test_bitcast_upcasted(self):
     a = Tensor.zeros(100, 4, dtype=dtypes.int32).contiguous() + 0x3f800000
     b = a.bitcast(dtypes.float32)
     assert b.numpy()[0,0] == 1.
 
-class TestInt16Dtype(TestDType): DTYPE = dtypes.int16
-class TestUint16Dtype(TestDType): DTYPE = dtypes.uint16
+class TestInt16DType(TestDType): DTYPE = dtypes.int16
 
-class TestInt32Dtype(TestDType): DTYPE = dtypes.int32
-class TestUint32Dtype(TestDType): DTYPE = dtypes.uint32
+class TestUint16DType(TestDType):
+  DTYPE = dtypes.uint16
 
-class TestInt64Dtype(TestDType): DTYPE = dtypes.int64
-class TestUint64Dtype(TestDType): DTYPE = dtypes.uint64
+  def test_uint16_to_int8_overflow(self):
+    _test_op(lambda: Tensor([2**16-1, 2**16-2, 1, 0], dtype=dtypes.uint16).cast(dtypes.int8), dtypes.int8, [-1, -2, 1, 0])
 
-class TestBoolDtype(TestDType): DTYPE = dtypes.bool
+class TestInt32DType(TestDType): DTYPE = dtypes.int32
+class TestUint32DType(TestDType): DTYPE = dtypes.uint32
+
+class TestInt64DType(TestDType): DTYPE = dtypes.int64
+class TestUint64DType(TestDType): DTYPE = dtypes.uint64
+
+class TestBoolDType(TestDType): DTYPE = dtypes.bool
 
 class TestImageDType(unittest.TestCase):
   def test_image_scalar(self):
     assert dtypes.imagef((10,10)).scalar() == dtypes.float32
     assert dtypes.imageh((10,10)).scalar() == dtypes.float32
   def test_image_vec(self):
     assert dtypes.imagef((10,10)).vec(4) == dtypes.float32.vec(4)
@@ -204,148 +285,179 @@
     assert dtypes.imageh((1,2,4)) != dtypes.imageh((1,4,2)), "different shape doesn't match"
     assert dtypes.imageh((1,2,4)) == dtypes.imageh((1,2,4)), "same shape matches"
     assert isinstance(dtypes.imageh((1,2,4)), ImageDType)
   def test_ptr_ne(self):
     if PtrDType is None: raise unittest.SkipTest("no PtrDType support")
     # TODO: is this the wrong behavior?
     assert PtrDType(dtypes.float32) == dtypes.float32
-    #assert PtrDType(dtypes.float32) == PtrDType(dtypes.float32)
+    assert not (PtrDType(dtypes.float32) != dtypes.float32)
+    assert PtrDType(dtypes.float32) == PtrDType(dtypes.float32)
+    assert not (PtrDType(dtypes.float32) != PtrDType(dtypes.float32))
     #assert PtrDType(dtypes.float32) != dtypes.float32
   def test_strs(self):
     if PtrDType is None: raise unittest.SkipTest("no PtrDType support")
     self.assertEqual(str(dtypes.imagef((1,2,4))), "dtypes.imagef((1, 2, 4))")
     self.assertEqual(str(PtrDType(dtypes.float32)), "ptr.dtypes.float")
 
 class TestHelpers(unittest.TestCase):
   signed_ints = (dtypes.int8, dtypes.int16, dtypes.int32, dtypes.int64)
   uints = (dtypes.uint8, dtypes.uint16, dtypes.uint32, dtypes.uint64)
   floats = (dtypes.float16, dtypes.float32, dtypes.float64)
 
-  @given(st.sampled_from(signed_ints+uints), st.integers(min_value=1, max_value=8))
+  @given(strat.sampled_from(signed_ints+uints), strat.integers(min_value=1, max_value=8))
   def test_is_int(self, dtype, amt):
     assert dtypes.is_int(dtype.vec(amt) if amt > 1 else dtype)
     assert not dtypes.is_float(dtype.vec(amt) if amt > 1 else dtype)
 
-  @given(st.sampled_from(uints), st.integers(min_value=1, max_value=8))
+  @given(strat.sampled_from(uints), strat.integers(min_value=1, max_value=8))
   def test_is_unsigned_uints(self, dtype, amt):
     assert dtypes.is_unsigned(dtype.vec(amt) if amt > 1 else dtype)
 
-  @given(st.sampled_from(signed_ints), st.integers(min_value=1, max_value=8))
+  @given(strat.sampled_from(signed_ints), strat.integers(min_value=1, max_value=8))
   def test_is_unsigned_signed_ints(self, dtype, amt):
     assert not dtypes.is_unsigned(dtype.vec(amt) if amt > 1 else dtype)
 
-  @given(st.sampled_from(floats), st.integers(min_value=1, max_value=8))
+  @given(strat.sampled_from(floats), strat.integers(min_value=1, max_value=8))
   def test_is_float(self, dtype, amt):
     assert dtypes.is_float(dtype.vec(amt) if amt > 1 else dtype)
     assert not dtypes.is_int(dtype.vec(amt) if amt > 1 else dtype)
     assert not dtypes.is_unsigned(dtype.vec(amt) if amt > 1 else dtype)
 
   def test_bf16_is_float(self):
     assert dtypes.is_float(dtypes.bfloat16)
 
-  @given(st.sampled_from([d for d in DTYPES_DICT.values() if dtypes.is_float(d) or dtypes.is_int(d)]), st.integers(min_value=2, max_value=8))
+  @given(strat.sampled_from([d for d in DTYPES_DICT.values() if dtypes.is_float(d) or dtypes.is_int(d)]), strat.integers(min_value=2, max_value=8))
   def test_scalar(self, dtype, amt):
     assert dtype.vec(amt).scalar() == dtype
 
 class TestTypeSpec(unittest.TestCase):
   def setUp(self):
     self.old_default_int, self.old_default_float = dtypes.default_int, dtypes.default_float
   def tearDown(self):
     dtypes.default_int, dtypes.default_float = self.old_default_int, self.old_default_float
 
   def test_set_dtype_default(self):
-    dtypes.default_int = dtypes.int16
-    assert dtypes.default_int == dtypes.int16
-    dtypes.default_int = dtypes.int64
-    assert dtypes.default_int == dtypes.int64
-    dtypes.default_int = dtypes.int32
-    assert dtypes.default_int == dtypes.int32
-    dtypes.default_float = dtypes.float16
-    assert dtypes.default_float == dtypes.float16
-    dtypes.default_float = dtypes.float64
-    assert dtypes.default_float == dtypes.float64
+    for default_int in [dtypes.int8, dtypes.int16, dtypes.int32, dtypes.int64]:
+      dtypes.default_int = default_int
+      assert dtypes.default_int == default_int
+
+    for default_float in [dtypes.float16, dtypes.bfloat16, dtypes.float32, dtypes.float64]:
+      dtypes.default_float = default_float
+      assert dtypes.default_float == default_float
+
+  def test_env_set_default_float(self):
+    # check default
+    subprocess.run(['python3 -c "from tinygrad import dtypes; assert dtypes.default_float == dtypes.float"'],
+                    shell=True, check=True)
+    # check change
+    subprocess.run(['DEFAULT_FLOAT=HALF python3 -c "from tinygrad import dtypes; assert dtypes.default_float == dtypes.half"'],
+                    shell=True, check=True)
+    # check invalid
+    with self.assertRaises(subprocess.CalledProcessError):
+      subprocess.run(['DEFAULT_FLOAT=INT32 python3 -c "from tinygrad import dtypes"'],
+                      shell=True, check=True)
+
+    with self.assertRaises(subprocess.CalledProcessError):
+      subprocess.run(['DEFAULT_FLOAT=TYPO python3 -c "from tinygrad import dtypes"'],
+                      shell=True, check=True)
 
-  @given(st.sampled_from([dtypes.int8,dtypes.int16,dtypes.int32,dtypes.int64]), st.sampled_from([dtypes.float16,dtypes.float32,dtypes.float64]))
+  @given(strat.sampled_from(dtype_ints), strat.sampled_from(dtype_floats))
   def test_creation(self, default_int, default_float):
     dtypes.default_int, dtypes.default_float = default_int, default_float
-    assert Tensor(True).dtype == dtypes.bool
-    assert Tensor(None).dtype == dtypes.default_float
-    assert Tensor(2).dtype == dtypes.default_int
-    assert Tensor(2.34).dtype == dtypes.default_float
-    assert Tensor([]).dtype == dtypes.default_float
-    assert Tensor([1]).dtype == dtypes.default_int
-    assert Tensor([1.1]).dtype == dtypes.default_float
-    assert Tensor([0,1], dtype=dtypes.bfloat16).dtype == dtypes.bfloat16
-
-    assert Tensor.eye(0).dtype == dtypes.default_float
-    assert Tensor.eye(3).dtype == dtypes.default_float
-    assert Tensor.eye(3, dtype=dtypes.float16).dtype == dtypes.float16
-    assert Tensor.eye(3, dtype=dtypes.int64).dtype == dtypes.int64
-
+    _assert_eq(Tensor(True), dtypes.bool, True)
+    _assert_eq(Tensor(None), dtypes.default_float, [])
+    _assert_eq(Tensor(2), dtypes.default_int, 2)
+    _assert_eq(Tensor(2.34), dtypes.default_float, 2.34)
+    _assert_eq(Tensor([]), dtypes.default_float, [])
+    _assert_eq(Tensor([1]), dtypes.default_int, [1])
+    _assert_eq(Tensor([1.1]), dtypes.default_float, [1.1])
+
+    _assert_eq(Tensor.eye(0), dtypes.default_float, np.eye(0))
+    _assert_eq(Tensor.eye(3), dtypes.default_float, np.eye(3))
+    _assert_eq(Tensor.eye(3, dtype=dtypes.int64), dtypes.int64, np.eye(3))
+    if is_dtype_supported(dtypes.float16):
+      _assert_eq(Tensor.eye(3, dtype=dtypes.float16), dtypes.float16, np.eye(3))
 
-  @given(st.sampled_from([dtypes.int8,dtypes.int16,dtypes.int32,dtypes.int64]), st.sampled_from([dtypes.float16,dtypes.float32,dtypes.float64]))
+  @given(strat.sampled_from(dtype_ints), strat.sampled_from(dtype_floats))
   def test_full(self, default_int, default_float):
     dtypes.default_int, dtypes.default_float = default_int, default_float
 
-    assert Tensor.ones([2,3]).dtype == dtypes.default_float
-    assert Tensor.zeros([2,3]).dtype == dtypes.default_float
-    assert Tensor.full([2,3], 3.3).dtype == dtypes.default_float
-    assert Tensor.full([2,3], 3).dtype == dtypes.default_int
-    assert Tensor.full([2,3], True).dtype == dtypes.bool
-
-    assert Tensor.zeros(3, 3).dtype == dtypes.default_float
-    assert Tensor.zeros(3, 3, dtype=dtypes.float16).dtype == dtypes.float16
-    assert Tensor.zeros(3, 3, dtype=dtypes.int64).dtype == dtypes.int64
-
-    assert Tensor.ones(3, 3).dtype == dtypes.default_float
-    assert Tensor.ones(3, 3, dtype=dtypes.float16).dtype == dtypes.float16
-    assert Tensor.ones(3, 3, dtype=dtypes.int64).dtype == dtypes.int64
-
-    assert Tensor.full((3, 3), 3).dtype == dtypes.default_int
-    assert Tensor.full((3, 3), 3.0).dtype == dtypes.default_float
-    assert Tensor.full((3, 3), 3, dtype=dtypes.float16).dtype == dtypes.float16
-    assert Tensor.full((3, 3), 3, dtype=dtypes.int64).dtype == dtypes.int64
-
-  def test_reduce_0d_default(self):
-    assert Tensor.ones([2,3,0]).sum(2).dtype ==  dtypes.default_float
-    # assert Tensor.ones([2,3,0], dtype=dtypes.int).sum(2).dtype == dtypes.int  # requires reduceop acc fix
+    _assert_eq(Tensor.zeros((2, 3)), dtypes.default_float, np.zeros((2, 3)))
+    _assert_eq(Tensor.zeros((2, 3), dtype=dtypes.int64), dtypes.int64, np.zeros((2, 3)))
+    if is_dtype_supported(dtypes.float16):
+      _assert_eq(Tensor.zeros((2, 3), dtype=dtypes.float16), dtypes.float16, np.zeros((2, 3)))
+
+    _assert_eq(Tensor.ones((2, 3)), dtypes.default_float, np.ones((2, 3)))
+    _assert_eq(Tensor.ones((2, 3), dtype=dtypes.int64), dtypes.int64, np.ones((2, 3)))
+    if is_dtype_supported(dtypes.float16):
+      _assert_eq(Tensor.ones((2, 3), dtype=dtypes.float16), dtypes.float16, np.ones((2, 3)))
+
+    _assert_eq(Tensor.full((2, 3), 3.0), dtypes.default_float, np.full((2, 3), 3.0))
+    _assert_eq(Tensor.full((2, 3), 3), dtypes.default_int, np.full((2, 3), 3))
+    _assert_eq(Tensor.full((2, 3), True), dtypes.bool, np.full((2, 3), True))
+    _assert_eq(Tensor.full((2, 3), 3, dtype=dtypes.int64), dtypes.int64, np.full((2, 3), 3))
+    _assert_eq(Tensor.full((2, 3), 3.0, dtype=dtypes.int64), dtypes.int64, np.full((2, 3), 3))
+    if is_dtype_supported(dtypes.float16):
+      _assert_eq(Tensor.full((2, 3), 3, dtype=dtypes.float16), dtypes.float16, np.full((2, 3), 3))
+      _assert_eq(Tensor.full((2, 3), 3.0, dtype=dtypes.float16), dtypes.float16, np.full((2, 3), 3))
+
+  @given(strat.sampled_from(dtype_ints), strat.sampled_from(dtype_floats))
+  def test_reduce_0d_default(self, default_int, default_float):
+    dtypes.default_int, dtypes.default_float = default_int, default_float
+    _assert_eq(Tensor.ones((2,3,0)).sum(2), dtypes.default_float, np.zeros((2, 3)))
+    # TODO: what should this one be?
+    # _assert_eq(Tensor.ones((2,3,0), dtype=dtypes.default_int).sum(2), dtypes.default_int, np.zeros((2, 3)))
+    _assert_eq(Tensor.ones((2,3,0), dtype=dtypes.int32).sum(2), dtypes.int32, np.zeros((2, 3)))
 
-  @given(st.sampled_from([dtypes.int8,dtypes.int16,dtypes.int32,dtypes.int64]), st.sampled_from([dtypes.float16,dtypes.float32,dtypes.float64]))
+  @given(strat.sampled_from(dtype_ints), strat.sampled_from(dtype_floats))
   def test_arange(self, default_int, default_float):
     dtypes.default_int, dtypes.default_float = default_int, default_float
 
-    assert Tensor.arange(5).dtype == dtypes.default_int
-    assert Tensor.arange(5.0).dtype == dtypes.default_float
-    assert Tensor.arange(5, dtype=dtypes.int16).dtype == dtypes.int16
-    assert Tensor.arange(5, dtype=dtypes.int64).dtype == dtypes.int64
-    assert Tensor.arange(5, dtype=dtypes.float16).dtype == dtypes.float16
-    assert Tensor.arange(3, 9, 0.7).dtype == dtypes.default_float
-    assert Tensor.arange(3, 8.5, 3).dtype == dtypes.default_float
+    _assert_eq(Tensor.arange(5), dtypes.default_int, np.arange(5))
+    _assert_eq(Tensor.arange(120), dtypes.default_int, np.arange(120))
+    _assert_eq(Tensor.arange(5.0), dtypes.default_float, np.arange(5))
+    _assert_eq(Tensor.arange(5, dtype=dtypes.int16), dtypes.int16, np.arange(5))
+    _assert_eq(Tensor.arange(5, dtype=dtypes.int64), dtypes.int64, np.arange(5))
+    if is_dtype_supported(dtypes.float16):
+      _assert_eq(Tensor.arange(5, dtype=dtypes.float16), dtypes.float16, np.arange(5))
+    _assert_eq(Tensor.arange(3, 9, 0.7), dtypes.default_float, np.arange(3, 9, 0.7))
+    _assert_eq(Tensor.arange(3, 8.5, 3), dtypes.default_float, np.arange(3, 8.5, 3))
 
-  @unittest.skipIf(Device.DEFAULT == "WEBGPU", "WEBGPU doesn't follow the bool ops spec")
-  @given(st.sampled_from(core_dtypes), st.sampled_from([operator.gt, operator.ge, operator.le, operator.lt, operator.eq, operator.ne]))
+  @given(strat.sampled_from(core_dtypes), strat.sampled_from([operator.gt, operator.ge, operator.le, operator.lt, operator.eq, operator.ne]))
   def test_bool_ops(self, dtype, op):
     assert op(Tensor.rand(4, 4, dtype=dtype), Tensor.rand(4, 4, dtype=dtype)).dtype == dtypes.bool
 
-  @given(st.sampled_from(core_dtypes),
-         st.sampled_from([dtypes.int8,dtypes.int16,dtypes.int32,dtypes.int64]), st.sampled_from([dtypes.float16,dtypes.float32,dtypes.float64]))
+  @given(strat.sampled_from(core_dtypes), strat.sampled_from(dtype_ints), strat.sampled_from(dtype_floats))
   def test_functions_return_index(self, dtype, default_int, default_float):
     dtypes.default_int, dtypes.default_float = default_int, default_float
-    assert Tensor([0, 1], dtype=dtype).argmax().dtype == dtypes.default_int
-    assert Tensor([0, 1], dtype=dtype).argmin().dtype == dtypes.default_int
-    assert Tensor([0, 1], dtype=dtype).multinomial().dtype == dtypes.default_int
+    assert Tensor([0, 1], dtype=dtype).argmax().dtype == dtypes.int32
+    assert Tensor([0, 1], dtype=dtype).argmin().dtype == dtypes.int32
+    assert Tensor([0, 1], dtype=dtype).multinomial().dtype == dtypes.int32
+
+  @given(strat.sampled_from(core_dtypes), strat.sampled_from(dtype_ints))
+  def test_tensor_indexing_returns_same_dtype(self, data_dtype, indices_dtype):
+    X_data =  Tensor.rand(60000, 1, 28, 28, dtype=data_dtype)
+    indices =  Tensor.randint(512, high=X_data.shape[0]).cast(indices_dtype)
+    assert X_data[indices].dtype == X_data.dtype
+
+  @given(strat.sampled_from(core_dtypes), strat.sampled_from(dtype_ints))
+  def test_gather_returns_same_dtype(self, data_dtype, indices_dtype):
+    X_data = Tensor([[1, 0], [0, 1]], dtype=data_dtype)
+    indices = Tensor([[0, 0], [1, 0]], dtype=indices_dtype)
+    assert X_data.gather(0, indices).dtype == X_data.dtype
+    assert X_data.gather(1, indices).dtype == X_data.dtype
 
 class TestTypePromotion(unittest.TestCase):
-  @given(st.sampled_from(core_dtypes))
+  @given(strat.sampled_from(core_dtypes))
   def test_self_promo_to_self(self, dtype):
     assert least_upper_dtype(dtype) == dtype
     assert least_upper_dtype(dtype, dtype) == dtype
     assert least_upper_dtype(dtype, dtype, dtype) == dtype
 
-  @given(st.sampled_from(core_dtypes), st.sampled_from(core_dtypes))
+  @given(strat.sampled_from(core_dtypes), strat.sampled_from(core_dtypes))
   def test_promo_resulted_higher_than_inputs(self, dtype1, dtype2):
     result = least_upper_dtype(dtype1, dtype2)
     assert result >= dtype1 and result >= dtype2
 
   def test_dtype_promo(self):
     assert least_upper_dtype(dtypes.bool, dtypes.int8) == dtypes.int8
     assert least_upper_dtype(dtypes.int8, dtypes.uint8) == dtypes.int16
@@ -360,26 +472,25 @@
     assert least_upper_dtype(dtypes.float32, dtypes.float64) == dtypes.float64
 
     assert least_upper_dtype(dtypes.bool, dtypes.float32) == dtypes.float32
     assert least_upper_dtype(dtypes.bool, dtypes.float64) == dtypes.float64
     assert least_upper_dtype(dtypes.float16, dtypes.int64) == dtypes.float16
     assert least_upper_dtype(dtypes.float16, dtypes.uint64) == dtypes.float16
 
-  @given(st.sampled_from(floats))
+  @given(strat.sampled_from(dtype_floats))
   def test_float_to_float(self, dt):
     assert least_upper_float(dt) == dt
 
 class TestAutoCastType(unittest.TestCase):
   def setUp(self):
     self.old_default_int, self.old_default_float = dtypes.default_int, dtypes.default_float
   def tearDown(self):
     dtypes.default_int, dtypes.default_float = self.old_default_int, self.old_default_float
 
-  @given(st.sampled_from([d for d in DTYPES_DICT.values() if dtypes.is_int(d) and is_dtype_supported(d)]))
-  @settings(deadline=None)
+  @given(strat.sampled_from([d for d in DTYPES_DICT.values() if dtypes.is_int(d) and is_dtype_supported(d)]))
   def test_int_to_float_unary_func(self, dtype):
     for func in [
       lambda t: t.exp(),
       lambda t: t.exp2(),
       lambda t: t.log(),
       lambda t: t.log2(),
       lambda t: t.sqrt(),
@@ -389,79 +500,175 @@
       lambda t: t.tan(),
       lambda t: t.sigmoid(),
     ]:
       a = [2, 3, 4]
       # float16 can have larger precision errors
       np.testing.assert_allclose(func(Tensor(a, dtype=dtype)).numpy(), func(torch.tensor(a)), rtol=1e-3, atol=1e-3)
 
-  @given(st.sampled_from([dtypes.float16,dtypes.float32,dtypes.float64]))
-  def test_broadcast_float(self, default_float):
-    dtypes.default_float = default_float
-    assert (Tensor.rand(4, 4, dtype=dtypes.bool) + 2.3).dtype == dtypes.default_float
-    assert (Tensor.rand(4, 4, dtype=dtypes.int) + 2.3).dtype == dtypes.default_float
-    assert (Tensor.rand(4, 4, dtype=dtypes.int8) + 2.3).dtype == dtypes.default_float
-    assert (Tensor.rand(4, 4, dtype=dtypes.uint64) + 2.3).dtype == dtypes.default_float
-    assert (Tensor.rand(4, 4, dtype=dtypes.float16) + 2.3).dtype == dtypes.float16
-    assert (Tensor.rand(4, 4, dtype=dtypes.bfloat16) + 2.3).dtype == dtypes.bfloat16
-    assert (Tensor.rand(4, 4, dtype=dtypes.float32) + 2.3).dtype == dtypes.float32
-    assert (Tensor.rand(4, 4, dtype=dtypes.float64) + 2.3).dtype == dtypes.float64
-
-  @given(st.sampled_from([dtypes.int8,dtypes.int16,dtypes.int32,dtypes.int64]))
-  def test_broadcast_int(self, default_int):
-    dtypes.default_int = default_int
-    assert (Tensor.rand(4, 4, dtype=dtypes.bool) + 2).dtype == dtypes.default_int
-    assert (Tensor.rand(4, 4, dtype=dtypes.int) + 2).dtype == dtypes.int
-    assert (Tensor.rand(4, 4, dtype=dtypes.int8) + 2).dtype == dtypes.int8
-    assert (Tensor.rand(4, 4, dtype=dtypes.uint64) + 2).dtype == dtypes.uint64
-    assert (Tensor.rand(4, 4, dtype=dtypes.float16) + 2).dtype == dtypes.float16
-    assert (Tensor.rand(4, 4, dtype=dtypes.bfloat16) + 2).dtype == dtypes.bfloat16
-    assert (Tensor.rand(4, 4, dtype=dtypes.float32) + 2).dtype == dtypes.float32
-    assert (Tensor.rand(4, 4, dtype=dtypes.float64) + 2).dtype == dtypes.float64
-
-  def test_broadcast_bool(self):
-    if Device.DEFAULT != "WEBGPU":
-      assert (Tensor([0, 1], dtype=dtypes.bool) + True).dtype == dtypes.bool
-    assert (Tensor([0, 1], dtype=dtypes.int) + True).dtype == dtypes.int32
-    assert (Tensor([0, 1], dtype=dtypes.int8) + True).dtype == dtypes.int8
-    assert (Tensor([0, 1], dtype=dtypes.uint64) + True).dtype == dtypes.uint64
-    assert (Tensor([0, 1], dtype=dtypes.float16) + True).dtype == dtypes.float16
-    assert (Tensor([0, 1], dtype=dtypes.bfloat16) + True).dtype == dtypes.bfloat16
-    assert (Tensor([0, 1], dtype=dtypes.float32) + True).dtype == dtypes.float32
-    assert (Tensor([0, 1], dtype=dtypes.float64) + True).dtype == dtypes.float64
+  @given(strat.sampled_from(core_dtypes))
+  def test_broadcast_scalar(self, dt):
+    assert (Tensor.rand(4, 4, dtype=dt) + 2.3).dtype == (dt if dtypes.is_float(dt) else dtypes.default_float)
+    assert (Tensor.rand(4, 4, dtype=dt) + 2).dtype == (dt if dtypes.is_float(dt) or dtypes.is_int(dt) else dtypes.default_int)
+    if Device.DEFAULT != "WEBGPU" and dt != dtypes.bool:
+      assert (Tensor.rand(4, 4, dtype=dt) + True).dtype == dt
 
   def test_sum(self):
     assert (Tensor([0, 1], dtype=dtypes.bool)).sum().dtype == dtypes.int32
     assert (Tensor([0, 1], dtype=dtypes.int8)).sum().dtype == dtypes.int32
     assert (Tensor([0, 1], dtype=dtypes.int16)).sum().dtype == dtypes.int32
     assert (Tensor([0, 1], dtype=dtypes.int32)).sum().dtype == dtypes.int32
     assert (Tensor([0, 1], dtype=dtypes.int64)).sum().dtype == dtypes.int64
     assert (Tensor([0, 1], dtype=dtypes.uint8)).sum().dtype == dtypes.uint32
     assert (Tensor([0, 1], dtype=dtypes.uint16)).sum().dtype == dtypes.uint32
     assert (Tensor([0, 1], dtype=dtypes.uint32)).sum().dtype == dtypes.uint32
     assert (Tensor([0, 1], dtype=dtypes.uint64)).sum().dtype == dtypes.uint64
     assert (Tensor([0, 1], dtype=dtypes.float16)).sum().dtype == dtypes.float16
-    assert (Tensor([0, 1], dtype=dtypes.bfloat16)).sum().dtype == dtypes.bfloat16
+    #assert (Tensor([0, 1], dtype=dtypes.bfloat16)).sum().dtype == dtypes.bfloat16
     assert (Tensor([0, 1], dtype=dtypes.float32)).sum().dtype == dtypes.float32
     assert (Tensor([0, 1], dtype=dtypes.float64)).sum().dtype == dtypes.float64
 
+  def test_mean(self):
+    assert (Tensor([0, 1], dtype=dtypes.bool)).mean().dtype == dtypes.float32
+    assert (Tensor([0, 1], dtype=dtypes.int8)).mean().dtype == dtypes.float32
+    assert (Tensor([0, 1], dtype=dtypes.int16)).mean().dtype == dtypes.float32
+    assert (Tensor([0, 1], dtype=dtypes.int32)).mean().dtype == dtypes.float32
+    assert (Tensor([0, 1], dtype=dtypes.int64)).mean().dtype == dtypes.float32
+    assert (Tensor([0, 1], dtype=dtypes.uint8)).mean().dtype == dtypes.float32
+    assert (Tensor([0, 1], dtype=dtypes.uint16)).mean().dtype == dtypes.float32
+    assert (Tensor([0, 1], dtype=dtypes.uint32)).mean().dtype == dtypes.float32
+    assert (Tensor([0, 1], dtype=dtypes.uint64)).mean().dtype == dtypes.float32
+    assert (Tensor([0, 1], dtype=dtypes.float16)).mean().dtype == dtypes.float16
+    #assert (Tensor([0, 1], dtype=dtypes.bfloat16)).mean().dtype == dtypes.bfloat16
+    assert (Tensor([0, 1], dtype=dtypes.float32)).mean().dtype == dtypes.float32
+    assert (Tensor([0, 1], dtype=dtypes.float64)).mean().dtype == dtypes.float64
+
   def test_cumsum(self):
     assert (Tensor([0, 1], dtype=dtypes.bool)).cumsum(0).dtype == dtypes.int32
     assert (Tensor([0, 1], dtype=dtypes.int8)).cumsum(0).dtype == dtypes.int32
     assert (Tensor([0, 1], dtype=dtypes.int16)).cumsum(0).dtype == dtypes.int32
     assert (Tensor([0, 1], dtype=dtypes.int32)).cumsum(0).dtype == dtypes.int32
     assert (Tensor([0, 1], dtype=dtypes.int64)).cumsum(0).dtype == dtypes.int64
     assert (Tensor([0, 1], dtype=dtypes.uint8)).cumsum(0).dtype == dtypes.uint32
     assert (Tensor([0, 1], dtype=dtypes.uint16)).cumsum(0).dtype == dtypes.uint32
     assert (Tensor([0, 1], dtype=dtypes.uint32)).cumsum(0).dtype == dtypes.uint32
     assert (Tensor([0, 1], dtype=dtypes.uint64)).cumsum(0).dtype == dtypes.uint64
     assert (Tensor([0, 1], dtype=dtypes.float16)).cumsum(0).dtype == dtypes.float16
-    assert (Tensor([0, 1], dtype=dtypes.bfloat16)).cumsum(0).dtype == dtypes.bfloat16
+    #assert (Tensor([0, 1], dtype=dtypes.bfloat16)).cumsum(0).dtype == dtypes.bfloat16
     assert (Tensor([0, 1], dtype=dtypes.float32)).cumsum(0).dtype == dtypes.float32
     assert (Tensor([0, 1], dtype=dtypes.float64)).cumsum(0).dtype == dtypes.float64
 
-  @given(st.sampled_from(core_dtypes), st.sampled_from(core_dtypes))
-  @settings(deadline=None)
+  @given(strat.sampled_from(core_dtypes), strat.sampled_from(core_dtypes))
   def test_matmul(self, dt1, dt2):
     assert (Tensor([0, 1], dtype=dt1) @ Tensor([0, 1], dtype=dt2)).dtype == least_upper_dtype(dt1, dt2)
 
+  @staticmethod
+  def check_where_alternate_input_other(input_, other, data_type):
+    assert (Tensor([True, False]).where(input_, other)).dtype == data_type
+    assert (Tensor([True, False]).where(other, input_)).dtype == data_type
+
+  @given(strat.sampled_from(core_dtypes), strat.sampled_from(core_dtypes))
+  def test_where_no_scalar(self, dt1, dt2):
+    self.check_where_alternate_input_other(Tensor(2, dtype=dt1), Tensor(3, dtype=dt2), least_upper_dtype(dt1, dt2))
+
+  @given(strat.sampled_from(core_dtypes))
+  def test_where_one_scalar(self, dt):
+    t = Tensor(2, dtype=dt)
+    self.check_where_alternate_input_other(t, 3.2, (dt if dtypes.is_float(dt) else dtypes.default_float))
+    self.check_where_alternate_input_other(t, 3, (dt if dtypes.is_float(dt) or dtypes.is_int(dt) else dtypes.default_int))
+    self.check_where_alternate_input_other(t, True, dt)
+
+  def test_where_two_scalars(self):
+    self.check_where_alternate_input_other(3.1, 3.2, dtypes.default_float)
+    self.check_where_alternate_input_other(3.1, 3, dtypes.default_float)
+    self.check_where_alternate_input_other(3.1, True, dtypes.default_float)
+    self.check_where_alternate_input_other(3, 2, dtypes.default_int)
+    self.check_where_alternate_input_other(3, True, dtypes.default_int)
+    self.check_where_alternate_input_other(False, True, dtypes.bool)
+
+  @given(strat.sampled_from(core_dtypes), strat.sampled_from(core_dtypes))
+  def test_maximum(self, dt1, dt2):
+    assert Tensor([0, 1, 2], dtype=dt1).maximum(Tensor([2, 0, 5], dtype=dt2)).dtype == least_upper_dtype(dt1, dt2)
+
+  @given(strat.sampled_from(core_dtypes))
+  def test_maximum_const(self, dt):
+    assert Tensor([1, 2], dtype=dt).maximum(3.1).dtype == (dt if dtypes.is_float(dt) else dtypes.default_float)
+    assert Tensor([1, 2], dtype=dt).maximum(3).dtype == (dt if dtypes.is_float(dt) or dtypes.is_int(dt) else dtypes.default_int)
+    assert Tensor([1, 2], dtype=dt).maximum(True).dtype == dt
+
+  def test_div(self):
+    assert (Tensor([1, 2], dtype=dtypes.int32) / Tensor([2, 2], dtype=dtypes.int32)).dtype == dtypes.default_float
+    assert (Tensor([1, 2], dtype=dtypes.int16) / Tensor([2, 2], dtype=dtypes.int32)).dtype == dtypes.default_float
+    assert (Tensor([1, 2], dtype=dtypes.float32) / Tensor([2, 2], dtype=dtypes.float16)).dtype == dtypes.float32
+    assert (Tensor([1, 2], dtype=dtypes.int32) / Tensor([2, 2], dtype=dtypes.float16)).dtype == dtypes.float16
+
+  def test_div_const(self):
+    assert (Tensor([1, 2], dtype=dtypes.int32) / 2).dtype == dtypes.default_float
+    assert (Tensor([1, 2], dtype=dtypes.int32) / 2.0).dtype == dtypes.default_float
+    assert (Tensor([1, 2], dtype=dtypes.float16) / 2).dtype == dtypes.float16
+    assert (Tensor([1, 2], dtype=dtypes.float16) / 2.0).dtype == dtypes.float16
+
+  def test_gradient_dtype(self):
+    old_default_float = dtypes.default_float
+
+    for default_dtype in [dtypes.float16, dtypes.bfloat16, dtypes.float32, dtypes.float64]:
+      if not is_dtype_supported(default_dtype): continue
+      dtypes.default_float = default_dtype
+      for dtype in [dtypes.float16, dtypes.bfloat16, dtypes.float32, dtypes.float64]:
+        if not is_dtype_supported(dtype): continue
+        if DEBUG >= 2:
+          print(f"testing {default_dtype=}, {dtype=}")
+        a = Tensor([1, 2, 3], dtype=dtype, requires_grad=True)
+        b = (a * 5).sum()
+        b.backward()  # if there is dtype mismatch, lazy should assert
+        assert a.grad.dtype == a.dtype
+        np.testing.assert_allclose(a.grad.numpy(), [5, 5, 5])
+
+    dtypes.default_float = old_default_float
+
+  @unittest.skipUnless(is_dtype_supported(dtypes.half), "need half")
+  def test_backward_sum_acc_dtype(self):
+    # test acc of sum in the backward is upcasted to float
+    t = Tensor([5, -5], dtype=dtypes.half, requires_grad=True)
+    t.reshape(2, 1).expand(2, 10001).max().backward()
+    np.testing.assert_allclose(t.grad.numpy(), [1, 0])
+
+  @unittest.skipIf(Device.DEFAULT=="PYTHON", "very slow")
+  @unittest.skipUnless(is_dtype_supported(dtypes.half), "need half")
+  def test_mean_half_precision_underflow(self):
+    N = 10000
+    x = 0.001
+    t = Tensor([[x]], dtype=dtypes.half, requires_grad=True).expand(N, N).contiguous()
+    np.testing.assert_allclose(t.mean(axis=1).numpy(), np.array([x] * N, dtype=np.float16), rtol=1e-3)
+
+  @unittest.skipUnless(is_dtype_supported(dtypes.half), "need half")
+  def test_mean_half_precision_overflow(self):
+    N = 256
+    t = Tensor([60000] * N*N, dtype=dtypes.half, requires_grad=True).reshape(N, N)
+    np.testing.assert_allclose(t.mean().numpy(), 60000)
+    t.square().mean().backward()
+    np.testing.assert_allclose(t.grad.numpy().flatten(), [60000 * 2 / (N*N)] * N*N)
+
+class TestImplicitFunctionTypeChange(unittest.TestCase):
+  def test_functions(self):
+    result = []
+    for func in [
+      lambda t: t.exp(),
+      lambda t: t.exp2(),
+      lambda t: t.log(),
+      lambda t: t.log2(),
+      lambda t: t.sqrt(),
+      lambda t: t.sin(),
+    ]:
+      t = func(Tensor([4.0, 3.0])).max() == func(Tensor([4.0, 3.0]))
+      result.append(t.numpy().sum())
+    assert all(result)
+
+class TestTensorMethod(unittest.TestCase):
+  @given(strat.sampled_from(core_dtypes))
+  def test_abs_diff(self, dt):
+    if dt == dtypes.bool or not is_dtype_supported(dt): return
+    a, b = Tensor([2], dtype=dt), Tensor([1], dtype=dt)
+    ret = (a - b).abs()
+    np.testing.assert_allclose(ret.numpy(), np.abs(a.numpy()-b.numpy()))
+
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `tinygrad-0.8.0/test/test_fusion_op.py` & `tinygrad-0.9.0/test/test_fusion_op.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import unittest
 import time
 import numpy as np
 from tinygrad import Tensor, dtypes
-from tinygrad.device import InterpretedASTRunner
-from tinygrad.lazy import create_schedule
-from tinygrad.realize import run_schedule, lower_schedule_item
+from tinygrad.engine.schedule import create_schedule
+from tinygrad.engine.realize import lower_schedule_item, run_schedule
 
 class TestFusionOp(unittest.TestCase):
   def test_contiguous_add(self):
     def test(contig=False):
       bt = Tensor(np.arange(16), dtype=dtypes.float32).reshape(4,4)
       x = bt.permute(1,0)
       if contig: x = x.contiguous()
@@ -16,25 +15,25 @@
     assert test() == test(True)
 
   def test_expand_fuse(self):
     bt = Tensor(np.ones((10, 1)), dtype=dtypes.float32)
     out = (bt*2).expand(10,10).sum(1)
     sched = create_schedule([out.lazydata], None)
     run_schedule(sched)
-    outd = out.data().tolist()
+    outd = out.tolist()
     assert all(x == 20.0 for x in outd)
 
   def test_recursive_add(self):
     st = time.perf_counter()
     a = Tensor([1,2,3,4])
     for _ in range(24): a = a + a
     sched = create_schedule([a.lazydata], None)
-    ji = lower_schedule_item(sched[-1])
+    ei = lower_schedule_item(sched[-1])
     self.assertLess(time.perf_counter()-st, 1.0)
-    assert isinstance(ji, InterpretedASTRunner) or len(ji.prg) < 5000
+    assert len(ei.prg.p.src.splitlines()) < 250
 
   def test_recursive_add_cmp(self):
     st = time.perf_counter()
     a = Tensor([1,2,3,4])
     for _ in range(24): a = a + a
     sched1 = create_schedule([a.lazydata], None)
     b = Tensor([1,2,3,4])
```

### Comparing `tinygrad-0.8.0/test/test_gc.py` & `tinygrad-0.9.0/test/test_gc.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 
 def tensors_allocated():
   return sum([isinstance(x, Tensor) for x in gc.get_objects()])
 
 class TestGC(unittest.TestCase):
 
   def test_gc(self):
-    a = Tensor.zeros(4, 4, requires_grad=True)
+    a = Tensor.rand(4, 4, requires_grad=True)
     b = Tensor.zeros(4, 4, requires_grad=True)
     (a*b).mean().backward()
     assert(tensors_allocated() > 0)
     del a,b
-    assert(tensors_allocated() == 0)
+    assert(tensors_allocated() == 1) # one for Tensor._rng_counter
 
   def test_gc_complex(self):
     a = Tensor(np.zeros((4, 4), dtype=np.float32), requires_grad=True)
-    b = Tensor(np.zeros((4, 4), dtype=np.float32), requires_grad=True)
-    assert(tensors_allocated() == 2)
+    b = Tensor.rand(4, 4, requires_grad=True)
+    assert(tensors_allocated() == 3)
     (a*b).mean().backward()
-    assert(tensors_allocated() == 4)
+    assert(tensors_allocated() == 5)
     del b
-    assert(tensors_allocated() == 2)
+    assert(tensors_allocated() == 3)
     b = Tensor(np.zeros((4, 4), dtype=np.float32), requires_grad=True)
     print(tensors_allocated())
     (a*b).mean().backward()
     print(tensors_allocated())
-    assert(tensors_allocated() == 4)
+    assert(tensors_allocated() == 5)
     del b
-    assert(tensors_allocated() == 2)
+    assert(tensors_allocated() == 3)
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `tinygrad-0.8.0/test/test_image_dtype.py` & `tinygrad-0.9.0/test/test_image_dtype.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 import numpy as np
 from tinygrad import Device, dtypes, Tensor, Variable
 from tinygrad.dtype import ImageDType
-from tinygrad.features.image import to_image_idx
+from tinygrad.codegen.linearizer import to_image_idx
 
 @unittest.skipIf(Device.DEFAULT != "GPU", "only images on GPU")
 class TestImageDType(unittest.TestCase):
   def test_image_and_back(self):
     data = Tensor.randn(9*27*4).realize()
     tst = data.numpy()
     it = data.cast(dtypes.imagef((9,27,4))).realize()
@@ -34,15 +34,15 @@
     it = Tensor.randn(8).cast(dtypes.imagef((1,2,4))).realize()
     imgv = it.numpy()
     np.testing.assert_equal(np.maximum(imgv[0:3], 0), it[0:3].relu().numpy())
 
   def test_shrink_to_float(self):
     it = Tensor.randn(4, 4).cast(dtypes.imagef((1,4,4))).realize()
     imgv = it.numpy()
-    np.testing.assert_equal(np.maximum(imgv[:, 0], 0), it[:, 0].relu().realize())
+    np.testing.assert_equal(np.maximum(imgv[:, 0], 0), it[:, 0].relu().numpy())
 
   def test_lru_alloc(self):
     data = Tensor.randn(9*27*4).realize()
     it = data.cast(dtypes.imagef((9,27,4))).realize()
     b1 = it.lazydata.base.realized._buf
     del it
     it = data.cast(dtypes.imagef((9,27,4))).realize()
```

### Comparing `tinygrad-0.8.0/test/test_jit.py` & `tinygrad-0.9.0/test/test_jit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,52 @@
 #!/usr/bin/env python
 import unittest, functools
 import numpy as np
 
 from test.helpers import assert_jit_cache_len
 from tinygrad.tensor import Tensor
-from tinygrad.jit import TinyJit
+from tinygrad.engine.jit import TinyJit
 from tinygrad.device import Device
 from tinygrad.helpers import CI
 
+def _simple_test(add, extract=lambda x: x, N=10):
+  for _ in range(5):
+    a = Tensor.randn(N, N)
+    b = Tensor.randn(N, N)
+    c = add(a, b)
+    np.testing.assert_allclose(extract(c).numpy(), a.numpy()+b.numpy(), atol=1e-4, rtol=1e-5)
+  assert_jit_cache_len(add, 1)
+
 class TestJit(unittest.TestCase):
   def test_simple_jit(self):
     @TinyJit
     def add(a, b): return (a+b).realize()
-    for _ in range(5):
-      a = Tensor.randn(10, 10)
-      b = Tensor.randn(10, 10)
-      c = add(a, b)
-      np.testing.assert_allclose(c.numpy(), a.numpy()+b.numpy(), atol=1e-4, rtol=1e-5)
-    assert_jit_cache_len(add, 1)
+    _simple_test(add)
+
+  def test_simple_jit_reset(self):
+    @TinyJit
+    def add(a, b): return (a+b).realize()
+    _simple_test(add)
+    add.reset()
+    _simple_test(add, N=20)
+
+  def test_simple_jit_norealize(self):
+    @TinyJit
+    def add(a, b): return (a+b)
+    _simple_test(add)
+
+  def test_simple_jit_norealize_list(self):
+    @TinyJit
+    def add(a, b): return [a+b]
+    _simple_test(add, extract=lambda x: x[0])
+
+  def test_simple_jit_norealize_dict(self):
+    @TinyJit
+    def add(a, b): return {"billy": a+b}
+    _simple_test(add, extract=lambda x: x["billy"])
 
   def test_jit_multiple_outputs(self):
     @TinyJit
     def f(a, b): return (a+b).realize(), (a-b).realize(), (a*b).realize()
     for _ in range(5):
       a = Tensor.randn(10, 10)
       b = Tensor.randn(10, 10)
@@ -29,15 +54,15 @@
       np.testing.assert_allclose(c.numpy(), a.numpy()+b.numpy(), atol=1e-4, rtol=1e-5)
       np.testing.assert_allclose(d.numpy(), a.numpy()-b.numpy(), atol=1e-4, rtol=1e-5)
       np.testing.assert_allclose(e.numpy(), a.numpy()*b.numpy(), atol=1e-4, rtol=1e-5)
     assert_jit_cache_len(f, 3)
 
   def test_nothing_jitted(self):
     @TinyJit
-    def add(a, b): return a+b
+    def add(a, b): return None
     with self.assertRaises(AssertionError):
       for _ in range(5):
         a = Tensor.randn(10, 10)
         b = Tensor.randn(10, 10)
         add(a, b)
 
   def test_jit_shape_mismatch(self):
@@ -74,14 +99,29 @@
     for _ in range(5):
       a = Tensor.randn(10, 10)
       b = Tensor.randn(10, 10)
       c = add_kwargs(first=a, second=b)
       np.testing.assert_allclose(c.numpy(), a.numpy()+b.numpy(), atol=1e-4, rtol=1e-5)
     assert_jit_cache_len(add_kwargs, 1)
 
+  def test_reorder_kwargs_jit(self):
+    @TinyJit
+    def add_kwargs(first, second): return (first/second).realize()
+    for _ in range(2):
+      a = Tensor.randn(10, 10)
+      b = Tensor.randn(10, 10)
+      c = add_kwargs(second=b, first=a)
+      np.testing.assert_allclose(c.numpy(), a.numpy()/b.numpy(), atol=1e-4, rtol=1e-5)
+    for _ in range(2):
+      a = Tensor.randn(10, 10)
+      b = Tensor.randn(10, 10)
+      c = add_kwargs(first=a, second=b)
+      np.testing.assert_allclose(c.numpy(), a.numpy()/b.numpy(), atol=1e-4, rtol=1e-5)
+    assert_jit_cache_len(add_kwargs, 1)
+
   def test_array_jit(self):
     @TinyJit
     def add_array(a, arr): return (a+arr[0]).realize()
     for i in range(5):
       a = Tensor.randn(10, 10)
       b = Tensor.randn(10, 10)
       a.realize(), b.realize()
@@ -89,14 +129,23 @@
       if i >= 2:
         # should fail once jitted since jit can't handle arrays
         np.testing.assert_allclose(np.any(np.not_equal(c.numpy(),a.numpy()+b.numpy())), True, atol=1e-4, rtol=1e-5)
       else:
         np.testing.assert_allclose(c.numpy(), a.numpy()+b.numpy(), atol=1e-4, rtol=1e-5)
     assert_jit_cache_len(add_array, 1)
 
+  def test_jit_copyin(self):
+    @TinyJit
+    def f(a):
+      return a + Tensor([1,2,3])
+    for _ in range(5):
+      b = Tensor.randn(3)
+      c = f(b)
+      np.testing.assert_allclose(c.numpy(), b.numpy()+[1,2,3], atol=1e-4, rtol=1e-5)
+
   def test_method_jit(self):
     class Fun:
       def __init__(self):
         self.a = Tensor.randn(10, 10)
       @TinyJit
       def __call__(self, b:Tensor) -> Tensor:
         return (self.a+b).realize()
@@ -136,32 +185,32 @@
   def test_jit_random_regen(self):
     def f(a, b):
       rn = Tensor.randn(*a.shape)
       return ((a+b)*rn).realize()
     a = Tensor.randn(10, 10).realize()  # realize these before resetting the random seed
     b = Tensor.randn(10, 10).realize()
 
-    Tensor._seed = 1234
+    Tensor.manual_seed(1234)
     jf = TinyJit(f)
     res = set()
     for _ in range(5):
       o1 = jf(a, b)
       res.add(o1.numpy()[0][0])
     assert len(res) == 5, "All values should be different, rand works in jit."
 
-    Tensor._seed = 1234
+    Tensor.manual_seed(1234)
     jf2 = TinyJit(f)
     res2 = set()
     for _ in range(5):
       o1 = jf2(a, b)
       res2.add(o1.numpy()[0][0])
     assert len(res2) == 5, "All values should be different, rand works in jit."
     assert res == res2, "Jit rand is not reproducible with the same seed"
 
-    Tensor._seed = 3421
+    Tensor.manual_seed(3421)
     jf3 = TinyJit(f)
     res3 = set()
     for _ in range(5):
       o1 = jf3(a, b)
       res3.add(o1.numpy()[0][0])
     assert len(res3) == 5, "All values should be different, rand works in jit."
     assert res3 != res2, "Jit rand is diff with diff seeds"
@@ -184,69 +233,14 @@
     foo(Tensor([7,7,7,7,7]))
     want = [[1., 2., 3., 4., 5.],
             [1., 3., 3., 4., 6.],
             [1., 2., 5., 4., 7.],
             [0., 2., 3., 1., 0.]]
     np.testing.assert_allclose(want, Y)
 
-  def test_jitted_read_assign(self):
-    class Cache:
-      def __init__(self):
-        self.good_cache = Tensor.zeros(1)
-        self.bad_cache = Tensor.zeros(1)
-        self.good_jitted = TinyJit(self.good)
-        self.bad_jitted = TinyJit(self.bad)
-
-      def good(self, y, cache_v=None):
-        if cache_v is not None:
-          self.good_cache.assign(cache_v+1-1).realize()
-        return (self.good_cache + y).realize()  # need + y to provide inputs to JIT
-
-      def bad(self, y, cache_v=None):
-        if cache_v is not None:
-          self.bad_cache.assign(cache_v).realize()
-        return (self.bad_cache + y).realize()
-
-    cache = Cache()
-    np.testing.assert_equal([0], cache.good_cache.numpy())
-    np.testing.assert_equal([0], cache.bad_cache.numpy())
-
-    zero = Tensor([0])
-    one = Tensor([1])
-    two = Tensor([2])
-
-    # save [1] in the caches
-    cache.good(zero, one)
-    cache.bad(zero, one)
-    np.testing.assert_equal([1], cache.good_cache.numpy())
-    np.testing.assert_equal([1], cache.bad_cache.numpy())
-
-    for i in range(5):
-      x = Tensor([i]) # NOTE: if this doesn't change, it just hits the lazybuffer cache
-      cache.good_jitted(x)
-      cache.bad_jitted(x)
-
-    # verify the jitted calls read 1 from the cache
-    np.testing.assert_equal([1], cache.good_jitted(zero).numpy())
-    np.testing.assert_equal([1], cache.bad_jitted(zero).numpy())
-
-    # save [2] in the caches
-    cache.good(zero, two)
-    cache.bad(zero, two)
-    np.testing.assert_equal([2], cache.good_cache)
-    np.testing.assert_equal([2], cache.bad_cache)
-
-    # verify the jitted calls read 2 from the cache
-    np.testing.assert_equal([2], cache.good_jitted(zero).numpy())
-    # but the bad_jitted doesn't!
-    np.testing.assert_equal([1], cache.bad_jitted(zero).numpy())
-
-    assert_jit_cache_len(cache.good_jitted, 1)
-    assert_jit_cache_len(cache.bad_jitted, 1)
-
   def test_jit_buffer_behavior(self):
     @TinyJit
     def foo(x) -> Tensor: return x.sum().realize()
 
     result_1 = foo(Tensor([1] * 2))
     result_2 = foo(Tensor([2] * 2))
     result_3 = foo(Tensor([3] * 2))
@@ -285,19 +279,59 @@
     graph_t = Device[Device.DEFAULT].graph.func if isinstance(Device[Device.DEFAULT].graph, functools.partial) else Device[Device.DEFAULT].graph
     # Checking that 2 graphs are inited.
     assert isinstance(jf.jit_cache[0].prg, graph_t)
     assert isinstance(jf.jit_cache[1].prg, graph_t)
 
   def test_jit_const_inputs(self):
     @TinyJit
-    def f(x,y): return (x+y).realize()
-    for _ in range(5):
-      np.testing.assert_equal(f(Tensor.ones(3), Tensor.zeros(3)).numpy(), np.ones(3))
-
-    @TinyJit
     def g(x,y,z): return (x+y+z).realize()
     for i in range(5):
       np.testing.assert_equal(g(Tensor([i]*3), Tensor.ones(3), Tensor.zeros(3)).numpy(), np.array([i+1]*3))
 
+  @unittest.skipIf(CI and Device.DEFAULT in {"GPU", "CUDA", "METAL", "HSA", "NV", "AMD"}, "no GPU CI")
+  def test_jitted_transfers(self):
+    d0, d1 = f"{Device.DEFAULT}:0", f"{Device.DEFAULT}:1"
+
+    def f(a, b):
+      x = a.to(d1)
+      y = b.to(d1)
+      return x.realize(), y.realize()
+
+    jf = TinyJit(f)
+    for _ in range(5):
+      a = Tensor.randn(10, 10, device=d0).realize()
+      b = Tensor.randn(10, 10, device=d0).realize()
+      xc, yc = jf(a, b)
+      np.testing.assert_allclose(a.numpy(), xc.numpy(), atol=1e-4, rtol=1e-5)
+      np.testing.assert_allclose(b.numpy(), yc.numpy(), atol=1e-4, rtol=1e-5)
+
+
+@unittest.skip("Pending multioutput implementation #3607")
+class TestMultioutputJit(unittest.TestCase):
+  def _test(self, f):
+    for _ in range(5):
+      a, b = Tensor.randn(10, 10), Tensor.randn(10, 10)
+      out0, out1, out2 = f(a, b)
+      np.testing.assert_allclose(out0.numpy(), a.numpy()+b.numpy(), atol=1e-4, rtol=1e-5)
+      np.testing.assert_allclose(out1.numpy(), a.numpy()-b.numpy(), atol=1e-4, rtol=1e-5)
+      np.testing.assert_allclose(out2.numpy(), a.numpy()*b.numpy(), atol=1e-4, rtol=1e-5)
+
+  def test_jit_multioutput_realize(self):
+    @TinyJit
+    def fxn(a, b): return (a+b).realize(), (a-b).realize(), (a*b).realize()
+    self._test(fxn)
+    assert_jit_cache_len(fxn, 3)
+
+  def test_jit_multioutput_norealize(self):
+    @TinyJit
+    def fxn(a, b): return a+b, a-b, a*b
+    self._test(fxn)
+    assert_jit_cache_len(fxn, 1)
+
+  def test_jit_multioutput_mix(self):
+    @TinyJit
+    def fxn(a, b): return a+b, a-b, (a*b).realize()
+    self._test(fxn)
+    assert_jit_cache_len(fxn, 2)
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `tinygrad-0.8.0/test/test_kernel_cache.py` & `tinygrad-0.9.0/test/test_kernel_cache.py`

 * *Files identical despite different names*

### Comparing `tinygrad-0.8.0/test/test_lazybuffer.py` & `tinygrad-0.9.0/test/test_pickle.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,60 @@
-#!/usr/bin/env python
+import unittest, pickle
 import numpy as np
-import unittest
-from tinygrad.lazy import LazyBuffer
-from tinygrad import Device
-from tinygrad.tensor import Tensor
-
-class TestLazyBuffer(unittest.TestCase):
-  @unittest.skip("it doesn't work like this anymore")
-  def test_fromcpu_buffer_sharing(self):
-    a = np.arange(8)
-    assert LazyBuffer.fromCPU(a).realized._buf is a
-
-  def test_fromcpu_shape_tracker(self):
-    def helper(a: np.ndarray):
-      print(a.shape, a.strides, a.flags.c_contiguous)
-      b = LazyBuffer.fromCPU(a)
-      #assert b.st.contiguous == a.flags.c_contiguous
-      assert b.st.shape == a.shape
-      np.testing.assert_equal(a, Tensor(b).numpy())
-
-    for ndims in range(1, 4):
-      a = np.random.randn(*(4,)*ndims).astype(np.float32)
-      for stride in [-2, 1, 2]:
-        for start in [0, 1]:
-          helper(a[(slice(start, None, stride),)*ndims])
-
-  def test_shuffle_pad_ops_cmpeq(self):
-    y = Tensor([1]).cat(Tensor([1]) == 0).numpy()
-    z = Tensor([1, 0]).numpy()
-    np.testing.assert_allclose(y, z)
-
-  def test_shuffle_pad_ops_div(self):
-    y = Tensor([1]).cat(Tensor([1]).div(Tensor([2.0]))).numpy()
-    z = Tensor([1, 0.5]).numpy()
-    np.testing.assert_allclose(y, z)
-
-  def test_shuffle_pad_ops_log(self):
-    y = Tensor([1]).cat(Tensor([1]).log()).numpy()
-    z = Tensor([1, 0]).numpy()
-    np.testing.assert_allclose(y, z)
-
-  def test_shuffle_pad_ops_exp(self):
-    y = Tensor([1]).cat(Tensor([1]).exp()).numpy()
-    z = Tensor([1, np.e]).numpy()
-    np.testing.assert_allclose(y, z)
-
-  def test_device_0_is_the_same_device(self):
-    a = Tensor([1, 2, 3], f"{Device.DEFAULT}")
-    b = Tensor([1, 2, 3], f"{Device.DEFAULT}:0")
-    assert a.device == b.device
+from tinygrad import Tensor, TinyJit
+from tinygrad.engine.schedule import create_schedule
 
-if __name__ == "__main__":
+class TestPickle(unittest.TestCase):
+  def test_pickle_realized_tensor(self):
+    t = Tensor.rand(10, 10).realize()
+    st = pickle.dumps(t)
+    t2:Tensor = pickle.loads(st)
+    np.testing.assert_equal(t.numpy(), t2.numpy())
+
+  def test_pickle_unrealized_tensor(self):
+    t = Tensor.ones(10, 10)
+    st = pickle.dumps(t)
+    t2:Tensor = pickle.loads(st)
+    np.testing.assert_equal(t.numpy(), t2.numpy())
+
+  def test_pickle_buffer_view(self):
+    t = Tensor.arange(10, device="CLANG").contiguous().realize()
+    vt = t[3:5].contiguous().realize()
+    assert hasattr(vt.lazydata.buffer, 'base')
+    ref_value = vt.tolist()
+    st = pickle.dumps(vt)
+    del t, vt
+    vt2 = pickle.loads(st)
+    assert hasattr(vt2.lazydata.buffer, 'base')
+    assert ref_value == vt2.tolist()
+
+  def test_pickle_numpy(self):
+    t = Tensor(np.array([1,2,3,4.]))
+    st = pickle.dumps(t)
+    t2:Tensor = pickle.loads(st)
+    np.testing.assert_equal(t.numpy(), t2.numpy())
+
+  def test_pickle_jit(self):
+    @TinyJit
+    def add(a, b): return a+b+1
+    for _ in range(3): add(Tensor.rand(10, 10), Tensor.rand(10, 10))
+    del add.fxn  # pickling the JIT requires the function to be deleted
+    st = pickle.dumps(add)
+    del add
+
+    add_fxn = pickle.loads(st)
+    x = Tensor.ones(10, 10).contiguous().realize()
+    y = Tensor.ones(10, 10).contiguous().realize()
+    print("post jit")
+    out = add_fxn(x, y)
+    np.testing.assert_equal(out.numpy(), 3)
+
+  def test_pickle_schedule(self):
+    a = Tensor([1,2])
+    out = a + 2
+    sched = create_schedule([out.lazydata])
+    pk = pickle.dumps(sched)
+    sched_pk = pickle.loads(pk)
+    assert sched_pk[-1].ast == sched[-1].ast
+
+if __name__ == '__main__':
   unittest.main()
```

### Comparing `tinygrad-0.8.0/test/test_lazyop.py` & `tinygrad-0.9.0/test/test_lazyop.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import unittest
 from tinygrad.tensor import Tensor
+from tinygrad.engine.schedule import create_schedule
 
 # stuff needed to unpack a kernel
 # ruff: noqa: F401
 from tinygrad.ops import LazyOp, TernaryOps, BinaryOps, UnaryOps, ReduceOps, BufferOps, MemBuffer, ConstBuffer
 from tinygrad.lazy import LazyBuffer
 from tinygrad import dtypes
 from tinygrad.shape.shapetracker import ShapeTracker
@@ -12,22 +13,22 @@
 import numpy as np
 import time
 inf, nan = float('inf'), float('nan')
 
 class TestLazyOp(unittest.TestCase):
   def test_lazyop_str(self):
     t = Tensor.rand(10) + Tensor.rand(10)
-    s = t.lazydata.schedule()
+    s = create_schedule([t.lazydata])
     ast = s[-1].ast
     ast_remade = eval(str(ast))
     self.assertEqual(ast, ast_remade)
 
   def test_selfreferential_speed(self):
     st = time.monotonic()
     for i in range(25):
-      p = LazyBuffer.fromCPU(np.array([1]))
+      p = Tensor([1]).lazydata
       for _ in range(i): p = p.e(BinaryOps.ADD, p)
       # sanity check if caching works this should be way faster
       assert time.monotonic() -st < 0.5, f"{i}"
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `tinygrad-0.8.0/test/test_masked_st.py` & `tinygrad-0.9.0/test/test_masked_st.py`

 * *Files identical despite different names*

### Comparing `tinygrad-0.8.0/test/test_method_cache.py` & `tinygrad-0.9.0/test/test_method_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import unittest
 from tinygrad import Tensor, Device, Variable
-from tinygrad.device import Compiled
 from examples.gpt2 import Transformer
 from tinygrad.nn.state import get_state_dict
 
-@unittest.skipIf(not isinstance(Device[Device.DEFAULT], Compiled), "only test for compiled backends")
 class TestMethodCache(unittest.TestCase):
   def setUp(self):
     self.backup_compiler = Device[Device.DEFAULT].compiler
   def tearDown(self):
     Device[Device.DEFAULT].compiler = self.backup_compiler
 
   def test_simple_methodcache(self):
@@ -28,14 +26,15 @@
 
   def test_nested_methodcache_swap(self):
     a,b,c,d = Tensor([1]), Tensor([2]), Tensor([3]), Tensor([4])
     ((a+b)+(c+d)).realize()
     Device[Device.DEFAULT].compiler = None
     ((c+d)+(a+b)).realize()
 
+  @unittest.skip("incorrect use of transformer")
   def test_small_transformer(self):
     args_tiny = {"dim": 16, "n_heads": 8, "n_layers": 8, "norm_eps": 1e-05, "vocab_size": 10}
     model = Transformer(**args_tiny)
     for v in get_state_dict(model).values(): v.assign(Tensor.empty(*v.shape, dtype=v.dtype).realize())
     # NOTE: you have to do this twice due to the k-v cache
     for i in range(3): model(Tensor([[1,2,3,4]]), Variable("start_pos", 0, 10).bind(i)).realize()
     for i in range(3): model(Tensor([[1,2,3,4]]), Variable("start_pos", 0, 10).bind(i)).realize()
```

### Comparing `tinygrad-0.8.0/test/test_net_speed.py` & `tinygrad-0.9.0/test/test_net_speed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 import time
 import unittest
 import torch
 from tinygrad import Tensor, Device
 from tinygrad.helpers import Profiling, CI
 
-@unittest.skipIf(CI and Device.DEFAULT == "CUDA", "slow")
+@unittest.skipIf(CI and Device.DEFAULT in {"CUDA", "NV"}, "slow")
 class TestConvSpeed(unittest.TestCase):
 
   def test_mnist(self):
     # https://keras.io/examples/vision/mnist_convnet/
     conv = 3
     inter_chan, out_chan = 32, 64
```

### Comparing `tinygrad-0.8.0/test/test_nn.py` & `tinygrad-0.9.0/test/test_nn.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 #!/usr/bin/env python
 import unittest
 import numpy as np
 import torch
 from tinygrad import Tensor, Device, TinyJit
-from tinygrad.helpers import CI
+from tinygrad.helpers import CI, Context
+from tinygrad.ops import BufferOps
 from tinygrad.nn import BatchNorm2d, Conv1d,ConvTranspose1d, Conv2d,ConvTranspose2d, Linear, GroupNorm, LayerNorm,LayerNorm2d, Embedding, InstanceNorm
+from tinygrad.nn.state import load_state_dict
+from tinygrad.engine.schedule import create_schedule
+from tinygrad.engine.realize import run_schedule
 
-@unittest.skipIf(CI and Device.DEFAULT == "CUDA", "slow")
+@unittest.skipIf(CI and Device.DEFAULT in {"CUDA", "NV"}, "slow")
 class TestNN(unittest.TestCase):
   @unittest.skipIf(Device.DEFAULT == "WEBGPU", "no int64 on WebGPU")
   def test_sparse_cat_cross_entropy(self):
     # create in tinygrad
-    input = Tensor.randn(3, 5)
-    target = Tensor.randint((3,), low=0, high=4)
-    loss = input.sparse_categorical_crossentropy(target)
-
+    input = Tensor.randn(5, 5)
+    target = Tensor([0, 0, 0, 1, 2])  # torch doesn't support target=-1
     torch_input = torch.tensor(input.numpy())
     torch_target = torch.tensor(target.numpy(), dtype=torch.long)
-    torch_loss = torch.nn.CrossEntropyLoss(reduction='mean')(torch_input, torch_target)
 
-    np.testing.assert_allclose(loss.numpy(), torch_loss.detach().numpy(), atol=1e-5, rtol=1e-6)
+    for smoothing in [0.0, 0.1, 0.5, 1.0]:
+      for ignore_index in [-1, 0, 2]:
+        loss = input.sparse_categorical_crossentropy(target, label_smoothing=smoothing, ignore_index=ignore_index)
+        torch_loss = torch.nn.CrossEntropyLoss(reduction='mean', label_smoothing=smoothing, ignore_index=ignore_index)(torch_input, torch_target)
+        np.testing.assert_allclose(loss.numpy(), torch_loss.detach().numpy(), atol=1e-5, rtol=1e-6)
 
   def test_batchnorm2d(self, training=False):
     with Tensor.train(training):
       szs = [4, 8, 16, 32]
       for sz in szs:
         # create in tinygrad
         bn = BatchNorm2d(sz, eps=1e-5, track_running_stats=training)
@@ -58,14 +63,32 @@
         np.testing.assert_allclose(outt.numpy(), toutt.detach().numpy(), rtol=5e-4, atol=1e-6)
         np.testing.assert_allclose(bn.running_mean.numpy(), tbn.running_mean.detach().numpy(), rtol=1e-5, atol=1e-6)
         np.testing.assert_allclose(bn.running_var.numpy(), tbn.running_var.detach().numpy(), rtol=1e-5, atol=1e-6)
 
   def test_batchnorm2d_training(self):
     self.test_batchnorm2d(True)
 
+  def test_batchnorm_axis(self):
+    sz = (2, 4, 3, 2, 2)
+    x = Tensor.randn(sz)
+    weight = Tensor.randn(2, 3)
+    bias = Tensor.randn(2, 3)
+    mean = Tensor.randn(2, 3)
+    invstd = Tensor.randn(2, 3)
+    a = (x.batchnorm(weight, bias, mean, invstd, axis=(0, 2))
+         .permute(1, 0, 2, 3, 4).reshape(4, 6, 2, 2))
+    b = (x.permute(1, 0, 2, 3, 4).reshape(4, 6, 2, 2)
+         .batchnorm(weight.flatten(), bias.flatten(), mean.flatten(), invstd.flatten()))
+    t_x = torch.tensor(x.permute(1, 0, 2, 3, 4).reshape(4, 6, 2, 2).numpy())
+    t_weight, t_bias = torch.tensor(weight.flatten().numpy()), torch.tensor(bias.flatten().numpy())
+    t_mean, t_invstd = torch.tensor(mean.flatten().numpy()), torch.tensor(invstd.flatten().numpy())
+    torch.nn.functional.batch_norm(t_x, t_mean, 1.0 / t_invstd**2, t_weight, t_bias)
+
+    np.testing.assert_allclose(a.numpy(), b.numpy())
+
   def test_linear(self):
     def _test_linear(x, in_dim, out_dim):
       # create in tinygrad
       model = Linear(in_dim, out_dim)
       z = model(x)
 
       # create in torch
@@ -119,15 +142,15 @@
     # test
     x = Tensor.uniform(BS, C1, H, W)
     z = layer(x)
     torch_x = torch.tensor(x.numpy())
     torch_z = torch_layer(torch_x)
     np.testing.assert_allclose(z.numpy(), torch_z.detach().numpy(), atol=5e-4, rtol=1e-5)
 
-  @unittest.skipIf(Device.DEFAULT not in {"CPU", "TORCH"}, "Takes too long to compile for Compiled backends")
+  @unittest.skip("Takes too long to compile for Compiled backends")
   def test_conv2d_winograd(self):
     BS, C1, H, W = 2, 8, 16, 16
     C2, K, S, P = 8, 3, 1, 1
 
     # create in tinygrad
     layer = Conv2d(C1, C2, kernel_size=K, stride=S, padding=P)
     layer.weight.requires_grad = True
@@ -137,18 +160,16 @@
     torch_layer = torch.nn.Conv2d(C1, C2, kernel_size=K, stride=S, padding=P).eval()
     torch_layer.weight = torch.nn.Parameter(torch.tensor(layer.weight.numpy(), dtype=torch.float32))
     torch_layer.bias = torch.nn.Parameter(torch.tensor(layer.bias.numpy(), dtype=torch.float32))
 
     # test
     x = Tensor.uniform(BS, C1, H, W, requires_grad=True)
 
-    old_wino = Tensor.wino
-    Tensor.wino = True
-    z = layer(x)
-    Tensor.wino = old_wino
+    with Context(WINO=1):
+      z = layer(x)
 
     torch_x = torch.tensor(x.numpy(), requires_grad=True)
     torch_z = torch_layer(torch_x)
     np.testing.assert_allclose(z.numpy(), torch_z.detach().numpy(), atol=5e-4, rtol=1e-5)
 
     m = z.mean()
     m.backward()
@@ -157,15 +178,14 @@
     gx = x.grad.realize()
 
     torch_z.mean().backward()
     np.testing.assert_allclose(gw.numpy(), torch_layer.weight.grad.numpy(), atol=5e-4, rtol=1e-5)
     np.testing.assert_allclose(gb.numpy(), torch_layer.bias.grad.numpy(), atol=5e-4, rtol=1e-5)
     np.testing.assert_allclose(gx.numpy(), torch_x.grad.numpy(), atol=5e-4, rtol=1e-5)
 
-
   @unittest.skipIf(CI and Device.DEFAULT == "WEBGPU", "runs out of memory in CI")
   def test_conv_transpose1d(self):
     BS, C1, W = 4, 16, 224//4
     C2, K, S, P = 64, 7, 2, 1
 
     # create in tinygrad
     layer = ConvTranspose1d(C1, C2, kernel_size=K, stride=S, padding=P)
@@ -331,10 +351,56 @@
     for _ in range(3):
       x = Tensor(np.random.randint(0, vocab_size, (B, T)))
       z = layer_jit(x)
       torch_x = torch.tensor(x.numpy())
       torch_z = torch_layer(torch_x)
       np.testing.assert_allclose(z.numpy(), torch_z.detach().numpy(), atol=1e-8, rtol=1e-8)
 
+  def test_embedding_one_kernel(self):
+    layer = Embedding(20, 30)
+    a = Tensor([[1, 5, 9, 11],
+                [12, 19, 8, 1]])
+    result = layer(a)
+    schedule = create_schedule([result.lazydata])
+    self.assertEqual(3, len([item for item in schedule if item.ast[0].op is BufferOps.STORE]), "first run realizes arange, weight, and embedding")
+    run_schedule(schedule)
+
+    b = Tensor([[1, 2, 3],
+                [4, 5, 6],
+                [7, 8, 9]])
+    result = layer(b)
+    schedule = create_schedule([result.lazydata])
+    self.assertEqual(1, len([item for item in schedule if item.ast[0].op is BufferOps.STORE]), "second run realizes embedding only")
+    run_schedule(schedule)
+
+  def test_load_state_dict(self):
+    layer = Conv2d(3, 5, kernel_size=3)
+
+    state_dict = {
+      'weight': Tensor.randn(5, 3, 3, 3),
+      'bias': Tensor.randn(5),
+    }
+    load_state_dict(layer, state_dict)
+
+    np.testing.assert_allclose(layer.weight.numpy(), state_dict['weight'].numpy())
+    np.testing.assert_allclose(layer.bias.numpy(), state_dict['bias'].numpy())
+
+  @unittest.skipIf(CI and Device.DEFAULT in {"GPU", "CUDA", "METAL"}, "no GPU CI")
+  def test_load_state_dict_sharded(self):
+    devices = (f"{Device.DEFAULT}:1", f"{Device.DEFAULT}:2")
+
+    layer = Conv2d(3, 5, kernel_size=3)
+    layer.weight.shard_(devices, -1)
+    layer.bias.shard_(devices, None)
+    state_dict = {
+      'weight': Tensor.randn(5, 3, 3, 3).shard(devices, -1),
+      'bias': Tensor.randn(5).shard(devices, None),
+    }
+    load_state_dict(layer, state_dict)
+
+    self.assertEqual(layer.weight.device, devices)
+    self.assertEqual(layer.bias.device, devices)
+    np.testing.assert_allclose(layer.weight.numpy(), state_dict['weight'].numpy())
+    np.testing.assert_allclose(layer.bias.numpy(), state_dict['bias'].numpy())
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `tinygrad-0.8.0/test/test_ops.py` & `tinygrad-0.9.0/test/test_ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,45 @@
-import torch
 import time, math, unittest
 import numpy as np
-from tinygrad.tensor import Tensor
+import torch
 from tinygrad.helpers import getenv, IMAGE, DEBUG, CI
-from tinygrad import Device, dtypes
+from tinygrad import Tensor, Device, dtypes
 
 if CI:
   import warnings
   warnings.filterwarnings("ignore", message="Non-empty compiler output encountered")
 
 FORWARD_ONLY = getenv("FORWARD_ONLY", 0)
 PRINT_TENSORS = getenv("PRINT_TENSORS", 0)
+
 def helper_test_op(shps, torch_fxn, tinygrad_fxn=None, atol=1e-6, rtol=1e-3, grad_atol=1e-4, grad_rtol=1e-3,
-                   forward_only=False, vals=None, a=-0.5, b=3):
+                   forward_only=False, vals=None, low=-1.5, high=1.5):
   if tinygrad_fxn is None: tinygrad_fxn = torch_fxn
-  ts, tst = prepare_test_op(a, b, shps, vals, forward_only)
+  ts, tst = prepare_test_op(low, high, shps, vals, forward_only)
 
   st = time.monotonic()
   out = torch_fxn(*ts)
   torch_fp = time.monotonic() - st
 
+  # move inputs to a different device, test the device of intermediate tensors are correct
+  if mt:=getenv("MOVE_TENSOR", ""):
+    for t in tst: t.to_(mt)
+
   st = time.monotonic()
   ret = tinygrad_fxn(*tst).realize()
   tinygrad_fp = time.monotonic() - st
 
-  def compare(s, x,y,atol,rtol):
-    if PRINT_TENSORS: print(s, x, y)
-    assert x.shape == y.shape, f"shape mismatch: tinygrad={x.shape} | torch={y.shape}"
+  def compare(s, tinygrad_output, torch_output, atol, rtol):
+    if PRINT_TENSORS: print(s, tinygrad_output, torch_output)
     try:
-      np.testing.assert_allclose(x,y, atol=atol, rtol=rtol)
-    except Exception:
-      raise Exception(f"{s} failed shape {x.shape}")
+      assert tinygrad_output.shape == torch_output.shape, f"shape mismatch: tinygrad={tinygrad_output.shape} | torch={torch_output.shape}"
+      assert tinygrad_output.dtype == torch_output.dtype, f"dtype mismatch: tinygrad={tinygrad_output.dtype} | torch={torch_output.dtype}"
+      np.testing.assert_allclose(tinygrad_output, torch_output, atol=atol, rtol=rtol)
+    except Exception as e:
+      raise Exception(f"{s} failed shape {tinygrad_output.shape}: {e}")
 
   if DEBUG >= 6:
     np.set_printoptions(linewidth=200, suppress=True)
     print(ret.numpy())
     print(out.detach().numpy())
   compare("forward pass", ret.numpy(), out.detach().numpy(), atol=atol, rtol=rtol)
 
@@ -52,112 +57,141 @@
     for i, (t, tt) in enumerate(zip(ts, tst)):
       compare(f"backward pass tensor {i}", tt.grad.numpy(), t.grad.detach().numpy(), atol=grad_atol, rtol=grad_rtol)
 
   if not CI:
     print("\ntesting %40r   torch/tinygrad fp: %.2f / %.2f ms  bp: %.2f / %.2f ms " % \
           (shps, torch_fp*1000, tinygrad_fp*1000, torch_fbp*1000, tinygrad_fbp*1000), end="")
 
-def prepare_test_op(a, b, shps, vals, forward_only=False):
-  torch.manual_seed(0)
-  np.random.seed(0)
-  if shps is None: ts = [torch.tensor(x, requires_grad=(not forward_only)) for x in vals]
-  else: ts = [torch.tensor((np.random.random(size=x) + a) * b, requires_grad=(not forward_only), dtype=torch.float32) for x in shps]
+def prepare_test_op(low, high, shps, vals, forward_only=False):
+  if shps is None:
+    ts = [torch.tensor(x, requires_grad=(not forward_only)) for x in vals]
+  else:
+    np.random.seed(0)
+    np_data = [np.random.uniform(low=low, high=high, size=size).astype(dtypes.default_float.np) for size in shps]
+    ts = [torch.tensor(data, requires_grad=(not forward_only)) for data in np_data]
   tst = [Tensor(x.detach().numpy(), requires_grad=(not forward_only and not FORWARD_ONLY)) for x in ts]
   return ts, tst
 
 class TestOps(unittest.TestCase):
 
-  def helper_test_exception(self, shps, torch_fxn, tinygrad_fxn, expected, exact=False, vals=None, a=-0.5, b=3):
-    if getenv("CUDACPU"): self.skipTest('helper_test_exception fails in CUDACPU')
-    ts, tst = prepare_test_op(a, b, shps, vals)
+  def helper_test_exception(self, shps, torch_fxn, tinygrad_fxn, expected, exact=False, vals=None, low=-1.5, high=1.5):
+    if getenv("CUDACPU") or (getenv("MOCKGPU") and Device.DEFAULT == "NV"): self.skipTest('helper_test_exception fails in CUDACPU')
+    ts, tst = prepare_test_op(low, high, shps, vals)
     with self.assertRaises(expected) as torch_cm:
       torch_fxn(*ts)
     with self.assertRaises(expected) as tinygrad_cm:
       tinygrad_fxn(*tst)
     if exact: self.assertEqual(str(torch_cm.exception), str(tinygrad_cm.exception))
     if not CI: print("\ntesting %40r   torch/tinygrad exception: %s / %s" % (shps, torch_cm.exception, tinygrad_cm.exception), end="")
 
   def test_full_like(self):
-    a = Tensor([[1,2,3],[4,5,6]])
-    b = torch.tensor([[1,2,3],[4,5,6]])
+    a = Tensor([[1,2,3],[4,5,6]], dtype=dtypes.float32)
+    b = torch.tensor([[1,2,3],[4,5,6]], dtype=torch.float32)
     helper_test_op([], lambda: torch.full_like(b, 4), lambda: Tensor.full_like(a, 4), forward_only=True)
+
+    a = Tensor([[1,2,3],[4,5,6]], dtype=dtypes.int32)
+    b = torch.tensor([[1,2,3],[4,5,6]], dtype=torch.int32)
+    helper_test_op([], lambda: torch.full_like(b, 4), lambda: Tensor.full_like(a, 4), forward_only=True)
+
   def test_full(self):
-    helper_test_op([], lambda: torch.full((45,65), 4), lambda: Tensor.full((45,65), 4), forward_only=True)
+    helper_test_op([], lambda: torch.full((45,65), 4, dtype=torch.int32), lambda: Tensor.full((45,65), 4), forward_only=True)
+
   def test_zeros(self):
     helper_test_op([], lambda: torch.zeros(45,65), lambda: Tensor.zeros(45,65), forward_only=True)
     helper_test_op([], lambda: torch.zeros([45,65]), lambda: Tensor.zeros([45,65]), forward_only=True)
     helper_test_op([], lambda: torch.zeros([]), lambda: Tensor.zeros([]), forward_only=True)
+
   def test_zeros_like(self):
-    a = Tensor([[1,2,3],[4,5,6]])
-    b = torch.tensor([[1,2,3],[4,5,6]])
+    a = Tensor([[1,2,3],[4,5,6]], dtype=dtypes.float32)
+    b = torch.tensor([[1,2,3],[4,5,6]], dtype=torch.float32)
+    helper_test_op([], lambda: torch.zeros_like(b), lambda: Tensor.zeros_like(a), forward_only=True)
+
+    a = Tensor([[1,2,3],[4,5,6]], dtype=dtypes.int32)
+    b = torch.tensor([[1,2,3],[4,5,6]], dtype=torch.int32)
     helper_test_op([], lambda: torch.zeros_like(b), lambda: Tensor.zeros_like(a), forward_only=True)
+
   def test_empty_0(self):
     helper_test_op([], lambda: torch.empty(45,65)*0/0, lambda: Tensor.empty(45,65)*0/0, forward_only=True)
+
   def test_ones(self):
     helper_test_op([], lambda: torch.ones(45,65), lambda: Tensor.ones(45,65), forward_only=True)
     helper_test_op([], lambda: torch.ones([45,65]), lambda: Tensor.ones([45,65]), forward_only=True)
     helper_test_op([], lambda: torch.ones([]), lambda: Tensor.ones([]), forward_only=True)
+
   def test_ones_like(self):
-    a = Tensor([[1,2,3],[4,5,6]])
-    b = torch.tensor([[1,2,3],[4,5,6]])
+    a = Tensor([[1,2,3],[4,5,6]], dtype=dtypes.float32)
+    b = torch.tensor([[1,2,3],[4,5,6]], dtype=torch.float32)
+    helper_test_op([], lambda: torch.ones_like(b), lambda: Tensor.ones_like(a), forward_only=True)
+
+    a = Tensor([[1,2,3],[4,5,6]], dtype=dtypes.int32)
+    b = torch.tensor([[1,2,3],[4,5,6]], dtype=torch.int32)
     helper_test_op([], lambda: torch.ones_like(b), lambda: Tensor.ones_like(a), forward_only=True)
+
   def test_eye(self):
     helper_test_op([], lambda: torch.eye(10), lambda: Tensor.eye(10), forward_only=True)
     helper_test_op([], lambda: torch.eye(1), lambda: Tensor.eye(1), forward_only=True)
+    helper_test_op([], lambda: torch.eye(0), lambda: Tensor.eye(0), forward_only=True)
 
   def test_split(self):
+    def tensor(s): return torch.arange(math.prod(s), dtype=torch.int32).reshape(s), Tensor.arange(math.prod(s)).reshape(s)
     test_cases = [
-      (torch.arange(10), Tensor.arange(10), 5),
-      (torch.arange(10), Tensor.arange(10), [1, 4, 5]),
-      (torch.arange(10), Tensor.arange(10), 3),
-      (torch.arange(12).reshape(3, 4), Tensor.arange(12).reshape(3, 4), 1),
-      (torch.arange(16).reshape(4, 4), Tensor.arange(16).reshape(4, 4), [2, 2]),
-      (torch.arange(10000), Tensor.arange(10000), 2500),
+      (tensor((10,)),       5, {}),
+      (tensor((10,)), [1,4,5], {}),
+      (tensor((10,)),       3, {}),
+      (tensor((3,4,)),      1, {}),
+      (tensor((3,4,)),      1, {'dim':1}),
+      (tensor((4,4,)),  [2,2], {}),
+      (tensor((4,4,)),  [2,2], {'dim':1}),
+      (tensor((10000,)), 2500, {}),
     ]
 
-    for tor, ten, sizes in test_cases:
-      tor_splits, ten_splits = tor.split(sizes), ten.split(sizes)
+    for (tor, ten), sizes, args in test_cases:
+      tor_splits, ten_splits = tor.split(sizes, **args), ten.split(sizes, **args)
       assert len(tor_splits) == len(ten_splits)
       for tor_chunk, ten_chunk in zip(tor_splits, ten_splits):
         helper_test_op([], lambda: tor_chunk, lambda: ten_chunk, forward_only=True)
 
   def test_chunk(self):
-    tor = torch.arange(13).repeat(8, 1).chunk(6, 1)
+    tor = torch.arange(13, dtype=torch.int32).repeat(8, 1).chunk(6, 1)
     ten = Tensor.arange(13).repeat((8, 1)).chunk(6, 1)
     assert len(tor) == len(ten)
     for i in range(len(tor)):
       helper_test_op([], lambda: tor[i], lambda: ten[i], forward_only=True)
 
-    tor = torch.arange(13).repeat(8, 1).chunk(6, 0)
+    tor = torch.arange(13, dtype=torch.int32).repeat(8, 1).chunk(6, 0)
     ten = Tensor.arange(13).repeat((8, 1)).chunk(6, 0)
     assert len(tor) == len(ten)
     for i in range(len(tor)):
       helper_test_op([], lambda: tor[i], lambda: ten[i], forward_only=True)
 
-    tor = torch.arange(13).repeat(8, 1).chunk(3, -1)
+    tor = torch.arange(13, dtype=torch.int32).repeat(8, 1).chunk(3, -1)
     ten = Tensor.arange(13).repeat((8, 1)).chunk(3, -1)
     assert len(tor) == len(ten)
     for i in range(len(tor)):
       helper_test_op([], lambda: tor[i], lambda: ten[i], forward_only=True)
 
-    tor = torch.arange(13).repeat(8, 3, 3).chunk(3, -2)
+    tor = torch.arange(13, dtype=torch.int32).repeat(8, 3, 3).chunk(3, -2)
     ten = Tensor.arange(13).repeat((8, 3, 3)).chunk(3, -2)
     assert len(tor) == len(ten)
     for i in range(len(tor)):
       helper_test_op([], lambda: tor[i], lambda: ten[i], forward_only=True)
 
   def test_arange(self):
-    helper_test_op([], lambda: torch.arange(10), lambda: Tensor.arange(10), forward_only=True)
-    helper_test_op([], lambda: torch.arange(5, 10, 3), lambda: Tensor.arange(5, 10, 3), forward_only=True)
-    helper_test_op([], lambda: torch.arange(10, 5, -3), lambda: Tensor.arange(10, 5, -3), forward_only=True)
-    helper_test_op([], lambda: torch.arange(11, 5, -3), lambda: Tensor.arange(11, 5, -3), forward_only=True)
-  def test_arange_simple(self):
-    helper_test_op([], lambda: torch.arange(10), lambda: Tensor.arange(10), forward_only=True)
+    helper_test_op([], lambda: torch.arange(10, dtype=torch.int32), lambda: Tensor.arange(10), forward_only=True)
+    helper_test_op([], lambda: torch.arange(36, dtype=torch.int32), lambda: Tensor.arange(36), forward_only=True)
+    helper_test_op([], lambda: torch.arange(5, 10, 3, dtype=torch.int32), lambda: Tensor.arange(5, 10, 3), forward_only=True)
+    helper_test_op([], lambda: torch.arange(10, 5, -3, dtype=torch.int32), lambda: Tensor.arange(10, 5, -3), forward_only=True)
+    helper_test_op([], lambda: torch.arange(11, 5, -3, dtype=torch.int32), lambda: Tensor.arange(11, 5, -3), forward_only=True)
+    helper_test_op([], lambda: torch.arange(1, 78, 2, dtype=torch.int32), lambda: Tensor.arange(1, 78, 2), forward_only=True)
+    helper_test_op([], lambda: torch.arange(5.5, 175.5, 2.5), lambda: Tensor.arange(5.5, 175.5, 2.5), forward_only=True)
+    helper_test_op([], lambda: torch.arange(-30.2, -0.3, 0.75), lambda: Tensor.arange(-30.2, -0.3, 0.75), forward_only=True)
+    helper_test_op([], lambda: torch.arange(-50.3, -380.2, -2.25), lambda: Tensor.arange(-50.3, -380.2, -2.25), forward_only=True)
+
   def test_arange_big(self):
-    helper_test_op([], lambda: torch.arange(256), lambda: Tensor.arange(256), forward_only=True)
+    helper_test_op([], lambda: torch.arange(256, dtype=torch.int32), lambda: Tensor.arange(256), forward_only=True)
 
   def test_sum_fake(self):
     helper_test_op([(256, 1)], lambda x: x.sum(axis=1))
 
   def test_sum_collapse(self):
     helper_test_op([], lambda: torch.ones(256,256).sum(axis=1), lambda: Tensor.ones(256,256).sum(axis=1), forward_only=True)
 
@@ -175,27 +209,27 @@
 
   def test_max_dont_collapse(self):
     helper_test_op([], lambda: torch.ones(256,256).max(1)[0], lambda: Tensor.ones(256,256).max(1), forward_only=True)
 
   def test_where(self):
     helper_test_op(
       [(100,)],
-      lambda x: torch.where(x > 0.5, 4, 2),
+      lambda x: torch.where(x > 0.5, 4, 2).type(torch.int32),
       lambda x: (x > 0.5).where(4, 2), forward_only=True)
 
     for shps in [[(8,),(1,),(1,)], [(10,10),(10,),(10,)], [(100,)]*3, [(10,10)]*3]:
       helper_test_op(
         shps,
         lambda x, a, b: torch.where(x > 0.5, a, b),
         lambda x, a, b: (x > 0.5).where(a, b), forward_only=True)
 
   def test_where_permute(self):
     helper_test_op(
       [(5, 5)],
-      lambda x: torch.where(x > 0.5, 4, 2).permute((1, 0)),
+      lambda x: torch.where(x > 0.5, 4, 2).type(torch.int32).permute((1, 0)),
       lambda x: (x > 0.5).where(4, 2).permute((1, 0)), forward_only=True)
 
   def _test_cmp(self, fxn, reverse=True):
     for shps in [[(3, 4, 5), (3, 4, 5)], [(3, 4, 5), (5,)], [(5,), (3, 4, 5)]]:
       helper_test_op(shps, fxn, fxn, forward_only=True)
     helper_test_op(None, fxn, fxn, forward_only=True, vals=[[0.,1,2], [2.,1,0]])
     helper_test_op(None, lambda x,y: fxn(x,2), lambda x,y: fxn(x,2), forward_only=True, vals=[[0.,1,2], [2.,1,0]])
@@ -212,277 +246,354 @@
   def test_cmp_eq_backwards(self):
     t1 = torch.ones(4, requires_grad=True)
     t2 = torch.ones(4, requires_grad=True)
     self.assertRaises(RuntimeError, (t1 == t2).sum().backward)
     tt1 = Tensor.ones(4, requires_grad=True)
     tt2 = Tensor.ones(4, requires_grad=True)
     self.assertRaises(RuntimeError, (tt1 == tt2).sum().backward)
+    tt = Tensor.randn(4, requires_grad=True)
+    (tt*(tt == 0)).sum().backward()
+    t = torch.tensor(tt.numpy(), requires_grad=True)
+    (t*(t == 0)).sum().backward()
+    np.testing.assert_allclose(t.grad.numpy(), tt.grad.numpy(), rtol=1e-5)
 
   def test_cmp_lt_backwards(self):
     t1 = torch.ones(4, requires_grad=True)
     t2 = torch.ones(4, requires_grad=True)
     self.assertRaises(RuntimeError, (t1 < t2).sum().backward)
     tt1 = Tensor.ones(4, requires_grad=True)
     tt2 = Tensor.ones(4, requires_grad=True)
     self.assertRaises(RuntimeError, (tt1 < tt2).sum().backward)
+    tt = Tensor.randn(4, requires_grad=True)
+    (tt*(tt < 0)).sum().backward()
+    t = torch.tensor(tt.numpy(), requires_grad=True)
+    (t*(t < 0)).sum().backward()
+    np.testing.assert_allclose(t.grad.numpy(), tt.grad.numpy(), rtol=1e-5)
 
-  #@unittest.skip("this is broken with contiguous")
   def test_trunc(self):
-    helper_test_op([(45,65)], lambda x: torch.trunc(x), lambda x: x.trunc(), forward_only=True)
-    a, b = Tensor([1.0, 2.1, 0.0, -5.0, -2.5]), torch.tensor([1.0, 2.1, 0.0, -5.0, -2.5])
-    helper_test_op([], lambda: torch.trunc(b), lambda: Tensor.trunc(a), forward_only=True)
-  #@unittest.skip("this is broken with contiguous")
+    helper_test_op([(45,35)], lambda x: x.trunc(), forward_only=True)
+    helper_test_op(None, lambda x: x.trunc(), vals=[[1.499, 1.5, 1.501, 1.0, 2.1, 0.0, -5.0, -2.499, -2.5, -2.501]], forward_only=True)
   def test_floor(self):
-    helper_test_op([(45,65)], lambda x: torch.floor(x), lambda x: x.floor(), forward_only=True)
-    a, b = Tensor([1.0, 2.1, 0.0, -5.0, -2.5]), torch.tensor([1.0, 2.1, 0.0, -5.0, -2.5])
-    helper_test_op([], lambda: torch.floor(b), lambda: Tensor.floor(a), forward_only=True)
-  #@unittest.skip("this is broken with contiguous")
+    helper_test_op([(45,35)], lambda x: x.floor(), forward_only=True)
+    helper_test_op(None, lambda x: x.floor(), vals=[[1.499, 1.5, 1.501, 1.0, 2.1, 0.0, -5.0, -2.499, -2.5, -2.501]], forward_only=True)
   def test_ceil(self):
-    helper_test_op([(45,65)], lambda x: torch.ceil(x), lambda x: x.ceil(), forward_only=True)
-    a, b = Tensor([1.0, 2.1, 0.0, -5.0, -2.5]), torch.tensor([1.0, 2.1, 0.0, -5.0, -2.5])
-    helper_test_op([], lambda: torch.ceil(b), lambda: Tensor.ceil(a), forward_only=True)
+    helper_test_op([(45,35)], lambda x: x.ceil(), forward_only=True)
+    helper_test_op(None, lambda x: x.ceil(), vals=[[1.499, 1.5, 1.501, 1.0, 2.1, 0.0, -5.0, -2.499, -2.5, -2.501]], forward_only=True)
+  def test_round(self):
+    helper_test_op([(45,35)], lambda x: x.round(), forward_only=True)
+    helper_test_op(None, lambda x: x.round(), vals=[[1.499, 1.5, 1.501, 1.0, 2.1, 0.0, -5.0, -2.499, -2.5, -2.501]], forward_only=True)
+    helper_test_op(None, lambda x: x.round(), vals=[[2.5, -1.5]], forward_only=True)
+  def test_lerp(self):
+    helper_test_op([(45,35), (45,35), (45,35)], lambda x,y,z: x.lerp(y,z))
+    helper_test_op(None, lambda x,y,z: x.lerp(y,z), vals=[[1.,2.,3.], [4.,5.,6.], 0.5])
+
   def test_tril(self):
-    helper_test_op([(3,3)], lambda x: x.tril(), lambda x: x.tril())
-    helper_test_op([(3,3)], lambda x: x.tril(1), lambda x: x.tril(1))
-    helper_test_op([(3,3)], lambda x: x.tril(-1), lambda x: x.tril(-1))
-    helper_test_op([(5,3,3)], lambda x: x.tril(), lambda x: x.tril())
-    helper_test_op([(5,3,3)], lambda x: x.tril(1), lambda x: x.tril(1))
+    helper_test_op([(3,3)], lambda x: x.tril())
+    helper_test_op([(3,3)], lambda x: x.tril(1))
+    helper_test_op([(3,3)], lambda x: x.tril(-1))
+    helper_test_op([(5,3,3)], lambda x: x.tril())
+    helper_test_op([(5,0,3)], lambda x: x.tril())
+    helper_test_op([(5,3,3)], lambda x: x.tril(1))
   def test_triu(self):
-    helper_test_op([(3,3)], lambda x: x.triu(), lambda x: x.triu())
-    helper_test_op([(3,3)], lambda x: x.triu(1), lambda x: x.triu(1))
-    helper_test_op([(3,3)], lambda x: x.triu(-1), lambda x: x.triu(-1))
-    helper_test_op([(5,3,3)], lambda x: x.triu(), lambda x: x.triu())
-    helper_test_op([(5,3,3)], lambda x: x.triu(1), lambda x: x.triu(1))
+    helper_test_op([(3,3)], lambda x: x.triu())
+    helper_test_op([(3,3)], lambda x: x.triu(1))
+    helper_test_op([(3,3)], lambda x: x.triu(-1))
+    helper_test_op([(5,3,3)], lambda x: x.triu())
+    helper_test_op([(5,0,3)], lambda x: x.triu())
+    helper_test_op([(5,3,3)], lambda x: x.triu(1))
+
   def test_maximum(self):
     helper_test_op([(45,65), (45,65)], torch.maximum, Tensor.maximum)
     helper_test_op([(), ()], torch.maximum, Tensor.maximum)
-    helper_test_op(None, torch.maximum, Tensor.maximum, vals=[[1., 0., 3., 4.], [1., 2., 3., 0.]])
-    helper_test_op(None, torch.maximum, Tensor.maximum, vals=np.array([[1, 0, 3, 4], [1, 2, 3, 0]], dtype=np.int32), forward_only=True)
+    helper_test_op(None, torch.maximum, Tensor.maximum, vals=[[1., 0., 3., -4.], 3.])
+    helper_test_op(None, torch.maximum, Tensor.maximum, vals=[[1., 0., 3., -4.], [-1., -2., 3., 0.]])
+    helper_test_op(None, torch.maximum, Tensor.maximum, vals=[[True, False, False], True], forward_only=True)
+    helper_test_op(None, torch.maximum, Tensor.maximum, vals=[[True, False, False], [True, True, False]], forward_only=True)
   def test_minimum(self):
     helper_test_op([(45,65), (45,65)], torch.minimum, Tensor.minimum)
     helper_test_op([(), ()], torch.minimum, Tensor.minimum)
+    helper_test_op(None, torch.minimum, Tensor.minimum, vals=[[1., 0., 3., -4.], 3.])
+    helper_test_op(None, torch.minimum, Tensor.minimum, vals=[[1., 0., 3., -4.], [-1., -2., 3., 0.]])
+    helper_test_op(None, torch.minimum, Tensor.minimum, vals=[[True, False, False], True], forward_only=True)
+    helper_test_op(None, torch.minimum, Tensor.minimum, vals=[[True, False, False], [True, True, False]], forward_only=True)
+
+  def test_tiny_add(self):
+    helper_test_op([(3), (3)], lambda x,y: x+y, Tensor.add, forward_only=True)
+
   def test_add(self):
     helper_test_op([(45,68), (45,68)], lambda x,y: x+y, Tensor.add)
-  def test_add_number(self):
-    helper_test_op([(), ()], lambda x,y: x+y, Tensor.add)
+    helper_test_op([(45,68), (45,68)], lambda x,y: x+y)
+    helper_test_op([(), ()], lambda x,y: x+y)
   def test_add3(self):
     helper_test_op([(45,65), (45,65), (45,65)], lambda x,y,z: x+y+z)
-  def test_add_simple(self):
-    helper_test_op([(256), (256)], lambda x,y: x+y, Tensor.add, forward_only=True)
   def test_broadcasted_add(self):
-    helper_test_op([(45,65), (45,1)], lambda x,y: x+y, lambda x,y: x+y)
-    helper_test_op([(45,65), ()], lambda x,y: x+y, lambda x,y: x+y)
+    helper_test_op([(45,65), (45,1)], lambda x,y: x+y)
+    helper_test_op([(45,65), ()], lambda x,y: x+y)
   def test_broadcasted_add_2(self):
-    helper_test_op([(45,65), (65,)], lambda x,y: x+y, lambda x,y: x+y)
+    helper_test_op([(45,65), (65,)], lambda x,y: x+y)
+
   def test_sub(self):
     helper_test_op([(45,65), (45,65)], lambda x,y: x-y, Tensor.sub)
-    helper_test_op([(), ()], lambda x,y: x-y, Tensor.sub)
+    helper_test_op([(45,65), (45,65)], lambda x,y: x-y)
+    helper_test_op([(), ()], lambda x,y: x-y)
+  def test_scalar_sub(self):
+    helper_test_op([(45,65)], lambda x: x-2)
+    helper_test_op([()], lambda x: x-2)
+  def test_scalar_rsub(self):
+    helper_test_op([(45,65)], lambda x: 2-x)
+    helper_test_op([()], lambda x: 2-x)
+
   def test_neg(self):
     helper_test_op([(45,65)], lambda x: -x)
-    helper_test_op([()], lambda x: -x)
+    helper_test_op([(45,65)], lambda x: x.neg())
+    helper_test_op([()], lambda x: x.neg())
+  def test_logical_not(self):
+    helper_test_op(None, torch.logical_not, Tensor.logical_not, vals=[[True, False, True]], forward_only=True)
+    helper_test_op(None, torch.logical_not, Tensor.logical_not, vals=[[1.,2.,0.,0.5]], forward_only=True)
+
   def test_mul(self):
     helper_test_op([(64,64), (64,64)], lambda x,y: x*y, Tensor.mul)
-  def test_mul_number(self):
-    helper_test_op([(), ()], lambda x,y: x*y, Tensor.mul)
-  def test_mul_const(self):
-    helper_test_op([(45,65)], lambda x: x*2, lambda x: x*2)
-    helper_test_op([(45,65)], lambda x: x*-1, lambda x: x*-1)
-    helper_test_op([(45,65)], lambda x: 255*x, lambda x: 255*x)
+    helper_test_op([(64,64), (64,64)], lambda x,y: x*y)
+    helper_test_op([(), ()], lambda x,y: x*y)
+  def test_scalar_mul(self):
+    helper_test_op([(45,65)], lambda x: x*2)
+    helper_test_op([(45,65)], lambda x: x*-1)
+    helper_test_op([(45,65)], lambda x: 255*x)
+    helper_test_op([(45,65)], lambda x: 2*x)
+    helper_test_op([()], lambda x: x*2)
+    helper_test_op([()], lambda x: 2*x)
+
   def test_div(self):
     helper_test_op([(45,65), (45,65)], lambda x,y: x/y, Tensor.div)
-    helper_test_op([(), ()], lambda x,y: x/y, Tensor.div)
-    helper_test_op(None, lambda x,y: x/y, Tensor.div, forward_only=True, vals=np.array([[5],[1]], dtype=np.int32))
+    helper_test_op([(45,65), (45,65)], lambda x,y: x/y)
+    helper_test_op([(), ()], lambda x,y: x/y)
   def test_div_int(self):
-    helper_test_op(None, lambda x: (x/2).to(torch.int), lambda x: x/2, forward_only=True, vals=np.array([[3]], dtype=np.int32))
-  def test_div_const(self):
-    helper_test_op([(45,65)], lambda x: x/255, lambda x: x/255)
-    helper_test_op([(45,65)], lambda x: x/1, lambda x: x/1)
-    helper_test_op([(45,65)], lambda x: 1/x, lambda x: 1/x)
-    helper_test_op([(45,65)], lambda x: x/2, lambda x: x/2)
-    helper_test_op([(45,65)], lambda x: 2/x, lambda x: 2/x)
-    helper_test_op([()], lambda x: x/2, lambda x: x/2)
-    helper_test_op([()], lambda x: 2/x, lambda x: 2/x)
-  @unittest.skipIf(Device.DEFAULT in ["METAL", "WEBGPU"], "METAL has issues with -inf")
-  def test_mul_const_naninf(self):
-    helper_test_op([(45,65)], lambda x: x*float("inf"), lambda x: x*float("inf"))
-    helper_test_op([(45,65)], lambda x: x*-float("inf"), lambda x: x*-float("inf"))
-    helper_test_op([(45,65)], lambda x: x*float("nan"), lambda x: x*float("nan"))
-  @unittest.skipIf(Device.DEFAULT in ["METAL", "WEBGPU"], "METAL has issues with -inf")
-  def test_div_const_naninf(self):
-    helper_test_op([(45,65)], lambda x: x/float("inf"), lambda x: x/float("inf"))
-    helper_test_op([(45,65)], lambda x: x/-float("inf"), lambda x: x/-float("inf"))
-    helper_test_op([(45,65)], lambda x: x/float("nan"), lambda x: x/float("nan"))
-    helper_test_op([(45,65)], lambda x: float("inf")/x, lambda x: float("inf")/x)
-    helper_test_op([(45,65)], lambda x: (-float("inf"))/x, lambda x: (-float("inf"))/x)
-    helper_test_op([(45,65)], lambda x: float("nan")/x, lambda x: float("nan")/x)
+    helper_test_op(None, lambda x,y: x/y, Tensor.div, forward_only=True, vals=np.array([[5, 6, 7],[1, 2, 3]], dtype=np.int32))
+    helper_test_op(None, lambda x: x/2, lambda x: x/2, forward_only=True, vals=np.array([[3, 4, 5]], dtype=np.int32))
+  def test_scalar_div(self):
+    helper_test_op([(45,65)], lambda x: x/255)
+    helper_test_op([(45,65)], lambda x: x/1)
+    helper_test_op([(45,65)], lambda x: 1/x)
+    helper_test_op([(45,65)], lambda x: x/2)
+    helper_test_op([(45,65)], lambda x: 2/x)
+    helper_test_op([()], lambda x: x/2)
+    helper_test_op([()], lambda x: 2/x)
+
+  def test_mul_naninf(self):
+    helper_test_op([(45,65)], lambda x: x*math.inf)
+    helper_test_op([(45,65)], lambda x: x*-math.inf)
+    helper_test_op([(45,65)], lambda x: x*math.nan)
+  def test_div_naninf(self):
+    helper_test_op([(45,65)], lambda x: x/math.inf)
+    helper_test_op([(45,65)], lambda x: x/-math.inf)
+    helper_test_op([(45,65)], lambda x: x/math.nan)
+    helper_test_op([(45,65)], lambda x: math.inf/x)
+    helper_test_op([(45,65)], lambda x: (-math.inf)/x)
+    helper_test_op([(45,65)], lambda x: math.nan/x)
+
   def test_pow_full(self):
-    helper_test_op([(45,65), (45,65)], lambda x,y: x**y, Tensor.pow, a=0)
+    helper_test_op([(45,65), (45,65)], lambda x,y: x**y)
+    helper_test_op([(45,65), (45,65)], lambda x,y: x.pow(y))
   def test_pow(self):
-    # TODO: why is a=0 for these tests?
-    helper_test_op([(45,65)], lambda x: x**0, lambda x: Tensor.pow(x,0), a=0)
-    helper_test_op([(45,65)], lambda x: x**1, lambda x: Tensor.pow(x,1), a=0)
-    helper_test_op([(45,65)], lambda x: x**2, lambda x: Tensor.pow(x,2), a=0)
-    helper_test_op([(45,65)], lambda x: x**3, lambda x: Tensor.pow(x,3), a=0)
-    helper_test_op([(45,65)], lambda x: x**-2, lambda x: Tensor.pow(x,-2), a=0)
-    helper_test_op([()], lambda x: x**2, lambda x: Tensor.pow(x,2), a=0)
-    helper_test_op([()], lambda x: x**-2, lambda x: Tensor.pow(x,-2), a=0)
+    helper_test_op([(45,65)], lambda x: x**0)
+    helper_test_op([(45,65)], lambda x: x**1)
+    helper_test_op([(45,65)], lambda x: x**2)
+    helper_test_op([(45,65)], lambda x: x**3)
+    helper_test_op([(45,65)], lambda x: x**-2)
+    helper_test_op([()], lambda x: x**2)
+    helper_test_op([()], lambda x: x**-2)
     # Regression tests for https://github.com/tinygrad/tinygrad/issues/1151
-    helper_test_op([(45,65)], lambda x: x**3, lambda x: Tensor.pow(x,3), a=-10)
-    helper_test_op([()], lambda x: x**3, lambda x: Tensor.pow(x,3), a=-10)
+    helper_test_op([(45,65)], lambda x: x**3, low=-30, high=-27)
+    helper_test_op([()], lambda x: x**3, low=-30, high=-27)
     # Regression tests for https://github.com/tinygrad/tinygrad/issues/1251
-    helper_test_op([(45,65)], lambda x: x**0.2, lambda x: Tensor.pow(x,0.2), a=-10)
-    helper_test_op([(45,65)], lambda x: x**1.2, lambda x: Tensor.pow(x,1.2), a=-10)
-    helper_test_op([()], lambda x: x**0.2, lambda x: Tensor.pow(x,0.2), a=-10)
-    helper_test_op([()], lambda x: x**1.2, lambda x: Tensor.pow(x,1.2), a=-10)
+    helper_test_op([(45,65)], lambda x: x**0.2, low=-30, high=-27)
+    helper_test_op([(45,65)], lambda x: x**1.2, low=-30, high=-27)
+    helper_test_op([()], lambda x: x**0.2, low=-30, high=-27)
+    helper_test_op([()], lambda x: x**1.2, low=-30, high=-27)
     a, b = Tensor([0.0], requires_grad=True), torch.tensor([0.0], requires_grad=True)
-    helper_test_op([], lambda: b**1.1, lambda: a**1.1, )
+    helper_test_op([], lambda: b**1.1, lambda: a**1.1)
   def test_pow_const(self):
-    helper_test_op([(45,65)], lambda x: x**1.0, lambda x: x**1.0)
-    helper_test_op([(45,65)], lambda x: x**-1.0, lambda x: x**-1.0)
-    helper_test_op([(45,65)], lambda x: 1.0**x, lambda x: 1.0**x)
-    helper_test_op([(45,65)], lambda x: x**2.0, lambda x: x**2.0)
-    helper_test_op([(45,65)], lambda x: 2.0**x, lambda x: 2.0**x)
-    helper_test_op([()], lambda x: x**2.0, lambda x: x**2.0)
-    helper_test_op([()], lambda x: 2.0**x, lambda x: 2.0**x)
+    helper_test_op([(45,65)], lambda x: x**1.0)
+    helper_test_op([(45,65)], lambda x: x**-1.0)
+    helper_test_op([(45,65)], lambda x: 1.0**x)
+    helper_test_op([(45,65)], lambda x: x**2.0)
+    helper_test_op([(45,65)], lambda x: 2.0**x)
+    helper_test_op([()], lambda x: x**2.0)
+    helper_test_op([()], lambda x: 2.0**x)
+    # TODO: fix backward
+    helper_test_op(None, lambda x: 0**x, vals=[[-2.,-1,0,1,2,3]], forward_only=True)
+    # TODO: fix backward, should be nan
+    helper_test_op(None, lambda x: (-2)**x, vals=[[-2.,-1,0,1,2,3]], forward_only=True)
+
   def test_sqrt(self):
-    helper_test_op([(45,65)], lambda x: x.sqrt(), Tensor.sqrt, a=0)
-    helper_test_op([()], lambda x: x.sqrt(), Tensor.sqrt, a=0)
+    helper_test_op([(45,65)], lambda x: x.sqrt())
+    helper_test_op([()], lambda x: x.sqrt())
   def test_rsqrt(self):
-    helper_test_op([(45,65)], lambda x: torch.rsqrt(x), Tensor.rsqrt, a=0)
-    helper_test_op([()], lambda x: torch.rsqrt(x), Tensor.rsqrt, a=0)
+    helper_test_op([(45,65)], lambda x: x.rsqrt())
+    helper_test_op([()], lambda x: x.rsqrt())
+
   def test_xor(self):
     tor = torch.tensor([[1,-8,1],[32,1,6]], dtype=torch.int)
     ten = Tensor([[1,-8,1],[32,1,6]], dtype=dtypes.int32)
     helper_test_op([], lambda: tor^tor, lambda: ten^ten, forward_only=True)
     helper_test_op([], lambda: tor^0x1337, lambda: ten^0x1337, forward_only=True)
     helper_test_op([], lambda: 0x1337^tor, lambda: 0x1337^ten, forward_only=True)
 
+  def test_lshift(self):
+    data = [[0,1,2],[1<<8,1<<16,1<<31-1]]
+    tor = torch.tensor(data, dtype=torch.int)
+    ten = Tensor(data, dtype=dtypes.uint32)
+    # cast to int32 because torch does not support uint32
+    helper_test_op([], lambda: tor << 0, lambda: (ten << 0).cast(dtypes.int32), forward_only=True)
+    helper_test_op([], lambda: tor << 2, lambda: (ten << 2).cast(dtypes.int32), forward_only=True)
+    helper_test_op([], lambda: tor << 31, lambda: (ten << 31).cast(dtypes.int32), forward_only=True)
+    helper_test_op([], lambda: tor.__lshift__(2), lambda: ten.__lshift__(2).cast(dtypes.int32), forward_only=True)
+    helper_test_op([], lambda: tor.bitwise_left_shift(2), lambda: ten.lshift(2).cast(dtypes.int32), forward_only=True)
+
+  def test_rshift(self):
+    data = [[0,1,2],[1<<8,1<<16,1<<31-1]]
+    tor = torch.tensor(data, dtype=torch.int)
+    ten = Tensor(data, dtype=dtypes.uint32)
+    # cast to int32 because torch does not support uint32
+    helper_test_op([], lambda: tor >> 0, lambda: (ten >> 0).cast(dtypes.int32), forward_only=True)
+    helper_test_op([], lambda: tor >> 2, lambda: (ten >> 2).cast(dtypes.int32), forward_only=True)
+    helper_test_op([], lambda: tor >> 31, lambda: (ten >> 31).cast(dtypes.int32), forward_only=True)
+    helper_test_op([], lambda: tor.__rshift__(2), lambda: ten.__rshift__(2).cast(dtypes.int32), forward_only=True)
+    helper_test_op([], lambda: tor.bitwise_right_shift(2), lambda: ten.rshift(2).cast(dtypes.int32), forward_only=True)
+
   def test_sin(self):
-    helper_test_op([(45,65)], lambda x: x.sin(), Tensor.sin, a=0)
+    helper_test_op([(45,65)], lambda x: x.sin())
+    helper_test_op([()], lambda x: x.sin())
   def test_cos(self):
-    helper_test_op([(45,65)], lambda x: x.cos(), Tensor.cos, a=0)
+    helper_test_op([(45,65)], lambda x: x.cos())
+    helper_test_op([()], lambda x: x.cos())
   def test_tan(self):
-    helper_test_op([(45,65)], lambda x: x.tan(), Tensor.tan, a=0)
+    helper_test_op([(45,65)], lambda x: x.tan())
+    helper_test_op([()], lambda x: x.tan())
 
   def test_relu(self):
-    helper_test_op([(64,64)], lambda x: x.relu(), Tensor.relu)
-    helper_test_op([()], lambda x: x.relu(), Tensor.relu)
+    helper_test_op([(64,64)], lambda x: x.relu())
+    helper_test_op([()], lambda x: x.relu())
   def test_relu_exact(self):
-    helper_test_op(None, lambda x: x.relu(), Tensor.relu, vals=[[-1.,0,1]])
+    helper_test_op(None, lambda x: x.relu(), vals=[[-1.,0,1]])
   def test_relu_maximum_exact(self):
     helper_test_op(None, lambda x: torch.maximum(x, torch.zeros_like(x, requires_grad=False)), lambda x: Tensor.maximum(x, 0), vals=[[-1.,0,1]])
   def test_leakyrelu(self):
     helper_test_op([(45,65)], lambda x: torch.nn.functional.leaky_relu(x,0.01), Tensor.leakyrelu)
     helper_test_op([()], lambda x: torch.nn.functional.leaky_relu(x,0.01), Tensor.leakyrelu)
   def test_celu(self):
     for val in range(1, 5):
       helper_test_op([(45,65)], lambda x: torch.nn.functional.celu(x,val), lambda x: x.celu(val))
       helper_test_op([()], lambda x: torch.nn.functional.celu(x,val), lambda x: x.celu(val))
+
   def test_abs(self):
-    helper_test_op([(45,65)], lambda x: torch.abs(x), Tensor.abs)
-    helper_test_op([()], lambda x: torch.abs(x), Tensor.abs)
+    helper_test_op([(45,65)], torch.abs, Tensor.abs)
+    helper_test_op([()], torch.abs, Tensor.abs)
+  def test_abs_exact(self):
+    helper_test_op(None, torch.abs, Tensor.abs, vals=[[-1.,0,1]])
+
   def test_log(self):
-    helper_test_op([(45,65)], lambda x: torch.log(x), Tensor.log)
-    helper_test_op([()], lambda x: torch.log(x), Tensor.log)
+    helper_test_op([(45,65)], torch.log, Tensor.log)
+    helper_test_op([()], torch.log, Tensor.log)
   def test_log2(self):
-    helper_test_op([(45,65)], lambda x: torch.log2(x), Tensor.log2)
-    helper_test_op([()], lambda x: torch.log2(x), Tensor.log2)
+    helper_test_op([(45,65)], torch.log2, Tensor.log2)
+    helper_test_op([()], torch.log2, Tensor.log2)
+
   def test_exp(self):
-    helper_test_op([(45,65)], lambda x: torch.exp(x), Tensor.exp)
-    helper_test_op([()], lambda x: torch.exp(x), Tensor.exp)
+    helper_test_op([(45,65)], torch.exp, Tensor.exp)
+    helper_test_op([()], torch.exp, Tensor.exp)
   def test_exp2(self):
-    helper_test_op([(45,65)], lambda x: torch.exp2(x), Tensor.exp2)
-    helper_test_op([()], lambda x: torch.exp2(x), Tensor.exp2)
+    helper_test_op([(45,65)], torch.exp2, Tensor.exp2)
+    helper_test_op([()], torch.exp2, Tensor.exp2)
+
   def test_sign(self):
-    helper_test_op([(45,65)], lambda x: torch.sign(x), Tensor.sign)
-    helper_test_op([()], lambda x: torch.sign(x), Tensor.sign)
+    helper_test_op([(45,65)], torch.sign, Tensor.sign)
+    helper_test_op([()], torch.sign, Tensor.sign)
+  def test_sign_exact(self):
+    helper_test_op(None, torch.sign, Tensor.sign, vals=[[-1.,0,1]])
+
   def test_softsign(self):
-    helper_test_op([(45,65)], lambda x: torch.nn.functional.softsign(x), Tensor.softsign)
-    helper_test_op([()], lambda x: torch.nn.functional.softsign(x), Tensor.softsign)
+    helper_test_op([(45,65)], torch.nn.functional.softsign, Tensor.softsign)
+    helper_test_op([()], torch.nn.functional.softsign, Tensor.softsign)
+  def test_softsign_exact(self):
+    helper_test_op(None, torch.nn.functional.softsign, Tensor.softsign, vals=[[-1.,0,1]])
+
   def test_sigmoid(self):
-    helper_test_op([(45,65)], lambda x: x.sigmoid(), Tensor.sigmoid)
-    helper_test_op([(45,65)], lambda x: x.sigmoid(), Tensor.sigmoid, a=100)
-    helper_test_op([(45,65)], lambda x: x.sigmoid(), Tensor.sigmoid, a=-100)
-    helper_test_op([()], lambda x: x.sigmoid(), Tensor.sigmoid, forward_only=True)
+    helper_test_op([(45,65)], torch.sigmoid, Tensor.sigmoid)
+    helper_test_op([(45,65)], torch.sigmoid, Tensor.sigmoid, low=300, high=303)
+    helper_test_op([(45,65)], torch.sigmoid, Tensor.sigmoid, low=-300, high=-297)
+    helper_test_op([()], torch.sigmoid, Tensor.sigmoid)
   def test_softplus(self):
-    helper_test_op([(45,65)], lambda x: torch.nn.functional.softplus(x), Tensor.softplus, atol=1e-6, grad_atol=1e-6)
-    helper_test_op([()], lambda x: torch.nn.functional.softplus(x), Tensor.softplus, atol=1e-6, grad_atol=1e-6)
+    helper_test_op([(45,65)], torch.nn.functional.softplus, Tensor.softplus, grad_atol=1e-6)
+    helper_test_op([()], torch.nn.functional.softplus, Tensor.softplus, grad_atol=1e-6)
+
   def test_gelu(self):
     helper_test_op([(45,65)], lambda x: torch.nn.functional.gelu(x, approximate="tanh"), Tensor.gelu)
-    #helper_test_op([(45,65)], lambda x: torch.nn.functional.gelu(x, approximate="tanh"), Tensor.gelu, a=100)
-    helper_test_op([(45,65)], lambda x: torch.nn.functional.gelu(x, approximate="tanh"), Tensor.gelu, a=-100)
+    helper_test_op([(45,65)], lambda x: torch.nn.functional.gelu(x, approximate="tanh"), Tensor.gelu, low=300, high=303)
+    helper_test_op([(45,65)], lambda x: torch.nn.functional.gelu(x, approximate="tanh"), Tensor.gelu, low=-300, high=-297)
   def test_quick_gelu(self):
     helper_test_op([(45,65)], lambda x: x * torch.sigmoid(1.702 * x), Tensor.quick_gelu)
-    helper_test_op([(45,65)], lambda x: x * torch.sigmoid(1.702 * x), Tensor.quick_gelu, a=100)
-    helper_test_op([(45,65)], lambda x: x * torch.sigmoid(1.702 * x), Tensor.quick_gelu, a=-100)
+    helper_test_op([(45,65)], lambda x: x * torch.sigmoid(1.702 * x), Tensor.quick_gelu, low=300, high=303)
+    helper_test_op([(45,65)], lambda x: x * torch.sigmoid(1.702 * x), Tensor.quick_gelu, low=-300, high=-297)
     helper_test_op([()], lambda x: x * torch.sigmoid(1.702 * x), Tensor.quick_gelu)
+
   def test_elu(self):
-    helper_test_op([(45,65)], lambda x: torch.nn.functional.elu(x), Tensor.elu)
+    helper_test_op([(45,65)], torch.nn.functional.elu, Tensor.elu)
     helper_test_op([(45,65)], lambda x: torch.nn.functional.elu(x, alpha=0.1), lambda x: Tensor.elu(x, alpha=0.1))
-    helper_test_op([()], lambda x: torch.nn.functional.elu(x), Tensor.elu)
+    helper_test_op([()], torch.nn.functional.elu, Tensor.elu)
   def test_relu6(self):
-    helper_test_op([(45,65)], lambda x: torch.nn.functional.relu6(x), Tensor.relu6)
-    helper_test_op([()], lambda x: torch.nn.functional.relu6(x), Tensor.relu6)
+    helper_test_op([(45,65)], torch.nn.functional.relu6, Tensor.relu6)
+    helper_test_op([()], torch.nn.functional.relu6, Tensor.relu6)
   def test_hardswish(self):
-    helper_test_op([(45,65)], lambda x: torch.nn.functional.hardswish(x), Tensor.hardswish, atol=1e-6, grad_atol=1e-6)
-    helper_test_op([()], lambda x: torch.nn.functional.hardswish(x), Tensor.hardswish, atol=1e-6, grad_atol=1e-6)
+    helper_test_op([(45,65)], torch.nn.functional.hardswish, Tensor.hardswish, grad_atol=1e-6)
+    helper_test_op([()], torch.nn.functional.hardswish, Tensor.hardswish, grad_atol=1e-6)
   def test_mish(self):
-    def _mish_pytorch(x):
-      return x*torch.tanh(torch.nn.functional.softplus(x))
-    helper_test_op([(45,65)], _mish_pytorch, Tensor.mish, atol=1e-4)
-    helper_test_op([()], _mish_pytorch, Tensor.mish, atol=1e-4)
-  @unittest.skipIf(IMAGE>0, "no 1d dot for images")
-  def test_dot_1d(self):
-    helper_test_op([(65), (65)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-4)
-    helper_test_op([(65), (65,45)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-4)
-    helper_test_op([(45,65), (65)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-4)
-    helper_test_op([(8,45,65), (65)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-4)
-    helper_test_op([(65), (8,65,45)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-4)
-    self.helper_test_exception([(4), (1,2)], lambda x, y: x.matmul(y), Tensor.dot, expected=(RuntimeError, AssertionError))
-    self.helper_test_exception([(2,1), (4)], lambda x, y: x.matmul(y), Tensor.dot, expected=(RuntimeError, AssertionError))
-    self.helper_test_exception([(1), (4)], lambda x, y: x.matmul(y), Tensor.dot, expected=(RuntimeError, AssertionError))
-  def test_dot(self):
-    helper_test_op([(45,65), (65,100)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-4)
-    helper_test_op([(8,45,65), (8,65,100)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-4)
-    self.helper_test_exception([(2, 4), (1, 3)], lambda x, y: x.matmul(y), Tensor.dot, expected=(RuntimeError, AssertionError))
-    self.helper_test_exception([(2, 1), (4, 3)], lambda x, y: x.matmul(y), Tensor.dot, expected=(RuntimeError, AssertionError))
-    with self.assertRaises(AssertionError):
-      a = Tensor(3.14)
-      a.matmul(a)
+    helper_test_op([(45,65)], torch.nn.functional.mish, Tensor.mish)
+    helper_test_op([()], torch.nn.functional.mish, Tensor.mish)
 
   def test_multinomial(self):
     # NOTE: this is random, so it has a very large atol
-    helper_test_op([(1000,)], lambda x: torch.multinomial(x.clip(0,1), num_samples=1),
+    helper_test_op([(1000,)], lambda x: torch.multinomial(x.clip(0,1), num_samples=1).type(torch.int32),
                               lambda x: Tensor.multinomial(x.clip(0,1)), forward_only=True, atol=1000.)
 
   def test_small_cumsum(self):
-    helper_test_op([(10)], lambda x: torch.cumsum(x, dim=0), lambda x: Tensor.cumsum(x, axis=0), atol=1e-6)
+    helper_test_op([(10)], lambda x: torch.cumsum(x, dim=0), lambda x: Tensor.cumsum(x, axis=0))
   def test_simple_cumsum(self):
-    helper_test_op([(512)], lambda x: torch.cumsum(x, dim=0), lambda x: Tensor.cumsum(x, axis=0), atol=1e-6)
-    helper_test_op([(1022)], lambda x: torch.cumsum(x, dim=0), lambda x: Tensor.cumsum(x, axis=0), atol=1e-6)
+    helper_test_op([(512)], lambda x: torch.cumsum(x, dim=0), lambda x: Tensor.cumsum(x, axis=0))
+    helper_test_op([(1022)], lambda x: torch.cumsum(x, dim=0), lambda x: Tensor.cumsum(x, axis=0))
   def test_cumsum(self):
-    helper_test_op([(20)], lambda x: torch.cumsum(x, dim=0), lambda x: Tensor.cumsum(x, axis=0), atol=1e-6)
-    helper_test_op([(20,30)], lambda x: torch.cumsum(x, dim=0), lambda x: Tensor.cumsum(x, axis=0), atol=1e-6)
-    helper_test_op([(20,30)], lambda x: torch.cumsum(x, dim=1), lambda x: Tensor.cumsum(x, axis=1), atol=1e-6)
-    helper_test_op([(20,30,40)], lambda x: torch.cumsum(x, dim=2), lambda x: Tensor.cumsum(x, axis=2), atol=1e-6)
-    helper_test_op([(20,30,40)], lambda x: torch.cumsum(x, dim=-1), lambda x: Tensor.cumsum(x, axis=-1), atol=1e-6)
+    helper_test_op([(20)], lambda x: torch.cumsum(x, dim=0), lambda x: Tensor.cumsum(x, axis=0))
+    helper_test_op([(20,30)], lambda x: torch.cumsum(x, dim=0), lambda x: Tensor.cumsum(x, axis=0))
+    helper_test_op([(20,30)], lambda x: torch.cumsum(x, dim=1), lambda x: Tensor.cumsum(x, axis=1))
+    helper_test_op([(20,30,40)], lambda x: torch.cumsum(x, dim=2), lambda x: Tensor.cumsum(x, axis=2))
+    helper_test_op([(20,30,40)], lambda x: torch.cumsum(x, dim=-1), lambda x: Tensor.cumsum(x, axis=-1))
+  def test_cumsum_zero_axis(self):
+    helper_test_op([(2,0,4)], lambda x: torch.cumsum(x, dim=1), lambda x: Tensor.cumsum(x, axis=1))
+    helper_test_op([(0,3)], lambda x: torch.cumsum(x, dim=0), lambda x: Tensor.cumsum(x, axis=0))
+    helper_test_op([(2,3,0)], lambda x: torch.cumsum(x, dim=2), lambda x: Tensor.cumsum(x, axis=2))
 
   def test_argmax(self):
-    self.assertEqual(torch.Tensor([2,2]).argmax().numpy(), Tensor([2,2]).argmax().numpy()) # check if returns first index for same max
-    helper_test_op([(10,20)], lambda x: x.argmax(), lambda x: x.argmax(), forward_only=True)
-    helper_test_op([(10,20)], lambda x: x.argmax(0, False), lambda x: x.argmax(0, False), forward_only=True)
-    helper_test_op([(10,20)], lambda x: x.argmax(1, False), lambda x: x.argmax(1, False), forward_only=True)
-    helper_test_op([(10,20)], lambda x: x.argmax(1, True), lambda x: x.argmax(1, True), forward_only=True)
+    # check if it returns the first index for multiple occurences
+    self.assertEqual(torch.tensor([2,2]).argmax().numpy(), Tensor([2,2]).argmax().numpy())
+    np.testing.assert_equal(Tensor([2,2]).argmax().numpy(), np.array(0))
+    np.testing.assert_equal(Tensor([1,2,2]).argmax().numpy(), np.array(1))
+    helper_test_op([(10,20)], lambda x: x.argmax().type(torch.int32), lambda x: x.argmax(), forward_only=True)
+    helper_test_op([(10,20)], lambda x: x.argmax(0, False).type(torch.int32), lambda x: x.argmax(0, False), forward_only=True)
+    helper_test_op([(10,20)], lambda x: x.argmax(1, False).type(torch.int32), lambda x: x.argmax(1, False), forward_only=True)
+    helper_test_op([(10,20)], lambda x: x.argmax(1, True).type(torch.int32), lambda x: x.argmax(1, True), forward_only=True)
 
   def test_argmin(self):
-    self.assertEqual(torch.Tensor([2, 2]).argmin().numpy(), Tensor([2, 2]).argmin().numpy())
-    helper_test_op([(10,20)], lambda x: x.argmin(), lambda x: x.argmin(), forward_only=True)
-    helper_test_op([(10,20)], lambda x: x.argmin(0, False), lambda x: x.argmin(0, False), forward_only=True)
-    helper_test_op([(10,20)], lambda x: x.argmin(1, False), lambda x: x.argmin(1, False), forward_only=True)
-    helper_test_op([(10,20)], lambda x: x.argmin(1, True), lambda x: x.argmin(1, True), forward_only=True)
+    # check if it returns the first index for multiple occurences
+    self.assertEqual(torch.tensor([2, 2]).argmin().numpy(), Tensor([2, 2]).argmin().numpy())
+    np.testing.assert_equal(Tensor([2,2]).argmin().numpy(), np.array(0))
+    np.testing.assert_equal(Tensor([3,2,2]).argmin().numpy(), np.array(1))
+    helper_test_op([(10,20)], lambda x: x.argmin().type(torch.int32), lambda x: x.argmin(), forward_only=True)
+    helper_test_op([(10,20)], lambda x: x.argmin(0, False).type(torch.int32), lambda x: x.argmin(0, False), forward_only=True)
+    helper_test_op([(10,20)], lambda x: x.argmin(1, False).type(torch.int32), lambda x: x.argmin(1, False), forward_only=True)
+    helper_test_op([(10,20)], lambda x: x.argmin(1, True).type(torch.int32), lambda x: x.argmin(1, True), forward_only=True)
 
   def test_einsum(self):
     # matrix transpose
     helper_test_op([(150,150)], lambda a: torch.einsum('ij->ji', a), lambda a: Tensor.einsum('ij->ji', a))
     helper_test_op([(150,150)], lambda a: torch.einsum('ij -> ji', a), lambda a: Tensor.einsum('ij -> ji', a))
     helper_test_op([(150,150)], lambda a: torch.einsum('ji', a), lambda a: Tensor.einsum('ji', a))
     helper_test_op([(20,30,40)], lambda a: torch.einsum('jki', a), lambda a: Tensor.einsum('jki', a))
@@ -493,32 +604,39 @@
     helper_test_op([(50,50)], lambda a: torch.einsum('ij->j', a), lambda a: Tensor.einsum('ij->j', a))
     # row sum
     helper_test_op([(15,15)], lambda a: torch.einsum('ij->i', a), lambda a: Tensor.einsum('ij->i', a))
     # matrix-vector multiplication
     helper_test_op([(15,20), (20,)], lambda a,b: torch.einsum('ik,k->i', a,b), lambda a,b: Tensor.einsum('ik,k->i', a, b))
     # matrix-matrix multiplication
     helper_test_op([(15,20), (20,30)], lambda a,b: torch.einsum('ik,kj->ij', a,b), lambda a,b: Tensor.einsum('ik,kj->ij', a, b))
+    # matrix-matrix multiplication, different letter order
+    helper_test_op([(15,20), (20,30)], lambda a,b: torch.einsum('jk,ki->ji', a,b), lambda a,b: Tensor.einsum('jk,ki->ji', a, b))
     # dot product
     helper_test_op([(30),(30)], lambda a,b: torch.einsum('i,i->i', [a,b]), lambda a,b: Tensor.einsum('i,i->i', [a,b]))
     # hadamard product
     helper_test_op([(30,40),(30,40)], lambda a,b: torch.einsum('ij,ij->ij', a,b), lambda a,b: Tensor.einsum('ij,ij->ij', a,b))
     # outer product
     helper_test_op([(15,), (15,)], lambda a,b: torch.einsum('i,j->ij', a,b), lambda a,b: Tensor.einsum('i,j->ij',a,b))
     # batch matrix multiplication
     helper_test_op([(10,20,30),(10,30,40)], lambda a,b: torch.einsum('ijk,ikl->ijl', [a, b]), lambda a,b: Tensor.einsum('ijk,ikl->ijl', [a, b]))
     # batch matrix multiplication, result permuted
     helper_test_op([(10,20,25),(10,25,32)], lambda a,b: torch.einsum('ijk,ikl->jil', [a, b]), lambda a,b: Tensor.einsum('ijk,ikl->jil', [a, b]))
     # batch matrix multiplication, result & input permuted
     helper_test_op([(20,10,25),(10,25,32)], lambda a,b: torch.einsum('jik,ikl->jil', [a, b]), lambda a,b: Tensor.einsum('jik,ikl->jil', [a, b]))
+    # batch matrix multiplication, result with different letters
+    helper_test_op([(10,20,30),(10,30,40)], lambda a,b: torch.einsum('ijk,ika->ija', [a, b]), lambda a,b: Tensor.einsum('ijk,ika->ija', [a, b]))
     # tensor contraction
     helper_test_op([(3,5,8,10),(11,13,5,16,8)], lambda a,b: torch.einsum('pqrs,tuqvr->pstuv', a,b),
                                                 lambda a,b: Tensor.einsum('pqrs,tuqvr->pstuv', a,b), atol=1e-5)
     # tensor contraction, input permuted
     helper_test_op([(3,8,10,5),(11,5,13,16,8)], lambda a,b: torch.einsum('prsq,tquvr->pstuv', a,b),
                                                 lambda a,b: Tensor.einsum('prsq,tquvr->pstuv', a,b), atol=1e-5)
+    # tensor contraction, result with different letters
+    helper_test_op([(3,5,8,10),(11,13,5,16,8)], lambda a,b: torch.einsum('zqrs,tuqvr->zstuv', a,b),
+                                                lambda a,b: Tensor.einsum('zqrs,tuqvr->zstuv', a,b), atol=1e-5)
     # bilinear transformation
     helper_test_op([(2,3),(5,3,7),(2,7)], lambda a,b,c: torch.einsum('ik,jkl,il->ij', [a,b,c]), lambda a,b,c: Tensor.einsum('ik,jkl,il->ij', [a,b,c]))
 
   def test_einsum_shape_check(self):
     a = Tensor.zeros(3,8,10,5)
     b = Tensor.zeros(11,5,13,16,8)
     with self.assertRaises(AssertionError):
@@ -532,247 +650,370 @@
       Tensor.einsum('ij,jk->ij', a,b,c)
 
   def test_einsum_arity_check2(self):
     a = Tensor.zeros(10,10)
     with self.assertRaises(AssertionError):
       Tensor.einsum('ij,jk->ij', a)
 
+  @unittest.skipIf(IMAGE>0, "no 1d dot for images")
+  def test_dot_1d(self):
+    helper_test_op([(65), (65)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-4)
+    helper_test_op([(65), (65,45)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-4)
+    helper_test_op([(45,65), (65)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-4)
+    helper_test_op([(8,45,65), (65)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-4)
+    helper_test_op([(65), (8,65,45)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-4)
+    self.helper_test_exception([(4), (1,2)], lambda x, y: x.matmul(y), Tensor.dot, expected=(RuntimeError, AssertionError))
+    self.helper_test_exception([(2,1), (4)], lambda x, y: x.matmul(y), Tensor.dot, expected=(RuntimeError, AssertionError))
+    self.helper_test_exception([(1), (4)], lambda x, y: x.matmul(y), Tensor.dot, expected=(RuntimeError, AssertionError))
+  def test_dot(self):
+    helper_test_op([(45,65), (65,100)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-4)
+    helper_test_op([(8,45,65), (8,65,100)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-4)
+    self.helper_test_exception([(2, 4), (1, 3)], lambda x, y: x.matmul(y), Tensor.dot, expected=(RuntimeError, AssertionError))
+    self.helper_test_exception([(2, 1), (4, 3)], lambda x, y: x.matmul(y), Tensor.dot, expected=(RuntimeError, AssertionError))
+    with self.assertRaises(AssertionError):
+      a = Tensor(3.14)
+      a.matmul(a)
+  def test_mulacc_with_zero_strides(self):
+    helper_test_op(
+      [],
+      lambda: torch.tensor(1.0).reshape((1,1,1)).expand(2,4,3).mul(torch.tensor(1.0).reshape((1,1,1)).expand(2,4,3)).sum(-1),
+      lambda: Tensor(1.0).reshape((1,1,1)).expand(2,4,3).mul(Tensor(1.0).reshape((1,1,1)).expand(2,4,3)).sum(-1),
+      forward_only=True
+    )
+    a = [[1.,1.,1.,1.], [1.,1.,1.,1.]]
+    b = [1.,1.,1.,1.]
+    helper_test_op(
+      [],
+      lambda: torch.tensor(a).reshape((2,4,1)).expand(2,4,3).mul(torch.tensor(b).reshape((1,4,1)).expand(2,4,3)).sum([0,2]),
+      lambda: Tensor(a).reshape((2,4,1)).expand(2,4,3).mul(Tensor(b).reshape((1,4,1)).expand(2,4,3)).sum([0,2]),
+      forward_only=True
+    )
+    helper_test_op(
+      [],
+      lambda: torch.ones((1,2)).matmul(torch.ones((2,3))), lambda: Tensor.ones((1,2)).dot(Tensor.ones((2,3))),
+      forward_only=True
+    )
+
   def test_matmul_simple(self):
     helper_test_op([(4), (4,4)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-4)
   def test_matmul(self):
     helper_test_op([(64), (64,99)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-4)
 
   @unittest.skipIf(IMAGE>0, "no batched matmul on images")
   def test_matmul_batched(self):
     helper_test_op([(3), (1,3,3,5)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-4)
 
   @unittest.skipIf(IMAGE>0, "no batched matmul on images")
   def test_matmul_batched_vector(self):
     helper_test_op([(4,3), (1,3,3,5)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-4)
   def test_small_gemm(self):
     helper_test_op([(8,8), (8,8)], lambda x,y: x.matmul(y), lambda x,y: x@y, atol=1e-3)
+  def test_small_gemm_range(self):
+    helper_test_op(None, lambda x,y: x.matmul(y), lambda x,y: x@y, atol=1e-3, vals=[np.arange(0,64,dtype=np.float32).reshape(8,8),
+                                                                                    np.arange(64,128,dtype=np.float32).reshape(8,8)])
   def test_small_gemm_eye(self):
     helper_test_op(None, lambda x,y: x.matmul(y), lambda x,y: x@y, atol=1e-3, vals=[np.eye(8).astype(np.float32), np.eye(8).astype(np.float32)])
   def test_gemm(self):
     helper_test_op([(64,64), (64,64)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-3)
   def test_big_gemm(self):
     helper_test_op([(256,256), (256,256)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-3)
+  @unittest.skipIf(IMAGE>0, "no 0 in shape matmul on images")
+  def test_gemm_with_zeros_shape(self):
+    helper_test_op([(8,8), (8,0)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-7)
+    helper_test_op([(0,8), (8,8)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-7)
+    helper_test_op([(0,8), (8,0)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-7)
+    helper_test_op([(8,0), (0,8)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-7)
+    helper_test_op([(0,0), (0,0)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-7)
+    helper_test_op([(0), (0,8)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-7)
+    helper_test_op([(0), (0)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-7)
   def test_broadcastdot(self):
     helper_test_op([(10,45,65), (65,45)], lambda x,y: x @ y, Tensor.dot, atol=1e-4)
     with self.assertRaises(AssertionError):
       a = Tensor(3.14)
       b = Tensor.ones(3,3)
       a @ b
   def test_multidot(self):
     helper_test_op([(10,45,65), (10,65,45)], lambda x,y: x @ y, Tensor.dot, atol=1e-4)
     helper_test_op([(3,3,45,65), (3,3,65,45)], lambda x,y: x @ y, Tensor.dot, atol=1e-4)
+
   def test_sum_simple(self):
-    helper_test_op(None, lambda x: x.sum(), Tensor.sum, vals=[[1.,1.]])
+    helper_test_op(None, lambda x: x.sum(), vals=[[1.,1.]])
   def test_sum_full(self):
-    helper_test_op([(16384)], lambda x: x.sum(), lambda x: x.sum())
-  def test_sum_small_full(self):
-    helper_test_op([(45,5)], lambda x: x.sum(), Tensor.sum)
+    helper_test_op([(16384)], lambda x: x.sum())
   def test_sum_relu(self):
-    helper_test_op([(3,4,5)], lambda x: x.relu().sum().relu(), lambda x: x.relu().sum().relu())
+    helper_test_op([(3,4,5)], lambda x: x.relu().sum().relu())
+  def test_sum_tiny(self):
+    helper_test_op([(4,2,2)], lambda x: x.sum(axis=(0,2)))
   def test_sum(self):
-    helper_test_op([(45,3)], lambda x: x.sum(), Tensor.sum)
-    helper_test_op([(3,4,5,6)], lambda x: x.sum(axis=3), lambda x: Tensor.sum(x, axis=3))
-    helper_test_op([(3,4,5,6)], lambda x: x.sum(axis=(1,3)), lambda x: Tensor.sum(x, axis=(1,3)))
-    helper_test_op([(3,4,5,6)], lambda x: x.sum(axis=(0,2)), lambda x: Tensor.sum(x, axis=(0,2)))
-    helper_test_op([(3,4,5,6)], lambda x: x.sum(axis=(1,2)), lambda x: Tensor.sum(x, axis=(1,2)))
-    helper_test_op([(3,4,5,6)], lambda x: x.sum(axis=1), lambda x: Tensor.sum(x, axis=1))
+    helper_test_op([(45,3)], lambda x: x.sum())
+    helper_test_op([(3,4,5,6)], lambda x: x.sum(axis=3))
+    helper_test_op([(3,4,5,6)], lambda x: x.sum(axis=(1,3)))
+    helper_test_op([(3,4,5,6)], lambda x: x.sum(axis=(0,2)))
+    helper_test_op([(3,4,5,6)], lambda x: x.sum(axis=(1,2)))
+    helper_test_op([(3,4,5,6)], lambda x: x.sum(axis=1))
     helper_test_op([()], lambda x: x.sum(), Tensor.sum)
+  def test_sum_with_zeros_shape(self):
+    helper_test_op([(4, 0)], lambda x: x.sum(axis=(0,)))
+    helper_test_op([(4, 0)], lambda x: x.sum(axis=(1,)))
+    helper_test_op([(4, 0)], lambda x: x.sum(axis=(0,1)))
+
   def test_min(self):
-    helper_test_op([(3,3)], lambda x: x.min(), Tensor.min)
-    helper_test_op([(45,3)], lambda x: x.min(), Tensor.min)
-    helper_test_op([(45,3)], lambda x: x.min().mul(0.5), lambda x: Tensor.min(x).mul(0.5))
-    helper_test_op([()], lambda x: x.min(), Tensor.min)
+    helper_test_op([(3,3)], lambda x: x.min())
+    helper_test_op([(45,3)], lambda x: x.min())
+    helper_test_op([(45,3)], lambda x: x.min().mul(0.5))
+    helper_test_op([()], lambda x: x.min())
   def test_max(self):
-    helper_test_op([(45,3)], lambda x: x.max(), Tensor.max)
-    helper_test_op([(45,3)], lambda x: x.max().mul(0.5), lambda x: Tensor.max(x).mul(0.5))
-    helper_test_op(None, lambda x: x.max().mul(0.5), lambda x: Tensor.max(x).mul(0.5),
-            vals=[
-                [[1.0,1.0,0.0,1.0]],
-                ])
-    helper_test_op([(3,4,5,6)], lambda x: x.max(axis=1)[0], lambda x: Tensor.max(x, axis=1))
-    helper_test_op([()], lambda x: x.max(), Tensor.max)
+    helper_test_op([(45,3)], lambda x: x.max())
+    helper_test_op([(45,3)], lambda x: x.max().mul(0.5))
+    helper_test_op(None, lambda x: x.max().mul(0.5), vals=[[[1.0,1.0,0.0,1.0]],])
+    helper_test_op([(3,4,5,6)], lambda x: x.max(axis=1)[0], lambda x: x.max(axis=1))
+    helper_test_op([()], lambda x: x.max())
+
   def test_mean(self):
     helper_test_op([(3,4,5,6)], lambda x: x.mean())
     helper_test_op([()], lambda x: x.mean())
   def test_mean_axis(self):
-    helper_test_op([(3,4,5,6)], lambda x: x.mean(axis=(1,2)), lambda x: Tensor.mean(x, axis=(1,2)))
-  @unittest.skipIf(Device.DEFAULT == "WEBGL" and CI, "Only broken on CI")
+    helper_test_op([(3,4,5,6)], lambda x: x.mean(axis=(1,2)))
+  def test_mean_zero_axis(self):
+    helper_test_op([(1,0,3,0,5)], lambda x: x.mean(axis=(1,3)))
+
+  def test_var(self):
+    helper_test_op([(15, 25, 35)], lambda x: x.var())
+    helper_test_op([(15, 25, 35)], lambda x: x.var(correction=0))
+    helper_test_op([(15, 25, 35)], lambda x: x.var(correction=5))
+    # TODO: fix this
+    # helper_test_op([(10, 2)], lambda x: x.var(correction=50))
+  def test_var_axis(self):
+    helper_test_op([(15, 25, 35)], lambda x: x.var(0))
+    helper_test_op([(15, 25, 35)], lambda x: x.var(2))
+    helper_test_op([(15, 25, 35)], lambda x: x.var([1, 2]))
+    helper_test_op([(15, 25, 35)], lambda x: x.var(0, correction=0))
+    helper_test_op([(15, 25, 35)], lambda x: x.var(2, correction=0))
+    helper_test_op([(15, 25, 35)], lambda x: x.var([1, 2], correction=0))
+  def test_var_zero_axis(self):
+    helper_test_op([(1,0,3,0,5)], lambda x: x.var(axis=(1,3)))
+    helper_test_op([(1,0,3,0,5)], lambda x: x.var(axis=(1,3), correction=0))
+    helper_test_op([(1,0,3,0,5)], lambda x: x.var(axis=(1,3), correction=5))
+  def test_var_keepdim(self):
+    helper_test_op([(15, 25, 35)], lambda x: x.var(keepdim=True))
+    helper_test_op([(15, 25, 35)], lambda x: x.var(0, keepdim=True, correction=0))
+
   def test_std(self):
-    helper_test_op([(45, 65, 85)], lambda x: torch.std(x), lambda x: Tensor.std(x))
-    helper_test_op([(45, 65, 85)], lambda x: torch.std(x, dim=None, correction=0), lambda x: Tensor.std(x, correction=0))
-    helper_test_op([(45, 65, 85)], lambda x: torch.std(x, dim=None, correction=5), lambda x: Tensor.std(x, correction=5))
-  @unittest.skipIf(Device.DEFAULT == "WEBGL" and CI, "Only broken on CI")
+    helper_test_op([(15, 25, 35)], lambda x: x.std())
+    helper_test_op([(15, 25, 35)], lambda x: x.std(correction=0))
+    helper_test_op([(15, 25, 35)], lambda x: x.std(correction=5))
   def test_std_axis(self):
-    helper_test_op([(45, 65, 85)], lambda x: torch.std(x, dim=0), lambda x: Tensor.std(x, axis=0))
-    helper_test_op([(45, 65, 85)], lambda x: torch.std(x, dim=2), lambda x: Tensor.std(x, axis=2))
-    helper_test_op([(45, 65, 85)], lambda x: torch.std(x, dim=[1, 2]), lambda x: Tensor.std(x, axis=[1, 2]))
-    helper_test_op([(45, 65, 85)], lambda x: torch.std(x, dim=None), lambda x: Tensor.std(x, axis=None))
-    helper_test_op([(45, 65, 85)], lambda x: torch.std(x, correction=0, dim=0), lambda x: Tensor.std(x, axis=0, correction=0))
-    helper_test_op([(45, 65, 85)], lambda x: torch.std(x, correction=0, dim=2), lambda x: Tensor.std(x, axis=2, correction=0))
-    helper_test_op([(45, 65, 85)], lambda x: torch.std(x, correction=0, dim=[1, 2]), lambda x: Tensor.std(x, axis=[1, 2], correction=0))
-    helper_test_op([(45, 65, 85)], lambda x: torch.std(x, correction=0, dim=None), lambda x: Tensor.std(x, axis=None, correction=0))
-  @unittest.skipIf(Device.DEFAULT == "WEBGL" and CI, "Only broken on CI")
+    helper_test_op([(15, 25, 35)], lambda x: x.std(0))
+    helper_test_op([(15, 25, 35)], lambda x: x.std(2))
+    helper_test_op([(15, 25, 35)], lambda x: x.std([1, 2]))
+    helper_test_op([(15, 25, 35)], lambda x: x.std(0, correction=0))
+    helper_test_op([(15, 25, 35)], lambda x: x.std(2, correction=0))
+    helper_test_op([(15, 25, 35)], lambda x: x.std([1, 2], correction=0))
+  def test_std_zero_axis(self):
+    helper_test_op([(1,0,3,0,5)], lambda x: x.std(axis=(1,3)))
+    helper_test_op([(1,0,3,0,5)], lambda x: x.std(axis=(1,3), correction=0))
+    helper_test_op([(1,0,3,0,5)], lambda x: x.std(axis=(1,3), correction=5))
   def test_std_keepdim(self):
-    helper_test_op([(45, 65, 85)], lambda x: torch.std(x, dim=None, keepdim=True), lambda x: Tensor.std(x, keepdim=True))
-    helper_test_op([(45, 65, 85)], lambda x: torch.std(x, dim=0, keepdim=True, correction=0),
-                                   lambda x: Tensor.std(x, keepdim=True, correction=0, axis=0))
+    helper_test_op([(15, 25, 35)], lambda x: x.std(keepdim=True))
+    helper_test_op([(15, 25, 35)], lambda x: x.std(0, keepdim=True, correction=0))
+
   def test_softmax(self):
     # exceed per kernel buffer limit with backward
     forward_only = (Device.DEFAULT == "WEBGPU")
-    helper_test_op([(45,65)], lambda x: torch.nn.Softmax(dim=1)(x), Tensor.softmax, atol=1e-7, grad_atol=1e-7, forward_only=forward_only)
-    helper_test_op([()], lambda x: torch.nn.Softmax(dim=0)(x), Tensor.softmax, atol=1e-7, grad_atol=1e-7, forward_only=forward_only)
+    helper_test_op([(45,65)], torch.nn.Softmax(dim=1), Tensor.softmax, atol=1e-7, grad_atol=1e-7, forward_only=forward_only)
+    helper_test_op([(45)], torch.nn.Softmax(dim=0), Tensor.softmax, atol=1e-7, grad_atol=1e-7, forward_only=forward_only)
+    helper_test_op([()], torch.nn.Softmax(dim=0), Tensor.softmax, atol=1e-7, grad_atol=1e-7, forward_only=forward_only)
+    helper_test_op([()], torch.nn.Softmax(dim=-1), Tensor.softmax, atol=1e-7, grad_atol=1e-7, forward_only=forward_only)
+  def test_softmax_other_axis(self):
+    helper_test_op([(10,10,10)], lambda x: x.softmax(0), atol=1e-7, grad_atol=1e-7)
+    helper_test_op([(10,10,10)], lambda x: x.softmax(1), atol=1e-7, grad_atol=1e-7)
+    helper_test_op([(10,10,10)], lambda x: x.softmax(2), atol=1e-7, grad_atol=1e-7)
+  def test_softmax_argmax(self):
+    helper_test_op([(45,65)], lambda x: x.softmax(0).argmax().type(torch.int32),
+                              lambda x: x.softmax(0).argmax(), forward_only=True, atol=1e-7, grad_atol=1e-7)
+    helper_test_op([(45,65)], lambda x: x.softmax(1).argmax().type(torch.int32),
+                              lambda x: x.softmax(1).argmax(), forward_only=True, atol=1e-7, grad_atol=1e-7)
   def test_log_softmax(self):
-    helper_test_op([(45,65)], lambda x: torch.nn.LogSoftmax(dim=1)(x), Tensor.log_softmax, atol=1e-7, grad_atol=1e-7)
-    helper_test_op([()], lambda x: torch.nn.LogSoftmax(dim=0)(x), Tensor.log_softmax, atol=1e-7, grad_atol=1e-7)
+    helper_test_op([(45,65)], torch.nn.LogSoftmax(dim=1), Tensor.log_softmax, atol=1e-7, grad_atol=1e-7)
+    helper_test_op([(45)], torch.nn.LogSoftmax(dim=0), Tensor.log_softmax, atol=1e-7, grad_atol=1e-7)
+    helper_test_op([()], torch.nn.LogSoftmax(dim=0), Tensor.log_softmax, atol=1e-7, grad_atol=1e-7)
+    helper_test_op([()], torch.nn.LogSoftmax(dim=-1), Tensor.log_softmax, atol=1e-7, grad_atol=1e-7)
   def test_log_softmax_other_axis(self):
-    helper_test_op([(10,10,10)], lambda x: x.log_softmax(0), lambda x: x.log_softmax(0), atol=1e-7, grad_atol=1e-7)
-    helper_test_op([(10,10,10)], lambda x: x.log_softmax(1), lambda x: x.log_softmax(1), atol=1e-7, grad_atol=1e-7)
-    helper_test_op([(10,10,10)], lambda x: x.log_softmax(2), lambda x: x.log_softmax(2), atol=1e-7, grad_atol=1e-7)
+    helper_test_op([(10,10,10)], lambda x: x.log_softmax(0), atol=1e-7, grad_atol=1e-7)
+    helper_test_op([(10,10,10)], lambda x: x.log_softmax(1), atol=1e-7, grad_atol=1e-7)
+    helper_test_op([(10,10,10)], lambda x: x.log_softmax(2), atol=1e-7, grad_atol=1e-7)
+
+  def test_logsumexp(self):
+    helper_test_op([(45,65)], lambda x: torch.logsumexp(x, dim=0), lambda x: x.logsumexp(0), atol=1e-7, grad_atol=1e-7)
+    helper_test_op([(45,65)], lambda x: torch.logsumexp(x, dim=0, keepdim=True), lambda x: x.logsumexp(0, True), atol=1e-7, grad_atol=1e-7)
+    helper_test_op([(45,65)], lambda x: torch.logsumexp(x, dim=1), lambda x: x.logsumexp(1), atol=1e-7, grad_atol=1e-7)
+    helper_test_op([(45)], lambda x: torch.logsumexp(x, dim=0), lambda x: x.logsumexp(0), atol=1e-7, grad_atol=1e-7)
+    helper_test_op([()], lambda x: torch.logsumexp(x, dim=0), lambda x: x.logsumexp(0), atol=1e-7, grad_atol=1e-7)
+    helper_test_op([()], lambda x: torch.logsumexp(x, dim=-1), lambda x: x.logsumexp(-1), atol=1e-7, grad_atol=1e-7)
+
+  def test_sinh(self):
+    helper_test_op([(45,65)], lambda x: x.sinh(), grad_atol=1e-6)
+    # TODO: backward nan instead of inf
+    helper_test_op([(45,65)], lambda x: x.sinh(), grad_atol=1e-6, low=-300, high=-297, forward_only=True)
+    helper_test_op([(45,65)], lambda x: x.sinh(), grad_atol=1e-6, low=300, high=303, forward_only=True)
+  def test_cosh(self):
+    helper_test_op([(45,65)], lambda x: x.cosh(), grad_atol=1e-6)
+    # TODO: backward nan instead of inf
+    helper_test_op([(45,65)], lambda x: x.cosh(), grad_atol=1e-6, low=-300, high=-297, forward_only=True)
+    helper_test_op([(45,65)], lambda x: x.cosh(), grad_atol=1e-6, low=300, high=303, forward_only=True)
   def test_tanh(self):
-    helper_test_op([(45,65)], lambda x: x.tanh(), Tensor.tanh, atol=1e-6, grad_atol=1e-6)
-    helper_test_op([(45,65)], lambda x: x.tanh(), Tensor.tanh, atol=1e-6, grad_atol=1e-6, a=-100)
-    helper_test_op([()], lambda x: x.tanh(), Tensor.tanh, atol=1e-6, grad_atol=1e-6)
+    helper_test_op([(45,65)], lambda x: x.tanh(), grad_atol=1e-6)
+    helper_test_op([(45,65)], lambda x: x.tanh(), grad_atol=1e-6, low=-300, high=-297)
+    helper_test_op([(45,65)], lambda x: x.tanh(), grad_atol=1e-6, low=300, high=303)
   def test_hardtanh(self):
     for val in range(10, 30, 5):
-      helper_test_op([(45,65)], lambda x: torch.nn.functional.hardtanh(x,-val, val), lambda x: x.hardtanh(-val, val), atol=1e-6, grad_atol=1e-6)
-      helper_test_op([()], lambda x: torch.nn.functional.hardtanh(x,-val, val), lambda x: x.hardtanh(-val, val), atol=1e-6, grad_atol=1e-6)
+      helper_test_op([(45,65)], lambda x: torch.nn.functional.hardtanh(x, -val, val), lambda x: x.hardtanh(-val, val), grad_atol=1e-6)
+      helper_test_op([()], lambda x: torch.nn.functional.hardtanh(x, -val, val), lambda x: x.hardtanh(-val, val), grad_atol=1e-6)
+  def test_asinh(self):
+    helper_test_op([(45,65)], lambda x: x.asinh(), grad_atol=1e-6)
+    # NOTE: this one has larger atol
+    helper_test_op([(45,65)], lambda x: x.asinh(), atol=1e-2, grad_atol=1e-6, low=-300, high=-297)
+    helper_test_op([(45,65)], lambda x: x.asinh(), grad_atol=1e-6, low=300, high=303)
+  def test_acosh(self):
+    helper_test_op([(45,65)], lambda x: x.acosh(), grad_atol=1e-6)
+    helper_test_op([(45,65)], lambda x: x.acosh(), grad_atol=1e-6, low=-300, high=-297)
+    helper_test_op([(45,65)], lambda x: x.acosh(), grad_atol=1e-6, low=300, high=303)
+  def test_atanh(self):
+    helper_test_op([(45,65)], lambda x: x.atanh(), grad_atol=1e-6)
+    helper_test_op([(45,65)], lambda x: x.atanh(), grad_atol=1e-6, low=-300, high=-297)
+    helper_test_op([(45,65)], lambda x: x.atanh(), grad_atol=1e-6, low=300, high=303)
+
   def test_topo_sort(self):
-    helper_test_op([(45,65)], lambda x: (x+x)*x, lambda x: x.add(x).mul(x), atol=1e-6, grad_atol=1e-6)
-    helper_test_op([()], lambda x: (x+x)*x, lambda x: x.add(x).mul(x), atol=1e-6, grad_atol=1e-6)
+    helper_test_op([(45,65)], lambda x: (x+x)*x, grad_atol=1e-6)
+    helper_test_op([()], lambda x: (x+x)*x, grad_atol=1e-6)
 
-  def test_scalar_mul(self):
-    helper_test_op([(45,65)], lambda x: x*2, lambda x: x*2)
-    helper_test_op([()], lambda x: x*2, lambda x: x*2)
-  def test_scalar_rmul(self):
-    helper_test_op([(45,65)], lambda x: 2*x, lambda x: 2*x)
-    helper_test_op([()], lambda x: 2*x, lambda x: 2*x)
-  def test_scalar_sub(self):
-    helper_test_op([(45,65)], lambda x: x-2, lambda x: x-2)
-    helper_test_op([()], lambda x: x-2, lambda x: x-2)
-  def test_scalar_rsub(self):
-    helper_test_op([(45,65)], lambda x: 2-x, lambda x: 2-x)
-    helper_test_op([()], lambda x: 2-x, lambda x: 2-x)
   def test_flip_eye_crash(self):
     helper_test_op([], lambda: (torch.eye(10)@torch.eye(10).flip(0)),
                        lambda: (Tensor.eye(10)@Tensor.eye(10).flip(0)), forward_only=True)
 
   def test_broadcast_full(self):
     for torch_op, tinygrad_op in [(torch.add, Tensor.add), (torch.sub, Tensor.sub), (torch.mul, Tensor.mul),
-                                  (torch.div, Tensor.div)]: #, (torch.pow, Tensor.pow)]:
+                                  (torch.div, Tensor.div), (torch.pow, Tensor.pow)]:
       for shapes in [((5,13,24,16), (5,1,24,1)), ((1,3,1,7,1), (2,1,5,1,8))]:
         with self.subTest(op=torch_op.__name__, shapes=shapes):
-          helper_test_op(shapes, torch_op, tinygrad_op, a=-0.5 if tinygrad_op != Tensor.pow else 0.0)
+          if tinygrad_op != Tensor.pow:
+            helper_test_op(shapes, torch_op, tinygrad_op)
+          else:
+            helper_test_op(shapes, torch_op, tinygrad_op, low=0, high=3)
 
   def test_broadcast_simple(self):
-    helper_test_op([(45,65), (45,1)], lambda x,y: x/y, lambda x,y: x/y)
-    helper_test_op([(45,65), ()], lambda x,y: x/y, lambda x,y: x/y)
+    helper_test_op([(45,65), (45,1)], lambda x,y: x/y)
+    helper_test_op([(45,65), ()], lambda x,y: x/y)
 
   def test_broadcast_partial(self):
     for torch_op, tinygrad_op in [(torch.add, Tensor.add), (torch.sub, Tensor.sub), (torch.mul, Tensor.mul),
-                                  (torch.div, Tensor.div)]: #, (torch.pow, Tensor.pow)]:
+                                  (torch.div, Tensor.div), (torch.pow, Tensor.pow)]:
       for shapes in [((1,32,32,32), (1,32,1,1)), ((5,13,24,16,2), (1,13,24,1,1)),
                      ((4,1), (4,5)), ((1,4), (5,4))]:
         with self.subTest(op=torch_op.__name__, shapes=shapes):
           # NOTE: ANE backwards?
-          helper_test_op(shapes, torch_op, tinygrad_op, a=-0.5 if tinygrad_op != Tensor.pow else 0.0)
+          if tinygrad_op != Tensor.pow:
+            helper_test_op(shapes, torch_op, tinygrad_op)
+          else:
+            helper_test_op(shapes, torch_op, tinygrad_op, low=0, high=3)
 
   def test_slice_in_bounds_1dim(self):
-    helper_test_op([(3)], lambda x: x[1:3], lambda x: x[1:3])
-    helper_test_op([(3)], lambda x: x[0:2], lambda x: x[0:2])
-    helper_test_op([(3)], lambda x: x[-2:2], lambda x: x[-2:2])
+    helper_test_op([(3)], lambda x: x[1:3])
+    helper_test_op([(3)], lambda x: x[0:2])
+    helper_test_op([(3)], lambda x: x[-2:2])
 
   def test_slice_on_0dim_tensor(self):
-    helper_test_op([()], lambda x: x[None], lambda x: x[None])
+    helper_test_op([()], lambda x: x[None])
 
     with self.assertRaises(IndexError):
       a = Tensor(3.14)
       a[0]
 
   def test_slice_int_indexing(self):
-    helper_test_op([(3)], lambda x: x[1], lambda x: x[1])
-    helper_test_op([(3)], lambda x: x[-2], lambda x: x[-2])
-    helper_test_op([(10,10)], lambda x: x[1], lambda x: x[1])
-    helper_test_op([(3,3,3)], lambda x: x[1,1,1], lambda x: x[1,1,1])
+    helper_test_op([(3)], lambda x: x[0])
+    helper_test_op([(3)], lambda x: x[2])
+    helper_test_op([(3)], lambda x: x[-1])
+    helper_test_op([(3)], lambda x: x[-3])
+    helper_test_op([(10,10)], lambda x: x[1])
+    helper_test_op([(3,3,3)], lambda x: x[1,1,1])
 
   def test_slice_in_bounds_multidim(self):
-    helper_test_op([(3,3,3)], lambda x: x[1:2], lambda x: x[1:2])
-    helper_test_op([(3,3,3)], lambda x: x[1:2, 2], lambda x: x[1:2, 2])
-    helper_test_op([(3,3,3)], lambda x: x[1:2, 1:2], lambda x: x[1:2, 1:2])
-    helper_test_op([(3,3,3)], lambda x: x[1:2, 1:2, 0:-1], lambda x: x[1:2, 1:2, 0:-1])
+    helper_test_op([(3,3,3)], lambda x: x[1:2])
+    helper_test_op([(3,3,3)], lambda x: x[1:2, 2])
+    helper_test_op([(3,3,3)], lambda x: x[1:2, 1:2])
+    helper_test_op([(3,3,3)], lambda x: x[1:2, 1:2, 0:-1])
 
   def test_slice_with_none(self):
-    helper_test_op([(3,3,3)], lambda x: x[None], lambda x: x[None])
-    helper_test_op([(3,3,3)], lambda x: x[1:2, None], lambda x: x[1:2, None])
-    helper_test_op([(3,3,3)], lambda x: x[1:2, None, 1:2], lambda x: x[1:2, None, 1:2])
-    helper_test_op([(3,3,3)], lambda x: x[1:2, 1:2, None, -1], lambda x: x[1:2, 1:2, None, -1])
-    helper_test_op([(3,3,3)], lambda x: x[None, None, 1, None, 2, 0:2], lambda x: x[None, None, 1, None, 2, 0:2])
+    helper_test_op([(3,3,3)], lambda x: x[None])
+    helper_test_op([(3,3,3)], lambda x: x[1:2, None])
+    helper_test_op([(3,3,3)], lambda x: x[1:2, None, 1:2])
+    helper_test_op([(3,3,3)], lambda x: x[1:2, 1:2, None, -1])
+    helper_test_op([(3,3,3)], lambda x: x[None, None, 1, None, 2, 0:2])
+
+  def test_slice_with_const_tensor(self):
+    t = Tensor.zeros(1, dtype=dtypes.int)
+    helper_test_op([(3,3,3)], lambda x: x[:, [0], :], lambda x: x[:, t, :])
+    helper_test_op([(3,3,3)], lambda x: x[:, [0], :], lambda x: x[:, t.contiguous(), :])
 
   def test_slice_one_endpoint_out_of_bounds(self):
-    helper_test_op([(3,3,3)], lambda x: x[0:4], lambda x: x[0:4])
-    helper_test_op([(3,3,3)], lambda x: x[-6:4], lambda x: x[-6:4])
-    helper_test_op([(3,3,3)], lambda x: x[1:50], lambda x: x[1:50])
-    helper_test_op([(3,3,3)], lambda x: x[1:50, 1:2, -1], lambda x: x[1:50, 1:2, -1])
+    helper_test_op([(3,3,3)], lambda x: x[0:4])
+    helper_test_op([(3,3,3)], lambda x: x[-6:4])
+    helper_test_op([(3,3,3)], lambda x: x[1:50])
+    helper_test_op([(3,3,3)], lambda x: x[1:50, 1:2, -1])
 
   def test_slice_stride_gt_one(self):
-    helper_test_op([(7,5,10)], lambda x: x[::2, ::3, ::4], lambda x: x[::2, ::3, ::4])
-    helper_test_op([(7,5,10)], lambda x: x[1:5:2, ::3, ::4], lambda x: x[1:5:2, ::3, ::4])
-    helper_test_op([(7,5,10)], lambda x: x[1:5:2, 3, ::4], lambda x: x[1:5:2, 3, ::4])
-    helper_test_op([(7,5,10)], lambda x: x[1:5:2, None, None, 3, None, ::4], lambda x: x[1:5:2, None, None, 3, None, ::4])
+    helper_test_op([(7,5,10)], lambda x: x[::2, ::3, ::4])
+    helper_test_op([(7,5,10)], lambda x: x[1:5:2, ::3, ::4])
+    helper_test_op([(7,5,10)], lambda x: x[1:5:2, 3, ::4])
+    helper_test_op([(7,5,10)], lambda x: x[1:5:2, None, None, 3, None, ::4])
 
   def test_slice_negative_strides(self):
     # Torch doesn't support slicing with negative steps
     a = np.random.randn(10, 10, 10).astype(np.float32)
     t = Tensor(a)
     np.testing.assert_allclose(a[::-1], t[::-1].numpy())
     np.testing.assert_allclose(a[::-2], t[::-2].numpy())
     np.testing.assert_allclose(a[:, 2:0:-1], t[:, 2:0:-1].numpy())
     np.testing.assert_allclose(a[:, 2:0:-1, 3:1:-2], t[:, 2:0:-1, 3:1:-2].numpy())
     np.testing.assert_allclose(a[4:0:-3, 2:0:-1, -1:-5:-2], t[4:0:-3, 2:0:-1, -1:-5:-2].numpy())
-    if Device.DEFAULT not in ["CPU"]:
-      # broken
-      np.testing.assert_allclose(a[2:5:-1, :, :], t[2:5:-1, :, :].numpy())  # shape = (0, 10, 10)
-      np.testing.assert_allclose(a[:, 2:5:-1, :], t[:, 2:5:-1, :].numpy())  # shape = (0, 10, 10)
-      np.testing.assert_allclose(a[:, :, 2:5:-1], t[:, :, 2:5:-1].numpy())  # shape = (0, 10, 10)
+    np.testing.assert_allclose(a[2:5:-1, :, :], t[2:5:-1, :, :].numpy())  # shape = (0, 10, 10)
+    np.testing.assert_allclose(a[:, 2:5:-1, :], t[:, 2:5:-1, :].numpy())  # shape = (0, 10, 10)
+    np.testing.assert_allclose(a[:, :, 2:5:-1], t[:, :, 2:5:-1].numpy())  # shape = (0, 10, 10)
 
   def test_slice_both_endpoints_out_of_bounds(self):
-    helper_test_op([(3,3,3)], lambda x: x[5:10], lambda x: x[5:10], forward_only=True)
-    helper_test_op([(3,3,3)], lambda x: x[-15:-7], lambda x: x[-15:-7], forward_only=True)
+    helper_test_op([(3,3,3)], lambda x: x[5:10])
+    helper_test_op([(3,3,3)], lambda x: x[-15:-7])
 
   def test_slice_start_gt_end(self):
-    helper_test_op([(3,3,3)], lambda x: x[-2:2], lambda x: x[-2:2], forward_only=True)
-    helper_test_op([(3,3,3)], lambda x: x[-2:-5], lambda x: x[-2:-5], forward_only=True)
+    helper_test_op([(3,3,3)], lambda x: x[-2:2])
+    helper_test_op([(3,3,3)], lambda x: x[-2:-5])
 
   def test_slice_empty(self):
-    helper_test_op([(10,10)], lambda x: x[1:1], lambda x: x[1:1], forward_only=True)
+    helper_test_op([(10,10)], lambda x: x[1:1])
 
   def test_slice_zero_in_shape(self):
-    helper_test_op([(10,10)], lambda x: x[1:1], lambda x: x[1:1], forward_only=True)  # x.shape = (0, 10)
-    helper_test_op([(3,3,3)], lambda x: x[-2:-5], lambda x: x[-2:-5], forward_only=True)  # x.shape = (0, 3, 3)
+    helper_test_op([(10,10)], lambda x: x[1:1])  # x.shape = (0, 10)
+    helper_test_op([(3,3,3)], lambda x: x[-2:-5])  # x.shape = (0, 3, 3)
 
   def test_slice_errors(self):
     a = Tensor.ones(4, 3)
     b = Tensor(2)
     with self.assertRaises(IndexError): a[1, 77, 77, 77] # IndexError: (finds too many indices before the out of bounds)
-    with self.assertRaises(IndexError): a[1, 77] # IndexError: (out of bounds).
-    with self.assertRaises(IndexError): a[1, -77]
+    with self.assertRaises(IndexError): a[1, 3] # IndexError: (out of bounds).
+    with self.assertRaises(IndexError): a[1, -4]
     with self.assertRaises(IndexError): a[..., ...] # IndexError: only single ellipsis
     with self.assertRaises(ValueError): a[::0, 1] # no 0 strides
     with self.assertRaises(IndexError): b[:] # slice cannot be applied to a 0-dim tensor
 
   def test_slice_ellipsis(self):
-    helper_test_op([(3,3,3,3)], lambda x: x[..., 0], lambda x: x[..., 0])
-    helper_test_op([(3,3,3,3)], lambda x: x[0, ...], lambda x: x[0, ...])
-    helper_test_op([(3,3,3,3)], lambda x: x[0, ..., 0], lambda x: x[0, ..., 0])
-    helper_test_op([(3,3,3,3)], lambda x: x[0:3, ..., 2:3], lambda x: x[0:3, ..., 2:3])
-    helper_test_op([(3,3,3,3)], lambda x: x[None, 0:3, ..., 0, None], lambda x: x[None, 0:3, ..., 0, None])
+    helper_test_op([(3,3,3,3)], lambda x: x[..., 0])
+    helper_test_op([(3,3,3,3)], lambda x: x[0, ...])
+    helper_test_op([(3,3,3,3)], lambda x: x[0, ..., 0])
+    helper_test_op([(3,3,3,3)], lambda x: x[0:3, ..., 2:3])
+    helper_test_op([(3,3,3,3)], lambda x: x[None, 0:3, ..., 0, None])
 
   def test_pad2d(self):
     helper_test_op([(3,3,3,3)], lambda x: torch.nn.functional.pad(x, (1,2,3,4)), lambda x: x.pad2d(padding=(1,2,3,4)))
     helper_test_op([(3,3,3,3)], lambda x: torch.nn.functional.pad(x, (-1,2,-3,4)), lambda x: x.pad2d(padding=(-1,2,-3,4)))
     helper_test_op([(3,3,3,3)], lambda x: torch.nn.functional.pad(x, (1,2,3,4), value=5), lambda x: x.pad2d(padding=(1,2,3,4),value=5))
     helper_test_op([(3,3,3,3)], lambda x: torch.nn.functional.pad(x, (-1,2,-3,4), value=5), lambda x: x.pad2d(padding=(-1,2,-3,4),value=5))
 
@@ -780,14 +1021,25 @@
     helper_test_op([(3,3)], lambda x: torch.nn.functional.pad(x, (1,2,3,4)),lambda x: x.pad(((3,4),(1,2))))
     helper_test_op([(3,3)], lambda x: torch.nn.functional.pad(x, (1,2,3,4), value=5), lambda x: x.pad(((3,4), (1,2)), value=5))
     helper_test_op([(3,3)], lambda x: torch.nn.functional.pad(x, (1,2,3,4), value=math.inf), lambda x: x.pad(((3,4), (1,2)), value=math.inf))
     helper_test_op([(3,3)], lambda x: torch.nn.functional.pad(x, (1,2,3,4), value=-math.inf), lambda x: x.pad(((3,4), (1,2)), value=-math.inf))
     helper_test_op([(3,3)], lambda x: torch.nn.functional.pad(x, (0,0,3,4), value=1), lambda x: x.pad(((3,4), None), value=1))
     helper_test_op([(3,3)], lambda x: torch.nn.functional.pad(x, (0,0,0,0), value=1), lambda x: x.pad((None, None), value=1))
 
+  def test_pad_reshape(self):
+    helper_test_op([(1, 2)],
+                   lambda x: torch.nn.functional.pad(x, (0, 1, 1, 0)).reshape((3, 2)),
+                   lambda x: x.pad2d((0, 1, 1, 0)).reshape((3, 2)), forward_only=True)
+    helper_test_op([(1, 2)],
+                   lambda x: torch.nn.functional.pad(x, (0, 2, 1, 1)).reshape((4, 3)),
+                   lambda x: x.pad2d((0, 2, 1, 1)).reshape((4, 3)), forward_only=True)
+    helper_test_op([(1, 1, 1, 2)],
+                   lambda x: torch.nn.functional.pad(x, (0, 4, 2, 2, 1, 2, 0, 2)).reshape((4, 3, 6, 5)),
+                   lambda x: x.pad(((0, 2), (1, 2), (2, 2), (0, 4))).reshape((4, 3, 6, 5)), forward_only=True)
+
   @unittest.skipIf(Device.DEFAULT == "WEBGL", "incorrect result")
   def test_pad_slice(self):
     for value in 0., 3.456:
       helper_test_op([(1)], lambda x: torch.nn.functional.pad(x,(1,0), value=value)[0], lambda x: x.pad(((1,0),), value=value)[0])
       helper_test_op([(4)], lambda x: torch.nn.functional.pad(x,(1,0), value=value)[0], lambda x: x.pad(((1,0),), value=value)[0])
       helper_test_op([(4)], lambda x: torch.nn.functional.pad(x,(3,0), value=value)[0:1], lambda x: x.pad(((3,0),), value=value)[0:1])
       helper_test_op([(4)], lambda x: torch.nn.functional.pad(x,(0,3), value=value)[6], lambda x: x.pad(((0,3),), value=value)[6])
@@ -806,93 +1058,104 @@
       helper_test_op([(3,3)], lambda x: torch.nn.functional.pad(x,(0,1,3,2), value=value)[0:2,:], lambda x: x.pad(((3,2),(0,1)), value=value)[0:2,:])
       helper_test_op([(3,3,3)], lambda x: torch.nn.functional.pad(x,(1,1,0,1,3,2), value=value)[0:2,:,:],
                                 lambda x: x.pad(((3,2),(0,1),(1,1)), value=value)[0:2,:,:])
       helper_test_op([(3,3,3)], lambda x: torch.nn.functional.pad(x,(1,1,0,1,3,2), value=value)[2:4,:,:],
                                 lambda x: x.pad(((3,2),(0,1),(1,1)), value=value)[2:4,:,:])
 
   def test_stack_slice(self):
-    helper_test_op([(4)], lambda x: torch.stack([x for i in range(3)])[0,:], lambda x: Tensor.stack([x for i in range(3)])[0,:])
-    helper_test_op([(5)], lambda x: torch.stack([x for i in range(3)])[0,0], lambda x: Tensor.stack([x for i in range(3)])[0,0])
-    helper_test_op([(4,4)], lambda x: torch.stack([x for i in range(4)])[3], lambda x: Tensor.stack([x for i in range(4)])[3])
+    helper_test_op([(4)], lambda x: torch.stack([x for i in range(3)])[0,:], lambda x: Tensor.stack(*[x for i in range(3)])[0,:])
+    helper_test_op([(5)], lambda x: torch.stack([x for i in range(3)])[0,0], lambda x: Tensor.stack(*[x for i in range(3)])[0,0])
+    helper_test_op([(4,4)], lambda x: torch.stack([x for i in range(4)])[3], lambda x: Tensor.stack(*[x for i in range(4)])[3])
 
   def test_transpose(self):
-    helper_test_op([(3,3,3)], lambda x: x.transpose(1,2), lambda x: x.transpose(1,2))
-    helper_test_op([(3,3,3)], lambda x: x.transpose(0,2), lambda x: x.transpose(0,2))
-    helper_test_op([(1,2,3,4)], lambda x: x.movedim((3,0,2,1),(0,1,2,3)), lambda x: x.permute(order=(3,0,2,1)))
-    helper_test_op([(3,4,5,6)], lambda x: x.movedim((3,2,1,0),(0,1,2,3)), lambda x: x.permute(order=(3,2,1,0)))
-    helper_test_op([()], lambda x: x.permute(()), lambda x: x.permute(()))
+    helper_test_op([(3,3)], lambda x: x.T)
+    helper_test_op([(3,3,3)], lambda x: x.transpose(1,2))
+    helper_test_op([(3,3,3)], lambda x: x.transpose(0,2))
+    helper_test_op([(1,2,3,4)], lambda x: x.permute((3,0,2,1)))
+    helper_test_op([(3,4,5,6)], lambda x: x.permute((3,2,1,0)))
+    helper_test_op([()], lambda x: x.permute(()))
 
   def test_reshape(self):
-    helper_test_op([(4,3,6,6)], lambda x: torch.reshape(x, (-1,3,6,6)), lambda x: x.reshape(shape=(-1,3,6,6)))
-    helper_test_op([(4,3,6,6)], lambda x: torch.reshape(x, (-1,1,6,6)), lambda x: x.reshape(shape=(-1,1,6,6)))
-    helper_test_op([()], lambda x: torch.reshape(x, []), lambda x: x.reshape([]))
-    helper_test_op([(1,)], lambda x: torch.reshape(x, []), lambda x: x.reshape([]))
-    helper_test_op([()], lambda x: torch.reshape(x, [1]), lambda x: x.reshape([1]))
+    helper_test_op([(4,3,6,6)], lambda x: x.reshape((-1,3,6,6)))
+    helper_test_op([(4,3,6,6)], lambda x: x.reshape((-1,1,6,6)))
+    helper_test_op([()], lambda x: x.reshape([]))
+    helper_test_op([(1,)], lambda x: x.reshape([]))
+    helper_test_op([()], lambda x: x.reshape([1]))
+    helper_test_op([()], lambda x: x.reshape([1, 1, 1]))
 
     with self.assertRaises(ValueError):
       x = Tensor.ones((4,3,6,6))
       x.reshape([])
 
   def test_flip(self):
-    helper_test_op([(4,3,6,6)], lambda x: torch.flip(x, (0,)), lambda x: x.flip(axis=(0,)))
-    helper_test_op([(4,3,6,6)], lambda x: torch.flip(x, (0,1)), lambda x: x.flip(axis=(0,1)))
-    helper_test_op([(4,3,6,6)], lambda x: torch.flip(x, (0,1,3)), lambda x: x.flip(axis=(0,1,3)))
-    helper_test_op([(4,3,6,6)], lambda x: torch.flip(x, (3,)), lambda x: x.flip(axis=(3,)))
-    helper_test_op([(4,3,6,6)], lambda x: torch.flip(x, (0,1,3)).flip((0,)), lambda x: x.flip(axis=(0,1,3)).flip(0))
-    helper_test_op([(4,3,6,6)], lambda x: torch.flip(x, (3,)), lambda x: x.flip(axis=(-1,)))
-    helper_test_op([()], lambda x: torch.flip(x, ()), lambda x: x.flip(axis=()))
-    helper_test_op([(1,)], lambda x: torch.flip(x, ()), lambda x: x.flip(axis=()))
-    helper_test_op([(4, 3, 6, 6)], lambda x: torch.flip(x, ()), lambda x: x.flip(axis=()))
+    helper_test_op([(4,3,6,6)], lambda x: x.flip((0,)))
+    helper_test_op([(4,3,6,6)], lambda x: x.flip((0,1)))
+    helper_test_op([(4,3,6,6)], lambda x: x.flip((0,1,3)))
+    helper_test_op([(4,3,6,6)], lambda x: x.flip((3,)))
+    helper_test_op([(4,3,6,6)], lambda x: x.flip((0,1,3)).flip(0))
+    helper_test_op([(4,3,6,6)], lambda x: x.flip((-1,)))
+    helper_test_op([()], lambda x: x.flip(()))
+    helper_test_op([(1,)], lambda x: x.flip(()))
+    helper_test_op([(4, 3, 6, 6)], lambda x: x.flip(()))
 
   def test_squeeze(self):
-    helper_test_op([(1,3,6,6)], lambda x: torch.squeeze(x, 0), lambda x: x.squeeze(dim=0))
-    helper_test_op([(4,3,1,6)], lambda x: torch.squeeze(x, 1), lambda x: x.squeeze(dim=1))
-    helper_test_op([(4,3,6,6)], lambda x: torch.squeeze(x, 3), lambda x: x.squeeze(dim=3))
+    helper_test_op([(1,3,6,6)], lambda x: x.squeeze(0))
+    helper_test_op([(4,3,1,6)], lambda x: x.squeeze(1))
+    helper_test_op([(4,3,6,6)], lambda x: x.squeeze(3))
     self.helper_test_exception([(4,3,6,6)], lambda x: torch.squeeze(x, 50), lambda x: x.squeeze(dim=50), expected=IndexError)
     self.helper_test_exception([(4,3,6,6)], lambda x: torch.squeeze(x, -50), lambda x: x.squeeze(dim=-50), expected=IndexError)
-    helper_test_op([(4,3,6,1)], lambda x: torch.squeeze(x, -1), lambda x: x.squeeze(dim=-1))
-    helper_test_op([(4,3,6,6)], lambda x: torch.squeeze(x), lambda x: x.squeeze())
-    helper_test_op([(1,3,6,6)], lambda x: torch.squeeze(x), lambda x: x.squeeze())
-    helper_test_op([(2,3,1)], lambda x: torch.squeeze(x), lambda x: x.squeeze())
-    helper_test_op([()], lambda x: torch.squeeze(x, -1), lambda x: x.squeeze(dim=-1))
-    helper_test_op([()], lambda x: torch.squeeze(x, 0), lambda x: x.squeeze(dim=0))
-    helper_test_op([()], lambda x: torch.squeeze(x), lambda x: x.squeeze())
+    helper_test_op([(4,3,6,1)], lambda x: x.squeeze(-1))
+    helper_test_op([(4,3,6,6)], lambda x: x.squeeze())
+    helper_test_op([(1,3,6,6)], lambda x: x.squeeze())
+    helper_test_op([(2,3,1)], lambda x: x.squeeze())
+    helper_test_op([()], lambda x: x.squeeze(-1))
+    helper_test_op([()], lambda x: x.squeeze(0))
+    helper_test_op([()], lambda x: x.squeeze())
     self.helper_test_exception([()], lambda x: torch.squeeze(x, 10), lambda x: x.squeeze(dim=10), expected=IndexError)
     self.helper_test_exception([()], lambda x: torch.squeeze(x, 1), lambda x: x.squeeze(dim=1), expected=IndexError)
     self.helper_test_exception([()], lambda x: torch.squeeze(x, -2), lambda x: x.squeeze(dim=-2), expected=IndexError)
 
   def test_unsqueeze(self):
-    helper_test_op([(4,3,6,6)], lambda x: torch.unsqueeze(x, 0), lambda x: x.unsqueeze(dim=0))
-    helper_test_op([(4,3,6,6)], lambda x: torch.unsqueeze(x, 4), lambda x: x.unsqueeze(dim=4))
-    helper_test_op([(4,3,6,6)], lambda x: torch.unsqueeze(x, -1), lambda x: x.unsqueeze(dim=-1))
-    helper_test_op([(4,3,6,6)], lambda x: torch.unsqueeze(x, -3), lambda x: x.unsqueeze(dim=-3))
-    helper_test_op([()], lambda x: torch.unsqueeze(x, 0), lambda x: x.unsqueeze(dim=0))
+    helper_test_op([(4,3,6,6)], lambda x: x.unsqueeze(0))
+    helper_test_op([(4,3,6,6)], lambda x: x.unsqueeze(4))
+    helper_test_op([(4,3,6,6)], lambda x: x.unsqueeze(-1))
+    helper_test_op([(4,3,6,6)], lambda x: x.unsqueeze(-3))
+    helper_test_op([()], lambda x: x.unsqueeze(0))
 
   def test_flatten(self):
     for axis in range(3):
-      helper_test_op([(4,3,6,6)], lambda x: torch.flatten(x, start_dim=axis), lambda x: x.flatten(start_dim=axis))
+      helper_test_op([(4,3,6,6)], lambda x: x.flatten(start_dim=axis))
     for axis in range(3):
-      helper_test_op([(4,3,6,6)], lambda x: torch.flatten(x, end_dim=axis), lambda x: x.flatten(end_dim=axis))
-    helper_test_op([(4,3,6,6)], lambda x: torch.flatten(x, start_dim=1, end_dim=3), lambda x: x.flatten(start_dim=1, end_dim=3))
-    helper_test_op([()], lambda x: x.flatten(), lambda x: x.flatten())
-    helper_test_op([(1,)], lambda x: x.flatten(), lambda x: x.flatten())
+      helper_test_op([(4,3,6,6)], lambda x: x.flatten(end_dim=axis))
+    helper_test_op([(4,3,6,6)], lambda x: x.flatten(start_dim=1, end_dim=3))
+    helper_test_op([()], lambda x: x.flatten())
+    helper_test_op([(1,)], lambda x: x.flatten())
 
   def test_unflatten(self):
-    helper_test_op([(4,3,6,6)], lambda x: torch.unflatten(x, 0, (2, 2)), lambda x: x.unflatten(0, (2, 2)))
-    helper_test_op([(4,3,6,6)], lambda x: torch.unflatten(x, 3, (3, 2)), lambda x: x.unflatten(3, (3, 2)))
-    helper_test_op([(4,3,6,6)], lambda x: torch.unflatten(x, -1, (3, 2, 1)), lambda x: x.unflatten(-1, (3, 2, 1)))
+    helper_test_op([(4,3,6,6)], lambda x: x.unflatten(0, (2, 2)))
+    helper_test_op([(4,3,6,6)], lambda x: x.unflatten(3, (3, 2)))
+    helper_test_op([(4,3,6,6)], lambda x: x.unflatten(-1, (3, 2, 1)))
 
   def test_detach(self):
-    helper_test_op([(4,3,6,6)], lambda x: x.detach(), lambda x: x.detach(), forward_only=True)
-    helper_test_op([()], lambda x: x.detach(), lambda x: x.detach(), forward_only=True)
+    helper_test_op([(4,3,6,6)], lambda x: x.detach(), forward_only=True)
+    helper_test_op([()], lambda x: x.detach(), forward_only=True)
 
   def test_expand(self):
-    arg = (4,3,2,6)
-    helper_test_op([(4,3,1,6)], lambda x: x.expand(arg), lambda x: x.expand(shape=arg))
-    helper_test_op([()], lambda x: x.expand([]), lambda x: x.expand(shape=[]))
+    helper_test_op([(4,3,1,6)], lambda x: x.expand((4,3,2,6)))
+    helper_test_op([(1,1,1,1)], lambda x: x.expand((4,3,2,6)))
+    helper_test_op([(4,3,1,6)], lambda x: x.expand((6,1,4,3,2,6)))
+    helper_test_op([(4,3,1,6)], lambda x: x.expand((0,1,4,3,2,6)))
+    helper_test_op([(4,3,1,6)], lambda x: x.expand((4,3,0,6)))
+    helper_test_op([()], lambda x: x.expand((4,3,2,6)))
+    helper_test_op([()], lambda x: x.expand([]))
+
+    with self.assertRaises((ValueError, RuntimeError)): Tensor.ones(4,3,1,6).expand(4,1,1,6)
+    with self.assertRaises((ValueError, RuntimeError)): Tensor.ones(4,3,1,6).expand(4,6,1,6)
+    with self.assertRaises((ValueError, RuntimeError)): Tensor.ones(4,3,1,6).expand(3,1,6)
+    with self.assertRaises((ValueError, RuntimeError)): Tensor.ones(4,3,2,6).expand(4,3,0,6)
 
   @unittest.skip("very slow")
   def test_sd_big_conv(self):
     # internal shape (1, 1, 512, 62, 62, 512, 3, 3) overflows a int
     helper_test_op([(1,256,64,64), (512,256,3,3)],
                     lambda x,w: torch.nn.functional.conv2d(x, w),
                     lambda x,w: x.conv2d(w), atol=1e-2)
@@ -927,15 +1190,15 @@
   def test_simple_conv3d(self):
     helper_test_op([(1,4,9,9,9), (4,4,3,3,3)],
       lambda x,w: torch.nn.functional.conv3d(x,w).relu(),
       lambda x,w: Tensor.conv2d(x,w).relu(), atol=1e-4, grad_rtol=1e-5)
 
   @unittest.skipIf(IMAGE>0, "no conv3d on images")
   def test_padded_conv3d(self):
-    helper_test_op([(1,4,9,9,9), (4,4,3,3,3)],
+    helper_test_op([(1,4,5,5,5), (4,4,3,3,3)],
       lambda x,w: torch.nn.functional.conv3d(x,w,padding=1).relu(),
       lambda x,w: Tensor.conv2d(x,w,padding=[1,1,1,1,1,1]).relu(), atol=1e-4, grad_rtol=1e-5)
 
   def test_simple_conv2d_m4(self):
     helper_test_op([(1,16,18,18), (16,16,3,3)],
       lambda x,w: torch.nn.functional.conv2d(x,w).relu(),
       lambda x,w: Tensor.conv2d(x,w).relu(), atol=1e-4, grad_rtol=1e-5)
@@ -1227,30 +1490,37 @@
   def test_maxpool2d_bigger_stride(self):
     for stride in [(2,3), (3,2), 2, 3]:
       with self.subTest(stride=stride):
         helper_test_op([(32,2,110,28)],
           lambda x: torch.nn.functional.max_pool2d(x, kernel_size=(2,2), stride=stride),
           lambda x: Tensor.max_pool2d(x, kernel_size=(2,2), stride=stride))
 
-  @unittest.skipIf(Device.DEFAULT == "CUDA", "CUDA fails on this")
+  def test_maxpool2d_bigger_stride_dilation(self):
+    for stride, dilation in zip([(2,3), (3,2), 2, 3, 4], [(3,2), (2,3), 2, 3, 6]):
+      with self.subTest(stride=stride):
+        helper_test_op([(32,2,110,28)],
+          lambda x: torch.nn.functional.max_pool2d(x, kernel_size=(2,2), stride=stride, dilation=dilation),
+          lambda x: Tensor.max_pool2d(x, kernel_size=(2,2), stride=stride, dilation=dilation))
+
+  @unittest.skipIf( Device.DEFAULT in {"CUDA", "NV"}, "CUDA fails on this")
   def test_maxpool2d_unit_stride(self):
-    helper_test_op([(32,2,110,28)],
+    helper_test_op([(8, 2, 17, 14)],
       lambda x: torch.nn.functional.max_pool2d(x, kernel_size=(5,5), stride=1),
       lambda x: Tensor.max_pool2d(x, kernel_size=(5,5), stride=1))
 
   def test_maxpool2d_smaller_stride(self):
     for stride in [(2,3), (3,2), 2, 3]:
       with self.subTest(stride=stride):
-        helper_test_op([(32,2,110,28)],
+        helper_test_op([(8, 2, 17, 14)],
           lambda x: torch.nn.functional.max_pool2d(x, kernel_size=(5,5), stride=stride),
           lambda x: Tensor.max_pool2d(x, kernel_size=(5,5), stride=stride))
 
   def test_maxpool2d_dilation(self):
     for dilation in [(2, 3), (3, 2), 2, 3]:
-      helper_test_op([(32,2,110,28)],
+      helper_test_op([(8, 2, 17, 14)],
         lambda x: torch.nn.functional.max_pool2d(x, kernel_size=(5,5), dilation=dilation),
         lambda x: Tensor.max_pool2d(x, kernel_size=(5,5), dilation=dilation))
 
   def test_avgpool2d(self):
     shape = (32,2,111,28)
     for ksz in [(2,2), (3,3), (3,2), (5,5), (5,1)]:
       with self.subTest(kernel_size=ksz):
@@ -1263,33 +1533,38 @@
       lambda x: torch.nn.functional.avg_pool2d(x, kernel_size=(111,28)),
       lambda x: Tensor.avg_pool2d(x, kernel_size=(111,28)), rtol=1e-5)
 
   def test_cat(self):
     for dim in range(-2, 3):
       helper_test_op([(45,65,9), (45,65,9), (45,65,9)], lambda x,y,z: torch.cat((x,y,z), dim), lambda x,y,z: x.cat(y, z, dim=dim))
 
-    with self.assertRaises(AssertionError):
+    # zero in non-cat axis
+    helper_test_op([(45,0,9), (45,0,9), (45,0,9)], lambda x,y,z: torch.cat((x,y,z), 0), lambda x,y,z: x.cat(y, z, dim=0))
+
+    # zero in cat axis
+    helper_test_op([(45,0,9), (45,1,9), (45,2,9)], lambda x,y,z: torch.cat((x,y,z), 1), lambda x,y,z: x.cat(y, z, dim=1))
+    helper_test_op([(45,0,9), (45,0,9), (45,0,9)], lambda x,y,z: torch.cat((x,y,z), 1), lambda x,y,z: x.cat(y, z, dim=1))
+
+    with self.assertRaises(IndexError):
       a = Tensor(3.14)
       a.cat(a)
 
   def test_multicat(self):
     for dim in range(-1, 2):
       helper_test_op([(45,65), (45,65), (45,65)], lambda x,y,z: torch.cat((x,y,z), dim), lambda x,y,z: x.cat(y, z, dim=dim))
 
   def test_stack(self):
-    x = Tensor.randn(45, 65, 3)
-
     for dim in range(-1, 3):
-      helper_test_op([(45,65,3), (45,65,3), (45,65,3)], lambda x, y, z: torch.stack((x, y, z), dim), lambda x, y, z: Tensor.stack([x, y, z], dim))
+      helper_test_op([(45,65,3), (45,65,3), (45,65,3)], lambda x, y, z: torch.stack((x, y, z), dim), lambda x, y, z: Tensor.stack(x, y, z, dim=dim))
 
     with self.assertRaises(IndexError):
-      Tensor.stack([x], dim=77)
+      Tensor.stack(Tensor.randn(45, 65, 3), dim=77)
 
     a = Tensor(3.14)
-    np.testing.assert_allclose(Tensor.stack([a, a]).numpy(), Tensor([3.14, 3.14]).numpy())
+    np.testing.assert_allclose(Tensor.stack(a, a).numpy(), Tensor([3.14, 3.14]).numpy())
 
   def test_repeat(self):
     x = Tensor.randn(4, 6, 3)
     base_repeats = [2, 4, 3]
 
     for reps in [[], [4], [2, 1], [3, 2, 2]]:
       repeats = base_repeats + reps
@@ -1302,20 +1577,20 @@
     np.testing.assert_allclose(x.repeat((2, 0, 4)).numpy(), Tensor.zeros(8, 0, 12).numpy())
 
   def test_simple_repeat(self):
     repeats = [3, 3, 4]
     helper_test_op([(3, 3)], lambda x: x.repeat(*repeats), lambda x: x.repeat(repeats))
 
   def test_clip(self):
-    helper_test_op([(45,65)], lambda x: x.clip(-2.3, 1.2), lambda x: x.clip(-2.3, 1.2))
-    helper_test_op([(45,65)], lambda x: x.clip(0, 0), lambda x: x.clip(0, 0))
-    helper_test_op([(45,65)], lambda x: x.clip(10, 100), lambda x: x.clip(10, 100))
-    helper_test_op([(45,65)], lambda x: x.clip(0, 0.1), lambda x: x.clip(0, 0.1))
-    helper_test_op([(45,65)], lambda x: x.clip(-0.3, -0.2), lambda x: x.clip(-0.3, -0.2))
-    helper_test_op([(45,65)], lambda x: x.clip(3, 0), lambda x: x.clip(3, 0))
+    helper_test_op([(45,65)], lambda x: x.clip(-2.3, 1.2))
+    helper_test_op([(45,65)], lambda x: x.clip(0, 0))
+    helper_test_op([(45,65)], lambda x: x.clip(10, 100))
+    helper_test_op([(45,65)], lambda x: x.clip(0, 0.1))
+    helper_test_op([(45,65)], lambda x: x.clip(-0.3, -0.2))
+    helper_test_op([(45,65)], lambda x: x.clip(3, 0))
 
   def test_matvecmat(self):
     helper_test_op([(1,128), (128,128), (128,128)], lambda x,y,z: (x@y).relu()@z, atol=1e-4)
 
   def test_matvec(self):
     helper_test_op([(1,128), (128,128)], lambda x,y: (x@y).relu(), atol=1e-4)
 
@@ -1376,15 +1651,15 @@
   def test_slice_fancy_indexing_dim_inject_and_collapse(self):
     a,b,c,d,e,i,j,k,o,p = self._get_index_randoms()  # noqa
     # dim injection and collapse
     helper_test_op([(2,5,6,5,3,4)], lambda x: x[1,b,None,d,1], lambda x: x[1,j,None,o,1])
     helper_test_op([(2,5,6,5,3,4)], lambda x: x[None,b,2,d,None], lambda x: x[None,j,2,o,None])
     helper_test_op([(2,5,6,5,3,4)], lambda x: x[...,1,d,None], lambda x: x[...,1,o,None])
 
-  def test_slice_fancy_indexing_with_idx(self):
+  def test_slice_fancy_indexing_with_tensors(self):
     # indexing using idx with different dim
     helper_test_op([(2,3)], lambda x: x[torch.tensor([[0,0,0],[0,0,0]]), torch.tensor(1)],
                             lambda x: x[Tensor([[0,0,0],[0,0,0]]), Tensor(1)])
     helper_test_op([(2,3)], lambda x: x[torch.tensor([1]), torch.tensor([[0,0,0],[0,0,0]])],
                             lambda x: x[Tensor([1]), Tensor([[0,0,0],[0,0,0]])])
     helper_test_op([(2,3)], lambda x: x[torch.tensor([[0,0,0],[0,0,0]]), torch.tensor([2,1,1])],
                             lambda x: x[Tensor([[0,0,0],[0,0,0]]), Tensor([2,1,1])])
@@ -1392,80 +1667,61 @@
                             lambda x: x[Tensor([[0,1,-1],[-1,-2,0]]), Tensor([2,1,-1])])
 
   def test_slice_fancy_indexing_list_indices(self):
     a,b,c,d,e,i,j,k,o,p = self._get_index_randoms()
     helper_test_op([(2,5,6,5,3,4)], lambda x: x[[[0]]], lambda x: x[[[0]]])
     helper_test_op([(2,5,6,5,3,4)], lambda x: x[[0],b,c,d,:], lambda x: x[[0],j,k,o,:])
     helper_test_op([(2,5,6,5,3,4)], lambda x: x[[[[0]]],b,c,d,[[1]]], lambda x: x[[[[0]]],j,k,o,[[1]]])
-    helper_test_op([(2,5,6,5,3,4)], lambda x: x[[1],b,c,d,:], lambda x: x[[1],j,k,o,:])
     helper_test_op([(2,5,6,5,3,4)], lambda x: x[[1,0],b,c,d,:], lambda x: x[[1,0],j,k,o,:])
     helper_test_op([(2,5,6,5,3,4)], lambda x: x[a,b,c,[1,2,3],...], lambda x: x[i,j,k,[1,2,3],...])
     helper_test_op([(2,5,6,5,3,4)], lambda x: x[a,b,c,[[1],[2],[3]],...], lambda x: x[i,j,k,[[1],[2],[3]],...])
     helper_test_op([(2,5,6,5,3,4)], lambda x: x[a,[2,1,0],c,[2,1,0],e], lambda x: x[i,[2,1,0],k,[2,1,0],p])
 
   def test_slice_fancy_indexing_tuple_indices(self):
     a,b,c,d,e,i,j,k,o,p = self._get_index_randoms()
     helper_test_op([(2,5,6,5,3,4)], lambda x: x[(((0,),),)], lambda x: x[(((0,),),)])
     helper_test_op([(2,5,6,5,3,4)], lambda x: x[(0,),b,c,d,:], lambda x: x[(0,),j,k,o,:])
-    helper_test_op([(2,5,6,5,3,4)], lambda x: x[(1,),b,c,d,:], lambda x: x[(1,),j,k,o,:])
     helper_test_op([(2,5,6,5,3,4)], lambda x: x[(1,0),b,c,d,:], lambda x: x[(1,0),j,k,o,:])
     helper_test_op([(2,5,6,5,3,4)], lambda x: x[a,b,c,(1,2,3),...], lambda x: x[i,j,k,(1,2,3),...])
-    helper_test_op([(2,5,6,5,3,4)], lambda x: x[a,(2,1,0),c,(2,1,0),e], lambda x: x[i,(2,1,0),k,(2,1,0),p])
+    helper_test_op([(2,5,6,5,3,4)], lambda x: x[a,((2,),(1,),(0,)),c,(2,1,0)], lambda x: x[i,((2,),(1,),(0,)),k,(2,1,0)])
     helper_test_op([(2,5,6,5,3,4)], lambda x: x[1,(2,1,0),None,c,(2,1,0),e], lambda x: x[1,(2,1,0),None,k,(2,1,0),p])
 
   def test_slice_fancy_indexing_list_with_tensors(self):
     a,b,c,d,e,i,j,k,o,p = self._get_index_randoms()
     helper_test_op([(2,5,6,5,3,4)], lambda x: x[[a]], lambda x: x[[i]])
     helper_test_op([(2,5,6,5,3,4)], lambda x: x[[a,1]], lambda x: x[[i,1]])
     helper_test_op([(2,5,6,5,3,4)], lambda x: x[[a,[1,1]]], lambda x: x[[i,[1,1]]])
     helper_test_op([(2,5,6,5,3,4)], lambda x: x[[a,(1,1)]], lambda x: x[[i,(1,1)]])
     helper_test_op([(2,5,6,5,3,4)], lambda x: x[[a,b,c,d,e]], lambda x: x[[i,j,k,o,p]])
 
-  def test_slice_fancy_indexing_tuple_with_tensors(self):
-    a,b,c,d,e,i,j,k,o,p = self._get_index_randoms()
-    # # TypeError: only integer tensors of a single element can be converted to an index
-    # helper_test_op([(2,5,6,5,3,4)], lambda x: x[(a,),], lambda x: x[(i,),])
-    # # TypeError: only integer tensors of a single element can be converted to an index
-    # helper_test_op([(2,5,6,5,3,4)], lambda x: x[(a,1),], lambda x: x[(i,1),])
-    helper_test_op([(2,5,6,5,3,4)], lambda x: x[(a,[1,1])], lambda x: x[(i,[1,1])])
-    helper_test_op([(2,5,6,5,3,4)], lambda x: x[(a,(1,1))], lambda x: x[(i,(1,1))])
-    helper_test_op([(2,5,6,5,3,4)], lambda x: x[(a,b,c,d,e)], lambda x: x[(i,j,k,o,p)])
-
   def test_slice_fancy_indexing_errors(self):
     a = Tensor.ones(10,11,12)
-    # tensors used as indices must be int or bool tensors
+    # tensors used as indices must be int tensors
     with self.assertRaises(IndexError): a[Tensor(1.1)]
-    # shape mismatch
-    with self.assertRaises(IndexError): a[Tensor.randint(3,1,1,1), Tensor.randint(1,4,1,1), Tensor.randint(2,4,4,1)]
-    with self.assertRaises(IndexError): a[Tensor.randint(3,1,1,1), Tensor.randint(1,4,1,1,1)]
-    # TODO: currently we do not support IndexError for out of bounds idx values
-    # any out of bounds in fancy indexing returns 0
-    # ex: Tensor([1,2])[Tensor([1,2,55])].numpy() -> array([2., 0., 0.], dtype=float32)
-    # TODO: currently we do not support tensor indexing for list of list tensor
-    # ex: torch.tensor([1,2])[[[[torch.tensor(1)]]]] -> tensor([[2]])
-    # currently we return ValueError: setting an array element with a sequence.
-    # TypeError: only integer tensors of a single element can be converted to an index
+    with self.assertRaises(IndexError): a[Tensor([True, True])]
+    # shape mismatch, cannot broadcast. either exception is okay
+    with self.assertRaises((IndexError, ValueError)): a[Tensor.randint(3,1,1,1), Tensor.randint(1,4,1,1), Tensor.randint(2,4,4,1)]
+    with self.assertRaises((IndexError, ValueError)): a[Tensor.randint(3,1,1,1), Tensor.randint(1,4,1,1,1)]
 
   def test_gather(self):
     # indices cannot have gradient
     # indices cannot be negative (torch gather)
     b = torch.randint(3, size=[3,4,5], dtype=torch.int64, requires_grad=False)
     a = Tensor(b.detach().numpy().astype(np.int32), dtype=dtypes.int32, requires_grad=False)
-    helper_test_op([(4,5,6)], lambda x: x.gather(index=b, dim=0), lambda x: x.gather(idx=a, dim=0))
-    helper_test_op([(4,5,6)], lambda x: x.gather(index=b, dim=1), lambda x: x.gather(idx=a, dim=1))
-    helper_test_op([(4,5,6)], lambda x: x.gather(index=b, dim=2), lambda x: x.gather(idx=a, dim=2))
-    helper_test_op([(3,4,5)], lambda x: x.gather(index=b, dim=0), lambda x: x.gather(idx=a, dim=0))
-    self.helper_test_exception([(4,5,6)], lambda x: x.gather(index=torch.tensor([1], dtype=torch.int64), dim=0),
-                                          lambda x: x.gather(idx=Tensor([1], dtype=dtypes.int32), dim=0), expected=(RuntimeError, AssertionError))
-    self.helper_test_exception([(2,1,1)], lambda x: x.gather(index=b, dim=0),
-                                          lambda x: x.gather(idx=a, dim=0), expected=(RuntimeError, AssertionError))
+    helper_test_op([(4,5,6)], lambda x: x.gather(dim=0, index=b), lambda x: x.gather(dim=0, index=a))
+    helper_test_op([(4,5,6)], lambda x: x.gather(dim=1, index=b), lambda x: x.gather(dim=1, index=a))
+    helper_test_op([(4,5,6)], lambda x: x.gather(dim=2, index=b), lambda x: x.gather(dim=2, index=a))
+    helper_test_op([(3,4,5)], lambda x: x.gather(dim=0, index=b), lambda x: x.gather(dim=0, index=a))
+    self.helper_test_exception([(4,5,6)], lambda x: x.gather(dim=0, index=torch.tensor([1], dtype=torch.int64)),
+                                          lambda x: x.gather(dim=0, index=Tensor([1], dtype=dtypes.int32)), expected=(RuntimeError, AssertionError))
+    self.helper_test_exception([(2,1,1)], lambda x: x.gather(dim=0, index=b),
+                                          lambda x: x.gather(dim=0, index=a), expected=(RuntimeError, AssertionError))
 
   def test_scaled_product_attention(self):
-    helper_test_op([(32,8,16,64), (32,8,16,64), (32,8,16,64)], lambda x,y,z: torch.nn.functional.scaled_dot_product_attention(x,y,z),
-                                                               lambda x,y,z: Tensor.scaled_dot_product_attention(x,y,z))
+    helper_test_op([(32,8,16,64), (32,8,16,64), (32,8,16,64)], torch.nn.functional.scaled_dot_product_attention, Tensor.scaled_dot_product_attention)
     helper_test_op([(32,8,16,64), (32,8,16,64), (32,8,16,64), (32,8,16,16)],
                    lambda x,y,z,m: torch.nn.functional.scaled_dot_product_attention(x,y,z,attn_mask=m),
                    lambda x,y,z,m: Tensor.scaled_dot_product_attention(x,y,z,attn_mask=m))
 
   def test_scaled_product_attention_causal(self):
     helper_test_op([(32,8,16,64), (32,8,16,64), (32,8,16,64)],
                    lambda x,y,z: torch.nn.functional.scaled_dot_product_attention(x,y,z,is_causal=True),
@@ -1477,10 +1733,22 @@
     helper_test_op([(32,10), (32,10)], lambda x,y: torch.nn.functional.binary_cross_entropy_with_logits(x,torch.clip(y,0,1)),
                                        lambda x,y: x.binary_crossentropy_logits(y.clip(0,1)))
     helper_test_op([(32,10), (32,10)], lambda x,y: torch.nn.functional.binary_cross_entropy_with_logits(x,torch.clip(y,0,1)),
                                        lambda x,y: x.sigmoid().binary_crossentropy(y.clip(0,1)))
     helper_test_op([(32,10), (32,10)], lambda x,y: torch.nn.functional.binary_cross_entropy(x.sigmoid(),torch.clip(y,0,1)),
                                        lambda x,y: x.binary_crossentropy_logits(y.clip(0,1)))
 
+  def test_one_hot(self):
+    data = [1, 2, 4]
+    helper_test_op([], lambda: torch.nn.functional.one_hot(torch.tensor(data), 6).type(torch.int32),
+                       lambda: Tensor(data).one_hot(6), forward_only=True)
+    data = [[[1, 2, 3], [0, 3, 5]], [[1, 2, 3], [0, 3, 5]]]
+    helper_test_op([], lambda: torch.nn.functional.one_hot(torch.tensor(data), 8).type(torch.int32),
+                       lambda: Tensor(data).one_hot(8), forward_only=True)
+
+  def test_masked_fill(self):
+    helper_test_op([(32,10)], lambda x: x.masked_fill((x>0.1).detach(), -math.inf))
+    helper_test_op([(32,10)], lambda x: x.masked_fill((x<0.1).detach(), -math.inf))
+
 if __name__ == '__main__':
   np.random.seed(1337)
   unittest.main(verbosity=2)
```

### Comparing `tinygrad-0.8.0/test/test_optim.py` & `tinygrad-0.9.0/test/test_optim.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 import torch
 import unittest
-from tinygrad import Tensor, Device
+from tinygrad import Tensor, Device, dtypes
 from tinygrad.nn.optim import Adam, SGD, AdamW
 from tinygrad.helpers import CI
+from test.helpers import is_dtype_supported
 
 np.random.seed(1337)
 x_init = np.random.randn(1,4).astype(np.float32)
 W_init = np.random.randn(4,4).astype(np.float32)
 m_init = np.random.randn(1,4).astype(np.float32)
 
 class TeenyNet:
@@ -36,16 +37,20 @@
   for _ in range(steps):
     out = net.forward()
     optim.zero_grad()
     out.backward()
     optim.step()
   return net.x.detach().numpy(), net.W.detach().numpy()
 
-@unittest.skipIf(CI and Device.DEFAULT == "CUDA", "slow")
+@unittest.skipIf(CI and Device.DEFAULT in {"CUDA", "NV"}, "slow")
 class TestOptim(unittest.TestCase):
+  def setUp(self):
+    self.old_training = Tensor.training
+    Tensor.training = True
+  def tearDown(self): Tensor.training = self.old_training
 
   def _test_optim(self, tinygrad_optim, torch_optim, steps, opts, atol, rtol):
     for x,y in zip(step(Tensor, tinygrad_optim, steps, **opts),
                    step(torch.tensor, torch_optim, steps, **opts)):
       np.testing.assert_allclose(x, y, atol=atol, rtol=rtol)
 
   def _test_sgd(self, steps, opts, atol, rtol): self._test_optim(SGD, torch.optim.SGD, steps, opts, atol, rtol)
@@ -79,15 +84,15 @@
 
   def test_adam(self): self._test_adam(1, {'lr': 0.001}, 1e-5, 0)
   def test_adam_high_lr(self): self._test_adam(1, {'lr': 10}, 1e-4, 1e-4)
   def test_adamw(self): self._test_adamw(1, {'lr': 0.001}, 1e-5, 0)
   def test_adamw_high_lr(self): self._test_adamw(1, {'lr': 10}, 1e-4, 1e-4)
 
   def test_multistep_adam(self): self._test_adam(10, {'lr': 0.001}, 1e-5, 0)
-  def test_multistep_adam_high_lr(self): self._test_adam(10, {'lr': 10}, 2e-4, 5e-4)
+  def test_multistep_adam_high_lr(self): self._test_adam(10, {'lr': 10}, 2e-3, 5e-4)
 
   def test_multistep_adamw(self): self._test_adamw(10, {'lr': 0.001}, 1e-5, 0)
   def test_multistep_adamw_high_lr(self): self._test_adamw(10, {'lr': 10}, 5e-4, 2e-3)
 
   def test_duped_weights(self):
     for Opt in [Adam, AdamW, SGD]:
       losses = []
@@ -101,9 +106,30 @@
           opt.zero_grad()
           loss.backward()
           opt.step()
         losses.append(loss.numpy())
 
       np.testing.assert_allclose(losses[0], losses[1], atol=1e-4, rtol=0)
 
+  @unittest.skipUnless(is_dtype_supported(dtypes.half), "need half")
+  def test_mixed_precision(self):
+    old_default_float, dtypes.default_float = dtypes.default_float, dtypes.half
+    # weight update would overflow without upcasting
+    self._test_sgd(10, {'lr': 1e10}, 1e-6, 3e-4)
+    self._test_adam(1, {'lr': 1e10}, 1e-4, 1e-4)
+    self._test_adamw(1, {'lr': 1e10}, 1e-4, 1e-4)
+    dtypes.default_float = old_default_float
+
+  def test_assert_tensor_train(self):
+    t = Tensor.ones((1,1), requires_grad=True)
+    optimizer = Adam([t])
+    optimizer.zero_grad()
+    old_state = Tensor.training
+    t.sum().backward()
+    Tensor.training = False
+    self.assertRaises(AssertionError, optimizer.step)
+    Tensor.training = True
+    optimizer.step()
+    Tensor.training = old_state
+
 if __name__ == '__main__':
-  unittest.main()
+  unittest.main()
```

### Comparing `tinygrad-0.8.0/test/test_sample.py` & `tinygrad-0.9.0/test/test_sample.py`

 * *Files identical despite different names*

### Comparing `tinygrad-0.8.0/test/test_specific_conv.py` & `tinygrad-0.9.0/test/test_specific_conv.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
-from tinygrad.tensor import Tensor
 from tinygrad.helpers import CI
-from tinygrad import Device, dtypes
+from tinygrad import Tensor, Device, dtypes
+from test.helpers import is_dtype_supported
 # similar to test/external/external_test_gpu_ast.py, but universal
 
-@unittest.skipIf(Device.DEFAULT == "CUDA" and CI, "slow on CUDA CI")
+@unittest.skipIf(Device.DEFAULT in {"CUDA", "NV"} and CI, "slow on CUDA CI")
 class TestSpecific(unittest.TestCase):
   # from openpilot
 
   # 1x1 6 <- 24
   def test_1x1_6_24(self):
     x = Tensor.randn(1,   24*4, 32, 64)
     w = Tensor.randn(6*4, 24*4, 1,  1)
@@ -16,22 +16,22 @@
 
   def test_vec_mul(self):
     # this forces it to be an image...
     x = Tensor.ones(1, 512, 4).contiguous().reshape(1, 2048)
     w = Tensor.randn(2048, 512)
     (x @ w).reshape(1, 128, 4).contiguous().realize()
 
-  @unittest.skipIf(Device.DEFAULT in ["LLVM", "WEBGPU", "GPU", "CUDA"], "Broken on LLVM and webgpu, GPU requires cl_khr_fp16")
+  @unittest.skipUnless(is_dtype_supported(dtypes.float16), "need float16 support")
   def test_big_vec_mul(self):
     # from LLaMA
     #   0 buffer<4096, dtypes.float>                      [View((1024, 1, 1, 4), (4, 0, 0, 1), 0, None)]
     #   1 buffer<4096, dtypes.float>                      [View((1024, 1024, 4, 4), (0, 4, 1, 0), 0, None)]
     #   2 buffer<16777216, dtypes.half>                   [View((1024, 1024, 4, 4), (16384, 4, 1, 4096), 0, None)]
     x = Tensor.randn(4096).realize()
-    w = Tensor.randn(4096, 4096, device='cpu').cast(dtypes.float16).to(Device.DEFAULT).realize()
+    w = Tensor.randn(4096, 4096, dtype=dtypes.float16).realize()
     (x @ w.T).realize()
 
   # from https://dl.acm.org/doi/pdf/10.1145/3495243.3517020
 
   # ~260 GFLOPS on Adreno 640, should be 260*(720/890)*(596/710) = 176.5 on downclocked 630
   # we get 170
   def test_1x1_28_28(self):
```

### Comparing `tinygrad-0.8.0/test/test_speed_v_torch.py` & `tinygrad-0.9.0/test/test_speed_v_torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,17 @@
 os.environ["OMP_NUM_THREADS"] = "1"
 import unittest
 import torch
 torch.set_num_threads(1)
 import time
 import numpy as np
 np.set_printoptions(linewidth=160)
-from tinygrad import Device, GlobalCounters
-from tinygrad.tensor import Tensor
+from tinygrad import Tensor, Device, GlobalCounters, TinyJit
 from tinygrad.nn import Conv2d
 from tinygrad.helpers import colored, getenv, CI
-from tinygrad.jit import TinyJit
 
 IN_CHANS = [int(x) for x in getenv("IN_CHANS", "4,16,64").split(",")]
 
 torch_dt = torch.float16 if getenv("HALF", 0) else torch.float32
 torch_device = torch.device('mps' if getenv("MPS", 0) else ('cuda' if getenv("TORCHCUDA", 0) else 'cpu'))
 if str(torch_device) == "mps":
   import torch.mps
@@ -115,15 +113,15 @@
   tiny_conv.weight = Tensor(torch_conv.weight.detach().cpu().numpy())
 
   def f1(torch_dat): return torch_conv(torch_dat)
   def f2(tiny_dat): return tiny_conv(tiny_dat).realize()
   helper_test_generic(f"conv bs:{bs:3d} chans:{in_chans:3d} -> {out_chans:3d} k:{kernel_size}", f1, (torch_dat,), TinyJit(f2), (tiny_dat,))
 
 @unittest.skipIf(getenv("BIG") == 0, "no big tests")
-@unittest.skipIf(getenv("CUDACPU"), "no CUDACPU")
+@unittest.skipIf(getenv("CUDACPU") or getenv("MOCKGPU"), "no CUDACPU or MOCKGPUs")
 class TestBigSpeed(unittest.TestCase):
   def test_add(self):
     def f(a, b): return a+b
     helper_test_generic_square('add', 8192, f, f)
   def test_exp(self):
     def f(a, b): return a.exp()
     helper_test_generic_square('exp', 8192, f, f, onearg=True)
@@ -136,15 +134,15 @@
   def test_large_conv_1x1(self): helper_test_conv(bs=32, in_chans=128, out_chans=128, kernel_size=1, img_size_y=128, img_size_x=128)
   def test_large_conv_3x3(self): helper_test_conv(bs=4, in_chans=128, out_chans=128, kernel_size=3, img_size_y=130, img_size_x=130)
   def test_large_conv_5x5(self): helper_test_conv(bs=4, in_chans=128, out_chans=128, kernel_size=5, img_size_y=132, img_size_x=132)
   def test_matvec_4096_16384(self): helper_test_matvec('matvec_4096_16384', 4096, 16384)
   def test_matvec_16384_4096(self): helper_test_matvec('matvec_16384_4096', 16384, 4096)
 
 @unittest.skipIf(getenv("BIG") == 1, "only big tests")
-@unittest.skipIf(getenv("CUDACPU"), "no CUDACPU")
+@unittest.skipIf(getenv("CUDACPU") or getenv("MOCKGPU"), "no CUDACPU or MOCKGPUs")
 class TestSpeed(unittest.TestCase):
   def test_sub(self):
     def f(a, b): return a-b
     helper_test_generic_square('sub', 4096, f, f)
 
   @unittest.skipIf(CI and Device.DEFAULT == "WEBGPU", "breaking on webgpu CI")
   def test_pow(self):
```

### Comparing `tinygrad-0.8.0/test/test_symbolic_jit.py` & `tinygrad-0.9.0/test/test_symbolic_ops.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,185 +1,185 @@
 import unittest
-
-from test.helpers import assert_jit_cache_len
-from tinygrad.jit import TinyJit
-from tinygrad.helpers import getenv
 from tinygrad.shape.symbolic import Variable
+from tinygrad.helpers import getenv
 from tinygrad.tensor import Tensor
+from examples.gpt2 import Attention
 import numpy as np
 
-@unittest.skipIf(getenv("ARM64") or getenv("PTX"), "ARM64 and PTX are not supported")
-class TestSymbolicJit(unittest.TestCase):
+class TestSymbolicOps(unittest.TestCase):
   def test_plus1(self):
     def f(a): return (a+1).realize()
-    jf = TinyJit(f)
     for i in range(1, 5):
       vi = Variable("i", 1, 10).bind(i)
       a = Tensor.rand(3, i)
-      symbolic = jf(a.reshape(3, vi)).reshape(3, i).numpy()
+      symbolic = f(a.reshape(3, vi)).reshape(3, i).numpy()
       expected = f(a).numpy()
       np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
-    assert_jit_cache_len(jf, 1)
 
   def test_add(self):
     def f(a, b): return (a+b).realize()
-    jf = TinyJit(f)
     for i in range(1, 5):
       vi = Variable("i", 1, 10).bind(i)
       a = Tensor.rand(3, i)
       b = Tensor.rand(3, i)
-      symbolic = jf(a.reshape(3, vi), b.reshape(3, vi)).reshape(3, i).numpy()
+      symbolic = f(a.reshape(3, vi), b.reshape(3, vi)).reshape(3, i).numpy()
       expected = f(a, b).numpy()
       np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
-    assert_jit_cache_len(jf, 1)
 
   def test_matmul(self):
     def f(a, b): return (a@b).realize()
-    jf = TinyJit(f)
-    for i in range(1, 5):
-      vi = Variable("i", 1, 10).bind(i)
-      a = Tensor.rand(3, i)
-      b = Tensor.rand(i, 5)
-      symbolic = jf(a.reshape(3, vi), b.reshape(vi, 5)).numpy()
-      expected = f(a, b).numpy()
-      np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
-    assert_jit_cache_len(jf, 1)
-
-  def test_mixed_with_no_symbol_kernel(self):
-    def f(a, b):
-      s = (a@b).realize()
-      s = (s+s).realize() # this one does not have symbols in input
-      return s
-    jf = TinyJit(f)
     for i in range(1, 5):
       vi = Variable("i", 1, 10).bind(i)
       a = Tensor.rand(3, i)
       b = Tensor.rand(i, 5)
-      symbolic = jf(a.reshape(3, vi), b.reshape(vi, 5)).numpy()
+      symbolic = f(a.reshape(3, vi), b.reshape(vi, 5)).numpy()
       expected = f(a, b).numpy()
       np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
-    assert_jit_cache_len(jf, 2)
 
-  def test_attention(self):
-    def f(q, k, v): return Tensor.scaled_dot_product_attention(q.transpose(1, 2), k.transpose(1, 2), v.transpose(1, 2)).realize()
-    jf = TinyJit(f)
+  def test_attention(self, dropout_p=0.0):
+    def f(q, k, v): return Tensor.scaled_dot_product_attention(q.transpose(1, 2), k.transpose(1, 2), v.transpose(1, 2), dropout_p=dropout_p).realize()
     for i in range(1, 5):
       vi = Variable("i", 1, 10).bind(i)
       q = Tensor.rand(2, 1, 4, 8)
       k = Tensor.rand(2, i, 4, 8)
       v = Tensor.rand(2, i, 4, 8)
-      symbolic = jf(q, k.reshape(2, vi, 4, 8), v.reshape(2, vi, 4, 8)).reshape(2, 4, 1, 8).numpy()
+      symbolic = f(q, k.reshape(2, vi, 4, 8), v.reshape(2, vi, 4, 8)).reshape(2, 4, 1, 8).numpy()
       expected = f(q, k, v).numpy()
       np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
-    assert_jit_cache_len(jf, 5)
+
+  @unittest.skipIf(getenv("MOCKHIP"), "MOCKHIP only compiles and does not run")
+  def test_attention_training(self):
+    with Tensor.train():
+      self.test_attention(dropout_p=0.0)
+      with self.assertRaises(AssertionError):
+        # symbolic shape dropout is not supported
+        self.test_attention(dropout_p=0.5)
+
+  def test_attention_pos_0_sz_0(self):
+    Attention(128, 8)(Tensor.ones(1, 0, 128), Variable("start_pos", 0, 128).bind(0), None)
+
+  def test_attention_pos_0_sz_1(self):
+    Attention(128, 8)(Tensor.ones(1, 1, 128), Variable("start_pos", 0, 128).bind(0), None)
+
+  def test_attention_pos_0_sz_2(self):
+    Attention(128, 8)(Tensor.ones(1, 2, 128), Variable("start_pos", 0, 128).bind(0), None)
 
   def test_cat_dim0(self):
     def f(a, b): return a.cat(b, dim=0).realize()
-    jf = TinyJit(f)
     for i in range(1, 5):
       vi = Variable("i", 1, 10).bind(i)
       a = Tensor.rand(i, 3)
       b = Tensor.rand(2, 3)
-      symbolic = jf(a.reshape(vi, 3), b).reshape(i+2, 3).numpy()
+      symbolic = f(a.reshape(vi, 3), b).reshape(i+2, 3).numpy()
       expected = f(a, b).numpy()
       np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
-    assert_jit_cache_len(jf, 1)
 
   def test_cat_dim1(self):
     def f(a, b): return a.cat(b, dim=1).realize()
-    jf = TinyJit(f)
     for i in range(1, 5):
       vi = Variable("i", 1, 10).bind(i)
       a = Tensor.rand(3, i)
       b = Tensor.rand(3, 2)
-      symbolic = jf(a.reshape(3, vi), b).reshape(3, i+2).numpy()
+      symbolic = f(a.reshape(3, vi), b).reshape(3, i+2).numpy()
       expected = f(a, b).numpy()
       np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
-    assert_jit_cache_len(jf, 1)
 
   def test_cat_dim0_two_vars(self):
     def f(a, b): return a.cat(b, dim=0).realize()
-    jf = TinyJit(f)
     for i in range(1, 5):
       for j in range(1, 5):
         vi = Variable("i", 1, 10).bind(i)
         vj = Variable("j", 1, 10).bind(j)
         a = Tensor.rand(i, 3)
         b = Tensor.rand(j, 3)
-        symbolic = jf(a.reshape(vi, 3), b.reshape(vj, 3)).reshape(i+j, 3).numpy()
+        symbolic = f(a.reshape(vi, 3), b.reshape(vj, 3)).reshape(i+j, 3).numpy()
         expected = f(a, b).numpy()
         np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
-    assert_jit_cache_len(jf, 1)
 
   def test_cat_dim1_two_vars(self):
     def f(a, b): return a.cat(b, dim=1).realize()
-    jf = TinyJit(f)
     for i in range(1, 5):
       for j in range(1, 5):
         vi = Variable("i", 1, 10).bind(i)
         vj = Variable("j", 1, 10).bind(j)
         a = Tensor.rand(3, i)
         b = Tensor.rand(3, j)
-        symbolic = jf(a.reshape(3, vi), b.reshape(3, vj)).reshape(3, i+j).numpy()
+        symbolic = f(a.reshape(3, vi), b.reshape(3, vj)).reshape(3, i+j).numpy()
         expected = f(a, b).numpy()
         np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
-    assert_jit_cache_len(jf, 1)
 
-  @unittest.skip("two vars not supported")
   def test_two_vars_plus1_ij(self):
     def f(a, b): return (a@b+1).realize()
-    jf = TinyJit(f)
     for i in range(1, 5):
       for j in range(1, 5):
         vi = Variable("i", 1, 10).bind(i)
         vj = Variable("j", 1, 10).bind(j)
         a = Tensor.rand(i, 3)
         b = Tensor.rand(3, j)
-        symbolic = jf(a.reshape(vi, 3), b.reshape(3, vj)).reshape(i, j).numpy()
+        symbolic = f(a.reshape(vi, 3), b.reshape(3, vj)).reshape(i, j).numpy()
         expected = f(a, b).numpy()
         np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
-    assert_jit_cache_len(jf, 1)
 
-  @unittest.skip("two vars not supported")
   def test_two_vars_plus1_ji(self):
+    # reverse the order of variables
     def f(a, b): return (a@b+1).realize()
-    jf = TinyJit(f)
     for i in range(1, 5):
       for j in range(1, 5):
         vi = Variable("i", 1, 10).bind(i)
         vj = Variable("j", 1, 10).bind(j)
         a = Tensor.rand(j, 3)
         b = Tensor.rand(3, i)
-        symbolic = jf(a.reshape(vj, 3), b.reshape(3, vi)).reshape(j, i).numpy()
+        symbolic = f(a.reshape(vj, 3), b.reshape(3, vi)).reshape(j, i).numpy()
         expected = f(a, b).numpy()
         np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
-    assert_jit_cache_len(jf, 1)
-
-  def test_jit_symbolic_shape_mismatch(self):
-    @TinyJit
-    def add(a, b): return (a+b).realize()
-    for i in range(1, 5):
-      vi = Variable("i", 1, 10).bind(i)
-      a = Tensor.rand(3, i).reshape(3, vi)
-      b = Tensor.rand(3, i).reshape(3, vi)
-      add(a, b)
-    vi2 = Variable("i", 1, 10).bind(7)
-    a = Tensor.rand(3, 7).reshape(3, vi2)
-    bad = Tensor.rand(4, 7).reshape(4, vi2)
-    with self.assertRaises(AssertionError):
-      add(a, bad)
 
   def test_shrink(self):
-    # shrink is a movement, so we pair it with a simple function to test the JIT interaction
-    def f(a): return (a+1).realize()
-    jf = TinyJit(f)
     for i in range(1, 5):
       vi = Variable("i", 1, 10).bind(i)
       a = Tensor.rand(7, 11)
       symbolic = a.shrink(((3,5),(vi,vi+2)))
-      symbolic = jf(symbolic).numpy()
-      expected = f(a.shrink(((3,5),(i,i+2)))).numpy()
+      symbolic = symbolic.numpy()
+      expected = a.shrink(((3,5),(i,i+2))).numpy()
       np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
-    assert_jit_cache_len(jf, 1)
+
+  def test_mean(self):
+    for i in range(1, 5):
+      vi = Variable("i", 1, 10).bind(i)
+      # aixs = None
+      a = Tensor.rand(i, 3)
+      symbolic = a.reshape(vi, 3).mean().numpy()
+      expected = a.mean().numpy()
+      np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
+      # aixs = 0
+      a = Tensor.rand(i, 3)
+      symbolic = a.reshape(vi, 3).mean(0).numpy()
+      expected = a.mean(0).numpy()
+      np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
+      # aixs = 1
+      a = Tensor.rand(i, 3)
+      symbolic = a.reshape(vi, 3).mean(1).reshape(i).numpy()
+      expected = a.mean(1).numpy()
+      np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
+
+  def test_mean_2d(self):
+    for i in range(1, 5):
+      for j in range(1, 5):
+        vi = Variable("i", 1, 10).bind(i)
+        vj = Variable("j", 1, 10).bind(j)
+        # aixs = None
+        a = Tensor.rand(i, j)
+        symbolic = a.reshape(vi, vj).mean().numpy()
+        expected = a.mean().numpy()
+        np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
+        # aixs = 0
+        a = Tensor.rand(i, j)
+        symbolic = a.reshape(vi, vj).mean(0).reshape(j).numpy()
+        expected = a.mean(0).numpy()
+        np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
+        # aixs = 1
+        a = Tensor.rand(i, j)
+        symbolic = a.reshape(vi, vj).mean(1).reshape(i).numpy()
+        expected = a.mean(1).numpy()
+        np.testing.assert_allclose(symbolic, expected, atol=1e-6, rtol=1e-6)
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `tinygrad-0.8.0/test/test_symbolic_shapetracker.py` & `tinygrad-0.9.0/test/test_symbolic_shapetracker.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,27 +78,33 @@
     st = st.reshape((3*4*3,))
     assert st.var_vals == {Variable("x", 1, 100): 3}
 
 class TestShapeTrackerUnbind(unittest.TestCase):
   def test_view_unbind(self):
     v = Variable("v", 1, 100)
     bv = Variable("v", 1, 100).bind(3)
-    assert View.create(shape=(bv, 4)).unbind() == View.create(shape=(v, 4))
+    unbound_view, var_val = View.create(shape=(bv, 4)).unbind()
+    assert unbound_view == View.create(shape=(v, 4))
+    assert var_val == {v: 3}
 
   def test_reshape_unbind(self):
     v = Variable("v", 1, 100)
     bv = Variable("v", 1, 100).bind(3)
     t = Tensor.rand(3, 4).reshape(bv, 4)
-    assert t.lazydata.st.unbind() == ShapeTracker((View.create(shape=(v, 4)),))
+    unbound_st, var_val = t.lazydata.st.unbind()
+    assert unbound_st == ShapeTracker((View.create(shape=(v, 4)),))
+    assert var_val == {v: 3}
 
   def test_shrink_unbind(self):
     v = Variable("v", 1, 100)
     bv = Variable("v", 1, 100).bind(2)
     t = Tensor.rand(3, 4).shrink(((bv, bv+1), (0, 4)))
-    assert t.lazydata.st.unbind() == ShapeTracker((View.create(shape=(1, 4), offset=4*v),))
+    unbound_st, var_val = t.lazydata.st.unbind()
+    assert unbound_st == ShapeTracker((View.create(shape=(1, 4), offset=4*v),))
+    assert var_val == {v: 2}
 
 class TestSymbolicReshape(unittest.TestCase):
   def test_reshape_into_symbols_simple(self):
     for i in range(1, 6):
       vi = Variable("i", 1, 5).bind(i)
       t = Tensor.rand(i, 4).reshape(vi, 4)
       assert t.shape == (vi, 4)
```

### Comparing `tinygrad-0.8.0/test/test_tensor.py` & `tinygrad-0.9.0/test/test_tensor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import numpy as np
 import torch
 import unittest, copy
 import mmap
 from tinygrad import Tensor, Device, dtypes
-from tinygrad.helpers import temp
+from tinygrad.helpers import temp, CI
 from extra.gradcheck import numerical_jacobian, jacobian, gradcheck
+from hypothesis import given, settings, strategies as strat
+
+settings.register_profile("my_profile", max_examples=200, deadline=None)
+settings.load_profile("my_profile")
 
 x_init = np.random.randn(1,3).astype(np.float32)
 U_init = np.random.randn(3,3).astype(np.float32)
 V_init = np.random.randn(3,3).astype(np.float32)
 W_init = np.random.randn(3,3).astype(np.float32)
 m_init = np.random.randn(1,3).astype(np.float32)
 
@@ -206,21 +210,48 @@
 
     self.assertEqual(Tensor.rand(1,10,20).shape, (1,10,20))
     self.assertEqual(Tensor.rand((10,20,40)).shape, (10,20,40))
 
     self.assertEqual(Tensor.empty(1,10,20).shape, (1,10,20))
     self.assertEqual(Tensor.empty((10,20,40)).shape, (10,20,40))
 
+    with self.assertRaises(ValueError):
+      Tensor.zeros((2, 2), 2, 2)
+    with self.assertRaises(ValueError):
+      Tensor.zeros((2, 2), (2, 2))
+    with self.assertRaises(ValueError):
+      Tensor.randn((128, 128), 0.0, 0.01)
+
   def test_numel(self):
     assert Tensor.randn(10, 10).numel() == 100
     assert Tensor.randn(1,2,5).numel() == 10
     assert Tensor.randn(1,1,1,1,1,1).numel() == 1
     assert Tensor([]).numel() == 0
     assert Tensor.randn(1,0,2,5).numel() == 0
 
+  def test_len(self):
+    assert len(torch.zeros(7)) == len(Tensor.zeros(7))
+    assert len(torch.zeros(10,20)) == len(Tensor.zeros(10,20))
+    assert len(torch.zeros(10,20)) == len(Tensor.zeros(10,20,30))
+    assert len(torch.zeros(1).flatten()) == len(Tensor.zeros(1).flatten())
+
+  def test_size(self):
+    t1, t2 = torch.zeros(10,20), Tensor.zeros(10,20)
+    assert t1.size() == t2.size()
+    assert t1.size(0) == t2.size(0)
+    assert t1.size(1) == t2.size(1)
+    assert t1.size(-1) == t2.size(-1)
+    assert t1.size(-2) == t2.size(-2)
+    with self.assertRaises(IndexError): t2.size(2)
+
+  def test_tolist(self):
+    # NOTE: float16 Tensor.tolist() requires python 3.12
+    for arr in [[1,2,3], [1.5,2,3], [[1,2,3], [4,5,6]], 3]:
+      assert Tensor(arr).tolist() == torch.tensor(arr).tolist() == arr
+
   def test_element_size(self):
     for _, dtype in dtypes.fields().items():
       assert dtype.itemsize == Tensor.randn(3, dtype=dtype).element_size(), f"Tensor.element_size() not matching Tensor.dtype.itemsize for {dtype}"
 
   def test_deepwalk_ctx_check(self):
     layer = Tensor.uniform(1, 1, requires_grad=True)
     x = Tensor.randn(1, 1, 1)
@@ -281,15 +312,15 @@
     with self.assertRaises(ValueError): Tensor([[1,1,1],[[1,1,1]]])
 
   def test_tensor_copy(self):
     x = copy.deepcopy(Tensor.ones((3,3,3)))
     np.testing.assert_allclose(x.numpy(), np.ones((3,3,3)))
 
   def test_copy_from_disk(self):
-    t = Tensor.randn(30, device="CPU").to(f"disk:{temp('test_copy_from_disk')}")
+    t = Tensor.randn(30).to(f"disk:{temp('test_copy_from_disk')}")
     a = t[10:20]
     dev = a.to(Device.DEFAULT)
     np.testing.assert_allclose(a.numpy(), dev.numpy())
 
   # Regression test for https://github.com/tinygrad/tinygrad/issues/1751
   def test_copy_from_numpy_unaligned(self):
     # 2**15 is the minimum for repro
@@ -311,27 +342,77 @@
       buffered_item = Tensor([a]).item()
       assert type(buffered_item) == type(a), a
       np.testing.assert_allclose(buffered_item, a), a
       reshaped_item = Tensor([a]).reshape((1, 1, 1, 1, 1)).item()
       assert type(reshaped_item) == type(a), a
       np.testing.assert_allclose(reshaped_item, a), a
 
+  def test_no_bool(self):
+    with self.assertRaises(TypeError):
+      if Tensor(["3"]):
+        print("hi")
+
+    with self.assertRaises(TypeError):
+      _a = Tensor([3]) in [Tensor([3]), Tensor([4]), Tensor([5])]
+
+  def test_repr_with_grad(self):
+    a = Tensor([1])
+    b = Tensor([1])
+    c = (a + b).mean().backward()
+    print(c)
+
+@unittest.skipIf(CI and Device.DEFAULT in {"GPU", "CUDA", "METAL", "NV", "AMD"}, "no GPU CI")
+class TestMoveTensor(unittest.TestCase):
+  d0, d1 = f"{Device.DEFAULT}:0", f"{Device.DEFAULT}:1"
+  @given(strat.sampled_from([d0, d1]), strat.sampled_from([d0, d1]),
+         strat.sampled_from([dtypes.float16, dtypes.float32]), strat.sampled_from([True, False, None]))
+  def test_to_preserves(self, src, dest, dtype, requires_grad):
+    s = Tensor([1, 2, 3], device=src, dtype=dtype, requires_grad=requires_grad)
+    if requires_grad: s.sum().backward()
+    t = s.to(dest)
+    np.testing.assert_equal(s.numpy(), t.numpy())
+    assert s.dtype == t.dtype
+    assert s.requires_grad == t.requires_grad
+    if requires_grad:
+      np.testing.assert_equal(s.grad.numpy(), t.grad.numpy())
+
+  @given(strat.sampled_from([dtypes.float16, dtypes.float32]), strat.sampled_from([True, False, None]))
+  def test_shard_preserves(self, dtype, requires_grad):
+    s = Tensor([1, 2, 3], dtype=dtype, requires_grad=requires_grad)
+    t = s.shard((f"{Device.DEFAULT}:0", f"{Device.DEFAULT}:1"))
+    np.testing.assert_equal(s.numpy(), t.numpy())
+    assert s.dtype == t.dtype
+    assert s.requires_grad == t.requires_grad
+
+  @given(strat.sampled_from([d0, d1]))
+  def test_same_dev(self, dev):
+    x = Tensor([1,2,3], device=dev)
+    y = x.to(dev)
+    assert x is y
+
+  def test_to_grad(self):
+    x = Tensor.eye(3, requires_grad=True, device=self.d0)
+    y = Tensor([[2.0,0,-2.0]], requires_grad=True, device=self.d0)
+    z = y.matmul(x).to(self.d1).sum()
+    z.backward()
+    np.testing.assert_equal(x.grad.numpy(), [[2,2,2],[0,0,0],[-2,-2,-2]])
+
 class TestZeroShapeTensor(unittest.TestCase):
   def test_shape_stride(self):
-    t = Tensor.rand(3, 2, 0)
+    t = Tensor.empty(3, 2, 0)
     assert t.shape == (3, 2, 0)
     # numpy has stride 0, 0, 0; torch has stride 2, 1, 1
     assert t.lazydata.st.real_strides() == (0, 0, 1)
 
-    t = Tensor.rand(3, 0, 2)
+    t = Tensor.empty(3, 0, 2)
     assert t.shape == (3, 0, 2)
     # numpy has stride 0, 0, 0; torch has stride 2, 2, 1
     assert t.lazydata.st.real_strides() == (0, 2, 1)
 
-    t = Tensor.rand(0, 0, 0)
+    t = Tensor.empty(0, 0, 0)
     assert t.shape == (0, 0, 0)
     # numpy has stride 0, 0, 0; torch has stride 1, 1, 1
     assert t.lazydata.st.real_strides() == (0, 0, 1)
 
   def test_rand(self):
     t = Tensor.rand(3, 2, 0)
     assert t.shape == (3, 2, 0)
@@ -357,51 +438,47 @@
     assert a.shape == (7, 0)
     np.testing.assert_equal(a.numpy(), np.zeros((7, 0)))
     with self.assertRaises(AssertionError):
       # cannot reshape from size 0 to size 1
       a = t.reshape(())
 
   def test_expand(self):
-    t = Tensor.full((3, 2, 0), 12).expand((6, 2, 0))
+    t = Tensor.full((1, 2, 0), 12).expand((6, 2, 0))
     assert t.shape == (6, 2, 0)
     np.testing.assert_equal(t.numpy(), np.full((6, 2, 0), 12))
 
   def test_pad(self):
     t = Tensor.rand(3, 2, 0).pad((None, None, (1, 1)), 1)
     assert t.shape == (3, 2, 2)
     np.testing.assert_equal(t.numpy(), np.ones((3, 2, 2)))
 
-    if Device.DEFAULT != "TORCH":
-      # torch does not support padding non-zero dim with 0-size. torch.nn.functional.pad(torch.zeros(3,2,0), [0,0,0,4,0,0])
-      t = Tensor.rand(3, 2, 0).pad((None, (1, 1), None), 1)
-      assert t.shape == (3, 4, 0)
-      np.testing.assert_equal(t.numpy(), np.ones((3, 4, 0)))
-
-      t = Tensor.rand(3, 2, 0).pad(((1, 1), None, None), 1)
-      assert t.shape == (5, 2, 0)
-      np.testing.assert_equal(t.numpy(), np.ones((5, 2, 0)))
+    t = Tensor.rand(3, 2, 0).pad((None, (1, 1), None), 1)
+    assert t.shape == (3, 4, 0)
+    np.testing.assert_equal(t.numpy(), np.ones((3, 4, 0)))
+
+    t = Tensor.rand(3, 2, 0).pad(((1, 1), None, None), 1)
+    assert t.shape == (5, 2, 0)
+    np.testing.assert_equal(t.numpy(), np.ones((5, 2, 0)))
 
   def test_shrink_into_zero(self):
     t = Tensor.rand(3, 4).realize()
     assert t.shrink((None, (2, 2))).realize().shape == (3, 0)
     assert t.shrink(((2, 2), None)).realize().shape == (0, 4)
     assert t.shrink(((2, 2), (2, 2))).realize().shape == (0, 0)
 
   def test_cat(self):
     s = Tensor.rand(3, 2, 2)
     t = Tensor.rand(3, 2, 0).cat(s, dim=2)
     assert t.shape == (3, 2, 2)
     np.testing.assert_equal(t.numpy(), s.numpy())
 
-    if Device.DEFAULT != "TORCH":
-      # torch does not support padding non-zero dim with 0-size. torch.nn.functional.pad(torch.zeros(3,2,0), [0,0,0,4,0,0])
-      s = Tensor.rand(3, 4, 0)
-      t = Tensor.rand(3, 2, 0).cat(s, dim=1)
-      assert t.shape == (3, 6, 0)
-      np.testing.assert_equal(t.numpy(), np.zeros((3, 6, 0)))
+    s = Tensor.rand(3, 4, 0)
+    t = Tensor.rand(3, 2, 0).cat(s, dim=1)
+    assert t.shape == (3, 6, 0)
+    np.testing.assert_equal(t.numpy(), np.zeros((3, 6, 0)))
 
   def test_elementwise(self):
     a = Tensor.rand(3, 2, 0)
     a_exp = a.exp()
     assert a_exp.shape == (3, 2, 0)
     np.testing.assert_equal(a_exp.numpy(), np.exp(a.numpy()))
 
@@ -431,11 +508,63 @@
     assert a.shape == (3, 2, 1)
     np.testing.assert_equal(a.numpy(), np.sum(np.zeros((3, 2, 0)), axis=2, keepdims=True))
 
   def test_reduce_default(self):
     np.testing.assert_equal(Tensor([]).max().numpy(), -float("inf"))
     np.testing.assert_equal(Tensor([]).min().numpy(), float("inf"))
     np.testing.assert_equal(Tensor([]).sum().numpy(), 0)
-    np.testing.assert_equal(Tensor([]).mean().numpy(), 0)
+    np.testing.assert_equal(Tensor([]).mean().numpy(), float("nan"))
+
+class TestTensorCreationDevice(unittest.TestCase):
+  # test auxiliary tensors are created on the same device
+  def test_one_hot(self):
+    y = Tensor([1, 2, 3]).to("CLANG")
+    x = y.one_hot(10)
+    x.realize()
+
+class TestTrainMode(unittest.TestCase):
+  def test_train_mode(self):
+    assert not Tensor.training
+    @Tensor.train()
+    def f():
+      assert Tensor.training
+    f()
+    assert not Tensor.training
+
+class TestInferenceMode(unittest.TestCase):
+  def test_inference_mode(self):
+    x = Tensor(x_init, requires_grad=True)
+    m = Tensor(m_init, requires_grad=True)
+    W = Tensor(W_init, requires_grad=True)
+    with Tensor.inference_mode():
+      tmp = x.mul(m)
+      mm = tmp.matmul(W)
+      out = mm.relu()
+      out = out.sum()
+      out.backward()
+    assert x.grad is None
+    assert m.grad is None
+    assert tmp.grad is None
+    assert mm.grad is None
+    assert W.grad is None
+    assert W.requires_grad
+
+  def test_no_grad_mode_context_manager(self):
+    x = Tensor(x_init, requires_grad=True)
+    m = Tensor(m_init, requires_grad=True)
+    W = Tensor(W_init, requires_grad=True)
+    @Tensor.inference_mode()
+    def f(x, m, W):
+      tmp = x.mul(m)
+      mm = tmp.matmul(W)
+      out = mm.relu()
+      out = out.sum()
+      out.backward()
+      assert x.grad is None
+      assert m.grad is None
+      assert tmp.grad is None
+      assert mm.grad is None
+      assert W.grad is None
+    f(x, m, W)
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `tinygrad-0.8.0/test/test_tensor_data.py` & `tinygrad-0.9.0/test/test_tensor_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,20 +27,29 @@
     assert dat.format == "i"
     assert dat.itemsize == 4
     assert dat.tolist() == [[1, 2], [3, 4]]
     assert dat.shape == (2,2)
     assert dat[0, 0] == 1
     assert dat[1, 1] == 4
 
+  def test_data_const(self):
+    a = Tensor(3, dtype=dtypes.int32)
+    dat = a.data()
+    assert dat.format == "i"
+    assert dat.itemsize == 4
+    assert dat.tolist() == 3
+    assert dat.shape == ()
+
   def test_data_float32(self):
     a = Tensor([[1,2.5],[3,4]], dtype=dtypes.float32)
     dat = a.data()
     assert dat.format == "f"
     assert dat[0, 1] == 2.5
 
+  @unittest.skip("requires python 3.12")
   def test_data_float16(self):
     a = Tensor([[1,2.5],[3,4]], dtype=dtypes.float16)
     dat = a.data()
     assert dat.format == "e"
     assert dat.shape == (2,2)
     # NOTE: python can't deref float16
```

### Comparing `tinygrad-0.8.0/test/test_zero_copy.py` & `tinygrad-0.9.0/test/test_zero_copy.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from tinygrad import Tensor, Device
 import time
 
 def time_tensor_numpy(out:Tensor):
   times = []
   for _ in range(5):
     st = time.perf_counter()
-    out.lazydata.base.realized.toCPU()
+    out.lazydata.base.realized.as_buffer(allow_zero_copy=True)
     et = time.perf_counter() - st
     times.append(et)
   return min(times)
 
 N = 4096
 class TestZeroCopy(unittest.TestCase):
   @unittest.skipIf(Device.DEFAULT not in {"CLANG", "LLVM", "CPU", "METAL"}, "device isn't zero copy")
```

### Comparing `tinygrad-0.8.0/tinygrad/codegen/kernel.py` & `tinygrad-0.9.0/tinygrad/codegen/kernel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,150 +1,140 @@
 from __future__ import annotations
-import os, math, itertools
+import math, itertools
 from typing import NamedTuple, Optional, List, Tuple, cast, Dict, Union
-from tinygrad.ops import LazyOp, FlopCounter, get_lazyop_info, UnaryOps, BinaryOps, ReduceOps, MemBuffer, ConstBuffer, BufferOps
-from tinygrad.device import Device, Compiled
+from tinygrad.ops import LazyOp, UnaryOps, BinaryOps, ReduceOps, MemBuffer, ConstBuffer, BufferOps, UNSAFE_PAD_OPS
+from tinygrad.device import Device
+from tinygrad.renderer import Renderer, TensorCore
 from tinygrad.dtype import dtypes, ImageDType, DType
-from tinygrad.helpers import dedup, colored, ansilen, getenv, prod, DEBUG, round_up, all_int
-from tinygrad.shape.shapetracker import ShapeTracker, get_contraction
+from tinygrad.helpers import colored, ansilen, dedup, flatten, getenv, prod, DEBUG, round_up, all_int, get_contraction
+from tinygrad.shape.shapetracker import ShapeTracker
 from tinygrad.shape.symbolic import sint
 from tinygrad.shape.view import View, strides_for_shape
 from dataclasses import dataclass
 from enum import Enum, auto
 
 class OptOps(Enum):
-  UPCAST = auto(); UPCASTMID = auto(); UNROLL = auto(); LOCAL = auto(); LASTLOCAL = auto() # noqa: E702
+  TC = auto(); UPCAST = auto(); UPCASTMID = auto(); UNROLL = auto(); LOCAL = auto() # noqa: E702
   GROUP = auto(); GROUPTOP = auto(); NOLOCALS = auto(); PADTO = auto() # noqa: E702
   def __lt__(self, x:OptOps): return self.value < x.value
 
+class KernelOptError(Exception): pass
+
+def check(cond:bool, msg:str=""):
+  if not cond: raise KernelOptError(msg)
+
 @dataclass(frozen=True, order=True)
 class Opt:
   op: OptOps
   axis: Optional[int] = None
   amt: Optional[int] = None
   def __repr__(self): return f"Opt(op={self.op}, axis={self.axis}, amt={self.amt})"
-
-@dataclass(frozen=True)
-class TensorCore:
-  device: str
-  dims: List[int]
-  dtype_in: DType
-  dtype_out: DType
-  threads: List[Tuple[int,int]] # list of (TC dim,amt) that construct the warp thread structure
-  upcast_dim: int # which TC dim to upcast
-  thread_local_aliases: List[List[List[int]]] # a list of [threads_1, ..., threads_n, upcast_1(unrolled), upcast_2(upcast)] defining the alias (-1 is upcast, 1-n is warp threads) for each TC dim # noqa: E501
-  thread_local_sizes: List[int] # in each thread, the number of elements stored in registers for each TC dim
-  arch: Optional[str] = None
-  def __str__(self): return f"tensor_core<{self.device}, {self.dims}, {self.dtype_in}, {self.dtype_out}>"
-
-tensor_cores: Dict[str, List[TensorCore]] = {
-  "METAL": [
-    TensorCore(device="METAL", dims=[8,8,8], dtype_in=dtypes.float, dtype_out=dtypes.float, upcast_dim=0, threads=[(0,2),(1,4),(0,2),(1,2)], thread_local_sizes=[2,2,2], thread_local_aliases= [ [[4],[0],[2],[0],[-1, 1, 3],[0]], [[0],[3],[0],[1],[2, 4],[-1]], [[4],[3],[2],[1],[0],[-1]] ], arch="arm64"), # noqa: E501
-    # TODO: enable half @ half -> half tensor core with correct dtypes in uop
-    # TensorCore(device="METAL", dims=[8,8,8], dtype_in=dtypes.half,  dtype_out=dtypes.half,  upcast_dim=0, threads=[(0,2),(1,4),(0,2),(1,2)], thread_local_sizes=[2,2,2], thread_local_aliases= [ [[4],[0],[2],[0],[-1, 1, 3],[0]], [[0],[3],[0],[1],[2, 4],[-1]], [[4],[3],[2],[1],[0],[-1]] ], arch="arm64"), # noqa: E501
-  ],
-  "HIP": [
-    TensorCore(device="HIP", dims=[16,16,16], dtype_in=dtypes.half, dtype_out=dtypes.float, upcast_dim=1, threads=[(0,16),(1,2)], thread_local_sizes=[16,16,8], thread_local_aliases=[ [[0],[0],[-1],[1]], [[0],[1],[-1],[0]], [[0],[1],[0],[2,-1]] ]),  # noqa: E501
-    TensorCore(device="HIP", dims=[16,16,16], dtype_in=dtypes.half, dtype_out=dtypes.half,  upcast_dim=1, threads=[(0,16),(1,2)], thread_local_sizes=[16,16,8], thread_local_aliases=[ [[0],[0],[-1],[1]], [[0],[1],[-1],[0]], [[0],[1],[0],[2,-1]] ]),  # noqa: E501
-  ]
-}
+  def real_axis(self, k:Kernel):
+    if self.axis is None: return -1
+    if self.op is OptOps.UNROLL: return k.first_reduce+self.axis
+    if self.op in {OptOps.GROUP, OptOps.GROUPTOP}: return k.first_reduce+k.group_for_reduces+self.axis
+    return self.axis
+
+class TensorCoreOptions(NamedTuple):
+  bufs: Tuple[int, int] # the local aliased buffers for A and B
+  axes: List[int] # the location of the original N and M axes if still in the shape
+  axes_exist: List[bool] # true if the original N and M axes are still in the shape
+  def fix_axes(self, removed_axis:int): # adjust the TC axes if necesssary when an dimension is removed
+    for tc_dim in [i for i in range(2) if self.axes_exist[i]]:
+      if removed_axis < self.axes[tc_dim]: self.axes[tc_dim] -= 1
+      elif removed_axis == self.axes[tc_dim]: self.axes_exist[tc_dim] = False
 
 class LocalBuffer(NamedTuple):
   name: str
   size: int
   dtype: DType = dtypes.float32
   realized: None = None
   def __str__(self): return f"localbuffer<{self.name}[{self.size}]>"
 
-class LinearizerOptions(NamedTuple):
-  device: str = ""
-  # TODO: make this generic with a list of supported types
-  supports_float4: bool = True
-  supports_float4_alu: bool = True
-  has_local: bool = True
-  has_shared: bool = True
-  # NOTE: these two should be in z,y,x(reversed) order for cstyle backends, they are flipped when kernel is rendered
-  global_max: Optional[List[int]] = None
-  local_max: Optional[List[int]] = None
-
 class Kernel:
-  def __init__(self, ast:LazyOp, opts:Optional[LinearizerOptions]=None):
-    self.opts = opts or (device.linearizer_opts if isinstance(device:=Device[Device.DEFAULT], Compiled) else LinearizerOptions())
+  def __init__(self, *ast:LazyOp, opts:Optional[Renderer]=None):
+    self.opts = opts if opts is not None else Device[Device.DEFAULT].renderer
+    assert all(op.op is BufferOps.STORE for op in ast), f"kernels must have stores as the output, got {ast}"
+    assert len(set(op.arg.st.size for op in ast)) == 1, f"all outbufs should have the same size, got {[op.arg.st for op in ast]}"
     self.ast = ast
-    assert ast.op == BufferOps.STORE, f"kernels must have a store as the output, got {ast.op}"
-
-    # fetch lazyop info
-    self.info: FlopCounter = get_lazyop_info(self.ast)
+    self.lazyops = flatten([op.lazyops for op in self.ast])
 
     # there's only allowed to be one reduceop
-    reduceops = [x for x in self.ast.lazyops if x.op in ReduceOps]
-    assert len(dedup(reduceops)) <= 1, "max one reduce op in an ast"
-    self.reduceop = reduceops[0] if reduceops else None
-
-    self.bufs: List[Union[MemBuffer, ConstBuffer, LocalBuffer]] = dedup([x.arg for x in self.ast.lazyops if x.op in BufferOps])
-    assert isinstance(self.bufs[0], MemBuffer) and self.bufs[0].idx == 0, f"buffer 0 is not the store buffer {self.bufs[0]}"
+    cached_ordered_lazyops: Dict[LazyOp, List[LazyOp]] = {}
+    def ordered_lazyops(op):
+      if op not in cached_ordered_lazyops: cached_ordered_lazyops[op] = dedup([item for x in op.src for item in ordered_lazyops(x)] + [op])
+      return cached_ordered_lazyops[op]
+    self.reduceops = dedup([x for out in self.ast for x in ordered_lazyops(out) if x.op in ReduceOps])
+    assert len(self.reduceops) < 2, "Only one reduceop allowed"
+
+    self.outbufs, self.vars = [x.arg for x in self.ast], flatten([x.vars() for x in self.ast])
+    loadops = [BufferOps.LOAD, BufferOps.CONST]
+    self.bufs: List[Union[MemBuffer, ConstBuffer, LocalBuffer]] = self.outbufs + dedup([x.arg for x in self.lazyops if x.op in loadops])
 
     # get earlybufs, before the one reduce op
-    self.earlybufs = [x.arg for x in self.reduceop.lazyops if x.op in BufferOps] if self.reduceop else []
+    self.earlybufs = [x.arg for reduceop in self.reduceops for x in reduceop.lazyops if x.op in BufferOps]
     self.full_buf_index: int = self.bufs.index(self.earlybufs[0]) if self.earlybufs else 0
 
     # create new shapetrackers inside this kernel, we will permute them
     self.sts: List[ShapeTracker] = [x.st for x in cast(List[Union[MemBuffer, ConstBuffer]], self.bufs)]
 
     # move all reduce axes to the end
-    reduce = list(enumerate(zip(self.full_shape, self.sts[0].shape)))
+    reduce = list(enumerate(zip(self.full_shape, self.output_shape)))
     permute = tuple([i for i,(s,n) in reduce if s == n] + [i for i,(s,n) in reduce if s != n])
     self.reshape_and_permute(None, permute)
 
     # parameters for optimization
     self.applied_opts: List[Opt] = []
-    self.group_for_reduce: List[int] = []
+    self.group_for_reduces: int = 0
     self.upcasted: int = 0
     self.local_dims: int = 0
     self.local_alias: Dict[int, LocalBuffer] = {}
     self.tensor_core: Optional[TensorCore] = None
+    self.tensor_core_opts: Optional[TensorCoreOptions] = None
     self.dont_use_locals: bool = False
 
     # group simplifies
     self.simplify_ones()
     self.simplify_merge_adjacent()
 
     # cache
     self.applied_opts_cache: Optional[List[Opt]] = None
 
   def copy(self):
     ret = type(self).__new__(type(self))
 
     # base linearizer params
-    ret.opts, ret.ast = self.opts, self.ast
+    ret.opts, ret.ast, ret.lazyops = self.opts, self.ast, self.lazyops
 
     # things downstream of the AST
-    # NOTE: we copy bufs for local buffers and sts for optimizations
-    ret.info, ret.reduceop, ret.bufs, ret.earlybufs, ret.full_buf_index, ret.sts = \
-      self.info, self.reduceop, self.bufs[:], self.earlybufs, self.full_buf_index, self.sts[:]
+    ret.reduceops, ret.outbufs, ret.vars, ret.bufs, ret.earlybufs, ret.full_buf_index = \
+      self.reduceops, self.outbufs, self.vars, [x for x in self.bufs if not isinstance(x, LocalBuffer)], self.earlybufs, self.full_buf_index
+    ret.sts = self.sts[:len(ret.bufs)] # NOTE: must redo the local buffers with TC in beam
 
     # parameters for optimizations
-    ret.applied_opts, ret.group_for_reduce, ret.upcasted, ret.local_dims, ret.local_alias, ret.tensor_core, ret.dont_use_locals = \
-      self.applied_opts[:], self.group_for_reduce[:], self.upcasted, self.local_dims, self.local_alias.copy(), self.tensor_core, self.dont_use_locals
+    ret.applied_opts, ret.group_for_reduces, ret.upcasted, ret.local_dims, ret.dont_use_locals = \
+      self.applied_opts[:], self.group_for_reduces, self.upcasted, self.local_dims, self.dont_use_locals
+    ret.tensor_core, ret.tensor_core_opts, ret.local_alias = self.tensor_core, self.tensor_core_opts, {}
 
     # uncached since linearize didn't run
     ret.applied_opts_cache = None
 
     return ret
 
   @property
   def membufs(self) -> List[MemBuffer]: return [x for x in self.bufs if isinstance(x, MemBuffer)]
 
   # TODO: these need more tests or it might silently be no-op
   def shape_offsets(self, i:int): return itertools.product(*[list(range(cast(int, s))) for s in self.sts[i].shape[self.shape_len-self.upcasted:][::-1]]) if self.upcasted > 0 else [tuple()]  # noqa: E501
   def float4_axis(self, i:int): return [x-(self.shape_len-self.upcasted) for x in self.sts[i].unit_stride_axes() if x >= self.shape_len-self.upcasted and self.sts[i].shape[x]%4 == 0]  # noqa: E501
 
-  def upcasted_axis(self, i:int):
-    return list(zip(self.sts[i].shape[self.shape_len-self.upcasted:],
-                    self.sts[i].real_strides()[self.shape_len-self.upcasted:],
+  def upcasted_axis(self, i:int) -> List[Tuple[int, Optional[sint], bool]]:
+    upcasted_shape, upcasted_stride = self.sts[i].shape[self.shape_len-self.upcasted:], self.sts[i].real_strides()[self.shape_len-self.upcasted:]
+    assert all_int(upcasted_shape), f"cannot upcast a symbolic amount {upcasted_shape=}"
+    return list(zip(upcasted_shape, upcasted_stride,
                     [x!=y for x,y in zip(self.sts[0].shape[self.shape_len-self.upcasted:], self.full_shape[self.shape_len-self.upcasted:])]))
 
   # TODO: is there a better way to write this?
   def acc_offsets(self, i:int) -> List[int]:
     if self.upcasted == 0: return [0]
     upcasted_i = self.upcasted_axis(i)
     acc_strides = [x*(1-upcasted_i[::-1][i][2]) for i,x in enumerate(strides_for_shape(tuple(1 if r else s for s,_,r in upcasted_i[::-1])))]
@@ -155,28 +145,31 @@
     return [x for x in self.sts[i].unit_stride_axes() if x >= self.shape_len-self.upcasted and self.sts[i].shape[x] > 1] if should_upcast else []
 
   @property
   def first_reduce(self) -> int:
     return [x!=y for x,y in zip(self.sts[0].shape[:self.shape_len-self.upcasted]+(0,), self.full_shape[:self.shape_len-self.upcasted]+(1,))].index(True)  # noqa: E501
 
   @property
+  def reduceop(self) -> Optional[LazyOp]: return self.reduceops[0] if len(self.reduceops) > 0 else None
+
+  @property
   def output_shape(self) -> Tuple[sint, ...]: return self.sts[0].shape
 
   @property
   def full_shape(self) -> Tuple[sint, ...]: return self.sts[self.full_buf_index].shape
 
   @property
   def full_unupcasted_shape(self) -> Tuple[sint, ...]: return self.full_shape[:self.shape_len-self.upcasted]
 
   @property
   def shape_len(self) -> int: return len(self.sts[0].shape)
 
   @property
   def upcast_in_mid_reduce_axes(self) -> List[int]:
-    return [j for j in range(self.first_reduce, self.first_reduce+len(self.group_for_reduce)) if self.full_shape[j] == self.sts[0].shape[j]]
+    return [j for j in range(self.first_reduce, self.first_reduce+self.group_for_reduces) if self.full_shape[j] == self.sts[0].shape[j]]
 
   @property
   def global_dims(self) -> int: return self.first_reduce-self.local_dims
 
   # there's eight chunks of the shape
   # blue   -- global dims
   # cyan   -- local dims (warp ones first)
@@ -188,18 +181,18 @@
   # purple -- reduce upcasted
   # yellow -- normal upcasted dimensions
   def colors(self) -> List[str]:
     # first non local non reduce dims are global (blue)
     colors = ["blue"] * self.global_dims if not self.dont_use_locals else ["BLUE"] * self.global_dims
     # after global are local_dims; warp ones used in tensor cores must be closest to first_reduce (cyan)
     colors += ["cyan"] * self.local_dims
-    # between first_reduce and first_reduce + group_for_reduce, they are either upcast mid reduce (white), or late upcasted (green)
-    colors += ["white" if i in self.upcast_in_mid_reduce_axes else "green" for i in range(self.first_reduce, self.first_reduce + len(self.group_for_reduce))]  # noqa: E501
-    # between first_reduce + group_for_reduce and upcasted, they are reduce (red)
-    colors += ["red"] * ((self.shape_len-self.upcasted) - (self.first_reduce + len(self.group_for_reduce)))
+    # between first_reduce and first_reduce + group_for_reduces, they are either upcast mid reduce (white), or late upcasted (green)
+    colors += ["white" if i in self.upcast_in_mid_reduce_axes else "green" for i in range(self.first_reduce, self.first_reduce + self.group_for_reduces)]  # noqa: E501
+    # between first_reduce + group_for_reduces and upcasted, they are reduce (red)
+    colors += ["red"] * ((self.shape_len-self.upcasted) - (self.first_reduce + self.group_for_reduces))
     # upcasted dimensions are reduce (magenta) or normal (yellow)
     colors += ["magenta" if self.full_shape[i] != self.sts[0].shape[i] else "yellow" for i in range(self.shape_len-self.upcasted, self.shape_len)]
     assert len(colors) == self.shape_len, "colors size mismatch"
     return colors
 
   def colored_shape(self, pad:Optional[int]=None, dense=False) -> str:
     ret = ' '.join(colored(s, color) for s,color in zip([f"{s:4d}" if isinstance(s, int) and not dense else s for s in self.full_shape], self.colors()))  # noqa: E501
@@ -215,15 +208,15 @@
       if new_shape_fxn is not None: st = st.reshape(tuple(new_shape_fxn(st.shape)))
       if axis is not None: st = st.permute(tuple(axis))
       new_sts.append(st)
     self.sts = new_sts
 
   # drops the final dimension
   def upcast(self):
-    assert self.full_shape[-1] != 1, "can't upcast a dimension with size 1"
+    check(self.full_shape[-1] != 1, "can't upcast a dimension with size 1")
     self.upcasted += 1
 
   # axis : the axis to pull from
   # amount : the amount to take
   # top : if you want to pull that amount from the top
   # insert_before : place to insert the new stuff
   def shift_to(self, axis, amount, top=False, insert_before=None):
@@ -238,27 +231,27 @@
 
   def simplify_ones(self) -> bool:
     # remove places where the shape is all ones
     # TODO: this should be factored in to multi shape stride
     if self.shape_len == 0: return False
     all_ones = [s==1 for s in self.full_shape]
     self.local_dims -= sum(all_ones[self.first_reduce-self.local_dims:self.first_reduce])
-    self.upcasted -= sum(all_ones[self.shape_len-self.upcasted:])
+    self.upcasted -= sum(all_ones[self.shape_len-self.upcasted:]) # TODO: no necessary since upcasted axis can't be un-upcasted
     self.reshape_and_permute(lambda shape: [x for i,x in enumerate(shape) if not all_ones[i]], None)
     return any(all_ones)
 
   def simplify_merge_adjacent(self):
     if self.shape_len == 0: return
     shapes, strides = [x.shape for x in self.sts], [x.real_strides() for x in self.sts]
 
     # if it's an image, insert fake strides such that this fusion doesn't happen across image axes
     if isinstance(self.bufs[0].dtype, ImageDType):
       base_shape = self.bufs[0].dtype.shape
       if shape_idx_groups := get_contraction(self.output_shape, base_shape):
-        special_strides: Tuple[int, ...] = tuple()
+        special_strides: Tuple[sint, ...] = tuple()
         for i,g in enumerate(shape_idx_groups):
           shape_piece = tuple(self.output_shape[x] for x in g)
           assert prod(shape_piece) == base_shape[i], f"get_contraction was wrong? {shape_piece} != {base_shape[i]}"
           special_strides += strides_for_shape(shape_piece)
         # adding the fake image shape
         shapes.append(self.output_shape)
         strides.append(special_strides)
@@ -277,43 +270,40 @@
       for j in range(len(shapes)):
         if mergeable: rets[j][-1] = (rets[j][-1][0] * shapes[j][i], strides[j][i])
         else: rets[j].append((shapes[j][i], strides[j][i]))
 
     # do the reshapes
     for i,x in enumerate(rets[:len(self.sts)]): self.sts[i] = self.sts[i].reshape(tuple([y[0] for y in x]))
 
-  # ******************** GPU simplifiers ********************
+  # ******************** helpers ********************
 
-  def _limit_size(self, x: Tuple[int], max_size: List) -> Tuple[int, ...]:
-    new_shape,dims = list(x), len(x)
-    for i in range(dims):
-      next_idx = (i + 1) % dims
+  def _limit_size(self, x: Tuple[int], max_size: List[Union[int,float]]) -> Tuple[int, ...]:
+    new_shape = list(x)
+    for i in range(len(new_shape)):
+      next_idx = (i + 1) % len(new_shape)
       while new_shape[i] > max_size[i]:
+        # TODO: what if new_shape[i] is not a multiple of 2??
         new_shape[i] = new_shape[i] // 2
-        if (new_shape[next_idx] <= max_size[next_idx]):
-          new_shape[next_idx] = new_shape[next_idx] * 2
-        else:
-          next_idx = (next_idx + 1) % dims
-          new_shape[next_idx] = new_shape[next_idx] * 2
+        next_idx = next_idx if new_shape[next_idx] <= max_size[next_idx] else (next_idx + 1) % len(new_shape)
+        new_shape[next_idx] = new_shape[next_idx] * 2
     return tuple(new_shape)
 
   def limit_dims_to_max(self, global_max: List[int], local_max: List[int]):
     # Check the global allocation limit, current the global_size will be flipped during codegen
     # and then padded right with 1s if its length < 3 which makes this part a bit awkward to write
-    global_dims = self.first_reduce-self.local_dims
-    if global_dims > 0:
+    if self.global_dims > 0:
       if global_max:
-        tmp = global_max[:global_dims] + (local_max[:self.local_dims] if local_max else [])
-        if max(global_max) < max(self.full_shape[:global_dims]):
+        tmp = global_max[:self.global_dims] + (local_max[:self.local_dims] if local_max else [])
+        if max(global_max) < max(self.full_shape[:self.global_dims]):
           self.reshape_and_permute(lambda x: self._limit_size(x, tmp + [math.inf] * (len(self.full_shape)-len(tmp))), None)
-        assert max(global_max) >= max(self.full_shape[:global_dims]), f"device max allocation {max(self.full_shape[:global_dims])} exceeds global dim maximum {max(global_max)}"  # noqa: E501
-      for i in range(global_dims-1):
+        assert max(global_max) >= max(self.full_shape[:self.global_dims]), f"device max allocation {max(self.full_shape[:self.global_dims])} exceeds global dim maximum {max(global_max)}"  # noqa: E501
+      for i in range(self.global_dims-1):
         if i < len(global_max) and self.full_shape[i] > global_max[i]:
           order = list(range(len(self.full_shape)))
-          order[i], order[global_dims-1] = order[global_dims-1], order[i]
+          order[i], order[self.global_dims-1] = order[self.global_dims-1], order[i]
           self.reshape_and_permute(None, order)
           if DEBUG >= 3: print("permuted global dim", order, "due to allocation exceeds global limit")
 
   def alias_buffer(self, i, pattern):
     assert len(pattern) == len(self.sts[i].shape), f"must include a pattern for each shape {pattern} {self.sts[i].shape}"
 
     bst = 1
@@ -328,158 +318,206 @@
     self.sts.append(ShapeTracker((View.create(tuple(shp), tuple(stride)),)))
     self.bufs.append(LocalBuffer(name=f"ldata{i}", size=self.sts[-1].size))
     if DEBUG >= 4: print("aliasing buffer", self.sts[i])
     self.local_alias[i] = cast(LocalBuffer, self.bufs[-1])
 
   # ******************** high level optimizers ********************
 
-  def apply_tensor_cores(self, use_tensor_cores=1, extra_opts:Optional[List[Opt]]=None) -> bool:
-    if use_tensor_cores and self.opts.has_local and self.reduceop and self.reduceop.op == ReduceOps.SUM and self.opts.device in tensor_cores:
-      for tc in tensor_cores[self.opts.device]:
-        if not (use_tensor_cores==2 or (tc.arch is None or tc.arch == os.uname().machine)): continue
+  def _apply_tc_opt(self, use_tensor_cores:int, axis:int, opt_level:int) -> bool:
+    if use_tensor_cores and self.opts.has_local and self.reduceop is not None and self.reduceop.op is ReduceOps.SUM:
+      for tc in self.opts.tensor_cores:
         has_cast = tc.dtype_in != tc.dtype_out
+        if has_cast and not(self.reduceop.src[0].op is UnaryOps.CAST and self.reduceop.src[0].arg == tc.dtype_out): continue
 
-        if has_cast and not(self.reduceop.src[0].op == UnaryOps.CAST and self.reduceop.src[0].arg[0] == tc.dtype_out): continue
         mul_op = self.reduceop.src[0].src[0] if has_cast else self.reduceop.src[0]
+        if mul_op.op is not BinaryOps.MUL: continue
 
-        if mul_op.op != BinaryOps.MUL: continue
-        if not (mul_op.src[0].op == BufferOps.LOAD and mul_op.src[0].arg.dtype == tc.dtype_in): continue
-        if not (mul_op.src[1].op == BufferOps.LOAD and mul_op.src[1].arg.dtype == tc.dtype_in): continue
-        buf0, buf1 = self.bufs.index(cast(MemBuffer, mul_op.src[0].arg)), self.bufs.index(cast(MemBuffer, mul_op.src[1].arg))
-        buf0_strides, buf1_strides = self.sts[buf0].real_strides(), self.sts[buf1].real_strides()
-        axis_buf0 = [(i,self.full_shape[i],buf1_strides[i]) for i,s in enumerate(buf0_strides[:self.first_reduce]) if s == 0 and self.full_shape[i]%tc.dims[0] == 0]  # noqa: E501
-        axis_buf1 = [(i,self.full_shape[i],buf0_strides[i]) for i,s in enumerate(buf1_strides[:self.first_reduce]) if s == 0 and self.full_shape[i]%tc.dims[1] == 0]  # noqa: E501
-
-        if not(axis_buf0 and axis_buf1 and self.full_shape[self.first_reduce]%tc.dims[2] == 0 and self.full_shape[self.first_reduce] >= tc.dims[2] and (self.shape_len-self.first_reduce) == 1): continue  # noqa: E501
-
-        if DEBUG >= 3: print("TENSOR CORES", axis_buf0, axis_buf1, tc)
+        def buf_index(src: LazyOp) -> Optional[int]:
+          # TODO: apply tc even if the sources are not from LOAD
+          if src.op is BufferOps.LOAD and src.arg.dtype == tc.dtype_in: return self.bufs.index(cast(MemBuffer, src.arg))
+          try:
+            if opt_level >= 1 and src.op is UnaryOps.CAST and src.arg == tc.dtype_in: return self.bufs.index(cast(MemBuffer, src.src[0].arg))
+          except ValueError: return None
+          return None
+        if (buf0:=buf_index(mul_op.src[0])) is None or (buf1:=buf_index(mul_op.src[1])) is None: continue
 
-        s0, s1 = axis_buf0[-1][0], axis_buf1[-1][0] # TODO: select axis in smart way
-        s0_exists, s1_exists = True, True
-        assert s0 != s1 and self.full_shape[s0]%tc.dims[0] == 0 and self.full_shape[s1]%tc.dims[1] == 0
-        def fix(needed, ax):
-          nonlocal s0, s1, s0_exists, s1_exists
-          if not needed: return
-          if s0_exists and ax == s0:
-            if s1_exists and s0 < s1: s1 -= 1
-            s0_exists = False
-          elif s1_exists and ax == s1:
-            if s0_exists and s1 < s0: s0 -= 1
-            s1_exists = False
+        buf0_strides, buf1_strides = self.sts[buf0].real_strides(), self.sts[buf1].real_strides()
+        axis_buf0 = [(i,self.full_shape[i],buf1_strides[i]) for i,s in enumerate(buf0_strides[:self.first_reduce]) if s == 0]
+        axis_buf1 = [(i,self.full_shape[i],buf0_strides[i]) for i,s in enumerate(buf1_strides[:self.first_reduce]) if s == 0]
+        if not(axis_buf0 and axis_buf1 and ((self.shape_len-self.first_reduce) == 1 or (opt_level >= 1))): continue
+
+        axis_choices = list(itertools.product(axis_buf0, axis_buf1, range(self.first_reduce, self.shape_len)))
+        if not(axis < len(axis_choices)): continue
+
+        s0, s1, s2 = axis_choices[-(axis+1)][0][0], axis_choices[-(axis+1)][1][0], axis_choices[-(axis+1)][2]  # s0 is n, s1 is m, s2 is k
+        axis_pads = [(x, tc.dims[i]) for i, x in enumerate([s0, s1, s2]) if self.full_shape[x]%tc.dims[i] != 0]
+        if axis_pads and (opt_level < 2): continue
 
         # tensor core -- unroll the reduce dim, upcast input, then create the correct thread pattern
-        self.apply_opt(Opt(OptOps.UNROLL, 0, tc.dims[2]))
-        self.apply_opt(Opt(OptOps.UPCAST, s0 if tc.upcast_dim == 0 else s1, (tc.dims[0]*tc.dims[2])//prod([a[1] for a in tc.threads])))
+        self.tensor_core_opts = (tc_opts:=TensorCoreOptions(bufs=(buf0, buf1), axes=[s0, s1], axes_exist=[True, True]))
+
+        # attempt to pad the tensor axes that require it
+        try:
+          for axis, dim in axis_pads: self.apply_opt(Opt(OptOps.PADTO, axis, dim), append_opt=False) # PADTO might fail
+        except KernelOptError: continue
+        self.apply_opt(Opt(OptOps.UNROLL, s2-self.first_reduce, tc.dims[2]), append_opt=False)
+        for i, sz in enumerate([prod(x) for x in [[x[1] for x in tc.threads if x[0]==dim] for dim in range(2)]]): # upcast non-local'd N, M
+          if tc.dims[i] > sz: self.apply_opt(Opt(OptOps.UPCAST, tc_opts.axes[i], tc.dims[i]//sz), append_opt=False)
         for (tc_dim, tc_amt) in tc.threads:
-          fix(self.apply_opt(Opt(OptOps.LASTLOCAL, s0 if tc_dim == 0 else s1, tc_amt)), s0 if tc_dim == 0 else s1)
+          self.apply_opt(Opt(OptOps.LOCAL, tc_opts.axes[tc_dim], tc_amt), append_opt=False)
 
-        # assert tensor core and prevent extra_opts from altering the key shape structure
+        # assert tensor core
+        if DEBUG >= 3: print("TENSOR CORES", axis_buf0, axis_buf1, tc)
         if use_tensor_cores == 1: self.tensor_core = tc # TC=2 will do the shape ops without the WMMA
+        return True
+    return False
+
+  def apply_tensor_cores(self, use_tensor_cores=1, extra_opts:Optional[List[Opt]]=None, axis:int=0, tc_opt:int=getenv("TC_OPT")) -> bool:
+    """ Attempts to apply a tensor core optimization to the kernel.  If one exists and applies properly, return true, otherwise return false.
+    Tensor cores are optimized instructions that matrix multiply-accumulate across a wave of threads: D(M, N) = A(M, K) * B(K, N) + C(M, N).
+
+    Keyword arguments:
+    use_tensor_cores -- controls how tensor cores are applied (default 1)
+      0: will disable any tensor core matching
+      1: enable tensor cores
+      2: apply tensor core shape but don't use UOp.WMMA
+    extra_opts -- additional Opt's to apply after the tensor core instead of the hand-coded additional Opt's (default None)
+    tc_opt -- controls which kinds of kernels may be eligible for tensor cores application (default 2 during BEAM, 0 otherwise)
+      0: applies to only kernels with a single reduce axis and direct BufferOps.LOAD into BinaryOps.MUL
+      1: allows kernels with multiple reduce axes and also multiplication of UnaryOps.CAST'd buffers
+      2: allows kernels with M, N, K axes that are not multiples of the tensor core dimensions by applying padding those axes as needed
+    """
+    if not self.opts.tensor_cores and use_tensor_cores != 2: return False
+    try: # check TC first and apply hand-coded opts if successful
+      self.apply_opt(Opt(OptOps.TC, axis, tc_opt))
 
+      if (tc_opts:=self.tensor_core_opts) is not None:
         if extra_opts is not None:
           for opt in extra_opts: self.apply_opt(opt)
         else:
           # hand-coded TC opts
-          if s1_exists:
-            s1_div = [upc for upc in [5,4,3,2,1] if self.full_shape[s1]%upc == 0][0]
-            if s1_div != 1: fix(self.apply_opt(Opt(OptOps.UPCAST, s1, s1_div)), s1)
-          if s0_exists:
-            s0_div = [upc for upc in [5,4,3,2,1] if self.full_shape[s0]%upc == 0][0]
-            if s0_div != 1: fix(self.apply_opt(Opt(OptOps.UPCAST, s0, s0_div)), s0)
-          if self.tensor_core and s0_exists:
+          def late_upcast_tc(tc_dim: int):
+            if tc_opts.axes_exist[tc_dim]:
+              ax_div = [upc for upc in [5,4,3,2,1] if self.full_shape[tc_opts.axes[tc_dim]]%upc == 0][0]
+              if ax_div != 1: self.apply_opt(Opt(OptOps.UPCAST, tc_opts.axes[tc_dim], ax_div))
+          late_upcast_tc(1) # attempt to upcast M
+          late_upcast_tc(0) # attempt to upcast N
+
+          if self.tensor_core and tc_opts.axes_exist[0]: # attempt to local N
             for upc in [4,2]:
-              if self.full_shape[s0] % upc == 0:
-                self.apply_opt(Opt(OptOps.LASTLOCAL, s0, upc))
+              if self.full_shape[tc_opts.axes[0]] % upc == 0:
+                self.apply_opt(Opt(OptOps.LOCAL, tc_opts.axes[0], upc))
                 break
 
-        # alias buffer
-        alias_pattern = [0]*(self.global_dims+(self.local_dims-len(tc.threads))) + [2]*(len(tc.threads)) + [0]*(self.shape_len-self.upcasted-self.first_reduce) + [1,1] + [3]*(self.upcasted-2)  # noqa: E501
-        self.alias_buffer(buf0, alias_pattern)
-        self.alias_buffer(buf1, alias_pattern)
-        return True
-    return False
+      return True
+    except KernelOptError:
+      return False
+
+  def apply_opt(self, opt:Opt, append_opt:bool=True):
+    check(not self.dont_use_locals or opt.op not in {OptOps.LOCAL, OptOps.GROUP, OptOps.GROUPTOP, OptOps.UPCASTMID}, "not using locals")
+
+    if opt.op is OptOps.TC:
+      check(len(self.applied_opts) == 0, "tensor core opts must be first") # TODO: things like PADTO might be fine
+      check(opt.axis is not None and opt.amt is not None, "tensor core opts must have an axis and amt")
+      check((use_tensor_cores:=getenv("TC", 1)) == 2 or len(self.opts.tensor_cores) > 0, "must have tensor cores or TC=2")
+      check(self._apply_tc_opt(use_tensor_cores, cast(int, opt.axis), cast(int, opt.amt)), "no tensor core available")
+      self.applied_opts.append(opt)
+      return
+
+    axis = opt.real_axis(self)
+    check(axis < len(self.full_shape), "invalid axis")
 
-  def apply_opt(self, opt:Opt):
-    assert not self.dont_use_locals or opt.op not in {OptOps.LOCAL, OptOps.LASTLOCAL, OptOps.GROUP, OptOps.GROUPTOP, OptOps.UPCASTMID}, "not using locals"  # noqa: E501
-    self.applied_opts.append(opt)
-    if opt.axis is not None:
-      axis = opt.axis + (self.first_reduce if opt.op == OptOps.UNROLL else (self.first_reduce+len(self.group_for_reduce) if opt.op in [OptOps.GROUP, OptOps.GROUPTOP] else 0))  # noqa: E501
-    else:
-      axis = -1
     if opt.amt is not None:
       amt = opt.amt if opt.amt != 0 else self.full_shape[axis]
-      assert isinstance(amt, int) and amt != 1, "shift/padto of amt 1 or Node is meaningless"
-      if opt.op != OptOps.PADTO: assert self.full_shape[axis] % amt == 0, "no longer valid shift"
-    else:
-      amt = -1
-    if opt.op in [OptOps.LOCAL, OptOps.LASTLOCAL]:    # cyan
-      assert self.opts.has_local, "target does not support local"
-      assert axis < self.first_reduce, "can't local a reduce"
-      if opt.op == OptOps.LOCAL:
-        assert not self.tensor_core, "can't local with tensor cores"
-        self.shift_to(axis, amt, insert_before=self.first_reduce)
-      else:
-        self.shift_to(axis, amt, insert_before=self.first_reduce-self.local_dims)
+      check(isinstance(amt, int) and amt != 1, "shift/padto of amt 1 or Node is meaningless")
+      if opt.op is not OptOps.PADTO: check(self.full_shape[axis] % amt == 0, "no longer valid shift")
+    else: amt = -1
+
+    if self.reduceop and (opt.op in {OptOps.GROUP, OptOps.GROUPTOP} or (self.group_for_reduces and opt.op not in {OptOps.NOLOCALS, OptOps.PADTO})):
+      acc_sz, upcast_idx = dt.base.itemsize if isinstance((dt:=self.reduceop.dtype), ImageDType) else dt.itemsize, self.shape_len-self.upcasted
+      upcast_sz = prod([a for a,b in zip(self.full_shape[upcast_idx:], self.sts[0].shape[upcast_idx:]) if a == b])
+      local_sz = prod(self.full_shape[self.first_reduce-self.local_dims:self.first_reduce+self.group_for_reduces])
+      smem_sz = amt*acc_sz*upcast_sz*local_sz
+      check(smem_sz <= self.opts.shared_max, f"exceeds maximum shared memory size: needs {smem_sz}, max {self.opts.shared_max}")
+
+    if opt.op is OptOps.LOCAL:    # cyan
+      check(self.opts.has_local, "target does not support local")
+      check(axis < self.global_dims, "local is for globals")
+      self.shift_to(axis, amt, insert_before=self.first_reduce)
       self.local_dims += 1
-    elif opt.op in [OptOps.GROUP, OptOps.GROUPTOP]:   # green
-      assert self.opts.has_local and self.opts.has_shared, "target does not support local or shared mem"
-      assert axis >= self.first_reduce + len(self.group_for_reduce) and axis < self.shape_len-self.upcasted, "must be reduce axis to group"
-      assert not self.tensor_core, "can't group with tensor cores"
-      self.shift_to(axis, amt, top=(opt.op==OptOps.GROUPTOP), insert_before=self.first_reduce + len(self.group_for_reduce))
-      self.group_for_reduce.append(amt)
-    elif opt.op == OptOps.UNROLL:                     # purple
-      assert axis < self.shape_len-self.upcasted, "can't upcasted already upcasted"
-      assert amt <= 32, "don't unroll more than 32"
+    elif opt.op in {OptOps.GROUP, OptOps.GROUPTOP}:   # green
+      check(self.opts.has_local and self.opts.has_shared, "target does not support local or shared mem")
+      check(axis >= self.first_reduce + self.group_for_reduces and axis < self.shape_len-self.upcasted, "must be reduce axis to group")
+      check(not self.tensor_core, "can't group with tensor cores")
+      self.shift_to(axis, amt, top=(opt.op is OptOps.GROUPTOP), insert_before=self.first_reduce + self.group_for_reduces)
+      self.group_for_reduces += 1
+    elif opt.op is OptOps.UNROLL:                     # purple
+      check(axis < self.shape_len-self.upcasted, "can't upcasted already upcasted")
+      check(amt <= 32, "don't unroll more than 32")
+      # TODO: fix upcast_count to put purples before yellows. broken because of METAL tensor cores
+      #upcast_count = sum(x == y for x,y in zip(self.full_shape[-self.upcasted:], self.output_shape[-self.upcasted:])) if self.upcasted else 0
+      #self.shift_to(axis, amt, insert_before=None if upcast_count == 0 else self.shape_len-upcast_count)
+      if self.full_shape[axis] == amt and axis == self.first_reduce: self.local_dims += 1 # first_reduce will ++, so offset loss in simplify_ones
+      if self.full_shape[axis] == amt and axis < self.first_reduce+self.group_for_reduces: self.group_for_reduces -= 1 # fully unrolling a GROUP
       self.shift_to(axis, amt, insert_before=None)
       self.upcast()
-    elif opt.op == OptOps.UPCAST:                     # yellow
-      assert axis < self.first_reduce, "upcast is for non-reduce"
-      assert amt <= 8, "don't upcast more than 8"
+    elif opt.op is OptOps.UPCAST:                     # yellow
+      check(axis < self.first_reduce, "upcast is for non-reduce")
+      check(not(self.tensor_core and self.global_dims <= axis < self.global_dims+len(self.tensor_core.threads)), "can't upcast TC locals")
+      check(amt <= 8, "don't upcast more than 8")
       self.shift_to(axis, amt, insert_before=None)
       self.upcast()
-    elif opt.op == OptOps.UPCASTMID:                  # white
-      assert self.bufs[0].dtype.name.startswith('image') and not self.float4_axis(0) and self.group_for_reduce and self.first_reduce <= 2 and prod(self.sts[0].shape) > 1, "invalid upcast mid reduce"  # noqa: E501
+    elif opt.op is OptOps.UPCASTMID:                  # white
+      check(self.bufs[0].dtype.name.startswith('image') and not self.float4_axis(0) and self.group_for_reduces != 0 and self.first_reduce <= 2 and prod(self.sts[0].shape) > 1, "invalid upcast mid reduce")  # noqa: E501
       axes = self.sts[0].unit_stride_axes()
-      assert len(axes) == 1, f"wrong number of stride 1 axis : {axes}"
-      assert axes[0] == axis, "wrong axis"
-      assert amt == 4, "don't upcast mid anything but 4"
-      self.shift_to(axis, amt, insert_before=self.first_reduce + len(self.group_for_reduce))
-      self.group_for_reduce.append(amt)
-    elif opt.op == OptOps.NOLOCALS:
-      assert self.opts.has_local and not self.dont_use_locals, "NOLOCALS is meaningless if target does not support local or already not using locals"
-      assert self.local_dims == 0 and len(self.group_for_reduce) == 0, "can't have no locals with locals"
+      check(len(axes) == 1, f"wrong number of stride 1 axis : {axes}")
+      check(axes[0] == axis, "wrong axis")
+      check(amt == 4, "don't upcast mid anything but 4")
+      self.shift_to(axis, amt, insert_before=self.first_reduce + self.group_for_reduces)
+      self.group_for_reduces += 1
+    elif opt.op is OptOps.NOLOCALS:
+      check(self.opts.has_local and not self.dont_use_locals, "NOLOCALS is meaningless if target does not support local or already not using locals")
+      check(self.local_dims == 0 and self.group_for_reduces == 0, "can't have no locals with locals")
       self.dont_use_locals = True
-    elif opt.op == OptOps.PADTO:
-      assert not self.ast.vars(), "does not work with symbolic shape"
-      assert axis < self.first_reduce, "cannot pad a reduce axis"
+    elif opt.op is OptOps.PADTO:
+      check(not self.vars, "does not work with symbolic shape")
+      check(axis < self.shape_len - self.upcasted, "cannot pad upcasted")
+      # ok to pad SUM if all parent ops have f(0) = 0
+      if self.first_reduce <= axis:
+        check((r:=cast(LazyOp, self.reduceop)).op is ReduceOps.SUM and \
+            all(op.op not in UNSAFE_PAD_OPS for ops in r.src for op in ops.lazyops), "cannot pad")
       padded = False
       for i,st in enumerate(self.sts):
-        assert self.sts[i].shape[axis] > amt//2, "pad adds more than double the work"
-        if (ru := round_up(self.sts[i].shape[axis], amt) - self.sts[i].shape[axis]):
+        if self.sts[i].shape[axis] == 1: continue  # reduced
+        check(self.sts[i].shape[axis] > amt//4, f"pad adds more than quadruple the work {self.sts[i].shape[axis]=} > {amt//4=}")
+        if (ru := round_up(cast(int, self.sts[i].shape[axis]), cast(int, amt)) - self.sts[i].shape[axis]):
           # pad right seems to be faster
           self.sts[i] = st.pad(((0,0),) * axis + ((0,ru),) + ((0,0),) * (len(st.shape)-axis-1))
           padded = True
-      assert padded, "nothing was padded"
-    return self.simplify_ones()
+      check(padded, "nothing was padded")
+
+    if append_opt: self.applied_opts.append(opt)
+    if self.simplify_ones() and self.tensor_core_opts:
+      self.tensor_core_opts.fix_axes(axis) # fix up axes in TC opts if required after simplify_ones()
 
   def required_optimizations(self):
     if self.bufs[0].dtype.__class__ is ImageDType:
       unit_stride_axes_mul_4 = [i for i in self.sts[0].unit_stride_axes(ignore_valid=True) if self.sts[0].shape[i]%4 == 0]
       assert len(unit_stride_axes_mul_4) >= 1, f"needs a unit stride axis in {self.bufs[0]}"
       if len(unit_stride_axes_mul_4) and all(x < (self.shape_len-self.upcasted) for x in unit_stride_axes_mul_4) and unit_stride_axes_mul_4[0] not in self.upcast_in_mid_reduce_axes:  # noqa: E501
         self.apply_opt(Opt(OptOps.UPCAST, unit_stride_axes_mul_4[0], 4))
 
   def hand_coded_optimizations(self):
     self.required_optimizations()
 
     # should use matvec - TODO: adjust/tune based on the wide vs tall/large vs small mat
     MV_BLOCKSIZE, MV_THREADS_PER_ROW, MV_ROWS_PER_THREAD = getenv("MV_BLOCKSIZE", 4), getenv("MV_THREADS_PER_ROW", 8), getenv("MV_ROWS_PER_THREAD", 4)
     if self.opts.has_local and getenv("MV",1) != 0 and (MV_BLOCKSIZE > 1 or MV_THREADS_PER_ROW > 1 or MV_ROWS_PER_THREAD > 1) and  \
-        self.reduceop and self.reduceop.op == ReduceOps.SUM and len(self.full_shape) >= 2 and self.opts.has_shared and \
-        (mulop:=self.reduceop.src[0]).op == BinaryOps.MUL and mulop.src[0].op == BufferOps.LOAD and mulop.src[1].op == BufferOps.LOAD:
+        self.reduceop is not None and self.reduceop.op is ReduceOps.SUM and len(self.full_shape) >= 2 and self.opts.has_shared and \
+        (mulop:=self.reduceop.src[0]).op is BinaryOps.MUL and mulop.src[0].op is BufferOps.LOAD and mulop.src[1].op is BufferOps.LOAD:
       st0, st1 = self.sts[self.bufs.index(mulop.src[0].arg)], self.sts[self.bufs.index(mulop.src[1].arg)]
       strides0, strides1 = st0.real_strides(), st1.real_strides()
       def has_expanded_axis(shape, strides): return any(s > 1 and st == 0 for s,st in zip(shape,strides))
       if strides0[self.first_reduce] == 1 and not (has_expanded_axis(st0.shape, strides0) and has_expanded_axis(st1.shape, strides1)):
         for global_idx in range(self.global_dims):
           if self.full_shape[self.first_reduce]%MV_THREADS_PER_ROW == 0 and self.full_shape[global_idx]%(MV_BLOCKSIZE*MV_ROWS_PER_THREAD) == 0:
             if DEBUG >= 3:
@@ -491,19 +529,21 @@
 
     if self.opts.has_local and self.opts.has_shared and all_int(self.sts[0].shape[:self.first_reduce]):
       # are we grouping? (requires local shape support)
       if not self.float4_axis(0) and self.first_reduce <= 2 and self.first_reduce + 1 <= self.shape_len and prod(self.sts[0].shape[:self.first_reduce]) <= 2048:  # noqa: E501
         # TODO: use 1024 if it's allowed in a smarter way
         for sz in (([256, 16]) if prod(self.sts[0].shape[:self.first_reduce]) <= 32 else [16]):
           if all(st.shape[self.first_reduce] % sz == 0 or st.shape[self.first_reduce] == 1 for st in self.sts):
-            self.apply_opt(Opt(OptOps.GROUPTOP, 0, sz))
-            break
+            try: # may fail due to excessive smem usage
+              self.apply_opt(Opt(OptOps.GROUPTOP, 0, sz))
+              break
+            except KernelOptError: pass
 
       # are we upcasting in mid reduce? (only for images)
-      if self.bufs[0].dtype.name.startswith('image') and not self.float4_axis(0) and self.group_for_reduce and self.first_reduce <= 2 and prod(self.sts[0].shape) > 1:  # noqa: E501
+      if self.bufs[0].dtype.name.startswith('image') and not self.float4_axis(0) and self.group_for_reduces and self.first_reduce <= 2 and prod(self.sts[0].shape) > 1:  # noqa: E501
         axes = self.sts[0].unit_stride_axes()
         assert len(axes) == 1, f"wrong number of stride 1 axis : {axes}"
         if self.sts[0].shape[axes[0]]%4 == 0:
           self.apply_opt(Opt(OptOps.UPCASTMID, axes[0], 4))
 
     # upcast float4 images
     for buf_index,buf in enumerate(self.bufs):
@@ -513,15 +553,15 @@
         if len(unit_stride_axes_mul_4) and all(x < (self.shape_len-self.upcasted) for x in unit_stride_axes_mul_4) and unit_stride_axes_mul_4[0] not in self.upcast_in_mid_reduce_axes:  # noqa: E501
           if unit_stride_axes_mul_4[0] < self.first_reduce:
             self.apply_opt(Opt(OptOps.UPCAST, unit_stride_axes_mul_4[0], 4))
           else:
             self.apply_opt(Opt(OptOps.UNROLL, unit_stride_axes_mul_4[0]-self.first_reduce, 4))
 
     # no more opt if we are grouping
-    if self.group_for_reduce: return
+    if self.group_for_reduces: return
 
     # **** below this line need to be optional and benchmarked ****
 
     # TODO: doing extra upcasts with images doesn't work for some reason (maybe has to do with to_image_idx)
     # to trigger the above bug, remove prod(self.full_shape[self.shape_len - self.upcasted:]) from the below
     # expression and run test/test_ops.py with IMAGE=2
     # if there are small dims with lots of valid masks, upcast them (they might be from Tensor.stack)
@@ -570,15 +610,15 @@
     for splits in [4]:
       if self.upcasted == 0 and self.full_unupcasted_shape and self.full_unupcasted_shape[-1] % splits == 0:
         self.apply_opt(Opt(OptOps.UPCAST, len(self.full_unupcasted_shape)-1, splits))
 
     # **** local groups ****
 
     if self.opts.has_local:
-      if getenv("NOLOCALS") and self.local_dims == 0 and not self.group_for_reduce:
+      if getenv("NOLOCALS") and self.local_dims == 0 and not self.group_for_reduces:
         self.apply_opt(Opt(OptOps.NOLOCALS))
       else:
         # prioritize making expand axes local
         local_axis_ranking = [(any(self.sts[buf_index].views[-1].strides[axis] == 0 for buf_index in range(len(self.sts))), axis) for axis in range(len(self.full_shape[:self.first_reduce]))]  # noqa: E501
         to_local: List[Tuple[int, int]] = []
         for _, axis in sorted(local_axis_ranking, key=lambda x: (-x[0], -x[1])):
           local_size = prod(sz for _, sz in to_local)
```

### Comparing `tinygrad-0.8.0/tinygrad/codegen/linearizer.py` & `tinygrad-0.9.0/tinygrad/codegen/linearizer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,566 +1,460 @@
 from __future__ import annotations
-from typing import List, Tuple, Any, Optional, cast, DefaultDict, Dict, Union, Sequence, Final, Set, Iterator
+from typing import List, Tuple, Any, Optional, cast, DefaultDict, Dict, Union, Final, Iterator, Sequence
 import itertools, math, functools
 from collections import defaultdict
-from enum import Enum, auto
-from dataclasses import dataclass
 
-from tinygrad.dtype import ImageDType, dtypes, DType, PtrDType
-from tinygrad.helpers import colored, DEBUG, prod, getenv, all_same, to_function_name, flatten
+from tinygrad.dtype import ImageDType, dtypes, DType, PtrDType, ConstType
+from tinygrad.helpers import colored, DEBUG, prod, getenv, to_function_name
 from tinygrad.ops import LazyOp, UnaryOps, BinaryOps, TernaryOps, ReduceOps, ConstBuffer, MemBuffer, BufferOps, get_lazyop_info
 from tinygrad.shape.shapetracker import ShapeTracker
-from tinygrad.shape.symbolic import Variable, NumNode, Node, SumNode, MulNode, DivNode, ModNode, LtNode, AndNode
+from tinygrad.shape.symbolic import Variable, NumNode, Node, SumNode, MulNode, DivNode, ModNode, LtNode, AndNode, create_lt_node
 from tinygrad.codegen.kernel import LocalBuffer, Kernel
-from tinygrad.features.image import to_image_idx
+from tinygrad.renderer import Program
 
-# bottom ones are asm only
-class UOps(Enum):
-  LOOP = auto(); IF = auto(); END = auto(); SPECIAL = auto() # loops can be global, local, or other # noqa: E702
-  DEFINE_GLOBAL = auto(); DEFINE_LOCAL = auto(); DEFINE_ACC = auto() # this defines buffers # noqa: E702
-  LOAD = auto(); STORE = auto(); CONST = auto(); BARRIER = auto(); PHI = auto() # noqa: E702
-  ALU = auto(); WMMA = auto(); CAST = auto(); GEP = auto() # noqa: E702
-
-@dataclass(eq=False)
-class UOp:
-  uop: UOps
-  dtype: Optional[DType]
-  vin: Tuple[UOp, ...]
-  arg: Any
-  def __repr__(self):
-    return f"{str(self.uop):20s}: {str(self.dtype) if self.dtype is not None else '':25s} {str([x.uop for x in self.vin]):32s} {self.arg}"
+from tinygrad.codegen.uops import UOps, UOp, UOpGraph
 
 def get_grouped_dims(prefix, start_dim, local_dims, maxdim:int=0):
-  local_idxs = loop_local_idxs = [Variable(f"{prefix}{start_dim+i}", 0, s-1) for i,s in enumerate(local_dims[0:maxdim-1] + (prod(local_dims[maxdim-1:]),) if len(local_dims) > maxdim else local_dims)]  # noqa: E501
+  local_idxs = loop_local_idxs = [Variable(f"{prefix}{start_dim+i}", 0, s-1) for i,s in enumerate((prod(local_dims[:-(maxdim-1)]),) + local_dims[-(maxdim-1):] if len(local_dims) > maxdim else local_dims)]  # noqa: E501
   if maxdim != 0 and len(local_dims) > maxdim:
-    dd = local_idxs[maxdim-1]
+    dd = local_idxs[0]
     nli = []
-    for s in local_dims[maxdim-1:][::-1]:
+    for s in local_dims[:-(maxdim-1)]:
       nli.append(dd % s)
       dd //= s
-    local_idxs = local_idxs[0:maxdim-1] + nli[::-1]
+    local_idxs = nli + local_idxs[-(maxdim-1):]
   return local_idxs, [x for x in loop_local_idxs if not isinstance(x, NumNode)]
 
-def expand_idx(node:Node) -> Union[Variable, NumNode]: return next((v for v in node.vars() if v.expr is None), NumNode(0))
+def expand_idx(node:Node) -> Union[Variable, NumNode]: return next((v for v in node.vars() if v.expr.startswith("_uidx")), NumNode(0))
+def expand_idxs(nodes:Sequence[Node]) -> Tuple[Union[Variable, NumNode], ...]:
+  eidxs = [expand_idx(node) for node in nodes]
+  return tuple([v if v not in eidxs[:j] else NumNode(0) for j, v in enumerate(eidxs)])  # take only first occurrence of expand variable
 def iter_idxs(idxs:Tuple[Union[Variable, NumNode], ...]) -> Iterator[Tuple[int,...]]:
   yield from (x[::-1] for x in itertools.product(*[[x for x in range(v.min, v.max + 1)] for v in idxs[::-1]]))
 
+def to_image_idx(base_shape:Tuple[int, ...], idxy:Node, valid:Node) -> Tuple[Tuple[Node, Node], Node]:
+  idx, idy = (idxy // 4) % base_shape[1], (idxy // (4 * base_shape[1]))
+  # TODO: bring back the valid removal logic (correct!)
+  if DEBUG>=5: print("to_image_idx", base_shape, idx.min, idx.max, idy.min, idy.max, idx, idy, valid)
+  return (idx, idy), valid
+
 # expand a Node into List[Node] that enumerates the underlying Variables from min to max
 # expand increments earlier variables faster than later variables (as specified in the argument)
 @functools.lru_cache(maxsize=None)
 def expand_node(node:Node, idxs:Optional[Tuple[Union[Variable, NumNode], ...]]=None) -> List[Node]:
   if idxs is None: idxs = (expand_idx(node),)
   return [node.substitute({k:v for k,v in zip(idxs, (NumNode(x) for x in rep)) if isinstance(k, Variable)}) for rep in iter_idxs(idxs)]
 
 class Linearizer(Kernel):
-  def uop_alu_idx(self, a:UOp, b, ops, ctx:Linearizer, op, dtype=dtypes.int32):
-    render_b:UOp = cast(UOp, (NumNode(b) if not isinstance(b, Node) else b).render(ops, ctx))
-    return self.uop(UOps.ALU, dtype, (a, render_b), op)
+  def uop_alu_idx(self, a:UOp, b, ops, ctx:Linearizer, op): return UOp.alu(op, a, (NumNode(b) if not isinstance(b, Node) else b).render(ops, ctx))
 
   # NOTE: the consts have to be cached for deduping of downstream uops to work
-  def const(self, b:Union[int,float], dtype=dtypes.int32, insert_before=None) -> UOp:
-    return self.uop(UOps.CONST, dtype, tuple(), b, insert_before=insert_before)
-
-  def cast(self, val: UOp, dtype) -> UOp: return self.uop(UOps.CAST, dtype, (val,)) if val.dtype != dtype else val
+  def const(self, b:ConstType, dtype:DType=dtypes.int32) -> UOp:
+    return self.uops.add(UOps.DEFINE_VAR, dtype, (), b.unbind()[0]) if isinstance(b, Variable) else UOp.const(dtype, b)
 
   def get_reduce_acc(self, reduceop:LazyOp):
-    dtype = get_lazyop_info(reduceop).dtype
-    if reduceop.op == ReduceOps.SUM: return 0.0 if dtypes.is_float(dtype) else 0
-    elif reduceop.op == ReduceOps.MAX:
-      if dtypes.is_int(dtype): return 0 if dtypes.is_unsigned(dtype) else -2**(dtype.itemsize*8-1)
-      return -math.inf if dtypes.is_float(dtype) else False
+    if reduceop.op is ReduceOps.SUM: return 0.0 if dtypes.is_float(reduceop.dtype) else 0
+    if reduceop.op is ReduceOps.MAX:
+      if dtypes.is_int(reduceop.dtype): return 0 if dtypes.is_unsigned(reduceop.dtype) else -2**(reduceop.dtype.itemsize*8-1)
+      return -math.inf if dtypes.is_float(reduceop.dtype) else False
 
   # NOTE: once images are loaded, we uop them as their base float
-  def get_base_dtype(self, dt:DType): return dt.base if isinstance(dt, ImageDType) else dt
+  def get_base_dtype(self, dt:DType) -> DType: return dt.base if isinstance(dt, ImageDType) else dt
 
   render_ops: Any = { Variable: lambda self, ops, ctx: ctx.loop_uops[self.expr], NumNode: lambda self, ops, ctx: ctx.const(self.b),
                 MulNode: lambda self, ops, ctx: ctx.uop_alu_idx(self.a.render(ops, ctx), self.b, ops, ctx, BinaryOps.MUL),
                 DivNode: lambda self, ops, ctx: ctx.uop_alu_idx(self.a.render(ops, ctx), self.b, ops, ctx, BinaryOps.DIV),
                 ModNode: lambda self, ops, ctx: ctx.uop_alu_idx(self.a.render(ops, ctx), self.b, ops, ctx, BinaryOps.MOD),
-                LtNode: lambda self, ops, ctx: ctx.uop_alu_idx(self.a.render(ops, ctx), self.b, ops, ctx, BinaryOps.CMPLT, dtype=dtypes.bool),
+                LtNode: lambda self, ops, ctx: ctx.uop_alu_idx(self.a.render(ops, ctx), self.b, ops, ctx, BinaryOps.CMPLT),
     SumNode: lambda self,ops,ctx:
       functools.reduce(lambda a,b: ctx.uop_alu_idx(a, b, ops, ctx, BinaryOps.ADD), self.nodes[1:], self.nodes[0].render(ops,ctx)),
     AndNode: lambda self,ops,ctx:
-      functools.reduce(lambda a,b: ctx.uop_alu_idx(a, b, ops, ctx, BinaryOps.MUL, dtype=dtypes.bool), self.nodes[1:], self.nodes[0].render(ops,ctx)) }
+      functools.reduce(lambda a,b: ctx.uop_alu_idx(a, b, ops, ctx, BinaryOps.MUL), self.nodes[1:], self.nodes[0].render(ops,ctx)) }
 
-  def global_load(self, i:int, idxs:Sequence[Node], acc=None, barrier:Optional[UOp]=None) -> List[UOp]:
+  def global_load(self, i:int, idxs:List[Node], acc:Optional[LazyOp]=None, barrier:Optional[UOp]=None, loop_ctx:Tuple[UOp, ...]=()) -> List[UOp]:
     buf = self.bufs[i]
-    localtype = self.get_base_dtype(buf.dtype if acc is None else get_lazyop_info(self.reduceop).dtype)
-    const = buf.val if isinstance(buf, ConstBuffer) else acc
+    localtype = self.get_base_dtype(buf.dtype if acc is None else acc.dtype)
+    const = buf.val if isinstance(buf, ConstBuffer) else None
 
-    def rename_var(v: Union[Variable, NumNode], expr: str): return v if isinstance(v, NumNode) else Variable(expr, v.min, v.max)
-    expand_vars = tuple([rename_var(expand_idx(idx), f"_uidx{j}") for j, idx in enumerate(idxs)])
-    fake_idxs = [idx.substitute({eidx: ev}) if isinstance(eidx:=expand_idx(idx), Variable) else idx for idx, ev in zip(idxs, expand_vars)]
+    expand_vars = expand_idxs(idxs)
 
     dim, amt = None, 1
     # float 4 grouping
     if len(upcast_dim := self.get_float4_upcast_dim(i)) == 1 and len(float4_expand := expand_node(idxs[upcast_dim[0]])) in [4,2]:
       dim, amt = upcast_dim[0], len(float4_expand)
-      g_idx, g_valid = self.sts[i].expr_idxs(fake_idxs[:dim] + [float4_expand[0]] + fake_idxs[dim+1:])
+      g_idx, g_valid = self.sts[i].expr_idxs(idxs[:dim] + [float4_expand[0]] + idxs[dim+1:])
       # do not use float4 if idx is not aligned
       if g_idx != (g_idx//amt*amt): dim, amt = None, 1
     if dim is None:
-      g_idx, g_valid = self.sts[i].expr_idxs(fake_idxs)
+      g_idx, g_valid = self.sts[i].expr_idxs(idxs)
+    # todo: multioutput test with different output valids to add if acc is None: g_valid = NumNode(1)
 
     if amt > 1: localtype = localtype.vec(amt)
     e_idxs, e_valids = expand_node(g_idx, expand_vars), expand_node(g_valid, expand_vars)
 
     ret = []
-    invalid_value = 0 if dtypes.is_int(buf.dtype) else 0.0
+    invalid_value = 0
+    acc_count = 0
     for idx, valid, rep_idx in zip(e_idxs, e_valids, iter_idxs(expand_vars)):
       this_const, idx, valid = (invalid_value, NumNode(0), NumNode(1)) if valid.max == 0 else (const, idx, valid)
-      key = f"{acc}{localtype}{this_const if this_const is not None and acc is None else (buf.idx if isinstance(buf, MemBuffer) else cast(LocalBuffer, buf).name)}{idx.render()}{valid.render()}"  # noqa: E501
+      # todo: when multiple reduceops are supported, clearly disambiguate and test acc load keys are unique for each reduceop
+      key = f"{acc is not None}{localtype}{'CONST'+str(this_const) if this_const is not None and acc is None else (buf.idx if isinstance(buf, MemBuffer) else cast(LocalBuffer, buf).name)}{idx.render()}{valid.render()}"  # noqa: E501
       if key not in self.load_cache:
         if acc is not None:
-          self.load_cache[key] = self.uop(UOps.DEFINE_ACC, localtype, (), this_const, cachable=False)
+          self.load_cache[key] = self.uops.add(UOps.DEFINE_ACC, localtype, loop_ctx, (self.get_reduce_acc(acc), i, acc_count))
+          acc_count += 1
         elif this_const is not None:
           self.load_cache[key] = self.const(this_const, localtype)
           if valid.min == 0 and valid.max == 1:
             valid_rendered = valid.render(self.render_ops, self)
-            self.load_cache[key] = self.uop(UOps.ALU, localtype, (valid_rendered, self.load_cache[key], self.const(invalid_value, localtype)), TernaryOps.WHERE)  # noqa: E501
+            self.load_cache[key] = UOp.alu(TernaryOps.WHERE, valid_rendered, self.load_cache[key], self.const(invalid_value, localtype))
         elif isinstance(buf.dtype, ImageDType):
           buf_uop = self.buf_uops[i]
           assert buf_uop is not None, f"buffer {i} wasn't UOped"
           image_idx, valid = to_image_idx(buf.dtype.shape, idx, valid)
-          rendered_idx = self.uop(UOps.CAST, dtypes.int.vec(2), tuple(x.render(self.render_ops, self) for x in image_idx))
+          rendered_idx = self.uops.add(UOps.CAST, dtypes.int.vec(2), tuple(x.render(self.render_ops, self) for x in image_idx))
           valid_tuple = (valid.render(self.render_ops, self), self.const(invalid_value, buf.dtype.base.vec(4))) if valid.min == 0 else tuple()
-          self.load_cache[key] = self.uop(UOps.LOAD, buf.dtype.base.vec(4), (buf_uop, rendered_idx) + valid_tuple + ((barrier,) if barrier else ()))
+          self.load_cache[key] = self.uops.add(UOps.LOAD, buf.dtype.base.vec(4),
+                                               (buf_uop, rendered_idx) + valid_tuple + ((barrier,) if barrier else ()))
           if localtype == localtype.scalar():
             idx_small = idx%4
             res = idx_small.render(self.render_ops, self)
-            out = self.uop(UOps.GEP, localtype, (self.load_cache[key],), idx_small.max)
+            out = self.uops.add(UOps.GEP, localtype, (self.load_cache[key],), idx_small.max)
             for ix in range(idx_small.max, idx_small.min, -1):
-              rvv = self.uop(UOps.GEP, localtype, (self.load_cache[key],), ix-1)
-              sel = self.uop(UOps.ALU, dtypes.bool, (res, self.const(ix)), BinaryOps.CMPLT)
-              out = self.uop(UOps.ALU, localtype, (sel, rvv, out), TernaryOps.WHERE)
+              rvv = self.uops.add(UOps.GEP, localtype, (self.load_cache[key],), ix-1)
+              sel = UOp.alu(BinaryOps.CMPLT, res, self.const(ix))
+              out = UOp.alu(TernaryOps.WHERE, sel, rvv, out)
             self.load_cache[key] = out
         else:
           buf_uop = self.buf_uops[i]
           assert buf_uop is not None, f"buffer {i} wasn't UOped"
           rendered_idx = idx.render(self.render_ops, self)
           valid_tuple = (valid.render(self.render_ops, self), self.const(invalid_value, localtype)) if valid.min == 0 else tuple()
-          self.load_cache[key] = self.uop(UOps.LOAD, localtype, (buf_uop, rendered_idx) + valid_tuple + ((barrier,) if barrier else ()))
-      ret.append(self.uop(UOps.GEP, localtype.scalar(), (self.load_cache[key],), rep_idx[dim]) if dim is not None else self.load_cache[key])
+          self.load_cache[key] = self.uops.add(UOps.LOAD, localtype, (buf_uop, rendered_idx) + valid_tuple + ((barrier,) if barrier else ()))
+      ret.append(self.uops.add(UOps.GEP, localtype.scalar(), (self.load_cache[key],), rep_idx[dim]) if dim is not None else self.load_cache[key])
     return ret
 
   def global_store(self, i:int, idxs:List[Node], store:List[UOp]) -> List[UOp]:
     buf = self.bufs[i]
     buf_uop = self.buf_uops[i]
     assert buf_uop is not None, f"buffer {i} wasn't UOped"
 
-    expanded_nodes = [expand_node(idx) for idx in idxs]
-    _idxs = [x[::-1] for x in itertools.product(*expanded_nodes[::-1])]
+    expand_vars = expand_idxs(idxs)
+    _idxs = zip(*[expand_node(idx, expand_vars) for idx in idxs]) if idxs else [tuple()]  # transpose
     store_offset = dict(zip(_idxs, store))
 
     # float4 grouping
-    if len(upcast_dim := self.get_float4_upcast_dim(i)) == 1 and len(float4_expand := expanded_nodes[upcast_dim[0]]) in [2,4]:
+    if len(upcast_dim := self.get_float4_upcast_dim(i)) == 1 and len(float4_expand := expand_node(idxs[upcast_dim[0]])) in [2,4]:
       grouped_store_offset = defaultdict(list)
       for k in store_offset:
         _idx = k[:upcast_dim[0]] + (float4_expand[0],) + k[upcast_dim[0]+1:]
         grouped_store_offset[_idx].append(store_offset[k])
       store_offset_new = {}
       for k,grouped in grouped_store_offset.items():
         amt = len(grouped)
         idx, valid = self.sts[i].expr_idxs(k)
         assert idx == ((idx//amt)*amt), "float4 stores are always aligned"
-        store_offset_new[k] = self.uop(UOps.CAST, buf.dtype.vec(amt), tuple(grouped))
+        store_offset_new[k] = self.uops.add(UOps.CAST, buf.dtype.vec(amt), tuple(grouped))
       store_offset = store_offset_new
 
     stores = []
-    for idx, var in store_offset.items():
-      idx, valid = self.sts[i].expr_idxs(idx)
+    for _idx, var in store_offset.items():
+      idx, valid = self.sts[i].expr_idxs(_idx)
       if isinstance(buf.dtype, ImageDType):
-        idx, valid = to_image_idx(buf.dtype.shape, idx, valid)
-        rendered_idx = self.uop(UOps.CAST, dtypes.int.vec(2), tuple(x.render(self.render_ops, self) for x in idx))
+        image_idx, valid = to_image_idx(buf.dtype.shape, idx, valid)
+        rendered_idx = self.uops.add(UOps.CAST, dtypes.int.vec(2), \
+                      tuple(x.render(self.render_ops, self) for x in image_idx))
       else:
         rendered_idx = idx.render(self.render_ops, self)
-      if valid.min == 1: stores.append(self.uop(UOps.STORE, None, (buf_uop, rendered_idx, var)))
-      else: stores.append(self.uop(UOps.STORE, None, (buf_uop, rendered_idx, var, valid.render(self.render_ops, self))))
+      if valid.min == 1: stores.append(self.uops.add(UOps.STORE, None, (buf_uop, rendered_idx, var)))
+      else: stores.append(self.uops.add(UOps.STORE, None, (buf_uop, rendered_idx, var, valid.render(self.render_ops, self))))
     return stores
 
+  # render loop
+  def render_loop(self, xx:List[Variable], depth:int) -> Tuple[UOp, ...]:
+    new_loops = {x.expr:self.uops.add(UOps.RANGE, dtypes.int32, (
+      self.const(x.min) if isinstance(x.min, int) else cast(Node, x.min).render(self.render_ops, self),
+      self.const(x.max+1) if isinstance(x.max, int) else cast(Node, x.max+1).render(self.render_ops, self)), arg=(depth,i)) for i,x in enumerate(xx) if not isinstance(x, NumNode) and x.expr is not None}  # noqa: E501
+    self.loop_uops.update(new_loops)
+    return tuple(new_loops.values())
+
+  def render_reduceop(self, reduceop:LazyOp, accs:Dict[LazyOp, List[UOp]], loaded_buffers:Dict[Union[MemBuffer, ConstBuffer, LocalBuffer], List[UOp]],
+                      global_idxs, local_idxs, upcast_idxs):
+    # define indicies
+    full_upcast_idxs = [Variable(f"_uidx{i}", 0, s-1) for i, s in enumerate(self.full_shape[self.shape_len-self.upcasted:])]
+    reduce_idxs = [Variable(f"ridx{i}", 0, self.full_shape[i]-1) for i in range(self.first_reduce+self.group_for_reduces, self.shape_len-self.upcasted)]  # noqa: E501
+    fake_reduce_idxs = [x*0 for x in reduce_idxs]
+
+    def calc_tc_idxs(local_sizes: List[int], aliases: List[List[int]]):
+      replace_idxs, thread_idxs, thread_idx = [], [], Variable("_uidx_tc", 0, prod(local_sizes)-1)
+      for s in local_sizes:
+        thread_idxs.append(thread_idx % s)
+        thread_idx //= s
+      for alias in aliases:
+        full_var, full_var_sz = NumNode(0), 1
+        if alias[0] != 0:
+          for i in alias:
+            next_var = local_idxs[i-1] if i > 0 else thread_idxs[-i-1]
+            full_var += next_var * full_var_sz
+            full_var_sz *= next_var.max+1
+        replace_idxs.append(full_var)
+      return replace_idxs
+
+    # compute local aliases - modify idxs if necessary for TC
+    alias_buf_idxs = []
+    for i in self.local_alias:
+      localbuf_idx = self.bufs.index(self.local_alias[i])
+      buf_idxs = [idx*0 if s == 0 else idx for idx,s in zip(global_idxs+local_idxs+reduce_idxs+full_upcast_idxs,self.sts[i].real_strides())]
+      if (tc:=self.tensor_core):
+        min_alias_idx = min(self.local_alias.keys())
+        replace_input_idxs = calc_tc_idxs(tc.thread_local_sizes[i-min_alias_idx], tc.thread_local_aliases[i-min_alias_idx])
+        for n in range(len(tc.threads)):
+          buf_idxs[self.global_dims+n] = replace_input_idxs[n] # replace locals
+        for n in range(tc.num_upcasts()):
+          buf_idxs[self.shape_len-self.upcasted+n] = replace_input_idxs[len(tc.threads)+n] # replace upcasts
+      if DEBUG >= 3: print(f"{localbuf_idx} alias {i}: sts={self.sts[i]} idxs={buf_idxs}")
+      alias_buf_idxs.append((i, localbuf_idx, buf_idxs,))
+
+    # reduce loop
+    loop_ctx = self.render_loop(reduce_idxs, 2)
+
+    # define accumulator - modify idxs if necessary for TC
+    out_buf = -1 if self.group_for_reduces else 0
+    if (tc:=self.tensor_core):
+      replace_acc_idxs = calc_tc_idxs(tc.thread_local_sizes[2], tc.thread_local_aliases[2])
+      for n in range(len(tc.threads)):
+        local_idxs[n] = replace_acc_idxs[n] # replace locals
+      for n in range(len(replace_acc_idxs)-len(tc.threads)):
+        upcast_idxs[n] = replace_acc_idxs[len(tc.threads)+n] # replace upcasts
+      if DEBUG >= 3: print(f"store alias: sts={self.sts[0]} idxs={global_idxs+local_idxs+fake_reduce_idxs+upcast_idxs}")
+    accs[reduceop] = self.global_load(out_buf, global_idxs+local_idxs+fake_reduce_idxs+upcast_idxs, acc=reduceop, loop_ctx=loop_ctx)
+
+    # store local aliases
+    locals_to_store = [(localbuf_idx, buf_idxs, self.global_load(i, buf_idxs)) for i, localbuf_idx, buf_idxs in alias_buf_idxs]
+
+    if (tc:=self.tensor_core):
+      # run tensor cores AST
+      wmma_sz = [prod(l) for l in tc.thread_local_sizes]
+      def upcast_strides(buf:int):
+        strides, next = [], 1
+        for (sz, stride, reduce) in self.upcasted_axis(buf)[tc.num_upcasts():]:
+          strides.append((0 if stride == 0 else next, sz))
+          next *= 1 if stride == 0 else sz
+        return strides
+      upcasts, dev = [upcast_strides(x) for x in [locals_to_store[0][0], locals_to_store[1][0], 0]], self.opts.device
+      # cast initial accs
+      wmmas = [self.uops.add(UOps.CAST, (dt3:=tc.dtype_out.vec(wmma_sz[2])), tuple(accs[reduceop][x:x+wmma_sz[2]]))
+               for x in range(0, len(accs[reduceop]), wmma_sz[2])]
+      for iter in [x[::-1] for x in itertools.product(*[x for x in [range(sz) for _,sz in upcasts[0]][::-1]])]:
+        offs = [x*y for (x,y) in zip([sum([prod(x) for x in zip(iter, [stride for stride,_ in y])]) for y in upcasts], wmma_sz)]
+        ops = (self.uops.add(UOps.CAST, tc.dtype_in.vec(wmma_sz[0]), tuple(locals_to_store[0][2][offs[0]:offs[0]+wmma_sz[0]])),
+                self.uops.add(UOps.CAST, tc.dtype_in.vec(wmma_sz[1]), tuple(locals_to_store[1][2][offs[1]:offs[1]+wmma_sz[1]])),
+                wmmas[(wmma_idx:=offs[2]//wmma_sz[2])])
+        # TODO: don't need to DEFINE_ACC, pass to WMMA in op3, or PHI accs that are not valid
+        wmmas[wmma_idx] = self.uops.add(UOps.WMMA, dt3, ops, (str(tc), tc.dims, tc.dtype_in, tc.dtype_out, tuple(wmma_sz), dev))
+      # phi the last wmmas back to accs
+      accs[reduceop] = [self.uops.add(UOps.PHI, tc.dtype_out, (acc, self.uops.add(UOps.GEP, tc.dtype_out, (wmmas[z//wmma_sz[2]],), z%wmma_sz[2])))
+                        for z, acc in enumerate(accs[reduceop])]
+    else:
+      assert not locals_to_store, "storing locals isn't supported here"
+
+      # load earlybufs
+      loaded_buffers.update({b:self.global_load(self.bufs.index(self.local_alias[i]) if i in self.local_alias else i,
+        global_idxs+local_idxs+reduce_idxs+full_upcast_idxs) for i,b in enumerate(self.bufs) if b in self.earlybufs})
+
+      # run early AST (with reduce)
+      self.ast_parse(reduceop, accs, self.acc_offsets(self.full_buf_index), loaded_buffers, reduce_acc=accs[reduceop])
+
+    # end the reduce loop
+    self.load_cache.clear()
+
+    # end the local loop, do the local reduce
+    if self.group_for_reduces:
+      fake_global_idxs = [x*0 for x in global_idxs]
+      stores = self.global_store(-1, fake_global_idxs+local_idxs+fake_reduce_idxs+upcast_idxs, accs[reduceop])  # store accumulators
+      barrier = self.uops.add(UOps.BARRIER, None, tuple(stores))
+      if self.opts.has_local:
+        fake_idxs = [NumNode(0)]*len(self.sts[-1].shape)
+        fake_idxs[self.global_dims+self.local_dims:self.global_dims+len(local_idxs)] = local_idxs[self.local_dims:]
+        if_cond: UOp = create_lt_node(self.sts[-1].expr_idxs(fake_idxs)[0], 1).render(self.render_ops, self)
+        barrier = self.uops.add(UOps.IF, None, (if_cond, barrier))
+
+      # create new late reduce local loops and replace local_idxs that have been used
+      end_local_idxs = [Variable(f"tidx{i}", 0, self.full_shape[i]-1 if i >= self.first_reduce and i not in self.upcast_in_mid_reduce_axes else 0) for i in range(0, self.first_reduce+self.group_for_reduces)]  # noqa: E501
+      local_idxs = local_idxs[:self.local_dims] + end_local_idxs[self.global_dims + self.local_dims:]
+
+      # if any group_for_reduce items aren't reduces, upcast them here
+      for j in self.upcast_in_mid_reduce_axes:
+        self.reshape_and_permute(None, [i for i in range(self.shape_len) if i != j] + [j])
+        self.upcast()
+        self.group_for_reduces -= 1
+        local_idxs = local_idxs[:-1]
+        end_local_idxs = end_local_idxs[:-1]
+        # regenerate upcast_idxs
+        upcast_idxs = [Variable(f"_uidx{i}", 0, s-1) for i, s in enumerate(self.output_shape[self.shape_len-self.upcasted:])]
+
+      # NOTE: this structure is the same as the reduce op above
+
+      # late reduce loop
+      loop_ctx = self.render_loop(end_local_idxs, 3)
+
+      # define late accumulator
+      accs[reduceop] = self.global_load(0, fake_global_idxs+local_idxs+fake_reduce_idxs+upcast_idxs, acc=reduceop, loop_ctx=loop_ctx)
+
+      # load localbufs
+      loaded_buffers[self.bufs[-1]] = self.global_load(-1, fake_global_idxs+local_idxs+fake_reduce_idxs+upcast_idxs, barrier=barrier)
+
+      # there's no AST here (and there's no shape for the reduce LazyOp)
+      self.ast_parse(LazyOp(reduceop.op, (LazyOp(BufferOps.LOAD, (), self.bufs[-1]),)),\
+                     accs, self.acc_offsets(-1), loaded_buffers, reduce_acc=accs[reduceop])
+
+      # end the late reduce loop
+      self.load_cache.clear()
+
+      # all local indices which were used for group_for_reduce are not valid any more and should be replaced with fake NumNode(0), since they have
+      # been rewritten with fake end_local_idxs.
+    return (accs, loaded_buffers, fake_reduce_idxs, local_idxs[:self.local_dims] + [NumNode(0) for i in range(self.group_for_reduces)], upcast_idxs)
+
   kernel_cnt: Final[DefaultDict[str, int]] = defaultdict(int)
   def linearize(self):
     # no new opts and we already ran? skip relinearizing
     if self.applied_opts == self.applied_opts_cache: return self
 
+    # late alias the tensor core buffers
+    if (tc:=self.tensor_core) and (tc_opts:=self.tensor_core_opts):
+      alias_pattern = [0]*(self.global_dims) + [2]*(len(tc.threads)) + [0]*(self.local_dims-len(tc.threads)) + [0]*(self.shape_len-self.upcasted-self.first_reduce) + [1,1] + [3]*(self.upcasted-2)  # noqa: E501
+      for tc_buf in tc_opts.bufs:
+        self.alias_buffer(tc_buf, alias_pattern)
+
     # save backups
-    sts_backup, gfr_backup, upc_backup = self.sts[:], self.group_for_reduce[:], self.upcasted
+    sts_backup, gfr_backup, upc_backup = self.sts[:], self.group_for_reduces, self.upcasted
 
     # global uop cache
     self.saved_exprs: Dict[Tuple, UOp] = dict()
 
     # limit dims if we need to
     if self.opts.global_max and self.opts.local_max: self.limit_dims_to_max(self.opts.global_max, self.opts.local_max)
 
     # uops
-    self.uops: List[UOp] = []
+    self.uops:UOpGraph = UOpGraph()
     self.buf_uops: List[Optional[UOp]] = [None]*len(self.bufs)
     self.loop_uops: Dict[str, UOp] = {}
 
     # add global buffers
     for i,buf in enumerate(self.bufs):
       if isinstance(buf, MemBuffer):
-        self.buf_uops[i] = self.uop(UOps.DEFINE_GLOBAL, buf.dtype if isinstance(buf.dtype, ImageDType) else PtrDType(buf.dtype), (), f"data{buf.idx}")
+        self.buf_uops[i] = self.uops.add(UOps.DEFINE_GLOBAL,
+                                         buf.dtype if isinstance(buf.dtype, ImageDType) else PtrDType(buf.dtype), (),
+                                         (buf.idx, any(buf.idx == x.idx for x in self.outbufs)))
     # add var vals
-    for var in self.ast.vars():
+    for i,var in enumerate(self.vars):
       assert var.expr is not None
-      self.loop_uops[var.expr] = self.uop(UOps.DEFINE_GLOBAL, dtypes.int32, (), var.expr)
+      self.loop_uops[var.expr] = self.uops.add(UOps.DEFINE_VAR, dtypes.int32, (), var)
     # define local buffers
     for lb in self.local_alias.values():
-      self.buf_uops[self.bufs.index(lb)] = self.uop(UOps.DEFINE_LOCAL, PtrDType(dtypes.float32), (), (lb.name, self.sts[self.bufs.index(lb)].size))
+      self.buf_uops[self.bufs.index(lb)] = self.uops.add(UOps.DEFINE_LOCAL,
+                                                         PtrDType(dtypes.float32), (), (lb.name, self.sts[self.bufs.index(lb)].size))
     # add a local buffer for multistage reduce. # TODO: use local alias
-    if self.group_for_reduce:
+    if self.group_for_reduces:
       # TODO: the strides of this can be controlled
-      self.sts.append(ShapeTracker.from_shape(tuple([1] * self.global_dims + list(self.full_shape[self.global_dims:self.global_dims+self.local_dims+len(self.group_for_reduce)]) + [1] * (self.shape_len - self.upcasted - len(self.group_for_reduce) - self.first_reduce) + [x[0] for x in self.upcasted_axis(0)])))  # noqa: E501
-      temp_dtype = self.get_base_dtype(get_lazyop_info(self.reduceop).dtype)
+      self.sts.append(ShapeTracker.from_shape(tuple([1] * self.global_dims + list(self.full_shape[self.global_dims:self.global_dims+self.local_dims+self.group_for_reduces]) + [1] * (self.shape_len - self.upcasted - self.group_for_reduces - self.first_reduce) + [x[0] for x in self.upcasted_axis(0)])))  # noqa: E501
+      temp_dtype = self.get_base_dtype(cast(LazyOp, self.reduceop).dtype)
       self.bufs.append(LocalBuffer("temp", self.sts[-1].size, temp_dtype))
-      self.buf_uops.append(self.uop(UOps.DEFINE_LOCAL, PtrDType(temp_dtype), (), ("temp", self.sts[-1].size)))
+      self.buf_uops.append(self.uops.add(UOps.DEFINE_LOCAL, PtrDType(temp_dtype), (), ("temp", self.sts[-1].size)))
 
     # kernel name (before late upcast)
-    self.name = ("r_" if self.reduceop else "E_") + colored('_', 'BLACK').join([colored(str(x), c) for x,c in zip(self.full_shape, self.colors())])
+    self.name = ("r" if self.reduceop else ("C" if all(x.op in BufferOps for x in self.lazyops) else "E")) + \
+                 (f"{len(self.outbufs)}_" if len(self.outbufs) > 1 else "_") + \
+                 colored('_', 'BLACK').join([colored(str(x), c) for x,c in zip(self.full_shape, self.colors())])
 
     # name the function something unique
     Linearizer.kernel_cnt[(function_name := to_function_name(self.name))] += 1
     suffix = f"{'n'+str(Linearizer.kernel_cnt[function_name]-1)}" if Linearizer.kernel_cnt[function_name] > 1 else ""
     self.name = self.name+colored(suffix, 'BLACK')
 
     # define indexes
     global_idxs, loop_global_idxs = get_grouped_dims("gidx", 0, self.full_shape[:self.global_dims], 3 if self.opts.has_local else 0)
-    local_idxs, loop_local_idxs = get_grouped_dims("lidx", self.global_dims, self.full_shape[self.global_dims:self.first_reduce+len(self.group_for_reduce)], 3 if self.opts.has_local else 0)  # noqa: E501
-    full_upcast_idxs = [Variable(None, 0, s-1) for s in self.full_shape[self.shape_len-self.upcasted:]]
-    upcast_idxs = [Variable(None, 0, s-1) for s in self.output_shape[self.shape_len-self.upcasted:]]
-
-    # global and local loops
-    def render_loop(xx:List[Variable]) -> Tuple[UOp, ...]:
-      new_loops = {x.expr:self.uop(UOps.LOOP, dtypes.int32, (
-        self.const(x.min) if isinstance(x.min, int) else cast(Node, x.min).render(self.render_ops, self),
-        self.const(x.max+1) if isinstance(x.max, int) else cast(Node, x.max+1).render(self.render_ops, self)), cachable=False) for x in xx if not isinstance(x, NumNode) and x.expr is not None}  # noqa: E501
-      self.loop_uops.update(new_loops)
-      return tuple(new_loops.values())
+    local_idxs, loop_local_idxs = get_grouped_dims("lidx", self.global_dims, self.full_shape[self.global_dims:self.first_reduce+self.group_for_reduces], 3 if self.opts.has_local else 0)  # noqa: E501
+    upcast_idxs = [Variable(f"_uidx{i}", 0, s-1) for i, s in enumerate(self.output_shape[self.shape_len-self.upcasted:])]
 
     # set global/local size
     self.global_size: Optional[List[int]] = None
     self.local_size: Optional[List[int]] = None
     if self.dont_use_locals:
       self.global_size = [x.max+1 for x in loop_global_idxs][::-1]
-      self.loop_uops.update({x.expr:self.uop(UOps.SPECIAL, dtypes.int32, (), (len(loop_global_idxs)-1-i, x.expr.replace("gidx", "idx"), x.max+1)) for i,x in enumerate(loop_global_idxs)})  # noqa: E501
+      self.loop_uops.update({x.expr:self.uops.add(UOps.SPECIAL, dtypes.int32, (), (len(loop_global_idxs)-1-i, x.expr.replace("gidx", "idx"), x.max+1)) for i,x in enumerate(loop_global_idxs)})  # noqa: E501
     elif self.opts.has_local:
-      self.global_size, self.local_size = [x.max+1 for x in loop_global_idxs][::-1], [x.max+1 for x in loop_local_idxs][::-1]
-      self.loop_uops.update({x.expr:self.uop(UOps.SPECIAL, dtypes.int32, (), (len(loop_global_idxs)-1-i, x.expr, x.max+1)) for i,x in enumerate(loop_global_idxs)})  # noqa: E501
-      self.loop_uops.update({x.expr:self.uop(UOps.SPECIAL, dtypes.int32, (), (len(loop_local_idxs)-1-i, x.expr, x.max+1)) for i,x in enumerate(loop_local_idxs)})  # noqa: E501
+      self.global_size, self.local_size = [x.max+1 for x in loop_global_idxs][::-1], [x.max+1 for x in loop_local_idxs]
+      self.loop_uops.update({x.expr:self.uops.add(UOps.SPECIAL, dtypes.int32, (), (len(loop_global_idxs)-1-i, x.expr, x.max+1)) for i,x in enumerate(loop_global_idxs)})  # noqa: E501
+      self.loop_uops.update({x.expr:self.uops.add(UOps.SPECIAL, dtypes.int32, (), (i, x.expr, x.max+1)) for i,x in enumerate(loop_local_idxs)})
     else:
-      render_loop(loop_global_idxs+loop_local_idxs)
+      self.render_loop(loop_global_idxs+loop_local_idxs, 1)
+    if self.global_size is not None: self.global_size += [1]*(3-len(self.global_size))
+    if self.local_size is not None: self.local_size += [1]*(3-len(self.local_size))
 
     # parse AST
-    loaded_buffers = {}
-    acc: List[UOp] = []
+    loaded_buffers:Dict[Union[MemBuffer, ConstBuffer, LocalBuffer], List[UOp]] = {}
+    accs: Dict[LazyOp, List[UOp]] = {}
     self.load_cache: Dict[str, UOp] = {}
 
     # reduce op
     fake_reduce_idxs: List[Variable] = []
-    if self.reduceop is not None:
-      # define indexes
-      reduce_idxs = [Variable(f"ridx{i}", 0, self.full_shape[i]-1) for i in range(self.first_reduce+len(self.group_for_reduce), self.shape_len-self.upcasted)]  # noqa: E501
-      fake_reduce_idxs = [x*0 for x in reduce_idxs]
-
-      # define accumulator
-      acc = self.global_load(0, global_idxs+local_idxs+fake_reduce_idxs+upcast_idxs, self.get_reduce_acc(self.reduceop))
-
-      if self.tensor_core:
-        def calc_tc_idxs(local_size: int, aliases: List[List[int]]):
-          replace_idxs = []
-          for alias in aliases:
-            full_var, full_var_sz = NumNode(0), 1
-            if alias[0] != 0:
-              for i in alias:
-                next_var = local_idxs[-i] if i > 0 else Variable(None, 0, local_size-1)
-                full_var += next_var * full_var_sz
-                full_var_sz *= next_var.max+1
-            replace_idxs.append(full_var)
-          return replace_idxs
-        replace_acc_idxs = calc_tc_idxs(self.tensor_core.thread_local_sizes[2], self.tensor_core.thread_local_aliases[2])
-        for n in range(len(self.tensor_core.threads)):
-          local_idxs[self.local_dims-len(self.tensor_core.threads)+n] = replace_acc_idxs[n] # replace locals
-        for n in range(len(replace_acc_idxs)-len(self.tensor_core.threads)):
-          upcast_idxs[n] = replace_acc_idxs[len(self.tensor_core.threads)+n] # replace upcasts
-
-      # reduce loop
-      loop_ctx = render_loop(reduce_idxs)
-
-      # barrier for fast GEMM
-      if self.tensor_core: self.uop(UOps.BARRIER, None, (), cachable=False)
-
-      # compute local aliases
-      locals_to_store = []
-      for i in self.local_alias:
-        localbuf_idx = self.bufs.index(self.local_alias[i])
-        buf_idxs = [idx*0 if s == 0 else idx for idx,s in zip(global_idxs+local_idxs+reduce_idxs+full_upcast_idxs,self.sts[i].real_strides())]
-        if self.tensor_core:
-          min_alias_idx = min(self.local_alias.keys())
-          replace_input_idxs = calc_tc_idxs(self.tensor_core.thread_local_sizes[i-min_alias_idx], self.tensor_core.thread_local_aliases[i-min_alias_idx])  # noqa: E501
-          for n in range(len(self.tensor_core.threads)):
-            buf_idxs[self.first_reduce-len(self.tensor_core.threads)+n] = replace_input_idxs[n] # replace locals
-          for n in range(len(replace_input_idxs)-len(self.tensor_core.threads)):
-            buf_idxs[self.shape_len-self.upcasted+n] = replace_input_idxs[len(self.tensor_core.threads)+n] # replace upcasts
-        if DEBUG >= 3: print(f"{localbuf_idx} alias {i}: idxs=", buf_idxs)
-        ll = self.global_load(i, buf_idxs)
-        locals_to_store.append((localbuf_idx, buf_idxs, ll))
-
-      # copy in any global buffers
-      if self.tensor_core:
-        wmma_sz = self.tensor_core.thread_local_sizes
-        # calculate the number of local accumulator reduces and render WMMAs: this is bad... this needs to come from someplace else
-        nx, ny, nacc = (len(locals_to_store[0][2])//wmma_sz[0]), (len(locals_to_store[1][2])//wmma_sz[1]), (len(acc)//wmma_sz[2])
-        acc_reds = math.isqrt((nx*ny)//nacc)
-        i, bx, by = 0, nx//acc_reds, ny//acc_reds
-        for y in range(by):
-          for x in range(bx):
-            for j in range(acc_reds):
-              op1, op2, op3 = locals_to_store[0][2][(x+(j*bx))*wmma_sz[0]:(x+(j*bx)+1)*wmma_sz[0]], locals_to_store[1][2][(y+(j*by))*wmma_sz[1]:(y+(j*by)+1)*wmma_sz[1]], acc[i:i+wmma_sz[2]]  # noqa: E501
-              if self.opts.device != "HIP":
-                ops = tuple(op1+op2+op3)
-              else:
-                ops = (self.uop(UOps.CAST, dtypes.half.vec(16), tuple(op1)),
-                       self.uop(UOps.CAST, dtypes.half.vec(16), tuple(op2)),
-                       self.uop(UOps.CAST, dtypes.float.vec(8), tuple(op3)))
-              ret = self.uop(UOps.WMMA, dtypes.float.vec(2) if wmma_sz[2] == 2 else dtypes.float.vec(8), ops, (self.opts.device, self.tensor_core.dtype_in, self.tensor_core.dtype_out,))  # noqa: E501
-              for z in range(cast(DType, ret.dtype).sz):
-                acc[i+z] = self.uop(UOps.PHI, dtypes.float, (op3[z], self.uop(UOps.GEP, dtypes.float, (ret,), z)) + loop_ctx)
-            i += wmma_sz[2]
-      else:
-        if locals_to_store:
-          self.uop(UOps.BARRIER, None, (), cachable=False)
-          for i, idxs, ll in locals_to_store: self.global_store(i, idxs, ll)
-          self.uop(UOps.BARRIER, None, (), cachable=False)
-
-        # load earlybufs
-        loaded_buffers.update({b:self.global_load(self.bufs.index(self.local_alias[i]) if i in self.local_alias else i, global_idxs+local_idxs+reduce_idxs+full_upcast_idxs) for i,b in enumerate(self.bufs[1:], start=1) if b in self.earlybufs})  # noqa: E501
-
-        # run early AST (with reduce)
-        self.ast_parse(self.reduceop, acc, self.acc_offsets(self.full_buf_index), loaded_buffers, do_reduce=True, loop_ctx=loop_ctx)
-
-      # end the reduce loop
-      self.load_cache.clear()
-
-      # end the local loop, do the local reduce
-      if self.group_for_reduce:
-        fake_global_idxs = [x*0 for x in global_idxs]
-        stores = self.global_store(-1, fake_global_idxs+local_idxs+fake_reduce_idxs+upcast_idxs, acc)  # store accumulators
-        barrier = self.uop(UOps.BARRIER, None, tuple(stores), cachable=False)
-        if self.opts.has_local:
-          fake_idxs = [NumNode(0)]*len(self.sts[-1].shape)
-          fake_idxs[self.global_dims+self.local_dims:self.global_dims+len(local_idxs)] = local_idxs[self.local_dims:]
-          if_cond: UOp = (self.sts[-1].expr_idxs(fake_idxs)[0]<1).render(self.render_ops, self)
-          barrier = self.uop(UOps.IF, None, (if_cond, barrier), cachable=False)
-
-        # create new late reduce local loops and replace local_idxs that have been used
-        end_local_idxs = [Variable(f"tidx{i}", 0, self.full_shape[i]-1 if i >= self.first_reduce and i not in self.upcast_in_mid_reduce_axes else 0) for i in range(0, self.first_reduce+len(self.group_for_reduce))]  # noqa: E501
-        local_idxs = local_idxs[:self.local_dims] + end_local_idxs[self.global_dims + self.local_dims:]
-
-        # if any group_for_reduce items aren't reduces, upcast them here
-        for j in self.upcast_in_mid_reduce_axes:
-          self.reshape_and_permute(None, [i for i in range(self.shape_len) if i != j] + [j])
-          self.upcast()
-          self.group_for_reduce.pop()
-          local_idxs = local_idxs[:-1]
-          end_local_idxs = end_local_idxs[:-1]
-          # regenerate upcast_idxs
-          upcast_idxs = [Variable(None, 0, s-1) for s in self.output_shape[self.shape_len-self.upcasted:]]
-
-        # NOTE: this structure is the same as the reduce op above
-
-        # define late accumulator
-        acc = self.global_load(-1, fake_global_idxs+local_idxs+fake_reduce_idxs+upcast_idxs, self.get_reduce_acc(self.reduceop))
-
-        # late reduce loop
-        loop_ctx = render_loop(end_local_idxs)
-
-        # load localbufs
-        loaded_buffers[self.bufs[-1]] = self.global_load(-1, fake_global_idxs+local_idxs+fake_reduce_idxs+upcast_idxs, barrier=barrier)
-
-        # there's no AST here (and there's no shape for the reduce LazyOp)
-        self.ast_parse(LazyOp(self.reduceop.op, (LazyOp(BufferOps.LOAD, (), self.bufs[-1]),)), acc, self.acc_offsets(-1), loaded_buffers, do_reduce=True, loop_ctx=loop_ctx)  # noqa: E501
-
-        # end the late reduce loop
-        self.load_cache.clear()
+    for reduceop in [self.reduceop] if self.reduceop is not None else []:
+      accs,loaded_buffers,fake_reduce_idxs,local_idxs,upcast_idxs = \
+        self.render_reduceop(reduceop,accs,loaded_buffers,global_idxs,local_idxs,upcast_idxs)
 
     # load latebufs
-    loaded_buffers.update({b:self.global_load(i, global_idxs+local_idxs+fake_reduce_idxs+upcast_idxs) for i,b in enumerate(self.bufs) if b not in self.earlybufs and i != 0 and b.__class__ is not LocalBuffer})  # noqa: E501
+    loaded_buffers.update({b:self.global_load(i, global_idxs+local_idxs+fake_reduce_idxs+upcast_idxs) \
+                           for i,b in enumerate(self.bufs) if b not in self.earlybufs and b.__class__ is not LocalBuffer})
 
     # run late AST (without the store)
-    val = self.ast_parse(self.ast.src[0], acc, None, loaded_buffers)
-
-    # store
-    self.global_store(0, global_idxs+local_idxs+fake_reduce_idxs+upcast_idxs, val)
-
-    # get PHI node loop scope, link anything using a DEFINE_ACC to the loop as a "parent"
-    acc_scope: DefaultDict[UOp, List[UOp]] = defaultdict(list)
-    for u in self.uops:
-      if u.uop == UOps.PHI:
-        acc_scope[u.vin[0]] += u.vin[2:]
-
-    # graph helper functions
-    @functools.lru_cache(None)
-    def get_recursive_parents(x:UOp, with_phi=False) -> Set[UOp]:
-      return set.union(set(x.vin), *[get_recursive_parents(p, with_phi) for p in x.vin], set(acc_scope[x]) if with_phi else set())
-
-    def get_recursive_children(x:UOp) -> Set[UOp]:
-      deps = set([x])
-      ssize = 0
-      while ssize != len(deps):
-        ssize = len(deps)
-        for u in self.uops:
-          if len(deps.intersection([x for x in u.vin if x.uop != UOps.PHI])):
-            deps.add(u)
-      return deps
-
-    def replace_op(old:UOp, new:UOp):
-      for u in self.uops:
-        u.vin = tuple(new if x is old else x for x in u.vin)
-      self.uops.remove(old)
-
-    # fix loop scope, push uops upward out of loop if it does not depend on the loop
-    loop_stack: List[List[UOp]] = [[]]
-    for u in self.uops:
-      if not loop_stack[-1]: loop_stack[-1].append(u)
-      elif u.uop == UOps.LOOP: loop_stack.append([u])
-      elif u.uop not in [UOps.CONST, UOps.ALU, UOps.CAST, UOps.LOAD]: loop_stack[-1].append(u)
-      else:
-        parents = get_recursive_parents(u, with_phi=True)
-        # don't push any local buffer because there might have STORE and BARRIER (not considered as parent) between DEFINE_LOCAL and here
-        if any(u.uop == UOps.DEFINE_LOCAL for u in parents): loop_stack[-1].append(u)
-        else:
-          for i in reversed(range(len(loop_stack))):
-            # check backwards and put the uop in the first encounter with some dependency
-            if any(x in parents for x in loop_stack[i]) or i == 0:
-              loop_stack[i].append(u)
-              break
-    self.uops = flatten(loop_stack)
-
-    # uops optimization
-    changed_something = True
-    while changed_something:
-      changed_something = False
-      for u in self.uops:
-        if u.uop == UOps.PHI and len(u.vin) == 3:
-          # if the parents of the PHI node don't have the LOOP in their parents, it can be folded
-          # TODO: ADD becomes a MUL, MAX can just become nothing
-          if all(x.uop != UOps.LOOP for x in get_recursive_parents(UOp(u.uop, u.dtype, u.vin[0:2], u.arg))) and u.vin[1].arg == BinaryOps.ADD:
-            if DEBUG >= 4: print(f"removing PHI node {u}")
-            del self.saved_exprs[(u.uop, u.dtype, u.vin, u.arg)]
-            # NOTE: assuming u.vin[2].vin[1] and u.vin[2].vin[0] have the same dtype
-            loop_len = self.uop(UOps.ALU, u.vin[2].vin[1].dtype, (u.vin[2].vin[1], u.vin[2].vin[0]), BinaryOps.SUB, insert_before=self.uops.index(u))
-            if loop_len.dtype != u.dtype: loop_len = self.uop(UOps.CAST, u.dtype, (loop_len,), insert_before=self.uops.index(u))
-            replace_op(u, self.uop(UOps.ALU, u.dtype, (u.vin[1], loop_len,), BinaryOps.MUL, insert_before=self.uops.index(u)))
-            changed_something = True
-
-    # (recursively) remove childless uops
-    # NOTE: DEFINE_GLOBAL should be removable, but we'd have to propagate that
-    UOPS_W_SIDE_EFFECTS = {UOps.STORE, UOps.BARRIER, UOps.DEFINE_GLOBAL}
-    while 1:
-      has_child: Set[UOp] = set()
-      for ru in self.uops:
-        for vu in ru.vin:
-          has_child.add(vu)
-      nu: List[UOp] = [x for x in self.uops if x in has_child or x.uop in UOPS_W_SIDE_EFFECTS]
-      if len(nu) == len(self.uops): break
-      if DEBUG >= 4: print(f"reduced UOp count from {len(self.uops)} to {len(nu)}")
-      self.uops = nu
-      del nu
-
-    # add UOps.END
-    for u in self.uops:
-      if u.uop == UOps.LOOP:
-        # add END of loops after the last thing that (recursively) depends on them
-        self.uop(UOps.END, None, (u,), cachable=False, insert_before=self.uops.index(sorted(list(get_recursive_children(u)), key=self.uops.index)[-1])+1)  # noqa: E501
-      elif u.uop == UOps.IF:
-        # END any if statements at the end of the uops
-        self.uop(UOps.END, None, (u,), cachable=False)
+    for op in self.ast:
+      val = self.ast_parse(op.src[0], accs, None, loaded_buffers)
+      self.global_store(op.arg.idx, global_idxs+local_idxs+fake_reduce_idxs+upcast_idxs, val)
 
     # maybe graph the uops
-    if DEBUG >= 5:
-      for u in self.uops:
-        print(f"{self.uops.index(u):4d} {str(u.uop):20s}: {str(u.dtype) if u.dtype is not None else '':25s} {str([self.uops.index(x) for x in u.vin]):32s} {u.arg}")  # noqa: E501
-    if getenv("GRAPHUOPS"):
-      from tinygrad.graph import graph_uops
-      graph_uops(self.uops)
+    if DEBUG >= 5: self.uops.print()
+    if getenv("GRAPHUOPS"): self.uops.graph()
 
     # restore backups
-    self.sts, self.group_for_reduce, self.upcasted = sts_backup, gfr_backup, upc_backup
+    self.sts, self.group_for_reduces, self.upcasted = sts_backup, gfr_backup, upc_backup
 
     # set cache and return
     self.applied_opts_cache = self.applied_opts[:]
     return self
 
-  def uop(self, uop:UOps, dtype:Optional[DType]=None, vin:Tuple[UOp, ...]=tuple(), arg:Any=None, cachable=True, insert_before=None, simplify=True) -> UOp:  # noqa: E501
-    if uop == UOps.ALU:
-      if arg in UnaryOps:
-        assert dtype == vin[0].dtype, f"{arg} dtype mismatch {dtype=} != {vin[0].dtype=}"
-      elif arg in (BinaryOps.CMPLT, BinaryOps.CMPEQ):
-        assert dtype == dtypes.bool, f"{arg} output dtype mismatch {dtype=} != {dtypes.bool}"
-        assert vin[0].dtype == vin[1].dtype, f"{arg} dtype mismatch {dtype=} != {vin[0].dtype=} != {vin[1].dtype=}"
-      elif arg in BinaryOps:
-        assert dtype == vin[0].dtype == vin[1].dtype, f"{arg} dtype mismatch {dtype=} != {vin[0].dtype=} != {vin[1].dtype=}"
-      elif arg == TernaryOps.WHERE:
-        assert vin[0].dtype == dtypes.bool, f"{arg} selector dtype mismatch {vin[0].dtype=} != {dtypes.bool}"
-        assert dtype == vin[1].dtype == vin[2].dtype, f"{arg} choice dtype mismatch {dtype=} != {vin[1].dtype=} != {vin[2].dtype=}"
-
-    if simplify:
-      if uop == UOps.PHI and len(vin) == 2: return vin[1]   # a phi without loops is a noop
-      if uop == UOps.GEP and vin[0].uop == UOps.CONST: return self.const(vin[0].arg, dtype, insert_before)
-      if uop == UOps.CAST and all(x.uop == UOps.CONST for x in vin) and all_same([x.arg for x in vin]):
-        return self.const(vin[0].arg, dtype, insert_before)
-      if uop == UOps.ALU:
-        # rewrites. NOTE: the rewritten NEG op is still around...
-        if arg == BinaryOps.ADD and vin[1].uop == UOps.ALU and vin[1].arg == UnaryOps.NEG:
-          return self.uop(UOps.ALU, dtype, (vin[0], vin[1].vin[0]), BinaryOps.SUB, cachable, insert_before)
-        # constant folding
-        if arg == UnaryOps.NEG and vin[0].uop == UOps.CONST: return self.const(-vin[0].arg, dtype, insert_before)
-        if arg == TernaryOps.WHERE and vin[1] == vin[2]: return vin[1] # a conditional with the same results either way is a noop
-        # zero folding
-        for x in [0,1]:
-          if arg == BinaryOps.ADD and vin[x].uop == UOps.CONST and vin[x].arg == 0.0: return vin[1-x]
-          if arg == BinaryOps.MUL and vin[x].uop == UOps.CONST and vin[x].arg == 1.0: return vin[1-x]
-          if arg == BinaryOps.MUL and vin[x].uop == UOps.CONST and vin[x].arg == 0.0: return vin[x]
-        if arg == BinaryOps.SUB and vin[1].uop == UOps.CONST and vin[1].arg == 0.0: return vin[0]
-        if arg == BinaryOps.DIV and vin[1].uop == UOps.CONST and vin[1].arg == 1.0: return vin[0]
-
-    key = (uop, dtype, vin, arg)
-    if insert_before is None: insert_before = len(self.uops)
-    # check if the cached expr is valid with the given insert place.
-    if cachable and (expr:=self.saved_exprs.get(key, None)) is not None and self.uops.index(expr) <= insert_before: return expr
-    ret = UOp(uop, dtype, vin, arg)
-    self.uops.insert(insert_before, ret)
-    if cachable: self.saved_exprs[key] = ret
-    return ret
-
-  def ast_parse(self, x:LazyOp, acc: List[UOp], offs:Optional[List[int]], loaded_buffers:Dict[Union[MemBuffer, ConstBuffer, LocalBuffer], List[UOp]], do_reduce=False, loop_ctx=tuple(), cache=None) -> List[UOp]:  # noqa: E501
+  def ast_parse(self, x:LazyOp, accs:Dict[LazyOp, List[UOp]], offs:Optional[List[int]], loaded_buffers:Dict[Union[MemBuffer, ConstBuffer, LocalBuffer], List[UOp]], reduce_acc:Optional[List[UOp]]=None, cache=None) -> List[UOp]: # noqa: E501
     if cache is None: cache = {}
     if x in cache: return cache[x]
     if x.op in BufferOps: return loaded_buffers[x.arg]
-    if x.op == UnaryOps.CAST:
-      return [self.uop(UOps.CAST, self.get_base_dtype(x.arg[0]), (u,), x.arg) for u in self.ast_parse(x.src[0], acc, offs, loaded_buffers)]
-    if x.op in ReduceOps and not do_reduce:
+    if x.op in [UnaryOps.CAST, UnaryOps.BITCAST]:
+      return [self.uops.add(UOps.BITCAST if x.op is UnaryOps.BITCAST else UOps.CAST,
+                            self.get_base_dtype(x.arg), (u,)) for u in self.ast_parse(x.src[0], accs, offs, loaded_buffers)]
+    if x.op in ReduceOps and reduce_acc is None:
       assert offs is None, "not available if we aren't doing reduce"
-      return acc
-    # MULACC fusion. TODO: this is copied from Interpreted
-    if x.op == ReduceOps.SUM:
-      if x.src[0].op == BinaryOps.MUL: x = LazyOp(TernaryOps.MULACC, x.src[0].src, x.arg)
-      if (castop:=x.src[0]).op == UnaryOps.CAST and (mulop:=castop.src[0]).op == BinaryOps.MUL:
-        # MULACC with acc cast rewrite: MUL -> CAST -> SUM => CAST -> MULACC
-        x = LazyOp(TernaryOps.MULACC, tuple(LazyOp(UnaryOps.CAST, (s, ), castop.arg) for s in mulop.src), x.arg)
+      return accs[x]
 
-    values = [self.ast_parse(v, acc, offs, loaded_buffers, loop_ctx=loop_ctx, cache=cache) for v in x.src]
-    ops = {ReduceOps.SUM:BinaryOps.ADD, ReduceOps.MAX:BinaryOps.MAX, TernaryOps.MULACC:TernaryOps.MULACC}
+    values = [self.ast_parse(v, accs, offs, loaded_buffers, cache=cache) for v in x.src]
+    ops = {ReduceOps.SUM:BinaryOps.ADD, ReduceOps.MAX:BinaryOps.MAX}
     if x.op in ops:
+      assert reduce_acc is not None
       ret: List[UOp] = []
-      input_acc = acc[:]
+      acc, input_acc = reduce_acc, reduce_acc[:]
       for val, off in zip(zip(*values), cast(List[int], offs)):
-        acc[off] = self.uop(UOps.ALU, acc[off].dtype, vin=val+(acc[off],), arg=ops[x.op])
+        acc[off] = UOp.alu(ops[cast(ReduceOps, x.op)], *(val+(acc[off], )))
         ret.append(acc[off])
       for off in range(len(acc)):
         if input_acc[off] != acc[off]:
-          acc[off] = self.uop(UOps.PHI, input_acc[off].dtype, (input_acc[off], acc[off]) + tuple(loop_ctx))
-    else:
-      ret = [self.uop(UOps.ALU, dtypes.bool if x.op in (BinaryOps.CMPLT, BinaryOps.CMPEQ) else val[-1].dtype, val, x.op) for val in zip(*values)]
+          acc[off] = self.uops.add(UOps.PHI, input_acc[off].dtype, (input_acc[off], acc[off]))
+    else: ret = [UOp.alu(x.op, *vin) for vin in zip(*values)]
     cache[x] = ret
     return ret
+
+  def to_program(self) -> Program:
+    self.linearize()
+    info = get_lazyop_info(self.ast[0])
+    src = self.opts.render(to_function_name(self.name), self.uops)
+    ops, mem = self.uops.flops_mem()
+    run_count = prod((self.global_size if self.global_size else []) + (self.local_size if self.local_size else []))
+    # NOTE: we use min here to ignore the indexing FLOPS
+    return Program(self.name, src, self.opts.device, self.global_size, self.local_size,
+                   self.uops, min(info.flops, ops * run_count), min(info.mem_estimate, mem * run_count))
```

### Comparing `tinygrad-0.8.0/tinygrad/dtype.py` & `tinygrad-0.9.0/tinygrad/dtype.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,86 +1,96 @@
-from typing import NamedTuple, Final, Optional, ClassVar, Set, Tuple, Dict
+from typing import Final, Optional, ClassVar, Set, Tuple, Dict, Union
+from dataclasses import dataclass
 import numpy as np  # TODO: remove numpy
 import functools
+from tinygrad.helpers import getenv
 
-# TODO: migrate this from NamedTuple -> dataclass
-class DType(NamedTuple):
+ConstType = Union[float, int, bool]
+
+@dataclass(frozen=True, order=True)
+class DType:
   priority: int  # this determines when things get upcasted
   itemsize: int
   name: str
-  np: Optional[type]  # TODO: someday this will be removed with the "remove numpy" project
-  sz: int = 1
-  def __repr__(self): return f"dtypes.{INVERSE_DTYPES_DICT[self]}" if self.sz == 1 else f"dtypes._{INVERSE_DTYPES_DICT[self.scalar()]}{self.sz}"
+  fmt: Optional[str]
+  count: int
+  def __repr__(self): return f"dtypes.{'_'*(c:=self.count!=1)}{INVERSE_DTYPES_DICT[self.name if not c else self.scalar().name]}{str(self.count)*c}"
   def vec(self, sz:int):
-    assert sz > 1 and self.sz == 1, f"can't vectorize {self} with size {sz}"
-    return DType(self.priority, self.itemsize*sz, f"{INVERSE_DTYPES_DICT[self]}{sz}", None, sz)
-  def scalar(self): return DTYPES_DICT[self.name[:-len(str(self.sz))]] if self.sz > 1 else self
+    assert sz > 1 and self.count == 1, f"can't vectorize {self} with size {sz}"
+    return DType(self.priority, self.itemsize*sz, f"{INVERSE_DTYPES_DICT[self.name]}{sz}", None, sz)
+  def scalar(self): return DTYPES_DICT[self.name[:-len(str(self.count))]] if self.count > 1 else self
+  # TODO: someday this will be removed with the "remove numpy" project
+  @property
+  def np(self) -> Optional[type]: return np.dtype(self.fmt).type if self.fmt is not None else None
 
 # dependent typing?
+@dataclass(frozen=True, repr=False)
 class ImageDType(DType):
-  def __new__(cls, priority, itemsize, name, np, shape, base):
-    return super().__new__(cls, priority, itemsize, name, np)
-  def __init__(self, priority, itemsize, name, np, shape, base):
-    self.shape: Tuple[int, ...] = shape  # arbitrary arg for the dtype, used in image for the shape
-    self.base: DType = base
-    super().__init__()
+  shape: Tuple[int, ...]   # arbitrary arg for the dtype, used in image for the shape
+  base: DType
   def scalar(self): return self.base
   def vec(self, sz:int): return self.base.vec(sz)
   def __repr__(self): return f"dtypes.{self.name}({self.shape})"
-  # TODO: fix this to not need these
-  def __hash__(self): return hash((super().__hash__(), self.shape))
-  def __eq__(self, x): return super().__eq__(x) and self.shape == x.shape
-  def __ne__(self, x): return super().__ne__(x) or self.shape != x.shape
 
+# @dataclass(frozen=True, init=False, repr=False, eq=False)
 class PtrDType(DType):
-  def __new__(cls, dt:DType): return super().__new__(cls, dt.priority, dt.itemsize, dt.name, dt.np, dt.sz)
+  def __init__(self, dt:DType): super().__init__(dt.priority, dt.itemsize, dt.name, dt.fmt, dt.count)
   def __repr__(self): return f"ptr.{super().__repr__()}"
+  def __hash__(self): return super().__hash__()
+  def __eq__(self, dt): return self.priority==dt.priority and self.itemsize==dt.itemsize and self.name==dt.name and self.count==dt.count
+  def __ne__(self, dt): return not (self == dt)
 
 class dtypes:
   @staticmethod
   def is_float(x: DType) -> bool: return x.scalar() in (dtypes.float16, dtypes.bfloat16, dtypes.float32, dtypes.float64)
   @staticmethod # static methds on top, or bool in the type info will refer to dtypes.bool
   def is_int(x: DType) -> bool: return x.scalar() in (dtypes.int8, dtypes.int16, dtypes.int32, dtypes.int64) or dtypes.is_unsigned(x)
   @staticmethod
   def is_unsigned(x: DType) -> bool: return x.scalar() in (dtypes.uint8, dtypes.uint16, dtypes.uint32, dtypes.uint64)
   @staticmethod
-  def from_np(x) -> DType: return DTYPES_DICT[np.dtype(x).name]
+  def from_np(x: type) -> DType: return DTYPES_DICT[np.dtype(x).name]
   @staticmethod  # NOTE: isinstance(True, int) is True in python
   def from_py(x) -> DType: return dtypes.default_float if isinstance(x, float) else dtypes.bool if isinstance(x, bool) else dtypes.default_int
   @staticmethod
+  def as_const(val: ConstType, dtype:DType): return int(val) if dtypes.is_int(dtype) else float(val) if dtypes.is_float(dtype) else bool(val)
+  @staticmethod
   def fields() -> Dict[str, DType]: return DTYPES_DICT
-  bool: Final[DType] = DType(0, 1, "bool", np.bool_)
-  int8: Final[DType] = DType(1, 1, "char", np.int8)
-  uint8: Final[DType] = DType(2, 1, "unsigned char", np.uint8)
-  int16: Final[DType] = DType(3, 2, "short", np.int16)
-  uint16: Final[DType] = DType(4, 2, "unsigned short", np.uint16)
-  int32: Final[DType] = DType(5, 4, "int", np.int32)
-  uint32: Final[DType] = DType(6, 4, "unsigned int", np.uint32)
-  int64: Final[DType] = DType(7, 8, "long", np.int64)
-  uint64: Final[DType] = DType(8, 8, "unsigned long", np.uint64)
-  float16: Final[DType] = DType(9, 2, "half", np.float16)
+  bool: Final[DType] = DType(0, 1, "bool", '?', 1)
+  int8: Final[DType] = DType(1, 1, "char", 'b', 1)
+  uint8: Final[DType] = DType(2, 1, "unsigned char", 'B', 1)
+  int16: Final[DType] = DType(3, 2, "short", 'h', 1)
+  uint16: Final[DType] = DType(4, 2, "unsigned short", 'H', 1)
+  int32: Final[DType] = DType(5, 4, "int", 'i', 1)
+  uint32: Final[DType] = DType(6, 4, "unsigned int", 'I', 1)
+  int64: Final[DType] = DType(7, 8, "long", 'l', 1)
+  uint64: Final[DType] = DType(8, 8, "unsigned long", 'L', 1)
+  float16: Final[DType] = DType(9, 2, "half", 'e', 1)
   # bfloat16 has higher priority than float16, so least_upper_dtype(dtypes.int64, dtypes.uint64) = dtypes.float16
-  bfloat16: Final[DType] = DType(10, 2, "__bf16", None)
-  float32: Final[DType] = DType(11, 4, "float", np.float32)
-  float64: Final[DType] = DType(12, 8, "double", np.float64)
+  bfloat16: Final[DType] = DType(10, 2, "__bf16", None, 1)
+  float32: Final[DType] = DType(11, 4, "float", 'f', 1)
+  float64: Final[DType] = DType(12, 8, "double", 'd', 1)
 
   # dtype aliases
   half = float16; float = float32; double = float64 # noqa: E702
   uchar = uint8; ushort = uint16; uint = uint32; ulong = uint64 # noqa: E702
   char = int8; short = int16; int = int32; long = int64 # noqa: E702
 
   # NOTE: these are image dtypes
   @staticmethod
-  def imageh(shp): return ImageDType(100, 2, "imageh", np.float16, shp, dtypes.float32)
+  def imageh(shp): return ImageDType(100, 2, "imageh", 'e', 1, shape=shp, base=dtypes.float32)
   @staticmethod
-  def imagef(shp): return ImageDType(100, 4, "imagef", np.float32, shp, dtypes.float32)
+  def imagef(shp): return ImageDType(100, 4, "imagef", 'f', 1, shape=shp, base=dtypes.float32)
 
   default_float: ClassVar[DType] = float32
   default_int: ClassVar[DType] = int32
 
+if (env_default_float := getenv("DEFAULT_FLOAT", "")):
+  dtypes.default_float = getattr(dtypes, env_default_float.lower())
+  assert dtypes.is_float(dtypes.default_float), f"{env_default_float} is not a float dtype"
+
 # https://jax.readthedocs.io/en/latest/jep/9407-type-promotion.html
 # we don't support weak type and complex type
 promo_lattice = { dtypes.bool: [dtypes.int8, dtypes.uint8], dtypes.int8: [dtypes.int16], dtypes.int16: [dtypes.int32], dtypes.int32: [dtypes.int64],
   dtypes.int64: [dtypes.float16, dtypes.bfloat16], dtypes.uint8: [dtypes.int16, dtypes.uint16], dtypes.uint16: [dtypes.int32, dtypes.uint32],
   dtypes.uint32: [dtypes.int64, dtypes.uint64], dtypes.uint64: [dtypes.float16, dtypes.bfloat16],
   dtypes.float16: [dtypes.float32], dtypes.bfloat16: [dtypes.float32], dtypes.float32: [dtypes.float64], }
 
@@ -90,8 +100,14 @@
 @functools.lru_cache(None)
 def least_upper_dtype(*ds:DType) -> DType:
   return min(set.intersection(*[_get_recursive_parents(d) for d in ds])) if not (images:=[d for d in ds if isinstance(d, ImageDType)]) else images[0]
 def least_upper_float(dt:DType) -> DType: return dt if dtypes.is_float(dt) else least_upper_dtype(dt, dtypes.float32)
 
 # HACK: staticmethods are not callable in 3.8 so we have to compare the class
 DTYPES_DICT = {k: v for k, v in dtypes.__dict__.items() if not (k.startswith(('__', 'default')) or v.__class__ is staticmethod)}
-INVERSE_DTYPES_DICT = {v:k for k,v in DTYPES_DICT.items()}
+INVERSE_DTYPES_DICT = {v.name:k for k,v in DTYPES_DICT.items()}
+
+def sum_acc_dtype(dt:DType):
+  # default acc dtype for sum
+  if dtypes.is_unsigned(dt): return least_upper_dtype(dt, dtypes.uint)
+  if dtypes.is_int(dt) or dt == dtypes.bool: return least_upper_dtype(dt, dtypes.int)
+  return least_upper_dtype(dt, dtypes.float)
```

### Comparing `tinygrad-0.8.0/tinygrad/graph.py` & `tinygrad-0.9.0/tinygrad/engine/graph.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,106 +1,100 @@
-import os, atexit
+import os, atexit, functools
 from collections import defaultdict
 from typing import List, Any, DefaultDict
-from tinygrad.ops import UnaryOps, BinaryOps, ReduceOps, MovementOps, LoadOps, BufferOps, TernaryOps, Op, LazyOp, GlobalCounters
+from tinygrad.ops import UnaryOps, BinaryOps, ReduceOps, LoadOps, BufferOps, TernaryOps, LazyOp
 from tinygrad.device import Device
-from tinygrad.helpers import GRAPH, GRAPHPATH, DEBUG, getenv
+from tinygrad.helpers import GRAPHPATH, DEBUG, GlobalCounters, getenv
 from tinygrad.codegen.linearizer import UOps, UOp
 from tinygrad.shape.symbolic import NumNode
+from tinygrad.lazy import LazyBuffer
+
+try: import networkx as nx
+except ImportError: pass
 
 # **** debugging and graphing ****
 
 if DEBUG >= 2:
   def print_globalcounters():
     if GlobalCounters.time_sum_s == 0: return
     print(f"avg: {GlobalCounters.global_ops*1e-9/GlobalCounters.time_sum_s:8.2f} GFLOPS {GlobalCounters.global_mem*1e-9/GlobalCounters.time_sum_s:8.2f} GB/s",  # noqa: E501
           f"{' '*10}total: {GlobalCounters.kernel_count:5d} kernels {GlobalCounters.global_ops*1e-9:8.2f} GOPS {GlobalCounters.global_mem*1e-9:8.2f} GB {GlobalCounters.time_sum_s*1e3:8.2f} ms")  # noqa: E501
   atexit.register(print_globalcounters)
 
+def save_graph(G, fn, opt=""):
+  print("saving", G, f"to {fn}.svg")
+  nx.drawing.nx_pydot.write_dot(G, f'{fn}.dot')
+  os.system(f'dot {opt} -Tsvg {fn}.dot -o {fn}.svg')
+
 G:Any = None
 def init_graph():
   global G
   if G is not None: return
-  import networkx as nx
   G = nx.DiGraph()
-  def save_graph_exit():
-    print("saving", G, f"to {GRAPHPATH}.svg")
-    nx.drawing.nx_pydot.write_dot(G, f'{GRAPHPATH}.dot')
-    # -Gnslimit=100 can make it finish, but you won't like results
-    os.system(f'dot -Tsvg {GRAPHPATH}.dot -o {GRAPHPATH}.svg')
-  atexit.register(save_graph_exit)
+  atexit.register(functools.partial(save_graph, G, GRAPHPATH)) # -Gnslimit=100 can make it finish, but you won't like results
 
 counts: DefaultDict[type, int] = defaultdict(int)
 def nm(x):
   if not hasattr(x, 'node_id'):
     setattr(x, 'node_id', counts[type(x)])
     counts[type(x)] += 1
   return x.node_id
 
-def get_sop(op: List[Op]):
-  op = [x for x in op if x not in BufferOps]
-  if len(op) <= 2: return '.'.join([str(y).split(".")[1] for y in op][::-1])
-  if len(op) <= 6: return '.'.join([str(y).split(".")[1][0:3] for y in op][::-1])
-  return str(len(op))
-
-def str_dtype(dtyp):
-  ret = str(dtyp)[7:]
-  return "" if ret == 'float' else f"\n{ret}"
-
-def realized_lazybuffer(lb, num):
-  if GRAPH:
-    init_graph()
-    G.nodes[nm(lb)]['style'] = '"filled,bold"'
-    G.nodes[nm(lb)]['fillcolor'] = G.nodes[nm(lb)]['fillcolor'][:-2]
-    G.nodes[nm(lb)]['label'] = '"' + G.nodes[nm(lb)]["label"].replace('"', '') + f'\nK:{num} b:{nm(lb.realized)}"'
-
-def log_lazybuffer(lb, scheduled=False):
-  top_colors = {LoadOps: '#FFFFa0', UnaryOps: "#c0c0c0", ReduceOps: "#FFA0A0", BinaryOps: "#c0c0c0",
-                MovementOps: "#80ff80", TernaryOps: "#c0c0c0", BufferOps: '#a0a0ff'}
-  if GRAPH:
-    init_graph()
-    if lb.base != lb:
-      offset = lb.st.expr_node(NumNode(0))[0]
-      label = f"{lb.st.shape}\n{lb.st.real_strides()}" + (f"\n{offset}" if offset != 0 else "")
-      G.add_node(nm(lb), style='"filled,dashed"', fillcolor="#80ff8080", color="black", label=label)
-      G.add_edge(nm(lb.base), nm(lb), color='#00000060')
-      lb = lb.base
-    if lb.realized is None:
-      for x in lb.srcs:
-        if nm(x) not in G.nodes: log_lazybuffer(x)
+def realized_lazybuffer(lb:'LazyBuffer', num):
+  init_graph()
+  G.nodes[nm(lb)]['style'] = '"filled,bold"'
+  G.nodes[nm(lb)]['fillcolor'] = G.nodes[nm(lb)]['fillcolor'][:-2]
+  G.nodes[nm(lb)]['label'] = '"' + G.nodes[nm(lb)]["label"].replace('"', '') + f'\nK:{num}"'
+
+top_colors = {LoadOps: '#FFFFa0', UnaryOps: "#c0c0c0", ReduceOps: "#FFA0A0", BinaryOps: "#c0c0c0",
+              TernaryOps: "#c0c0c0", BufferOps: '#a0a0ff'}
+def log_lazybuffer(lb:'LazyBuffer', scheduled=False):
+  init_graph()
+  if lb.base.realized is None and lb.base.op is LoadOps.CONST: return
+  if lb.base != lb:
+    offset = lb.st.expr_idxs([NumNode(0)] * len(lb.st.shape))[0]
+    label = f"{lb.st.shape}\n{lb.st.real_strides()}" + (f"\n{offset}" if offset != 0 else "")
+    G.add_node(nm(lb), style='"filled,dashed"', fillcolor="#80ff8080", color="black", label=label)
+    G.add_edge(nm(lb.base), nm(lb), color='#00000060')
+    lb = lb.base
+  if lb.realized is None:
+    label_append = []
+    for idx,x in enumerate(lb.srcs):
+      if nm(x) not in G.nodes: log_lazybuffer(x)
+      if x.base.realized is None and x.base.op is LoadOps.CONST:
+        label_append.append(f"\nCONST{idx} {x.base.arg}")
+      else:
         G.add_edge(nm(x), nm(lb), color='#a0a0a0')
-      label = '"' + \
-        (str(set(x.shape for x in lb.srcs))+"\n"+str(lb.shape) if lb.op in ReduceOps else str(lb.shape)) + \
-        str_dtype(lb.dtype)+f"\n{lb.op}"+(f"\n{lb.arg}" if lb.op in {LoadOps.CONST, UnaryOps.CAST} else "") + \
-        (f"\n{lb.device}" if lb.device != Device.DEFAULT else "") + '"'
-      G.add_node(nm(lb), style='"filled,dashed"', fillcolor=[v for k,v in top_colors.items() if lb.op in k][0] + "80", color="black", label=label)
-      if scheduled: G.nodes[nm(lb)]['shape'] = 'box'
-    else:
-      if nm(lb) not in G.nodes:
-        # realized but unseen?
-        G.add_node(nm(lb), label=f'"{str(lb.base.realized)[5:-1].replace(" ", chr(10))}\nb:{nm(lb.realized)}"', style='filled', fillcolor="#f0c08080")
+    label = '"' + \
+      (str(set(x.shape for x in lb.srcs))+"\n"+str(lb.shape) if lb.op in ReduceOps else str(lb.shape)) + \
+      (f"\n{lb.dtype.name}" if lb.dtype.name != "float" else "")+f"\n{lb.op}"+(f"\n{lb.arg}" if lb.op in {LoadOps.CONST, UnaryOps.CAST} else "") + \
+      (f"\n{lb.device}" if lb.device != Device.DEFAULT else "") + ''.join(label_append) + '"'
+    G.add_node(nm(lb), style='"filled,dashed"', fillcolor=[v for k,v in top_colors.items() if lb.op in k][0] + "80", color="black", label=label)
+    if scheduled: G.nodes[nm(lb)]['shape'] = 'box'
+  else:
+    if nm(lb) not in G.nodes:
+      # realized but unseen?
+      G.add_node(nm(lb), label=f'"{str(lb.base.realized)[5:-1].replace(" ", chr(10))}\nb:{nm(lb.realized)}"', style='filled', fillcolor="#f0c08080")
 
-def _tree(lazydata, cycles, cnt, prefix=""):
+def _tree(lazyop:LazyOp, cycles, cnt, prefix=""):
   cnt[0] += 1
-  if len(lazydata.src) == 0: return [f"━━ {prefix}{lazydata.op.name} {lazydata.arg if lazydata.arg else ''}"]
-  if (lid := id(lazydata)) in cycles and cycles[lid][1] > (tcnt := getenv("TREE_CYCLE_CNT", 5)) and tcnt >= 0:
-    return [f"━⬆︎ goto {cycles[id(lazydata)][0]}: {lazydata.op.name}"]
+  if len(lazyop.src) == 0: return [f"━━ {prefix}{lazyop.op.name} {lazyop.arg if lazyop.arg else ''}"]
+  if (lid := id(lazyop)) in cycles and cycles[lid][1] > (tcnt := getenv("TREE_CYCLE_CNT", 5)) and tcnt >= 0:
+    return [f"━⬆︎ goto {cycles[id(lazyop)][0]}: {lazyop.op.name}"]
   cycles[lid] = (cnt[0], 1 if lid not in cycles else cycles[lid][1]+1)
-  lines = [f"━┳ {prefix}{lazydata.op.name} {lazydata.arg if lazydata.arg else ''}"]
-  childs = [_tree(c, cycles, cnt) for c in lazydata.src[:]]
+  lines = [f"━┳ {prefix}{lazyop.op.name} {lazyop.arg if lazyop.arg else ''}"]
+  childs = [_tree(c, cycles, cnt) for c in lazyop.src[:]]
   for c in childs[:-1]: lines += [f" ┣{c[0]}"] + [f" ┃{l}" for l in c[1:]]
   return lines + [" ┗"+childs[-1][0]] + ["  "+l for l in childs[-1][1:]]
 
-def print_tree(lazydata:LazyOp): print("\n".join([f"{str(i).rjust(3)} {s}" for i,s in enumerate(_tree(lazydata, {}, [-1]))]))
+def print_tree(lazyop:LazyOp): print("\n".join([f"{str(i).rjust(3)} {s}" for i,s in enumerate(_tree(lazyop, {}, [-1]))]))
 
 def graph_uops(uops:List[UOp]):
-  import networkx as nx
   colors = {UOps.ALU: "#ffffc0", UOps.LOAD: "#ffc0c0", UOps.STORE: "#c0ffc0", UOps.SPECIAL: "#c0c0ff", UOps.CONST: "#e0e0e0",
             UOps.DEFINE_GLOBAL: "#ffe0b0", UOps.DEFINE_LOCAL: "#ffe0d0", UOps.DEFINE_ACC: "#f0ffe0",
-            UOps.LOOP: "#c8a0e0", UOps.PHI: "#e0ffc0", UOps.BARRIER: "#ff8080", UOps.IF: "#c8b0c0"}
+            UOps.RANGE: "#c8a0e0", UOps.PHI: "#e0ffc0", UOps.BARRIER: "#ff8080", UOps.IF: "#c8b0c0"}
   G = nx.DiGraph()
   for u in uops:
-    if u.uop == UOps.END: continue
+    if u.uop in {UOps.ENDRANGE, UOps.ENDIF}: continue
     G.add_node(uops.index(u), label=f"{str(u.uop)[5:]}{(' '+str(u.arg)) if u.arg is not None else ''}\n{str(u.dtype)}", style="filled", fillcolor=colors.get(u.uop, "#ffffff"))  # noqa: E501
     for v in u.vin: G.add_edge(uops.index(v), uops.index(u))
-  nx.drawing.nx_pydot.write_dot(G, f'{GRAPHPATH}.uops.dot')
-  os.system(f'dot -Grankdir=LR -Tsvg {GRAPHPATH}.uops.dot -o {GRAPHPATH}.uops.svg')
+  save_graph(G, f'{GRAPHPATH}.uops', '-Grankdir=LR')
```

### Comparing `tinygrad-0.8.0/tinygrad/helpers.py` & `tinygrad-0.9.0/tinygrad/helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 from __future__ import annotations
 import os, functools, platform, time, re, contextlib, operator, hashlib, pickle, sqlite3, cProfile, pstats, tempfile, pathlib, string, ctypes
-from urllib import request  # NOTE: this has to be imported specifically
+import itertools, urllib.request, subprocess
 from tqdm import tqdm
 from typing import Dict, Tuple, Union, List, ClassVar, Optional, Iterable, Any, TypeVar, TYPE_CHECKING, Callable, Sequence
 if TYPE_CHECKING:  # TODO: remove this and import TypeGuard from typing once minimum python supported version is 3.10
   from typing_extensions import TypeGuard
+  from tinygrad.shape.shapetracker import sint
 
 T = TypeVar("T")
 U = TypeVar("U")
 # NOTE: it returns int 1 if x is empty regardless of the type of x
-def prod(x:Iterable[T]) -> Union[T,int]: return functools.reduce(operator.__mul__, x, 1)
+def prod(x:Iterable[T]) -> Union[T,int]: return functools.reduce(operator.mul, x, 1)
 
 # NOTE: helpers is not allowed to import from anything else in tinygrad
 OSX = platform.system() == "Darwin"
 CI = os.getenv("CI", "") != ""
 
 def dedup(x:Iterable[T]): return list(dict.fromkeys(x))   # retains list order
-def argfix(*x): return tuple(x[0]) if x and x[0].__class__ in (tuple, list) else x
+def argfix(*x):
+  if x and x[0].__class__ in (tuple, list):
+    if len(x) != 1: raise ValueError(f"bad arg {x}")
+    return tuple(x[0])
+  return x
 def argsort(x): return type(x)(sorted(range(len(x)), key=x.__getitem__)) # https://stackoverflow.com/questions/3382352/equivalent-of-numpy-argsort-in-basic-python
 def all_same(items:List[T]): return all(x == items[0] for x in items)
 def all_int(t: Sequence[Any]) -> TypeGuard[Tuple[int, ...]]: return all(isinstance(s, int) for s in t)
 def colored(st, color:Optional[str], background=False): return f"\u001b[{10*background+60*(color.upper() == color)+30+['black', 'red', 'green', 'yellow', 'blue', 'magenta', 'cyan', 'white'].index(color.lower())}m{st}\u001b[0m" if color is not None else st  # replace the termcolor library with one line  # noqa: E501
 def ansistrip(s:str): return re.sub('\x1b\\[(K|.*?m)', '', s)
 def ansilen(s:str): return len(ansistrip(s))
 def make_pair(x:Union[int, Tuple[int, ...]], cnt=2) -> Tuple[int, ...]: return (x,)*cnt if isinstance(x, int) else x
@@ -47,115 +52,160 @@
 def get_child(obj, key):
   for k in key.split('.'):
     if k.isnumeric(): obj = obj[int(k)]
     elif isinstance(obj, dict): obj = obj[k]
     else: obj = getattr(obj, k)
   return obj
 
+# returns the axes to create new_shape if new_shape can be created by combining axis from old_shape
+def get_contraction(old_shape:Tuple[sint, ...], new_shape:Tuple[sint, ...]) -> Optional[List[List[int]]]:
+  acc_old, acc_new = list(itertools.accumulate(old_shape, operator.mul)), list(itertools.accumulate(new_shape, operator.mul))
+  try: split = [acc_old.index(acc)+1 if acc != 1 else 0 for acc in acc_new]
+  except ValueError: return None
+  return [list(range(st,ed)) for st,ed in zip([0]+split[:-1], split[:-1]+[len(old_shape)])]
+
 @functools.lru_cache(maxsize=None)
 def to_function_name(s:str): return ''.join([c if c in (string.ascii_letters+string.digits+'_') else f'{ord(c):02X}' for c in ansistrip(s)])
 @functools.lru_cache(maxsize=None)
 def getenv(key:str, default=0): return type(default)(os.getenv(key, default))
 def temp(x:str) -> str: return (pathlib.Path(tempfile.gettempdir()) / x).as_posix()
 
+class GraphException(Exception): pass
+
 class Context(contextlib.ContextDecorator):
   stack: ClassVar[List[dict[str, int]]] = [{}]
   def __init__(self, **kwargs): self.kwargs = kwargs
   def __enter__(self):
     Context.stack[-1] = {k:o.value for k,o in ContextVar._cache.items()} # Store current state.
     for k,v in self.kwargs.items(): ContextVar._cache[k].value = v # Update to new temporary state.
     Context.stack.append(self.kwargs) # Store the temporary state so we know what to undo later.
   def __exit__(self, *args):
     for k in Context.stack.pop(): ContextVar._cache[k].value = Context.stack[-1].get(k, ContextVar._cache[k].value)
 
 class ContextVar:
   _cache: ClassVar[Dict[str, ContextVar]] = {}
   value: int
+  key: str
   def __new__(cls, key, default_value):
     if key in ContextVar._cache: return ContextVar._cache[key]
     instance = ContextVar._cache[key] = super().__new__(cls)
-    instance.value = getenv(key, default_value)
+    instance.value, instance.key = getenv(key, default_value), key
     return instance
   def __bool__(self): return bool(self.value)
   def __ge__(self, x): return self.value >= x
   def __gt__(self, x): return self.value > x
   def __lt__(self, x): return self.value < x
 
-DEBUG, IMAGE, BEAM, NOOPT = ContextVar("DEBUG", 0), ContextVar("IMAGE", 0), ContextVar("BEAM", 0), ContextVar("NOOPT", 0)
-GRAPH, GRAPHPATH = ContextVar("GRAPH", 0), getenv("GRAPHPATH", "/tmp/net")
+DEBUG, IMAGE, BEAM, NOOPT, JIT = ContextVar("DEBUG", 0), ContextVar("IMAGE", 0), ContextVar("BEAM", 0), ContextVar("NOOPT", 0), ContextVar("JIT", 1)
+WINO, THREEFRY, CACHECOLLECTING = ContextVar("WINO", 0), ContextVar("THREEFRY", 0), ContextVar("CACHECOLLECTING", 1)
+GRAPH, GRAPHPATH, SAVE_SCHEDULE, RING = ContextVar("GRAPH", 0), getenv("GRAPHPATH", "/tmp/net"), ContextVar("SAVE_SCHEDULE", 0), ContextVar("RING", 1)
+MULTIOUTPUT = ContextVar("MULTIOUTPUT", 1)
+
+# **************** global state Counters ****************
+
+class GlobalCounters:
+  global_ops: ClassVar[int] = 0
+  global_mem: ClassVar[int] = 0
+  time_sum_s: ClassVar[float] = 0.0
+  kernel_count: ClassVar[int] = 0
+  mem_used: ClassVar[int] = 0   # NOTE: this is not reset
+  @staticmethod
+  def reset(): GlobalCounters.global_ops, GlobalCounters.global_mem, GlobalCounters.time_sum_s, GlobalCounters.kernel_count = 0,0,0.0,0
+
+# **************** timer and profiler ****************
 
 class Timing(contextlib.ContextDecorator):
   def __init__(self, prefix="", on_exit=None, enabled=True): self.prefix, self.on_exit, self.enabled = prefix, on_exit, enabled
   def __enter__(self): self.st = time.perf_counter_ns()
   def __exit__(self, *exc):
     self.et = time.perf_counter_ns() - self.st
     if self.enabled: print(f"{self.prefix}{self.et*1e-6:6.2f} ms"+(self.on_exit(self.et) if self.on_exit else ""))
 
+def _format_fcn(fcn): return f"{fcn[0]}:{fcn[1]}:{fcn[2]}"
 class Profiling(contextlib.ContextDecorator):
-  def __init__(self, enabled=True, sort='cumtime', frac=0.2, fn=None): self.enabled, self.sort, self.frac, self.fn = enabled, sort, frac, fn
+  def __init__(self, enabled=True, sort='cumtime', frac=0.2, fn=None, ts=1):
+    self.enabled, self.sort, self.frac, self.fn, self.time_scale = enabled, sort, frac, fn, 1e3/ts
   def __enter__(self):
-    self.pr = cProfile.Profile(timer=lambda: int(time.time()*1e9), timeunit=1e-6)
+    self.pr = cProfile.Profile()
     if self.enabled: self.pr.enable()
   def __exit__(self, *exc):
     if self.enabled:
       self.pr.disable()
       if self.fn: self.pr.dump_stats(self.fn)
-      pstats.Stats(self.pr).strip_dirs().sort_stats(self.sort).print_stats(self.frac)
+      stats = pstats.Stats(self.pr).strip_dirs().sort_stats(self.sort)
+      for fcn in stats.fcn_list[0:int(len(stats.fcn_list)*self.frac)]:    # type: ignore[attr-defined]
+        (_primitive_calls, num_calls, tottime, cumtime, callers) = stats.stats[fcn]    # type: ignore[attr-defined]
+        scallers = sorted(callers.items(), key=lambda x: -x[1][2])
+        print(f"n:{num_calls:8d}  tm:{tottime*self.time_scale:7.2f}ms  tot:{cumtime*self.time_scale:7.2f}ms",
+              colored(_format_fcn(fcn), "yellow") + " "*(50-len(_format_fcn(fcn))),
+              colored(f"<- {(scallers[0][1][2]/tottime)*100:3.0f}% {_format_fcn(scallers[0][0])}", "BLACK") if len(scallers) else '')
 
 # *** universal database cache ***
 
 _cache_dir: str = getenv("XDG_CACHE_HOME", os.path.expanduser("~/Library/Caches" if OSX else "~/.cache"))
 CACHEDB: str = getenv("CACHEDB", os.path.abspath(os.path.join(_cache_dir, "tinygrad", "cache.db")))
 CACHELEVEL = getenv("CACHELEVEL", 2)
 
-VERSION = 10
+VERSION = 16
 _db_connection = None
 def db_connection():
   global _db_connection
   if _db_connection is None:
     os.makedirs(CACHEDB.rsplit(os.sep, 1)[0], exist_ok=True)
     _db_connection = sqlite3.connect(CACHEDB)
     if DEBUG >= 7: _db_connection.set_trace_callback(print)
   return _db_connection
 
+def diskcache_clear():
+  cur = db_connection().cursor()
+  drop_tables = cur.execute("SELECT 'DROP TABLE IF EXISTS ' || quote(name) || ';' FROM sqlite_master WHERE type = 'table';").fetchall()
+  cur.executescript("\n".join([s[0] for s in drop_tables]))
+
 def diskcache_get(table:str, key:Union[Dict, str, int]) -> Any:
   if CACHELEVEL == 0: return None
   if isinstance(key, (str,int)): key = {"key": key}
   conn = db_connection()
   cur = conn.cursor()
   try:
-    res = cur.execute(f"SELECT val FROM {table}_{VERSION} WHERE {' AND '.join([f'{x}=?' for x in key.keys()])}", tuple(key.values()))
+    res = cur.execute(f"SELECT val FROM '{table}_{VERSION}' WHERE {' AND '.join([f'{x}=?' for x in key.keys()])}", tuple(key.values()))
   except sqlite3.OperationalError:
     return None  # table doesn't exist
   if (val:=res.fetchone()) is not None: return pickle.loads(val[0])
   return None
 
 _db_tables = set()
 def diskcache_put(table:str, key:Union[Dict, str, int], val:Any):
   if CACHELEVEL == 0: return val
   if isinstance(key, (str,int)): key = {"key": key}
   conn = db_connection()
   cur = conn.cursor()
   if table not in _db_tables:
     TYPES = {str: "text", bool: "integer", int: "integer", float: "numeric", bytes: "blob"}
     ltypes = ', '.join(f"{k} {TYPES[type(key[k])]}" for k in key.keys())
-    cur.execute(f"CREATE TABLE IF NOT EXISTS {table}_{VERSION} ({ltypes}, val blob, PRIMARY KEY ({', '.join(key.keys())}))")
+    cur.execute(f"CREATE TABLE IF NOT EXISTS '{table}_{VERSION}' ({ltypes}, val blob, PRIMARY KEY ({', '.join(key.keys())}))")
     _db_tables.add(table)
-  cur.execute(f"REPLACE INTO {table}_{VERSION} ({', '.join(key.keys())}, val) VALUES ({', '.join(['?']*len(key.keys()))}, ?)", tuple(key.values()) + (pickle.dumps(val), ))  # noqa: E501
+  cur.execute(f"REPLACE INTO '{table}_{VERSION}' ({', '.join(key.keys())}, val) VALUES ({', '.join(['?']*len(key.keys()))}, ?)", tuple(key.values()) + (pickle.dumps(val), ))  # noqa: E501
   conn.commit()
   cur.close()
   return val
 
+def diskcache(func):
+  def wrapper(*args, **kwargs) -> bytes:
+    table, key = f"cache_{func.__name__}", hashlib.sha256(pickle.dumps((args, kwargs))).hexdigest()
+    if (ret:=diskcache_get(table, key)): return ret
+    return diskcache_put(table, key, func(*args, **kwargs))
+  return wrapper
+
 # *** http support ***
 
 def fetch(url:str, name:Optional[Union[pathlib.Path, str]]=None, allow_caching=not getenv("DISABLE_HTTP_CACHE")) -> pathlib.Path:
   if url.startswith(("/", ".")): return pathlib.Path(url)
   fp = pathlib.Path(name) if name is not None and (isinstance(name, pathlib.Path) or '/' in name) else pathlib.Path(_cache_dir) / "tinygrad" / "downloads" / (name if name else hashlib.md5(url.encode('utf-8')).hexdigest())  # noqa: E501
   if not fp.is_file() or not allow_caching:
-    with request.urlopen(url, timeout=10) as r:
+    with urllib.request.urlopen(url, timeout=10) as r:
       assert r.status == 200
       total_length = int(r.headers.get('content-length', 0))
       progress_bar = tqdm(total=total_length, unit='B', unit_scale=True, desc=url)
       (path := fp.parent).mkdir(parents=True, exist_ok=True)
       with tempfile.NamedTemporaryFile(dir=path, delete=False) as f:
         while chunk := r.read(16384): progress_bar.update(f.write(chunk))
         f.close()
@@ -166,47 +216,26 @@
 # *** Exec helpers
 
 def cpu_time_execution(cb, enable):
   if enable: st = time.perf_counter()
   cb()
   if enable: return time.perf_counter()-st
 
+def cpu_objdump(lib):
+  with tempfile.NamedTemporaryFile(delete=True) as f:
+    pathlib.Path(f.name).write_bytes(lib)
+    print(subprocess.check_output(['objdump', '-d', f.name]).decode('utf-8'))
+
 # *** ctypes helpers
 
 # TODO: make this work with read only memoryviews (if possible)
-def from_mv(mv:memoryview, to_type=ctypes.c_char): return ctypes.cast(ctypes.addressof(to_type.from_buffer(mv)), ctypes.POINTER(to_type))
+def from_mv(mv:memoryview, to_type=ctypes.c_char):
+  return ctypes.cast(ctypes.addressof(to_type.from_buffer(mv)), ctypes.POINTER(to_type * len(mv))).contents
 def to_mv(ptr, sz) -> memoryview: return memoryview(ctypes.cast(ptr, ctypes.POINTER(ctypes.c_uint8 * sz)).contents).cast("B")
 def to_char_p_p(options: List[bytes], to_type=ctypes.c_char): return (ctypes.POINTER(to_type) * len(options))(*[ctypes.cast(ctypes.create_string_buffer(o), ctypes.POINTER(to_type)) for o in options])  # noqa: E501
 @functools.lru_cache(maxsize=None)
 def init_c_struct_t(fields: Tuple[Tuple[str, ctypes._SimpleCData], ...]):
   class CStruct(ctypes.Structure):
     _pack_, _fields_ = 1, fields
   return CStruct
 def init_c_var(ctypes_var, creat_cb): return (creat_cb(ctypes_var), ctypes_var)[1]
-def get_bytes(arg, get_sz, get_str, check) -> bytes: return (sz := init_c_var(ctypes.c_size_t(), lambda x: check(get_sz(arg, ctypes.byref(x)))), ctypes.string_at(init_c_var(ctypes.create_string_buffer(sz.value), lambda x: check(get_str(arg, x))), size=sz.value))[1]  # noqa: E501
-def flat_mv(mv:memoryview):
-  if len(mv) == 0: return mv
-  return mv.cast("B", shape=(mv.nbytes,))
-
-# *** Helpers for CUDA-like APIs.
-
-def compile_cuda_style(prg, compile_options, prog_t, create_prog, compile_prog, get_code, get_code_size, get_log, get_log_size, check) -> bytes:
-  check(create_prog(ctypes.byref(prog := prog_t()), prg.encode(), "<null>".encode(), 0, None, None))
-  status = compile_prog(prog, len(compile_options), to_char_p_p([o.encode() for o in compile_options]))
-
-  if status != 0: raise RuntimeError(f"compile failed: {get_bytes(prog, get_log_size, get_log, check).decode()}")
-  return get_bytes(prog, get_code_size, get_code, check)
-
-def encode_args_cuda_style(bufs, vals, device_ptr_t, marks) -> Tuple[ctypes.Array, ctypes.Structure]:
-  c_args = init_c_struct_t(tuple([(f'f{i}', device_ptr_t) for i in range(len(bufs))] + [(f'f{i}', ctypes.c_int) for i in range(len(bufs), len(bufs)+len(vals))]))(*bufs, *vals)  # noqa: E501
-  return (ctypes.c_void_p * 5)(ctypes.c_void_p(marks[0]), ctypes.cast(ctypes.pointer(c_args), ctypes.c_void_p), ctypes.c_void_p(marks[1]), ctypes.cast(ctypes.pointer(ctypes.c_size_t(ctypes.sizeof(c_args))), ctypes.c_void_p), ctypes.c_void_p(marks[2])), c_args  # noqa: E501
-
-def time_execution_cuda_style(cb, ev_t, evcreate, evrecord, evsync, evdestroy, evtime, enable=False) -> Optional[float]:
-  if not enable: return cb()
-  evs = [init_c_var(ev_t(), lambda x: evcreate(ctypes.byref(x), 0)) for _ in range(2)]
-  evrecord(evs[0], None)
-  cb()
-  evrecord(evs[1], None)
-  evsync(evs[1])
-  evtime(ctypes.byref(ret := ctypes.c_float()), evs[0], evs[1])
-  for ev in evs: evdestroy(ev)
-  return ret.value * 1e-3
+def flat_mv(mv:memoryview): return mv if len(mv) == 0 else mv.cast("B", shape=(mv.nbytes,))
```

### Comparing `tinygrad-0.8.0/tinygrad/lazy.py` & `tinygrad-0.9.0/tinygrad/engine/schedule.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,319 +1,362 @@
-from __future__ import annotations
-import sys, math
-import numpy as np
-from collections import defaultdict
-from typing import Union, Optional, Any, Tuple, List, Set, Dict, DefaultDict
-from tinygrad.dtype import dtypes, DType, ImageDType
-from tinygrad.helpers import prod, merge_dicts, flatten, getenv, dedup, DEBUG, all_int, all_same
-from tinygrad.ops import LoadOps, UnaryOps, BinaryOps, TernaryOps, ReduceOps, BufferOps, Op, LazyOp, ConstBuffer, MemBuffer, ScheduleItem
-from tinygrad.shape.symbolic import sint, Variable
+import sys, pickle, atexit
+from collections import defaultdict, deque
+from dataclasses import dataclass
+from typing import Tuple, List, Dict, Optional, Set, DefaultDict, Union
+from tinygrad.ops import LoadOps, BufferOps, LazyOp, ReduceOps, ConstBuffer, MemBuffer, UNSAFE_PAD_OPS, UnaryOps
+from tinygrad.engine.graph import log_lazybuffer, realized_lazybuffer
+from tinygrad.helpers import GRAPH, DEBUG, MULTIOUTPUT, SAVE_SCHEDULE, GlobalCounters, prod, dedup, all_int, merge_dicts, getenv
+from tinygrad.shape.symbolic import Variable
+from tinygrad.dtype import ImageDType, dtypes, DType
+from tinygrad.lazy import LazyBuffer
 from tinygrad.shape.shapetracker import ShapeTracker
-from tinygrad.device import Buffer, Device
-from tinygrad.graph import log_lazybuffer
-from weakref import ref, WeakValueDictionary, ReferenceType
+from tinygrad.device import Buffer
 
-# lazy can recurse a lot
+# creation can recurse a lot
 sys.setrecursionlimit(10000)
 
-lazycache: WeakValueDictionary = WeakValueDictionary()
-def create_lazybuffer(device:str, st:ShapeTracker, dtype:DType,
-                      op:Optional[Op]=None, arg:Any=None, srcs:Tuple[LazyBuffer, ...]=(),
-                      base:Optional[LazyBuffer]=None):
-  if 0 in st.shape: st, op, arg, srcs = ShapeTracker.from_shape(st.shape), LoadOps.CONST, 0, ()
-
-  wop = (device, st, dtype, op, arg, tuple(ref(x) for x in srcs), ref(base) if base else None)
-  if wop in lazycache: return lazycache[wop]
-
-  ret = LazyBuffer(device, st, dtype, op, arg, srcs, base=base)
-  # TODO: remove LoadOps.CONST here while keeping a pretty graph and working fusions
-  # TODO: might be possible to remove LoadOps.COPY
-  if op not in {LoadOps.EMPTY, LoadOps.CUSTOM, LoadOps.CONST, LoadOps.COPY} and getenv("LAZYCACHE", 1): lazycache[wop] = ret
-  return ret
-
-class LazyBuffer:
-  def __init__(self, device:str, st:ShapeTracker, dtype:DType,
-               op:Optional[Op]=None, arg:Any=None, srcs:Tuple[LazyBuffer, ...]=(),
-               base:Optional[LazyBuffer]=None):
-    assert isinstance(device, str) and device == Device.canonicalize(device)
-    self.device, self.st, self.dtype, self.shape, self.size = device, st, dtype, st.shape, st.size
-    if base is None:
-      # properties on base
-      self.op, self.arg, self.srcs = op, arg, srcs  # this is a LazyOp, except the src is LazyBuffers and not LazyOps
-      self.realized: Optional[Buffer] = None
-      self.output_buffer: Optional[Buffer] = None
-      self.forced_realize = False
-      self.contiguous_child: Optional[Tuple[ReferenceType[LazyBuffer], ShapeTracker]] = None
-    else:
-      # properties on view
-      assert base.base == base, "base must be a base itself"
-      self._base = base
+# optionally log the ops to disk
+logops = open(getenv("LOGOPS", ""), "a") if getenv("LOGOPS", "") else None
 
-  def __repr__(self) -> str:
-    return f"<LB {self.device} {self.shape} contig:{self.st.contiguous} {self.st if hasattr(self, '_base') else (self.op, self.realized)}>"
+# *** ScheduleItem return type ***
 
+@dataclass(frozen=True)
+class ScheduleItem:
+  ast: Tuple[LazyOp, ...]
+  bufs: Tuple[Buffer, ...]
   @property
-  def base(self) -> LazyBuffer: return self._base if hasattr(self, '_base') else self
-
-  @staticmethod
-  def loadop(op, shape:Tuple[sint,...], dtype:DType, device:str, arg=None, src:Optional[LazyBuffer]=None) -> LazyBuffer:
-    return create_lazybuffer(device, ShapeTracker.from_shape(shape), dtype, op, arg, (src,) if src is not None else ())
-
-  def const(self, val:Union[float, int]) -> LazyBuffer:
-    return LazyBuffer.loadop(LoadOps.CONST, tuple(), self.dtype, self.device, arg=val).reshape((1,)*len(self.shape)).expand(self.shape)
-
-  def contiguous(self):
-    if not self.st.contiguous or self.size != self.base.size or self.is_unrealized_const():
-      ret = self.e(LoadOps.CONTIGUOUS)
-      sti = self.st.invert(self.base.shape)
-      if sti is not None: self.base.contiguous_child = ref(ret), sti
-      return ret
-    self.base.forced_realize = True
-    return self
-
-  def cast(self, dtype:DType, bitcast:bool=False):
-    if self.dtype == dtype: return self
-    return create_lazybuffer(self.device, ShapeTracker.from_shape(self.shape), dtype, UnaryOps.CAST, (dtype, bitcast), (self,))
-
-  def is_unrealized_const(self): return not self.base.realized and self.base.op == LoadOps.CONST
-  def is_unrealized_contiguous_const(self): return self.base == self and not self.base.realized and self.op == LoadOps.CONST
-
-  def schedule(self, seen=None): return create_schedule([self], seen)
-
-  @staticmethod
-  def fromCPU(x: np.ndarray) -> LazyBuffer:
-    ret = LazyBuffer("CPU", ShapeTracker.from_shape(x.shape), dtypes.from_np(x.dtype), op=LoadOps.EMPTY)
-    ret.realized = Buffer("CPU", prod(x.shape), dtypes.from_np(x.dtype), x.flatten())
-    return ret
-
-  def copy_to_device(self, device:str) -> LazyBuffer:
-    # no COPY
-    if self.device == device: return self
-
-    # double COPY = one COPY
-    if self.st.contiguous and self.size == self.base.size and not self.base.realized and self.base.op == LoadOps.COPY:
-      return self.base.srcs[0].copy_to_device(device).reshape(self.st.shape)
-
-    # const doesn't have to be copied (issues with disk tensor)
-    if self.is_unrealized_const():
-      return LazyBuffer.loadop(LoadOps.CONST, tuple(), self.dtype, device, arg=self.base.arg)._view(self.st)
-
-    # if it's a shrink, do the shrink before the copy with CONTIGUOUS
-    if prod(self.st.shape) < prod(self.base.st.shape):
-      return create_lazybuffer(device, ShapeTracker.from_shape(self.shape), self.dtype, LoadOps.COPY, srcs=(self.contiguous(),))
-
-    # copy the base and apply the shapetracker on the new device
-    return create_lazybuffer(device, self.base.st, self.dtype, LoadOps.COPY, srcs=(self.base,))._view(self.st)
-
-  def e(self, op:Union[LoadOps, UnaryOps, BinaryOps, TernaryOps], *in_srcs:LazyBuffer, arg:Optional[Any]=None) -> LazyBuffer:
-    srcs: List[LazyBuffer] = []
-    for s in (self,)+in_srcs:
-      if s == s.base and s.base.contiguous_child and (root:=s.base.contiguous_child[0]()) is not None:
-        srcs.append(root._view(s.base.contiguous_child[1]))
-      else:
-        srcs.append(s)
-    assert all_same(dts:=[x.dtype.scalar() for x in (srcs if op != TernaryOps.WHERE else srcs[1:])]), f"all dtypes must match {dts} on {op}"
-    assert all_same([x.shape for x in srcs]), f"all shapes must be the same {[x.shape for x in srcs]}"
-    if op == TernaryOps.WHERE: assert srcs[0].dtype == dtypes.bool, "TernaryOps.WHERE must have the first arg be bool"
-    out_dtype = srcs[-1].dtype if op not in (BinaryOps.CMPLT, BinaryOps.CMPEQ) else dtypes.bool
-    ret = create_lazybuffer(self.device, ShapeTracker.from_shape(self.shape), out_dtype, op, arg, tuple(srcs))
-    return ret
-
-  # *** reduce ops ***
-
-  def _reduce_op(self, op:ReduceOps, new_shape:Tuple[sint, ...]) -> LazyBuffer:
-    if self.shape == tuple(new_shape): return self
-    unbound_new_shape = tuple(s.unbind()[0] if not isinstance(s, int) else s for s in new_shape)
-    return create_lazybuffer(self.device, ShapeTracker.from_shape(new_shape), self.dtype, op, unbound_new_shape, (self,))
-
-  def r(self, op:ReduceOps, new_shape:Tuple[sint, ...]) -> LazyBuffer:
-    assert len(self.shape) == len(new_shape) and all(s == ns or ns == 1 for s,ns in zip(self.shape, new_shape)), \
-      f"reduce shape lens must match {self.shape} {new_shape}"
-    # TODO: can we split symbolic shape if the reduce axis is not symbolic?
-    if not all_int(self.shape) or (0 in self.shape) or prod(self.shape) // prod(new_shape) < getenv("REDUCEOP_SPLIT_THRESHOLD", 32768):
-      return self._reduce_op(op, new_shape)
-    heuristic, divisor, dim_to_split = max(((divisor := math.gcd(256, old))/(stride or math.inf), divisor, i) for i, (old, new, stride) in enumerate(zip(self.shape, new_shape, self.st.real_strides())) if old != new) # type: ignore  # noqa: E501
-    if divisor < 16 or heuristic < 0.1: return self._reduce_op(op, new_shape)
-    # choose largest divisor (>=16) to split on, penalize large strides
-    def splitted_shape(dim_aft_div):
-      return self.shape[:dim_to_split] + (self.shape[dim_to_split]//divisor,) + dim_aft_div + self.shape[dim_to_split+1:]
-    return self.reshape(splitted_shape((divisor,)))._reduce_op(op, splitted_shape((1,))).reshape(splitted_shape(()))._reduce_op(op, new_shape)
-
-  # *** movement ops ***
-
-  def _view(self, new_st:ShapeTracker) -> LazyBuffer:
-    if new_st.contiguous and self.base.shape == new_st.shape: return self.base
-    return create_lazybuffer(self.device, new_st, self.dtype, base=self.base)
-
-  def reshape(self, arg:Tuple[sint, ...]): return self._view(self.st.reshape(arg))
-  def pad(self, arg:Tuple[Tuple[sint, sint], ...]): return self._view(self.st.pad(arg))
-  def expand(self, arg:Tuple[sint, ...]): return self._view(self.st.expand(arg))
-  def permute(self, arg:Tuple[int, ...]): return self._view(self.st.permute(arg))
-  def shrink(self, arg:Tuple[Tuple[sint, sint], ...]): return self._view(self.st.shrink(arg))
-  def stride(self, arg:Tuple[int, ...]): return self._view(self.st.stride(arg))
-
-# *** schedule creation ***
-
-# recursively create a lazyop
-def _recursive_lazyop(buf:LazyBuffer, inputs:List[LazyBuffer], var_vals:Dict[Variable, int], st:ShapeTracker,
-                      realizes:Set[LazyBuffer], cache, first=True) -> LazyOp:
+  def outputs(self) -> Tuple[Buffer, ...]:
+    """Read/write or write only buffers in the schedule."""
+    return self.bufs[:len(self.ast)]
+  @property
+  def inputs(self) -> Tuple[Buffer, ...]:
+    """Read only buffers in the schedule."""
+    return self.bufs[len(self.ast):]
+
+# *** DAG transformation: List[LazyBuffer] -> ScheduleItem ***
+
+# TODO: it's unfortunate this needs to exist, but because of ASSIGN, we have to retain the LazyBuffer structure until post toposort
+@dataclass(frozen=True)
+class _LBScheduleItem:
+  ast: Tuple[LazyOp, ...]
+  outputs: Tuple[LazyBuffer, ...]
+  inputs: Tuple[LazyBuffer, ...]
+  var_vals: Dict[Variable, int]
+
+def _recursive_lazyop(buf:LazyBuffer, inputs:List[LazyBuffer], outputs:Tuple[LazyBuffer, ...], var_vals:Dict[Variable, int], st:ShapeTracker,
+                      realizes:Dict[LazyBuffer, None], assign_targets:Dict[LazyBuffer, LazyBuffer], cache) -> LazyOp:
+  """recursively create a lazyop"""
   if (buf, st) in cache: return cache[(buf, st)]
   if buf != buf.base:
     st = buf.st + st
     buf = buf.base
   # all buffers here are base now
   assert buf.op is not None
 
   # consts are always fused and generated
-  if buf.op == LoadOps.CONST:
-    # TODO: make shapetracker unbind also return var_vals
-    var_vals.update(merge_dicts([var_vals, st.var_vals]))
-    return LazyOp(BufferOps.CONST, (), ConstBuffer(float(buf.arg), buf.dtype, st.simplify().unbind()))
+  if buf.op is LoadOps.CONST:
+    unbound_st, st_var_vals = st.simplify().unbind()
+    var_vals.update(st_var_vals)
+    if isinstance(buf.arg, Variable): var_vals.__setitem__(*buf.arg.unbind())
+    return LazyOp(BufferOps.CONST, (), ConstBuffer(buf.arg, buf.dtype, unbound_st))
 
   # if we aren't fusing it, it's a load and we add it to the inputs
-  if buf.realized or (buf in realizes and not first):
+  if buf.realized is not None or (buf in realizes and buf not in outputs):
+    unbound_st, st_var_vals = st.simplify().unbind()
+    var_vals.update(st_var_vals)
+    if buf in assign_targets:
+      # can only assign to contiguous read+write buffer
+      if not unbound_st.contiguous:
+        # we also allow masked views. if it has a single view and it's equal when you shrink a contig, it's fine
+        if not (len(unbound_st.views) == 1 and unbound_st.views[0].mask is not None and
+            ShapeTracker.from_shape(unbound_st.shape).shrink(unbound_st.views[0].mask) == unbound_st.shrink(unbound_st.views[0].mask)):
+          raise RuntimeError(f"must be contiguous for assign {unbound_st}")
+      return LazyOp(BufferOps.LOAD, (), MemBuffer(outputs.index(assign_targets[buf]), buf.dtype, unbound_st))
     if buf not in inputs: inputs.append(buf)
-    var_vals.update(merge_dicts([var_vals, st.var_vals]))
-    return LazyOp(BufferOps.LOAD, (), MemBuffer(inputs.index(buf)+1, buf.dtype, st.simplify().unbind()))
+    return LazyOp(BufferOps.LOAD, (), MemBuffer(len(outputs)+inputs.index(buf), buf.dtype, unbound_st))
 
-  # if a CONTIGUOUS made it all the way here, just skip it
-  if buf.op == LoadOps.CONTIGUOUS:
-    assert first
-    return _recursive_lazyop(buf.srcs[0], inputs, var_vals, st, realizes, cache, False)
+  # if a CONTIGUOUS or ASSIGN made it all the way here, just skip it
+  if buf.op is LoadOps.CONTIGUOUS:
+    assert buf in outputs
+    return _recursive_lazyop(buf.srcs[0], inputs, outputs, var_vals, st, realizes, assign_targets, cache)
+  if buf.op is LoadOps.ASSIGN:
+    assert buf in outputs
+    assert buf.srcs[1].base is buf.srcs[1], "assign must be to base"
+    assert buf.srcs[1].realized is not None, f"assign must be already realized to schedule {buf.srcs[1]}"
+    return _recursive_lazyop(buf.srcs[0], inputs, outputs, var_vals, st, realizes, assign_targets, cache)
 
   # if it's a reduce, we have to change the shapetracker
   if buf.op in ReduceOps:
     assert st.contiguous, "ReduceOps late fusion must be contiguous"
     st = ShapeTracker.from_shape(buf.srcs[0].shape)
 
   # otherwise we fuse it like normal
-  cache[(buf, st)] = ret = LazyOp(buf.op, tuple(_recursive_lazyop(x, inputs, var_vals, st, realizes, cache, False) for x in buf.srcs), buf.arg)
+  cache[(buf, st)] = ret = \
+    LazyOp(buf.op, tuple(_recursive_lazyop(x, inputs, outputs, var_vals, st, realizes, assign_targets, cache) for x in buf.srcs), buf.arg)
   return ret
 
-# recursively walk back in the graph to create the schedule
-def _recursive_schedule(out:LazyBuffer, seen:Set[LazyBuffer], realizes:Set[LazyBuffer],
-                        reduce_for_op: Dict[LazyBuffer, LazyBuffer]) -> List[ScheduleItem]:
-  if out in seen or out.realized or out.op == LoadOps.CONST: return []
-  assert out.base == out
-  seen.add(out)
-
+def _schedule_group(outs:Tuple[LazyBuffer, ...], realizes:Dict[LazyBuffer, None], reduce_for_op: Dict[LazyBuffer, LazyBuffer]) -> _LBScheduleItem:
+  """create a schedule item from a list of outputs"""
   inputs: List[LazyBuffer] = []
-  var_vals: Dict[Variable, int] = out.st.var_vals.copy()
-  if out.op == LoadOps.COPY:
-    op, inputs = LazyOp(LoadOps.COPY, (), out.srcs[0].base), [out.srcs[0].base]
-  elif out.op == LoadOps.CUSTOM:
-    op, inputs = LazyOp(LoadOps.CUSTOM, (), out.arg), list(out.srcs)
-  elif out.op == LoadOps.EMPTY:
-    op = LazyOp(LoadOps.EMPTY)
+  ast: List[LazyOp] = []
+  var_vals: Dict[Variable, int] = merge_dicts([out.st.var_vals.copy() for out in outs])
+  # single output AST
+  if (op:=(out:=outs[0]).op) in {LoadOps.CUSTOM, LoadOps.COPY, LoadOps.EMPTY, LoadOps.VIEW}:
+    assert len(outs) == 1, f"can't schedule a group of {op}"
+    inputs = [x.base for x in out.srcs]
+    if getenv("USE_COPY_KERNEL") and op is LoadOps.COPY and out.device.split(":")[0] == out.srcs[0].device.split(":")[0]:
+      rd = LazyOp(BufferOps.LOAD, (), MemBuffer(1, dtypes.uint8, st:=ShapeTracker.from_shape((out.arg,))))
+      ast = [LazyOp(BufferOps.STORE, (rd,), MemBuffer(0, dtypes.uint8, st))]
+    else: ast = [LazyOp(op, (), out.arg)]
+  # multi output AST
   else:
-    output_st = ShapeTracker.from_shape(reduce_for_op[out].shape if out in reduce_for_op else out.shape)
-    op = _recursive_lazyop(out, inputs, var_vals, output_st, realizes, cache={})
-    op = LazyOp(BufferOps.STORE, (op, ), MemBuffer(0, out.dtype, output_st.simplify().unbind()))
-
-  return flatten(_recursive_schedule(x.base, seen, realizes, reduce_for_op) for x in inputs) + [ScheduleItem(op, out, tuple(inputs), var_vals)]
-
-# recursively search the entire graph for all LazyBuffers, insert realizes after expands
-def _recurse_lb(buf:LazyBuffer, realizes:Set[LazyBuffer], allbufs:Dict[LazyBuffer, None],
-                simple_pads:Set[LazyBuffer], children:DefaultDict[LazyBuffer, Dict[LazyBuffer, None]]):
-  if buf in allbufs or buf.base.realized: return
-  log_lazybuffer(buf)
-  if isinstance(buf.dtype, ImageDType) and (prod(buf.shape) != prod(buf.dtype.shape) or
-                                            not any(buf.shape[x]%4 == 0 for x in buf.st.unit_stride_axes())):
-    if DEBUG >= 3: print(f"forcing image {buf.dtype} with shape {buf.shape} to float32")
-    buf.dtype = dtypes.float32  # NOTE; this is what makes the dtype above not match
+    assign_targets = {x.srcs[1]:x for x in outs if x.op is LoadOps.ASSIGN}
+    for i, out in enumerate(outs):
+      output_st = ShapeTracker.from_shape(reduce_for_op[out].shape if out in reduce_for_op else out.shape)
+      output_view = out.arg[0] if out.op is LoadOps.ASSIGN and out.arg else output_st
+      lop = _recursive_lazyop(out, inputs, outs, var_vals, output_st, realizes, assign_targets, cache={})
+      output_view, vv = output_view.simplify().unbind()
+      if vv: var_vals.update(vv)
+      ast.append(LazyOp(BufferOps.STORE, (lop, ), MemBuffer(i, out.dtype, output_view)))
+  return _LBScheduleItem(tuple(ast), outs, tuple(inputs), var_vals)
+
+# *** DAG creation: decide which LazyBuffers should realize ***
+
+def _recurse_lb(buf:LazyBuffer, realizes:Dict[LazyBuffer, None], allbufs:Dict[LazyBuffer, None],
+                simple_pads:Set[LazyBuffer], children:DefaultDict[LazyBuffer, Dict[LazyBuffer, None]], scheduled=False):
+  """recursively search the entire graph for all LazyBuffers, insert realizes after expands"""
+  if buf in allbufs or buf.base.realized is not None: return
+  if GRAPH: log_lazybuffer(buf, scheduled)
+  # view
   if buf.base != buf:
-    # realize all places where the buffer is expanded
-    if prod(buf.base.st.shape) < prod(buf.st.shape):
-      if len(buf.st.views) == 1 and buf.st.views[-1].mask and all_int(buf.base.st.shape) and \
-          prod(buf.base.st.shape) == prod([y-x for x,y in buf.st.views[-1].mask]):
-        simple_pads.add(buf.base)
+    # fuse some pads
+    if len(buf.st.views) == 1 and buf.st.views[-1].mask is not None and all_int(buf.base.st.shape) and \
+        prod(buf.base.st.shape) >= prod([y-x for x,y in buf.st.views[-1].mask]):
+      simple_pads.add(buf.base)
+    # realize all expands
+    elif prod(buf.base.st.shape) < prod(buf.st.shape):
+      if buf.base.op is UnaryOps.CAST and isinstance(buf.base.srcs[0].dtype, ImageDType) and isinstance(buf.base.arg, ImageDType):
+        pass # don't realize image to image casts. this is part of a larger problem
       else:
-        realizes.add(buf.base)
+        realizes[buf.base] = None
     return _recurse_lb(buf.base, realizes, allbufs, simple_pads, children)
-  if buf.forced_realize: realizes.add(buf)
+  # base
   allbufs[buf] = None
-  if buf.op in LoadOps: realizes.add(buf.base)
-  if buf.op == LoadOps.COPY:
+  if buf.forced_realize: realizes[buf] = None
+  if buf.op in LoadOps: realizes[buf.base] = None
+  if buf.op is LoadOps.COPY:
     assert buf.srcs[0].st.contiguous and buf.srcs[0].size == buf.srcs[0].base.size, "can only copy contig"
-    realizes.add(buf.srcs[0].base)
+    realizes[buf.srcs[0].base] = None
+  if buf.op is LoadOps.VIEW: realizes[buf.srcs[0].base] = None
   for x in buf.srcs:
     children[x.base][buf] = None
     _recurse_lb(x, realizes, allbufs, simple_pads, children)
 
-UNSAFE_PAD_OPS = {BinaryOps.DIV, BinaryOps.CMPLT, BinaryOps.CMPEQ, UnaryOps.LOG2, UnaryOps.EXP2}
-def _is_padding_okay(buf:LazyBuffer, realizes:Set[LazyBuffer]) -> bool:
-  if buf in realizes or buf.realized: return True
+def _is_padding_okay(buf:LazyBuffer, realizes:Dict[LazyBuffer, None]) -> bool:
+  if buf in realizes or buf.realized is not None: return True
   # NOTE: this broke to_image_idx and coder with JIT
   if buf.op in UNSAFE_PAD_OPS: return False
   return all(_is_padding_okay(x.base, realizes) for x in buf.srcs)
 
-def create_schedule(outs:List[LazyBuffer], seen:Optional[Set[LazyBuffer]]=None) -> List[ScheduleItem]:
-  if seen is None: seen = set()
-  for out in outs: log_lazybuffer(out, scheduled=True)
-
+def _recursive_group(tr:LazyBuffer, st:ShapeTracker, r:LazyBuffer, children:DefaultDict[LazyBuffer, Dict[LazyBuffer, None]],
+                     realizes:Dict[LazyBuffer, None], reduce_for_op:Dict[LazyBuffer, LazyBuffer], group:Set[LazyBuffer]):
+  """recursively search the LazyBuffer for groupable children, realize the LazyBuffer if a child can't group"""
+  if tr in realizes:
+    # can only fuse contiguous
+    # max one reduceop per kernel
+    if not st.contiguous or st.size != r.st.size or tr in reduce_for_op: group.add(r)
+    return group.add(tr)
+  for tr_next in children[tr]:
+    if tr_next.realized is None:
+      # max one reduceop per kernel
+      if tr_next.op in ReduceOps: return group.add(r)
+      # can only fuse contiguous
+      if len(st_childs:=dedup(s for s in tr_next.srcs if s.base == tr)) > 1: return group.add(r)
+      _recursive_group(tr_next, st+st_childs[0].st, r, children, realizes, reduce_for_op, group)
+
+def _graph_schedule(outs:List[LazyBuffer], seen:Set[LazyBuffer]) -> Tuple[DefaultDict[LazyBuffer, List[LazyBuffer]], DefaultDict[LazyBuffer, int],
+                                                                    Dict[LazyBuffer, _LBScheduleItem]]:
+  """create a graph for realizing the outputs"""
   # start by just realizing the buffers passed in
-  realizes: Set[LazyBuffer] = set([x.base for x in outs if not x.base.realized])
+  realizes: Dict[LazyBuffer, None] = {x.base:None for x in outs if x.base.realized is None}
   allbufs: Dict[LazyBuffer, None] = {}
   simple_pads: Set[LazyBuffer] = set()
   children: DefaultDict[LazyBuffer, Dict[LazyBuffer, None]] = defaultdict(dict)
-  for out in outs: _recurse_lb(out.base, realizes, allbufs, simple_pads, children)
+  for out in outs: _recurse_lb(out.base, realizes, allbufs, simple_pads, children, scheduled=True)
+  assign_targets = {x.srcs[1]:x for x in realizes if x.op is LoadOps.ASSIGN and x not in seen and x.realized is None}
 
   # check if we have to realize pads
   for p in simple_pads:
     if not _is_padding_okay(p, realizes):
-      realizes.add(p)
+      realizes[p] = None
 
   # find all reduces, and pair them to a elementwise op. if they can't be cleanly paired, force realize the reduce (or a contig child)
   reduce_for_op: Dict[LazyBuffer, LazyBuffer] = {}
-  for r in allbufs.keys():
-    if r != r.base or r.op not in ReduceOps or r in realizes: continue
+  for r in allbufs:
+    if r.op not in ReduceOps or r in realizes: continue
 
-    # follow the reduce down
-    child_set: Dict[LazyBuffer, ShapeTracker] = {r: r.st}
-    realized_children: Dict[LazyBuffer, ShapeTracker] = {}
-    forced_realize = False
-    can_chase = True
-    while not forced_realize and len(child_set):
-      next_child_set = {}
-      for tr,st in child_set.items():
-        if tr in realizes:
-          realized_children[tr] = st
-          # can only have one output buffer
-          # can only reduce contiguous
-          # max one reduceop per kernel
-          if len(realized_children) > 1 or not st.contiguous or st.size != r.st.size or (tr in reduce_for_op and reduce_for_op[tr] != r):
-            can_chase = tr not in reduce_for_op or reduce_for_op[tr] == r
-            forced_realize = True
-            break
+    group: Set[LazyBuffer] = set()
+    _recursive_group(r, r.st, r, children, realizes, reduce_for_op, group)
+    # max one reduceop per kernel
+    can_chase = all(tr not in reduce_for_op for tr in group)
+    # TODO: forced_realize exists because the scheduler is incapable of checking for self-contained DAGs
+    forced_realize = r in group
+    if not forced_realize and len(group) > 1:
+      # create a multi output kernel if the LazyBufferss can cleanly group
+      rc_parents, rc_children = deque(group), deque(group)
+      while rc_parents and not forced_realize:
+        # max one reduceop per kernel
+        if (p:=rc_parents.pop()).op in ReduceOps: forced_realize = True
+        else: rc_parents.extend(x.base for x in p.srcs if x.base.realized is None and x.base is not r)
+      # search descendants of the reduceop that can cleanly group
+      realized_descendants: Set[LazyBuffer] = set()
+      while rc_children and not forced_realize:
+        if (c:=rc_children.pop()).op in ReduceOps or not c.st.contiguous or c.st.size != r.st.size or c in reduce_for_op:
+          realized_descendants.clear()
+          break
+        if c in realizes and c not in group: realized_descendants.add(c)
+        rc_children.extend(x for x in children[c] if x.realized is None and x.device == r.device)
+      group.update(realized_descendants)
+    # can only fuse assign if no other assign_target is used in the kernel
+    if not forced_realize and any(x.op is LoadOps.ASSIGN for x in group):
+      parents = deque((r, *group))
+      while parents and not forced_realize:
+        if (p:=parents.pop().base).realized or p in realizes:
+          if p in assign_targets and assign_targets[p] not in group: forced_realize, can_chase = True, False
           continue
-        for tr_next in children[tr].keys():
-          if not tr_next.realized:
-            # max one reduceop per kernel
-            if tr_next.op in ReduceOps:
-              forced_realize = True
-              break
-            st_childs = dedup([s for s in tr_next.srcs if s.base == tr])
-            if len(st_childs) > 1:
-              forced_realize = True
-              break
-            next_child_set[tr_next] = st + st_childs[0].st
-      child_set = next_child_set
+        parents.extend(p.srcs)
     if forced_realize:
       tr = r
       if can_chase:
         # can chase this down to contiguous children
         st = tr.st
         while len(children[tr]) == 1:
-          tr_next = next(iter(children[tr].keys()))
-          st_childs = dedup([s for s in tr_next.srcs if s.base == tr])
+          tr_next = next(iter(children[tr]))
+          st_childs = dedup(s for s in tr_next.srcs if s.base is tr)
           if len(st_childs) > 1: break
           if st.size != st_childs[0].st.size: break
           st = st + st_childs[0].st
           if not st.contiguous or tr_next.op in ReduceOps: break
           tr = tr_next
+        # don't cast to higher size before store (tr cannot be realized if forced_realize)
+        if tr.op is UnaryOps.CAST and tr.arg.itemsize > tr.srcs[0].dtype.itemsize:
+          tr = tr.srcs[0].base
         reduce_for_op[tr] = r
-      realizes.add(tr)
-    else:
-      assert len(realized_children) == 1
-      reduce_for_op[next(iter(realized_children.keys()))] = r
+      realizes[tr] = None
+    else: reduce_for_op.update((tr, r) for tr in group)
+
+  output_groups: DefaultDict[LazyBuffer, List[LazyBuffer]] = defaultdict(list)
+  for buf in realizes:
+    if buf.realized is not None or buf.op is LoadOps.CONST or buf in seen: continue
+    output_groups[reduce_for_op[buf] if buf in reduce_for_op and MULTIOUTPUT else buf].append(buf)
+
+    # make things that can't be images not images
+    if isinstance(buf.dtype, ImageDType) and (prod(buf.shape) != prod(buf.dtype.shape) or
+                                              not any(buf.shape[x]%4 == 0 for x in buf.st.unit_stride_axes())):
+      if DEBUG >= 2: print(f"forcing image {buf.dtype} with shape {buf.shape} to float32")
+      buf.dtype = dtypes.float32
+      # hack the underlying buffer too
+      if buf.base is buf:
+        assert not hasattr(buf.buffer, '_buf'), "can't fixup allocated buffer"
+        buf.buffer.dtype = dtypes.float32
+        buf.buffer.options = None
+
+  # preschedule all buffers in realizes
+  prescheduled = {group[0]:_schedule_group(tuple(group), realizes, reduce_for_op) for group in output_groups.values()}
+  schedule_targets = {out:ps for ps in prescheduled.values() for out in ps.outputs}
+
+  graph: DefaultDict[LazyBuffer, List[LazyBuffer]] = defaultdict(list)
+  in_degree: DefaultDict[LazyBuffer, int] = defaultdict(int)
+  for key, lsi in prescheduled.items():
+    if key not in in_degree: in_degree[key] = 0
+    # realize outputs after all parents are realized
+    scheduled_parents = set(schedule_targets[x].outputs[0] for x in lsi.inputs if x in schedule_targets)
+    for x in scheduled_parents:
+      graph[x].append(key)
+      in_degree[key] += 1
+    # realize outputs before a parent is assigned to
+    parents_assigns = set(schedule_targets[assign_targets[x]].outputs[0] for x in lsi.inputs if x in assign_targets)
+    for assign in parents_assigns:
+      graph[key].append(assign)
+      in_degree[assign] += 1
+
+  return graph, in_degree, prescheduled
+
+# *** DAG ordering: breadth first search ***
+
+SCHEDULES: List = []
+def create_schedule_with_vars(outs:List[LazyBuffer], seen:Optional[Set[LazyBuffer]]=None) -> Tuple[List[ScheduleItem], Dict[Variable, int]]:
+  if seen is None: seen = set()
+  graph, in_degree, prescheduled = _graph_schedule(outs, seen)
+  queue = deque(si for key, si in prescheduled.items() if in_degree[key] == 0)
+  schedule: List[ScheduleItem] = []
+  var_vals: Dict[Variable, int] = {}
+  kernel_number = GlobalCounters.kernel_count
+  while queue:
+    ps = queue.popleft()
+    for buf in ps.outputs: seen.add(buf)
+    if GRAPH:
+      kernel_number += 1
+      for out in ps.outputs: realized_lazybuffer(out, kernel_number)
+    var_vals = merge_dicts([var_vals, ps.var_vals])
+    for out in ps.outputs: del out.srcs  # can only schedule once
+    schedule.append(si:=ScheduleItem(ps.ast, tuple(x.buffer for x in (ps.outputs+ps.inputs) if x.size != 0)))
+    if logops and si.ast[0].op not in LoadOps and not any(i.device.startswith("DISK:") for i in si.inputs): logops.write(str(si.ast)+"\n")
+    for x in graph[ps.outputs[0]]:
+      in_degree[x] -= 1
+      if in_degree[x] == 0: queue.append(prescheduled[x])
+
+  if SAVE_SCHEDULE:
+    def _save():
+      print(f"saving {len(SCHEDULES)} schedule graphs to", fp:=getenv("SAVE_SCHEDULE_PATH", "schedule.pkl"))
+      pickle.dump(SCHEDULES, open(fp, "wb"))
+    if len(SCHEDULES) == 0: atexit.register(_save)
+    SCHEDULES.extend((ps.ast for ps in prescheduled.values()) if getenv("CAPTURE_AST") else [(graph, prescheduled)])
+  # confirm everything was scheduled correctly
+  if not all(degree == 0 for degree in in_degree.values()) or len(prescheduled) != len(schedule):
+    raise RuntimeError(f"cycle detected in graph, prescheduled {len(prescheduled)} but only scheduled {len(schedule)}")
+  if DEBUG >= 1 and len(schedule) >= 10: print(f"scheduled {len(schedule)} kernels")
+  return schedule, var_vals
+
+def create_schedule(outs:List[LazyBuffer], seen:Optional[Set[LazyBuffer]]=None) -> List[ScheduleItem]:
+  schedule, var_vals = create_schedule_with_vars(outs, seen)
+  assert len(var_vals) == 0
+  return schedule
+
+# *** memory planning ***
+
+def _internal_memory_planner(buffers:List[Union[List[Buffer], Tuple[Buffer, ...]]], debug_prefix="") -> Dict[Buffer, Buffer]:
+  if getenv("NO_MEMORY_PLANNER"): return {}
+  last_appearance = {}
+  for i,u in enumerate(buffers):
+    for buf in u: last_appearance[buf] = i
+
+  # LRU algorithm
+  assigned: Dict[Buffer, Buffer] = {}
+  local_cache: DefaultDict[Tuple[str, int, DType], List[Buffer]] = defaultdict(list)
+
+  def handle_buffer(buf):
+    key = (buf.device, buf.size, buf.dtype)
+    if buf not in assigned:
+      if len(ll:=local_cache[key]): assigned[buf] = ll.pop()
+      else: assigned[buf] = Buffer(*key)
+    if i == last_appearance[buf]:
+      if assigned[buf] not in local_cache[key]: local_cache[key].append(assigned[buf])
+
+  for i,u in enumerate(buffers):
+    for buf in u:
+      # all unallocated unparented buffers are fair game to replace
+      if buf.is_allocated() or buf.lb_refcount > 0: continue
+      # handle view buffers
+      if buf._base is not None:
+        assigned[buf] = Buffer(buf.device, buf.size, buf.dtype, base=assigned.get(buf._base, buf._base), offset=buf.offset)
+      else:
+        handle_buffer(buf)
 
-  return flatten(_recursive_schedule(x.base, seen, realizes, reduce_for_op) for x in outs)
+  if DEBUG >= 1 and len(ak:=dedup(assigned.keys())) != len(av:=dedup(assigned.values())):
+    print(debug_prefix+f"memory reduced from {sum([x.nbytes for x in ak])/1e6:.2f} MB -> {sum([x.nbytes for x in av])/1e6:.2f} MB,",
+          f"{len(ak)} -> {len(av)} bufs")
+  return assigned
+
+def memory_planner(schedule:List[ScheduleItem]) -> List[ScheduleItem]:
+  assigned = _internal_memory_planner([si.bufs for si in schedule])
+  return [ScheduleItem(si.ast, tuple(assigned.get(x, x) for x in si.bufs)) for si in schedule]
```

### Comparing `tinygrad-0.8.0/tinygrad/mlops.py` & `tinygrad-0.9.0/tinygrad/function.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+"""This is where the forwards and backwards passes live."""
 import math
 from typing import Tuple, Optional
 from tinygrad.helpers import argsort
-from tinygrad.dtype import DType
+from tinygrad.dtype import dtypes, DType, sum_acc_dtype
 from tinygrad.ops import UnaryOps, BinaryOps, TernaryOps, ReduceOps
 from tinygrad.tensor import Function
 from tinygrad.lazy import LazyBuffer
 from tinygrad.shape.symbolic import sint
 
 class Contiguous(Function):
   def forward(self, x:LazyBuffer) -> LazyBuffer: return x.contiguous()
@@ -20,22 +21,25 @@
     self.input_dtype, self.bitcast = x.dtype, bitcast
     return x.cast(dtype, bitcast)
 
   def backward(self, grad_output:LazyBuffer) -> LazyBuffer: return grad_output.cast(self.input_dtype, self.bitcast)
 
 # ************* unary ops *************
 
-class Zero(Function):
-  def forward(self, x:LazyBuffer) -> LazyBuffer: return x.const(0)
-  def backward(self, grad_output:LazyBuffer) -> LazyBuffer: return grad_output.const(0)
-
 class Neg(Function):
   def forward(self, x:LazyBuffer) -> LazyBuffer: return x.e(UnaryOps.NEG)
   def backward(self, grad_output:LazyBuffer) -> LazyBuffer: return grad_output.e(UnaryOps.NEG)
 
+class Reciprocal(Function):
+  def forward(self, x:LazyBuffer) -> LazyBuffer:
+    self.ret = x.const(1).e(BinaryOps.DIV, x)
+    return self.ret
+  def backward(self, grad_output:LazyBuffer) -> LazyBuffer:
+    return grad_output.e(UnaryOps.NEG).e(BinaryOps.MUL, self.ret).e(BinaryOps.MUL, self.ret)
+
 class Sin(Function):
   def forward(self, x:LazyBuffer) -> LazyBuffer:
     self.x = x
     return x.e(UnaryOps.SIN)
 
   def backward(self, grad_output:LazyBuffer) -> LazyBuffer:
     return self.x.const(math.pi / 2).e(BinaryOps.SUB, self.x).e(UnaryOps.SIN).e(BinaryOps.MUL, grad_output)
@@ -78,21 +82,30 @@
   def forward(self, x:LazyBuffer) -> LazyBuffer:
     self.ret = x.const(1).e(BinaryOps.DIV, x.const(1).e(BinaryOps.ADD, x.e(BinaryOps.MUL, x.const(-1/math.log(2))).e(UnaryOps.EXP2)))
     return self.ret
 
   def backward(self, grad_output:LazyBuffer) -> LazyBuffer:
     return self.ret.e(BinaryOps.MUL, self.ret.const(1).e(BinaryOps.SUB, self.ret)).e(BinaryOps.MUL, grad_output)
 
+class Sign(Function):
+  def forward(self, x:LazyBuffer) -> LazyBuffer:
+    return x.e(BinaryOps.CMPEQ, x.const(0)).e(TernaryOps.WHERE, x.const(0),
+                                              x.e(BinaryOps.CMPLT, x.const(0)).e(TernaryOps.WHERE, x.const(-1), x.const(1)))
+  # backward always return 0 to match torch
+  def backward(self, grad_output:LazyBuffer) -> LazyBuffer: return grad_output.const(0)
+
 # ************* binary ops *************
 
 class Less(Function):
   def forward(self, x:LazyBuffer, y:LazyBuffer) -> LazyBuffer: return x.e(BinaryOps.CMPLT, y)
+  def backward(self, grad_output:LazyBuffer) -> Tuple[Optional[LazyBuffer], Optional[LazyBuffer]]: return None, None
 
 class Eq(Function):
   def forward(self, x:LazyBuffer, y:LazyBuffer) -> LazyBuffer: return x.e(BinaryOps.CMPEQ, y)
+  def backward(self, grad_output:LazyBuffer) -> Tuple[Optional[LazyBuffer], Optional[LazyBuffer]]: return None, None
 
 class Xor(Function):
   def forward(self, x:LazyBuffer, y:LazyBuffer) -> LazyBuffer: return x.e(BinaryOps.XOR, y)
 
 class Add(Function):
   def forward(self, x:LazyBuffer, y:LazyBuffer) -> LazyBuffer: return x.e(BinaryOps.ADD, y)
 
@@ -136,40 +149,41 @@
     return None, \
       self.x.e(TernaryOps.WHERE, grad_output, grad_output.const(0)) if self.needs_input_grad[1] else None, \
       self.x.e(TernaryOps.WHERE, grad_output.const(0), grad_output) if self.needs_input_grad[2] else None
 
 # ************* reduce ops *************
 
 class Sum(Function):
-  def forward(self, x:LazyBuffer, new_shape:Tuple[int, ...]) -> LazyBuffer:
+  def forward(self, x:LazyBuffer, axis:Tuple[int, ...]) -> LazyBuffer:
     self.input_shape = x.shape
-    return x.r(ReduceOps.SUM, new_shape)
+    return x.r(ReduceOps.SUM, axis)
 
   def backward(self, grad_output:LazyBuffer) -> LazyBuffer: return grad_output.expand(self.input_shape)
 
 class Max(Function):
-  def forward(self, x:LazyBuffer, new_shape:Tuple[int, ...]) -> LazyBuffer:
-    self.x, self.ret = x, x.r(ReduceOps.MAX, new_shape)
+  def forward(self, x:LazyBuffer, axis:Tuple[int, ...]) -> LazyBuffer:
+    self.x, self.ret, self.axis = x, x.r(ReduceOps.MAX, axis), axis
     return self.ret
 
   def backward(self, grad_output:LazyBuffer) -> LazyBuffer:
     # 1s in locations where the max was chosen (can be two locations)
-    max_is_1s = self.x.e(BinaryOps.CMPEQ, self.ret.expand(self.x.shape)).cast(self.x.dtype)
-    div = max_is_1s.r(ReduceOps.SUM, grad_output.shape).expand(self.x.shape)
-    return max_is_1s.e(BinaryOps.DIV, div).e(BinaryOps.MUL, grad_output.expand(self.x.shape))
+    max_is_1s = self.x.e(BinaryOps.CMPEQ, self.ret.expand(self.x.shape)).cast(dtypes.float)
+    div = max_is_1s.r(ReduceOps.SUM, self.axis).expand(self.x.shape)
+    return max_is_1s.e(BinaryOps.DIV, div).cast(grad_output.dtype).e(BinaryOps.MUL, grad_output.expand(self.x.shape))
 
 # ************* movement ops *************
 
 # NOTE: this is sum in reverse
 class Expand(Function):
   def forward(self, x:LazyBuffer, shape:Tuple[int, ...]) -> LazyBuffer:
-    self.input_shape = x.shape
+    self.expanded_axis = tuple(i for i, (si, so) in enumerate(zip(x.shape, shape)) if si != so)
     return x.expand(shape)
 
-  def backward(self, grad_output:LazyBuffer) -> LazyBuffer: return grad_output.r(ReduceOps.SUM, self.input_shape)
+  def backward(self, grad_output:LazyBuffer) -> LazyBuffer:
+    return grad_output.cast(sum_acc_dtype(grad_output.dtype)).r(ReduceOps.SUM, self.expanded_axis).cast(grad_output.dtype)
 
 class Reshape(Function):
   def forward(self, x:LazyBuffer, shape:Tuple[int, ...]) -> LazyBuffer:
     self.input_shape = x.shape
     return x.reshape(shape)
 
   def backward(self, grad_output:LazyBuffer) -> LazyBuffer: return grad_output.reshape(self.input_shape)
```

### Comparing `tinygrad-0.8.0/tinygrad/nn/state.py` & `tinygrad-0.9.0/tinygrad/nn/state.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,102 +1,171 @@
 import os, json, pathlib, zipfile, pickle, tarfile, struct
 from tqdm import tqdm
 from typing import Dict, Union, List, Optional, Any, Tuple
 from tinygrad.tensor import Tensor
-from tinygrad.ops import GlobalCounters
 from tinygrad.dtype import dtypes
-from tinygrad.helpers import prod, argsort, DEBUG, Timing, CI, unwrap
+from tinygrad.helpers import prod, argsort, DEBUG, Timing, CI, unwrap, GlobalCounters
 from tinygrad.shape.view import strides_for_shape
+from tinygrad.multi import MultiLazyBuffer
 
-safe_dtypes = {"F16": dtypes.float16, "F32": dtypes.float32, "U8": dtypes.uint8, "I8": dtypes.int8, "I32": dtypes.int32, "I64": dtypes.int64,
-               "F64": dtypes.double, "B": dtypes.bool, "I16": dtypes.short, "U16": dtypes.ushort, "UI": dtypes.uint, "UL": dtypes.ulong}
+safe_dtypes = {"BOOL":dtypes.bool, "I8":dtypes.int8, "U8":dtypes.uint8, "I16":dtypes.int16, "U16":dtypes.uint16, "I32":dtypes.int, "U32":dtypes.uint,
+               "I64":dtypes.int64, "U64":dtypes.uint64, "F16":dtypes.float16, "BF16":dtypes.bfloat16, "F32":dtypes.float32, "F64":dtypes.float64}
 inverse_safe_dtypes = {v:k for k,v in safe_dtypes.items()}
 
 def safe_load_metadata(fn:Union[Tensor,str]) -> Tuple[Tensor, int, Any]:
+  """
+  Loads a .safetensor file from disk, returning the data, metadata length, and metadata.
+  """
   t = fn if isinstance(fn, Tensor) else Tensor.empty(os.stat(fn).st_size, dtype=dtypes.uint8, device=f"disk:{fn}")
-  json_len = t[0:1].cast(dtypes.int64).numpy()[0]
-  return (t, json_len, json.loads(t[8:8+json_len].numpy().tobytes()))
+  json_len = t[0:8].bitcast(dtypes.int64).item()
+  return t, json_len, json.loads(t[8:8+json_len].numpy().tobytes())
 
 def safe_load(fn:Union[Tensor,str]) -> Dict[str, Tensor]:
+  """
+  Loads a .safetensor file from disk, returning the state_dict.
+
+  ```python
+  state_dict = nn.state.safe_load("test.safetensor")
+  ```
+  """
   t, json_len, metadata = safe_load_metadata(fn)
   ret = {}
   for k,v in metadata.items():
     if k == "__metadata__": continue
     dtype = safe_dtypes[v['dtype']]
-    sz = (v['data_offsets'][1]-v['data_offsets'][0])//dtype.itemsize
-    ret[k] = t[8+json_len+v['data_offsets'][0]:8+json_len+v['data_offsets'][0]+sz].cast(dtype).reshape(v['shape'])
+    sz = (v['data_offsets'][1]-v['data_offsets'][0])
+    ret[k] = t[8+json_len+v['data_offsets'][0]:8+json_len+v['data_offsets'][0]+sz].bitcast(dtype).reshape(v['shape'])
   return ret
 
 def safe_save(tensors:Dict[str, Tensor], fn:str, metadata:Optional[Dict[str, Any]]=None):
+  """
+  Saves a state_dict to disk in a .safetensor file with optional metadata.
+
+  ```python
+  t = nn.Tensor([1, 2, 3])
+  nn.state.safe_save({'t':t}, "test.safetensor")
+  ```
+  """
   headers, offset = {}, 0
   if metadata: headers['__metadata__'] = metadata
   for k,v in tensors.items():
     headers[k] = {'dtype': inverse_safe_dtypes[v.dtype], 'shape': list(v.shape), 'data_offsets':[offset, offset+v.nbytes()]}
     offset += v.nbytes()
   j = json.dumps(headers, separators=(',', ':'))
   j += "\x20"*((8-len(j)%8)%8)
   pathlib.Path(fn).unlink(missing_ok=True)
   t = Tensor.empty(8+len(j)+offset, dtype=dtypes.uint8, device=f"disk:{fn}")
-  t[0:1].cast(dtypes.int64).assign([len(j)])
-  t[8:8+len(j)].assign(Tensor(list(j.encode('utf-8')), dtype=dtypes.uint8, device="cpu"))
+  t[0:8].bitcast(dtypes.int64).assign([len(j)])
+  t[8:8+len(j)].assign(list(j.encode('utf-8')))
   for k,v in safe_load(t).items(): v.assign(tensors[k])
 
 # state dict
 
 from collections import OrderedDict
 def get_state_dict(obj, prefix:str='', tensor_type=Tensor) -> Dict[str, Tensor]:
+  """
+  Returns a state_dict of the object, with optional prefix.
+
+  ```python exec="true" source="above" session="tensor" result="python"
+  class Net:
+    def __init__(self):
+      self.l1 = nn.Linear(4, 5)
+      self.l2 = nn.Linear(5, 6)
+
+  net = Net()
+  print(nn.state.get_state_dict(net).keys())
+  ```
+  """
   if isinstance(obj, tensor_type): return {prefix.strip('.'):obj}
   if hasattr(obj, '_asdict'): return get_state_dict(obj._asdict(), prefix, tensor_type)  # namedtuple
   if isinstance(obj, OrderedDict): return get_state_dict(dict(obj), prefix, tensor_type)
   if hasattr(obj, '__dict__'): return get_state_dict(obj.__dict__, prefix, tensor_type)
   state_dict = {}
   if isinstance(obj, (list, tuple)):
     for i,x in enumerate(obj): state_dict.update(get_state_dict(x, f"{prefix}{str(i)}.", tensor_type))
   elif isinstance(obj, dict):
     for k,v in obj.items(): state_dict.update(get_state_dict(v, f"{prefix}{str(k)}.", tensor_type))
   return state_dict
-def get_parameters(obj) -> List[Tensor]: return list(get_state_dict(obj).values())
-
-def load_state_dict(model, state_dict, strict=True, verbose=True):
+def get_parameters(obj) -> List[Tensor]:
+  """
+  ```python exec="true" source="above" session="tensor" result="python"
+  class Net:
+    def __init__(self):
+      self.l1 = nn.Linear(4, 5)
+      self.l2 = nn.Linear(5, 6)
+
+  net = Net()
+  print(len(nn.state.get_parameters(net)))
+  ```
+  """
+  return list(get_state_dict(obj).values())
+
+def load_state_dict(model, state_dict:Dict[str, Tensor], strict=True, verbose=True, consume=False) -> None:
+  """
+  Loads a state_dict into a model.
+
+  ```python
+  class Net:
+    def __init__(self):
+      self.l1 = nn.Linear(4, 5)
+      self.l2 = nn.Linear(5, 6)
+
+  net = Net()
+  state_dict = nn.state.get_state_dict(net)
+  nn.state.load_state_dict(net, state_dict)
+  ```
+  """
   start_mem_used = GlobalCounters.mem_used
   with Timing("loaded weights in ", lambda et_ns: f", {(GlobalCounters.mem_used-start_mem_used)/1e9:.2f} GB loaded at {(GlobalCounters.mem_used-start_mem_used)/et_ns:.2f} GB/s"):  # noqa: E501
     model_state_dict = get_state_dict(model)
     if DEBUG >= 1 and len(state_dict) > len(model_state_dict):
       print("WARNING: unused weights in state_dict", sorted(list(state_dict.keys() - model_state_dict.keys())))
     for k,v in (t := tqdm(model_state_dict.items(), disable=CI or not verbose)):
       t.set_description(f"ram used: {GlobalCounters.mem_used/1e9:5.2f} GB, {k:50s}")
       if k not in state_dict and not strict:
         if DEBUG >= 1: print(f"WARNING: not loading {k}")
         continue
-      v.assign(state_dict[k].to(v.device)).realize()
+      if isinstance((mlb:=v.lazydata), MultiLazyBuffer):
+        if isinstance(state_dict[k].lazydata, MultiLazyBuffer): v.replace(state_dict[k]).realize()
+        else: v.replace(state_dict[k].shard(mlb.device, mlb.axis)).realize()
+      else: v.replace(state_dict[k].to(v.device)).realize()
+      if consume: del state_dict[k]
 
 # torch support!
 
 def torch_load(fn:str) -> Dict[str, Tensor]:
+  """
+  Loads a torch .pth file from disk.
+
+  ```python
+  state_dict = nn.state.torch_load("test.pth")
+  ```
+  """
   t = Tensor.empty(os.stat(fn).st_size, dtype=dtypes.uint8, device=f"disk:{fn}")
 
   offsets: Dict[Union[str, int], int] = {}
   lens: Dict[Union[str, int], int] = {}
   def _rebuild_tensor_v2(storage, storage_offset, size, stride, requires_grad=None, backward_hooks=None, metadata=None):
     #print(storage, storage_offset, size, stride, requires_grad, backward_hooks, metadata)
     lens[storage[2]] = storage[4] * storage[1].itemsize
     if storage[2] not in offsets: return None
     byte_offset = offsets[storage[2]]+storage_offset*storage[1].itemsize
-    ret = t[byte_offset:byte_offset+prod(size)].cast(storage[1])
+    ret = t[byte_offset:byte_offset+prod(size)*storage[1].itemsize].bitcast(storage[1])
 
     # 7 lines to deal with permuted tensors. NOTE: this currently requires reading off the disk
     shape_strides = [(s, st) for s,st in zip(size, stride) if s != 1]
     permute_indexes = [len(shape_strides)-1-y for y in argsort([x[1] for x in shape_strides])]
     if tuple(permute_indexes) != tuple(range(len(permute_indexes))):
       intermediate_shape = tuple([shape_strides[x][0] for x in argsort(permute_indexes)])
       assert tuple([shape_strides[i][1] for i in argsort(permute_indexes)]) == strides_for_shape(intermediate_shape), "nonpermutable strides"
-      if DEBUG >= 3: print(f"WARNING: this torch load is slow. CPU to permute {intermediate_shape} with {permute_indexes}")
-      assert storage[1] != dtypes.bfloat16, "can't CPU permute BF16"
+      if DEBUG >= 3: print(f"WARNING: this torch load is slow. CLANG to permute {intermediate_shape} with {permute_indexes}")
+      assert storage[1] != dtypes.bfloat16, "can't CLANG permute BF16"
       # TODO: find a nice way to support all shapetracker on disktensors
-      ret = ret.cpu().reshape(intermediate_shape).permute(permute_indexes)
+      # TODO: BUG: a ".realize()" is needed here for 'GPU=1 python3 test/models/test_efficientnet.py TestEfficientNet.test_car'
+      ret = ret.clang().reshape(intermediate_shape).permute(permute_indexes).realize()
 
     return ret.reshape(size)
 
   class Parameter:
     def __setstate__(self, state): self.tensor = state[0]
 
   deserialized_objects: Dict[str, Any] = {}
```

### Comparing `tinygrad-0.8.0/tinygrad/ops.py` & `tinygrad-0.9.0/tinygrad/ops.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,110 +1,136 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING, Union, Type, Tuple, Any, List, Dict, Callable, ClassVar
-import functools
+from typing import Union, Tuple, Any, List, Dict, Callable
+import functools, hashlib, math, operator, ctypes
 from enum import Enum, auto
-from tinygrad.helpers import prod, dedup
-from tinygrad.dtype import dtypes, DType
-from tinygrad.shape.symbolic import Variable
 from dataclasses import dataclass
+from tinygrad.helpers import prod, dedup
+from tinygrad.dtype import dtypes, DType, ConstType
+from tinygrad.shape.symbolic import Variable, sint
+from tinygrad.shape.shapetracker import ShapeTracker
 
 # these are the llops your accelerator must implement, along with toCpu
 # the Enum class doesn't work with mypy, this is static. sorry it's ugly
 # NOTE: MOD, CMPLT don't have to be implemented on vectors, just scalars
 # NOTE: many GPUs don't have DIV, but UnaryOps.RECIP doesn't work for integer division
-class UnaryOps(Enum): EXP2 = auto(); LOG2 = auto(); CAST = auto(); SIN = auto(); SQRT = auto(); NEG = auto() # noqa: E702
+class UnaryOps(Enum):
+  """A -> A (elementwise)"""
+  EXP2 = auto(); LOG2 = auto(); CAST = auto(); BITCAST = auto(); SIN = auto(); SQRT = auto(); NEG = auto() # noqa: E702
 class BinaryOps(Enum):
+  """A + A -> A (elementwise)"""
   ADD = auto(); SUB = auto(); MUL = auto(); DIV = auto(); MAX = auto(); MOD = auto(); CMPLT = auto(); CMPEQ = auto(); XOR = auto() # noqa: E702
-class TernaryOps(Enum): MULACC = auto(); WHERE = auto() # noqa: E702
-class ReduceOps(Enum): SUM = auto(); MAX = auto() # noqa: E702
+class TernaryOps(Enum):
+  """A + A + A -> A (elementwise)"""
+  WHERE = auto(); MULACC = auto() # noqa: E702
+class ReduceOps(Enum):
+  """A -> B (reduce)"""
+  SUM = auto(); MAX = auto() # noqa: E702
 class BufferOps(Enum): LOAD = auto(); CONST = auto(); STORE = auto() # noqa: E702
-# Ops below this line are not allowed in ASTs
-class MovementOps(Enum): RESHAPE = auto(); PERMUTE = auto(); EXPAND = auto(); PAD = auto(); SHRINK = auto(); STRIDE = auto(); AS_STRIDED = auto() # noqa: E702
-class LoadOps(Enum): EMPTY = auto(); CONST = auto(); COPY = auto(); CONTIGUOUS = auto(); CUSTOM = auto() # noqa: E702
-
-Op = Union[UnaryOps, BinaryOps, ReduceOps, MovementOps, LoadOps, TernaryOps, BufferOps]
-OpType = Union[Type[UnaryOps], Type[BinaryOps], Type[ReduceOps], Type[MovementOps], Type[LoadOps], Type[TernaryOps], Type[BufferOps]]
-
-if TYPE_CHECKING:
-  from tinygrad.shape.shapetracker import ShapeTracker
-  from tinygrad.lazy import LazyBuffer
+class LoadOps(Enum): EMPTY = auto(); CONST = auto(); COPY = auto(); CONTIGUOUS = auto(); CUSTOM = auto(); ASSIGN = auto(); VIEW = auto() # noqa: E702
+
+Op = Union[UnaryOps, BinaryOps, ReduceOps, LoadOps, TernaryOps, BufferOps]
+
+# do not preserve f(0) = 0
+UNSAFE_PAD_OPS = {BinaryOps.DIV, BinaryOps.CMPLT, BinaryOps.CMPEQ, UnaryOps.LOG2, UnaryOps.EXP2}
 
 @dataclass(frozen=True)
 class MemBuffer:
   idx: int
   dtype: DType
   st: ShapeTracker
 
 @dataclass(frozen=True)
 class ConstBuffer:
-  val: Union[int, float]
+  val: ConstType
   dtype: DType
   st: ShapeTracker
 
-@dataclass(frozen=True)
-class ScheduleItem:
-  ast: LazyOp
-  out: LazyBuffer
-  inputs: Tuple[LazyBuffer, ...]
-  var_vals: Dict[Variable, int]
-
 @dataclass(frozen=True, eq=False)
 class LazyOp:
   op: Op
   src: Tuple[LazyOp, ...] = ()
   arg: Any = None
   def cached_compare(self, x, context):
     if id(self) == id(x): return True
     if self.op != x.op or self.arg != x.arg or len(self.src) != len(x.src): return False
     if (key := (id(self), id(x))) in context: return context[key]
     ret = context[key] = all(a.cached_compare(b, context) for a,b in zip(self.src, x.src))
     return ret
   def __eq__(self, x): return self.cached_compare(x, context={})
   def __repr__(self): return f"LazyOp(op={self.op}, src={self.src}, arg={self.arg})"
   @functools.cached_property
+  def dtype(self) -> DType:
+    if self.op in BufferOps: return self.arg.dtype
+    if self.op in [UnaryOps.CAST, UnaryOps.BITCAST]: return self.arg
+    return dtypes.bool if self.op in {BinaryOps.CMPLT, BinaryOps.CMPEQ} else self.src[-1].dtype
+
+  @functools.cached_property
+  def key(self) -> bytes:
+    return hashlib.sha256(functools.reduce(lambda x,y: x+y, [s.key for s in self.src], str((self.op, self.arg)).encode())).digest()
+  @functools.cached_property
   def hash(self): return hash((self.op, self.src, self.arg))
   def __hash__(self): return self.hash
   @functools.cached_property
   def lazyops(self) -> List[LazyOp]: return dedup([self] + [item for x in self.src for item in x.lazyops])
   def vars(self) -> List[Variable]:
-    return sorted(set.union(*[x.arg.st.vars() for x in self.lazyops if x.op in BufferOps], set()), key=lambda x: str(x.expr))
+    extract_vars = [x.arg.st.vars() for x in self.lazyops if x.op in BufferOps]
+    const_vars = [x.arg.val.unbind()[0] for x in self.lazyops if x.op is BufferOps.CONST and isinstance(x.arg.val, Variable)]
+    return sorted(set.union(*extract_vars, set(const_vars)), key=lambda x: str(x.expr))
 
 # **************** independent FlopCounter ****************
 
 @dataclass
 class FlopCounter:
   shape: Tuple[int, ...]
-  dtype: DType
-  flops: int
+  flops: sint
   mem: Dict[int, int]
   @property
   def mem_estimate(self): return sum(self.mem.values())
   def consume_flops(self):
     self.flops, ret = 0, self.flops
     return ret
 
 InterpretedFlopCounter: Dict[Op, Callable] = {
-  BufferOps.LOAD: lambda arg: FlopCounter(arg.st.shape, arg.dtype, 0, {arg.idx: arg.dtype.itemsize*arg.st.real_size()}),
-  BufferOps.CONST: lambda arg: FlopCounter(arg.st.shape, arg.dtype, 0, {}),
-  BufferOps.STORE: lambda self,arg: FlopCounter(arg.st.shape, arg.dtype, self.consume_flops(), {**self.mem, arg.idx: arg.dtype.itemsize*arg.st.real_size()}),  # noqa: E501
-  UnaryOps.CAST: lambda self,arg: FlopCounter(self.shape, arg[0], self.consume_flops(), self.mem),   # cast uses no flops
-  **{op:lambda self: FlopCounter(self.shape, self.dtype, self.consume_flops() + prod(self.shape), self.mem) for op in UnaryOps if op != UnaryOps.CAST},  # noqa: E501
-  **{op:lambda self,y,op=op: FlopCounter(self.shape,  dtypes.bool if op in (BinaryOps.CMPLT, BinaryOps.CMPEQ) else self.dtype, self.consume_flops() + y.consume_flops() + prod(self.shape), {**self.mem, **y.mem}) for op in BinaryOps},  # noqa: E501
-  **{op:lambda self,new_shape: FlopCounter(new_shape, self.dtype, self.consume_flops() + prod(self.shape), self.mem) for op in ReduceOps},
-  TernaryOps.WHERE: lambda self,y,z: FlopCounter(self.shape, y.dtype, self.consume_flops() + y.consume_flops() + z.consume_flops() + prod(self.shape), {**self.mem, **y.mem, **z.mem})}  # noqa: E501
+  BufferOps.LOAD: lambda arg: FlopCounter(arg.st.shape, 0, {arg.idx: arg.dtype.itemsize * arg.st.real_size()}),
+  BufferOps.CONST: lambda arg: FlopCounter(arg.st.shape, 0, {}),
+  BufferOps.STORE: lambda self,arg: FlopCounter(arg.st.shape, self.consume_flops(), {**self.mem, arg.idx: arg.dtype.itemsize * arg.st.real_size()}),
+  UnaryOps.CAST: lambda self,arg: FlopCounter(self.shape, self.consume_flops(), self.mem),   # cast uses no flops
+  UnaryOps.BITCAST: lambda self,arg: FlopCounter(self.shape, self.consume_flops(), self.mem),   # bitcast uses no flops
+  **{op:lambda self: FlopCounter(self.shape, self.consume_flops() + prod(self.shape), self.mem) for op in UnaryOps if op not in {UnaryOps.CAST, UnaryOps.BITCAST}},  # noqa: E501
+  **{op:lambda self,y: FlopCounter(self.shape, self.consume_flops() + y.consume_flops() + prod(self.shape), {**self.mem, **y.mem}) for op in BinaryOps},  # noqa: E501
+  **{op:lambda self,axis: FlopCounter(tuple(1 if i in axis else s for i,s in enumerate(self.shape)), self.consume_flops() + prod(self.shape), self.mem) for op in ReduceOps},  # noqa: E501
+  TernaryOps.WHERE: lambda self,y,z: FlopCounter(self.shape, self.consume_flops() + y.consume_flops() + z.consume_flops() + prod(self.shape), {**self.mem, **y.mem, **z.mem})}  # noqa: E501
 
 @functools.lru_cache(None)
 def get_lazyop_info(ast:LazyOp) -> FlopCounter:
   @functools.lru_cache(None) # NOTE: this cache needs to be recreated for new ASTs
   def run_ast(ast): return InterpretedFlopCounter[ast.op](*([run_ast(x) for x in ast.src]+([ast.arg] if ast.arg is not None else [])))
   return run_ast(ast)
 
-# **************** global state Counters ****************
+# **************** ops in python ****************
+
+def hook_overflow(dv, fxn):
+  def wfxn(*args):
+    try: return fxn(*args)
+    except OverflowError: return dv
+  return wfxn
+
+python_alu = {
+  UnaryOps.LOG2: lambda x: math.log2(x) if x > 0 else -math.inf if x == 0 else math.nan,
+  UnaryOps.EXP2: hook_overflow(math.inf, lambda x: math.exp(x*math.log(2))),
+  UnaryOps.SQRT: lambda x: math.sqrt(x) if x >= 0 else math.nan, UnaryOps.SIN: math.sin,
+  UnaryOps.NEG: lambda x: (not x) if isinstance(x, bool) else -x,
+  BinaryOps.MUL: operator.mul, BinaryOps.ADD: operator.add, BinaryOps.SUB: operator.sub, BinaryOps.XOR: operator.xor,
+  BinaryOps.MAX: max, BinaryOps.CMPEQ: operator.eq, BinaryOps.CMPLT: operator.lt,
+  BinaryOps.MOD: lambda x,y: abs(int(x))%abs(int(y))*(1,-1)[x<0],
+  BinaryOps.DIV: lambda x,y: int(x/y) if isinstance(x, int) else (x/y if y != 0 else x*math.inf),
+  TernaryOps.WHERE: lambda x,y,z: y if x else z}
+
+truncate: Dict[DType, Callable] = {dtypes.bool: bool,
+  # TODO: float16 and bfloat16?
+  dtypes.float32: lambda x: ctypes.c_float(x).value, dtypes.float64: lambda x: ctypes.c_double(x).value,
+  dtypes.uint8: lambda x: ctypes.c_uint8(x).value, dtypes.uint16: lambda x: ctypes.c_uint16(x).value,
+  dtypes.uint32: lambda x: ctypes.c_uint32(x).value, dtypes.uint64: lambda x: ctypes.c_uint64(x).value,
+  dtypes.int8: lambda x: ctypes.c_int8(x).value, dtypes.int16: lambda x: ctypes.c_int16(x).value,
+  dtypes.int32: lambda x: ctypes.c_int32(x).value, dtypes.int64: lambda x: ctypes.c_int64(x).value,}
 
-class GlobalCounters:
-  global_ops: ClassVar[int] = 0
-  global_mem: ClassVar[int] = 0
-  time_sum_s: ClassVar[float] = 0.0
-  kernel_count: ClassVar[int] = 0
-  mem_used: ClassVar[int] = 0   # NOTE: this is not reset
-  @staticmethod
-  def reset(): GlobalCounters.global_ops, GlobalCounters.global_mem, GlobalCounters.time_sum_s, GlobalCounters.kernel_count = 0,0,0.0,0
+def exec_alu(op:Op, dtype:DType, operands): return truncate.get(dtype, lambda x: x)(python_alu[op](*operands))
```

### Comparing `tinygrad-0.8.0/tinygrad/renderer/llvmir.py` & `tinygrad-0.9.0/tinygrad/renderer/llvmir.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,165 +1,160 @@
 from typing import Final, Dict, Callable, Any, List, Optional
 from llvmlite import ir
 from tinygrad.codegen.linearizer import UOps, UOp
 from tinygrad.dtype import DType, PtrDType, dtypes
 from tinygrad.ops import Op, UnaryOps, BinaryOps, TernaryOps
+from tinygrad.codegen.uops import UOpGraph
+from tinygrad.renderer import Renderer
 
 MFLAGS = ('nsz', 'arcp', 'contract', 'afn', 'reassoc') # All from fast math, but nnan and ninf
 
 def is_bool_or_unsigned(dtype: DType): return dtype == dtypes.bool or dtypes.is_unsigned(dtype)
 
 code_for_op: Final[Dict[Op, Callable]] = {
-    UnaryOps.NEG: lambda builder, x, var_dtype: builder.xor(x, ir.Constant(ir.IntType(1), 1)) if var_dtype == dtypes.bool else builder.neg(x) if dtypes.is_int(var_dtype) else builder.fneg(x, flags=MFLAGS),  # noqa: E501
-    UnaryOps.EXP2: lambda builder, x, var_dtype: builder.call(builder._block.module.declare_intrinsic('llvm.exp2', [x.type]), [x], fastmath=MFLAGS),
-    UnaryOps.LOG2: lambda builder, x, var_dtype: builder.call(builder._block.module.declare_intrinsic('llvm.log2', [x.type]), [x], fastmath=MFLAGS),
-    UnaryOps.SIN: lambda builder, x, var_dtype: builder.call(builder._block.module.declare_intrinsic('llvm.sin', [x.type]), [x], fastmath=MFLAGS),
-    UnaryOps.SQRT: lambda builder, x, var_dtype: builder.call(builder._block.module.declare_intrinsic('llvm.sqrt', [x.type]), [x], fastmath=MFLAGS),
-    BinaryOps.ADD: lambda builder, x, y, var_dtype: builder.or_(x, y) if var_dtype == dtypes.bool else builder.add(x, y) if dtypes.is_int(var_dtype) else builder.fadd(x, y, flags=MFLAGS),  # noqa: E501
-    BinaryOps.SUB: lambda builder, x, y, var_dtype: builder.sub(x, y) if dtypes.is_int(var_dtype) else builder.fsub(x, y, flags=MFLAGS),
-    BinaryOps.MUL: lambda builder, x, y, var_dtype: # TOOD should we use umul_with_overflow?
-      builder.mul(x, y) if is_bool_or_unsigned(var_dtype) or dtypes.is_int(var_dtype) else builder.fmul(x, y, flags=MFLAGS),
-    BinaryOps.DIV: lambda builder, x, y, var_dtype:
-      builder.udiv(x, y) if is_bool_or_unsigned(var_dtype) else builder.sdiv(x, y) if dtypes.is_int(var_dtype) else builder.fdiv(x, y, flags=MFLAGS),
-    BinaryOps.CMPLT: lambda builder, x, y, var_dtype: builder.icmp_unsigned("<", x, y) if is_bool_or_unsigned(var_dtype) else builder.icmp_signed("<", x, y) if dtypes.is_int(var_dtype) else builder.fcmp_unordered("<", x, y, flags=MFLAGS),  # noqa: E501
-    BinaryOps.CMPEQ: lambda builder, x, y, var_dtype: builder.icmp_unsigned("==", x, y) if is_bool_or_unsigned(var_dtype) else builder.icmp_signed("==", x, y) if dtypes.is_int(var_dtype) else builder.fcmp_unordered("==", x, y, flags=MFLAGS),  # noqa: E501
-    BinaryOps.MAX: lambda builder, x, y, var_dtype: builder.select(builder.icmp_unsigned(">", x, y) if is_bool_or_unsigned(var_dtype) else builder.icmp_signed(">", x, y) if dtypes.is_int(var_dtype) else builder.fcmp_unordered(">", x, y, flags=MFLAGS), x, y),  # noqa: E501
-    BinaryOps.MOD: lambda builder, x, y, var_dtype:
-      builder.urem(x, y) if is_bool_or_unsigned(var_dtype) else builder.srem(x, y) if dtypes.is_int(var_dtype) else builder.frem(x, y),
-    BinaryOps.XOR: lambda builder, x, y, var_dtype: builder.xor(x, y),
-    TernaryOps.MULACC: lambda builder, x, y, z, var_dtype: builder.fadd(builder.fmul(x, y, flags=MFLAGS), z, flags=MFLAGS) \
-      if dtypes.is_float(var_dtype) else builder.add(builder.mul(x, y), z),
-    TernaryOps.WHERE: lambda builder, x, y, z, var_dtype: builder.select(x, y, z),
-}
+  UnaryOps.NEG: lambda builder, x, dtype: builder.neg(x) if dtypes.is_int(dtype) else \
+    (builder.not_(x) if dtype == dtypes.bool else builder.fneg(x, flags=MFLAGS)),
+  UnaryOps.EXP2: lambda builder, x, dtype: builder.call(builder.module.declare_intrinsic('llvm.exp2', [x.type]), [x], fastmath=MFLAGS),
+  UnaryOps.LOG2: lambda builder, x, dtype: builder.call(builder.module.declare_intrinsic('llvm.log2', [x.type]), [x], fastmath=MFLAGS),
+  UnaryOps.SIN: lambda builder, x, dtype: builder.call(builder.module.declare_intrinsic('llvm.sin', [x.type]), [x], fastmath=MFLAGS),
+  UnaryOps.SQRT: lambda builder, x, dtype: builder.call(builder.module.declare_intrinsic('llvm.sqrt', [x.type]), [x], fastmath=MFLAGS),
+  BinaryOps.ADD: lambda builder, x, y, dtype: builder.or_(x, y) if dtype == dtypes.bool else builder.add(x, y) if dtypes.is_int(dtype) else builder.fadd(x, y, flags=MFLAGS),  # noqa: E501
+  BinaryOps.SUB: lambda builder, x, y, dtype: builder.sub(x, y) if dtypes.is_int(dtype) else builder.fsub(x, y, flags=MFLAGS),
+  BinaryOps.MUL: lambda builder, x, y, dtype: builder.mul(x, y) if is_bool_or_unsigned(dtype) or dtypes.is_int(dtype) else builder.fmul(x, y, flags=MFLAGS),  # noqa: E501
+  BinaryOps.DIV: lambda builder, x, y, dtype: builder.udiv(x, y) if is_bool_or_unsigned(dtype) else builder.sdiv(x, y) if dtypes.is_int(dtype) else builder.fdiv(x, y, flags=MFLAGS),  # noqa: E501
+  BinaryOps.CMPLT: lambda builder, x, y, dtype: builder.icmp_unsigned("<", x, y) if is_bool_or_unsigned(dtype) else builder.icmp_signed("<", x, y) if dtypes.is_int(dtype) else builder.fcmp_unordered("<", x, y, flags=MFLAGS),  # noqa: E501
+  BinaryOps.CMPEQ: lambda builder, x, y, dtype: builder.icmp_unsigned("==", x, y) if is_bool_or_unsigned(dtype) else builder.icmp_signed("==", x, y) if dtypes.is_int(dtype) else builder.fcmp_unordered("==", x, y, flags=MFLAGS),  # noqa: E501
+  BinaryOps.MAX: lambda builder, x, y, dtype: builder.select(builder.icmp_unsigned(">", x, y) if is_bool_or_unsigned(dtype) else builder.icmp_signed(">", x, y) if dtypes.is_int(dtype) else builder.fcmp_unordered(">", x, y, flags=MFLAGS), x, y),  # noqa: E501
+  BinaryOps.MOD: lambda builder, x, y, dtype: builder.urem(x, y) if is_bool_or_unsigned(dtype) else builder.srem(x, y) if dtypes.is_int(dtype) else builder.frem(x, y),  # noqa: E501
+  BinaryOps.XOR: lambda builder, x, y, dtype: builder.xor(x, y),
+  TernaryOps.WHERE: lambda builder, x, y, z, dtype: builder.select(x, y, z)}
 
 dtype_to_llvm_dtype = { dtypes.bool:ir.IntType(1), dtypes.int8:ir.IntType(8), dtypes.uint8:ir.IntType(8), dtypes.int16:ir.IntType(16),
   dtypes.uint16:ir.IntType(16), dtypes.int32:ir.IntType(32), dtypes.uint32:ir.IntType(32), dtypes.int64:ir.IntType(64), dtypes.uint64:ir.IntType(64),
   dtypes.float16:ir.HalfType(), dtypes.bfloat16:ir.IntType(16), dtypes.float32:ir.FloatType(), dtypes.float64:ir.DoubleType() }
 
 def cast(bb, val, input_type, output_type, bitcast=False):
   if input_type == output_type: return val
-  if bitcast: return bb[-1].bitcast(val, dtype_to_llvm_dtype[output_type])
+  llvm_type = dtype_to_llvm_dtype[output_type]
+  if bitcast: return bb[-1].bitcast(val, llvm_type)
 
   if input_type == dtypes.bfloat16:
     val = bb[-1].bitcast(bb[-1].shl(bb[-1].sext(val, ir.IntType(32)), ir.Constant(ir.IntType(32), 16)),val, ir.FloatType())
     input_type = dtypes.float32
   if output_type == dtypes.bfloat16:
     val = cast(bb, val, input_type, dtypes.float32)
     return bb[-1].trunc(bb[-1].lshr(bb[-1].bitcast(val, ir.IntType(32)), ir.Constant(ir.IntType(32), 16)), ir.IntType(16))
 
   if dtypes.is_float(input_type):
     if dtypes.is_float(output_type):
-      if output_type.itemsize > input_type.itemsize: return bb[-1].fpext(val, dtype_to_llvm_dtype[output_type])
-      return bb[-1].fptrunc(val, dtype_to_llvm_dtype[output_type])
-    if dtypes.is_int(output_type):
-      if dtypes.is_unsigned(output_type): return bb[-1].fptoui(val, dtype_to_llvm_dtype[output_type])
-      return bb[-1].fptosi(val, dtype_to_llvm_dtype[output_type])
+      return bb[-1].fpext(val, llvm_type) if output_type.itemsize > input_type.itemsize else bb[-1].fptrunc(val, llvm_type)
+    if dtypes.is_int(output_type): return bb[-1].fptoui(val, llvm_type) if dtypes.is_unsigned(output_type) else bb[-1].fptosi(val, llvm_type)
     if output_type == dtypes.bool: return bb[-1].fcmp_unordered('!=', cast(bb, val, input_type, dtypes.float32), ir.Constant(ir.FloatType(), 0))
 
   if dtypes.is_unsigned(input_type) or input_type == dtypes.bool:
     if output_type == dtypes.float16: return bb[-1].fptrunc(bb[-1].uitofp(val, ir.FloatType()), ir.HalfType())
     if dtypes.is_float(output_type): return bb[-1].uitofp(val, dtype_to_llvm_dtype[output_type])
-    if dtypes.is_int(output_type):
-      if input_type.itemsize > output_type.itemsize: return bb[-1].trunc(val, dtype_to_llvm_dtype[output_type])
-      return bb[-1].zext(val, dtype_to_llvm_dtype[output_type])
+    if dtypes.is_int(output_type): return bb[-1].trunc(val, llvm_type) if input_type.itemsize > output_type.itemsize else bb[-1].zext(val, llvm_type)
     if output_type == dtypes.bool: return bb[-1].icmp_unsigned('!=', val, ir.Constant(val.type, 0))
 
   if dtypes.is_int(input_type):
     if output_type == dtypes.float16: return bb[-1].fptrunc(bb[-1].sitofp(val, ir.FloatType()), ir.HalfType())
-    if dtypes.is_float(output_type): return bb[-1].sitofp(val, dtype_to_llvm_dtype[output_type])
-    if dtypes.is_int(output_type):
-      if input_type.itemsize > output_type.itemsize: return bb[-1].trunc(val, dtype_to_llvm_dtype[output_type])
-      return bb[-1].sext(val, dtype_to_llvm_dtype[output_type])
+    if dtypes.is_float(output_type): return bb[-1].sitofp(val, llvm_type)
+    if dtypes.is_int(output_type): return bb[-1].trunc(val, llvm_type) if input_type.itemsize > output_type.itemsize else bb[-1].sext(val, llvm_type)
     if output_type == dtypes.bool: return bb[-1].icmp_signed('!=', val, ir.Constant(val.type, 0))
 
   raise NotImplementedError(f"cast from {input_type} -> {output_type} not implemented")
 
-def const(args, dtype):
-  # TODO: remove int from int(args) once const args conform with dtype
-  return ir.Constant(dtype_to_llvm_dtype[dtype], int(args) if dtypes.is_int(dtype) else bool(args) if dtype == dtypes.bool else args)
-
-def uops_to_llvm_ir(function_name:str, uops:List[UOp]) -> str:
-  # all llvm stuff goes into a module
-  module = ir.Module(name=__file__)
-
-  # extract global buffers
-  buf_to_dtype = {u.arg:u.dtype for u in uops if u.uop == UOps.DEFINE_GLOBAL}
-  buf_index = {x:i for i,x in enumerate(buf_to_dtype.keys())}
-
-  # create llvm function
-  func_dtypes = [(dtype_to_llvm_dtype[dtype],dtype) for dtype in buf_to_dtype.values() if dtype is not None]
-  func = ir.Function(module, ir.FunctionType(ir.VoidType(), [x.as_pointer() if isinstance(dt, PtrDType) else x for x,dt in func_dtypes]), name=function_name)  # noqa: E501
-  for a in func.args:
-    if a.type.is_pointer: a.add_attribute("noalias")
-
-  # add the function attribute "no-nans-fp-math"="true", which informs llvm that it allowed to use vectorization optimizations
-  func.attributes._known = func.attributes._known.union(frozenset(['"no-nans-fp-math"="true"']))
-  func.attributes.add('"no-nans-fp-math"="true"')
-
-  bb = [ir.IRBuilder(func.append_basic_block("entry"))]
-  loop_blocks: List = []
-  reduce_phis: List = []
-  # TODO: newvar probably shouldn't be optional
-  lvars: Dict[Optional[UOp], Any] = {}  # this Any is an llvm type
-
-  for bufname,dtype in buf_to_dtype.items():
-    if not isinstance(dtype, PtrDType) and dtype == dtypes.int32: lvars[bufname] = bb[-1].sext(func.args[buf_index[bufname]], ir.IntType(32))
-
-  for u in uops:
-    uop,dtype,vin,args = u.uop,u.dtype,u.vin,u.arg
-    if uop == UOps.LOOP:
-      bb.append(ir.IRBuilder(func.append_basic_block(f"loop_body_{len(loop_blocks)}")))
-      bb[-2].branch(bb[-1]._block)
-
-      phis = []
-      for rp in reduce_phis:
-        incoming = lvars[rp]
-        lvars[rp] = bb[-1].phi(dtype_to_llvm_dtype[rp.dtype])
-        lvars[rp].add_incoming(incoming, bb[-2]._block)
-        phis.append((rp, lvars[rp]))
-
-      lvars[u] = bb[-1].phi(ir.IntType(32), name=f"loop{len(loop_blocks)}")
-      lvars[u].add_incoming(lvars[vin[0]], bb[-2]._block)
-      loop_blocks.append((bb[-1], phis))
-    if uop == UOps.END:
-      block, phis = loop_blocks.pop()
-      idx_p1 = bb[-1].add(lvars[vin[0]], ir.Constant(ir.IntType(32), 1))
-      lvars[vin[0]].add_incoming(idx_p1, bb[-1]._block)
-      for n,phi in phis: phi.add_incoming(lvars[n], bb[-1]._block)
-      bb.append(ir.IRBuilder(func.append_basic_block(f"loop_exit_{len(loop_blocks)}")))
-      bb[-2].cbranch(bb[-2].icmp_unsigned("<", idx_p1, lvars[vin[0].vin[1]]), block._block, bb[-1]._block)
-    if uop == UOps.DEFINE_GLOBAL: lvars[u] = func.args[buf_index[args]]
-    if uop == UOps.DEFINE_ACC:
-      lvars[u] = const(args, dtype)
-      reduce_phis.append(u)
-    if uop == UOps.SPECIAL: lvars[u] = lvars[args.expr]
-    if uop == UOps.CONST: lvars[u] = const(args, dtype)
-    if uop == UOps.LOAD:
-      assert dtype is not None
-      if len(vin) > 2:
-        gate = bb[-1].trunc(lvars[vin[2]], ir.IntType(1))
-        aug_idx = bb[-1].select(gate, lvars[vin[1]], ir.Constant(ir.IntType(32), 0))
-        val = bb[-1].load(bb[-1].gep(lvars[vin[0]], [aug_idx], inbounds=True))
-        val = cast(bb, val, vin[0].dtype, dtype)
-        val = bb[-1].select(gate, val, lvars[vin[3]])
+def const(args, dtype): return ir.Constant(dtype_to_llvm_dtype[dtype], args)
+
+class LLVMRenderer(Renderer):
+  device = "LLVM"
+  supports_float4=False
+  has_local=False
+  has_shared=False
+
+  def render(self, name:str, uops:UOpGraph) -> str:
+    # all llvm stuff goes into a module
+    module = ir.Module(name=__file__)
+
+    # extract global buffers (NOTE: this isn't right if DEFINE_GLOBAL is out of order)
+    buf_to_dtype = {u.arg:u.dtype for u in uops if u.uop in {UOps.DEFINE_GLOBAL, UOps.DEFINE_VAR}}
+    buf_index = {x:i for i,x in enumerate(buf_to_dtype.keys())}
+
+    # create llvm function
+    func_dtypes = [(dtype_to_llvm_dtype[dtype],dtype) for dtype in buf_to_dtype.values() if dtype is not None]
+    func = ir.Function(module, ir.FunctionType(ir.VoidType(), [x.as_pointer() if isinstance(dt, PtrDType) else x for x,dt in func_dtypes]), name=name)
+    for a in func.args:
+      if a.type.is_pointer: a.add_attribute("noalias")
+
+    # add the function attribute "no-nans-fp-math"="true", which informs llvm that it allowed to use vectorization optimizations
+    func.attributes._known = func.attributes._known.union(frozenset(['"no-nans-fp-math"="true"']))
+    func.attributes.add('"no-nans-fp-math"="true"')
+
+    bb = [ir.IRBuilder(func.append_basic_block("entry"))]
+    loop_blocks: List = []
+    reduce_phis: List = []
+    # TODO: newvar probably shouldn't be optional
+    lvars: Dict[Optional[UOp], Any] = {}  # this Any is an llvm type
+
+    for bufname,dtype in buf_to_dtype.items():
+      if not isinstance(dtype, PtrDType) and dtype == dtypes.int32: lvars[bufname] = bb[-1].sext(func.args[buf_index[bufname]], ir.IntType(32))
+
+    for u in uops:
+      uop,dtype,vin,args = u.uop,u.dtype,u.vin,u.arg
+      if uop is UOps.STORE:
+        element = cast(bb, lvars[vin[2]], vin[2].dtype, vin[0].dtype)
+        if len(vin) > 3:
+          with bb[-1].if_then(lvars[vin[3]]):
+            bb[-1].store(element, bb[-1].gep(lvars[vin[0]], [lvars[vin[1]]], inbounds=True))
+        else:
+          bb[-1].store(element, bb[-1].gep(lvars[vin[0]], [lvars[vin[1]]], inbounds=True))
+      elif uop is UOps.ENDRANGE:
+        loop_entry_bb, phis = loop_blocks.pop()
+        idx_p1 = bb[-1].add(lvars[vin[0]], ir.Constant(ir.IntType(32), 1))
+        lvars[vin[0]].add_incoming(idx_p1, bb[-1].block)
+        for n,phi in phis: phi.add_incoming(lvars[n], bb[-1].block)
+        bb.append(ir.IRBuilder(func.append_basic_block(f"loop_exit_{len(loop_blocks)}")))
+        bb[-2].cbranch(bb[-2].icmp_unsigned("<", idx_p1, lvars[vin[0].vin[1]]), loop_entry_bb, bb[-1].block)
       else:
-        val = bb[-1].load(bb[-1].gep(lvars[vin[0]], [lvars[vin[1]]], inbounds=True))
-        val = cast(bb, val, vin[0].dtype, dtype)
-      lvars[u] = val
-    if uop == UOps.PHI:
-      lvars[u] = lvars[vin[1]]
-      # PHI UOps can link to other PHI Uops, backtrace this to DEFINE_ACC
-      backward = vin[0]
-      while backward.uop == UOps.PHI: backward = backward.vin[0]
-      lvars[backward] = lvars[u]
-    if uop == UOps.STORE:
-      element = cast(bb, lvars[vin[2]], vin[2].dtype, vin[0].dtype)
-      def store_op(): bb[-1].store(element, bb[-1].gep(lvars[vin[0]], [lvars[vin[1]]], inbounds=True))
-      if len(vin) > 3:
-        with bb[-1].if_then(bb[-1].trunc(lvars[vin[3]], ir.IntType(1))): store_op()
-      else: store_op()
-    if uop == UOps.ALU:
-      lvars[u] = code_for_op[args](bb[-1], *[lvars[x] for x in vin] + [dtype if args not in (BinaryOps.CMPLT, BinaryOps.CMPEQ) else vin[0].dtype])
-    if uop == UOps.CAST: lvars[u] = cast(bb, lvars[vin[0]], vin[0].dtype, dtype, bitcast=isinstance(args, tuple) and args[1])
+        assert dtype is not None, f"None dtype for uop {uop}"
+        if uop is UOps.RANGE:
+          bb.append(ir.IRBuilder(func.append_basic_block(f"loop_body_{len(loop_blocks)}")))
+          bb[-2].branch(bb[-1].block)
+
+          phis = []
+          for rp in reduce_phis:
+            incoming = lvars[rp]
+            lvars[rp] = bb[-1].phi(dtype_to_llvm_dtype[rp.dtype])
+            lvars[rp].add_incoming(incoming, bb[-2].block)
+            phis.append((rp, lvars[rp]))
+
+          lvars[u] = bb[-1].phi(ir.IntType(32), name=f"loop{len(loop_blocks)}")
+          lvars[u].add_incoming(lvars[vin[0]], bb[-2].block)
+          loop_blocks.append((bb[-1].block, phis))
+        elif uop is UOps.DEFINE_ACC:
+          lvars[u] = const(args[0], dtype)
+          reduce_phis.append(u)
+        elif uop is UOps.LOAD:
+          if len(vin) > 2:
+            aug_idx = bb[-1].select(lvars[vin[2]], lvars[vin[1]], ir.Constant(ir.IntType(32), 0))
+            val = bb[-1].load(bb[-1].gep(lvars[vin[0]], [aug_idx], inbounds=True))
+            val = bb[-1].select(lvars[vin[2]], val, lvars[vin[3]])
+          else:
+            val = bb[-1].load(bb[-1].gep(lvars[vin[0]], [lvars[vin[1]]], inbounds=True))
+          lvars[u] = val
+        elif uop is UOps.PHI:
+          lvars[u] = lvars[vin[1]]
+          # PHI UOps can link to other PHI Uops, backtrace this to DEFINE_ACC
+          backward = vin[0]
+          while backward.uop is UOps.PHI: backward = backward.vin[0]
+          lvars[backward] = lvars[u]
+        elif uop is UOps.ALU:
+          lvars[u] = code_for_op[args](bb[-1], *[lvars[x] for x in vin], dtype if args not in (BinaryOps.CMPLT, BinaryOps.CMPEQ) else vin[0].dtype)
+        elif uop in {UOps.CAST, UOps.BITCAST}: lvars[u] = cast(bb, lvars[vin[0]], vin[0].dtype, dtype, bitcast=uop is UOps.BITCAST)
+        elif uop in {UOps.DEFINE_GLOBAL, UOps.DEFINE_VAR}: lvars[u] = func.args[buf_index[args]]
+        elif uop is UOps.SPECIAL: lvars[u] = lvars[args.expr]
+        elif uop is UOps.CONST: lvars[u] = const(args, dtype)
+        else: raise RuntimeError(f"failed to render {uop}")
 
-  bb[-1].ret_void()
-  return str(module)
+    bb[-1].ret_void()
+    return str(module)
```

### Comparing `tinygrad-0.8.0/tinygrad/runtime/graph/cuda.py` & `tinygrad-0.9.0/tinygrad/runtime/graph/cuda.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,76 +1,81 @@
 import ctypes
 from typing import Any, Optional, Tuple, Dict, List, cast
-import gpuctypes.cuda as cuda
-from tinygrad.helpers import init_c_var, encode_args_cuda_style
-from tinygrad.device import CompiledASTRunner, update_stats, Buffer
-from tinygrad.runtime.ops_cuda import check, cu_time_execution
+import tinygrad.runtime.autogen.cuda as cuda
+from tinygrad.helpers import init_c_var, GraphException
+from tinygrad.device import Buffer, Device
+from tinygrad.runtime.ops_cuda import CUDADevice, check, encode_args, cu_time_execution
 from tinygrad.shape.symbolic import Variable
-from tinygrad.jit import JitItem, get_input_replace, get_jit_stats, get_jc_idxs_with_updatable_launch_dims, get_jc_idxs_with_updatable_var_vals, GraphException  # noqa: E501
+from tinygrad.engine.realize import ExecItem, BufferXfer, CompiledRunner
+from tinygrad.engine.jit import MultiGraphRunner
 
-class CUDAGraph:
-  def __init__(self, jit_cache: List[JitItem], input_rawbuffers: List[Buffer], var_vals: Dict[Variable, int]):
-    if not all(isinstance(ji.prg, CompiledASTRunner) for ji in jit_cache): raise GraphException
-
-    self.jit_cache = jit_cache
-    self.input_replace = get_input_replace(jit_cache, input_rawbuffers)
-    self.op_estimate, self.mem_estimate = get_jit_stats(jit_cache)
-    self.jc_idxs_with_updatable_launch_dims = get_jc_idxs_with_updatable_launch_dims(jit_cache)
-    self.jc_idxs_with_updatable_var_vals = get_jc_idxs_with_updatable_var_vals(jit_cache)
-    self.jc_idxs_with_updatable_rawbufs = list(set([x[0] for x in self.input_replace.keys()]))
-    self.updatable_nodes: Dict[int, Tuple[Any, Any, Any]] = {} # Dict[jc index] = tuple(graph node, node params, input kernel params)
+class CUDAGraph(MultiGraphRunner):
+  def __init__(self, jit_cache: List[ExecItem], input_rawbuffers: List[Buffer], var_vals: Dict[Variable, int]):
+    super().__init__(jit_cache, input_rawbuffers, var_vals)
 
-    self.graph = self.graph_create()
-    graph_node: Optional[ctypes._CData] = None
+    # Check all jit items are compatible.
+    if not all(isinstance(ji.prg, (CompiledRunner, BufferXfer)) for ji in jit_cache): raise GraphException
 
-    for (j,i),input_name in self.input_replace.items(): self.jit_cache[j].rawbufs[i] = input_rawbuffers[input_name]
-    for j,ji in enumerate(self.jit_cache):
-      prg: CompiledASTRunner = cast(CompiledASTRunner, ji.prg)
+    self.jc_idx_with_updatable_rawbufs = list(set([x[0] for x in self.input_replace.keys()]))
+    self.updatable_nodes: Dict[int, Tuple[Any, Any, Any, bool]] = {} # Dict[jc index] = tuple(graph node, node params, input kernel params, is memcpy)
+
+    self.graph = init_c_var(cuda.CUgraph(), lambda x: check(cuda.cuGraphCreate(ctypes.byref(x), 0)))
 
-      c_deps = (type(graph_node)*1)(*(graph_node,)) if graph_node is not None else None
-      c_kernel_input_config, c_input_params = encode_args_cuda_style([cast(Buffer, x)._buf for x in ji.rawbufs], [var_vals[x] for x in prg.vars], *self.encode_args_info())  # noqa: E501
-      c_node_params = self.build_kernel_node_params(prg, *cast(Tuple[List[int], List[int]], prg.launch_dims(var_vals)), c_kernel_input_config)
-      graph_node = self.graph_add_kernel_node(self.graph, c_deps, c_node_params)
+    for j,ji in enumerate(self.jit_cache):
+      if isinstance(ji.prg, CompiledRunner):
+        global_size, local_size = ji.prg.p.launch_dims(var_vals)
 
-      if j in self.jc_idxs_with_updatable_launch_dims or j in self.jc_idxs_with_updatable_var_vals or j in self.jc_idxs_with_updatable_rawbufs:
-        self.updatable_nodes[j] = (graph_node, c_node_params, c_input_params)
+        new_node = cuda.CUgraphNode()
+        deps = self._access_resources([x.base for x in ji.bufs[ji.prg.p.outcount:] if x is not None],
+                                      [x.base for x in ji.bufs[:ji.prg.p.outcount] if x is not None], new_dependency=new_node)
+        c_deps = (cuda.CUgraphNode*len(deps))(*deps) if deps else None
+
+        c_args, vargs = encode_args([cast(Buffer, x)._buf for x in ji.bufs], [var_vals[x] for x in ji.prg.p.vars])
+        kern_params = cuda.CUDA_KERNEL_NODE_PARAMS(ji.prg.clprg.prg, *global_size, *local_size, 0, None, vargs)
+        check(cuda.cuGraphAddKernelNode(ctypes.byref(new_node), self.graph, c_deps, len(deps), ctypes.byref(kern_params)))
+
+        if j in self.jc_idx_with_updatable_launch_dims or j in self.jc_idx_with_updatable_var_vals or j in self.jc_idx_with_updatable_rawbufs:
+          self.updatable_nodes[j] = (new_node, kern_params, c_args, False)
+      elif isinstance(ji.prg, BufferXfer):
+        dest, src = [cast(Buffer, x) for x in ji.bufs[0:2]]
+        src_dev = cast(CUDADevice, Device[src.device])
+        node_from = cuda.CUgraphNode()
+        deps = self._access_resources(read=[src.base], write=[dest.base], new_dependency=node_from)
+        c_deps = (cuda.CUgraphNode*len(deps))(*deps) if deps else None
+        cp_params = cuda.CUDA_MEMCPY3D_v2(srcMemoryType=cuda.CU_MEMORYTYPE_DEVICE, srcDevice=src._buf, srcPitch=src.nbytes, srcHeight=1,
+                                          dstMemoryType=cuda.CU_MEMORYTYPE_DEVICE, dstDevice=dest._buf, dstPitch=dest.nbytes, dstHeight=1,
+                                          WidthInBytes=dest.nbytes, Height=1, Depth=1)
+        check(cuda.cuGraphAddMemcpyNode(ctypes.byref(node_from), self.graph, c_deps, len(deps), ctypes.byref(cp_params), src_dev.context))
+        if j in self.jc_idx_with_updatable_rawbufs: self.updatable_nodes[j] = (node_from, cp_params, src_dev.context, True)
 
-    self.instance = self.graph_instantiate(self.graph)
+    self.instance = init_c_var(cuda.CUgraphExec(), lambda x: check(cuda.cuGraphInstantiate_v2(ctypes.byref(x), self.graph, None, None, 0)))
 
-  def __call__(self, input_rawbuffers: List[Buffer], var_vals: Dict[Variable, int], wait=False, jit=False) -> Optional[float]:
-    # Update rawbuffers in the c_input_params struct.
+  def __call__(self, input_rawbuffers: List[Buffer], var_vals: Dict[Variable, int], wait=False) -> Optional[float]:
+    # Update rawbuffers in the c_args struct.
     for (j,i),input_idx in self.input_replace.items():
-      setattr(self.updatable_nodes[j][2], f'f{i}', input_rawbuffers[input_idx]._buf)
-
-    # Update var_vals in the c_input_params struct.
-    for j in self.jc_idxs_with_updatable_var_vals:
-      for i,v in enumerate(cast(CompiledASTRunner, self.jit_cache[j].prg).vars):
-        setattr(self.updatable_nodes[j][2], f'f{len(self.jit_cache[j].rawbufs) + i}', var_vals[v])
-
-    # Update launch dims in the c_node_params struct.
-    for j in self.jc_idxs_with_updatable_launch_dims:
-      self.set_kernel_node_launch_dims(self.updatable_nodes[j][1], *cast(CompiledASTRunner, self.jit_cache[j].prg).launch_dims(var_vals))
+      if not self.updatable_nodes[j][3]: setattr(self.updatable_nodes[j][2], f'f{i}', input_rawbuffers[input_idx]._buf)
+      else:
+        if i == 0: self.updatable_nodes[j][1].destDevice = input_rawbuffers[input_idx]._buf
+        elif i == 1: self.updatable_nodes[j][1].srcDevice = input_rawbuffers[input_idx]._buf
+
+    # Update var_vals in the c_args struct.
+    for j in self.jc_idx_with_updatable_var_vals:
+      for i,v in enumerate(cast(CompiledRunner, self.jit_cache[j].prg).p.vars):
+        setattr(self.updatable_nodes[j][2], f'v{i}', var_vals[v])
+
+    # Update launch dims in the kern_params struct.
+    for j in self.jc_idx_with_updatable_launch_dims:
+      self.set_kernel_node_launch_dims(self.updatable_nodes[j][1], *cast(CompiledRunner, self.jit_cache[j].prg).p.launch_dims(var_vals))
 
     # Update graph nodes with the updated structs.
-    for node, c_node_params, _ in self.updatable_nodes.values():
-      self.graph_exec_kernel_node_set_params(self.instance, node, ctypes.byref(c_node_params))
+    for node, c_node_params, c_args, is_copy in self.updatable_nodes.values():
+      if not is_copy: check(cuda.cuGraphExecKernelNodeSetParams(self.instance, node, ctypes.byref(c_node_params)))
+      else: check(cuda.cuGraphExecMemcpyNodeSetParams(self.instance, node, ctypes.byref(c_node_params), c_args))
 
-    et = self.graph_launch(self.instance, None, wait=wait)
-    update_stats(f"<batched {len(self.jit_cache)}>", self.op_estimate, self.mem_estimate, var_vals, et, buf_count=len(input_rawbuffers), jit=jit, num_kernels=len(self.jit_cache))  # noqa: E501
-    return et
+    return cu_time_execution(lambda: check(cuda.cuGraphLaunch(self.instance, None)), enable=wait)
 
   def __del__(self):
-    check(cuda.cuGraphDestroy(self.graph))
-    check(cuda.cuGraphExecDestroy(self.instance))
+    if hasattr(self, 'graph'): check(cuda.cuGraphDestroy(self.graph))
+    if hasattr(self, 'instance'): check(cuda.cuGraphExecDestroy(self.instance))
 
-  def encode_args_info(self): return (cuda.CUdeviceptr_v2, (1,2,0))
-  def graph_create(self): return init_c_var(cuda.CUgraph(), lambda x: check(cuda.cuGraphCreate(ctypes.byref(x), 0)))
-  def graph_instantiate(self, graph):
-    return init_c_var(cuda.CUgraphExec(), lambda x: check(cuda.cuGraphInstantiate_v2(ctypes.byref(x), graph, None, None, 0)))
-  def graph_add_kernel_node(self, graph, c_deps, c_node_params):
-    return init_c_var(cuda.CUgraphNode(), lambda x: check(cuda.cuGraphAddKernelNode(ctypes.byref(x), graph, c_deps, ctypes.sizeof(c_deps)//8 if c_deps else 0, ctypes.byref(c_node_params))))  # noqa: E501
-  def graph_launch(self, *args, wait=False): return cu_time_execution(lambda: check(cuda.cuGraphLaunch(*args)), enable=wait)
-  def graph_exec_kernel_node_set_params(self, *args): return check(cuda.cuGraphExecKernelNodeSetParams(*args))
-  def build_kernel_node_params(self, prg, global_size, local_size, c_kernel_config):
-    return cuda.CUDA_KERNEL_NODE_PARAMS(prg.clprg.prg, *global_size, *local_size, 0, None, c_kernel_config)
   def set_kernel_node_launch_dims(self, node, global_size: Tuple[int, int, int], local_size: Tuple[int, int, int]):
     node.blockDimX, node.blockDimY, node.blockDimZ, node.gridDimX, node.gridDimY, node.gridDimZ = *local_size, *global_size
```

### Comparing `tinygrad-0.8.0/tinygrad/runtime/graph/metal.py` & `tinygrad-0.9.0/tinygrad/runtime/graph/metal.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,75 @@
 from typing import List, Any, Dict, cast, Optional
-import numpy as np
 import Metal
 from tinygrad.dtype import dtypes
-from tinygrad.helpers import dedup, unwrap2
-from tinygrad.device import Buffer, CompiledASTRunner, update_stats
-from tinygrad.jit import JitItem, get_input_replace, get_jit_stats, get_jc_idxs_with_updatable_launch_dims, GraphException
+from tinygrad.helpers import dedup, unwrap2, GraphException
+from tinygrad.device import Buffer
+from tinygrad.engine.realize import ExecItem, CompiledRunner
+from tinygrad.engine.jit import GraphRunner
 from tinygrad.shape.symbolic import Variable
-from tinygrad.runtime.ops_metal import MetalDevice
+from tinygrad.runtime.ops_metal import wait_check
 
-class MetalGraph:
-  def __init__(self, device:MetalDevice, jit_cache: List[JitItem], input_rawbuffers: List[Buffer], var_vals: Dict[Variable, int]):
-    if not all(isinstance(ji.prg, CompiledASTRunner) for ji in jit_cache): raise GraphException
-
-    self.jit_cache = jit_cache
-    self.input_replace = get_input_replace(jit_cache, input_rawbuffers)
-    self.op_estimate, self.mem_estimate = get_jit_stats(jit_cache)
-    self.jc_idx_with_updatable_launch_dims = get_jc_idxs_with_updatable_launch_dims(jit_cache)
-    self.device: MetalDevice = device
+class MetalGraph(GraphRunner):
+  def __init__(self, jit_cache: List[ExecItem], input_rawbuffers: List[Buffer], var_vals: Dict[Variable, int]):
+    super().__init__(jit_cache, input_rawbuffers, var_vals)
+    if not all(isinstance(ji.prg, CompiledRunner) for ji in jit_cache): raise GraphException
 
     # create metal batch exec
     icb_descriptor = Metal.MTLIndirectCommandBufferDescriptor.new()
     icb_descriptor.setCommandTypes_(Metal.MTLIndirectCommandType(Metal.MTLIndirectCommandTypeConcurrentDispatch))
     icb_descriptor.setInheritBuffers_(False)
     icb_descriptor.setInheritPipelineState_(False)
     icb_descriptor.setMaxKernelBufferBindCount_(31)
-    self.icb = self.device.device.newIndirectCommandBufferWithDescriptor_maxCommandCount_options_(icb_descriptor, len(self.jit_cache), Metal.MTLResourceOptions(0))  # noqa: E501
+    self.icb = self.device.device.newIndirectCommandBufferWithDescriptor_maxCommandCount_options_(icb_descriptor, len(self.jit_cache),
+                                                                                                  Metal.MTLResourceOptions(0))
     if self.icb is None: raise GraphException("create indirect command buffer failed, does your system support this?")
 
-    if len(var_vals): self.int_buf = self.device.allocator.alloc(len(var_vals)*dtypes.int32.itemsize)
-    all_resources = [self.int_buf] if len(var_vals) else []
+    if len(self.vars): self.int_buf = self.device.allocator.alloc(len(self.vars)*dtypes.int32.itemsize)
+    all_resources = [self.int_buf] if len(self.vars) else []
+
     for j,ji in enumerate(self.jit_cache):
-      prg: CompiledASTRunner = cast(CompiledASTRunner, ji.prg)
+      prg: CompiledRunner = cast(CompiledRunner, ji.prg)
       descriptor = Metal.MTLComputePipelineDescriptor.new()
       descriptor.setComputeFunction_(prg.clprg.fxn)
       descriptor.setSupportIndirectCommandBuffers_(True)
-      pipeline_state = unwrap2(self.device.device.newComputePipelineStateWithDescriptor_options_reflection_error_(descriptor, Metal.MTLPipelineOption(0), None, None))  # noqa: E501
       icb_command = self.icb.indirectComputeCommandAtIndex_(j)
-      icb_command.setComputePipelineState_(pipeline_state)
-      for i,b in enumerate(ji.rawbufs):
+      icb_command.setComputePipelineState_(unwrap2(
+        self.device.device.newComputePipelineStateWithDescriptor_options_reflection_error_(descriptor, Metal.MTLPipelineOption(0), None, None)))
+      for i,b in enumerate(ji.bufs):
         if b is not None:
           icb_command.setKernelBuffer_offset_atIndex_(b._buf, 0, i)
           all_resources.append(b._buf)
-      var_vals_keys = list(var_vals.keys())
-      for i,v in enumerate(prg.vars):
-        icb_command.setKernelBuffer_offset_atIndex_(self.int_buf, var_vals_keys.index(v)*4, len(ji.rawbufs)+i)
+      for i,v in enumerate(prg.p.vars): icb_command.setKernelBuffer_offset_atIndex_(self.int_buf, self.vars.index(v)*4, len(ji.bufs)+i)
       if j not in self.jc_idx_with_updatable_launch_dims:
-        global_size, local_size = prg.launch_dims(var_vals)
+        global_size, local_size = prg.p.launch_dims(var_vals)
         icb_command.concurrentDispatchThreadgroups_threadsPerThreadgroup_(Metal.MTLSize(*global_size), Metal.MTLSize(*local_size))
       icb_command.setBarrier()
+
     self.all_resources = dedup(all_resources)
     self.command_buffer: Any = None
-    if len(var_vals): self.int_buf_view = np.frombuffer(self.int_buf.contents().as_buffer(self.int_buf.length()), np.int32)
+    if len(self.vars): self.int_buf_view = self.int_buf.contents().as_buffer(self.int_buf.length()).cast('i')
+
+  def __call__(self, input_rawbuffers: List[Buffer], var_vals: Dict[Variable, int], wait=False) -> Optional[float]:
+    if self.command_buffer is not None and self.command_buffer in self.device.mtl_buffers_in_flight: wait_check(self.command_buffer)
+    all_resources = dedup(self.all_resources + [x._buf for x in input_rawbuffers])
 
-  def __call__(self, input_rawbuffers: List[Buffer], var_vals: Dict[Variable, int], wait=False, jit=False) -> Optional[float]:
-    # NOTE: you at least can't update the ints if this is running
-    if self.command_buffer is not None and self.command_buffer in self.device.mtl_buffers_in_flight: self.command_buffer.waitUntilCompleted()
-    all_resources = self.all_resources + [x._buf for x in input_rawbuffers]
     for (j,i),input_idx in self.input_replace.items():
       self.icb.indirectComputeCommandAtIndex_(j).setKernelBuffer_offset_atIndex_(input_rawbuffers[input_idx]._buf, 0, i)
     for j in self.jc_idx_with_updatable_launch_dims:
-      global_size, local_size = cast(CompiledASTRunner, self.jit_cache[j].prg).launch_dims(var_vals)
-      self.icb.indirectComputeCommandAtIndex_(j).concurrentDispatchThreadgroups_threadsPerThreadgroup_(Metal.MTLSize(*global_size), Metal.MTLSize(*local_size))  # noqa: E501
-    if len(var_vals): self.int_buf_view[:] = list(var_vals.values())
+      global_size, local_size = cast(CompiledRunner, self.jit_cache[j].prg).p.launch_dims(var_vals)
+      self.icb.indirectComputeCommandAtIndex_(j).concurrentDispatchThreadgroups_threadsPerThreadgroup_(Metal.MTLSize(*global_size),
+                                                                                                       Metal.MTLSize(*local_size))
+    for j, var in enumerate(self.vars): self.int_buf_view[j] = var_vals[var]
+
     command_buffer = self.device.mtl_queue.commandBuffer()
     encoder = command_buffer.computeCommandEncoder()
     encoder.useResources_count_usage_(all_resources, len(all_resources), Metal.MTLResourceUsageRead | Metal.MTLResourceUsageWrite)
-    encoder.executeCommandsInBuffer_withRange_(self.icb, Metal.MTLIndirectCommandBufferExecutionRangeMake(0,len(self.jit_cache)))
+    encoder.executeCommandsInBuffer_withRange_(self.icb, Metal.MTLIndirectCommandBufferExecutionRangeMake(0, len(self.jit_cache)))
     encoder.endEncoding()
     command_buffer.commit()
     self.command_buffer = command_buffer
+
     if wait:
-      command_buffer.waitUntilCompleted()
-      et = command_buffer.GPUEndTime() - command_buffer.GPUStartTime()
-    else:
-      self.device.mtl_buffers_in_flight.append(command_buffer)
-      et = None
-    update_stats(f"<batched {len(self.jit_cache)}>", self.op_estimate, self.mem_estimate, var_vals, et, buf_count=len(input_rawbuffers), jit=jit, num_kernels=len(self.jit_cache))  # noqa: E501
-    return et
+      wait_check(command_buffer)
+      return command_buffer.GPUEndTime() - command_buffer.GPUStartTime()
+    self.device.mtl_buffers_in_flight.append(command_buffer)
+    return None
```

### Comparing `tinygrad-0.8.0/tinygrad/runtime/ops_gpu.py` & `tinygrad-0.9.0/tinygrad/runtime/ops_gpu.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,101 +1,103 @@
 from __future__ import annotations
-from typing import Tuple, Optional, List
-import ctypes, functools
-import gpuctypes.opencl as cl
+from typing import Tuple, Optional, List, cast
+import ctypes, functools, hashlib
+import tinygrad.runtime.autogen.opencl as cl
 from tinygrad.helpers import init_c_var, to_char_p_p, from_mv, OSX, DEBUG
-from tinygrad.dtype import ImageDType
-from tinygrad.codegen.kernel import LinearizerOptions
 from tinygrad.renderer.cstyle import OpenCLRenderer
-from tinygrad.device import Compiled, LRUAllocator
+from tinygrad.device import BufferOptions, LRUAllocator, Compiled, Compiler, CompileError
 
 # see test/external/external_osx_profiling.py to determine this ratio. it's in like GPU clocks or something
 OSX_TIMING_RATIO = (125/3) if OSX else 1.0
 
 def check(status):
   if status != 0: raise RuntimeError(f"OpenCL Error {status}")
 def checked(ret, status): return (check(status.value), ret)[1]
 
-def compile_cl(prg:str) -> bytes:
-  assert CLDevice.compiler_context is not None, 'OpenCL requires a "compiler_context" to compile, init a device before you call this'
-  program = checked(cl.clCreateProgramWithSource(CLDevice.compiler_context.context, 1, to_char_p_p([prg_bytes := prg.encode()]),
-                                                 ctypes.byref(ctypes.c_size_t(len(prg_bytes))), ctypes.byref(status := ctypes.c_int32())), status)
-  status = cl.clBuildProgram(program, 1, ctypes.byref(CLDevice.compiler_context.device_id), None, cl.clBuildProgram.argtypes[4](), None)
-  if status != 0:
-    cl.clGetProgramBuildInfo(program, CLDevice.compiler_context.device_id, cl.CL_PROGRAM_BUILD_LOG, 0, None, ctypes.byref(log_size := ctypes.c_size_t()))  # noqa: E501
-    cl.clGetProgramBuildInfo(program, CLDevice.compiler_context.device_id, cl.CL_PROGRAM_BUILD_LOG, log_size.value, mstr := ctypes.create_string_buffer(log_size.value), None)  # noqa: E501
-    raise RuntimeError(f"OpenCL Compile Error\n\n{ctypes.string_at(mstr, size=log_size.value).decode()}")
-  binary_sizes = init_c_var((ctypes.c_size_t * 1)(), lambda x: check(cl.clGetProgramInfo(program, cl.CL_PROGRAM_BINARY_SIZES, ctypes.sizeof(x), ctypes.byref(x), None)))  # noqa: E501
-  binary = init_c_var(ctypes.create_string_buffer(binary_sizes[0]), lambda x: check(cl.clGetProgramInfo(program, cl.CL_PROGRAM_BINARIES, ctypes.sizeof(ctypes.c_void_p), ctypes.byref((ctypes.c_void_p * 1)(ctypes.addressof(x))), None)))  # noqa: E501
-  check(cl.clReleaseProgram(program))
-  return bytes(binary)
+class CLCompiler(Compiler):
+  def __init__(self, device:CLDevice, compile_key:str):
+    self.device = device
+    super().__init__(f"compile_cl_{compile_key}")
+  def compile(self, src:str) -> bytes:
+    program = checked(cl.clCreateProgramWithSource(self.device.context, 1, to_char_p_p([src.encode()]), None, status := ctypes.c_int32()), status)
+    build_status: int = cl.clBuildProgram(program, 1, self.device.device_id, None, cl.clBuildProgram.argtypes[4](), None)
+    if build_status != 0:
+      cl.clGetProgramBuildInfo(program, self.device.device_id, cl.CL_PROGRAM_BUILD_LOG, 0, None, log_size := ctypes.c_size_t())
+      cl.clGetProgramBuildInfo(program, self.device.device_id, cl.CL_PROGRAM_BUILD_LOG, log_size.value, mstr := ctypes.create_string_buffer(log_size.value), None)  # noqa: E501
+      raise CompileError(f"OpenCL Compile Error\n\n{mstr.value.decode()}")
+    check(cl.clGetProgramInfo(program, cl.CL_PROGRAM_BINARY_SIZES, ctypes.sizeof(ctypes.c_size_t), binary_sizes := (ctypes.c_size_t * 1)(), None))
+    check(cl.clGetProgramInfo(program, cl.CL_PROGRAM_BINARIES, ctypes.sizeof(ctypes.c_void_p), (ctypes.c_void_p * 1)(ctypes.addressof(binary := ctypes.create_string_buffer(binary_sizes[0]))), None))  # noqa: E501
+    check(cl.clReleaseProgram(program))
+    return bytes(binary)
 
 class CLProgram:
   def __init__(self, device:CLDevice, name:str, lib:bytes):
     self.device, self.name, self.lib = device, name, lib
-    self.program = checked(cl.clCreateProgramWithBinary(device.context, 1, ctypes.byref(device.device_id), (ctypes.c_size_t * 1)(len(lib)),
-                                                        to_char_p_p([lib], ctypes.c_ubyte), ctypes.byref(binary_status := ctypes.c_int32()),
-                                                        ctypes.byref(errcode_ret := ctypes.c_int32())), errcode_ret)
+    self.program = checked(cl.clCreateProgramWithBinary(device.context, 1, device.device_id, (ctypes.c_size_t * 1)(len(lib)),
+                                                        to_char_p_p([lib], ctypes.c_ubyte), binary_status := ctypes.c_int32(),
+                                                        errcode_ret := ctypes.c_int32()), errcode_ret)
     check(binary_status.value)
-    check(cl.clBuildProgram(self.program, 1, ctypes.byref(device.device_id), None, cl.clBuildProgram.argtypes[4](), None)) # NOTE: OSX requires this
-    self.kernel = checked(cl.clCreateKernel(self.program, name.encode(), ctypes.byref(status := ctypes.c_int32())), status)
+    check(cl.clBuildProgram(self.program, 1, device.device_id, None, cl.clBuildProgram.argtypes[4](), None)) # NOTE: OSX requires this
+    self.kernel = checked(cl.clCreateKernel(self.program, name.encode(), status := ctypes.c_int32()), status)
 
   def __del__(self):
-    check(cl.clReleaseKernel(self.kernel))
-    check(cl.clReleaseProgram(self.program))
+    if hasattr(self, 'kernel'): check(cl.clReleaseKernel(self.kernel))
+    if hasattr(self, 'program'): check(cl.clReleaseProgram(self.program))
 
-  def __call__(self, *bufs:cl.cl_mem, global_size:Tuple[int,...], local_size:Optional[Tuple[int,...]]=None, vals:Tuple[int, ...]=(), wait=False) -> Optional[float]:  # noqa: E501
+  def __call__(self, *bufs:ctypes._CData, global_size:Tuple[int,int,int]=(1,1,1), local_size:Optional[Tuple[int,int,int]]=None, vals:Tuple[int, ...]=(), wait=False) -> Optional[float]:  # noqa: E501
     for i,b in enumerate(bufs): cl.clSetKernelArg(self.kernel, i, ctypes.sizeof(b), ctypes.byref(b))
-    for i,b in enumerate(vals,start=len(bufs)): cl.clSetKernelArg(self.kernel, i, 4, ctypes.byref(ctypes.c_int32(b)))
-    if local_size is not None: global_size = tuple(int(g*l) for g,l in zip(global_size, local_size))
+    for i,v in enumerate(vals,start=len(bufs)): cl.clSetKernelArg(self.kernel, i, 4, ctypes.byref(ctypes.c_int32(v)))
+    if local_size is not None: global_size = cast(Tuple[int,int,int], tuple(int(g*l) for g,l in zip(global_size, local_size)))
     event = cl.cl_event() if wait else None
     check(cl.clEnqueueNDRangeKernel(self.device.queue, self.kernel, len(global_size), None, (ctypes.c_size_t * len(global_size))(*global_size), (ctypes.c_size_t * len(local_size))(*local_size) if local_size else None, 0, None, event))  # noqa: E501
     if wait:
-      check(cl.clWaitForEvents(1, ctypes.byref(event)))
-      start = init_c_var(ctypes.c_uint64(), lambda x: check(cl.clGetEventProfilingInfo(event, cl.CL_PROFILING_COMMAND_START, ctypes.sizeof(x), ctypes.byref(x), None)))  # noqa: E501
-      end = init_c_var(ctypes.c_uint64(), lambda x: check(cl.clGetEventProfilingInfo(event, cl.CL_PROFILING_COMMAND_END, ctypes.sizeof(x), ctypes.byref(x), None)))  # noqa: E501
+      assert event is not None
+      check(cl.clWaitForEvents(1, event))
+      check(cl.clGetEventProfilingInfo(event, cl.CL_PROFILING_COMMAND_START, 8, ctypes.byref(start := ctypes.c_uint64()), None))
+      check(cl.clGetEventProfilingInfo(event, cl.CL_PROFILING_COMMAND_END, 8, ctypes.byref(end := ctypes.c_uint64()), None))
       return float(end.value-start.value) * OSX_TIMING_RATIO * 1e-9
     return None
 
 class CLAllocator(LRUAllocator):
   def __init__(self, device:CLDevice):
     self.device = device
     super().__init__()
-  def _alloc(self, size:int) -> cl.cl_mem:
-    return checked(cl.clCreateBuffer(self.device.context, cl.CL_MEM_READ_WRITE, size, None, ctypes.byref(status := ctypes.c_int32())), status)
-  def _alloc_image(self, dtype:ImageDType) -> cl.cl_mem:
-    return checked(cl.clCreateImage2D(self.device.context, cl.CL_MEM_READ_WRITE,
-                                      cl.cl_image_format(cl.CL_RGBA, {2: cl.CL_HALF_FLOAT, 4: cl.CL_FLOAT}[dtype.itemsize]),
-                                      dtype.shape[1], dtype.shape[0], 0, None, ctypes.byref(status := ctypes.c_int32())), status)
-  def _free(self, buf:cl.cl_mem): check(cl.clReleaseMemObject(buf))
-  def copyin(self, dest:cl.cl_mem, src:memoryview):
+  def _alloc(self, size:int, options:BufferOptions) -> ctypes._CData:
+    if options.image is not None:
+      return checked(cl.clCreateImage2D(self.device.context, cl.CL_MEM_READ_WRITE,
+                                        cl.cl_image_format(cl.CL_RGBA, {2: cl.CL_HALF_FLOAT, 4: cl.CL_FLOAT}[options.image.itemsize]),
+                                        options.image.shape[1], options.image.shape[0], 0, None, status := ctypes.c_int32()), status)
+    else: return checked(cl.clCreateBuffer(self.device.context, cl.CL_MEM_READ_WRITE, size, None, status := ctypes.c_int32()), status)
+  def _free(self, buf:ctypes._CData, options:BufferOptions): check(cl.clReleaseMemObject(buf))
+  def copyin(self, dest:ctypes._CData, src:memoryview):
     check(cl.clEnqueueWriteBuffer(self.device.queue, dest, False, 0, len(src)*src.itemsize, from_mv(src), 0, None, None))
     self.device.pending_copyin.append(src)    # NOTE: these can't be freed until the GPU actually executes this command
-  def copyout(self, dest:memoryview, src:cl.cl_mem):
+  def copyout(self, dest:memoryview, src:ctypes._CData):
     check(cl.clEnqueueReadBuffer(self.device.queue, src, False, 0, len(dest)*dest.itemsize, from_mv(dest), 0, None, None))
     self.device.synchronize()
 
 class CLDevice(Compiled):
   device_ids = None                 # this is global and only initted once
-  compiler_context = None           # this is the first created context. we make an assumption they are all the same for the compiler
   def __init__(self, device:str=""):
     if CLDevice.device_ids is None:
-      num_platforms = init_c_var(ctypes.c_uint32(), lambda x: check(cl.clGetPlatformIDs(0, None, ctypes.byref(x))))
-      platform_ids = init_c_var((cl.cl_platform_id * num_platforms.value)(), lambda x: check(cl.clGetPlatformIDs(num_platforms.value, x, None)))
+      check(cl.clGetPlatformIDs(0, None, num_platforms := ctypes.c_uint32()))
+      check(cl.clGetPlatformIDs(num_platforms.value, platform_ids := (cl.cl_platform_id * num_platforms.value)(), None))
       for device_type in [cl.CL_DEVICE_TYPE_GPU, cl.CL_DEVICE_TYPE_DEFAULT]:
-        num_devices = ctypes.c_uint32()
-        err = cl.clGetDeviceIDs(platform_ids[0], device_type, 0, None, ctypes.byref(num_devices))
+        err = cl.clGetDeviceIDs(platform_ids[0], device_type, 0, None, num_devices := ctypes.c_uint32())
         if err == 0 and num_devices.value != 0: break
       if DEBUG >= 1: print(f"CLDevice: got {num_platforms.value} platforms and {num_devices.value} devices")
       CLDevice.device_ids = init_c_var((cl.cl_device_id * num_devices.value)(), lambda x: check(cl.clGetDeviceIDs(platform_ids[0], device_type, num_devices, x, None)))  # noqa: E501
 
     self.device_id = CLDevice.device_ids[0 if ":" not in device else int(device.split(":")[1])]
-    self.context = checked(cl.clCreateContext(None, 1, ctypes.byref(self.device_id), cl.clCreateContext.argtypes[3](), None, ctypes.byref(status := ctypes.c_int32())), status)  # noqa: E501
-    if CLDevice.compiler_context is None: CLDevice.compiler_context = self
-    self.queue = checked(cl.clCreateCommandQueue(self.context, self.device_id, cl.CL_QUEUE_PROFILING_ENABLE, ctypes.byref(status)), status)
+    self.device_name = (cl.clGetDeviceInfo(self.device_id, cl.CL_DEVICE_NAME, 256, buf := ctypes.create_string_buffer(256), None), buf.value.decode())[1]  # noqa: E501
+    self.driver_version = (cl.clGetDeviceInfo(self.device_id, cl.CL_DRIVER_VERSION, 256, buf := ctypes.create_string_buffer(256), None), buf.value.decode())[1]  # noqa: E501
+    self.context = checked(cl.clCreateContext(None, 1, self.device_id, cl.clCreateContext.argtypes[3](), None, status := ctypes.c_int32()), status)
+    self.queue = checked(cl.clCreateCommandQueue(self.context, self.device_id, cl.CL_QUEUE_PROFILING_ENABLE, status), status)
     self.pending_copyin: List[memoryview] = []
-    super().__init__(CLAllocator(self), LinearizerOptions(), OpenCLRenderer, compile_cl, functools.partial(CLProgram, self))
+
+    compile_key = hashlib.md5(self.device_name.encode() + self.driver_version.encode()).hexdigest()
+    super().__init__(device, CLAllocator(self), OpenCLRenderer(), CLCompiler(self, f"compile_cl_{compile_key}"), functools.partial(CLProgram, self))
   def synchronize(self):
     check(cl.clFinish(self.queue))
     self.pending_copyin.clear()
 
 GPUDevice = CLDevice # for legacy reasons
```

### Comparing `tinygrad-0.8.0/tinygrad/runtime/ops_metal.py` & `tinygrad-0.9.0/tinygrad/runtime/ops_metal.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,88 +1,106 @@
 from __future__ import annotations
 import os, subprocess, pathlib, ctypes, tempfile, functools
 import Metal, libdispatch
-from typing import List, Any, Tuple, Optional
-from tinygrad.codegen.kernel import LinearizerOptions
+from typing import List, Set, Any, Tuple, Optional
 from tinygrad.helpers import prod, getenv, DEBUG, unwrap2
-from tinygrad.device import Compiled, LRUAllocator
+from tinygrad.device import Compiled, Compiler, CompileError, LRUAllocator
 from tinygrad.renderer.cstyle import MetalRenderer
 
-def compile_metal(prg, use_xcode=bool(getenv("METAL_XCODE"))) -> bytes:
-  assert MetalDevice.compiler_device, "metal device creation is required for metal compile"
-  if use_xcode:
-    # NOTE: if you run llvm-dis on "air" you can see the llvm bytecode
-    air = subprocess.check_output(['xcrun', '-sdk', 'macosx', 'metal', '-x', 'metal', '-c', '-', '-o', '-'], input=prg.encode('utf-8'))
-    return subprocess.check_output(['xcrun', '-sdk', 'macosx', 'metallib', '-', '-o', '-'], input=air)
-  options = Metal.MTLCompileOptions.new()
-  library = unwrap2(MetalDevice.compiler_device.newLibraryWithSource_options_error_(prg, options, None))
-  return library.libraryDataContents().bytes().tobytes()
+def wait_check(cbuf: Any):
+  cbuf.waitUntilCompleted()
+  if (error := cbuf.error()) is not None:
+    raise RuntimeError(error)
+
+class MetalCompiler(Compiler):
+  def __init__(self, device:Optional[MetalDevice]):
+    self.device = device
+    super().__init__("compile_metal")
+  def compile(self, src:str) -> bytes:
+    if self.device is None:
+      # NOTE: if you run llvm-dis on "air" you can see the llvm bytecode
+      air = subprocess.check_output(['xcrun', '-sdk', 'macosx', 'metal', '-x', 'metal', '-c', '-', '-o', '-'], input=src.encode('utf-8'))
+      return subprocess.check_output(['xcrun', '-sdk', 'macosx', 'metallib', '-', '-o', '-'], input=air)
+    else:
+      options = Metal.MTLCompileOptions.new()
+      options.setFastMathEnabled_(getenv("METAL_FAST_MATH"))
+      try: library = unwrap2(self.device.device.newLibraryWithSource_options_error_(src, options, None))
+      except AssertionError as e: raise CompileError(e)
+      return library.libraryDataContents().bytes().tobytes()
 
 class MetalProgram:
   def __init__(self, device:MetalDevice, name:str, lib:bytes):
     self.device, self.name, self.lib = device, name, lib
     if DEBUG >= 6:
       with tempfile.NamedTemporaryFile(delete=True) as shader:
         shader.write(lib)
         shader.flush()
-        os.system(f"cd {pathlib.Path(__file__).parents[2]}/disassemblers/applegpu && python3 compiler_explorer.py {shader.name}")
+        os.system(f"cd {pathlib.Path(__file__).parents[2]}/extra/disassemblers/applegpu && python3 compiler_explorer.py {shader.name}")
+    assert lib[:4] == b"MTLB", "Invalid Metal library. Could be due to using conda. Try system python or METAL_XCODE=1 DISABLE_COMPILER_CACHE=1."
     data = libdispatch.dispatch_data_create(lib, len(lib), None, None)
     self.library = unwrap2(self.device.device.newLibraryWithData_error_(data, None))
     self.fxn = self.library.newFunctionWithName_(name)
     self.pipeline_state = unwrap2(self.device.device.newComputePipelineStateWithFunction_error_(self.fxn, None))
 
-  def __call__(self, *bufs, global_size:Tuple[int,int,int], local_size:Tuple[int,int,int], vals:Tuple[int, ...]=(), wait=False):
-    assert prod(local_size) <= self.pipeline_state.maxTotalThreadsPerThreadgroup(),f"local size {local_size} bigger than {self.pipeline_state.maxTotalThreadsPerThreadgroup()} with exec width {self.pipeline_state.threadExecutionWidth()} memory length {self.pipeline_state.staticThreadgroupMemoryLength()}"  # noqa: E501
+  def __call__(self, *bufs, global_size:Tuple[int,int,int]=(1,1,1), local_size:Tuple[int,int,int]=(1,1,1), vals:Tuple[int, ...]=(), wait=False):
+    if prod(local_size) > self.pipeline_state.maxTotalThreadsPerThreadgroup(): raise RuntimeError(f"local size {local_size} bigger than {self.pipeline_state.maxTotalThreadsPerThreadgroup()} with exec width {self.pipeline_state.threadExecutionWidth()} memory length {self.pipeline_state.staticThreadgroupMemoryLength()}")  # noqa: E501
     command_buffer = self.device.mtl_queue.commandBuffer()
     encoder = command_buffer.computeCommandEncoder()
     encoder.setComputePipelineState_(self.pipeline_state)
     for i,a in enumerate(bufs): encoder.setBuffer_offset_atIndex_(a, 0, i)
     for i,a in enumerate(vals,start=len(bufs)): encoder.setBytes_length_atIndex_(ctypes.c_int32(a), 4, i)
     encoder.dispatchThreadgroups_threadsPerThreadgroup_(Metal.MTLSize(*global_size), Metal.MTLSize(*local_size))
     encoder.endEncoding()
     command_buffer.commit()
     if wait:
-      command_buffer.waitUntilCompleted()
+      wait_check(command_buffer)
       return command_buffer.GPUEndTime() - command_buffer.GPUStartTime()
     self.device.mtl_buffers_in_flight.append(command_buffer)
 
 class MetalAllocator(LRUAllocator):
   def __init__(self, device:MetalDevice):
     self.device:MetalDevice = device
+    self.track_cross_device: Set[MetalDevice] = set()
     super().__init__()
-  def _alloc(self, size:int) -> Any:
+  def free_cache(self):
+    self.device.synchronize()
+    for x in self.track_cross_device: x.synchronize()
+    self.track_cross_device.clear()
+    return super().free_cache()
+  def _alloc(self, size:int, options) -> Any:
     ret = self.device.device.newBufferWithLength_options_(size, Metal.MTLResourceStorageModeShared)
     if ret is None: raise MemoryError(f"Metal OOM while allocating {size=}")
     return ret
-  def transfer(self, dest:Any, src:Any, sz:int):
+  def transfer(self, dest:Any, src:Any, sz:int, src_dev: MetalDevice, **kwargs):
+    src_dev.synchronize()
     command_buffer = self.device.mtl_queue.commandBuffer()
     encoder = command_buffer.blitCommandEncoder()
     encoder.copyFromBuffer_sourceOffset_toBuffer_destinationOffset_size_(src, 0, dest, 0, sz)
     encoder.endEncoding()
     command_buffer.commit()
     self.device.mtl_buffers_in_flight.append(command_buffer)
   def from_buffer(self, src:memoryview) -> Optional[Any]:
     ret = self.device.device.newBufferWithBytesNoCopy_length_options_deallocator_(src, len(src), Metal.MTLResourceStorageModeShared, None)
     if ret: self.device.mv_in_metal.append(src)
     return ret
-  def _free(self, opaque:Any): opaque.release()
+  def _free(self, opaque:Any, options): opaque.release()
   def as_buffer(self, src:Any) -> memoryview:
     self.device.synchronize()
     return src.contents().as_buffer(src.length())
   def copyin(self, dest:Any, src:memoryview): self.as_buffer(dest)[:] = src
   def copyout(self, dest:memoryview, src:Any): dest[:] = self.as_buffer(src)
 
 class MetalDevice(Compiled):
-  compiler_device = None
   def __init__(self, device:str):
     self.device = Metal.MTLCreateSystemDefaultDevice()
-    if MetalDevice.compiler_device is None: MetalDevice.compiler_device = self.device
     self.mtl_queue = self.device.newCommandQueueWithMaxCommandBufferCount_(1024)
     self.mtl_buffers_in_flight: List[Any] = []
     self.mv_in_metal: List[memoryview] = []
+    self.track_cross_buffer: List[Any] = []
     from tinygrad.runtime.graph.metal import MetalGraph
-    super().__init__(MetalAllocator(self), LinearizerOptions(device="METAL"), MetalRenderer,
-                     compile_metal, functools.partial(MetalProgram, self), functools.partial(MetalGraph, self))
+    super().__init__(device, MetalAllocator(self), MetalRenderer(), MetalCompiler(None if getenv("METAL_XCODE") else self),
+                     functools.partial(MetalProgram, self), MetalGraph)
   def synchronize(self):
-    for cbuf in self.mtl_buffers_in_flight: cbuf.waitUntilCompleted()
+    for cbuf in self.mtl_buffers_in_flight: wait_check(cbuf)
     self.mv_in_metal.clear()
     self.mtl_buffers_in_flight.clear()
+    self.track_cross_buffer.clear()
```

### Comparing `tinygrad-0.8.0/tinygrad/shape/symbolic.py` & `tinygrad-0.9.0/tinygrad/shape/symbolic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,83 +1,76 @@
 from __future__ import annotations
 import functools
 from math import gcd
 from tinygrad.helpers import partition
-from typing import List, Dict, Callable, Tuple, Type, Union, Optional, Any, Set
+from typing import List, Dict, Callable, Tuple, Type, Union, Optional, Any, Set, Mapping
 
 # NOTE: Python has different behavior for negative mod and floor div than c
 # symbolic matches the Python behavior, but the code output is agnostic, and will never have negative numbers in div or mod
 
 class Node:
   b: Union[Node, int]
   min: int
-  max: int
+  max: sint
   def render(self, ops=None, ctx=None) -> Any:
     if ops is None: ops = render_python
     assert self.__class__ in (Variable, NumNode) or self.min != self.max
     return ops[type(self)](self, ops, ctx)
   def vars(self) -> Set[Variable]: return set()
   # substitute Variables with the values in var_vals
-  def substitute(self, var_vals: Dict[Variable, Node]) -> Node: raise RuntimeError(self.__class__.__name__)
+  def substitute(self, var_vals: Mapping[Variable, Union[NumNode, Variable]]) -> Node: raise RuntimeError(self.__class__.__name__)
   def unbind(self) -> Tuple[Node, Optional[int]]: return self.substitute({v: v.unbind()[0] for v in self.vars() if v.val is not None}), None
 
   @functools.cached_property
   def key(self) -> str: return self.render(ctx="DEBUG")
   @functools.cached_property
   def hash(self) -> int: return hash(self.key)
   def __repr__(self): return self.render(ctx="REPR")
   def __str__(self): return "<"+self.key+">"
   def __hash__(self): return self.hash
   def __bool__(self): return not (self.max == self.min == 0)
   def __eq__(self, other:object) -> bool:
     if not isinstance(other, Node): return NotImplemented
     return self.key == other.key
   def __neg__(self): return self*-1
-  def __add__(self, b:Union[Node,int]): return Node.sum([self, b if isinstance(b, Node) else NumNode(b)])
+  def __add__(self, b:Union[Node,int]): return Node.sum([self, NumNode(b) if isinstance(b, int) else b])
   def __radd__(self, b:int): return self+b
   def __sub__(self, b:Union[Node,int]): return self+-b
   def __rsub__(self, b:int): return -self+b
   def __le__(self, b:Union[Node,int]): return self < (b+1)
   def __gt__(self, b:Union[Node,int]): return (-self) < (-b)
   def __ge__(self, b:Union[Node,int]): return (-self) < (-b+1)
   def __lt__(self, b:Union[Node,int]): return create_node(LtNode(self, b))
   def __mul__(self, b:Union[Node, int]):
     if b == 0: return NumNode(0)
     if b == 1: return self
-    if self.__class__ is NumNode: return NumNode(self.b*b) if isinstance(b, int) else b*self.b
     return create_node(MulNode(self, b.b)) if isinstance(b, NumNode) else create_node(MulNode(self, b))
   def __rmul__(self, b:int): return self*b
 
   # *** complex ops ***
 
-  def __rfloordiv__(self, b:int):
-    if self.min > b >= 0: return NumNode(0)
-    if isinstance(self, NumNode): return NumNode(b // self.b)
-    raise RuntimeError(f"not supported: {b} // {self}")
+  def __rfloordiv__(self, b:int): return NumNode(b) // self
   def __floordiv__(self, b:Union[Node,int], factoring_allowed=True):
     if isinstance(b, Node):
-      if b.__class__ is NumNode: return self // b.b
+      if b.__class__ is NumNode: return self.__floordiv__(b.b, factoring_allowed)
       if self == b: return NumNode(1)
       if (b - self).min > 0 and self.min >= 0: return NumNode(0) # b - self simplifies the node
       raise RuntimeError(f"not supported: {self} // {b}")
     assert b != 0
-    if b < 0: return (self//-b)*-1
+    if b < 0: return (self*-1).__floordiv__(-b, factoring_allowed)
     if b == 1: return self
 
     # the numerator of div is not allowed to be negative
     if self.min < 0:
       offset = self.min//b
       # factor out an "offset" to make the numerator positive. don't allowing factoring again
       return (self + -offset*b).__floordiv__(b, factoring_allowed=False) + offset
     return create_node(DivNode(self, b))
 
-  def __rmod__(self, b:int):
-    if self.min > b >= 0: return NumNode(b)
-    if isinstance(self, NumNode): return NumNode(b % self.b)
-    raise RuntimeError(f"not supported: {b} % {self}")
+  def __rmod__(self, b:int): return NumNode(b) % self
   def __mod__(self, b:Union[Node,int]):
     if isinstance(b, Node):
       if b.__class__ is NumNode: return self % b.b
       if self == b: return NumNode(0)
       if (b - self).min > 0 and self.min >= 0: return self # b - self simplifies the node
       raise RuntimeError(f"not supported: {self} % {b}")
     assert b > 0
@@ -98,229 +91,239 @@
     num_node_sum = 0
     for node in SumNode(nodes).flat_components:
       if node.__class__ is NumNode: num_node_sum += node.b
       elif node.__class__ is MulNode: mul_groups[node.a] = mul_groups.get(node.a, 0) + node.b
       else: mul_groups[node] = mul_groups.get(node, 0) + 1
     new_nodes = [MulNode(a, b_sum) if b_sum != 1 else a for a, b_sum in mul_groups.items() if b_sum != 0]
     if num_node_sum: new_nodes.append(NumNode(num_node_sum))
-    return create_rednode(SumNode, new_nodes) if len(new_nodes) > 1 else new_nodes[0] if len(new_nodes) == 1 else NumNode(0)
+    return create_node(SumNode(new_nodes)) if len(new_nodes) > 1 else new_nodes[0] if len(new_nodes) == 1 else NumNode(0)
 
   @staticmethod
   def ands(nodes:List[Node]) -> Node:
     if not nodes: return NumNode(1)
     if len(nodes) == 1: return nodes[0]
     if any(not x for x in nodes): return NumNode(0)
 
     # filter 1s
     nodes = [x for x in nodes if x.min != x.max]
-    return create_rednode(AndNode, nodes) if len(nodes) > 1 else (nodes[0] if len(nodes) == 1 else NumNode(1))
+    return create_node(AndNode(nodes)) if len(nodes) > 1 else (nodes[0] if len(nodes) == 1 else NumNode(1))
 
 # 4 basic node types
 
 class Variable(Node):
   def __new__(cls, *args):
-    if len(args) == 0: return super().__new__(cls)   # fix pickle
     expr, nmin, nmax = args
     assert nmin >= 0 and nmin <= nmax, f"invalid Variable {expr=} {nmin=} {nmax=}"
     if nmin == nmax: return NumNode(nmin)
     return super().__new__(cls)
 
-  def __init__(self, expr:Optional[str], nmin:int, nmax:int):
+  def __getnewargs__(self): return (self.expr, self.min, self.max)  # args passed to __new__ when unpickling
+
+  def __init__(self, expr:str, nmin:int, nmax:sint):
     self.expr, self.min, self.max = expr, nmin, nmax
     self._val: Optional[int] = None
   @property
   def val(self):
     assert self._val is not None, f"Variable isn't bound, can't access val of {self}"
     return self._val
   def bind(self, val):
     assert self._val is None and self.min<=val<=self.max, f"cannot bind {val} to {self}"
     self._val = val
     return self
   def unbind(self) -> Tuple[Variable, int]:
     assert self.val is not None, f"cannot unbind {self}"
     return Variable(self.expr, self.min, self.max), self.val
   def vars(self): return {self}
-  def substitute(self, var_vals: Dict[Variable, Node]) -> Node: return var_vals.get(self, self)
+  def substitute(self, var_vals: Mapping[Variable, Union[NumNode, Variable]]) -> Node: return var_vals.get(self, self)
 
 class NumNode(Node):
   def __init__(self, num:int):
     assert isinstance(num, int), f"{num} is not an int"
     self.b:int = num
     self.min, self.max = num, num
   def bind(self, val):
     assert self.b == val, f"cannot bind {val} to {self}"
     return self
+  def __mul__(self, b:Union[Node,int]): return NumNode(self.b*b) if isinstance(b, int) else b*self.b
   def __eq__(self, other): return self.b == other
-  def __hash__(self): return self.hash  # needed with __eq__ override
-  def substitute(self, var_vals: Dict[Variable, Node]) -> Node: return self
+  def __hash__(self): return hash(self.b)  # needed with __eq__ override
+  def substitute(self, var_vals: Mapping[Variable, Union[NumNode, Variable]]) -> Node: return self
 
 def create_node(ret:Node):
   assert ret.min <= ret.max, f"min greater than max! {ret.min} {ret.max} when creating {type(ret)} {ret}"
   if ret.min == ret.max: return NumNode(ret.min)
   return ret
 
+def create_lt_node(lhs:Node, b:Union[Node, int]):
+  if isinstance(lhs, SumNode):
+    if isinstance(b, int):
+      new_sum = []
+      for x in lhs.nodes:
+        # TODO: should we just force the last one to always be the number
+        if isinstance(x, NumNode): b -= x.b
+        else: new_sum.append(x)
+      lhs = Node.sum(new_sum)
+      nodes = lhs.nodes if isinstance(lhs, SumNode) else [lhs]
+      assert all(not isinstance(node, MulNode) or isinstance(node.b, int) for node in nodes), "not supported"
+      muls, others = partition(nodes, lambda x: isinstance(x, MulNode) and x.b > 0 and x.max >= b)
+      if muls:
+        # NOTE: gcd in python 3.8 takes exactly 2 args
+        mul_gcd = b
+        for x in muls: mul_gcd = gcd(mul_gcd, x.b)  # type: ignore  # mypy cannot tell that x.b is int here due to assert above
+        all_others = Node.sum(others)
+        if all_others.min >= 0 and all_others.max < mul_gcd:
+          lhs, b = Node.sum([mul//mul_gcd for mul in muls]), b//mul_gcd
+    return create_node(LtNode(lhs, b)) if isinstance(lhs, SumNode) else create_lt_node(lhs, b)
+  if isinstance(lhs, MulNode):
+    if isinstance(b, Node) or isinstance(lhs.b, Node) or lhs.b == -1: return create_node(LtNode(lhs, b))
+    sgn = 1 if lhs.b > 0 else -1
+    return create_node(LtNode(lhs.a*sgn, (b + abs(lhs.b) - 1)//abs(lhs.b)))
+  return create_node(LtNode(lhs, b))
+
+def create_ge_node(lhs:Node, b:Union[Node, int]): return create_lt_node(-lhs, -b+1)
+
 class OpNode(Node):
   def __init__(self, a:Node, b:Union[Node, int]):
     self.a, self.b = a, b
     self.min, self.max = self.get_bounds()
   def vars(self): return self.a.vars() | (self.b.vars() if isinstance(self.b, Node) else set())
-  def get_bounds(self) -> Tuple[int, int]: raise NotImplementedError("must be implemented")
+  def get_bounds(self) -> Tuple[int, sint]: raise NotImplementedError("must be implemented")
 
 class LtNode(OpNode):
-  def __floordiv__(self, b: Union[Node, int], _=False): return (self.a//b) < (self.b//b)
   def get_bounds(self) -> Tuple[int, int]:
+    if self.a == self.b: return (0, 0)
     if isinstance(self.b, int): return (1, 1) if self.a.max < self.b else (0, 0) if self.a.min >= self.b else (0, 1)
     return (1, 1) if self.a.max < self.b.min else (0, 0) if self.a.min >= self.b.max else (0, 1)
-  def substitute(self, var_vals: Dict[Variable, Node]) -> Node:
-    return self.a.substitute(var_vals) < (self.b if isinstance(self.b, int) else self.b.substitute(var_vals))
+  def substitute(self, var_vals: Mapping[Variable, Union[NumNode, Variable]]) -> Node:
+    return create_lt_node(self.a.substitute(var_vals), (self.b if isinstance(self.b, int) else self.b.substitute(var_vals)))
 
 class MulNode(OpNode):
-  def __lt__(self, b: Union[Node, int]):
-    if isinstance(b, Node) or isinstance(self.b, Node) or self.b == -1: return Node.__lt__(self, b)
-    sgn = 1 if self.b > 0 else -1
-    return Node.__lt__(self.a*sgn, (b + abs(self.b) - 1)//abs(self.b))
   def __mul__(self, b: Union[Node, int]): return self.a*(self.b*b) # two muls in one mul
   def __floordiv__(self, b: Union[Node, int], factoring_allowed=False): # NOTE: mod negative isn't handled right
     if self.b % b == 0: return self.a*(self.b//b)
     if b % self.b == 0 and self.b > 0: return self.a//(b//self.b)
     return Node.__floordiv__(self, b, factoring_allowed)
   def __mod__(self, b: Union[Node, int]): return Node.__mod__(self.a * (self.b%b), b)
-  def get_bounds(self) -> Tuple[int, int]: return (self.a.min*self.b, self.a.max*self.b) if self.b >= 0 else (self.a.max*self.b, self.a.min*self.b)
-  def substitute(self, var_vals: Dict[Variable, Node]) -> Node:
+  def get_bounds(self) -> Tuple[int, sint]:
+    assert self.a.min >= 0
+    if isinstance(self.b, int): return (self.a.min*self.b, self.a.max*self.b) if self.b >= 0 else (self.a.max*self.b, self.a.min*self.b)
+    return (self.a.min*self.b.min, self.a.max*self.b.max) if self.b.min >= 0 else (self.a.max*self.b.min, self.a.min*self.b.max)
+  def substitute(self, var_vals: Mapping[Variable, Union[NumNode, Variable]]) -> Node:
     return self.a.substitute(var_vals) * (self.b if isinstance(self.b, int) else self.b.substitute(var_vals))
 
 class DivNode(OpNode):
   def __floordiv__(self, b: Union[Node, int], _=False): return self.a//(self.b*b) # two divs is one div
-  def get_bounds(self) -> Tuple[int, int]:
+  def get_bounds(self) -> Tuple[int, sint]:
     assert self.a.min >= 0 and isinstance(self.b, int)
     return self.a.min//self.b, self.a.max//self.b
-  def substitute(self, var_vals: Dict[Variable, Node]) -> Node: return self.a.substitute(var_vals) // self.b
+  def substitute(self, var_vals: Mapping[Variable, Union[NumNode, Variable]]) -> Node: return self.a.substitute(var_vals) // self.b
 
 class ModNode(OpNode):
   def __mod__(self, b: Union[Node, int]):
-    if isinstance(b, Node) or isinstance(self.b, Node): return Node.__mod__(self, b)
-    return self.a % b if self.b % b == 0 else Node.__mod__(self, b)
+    if isinstance(b, int) and isinstance(self.b, int) and self.b % b == 0: return self.a % b
+    return Node.__mod__(self, b)
   def __floordiv__(self, b: Union[Node, int], factoring_allowed=True):
     return (self.a//b) % (self.b//b) if self.b % b == 0 else Node.__floordiv__(self, b, factoring_allowed)
-  def get_bounds(self) -> Tuple[int, int]:
+  def get_bounds(self) -> Tuple[int, sint]:
     assert self.a.min >= 0 and isinstance(self.b, int)
-    return (0, self.b-1) if self.a.max - self.a.min >= self.b or (self.a.min != self.a.max and self.a.min%self.b >= self.a.max%self.b) else (self.a.min%self.b, self.a.max%self.b)  # noqa: E501
-  def substitute(self, var_vals: Dict[Variable, Node]) -> Node: return self.a.substitute(var_vals) % self.b
+    if self.a.max - self.a.min >= self.b or (self.a.min != self.a.max and self.a.min%self.b >= self.a.max%self.b): return (0, self.b-1)
+    return (self.a.min%self.b, self.a.max%self.b)
+  def substitute(self, var_vals: Mapping[Variable, Union[NumNode, Variable]]) -> Node: return self.a.substitute(var_vals) % self.b
 
 class RedNode(Node):
-  def __init__(self, nodes:List[Node]): self.nodes = nodes
+  def __init__(self, nodes:List[Node]):
+    self.nodes = nodes
+    self.min, self.max = self.get_bounds()
   def vars(self) -> Set[Variable]: return set.union(*[x.vars() for x in self.nodes], set())
+  def get_bounds(self) -> Tuple[int, sint]: raise NotImplementedError("must be implemented")
 
 class SumNode(RedNode):
+  def get_bounds(self) -> Tuple[int, sint]: return sum([x.min for x in self.nodes]), sum([x.max for x in self.nodes])
   @functools.lru_cache(maxsize=None)  # pylint: disable=method-cache-max-size-none
   def __mul__(self, b: Union[Node, int]): return Node.sum([x*b for x in self.nodes]) # distribute mul into sum
   @functools.lru_cache(maxsize=None)  # pylint: disable=method-cache-max-size-none
-  def __floordiv__(self, b: Union[Node, int], factoring_allowed=True):
+  def __floordiv__(self, b: Union[Node, sint], factoring_allowed=True):
+    if self == b: return NumNode(1)
     fully_divided: List[Node] = []
     rest: List[Node] = []
-    if isinstance(b, SumNode):
-      nu_num = sum(node.b for node in self.flat_components if node.__class__ is NumNode)
-      de_num = sum(node.b for node in b.flat_components if node.__class__ is NumNode)
-      if nu_num > 0 and de_num and (d:=nu_num//de_num) > 0: return NumNode(d) + (self-b*d) // b
     if isinstance(b, Node):
       for x in self.flat_components:
         if x % b == 0: fully_divided.append(x // b)
         else: rest.append(x)
-      if (sum_fully_divided:=create_rednode(SumNode, fully_divided)) != 0: return sum_fully_divided + create_rednode(SumNode, rest) // b
+      if (sum_fully_divided:=create_node(SumNode(fully_divided))) != 0: return sum_fully_divided + create_node(SumNode(rest)) // b
       return Node.__floordiv__(self, b, False)
     if b == 1: return self
     if not factoring_allowed: return Node.__floordiv__(self, b, factoring_allowed)
-    fully_divided, rest = [], []
     _gcd = b
     divisor = 1
     for x in self.flat_components:
       if x.__class__ in (NumNode, MulNode):
-        if x.b%b == 0: fully_divided.append(x//b)
+        if x.b % b == 0: fully_divided.append(x // b)
         else:
+          if x.__class__ is NumNode and (div := x.b // b):
+            fully_divided.append(NumNode(div))
+            x = NumNode(x.b - b * div)
           rest.append(x)
           if isinstance(x.b, int):
             _gcd = gcd(_gcd, x.b)
-            if x.__class__ == MulNode and divisor == 1 and b%x.b == 0: divisor = x.b
+            if x.__class__ == MulNode and divisor == 1 and b % x.b == 0: divisor = x.b
           else:
             _gcd = 1
       else:
         rest.append(x)
         _gcd = 1
     if _gcd > 1: return Node.sum(fully_divided) + Node.sum(rest).__floordiv__(_gcd) // (b//_gcd)
     if divisor > 1: return Node.sum(fully_divided) + Node.sum(rest).__floordiv__(divisor) // (b//divisor)
     return Node.sum(fully_divided) + Node.__floordiv__(Node.sum(rest), b)
 
   @functools.lru_cache(maxsize=None)  # pylint: disable=method-cache-max-size-none
   def __mod__(self, b: Union[Node, int]):
-    if isinstance(b, SumNode):
-      nu_num = sum(node.b for node in self.flat_components if node.__class__ is NumNode)
-      de_num = sum(node.b for node in b.flat_components if node.__class__ is NumNode)
-      if nu_num > 0 and de_num and (d:=nu_num//de_num) > 0: return (self-b*d) % b
+    if self == b: return NumNode(0)
     if isinstance(b, Node) and (b - self).min > 0: return self # b - self simplifies the node
-    new_nodes: List[Node] = []
-    for x in self.nodes:
-      if x.__class__ in (NumNode, MulNode): new_nodes.append(x%b) # might simplify
-      else: new_nodes.append(x)
-    return Node.__mod__(Node.sum(new_nodes), b)
-
-  def __lt__(self, b:Union[Node,int]):
-    lhs: Node = self
-    if isinstance(b, int):
-      new_sum = []
-      for x in self.nodes:
-        # TODO: should we just force the last one to always be the number
-        if isinstance(x, NumNode): b -= x.b
-        else: new_sum.append(x)
-      lhs = Node.sum(new_sum)
-      nodes = lhs.nodes if isinstance(lhs, SumNode) else [lhs]
-      assert all(not isinstance(node, MulNode) or isinstance(node.b, int) for node in nodes), "not supported"
-      muls, others = partition(nodes, lambda x: isinstance(x, MulNode) and x.b > 0 and x.max >= b)
-      if muls:
-        # NOTE: gcd in python 3.8 takes exactly 2 args
-        mul_gcd = b
-        for x in muls: mul_gcd = gcd(mul_gcd, x.b)  # type: ignore  # mypy cannot tell that x.b is int here due to assert above
-        all_others = Node.sum(others)
-        if all_others.min >= 0 and all_others.max < mul_gcd:
-          lhs, b = Node.sum([mul//mul_gcd for mul in muls]), b//mul_gcd
-    return Node.__lt__(lhs, b) if isinstance(lhs, SumNode) else lhs < b
+    new_sum = Node.sum([node%b if node.__class__ in (NumNode, MulNode) else node for node in self.nodes])
+    return Node.__mod__(new_sum, b)
 
-  def substitute(self, var_vals: Dict[Variable, Node]) -> Node: return Node.sum([node.substitute(var_vals) for node in self.nodes])
+  def substitute(self, var_vals: Mapping[Variable, Union[NumNode, Variable]]) -> Node:
+    return Node.sum([node.substitute(var_vals) for node in self.nodes])
 
   # recursively expand sumnode components
   # TODO: can remove this if there's no SumNode inside SumNode
   @property
   def flat_components(self): return [y for x in self.nodes for y in (x.flat_components if isinstance(x, SumNode) else [x])]
 
 class AndNode(RedNode):
-  def substitute(self, var_vals: Dict[Variable, Node]) -> Node:
+  def get_bounds(self) -> Tuple[int, sint]: return min([x.min for x in self.nodes]), max([x.max for x in self.nodes])
+  def substitute(self, var_vals: Mapping[Variable, Union[NumNode, Variable]]) -> Node:
     subed = []
     for node in self.nodes:
       if not (sub:=node.substitute(var_vals)): return NumNode(0)
       subed.append(sub)
     return Node.ands(subed)
 
-def create_rednode(typ:Type[RedNode], nodes:List[Node]):
-  ret = typ(nodes)
-  if typ == SumNode: ret.min, ret.max = (sum([x.min for x in nodes]), sum([x.max for x in nodes]))
-  elif typ == AndNode: ret.min, ret.max = (min([x.min for x in nodes]), max([x.max for x in nodes]))
-  return create_node(ret)
-
 def sym_render(a: Union[Node, int], ops=None, ctx=None) -> str: return str(a) if isinstance(a, int) else a.render(ops, ctx)
-def sym_infer(a: Union[Node, int], var_vals: Dict[Variable, int]) -> int:
+def sym_infer(a: Union[Node, int], var_vals: Optional[Dict[Variable, int]]) -> int:
   if isinstance(a, (int, float)): return a
-  ret = a.substitute({k:NumNode(v) for k, v in var_vals.items()})
+  ret = a.substitute({k:NumNode(v) for k, v in var_vals.items()}) if var_vals is not None else a
   assert isinstance(ret, NumNode), f"sym_infer didn't produce NumNode from {a} with {var_vals}"
   return ret.b
 
-# symbolic int
-sint = Union[Node, int]
+# symbolic int, these are allowed in a Tensor shape
+sint = Union[int, Variable, MulNode, SumNode]
 
-render_python: Dict[Type, Callable] = {
-  Variable: lambda self,ops,ctx: f"{self.expr}[{self.min}-{self.max}{'='+str(self.val) if self._val is not None else ''}]" if ctx == "DEBUG" else (f"Variable('{self.expr}', {self.min}, {self.max})"+(f".bind({self.val})" if self._val is not None else '') if ctx == "REPR" else f"{self.expr}"),  # noqa: E501
+def render_mulnode(node:MulNode, ops, ctx):
+  # TODO: add ProdNode and remove this case
+  if isinstance(node.a,Variable) and isinstance(node.b,Variable) and node.a.expr and node.b.expr and node.b.expr < node.a.expr:
+    return f"({sym_render(node.b,ops,ctx)}*{node.a.render(ops,ctx)})"
+  return f"({node.a.render(ops,ctx)}*{sym_render(node.b,ops,ctx)})"
+
+render_python: Dict[Type, Callable[..., str]] = {
+  Variable: lambda self,ops,ctx: f"{self.expr}[{self.min}-{self.max}{'='+str(self.val) if self._val is not None else ''}]" if ctx == "DEBUG" \
+    else (f"Variable('{self.expr}', {self.min}, {self.max})"+(f".bind({self.val})" if self._val is not None else '') if ctx == "REPR" \
+    else f"{self.expr}"),
   NumNode: lambda self,ops,ctx: f"NumNode({self.b})" if ctx == "REPR" else f"{self.b}",
-  MulNode: lambda self,ops,ctx: f"({sym_render(self.b,ops,ctx)}*{self.a.render(ops,ctx)})" if isinstance(self.a,Variable) and isinstance(self.b,Variable) and self.a.expr and self.b.expr and self.b.expr < self.a.expr else f"({self.a.render(ops,ctx)}*{sym_render(self.b,ops,ctx)})",  # noqa: E501
+  MulNode: render_mulnode,
   DivNode: lambda self,ops,ctx: f"({self.a.render(ops,ctx)}//{self.b})",
   ModNode: lambda self,ops,ctx: f"({self.a.render(ops,ctx)}%{self.b})",
   LtNode: lambda self,ops,ctx: f"({self.a.render(ops,ctx)}<{sym_render(self.b,ops,ctx)})",
   SumNode: lambda self,ops,ctx: f"({'+'.join(sorted([x.render(ops,ctx) for x in self.nodes]))})",
-  AndNode: lambda self,ops,ctx: f"({' and '.join(sorted([x.render(ops,ctx) for x in self.nodes]))})"
+  AndNode: lambda self,ops,ctx: f"({' and '.join(sorted([x.render(ops,ctx) for x in self.nodes]))})",
 }
```

### Comparing `tinygrad-0.8.0/tinygrad/shape/view.py` & `tinygrad-0.9.0/tinygrad/shape/view.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from __future__ import annotations
-import functools, operator
+import functools, operator, itertools, math
 from dataclasses import dataclass
-from typing import Tuple, List, Optional, Dict, cast
+from typing import Tuple, List, Optional, Dict, Set, cast
 from tinygrad.helpers import prod, all_int, argsort
-from tinygrad.shape.symbolic import Node, NumNode, Variable, Set, sint
+from tinygrad.shape.symbolic import Node, NumNode, Variable, sint
 
 @functools.lru_cache(maxsize=None)
-def filter_strides(shape:Tuple[int, ...], strides:Tuple[int, ...]) -> Tuple[int, ...]:
-  return tuple(stride if shp != 1 else 0 for stride, shp in zip(strides, shape))
+def canonicalize_strides(shape:Tuple[sint, ...], strides:Tuple[sint, ...]) -> Tuple[sint, ...]:
+  return tuple(0 if s == 1 else st for s, st in zip(shape, strides))
 
 @functools.lru_cache(maxsize=None)
-def strides_for_shape(shape:Tuple[int, ...]) -> Tuple[int, ...]:
-  strides = [1] if shape else []
-  for d in reversed(shape[1:]): strides.append(d*strides[-1])
-  return filter_strides(shape, tuple(reversed(strides)))
+def strides_for_shape(shape:Tuple[sint, ...]) -> Tuple[sint, ...]:
+  if not shape: return ()
+  strides = tuple(itertools.accumulate(reversed(shape[1:]), operator.mul, initial=1))
+  return canonicalize_strides(shape, strides[::-1])
 
 @functools.lru_cache(maxsize=None)
-def _merge_dims(shape:Tuple[int, ...], strides:Tuple[int, ...], mask:Optional[Tuple[Tuple[int, int], ...]] = None) -> Tuple[Tuple[int, int, int], ...]:  # noqa: E501
+def _merge_dims(shape:Tuple[int, ...], strides:Tuple[int, ...], mask:Optional[Tuple[Tuple[int, int], ...]]=None) -> Tuple[Tuple[int, int, int], ...]:
   # merge contiguous subparts or zero strided dims. ret = List[(merged_dims, stride, merged dims w/o zero stride), ...]
   if not shape: return tuple()
   assert len(shape) == len(strides)
   ret = [(shape[0], strides[0], shape[0] if strides[0] else 0)]
-  # state (0, 1, 2) -> (none, in-progress, done). wrt merging zero strided dimensions
-  state = 1 if mask and strides[0] == 0 and shape[0] != 1 and mask[0][1] - mask[0][0] == 1 else 0
+  # wrt merging zero strided dimensions
+  merging = strides[0] == 0 and (mask[0][1] - mask[0][0] == 1 if mask else shape[0] == 1)
   for i, (sh, st) in enumerate(zip(shape[1:], strides[1:]), start=1):
     if sh == 1: continue
-    if state == 1 or ret[-1][1] == sh * st: # mergeable
-      ret[-1] = (ret[-1][0] * sh, st, (sh if state == 1 else ret[-1][2] * sh) if st else 0)
+    if merging or ret[-1][1] == sh * st: # mergeable
+      ret[-1] = (ret[-1][0] * sh, st, (sh if merging else ret[-1][2] * sh) if st else 0)
     else: ret.append((sh, st, sh if st else 0)) # begin new
     # merging ends with either non-zero strided dim or zero strided dim with mask range > 1
-    state = 1 if (st == 0 and mask and mask[i][1] - mask[i][0] == 1) else (2 if state != 0 else 0)
+    merging = st == 0 and (mask[i][1] - mask[i][0] == 1 if mask else sh == 1)
   return tuple(ret)
 
 @functools.lru_cache(maxsize=None)
 def _reshape_mask(view: View, new_shape:Tuple[sint, ...]) -> Tuple[Optional[Tuple[Tuple[sint, sint], ...]], bool]:
   if view.mask is None: return view.mask, False
   if any(not isinstance(m[0], int) or not isinstance(m[1], int) for m in view.mask): return view.mask, True
   new_mask: List[Tuple[int, int]] = []
@@ -48,81 +48,179 @@
     if old_dim >= next_stride: # need to split mask.
       if old_dim == next_stride: # simply copy the mask and get next batch for merging
         new_mask.append((l // curr_stride, (r - 1) // curr_stride + 1))
         curr_stride, old_dim, new_dim, mask = 1, next(r_shape, 1), next(r_new_shape, 1), next(r_masks, (0,1))
         if mask[1] - mask[0] < 1: return ((0, 0),) * len(new_shape), False # invalid mask
 
       else: # mask can only be splitted if reshape doesn't cut across the mask.
-        if ((l % next_stride != 0 or r % next_stride != 0) and l // next_stride != (r - 1) // next_stride): return view.mask, True
+        if (((l % next_stride != 0 or r % next_stride != 0) and l // next_stride != (r - 1) // next_stride)
+            or old_dim % next_stride != 0): return view.mask, True
         new_mask.append((l % next_stride // curr_stride, (r - 1) % next_stride // curr_stride + 1))
         curr_stride, new_dim = next_stride,  next(r_new_shape, 1) # need to get mask for next dimension
 
     else:
       next_mask = next(r_masks, (0, 1))
       # combine if the mask can unfold continuously
       if mask != (0, old_dim) and next_mask[1] - next_mask[0] != 1: return view.mask, True
       mask, old_dim = (next_mask[0] * old_dim + l, (next_mask[1] - 1) * old_dim + r), old_dim * next(r_shape, 1)
 
   for mask in r_masks: # if the old shape has leading 1s, need to make sure their mask is (0,1)
     if mask != (0, 1): return ((0, 0),) * len(new_shape), False # invalid mask
 
   return tuple(reversed(new_mask)), False
 
+def un1d(shape:Tuple[sint, ...], offs:sint) -> List[sint]:
+  strides = strides_for_shape(shape)
+  result = []
+  for stride in strides:
+    here = offs // stride if stride else 0
+    result.append(here)
+    offs -= here * stride
+  return result
+
 @dataclass(frozen=True)
 class View:
   shape:Tuple[sint, ...]
   strides:Tuple[sint, ...]
   offset:sint
   mask:Optional[Tuple[Tuple[sint, sint], ...]]
   contiguous:bool
 
+  @functools.lru_cache(maxsize=None)  # pylint: disable=method-cache-max-size-none
+  def size(self) -> int:
+    # NOTE: Variable and the Node derived from it in symbolic shapes can only have int as max.
+    ret = prod([x.max if isinstance(x, Node) else x for x in self.shape])
+    assert isinstance(ret, int), f"{ret=} is not int"
+    return ret
+
   @staticmethod
   @functools.lru_cache(maxsize=None)
   def create(shape:Tuple[sint, ...], strides:Optional[Tuple[sint, ...]]=None, offset:sint=0, mask:Optional[Tuple[Tuple[sint, sint], ...]]=None):
-    strides = filter_strides(shape, strides) if strides else strides_for_shape(shape)
+    strides = canonicalize_strides(shape, strides) if strides else strides_for_shape(shape)
+    # canonicalize empty mask
+    if mask is not None and all(m == (0,s) for m,s in zip(mask, shape)): mask = None
     contiguous = offset == 0 and mask is None and strides == strides_for_shape(shape)
+    # if any dimension has size >1, but is masked such that only one index in the dimension is unmasked
+    # then its stride can also be set to 0, albeit with a corresponding adjustment required to the offset
+    # TODO: assert comparison with LtNode to avoid mis-using symbolic
+    if mask and any(elim := [not (b+1 < e) for b,e in mask]):
+      if any(not (b < e) for b,e in mask):
+        strides, offset, mask = (0,) * len(shape), 0, ((0,0),) * len(shape)
+      offset += sum((strides[i] * mask[i][0]) if e else 0 for i, e in enumerate(elim))
+      strides = tuple(0 if e else st for st,e in zip(strides, elim))
     return View(shape, strides, offset, mask, contiguous)
 
   @functools.lru_cache(None)  # pylint: disable=method-cache-max-size-none
   def vars(self) -> Set[Variable]:
     flatten_mask = tuple(x for m in self.mask for x in m) if self.mask is not None else tuple()
     return functools.reduce(operator.or_, [x.vars() for x in self.shape+self.strides+(self.offset,)+flatten_mask if isinstance(x, Node)], set())
 
   @functools.lru_cache(None)  # pylint: disable=method-cache-max-size-none
-  def unbind(self) -> View:
-    unbound_vars:Dict[Variable,Node] = {v: v.unbind()[0] for v in self.vars() if v.val is not None}
+  def unbind(self) -> Tuple[View, Dict[Variable, int]]:
+    var_unboundvar_val = [(v, v.unbind()) for v in self.vars() if v.val is not None]
+    unbound_vars = {v:uv for v,(uv,_) in var_unboundvar_val}
     new_shape = tuple([s if isinstance(s, int) else s.substitute(unbound_vars) for s in self.shape])
     new_strides = tuple([s if isinstance(s, int) else s.substitute(unbound_vars) for s in self.strides])
     new_offset = self.offset if isinstance(self.offset, int) else self.offset.substitute(unbound_vars)
-    new_mask = tuple((a if isinstance(a, int) else a.substitute(unbound_vars), b if isinstance(b, int) else b.substitute(unbound_vars)) for (a, b) in self.mask) if self.mask is not None else None  # noqa: E501
-    return View.create(new_shape, new_strides, new_offset, new_mask)
+    new_mask = tuple((a if isinstance(a, int) else a.substitute(unbound_vars),
+                      b if isinstance(b, int) else b.substitute(unbound_vars)) for (a, b) in self.mask) if self.mask is not None else None
+    return View.create(new_shape, new_strides, new_offset, new_mask), dict(x[1] for x in var_unboundvar_val)
+
+  @functools.lru_cache(maxsize=None)  # pylint: disable=method-cache-max-size-none
+  def __add__(self, vm1:View) -> Optional[View]:
+    vm2 = self
+    if vm2.contiguous: return vm1
+    if vm1.contiguous and vm1.shape == vm2.shape: return vm2
+    if vm1.contiguous and vm1.size() == vm2.size() and (ret := vm2.reshape(vm1.shape)) is not None: return ret
+    if vm1.mask:
+      for b,e in vm1.mask:
+        if not (b < e): return View.create(vm1.shape, (0,) * len(vm1.shape), 0, ((0,0),) * len(vm1.shape))
+      return (merged := vm2 + vm1.shrink(vm1.mask)) and merged.pad(tuple((b,s-e) for (b,e),s in zip(vm1.mask, vm1.shape)))
+
+    # Project vm1's offset and strides on to vm2.
+    origin = un1d(vm2.shape, vm1.offset)
+    terms: List[List[Tuple[int, sint]]] = [[] for _ in origin]
+    strides: List[sint] = [0] * len(vm1.shape)
+    for d1, st in enumerate(vm1.strides):
+      if st == 0: continue
+      for d2, (o, s1) in enumerate(zip(origin, un1d(vm2.shape, vm1.offset + st))):
+        if (s1 := s1 - o) == 0: continue
+        terms[d2].append((d1, s1))
+        strides[d1] += s1 * vm2.strides[d2]
+
+    # Merge dimensions in vm2 if required.
+    # NB: Merging too many dimensions can make it difficult to project vm2's mask, hence only combining when required.
+    idxs: List[Node] = [Variable(f"idx{i}", 0, s-1) for i,s in enumerate(vm1.shape)]
+    merged_size, merged_term = 1, NumNode(0)
+    extents: List[Tuple[sint, Node]] = []
+    for term, s, o in zip(reversed(terms), reversed(vm2.shape), reversed(origin)):
+      merged_term += Variable.sum([idxs[d1] * (s1 * merged_size) for d1, s1 in term]) + o * merged_size
+      merged_size *= s
+      if not (merged_term >= merged_size) and not (merged_term < 0):
+        extents.append((merged_size, merged_term))
+        merged_size, merged_term = 1, NumNode(0)
+    if merged_term: return None
+    if (vm2_shape := tuple(s for s,_ in reversed(extents))) != vm2.shape:
+      return (reshaped_vm2 := vm2.reshape(vm2_shape)) and reshaped_vm2 + vm1
+
+    if vm2.mask:
+      # Try to project vm2's mask on to vm1.
+      newb, newe, bad = [0] * len(vm1.shape), list(vm1.shape), False
+      for d2, ((b, e), o, (_, t)) in enumerate(zip(vm2.mask, origin, reversed(extents))):
+        if not (t.min < b or t.max >= e): continue
+        if not isinstance(o, int) or not isinstance(b, int) or not isinstance(e, int):
+          bad = True
+          continue
+        term = terms[d2]
+        if len(term) != 1:
+          if not term and newe: newe[0] = 0
+          else: bad = True
+          continue
+        d1, s1 = term[0]
+        if not isinstance(s1, int) or not isinstance(newe[d1], int):
+          bad = True
+          continue
+        newb[d1] = max(newb[d1], math.ceil((b - o if s1 > 0 else e - o - 1) / s1))
+        newe[d1] = min(newe[d1], (b - o if s1 < 0 else e - o - 1) // s1 + 1)
+
+      # If any of vm1 was masked off, try again with that mask in place.
+      for b, e, s in zip(newb, newe, vm1.shape):
+        if b != 0 or e != s:
+          return vm2 + View.create(vm1.shape, vm1.strides, vm1.offset, tuple(zip(newb, newe)))
+      # Otherwise if vm2's mask was violated, then cannot merge.
+      if bad: return None
+
+    return View.create(vm1.shape, tuple(strides), sum(o * s for o, s in zip(origin, vm2.strides)) + vm2.offset)
 
   @functools.lru_cache(maxsize=None)  # pylint: disable=method-cache-max-size-none
   def invert(self, out_shape:Tuple[sint, ...]) -> Optional[View]:
     ret = View.create(self.shape)
     if self.mask: ret = ret.shrink(self.mask)
     ret = ret.stride(tuple(-1 if x < 0 else 1 for x in self.strides)).permute(argsort(tuple(-x if x > 0 else x for x in self.strides)))
     return ret if prod(ret.shape) == prod(out_shape) else None   # don't support shrink, expand, or stride != (-1, 1)
 
-  # MovementOps live here now
+  @functools.lru_cache(maxsize=None)  # pylint: disable=method-cache-max-size-none
+  def minify(self):
+    min_shape = tuple(x[0] for x in _merge_dims(self.shape, self.strides, self.mask))
+    return nv if (nv := self.reshape(min_shape)) else self
 
   def __unsafe_resize(self, arg: Tuple[Tuple[sint, sint], ...], mask=None) -> View:
     offset = sum([s * x[0] for s, x in zip(self.strides,arg)])
     if self.mask:
       # move the old mask
       nmask = tuple([(max(0, min(mx-ax,ay-ax)), max(0, min(my-ax,ay-ax))) for (mx,my),(ax,ay) in zip(self.mask, arg)])
       # merge the masks if we have two
       mask = tuple([(max(mx1, mx2), min(my1, my2)) for (mx1, my1), (mx2, my2) in zip(nmask, mask)]) if mask is not None else nmask
     shape = [y-x for x,y in arg]
     if mask is not None and all(m[0] == 0 and m[1] == s for m,s in zip(mask, shape)): mask = None
     return View.create(tuple(s.b if isinstance(s, NumNode) else s for s in shape), self.strides, self.offset+offset, mask)
 
   @functools.lru_cache(maxsize=None)  # pylint: disable=method-cache-max-size-none
-  def pad(self, arg: Tuple[Tuple[int, int], ...]) -> View:
-    assert all((b>=0 and e>=0) for b,e in arg) and len(arg) == len(self.shape)
+  def pad(self, arg: Tuple[Tuple[sint, sint], ...]) -> View:
+    assert all((b>=0 and e>=0) for b,e in arg) and len(arg) == len(self.shape), f"{self.shape=}, {arg=}"
     if any(b or e for b, e in arg):
       zvarg = tuple([(-b,s+e) for s,(b,e) in zip(self.shape, arg)])
       mask = tuple([(b,s+b) for s,(b,_) in zip(self.shape, arg)])
       return self.__unsafe_resize(zvarg, mask=mask)
     return self
 
   @functools.lru_cache(maxsize=None)  # pylint: disable=method-cache-max-size-none
@@ -141,24 +239,26 @@
     mask = tuple([(((0,0) if m != (0,1) else (0,ns)) if s != ns else m) for m,s,ns in zip(self.mask, self.shape, new_shape)]) if self.mask else None
     return View.create(new_shape, self.strides, self.offset, mask)
 
   @functools.lru_cache(maxsize=None)  # pylint: disable=method-cache-max-size-none
   def permute(self, axis: Tuple[int, ...]) -> View:
     assert all(isinstance(x, int) and x >= 0 and x < len(self.shape) for x in axis), f"invalid permute {axis} for {self.shape}"
     assert len(set(axis)) == len(axis) and len(axis) == len(self.shape), f"can't permute {self.shape} with {axis}"
-    return View.create(tuple([self.shape[a] for a in axis]), tuple([self.strides[a] for a in axis]), self.offset, tuple([self.mask[a] for a in axis]) if self.mask is not None else None)  # noqa: E501
+    return View.create(tuple(self.shape[a] for a in axis), tuple(self.strides[a] for a in axis), self.offset,
+                       tuple(self.mask[a] for a in axis) if self.mask is not None else None)
 
   @functools.lru_cache(maxsize=None)  # pylint: disable=method-cache-max-size-none
   def stride(self, mul: Tuple[int, ...]) -> View:
     # except for the negative case, you can build this from the others. invertible in the negative case
     assert all(isinstance(x, int) and x != 0 for x in mul), f"invalid stride {mul} for {self.shape}"
     strides = tuple([z*m for z,m in zip(self.strides, mul)])
     new_shape = tuple([(s+(abs(m)-1))//abs(m) for s,m in zip(self.shape, mul)])
     offset = sum([(s-1)*z for s,z,m in zip(self.shape, self.strides, mul) if m < 0])
-    mask = tuple([(((mx if m > 0 else s-my)+(abs(m)-1))//abs(m), ((my if m > 0 else s-mx)+(abs(m)-1))//abs(m)) for (mx,my),s,m in zip(self.mask, self.shape, mul)]) if self.mask is not None else None  # noqa: E501
+    mask = tuple([(((mx if m > 0 else s-my)+(abs(m)-1))//abs(m), ((my if m > 0 else s-mx)+(abs(m)-1))//abs(m)) \
+                  for (mx,my),s,m in zip(self.mask, self.shape, mul)]) if self.mask is not None else None
     return View.create(new_shape, strides, self.offset + offset, mask)
 
   @functools.lru_cache(maxsize=None)  # pylint: disable=method-cache-max-size-none
   def reshape(self, new_shape: Tuple[sint, ...]) -> Optional[View]:
     if self.shape == new_shape: return self
 
     assert all(x >= 0 for x in new_shape), f"shape can't contain negative numbers {new_shape}"
@@ -173,22 +273,24 @@
 
     if new_shape == () and self.mask and any(mx==my for (mx,my) in self.mask): return None
 
     # after the asserts, it's okay to check contiguous
     if self.contiguous: return View.create(new_shape)
 
     strides, r_new_shape = [], reversed(new_shape)
-    for merged_dim, s, real_dim in reversed(_merge_dims(self.shape, self.strides, self.mask)):
-      acc, new_stride = 1, s
+    for merged_dim, new_stride, real_dim in reversed(_merge_dims(self.shape, self.strides, self.mask)):
+      acc = 1
+      # TODO: this <= and != is for symbolic!?
       while acc <= merged_dim and acc != merged_dim and (new_dim := next(r_new_shape, None)):
-        strides.append(new_stride if new_dim != 1 else 0)
-        if new_dim == 1: continue
-        new_stride *= (new_dim if (acc :=  acc * new_dim) < real_dim else 0)
+        strides.append(new_stride)
+        if new_dim != 1: new_stride *= (new_dim if (acc :=  acc * new_dim) < real_dim else 0)
       if acc != merged_dim: break
     else:
       strides += [0,] * (len(new_shape) - len(strides))
-      mask, extra = _reshape_mask(self, new_shape)
-      fstrides = filter_strides(tuple(e-b for b,e in mask) if mask else new_shape, tuple(reversed(strides)))
-      extra_offset = (sum(m[0] * s for m,s in zip(self.mask, self.strides)) if self.mask else 0) - (sum(m[0] * s for m,s in zip(mask, fstrides)) if mask else 0) # noqa: E501
-      if not extra: return View.create(new_shape, fstrides, self.offset + extra_offset, mask)
+      new_mask, extra = _reshape_mask(self, new_shape)
+      if not extra:
+        new_strides = canonicalize_strides(tuple(e-b for b,e in new_mask) if new_mask else new_shape, tuple(reversed(strides)))
+        extra_offset = (sum(m[0] * s for m,s in zip(self.mask, self.strides)) if self.mask else 0) - \
+                       (sum(m[0] * s for m,s in zip(new_mask, new_strides)) if new_mask else 0)
+        return View.create(new_shape, new_strides, self.offset + extra_offset, new_mask)
 
     return None
```

### Comparing `tinygrad-0.8.0/tinygrad.egg-info/PKG-INFO` & `tinygrad-0.9.0/tinygrad.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: tinygrad
-Version: 0.8.0
+Version: 0.9.0
 Summary: You like pytorch? You like micrograd? You love tinygrad! <3
 Author: George Hotz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: tqdm
-Requires-Dist: gpuctypes
 Requires-Dist: pyobjc-framework-Metal; platform_system == "Darwin"
 Requires-Dist: pyobjc-framework-libdispatch; platform_system == "Darwin"
 Provides-Extra: llvm
 Requires-Dist: llvmlite; extra == "llvm"
 Provides-Extra: arm
 Requires-Dist: unicorn; extra == "arm"
 Provides-Extra: triton
@@ -28,29 +27,42 @@
 Requires-Dist: ruff; extra == "linting"
 Requires-Dist: types-tqdm; extra == "linting"
 Provides-Extra: testing
 Requires-Dist: torch; extra == "testing"
 Requires-Dist: pillow; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-xdist; extra == "testing"
-Requires-Dist: onnx==1.15.0; extra == "testing"
+Requires-Dist: onnx==1.16.0; extra == "testing"
 Requires-Dist: onnx2torch; extra == "testing"
 Requires-Dist: opencv-python; extra == "testing"
 Requires-Dist: tabulate; extra == "testing"
 Requires-Dist: safetensors; extra == "testing"
 Requires-Dist: transformers; extra == "testing"
 Requires-Dist: sentencepiece; extra == "testing"
 Requires-Dist: tiktoken; extra == "testing"
 Requires-Dist: librosa; extra == "testing"
 Requires-Dist: networkx; extra == "testing"
 Requires-Dist: hypothesis; extra == "testing"
+Requires-Dist: nibabel; extra == "testing"
+Provides-Extra: docs
+Requires-Dist: mkdocs-material; extra == "docs"
+Requires-Dist: mkdocstrings[python]; extra == "docs"
+Requires-Dist: markdown-callouts; extra == "docs"
+Requires-Dist: markdown-exec[ansi]; extra == "docs"
+Requires-Dist: black; extra == "docs"
+Provides-Extra: testing-tf
+Requires-Dist: tensorflow==2.15.1; extra == "testing-tf"
+Requires-Dist: tensorflow_addons; extra == "testing-tf"
 
 <div align="center">
 
-[![logo](https://raw.githubusercontent.com/tinygrad/tinygrad/master/docs/logo.png)](https://tinygrad.org)
+<picture>
+  <source media="(prefers-color-scheme: light)" srcset="/docs/logo_tiny_light.svg">
+  <img alt="tiny corp logo" src="/docs/logo_tiny_dark.svg" width="50%" height="50%">
+</picture>
 
 tinygrad: For something between [PyTorch](https://github.com/pytorch/pytorch) and [karpathy/micrograd](https://github.com/karpathy/micrograd). Maintained by [tiny corp](https://tinygrad.org).
 
 <h3>
 
 [Homepage](https://github.com/tinygrad/tinygrad) | [Documentation](/docs) | [Examples](/examples) | [Showcase](/docs/showcase.md) | [Discord](https://discord.gg/ZjZadyC7PK)
 
@@ -118,25 +130,22 @@
 
 See [examples/beautiful_mnist.py](examples/beautiful_mnist.py) for the full version that gets 98% in ~5 seconds
 
 ## Accelerators
 
 tinygrad already supports numerous accelerators, including:
 
-- [x] [CPU](tinygrad/runtime/ops_cpu.py)
 - [x] [GPU (OpenCL)](tinygrad/runtime/ops_gpu.py)
-- [x] [C Code (Clang)](tinygrad/runtime/ops_clang.py)
+- [x] [CLANG (C Code)](tinygrad/runtime/ops_clang.py)
 - [x] [LLVM](tinygrad/runtime/ops_llvm.py)
 - [x] [METAL](tinygrad/runtime/ops_metal.py)
 - [x] [CUDA](tinygrad/runtime/ops_cuda.py)
-- [x] [PyTorch](tinygrad/runtime/ops_torch.py)
-- [x] [HIP](tinygrad/runtime/ops_hip.py)
+- [x] [HSA](tinygrad/runtime/ops_hsa.py)
 
 And it is easy to add more! Your accelerator of choice only needs to support a total of ~25 low level ops.
-More information can be found in the [documentation for adding new accelerators](/docs/adding_new_accelerators.md).
 
 ## Installation
 
 The current recommended way to install tinygrad is from source.
 
 ### From source
 
@@ -189,14 +198,15 @@
 
 We'll start with what will get your PR closed with a pointer to this section:
 
 - No code golf! While low line count is a guiding light of this project, anything that remotely looks like code golf will be closed. The true goal is reducing complexity and increasing readability, and deleting `\n`s does nothing to help with that.
 - All docs and whitespace changes will be closed unless you are a well-known contributor. The people writing the docs should be those who know the codebase the absolute best. People who have not demonstrated that shouldn't be messing with docs. Whitespace changes are both useless *and* carry a risk of introducing bugs.
 - Anything you claim is a "speedup" must be benchmarked. In general, the goal is simplicity, so even if your PR makes things marginally faster, you have to consider the tradeoff with maintainablity and readablity.
 - In general, the code outside the core `tinygrad/` folder is not well tested, so unless the current code there is broken, you shouldn't be changing it.
+- If your PR looks "complex", is a big diff, or adds lots of lines, it won't be reviewed or merged. Consider breaking it up into smaller PRs that are individually clear wins. A common pattern I see is prerequisite refactors before adding new functionality. If you can (cleanly) refactor to the point that the feature is a 3 line change, this is great, and something easy for us to review.
 
 Now, what we want:
 
 - Bug fixes (with a regression test) are great! This library isn't 1.0 yet, so if you stumble upon a bug, fix it, write a test, and submit a PR, this is valuable work.
 - Solving bounties! tinygrad [offers cash bounties](https://docs.google.com/spreadsheets/d/1WKHbT-7KOgjEawq5h5Ic1qUWzpfAzuD_J06N1JwOCGs/edit?usp=sharing) for certain improvements to the library. All new code should be high quality and well tested.
 - Features. However, if you are adding a feature, consider the line tradeoff. If it's 3 lines, there's less of a bar of usefulness it has to meet over something that's 30 or 300 lines. All features must have regression tests. In general with no other constraints, your feature's API should match torch or numpy.
 - Refactors that are clear wins. In general, if your refactor isn't a clear win it will be closed. But some refactors are amazing! Think about readability in a deep core sense. A whitespace change or moving a few functions around is useless, but if you realize that two 100 line functions can actually use the same 110 line function with arguments while also improving readability, this is a big win.
```

### Comparing `tinygrad-0.8.0/tinygrad.egg-info/SOURCES.txt` & `tinygrad-0.9.0/tinygrad.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,113 @@
 LICENSE
 README.md
 setup.py
+test/test_arange.py
 test/test_assign.py
+test/test_const_folding.py
 test/test_conv.py
 test/test_conv_shapetracker.py
 test/test_copy_speed.py
 test/test_custom_function.py
+test/test_device_speed.py
 test/test_dtype.py
 test/test_dtype_alu.py
 test/test_fusion_op.py
+test/test_fuzz_shape_ops.py
 test/test_gc.py
-test/test_hip_rdna3.py
 test/test_image_dtype.py
 test/test_jit.py
 test/test_kernel_cache.py
 test/test_lazybuffer.py
 test/test_lazyop.py
 test/test_linearizer.py
 test/test_linearizer_failures.py
+test/test_linearizer_overflows.py
 test/test_masked_st.py
 test/test_method_cache.py
 test/test_multitensor.py
 test/test_net_speed.py
 test/test_nn.py
 test/test_ops.py
 test/test_optim.py
+test/test_pattern_matcher.py
+test/test_pickle.py
 test/test_randomness.py
 test/test_sample.py
 test/test_schedule.py
 test/test_search.py
+test/test_setitem.py
 test/test_specific_conv.py
 test/test_speed_v_torch.py
+test/test_subbuffer.py
 test/test_symbolic_jit.py
 test/test_symbolic_ops.py
 test/test_symbolic_shapetracker.py
 test/test_tensor.py
 test/test_tensor_data.py
+test/test_tensor_variable.py
 test/test_to_numpy.py
+test/test_uop_graph.py
 test/test_uops.py
+test/test_uops_stats.py
 test/test_winograd.py
 test/test_zero_copy.py
 tinygrad/__init__.py
 tinygrad/device.py
 tinygrad/dtype.py
-tinygrad/graph.py
+tinygrad/function.py
 tinygrad/helpers.py
-tinygrad/jit.py
 tinygrad/lazy.py
-tinygrad/mlops.py
+tinygrad/multi.py
 tinygrad/ops.py
-tinygrad/realize.py
 tinygrad/tensor.py
 tinygrad.egg-info/PKG-INFO
 tinygrad.egg-info/SOURCES.txt
 tinygrad.egg-info/dependency_links.txt
 tinygrad.egg-info/requires.txt
 tinygrad.egg-info/top_level.txt
 tinygrad/codegen/kernel.py
 tinygrad/codegen/linearizer.py
-tinygrad/features/image.py
-tinygrad/features/multi.py
-tinygrad/features/search.py
+tinygrad/codegen/uops.py
+tinygrad/engine/__init__.py
+tinygrad/engine/graph.py
+tinygrad/engine/jit.py
+tinygrad/engine/realize.py
+tinygrad/engine/schedule.py
+tinygrad/engine/search.py
 tinygrad/nn/__init__.py
+tinygrad/nn/datasets.py
 tinygrad/nn/optim.py
 tinygrad/nn/state.py
+tinygrad/renderer/__init__.py
+tinygrad/renderer/assembly.py
 tinygrad/renderer/cstyle.py
 tinygrad/renderer/llvmir.py
+tinygrad/runtime/ops_amd.py
 tinygrad/runtime/ops_clang.py
-tinygrad/runtime/ops_cpu.py
 tinygrad/runtime/ops_cuda.py
 tinygrad/runtime/ops_disk.py
 tinygrad/runtime/ops_gpu.py
-tinygrad/runtime/ops_hip.py
+tinygrad/runtime/ops_hsa.py
 tinygrad/runtime/ops_llvm.py
 tinygrad/runtime/ops_metal.py
-tinygrad/runtime/ops_torch.py
+tinygrad/runtime/ops_npy.py
+tinygrad/runtime/ops_nv.py
+tinygrad/runtime/ops_python.py
+tinygrad/runtime/autogen/amd_gpu.py
+tinygrad/runtime/autogen/comgr.py
+tinygrad/runtime/autogen/cuda.py
+tinygrad/runtime/autogen/hip.py
+tinygrad/runtime/autogen/hsa.py
+tinygrad/runtime/autogen/kfd.py
+tinygrad/runtime/autogen/nv_gpu.py
+tinygrad/runtime/autogen/opencl.py
+tinygrad/runtime/driver/hip_comgr.py
+tinygrad/runtime/driver/hsa.py
+tinygrad/runtime/graph/clang.py
 tinygrad/runtime/graph/cuda.py
-tinygrad/runtime/graph/hip.py
+tinygrad/runtime/graph/hcq.py
+tinygrad/runtime/graph/hsa.py
 tinygrad/runtime/graph/metal.py
 tinygrad/shape/shapetracker.py
 tinygrad/shape/symbolic.py
 tinygrad/shape/view.py
```

