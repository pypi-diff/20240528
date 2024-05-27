# Comparing `tmp/jaanca_utils_os-0.1.2rc1.tar.gz` & `tmp/jaanca_utils_os-0.1.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca_utils_os-0.1.2rc1.tar", last modified: Mon May 27 23:45:04 2024, max compression
+gzip compressed data, was "jaanca_utils_os-0.1.2rc2.tar", last modified: Mon May 27 23:54:30 2024, max compression
```

## Comparing `jaanca_utils_os-0.1.2rc1.tar` & `jaanca_utils_os-0.1.2rc2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 23:45:04.549275 jaanca_utils_os-0.1.2rc1/
--rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.2rc1/LICENSE.txt
--rw-rw-rw-   0        0        0    10967 2024-05-27 23:45:04.548314 jaanca_utils_os-0.1.2rc1/PKG-INFO
--rw-rw-rw-   0        0        0     9557 2024-05-27 23:23:26.000000 jaanca_utils_os-0.1.2rc1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 23:45:04.513117 jaanca_utils_os-0.1.2rc1/jaanca_utils_os/
--rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 23:45:04.526121 jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 23:45:04.542275 jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     5526 2024-05-27 23:44:11.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/helpers/environment_parser_loader.py
--rw-rw-rw-   0        0        0     6835 2024-05-27 22:01:52.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/helpers/file_folder_management.py
--rw-rw-rw-   0        0        0     3289 2024-05-27 22:09:16.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/helpers/file_properties.py
--rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/helpers/parse_bool.py
--rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/helpers/parse_types.py
-drwxrwxrwx   0        0        0        0 2024-05-27 23:45:04.545277 jaanca_utils_os-0.1.2rc1/jaanca_utils_os.egg-info/
--rw-rw-rw-   0        0        0    10967 2024-05-27 23:45:04.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      591 2024-05-27 23:45:04.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 23:45:04.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-27 23:45:04.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-27 23:45:04.000000 jaanca_utils_os-0.1.2rc1/jaanca_utils_os.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 23:45:04.551285 jaanca_utils_os-0.1.2rc1/setup.cfg
--rw-rw-rw-   0        0        0     1759 2024-05-27 23:42:16.000000 jaanca_utils_os-0.1.2rc1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 23:54:30.603018 jaanca_utils_os-0.1.2rc2/
+-rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.2rc2/LICENSE.txt
+-rw-rw-rw-   0        0        0    10967 2024-05-27 23:54:30.602014 jaanca_utils_os-0.1.2rc2/PKG-INFO
+-rw-rw-rw-   0        0        0     9557 2024-05-27 23:23:26.000000 jaanca_utils_os-0.1.2rc2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 23:54:30.572486 jaanca_utils_os-0.1.2rc2/jaanca_utils_os/
+-rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.1.2rc2/jaanca_utils_os/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 23:54:30.583489 jaanca_utils_os-0.1.2rc2/jaanca_utils_os/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.2rc2/jaanca_utils_os/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 23:54:30.597005 jaanca_utils_os-0.1.2rc2/jaanca_utils_os/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.2rc2/jaanca_utils_os/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     5671 2024-05-27 23:53:55.000000 jaanca_utils_os-0.1.2rc2/jaanca_utils_os/utils/helpers/environment_parser_loader.py
+-rw-rw-rw-   0        0        0     6835 2024-05-27 22:01:52.000000 jaanca_utils_os-0.1.2rc2/jaanca_utils_os/utils/helpers/file_folder_management.py
+-rw-rw-rw-   0        0        0     3289 2024-05-27 22:09:16.000000 jaanca_utils_os-0.1.2rc2/jaanca_utils_os/utils/helpers/file_properties.py
+-rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.1.2rc2/jaanca_utils_os/utils/helpers/parse_bool.py
+-rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.1.2rc2/jaanca_utils_os/utils/helpers/parse_types.py
+drwxrwxrwx   0        0        0        0 2024-05-27 23:54:30.599018 jaanca_utils_os-0.1.2rc2/jaanca_utils_os.egg-info/
+-rw-rw-rw-   0        0        0    10967 2024-05-27 23:54:30.000000 jaanca_utils_os-0.1.2rc2/jaanca_utils_os.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      591 2024-05-27 23:54:30.000000 jaanca_utils_os-0.1.2rc2/jaanca_utils_os.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 23:54:30.000000 jaanca_utils_os-0.1.2rc2/jaanca_utils_os.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-27 23:54:30.000000 jaanca_utils_os-0.1.2rc2/jaanca_utils_os.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-27 23:54:30.000000 jaanca_utils_os-0.1.2rc2/jaanca_utils_os.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 23:54:30.605018 jaanca_utils_os-0.1.2rc2/setup.cfg
+-rw-rw-rw-   0        0        0     1759 2024-05-27 23:54:21.000000 jaanca_utils_os-0.1.2rc2/setup.py
```

### Comparing `jaanca_utils_os-0.1.2rc1/LICENSE.txt` & `jaanca_utils_os-0.1.2rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.2rc1/PKG-INFO` & `jaanca_utils_os-0.1.2rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-utils-os
-Version: 0.1.2rc1
+Version: 0.1.2rc2
 Summary: A tool library created by jaanca with operating system help functions such as reading environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: datetime,utc
 Classifier: Development Status :: 4 - Beta
@@ -23,15 +23,15 @@
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Provides-Extra: dotenv
-Requires-Dist: python-dotenv>=1.0.1; extra == "dotenv"
+Requires-Dist: python-dotenv>=1.0.0; extra == "dotenv"
 
 <p align="center">
     <em>jaanca public libraries</em>
 </p>
 
 <p align="center">
 <a href="https://pypi.org/project/jaanca-utils-os" target="_blank">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.2rc1 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.2rc2 Summary: A tool
 library created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com
 License: MIT License Keywords: datetime,utc Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
@@ -11,15 +11,15 @@
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Software Development Classifier: Typing :: Typed Requires-
 Python: >=3.8 Description-Content-Type: text/markdown License-File: LICENSE.txt
-Provides-Extra: dotenv Requires-Dist: python-dotenv>=1.0.1; extra == "dotenv"
+Provides-Extra: dotenv Requires-Dist: python-dotenv>=1.0.0; extra == "dotenv"
                             jjaaaannccaa ppuubblliicc lliibbrraarriieess
                            _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]
 --- # A tool library created by jaanca * **Python library**: A tool library
 created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others. *
 **EnvironmentParserLoader**: A class that loads, parses, and manages system
 environment variables into various data types. General Functionality ## The
```

### Comparing `jaanca_utils_os-0.1.2rc1/README.md` & `jaanca_utils_os-0.1.2rc2/README.md`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.2rc1/jaanca_utils_os/__init__.py` & `jaanca_utils_os-0.1.2rc2/jaanca_utils_os/__init__.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/helpers/environment_parser_loader.py` & `jaanca_utils_os-0.1.2rc2/jaanca_utils_os/utils/helpers/environment_parser_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,21 +83,23 @@
         BOOL_FALSE_TWO = "BOOL_FALSE_TWO"
         BOOL_FALSE_INCORRECT = "BOOL_FALSE_INCORRECT"
         NO_DATA_TUPLE = ("VARIABLE","Not Exist")
         NO_DATA_LIST = ["VARIABLE","Not Exist"]
         NO_DATA_BOOL = ["VARIABLE","1"]
 
     # Load varibles from current folder
-    env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env")
+    # env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env")
     # Load varibles from current folder and subfolders
     # env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env",folder_list=["folder2"])
     # Load varibles from disk path: c:\tmp
     # env_full_path = FileFolderManagement.build_full_path_to_file("c:",file_name=".env",folder_list=["tmp"])
 
-    settings = EnvironmentParserLoader(Environment,env_full_path=env_full_path)
+    # Run the script from where the default environment variables .env file is located
+    settings = EnvironmentParserLoader(Environment)
+    # settings = EnvironmentParserLoader(Environment,env_full_path=env_full_path)
 
     def print_attributes(cls):
         columns = ["Name", "Type", "Value"]
         myTable = PrettyTable(columns)
         for attribute_name, attribute_value in vars(cls).items():
             attribute_type = type(attribute_value)
             myTable.add_row([attribute_name, attribute_type.__name__, attribute_value])
```

### Comparing `jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/helpers/file_folder_management.py` & `jaanca_utils_os-0.1.2rc2/jaanca_utils_os/utils/helpers/file_folder_management.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/helpers/file_properties.py` & `jaanca_utils_os-0.1.2rc2/jaanca_utils_os/utils/helpers/file_properties.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/helpers/parse_bool.py` & `jaanca_utils_os-0.1.2rc2/jaanca_utils_os/utils/helpers/parse_bool.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.2rc1/jaanca_utils_os/utils/helpers/parse_types.py` & `jaanca_utils_os-0.1.2rc2/jaanca_utils_os/utils/helpers/parse_types.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.2rc1/jaanca_utils_os.egg-info/PKG-INFO` & `jaanca_utils_os-0.1.2rc2/jaanca_utils_os.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-utils-os
-Version: 0.1.2rc1
+Version: 0.1.2rc2
 Summary: A tool library created by jaanca with operating system help functions such as reading environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: datetime,utc
 Classifier: Development Status :: 4 - Beta
@@ -23,15 +23,15 @@
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Provides-Extra: dotenv
-Requires-Dist: python-dotenv>=1.0.1; extra == "dotenv"
+Requires-Dist: python-dotenv>=1.0.0; extra == "dotenv"
 
 <p align="center">
     <em>jaanca public libraries</em>
 </p>
 
 <p align="center">
 <a href="https://pypi.org/project/jaanca-utils-os" target="_blank">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.2rc1 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.2rc2 Summary: A tool
 library created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com
 License: MIT License Keywords: datetime,utc Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
@@ -11,15 +11,15 @@
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Software Development Classifier: Typing :: Typed Requires-
 Python: >=3.8 Description-Content-Type: text/markdown License-File: LICENSE.txt
-Provides-Extra: dotenv Requires-Dist: python-dotenv>=1.0.1; extra == "dotenv"
+Provides-Extra: dotenv Requires-Dist: python-dotenv>=1.0.0; extra == "dotenv"
                             jjaaaannccaa ppuubblliicc lliibbrraarriieess
                            _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]
 --- # A tool library created by jaanca * **Python library**: A tool library
 created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others. *
 **EnvironmentParserLoader**: A class that loads, parses, and manages system
 environment variables into various data types. General Functionality ## The
```

### Comparing `jaanca_utils_os-0.1.2rc1/jaanca_utils_os.egg-info/SOURCES.txt` & `jaanca_utils_os-0.1.2rc2/jaanca_utils_os.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.2rc1/setup.py` & `jaanca_utils_os-0.1.2rc2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca-utils-os"
-VERSION = "0.1.2rc1"
+VERSION = "0.1.2rc2"
 
 install_requires = [""]
 extras_require = {
-    "dotenv": "python-dotenv>=1.0.1"
+    "dotenv": "python-dotenv>=1.0.0"
 }
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'A tool library created by {COMPANY_NAME} with operating system help functions such as reading environment variables, reading/writing files, file properties, among others.',
     long_description=open('README.md', 'r').read(),
```

