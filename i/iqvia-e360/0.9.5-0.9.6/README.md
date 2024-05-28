# Comparing `tmp/iqvia_e360-0.9.5-py3-none-any.whl.zip` & `tmp/iqvia_e360-0.9.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 12413 bytes, number of entries: 10
--rw-r--r--  2.0 unx     1020 b- defN 23-Apr-24 17:19 iqvia_e360/__init__.py
--rw-r--r--  2.0 unx    16251 b- defN 23-Apr-21 12:25 iqvia_e360/e360_context.py
--rw-r--r--  2.0 unx       46 b- defN 23-Apr-21 12:25 iqvia_e360/exceptions.py
--rw-r--r--  2.0 unx     8212 b- defN 23-Apr-21 12:25 iqvia_e360/models.py
--rw-r--r--  2.0 unx     2134 b- defN 23-Apr-21 12:25 iqvia_e360/settings.py
--rw-rw-rw-  2.0 unx      575 b- defN 23-Apr-26 15:31 iqvia_e360-0.9.5.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    15456 b- defN 23-Apr-26 15:31 iqvia_e360-0.9.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-26 15:31 iqvia_e360-0.9.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-26 15:31 iqvia_e360-0.9.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      803 b- defN 23-Apr-26 15:31 iqvia_e360-0.9.5.dist-info/RECORD
-10 files, 44600 bytes uncompressed, 11047 bytes compressed:  75.2%
+Zip file size: 12408 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     1020 b- defN 24-May-28 11:58 iqvia_e360/__init__.py
+-rw-r--r--  2.0 unx    16251 b- defN 22-Dec-20 13:31 iqvia_e360/e360_context.py
+-rw-r--r--  2.0 unx       46 b- defN 22-Jul-26 10:49 iqvia_e360/exceptions.py
+-rw-r--r--  2.0 unx     8212 b- defN 22-Aug-17 15:14 iqvia_e360/models.py
+-rw-r--r--  2.0 unx     2134 b- defN 22-Jul-26 10:49 iqvia_e360/settings.py
+-rw-rw-rw-  2.0 unx      575 b- defN 24-May-28 13:21 iqvia_e360-0.9.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    15406 b- defN 24-May-28 13:21 iqvia_e360-0.9.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 13:21 iqvia_e360-0.9.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-May-28 13:21 iqvia_e360-0.9.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      803 b- defN 24-May-28 13:21 iqvia_e360-0.9.6.dist-info/RECORD
+10 files, 44550 bytes uncompressed, 11042 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: iqvia_e360/models.py
 Comment: 
 
 Filename: iqvia_e360/settings.py
 Comment: 
 
-Filename: iqvia_e360-0.9.5.dist-info/LICENSE.txt
+Filename: iqvia_e360-0.9.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: iqvia_e360-0.9.5.dist-info/METADATA
+Filename: iqvia_e360-0.9.6.dist-info/METADATA
 Comment: 
 
-Filename: iqvia_e360-0.9.5.dist-info/WHEEL
+Filename: iqvia_e360-0.9.6.dist-info/WHEEL
 Comment: 
 
-Filename: iqvia_e360-0.9.5.dist-info/top_level.txt
+Filename: iqvia_e360-0.9.6.dist-info/top_level.txt
 Comment: 
 
-Filename: iqvia_e360-0.9.5.dist-info/RECORD
+Filename: iqvia_e360-0.9.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## iqvia_e360/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.5"
+__version__ = "0.9.6"
 
 __all__ = [
     "E360Context",
     "Settings",
     "AnalyticDatasetModel",
     "AnalyticDatasetDefinitionModel",
     "Granularity",
```

## Comparing `iqvia_e360-0.9.5.dist-info/LICENSE.txt` & `iqvia_e360-0.9.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `iqvia_e360-0.9.5.dist-info/METADATA` & `iqvia_e360-0.9.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: iqvia-e360
-Version: 0.9.5
+Version: 0.9.6
 Summary: E360 Clients Wrapper for Python
 Author: IQVIA
 Author-email: e360pypi@iqvia.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: adt-clients (<3,>=2.0.0)
 Requires-Dist: analytic-workbench-clients
 Requires-Dist: clients-core (<3,>=2.1.3)
 Requires-Dist: e360-charting (<2,>=1.3.0)
 Requires-Dist: dashboard-clients (<4,>=3.0.1)
```

