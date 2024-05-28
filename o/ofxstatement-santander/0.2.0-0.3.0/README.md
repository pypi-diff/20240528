# Comparing `tmp/ofxstatement_santander-0.2.0-py3-none-any.whl.zip` & `tmp/ofxstatement_santander-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3747 bytes, number of entries: 7
--rw-r--r--  2.0 unx        0 b- defN 24-May-26 19:09 ofxstatement_santander/__init__.py
--rw-r--r--  2.0 unx     3007 b- defN 24-May-26 19:09 ofxstatement_santander/santander_uk_qif.py
--rw-r--r--  2.0 unx     2487 b- defN 24-May-26 19:18 ofxstatement_santander-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-26 19:18 ofxstatement_santander-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       95 b- defN 24-May-26 19:18 ofxstatement_santander-0.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 24-May-26 19:18 ofxstatement_santander-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      655 b- defN 24-May-26 19:18 ofxstatement_santander-0.2.0.dist-info/RECORD
-7 files, 6359 bytes uncompressed, 2555 bytes compressed:  59.8%
+Zip file size: 3761 bytes, number of entries: 7
+-rw-r--r--  2.0 unx        0 b- defN 24-May-28 09:13 ofxstatement_santander/__init__.py
+-rw-r--r--  2.0 unx     3028 b- defN 24-May-28 09:13 ofxstatement_santander/santander_uk_qif.py
+-rw-r--r--  2.0 unx     2487 b- defN 24-May-28 09:22 ofxstatement_santander-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 09:22 ofxstatement_santander-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       95 b- defN 24-May-28 09:22 ofxstatement_santander-0.3.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 24-May-28 09:22 ofxstatement_santander-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      655 b- defN 24-May-28 09:22 ofxstatement_santander-0.3.0.dist-info/RECORD
+7 files, 6380 bytes uncompressed, 2569 bytes compressed:  59.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: ofxstatement_santander/__init__.py
 Comment: 
 
 Filename: ofxstatement_santander/santander_uk_qif.py
 Comment: 
 
-Filename: ofxstatement_santander-0.2.0.dist-info/METADATA
+Filename: ofxstatement_santander-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: ofxstatement_santander-0.2.0.dist-info/WHEEL
+Filename: ofxstatement_santander-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: ofxstatement_santander-0.2.0.dist-info/entry_points.txt
+Filename: ofxstatement_santander-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: ofxstatement_santander-0.2.0.dist-info/top_level.txt
+Filename: ofxstatement_santander-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: ofxstatement_santander-0.2.0.dist-info/RECORD
+Filename: ofxstatement_santander-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ofxstatement_santander/santander_uk_qif.py

```diff
@@ -1,11 +1,12 @@
 import logging
 from decimal import Decimal
 from typing import Dict, Optional, Iterable, Tuple
 import html
+import re
 
 from ofxstatement.parser import StatementParser
 from ofxstatement.plugin import Plugin
 from ofxstatement.statement import StatementLine, generate_transaction_id, Currency
 
 from ofxstatement_qif.plugin import QIFParser
 
@@ -76,15 +77,15 @@
             path, separator, day_first, encoding, account_name, currency
         )
 
     @staticmethod
     def get_transaction_memo(memo: Optional[str]) -> Optional[str]:
         if not memo:
             return None
-        split_memo = memo.split(" , ")
+        split_memo = re.split(r" , \d(.*)", memo)
         if len(split_memo) < 2:
             return None
         return html.unescape(split_memo[0].strip())
 
     def split_records(self) -> Iterable[StatementLine]:
         statement = self.parser.parse()
         return statement.lines
```

## Comparing `ofxstatement_santander-0.2.0.dist-info/METADATA` & `ofxstatement_santander-0.3.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofxstatement-santander
-Version: 0.2.0
+Version: 0.3.0
 Summary: ofxstatement plugin to handle Santander transaction files
 Author-email: R Vadai <rvadai@segence.com>
 Project-URL: repository, https://github.com/robvadai/ofxstatement-santander
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

## Comparing `ofxstatement_santander-0.2.0.dist-info/RECORD` & `ofxstatement_santander-0.3.0.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 ofxstatement_santander/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ofxstatement_santander/santander_uk_qif.py,sha256=Wwr7fk0CPGsWKZJq8F2_TrosGaxYLetACFvOGqcAXI8,3007
-ofxstatement_santander-0.2.0.dist-info/METADATA,sha256=aKbGdZu6b5E-Gmriq4ng61bhXfX6qTu7vlF7Bf78a38,2487
-ofxstatement_santander-0.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ofxstatement_santander-0.2.0.dist-info/entry_points.txt,sha256=tgIWawfPCfLGzH_6kCmpPNasPKdpAcs9YF4UDnlay8g,95
-ofxstatement_santander-0.2.0.dist-info/top_level.txt,sha256=zCNNe-6EKjXWOmMgTO64BQN-fy-mRhz8bAQNsdQNiXA,23
-ofxstatement_santander-0.2.0.dist-info/RECORD,,
+ofxstatement_santander/santander_uk_qif.py,sha256=XEzYORD8wEih-352ZiZjQs3D9EmrrUCHST_dnOona8E,3028
+ofxstatement_santander-0.3.0.dist-info/METADATA,sha256=aSGiE3R6hHm962AfNs2fIeSOT_9gcSc-Yaym1e5uZyg,2487
+ofxstatement_santander-0.3.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ofxstatement_santander-0.3.0.dist-info/entry_points.txt,sha256=tgIWawfPCfLGzH_6kCmpPNasPKdpAcs9YF4UDnlay8g,95
+ofxstatement_santander-0.3.0.dist-info/top_level.txt,sha256=zCNNe-6EKjXWOmMgTO64BQN-fy-mRhz8bAQNsdQNiXA,23
+ofxstatement_santander-0.3.0.dist-info/RECORD,,
```

