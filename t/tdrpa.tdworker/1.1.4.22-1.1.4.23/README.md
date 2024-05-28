# Comparing `tmp/tdrpa.tdworker-1.1.4.22-py39-none-win_amd64.whl.zip` & `tmp/tdrpa.tdworker-1.1.4.23-py39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 456986 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat  1310720 b- defN 24-May-28 15:30 tdrpa/tdworker.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      138 b- defN 24-May-28 15:16 tdrpa/tdworker/__init__.pyi
+Zip file size: 460011 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat  1313280 b- defN 24-May-28 16:01 tdrpa/tdworker.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      116 b- defN 24-May-28 15:52 tdrpa/tdworker/__init__.pyi
 -rw-rw-rw-  2.0 fat     5043 b- defN 24-May-28 11:45 tdrpa/tdworker/_w.pyi
 -rw-rw-rw-  2.0 fat    17514 b- defN 24-May-28 11:45 tdrpa/tdworker/_winE.pyi
 -rw-rw-rw-  2.0 fat     5419 b- defN 24-May-28 11:46 tdrpa/tdworker/_winK.pyi
 -rw-rw-rw-  2.0 fat     7936 b- defN 24-May-28 11:46 tdrpa/tdworker/_winM.pyi
--rw-rw-rw-  2.0 fat      709 b- defN 24-May-28 15:30 tdrpa.tdworker-1.1.4.22.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-28 15:30 tdrpa.tdworker-1.1.4.22.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-May-28 15:30 tdrpa.tdworker-1.1.4.22.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      834 b- defN 24-May-28 15:30 tdrpa.tdworker-1.1.4.22.dist-info/RECORD
-10 files, 1348411 bytes uncompressed, 455562 bytes compressed:  66.2%
+-rw-rw-rw-  2.0 fat      709 b- defN 24-May-28 16:01 tdrpa.tdworker-1.1.4.23.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-28 16:01 tdrpa.tdworker-1.1.4.23.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-28 16:01 tdrpa.tdworker-1.1.4.23.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      834 b- defN 24-May-28 16:01 tdrpa.tdworker-1.1.4.23.dist-info/RECORD
+10 files, 1350949 bytes uncompressed, 458587 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: tdrpa/tdworker/_winK.pyi
 Comment: 
 
 Filename: tdrpa/tdworker/_winM.pyi
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.22.dist-info/METADATA
+Filename: tdrpa.tdworker-1.1.4.23.dist-info/METADATA
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.22.dist-info/WHEEL
+Filename: tdrpa.tdworker-1.1.4.23.dist-info/WHEEL
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.22.dist-info/top_level.txt
+Filename: tdrpa.tdworker-1.1.4.23.dist-info/top_level.txt
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.22.dist-info/RECORD
+Filename: tdrpa.tdworker-1.1.4.23.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tdrpa/tdworker/__init__.pyi

```diff
@@ -1,5 +1,4 @@
 from ._w import Window
 from ._winE import WinElement
 from ._winK import WinKeyboard
 from ._winM import WinMouse
-from ._i import data
```

## Comparing `tdrpa.tdworker-1.1.4.22.dist-info/METADATA` & `tdrpa.tdworker-1.1.4.23.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdrpa.tdworker
-Version: 1.1.4.22
+Version: 1.1.4.23
 Summary: tdworker for tdrpa developers. supports python3.8+, windows x64
 Home-page: https://www.showdoc.com.cn/tdworker
 Author: vx:RPA_CREATOR
 Author-email: oldplayerliu@gmail.com
 License: Apache 2.0
 Keywords: RPA,tdRPA,tdworker,rpaworker,worker,uiautomation,uia,creator,windows,python,bot,robot,aigc,ai
 Platform: Windows Only
```

## Comparing `tdrpa.tdworker-1.1.4.22.dist-info/RECORD` & `tdrpa.tdworker-1.1.4.23.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-tdrpa/tdworker.cp39-win_amd64.pyd,sha256=twHhGM30rqoAHTtWkJqKqcbEtAhr0NLA41H2RlLnoKQ,1310720
-tdrpa/tdworker/__init__.pyi,sha256=eo6H_RM9ddvqmxIobBMiQATtrIDrExG31tLOU7AXpPY,138
+tdrpa/tdworker.cp39-win_amd64.pyd,sha256=MTwjY-VP3RVJetormbwpTg-dMPD7wLnllBX8jhSV7QA,1313280
+tdrpa/tdworker/__init__.pyi,sha256=n_psnvjeF6Cn_Gk-PKQqgXIU3-QValxeBLdszf-P3sY,116
 tdrpa/tdworker/_w.pyi,sha256=sleUdSrw0lLsBzpTHobCm8sPa0oS-c08XSersrEUBnw,5043
 tdrpa/tdworker/_winE.pyi,sha256=8lBiTZvP1K3LXEgPNdyfpl42x9AK3JiuBdSz3vsdXyo,17514
 tdrpa/tdworker/_winK.pyi,sha256=qHWt3fsjbfokBNnmt30oqJxeNELrCJznhXSNyCECDBs,5419
 tdrpa/tdworker/_winM.pyi,sha256=imb92Y2LGhsy-nXKyOYlcU0TLmEKddZQ4aSyoGWfGwU,7936
-tdrpa.tdworker-1.1.4.22.dist-info/METADATA,sha256=VwHMw2RI0YMhLfNryV_6gT1pIVyjzoLDlgjh9Tc-6UA,709
-tdrpa.tdworker-1.1.4.22.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-tdrpa.tdworker-1.1.4.22.dist-info/top_level.txt,sha256=S9UoqmC_cyGqKbGsBkLQPEeQLbDrWD0SRwbxPpQpyyU,6
-tdrpa.tdworker-1.1.4.22.dist-info/RECORD,,
+tdrpa.tdworker-1.1.4.23.dist-info/METADATA,sha256=mZS8N70DbP2dvd_ZMWd52pZBqB4rUI9hiQT4EfUjUg8,709
+tdrpa.tdworker-1.1.4.23.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+tdrpa.tdworker-1.1.4.23.dist-info/top_level.txt,sha256=S9UoqmC_cyGqKbGsBkLQPEeQLbDrWD0SRwbxPpQpyyU,6
+tdrpa.tdworker-1.1.4.23.dist-info/RECORD,,
```

