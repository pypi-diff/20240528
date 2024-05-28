# Comparing `tmp/Yifengw-0.0.0.tar.gz` & `tmp/Yifengw-0.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Yifengw-0.0.0.tar", last modified: Tue May 28 08:28:52 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

