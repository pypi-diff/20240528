# Comparing `tmp/kerch-0.3.1.3.tar.gz` & `tmp/kerch-0.3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kerch-0.3.1.3.tar", last modified: Tue May 28 15:36:11 2024, max compression
+gzip compressed data, was "kerch-0.3.1.4.tar", last modified: Tue May 28 15:39:19 2024, max compression
```

## Comparing `kerch-0.3.1.3.tar` & `kerch-0.3.1.4.tar`

### file list

```diff
@@ -1,114 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.315999 kerch-0.3.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-28 15:36:07.000000 kerch-0.3.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-28 15:36:07.000000 kerch-0.3.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15339 2024-05-28 15:36:11.315999 kerch-0.3.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-28 15:36:07.000000 kerch-0.3.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.300000 kerch-0.3.1.3/kerch/
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/_dataholder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/_stochastic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.300000 kerch-0.3.1.3/kerch/data/
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/data/_LearningSet.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/data/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.300000 kerch-0.3.1.3/kerch/feature/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/feature/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13689 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/feature/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/feature/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/feature/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    12459 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/feature/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/feature/stochastic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.304000 kerch-0.3.1.3/kerch/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/kernel/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12328 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/kernel/_base_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/kernel/_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/kernel/explicit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/kernel/implicit.py
--rw-r--r--   0 runner    (1001) docker     (127)    15564 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/kernel/kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7649 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/kernel/nystrom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.304000 kerch-0.3.1.3/kerch/level/
--rw-r--r--   0 runner    (1001) docker     (127)    14868 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/level/_KPCA.py
--rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/level/_Level.py
--rw-r--r--   0 runner    (1001) docker     (127)    11645 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/level/_PPCA.py
--rw-r--r--   0 runner    (1001) docker     (127)    16228 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/level/_View.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/level/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/level/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.304000 kerch-0.3.1.3/kerch/method/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/method/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/method/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/method/_iterative.py
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/method/_knn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/method/_smoother.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.307999 kerch-0.3.1.3/kerch/monitor/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/monitor/Local.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/monitor/Plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/monitor/Saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/monitor/WandB.py
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/monitor/Watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/monitor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/monitor/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/monitor/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/monitor/module.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/monitor/rkm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.307999 kerch-0.3.1.3/kerch/opt/
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/opt/Optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/opt/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.307999 kerch-0.3.1.3/kerch/plot/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/plot/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9538 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/plot/matplotlib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.307999 kerch-0.3.1.3/kerch/preimage/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/preimage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/preimage/iterative.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/preimage/knn.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/preimage/ridge_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/preimage/smoother.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.311999 kerch-0.3.1.3/kerch/script/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/script/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/script/_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/script/expe.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/script/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/script/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.311999 kerch-0.3.1.3/kerch/train/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/train/Hyper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/train/Trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/train/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.311999 kerch-0.3.1.3/kerch/transform/
--rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/transform/Transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/transform/TransformTree.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/transform/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.315999 kerch-0.3.1.3/kerch/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/utils/arch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/utils/cast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/utils/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/utils/tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/utils/type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.315999 kerch-0.3.1.3/kerch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15339 2024-05-28 15:36:11.000000 kerch-0.3.1.3/kerch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-28 15:36:11.000000 kerch-0.3.1.3/kerch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:36:11.000000 kerch-0.3.1.3/kerch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 15:36:11.000000 kerch-0.3.1.3/kerch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 15:36:11.000000 kerch-0.3.1.3/kerch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-05-28 15:36:07.000000 kerch-0.3.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:36:11.315999 kerch-0.3.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 15:36:07.000000 kerch-0.3.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:39:19.301354 kerch-0.3.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-28 15:39:14.000000 kerch-0.3.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-28 15:39:14.000000 kerch-0.3.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15339 2024-05-28 15:39:19.301354 kerch-0.3.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-28 15:39:14.000000 kerch-0.3.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:39:19.285354 kerch-0.3.1.4/kerch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/_dataholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/_stochastic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:39:19.285354 kerch-0.3.1.4/kerch/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/data/_LearningSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/data/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:39:19.289354 kerch-0.3.1.4/kerch/feature/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/feature/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13689 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/feature/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/feature/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/feature/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12459 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/feature/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/feature/stochastic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:39:19.289354 kerch-0.3.1.4/kerch/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/kernel/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12328 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/kernel/_base_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/kernel/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/kernel/explicit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/kernel/implicit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15564 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/kernel/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7649 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/kernel/nystrom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:39:19.289354 kerch-0.3.1.4/kerch/level/
+-rw-r--r--   0 runner    (1001) docker     (127)    14868 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/level/_KPCA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/level/_Level.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11645 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/level/_PPCA.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16228 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/level/_View.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/level/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/level/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:39:19.293354 kerch-0.3.1.4/kerch/method/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/method/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/method/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/method/_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/method/_knn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/method/_smoother.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:39:19.293354 kerch-0.3.1.4/kerch/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/model/KPCA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/model/LSSVM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/model/Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/model/RKM.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/model/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/model/_kpca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/model/_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/model/_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/model/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/model/level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/model/ridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/model/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:39:19.297354 kerch-0.3.1.4/kerch/monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/monitor/Local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/monitor/Plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/monitor/Saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/monitor/WandB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/monitor/Watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/monitor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/monitor/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/monitor/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/monitor/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/monitor/rkm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:39:19.297354 kerch-0.3.1.4/kerch/opt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/opt/Optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/opt/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:39:19.297354 kerch-0.3.1.4/kerch/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/plot/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9538 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/plot/matplotlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:39:19.297354 kerch-0.3.1.4/kerch/preimage/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/preimage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/preimage/iterative.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/preimage/knn.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/preimage/ridge_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/preimage/smoother.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:39:19.297354 kerch-0.3.1.4/kerch/script/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/script/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/script/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/script/expe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/script/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/script/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:39:19.301354 kerch-0.3.1.4/kerch/train/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/train/Hyper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/train/Trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/train/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:39:19.301354 kerch-0.3.1.4/kerch/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/transform/Transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/transform/TransformTree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/transform/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:39:19.301354 kerch-0.3.1.4/kerch/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/utils/arch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/utils/cast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/utils/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/utils/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-28 15:39:14.000000 kerch-0.3.1.4/kerch/utils/type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:39:19.301354 kerch-0.3.1.4/kerch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15339 2024-05-28 15:39:19.000000 kerch-0.3.1.4/kerch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-28 15:39:19.000000 kerch-0.3.1.4/kerch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:39:19.000000 kerch-0.3.1.4/kerch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 15:39:19.000000 kerch-0.3.1.4/kerch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 15:39:19.000000 kerch-0.3.1.4/kerch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10162 2024-05-28 15:39:14.000000 kerch-0.3.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:39:19.301354 kerch-0.3.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 15:39:14.000000 kerch-0.3.1.4/setup.py
```

### Comparing `kerch-0.3.1.3/LICENSE` & `kerch-0.3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/PKG-INFO` & `kerch-0.3.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kerch
-Version: 0.3.1.3
+Version: 0.3.1.4
 Summary: Kernel Methods in PyTorch
 Author-email: Henri DE PLAEN <henri.deplaen@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `kerch-0.3.1.3/README.md` & `kerch-0.3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/__init__.py` & `kerch-0.3.1.4/kerch/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-__version__ = "0.3.1.3"
+__version__ = "0.3.1.4"
 __author__ = "HENRI DE PLAEN"
 __credits__ = "KU Leuven"
 __status__ = "beta"
 __date__ = "May 2024"
 __license__ = "LGPL-3.0"
 
 # GLOBAL MODULE-WIDE VARIABLES
```

### Comparing `kerch-0.3.1.3/kerch/_cache.py` & `kerch-0.3.1.4/kerch/_cache.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/_dataholder.py` & `kerch-0.3.1.4/kerch/_dataholder.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/_logger.py` & `kerch-0.3.1.4/kerch/_logger.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/_module.py` & `kerch-0.3.1.4/kerch/_module.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/_sample.py` & `kerch-0.3.1.4/kerch/_sample.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/_stochastic.py` & `kerch-0.3.1.4/kerch/_stochastic.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/data/_LearningSet.py` & `kerch-0.3.1.4/kerch/data/_LearningSet.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/data/datasets.py` & `kerch-0.3.1.4/kerch/data/datasets.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/data/factory.py` & `kerch-0.3.1.4/kerch/data/factory.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/feature/cache.py` & `kerch-0.3.1.4/kerch/feature/cache.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/feature/logger.py` & `kerch-0.3.1.4/kerch/feature/logger.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/feature/module.py` & `kerch-0.3.1.4/kerch/feature/module.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/feature/sample.py` & `kerch-0.3.1.4/kerch/feature/sample.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/feature/stochastic.py` & `kerch-0.3.1.4/kerch/feature/stochastic.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/kernel/__init__.pyi` & `kerch-0.3.1.4/kerch/kernel/__init__.pyi`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/kernel/_base_kernel.py` & `kerch-0.3.1.4/kerch/kernel/_base_kernel.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/kernel/_factory.py` & `kerch-0.3.1.4/kerch/kernel/_factory.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/kernel/explicit.py` & `kerch-0.3.1.4/kerch/kernel/explicit.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/kernel/implicit.py` & `kerch-0.3.1.4/kerch/kernel/implicit.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/kernel/kernel.py` & `kerch-0.3.1.4/kerch/kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/kernel/nystrom.py` & `kerch-0.3.1.4/kerch/kernel/nystrom.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/level/_KPCA.py` & `kerch-0.3.1.4/kerch/level/_KPCA.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/level/_Level.py` & `kerch-0.3.1.4/kerch/level/_Level.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/level/_PPCA.py` & `kerch-0.3.1.4/kerch/level/_PPCA.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/level/_View.py` & `kerch-0.3.1.4/kerch/level/_View.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/level/factory.py` & `kerch-0.3.1.4/kerch/level/factory.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/method/_iterative.py` & `kerch-0.3.1.4/kerch/method/_iterative.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/method/_knn.py` & `kerch-0.3.1.4/kerch/method/_knn.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/method/_smoother.py` & `kerch-0.3.1.4/kerch/method/_smoother.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/monitor/Plotter.py` & `kerch-0.3.1.4/kerch/monitor/Plotter.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/monitor/Saver.py` & `kerch-0.3.1.4/kerch/monitor/Saver.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/monitor/WandB.py` & `kerch-0.3.1.4/kerch/monitor/WandB.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/monitor/Watcher.py` & `kerch-0.3.1.4/kerch/monitor/Watcher.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/monitor/factory.py` & `kerch-0.3.1.4/kerch/monitor/factory.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/monitor/model.py` & `kerch-0.3.1.4/kerch/monitor/model.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/monitor/module.py` & `kerch-0.3.1.4/kerch/monitor/module.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/monitor/rkm.py` & `kerch-0.3.1.4/kerch/monitor/rkm.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/opt/Optimizer.py` & `kerch-0.3.1.4/kerch/opt/Optimizer.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/plot/matplotlib.py` & `kerch-0.3.1.4/kerch/plot/matplotlib.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/preimage/knn.py` & `kerch-0.3.1.4/kerch/preimage/knn.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/preimage/smoother.py` & `kerch-0.3.1.4/kerch/preimage/smoother.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/script/_parser.py` & `kerch-0.3.1.4/kerch/script/_parser.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/script/expe.py` & `kerch-0.3.1.4/kerch/script/expe.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/script/version.py` & `kerch-0.3.1.4/kerch/script/version.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/train/Trainer.py` & `kerch-0.3.1.4/kerch/train/Trainer.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/transform/Transform.py` & `kerch-0.3.1.4/kerch/transform/Transform.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/transform/TransformTree.py` & `kerch-0.3.1.4/kerch/transform/TransformTree.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/utils/__init__.pyi` & `kerch-0.3.1.4/kerch/utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/utils/arch.py` & `kerch-0.3.1.4/kerch/utils/arch.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/utils/cast.py` & `kerch-0.3.1.4/kerch/utils/cast.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/utils/decorators.py` & `kerch-0.3.1.4/kerch/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/utils/defaults.py` & `kerch-0.3.1.4/kerch/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/utils/errors.py` & `kerch-0.3.1.4/kerch/utils/errors.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/utils/math.py` & `kerch-0.3.1.4/kerch/utils/math.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/utils/tensor.py` & `kerch-0.3.1.4/kerch/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch/utils/type.py` & `kerch-0.3.1.4/kerch/utils/type.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.3/kerch.egg-info/PKG-INFO` & `kerch-0.3.1.4/kerch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kerch
-Version: 0.3.1.3
+Version: 0.3.1.4
 Summary: Kernel Methods in PyTorch
 Author-email: Henri DE PLAEN <henri.deplaen@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `kerch-0.3.1.3/kerch.egg-info/SOURCES.txt` & `kerch-0.3.1.4/kerch.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,27 @@
 kerch/level/__init__.pyi
 kerch/level/factory.py
 kerch/method/__init__.py
 kerch/method/__init__.pyi
 kerch/method/_iterative.py
 kerch/method/_knn.py
 kerch/method/_smoother.py
+kerch/model/KPCA.py
+kerch/model/LSSVM.py
+kerch/model/Model.py
+kerch/model/RKM.py
+kerch/model/__init__.py
+kerch/model/__init__.pyi
+kerch/model/_kpca.py
+kerch/model/_level.py
+kerch/model/_view.py
+kerch/model/factory.py
+kerch/model/level.py
+kerch/model/ridge.py
+kerch/model/view.py
 kerch/monitor/Local.py
 kerch/monitor/Plotter.py
 kerch/monitor/Saver.py
 kerch/monitor/WandB.py
 kerch/monitor/Watcher.py
 kerch/monitor/__init__.py
 kerch/monitor/__init__.pyi
```

### Comparing `kerch-0.3.1.3/pyproject.toml` & `kerch-0.3.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 packages = [
     "kerch",
     "kerch.data",
     "kerch.feature",
     "kerch.kernel",
     "kerch.level",
     "kerch.method",
+    "kerch.model",
     "kerch.monitor",
     "kerch.opt",
     "kerch.plot",
     "kerch.preimage",
     "kerch.script",
     "kerch.train",
     "kerch.transform",
```

