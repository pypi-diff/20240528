# Comparing `tmp/adrmdr-0.1.7-py3-none-any.whl.zip` & `tmp/adrmdr-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 192112 bytes, number of entries: 9
+Zip file size: 192127 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      834 b- defN 23-Oct-25 05:36 adrmdr/__init__.py
--rw-rw-rw-  2.0 fat   275563 b- defN 24-Apr-08 00:43 adrmdr/adrmdr.py
+-rw-rw-rw-  2.0 fat   275563 b- defN 24-May-28 01:04 adrmdr/adrmdr.py
 -rw-rw-rw-  2.0 fat   187510 b- defN 23-Nov-07 02:41 adrmdr/def.py
--rw-rw-rw-  2.0 fat     1074 b- defN 24-Apr-08 00:45 adrmdr-0.1.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      707 b- defN 24-Apr-08 00:45 adrmdr-0.1.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-08 00:45 adrmdr-0.1.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       39 b- defN 24-Apr-08 00:45 adrmdr-0.1.7.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        7 b- defN 24-Apr-08 00:45 adrmdr-0.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      694 b- defN 24-Apr-08 00:45 adrmdr-0.1.7.dist-info/RECORD
-9 files, 466520 bytes uncompressed, 190926 bytes compressed:  59.1%
+-rw-rw-rw-  2.0 fat     1074 b- defN 24-May-28 01:08 adrmdr-0.1.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      721 b- defN 24-May-28 01:08 adrmdr-0.1.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-28 01:08 adrmdr-0.1.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       39 b- defN 24-May-28 01:08 adrmdr-0.1.8.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        7 b- defN 24-May-28 01:08 adrmdr-0.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      694 b- defN 24-May-28 01:08 adrmdr-0.1.8.dist-info/RECORD
+9 files, 466534 bytes uncompressed, 190941 bytes compressed:  59.1%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: adrmdr/adrmdr.py
 Comment: 
 
 Filename: adrmdr/def.py
 Comment: 
 
-Filename: adrmdr-0.1.7.dist-info/LICENSE
+Filename: adrmdr-0.1.8.dist-info/LICENSE
 Comment: 
 
-Filename: adrmdr-0.1.7.dist-info/METADATA
+Filename: adrmdr-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: adrmdr-0.1.7.dist-info/WHEEL
+Filename: adrmdr-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: adrmdr-0.1.7.dist-info/entry_points.txt
+Filename: adrmdr-0.1.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: adrmdr-0.1.7.dist-info/top_level.txt
+Filename: adrmdr-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: adrmdr-0.1.7.dist-info/RECORD
+Filename: adrmdr-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## adrmdr/adrmdr.py

```diff
@@ -64,15 +64,15 @@
 
 
 global version_now
 global usergroup
 global setting_cfg
 global csdir
 global peizhidir
-version_now="0.1.7" 
+version_now="0.1.8" 
 usergroup="用户组=0"
 setting_cfg=""
 csdir =str (os .path .abspath (__file__ )).replace (str (__file__ ),"")
 if csdir=="":
     csdir =str (os .path .dirname (__file__ ))#
     csdir =csdir +csdir.split ("adrmdr")[0 ][-1 ]#
```

## Comparing `adrmdr-0.1.7.dist-info/LICENSE` & `adrmdr-0.1.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `adrmdr-0.1.7.dist-info/RECORD` & `adrmdr-0.1.8.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 adrmdr/__init__.py,sha256=WOQVHRGH7qnH1l6p-PLsGWBoJHpWy73c9uDsjm2baJs,834
-adrmdr/adrmdr.py,sha256=0YhN_XH64mGXgB2TOgjGOAWZu9JEzXFMnZNtNHr8iDo,275563
+adrmdr/adrmdr.py,sha256=YfRrsd4nauIjE5-EaVHzZgcsgUngZHjGIKTOJUwD6po,275563
 adrmdr/def.py,sha256=5-BLEpcel4Y0lrgluNgpuj_wvrmgj20GQdwZtv4ACXc,187510
-adrmdr-0.1.7.dist-info/LICENSE,sha256=nC_P4SgMa07filsYB3QtksztRZ6EIwTDALA1pdyg__c,1074
-adrmdr-0.1.7.dist-info/METADATA,sha256=c-sJzWK-vOaqWvxcdyU7ZpG1nG3K9WE9xYTKTuPq_Do,707
-adrmdr-0.1.7.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-adrmdr-0.1.7.dist-info/entry_points.txt,sha256=-5hzbwj_1Wzf99wpjyLuGUCDb7tEaO4Fi0PuwlRc3Yw,39
-adrmdr-0.1.7.dist-info/top_level.txt,sha256=LHrx2R0xwMuSXcbeVRkxYrpOnQCiVSdnYPa-3UmkVWE,7
-adrmdr-0.1.7.dist-info/RECORD,,
+adrmdr-0.1.8.dist-info/LICENSE,sha256=nC_P4SgMa07filsYB3QtksztRZ6EIwTDALA1pdyg__c,1074
+adrmdr-0.1.8.dist-info/METADATA,sha256=8pY6ZQHpArKpdiGDo2pTiYlgGVHtiEkQrnT6FlY5YDE,721
+adrmdr-0.1.8.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+adrmdr-0.1.8.dist-info/entry_points.txt,sha256=-5hzbwj_1Wzf99wpjyLuGUCDb7tEaO4Fi0PuwlRc3Yw,39
+adrmdr-0.1.8.dist-info/top_level.txt,sha256=LHrx2R0xwMuSXcbeVRkxYrpOnQCiVSdnYPa-3UmkVWE,7
+adrmdr-0.1.8.dist-info/RECORD,,
```

