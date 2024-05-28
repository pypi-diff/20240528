# Comparing `tmp/xlextract-0.1.7.tar.gz` & `tmp/xlextract-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlextract-0.1.7.tar", max compression
+gzip compressed data, was "xlextract-0.1.8.tar", max compression
```

## Comparing `xlextract-0.1.7.tar` & `xlextract-0.1.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3990 2024-05-02 00:54:15.458342 xlextract-0.1.7/README.md
--rw-r--r--   0        0        0      392 2024-05-02 01:01:31.842086 xlextract-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4455 2024-05-02 01:00:37.101623 xlextract-0.1.7/xlextract/__init__.py
--rw-r--r--   0        0        0     1886 2024-05-02 01:00:47.081709 xlextract-0.1.7/xlextract/classes.py
--rw-r--r--   0        0        0     4400 1970-01-01 00:00:00.000000 xlextract-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     3990 2024-05-28 20:17:36.801741 xlextract-0.1.8/README.md
+-rw-r--r--   0        0        0      392 2024-05-28 20:39:16.491315 xlextract-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4594 2024-05-28 20:39:39.001307 xlextract-0.1.8/xlextract/__init__.py
+-rw-r--r--   0        0        0     1886 2024-05-28 20:17:36.801741 xlextract-0.1.8/xlextract/classes.py
+-rw-r--r--   0        0        0     4400 1970-01-01 00:00:00.000000 xlextract-0.1.8/PKG-INFO
```

### Comparing `xlextract-0.1.7/README.md` & `xlextract-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.7/xlextract/__init__.py` & `xlextract-0.1.8/xlextract/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,16 +63,20 @@
                 header_row, left_current_column
             ).value
             if (
                 not left_cell_content
             ):  # Encountered empty cell, exit left boundary discovery
                 col_range[0] = left_current_column + 1
                 break
+            elif left_current_column == 1:  # Left edge of the spreadsheet reached
+                col_range[0] = 1
+                break
             else:
                 left_current_column -= 1
+
         right_current_column: int = keyword_column
         while True:  # Begin Searching Right of Keyword
             try:
                 right_cell_content: str = self.sheet.cell(
                     header_row, right_current_column
                 ).value
             except IndexError:
```

### Comparing `xlextract-0.1.7/xlextract/classes.py` & `xlextract-0.1.8/xlextract/classes.py`

 * *Files identical despite different names*

### Comparing `xlextract-0.1.7/PKG-INFO` & `xlextract-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xlextract
-Version: 0.1.7
+Version: 0.1.8
 Summary: Extract data from Excel files
 Author: AJ Cruz
 Author-email: aj.cruz@computacenter.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

