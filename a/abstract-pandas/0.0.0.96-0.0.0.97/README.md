# Comparing `tmp/abstract_pandas-0.0.0.96.tar.gz` & `tmp/abstract_pandas-0.0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_pandas-0.0.0.96.tar", last modified: Wed May 15 17:46:18 2024, max compression
+gzip compressed data, was "abstract_pandas-0.0.0.97.tar", last modified: Tue May 28 06:52:46 2024, max compression
```

## Comparing `abstract_pandas-0.0.0.96.tar` & `abstract_pandas-0.0.0.97.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-15 17:46:18.517767 abstract_pandas-0.0.0.96/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      732 2024-05-15 17:46:18.517767 abstract_pandas-0.0.0.96/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_pandas-0.0.0.96/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-15 17:46:18.517767 abstract_pandas-0.0.0.96/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     1036 2024-05-15 17:45:46.000000 abstract_pandas-0.0.0.96/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-15 17:46:18.513767 abstract_pandas-0.0.0.96/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-15 17:46:18.513767 abstract_pandas-0.0.0.96/src/abstract_pandas/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       29 2024-05-10 04:14:51.000000 abstract_pandas-0.0.0.96/src/abstract_pandas/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     5943 2024-05-10 08:14:17.000000 abstract_pandas-0.0.0.96/src/abstract_pandas/abstractLandManager.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     7395 2024-05-05 05:32:14.000000 abstract_pandas-0.0.0.96/src/abstract_pandas/depriciated.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     6290 2024-05-10 04:15:06.000000 abstract_pandas-0.0.0.96/src/abstract_pandas/excel_classes.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    20476 2024-05-05 07:05:13.000000 abstract_pandas-0.0.0.96/src/abstract_pandas/excel_gui.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    12495 2024-05-10 04:19:05.000000 abstract_pandas-0.0.0.96/src/abstract_pandas/excel_module.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    14996 2024-05-10 05:10:26.000000 abstract_pandas-0.0.0.96/src/abstract_pandas/file_utils.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     8233 2024-05-06 03:12:41.000000 abstract_pandas-0.0.0.96/src/abstract_pandas/functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     7459 2024-05-06 03:49:09.000000 abstract_pandas-0.0.0.96/src/abstract_pandas/general_functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     1745 2024-05-10 04:14:25.000000 abstract_pandas-0.0.0.96/src/abstract_pandas/location_functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     2724 2024-05-10 05:00:14.000000 abstract_pandas-0.0.0.96/src/abstract_pandas/proj_tools.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     8552 2024-05-10 04:14:42.000000 abstract_pandas-0.0.0.96/src/abstract_pandas/query_tools.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-15 17:46:18.517767 abstract_pandas-0.0.0.96/src/abstract_pandas.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      732 2024-05-15 17:46:18.000000 abstract_pandas-0.0.0.96/src/abstract_pandas.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      667 2024-05-15 17:46:18.000000 abstract_pandas-0.0.0.96/src/abstract_pandas.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-15 17:46:18.000000 abstract_pandas-0.0.0.96/src/abstract_pandas.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      108 2024-05-15 17:46:18.000000 abstract_pandas-0.0.0.96/src/abstract_pandas.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-15 17:46:18.000000 abstract_pandas-0.0.0.96/src/abstract_pandas.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-28 06:52:46.840723 abstract_pandas-0.0.0.97/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      732 2024-05-28 06:52:46.840723 abstract_pandas-0.0.0.97/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_pandas-0.0.0.97/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-05-28 06:52:46.840723 abstract_pandas-0.0.0.97/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     1036 2024-05-28 06:39:46.000000 abstract_pandas-0.0.0.97/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-28 06:52:46.840723 abstract_pandas-0.0.0.97/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-28 06:52:46.840723 abstract_pandas-0.0.0.97/src/abstract_pandas/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       29 2024-05-10 04:14:51.000000 abstract_pandas-0.0.0.97/src/abstract_pandas/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     5943 2024-05-10 08:14:17.000000 abstract_pandas-0.0.0.97/src/abstract_pandas/abstractLandManager.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     7395 2024-05-05 05:32:14.000000 abstract_pandas-0.0.0.97/src/abstract_pandas/depriciated.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     6290 2024-05-10 04:15:06.000000 abstract_pandas-0.0.0.97/src/abstract_pandas/excel_classes.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    20476 2024-05-05 07:05:13.000000 abstract_pandas-0.0.0.97/src/abstract_pandas/excel_gui.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    12495 2024-05-10 04:19:05.000000 abstract_pandas-0.0.0.97/src/abstract_pandas/excel_module.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    15024 2024-05-28 06:39:39.000000 abstract_pandas-0.0.0.97/src/abstract_pandas/file_utils.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     8233 2024-05-06 03:12:41.000000 abstract_pandas-0.0.0.97/src/abstract_pandas/functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     7459 2024-05-06 03:49:09.000000 abstract_pandas-0.0.0.97/src/abstract_pandas/general_functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     1745 2024-05-10 04:14:25.000000 abstract_pandas-0.0.0.97/src/abstract_pandas/location_functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     2724 2024-05-10 05:00:14.000000 abstract_pandas-0.0.0.97/src/abstract_pandas/proj_tools.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     8552 2024-05-10 04:14:42.000000 abstract_pandas-0.0.0.97/src/abstract_pandas/query_tools.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-05-28 06:52:46.840723 abstract_pandas-0.0.0.97/src/abstract_pandas.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      732 2024-05-28 06:52:46.000000 abstract_pandas-0.0.0.97/src/abstract_pandas.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      667 2024-05-28 06:52:46.000000 abstract_pandas-0.0.0.97/src/abstract_pandas.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-05-28 06:52:46.000000 abstract_pandas-0.0.0.97/src/abstract_pandas.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      108 2024-05-28 06:52:46.000000 abstract_pandas-0.0.0.97/src/abstract_pandas.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-05-28 06:52:46.000000 abstract_pandas-0.0.0.97/src/abstract_pandas.egg-info/top_level.txt
```

### Comparing `abstract_pandas-0.0.0.96/PKG-INFO` & `abstract_pandas-0.0.0.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_pandas
-Version: 0.0.0.96
+Version: 0.0.0.97
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_pandas-0.0.0.96/setup.py` & `abstract_pandas-0.0.0.97/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_pandas',
-    version='0.0.0.96',
+    version='0.0.0.97',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `abstract_pandas-0.0.0.96/src/abstract_pandas/abstractLandManager.py` & `abstract_pandas-0.0.0.97/src/abstract_pandas/abstractLandManager.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.96/src/abstract_pandas/depriciated.py` & `abstract_pandas-0.0.0.97/src/abstract_pandas/depriciated.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.96/src/abstract_pandas/excel_classes.py` & `abstract_pandas-0.0.0.97/src/abstract_pandas/excel_classes.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.96/src/abstract_pandas/excel_gui.py` & `abstract_pandas-0.0.0.97/src/abstract_pandas/excel_gui.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.96/src/abstract_pandas/excel_module.py` & `abstract_pandas-0.0.0.97/src/abstract_pandas/excel_module.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.96/src/abstract_pandas/file_utils.py` & `abstract_pandas-0.0.0.97/src/abstract_pandas/file_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 def source_ext(typ=None):
     source_js = {'.parquet':'pyarrow','.txt':'python','.xlsx':'openpyxl','.xls':'openpyxl','.xlsb':'pyxlsb','.ods':'odf','.geojson':'GeoJSON'}
     if typ:
         source_js = source_js.get(typ)
     return source_js
 def is_file(file_path):
-    if file_path and isinstance(file_path, str) and os.path.isfile(file_path):
+    if file_path not in ['',' ',None,'None'] and isinstance(file_path, str) and os.path.isfile(file_path):
         return os.path.splitext(file_path)[-1]
 def isDataFrame(obj):
     return isinstance(obj, pd.DataFrame)
 def create_dataframe(new_data=None,columns=None):
     if isDataFrame(new_data):
         return new_data
     new_data = new_data or {}
```

### Comparing `abstract_pandas-0.0.0.96/src/abstract_pandas/functions.py` & `abstract_pandas-0.0.0.97/src/abstract_pandas/functions.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.96/src/abstract_pandas/general_functions.py` & `abstract_pandas-0.0.0.97/src/abstract_pandas/general_functions.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.96/src/abstract_pandas/location_functions.py` & `abstract_pandas-0.0.0.97/src/abstract_pandas/location_functions.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.96/src/abstract_pandas/proj_tools.py` & `abstract_pandas-0.0.0.97/src/abstract_pandas/proj_tools.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.96/src/abstract_pandas/query_tools.py` & `abstract_pandas-0.0.0.97/src/abstract_pandas/query_tools.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.96/src/abstract_pandas.egg-info/PKG-INFO` & `abstract_pandas-0.0.0.97/src/abstract_pandas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_pandas
-Version: 0.0.0.96
+Version: 0.0.0.97
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_pandas-0.0.0.96/src/abstract_pandas.egg-info/SOURCES.txt` & `abstract_pandas-0.0.0.97/src/abstract_pandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

