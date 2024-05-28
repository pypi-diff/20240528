# Comparing `tmp/uvx-2.1.0.tar.gz` & `tmp/uvx-2.2.0-py3-none-manylinux_2_34_aarch64.whl.zip`

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

