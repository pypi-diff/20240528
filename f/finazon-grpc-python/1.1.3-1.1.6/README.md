# Comparing `tmp/finazon_grpc_python-1.1.3.tar.gz` & `tmp/finazon_grpc_python-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finazon_grpc_python-1.1.3.tar", max compression
+gzip compressed data, was "finazon_grpc_python-1.1.6.tar", max compression
```

## Comparing `finazon_grpc_python-1.1.3.tar` & `finazon_grpc_python-1.1.6.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     1064 2024-04-16 10:03:58.625999 finazon_grpc_python-1.1.3/LICENSE.txt
--rw-r--r--   0        0        0    13306 2024-04-16 10:03:58.906004 finazon_grpc_python-1.1.3/README.md
--rw-r--r--   0        0        0        0 2024-04-16 10:03:58.625999 finazon_grpc_python-1.1.3/finazon_grpc_python/__init__.py
--rw-r--r--   0        0        0     2030 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/api_usage_pb2.py
--rw-r--r--   0        0        0     2776 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/api_usage_pb2.pyi
--rw-r--r--   0        0        0     2715 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/api_usage_pb2_grpc.py
--rw-r--r--   0        0        0      504 2024-04-16 10:04:20.574384 finazon_grpc_python-1.1.3/finazon_grpc_python/api_usage_service.py
--rw-r--r--   0        0        0     9732 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/benzinga_pb2.py
--rw-r--r--   0        0        0    26705 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/benzinga_pb2.pyi
--rw-r--r--   0        0        0     7871 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/benzinga_pb2_grpc.py
--rw-r--r--   0        0        0     1175 2024-04-16 10:04:20.630385 finazon_grpc_python-1.1.3/finazon_grpc_python/benzinga_service.py
--rw-r--r--   0        0        0     2485 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/binance_pb2.py
--rw-r--r--   0        0        0     3890 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/binance_pb2.pyi
--rw-r--r--   0        0        0     2769 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/binance_pb2_grpc.py
--rw-r--r--   0        0        0      537 2024-04-16 10:04:20.638385 finazon_grpc_python-1.1.3/finazon_grpc_python/binance_service.py
--rw-r--r--   0        0        0        0 2024-04-16 10:03:58.629999 finazon_grpc_python-1.1.3/finazon_grpc_python/common/__init__.py
--rw-r--r--   0        0        0     1786 2024-04-16 10:03:58.629999 finazon_grpc_python-1.1.3/finazon_grpc_python/common/client.py
--rw-r--r--   0        0        0      496 2024-04-16 10:03:58.629999 finazon_grpc_python-1.1.3/finazon_grpc_python/common/errors.py
--rw-r--r--   0        0        0      177 2024-04-16 10:03:58.926005 finazon_grpc_python-1.1.3/finazon_grpc_python/common/settings.py
--rw-r--r--   0        0        0     1966 2024-04-16 10:03:58.629999 finazon_grpc_python-1.1.3/finazon_grpc_python/common/utils.py
--rw-r--r--   0        0        0     2254 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/crypto_pb2.py
--rw-r--r--   0        0        0     3113 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/crypto_pb2.pyi
--rw-r--r--   0        0        0     2737 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/crypto_pb2_grpc.py
--rw-r--r--   0        0        0      528 2024-04-16 10:04:20.750387 finazon_grpc_python-1.1.3/finazon_grpc_python/crypto_service.py
--rw-r--r--   0        0        0     1820 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/datasets_pb2.py
--rw-r--r--   0        0        0     2040 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/datasets_pb2.pyi
--rw-r--r--   0        0        0     2718 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/datasets_pb2_grpc.py
--rw-r--r--   0        0        0      501 2024-04-16 10:04:20.826389 finazon_grpc_python-1.1.3/finazon_grpc_python/datasets_service.py
--rw-r--r--   0        0        0        0 2024-04-16 10:03:58.629999 finazon_grpc_python-1.1.3/finazon_grpc_python/examples/__init__.py
--rw-r--r--   0        0        0      627 2024-04-16 10:03:58.629999 finazon_grpc_python-1.1.3/finazon_grpc_python/examples/indicator_atr.py
--rw-r--r--   0        0        0      598 2024-04-16 10:03:58.629999 finazon_grpc_python-1.1.3/finazon_grpc_python/examples/indicator_ma.py
--rw-r--r--   0        0        0      689 2024-04-16 10:03:58.629999 finazon_grpc_python-1.1.3/finazon_grpc_python/examples/indicator_ma_pandas.py
--rw-r--r--   0        0        0      489 2024-04-16 10:03:58.629999 finazon_grpc_python-1.1.3/finazon_grpc_python/examples/tickers.py
--rw-r--r--   0        0        0      635 2024-04-16 10:03:58.629999 finazon_grpc_python-1.1.3/finazon_grpc_python/examples/time_series.py
--rw-r--r--   0        0        0      619 2024-04-16 10:03:58.629999 finazon_grpc_python-1.1.3/finazon_grpc_python/examples/time_series_pandas.py
--rw-r--r--   0        0        0     2823 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/exchange_pb2.py
--rw-r--r--   0        0        0     4268 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/exchange_pb2.pyi
--rw-r--r--   0        0        0     4553 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/exchange_pb2_grpc.py
--rw-r--r--   0        0        0      771 2024-04-16 10:04:20.602385 finazon_grpc_python-1.1.3/finazon_grpc_python/exchange_service.py
--rw-r--r--   0        0        0     2210 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/forex_pb2.py
--rw-r--r--   0        0        0     2978 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/forex_pb2.pyi
--rw-r--r--   0        0        0     2713 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/forex_pb2_grpc.py
--rw-r--r--   0        0        0      519 2024-04-16 10:04:20.770388 finazon_grpc_python-1.1.3/finazon_grpc_python/forex_service.py
--rw-r--r--   0        0        0     1838 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/publishers_pb2.py
--rw-r--r--   0        0        0     2062 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/publishers_pb2.pyi
--rw-r--r--   0        0        0     2778 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/publishers_pb2_grpc.py
--rw-r--r--   0        0        0      520 2024-04-16 10:04:20.814388 finazon_grpc_python-1.1.3/finazon_grpc_python/publishers_service.py
--rw-r--r--   0        0        0     2667 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/sec_pb2.py
--rw-r--r--   0        0        0     5038 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/sec_pb2.pyi
--rw-r--r--   0        0        0     2711 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/sec_pb2_grpc.py
--rw-r--r--   0        0        0      486 2024-04-16 10:04:20.650385 finazon_grpc_python-1.1.3/finazon_grpc_python/sec_service.py
--rw-r--r--   0        0        0     3205 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/sip_pb2.py
--rw-r--r--   0        0        0     5780 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/sip_pb2.pyi
--rw-r--r--   0        0        0     4372 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/sip_pb2_grpc.py
--rw-r--r--   0        0        0      716 2024-04-16 10:04:20.586384 finazon_grpc_python-1.1.3/finazon_grpc_python/sip_service.py
--rw-r--r--   0        0        0     3662 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/snapshot_pb2.py
--rw-r--r--   0        0        0     7564 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/snapshot_pb2.pyi
--rw-r--r--   0        0        0     2822 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/snapshot_pb2_grpc.py
--rw-r--r--   0        0        0      501 2024-04-16 10:04:20.762388 finazon_grpc_python-1.1.3/finazon_grpc_python/snapshot_service.py
--rw-r--r--   0        0        0     5474 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/tickers_pb2.py
--rw-r--r--   0        0        0    11601 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/tickers_pb2.pyi
--rw-r--r--   0        0        0     8236 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/tickers_pb2_grpc.py
--rw-r--r--   0        0        0     1235 2024-04-16 10:04:20.798388 finazon_grpc_python-1.1.3/finazon_grpc_python/tickers_service.py
--rw-r--r--   0        0        0    11805 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/time_series_pb2.py
--rw-r--r--   0        0        0    27027 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/time_series_pb2.pyi
--rw-r--r--   0        0        0    19109 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/time_series_pb2_grpc.py
--rw-r--r--   0        0        0     2765 2024-04-16 10:04:20.742387 finazon_grpc_python-1.1.3/finazon_grpc_python/time_series_service.py
--rw-r--r--   0        0        0     2415 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/trade_pb2.py
--rw-r--r--   0        0        0     4127 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/trade_pb2.pyi
--rw-r--r--   0        0        0     2630 2024-04-16 10:04:21.018392 finazon_grpc_python-1.1.3/finazon_grpc_python/trade_pb2_grpc.py
--rw-r--r--   0        0        0      474 2024-04-16 10:04:20.806388 finazon_grpc_python-1.1.3/finazon_grpc_python/trade_service.py
--rw-r--r--   0        0        0      813 2024-04-16 10:03:58.926005 finazon_grpc_python-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      443 2024-04-16 10:03:58.629999 finazon_grpc_python-1.1.3/requirements.txt
--rw-r--r--   0        0        0    14198 1970-01-01 00:00:00.000000 finazon_grpc_python-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-28 08:52:41.670222 finazon_grpc_python-1.1.6/LICENSE.txt
+-rw-r--r--   0        0        0    13306 2024-05-28 08:52:41.922226 finazon_grpc_python-1.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 08:52:41.670222 finazon_grpc_python-1.1.6/finazon_grpc_python/__init__.py
+-rw-r--r--   0        0        0     2030 2024-05-28 08:53:04.590631 finazon_grpc_python-1.1.6/finazon_grpc_python/api_usage_pb2.py
+-rw-r--r--   0        0        0     2776 2024-05-28 08:53:04.590631 finazon_grpc_python-1.1.6/finazon_grpc_python/api_usage_pb2.pyi
+-rw-r--r--   0        0        0     2715 2024-05-28 08:53:04.590631 finazon_grpc_python-1.1.6/finazon_grpc_python/api_usage_pb2_grpc.py
+-rw-r--r--   0        0        0      504 2024-05-28 08:53:04.134623 finazon_grpc_python-1.1.6/finazon_grpc_python/api_usage_service.py
+-rw-r--r--   0        0        0     9732 2024-05-28 08:53:04.590631 finazon_grpc_python-1.1.6/finazon_grpc_python/benzinga_pb2.py
+-rw-r--r--   0        0        0    26705 2024-05-28 08:53:04.590631 finazon_grpc_python-1.1.6/finazon_grpc_python/benzinga_pb2.pyi
+-rw-r--r--   0        0        0     7871 2024-05-28 08:53:04.590631 finazon_grpc_python-1.1.6/finazon_grpc_python/benzinga_pb2_grpc.py
+-rw-r--r--   0        0        0     1175 2024-05-28 08:53:04.190624 finazon_grpc_python-1.1.6/finazon_grpc_python/benzinga_service.py
+-rw-r--r--   0        0        0     2485 2024-05-28 08:53:04.590631 finazon_grpc_python-1.1.6/finazon_grpc_python/binance_pb2.py
+-rw-r--r--   0        0        0     3890 2024-05-28 08:53:04.590631 finazon_grpc_python-1.1.6/finazon_grpc_python/binance_pb2.pyi
+-rw-r--r--   0        0        0     2769 2024-05-28 08:53:04.594631 finazon_grpc_python-1.1.6/finazon_grpc_python/binance_pb2_grpc.py
+-rw-r--r--   0        0        0      537 2024-05-28 08:53:04.198624 finazon_grpc_python-1.1.6/finazon_grpc_python/binance_service.py
+-rw-r--r--   0        0        0        0 2024-05-28 08:52:41.670222 finazon_grpc_python-1.1.6/finazon_grpc_python/common/__init__.py
+-rw-r--r--   0        0        0     1786 2024-05-28 08:52:41.670222 finazon_grpc_python-1.1.6/finazon_grpc_python/common/client.py
+-rw-r--r--   0        0        0      496 2024-05-28 08:52:41.670222 finazon_grpc_python-1.1.6/finazon_grpc_python/common/errors.py
+-rw-r--r--   0        0        0      177 2024-05-28 08:52:41.946227 finazon_grpc_python-1.1.6/finazon_grpc_python/common/settings.py
+-rw-r--r--   0        0        0     1966 2024-05-28 08:52:41.670222 finazon_grpc_python-1.1.6/finazon_grpc_python/common/utils.py
+-rw-r--r--   0        0        0     2254 2024-05-28 08:53:04.594631 finazon_grpc_python-1.1.6/finazon_grpc_python/crypto_pb2.py
+-rw-r--r--   0        0        0     3113 2024-05-28 08:53:04.594631 finazon_grpc_python-1.1.6/finazon_grpc_python/crypto_pb2.pyi
+-rw-r--r--   0        0        0     2737 2024-05-28 08:53:04.594631 finazon_grpc_python-1.1.6/finazon_grpc_python/crypto_pb2_grpc.py
+-rw-r--r--   0        0        0      528 2024-05-28 08:53:04.306626 finazon_grpc_python-1.1.6/finazon_grpc_python/crypto_service.py
+-rw-r--r--   0        0        0     1820 2024-05-28 08:53:04.594631 finazon_grpc_python-1.1.6/finazon_grpc_python/datasets_pb2.py
+-rw-r--r--   0        0        0     2040 2024-05-28 08:53:04.594631 finazon_grpc_python-1.1.6/finazon_grpc_python/datasets_pb2.pyi
+-rw-r--r--   0        0        0     2718 2024-05-28 08:53:04.594631 finazon_grpc_python-1.1.6/finazon_grpc_python/datasets_pb2_grpc.py
+-rw-r--r--   0        0        0      501 2024-05-28 08:53:04.378627 finazon_grpc_python-1.1.6/finazon_grpc_python/datasets_service.py
+-rw-r--r--   0        0        0        0 2024-05-28 08:52:41.670222 finazon_grpc_python-1.1.6/finazon_grpc_python/examples/__init__.py
+-rw-r--r--   0        0        0      627 2024-05-28 08:52:41.670222 finazon_grpc_python-1.1.6/finazon_grpc_python/examples/indicator_atr.py
+-rw-r--r--   0        0        0      598 2024-05-28 08:52:41.670222 finazon_grpc_python-1.1.6/finazon_grpc_python/examples/indicator_ma.py
+-rw-r--r--   0        0        0      689 2024-05-28 08:52:41.670222 finazon_grpc_python-1.1.6/finazon_grpc_python/examples/indicator_ma_pandas.py
+-rw-r--r--   0        0        0      489 2024-05-28 08:52:41.670222 finazon_grpc_python-1.1.6/finazon_grpc_python/examples/tickers.py
+-rw-r--r--   0        0        0      635 2024-05-28 08:52:41.670222 finazon_grpc_python-1.1.6/finazon_grpc_python/examples/time_series.py
+-rw-r--r--   0        0        0      619 2024-05-28 08:52:41.670222 finazon_grpc_python-1.1.6/finazon_grpc_python/examples/time_series_pandas.py
+-rw-r--r--   0        0        0     2823 2024-05-28 08:53:04.594631 finazon_grpc_python-1.1.6/finazon_grpc_python/exchange_pb2.py
+-rw-r--r--   0        0        0     4268 2024-05-28 08:53:04.594631 finazon_grpc_python-1.1.6/finazon_grpc_python/exchange_pb2.pyi
+-rw-r--r--   0        0        0     4553 2024-05-28 08:53:04.594631 finazon_grpc_python-1.1.6/finazon_grpc_python/exchange_pb2_grpc.py
+-rw-r--r--   0        0        0      771 2024-05-28 08:53:04.162624 finazon_grpc_python-1.1.6/finazon_grpc_python/exchange_service.py
+-rw-r--r--   0        0        0     2210 2024-05-28 08:53:04.594631 finazon_grpc_python-1.1.6/finazon_grpc_python/forex_pb2.py
+-rw-r--r--   0        0        0     2978 2024-05-28 08:53:04.594631 finazon_grpc_python-1.1.6/finazon_grpc_python/forex_pb2.pyi
+-rw-r--r--   0        0        0     2713 2024-05-28 08:53:04.594631 finazon_grpc_python-1.1.6/finazon_grpc_python/forex_pb2_grpc.py
+-rw-r--r--   0        0        0      519 2024-05-28 08:53:04.326626 finazon_grpc_python-1.1.6/finazon_grpc_python/forex_service.py
+-rw-r--r--   0        0        0     1838 2024-05-28 08:53:04.594631 finazon_grpc_python-1.1.6/finazon_grpc_python/publishers_pb2.py
+-rw-r--r--   0        0        0     2062 2024-05-28 08:53:04.594631 finazon_grpc_python-1.1.6/finazon_grpc_python/publishers_pb2.pyi
+-rw-r--r--   0        0        0     2778 2024-05-28 08:53:04.594631 finazon_grpc_python-1.1.6/finazon_grpc_python/publishers_pb2_grpc.py
+-rw-r--r--   0        0        0      520 2024-05-28 08:53:04.370627 finazon_grpc_python-1.1.6/finazon_grpc_python/publishers_service.py
+-rw-r--r--   0        0        0     2667 2024-05-28 08:53:04.594631 finazon_grpc_python-1.1.6/finazon_grpc_python/sec_pb2.py
+-rw-r--r--   0        0        0     5038 2024-05-28 08:53:04.598631 finazon_grpc_python-1.1.6/finazon_grpc_python/sec_pb2.pyi
+-rw-r--r--   0        0        0     2711 2024-05-28 08:53:04.598631 finazon_grpc_python-1.1.6/finazon_grpc_python/sec_pb2_grpc.py
+-rw-r--r--   0        0        0      486 2024-05-28 08:53:04.210624 finazon_grpc_python-1.1.6/finazon_grpc_python/sec_service.py
+-rw-r--r--   0        0        0     3205 2024-05-28 08:53:04.598631 finazon_grpc_python-1.1.6/finazon_grpc_python/sip_pb2.py
+-rw-r--r--   0        0        0     5780 2024-05-28 08:53:04.598631 finazon_grpc_python-1.1.6/finazon_grpc_python/sip_pb2.pyi
+-rw-r--r--   0        0        0     4372 2024-05-28 08:53:04.598631 finazon_grpc_python-1.1.6/finazon_grpc_python/sip_pb2_grpc.py
+-rw-r--r--   0        0        0      716 2024-05-28 08:53:04.150623 finazon_grpc_python-1.1.6/finazon_grpc_python/sip_service.py
+-rw-r--r--   0        0        0     3662 2024-05-28 08:53:04.606631 finazon_grpc_python-1.1.6/finazon_grpc_python/snapshot_pb2.py
+-rw-r--r--   0        0        0     7564 2024-05-28 08:53:04.606631 finazon_grpc_python-1.1.6/finazon_grpc_python/snapshot_pb2.pyi
+-rw-r--r--   0        0        0     2822 2024-05-28 08:53:04.610631 finazon_grpc_python-1.1.6/finazon_grpc_python/snapshot_pb2_grpc.py
+-rw-r--r--   0        0        0      501 2024-05-28 08:53:04.314626 finazon_grpc_python-1.1.6/finazon_grpc_python/snapshot_service.py
+-rw-r--r--   0        0        0     5474 2024-05-28 08:53:04.610631 finazon_grpc_python-1.1.6/finazon_grpc_python/tickers_pb2.py
+-rw-r--r--   0        0        0    11601 2024-05-28 08:53:04.610631 finazon_grpc_python-1.1.6/finazon_grpc_python/tickers_pb2.pyi
+-rw-r--r--   0        0        0     8236 2024-05-28 08:53:04.610631 finazon_grpc_python-1.1.6/finazon_grpc_python/tickers_pb2_grpc.py
+-rw-r--r--   0        0        0     1235 2024-05-28 08:53:04.350627 finazon_grpc_python-1.1.6/finazon_grpc_python/tickers_service.py
+-rw-r--r--   0        0        0    11805 2024-05-28 08:53:04.610631 finazon_grpc_python-1.1.6/finazon_grpc_python/time_series_pb2.py
+-rw-r--r--   0        0        0    27027 2024-05-28 08:53:04.610631 finazon_grpc_python-1.1.6/finazon_grpc_python/time_series_pb2.pyi
+-rw-r--r--   0        0        0    19109 2024-05-28 08:53:04.610631 finazon_grpc_python-1.1.6/finazon_grpc_python/time_series_pb2_grpc.py
+-rw-r--r--   0        0        0     2765 2024-05-28 08:53:04.298626 finazon_grpc_python-1.1.6/finazon_grpc_python/time_series_service.py
+-rw-r--r--   0        0        0     2415 2024-05-28 08:53:04.610631 finazon_grpc_python-1.1.6/finazon_grpc_python/trade_pb2.py
+-rw-r--r--   0        0        0     4127 2024-05-28 08:53:04.610631 finazon_grpc_python-1.1.6/finazon_grpc_python/trade_pb2.pyi
+-rw-r--r--   0        0        0     2630 2024-05-28 08:53:04.610631 finazon_grpc_python-1.1.6/finazon_grpc_python/trade_pb2_grpc.py
+-rw-r--r--   0        0        0      474 2024-05-28 08:53:04.358627 finazon_grpc_python-1.1.6/finazon_grpc_python/trade_service.py
+-rw-r--r--   0        0        0      813 2024-05-28 08:52:41.942227 finazon_grpc_python-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0      443 2024-05-28 08:52:41.674222 finazon_grpc_python-1.1.6/requirements.txt
+-rw-r--r--   0        0        0    14198 1970-01-01 00:00:00.000000 finazon_grpc_python-1.1.6/PKG-INFO
```

### Comparing `finazon_grpc_python-1.1.3/LICENSE.txt` & `finazon_grpc_python-1.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/README.md` & `finazon_grpc_python-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/api_usage_pb2.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/api_usage_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/api_usage_pb2.pyi` & `finazon_grpc_python-1.1.6/finazon_grpc_python/api_usage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/api_usage_pb2_grpc.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/api_usage_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/benzinga_pb2.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/benzinga_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/benzinga_pb2.pyi` & `finazon_grpc_python-1.1.6/finazon_grpc_python/benzinga_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/benzinga_pb2_grpc.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/benzinga_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/benzinga_service.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/benzinga_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/binance_pb2.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/binance_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/binance_pb2.pyi` & `finazon_grpc_python-1.1.6/finazon_grpc_python/binance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/binance_pb2_grpc.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/binance_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/binance_service.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/binance_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/common/client.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/common/client.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/common/utils.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/common/utils.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/crypto_pb2.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/crypto_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/crypto_pb2.pyi` & `finazon_grpc_python-1.1.6/finazon_grpc_python/crypto_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/crypto_pb2_grpc.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/crypto_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/crypto_service.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/crypto_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/datasets_pb2.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/datasets_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/datasets_pb2.pyi` & `finazon_grpc_python-1.1.6/finazon_grpc_python/datasets_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/datasets_pb2_grpc.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/datasets_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/examples/indicator_atr.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/examples/indicator_atr.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/examples/indicator_ma.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/examples/indicator_ma.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/examples/indicator_ma_pandas.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/examples/indicator_ma_pandas.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/examples/time_series.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/examples/time_series.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/examples/time_series_pandas.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/examples/time_series_pandas.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/exchange_pb2.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/exchange_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/exchange_pb2.pyi` & `finazon_grpc_python-1.1.6/finazon_grpc_python/exchange_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/exchange_pb2_grpc.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/exchange_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/exchange_service.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/exchange_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/forex_pb2.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/forex_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/forex_pb2.pyi` & `finazon_grpc_python-1.1.6/finazon_grpc_python/forex_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/forex_pb2_grpc.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/forex_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/forex_service.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/forex_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/publishers_pb2.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/publishers_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/publishers_pb2.pyi` & `finazon_grpc_python-1.1.6/finazon_grpc_python/publishers_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/publishers_pb2_grpc.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/publishers_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/publishers_service.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/publishers_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/sec_pb2.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/sec_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/sec_pb2.pyi` & `finazon_grpc_python-1.1.6/finazon_grpc_python/sec_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/sec_pb2_grpc.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/sec_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/sip_pb2.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/sip_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/sip_pb2.pyi` & `finazon_grpc_python-1.1.6/finazon_grpc_python/sip_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/sip_pb2_grpc.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/sip_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/sip_service.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/sip_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/snapshot_pb2.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/snapshot_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/snapshot_pb2.pyi` & `finazon_grpc_python-1.1.6/finazon_grpc_python/snapshot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/snapshot_pb2_grpc.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/snapshot_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/tickers_pb2.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/tickers_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/tickers_pb2.pyi` & `finazon_grpc_python-1.1.6/finazon_grpc_python/tickers_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/tickers_pb2_grpc.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/tickers_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/tickers_service.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/tickers_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/time_series_pb2.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/time_series_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/time_series_pb2.pyi` & `finazon_grpc_python-1.1.6/finazon_grpc_python/time_series_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/time_series_pb2_grpc.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/time_series_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/time_series_service.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/time_series_service.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/trade_pb2.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/trade_pb2.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/trade_pb2.pyi` & `finazon_grpc_python-1.1.6/finazon_grpc_python/trade_pb2.pyi`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/finazon_grpc_python/trade_pb2_grpc.py` & `finazon_grpc_python-1.1.6/finazon_grpc_python/trade_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `finazon_grpc_python-1.1.3/pyproject.toml` & `finazon_grpc_python-1.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "finazon-grpc-python"
 packages = [{include = "finazon_grpc_python"}]
 include = ["requirements.txt", "finazon_grpc_python/*.p*"]
-version = "1.1.3"
+version = "1.1.6"
 description = "Finazon gRPC client library for Python"
 authors = ["Finazon <team@finazon.io>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/finazon-io/finazon-grpc-python"
 repository = "https://github.com/finazon-io/finazon-grpc-python"
```

### Comparing `finazon_grpc_python-1.1.3/PKG-INFO` & `finazon_grpc_python-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finazon-grpc-python
-Version: 1.1.3
+Version: 1.1.6
 Summary: Finazon gRPC client library for Python
 Home-page: https://github.com/finazon-io/finazon-grpc-python
 License: MIT
 Author: Finazon
 Author-email: team@finazon.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

