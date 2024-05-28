# Comparing `tmp/abstract_pandas-0.0.42.0.tar.gz` & `tmp/abstract_pandas-0.0.43.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_pandas-0.0.42.0.tar", last modified: Tue May 28 16:59:45 2024, max compression
+gzip compressed data, was "abstract_pandas-0.0.43.0.tar", last modified: Tue May 28 17:07:15 2024, max compression
```

## Comparing `abstract_pandas-0.0.42.0.tar` & `abstract_pandas-0.0.43.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-28 16:59:45.689192 abstract_pandas-0.0.42.0/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      732 2024-05-28 16:59:45.689192 abstract_pandas-0.0.42.0/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_pandas-0.0.42.0/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-28 16:59:45.689192 abstract_pandas-0.0.42.0/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     1036 2024-05-28 16:59:37.000000 abstract_pandas-0.0.42.0/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-28 16:59:45.689192 abstract_pandas-0.0.42.0/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-28 16:59:45.689192 abstract_pandas-0.0.42.0/src/abstract_pandas/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       29 2024-05-10 04:14:51.000000 abstract_pandas-0.0.42.0/src/abstract_pandas/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     5943 2024-05-10 08:14:17.000000 abstract_pandas-0.0.42.0/src/abstract_pandas/abstractLandManager.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     7395 2024-05-05 05:32:14.000000 abstract_pandas-0.0.42.0/src/abstract_pandas/depriciated.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     6290 2024-05-10 04:15:06.000000 abstract_pandas-0.0.42.0/src/abstract_pandas/excel_classes.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    20476 2024-05-05 07:05:13.000000 abstract_pandas-0.0.42.0/src/abstract_pandas/excel_gui.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    12527 2024-05-28 16:59:30.000000 abstract_pandas-0.0.42.0/src/abstract_pandas/excel_module.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    15024 2024-05-28 06:39:39.000000 abstract_pandas-0.0.42.0/src/abstract_pandas/file_utils.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     8233 2024-05-06 03:12:41.000000 abstract_pandas-0.0.42.0/src/abstract_pandas/functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     7459 2024-05-06 03:49:09.000000 abstract_pandas-0.0.42.0/src/abstract_pandas/general_functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     1745 2024-05-10 04:14:25.000000 abstract_pandas-0.0.42.0/src/abstract_pandas/location_functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     2724 2024-05-10 05:00:14.000000 abstract_pandas-0.0.42.0/src/abstract_pandas/proj_tools.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     8552 2024-05-10 04:14:42.000000 abstract_pandas-0.0.42.0/src/abstract_pandas/query_tools.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-28 16:59:45.689192 abstract_pandas-0.0.42.0/src/abstract_pandas.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      732 2024-05-28 16:59:45.000000 abstract_pandas-0.0.42.0/src/abstract_pandas.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      667 2024-05-28 16:59:45.000000 abstract_pandas-0.0.42.0/src/abstract_pandas.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-28 16:59:45.000000 abstract_pandas-0.0.42.0/src/abstract_pandas.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      108 2024-05-28 16:59:45.000000 abstract_pandas-0.0.42.0/src/abstract_pandas.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-28 16:59:45.000000 abstract_pandas-0.0.42.0/src/abstract_pandas.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-28 17:07:15.522829 abstract_pandas-0.0.43.0/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      732 2024-05-28 17:07:15.522829 abstract_pandas-0.0.43.0/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_pandas-0.0.43.0/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-28 17:07:15.522829 abstract_pandas-0.0.43.0/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     1036 2024-05-28 17:07:08.000000 abstract_pandas-0.0.43.0/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-28 17:07:15.518829 abstract_pandas-0.0.43.0/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-28 17:07:15.522829 abstract_pandas-0.0.43.0/src/abstract_pandas/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       29 2024-05-10 04:14:51.000000 abstract_pandas-0.0.43.0/src/abstract_pandas/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     5943 2024-05-10 08:14:17.000000 abstract_pandas-0.0.43.0/src/abstract_pandas/abstractLandManager.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     7395 2024-05-05 05:32:14.000000 abstract_pandas-0.0.43.0/src/abstract_pandas/depriciated.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     6290 2024-05-10 04:15:06.000000 abstract_pandas-0.0.43.0/src/abstract_pandas/excel_classes.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    20476 2024-05-05 07:05:13.000000 abstract_pandas-0.0.43.0/src/abstract_pandas/excel_gui.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    12691 2024-05-28 17:07:02.000000 abstract_pandas-0.0.43.0/src/abstract_pandas/excel_module.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    15024 2024-05-28 06:39:39.000000 abstract_pandas-0.0.43.0/src/abstract_pandas/file_utils.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     8233 2024-05-06 03:12:41.000000 abstract_pandas-0.0.43.0/src/abstract_pandas/functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     7459 2024-05-06 03:49:09.000000 abstract_pandas-0.0.43.0/src/abstract_pandas/general_functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     1745 2024-05-10 04:14:25.000000 abstract_pandas-0.0.43.0/src/abstract_pandas/location_functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     2724 2024-05-10 05:00:14.000000 abstract_pandas-0.0.43.0/src/abstract_pandas/proj_tools.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     8552 2024-05-10 04:14:42.000000 abstract_pandas-0.0.43.0/src/abstract_pandas/query_tools.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-28 17:07:15.522829 abstract_pandas-0.0.43.0/src/abstract_pandas.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      732 2024-05-28 17:07:15.000000 abstract_pandas-0.0.43.0/src/abstract_pandas.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      667 2024-05-28 17:07:15.000000 abstract_pandas-0.0.43.0/src/abstract_pandas.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-28 17:07:15.000000 abstract_pandas-0.0.43.0/src/abstract_pandas.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      108 2024-05-28 17:07:15.000000 abstract_pandas-0.0.43.0/src/abstract_pandas.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-28 17:07:15.000000 abstract_pandas-0.0.43.0/src/abstract_pandas.egg-info/top_level.txt
```

### Comparing `abstract_pandas-0.0.42.0/PKG-INFO` & `abstract_pandas-0.0.43.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_pandas
-Version: 0.0.42.0
+Version: 0.0.43.0
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_pandas-0.0.42.0/setup.py` & `abstract_pandas-0.0.43.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_pandas',
-    version='0.0.42.0',
+    version='0.0.43.0',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `abstract_pandas-0.0.42.0/src/abstract_pandas/abstractLandManager.py` & `abstract_pandas-0.0.43.0/src/abstract_pandas/abstractLandManager.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.42.0/src/abstract_pandas/depriciated.py` & `abstract_pandas-0.0.43.0/src/abstract_pandas/depriciated.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.42.0/src/abstract_pandas/excel_classes.py` & `abstract_pandas-0.0.43.0/src/abstract_pandas/excel_classes.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.42.0/src/abstract_pandas/excel_gui.py` & `abstract_pandas-0.0.43.0/src/abstract_pandas/excel_gui.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.42.0/src/abstract_pandas/excel_module.py` & `abstract_pandas-0.0.43.0/src/abstract_pandas/excel_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,19 @@
     """
     if column_name not in df.columns:
         df[column_name] = default_value
     else:
         print(f"Column '{column_name}' already exists in the DataFrame. No changes made.")
 
     return df
+def does_not_equal_in_list(obj,list_obj):
+    for list_obj in list_objs:
+        if obj == list_obj:
+            return False
+    return True
 def update_or_append_data(df_new_data=None, df_existing_data=None, search_column=None, search_value=None, clear_duplicates=False):
     df_new = get_df(df_new_data)
     df_existing = get_df(df_existing_data)
     
     if df_existing.empty:
         return df_new
 
@@ -58,15 +63,15 @@
         if isinstance(search_column, list) and isinstance(search_value, list):
             mask = pd.Series(True, index=df_existing.index)
             for col, val in zip(search_column, search_value):
                 mask &= (df_existing[col] == val)
         else:
             mask = (df_existing[search_column] == search_value)
 
-        if mask not in ['',' ',[],None,'none','None']:
+        if does_not_equal_in_list(mask,['',' ',[],None,'none','None']):
             # Update existing rows based on mask
             for col in df_new.columns:
                 df_existing.loc[mask, col] = df_new.loc[df_new.index[0], col]
             print(f"Updated rows where {search_column} matches {search_value}.")
         else:
             # Append new data if no matching row is found
             df_existing = pd.concat([df_existing, df_new], ignore_index=True)
```

### Comparing `abstract_pandas-0.0.42.0/src/abstract_pandas/file_utils.py` & `abstract_pandas-0.0.43.0/src/abstract_pandas/file_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.42.0/src/abstract_pandas/functions.py` & `abstract_pandas-0.0.43.0/src/abstract_pandas/functions.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.42.0/src/abstract_pandas/general_functions.py` & `abstract_pandas-0.0.43.0/src/abstract_pandas/general_functions.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.42.0/src/abstract_pandas/location_functions.py` & `abstract_pandas-0.0.43.0/src/abstract_pandas/location_functions.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.42.0/src/abstract_pandas/proj_tools.py` & `abstract_pandas-0.0.43.0/src/abstract_pandas/proj_tools.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.42.0/src/abstract_pandas/query_tools.py` & `abstract_pandas-0.0.43.0/src/abstract_pandas/query_tools.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.42.0/src/abstract_pandas.egg-info/PKG-INFO` & `abstract_pandas-0.0.43.0/src/abstract_pandas.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_pandas
-Version: 0.0.42.0
+Version: 0.0.43.0
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_pandas-0.0.42.0/src/abstract_pandas.egg-info/SOURCES.txt` & `abstract_pandas-0.0.43.0/src/abstract_pandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

