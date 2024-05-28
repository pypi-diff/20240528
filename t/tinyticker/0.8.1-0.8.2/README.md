# Comparing `tmp/tinyticker-0.8.1.tar.gz` & `tmp/tinyticker-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyticker-0.8.1.tar", max compression
+gzip compressed data, was "tinyticker-0.8.2.tar", max compression
```

## Comparing `tinyticker-0.8.1.tar` & `tinyticker-0.8.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1068 2024-05-28 13:04:32.356545 tinyticker-0.8.1/LICENSE
--rw-r--r--   0        0        0     3955 2024-05-28 13:04:32.356545 tinyticker-0.8.1/README.md
--rw-r--r--   0        0        0      917 2024-05-28 13:04:32.356545 tinyticker-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      518 2024-05-28 13:04:32.360545 tinyticker-0.8.1/tinyticker/__init__.py
--rw-r--r--   0        0        0     4712 2024-05-28 13:04:32.360545 tinyticker-0.8.1/tinyticker/__main__.py
--rw-r--r--   0        0        0     3183 2024-05-28 13:04:32.360545 tinyticker-0.8.1/tinyticker/config.py
--rw-r--r--   0        0        0     4843 2024-05-28 13:04:32.360545 tinyticker-0.8.1/tinyticker/display.py
--rw-r--r--   0        0        0     8241 2024-05-28 13:04:32.360545 tinyticker-0.8.1/tinyticker/layouts.py
--rw-r--r--   0        0        0      345 2024-05-28 13:04:32.360545 tinyticker-0.8.1/tinyticker/paths.py
--rw-r--r--   0        0        0     5483 2024-05-28 13:04:32.360545 tinyticker-0.8.1/tinyticker/sequence.py
--rw-r--r--   0        0        0     1112 2024-05-28 13:04:32.360545 tinyticker-0.8.1/tinyticker/tickers/__init__.py
--rw-r--r--   0        0        0     3563 2024-05-28 13:04:32.360545 tinyticker-0.8.1/tinyticker/tickers/_base.py
--rw-r--r--   0        0        0     4620 2024-05-28 13:04:32.360545 tinyticker-0.8.1/tinyticker/tickers/crypto.py
--rw-r--r--   0        0        0     3872 2024-05-28 13:04:32.360545 tinyticker-0.8.1/tinyticker/tickers/stock.py
--rw-r--r--   0        0        0     2391 2024-05-28 13:04:32.360545 tinyticker-0.8.1/tinyticker/utils.py
--rw-r--r--   0        0        0      278 2024-05-28 13:04:32.360545 tinyticker-0.8.1/tinyticker/waveshare_lib/__init__.py
--rw-r--r--   0        0        0     1297 2024-05-28 13:04:32.360545 tinyticker-0.8.1/tinyticker/waveshare_lib/_base.py
--rw-r--r--   0        0        0     4104 2024-05-28 13:04:32.360545 tinyticker-0.8.1/tinyticker/waveshare_lib/device.py
--rw-r--r--   0        0        0     8593 2024-05-28 13:04:32.360545 tinyticker-0.8.1/tinyticker/waveshare_lib/epd2in13.py
--rw-r--r--   0        0        0    12127 2024-05-28 13:04:32.360545 tinyticker-0.8.1/tinyticker/waveshare_lib/epd2in13_V2.py
--rw-r--r--   0        0        0    14828 2024-05-28 13:04:32.360545 tinyticker-0.8.1/tinyticker/waveshare_lib/epd2in13_V3.py
--rw-r--r--   0        0        0    10709 2024-05-28 13:04:32.360545 tinyticker-0.8.1/tinyticker/waveshare_lib/epd2in13_V4.py
--rw-r--r--   0        0        0     6057 2024-05-28 13:04:32.360545 tinyticker-0.8.1/tinyticker/waveshare_lib/epd2in13b_V3.py
--rw-r--r--   0        0        0     6860 2024-05-28 13:04:32.360545 tinyticker-0.8.1/tinyticker/waveshare_lib/epd2in13b_V4.py
--rw-r--r--   0        0        0     5907 2024-05-28 13:04:32.360545 tinyticker-0.8.1/tinyticker/waveshare_lib/epd2in13bc.py
--rw-r--r--   0        0        0    21091 2024-05-28 13:04:32.364545 tinyticker-0.8.1/tinyticker/waveshare_lib/epd2in7.py
--rw-r--r--   0        0        0    19697 2024-05-28 13:04:32.364545 tinyticker-0.8.1/tinyticker/waveshare_lib/epd2in7_V2.py
--rw-r--r--   0        0        0     1558 2024-05-28 13:04:32.364545 tinyticker-0.8.1/tinyticker/waveshare_lib/models.py
--rw-r--r--   0        0        0       95 2024-05-28 13:04:32.364545 tinyticker-0.8.1/tinyticker/web/__init__.py
--rw-r--r--   0        0        0     2895 2024-05-28 13:04:32.364545 tinyticker-0.8.1/tinyticker/web/__main__.py
--rw-r--r--   0        0        0     8792 2024-05-28 13:04:32.364545 tinyticker-0.8.1/tinyticker/web/app.py
--rw-r--r--   0        0        0     3656 2024-05-28 13:04:32.364545 tinyticker-0.8.1/tinyticker/web/command.py
--rw-r--r--   0        0        0      593 2024-05-28 13:04:32.364545 tinyticker-0.8.1/tinyticker/web/startup.py
--rw-r--r--   0        0        0   274777 2024-05-28 13:04:32.364545 tinyticker-0.8.1/tinyticker/web/templates/css/uikit.min.css
--rw-r--r--   0        0        0    12844 2024-05-28 13:04:32.364545 tinyticker-0.8.1/tinyticker/web/templates/images/apple-touch-icon.png
--rw-r--r--   0        0        0      742 2024-05-28 13:04:32.364545 tinyticker-0.8.1/tinyticker/web/templates/images/favicon-16x16.png
--rw-r--r--   0        0        0     1645 2024-05-28 13:04:32.364545 tinyticker-0.8.1/tinyticker/web/templates/images/favicon-32x32.png
--rw-r--r--   0        0        0    18394 2024-05-28 13:04:32.364545 tinyticker-0.8.1/tinyticker/web/templates/index.html
--rw-r--r--   0        0        0     1924 2024-05-28 13:04:32.364545 tinyticker-0.8.1/tinyticker/web/templates/js/index.js
--rw-r--r--   0        0        0    65291 2024-05-28 13:04:32.364545 tinyticker-0.8.1/tinyticker/web/templates/js/uikit-icons.min.js
--rw-r--r--   0        0        0   136629 2024-05-28 13:04:32.364545 tinyticker-0.8.1/tinyticker/web/templates/js/uikit.min.js
--rw-r--r--   0        0        0     2449 2024-05-28 13:04:32.364545 tinyticker-0.8.1/tinyticker/web/templates/logfiles.html
--rw-r--r--   0        0        0     3173 2024-05-28 13:04:32.364545 tinyticker-0.8.1/tinyticker/web/templates/startup.html
--rw-r--r--   0        0        0     5244 1970-01-01 00:00:00.000000 tinyticker-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-28 13:12:45.252790 tinyticker-0.8.2/LICENSE
+-rw-r--r--   0        0        0     3955 2024-05-28 13:12:45.252790 tinyticker-0.8.2/README.md
+-rw-r--r--   0        0        0      917 2024-05-28 13:12:45.252790 tinyticker-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0      518 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/__init__.py
+-rw-r--r--   0        0        0     4712 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/__main__.py
+-rw-r--r--   0        0        0     3172 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/config.py
+-rw-r--r--   0        0        0     4843 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/display.py
+-rw-r--r--   0        0        0     8241 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/layouts.py
+-rw-r--r--   0        0        0      345 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/paths.py
+-rw-r--r--   0        0        0     5504 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/sequence.py
+-rw-r--r--   0        0        0     1112 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/tickers/__init__.py
+-rw-r--r--   0        0        0     3467 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/tickers/_base.py
+-rw-r--r--   0        0        0     4620 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/tickers/crypto.py
+-rw-r--r--   0        0        0     3872 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/tickers/stock.py
+-rw-r--r--   0        0        0     2391 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/utils.py
+-rw-r--r--   0        0        0      278 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/waveshare_lib/__init__.py
+-rw-r--r--   0        0        0     1297 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/waveshare_lib/_base.py
+-rw-r--r--   0        0        0     4104 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/waveshare_lib/device.py
+-rw-r--r--   0        0        0     8593 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13.py
+-rw-r--r--   0        0        0    12127 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13_V2.py
+-rw-r--r--   0        0        0    14828 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13_V3.py
+-rw-r--r--   0        0        0    10709 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13_V4.py
+-rw-r--r--   0        0        0     6057 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13b_V3.py
+-rw-r--r--   0        0        0     6860 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13b_V4.py
+-rw-r--r--   0        0        0     5907 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13bc.py
+-rw-r--r--   0        0        0    21091 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in7.py
+-rw-r--r--   0        0        0    19697 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in7_V2.py
+-rw-r--r--   0        0        0     1558 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/waveshare_lib/models.py
+-rw-r--r--   0        0        0       95 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/__init__.py
+-rw-r--r--   0        0        0     2895 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/__main__.py
+-rw-r--r--   0        0        0     8792 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/app.py
+-rw-r--r--   0        0        0     3656 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/command.py
+-rw-r--r--   0        0        0      593 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/startup.py
+-rw-r--r--   0        0        0   274777 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/templates/css/uikit.min.css
+-rw-r--r--   0        0        0    12844 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/templates/images/apple-touch-icon.png
+-rw-r--r--   0        0        0      742 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/templates/images/favicon-16x16.png
+-rw-r--r--   0        0        0     1645 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/templates/images/favicon-32x32.png
+-rw-r--r--   0        0        0    18323 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/templates/index.html
+-rw-r--r--   0        0        0     1924 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/templates/js/index.js
+-rw-r--r--   0        0        0    65291 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/templates/js/uikit-icons.min.js
+-rw-r--r--   0        0        0   136629 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/templates/js/uikit.min.js
+-rw-r--r--   0        0        0     2449 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/templates/logfiles.html
+-rw-r--r--   0        0        0     3173 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/templates/startup.html
+-rw-r--r--   0        0        0     5244 1970-01-01 00:00:00.000000 tinyticker-0.8.2/PKG-INFO
```

### Comparing `tinyticker-0.8.1/LICENSE` & `tinyticker-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/README.md` & `tinyticker-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/pyproject.toml` & `tinyticker-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tinyticker"
-version = "0.8.1"
+version = "0.8.2"
 description = "A tiny Raspberry Pi powered ePaper ticker."
 authors = ["Loic Coyle <loic.coyle@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/loiccoyle/tinyticker"
 keywords = ["raspberry-pi", "ticker", "stock", "crypto", "epaper", "finance"]
```

### Comparing `tinyticker-0.8.1/tinyticker/__init__.py` & `tinyticker-0.8.2/tinyticker/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/__main__.py` & `tinyticker-0.8.2/tinyticker/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/config.py` & `tinyticker-0.8.2/tinyticker/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 @dc.dataclass
 class TickerConfig:
     symbol_type: str = "stock"
     symbol: str = "SPY"
     interval: str = "1d"
     lookback: Optional[int] = None
-    wait_time: Optional[int] = None
+    wait_time: int = 600
     plot_type: str = "candle"
     mav: Optional[int] = None
     volume: bool = False
     avg_buy_price: Optional[float] = None
     prepost: bool = False
     layout: LayoutConfig = dc.field(default_factory=lambda: LayoutConfig())
```

### Comparing `tinyticker-0.8.1/tinyticker/display.py` & `tinyticker-0.8.2/tinyticker/display.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/layouts.py` & `tinyticker-0.8.2/tinyticker/layouts.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/sequence.py` & `tinyticker-0.8.2/tinyticker/sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     ) -> AsyncGenerator[Tuple[TickerBase, TickerResponse], None]:
         """Start iterating through the tickers.
 
         Returns:
             The `Ticker` instance and its response.
         """
         # if all tickers are skipped, we want to sleep for the smallest wait time
-        all_skipped_cooldown = min(ticker.wait_time for ticker in self.tickers)
+        all_skipped_cooldown = min(ticker.config.wait_time for ticker in self.tickers)
 
         all_skipped = False
         while True:
             if all_skipped:
                 LOGGER.info(f"All tickers skipped, sleeping {all_skipped_cooldown}s.")
                 time.sleep(all_skipped_cooldown)
             all_skipped = True
@@ -123,18 +123,18 @@
                         > outdated_min_delta
                     ):
                         LOGGER.debug(f"{ticker} response outdated, skipping.")
                         continue
                 all_skipped = False
                 yield (ticker, response)
 
-                LOGGER.info(f"Sleeping {ticker.wait_time}s.")
+                LOGGER.info(f"Sleeping {ticker.config.wait_time}s.")
                 # we want to sleep for the ticker's wait time and check every second if we
                 # should skip this ticker.
-                for _ in range(ticker.wait_time):
+                for _ in range(ticker.config.wait_time):
                     if self._skip_ticker:
                         LOGGER.info(f"Stop waiting, skipping {ticker}.")
                         break
                     await asyncio.sleep(1)
 
     def __str__(self):
         return (
```

### Comparing `tinyticker-0.8.1/tinyticker/tickers/__init__.py` & `tinyticker-0.8.2/tinyticker/tickers/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/tickers/_base.py` & `tinyticker-0.8.2/tinyticker/tickers/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,17 +77,14 @@
         self.config = config
         self.interval_dt = INTERVAL_TIMEDELTAS[config.interval]
         self.lookback = (
             self.config.lookback
             if self.config.lookback is not None
             else INTERVAL_LOOKBACKS[config.interval]
         )
-        self.wait_time = (
-            self.config.wait_time if self.config.wait_time is not None else 600
-        )
 
     def _single_tick(self) -> Tuple[pd.DataFrame, Optional[float]]: ...
 
     def single_tick(self) -> TickerResponse:
         """Get the historical and current price data for a single tick.
 
         Returns:
@@ -117,20 +114,20 @@
 
         Returns:
             Iterator over the responses.
         """
         while True:
             self._log.info("Ticker start.")
             yield self.single_tick()
-            self._log.debug("Sleeping %i s", self.wait_time)
-            time.sleep(self.wait_time)  # type: ignore
+            self._log.debug("Sleeping %i s", self.config.wait_time)
+            time.sleep(self.config.wait_time)  # type: ignore
 
     def __str__(self) -> str:
         return "\t".join(
             [
                 "Ticker",
                 self.config.symbol_type,
                 self.config.symbol,
                 f"{self.lookback}x{self.config.interval}",
-                str(self.wait_time),
+                str(self.config.wait_time),
             ]
         )
```

### Comparing `tinyticker-0.8.1/tinyticker/tickers/crypto.py` & `tinyticker-0.8.2/tinyticker/tickers/crypto.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/tickers/stock.py` & `tinyticker-0.8.2/tinyticker/tickers/stock.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/utils.py` & `tinyticker-0.8.2/tinyticker/utils.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/waveshare_lib/_base.py` & `tinyticker-0.8.2/tinyticker/waveshare_lib/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/waveshare_lib/device.py` & `tinyticker-0.8.2/tinyticker/waveshare_lib/device.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/waveshare_lib/epd2in13.py` & `tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/waveshare_lib/epd2in13_V2.py` & `tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/waveshare_lib/epd2in13_V3.py` & `tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/waveshare_lib/epd2in13_V4.py` & `tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/waveshare_lib/epd2in13b_V3.py` & `tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13b_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/waveshare_lib/epd2in13b_V4.py` & `tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13b_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/waveshare_lib/epd2in13bc.py` & `tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13bc.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/waveshare_lib/epd2in7.py` & `tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in7.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/waveshare_lib/epd2in7_V2.py` & `tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in7_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/waveshare_lib/models.py` & `tinyticker-0.8.2/tinyticker/waveshare_lib/models.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/web/__main__.py` & `tinyticker-0.8.2/tinyticker/web/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/web/app.py` & `tinyticker-0.8.2/tinyticker/web/app.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/web/command.py` & `tinyticker-0.8.2/tinyticker/web/command.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/web/startup.py` & `tinyticker-0.8.2/tinyticker/web/startup.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/web/templates/css/uikit.min.css` & `tinyticker-0.8.2/tinyticker/web/templates/css/uikit.min.css`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/web/templates/images/apple-touch-icon.png` & `tinyticker-0.8.2/tinyticker/web/templates/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/web/templates/images/favicon-16x16.png` & `tinyticker-0.8.2/tinyticker/web/templates/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/web/templates/images/favicon-32x32.png` & `tinyticker-0.8.2/tinyticker/web/templates/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/web/templates/index.html` & `tinyticker-0.8.2/tinyticker/web/templates/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,15 @@
                     <input
                       class="uk-input uk-form-small uk-width-1-3"
                       inputmode="numeric"
                       id="wait_time"
                       name="wait_time"
                       min="1"
                       uk-tooltip="Time to wait on this ticker."
-                      {% if ticker.wait_time is none %}placeholder="600"{% else %}value="{{ ticker.wait_time }}"{% endif %}
+                      value="{{ ticker.wait_time }}"
                     />
                   </div>
 
                   <div class="uk-flex uk-flex-between">
                     <label class="uk-form-label" for="mav">
                       Moving average
                     </label>
```

#### html2text {}

```diff
@@ -30,17 +30,15 @@
 { plot_type_option }}
 {%- endfor -%}
 Lookback
 #- If the look back is None then it has not been set so use the default
 lookback for the interval #} {% if ticker.lookback is none %}placeholder="{
 { interval_lookbacks[ticker.interval] }}"{% else %}value="{{ ticker.lookback
 }}"{% endif %} />
-Wait time (s)
-% if ticker.wait_time is none %}placeholder="600"{% else %}value="{
-{ ticker.wait_time }}"{% endif %} />
+Wait time (s)[{{ ticker.wait_time }}]
 Moving average[{{ ticker.mav if ticker.mav is not none }}]
 Average buy price[{{ ticker.avg_buy_price if ticker.avg_buy_price is not none
 }}]
 % if ticker.volume | default(False) %}checked{% endif %}
 onclick="this.previousElementSibling.value=1-this.previousElementSibling.value"
 /> Show trade volume
 % if ticker.prepost| default(False) %}checked{% endif %}
```

### Comparing `tinyticker-0.8.1/tinyticker/web/templates/js/index.js` & `tinyticker-0.8.2/tinyticker/web/templates/js/index.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/web/templates/js/uikit-icons.min.js` & `tinyticker-0.8.2/tinyticker/web/templates/js/uikit-icons.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/web/templates/js/uikit.min.js` & `tinyticker-0.8.2/tinyticker/web/templates/js/uikit.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/web/templates/logfiles.html` & `tinyticker-0.8.2/tinyticker/web/templates/logfiles.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/tinyticker/web/templates/startup.html` & `tinyticker-0.8.2/tinyticker/web/templates/startup.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.1/PKG-INFO` & `tinyticker-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyticker
-Version: 0.8.1
+Version: 0.8.2
 Summary: A tiny Raspberry Pi powered ePaper ticker.
 Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT
 Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance
 Author: Loic Coyle
 Author-email: loic.coyle@hotmail.fr
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tinyticker Version: 0.8.1 Summary: A tiny Raspberry
+Metadata-Version: 2.1 Name: tinyticker Version: 0.8.2 Summary: A tiny Raspberry
 Pi powered ePaper ticker. Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance Author:
 Loic Coyle Author-email: loic.coyle@hotmail.fr Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

