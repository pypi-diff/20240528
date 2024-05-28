# Comparing `tmp/tinyticker-0.8.2.tar.gz` & `tmp/tinyticker-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyticker-0.8.2.tar", max compression
+gzip compressed data, was "tinyticker-0.8.3.tar", max compression
```

## Comparing `tinyticker-0.8.2.tar` & `tinyticker-0.8.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1068 2024-05-28 13:12:45.252790 tinyticker-0.8.2/LICENSE
--rw-r--r--   0        0        0     3955 2024-05-28 13:12:45.252790 tinyticker-0.8.2/README.md
--rw-r--r--   0        0        0      917 2024-05-28 13:12:45.252790 tinyticker-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      518 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/__init__.py
--rw-r--r--   0        0        0     4712 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/__main__.py
--rw-r--r--   0        0        0     3172 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/config.py
--rw-r--r--   0        0        0     4843 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/display.py
--rw-r--r--   0        0        0     8241 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/layouts.py
--rw-r--r--   0        0        0      345 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/paths.py
--rw-r--r--   0        0        0     5504 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/sequence.py
--rw-r--r--   0        0        0     1112 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/tickers/__init__.py
--rw-r--r--   0        0        0     3467 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/tickers/_base.py
--rw-r--r--   0        0        0     4620 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/tickers/crypto.py
--rw-r--r--   0        0        0     3872 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/tickers/stock.py
--rw-r--r--   0        0        0     2391 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/utils.py
--rw-r--r--   0        0        0      278 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/waveshare_lib/__init__.py
--rw-r--r--   0        0        0     1297 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/waveshare_lib/_base.py
--rw-r--r--   0        0        0     4104 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/waveshare_lib/device.py
--rw-r--r--   0        0        0     8593 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13.py
--rw-r--r--   0        0        0    12127 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13_V2.py
--rw-r--r--   0        0        0    14828 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13_V3.py
--rw-r--r--   0        0        0    10709 2024-05-28 13:12:45.256790 tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13_V4.py
--rw-r--r--   0        0        0     6057 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13b_V3.py
--rw-r--r--   0        0        0     6860 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13b_V4.py
--rw-r--r--   0        0        0     5907 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13bc.py
--rw-r--r--   0        0        0    21091 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in7.py
--rw-r--r--   0        0        0    19697 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in7_V2.py
--rw-r--r--   0        0        0     1558 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/waveshare_lib/models.py
--rw-r--r--   0        0        0       95 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/__init__.py
--rw-r--r--   0        0        0     2895 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/__main__.py
--rw-r--r--   0        0        0     8792 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/app.py
--rw-r--r--   0        0        0     3656 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/command.py
--rw-r--r--   0        0        0      593 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/startup.py
--rw-r--r--   0        0        0   274777 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/templates/css/uikit.min.css
--rw-r--r--   0        0        0    12844 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/templates/images/apple-touch-icon.png
--rw-r--r--   0        0        0      742 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/templates/images/favicon-16x16.png
--rw-r--r--   0        0        0     1645 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/templates/images/favicon-32x32.png
--rw-r--r--   0        0        0    18323 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/templates/index.html
--rw-r--r--   0        0        0     1924 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/templates/js/index.js
--rw-r--r--   0        0        0    65291 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/templates/js/uikit-icons.min.js
--rw-r--r--   0        0        0   136629 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/templates/js/uikit.min.js
--rw-r--r--   0        0        0     2449 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/templates/logfiles.html
--rw-r--r--   0        0        0     3173 2024-05-28 13:12:45.260790 tinyticker-0.8.2/tinyticker/web/templates/startup.html
--rw-r--r--   0        0        0     5244 1970-01-01 00:00:00.000000 tinyticker-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-28 20:16:03.885182 tinyticker-0.8.3/LICENSE
+-rw-r--r--   0        0        0     3955 2024-05-28 20:16:03.885182 tinyticker-0.8.3/README.md
+-rw-r--r--   0        0        0      917 2024-05-28 20:16:03.889183 tinyticker-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0      518 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/__init__.py
+-rw-r--r--   0        0        0     4712 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/__main__.py
+-rw-r--r--   0        0        0     3263 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/config.py
+-rw-r--r--   0        0        0     4843 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/display.py
+-rw-r--r--   0        0        0     8241 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/layouts.py
+-rw-r--r--   0        0        0      345 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/paths.py
+-rw-r--r--   0        0        0     5504 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/sequence.py
+-rw-r--r--   0        0        0     1112 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/tickers/__init__.py
+-rw-r--r--   0        0        0     3451 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/tickers/_base.py
+-rw-r--r--   0        0        0     4620 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/tickers/crypto.py
+-rw-r--r--   0        0        0     3872 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/tickers/stock.py
+-rw-r--r--   0        0        0     2391 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/utils.py
+-rw-r--r--   0        0        0      278 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/__init__.py
+-rw-r--r--   0        0        0     1297 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/_base.py
+-rw-r--r--   0        0        0     4104 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/device.py
+-rw-r--r--   0        0        0     8593 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13.py
+-rw-r--r--   0        0        0    12127 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13_V2.py
+-rw-r--r--   0        0        0    14828 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13_V3.py
+-rw-r--r--   0        0        0    10709 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13_V4.py
+-rw-r--r--   0        0        0     6057 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13b_V3.py
+-rw-r--r--   0        0        0     6860 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13b_V4.py
+-rw-r--r--   0        0        0     5907 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13bc.py
+-rw-r--r--   0        0        0    21091 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in7.py
+-rw-r--r--   0        0        0    19697 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in7_V2.py
+-rw-r--r--   0        0        0     1558 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/models.py
+-rw-r--r--   0        0        0       95 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/web/__init__.py
+-rw-r--r--   0        0        0     2895 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/web/__main__.py
+-rw-r--r--   0        0        0     6825 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/web/app.py
+-rw-r--r--   0        0        0     3656 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/web/command.py
+-rw-r--r--   0        0        0      593 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/web/startup.py
+-rw-r--r--   0        0        0   274777 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/web/templates/css/uikit.min.css
+-rw-r--r--   0        0        0    12844 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/web/templates/images/apple-touch-icon.png
+-rw-r--r--   0        0        0      742 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/web/templates/images/favicon-16x16.png
+-rw-r--r--   0        0        0     1645 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/web/templates/images/favicon-32x32.png
+-rw-r--r--   0        0        0    19697 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/web/templates/index.html
+-rw-r--r--   0        0        0     3463 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/web/templates/js/index.js
+-rw-r--r--   0        0        0    65291 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/web/templates/js/uikit-icons.min.js
+-rw-r--r--   0        0        0   136629 2024-05-28 20:16:03.897183 tinyticker-0.8.3/tinyticker/web/templates/js/uikit.min.js
+-rw-r--r--   0        0        0     2449 2024-05-28 20:16:03.897183 tinyticker-0.8.3/tinyticker/web/templates/logfiles.html
+-rw-r--r--   0        0        0     3173 2024-05-28 20:16:03.897183 tinyticker-0.8.3/tinyticker/web/templates/startup.html
+-rw-r--r--   0        0        0     5244 1970-01-01 00:00:00.000000 tinyticker-0.8.3/PKG-INFO
```

### Comparing `tinyticker-0.8.2/LICENSE` & `tinyticker-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/README.md` & `tinyticker-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/pyproject.toml` & `tinyticker-0.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tinyticker"
-version = "0.8.2"
+version = "0.8.3"
 description = "A tiny Raspberry Pi powered ePaper ticker."
 authors = ["Loic Coyle <loic.coyle@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/loiccoyle/tinyticker"
 keywords = ["raspberry-pi", "ticker", "stock", "crypto", "epaper", "finance"]
```

### Comparing `tinyticker-0.8.2/tinyticker/__init__.py` & `tinyticker-0.8.3/tinyticker/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/__main__.py` & `tinyticker-0.8.3/tinyticker/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/config.py` & `tinyticker-0.8.3/tinyticker/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,15 +53,18 @@
 
     def to_file(self, file: Path) -> None:
         with file.open("w") as fp:
             json.dump(self.to_dict(), fp, indent=2)
 
     @classmethod
     def from_json(cls, json_: Union[str, bytes, bytearray]) -> "TinytickerConfig":
-        data = json.loads(json_)
+        return cls.from_dict(json.loads(json_))
+
+    @classmethod
+    def from_dict(cls, data: dict) -> "TinytickerConfig":
         # convert the layout dict to a propoer LayoutConfig object
         [
             ticker_data.update(
                 {
                     "layout": LayoutConfig(
                         **ticker_data.get("layout", dc.asdict(LayoutConfig()))
                     )
```

### Comparing `tinyticker-0.8.2/tinyticker/display.py` & `tinyticker-0.8.3/tinyticker/display.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/layouts.py` & `tinyticker-0.8.3/tinyticker/layouts.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/sequence.py` & `tinyticker-0.8.3/tinyticker/sequence.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/tickers/__init__.py` & `tinyticker-0.8.3/tinyticker/tickers/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/tickers/_base.py` & `tinyticker-0.8.3/tinyticker/tickers/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,17 @@
     if interval in WEIRD_INTERVALS
     else pd.to_timedelta(interval)
     for interval in INTERVALS
 }
 
 INTERVAL_LOOKBACKS = {
     "1m": 20,  # 20m
-    "2m": 15,  # 30m
+    "2m": 30,  # 1h
     "5m": 24,  # 2h
-    "15m": 16,  # 8h
+    "15m": 32,  # 16h
     "30m": 24,  # 12h
     "1h": 24,  # 24h
     "90m": 24,  # 36h
     "1d": 30,  # 1mo
     "5d": 30,  # 150d
     "1wk": 26,  # 6mo
     "1mo": 24,  # 2yrs
@@ -115,15 +115,15 @@
         Returns:
             Iterator over the responses.
         """
         while True:
             self._log.info("Ticker start.")
             yield self.single_tick()
             self._log.debug("Sleeping %i s", self.config.wait_time)
-            time.sleep(self.config.wait_time)  # type: ignore
+            time.sleep(self.config.wait_time)
 
     def __str__(self) -> str:
         return "\t".join(
             [
                 "Ticker",
                 self.config.symbol_type,
                 self.config.symbol,
```

### Comparing `tinyticker-0.8.2/tinyticker/tickers/crypto.py` & `tinyticker-0.8.3/tinyticker/tickers/crypto.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/tickers/stock.py` & `tinyticker-0.8.3/tinyticker/tickers/stock.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/utils.py` & `tinyticker-0.8.3/tinyticker/utils.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/waveshare_lib/_base.py` & `tinyticker-0.8.3/tinyticker/waveshare_lib/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/waveshare_lib/device.py` & `tinyticker-0.8.3/tinyticker/waveshare_lib/device.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13.py` & `tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13_V2.py` & `tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13_V3.py` & `tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13_V4.py` & `tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13b_V3.py` & `tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13b_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13b_V4.py` & `tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13b_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in13bc.py` & `tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13bc.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in7.py` & `tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in7.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/waveshare_lib/epd2in7_V2.py` & `tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in7_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/waveshare_lib/models.py` & `tinyticker-0.8.3/tinyticker/waveshare_lib/models.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/web/__main__.py` & `tinyticker-0.8.3/tinyticker/web/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/web/app.py` & `tinyticker-0.8.3/tinyticker/web/app.py`

 * *Files 21% similar despite different names*

```diff
@@ -95,62 +95,22 @@
             **tt_config.to_dict(),
         )
 
     @app.route("/logfiles")
     def logs():
         return render_template("logfiles.html", log_files=log_files)
 
-    @app.route("/config")
+    @app.route("/config", methods=["POST"])
     def config():
-        # TODO: post the config via a json post instead of parsing it here
-        # Something like:
-        # https://stackoverflow.com/questions/22195065/how-to-send-a-json-object-using-html-form-data
-        LOGGER.debug("/config url args: %s", request.args)
-        tickers = {}
-        tickers["symbol"] = request.args.getlist("symbol")
-        tickers["symbol_type"] = request.args.getlist("symbol_type")
-        tickers["plot_type"] = request.args.getlist("plot_type")
-        tickers["interval"] = request.args.getlist("interval")
-        tickers["lookback"] = request.args.getlist("lookback", type=no_empty_int)
-        tickers["wait_time"] = request.args.getlist("wait_time", type=no_empty_int)
-        tickers["mav"] = request.args.getlist("mav", type=no_empty_int)
-        tickers["volume"] = request.args.getlist("volume", type=str_to_bool)
-        tickers["avg_buy_price"] = request.args.getlist(
-            "avg_buy_price", type=no_empty_float
-        )
-        tickers["prepost"] = request.args.getlist("prepost", type=str_to_bool)
-
-        layouts = {}
-        layouts["name"] = request.args.getlist("layout_name")
-        layouts["y_axis"] = request.args.getlist("layout_y_axis", type=str_to_bool)
-        layouts["x_gaps"] = request.args.getlist("layout_x_gaps", type=str_to_bool)
-        layouts = [
-            LayoutConfig(**dict(zip(layouts, l)))
-            for l in zip(*layouts.values())  # noqa: E741
-        ]
-
-        tickers["layout"] = layouts
+        """Post the config via a json post instead of parsing it here."""
+        LOGGER.debug("/config request.json: %s", request.json)
+        if not request.json:
+            abort(400)
 
-        sequence = SequenceConfig(
-            skip_outdated=request.args.get("skip_outdated", False, type=bool),
-            # NOTE: currently not toggleable from the web app
-            skip_empty=request.args.get("skip_empty", True, type=bool),
-        )
-
-        # invert the ticker dict of list to list of dict and create ticker list
-        tickers = [
-            TickerConfig(**dict(zip(tickers, t))) for t in zip(*tickers.values())
-        ]
-        tt_config = TinytickerConfig(
-            api_key=request.args.get("api_key", type=no_empty_str),
-            flip=request.args.get("flip", default=False, type=bool),
-            epd_model=request.args.get("epd_model", "EPD_v3"),
-            tickers=tickers,
-            sequence=sequence,
-        )
+        tt_config = TinytickerConfig.from_dict(request.json)
         LOGGER.debug(tt_config)
         # writing the config to file, the main ticker process is monitoring this file
         # and will refresh the ticker process
         tt_config.to_file(config_file)
         return redirect("/", code=302)
 
     @app.route("/command")
```

### Comparing `tinyticker-0.8.2/tinyticker/web/command.py` & `tinyticker-0.8.3/tinyticker/web/command.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/web/startup.py` & `tinyticker-0.8.3/tinyticker/web/startup.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/web/templates/css/uikit.min.css` & `tinyticker-0.8.3/tinyticker/web/templates/css/uikit.min.css`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/web/templates/images/apple-touch-icon.png` & `tinyticker-0.8.3/tinyticker/web/templates/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/web/templates/images/favicon-16x16.png` & `tinyticker-0.8.3/tinyticker/web/templates/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/web/templates/images/favicon-32x32.png` & `tinyticker-0.8.3/tinyticker/web/templates/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/web/templates/index.html` & `tinyticker-0.8.3/tinyticker/web/templates/index.html`

 * *Files 20% similar despite different names*

```diff
@@ -70,15 +70,15 @@
               id="hostname"
               name="hostname"
               value="{{ hostname }}"
             />
             <input class="uk-button-small" type="submit" value="Set & Reboot" />
           </form>
           <hr />
-          <form class="uk-form-stacked uk-width-1-1" action="/config">
+          <form id="form-config" class="uk-form-stacked uk-width-1-1">
             <div class="uk-flex uk-flex-middle uk-margin-small-bottom">
               <span
                 uk-icon="icon: tv; ratio: 2"
                 class="uk-padding-small uk-padding-remove-vertical"
                 style="width: 40px;"
               ></span>
               <select
@@ -149,229 +149,238 @@
                       type="button"
                       uk-close
                       onclick="remove_ticker(this)"
                     ></button>
                   </div>
 
                   <div class="uk-flex uk-flex-between">
-                    <label class="uk-form-label" for="symbol_type">
+                    <label class="uk-form-label" for="ticker-symbol_type">
                       Symbol type
                     </label>
                     <select
                       class="uk-select uk-form-small uk-width-1-3"
-                      id="symbol_type"
-                      name="symbol_type"
+                      id="ticker-symbol_type"
+                      name="ticker-symbol_type"
                       onchange="hide_prepost(this)"
                     >
                       {%- for symbol_type_option in symbol_type_options -%}
                         <option
                           value="{{ symbol_type_option }}"
                           {% if symbol_type_option == ticker.symbol_type %}selected{% endif %}
                         >
                           {{ symbol_type_option }}
                         </option>
                       {%- endfor -%}
                     </select>
                   </div>
 
                   <div class="uk-flex uk-flex-between">
-                    <label class="uk-form-label" for="symbol">Symbol</label>
+                    <label class="uk-form-label" for="ticker-symbol">
+                      Symbol
+                    </label>
                     <input
                       class="uk-input uk-form-small uk-width-1-3"
                       type="text"
-                      id="symbol"
-                      name="symbol"
+                      id="ticker-symbol"
+                      name="ticker-symbol"
                       value="{{ ticker.symbol }}"
                     />
                   </div>
 
                   <div class="uk-flex uk-flex-between">
-                    <label class="uk-form-label" for="interval">Interval</label>
+                    <label class="uk-form-label" for="ticker-interval">
+                      Interval
+                    </label>
                     <select
                       class="uk-select uk-form-small uk-width-1-3"
-                      id="interval"
-                      name="interval"
+                      id="ticker-interval"
+                      name="ticker-interval"
                     >
                       {%- for interval_option in interval_options -%}
                         <option
                           value="{{ interval_option }}"
                           {% if interval_option == ticker.interval %}selected{% endif %}
                         >
                           {{ interval_option }}
                         </option>
                       {%- endfor -%}
                     </select>
                   </div>
 
                   <div class="uk-flex uk-flex-between">
-                    <label class="uk-form-label" for="plot_type">
+                    <label class="uk-form-label" for="ticker-plot_type">
                       Plot type
                     </label>
                     <select
                       class="uk-select uk-form-small uk-width-1-3"
-                      id="plot_type"
-                      name="plot_type"
+                      id="ticker-plot_type"
+                      name="ticker-plot_type"
                     >
                       {%- for plot_type_option in plot_type_options -%}
                         <option
                           value="{{ plot_type_option }}"
                           {% if plot_type_option == ticker.plot_type %}selected{% endif %}
                         >
                           {{ plot_type_option }}
                         </option>
                       {%- endfor -%}
                     </select>
                   </div>
 
                   <div class="uk-flex uk-flex-between">
-                    <label class="uk-form-label" for="lookback">Lookback</label>
+                    <label class="uk-form-label" for="ticker-lookback">
+                      Lookback
+                    </label>
                     <input
                       class="uk-input uk-form-small uk-width-1-3"
                       inputmode="numeric"
-                      id="lookback"
-                      name="lookback"
+                      id="ticker-lookback"
+                      name="ticker-lookback"
                       min="1"
                       uk-tooltip="Number of intervals to look back for."
                       {#- If the look back is None then it has not been set so use the default lookback for the interval #}
                       {% if ticker.lookback is none %}placeholder="{{ interval_lookbacks[ticker.interval] }}"{% else %}value="{{ ticker.lookback }}"{% endif %}
                     />
                   </div>
 
                   <div class="uk-flex uk-flex-between">
-                    <label class="uk-form-label" for="wait_time">
+                    <label class="uk-form-label" for="ticker-wait_time">
                       Wait time (s)
                     </label>
                     <input
                       class="uk-input uk-form-small uk-width-1-3"
                       inputmode="numeric"
-                      id="wait_time"
-                      name="wait_time"
+                      id="ticker-wait_time"
+                      name="ticker-wait_time"
                       min="1"
                       uk-tooltip="Time to wait on this ticker."
                       value="{{ ticker.wait_time }}"
                     />
                   </div>
 
                   <div class="uk-flex uk-flex-between">
-                    <label class="uk-form-label" for="mav">
+                    <label class="uk-form-label" for="ticker-mav">
                       Moving average
                     </label>
                     <input
                       class="uk-input uk-form-small uk-width-1-3"
                       inputmode="numeric"
-                      id="mav"
-                      name="mav"
+                      id="ticker-mav"
+                      name="ticker-mav"
                       min="1"
                       uk-tooltip="Optional, number of intervals to include in the moving average."
                       value="{{ ticker.mav if ticker.mav is not none }}"
                     />
                   </div>
 
                   <div class="uk-flex uk-flex-between">
-                    <label class="uk-form-label" for="avg_buy_price">
+                    <label class="uk-form-label" for="ticker-avg_buy_price">
                       Average buy price
                     </label>
                     <input
                       class="uk-input uk-form-small uk-width-1-3"
                       inputmode="numeric"
-                      id="avg_buy_price"
-                      name="avg_buy_price"
+                      id="ticker-avg_buy_price"
+                      name="ticker-avg_buy_price"
                       min="0"
                       value="{{ ticker.avg_buy_price if ticker.avg_buy_price is not none }}"
                       uk-tooltip="Optional, used to display percentage change from buy price."
                     />
                   </div>
 
                   <label
                     class="uk-form-label"
-                    for="volume"
+                    for="ticker-volume"
                     uk-tooltip="Add a trade volume plot bellow the graph."
                   >
                     <input
                       type="hidden"
-                      name="volume"
+                      id="ticker-volume"
+                      name="ticker-volume"
                       value="{{ 1 if ticker.volume | default(False) else 0 }}"
                     />
                     <input
                       class="uk-checkbox"
                       type="checkbox"
                       {% if ticker.volume | default(False) %}checked{% endif %}
                       onclick="this.previousElementSibling.value=1-this.previousElementSibling.value"
                     />
                     Show trade volume
                   </label>
 
                   <label
                     class="uk-form-label"
-                    for="prepost"
+                    for="ticker-prepost"
                     uk-tooltip="Show pre/post market stock data."
                   >
                     <input
                       type="hidden"
-                      id="prepost"
-                      name="prepost"
+                      id="ticker-prepost"
+                      name="ticker-prepost"
                       value="{{ 1 if ticker.prepost | default(False) else 0 }}"
                     />
                     <input
                       class="uk-checkbox"
                       type="checkbox"
                       {% if ticker.prepost| default(False) %}checked{% endif %}
                       onclick="this.previousElementSibling.value=1-this.previousElementSibling.value"
                     />
                     Fetch pre/post market data
                   </label>
 
                   <hr />
                   <div class="uk-flex uk-flex-between">
-                    <label class="uk-form-label" for="symbol_type">
+                    <label class="uk-form-label" for="ticker-layout-name">
                       Layout
                     </label>
                     <select
                       class="uk-select uk-form-small uk-width-1-3"
-                      id="layout_name"
-                      name="layout_name"
+                      name="ticker-layout-name"
+                      id="ticker-layout-name"
                     >
                       {%- for layout_option in layout_options -%}
                         <option
                           value="{{ layout_option.name }}"
                           {% if layout_option.name == ticker.layout.name %}selected{% endif %}
                         >
                           {{ layout_option.name }}
                         </option>
                       {%- endfor -%}
                     </select>
                   </div>
 
                   <label
                     class="uk-form-label"
-                    for="layout_y_axis"
+                    for="ticker-layout-y_axis"
                     uk-tooltip="Show the y axis of the plot."
                   >
                     <input
                       type="hidden"
-                      name="layout_y_axis"
+                      name="ticker-layout-y_axis"
+                      id="ticker-layout-y_axis"
                       value="{{ 1 if ticker.layout.y_axis | default(False) else 0 }}"
                     />
                     <input
                       class="uk-checkbox"
                       type="checkbox"
                       {% if ticker.layout.y_axis | default(False) %}checked{% endif %}
                       onclick="this.previousElementSibling.value=1-this.previousElementSibling.value"
                     />
                     Show y axis
                   </label>
 
                   <label
                     class="uk-form-label"
-                    for="layout_x_gaps"
+                    for="ticker-layout-x_gaps"
                     uk-tooltip="Add a vertical line to show time gaps, i.e. closed market & weekends."
                   >
                     <input
                       type="hidden"
-                      name="layout_x_gaps"
+                      id="ticker-layout-x_gaps"
+                      name="ticker-layout-x_gaps"
                       value="{{ 1 if ticker.layout.x_gaps | default(False) else 0 }}"
                     />
                     <input
                       class="uk-checkbox"
                       type="checkbox"
                       {% if ticker.layout.x_gaps | default(True) %}checked{% endif %}
                       onclick="this.previousElementSibling.value=1-this.previousElementSibling.value"
@@ -387,24 +396,31 @@
               >
                 <span uk-icon="plus"></span>
               </div>
             </div>
             <div class="uk-width-1-1 uk-margin">
               <label
                 class="uk-form-label"
-                for="skip_outdated"
+                for="sequence-skip_outdated"
                 uk-tooltip="Typically happens when the market is closed."
-                ><input
+              >
+                <input
+                  type="hidden"
+                  id="sequence-skip_outdated"
+                  name="sequence-skip_outdated"
+                  value="{{ 1 if sequence.skip_outdated | default(False) else 0 }}"
+                />
+                <input
                   class="uk-checkbox uk-margin-small-right"
                   type="checkbox"
-                  id="skip_outdated"
-                  name="skip_outdated"
                   {% if sequence.skip_outdated | default(True) %}checked{% endif %}
-                />Skip tickers with outdated data</label
-              >
+                  onclick="this.previousElementSibling.value=1-this.previousElementSibling.value"
+                />
+                Skip tickers with outdated data
+              </label>
               <button
                 type="submit"
                 value="submit"
                 class="uk-button uk-button-primary uk-width-expand"
               >
                 Apply
               </button>
@@ -428,38 +444,57 @@
               {% endfor %}
             </form>
           </div>
         </div>
       </div>
     </div>
     <div class="uk-text-center uk-position-small">
-      <span class="uk-text-small uk-text-muted"
-        >TinyTicker v{{ version }} - <span uk-icon="github"></span
-        ><a
+      <span class="uk-text-small uk-text-muted">
+        TinyTicker v{{ version }} - <span uk-icon="github"></span>
+        <a
           href="https://github.com/loiccoyle/tinyticker"
           title="tinyticker"
           target="_blank"
-          >TinyTicker</a
         >
-        - <span uk-icon="question"></span
-        ><a
+          TinyTicker
+        </a>
+        - <span uk-icon="question"></span>
+        <a
           href="https://github.com/loiccoyle/tinyticker/issues/new"
           title="issues"
           target="_blank"
-          >Report an issue</a
         >
+          Report an issue
+        </a>
       </span>
     </div>
   </body>
   <script>
     checkForUpdate("{{version}}").then((isUpdateAvailable) => {
       document.getElementById("updateDiv").style.display = isUpdateAvailable
         ? "block"
         : "none";
     });
 
     // run hide_prepost on all tickers
-    document.querySelectorAll("#symbol_type").forEach((element) => {
+    document.querySelectorAll("#ticker-symbol_type").forEach((element) => {
       hide_prepost(element);
     });
+
+    // post the form json to the config endpoint when the form is submitted
+    document
+      .querySelector("#form-config")
+      .addEventListener("submit", (event) => {
+        event.preventDefault();
+        fetch("/config", {
+          method: "POST",
+          headers: {
+            "Content-Type": "application/json",
+          },
+          body: JSON.stringify(formToJson(event.target)),
+        }).then(() => {
+          // refresh the page
+          document.location.reload();
+        });
+      });
   </script>
 </html>
```

#### html2text {}

```diff
@@ -52,12 +52,13 @@
 % if ticker.layout.y_axis | default(False) %}checked{% endif %}
 onclick="this.previousElementSibling.value=1-this.previousElementSibling.value"
 /> Show y axis
 % if ticker.layout.x_gaps | default(True) %}checked{% endif %}
 onclick="this.previousElementSibling.value=1-this.previousElementSibling.value"
 /> Add line on time gap
 {%- endfor -%}
-% if sequence.skip_outdated | default(True) %}checked{% endif %} />Skip tickers
-with outdated data Apply
+% if sequence.skip_outdated | default(True) %}checked{% endif %}
+onclick="this.previousElementSibling.value=1-this.previousElementSibling.value"
+/> Skip tickers with outdated data Apply
 ===============================================================================
 {% for command, desc in commands | items %} {{ command.title() }} {% endfor %}
-TinyTicker v{{ version }} - _T_i_n_y_T_i_c_k_e_r - _R_e_p_o_r_t_ _a_n_ _i_s_s_u_e
+TinyTicker v{{ version }} - _T_i_n_y_T_i_c_k_e_r_ - _R_e_p_o_r_t_ _a_n_ _i_s_s_u_e
```

### Comparing `tinyticker-0.8.2/tinyticker/web/templates/js/uikit-icons.min.js` & `tinyticker-0.8.3/tinyticker/web/templates/js/uikit-icons.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/web/templates/js/uikit.min.js` & `tinyticker-0.8.3/tinyticker/web/templates/js/uikit.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/tinyticker/web/templates/logfiles.html` & `tinyticker-0.8.3/tinyticker/web/templates/logfiles.html`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
           });
       }
       // update the content of all log files every 60s
       function updateAllLogFileContent() {
         {% for log_file in log_files %}
           updateLogFileContent('{{ log_file }}');
         {% endfor %}
-        setTimeout(updateAllLogFileContent, 60000);
+        setTimeout(updateAllLogFileContent, 10000);
       }
       // start updating the content of all log files
       updateAllLogFileContent();
     </script>
   </head>
   <body class="uk-background-muted uk-height-1-1 uk-padding-small">
     <div class="uk-text-center uk-margin">
```

### Comparing `tinyticker-0.8.2/tinyticker/web/templates/startup.html` & `tinyticker-0.8.3/tinyticker/web/templates/startup.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.2/PKG-INFO` & `tinyticker-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyticker
-Version: 0.8.2
+Version: 0.8.3
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
-Metadata-Version: 2.1 Name: tinyticker Version: 0.8.2 Summary: A tiny Raspberry
+Metadata-Version: 2.1 Name: tinyticker Version: 0.8.3 Summary: A tiny Raspberry
 Pi powered ePaper ticker. Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance Author:
 Loic Coyle Author-email: loic.coyle@hotmail.fr Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

