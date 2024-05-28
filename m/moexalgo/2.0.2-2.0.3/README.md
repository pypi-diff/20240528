# Comparing `tmp/moexalgo-2.0.2.tar.gz` & `tmp/moexalgo-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moexalgo-2.0.2.tar", last modified: Fri May  3 14:38:58 2024, max compression
+gzip compressed data, was "moexalgo-2.0.3.tar", last modified: Fri May  3 15:00:25 2024, max compression
```

## Comparing `moexalgo-2.0.2.tar` & `moexalgo-2.0.3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:38:58.158493 moexalgo-2.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:38:58.146493 moexalgo-2.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:38:58.146493 moexalgo-2.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-03 14:38:53.000000 moexalgo-2.0.2/.github/workflows/python-publish_flow.yml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-03 14:38:53.000000 moexalgo-2.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-03 14:38:53.000000 moexalgo-2.0.2/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-03 14:38:53.000000 moexalgo-2.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-03 14:38:58.154493 moexalgo-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-03 14:38:53.000000 moexalgo-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:38:58.146493 moexalgo-2.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-03 14:38:53.000000 moexalgo-2.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-03 14:38:53.000000 moexalgo-2.0.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:38:58.150493 moexalgo-2.0.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:38:58.150493 moexalgo-2.0.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    48404 2024-05-03 14:38:53.000000 moexalgo-2.0.2/docs/source/_static/newplot.png
--rw-r--r--   0 runner    (1001) docker     (127)    34177 2024-05-03 14:38:53.000000 moexalgo-2.0.2/docs/source/_static/output_4_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-03 14:38:53.000000 moexalgo-2.0.2/docs/source/candels.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-03 14:38:53.000000 moexalgo-2.0.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-03 14:38:53.000000 moexalgo-2.0.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-03 14:38:53.000000 moexalgo-2.0.2/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-03 14:38:53.000000 moexalgo-2.0.2/docs/source/moexalgo.currency.rst
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-03 14:38:53.000000 moexalgo-2.0.2/docs/source/moexalgo.futures.rst
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-03 14:38:53.000000 moexalgo-2.0.2/docs/source/moexalgo.indices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-03 14:38:53.000000 moexalgo-2.0.2/docs/source/moexalgo.market.rst
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-03 14:38:53.000000 moexalgo-2.0.2/docs/source/moexalgo.models.common.rst
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-03 14:38:53.000000 moexalgo-2.0.2/docs/source/moexalgo.models.indices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-03 14:38:53.000000 moexalgo-2.0.2/docs/source/moexalgo.models.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-03 14:38:53.000000 moexalgo-2.0.2/docs/source/moexalgo.models.shares.rst
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-03 14:38:53.000000 moexalgo-2.0.2/docs/source/moexalgo.rst
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-03 14:38:53.000000 moexalgo-2.0.2/docs/source/moexalgo.session.rst
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-03 14:38:53.000000 moexalgo-2.0.2/docs/source/moexalgo.stocks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-03 14:38:53.000000 moexalgo-2.0.2/docs/source/moexalgo.tickers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-03 14:38:53.000000 moexalgo-2.0.2/docs/source/moexalgo.utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:38:58.154493 moexalgo-2.0.2/moexalgo/
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-03 14:38:53.000000 moexalgo-2.0.2/moexalgo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 14:38:58.000000 moexalgo-2.0.2/moexalgo/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-03 14:38:53.000000 moexalgo-2.0.2/moexalgo/candles.py
--rw-r--r--   0 runner    (1001) docker     (127)    13794 2024-05-03 14:38:53.000000 moexalgo-2.0.2/moexalgo/currency.py
--rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-03 14:38:53.000000 moexalgo-2.0.2/moexalgo/futures.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-03 14:38:53.000000 moexalgo-2.0.2/moexalgo/indices.py
--rw-r--r--   0 runner    (1001) docker     (127)    24499 2024-05-03 14:38:53.000000 moexalgo-2.0.2/moexalgo/market.py
--rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-05-03 14:38:53.000000 moexalgo-2.0.2/moexalgo/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:38:58.154493 moexalgo-2.0.2/moexalgo/models/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-03 14:38:53.000000 moexalgo-2.0.2/moexalgo/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-03 14:38:53.000000 moexalgo-2.0.2/moexalgo/models/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-03 14:38:53.000000 moexalgo-2.0.2/moexalgo/models/indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-03 14:38:53.000000 moexalgo-2.0.2/moexalgo/models/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12982 2024-05-03 14:38:53.000000 moexalgo-2.0.2/moexalgo/models/shares.py
--rw-r--r--   0 runner    (1001) docker     (127)    13976 2024-05-03 14:38:53.000000 moexalgo-2.0.2/moexalgo/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    13607 2024-05-03 14:38:53.000000 moexalgo-2.0.2/moexalgo/stocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-03 14:38:53.000000 moexalgo-2.0.2/moexalgo/tickers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-03 14:38:53.000000 moexalgo-2.0.2/moexalgo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:38:58.154493 moexalgo-2.0.2/moexalgo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-03 14:38:58.000000 moexalgo-2.0.2/moexalgo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-03 14:38:58.000000 moexalgo-2.0.2/moexalgo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 14:38:58.000000 moexalgo-2.0.2/moexalgo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-03 14:38:58.000000 moexalgo-2.0.2/moexalgo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 14:38:58.000000 moexalgo-2.0.2/moexalgo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-03 14:38:53.000000 moexalgo-2.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:38:58.154493 moexalgo-2.0.2/samples/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 14:38:53.000000 moexalgo-2.0.2/samples/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-03 14:38:53.000000 moexalgo-2.0.2/samples/auth.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   138920 2024-05-03 14:38:53.000000 moexalgo-2.0.2/samples/quick_start.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 14:38:58.158493 moexalgo-2.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:38:58.154493 moexalgo-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 14:38:53.000000 moexalgo-2.0.2/tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-03 14:38:53.000000 moexalgo-2.0.2/tests/test_currency.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-03 14:38:53.000000 moexalgo-2.0.2/tests/test_futures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-03 14:38:53.000000 moexalgo-2.0.2/tests/test_markets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-03 14:38:53.000000 moexalgo-2.0.2/tests/test_stocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-03 14:38:53.000000 moexalgo-2.0.2/tests/test_tickers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:00:25.298800 moexalgo-2.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:00:25.286800 moexalgo-2.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:00:25.290799 moexalgo-2.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-03 15:00:20.000000 moexalgo-2.0.3/.github/workflows/python-publish_flow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-03 15:00:20.000000 moexalgo-2.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-03 15:00:20.000000 moexalgo-2.0.3/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-03 15:00:20.000000 moexalgo-2.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-03 15:00:25.298800 moexalgo-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-03 15:00:20.000000 moexalgo-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:00:25.290799 moexalgo-2.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:00:25.290799 moexalgo-2.0.3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:00:25.290799 moexalgo-2.0.3/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    48404 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/_static/newplot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34177 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/_static/output_4_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/candels.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.currency.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.futures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.indices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.market.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.models.common.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.models.indices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.models.shares.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.session.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.stocks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.tickers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:00:25.294800 moexalgo-2.0.3/moexalgo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 15:00:25.000000 moexalgo-2.0.3/moexalgo/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/candles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13794 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24499 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/market.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:00:25.294800 moexalgo-2.0.3/moexalgo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/models/indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/models/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12982 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/models/shares.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14033 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13607 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/stocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/tickers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:00:25.298800 moexalgo-2.0.3/moexalgo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-03 15:00:25.000000 moexalgo-2.0.3/moexalgo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-03 15:00:25.000000 moexalgo-2.0.3/moexalgo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:00:25.000000 moexalgo-2.0.3/moexalgo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-03 15:00:25.000000 moexalgo-2.0.3/moexalgo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 15:00:25.000000 moexalgo-2.0.3/moexalgo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-03 15:00:20.000000 moexalgo-2.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:00:25.298800 moexalgo-2.0.3/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 15:00:20.000000 moexalgo-2.0.3/samples/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-03 15:00:20.000000 moexalgo-2.0.3/samples/auth.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   138920 2024-05-03 15:00:20.000000 moexalgo-2.0.3/samples/quick_start.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 15:00:25.298800 moexalgo-2.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:00:25.298800 moexalgo-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 15:00:20.000000 moexalgo-2.0.3/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-03 15:00:20.000000 moexalgo-2.0.3/tests/test_currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-03 15:00:20.000000 moexalgo-2.0.3/tests/test_futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-03 15:00:20.000000 moexalgo-2.0.3/tests/test_markets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-03 15:00:20.000000 moexalgo-2.0.3/tests/test_stocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-03 15:00:20.000000 moexalgo-2.0.3/tests/test_tickers.py
```

### Comparing `moexalgo-2.0.2/.github/workflows/python-publish_flow.yml` & `moexalgo-2.0.3/.github/workflows/python-publish_flow.yml`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/.gitlab-ci.yml` & `moexalgo-2.0.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/CHANGELOG.md` & `moexalgo-2.0.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/PKG-INFO` & `moexalgo-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moexalgo
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python lib for MOEX AlgoPack data
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Financial and Insurance Industry
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `moexalgo-2.0.2/README.md` & `moexalgo-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/docs/Makefile` & `moexalgo-2.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/docs/make.bat` & `moexalgo-2.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/docs/source/_static/newplot.png` & `moexalgo-2.0.3/docs/source/_static/newplot.png`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/docs/source/_static/output_4_0.png` & `moexalgo-2.0.3/docs/source/_static/output_4_0.png`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/docs/source/candels.rst` & `moexalgo-2.0.3/docs/source/candels.rst`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/docs/source/conf.py` & `moexalgo-2.0.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/moexalgo/__init__.py` & `moexalgo-2.0.3/moexalgo/__init__.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/moexalgo/candles.py` & `moexalgo-2.0.3/moexalgo/candles.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/moexalgo/currency.py` & `moexalgo-2.0.3/moexalgo/currency.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/moexalgo/futures.py` & `moexalgo-2.0.3/moexalgo/futures.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/moexalgo/indices.py` & `moexalgo-2.0.3/moexalgo/indices.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/moexalgo/market.py` & `moexalgo-2.0.3/moexalgo/market.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/moexalgo/metrics.py` & `moexalgo-2.0.3/moexalgo/metrics.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/moexalgo/models/common.py` & `moexalgo-2.0.3/moexalgo/models/common.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/moexalgo/models/indices.py` & `moexalgo-2.0.3/moexalgo/models/indices.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/moexalgo/models/metrics.py` & `moexalgo-2.0.3/moexalgo/models/metrics.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/moexalgo/models/shares.py` & `moexalgo-2.0.3/moexalgo/models/shares.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/moexalgo/session.py` & `moexalgo-2.0.3/moexalgo/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -451,11 +451,13 @@
         while True:
             options['start'] = start
             items = client.get_objects(path, lambda data: result_deserializer(data, section), **options)
             if metrics := items.get(section):
                 for item in metrics:
                     yield item
                     start += 1
-                    if (start - offset) >= limit or limit < -1:
+                    if (start - offset) >= limit and limit > 0:
                         return
+                if limit < 0:
+                    return
             else:
                 return
```

### Comparing `moexalgo-2.0.2/moexalgo/stocks.py` & `moexalgo-2.0.3/moexalgo/stocks.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/moexalgo/tickers.py` & `moexalgo-2.0.3/moexalgo/tickers.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/moexalgo/utils.py` & `moexalgo-2.0.3/moexalgo/utils.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/moexalgo.egg-info/PKG-INFO` & `moexalgo-2.0.3/moexalgo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moexalgo
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python lib for MOEX AlgoPack data
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Financial and Insurance Industry
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `moexalgo-2.0.2/moexalgo.egg-info/SOURCES.txt` & `moexalgo-2.0.3/moexalgo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/pyproject.toml` & `moexalgo-2.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/samples/auth.ipynb` & `moexalgo-2.0.3/samples/auth.ipynb`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/samples/quick_start.ipynb` & `moexalgo-2.0.3/samples/quick_start.ipynb`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/tests/test_currency.py` & `moexalgo-2.0.3/tests/test_currency.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/tests/test_futures.py` & `moexalgo-2.0.3/tests/test_futures.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/tests/test_markets.py` & `moexalgo-2.0.3/tests/test_markets.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/tests/test_stocks.py` & `moexalgo-2.0.3/tests/test_stocks.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.2/tests/test_tickers.py` & `moexalgo-2.0.3/tests/test_tickers.py`

 * *Files identical despite different names*

