# Comparing `tmp/athlib-0.7.8-py2.py3-none-any.whl.zip` & `tmp/athlib-0.7.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 75330 bytes, number of entries: 25
--rw-r--r--  2.0 unx     3307 b- defN 23-Aug-22 20:11 athlib/__init__.py
+Zip file size: 136187 bytes, number of entries: 26
+-rw-r--r--  2.0 unx     3361 b- defN 24-Jan-25 02:59 athlib/__init__.py
 -rw-r--r--  2.0 unx     9593 b- defN 23-Aug-22 20:06 athlib/athlon_score.py
+-rw-r--r--  2.0 unx   438962 b- defN 24-Jan-25 02:56 athlib/bulgarian_score.py
 -rw-r--r--  2.0 unx     6884 b- defN 22-Dec-20 11:05 athlib/codes.py
 -rw-r--r--  2.0 unx      278 b- defN 22-Dec-20 11:05 athlib/exceptions.py
 -rw-r--r--  2.0 unx    19215 b- defN 22-Dec-20 11:05 athlib/highjump.py
 -rw-r--r--  2.0 unx     7401 b- defN 22-Dec-20 11:05 athlib/hungarian_score.py
 -rw-r--r--  2.0 unx     6716 b- defN 22-Dec-20 11:05 athlib/implements.py
 -rw-r--r--  2.0 unx     4396 b- defN 22-Dec-20 11:05 athlib/jsondict.py
 -rw-r--r--  2.0 unx     2803 b- defN 22-Dec-20 11:05 athlib/qkids_score.py
@@ -15,13 +16,13 @@
 -rw-r--r--  2.0 unx    11532 b- defN 22-Dec-20 11:05 athlib/uka/agegroups.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Dec-20 11:05 athlib/wma/__init__.py
 -rw-r--r--  2.0 unx     9996 b- defN 23-Mar-14 10:17 athlib/wma/agegrader.py
 -rw-r--r--  2.0 unx     4575 b- defN 23-Mar-13 22:27 athlib/wma/wma-athlons-data.json
 -rw-r--r--  2.0 unx    92650 b- defN 23-Mar-13 22:27 athlib/wma/wma-data.json
 -rw-r--r--  2.0 unx      137 b- defN 22-Dec-22 21:24 athlib/wma/__pycache__/__init__.cpython-39.pyc
 -rw-r--r--  2.0 unx     9116 b- defN 23-Mar-14 10:17 athlib/wma/__pycache__/agegrader.cpython-39.pyc
--rw-r--r--  2.0 unx    11357 b- defN 23-Aug-22 20:12 athlib-0.7.8.dist-info/LICENSE
--rw-r--r--  2.0 unx      821 b- defN 23-Aug-22 20:12 athlib-0.7.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Aug-22 20:12 athlib-0.7.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Aug-22 20:12 athlib-0.7.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1999 b- defN 23-Aug-22 20:12 athlib-0.7.8.dist-info/RECORD
-25 files, 253470 bytes uncompressed, 72140 bytes compressed:  71.5%
+-rw-r--r--  2.0 unx    11357 b- defN 24-Jan-25 03:00 athlib-0.7.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      821 b- defN 24-Jan-25 03:00 athlib-0.7.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Jan-25 03:00 athlib-0.7.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Jan-25 03:00 athlib-0.7.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2083 b- defN 24-Jan-25 03:00 athlib-0.7.9.dist-info/RECORD
+26 files, 692570 bytes uncompressed, 132871 bytes compressed:  80.8%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: athlib/__init__.py
 Comment: 
 
 Filename: athlib/athlon_score.py
 Comment: 
 
+Filename: athlib/bulgarian_score.py
+Comment: 
+
 Filename: athlib/codes.py
 Comment: 
 
 Filename: athlib/exceptions.py
 Comment: 
 
 Filename: athlib/highjump.py
@@ -54,23 +57,23 @@
 
 Filename: athlib/wma/__pycache__/__init__.cpython-39.pyc
 Comment: 
 
 Filename: athlib/wma/__pycache__/agegrader.cpython-39.pyc
 Comment: 
 
-Filename: athlib-0.7.8.dist-info/LICENSE
+Filename: athlib-0.7.9.dist-info/LICENSE
 Comment: 
 
-Filename: athlib-0.7.8.dist-info/METADATA
+Filename: athlib-0.7.9.dist-info/METADATA
 Comment: 
 
-Filename: athlib-0.7.8.dist-info/WHEEL
+Filename: athlib-0.7.9.dist-info/WHEEL
 Comment: 
 
-Filename: athlib-0.7.8.dist-info/top_level.txt
+Filename: athlib-0.7.9.dist-info/top_level.txt
 Comment: 
 
-Filename: athlib-0.7.8.dist-info/RECORD
+Filename: athlib-0.7.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## athlib/__init__.py

```diff
@@ -1,16 +1,17 @@
 def __wma_delay__():
     from .wma.agegrader import AgeGrader, AthlonsAgeGrader
     return AgeGrader, AthlonsAgeGrader
 from .uka.agegroups import calc_uka_age_group
 from .athlon_score import score as athlon_score
 from .hungarian_score import score as hungarian_score
+from .bulgarian_score import score as bulgarian_score
 from .athlon_score import performance as athlon_performance_needed
 
-__version__ = u'0.7.8'
+__version__ = u'0.7.9'
 
 from .exceptions import RuleViolation
 
 from .utils import (
     normalize_gender,
     str2num,
     parse_hms,
```

## Comparing `athlib-0.7.8.dist-info/LICENSE` & `athlib-0.7.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `athlib-0.7.8.dist-info/METADATA` & `athlib-0.7.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athlib
-Version: 0.7.8
+Version: 0.7.9
 Summary: Utilities for track and field athletics
 Home-page: https://github.com/openath/athlib
 Author: Andy Robinson and others
 Author-email: andy@reportlab.com
 License: Apache
 Keywords: athletics track field
 Platform: UNKNOWN
```

## Comparing `athlib-0.7.8.dist-info/RECORD` & `athlib-0.7.9.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-athlib/__init__.py,sha256=S2W9JyeaUi2gbhweFKl-UyI7o1-tu7SSFtSDqCHA_Xk,3307
+athlib/__init__.py,sha256=2CxX7G2iyrtGO2U7IZlSG0N3lBgtvNXugjhDY7ztpKA,3361
 athlib/athlon_score.py,sha256=upnwOCEvxZPEElM4gt6qiAzHBUJ3PlYkCbHvfiJjALY,9593
+athlib/bulgarian_score.py,sha256=5MClMlGthXkrjg1A75nT283VsI6okkXhvoWmGuCXw_s,438962
 athlib/codes.py,sha256=6vDQXkQUaJrvw1gdIlCc5MLSwWEfgXTxMIFYoVZ9vo0,6884
 athlib/exceptions.py,sha256=-Z8IQmqTJl3Gc46BCMKUKF-lmMfYc5cmuH2hh6bI1cI,278
 athlib/highjump.py,sha256=Zc2oadVd-Y3uZRWVvo_d0EDQ1zoOrFV-wCuS3BTzqaA,19215
 athlib/hungarian_score.py,sha256=hZEo5_3zuutAsn0q3O57rBTj24b37Xnrd3r-ize1Y50,7401
 athlib/implements.py,sha256=FXAGETJc64RA3ud0g5FnIik25CS001zG2WTgKRgRWMg,6716
 athlib/jsondict.py,sha256=pOOmn1lH-Je2zs_qq2SI1eL_96kaS2AtFrRfu7rAw-o,4396
 athlib/qkids_score.py,sha256=oHCD3OuMGiB96KeESmRoLfSOinfPIBS2Pma2Hjd6RJw,2803
@@ -14,12 +15,12 @@
 athlib/uka/agegroups.py,sha256=0oF32MB0jwdzeHh-pJ_TrgPS9RoRBkZHBx8qR2MteMc,11532
 athlib/wma/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 athlib/wma/agegrader.py,sha256=Z5vDADQGI-0Z5RSSW_E0frZ9JxiEq4r-fjya1E_qFjc,9996
 athlib/wma/wma-athlons-data.json,sha256=FSx9_LSR2Ocwnvax-9HlSgmH2lfU0XQOyTVA3wcV-YE,4575
 athlib/wma/wma-data.json,sha256=HjiMF9FAFsZy44ylalySrwiCRGAzTJ2AhBxUbZGUB3E,92650
 athlib/wma/__pycache__/__init__.cpython-39.pyc,sha256=oRUC2PIPBBP02ZGjquj_TaBv3i31fpx9YCrtvEAj-fM,137
 athlib/wma/__pycache__/agegrader.cpython-39.pyc,sha256=a9uPWyhw8DKcD1XNXhN-PovpvjtGAtcrBnI32Y4nLdQ,9116
-athlib-0.7.8.dist-info/LICENSE,sha256=tAkwu8-AdEyGxGoSvJ2gVmQdcicWw3j1ZZueVV74M-E,11357
-athlib-0.7.8.dist-info/METADATA,sha256=VVbmAiJK8bkBhwIT_QKQhfTlVakN92UUmxkWEBVzxko,821
-athlib-0.7.8.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-athlib-0.7.8.dist-info/top_level.txt,sha256=avX3ZjuGfXEoo_CNHCDSy_ZamQt2-PH7QXh7bJPqG2A,7
-athlib-0.7.8.dist-info/RECORD,,
+athlib-0.7.9.dist-info/LICENSE,sha256=tAkwu8-AdEyGxGoSvJ2gVmQdcicWw3j1ZZueVV74M-E,11357
+athlib-0.7.9.dist-info/METADATA,sha256=oH_hEjJqTNytkZj1C8tg0KGJLxxt-Zzmy1QD2wr3gtM,821
+athlib-0.7.9.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+athlib-0.7.9.dist-info/top_level.txt,sha256=avX3ZjuGfXEoo_CNHCDSy_ZamQt2-PH7QXh7bJPqG2A,7
+athlib-0.7.9.dist-info/RECORD,,
```

