# Comparing `tmp/ddtrace-2.9.0rc7.tar.gz` & `tmp/ddtrace-2.9.0rc8-cp310-cp310-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ddtrace-2.9.0rc7.tar", last modified: Tue May 14 14:06:39 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

