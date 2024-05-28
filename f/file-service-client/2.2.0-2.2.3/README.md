# Comparing `tmp/file_service_client-2.2.0-py3-none-any.whl.zip` & `tmp/file_service_client-2.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6307 bytes, number of entries: 10
--rw-r--r--  2.0 unx      309 b- defN 23-Oct-24 09:55 file_service_client/__init__.py
+Zip file size: 6310 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      309 b- defN 24-May-28 09:06 file_service_client/__init__.py
 -rw-r--r--  2.0 unx     4578 b- defN 23-Oct-24 08:13 file_service_client/file_service_client.py
 -rw-r--r--  2.0 unx     3835 b- defN 23-Oct-23 16:24 file_service_client/file_store_client.py
 -rw-r--r--  2.0 unx     1866 b- defN 23-Oct-24 08:13 file_service_client/models.py
 -rw-r--r--  2.0 unx      282 b- defN 23-Oct-23 16:24 file_service_client/utils.py
--rw-rw-rw-  2.0 unx      575 b- defN 24-Mar-12 11:43 file_service_client-2.2.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      871 b- defN 24-Mar-12 11:43 file_service_client-2.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-12 11:43 file_service_client-2.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 24-Mar-12 11:43 file_service_client-2.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      901 b- defN 24-Mar-12 11:43 file_service_client-2.2.0.dist-info/RECORD
-10 files, 13329 bytes uncompressed, 4739 bytes compressed:  64.4%
+-rw-rw-rw-  2.0 unx      575 b- defN 24-May-28 09:59 file_service_client-2.2.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      871 b- defN 24-May-28 09:59 file_service_client-2.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 09:59 file_service_client-2.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 24-May-28 09:59 file_service_client-2.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      901 b- defN 24-May-28 09:59 file_service_client-2.2.3.dist-info/RECORD
+10 files, 13329 bytes uncompressed, 4742 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: file_service_client/models.py
 Comment: 
 
 Filename: file_service_client/utils.py
 Comment: 
 
-Filename: file_service_client-2.2.0.dist-info/LICENSE.txt
+Filename: file_service_client-2.2.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: file_service_client-2.2.0.dist-info/METADATA
+Filename: file_service_client-2.2.3.dist-info/METADATA
 Comment: 
 
-Filename: file_service_client-2.2.0.dist-info/WHEEL
+Filename: file_service_client-2.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: file_service_client-2.2.0.dist-info/top_level.txt
+Filename: file_service_client-2.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: file_service_client-2.2.0.dist-info/RECORD
+Filename: file_service_client-2.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## file_service_client/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.2.0"
+__version__ = "2.2.3"
 
 __all__ = [
     "FileServiceClient",
     "FileStoreServiceClient",
     "FileDefinitionModel",
     "FileResourceModel",
 ]
```

## Comparing `file_service_client-2.2.0.dist-info/LICENSE.txt` & `file_service_client-2.2.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `file_service_client-2.2.0.dist-info/METADATA` & `file_service_client-2.2.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file_service_client
-Version: 2.2.0
+Version: 2.2.3
 Summary: E360 File Service Client for Python
 Author: IQVIA
 Author-email: e360pypi@iqvia.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `file_service_client-2.2.0.dist-info/RECORD` & `file_service_client-2.2.3.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-file_service_client/__init__.py,sha256=M8H2ChuHUmzt73WLdJJBa39mStOa-eTj12hlAG-kS8c,309
+file_service_client/__init__.py,sha256=S6veAmLfJ30l35euR719RldnNtGAQy3892NdT-XTaEA,309
 file_service_client/file_service_client.py,sha256=ak4URF6WKWv1Sai40TJ0HZ-0IfODn2l1n4gRuSZoYrk,4578
 file_service_client/file_store_client.py,sha256=LhZb5b2UPmFQNtdBwyR5Xav90lLJkhYRSR0majDO41g,3835
 file_service_client/models.py,sha256=yGKDl1-zSEo4LLv83VYWbBa2MYBHt1MS5jAWWpkPgzA,1866
 file_service_client/utils.py,sha256=pRuUdsDBnCM17FcsmYPcYIdCZecN4oNKynMCZ8EFxhw,282
-file_service_client-2.2.0.dist-info/LICENSE.txt,sha256=uoI1G5lxk8h5Ua5OqmR7137DhTctSXGt9z7EBa1yclI,575
-file_service_client-2.2.0.dist-info/METADATA,sha256=lRMXv_FM7EnrK7t34Mb7J7d0kbTvPiGaxsz7YLHhq4g,871
-file_service_client-2.2.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-file_service_client-2.2.0.dist-info/top_level.txt,sha256=xMJ4t2DkLBBGaFgJY_D3FcIm-rdbO50rrU7-LyPnXNI,20
-file_service_client-2.2.0.dist-info/RECORD,,
+file_service_client-2.2.3.dist-info/LICENSE.txt,sha256=uoI1G5lxk8h5Ua5OqmR7137DhTctSXGt9z7EBa1yclI,575
+file_service_client-2.2.3.dist-info/METADATA,sha256=4EzYEzH_WftaiF8bSpsFGLrWECSBlqeOaTENlQgG4aA,871
+file_service_client-2.2.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+file_service_client-2.2.3.dist-info/top_level.txt,sha256=xMJ4t2DkLBBGaFgJY_D3FcIm-rdbO50rrU7-LyPnXNI,20
+file_service_client-2.2.3.dist-info/RECORD,,
```

