# Comparing `tmp/pyobjc-framework-Symbols-10.2.tar.gz` & `tmp/pyobjc_framework_Symbols-10.3-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-Symbols-10.2.tar", last modified: Sat Mar  9 11:08:37 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
