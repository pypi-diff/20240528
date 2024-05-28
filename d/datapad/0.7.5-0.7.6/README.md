# Comparing `tmp/datapad-0.7.5.tar.gz` & `tmp/datapad-0.7.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapad-0.7.5.tar", last modified: Thu May 23 17:58:10 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

