# Comparing `tmp/pip_earth-0.1-py3-none-any.whl.zip` & `tmp/pip_earth-0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2048 bytes, number of entries: 7
--rw-r--r--  2.0 unx      151 b- defN 24-May-28 05:52 pip_earth/__init__.py
+Zip file size: 2085 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      151 b- defN 24-May-28 06:48 pip_earth/__init__.py
 -rw-r--r--  2.0 unx      151 b- defN 24-May-28 05:52 pip_package/__init__.py
--rw-r--r--  2.0 unx      588 b- defN 24-May-28 06:26 pip_earth-0.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      303 b- defN 24-May-28 06:26 pip_earth-0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-28 06:26 pip_earth-0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-May-28 06:26 pip_earth-0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      544 b- defN 24-May-28 06:26 pip_earth-0.1.dist-info/RECORD
-7 files, 1839 bytes uncompressed, 1080 bytes compressed:  41.3%
+-rw-r--r--  2.0 unx      588 b- defN 24-May-28 06:53 pip_earth-0.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      303 b- defN 24-May-28 06:53 pip_earth-0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 06:53 pip_earth-0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-May-28 06:53 pip_earth-0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      544 b- defN 24-May-28 06:53 pip_earth-0.2.dist-info/RECORD
+7 files, 1839 bytes uncompressed, 1117 bytes compressed:  39.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pip_earth/__init__.py
 Comment: 
 
 Filename: pip_package/__init__.py
 Comment: 
 
-Filename: pip_earth-0.1.dist-info/LICENSE.txt
+Filename: pip_earth-0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pip_earth-0.1.dist-info/METADATA
+Filename: pip_earth-0.2.dist-info/METADATA
 Comment: 
 
-Filename: pip_earth-0.1.dist-info/WHEEL
+Filename: pip_earth-0.2.dist-info/WHEEL
 Comment: 
 
-Filename: pip_earth-0.1.dist-info/top_level.txt
+Filename: pip_earth-0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pip_earth-0.1.dist-info/RECORD
+Filename: pip_earth-0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pip_earth/__init__.py

```diff
@@ -1,8 +1,8 @@
-def add_numbers(a,b):
+def sum_numbers(a,b):
     return a+b
 
 def mul_numbers(a,b):
     return a*b
 
 def sub_numbers(a,b):
     return a-b
```

## Comparing `pip_earth-0.1.dist-info/LICENSE.txt` & `pip_earth-0.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

