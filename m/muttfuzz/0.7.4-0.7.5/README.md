# Comparing `tmp/muttfuzz-0.7.4-py3-none-any.whl.zip` & `tmp/muttfuzz-0.7.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8684 bytes, number of entries: 8
+Zip file size: 8681 bytes, number of entries: 8
 -rw-r--r--  2.0 unx     4559 b- defN 24-May-28 03:37 muttfuzz/fuzz.py
 -rw-r--r--  2.0 unx     9345 b- defN 24-May-28 03:37 muttfuzz/fuzzutil.py
--rw-r--r--  2.0 unx     5142 b- defN 24-May-28 03:37 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     4589 b- defN 24-May-28 03:37 muttfuzz-0.7.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-28 03:37 muttfuzz-0.7.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-May-28 03:37 muttfuzz-0.7.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-28 03:37 muttfuzz-0.7.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      622 b- defN 24-May-28 03:37 muttfuzz-0.7.4.dist-info/RECORD
-8 files, 24419 bytes uncompressed, 7600 bytes compressed:  68.9%
+-rw-r--r--  2.0 unx     5145 b- defN 24-May-28 03:40 muttfuzz/mutate.py
+-rw-r--r--  2.0 unx     4589 b- defN 24-May-28 03:40 muttfuzz-0.7.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 03:40 muttfuzz-0.7.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-May-28 03:40 muttfuzz-0.7.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-28 03:40 muttfuzz-0.7.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      622 b- defN 24-May-28 03:40 muttfuzz-0.7.5.dist-info/RECORD
+8 files, 24422 bytes uncompressed, 7597 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.7.4.dist-info/METADATA
+Filename: muttfuzz-0.7.5.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.7.4.dist-info/WHEEL
+Filename: muttfuzz-0.7.5.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.7.4.dist-info/entry_points.txt
+Filename: muttfuzz-0.7.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.7.4.dist-info/top_level.txt
+Filename: muttfuzz-0.7.5.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.7.4.dist-info/RECORD
+Filename: muttfuzz-0.7.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/mutate.py

```diff
@@ -99,15 +99,15 @@
         return bytearray(f.read())
 
 def mutant_from(code, jumps, order=1):
     new_code = bytearray(code)
     reach_code = bytearray(code)
     for i in range(order): # allows higher-order mutants, though can undo mutations
         (loc, new_data) = pick_and_change(jumps)
-        reach_code[loc] = HALT
+        reach_code[loc] = HALT[0]
         for offset in range(0, len(new_data)):
             new_code[loc + offset] = new_data[offset]
     return (new_code, reach_code)
 
 def mutant(filename, order=1, avoid_mutating=[]):
     return mutant_from(get_code(filename), get_jumps(filename, avoid_mutating), order=order)
```

## Comparing `muttfuzz-0.7.4.dist-info/METADATA` & `muttfuzz-0.7.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.7.4
+Version: 0.7.5
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

## Comparing `muttfuzz-0.7.4.dist-info/RECORD` & `muttfuzz-0.7.5.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 muttfuzz/fuzz.py,sha256=_9UOO9giNQiUNWAbJDQO0LB8jgkbyqf8lZ04ck-hZGI,4559
 muttfuzz/fuzzutil.py,sha256=FGvQNwfclsHPK5Wlp904npeuShPy_KOwUbezcXSNh4E,9345
-muttfuzz/mutate.py,sha256=RA6iQJzK5ruTwoTzaWRRO6zuhBiB_b4HJfkC5gf9z0w,5142
-muttfuzz-0.7.4.dist-info/METADATA,sha256=f6JwBShAGK5P4urXfbLI6nx2w-pXMvWppJ6gRHv-Cyo,4589
-muttfuzz-0.7.4.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-muttfuzz-0.7.4.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
-muttfuzz-0.7.4.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
-muttfuzz-0.7.4.dist-info/RECORD,,
+muttfuzz/mutate.py,sha256=ctqTDrYlWyCDB6xHCAb7C5HBzLipxgzzlj_pY79Et88,5145
+muttfuzz-0.7.5.dist-info/METADATA,sha256=ySUo8NQlWHlkOQBZq5lulG241SMk0P8DhCy_y5_KS34,4589
+muttfuzz-0.7.5.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+muttfuzz-0.7.5.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
+muttfuzz-0.7.5.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
+muttfuzz-0.7.5.dist-info/RECORD,,
```

