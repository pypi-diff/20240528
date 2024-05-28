# Comparing `tmp/pyobjc-framework-Cinematic-10.2.tar.gz` & `tmp/pyobjc_framework_Cinematic-10.3-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-Cinematic-10.2.tar", last modified: Sat Mar  9 10:40:27 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

