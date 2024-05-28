# Comparing `tmp/ptinsearcher-1.0.8.tar.gz` & `tmp/ptinsearcher-1.0.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptinsearcher-1.0.8.tar", last modified: Tue May  7 15:09:47 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

