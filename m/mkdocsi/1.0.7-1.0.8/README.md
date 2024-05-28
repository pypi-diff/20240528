# Comparing `tmp/mkdocsi-1.0.7.tar.gz` & `tmp/mkdocsi-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocsi-1.0.7.tar", last modified: Tue May 28 21:29:54 2024, max compression
+gzip compressed data, was "mkdocsi-1.0.8.tar", last modified: Tue May 28 21:32:25 2024, max compression
```

## Comparing `mkdocsi-1.0.7.tar` & `mkdocsi-1.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 21:29:54.289939 mkdocsi-1.0.7/
--rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 21:29:54.289939 mkdocsi-1.0.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-28 21:29:45.000000 mkdocsi-1.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 21:29:54.287939 mkdocsi-1.0.7/mkdocsi/
--rw-rw-rw-   0 root         (0) root         (0)      172 2024-05-28 21:29:45.000000 mkdocsi-1.0.7/mkdocsi/Main.py
--rw-rw-rw-   0 root         (0) root         (0)     5953 2024-05-28 21:29:45.000000 mkdocsi-1.0.7/mkdocsi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 21:29:54.288939 mkdocsi-1.0.7/mkdocsi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 21:29:54.000000 mkdocsi-1.0.7/mkdocsi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2024-05-28 21:29:54.000000 mkdocsi-1.0.7/mkdocsi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 21:29:54.000000 mkdocsi-1.0.7/mkdocsi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-05-28 21:29:54.000000 mkdocsi-1.0.7/mkdocsi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-28 21:29:54.000000 mkdocsi-1.0.7/mkdocsi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 21:29:54.000000 mkdocsi-1.0.7/mkdocsi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 21:29:54.289939 mkdocsi-1.0.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-28 21:29:45.000000 mkdocsi-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 21:32:25.847514 mkdocsi-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 21:32:25.847514 mkdocsi-1.0.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-28 21:32:16.000000 mkdocsi-1.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 21:32:25.845514 mkdocsi-1.0.8/mkdocsi/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-05-28 21:32:16.000000 mkdocsi-1.0.8/mkdocsi/Main.py
+-rw-rw-rw-   0 root         (0) root         (0)     5955 2024-05-28 21:32:16.000000 mkdocsi-1.0.8/mkdocsi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 21:32:25.846514 mkdocsi-1.0.8/mkdocsi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 21:32:25.000000 mkdocsi-1.0.8/mkdocsi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2024-05-28 21:32:25.000000 mkdocsi-1.0.8/mkdocsi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 21:32:25.000000 mkdocsi-1.0.8/mkdocsi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-05-28 21:32:25.000000 mkdocsi-1.0.8/mkdocsi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-28 21:32:25.000000 mkdocsi-1.0.8/mkdocsi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 21:32:25.000000 mkdocsi-1.0.8/mkdocsi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 21:32:25.847514 mkdocsi-1.0.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-28 21:32:16.000000 mkdocsi-1.0.8/setup.py
```

### Comparing `mkdocsi-1.0.7/PKG-INFO` & `mkdocsi-1.0.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.0.7
+Version: 1.0.8
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.0.7/mkdocsi/__init__.py` & `mkdocsi-1.0.8/mkdocsi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,17 +43,17 @@
       name: Switch to light mode
 
 """
 
 class MkdocsUtils : 
     def __init__(self , docs_folder  ,  Template_mkdocs   = None ) : 
         if Template_mkdocs is not None : 
-            self.Template_mkdocs = DEFAULT_MKDOCS
+            self.Template_mkdocs = Template_mkdocs 
         else  : 
-            self.Template_mkdocs = Template_mkdocs
+            self.Template_mkdocs = DEFAULT_MKDOCS 
         self.docs_folder = os.path.abspath(docs_folder)  
         self.new_mkdocsfile = os.path.join(self.docs_folder , "mkdocs.yml")
         self.mkdocs_data = yaml.safe_load(self.Template_mkdocs)
         if not ('nav' in self.mkdocs_data.keys()) : self.mkdocs_data['nav'] = list()
 
     def __repr__(self) : 
         return json.dumps(self.mkdocs_data , indent = 4 )
```

### Comparing `mkdocsi-1.0.7/mkdocsi.egg-info/PKG-INFO` & `mkdocsi-1.0.8/mkdocsi.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.0.7
+Version: 1.0.8
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.0.7/setup.py` & `mkdocsi-1.0.8/setup.py`

 * *Files identical despite different names*

