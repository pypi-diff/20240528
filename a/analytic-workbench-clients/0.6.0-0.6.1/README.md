# Comparing `tmp/analytic_workbench_clients-0.6.0-py3-none-any.whl.zip` & `tmp/analytic_workbench_clients-0.6.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7390 bytes, number of entries: 11
--rw-r--r--  2.0 unx      428 b- defN 24-Mar-12 11:10 analytic_workbench_clients/__init__.py
--rw-r--r--  2.0 unx     1417 b- defN 24-Mar-12 11:10 analytic_workbench_clients/cache_store_client.py
--rw-r--r--  2.0 unx     5516 b- defN 24-Mar-12 11:10 analytic_workbench_clients/job_client.py
--rw-r--r--  2.0 unx     1302 b- defN 22-Oct-12 13:10 analytic_workbench_clients/methods_client.py
--rw-r--r--  2.0 unx     1968 b- defN 24-Mar-12 11:10 analytic_workbench_clients/models.py
--rw-r--r--  2.0 unx     1231 b- defN 22-Nov-22 18:56 analytic_workbench_clients/resource_client.py
--rw-rw-rw-  2.0 unx      575 b- defN 24-Mar-12 11:10 analytic_workbench_clients-0.6.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      892 b- defN 24-Mar-12 11:10 analytic_workbench_clients-0.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-12 11:10 analytic_workbench_clients-0.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       27 b- defN 24-Mar-12 11:10 analytic_workbench_clients-0.6.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1075 b- defN 24-Mar-12 11:10 analytic_workbench_clients-0.6.0.dist-info/RECORD
-11 files, 14523 bytes uncompressed, 5514 bytes compressed:  62.0%
+Zip file size: 7387 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      428 b- defN 24-May-24 11:15 analytic_workbench_clients/__init__.py
+-rw-r--r--  2.0 unx     1417 b- defN 24-Mar-11 11:09 analytic_workbench_clients/cache_store_client.py
+-rw-r--r--  2.0 unx     5516 b- defN 24-Mar-11 11:09 analytic_workbench_clients/job_client.py
+-rw-r--r--  2.0 unx     1302 b- defN 23-Oct-23 08:40 analytic_workbench_clients/methods_client.py
+-rw-r--r--  2.0 unx     1968 b- defN 24-Mar-11 11:09 analytic_workbench_clients/models.py
+-rw-r--r--  2.0 unx     1231 b- defN 23-Oct-23 08:40 analytic_workbench_clients/resource_client.py
+-rw-rw-rw-  2.0 unx      575 b- defN 24-May-24 15:31 analytic_workbench_clients-0.6.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      892 b- defN 24-May-24 15:31 analytic_workbench_clients-0.6.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 15:31 analytic_workbench_clients-0.6.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       27 b- defN 24-May-24 15:31 analytic_workbench_clients-0.6.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1075 b- defN 24-May-24 15:31 analytic_workbench_clients-0.6.1.dist-info/RECORD
+11 files, 14523 bytes uncompressed, 5511 bytes compressed:  62.1%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: analytic_workbench_clients/models.py
 Comment: 
 
 Filename: analytic_workbench_clients/resource_client.py
 Comment: 
 
-Filename: analytic_workbench_clients-0.6.0.dist-info/LICENSE.txt
+Filename: analytic_workbench_clients-0.6.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: analytic_workbench_clients-0.6.0.dist-info/METADATA
+Filename: analytic_workbench_clients-0.6.1.dist-info/METADATA
 Comment: 
 
-Filename: analytic_workbench_clients-0.6.0.dist-info/WHEEL
+Filename: analytic_workbench_clients-0.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: analytic_workbench_clients-0.6.0.dist-info/top_level.txt
+Filename: analytic_workbench_clients-0.6.1.dist-info/top_level.txt
 Comment: 
 
-Filename: analytic_workbench_clients-0.6.0.dist-info/RECORD
+Filename: analytic_workbench_clients-0.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## analytic_workbench_clients/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 
 __all__ = [
     "AWResourcesClient",
     "AWJobsClient",
     "AWCacheStoreClient",
     "MethodsClient",
     "JobModel",
```

## Comparing `analytic_workbench_clients-0.6.0.dist-info/LICENSE.txt` & `analytic_workbench_clients-0.6.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `analytic_workbench_clients-0.6.0.dist-info/METADATA` & `analytic_workbench_clients-0.6.1.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: analytic_workbench_clients
-Version: 0.6.0
+Version: 0.6.1
 Summary: E360 Analytic Workbench Clients for Python
 Author: IQVIA
 Author-email: e360pypi@iqvia.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `analytic_workbench_clients-0.6.0.dist-info/RECORD` & `analytic_workbench_clients-0.6.1.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-analytic_workbench_clients/__init__.py,sha256=mpZPr--mlRkaS_CShcskhsi5FEhndndLfgLGxIOZR0o,428
+analytic_workbench_clients/__init__.py,sha256=ENjl0JSeBxexkrsDBHt-E32_Ix60KqZgLllB0gQ71MY,428
 analytic_workbench_clients/cache_store_client.py,sha256=7Uv20xX2twL3FZWoHEUxbEwUFgnBe2ZC0xrXBub3b0Q,1417
 analytic_workbench_clients/job_client.py,sha256=Fp1zWu9U6qlScaLXvGc4ztSfLbv9SWR7oCFxaom7Pdk,5516
 analytic_workbench_clients/methods_client.py,sha256=tgI7M5KpS9JASQ2EL29hM2MSDnEIQWxGyQzIWLnen-s,1302
 analytic_workbench_clients/models.py,sha256=yW3sHnIb9m_73NpS9yYYYWOyIJGkMB3HUkv-j7yOqkg,1968
 analytic_workbench_clients/resource_client.py,sha256=5-zbWnGMnLdmLSGrMpgSXmQVXBTM-Mh3OLwcCfxI224,1231
-analytic_workbench_clients-0.6.0.dist-info/LICENSE.txt,sha256=uoI1G5lxk8h5Ua5OqmR7137DhTctSXGt9z7EBa1yclI,575
-analytic_workbench_clients-0.6.0.dist-info/METADATA,sha256=Erv_xnrF659lUKuipj233I6bMwLu2GflU7UithhZTiA,892
-analytic_workbench_clients-0.6.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-analytic_workbench_clients-0.6.0.dist-info/top_level.txt,sha256=RC7U-rQ4DxIls5nD1ZlqT_CmQG2AGqPkm5Syd4XQZM4,27
-analytic_workbench_clients-0.6.0.dist-info/RECORD,,
+analytic_workbench_clients-0.6.1.dist-info/LICENSE.txt,sha256=uoI1G5lxk8h5Ua5OqmR7137DhTctSXGt9z7EBa1yclI,575
+analytic_workbench_clients-0.6.1.dist-info/METADATA,sha256=7fdeQLltif7FJ6Hw_dx3io0RbCvo3LroK35qpp6UopQ,892
+analytic_workbench_clients-0.6.1.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+analytic_workbench_clients-0.6.1.dist-info/top_level.txt,sha256=RC7U-rQ4DxIls5nD1ZlqT_CmQG2AGqPkm5Syd4XQZM4,27
+analytic_workbench_clients-0.6.1.dist-info/RECORD,,
```

