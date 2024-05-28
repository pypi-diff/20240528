# Comparing `tmp/ns_search_saved_export-0.1.7.tar.gz` & `tmp/ns_search_saved_export-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ns_search_saved_export-0.1.7.tar", last modified: Tue May 28 01:50:44 2024, max compression
+gzip compressed data, was "ns_search_saved_export-0.1.8.tar", last modified: Tue May 28 02:03:50 2024, max compression
```

## Comparing `ns_search_saved_export-0.1.7.tar` & `ns_search_saved_export-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 01:50:44.241357 ns_search_saved_export-0.1.7/
--rw-rw-rw-   0        0        0      171 2024-05-25 23:39:23.000000 ns_search_saved_export-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     1615 2024-05-28 01:50:44.240238 ns_search_saved_export-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      989 2024-05-26 17:14:05.000000 ns_search_saved_export-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 01:50:44.216366 ns_search_saved_export-0.1.7/Tests/
--rw-rw-rw-   0        0        0        0 2024-05-25 23:37:11.000000 ns_search_saved_export-0.1.7/Tests/__init__.py
--rw-rw-rw-   0        0        0      954 2024-05-26 17:33:39.000000 ns_search_saved_export-0.1.7/Tests/test_main.py
--rw-rw-rw-   0        0        0     2660 2024-05-26 17:29:33.000000 ns_search_saved_export-0.1.7/Tests/test_ns_search_saved_export.py
--rw-rw-rw-   0        0        0      948 2024-05-26 16:45:44.000000 ns_search_saved_export-0.1.7/Tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-28 01:50:44.185380 ns_search_saved_export-0.1.7/ns_search_saved_export/
--rw-rw-rw-   0        0        0      173 2024-05-25 23:49:02.000000 ns_search_saved_export-0.1.7/ns_search_saved_export/__init__.py
--rw-rw-rw-   0        0        0     5014 2024-05-28 01:50:30.000000 ns_search_saved_export-0.1.7/ns_search_saved_export/ns_search_saved_export.py
--rw-rw-rw-   0        0        0     1038 2024-05-25 23:43:38.000000 ns_search_saved_export-0.1.7/ns_search_saved_export/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-28 01:50:44.217483 ns_search_saved_export-0.1.7/ns_search_saved_export.egg-info/
--rw-rw-rw-   0        0        0     1615 2024-05-28 01:50:44.000000 ns_search_saved_export-0.1.7/ns_search_saved_export.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      556 2024-05-28 01:50:44.000000 ns_search_saved_export-0.1.7/ns_search_saved_export.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 01:50:44.000000 ns_search_saved_export-0.1.7/ns_search_saved_export.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-05-28 01:50:44.000000 ns_search_saved_export-0.1.7/ns_search_saved_export.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-05-28 01:50:44.000000 ns_search_saved_export-0.1.7/ns_search_saved_export.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      497 2024-05-26 18:01:07.000000 ns_search_saved_export-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-28 01:50:44.241861 ns_search_saved_export-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      799 2024-05-28 01:46:15.000000 ns_search_saved_export-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 02:03:50.816044 ns_search_saved_export-0.1.8/
+-rw-rw-rw-   0        0        0      171 2024-05-25 23:39:23.000000 ns_search_saved_export-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     1615 2024-05-28 02:03:50.814937 ns_search_saved_export-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      989 2024-05-26 17:14:05.000000 ns_search_saved_export-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 02:03:50.812629 ns_search_saved_export-0.1.8/Tests/
+-rw-rw-rw-   0        0        0        0 2024-05-25 23:37:11.000000 ns_search_saved_export-0.1.8/Tests/__init__.py
+-rw-rw-rw-   0        0        0      954 2024-05-26 17:33:39.000000 ns_search_saved_export-0.1.8/Tests/test_main.py
+-rw-rw-rw-   0        0        0     2660 2024-05-26 17:29:33.000000 ns_search_saved_export-0.1.8/Tests/test_ns_search_saved_export.py
+-rw-rw-rw-   0        0        0      948 2024-05-26 16:45:44.000000 ns_search_saved_export-0.1.8/Tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-28 02:03:50.787903 ns_search_saved_export-0.1.8/ns_search_saved_export/
+-rw-rw-rw-   0        0        0      173 2024-05-25 23:49:02.000000 ns_search_saved_export-0.1.8/ns_search_saved_export/__init__.py
+-rw-rw-rw-   0        0        0     5014 2024-05-28 02:02:29.000000 ns_search_saved_export-0.1.8/ns_search_saved_export/ns_search_saved_export.py
+-rw-rw-rw-   0        0        0     1038 2024-05-25 23:43:38.000000 ns_search_saved_export-0.1.8/ns_search_saved_export/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-28 02:03:50.813837 ns_search_saved_export-0.1.8/ns_search_saved_export.egg-info/
+-rw-rw-rw-   0        0        0     1615 2024-05-28 02:03:50.000000 ns_search_saved_export-0.1.8/ns_search_saved_export.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2024-05-28 02:03:50.000000 ns_search_saved_export-0.1.8/ns_search_saved_export.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 02:03:50.000000 ns_search_saved_export-0.1.8/ns_search_saved_export.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-28 02:03:50.000000 ns_search_saved_export-0.1.8/ns_search_saved_export.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-05-28 02:03:50.000000 ns_search_saved_export-0.1.8/ns_search_saved_export.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      497 2024-05-26 18:01:07.000000 ns_search_saved_export-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-28 02:03:50.816780 ns_search_saved_export-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      799 2024-05-28 02:03:23.000000 ns_search_saved_export-0.1.8/setup.py
```

### Comparing `ns_search_saved_export-0.1.7/PKG-INFO` & `ns_search_saved_export-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_search_saved_export
-Version: 0.1.7
+Version: 0.1.8
 Summary: A library for interacting with NetSuite API and exporting data
 Home-page: https://github.com/gildder/netsuite-search-saved-export
 Author: Gildder
 Author-email: gildder@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ns_search_saved_export-0.1.7/README.md` & `ns_search_saved_export-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.7/Tests/test_main.py` & `ns_search_saved_export-0.1.8/Tests/test_main.py`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.7/Tests/test_ns_search_saved_export.py` & `ns_search_saved_export-0.1.8/Tests/test_ns_search_saved_export.py`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.7/Tests/test_utils.py` & `ns_search_saved_export-0.1.8/Tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.7/ns_search_saved_export/ns_search_saved_export.py` & `ns_search_saved_export-0.1.8/ns_search_saved_export/ns_search_saved_export.py`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.7/ns_search_saved_export/utils.py` & `ns_search_saved_export-0.1.8/ns_search_saved_export/utils.py`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.7/ns_search_saved_export.egg-info/PKG-INFO` & `ns_search_saved_export-0.1.8/ns_search_saved_export.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ns_search_saved_export
-Version: 0.1.7
+Version: 0.1.8
 Summary: A library for interacting with NetSuite API and exporting data
 Home-page: https://github.com/gildder/netsuite-search-saved-export
 Author: Gildder
 Author-email: gildder@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ns_search_saved_export-0.1.7/ns_search_saved_export.egg-info/SOURCES.txt` & `ns_search_saved_export-0.1.8/ns_search_saved_export.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ns_search_saved_export-0.1.7/setup.py` & `ns_search_saved_export-0.1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ns_search_saved_export',
-    version='0.1.7',
+    version='0.1.8',
     description='A library for interacting with NetSuite API and exporting data',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Gildder',
     author_email='gildder@outlook.com',
     url='https://github.com/gildder/netsuite-search-saved-export',
     packages=find_packages(),
```

