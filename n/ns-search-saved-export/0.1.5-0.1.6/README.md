# Comparing `tmp/ns_search_saved_export-0.1.5.tar.gz` & `tmp/ns_search_saved_export-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ns_search_saved_export-0.1.5.tar", last modified: Tue May 28 00:44:40 2024, max compression
+gzip compressed data, was "ns_search_saved_export-0.1.6.tar", last modified: Tue May 28 01:05:03 2024, max compression
```

## Comparing `ns_search_saved_export-0.1.5.tar` & `ns_search_saved_export-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 00:44:40.569929 ns_search_saved_export-0.1.5/
--rw-rw-rw-   0        0        0      171 2024-05-25 23:39:23.000000 ns_search_saved_export-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     1615 2024-05-28 00:44:40.568782 ns_search_saved_export-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      989 2024-05-26 17:14:05.000000 ns_search_saved_export-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 00:44:40.565870 ns_search_saved_export-0.1.5/Tests/
--rw-rw-rw-   0        0        0        0 2024-05-25 23:37:11.000000 ns_search_saved_export-0.1.5/Tests/__init__.py
--rw-rw-rw-   0        0        0      954 2024-05-26 17:33:39.000000 ns_search_saved_export-0.1.5/Tests/test_main.py
--rw-rw-rw-   0        0        0     2660 2024-05-26 17:29:33.000000 ns_search_saved_export-0.1.5/Tests/test_ns_search_saved_export.py
--rw-rw-rw-   0        0        0      948 2024-05-26 16:45:44.000000 ns_search_saved_export-0.1.5/Tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-28 00:44:40.550929 ns_search_saved_export-0.1.5/ns_search_saved_export/
--rw-rw-rw-   0        0        0      173 2024-05-25 23:49:02.000000 ns_search_saved_export-0.1.5/ns_search_saved_export/__init__.py
--rw-rw-rw-   0        0        0     4812 2024-05-28 00:38:23.000000 ns_search_saved_export-0.1.5/ns_search_saved_export/ns_search_saved_export.py
--rw-rw-rw-   0        0        0     1038 2024-05-25 23:43:38.000000 ns_search_saved_export-0.1.5/ns_search_saved_export/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-28 00:44:40.567611 ns_search_saved_export-0.1.5/ns_search_saved_export.egg-info/
--rw-rw-rw-   0        0        0     1615 2024-05-28 00:44:40.000000 ns_search_saved_export-0.1.5/ns_search_saved_export.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      556 2024-05-28 00:44:40.000000 ns_search_saved_export-0.1.5/ns_search_saved_export.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 00:44:40.000000 ns_search_saved_export-0.1.5/ns_search_saved_export.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-05-28 00:44:40.000000 ns_search_saved_export-0.1.5/ns_search_saved_export.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-05-28 00:44:40.000000 ns_search_saved_export-0.1.5/ns_search_saved_export.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      497 2024-05-26 18:01:07.000000 ns_search_saved_export-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-28 00:44:40.570486 ns_search_saved_export-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      799 2024-05-28 00:38:40.000000 ns_search_saved_export-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 01:05:03.440539 ns_search_saved_export-0.1.6/
+-rw-rw-rw-   0        0        0      171 2024-05-25 23:39:23.000000 ns_search_saved_export-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     1615 2024-05-28 01:05:03.439357 ns_search_saved_export-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      989 2024-05-26 17:14:05.000000 ns_search_saved_export-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 01:05:03.437178 ns_search_saved_export-0.1.6/Tests/
+-rw-rw-rw-   0        0        0        0 2024-05-25 23:37:11.000000 ns_search_saved_export-0.1.6/Tests/__init__.py
+-rw-rw-rw-   0        0        0      954 2024-05-26 17:33:39.000000 ns_search_saved_export-0.1.6/Tests/test_main.py
+-rw-rw-rw-   0        0        0     2660 2024-05-26 17:29:33.000000 ns_search_saved_export-0.1.6/Tests/test_ns_search_saved_export.py
+-rw-rw-rw-   0        0        0      948 2024-05-26 16:45:44.000000 ns_search_saved_export-0.1.6/Tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-28 01:05:03.392933 ns_search_saved_export-0.1.6/ns_search_saved_export/
+-rw-rw-rw-   0        0        0      173 2024-05-25 23:49:02.000000 ns_search_saved_export-0.1.6/ns_search_saved_export/__init__.py
+-rw-rw-rw-   0        0        0     4807 2024-05-28 01:04:35.000000 ns_search_saved_export-0.1.6/ns_search_saved_export/ns_search_saved_export.py
+-rw-rw-rw-   0        0        0     1038 2024-05-25 23:43:38.000000 ns_search_saved_export-0.1.6/ns_search_saved_export/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-28 01:05:03.438310 ns_search_saved_export-0.1.6/ns_search_saved_export.egg-info/
+-rw-rw-rw-   0        0        0     1615 2024-05-28 01:05:03.000000 ns_search_saved_export-0.1.6/ns_search_saved_export.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2024-05-28 01:05:03.000000 ns_search_saved_export-0.1.6/ns_search_saved_export.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 01:05:03.000000 ns_search_saved_export-0.1.6/ns_search_saved_export.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-28 01:05:03.000000 ns_search_saved_export-0.1.6/ns_search_saved_export.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-05-28 01:05:03.000000 ns_search_saved_export-0.1.6/ns_search_saved_export.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      497 2024-05-26 18:01:07.000000 ns_search_saved_export-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-28 01:05:03.441043 ns_search_saved_export-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      799 2024-05-28 01:04:46.000000 ns_search_saved_export-0.1.6/setup.py
```

### Comparing `ns_search_saved_export-0.1.5/PKG-INFO` & `ns_search_saved_export-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_search_saved_export
-Version: 0.1.5
+Version: 0.1.6
 Summary: A library for interacting with NetSuite API and exporting data
 Home-page: https://github.com/gildder/netsuite-search-saved-export
 Author: Gildder
 Author-email: gildder@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ns_search_saved_export-0.1.5/README.md` & `ns_search_saved_export-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.5/Tests/test_main.py` & `ns_search_saved_export-0.1.6/Tests/test_main.py`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.5/Tests/test_ns_search_saved_export.py` & `ns_search_saved_export-0.1.6/Tests/test_ns_search_saved_export.py`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.5/Tests/test_utils.py` & `ns_search_saved_export-0.1.6/Tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.5/ns_search_saved_export/ns_search_saved_export.py` & `ns_search_saved_export-0.1.6/ns_search_saved_export/ns_search_saved_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             json_data (dict): Data obtained in the POST response
 
         Returns:
             list: List of saved search data
         """
         # Export original JSON data to a JSON file
         with open(self.search_id, 'w', encoding='utf-8') as json_file:
-            json.dump(json_data, self.search_id, ensure_ascii=False, indent=4)
+            json.dump(json_data, json_file, ensure_ascii=False, indent=4)
         
         matrix = []
         headers = set()
         for index, data in enumerate(json_data['results']):
             row = []
             values = data['values']
```

### Comparing `ns_search_saved_export-0.1.5/ns_search_saved_export/utils.py` & `ns_search_saved_export-0.1.6/ns_search_saved_export/utils.py`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.5/ns_search_saved_export.egg-info/PKG-INFO` & `ns_search_saved_export-0.1.6/ns_search_saved_export.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_search_saved_export
-Version: 0.1.5
+Version: 0.1.6
 Summary: A library for interacting with NetSuite API and exporting data
 Home-page: https://github.com/gildder/netsuite-search-saved-export
 Author: Gildder
 Author-email: gildder@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ns_search_saved_export-0.1.5/ns_search_saved_export.egg-info/SOURCES.txt` & `ns_search_saved_export-0.1.6/ns_search_saved_export.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.5/setup.py` & `ns_search_saved_export-0.1.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ns_search_saved_export',
-    version='0.1.5',
+    version='0.1.6',
     description='A library for interacting with NetSuite API and exporting data',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Gildder',
     author_email='gildder@outlook.com',
     url='https://github.com/gildder/netsuite-search-saved-export',
     packages=find_packages(),
```

