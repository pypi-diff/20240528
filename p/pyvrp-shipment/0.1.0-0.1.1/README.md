# Comparing `tmp/pyvrp_shipment-0.1.0-py3-none-any.whl.zip` & `tmp/pyvrp_shipment-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,8 @@
-Zip file size: 6312 bytes, number of entries: 5
+Zip file size: 6484 bytes, number of entries: 6
 -rw-r--r--  2.0 unx     1845 b- defN 80-Jan-01 00:00 pyvrp_shipment/__init__.py
--rw-r--r--  2.0 unx    10758 b- defN 80-Jan-01 00:00 pyvrp_shipment-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1530 b- defN 80-Jan-01 00:00 pyvrp_shipment-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 pyvrp_shipment-0.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx      406 b- defN 16-Jan-01 00:00 pyvrp_shipment-0.1.0.dist-info/RECORD
-5 files, 14627 bytes uncompressed, 5558 bytes compressed:  62.0%
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 pyvrp_shipment/py.typed
+-rw-r--r--  2.0 unx    10758 b- defN 80-Jan-01 00:00 pyvrp_shipment-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1581 b- defN 80-Jan-01 00:00 pyvrp_shipment-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 pyvrp_shipment-0.1.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx      483 b- defN 16-Jan-01 00:00 pyvrp_shipment-0.1.1.dist-info/RECORD
+6 files, 14755 bytes uncompressed, 5608 bytes compressed:  62.0%
```

## zipnote {}

```diff
@@ -1,16 +1,19 @@
 Filename: pyvrp_shipment/__init__.py
 Comment: 
 
-Filename: pyvrp_shipment-0.1.0.dist-info/LICENSE
+Filename: pyvrp_shipment/py.typed
 Comment: 
 
-Filename: pyvrp_shipment-0.1.0.dist-info/METADATA
+Filename: pyvrp_shipment-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: pyvrp_shipment-0.1.0.dist-info/WHEEL
+Filename: pyvrp_shipment-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pyvrp_shipment-0.1.0.dist-info/RECORD
+Filename: pyvrp_shipment-0.1.1.dist-info/WHEEL
+Comment: 
+
+Filename: pyvrp_shipment-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pyvrp_shipment-0.1.0.dist-info/LICENSE` & `pyvrp_shipment-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyvrp_shipment-0.1.0.dist-info/METADATA` & `pyvrp_shipment-0.1.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: pyvrp-shipment
-Version: 0.1.0
+Version: 0.1.1
 Summary: `pyvrp-shipment` is a package for wrapper for solving shipment in PyVRP
 Home-page: https://github.com/SaitoTsutomu/pyvrp-shipment
 License: Apache-2.0
 Author: Saito Tsutomu
 Author-email: tsutomu7@hotmail.co.jp
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Dist: pyvrp (>=0.8.2,<0.9.0)
 Description-Content-Type: text/markdown
 
 # pyvrp-shipment
```

