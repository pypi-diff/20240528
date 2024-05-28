# Comparing `tmp/muttfuzz-0.7.1-py3-none-any.whl.zip` & `tmp/muttfuzz-0.7.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8456 bytes, number of entries: 8
+Zip file size: 8460 bytes, number of entries: 8
 -rw-r--r--  2.0 unx     4104 b- defN 24-May-25 14:57 muttfuzz/fuzz.py
 -rw-r--r--  2.0 unx     8432 b- defN 24-May-26 20:32 muttfuzz/fuzzutil.py
--rw-r--r--  2.0 unx     4932 b- defN 24-May-28 02:33 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     4589 b- defN 24-May-28 02:33 muttfuzz-0.7.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-28 02:33 muttfuzz-0.7.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-May-28 02:33 muttfuzz-0.7.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-28 02:33 muttfuzz-0.7.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      622 b- defN 24-May-28 02:33 muttfuzz-0.7.1.dist-info/RECORD
-8 files, 22841 bytes uncompressed, 7372 bytes compressed:  67.7%
+-rw-r--r--  2.0 unx     4937 b- defN 24-May-28 02:45 muttfuzz/mutate.py
+-rw-r--r--  2.0 unx     4589 b- defN 24-May-28 02:45 muttfuzz-0.7.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 02:45 muttfuzz-0.7.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-May-28 02:45 muttfuzz-0.7.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-28 02:45 muttfuzz-0.7.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      622 b- defN 24-May-28 02:45 muttfuzz-0.7.2.dist-info/RECORD
+8 files, 22846 bytes uncompressed, 7376 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.7.1.dist-info/METADATA
+Filename: muttfuzz-0.7.2.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.7.1.dist-info/WHEEL
+Filename: muttfuzz-0.7.2.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.7.1.dist-info/entry_points.txt
+Filename: muttfuzz-0.7.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.7.1.dist-info/top_level.txt
+Filename: muttfuzz-0.7.2.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.7.1.dist-info/RECORD
+Filename: muttfuzz-0.7.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/mutate.py

```diff
@@ -84,20 +84,20 @@
         return random.choice(list(filter(lambda j: j[0] != hexdata[0], SHORT_JUMPS[:-1])))
 
 def pick_and_change(jumps):
     loc = random.choice(list(jumps.keys()))
     changed = different_jump(jumps[loc][1])
     print("MUTATING JUMP IN", jumps[loc][2], "WITH ORIGINAL OPCODE", jumps[loc][0])
     print("ORIGINAL CODE:", jumps[loc][3])
-    if changed[0] == NOP:
-        print("CHANGING TO NOP")
-    elif changed in SHORT_NAMES:
+    if changed in SHORT_NAMES:
         print("CHANGING TO", SHORT_NAMES[changed])
-    else:
+    elif changed in NEAR_NAMES:
         print("CHANGING TO", NEAR_NAMES[changed])
+    else:
+        print("CHANGING TO NOPS")
     return (loc, changed)
 
 def get_code(filename):
     with open(filename, "rb") as f:
         return bytearray(f.read())
 
 def check_reachable(code, loc, reachability_check):
```

## Comparing `muttfuzz-0.7.1.dist-info/METADATA` & `muttfuzz-0.7.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.7.1
+Version: 0.7.2
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

## Comparing `muttfuzz-0.7.1.dist-info/RECORD` & `muttfuzz-0.7.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 muttfuzz/fuzz.py,sha256=3597RhXkUl4GQuIo5BFH-IHehOBqxqS5PYqjm1X21QU,4104
 muttfuzz/fuzzutil.py,sha256=dsIbVqP_XyZao6orvVPM2stGQU9bBM0CB-8M3CkzDpI,8432
-muttfuzz/mutate.py,sha256=A9aYrCOI9jbvvWQXLTbzmP8mqsqK0J3r4i-VkzJ_fbM,4932
-muttfuzz-0.7.1.dist-info/METADATA,sha256=Q8CIOA6mnRefCrORK55GVyL7xZycLXkt6loz0NJ9LQ0,4589
-muttfuzz-0.7.1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-muttfuzz-0.7.1.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
-muttfuzz-0.7.1.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
-muttfuzz-0.7.1.dist-info/RECORD,,
+muttfuzz/mutate.py,sha256=rA7KRN0eHh_BNbOxevnlNzZ-ApyQvMneYR_Udhr4E5Y,4937
+muttfuzz-0.7.2.dist-info/METADATA,sha256=wxCt2jpMtJmXWqQX0CLSNC1VEaPK4v5Ps0XPqQcHqZQ,4589
+muttfuzz-0.7.2.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+muttfuzz-0.7.2.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
+muttfuzz-0.7.2.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
+muttfuzz-0.7.2.dist-info/RECORD,,
```

