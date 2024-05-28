# Comparing `tmp/mkdocsi-1.0.5.tar.gz` & `tmp/mkdocsi-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocsi-1.0.5.tar", last modified: Tue May 28 16:13:50 2024, max compression
+gzip compressed data, was "mkdocsi-1.0.6.tar", last modified: Tue May 28 18:31:40 2024, max compression
```

## Comparing `mkdocsi-1.0.5.tar` & `mkdocsi-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:13:50.273381 mkdocsi-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 16:13:50.273381 mkdocsi-1.0.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-28 16:13:40.000000 mkdocsi-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:13:50.271381 mkdocsi-1.0.5/mkdocsi/
--rw-rw-rw-   0 root         (0) root         (0)      172 2024-05-28 16:13:40.000000 mkdocsi-1.0.5/mkdocsi/Main.py
--rw-rw-rw-   0 root         (0) root         (0)     5273 2024-05-28 16:13:40.000000 mkdocsi-1.0.5/mkdocsi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:13:50.273381 mkdocsi-1.0.5/mkdocsi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 16:13:50.000000 mkdocsi-1.0.5/mkdocsi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2024-05-28 16:13:50.000000 mkdocsi-1.0.5/mkdocsi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 16:13:50.000000 mkdocsi-1.0.5/mkdocsi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-05-28 16:13:50.000000 mkdocsi-1.0.5/mkdocsi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-28 16:13:50.000000 mkdocsi-1.0.5/mkdocsi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 16:13:50.000000 mkdocsi-1.0.5/mkdocsi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 16:13:50.273381 mkdocsi-1.0.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-28 16:13:40.000000 mkdocsi-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 18:31:40.680573 mkdocsi-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 18:31:40.679573 mkdocsi-1.0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-28 18:31:30.000000 mkdocsi-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 18:31:40.677573 mkdocsi-1.0.6/mkdocsi/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-05-28 18:31:30.000000 mkdocsi-1.0.6/mkdocsi/Main.py
+-rw-rw-rw-   0 root         (0) root         (0)     5271 2024-05-28 18:31:30.000000 mkdocsi-1.0.6/mkdocsi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 18:31:40.679573 mkdocsi-1.0.6/mkdocsi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 18:31:40.000000 mkdocsi-1.0.6/mkdocsi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2024-05-28 18:31:40.000000 mkdocsi-1.0.6/mkdocsi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 18:31:40.000000 mkdocsi-1.0.6/mkdocsi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-05-28 18:31:40.000000 mkdocsi-1.0.6/mkdocsi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-28 18:31:40.000000 mkdocsi-1.0.6/mkdocsi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 18:31:40.000000 mkdocsi-1.0.6/mkdocsi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 18:31:40.680573 mkdocsi-1.0.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-28 18:31:30.000000 mkdocsi-1.0.6/setup.py
```

### Comparing `mkdocsi-1.0.5/PKG-INFO` & `mkdocsi-1.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.0.5
+Version: 1.0.6
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.0.5/mkdocsi/__init__.py` & `mkdocsi-1.0.6/mkdocsi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 class MkdocsUtils : 
     def __init__(self , docs_folder  ,  Template_mkdocs_file   = None ) : 
         if Template_mkdocs_file is not None : 
             self.Template_mkdocs_file = os.path.abspath(Template_mkdocs_file)
         else  : 
-            self.Template_mkdocs_file = os.path.join((os.path.dirname(__file__),"mkdocs.yml"))
+            self.Template_mkdocs_file = os.path.join(os.path.dirname(__file__),"mkdocs.yml")
 
         self.docs_folder = os.path.abspath(docs_folder)  
         self.new_mkdocsfile = os.path.join(self.docs_folder , "mkdocs.yml")
         with open(self.Template_mkdocs_file, 'r') as f: self.mkdocs_data = yaml.safe_load(f)
 
     def __repr__(self) : 
         return json.dumps(self.mkdocs_data , indent = 4 )
```

### Comparing `mkdocsi-1.0.5/mkdocsi.egg-info/PKG-INFO` & `mkdocsi-1.0.6/mkdocsi.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.0.5
+Version: 1.0.6
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.0.5/setup.py` & `mkdocsi-1.0.6/setup.py`

 * *Files identical despite different names*

