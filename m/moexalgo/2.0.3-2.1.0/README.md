# Comparing `tmp/moexalgo-2.0.3.tar.gz` & `tmp/moexalgo-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moexalgo-2.0.3.tar", last modified: Fri May  3 15:00:25 2024, max compression
+gzip compressed data, was "moexalgo-2.1.0.tar", last modified: Tue May 28 15:57:04 2024, max compression
```

## Comparing `moexalgo-2.0.3.tar` & `moexalgo-2.1.0.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:00:25.298800 moexalgo-2.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:00:25.286800 moexalgo-2.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:00:25.290799 moexalgo-2.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-03 15:00:20.000000 moexalgo-2.0.3/.github/workflows/python-publish_flow.yml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-03 15:00:20.000000 moexalgo-2.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-03 15:00:20.000000 moexalgo-2.0.3/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-03 15:00:20.000000 moexalgo-2.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-03 15:00:25.298800 moexalgo-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-03 15:00:20.000000 moexalgo-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:00:25.290799 moexalgo-2.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:00:25.290799 moexalgo-2.0.3/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:00:25.290799 moexalgo-2.0.3/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    48404 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/_static/newplot.png
--rw-r--r--   0 runner    (1001) docker     (127)    34177 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/_static/output_4_0.png
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/candels.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.currency.rst
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.futures.rst
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.indices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.market.rst
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.models.common.rst
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.models.indices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.models.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.models.shares.rst
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.rst
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.session.rst
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.stocks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.tickers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-03 15:00:20.000000 moexalgo-2.0.3/docs/source/moexalgo.utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:00:25.294800 moexalgo-2.0.3/moexalgo/
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 15:00:25.000000 moexalgo-2.0.3/moexalgo/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/candles.py
--rw-r--r--   0 runner    (1001) docker     (127)    13794 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/currency.py
--rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/futures.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/indices.py
--rw-r--r--   0 runner    (1001) docker     (127)    24499 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/market.py
--rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:00:25.294800 moexalgo-2.0.3/moexalgo/models/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/models/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/models/indices.py
--rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/models/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12982 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/models/shares.py
--rw-r--r--   0 runner    (1001) docker     (127)    14033 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    13607 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/stocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10911 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/tickers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-03 15:00:20.000000 moexalgo-2.0.3/moexalgo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:00:25.298800 moexalgo-2.0.3/moexalgo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-03 15:00:25.000000 moexalgo-2.0.3/moexalgo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-03 15:00:25.000000 moexalgo-2.0.3/moexalgo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:00:25.000000 moexalgo-2.0.3/moexalgo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-03 15:00:25.000000 moexalgo-2.0.3/moexalgo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 15:00:25.000000 moexalgo-2.0.3/moexalgo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-03 15:00:20.000000 moexalgo-2.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:00:25.298800 moexalgo-2.0.3/samples/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-03 15:00:20.000000 moexalgo-2.0.3/samples/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-03 15:00:20.000000 moexalgo-2.0.3/samples/auth.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   138920 2024-05-03 15:00:20.000000 moexalgo-2.0.3/samples/quick_start.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 15:00:25.298800 moexalgo-2.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:00:25.298800 moexalgo-2.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 15:00:20.000000 moexalgo-2.0.3/tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-03 15:00:20.000000 moexalgo-2.0.3/tests/test_currency.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-03 15:00:20.000000 moexalgo-2.0.3/tests/test_futures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-03 15:00:20.000000 moexalgo-2.0.3/tests/test_markets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-03 15:00:20.000000 moexalgo-2.0.3/tests/test_stocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-03 15:00:20.000000 moexalgo-2.0.3/tests/test_tickers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:57:04.232902 moexalgo-2.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:57:04.216902 moexalgo-2.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:57:04.220902 moexalgo-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-28 15:56:59.000000 moexalgo-2.1.0/.github/workflows/python-publish_flow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-28 15:56:59.000000 moexalgo-2.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-28 15:56:59.000000 moexalgo-2.1.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-28 15:56:59.000000 moexalgo-2.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-05-28 15:57:04.232902 moexalgo-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-05-28 15:56:59.000000 moexalgo-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:57:04.220902 moexalgo-2.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-28 15:56:59.000000 moexalgo-2.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-28 15:56:59.000000 moexalgo-2.1.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:57:04.224902 moexalgo-2.1.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:57:04.224902 moexalgo-2.1.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    48404 2024-05-28 15:56:59.000000 moexalgo-2.1.0/docs/source/_static/newplot.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34177 2024-05-28 15:56:59.000000 moexalgo-2.1.0/docs/source/_static/output_4_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-05-28 15:56:59.000000 moexalgo-2.1.0/docs/source/candels.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-28 15:56:59.000000 moexalgo-2.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-28 15:56:59.000000 moexalgo-2.1.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-28 15:56:59.000000 moexalgo-2.1.0/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-28 15:56:59.000000 moexalgo-2.1.0/docs/source/moexalgo.currency.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-28 15:56:59.000000 moexalgo-2.1.0/docs/source/moexalgo.futures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-28 15:56:59.000000 moexalgo-2.1.0/docs/source/moexalgo.indices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-28 15:56:59.000000 moexalgo-2.1.0/docs/source/moexalgo.market.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-28 15:56:59.000000 moexalgo-2.1.0/docs/source/moexalgo.models.common.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 15:56:59.000000 moexalgo-2.1.0/docs/source/moexalgo.models.indices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-28 15:56:59.000000 moexalgo-2.1.0/docs/source/moexalgo.models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-28 15:56:59.000000 moexalgo-2.1.0/docs/source/moexalgo.models.shares.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-28 15:56:59.000000 moexalgo-2.1.0/docs/source/moexalgo.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-28 15:56:59.000000 moexalgo-2.1.0/docs/source/moexalgo.session.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-28 15:56:59.000000 moexalgo-2.1.0/docs/source/moexalgo.stocks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-28 15:56:59.000000 moexalgo-2.1.0/docs/source/moexalgo.tickers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-28 15:56:59.000000 moexalgo-2.1.0/docs/source/moexalgo.utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:57:04.224902 moexalgo-2.1.0/moexalgo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-28 15:56:59.000000 moexalgo-2.1.0/moexalgo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-28 15:57:04.000000 moexalgo-2.1.0/moexalgo/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-28 15:56:59.000000 moexalgo-2.1.0/moexalgo/candles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13794 2024-05-28 15:56:59.000000 moexalgo-2.1.0/moexalgo/currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-28 15:56:59.000000 moexalgo-2.1.0/moexalgo/futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-28 15:56:59.000000 moexalgo-2.1.0/moexalgo/indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25362 2024-05-28 15:56:59.000000 moexalgo-2.1.0/moexalgo/market.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-28 15:56:59.000000 moexalgo-2.1.0/moexalgo/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:57:04.228901 moexalgo-2.1.0/moexalgo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-28 15:56:59.000000 moexalgo-2.1.0/moexalgo/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-28 15:56:59.000000 moexalgo-2.1.0/moexalgo/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-05-28 15:56:59.000000 moexalgo-2.1.0/moexalgo/models/indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-05-28 15:56:59.000000 moexalgo-2.1.0/moexalgo/models/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12982 2024-05-28 15:56:59.000000 moexalgo-2.1.0/moexalgo/models/shares.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14033 2024-05-28 15:56:59.000000 moexalgo-2.1.0/moexalgo/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13607 2024-05-28 15:56:59.000000 moexalgo-2.1.0/moexalgo/stocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13276 2024-05-28 15:56:59.000000 moexalgo-2.1.0/moexalgo/tickers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-05-28 15:56:59.000000 moexalgo-2.1.0/moexalgo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:57:04.228901 moexalgo-2.1.0/moexalgo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6086 2024-05-28 15:57:04.000000 moexalgo-2.1.0/moexalgo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-28 15:57:04.000000 moexalgo-2.1.0/moexalgo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:57:04.000000 moexalgo-2.1.0/moexalgo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-28 15:57:04.000000 moexalgo-2.1.0/moexalgo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 15:57:04.000000 moexalgo-2.1.0/moexalgo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-28 15:56:59.000000 moexalgo-2.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:57:04.228901 moexalgo-2.1.0/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 15:56:59.000000 moexalgo-2.1.0/samples/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-28 15:56:59.000000 moexalgo-2.1.0/samples/auth.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-05-28 15:56:59.000000 moexalgo-2.1.0/samples/download_algopack_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   115636 2024-05-28 15:56:59.000000 moexalgo-2.1.0/samples/quick_start.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:57:04.232902 moexalgo-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:57:04.228901 moexalgo-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-28 15:56:59.000000 moexalgo-2.1.0/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-28 15:56:59.000000 moexalgo-2.1.0/tests/test_currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-28 15:56:59.000000 moexalgo-2.1.0/tests/test_futures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-28 15:56:59.000000 moexalgo-2.1.0/tests/test_markets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-28 15:56:59.000000 moexalgo-2.1.0/tests/test_stocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-28 15:56:59.000000 moexalgo-2.1.0/tests/test_tickers.py
```

### Comparing `moexalgo-2.0.3/.github/workflows/python-publish_flow.yml` & `moexalgo-2.1.0/.github/workflows/python-publish_flow.yml`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.3/.gitlab-ci.yml` & `moexalgo-2.1.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.3/CHANGELOG.md` & `moexalgo-2.1.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.3/PKG-INFO` & `moexalgo-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moexalgo
-Version: 2.0.3
+Version: 2.1.0
 Summary: Python lib for MOEX AlgoPack data
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Financial and Insurance Industry
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -49,17 +49,19 @@
 
 <br>
 
 ## 🚀 Пример использования
 
 <hr>
 
-#### ⚡️ Быстрое знакомство с библиотекой MoexAlgo - [quick_start.ipynb](https://github.com/moexalgo/moexalgo/blob/main/samples/quick_start.ipynb)
+#### ⚡️ Быстрое знакомство с библиотекой MoexAlgo - [quick_start.ipynb](./samples/quick_start.ipynb)
 
-#### 🔐 Пример авторизации - [auth.ipynb](https://github.com/moexalgo/moexalgo/blob/main/samples/auth.ipynb)
+#### ⬇️ Получение данных через API - [download_algopack_data.ipynb](./samples/download_algopack_data.ipynb)
+
+#### 🔐 Пример авторизации - [auth.ipynb](./samples/auth.ipynb)
 <hr>
 
 Для работы с библиотекой необходимо авторизоваться на https://passport.moex.com
 
 ```python
 from moexalgo import session
```

### Comparing `moexalgo-2.0.3/README.md` & `moexalgo-2.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -35,17 +35,19 @@
 
 <br>
 
 ## 🚀 Пример использования
 
 <hr>
 
-#### ⚡️ Быстрое знакомство с библиотекой MoexAlgo - [quick_start.ipynb](https://github.com/moexalgo/moexalgo/blob/main/samples/quick_start.ipynb)
+#### ⚡️ Быстрое знакомство с библиотекой MoexAlgo - [quick_start.ipynb](./samples/quick_start.ipynb)
 
-#### 🔐 Пример авторизации - [auth.ipynb](https://github.com/moexalgo/moexalgo/blob/main/samples/auth.ipynb)
+#### ⬇️ Получение данных через API - [download_algopack_data.ipynb](./samples/download_algopack_data.ipynb)
+
+#### 🔐 Пример авторизации - [auth.ipynb](./samples/auth.ipynb)
 <hr>
 
 Для работы с библиотекой необходимо авторизоваться на https://passport.moex.com
 
 ```python
 from moexalgo import session
```

### Comparing `moexalgo-2.0.3/docs/Makefile` & `moexalgo-2.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.3/docs/make.bat` & `moexalgo-2.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.3/docs/source/_static/newplot.png` & `moexalgo-2.1.0/docs/source/_static/newplot.png`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.3/docs/source/_static/output_4_0.png` & `moexalgo-2.1.0/docs/source/_static/output_4_0.png`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.3/docs/source/candels.rst` & `moexalgo-2.1.0/docs/source/candels.rst`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 Также, можно получить справочную информацию по инструментам, свечи и прочую торговую статистику
 
 Пример использования
 --------------------
 
 Быстрое знакомство с библиотекой moexalgo - `quick_start.ipynb <./../../../samples/quick_start.ipynb>`_
 
+Получение данных с использованием API - `download_algopack_data.ipynb <./../../../samples/download_algopack_data.ipynb>`_
+
 Пример авторизации - `auth.ipynb <./../../../samples/auth.ipynb>`_
 
 Для работы с библиотекой необходимо авторизоваться на https://passport.moex.com
 
 .. code:: python
 
     from moexalgo import session
```

### Comparing `moexalgo-2.0.3/docs/source/conf.py` & `moexalgo-2.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.3/moexalgo/__init__.py` & `moexalgo-2.1.0/moexalgo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,17 +54,18 @@
         >>> try:
         >>>     instrument = Ticker("GAZP", "TQBR")
         >>>     print(instrument)
         >>> except LookupError:
         >>>     print("Тикер не найден.")
     """
     if boardid is None:
-        secid, *args = re.split('\W', secid)
+        secid, *args = re.split('[^a-zA-Z0-9-]', secid)
         if args:
             boardid = args[0]
+
     stocks = Market('stocks', boardid)
     if stocks._ticker_info(secid):
         return Stock(secid, stocks._boardid)
 
     currencies = Market('selt', boardid)
     if currencies._ticker_info(secid):
         return Currency(secid, currencies._boardid)
```

### Comparing `moexalgo-2.0.3/moexalgo/candles.py` & `moexalgo-2.1.0/moexalgo/candles.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.3/moexalgo/currency.py` & `moexalgo-2.1.0/moexalgo/currency.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.3/moexalgo/futures.py` & `moexalgo-2.1.0/moexalgo/futures.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.3/moexalgo/indices.py` & `moexalgo-2.1.0/moexalgo/indices.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.3/moexalgo/market.py` & `moexalgo-2.1.0/moexalgo/market.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 from datetime import date
 import re
+from datetime import date
 from typing import Optional, Union
 
 from moexalgo import session
 from moexalgo.metrics import prepare_market_request, dataclass_it, pandas_frame
-from moexalgo.session import Session
+from moexalgo.session import Session, data_gen
 from moexalgo.utils import result_deserializer, pd
 
 _AVAILABLE = {
     'index': dict(),
     'shares': dict(),
     'selt': dict(),
     
@@ -118,14 +119,15 @@
     """
     _name: str
     _path: str
     _pref: str
     _boardid: str
     _fields: dict[str, dict[str, dict]] = None
     _values: dict[str, dict[str, dict]] = None
+    _delisted: list = None
     _LIMIT = 25_000
 
     def __new__(cls, name: str, boardid: str = None) -> Market:
         """
         Создает новый экземпляр класса Market.
 
         Parameters
@@ -157,15 +159,15 @@
         path = 'engines/stock/markets'
         if boardid is None:
             name_, boardid = _ALIASES.get(name, (None, None))
 
             if boardid is not None:
                 name = name_
             else:
-                name, *args = re.split('\W', name)
+                name, *args = re.split('[^a-zA-Z0-9-]', name)
                 if args:
                     boardid = args[0]
             
         if '/' in name:
             *path, name = name.split('/')
             path = "/".join(item for item in path if item)
         
@@ -206,14 +208,28 @@
                     f'{self._path}/{self._name}/boards/{self._boardid}/securities/columns',
                     lambda data: result_deserializer(data, key=lambda item: item['name']))
                 
                 self._values = client.get_objects(
                     f'{self._path}/{self._name}/boards/{self._boardid}/securities/',
                     lambda data: result_deserializer(data, key=lambda item: item['SECID']))
 
+    def _is_delisted(self, secid: str, cs: Session = None):
+        self._ensure_loaded(cs)
+        if self._delisted is None:
+            market = self._name
+            engine = self._path.split('/')[1]
+            "&group_by=type&group_by_filter=preferred_share&iss.only=securities&securities.columns=secid"
+            with Session(cs or session.default) as client:
+                data = data_gen(cs, f'securities/',
+                                {'engine': engine, 'market': market, 'is_trading': 0,
+                                 'iss.only': 'securities', 'securities.columns': 'secid'},
+                                0, 10000, 'securities')
+                self._delisted = [row['secid'] for row in data]
+        return secid in self._delisted
+
     def _ticker_info(self, secid: str, cs: Session = None) -> dict[str, dict[str, dict]]:
         """
         Возвращает информацию о заданном инструменте.
 
         Parameters
         ----------
         secid : str
@@ -519,16 +535,16 @@
             cs, 
             use_dataframe
         )
 
     def futoi(self, 
               *, 
               date: Union[str, date] = None, 
-              latest: bool = None,
-              offset: int = None,
+              # latest: bool = None,
+              # offset: int = None,
               cs: Session = None, 
               use_dataframe: bool = True) -> Union[iter, pd.DataFrame]:
         """
         Возвращает метрики `FUTOI` по заданным параметрам.
 
         Parameters
         ----------
@@ -557,12 +573,12 @@
         if self._path != 'engines/futures/markets':
             raise NotImplementedError("FUTOI is not implemented for this market")
         
         return self._prepare_metric(
             'FUTOI',
             self._pref,
             date, 
-            latest,
-            offset,
-            cs, 
-            use_dataframe
+            latest=None,
+            offset=None,
+            cs=cs,
+            use_dataframe=use_dataframe
         )
```

### Comparing `moexalgo-2.0.3/moexalgo/metrics.py` & `moexalgo-2.1.0/moexalgo/metrics.py`

 * *Files 9% similar despite different names*

```diff
@@ -223,33 +223,39 @@
 
     offset, limit = clac_offset_limit(offset, limit)
     path = get_metrics_path(metric, secid)
 
     return data_gen(cs, path, options, offset, limit, section='data')
 
 
-def prepare_market_request(metric: str, 
+def prepare_market_request(metric: str,
                            cs: Session, 
                            *, 
                            secid: str = None, 
                            date_: Union[str, date] = None,
+                           start: Union[str, date] = None,
+                           end: Union[str, date] = None,
                            latest: bool = False, 
                            offset: int = None, 
                            limit: int = None) -> iter[dict]:
     """
     Подготовка запроса к API (для рынка).
 
     Parameters
     ----------
     metric : str
         Метрика.
     cs : Session
         Сессия.
     secid : str, optional
         Наименование инструмента, by default None.
+    start : Union[str, date]
+            Дата начала диапазона выдачи данных. (`start` может быть равен `end`, тогда вернутся записи за один день)
+    end : Union[str, date]
+        Дата конца диапазона выдачи данных.
     date_ : Union[str, date], optional
         Дата, by default None.
     latest : bool, optional
         Получить последние данные, by default `False`.
     offset : int, optional
         Смещение, by default None.
     limit : int, optional
@@ -260,21 +266,35 @@
     return : iter[dict]
         Итератор с данными.
     """
 
     date_ = date.today() if (date_ is None) or (date_ == 'today') else date_
     if isinstance(date_, str):
         date_ = date.fromisoformat(date_)
-    
-    options = {'date': date_.isoformat()}
+
+    if isinstance(start, str):
+        start = date.fromisoformat(start)
+
+    if isinstance(end, str):
+        end = date.fromisoformat(end)
+
+    if secid is not None:
+        options = {'from': start.isoformat(), 'till': end.isoformat()}
+    else:
+        options = {'date': date_.isoformat()}
+
     if latest:
         options['latest'] = 1
     
     offset, limit = clac_offset_limit(offset, limit)
-    if metric.lower() == 'fo/futoi':
-        section = 'futoi'
-        path = f'analyticalproducts/futoi/securities'
+    if metric.lower().startswith('fo/futoi'):
+        if len(metric.lower().split("/")) == 3:
+            section = 'futoi'
+            path = f'analyticalproducts/futoi/securities/{metric.lower().split("/")[-1]}'
+        else:
+            section = 'futoi'
+            path = f'analyticalproducts/futoi/securities'
     else:
         section = 'data'
         path = get_metrics_path(metric, secid)
 
     return data_gen(cs, path, options, offset, limit, section=section)
```

### Comparing `moexalgo-2.0.3/moexalgo/models/common.py` & `moexalgo-2.1.0/moexalgo/models/common.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.3/moexalgo/models/indices.py` & `moexalgo-2.1.0/moexalgo/models/indices.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.3/moexalgo/models/metrics.py` & `moexalgo-2.1.0/moexalgo/models/metrics.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.3/moexalgo/models/shares.py` & `moexalgo-2.1.0/moexalgo/models/shares.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.3/moexalgo/session.py` & `moexalgo-2.1.0/moexalgo/session.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.3/moexalgo/stocks.py` & `moexalgo-2.1.0/moexalgo/stocks.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.3/moexalgo/tickers.py` & `moexalgo-2.1.0/moexalgo/tickers.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from datetime import date
 import re
 from typing import Union
 import weakref
 
 from moexalgo.candles import Candle, dataclass_it, prepare_request, pandas_frame
 from moexalgo.market import Market
+from moexalgo.metrics import prepare_market_request
 from moexalgo.session import Session, data_gen
 from moexalgo.utils import pd, CandlePeriod
 
 
 class _Ticker:
     """
     Базовый класс для работы с инструментами.
@@ -65,14 +66,15 @@
         >>> print(orderbook)
     """
 
     _PATH = 'Основная часть пути к API, должна быть определена в суперклассах'
 
     _secid: str
     _boardid: str
+    _delisted: bool
 
     def __new__(cls, secid: str, boardid: str = None) -> _Ticker:
         """
         Создает новый объект инструмента.
 
         Parameters
         ----------
@@ -83,24 +85,26 @@
 
         Returns
         -------
         _Ticker
             Объект инструмента.
         """
         if boardid is None:
-            secid, *args = re.split('\W', secid)
+            secid, *args = re.split('[^a-zA-Z0-9-]', secid)
             if args:
                 boardid = args[0]
         
         market = Market(cls._PATH, boardid)
-        if market._ticker_info(secid):
+        delisted = False if market._ticker_info(secid) else market._is_delisted(secid)
+        if market._ticker_info(secid) or delisted:
             instance = super().__new__(cls)
             instance._secid = secid
             instance._boardid = market._boardid
             instance._r_market = weakref.ref(market)
+            instance._delisted = delisted
             return instance
         raise LookupError(f"Cannot found ticker: ({secid}, {boardid or ''})")
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}('{self._secid}/{self._boardid}')"
 
     @property
@@ -281,7 +285,60 @@
             path=path, 
             options={}, 
             offset=0, 
             limit=-1,
             section='orderbook'
         )
         return pandas_frame(orderbook_it) if use_dataframe else dataclass_it(orderbook_it)
+
+    def futoi(
+            self,
+            *,
+            start: Union[str, date],
+            end: Union[str, date],
+            # latest: bool = None,
+            # offset: int = None,
+            cs: Session = None,
+            use_dataframe: bool = True
+    ) -> Union[iter, pd.DataFrame]:
+        """
+        Возвращает метрики `FUTOI` по заданным параметрам.
+
+        Parameters
+        ----------
+        start : Union[str, date]
+            Дата начала диапазона выдачи данных. (`start` может быть равен `end`, тогда вернутся записи за один день)
+        end : Union[str, date]
+            Дата конца диапазона выдачи данных.
+        latest : bool, optional
+            Включает режим выдачи последних записей в наборе.
+        offset : int, optional
+            Начальная позиция в последовательности записей.
+        cs : Session, optional
+            Клиентская сессия, если используется.
+        use_dataframe : bool, optional
+            Изменяет тип возвращаемого объекта, by default `True`.
+            Если `True`, то возвращает `pd.DataFrame`, иначе итератор.
+
+        Returns
+        -------
+        return : Union[iter, pd.DataFrame]
+            Итератор или `pd.DataFrame` метрик `FUTOI`.
+
+        Raises
+        ------
+        NotImplementedError
+            Вызывается, если `FUTOI` не поддерживается для данного рынка.
+        """
+
+        sectype = self._market._values['securities'][self._secid]['SECTYPE']
+
+        metrics_it = prepare_market_request(
+            f'fo/futoi/{sectype}',
+            cs,
+            secid=self._secid,
+            start=start,
+            end=end,
+            # latest=latest,
+            # offset=offset
+        )
+        return pandas_frame(metrics_it) if use_dataframe else dataclass_it(metrics_it)
```

### Comparing `moexalgo-2.0.3/moexalgo/utils.py` & `moexalgo-2.1.0/moexalgo/utils.py`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.3/moexalgo.egg-info/PKG-INFO` & `moexalgo-2.1.0/moexalgo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moexalgo
-Version: 2.0.3
+Version: 2.1.0
 Summary: Python lib for MOEX AlgoPack data
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Financial and Insurance Industry
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -49,17 +49,19 @@
 
 <br>
 
 ## 🚀 Пример использования
 
 <hr>
 
-#### ⚡️ Быстрое знакомство с библиотекой MoexAlgo - [quick_start.ipynb](https://github.com/moexalgo/moexalgo/blob/main/samples/quick_start.ipynb)
+#### ⚡️ Быстрое знакомство с библиотекой MoexAlgo - [quick_start.ipynb](./samples/quick_start.ipynb)
 
-#### 🔐 Пример авторизации - [auth.ipynb](https://github.com/moexalgo/moexalgo/blob/main/samples/auth.ipynb)
+#### ⬇️ Получение данных через API - [download_algopack_data.ipynb](./samples/download_algopack_data.ipynb)
+
+#### 🔐 Пример авторизации - [auth.ipynb](./samples/auth.ipynb)
 <hr>
 
 Для работы с библиотекой необходимо авторизоваться на https://passport.moex.com
 
 ```python
 from moexalgo import session
```

### Comparing `moexalgo-2.0.3/moexalgo.egg-info/SOURCES.txt` & `moexalgo-2.1.0/moexalgo.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 moexalgo/models/__init__.py
 moexalgo/models/common.py
 moexalgo/models/indices.py
 moexalgo/models/metrics.py
 moexalgo/models/shares.py
 samples/.gitignore
 samples/auth.ipynb
+samples/download_algopack_data.ipynb
 samples/quick_start.ipynb
 tests/.gitignore
 tests/test_currency.py
 tests/test_futures.py
 tests/test_markets.py
 tests/test_stocks.py
 tests/test_tickers.py
```

### Comparing `moexalgo-2.0.3/pyproject.toml` & `moexalgo-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.3/samples/auth.ipynb` & `moexalgo-2.1.0/samples/auth.ipynb`

 * *Files identical despite different names*

### Comparing `moexalgo-2.0.3/tests/test_currency.py` & `moexalgo-2.1.0/tests/test_currency.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,33 +5,36 @@
 import pandas as pd
 
 
 def test_candles_currency():
     cny000000tod = Currency('CNY000000TOD', 'CETS')
     it = cny000000tod.candles(start='2024-04-22', end='2024-04-22', use_dataframe=False)
     assert isinstance(next(it), object)
-    
+    assert next(it)
+
 
     it = cny000000tod.candles(start='2024-04-22', end='2024-04-22', use_dataframe=True)
     assert isinstance(it, pd.DataFrame)
 
     it = cny000000tod.tradestats(start='2024-04-22', end='2024-04-22', use_dataframe=False)
     assert isinstance(next(it), object)
-    
+    assert next(it)
+
 
 
 def test_currency_ticker():
     cny000000tod = Ticker('CNY000000TOD')
     it = cny000000tod.candles(start='2024-04-22', end='2024-04-22', use_dataframe=False)
     assert isinstance(next(it), object)
     
 
     it = cny000000tod.tradestats(start='2024-04-22', end='2024-04-22', use_dataframe=False)
     assert isinstance(next(it), object)
-    
+    assert next(it)
+
 
 
 def test_currency_tradestats():
     cny000000tod = Currency('CNY000000TOD', 'CETS')
     cny000000tod.tradestats(start=date(2024, 4, 22),  end='2024-04-22')
     cny000000tod.tradestats(start=date(2024, 4, 22), end=date(2024, 4, 22))
     cny000000tod.tradestats(start='2024-04-22', end='2024-04-22')
```

### Comparing `moexalgo-2.0.3/tests/test_futures.py` & `moexalgo-2.1.0/tests/test_futures.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,39 @@
 import pandas as pd
 
 
 def test_candles_futures():
     AKM4 = Futures('AKM4', 'RFUD')
     it = AKM4.candles(start='2024-04-22', end='2024-04-22', use_dataframe=False)
     assert isinstance(next(it), object)
-    
+    assert next(it)
+
 
     it = AKM4.candles(start='2024-04-22', end='2024-04-22', use_dataframe=True)
     assert isinstance(it, pd.DataFrame)
 
     it = AKM4.tradestats(start='2024-04-22', end='2024-04-22', use_dataframe=False)
     assert isinstance(next(it), object)
-    
+    assert next(it)
+
 
 
 def test_futures_ticker():
     AKM4 = Ticker('AKM4')
     it = AKM4.candles(start='2024-04-22', end='2024-04-22', use_dataframe=False)
     assert isinstance(next(it), object)
-    
+    assert next(it)
+
+
+
+def test_delisted_shares():
+    RIZ2 = Futures('RIZ2', 'RFUD')
+    it = RIZ2.tradestats(start='2022-08-02', end='2022-08-02', use_dataframe=False)
+    assert next(it)
+    assert next(it)
 
 
 def test_futures_tradestats():
     AKM4 = Futures('AKM4', 'RFUD')
     AKM4.tradestats(start=date(2024, 4, 22),  end='2024-04-22')
     AKM4.tradestats(start=date(2024, 4, 22), end=date(2024, 4, 22))
     AKM4.tradestats(start='2024-04-22', end='2024-04-22')
@@ -53,7 +63,18 @@
     AKM4.hi2(start=date(2024, 4, 22),  end='2024-04-22')
     AKM4.hi2(start=date(2024, 4, 22), end=date(2024, 4, 22))
     AKM4.hi2(start='2024-04-22', end='2024-04-22')
     with pytest.raises(Exception):
         AKM4.hi2(start='2024-04-23', end='2024-04-22')
     with pytest.raises(Exception):
         AKM4.hi2(start=None, end=None)
+
+
+def test_futures_futoi():
+    AKM4 = Futures('AKM4', 'RFUD')
+    AKM4.futoi(start=date(2024, 4, 22),  end='2024-04-22')
+    AKM4.futoi(start=date(2024, 4, 22), end=date(2024, 4, 22))
+    AKM4.futoi(start='2024-04-22', end='2024-04-22')
+    # with pytest.raises(Exception):
+    #     AKM4.futoi(start='2024-04-23', end='2024-04-22')
+    with pytest.raises(Exception):
+        AKM4.futoi(start=None, end=None)
```

### Comparing `moexalgo-2.0.3/tests/test_markets.py` & `moexalgo-2.1.0/tests/test_markets.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,51 +6,55 @@
     eq = Market('EQ')
     assert eq == Market('EQ')
     assert eq == Market('shares')
     assert eq == Market('shares', 'TQBR')
 
     it = eq.tradestats(date="2024-01-10", use_dataframe=False)
     assert isinstance(next(it), object)
-    
+    assert next(it)
+
 
     index = Market('index')
     assert index != eq
     assert index == Market('index', 'SNDX')
 
 
 def test_market_eq():
     eq = Market('shares')
     assert eq._pref == 'eq'
     it = eq.tradestats(date="2024-01-10", use_dataframe=False)
     assert isinstance(next(it), object)
-    
+    assert next(it)
+
 
 
 def test_market_fx():
     fx = Market('currency')
     assert fx._pref == 'fx'
     it = fx.tradestats(date="2024-04-22", use_dataframe=False)
     assert isinstance(next(it), object)
-    
+    assert next(it)
+
 
 
 def test_market_fo():
     fo = Market('futures')
     assert fo._pref == 'fo'
     it = fo.tradestats(date="2024-04-22", use_dataframe=False)
     assert isinstance(next(it), object)
-    
+    assert next(it)
 
 
 def test_futoi():
     fo = Market('FO')
     it = fo.tradestats(date='2024-04-22', use_dataframe=False)
     assert isinstance(next(it), object)
-    
+    assert next(it)
+
 
     it = fo.futoi(date='2024-04-08', use_dataframe=False)
     assert isinstance(next(it), object)
-    
+    assert next(it)
 
 
 if __name__ == '__main__':
     pytest.main()
```

### Comparing `moexalgo-2.0.3/tests/test_stocks.py` & `moexalgo-2.1.0/tests/test_stocks.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,42 +5,52 @@
 import pandas as pd
 
 
 def test_candles_shares():
     ABIO = Stock('ABIO', 'TQBR')
     it = ABIO.candles(start='2024-04-22', end='2024-04-22', use_dataframe=False)
     assert isinstance(next(it), object)
+    assert next(it)
     
 
     it = ABIO.candles(start='2024-04-22', end='2024-04-22', use_dataframe=True)
     assert isinstance(it, pd.DataFrame)
 
     it = ABIO.tradestats(start='2024-04-22', end='2024-04-22', use_dataframe=False)
     assert isinstance(next(it), object)
-    
+    assert next(it)
+
 
 
 def test_shares_ticker():
     ABIO = Ticker('ABIO')
     it = ABIO.candles(start='2024-04-22', end='2024-04-22', use_dataframe=False)
     assert isinstance(next(it), object)
-    
+    assert next(it)
+
 
 
 def test_shares_tradestats():
     ABIO = Stock('ABIO', 'TQBR')
     ABIO.tradestats(start=date(2024, 4, 22),  end='2024-04-22')
     ABIO.tradestats(start=date(2024, 4, 22), end=date(2024, 4, 22))
     ABIO.tradestats(start='2024-04-22', end='2024-04-22')
     with pytest.raises(Exception):
         ABIO.tradestats(start='2024-04-23', end='2024-04-22')
     with pytest.raises(Exception):
         ABIO.tradestats(start=None, end=None)
 
 
+def test_delisted_shares():
+    MFON = Stock('MORI', 'TQBR')
+    it = MFON.obstats(start='2022-04-07', end='2022-04-07', use_dataframe=False)
+    assert next(it)
+    assert next(it)
+
+
 def test_shares_orderstats():
     ABIO = Stock('ABIO', 'TQBR')
     ABIO.orderstats(start=date(2024, 4, 22),  end='2024-04-22')
     ABIO.orderstats(start=date(2024, 4, 22), end=date(2024, 4, 22))
     ABIO.orderstats(start='2024-04-22', end='2024-04-22')
     with pytest.raises(Exception):
         ABIO.orderstats(start='2024-04-23', end='2024-04-22')
```

### Comparing `moexalgo-2.0.3/tests/test_tickers.py` & `moexalgo-2.1.0/tests/test_tickers.py`

 * *Files identical despite different names*

