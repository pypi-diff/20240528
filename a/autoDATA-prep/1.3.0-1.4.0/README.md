# Comparing `tmp/autoDATA-prep-1.3.0.tar.gz` & `tmp/autoDATA_prep-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/autoDATA-prep-1.3.0.tar", last modified: Tue May 28 18:09:50 2024, max compression
+gzip compressed data, was "dist/autoDATA_prep-1.4.0.tar", last modified: Tue May 28 18:30:28 2024, max compression
```

## Comparing `autoDATA-prep-1.3.0.tar` & `autoDATA_prep-1.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 18:09:50.000000 autoDATA-prep-1.3.0/
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 18:09:50.000000 autoDATA-prep-1.3.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 18:09:50.000000 autoDATA-prep-1.3.0/assets/
--rw-r--r--   0 root         (0) root         (0)   113880 2024-05-28 17:43:23.000000 autoDATA-prep-1.3.0/assets/data-preprocessing-cover.png
--rw-r--r--   0 root         (0) root         (0)      831 2024-05-28 18:09:50.000000 autoDATA-prep-1.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       61 2024-05-28 17:58:45.000000 autoDATA-prep-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      692 2024-05-28 18:08:53.000000 autoDATA-prep-1.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 18:09:50.000000 autoDATA-prep-1.3.0/autoDATA-prep/
--rw-r--r--   0 root         (0) root         (0)     7632 2024-05-28 00:48:36.000000 autoDATA-prep-1.3.0/autoDATA-prep/python_code.py
--rw-r--r--   0 root         (0) root         (0)        0 2018-06-02 00:07:44.000000 autoDATA-prep-1.3.0/autoDATA-prep/__init__.py
--rw-r--r--   0 root         (0) root         (0)      494 2024-05-28 18:08:03.000000 autoDATA-prep-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 18:09:50.000000 autoDATA-prep-1.3.0/autoDATA_prep.egg-info/
--rw-r--r--   0 root         (0) root         (0)      305 2024-05-28 18:09:50.000000 autoDATA-prep-1.3.0/autoDATA_prep.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      831 2024-05-28 18:09:50.000000 autoDATA-prep-1.3.0/autoDATA_prep.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       14 2024-05-28 18:09:50.000000 autoDATA-prep-1.3.0/autoDATA_prep.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 18:09:50.000000 autoDATA-prep-1.3.0/autoDATA_prep.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 18:09:50.000000 autoDATA-prep-1.3.0/autoDATA_prep.egg-info/dependency_links.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 18:30:28.000000 autoDATA_prep-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 18:30:28.000000 autoDATA_prep-1.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 18:30:28.000000 autoDATA_prep-1.4.0/assets/
+-rw-r--r--   0 root         (0) root         (0)   113880 2024-05-28 17:43:23.000000 autoDATA_prep-1.4.0/assets/data-preprocessing-cover.png
+-rw-r--r--   0 root         (0) root         (0)      831 2024-05-28 18:30:28.000000 autoDATA_prep-1.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       61 2024-05-28 17:58:45.000000 autoDATA_prep-1.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      715 2024-05-28 18:29:48.000000 autoDATA_prep-1.4.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)      494 2024-05-28 18:08:03.000000 autoDATA_prep-1.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 18:30:28.000000 autoDATA_prep-1.4.0/autoDATA_prep.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      305 2024-05-28 18:30:28.000000 autoDATA_prep-1.4.0/autoDATA_prep.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      831 2024-05-28 18:30:28.000000 autoDATA_prep-1.4.0/autoDATA_prep.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-28 18:30:28.000000 autoDATA_prep-1.4.0/autoDATA_prep.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 18:30:28.000000 autoDATA_prep-1.4.0/autoDATA_prep.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 18:30:28.000000 autoDATA_prep-1.4.0/autoDATA_prep.egg-info/dependency_links.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 18:30:28.000000 autoDATA_prep-1.4.0/autoDATA_prep/
+-rw-r--r--   0 root         (0) root         (0)     7632 2024-05-28 00:48:36.000000 autoDATA_prep-1.4.0/autoDATA_prep/python_code.py
+-rw-r--r--   0 root         (0) root         (0)        0 2018-06-02 00:07:44.000000 autoDATA_prep-1.4.0/autoDATA_prep/__init__.py
```

### Comparing `autoDATA-prep-1.3.0/assets/data-preprocessing-cover.png` & `autoDATA_prep-1.4.0/assets/data-preprocessing-cover.png`

 * *Files identical despite different names*

### Comparing `autoDATA-prep-1.3.0/PKG-INFO` & `autoDATA_prep-1.4.0/autoDATA_prep.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: autoDATA-prep
-Version: 1.3.0
+Version: 1.4.0
 Summary: Data pre-processing library
 Home-page: UNKNOWN
 Author: Emmanuel Ezenwere
 Author-email: emmaezenwere@gmail.com
 License: UNKNOWN
 Description-Content-Type: text/markdown
 Description: autoDATA-prep automates the data pre-processing step, this accelerates the first stage of any Data Analysis/ Data Science/ML pipeline.
```

### Comparing `autoDATA-prep-1.3.0/setup.py` & `autoDATA_prep-1.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 # Read the contents of your README file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
-    name='autoDATA-prep',
-    version='1.3.0',
+    name='autoDATA_prep',  # Use underscore here
+    version='1.4.0',
     description='Data pre-processing library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Emmanuel Ezenwere',
     author_email='emmaezenwere@gmail.com',
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `autoDATA-prep-1.3.0/autoDATA-prep/python_code.py` & `autoDATA_prep-1.4.0/autoDATA_prep/python_code.py`

 * *Files identical despite different names*

### Comparing `autoDATA-prep-1.3.0/autoDATA_prep.egg-info/PKG-INFO` & `autoDATA_prep-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
-Name: autoDATA-prep
-Version: 1.3.0
+Name: autoDATA_prep
+Version: 1.4.0
 Summary: Data pre-processing library
 Home-page: UNKNOWN
 Author: Emmanuel Ezenwere
 Author-email: emmaezenwere@gmail.com
 License: UNKNOWN
 Description-Content-Type: text/markdown
 Description: autoDATA-prep automates the data pre-processing step, this accelerates the first stage of any Data Analysis/ Data Science/ML pipeline.
```

