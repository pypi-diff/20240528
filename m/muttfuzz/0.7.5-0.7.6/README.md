# Comparing `tmp/muttfuzz-0.7.5-py3-none-any.whl.zip` & `tmp/muttfuzz-0.7.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8681 bytes, number of entries: 8
+Zip file size: 8687 bytes, number of entries: 8
 -rw-r--r--  2.0 unx     4559 b- defN 24-May-28 03:37 muttfuzz/fuzz.py
--rw-r--r--  2.0 unx     9345 b- defN 24-May-28 03:37 muttfuzz/fuzzutil.py
+-rw-r--r--  2.0 unx     9353 b- defN 24-May-28 03:44 muttfuzz/fuzzutil.py
 -rw-r--r--  2.0 unx     5145 b- defN 24-May-28 03:40 muttfuzz/mutate.py
--rw-r--r--  2.0 unx     4589 b- defN 24-May-28 03:40 muttfuzz-0.7.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-28 03:40 muttfuzz-0.7.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       61 b- defN 24-May-28 03:40 muttfuzz-0.7.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-28 03:40 muttfuzz-0.7.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      622 b- defN 24-May-28 03:40 muttfuzz-0.7.5.dist-info/RECORD
-8 files, 24422 bytes uncompressed, 7597 bytes compressed:  68.9%
+-rw-r--r--  2.0 unx     4589 b- defN 24-May-28 03:44 muttfuzz-0.7.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 03:44 muttfuzz-0.7.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       61 b- defN 24-May-28 03:44 muttfuzz-0.7.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-28 03:44 muttfuzz-0.7.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      622 b- defN 24-May-28 03:44 muttfuzz-0.7.6.dist-info/RECORD
+8 files, 24430 bytes uncompressed, 7603 bytes compressed:  68.9%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: muttfuzz/fuzzutil.py
 Comment: 
 
 Filename: muttfuzz/mutate.py
 Comment: 
 
-Filename: muttfuzz-0.7.5.dist-info/METADATA
+Filename: muttfuzz-0.7.6.dist-info/METADATA
 Comment: 
 
-Filename: muttfuzz-0.7.5.dist-info/WHEEL
+Filename: muttfuzz-0.7.6.dist-info/WHEEL
 Comment: 
 
-Filename: muttfuzz-0.7.5.dist-info/entry_points.txt
+Filename: muttfuzz-0.7.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: muttfuzz-0.7.5.dist-info/top_level.txt
+Filename: muttfuzz-0.7.6.dist-info/top_level.txt
 Comment: 
 
-Filename: muttfuzz-0.7.5.dist-info/RECORD
+Filename: muttfuzz-0.7.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## muttfuzz/fuzzutil.py

```diff
@@ -25,17 +25,17 @@
         yield
     finally:
         signal.alarm(0)
 
 
 def restore_executable(executable, executable_code):
     # We do this because it could still be busy if fuzzer hasn't shut down yet
-    with open("/tmp/new_executable", 'wb') as f:
+    with open("/tmp/restore_executable", 'wb') as f:
         f.write(executable_code)
-    os.rename("/tmp/new_executable", executable)
+    os.rename("/tmp/restore_executable", executable)
     subprocess.check_call(['chmod', '+x', executable])
 
 
 def silent_run_with_timeout(cmd, timeout):
     dnull = open(os.devnull, 'w')
     start_P = time.time()
     try:
```

## Comparing `muttfuzz-0.7.5.dist-info/METADATA` & `muttfuzz-0.7.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muttfuzz
-Version: 0.7.5
+Version: 0.7.6
 Summary: Fuzzing with mutants
 Home-page: https://github.com/agroce/muttfuzz
 License: MIT
 Keywords: fuzzing mutation
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

## Comparing `muttfuzz-0.7.5.dist-info/RECORD` & `muttfuzz-0.7.6.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 muttfuzz/fuzz.py,sha256=_9UOO9giNQiUNWAbJDQO0LB8jgkbyqf8lZ04ck-hZGI,4559
-muttfuzz/fuzzutil.py,sha256=FGvQNwfclsHPK5Wlp904npeuShPy_KOwUbezcXSNh4E,9345
+muttfuzz/fuzzutil.py,sha256=HM9C3dUws1ELRHVpe4hd1cRANvS15oQk4rfszpLAZB8,9353
 muttfuzz/mutate.py,sha256=ctqTDrYlWyCDB6xHCAb7C5HBzLipxgzzlj_pY79Et88,5145
-muttfuzz-0.7.5.dist-info/METADATA,sha256=ySUo8NQlWHlkOQBZq5lulG241SMk0P8DhCy_y5_KS34,4589
-muttfuzz-0.7.5.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-muttfuzz-0.7.5.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
-muttfuzz-0.7.5.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
-muttfuzz-0.7.5.dist-info/RECORD,,
+muttfuzz-0.7.6.dist-info/METADATA,sha256=JFCRiomLFIjd_qGE5EJVUZRVMLHZo1KdwQTE6vujI04,4589
+muttfuzz-0.7.6.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+muttfuzz-0.7.6.dist-info/entry_points.txt,sha256=o_y9rXeBbjEVGg-hChmZuRg-7JHOw70FtneWQOtn9ls,61
+muttfuzz-0.7.6.dist-info/top_level.txt,sha256=aUyZ-c9pAiqGuLfuoiIX_fXyaA__FTsdwtVUADVd9Gg,9
+muttfuzz-0.7.6.dist-info/RECORD,,
```

