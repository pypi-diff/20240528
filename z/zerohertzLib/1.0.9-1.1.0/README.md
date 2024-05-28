# Comparing `tmp/zerohertzLib-1.0.9.tar.gz` & `tmp/zerohertzLib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerohertzLib-1.0.9.tar", last modified: Wed May 22 18:08:14 2024, max compression
+gzip compressed data, was "zerohertzLib-1.1.0.tar", last modified: Tue May 28 14:49:18 2024, max compression
```

## Comparing `zerohertzLib-1.0.9.tar` & `zerohertzLib-1.1.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:08:14.787715 zerohertzLib-1.0.9/
--rw-r--r--   0 root         (0) root         (0)     1067 2024-05-22 18:08:08.000000 zerohertzLib-1.0.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-22 18:08:08.000000 zerohertzLib-1.0.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3318 2024-05-22 18:08:14.787715 zerohertzLib-1.0.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2316 2024-05-22 18:08:08.000000 zerohertzLib-1.0.9/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 18:08:14.787715 zerohertzLib-1.0.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2704 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:08:14.779715 zerohertzLib-1.0.9/test/
--rw-r--r--   0 root         (0) root         (0)     4501 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/test/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     1822 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/test/test_api.py
--rw-r--r--   0 root         (0) root         (0)     1230 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/test/test_logging.py
--rw-r--r--   0 root         (0) root         (0)      220 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/test/test_monitoring.py
--rw-r--r--   0 root         (0) root         (0)     8641 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/test/test_plot.py
--rw-r--r--   0 root         (0) root         (0)     2150 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/test/test_quant.py
--rw-r--r--   0 root         (0) root         (0)     1961 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/test/test_util.py
--rw-r--r--   0 root         (0) root         (0)    14679 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/test/test_vision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:08:14.779715 zerohertzLib-1.0.9/zerohertzLib/
--rw-r--r--   0 root         (0) root         (0)     1794 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:08:14.779715 zerohertzLib-1.0.9/zerohertzLib/algorithm/
--rw-r--r--   0 root         (0) root         (0)     1040 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/algorithm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2626 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/algorithm/bisect.py
--rw-r--r--   0 root         (0) root         (0)     6708 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/algorithm/collections.py
--rw-r--r--   0 root         (0) root         (0)     2420 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/algorithm/fft.py
--rw-r--r--   0 root         (0) root         (0)     7065 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/algorithm/graph.py
--rw-r--r--   0 root         (0) root         (0)     1676 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/algorithm/prime.py
--rw-r--r--   0 root         (0) root         (0)     8048 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/algorithm/sort.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:08:14.779715 zerohertzLib-1.0.9/zerohertzLib/api/
--rw-r--r--   0 root         (0) root         (0)      446 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3865 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/api/discord.py
--rw-r--r--   0 root         (0) root         (0)    11096 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/api/github.py
--rw-r--r--   0 root         (0) root         (0)    30846 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/api/koreainvestment.py
--rw-r--r--   0 root         (0) root         (0)     5011 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/api/open_ai.py
--rw-r--r--   0 root         (0) root         (0)     7698 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/api/slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:08:14.779715 zerohertzLib-1.0.9/zerohertzLib/logging/
--rw-r--r--   0 root         (0) root         (0)      359 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/logging/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4738 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/logging/handler.py
--rw-r--r--   0 root         (0) root         (0)     5264 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/logging/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:08:14.779715 zerohertzLib-1.0.9/zerohertzLib/mlops/
--rw-r--r--   0 root         (0) root         (0)      273 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/mlops/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18002 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/mlops/triton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:08:14.779715 zerohertzLib-1.0.9/zerohertzLib/monitoring/
--rw-r--r--   0 root         (0) root         (0)      333 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2829 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/monitoring/cpu.py
--rw-r--r--   0 root         (0) root         (0)     5184 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/monitoring/gpu.py
--rw-r--r--   0 root         (0) root         (0)     2678 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/monitoring/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:08:14.779715 zerohertzLib-1.0.9/zerohertzLib/plot/
--rw-r--r--   0 root         (0) root         (0)     1552 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/plot/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15381 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/plot/bar_chart.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:08:14.783715 zerohertzLib-1.0.9/zerohertzLib/plot/fonts/
--rw-r--r--   0 root         (0) root         (0)  7549348 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf
--rw-r--r--   0 root         (0) root         (0)   347988 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/plot/fonts/times.ttf
--rw-r--r--   0 root         (0) root         (0)     3435 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/plot/pie.py
--rw-r--r--   0 root         (0) root         (0)    11476 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/plot/plot.py
--rw-r--r--   0 root         (0) root         (0)     4046 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/plot/scatter.py
--rw-r--r--   0 root         (0) root         (0)     3292 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/plot/table.py
--rw-r--r--   0 root         (0) root         (0)     4838 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/plot/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:08:14.783715 zerohertzLib-1.0.9/zerohertzLib/quant/
--rw-r--r--   0 root         (0) root         (0)      885 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/quant/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14935 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/quant/backtest.py
--rw-r--r--   0 root         (0) root         (0)    13182 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/quant/methods.py
--rw-r--r--   0 root         (0) root         (0)    44465 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/quant/quant.py
--rw-r--r--   0 root         (0) root         (0)     3755 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/quant/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:08:14.783715 zerohertzLib-1.0.9/zerohertzLib/util/
--rw-r--r--   0 root         (0) root         (0)      458 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4527 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/util/csv.py
--rw-r--r--   0 root         (0) root         (0)    11173 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/util/data.py
--rw-r--r--   0 root         (0) root         (0)    11652 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/util/json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:08:14.787715 zerohertzLib-1.0.9/zerohertzLib/vision/
--rw-r--r--   0 root         (0) root         (0)     1623 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/vision/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6967 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/vision/compare.py
--rw-r--r--   0 root         (0) root         (0)    12885 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/vision/convert.py
--rw-r--r--   0 root         (0) root         (0)    22463 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/vision/data.py
--rw-r--r--   0 root         (0) root         (0)    14878 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/vision/eval.py
--rw-r--r--   0 root         (0) root         (0)     4188 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/vision/gif.py
--rw-r--r--   0 root         (0) root         (0)    22281 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/vision/loader.py
--rw-r--r--   0 root         (0) root         (0)     7826 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/vision/transform.py
--rw-r--r--   0 root         (0) root         (0)     4219 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/vision/util.py
--rw-r--r--   0 root         (0) root         (0)    17516 2024-05-22 18:08:09.000000 zerohertzLib-1.0.9/zerohertzLib/vision/visual.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:08:14.779715 zerohertzLib-1.0.9/zerohertzLib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3318 2024-05-22 18:08:14.000000 zerohertzLib-1.0.9/zerohertzLib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1923 2024-05-22 18:08:14.000000 zerohertzLib-1.0.9/zerohertzLib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 18:08:14.000000 zerohertzLib-1.0.9/zerohertzLib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      457 2024-05-22 18:08:14.000000 zerohertzLib-1.0.9/zerohertzLib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-22 18:08:14.000000 zerohertzLib-1.0.9/zerohertzLib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 14:49:18.843528 zerohertzLib-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-05-28 14:49:12.000000 zerohertzLib-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-28 14:49:12.000000 zerohertzLib-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3318 2024-05-28 14:49:18.843528 zerohertzLib-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2316 2024-05-28 14:49:12.000000 zerohertzLib-1.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 14:49:18.843528 zerohertzLib-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2704 2024-05-28 14:49:12.000000 zerohertzLib-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 14:49:18.827528 zerohertzLib-1.1.0/test/
+-rw-r--r--   0 root         (0) root         (0)     4501 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/test/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/test/test_api.py
+-rw-r--r--   0 root         (0) root         (0)     1230 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/test/test_logging.py
+-rw-r--r--   0 root         (0) root         (0)      220 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/test/test_monitoring.py
+-rw-r--r--   0 root         (0) root         (0)     8641 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/test/test_plot.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/test/test_quant.py
+-rw-r--r--   0 root         (0) root         (0)     1961 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/test/test_util.py
+-rw-r--r--   0 root         (0) root         (0)    14679 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/test/test_vision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 14:49:18.827528 zerohertzLib-1.1.0/zerohertzLib/
+-rw-r--r--   0 root         (0) root         (0)     1794 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 14:49:18.831528 zerohertzLib-1.1.0/zerohertzLib/algorithm/
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/algorithm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/algorithm/bisect.py
+-rw-r--r--   0 root         (0) root         (0)     6708 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/algorithm/collections.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/algorithm/fft.py
+-rw-r--r--   0 root         (0) root         (0)     7065 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/algorithm/graph.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/algorithm/prime.py
+-rw-r--r--   0 root         (0) root         (0)     8048 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/algorithm/sort.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 14:49:18.831528 zerohertzLib-1.1.0/zerohertzLib/api/
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3865 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/api/discord.py
+-rw-r--r--   0 root         (0) root         (0)    11096 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/api/github.py
+-rw-r--r--   0 root         (0) root         (0)    30846 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/api/koreainvestment.py
+-rw-r--r--   0 root         (0) root         (0)     5011 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/api/open_ai.py
+-rw-r--r--   0 root         (0) root         (0)     7698 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/api/slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 14:49:18.831528 zerohertzLib-1.1.0/zerohertzLib/logging/
+-rw-r--r--   0 root         (0) root         (0)      359 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/logging/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4738 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/logging/handler.py
+-rw-r--r--   0 root         (0) root         (0)     5264 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/logging/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 14:49:18.831528 zerohertzLib-1.1.0/zerohertzLib/mlops/
+-rw-r--r--   0 root         (0) root         (0)      273 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/mlops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18002 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/mlops/triton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 14:49:18.831528 zerohertzLib-1.1.0/zerohertzLib/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      333 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2829 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/monitoring/cpu.py
+-rw-r--r--   0 root         (0) root         (0)     5184 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/monitoring/gpu.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/monitoring/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 14:49:18.831528 zerohertzLib-1.1.0/zerohertzLib/plot/
+-rw-r--r--   0 root         (0) root         (0)     1552 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/plot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15381 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/plot/bar_chart.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 14:49:18.839528 zerohertzLib-1.1.0/zerohertzLib/plot/fonts/
+-rw-r--r--   0 root         (0) root         (0)  7549348 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf
+-rw-r--r--   0 root         (0) root         (0)   347988 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/plot/fonts/times.ttf
+-rw-r--r--   0 root         (0) root         (0)     3435 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/plot/pie.py
+-rw-r--r--   0 root         (0) root         (0)    11476 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/plot/plot.py
+-rw-r--r--   0 root         (0) root         (0)     4046 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/plot/scatter.py
+-rw-r--r--   0 root         (0) root         (0)     3292 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/plot/table.py
+-rw-r--r--   0 root         (0) root         (0)     4838 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/plot/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 14:49:18.839528 zerohertzLib-1.1.0/zerohertzLib/quant/
+-rw-r--r--   0 root         (0) root         (0)      885 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/quant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14935 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/quant/backtest.py
+-rw-r--r--   0 root         (0) root         (0)    13182 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/quant/methods.py
+-rw-r--r--   0 root         (0) root         (0)    44465 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/quant/quant.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/quant/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 14:49:18.839528 zerohertzLib-1.1.0/zerohertzLib/util/
+-rw-r--r--   0 root         (0) root         (0)      458 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4527 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/util/csv.py
+-rw-r--r--   0 root         (0) root         (0)    11173 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/util/data.py
+-rw-r--r--   0 root         (0) root         (0)    11652 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/util/json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 14:49:18.843528 zerohertzLib-1.1.0/zerohertzLib/vision/
+-rw-r--r--   0 root         (0) root         (0)     1623 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/vision/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6967 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/vision/compare.py
+-rw-r--r--   0 root         (0) root         (0)    12885 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/vision/convert.py
+-rw-r--r--   0 root         (0) root         (0)    22463 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/vision/data.py
+-rw-r--r--   0 root         (0) root         (0)    14878 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/vision/eval.py
+-rw-r--r--   0 root         (0) root         (0)     4188 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/vision/gif.py
+-rw-r--r--   0 root         (0) root         (0)    22281 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/vision/loader.py
+-rw-r--r--   0 root         (0) root         (0)     7826 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/vision/transform.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/vision/util.py
+-rw-r--r--   0 root         (0) root         (0)    17516 2024-05-28 14:49:13.000000 zerohertzLib-1.1.0/zerohertzLib/vision/visual.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 14:49:18.827528 zerohertzLib-1.1.0/zerohertzLib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3318 2024-05-28 14:49:18.000000 zerohertzLib-1.1.0/zerohertzLib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1923 2024-05-28 14:49:18.000000 zerohertzLib-1.1.0/zerohertzLib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 14:49:18.000000 zerohertzLib-1.1.0/zerohertzLib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      457 2024-05-28 14:49:18.000000 zerohertzLib-1.1.0/zerohertzLib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-28 14:49:18.000000 zerohertzLib-1.1.0/zerohertzLib.egg-info/top_level.txt
```

### Comparing `zerohertzLib-1.0.9/LICENSE` & `zerohertzLib-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/PKG-INFO` & `zerohertzLib-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerohertzLib
-Version: 1.0.9
+Version: 1.1.0
 Summary: Zerohertz's Library
 Home-page: https://github.com/Zerohertz/zerohertzLib
 Author: Zerohertz
 Author-email: ohg3417@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.9 Summary: Zerohertz's
+Metadata-Version: 2.1 Name: zerohertzLib Version: 1.1.0 Summary: Zerohertz's
 Library Home-page: https://github.com/Zerohertz/zerohertzLib Author: Zerohertz
 Author-email: ohg3417@gmail.com License: MIT Classifier: Development Status ::
 5 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
 Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Software
```

### Comparing `zerohertzLib-1.0.9/README.md` & `zerohertzLib-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/setup.py` & `zerohertzLib-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/test/test_algorithm.py` & `zerohertzLib-1.1.0/test/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/test/test_api.py` & `zerohertzLib-1.1.0/test/test_api.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/test/test_logging.py` & `zerohertzLib-1.1.0/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/test/test_plot.py` & `zerohertzLib-1.1.0/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/test/test_quant.py` & `zerohertzLib-1.1.0/test/test_quant.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/test/test_util.py` & `zerohertzLib-1.1.0/test/test_util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/test/test_vision.py` & `zerohertzLib-1.1.0/test/test_vision.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/__init__.py` & `zerohertzLib-1.1.0/zerohertzLib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,8 +52,8 @@
     print("=" * 100)
     print(f"[Warning] {error}")
     print("Please Install OpenCV Dependency")
     print("--->\t$ sudo apt install python3-opencv -y\t<---")
     print("(but you can use other submodules except zerohertzLib.vision)")
     print("=" * 100)
 
-__version__ = "v1.0.9"
+__version__ = "v1.1.0"
```

### Comparing `zerohertzLib-1.0.9/zerohertzLib/algorithm/__init__.py` & `zerohertzLib-1.1.0/zerohertzLib/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/algorithm/bisect.py` & `zerohertzLib-1.1.0/zerohertzLib/algorithm/bisect.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/algorithm/collections.py` & `zerohertzLib-1.1.0/zerohertzLib/algorithm/collections.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/algorithm/fft.py` & `zerohertzLib-1.1.0/zerohertzLib/algorithm/fft.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/algorithm/graph.py` & `zerohertzLib-1.1.0/zerohertzLib/algorithm/graph.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/algorithm/prime.py` & `zerohertzLib-1.1.0/zerohertzLib/algorithm/prime.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/algorithm/sort.py` & `zerohertzLib-1.1.0/zerohertzLib/algorithm/sort.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/api/discord.py` & `zerohertzLib-1.1.0/zerohertzLib/api/discord.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/api/github.py` & `zerohertzLib-1.1.0/zerohertzLib/api/github.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/api/koreainvestment.py` & `zerohertzLib-1.1.0/zerohertzLib/api/koreainvestment.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/api/open_ai.py` & `zerohertzLib-1.1.0/zerohertzLib/api/open_ai.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/api/slack.py` & `zerohertzLib-1.1.0/zerohertzLib/api/slack.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/logging/handler.py` & `zerohertzLib-1.1.0/zerohertzLib/logging/handler.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/logging/logger.py` & `zerohertzLib-1.1.0/zerohertzLib/logging/logger.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/mlops/triton.py` & `zerohertzLib-1.1.0/zerohertzLib/mlops/triton.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/monitoring/cpu.py` & `zerohertzLib-1.1.0/zerohertzLib/monitoring/cpu.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/monitoring/gpu.py` & `zerohertzLib-1.1.0/zerohertzLib/monitoring/gpu.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/monitoring/storage.py` & `zerohertzLib-1.1.0/zerohertzLib/monitoring/storage.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/plot/__init__.py` & `zerohertzLib-1.1.0/zerohertzLib/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/plot/bar_chart.py` & `zerohertzLib-1.1.0/zerohertzLib/plot/bar_chart.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf` & `zerohertzLib-1.1.0/zerohertzLib/plot/fonts/NotoSerifKR-Medium.otf`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/plot/fonts/times.ttf` & `zerohertzLib-1.1.0/zerohertzLib/plot/fonts/times.ttf`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/plot/pie.py` & `zerohertzLib-1.1.0/zerohertzLib/plot/pie.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/plot/plot.py` & `zerohertzLib-1.1.0/zerohertzLib/plot/plot.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/plot/scatter.py` & `zerohertzLib-1.1.0/zerohertzLib/plot/scatter.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/plot/table.py` & `zerohertzLib-1.1.0/zerohertzLib/plot/table.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/plot/util.py` & `zerohertzLib-1.1.0/zerohertzLib/plot/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/quant/__init__.py` & `zerohertzLib-1.1.0/zerohertzLib/quant/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/quant/backtest.py` & `zerohertzLib-1.1.0/zerohertzLib/quant/backtest.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/quant/methods.py` & `zerohertzLib-1.1.0/zerohertzLib/quant/methods.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/quant/quant.py` & `zerohertzLib-1.1.0/zerohertzLib/quant/quant.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/quant/util.py` & `zerohertzLib-1.1.0/zerohertzLib/quant/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/util/csv.py` & `zerohertzLib-1.1.0/zerohertzLib/util/csv.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/util/data.py` & `zerohertzLib-1.1.0/zerohertzLib/util/data.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/util/json.py` & `zerohertzLib-1.1.0/zerohertzLib/util/json.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/vision/__init__.py` & `zerohertzLib-1.1.0/zerohertzLib/vision/__init__.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/vision/compare.py` & `zerohertzLib-1.1.0/zerohertzLib/vision/compare.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/vision/convert.py` & `zerohertzLib-1.1.0/zerohertzLib/vision/convert.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/vision/data.py` & `zerohertzLib-1.1.0/zerohertzLib/vision/data.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/vision/eval.py` & `zerohertzLib-1.1.0/zerohertzLib/vision/eval.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/vision/gif.py` & `zerohertzLib-1.1.0/zerohertzLib/vision/gif.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/vision/loader.py` & `zerohertzLib-1.1.0/zerohertzLib/vision/loader.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/vision/transform.py` & `zerohertzLib-1.1.0/zerohertzLib/vision/transform.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/vision/util.py` & `zerohertzLib-1.1.0/zerohertzLib/vision/util.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib/vision/visual.py` & `zerohertzLib-1.1.0/zerohertzLib/vision/visual.py`

 * *Files identical despite different names*

### Comparing `zerohertzLib-1.0.9/zerohertzLib.egg-info/PKG-INFO` & `zerohertzLib-1.1.0/zerohertzLib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerohertzLib
-Version: 1.0.9
+Version: 1.1.0
 Summary: Zerohertz's Library
 Home-page: https://github.com/Zerohertz/zerohertzLib
 Author: Zerohertz
 Author-email: ohg3417@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zerohertzLib Version: 1.0.9 Summary: Zerohertz's
+Metadata-Version: 2.1 Name: zerohertzLib Version: 1.1.0 Summary: Zerohertz's
 Library Home-page: https://github.com/Zerohertz/zerohertzLib Author: Zerohertz
 Author-email: ohg3417@gmail.com License: MIT Classifier: Development Status ::
 5 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
 Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Software
```

### Comparing `zerohertzLib-1.0.9/zerohertzLib.egg-info/SOURCES.txt` & `zerohertzLib-1.1.0/zerohertzLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

