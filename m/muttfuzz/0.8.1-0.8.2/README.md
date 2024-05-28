# Comparing `tmp/muttfuzz-0.8.1-py3-none-any.whl.zip` & `tmp/muttfuzz-0.8.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9705 bytes, number of entries: 8
+Zip file size: 10036 bytes, number of entries: 8
 -rw-r--r--  2.0 unx     4944 b- defN 24-May-28 17:16 muttfuzz/fuzz.py
--rw-r--r--  2.0 unx    10417 b- defN 24-May-28 17:16 muttfuzz/fuzzutil.py
+-rw-r--r--  2.0 unx    11128 b- defN 24-May-28 17:49 muttfuzz/fuzzutil.py
 -rw-r--r--  2.0 unx     5721 b- defN 24-May-28 10:34 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     6137 b- defN 24-May-28 17:16 muttfuzz-0.8.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-28 17:16 muttfuzz-0.8.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-May-28 17:16 muttfuzz-0.8.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-28 17:16 muttfuzz-0.8.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      623 b- defN 24-May-28 17:16 muttfuzz-0.8.1.dist-info/RECORD
-8 files, 28004 bytes uncompressed, 8621 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx     6714 b- defN 24-May-28 17:49 muttfuzz-0.8.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 17:49 muttfuzz-0.8.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-May-28 17:49 muttfuzz-0.8.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-28 17:49 muttfuzz-0.8.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      623 b- defN 24-May-28 17:49 muttfuzz-0.8.2.dist-info/RECORD
+8 files, 29292 bytes uncompressed, 8952 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.8.1.dist-info/METADATA
+Filename: muttfuzz-0.8.2.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.8.1.dist-info/WHEEL
+Filename: muttfuzz-0.8.2.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.8.1.dist-info/entry_points.txt
+Filename: muttfuzz-0.8.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.8.1.dist-info/top_level.txt
+Filename: muttfuzz-0.8.2.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.8.1.dist-info/RECORD
+Filename: muttfuzz-0.8.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/fuzzutil.py

```diff
@@ -90,39 +90,47 @@
                 print("INITIAL STATUS:")
                 subprocess.call(status_cmd, shell=True)
             if post_initial_cmd != "":
                 subprocess.call(post_initial_cmd, shell=True)
 
         if reachability_check_cmd != "":
             reachability_filename = "/tmp/reachability_executable"
+            reachability_checks = 0.0
+            reachability_hits = 0.0
         else:
             reachability_filename = ""
         if score:
             mutants_run = 0.0
             mutants_killed = 0.0
+            fraction_mutant = 1.0 # No final fuzz for mutation score estimation!
         while ((time.time() - start_fuzz) - initial_budget) < (budget * fraction_mutant):
             print("=" * 10,
                   datetime.utcfromtimestamp(time.time()).strftime('%Y-%m-%d %H:%M:%S'),
                   "=" * 10)
             print(round(time.time() - start_fuzz, 2),
                   "ELAPSED: GENERATING MUTANT #" + str(mutant_no))
             mutant_no += 1
             # make a new mutant of the executable; rename avoids hitting a busy executable
             mutate.mutate_from(executable_code, executable_jumps, "/tmp/new_executable", order=order,
                                reachability_filename=reachability_filename)
             mutant_ok = True
             if reachability_check_cmd != "":
                 print("CHECKING REACHABILITY")
+                reachability_checks += 1.0
                 os.rename(reachability_filename, executable)
                 subprocess.check_call(['chmod', '+x', executable])
                 r = silent_run_with_timeout(reachability_check_cmd, reachability_check_timeout)
                 restore_executable(executable, executable_code)
                 if r == 0:
                     print("MUTANT IS NOT REACHABLE (RETURN CODE 0)")
                     mutant_ok = False
+                else:
+                    reachability_hits += 1.0
+                print ("RUNNING COVERAGE ESTIMATE OVER", int(mutants_run), "MUTANTS:",
+                       str(round((reachability_hits / reachability_checks) * 100.0, 2)) + "%")
             if mutant_ok:
                 os.rename("/tmp/new_executable", executable)
                 subprocess.check_call(['chmod', '+x', executable])
                 if prune_mutant_cmd != "":
                     print("PRUNING MUTANT...")
                     r = silent_run_with_timeout(prune_mutant_cmd, prune_mutant_timeout)
                     if r != 0:
@@ -135,15 +143,16 @@
                 if score:
                     mutants_run += 1
                     if (r != 0):
                         mutants_killed += 1
                         print ("** MUTANT KILLED **")
                     else:
                         print ("** MUTANT NOT KILLED **")
-                    print ("RUNNING MUTATION SCORE ON", int(mutants_run), "MUTANTS:", str(round((mutants_killed / mutants_run)*100.0, 2)) + "%")
+                    print ("RUNNING MUTATION SCORE ON", int(mutants_run), "MUTANTS:",
+                           str(round((mutants_killed / mutants_run) * 100.0, 2)) + "%")
                 print("FINISHED FUZZING IN", round(time.time() - start_run, 2), "SECONDS")
                 if post_mutant_cmd != "":
                     restore_executable(executable, executable_code) # Might need original for post
                     print("RUNNING POST-MUTANT COMMAND")
                     silent_run_with_timeout(post_mutant_cmd, post_mutant_timeout)
                 if status_cmd != "":
                     restore_executable(executable, executable_code) # Might need for status
@@ -154,16 +163,20 @@
         print(round(time.time() - start_fuzz, 2), "ELAPSED: STARTING FINAL FUZZ")
         restore_executable(executable, executable_code)
         silent_run_with_timeout(fuzzer_cmd, budget - (time.time() - start_fuzz))
         print("COMPLETED ALL FUZZING AFTER", round(time.time() - start_fuzz, 2), "SECONDS")
         if status_cmd != "":
             print("FINAL STATUS:")
             subprocess.call(status_cmd, shell=True)
+        if reachability_check_cmd != "":
+            print ("FINAL COVERAGE ESTIMATE OVER", int(mutants_run), "MUTANTS:",
+                   str(round((reachability_hits / reachability_checks) * 100.0, 2)) + "%")
         if score:
-            print ("FINAL MUTATION SCORE OVER", int(mutants_run), "MUTANTS:", str(round((mutants_killed / mutants_run)*100.0, 2)) + "%")
+            print ("FINAL MUTATION SCORE OVER", int(mutants_run), "MUTANTS:",
+                    str(round((mutants_killed / mutants_run) * 100.0, 2)) + "%")
             print ("NOTE:  MUTANTS MAY BE REDUNDANT")
     finally:
         # always restore the original binary!
         restore_executable(executable, executable_code)
 
 # Currently this is not used, and is not updated to match all changes to the API!
 # It should work, but it does not support everything the command line does
```

## Comparing `muttfuzz-0.8.1.dist-info/METADATA` & `muttfuzz-0.8.2.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.8.1
+Version: 0.8.2
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
@@ -67,14 +67,16 @@
 
 **A**: For more information on that, and on the source-based version of this idea, see [our paper in submission to ACM TOSEM, the final version of our FUZZING'22 registered report](https://github.com/agroce/fuzzing22report/blob/master/tosem/currentdraft.pdf).  Long story short, we speculate that some mutants remove common barriers to fuzzing, and/or allow fuzzing to find branches "non-chronologically."
 
 **Q**: Hey, you said I could use MuttFuzz to estimate a mutation score?
 
 **A**: Yes, just use a fuzzing command that does nothing but check a mutant for detection (something like the commands used for reachability and pruning) that returns non-zero on detected mutants, and add the `--score` option.  Note that MuttFuzz uses a peculiar and biased set of mutation operators, and may score the same mutant multiple times, so take this value with a grain of salt.  You can also have the fuzzing command do some actual fuzzing, and then check for detection after the fuzzing.
 
+Note that reachability and pruning work as usual here.  Pruning will seldom be needed, but there may be some notion of invalid mutants you want to use.  Reachability lets you compute  a score over mutants the corpus actually executes, which is usually more informative than including mutants not even executed.  The distinction is between "mutation score" and "covered mutation score" (see [this paper](https://agroce.github.io/issre23.pdf)).  Note that MuttFuzz, when a reachability check is included, always shows a running and final total of estimated coverage of mutants.
+
 **Q**: Why "MuttFuzz"?
 
 **A**: When I (Alex) created the repo, I made a typo, but I liked it.  Certainly memorable compared to "mutfuzz" for "mutant fuzzer".
 
 -------------------------------
 
 Thanks to: Peter Goodman @ Trail of Bits, Kush Jain, and Richard Hipp.
```

## Comparing `muttfuzz-0.8.1.dist-info/RECORD` & `muttfuzz-0.8.2.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 muttfuzz/fuzz.py,sha256=cis3_IqePjHxFGhsi7RXmHdpYVrZqxeJ3TUyZ_HJ4x8,4944
-muttfuzz/fuzzutil.py,sha256=P1KHD29PkJZpMhdYHLeyhNYZs2-68rYui441vsjAPHs,10417
+muttfuzz/fuzzutil.py,sha256=S7PaiD8Wxgxd614JftRmmbVFyzc87NROn034kpl3ERA,11128
 muttfuzz/mutate.py,sha256=EUFlHVAhzW9FSBuaNz-nHtcp_CgGgQCOyLyzQEyHPxQ,5721
-muttfuzz-0.8.1.dist-info/METADATA,sha256=2CYzTAjiJ5b2bi5a4Ll4mU3cn8mRAL8o3xZ3j5AsxPM,6137
-muttfuzz-0.8.1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-muttfuzz-0.8.1.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
-muttfuzz-0.8.1.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
-muttfuzz-0.8.1.dist-info/RECORD,,
+muttfuzz-0.8.2.dist-info/METADATA,sha256=aEfh2WNwnpmv7KHqXW8lDiaoJol0fpOaYQ0sylNdJn0,6714
+muttfuzz-0.8.2.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+muttfuzz-0.8.2.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
+muttfuzz-0.8.2.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
+muttfuzz-0.8.2.dist-info/RECORD,,
```

