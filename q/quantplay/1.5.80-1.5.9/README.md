# Comparing `tmp/quantplay-1.5.80.tar.gz` & `tmp/quantplay-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantplay-1.5.80.tar", last modified: Tue May 28 07:45:08 2024, max compression
+gzip compressed data, was "quantplay-1.5.9.tar", last modified: Fri Mar 15 04:41:41 2024, max compression
```

## Comparing `quantplay-1.5.80.tar` & `quantplay-1.5.9.tar`

### file list

```diff
@@ -1,155 +1,160 @@
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.170854 quantplay-1.5.80/
--rw-r--r--   0 ashok      (502) staff       (20)      663 2024-05-28 07:45:08.170928 quantplay-1.5.80/PKG-INFO
--rw-r--r--   0 ashok      (502) staff       (20)      494 2023-04-19 06:36:45.000000 quantplay-1.5.80/README.md
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.146115 quantplay-1.5.80/quantplay/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.147032 quantplay-1.5.80/quantplay/backtest/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/backtest/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    17974 2024-01-30 12:40:34.000000 quantplay-1.5.80/quantplay/backtest/backtest_trades.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.152709 quantplay-1.5.80/quantplay/broker/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/broker/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    15481 2024-05-28 07:44:59.000000 quantplay-1.5.80/quantplay/broker/aliceblue.py
--rw-r--r--   0 ashok      (502) staff       (20)    17909 2024-05-20 11:54:09.000000 quantplay-1.5.80/quantplay/broker/angelone.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.153183 quantplay-1.5.80/quantplay/broker/auto_login/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2024-05-17 05:47:14.000000 quantplay-1.5.80/quantplay/broker/auto_login/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     3364 2024-05-28 07:44:13.000000 quantplay-1.5.80/quantplay/broker/auto_login/aliceblue.py
--rw-r--r--   0 ashok      (502) staff       (20)     3738 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/broker/broker_client.py
--rw-r--r--   0 ashok      (502) staff       (20)       87 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/broker/client.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.153523 quantplay-1.5.80/quantplay/broker/finvasia_utils/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/broker/finvasia_utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    32131 2024-03-14 05:08:38.000000 quantplay-1.5.80/quantplay/broker/finvasia_utils/fa_noren.py
--rw-r--r--   0 ashok      (502) staff       (20)    15714 2024-05-23 15:10:02.000000 quantplay-1.5.80/quantplay/broker/five_paisa.py
--rw-r--r--   0 ashok      (502) staff       (20)     2717 2024-03-06 12:51:21.000000 quantplay-1.5.80/quantplay/broker/flattrade.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.154348 quantplay-1.5.80/quantplay/broker/ft_utils/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-06 12:37:31.000000 quantplay-1.5.80/quantplay/broker/ft_utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2247 2024-01-23 17:16:24.000000 quantplay-1.5.80/quantplay/broker/ft_utils/flattrade_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)    32131 2024-03-14 05:08:42.000000 quantplay-1.5.80/quantplay/broker/ft_utils/ft_noren.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.154861 quantplay-1.5.80/quantplay/broker/generics/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/broker/generics/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    44858 2024-05-28 05:18:48.000000 quantplay-1.5.80/quantplay/broker/generics/broker.py
--rw-r--r--   0 ashok      (502) staff       (20)     3936 2024-04-23 14:23:38.000000 quantplay-1.5.80/quantplay/broker/icici.py
--rw-r--r--   0 ashok      (502) staff       (20)     3897 2023-05-17 07:17:28.000000 quantplay-1.5.80/quantplay/broker/iifl.py
--rw-r--r--   0 ashok      (502) staff       (20)      750 2024-03-14 07:46:45.000000 quantplay-1.5.80/quantplay/broker/iifl_xts.py
--rw-r--r--   0 ashok      (502) staff       (20)     3862 2024-03-09 04:22:31.000000 quantplay-1.5.80/quantplay/broker/kite_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)    27502 2024-05-22 11:40:12.000000 quantplay-1.5.80/quantplay/broker/motilal.py
--rw-r--r--   0 ashok      (502) staff       (20)    23296 2024-05-28 05:18:55.000000 quantplay-1.5.80/quantplay/broker/noren.py
--rw-r--r--   0 ashok      (502) staff       (20)     2515 2024-03-06 12:50:44.000000 quantplay-1.5.80/quantplay/broker/shoonya.py
--rw-r--r--   0 ashok      (502) staff       (20)      515 2023-04-19 06:37:00.000000 quantplay-1.5.80/quantplay/broker/symphony.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.155419 quantplay-1.5.80/quantplay/broker/uplink/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-10 17:08:05.000000 quantplay-1.5.80/quantplay/broker/uplink/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     4019 2024-03-11 14:33:40.000000 quantplay-1.5.80/quantplay/broker/uplink/uplink_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)    19242 2024-05-08 08:54:26.000000 quantplay-1.5.80/quantplay/broker/upstox.py
--rw-r--r--   0 ashok      (502) staff       (20)    23810 2024-05-22 11:40:54.000000 quantplay-1.5.80/quantplay/broker/xts.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.157313 quantplay-1.5.80/quantplay/broker/xts_utils/
--rw-r--r--   0 ashok      (502) staff       (20)    33459 2024-03-26 12:19:14.000000 quantplay-1.5.80/quantplay/broker/xts_utils/Connect.py
--rw-r--r--   0 ashok      (502) staff       (20)     2900 2024-01-10 08:54:27.000000 quantplay-1.5.80/quantplay/broker/xts_utils/Exception.py
--rw-r--r--   0 ashok      (502) staff       (20)     6422 2024-01-10 08:54:27.000000 quantplay-1.5.80/quantplay/broker/xts_utils/InteractiveSocketClient.py
--rw-r--r--   0 ashok      (502) staff       (20)     9365 2024-02-29 11:34:06.000000 quantplay-1.5.80/quantplay/broker/xts_utils/MarketDataSocketClient.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/broker/xts_utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    19399 2024-05-18 08:39:29.000000 quantplay-1.5.80/quantplay/broker/zerodha.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.157442 quantplay-1.5.80/quantplay/brokerage/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/brokerage/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.157686 quantplay-1.5.80/quantplay/brokerage/generics/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/brokerage/generics/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    28456 2023-08-22 08:10:22.000000 quantplay-1.5.80/quantplay/brokerage/generics/broker.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.158625 quantplay-1.5.80/quantplay/brokerage/zerodha/
--rw-r--r--   0 ashok      (502) staff       (20)    18224 2023-09-25 04:30:48.000000 quantplay-1.5.80/quantplay/brokerage/zerodha/ZBroker.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/brokerage/zerodha/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.158885 quantplay-1.5.80/quantplay/config/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/config/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1461 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/config/qplay_config.py
--rw-r--r--   0 ashok      (502) staff       (20)     1127 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/create_sample_data.py
--rw-r--r--   0 ashok      (502) staff       (20)     1725 2023-04-19 06:37:00.000000 quantplay-1.5.80/quantplay/data_modify_script.py
--rw-r--r--   0 ashok      (502) staff       (20)     3481 2023-06-23 06:49:50.000000 quantplay-1.5.80/quantplay/date_fix.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.159767 quantplay-1.5.80/quantplay/exception/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/exception/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     3253 2024-04-19 04:32:07.000000 quantplay-1.5.80/quantplay/exception/exceptions.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.160378 quantplay-1.5.80/quantplay/indicators/
--rw-r--r--   0 ashok      (502) staff       (20)     1747 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/indicators/Indicator.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/indicators/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      455 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/indicators/atr.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.160549 quantplay-1.5.80/quantplay/model/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/model/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.161386 quantplay-1.5.80/quantplay/model/exchange/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/model/exchange/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1472 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/model/exchange/instrument.py
--rw-r--r--   0 ashok      (502) staff       (20)     8794 2023-05-17 08:03:33.000000 quantplay-1.5.80/quantplay/model/exchange/order.py
--rw-r--r--   0 ashok      (502) staff       (20)     3238 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/model/exchange/tick.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.161708 quantplay-1.5.80/quantplay/model/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/model/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      206 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/model/strategy/strategy_response.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.161891 quantplay-1.5.80/quantplay/oms/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/oms/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.162127 quantplay-1.5.80/quantplay/options/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-12-24 05:33:30.000000 quantplay-1.5.80/quantplay/options/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1964 2024-02-03 08:46:26.000000 quantplay-1.5.80/quantplay/options/analytics.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.162759 quantplay-1.5.80/quantplay/order_execution/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/order_execution/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2048 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/order_execution/execution_algorithm.py
--rw-r--r--   0 ashok      (502) staff       (20)     1281 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/order_execution/mean_price.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.163419 quantplay-1.5.80/quantplay/reporting/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/reporting/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10801 2023-06-23 06:49:43.000000 quantplay-1.5.80/quantplay/reporting/strategy_report.py
--rw-r--r--   0 ashok      (502) staff       (20)     1521 2023-04-19 06:37:00.000000 quantplay-1.5.80/quantplay/reporting/visuals.py
--rw-r--r--   0 ashok      (502) staff       (20)      231 2023-04-24 06:31:05.000000 quantplay-1.5.80/quantplay/service.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.164091 quantplay-1.5.80/quantplay/services/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/services/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    15321 2024-04-25 17:55:10.000000 quantplay-1.5.80/quantplay/services/market.py
--rw-r--r--   0 ashok      (502) staff       (20)    11648 2023-06-23 06:49:43.000000 quantplay-1.5.80/quantplay/services/tradelens.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.164397 quantplay-1.5.80/quantplay/strategies/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-15 03:15:32.000000 quantplay-1.5.80/quantplay/strategies/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.164506 quantplay-1.5.80/quantplay/strategies/equities/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-15 03:15:32.000000 quantplay-1.5.80/quantplay/strategies/equities/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.164621 quantplay-1.5.80/quantplay/strategies/equities/intraday/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-15 03:15:32.000000 quantplay-1.5.80/quantplay/strategies/equities/intraday/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.164737 quantplay-1.5.80/quantplay/strategies/equities/overnight/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-15 03:15:32.000000 quantplay-1.5.80/quantplay/strategies/equities/overnight/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.164851 quantplay-1.5.80/quantplay/strategies/futures/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-15 03:15:32.000000 quantplay-1.5.80/quantplay/strategies/futures/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.164963 quantplay-1.5.80/quantplay/strategies/futures/overnight/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-15 03:15:32.000000 quantplay-1.5.80/quantplay/strategies/futures/overnight/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.165063 quantplay-1.5.80/quantplay/strategies/options/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-15 03:15:32.000000 quantplay-1.5.80/quantplay/strategies/options/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.165881 quantplay-1.5.80/quantplay/strategies/options/intraday/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-15 03:15:32.000000 quantplay-1.5.80/quantplay/strategies/options/intraday/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1958 2024-03-15 03:15:32.000000 quantplay-1.5.80/quantplay/strategies/options/intraday/ladder.py
--rw-r--r--   0 ashok      (502) staff       (20)     2675 2024-03-15 03:15:32.000000 quantplay-1.5.80/quantplay/strategies/options/intraday/musk.py
--rw-r--r--   0 ashok      (502) staff       (20)      403 2024-03-15 03:15:32.000000 quantplay-1.5.80/quantplay/strategies/options/intraday/short_straddle.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.166509 quantplay-1.5.80/quantplay/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    13601 2024-04-25 17:58:36.000000 quantplay-1.5.80/quantplay/strategy/base.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-09-21 06:34:05.000000 quantplay-1.5.80/quantplay/strategy/investment_algorithm.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-09-21 06:34:44.000000 quantplay-1.5.80/quantplay/strategy.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.168691 quantplay-1.5.80/quantplay/utils/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      723 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/utils/config_util.py
--rw-r--r--   0 ashok      (502) staff       (20)    24181 2023-04-24 06:31:05.000000 quantplay-1.5.80/quantplay/utils/constant.py
--rw-r--r--   0 ashok      (502) staff       (20)     5446 2023-10-07 15:49:03.000000 quantplay-1.5.80/quantplay/utils/data_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)      711 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/utils/exchange.py
--rw-r--r--   0 ashok      (502) staff       (20)      517 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/utils/number_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)     1664 2024-01-16 16:34:52.000000 quantplay-1.5.80/quantplay/utils/pickle_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)     1225 2023-10-08 10:27:32.000000 quantplay-1.5.80/quantplay/utils/selenium_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)     4094 2023-04-19 06:36:45.000000 quantplay-1.5.80/quantplay/utils/transaction_utils.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.168885 quantplay-1.5.80/quantplay/wrapper/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-09-06 13:53:58.000000 quantplay-1.5.80/quantplay/wrapper/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.169120 quantplay-1.5.80/quantplay/wrapper/aws/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-09-06 13:54:05.000000 quantplay-1.5.80/quantplay/wrapper/aws/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1605 2024-04-11 05:52:45.000000 quantplay-1.5.80/quantplay/wrapper/aws/s3.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.146786 quantplay-1.5.80/quantplay.egg-info/
--rw-r--r--   0 ashok      (502) staff       (20)      663 2024-05-28 07:45:08.000000 quantplay-1.5.80/quantplay.egg-info/PKG-INFO
--rw-r--r--   0 ashok      (502) staff       (20)     3816 2024-05-28 07:45:08.000000 quantplay-1.5.80/quantplay.egg-info/SOURCES.txt
--rw-r--r--   0 ashok      (502) staff       (20)        1 2024-05-28 07:45:08.000000 quantplay-1.5.80/quantplay.egg-info/dependency_links.txt
--rw-r--r--   0 ashok      (502) staff       (20)      345 2024-05-28 07:45:08.000000 quantplay-1.5.80/quantplay.egg-info/requires.txt
--rw-r--r--   0 ashok      (502) staff       (20)       15 2024-05-28 07:45:08.000000 quantplay-1.5.80/quantplay.egg-info/top_level.txt
--rw-r--r--   0 ashok      (502) staff       (20)       49 2024-05-28 07:45:08.171191 quantplay-1.5.80/setup.cfg
--rw-r--r--   0 ashok      (502) staff       (20)      879 2024-05-28 07:45:05.000000 quantplay-1.5.80/setup.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.169460 quantplay-1.5.80/test/
--rw-------   0 ashok      (502) staff       (20)        0 2022-04-15 16:22:35.000000 quantplay-1.5.80/test/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.169956 quantplay-1.5.80/test/broker/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.80/test/broker/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      220 2023-04-19 06:36:45.000000 quantplay-1.5.80/test/broker/finvasia.py
--rw-r--r--   0 ashok      (502) staff       (20)     1228 2023-10-06 09:00:31.000000 quantplay-1.5.80/test/broker/motilal.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-05-28 07:45:08.170632 quantplay-1.5.80/test/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.80/test/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      292 2023-04-19 06:36:45.000000 quantplay-1.5.80/test/strategy/base.py
--rw-r--r--   0 ashok      (502) staff       (20)     2194 2023-04-19 06:36:45.000000 quantplay-1.5.80/test/strategy/sample_strategy.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.807682 quantplay-1.5.9/
+-rw-r--r--   0 ashok      (502) staff       (20)      662 2024-03-15 04:41:41.807766 quantplay-1.5.9/PKG-INFO
+-rw-r--r--   0 ashok      (502) staff       (20)      494 2023-04-19 06:36:45.000000 quantplay-1.5.9/README.md
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.786357 quantplay-1.5.9/quantplay/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.787330 quantplay-1.5.9/quantplay/backtest/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/backtest/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    17974 2024-01-30 12:40:34.000000 quantplay-1.5.9/quantplay/backtest/backtest_trades.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.791943 quantplay-1.5.9/quantplay/broker/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/broker/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    14854 2024-03-12 09:33:38.000000 quantplay-1.5.9/quantplay/broker/aliceblue.py
+-rw-r--r--   0 ashok      (502) staff       (20)    16155 2024-03-12 13:50:49.000000 quantplay-1.5.9/quantplay/broker/angelone.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3738 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/broker/broker_client.py
+-rw-r--r--   0 ashok      (502) staff       (20)       87 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/broker/client.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.792326 quantplay-1.5.9/quantplay/broker/finvasia_utils/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/broker/finvasia_utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    32131 2024-03-14 05:08:38.000000 quantplay-1.5.9/quantplay/broker/finvasia_utils/fa_noren.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2717 2024-03-06 12:51:21.000000 quantplay-1.5.9/quantplay/broker/flattrade.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.793109 quantplay-1.5.9/quantplay/broker/ft_utils/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-06 12:37:31.000000 quantplay-1.5.9/quantplay/broker/ft_utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2247 2024-01-23 17:16:24.000000 quantplay-1.5.9/quantplay/broker/ft_utils/flattrade_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)    32131 2024-03-14 05:08:42.000000 quantplay-1.5.9/quantplay/broker/ft_utils/ft_noren.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.793612 quantplay-1.5.9/quantplay/broker/generics/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/broker/generics/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    43058 2024-03-15 04:40:14.000000 quantplay-1.5.9/quantplay/broker/generics/broker.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3897 2023-05-17 07:17:28.000000 quantplay-1.5.9/quantplay/broker/iifl.py
+-rw-r--r--   0 ashok      (502) staff       (20)      750 2024-03-14 07:46:45.000000 quantplay-1.5.9/quantplay/broker/iifl_xts.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3862 2024-03-09 04:22:31.000000 quantplay-1.5.9/quantplay/broker/kite_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)    26560 2024-03-12 09:32:00.000000 quantplay-1.5.9/quantplay/broker/motilal.py
+-rw-r--r--   0 ashok      (502) staff       (20)    17924 2024-03-13 04:41:41.000000 quantplay-1.5.9/quantplay/broker/noren.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2515 2024-03-06 12:50:44.000000 quantplay-1.5.9/quantplay/broker/shoonya.py
+-rw-r--r--   0 ashok      (502) staff       (20)      515 2023-04-19 06:37:00.000000 quantplay-1.5.9/quantplay/broker/symphony.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.794149 quantplay-1.5.9/quantplay/broker/uplink/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-10 17:08:05.000000 quantplay-1.5.9/quantplay/broker/uplink/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     4019 2024-03-11 14:33:40.000000 quantplay-1.5.9/quantplay/broker/uplink/uplink_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)    15325 2024-03-14 04:29:38.000000 quantplay-1.5.9/quantplay/broker/upstox.py
+-rw-r--r--   0 ashok      (502) staff       (20)    21807 2024-03-15 03:09:59.000000 quantplay-1.5.9/quantplay/broker/xts.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.795681 quantplay-1.5.9/quantplay/broker/xts_utils/
+-rw-r--r--   0 ashok      (502) staff       (20)    33459 2024-03-15 03:09:39.000000 quantplay-1.5.9/quantplay/broker/xts_utils/Connect.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2900 2024-01-10 08:54:27.000000 quantplay-1.5.9/quantplay/broker/xts_utils/Exception.py
+-rw-r--r--   0 ashok      (502) staff       (20)     6422 2024-01-10 08:54:27.000000 quantplay-1.5.9/quantplay/broker/xts_utils/InteractiveSocketClient.py
+-rw-r--r--   0 ashok      (502) staff       (20)     9365 2024-02-29 11:34:06.000000 quantplay-1.5.9/quantplay/broker/xts_utils/MarketDataSocketClient.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/broker/xts_utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    15190 2024-03-14 05:10:02.000000 quantplay-1.5.9/quantplay/broker/zerodha.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.795873 quantplay-1.5.9/quantplay/brokerage/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/brokerage/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.796118 quantplay-1.5.9/quantplay/brokerage/angelone/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/brokerage/angelone/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10989 2023-08-08 03:19:52.000000 quantplay-1.5.9/quantplay/brokerage/angelone/angel_broker.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.796582 quantplay-1.5.9/quantplay/brokerage/generics/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/brokerage/generics/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    28456 2023-08-22 08:10:22.000000 quantplay-1.5.9/quantplay/brokerage/generics/broker.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.797429 quantplay-1.5.9/quantplay/brokerage/zerodha/
+-rw-r--r--   0 ashok      (502) staff       (20)    18224 2023-09-25 04:30:48.000000 quantplay-1.5.9/quantplay/brokerage/zerodha/ZBroker.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/brokerage/zerodha/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.797605 quantplay-1.5.9/quantplay/config/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/config/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1461 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/config/qplay_config.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1127 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/create_sample_data.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1725 2023-04-19 06:37:00.000000 quantplay-1.5.9/quantplay/data_modify_script.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3481 2023-06-23 06:49:50.000000 quantplay-1.5.9/quantplay/date_fix.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.797884 quantplay-1.5.9/quantplay/exception/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/exception/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3040 2024-03-03 06:58:26.000000 quantplay-1.5.9/quantplay/exception/exceptions.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.798211 quantplay-1.5.9/quantplay/executor/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/executor/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     6064 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/executor/strategy_executor.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.798665 quantplay-1.5.9/quantplay/indicators/
+-rw-r--r--   0 ashok      (502) staff       (20)     1747 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/indicators/Indicator.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/indicators/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      455 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/indicators/atr.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.798902 quantplay-1.5.9/quantplay/model/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/model/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.799515 quantplay-1.5.9/quantplay/model/exchange/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/model/exchange/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1472 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/model/exchange/instrument.py
+-rw-r--r--   0 ashok      (502) staff       (20)     8794 2023-05-17 08:03:33.000000 quantplay-1.5.9/quantplay/model/exchange/order.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3238 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/model/exchange/tick.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.799804 quantplay-1.5.9/quantplay/model/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/model/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      206 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/model/strategy/strategy_response.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.799973 quantplay-1.5.9/quantplay/oms/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/oms/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.800165 quantplay-1.5.9/quantplay/options/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-12-24 05:33:30.000000 quantplay-1.5.9/quantplay/options/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1964 2024-02-03 08:46:26.000000 quantplay-1.5.9/quantplay/options/analytics.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.800650 quantplay-1.5.9/quantplay/order_execution/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/order_execution/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2048 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/order_execution/execution_algorithm.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1281 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/order_execution/mean_price.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.801145 quantplay-1.5.9/quantplay/reporting/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/reporting/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10801 2023-06-23 06:49:43.000000 quantplay-1.5.9/quantplay/reporting/strategy_report.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1521 2023-04-19 06:37:00.000000 quantplay-1.5.9/quantplay/reporting/visuals.py
+-rw-r--r--   0 ashok      (502) staff       (20)      231 2023-04-24 06:31:05.000000 quantplay-1.5.9/quantplay/service.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.802117 quantplay-1.5.9/quantplay/services/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/services/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    18366 2023-05-26 07:55:13.000000 quantplay-1.5.9/quantplay/services/market.py
+-rw-r--r--   0 ashok      (502) staff       (20)    11648 2023-06-23 06:49:43.000000 quantplay-1.5.9/quantplay/services/tradelens.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.802361 quantplay-1.5.9/quantplay/strategies/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-15 03:15:32.000000 quantplay-1.5.9/quantplay/strategies/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.802476 quantplay-1.5.9/quantplay/strategies/equities/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-15 03:15:32.000000 quantplay-1.5.9/quantplay/strategies/equities/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.802591 quantplay-1.5.9/quantplay/strategies/equities/intraday/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-15 03:15:32.000000 quantplay-1.5.9/quantplay/strategies/equities/intraday/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.802696 quantplay-1.5.9/quantplay/strategies/equities/overnight/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-15 03:15:32.000000 quantplay-1.5.9/quantplay/strategies/equities/overnight/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.802795 quantplay-1.5.9/quantplay/strategies/futures/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-15 03:15:32.000000 quantplay-1.5.9/quantplay/strategies/futures/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.802893 quantplay-1.5.9/quantplay/strategies/futures/overnight/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-15 03:15:32.000000 quantplay-1.5.9/quantplay/strategies/futures/overnight/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.803006 quantplay-1.5.9/quantplay/strategies/options/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-15 03:15:32.000000 quantplay-1.5.9/quantplay/strategies/options/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.803645 quantplay-1.5.9/quantplay/strategies/options/intraday/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-15 03:15:32.000000 quantplay-1.5.9/quantplay/strategies/options/intraday/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1958 2024-03-15 03:15:32.000000 quantplay-1.5.9/quantplay/strategies/options/intraday/ladder.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2675 2024-03-15 03:15:32.000000 quantplay-1.5.9/quantplay/strategies/options/intraday/musk.py
+-rw-r--r--   0 ashok      (502) staff       (20)      403 2024-03-15 03:15:32.000000 quantplay-1.5.9/quantplay/strategies/options/intraday/short_straddle.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.804154 quantplay-1.5.9/quantplay/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    12759 2023-05-17 07:17:28.000000 quantplay-1.5.9/quantplay/strategy/base.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-09-21 06:34:05.000000 quantplay-1.5.9/quantplay/strategy/investment_algorithm.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-09-21 06:34:44.000000 quantplay-1.5.9/quantplay/strategy.py
+-rw-r--r--   0 ashok      (502) staff       (20)      214 2022-06-28 09:52:29.000000 quantplay-1.5.9/quantplay/strategy_run.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.805833 quantplay-1.5.9/quantplay/utils/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      723 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/utils/config_util.py
+-rw-r--r--   0 ashok      (502) staff       (20)    24181 2023-04-24 06:31:05.000000 quantplay-1.5.9/quantplay/utils/constant.py
+-rw-r--r--   0 ashok      (502) staff       (20)     5446 2023-10-07 15:49:03.000000 quantplay-1.5.9/quantplay/utils/data_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)      711 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/utils/exchange.py
+-rw-r--r--   0 ashok      (502) staff       (20)      517 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/utils/number_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1664 2024-01-16 16:34:52.000000 quantplay-1.5.9/quantplay/utils/pickle_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1225 2023-10-08 10:27:32.000000 quantplay-1.5.9/quantplay/utils/selenium_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)     4094 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/utils/transaction_utils.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.805971 quantplay-1.5.9/quantplay/wrapper/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-09-06 13:53:58.000000 quantplay-1.5.9/quantplay/wrapper/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.806184 quantplay-1.5.9/quantplay/wrapper/aws/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-09-06 13:54:05.000000 quantplay-1.5.9/quantplay/wrapper/aws/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1157 2023-09-06 14:08:43.000000 quantplay-1.5.9/quantplay/wrapper/aws/s3.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.787118 quantplay-1.5.9/quantplay.egg-info/
+-rw-r--r--   0 ashok      (502) staff       (20)      662 2024-03-15 04:41:41.000000 quantplay-1.5.9/quantplay.egg-info/PKG-INFO
+-rw-r--r--   0 ashok      (502) staff       (20)     3922 2024-03-15 04:41:41.000000 quantplay-1.5.9/quantplay.egg-info/SOURCES.txt
+-rw-r--r--   0 ashok      (502) staff       (20)        1 2024-03-15 04:41:41.000000 quantplay-1.5.9/quantplay.egg-info/dependency_links.txt
+-rw-r--r--   0 ashok      (502) staff       (20)      321 2024-03-15 04:41:41.000000 quantplay-1.5.9/quantplay.egg-info/requires.txt
+-rw-r--r--   0 ashok      (502) staff       (20)       15 2024-03-15 04:41:41.000000 quantplay-1.5.9/quantplay.egg-info/top_level.txt
+-rw-r--r--   0 ashok      (502) staff       (20)       49 2024-03-15 04:41:41.808027 quantplay-1.5.9/setup.cfg
+-rw-r--r--   0 ashok      (502) staff       (20)      875 2024-03-15 04:41:38.000000 quantplay-1.5.9/setup.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.806432 quantplay-1.5.9/test/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-04-15 16:22:35.000000 quantplay-1.5.9/test/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.806751 quantplay-1.5.9/test/broker/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/test/broker/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      220 2023-04-19 06:36:45.000000 quantplay-1.5.9/test/broker/finvasia.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1228 2023-10-06 09:00:31.000000 quantplay-1.5.9/test/broker/motilal.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.807111 quantplay-1.5.9/test/executor/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/test/executor/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      304 2023-04-19 06:36:45.000000 quantplay-1.5.9/test/executor/strategy_executor.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.807492 quantplay-1.5.9/test/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/test/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      292 2023-04-19 06:36:45.000000 quantplay-1.5.9/test/strategy/base.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2194 2023-04-19 06:36:45.000000 quantplay-1.5.9/test/strategy/sample_strategy.py
```

### Comparing `quantplay-1.5.80/PKG-INFO` & `quantplay-1.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantplay
-Version: 1.5.80
+Version: 1.5.9
 Summary: This python package will be stored in AWS CodeArtifact
 Home-page: 
 Author: 
 Author-email: 
 License: MIT
 
 # Quantplay Alpha playground
```

### Comparing `quantplay-1.5.80/quantplay/backtest/backtest_trades.py` & `quantplay-1.5.9/quantplay/backtest/backtest_trades.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/broker/aliceblue.py` & `quantplay-1.5.9/quantplay/broker/aliceblue.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,15 +202,15 @@
             print(traceback.print_exc())
             exception_message = f"Order placement failed [{str(e)}]"
             raise QuantplayOrderPlacementException(exception_message)
 
     def get_ltp(self, exchange, tradingsymbol):
         inst = self.alice.get_instrument_by_symbol(exchange, tradingsymbol)
         info = self.alice.get_scrip_info(inst)
-        return float(info["LTP"])
+        return info["LTP"]
 
     @retry(
         wait_exponential_multiplier=3000,
         wait_exponential_max=10000,
         stop_max_attempt_number=3,
     )
     def modify_order(self, data):
@@ -283,55 +283,46 @@
     def positions(self):
         positions = self.alice.get_netwise_positions()
 
         if not isinstance(positions, list):
             return pd.DataFrame(columns=self.positions_column_list)
 
         positions = pd.DataFrame(positions)
+
+        positions.loc[:, "tradingsymbol"] = positions.Tsym
+        positions.loc[:, "ltp"] = positions.LTP.astype(float)
         positions.loc[:, "pnl"] = positions.realisedprofitloss.astype(
             float
         ) + positions.unrealisedprofitloss.astype(float)
 
+        positions.loc[:, "option_type"] = positions.Opttype
+
         positions.rename(
             columns={
-                "LTP": "ltp",
-                "Tsym": "tradingsymbol",
-                "Opttype": "option_type",
                 "Pcode": "product",
                 "netsellqty": "sell_quantity",
                 "netbuyqty": "buy_quantity",
                 "Exchange": "exchange",
-                "Token": "token",
-                "netbuyamt": "buy_value",
-                "netSellamt": "sell_value",
             },
             inplace=True,
         )
 
-        positions["ltp"] = positions.ltp.astype(float)
         positions["buy_quantity"] = positions.buy_quantity.astype(int)
         positions["sell_quantity"] = positions.sell_quantity.astype(int)
         positions["quantity"] = positions.buy_quantity - positions.sell_quantity
-        positions["average_price"] = np.where(
-            positions.quantity > 0, positions.NetBuyavgprc, positions.NetSellavgprc
-        )
-        positions["average_price"] = np.where(
-            positions.quantity == 0, 0, positions.average_price
-        )
 
         return positions[self.positions_column_list]
 
     def orders(self, tag=None, status=None, add_ltp=True):
         orders = self.alice.order_data()
         if not isinstance(orders, list) and (
             ("no data" in orders["emsg"].lower()) or ("401" in orders["emsg"].lower())
         ):
             return pd.DataFrame(columns=self.orders_column_list)
         positions = self.positions()
-        positions = positions.sort_values("product").groupby(["tradingsymbol"]).head(1)
         if len(orders) == 0:
             return pd.DataFrame(columns=self.orders_column_list)
 
         orders = pd.DataFrame(orders)
         orders.loc[:, "tradingsymbol"] = orders.Trsym
 
         orders = pd.merge(
@@ -359,14 +350,20 @@
                 "orderentrytime": "order_timestamp",
                 "Prctype": "order_type",
                 "Status": "status",
             },
             inplace=True,
         )
 
+        existing_columns = list(orders.columns)
+        columns_to_keep = list(
+            set(self.orders_column_list).intersection(set(existing_columns))
+        )
+        orders = orders[columns_to_keep]
+
         if "filled_quantity" not in orders.columns:
             orders.loc[:, "filled_quantity"] = 0
         if "average_price" not in orders.columns:
             orders.loc[:, "average_price"] = 0
         orders["filled_quantity"] = orders.filled_quantity.astype(float)
         orders["average_price"] = orders.average_price.astype(float)
         orders.loc[:, "pnl"] = (
@@ -397,30 +394,21 @@
         )
 
         orders.order_type = orders.order_type.replace(
             ["MKT", "L", "SL"], [OrderType.market, OrderType.limit, OrderType.sl]
         )
 
         orders = self.filter_orders(orders, status=status, tag=tag)
-        for col in [
-            "tag",
-            "pending_quantity",
-            "variety",
-            "status_message",
-            "status_message_raw",
-        ]:
-            orders[col] = None
-        return orders[self.orders_column_list]
+
+        return orders
 
     def margins(self):
         margins = self.alice.get_balance()
         if "emsg" in margins and "expired" in margins["emsg"].lower():
             raise TokenException("Session expired")
-        if "stat" in margins and "not_ok" in margins["stat"].lower():
-            raise TokenException(f"Aliceblue broker error: {margins['emsg']}")
         margins = [a for a in margins if a["segment"] == "ALL"][0]
 
         response = {
             "margin_used": float(margins["debits"]),
             "total_balance": float(margins["credits"]),
             "margin_available": float(margins["net"]),
         }
```

### Comparing `quantplay-1.5.80/quantplay/broker/angelone.py` & `quantplay-1.5.9/quantplay/broker/angelone.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 from quantplay.utils.exchange import Market as MarketConstants
 from quantplay.exception.exceptions import (
     QuantplayOrderPlacementException,
     TokenException,
     ServiceException,
     RetryableException,
     retry_exception,
-    BrokerException,
 )
-from requests.exceptions import ConnectTimeout, ConnectionError
 import pickle
 import codecs
 from quantplay.wrapper.aws.s3 import S3Utils
 
 from quantplay.utils.pickle_utils import InstrumentData
 
 from quantplay.utils.constant import Constants, OrderType, timeit
@@ -89,18 +87,14 @@
             self.load_instrument()
 
     def set_wrapper(self, serialized_wrapper):
         self.wrapper = pickle.loads(
             codecs.decode(serialized_wrapper.encode(), "base64")
         )
 
-    def handle_exception(self, response):
-        if "errorCode" in response and response["errorCode"] == "AG8001":
-            raise TokenException(f"{self.user_id}: Invalid Token")
-
     @timeit(MetricName="Angelone:load_instrument")
     def load_instrument(self):
         try:
             self.symbol_data = InstrumentData.get_instance().load_data(
                 "angelone_instruments"
             )
             Constants.logger.info("[LOADING_INSTRUMENTS] loading data from cache")
@@ -218,19 +212,16 @@
                 "quantity": quantity,
                 "duration": "DAY",
                 "ordertag": tag,
             }
 
             Constants.logger.info("[PLACING_ORDER] {}".format(json.dumps(order)))
             return self.wrapper.placeOrder(order)
-        except (TimeoutError, ConnectTimeout) as e:
-            Constants.logger.info(f"[ANGELONE_REQUEST_TIMEOUT] {order}")
         except Exception as e:
-            traceback.print_exc()
-            Constants.logger.error(f"[PLACE_ORDER_FAILED] {e} {order}")
+            Constants.logger.error(traceback.print_exc())
             raise QuantplayOrderPlacementException(str(e))
 
     def get_variety(self, variety):
         if variety == "regular":
             return "NORMAL"
         return variety
 
@@ -277,37 +268,32 @@
             Constants.logger.info(
                 f"Modifying order [{order_id}] params [{order_params}]"
             )
             response = self.wrapper.modifyOrder(order_params)
             Constants.logger.info(f"[MODIFY_ORDER_RESPONSE] {response}")
             return response
         except Exception as e:
-            traceback.print_exc()
+            Constants.logger.error(traceback.print_exc())
             Constants.logger.error(
                 f"[MODIFY_ORDER_FAILED] for {data['order_id']} failed with exception {e}"
             )
             raise
 
     @timeit(MetricName="Angelone:cancel_order")
     def cancel_order(self, order_id, variety="NORMAL"):
         self.wrapper.cancelOrder(order_id=order_id, variety=variety)
 
     @timeit(MetricName="Angelone:positions")
     @retry(
         wait_exponential_multiplier=3000,
         wait_exponential_max=15000,
         stop_max_attempt_number=5,
-        retry_on_exception=retry_exception,
     )
     def positions(self):
-        try:
-            positions = self.wrapper.position()
-        except:
-            raise RetryableException("Access Denied retrying")
-        self.handle_exception(positions)
+        positions = self.wrapper.position()
 
         if positions["data"] is None:
             return pd.DataFrame(columns=self.positions_column_list)
 
         positions = pd.DataFrame(positions["data"])
 
         if "optiontype" not in positions.columns:
@@ -335,34 +321,24 @@
         positions.loc[:, "pnl"] = positions.pnl.astype(float)
         positions.loc[:, "quantity"] = positions.buy_quantity - positions.sell_quantity
 
         positions["product"] = positions["product"].replace(
             ["DELIVERY", "CARRYFORWARD", "INTRADAY"], ["CNC", "NRML", "MIS"]
         )
 
-        existing_columns = list(positions.columns)
-        columns_to_keep = list(
-            set(self.positions_column_list).intersection(set(existing_columns))
-        )
-        return positions[columns_to_keep]
+        return positions[self.positions_column_list]
 
     @timeit(MetricName="Angelone:orders")
     @retry(
         wait_exponential_multiplier=3000,
         wait_exponential_max=10000,
         stop_max_attempt_number=3,
-        retry_on_exception=retry_exception,
     )
     def orders(self, tag=None, status=None, add_ltp=True):
-        try:
-            order_book = self.wrapper.orderBook()
-        except:
-            raise RetryableException("Access Denied retrying")
-        self.handle_exception(order_book)
-
+        order_book = self.wrapper.orderBook()
         if order_book["data"]:
             orders = pd.DataFrame(order_book["data"])
 
             if len(orders) == 0:
                 return pd.DataFrame(columns=self.orders_column_list)
 
             if add_ltp:
@@ -434,62 +410,46 @@
                 raise ServiceException("Unknown error while fetching order book [{}]")
 
     @timeit(MetricName="Angelone:profile")
     @retry(
         wait_exponential_multiplier=3000,
         wait_exponential_max=10000,
         stop_max_attempt_number=3,
-        retry_on_exception=retry_exception,
     )
     def profile(self):
-        try:
-            profile_data = self.wrapper.getProfile(self.refresh_token)
-        except:
-            raise RetryableException("Access Denied retrying")
-        self.handle_exception(profile_data)
-
-        profile_data = profile_data["data"]
+        profile_data = self.wrapper.getProfile(self.refresh_token)["data"]
         response = {
             "user_id": profile_data["clientcode"],
             "full_name": profile_data["name"],
             "email": profile_data["email"],
         }
 
         return response
 
     @timeit(MetricName="Angelone:margins")
     @retry(
         wait_exponential_multiplier=3000,
         wait_exponential_max=10000,
         stop_max_attempt_number=3,
-        retry_on_exception=retry_exception,
     )
     def margins(self):
         api_margins = self.wrapper.rmsLimit()
-        self.handle_exception(api_margins)
         if "data" in api_margins and api_margins["data"] is None:
-            if "errorcode" in api_margins and api_margins["errorcode"] == "AB1004":
-                raise TokenException(f"Angelone server not not responding")
-            return {"margin_used": 0, "margin_available": 0, "total_balance": 0}
+            return {"net": 0}
         api_margins = api_margins["data"]
 
-        try:
-            collateral = 0
-            if "collateral" in api_margins:
-                collateral = float(api_margins["collateral"])
-            margins = {}
-            margins["margin_used"] = float(api_margins["net"])
-            margins["margin_available"] = float(api_margins["net"])
-            margins["total_balance"] = float(api_margins["net"])
-
-            return margins
-        except (ConnectionError, ConnectTimeout) as e:
-            raise BrokerException("Angelone broker error while fetching margins")
-        except Exception as e:
-            raise RetryableException(f"Angelone: Failed to fetch margin {e}")
+        collateral = 0
+        if "collateral" in api_margins:
+            collateral = float(api_margins["collateral"])
+        margins = {}
+        margins["margin_used"] = float(api_margins["net"])
+        margins["margin_available"] = float(api_margins["net"])
+        margins["total_balance"] = float(api_margins["net"])
+
+        return margins
 
     def account_summary(self):
         margins = self.margins()
 
         pnl = 0
         positions = self.positions()
         if len(positions) > 0:
```

### Comparing `quantplay-1.5.80/quantplay/broker/broker_client.py` & `quantplay-1.5.9/quantplay/broker/broker_client.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/broker/finvasia_utils/fa_noren.py` & `quantplay-1.5.9/quantplay/broker/finvasia_utils/fa_noren.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/broker/five_paisa.py` & `quantplay-1.5.9/quantplay/broker/zerodha.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,474 +1,456 @@
-import numpy as np
 import pandas as pd
-import pyotp, pickle, codecs
-from py5paisa import FivePaisaClient
+import codecs
+import pickle
+import numpy as np
 from retrying import retry
-import json, traceback
-from datetime import datetime
-
+from quantplay.utils.constant import Constants, timeit
 from quantplay.broker.generics.broker import Broker
+from quantplay.config.qplay_config import QplayConfig
+from kiteconnect import KiteConnect
+from kiteconnect.exceptions import TokenException
+import traceback
+
+from quantplay.broker.kite_utils import KiteUtils
+
+from kiteconnect import KiteTicker
 from quantplay.exception.exceptions import (
-    RetryableException,
-    TokenException,
-    QuantplayOrderPlacementException,
     InvalidArgumentException,
-    retry_exception,
+    QuantplayOrderPlacementException,
 )
-from quantplay.utils.constant import Constants, timeit, OrderStatus
+from quantplay.utils.pickle_utils import PickleUtils, InstrumentData
 
-logger = Constants.logger
 
+class Zerodha(Broker):
+    stoploss = "stoploss"
+    zerodha_api_key = "zerodha_api_key"
+    zerodha_api_secret = "zerodha_api_secret"
+    zerodha_wrapper = "zerodha_wrapper"
 
-class FivePaisa(Broker):
-    @retry(
-        wait_exponential_multiplier=1000,
-        wait_exponential_max=10000,
-        stop_max_attempt_number=3,
-        retry_on_exception=retry_exception,
-    )
-    @timeit(MetricName="5Paisa:__init__")
+    @timeit(MetricName="Zerodha:__init__")
     def __init__(
         self,
-        app_source=None,
-        app_user_id=None,
-        app_password=None,
-        user_key=None,
-        encryption_key=None,
-        client_id=None,
-        totp_key=None,
-        pin=None,
-        client=None,
+        wrapper=None,
+        user_id=None,
+        api_key=None,
+        api_secret=None,
+        password=None,
+        totp=None,
         load_instrument=True,
     ):
-        self.broker_name = "FivePaisa_OpenAPI"
         try:
-            if client:
-                self.set_client(client)
+            if wrapper:
+                self.set_wrapper(wrapper)
             else:
-                client = FivePaisaClient(
-                    cred={
-                        "APP_SOURCE": app_source,
-                        "APP_NAME": f"5P{client_id}",
-                        "USER_ID": app_user_id,
-                        "USER_KEY": user_key,
-                        "PASSWORD": app_password,
-                        "ENCRYPTION_KEY": encryption_key,
-                    }
-                )
-                self.user_key = user_key
-                self.client = client
-                self.client.get_totp_session(client_id, pyotp.TOTP(totp_key).now(), pin)
-
-                try:
-                    self.margins()
-                except TokenException as e:
-                    raise RetryableException("Generating token again")
-        except RetryableException as e:
-            raise
+                self.generate_token(user_id, api_key, api_secret, password, totp)
         except Exception as e:
             raise e
 
-        self.set_user_id()
+        try:
+            self.wrapper.orders()
+        except Exception as e:
+            raise InvalidArgumentException(
+                "Zerodha client generation failed due to invalid arguments"
+            )
+
+        Constants.logger.info(self.wrapper.profile())
 
         if load_instrument:
-            self.load_instrument()
-        super(FivePaisa, self).__init__()
+            self.initialize_symbol_data()
+        super(Zerodha, self).__init__()
 
-    def set_client(self, serialized_client):
-        self.client = pickle.loads(codecs.decode(serialized_client.encode(), "base64"))
+    def set_wrapper(self, serialized_wrapper):
+        self.wrapper = pickle.loads(
+            codecs.decode(serialized_wrapper.encode(), "base64")
+        )
 
-    def set_user_id(self):
-        self.user_id = self.client.client_code
+    def initialize_symbol_data(self):
+        try:
+            self.symbol_data = InstrumentData.get_instance().load_data(
+                "zerodha_instruments"
+            )
+            Constants.logger.info("[LOADING_INSTRUMENTS] loading data from cache")
+        except Exception as e:
+            instruments = self.wrapper.instruments()
+            self.symbol_data = {}
+            for instrument in instruments:
+                exchange = instrument["exchange"]
+                tradingsymbol = instrument["tradingsymbol"]
+                self.symbol_data["{}:{}".format(exchange, tradingsymbol)] = instrument
+
+            PickleUtils.save_data(self.symbol_data, "zerodha_instruments")
+            Constants.logger.info("[LOADING_INSTRUMENTS] loading data from server")
+
+    def set_username(self, username):
+        self.username = username
+
+    def get_username(self):
+        return self.username
+
+    def on_ticks(self, kws, ticks):
+        """Callback on live ticks"""
+        # logger.info("[TEST_TICK] {}".format(ticks))
+        pass
+
+    def on_order_update(self, kws, data):
+        """Callback on order update"""
+        Constants.logger.info("[UPDATE_RECEIVED] {}".format(data))
+        self.order_updates.put(data)
+
+    def on_connect(self, kws, response):
+        """Callback on successfull connect"""
+        kws.subscribe([256265])
+        kws.set_mode(kws.MODE_FULL, [256265])
+
+    def stream_order_data(self):
+        kite_ticker = KiteTicker(self.wrapper.api_key, self.wrapper.access_token)
+        kite_ticker.on_order_update = self.on_order_update
+        kite_ticker.on_ticks = self.on_ticks
+        kite_ticker.on_connect = self.on_connect
 
-    def get_client(self):
-        return codecs.encode(pickle.dumps(self.client), "base64").decode()
-
-    def load_instrument(self):
-        super().load_instrument("5paisa_instruments")
-
-    def handle_exception(self, e):
-        if "Unauthorized" in e.reason:
-            raise TokenException("Token Expired")
-        raise RetryableException(e.reason)
-
-    def token_url(self):
-        url = f"https://dev-openapi.5paisa.com/WebVendorLogin/VLogin/Index?VendorKey={self.user_key}&ResponseURL=http://127.0.0.1"
-
-    def holdings(self):
-        data = self.client.holdings()
-        return pd.DataFrame(data)
-
-    def set_access_token(self, access_token):
-        self.access_token = access_token
-
-    def get_product(self, product):
-        if product == "NRML":
-            return "D"
-        elif product == "CNC":
-            return "D"
-        elif product == "MIS":
-            return "I"
-        return product
-
-    def get_lot_size(self, exchange, tradingsymbol):
-        tradingsymbol = self.get_symbol(tradingsymbol, exchange)
-        return int(
-            self.symbol_data["{}:{}".format(exchange, tradingsymbol)]["lot_size"]
-        )
+        kite_ticker.connect(threaded=True)
 
     @retry(
-        wait_exponential_multiplier=1000,
+        wait_exponential_multiplier=3000,
         wait_exponential_max=10000,
         stop_max_attempt_number=3,
-        retry_on_exception=retry_exception,
     )
-    @timeit(MetricName="5Paisa:profile")
-    def profile(self):
-        response = {"user_id": self.client.client_code}
-
+    @timeit(MetricName="Zerodha:get_ltps")
+    def get_ltps(self, trading_symbols):
+        response = self.wrapper.ltp(trading_symbols)
         return response
 
+    def get_quantplay_symbol(self, symbol):
+        return symbol
+
     @retry(
-        wait_exponential_multiplier=1000,
+        wait_exponential_multiplier=3000,
         wait_exponential_max=10000,
         stop_max_attempt_number=3,
-        retry_on_exception=retry_exception,
     )
-    @timeit(MetricName="5Paisa:get_ltp")
-    def get_ltp(self, exchange, tradingsymbol):
-        tradingsymbol = self.get_symbol(tradingsymbol, exchange)
-        exchange_name = self.get_exchange(exchange)
-        exchange_type = self.get_exchange_type(exchange)
-        token = self.symbol_attribute(exchange, tradingsymbol, "token")
-        req_list_ = [
-            {"Exch": exchange_name, "ExchType": exchange_type, "ScripCode": token}
-        ]
+    @timeit(MetricName="Zerodha:get_ltp")
+    def get_ltp(self, exchange=None, tradingsymbol=None):
+        try:
+            key = "{}:".format(exchange) + tradingsymbol
+            response = self.wrapper.ltp([key])
 
-        return self.client.fetch_market_feed_scrip(req_list_)["Data"][0]["LastRate"]
+            if key not in response:
+                raise InvalidArgumentException(
+                    "Symbol {} not listed on exchange".format(tradingsymbol)
+                )
 
-        return response
+            response = response[key]["last_price"]
+            return response
+        except Exception as e:
+            exception_message = "GetLtp call failed for [{}] with error [{}]".format(
+                tradingsymbol, str(e)
+            )
+            Constants.logger.error("{}".format(exception_message))
+
+    @retry(
+        wait_exponential_multiplier=3000,
+        wait_exponential_max=10000,
+        stop_max_attempt_number=3,
+    )
+    def get_orders(self, status=None):
+        orders = self.wrapper.orders()
+        if status:
+            orders = [a for a in orders if a["status"] == status]
+        return orders
+
+    @retry(
+        wait_exponential_multiplier=3000,
+        wait_exponential_max=10000,
+        stop_max_attempt_number=3,
+    )
+    @timeit(MetricName="Zerodha:modify_order")
+    def modify_order(self, data):
+        order_id = data["order_id"]
+
+        try:
+            data["variety"] = "regular"
+            if "trigger_price" not in data:
+                data["trigger_price"] = None
+            Constants.logger.info(
+                "Modifying order [{}] new price [{}]".format(
+                    data["order_id"], data["price"]
+                )
+            )
+            response = self.wrapper.modify_order(
+                order_id=order_id,
+                variety=data["variety"],
+                price=data["price"],
+                trigger_price=data["trigger_price"],
+                order_type=data["order_type"],
+            )
+            return response
+        except Exception as e:
+            exception_message = (
+                "OrderModificationFailed for {} failed with exception {}".format(
+                    data["order_id"], e
+                )
+            )
+            if (
+                "Order cannot be modified as it is being processed"
+                not in exception_message
+            ):
+                Constants.logger.error("{}".format(exception_message))
+
+    @timeit(MetricName="Zerodha:cancel_order")
+    def cancel_order(self, order_id, variety="regular"):
+        self.wrapper.cancel_order(order_id=order_id, variety=variety)
+
+    def get_ltp_by_order(self, order):
+        exchange = order["exchange"]
+        tradingsymbol = order["tradingsymbol"]
 
-    def add_exchange(self, data):
-        exchange_condition = [
-            (data["Exch"] == "N") & (data["ExchType"] == "D"),
-            (data["Exch"] == "N") & (data["ExchType"] == "C"),
-            (data["Exch"] == "B") & (data["ExchType"] == "D"),
-            (data["Exch"] == "B") & (data["ExchType"] == "C"),
-        ]
+        return self.get_ltp(exchange, tradingsymbol)
 
-        exchange_name = ["NFO", "NSE", "BFO", "BSE"]
+    @retry(
+        wait_exponential_multiplier=3000,
+        wait_exponential_max=10000,
+        stop_max_attempt_number=3,
+    )
+    def get_positions(self):
+        return self.wrapper.positions()
+
+    def positions_pnl(self):
+        positions = pd.DataFrame(self.get_positions()["net"])
+        print("Total PnL {}".format(positions.pnl.astype(float).sum()))
 
-        data.loc[:, "exchange"] = np.select(
-            exchange_condition, exchange_name, default=0
+    def add_params(self, orders):
+        df = pd.DataFrame(orders)
+        df.loc[:, "price"] = df.apply(
+            lambda x: self.get_ltp(x["exchange"], x["tradingsymbol"]), axis=1
         )
 
+        df.loc[:, "disclosedquantity"] = np.where(
+            df.exchange == "NSE", df.quantity / 10 + 1, df.quantity
+        )
+        df.loc[:, "disclosedquantity"] = df.disclosedquantity.astype(int)
+
+        return df.to_dict("records")
+
+    # @retry(wait_exponential_multiplier=3000, wait_exponential_max=10000, stop_max_attempt_number=3)
+    @timeit(MetricName="Zerodha:place_order")
+    def place_order(
+        self,
+        tradingsymbol=None,
+        exchange=None,
+        quantity=None,
+        order_type=None,
+        transaction_type=None,
+        tag=None,
+        product=None,
+        price=None,
+        trigger_price=None,
+    ):
+        try:
+            Constants.logger.info(
+                f"[PLACING_ORDER] {tradingsymbol} {exchange} {quantity} {tag}"
+            )
+            order_id = self.wrapper.place_order(
+                variety="regular",
+                tradingsymbol=tradingsymbol,
+                exchange=exchange,
+                transaction_type=transaction_type,
+                quantity=int(abs(quantity)),
+                order_type=order_type,
+                disclosed_quantity=None,
+                price=price,
+                trigger_price=trigger_price,
+                product=product,
+                tag=tag,
+            )
+            return order_id
+        except Exception as e:
+            raise QuantplayOrderPlacementException(str(e))
+
+    def configure(self):
+        quantplay_config = QplayConfig.get_config()
+
+        print("Enter Zerodha API key:")
+        api_key = input()
+
+        print("Enter Zerodha API Secret:")
+        api_secret = input()
+
+        quantplay_config["DEFAULT"][Zerodha.zerodha_api_key] = api_key
+        quantplay_config["DEFAULT"][Zerodha.zerodha_api_secret] = api_secret
+
+        with open("{}/config".format(QplayConfig.config_path), "w") as configfile:
+            quantplay_config.write(configfile)
+
+    def validate_config(self, quantplay_config):
+        if quantplay_config is None:
+            return False
+        if Zerodha.zerodha_api_key not in quantplay_config["DEFAULT"]:
+            return False
+        if Zerodha.zerodha_api_secret not in quantplay_config["DEFAULT"]:
+            return False
+
+        return True
+
+    def generate_token(self, user_id, api_key, api_secret, password, totp):
+        kite = KiteConnect(api_key=api_key)
+
+        try:
+            request_token = KiteUtils.get_request_token(
+                api_key=api_key, user_id=user_id, password=password, totp=totp
+            )
+            data = kite.generate_session(request_token, api_secret=api_secret)
+            kite.set_access_token(data["access_token"])
+        except TokenException as e:
+            message = str(e)
+            if "Invalid" in message and "checksum" in message:
+                raise InvalidArgumentException("Invalid API secret")
+            raise
+        except Exception as e:
+            traceback.print_exc()
+            print("Need token input " + kite.login_url())
+            raise e
+
+        self.kite = kite
+        self.wrapper = kite
+
+    @timeit(MetricName="Zerodha:profile")
+    def profile(self):
+        user_profile = self.wrapper.profile()
+
+        response = {
+            "user_id": user_profile["user_id"],
+            "full_name": user_profile["user_name"],
+            "segments": user_profile["exchanges"],
+            "email": user_profile["email"],
+        }
+
+        return response
+
     @retry(
         wait_exponential_multiplier=3000,
         wait_exponential_max=10000,
         stop_max_attempt_number=3,
-        retry_on_exception=retry_exception,
     )
-    @timeit(MetricName="5Paisa:positions")
+    @timeit(MetricName="Zerodha:positions")
     def positions(self, drop_cnc=True):
-        # create an instance of the API class
-        positions = self.client.positions()
-        if positions is None:
-            raise TokenException("5Paisa Token expired")
+        positions = pd.DataFrame(self.wrapper.positions()["net"])
 
         if len(positions) == 0:
             return pd.DataFrame(columns=self.positions_column_list)
-        positions = pd.DataFrame(positions)
-        positions.rename(
-            columns={
-                "ScripName": "tradingsymbol",
-                "AvgRate": "average_price",
-                "SellQty": "sell_quantity",
-                "BuyQty": "buy_quantity",
-                "SellValue": "sell_value",
-                "BuyValue": "buy_value",
-                "LTP": "ltp",
-                "ScripCode": "token",
-                "NetQty": "quantity",
-            },
-            inplace=True,
-        )
-
-        positions["sell_quantity"] = np.where(
-            positions.CFQty < 0,
-            -positions.CFQty + positions.sell_quantity,
-            positions.sell_quantity,
-        )
-        positions["buy_quantity"] = np.where(
-            positions.CFQty > 0,
-            positions.CFQty + positions.buy_quantity,
-            positions.buy_quantity,
-        )
-        positions["buy_value"] = (
-            positions.buy_value + positions.CFQty * positions.AvgCFQty
+
+        positions.loc[:, "exchange_symbol"] = (
+            positions.exchange + ":" + positions.tradingsymbol
         )
-        # positions["sell_value"] = positions.BookedPL
-        # positions["buy_value"] = 0
+        symbols = positions.exchange_symbol.unique().tolist()
+        symbol_ltps = self.get_ltps(symbols)
 
+        positions.loc[:, "ltp"] = positions.exchange_symbol.apply(
+            lambda x: symbol_ltps[x]["last_price"]
+        )
         positions.loc[:, "pnl"] = positions.sell_value - positions.buy_value
-        positions.loc[:, "pnl"] += (
-            positions.buy_quantity - positions.sell_quantity
-        ) * positions.ltp
-
-        self.add_exchange(positions)
+        positions.loc[:, "pnl"] += (positions.quantity) * positions.ltp
 
         positions.loc[:, "option_type"] = np.where(
-            positions.exchange.isin(["NFO", "BFO"]),
-            positions.tradingsymbol.str.split(" ").str[-2],
-            np.nan,
+            "PE" == positions.tradingsymbol.str[-2:], "PE", "CE"
         )
-
-        positions["product"] = positions["OrderFor"].replace(
-            ["I", "D"], ["MIS", "NRML"]
-        )
-        positions["product"] = np.where(
-            (
-                (positions["exchange"].isin(["NSE", "BSE"]))
-                & (positions["product"] == "NRML")
-            ),
-            "CNC",
-            positions["product"],
+        positions.loc[:, "option_type"] = np.where(
+            positions.exchange.isin(["NFO", "BFO"]), positions.option_type, None
+        )
+        positions["token"] = positions.apply(
+            lambda x: self.symbol_data[f"{x['exchange']}:{x['tradingsymbol']}"][
+                "exchange_token"
+            ],
+            axis=1,
         )
 
         if drop_cnc:
             positions = positions[positions["product"] != "CNC"]
         return positions[self.positions_column_list]
 
     @retry(
-        wait_exponential_multiplier=1000,
+        wait_exponential_multiplier=3000,
         wait_exponential_max=10000,
         stop_max_attempt_number=3,
-        retry_on_exception=retry_exception,
     )
-    @timeit(MetricName="Upstox:orders")
+    @timeit(MetricName="Zerodha:orders")
     def orders(self, tag=None, add_ltp=True):
-        orders = self.client.order_book()
+        orders = pd.DataFrame(self.wrapper.orders())
+
+        positions = self.positions()
         if len(orders) == 0:
             return pd.DataFrame(columns=self.orders_column_list)
-        orders = pd.DataFrame(orders)
-        self.add_exchange(orders)
-
-        orders.rename(
-            columns={
-                "OrderRequesterCode": "user_id",
-                "ExchOrderID": "order_id",
-                "ScripCode": "token",
-                "ScripName": "tradingsymbol",
-                "BuySell": "transaction_type",
-                "AveragePrice": "average_price",
-                "Qty": "quantity",
-                "Rate": "price",
-                "SLTriggerRate": "trigger_price",
-                "OrderStatus": "status",
-                "TradedQty": "filled_quantity",
-                "PendingQty": "pending_quantity",
-                "BrokerOrderTime": "order_timestamp",
-                "Reason": "status_message",
-            },
-            inplace=True,
-        )
 
-        positions = self.positions()
         positions = positions.sort_values("product").groupby(["tradingsymbol"]).head(1)
         orders = pd.merge(
             orders,
             positions[["tradingsymbol", "ltp"]],
             how="left",
             left_on=["tradingsymbol"],
             right_on=["tradingsymbol"],
         )
 
-        orders.loc[:, "order_type"] = np.where(
-            orders["AtMarket"] == "Y", "MARKET", "LIMIT"
-        )
-        orders.loc[:, "order_type"] = np.where(
-            ((orders["order_type"] == "LIMIT") & (orders["WithSL"] == "Y")),
-            "SL",
-            orders["order_type"],
+        orders.rename(columns={"placed_by": "user_id"}, inplace=True)
+
+        existing_columns = list(orders.columns)
+        columns_to_keep = list(
+            set(self.orders_column_list).intersection(set(existing_columns))
         )
+        orders = orders[columns_to_keep]
 
         orders.loc[:, "pnl"] = (
             orders.ltp * orders.filled_quantity
             - orders.average_price * orders.filled_quantity
         )
         orders.loc[:, "pnl"] = np.where(
             orders.transaction_type == "SELL", -orders.pnl, orders.pnl
         )
-        orders.transaction_type = orders.transaction_type.replace(
-            ["S", "B"], ["SELL", "BUY"]
-        )
 
         if tag:
             orders = orders[orders.tag == tag]
 
-        orders["tradingsymbol"] = np.where(
-            orders.exchange == "NSE",
-            orders.tradingsymbol.str.replace("-EQ", ""),
-            orders.tradingsymbol,
-        )
-
-        orders["update_timestamp"] = orders.order_timestamp
-        orders["status"] = orders.status.replace(
-            ["Pending", "Modified", "Cancelled", "Fully Executed"],
-            [
-                OrderStatus.open,
-                OrderStatus.open,
-                OrderStatus.cancelled,
-                OrderStatus.complete,
-            ],
-        )
-        orders["status"] = np.where(
-            orders.status.str.lower().str.contains("rejected"),
-            OrderStatus.rejected,
-            orders.status,
-        )
-        orders["status"] = np.where(
-            ((orders.status == "OPEN") & (orders.order_type == "SL")),
-            OrderStatus.trigger_pending,
-            orders.status,
-        )
-
-        orders["product"] = orders["DelvIntra"].replace(["D", "I"], ["CNC", "MIS"])
-        orders["product"] = np.where(
-            ((orders["product"] == "CNC") & (orders["exchange"].isin(["NFO", "BFO"]))),
-            "NRML",
-            orders["product"],
-        )
-
-        orders["tag"] = None
-        orders["status_message_raw"] = None
-        orders["variety"] = "regular"
-        orders["order_timestamp"] = orders.order_timestamp.apply(
-            lambda x: datetime.fromtimestamp(int(x[6:16]))
-        )
-        orders["update_timestamp"] = orders.update_timestamp.apply(
-            lambda x: datetime.fromtimestamp(int(x[6:16]))
-        )
-
-        orders = orders[self.orders_column_list]
         return orders
 
-    def get_symbol(self, symbol, exchange=None):
-        if symbol not in self.quantplay_symbol_map:
-            return symbol
-        return self.quantplay_symbol_map[symbol]
-
-    @staticmethod
-    def is_intraday(product):
-        if product in ["MIS"]:
-            return True
-        return False
-
-    @staticmethod
-    def get_exchange(exch):
-        return exch[0]
-
-    @staticmethod
-    def get_exchange_type(exchange):
-        if exchange in ["NSE", "BSE"]:
-            return "C"
-        elif exchange in ["NFO", "BFO"]:
-            return "D"
-        raise InvalidArgumentException(f"exchange {exchange} not supported")
-
-    @timeit(MetricName="FivePaisa:place_order")
-    def place_order(
-        self,
-        tradingsymbol=None,
-        exchange=None,
-        quantity=None,
-        order_type=None,
-        transaction_type=None,
-        tag=None,
-        product=None,
-        price=None,
-        trigger_price=None,
-    ):
-        try:
-            if trigger_price is None:
-                trigger_price = 0
-
-            product = self.get_product(product)
-            tradingsymbol = self.get_symbol(tradingsymbol)
-
-            try:
-                token = self.symbol_attribute(exchange, tradingsymbol, "token")
-            except Exception as e:
-                raise InvalidArgumentException(
-                    f"Invalid symbol {tradingsymbol} for exchange {exchange}"
-                )
-
-            Constants.logger.info(
-                f"[PLACING_ORDER] {tradingsymbol} {transaction_type[0]} {exchange} {token} {quantity}"
-            )
-            response = self.client.place_order(
-                OrderType=transaction_type[0],
-                Exchange=FivePaisa.get_exchange(exchange),
-                ExchangeType=FivePaisa.get_exchange_type(exchange),
-                ScripCode=token,
-                Qty=quantity,
-                Price=price,
-                IsIntraday=FivePaisa.is_intraday(product),
-                StopLossPrice=trigger_price,
-            )
-
-            logger.info(f"[PLACE_ORDER_RESPONSE] {self.broker_name} {response}")
-            if response is None:
-                raise QuantplayOrderPlacementException(
-                    "Failed to place order on 5Paisa"
-                )
-            if "Status" in response and response["Status"] == 1:
-                logger.error(
-                    f"[ORDER_PLACED_FAILED] {self.broker_name}-{self.user_id} {response}"
-                )
-                raise QuantplayOrderPlacementException(response["Message"])
-            if "BrokerOrderID" in response:
-                return response["BrokerOrderID"]
-        except (QuantplayOrderPlacementException, InvalidArgumentException) as e:
-            raise e
-        except Exception as e:
-            traceback.print_exc()
-            exception_message = "Order placement failed with error [{}]".format(str(e))
-            logger.error(f"[PLACE_ORDER_FAILED] {self.broker_name} {exception_message}")
-
     @retry(
         wait_exponential_multiplier=3000,
         wait_exponential_max=10000,
         stop_max_attempt_number=3,
-        retry_on_exception=retry_exception,
     )
-    @timeit(MetricName="FivePaisa:margins")
+    @timeit(MetricName="Zerodha:margins")
     def margins(self):
-        margins = self.client.margin()
-        if margins is None:
-            raise TokenException("5Paisa Token expired")
-        margins = margins[0]
+        margins = self.wrapper.margins()
 
         margins = {
-            "margin_used": margins["MarginUtilized"],
-            "margin_available": margins["NetAvailableMargin"],
+            "margin_used": float(margins["equity"]["utilised"]["debits"]),
+            "margin_available": float(margins["equity"]["net"]),
         }
         return margins
 
-    @timeit(MetricName="5Paisa:account_summary")
+    def basket_margin(self, basket_orders):
+        response = self.wrapper.basket_order_margins(basket_orders, mode="compact")
+
+        charges = response["orders"]
+        return {
+            "initial": response["initial"]["total"],
+            "final": response["final"]["total"],
+            "total_charges": sum([a["charges"]["total"] for a in charges]),
+            "exchange_turnover_charge": sum(
+                [a["charges"]["exchange_turnover_charge"] for a in charges]
+            ),
+            "brokerage": sum([a["charges"]["brokerage"] for a in charges]),
+            "transaction_tax": sum([a["charges"]["transaction_tax"] for a in charges]),
+            "gst": sum([a["charges"]["gst"]["total"] for a in charges]),
+        }
+
+    @retry(
+        wait_exponential_multiplier=3000,
+        wait_exponential_max=10000,
+        stop_max_attempt_number=3,
+    )
+    @timeit(MetricName="Zerodha:account_summary")
     def account_summary(self):
         margins = self.margins()
         response = {
             "margin_used": margins["margin_used"],
             "margin_available": margins["margin_available"],
             "pnl": float(self.positions().pnl.sum()),
         }
         return response
-
-    def get_quantplay_product(self, exchange, product):
-        product_map = {"D": "CNC", "I": "MIS"}
-        if product in product_map:
-            product = product_map[product]
-        if product == "CNC" and exchange in ["NFO", "BFO"]:
-            product = "NRML"
-
-        return product
```

### Comparing `quantplay-1.5.80/quantplay/broker/flattrade.py` & `quantplay-1.5.9/quantplay/broker/flattrade.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/broker/ft_utils/flattrade_utils.py` & `quantplay-1.5.9/quantplay/broker/ft_utils/flattrade_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/broker/ft_utils/ft_noren.py` & `quantplay-1.5.9/quantplay/broker/ft_utils/ft_noren.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/broker/generics/broker.py` & `quantplay-1.5.9/quantplay/broker/generics/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 import zipfile
 import requests
 import platform
 
 from quantplay.exception.exceptions import (
     QuantplayOrderPlacementException,
     InvalidArgumentException,
-    StaleDataFound,
     FeatureNotSupported,
 )
 from quantplay.utils.constant import Constants
 from quantplay.utils.exchange import Market as MarketConstants
 from quantplay.utils.number_utils import NumberUtils
 from quantplay.utils.constant import Order, StrategyType, ExchangeName, timeit
 import traceback, copy
@@ -58,66 +57,32 @@
             "order_timestamp",
             "trigger_price",
             "price",
             "token",
             "update_timestamp",
             "order_type",
             "variety",
-            "status_message",
-            "status_message_raw",
         ]
         self.positions_column_list = [
             "token",
             "tradingsymbol",
             "quantity",
-            "average_price",
             "buy_quantity",
             "sell_quantity",
             "buy_value",
             "sell_value",
             "exchange",
             "product",
             "option_type",
             "ltp",
             "pnl",
         ]
-        self.holdings_column_list = [
-            "exchange",
-            "token",
-            "tradingsymbol",
-            "isin",
-            "quantity",
-            "pledged_quantity",
-            "average_price",
-            "price",
-            "buy_value",
-            "current_value",
-            "pct_change",
-        ]
         self.trigger_pending_status = "TRIGGER PENDING"
         self.lock = Lock()
 
-    def validate_exchange(self, exchange):
-        if exchange not in ["NSE", "NFO", "BFO", "BSE"]:
-            raise InvalidArgumentException(f"exchange {exchange} not supported")
-
-    def validate_existance(self, input, message):
-        if not input:
-            raise InvalidArgumentException(message)
-
-    def symbol_attribute(self, exchange, symbol, value):
-        try:
-            value = self.symbol_data[f"{exchange}:{symbol}"][value]
-            return value
-        except KeyError as e:
-            logger.error(
-                f"[MISSING_SYMBOL_DATA] for [{exchange}:{symbol}] attribute {value}"
-            )
-            raise StaleDataFound(f"Couldn't find symbol data for [{exchange}:{symbol}]")
-
     def initialize_symbol_data(self, save_as=None):
         instruments = self.instrument_data
         instruments = instruments.to_dict("records")
         self.symbol_data = {}
         for instrument in instruments:
             exchange = instrument["exchange"]
             tradingsymbol = instrument["broker_symbol"]
@@ -127,17 +92,17 @@
 
         PickleUtils.save_data(self.symbol_data, save_as)
 
     @timeit(MetricName="Broker:initialize_broker_symbol_map")
     def initialize_broker_symbol_map(self):
         self.broker_symbol_map = {}
         for a in self.symbol_data:
-            self.broker_symbol_map[self.symbol_data[a]["broker_symbol"]] = (
-                self.symbol_data[a]["tradingsymbol"]
-            )
+            self.broker_symbol_map[
+                self.symbol_data[a]["broker_symbol"]
+            ] = self.symbol_data[a]["tradingsymbol"]
         platform_version = platform.python_version().split(".")
         if (
             len(platform_version) >= 2
             and platform_version[0] == "3"
             and platform_version[1] == "8"
         ):
             self.quantplay_symbol_map = {}
@@ -179,17 +144,17 @@
             exchange, symbol, instrument_id = (
                 instrument.exchange,
                 instrument.symbol,
                 instrument.instrument_id,
             )
             self.instrument_id_to_symbol_map[instrument_id] = symbol
             self.instrument_id_to_exchange_map[instrument_id] = exchange
-            self.instrument_id_to_security_type_map[instrument_id] = (
-                instrument.security_type()
-            )
+            self.instrument_id_to_security_type_map[
+                instrument_id
+            ] = instrument.security_type()
             self.exchange_symbol_to_instrument_id_map[exchange][symbol] = instrument_id
 
     def add_quantplay_fut_tradingsymbol(self):
         seg_condition = [
             (
                 (self.instrument_data["instrument"].str.contains("FUT"))
                 & (self.instrument_data.instrument != "OPTFUT")
@@ -261,17 +226,17 @@
         z.extractall(path=directory)
         file_name = url.split(".txt")[0].split("/")[-1]
         os.system("cp /tmp/{}.txt /tmp/{}.csv".format(file_name, file_name))
         time.sleep(2)
         return pd.read_csv("/tmp/{}.csv".format(file_name))
 
     def initialize_expiry_fields(self):
-        self.instrument_data.loc[:, "tradingsymbol"] = (
-            self.instrument_data.instrument_symbol
-        )
+        self.instrument_data.loc[
+            :, "tradingsymbol"
+        ] = self.instrument_data.instrument_symbol
         self.instrument_data.loc[:, "expiry"] = pd.to_datetime(
             self.instrument_data.instrument_expiry
         )
 
         self.instrument_data.loc[:, "expiry_year"] = (
             self.instrument_data["expiry"].dt.strftime("%y").astype(str)
         )
@@ -292,17 +257,17 @@
             self.instrument_data.month_number.astype(float) >= 10,
             self.instrument_data.month.str[0]
             + self.instrument_data["expiry"].dt.strftime("%d").astype(str),
             self.instrument_data.month_number
             + self.instrument_data["expiry"].dt.strftime("%d").astype(str),
         )
 
-        self.instrument_data.loc[:, "next_expiry"] = (
-            self.instrument_data.expiry + pd.DateOffset(days=7)
-        )
+        self.instrument_data.loc[
+            :, "next_expiry"
+        ] = self.instrument_data.expiry + pd.DateOffset(days=7)
 
     def execute_order_v2(self, order):
         start_time = datetime.now()
         tradingsymbol = order["tradingsymbol"]
         exchange = order["exchange"]
         trigger_price = order["trigger_price"]
         transaction_type = order["transaction_type"]
@@ -507,23 +472,25 @@
 
     def get_product(self, product):
         return product
 
     def get_lot_size(self, exchange, tradingsymbol):
         tradingsymbol = self.get_symbol(tradingsymbol, exchange=exchange)
         exchange = self.get_exchange(exchange)
-        if exchange == "BSE" or exchange == "NSE":
+        if exchange == "BSE":
             return 1
         try:
             return int(
                 self.symbol_data["{}:{}".format(exchange, tradingsymbol)]["lot_size"]
             )
         except Exception as e:
             logger.error(
-                f"[GET_LOT_SIZE] unable to get lot size for {exchange} {tradingsymbol}"
+                "[GET_LOT_SIZE] unable to get lot size for {} {}".format(
+                    exchange, tradingsymbol
+                )
             )
             raise e
 
     def filter_orders(self, orders, tag=None, status=None):
         if tag:
             orders = orders[orders.tag == tag]
 
@@ -579,17 +546,17 @@
         if symbol_contains is not None:
             symbol_contains = self.get_symbol(symbol_contains)
             stoploss_orders = stoploss_orders[
                 stoploss_orders["tradingsymbol"].str.contains(symbol_contains)
             ]
 
         if order_timestamp is not None:
-            stoploss_orders.loc[:, "order_timestamp"] = (
-                stoploss_orders.order_timestamp.apply(lambda x: x.replace(second=0))
-            )
+            stoploss_orders.loc[
+                :, "order_timestamp"
+            ] = stoploss_orders.order_timestamp.apply(lambda x: x.replace(second=0))
             stoploss_orders = stoploss_orders[
                 stoploss_orders.order_timestamp.astype(str) == order_timestamp
             ]
 
         if len(stoploss_orders) == 0:
             Constants.logger.info("All stoploss orders have been already closed")
             return
@@ -787,14 +754,15 @@
             time.sleep(1)
         self.order_updates.put(order)
 
     def get_quantplay_symbol(self, symbol):
         return self.broker_symbol_map[symbol]
 
     def stream_order_updates(self):
+
         self.order_log = {}
         while 1:
             try:
                 orders = self.orders(add_ltp=False)
 
                 if len(orders) > 0:
                     delta_time = str(
@@ -822,52 +790,43 @@
                 print(f"Unable to process order stream for {self.user_id}")
                 time.sleep(5)
 
     def stream_order_data(self):
         th = threading.Thread(target=self.stream_order_updates, daemon=True)
         th.start()
 
-    def underlying_config(self, underlying_symbol, expiry=None):
+    def underlying_config(self, underlying_symbol, expiry):
         if underlying_symbol in ["BANKNIFTY", "BANKEX"]:
             return {"max_lots": 60, "lot_size": 15, "strike_gap": 100}
         elif underlying_symbol == "FINNIFTY":
             return {"max_lots": 45, "lot_size": 40, "strike_gap": 50}
         elif underlying_symbol == "SENSEX":
             return {"max_lots": 100, "lot_size": 10, "strike_gap": 100}
         elif underlying_symbol == "NIFTY":
-            return {"max_lots": 72, "lot_size": 25, "strike_gap": 50}
+            return {"max_lots": 36, "lot_size": 50, "strike_gap": 50}
         elif underlying_symbol == "MIDCPNIFTY":
             return {"max_lots": 56, "lot_size": 75, "strike_gap": 25}
 
         raise Exception(f"Underlying {underlying_symbol} symbol not supported")
 
     def symbol_max_lots(self, exchange, symbol):
         try:
-            if symbol in self.broker_symbol_map:
-                symbol = self.broker_symbol_map[symbol]
             if "BANKNIFTY" in symbol and exchange == "NFO":
-                return self.underlying_config("BANKNIFTY")["max_lots"]
+                return 60
             elif "FINNIFTY" in symbol and exchange == "NFO":
-                return self.underlying_config("FINNIFTY")["max_lots"]
-            elif "MIDCPNIFTY" in symbol and exchange == "NFO":
-                return self.underlying_config("MIDCPNIFTY")["max_lots"]
-            elif "NIFTY" in symbol and exchange == "NFO":
-                return self.underlying_config("NIFTY")["max_lots"]
-            elif "BANKEX" in symbol and exchange == "BFO":
-                return self.underlying_config("BANKEX")["max_lots"]
+                return 45
             elif "SENSEX" in symbol and exchange == "BFO":
-                return self.underlying_config("SENSEX")["max_lots"]
+                return 100
             elif exchange == "NSE":
-                max_qty = int(500000 / self.get_ltp(exchange, symbol))
+                max_qty = int(50000 / self.get_ltp(exchange, symbol))
                 if max_qty == 0:
                     return 1
                 return max_qty
             return 36
         except Exception as e:
-            traceback.print_exc()
             logger.error(f"Couldn't compute freeze quantity for {exchange} {symbol}")
             return 25
 
     def square_off_by_tag(self, tag, dry_run=True, sleep_time=0.05):
         self.exit_all_trigger_orders(tag=tag)
         orders = self.orders(tag=tag)
```

### Comparing `quantplay-1.5.80/quantplay/broker/iifl.py` & `quantplay-1.5.9/quantplay/broker/iifl.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/broker/iifl_xts.py` & `quantplay-1.5.9/quantplay/broker/iifl_xts.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/broker/kite_utils.py` & `quantplay-1.5.9/quantplay/broker/kite_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/broker/motilal.py` & `quantplay-1.5.9/quantplay/broker/motilal.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,38 +370,27 @@
                 "[ORDER_MODIFICATION_FAILED] for {} failed with exception {}".format(
                     order["uniqueorderid"], e
                 )
             )
             Constants.logger.error("{}".format(exception_message))
 
     @timeit(MetricName="Motilal:cancel_order")
-    @retry(
-        wait_exponential_multiplier=3000,
-        wait_exponential_max=10000,
-        stop_max_attempt_number=2,
-        retry_on_exception=retry_exception,
-    )
     def cancel_order(self, unique_order_id):
         data = {"uniqueorderid": unique_order_id}
 
         try:
             Constants.logger.info("Cancelling order [{}]".format(unique_order_id))
             response = requests.post(
                 self.cancel_order_url, headers=self.headers, data=json.dumps(data)
             ).json()
             if "errorcode" in response and response["errorcode"] in ["MO1066"]:
                 Constants.logger.info(
                     f"[CANCEL_ORDER_RESPONSE] [{unique_order_id}] already cancelled"
                 )
                 return
-            elif "errorcode" in response and response["errorcode"] in ["MO5002"]:
-                raise RetryableException("Retry due to network error")
-            elif "errorcode" in response and response["errorcode"] in ["MO1060"]:
-                # Invalid order Id
-                return
             Constants.logger.info("Cancel order response [{}]".format(response))
         except Exception as e:
             exception_message = (
                 "[ORDER_CANCELLATION_FAILED] unique_order_id {} exception {}".format(
                     unique_order_id, e
                 )
             )
@@ -488,16 +477,14 @@
             "tag": tag,
         }
         try:
             Constants.logger.info("[PLACING_ORDER] {}".format(json.dumps(data)))
             response = requests.post(
                 self.place_order_url, headers=self.headers, data=json.dumps(data)
             ).json()
-            if "errorcode" in response and response["errorcode"] in ["100018"]:
-                return
             Constants.logger.info(
                 "[PLACE_ORDER_RESPONSE] {} input {}".format(response, json.dumps(data))
             )
             if response["status"] == "ERROR":
                 raise QuantplayOrderPlacementException(response["message"])
             return response["uniqueorderid"]
         except QuantplayOrderPlacementException as e:
@@ -643,23 +630,19 @@
             },
             inplace=True,
         )
 
         positions["exchange"] = positions["exchange"].replace(
             ["NSEFO", "BSEFO"], ["NFO", "BFO"]
         )
-        positions["product"] = positions["product"].replace(["NORMAL"], ["NRML"])
 
-        existing_columns = list(positions.columns)
-        columns_to_keep = list(
-            set(self.positions_column_list).intersection(set(existing_columns))
-        )
-        return positions[columns_to_keep]
+        return positions[self.positions_column_list]
 
     def order_details(self, order_id):
+
         response = (
             requests.post(
                 self.order_details_url,
                 headers=self.headers,
                 data=json.dumps({"uniqueorderid": order_id}),
             )
         ).json()
@@ -672,15 +655,14 @@
                 "Error while fetching order book [{}]".format(response["message"])
             )
             raise Exception(response["message"])
         orders = response["data"]
         orders = pd.DataFrame(orders)
 
         positions = self.positions()
-        positions = positions.sort_values("product").groupby(["tradingsymbol"]).head(1)
         if len(orders) == 0:
             return pd.DataFrame(columns=self.orders_column_list)
 
         orders.loc[:, "tradingsymbol"] = orders.symbol
         orders = pd.merge(
             orders,
             positions[["tradingsymbol", "ltp"]],
@@ -689,15 +671,14 @@
             right_on=["tradingsymbol"],
         )
 
         orders.rename(
             columns={
                 "clientid": "user_id",
                 "LTP": "ltp",
-                "symboltoken": "token",
                 "buyorsell": "transaction_type",
                 "averageprice": "average_price",
                 "uniqueorderid": "order_id",
                 "orderstatus": "status",
                 "recordinserttime": "order_timestamp",
                 "orderqty": "quantity",
                 "triggerprice": "trigger_price",
```

### Comparing `quantplay-1.5.80/quantplay/broker/noren.py` & `quantplay-1.5.9/quantplay/broker/noren.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,19 @@
 import json
 import traceback
 
 import numpy as np
 import pandas as pd
 from retrying import retry
-from json.decoder import JSONDecodeError
 
 from quantplay.broker.generics.broker import Broker
-from quantplay.exception.exceptions import (
-    InvalidArgumentException,
-    RetryableException,
-    TokenException,
-    retry_exception,
-    BrokerException,
-)
+from quantplay.exception.exceptions import InvalidArgumentException
 from quantplay.utils.constant import Constants, OrderType, timeit
 from quantplay.utils.pickle_utils import InstrumentData
 from quantplay.wrapper.aws.s3 import S3Utils
-from datetime import datetime, timedelta
 
 logger = Constants.logger
 
 
 class Noren(Broker):
     def __init__(
         self,
@@ -216,100 +208,107 @@
                 "[PLACE_ORDER_RESPONSE] {} input {}".format(response, json.dumps(data))
             )
             if "norenordno" in response:
                 return response["norenordno"]
             else:
                 raise Exception(response)
         except Exception as e:
-            traceback.print_exc()
+            print(traceback.print_exc())
             exception_message = "Order placement failed with error [{}]".format(str(e))
-            logger.error(f"[PLACE_ORDER_FAILED] {exception_message}")
+            print(exception_message)
 
     def get_orders(self):
         return self.api.get_order_book()
 
-    @retry(
-        wait_exponential_multiplier=3000,
-        wait_exponential_max=10000,
-        stop_max_attempt_number=3,
-    )
-    @timeit(MetricName="Noren:get_ltp")
+    @timeit(MetricName="Finvasia:get_ltp")
     def get_ltp(self, exchange, tradingsymbol):
         tradingsymbol = self.get_symbol(tradingsymbol)
-
         token = self.symbol_data["{}:{}".format(exchange, tradingsymbol)]["token"]
         return float(self.api.get_quotes(exchange, str(token))["lp"])
 
     def live_data(self, exchange, tradingsymbol):
         tradingsymbol = self.get_symbol(tradingsymbol)
         token = self.symbol_data["{}:{}".format(exchange, tradingsymbol)]["token"]
         data = self.api.get_quotes(exchange, str(token))
         return {
             "ltp": float(data["lp"]),
             "upper_circuit": float(data["uc"]),
             "lower_circuit": float(data["lc"]),
         }
 
-    def order_history(self, order_id):
-        order_history = self.api.single_order_history(order_id)
-        order_details = order_history[0]
-
-        data = {}
-        data["order_id"] = order_id
-        data["order_type"] = order_details["prctyp"]
-        data["exchange"] = order_details["exch"]
-        data["quantity"] = order_details["qty"]
-        data["tradingsymbol"] = order_details["tsym"]
-
-        return data
-
     @retry(
         wait_exponential_multiplier=3000,
         wait_exponential_max=10000,
         stop_max_attempt_number=3,
     )
     @timeit(MetricName="Finvasia:modify_order")
     def modify_order(self, data):
-        order_id = data["order_id"]
         data["order_type"] = self.get_order_type(data["order_type"])
-        existing_details = self.order_history(order_id)
 
         if "trigger_price" not in data:
             data["trigger_price"] = None
-
-        if "order_type" not in data:
-            data["order_type"] = existing_details["order_type"]
-        if "quantity" not in data:
-            data["quantity"] = existing_details["quantity"]
-
+        if "order_id" in data:
+            data["norenordno"] = data["order_id"]
+        if "exchange" in data:
+            data["exch"] = data["exchange"]
+        if "tradingsymbol" in data:
+            data["tsym"] = data["tradingsymbol"]
+        if "order_type" in data:
+            data["prctyp"] = data["order_type"]
+        if "quantity" in data:
+            data["qty"] = data["quantity"]
+        if "price" in data:
+            data["prc"] = data["price"]
         try:
-            logger.info(f"[MODIFYING_ORDER] {data}")
+            logger.info(
+                "Modifying order [{}] new price [{}]".format(
+                    data["norenordno"], data["prc"]
+                )
+            )
             response = self.api.modify_order(
-                orderno=order_id,
-                exchange=existing_details["exchange"],
-                tradingsymbol=existing_details["tradingsymbol"],
-                newprice_type=data["order_type"],
-                newquantity=data["quantity"],
-                newprice=data["price"],
+                orderno=data["norenordno"],
+                exchange=data["exch"],
+                tradingsymbol=data["tsym"],
+                newprice_type=data["prctyp"],
+                newquantity=data["qty"],
+                newprice=data["prc"],
                 newtrigger_price=data["trigger_price"],
             )
             logger.info(
                 "[MODIFY_ORDER_RESPONSE] order id [{}] response [{}]".format(
-                    data["order_id"], response
+                    data["norenordno"], response
                 )
             )
             return response
         except Exception as e:
             exception_message = (
                 "OrderModificationFailed for {} failed with exception {}".format(
-                    data["order_id"], e
+                    data["norenordno"], e
                 )
             )
             Constants.logger.error("{}".format(exception_message))
-            raise e
+
+    @timeit(MetricName="Finvasia:modify_price")
+    def modify_price(self, order_id, price, trigger_price=None, order_type=None):
+        data = {}
+        order_history = self.api.single_order_history(order_id)
+        order_details = order_history[0]
+        data["norenordno"] = order_id
+        data["prc"] = price
+        data["prctyp"] = order_details["prctyp"]
+        data["exch"] = order_details["exch"]
+        data["qty"] = order_details["qty"]
+        data["tsym"] = order_details["tsym"]
+        data["order_type"] = order_type
+        if trigger_price != None and trigger_price > 0:
+            data["newtrigger_price"] = trigger_price
+        else:
+            data["newtrigger_price"] = None
+
+        self.modify_order(data)
 
     @timeit(MetricName="Finvasia:cancel_order")
     def cancel_order(self, order_id):
         self.api.cancel_order(order_id)
 
     def stream_order_data(self):
         self.api.start_websocket(order_update_callback=self.event_handler_order_update)
@@ -320,69 +319,22 @@
             "user_id": self.user_id,
             "full_name": self.full_name,
             "email": self.email,
         }
 
         return response
 
-    @timeit(MetricName="Noren:holdings")
-    @retry(
-        wait_exponential_multiplier=3000,
-        wait_exponential_max=10000,
-        stop_max_attempt_number=3,
-    )
-    def holdings(self):
-        holdings = self.api.get_holdings()
-        if holdings is None or len(holdings) == 0:
-            return pd.DataFrame(columns=self.holdings_column_list)
-
-        holdings = [
-            {
-                "exchange": h["exch_tsym"][0]["exch"],
-                "token": h["exch_tsym"][0]["token"],
-                "tradingsymbol": h["exch_tsym"][0]["tsym"],
-                "isin": h["exch_tsym"][0]["isin"],
-                "quantity": int(h["holdqty"])
-                + int(h.get("npoadqty", 0))
-                + int(h.get("brkcolqty", 0)),
-                "pledged_quantity": int(h.get("brkcolqty", 0)),
-                "average_price": float(h.get("upldprc", 0)),
-            }
-            for h in holdings
-        ]
-        holdings = pd.DataFrame(holdings)
-        holdings["price"] = holdings.apply(
-            lambda x: self.get_ltp(x["exchange"], x["tradingsymbol"]), axis=1
-        )
-
-        holdings["tradingsymbol"] = holdings.tradingsymbol.str.replace("-EQ", "")
-        holdings["buy_value"] = holdings.quantity * holdings.average_price
-        holdings["current_value"] = holdings.quantity * holdings.price
-        holdings["pct_change"] = (holdings.price / holdings.average_price - 1) * 100
-
-        return holdings[self.holdings_column_list]
-
     @timeit(MetricName="Finvasia:positions")
     @retry(
         wait_exponential_multiplier=3000,
         wait_exponential_max=10000,
         stop_max_attempt_number=3,
-        retry_on_exception=retry_exception,
     )
     def positions(self):
-        try:
-            positions = self.api.get_positions()
-            if positions is None:
-                return pd.DataFrame(columns=self.positions_column_list)
-        except BrokerException:
-            raise
-        except JSONDecodeError as e:
-            raise BrokerException("Broker failed to send positions")
-        except Exception as e:
-            raise
+        positions = self.api.get_positions()
 
         if positions is None or len(positions) == 0:
             return pd.DataFrame(columns=self.positions_column_list)
 
         positions = pd.DataFrame(positions)
 
         positions.loc[:, "tradingsymbol"] = positions.tsym
@@ -409,28 +361,27 @@
             positions.exch.isin(["NFO", "BFO"]), positions.option_type, None
         )
 
         positions.rename(
             columns={
                 "prd": "product",
                 "exch": "exchange",
-                "netavgprc": "average_price",
             },
             inplace=True,
         )
 
         mandatory_columns = ["daybuyqty", "daysellqty", "cfbuyqty", "cfsellqty"]
         for mad_c in mandatory_columns:
             if mad_c not in positions.columns:
                 positions.loc[:, mad_c] = 0
 
-        positions.loc[:, "buy_quantity"] = positions.daybuyqty.fillna(0).astype(
+        positions.loc[:, "buy_quantity"] = positions.daybuyqty.astype(
             int
         ) + positions.cfbuyqty.astype(int)
-        positions.loc[:, "sell_quantity"] = positions.daysellqty.fillna(0).astype(
+        positions.loc[:, "sell_quantity"] = positions.daysellqty.astype(
             int
         ) + positions.cfsellqty.astype(int)
         positions.loc[:, "quantity"] = positions.buy_quantity - positions.sell_quantity
 
         positions["product"] = positions["product"].replace(
             ["I", "C", "M"], ["MIS", "CNC", "NRML"]
         )
@@ -439,41 +390,25 @@
             columns={
                 "totsellamt": "sell_value",
                 "totbuyamt": "buy_value",
             },
             inplace=True,
         )
 
-        existing_columns = list(positions.columns)
-        columns_to_keep = list(
-            set(self.positions_column_list).intersection(set(existing_columns))
-        )
-        return positions[columns_to_keep]
+        return positions[self.positions_column_list]
 
     def add_transaction_charges(self, orders):
         return super(Noren, self).add_transaction_charges(
             orders, cm_charges=0, fo_charges=0
         )
 
     @timeit(MetricName="Finvasia:orders")
     def orders(self, tag=None, status=None, add_ltp=True):
-        try:
-            orders = self.api.get_order_book()
-            if orders is None:
-                return pd.DataFrame(columns=self.orders_column_list)
-        except BrokerException:
-            raise
-        except JSONDecodeError as e:
-            raise BrokerException("Broker failed to send orders")
-        except Exception as e:
-            raise
-
-        orders = pd.DataFrame(orders)
+        orders = pd.DataFrame(self.api.get_order_book())
         positions = self.positions()
-        positions = positions.sort_values("product").groupby(["tradingsymbol"]).head(1)
         if len(orders) == 0:
             return pd.DataFrame(columns=self.orders_column_list)
 
         orders.loc[:, "tradingsymbol"] = orders.tsym
         orders = pd.merge(
             orders,
             positions[["tradingsymbol", "ltp"]],
@@ -490,19 +425,17 @@
                 "remarks": "tag",
                 "avgprc": "average_price",
                 "prd": "product",
                 "trantype": "transaction_type",
                 "qty": "quantity",
                 "trgprc": "trigger_price",
                 "prc": "price",
-                "prctyp": "order_type",
                 "fillshares": "filled_quantity",
                 "rorgqty": "pending_quantity",
                 "norentm": "order_timestamp",
-                "rejreason": "status_message",
             },
             inplace=True,
         )
 
         existing_columns = list(orders.columns)
         columns_to_keep = list(
             set(self.orders_column_list).intersection(set(existing_columns))
@@ -535,63 +468,48 @@
         orders.status = orders.status.replace(
             ["TRIGGER_PENDING", "CANCELED"], ["TRIGGER PENDING", "CANCELLED"]
         )
 
         orders["product"] = orders["product"].replace(
             ["I", "C", "M"], ["MIS", "CNC", "NRML"]
         )
-        orders["order_type"] = orders["order_type"].replace(
-            ["MKT", "LMT", "SL-LMT", "SL-MKT"], ["MARKET", "LIMIT", "SL", "SL-M"]
-        )
 
         return orders
 
     @timeit(MetricName="Finvasia:positions")
     @retry(
-        wait_exponential_multiplier=1000,
-        wait_exponential_max=10000,
+        wait_exponential_multiplier=3000,
+        wait_exponential_max=15000,
         stop_max_attempt_number=3,
-        retry_on_exception=retry_exception,
     )
     def margins(self):
         api_margins = self.api.get_limits()
-        if "stat" in api_margins and "not_ok" == api_margins["stat"].lower():
-            raise TokenException(api_margins["emsg"])
+        collateral = 0
+        if "collateral" in api_margins:
+            collateral = api_margins["collateral"]
 
-        try:
-            collateral = 0
-            if "collateral" in api_margins:
-                collateral = api_margins["collateral"]
-
-            if "marginused" not in api_margins:
-                api_margins["margin_used"] = 0
-            else:
-                api_margins["margin_used"] = api_margins["marginused"]
-            if "payin" not in api_margins:
-                api_margins["payin"] = 0
-            margin_available = (
-                float(api_margins["cash"])
-                + float(collateral)
-                + float(api_margins["payin"])
-                - float(api_margins["margin_used"])
-            )
-
-            margins = {}
-            margins["margin_used"] = api_margins["margin_used"]
-            margins["margin_available"] = margin_available
-            try:
-                margins["cash"] = float(api_margins["cash"])
-            except:
-                margins["cash"] = 0
-            margins["total_balance"] = float(api_margins["cash"]) + float(collateral)
+        if "marginused" not in api_margins:
+            api_margins["margin_used"] = 0
+        else:
+            api_margins["margin_used"] = api_margins["marginused"]
+        if "payin" not in api_margins:
+            api_margins["payin"] = 0
+        margin_available = (
+            float(api_margins["cash"])
+            + float(collateral)
+            + float(api_margins["payin"])
+            - float(api_margins["margin_used"])
+        )
+
+        margins = {}
+        margins["margin_used"] = api_margins["margin_used"]
+        margins["margin_available"] = margin_available
+        margins["total_balance"] = float(api_margins["cash"]) + float(collateral)
 
-            return margins
-        except Exception as e:
-            logger.error(f"[NOREN_MARGIN_ERROR] {e}")
-            RetryableException("[NOREN] Failed to fetch account margin")
+        return margins
 
     @timeit(MetricName="Finvasia:account_summary")
     def account_summary(self):
         margins = self.margins()
         pnl = 0
         positions = self.positions()
         if len(positions) > 0:
@@ -600,78 +518,7 @@
         response = {
             "margin_used": margins["margin_used"],
             "total_balance": margins["total_balance"],
             "margin_available": margins["margin_available"],
             "pnl": pnl,
         }
         return response
-
-    def historical_data(
-        self,
-        exchange=None,
-        token=None,
-        tradingsymbol=None,
-        interval=None,
-        start_time=None,
-        end_time=datetime.now(),
-        days=None,
-    ):
-        self.validate_exchange(exchange)
-        if tradingsymbol:
-            tradingsymbol = self.get_symbol(tradingsymbol, exchange=exchange)
-            token = self.symbol_data[f"{exchange}:{tradingsymbol}"]["token"]
-            self.validate_existance(token, "Invalid trading symbol")
-        self.validate_existance(token, "Invalid token")
-
-        if days:
-            start_time = datetime.now() - timedelta(days=days)
-            end_time = datetime.now()
-
-        if interval == "day":
-            data = self.api.get_daily_price_series(
-                exchange=exchange,
-                tradingsymbol=tradingsymbol,
-                startdate=start_time.timestamp(),
-                enddate=end_time.timestamp(),
-            )
-            data = [json.loads(a) for a in data]
-        else:
-            interval_map = {"minute": 1, "5minute": 5}
-            interval = interval_map[interval]
-
-            data = self.api.get_time_price_series(
-                exchange=exchange,
-                token=str(token),
-                starttime=start_time.timestamp(),
-                endtime=end_time.timestamp(),
-                interval=interval,
-            )
-        data = pd.DataFrame(data)
-        data.rename(
-            columns={
-                "time": "date",
-                "into": "open",
-                "inth": "high",
-                "intl": "low",
-                "intc": "close",
-                "intvwap": "vwap",
-                "intv": "volume",
-            },
-            inplace=True,
-        )
-
-        if interval == "day":
-            data["date"] = pd.to_datetime(data["date"], format="%d-%b-%Y")
-        else:
-            data["date"] = pd.to_datetime(data["date"], format="%d-%m-%Y %H:%M:%S")
-        columns_to_return = [
-            "date",
-            "open",
-            "high",
-            "low",
-            "close",
-            "vwap",
-            "volume",
-            "oi",
-        ]
-        data = data[list(set(columns_to_return).intersection(set(data.columns)))]
-        return data.sort_values("date").reset_index(drop=True)
```

### Comparing `quantplay-1.5.80/quantplay/broker/shoonya.py` & `quantplay-1.5.9/quantplay/broker/shoonya.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/broker/symphony.py` & `quantplay-1.5.9/quantplay/broker/symphony.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/broker/uplink/uplink_utils.py` & `quantplay-1.5.9/quantplay/broker/uplink/uplink_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/broker/upstox.py` & `quantplay-1.5.9/quantplay/broker/upstox.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 import traceback
 
 import numpy as np
 import pandas as pd
 import upstox_client
-import asyncio
-import threading
-import ssl
-import json
-import websockets
 from quantplay.exception.exceptions import (
     InvalidArgumentException,
     RetryableException,
     TokenException,
     retry_exception,
 )
 from retrying import retry
@@ -68,19 +63,14 @@
         if load_instrument:
             self.load_instrument()
         super(Upstox, self).__init__()
 
     def load_instrument(self):
         super().load_instrument("upstox_instruments")
 
-    def handle_exception(self, e):
-        if "Unauthorized" in e.reason:
-            raise TokenException("Token Expired")
-        raise RetryableException(e.reason)
-
     def set_access_token(self, access_token):
         self.access_token = access_token
 
     def get_product(self, product):
         if product == "NRML":
             return "D"
         elif product == "CNC":
@@ -111,18 +101,17 @@
 
     def get_lot_size(self, exchange, tradingsymbol):
         return int(
             self.symbol_data["{}:{}".format(exchange, tradingsymbol)]["lot_size"]
         )
 
     @retry(
-        wait_exponential_multiplier=1000,
+        wait_exponential_multiplier=3000,
         wait_exponential_max=10000,
         stop_max_attempt_number=3,
-        retry_on_exception=retry_exception,
     )
     @timeit(MetricName="Upstox:get_ltp")
     def get_ltp(self, exchange=None, tradingsymbol=None):
         # create an instance of the API class
         api_instance = upstox_client.MarketQuoteApi(
             upstox_client.ApiClient(self.configuration)
         )
@@ -133,24 +122,20 @@
             # Market quotes and instruments - LTP quotes.
             api_response = api_instance.ltp(symbol_info["instrument_key"], api_version)
 
             return api_response.data[
                 f"{self.get_exchange(symbol_info['exchange'])}:{tradingsymbol}"
             ].last_price
         except ApiException as e:
-            Constants.logger.error(
-                "Exception when calling MarketQuoteApi->ltp: %s\n" % e
-            )
-            self.handle_exception(e)
+            Constants.logger("Exception when calling MarketQuoteApi->ltp: %s\n" % e)
 
     @retry(
-        wait_exponential_multiplier=1000,
+        wait_exponential_multiplier=3000,
         wait_exponential_max=10000,
         stop_max_attempt_number=3,
-        retry_on_exception=retry_exception,
     )
     @timeit(MetricName="Upstox:modify_order")
     def modify_order(self, data):
         if "trigger_price" not in data or data["trigger_price"] is None:
             data["trigger_price"] = 0
         # create an instance of the API class
         api_instance = upstox_client.OrderApi(
@@ -166,42 +151,36 @@
         api_version = "2.0"  # str | API Version Header
 
         try:
             # Modify order
             api_response = api_instance.modify_order(body, api_version)
             return api_response.status
         except ApiException as e:
-            Constants.logger.error(
-                "Exception when calling OrderApi->modify_order: %s\n" % e
-            )
+            Constants.logger("Exception when calling OrderApi->modify_order: %s\n" % e)
 
             Constants.logger.info(
                 "Modifying order [{}] new price [{}]".format(
                     data["order_id"], data["price"]
                 )
             )
-            self.handle_exception(e)
 
     @timeit(MetricName="Upstox:cancel_order")
     def cancel_order(self, order_id, variety="regular"):
         # create an instance of the API class
         api_instance = upstox_client.OrderApi(
             upstox_client.ApiClient(self.configuration)
         )
         api_version = "2.0"  # str | API Version Header
 
         try:
             # Cancel order
             api_response = api_instance.cancel_order(order_id, api_version)
             return api_response.status
         except ApiException as e:
-            Constants.logger.error(
-                "Exception when calling OrderApi->cancel_order: %s\n" % e
-            )
-            self.handle_exception(e)
+            Constants.logger("Exception when calling OrderApi->cancel_order: %s\n" % e)
 
     @timeit(MetricName="Upstox:place_order")
     def place_order(
         self,
         tradingsymbol=None,
         exchange=None,
         quantity=None,
@@ -268,38 +247,31 @@
         except TokenException as e:
             message = str(e)
             if "Invalid" in message and "checksum" in message:
                 raise InvalidArgumentException("Invalid API secret")
             raise
         except Exception as e:
             traceback.print_exc()
-            Constants.logger.error(f"Failed to generate upstox token {e}")
+            Constants.logger(f"Failed to generate upstox token {e}")
             raise e
 
-    @retry(
-        wait_exponential_multiplier=1000,
-        wait_exponential_max=10000,
-        stop_max_attempt_number=3,
-        retry_on_exception=retry_exception,
-    )
     @timeit(MetricName="Upstox:profile")
     def profile(self):
         # create an instance of the API class
         api_instance = upstox_client.UserApi(
             upstox_client.ApiClient(self.configuration)
         )
         api_version = "2.0"  # str | API Version Header
 
         try:
             # Get profile
             api_response = api_instance.get_profile(api_version)
             profile_data = api_response.data
         except ApiException as e:
-            Constants.logger.info("error when calling UserApi->get_profile: %s\n" % e)
-            self.handle_exception(e)
+            Constants.logger("Exception when calling UserApi->get_profile: %s\n" % e)
 
         response = {
             "user_id": profile_data.user_id,
             "full_name": profile_data.user_name,
             "exchanges": profile_data.exchanges,
             "email": profile_data.email,
         }
@@ -325,18 +297,20 @@
 
         try:
             # Get Positions
             api_response = api_instance.get_positions(api_version)
             positions = [position.to_dict() for position in api_response.data]
             positions = pd.DataFrame(positions)
         except ApiException as e:
-            Constants.logger.error(
+            if "Unauthorized" in e.reason:
+                raise TokenException("Token Expired")
+            Constants.logger(
                 "Exception when calling PortfolioApi->get_positions: %s\n" % e
             )
-            self.handle_exception(e)
+            raise RetryableException(e.reason)
 
         if len(positions) == 0:
             return pd.DataFrame(columns=self.positions_column_list)
 
         positions.rename(columns={"last_price": "ltp"}, inplace=True)
 
         positions["pnl"] = positions.sell_value - positions.buy_value
@@ -358,42 +332,36 @@
 
         positions["product"] = positions["product"].replace(
             ["I", "C", "D"], ["MIS", "CNC", "NRML"]
         )
 
         if drop_cnc:
             positions = positions[positions["product"] != "CNC"]
-        existing_columns = list(positions.columns)
-        columns_to_keep = list(
-            set(self.positions_column_list).intersection(set(existing_columns))
-        )
-        return positions[columns_to_keep]
+        return positions[self.positions_column_list]
 
     @retry(
-        wait_exponential_multiplier=1000,
+        wait_exponential_multiplier=3000,
         wait_exponential_max=10000,
         stop_max_attempt_number=3,
-        retry_on_exception=retry_exception,
     )
     @timeit(MetricName="Upstox:orders")
     def orders(self, tag=None, add_ltp=True):
         # create an instance of the API class
         api_instance = upstox_client.OrderApi(
             upstox_client.ApiClient(self.configuration)
         )
         api_version = "2.0"  # str | API Version Header
 
         try:
             # Get order book
             api_response = api_instance.get_order_book(api_version)
         except ApiException as e:
-            Constants.logger.error(
+            Constants.logger(
                 "Exception when calling OrderApi->get_order_book: %s\n" % e
             )
-            self.handle_exception(e)
 
         orders = [order.to_dict() for order in api_response.data]
         orders = pd.DataFrame(orders)
         if len(orders) == 0:
             return pd.DataFrame(columns=self.orders_column_list)
 
         positions = self.positions()
@@ -431,28 +399,14 @@
         )
         orders["token"] = orders.apply(
             lambda x: self.symbol_data[f"{x['exchange']}:{x['tradingsymbol']}"][
                 "token"
             ],
             axis=1,
         )
-        orders.loc[:, "order_timestamp"] = pd.to_datetime(
-            orders.order_timestamp, format="%Y-%m-%d %H:%M:%S"
-        )
-        orders["update_timestamp"] = orders.order_timestamp
-        orders.status = orders.status.replace(
-            ["open", "cancelled", "trigger pending", "complete", "rejected"],
-            ["OPEN", "CANCELLED", "TRIGGER PENDING", "COMPLETE", "REJECTED"],
-        )
-        orders["product"] = orders["product"].replace(["D", "I"], ["CNC", "MIS"])
-        orders["product"] = np.where(
-            ((orders["product"] == "CNC") & (orders["exchange"].isin(["NFO", "BFO"]))),
-            "NRML",
-            orders["product"],
-        )
 
         return orders
 
     @retry(
         wait_exponential_multiplier=3000,
         wait_exponential_max=10000,
         stop_max_attempt_number=3,
@@ -468,18 +422,20 @@
 
         try:
             # Get User Fund And Margin
             api_response = api_instance.get_user_fund_margin(
                 api_version, segment=segment
             )
         except ApiException as e:
-            Constants.logger.error(
+            if "Unauthorized" in e.reason:
+                raise TokenException("Token Expired")
+            Constants.logger(
                 "Exception when calling UserApi->get_user_fund_margin: %s\n" % e
             )
-            self.handle_exception(e)
+            raise RetryableException(e.reason)
 
         margins = {
             "margin_used": float(api_response.data["equity"].used_margin),
             "margin_available": float(api_response.data["equity"].available_margin),
         }
         return margins
 
@@ -495,72 +451,8 @@
             "margin_used": margins["margin_used"],
             "margin_available": margins["margin_available"],
             "pnl": float(self.positions().pnl.sum()),
         }
         return response
 
     def stream_order_data(self):
-        th = threading.Thread(target=self.between_callback, daemon=True)
-        th.start()
-
-    def between_callback(self):
-        loop = asyncio.new_event_loop()
-        asyncio.set_event_loop(loop)
-
-        loop.run_until_complete(self.fetch_order_updates())
-        loop.close()
-
-    async def fetch_order_updates(self):
-        ssl_context = ssl.create_default_context()
-        ssl_context.check_hostname = False
-        ssl_context.verify_mode = ssl.CERT_NONE
-
-        # Configure OAuth2 access token for authorization: OAUTH2
-        configuration = upstox_client.Configuration()
-
-        api_version = "2.0"
-        configuration.access_token = self.access_token
-
-        # Get portfolio stream feed authorize
-        response = self.get_portfolio_stream_feed_authorize(api_version, configuration)
-
-        async with websockets.connect(
-            response.data.authorized_redirect_uri, ssl=ssl_context
-        ) as websocket:
-            print("Connection established")
-
-            # Perform WebSocket operations
-            while True:
-                message = await websocket.recv()
-                self.order_event_handler(json.dumps(message))
-
-    def get_portfolio_stream_feed_authorize(self, api_version, configuration):
-        api_instance = upstox_client.WebsocketApi(
-            upstox_client.ApiClient(configuration)
-        )
-        api_response = api_instance.get_portfolio_stream_feed_authorize(api_version)
-        return api_response
-
-    def get_quantplay_product(self, exchange, product):
-        product_map = {"D": "CNC", "I": "MIS"}
-        if product in product_map:
-            product = product_map[product]
-        if product == "CNC" and exchange in ["NFO", "BFO"]:
-            product = "NRML"
-
-        return product
-
-    def order_event_handler(self, order):
-        order = json.loads(json.loads(order))
-
-        try:
-            order["status"] = order["status"].upper()
-            if order["exchange"] in ["NSE", "BSE"]:
-                order["tradingsymbol"] = order["tradingsymbol"].replace("-EQ", "")
-            order["product"] = self.get_quantplay_product(
-                order["exchange"], order["product"]
-            )
-            Constants.logger.info("[UPDATE_RECEIVED] {}".format(order))
-            self.order_updates.put(order)
-        except Exception as e:
-            traceback.print_exc()
-            Constants.logger.error("[ORDER_UPDATE_PROCESSING_FAILED] {}".format(e))
+        pass
```

### Comparing `quantplay-1.5.80/quantplay/broker/xts.py` & `quantplay-1.5.9/quantplay/broker/xts.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,24 +7,19 @@
 import codecs
 from datetime import datetime
 
 from quantplay.broker.generics.broker import Broker
 from quantplay.utils.constant import Constants, timeit, OrderType
 from quantplay.broker.xts_utils.Connect import XTSConnect
 from quantplay.utils.pickle_utils import PickleUtils, InstrumentData
-from quantplay.exception.exceptions import (
-    InvalidArgumentException,
-    RetryableException,
-    retry_exception,
-)
+from quantplay.exception.exceptions import InvalidArgumentException
 from quantplay.broker.xts_utils.InteractiveSocketClient import OrderSocket_io
 
 from quantplay.exception.exceptions import TokenException
-import requests, time
-from retrying import retry
+import requests
 from urllib3.exceptions import InsecureRequestWarning
 
 # Suppress only the single warning from urllib3 needed.
 requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
 
 
 class XTS(Broker):
@@ -46,16 +41,14 @@
         super(XTS, self).__init__()
         self.order_updates = order_updates
 
         try:
             if wrapper:
                 self.set_wrapper(wrapper, md_wrapper)
                 self.ClientID = ClientID
-                self.wrapper.root = self.root_url
-                self.md_wrapper.root = self.root_url
             else:
                 self.login(api_key, api_secret, md_api_key, md_api_secret)
         except Exception as e:
             print(traceback.print_exc())
             raise e
 
         if load_instrument:
@@ -138,47 +131,27 @@
                 raise TokenException("Market data api credentials are invalid")
             self.ClientID = xt_core_response["result"]["userID"]
         except TokenException as e:
             raise
         except Exception as e:
             raise InvalidArgumentException("Invalid api key/secret")
 
-    def handle_exception(self, response):
-        if "data" in response and "description" in response["data"]:
-            data = response["data"]
-            if "max limit" in data["description"].lower():
-                user_id = self.profile()["user_id"]
-                print("Rate limit problem")
-                raise RetryableException(f"{user_id}: Request limit exceeded")
-        if (
-            "description" in response
-            and "Authorization not found" in response["description"]
-        ):
-            raise TokenException(response["description"])
-        if "type" in response and response["type"] == "error":
-            raise Exception("[XTS_Error]: " + response["description"])
-
-    @retry(
-        wait_exponential_multiplier=3000,
-        wait_exponential_max=10000,
-        stop_max_attempt_number=3,
-        retry_on_exception=retry_exception,
-    )
     def margins(self):
         # TODO: Edit For Dealers
 
         api_response = self.wrapper.get_balance(clientID=self.ClientID)
-        self.handle_exception(api_response)
 
         if not api_response:
             return {
                 "margin_used": 0,
                 "margin_available": 0,
             }
+
         api_response = api_response["result"]["BalanceList"][0]["limitObject"]
+
         return {
             # TODO: Get PNL
             "pnl": 0,
             "margin_used": api_response["RMSSubLimits"]["marginUtilized"],
             "margin_available": api_response["RMSSubLimits"]["netMarginAvailable"],
         }
 
@@ -195,30 +168,26 @@
             "user_id": api_response["ClientId"],
             "full_name": api_response["ClientName"],
             "segments": api_response["ClientExchangeDetailsList"],
         }
 
         return response
 
-    @retry(
-        wait_exponential_multiplier=3000,
-        wait_exponential_max=10000,
-        stop_max_attempt_number=3,
-        retry_on_exception=retry_exception,
-    )
     def orders(self, tag=None, order_type=None, add_ltp=True):
         api_response = self.wrapper.get_order_book(self.ClientID)
-        self.handle_exception(api_response)
+
+        if api_response["type"] == "error":
+            raise Exception("[XTS_Error]: " + api_response["description"])
 
         api_response = api_response["result"]
 
         orders = pd.DataFrame(api_response)
         positions = self.positions()
-        positions = positions.sort_values("product").groupby(["tradingsymbol"]).head(1)
-        if orders is None or len(orders) == 0:
+
+        if len(orders) == 0:
             return pd.DataFrame(columns=self.orders_column_list)
 
         orders.loc[:, "tradingsymbol"] = orders.TradingSymbol
         orders = pd.merge(
             orders,
             positions[["tradingsymbol", "ltp"]],
             how="left",
@@ -277,40 +246,33 @@
             ["Rejected", "Cancelled", "Filled", "New"],
             ["REJECTED", "CANCELLED", "COMPLETE", "OPEN"],
         )
         orders.loc[:, "order_type"] = orders.order_type.replace(
             ["Limit", "StopLimit", "Market"], ["LIMIT", "SL", "MARKET"]
         )
 
-        existing_columns = list(orders.columns)
-        columns_to_keep = list(
-            set(self.orders_column_list).intersection(set(existing_columns))
-        )
-        orders = orders[columns_to_keep]
+        orders = orders[self.orders_column_list]
 
         if tag:
             orders = orders[orders.tag == tag]
 
         if order_type:
             orders = orders[orders.order_type == order_type]
 
         return orders
 
-    @retry(
-        wait_exponential_multiplier=3000,
-        wait_exponential_max=10000,
-        stop_max_attempt_number=3,
-        retry_on_exception=retry_exception,
-    )
     def positions(self):
         # TODO: get sell_value, buy_value
         api_response = self.wrapper.get_position_daywise(self.ClientID)
-        self.handle_exception(api_response)
+
+        if api_response["type"] == "error":
+            raise Exception("[XTS_Error]: " + api_response["description"])
 
         api_response = api_response["result"]["positionList"]
+
         positions = pd.DataFrame(api_response)
 
         if len(positions) == 0:
             return pd.DataFrame(columns=self.positions_column_list)
 
         positions.rename(
             columns={
@@ -357,19 +319,15 @@
         positions.loc[:, "option_type"] = np.where(
             "CE" == positions.tradingsymbol.str[-2:], "CE", positions.option_type
         )
         positions.loc[:, "option_type"] = np.where(
             positions.exchange.isin(["NFO", "BFO"]), positions.option_type, None
         )
 
-        existing_columns = list(positions.columns)
-        columns_to_keep = list(
-            set(self.positions_column_list).intersection(set(existing_columns))
-        )
-        return positions[columns_to_keep]
+        return positions[self.positions_column_list]
 
     def get_quantplay_symbol(self, symbol):
         if symbol in self.broker_symbol_map:
             return self.broker_symbol_map[symbol]
         return symbol
 
     def get_ltps(self, symbols):
@@ -380,60 +338,53 @@
             }
             for x in symbols
         ]
         api_response = self.md_wrapper.get_quote(
             Instruments=instruments,
             xtsMessageCode=1512,
             publishFormat="JSON",
-        )
-
-        if "type" in api_response and api_response["type"] == "error":
-            raise TokenException(api_response["description"])
-        api_response = api_response["result"]
+        )["result"]
 
         ltp_json = api_response["listQuotes"]
 
         ltp = [json.loads(x) for x in ltp_json]
 
         ltp = {x["ExchangeInstrumentID"]: x["LastTradedPrice"] for x in ltp}
         return ltp
 
     def get_exchange_code(self, exchange):
         exchange_code_map = {
             "NSE": 1,
             "NFO": 2,
-            "BFO": 12,
-            "BSE": 11,
             "NSECM": 1,
             "NSEFO": 2,
             "NSECD": 3,
             "BSECM": 11,
             "BSEFO": 12,
         }
 
         if exchange not in exchange_code_map:
             raise KeyError(
-                f"INVALID_EXCHANGE: Exchange {exchange} not in ['NSE', 'NFO', 'NSECD', 'BSECM', 'BSEFO']"
+                "INVALID_EXCHANGE: Exchange not in ['NSE', 'NFO', 'NSECD', 'BSECM', 'BSEFO']"
             )
 
         return exchange_code_map[exchange]
 
     def get_exchange_name(self, exchange):
         exchange_code_map = {
             "NSE": "NSECM",
             "NFO": "NSEFO",
-            "BFO": "BSEFO",
             "NSECD": "NSECD",
             "BSECM": "BSECM",
             "BSEFO": "BSEFO",
         }
 
         if exchange not in exchange_code_map:
             raise KeyError(
-                f"INVALID_EXCHANGE: Exchange {exchange} not in ['NSE', 'NFO', 'NSECD', 'BSECM', 'BSEFO']"
+                "INVALID_EXCHANGE: Exchange not in ['NSE', 'NFO', 'NSECD', 'BSECM', 'BSEFO']"
             )
 
         return exchange_code_map[exchange]
 
     def get_ltp(self, exchange=None, tradingsymbol=None):
         exchange_code = self.get_exchange_code(exchange)
         exchange_token = self.symbol_data[f"{exchange}:{tradingsymbol}"][
```

### Comparing `quantplay-1.5.80/quantplay/broker/xts_utils/Connect.py` & `quantplay-1.5.9/quantplay/broker/xts_utils/Connect.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/broker/xts_utils/Exception.py` & `quantplay-1.5.9/quantplay/broker/xts_utils/Exception.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/broker/xts_utils/InteractiveSocketClient.py` & `quantplay-1.5.9/quantplay/broker/xts_utils/InteractiveSocketClient.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/broker/xts_utils/MarketDataSocketClient.py` & `quantplay-1.5.9/quantplay/broker/xts_utils/MarketDataSocketClient.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/brokerage/generics/broker.py` & `quantplay-1.5.9/quantplay/brokerage/generics/broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/brokerage/zerodha/ZBroker.py` & `quantplay-1.5.9/quantplay/brokerage/zerodha/ZBroker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/config/qplay_config.py` & `quantplay-1.5.9/quantplay/config/qplay_config.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/create_sample_data.py` & `quantplay-1.5.9/quantplay/create_sample_data.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/data_modify_script.py` & `quantplay-1.5.9/quantplay/data_modify_script.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/date_fix.py` & `quantplay-1.5.9/quantplay/date_fix.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/exception/exceptions.py` & `quantplay-1.5.9/quantplay/exception/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,7 @@
 
 class WrongLibrarySetup(Exception):
     code = "501"
 
     def __init__(self, message):
         # Call the base class constructor with the parameters it needs
         super(WrongLibrarySetup, self).__init__(message)
-
-
-class BrokerException(Exception):
-    code = "510"
-
-    def __init__(self, message):
-        # Call the base class constructor with the parameters it needs
-        super(BrokerException, self).__init__(message)
```

### Comparing `quantplay-1.5.80/quantplay/indicators/Indicator.py` & `quantplay-1.5.9/quantplay/indicators/Indicator.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/model/exchange/instrument.py` & `quantplay-1.5.9/quantplay/model/exchange/instrument.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/model/exchange/order.py` & `quantplay-1.5.9/quantplay/model/exchange/order.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/model/exchange/tick.py` & `quantplay-1.5.9/quantplay/model/exchange/tick.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/options/analytics.py` & `quantplay-1.5.9/quantplay/options/analytics.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/order_execution/execution_algorithm.py` & `quantplay-1.5.9/quantplay/order_execution/execution_algorithm.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/order_execution/mean_price.py` & `quantplay-1.5.9/quantplay/order_execution/mean_price.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/reporting/strategy_report.py` & `quantplay-1.5.9/quantplay/reporting/strategy_report.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/reporting/visuals.py` & `quantplay-1.5.9/quantplay/reporting/visuals.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/services/market.py` & `quantplay-1.5.9/quantplay/services/market.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,27 +16,25 @@
 from quantplay.utils.constant import Constants
 from datetime import datetime
 
 
 class Market:
     BASE_URL = "https://7tpcay1yyk.execute-api.ap-south-1.amazonaws.com/prod/"
 
-    GET_SYMBOLS_URL = "{}get_symbols".format(BASE_URL)
+    GET_SYMBOLS_URL =  "{}get_symbols".format(BASE_URL)
     EXPIRY_DATA_URL = "{}nearest_expiry".format(BASE_URL)
     SECURITY_DATA_URL = "{}get_security_delivery".format(BASE_URL)
 
     def __init__(self):
         config = QuantplayConfig.get_config()
         self.base_path = "{}/.quantplay/".format(expanduser("~"))
         self.nse_equity_path = "{}/.quantplay/NSE_EQ/".format(expanduser("~"))
         self.nse_opt_path = "{}/.quantplay/NSE_OPT/".format(expanduser("~"))
         self.nse_fut_path = "{}/.quantplay/NSE_FUT/".format(expanduser("~"))
-        self.nse_market_data_path = "{}/.quantplay/NSE_MARKET_DATA/".format(
-            expanduser("~")
-        )
+        self.nse_market_data_path = "{}/.quantplay/NSE_MARKET_DATA/".format(expanduser("~"))
         self.mcx_path = "{}/.quantplay/MCX/".format(expanduser("~"))
 
         if "DEFAULT" in config and "base_path" in config["DEFAULT"]:
             self.base_path = config["DEFAULT"]["base_path"]
         if "DEFAULT" in config and "nse_equity_path" in config["DEFAULT"]:
             self.nse_equity_path = config["DEFAULT"]["nse_equity_path"]
         if "DEFAULT" in config and "nse_opt_path" in config["DEFAULT"]:
@@ -44,99 +42,176 @@
         if "DEFAULT" in config and "nse_fut_path" in config["DEFAULT"]:
             self.nse_fut_path = config["DEFAULT"]["nse_fut_path"]
         if "DEFAULT" in config and "nse_market_data_path" in config["DEFAULT"]:
             self.nse_market_data_path = config["DEFAULT"]["nse_market_data_path"]
         if "DEFAULT" in config and "mcx_path" in config["DEFAULT"]:
             self.mcx_path = config["DEFAULT"]["mcx_path"]
 
+
     def initialize_broker(self, broker_name=None):
         config = QuantplayConfig.get_config()
 
-        if (
-            "DEFAULT" in config
-            and "preferred_broker" in config["DEFAULT"]
-            and broker_name is None
-        ):
+        if "DEFAULT" in config and "preferred_broker" in config["DEFAULT"] and broker_name is None:
             preferred_broker = config["DEFAULT"]["preferred_broker"]
-            Constants.logger.info(
-                "Using {} as preferred broker".format(preferred_broker)
-            )
+            Constants.logger.info("Using {} as preferred broker".format(preferred_broker))
             broker_name = preferred_broker
 
         if broker_name is None:
             raise Exception("please provide broker_name to initialize broker")
 
         if broker_name == "Zerodha":
             self.broker = Zerodha(wrapper=config["DEFAULT"]["zerodha_wrapper"])
         elif broker_name == "AngelOne":
             self.broker = AngelOne()
         elif broker_name == "Motilal":
             self.broker = Motilal()
         else:
             raise Exception("broker [{}] not supported".format(broker_name))
 
-    def symbols(self, universe=None, filters={}):
+    def get_nearest_expiry_data(
+        self,
+        symbols=[],
+        days_offset=0,
+        security_type=None,
+        depth=None,
+        after_date=None,
+        before_date=None,
+    ):
         credentials = QuantplayConfig.get_credentials()
         if "DEFAULT" not in credentials or "access_token" not in credentials["DEFAULT"]:
             raise AccessDeniedException(
                 "Access Denied, please signin using [quantplay user signin]"
             )
+
+        access_token = credentials["DEFAULT"]["access_token"]
+        input = {
+            "access_token": access_token,
+            "days_offset": days_offset,
+        }
+
+        if symbols:
+            input["symbols"] = symbols
+        if security_type:
+            input["security_type"] = security_type
+        if depth is not None:
+            input["depth"] = depth
+
+        x = requests.post(Market.EXPIRY_DATA_URL, data=json.dumps(input))
+        response = json.loads(x.text)
+
+        if "error" in response and response["error"] == True:
+            print(response["message"])
+            raise Exception(response["message"])
+
+        data = pd.DataFrame(response["data"])
+
+        # TODO Move after date to API input
+        if after_date is not None:
+            data = data[data.date >= after_date]
+        if before_date is not None:
+            data = data[data.date <= before_date]
+        return data
+
+    def add_expiry(
+        self, data, security_type=None, days_offset=0
+    ):
+        columns_to_be_added = ["expiry_date", "strike_spread"]
+
+        for column in columns_to_be_added:
+            if column in data.columns:
+                data = data.drop([column], axis=1)
+
+        symbols = [
+            MarketConstants.INDEX_SYMBOL_TO_DERIVATIVE_SYMBOL_MAP.get(symbol, symbol)
+            for symbol in data.symbol.unique()
+        ]
+
+
+        expiry_data = self.get_nearest_expiry_data(
+            symbols=symbols,
+            security_type=security_type,
+            days_offset=days_offset,
+        )
+
+        data.loc[:, "date_only"] = pd.to_datetime(data.date.dt.date)
+        expiry_data.loc[:, "expiry_date"] = pd.to_datetime(expiry_data.expiry_date)
+        expiry_data.loc[:, "date_only"] = pd.to_datetime(expiry_data.date)
+
+        for (
+            idx_derivative_symbol,
+            idx_symbol,
+        ) in MarketConstants.DERIVATIVE_SYMBOL_TO_INDEX_SYMBOL_MAP.items():
+            expiry_data.loc[:, "symbol"] = expiry_data["symbol"].replace(
+                [idx_derivative_symbol], idx_symbol
+            )
+
+        data = pd.merge(
+            data,
+            expiry_data[["date_only", "symbol", "expiry_date", "strike_gap"]],
+            how="left",
+            left_on=["symbol", "date_only"],
+            right_on=["symbol", "date_only"],
+        )
+        return data
+
+    def symbols(self, universe=None, filters={}):
+        credentials = QuantplayConfig.get_credentials()
+        if "DEFAULT" not in credentials or "access_token" not in credentials["DEFAULT"]:
+            raise AccessDeniedException("Access Denied, please signin using [quantplay user signin]")
         input = {}
         if universe != None:
             input["universe"] = universe
 
         access_token = credentials["DEFAULT"]["access_token"]
-        input["access_token"] = access_token
-        input["filters"] = filters
+        input['access_token'] = access_token
+        input['filters'] = filters
 
         x = requests.post(Market.GET_SYMBOLS_URL, data=json.dumps(input))
         response = json.loads(x.text)
 
         if "error" in response and response["error"] == True:
             print(response["message"])
             raise Exception(response["message"])
 
-        return response["data"]
+        return response['data']
 
     def add_security_delivery_data(self, trades):
         credentials = QuantplayConfig.get_credentials()
         if "DEFAULT" not in credentials or "access_token" not in credentials["DEFAULT"]:
-            raise AccessDeniedException(
-                "Access Denied, please signin using [quantplay user signin]"
-            )
+            raise AccessDeniedException("Access Denied, please signin using [quantplay user signin]")
 
         access_token = credentials["DEFAULT"]["access_token"]
 
-        data = copy.deepcopy(trades[["symbol", "date"]])
-        data.loc[:, "date"] = trades.date.dt.date.astype(str)
+        data = copy.deepcopy(trades[['symbol', 'date']])
+        data.loc[:, 'date'] = trades.date.dt.date.astype(str)
 
         request_input = {}
-        request_input["access_token"] = access_token
-        request_input["data"] = data.to_dict("records")
+        request_input['access_token'] = access_token
+        request_input['data'] = data.to_dict('records')
 
         x = requests.post(Market.SECURITY_DATA_URL, data=json.dumps(request_input))
 
         response = json.loads(x.text)
-        df = pd.DataFrame(response["data"])
-        trades.loc[:, "yesterdays_delivery_ratio"] = df.yesterdays_delivery_ratio
-        trades.loc[:, "delivery_ratio"] = df.delivery_ratio
+        df = pd.DataFrame(response['data'])
+        trades.loc[:, 'yesterdays_delivery_ratio'] = df.yesterdays_delivery_ratio
+        trades.loc[:, 'delivery_ratio'] = df.delivery_ratio
 
     def future_symbol(self, trade_data):
         trades = copy.deepcopy(trade_data)
         trades.loc[:, "tradingsymbol"] = trades["symbol"].replace(
             MarketConstants.INDEX_SYMBOL_TO_DERIVATIVE_SYMBOL_MAP
         )
 
         trades.loc[:, "tradingsymbol"] = trades.tradingsymbol + trades[
             "expiry_date"
         ].dt.strftime("%y").astype(str)
 
-        trades.loc[:, "tradingsymbol"] = (
-            trades.tradingsymbol + trades["expiry_date"].dt.strftime("%b").str.upper()
-        )
+        trades.loc[:, "tradingsymbol"] = trades.tradingsymbol + \
+                                         trades["expiry_date"].dt.strftime("%b").str.upper()
+
 
         trades.loc[:, "tradingsymbol"] = trades.tradingsymbol + "FUT"
         trades.loc[:, "security_type"] = "FUT"
 
         return trades
 
     def option_symbol(self, trade_data, price_column=None, option_type=None):
@@ -294,32 +369,29 @@
 
     def data_by_path(self, interval=None, symbols=None, path=None):
         df = DataUtils.load_data_using_pandas(
             stocks=symbols, interval=interval, path=path
         )
 
         return df
-
     def mcx_data(self, interval=None, symbols=None):
         df = DataUtils.load_data_using_pandas(
             stocks=symbols, interval=interval, path=self.mcx_path
         )
         return df
 
     def data(self, interval=None, symbols_by_security_type=None, **kwargs):
         security_type_data_path = {
             "EQ": self.nse_equity_path,
             "FUT": self.nse_fut_path,
             "OPT": self.nse_opt_path,
         }
         if "path_suffix" in kwargs:
             for key in security_type_data_path:
-                security_type_data_path[key] = (
-                    security_type_data_path[key] + kwargs["path_suffix"]
-                )
+                security_type_data_path[key] = security_type_data_path[key] + kwargs["path_suffix"]
 
         dfs = []
         for security_type, symbols in symbols_by_security_type.items():
 
             print(
                 f"Loading {security_type} data for {len(set(symbols))} symbols, interval {interval}"
             )
@@ -359,15 +431,15 @@
     @staticmethod
     def merge_price(
         trades,
         data,
         time=None,
         column_name=None,
         merge_on_columns=["symbol", "date_only"],
-        column_type="close",
+        column_type='close'
     ):
         filter_data = data[
             data.assign(Time=data["date"].dt.time.astype(str))["Time"].str.match(time)
         ]
 
         filter_data.loc[:, column_name] = filter_data[column_type]
         trades = pd.merge(
@@ -395,23 +467,32 @@
         data.loc[:, "intraday_high"] = data.groupby(
             ["symbol", "date_only"]
         ).intraday_high.transform(max)
         data.loc[:, "intraday_low"] = data.groupby(
             ["symbol", "date_only"]
         ).intraday_low.transform(min)
 
-    def day_candle(self, market_data):
-        day_candle = (
-            market_data.groupby(["symbol", pd.Grouper(key="date", freq="1d")])
-            .agg(
-                {
-                    "open": "first",
-                    "high": "max",
-                    "low": "min",
-                    "close": "last",
-                    "volume": "sum",
-                }
-            )
-            .reset_index()
+    def nearest_expiry(self, symbol=None, security_type=None, days_offset=0):
+        symbol = MarketConstants.INDEX_SYMBOL_TO_DERIVATIVE_SYMBOL_MAP[symbol]
+        data = self.get_nearest_expiry_data(
+            symbols=[symbol],
+            security_type=security_type,
+            days_offset=days_offset,
         )
+        today_date = str(datetime.now().date())
+        data = data[data.date == today_date]
+
+        data = data.to_dict('records')[0]
+        data['expiry_date'] = datetime.strptime(data['expiry_date'], '%Y-%m-%d')
+
+        return data
+
+    def day_candle(self, market_data):
+        day_candle = market_data.groupby(["symbol", pd.Grouper(key='date', freq="1d")]).agg({
+            "open": "first",
+            "high": "max",
+            "low": "min",
+            "close": "last",
+            "volume": "sum"
+        }).reset_index()
 
-        return day_candle
+        return day_candle
```

### Comparing `quantplay-1.5.80/quantplay/services/tradelens.py` & `quantplay-1.5.9/quantplay/services/tradelens.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/strategies/options/intraday/ladder.py` & `quantplay-1.5.9/quantplay/strategies/options/intraday/ladder.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/strategies/options/intraday/musk.py` & `quantplay-1.5.9/quantplay/strategies/options/intraday/musk.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/strategy/base.py` & `quantplay-1.5.9/quantplay/strategy/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from quantplay.utils.constant import Constants, OrderType, IntervalAttribute
 from quantplay.service import market, backtesting
 from quantplay.utils.exchange import Market as MarketConstants
 from quantplay.model.exchange.order import QuantplayExchangeOrder
 from quantplay.exception.exceptions import StrategyInvocationException
 import datetime
 import pandas as pd
-import polars as pl
 from datetime import timedelta
 
 pd.options.mode.chained_assignment = None  # default='warn'
 
 
 class QuantplayAlgorithm:
     MAX_LEN_FOR_STRATEGY_TAG = 15
@@ -31,19 +30,16 @@
             raise Exception("Strategy must have 'execution_algo' attribute")
 
         if not hasattr(self, "order_type"):
             raise Exception("Strategy must have 'order_type' attribute")
 
         supported_orders = [OrderType.market, OrderType.limit]
         if self.order_type not in supported_orders:
-            raise Exception(
-                "order type {} not supported, please use {}".format(
-                    self.order_type, supported_orders
-                )
-            )
+            raise Exception("order type {} not supported, please use {}".format(self.order_type,
+                                                                                supported_orders))
         self.validate()
 
     def validate(self):
         if not hasattr(self, "interval"):
             raise Exception("Strategy must have an 'interval' attribute.")
 
         if not hasattr(self, "exchange_to_trade_on"):
@@ -123,138 +119,111 @@
         trades["uuid"] = uuids[g.ngroup()]
 
     def filter_uuids_not_matching_count(self, trades):
         """Filters out trades with uuids not matching the self.exact_number_of_order_per_uuid count"""
         self.add_orders_uuid(trades, self.columns_for_uuid)
 
         trades.loc[
-            :, "exact_number_of_orders_per_uuid"
+        :, "exact_number_of_orders_per_uuid"
         ] = self.exact_number_of_orders_per_uuid
 
         return trades[
             trades["uuid"].map(trades["uuid"].value_counts())
             == trades["exact_number_of_orders_per_uuid"]
-        ]
+            ]
 
     def live_orders(self, market_data, tick_time):
         """Returns list of QuantplayExchangeOrder tuples
         which are to be executed immediately.
         """
         try:
             trades = self.get_trades(market_data)
 
             if len(trades) == 0:
-                return {"entry_orders": trades}
+                return {
+                    "entry_orders": trades
+                }
 
-            interval_minutes = int(
-                Constants.interval_attributes[self.interval][IntervalAttribute.seconds]
-                / 60
-            )
+            interval_minutes = int(Constants.interval_attributes[self.interval][IntervalAttribute.seconds] / 60)
 
             trades.loc[:, "tag"] = self.strategy_tag
             trades.loc[:, "strategy_type"] = self.strategy_type
-            trades.loc[:, "order_timestamp"] = trades.date.apply(
-                lambda x: x + timedelta(minutes=interval_minutes)
-            )
+            trades.loc[:, 'order_timestamp'] = trades.date.apply(lambda x: x + timedelta(minutes=interval_minutes))
 
             exit_orders = []
             if "exit_time" in trades.columns:
                 exit_trades = trades[trades.exit_time == tick_time]
                 exit_trades = exit_trades.to_dict("records")
                 exit_orders = QuantplayExchangeOrder.get_exchange_orders(
-                    exit_trades,
-                    order_type=self.order_type,
-                    exchange=self.exchange_to_trade_on,
-                    execution_algo=self.execution_algo,
-                )
+                        exit_trades,
+                        order_type=self.order_type,
+                        exchange=self.exchange_to_trade_on,
+                        execution_algo=self.execution_algo,
+                    )
 
             entry_trades = trades[trades.date == tick_time]
             entry_trades = entry_trades.to_dict("records")
             entry_orders = QuantplayExchangeOrder.get_exchange_orders(
                 entry_trades,
                 order_type=self.order_type,
                 exchange=self.exchange_to_trade_on,
                 execution_algo=self.execution_algo,
             )
 
-            return {"entry_orders": entry_orders, "exit_orders": exit_orders}
+            return {
+                "entry_orders": entry_orders,
+                "exit_orders": exit_orders
+            }
         except Exception as e:
             raise StrategyInvocationException(
                 f"Failed to invoke strategy {self.strategy_tag}"
             ) from e
 
-    def get_nearest_expiry_data(
-        self, symbols, days_offset, after_date, before_date
-    ) -> pl.DataFrame:
-        expiry_data = pl.read_parquet(
-            f"{market.nse_market_data_path}expiry_data.parquet"
-        )
-
-        expiry_data = expiry_data.filter(
-            pl.col("expiry_date") >= pl.col("date").add(timedelta(days=days_offset))
-        )
-        expiry_data = expiry_data.filter(pl.col("symbol").is_in(symbols))
-        expiry_data = (
-            expiry_data.sort("expiry_date")
-            .group_by(["symbol", "date"])
-            .first()
-            .sort("date")
-        )
-        if after_date is not None:
-            expiry_data = expiry_data.filter(
-                pl.col("date").dt.date().cast(pl.String) >= after_date
-            )
-        if before_date is not None:
-            expiry_data = expiry_data.filter(
-                pl.col("date").dt.date().cast(pl.String) <= before_date
-            )
-
-        return expiry_data
-
-    def add_derivative_symbols(self, mode="backtest"):
+    def add_derivative_symbols(self, mode='backtest'):
         opt_derivative_symbols, fut_derivative_symbols = set(), set()
 
         equity_symbols = []
         if "EQ" in self.stream_symbols_by_security_type:
             equity_symbols = [
-                MarketConstants.INDEX_SYMBOL_TO_DERIVATIVE_SYMBOL_MAP.get(
-                    symbol, symbol
-                )
+                MarketConstants.INDEX_SYMBOL_TO_DERIVATIVE_SYMBOL_MAP.get(symbol, symbol)
                 for symbol in self.stream_symbols_by_security_type["EQ"]
             ]
 
         if hasattr(self, "option_nearest_expiry_offset"):
             depth = None
             after_date = None
             before_date = None
             if hasattr(self, "option_chain_depth"):
                 depth = self.option_chain_depth
             if hasattr(self, "backtest_after_date"):
                 after_date = self.backtest_after_date
             if hasattr(self, "backtest_before_date"):
                 before_date = self.backtest_before_date
-            if mode == "prod":
+            if mode == 'prod':
                 after_date = str(datetime.datetime.now().date())
                 before_date = str(datetime.datetime.now().date())
 
-            self.opt_expiry_data = self.get_nearest_expiry_data(
+            self.opt_expiry_data = market.get_nearest_expiry_data(
                 symbols=equity_symbols,
                 days_offset=self.option_nearest_expiry_offset,
+                security_type="OPT",
+                depth=depth,
                 after_date=after_date,
                 before_date=before_date,
             )
-            opt_expiry_data_records = self.opt_expiry_data.to_dicts()
+            opt_expiry_data_records = self.opt_expiry_data.to_dict("records")
             for record in opt_expiry_data_records:
                 (symbol, expiry_date, strike_gap, lowest_strike, highest_strike,) = (
                     record["symbol"],
                     record["expiry_date"],
                     int(record["strike_gap"]),
                     int(record["lowest_strike_price"]),
                     int(record["highest_strike_price"]),
                 )
+                expiry_date = datetime.date.fromisoformat(expiry_date)
                 formatted_expiry_date = market.format_expiry_date(
                     expiry_date, security_type="OPT"
                 )
                 ce_symbols = [
                     symbol + formatted_expiry_date + str(strike) + "CE"
                     for strike in range(lowest_strike, highest_strike, strike_gap)
                 ]
```

### Comparing `quantplay-1.5.80/quantplay/utils/config_util.py` & `quantplay-1.5.9/quantplay/utils/config_util.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/utils/constant.py` & `quantplay-1.5.9/quantplay/utils/constant.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/utils/data_utils.py` & `quantplay-1.5.9/quantplay/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/utils/exchange.py` & `quantplay-1.5.9/quantplay/utils/exchange.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/utils/number_utils.py` & `quantplay-1.5.9/quantplay/utils/number_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/utils/pickle_utils.py` & `quantplay-1.5.9/quantplay/utils/pickle_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/utils/selenium_utils.py` & `quantplay-1.5.9/quantplay/utils/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/utils/transaction_utils.py` & `quantplay-1.5.9/quantplay/utils/transaction_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/quantplay/wrapper/aws/s3.py` & `quantplay-1.5.9/quantplay/wrapper/aws/s3.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,10 @@
 import boto3
 import pandas as pd
 import os
-from boto3.s3.transfer import TransferConfig
-from threading import Lock
-from quantplay.utils.constant import Constants
-
-lock = Lock()
-
-TransferConfig(use_threads=False)
 
 
 class S3Bucket:
     quantplay_market_data = "quantplay-market-data"
 
 
 class S3Utils:
@@ -19,24 +12,15 @@
 
     @staticmethod
     def read_csv(bucket, key, read_from_local=True):
         full_path = f"/tmp/{bucket}/{key}"
         try:
             if not read_from_local:
                 raise Exception("read from local is false")
-            try:
-                lock.acquire()
-                data = pd.read_csv(full_path)
-                return data
-            except Exception as e:
-                Constants.logger.error(f"[S3_READ_FAILED] failed to read from s3")
-                lock.release()
-                raise
-            lock.release()
-
+            return pd.read_csv(full_path)
         except Exception as e:
             print("Data not found for {}".format(key))
         print("fetching bucket from s3 {} key {}".format(bucket, key))
         client = boto3.client("s3")
         raw_stream = client.get_object(Bucket=bucket, Key=key)
         content = raw_stream["Body"].read().decode("utf-8")
```

### Comparing `quantplay-1.5.80/quantplay.egg-info/PKG-INFO` & `quantplay-1.5.9/quantplay.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantplay
-Version: 1.5.80
+Version: 1.5.9
 Summary: This python package will be stored in AWS CodeArtifact
 Home-page: 
 Author: 
 Author-email: 
 License: MIT
 
 # Quantplay Alpha playground
```

### Comparing `quantplay-1.5.80/quantplay.egg-info/SOURCES.txt` & `quantplay-1.5.9/quantplay.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,41 +3,38 @@
 setup.py
 quantplay/__init__.py
 quantplay/create_sample_data.py
 quantplay/data_modify_script.py
 quantplay/date_fix.py
 quantplay/service.py
 quantplay/strategy.py
+quantplay/strategy_run.py
 quantplay.egg-info/PKG-INFO
 quantplay.egg-info/SOURCES.txt
 quantplay.egg-info/dependency_links.txt
 quantplay.egg-info/requires.txt
 quantplay.egg-info/top_level.txt
 quantplay/backtest/__init__.py
 quantplay/backtest/backtest_trades.py
 quantplay/broker/__init__.py
 quantplay/broker/aliceblue.py
 quantplay/broker/angelone.py
 quantplay/broker/broker_client.py
 quantplay/broker/client.py
-quantplay/broker/five_paisa.py
 quantplay/broker/flattrade.py
-quantplay/broker/icici.py
 quantplay/broker/iifl.py
 quantplay/broker/iifl_xts.py
 quantplay/broker/kite_utils.py
 quantplay/broker/motilal.py
 quantplay/broker/noren.py
 quantplay/broker/shoonya.py
 quantplay/broker/symphony.py
 quantplay/broker/upstox.py
 quantplay/broker/xts.py
 quantplay/broker/zerodha.py
-quantplay/broker/auto_login/__init__.py
-quantplay/broker/auto_login/aliceblue.py
 quantplay/broker/finvasia_utils/__init__.py
 quantplay/broker/finvasia_utils/fa_noren.py
 quantplay/broker/ft_utils/__init__.py
 quantplay/broker/ft_utils/flattrade_utils.py
 quantplay/broker/ft_utils/ft_noren.py
 quantplay/broker/generics/__init__.py
 quantplay/broker/generics/broker.py
@@ -45,22 +42,26 @@
 quantplay/broker/uplink/uplink_utils.py
 quantplay/broker/xts_utils/Connect.py
 quantplay/broker/xts_utils/Exception.py
 quantplay/broker/xts_utils/InteractiveSocketClient.py
 quantplay/broker/xts_utils/MarketDataSocketClient.py
 quantplay/broker/xts_utils/__init__.py
 quantplay/brokerage/__init__.py
+quantplay/brokerage/angelone/__init__.py
+quantplay/brokerage/angelone/angel_broker.py
 quantplay/brokerage/generics/__init__.py
 quantplay/brokerage/generics/broker.py
 quantplay/brokerage/zerodha/ZBroker.py
 quantplay/brokerage/zerodha/__init__.py
 quantplay/config/__init__.py
 quantplay/config/qplay_config.py
 quantplay/exception/__init__.py
 quantplay/exception/exceptions.py
+quantplay/executor/__init__.py
+quantplay/executor/strategy_executor.py
 quantplay/indicators/Indicator.py
 quantplay/indicators/__init__.py
 quantplay/indicators/atr.py
 quantplay/model/__init__.py
 quantplay/model/exchange/__init__.py
 quantplay/model/exchange/instrument.py
 quantplay/model/exchange/order.py
@@ -105,10 +106,12 @@
 quantplay/wrapper/__init__.py
 quantplay/wrapper/aws/__init__.py
 quantplay/wrapper/aws/s3.py
 test/__init__.py
 test/broker/__init__.py
 test/broker/finvasia.py
 test/broker/motilal.py
+test/executor/__init__.py
+test/executor/strategy_executor.py
 test/strategy/__init__.py
 test/strategy/base.py
 test/strategy/sample_strategy.py
```

### Comparing `quantplay-1.5.80/setup.py` & `quantplay-1.5.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-from pathlib import Path
+from path import Path
 from setuptools import setup, find_packages
 
 
 def is_requirement(s: str) -> bool:
     """Returns true if the string is a valid requirement.
     For the requirement to be valid, it must be non empty
     and must not start from - or #.
@@ -17,15 +17,15 @@
     for line in Path("requirements.txt").read_text().splitlines()
     if is_requirement(line)
 ]
 
 setup(
     name="quantplay",
     long_description=Path("README.md").read_text(),
-    version="1.5.80",
+    version="1.5.9",
     setup_requires=["pytest-runner"],
     install_requires=requirements,
     tests_require=[],
     packages=find_packages(),
     url="",
     license="MIT",
     author="",
```

### Comparing `quantplay-1.5.80/test/broker/motilal.py` & `quantplay-1.5.9/test/broker/motilal.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.80/test/strategy/sample_strategy.py` & `quantplay-1.5.9/test/strategy/sample_strategy.py`

 * *Files identical despite different names*

