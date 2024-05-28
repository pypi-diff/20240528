# Comparing `tmp/zut-0.9.2-py3-none-any.whl.zip` & `tmp/zut-0.9.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 48922 bytes, number of entries: 16
--rw-rw-rw-  2.0 fat    89190 b- defN 24-May-23 15:47 zut/__init__.py
--rw-rw-rw-  2.0 fat      427 b- defN 24-May-23 17:07 zut/_version.py
+Zip file size: 49074 bytes, number of entries: 16
+-rw-rw-rw-  2.0 fat    89219 b- defN 24-May-28 13:01 zut/__init__.py
+-rw-rw-rw-  2.0 fat      427 b- defN 24-May-28 14:49 zut/_version.py
 -rw-rw-rw-  2.0 fat    25956 b- defN 24-May-23 09:45 zut/excel.py
--rw-rw-rw-  2.0 fat    12923 b- defN 24-May-23 12:12 zut/files.py
+-rw-rw-rw-  2.0 fat    13593 b- defN 24-May-28 14:47 zut/files.py
 -rw-rw-rw-  2.0 fat     2984 b- defN 24-May-20 14:22 zut/db/__init__.py
 -rw-rw-rw-  2.0 fat    25278 b- defN 24-May-21 12:29 zut/db/base.py
 -rw-rw-rw-  2.0 fat     7700 b- defN 24-May-21 12:29 zut/db/mssql.py
 -rw-rw-rw-  2.0 fat     3265 b- defN 24-May-21 12:29 zut/db/mysql.py
 -rw-rw-rw-  2.0 fat     7151 b- defN 24-May-21 12:29 zut/db/pg.py
 -rw-rw-rw-  2.0 fat     3557 b- defN 24-May-21 12:29 zut/db/pg2.py
 -rw-rw-rw-  2.0 fat     1641 b- defN 24-Jan-24 18:06 zut/db/sql-utils/pg.sql
--rw-rw-rw-  2.0 fat     1103 b- defN 24-May-23 17:07 zut-0.9.2.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     3872 b- defN 24-May-23 17:07 zut-0.9.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-23 17:07 zut-0.9.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 24-May-23 17:07 zut-0.9.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1163 b- defN 24-May-23 17:07 zut-0.9.2.dist-info/RECORD
-16 files, 186306 bytes uncompressed, 47070 bytes compressed:  74.7%
+-rw-rw-rw-  2.0 fat     1103 b- defN 24-May-28 14:49 zut-0.9.3.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     3872 b- defN 24-May-28 14:49 zut-0.9.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-28 14:49 zut-0.9.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 24-May-28 14:49 zut-0.9.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1163 b- defN 24-May-28 14:49 zut-0.9.3.dist-info/RECORD
+16 files, 187005 bytes uncompressed, 47222 bytes compressed:  74.7%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: zut/db/pg2.py
 Comment: 
 
 Filename: zut/db/sql-utils/pg.sql
 Comment: 
 
-Filename: zut-0.9.2.dist-info/LICENSE.txt
+Filename: zut-0.9.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: zut-0.9.2.dist-info/METADATA
+Filename: zut-0.9.3.dist-info/METADATA
 Comment: 
 
-Filename: zut-0.9.2.dist-info/WHEEL
+Filename: zut-0.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: zut-0.9.2.dist-info/top_level.txt
+Filename: zut-0.9.3.dist-info/top_level.txt
 Comment: 
 
-Filename: zut-0.9.2.dist-info/RECORD
+Filename: zut-0.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zut/__init__.py

```diff
@@ -1261,15 +1261,16 @@
 
 #endregion
 
 
 #region Output
 
 def normalize_out(out: str|Path|IOBase|DbAdapter|Literal[False]|None, *, dir: str|Path|None = None, **params) -> str|IOBase|DbAdapter|None:
-    from zut.db import DbAdapter, get_db_adapter
+    from zut.db import DbAdapter, get_db_adapter    
+    from zut import files
 
     if out is None or out == 'stdout':
         return sys.stdout
     elif out == 'stderr':
         return sys.stderr
     elif out == 'stdin':
         return sys.stdin
@@ -1286,15 +1287,15 @@
             out = str(out)
         
         out = out.format(**params)
         if is_url:
             return get_db_adapter(out)
 
         if dir and not out.startswith(('./', '.\\')):
-            out = os.path.join(str(dir), out)
+            out = files.join(str(dir), out)
         return os.path.expanduser(out)
     elif isinstance(out, DbAdapter):
         return out
     else:
         raise TypeError(f"Invalid type for out: {type(out)}")
```

## zut/_version.py

```diff
@@ -8,9 +8,9 @@
     VERSION_TUPLE = object
 
 version: str
 __version__: str
 __version_tuple__: VERSION_TUPLE
 version_tuple: VERSION_TUPLE
 
-__version__ = version = '0.9.2'
-__version_tuple__ = version_tuple = (0, 9, 2)
+__version__ = version = '0.9.3'
+__version_tuple__ = version_tuple = (0, 9, 3)
```

## zut/files.py

```diff
@@ -68,15 +68,37 @@
 def basename(path: str):
     path, use_native = _standardize(path)
 
     if use_native:
         return os.path.basename(path)
 
     return ntpath.basename(path)
-    
+
+
+def join(*paths: str):
+    remaining_paths = []
+    method = 'os'
+    for path in paths:
+        path = os.path.expanduser(path)
+        if isinstance(path, str) and (path.startswith("//") or '://' in path):
+            remaining_paths = [path]
+            method = 'custom'
+        elif isinstance(path, str) and (path.startswith('\\\\')):
+            remaining_paths = [path]
+            method = 'nt'
+        else:
+            remaining_paths.append(path)
+
+    if method == 'os':
+        return os.path.join(*remaining_paths)
+    elif method == 'nt':
+        return ntpath.join(*remaining_paths)
+    else:
+        return '/'.join(remaining_paths)
+
 
 def splitext(path: str):
     path, use_native = _standardize(path)
 
     if use_native:
         return os.path.splitext(path)
```

## Comparing `zut-0.9.2.dist-info/LICENSE.txt` & `zut-0.9.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `zut-0.9.2.dist-info/METADATA` & `zut-0.9.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zut
-Version: 0.9.2
+Version: 0.9.3
 Summary: Reusable Python utilities.
 Author-email: Sébastien Hocquet <dev@ipamo.net>
 Project-URL: Homepage, https://github.com/ipamo/zut
 Project-URL: Bug Tracker, https://github.com/ipamo/zut/issues
 Keywords: reusable,util,utils,common,commons,base,flexout,csv,excel,tabulate,smb,samba,share,out_table,out_file,db,DbAdapter
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `zut-0.9.2.dist-info/RECORD` & `zut-0.9.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-zut/__init__.py,sha256=zdPqZrqtjPxlmDL0JUkx21Y-CI7qZk_ba4cDBNKEikk,89190
-zut/_version.py,sha256=kf5P3B7rwrwCFjPGDgU8SMAYD27mDNFGKu1xYp5aJx8,427
+zut/__init__.py,sha256=me-hc_-Ei2QnQCZ9CBRLmi3eglfDDEJFIAfS9E8zElk,89219
+zut/_version.py,sha256=nPnMrWQJZ02EkOD6cU_YMMtWJUaS6HQzz8wN3r45V7Y,427
 zut/excel.py,sha256=Tudw8Rzt-DrR8_n6rRpX4InJ2espLXwzFTz9cc5Ele4,25956
-zut/files.py,sha256=PhJNKPdaO6wI58ciHr1P_hwCavJ8pZhU-hK2a3k5rd4,12923
+zut/files.py,sha256=3KrKe3TSJi3hZT_JrzhujcAYS51Gl-Tup2Iw2Je3sYs,13593
 zut/db/__init__.py,sha256=q22yE2ezKoXt1nNK_Yrjnt9qyao2g2DrAQWoDIgOwjQ,2984
 zut/db/base.py,sha256=NMjuyBULQA1YQxg7e0Mm4SsM0PFQxllbp5Yfmf45oEU,25278
 zut/db/mssql.py,sha256=FuS-d25WFzps6OTCI6HbAMkhm__N65cn8F-7jbyieHs,7700
 zut/db/mysql.py,sha256=M6fqDPcDbYlK4XE5fUJ5mDvJT8dTdfHrmMhbVEGoR2g,3265
 zut/db/pg.py,sha256=9qpserJkVziTLvvpKIv-5e2F9YSmco0650p04Q1FlIA,7151
 zut/db/pg2.py,sha256=iNkaIsNyozF7sp5LdlbfmGS8iGVXrKKop66H_cH82BA,3557
 zut/db/sql-utils/pg.sql,sha256=_CfoOZeIXJROCZcEHzrtBdjDBzloMyrGAObUzR2BmMU,1641
-zut-0.9.2.dist-info/LICENSE.txt,sha256=YTk_lGVv3UxRgzQTkxwYdikccg_bow2NGaId-s45n-I,1103
-zut-0.9.2.dist-info/METADATA,sha256=-y_-MgbxKrEUQ_j6GTA8rYUmJGsbHRwnCmnA2acoRJc,3872
-zut-0.9.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-zut-0.9.2.dist-info/top_level.txt,sha256=0b5rfbMHLPzpcwBifEaAzzfyv1gZPGT7RXa2myDnXXs,4
-zut-0.9.2.dist-info/RECORD,,
+zut-0.9.3.dist-info/LICENSE.txt,sha256=YTk_lGVv3UxRgzQTkxwYdikccg_bow2NGaId-s45n-I,1103
+zut-0.9.3.dist-info/METADATA,sha256=ESz5Rh_4pBSDTRfxRk4r4OtLkOJ0VyB_SBWdbJKstS8,3872
+zut-0.9.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+zut-0.9.3.dist-info/top_level.txt,sha256=0b5rfbMHLPzpcwBifEaAzzfyv1gZPGT7RXa2myDnXXs,4
+zut-0.9.3.dist-info/RECORD,,
```

