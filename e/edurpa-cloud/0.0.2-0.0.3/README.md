# Comparing `tmp/edurpa_cloud-0.0.2-py3-none-any.whl.zip` & `tmp/edurpa_cloud-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 11171 bytes, number of entries: 14
+Zip file size: 11190 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-17 16:24 EduRPA/__init__.py
 -rw-rw-rw-  2.0 fat    13103 b- defN 24-Apr-18 09:37 EduRPA/Google/Classroom.py
 -rw-rw-rw-  2.0 fat     1511 b- defN 24-Apr-23 16:12 EduRPA/Google/CustomOAuth.py
 -rw-rw-rw-  2.0 fat    11964 b- defN 24-Apr-18 09:38 EduRPA/Google/Form.py
 -rw-rw-rw-  2.0 fat      314 b- defN 24-Apr-21 05:45 EduRPA/Google/Utils.py
 -rw-rw-rw-  2.0 fat      469 b- defN 24-Apr-21 13:23 EduRPA/Google/__init__.py
--rw-rw-rw-  2.0 fat     1577 b- defN 24-May-25 13:07 EduRPA/Storage/S3Storage.py
+-rw-rw-rw-  2.0 fat     1603 b- defN 24-May-28 12:25 EduRPA/Storage/S3Storage.py
 -rw-rw-rw-  2.0 fat     1575 b- defN 24-Apr-28 06:10 EduRPA/Storage/Storage.py
 -rw-rw-rw-  2.0 fat      312 b- defN 24-May-25 13:07 EduRPA/Storage/__init__.py
--rw-rw-rw-  2.0 fat     1088 b- defN 24-May-25 13:07 edurpa_cloud-0.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      716 b- defN 24-May-25 13:07 edurpa_cloud-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-25 13:07 edurpa_cloud-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 24-May-25 13:07 edurpa_cloud-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1136 b- defN 24-May-25 13:07 edurpa_cloud-0.0.2.dist-info/RECORD
-14 files, 33864 bytes uncompressed, 9281 bytes compressed:  72.6%
+-rw-rw-rw-  2.0 fat     1088 b- defN 24-May-28 12:25 edurpa_cloud-0.0.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      716 b- defN 24-May-28 12:25 edurpa_cloud-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-28 12:25 edurpa_cloud-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 24-May-28 12:25 edurpa_cloud-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1136 b- defN 24-May-28 12:25 edurpa_cloud-0.0.3.dist-info/RECORD
+14 files, 33890 bytes uncompressed, 9300 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: EduRPA/Storage/Storage.py
 Comment: 
 
 Filename: EduRPA/Storage/__init__.py
 Comment: 
 
-Filename: edurpa_cloud-0.0.2.dist-info/LICENSE
+Filename: edurpa_cloud-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: edurpa_cloud-0.0.2.dist-info/METADATA
+Filename: edurpa_cloud-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: edurpa_cloud-0.0.2.dist-info/WHEEL
+Filename: edurpa_cloud-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: edurpa_cloud-0.0.2.dist-info/top_level.txt
+Filename: edurpa_cloud-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: edurpa_cloud-0.0.2.dist-info/RECORD
+Filename: edurpa_cloud-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## EduRPA/Storage/S3Storage.py

```diff
@@ -1,16 +1,16 @@
 from robot.api.deco import keyword, not_keyword
 import os
 import requests
 
 class S3Storage:
     def __init__(self) -> None:
         self.user_id = os.getenv('USER_ID')
-        self.service_key = os.getenv('SERVICE_KEY')
-        self.base_url = os.getenv('BASE_URL')
+        self.service_key = os.getenv('FILE_STORAGE_SERVICE_KEY')
+        self.base_url = os.getenv('FILE_STORAGE_BASE_URL')
 
     @keyword("Upload File", types={'file': 'str', 'file_name': 'str', 'folder_path': 'str'})
     def upload_file(self, file, file_name, folder_path):
         # read the file
         with open(file, 'rb') as f:
             file_data = f.read()
```

## Comparing `edurpa_cloud-0.0.2.dist-info/LICENSE` & `edurpa_cloud-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `edurpa_cloud-0.0.2.dist-info/METADATA` & `edurpa_cloud-0.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edurpa-cloud
-Version: 0.0.2
+Version: 0.0.3
 Summary: Education Google RPA Librabry For Education
 Home-page: https://github.com/edu-rpa/edurpa-google
 Author: david
 Author-email: davidhuynh0222@gmail.com
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

