# Comparing `tmp/dashboard_clients-3.0.3-py3-none-any.whl.zip` & `tmp/dashboard_clients-3.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4802 bytes, number of entries: 8
--rw-r--r--  2.0 unx      645 b- defN 22-Nov-22 14:13 dashboard_clients/__init__.py
--rw-r--r--  2.0 unx     2315 b- defN 22-Aug-18 10:18 dashboard_clients/dashboard_service_client.py
--rw-r--r--  2.0 unx     6483 b- defN 22-Aug-17 14:49 dashboard_clients/models.py
--rw-rw-rw-  2.0 unx      575 b- defN 22-Nov-25 16:14 dashboard_clients-3.0.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      896 b- defN 22-Nov-25 16:14 dashboard_clients-3.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-25 16:14 dashboard_clients-3.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 22-Nov-25 16:14 dashboard_clients-3.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      709 b- defN 22-Nov-25 16:14 dashboard_clients-3.0.3.dist-info/RECORD
-8 files, 11733 bytes uncompressed, 3544 bytes compressed:  69.8%
+Zip file size: 4806 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      645 b- defN 24-May-24 11:54 dashboard_clients/__init__.py
+-rw-r--r--  2.0 unx     2315 b- defN 24-May-24 11:54 dashboard_clients/dashboard_service_client.py
+-rw-r--r--  2.0 unx     6483 b- defN 24-May-24 11:54 dashboard_clients/models.py
+-rw-rw-rw-  2.0 unx      575 b- defN 24-May-28 09:57 dashboard_clients-3.0.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      896 b- defN 24-May-28 09:57 dashboard_clients-3.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 09:57 dashboard_clients-3.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 24-May-28 09:57 dashboard_clients-3.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      709 b- defN 24-May-28 09:57 dashboard_clients-3.0.4.dist-info/RECORD
+8 files, 11733 bytes uncompressed, 3548 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: dashboard_clients/dashboard_service_client.py
 Comment: 
 
 Filename: dashboard_clients/models.py
 Comment: 
 
-Filename: dashboard_clients-3.0.3.dist-info/LICENSE.txt
+Filename: dashboard_clients-3.0.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dashboard_clients-3.0.3.dist-info/METADATA
+Filename: dashboard_clients-3.0.4.dist-info/METADATA
 Comment: 
 
-Filename: dashboard_clients-3.0.3.dist-info/WHEEL
+Filename: dashboard_clients-3.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: dashboard_clients-3.0.3.dist-info/top_level.txt
+Filename: dashboard_clients-3.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: dashboard_clients-3.0.3.dist-info/RECORD
+Filename: dashboard_clients-3.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dashboard_clients/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.0.3"
+__version__ = "3.0.4"
 
 __all__ = [
     "DashboardsClient",
     "TabbedDashboardModel",
     "TabModel",
     "TileModel",
     "TileConfigurationModel",
```

## Comparing `dashboard_clients-3.0.3.dist-info/LICENSE.txt` & `dashboard_clients-3.0.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `dashboard_clients-3.0.3.dist-info/METADATA` & `dashboard_clients-3.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashboard-clients
-Version: 3.0.3
+Version: 3.0.4
 Summary: E360 Dashboard Service Client for Python
 Author: IQVIA
 Author-email: e360pypi@iqvia.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `dashboard_clients-3.0.3.dist-info/RECORD` & `dashboard_clients-3.0.4.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-dashboard_clients/__init__.py,sha256=IbulO2ey93TJsoiwcqQtmmz_cjaTiS0AAX4iddnYgIo,645
+dashboard_clients/__init__.py,sha256=rfajQ4Zf5ObsjpL1XkPxWT7yqGJS8JQvx9poFZbhCr4,645
 dashboard_clients/dashboard_service_client.py,sha256=On-6bPg1ghlSJKTF_cQM8H4xo87Kfm0pFcUUxqJhq7w,2315
 dashboard_clients/models.py,sha256=qfxA0RSqNkSc8u_tUMio6vE-LNDcX40v0NDQBIcKTnU,6483
-dashboard_clients-3.0.3.dist-info/LICENSE.txt,sha256=I7qhxQ9AQQRmqxoonhxW1b4hE1pOxxnyWE9WbrX5E4A,575
-dashboard_clients-3.0.3.dist-info/METADATA,sha256=b2kD-UxO36gvgWS0aSs81LmR-EXCIfHQcQB7nFyne-M,896
-dashboard_clients-3.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-dashboard_clients-3.0.3.dist-info/top_level.txt,sha256=dSKrwg7QvvwnvqSSj5oolzj2PO-EJA2R2wJ9LTBRI40,18
-dashboard_clients-3.0.3.dist-info/RECORD,,
+dashboard_clients-3.0.4.dist-info/LICENSE.txt,sha256=I7qhxQ9AQQRmqxoonhxW1b4hE1pOxxnyWE9WbrX5E4A,575
+dashboard_clients-3.0.4.dist-info/METADATA,sha256=Umo_zWoSQy-0MQ3y3-wmFI8-2ts7Y9_uaOltAd3wGf4,896
+dashboard_clients-3.0.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+dashboard_clients-3.0.4.dist-info/top_level.txt,sha256=dSKrwg7QvvwnvqSSj5oolzj2PO-EJA2R2wJ9LTBRI40,18
+dashboard_clients-3.0.4.dist-info/RECORD,,
```

