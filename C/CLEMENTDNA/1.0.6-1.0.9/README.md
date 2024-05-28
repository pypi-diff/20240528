# Comparing `tmp/CLEMENTDNA-1.0.6-py3-none-any.whl.zip` & `tmp/CLEMENTDNA-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 170416 bytes, number of entries: 49
+Zip file size: 170417 bytes, number of entries: 49
 -rw-rw-rw-  2.0 unx    15254 b- defN 23-Dec-31 11:04 CLEMENT/Bunch.py
 -rw-rw-rw-  2.0 unx    65990 b- defN 24-Jan-09 10:38 CLEMENT/CLEMENT.py
 -rw-rw-rw-  2.0 unx    16428 b- defN 24-Jan-01 11:29 CLEMENT/EMhard.py
 -rw-rw-rw-  2.0 unx    19350 b- defN 23-Dec-31 11:04 CLEMENT/Estep.py
 -rw-rw-rw-  2.0 unx    21327 b- defN 24-Jan-01 11:39 CLEMENT/Mstep.py
 -rw-rw-rw-  2.0 unx        7 b- defN 23-Aug-02 04:00 CLEMENT/__init__.py
 -rw-rw-rw-  2.0 unx    20001 b- defN 24-Jan-01 12:12 CLEMENT/clementrec.py
@@ -39,13 +39,13 @@
 -rw-rw-rw-  2.0 unx     4323 b- defN 24-Jan-01 10:04 script/result.py
 -rw-rw-rw-  2.0 unx    20654 b- defN 24-Jan-01 10:05 script/scoring.py
 -rw-rw-rw-  2.0 unx    38247 b- defN 23-Dec-31 11:04 script/visualizationeachstep.py
 -rw-rw-rw-  2.0 unx    11446 b- defN 23-Dec-31 11:04 script/visualizationpair.py
 -rw-rw-rw-  2.0 unx     7602 b- defN 23-Dec-31 11:04 script/visualizationpairsoft.py
 -rw-rw-rw-  2.0 unx    21489 b- defN 23-Dec-31 11:04 script/visualizationsingle.py
 -rw-rw-rw-  2.0 unx    11051 b- defN 23-Dec-31 11:04 script/visualizationsinglesoft.py
--rw-rw-rw-  2.0 unx     5648 b- defN 24-Jan-09 10:56 CLEMENTDNA-1.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 24-Jan-09 10:56 CLEMENTDNA-1.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 unx       49 b- defN 24-Jan-09 10:56 CLEMENTDNA-1.0.6.dist-info/entry_points.txt
--rw-rw-rw-  2.0 unx        8 b- defN 24-Jan-09 10:56 CLEMENTDNA-1.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3855 b- defN 24-Jan-09 10:56 CLEMENTDNA-1.0.6.dist-info/RECORD
-49 files, 831302 bytes uncompressed, 164464 bytes compressed:  80.2%
+-rw-rw-rw-  2.0 unx     5648 b- defN 24-Jan-09 10:57 CLEMENTDNA-1.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 24-Jan-09 10:57 CLEMENTDNA-1.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       49 b- defN 24-Jan-09 10:57 CLEMENTDNA-1.0.9.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 unx        8 b- defN 24-Jan-09 10:57 CLEMENTDNA-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3855 b- defN 24-Jan-09 10:57 CLEMENTDNA-1.0.9.dist-info/RECORD
+49 files, 831302 bytes uncompressed, 164465 bytes compressed:  80.2%
```

## zipnote {}

```diff
@@ -126,23 +126,23 @@
 
 Filename: script/visualizationsingle.py
 Comment: 
 
 Filename: script/visualizationsinglesoft.py
 Comment: 
 
-Filename: CLEMENTDNA-1.0.6.dist-info/METADATA
+Filename: CLEMENTDNA-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: CLEMENTDNA-1.0.6.dist-info/WHEEL
+Filename: CLEMENTDNA-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: CLEMENTDNA-1.0.6.dist-info/entry_points.txt
+Filename: CLEMENTDNA-1.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: CLEMENTDNA-1.0.6.dist-info/top_level.txt
+Filename: CLEMENTDNA-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: CLEMENTDNA-1.0.6.dist-info/RECORD
+Filename: CLEMENTDNA-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `CLEMENTDNA-1.0.6.dist-info/METADATA` & `CLEMENTDNA-1.0.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CLEMENTDNA
-Version: 1.0.6
+Version: 1.0.9
 Summary: Genomic decomposition and reconstruction of non-tumor diploid subclones
 Home-page: https://github.com/Yonsei-TGIL/CLEMENT
 Download-URL: https://github.com/Yonsei-TGIL/CLEMENT.git
 Author: Young-soo Chung, M.D.
 Author-email: goldpm1@yuhs.ac
 License: GPL v3
 Keywords: CLEMENT,genomic decomposition
@@ -51,15 +51,15 @@
 
 2. pip3 install git+https://github.com/Yonsei-TGIL/CLEMENT.git    
 
 ### Install from PyPi
 3. pip3 install CLEMENTDNA   
 
 ## Version update
-1.0.6 (Jan 1st, 2024)
+1.0.9 (Jan 1st, 2024)
 
 ## Input format
 As now of 1.0.4, CLEMENT only supports standardized TSV input. Examples of input file is shown in _"example"_ directory.
 - 1st column: mutation ID (CHR_POS is recommended)
 - 2nd column: label (answer), if possible. If user don't know the label (answer), just set 0
 - 3rd column: **Depth1,Alt1,Depth2,Alt2....,Depth_n,Alt_n**    * should be comma-separated, and no space permitted
 - 4th column: **BQ1,BQ2....,BQ_n**    * should be comma-separated, and no space permitted. If absent, CLEMENT set default BQ as 20.
```

## Comparing `CLEMENTDNA-1.0.6.dist-info/RECORD` & `CLEMENTDNA-1.0.9.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -38,12 +38,12 @@
 script/result.py,sha256=POTIEbgvR-3LTY1TdNw_-lbd7hEdNF1FyHgVJyzuIgY,4323
 script/scoring.py,sha256=Vkw8gUpeukcz7VxpJuOplBYvxl6NHt0GnshNylGi9o8,20654
 script/visualizationeachstep.py,sha256=Pyo1UUjffmt0wC8Aycinpjol2WRcXQcLF3dzhWo7BGM,38247
 script/visualizationpair.py,sha256=o-FFneG4lMJocuNAxhdl9prmZWy_J2qU7pZwAjT1xZE,11446
 script/visualizationpairsoft.py,sha256=xvBxq-DMjIBRb9Dqci8lYjhbAWDoT9JGhG0qBG4BIGw,7602
 script/visualizationsingle.py,sha256=sL0z2Q5TNLyh9oZsfJEd2-IAHJQREsToGTLttOZCsxc,21489
 script/visualizationsinglesoft.py,sha256=ab2mPzmUbN1QCXgAoHNEChL85Crn32pUbQhhxTxFfos,11051
-CLEMENTDNA-1.0.6.dist-info/METADATA,sha256=dcWkigHv7eyxkoEZAaheUhPANxQeiZLoAICJD3_CC9Y,5648
-CLEMENTDNA-1.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-CLEMENTDNA-1.0.6.dist-info/entry_points.txt,sha256=h95iKQKpXgFnu6RZE08iIrlGkjBD2fNtJr7ej_Nc11Q,49
-CLEMENTDNA-1.0.6.dist-info/top_level.txt,sha256=ofcg5hrlPtWAbdAAduNn27261mZ3eWia2kUszSVW684,8
-CLEMENTDNA-1.0.6.dist-info/RECORD,,
+CLEMENTDNA-1.0.9.dist-info/METADATA,sha256=7S66omhHtNbOK4G8zzRjoQqXjMacdsHyjZP9hYtC-zE,5648
+CLEMENTDNA-1.0.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+CLEMENTDNA-1.0.9.dist-info/entry_points.txt,sha256=h95iKQKpXgFnu6RZE08iIrlGkjBD2fNtJr7ej_Nc11Q,49
+CLEMENTDNA-1.0.9.dist-info/top_level.txt,sha256=ofcg5hrlPtWAbdAAduNn27261mZ3eWia2kUszSVW684,8
+CLEMENTDNA-1.0.9.dist-info/RECORD,,
```

