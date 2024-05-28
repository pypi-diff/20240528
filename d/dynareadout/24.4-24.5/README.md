# Comparing `tmp/dynareadout-24.4.tar.gz` & `tmp/dynareadout-24.5-pp39-pypy39_pp73-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynareadout-24.4.tar", last modified: Fri Apr 26 06:43:47 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

