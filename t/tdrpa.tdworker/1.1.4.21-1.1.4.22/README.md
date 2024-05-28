# Comparing `tmp/tdrpa.tdworker-1.1.4.21-py39-none-win_amd64.whl.zip` & `tmp/tdrpa.tdworker-1.1.4.22-py39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 456996 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat  1310720 b- defN 24-May-28 11:51 tdrpa/tdworker.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      167 b- defN 24-May-28 11:45 tdrpa/tdworker/__init__.pyi
+Zip file size: 456986 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat  1310720 b- defN 24-May-28 15:30 tdrpa/tdworker.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      138 b- defN 24-May-28 15:16 tdrpa/tdworker/__init__.pyi
 -rw-rw-rw-  2.0 fat     5043 b- defN 24-May-28 11:45 tdrpa/tdworker/_w.pyi
 -rw-rw-rw-  2.0 fat    17514 b- defN 24-May-28 11:45 tdrpa/tdworker/_winE.pyi
 -rw-rw-rw-  2.0 fat     5419 b- defN 24-May-28 11:46 tdrpa/tdworker/_winK.pyi
 -rw-rw-rw-  2.0 fat     7936 b- defN 24-May-28 11:46 tdrpa/tdworker/_winM.pyi
--rw-rw-rw-  2.0 fat      709 b- defN 24-May-28 11:51 tdrpa.tdworker-1.1.4.21.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-28 11:51 tdrpa.tdworker-1.1.4.21.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-May-28 11:51 tdrpa.tdworker-1.1.4.21.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      834 b- defN 24-May-28 11:51 tdrpa.tdworker-1.1.4.21.dist-info/RECORD
-10 files, 1348440 bytes uncompressed, 455572 bytes compressed:  66.2%
+-rw-rw-rw-  2.0 fat      709 b- defN 24-May-28 15:30 tdrpa.tdworker-1.1.4.22.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-28 15:30 tdrpa.tdworker-1.1.4.22.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-28 15:30 tdrpa.tdworker-1.1.4.22.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      834 b- defN 24-May-28 15:30 tdrpa.tdworker-1.1.4.22.dist-info/RECORD
+10 files, 1348411 bytes uncompressed, 455562 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: tdrpa/tdworker/_winK.pyi
 Comment: 
 
 Filename: tdrpa/tdworker/_winM.pyi
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.21.dist-info/METADATA
+Filename: tdrpa.tdworker-1.1.4.22.dist-info/METADATA
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.21.dist-info/WHEEL
+Filename: tdrpa.tdworker-1.1.4.22.dist-info/WHEEL
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.21.dist-info/top_level.txt
+Filename: tdrpa.tdworker-1.1.4.22.dist-info/top_level.txt
 Comment: 
 
-Filename: tdrpa.tdworker-1.1.4.21.dist-info/RECORD
+Filename: tdrpa.tdworker-1.1.4.22.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tdrpa/tdworker/__init__.pyi

```diff
@@ -1,4 +1,5 @@
-from ._w import Window as Window
-from ._winE import WinElement as WinElement
-from ._winK import WinKeyboard as WinKeyboard
-from ._winM import WinMouse as WinMouse
+from ._w import Window
+from ._winE import WinElement
+from ._winK import WinKeyboard
+from ._winM import WinMouse
+from ._i import data
```

## Comparing `tdrpa.tdworker-1.1.4.21.dist-info/METADATA` & `tdrpa.tdworker-1.1.4.22.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdrpa.tdworker
-Version: 1.1.4.21
+Version: 1.1.4.22
 Summary: tdworker for tdrpa developers. supports python3.8+, windows x64
 Home-page: https://www.showdoc.com.cn/tdworker
 Author: vx:RPA_CREATOR
 Author-email: oldplayerliu@gmail.com
 License: Apache 2.0
 Keywords: RPA,tdRPA,tdworker,rpaworker,worker,uiautomation,uia,creator,windows,python,bot,robot,aigc,ai
 Platform: Windows Only
```

