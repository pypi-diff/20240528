# Comparing `tmp/chiral-client-0.3.0.tar.gz` & `tmp/chiral_client-0.3.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiral-client-0.3.0.tar", last modified: Fri Feb 23 08:00:14 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

