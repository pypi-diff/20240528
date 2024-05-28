# Comparing `tmp/exv-1.0.2.tar.gz` & `tmp/exv-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exv-1.0.2.tar", last modified: Tue May 28 07:19:06 2024, max compression
+gzip compressed data, was "exv-1.1.tar", last modified: Tue May 28 09:22:44 2024, max compression
```

## Comparing `exv-1.0.2.tar` & `exv-1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:19:06.343549 exv-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-28 07:18:58.000000 exv-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-28 07:19:06.343549 exv-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-28 07:18:58.000000 exv-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-28 07:18:58.000000 exv-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 07:19:06.343549 exv-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:19:06.343549 exv-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:19:06.343549 exv-1.0.2/src/exv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-28 07:19:06.000000 exv-1.0.2/src/exv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-28 07:19:06.000000 exv-1.0.2/src/exv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 07:19:06.000000 exv-1.0.2/src/exv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 07:19:06.000000 exv-1.0.2/src/exv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 07:19:06.000000 exv-1.0.2/src/exv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 07:19:06.000000 exv-1.0.2/src/exv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-28 07:18:58.000000 exv-1.0.2/src/exv.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 07:18:58.000000 exv-1.0.2/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:22:44.846369 exv-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-28 09:22:36.000000 exv-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-28 09:22:44.846369 exv-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-28 09:22:36.000000 exv-1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-28 09:22:36.000000 exv-1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 09:22:44.846369 exv-1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:22:44.842369 exv-1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:22:44.842369 exv-1.1/src/exv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-28 09:22:44.000000 exv-1.1/src/exv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-28 09:22:44.000000 exv-1.1/src/exv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:22:44.000000 exv-1.1/src/exv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 09:22:44.000000 exv-1.1/src/exv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 09:22:44.000000 exv-1.1/src/exv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 09:22:44.000000 exv-1.1/src/exv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-28 09:22:36.000000 exv-1.1/src/exv.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 09:22:36.000000 exv-1.1/src/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-28 09:22:36.000000 exv-1.1/src/xlfile.py
```

### Comparing `exv-1.0.2/LICENSE` & `exv-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exv-1.0.2/PKG-INFO` & `exv-1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: exv
-Version: 1.0.2
+Version: 1.1
 Summary: View Excel files in the terminal
 Author-email: Lars Arvestad <arve@math.su.se>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, http://github.com/arvestad/exv
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tabulate
-Requires-Dist: openpyxl
+Requires-Dist: openpyxl>3.0
+Requires-Dist: xlrd>2.0
 
 # exv:  a simple Excel file viewer for the command line
 
 Command line tool for viewing Excel files.
 
 The module `openpyxl` is used for parsing and interpretation of the input files,
 and `tabulate` is used for viewing worksheets in a tabular fashion.
```

### Comparing `exv-1.0.2/README.md` & `exv-1.1/README.md`

 * *Files identical despite different names*

### Comparing `exv-1.0.2/pyproject.toml` & `exv-1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [project]
 name = "exv"
 dependencies = [
     "tabulate",
-    "openpyxl"
+    "openpyxl>3.0",
+    "xlrd>2.0"
 ]
 authors = [
     {name = "Lars Arvestad", email = "arve@math.su.se"}
 ]
 description = "View Excel files in the terminal"
 readme = "README.md"
 license = {text = "GNU General Public License v3 (GPLv3)"}
```

### Comparing `exv-1.0.2/src/exv.egg-info/PKG-INFO` & `exv-1.1/src/exv.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: exv
-Version: 1.0.2
+Version: 1.1
 Summary: View Excel files in the terminal
 Author-email: Lars Arvestad <arve@math.su.se>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, http://github.com/arvestad/exv
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tabulate
-Requires-Dist: openpyxl
+Requires-Dist: openpyxl>3.0
+Requires-Dist: xlrd>2.0
 
 # exv:  a simple Excel file viewer for the command line
 
 Command line tool for viewing Excel files.
 
 The module `openpyxl` is used for parsing and interpretation of the input files,
 and `tabulate` is used for viewing worksheets in a tabular fashion.
```

### Comparing `exv-1.0.2/src/exv.py` & `exv-1.1/src/exv.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import argparse
 from tabulate import tabulate, tabulate_formats
-from openpyxl import load_workbook
 from version import __version__
 import string
+import sys
+
+from xlfile import xlFile, xlFileErrorSheetnameError
+
 
 def setup_argparse():
     ap = argparse.ArgumentParser(prog='exv', description='Command line tool for viewing Excel files.') 
     ap.add_argument('infile', help='An Excel file')
     ap.add_argument('worksheet', nargs='?',
                     help='View the named worksheet. Without a worksheet either the single existing worksheet is viewed or a list of worksheets is displayed.')
     ap.add_argument('-n', '--no-indices', action='store_true',
                     help='Do not show row and column indices.')
     ap.add_argument('-nc', '--no-col-indices', action='store_true',
                     help='Do not show column indices.')
     ap.add_argument('-nr', '--no-row-numbers', action='store_true',
                     help='Do not show row numbers.')
     ap.add_argument('-f', '--format', choices=tabulate_formats,
-                    default='plain',
+                    default='presto',
                     help='Output format.')
     ap.add_argument('-v', '--version', action='version', version='%(prog)s '+__version__)    
 
     return ap
 
 
 def columns_ident(i):
@@ -38,24 +41,24 @@
         prefix = columns_ident(i // 26 - 1)
     else:
         prefix = ''
     return prefix + (string.ascii_uppercase[i % 26])
 
 
 def view_worksheet(book, sheetname, args):
-    sh = book[sheetname]
+    sh = book.sheet(sheetname)
     tab_rows = []
 
-    for row in sh.values:
+    for row in sh.rows():
         new_row = []
         for cell in row:
             new_row.append(cell)
         tab_rows.append(new_row)
 
-    header = list(map(columns_ident, range(sh.max_column)))
+    header = list(map(columns_ident, range(sh.n_columns())))
     if args.no_indices:
         print(tabulate(tab_rows, tablefmt=args.format))
     elif args.no_col_indices:
         print(tabulate(tab_rows, showindex='always', tablefmt=args.format))
     elif args.no_row_numbers:
         print(tabulate(tab_rows, headers=header, tablefmt=args.format))
     else:
@@ -63,20 +66,24 @@
 
     
 
 def main():
     ap = setup_argparse()
     args = ap.parse_args()
 
-    wb = load_workbook(args.infile, data_only=True)
-    if args.worksheet:
-        view_worksheet(wb, args.worksheet, args)
-    elif len(wb.sheetnames) > 1:
-        print('Available sheets:')
-        for sheetname in wb.sheetnames:
-            print(sheetname)
-    else:
-        view_worksheet(wb, wb.sheetnames[0], args)
+    wb = xlFile.load_excel_file(args.infile)
+
+    try:
+        if args.worksheet:
+            view_worksheet(wb, args.worksheet, args)
+        elif len(wb.sheet_names()) > 1:
+            print('Available sheets:')
+            for sheetname in wb.sheet_names():
+                print(sheetname)
+        else:
+            view_worksheet(wb, wb.sheet_names()[0], args)
+    except xlFileErrorSheetnameError:
+        sys.exit(f'exv: Wrong sheet name')
         
 
 if __name__ == '__main__':
     main()
```

