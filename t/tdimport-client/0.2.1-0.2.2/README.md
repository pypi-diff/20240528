# Comparing `tmp/tdimport_client-0.2.1-py3-none-any.whl.zip` & `tmp/tdimport_client-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4614 bytes, number of entries: 9
--rw-r--r--  2.0 unx      589 b- defN 22-Nov-23 10:47 tdimport_client/__init__.py
+Zip file size: 4613 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      589 b- defN 24-May-28 12:12 tdimport_client/__init__.py
 -rw-r--r--  2.0 unx     2079 b- defN 22-Nov-23 10:47 tdimport_client/models.py
 -rw-r--r--  2.0 unx     1051 b- defN 22-Nov-23 10:47 tdimport_client/sftp_client.py
 -rw-r--r--  2.0 unx      900 b- defN 22-Nov-23 10:47 tdimport_client/tdimport_client.py
--rw-rw-rw-  2.0 unx      575 b- defN 22-Nov-25 16:32 tdimport_client-0.2.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      915 b- defN 22-Nov-25 16:32 tdimport_client-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-25 16:32 tdimport_client-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 22-Nov-25 16:32 tdimport_client-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      770 b- defN 22-Nov-25 16:32 tdimport_client-0.2.1.dist-info/RECORD
-9 files, 6987 bytes uncompressed, 3270 bytes compressed:  53.2%
+-rw-rw-rw-  2.0 unx      575 b- defN 24-May-28 12:21 tdimport_client-0.2.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      893 b- defN 24-May-28 12:21 tdimport_client-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 12:21 tdimport_client-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 24-May-28 12:21 tdimport_client-0.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      770 b- defN 24-May-28 12:21 tdimport_client-0.2.2.dist-info/RECORD
+9 files, 6965 bytes uncompressed, 3269 bytes compressed:  53.1%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: tdimport_client/sftp_client.py
 Comment: 
 
 Filename: tdimport_client/tdimport_client.py
 Comment: 
 
-Filename: tdimport_client-0.2.1.dist-info/LICENSE.txt
+Filename: tdimport_client-0.2.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: tdimport_client-0.2.1.dist-info/METADATA
+Filename: tdimport_client-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: tdimport_client-0.2.1.dist-info/WHEEL
+Filename: tdimport_client-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: tdimport_client-0.2.1.dist-info/top_level.txt
+Filename: tdimport_client-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: tdimport_client-0.2.1.dist-info/RECORD
+Filename: tdimport_client-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tdimport_client/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 __all__ = [
     "TDImportServiceClient",
     "TDBundleUploadSFTPClient",
     "TDBundleImportModel",
     "TDBundleUploadModel",
 ]
```

## Comparing `tdimport_client-0.2.1.dist-info/LICENSE.txt` & `tdimport_client-0.2.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `tdimport_client-0.2.1.dist-info/METADATA` & `tdimport_client-0.2.2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdimport-client
-Version: 0.2.1
+Version: 0.2.2
 Summary: E360 TDImport Service Client for Python
 Author: IQVIA
 Author-email: e360pypi@iqvia.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -17,9 +17,8 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.7
 License-File: LICENSE.txt
 Requires-Dist: clients-core (<3,>=2.1.1)
 Requires-Dist: pydantic
-Requires-Dist: pysftp
```

