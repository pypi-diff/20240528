# Comparing `tmp/quantstats-lumi-0.2.0.tar.gz` & `tmp/quantstats-lumi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantstats-lumi-0.2.0.tar", last modified: Sun Mar 31 03:36:15 2024, max compression
+gzip compressed data, was "quantstats-lumi-0.3.0.tar", last modified: Tue May 28 07:34:19 2024, max compression
```

## Comparing `quantstats-lumi-0.2.0.tar` & `quantstats-lumi-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-03-31 03:36:15.486528 quantstats-lumi-0.2.0/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    11358 2024-03-19 10:30:17.000000 quantstats-lumi-0.2.0/LICENSE.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      154 2024-03-19 10:30:17.000000 quantstats-lumi-0.2.0/MANIFEST.in
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    10144 2024-03-31 03:36:15.486404 quantstats-lumi-0.2.0/PKG-INFO
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     8483 2024-03-19 10:30:17.000000 quantstats-lumi-0.2.0/README.rst
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-03-31 03:36:15.482887 quantstats-lumi-0.2.0/quantstats_lumi/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     5526 2024-03-19 10:30:17.000000 quantstats-lumi-0.2.0/quantstats_lumi/__init__.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-03-31 03:36:15.485242 quantstats-lumi-0.2.0/quantstats_lumi/_plotting/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      718 2024-03-19 10:30:17.000000 quantstats-lumi-0.2.0/quantstats_lumi/_plotting/__init__.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    33041 2024-03-31 03:00:03.000000 quantstats-lumi-0.2.0/quantstats_lumi/_plotting/core.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    26934 2024-03-31 03:00:03.000000 quantstats-lumi-0.2.0/quantstats_lumi/_plotting/wrappers.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      886 2024-03-19 10:30:17.000000 quantstats-lumi-0.2.0/quantstats_lumi/plots.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     4691 2024-03-31 03:32:10.000000 quantstats-lumi-0.2.0/quantstats_lumi/report.html
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    57065 2024-03-31 03:34:06.000000 quantstats-lumi-0.2.0/quantstats_lumi/reports.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    37321 2024-03-31 03:00:03.000000 quantstats-lumi-0.2.0/quantstats_lumi/stats.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    13791 2024-03-19 10:30:17.000000 quantstats-lumi-0.2.0/quantstats_lumi/utils.py
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       18 2024-03-31 03:35:19.000000 quantstats-lumi-0.2.0/quantstats_lumi/version.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-03-31 03:36:15.486095 quantstats-lumi-0.2.0/quantstats_lumi.egg-info/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)    10144 2024-03-31 03:36:15.000000 quantstats-lumi-0.2.0/quantstats_lumi.egg-info/PKG-INFO
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      623 2024-03-31 03:36:15.000000 quantstats-lumi-0.2.0/quantstats_lumi.egg-info/SOURCES.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)        1 2024-03-31 03:36:15.000000 quantstats-lumi-0.2.0/quantstats_lumi.egg-info/dependency_links.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       39 2024-03-31 03:36:15.000000 quantstats-lumi-0.2.0/quantstats_lumi.egg-info/entry_points.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      145 2024-03-31 03:36:15.000000 quantstats-lumi-0.2.0/quantstats_lumi.egg-info/requires.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       16 2024-03-31 03:36:15.000000 quantstats-lumi-0.2.0/quantstats_lumi.egg-info/top_level.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)      145 2024-03-31 03:00:03.000000 quantstats-lumi-0.2.0/requirements.txt
--rw-r--r--   0 robertgrzesik   (501) staff       (20)       67 2024-03-31 03:36:15.486737 quantstats-lumi-0.2.0/setup.cfg
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     2939 2024-03-19 10:30:17.000000 quantstats-lumi-0.2.0/setup.py
-drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-03-31 03:36:15.485751 quantstats-lumi-0.2.0/tests/
--rw-r--r--   0 robertgrzesik   (501) staff       (20)     3366 2024-03-31 03:31:38.000000 quantstats-lumi-0.2.0/tests/test_reports.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-28 07:34:19.636792 quantstats-lumi-0.3.0/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    11358 2024-03-19 10:30:17.000000 quantstats-lumi-0.3.0/LICENSE.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      154 2024-03-19 10:30:17.000000 quantstats-lumi-0.3.0/MANIFEST.in
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    10144 2024-05-28 07:34:19.636665 quantstats-lumi-0.3.0/PKG-INFO
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     8483 2024-03-19 10:30:17.000000 quantstats-lumi-0.3.0/README.rst
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-28 07:34:19.634968 quantstats-lumi-0.3.0/quantstats_lumi/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     5526 2024-03-19 10:30:17.000000 quantstats-lumi-0.3.0/quantstats_lumi/__init__.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-28 07:34:19.636078 quantstats-lumi-0.3.0/quantstats_lumi/_plotting/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      718 2024-03-19 10:30:17.000000 quantstats-lumi-0.3.0/quantstats_lumi/_plotting/__init__.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    33041 2024-03-31 03:00:03.000000 quantstats-lumi-0.3.0/quantstats_lumi/_plotting/core.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    26934 2024-03-31 03:00:03.000000 quantstats-lumi-0.3.0/quantstats_lumi/_plotting/wrappers.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      886 2024-03-19 10:30:17.000000 quantstats-lumi-0.3.0/quantstats_lumi/plots.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     9453 2024-05-28 06:20:33.000000 quantstats-lumi-0.3.0/quantstats_lumi/report.html
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    57284 2024-05-28 07:31:39.000000 quantstats-lumi-0.3.0/quantstats_lumi/reports.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    37321 2024-03-31 03:00:03.000000 quantstats-lumi-0.3.0/quantstats_lumi/stats.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    13791 2024-03-19 10:30:17.000000 quantstats-lumi-0.3.0/quantstats_lumi/utils.py
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       18 2024-05-28 06:25:45.000000 quantstats-lumi-0.3.0/quantstats_lumi/version.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-28 07:34:19.636370 quantstats-lumi-0.3.0/quantstats_lumi.egg-info/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)    10144 2024-05-28 07:34:19.000000 quantstats-lumi-0.3.0/quantstats_lumi.egg-info/PKG-INFO
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      623 2024-05-28 07:34:19.000000 quantstats-lumi-0.3.0/quantstats_lumi.egg-info/SOURCES.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)        1 2024-05-28 07:34:19.000000 quantstats-lumi-0.3.0/quantstats_lumi.egg-info/dependency_links.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       39 2024-05-28 07:34:19.000000 quantstats-lumi-0.3.0/quantstats_lumi.egg-info/entry_points.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      145 2024-05-28 07:34:19.000000 quantstats-lumi-0.3.0/quantstats_lumi.egg-info/requires.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       16 2024-05-28 07:34:19.000000 quantstats-lumi-0.3.0/quantstats_lumi.egg-info/top_level.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)      145 2024-03-31 03:00:03.000000 quantstats-lumi-0.3.0/requirements.txt
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)       67 2024-05-28 07:34:19.636994 quantstats-lumi-0.3.0/setup.cfg
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     2939 2024-03-19 10:30:17.000000 quantstats-lumi-0.3.0/setup.py
+drwxr-xr-x   0 robertgrzesik   (501) staff       (20)        0 2024-05-28 07:34:19.636210 quantstats-lumi-0.3.0/tests/
+-rw-r--r--   0 robertgrzesik   (501) staff       (20)     3366 2024-03-31 03:31:38.000000 quantstats-lumi-0.3.0/tests/test_reports.py
```

### Comparing `quantstats-lumi-0.2.0/LICENSE.txt` & `quantstats-lumi-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `quantstats-lumi-0.2.0/PKG-INFO` & `quantstats-lumi-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantstats-lumi
-Version: 0.2.0
+Version: 0.3.0
 Summary: Portfolio analytics for quants
 Home-page: https://github.com/Lumiwealth/quantstats_lumi
 Author: Robert Grzesik (Lumiwealth)
 Author-email: rob@lumiwealth.com
 License: Apache Software License
 Keywords: quant algotrading algorithmic-trading quantitative-trading
                 quantitative-analysis algo-trading visualization plotting
```

### Comparing `quantstats-lumi-0.2.0/README.rst` & `quantstats-lumi-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `quantstats-lumi-0.2.0/quantstats_lumi/__init__.py` & `quantstats-lumi-0.3.0/quantstats_lumi/__init__.py`

 * *Files identical despite different names*

### Comparing `quantstats-lumi-0.2.0/quantstats_lumi/_plotting/__init__.py` & `quantstats-lumi-0.3.0/quantstats_lumi/_plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `quantstats-lumi-0.2.0/quantstats_lumi/_plotting/core.py` & `quantstats-lumi-0.3.0/quantstats_lumi/_plotting/core.py`

 * *Files identical despite different names*

### Comparing `quantstats-lumi-0.2.0/quantstats_lumi/_plotting/wrappers.py` & `quantstats-lumi-0.3.0/quantstats_lumi/_plotting/wrappers.py`

 * *Files identical despite different names*

### Comparing `quantstats-lumi-0.2.0/quantstats_lumi/plots.py` & `quantstats-lumi-0.3.0/quantstats_lumi/plots.py`

 * *Files identical despite different names*

### Comparing `quantstats-lumi-0.2.0/quantstats_lumi/reports.py` & `quantstats-lumi-0.3.0/quantstats_lumi/reports.py`

 * *Files 3% similar despite different names*

```diff
@@ -184,14 +184,49 @@
         prepare_returns=False,
         benchmark_title=benchmark_title,
         strategy_title=strategy_title,
     )[2:]
 
     mtrx.index.name = "Metric"
     tpl = tpl.replace("{{metrics}}", _html_table(mtrx))
+
+    # Add all of the summary metrics
+    
+    # CAGR #
+    # Get the value of the "Strategy" column where the "Metric" column is "CAGR% (Annual Return)"
+    cagr = mtrx.loc["CAGR% (Annual Return)", strategy_title]
+    # Add the CAGR to the template
+    tpl = tpl.replace("{{cagr}}", cagr)
+
+    # Total Return #
+    # Get the value of the "Strategy" column where the "Metric" column is "Total Return"
+    total_return = mtrx.loc["Total Return", strategy_title]
+    # Add the total return to the template
+    tpl = tpl.replace("{{total_return}}", total_return)
+
+
+    # Max Drawdown #
+    # Get the value of the "Strategy" column where the "Mteric" column is "Max Drawdown"
+    max_drawdown = mtrx.loc["Max Drawdown", strategy_title]
+    # Add the max drawdown to the template
+    tpl = tpl.replace("{{max_drawdown}}", max_drawdown)
+    
+    # RoMaD #
+    # Get the value of the "Strategy" column where the "Mteric" column is "RoMaD"
+    romad = mtrx.loc["RoMaD", strategy_title]
+    # Add the RoMaD to the template
+    tpl = tpl.replace("{{romad}}", romad)
+
+    # Longest Drawdown Duration #
+    # Get the value of the "Strategy" column where the "Mteric" column is "Longest Drawdown Duration"
+    longest_dd_days = mtrx.loc["Longest DD Days", strategy_title]
+    # Add the longest drawdown duration to the template
+    tpl = tpl.replace("{{longest_dd_days}}", longest_dd_days)
+
+
     if isinstance(returns, _pd.DataFrame):
         num_cols = len(returns.columns)
         for i in reversed(range(num_cols + 1, num_cols + 3)):
             str_td = "<td></td>" * i
             tpl = tpl.replace(
                 f"<tr>{str_td}</tr>", '<tr><td colspan="{}"><hr></td></tr>'.format(i)
             )
@@ -911,24 +946,24 @@
     metrics["End Period"] = _pd.Series(s_end)
     metrics["Risk-Free Rate % "] = _pd.Series(s_rf) * 100
     metrics["Time in Market % "] = _stats.exposure(df, prepare_returns=False) * pct
 
     metrics["~"] = blank
 
     if compounded:
-        metrics["Total Return % "] = (_stats.comp(df) * pct).map("{:,.2f}".format)
+        metrics["Total Return"] = (_stats.comp(df) * pct).map("{:,.2f}%".format)
     else:
-        metrics["Total Return % "] = (df.sum() * pct).map("{:,.2f}".format)
+        metrics["Total Return"] = (df.sum() * pct).map("{:,.2f}%".format)
 
     metrics["CAGR% (Annual Return) "] = _stats.cagr(df, rf, compounded, win_year) * pct
 
     metrics["~~~~~~~~~~~~~~"] = blank
 
     metrics["Sharpe"] = _stats.sharpe(df, rf, win_year, True)
-    metrics["ROMaD"] = _stats.romad(df, win_year, True)
+    metrics["RoMaD"] = _stats.romad(df, win_year, True)
     
     if benchmark is not None:
         metrics["Corr to Benchmark "] = _stats.benchmark_correlation(df, benchmark, True)
     metrics["Prob. Sharpe Ratio %"] = (
         _stats.probabilistic_sharpe_ratio(df, rf, win_year, False) * pct
     )
     if mode.lower() == "full":
@@ -1023,44 +1058,22 @@
         )
         metrics["Expected Yearly %%"] = (
             _stats.expected_return(
                 df, compounded=compounded, aggregate="YE", prepare_returns=False
             )
             * pct
         )
-        metrics["Kelly Criterion %"] = (
-            _stats.kelly_criterion(df, prepare_returns=False) * pct
-        )
-        metrics["Risk of Ruin %"] = _stats.risk_of_ruin(df, prepare_returns=False)
 
         metrics["Daily Value-at-Risk %"] = -abs(
             _stats.var(df, prepare_returns=False) * pct
         )
         metrics["Expected Shortfall (cVaR) %"] = -abs(
             _stats.cvar(df, prepare_returns=False) * pct
         )
 
-    metrics["~~~~~~"] = blank
-
-    if mode.lower() == "full":
-        metrics["Max Consecutive Wins *int"] = _stats.consecutive_wins(df)
-        metrics["Max Consecutive Losses *int"] = _stats.consecutive_losses(df)
-
-    metrics["Gain/Pain Ratio"] = _stats.gain_to_pain_ratio(df, rf)
-    metrics["Gain/Pain (1M)"] = _stats.gain_to_pain_ratio(df, rf, "ME")
-    metrics["~~~~~~~"] = blank
-
-    metrics["Payoff Ratio"] = _stats.payoff_ratio(df, prepare_returns=False)
-    metrics["Profit Factor"] = _stats.profit_factor(df, prepare_returns=False)
-    metrics["Common Sense Ratio"] = _stats.common_sense_ratio(df, prepare_returns=False)
-    metrics["CPC Index"] = _stats.cpc_index(df, prepare_returns=False)
-    metrics["Tail Ratio"] = _stats.tail_ratio(df, prepare_returns=False)
-    metrics["Outlier Win Ratio"] = _stats.outlier_win_ratio(df, prepare_returns=False)
-    metrics["Outlier Loss Ratio"] = _stats.outlier_loss_ratio(df, prepare_returns=False)
-
     # returns
     metrics["~~"] = blank
     comp_func = _stats.comp if compounded else lambda x: _np.sum(x, axis=0)
 
     today = df.index[-1]  # _dt.today()
     metrics["MTD %"] = comp_func(df[df.index >= _dt(today.year, today.month, 1)]) * pct
```

### Comparing `quantstats-lumi-0.2.0/quantstats_lumi/stats.py` & `quantstats-lumi-0.3.0/quantstats_lumi/stats.py`

 * *Files identical despite different names*

### Comparing `quantstats-lumi-0.2.0/quantstats_lumi/utils.py` & `quantstats-lumi-0.3.0/quantstats_lumi/utils.py`

 * *Files identical despite different names*

### Comparing `quantstats-lumi-0.2.0/quantstats_lumi.egg-info/PKG-INFO` & `quantstats-lumi-0.3.0/quantstats_lumi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantstats-lumi
-Version: 0.2.0
+Version: 0.3.0
 Summary: Portfolio analytics for quants
 Home-page: https://github.com/Lumiwealth/quantstats_lumi
 Author: Robert Grzesik (Lumiwealth)
 Author-email: rob@lumiwealth.com
 License: Apache Software License
 Keywords: quant algotrading algorithmic-trading quantitative-trading
                 quantitative-analysis algo-trading visualization plotting
```

### Comparing `quantstats-lumi-0.2.0/quantstats_lumi.egg-info/SOURCES.txt` & `quantstats-lumi-0.3.0/quantstats_lumi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quantstats-lumi-0.2.0/setup.py` & `quantstats-lumi-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `quantstats-lumi-0.2.0/tests/test_reports.py` & `quantstats-lumi-0.3.0/tests/test_reports.py`

 * *Files identical despite different names*

