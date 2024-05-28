# Comparing `tmp/tinyticker-0.8.3.tar.gz` & `tmp/tinyticker-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyticker-0.8.3.tar", max compression
+gzip compressed data, was "tinyticker-0.8.4.tar", max compression
```

## Comparing `tinyticker-0.8.3.tar` & `tinyticker-0.8.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1068 2024-05-28 20:16:03.885182 tinyticker-0.8.3/LICENSE
--rw-r--r--   0        0        0     3955 2024-05-28 20:16:03.885182 tinyticker-0.8.3/README.md
--rw-r--r--   0        0        0      917 2024-05-28 20:16:03.889183 tinyticker-0.8.3/pyproject.toml
--rw-r--r--   0        0        0      518 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/__init__.py
--rw-r--r--   0        0        0     4712 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/__main__.py
--rw-r--r--   0        0        0     3263 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/config.py
--rw-r--r--   0        0        0     4843 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/display.py
--rw-r--r--   0        0        0     8241 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/layouts.py
--rw-r--r--   0        0        0      345 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/paths.py
--rw-r--r--   0        0        0     5504 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/sequence.py
--rw-r--r--   0        0        0     1112 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/tickers/__init__.py
--rw-r--r--   0        0        0     3451 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/tickers/_base.py
--rw-r--r--   0        0        0     4620 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/tickers/crypto.py
--rw-r--r--   0        0        0     3872 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/tickers/stock.py
--rw-r--r--   0        0        0     2391 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/utils.py
--rw-r--r--   0        0        0      278 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/__init__.py
--rw-r--r--   0        0        0     1297 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/_base.py
--rw-r--r--   0        0        0     4104 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/device.py
--rw-r--r--   0        0        0     8593 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13.py
--rw-r--r--   0        0        0    12127 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13_V2.py
--rw-r--r--   0        0        0    14828 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13_V3.py
--rw-r--r--   0        0        0    10709 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13_V4.py
--rw-r--r--   0        0        0     6057 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13b_V3.py
--rw-r--r--   0        0        0     6860 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13b_V4.py
--rw-r--r--   0        0        0     5907 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13bc.py
--rw-r--r--   0        0        0    21091 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in7.py
--rw-r--r--   0        0        0    19697 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in7_V2.py
--rw-r--r--   0        0        0     1558 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/waveshare_lib/models.py
--rw-r--r--   0        0        0       95 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/web/__init__.py
--rw-r--r--   0        0        0     2895 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/web/__main__.py
--rw-r--r--   0        0        0     6825 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/web/app.py
--rw-r--r--   0        0        0     3656 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/web/command.py
--rw-r--r--   0        0        0      593 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/web/startup.py
--rw-r--r--   0        0        0   274777 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/web/templates/css/uikit.min.css
--rw-r--r--   0        0        0    12844 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/web/templates/images/apple-touch-icon.png
--rw-r--r--   0        0        0      742 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/web/templates/images/favicon-16x16.png
--rw-r--r--   0        0        0     1645 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/web/templates/images/favicon-32x32.png
--rw-r--r--   0        0        0    19697 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/web/templates/index.html
--rw-r--r--   0        0        0     3463 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/web/templates/js/index.js
--rw-r--r--   0        0        0    65291 2024-05-28 20:16:03.893183 tinyticker-0.8.3/tinyticker/web/templates/js/uikit-icons.min.js
--rw-r--r--   0        0        0   136629 2024-05-28 20:16:03.897183 tinyticker-0.8.3/tinyticker/web/templates/js/uikit.min.js
--rw-r--r--   0        0        0     2449 2024-05-28 20:16:03.897183 tinyticker-0.8.3/tinyticker/web/templates/logfiles.html
--rw-r--r--   0        0        0     3173 2024-05-28 20:16:03.897183 tinyticker-0.8.3/tinyticker/web/templates/startup.html
--rw-r--r--   0        0        0     5244 1970-01-01 00:00:00.000000 tinyticker-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-28 21:15:03.187171 tinyticker-0.8.4/LICENSE
+-rw-r--r--   0        0        0     3955 2024-05-28 21:15:03.187171 tinyticker-0.8.4/README.md
+-rw-r--r--   0        0        0      917 2024-05-28 21:15:03.191171 tinyticker-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0      518 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/__init__.py
+-rw-r--r--   0        0        0     4712 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/__main__.py
+-rw-r--r--   0        0        0     3263 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/config.py
+-rw-r--r--   0        0        0     4843 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/display.py
+-rw-r--r--   0        0        0     8241 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/layouts.py
+-rw-r--r--   0        0        0      345 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/paths.py
+-rw-r--r--   0        0        0     5504 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/sequence.py
+-rw-r--r--   0        0        0     1112 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/tickers/__init__.py
+-rw-r--r--   0        0        0     3451 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/tickers/_base.py
+-rw-r--r--   0        0        0     4620 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/tickers/crypto.py
+-rw-r--r--   0        0        0     4093 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/tickers/stock.py
+-rw-r--r--   0        0        0     2391 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/utils.py
+-rw-r--r--   0        0        0      278 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/waveshare_lib/__init__.py
+-rw-r--r--   0        0        0     1297 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/waveshare_lib/_base.py
+-rw-r--r--   0        0        0     4104 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/waveshare_lib/device.py
+-rw-r--r--   0        0        0     8593 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/waveshare_lib/epd2in13.py
+-rw-r--r--   0        0        0    12127 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/waveshare_lib/epd2in13_V2.py
+-rw-r--r--   0        0        0    14828 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/waveshare_lib/epd2in13_V3.py
+-rw-r--r--   0        0        0    10709 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/waveshare_lib/epd2in13_V4.py
+-rw-r--r--   0        0        0     6057 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/waveshare_lib/epd2in13b_V3.py
+-rw-r--r--   0        0        0     6860 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/waveshare_lib/epd2in13b_V4.py
+-rw-r--r--   0        0        0     5907 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/waveshare_lib/epd2in13bc.py
+-rw-r--r--   0        0        0    21091 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/waveshare_lib/epd2in7.py
+-rw-r--r--   0        0        0    19697 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/waveshare_lib/epd2in7_V2.py
+-rw-r--r--   0        0        0     1558 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/waveshare_lib/models.py
+-rw-r--r--   0        0        0       95 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/web/__init__.py
+-rw-r--r--   0        0        0     2895 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/web/__main__.py
+-rw-r--r--   0        0        0     6825 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/web/app.py
+-rw-r--r--   0        0        0     3656 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/web/command.py
+-rw-r--r--   0        0        0      593 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/web/startup.py
+-rw-r--r--   0        0        0   274777 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/web/templates/css/uikit.min.css
+-rw-r--r--   0        0        0    12844 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/web/templates/images/apple-touch-icon.png
+-rw-r--r--   0        0        0      742 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/web/templates/images/favicon-16x16.png
+-rw-r--r--   0        0        0     1645 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/web/templates/images/favicon-32x32.png
+-rw-r--r--   0        0        0    19697 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/web/templates/index.html
+-rw-r--r--   0        0        0     3463 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/web/templates/js/index.js
+-rw-r--r--   0        0        0    65291 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/web/templates/js/uikit-icons.min.js
+-rw-r--r--   0        0        0   136629 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/web/templates/js/uikit.min.js
+-rw-r--r--   0        0        0     2449 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/web/templates/logfiles.html
+-rw-r--r--   0        0        0     3173 2024-05-28 21:15:03.195170 tinyticker-0.8.4/tinyticker/web/templates/startup.html
+-rw-r--r--   0        0        0     5244 1970-01-01 00:00:00.000000 tinyticker-0.8.4/PKG-INFO
```

### Comparing `tinyticker-0.8.3/LICENSE` & `tinyticker-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/README.md` & `tinyticker-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/pyproject.toml` & `tinyticker-0.8.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tinyticker"
-version = "0.8.3"
+version = "0.8.4"
 description = "A tiny Raspberry Pi powered ePaper ticker."
 authors = ["Loic Coyle <loic.coyle@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/loiccoyle/tinyticker"
 keywords = ["raspberry-pi", "ticker", "stock", "crypto", "epaper", "finance"]
```

### Comparing `tinyticker-0.8.3/tinyticker/__init__.py` & `tinyticker-0.8.4/tinyticker/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/__main__.py` & `tinyticker-0.8.4/tinyticker/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/config.py` & `tinyticker-0.8.4/tinyticker/config.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/display.py` & `tinyticker-0.8.4/tinyticker/display.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/layouts.py` & `tinyticker-0.8.4/tinyticker/layouts.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/sequence.py` & `tinyticker-0.8.4/tinyticker/sequence.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/tickers/__init__.py` & `tinyticker-0.8.4/tinyticker/tickers/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/tickers/_base.py` & `tinyticker-0.8.4/tinyticker/tickers/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/tickers/crypto.py` & `tinyticker-0.8.4/tinyticker/tickers/crypto.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/tickers/stock.py` & `tinyticker-0.8.4/tinyticker/tickers/stock.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,17 @@
         # max(0, start.weekday() - 4) is 0 for Mon-Fri, 1 for Sat, 2 for Sun
         start -= pd.to_timedelta("1d") * max(0, start.weekday() - 4)
         return (start, end)
 
     def _fix_prepost(self, historical: pd.DataFrame) -> pd.DataFrame:
         # when the market is closed, the volume is 0
         prepost_range = historical["Volume"] == 0
+        # add one more row before and after open/close to make sure we don't miss the start/end
+        prepost_range |= prepost_range.shift(-1).fillna(False)
+        prepost_range |= prepost_range.shift(1).fillna(False)
         # When in prepost, the high & lows can be off
         high_bars = historical["High"] - historical[["Close", "Open"]].max(axis=1)
         low_bars = historical[["Close", "Open"]].min(axis=1) - historical["Low"]
 
         to_correct_high = high_bars[prepost_range] > high_bars.mean() + high_bars.std()
         to_correct_low = low_bars[prepost_range] > low_bars.mean() + low_bars.std()
         # we could also set them to the avg of the previous and next high/low
```

### Comparing `tinyticker-0.8.3/tinyticker/utils.py` & `tinyticker-0.8.4/tinyticker/utils.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/waveshare_lib/_base.py` & `tinyticker-0.8.4/tinyticker/waveshare_lib/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/waveshare_lib/device.py` & `tinyticker-0.8.4/tinyticker/waveshare_lib/device.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13.py` & `tinyticker-0.8.4/tinyticker/waveshare_lib/epd2in13.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13_V2.py` & `tinyticker-0.8.4/tinyticker/waveshare_lib/epd2in13_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13_V3.py` & `tinyticker-0.8.4/tinyticker/waveshare_lib/epd2in13_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13_V4.py` & `tinyticker-0.8.4/tinyticker/waveshare_lib/epd2in13_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13b_V3.py` & `tinyticker-0.8.4/tinyticker/waveshare_lib/epd2in13b_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13b_V4.py` & `tinyticker-0.8.4/tinyticker/waveshare_lib/epd2in13b_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in13bc.py` & `tinyticker-0.8.4/tinyticker/waveshare_lib/epd2in13bc.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in7.py` & `tinyticker-0.8.4/tinyticker/waveshare_lib/epd2in7.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/waveshare_lib/epd2in7_V2.py` & `tinyticker-0.8.4/tinyticker/waveshare_lib/epd2in7_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/waveshare_lib/models.py` & `tinyticker-0.8.4/tinyticker/waveshare_lib/models.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/web/__main__.py` & `tinyticker-0.8.4/tinyticker/web/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/web/app.py` & `tinyticker-0.8.4/tinyticker/web/app.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/web/command.py` & `tinyticker-0.8.4/tinyticker/web/command.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/web/startup.py` & `tinyticker-0.8.4/tinyticker/web/startup.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/web/templates/css/uikit.min.css` & `tinyticker-0.8.4/tinyticker/web/templates/css/uikit.min.css`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/web/templates/images/apple-touch-icon.png` & `tinyticker-0.8.4/tinyticker/web/templates/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/web/templates/images/favicon-16x16.png` & `tinyticker-0.8.4/tinyticker/web/templates/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/web/templates/images/favicon-32x32.png` & `tinyticker-0.8.4/tinyticker/web/templates/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/web/templates/index.html` & `tinyticker-0.8.4/tinyticker/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/web/templates/js/index.js` & `tinyticker-0.8.4/tinyticker/web/templates/js/index.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/web/templates/js/uikit-icons.min.js` & `tinyticker-0.8.4/tinyticker/web/templates/js/uikit-icons.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/web/templates/js/uikit.min.js` & `tinyticker-0.8.4/tinyticker/web/templates/js/uikit.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/web/templates/logfiles.html` & `tinyticker-0.8.4/tinyticker/web/templates/logfiles.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/tinyticker/web/templates/startup.html` & `tinyticker-0.8.4/tinyticker/web/templates/startup.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.8.3/PKG-INFO` & `tinyticker-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyticker
-Version: 0.8.3
+Version: 0.8.4
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
-Metadata-Version: 2.1 Name: tinyticker Version: 0.8.3 Summary: A tiny Raspberry
+Metadata-Version: 2.1 Name: tinyticker Version: 0.8.4 Summary: A tiny Raspberry
 Pi powered ePaper ticker. Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance Author:
 Loic Coyle Author-email: loic.coyle@hotmail.fr Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

