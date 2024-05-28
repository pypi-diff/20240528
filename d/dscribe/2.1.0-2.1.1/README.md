# Comparing `tmp/dscribe-2.1.0.tar.gz` & `tmp/dscribe-2.1.1-cp311-cp311-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dscribe-2.1.0.tar", last modified: Tue Sep  5 16:51:22 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

