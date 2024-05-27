# Comparing `tmp/jaanca_utils_os-0.0.1rc5.tar.gz` & `tmp/jaanca_utils_os-0.0.1rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca_utils_os-0.0.1rc5.tar", last modified: Mon May 27 21:28:24 2024, max compression
+gzip compressed data, was "jaanca_utils_os-0.0.1rc6.tar", last modified: Mon May 27 22:12:21 2024, max compression
```

## Comparing `jaanca_utils_os-0.0.1rc5.tar` & `jaanca_utils_os-0.0.1rc6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 21:28:24.359658 jaanca_utils_os-0.0.1rc5/
--rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc5/LICENSE.txt
--rw-rw-rw-   0        0        0     3980 2024-05-27 21:28:24.359658 jaanca_utils_os-0.0.1rc5/PKG-INFO
--rw-rw-rw-   0        0        0     2655 2024-05-27 20:05:31.000000 jaanca_utils_os-0.0.1rc5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 21:28:24.333657 jaanca_utils_os-0.0.1rc5/jaanca_utils_os/
--rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.0.1rc5/jaanca_utils_os/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 21:28:24.344658 jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 21:28:24.355659 jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     2130 2024-05-27 21:28:03.000000 jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/helpers/environment_parser_loader.py
--rw-rw-rw-   0        0        0     6786 2024-05-27 21:23:44.000000 jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/helpers/file_folder_management.py
--rw-rw-rw-   0        0        0     3213 2024-05-27 19:49:12.000000 jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/helpers/file_properties.py
--rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/helpers/parse_bool.py
--rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/helpers/parse_types.py
-drwxrwxrwx   0        0        0        0 2024-05-27 21:28:24.357660 jaanca_utils_os-0.0.1rc5/jaanca_utils_os.egg-info/
--rw-rw-rw-   0        0        0     3980 2024-05-27 21:28:24.000000 jaanca_utils_os-0.0.1rc5/jaanca_utils_os.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2024-05-27 21:28:24.000000 jaanca_utils_os-0.0.1rc5/jaanca_utils_os.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 21:28:24.000000 jaanca_utils_os-0.0.1rc5/jaanca_utils_os.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-27 21:28:24.000000 jaanca_utils_os-0.0.1rc5/jaanca_utils_os.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 21:28:24.361658 jaanca_utils_os-0.0.1rc5/setup.cfg
--rw-rw-rw-   0        0        0     1662 2024-05-27 21:28:14.000000 jaanca_utils_os-0.0.1rc5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:12:21.446790 jaanca_utils_os-0.0.1rc6/
+-rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc6/LICENSE.txt
+-rw-rw-rw-   0        0        0    10105 2024-05-27 22:12:21.445790 jaanca_utils_os-0.0.1rc6/PKG-INFO
+-rw-rw-rw-   0        0        0     8775 2024-05-27 22:11:48.000000 jaanca_utils_os-0.0.1rc6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 22:12:21.421789 jaanca_utils_os-0.0.1rc6/jaanca_utils_os/
+-rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.0.1rc6/jaanca_utils_os/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:12:21.430790 jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:12:21.441789 jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     4699 2024-05-27 21:37:19.000000 jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/helpers/environment_parser_loader.py
+-rw-rw-rw-   0        0        0     6835 2024-05-27 22:01:52.000000 jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/helpers/file_folder_management.py
+-rw-rw-rw-   0        0        0     3289 2024-05-27 22:09:16.000000 jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/helpers/file_properties.py
+-rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/helpers/parse_bool.py
+-rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/helpers/parse_types.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:12:21.444790 jaanca_utils_os-0.0.1rc6/jaanca_utils_os.egg-info/
+-rw-rw-rw-   0        0        0    10105 2024-05-27 22:12:21.000000 jaanca_utils_os-0.0.1rc6/jaanca_utils_os.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2024-05-27 22:12:21.000000 jaanca_utils_os-0.0.1rc6/jaanca_utils_os.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 22:12:21.000000 jaanca_utils_os-0.0.1rc6/jaanca_utils_os.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-27 22:12:21.000000 jaanca_utils_os-0.0.1rc6/jaanca_utils_os.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 22:12:21.447792 jaanca_utils_os-0.0.1rc6/setup.cfg
+-rw-rw-rw-   0        0        0     1662 2024-05-27 22:12:16.000000 jaanca_utils_os-0.0.1rc6/setup.py
```

### Comparing `jaanca_utils_os-0.0.1rc5/LICENSE.txt` & `jaanca_utils_os-0.0.1rc6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc5/jaanca_utils_os/__init__.py` & `jaanca_utils_os-0.0.1rc6/jaanca_utils_os/__init__.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/helpers/file_folder_management.py` & `jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/helpers/file_folder_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,24 @@
         '''Description
         Create the full path to reach the file or folders structure.
         :param path_base:str: Use the __file__ parameter, as the path of the current execution file.
 
         ## Example:
         
         ```Phython
-        from file_management import FileFolderManagement
+        from jaanca_utils_os import FileFolderManagement
 
         # root path
-        folder_list = ["folder1", "folder2","file_name"]
-        print(f"Full path from current folder: {FileFolderManagement.build_full_path_from_current_folder(__file__)}")
+        path=FileFolderManagement.build_full_path_from_current_folder(__file__,filename="filename.txt")
+        print(f"Full path from current folder: {path}")
 
         # subfolders path from current folder
-        folder_list = ["folder1", "folder2","file_name"]
-        print(f"Full path from current folder: {FileFolderManagement.build_full_path_from_current_folder(__file__)}")
+        folder_list = ["folder1", "folder2"]
+        path=FileFolderManagement.build_full_path_from_current_folder(__file__,folder_list=folder_list,filename="filename.txt")
+        print(f"Full path from current folder: {path}")
         ```
         '''
         folder_path=os.path.abspath(os.path.join(os.path.dirname(path_base),cls.get_folder_path(folder_list)))
         return os.path.abspath(os.path.join(folder_path,filename))
     
     @classmethod
     def build_full_path_to_file(cls,drive:str, file_name:str, folder_list:list[str]=[])->str:
@@ -50,15 +51,15 @@
 
         :param: drive str               : Disk letter in windows or mount point in unix, examples: "c:", "d:", "/", "/home"
         :param: filename:str            : Filename with extesion
         :param: folder_list:list[str]   : Complete folders until you reach the file,  example: ["folder1", "folder2"]
         :return str                     : Joins the arguments received into a disk path according to the operating system
         ## Example:
         ```Python
-        from file_management import FileFolderManagement
+        from jaanca_utils_os import FileFolderManagement
 
         # root path
         file_name = "hello.txt"
         file_name_full_path = FileFolderManagement.build_full_path_to_file("c:",file_name)
         file_name_full_path_without_file_name = FileFolderManagement.build_full_path_to_file("c:",file_name='')
         print(f"file_name_full_path={file_name_full_path}")
         print(f"file_name_full_path_without_file_name={file_name_full_path_without_file_name}")
@@ -113,20 +114,19 @@
 
     def write_to_disk(self,text:str)->tuple[bool,str]:
         '''Description
         :return status:bool,error_msg:str: False/True if the file is written correctly, if there was an error the Exception message. 
 
         ## Example
         ```Python
-
-        from file_management import FileFolderManagement
+        from jaanca_utils_os import FileFolderManagement
 
         # Write file to current folder
         file_name="hello.txt"
-        current_folder=FileFolderManagement.get_current_folder()
+        current_folder=FileFolderManagement.build_full_path_from_current_folder(__file__)
         folders=FileFolderManagement.get_folder_list(current_folder)
         file_name_full_path = FileFolderManagement.build_full_path_to_file("c:",file_name,folders)
         text = """Hello world !
         Hello world !"""
         status,error_msg=FileFolderManagement(file_name_full_path).write_to_disk(text)
         if(status):
             print("file created successfully: "+file_name_full_path)
@@ -138,15 +138,16 @@
         file_name_full_path = FileFolderManagement.build_full_path_to_file("c:",file_name)
         text = """Hello world !
         Hello world !"""
         status,error_msg=FileFolderManagement(file_name_full_path).write_to_disk(text)
         if(status):
             print("file created successfully: "+file_name_full_path)
         else:
-            print("error:" + error_msg)                
+            print("error:" + error_msg)
+
         ```
         '''
         error_msg=''
         status=True
         try:
             with FileFolderManagement(self.filename) as f:
                 for line in text:
```

### Comparing `jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/helpers/file_properties.py` & `jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/helpers/file_properties.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,40 +3,35 @@
 import os
 
 
 class FilePropertiesErrorCodes(StrEnum):
     ATTRIBUTES_READING_ERROR = "File not found error or there is an error reading the file attributes"
 
 class FileProperties:
-    """Blob Properties.
+    """File Properties.
+    Functionalities to read properties of an operating system file, such as: modification date, creation, size in bytes, among others.
     
     ## Example
 
     ```Python
 
-    from file_properties import FileProperties
+    from jaanca_utils_os import FileProperties, FileFolderManagement
     import json
-    import os
-
-    from file_properties import FileProperties
-    import json
-    import os
 
     file_name="hello asa s sas. as as a. as as .txt"
-    file_name_full_path_from_actual_folder=os.path.abspath(os.path.join(os.path.dirname(__file__),file_name))
-    file_properties=FileProperties(file_name_full_path_from_actual_folder)
+    filename_full_path_from_current_folder=FileFolderManagement.build_full_path_from_current_folder(__file__,folder_list=["file"])
+    file_properties=FileProperties(filename_full_path_from_current_folder)
     status = file_properties.get_attribute_reading_status()
     if status is True:
         print(json.dumps(file_properties.get_dict(),indent=4))
         print(f"name:{file_properties.name}")
         print(f"extension:{file_properties.extension}")
         print(f"modification_date:{file_properties.modification_date}")
     else:
-        print(status)    
-        
+        print(status)        
     ```
     
     """
     name:str
     """File name."""
     extension:str
     """Filename extension."""
```

### Comparing `jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/helpers/parse_bool.py` & `jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/helpers/parse_bool.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/helpers/parse_types.py` & `jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/helpers/parse_types.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc5/jaanca_utils_os.egg-info/SOURCES.txt` & `jaanca_utils_os-0.0.1rc6/jaanca_utils_os.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc5/setup.py` & `jaanca_utils_os-0.0.1rc6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca-utils-os"
-VERSION = "0.0.1rc5"
+VERSION = "0.0.1rc6"
 
 install_requires = [""]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'A tool library created by {COMPANY_NAME} with operating system help functions such as reading environment variables, reading/writing files, file properties, among others.',
```

