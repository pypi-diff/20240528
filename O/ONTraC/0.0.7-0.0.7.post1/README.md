# Comparing `tmp/ontrac-0.0.7.tar.gz` & `tmp/ONTraC-0.0.7.post1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontrac-0.0.7.tar", last modified: Mon May 13 18:31:47 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

