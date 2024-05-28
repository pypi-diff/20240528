# Comparing `tmp/jaanca_utils_os-0.1.4.tar.gz` & `tmp/jaanca_utils_os-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca_utils_os-0.1.4.tar", last modified: Tue May 28 00:00:29 2024, max compression
+gzip compressed data, was "jaanca_utils_os-0.1.5.tar", last modified: Tue May 28 00:03:42 2024, max compression
```

## Comparing `jaanca_utils_os-0.1.4.tar` & `jaanca_utils_os-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 00:00:29.772829 jaanca_utils_os-0.1.4/
--rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0    10892 2024-05-28 00:00:29.771827 jaanca_utils_os-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     9485 2024-05-28 00:00:21.000000 jaanca_utils_os-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 00:00:29.745129 jaanca_utils_os-0.1.4/jaanca_utils_os/
--rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.1.4/jaanca_utils_os/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 00:00:29.757577 jaanca_utils_os-0.1.4/jaanca_utils_os/utils/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.4/jaanca_utils_os/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 00:00:29.767928 jaanca_utils_os-0.1.4/jaanca_utils_os/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.4/jaanca_utils_os/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     5671 2024-05-27 23:53:55.000000 jaanca_utils_os-0.1.4/jaanca_utils_os/utils/helpers/environment_parser_loader.py
--rw-rw-rw-   0        0        0     6835 2024-05-27 22:01:52.000000 jaanca_utils_os-0.1.4/jaanca_utils_os/utils/helpers/file_folder_management.py
--rw-rw-rw-   0        0        0     3289 2024-05-27 22:09:16.000000 jaanca_utils_os-0.1.4/jaanca_utils_os/utils/helpers/file_properties.py
--rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.1.4/jaanca_utils_os/utils/helpers/parse_bool.py
--rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.1.4/jaanca_utils_os/utils/helpers/parse_types.py
-drwxrwxrwx   0        0        0        0 2024-05-28 00:00:29.769827 jaanca_utils_os-0.1.4/jaanca_utils_os.egg-info/
--rw-rw-rw-   0        0        0    10892 2024-05-28 00:00:29.000000 jaanca_utils_os-0.1.4/jaanca_utils_os.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      591 2024-05-28 00:00:29.000000 jaanca_utils_os-0.1.4/jaanca_utils_os.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 00:00:29.000000 jaanca_utils_os-0.1.4/jaanca_utils_os.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-28 00:00:29.000000 jaanca_utils_os-0.1.4/jaanca_utils_os.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-28 00:00:29.000000 jaanca_utils_os-0.1.4/jaanca_utils_os.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 00:00:29.773827 jaanca_utils_os-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1756 2024-05-27 23:59:47.000000 jaanca_utils_os-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 00:03:42.719653 jaanca_utils_os-0.1.5/
+-rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0    10991 2024-05-28 00:03:42.718677 jaanca_utils_os-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     9584 2024-05-28 00:03:02.000000 jaanca_utils_os-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 00:03:42.692786 jaanca_utils_os-0.1.5/jaanca_utils_os/
+-rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.1.5/jaanca_utils_os/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 00:03:42.703728 jaanca_utils_os-0.1.5/jaanca_utils_os/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.5/jaanca_utils_os/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 00:03:42.714622 jaanca_utils_os-0.1.5/jaanca_utils_os/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.5/jaanca_utils_os/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     5663 2024-05-28 00:03:33.000000 jaanca_utils_os-0.1.5/jaanca_utils_os/utils/helpers/environment_parser_loader.py
+-rw-rw-rw-   0        0        0     6835 2024-05-27 22:01:52.000000 jaanca_utils_os-0.1.5/jaanca_utils_os/utils/helpers/file_folder_management.py
+-rw-rw-rw-   0        0        0     3289 2024-05-27 22:09:16.000000 jaanca_utils_os-0.1.5/jaanca_utils_os/utils/helpers/file_properties.py
+-rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.1.5/jaanca_utils_os/utils/helpers/parse_bool.py
+-rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.1.5/jaanca_utils_os/utils/helpers/parse_types.py
+drwxrwxrwx   0        0        0        0 2024-05-28 00:03:42.716636 jaanca_utils_os-0.1.5/jaanca_utils_os.egg-info/
+-rw-rw-rw-   0        0        0    10991 2024-05-28 00:03:42.000000 jaanca_utils_os-0.1.5/jaanca_utils_os.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      591 2024-05-28 00:03:42.000000 jaanca_utils_os-0.1.5/jaanca_utils_os.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 00:03:42.000000 jaanca_utils_os-0.1.5/jaanca_utils_os.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-28 00:03:42.000000 jaanca_utils_os-0.1.5/jaanca_utils_os.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-28 00:03:42.000000 jaanca_utils_os-0.1.5/jaanca_utils_os.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 00:03:42.720654 jaanca_utils_os-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1756 2024-05-28 00:03:10.000000 jaanca_utils_os-0.1.5/setup.py
```

### Comparing `jaanca_utils_os-0.1.4/LICENSE.txt` & `jaanca_utils_os-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.4/PKG-INFO` & `jaanca_utils_os-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-utils-os
-Version: 0.1.4
+Version: 0.1.5
 Summary: A tool library created by jaanca with operating system help functions such as reading environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: datetime,utc
 Classifier: Development Status :: 4 - Beta
@@ -63,16 +63,15 @@
 | [Package (PyPI)](https://pypi.org/project/jaanca-utils-os/)
 | [Samples](https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os/samples)
 
 ---
 
 # library installation
 ```console    
-pip install prettytable==3.10.0
-pip install python-dotenv==1.0.0
+pip install python-dotenv --upgrade
 pip install jaanca_utils_os[dotenv] --upgrade
 ```
 
 ---
 # environment_parser_loader: Example of use
 
 ### Considerations on environmental variables
@@ -131,20 +130,22 @@
     NO_DATA_TUPLE = ("VARIABLE","Not Exist")
     NO_DATA_LIST = ["VARIABLE","Not Exist"]
     NO_DATA_BOOL = ["VARIABLE","1"]
 
 # Load varibles from current folder
 env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env")
 # Load varibles from current folder and subfolders
-# env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env",folder_list=["folder2"])
+env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env",folder_list=["folder2"])
 # Load varibles from disk path: c:\tmp
-# env_full_path = FileFolderManagement.build_full_path_to_file("c:",file_name=".env",folder_list=["tmp"])
-
+env_full_path = FileFolderManagement.build_full_path_to_file("c:",file_name=".env",folder_list=["tmp"])
 settings = EnvironmentParserLoader(Environment,env_full_path=env_full_path)
 
+# Run the script from where the default environment variables .env file is located
+settings = EnvironmentParserLoader(Environment)
+
 def print_attributes(cls):
     columns = ["Name", "Type", "Value"]
     myTable = PrettyTable(columns)
     for attribute_name, attribute_value in vars(cls).items():
         attribute_type = type(attribute_value)
         myTable.add_row([attribute_name, attribute_type.__name__, attribute_value])
     print(myTable)        
@@ -264,11 +265,11 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 ## [0.0.1rcX] - 2024-05-27
 ### Added
 - First tests using pypi.org in develop environment.
 
-## [0.1.1-4] - 2024-05-27
+## [0.1.1-5] - 2024-05-27
 ### Added
 - Completion of testing and launch into production.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.4 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.5 Summary: A tool
 library created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com
 License: MIT License Keywords: datetime,utc Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
@@ -31,50 +31,52 @@
 a default value is not assigned, a KeyError exception will be returned. *
 **FileFolderManagement**: To write files, use the write_to_disk() method *
 **FileProperties**: Functionalities to read properties of an operating system
 file, such as: modification date, creation, size in bytes, among others.
 [Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca-
 utils-os) | [Package (PyPI)](https://pypi.org/project/jaanca-utils-os/) |
 [Samples](https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os/
-samples) --- # library installation ```console pip install prettytable==3.10.0
-pip install python-dotenv==1.0.0 pip install jaanca_utils_os[dotenv] --upgrade
-``` --- # environment_parser_loader: Example of use ### Considerations on
-environmental variables - An object must be specified with the variables that
-you want to create. - The attributes of these objects will be loaded with the
-environment variables, according to the name assigned to them. - If the
-attribute is mandatory, it will only be of type str and will contain the name
-of the environment variable to read. - If the environment variable is optional
-or may not exist, the attribute must be of type tuple or list, where the first
-element is the environment variable to read and the second the default value to
-assign. - Example: ```Python class Environment: ENV_VAR_NO_EXIT =
-("VARIABLE","Not Exist") ENV_VAR_IS_MANDATORY = "VARIABLE" ``` ### File with
-environments vars .env ```console ENGINE_POSTGRES_CONN_HOST=psqlt
-ENGINE_POSTGRES_CONN_DB=test ENGINE_POSTGRES_CONN_PASSWORD=es3bv3v3
-ENGINE_POSTGRES_CONN_PORT=5432 ENGINE_POSTGRES_CONN_USER=postgres
-ENGINE_POSTGRES_CONN_SSL=false FLOAT=3.3 LIST=[1,2,3,"4","5"] DICT='{"one":
-"one", "two": 2}' BOOL_TRUE = true BOOL_TRUE_ONE = 1 BOOL_TRUE_TWO = "1"
-BOOL_FALSE_ONE = 0 BOOL_FALSE_TWO = "0" BOOL_FALSE_INCORRECT = "incorrect" ```
-### Example ```Python from jaanca_utils_os import EnvironmentParserLoader,
-FileFolderManagement from prettytable import PrettyTable class Environment:
-HOST = "ENGINE_POSTGRES_CONN_HOST" DB_NAME = "ENGINE_POSTGRES_CONN_DB" PASSWORD
-= "ENGINE_POSTGRES_CONN_PASSWORD" PORT = "ENGINE_POSTGRES_CONN_PORT" USER =
+samples) --- # library installation ```console pip install python-dotenv --
+upgrade pip install jaanca_utils_os[dotenv] --upgrade ``` --- #
+environment_parser_loader: Example of use ### Considerations on environmental
+variables - An object must be specified with the variables that you want to
+create. - The attributes of these objects will be loaded with the environment
+variables, according to the name assigned to them. - If the attribute is
+mandatory, it will only be of type str and will contain the name of the
+environment variable to read. - If the environment variable is optional or may
+not exist, the attribute must be of type tuple or list, where the first element
+is the environment variable to read and the second the default value to assign.
+- Example: ```Python class Environment: ENV_VAR_NO_EXIT = ("VARIABLE","Not
+Exist") ENV_VAR_IS_MANDATORY = "VARIABLE" ``` ### File with environments vars
+.env ```console ENGINE_POSTGRES_CONN_HOST=psqlt ENGINE_POSTGRES_CONN_DB=test
+ENGINE_POSTGRES_CONN_PASSWORD=es3bv3v3 ENGINE_POSTGRES_CONN_PORT=5432
+ENGINE_POSTGRES_CONN_USER=postgres ENGINE_POSTGRES_CONN_SSL=false FLOAT=3.3
+LIST=[1,2,3,"4","5"] DICT='{"one": "one", "two": 2}' BOOL_TRUE = true
+BOOL_TRUE_ONE = 1 BOOL_TRUE_TWO = "1" BOOL_FALSE_ONE = 0 BOOL_FALSE_TWO = "0"
+BOOL_FALSE_INCORRECT = "incorrect" ``` ### Example ```Python from
+jaanca_utils_os import EnvironmentParserLoader, FileFolderManagement from
+prettytable import PrettyTable class Environment: HOST =
+"ENGINE_POSTGRES_CONN_HOST" DB_NAME = "ENGINE_POSTGRES_CONN_DB" PASSWORD =
+"ENGINE_POSTGRES_CONN_PASSWORD" PORT = "ENGINE_POSTGRES_CONN_PORT" USER =
 "ENGINE_POSTGRES_CONN_USER" SSL = "ENGINE_POSTGRES_CONN_SSL" FLOAT = "FLOAT"
 LIST = "LIST" DICT = "DICT" BOOL_TRUE = "BOOL_TRUE" BOOL_TRUE_ONE =
 "BOOL_TRUE_ONE" BOOL_TRUE_TWO = "BOOL_TRUE_TWO" BOOL_FALSE_ONE =
 "BOOL_FALSE_ONE" BOOL_FALSE_TWO = "BOOL_FALSE_TWO" BOOL_FALSE_INCORRECT =
 "BOOL_FALSE_INCORRECT" NO_DATA_TUPLE = ("VARIABLE","Not Exist") NO_DATA_LIST =
 ["VARIABLE","Not Exist"] NO_DATA_BOOL = ["VARIABLE","1"] # Load varibles from
 current folder env_full_path =
 FileFolderManagement.build_full_path_from_current_folder
-(__file__,filename=".env") # Load varibles from current folder and subfolders #
+(__file__,filename=".env") # Load varibles from current folder and subfolders
 env_full_path = FileFolderManagement.build_full_path_from_current_folder
 (__file__,filename=".env",folder_list=["folder2"]) # Load varibles from disk
-path: c:\tmp # env_full_path = FileFolderManagement.build_full_path_to_file("c:
+path: c:\tmp env_full_path = FileFolderManagement.build_full_path_to_file("c:
 ",file_name=".env",folder_list=["tmp"]) settings = EnvironmentParserLoader
-(Environment,env_full_path=env_full_path) def print_attributes(cls): columns =
+(Environment,env_full_path=env_full_path) # Run the script from where the
+default environment variables .env file is located settings =
+EnvironmentParserLoader(Environment) def print_attributes(cls): columns =
 ["Name", "Type", "Value"] myTable = PrettyTable(columns) for attribute_name,
 attribute_value in vars(cls).items(): attribute_type = type(attribute_value)
 myTable.add_row([attribute_name, attribute_type.__name__, attribute_value])
 print(myTable) print_attributes(settings) ``` ### Output | Name | Type | Value
 | |----------------------|-------|--------------------------| | HOST | str |
 psqlt | | DB_NAME | str | test | | PASSWORD | str | es3bv3v3 | | PORT | int |
 5432 | | USER | str | postgres | | SSL | bool | False | | FLOAT | float | 3.3 |
@@ -121,8 +123,8 @@
 will be documented in this file. The format is based on [Keep a Changelog]
 (https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic
 Versioning](https://semver.org/spec/v2.0.0.html). ## Types of changes - Added
 for new features. - Changed for changes in existing functionality. - Deprecated
 for soon-to-be removed features. - Removed for now removed features. - Fixed
 for any bug fixes. - Security in case of vulnerabilities. ## [0.0.1rcX] - 2024-
 05-27 ### Added - First tests using pypi.org in develop environment. ## [0.1.1-
-4] - 2024-05-27 ### Added - Completion of testing and launch into production.
+5] - 2024-05-27 ### Added - Completion of testing and launch into production.
```

### Comparing `jaanca_utils_os-0.1.4/README.md` & `jaanca_utils_os-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,15 @@
 | [Package (PyPI)](https://pypi.org/project/jaanca-utils-os/)
 | [Samples](https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os/samples)
 
 ---
 
 # library installation
 ```console    
-pip install prettytable==3.10.0
-pip install python-dotenv==1.0.0
+pip install python-dotenv --upgrade
 pip install jaanca_utils_os[dotenv] --upgrade
 ```
 
 ---
 # environment_parser_loader: Example of use
 
 ### Considerations on environmental variables
@@ -100,20 +99,22 @@
     NO_DATA_TUPLE = ("VARIABLE","Not Exist")
     NO_DATA_LIST = ["VARIABLE","Not Exist"]
     NO_DATA_BOOL = ["VARIABLE","1"]
 
 # Load varibles from current folder
 env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env")
 # Load varibles from current folder and subfolders
-# env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env",folder_list=["folder2"])
+env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env",folder_list=["folder2"])
 # Load varibles from disk path: c:\tmp
-# env_full_path = FileFolderManagement.build_full_path_to_file("c:",file_name=".env",folder_list=["tmp"])
-
+env_full_path = FileFolderManagement.build_full_path_to_file("c:",file_name=".env",folder_list=["tmp"])
 settings = EnvironmentParserLoader(Environment,env_full_path=env_full_path)
 
+# Run the script from where the default environment variables .env file is located
+settings = EnvironmentParserLoader(Environment)
+
 def print_attributes(cls):
     columns = ["Name", "Type", "Value"]
     myTable = PrettyTable(columns)
     for attribute_name, attribute_value in vars(cls).items():
         attribute_type = type(attribute_value)
         myTable.add_row([attribute_name, attribute_type.__name__, attribute_value])
     print(myTable)        
@@ -233,11 +234,11 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 ## [0.0.1rcX] - 2024-05-27
 ### Added
 - First tests using pypi.org in develop environment.
 
-## [0.1.1-4] - 2024-05-27
+## [0.1.1-5] - 2024-05-27
 ### Added
 - Completion of testing and launch into production.
```

#### html2text {}

```diff
@@ -13,50 +13,52 @@
 a default value is not assigned, a KeyError exception will be returned. *
 **FileFolderManagement**: To write files, use the write_to_disk() method *
 **FileProperties**: Functionalities to read properties of an operating system
 file, such as: modification date, creation, size in bytes, among others.
 [Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca-
 utils-os) | [Package (PyPI)](https://pypi.org/project/jaanca-utils-os/) |
 [Samples](https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os/
-samples) --- # library installation ```console pip install prettytable==3.10.0
-pip install python-dotenv==1.0.0 pip install jaanca_utils_os[dotenv] --upgrade
-``` --- # environment_parser_loader: Example of use ### Considerations on
-environmental variables - An object must be specified with the variables that
-you want to create. - The attributes of these objects will be loaded with the
-environment variables, according to the name assigned to them. - If the
-attribute is mandatory, it will only be of type str and will contain the name
-of the environment variable to read. - If the environment variable is optional
-or may not exist, the attribute must be of type tuple or list, where the first
-element is the environment variable to read and the second the default value to
-assign. - Example: ```Python class Environment: ENV_VAR_NO_EXIT =
-("VARIABLE","Not Exist") ENV_VAR_IS_MANDATORY = "VARIABLE" ``` ### File with
-environments vars .env ```console ENGINE_POSTGRES_CONN_HOST=psqlt
-ENGINE_POSTGRES_CONN_DB=test ENGINE_POSTGRES_CONN_PASSWORD=es3bv3v3
-ENGINE_POSTGRES_CONN_PORT=5432 ENGINE_POSTGRES_CONN_USER=postgres
-ENGINE_POSTGRES_CONN_SSL=false FLOAT=3.3 LIST=[1,2,3,"4","5"] DICT='{"one":
-"one", "two": 2}' BOOL_TRUE = true BOOL_TRUE_ONE = 1 BOOL_TRUE_TWO = "1"
-BOOL_FALSE_ONE = 0 BOOL_FALSE_TWO = "0" BOOL_FALSE_INCORRECT = "incorrect" ```
-### Example ```Python from jaanca_utils_os import EnvironmentParserLoader,
-FileFolderManagement from prettytable import PrettyTable class Environment:
-HOST = "ENGINE_POSTGRES_CONN_HOST" DB_NAME = "ENGINE_POSTGRES_CONN_DB" PASSWORD
-= "ENGINE_POSTGRES_CONN_PASSWORD" PORT = "ENGINE_POSTGRES_CONN_PORT" USER =
+samples) --- # library installation ```console pip install python-dotenv --
+upgrade pip install jaanca_utils_os[dotenv] --upgrade ``` --- #
+environment_parser_loader: Example of use ### Considerations on environmental
+variables - An object must be specified with the variables that you want to
+create. - The attributes of these objects will be loaded with the environment
+variables, according to the name assigned to them. - If the attribute is
+mandatory, it will only be of type str and will contain the name of the
+environment variable to read. - If the environment variable is optional or may
+not exist, the attribute must be of type tuple or list, where the first element
+is the environment variable to read and the second the default value to assign.
+- Example: ```Python class Environment: ENV_VAR_NO_EXIT = ("VARIABLE","Not
+Exist") ENV_VAR_IS_MANDATORY = "VARIABLE" ``` ### File with environments vars
+.env ```console ENGINE_POSTGRES_CONN_HOST=psqlt ENGINE_POSTGRES_CONN_DB=test
+ENGINE_POSTGRES_CONN_PASSWORD=es3bv3v3 ENGINE_POSTGRES_CONN_PORT=5432
+ENGINE_POSTGRES_CONN_USER=postgres ENGINE_POSTGRES_CONN_SSL=false FLOAT=3.3
+LIST=[1,2,3,"4","5"] DICT='{"one": "one", "two": 2}' BOOL_TRUE = true
+BOOL_TRUE_ONE = 1 BOOL_TRUE_TWO = "1" BOOL_FALSE_ONE = 0 BOOL_FALSE_TWO = "0"
+BOOL_FALSE_INCORRECT = "incorrect" ``` ### Example ```Python from
+jaanca_utils_os import EnvironmentParserLoader, FileFolderManagement from
+prettytable import PrettyTable class Environment: HOST =
+"ENGINE_POSTGRES_CONN_HOST" DB_NAME = "ENGINE_POSTGRES_CONN_DB" PASSWORD =
+"ENGINE_POSTGRES_CONN_PASSWORD" PORT = "ENGINE_POSTGRES_CONN_PORT" USER =
 "ENGINE_POSTGRES_CONN_USER" SSL = "ENGINE_POSTGRES_CONN_SSL" FLOAT = "FLOAT"
 LIST = "LIST" DICT = "DICT" BOOL_TRUE = "BOOL_TRUE" BOOL_TRUE_ONE =
 "BOOL_TRUE_ONE" BOOL_TRUE_TWO = "BOOL_TRUE_TWO" BOOL_FALSE_ONE =
 "BOOL_FALSE_ONE" BOOL_FALSE_TWO = "BOOL_FALSE_TWO" BOOL_FALSE_INCORRECT =
 "BOOL_FALSE_INCORRECT" NO_DATA_TUPLE = ("VARIABLE","Not Exist") NO_DATA_LIST =
 ["VARIABLE","Not Exist"] NO_DATA_BOOL = ["VARIABLE","1"] # Load varibles from
 current folder env_full_path =
 FileFolderManagement.build_full_path_from_current_folder
-(__file__,filename=".env") # Load varibles from current folder and subfolders #
+(__file__,filename=".env") # Load varibles from current folder and subfolders
 env_full_path = FileFolderManagement.build_full_path_from_current_folder
 (__file__,filename=".env",folder_list=["folder2"]) # Load varibles from disk
-path: c:\tmp # env_full_path = FileFolderManagement.build_full_path_to_file("c:
+path: c:\tmp env_full_path = FileFolderManagement.build_full_path_to_file("c:
 ",file_name=".env",folder_list=["tmp"]) settings = EnvironmentParserLoader
-(Environment,env_full_path=env_full_path) def print_attributes(cls): columns =
+(Environment,env_full_path=env_full_path) # Run the script from where the
+default environment variables .env file is located settings =
+EnvironmentParserLoader(Environment) def print_attributes(cls): columns =
 ["Name", "Type", "Value"] myTable = PrettyTable(columns) for attribute_name,
 attribute_value in vars(cls).items(): attribute_type = type(attribute_value)
 myTable.add_row([attribute_name, attribute_type.__name__, attribute_value])
 print(myTable) print_attributes(settings) ``` ### Output | Name | Type | Value
 | |----------------------|-------|--------------------------| | HOST | str |
 psqlt | | DB_NAME | str | test | | PASSWORD | str | es3bv3v3 | | PORT | int |
 5432 | | USER | str | postgres | | SSL | bool | False | | FLOAT | float | 3.3 |
@@ -103,8 +105,8 @@
 will be documented in this file. The format is based on [Keep a Changelog]
 (https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic
 Versioning](https://semver.org/spec/v2.0.0.html). ## Types of changes - Added
 for new features. - Changed for changes in existing functionality. - Deprecated
 for soon-to-be removed features. - Removed for now removed features. - Fixed
 for any bug fixes. - Security in case of vulnerabilities. ## [0.0.1rcX] - 2024-
 05-27 ### Added - First tests using pypi.org in develop environment. ## [0.1.1-
-4] - 2024-05-27 ### Added - Completion of testing and launch into production.
+5] - 2024-05-27 ### Added - Completion of testing and launch into production.
```

### Comparing `jaanca_utils_os-0.1.4/jaanca_utils_os/__init__.py` & `jaanca_utils_os-0.1.5/jaanca_utils_os/__init__.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.4/jaanca_utils_os/utils/helpers/environment_parser_loader.py` & `jaanca_utils_os-0.1.5/jaanca_utils_os/utils/helpers/environment_parser_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,23 +83,23 @@
         BOOL_FALSE_TWO = "BOOL_FALSE_TWO"
         BOOL_FALSE_INCORRECT = "BOOL_FALSE_INCORRECT"
         NO_DATA_TUPLE = ("VARIABLE","Not Exist")
         NO_DATA_LIST = ["VARIABLE","Not Exist"]
         NO_DATA_BOOL = ["VARIABLE","1"]
 
     # Load varibles from current folder
-    # env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env")
+    env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env")
     # Load varibles from current folder and subfolders
-    # env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env",folder_list=["folder2"])
+    env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env",folder_list=["folder2"])
     # Load varibles from disk path: c:\tmp
-    # env_full_path = FileFolderManagement.build_full_path_to_file("c:",file_name=".env",folder_list=["tmp"])
+    env_full_path = FileFolderManagement.build_full_path_to_file("c:",file_name=".env",folder_list=["tmp"])
+    settings = EnvironmentParserLoader(Environment,env_full_path=env_full_path)
 
     # Run the script from where the default environment variables .env file is located
     settings = EnvironmentParserLoader(Environment)
-    # settings = EnvironmentParserLoader(Environment,env_full_path=env_full_path)
 
     def print_attributes(cls):
         columns = ["Name", "Type", "Value"]
         myTable = PrettyTable(columns)
         for attribute_name, attribute_value in vars(cls).items():
             attribute_type = type(attribute_value)
             myTable.add_row([attribute_name, attribute_type.__name__, attribute_value])
```

### Comparing `jaanca_utils_os-0.1.4/jaanca_utils_os/utils/helpers/file_folder_management.py` & `jaanca_utils_os-0.1.5/jaanca_utils_os/utils/helpers/file_folder_management.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.4/jaanca_utils_os/utils/helpers/file_properties.py` & `jaanca_utils_os-0.1.5/jaanca_utils_os/utils/helpers/file_properties.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.4/jaanca_utils_os/utils/helpers/parse_bool.py` & `jaanca_utils_os-0.1.5/jaanca_utils_os/utils/helpers/parse_bool.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.4/jaanca_utils_os/utils/helpers/parse_types.py` & `jaanca_utils_os-0.1.5/jaanca_utils_os/utils/helpers/parse_types.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.4/jaanca_utils_os.egg-info/PKG-INFO` & `jaanca_utils_os-0.1.5/jaanca_utils_os.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-utils-os
-Version: 0.1.4
+Version: 0.1.5
 Summary: A tool library created by jaanca with operating system help functions such as reading environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: datetime,utc
 Classifier: Development Status :: 4 - Beta
@@ -63,16 +63,15 @@
 | [Package (PyPI)](https://pypi.org/project/jaanca-utils-os/)
 | [Samples](https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os/samples)
 
 ---
 
 # library installation
 ```console    
-pip install prettytable==3.10.0
-pip install python-dotenv==1.0.0
+pip install python-dotenv --upgrade
 pip install jaanca_utils_os[dotenv] --upgrade
 ```
 
 ---
 # environment_parser_loader: Example of use
 
 ### Considerations on environmental variables
@@ -131,20 +130,22 @@
     NO_DATA_TUPLE = ("VARIABLE","Not Exist")
     NO_DATA_LIST = ["VARIABLE","Not Exist"]
     NO_DATA_BOOL = ["VARIABLE","1"]
 
 # Load varibles from current folder
 env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env")
 # Load varibles from current folder and subfolders
-# env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env",folder_list=["folder2"])
+env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env",folder_list=["folder2"])
 # Load varibles from disk path: c:\tmp
-# env_full_path = FileFolderManagement.build_full_path_to_file("c:",file_name=".env",folder_list=["tmp"])
-
+env_full_path = FileFolderManagement.build_full_path_to_file("c:",file_name=".env",folder_list=["tmp"])
 settings = EnvironmentParserLoader(Environment,env_full_path=env_full_path)
 
+# Run the script from where the default environment variables .env file is located
+settings = EnvironmentParserLoader(Environment)
+
 def print_attributes(cls):
     columns = ["Name", "Type", "Value"]
     myTable = PrettyTable(columns)
     for attribute_name, attribute_value in vars(cls).items():
         attribute_type = type(attribute_value)
         myTable.add_row([attribute_name, attribute_type.__name__, attribute_value])
     print(myTable)        
@@ -264,11 +265,11 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 ## [0.0.1rcX] - 2024-05-27
 ### Added
 - First tests using pypi.org in develop environment.
 
-## [0.1.1-4] - 2024-05-27
+## [0.1.1-5] - 2024-05-27
 ### Added
 - Completion of testing and launch into production.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.4 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.5 Summary: A tool
 library created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com
 License: MIT License Keywords: datetime,utc Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
@@ -31,50 +31,52 @@
 a default value is not assigned, a KeyError exception will be returned. *
 **FileFolderManagement**: To write files, use the write_to_disk() method *
 **FileProperties**: Functionalities to read properties of an operating system
 file, such as: modification date, creation, size in bytes, among others.
 [Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca-
 utils-os) | [Package (PyPI)](https://pypi.org/project/jaanca-utils-os/) |
 [Samples](https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os/
-samples) --- # library installation ```console pip install prettytable==3.10.0
-pip install python-dotenv==1.0.0 pip install jaanca_utils_os[dotenv] --upgrade
-``` --- # environment_parser_loader: Example of use ### Considerations on
-environmental variables - An object must be specified with the variables that
-you want to create. - The attributes of these objects will be loaded with the
-environment variables, according to the name assigned to them. - If the
-attribute is mandatory, it will only be of type str and will contain the name
-of the environment variable to read. - If the environment variable is optional
-or may not exist, the attribute must be of type tuple or list, where the first
-element is the environment variable to read and the second the default value to
-assign. - Example: ```Python class Environment: ENV_VAR_NO_EXIT =
-("VARIABLE","Not Exist") ENV_VAR_IS_MANDATORY = "VARIABLE" ``` ### File with
-environments vars .env ```console ENGINE_POSTGRES_CONN_HOST=psqlt
-ENGINE_POSTGRES_CONN_DB=test ENGINE_POSTGRES_CONN_PASSWORD=es3bv3v3
-ENGINE_POSTGRES_CONN_PORT=5432 ENGINE_POSTGRES_CONN_USER=postgres
-ENGINE_POSTGRES_CONN_SSL=false FLOAT=3.3 LIST=[1,2,3,"4","5"] DICT='{"one":
-"one", "two": 2}' BOOL_TRUE = true BOOL_TRUE_ONE = 1 BOOL_TRUE_TWO = "1"
-BOOL_FALSE_ONE = 0 BOOL_FALSE_TWO = "0" BOOL_FALSE_INCORRECT = "incorrect" ```
-### Example ```Python from jaanca_utils_os import EnvironmentParserLoader,
-FileFolderManagement from prettytable import PrettyTable class Environment:
-HOST = "ENGINE_POSTGRES_CONN_HOST" DB_NAME = "ENGINE_POSTGRES_CONN_DB" PASSWORD
-= "ENGINE_POSTGRES_CONN_PASSWORD" PORT = "ENGINE_POSTGRES_CONN_PORT" USER =
+samples) --- # library installation ```console pip install python-dotenv --
+upgrade pip install jaanca_utils_os[dotenv] --upgrade ``` --- #
+environment_parser_loader: Example of use ### Considerations on environmental
+variables - An object must be specified with the variables that you want to
+create. - The attributes of these objects will be loaded with the environment
+variables, according to the name assigned to them. - If the attribute is
+mandatory, it will only be of type str and will contain the name of the
+environment variable to read. - If the environment variable is optional or may
+not exist, the attribute must be of type tuple or list, where the first element
+is the environment variable to read and the second the default value to assign.
+- Example: ```Python class Environment: ENV_VAR_NO_EXIT = ("VARIABLE","Not
+Exist") ENV_VAR_IS_MANDATORY = "VARIABLE" ``` ### File with environments vars
+.env ```console ENGINE_POSTGRES_CONN_HOST=psqlt ENGINE_POSTGRES_CONN_DB=test
+ENGINE_POSTGRES_CONN_PASSWORD=es3bv3v3 ENGINE_POSTGRES_CONN_PORT=5432
+ENGINE_POSTGRES_CONN_USER=postgres ENGINE_POSTGRES_CONN_SSL=false FLOAT=3.3
+LIST=[1,2,3,"4","5"] DICT='{"one": "one", "two": 2}' BOOL_TRUE = true
+BOOL_TRUE_ONE = 1 BOOL_TRUE_TWO = "1" BOOL_FALSE_ONE = 0 BOOL_FALSE_TWO = "0"
+BOOL_FALSE_INCORRECT = "incorrect" ``` ### Example ```Python from
+jaanca_utils_os import EnvironmentParserLoader, FileFolderManagement from
+prettytable import PrettyTable class Environment: HOST =
+"ENGINE_POSTGRES_CONN_HOST" DB_NAME = "ENGINE_POSTGRES_CONN_DB" PASSWORD =
+"ENGINE_POSTGRES_CONN_PASSWORD" PORT = "ENGINE_POSTGRES_CONN_PORT" USER =
 "ENGINE_POSTGRES_CONN_USER" SSL = "ENGINE_POSTGRES_CONN_SSL" FLOAT = "FLOAT"
 LIST = "LIST" DICT = "DICT" BOOL_TRUE = "BOOL_TRUE" BOOL_TRUE_ONE =
 "BOOL_TRUE_ONE" BOOL_TRUE_TWO = "BOOL_TRUE_TWO" BOOL_FALSE_ONE =
 "BOOL_FALSE_ONE" BOOL_FALSE_TWO = "BOOL_FALSE_TWO" BOOL_FALSE_INCORRECT =
 "BOOL_FALSE_INCORRECT" NO_DATA_TUPLE = ("VARIABLE","Not Exist") NO_DATA_LIST =
 ["VARIABLE","Not Exist"] NO_DATA_BOOL = ["VARIABLE","1"] # Load varibles from
 current folder env_full_path =
 FileFolderManagement.build_full_path_from_current_folder
-(__file__,filename=".env") # Load varibles from current folder and subfolders #
+(__file__,filename=".env") # Load varibles from current folder and subfolders
 env_full_path = FileFolderManagement.build_full_path_from_current_folder
 (__file__,filename=".env",folder_list=["folder2"]) # Load varibles from disk
-path: c:\tmp # env_full_path = FileFolderManagement.build_full_path_to_file("c:
+path: c:\tmp env_full_path = FileFolderManagement.build_full_path_to_file("c:
 ",file_name=".env",folder_list=["tmp"]) settings = EnvironmentParserLoader
-(Environment,env_full_path=env_full_path) def print_attributes(cls): columns =
+(Environment,env_full_path=env_full_path) # Run the script from where the
+default environment variables .env file is located settings =
+EnvironmentParserLoader(Environment) def print_attributes(cls): columns =
 ["Name", "Type", "Value"] myTable = PrettyTable(columns) for attribute_name,
 attribute_value in vars(cls).items(): attribute_type = type(attribute_value)
 myTable.add_row([attribute_name, attribute_type.__name__, attribute_value])
 print(myTable) print_attributes(settings) ``` ### Output | Name | Type | Value
 | |----------------------|-------|--------------------------| | HOST | str |
 psqlt | | DB_NAME | str | test | | PASSWORD | str | es3bv3v3 | | PORT | int |
 5432 | | USER | str | postgres | | SSL | bool | False | | FLOAT | float | 3.3 |
@@ -121,8 +123,8 @@
 will be documented in this file. The format is based on [Keep a Changelog]
 (https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic
 Versioning](https://semver.org/spec/v2.0.0.html). ## Types of changes - Added
 for new features. - Changed for changes in existing functionality. - Deprecated
 for soon-to-be removed features. - Removed for now removed features. - Fixed
 for any bug fixes. - Security in case of vulnerabilities. ## [0.0.1rcX] - 2024-
 05-27 ### Added - First tests using pypi.org in develop environment. ## [0.1.1-
-4] - 2024-05-27 ### Added - Completion of testing and launch into production.
+5] - 2024-05-27 ### Added - Completion of testing and launch into production.
```

### Comparing `jaanca_utils_os-0.1.4/jaanca_utils_os.egg-info/SOURCES.txt` & `jaanca_utils_os-0.1.5/jaanca_utils_os.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.4/setup.py` & `jaanca_utils_os-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca-utils-os"
-VERSION = "0.1.4"
+VERSION = "0.1.5"
 
 install_requires = [""]
 extras_require = {
     "dotenv": "python-dotenv>=1.0.0"
 }
 
 setup(
```

