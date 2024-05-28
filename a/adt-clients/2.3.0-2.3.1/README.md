# Comparing `tmp/adt_clients-2.3.0-py3-none-any.whl.zip` & `tmp/adt_clients-2.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 12038 bytes, number of entries: 9
--rw-r--r--  2.0 unx      791 b- defN 23-Jun-13 09:57 adt_clients/__init__.py
+Zip file size: 12036 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      791 b- defN 24-May-24 11:49 adt_clients/__init__.py
 -rw-r--r--  2.0 unx    11293 b- defN 23-Apr-05 09:59 adt_clients/analytic_dataset_client.py
 -rw-r--r--  2.0 unx     3649 b- defN 23-Jun-13 09:57 adt_clients/analytic_dataset_definition_client.py
--rw-r--r--  2.0 unx    28111 b- defN 23-Apr-05 11:30 adt_clients/models.py
--rw-rw-rw-  2.0 unx      575 b- defN 23-Jun-13 11:32 adt_clients-2.3.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      845 b- defN 23-Jun-13 11:32 adt_clients-2.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 11:32 adt_clients-2.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-13 11:32 adt_clients-2.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      768 b- defN 23-Jun-13 11:32 adt_clients-2.3.0.dist-info/RECORD
-9 files, 46136 bytes uncompressed, 10704 bytes compressed:  76.8%
+-rw-r--r--  2.0 unx    28115 b- defN 24-May-24 11:59 adt_clients/models.py
+-rw-rw-rw-  2.0 unx      575 b- defN 24-May-28 09:55 adt_clients-2.3.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      845 b- defN 24-May-28 09:55 adt_clients-2.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 09:55 adt_clients-2.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-28 09:55 adt_clients-2.3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      768 b- defN 24-May-28 09:55 adt_clients-2.3.1.dist-info/RECORD
+9 files, 46140 bytes uncompressed, 10702 bytes compressed:  76.8%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: adt_clients/analytic_dataset_definition_client.py
 Comment: 
 
 Filename: adt_clients/models.py
 Comment: 
 
-Filename: adt_clients-2.3.0.dist-info/LICENSE.txt
+Filename: adt_clients-2.3.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: adt_clients-2.3.0.dist-info/METADATA
+Filename: adt_clients-2.3.1.dist-info/METADATA
 Comment: 
 
-Filename: adt_clients-2.3.0.dist-info/WHEEL
+Filename: adt_clients-2.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: adt_clients-2.3.0.dist-info/top_level.txt
+Filename: adt_clients-2.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: adt_clients-2.3.0.dist-info/RECORD
+Filename: adt_clients-2.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## adt_clients/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.3.0"
+__version__ = "2.3.1"
 
 __all__ = [
     "AnalyticDatasetClient",
     "AnalyticDatasetModel",
     "AnalyticDatasetDefinitionClient",
     "AnalyticDatasetDefinitionModel",
     "AnalyticDatasetMergeRequestModel",
```

## adt_clients/models.py

```diff
@@ -388,17 +388,17 @@
     groups: Optional[List[DemographicCharacteristicGroupModel]] = None
     doesSupportGroupDescription: Optional[bool] = None
     useGroupDescription: Optional[bool] = None
     doesSupportGroupOrdinal: Optional[bool] = None
     useGroupOrdinal: Optional[bool] = None
     costOfCareDays: Optional[int] = None
     exportAsEvent: Optional[bool] = None
-    granularitiesSupported: Optional[
-        List[Any]
-    ] = None  # 'Granularity' replaced to Any due to int/str usage by the service
+    granularitiesSupported: Optional[List[Any]] = (
+        None  # 'Granularity' replaced to Any due to int/str usage by the service
+    )
     id: Optional[int] = None
     created: Optional[datetime] = None
     updated: Optional[datetime] = None
 
 
 class CountType(str, Enum):
     PATIENT = "patient"
@@ -538,17 +538,17 @@
     relativeToIndexDatePrePeriodType: Optional[int] = None
     relativeToIndexDatePostPeriod: Optional[int] = None
     relativeToIndexDatePostPeriodType: Optional[int] = None
     visitType: Optional[VisitType] = None
     eventOccurrence: Optional[bool] = None
     eventCount: Optional[bool] = None
     descriptionInColumnName: Optional[bool] = None
-    topNExecution: Optional[
-        HighDimensionalCharacteristicTopNExecutionResponseModel
-    ] = None
+    topNExecution: Optional[HighDimensionalCharacteristicTopNExecutionResponseModel] = (
+        None
+    )
     columns: Optional[List[HighDimensionalCharacteristicColumnsResponseModel]] = None
 
 
 class AnalyticDatasetMergeResponseModel(BaseADTModel):
     id: Optional[UUID] = None
     analyticDatasetId: Optional[UUID] = None
     analyticDatasetAssetId: Optional[UUID] = None
```

## Comparing `adt_clients-2.3.0.dist-info/LICENSE.txt` & `adt_clients-2.3.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `adt_clients-2.3.0.dist-info/METADATA` & `adt_clients-2.3.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adt-clients
-Version: 2.3.0
+Version: 2.3.1
 Summary: E360 Analytic Dataset Tools Client for Python
 Author: IQVIA
 Author-email: e360pypi@iqvia.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

