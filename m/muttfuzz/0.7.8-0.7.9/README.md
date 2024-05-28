# Comparing `tmp/muttfuzz-0.7.8-py3-none-any.whl.zip` & `tmp/muttfuzz-0.7.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8871 bytes, number of entries: 8
--rw-r--r--  2.0 unx     4692 b- defN 24-May-28 11:03 muttfuzz/fuzz.py
--rw-r--r--  2.0 unx     9618 b- defN 24-May-28 11:03 muttfuzz/fuzzutil.py
+Zip file size: 8878 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     4755 b- defN 24-May-28 11:08 muttfuzz/fuzz.py
+-rw-r--r--  2.0 unx     9665 b- defN 24-May-28 11:08 muttfuzz/fuzzutil.py
 -rw-r--r--  2.0 unx     5721 b- defN 24-May-28 10:34 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     4589 b- defN 24-May-28 11:03 muttfuzz-0.7.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-28 11:03 muttfuzz-0.7.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-May-28 11:03 muttfuzz-0.7.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-28 11:03 muttfuzz-0.7.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      622 b- defN 24-May-28 11:03 muttfuzz-0.7.8.dist-info/RECORD
-8 files, 25404 bytes uncompressed, 7787 bytes compressed:  69.3%
+-rw-r--r--  2.0 unx     4589 b- defN 24-May-28 11:08 muttfuzz-0.7.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 11:08 muttfuzz-0.7.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-May-28 11:08 muttfuzz-0.7.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-28 11:08 muttfuzz-0.7.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      622 b- defN 24-May-28 11:08 muttfuzz-0.7.9.dist-info/RECORD
+8 files, 25514 bytes uncompressed, 7794 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.7.8.dist-info/METADATA
+Filename: muttfuzz-0.7.9.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.7.8.dist-info/WHEEL
+Filename: muttfuzz-0.7.9.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.7.8.dist-info/entry_points.txt
+Filename: muttfuzz-0.7.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.7.8.dist-info/top_level.txt
+Filename: muttfuzz-0.7.9.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.7.8.dist-info/RECORD
+Filename: muttfuzz-0.7.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/fuzz.py

```diff
@@ -76,14 +76,15 @@
                                    config.reachability_check_timeout,
                                    config.prune_mutant_cmd,
                                    config.prune_mutant_timeout,
                                    config.initial_fuzz_cmd,
                                    config.initial_budget,
                                    config.post_initial_cmd,
                                    config.post_mutant_cmd,
+                                   config.post_mutant_timeout,
                                    config.status_cmd,
                                    config.order)
     except IndexError:
         print("Target binary seems to have no jumps, so mutation will not do anything!")
```

## muttfuzz/fuzzutil.py

```diff
@@ -67,14 +67,15 @@
                       reachability_check_timeout=2.0,
                       prune_mutant_cmd="",
                       prune_mutant_timeout=2.0,
                       initial_fuzz_cmd="",
                       initial_budget=0,
                       post_initial_cmd="",
                       post_mutant_cmd="",
+                      post_mutant_timeout=2.0,
                       status_cmd="",
                       order=1):
     executable_code = mutate.get_code(executable)
     executable_jumps = mutate.get_jumps(executable, only_mutate, avoid_mutating)
     start_fuzz = time.time()
     mutant_no = 1
     try:
```

## Comparing `muttfuzz-0.7.8.dist-info/METADATA` & `muttfuzz-0.7.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.7.8
+Version: 0.7.9
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

## Comparing `muttfuzz-0.7.8.dist-info/RECORD` & `muttfuzz-0.7.9.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-muttfuzz/fuzz.py,sha256=bS8JZtHP89PeKi08XROeopjalCYq54P9uokhCIeMK5Q,4692
-muttfuzz/fuzzutil.py,sha256=DciExYT6J-FVo9aJ_8XoJQ7b_NXYigss1ZgolmHpEMg,9618
+muttfuzz/fuzz.py,sha256=k0LrPfj2xcgRXVFOUfCZjFoQioiLJMQg6X5o76_tS0o,4755
+muttfuzz/fuzzutil.py,sha256=GZ5Aq0TAwCObwb-LBkw_eMxW6rIBuUht6tTYuSlx7Hs,9665
 muttfuzz/mutate.py,sha256=EUFlHVAhzW9FSBuaNz-nHtcp_CgGgQCOyLyzQEyHPxQ,5721
-muttfuzz-0.7.8.dist-info/METADATA,sha256=JDf-uYR6rfo5gt1sccOQiMupUsTiYDdEPf_Nt5uX-bM,4589
-muttfuzz-0.7.8.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-muttfuzz-0.7.8.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
-muttfuzz-0.7.8.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
-muttfuzz-0.7.8.dist-info/RECORD,,
+muttfuzz-0.7.9.dist-info/METADATA,sha256=WRXytJrSrsw8CXAUxhW_RqD6Oi-USVatvotA_qaJIxs,4589
+muttfuzz-0.7.9.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+muttfuzz-0.7.9.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
+muttfuzz-0.7.9.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
+muttfuzz-0.7.9.dist-info/RECORD,,
```

