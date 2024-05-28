# Comparing `tmp/apngasm_python-1.3.0.tar.gz` & `tmp/apngasm_python-1.3.1-cp312-abi3-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apngasm_python-1.3.0.tar", last modified: Fri May 24 02:41:40 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

