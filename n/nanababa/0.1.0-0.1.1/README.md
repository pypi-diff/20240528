# Comparing `tmp/nanababa-0.1.0-py3-none-any.whl.zip` & `tmp/nanababa-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 1854 bytes, number of entries: 7
--rw-r--r--  2.0 unx       24 b- defN 24-May-28 03:27 something/__init__.py
+Zip file size: 1850 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       32 b- defN 24-May-28 03:43 something/__init__.py
 -rw-r--r--  2.0 unx       47 b- defN 24-May-28 03:24 something/something.py
--rw-r--r--  2.0 unx      433 b- defN 24-May-28 03:29 nanababa-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-28 03:29 nanababa-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       62 b- defN 24-May-28 03:29 nanababa-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 24-May-28 03:29 nanababa-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      550 b- defN 24-May-28 03:29 nanababa-0.1.0.dist-info/RECORD
-7 files, 1218 bytes uncompressed, 868 bytes compressed:  28.7%
+-rw-r--r--  2.0 unx      433 b- defN 24-May-28 03:43 nanababa-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 03:43 nanababa-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       62 b- defN 24-May-28 03:43 nanababa-0.1.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 24-May-28 03:43 nanababa-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      550 b- defN 24-May-28 03:43 nanababa-0.1.1.dist-info/RECORD
+7 files, 1226 bytes uncompressed, 864 bytes compressed:  29.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: something/__init__.py
 Comment: 
 
 Filename: something/something.py
 Comment: 
 
-Filename: nanababa-0.1.0.dist-info/METADATA
+Filename: nanababa-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: nanababa-0.1.0.dist-info/WHEEL
+Filename: nanababa-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: nanababa-0.1.0.dist-info/entry_points.txt
+Filename: nanababa-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: nanababa-0.1.0.dist-info/top_level.txt
+Filename: nanababa-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: nanababa-0.1.0.dist-info/RECORD
+Filename: nanababa-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## something/__init__.py

```diff
@@ -1 +1 @@
-from .something import *
+from .something import something
```

