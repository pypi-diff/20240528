# Comparing `tmp/jaanca_utils_os-0.1.1.tar.gz` & `tmp/jaanca_utils_os-0.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca_utils_os-0.1.1.tar", last modified: Mon May 27 23:23:51 2024, max compression
+gzip compressed data, was "jaanca_utils_os-0.1.2rc1.tar", last modified: Mon May 27 23:45:04 2024, max compression
```

## Comparing `jaanca_utils_os-0.1.1.tar` & `jaanca_utils_os-0.1.2rc1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 23:23:51.343792 jaanca_utils_os-0.1.1/
--rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0    10964 2024-05-27 23:23:51.342793 jaanca_utils_os-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     9557 2024-05-27 23:23:26.000000 jaanca_utils_os-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 23:23:51.316795 jaanca_utils_os-0.1.1/jaanca_utils_os/
--rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.1.1/jaanca_utils_os/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 23:23:51.327794 jaanca_utils_os-0.1.1/jaanca_utils_os/utils/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.1/jaanca_utils_os/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 23:23:51.338793 jaanca_utils_os-0.1.1/jaanca_utils_os/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.1/jaanca_utils_os/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     5442 2024-05-27 23:20:08.000000 jaanca_utils_os-0.1.1/jaanca_utils_os/utils/helpers/environment_parser_loader.py
--rw-rw-rw-   0        0        0     6835 2024-05-27 22:01:52.000000 jaanca_utils_os-0.1.1/jaanca_utils_os/utils/helpers/file_folder_management.py
--rw-rw-rw-   0        0        0     3289 2024-05-27 22:09:16.000000 jaanca_utils_os-0.1.1/jaanca_utils_os/utils/helpers/file_properties.py
--rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.1.1/jaanca_utils_os/utils/helpers/parse_bool.py
--rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.1.1/jaanca_utils_os/utils/helpers/parse_types.py
-drwxrwxrwx   0        0        0        0 2024-05-27 23:23:51.341794 jaanca_utils_os-0.1.1/jaanca_utils_os.egg-info/
--rw-rw-rw-   0        0        0    10964 2024-05-27 23:23:51.000000 jaanca_utils_os-0.1.1/jaanca_utils_os.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      591 2024-05-27 23:23:51.000000 jaanca_utils_os-0.1.1/jaanca_utils_os.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 23:23:51.000000 jaanca_utils_os-0.1.1/jaanca_utils_os.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-27 23:23:51.000000 jaanca_utils_os-0.1.1/jaanca_utils_os.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-27 23:23:51.000000 jaanca_utils_os-0.1.1/jaanca_utils_os.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 23:23:51.345792 jaanca_utils_os-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1756 2024-05-27 23:23:06.000000 jaanca_utils_os-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 23:45:04.549275 jaanca_utils_os-0.1.2rc1/
+-rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.2rc1/LICENSE.txt
+-rw-rw-rw-   0        0        0    10967 2024-05-27 23:45:04.548314 jaanca_utils_os-0.1.2rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     9557 2024-05-27 23:23:26.000000 jaanca_utils_os-0.1.2rc1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 23:45:04.513117 jaanca_utils_os-0.1.2rc1/jaanca_utils_os/
+-rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 23:45:04.526121 jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 23:45:04.542275 jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     5526 2024-05-27 23:44:11.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/helpers/environment_parser_loader.py
+-rw-rw-rw-   0        0        0     6835 2024-05-27 22:01:52.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/helpers/file_folder_management.py
+-rw-rw-rw-   0        0        0     3289 2024-05-27 22:09:16.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/helpers/file_properties.py
+-rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/helpers/parse_bool.py
+-rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/helpers/parse_types.py
+drwxrwxrwx   0        0        0        0 2024-05-27 23:45:04.545277 jaanca_utils_os-0.1.2rc1/jaanca_utils_os.egg-info/
+-rw-rw-rw-   0        0        0    10967 2024-05-27 23:45:04.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      591 2024-05-27 23:45:04.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 23:45:04.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-27 23:45:04.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-27 23:45:04.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 23:45:04.551285 jaanca_utils_os-0.1.2rc1/setup.cfg
+-rw-rw-rw-   0        0        0     1759 2024-05-27 23:42:16.000000 jaanca_utils_os-0.1.2rc1/setup.py
```

### Comparing `jaanca_utils_os-0.1.1/LICENSE.txt` & `jaanca_utils_os-0.1.2rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.1/PKG-INFO` & `jaanca_utils_os-0.1.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-utils-os
-Version: 0.1.1
+Version: 0.1.2rc1
 Summary: A tool library created by jaanca with operating system help functions such as reading environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: datetime,utc
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.1 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.2rc1 Summary: A tool
 library created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com
 License: MIT License Keywords: datetime,utc Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
```

### Comparing `jaanca_utils_os-0.1.1/README.md` & `jaanca_utils_os-0.1.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.1/jaanca_utils_os/__init__.py` & `jaanca_utils_os-0.1.2rc1/jaanca_utils_os/__init__.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.1/jaanca_utils_os/utils/helpers/environment_parser_loader.py` & `jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/helpers/environment_parser_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,17 @@
             myTable.add_row([attribute_name, attribute_type.__name__, attribute_value])
         print(myTable)        
 
     print_attributes(settings)
 
     ```
     '''
-    def __init__(self,cls,env_full_path:str):
+    def __init__(self,cls,env_full_path:str=''):
+        if env_full_path == '':
+            env_full_path = Path('.') / '.env'
         load_dotenv(dotenv_path=env_full_path)
         for key, value in vars(cls).items():
             if not key.startswith('__'):
                 default_value = None
                 if isinstance(value,tuple) or isinstance(value,list):
                     default_value=value[1]
                     value=value[0]
```

### Comparing `jaanca_utils_os-0.1.1/jaanca_utils_os/utils/helpers/file_folder_management.py` & `jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/helpers/file_folder_management.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.1/jaanca_utils_os/utils/helpers/file_properties.py` & `jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/helpers/file_properties.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.1/jaanca_utils_os/utils/helpers/parse_bool.py` & `jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/helpers/parse_bool.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.1/jaanca_utils_os/utils/helpers/parse_types.py` & `jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/helpers/parse_types.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.1/jaanca_utils_os.egg-info/PKG-INFO` & `jaanca_utils_os-0.1.2rc1/jaanca_utils_os.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-utils-os
-Version: 0.1.1
+Version: 0.1.2rc1
 Summary: A tool library created by jaanca with operating system help functions such as reading environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: datetime,utc
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.1 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.2rc1 Summary: A tool
 library created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com
 License: MIT License Keywords: datetime,utc Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
```

### Comparing `jaanca_utils_os-0.1.1/jaanca_utils_os.egg-info/SOURCES.txt` & `jaanca_utils_os-0.1.2rc1/jaanca_utils_os.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.1/setup.py` & `jaanca_utils_os-0.1.2rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca-utils-os"
-VERSION = "0.1.1"
+VERSION = "0.1.2rc1"
 
 install_requires = [""]
 extras_require = {
     "dotenv": "python-dotenv>=1.0.1"
 }
 
 setup(
```

