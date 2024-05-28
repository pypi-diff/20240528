# Comparing `tmp/muttfuzz-0.7.3-py3-none-any.whl.zip` & `tmp/muttfuzz-0.7.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8479 bytes, number of entries: 8
--rw-r--r--  2.0 unx     4104 b- defN 24-May-25 14:57 muttfuzz/fuzz.py
--rw-r--r--  2.0 unx     8432 b- defN 24-May-26 20:32 muttfuzz/fuzzutil.py
--rw-r--r--  2.0 unx     4978 b- defN 24-May-28 02:55 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     4589 b- defN 24-May-28 02:55 muttfuzz-0.7.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-28 02:55 muttfuzz-0.7.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-May-28 02:55 muttfuzz-0.7.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-28 02:55 muttfuzz-0.7.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      622 b- defN 24-May-28 02:55 muttfuzz-0.7.3.dist-info/RECORD
-8 files, 22887 bytes uncompressed, 7395 bytes compressed:  67.7%
+Zip file size: 8684 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     4559 b- defN 24-May-28 03:37 muttfuzz/fuzz.py
+-rw-r--r--  2.0 unx     9345 b- defN 24-May-28 03:37 muttfuzz/fuzzutil.py
+-rw-r--r--  2.0 unx     5142 b- defN 24-May-28 03:37 muttfuzz/mutate.py
+-rw-r--r--  2.0 unx     4589 b- defN 24-May-28 03:37 muttfuzz-0.7.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 03:37 muttfuzz-0.7.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-May-28 03:37 muttfuzz-0.7.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-28 03:37 muttfuzz-0.7.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      622 b- defN 24-May-28 03:37 muttfuzz-0.7.4.dist-info/RECORD
+8 files, 24419 bytes uncompressed, 7600 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.7.3.dist-info/METADATA
+Filename: muttfuzz-0.7.4.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.7.3.dist-info/WHEEL
+Filename: muttfuzz-0.7.4.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.7.3.dist-info/entry_points.txt
+Filename: muttfuzz-0.7.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.7.3.dist-info/top_level.txt
+Filename: muttfuzz-0.7.4.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.7.3.dist-info/RECORD
+Filename: muttfuzz-0.7.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/fuzz.py

```diff
@@ -17,14 +17,18 @@
                         help='max time to fuzz each mutant in seconds (default 300)')
     parser.add_argument('--fraction_mutant', type=float, default=0.5,
                         help='portion of budget to devote to mutants (default 0.5)')
     parser.add_argument('--only_mutate', type=str, default="",
                         help='string with comma delimited list of functions patterns to mutate (match by simple inclusion)')
     parser.add_argument('--avoid_mutating', type=str, default="",
                         help='string with comma delimited list of function patterns not to mutate (match by simple inclusion)')
+    parser.add_argument('--reachability_check_cmd', type=str, default="",
+                        help='command to check reachability; should return non-zero if some inputs crash')
+    parser.add_argument('--reachability_check_timeout', type=float, default=2.0,
+                        help='timeout for mutant check')
     parser.add_argument('--prune_mutant_cmd', type=str, default="",
                         help='command to check mutants for validity/interest')
     parser.add_argument('--prune_mutant_timeout', type=float, default=2.0,
                         help='timeout for mutant check')
     parser.add_argument('--initial_fuzz_cmd', type=str, default="",
                         help='command for initial fuzzing before mutants')
     parser.add_argument('--initial_budget', type=int, default=60,
@@ -62,14 +66,16 @@
         fuzzutil.fuzz_with_mutants(config.fuzzer_cmd,
                                    config.executable,
                                    config.budget,
                                    config.time_per_mutant,
                                    config.fraction_mutant,
                                    list(filter(None, config.only_mutate.replace(", ", ",").split(","))),
                                    list(filter(None, config.avoid_mutating.replace(", ", ",").split(","))),
+                                   config.reachability_check_cmd,
+                                   config.reachability_check_timeout,
                                    config.prune_mutant_cmd,
                                    config.prune_mutant_timeout,
                                    config.initial_fuzz_cmd,
                                    config.initial_budget,
                                    config.post_initial_cmd,
                                    config.post_mutant_cmd,
                                    config.status_cmd,
```

## muttfuzz/fuzzutil.py

```diff
@@ -59,16 +59,18 @@
             os.killpg(os.getpgid(P.pid), signal.SIGTERM)
     return P.returncode
 
 
 def fuzz_with_mutants(fuzzer_cmd, executable, budget, time_per_mutant, fraction_mutant,
                       only_mutate=[],
                       avoid_mutating=[],
+                      reachability_check_cmd="",
+                      reachability_check_timeout=2.0,
                       prune_mutant_cmd="",
-                      prune_mutant_timeout=1,
+                      prune_mutant_timeout=2.0,
                       initial_fuzz_cmd="",
                       initial_budget=0,
                       post_initial_cmd="",
                       post_mutant_cmd="",
                       status_cmd="",
                       order=1):
     executable_code = mutate.get_code(executable)
@@ -84,33 +86,48 @@
             silent_run_with_timeout(initial_fuzz_cmd, initial_budget)
             if status_cmd != "":
                 print("INITIAL STATUS:")
                 subprocess.call(status_cmd, shell=True)
             if post_initial_cmd != "":
                 subprocess.call(post_initial_cmd, shell=True)
 
+        if reachability_check_cmd != "":
+            reachability_filename = "/tmp/reachability_executable"
+        else:
+            reachability_filename = ""
         while ((time.time() - start_fuzz) - initial_budget) < (budget * fraction_mutant):
             print("=" * 10,
                   datetime.utcfromtimestamp(time.time()).strftime('%Y-%m-%d %H:%M:%S'),
                   "=" * 10)
             print(round(time.time() - start_fuzz, 2),
                   "ELAPSED: GENERATING MUTANT #" + str(mutant_no))
             mutant_no += 1
             # make a new mutant of the executable; rename avoids hitting a busy executable
-            mutate.mutate_from(executable_code, executable_jumps, "/tmp/new_executable", order=order)
-            os.rename("/tmp/new_executable", executable)
-            subprocess.check_call(['chmod', '+x', executable])
+            mutate.mutate_from(executable_code, executable_jumps, "/tmp/new_executable", order=order,
+                               reachability_filename=reachability_filename)
             mutant_ok = True
-            if prune_mutant_cmd != "":
-                print("CHECKING MUTANT...")
-                r = silent_run_with_timeout(prune_mutant_cmd, prune_mutant_timeout)
-                if r != 0:
-                    print("CHECK FAILED WITH RETURN CODE", r)
+            if reachability_check_cmd != "":
+                print("CHECKING REACHABILITY")
+                os.rename(reachability_filename, executable)
+                subprocess.check_call(['chmod', '+x', executable])
+                r = silent_run_with_timeout(reachability_check_cmd, reachability_check_timeout)
+                restore_executable(executable, executable_code)
+                if r == 0:
+                    print("MUTANT IS NOT REACHABLE (RETURN CODE 0)")
                     mutant_ok = False
             if mutant_ok:
+                os.rename("/tmp/new_executable", executable)
+                subprocess.check_call(['chmod', '+x', executable])
+                if prune_mutant_cmd != "":
+                    print("PRUNING MUTANT...")
+                    r = silent_run_with_timeout(prune_mutant_cmd, prune_mutant_timeout)
+                    if r != 0:
+                        print("CHECK FAILED WITH RETURN CODE", r)
+                        mutant_ok = False
+            if mutant_ok:
                 print("FUZZING MUTANT...")
                 start_run = time.time()
                 silent_run_with_timeout(fuzzer_cmd, time_per_mutant)
                 print("FINISHED FUZZING IN", round(time.time() - start_run, 2), "SECONDS")
                 if post_mutant_cmd != "":
                     subprocess.call(post_mutant_cmd, shell=True)
                 if status_cmd != "":
```

## muttfuzz/mutate.py

```diff
@@ -1,20 +1,17 @@
 import random
 import subprocess
 
-from muttfuzz import fuzzutil
-
 JUMP_OPCODES = ["je", "jne", "jl", "jle", "jg", "jge"]
 SHORT_JUMPS = list(map(bytes.fromhex, ["74", "75", "7C", "7D", "7E", "7F", "EB"]))
 SHORT_NAMES = dict(zip(SHORT_JUMPS, ["je", "jne", "jl", "jge", "jle", "jg", "jmp"]))
 NEAR_JUMPS = list(map(bytes.fromhex, ["0F 84", "0F 85", "0F 8C", "0F 8D", "0F 8E", "0F 8F", "90 E9"]))
 NEAR_NAMES = dict(zip(NEAR_JUMPS, ["je", "jne", "jl", "jge", "jle", "jg", "jmp"]))
 
 NOP = bytes.fromhex("90") # Needed to erase a jump
-
 HALT = bytes.fromhex("F4") # Needed for reachability check
 
 # known markers for fuzzer/compiler injected instrumentation/etc.
 INST_SET = ["__afl", "__asan", "__ubsan", "__sanitizer", "__lsan", "__sancov", "AFL_"]
 INST_SET.extend(["DeepState", "deepstate"])
 
 def get_jumps(filename, only_mutate=[], avoid_mutating=[]):
@@ -97,30 +94,35 @@
         print("CHANGING TO NOPS")
     return (loc, changed)
 
 def get_code(filename):
     with open(filename, "rb") as f:
         return bytearray(f.read())
 
-def check_reachable(code, loc, reachability_check):
-    new_code[loc] = HALT
-    # need code to actually generate and change
-    return True
-
 def mutant_from(code, jumps, order=1):
     new_code = bytearray(code)
+    reach_code = bytearray(code)
     for i in range(order): # allows higher-order mutants, though can undo mutations
         (loc, new_data) = pick_and_change(jumps)
+        reach_code[loc] = HALT
         for offset in range(0, len(new_data)):
             new_code[loc + offset] = new_data[offset]
-    return new_code
+    return (new_code, reach_code)
 
 def mutant(filename, order=1, avoid_mutating=[]):
     return mutant_from(get_code(filename), get_jumps(filename, avoid_mutating), order=order)
 
-def mutate_from(code, jumps, new_filename, order=1, reachability_check=""):
+def mutate_from(code, jumps, new_filename, order=1, reachability_filename=""):
+    (m, r) = mutant_from(code, jumps, order=order)
     with open(new_filename, 'wb') as f:
-        f.write(mutant_from(code, jumps, order=order))
+        f.write(m)
+    if reachability_filename != "":
+        with open(reachability_filename, "wb") as f:
+            f.write(r)
 
-def mutate(filename, new_filename, order=1, avoid_mutating=[], reachability_check=""):
+def mutate(filename, new_filename, order=1, avoid_mutating=[], reachability_filename=""):
+    (m, r) = mutant(filename, order=order, avoid_mutating=avoid_mutating)
     with open(new_filename, "wb") as f:
-        f.write(mutant(filename, order=order, avoid_mutating=avoid_mutating))
+        f.write(m)
+    if reachability_filename != "":
+        with open(reachability_filename, "wb") as f:
+            f.write(r)
```

## Comparing `muttfuzz-0.7.3.dist-info/METADATA` & `muttfuzz-0.7.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.7.3
+Version: 0.7.4
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

## Comparing `muttfuzz-0.7.3.dist-info/RECORD` & `muttfuzz-0.7.4.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-muttfuzz/fuzz.py,sha256=3597RhXkUl4GQuIo5BFH-IHehOBqxqS5PYqjm1X21QU,4104
-muttfuzz/fuzzutil.py,sha256=dsIbVqP_XyZao6orvVPM2stGQU9bBM0CB-8M3CkzDpI,8432
-muttfuzz/mutate.py,sha256=S6NaFqlGzXUFR7f8ole2211QspBKkiEbDyzrCVPzhAc,4978
-muttfuzz-0.7.3.dist-info/METADATA,sha256=MtkPaXFwiFXJ7UUyqZgGOztOryeoLVrIdBJUjLb-NUo,4589
-muttfuzz-0.7.3.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-muttfuzz-0.7.3.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
-muttfuzz-0.7.3.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
-muttfuzz-0.7.3.dist-info/RECORD,,
+muttfuzz/fuzz.py,sha256=_9UOO9giNQiUNWAbJDQO0LB8jgkbyqf8lZ04ck-hZGI,4559
+muttfuzz/fuzzutil.py,sha256=FGvQNwfclsHPK5Wlp904npeuShPy_KOwUbezcXSNh4E,9345
+muttfuzz/mutate.py,sha256=RA6iQJzK5ruTwoTzaWRRO6zuhBiB_b4HJfkC5gf9z0w,5142
+muttfuzz-0.7.4.dist-info/METADATA,sha256=f6JwBShAGK5P4urXfbLI6nx2w-pXMvWppJ6gRHv-Cyo,4589
+muttfuzz-0.7.4.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+muttfuzz-0.7.4.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
+muttfuzz-0.7.4.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
+muttfuzz-0.7.4.dist-info/RECORD,,
```

