# Comparing `tmp/arff-format-converter-1.0.3b4.tar.gz` & `tmp/arff_format_converter-1.0.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arff-format-converter-1.0.3b4.tar", last modified: Sun Feb  4 10:02:09 2024, max compression
+gzip compressed data, was "arff_format_converter-1.0.4b0.tar", last modified: Tue May 28 12:15:53 2024, max compression
```

## Comparing `arff-format-converter-1.0.3b4.tar` & `arff_format_converter-1.0.4b0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-02-04 10:02:09.359870 arff-format-converter-1.0.3b4/
--rw-rw-rw-   0        0        0     1139 2024-02-04 09:01:36.000000 arff-format-converter-1.0.3b4/LICENSE
--rw-rw-rw-   0        0        0     3508 2024-02-04 10:02:09.356880 arff-format-converter-1.0.3b4/PKG-INFO
--rw-rw-rw-   0        0        0     1404 2024-02-04 08:20:27.000000 arff-format-converter-1.0.3b4/README.md
-drwxrwxrwx   0        0        0        0 2024-02-04 10:02:09.310982 arff-format-converter-1.0.3b4/arff_format_converter/
--rw-rw-rw-   0        0        0     1166 2024-02-04 09:55:57.000000 arff-format-converter-1.0.3b4/arff_format_converter/__init__.py
--rw-rw-rw-   0        0        0      156 2024-02-04 10:01:44.000000 arff-format-converter-1.0.3b4/arff_format_converter/arff_converter.py
--rw-rw-rw-   0        0        0      762 2024-02-03 15:56:31.000000 arff-format-converter-1.0.3b4/arff_format_converter/logs.py
--rw-rw-rw-   0        0        0     4339 2024-02-04 09:53:25.000000 arff-format-converter-1.0.3b4/arff_format_converter/output.py
--rw-rw-rw-   0        0        0      441 2024-02-04 09:56:11.000000 arff-format-converter-1.0.3b4/arff_format_converter/texts.py
--rw-rw-rw-   0        0        0     3019 2024-02-04 09:53:08.000000 arff-format-converter-1.0.3b4/arff_format_converter/utils.py
--rw-rw-rw-   0        0        0      728 2024-02-04 09:53:16.000000 arff-format-converter-1.0.3b4/arff_format_converter/validate.py
-drwxrwxrwx   0        0        0        0 2024-02-04 10:02:09.353391 arff-format-converter-1.0.3b4/arff_format_converter.egg-info/
--rw-rw-rw-   0        0        0     3508 2024-02-04 10:02:09.000000 arff-format-converter-1.0.3b4/arff_format_converter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      545 2024-02-04 10:02:09.000000 arff-format-converter-1.0.3b4/arff_format_converter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-04 10:02:09.000000 arff-format-converter-1.0.3b4/arff_format_converter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2024-02-04 10:02:09.000000 arff-format-converter-1.0.3b4/arff_format_converter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2024-02-04 10:02:09.000000 arff-format-converter-1.0.3b4/arff_format_converter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-02-04 10:02:09.000000 arff-format-converter-1.0.3b4/arff_format_converter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      600 2024-02-04 10:02:00.000000 arff-format-converter-1.0.3b4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-04 10:02:09.359870 arff-format-converter-1.0.3b4/setup.cfg
--rw-rw-rw-   0        0        0     1562 2024-02-04 10:02:06.000000 arff-format-converter-1.0.3b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:53.853645 arff_format_converter-1.0.4b0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-28 12:15:32.000000 arff_format_converter-1.0.4b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-28 12:15:53.853645 arff_format_converter-1.0.4b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-28 12:15:32.000000 arff_format_converter-1.0.4b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:53.853645 arff_format_converter-1.0.4b0/arff_format_converter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-28 12:15:32.000000 arff_format_converter-1.0.4b0/arff_format_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-28 12:15:32.000000 arff_format_converter-1.0.4b0/arff_format_converter/arff_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-28 12:15:32.000000 arff_format_converter-1.0.4b0/arff_format_converter/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-28 12:15:32.000000 arff_format_converter-1.0.4b0/arff_format_converter/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-28 12:15:32.000000 arff_format_converter-1.0.4b0/arff_format_converter/texts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-28 12:15:32.000000 arff_format_converter-1.0.4b0/arff_format_converter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-28 12:15:32.000000 arff_format_converter-1.0.4b0/arff_format_converter/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:15:53.853645 arff_format_converter-1.0.4b0/arff_format_converter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-28 12:15:53.000000 arff_format_converter-1.0.4b0/arff_format_converter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-28 12:15:53.000000 arff_format_converter-1.0.4b0/arff_format_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:15:53.000000 arff_format_converter-1.0.4b0/arff_format_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-28 12:15:53.000000 arff_format_converter-1.0.4b0/arff_format_converter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 12:15:53.000000 arff_format_converter-1.0.4b0/arff_format_converter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 12:15:53.000000 arff_format_converter-1.0.4b0/arff_format_converter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-28 12:15:32.000000 arff_format_converter-1.0.4b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 12:15:53.853645 arff_format_converter-1.0.4b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-28 12:15:32.000000 arff_format_converter-1.0.4b0/setup.py
```

### Comparing `arff-format-converter-1.0.3b4/LICENSE` & `arff_format_converter-1.0.4b0/LICENSE`

 * *Files identical despite different names*

### Comparing `arff-format-converter-1.0.3b4/arff_format_converter/__init__.py` & `arff_format_converter-1.0.4b0/arff_format_converter/__init__.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-"""
-Convert ARFF files to different formats.
-The arff-converter tool allows you to convert ARFF files to various output formats. Below are the details:
-
-*SYNOPSIS:
-    arff-format-converter -f <file> -o <output_folder> -fmt <output_format>
-
-*EXAMPLES:
-    arff-format-converter -f data.arff -o output -fmt json
-    arff-format-converter -f data.arff -o output -fmt xml
-    arff-format-converter -f data.arff -o output -fmt csv
-    arff-format-converter -f data.arff -o output -fmt xlsx
-    arff-format-converter -f data.arff -o output -fmt orc
-
-*OPTIONS:
-    -f, --file      Path to the ARFF file.
-    -o, --output    Path to the output folder.
-    -fmt, --format  Output format: 'xml', 'json', 'csv', 'xlsx', 'orc'.
-
-*SUPPORTED FORMATS:
-    - ARFF (input)
-    - XML (output)
-    - JSON (output)
-    - CSV (output)
-    - XLSX (output)
-    - ORC (Apache ORC format) (output)
-
-*AUTHOR:
-    Written by Shani Sinojiya <https://www.shanisinojiya.com>.
-
-*REPORTING BUGS:
-    Report bugs to <https://github.com/Shani-Sinojiya/arff-format-converter/issues>
-
-*COPYRIGHT:
-    The MIT License (MIT)
-    Copyright © 2024 Shani Sinojiya
-"""
+"""
+Convert ARFF files to different formats.
+The arff-converter tool allows you to convert ARFF files to various output formats. Below are the details:
+
+*SYNOPSIS:
+    arff-format-converter -f <file> -o <output_folder> -fmt <output_format>
+
+*EXAMPLES:
+    arff-format-converter -f data.arff -o output -fmt json
+    arff-format-converter -f data.arff -o output -fmt xml
+    arff-format-converter -f data.arff -o output -fmt csv
+    arff-format-converter -f data.arff -o output -fmt xlsx
+    arff-format-converter -f data.arff -o output -fmt orc
+
+*OPTIONS:
+    -f, --file      Path to the ARFF file.
+    -o, --output    Path to the output folder.
+    -fmt, --format  Output format: 'xml', 'json', 'csv', 'xlsx', 'orc'.
+
+*SUPPORTED FORMATS:
+    - ARFF (input)
+    - XML (output)
+    - JSON (output)
+    - CSV (output)
+    - XLSX (output)
+    - ORC (Apache ORC format) (output)
+
+*AUTHOR:
+    Written by Shani Sinojiya <https://www.shanisinojiya.com>.
+
+*REPORTING BUGS:
+    Report bugs to <https://github.com/Shani-Sinojiya/arff-format-converter/issues>
+
+*COPYRIGHT:
+    The MIT License (MIT)
+    Copyright © 2024 Shani Sinojiya
+"""
```

### Comparing `arff-format-converter-1.0.3b4/arff_format_converter/logs.py` & `arff_format_converter-1.0.4b0/arff_format_converter/logs.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import sys
-
-FILE_ERROR = 0
-OPTION_ERROR = 1
-OTHER_ERROR = 2
-legal_formats = ["xml", "json", "csv", "xlsx", "orc"]
-error_array = ["Invalid file extension - expects '<filename>.arff'",
-               "Invalid option - expects 'xml', 'json', 'csv', 'xlsx', or 'orc'.", "The file format is invalid."]
-error_log = []
-
-
-def console(msg):
-    print(msg, file=sys.stderr)
-
-
-def log_error(line_num, error_index, details):
-    this_error = {"line_num": line_num,
-                  "message": error_array[error_index], "details": details}
-    error_log.append(this_error)
-    console(f"Error at {line_num}:")
-    console(error_array[error_index])
-    console(details)
-
-
-def exit_with_errors():
-    console("Exiting with errors.")
-    sys.exit(1)
+import sys
+
+FILE_ERROR = 0
+OPTION_ERROR = 1
+OTHER_ERROR = 2
+legal_formats = ["xml", "json", "csv", "xlsx", "orc"]
+error_array = ["Invalid file extension - expects '<filename>.arff'",
+               "Invalid option - expects 'xml', 'json', 'csv', 'xlsx', or 'orc'.", "The file format is invalid."]
+error_log = []
+
+
+def console(msg):
+    print(msg, file=sys.stderr)
+
+
+def log_error(line_num, error_index, details):
+    this_error = {"line_num": line_num,
+                  "message": error_array[error_index], "details": details}
+    error_log.append(this_error)
+    console(f"Error at {line_num}:")
+    console(error_array[error_index])
+    console(details)
+
+
+def exit_with_errors():
+    console("Exiting with errors.")
+    sys.exit(1)
```

### Comparing `arff-format-converter-1.0.3b4/arff_format_converter/validate.py` & `arff_format_converter-1.0.4b0/arff_format_converter/validate.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from .logs import *
-import os
-
-
-def validate_file_path(path: str):
-    if not os.path.isfile(path):
-        log_error(
-            0, FILE_ERROR, "Invalid file path. Please provide a valid path to the ARFF file.")
-        exit_with_errors()
-
-
-def validate_output_folder(path: str):
-    if not os.path.isdir(path):
-        log_error(
-            0, FILE_ERROR, "Invalid output folder path. Please provide a valid path to the output folder.")
-        exit_with_errors()
-
-
-def validate_output_format(output_format: str):
-    if output_format not in legal_formats:
-        log_error(0, OPTION_ERROR,
-                  "Invalid output format. Please provide a valid output format.")
-        exit_with_errors()
+from .logs import *
+import os
+
+
+def validate_file_path(path: str):
+    if not os.path.isfile(path):
+        log_error(
+            0, FILE_ERROR, "Invalid file path. Please provide a valid path to the ARFF file.")
+        exit_with_errors()
+
+
+def validate_output_folder(path: str):
+    if not os.path.isdir(path):
+        log_error(
+            0, FILE_ERROR, "Invalid output folder path. Please provide a valid path to the output folder.")
+        exit_with_errors()
+
+
+def validate_output_format(output_format: str):
+    if output_format not in legal_formats:
+        log_error(0, OPTION_ERROR,
+                  "Invalid output format. Please provide a valid output format.")
+        exit_with_errors()
```

### Comparing `arff-format-converter-1.0.3b4/arff_format_converter.egg-info/SOURCES.txt` & `arff_format_converter-1.0.4b0/arff_format_converter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arff-format-converter-1.0.3b4/pyproject.toml` & `arff_format_converter-1.0.4b0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-[build-system]
-build-backend = "setuptools.build_meta"
-requires = ["setuptools", "wheel"]
-
-[tool.poetry]
-authors = ["Shani Sinojiya <shanisinojiya@gmail.com>"]
-description = "A tool to convert ARFF files to different formats."
-license = "MIT"
-name = "arff-format-converter"
-readme = "README.md"
-requires-python = ">=3.6"
-version = "1.0.3-beta-4"
-
-[tool.poetry.dependencies]
-argparse = "^1.4.0"
-fastavro = "^1.9.3"
-openpyxl = "^3.1.2"
-pandas = "^2.2.0"
-tqdm = "^4.66.1"
-ujson = "^5.9.0"
-
-[tool.poetry.scripts]
-arff-format-converter = "arff_format_converter.arff_converter:main"
+[build-system]
+build-backend = "setuptools.build_meta"
+requires = ["setuptools>=61.0", "wheel"]
+
+[tool.poetry]
+authors = ["Shani Sinojiya <shanisinojiya@gmail.com>"]
+description = "A tool to convert ARFF files to different formats."
+license = "MIT"
+name = "arff-format-converter"
+readme = "README.md"
+requires-python = ">=3.8"
+version = "1.0.4b0"
+
+[tool.poetry.dependencies]
+argparse = "^1.4.0"
+pandas = "^2.2.0"
+pyarrow = "^16.0.0"
+
+[tool.poetry.scripts]
+arff-format-converter = "arff_format_converter.arff_converter:main"
+
+[tool.poetry.urls]
+Homepage = "https://github.com/Shani-Sinojiya/arff-format-converter"
+Issues = "https://github.com/Shani-Sinojiya/arff-format-converter/issues"
```

