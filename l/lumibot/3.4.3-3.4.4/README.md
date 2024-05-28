# Comparing `tmp/lumibot-3.4.3.tar.gz` & `tmp/lumibot-3.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumibot-3.4.3.tar", last modified: Fri May 24 17:43:57 2024, max compression
+gzip compressed data, was "lumibot-3.4.4.tar", last modified: Tue May 28 07:37:00 2024, max compression
```

## Comparing `lumibot-3.4.3.tar` & `lumibot-3.4.4.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.423857 lumibot-3.4.3/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    35130 2024-03-18 04:35:37.000000 lumibot-3.4.3/LICENSE
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-05-24 17:43:57.423782 lumibot-3.4.3/PKG-INFO
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3861 2024-03-18 04:35:37.000000 lumibot-3.4.3/README.md
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.397703 lumibot-3.4.3/lumibot/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      693 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/__init__.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.400475 lumibot-3.4.3/lumibot/backtesting/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      371 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/backtesting/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      387 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/backtesting/alpaca_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      417 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/backtesting/alpha_vantage_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    31699 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/backtesting/backtesting_broker.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      244 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/backtesting/ccxt_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      388 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/backtesting/pandas_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    14652 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/backtesting/polygon_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      344 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/backtesting/yahoo_backtesting.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.402704 lumibot-3.4.3/lumibot/brokers/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      158 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/brokers/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    18630 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/brokers/alpaca.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    44490 2024-05-24 16:33:35.000000 lumibot-3.4.3/lumibot/brokers/broker.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    30406 2024-04-16 22:57:26.000000 lumibot-3.4.3/lumibot/brokers/ccxt.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    47384 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/brokers/interactive_brokers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    29851 2024-05-24 16:33:35.000000 lumibot-3.4.3/lumibot/brokers/tradier.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.406234 lumibot-3.4.3/lumibot/data_sources/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      492 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/data_sources/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    12688 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/data_sources/alpaca_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5094 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/data_sources/alpha_vantage_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    10614 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/data_sources/ccxt_backtesting_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7647 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/data_sources/ccxt_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    19315 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/data_sources/data_source.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2944 2024-04-03 02:08:33.000000 lumibot-3.4.3/lumibot/data_sources/data_source_backtesting.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      557 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/data_sources/exceptions.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    11836 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/data_sources/interactive_brokers_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15521 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/data_sources/pandas_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    11734 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/data_sources/tradier_data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7022 2024-04-10 20:12:46.000000 lumibot-3.4.3/lumibot/data_sources/yahoo_data.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.408550 lumibot-3.4.3/lumibot/entities/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      230 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/entities/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     9605 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/entities/asset.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5993 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/entities/bar.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    10205 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/entities/bars.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21849 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/entities/data.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      182 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/entities/dataline.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    28502 2024-05-24 16:33:35.000000 lumibot-3.4.3/lumibot/entities/order.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4646 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/entities/position.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1920 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/entities/trading_fee.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.411294 lumibot-3.4.3/lumibot/example_strategies/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)        0 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/example_strategies/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5551 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/example_strategies/ccxt_backtesting_example.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5098 2024-04-16 22:57:26.000000 lumibot-3.4.3/lumibot/example_strategies/crypto_important_functions.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2613 2024-04-10 20:12:46.000000 lumibot-3.4.3/lumibot/example_strategies/options_hold_to_expiry.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1226 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/example_strategies/simple_start_single_file.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2220 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/example_strategies/stock_bracket.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1895 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/example_strategies/stock_buy_and_hold.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5137 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/example_strategies/stock_diversified_leverage.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2980 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/example_strategies/stock_limit_and_trailing_stops.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     6476 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/example_strategies/stock_momentum.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2426 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/example_strategies/stock_oco.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    12862 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/example_strategies/strangle.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.413462 lumibot-3.4.3/lumibot/strategies/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       79 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/strategies/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    53746 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/strategies/_strategy.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)   153357 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/strategies/strategy.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    39943 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/strategies/strategy_executor.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.417320 lumibot-3.4.3/lumibot/tools/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1321 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/tools/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    25331 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/tools/black_scholes.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21351 2024-04-07 08:25:48.000000 lumibot-3.4.3/lumibot/tools/ccxt_data_store.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      485 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/tools/debugers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2017 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/tools/decorators.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7570 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/tools/helpers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    26283 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/tools/indicators.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1017 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/tools/lumibot_time.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1342 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/tools/pandas.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21338 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/tools/polygon_helper.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1866 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/tools/types.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    15762 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/tools/yahoo_helper.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.417749 lumibot-3.4.3/lumibot/traders/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       27 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/traders/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7997 2024-05-24 15:40:21.000000 lumibot-3.4.3/lumibot/traders/trader.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.418426 lumibot-3.4.3/lumibot/trading_builtins/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       87 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/trading_builtins/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3261 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/trading_builtins/custom_stream.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1975 2024-03-18 04:35:37.000000 lumibot-3.4.3/lumibot/trading_builtins/safe_list.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.423444 lumibot-3.4.3/lumibot.egg-info/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-05-24 17:43:57.000000 lumibot-3.4.3/lumibot.egg-info/PKG-INFO
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3260 2024-05-24 17:43:57.000000 lumibot-3.4.3/lumibot.egg-info/SOURCES.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)        1 2024-05-24 17:43:57.000000 lumibot-3.4.3/lumibot.egg-info/dependency_links.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      572 2024-05-24 17:43:57.000000 lumibot-3.4.3/lumibot.egg-info/requires.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       14 2024-05-24 17:43:57.000000 lumibot-3.4.3/lumibot.egg-info/top_level.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      618 2024-03-18 04:35:37.000000 lumibot-3.4.3/pyproject.toml
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1352 2024-05-24 17:43:57.424163 lumibot-3.4.3/setup.cfg
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1809 2024-05-24 16:33:35.000000 lumibot-3.4.3/setup.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.421351 lumibot-3.4.3/tests/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      393 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/__init__.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-24 17:43:57.423129 lumibot-3.4.3/tests/backtest/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      400 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/backtest/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      553 2024-05-24 15:40:21.000000 lumibot-3.4.3/tests/backtest/fixtures.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    11668 2024-05-24 15:40:21.000000 lumibot-3.4.3/tests/backtest/test_example_strategies.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     7259 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/backtest/test_main_pandas_daily.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    17827 2024-05-24 15:40:21.000000 lumibot-3.4.3/tests/backtest/test_polygon.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1289 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/backtest/test_strategy_executor.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1928 2024-05-24 15:40:21.000000 lumibot-3.4.3/tests/backtest/test_yahoo.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      961 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/test_alpaca.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     9906 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/test_alpaca_old.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2015 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/test_asset.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2287 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/test_backtesting_broker.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1365 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/test_ccxt.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4457 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/test_ccxt_store.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1571 2024-05-24 15:40:21.000000 lumibot-3.4.3/tests/test_data_source.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      963 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/test_interactive_brokers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4177 2024-04-10 20:12:46.000000 lumibot-3.4.3/tests/test_order.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21487 2024-05-24 15:40:21.000000 lumibot-3.4.3/tests/test_polygon_helper.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     1494 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/test_strategy_methods.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    21225 2024-05-24 15:40:21.000000 lumibot-3.4.3/tests/test_tradier.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      163 2024-03-18 04:35:37.000000 lumibot-3.4.3/tests/test_tradingfee.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-28 07:37:00.505407 lumibot-3.4.4/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    35130 2024-03-18 04:35:37.000000 lumibot-3.4.4/LICENSE
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-05-28 07:37:00.505340 lumibot-3.4.4/PKG-INFO
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3861 2024-03-18 04:35:37.000000 lumibot-3.4.4/README.md
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-28 07:37:00.492099 lumibot-3.4.4/lumibot/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      693 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/__init__.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-28 07:37:00.493916 lumibot-3.4.4/lumibot/backtesting/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      371 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/backtesting/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      387 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/backtesting/alpaca_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      417 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/backtesting/alpha_vantage_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    31699 2024-05-24 15:40:21.000000 lumibot-3.4.4/lumibot/backtesting/backtesting_broker.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      244 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/backtesting/ccxt_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      388 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/backtesting/pandas_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    14652 2024-05-24 15:40:21.000000 lumibot-3.4.4/lumibot/backtesting/polygon_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      344 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/backtesting/yahoo_backtesting.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-28 07:37:00.494684 lumibot-3.4.4/lumibot/brokers/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      158 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/brokers/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    18630 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/brokers/alpaca.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    44490 2024-05-24 16:33:35.000000 lumibot-3.4.4/lumibot/brokers/broker.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    30406 2024-04-16 22:57:26.000000 lumibot-3.4.4/lumibot/brokers/ccxt.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    47384 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/brokers/interactive_brokers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    29851 2024-05-24 16:33:35.000000 lumibot-3.4.4/lumibot/brokers/tradier.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-28 07:37:00.496256 lumibot-3.4.4/lumibot/data_sources/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      492 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/data_sources/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    12688 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/data_sources/alpaca_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5094 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/data_sources/alpha_vantage_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    10614 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/data_sources/ccxt_backtesting_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7647 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/data_sources/ccxt_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    19315 2024-05-24 15:40:21.000000 lumibot-3.4.4/lumibot/data_sources/data_source.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2944 2024-04-03 02:08:33.000000 lumibot-3.4.4/lumibot/data_sources/data_source_backtesting.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      557 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/data_sources/exceptions.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    11836 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/data_sources/interactive_brokers_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15521 2024-05-24 15:40:21.000000 lumibot-3.4.4/lumibot/data_sources/pandas_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    11734 2024-05-24 15:40:21.000000 lumibot-3.4.4/lumibot/data_sources/tradier_data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7022 2024-04-10 20:12:46.000000 lumibot-3.4.4/lumibot/data_sources/yahoo_data.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-28 07:37:00.497457 lumibot-3.4.4/lumibot/entities/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      230 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/entities/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     9605 2024-05-24 15:40:21.000000 lumibot-3.4.4/lumibot/entities/asset.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5993 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/entities/bar.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    10205 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/entities/bars.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21849 2024-05-24 15:40:21.000000 lumibot-3.4.4/lumibot/entities/data.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      182 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/entities/dataline.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    28502 2024-05-24 16:33:35.000000 lumibot-3.4.4/lumibot/entities/order.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4646 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/entities/position.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1920 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/entities/trading_fee.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-28 07:37:00.498983 lumibot-3.4.4/lumibot/example_strategies/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)        0 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/example_strategies/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5551 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/example_strategies/ccxt_backtesting_example.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5098 2024-04-16 22:57:26.000000 lumibot-3.4.4/lumibot/example_strategies/crypto_important_functions.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2613 2024-04-10 20:12:46.000000 lumibot-3.4.4/lumibot/example_strategies/options_hold_to_expiry.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1226 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/example_strategies/simple_start_single_file.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2220 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/example_strategies/stock_bracket.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1895 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/example_strategies/stock_buy_and_hold.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5137 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/example_strategies/stock_diversified_leverage.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2980 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/example_strategies/stock_limit_and_trailing_stops.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     6476 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/example_strategies/stock_momentum.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2426 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/example_strategies/stock_oco.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    12862 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/example_strategies/strangle.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-28 07:37:00.499519 lumibot-3.4.4/lumibot/strategies/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       79 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/strategies/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    53746 2024-05-24 15:40:21.000000 lumibot-3.4.4/lumibot/strategies/_strategy.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)   153357 2024-05-24 15:40:21.000000 lumibot-3.4.4/lumibot/strategies/strategy.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    39943 2024-05-24 15:40:21.000000 lumibot-3.4.4/lumibot/strategies/strategy_executor.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-28 07:37:00.501376 lumibot-3.4.4/lumibot/tools/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1321 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/tools/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    25331 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/tools/black_scholes.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21351 2024-04-07 08:25:48.000000 lumibot-3.4.4/lumibot/tools/ccxt_data_store.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      485 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/tools/debugers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2017 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/tools/decorators.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7570 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/tools/helpers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    26283 2024-05-24 15:40:21.000000 lumibot-3.4.4/lumibot/tools/indicators.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1017 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/tools/lumibot_time.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1342 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/tools/pandas.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21338 2024-05-24 15:40:21.000000 lumibot-3.4.4/lumibot/tools/polygon_helper.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1866 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/tools/types.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    15762 2024-05-24 15:40:21.000000 lumibot-3.4.4/lumibot/tools/yahoo_helper.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-28 07:37:00.501610 lumibot-3.4.4/lumibot/traders/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       27 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/traders/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7997 2024-05-24 15:40:21.000000 lumibot-3.4.4/lumibot/traders/trader.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-28 07:37:00.502144 lumibot-3.4.4/lumibot/trading_builtins/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       87 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/trading_builtins/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3261 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/trading_builtins/custom_stream.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1975 2024-03-18 04:35:37.000000 lumibot-3.4.4/lumibot/trading_builtins/safe_list.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-28 07:37:00.505000 lumibot-3.4.4/lumibot.egg-info/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5467 2024-05-28 07:37:00.000000 lumibot-3.4.4/lumibot.egg-info/PKG-INFO
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3260 2024-05-28 07:37:00.000000 lumibot-3.4.4/lumibot.egg-info/SOURCES.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)        1 2024-05-28 07:37:00.000000 lumibot-3.4.4/lumibot.egg-info/dependency_links.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      572 2024-05-28 07:37:00.000000 lumibot-3.4.4/lumibot.egg-info/requires.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       14 2024-05-28 07:37:00.000000 lumibot-3.4.4/lumibot.egg-info/top_level.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      618 2024-03-18 04:35:37.000000 lumibot-3.4.4/pyproject.toml
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1352 2024-05-28 07:37:00.505715 lumibot-3.4.4/setup.cfg
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1809 2024-05-28 07:35:17.000000 lumibot-3.4.4/setup.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-28 07:37:00.503884 lumibot-3.4.4/tests/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      393 2024-03-18 04:35:37.000000 lumibot-3.4.4/tests/__init__.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-28 07:37:00.504829 lumibot-3.4.4/tests/backtest/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      400 2024-03-18 04:35:37.000000 lumibot-3.4.4/tests/backtest/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      553 2024-05-24 15:40:21.000000 lumibot-3.4.4/tests/backtest/fixtures.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    11668 2024-05-24 15:40:21.000000 lumibot-3.4.4/tests/backtest/test_example_strategies.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     7259 2024-03-18 04:35:37.000000 lumibot-3.4.4/tests/backtest/test_main_pandas_daily.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    17827 2024-05-24 15:40:21.000000 lumibot-3.4.4/tests/backtest/test_polygon.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1289 2024-03-18 04:35:37.000000 lumibot-3.4.4/tests/backtest/test_strategy_executor.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1928 2024-05-24 15:40:21.000000 lumibot-3.4.4/tests/backtest/test_yahoo.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      961 2024-03-18 04:35:37.000000 lumibot-3.4.4/tests/test_alpaca.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     9906 2024-03-18 04:35:37.000000 lumibot-3.4.4/tests/test_alpaca_old.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2015 2024-03-18 04:35:37.000000 lumibot-3.4.4/tests/test_asset.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2287 2024-03-18 04:35:37.000000 lumibot-3.4.4/tests/test_backtesting_broker.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1365 2024-03-18 04:35:37.000000 lumibot-3.4.4/tests/test_ccxt.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4457 2024-03-18 04:35:37.000000 lumibot-3.4.4/tests/test_ccxt_store.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1571 2024-05-24 15:40:21.000000 lumibot-3.4.4/tests/test_data_source.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      963 2024-03-18 04:35:37.000000 lumibot-3.4.4/tests/test_interactive_brokers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     4177 2024-04-10 20:12:46.000000 lumibot-3.4.4/tests/test_order.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21487 2024-05-24 15:40:21.000000 lumibot-3.4.4/tests/test_polygon_helper.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     1494 2024-03-18 04:35:37.000000 lumibot-3.4.4/tests/test_strategy_methods.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    21225 2024-05-24 15:40:21.000000 lumibot-3.4.4/tests/test_tradier.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      163 2024-03-18 04:35:37.000000 lumibot-3.4.4/tests/test_tradingfee.py
```

### Comparing `lumibot-3.4.3/LICENSE` & `lumibot-3.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/PKG-INFO` & `lumibot-3.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumibot
-Version: 3.4.3
+Version: 3.4.4
 Summary: Backtesting and Trading Library, Made by Lumiwealth
 Home-page: https://github.com/Lumiwealth/lumibot
 Author: Robert Grzesik
 Author-email: rob@lumiwealth.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 Requires-Dist: flask-security
 Requires-Dist: marshmallow-sqlalchemy
 Requires-Dist: email_validator
 Requires-Dist: bcrypt
 Requires-Dist: pytest
 Requires-Dist: scipy>=1.13.0
 Requires-Dist: ipython
-Requires-Dist: quantstats-lumi>=0.2.0
+Requires-Dist: quantstats-lumi>=0.3.0
 Requires-Dist: python-dotenv
 Requires-Dist: ccxt==4.2.85
 Requires-Dist: termcolor
 Requires-Dist: jsonpickle
 Requires-Dist: apscheduler==3.10.4
 Requires-Dist: appdirs
 Requires-Dist: pyarrow
```

### Comparing `lumibot-3.4.3/README.md` & `lumibot-3.4.4/README.md`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/__init__.py` & `lumibot-3.4.4/lumibot/__init__.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/backtesting/backtesting_broker.py` & `lumibot-3.4.4/lumibot/backtesting/backtesting_broker.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/backtesting/polygon_backtesting.py` & `lumibot-3.4.4/lumibot/backtesting/polygon_backtesting.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/brokers/alpaca.py` & `lumibot-3.4.4/lumibot/brokers/alpaca.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/brokers/broker.py` & `lumibot-3.4.4/lumibot/brokers/broker.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/brokers/ccxt.py` & `lumibot-3.4.4/lumibot/brokers/ccxt.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/brokers/interactive_brokers.py` & `lumibot-3.4.4/lumibot/brokers/interactive_brokers.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/brokers/tradier.py` & `lumibot-3.4.4/lumibot/brokers/tradier.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/data_sources/alpaca_data.py` & `lumibot-3.4.4/lumibot/data_sources/alpaca_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/data_sources/alpha_vantage_data.py` & `lumibot-3.4.4/lumibot/data_sources/alpha_vantage_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/data_sources/ccxt_backtesting_data.py` & `lumibot-3.4.4/lumibot/data_sources/ccxt_backtesting_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/data_sources/ccxt_data.py` & `lumibot-3.4.4/lumibot/data_sources/ccxt_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/data_sources/data_source.py` & `lumibot-3.4.4/lumibot/data_sources/data_source.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/data_sources/data_source_backtesting.py` & `lumibot-3.4.4/lumibot/data_sources/data_source_backtesting.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/data_sources/exceptions.py` & `lumibot-3.4.4/lumibot/data_sources/exceptions.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/data_sources/interactive_brokers_data.py` & `lumibot-3.4.4/lumibot/data_sources/interactive_brokers_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/data_sources/pandas_data.py` & `lumibot-3.4.4/lumibot/data_sources/pandas_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/data_sources/tradier_data.py` & `lumibot-3.4.4/lumibot/data_sources/tradier_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/data_sources/yahoo_data.py` & `lumibot-3.4.4/lumibot/data_sources/yahoo_data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/entities/asset.py` & `lumibot-3.4.4/lumibot/entities/asset.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/entities/bar.py` & `lumibot-3.4.4/lumibot/entities/bar.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/entities/bars.py` & `lumibot-3.4.4/lumibot/entities/bars.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/entities/data.py` & `lumibot-3.4.4/lumibot/entities/data.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/entities/order.py` & `lumibot-3.4.4/lumibot/entities/order.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/entities/position.py` & `lumibot-3.4.4/lumibot/entities/position.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/entities/trading_fee.py` & `lumibot-3.4.4/lumibot/entities/trading_fee.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/example_strategies/ccxt_backtesting_example.py` & `lumibot-3.4.4/lumibot/example_strategies/ccxt_backtesting_example.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/example_strategies/crypto_important_functions.py` & `lumibot-3.4.4/lumibot/example_strategies/crypto_important_functions.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/example_strategies/options_hold_to_expiry.py` & `lumibot-3.4.4/lumibot/example_strategies/options_hold_to_expiry.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/example_strategies/simple_start_single_file.py` & `lumibot-3.4.4/lumibot/example_strategies/simple_start_single_file.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/example_strategies/stock_bracket.py` & `lumibot-3.4.4/lumibot/example_strategies/stock_bracket.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/example_strategies/stock_buy_and_hold.py` & `lumibot-3.4.4/lumibot/example_strategies/stock_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/example_strategies/stock_diversified_leverage.py` & `lumibot-3.4.4/lumibot/example_strategies/stock_diversified_leverage.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/example_strategies/stock_limit_and_trailing_stops.py` & `lumibot-3.4.4/lumibot/example_strategies/stock_limit_and_trailing_stops.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/example_strategies/stock_momentum.py` & `lumibot-3.4.4/lumibot/example_strategies/stock_momentum.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/example_strategies/stock_oco.py` & `lumibot-3.4.4/lumibot/example_strategies/stock_oco.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/example_strategies/strangle.py` & `lumibot-3.4.4/lumibot/example_strategies/strangle.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/strategies/_strategy.py` & `lumibot-3.4.4/lumibot/strategies/_strategy.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/strategies/strategy.py` & `lumibot-3.4.4/lumibot/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/strategies/strategy_executor.py` & `lumibot-3.4.4/lumibot/strategies/strategy_executor.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/tools/__init__.py` & `lumibot-3.4.4/lumibot/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/tools/black_scholes.py` & `lumibot-3.4.4/lumibot/tools/black_scholes.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/tools/ccxt_data_store.py` & `lumibot-3.4.4/lumibot/tools/ccxt_data_store.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/tools/decorators.py` & `lumibot-3.4.4/lumibot/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/tools/helpers.py` & `lumibot-3.4.4/lumibot/tools/helpers.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/tools/indicators.py` & `lumibot-3.4.4/lumibot/tools/indicators.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/tools/lumibot_time.py` & `lumibot-3.4.4/lumibot/tools/lumibot_time.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/tools/pandas.py` & `lumibot-3.4.4/lumibot/tools/pandas.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/tools/polygon_helper.py` & `lumibot-3.4.4/lumibot/tools/polygon_helper.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/tools/types.py` & `lumibot-3.4.4/lumibot/tools/types.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/tools/yahoo_helper.py` & `lumibot-3.4.4/lumibot/tools/yahoo_helper.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/traders/trader.py` & `lumibot-3.4.4/lumibot/traders/trader.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/trading_builtins/custom_stream.py` & `lumibot-3.4.4/lumibot/trading_builtins/custom_stream.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot/trading_builtins/safe_list.py` & `lumibot-3.4.4/lumibot/trading_builtins/safe_list.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot.egg-info/PKG-INFO` & `lumibot-3.4.4/lumibot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumibot
-Version: 3.4.3
+Version: 3.4.4
 Summary: Backtesting and Trading Library, Made by Lumiwealth
 Home-page: https://github.com/Lumiwealth/lumibot
 Author: Robert Grzesik
 Author-email: rob@lumiwealth.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,15 +30,15 @@
 Requires-Dist: flask-security
 Requires-Dist: marshmallow-sqlalchemy
 Requires-Dist: email_validator
 Requires-Dist: bcrypt
 Requires-Dist: pytest
 Requires-Dist: scipy>=1.13.0
 Requires-Dist: ipython
-Requires-Dist: quantstats-lumi>=0.2.0
+Requires-Dist: quantstats-lumi>=0.3.0
 Requires-Dist: python-dotenv
 Requires-Dist: ccxt==4.2.85
 Requires-Dist: termcolor
 Requires-Dist: jsonpickle
 Requires-Dist: apscheduler==3.10.4
 Requires-Dist: appdirs
 Requires-Dist: pyarrow
```

### Comparing `lumibot-3.4.3/lumibot.egg-info/SOURCES.txt` & `lumibot-3.4.4/lumibot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/lumibot.egg-info/requires.txt` & `lumibot-3.4.4/lumibot.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 flask-security
 marshmallow-sqlalchemy
 email_validator
 bcrypt
 pytest
 scipy>=1.13.0
 ipython
-quantstats-lumi>=0.2.0
+quantstats-lumi>=0.3.0
 python-dotenv
 ccxt==4.2.85
 termcolor
 jsonpickle
 apscheduler==3.10.4
 appdirs
 pyarrow
```

### Comparing `lumibot-3.4.3/pyproject.toml` & `lumibot-3.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/setup.cfg` & `lumibot-3.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/setup.py` & `lumibot-3.4.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lumibot",
-    version="3.4.3",
+    version="3.4.4",
     author="Robert Grzesik",
     author_email="rob@lumiwealth.com",
     description="Backtesting and Trading Library, Made by Lumiwealth",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Lumiwealth/lumibot",
     packages=setuptools.find_packages(),
@@ -33,15 +33,15 @@
         "flask-security",
         "marshmallow-sqlalchemy",
         "email_validator",
         "bcrypt",
         "pytest",
         "scipy>=1.13.0",
         "ipython",  # required for quantstats, but not in their dependency list for some reason
-        "quantstats-lumi>=0.2.0",
+        "quantstats-lumi>=0.3.0",
         "python-dotenv",  # Secret Storage
         "ccxt==4.2.85",
         "termcolor",
         "jsonpickle",
         "apscheduler==3.10.4",
         "appdirs",
         "pyarrow",
```

### Comparing `lumibot-3.4.3/tests/backtest/fixtures.py` & `lumibot-3.4.4/tests/backtest/fixtures.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/tests/backtest/test_example_strategies.py` & `lumibot-3.4.4/tests/backtest/test_example_strategies.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/tests/backtest/test_main_pandas_daily.py` & `lumibot-3.4.4/tests/backtest/test_main_pandas_daily.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/tests/backtest/test_polygon.py` & `lumibot-3.4.4/tests/backtest/test_polygon.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/tests/backtest/test_strategy_executor.py` & `lumibot-3.4.4/tests/backtest/test_strategy_executor.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/tests/backtest/test_yahoo.py` & `lumibot-3.4.4/tests/backtest/test_yahoo.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/tests/test_alpaca.py` & `lumibot-3.4.4/tests/test_alpaca.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/tests/test_alpaca_old.py` & `lumibot-3.4.4/tests/test_alpaca_old.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/tests/test_asset.py` & `lumibot-3.4.4/tests/test_asset.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/tests/test_backtesting_broker.py` & `lumibot-3.4.4/tests/test_backtesting_broker.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/tests/test_ccxt.py` & `lumibot-3.4.4/tests/test_ccxt.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/tests/test_ccxt_store.py` & `lumibot-3.4.4/tests/test_ccxt_store.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/tests/test_data_source.py` & `lumibot-3.4.4/tests/test_data_source.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/tests/test_interactive_brokers.py` & `lumibot-3.4.4/tests/test_interactive_brokers.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/tests/test_order.py` & `lumibot-3.4.4/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/tests/test_polygon_helper.py` & `lumibot-3.4.4/tests/test_polygon_helper.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/tests/test_strategy_methods.py` & `lumibot-3.4.4/tests/test_strategy_methods.py`

 * *Files identical despite different names*

### Comparing `lumibot-3.4.3/tests/test_tradier.py` & `lumibot-3.4.4/tests/test_tradier.py`

 * *Files identical despite different names*

