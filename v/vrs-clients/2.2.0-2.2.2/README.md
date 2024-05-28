# Comparing `tmp/vrs_clients-2.2.0-py3-none-any.whl.zip` & `tmp/vrs_clients-2.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5415 bytes, number of entries: 9
--rw-r--r--  2.0 unx      204 b- defN 23-Oct-24 09:58 vrs_clients/__init__.py
--rw-r--r--  2.0 unx     2615 b- defN 23-Oct-24 08:41 vrs_clients/models.py
--rw-r--r--  2.0 unx     1505 b- defN 23-Oct-23 13:15 vrs_clients/utils.py
--rw-r--r--  2.0 unx     5496 b- defN 23-Oct-24 08:41 vrs_clients/vrs_clients.py
--rw-rw-rw-  2.0 unx      575 b- defN 24-Mar-12 11:17 vrs_clients-2.2.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      871 b- defN 24-Mar-12 11:17 vrs_clients-2.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-12 11:17 vrs_clients-2.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-Mar-12 11:17 vrs_clients-2.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      725 b- defN 24-Mar-12 11:17 vrs_clients-2.2.0.dist-info/RECORD
-9 files, 12095 bytes uncompressed, 4163 bytes compressed:  65.6%
+Zip file size: 5416 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      204 b- defN 24-May-28 11:24 vrs_clients/__init__.py
+-rw-r--r--  2.0 unx     2615 b- defN 23-Oct-23 13:21 vrs_clients/models.py
+-rw-r--r--  2.0 unx     1505 b- defN 22-Jun-20 08:23 vrs_clients/utils.py
+-rw-r--r--  2.0 unx     5496 b- defN 23-Oct-23 13:21 vrs_clients/vrs_clients.py
+-rw-rw-rw-  2.0 unx      575 b- defN 24-May-28 11:29 vrs_clients-2.2.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      871 b- defN 24-May-28 11:29 vrs_clients-2.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 11:29 vrs_clients-2.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-28 11:29 vrs_clients-2.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      725 b- defN 24-May-28 11:29 vrs_clients-2.2.2.dist-info/RECORD
+9 files, 12095 bytes uncompressed, 4164 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: vrs_clients/utils.py
 Comment: 
 
 Filename: vrs_clients/vrs_clients.py
 Comment: 
 
-Filename: vrs_clients-2.2.0.dist-info/LICENSE.txt
+Filename: vrs_clients-2.2.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: vrs_clients-2.2.0.dist-info/METADATA
+Filename: vrs_clients-2.2.2.dist-info/METADATA
 Comment: 
 
-Filename: vrs_clients-2.2.0.dist-info/WHEEL
+Filename: vrs_clients-2.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: vrs_clients-2.2.0.dist-info/top_level.txt
+Filename: vrs_clients-2.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: vrs_clients-2.2.0.dist-info/RECORD
+Filename: vrs_clients-2.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vrs_clients/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.2.0"
+__version__ = "2.2.2"
 
 __all__ = ["PlotlyVisualizationResourceClient", "VisualizationResourceClient"]
 
 from .vrs_clients import (
     PlotlyVisualizationResourceClient,
     VisualizationResourceClient,
 )
```

## Comparing `vrs_clients-2.2.0.dist-info/LICENSE.txt` & `vrs_clients-2.2.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `vrs_clients-2.2.0.dist-info/METADATA` & `vrs_clients-2.2.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vrs_clients
-Version: 2.2.0
+Version: 2.2.2
 Summary: E360 Visualization Resource Clients for Python
 Author: IQVIA
 Author-email: e360pypi@iqvia.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

