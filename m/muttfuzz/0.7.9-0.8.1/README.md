# Comparing `tmp/muttfuzz-0.7.9-py3-none-any.whl.zip` & `tmp/muttfuzz-0.8.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8878 bytes, number of entries: 8
--rw-r--r--  2.0 unx     4755 b- defN 24-May-28 11:08 muttfuzz/fuzz.py
--rw-r--r--  2.0 unx     9665 b- defN 24-May-28 11:08 muttfuzz/fuzzutil.py
+Zip file size: 9705 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     4944 b- defN 24-May-28 17:16 muttfuzz/fuzz.py
+-rw-r--r--  2.0 unx    10417 b- defN 24-May-28 17:16 muttfuzz/fuzzutil.py
 -rw-r--r--  2.0 unx     5721 b- defN 24-May-28 10:34 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     4589 b- defN 24-May-28 11:08 muttfuzz-0.7.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-28 11:08 muttfuzz-0.7.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-May-28 11:08 muttfuzz-0.7.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-28 11:08 muttfuzz-0.7.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      622 b- defN 24-May-28 11:08 muttfuzz-0.7.9.dist-info/RECORD
-8 files, 25514 bytes uncompressed, 7794 bytes compressed:  69.5%
+-rw-r--r--  2.0 unx     6137 b- defN 24-May-28 17:16 muttfuzz-0.8.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 17:16 muttfuzz-0.8.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-May-28 17:16 muttfuzz-0.8.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-28 17:16 muttfuzz-0.8.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      623 b- defN 24-May-28 17:16 muttfuzz-0.8.1.dist-info/RECORD
+8 files, 28004 bytes uncompressed, 8621 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.7.9.dist-info/METADATA
+Filename: muttfuzz-0.8.1.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.7.9.dist-info/WHEEL
+Filename: muttfuzz-0.8.1.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.7.9.dist-info/entry_points.txt
+Filename: muttfuzz-0.8.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.7.9.dist-info/top_level.txt
+Filename: muttfuzz-0.8.1.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.7.9.dist-info/RECORD
+Filename: muttfuzz-0.8.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/fuzz.py

```diff
@@ -35,18 +35,20 @@
                         help='how long to run initial fuzzing, in seconds (default 60)')
     parser.add_argument('--post_initial_cmd', type=str, default="",
                         help='command to run after initial fuzzing')
     parser.add_argument('--post_mutant_cmd', type=str, default="",
                         help='command to run after each mutant (e.g., fuzz of original)')
     parser.add_argument('--post_mutant_timeout', type=float, default=2.0,
                         help='timeout for post-mutant command')
-    parser.add_argument('--order', type=int, default=1,
-                        help='mutation order (default 1)')
     parser.add_argument('--status_cmd', type=str, default="",
                         help='command to execute to show fuzzing stats')
+    parser.add_argument('--order', type=int, default=1,
+                        help='mutation order (default 1)')
+    parser.add_argument('-s', '--score', action='store_true',
+                        help="compute a mutation score, instead of fuzzing.")
 
     parsed_args = parser.parse_args(sys.argv[1:])
     return (parsed_args, parser)
 
 
 def make_config(pargs):
     """
@@ -78,15 +80,16 @@
                                    config.prune_mutant_timeout,
                                    config.initial_fuzz_cmd,
                                    config.initial_budget,
                                    config.post_initial_cmd,
                                    config.post_mutant_cmd,
                                    config.post_mutant_timeout,
                                    config.status_cmd,
-                                   config.order)
+                                   config.order,
+                                   config.score)
     except IndexError:
         print("Target binary seems to have no jumps, so mutation will not do anything!")
 
 
 
 if __name__ == "__main__":
     main()
```

## muttfuzz/fuzzutil.py

```diff
@@ -69,15 +69,16 @@
                       prune_mutant_timeout=2.0,
                       initial_fuzz_cmd="",
                       initial_budget=0,
                       post_initial_cmd="",
                       post_mutant_cmd="",
                       post_mutant_timeout=2.0,
                       status_cmd="",
-                      order=1):
+                      order=1,
+                      score=False):
     executable_code = mutate.get_code(executable)
     executable_jumps = mutate.get_jumps(executable, only_mutate, avoid_mutating)
     start_fuzz = time.time()
     mutant_no = 1
     try:
         if initial_fuzz_cmd != "":
             print("=" * 10,
@@ -91,14 +92,17 @@
             if post_initial_cmd != "":
                 subprocess.call(post_initial_cmd, shell=True)
 
         if reachability_check_cmd != "":
             reachability_filename = "/tmp/reachability_executable"
         else:
             reachability_filename = ""
+        if score:
+            mutants_run = 0.0
+            mutants_killed = 0.0
         while ((time.time() - start_fuzz) - initial_budget) < (budget * fraction_mutant):
             print("=" * 10,
                   datetime.utcfromtimestamp(time.time()).strftime('%Y-%m-%d %H:%M:%S'),
                   "=" * 10)
             print(round(time.time() - start_fuzz, 2),
                   "ELAPSED: GENERATING MUTANT #" + str(mutant_no))
             mutant_no += 1
@@ -123,15 +127,23 @@
                     r = silent_run_with_timeout(prune_mutant_cmd, prune_mutant_timeout)
                     if r != 0:
                         print("CHECK FAILED WITH RETURN CODE", r)
                         mutant_ok = False
             if mutant_ok:
                 print("FUZZING MUTANT...")
                 start_run = time.time()
-                silent_run_with_timeout(fuzzer_cmd, time_per_mutant)
+                r = silent_run_with_timeout(fuzzer_cmd, time_per_mutant)
+                if score:
+                    mutants_run += 1
+                    if (r != 0):
+                        mutants_killed += 1
+                        print ("** MUTANT KILLED **")
+                    else:
+                        print ("** MUTANT NOT KILLED **")
+                    print ("RUNNING MUTATION SCORE ON", int(mutants_run), "MUTANTS:", str(round((mutants_killed / mutants_run)*100.0, 2)) + "%")
                 print("FINISHED FUZZING IN", round(time.time() - start_run, 2), "SECONDS")
                 if post_mutant_cmd != "":
                     restore_executable(executable, executable_code) # Might need original for post
                     print("RUNNING POST-MUTANT COMMAND")
                     silent_run_with_timeout(post_mutant_cmd, post_mutant_timeout)
                 if status_cmd != "":
                     restore_executable(executable, executable_code) # Might need for status
@@ -142,14 +154,17 @@
         print(round(time.time() - start_fuzz, 2), "ELAPSED: STARTING FINAL FUZZ")
         restore_executable(executable, executable_code)
         silent_run_with_timeout(fuzzer_cmd, budget - (time.time() - start_fuzz))
         print("COMPLETED ALL FUZZING AFTER", round(time.time() - start_fuzz, 2), "SECONDS")
         if status_cmd != "":
             print("FINAL STATUS:")
             subprocess.call(status_cmd, shell=True)
+        if score:
+            print ("FINAL MUTATION SCORE OVER", int(mutants_run), "MUTANTS:", str(round((mutants_killed / mutants_run)*100.0, 2)) + "%")
+            print ("NOTE:  MUTANTS MAY BE REDUNDANT")
     finally:
         # always restore the original binary!
         restore_executable(executable, executable_code)
 
 # Currently this is not used, and is not updated to match all changes to the API!
 # It should work, but it does not support everything the command line does
 def fuzz_with_mutants_via_function(fuzzer_fn, executable, budget,
```

## Comparing `muttfuzz-0.7.9.dist-info/METADATA` & `muttfuzz-0.8.1.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.7.9
+Version: 0.8.1
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
@@ -17,15 +17,15 @@
 
 ---------------------------------
 
 **FAQ**
 
 **Q**:  Is this a mutation testing tool?
 
-**A**:  No.  MuttFuzz is only mutating your code in order to fuzz it better.  You don't need to care about the mutants, you'll never see them.  Coverage and bugs will be for your fuzzed program.
+**A**:  No.  MuttFuzz is only mutating your code in order to fuzz it better.  You don't need to care about the mutants, you'll never see them.  Coverage and bugs will be for your fuzzed program.  However, MuttFuzz does provide a mode in which it can give a quick-and-dirty mutation score estimate for a program.  See below.
 
 **Q**: What fuzzing algorithm does MuttFuzz use?
 
 **A**: MuttFuzz doesn't use a fuzzing algorithm.  MuttFuzz is a *meta-fuzzer*.  This means you tell MuttFuzz what fuzzer you're using (and how you call it), and where your executable is, and MuttFuzz will orchestrate a fuzzing campaign, doing some behind-the-scenes work on the fuzzed executable that is likely to improve the effectiveness of that fuzzing.  MuttFuzz should work with most popular fuzzing tools.
 
 **Q**: What are major limitations of MuttFuzz?
 
@@ -44,32 +44,37 @@
 should do the trick.  Right now, there are no serious dependencies.
 
 **Q: How do I use MuttFuzz?** 
 
 **A**: Let's say you want to use AFL to fuzz a program whose compiled and AFL-instrumented executable is named `target` and which takes its input from `stdin`:
 
 ~~~
-export AFL_SKIP_CRASHES=TRUE
 muttfuzz "afl-fuzz -i- -o fuzz_target -d ./target @@" target --initial_fuzz_cmd "afl-fuzz -i in -o fuzz_target -d ./target @@" --initial_budget 1800 --budget 86400 --post_mutant_cmd "cp fuzz_target/crashes.*/id* fuzz_target/queue/; rm -rf fuzz_target/crashes.*"
 ~~~
 
-That will 1) create a directory `fuzz_target` and use AFL to fuzz `target` for 30 minutes, then 2) switch to fuzzing a series of mutants of `target` for five minutes each before 3) finally switching back to fuzzing using AFL on the original `target`.  The total time spent fuzzing will be 24 hours, and MuttFuzz will spend half that time fuzzing mutants.  The `--post_mutant_cmd` and `AFL_SKIP_CRASHES` setting handles the fact that things that crash some mutants may not crash the real `target` and vice versa.  When you're done fuzzing, you'll want to look in both `crashes` and `queue` for possible crashing inputs for `target`, due to the same issue.
+That will 1) create a directory `fuzz_target` and use AFL to fuzz `target` for 30 minutes, then 2) switch to fuzzing a series of mutants of `target` for five minutes each before 3) finally switching back to fuzzing using AFL on the original `target`.  The total time spent fuzzing will be 24 hours, and MuttFuzz will spend half that time fuzzing mutants.  The `--post_mutant_cmd` handles the fact that things that crash some mutants may not crash the real `target`.   AFL++ removes crashes that don't crash the current version of a program, but we want them in the queue to explore.   When you're done fuzzing, you'll want to look in both `crashes` and `queue` for possible crashing inputs for `target`, due to the same issue.
+
+You can likely improve your fuzzing if you can provide MuttFuzz with commands to 1) throw out mutants that aren't even reachable in the current corpus and 2) throw out mutants that already trigger a crash.  The first case is likely to be almost always helpful; the second is less certain.  These effects are achieved by, respectively, the `--reachability_check_cmd` and `--prune_mutants_cmd` arguments.  Both should tell MuttFuzz how to execute the current corpus, with this being done in such a way that if there is a crash, the output is a non-zero return value from the command.  In the reachability case, non-zero means the mutant is reached (we replace the mutant with a HALT) and in the pruning case (which uses the actual mutant) non-zero means the mutant induces crashes and should be skipped.
 
 ```muttfuzz --help``` will give details on other options.  One nice thing is to print out status (e.g., cat the AFL stats file, or ls | wc -l on crashes/queue) after each fuzzing run.
 
 This example shows how to use MuttFuzz with AFL (or AFLplusplus) but using it with libFuzzer or Honggfuzz should be approximately as easy, or easier.
 
 **Q**: How good is MuttFuzz?
 
 **A**: We're not sure yet, experiments are pending.  We know that a source-based variant of the same technique, somewhat less tuned, outperformed AFLplusplus on FuzzBench, so we're optimistic that this is both easier to use and even more effective than that.  In our limited experiments thus far, it is dramatically improving fuzzing a toy benchmark using AFL, much more than the source-based approach did.
 
 **Q**: Why is fuzzing mutants helpful?
 
 **A**: For more information on that, and on the source-based version of this idea, see [our paper in submission to ACM TOSEM, the final version of our FUZZING'22 registered report](https://github.com/agroce/fuzzing22report/blob/master/tosem/currentdraft.pdf).  Long story short, we speculate that some mutants remove common barriers to fuzzing, and/or allow fuzzing to find branches "non-chronologically."
 
+**Q**: Hey, you said I could use MuttFuzz to estimate a mutation score?
+
+**A**: Yes, just use a fuzzing command that does nothing but check a mutant for detection (something like the commands used for reachability and pruning) that returns non-zero on detected mutants, and add the `--score` option.  Note that MuttFuzz uses a peculiar and biased set of mutation operators, and may score the same mutant multiple times, so take this value with a grain of salt.  You can also have the fuzzing command do some actual fuzzing, and then check for detection after the fuzzing.
+
 **Q**: Why "MuttFuzz"?
 
 **A**: When I (Alex) created the repo, I made a typo, but I liked it.  Certainly memorable compared to "mutfuzz" for "mutant fuzzer".
 
 -------------------------------
 
 Thanks to: Peter Goodman @ Trail of Bits, Kush Jain, and Richard Hipp.
```

## Comparing `muttfuzz-0.7.9.dist-info/RECORD` & `muttfuzz-0.8.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-muttfuzz/fuzz.py,sha256=k0LrPfj2xcgRXVFOUfCZjFoQioiLJMQg6X5o76_tS0o,4755
-muttfuzz/fuzzutil.py,sha256=GZ5Aq0TAwCObwb-LBkw_eMxW6rIBuUht6tTYuSlx7Hs,9665
+muttfuzz/fuzz.py,sha256=cis3_IqePjHxFGhsi7RXmHdpYVrZqxeJ3TUyZ_HJ4x8,4944
+muttfuzz/fuzzutil.py,sha256=P1KHD29PkJZpMhdYHLeyhNYZs2-68rYui441vsjAPHs,10417
 muttfuzz/mutate.py,sha256=EUFlHVAhzW9FSBuaNz-nHtcp_CgGgQCOyLyzQEyHPxQ,5721
-muttfuzz-0.7.9.dist-info/METADATA,sha256=WRXytJrSrsw8CXAUxhW_RqD6Oi-USVatvotA_qaJIxs,4589
-muttfuzz-0.7.9.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-muttfuzz-0.7.9.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
-muttfuzz-0.7.9.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
-muttfuzz-0.7.9.dist-info/RECORD,,
+muttfuzz-0.8.1.dist-info/METADATA,sha256=2CYzTAjiJ5b2bi5a4Ll4mU3cn8mRAL8o3xZ3j5AsxPM,6137
+muttfuzz-0.8.1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+muttfuzz-0.8.1.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
+muttfuzz-0.8.1.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
+muttfuzz-0.8.1.dist-info/RECORD,,
```

