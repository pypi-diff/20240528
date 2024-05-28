# Comparing `tmp/habslib-0.1.6.tar.gz` & `tmp/habslib-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habslib-0.1.6.tar", last modified: Tue May 28 16:30:58 2024, max compression
+gzip compressed data, was "habslib-0.1.7.tar", last modified: Tue May 28 16:33:18 2024, max compression
```

## Comparing `habslib-0.1.6.tar` & `habslib-0.1.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 16:30:58.165956 habslib-0.1.6/
-drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 16:30:58.164220 habslib-0.1.6/HABSlib/
--rw-r--r--   0 do         (501) staff       (20)      126 2024-05-23 15:47:32.000000 habslib-0.1.6/HABSlib/__init__.py
--rwxr-xr-x   0 do         (501) staff       (20)     6925 2024-05-28 14:44:06.000000 habslib-0.1.6/HABSlib/board_manager.py
--rw-r--r--   0 do         (501) staff       (20)      131 2024-05-23 15:47:32.000000 habslib-0.1.6/HABSlib/config.py
--rw-r--r--   0 do         (501) staff       (20)     3706 2024-05-23 15:47:32.000000 habslib-0.1.6/HABSlib/crypt.py
--rw-r--r--   0 do         (501) staff       (20)    15578 2024-05-28 16:25:54.000000 habslib-0.1.6/HABSlib/service.py
--rwxr-xr-x   0 do         (501) staff       (20)      962 2024-05-23 15:47:32.000000 habslib-0.1.6/HABSlib/utils.py
-drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 16:30:58.165605 habslib-0.1.6/HABSlib.egg-info/
--rw-r--r--   0 do         (501) staff       (20)     2025 2024-05-28 16:30:58.000000 habslib-0.1.6/HABSlib.egg-info/PKG-INFO
--rw-r--r--   0 do         (501) staff       (20)      399 2024-05-28 16:30:58.000000 habslib-0.1.6/HABSlib.egg-info/SOURCES.txt
--rw-r--r--   0 do         (501) staff       (20)        1 2024-05-28 16:30:58.000000 habslib-0.1.6/HABSlib.egg-info/dependency_links.txt
--rw-r--r--   0 do         (501) staff       (20)      167 2024-05-28 16:30:58.000000 habslib-0.1.6/HABSlib.egg-info/requires.txt
--rw-r--r--   0 do         (501) staff       (20)       14 2024-05-28 16:30:58.000000 habslib-0.1.6/HABSlib.egg-info/top_level.txt
--rw-r--r--   0 do         (501) staff       (20)     1060 2024-05-28 10:05:57.000000 habslib-0.1.6/LICENCE
--rw-r--r--   0 do         (501) staff       (20)       42 2024-05-27 22:43:14.000000 habslib-0.1.6/MANIFEST.in
--rw-r--r--   0 do         (501) staff       (20)     2025 2024-05-28 16:30:58.165791 habslib-0.1.6/PKG-INFO
--rw-r--r--   0 do         (501) staff       (20)     1215 2024-05-28 15:35:25.000000 habslib-0.1.6/README.md
--rw-r--r--   0 do         (501) staff       (20)      172 2024-05-28 15:44:25.000000 habslib-0.1.6/requirements.txt
--rw-r--r--   0 do         (501) staff       (20)       38 2024-05-28 16:30:58.166000 habslib-0.1.6/setup.cfg
--rw-r--r--   0 do         (501) staff       (20)     1018 2024-05-28 16:30:41.000000 habslib-0.1.6/setup.py
-drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 16:30:58.165402 habslib-0.1.6/tests/
--rw-r--r--   0 do         (501) staff       (20)       62 2024-05-23 15:47:32.000000 habslib-0.1.6/tests/__init__.py
--rw-r--r--   0 do         (501) staff       (20)      131 2024-05-23 15:47:32.000000 habslib-0.1.6/tests/config.py
--rw-r--r--   0 do         (501) staff       (20)     1934 2024-05-23 15:47:32.000000 habslib-0.1.6/tests/conftest.py
--rw-r--r--   0 do         (501) staff       (20)     8909 2024-05-28 15:51:37.000000 habslib-0.1.6/tests/test_habslib.py
+drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 16:33:18.383192 habslib-0.1.7/
+drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 16:33:18.381626 habslib-0.1.7/HABSlib/
+-rw-r--r--   0 do         (501) staff       (20)      126 2024-05-23 15:47:32.000000 habslib-0.1.7/HABSlib/__init__.py
+-rwxr-xr-x   0 do         (501) staff       (20)     6925 2024-05-28 14:44:06.000000 habslib-0.1.7/HABSlib/board_manager.py
+-rw-r--r--   0 do         (501) staff       (20)      131 2024-05-23 15:47:32.000000 habslib-0.1.7/HABSlib/config.py
+-rw-r--r--   0 do         (501) staff       (20)     3706 2024-05-23 15:47:32.000000 habslib-0.1.7/HABSlib/crypt.py
+-rw-r--r--   0 do         (501) staff       (20)    15580 2024-05-28 16:32:30.000000 habslib-0.1.7/HABSlib/service.py
+-rwxr-xr-x   0 do         (501) staff       (20)      962 2024-05-23 15:47:32.000000 habslib-0.1.7/HABSlib/utils.py
+drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 16:33:18.382820 habslib-0.1.7/HABSlib.egg-info/
+-rw-r--r--   0 do         (501) staff       (20)     2025 2024-05-28 16:33:18.000000 habslib-0.1.7/HABSlib.egg-info/PKG-INFO
+-rw-r--r--   0 do         (501) staff       (20)      399 2024-05-28 16:33:18.000000 habslib-0.1.7/HABSlib.egg-info/SOURCES.txt
+-rw-r--r--   0 do         (501) staff       (20)        1 2024-05-28 16:33:18.000000 habslib-0.1.7/HABSlib.egg-info/dependency_links.txt
+-rw-r--r--   0 do         (501) staff       (20)      167 2024-05-28 16:33:18.000000 habslib-0.1.7/HABSlib.egg-info/requires.txt
+-rw-r--r--   0 do         (501) staff       (20)       14 2024-05-28 16:33:18.000000 habslib-0.1.7/HABSlib.egg-info/top_level.txt
+-rw-r--r--   0 do         (501) staff       (20)     1060 2024-05-28 10:05:57.000000 habslib-0.1.7/LICENCE
+-rw-r--r--   0 do         (501) staff       (20)       42 2024-05-27 22:43:14.000000 habslib-0.1.7/MANIFEST.in
+-rw-r--r--   0 do         (501) staff       (20)     2025 2024-05-28 16:33:18.383015 habslib-0.1.7/PKG-INFO
+-rw-r--r--   0 do         (501) staff       (20)     1215 2024-05-28 15:35:25.000000 habslib-0.1.7/README.md
+-rw-r--r--   0 do         (501) staff       (20)      172 2024-05-28 15:44:25.000000 habslib-0.1.7/requirements.txt
+-rw-r--r--   0 do         (501) staff       (20)       38 2024-05-28 16:33:18.383226 habslib-0.1.7/setup.cfg
+-rw-r--r--   0 do         (501) staff       (20)     1018 2024-05-28 16:32:39.000000 habslib-0.1.7/setup.py
+drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 16:33:18.382649 habslib-0.1.7/tests/
+-rw-r--r--   0 do         (501) staff       (20)       62 2024-05-23 15:47:32.000000 habslib-0.1.7/tests/__init__.py
+-rw-r--r--   0 do         (501) staff       (20)      131 2024-05-23 15:47:32.000000 habslib-0.1.7/tests/config.py
+-rw-r--r--   0 do         (501) staff       (20)     1934 2024-05-23 15:47:32.000000 habslib-0.1.7/tests/conftest.py
+-rw-r--r--   0 do         (501) staff       (20)     8909 2024-05-28 15:51:37.000000 habslib-0.1.7/tests/test_habslib.py
```

### Comparing `habslib-0.1.6/HABSlib/board_manager.py` & `habslib-0.1.7/HABSlib/board_manager.py`

 * *Files identical despite different names*

### Comparing `habslib-0.1.6/HABSlib/crypt.py` & `habslib-0.1.7/HABSlib/crypt.py`

 * *Files identical despite different names*

### Comparing `habslib-0.1.6/HABSlib/service.py` & `habslib-0.1.7/HABSlib/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 #       Human
 #       Automated (unit test passing GitLab Ops)
 
 
 
 ######################################################
 # validate the metadata against a specified schema
-def validate_metadata(metadata, schema_name, schemafile='metadata.json'):
+def validate_metadata(metadata, schema_name, schemafile='./metadata.json'):
 
     try:
         with open(schemafile, 'r') as file:
             content = file.read()
             schemas = json.loads(content)
         schema = schemas[schema_name]
         validate(instance=metadata, schema=schema) #, format_checker=FormatChecker())
```

### Comparing `habslib-0.1.6/HABSlib/utils.py` & `habslib-0.1.7/HABSlib/utils.py`

 * *Files identical despite different names*

### Comparing `habslib-0.1.6/HABSlib.egg-info/PKG-INFO` & `habslib-0.1.7/HABSlib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HABSlib
-Version: 0.1.6
+Version: 0.1.7
 Summary: A library for interacting with the HABS BrainOS API.
 Home-page: https://github.com/Olocufier/HABS.git
 Author: Domenico Guarino
 Author-email: domenico@habs.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `habslib-0.1.6/LICENCE` & `habslib-0.1.7/LICENCE`

 * *Files identical despite different names*

### Comparing `habslib-0.1.6/PKG-INFO` & `habslib-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HABSlib
-Version: 0.1.6
+Version: 0.1.7
 Summary: A library for interacting with the HABS BrainOS API.
 Home-page: https://github.com/Olocufier/HABS.git
 Author: Domenico Guarino
 Author-email: domenico@habs.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `habslib-0.1.6/README.md` & `habslib-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `habslib-0.1.6/setup.py` & `habslib-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="HABSlib",
-    version="0.1.6",
+    version="0.1.7",
     author="Domenico Guarino",
     author_email="domenico@habs.ai",
     description="A library for interacting with the HABS BrainOS API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Olocufier/HABS.git",
     packages=find_packages(),
```

### Comparing `habslib-0.1.6/tests/conftest.py` & `habslib-0.1.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `habslib-0.1.6/tests/test_habslib.py` & `habslib-0.1.7/tests/test_habslib.py`

 * *Files identical despite different names*

