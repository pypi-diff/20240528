# Comparing `tmp/nfinance-0.4.3.tar.gz` & `tmp/nfinance-0.4.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nfinance-0.4.3.tar", last modified: Mon May 27 08:18:51 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

