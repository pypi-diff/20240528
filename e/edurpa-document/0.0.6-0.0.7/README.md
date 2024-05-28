# Comparing `tmp/edurpa_document-0.0.6-py3-none-any.whl.zip` & `tmp/edurpa_document-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6325 bytes, number of entries: 9
+Zip file size: 6343 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-28 07:01 EduRPA/__init__.py
--rw-rw-rw-  2.0 fat     5686 b- defN 24-May-27 16:00 EduRPA/Document/DocumentAutomation.py
+-rw-rw-rw-  2.0 fat     5684 b- defN 24-May-27 16:09 EduRPA/Document/DocumentAutomation.py
 -rw-rw-rw-  2.0 fat      617 b- defN 24-May-27 15:57 EduRPA/Document/__init__.py
 -rw-rw-rw-  2.0 fat     2624 b- defN 24-Apr-28 06:18 EduRPA/Document/transform.py
--rw-rw-rw-  2.0 fat     1088 b- defN 24-May-27 16:00 edurpa_document-0.0.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2019 b- defN 24-May-27 16:00 edurpa_document-0.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-27 16:00 edurpa_document-0.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 24-May-27 16:00 edurpa_document-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      759 b- defN 24-May-27 16:00 edurpa_document-0.0.6.dist-info/RECORD
-9 files, 12892 bytes uncompressed, 5001 bytes compressed:  61.2%
+-rw-rw-rw-  2.0 fat     1088 b- defN 24-May-27 16:10 edurpa_document-0.0.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2019 b- defN 24-May-27 16:10 edurpa_document-0.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-27 16:10 edurpa_document-0.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 24-May-27 16:10 edurpa_document-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      759 b- defN 24-May-27 16:10 edurpa_document-0.0.7.dist-info/RECORD
+9 files, 12890 bytes uncompressed, 5019 bytes compressed:  61.1%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: EduRPA/Document/__init__.py
 Comment: 
 
 Filename: EduRPA/Document/transform.py
 Comment: 
 
-Filename: edurpa_document-0.0.6.dist-info/LICENSE
+Filename: edurpa_document-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: edurpa_document-0.0.6.dist-info/METADATA
+Filename: edurpa_document-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: edurpa_document-0.0.6.dist-info/WHEEL
+Filename: edurpa_document-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: edurpa_document-0.0.6.dist-info/top_level.txt
+Filename: edurpa_document-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: edurpa_document-0.0.6.dist-info/RECORD
+Filename: edurpa_document-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## EduRPA/Document/DocumentAutomation.py

```diff
@@ -6,14 +6,15 @@
 import json
 from openpyxl import Workbook
 from datetime import datetime
 from .transform import perspective_transform, resize_image
 import string
 import unicodedata
 import editdistance
+import re
 class DocumentAutomation:
     def __init__(self, lang, performance, tolerate, **kwargs):
         if kwargs["dryrun"]:
             # If running dryrun, ignore initialization
             return
         
         self.tolerate = tolerate
@@ -86,16 +87,17 @@
         return self.extract(extracted_labeled_images)
     
     @not_keyword
     def evaluate_answer(self, answer, correct):
         pd = unicodedata.normalize("NFKD", answer).encode("ASCII", "ignore").decode("ASCII")
         gt = unicodedata.normalize("NFKD", correct).encode("ASCII", "ignore").decode("ASCII")
         
-        pd = pd.translate(str.maketrans("", "", string.punctuation))
-        gt = gt.translate(str.maketrans("", "", string.punctuation))
+        # Remove punctuation and special characters
+        pd = re.sub(r'[.]', '', pd)
+        gt = re.sub(r'[.]', '', gt)
         
         pd_cer, gt_cer = list(pd.lower()), list(gt.lower())
         dist = editdistance.eval(pd_cer, gt_cer)
         cer = dist / (max(len(pd_cer), len(gt_cer)))
         
         return cer < self.tolerate
```

## Comparing `edurpa_document-0.0.6.dist-info/LICENSE` & `edurpa_document-0.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `edurpa_document-0.0.6.dist-info/METADATA` & `edurpa_document-0.0.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edurpa-document
-Version: 0.0.6
+Version: 0.0.7
 Summary: education librabry for RPA
 Home-page: https://github.com/edu-rpa/edu-rpa-library
 Author: david
 Author-email: davidhuynh0222@gmail.com
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `edurpa_document-0.0.6.dist-info/RECORD` & `edurpa_document-0.0.7.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 EduRPA/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-EduRPA/Document/DocumentAutomation.py,sha256=-dNJ7zjrrLs9O-xlHKpdRXhHDfSKJwTau-pjGG3bPts,5686
+EduRPA/Document/DocumentAutomation.py,sha256=XFE11wATDQcNJKG1QQrZBQlPyGYoYayINLL1aAz18Ps,5684
 EduRPA/Document/__init__.py,sha256=VvSYj27I8fJRzrzaQS5c-jpOb_ZZFSBBa6u8vdG6yrM,617
 EduRPA/Document/transform.py,sha256=TRL-dYUvUJcGS9h_pph3fm_-02dQfzh0pGMoVN3T7wY,2624
-edurpa_document-0.0.6.dist-info/LICENSE,sha256=YgvlMcXsea3kZqp1y62n8AgkwZp6xXbWSYW17pT58Yg,1088
-edurpa_document-0.0.6.dist-info/METADATA,sha256=B_i0uiM8ZfSeXH4Xz4xhVzrASMb8uRcIdS_4E97u5Yk,2019
-edurpa_document-0.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-edurpa_document-0.0.6.dist-info/top_level.txt,sha256=Wl0EDd9il1J3fz62-gLcRCpFYSlEbU4KVE_SNWkcpaI,7
-edurpa_document-0.0.6.dist-info/RECORD,,
+edurpa_document-0.0.7.dist-info/LICENSE,sha256=YgvlMcXsea3kZqp1y62n8AgkwZp6xXbWSYW17pT58Yg,1088
+edurpa_document-0.0.7.dist-info/METADATA,sha256=Q3i5-XZlDFa9MsDG9uqyD8j9EZcN8lWjEuCKCKGDK18,2019
+edurpa_document-0.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+edurpa_document-0.0.7.dist-info/top_level.txt,sha256=Wl0EDd9il1J3fz62-gLcRCpFYSlEbU4KVE_SNWkcpaI,7
+edurpa_document-0.0.7.dist-info/RECORD,,
```

