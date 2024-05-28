# Comparing `tmp/pkscreener-0.45.20240527.419.tar.gz` & `tmp/pkscreener-0.45.20240528.420.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.45.20240527.419.tar", last modified: Mon May 27 21:54:59 2024, max compression
+gzip compressed data, was "pkscreener-0.45.20240528.420.tar", last modified: Tue May 28 09:36:44 2024, max compression
```

## Comparing `pkscreener-0.45.20240527.419.tar` & `pkscreener-0.45.20240528.420.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:54:59.131188 pkscreener-0.45.20240527.419/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/LICENSE-Others
--rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-27 21:54:59.131188 pkscreener-0.45.20240527.419/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:54:59.127188 pkscreener-0.45.20240527.419/pkscreener/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:54:59.131188 pkscreener-0.45.20240527.419/pkscreener/classes/
--rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/ArtTexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/Backtest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/Barometer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/CandlePatterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/Changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)    33678 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/Fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/MarketMonitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/MarketStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)    46722 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/MenuOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/OtaUpdater.py
--rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/PKScanRunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/PKScheduledTaskProgress.py
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/PKScheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/PKSpreadsheets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/PKTask.py
--rw-r--r--   0 runner    (1001) docker     (127)    19048 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/Pktalib.py
--rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/Portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)    47779 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/PortfolioXRay.py
--rw-r--r--   0 runner    (1001) docker     (127)   158334 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/ScreeningStatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    56970 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/StockScreener.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/UserMenuChoicesHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    85524 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/Utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/WorkflowManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-27 21:54:52.000000 pkscreener-0.45.20240527.419/pkscreener/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/classes/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)   791436 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/courbd.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   145709 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/pkscreener.ini
--rw-r--r--   0 runner    (1001) docker     (127)    53279 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/pkscreenerbot.py
--rw-r--r--   0 runner    (1001) docker     (127)    33987 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/pkscreener/pkscreenercli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 21:54:59.127188 pkscreener-0.45.20240527.419/pkscreener.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-27 21:54:59.000000 pkscreener-0.45.20240527.419/pkscreener.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-27 21:54:59.000000 pkscreener-0.45.20240527.419/pkscreener.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 21:54:59.000000 pkscreener-0.45.20240527.419/pkscreener.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-27 21:54:59.000000 pkscreener-0.45.20240527.419/pkscreener.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 21:54:59.000000 pkscreener-0.45.20240527.419/pkscreener.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-27 21:54:59.000000 pkscreener-0.45.20240527.419/pkscreener.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-27 21:54:59.000000 pkscreener-0.45.20240527.419/pkscreener.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-27 21:54:59.131188 pkscreener-0.45.20240527.419/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-27 21:53:26.000000 pkscreener-0.45.20240527.419/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:36:44.146202 pkscreener-0.45.20240528.420/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/LICENSE-Others
+-rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-28 09:36:44.146202 pkscreener-0.45.20240528.420/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:36:44.142202 pkscreener-0.45.20240528.420/pkscreener/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:36:44.146202 pkscreener-0.45.20240528.420/pkscreener/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/ArtTexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/Backtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/Barometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/CandlePatterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/Changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33678 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/ConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/Fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/MarketMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/MarketStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47096 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/MenuOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/OtaUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/PKScanRunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/PKScheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/PKSpreadsheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/PKTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19048 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/Pktalib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/Portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47779 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/PortfolioXRay.py
+-rw-r--r--   0 runner    (1001) docker     (127)   158334 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/ScreeningStatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56970 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/StockScreener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85524 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/Utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/WorkflowManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-28 09:36:37.000000 pkscreener-0.45.20240528.420/pkscreener/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/classes/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)   791436 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/courbd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   145709 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/pkscreener.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    53805 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/pkscreenerbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33987 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/pkscreener/pkscreenercli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:36:44.142202 pkscreener-0.45.20240528.420/pkscreener.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-28 09:36:44.000000 pkscreener-0.45.20240528.420/pkscreener.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-28 09:36:44.000000 pkscreener-0.45.20240528.420/pkscreener.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:36:44.000000 pkscreener-0.45.20240528.420/pkscreener.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-28 09:36:44.000000 pkscreener-0.45.20240528.420/pkscreener.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:36:44.000000 pkscreener-0.45.20240528.420/pkscreener.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-28 09:36:44.000000 pkscreener-0.45.20240528.420/pkscreener.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-28 09:36:44.000000 pkscreener-0.45.20240528.420/pkscreener.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-28 09:36:44.150202 pkscreener-0.45.20240528.420/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-28 09:35:12.000000 pkscreener-0.45.20240528.420/setup.py
```

### Comparing `pkscreener-0.45.20240527.419/LICENSE` & `pkscreener-0.45.20240528.420/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/LICENSE-Others` & `pkscreener-0.45.20240528.420/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/PKG-INFO` & `pkscreener-0.45.20240528.420/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240527.419
+Version: 0.45.20240528.420
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240527.419.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240528.420.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -274,19 +274,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.418/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.419/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.418/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.419/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.418/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.419/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240527.419/README.md` & `pkscreener-0.45.20240528.420/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -252,19 +252,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.418/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.419/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.418/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.419/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.418/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.419/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240527.419/pkscreener/__init__.py` & `pkscreener-0.45.20240528.420/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/ArtTexts.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/Backtest.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/Barometer.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/Changelog.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/ConfigManager.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/Fetcher.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/MarketStatus.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/MenuOptions.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/MenuOptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -624,15 +624,15 @@
             renderExceptionKeys=["M"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
             substitutes = substitutes
-        ).render(asList=asList,coloredValues=["M"])
+        ).render(asList=asList,coloredValues=["M"] if not asList else [])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -657,15 +657,15 @@
             level0MenuDict,
             renderExceptionKeys=["P", "T", "E", "U", "Z", "L", "D"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList,coloredValues=["X"])
+        ).render(asList=asList,coloredValues=["X"] if not asList else [])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -738,15 +738,15 @@
             level1_T_MenuDict,
             renderExceptionKeys=["M"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList,coloredValues=[defaultKey])
+        ).render(asList=asList,coloredValues=[defaultKey] if not asList else [])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -773,15 +773,15 @@
             level1_P_MenuDict,
             renderExceptionKeys=["M"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList, coloredValues=["1"])
+        ).render(asList=asList, coloredValues=["1"] if not asList else [])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -808,15 +808,15 @@
             level2_P_MenuDict,
             renderExceptionKeys=["M"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.TWO_PER_ROW,
             skip=skip,
             parent=parent,
-        ).render(asList=asList,coloredValues=["1"])
+        ).render(asList=asList,coloredValues=["1"] if not asList else [])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -843,15 +843,15 @@
             level1_X_MenuDict,
             renderExceptionKeys=["W", "0", "M", "15"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.THREE_PER_ROW,
             skip=skip,
             parent=parent,
-        ).render(asList=asList, coloredValues=["15",str(configManager.defaultIndex)])
+        ).render(asList=asList, coloredValues=["15",str(configManager.defaultIndex)] if not asList else [])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -878,15 +878,15 @@
             level2_T_MenuDict_L,
             renderExceptionKeys=["4","5","M"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList, coloredValues=["1"])
+        ).render(asList=asList, coloredValues=["1"] if not asList else [])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -913,15 +913,15 @@
             level2_T_MenuDict_S,
             renderExceptionKeys=["5", "M"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList, coloredValues=["1"])
+        ).render(asList=asList, coloredValues=["1"] if not asList else [])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -948,15 +948,15 @@
             level2_X_MenuDict,
             renderExceptionKeys=["0", "42", "M"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.TWO_PER_ROW,
             skip=skip,
             parent=parent,
-        ).render(asList=asList, coloredValues=["9"])
+        ).render(asList=asList, coloredValues=["9"] if not asList else [])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -982,15 +982,15 @@
             level3_X_Reversal_MenuDict,
             renderExceptionKeys=["0"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList,coloredValues=["3"])
+        ).render(asList=asList,coloredValues=["3"] if not asList else [])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -1016,15 +1016,15 @@
             level3_X_ChartPattern_MenuDict,
             renderExceptionKeys=["0"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList,coloredValues=["3"])
+        ).render(asList=asList,coloredValues=["3"] if not asList else [])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -1050,15 +1050,15 @@
             level3_X_PopularStocks_MenuDict,
             renderExceptionKeys=["0"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList, coloredValues=["1"])
+        ).render(asList=asList, coloredValues=["1"] if not asList else [])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -1084,15 +1084,15 @@
             level3_X_StockPerformance_MenuDict,
             renderExceptionKeys=["0"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList,coloredValues=["1"])
+        ).render(asList=asList,coloredValues=["1"] if not asList else [])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -1118,15 +1118,15 @@
             level4_X_Lorenzian_MenuDict,
             renderExceptionKeys=["0"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList, coloredValues=["1"])
+        ).render(asList=asList, coloredValues=["1"] if not asList else [])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -1153,15 +1153,15 @@
             level4_X_ChartPattern_BBands_SQZ_MenuDict,
             renderExceptionKeys=["0"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList, coloredValues=["1"])
+        ).render(asList=asList, coloredValues=["1"] if not asList else [])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -1187,15 +1187,15 @@
             level4_X_ChartPattern_MASignalMenuDict,
             renderExceptionKeys=["0"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList, coloredValues=["1"])
+        ).render(asList=asList, coloredValues=["1"] if not asList else [])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
@@ -1221,15 +1221,15 @@
             level4_X_ChartPattern_Confluence_MenuDict,
             renderExceptionKeys=["0"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
             parent=parent,
-        ).render(asList=asList,coloredValues=["1"])
+        ).render(asList=asList,coloredValues=["1"] if not asList else [])
         if asList:
             return menuText
         else:
             if OutputControls().enableMultipleLineOutput:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.WARN
```

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/PKScheduler.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/PKTask.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/Pktalib.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/Portfolio.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/StockScreener.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/Utility.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/classes/keys.py` & `pkscreener-0.45.20240528.420/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/courbd.ttf` & `pkscreener-0.45.20240528.420/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/globals.py` & `pkscreener-0.45.20240528.420/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/pkscreener.ini` & `pkscreener-0.45.20240528.420/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener/pkscreenerbot.py` & `pkscreener-0.45.20240528.420/pkscreener/pkscreenerbot.py`

 * *Files 2% similar despite different names*

```diff
@@ -355,14 +355,15 @@
         m1.renderForMenu(
             m0.find(data),
             skip=skipMenus,
             renderStyle=MenuRenderStyle.STANDALONE,
         )
         .replace("     ", "")
         .replace("    ", "")
+        .replace("  ", "")
         .replace("\t", "")
         .replace(colorText.FAIL,"").replace(colorText.END,"")
     )
     menuText = menuText + "\n\nH > Home"
     mns = m1.renderForMenu(
         m0.find(data),
         skip=skipMenus,
@@ -377,14 +378,15 @@
                 mnu.menuKey, callback_data=str(f"{query.data}_{mnu.menuKey}")
             )
         )
     keyboard = [inlineMenus]
     reply_markup = InlineKeyboardMarkup(keyboard)
     if query.message.text == menuText:
         menuText = f"{PKDateUtilities.currentDateTime()}:\n{menuText}"
+    menuText = f"{menuText}\nClick /start if you want to restart the session."
     await query.edit_message_text(text=menuText, reply_markup=reply_markup)
     return START_ROUTES
 
 
 async def Level2(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
     """Show new choice of buttons"""
     inlineMenus = []
@@ -575,14 +577,15 @@
     reply_markup = InlineKeyboardMarkup(keyboard)
     return reply_markup
 
 
 async def sendUpdatedMenu(menuText, update: Update, context, reply_markup, replaceWhiteSpaces=True):
     try:
         menuText.replace("     ", "").replace("    ", "").replace("\t", "").replace(colorText.FAIL,"").replace(colorText.END,"") if replaceWhiteSpaces else menuText
+        menuText = f"{menuText}\nClick /start if you want to restart the session."
         if update.callback_query.message.text == menuText:
             menuText = f"{PKDateUtilities.currentDateTime()}:\n{menuText}"
         await update.callback_query.edit_message_text(
             text=menuText,
             parse_mode="HTML",
             reply_markup=reply_markup,
         )
@@ -602,14 +605,15 @@
             responseText = f"Thank you for choosing {optionChoices}!\n\nHere are the results:\n\nInsights: https://pkjmesra.github.io/PKScreener/Backtest-Reports/PKScreener_{optionChoices}_Insights_DateSorted.html"
             responseText = f"{responseText}\n\nSummary: https://pkjmesra.github.io/PKScreener/Backtest-Reports/PKScreener_{optionChoices}_Summary_StockSorted.html"
             responseText = f"{responseText}\n\nStock-wise: https://pkjmesra.github.io/PKScreener/Backtest-Reports/PKScreener_{optionChoices}_backtest_result_StockSorted.html"
             responseText = f"{responseText}\n\nOther Reports: https://pkjmesra.github.io/PKScreener/BacktestReports.html"
             if update is not None and update.message is not None:
                 await update.message.reply_text(responseText)
             else:
+                responseText = f"{responseText}\nClick /start if you want to restart the session."
                 await update.callback_query.edit_message_text(
                     text=responseText,
                     reply_markup=default_markup([]),
                 )
             await shareUpdateWithChannel(
                 update=update, context=context, optionChoices=optionChoices
             )
@@ -656,29 +660,33 @@
     keyboard = [
         [
             InlineKeyboardButton("Try Scanners", callback_data=str("CX")),
             # InlineKeyboardButton("Growth of 10k", callback_data=str("CG")),
         ]
     ]
     reply_markup = InlineKeyboardMarkup(keyboard)
+    responseText = "Backtesting NOT implemented yet in this Bot!\n\n\nYou can use backtesting by downloading the software from https://github.com/pkjmesra/PKScreener/"
+    responseText = f"{responseText}\nClick /start if you want to restart the session."
     await query.edit_message_text(
-        text="Backtesting NOT implemented yet in this Bot!\n\n\nYou can use backtesting by downloading the software from https://github.com/pkjmesra/PKScreener/",
+        text=responseText,
         reply_markup=reply_markup,
     )
     return START_ROUTES
 
 
 async def end(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
     """Returns `ConversationHandler.END`, which tells the
     ConversationHandler that the conversation is over.
     """
     query = update.callback_query
     await query.answer()
+    responseText = "See https://github.com/pkjmesra/PKScreener/ for more details or join https://t.me/PKScreener. \n\n\nSee you next time!"
+    responseText = f"{responseText}\nClick /start if you want to restart the session."
     await query.edit_message_text(
-        text="See https://github.com/pkjmesra/PKScreener/ for more details or join https://t.me/PKScreener. \n\n\nSee you next time!"
+        text=responseText
     )
     return ConversationHandler.END
 
 
 # This can be your own ID, or one for a developer group/channel.
 # You can use the /start command of this bot to see your chat id.
 chat_idADMIN = 123456789
```

### Comparing `pkscreener-0.45.20240527.419/pkscreener/pkscreenercli.py` & `pkscreener-0.45.20240528.420/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.45.20240528.420/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240527.419
+Version: 0.45.20240528.420
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240527.419.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240528.420.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -274,19 +274,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.418/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.419/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.418/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.419/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.418/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240527.419/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240527.419/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.45.20240528.420/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240527.419/setup.py` & `pkscreener-0.45.20240528.420/setup.py`

 * *Files identical despite different names*

