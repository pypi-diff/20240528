# Comparing `tmp/mkdocsi-1.0.1.tar.gz` & `tmp/mkdocsi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocsi-1.0.1.tar", last modified: Tue May 28 15:45:21 2024, max compression
+gzip compressed data, was "mkdocsi-1.0.2.tar", last modified: Tue May 28 15:50:29 2024, max compression
```

## Comparing `mkdocsi-1.0.1.tar` & `mkdocsi-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:45:21.352274 mkdocsi-1.0.1/
--rw-r--r--   0 root         (0) root         (0)      550 2024-05-28 15:45:21.352274 mkdocsi-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-28 15:45:10.000000 mkdocsi-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:45:21.350273 mkdocsi-1.0.1/mkdocsi/
--rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-28 15:45:10.000000 mkdocsi-1.0.1/mkdocsi/Main.py
--rw-rw-rw-   0 root         (0) root         (0)     5014 2024-05-28 15:45:10.000000 mkdocsi-1.0.1/mkdocsi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:45:21.352274 mkdocsi-1.0.1/mkdocsi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      550 2024-05-28 15:45:21.000000 mkdocsi-1.0.1/mkdocsi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2024-05-28 15:45:21.000000 mkdocsi-1.0.1/mkdocsi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 15:45:21.000000 mkdocsi-1.0.1/mkdocsi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-05-28 15:45:21.000000 mkdocsi-1.0.1/mkdocsi.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-28 15:45:21.000000 mkdocsi-1.0.1/mkdocsi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 15:45:21.000000 mkdocsi-1.0.1/mkdocsi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 15:45:21.353273 mkdocsi-1.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3019 2024-05-28 15:45:10.000000 mkdocsi-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:50:29.568166 mkdocsi-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 15:50:29.568166 mkdocsi-1.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-28 15:50:19.000000 mkdocsi-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:50:29.566166 mkdocsi-1.0.2/mkdocsi/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-05-28 15:50:19.000000 mkdocsi-1.0.2/mkdocsi/Main.py
+-rw-rw-rw-   0 root         (0) root         (0)     5013 2024-05-28 15:50:19.000000 mkdocsi-1.0.2/mkdocsi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:50:29.568166 mkdocsi-1.0.2/mkdocsi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      582 2024-05-28 15:50:29.000000 mkdocsi-1.0.2/mkdocsi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2024-05-28 15:50:29.000000 mkdocsi-1.0.2/mkdocsi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 15:50:29.000000 mkdocsi-1.0.2/mkdocsi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-05-28 15:50:29.000000 mkdocsi-1.0.2/mkdocsi.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-28 15:50:29.000000 mkdocsi-1.0.2/mkdocsi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-28 15:50:29.000000 mkdocsi-1.0.2/mkdocsi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 15:50:29.568166 mkdocsi-1.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3042 2024-05-28 15:50:19.000000 mkdocsi-1.0.2/setup.py
```

### Comparing `mkdocsi-1.0.1/PKG-INFO` & `mkdocsi-1.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.0.1
+Version: 1.0.2
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: bashi
+Requires-Dist: mkdocs
+Requires-Dist: mkdocs-material
 
 # nested-docs
 
 
 ## Installation : 
 ```bash
 pip install nested-docs
```

### Comparing `mkdocsi-1.0.1/mkdocsi/__init__.py` & `mkdocsi-1.0.2/mkdocsi/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import yaml  , os , json , sys 
 from glob import glob 
 
 
 class MkdocsUtils : 
-    def __init__(self , docs_folder  ,  mkdocs_file  ) : 
-        self.mkdocs_file = os.path.abspath(mkdocs_file)
-        self.mkdocs_data = None 
+    def __init__(self , docs_folder  ,  Template_mkdocs_file  ) : 
+        self.Template_mkdocs_file = os.path.abspath(Template_mkdocs_file)
+        self.Template_mkdocs_file = None 
         self.docs_folder = os.path.abspath(docs_folder)  
-        with open(self.mkdocs_file, 'r') as f: self.mkdocs_data = yaml.safe_load(f)
+        with open(self.Template_mkdocs_file, 'r') as f: self.mkdocs_data = yaml.safe_load(f)
 
     def __repr__(self) : 
         return json.dumps(self.mkdocs_data , indent = 4 )
 
     def buildTree(self) : 
         self.mkdocs_data['nav'] = self.get_md_files_tree() 
-        output_file = "./test.yml"
-        output_file = "/home/ismhadhb@actia.local/Music/dev/mkdocs/mkdocs.yml"
+        output_file = os.path.join(self.docs_folder , "mkdocs.yml")
         with open(output_file, 'w') as file:                                                                                                                                                       
             yaml.dump(self.mkdocs_data, file, default_flow_style=False)       
                                                                                                                                                                                           
     def to_camel_case(self , snake_str):                                                                                                                                                                  
         components = snake_str.split('_')   
         print(components)                                                                                                                                                       
         return " ".join(components)
```

### Comparing `mkdocsi-1.0.1/mkdocsi.egg-info/PKG-INFO` & `mkdocsi-1.0.2/mkdocsi.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: mkdocsi
-Version: 1.0.1
+Version: 1.0.2
 Summary: convert docs folder to mkdocs site , dynamic nested docs and folders
 Home-page: https://gitlab.com/isampypi/mkdocsi
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: bashi
+Requires-Dist: mkdocs
+Requires-Dist: mkdocs-material
 
 # nested-docs
 
 
 ## Installation : 
 ```bash
 pip install nested-docs
```

### Comparing `mkdocsi-1.0.1/setup.py` & `mkdocsi-1.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             packages=find_packages(),
             author= author  ,
             author_email=author_email   ,
             description= description,
             long_description=open("README.md").read(),
             long_description_content_type="text/markdown",
             url= url    ,
-            install_requires=["bashi"]  ,
+            install_requires=["mkdocs" , "mkdocs-material"  ]  ,
             classifiers=[
                 'Programming Language :: Python :: 3',
                 'License :: OSI Approved :: MIT License',
                 'Operating System :: OS Independent',
             ],
             entry_points={
                 'console_scripts': [
```

