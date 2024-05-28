# Comparing `tmp/chart_image_clients-1.1.2-py3-none-any.whl.zip` & `tmp/chart_image_clients-1.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3214 bytes, number of entries: 7
--rw-r--r--  2.0 unx      349 b- defN 22-Nov-23 10:45 chart_image_clients/__init__.py
--rw-r--r--  2.0 unx     1526 b- defN 22-Nov-23 10:45 chart_image_clients/plotly_client.py
--rw-rw-rw-  2.0 unx      575 b- defN 22-Nov-25 16:06 chart_image_clients-1.1.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      918 b- defN 22-Nov-25 16:06 chart_image_clients-1.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-25 16:06 chart_image_clients-1.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 22-Nov-25 16:06 chart_image_clients-1.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      628 b- defN 22-Nov-25 16:06 chart_image_clients-1.1.2.dist-info/RECORD
-7 files, 4108 bytes uncompressed, 2080 bytes compressed:  49.4%
+Zip file size: 3224 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      349 b- defN 24-May-24 12:06 chart_image_clients/__init__.py
+-rw-r--r--  2.0 unx     1526 b- defN 24-May-24 12:06 chart_image_clients/plotly_client.py
+-rw-rw-rw-  2.0 unx      575 b- defN 24-May-28 09:58 chart_image_clients-1.1.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      942 b- defN 24-May-28 09:58 chart_image_clients-1.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 09:58 chart_image_clients-1.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 24-May-28 09:58 chart_image_clients-1.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      628 b- defN 24-May-28 09:58 chart_image_clients-1.1.3.dist-info/RECORD
+7 files, 4132 bytes uncompressed, 2090 bytes compressed:  49.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: chart_image_clients/__init__.py
 Comment: 
 
 Filename: chart_image_clients/plotly_client.py
 Comment: 
 
-Filename: chart_image_clients-1.1.2.dist-info/LICENSE.txt
+Filename: chart_image_clients-1.1.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: chart_image_clients-1.1.2.dist-info/METADATA
+Filename: chart_image_clients-1.1.3.dist-info/METADATA
 Comment: 
 
-Filename: chart_image_clients-1.1.2.dist-info/WHEEL
+Filename: chart_image_clients-1.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: chart_image_clients-1.1.2.dist-info/top_level.txt
+Filename: chart_image_clients-1.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: chart_image_clients-1.1.2.dist-info/RECORD
+Filename: chart_image_clients-1.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## chart_image_clients/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.1.2"
+__version__ = "1.1.3"
 
 __all__ = ["ChartImageServicePlotlyClient"]
 
 try:
     # Attempts to import the client class
     # Allowed to fail importing so the package metadata can be read for building
     from .plotly_client import ChartImageServicePlotlyClient
```

## Comparing `chart_image_clients-1.1.2.dist-info/LICENSE.txt` & `chart_image_clients-1.1.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `chart_image_clients-1.1.2.dist-info/METADATA` & `chart_image_clients-1.1.3.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chart-image-clients
-Version: 1.1.2
+Version: 1.1.3
 Summary: E360 Chart Image Client for Python
 Author: IQVIA
 Author-email: e360pypi@iqvia.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -17,8 +17,9 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.6
 License-File: LICENSE.txt
 Requires-Dist: clients-core (<3,>=2.1.1)
+Requires-Dist: pydantic
```

## Comparing `chart_image_clients-1.1.2.dist-info/RECORD` & `chart_image_clients-1.1.3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-chart_image_clients/__init__.py,sha256=thOa1wFfBK3rfdOENcnabRAGpGoMd1rnLnDfGyu_PJg,349
+chart_image_clients/__init__.py,sha256=IMfug_bUPXLelStPGqgVUQ9hvT-5ijU46N6iCtRxDqI,349
 chart_image_clients/plotly_client.py,sha256=MeTgVI72P6kvuFl7DbbTKlRX_uX7wlZGF1GCFX4bTlw,1526
-chart_image_clients-1.1.2.dist-info/LICENSE.txt,sha256=S9X_6Wphp7hv_2oZKR6dUNq-bUvewqXeEBiDQ8CVJMY,575
-chart_image_clients-1.1.2.dist-info/METADATA,sha256=gt1fTpLTmNv9nc7VMgjvmf5vsniDSJfmD9hDKlcpyf8,918
-chart_image_clients-1.1.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-chart_image_clients-1.1.2.dist-info/top_level.txt,sha256=CgbWhXMBnn035bGvCcGg7c05g-zANFP3K4LMWRZQ58c,20
-chart_image_clients-1.1.2.dist-info/RECORD,,
+chart_image_clients-1.1.3.dist-info/LICENSE.txt,sha256=S9X_6Wphp7hv_2oZKR6dUNq-bUvewqXeEBiDQ8CVJMY,575
+chart_image_clients-1.1.3.dist-info/METADATA,sha256=YXdw-Dr9FzA8GQ4bolBIz2-0rfsOQh-V02v0UnKBYRY,942
+chart_image_clients-1.1.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+chart_image_clients-1.1.3.dist-info/top_level.txt,sha256=CgbWhXMBnn035bGvCcGg7c05g-zANFP3K4LMWRZQ58c,20
+chart_image_clients-1.1.3.dist-info/RECORD,,
```

