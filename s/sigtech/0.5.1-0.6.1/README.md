# Comparing `tmp/sigtech-0.5.1.tar.gz` & `tmp/sigtech-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigtech-0.5.1.tar", last modified: Mon Mar 25 14:41:40 2024, max compression
+gzip compressed data, was "sigtech-0.6.1.tar", last modified: Tue May 28 16:21:10 2024, max compression
```

## Comparing `sigtech-0.5.1.tar` & `sigtech-0.6.1.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:41:40.327077 sigtech-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-03-25 14:41:08.000000 sigtech-0.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-03-25 14:41:40.327077 sigtech-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-03-25 14:41:08.000000 sigtech-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-03-25 14:41:08.000000 sigtech-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 14:41:40.327077 sigtech-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:41:40.315076 sigtech-0.5.1/sigtech/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:41:40.319076 sigtech-0.5.1/sigtech/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:41:40.319076 sigtech-0.5.1/sigtech/api/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/client/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:41:40.319076 sigtech-0.5.1/sigtech/api/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/datasets/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/datasets/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/datasets/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/datasets/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:41:40.319076 sigtech-0.5.1/sigtech/api/framework/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/framework/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/framework/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/framework/framework_api_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:41:40.319076 sigtech-0.5.1/sigtech/api/framework/indices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/framework/indices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/framework/indices/tradable_index.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:41:40.323076 sigtech-0.5.1/sigtech/api/framework/instruments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/framework/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/framework/instruments/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/framework/instruments/cash.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/framework/instruments/fixes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/framework/instruments/futures.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/framework/instruments/fx_otc.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/framework/instruments/indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/framework/instruments/ir_otc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/framework/instruments/ois_swap.py
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/framework/plot_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:41:40.323076 sigtech-0.5.1/sigtech/api/framework/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/framework/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/framework/strategies/basket_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/framework/strategies/reinvestment_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/framework/strategies/rolling_future_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/framework/strategies/rolling_fx_forward_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/framework/strategies/rolling_swap_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/framework/strategies/signal_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/framework/strategies/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:41:40.323076 sigtech-0.5.1/sigtech/api/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)     8200 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-25 14:41:08.000000 sigtech-0.5.1/sigtech/api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:41:40.323076 sigtech-0.5.1/sigtech.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-03-25 14:41:40.000000 sigtech-0.5.1/sigtech.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-25 14:41:40.000000 sigtech-0.5.1/sigtech.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 14:41:40.000000 sigtech-0.5.1/sigtech.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-25 14:41:40.000000 sigtech-0.5.1/sigtech.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-25 14:41:40.000000 sigtech-0.5.1/sigtech.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:21:10.565661 sigtech-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-28 16:20:34.000000 sigtech-0.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-05-28 16:21:10.565661 sigtech-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-05-28 16:20:34.000000 sigtech-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-28 16:20:34.000000 sigtech-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 16:21:10.565661 sigtech-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:21:10.557661 sigtech-0.6.1/sigtech/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:21:10.557661 sigtech-0.6.1/sigtech/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:21:10.557661 sigtech-0.6.1/sigtech/api/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/client/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:21:10.561661 sigtech-0.6.1/sigtech/api/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/datasets/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/datasets/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/datasets/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9230 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/datasets/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:21:10.561661 sigtech-0.6.1/sigtech/api/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/framework_api_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:21:10.561661 sigtech-0.6.1/sigtech/api/framework/indices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/indices/tradable_index.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:21:10.561661 sigtech-0.6.1/sigtech/api/framework/instruments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/instruments/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/instruments/cash.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/instruments/fixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/instruments/futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/instruments/fx_otc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/instruments/indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/instruments/ir_otc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/instruments/ois_swap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/plot_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:21:10.565661 sigtech-0.6.1/sigtech/api/framework/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/strategies/basket_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/strategies/reinvestment_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/strategies/rolling_bond_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/strategies/rolling_future_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/strategies/rolling_fx_forward_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/strategies/rolling_swap_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/strategies/signal_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/framework/strategies/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:21:10.565661 sigtech-0.6.1/sigtech/api/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 16:20:34.000000 sigtech-0.6.1/sigtech/api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:21:10.565661 sigtech-0.6.1/sigtech.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-05-28 16:21:10.000000 sigtech-0.6.1/sigtech.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-28 16:21:10.000000 sigtech-0.6.1/sigtech.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 16:21:10.000000 sigtech-0.6.1/sigtech.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 16:21:10.000000 sigtech-0.6.1/sigtech.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 16:21:10.000000 sigtech-0.6.1/sigtech.egg-info/top_level.txt
```

### Comparing `sigtech-0.5.1/LICENSE.txt` & `sigtech-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sigtech-0.5.1/PKG-INFO` & `sigtech-0.6.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigtech
-Version: 0.5.1
+Version: 0.6.1
 Summary: SigTech Python SDK
 Author-email: SigTech <support@sigtech.com>
 License: MIT
 Project-URL: Homepage, https://github.com/SIGTechnologies/sigtech-python
 Keywords: SIGTECH,FINANCE,TRADING,BACKTEST,QUANT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -44,24 +44,21 @@
 Requires-Dist: statsmodels; extra == "test"
 
 ![SigTech SDK Banner](https://sigtech.com/wp-content/uploads/2023/08/Python-SDK_github_856x268-1.png "SigTech SDK Banner")
 
 &nbsp;
 
 <p align="center" id="dummy">
-    <a href="https://discord.gg/ZcFeutSrWM">
-        <img src="https://img.shields.io/badge/CHAT-DISCORD-blue?style=for-the-badge&logo=discord&labelColor=rgb(55,55,55)&color=blueviolet">
+    <a href="https://api.sigtech.com/docs">
+        <img src="https://img.shields.io/badge/Docs-API_REFERENCE-1338be?&style=for-the-badge&logo=wiki&link=https://api.sigtech.com/docs" alt="Docs" />
     </a>
-    <a href="https://learn.sigtech.com/reference/">
-        <img src="https://img.shields.io/badge/Docs-API_REFERENCE-1338be?&style=for-the-badge&logo=wiki&link=https://learn.sigtech.com/reference" alt="Docs" />
+     <a href="https://twitter.com/sigtech_ai/">
+        <img src="https://img.shields.io/badge/follow-%40sigtech_ai-1DA1F2?logo=twitter&style=for-the-badge" />
     </a>
-     <a href="https://twitter.com/sigtechltd/">
-        <img src="https://img.shields.io/badge/follow-%40sigtechltd-1DA1F2?logo=twitter&style=for-the-badge" />
-    </a>
-<p>
+</p>
 
 <div align="center">
 
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 ![Stargazers][stars-shield]
 [![Issues][issues-shield]][issues-url]
@@ -83,33 +80,32 @@
 
 The SigTech Python SDK is designed to simplify the usage of the SigTech API for backtesting investment strategies by providing a higher-level, object-oriented method of interfacing with our API. With this SDK, you can easily test and view the performance of historical strategies.
 
 #### Key Features
 
 - Provides a higher-level object-based interface for convenient interaction with the SigTech API.
 - Simplifies the creation of advanced trading strategies by providing methods which simulate rolling future strategies, basket strategies, and more.
-- Interfaces with SigTech's collection of historical performance data facilitating accurate backtesting. Explore the [SigTech API data catalog](https://sigtechapi.streamlit.app/) to see the library of instruments available.
+- Interfaces with SigTech's historical market data facilitating accurate backtesting. Explore the [SigTech API data catalog](https://github.com/SIGTechnologies/sigtech-python/blob/master/docs/data.md) to see the list of instruments available.
 
 ## Installation
 
 ```sh
 pip install sigtech
 ```
 
 ### Requirements
 
 - Python 3.6+
 
-## Getting started with SigTech Python SDK
+## Getting started
 
 ### Authentication
 
-1. [Sign-up](https://dashboard.sigtech.com/register) for our API.
 1. Generate an API key using our [dashboard](https://dashboard.sigtech.com/api-keys).
-1. Secure your API key and save it as a global environment variable by following our instructions [here](https://learn.sigtech.com/docs/auth).
+1. Secure your API key and save it as a global environment variable by following our instructions [here](https://github.com/SIGTechnologies/sigtech-python/blob/master/docs/auth.md).
 
 ### Creating your first strategy
 
 Our SDK provides convenient wrappers for boilerplate functions that are required to interact with our API. Copy the following code into your IDE and run it to quickly create, backtest, and view the performance of a custom rolling futures strategy.
 
 >**Note!**\
 >The example below will only work if you have saved your API key as the global environment variable `SIGTECH_API_KEY`.
@@ -133,51 +129,53 @@
 
 # Retrieve the strategy history
 print(es_future.history())
 ```
 
 ## Next steps
 
-1. Learn more about the API with the [reference guide](https://learn.sigtech.com/reference). 
 1. Follow some of our [examples](https://github.com/SIGTechnologies/sigtech-python/tree/master/examples) to see how you can replicate and backtest more complex, real-world trading strategies.
+1. Explore the full range of available instruments in the [API data catalog](https://github.com/SIGTechnologies/sigtech-python/blob/master/docs/data.md).
+1. Explore the full range of endpoints in the [API reference](https://api.sigtech.com/docs). 
+
+
+
 
 ## Google Colab
 
-We understand that getting started with backtesting and evaluating trading strategies can be a daunting task, especially for users new to financial data analysis and Python development. To make the process as seamless as possible, we've prepared a collection of real-world [examples](https://github.com/SIGTechnologies/sigtech-python/tree/master/examples) in Jupyter Notebook format (.ipynb). All you need to follow along is a SigTech API key.
+We understand that getting started with backtesting and evaluating trading strategies can be a daunting task, especially for users new to financial data analysis and Python development. To make the process as seamless as possible, we've prepared a collection of real-world [examples](https://github.com/SIGTechnologies/sigtech-python/tree/master/examples) in Jupyter Notebook format (`.ipynb`). All you need to follow along is a SigTech API key.
 
 ## Logging
 
 Logs down to the `debug` log level are available for all API requests. They can be accessed using the Python `logging` library.
 
 ```python
 import logging
 logging.basicConfig(level=logging.DEBUG)
 ```
 
-For more information, please refer to the `logging` library's [documentation](https://docs.python.org/3/library/logging.html). See [Logging in Python](https://realpython.com/python-logging/) for a useful summary of the `logging` library's capabilities.
-
-## API Documentation
+For more information, please refer to the `logging` library's [documentation](https://docs.python.org/3/library/logging.html).
 
-For detailed information about the SigTech API, please refer to our official [API user guide](https://learn.sigtech.com/docs) and our interactive [API reference guide](https://learn.sigtech.com/reference).
 
-## Contributing to the SigTech Python SDK
+## Contributing
 
 We appreciate and encourage your contributions to the SigTech Python SDK! If you are enjoying the SDK, please show your support by starring this repository and sharing it on social media channels.
 
 To contribute an example, provide feedback, report a bug or otherwise bring an issue to our attention regarding this project, please follow the steps outlined in the [Contribution guidelines](https://github.com/SIGTechnologies/sigtech-python/blob/master/CONTRIBUTING.md).
 
 Please remember that all contributors are expected to behave appropriately and abide by our [Code of conduct](https://github.com/SIGTechnologies/sigtech-python/blob/master/CODE_OF_CONDUCT.md).
 
-## Reporting security issues
+## Security issues
 
 If you believe you have discovered a security vulnerability in our repository please report it to us immediately following the instructions [here](https://github.com/SIGTechnologies/sigtech-python/blob/master/SECURITY.md).
 
->Attention!\
->Please follow the instructions detailed. **Do not** publicly disclose the vulnerability in a Github Issue or on a public forum such as Discord or Twitter.
+>**Attention!**\
+>Do not publicly disclose the vulnerability in a Github Issue or on a public forum such as X/Twitter.
 
 ## Support
 
-If you encounter any issues or have any questions regarding our API or SDK, you can reach out to us via our [Discord](https://discord.gg/ZcFeutSrWM) or [Twitter](https://twitter.com/sigtechltd/).
+If you encounter any issues or have any questions regarding our API or SDK, 
+you can reach out to us via email at [support@sigtech.com](mailto:support@sigtech.com).
 
 ## License
 
 The SigTech Python SDK is released under the [MIT License](https://github.com/SIGTechnologies/sigtech-python/blob/master/LICENSE).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sigtech Version: 0.5.1 Summary: SigTech Python SDK
+Metadata-Version: 2.1 Name: sigtech Version: 0.6.1 Summary: SigTech Python SDK
 Author-email: SigTech
 sigtech.com> License: MIT Project-URL: Homepage, https://github.com/
 SIGTechnologies/sigtech-python Keywords: SIGTECH,FINANCE,TRADING,BACKTEST,QUANT
 Classifier: Development Status :: 5 - Production/Stable Classifier: Operating
 System :: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Financial and Insurance Industry Classifier: Programming Language :: Python
@@ -21,18 +21,16 @@
 Requires-Dist: python-semantic-release<=7.34.6; extra == "tools" Requires-Dist:
 types-requests; extra == "tools" Requires-Dist: types-jinja2; extra == "tools"
 Provides-Extra: test Requires-Dist: jupyter; extra == "test" Requires-Dist:
 matplotlib; extra == "test" Requires-Dist: pytest; extra == "test" Requires-
 Dist: statsmodels; extra == "test" ![SigTech SDK Banner](https://sigtech.com/
 wp-content/uploads/2023/08/Python-SDK_github_856x268-1.png "SigTech SDK
 Banner")  
-        _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_H_A_T_-_D_I_S_C_O_R_D_-_b_l_u_e_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
- _b_a_d_g_e_&_l_o_g_o_=_d_i_s_c_o_r_d_&_l_a_b_e_l_C_o_l_o_r_=_r_g_b_(_5_5_,_5_5_,_5_5_)_&_c_o_l_o_r_=_b_l_u_e_v_i_o_l_e_t_]_[_D_o_c_s_]_[_h_t_t_p_s_:_/_/
- _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_f_o_l_l_o_w_-_%_4_0_s_i_g_t_e_c_h_l_t_d_-_1_D_A_1_F_2_?_l_o_g_o_=_t_w_i_t_t_e_r_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-
-                                    _b_a_d_g_e_]
+           _[_D_o_c_s_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_f_o_l_l_o_w_-_%_4_0_s_i_g_t_e_c_h___a_i_-
+                   _1_D_A_1_F_2_?_l_o_g_o_=_t_w_i_t_t_e_r_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
    [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
   shield]][forks-url] ![Stargazers][stars-shield] [![Issues][issues-shield]]
           [issues-url] [![MIT License][license-shield]][license-url]
 [contributors-shield]: https://img.shields.io/github/contributors/
 SIGTechnologies/sigtech-python.svg?style=for-the-badge [contributors-url]:
 https://github.com/SIGTechnologies/sigtech-python/graphs/contributors [forks-
 shield]: https://img.shields.io/github/forks/SIGTechnologies/sigtech-
@@ -47,66 +45,61 @@
 SigTech Python SDK The SigTech Python SDK is designed to simplify the usage of
 the SigTech API for backtesting investment strategies by providing a higher-
 level, object-oriented method of interfacing with our API. With this SDK, you
 can easily test and view the performance of historical strategies. #### Key
 Features - Provides a higher-level object-based interface for convenient
 interaction with the SigTech API. - Simplifies the creation of advanced trading
 strategies by providing methods which simulate rolling future strategies,
-basket strategies, and more. - Interfaces with SigTech's collection of
-historical performance data facilitating accurate backtesting. Explore the
-[SigTech API data catalog](https://sigtechapi.streamlit.app/) to see the
-library of instruments available. ## Installation ```sh pip install sigtech ```
-### Requirements - Python 3.6+ ## Getting started with SigTech Python SDK ###
-Authentication 1. [Sign-up](https://dashboard.sigtech.com/register) for our
-API. 1. Generate an API key using our [dashboard](https://
+basket strategies, and more. - Interfaces with SigTech's historical market data
+facilitating accurate backtesting. Explore the [SigTech API data catalog]
+(https://github.com/SIGTechnologies/sigtech-python/blob/master/docs/data.md) to
+see the list of instruments available. ## Installation ```sh pip install
+sigtech ``` ### Requirements - Python 3.6+ ## Getting started ###
+Authentication 1. Generate an API key using our [dashboard](https://
 dashboard.sigtech.com/api-keys). 1. Secure your API key and save it as a global
-environment variable by following our instructions [here](https://
-learn.sigtech.com/docs/auth). ### Creating your first strategy Our SDK provides
-convenient wrappers for boilerplate functions that are required to interact
-with our API. Copy the following code into your IDE and run it to quickly
-create, backtest, and view the performance of a custom rolling futures
-strategy. >**Note!**\ >The example below will only work if you have saved your
-API key as the global environment variable `SIGTECH_API_KEY`. ```python #
-Import the SigTech API import sigtech.api as sig # Initialize your session
-sig.init() # Create a Rolling Future Strategy es_future =
-sig.RollingFutureStrategy( currency="USD", start_date="2020-01-04",
+environment variable by following our instructions [here](https://github.com/
+SIGTechnologies/sigtech-python/blob/master/docs/auth.md). ### Creating your
+first strategy Our SDK provides convenient wrappers for boilerplate functions
+that are required to interact with our API. Copy the following code into your
+IDE and run it to quickly create, backtest, and view the performance of a
+custom rolling futures strategy. >**Note!**\ >The example below will only work
+if you have saved your API key as the global environment variable
+`SIGTECH_API_KEY`. ```python # Import the SigTech API import sigtech.api as sig
+# Initialize your session sig.init() # Create a Rolling Future Strategy
+es_future = sig.RollingFutureStrategy( currency="USD", start_date="2020-01-04",
 contract_code="ES", contract_sector="INDEX", rolling_rule="front",
 front_offset="-6,-5", ) # Retrieve the strategy history print(es_future.history
-()) ``` ## Next steps 1. Learn more about the API with the [reference guide]
-(https://learn.sigtech.com/reference). 1. Follow some of our [examples](https:/
-/github.com/SIGTechnologies/sigtech-python/tree/master/examples) to see how you
-can replicate and backtest more complex, real-world trading strategies. ##
-Google Colab We understand that getting started with backtesting and evaluating
-trading strategies can be a daunting task, especially for users new to
-financial data analysis and Python development. To make the process as seamless
-as possible, we've prepared a collection of real-world [examples](https://
-github.com/SIGTechnologies/sigtech-python/tree/master/examples) in Jupyter
-Notebook format (.ipynb). All you need to follow along is a SigTech API key. ##
-Logging Logs down to the `debug` log level are available for all API requests.
-They can be accessed using the Python `logging` library. ```python import
-logging logging.basicConfig(level=logging.DEBUG) ``` For more information,
-please refer to the `logging` library's [documentation](https://
-docs.python.org/3/library/logging.html). See [Logging in Python](https://
-realpython.com/python-logging/) for a useful summary of the `logging` library's
-capabilities. ## API Documentation For detailed information about the SigTech
-API, please refer to our official [API user guide](https://learn.sigtech.com/
-docs) and our interactive [API reference guide](https://learn.sigtech.com/
-reference). ## Contributing to the SigTech Python SDK We appreciate and
+()) ``` ## Next steps 1. Follow some of our [examples](https://github.com/
+SIGTechnologies/sigtech-python/tree/master/examples) to see how you can
+replicate and backtest more complex, real-world trading strategies. 1. Explore
+the full range of available instruments in the [API data catalog](https://
+github.com/SIGTechnologies/sigtech-python/blob/master/docs/data.md). 1. Explore
+the full range of endpoints in the [API reference](https://api.sigtech.com/
+docs). ## Google Colab We understand that getting started with backtesting and
+evaluating trading strategies can be a daunting task, especially for users new
+to financial data analysis and Python development. To make the process as
+seamless as possible, we've prepared a collection of real-world [examples]
+(https://github.com/SIGTechnologies/sigtech-python/tree/master/examples) in
+Jupyter Notebook format (`.ipynb`). All you need to follow along is a SigTech
+API key. ## Logging Logs down to the `debug` log level are available for all
+API requests. They can be accessed using the Python `logging` library.
+```python import logging logging.basicConfig(level=logging.DEBUG) ``` For more
+information, please refer to the `logging` library's [documentation](https://
+docs.python.org/3/library/logging.html). ## Contributing We appreciate and
 encourage your contributions to the SigTech Python SDK! If you are enjoying the
 SDK, please show your support by starring this repository and sharing it on
 social media channels. To contribute an example, provide feedback, report a bug
 or otherwise bring an issue to our attention regarding this project, please
 follow the steps outlined in the [Contribution guidelines](https://github.com/
 SIGTechnologies/sigtech-python/blob/master/CONTRIBUTING.md). Please remember
 that all contributors are expected to behave appropriately and abide by our
 [Code of conduct](https://github.com/SIGTechnologies/sigtech-python/blob/
-master/CODE_OF_CONDUCT.md). ## Reporting security issues If you believe you
-have discovered a security vulnerability in our repository please report it to
-us immediately following the instructions [here](https://github.com/
-SIGTechnologies/sigtech-python/blob/master/SECURITY.md). >Attention!\ >Please
-follow the instructions detailed. **Do not** publicly disclose the
-vulnerability in a Github Issue or on a public forum such as Discord or
-Twitter. ## Support If you encounter any issues or have any questions regarding
-our API or SDK, you can reach out to us via our [Discord](https://discord.gg/
-ZcFeutSrWM) or [Twitter](https://twitter.com/sigtechltd/). ## License The
-SigTech Python SDK is released under the [MIT License](https://github.com/
+master/CODE_OF_CONDUCT.md). ## Security issues If you believe you have
+discovered a security vulnerability in our repository please report it to us
+immediately following the instructions [here](https://github.com/
+SIGTechnologies/sigtech-python/blob/master/SECURITY.md). >**Attention!**\ >Do
+not publicly disclose the vulnerability in a Github Issue or on a public forum
+such as X/Twitter. ## Support If you encounter any issues or have any questions
+regarding our API or SDK, you can reach out to us via email at
+[support@sigtech.com](mailto:support@sigtech.com). ## License The SigTech
+Python SDK is released under the [MIT License](https://github.com/
 SIGTechnologies/sigtech-python/blob/master/LICENSE).
```

### Comparing `sigtech-0.5.1/README.md` & `sigtech-0.6.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 ![SigTech SDK Banner](https://sigtech.com/wp-content/uploads/2023/08/Python-SDK_github_856x268-1.png "SigTech SDK Banner")
 
 &nbsp;
 
 <p align="center" id="dummy">
-    <a href="https://discord.gg/ZcFeutSrWM">
-        <img src="https://img.shields.io/badge/CHAT-DISCORD-blue?style=for-the-badge&logo=discord&labelColor=rgb(55,55,55)&color=blueviolet">
+    <a href="https://api.sigtech.com/docs">
+        <img src="https://img.shields.io/badge/Docs-API_REFERENCE-1338be?&style=for-the-badge&logo=wiki&link=https://api.sigtech.com/docs" alt="Docs" />
     </a>
-    <a href="https://learn.sigtech.com/reference/">
-        <img src="https://img.shields.io/badge/Docs-API_REFERENCE-1338be?&style=for-the-badge&logo=wiki&link=https://learn.sigtech.com/reference" alt="Docs" />
+     <a href="https://twitter.com/sigtech_ai/">
+        <img src="https://img.shields.io/badge/follow-%40sigtech_ai-1DA1F2?logo=twitter&style=for-the-badge" />
     </a>
-     <a href="https://twitter.com/sigtechltd/">
-        <img src="https://img.shields.io/badge/follow-%40sigtechltd-1DA1F2?logo=twitter&style=for-the-badge" />
-    </a>
-<p>
+</p>
 
 <div align="center">
 
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 ![Stargazers][stars-shield]
 [![Issues][issues-shield]][issues-url]
@@ -38,33 +35,32 @@
 
 The SigTech Python SDK is designed to simplify the usage of the SigTech API for backtesting investment strategies by providing a higher-level, object-oriented method of interfacing with our API. With this SDK, you can easily test and view the performance of historical strategies.
 
 #### Key Features
 
 - Provides a higher-level object-based interface for convenient interaction with the SigTech API.
 - Simplifies the creation of advanced trading strategies by providing methods which simulate rolling future strategies, basket strategies, and more.
-- Interfaces with SigTech's collection of historical performance data facilitating accurate backtesting. Explore the [SigTech API data catalog](https://sigtechapi.streamlit.app/) to see the library of instruments available.
+- Interfaces with SigTech's historical market data facilitating accurate backtesting. Explore the [SigTech API data catalog](https://github.com/SIGTechnologies/sigtech-python/blob/master/docs/data.md) to see the list of instruments available.
 
 ## Installation
 
 ```sh
 pip install sigtech
 ```
 
 ### Requirements
 
 - Python 3.6+
 
-## Getting started with SigTech Python SDK
+## Getting started
 
 ### Authentication
 
-1. [Sign-up](https://dashboard.sigtech.com/register) for our API.
 1. Generate an API key using our [dashboard](https://dashboard.sigtech.com/api-keys).
-1. Secure your API key and save it as a global environment variable by following our instructions [here](https://learn.sigtech.com/docs/auth).
+1. Secure your API key and save it as a global environment variable by following our instructions [here](https://github.com/SIGTechnologies/sigtech-python/blob/master/docs/auth.md).
 
 ### Creating your first strategy
 
 Our SDK provides convenient wrappers for boilerplate functions that are required to interact with our API. Copy the following code into your IDE and run it to quickly create, backtest, and view the performance of a custom rolling futures strategy.
 
 >**Note!**\
 >The example below will only work if you have saved your API key as the global environment variable `SIGTECH_API_KEY`.
@@ -88,51 +84,53 @@
 
 # Retrieve the strategy history
 print(es_future.history())
 ```
 
 ## Next steps
 
-1. Learn more about the API with the [reference guide](https://learn.sigtech.com/reference). 
 1. Follow some of our [examples](https://github.com/SIGTechnologies/sigtech-python/tree/master/examples) to see how you can replicate and backtest more complex, real-world trading strategies.
+1. Explore the full range of available instruments in the [API data catalog](https://github.com/SIGTechnologies/sigtech-python/blob/master/docs/data.md).
+1. Explore the full range of endpoints in the [API reference](https://api.sigtech.com/docs). 
+
+
+
 
 ## Google Colab
 
-We understand that getting started with backtesting and evaluating trading strategies can be a daunting task, especially for users new to financial data analysis and Python development. To make the process as seamless as possible, we've prepared a collection of real-world [examples](https://github.com/SIGTechnologies/sigtech-python/tree/master/examples) in Jupyter Notebook format (.ipynb). All you need to follow along is a SigTech API key.
+We understand that getting started with backtesting and evaluating trading strategies can be a daunting task, especially for users new to financial data analysis and Python development. To make the process as seamless as possible, we've prepared a collection of real-world [examples](https://github.com/SIGTechnologies/sigtech-python/tree/master/examples) in Jupyter Notebook format (`.ipynb`). All you need to follow along is a SigTech API key.
 
 ## Logging
 
 Logs down to the `debug` log level are available for all API requests. They can be accessed using the Python `logging` library.
 
 ```python
 import logging
 logging.basicConfig(level=logging.DEBUG)
 ```
 
-For more information, please refer to the `logging` library's [documentation](https://docs.python.org/3/library/logging.html). See [Logging in Python](https://realpython.com/python-logging/) for a useful summary of the `logging` library's capabilities.
-
-## API Documentation
+For more information, please refer to the `logging` library's [documentation](https://docs.python.org/3/library/logging.html).
 
-For detailed information about the SigTech API, please refer to our official [API user guide](https://learn.sigtech.com/docs) and our interactive [API reference guide](https://learn.sigtech.com/reference).
 
-## Contributing to the SigTech Python SDK
+## Contributing
 
 We appreciate and encourage your contributions to the SigTech Python SDK! If you are enjoying the SDK, please show your support by starring this repository and sharing it on social media channels.
 
 To contribute an example, provide feedback, report a bug or otherwise bring an issue to our attention regarding this project, please follow the steps outlined in the [Contribution guidelines](https://github.com/SIGTechnologies/sigtech-python/blob/master/CONTRIBUTING.md).
 
 Please remember that all contributors are expected to behave appropriately and abide by our [Code of conduct](https://github.com/SIGTechnologies/sigtech-python/blob/master/CODE_OF_CONDUCT.md).
 
-## Reporting security issues
+## Security issues
 
 If you believe you have discovered a security vulnerability in our repository please report it to us immediately following the instructions [here](https://github.com/SIGTechnologies/sigtech-python/blob/master/SECURITY.md).
 
->Attention!\
->Please follow the instructions detailed. **Do not** publicly disclose the vulnerability in a Github Issue or on a public forum such as Discord or Twitter.
+>**Attention!**\
+>Do not publicly disclose the vulnerability in a Github Issue or on a public forum such as X/Twitter.
 
 ## Support
 
-If you encounter any issues or have any questions regarding our API or SDK, you can reach out to us via our [Discord](https://discord.gg/ZcFeutSrWM) or [Twitter](https://twitter.com/sigtechltd/).
+If you encounter any issues or have any questions regarding our API or SDK, 
+you can reach out to us via email at [support@sigtech.com](mailto:support@sigtech.com).
 
 ## License
 
 The SigTech Python SDK is released under the [MIT License](https://github.com/SIGTechnologies/sigtech-python/blob/master/LICENSE).
```

#### html2text {}

```diff
@@ -1,13 +1,11 @@
 ![SigTech SDK Banner](https://sigtech.com/wp-content/uploads/2023/08/Python-
 SDK_github_856x268-1.png "SigTech SDK Banner")  
-        _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_H_A_T_-_D_I_S_C_O_R_D_-_b_l_u_e_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
- _b_a_d_g_e_&_l_o_g_o_=_d_i_s_c_o_r_d_&_l_a_b_e_l_C_o_l_o_r_=_r_g_b_(_5_5_,_5_5_,_5_5_)_&_c_o_l_o_r_=_b_l_u_e_v_i_o_l_e_t_]_[_D_o_c_s_]_[_h_t_t_p_s_:_/_/
- _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_f_o_l_l_o_w_-_%_4_0_s_i_g_t_e_c_h_l_t_d_-_1_D_A_1_F_2_?_l_o_g_o_=_t_w_i_t_t_e_r_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-
-                                    _b_a_d_g_e_]
+           _[_D_o_c_s_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_f_o_l_l_o_w_-_%_4_0_s_i_g_t_e_c_h___a_i_-
+                   _1_D_A_1_F_2_?_l_o_g_o_=_t_w_i_t_t_e_r_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
    [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
   shield]][forks-url] ![Stargazers][stars-shield] [![Issues][issues-shield]]
           [issues-url] [![MIT License][license-shield]][license-url]
 [contributors-shield]: https://img.shields.io/github/contributors/
 SIGTechnologies/sigtech-python.svg?style=for-the-badge [contributors-url]:
 https://github.com/SIGTechnologies/sigtech-python/graphs/contributors [forks-
 shield]: https://img.shields.io/github/forks/SIGTechnologies/sigtech-
@@ -22,66 +20,61 @@
 SigTech Python SDK The SigTech Python SDK is designed to simplify the usage of
 the SigTech API for backtesting investment strategies by providing a higher-
 level, object-oriented method of interfacing with our API. With this SDK, you
 can easily test and view the performance of historical strategies. #### Key
 Features - Provides a higher-level object-based interface for convenient
 interaction with the SigTech API. - Simplifies the creation of advanced trading
 strategies by providing methods which simulate rolling future strategies,
-basket strategies, and more. - Interfaces with SigTech's collection of
-historical performance data facilitating accurate backtesting. Explore the
-[SigTech API data catalog](https://sigtechapi.streamlit.app/) to see the
-library of instruments available. ## Installation ```sh pip install sigtech ```
-### Requirements - Python 3.6+ ## Getting started with SigTech Python SDK ###
-Authentication 1. [Sign-up](https://dashboard.sigtech.com/register) for our
-API. 1. Generate an API key using our [dashboard](https://
+basket strategies, and more. - Interfaces with SigTech's historical market data
+facilitating accurate backtesting. Explore the [SigTech API data catalog]
+(https://github.com/SIGTechnologies/sigtech-python/blob/master/docs/data.md) to
+see the list of instruments available. ## Installation ```sh pip install
+sigtech ``` ### Requirements - Python 3.6+ ## Getting started ###
+Authentication 1. Generate an API key using our [dashboard](https://
 dashboard.sigtech.com/api-keys). 1. Secure your API key and save it as a global
-environment variable by following our instructions [here](https://
-learn.sigtech.com/docs/auth). ### Creating your first strategy Our SDK provides
-convenient wrappers for boilerplate functions that are required to interact
-with our API. Copy the following code into your IDE and run it to quickly
-create, backtest, and view the performance of a custom rolling futures
-strategy. >**Note!**\ >The example below will only work if you have saved your
-API key as the global environment variable `SIGTECH_API_KEY`. ```python #
-Import the SigTech API import sigtech.api as sig # Initialize your session
-sig.init() # Create a Rolling Future Strategy es_future =
-sig.RollingFutureStrategy( currency="USD", start_date="2020-01-04",
+environment variable by following our instructions [here](https://github.com/
+SIGTechnologies/sigtech-python/blob/master/docs/auth.md). ### Creating your
+first strategy Our SDK provides convenient wrappers for boilerplate functions
+that are required to interact with our API. Copy the following code into your
+IDE and run it to quickly create, backtest, and view the performance of a
+custom rolling futures strategy. >**Note!**\ >The example below will only work
+if you have saved your API key as the global environment variable
+`SIGTECH_API_KEY`. ```python # Import the SigTech API import sigtech.api as sig
+# Initialize your session sig.init() # Create a Rolling Future Strategy
+es_future = sig.RollingFutureStrategy( currency="USD", start_date="2020-01-04",
 contract_code="ES", contract_sector="INDEX", rolling_rule="front",
 front_offset="-6,-5", ) # Retrieve the strategy history print(es_future.history
-()) ``` ## Next steps 1. Learn more about the API with the [reference guide]
-(https://learn.sigtech.com/reference). 1. Follow some of our [examples](https:/
-/github.com/SIGTechnologies/sigtech-python/tree/master/examples) to see how you
-can replicate and backtest more complex, real-world trading strategies. ##
-Google Colab We understand that getting started with backtesting and evaluating
-trading strategies can be a daunting task, especially for users new to
-financial data analysis and Python development. To make the process as seamless
-as possible, we've prepared a collection of real-world [examples](https://
-github.com/SIGTechnologies/sigtech-python/tree/master/examples) in Jupyter
-Notebook format (.ipynb). All you need to follow along is a SigTech API key. ##
-Logging Logs down to the `debug` log level are available for all API requests.
-They can be accessed using the Python `logging` library. ```python import
-logging logging.basicConfig(level=logging.DEBUG) ``` For more information,
-please refer to the `logging` library's [documentation](https://
-docs.python.org/3/library/logging.html). See [Logging in Python](https://
-realpython.com/python-logging/) for a useful summary of the `logging` library's
-capabilities. ## API Documentation For detailed information about the SigTech
-API, please refer to our official [API user guide](https://learn.sigtech.com/
-docs) and our interactive [API reference guide](https://learn.sigtech.com/
-reference). ## Contributing to the SigTech Python SDK We appreciate and
+()) ``` ## Next steps 1. Follow some of our [examples](https://github.com/
+SIGTechnologies/sigtech-python/tree/master/examples) to see how you can
+replicate and backtest more complex, real-world trading strategies. 1. Explore
+the full range of available instruments in the [API data catalog](https://
+github.com/SIGTechnologies/sigtech-python/blob/master/docs/data.md). 1. Explore
+the full range of endpoints in the [API reference](https://api.sigtech.com/
+docs). ## Google Colab We understand that getting started with backtesting and
+evaluating trading strategies can be a daunting task, especially for users new
+to financial data analysis and Python development. To make the process as
+seamless as possible, we've prepared a collection of real-world [examples]
+(https://github.com/SIGTechnologies/sigtech-python/tree/master/examples) in
+Jupyter Notebook format (`.ipynb`). All you need to follow along is a SigTech
+API key. ## Logging Logs down to the `debug` log level are available for all
+API requests. They can be accessed using the Python `logging` library.
+```python import logging logging.basicConfig(level=logging.DEBUG) ``` For more
+information, please refer to the `logging` library's [documentation](https://
+docs.python.org/3/library/logging.html). ## Contributing We appreciate and
 encourage your contributions to the SigTech Python SDK! If you are enjoying the
 SDK, please show your support by starring this repository and sharing it on
 social media channels. To contribute an example, provide feedback, report a bug
 or otherwise bring an issue to our attention regarding this project, please
 follow the steps outlined in the [Contribution guidelines](https://github.com/
 SIGTechnologies/sigtech-python/blob/master/CONTRIBUTING.md). Please remember
 that all contributors are expected to behave appropriately and abide by our
 [Code of conduct](https://github.com/SIGTechnologies/sigtech-python/blob/
-master/CODE_OF_CONDUCT.md). ## Reporting security issues If you believe you
-have discovered a security vulnerability in our repository please report it to
-us immediately following the instructions [here](https://github.com/
-SIGTechnologies/sigtech-python/blob/master/SECURITY.md). >Attention!\ >Please
-follow the instructions detailed. **Do not** publicly disclose the
-vulnerability in a Github Issue or on a public forum such as Discord or
-Twitter. ## Support If you encounter any issues or have any questions regarding
-our API or SDK, you can reach out to us via our [Discord](https://discord.gg/
-ZcFeutSrWM) or [Twitter](https://twitter.com/sigtechltd/). ## License The
-SigTech Python SDK is released under the [MIT License](https://github.com/
+master/CODE_OF_CONDUCT.md). ## Security issues If you believe you have
+discovered a security vulnerability in our repository please report it to us
+immediately following the instructions [here](https://github.com/
+SIGTechnologies/sigtech-python/blob/master/SECURITY.md). >**Attention!**\ >Do
+not publicly disclose the vulnerability in a Github Issue or on a public forum
+such as X/Twitter. ## Support If you encounter any issues or have any questions
+regarding our API or SDK, you can reach out to us via email at
+[support@sigtech.com](mailto:support@sigtech.com). ## License The SigTech
+Python SDK is released under the [MIT License](https://github.com/
 SIGTechnologies/sigtech-python/blob/master/LICENSE).
```

### Comparing `sigtech-0.5.1/pyproject.toml` & `sigtech-0.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sigtech"
-version = "0.5.1"
+version = "0.6.1"
 authors = [
   { name="SigTech", email="support@sigtech.com" },
 ]
 description = "SigTech Python SDK"
 readme = {file = "README.md", content-type = "text/markdown"}
 keywords = ["SIGTECH", "FINANCE", "TRADING", "BACKTEST", "QUANT"]
 license = {text= "MIT"}
```

### Comparing `sigtech-0.5.1/sigtech/api/__init__.py` & `sigtech-0.6.1/sigtech/api/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from sigtech.api.framework.instruments.ir_otc import InterestRateSwap
 from sigtech.api.framework.instruments.ois_swap import OISSwap
 from sigtech.api.framework.strategies.basket_strategy import BasketStrategy
 from sigtech.api.framework.strategies.reinvestment_strategy import (
     ReinvestmentStrategy,
     get_single_stock_strategy,
 )
+from sigtech.api.framework.strategies.rolling_bond_strategy import (
+    RollingBondStrategy,
+    SingleBondStrategy,
+)
 from sigtech.api.framework.strategies.rolling_future_strategy import (
     RollingFutureStrategy,
 )
 from sigtech.api.framework.strategies.rolling_fx_forward_strategy import (
     RollingFXForwardStrategy,
 )
 from sigtech.api.framework.strategies.rolling_swap_strategy import RollingSwapStrategy
@@ -23,14 +27,16 @@
     "Client",
     "SignalStrategy",
     "BasketStrategy",
     "ReinvestmentStrategy",
     "RollingFutureStrategy",
     "RollingFXForwardStrategy",
     "RollingSwapStrategy",
+    "SingleBondStrategy",
+    "RollingBondStrategy",
     "TradableTSIndex",
     "OISSwap",
     "InterestRateSwap",
     "FXForward",
     "env",
     "get_single_stock_strategy",
     "init",
```

### Comparing `sigtech-0.5.1/sigtech/api/client/client.py` & `sigtech-0.6.1/sigtech/api/client/client.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.5.1/sigtech/api/client/response.py` & `sigtech-0.6.1/sigtech/api/client/response.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.5.1/sigtech/api/client/utils.py` & `sigtech-0.6.1/sigtech/api/client/utils.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.5.1/sigtech/api/datasets/__init__.py` & `sigtech-0.6.1/sigtech/api/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.5.1/sigtech/api/datasets/__main__.py` & `sigtech-0.6.1/sigtech/api/datasets/__main__.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.5.1/sigtech/api/datasets/delete.py` & `sigtech-0.6.1/sigtech/api/datasets/delete.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.5.1/sigtech/api/datasets/upload.py` & `sigtech-0.6.1/sigtech/api/datasets/upload.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.5.1/sigtech/api/framework/environment.py` & `sigtech-0.6.1/sigtech/api/framework/environment.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.5.1/sigtech/api/framework/framework_api_object.py` & `sigtech-0.6.1/sigtech/api/framework/framework_api_object.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.5.1/sigtech/api/framework/indices/tradable_index.py` & `sigtech-0.6.1/sigtech/api/framework/indices/tradable_index.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.5.1/sigtech/api/framework/instruments/futures.py` & `sigtech-0.6.1/sigtech/api/framework/instruments/futures.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.5.1/sigtech/api/framework/instruments/fx_otc.py` & `sigtech-0.6.1/sigtech/api/framework/instruments/fx_otc.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.5.1/sigtech/api/framework/instruments/ir_otc.py` & `sigtech-0.6.1/sigtech/api/framework/instruments/ir_otc.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.5.1/sigtech/api/framework/instruments/ois_swap.py` & `sigtech-0.6.1/sigtech/api/framework/instruments/ois_swap.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.5.1/sigtech/api/framework/plot_wrapper.py` & `sigtech-0.6.1/sigtech/api/framework/plot_wrapper.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.5.1/sigtech/api/framework/strategies/basket_strategy.py` & `sigtech-0.6.1/sigtech/api/framework/strategies/basket_strategy.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.5.1/sigtech/api/framework/strategies/reinvestment_strategy.py` & `sigtech-0.6.1/sigtech/api/framework/strategies/reinvestment_strategy.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.5.1/sigtech/api/framework/strategies/rolling_future_strategy.py` & `sigtech-0.6.1/sigtech/api/framework/strategies/rolling_future_strategy.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.5.1/sigtech/api/framework/strategies/rolling_fx_forward_strategy.py` & `sigtech-0.6.1/sigtech/api/framework/strategies/rolling_fx_forward_strategy.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.5.1/sigtech/api/framework/strategies/rolling_swap_strategy.py` & `sigtech-0.6.1/sigtech/api/framework/strategies/rolling_swap_strategy.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.5.1/sigtech/api/framework/strategies/signal_strategy.py` & `sigtech-0.6.1/sigtech/api/framework/strategies/signal_strategy.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.5.1/sigtech/api/framework/strategies/strategy.py` & `sigtech-0.6.1/sigtech/api/framework/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `sigtech-0.5.1/sigtech/api/jobs/__init__.py` & `sigtech-0.6.1/sigtech/api/jobs/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime as dtm
 import io
 import json
 import logging
 import os
 from collections import defaultdict
+from functools import lru_cache
 
 import pandas as pd
 import requests
 
 logger = logging.getLogger("jobs")
 
 
@@ -58,14 +59,18 @@
     pass
 
 
 class OutputDoesNotExist(Exception):
     pass
 
 
+class OutputFormatDoesNotExist(Exception):
+    pass
+
+
 class ApiObject:
     def __init__(self, obj, session, url):
         self._obj = obj
         self.session = session
         self.url = url
 
     def __repr__(self):
@@ -225,106 +230,90 @@
 
     @property
     def obj(self):
         if self._obj is not None:
             return self._obj
 
         self._obj = [
-            Output(o, self.session, f"{self.url}/{o['artifact_id']}")
+            Output(o, self.session, f"{self.url}/{o['artifact_name']}")
             for o in super().obj
         ]
         return self._obj
 
     def __getitem__(self, item):
         if isinstance(item, int):
             return self.obj[item]
         resp = self.session.get(f"{self.url}/{item}/info")
         if resp.status_code == 200:
             return Output(resp.json(), self.session, f"{self.url}/{item}")
         assert resp.status_code == 404
-        try:
-            obj = get_list_by_keys(self.obj, ["id", "sha", "name"], item)
-        except KeyError:
-            raise OutputDoesNotExist(item)
-        return obj
+        raise OutputDoesNotExist(item)
 
     def get(self, output_id):
         return self[output_id]
 
 
 class Output(ApiObject):
 
     def __init__(self, obj, session, url):
         super().__init__(obj, session, url)
-        self._content = None
-
-    @property
-    def id(self):
-        return self.obj["artifact_id"]
 
     @property
     def name(self):
         return self.obj["artifact_name"]
 
     @property
-    def sha(self):
-        return self.obj["sha"]
-
-    @property
     def created_at(self):
         return epoch_to_datetime(self.obj["ts_epoch"])
 
-    @property
-    def content(self):
-        if self._content is not None:
-            return self._content
-        resp = self.session.get(self.url)
-        resp.raise_for_status()
-        self._content = resp.content
-        return self._content
-
     def dict(self):
         return {
             "name": self.name,
-            "id": self.id,
-            "sha": self.sha,
             "created_at": self.created_at,
         }
 
     def __repr__(self):
         items = (f"{k}={repr(v)}" for k, v in self.dict().items())
         return f"{type(self).__name__}({', '.join(items)})"
 
+    def _get_format_url(self, format):
+        assert self.url.endswith(self.name)
+        url = self.url.removesuffix(self.name)
+        return f"{url}_artifacts.{self.name}.{format}"
+
+    @lru_cache()
     def json(self):
-        if self.id.endswith(".gzip+json"):
-            return json.loads(self.content)
-        elif self.id.endswith(".parquet-snappy"):
-            import pyarrow.parquet  # type: ignore
-
-            t = pyarrow.parquet.read_table(
-                io.BytesIO(self.content),
-                use_pandas_metadata=False,
+        url = self._get_format_url("gzip+json")
+        resp = self.session.get(url)
+        if resp.status_code == 404:
+            raise OutputFormatDoesNotExist(
+                f"json format not available for output: {self.name}"
             )
-            return t.to_pydict()
-        raise NotImplementedError("unknown artifact format")
+        resp.raise_for_status()
+        return json.loads(resp.content)
 
+    @lru_cache()
     def df(self):
-        content = self.content
-        if self.id.endswith(".gzip+json"):
-            return pd.DataFrame(json.loads(content))
-        elif self.id.endswith(".parquet-snappy"):
-            try:
-                return pd.read_parquet(io.BytesIO(content))
-            except Exception as e:
-                logger.error(
-                    f"Error during pandas.read_parquet(): {e}. "
-                    f"Using pyarrow.parquet.read_table() instead."
-                )
-            import pyarrow.parquet
-
-            t = pyarrow.parquet.read_table(
-                io.BytesIO(content),
-                use_pandas_metadata=False,
+        url = self._get_format_url("parquet-snappy")
+        resp = self.session.get(url)
+        if resp.status_code == 404:
+            raise OutputFormatDoesNotExist(
+                f"parquet format not available for output: {self.name}"
             )
-            return pd.DataFrame(t.to_pydict())
-        else:
-            raise NotImplementedError("unknown artifact format")
+        resp.raise_for_status()
+        content = resp.content
+        f = io.BytesIO(content)
+
+        f.seek(0)
+        try:
+            return pd.read_parquet(f)
+        except Exception as e:
+            logger.error(
+                f"Error during pandas.read_parquet(): {e}. "
+                f"Using pyarrow.parquet.read_table() instead."
+            )
+
+        import pyarrow.parquet  # type: ignore
+
+        f.seek(0)
+        t = pyarrow.parquet.read_table(f, use_pandas_metadata=False)
+        return pd.DataFrame(t.to_pydict())
```

### Comparing `sigtech-0.5.1/sigtech.egg-info/PKG-INFO` & `sigtech-0.6.1/sigtech.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigtech
-Version: 0.5.1
+Version: 0.6.1
 Summary: SigTech Python SDK
 Author-email: SigTech <support@sigtech.com>
 License: MIT
 Project-URL: Homepage, https://github.com/SIGTechnologies/sigtech-python
 Keywords: SIGTECH,FINANCE,TRADING,BACKTEST,QUANT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -44,24 +44,21 @@
 Requires-Dist: statsmodels; extra == "test"
 
 ![SigTech SDK Banner](https://sigtech.com/wp-content/uploads/2023/08/Python-SDK_github_856x268-1.png "SigTech SDK Banner")
 
 &nbsp;
 
 <p align="center" id="dummy">
-    <a href="https://discord.gg/ZcFeutSrWM">
-        <img src="https://img.shields.io/badge/CHAT-DISCORD-blue?style=for-the-badge&logo=discord&labelColor=rgb(55,55,55)&color=blueviolet">
+    <a href="https://api.sigtech.com/docs">
+        <img src="https://img.shields.io/badge/Docs-API_REFERENCE-1338be?&style=for-the-badge&logo=wiki&link=https://api.sigtech.com/docs" alt="Docs" />
     </a>
-    <a href="https://learn.sigtech.com/reference/">
-        <img src="https://img.shields.io/badge/Docs-API_REFERENCE-1338be?&style=for-the-badge&logo=wiki&link=https://learn.sigtech.com/reference" alt="Docs" />
+     <a href="https://twitter.com/sigtech_ai/">
+        <img src="https://img.shields.io/badge/follow-%40sigtech_ai-1DA1F2?logo=twitter&style=for-the-badge" />
     </a>
-     <a href="https://twitter.com/sigtechltd/">
-        <img src="https://img.shields.io/badge/follow-%40sigtechltd-1DA1F2?logo=twitter&style=for-the-badge" />
-    </a>
-<p>
+</p>
 
 <div align="center">
 
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 ![Stargazers][stars-shield]
 [![Issues][issues-shield]][issues-url]
@@ -83,33 +80,32 @@
 
 The SigTech Python SDK is designed to simplify the usage of the SigTech API for backtesting investment strategies by providing a higher-level, object-oriented method of interfacing with our API. With this SDK, you can easily test and view the performance of historical strategies.
 
 #### Key Features
 
 - Provides a higher-level object-based interface for convenient interaction with the SigTech API.
 - Simplifies the creation of advanced trading strategies by providing methods which simulate rolling future strategies, basket strategies, and more.
-- Interfaces with SigTech's collection of historical performance data facilitating accurate backtesting. Explore the [SigTech API data catalog](https://sigtechapi.streamlit.app/) to see the library of instruments available.
+- Interfaces with SigTech's historical market data facilitating accurate backtesting. Explore the [SigTech API data catalog](https://github.com/SIGTechnologies/sigtech-python/blob/master/docs/data.md) to see the list of instruments available.
 
 ## Installation
 
 ```sh
 pip install sigtech
 ```
 
 ### Requirements
 
 - Python 3.6+
 
-## Getting started with SigTech Python SDK
+## Getting started
 
 ### Authentication
 
-1. [Sign-up](https://dashboard.sigtech.com/register) for our API.
 1. Generate an API key using our [dashboard](https://dashboard.sigtech.com/api-keys).
-1. Secure your API key and save it as a global environment variable by following our instructions [here](https://learn.sigtech.com/docs/auth).
+1. Secure your API key and save it as a global environment variable by following our instructions [here](https://github.com/SIGTechnologies/sigtech-python/blob/master/docs/auth.md).
 
 ### Creating your first strategy
 
 Our SDK provides convenient wrappers for boilerplate functions that are required to interact with our API. Copy the following code into your IDE and run it to quickly create, backtest, and view the performance of a custom rolling futures strategy.
 
 >**Note!**\
 >The example below will only work if you have saved your API key as the global environment variable `SIGTECH_API_KEY`.
@@ -133,51 +129,53 @@
 
 # Retrieve the strategy history
 print(es_future.history())
 ```
 
 ## Next steps
 
-1. Learn more about the API with the [reference guide](https://learn.sigtech.com/reference). 
 1. Follow some of our [examples](https://github.com/SIGTechnologies/sigtech-python/tree/master/examples) to see how you can replicate and backtest more complex, real-world trading strategies.
+1. Explore the full range of available instruments in the [API data catalog](https://github.com/SIGTechnologies/sigtech-python/blob/master/docs/data.md).
+1. Explore the full range of endpoints in the [API reference](https://api.sigtech.com/docs). 
+
+
+
 
 ## Google Colab
 
-We understand that getting started with backtesting and evaluating trading strategies can be a daunting task, especially for users new to financial data analysis and Python development. To make the process as seamless as possible, we've prepared a collection of real-world [examples](https://github.com/SIGTechnologies/sigtech-python/tree/master/examples) in Jupyter Notebook format (.ipynb). All you need to follow along is a SigTech API key.
+We understand that getting started with backtesting and evaluating trading strategies can be a daunting task, especially for users new to financial data analysis and Python development. To make the process as seamless as possible, we've prepared a collection of real-world [examples](https://github.com/SIGTechnologies/sigtech-python/tree/master/examples) in Jupyter Notebook format (`.ipynb`). All you need to follow along is a SigTech API key.
 
 ## Logging
 
 Logs down to the `debug` log level are available for all API requests. They can be accessed using the Python `logging` library.
 
 ```python
 import logging
 logging.basicConfig(level=logging.DEBUG)
 ```
 
-For more information, please refer to the `logging` library's [documentation](https://docs.python.org/3/library/logging.html). See [Logging in Python](https://realpython.com/python-logging/) for a useful summary of the `logging` library's capabilities.
-
-## API Documentation
+For more information, please refer to the `logging` library's [documentation](https://docs.python.org/3/library/logging.html).
 
-For detailed information about the SigTech API, please refer to our official [API user guide](https://learn.sigtech.com/docs) and our interactive [API reference guide](https://learn.sigtech.com/reference).
 
-## Contributing to the SigTech Python SDK
+## Contributing
 
 We appreciate and encourage your contributions to the SigTech Python SDK! If you are enjoying the SDK, please show your support by starring this repository and sharing it on social media channels.
 
 To contribute an example, provide feedback, report a bug or otherwise bring an issue to our attention regarding this project, please follow the steps outlined in the [Contribution guidelines](https://github.com/SIGTechnologies/sigtech-python/blob/master/CONTRIBUTING.md).
 
 Please remember that all contributors are expected to behave appropriately and abide by our [Code of conduct](https://github.com/SIGTechnologies/sigtech-python/blob/master/CODE_OF_CONDUCT.md).
 
-## Reporting security issues
+## Security issues
 
 If you believe you have discovered a security vulnerability in our repository please report it to us immediately following the instructions [here](https://github.com/SIGTechnologies/sigtech-python/blob/master/SECURITY.md).
 
->Attention!\
->Please follow the instructions detailed. **Do not** publicly disclose the vulnerability in a Github Issue or on a public forum such as Discord or Twitter.
+>**Attention!**\
+>Do not publicly disclose the vulnerability in a Github Issue or on a public forum such as X/Twitter.
 
 ## Support
 
-If you encounter any issues or have any questions regarding our API or SDK, you can reach out to us via our [Discord](https://discord.gg/ZcFeutSrWM) or [Twitter](https://twitter.com/sigtechltd/).
+If you encounter any issues or have any questions regarding our API or SDK, 
+you can reach out to us via email at [support@sigtech.com](mailto:support@sigtech.com).
 
 ## License
 
 The SigTech Python SDK is released under the [MIT License](https://github.com/SIGTechnologies/sigtech-python/blob/master/LICENSE).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sigtech Version: 0.5.1 Summary: SigTech Python SDK
+Metadata-Version: 2.1 Name: sigtech Version: 0.6.1 Summary: SigTech Python SDK
 Author-email: SigTech
 sigtech.com> License: MIT Project-URL: Homepage, https://github.com/
 SIGTechnologies/sigtech-python Keywords: SIGTECH,FINANCE,TRADING,BACKTEST,QUANT
 Classifier: Development Status :: 5 - Production/Stable Classifier: Operating
 System :: OS Independent Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Financial and Insurance Industry Classifier: Programming Language :: Python
@@ -21,18 +21,16 @@
 Requires-Dist: python-semantic-release<=7.34.6; extra == "tools" Requires-Dist:
 types-requests; extra == "tools" Requires-Dist: types-jinja2; extra == "tools"
 Provides-Extra: test Requires-Dist: jupyter; extra == "test" Requires-Dist:
 matplotlib; extra == "test" Requires-Dist: pytest; extra == "test" Requires-
 Dist: statsmodels; extra == "test" ![SigTech SDK Banner](https://sigtech.com/
 wp-content/uploads/2023/08/Python-SDK_github_856x268-1.png "SigTech SDK
 Banner")  
-        _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_H_A_T_-_D_I_S_C_O_R_D_-_b_l_u_e_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
- _b_a_d_g_e_&_l_o_g_o_=_d_i_s_c_o_r_d_&_l_a_b_e_l_C_o_l_o_r_=_r_g_b_(_5_5_,_5_5_,_5_5_)_&_c_o_l_o_r_=_b_l_u_e_v_i_o_l_e_t_]_[_D_o_c_s_]_[_h_t_t_p_s_:_/_/
- _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_f_o_l_l_o_w_-_%_4_0_s_i_g_t_e_c_h_l_t_d_-_1_D_A_1_F_2_?_l_o_g_o_=_t_w_i_t_t_e_r_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-
-                                    _b_a_d_g_e_]
+           _[_D_o_c_s_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_f_o_l_l_o_w_-_%_4_0_s_i_g_t_e_c_h___a_i_-
+                   _1_D_A_1_F_2_?_l_o_g_o_=_t_w_i_t_t_e_r_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
    [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
   shield]][forks-url] ![Stargazers][stars-shield] [![Issues][issues-shield]]
           [issues-url] [![MIT License][license-shield]][license-url]
 [contributors-shield]: https://img.shields.io/github/contributors/
 SIGTechnologies/sigtech-python.svg?style=for-the-badge [contributors-url]:
 https://github.com/SIGTechnologies/sigtech-python/graphs/contributors [forks-
 shield]: https://img.shields.io/github/forks/SIGTechnologies/sigtech-
@@ -47,66 +45,61 @@
 SigTech Python SDK The SigTech Python SDK is designed to simplify the usage of
 the SigTech API for backtesting investment strategies by providing a higher-
 level, object-oriented method of interfacing with our API. With this SDK, you
 can easily test and view the performance of historical strategies. #### Key
 Features - Provides a higher-level object-based interface for convenient
 interaction with the SigTech API. - Simplifies the creation of advanced trading
 strategies by providing methods which simulate rolling future strategies,
-basket strategies, and more. - Interfaces with SigTech's collection of
-historical performance data facilitating accurate backtesting. Explore the
-[SigTech API data catalog](https://sigtechapi.streamlit.app/) to see the
-library of instruments available. ## Installation ```sh pip install sigtech ```
-### Requirements - Python 3.6+ ## Getting started with SigTech Python SDK ###
-Authentication 1. [Sign-up](https://dashboard.sigtech.com/register) for our
-API. 1. Generate an API key using our [dashboard](https://
+basket strategies, and more. - Interfaces with SigTech's historical market data
+facilitating accurate backtesting. Explore the [SigTech API data catalog]
+(https://github.com/SIGTechnologies/sigtech-python/blob/master/docs/data.md) to
+see the list of instruments available. ## Installation ```sh pip install
+sigtech ``` ### Requirements - Python 3.6+ ## Getting started ###
+Authentication 1. Generate an API key using our [dashboard](https://
 dashboard.sigtech.com/api-keys). 1. Secure your API key and save it as a global
-environment variable by following our instructions [here](https://
-learn.sigtech.com/docs/auth). ### Creating your first strategy Our SDK provides
-convenient wrappers for boilerplate functions that are required to interact
-with our API. Copy the following code into your IDE and run it to quickly
-create, backtest, and view the performance of a custom rolling futures
-strategy. >**Note!**\ >The example below will only work if you have saved your
-API key as the global environment variable `SIGTECH_API_KEY`. ```python #
-Import the SigTech API import sigtech.api as sig # Initialize your session
-sig.init() # Create a Rolling Future Strategy es_future =
-sig.RollingFutureStrategy( currency="USD", start_date="2020-01-04",
+environment variable by following our instructions [here](https://github.com/
+SIGTechnologies/sigtech-python/blob/master/docs/auth.md). ### Creating your
+first strategy Our SDK provides convenient wrappers for boilerplate functions
+that are required to interact with our API. Copy the following code into your
+IDE and run it to quickly create, backtest, and view the performance of a
+custom rolling futures strategy. >**Note!**\ >The example below will only work
+if you have saved your API key as the global environment variable
+`SIGTECH_API_KEY`. ```python # Import the SigTech API import sigtech.api as sig
+# Initialize your session sig.init() # Create a Rolling Future Strategy
+es_future = sig.RollingFutureStrategy( currency="USD", start_date="2020-01-04",
 contract_code="ES", contract_sector="INDEX", rolling_rule="front",
 front_offset="-6,-5", ) # Retrieve the strategy history print(es_future.history
-()) ``` ## Next steps 1. Learn more about the API with the [reference guide]
-(https://learn.sigtech.com/reference). 1. Follow some of our [examples](https:/
-/github.com/SIGTechnologies/sigtech-python/tree/master/examples) to see how you
-can replicate and backtest more complex, real-world trading strategies. ##
-Google Colab We understand that getting started with backtesting and evaluating
-trading strategies can be a daunting task, especially for users new to
-financial data analysis and Python development. To make the process as seamless
-as possible, we've prepared a collection of real-world [examples](https://
-github.com/SIGTechnologies/sigtech-python/tree/master/examples) in Jupyter
-Notebook format (.ipynb). All you need to follow along is a SigTech API key. ##
-Logging Logs down to the `debug` log level are available for all API requests.
-They can be accessed using the Python `logging` library. ```python import
-logging logging.basicConfig(level=logging.DEBUG) ``` For more information,
-please refer to the `logging` library's [documentation](https://
-docs.python.org/3/library/logging.html). See [Logging in Python](https://
-realpython.com/python-logging/) for a useful summary of the `logging` library's
-capabilities. ## API Documentation For detailed information about the SigTech
-API, please refer to our official [API user guide](https://learn.sigtech.com/
-docs) and our interactive [API reference guide](https://learn.sigtech.com/
-reference). ## Contributing to the SigTech Python SDK We appreciate and
+()) ``` ## Next steps 1. Follow some of our [examples](https://github.com/
+SIGTechnologies/sigtech-python/tree/master/examples) to see how you can
+replicate and backtest more complex, real-world trading strategies. 1. Explore
+the full range of available instruments in the [API data catalog](https://
+github.com/SIGTechnologies/sigtech-python/blob/master/docs/data.md). 1. Explore
+the full range of endpoints in the [API reference](https://api.sigtech.com/
+docs). ## Google Colab We understand that getting started with backtesting and
+evaluating trading strategies can be a daunting task, especially for users new
+to financial data analysis and Python development. To make the process as
+seamless as possible, we've prepared a collection of real-world [examples]
+(https://github.com/SIGTechnologies/sigtech-python/tree/master/examples) in
+Jupyter Notebook format (`.ipynb`). All you need to follow along is a SigTech
+API key. ## Logging Logs down to the `debug` log level are available for all
+API requests. They can be accessed using the Python `logging` library.
+```python import logging logging.basicConfig(level=logging.DEBUG) ``` For more
+information, please refer to the `logging` library's [documentation](https://
+docs.python.org/3/library/logging.html). ## Contributing We appreciate and
 encourage your contributions to the SigTech Python SDK! If you are enjoying the
 SDK, please show your support by starring this repository and sharing it on
 social media channels. To contribute an example, provide feedback, report a bug
 or otherwise bring an issue to our attention regarding this project, please
 follow the steps outlined in the [Contribution guidelines](https://github.com/
 SIGTechnologies/sigtech-python/blob/master/CONTRIBUTING.md). Please remember
 that all contributors are expected to behave appropriately and abide by our
 [Code of conduct](https://github.com/SIGTechnologies/sigtech-python/blob/
-master/CODE_OF_CONDUCT.md). ## Reporting security issues If you believe you
-have discovered a security vulnerability in our repository please report it to
-us immediately following the instructions [here](https://github.com/
-SIGTechnologies/sigtech-python/blob/master/SECURITY.md). >Attention!\ >Please
-follow the instructions detailed. **Do not** publicly disclose the
-vulnerability in a Github Issue or on a public forum such as Discord or
-Twitter. ## Support If you encounter any issues or have any questions regarding
-our API or SDK, you can reach out to us via our [Discord](https://discord.gg/
-ZcFeutSrWM) or [Twitter](https://twitter.com/sigtechltd/). ## License The
-SigTech Python SDK is released under the [MIT License](https://github.com/
+master/CODE_OF_CONDUCT.md). ## Security issues If you believe you have
+discovered a security vulnerability in our repository please report it to us
+immediately following the instructions [here](https://github.com/
+SIGTechnologies/sigtech-python/blob/master/SECURITY.md). >**Attention!**\ >Do
+not publicly disclose the vulnerability in a Github Issue or on a public forum
+such as X/Twitter. ## Support If you encounter any issues or have any questions
+regarding our API or SDK, you can reach out to us via email at
+[support@sigtech.com](mailto:support@sigtech.com). ## License The SigTech
+Python SDK is released under the [MIT License](https://github.com/
 SIGTechnologies/sigtech-python/blob/master/LICENSE).
```

### Comparing `sigtech-0.5.1/sigtech.egg-info/SOURCES.txt` & `sigtech-0.6.1/sigtech.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -33,13 +33,14 @@
 sigtech/api/framework/instruments/fx_otc.py
 sigtech/api/framework/instruments/indices.py
 sigtech/api/framework/instruments/ir_otc.py
 sigtech/api/framework/instruments/ois_swap.py
 sigtech/api/framework/strategies/__init__.py
 sigtech/api/framework/strategies/basket_strategy.py
 sigtech/api/framework/strategies/reinvestment_strategy.py
+sigtech/api/framework/strategies/rolling_bond_strategy.py
 sigtech/api/framework/strategies/rolling_future_strategy.py
 sigtech/api/framework/strategies/rolling_fx_forward_strategy.py
 sigtech/api/framework/strategies/rolling_swap_strategy.py
 sigtech/api/framework/strategies/signal_strategy.py
 sigtech/api/framework/strategies/strategy.py
 sigtech/api/jobs/__init__.py
```

