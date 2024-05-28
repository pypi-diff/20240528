# Comparing `tmp/muttfuzz-0.6.9-py3-none-any.whl.zip` & `tmp/muttfuzz-0.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8237 bytes, number of entries: 8
--rw-r--r--  2.0 unx     4102 b- defN 24-May-25 14:56 muttfuzz/fuzz.py
--rw-r--r--  2.0 unx     8277 b- defN 24-May-25 14:43 muttfuzz/fuzzutil.py
--rw-r--r--  2.0 unx     4648 b- defN 24-May-25 14:43 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     4589 b- defN 24-May-25 14:56 muttfuzz-0.6.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-25 14:56 muttfuzz-0.6.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-May-25 14:56 muttfuzz-0.6.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-25 14:56 muttfuzz-0.6.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      622 b- defN 24-May-25 14:56 muttfuzz-0.6.9.dist-info/RECORD
-8 files, 22400 bytes uncompressed, 7153 bytes compressed:  68.1%
+Zip file size: 8456 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     4104 b- defN 24-May-25 14:57 muttfuzz/fuzz.py
+-rw-r--r--  2.0 unx     8432 b- defN 24-May-26 20:32 muttfuzz/fuzzutil.py
+-rw-r--r--  2.0 unx     4934 b- defN 24-May-28 02:31 muttfuzz/mutate.py
+-rw-r--r--  2.0 unx     4589 b- defN 24-May-28 02:32 muttfuzz-0.7.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 02:32 muttfuzz-0.7.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-May-28 02:32 muttfuzz-0.7.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-28 02:32 muttfuzz-0.7.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      622 b- defN 24-May-28 02:32 muttfuzz-0.7.0.dist-info/RECORD
+8 files, 22843 bytes uncompressed, 7372 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.6.9.dist-info/METADATA
+Filename: muttfuzz-0.7.0.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.6.9.dist-info/WHEEL
+Filename: muttfuzz-0.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.6.9.dist-info/entry_points.txt
+Filename: muttfuzz-0.7.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.6.9.dist-info/top_level.txt
+Filename: muttfuzz-0.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.6.9.dist-info/RECORD
+Filename: muttfuzz-0.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/fuzz.py

```diff
@@ -60,16 +60,16 @@
     config = make_config(parsed_args)
     try:
         fuzzutil.fuzz_with_mutants(config.fuzzer_cmd,
                                    config.executable,
                                    config.budget,
                                    config.time_per_mutant,
                                    config.fraction_mutant,
-                                   list(filter(None, config.only_mutate.replace(", ", ",").split(",")),
-                                   list(filter(None, config.avoid_mutating.replace(", ", ",").split(",")),
+                                   list(filter(None, config.only_mutate.replace(", ", ",").split(","))),
+                                   list(filter(None, config.avoid_mutating.replace(", ", ",").split(","))),
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
@@ -43,18 +43,21 @@
             P = subprocess.Popen(cmd, shell=True, preexec_fn=os.setsid,
                                  stdout=dnull, stderr=cmd_errors)
             while (P.poll() is None) and ((time.time() - start_P) < timeout):
                 time.sleep(min(0.5, timeout / 10.0)) # Allow for small timeouts
             if P.poll() is None:
                 os.killpg(os.getpgid(P.pid), signal.SIGTERM)
         with open("cmd_errors.txt", 'r') as cmd_errors:
-            cmd_errors_out = cmd_errors.read()
+            try:
+                cmd_errors_out = cmd_errors.read()
+            except:
+                cmd_errors_out = "ERROR READING OUTPUT"
         if len(cmd_errors_out) > 0:
-            print("ERRORS:")
-            print(cmd_errors_out)
+            print("OUTPUT (TRUNCATED TO LAST 20 LINES):")
+            print("\n".join(cmd_errors_out.split("\n")[-20:]))
     finally:
         if P.poll() is None:
             os.killpg(os.getpgid(P.pid), signal.SIGTERM)
     return P.returncode
 
 
 def fuzz_with_mutants(fuzzer_cmd, executable, budget, time_per_mutant, fraction_mutant,
```

## muttfuzz/mutate.py

```diff
@@ -1,16 +1,22 @@
 import random
 import subprocess
 
+import muttfuzz import fuzzutil
+
 JUMP_OPCODES = ["je", "jne", "jl", "jle", "jg", "jge"]
 SHORT_JUMPS = list(map(bytes.fromhex, ["74", "75", "7C", "7D", "7E", "7F", "EB"]))
 SHORT_NAMES = dict(zip(SHORT_JUMPS, ["je", "jne", "jl", "jge", "jle", "jg", "jmp"]))
 NEAR_JUMPS = list(map(bytes.fromhex, ["0F 84", "0F 85", "0F 8C", "0F 8D", "0F 8E", "0F 8F", "90 E9"]))
 NEAR_NAMES = dict(zip(NEAR_JUMPS, ["je", "jne", "jl", "jge", "jle", "jg", "jmp"]))
 
+NOP = bytes.fromhex("90") # Needed to erase a jump
+
+HALT = bytes.fromhex("F4") # Needed for reachability check
+
 # known markers for fuzzer/compiler injected instrumentation/etc.
 INST_SET = ["__afl", "__asan", "__ubsan", "__sanitizer", "__lsan", "__sancov", "AFL_"]
 INST_SET.extend(["DeepState", "deepstate"])
 
 def get_jumps(filename, only_mutate=[], avoid_mutating=[]):
     jumps = {}
 
@@ -60,51 +66,60 @@
                     jumps[loc] = (opcode, bytes.fromhex(fields[1]), section_name, line)
         except: # If we can't parse some line in the objdump, just skip it
             pass
 
     return jumps
 
 def different_jump(hexdata):
+    P_DC = 0.40 # P(Don't Care)
+    # Current approach is to change to "don't care" (take or avoid) 80% of time, mutate 20%
+    if (random.random() <= P_DC): # Just remove the jump by providing a NOP sled
+        return NOP * len(hexdata)
     if hexdata[0] == 15: # NEAR JUMP BYTE CHECK
-        # Have a high chance of just changing near JE and JNE to a forced JMP, "removing" a branch
-        if ((hexdata[1] == NEAR_JUMPS[0][1])  or (hexdata[1] == NEAR_JUMPS[1][1])) and (random.random() <= 0.75):
+        if random.random() <= P_DC:
             return NEAR_JUMPS[-1]
-        return random.choice(list(filter(lambda j: j[1] != hexdata[1], NEAR_JUMPS)))
+        return random.choice(list(filter(lambda j: j[1] != hexdata[1], NEAR_JUMPS[:-1])))
     else:
-        # Have a high chance of just changing short JE and JNE to a forced JMP, "removing" a branch
-        if ((hexdata[0] == SHORT_JUMPS[0][0])  or (hexdata[0] == SHORT_JUMPS[1][0])) and (random.random() <= 0.75):
+        if random.random() <= P_DC:
             return SHORT_JUMPS[-1]
-        return random.choice(list(filter(lambda j: j[0] != hexdata[0], SHORT_JUMPS)))
+        return random.choice(list(filter(lambda j: j[0] != hexdata[0], SHORT_JUMPS[:-1])))
 
 def pick_and_change(jumps):
     loc = random.choice(list(jumps.keys()))
     changed = different_jump(jumps[loc][1])
     print("MUTATING JUMP IN", jumps[loc][2], "WITH ORIGINAL OPCODE", jumps[loc][0])
     print("ORIGINAL CODE:", jumps[loc][3])
-    if changed in SHORT_NAMES:
+    if changed[0] == NOP:
+        print("CHANGING TO NOP")
+    elif changed in SHORT_NAMES:
         print("CHANGING TO", SHORT_NAMES[changed])
     else:
         print("CHANGING TO", NEAR_NAMES[changed])
     return (loc, changed)
 
 def get_code(filename):
     with open(filename, "rb") as f:
         return bytearray(f.read())
 
+def check_reachable(code, loc, reachability_check):
+    new_code[loc] = HALT
+    # need code to actually generate and change
+    return True
+
 def mutant_from(code, jumps, order=1):
     new_code = bytearray(code)
     for i in range(order): # allows higher-order mutants, though can undo mutations
         (loc, new_data) = pick_and_change(jumps)
         for offset in range(0, len(new_data)):
             new_code[loc + offset] = new_data[offset]
     return new_code
 
 def mutant(filename, order=1, avoid_mutating=[]):
     return mutant_from(get_code(filename), get_jumps(filename, avoid_mutating), order=order)
 
-def mutate_from(code, jumps, new_filename, order=1):
+def mutate_from(code, jumps, new_filename, order=1, reachability_check=""):
     with open(new_filename, 'wb') as f:
         f.write(mutant_from(code, jumps, order=order))
 
-def mutate(filename, new_filename, order=1, avoid_mutating=[]):
+def mutate(filename, new_filename, order=1, avoid_mutating=[], reachability_check=""):
     with open(new_filename, "wb") as f:
         f.write(mutant(filename, order=order, avoid_mutating=avoid_mutating))
```

## Comparing `muttfuzz-0.6.9.dist-info/METADATA` & `muttfuzz-0.7.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.6.9
+Version: 0.7.0
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

