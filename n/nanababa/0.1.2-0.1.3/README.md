# Comparing `tmp/nanababa-0.1.2.tar.gz` & `tmp/nanababa-0.1.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanababa-0.1.2.tar", last modified: Tue May 28 03:47:15 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

