# Comparing `tmp/jaanca_utils_os-0.1.5.tar.gz` & `tmp/jaanca_utils_os-0.1.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca_utils_os-0.1.5.tar", last modified: Tue May 28 00:03:42 2024, max compression
+gzip compressed data, was "jaanca_utils_os-0.1.6rc1.tar", last modified: Tue May 28 00:11:08 2024, max compression
```

## Comparing `jaanca_utils_os-0.1.5.tar` & `jaanca_utils_os-0.1.6rc1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 00:03:42.719653 jaanca_utils_os-0.1.5/
--rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0    10991 2024-05-28 00:03:42.718677 jaanca_utils_os-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     9584 2024-05-28 00:03:02.000000 jaanca_utils_os-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 00:03:42.692786 jaanca_utils_os-0.1.5/jaanca_utils_os/
--rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.1.5/jaanca_utils_os/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 00:03:42.703728 jaanca_utils_os-0.1.5/jaanca_utils_os/utils/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.5/jaanca_utils_os/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 00:03:42.714622 jaanca_utils_os-0.1.5/jaanca_utils_os/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.5/jaanca_utils_os/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     5663 2024-05-28 00:03:33.000000 jaanca_utils_os-0.1.5/jaanca_utils_os/utils/helpers/environment_parser_loader.py
--rw-rw-rw-   0        0        0     6835 2024-05-27 22:01:52.000000 jaanca_utils_os-0.1.5/jaanca_utils_os/utils/helpers/file_folder_management.py
--rw-rw-rw-   0        0        0     3289 2024-05-27 22:09:16.000000 jaanca_utils_os-0.1.5/jaanca_utils_os/utils/helpers/file_properties.py
--rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.1.5/jaanca_utils_os/utils/helpers/parse_bool.py
--rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.1.5/jaanca_utils_os/utils/helpers/parse_types.py
-drwxrwxrwx   0        0        0        0 2024-05-28 00:03:42.716636 jaanca_utils_os-0.1.5/jaanca_utils_os.egg-info/
--rw-rw-rw-   0        0        0    10991 2024-05-28 00:03:42.000000 jaanca_utils_os-0.1.5/jaanca_utils_os.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      591 2024-05-28 00:03:42.000000 jaanca_utils_os-0.1.5/jaanca_utils_os.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 00:03:42.000000 jaanca_utils_os-0.1.5/jaanca_utils_os.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-28 00:03:42.000000 jaanca_utils_os-0.1.5/jaanca_utils_os.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-28 00:03:42.000000 jaanca_utils_os-0.1.5/jaanca_utils_os.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 00:03:42.720654 jaanca_utils_os-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1756 2024-05-28 00:03:10.000000 jaanca_utils_os-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 00:11:08.163180 jaanca_utils_os-0.1.6rc1/
+-rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.6rc1/LICENSE.txt
+-rw-rw-rw-   0        0        0    11152 2024-05-28 00:11:08.163180 jaanca_utils_os-0.1.6rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     9742 2024-05-28 00:10:54.000000 jaanca_utils_os-0.1.6rc1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 00:11:08.135240 jaanca_utils_os-0.1.6rc1/jaanca_utils_os/
+-rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.1.6rc1/jaanca_utils_os/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 00:11:08.147165 jaanca_utils_os-0.1.6rc1/jaanca_utils_os/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.6rc1/jaanca_utils_os/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 00:11:08.159184 jaanca_utils_os-0.1.6rc1/jaanca_utils_os/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.6rc1/jaanca_utils_os/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     5849 2024-05-28 00:10:39.000000 jaanca_utils_os-0.1.6rc1/jaanca_utils_os/utils/helpers/environment_parser_loader.py
+-rw-rw-rw-   0        0        0     6835 2024-05-27 22:01:52.000000 jaanca_utils_os-0.1.6rc1/jaanca_utils_os/utils/helpers/file_folder_management.py
+-rw-rw-rw-   0        0        0     3289 2024-05-27 22:09:16.000000 jaanca_utils_os-0.1.6rc1/jaanca_utils_os/utils/helpers/file_properties.py
+-rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.1.6rc1/jaanca_utils_os/utils/helpers/parse_bool.py
+-rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.1.6rc1/jaanca_utils_os/utils/helpers/parse_types.py
+drwxrwxrwx   0        0        0        0 2024-05-28 00:11:08.161181 jaanca_utils_os-0.1.6rc1/jaanca_utils_os.egg-info/
+-rw-rw-rw-   0        0        0    11152 2024-05-28 00:11:08.000000 jaanca_utils_os-0.1.6rc1/jaanca_utils_os.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      591 2024-05-28 00:11:08.000000 jaanca_utils_os-0.1.6rc1/jaanca_utils_os.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 00:11:08.000000 jaanca_utils_os-0.1.6rc1/jaanca_utils_os.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-28 00:11:08.000000 jaanca_utils_os-0.1.6rc1/jaanca_utils_os.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-28 00:11:08.000000 jaanca_utils_os-0.1.6rc1/jaanca_utils_os.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 00:11:08.165180 jaanca_utils_os-0.1.6rc1/setup.cfg
+-rw-rw-rw-   0        0        0     1759 2024-05-28 00:11:00.000000 jaanca_utils_os-0.1.6rc1/setup.py
```

### Comparing `jaanca_utils_os-0.1.5/LICENSE.txt` & `jaanca_utils_os-0.1.6rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.5/PKG-INFO` & `jaanca_utils_os-0.1.6rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-utils-os
-Version: 0.1.5
+Version: 0.1.6rc1
 Summary: A tool library created by jaanca with operating system help functions such as reading environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: datetime,utc
 Classifier: Development Status :: 4 - Beta
@@ -127,24 +127,33 @@
     BOOL_FALSE_ONE = "BOOL_FALSE_ONE"
     BOOL_FALSE_TWO = "BOOL_FALSE_TWO"
     BOOL_FALSE_INCORRECT = "BOOL_FALSE_INCORRECT"
     NO_DATA_TUPLE = ("VARIABLE","Not Exist")
     NO_DATA_LIST = ["VARIABLE","Not Exist"]
     NO_DATA_BOOL = ["VARIABLE","1"]
 
-# Load varibles from current folder
-env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env")
+############
+# select the location of the file to read
+############
+
+############
+# Option 1
+# Run the script from where the default environment variables .env file is located
+# settings:Environment = EnvironmentParserLoader(Environment)
+
+############
+# Other Options
 # Load varibles from current folder and subfolders
 env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env",folder_list=["folder2"])
 # Load varibles from disk path: c:\tmp
 env_full_path = FileFolderManagement.build_full_path_to_file("c:",file_name=".env",folder_list=["tmp"])
-settings = EnvironmentParserLoader(Environment,env_full_path=env_full_path)
+# Load varibles from current folder
+env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env")
 
-# Run the script from where the default environment variables .env file is located
-settings = EnvironmentParserLoader(Environment)
+settings:Environment = EnvironmentParserLoader(Environment,env_full_path=env_full_path)
 
 def print_attributes(cls):
     columns = ["Name", "Type", "Value"]
     myTable = PrettyTable(columns)
     for attribute_name, attribute_value in vars(cls).items():
         attribute_type = type(attribute_value)
         myTable.add_row([attribute_name, attribute_type.__name__, attribute_value])
@@ -265,11 +274,11 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 ## [0.0.1rcX] - 2024-05-27
 ### Added
 - First tests using pypi.org in develop environment.
 
-## [0.1.1-5] - 2024-05-27
+## [0.1.1-6] - 2024-05-27
 ### Added
 - Completion of testing and launch into production.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.5 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.6rc1 Summary: A tool
 library created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com
 License: MIT License Keywords: datetime,utc Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
@@ -58,25 +58,26 @@
 "ENGINE_POSTGRES_CONN_HOST" DB_NAME = "ENGINE_POSTGRES_CONN_DB" PASSWORD =
 "ENGINE_POSTGRES_CONN_PASSWORD" PORT = "ENGINE_POSTGRES_CONN_PORT" USER =
 "ENGINE_POSTGRES_CONN_USER" SSL = "ENGINE_POSTGRES_CONN_SSL" FLOAT = "FLOAT"
 LIST = "LIST" DICT = "DICT" BOOL_TRUE = "BOOL_TRUE" BOOL_TRUE_ONE =
 "BOOL_TRUE_ONE" BOOL_TRUE_TWO = "BOOL_TRUE_TWO" BOOL_FALSE_ONE =
 "BOOL_FALSE_ONE" BOOL_FALSE_TWO = "BOOL_FALSE_TWO" BOOL_FALSE_INCORRECT =
 "BOOL_FALSE_INCORRECT" NO_DATA_TUPLE = ("VARIABLE","Not Exist") NO_DATA_LIST =
-["VARIABLE","Not Exist"] NO_DATA_BOOL = ["VARIABLE","1"] # Load varibles from
-current folder env_full_path =
-FileFolderManagement.build_full_path_from_current_folder
-(__file__,filename=".env") # Load varibles from current folder and subfolders
-env_full_path = FileFolderManagement.build_full_path_from_current_folder
+["VARIABLE","Not Exist"] NO_DATA_BOOL = ["VARIABLE","1"] ############ # select
+the location of the file to read ############ ############ # Option 1 # Run the
+script from where the default environment variables .env file is located #
+settings:Environment = EnvironmentParserLoader(Environment) ############ #
+Other Options # Load varibles from current folder and subfolders env_full_path
+= FileFolderManagement.build_full_path_from_current_folder
 (__file__,filename=".env",folder_list=["folder2"]) # Load varibles from disk
 path: c:\tmp env_full_path = FileFolderManagement.build_full_path_to_file("c:
-",file_name=".env",folder_list=["tmp"]) settings = EnvironmentParserLoader
-(Environment,env_full_path=env_full_path) # Run the script from where the
-default environment variables .env file is located settings =
-EnvironmentParserLoader(Environment) def print_attributes(cls): columns =
+",file_name=".env",folder_list=["tmp"]) # Load varibles from current folder
+env_full_path = FileFolderManagement.build_full_path_from_current_folder
+(__file__,filename=".env") settings:Environment = EnvironmentParserLoader
+(Environment,env_full_path=env_full_path) def print_attributes(cls): columns =
 ["Name", "Type", "Value"] myTable = PrettyTable(columns) for attribute_name,
 attribute_value in vars(cls).items(): attribute_type = type(attribute_value)
 myTable.add_row([attribute_name, attribute_type.__name__, attribute_value])
 print(myTable) print_attributes(settings) ``` ### Output | Name | Type | Value
 | |----------------------|-------|--------------------------| | HOST | str |
 psqlt | | DB_NAME | str | test | | PASSWORD | str | es3bv3v3 | | PORT | int |
 5432 | | USER | str | postgres | | SSL | bool | False | | FLOAT | float | 3.3 |
@@ -123,8 +124,8 @@
 will be documented in this file. The format is based on [Keep a Changelog]
 (https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic
 Versioning](https://semver.org/spec/v2.0.0.html). ## Types of changes - Added
 for new features. - Changed for changes in existing functionality. - Deprecated
 for soon-to-be removed features. - Removed for now removed features. - Fixed
 for any bug fixes. - Security in case of vulnerabilities. ## [0.0.1rcX] - 2024-
 05-27 ### Added - First tests using pypi.org in develop environment. ## [0.1.1-
-5] - 2024-05-27 ### Added - Completion of testing and launch into production.
+6] - 2024-05-27 ### Added - Completion of testing and launch into production.
```

### Comparing `jaanca_utils_os-0.1.5/README.md` & `jaanca_utils_os-0.1.6rc1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -96,24 +96,33 @@
     BOOL_FALSE_ONE = "BOOL_FALSE_ONE"
     BOOL_FALSE_TWO = "BOOL_FALSE_TWO"
     BOOL_FALSE_INCORRECT = "BOOL_FALSE_INCORRECT"
     NO_DATA_TUPLE = ("VARIABLE","Not Exist")
     NO_DATA_LIST = ["VARIABLE","Not Exist"]
     NO_DATA_BOOL = ["VARIABLE","1"]
 
-# Load varibles from current folder
-env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env")
+############
+# select the location of the file to read
+############
+
+############
+# Option 1
+# Run the script from where the default environment variables .env file is located
+# settings:Environment = EnvironmentParserLoader(Environment)
+
+############
+# Other Options
 # Load varibles from current folder and subfolders
 env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env",folder_list=["folder2"])
 # Load varibles from disk path: c:\tmp
 env_full_path = FileFolderManagement.build_full_path_to_file("c:",file_name=".env",folder_list=["tmp"])
-settings = EnvironmentParserLoader(Environment,env_full_path=env_full_path)
+# Load varibles from current folder
+env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env")
 
-# Run the script from where the default environment variables .env file is located
-settings = EnvironmentParserLoader(Environment)
+settings:Environment = EnvironmentParserLoader(Environment,env_full_path=env_full_path)
 
 def print_attributes(cls):
     columns = ["Name", "Type", "Value"]
     myTable = PrettyTable(columns)
     for attribute_name, attribute_value in vars(cls).items():
         attribute_type = type(attribute_value)
         myTable.add_row([attribute_name, attribute_type.__name__, attribute_value])
@@ -234,11 +243,11 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 ## [0.0.1rcX] - 2024-05-27
 ### Added
 - First tests using pypi.org in develop environment.
 
-## [0.1.1-5] - 2024-05-27
+## [0.1.1-6] - 2024-05-27
 ### Added
 - Completion of testing and launch into production.
```

#### html2text {}

```diff
@@ -40,25 +40,26 @@
 "ENGINE_POSTGRES_CONN_HOST" DB_NAME = "ENGINE_POSTGRES_CONN_DB" PASSWORD =
 "ENGINE_POSTGRES_CONN_PASSWORD" PORT = "ENGINE_POSTGRES_CONN_PORT" USER =
 "ENGINE_POSTGRES_CONN_USER" SSL = "ENGINE_POSTGRES_CONN_SSL" FLOAT = "FLOAT"
 LIST = "LIST" DICT = "DICT" BOOL_TRUE = "BOOL_TRUE" BOOL_TRUE_ONE =
 "BOOL_TRUE_ONE" BOOL_TRUE_TWO = "BOOL_TRUE_TWO" BOOL_FALSE_ONE =
 "BOOL_FALSE_ONE" BOOL_FALSE_TWO = "BOOL_FALSE_TWO" BOOL_FALSE_INCORRECT =
 "BOOL_FALSE_INCORRECT" NO_DATA_TUPLE = ("VARIABLE","Not Exist") NO_DATA_LIST =
-["VARIABLE","Not Exist"] NO_DATA_BOOL = ["VARIABLE","1"] # Load varibles from
-current folder env_full_path =
-FileFolderManagement.build_full_path_from_current_folder
-(__file__,filename=".env") # Load varibles from current folder and subfolders
-env_full_path = FileFolderManagement.build_full_path_from_current_folder
+["VARIABLE","Not Exist"] NO_DATA_BOOL = ["VARIABLE","1"] ############ # select
+the location of the file to read ############ ############ # Option 1 # Run the
+script from where the default environment variables .env file is located #
+settings:Environment = EnvironmentParserLoader(Environment) ############ #
+Other Options # Load varibles from current folder and subfolders env_full_path
+= FileFolderManagement.build_full_path_from_current_folder
 (__file__,filename=".env",folder_list=["folder2"]) # Load varibles from disk
 path: c:\tmp env_full_path = FileFolderManagement.build_full_path_to_file("c:
-",file_name=".env",folder_list=["tmp"]) settings = EnvironmentParserLoader
-(Environment,env_full_path=env_full_path) # Run the script from where the
-default environment variables .env file is located settings =
-EnvironmentParserLoader(Environment) def print_attributes(cls): columns =
+",file_name=".env",folder_list=["tmp"]) # Load varibles from current folder
+env_full_path = FileFolderManagement.build_full_path_from_current_folder
+(__file__,filename=".env") settings:Environment = EnvironmentParserLoader
+(Environment,env_full_path=env_full_path) def print_attributes(cls): columns =
 ["Name", "Type", "Value"] myTable = PrettyTable(columns) for attribute_name,
 attribute_value in vars(cls).items(): attribute_type = type(attribute_value)
 myTable.add_row([attribute_name, attribute_type.__name__, attribute_value])
 print(myTable) print_attributes(settings) ``` ### Output | Name | Type | Value
 | |----------------------|-------|--------------------------| | HOST | str |
 psqlt | | DB_NAME | str | test | | PASSWORD | str | es3bv3v3 | | PORT | int |
 5432 | | USER | str | postgres | | SSL | bool | False | | FLOAT | float | 3.3 |
@@ -105,8 +106,8 @@
 will be documented in this file. The format is based on [Keep a Changelog]
 (https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic
 Versioning](https://semver.org/spec/v2.0.0.html). ## Types of changes - Added
 for new features. - Changed for changes in existing functionality. - Deprecated
 for soon-to-be removed features. - Removed for now removed features. - Fixed
 for any bug fixes. - Security in case of vulnerabilities. ## [0.0.1rcX] - 2024-
 05-27 ### Added - First tests using pypi.org in develop environment. ## [0.1.1-
-5] - 2024-05-27 ### Added - Completion of testing and launch into production.
+6] - 2024-05-27 ### Added - Completion of testing and launch into production.
```

### Comparing `jaanca_utils_os-0.1.5/jaanca_utils_os/__init__.py` & `jaanca_utils_os-0.1.6rc1/jaanca_utils_os/__init__.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.5/jaanca_utils_os/utils/helpers/environment_parser_loader.py` & `jaanca_utils_os-0.1.6rc1/jaanca_utils_os/utils/helpers/environment_parser_loader.py`

 * *Files 13% similar despite different names*

```diff
@@ -82,24 +82,33 @@
         BOOL_FALSE_ONE = "BOOL_FALSE_ONE"
         BOOL_FALSE_TWO = "BOOL_FALSE_TWO"
         BOOL_FALSE_INCORRECT = "BOOL_FALSE_INCORRECT"
         NO_DATA_TUPLE = ("VARIABLE","Not Exist")
         NO_DATA_LIST = ["VARIABLE","Not Exist"]
         NO_DATA_BOOL = ["VARIABLE","1"]
 
-    # Load varibles from current folder
-    env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env")
+    ############
+    # select the location of the file to read
+    ############
+
+    ############
+    # Option 1
+    # Run the script from where the default environment variables .env file is located
+    # settings:Environment = EnvironmentParserLoader(Environment)
+
+    ############
+    # Other Options
     # Load varibles from current folder and subfolders
     env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env",folder_list=["folder2"])
     # Load varibles from disk path: c:\tmp
     env_full_path = FileFolderManagement.build_full_path_to_file("c:",file_name=".env",folder_list=["tmp"])
-    settings = EnvironmentParserLoader(Environment,env_full_path=env_full_path)
+    # Load varibles from current folder
+    env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env")
 
-    # Run the script from where the default environment variables .env file is located
-    settings = EnvironmentParserLoader(Environment)
+    settings:Environment = EnvironmentParserLoader(Environment,env_full_path=env_full_path)
 
     def print_attributes(cls):
         columns = ["Name", "Type", "Value"]
         myTable = PrettyTable(columns)
         for attribute_name, attribute_value in vars(cls).items():
             attribute_type = type(attribute_value)
             myTable.add_row([attribute_name, attribute_type.__name__, attribute_value])
```

### Comparing `jaanca_utils_os-0.1.5/jaanca_utils_os/utils/helpers/file_folder_management.py` & `jaanca_utils_os-0.1.6rc1/jaanca_utils_os/utils/helpers/file_folder_management.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.5/jaanca_utils_os/utils/helpers/file_properties.py` & `jaanca_utils_os-0.1.6rc1/jaanca_utils_os/utils/helpers/file_properties.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.5/jaanca_utils_os/utils/helpers/parse_bool.py` & `jaanca_utils_os-0.1.6rc1/jaanca_utils_os/utils/helpers/parse_bool.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.5/jaanca_utils_os/utils/helpers/parse_types.py` & `jaanca_utils_os-0.1.6rc1/jaanca_utils_os/utils/helpers/parse_types.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.5/jaanca_utils_os.egg-info/PKG-INFO` & `jaanca_utils_os-0.1.6rc1/jaanca_utils_os.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-utils-os
-Version: 0.1.5
+Version: 0.1.6rc1
 Summary: A tool library created by jaanca with operating system help functions such as reading environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: datetime,utc
 Classifier: Development Status :: 4 - Beta
@@ -127,24 +127,33 @@
     BOOL_FALSE_ONE = "BOOL_FALSE_ONE"
     BOOL_FALSE_TWO = "BOOL_FALSE_TWO"
     BOOL_FALSE_INCORRECT = "BOOL_FALSE_INCORRECT"
     NO_DATA_TUPLE = ("VARIABLE","Not Exist")
     NO_DATA_LIST = ["VARIABLE","Not Exist"]
     NO_DATA_BOOL = ["VARIABLE","1"]
 
-# Load varibles from current folder
-env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env")
+############
+# select the location of the file to read
+############
+
+############
+# Option 1
+# Run the script from where the default environment variables .env file is located
+# settings:Environment = EnvironmentParserLoader(Environment)
+
+############
+# Other Options
 # Load varibles from current folder and subfolders
 env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env",folder_list=["folder2"])
 # Load varibles from disk path: c:\tmp
 env_full_path = FileFolderManagement.build_full_path_to_file("c:",file_name=".env",folder_list=["tmp"])
-settings = EnvironmentParserLoader(Environment,env_full_path=env_full_path)
+# Load varibles from current folder
+env_full_path = FileFolderManagement.build_full_path_from_current_folder(__file__,filename=".env")
 
-# Run the script from where the default environment variables .env file is located
-settings = EnvironmentParserLoader(Environment)
+settings:Environment = EnvironmentParserLoader(Environment,env_full_path=env_full_path)
 
 def print_attributes(cls):
     columns = ["Name", "Type", "Value"]
     myTable = PrettyTable(columns)
     for attribute_name, attribute_value in vars(cls).items():
         attribute_type = type(attribute_value)
         myTable.add_row([attribute_name, attribute_type.__name__, attribute_value])
@@ -265,11 +274,11 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 ## [0.0.1rcX] - 2024-05-27
 ### Added
 - First tests using pypi.org in develop environment.
 
-## [0.1.1-5] - 2024-05-27
+## [0.1.1-6] - 2024-05-27
 ### Added
 - Completion of testing and launch into production.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.5 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.6rc1 Summary: A tool
 library created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com
 License: MIT License Keywords: datetime,utc Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
@@ -58,25 +58,26 @@
 "ENGINE_POSTGRES_CONN_HOST" DB_NAME = "ENGINE_POSTGRES_CONN_DB" PASSWORD =
 "ENGINE_POSTGRES_CONN_PASSWORD" PORT = "ENGINE_POSTGRES_CONN_PORT" USER =
 "ENGINE_POSTGRES_CONN_USER" SSL = "ENGINE_POSTGRES_CONN_SSL" FLOAT = "FLOAT"
 LIST = "LIST" DICT = "DICT" BOOL_TRUE = "BOOL_TRUE" BOOL_TRUE_ONE =
 "BOOL_TRUE_ONE" BOOL_TRUE_TWO = "BOOL_TRUE_TWO" BOOL_FALSE_ONE =
 "BOOL_FALSE_ONE" BOOL_FALSE_TWO = "BOOL_FALSE_TWO" BOOL_FALSE_INCORRECT =
 "BOOL_FALSE_INCORRECT" NO_DATA_TUPLE = ("VARIABLE","Not Exist") NO_DATA_LIST =
-["VARIABLE","Not Exist"] NO_DATA_BOOL = ["VARIABLE","1"] # Load varibles from
-current folder env_full_path =
-FileFolderManagement.build_full_path_from_current_folder
-(__file__,filename=".env") # Load varibles from current folder and subfolders
-env_full_path = FileFolderManagement.build_full_path_from_current_folder
+["VARIABLE","Not Exist"] NO_DATA_BOOL = ["VARIABLE","1"] ############ # select
+the location of the file to read ############ ############ # Option 1 # Run the
+script from where the default environment variables .env file is located #
+settings:Environment = EnvironmentParserLoader(Environment) ############ #
+Other Options # Load varibles from current folder and subfolders env_full_path
+= FileFolderManagement.build_full_path_from_current_folder
 (__file__,filename=".env",folder_list=["folder2"]) # Load varibles from disk
 path: c:\tmp env_full_path = FileFolderManagement.build_full_path_to_file("c:
-",file_name=".env",folder_list=["tmp"]) settings = EnvironmentParserLoader
-(Environment,env_full_path=env_full_path) # Run the script from where the
-default environment variables .env file is located settings =
-EnvironmentParserLoader(Environment) def print_attributes(cls): columns =
+",file_name=".env",folder_list=["tmp"]) # Load varibles from current folder
+env_full_path = FileFolderManagement.build_full_path_from_current_folder
+(__file__,filename=".env") settings:Environment = EnvironmentParserLoader
+(Environment,env_full_path=env_full_path) def print_attributes(cls): columns =
 ["Name", "Type", "Value"] myTable = PrettyTable(columns) for attribute_name,
 attribute_value in vars(cls).items(): attribute_type = type(attribute_value)
 myTable.add_row([attribute_name, attribute_type.__name__, attribute_value])
 print(myTable) print_attributes(settings) ``` ### Output | Name | Type | Value
 | |----------------------|-------|--------------------------| | HOST | str |
 psqlt | | DB_NAME | str | test | | PASSWORD | str | es3bv3v3 | | PORT | int |
 5432 | | USER | str | postgres | | SSL | bool | False | | FLOAT | float | 3.3 |
@@ -123,8 +124,8 @@
 will be documented in this file. The format is based on [Keep a Changelog]
 (https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic
 Versioning](https://semver.org/spec/v2.0.0.html). ## Types of changes - Added
 for new features. - Changed for changes in existing functionality. - Deprecated
 for soon-to-be removed features. - Removed for now removed features. - Fixed
 for any bug fixes. - Security in case of vulnerabilities. ## [0.0.1rcX] - 2024-
 05-27 ### Added - First tests using pypi.org in develop environment. ## [0.1.1-
-5] - 2024-05-27 ### Added - Completion of testing and launch into production.
+6] - 2024-05-27 ### Added - Completion of testing and launch into production.
```

### Comparing `jaanca_utils_os-0.1.5/jaanca_utils_os.egg-info/SOURCES.txt` & `jaanca_utils_os-0.1.6rc1/jaanca_utils_os.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.5/setup.py` & `jaanca_utils_os-0.1.6rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca-utils-os"
-VERSION = "0.1.5"
+VERSION = "0.1.6rc1"
 
 install_requires = [""]
 extras_require = {
     "dotenv": "python-dotenv>=1.0.0"
 }
 
 setup(
```

