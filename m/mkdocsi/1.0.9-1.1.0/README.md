# Comparing `tmp/mkdocsi-1.0.9.tar.gz` & `tmp/mkdocsi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocsi-1.0.9.tar", last modified: Tue May 28 21:34:30 2024, max compression
+gzip compressed data, was "mkdocsi-1.1.0.tar", last modified: Tue May 28 21:41:11 2024, max compression
```

## Comparing `mkdocsi-1.0.9.tar` & `mkdocsi-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 21:34:30.987386 mkdocsi-1.0.9/
--rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 21:34:30.987386 mkdocsi-1.0.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-28 21:34:21.000000 mkdocsi-1.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 21:34:30.985386 mkdocsi-1.0.9/mkdocsi/
--rw-rw-rw-   0 root         (0) root         (0)      172 2024-05-28 21:34:21.000000 mkdocsi-1.0.9/mkdocsi/Main.py
--rw-rw-rw-   0 root         (0) root         (0)     5960 2024-05-28 21:34:21.000000 mkdocsi-1.0.9/mkdocsi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 21:34:30.987386 mkdocsi-1.0.9/mkdocsi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 21:34:30.000000 mkdocsi-1.0.9/mkdocsi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2024-05-28 21:34:30.000000 mkdocsi-1.0.9/mkdocsi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 21:34:30.000000 mkdocsi-1.0.9/mkdocsi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-05-28 21:34:30.000000 mkdocsi-1.0.9/mkdocsi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-28 21:34:30.000000 mkdocsi-1.0.9/mkdocsi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 21:34:30.000000 mkdocsi-1.0.9/mkdocsi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 21:34:30.987386 mkdocsi-1.0.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-28 21:34:21.000000 mkdocsi-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 21:41:11.436543 mkdocsi-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 21:41:11.436543 mkdocsi-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-28 21:41:02.000000 mkdocsi-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 21:41:11.434543 mkdocsi-1.1.0/mkdocsi/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-05-28 21:41:02.000000 mkdocsi-1.1.0/mkdocsi/Main.py
+-rw-rw-rw-   0 root         (0) root         (0)     6206 2024-05-28 21:41:02.000000 mkdocsi-1.1.0/mkdocsi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 21:41:11.436543 mkdocsi-1.1.0/mkdocsi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 21:41:11.000000 mkdocsi-1.1.0/mkdocsi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2024-05-28 21:41:11.000000 mkdocsi-1.1.0/mkdocsi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 21:41:11.000000 mkdocsi-1.1.0/mkdocsi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-05-28 21:41:11.000000 mkdocsi-1.1.0/mkdocsi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-28 21:41:11.000000 mkdocsi-1.1.0/mkdocsi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 21:41:11.000000 mkdocsi-1.1.0/mkdocsi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 21:41:11.436543 mkdocsi-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-28 21:41:02.000000 mkdocsi-1.1.0/setup.py
```

### Comparing `mkdocsi-1.0.9/PKG-INFO` & `mkdocsi-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.0.9
+Version: 1.1.0
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.0.9/mkdocsi/__init__.py` & `mkdocsi-1.1.0/mkdocsi/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,18 +51,25 @@
         else  : 
             self.Template_mkdocs = DEFAULT_MKDOCS 
         self.docs_folder = os.path.abspath(docs_folder)  
         self.new_mkdocsfile = os.path.join(self.docs_folder ,"..", "mkdocs.yml")
         self.mkdocs_data = yaml.safe_load(self.Template_mkdocs)
         if not ('nav' in self.mkdocs_data.keys()) : self.mkdocs_data['nav'] = list()
 
+    def make_safe(self) : 
+        Tags_md = os.path.join(self.docs_folder , "Tags.md")
+        if not os.path.isfile(Tags_md) : 
+            print("<!-- material/tags { scope: true } -->" , file = open(Tags_md , "w"))
+
+
     def __repr__(self) : 
         return json.dumps(self.mkdocs_data , indent = 4 )
 
     def buildTree(self) : 
+        self.make_safe()
         self.mkdocs_data['nav'].extend(self.get_md_files_tree())
         with open(self.new_mkdocsfile, 'w') as file:                                                                                                                                                       
             yaml.dump(self.mkdocs_data, file, default_flow_style=False)       
                                                                                                                                                                                           
     def to_camel_case(self , snake_str):                                                                                                                                                                  
         components = snake_str.split('_')                                                                                                                                                     
         return " ".join(components)
```

### Comparing `mkdocsi-1.0.9/mkdocsi.egg-info/PKG-INFO` & `mkdocsi-1.1.0/mkdocsi.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.0.9
+Version: 1.1.0
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.0.9/setup.py` & `mkdocsi-1.1.0/setup.py`

 * *Files identical despite different names*

