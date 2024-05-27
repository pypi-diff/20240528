# Comparing `tmp/infisical_python-2.2.2.tar.gz` & `tmp/infisical_python-2.2.3-cp39-cp39-macosx_10_12_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

