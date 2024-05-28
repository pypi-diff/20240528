# Comparing `tmp/synct-1.5.3.tar.gz` & `tmp/synct-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synct-1.5.3.tar", last modified: Fri Dec 22 14:08:11 2023, max compression
+gzip compressed data, was "synct-1.6.0.tar", last modified: Tue May 28 08:50:48 2024, max compression
```

## Comparing `synct-1.5.3.tar` & `synct-1.6.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 14:08:11.857077 synct-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-22 14:08:03.000000 synct-1.5.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    32423 2023-12-22 14:08:03.000000 synct-1.5.3/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-22 14:08:03.000000 synct-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16761 2023-12-22 14:08:11.857077 synct-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16220 2023-12-22 14:08:03.000000 synct-1.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-22 14:08:03.000000 synct-1.5.3/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-22 14:08:03.000000 synct-1.5.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 14:08:11.857077 synct-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-12-22 14:08:03.000000 synct-1.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 14:08:11.857077 synct-1.5.3/synct/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 14:08:03.000000 synct-1.5.3/synct/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      884 2023-12-22 14:08:03.000000 synct-1.5.3/synct/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2023-12-22 14:08:03.000000 synct-1.5.3/synct/bzilla.py
--rw-r--r--   0 runner    (1001) docker     (127)    14129 2023-12-22 14:08:03.000000 synct-1.5.3/synct/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2023-12-22 14:08:03.000000 synct-1.5.3/synct/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2023-12-22 14:08:03.000000 synct-1.5.3/synct/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (127)    11484 2023-12-22 14:08:03.000000 synct-1.5.3/synct/gsheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2023-12-22 14:08:03.000000 synct-1.5.3/synct/jira.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2023-12-22 14:08:03.000000 synct-1.5.3/synct/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     9961 2023-12-22 14:08:03.000000 synct-1.5.3/synct/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     7708 2023-12-22 14:08:03.000000 synct-1.5.3/synct/synct.py
--rw-r--r--   0 runner    (1001) docker     (127)     5069 2023-12-22 14:08:03.000000 synct-1.5.3/synct/tsheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2023-12-22 14:08:03.000000 synct-1.5.3/synct/xsheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     7770 2023-12-22 14:08:03.000000 synct-1.5.3/synct/ysheet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 14:08:11.857077 synct-1.5.3/synct.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16761 2023-12-22 14:08:11.000000 synct-1.5.3/synct.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      538 2023-12-22 14:08:11.000000 synct-1.5.3/synct.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 14:08:11.000000 synct-1.5.3/synct.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-22 14:08:11.000000 synct-1.5.3/synct.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 14:08:11.000000 synct-1.5.3/synct.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-22 14:08:11.000000 synct-1.5.3/synct.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-22 14:08:11.000000 synct-1.5.3/synct.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 14:08:11.857077 synct-1.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 14:08:03.000000 synct-1.5.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2023-12-22 14:08:03.000000 synct-1.5.3/tests/test_synct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:50:48.597069 synct-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 08:50:43.000000 synct-1.6.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    32423 2024-05-28 08:50:43.000000 synct-1.6.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 08:50:43.000000 synct-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16761 2024-05-28 08:50:48.597069 synct-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16220 2024-05-28 08:50:43.000000 synct-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 08:50:43.000000 synct-1.6.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-28 08:50:43.000000 synct-1.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 08:50:48.597069 synct-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-28 08:50:43.000000 synct-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:50:48.593069 synct-1.6.0/synct/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:50:43.000000 synct-1.6.0/synct/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      884 2024-05-28 08:50:43.000000 synct-1.6.0/synct/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-28 08:50:43.000000 synct-1.6.0/synct/bzilla.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14129 2024-05-28 08:50:43.000000 synct-1.6.0/synct/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-28 08:50:43.000000 synct-1.6.0/synct/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-28 08:50:43.000000 synct-1.6.0/synct/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11484 2024-05-28 08:50:43.000000 synct-1.6.0/synct/gsheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-28 08:50:43.000000 synct-1.6.0/synct/jira.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-28 08:50:43.000000 synct-1.6.0/synct/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-05-28 08:50:43.000000 synct-1.6.0/synct/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-05-28 08:50:43.000000 synct-1.6.0/synct/synct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-05-28 08:50:43.000000 synct-1.6.0/synct/tsheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-05-28 08:50:43.000000 synct-1.6.0/synct/xsheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-05-28 08:50:43.000000 synct-1.6.0/synct/ysheet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:50:48.597069 synct-1.6.0/synct.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16761 2024-05-28 08:50:48.000000 synct-1.6.0/synct.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-28 08:50:48.000000 synct-1.6.0/synct.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 08:50:48.000000 synct-1.6.0/synct.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 08:50:48.000000 synct-1.6.0/synct.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 08:50:48.000000 synct-1.6.0/synct.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-28 08:50:48.000000 synct-1.6.0/synct.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 08:50:48.000000 synct-1.6.0/synct.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:50:48.597069 synct-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:50:43.000000 synct-1.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-05-28 08:50:43.000000 synct-1.6.0/tests/test_synct.py
```

### Comparing `synct-1.5.3/COPYING` & `synct-1.6.0/COPYING`

 * *Files identical despite different names*

### Comparing `synct-1.5.3/PKG-INFO` & `synct-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synct
-Version: 1.5.3
+Version: 1.6.0
 Summary: Transform data from source to Google or Excel spreadsheet
 Home-page: https://github.com/ari3s/synct
 Author: Jan Beran
 Author-email: ari3s.git@gmail.com
 License: GPL-3.0-or-later
 Description-Content-Type: text/markdown
 License-File: COPYING
@@ -27,15 +27,15 @@
 ## Installation
 
 ### Fedora
 
 The script can be installed on Fedora systems using `dnf` from the package stored in this project:
 
 ```
-sudo dnf install synct-1.5.3-1.fc39.noarch.rpm
+sudo dnf install synct-1.6.0-1.fc39.noarch.rpm
 ```
 
 The script can also be installed from Fedora COPR using these commands:
 
 ```
 sudo dnf copr enable aries/synct
 sudo dnf install synct
@@ -55,15 +55,15 @@
 ```
 
 ### Linux and MacOS
 
 The script can be installed on Linux or MacOS systems using `pip`:
 
 ```
-python -m pip install synct-1.5.3.tar.gz
+python -m pip install synct-1.6.0.tar.gz
 ```
 
 The following dependencies will be installed from PyPI by the above command:
 
 ```
 google-api-python-client
 google-auth-oauthlib
```

### Comparing `synct-1.5.3/README.md` & `synct-1.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ## Installation
 
 ### Fedora
 
 The script can be installed on Fedora systems using `dnf` from the package stored in this project:
 
 ```
-sudo dnf install synct-1.5.3-1.fc39.noarch.rpm
+sudo dnf install synct-1.6.0-1.fc39.noarch.rpm
 ```
 
 The script can also be installed from Fedora COPR using these commands:
 
 ```
 sudo dnf copr enable aries/synct
 sudo dnf install synct
@@ -35,15 +35,15 @@
 ```
 
 ### Linux and MacOS
 
 The script can be installed on Linux or MacOS systems using `pip`:
 
 ```
-python -m pip install synct-1.5.3.tar.gz
+python -m pip install synct-1.6.0.tar.gz
 ```
 
 The following dependencies will be installed from PyPI by the above command:
 
 ```
 google-api-python-client
 google-auth-oauthlib
```

### Comparing `synct-1.5.3/setup.py` & `synct-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `synct-1.5.3/synct/__main__.py` & `synct-1.6.0/synct/__main__.py`

 * *Files identical despite different names*

### Comparing `synct-1.5.3/synct/bzilla.py` & `synct-1.6.0/synct/bzilla.py`

 * *Files identical despite different names*

### Comparing `synct-1.5.3/synct/config.py` & `synct-1.6.0/synct/config.py`

 * *Files identical despite different names*

### Comparing `synct-1.5.3/synct/github.py` & `synct-1.6.0/synct/github.py`

 * *Files identical despite different names*

### Comparing `synct-1.5.3/synct/gitlab.py` & `synct-1.6.0/synct/gitlab.py`

 * *Files identical despite different names*

### Comparing `synct-1.5.3/synct/gsheet.py` & `synct-1.6.0/synct/gsheet.py`

 * *Files identical despite different names*

### Comparing `synct-1.5.3/synct/jira.py` & `synct-1.6.0/synct/jira.py`

 * *Files identical despite different names*

### Comparing `synct-1.5.3/synct/logger.py` & `synct-1.6.0/synct/logger.py`

 * *Files identical despite different names*

### Comparing `synct-1.5.3/synct/source.py` & `synct-1.6.0/synct/source.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,28 +27,29 @@
 
 import pandas as pd
 import synct.logger as log
 
 SOURCE_DATA_KEY = 'SOURCE DATA: key = '
 
 # Warning messages:
+DUPLICATED_TARGET_COLUMN_NAME = 'duplicated column name in the target sheet '
 MISSING_IN_THE_TARGET_SPREADSHEET = 'missing in the target spreadsheet'
 
 class SourceData:
     """ Source data class """
     data = {}
     key_dict = {}
     used_key = {}
 
-    def __init__(self, source_data, sheet_config, target_sheet=None):
+    def __init__(self, source_data, sheet_config, target_sheet_name=None, target_sheet=None):
         """ Convert source data """
         self.key_dict = {}
         self.used_key = {}
         converted_data = []
-        columns_list = create_columns_list(sheet_config, target_sheet)
+        columns_list = create_columns_list(sheet_config, target_sheet_name, target_sheet)
         index = 0
         for source_item in source_data:
             key_value = get_value(source_item, sheet_config, sheet_config.key)
             if key_value is None:
                 continue
             if not isinstance(key_value, str):
                 try:
@@ -107,19 +108,24 @@
             if str(target_sheet.loc[row, (sheet_config.key)]) == str(key_value):
                 target_row = row
                 break
         if target_row is not None:         # original value in the default column
             value = target_sheet.loc[target_row, (column)]
     return value
 
-def create_columns_list(sheet_config, target_sheet):
+def create_columns_list(sheet_config, target_sheet_name, target_sheet):
     """ Create a columns list """
     columns_list = list(sheet_config.columns.keys())
     if target_sheet is not None:
+        duplicates = []
         for column in target_sheet.columns:
+            if column in duplicates:
+                col = column if column else "<empty string>"
+                log.warning(DUPLICATED_TARGET_COLUMN_NAME + target_sheet_name + ': ' +col)
+            duplicates.append(column)
             if column not in columns_list:
                 columns_list.append(column)
     return columns_list
 
 def display_source_record(source_item, key_value, index):
     """ Display the first source data structured record in the debug mode """
     if index > 0 or not log.debug_level():
```

### Comparing `synct-1.5.3/synct/synct.py` & `synct-1.6.0/synct/synct.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,23 +18,25 @@
 
 """
 
 import argparse
 import importlib
 import pyperclip
 
+import pandas as pd
+
 import synct.logger as log
 
 from synct.config import Config
 #from synct.gsheet import Gsheet
 from synct.source import SourceData
 from synct.tsheet import update_target_row_data
 
 PROG = 'synct'
-VERSION = "1.5.3"               # Keep quotation marks here
+VERSION = "1.6.0"               # Keep quotation marks here
 DESCRIPTION = 'Retrieve data from a source and convert it to either '\
         'Google or Excel spreadsheet as defined in the configuration file.'
 EPILOG = 'More details at https://github.com/ari3s/synct'
 
 CONFIG_FILE = PROG + '.yaml'
 
 # Debug messages:
@@ -81,45 +83,64 @@
 def get_data(config, target_spreadsheet):
     """ Get source data """
     source_data = {}
     for sheet_name, query in config.queries.items():
         if config.sheets[sheet_name].default_columns:
             source_data[sheet_name] = SourceData( \
                 config.source.data_query(sheet_name, query), \
-                config.sheets[sheet_name], target_spreadsheet.data[sheet_name])
+                config.sheets[sheet_name], sheet_name, target_spreadsheet.data[sheet_name])
         else:
             source_data[sheet_name] = SourceData( \
                 config.source.data_query(sheet_name, query), \
                 config.sheets[sheet_name])
     log.check_error()
     return source_data
 
+def keep_formula(cell):
+    """ Keep formula and ignore anything else """
+    result = None
+    if isinstance(cell, str) and len(cell) > 0 and cell[0] == '=':
+        result = cell
+    elif isinstance(cell, pd.core.series.Series):
+        formula_flag = False
+        tmp = cell.copy()
+        for index, item in enumerate(list(cell)):
+            if isinstance(item, str) and len(item) > 0 and item[0] == '=':
+                formula_flag = True
+            else:
+                tmp.iat[index] = ''
+        if formula_flag:
+            result = tmp
+    return result
+
 def get_formula(source, target, sheet_name):
     """
     Get formula in the target spreadsheet columns, that are not included
     in the source columns, from the last row.
     """
     formula = {}
+    columns = {}
     for column in target.data[sheet_name].columns:
+        if column in columns:
+            continue
+        columns[column] = True
         condition_1 = target.sheets_config[sheet_name].inherit_formulas and \
                 (column not in list(target.sheets_config[sheet_name].columns.keys()) or \
                 target.sheets_config[sheet_name].default_columns and \
                 column not in source[sheet_name].data.columns)
         condition_2 = column in target.sheets_config[sheet_name].columns and \
                 target.sheets_config[sheet_name].columns[column].inherit_formulas
         if condition_1 or condition_2:
             try:
                 cell = target.data[sheet_name].at[len(target.data[sheet_name])-1, column]
             except KeyError:
                 continue
-            try:
-                if cell[0] == "=":
-                    formula[column] = cell
-            except (IndexError, TypeError):
-                continue
+            result = keep_formula(cell)
+            if result is not None:
+                formula[column] = result
     return formula
 
 def transform_data(source, target, args):
     """ Copy transformed data from the source to the target spreadsheet """
     missing_all_target_key_values = []
     for sheet_name in target.active_sheets:
         key = target.sheets_config[sheet_name].key
@@ -140,23 +161,25 @@
                     message = key + ': <empty key>' + NOT_AVAILABLE + sheet_name
                 if args.remove:
                     log.info(message)
                 else:
                     log.warning(message)
                 target.remove_rows[sheet_name].append(row)
                 continue
-            update_target_row_data(source[sheet_name], key_index, target.data[sheet_name], row)
+            update_target_row_data(source[sheet_name], key_index, target.data[sheet_name], \
+                    target.unique_columns[sheet_name], row)
         # Identify missing keys in the target sheet which data are available from the source
         missing_target_keys = source[sheet_name].check_missing_keys(sheet_name, key, \
                 target.sheets_config[sheet_name], args.add)
         if args.add and not args.noupdate:
             formula = get_formula(source, target, sheet_name)
             for key_value in missing_target_keys:
                 update_target_row_data(source[sheet_name], source[sheet_name].key_dict[key_value], \
-                        target.data[sheet_name], len(target.data[sheet_name]), formula)
+                        target.data[sheet_name], target.unique_columns[sheet_name], \
+                        len(target.data[sheet_name]), formula)
         missing_all_target_key_values = missing_all_target_key_values + missing_target_keys
 
     if missing_all_target_key_values:
         pyperclip.copy('\n'.join(map(str, missing_all_target_key_values)))
 
 def main():
     """
```

### Comparing `synct-1.5.3/synct/tsheet.py` & `synct-1.6.0/synct/tsheet.py`

 * *Files 27% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import pandas as pd
 
 class Tsheet:   # pylint: disable=too-many-instance-attributes
     """ Google spreadsheet class """
     data = {}
     rows = {}
     remove_rows = {}
+    unique_columns = {}
     active_sheets = []
 #    sheet_length = {}   # It is needed for delete_rows workaround.
 
     def __init__(self, config):
         """ Acccess the target spreadsheet and read data """
         self.active_sheets = list(config.sheets.keys())
         self.sheets_config = config.sheets
@@ -44,14 +45,16 @@
         for sheet in self.active_sheets:
             self.get_sheet_data(sheet)
             if self.data[sheet] is None:    # empty table without header
                 remove_sheets.append(sheet) # sign for removing from active sheets
             else:
                 self.remove_rows[sheet] = []
                 self.rows[sheet] = len(self.data[sheet].index)
+                self.unique_columns[sheet] = list(dict.fromkeys( \
+                    self.data[sheet].columns.values.tolist()))
         for sheet in remove_sheets:         # remove signed empty sheets from the next operations
             self.active_sheets.remove(sheet)
 
     def get_sheet_data(self, sheet):
         """ Read sheet data from the target spreadsheet """
 
 #    def insert_rows(self, sheet, start_row, inserted_rows):
@@ -97,26 +100,50 @@
 
 def normalize_type(value):
     """ Avoid numpy type int64 issue that is not allowed in JSON """
     if numpy.issubdtype(type(value), int):
         value = int(value)
     return value
 
-def update_target_row_data(s_sheet, s_key_index, t_sheet, t_row, formula=None):
+def update_target_cell_1(s_sheet, s_key_index, t_sheet, column, t_row, formula):
+    """ Update the target cell with source data """
+    if isinstance(s_sheet.data.loc[s_key_index, (column)], pd.core.series.Series):
+        values = [''] * len(t_sheet.loc[t_row, (column)])
+        for index, element in enumerate(s_sheet.data.loc[s_key_index, (column)]):
+            values[index] = normalize_type(element)
+            if values[index] == '' and formula and column in formula:
+                values[index] = formula[column][index]
+        t_sheet.loc[t_row, (column)] = values
+    else:
+        value = normalize_type(s_sheet.data.loc[s_key_index, (column)])
+        if value == '' and formula and column in formula:
+            value = formula[column]
+        t_sheet.loc[t_row, (column)] = value
+
+def update_target_cell_2(t_sheet, column, t_row, formula):
+    """ Update the target cell with data """
+    if isinstance(t_sheet.loc[t_row, (column)], pd.core.series.Series):
+        values = [''] * len(t_sheet.loc[t_row, (column)])
+        for index, element in enumerate(t_sheet.loc[t_row, (column)].fillna(value='')):
+            values[index] = normalize_type(element)
+            if values[index] == '' and formula and column in formula:
+                values[index] = formula[column][index]
+        t_sheet.loc[t_row, (column)] = values
+    else:
+        if formula and column in formula:
+            value = formula[column]
+        else:
+            value = ''
+        try:
+            if pd.isnull(t_sheet.loc[t_row, (column)]):
+                t_sheet.loc[t_row, (column)] = normalize_type(value)
+        # Fix undefined variable or value issue
+        except (KeyError, ValueError):
+            t_sheet.loc[t_row, (column)] = normalize_type(value)
+
+def update_target_row_data(s_sheet, s_key_index, t_sheet, t_unique_columns, t_row, formula=None):
     """ Update the target row with source data """
-    for column in t_sheet.columns:
+    for column in t_unique_columns:
         if column in s_sheet.data.columns:
-            value = normalize_type(s_sheet.data.loc[s_key_index, (column)])
-            if value == '' and formula and column in formula:
-                value = formula[column]
-            t_sheet.loc[t_row, (column)] = value
+            update_target_cell_1(s_sheet, s_key_index, t_sheet, column, t_row, formula)
         else:
-            if formula and column in formula:
-                value = formula[column]
-            else:
-                value = ""
-            try:
-                if pd.isnull(t_sheet.loc[t_row, (column)]):
-                    t_sheet.loc[t_row, (column)] = normalize_type(value)   # fix undefined value
-            # Fix undefined variable or value issue
-            except (KeyError, ValueError):
-                t_sheet.loc[t_row, (column)] = normalize_type(value)
+            update_target_cell_2(t_sheet, column, t_row, formula)
```

### Comparing `synct-1.5.3/synct/xsheet.py` & `synct-1.6.0/synct/xsheet.py`

 * *Files identical despite different names*

### Comparing `synct-1.5.3/synct/ysheet.py` & `synct-1.6.0/synct/ysheet.py`

 * *Files identical despite different names*

### Comparing `synct-1.5.3/synct.egg-info/PKG-INFO` & `synct-1.6.0/synct.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synct
-Version: 1.5.3
+Version: 1.6.0
 Summary: Transform data from source to Google or Excel spreadsheet
 Home-page: https://github.com/ari3s/synct
 Author: Jan Beran
 Author-email: ari3s.git@gmail.com
 License: GPL-3.0-or-later
 Description-Content-Type: text/markdown
 License-File: COPYING
@@ -27,15 +27,15 @@
 ## Installation
 
 ### Fedora
 
 The script can be installed on Fedora systems using `dnf` from the package stored in this project:
 
 ```
-sudo dnf install synct-1.5.3-1.fc39.noarch.rpm
+sudo dnf install synct-1.6.0-1.fc39.noarch.rpm
 ```
 
 The script can also be installed from Fedora COPR using these commands:
 
 ```
 sudo dnf copr enable aries/synct
 sudo dnf install synct
@@ -55,15 +55,15 @@
 ```
 
 ### Linux and MacOS
 
 The script can be installed on Linux or MacOS systems using `pip`:
 
 ```
-python -m pip install synct-1.5.3.tar.gz
+python -m pip install synct-1.6.0.tar.gz
 ```
 
 The following dependencies will be installed from PyPI by the above command:
 
 ```
 google-api-python-client
 google-auth-oauthlib
```

### Comparing `synct-1.5.3/synct.egg-info/SOURCES.txt` & `synct-1.6.0/synct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `synct-1.5.3/tests/test_synct.py` & `synct-1.6.0/tests/test_synct.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,45 +19,73 @@
 
 TESTS_DIR = Path(__file__).parent
 DATA_DIR = TESTS_DIR / 'data'
 SUFFIX = '.txt'
 
 CONFIG_DATA = DATA_DIR / 'config.yaml'
 SOURCE_DATA = DATA_DIR / 'source_data.txt'
-INITIAL_DATA = DATA_DIR / 'initial_data.txt'
+INITIAL_DATA_BASIC = DATA_DIR / 'initial_data_basic.txt'
+INITIAL_DATA_ADV = DATA_DIR / 'initial_data_adv.txt'
 
-EXPECTED_DATA_0 = DATA_DIR / "expected_data_0.txt"
-EXPECTED_DATA_1 = DATA_DIR / "expected_data_1.txt"
-EXPECTED_DATA_2 = DATA_DIR / "expected_data_2.txt"
-EXPECTED_DATA_3 = DATA_DIR / "expected_data_3.txt"
-EXPECTED_DATA_4 = DATA_DIR / "expected_data_4.txt"
-EXPECTED_DATA_5 = DATA_DIR / "expected_data_5.txt"
-EXPECTED_DATA_6 = DATA_DIR / "expected_data_6.txt"
-EXPECTED_DATA_7 = DATA_DIR / "expected_data_7.txt"
+EXPECTED_DATA_BASIC_0 = DATA_DIR / "expected_data_basic_0.txt"
+EXPECTED_DATA_BASIC_1 = DATA_DIR / "expected_data_basic_1.txt"
+EXPECTED_DATA_BASIC_2 = DATA_DIR / "expected_data_basic_2.txt"
+EXPECTED_DATA_BASIC_3 = DATA_DIR / "expected_data_basic_3.txt"
+EXPECTED_DATA_BASIC_4 = DATA_DIR / "expected_data_basic_4.txt"
+EXPECTED_DATA_BASIC_5 = DATA_DIR / "expected_data_basic_5.txt"
+EXPECTED_DATA_BASIC_6 = DATA_DIR / "expected_data_basic_6.txt"
+EXPECTED_DATA_BASIC_7 = DATA_DIR / "expected_data_basic_7.txt"
+
+EXPECTED_DATA_ADV_0 = DATA_DIR / "expected_data_adv_0.txt"
+EXPECTED_DATA_ADV_1 = DATA_DIR / "expected_data_adv_1.txt"
+EXPECTED_DATA_ADV_2 = DATA_DIR / "expected_data_adv_2.txt"
+EXPECTED_DATA_ADV_3 = DATA_DIR / "expected_data_adv_3.txt"
+EXPECTED_DATA_ADV_4 = DATA_DIR / "expected_data_adv_4.txt"
+EXPECTED_DATA_ADV_5 = DATA_DIR / "expected_data_adv_5.txt"
+EXPECTED_DATA_ADV_6 = DATA_DIR / "expected_data_adv_6.txt"
+EXPECTED_DATA_ADV_7 = DATA_DIR / "expected_data_adv_7.txt"
 
 SHEET = "TEST"
 
 class Args:                  #pylint: disable=too-few-public-methods
     """ Default command line arguments of the script """
     add = False
     remove = False
     noupdate = False
 
-def operation(mock_tsheet_class, add, default_columns, inherit_formulas):
+def allow_duplicated_columns(df):
+    """ Transformation data structure like obtained from pd.read_excel """
+    col_map = []
+    for col in df.columns:
+        if col.rpartition('.')[0]:
+            col_name = col.rpartition('.')[0]
+            in_map = col.rpartition('.')[0] in col_map
+            last_is_num = col.rpartition('.')[-1].isdigit()
+            dupe_count = col_map.count(col_name)
+            if in_map and last_is_num and (int(col.rpartition('.')[-1]) == dupe_count):
+                col_map.append(col_name)
+                continue
+        col_map.append(col)
+    df.columns = col_map
+
+def operation(initial_data, mock_tsheet_class, add, default_columns, inherit_formulas):
     """ Make the operation with data and return the final data """
 
     # Arguments set-up
     args = Args()
     args.add = add
 
     # Prepare the mock Gsheet instance
-    target_spreadsheet_data = pd.read_fwf(INITIAL_DATA, encoding='utf-8', dtype=str)
+    target_spreadsheet_data = pd.read_fwf(initial_data, encoding='utf-8', dtype=str)
+    allow_duplicated_columns(target_spreadsheet_data)
     tsheet_instance = mock_tsheet_class.return_value
     tsheet_instance.active_sheets = [SHEET]
     tsheet_instance.data = {SHEET: target_spreadsheet_data}
+    tsheet_instance.unique_columns = \
+            {SHEET: list(dict.fromkeys(target_spreadsheet_data.columns.values.tolist()))}
 
     # Read source data
     source_data = pd.read_fwf(SOURCE_DATA, encoding='utf-8', dtype=str).to_dict(orient='records')
 
     # Configure tests parameters
     sheet_conf = configure(default_columns, inherit_formulas)
     tsheet_instance.sheets_config = sheet_conf
@@ -89,15 +117,15 @@
     return sheet_conf
 
 def set_source_data_instance(source_data, sheet_conf, tsheet_instance):
     """ Set up source data instance """
     source_data_instance = {}
     if sheet_conf[SHEET].default_columns:
         source_data_instance[SHEET] = SourceData(source_data, \
-            sheet_conf[SHEET], tsheet_instance.data[SHEET])
+            sheet_conf[SHEET], SHEET, tsheet_instance.data[SHEET])
     else:
         source_data_instance[SHEET] = SourceData(source_data, \
             sheet_conf[SHEET])
     return source_data_instance
 
 def custom_name_func(testcase_func, param_num, param):
     """
@@ -106,29 +134,56 @@
     :param param_num: will be the index of the test case parameters in the list of parameters
     :param param: (an instance of param) will be the parameters which will be used.
     :return: test case name
     """
     return (f"{testcase_func.__name__}_"
             f"{parameterized.to_safe_name('_'.join([str(param.args[0]), param_num]))}")
 
-class TestTransformData(unittest.TestCase):
-    """ Test the synct script functionality """
+class TestTransformDataBasic(unittest.TestCase):
+    """ Test the basic synct script functionality with unique columns """
+    @parameterized.expand([
+        # Order of parameters:
+        # test name, add rows, default columns, inherit formulas, expected data
+        ('disabledparameters', False, False, False, EXPECTED_DATA_BASIC_0),
+        ('addrows', True, False, False, EXPECTED_DATA_BASIC_1),
+        ('defaultcolumns', False, True, False, EXPECTED_DATA_BASIC_2),
+        ('addrows_defaultcolumns', True, True, False, EXPECTED_DATA_BASIC_3),
+        ('inheritformulas', False, False, True, EXPECTED_DATA_BASIC_4),
+        ('addrows_inheritformulas', True, False, True, EXPECTED_DATA_BASIC_5),
+        ('defaultcolumns_inheritformulas', False, True, True, EXPECTED_DATA_BASIC_6),
+        ('addrows_defaultcolumns_inheritformulas', True, True, True, EXPECTED_DATA_BASIC_7)
+    ], name_func=custom_name_func)
+
+    @patch('synct.tsheet.Tsheet', autospec=True)
+    def test_transform_data(self, name, add, default_columns, inherit_formulas, expected_data, \
+            mock_tsheet_class):           #pylint: disable=too-many-arguments,unused-argument
+        """ Testing with fake data """
+        transformed_data = operation(INITIAL_DATA_BASIC, mock_tsheet_class, add, default_columns, \
+                inherit_formulas).fillna('')
+        expected_data = pd.read_fwf(expected_data, encoding='utf-8', dtype=str).fillna('')
+        allow_duplicated_columns(expected_data)
+        assert_frame_equal(transformed_data, expected_data, check_dtype=False)
+
+class TestTransformDataAdv(unittest.TestCase):
+    """ Test the advanced synct script functionality with multiple target columns """
     @parameterized.expand([
         # Order of parameters:
         # test name, add rows, default columns, inherit formulas, expected data
-        ('disabledparameters', False, False, False, EXPECTED_DATA_0),
-        ('addrows', True, False, False, EXPECTED_DATA_1),
-        ('defaultcolumns', False, True, False, EXPECTED_DATA_2),
-        ('addrows_defaultcolumns', True, True, False, EXPECTED_DATA_3),
-        ('inheritformulas', False, False, True, EXPECTED_DATA_4),
-        ('addrows_inheritformulas', True, False, True, EXPECTED_DATA_5),
-        ('defaultcolumns_inheritformulas', False, True, True, EXPECTED_DATA_6),
-        ('addrows_defaultcolumns_inheritformulas', True, True, True, EXPECTED_DATA_7)
+        ('disabledparameters', False, False, False, EXPECTED_DATA_ADV_0),
+        ('addrows', True, False, False, EXPECTED_DATA_ADV_1),
+        ('defaultcolumns', False, True, False, EXPECTED_DATA_ADV_2),
+        ('addrows_defaultcolumns', True, True, False, EXPECTED_DATA_ADV_3),
+        ('inheritformulas', False, False, True, EXPECTED_DATA_ADV_4),
+        ('addrows_inheritformulas', True, False, True, EXPECTED_DATA_ADV_5),
+        ('defaultcolumns_inheritformulas', False, True, True, EXPECTED_DATA_ADV_6),
+        ('addrows_defaultcolumns_inheritformulas', True, True, True, EXPECTED_DATA_ADV_7)
     ], name_func=custom_name_func)
 
     @patch('synct.tsheet.Tsheet', autospec=True)
     def test_transform_data(self, name, add, default_columns, inherit_formulas, expected_data, \
             mock_tsheet_class):           #pylint: disable=too-many-arguments,unused-argument
         """ Testing with fake data """
-        transformed_data = operation(mock_tsheet_class, add, default_columns, inherit_formulas)
+        transformed_data = operation(INITIAL_DATA_ADV, mock_tsheet_class, add, default_columns, \
+                inherit_formulas).fillna('')
         expected_data = pd.read_fwf(expected_data, encoding='utf-8', dtype=str).fillna('')
+        allow_duplicated_columns(expected_data)
         assert_frame_equal(transformed_data, expected_data, check_dtype=False)
```

