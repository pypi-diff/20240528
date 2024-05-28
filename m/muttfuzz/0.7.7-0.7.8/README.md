# Comparing `tmp/muttfuzz-0.7.7-py3-none-any.whl.zip` & `tmp/muttfuzz-0.7.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8820 bytes, number of entries: 8
--rw-r--r--  2.0 unx     4559 b- defN 24-May-28 03:37 muttfuzz/fuzz.py
--rw-r--r--  2.0 unx     9353 b- defN 24-May-28 03:44 muttfuzz/fuzzutil.py
+Zip file size: 8871 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     4692 b- defN 24-May-28 11:03 muttfuzz/fuzz.py
+-rw-r--r--  2.0 unx     9618 b- defN 24-May-28 11:03 muttfuzz/fuzzutil.py
 -rw-r--r--  2.0 unx     5721 b- defN 24-May-28 10:34 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     4589 b- defN 24-May-28 10:34 muttfuzz-0.7.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-28 10:34 muttfuzz-0.7.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-May-28 10:34 muttfuzz-0.7.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-28 10:34 muttfuzz-0.7.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      622 b- defN 24-May-28 10:34 muttfuzz-0.7.7.dist-info/RECORD
-8 files, 25006 bytes uncompressed, 7736 bytes compressed:  69.1%
+-rw-r--r--  2.0 unx     4589 b- defN 24-May-28 11:03 muttfuzz-0.7.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 11:03 muttfuzz-0.7.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-May-28 11:03 muttfuzz-0.7.8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-28 11:03 muttfuzz-0.7.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      622 b- defN 24-May-28 11:03 muttfuzz-0.7.8.dist-info/RECORD
+8 files, 25404 bytes uncompressed, 7787 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.7.7.dist-info/METADATA
+Filename: muttfuzz-0.7.8.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.7.7.dist-info/WHEEL
+Filename: muttfuzz-0.7.8.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.7.7.dist-info/entry_points.txt
+Filename: muttfuzz-0.7.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.7.7.dist-info/top_level.txt
+Filename: muttfuzz-0.7.8.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.7.7.dist-info/RECORD
+Filename: muttfuzz-0.7.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/fuzz.py

```diff
@@ -32,15 +32,17 @@
     parser.add_argument('--initial_fuzz_cmd', type=str, default="",
                         help='command for initial fuzzing before mutants')
     parser.add_argument('--initial_budget', type=int, default=60,
                         help='how long to run initial fuzzing, in seconds (default 60)')
     parser.add_argument('--post_initial_cmd', type=str, default="",
                         help='command to run after initial fuzzing')
     parser.add_argument('--post_mutant_cmd', type=str, default="",
-                        help='command to run after each mutant, (e.g., for AFL_SKIP_CRASHES)')
+                        help='command to run after each mutant (e.g., fuzz of original)')
+    parser.add_argument('--post_mutant_timeout', type=float, default=2.0,
+                        help='timeout for post-mutant command')
     parser.add_argument('--order', type=int, default=1,
                         help='mutation order (default 1)')
     parser.add_argument('--status_cmd', type=str, default="",
                         help='command to execute to show fuzzing stats')
 
     parsed_args = parser.parse_args(sys.argv[1:])
     return (parsed_args, parser)
```

## muttfuzz/fuzzutil.py

```diff
@@ -125,16 +125,19 @@
                         mutant_ok = False
             if mutant_ok:
                 print("FUZZING MUTANT...")
                 start_run = time.time()
                 silent_run_with_timeout(fuzzer_cmd, time_per_mutant)
                 print("FINISHED FUZZING IN", round(time.time() - start_run, 2), "SECONDS")
                 if post_mutant_cmd != "":
-                    subprocess.call(post_mutant_cmd, shell=True)
+                    restore_executable(executable, executable_code) # Might need original for post
+                    print("RUNNING POST-MUTANT COMMAND")
+                    silent_run_with_timeout(post_mutant_cmd, post_mutant_timeout)
                 if status_cmd != "":
+                    restore_executable(executable, executable_code) # Might need for status
                     print("STATUS:")
                     subprocess.call(status_cmd, shell=True)
 
         print(datetime.utcfromtimestamp(time.time()).strftime('%Y-%m-%d %H:%M:%S'))
         print(round(time.time() - start_fuzz, 2), "ELAPSED: STARTING FINAL FUZZ")
         restore_executable(executable, executable_code)
         silent_run_with_timeout(fuzzer_cmd, budget - (time.time() - start_fuzz))
```

## Comparing `muttfuzz-0.7.7.dist-info/METADATA` & `muttfuzz-0.7.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.7.7
+Version: 0.7.8
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

## Comparing `muttfuzz-0.7.7.dist-info/RECORD` & `muttfuzz-0.7.8.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-muttfuzz/fuzz.py,sha256=_9UOO9giNQiUNWAbJDQO0LB8jgkbyqf8lZ04ck-hZGI,4559
-muttfuzz/fuzzutil.py,sha256=HM9C3dUws1ELRHVpe4hd1cRANvS15oQk4rfszpLAZB8,9353
+muttfuzz/fuzz.py,sha256=bS8JZtHP89PeKi08XROeopjalCYq54P9uokhCIeMK5Q,4692
+muttfuzz/fuzzutil.py,sha256=DciExYT6J-FVo9aJ_8XoJQ7b_NXYigss1ZgolmHpEMg,9618
 muttfuzz/mutate.py,sha256=EUFlHVAhzW9FSBuaNz-nHtcp_CgGgQCOyLyzQEyHPxQ,5721
-muttfuzz-0.7.7.dist-info/METADATA,sha256=bM1fAsOP06OWhtOQ5BMHRJqnfeClvA9nGumZ69Byv9g,4589
-muttfuzz-0.7.7.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-muttfuzz-0.7.7.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
-muttfuzz-0.7.7.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
-muttfuzz-0.7.7.dist-info/RECORD,,
+muttfuzz-0.7.8.dist-info/METADATA,sha256=JDf-uYR6rfo5gt1sccOQiMupUsTiYDdEPf_Nt5uX-bM,4589
+muttfuzz-0.7.8.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+muttfuzz-0.7.8.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
+muttfuzz-0.7.8.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
+muttfuzz-0.7.8.dist-info/RECORD,,
```

