# Comparing `tmp/nfinance-0.4.5-py3-none-any.whl.zip` & `tmp/nfinance-0.4.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 8457 bytes, number of entries: 12
+Zip file size: 8456 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      456 b- defN 24-May-28 04:32 nfinance/__init__.py
 -rw-r--r--  2.0 unx     2121 b- defN 24-May-28 04:32 nfinance/financials.py
 -rw-r--r--  2.0 unx      481 b- defN 24-May-28 04:32 nfinance/rsi.py
 -rw-r--r--  2.0 unx     3067 b- defN 24-May-28 04:33 nfinance/stock_data.py
 -rw-r--r--  2.0 unx     4027 b- defN 24-May-28 04:32 nfinance/stock_listing.py
 -rw-r--r--  2.0 unx       45 b- defN 24-May-28 04:32 tests/__init__.py
 -rw-r--r--  2.0 unx     1485 b- defN 24-May-28 04:32 tests/test_stock_data.py
--rw-r--r--  2.0 unx     1064 b- defN 24-May-28 04:34 nfinance-0.4.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     3646 b- defN 24-May-28 04:34 nfinance-0.4.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-28 04:34 nfinance-0.4.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 24-May-28 04:34 nfinance-0.4.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      931 b- defN 24-May-28 04:34 nfinance-0.4.5.dist-info/RECORD
-12 files, 17430 bytes uncompressed, 6905 bytes compressed:  60.4%
+-rw-r--r--  2.0 unx     1064 b- defN 24-May-28 04:49 nfinance-0.4.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3646 b- defN 24-May-28 04:49 nfinance-0.4.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 04:49 nfinance-0.4.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 24-May-28 04:49 nfinance-0.4.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      931 b- defN 24-May-28 04:49 nfinance-0.4.6.dist-info/RECORD
+12 files, 17430 bytes uncompressed, 6904 bytes compressed:  60.4%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_stock_data.py
 Comment: 
 
-Filename: nfinance-0.4.5.dist-info/LICENSE
+Filename: nfinance-0.4.6.dist-info/LICENSE
 Comment: 
 
-Filename: nfinance-0.4.5.dist-info/METADATA
+Filename: nfinance-0.4.6.dist-info/METADATA
 Comment: 
 
-Filename: nfinance-0.4.5.dist-info/WHEEL
+Filename: nfinance-0.4.6.dist-info/WHEEL
 Comment: 
 
-Filename: nfinance-0.4.5.dist-info/top_level.txt
+Filename: nfinance-0.4.6.dist-info/top_level.txt
 Comment: 
 
-Filename: nfinance-0.4.5.dist-info/RECORD
+Filename: nfinance-0.4.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `nfinance-0.4.5.dist-info/LICENSE` & `nfinance-0.4.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `nfinance-0.4.5.dist-info/METADATA` & `nfinance-0.4.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nfinance
-Version: 0.4.5
+Version: 0.4.6
 Summary: A simple finance data fetching library for Naver Finance data.
 Home-page: https://github.com/lega001/nfinance
 Author: lega001
 Author-email: lega01077970523@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `nfinance-0.4.5.dist-info/RECORD` & `nfinance-0.4.6.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 nfinance/__init__.py,sha256=JPqPpqat_GZctMZJdnP67pfQIug2STg0KVEO8njkOmI,456
 nfinance/financials.py,sha256=STKNdzWnLx2TntMgiYNERktVNiUs70ia1DxwOX02HzY,2121
 nfinance/rsi.py,sha256=aNaV5DNpCdEiZeY2-RnIwTOIf7wt1G8Kafz9aMr9JdY,481
 nfinance/stock_data.py,sha256=XBY-eRlqx5ZRStnQ-56xXQxR2bbo8lHBuIu2BxYr5nQ,3067
 nfinance/stock_listing.py,sha256=ME1q4tpLxfwqKZFVNSdpD_K8apYSunI9lRuozn5eVlk,4027
 tests/__init__.py,sha256=PG_aDJEGJwy2Ls4tNVDssNXIARlEqzKc4hB7FAEE31g,45
 tests/test_stock_data.py,sha256=nobDuOLwlap9sPzyyIFKb05um2mbVrYOAlzeRqjO-jE,1485
-nfinance-0.4.5.dist-info/LICENSE,sha256=W-G02SIVZT605TQhaNoPMh3yDfjDdwj91mWwo-3-mcU,1064
-nfinance-0.4.5.dist-info/METADATA,sha256=9MfEcG4XJs-1YlIj7xotV6v7feBOqYaoklVnGhC9Px4,3646
-nfinance-0.4.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nfinance-0.4.5.dist-info/top_level.txt,sha256=lFnY9sT0iM6MkEPAa3XqYKwA9dUFIA8R31RYsU1nyzg,15
-nfinance-0.4.5.dist-info/RECORD,,
+nfinance-0.4.6.dist-info/LICENSE,sha256=W-G02SIVZT605TQhaNoPMh3yDfjDdwj91mWwo-3-mcU,1064
+nfinance-0.4.6.dist-info/METADATA,sha256=Tn7Fw_wrl8OTgmMdIcT7HvjloPY4iu-nD423oZNZmq8,3646
+nfinance-0.4.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nfinance-0.4.6.dist-info/top_level.txt,sha256=lFnY9sT0iM6MkEPAa3XqYKwA9dUFIA8R31RYsU1nyzg,15
+nfinance-0.4.6.dist-info/RECORD,,
```

