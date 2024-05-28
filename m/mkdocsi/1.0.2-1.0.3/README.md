# Comparing `tmp/mkdocsi-1.0.2.tar.gz` & `tmp/mkdocsi-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocsi-1.0.2.tar", last modified: Tue May 28 15:50:29 2024, max compression
+gzip compressed data, was "mkdocsi-1.0.3.tar", last modified: Tue May 28 15:56:31 2024, max compression
```

## Comparing `mkdocsi-1.0.2.tar` & `mkdocsi-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:50:29.568166 mkdocsi-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 15:50:29.568166 mkdocsi-1.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-28 15:50:19.000000 mkdocsi-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:50:29.566166 mkdocsi-1.0.2/mkdocsi/
--rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-28 15:50:19.000000 mkdocsi-1.0.2/mkdocsi/Main.py
--rw-rw-rw-   0 root         (0) root         (0)     5013 2024-05-28 15:50:19.000000 mkdocsi-1.0.2/mkdocsi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:50:29.568166 mkdocsi-1.0.2/mkdocsi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 15:50:29.000000 mkdocsi-1.0.2/mkdocsi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2024-05-28 15:50:29.000000 mkdocsi-1.0.2/mkdocsi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 15:50:29.000000 mkdocsi-1.0.2/mkdocsi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-05-28 15:50:29.000000 mkdocsi-1.0.2/mkdocsi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-28 15:50:29.000000 mkdocsi-1.0.2/mkdocsi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 15:50:29.000000 mkdocsi-1.0.2/mkdocsi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 15:50:29.568166 mkdocsi-1.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-28 15:50:19.000000 mkdocsi-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:56:31.057932 mkdocsi-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 15:56:31.056932 mkdocsi-1.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-28 15:56:21.000000 mkdocsi-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:56:31.054932 mkdocsi-1.0.3/mkdocsi/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-28 15:56:21.000000 mkdocsi-1.0.3/mkdocsi/Main.py
+-rw-rw-rw-   0 root         (0) root         (0)     5190 2024-05-28 15:56:21.000000 mkdocsi-1.0.3/mkdocsi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:56:31.056932 mkdocsi-1.0.3/mkdocsi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 15:56:31.000000 mkdocsi-1.0.3/mkdocsi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2024-05-28 15:56:31.000000 mkdocsi-1.0.3/mkdocsi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 15:56:31.000000 mkdocsi-1.0.3/mkdocsi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-05-28 15:56:31.000000 mkdocsi-1.0.3/mkdocsi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-28 15:56:31.000000 mkdocsi-1.0.3/mkdocsi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 15:56:31.000000 mkdocsi-1.0.3/mkdocsi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 15:56:31.057932 mkdocsi-1.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-28 15:56:21.000000 mkdocsi-1.0.3/setup.py
```

### Comparing `mkdocsi-1.0.2/PKG-INFO` & `mkdocsi-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.0.2
+Version: 1.0.3
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.0.2/mkdocsi/__init__.py` & `mkdocsi-1.0.3/mkdocsi/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 import yaml  , os , json , sys 
 from glob import glob 
 
 
 class MkdocsUtils : 
-    def __init__(self , docs_folder  ,  Template_mkdocs_file  ) : 
-        self.Template_mkdocs_file = os.path.abspath(Template_mkdocs_file)
-        self.Template_mkdocs_file = None 
+    def __init__(self , docs_folder  ,  Template_mkdocs_file   = None ) : 
+        if Template_mkdocs_file is not None : 
+            self.Template_mkdocs_file = os.path.abspath(Template_mkdocs_file)
+        else  : 
+            self.Template_mkdocs_file = os.path.join((os.path.dirname(__file__),"mkdocs.yml"))
+
         self.docs_folder = os.path.abspath(docs_folder)  
+        self.new_mkdocsfile = os.path.join(self.docs_folder , "mkdocs.yml")
         with open(self.Template_mkdocs_file, 'r') as f: self.mkdocs_data = yaml.safe_load(f)
 
     def __repr__(self) : 
         return json.dumps(self.mkdocs_data , indent = 4 )
 
     def buildTree(self) : 
         self.mkdocs_data['nav'] = self.get_md_files_tree() 
-        output_file = os.path.join(self.docs_folder , "mkdocs.yml")
-        with open(output_file, 'w') as file:                                                                                                                                                       
+        with open(self.new_mkdocsfile, 'w') as file:                                                                                                                                                       
             yaml.dump(self.mkdocs_data, file, default_flow_style=False)       
                                                                                                                                                                                           
     def to_camel_case(self , snake_str):                                                                                                                                                                  
-        components = snake_str.split('_')   
-        print(components)                                                                                                                                                       
+        components = snake_str.split('_')                                                                                                                                                     
         return " ".join(components)                                                                                                                       
                                                                                                                                                                                                 
     def get_md_files_tree(self):                                                                                                                                                            
         def walk_dir(folder, parent_path=''):                                                                                                                                                      
             tree = []                                                                                                                                                                              
             for item in sorted(os.listdir(folder)):                                                                                                                                                
                 path = os.path.join(folder, item)                                                                                                                                             
                 relative_path = os.path.join(parent_path, item)
-                
-
                 if os.path.isdir(path):  
                     # path = os.path.relpath(path, self.docs_folder)                                                                                                                                                         
                     subtree = walk_dir(path, relative_path)                                                                                                                                        
                     if subtree:  # Only include non-empty directories                                                                                                                              
                         tree.append({item: subtree})                                                                                                                                               
                 elif item.endswith('.md'):                                                                                                                                                         
                     base_name = os.path.splitext(item)[0]                                                                                                                                          
                     camel_case_name = self.to_camel_case(base_name)                                                                                                                                     
                     tree.append({camel_case_name: relative_path})                                                                                                                                  
             return tree                                                                                                                                                                            
                                                                                                                                                                                                 
-        return walk_dir(self.docs_folder)    
+        return walk_dir(self.docs_folder)    
+
+
+def generate_site(docs_folder) : 
+    _MkdocsUtils = MkdocsUtils(docs_folder)
```

### Comparing `mkdocsi-1.0.2/mkdocsi.egg-info/PKG-INFO` & `mkdocsi-1.0.3/mkdocsi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.0.2
+Version: 1.0.3
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mkdocsi-1.0.2/setup.py` & `mkdocsi-1.0.3/setup.py`

 * *Files identical despite different names*

