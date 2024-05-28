# Comparing `tmp/kerch-0.3.1.1.post1.tar.gz` & `tmp/kerch-0.3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kerch-0.3.1.1.post1.tar", last modified: Fri May 24 14:31:53 2024, max compression
+gzip compressed data, was "kerch-0.3.1.2.tar", last modified: Tue May 28 15:29:25 2024, max compression
```

## Comparing `kerch-0.3.1.1.post1.tar` & `kerch-0.3.1.2.tar`

### file list

```diff
@@ -1,22 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:31:53.733945 kerch-0.3.1.1.post1/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-24 14:31:49.000000 kerch-0.3.1.1.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-24 14:31:49.000000 kerch-0.3.1.1.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15345 2024-05-24 14:31:53.733945 kerch-0.3.1.1.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-24 14:31:49.000000 kerch-0.3.1.1.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:31:53.729945 kerch-0.3.1.1.post1/kerch/
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-24 14:31:50.000000 kerch-0.3.1.1.post1/kerch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-24 14:31:50.000000 kerch-0.3.1.1.post1/kerch/_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-24 14:31:50.000000 kerch-0.3.1.1.post1/kerch/_dataholder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-24 14:31:50.000000 kerch-0.3.1.1.post1/kerch/_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-24 14:31:50.000000 kerch-0.3.1.1.post1/kerch/_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-24 14:31:50.000000 kerch-0.3.1.1.post1/kerch/_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-24 14:31:50.000000 kerch-0.3.1.1.post1/kerch/_stochastic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:31:53.733945 kerch-0.3.1.1.post1/kerch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15345 2024-05-24 14:31:53.000000 kerch-0.3.1.1.post1/kerch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-24 14:31:53.000000 kerch-0.3.1.1.post1/kerch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 14:31:53.000000 kerch-0.3.1.1.post1/kerch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-24 14:31:53.000000 kerch-0.3.1.1.post1/kerch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-24 14:31:53.000000 kerch-0.3.1.1.post1/kerch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-05-24 14:31:50.000000 kerch-0.3.1.1.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 14:31:53.733945 kerch-0.3.1.1.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-24 14:31:50.000000 kerch-0.3.1.1.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.134511 kerch-0.3.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-28 15:29:18.000000 kerch-0.3.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-28 15:29:18.000000 kerch-0.3.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15339 2024-05-28 15:29:25.134511 kerch-0.3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-28 15:29:18.000000 kerch-0.3.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.118511 kerch-0.3.1.2/kerch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/_dataholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/_stochastic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.118511 kerch-0.3.1.2/kerch/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/data/_LearningSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/data/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.122511 kerch-0.3.1.2/kerch/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/kernel/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12328 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/kernel/_base_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/kernel/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/kernel/explicit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/kernel/implicit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15564 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/kernel/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7649 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/kernel/nystrom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.122511 kerch-0.3.1.2/kerch/level/
+-rw-r--r--   0 runner    (1001) docker     (127)    14868 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/level/_KPCA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/level/_Level.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11645 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/level/_PPCA.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16228 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/level/_View.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/level/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/level/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.122511 kerch-0.3.1.2/kerch/method/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/method/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/method/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/method/_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/method/_knn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/method/_smoother.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.126510 kerch-0.3.1.2/kerch/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/KPCA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/LSSVM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/RKM.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/_kpca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/ridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/model/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.126510 kerch-0.3.1.2/kerch/monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/monitor/Local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/monitor/Plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/monitor/Saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/monitor/WandB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/monitor/Watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/monitor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/monitor/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/monitor/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/monitor/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/monitor/rkm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.130511 kerch-0.3.1.2/kerch/opt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/opt/Optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/opt/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.130511 kerch-0.3.1.2/kerch/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/plot/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9538 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/plot/matplotlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.130511 kerch-0.3.1.2/kerch/script/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/script/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/script/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/script/expe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/script/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/script/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.130511 kerch-0.3.1.2/kerch/train/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/train/Hyper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7739 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/train/Trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/train/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.134511 kerch-0.3.1.2/kerch/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/utils/arch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/utils/cast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/utils/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/utils/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-28 15:29:18.000000 kerch-0.3.1.2/kerch/utils/type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:29:25.134511 kerch-0.3.1.2/kerch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15339 2024-05-28 15:29:25.000000 kerch-0.3.1.2/kerch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-28 15:29:25.000000 kerch-0.3.1.2/kerch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:29:25.000000 kerch-0.3.1.2/kerch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 15:29:25.000000 kerch-0.3.1.2/kerch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 15:29:25.000000 kerch-0.3.1.2/kerch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-28 15:29:18.000000 kerch-0.3.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:29:25.134511 kerch-0.3.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-28 15:29:19.000000 kerch-0.3.1.2/setup.py
```

### Comparing `kerch-0.3.1.1.post1/LICENSE` & `kerch-0.3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.1.post1/PKG-INFO` & `kerch-0.3.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kerch
-Version: 0.3.1.1.post1
+Version: 0.3.1.2
 Summary: Kernel Methods in PyTorch
 Author-email: Henri DE PLAEN <henri.deplaen@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `kerch-0.3.1.1.post1/README.md` & `kerch-0.3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.1.post1/kerch/__init__.py` & `kerch-0.3.1.2/kerch/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding=utf-8
-__version__ = "0.3.1.1post1"
+__version__ = "0.3.1.2"
 __author__ = "HENRI DE PLAEN"
 __credits__ = "KU Leuven"
 __status__ = "beta"
-__date__ = "January 2024"
+__date__ = "May 2024"
 __license__ = "LGPL-3.0"
 
 # GLOBAL MODULE-WIDE VARIABLES
 _GLOBALS = {"PLOT_ENV": None,
             "LOG_LEVEL": 30,  # this corresponds to logging.WARNING
             }
```

### Comparing `kerch-0.3.1.1.post1/kerch/_cache.py` & `kerch-0.3.1.2/kerch/_cache.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.1.post1/kerch/_dataholder.py` & `kerch-0.3.1.2/kerch/_dataholder.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.1.post1/kerch/_logger.py` & `kerch-0.3.1.2/kerch/_logger.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.1.post1/kerch/_module.py` & `kerch-0.3.1.2/kerch/_module.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.1.post1/kerch/_sample.py` & `kerch-0.3.1.2/kerch/_sample.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.1.post1/kerch/_stochastic.py` & `kerch-0.3.1.2/kerch/_stochastic.py`

 * *Files identical despite different names*

### Comparing `kerch-0.3.1.1.post1/kerch.egg-info/PKG-INFO` & `kerch-0.3.1.2/kerch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kerch
-Version: 0.3.1.1.post1
+Version: 0.3.1.2
 Summary: Kernel Methods in PyTorch
 Author-email: Henri DE PLAEN <henri.deplaen@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `kerch-0.3.1.1.post1/pyproject.toml` & `kerch-0.3.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -57,8 +57,21 @@
 E-DUALITY = "https://www.esat.kuleuven.be/stadius/E/"
 ESAT-STADIUS = "https://www.esat.kuleuven.be/stadius/"
 
 [tool.setuptools.dynamic]
 version = {attr = "kerch.__version__"}
 
 [tool.setuptools]
-packages = ["kerch"]
+packages = [
+    "kerch",
+    "kerch.kernel",
+    "kerch.level",
+    "kerch.model",
+    "kerch.data",
+    "kerch.train",
+    "kerch.monitor",
+    "kerch.plot",
+    "kerch.opt",
+    "kerch.script",
+    "kerch.method",
+    "kerch.utils"
+]
```

