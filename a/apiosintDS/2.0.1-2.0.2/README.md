# Comparing `tmp/apiosintDS-2.0.1.tar.gz` & `tmp/apiosintDS-2.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apiosintDS-2.0.1.tar", last modified: Sat Jul 15 10:16:41 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

