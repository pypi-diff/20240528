# Comparing `tmp/abstract_pandas-0.0.0.98.tar.gz` & `tmp/abstract_pandas-0.0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_pandas-0.0.0.98.tar", last modified: Tue May 28 06:56:26 2024, max compression
+gzip compressed data, was "abstract_pandas-0.0.0.99.tar", last modified: Tue May 28 06:59:12 2024, max compression
```

## Comparing `abstract_pandas-0.0.0.98.tar` & `abstract_pandas-0.0.0.99.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-28 06:56:26.953765 abstract_pandas-0.0.0.98/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      732 2024-05-28 06:56:26.953765 abstract_pandas-0.0.0.98/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_pandas-0.0.0.98/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-28 06:56:26.953765 abstract_pandas-0.0.0.98/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     1036 2024-05-28 06:54:46.000000 abstract_pandas-0.0.0.98/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-28 06:56:26.949765 abstract_pandas-0.0.0.98/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-28 06:56:26.949765 abstract_pandas-0.0.0.98/src/abstract_pandas/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       29 2024-05-10 04:14:51.000000 abstract_pandas-0.0.0.98/src/abstract_pandas/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     5943 2024-05-10 08:14:17.000000 abstract_pandas-0.0.0.98/src/abstract_pandas/abstractLandManager.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     7395 2024-05-05 05:32:14.000000 abstract_pandas-0.0.0.98/src/abstract_pandas/depriciated.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     6290 2024-05-10 04:15:06.000000 abstract_pandas-0.0.0.98/src/abstract_pandas/excel_classes.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    20476 2024-05-05 07:05:13.000000 abstract_pandas-0.0.0.98/src/abstract_pandas/excel_gui.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    12495 2024-05-10 04:19:05.000000 abstract_pandas-0.0.0.98/src/abstract_pandas/excel_module.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    15024 2024-05-28 06:39:39.000000 abstract_pandas-0.0.0.98/src/abstract_pandas/file_utils.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     8233 2024-05-06 03:12:41.000000 abstract_pandas-0.0.0.98/src/abstract_pandas/functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     7459 2024-05-06 03:49:09.000000 abstract_pandas-0.0.0.98/src/abstract_pandas/general_functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     1745 2024-05-10 04:14:25.000000 abstract_pandas-0.0.0.98/src/abstract_pandas/location_functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     2724 2024-05-10 05:00:14.000000 abstract_pandas-0.0.0.98/src/abstract_pandas/proj_tools.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     8552 2024-05-10 04:14:42.000000 abstract_pandas-0.0.0.98/src/abstract_pandas/query_tools.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-28 06:56:26.949765 abstract_pandas-0.0.0.98/src/abstract_pandas.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      732 2024-05-28 06:56:26.000000 abstract_pandas-0.0.0.98/src/abstract_pandas.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      667 2024-05-28 06:56:26.000000 abstract_pandas-0.0.0.98/src/abstract_pandas.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-28 06:56:26.000000 abstract_pandas-0.0.0.98/src/abstract_pandas.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      108 2024-05-28 06:56:26.000000 abstract_pandas-0.0.0.98/src/abstract_pandas.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-28 06:56:26.000000 abstract_pandas-0.0.0.98/src/abstract_pandas.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-28 06:59:12.327555 abstract_pandas-0.0.0.99/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      732 2024-05-28 06:59:12.327555 abstract_pandas-0.0.0.99/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_pandas-0.0.0.99/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-28 06:59:12.327555 abstract_pandas-0.0.0.99/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     1036 2024-05-28 06:59:06.000000 abstract_pandas-0.0.0.99/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-28 06:59:12.323555 abstract_pandas-0.0.0.99/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-28 06:59:12.327555 abstract_pandas-0.0.0.99/src/abstract_pandas/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       29 2024-05-10 04:14:51.000000 abstract_pandas-0.0.0.99/src/abstract_pandas/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     5943 2024-05-10 08:14:17.000000 abstract_pandas-0.0.0.99/src/abstract_pandas/abstractLandManager.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     7395 2024-05-05 05:32:14.000000 abstract_pandas-0.0.0.99/src/abstract_pandas/depriciated.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     6290 2024-05-10 04:15:06.000000 abstract_pandas-0.0.0.99/src/abstract_pandas/excel_classes.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    20476 2024-05-05 07:05:13.000000 abstract_pandas-0.0.0.99/src/abstract_pandas/excel_gui.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    12519 2024-05-28 06:58:53.000000 abstract_pandas-0.0.0.99/src/abstract_pandas/excel_module.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    15024 2024-05-28 06:39:39.000000 abstract_pandas-0.0.0.99/src/abstract_pandas/file_utils.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     8233 2024-05-06 03:12:41.000000 abstract_pandas-0.0.0.99/src/abstract_pandas/functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     7459 2024-05-06 03:49:09.000000 abstract_pandas-0.0.0.99/src/abstract_pandas/general_functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     1745 2024-05-10 04:14:25.000000 abstract_pandas-0.0.0.99/src/abstract_pandas/location_functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     2724 2024-05-10 05:00:14.000000 abstract_pandas-0.0.0.99/src/abstract_pandas/proj_tools.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     8552 2024-05-10 04:14:42.000000 abstract_pandas-0.0.0.99/src/abstract_pandas/query_tools.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-28 06:59:12.327555 abstract_pandas-0.0.0.99/src/abstract_pandas.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      732 2024-05-28 06:59:12.000000 abstract_pandas-0.0.0.99/src/abstract_pandas.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      667 2024-05-28 06:59:12.000000 abstract_pandas-0.0.0.99/src/abstract_pandas.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-28 06:59:12.000000 abstract_pandas-0.0.0.99/src/abstract_pandas.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      108 2024-05-28 06:59:12.000000 abstract_pandas-0.0.0.99/src/abstract_pandas.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-28 06:59:12.000000 abstract_pandas-0.0.0.99/src/abstract_pandas.egg-info/top_level.txt
```

### Comparing `abstract_pandas-0.0.0.98/PKG-INFO` & `abstract_pandas-0.0.0.99/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_pandas
-Version: 0.0.0.98
+Version: 0.0.0.99
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_pandas-0.0.0.98/setup.py` & `abstract_pandas-0.0.0.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_pandas',
-    version='0.0.0.98',
+    version='0.0.0.99',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `abstract_pandas-0.0.0.98/src/abstract_pandas/abstractLandManager.py` & `abstract_pandas-0.0.0.99/src/abstract_pandas/abstractLandManager.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.98/src/abstract_pandas/depriciated.py` & `abstract_pandas-0.0.0.99/src/abstract_pandas/depriciated.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.98/src/abstract_pandas/excel_classes.py` & `abstract_pandas-0.0.0.99/src/abstract_pandas/excel_classes.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.98/src/abstract_pandas/excel_gui.py` & `abstract_pandas-0.0.0.99/src/abstract_pandas/excel_gui.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.98/src/abstract_pandas/excel_module.py` & `abstract_pandas-0.0.0.99/src/abstract_pandas/excel_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         print(f"Column '{column_name}' already exists in the DataFrame. No changes made.")
 
     return df
 def update_or_append_data(df_new_data=None, df_existing_data=None, search_column=None, search_value=None, clear_duplicates=False):
     df_new = get_df(df_new_data)
     df_existing = get_df(df_existing_data)
     
-    if df_existing.empty:
+    if df_existing is None or len(df_existing)<1:
         return df_new
 
     # Ensure new data columns exist in the existing dataframe, add if not
     for col in df_new.columns:
         if col not in df_existing.columns:
             df_existing[col] = pd.NA  # Use pd.NA for missing data
```

### Comparing `abstract_pandas-0.0.0.98/src/abstract_pandas/file_utils.py` & `abstract_pandas-0.0.0.99/src/abstract_pandas/file_utils.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.98/src/abstract_pandas/functions.py` & `abstract_pandas-0.0.0.99/src/abstract_pandas/functions.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.98/src/abstract_pandas/general_functions.py` & `abstract_pandas-0.0.0.99/src/abstract_pandas/general_functions.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.98/src/abstract_pandas/location_functions.py` & `abstract_pandas-0.0.0.99/src/abstract_pandas/location_functions.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.98/src/abstract_pandas/proj_tools.py` & `abstract_pandas-0.0.0.99/src/abstract_pandas/proj_tools.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.98/src/abstract_pandas/query_tools.py` & `abstract_pandas-0.0.0.99/src/abstract_pandas/query_tools.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.98/src/abstract_pandas.egg-info/PKG-INFO` & `abstract_pandas-0.0.0.99/src/abstract_pandas.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_pandas
-Version: 0.0.0.98
+Version: 0.0.0.99
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_pandas-0.0.0.98/src/abstract_pandas.egg-info/SOURCES.txt` & `abstract_pandas-0.0.0.99/src/abstract_pandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

