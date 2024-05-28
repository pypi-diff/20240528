# Comparing `tmp/muttfuzz-0.7.6-py3-none-any.whl.zip` & `tmp/muttfuzz-0.7.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8687 bytes, number of entries: 8
+Zip file size: 8820 bytes, number of entries: 8
 -rw-r--r--  2.0 unx     4559 b- defN 24-May-28 03:37 muttfuzz/fuzz.py
 -rw-r--r--  2.0 unx     9353 b- defN 24-May-28 03:44 muttfuzz/fuzzutil.py
--rw-r--r--  2.0 unx     5145 b- defN 24-May-28 03:40 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     4589 b- defN 24-May-28 03:44 muttfuzz-0.7.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-28 03:44 muttfuzz-0.7.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-May-28 03:44 muttfuzz-0.7.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-28 03:44 muttfuzz-0.7.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      622 b- defN 24-May-28 03:44 muttfuzz-0.7.6.dist-info/RECORD
-8 files, 24430 bytes uncompressed, 7603 bytes compressed:  68.9%
+-rw-r--r--  2.0 unx     5721 b- defN 24-May-28 10:34 muttfuzz/mutate.py
+-rw-r--r--  2.0 unx     4589 b- defN 24-May-28 10:34 muttfuzz-0.7.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 10:34 muttfuzz-0.7.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-May-28 10:34 muttfuzz-0.7.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-28 10:34 muttfuzz-0.7.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      622 b- defN 24-May-28 10:34 muttfuzz-0.7.7.dist-info/RECORD
+8 files, 25006 bytes uncompressed, 7736 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.7.6.dist-info/METADATA
+Filename: muttfuzz-0.7.7.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.7.6.dist-info/WHEEL
+Filename: muttfuzz-0.7.7.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.7.6.dist-info/entry_points.txt
+Filename: muttfuzz-0.7.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.7.6.dist-info/top_level.txt
+Filename: muttfuzz-0.7.7.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.7.6.dist-info/RECORD
+Filename: muttfuzz-0.7.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/mutate.py

```diff
@@ -1,15 +1,19 @@
 import random
 import subprocess
 
 JUMP_OPCODES = ["je", "jne", "jl", "jle", "jg", "jge"]
 SHORT_JUMPS = list(map(bytes.fromhex, ["74", "75", "7C", "7D", "7E", "7F", "EB"]))
 SHORT_NAMES = dict(zip(SHORT_JUMPS, ["je", "jne", "jl", "jge", "jle", "jg", "jmp"]))
+SHORT_OPPOSITES = list(map(bytes.fromhex, ["75", "74", "7D", "7C", "7F", "7E"]))
+SHORT_FLIP = dict(zip(map(lambda x: x[0], SHORT_JUMPS[:-1]), SHORT_OPPOSITES))
 NEAR_JUMPS = list(map(bytes.fromhex, ["0F 84", "0F 85", "0F 8C", "0F 8D", "0F 8E", "0F 8F", "90 E9"]))
 NEAR_NAMES = dict(zip(NEAR_JUMPS, ["je", "jne", "jl", "jge", "jle", "jg", "jmp"]))
+NEAR_OPPOSITES = list(map(bytes.fromhex, ["0F 85", "0F 84", "0F 8D", "0F 8C", "0F 8F", "0F 8E"]))
+NEAR_FLIP = dict(zip(map(lambda x: x[1], NEAR_JUMPS[:-1]), NEAR_OPPOSITES))
 
 NOP = bytes.fromhex("90") # Needed to erase a jump
 HALT = bytes.fromhex("F4") # Needed for reachability check
 
 # known markers for fuzzer/compiler injected instrumentation/etc.
 INST_SET = ["__afl", "__asan", "__ubsan", "__sanitizer", "__lsan", "__sancov", "AFL_"]
 INST_SET.extend(["DeepState", "deepstate"])
@@ -63,17 +67,24 @@
                     jumps[loc] = (opcode, bytes.fromhex(fields[1]), section_name, line)
         except: # If we can't parse some line in the objdump, just skip it
             pass
 
     return jumps
 
 def different_jump(hexdata):
+    P_FLIP = 0.70
+    # First, just flip the jump condition 70% of the time
+    if (random.random() <= P_FLIP):
+        if hexdata[0] == 15: # NEAR JUMP
+            return NEAR_FLIP[hexdata[1]]
+        else:
+            return SHORT_FLIP[hexdata[0]]
     P_DC = 0.40 # P(Don't Care)
     P_DC_JMP = P_DC / (1 - P_DC)
-    # Current approach is to change to "don't care" (take or avoid) 80% of time, mutate 20%
+    # Then change to "don't care" (take or avoid) 80% of time, mutate otherwise 20%
     if (random.random() <= P_DC): # Just remove the jump by providing a NOP sled
         return NOP * len(hexdata)
     if hexdata[0] == 15: # NEAR JUMP BYTE CHECK
         if random.random() <= P_DC_JMP:
             return NEAR_JUMPS[-1]
         return random.choice(list(filter(lambda j: j[1] != hexdata[1], NEAR_JUMPS[:-1])))
     else:
```

## Comparing `muttfuzz-0.7.6.dist-info/METADATA` & `muttfuzz-0.7.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.7.6
+Version: 0.7.7
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

## Comparing `muttfuzz-0.7.6.dist-info/RECORD` & `muttfuzz-0.7.7.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 muttfuzz/fuzz.py,sha256=_9UOO9giNQiUNWAbJDQO0LB8jgkbyqf8lZ04ck-hZGI,4559
 muttfuzz/fuzzutil.py,sha256=HM9C3dUws1ELRHVpe4hd1cRANvS15oQk4rfszpLAZB8,9353
-muttfuzz/mutate.py,sha256=ctqTDrYlWyCDB6xHCAb7C5HBzLipxgzzlj_pY79Et88,5145
-muttfuzz-0.7.6.dist-info/METADATA,sha256=JFCRiomLFIjd_qGE5EJVUZRVMLHZo1KdwQTE6vujI04,4589
-muttfuzz-0.7.6.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-muttfuzz-0.7.6.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
-muttfuzz-0.7.6.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
-muttfuzz-0.7.6.dist-info/RECORD,,
+muttfuzz/mutate.py,sha256=EUFlHVAhzW9FSBuaNz-nHtcp_CgGgQCOyLyzQEyHPxQ,5721
+muttfuzz-0.7.7.dist-info/METADATA,sha256=bM1fAsOP06OWhtOQ5BMHRJqnfeClvA9nGumZ69Byv9g,4589
+muttfuzz-0.7.7.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+muttfuzz-0.7.7.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
+muttfuzz-0.7.7.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
+muttfuzz-0.7.7.dist-info/RECORD,,
```

