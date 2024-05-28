# Comparing `tmp/record3d-1.3.1-2.tar.gz` & `tmp/record3d-1.4-cp36-cp36m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "record3d-1.3.1.post2.tar", last modified: Thu Dec 15 08:17:48 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

