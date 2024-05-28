# Comparing `tmp/webportal_utils-0.1.2-py3-none-any.whl.zip` & `tmp/webportal_utils-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 8710 bytes, number of entries: 13
+Zip file size: 8719 bytes, number of entries: 13
 -rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 wp_utils/__init__.py
 -rw-r--r--  2.0 unx     1411 b- defN 20-Feb-02 00:00 wp_utils/settings.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 wp_utils/application/__init__.py
 -rw-r--r--  2.0 unx     3237 b- defN 20-Feb-02 00:00 wp_utils/application/admin.py
 -rw-r--r--  2.0 unx      201 b- defN 20-Feb-02 00:00 wp_utils/application/version.py
 -rw-r--r--  2.0 unx      100 b- defN 20-Feb-02 00:00 wp_utils/logging/__init__.py
 -rw-r--r--  2.0 unx     1342 b- defN 20-Feb-02 00:00 wp_utils/logging/loggers.py
 -rw-r--r--  2.0 unx     3371 b- defN 20-Feb-02 00:00 wp_utils/logging/mixins.py
--rw-r--r--  2.0 unx     2137 b- defN 20-Feb-02 00:00 wp_utils/logging/solr.py
-?rw-r--r--  2.0 unx     4398 b- defN 20-Feb-02 00:00 webportal_utils-0.1.2.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 webportal_utils-0.1.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1074 b- defN 20-Feb-02 00:00 webportal_utils-0.1.2.dist-info/licenses/LICENCE
-?rw-r--r--  2.0 unx     1078 b- defN 20-Feb-02 00:00 webportal_utils-0.1.2.dist-info/RECORD
-13 files, 18458 bytes uncompressed, 6900 bytes compressed:  62.6%
+-rw-r--r--  2.0 unx     2153 b- defN 20-Feb-02 00:00 wp_utils/logging/solr.py
+?rw-r--r--  2.0 unx     4398 b- defN 20-Feb-02 00:00 webportal_utils-0.1.3.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 webportal_utils-0.1.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1074 b- defN 20-Feb-02 00:00 webportal_utils-0.1.3.dist-info/licenses/LICENCE
+?rw-r--r--  2.0 unx     1078 b- defN 20-Feb-02 00:00 webportal_utils-0.1.3.dist-info/RECORD
+13 files, 18474 bytes uncompressed, 6909 bytes compressed:  62.6%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: wp_utils/logging/mixins.py
 Comment: 
 
 Filename: wp_utils/logging/solr.py
 Comment: 
 
-Filename: webportal_utils-0.1.2.dist-info/METADATA
+Filename: webportal_utils-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: webportal_utils-0.1.2.dist-info/WHEEL
+Filename: webportal_utils-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: webportal_utils-0.1.2.dist-info/licenses/LICENCE
+Filename: webportal_utils-0.1.3.dist-info/licenses/LICENCE
 Comment: 
 
-Filename: webportal_utils-0.1.2.dist-info/RECORD
+Filename: webportal_utils-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wp_utils/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

## wp_utils/logging/solr.py

```diff
@@ -36,17 +36,17 @@
         log_record: Dict[str, Any] = dict()
         self.add_fields(log_record, record, message_dict)
 
         return log_record
 
 
 class SolrHandler(logging.StreamHandler):
-    def __init__(self):
+    def __init__(self, url: str = utils_settings.SOLR_LOGS_URL):
         super().__init__()
-        self.solr = pysolr.Solr(utils_settings.SOLR_LOGS_URL, always_commit=True)
+        self.solr = pysolr.Solr(url, always_commit=True)
         self.solr.ping()
 
     def emit(self, record: logging.LogRecord) -> None:
         json_record = self.format(record)
         try:
             self.solr.add([json_record])
         except pysolr.SolrError:
```

## Comparing `webportal_utils-0.1.2.dist-info/METADATA` & `webportal_utils-0.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: webportal-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: Пакет утилит для webportal.
 Author-email: Nikita Sysoev <nylinary@gmail.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

## Comparing `webportal_utils-0.1.2.dist-info/licenses/LICENCE` & `webportal_utils-0.1.3.dist-info/licenses/LICENCE`

 * *Files identical despite different names*

## Comparing `webportal_utils-0.1.2.dist-info/RECORD` & `webportal_utils-0.1.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-wp_utils/__init__.py,sha256=YvuYzWnKtqBb-IqG8HAu-nhIYAsgj9Vmc_b9o7vO-js,22
+wp_utils/__init__.py,sha256=XEqb2aiIn8fzGE68Mph4ck1FtQqsR_am0wRWvrYPffQ,22
 wp_utils/settings.py,sha256=WRR7p6n_OYEAbMzCa1S1E0stQZe3JuEsg_HiTxVrd7g,1411
 wp_utils/application/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 wp_utils/application/admin.py,sha256=TB4Z57XPtfQ0a05yicl0_wqUQwlrRWXyixNXscvd4g0,3237
 wp_utils/application/version.py,sha256=Fg1q5zwkjofECKxBHDpumf7F51tq7vDlvSqj2_eLKpY,201
 wp_utils/logging/__init__.py,sha256=-gsjoVvfeMoqWYKW45b4TP1Imrt-j4ORgYLUA4GWxco,100
 wp_utils/logging/loggers.py,sha256=z387tJRIf8Fs7G1762cctneeIPrzyJrljyirMBS9mZ0,1342
 wp_utils/logging/mixins.py,sha256=A9HAz9mxky08ccREXEz-z95xQnTuXdz9ieZIbCx-dpg,3371
-wp_utils/logging/solr.py,sha256=wjie20UZBq0bgppFfhr-GFSGEU2G8veT66CLgqNAY8w,2137
-webportal_utils-0.1.2.dist-info/METADATA,sha256=5yCMFQagQP_NUWAt0qzMLcBfkIO4pHXhm5iXFTrlQhw,4398
-webportal_utils-0.1.2.dist-info/WHEEL,sha256=TJPnKdtrSue7xZ_AVGkp9YXcvDrobsjBds1du3Nx6dc,87
-webportal_utils-0.1.2.dist-info/licenses/LICENCE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
-webportal_utils-0.1.2.dist-info/RECORD,,
+wp_utils/logging/solr.py,sha256=z_FdXCbUvChY1ylH4WfOOhsS0oJPa7chhV-Qv-0Gulo,2153
+webportal_utils-0.1.3.dist-info/METADATA,sha256=QWUKXLVrG7Bz1dlV9Vk_PEcyZ1Pt962B4rW-xhI0uQg,4398
+webportal_utils-0.1.3.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+webportal_utils-0.1.3.dist-info/licenses/LICENCE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
+webportal_utils-0.1.3.dist-info/RECORD,,
```

