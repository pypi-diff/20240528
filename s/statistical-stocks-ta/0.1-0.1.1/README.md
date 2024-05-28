# Comparing `tmp/statistical_stocks_ta-0.1.tar.gz` & `tmp/statistical_stocks_ta-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statistical_stocks_ta-0.1.tar", last modified: Mon May 27 15:40:48 2024, max compression
+gzip compressed data, was "statistical_stocks_ta-0.1.1.tar", last modified: Mon May 27 23:39:38 2024, max compression
```

## Comparing `statistical_stocks_ta-0.1.tar` & `statistical_stocks_ta-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 octo      (1000) octo      (1000)        0 2024-05-27 15:40:48.106498 statistical_stocks_ta-0.1/
--rw-rw-r--   0 octo      (1000) octo      (1000)     1067 2024-05-27 15:35:00.000000 statistical_stocks_ta-0.1/LICENSE
--rw-r--r--   0 octo      (1000) octo      (1000)     6630 2024-05-27 15:40:48.106498 statistical_stocks_ta-0.1/PKG-INFO
--rw-rw-r--   0 octo      (1000) octo      (1000)     5948 2024-05-27 15:34:24.000000 statistical_stocks_ta-0.1/README.md
--rw-rw-r--   0 octo      (1000) octo      (1000)       38 2024-05-27 15:40:48.106498 statistical_stocks_ta-0.1/setup.cfg
--rw-rw-r--   0 octo      (1000) octo      (1000)      843 2024-05-27 15:39:04.000000 statistical_stocks_ta-0.1/setup.py
-drwxrwxr-x   0 octo      (1000) octo      (1000)        0 2024-05-27 15:40:48.106498 statistical_stocks_ta-0.1/statistical_stocks_ta/
--rw-rw-r--   0 octo      (1000) octo      (1000)       36 2024-05-26 22:46:33.000000 statistical_stocks_ta-0.1/statistical_stocks_ta/__init__.py
--rw-rw-r--   0 octo      (1000) octo      (1000)     1435 2024-05-27 12:57:24.000000 statistical_stocks_ta-0.1/statistical_stocks_ta/indicators.py
--rw-rw-r--   0 octo      (1000) octo      (1000)     4125 2024-05-27 14:56:44.000000 statistical_stocks_ta-0.1/statistical_stocks_ta/patterns.py
--rw-rw-r--   0 octo      (1000) octo      (1000)     3914 2024-05-27 15:15:46.000000 statistical_stocks_ta-0.1/statistical_stocks_ta/plotting.py
--rw-rw-r--   0 octo      (1000) octo      (1000)     1786 2024-05-27 15:34:44.000000 statistical_stocks_ta-0.1/statistical_stocks_ta/statistical_stocks_ta.py
--rw-rw-r--   0 octo      (1000) octo      (1000)      573 2024-05-27 12:57:10.000000 statistical_stocks_ta-0.1/statistical_stocks_ta/support_resistance.py
-drwxrwxr-x   0 octo      (1000) octo      (1000)        0 2024-05-27 15:40:48.106498 statistical_stocks_ta-0.1/statistical_stocks_ta.egg-info/
--rw-r--r--   0 octo      (1000) octo      (1000)     6630 2024-05-27 15:40:48.000000 statistical_stocks_ta-0.1/statistical_stocks_ta.egg-info/PKG-INFO
--rw-rw-r--   0 octo      (1000) octo      (1000)      479 2024-05-27 15:40:48.000000 statistical_stocks_ta-0.1/statistical_stocks_ta.egg-info/SOURCES.txt
--rw-rw-r--   0 octo      (1000) octo      (1000)        1 2024-05-27 15:40:48.000000 statistical_stocks_ta-0.1/statistical_stocks_ta.egg-info/dependency_links.txt
--rw-rw-r--   0 octo      (1000) octo      (1000)       54 2024-05-27 15:40:48.000000 statistical_stocks_ta-0.1/statistical_stocks_ta.egg-info/requires.txt
--rw-rw-r--   0 octo      (1000) octo      (1000)       22 2024-05-27 15:40:48.000000 statistical_stocks_ta-0.1/statistical_stocks_ta.egg-info/top_level.txt
+drwxrwxr-x   0 octo      (1000) octo      (1000)        0 2024-05-27 23:39:38.243227 statistical_stocks_ta-0.1.1/
+-rw-rw-r--   0 octo      (1000) octo      (1000)     1067 2024-05-27 15:35:00.000000 statistical_stocks_ta-0.1.1/LICENSE
+-rw-r--r--   0 octo      (1000) octo      (1000)    10261 2024-05-27 23:39:38.243227 statistical_stocks_ta-0.1.1/PKG-INFO
+-rw-rw-r--   0 octo      (1000) octo      (1000)     9543 2024-05-27 23:37:45.000000 statistical_stocks_ta-0.1.1/README.md
+-rw-rw-r--   0 octo      (1000) octo      (1000)       38 2024-05-27 23:39:38.243227 statistical_stocks_ta-0.1.1/setup.cfg
+-rw-rw-r--   0 octo      (1000) octo      (1000)      875 2024-05-27 23:38:02.000000 statistical_stocks_ta-0.1.1/setup.py
+drwxrwxr-x   0 octo      (1000) octo      (1000)        0 2024-05-27 23:39:38.243227 statistical_stocks_ta-0.1.1/statistical_stocks_ta/
+-rw-rw-r--   0 octo      (1000) octo      (1000)       36 2024-05-26 22:46:33.000000 statistical_stocks_ta-0.1.1/statistical_stocks_ta/__init__.py
+-rw-rw-r--   0 octo      (1000) octo      (1000)     1435 2024-05-27 15:55:02.000000 statistical_stocks_ta-0.1.1/statistical_stocks_ta/indicators.py
+-rw-rw-r--   0 octo      (1000) octo      (1000)     4125 2024-05-27 15:55:02.000000 statistical_stocks_ta-0.1.1/statistical_stocks_ta/patterns.py
+-rw-rw-r--   0 octo      (1000) octo      (1000)    11564 2024-05-27 23:28:03.000000 statistical_stocks_ta-0.1.1/statistical_stocks_ta/plotting.py
+-rw-rw-r--   0 octo      (1000) octo      (1000)    13166 2024-05-27 23:25:55.000000 statistical_stocks_ta-0.1.1/statistical_stocks_ta/smc.py
+-rw-rw-r--   0 octo      (1000) octo      (1000)     2450 2024-05-27 23:32:00.000000 statistical_stocks_ta-0.1.1/statistical_stocks_ta/statistical_stocks_ta.py
+-rw-rw-r--   0 octo      (1000) octo      (1000)      573 2024-05-27 15:55:02.000000 statistical_stocks_ta-0.1.1/statistical_stocks_ta/support_resistance.py
+drwxrwxr-x   0 octo      (1000) octo      (1000)        0 2024-05-27 23:39:38.243227 statistical_stocks_ta-0.1.1/statistical_stocks_ta.egg-info/
+-rw-r--r--   0 octo      (1000) octo      (1000)    10261 2024-05-27 23:39:38.000000 statistical_stocks_ta-0.1.1/statistical_stocks_ta.egg-info/PKG-INFO
+-rw-rw-r--   0 octo      (1000) octo      (1000)      508 2024-05-27 23:39:38.000000 statistical_stocks_ta-0.1.1/statistical_stocks_ta.egg-info/SOURCES.txt
+-rw-rw-r--   0 octo      (1000) octo      (1000)        1 2024-05-27 23:39:38.000000 statistical_stocks_ta-0.1.1/statistical_stocks_ta.egg-info/dependency_links.txt
+-rw-rw-r--   0 octo      (1000) octo      (1000)       73 2024-05-27 23:39:38.000000 statistical_stocks_ta-0.1.1/statistical_stocks_ta.egg-info/requires.txt
+-rw-rw-r--   0 octo      (1000) octo      (1000)       22 2024-05-27 23:39:38.000000 statistical_stocks_ta-0.1.1/statistical_stocks_ta.egg-info/top_level.txt
```

### Comparing `statistical_stocks_ta-0.1/LICENSE` & `statistical_stocks_ta-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `statistical_stocks_ta-0.1/setup.py` & `statistical_stocks_ta-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="statistical-stocks-ta",
-    version="0.1",
+    version="0.1.1",
     author="Nils Lopez",
     author_email="lopez.nils@doctopus.app",
     description="A python package for Statistical Stocks TA (computing patterns, ma, indicators) and data fetching.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Nils-Lopez/statistical-stocks-ta",
     packages=find_packages(),
@@ -14,14 +14,15 @@
         "requests",
         "pandas",
         "numpy",
         "ta",
         "mplfinance",
         "ccxt",
         "scikit-learn",
+        "smartmoneyconcepts",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
```

### Comparing `statistical_stocks_ta-0.1/statistical_stocks_ta/indicators.py` & `statistical_stocks_ta-0.1.1/statistical_stocks_ta/indicators.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,38 +3,38 @@
 from ta.trend import SMAIndicator, EMAIndicator
 from ta.momentum import RSIIndicator
 from ta.trend import MACD
 
 
 def calculate_bollinger_bands(candles, window=20, std_dev=2):
     indicator_bb = BollingerBands(
-        close=candles["Close"], window=window, window_dev=std_dev
+        close=candles["close"], window=window, window_dev=std_dev
     )
-    candles["BB_High"] = indicator_bb.bollinger_hband()
-    candles["BB_Low"] = indicator_bb.bollinger_lband()
+    candles["BB_high"] = indicator_bb.bollinger_hband()
+    candles["BB_low"] = indicator_bb.bollinger_lband()
     return candles
 
 
 def calculate_moving_averages(candles, short_window=20, long_window=50):
-    sma_short = SMAIndicator(close=candles["Close"], window=short_window)
-    sma_long = SMAIndicator(close=candles["Close"], window=long_window)
-    ema_short = EMAIndicator(close=candles["Close"], window=short_window)
-    ema_long = EMAIndicator(close=candles["Close"], window=long_window)
+    sma_short = SMAIndicator(close=candles["close"], window=short_window)
+    sma_long = SMAIndicator(close=candles["close"], window=long_window)
+    ema_short = EMAIndicator(close=candles["close"], window=short_window)
+    ema_long = EMAIndicator(close=candles["close"], window=long_window)
     candles["SMA_Short"] = sma_short.sma_indicator()
     candles["SMA_Long"] = sma_long.sma_indicator()
     candles["EMA_Short"] = ema_short.ema_indicator()
     candles["EMA_Long"] = ema_long.ema_indicator()
     return candles
 
 
 def calculate_rsi(candles, window=14):
-    rsi = RSIIndicator(close=candles["Close"], window=window)
+    rsi = RSIIndicator(close=candles["close"], window=window)
     candles["RSI"] = rsi.rsi()
     return candles
 
 
 def calculate_macd(candles):
-    macd = MACD(close=candles["Close"])
+    macd = MACD(close=candles["close"])
     candles["MACD"] = macd.macd()
     candles["MACD_Signal"] = macd.macd_signal()
     candles["MACD_Diff"] = macd.macd_diff()
     return candles
```

### Comparing `statistical_stocks_ta-0.1/statistical_stocks_ta/patterns.py` & `statistical_stocks_ta-0.1.1/statistical_stocks_ta/patterns.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,41 +2,41 @@
 
 
 def detect_flags(candles, trend_window=20, flag_window=5, breakout_threshold=0.1):
     # Initialize flag column with None
     candles["Flag"] = None
 
     # Calculate returns to identify strong movements
-    candles["Returns"] = candles["Close"].pct_change()
+    candles["Returns"] = candles["close"].pct_change()
 
     # Loop through candles
     for i in range(trend_window + flag_window, len(candles)):
         # Define the prior trend
         trend_period = candles.iloc[i - trend_window - flag_window : i - flag_window]
         trend_up = trend_period["Returns"].sum() > 0
         trend_down = trend_period["Returns"].sum() < 0
 
         # Defining the flag consolidation
         flag_period = candles.iloc[i - flag_window : i]
-        max_high = flag_period["High"].max()
-        min_low = flag_period["Low"].min()
+        max_high = flag_period["high"].max()
+        min_low = flag_period["low"].min()
         range_c = max_high - min_low
 
         # Flag validation conditions
         within_range = (
-            flag_period["High"] < max_high + (range_c * breakout_threshold)
-        ) & (flag_period["Low"] > min_low - (range_c * breakout_threshold))
+            flag_period["high"] < max_high + (range_c * breakout_threshold)
+        ) & (flag_period["low"] > min_low - (range_c * breakout_threshold))
 
         # Check if all candles in flag window meet the range condition
         if within_range.all():
             # Check for breakout
             current_candle = candles.iloc[i]
-            if trend_up and current_candle["Close"] > max_high:
+            if trend_up and current_candle["close"] > max_high:
                 candles.at[candles.index[i], "Flag"] = "bullish"
-            elif trend_down and current_candle["Close"] < min_low:
+            elif trend_down and current_candle["close"] < min_low:
                 candles.at[candles.index[i], "Flag"] = "bearish"
 
     return candles
 
 
 def identify_patterns(
     candles,
@@ -45,51 +45,51 @@
     rolling_window=10,
     channel_window_range=(10, 15),
     flag_sensitivity=0.8,
 ):
     # Detecting Doji candles
     candles["Doji"] = np.where(
         (
-            abs(candles["Close"] - candles["Open"]) / (candles["High"] - candles["Low"])
+            abs(candles["close"] - candles["open"]) / (candles["high"] - candles["low"])
             < doji_threshold
         )
         & (
-            (candles["High"] - candles["Low"])
-            > candles["Close"].rolling(window=rolling_window).std()
+            (candles["high"] - candles["low"])
+            > candles["close"].rolling(window=rolling_window).std()
         ),
         1,
         0,
     )
 
     print("Doji candles: ", candles["Doji"].sum())
 
     # Detecting Engulfing patterns
     candles["Bullish_Engulfing"] = np.where(
-        (candles["Close"].shift(1) < candles["Open"].shift(1))
-        & (candles["Open"] < candles["Close"].shift(1))
-        & (candles["Close"] > candles["Open"].shift(1)),
+        (candles["close"].shift(1) < candles["open"].shift(1))
+        & (candles["open"] < candles["close"].shift(1))
+        & (candles["close"] > candles["open"].shift(1)),
         1,
         0,
     )
 
     print("Bullish Engulfing: ", candles["Bullish_Engulfing"].sum())
 
     candles["Bearish_Engulfing"] = np.where(
-        (candles["Open"].shift(1) < candles["Close"].shift(1))
-        & (candles["Open"] > candles["Close"].shift(1))
-        & (candles["Close"] < candles["Open"].shift(1)),
+        (candles["open"].shift(1) < candles["close"].shift(1))
+        & (candles["open"] > candles["close"].shift(1))
+        & (candles["close"] < candles["open"].shift(1)),
         1,
         0,
     )
 
     print("Bearish Engulfing: ", candles["Bearish_Engulfing"].sum())
 
     def dynamic_window(candles):
         # Example of dynamic window based on recent volatility
-        returns = candles["Close"].pct_change()
+        returns = candles["close"].pct_change()
         vol = returns.rolling(window=rolling_window).std()
         scaled_window = (
             (20 / vol)
             .fillna(20)
             .astype(int)
             .clip(lower=channel_window_range[0], upper=channel_window_range[1])
         )
@@ -98,22 +98,22 @@
     # Window calculation and channel identification
     window = dynamic_window(candles)
     channel_up = np.zeros(len(candles), dtype=int)
     channel_down = np.zeros(len(candles), dtype=int)
 
     for i in range(len(candles)):
         if i >= window.iloc[i]:
-            roll_high = candles["High"].iloc[i - window.iloc[i] : i].max()
-            roll_low = candles["Low"].iloc[i - window.iloc[i] : i].min()
+            roll_high = candles["high"].iloc[i - window.iloc[i] : i].max()
+            roll_low = candles["low"].iloc[i - window.iloc[i] : i].min()
 
-            std_dev = candles["Close"].iloc[i - window.iloc[i] : i].std()
+            std_dev = candles["close"].iloc[i - window.iloc[i] : i].std()
             buffer = buffer_factor * std_dev  # Adjust buffer factor
 
-            channel_up[i] = 1 if candles["High"].iloc[i] >= roll_high + buffer else 0
-            channel_down[i] = 1 if candles["Low"].iloc[i] <= roll_low - buffer else 0
+            channel_up[i] = 1 if candles["high"].iloc[i] >= roll_high + buffer else 0
+            channel_down[i] = 1 if candles["low"].iloc[i] <= roll_low - buffer else 0
 
     candles["Channel_Up"] = channel_up
     candles["Channel_Down"] = channel_down
     print("Channel Up: ", candles["Channel_Up"].sum())
     print("Channel Down: ", candles["Channel_Down"].sum())
 
     return candles
```

### Comparing `statistical_stocks_ta-0.1/statistical_stocks_ta/statistical_stocks_ta.py` & `statistical_stocks_ta-0.1.1/statistical_stocks_ta/statistical_stocks_ta.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 from support_resistance import quantile_regression_support_resistance
 from indicators import (
     calculate_bollinger_bands,
     calculate_moving_averages,
     calculate_rsi,
     calculate_macd,
 )
+from smc import compute_smc, compute_smc_bis
 from patterns import identify_patterns
-from plotting import plot_analysis
+from plotting import plot_analysis, plot_smc
+import matplotlib.pyplot as plt
 
 
-def fetch_data(symbol="SOL/USDT", timeframe="1h", limit=300):
+def fetch_data(symbol="ETH/USDT", timeframe="4h", limit=300):
     exchange = ccxt.binance({"rateLimit": 1200, "enableRateLimit": True})
     ohlcv = exchange.fetch_ohlcv(symbol, timeframe=timeframe, limit=limit)
-    data = pd.DataFrame(
-        ohlcv, columns=["Date", "Open", "High", "Low", "Close", "Volume"]
-    )
-    data["Date"] = pd.to_datetime(data["Date"], unit="ms")
-    data.set_index("Date", inplace=True)
+    data = pd.DataFrame(ohlcv, columns=["ds", "open", "high", "low", "close", "volume"])
+    data["ds"] = pd.to_datetime(data["ds"], unit="ms")
+    data.set_index("ds", inplace=True)
     return data
 
 
 def analyze_candles(
     candles,
     calc_bollinger_bands=True,
     bb_settings={"window": 20, "std_dev": 2},
@@ -35,14 +35,15 @@
     rsi_settings={"window": 14},
     calc_macd=True,
     macd_settings={},
     detect_patterns=True,
     pattern_settings={},
     plot=True,
     plot_settings={},
+    smc=True,
 ):
     if calc_bollinger_bands:
         candles = calculate_bollinger_bands(candles, **bb_settings)
 
     if calc_moving_averages:
         candles = calculate_moving_averages(candles, **ma_settings)
 
@@ -51,20 +52,36 @@
 
     if calc_macd:
         candles = calculate_macd(candles, **macd_settings)
 
     if detect_patterns:
         candles = identify_patterns(candles, **pattern_settings)
 
+    if smc:
+        candles = compute_smc(candles)
+
     if plot:
-        plot_analysis(candles, **plot_settings)
+        fig1, fig2, fig3, fig4 = plot_analysis(candles, **plot_settings)
 
     return candles
 
 
 def main():
     candles = fetch_data()
-    candles = analyze_candles(candles)
+    candles = identify_patterns(candles)
+    candles = calculate_rsi(candles)
+    candles = calculate_macd(candles)
+    candles = calculate_moving_averages(candles)
+    candles = calculate_bollinger_bands(candles)
+    candles = quantile_regression_support_resistance(candles)
+    candles = compute_smc(candles)
+    # candles = compute_smc_bis(candles)
+    # Check if the DataFrame is not empty
+    if candles.empty:
+        print("No data available after SMC computation.")
+        return
+    fig1, _, _, _ = plot_analysis(candles)
+    plt.show()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `statistical_stocks_ta-0.1/statistical_stocks_ta/support_resistance.py` & `statistical_stocks_ta-0.1.1/statistical_stocks_ta/support_resistance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 from sklearn.linear_model import QuantileRegressor
 
 
 def quantile_regression_support_resistance(candles, quantiles=[0.10, 0.90]):
     print("=== Starting quantile regression for support and resistance ===")
     x = np.arange(len(candles)).reshape(-1, 1)
-    y = candles["Close"].values
+    y = candles["close"].values
 
     for q in quantiles:
         model = QuantileRegressor(quantile=q).fit(x, y)
         pred = model.predict(x)
         key = "Support_Q" if q < 0.5 else "Resistance_Q"
         candles[key] = pred
     print("=== Quantile regression completed ===")
```

