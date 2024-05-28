# Comparing `tmp/dpkits-1.2.6.tar.gz` & `tmp/dpkits-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpkits-1.2.6.tar", last modified: Thu May 23 04:25:02 2024, max compression
+gzip compressed data, was "dpkits-1.2.7.tar", last modified: Tue May 28 03:21:12 2024, max compression
```

## Comparing `dpkits-1.2.6.tar` & `dpkits-1.2.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 04:25:02.137490 dpkits-1.2.6/
--rw-rw-rw-   0        0        0     1091 2023-08-31 09:04:23.000000 dpkits-1.2.6/LICENSE
--rw-rw-rw-   0        0        0    12196 2024-05-23 04:25:02.135809 dpkits-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0    11652 2023-10-06 10:25:52.000000 dpkits-1.2.6/README.md
--rw-rw-rw-   0        0        0      626 2024-05-23 04:23:16.000000 dpkits-1.2.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-23 04:25:02.137490 dpkits-1.2.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-23 04:25:02.073214 dpkits-1.2.6/src/
-drwxrwxrwx   0        0        0        0 2024-05-23 04:25:02.097501 dpkits-1.2.6/src/dpkits/
--rw-rw-rw-   0        0        0      565 2024-01-11 08:02:54.000000 dpkits-1.2.6/src/dpkits/__init__.py
--rw-rw-rw-   0        0        0    28970 2024-05-23 03:35:42.000000 dpkits-1.2.6/src/dpkits/ap_data_converter.py
--rw-rw-rw-   0        0        0     9948 2023-10-04 08:35:50.000000 dpkits-1.2.6/src/dpkits/calculate_lsm.py
--rw-rw-rw-   0        0        0    11069 2024-01-31 04:23:09.000000 dpkits-1.2.6/src/dpkits/codeframe_reader.py
--rw-rw-rw-   0        0        0     5209 2024-05-06 08:45:27.000000 dpkits-1.2.6/src/dpkits/data_analysis.py
--rw-rw-rw-   0        0        0     3241 2024-05-16 11:03:27.000000 dpkits-1.2.6/src/dpkits/data_processing.py
--rw-rw-rw-   0        0        0     8198 2024-03-29 03:28:36.000000 dpkits-1.2.6/src/dpkits/data_transpose.py
--rw-rw-rw-   0        0        0    26578 2024-05-10 10:00:29.000000 dpkits-1.2.6/src/dpkits/table_formater.py
--rw-rw-rw-   0        0        0    67398 2024-05-23 04:14:33.000000 dpkits-1.2.6/src/dpkits/table_generator.py
-drwxrwxrwx   0        0        0        0 2024-05-23 04:25:02.132583 dpkits-1.2.6/src/dpkits.egg-info/
--rw-rw-rw-   0        0        0    12196 2024-05-23 04:25:02.000000 dpkits-1.2.6/src/dpkits.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2024-05-23 04:25:02.000000 dpkits-1.2.6/src/dpkits.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 04:25:02.000000 dpkits-1.2.6/src/dpkits.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-23 04:25:02.000000 dpkits-1.2.6/src/dpkits.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 03:21:12.306970 dpkits-1.2.7/
+-rw-rw-rw-   0        0        0     1091 2023-08-31 09:04:23.000000 dpkits-1.2.7/LICENSE
+-rw-rw-rw-   0        0        0    12196 2024-05-28 03:21:12.304137 dpkits-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0    11652 2023-10-06 10:25:52.000000 dpkits-1.2.7/README.md
+-rw-rw-rw-   0        0        0      626 2024-05-28 03:14:18.000000 dpkits-1.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-28 03:21:12.307484 dpkits-1.2.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-28 03:21:12.226396 dpkits-1.2.7/src/
+drwxrwxrwx   0        0        0        0 2024-05-28 03:21:12.268340 dpkits-1.2.7/src/dpkits/
+-rw-rw-rw-   0        0        0      565 2024-01-11 08:02:54.000000 dpkits-1.2.7/src/dpkits/__init__.py
+-rw-rw-rw-   0        0        0    28970 2024-05-23 03:35:42.000000 dpkits-1.2.7/src/dpkits/ap_data_converter.py
+-rw-rw-rw-   0        0        0     9948 2023-10-04 08:35:50.000000 dpkits-1.2.7/src/dpkits/calculate_lsm.py
+-rw-rw-rw-   0        0        0    11069 2024-01-31 04:23:09.000000 dpkits-1.2.7/src/dpkits/codeframe_reader.py
+-rw-rw-rw-   0        0        0     5209 2024-05-06 08:45:27.000000 dpkits-1.2.7/src/dpkits/data_analysis.py
+-rw-rw-rw-   0        0        0     4428 2024-05-28 02:52:30.000000 dpkits-1.2.7/src/dpkits/data_processing.py
+-rw-rw-rw-   0        0        0     8198 2024-03-29 03:28:36.000000 dpkits-1.2.7/src/dpkits/data_transpose.py
+-rw-rw-rw-   0        0        0    26578 2024-05-10 10:00:29.000000 dpkits-1.2.7/src/dpkits/table_formater.py
+-rw-rw-rw-   0        0        0    67398 2024-05-23 09:51:47.000000 dpkits-1.2.7/src/dpkits/table_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-28 03:21:12.301661 dpkits-1.2.7/src/dpkits.egg-info/
+-rw-rw-rw-   0        0        0    12196 2024-05-28 03:21:12.000000 dpkits-1.2.7/src/dpkits.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2024-05-28 03:21:12.000000 dpkits-1.2.7/src/dpkits.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 03:21:12.000000 dpkits-1.2.7/src/dpkits.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-28 03:21:12.000000 dpkits-1.2.7/src/dpkits.egg-info/top_level.txt
```

### Comparing `dpkits-1.2.6/LICENSE` & `dpkits-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.6/PKG-INFO` & `dpkits-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpkits
-Version: 1.2.6
+Version: 1.2.7
 Summary: A small package for data processing
 Author-email: Hung Dao <hung.daotuan.1991@gmail.com>
 Project-URL: Homepage, https://github.com/HungDaoHD/packaging_dpkits
 Project-URL: Bug Tracker, https://github.com/HungDaoHD/packaging_dpkits/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dpkits-1.2.6/README.md` & `dpkits-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.6/pyproject.toml` & `dpkits-1.2.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dpkits"
-version = "1.2.6"
+version = "1.2.7"
 authors = [
   { name="Hung Dao", email="hung.daotuan.1991@gmail.com" },
 ]
 description = "A small package for data processing"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `dpkits-1.2.6/src/dpkits/__init__.py` & `dpkits-1.2.7/src/dpkits/__init__.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.6/src/dpkits/ap_data_converter.py` & `dpkits-1.2.7/src/dpkits/ap_data_converter.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.6/src/dpkits/calculate_lsm.py` & `dpkits-1.2.7/src/dpkits/calculate_lsm.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.6/src/dpkits/codeframe_reader.py` & `dpkits-1.2.7/src/dpkits/codeframe_reader.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.6/src/dpkits/data_analysis.py` & `dpkits-1.2.7/src/dpkits/data_analysis.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.6/src/dpkits/data_processing.py` & `dpkits-1.2.7/src/dpkits/data_processing.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
 import numpy as np
-
+from colorama import Fore
 
 
 class DataProcessing:
 
     def __init__(self):
         pass
 
@@ -77,22 +77,54 @@
         df_data.reset_index(drop=True, inplace=True)
         df_info.reset_index(drop=True, inplace=True)
 
         return df_data, df_info
 
 
 
-    def concept_evaluate(self, cpt_filename: str, ) -> (pd.DataFrame, dict):
+    @staticmethod
+    def merge_qres(*, df_data: pd.DataFrame, lst_merge: list, lst_to_merge: list, dk_code: int) -> pd.DataFrame:
+
+        if len(lst_merge) < len(lst_to_merge):
+            print(f"{Fore.RED}Merge_qres(error): Length of lst_merge should be greater than or equal length of lst_to_merge!!!\n"
+                  f"lst_merge = {lst_merge}\nlst_to_merge = {lst_to_merge}\nProcessing terminated!!!{Fore.RESET}")
+            exit()
+
+
+
+        def merge_row(sr_row: pd.Series, lst_col_name: list, dk: int) -> pd.Series:
+
+            lst_output = sr_row.reset_index(drop=True).drop_duplicates(keep='first').dropna().sort_values().values.tolist()
+            output_len = len(lst_col_name)
+
+            if len(lst_output) > 1 and dk in lst_output:
+                lst_output.remove(dk)
+
+            if len(lst_output) < output_len:
+                lst_output.extend([np.nan] * (output_len - len(lst_output)))
+
+            return pd.Series(data=lst_output, index=lst_col_name)
+
+        df_data[lst_merge] = df_data[lst_to_merge].apply(merge_row, lst_col_name=lst_merge, dk=dk_code, axis=1)
+
+        return df_data
+
+
+
+
+
+
+
+
+    @staticmethod
+    def concept_evaluate(cpt_filename: str, ) -> (pd.DataFrame, dict):
         # Here: May 16
         # 1. clean inputted concept
         # 2. create codeframe for each word for concept
         # 3. match verbatim to concept codeframe
         # 4. return dataframe with codes of the words in concept
 
-
-
-        
         return pd.DataFrame(), dict()  # dataframe & codelíst
```

### Comparing `dpkits-1.2.6/src/dpkits/data_transpose.py` & `dpkits-1.2.7/src/dpkits/data_transpose.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.6/src/dpkits/table_formater.py` & `dpkits-1.2.7/src/dpkits/table_formater.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.6/src/dpkits/table_generator.py` & `dpkits-1.2.7/src/dpkits/table_generator.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.6/src/dpkits.egg-info/PKG-INFO` & `dpkits-1.2.7/src/dpkits.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpkits
-Version: 1.2.6
+Version: 1.2.7
 Summary: A small package for data processing
 Author-email: Hung Dao <hung.daotuan.1991@gmail.com>
 Project-URL: Homepage, https://github.com/HungDaoHD/packaging_dpkits
 Project-URL: Bug Tracker, https://github.com/HungDaoHD/packaging_dpkits/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

