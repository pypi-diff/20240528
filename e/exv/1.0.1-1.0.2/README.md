# Comparing `tmp/exv-1.0.1.tar.gz` & `tmp/exv-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exv-1.0.1.tar", last modified: Mon May 27 20:46:23 2024, max compression
+gzip compressed data, was "exv-1.0.2.tar", last modified: Tue May 28 07:19:06 2024, max compression
```

## Comparing `exv-1.0.1.tar` & `exv-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:46:23.731293 exv-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 20:46:19.000000 exv-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-27 20:46:23.731293 exv-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-27 20:46:19.000000 exv-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-27 20:46:19.000000 exv-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:46:23.731293 exv-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:46:23.731293 exv-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:46:23.731293 exv-1.0.1/src/exv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-27 20:46:23.000000 exv-1.0.1/src/exv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-27 20:46:23.000000 exv-1.0.1/src/exv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:46:23.000000 exv-1.0.1/src/exv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-27 20:46:23.000000 exv-1.0.1/src/exv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-27 20:46:23.000000 exv-1.0.1/src/exv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-27 20:46:23.000000 exv-1.0.1/src/exv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-27 20:46:19.000000 exv-1.0.1/src/exv.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 20:46:19.000000 exv-1.0.1/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:19:06.343549 exv-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-28 07:18:58.000000 exv-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-28 07:19:06.343549 exv-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-28 07:18:58.000000 exv-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-28 07:18:58.000000 exv-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 07:19:06.343549 exv-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:19:06.343549 exv-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:19:06.343549 exv-1.0.2/src/exv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-28 07:19:06.000000 exv-1.0.2/src/exv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-28 07:19:06.000000 exv-1.0.2/src/exv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 07:19:06.000000 exv-1.0.2/src/exv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 07:19:06.000000 exv-1.0.2/src/exv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 07:19:06.000000 exv-1.0.2/src/exv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 07:19:06.000000 exv-1.0.2/src/exv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-28 07:18:58.000000 exv-1.0.2/src/exv.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 07:18:58.000000 exv-1.0.2/src/version.py
```

### Comparing `exv-1.0.1/LICENSE` & `exv-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `exv-1.0.1/PKG-INFO` & `exv-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exv
-Version: 1.0.1
+Version: 1.0.2
 Summary: View Excel files in the terminal
 Author-email: Lars Arvestad <arve@math.su.se>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, http://github.com/arvestad/exv
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 
 Command line tool for viewing Excel files.
 
 The module `openpyxl` is used for parsing and interpretation of the input files,
 and `tabulate` is used for viewing worksheets in a tabular fashion.
 
 Formulas are handled, but no attempt is made at making use of embedded charts and other non-tabular objects.
-
+In fact, nothing fancy has dealt with.
 
 ## Usage
 
 The basic usage is `exv <excelfile> [<worksheet>]`. If the given excel file has a single worksheet, then the worksheet is viewed.
 A list of worksheet names are given if there is more than one worksheet defined in the file. You can give a format argument
 to have the sheet displayed in a special way.
```

### Comparing `exv-1.0.1/README.md` & `exv-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Command line tool for viewing Excel files.
 
 The module `openpyxl` is used for parsing and interpretation of the input files,
 and `tabulate` is used for viewing worksheets in a tabular fashion.
 
 Formulas are handled, but no attempt is made at making use of embedded charts and other non-tabular objects.
-
+In fact, nothing fancy has dealt with.
 
 ## Usage
 
 The basic usage is `exv <excelfile> [<worksheet>]`. If the given excel file has a single worksheet, then the worksheet is viewed.
 A list of worksheet names are given if there is more than one worksheet defined in the file. You can give a format argument
 to have the sheet displayed in a special way.
```

### Comparing `exv-1.0.1/pyproject.toml` & `exv-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `exv-1.0.1/src/exv.egg-info/PKG-INFO` & `exv-1.0.2/src/exv.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exv
-Version: 1.0.1
+Version: 1.0.2
 Summary: View Excel files in the terminal
 Author-email: Lars Arvestad <arve@math.su.se>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, http://github.com/arvestad/exv
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 
 Command line tool for viewing Excel files.
 
 The module `openpyxl` is used for parsing and interpretation of the input files,
 and `tabulate` is used for viewing worksheets in a tabular fashion.
 
 Formulas are handled, but no attempt is made at making use of embedded charts and other non-tabular objects.
-
+In fact, nothing fancy has dealt with.
 
 ## Usage
 
 The basic usage is `exv <excelfile> [<worksheet>]`. If the given excel file has a single worksheet, then the worksheet is viewed.
 A list of worksheet names are given if there is more than one worksheet defined in the file. You can give a format argument
 to have the sheet displayed in a special way.
```

