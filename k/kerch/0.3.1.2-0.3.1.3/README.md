# Comparing `tmp/kerch-0.3.1.2.tar.gz` & `tmp/kerch-0.3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kerch-0.3.1.2.tar", last modified: Tue May 28 15:29:25 2024, max compression
+gzip compressed data, was "kerch-0.3.1.3.tar", last modified: Tue May 28 15:36:11 2024, max compression
```

## Comparing `kerch-0.3.1.2.tar` & `kerch-0.3.1.3.tar`

### file list

```diff
@@ -1,109 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.134511 kerch-0.3.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-28 15:29:18.000000 kerch-0.3.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-28 15:29:18.000000 kerch-0.3.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15339 2024-05-28 15:29:25.134511 kerch-0.3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-28 15:29:18.000000 kerch-0.3.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.118511 kerch-0.3.1.2/kerch/
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/_dataholder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/_stochastic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.118511 kerch-0.3.1.2/kerch/data/
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/data/_LearningSet.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/data/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.122511 kerch-0.3.1.2/kerch/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/kernel/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12328 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/kernel/_base_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/kernel/_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/kernel/explicit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/kernel/implicit.py
--rw-r--r--   0 runner    (1001) docker     (127)    15564 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/kernel/kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7649 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/kernel/nystrom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.122511 kerch-0.3.1.2/kerch/level/
--rw-r--r--   0 runner    (1001) docker     (127)    14868 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/level/_KPCA.py
--rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/level/_Level.py
--rw-r--r--   0 runner    (1001) docker     (127)    11645 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/level/_PPCA.py
--rw-r--r--   0 runner    (1001) docker     (127)    16228 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/level/_View.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/level/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/level/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.122511 kerch-0.3.1.2/kerch/method/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/method/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/method/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/method/_iterative.py
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/method/_knn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/method/_smoother.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.126510 kerch-0.3.1.2/kerch/model/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/KPCA.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/LSSVM.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/Model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/RKM.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/_kpca.py
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/_level.py
--rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/level.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/ridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.126510 kerch-0.3.1.2/kerch/monitor/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/monitor/Local.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/monitor/Plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/monitor/Saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/monitor/WandB.py
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/monitor/Watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/monitor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/monitor/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/monitor/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/monitor/module.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/monitor/rkm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.130511 kerch-0.3.1.2/kerch/opt/
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/opt/Optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/opt/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.130511 kerch-0.3.1.2/kerch/plot/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/plot/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9538 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/plot/matplotlib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.130511 kerch-0.3.1.2/kerch/script/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/script/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/script/_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/script/expe.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/script/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/script/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.130511 kerch-0.3.1.2/kerch/train/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/train/Hyper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/train/Trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/train/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.134511 kerch-0.3.1.2/kerch/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/utils/arch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/utils/cast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/utils/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/utils/tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/utils/type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.134511 kerch-0.3.1.2/kerch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15339 2024-05-28 15:29:25.000000 kerch-0.3.1.2/kerch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-28 15:29:25.000000 kerch-0.3.1.2/kerch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:29:25.000000 kerch-0.3.1.2/kerch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 15:29:25.000000 kerch-0.3.1.2/kerch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 15:29:25.000000 kerch-0.3.1.2/kerch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-28 15:29:18.000000 kerch-0.3.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:29:25.134511 kerch-0.3.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 15:29:19.000000 kerch-0.3.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.315999 kerch-0.3.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-28 15:36:07.000000 kerch-0.3.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-28 15:36:07.000000 kerch-0.3.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15339 2024-05-28 15:36:11.315999 kerch-0.3.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-28 15:36:07.000000 kerch-0.3.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.300000 kerch-0.3.1.3/kerch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/_dataholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/_stochastic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.300000 kerch-0.3.1.3/kerch/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/data/_LearningSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/data/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.300000 kerch-0.3.1.3/kerch/feature/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/feature/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13689 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/feature/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/feature/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/feature/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12459 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/feature/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/feature/stochastic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.304000 kerch-0.3.1.3/kerch/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/kernel/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12328 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/kernel/_base_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/kernel/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/kernel/explicit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/kernel/implicit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15564 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/kernel/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7649 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/kernel/nystrom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.304000 kerch-0.3.1.3/kerch/level/
+-rw-r--r--   0 runner    (1001) docker     (127)    14868 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/level/_KPCA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/level/_Level.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11645 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/level/_PPCA.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16228 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/level/_View.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/level/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/level/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.304000 kerch-0.3.1.3/kerch/method/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/method/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/method/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/method/_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/method/_knn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/method/_smoother.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.307999 kerch-0.3.1.3/kerch/monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/monitor/Local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/monitor/Plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/monitor/Saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/monitor/WandB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/monitor/Watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/monitor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/monitor/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/monitor/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/monitor/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/monitor/rkm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.307999 kerch-0.3.1.3/kerch/opt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/opt/Optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/opt/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.307999 kerch-0.3.1.3/kerch/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/plot/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9538 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/plot/matplotlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.307999 kerch-0.3.1.3/kerch/preimage/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/preimage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/preimage/iterative.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/preimage/knn.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/preimage/ridge_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/preimage/smoother.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.311999 kerch-0.3.1.3/kerch/script/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/script/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/script/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/script/expe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/script/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/script/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.311999 kerch-0.3.1.3/kerch/train/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/train/Hyper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/train/Trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/train/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.311999 kerch-0.3.1.3/kerch/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/transform/Transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/transform/TransformTree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/transform/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.315999 kerch-0.3.1.3/kerch/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/utils/arch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/utils/cast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/utils/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/utils/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-28 15:36:07.000000 kerch-0.3.1.3/kerch/utils/type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:36:11.315999 kerch-0.3.1.3/kerch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15339 2024-05-28 15:36:11.000000 kerch-0.3.1.3/kerch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-28 15:36:11.000000 kerch-0.3.1.3/kerch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:36:11.000000 kerch-0.3.1.3/kerch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 15:36:11.000000 kerch-0.3.1.3/kerch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 15:36:11.000000 kerch-0.3.1.3/kerch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-05-28 15:36:07.000000 kerch-0.3.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:36:11.315999 kerch-0.3.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 15:36:07.000000 kerch-0.3.1.3/setup.py
```

### Comparing `kerch-0.3.1.2/LICENSE` & `kerch-0.3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/PKG-INFO` & `kerch-0.3.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kerch
-Version: 0.3.1.2
+Version: 0.3.1.3
 Summary: Kernel Methods in PyTorch
 Author-email: Henri DE PLAEN <henri.deplaen@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `kerch-0.3.1.2/README.md` & `kerch-0.3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/__init__.py` & `kerch-0.3.1.3/kerch/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-__version__ = "0.3.1.2"
+__version__ = "0.3.1.3"
 __author__ = "HENRI DE PLAEN"
 __credits__ = "KU Leuven"
 __status__ = "beta"
 __date__ = "May 2024"
 __license__ = "LGPL-3.0"
 
 # GLOBAL MODULE-WIDE VARIABLES
```

### Comparing `kerch-0.3.1.2/kerch/_cache.py` & `kerch-0.3.1.3/kerch/_cache.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/_dataholder.py` & `kerch-0.3.1.3/kerch/_dataholder.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/_logger.py` & `kerch-0.3.1.3/kerch/_logger.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/_module.py` & `kerch-0.3.1.3/kerch/_module.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/_sample.py` & `kerch-0.3.1.3/kerch/_sample.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/_stochastic.py` & `kerch-0.3.1.3/kerch/_stochastic.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/data/_LearningSet.py` & `kerch-0.3.1.3/kerch/data/_LearningSet.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/data/datasets.py` & `kerch-0.3.1.3/kerch/data/datasets.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/data/factory.py` & `kerch-0.3.1.3/kerch/data/factory.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/kernel/__init__.pyi` & `kerch-0.3.1.3/kerch/kernel/__init__.pyi`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/kernel/_base_kernel.py` & `kerch-0.3.1.3/kerch/kernel/_base_kernel.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/kernel/_factory.py` & `kerch-0.3.1.3/kerch/kernel/_factory.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/kernel/explicit.py` & `kerch-0.3.1.3/kerch/kernel/explicit.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/kernel/implicit.py` & `kerch-0.3.1.3/kerch/kernel/implicit.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/kernel/kernel.py` & `kerch-0.3.1.3/kerch/kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/kernel/nystrom.py` & `kerch-0.3.1.3/kerch/kernel/nystrom.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/level/_KPCA.py` & `kerch-0.3.1.3/kerch/level/_KPCA.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/level/_Level.py` & `kerch-0.3.1.3/kerch/level/_Level.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/level/_PPCA.py` & `kerch-0.3.1.3/kerch/level/_PPCA.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/level/_View.py` & `kerch-0.3.1.3/kerch/level/_View.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/level/factory.py` & `kerch-0.3.1.3/kerch/level/factory.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/method/_iterative.py` & `kerch-0.3.1.3/kerch/method/_iterative.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/method/_knn.py` & `kerch-0.3.1.3/kerch/method/_knn.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/method/_smoother.py` & `kerch-0.3.1.3/kerch/method/_smoother.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/model/view.py` & `kerch-0.3.1.3/kerch/train/Trainer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,227 +1,229 @@
-"""
-Abstract RKM View class.
-
-@author: HENRI DE PLAEN
-@copyright: KU LEUVEN
-@license: MIT
-@date: March 2021, rewritten in June 2022
-"""
+# coding=utf-8
+from __future__ import annotations
 
 import torch
-from torch import Tensor
-from math import sqrt
-
-import kerch.rkm
-from kerch import utils
-from kerch.kernel import factory, _Base
-from kerch._sample import _Sample
-from ._view import _View
-
-
-@utils.extend_docstring(_Sample)
-class View(_View, _Sample):
-    r"""
-    :param kernel: Initiates a View _Based on an existing kernel object. If the value is not `None`, all other
-        parameters are neglected and inherited from the provided kernel., default to `None`
-    :param bias: Bias
-    :param bias_trainable: defaults to `False`
-
-    :type kernel: kerch.kernel._Projected, optional
-    :type bias: bool, optional
-    :type bias_trainable: bool, optional
-    """
-
-    @utils.kwargs_decorator({
-        "kernel": None,
-        "bias": False,
-        "bias_trainable": False,
-        "kappa": 1.,
-        "targets" : None
-    })
-    def __init__(self, *args, **kwargs):
-        """
-        A View is made of a kernel and primal or dual variables. This second part is handled by the daughter classes.
-        """
-        super(View, self).__init__(*args, **kwargs)
+from torch.utils.data import SequentialSampler
+import tqdm
 
-        # KAPPA
-        self._kappa = kwargs["kappa"]
-        self._kappa_sqrt = sqrt(self._kappa)
-        self._mask = None
-
-        # BIAS
-        self._bias_trainable = kwargs["bias_trainable"]
-        self._requires_bias = kwargs["bias"]
-        self._bias = torch.nn.Parameter(torch.empty(0, dtype=utils.FTYPE),
-                                        requires_grad=self._bias_trainable)
-
-
-        # KERNEL INIT
-        # always share sample with kernel
-        kernel = kwargs["kernel"]
-        if kernel is None:
-            self._kernel = factory(**{**kwargs,
-                                      "sample": self.sample,
-                                      "idx_sample": self.idx})
-        elif isinstance(kernel, _Base):
-            self._log.info("Initiating View _Based on existing kernel and overwriting its sample.")
-            self._kernel = kernel
-            self._kernel.init_sample(sample=self.sample,
-                                     idx_sample=self.idx)
+from ..model.Model import Model
+from ..feature.logger import Logger
+from ..utils import kwargs_decorator
+from ..opt import Optimizer
+from ..data import _LearningSet
+from .. import monitor
+
+
+class Trainer(Logger):
+    def __init__(self, model: Model, learning_set: _LearningSet, **kwargs):
+        super(Trainer, self).__init__(**kwargs)
+        self._learning_set: _LearningSet = learning_set
+        self._model: Model = model
+        self.problem = kwargs.pop('problem', 'regression')
+        self.batch_size = kwargs.pop('batch_size', 'all')
+        self.epochs = kwargs.pop('epochs', 100)
+        self.use_gpu = kwargs.pop('use_gpu', False)
+        self.stiefel_lr = kwargs.pop('stiefel_lr', 1e-3)
+        self.euclidean_lr = kwargs.pop('euclidean_lr', 1e-3)
+        self.slow_lr = kwargs.pop('slow_lr', 1e-4)
+        self._verbose = kwargs.pop('verbose', False)
+        self._watcher_kwargs = kwargs.pop('watcher', dict())
+        self._expe_name = kwargs.pop('expe_name', 'expe')
+
+    @property
+    def problem(self) -> str:
+        return self._problem
+
+    @problem.setter
+    def problem(self, val: str):
+        msg = "The problem argument can either be set to the strings 'regression' or 'classification'."
+        assert isinstance(val, str), msg
+        if val == 'regression':
+            self._loss = torch.nn.MSELoss(reduction='mean')
+        elif val == 'classification':
+            raise NotImplementedError
         else:
-            raise TypeError("Argument kernel is not of the kernel class.")
-
-        # TARGETS
-        targets = kwargs["targets"]
-        targets = utils.castf(targets, tensor=True)
-        if self._dim_output is None and targets is not None:
-            self._dim_output = targets.shape[1]
-        self.targets = targets
-
-
+            raise AssertionError(msg)
+        self._problem = val
 
-        self._log.debug("View initialized with " + str(self._kernel))
+    @property
+    def model(self) -> Model:
+        return self._model
 
-    def __str__(self):
-        return "view with " + str(self._kernel)
+    @property
+    def epochs(self) -> int:
+        return self._epochs
 
-    def _reset_weight(self) -> None:
-        self._weight = torch.nn.Parameter(torch.empty(0, dtype=utils.FTYPE,
-                                                      device=self._weight.device),
-                                          requires_grad=self._weight.requires_grad)
+    @epochs.setter
+    def epochs(self, val: int):
+        assert val > 0, "The number of epochs must be strictly positive."
+        self._epochs = val
 
     @property
-    def kappa(self) -> float:
-        return self._kappa
+    def batch_size(self) -> int | str:
+        return self._batch_size
 
-    @kappa.setter
-    def kappa(self, val:float):
-        self._kappa = val
+    @batch_size.setter
+    def batch_size(self, val: int | str):
+        msg = "The batch_size argument can only take an integer or the string 'all' as valid option."
+        num = len(self._learning_set.training_set)
+        if isinstance(val, str):
+            assert val == 'all', msg
+            self._sampler = torch.utils.data.BatchSampler(SequentialSampler(range(num)),
+                                                          batch_size=num, drop_last=False)
+        else:
+            assert isinstance(val, int), msg
+            assert val > 0, \
+                f"Only positive values for the batch size are allowed ({val} given)."
+            assert val <= num, \
+                f"The batch size ({val}) cannot be greater than the number of elements in the training set ({num})."
+            self._sampler = torch.utils.data.BatchSampler(SequentialSampler(range(num)),
+                                                          batch_size=val, drop_last=False)
+        self._batch_size = val
 
     @property
-    def bias(self) -> Tensor:
-        if self._bias.nelement() != 0:
-            return self._bias
-        self._log.debug("No bias has been initialized yet.")
-
-    @bias.setter
-    def bias(self, val):
-        if val is not None:
-            val = utils.castf(val, dev=self._bias.device).squeeze()
-            dim_val = len(val.shape)
+    def _mask_batch_progress(self) -> bool:
+        return self.batch_size == 'all'
 
-            # verifying the shape of the bias
-            if dim_val == 0:
-                val = val.repeat(self._dim_output)
-            elif dim_val > 1:
-                self._log.error("The bias can only be set to a scalar or a vector. "
-                                "This operation is thus discarded.")
-            # setting the value
-            if self._bias.nelement() == 0:
-                self._bias = torch.nn.Parameter(val,
-                                                requires_grad=self._bias_trainable)
-            else:
-                self._bias.data = val
-                # zeroing the gradients if relevant
-                if self._bias_trainable:
-                    self._bias.grad.sample.zero_()
+    @property
+    def _training_data(self) -> torch.Tensor:
+        return (self._learning_set.training_set[:])[0]
 
     @property
-    def bias_trainable(self) -> bool:
-        return self._bias_trainable
+    def _training_labels(self) -> torch.Tensor:
+        return (self._learning_set.training_set[:])[1]
 
-    @bias_trainable.setter
-    def bias_trainable(self, val: bool):
-        self._bias_trainable = val
-        self._bias.requires_grad = self._bias_trainable
+    @property
+    def _validation_data(self) -> torch.Tensor:
+        return (self._learning_set.validation_set[:])[0]
 
     @property
-    def _bias_exists(self) -> bool:
-        return self._bias.nelement() != 0
+    def _validation_labels(self) -> torch.Tensor:
+        return (self._learning_set.validation_set[:])[1]
 
-    ####################################################################################################################
-    ## TARGETS
+    @property
+    def _test_data(self) -> torch.Tensor:
+        return (self._learning_set.test_set[:])[0]
 
     @property
-    def targets(self) -> Tensor:
-        r"""
-            Targets to be matched to.
-        """
-        if self._targets is None:
-            self._log.warning("Empty target values.")
-        return self._targets
-
-    @targets.setter
-    def targets(self, val):
-        val = utils.castf(val, dev=self._sample.device, tensor=True)
-        if val is None:
-            self._log.debug("Targets set to empty values.")
-        else:
-            assert self.dim_output == val.shape[1], f"The shape of the given target {val.shape[1]} does not match the" \
-                                                    f" required one {self.dim_output}."
-            assert self.num_sample == val.shape[0], f"The number of target points {val.shape[0]} does not match the " \
-                                                    f"required one {self.dim_input}."
-        self._targets = torch.nn.Parameter(val)
+    def _test_labels(self) -> torch.Tensor:
+        return (self._learning_set.test_set[:])[1]
 
     @property
-    def current_targets(self) -> Tensor:
+    def use_gpu(self) -> bool:
         r"""
-            Returns the targets that are currently used in the computations and for the normalizing and centering
-            statistics if relevant.
+        Specifies whether the gpu has to be used
         """
-        return self.targets[self.idx, :]
+        return self._use_gpu
 
+    @use_gpu.setter
+    def use_gpu(self, val: bool):
+        self._use_gpu = val
 
-    ########################################################################
     @property
-    def dim_feature(self) -> int:
-        return self.kernel.dim_feature
-
-    @property
-    def kernel(self) -> _Base:
+    def stiefel_lr(self) -> float:
         r"""
-        The kernel used by the model or View.
+        Learning rate for the Stiefel manifold
         """
-        return self._kernel
+        return self._stiefel_lr
+
+    @stiefel_lr.setter
+    def stiefel_lr(self, val: float):
+        self._stiefel_lr = val
 
-    def set_kernel(self, val: _Base):
+    @property
+    def euclidean_lr(self) -> float:
         r"""
-        For some obscure reason, this does not work as a setter (@kernel.setter).
-        TODO: find out why and solve
+        Learning rate for the Euclidean manifold, i.e. the 'normal' parameters.
         """
-        self._log.info("Updating View _Based on an external kernel and overwriting its sample.")
-        self._kernel = val
-        self._kernel.init_sample(sample=self.sample,
-                                 idx_sample=self.idx)
-
-    #########################################################################
-    ## WEIGHT
-    def _update_weight_from_hidden(self):
-        if self._hidden_exists:
-            # will return a ExplicitError if not available
-            self.weight = self.Phi.T @ self.H
-            self._log.debug("Setting the weight _Based on the hidden values.")
-        else:
-            self._log.info("The weight cannot _Based on the hidden values as these are unset.")
-
-    def _update_hidden_from_weight(self):
-        raise NotImplementedError
-
-    ## MATHS
-
-    def phi(self, x=None) -> Tensor:
-        return self._kappa_sqrt * self.kernel.phi(x)
+        return self._euclidean_lr
 
-    def k(self, x=None) -> Tensor:
-        return self.kappa * self.kernel.k(x)
+    @euclidean_lr.setter
+    def euclidean_lr(self, val: float):
+        self._euclidean_lr = val
 
     @property
-    def K(self) -> Tensor:
-        return self.kappa * self.kernel.K
+    def slow_lr(self) -> float:
+        r"""
+        Learning rate for specific hyperparameters that are better trained slower, i.e. the bandwidth of
+        an RBF kernel.
+        """
+        return self._slow_lr
 
-    def forward(self, x=None, representation=None):
-        representation = utils.check_representation(representation, default=self._representation)
-        if self._bias_exists:
-            return self.phiw(x, representation) + self._kappa_sqrt * self._bias[:, None]
-        else:
-            return self.phiw(x, representation)
+    @slow_lr.setter
+    def slow_lr(self, val: float):
+        self._slow_lr = val
+
+    def _init_fit(self):
+        if self.use_gpu:
+            self.model.to('cuda:0')
+
+        self.model.init_sample(self._training_data)
+        self.model.init_levels()
+        self.model.init_target(self._training_labels)
+
+        self._optimizer = Optimizer(module=self.model,
+                                    stiefel_lr=self._stiefel_lr,
+                                    euclidean_lr=self._euclidean_lr,
+                                    slow_lr=self._slow_lr)
+
+    @torch.no_grad()
+    def _problem_loss(self, data, labels) -> float:
+        if len(data) == 0:
+            return 0.
+        self.model.eval()
+        pred = self.model(data)
+        self.model.train()
+        return self._loss(pred, labels)
+
+    def fit(self) -> Model:
+        self._init_fit()
+        self.model.train()
+
+        epoch_progress = tqdm.tqdm(range(self.epochs),
+                                   position=0,
+                                   leave=True,
+                                   desc="Epoch",
+                                   disable=not self._verbose)
+        batch_progress = tqdm.tqdm(self._sampler,
+                                   position=0,
+                                   leave=False,
+                                   disable=self._mask_batch_progress or not self._verbose,
+                                   desc="Batch")
+
+        watcher = monitor.factory(model=self.model, opt=self._optimizer, expe_name=self._expe_name,
+                                  verbose=self._verbose, **self._watcher_kwargs)
+
+        def closure():
+            self.model()
+            loss = self._model.loss()
+            if self._optimizer.requires_grad:
+                loss.backward()
+            return loss
+
+        # TRAINING LOOP
+        for epoch in epoch_progress:
+            # preliminaries
+            self._optimizer.zero_grad()
+            if self.use_gpu:
+                torch.cuda.empty_cache()
+            batch_loss = 0.
+            # forward and backward
+            for idx_batch in batch_progress:
+                self.model.before_step()
+                self.model.stochastic(idx=idx_batch)
+                batch_loss += self._optimizer.step(closure)
+                self.model.after_step()
+
+            # validation and test
+            train_loss = self._problem_loss(self._training_data, self._training_labels)
+            val_loss = self._problem_loss(self._validation_data, self._validation_labels)
+            test_loss = self._problem_loss(self._test_data, self._test_labels)
+            watcher.update(epoch=epoch,
+                           objective_loss=batch_loss,
+                           training_error=train_loss,
+                           validation_error=val_loss,
+                           test_error=test_loss)
+
+        watcher.finish()
+        self.model.eval()
+        return self.model
```

### Comparing `kerch-0.3.1.2/kerch/monitor/Plotter.py` & `kerch-0.3.1.3/kerch/monitor/Plotter.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/monitor/Saver.py` & `kerch-0.3.1.3/kerch/monitor/Saver.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/monitor/WandB.py` & `kerch-0.3.1.3/kerch/monitor/WandB.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/monitor/Watcher.py` & `kerch-0.3.1.3/kerch/monitor/Watcher.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/monitor/factory.py` & `kerch-0.3.1.3/kerch/monitor/factory.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/monitor/model.py` & `kerch-0.3.1.3/kerch/monitor/model.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/monitor/module.py` & `kerch-0.3.1.3/kerch/monitor/module.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/monitor/rkm.py` & `kerch-0.3.1.3/kerch/monitor/rkm.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/opt/Optimizer.py` & `kerch-0.3.1.3/kerch/opt/Optimizer.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/plot/matplotlib.py` & `kerch-0.3.1.3/kerch/plot/matplotlib.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/script/_parser.py` & `kerch-0.3.1.3/kerch/script/_parser.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/script/expe.py` & `kerch-0.3.1.3/kerch/script/expe.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/script/version.py` & `kerch-0.3.1.3/kerch/script/version.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/utils/__init__.pyi` & `kerch-0.3.1.3/kerch/utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/utils/arch.py` & `kerch-0.3.1.3/kerch/utils/arch.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/utils/cast.py` & `kerch-0.3.1.3/kerch/utils/cast.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/utils/decorators.py` & `kerch-0.3.1.3/kerch/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/utils/defaults.py` & `kerch-0.3.1.3/kerch/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/utils/errors.py` & `kerch-0.3.1.3/kerch/utils/errors.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/utils/math.py` & `kerch-0.3.1.3/kerch/utils/math.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/utils/tensor.py` & `kerch-0.3.1.3/kerch/utils/tensor.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch/utils/type.py` & `kerch-0.3.1.3/kerch/utils/type.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.2/kerch.egg-info/PKG-INFO` & `kerch-0.3.1.3/kerch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kerch
-Version: 0.3.1.2
+Version: 0.3.1.3
 Summary: Kernel Methods in PyTorch
 Author-email: Henri DE PLAEN <henri.deplaen@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `kerch-0.3.1.2/kerch.egg-info/SOURCES.txt` & `kerch-0.3.1.3/kerch.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -16,14 +16,21 @@
 kerch.egg-info/requires.txt
 kerch.egg-info/top_level.txt
 kerch/data/_LearningSet.py
 kerch/data/__init__.py
 kerch/data/__init__.pyi
 kerch/data/datasets.py
 kerch/data/factory.py
+kerch/feature/__init__.py
+kerch/feature/__init__.pyi
+kerch/feature/cache.py
+kerch/feature/logger.py
+kerch/feature/module.py
+kerch/feature/sample.py
+kerch/feature/stochastic.py
 kerch/kernel/__init__.py
 kerch/kernel/__init__.pyi
 kerch/kernel/_base_kernel.py
 kerch/kernel/_factory.py
 kerch/kernel/explicit.py
 kerch/kernel/implicit.py
 kerch/kernel/kernel.py
@@ -36,27 +43,14 @@
 kerch/level/__init__.pyi
 kerch/level/factory.py
 kerch/method/__init__.py
 kerch/method/__init__.pyi
 kerch/method/_iterative.py
 kerch/method/_knn.py
 kerch/method/_smoother.py
-kerch/model/KPCA.py
-kerch/model/LSSVM.py
-kerch/model/Model.py
-kerch/model/RKM.py
-kerch/model/__init__.py
-kerch/model/__init__.pyi
-kerch/model/_kpca.py
-kerch/model/_level.py
-kerch/model/_view.py
-kerch/model/factory.py
-kerch/model/level.py
-kerch/model/ridge.py
-kerch/model/view.py
 kerch/monitor/Local.py
 kerch/monitor/Plotter.py
 kerch/monitor/Saver.py
 kerch/monitor/WandB.py
 kerch/monitor/Watcher.py
 kerch/monitor/__init__.py
 kerch/monitor/__init__.pyi
@@ -66,24 +60,33 @@
 kerch/monitor/rkm.py
 kerch/opt/Optimizer.py
 kerch/opt/__init__.py
 kerch/opt/__init__.pyi
 kerch/plot/__init__.py
 kerch/plot/__init__.pyi
 kerch/plot/matplotlib.py
+kerch/preimage/__init__.py
+kerch/preimage/iterative.py
+kerch/preimage/knn.py
+kerch/preimage/ridge_regression.py
+kerch/preimage/smoother.py
 kerch/script/__init__.py
 kerch/script/__init__.pyi
 kerch/script/_parser.py
 kerch/script/expe.py
 kerch/script/main.py
 kerch/script/version.py
 kerch/train/Hyper.py
 kerch/train/Trainer.py
 kerch/train/__init__.py
 kerch/train/__init__.pyi
+kerch/transform/Transform.py
+kerch/transform/TransformTree.py
+kerch/transform/__init__.py
+kerch/transform/__init__.pyi
 kerch/utils/__init__.py
 kerch/utils/__init__.pyi
 kerch/utils/arch.py
 kerch/utils/cast.py
 kerch/utils/decorators.py
 kerch/utils/defaults.py
 kerch/utils/dict.py
```

### Comparing `kerch-0.3.1.2/pyproject.toml` & `kerch-0.3.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -59,19 +59,21 @@
 
 [tool.setuptools.dynamic]
 version = {attr = "kerch.__version__"}
 
 [tool.setuptools]
 packages = [
     "kerch",
+    "kerch.data",
+    "kerch.feature",
     "kerch.kernel",
     "kerch.level",
-    "kerch.model",
-    "kerch.data",
-    "kerch.train",
+    "kerch.method",
     "kerch.monitor",
-    "kerch.plot",
     "kerch.opt",
+    "kerch.plot",
+    "kerch.preimage",
     "kerch.script",
-    "kerch.method",
+    "kerch.train",
+    "kerch.transform",
     "kerch.utils"
 ]
```

