# Comparing `tmp/jaanca_utils_os-0.1.0.tar.gz` & `tmp/jaanca_utils_os-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca_utils_os-0.1.0.tar", last modified: Mon May 27 22:22:43 2024, max compression
+gzip compressed data, was "jaanca_utils_os-0.1.1.tar", last modified: Mon May 27 23:23:51 2024, max compression
```

## Comparing `jaanca_utils_os-0.1.0.tar` & `jaanca_utils_os-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 22:22:43.115286 jaanca_utils_os-0.1.0/
--rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0    10226 2024-05-27 22:22:43.115286 jaanca_utils_os-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     8819 2024-05-27 22:17:09.000000 jaanca_utils_os-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 22:22:43.088285 jaanca_utils_os-0.1.0/jaanca_utils_os/
--rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.1.0/jaanca_utils_os/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 22:22:43.099287 jaanca_utils_os-0.1.0/jaanca_utils_os/utils/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.0/jaanca_utils_os/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 22:22:43.111286 jaanca_utils_os-0.1.0/jaanca_utils_os/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.0/jaanca_utils_os/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     4699 2024-05-27 21:37:19.000000 jaanca_utils_os-0.1.0/jaanca_utils_os/utils/helpers/environment_parser_loader.py
--rw-rw-rw-   0        0        0     6835 2024-05-27 22:01:52.000000 jaanca_utils_os-0.1.0/jaanca_utils_os/utils/helpers/file_folder_management.py
--rw-rw-rw-   0        0        0     3289 2024-05-27 22:09:16.000000 jaanca_utils_os-0.1.0/jaanca_utils_os/utils/helpers/file_properties.py
--rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.1.0/jaanca_utils_os/utils/helpers/parse_bool.py
--rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.1.0/jaanca_utils_os/utils/helpers/parse_types.py
-drwxrwxrwx   0        0        0        0 2024-05-27 22:22:43.113285 jaanca_utils_os-0.1.0/jaanca_utils_os.egg-info/
--rw-rw-rw-   0        0        0    10226 2024-05-27 22:22:43.000000 jaanca_utils_os-0.1.0/jaanca_utils_os.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      591 2024-05-27 22:22:43.000000 jaanca_utils_os-0.1.0/jaanca_utils_os.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 22:22:43.000000 jaanca_utils_os-0.1.0/jaanca_utils_os.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-27 22:22:43.000000 jaanca_utils_os-0.1.0/jaanca_utils_os.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-27 22:22:43.000000 jaanca_utils_os-0.1.0/jaanca_utils_os.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 22:22:43.117285 jaanca_utils_os-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1756 2024-05-27 22:19:24.000000 jaanca_utils_os-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 23:23:51.343792 jaanca_utils_os-0.1.1/
+-rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0    10964 2024-05-27 23:23:51.342793 jaanca_utils_os-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9557 2024-05-27 23:23:26.000000 jaanca_utils_os-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 23:23:51.316795 jaanca_utils_os-0.1.1/jaanca_utils_os/
+-rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.1.1/jaanca_utils_os/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 23:23:51.327794 jaanca_utils_os-0.1.1/jaanca_utils_os/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.1/jaanca_utils_os/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 23:23:51.338793 jaanca_utils_os-0.1.1/jaanca_utils_os/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.1/jaanca_utils_os/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     5442 2024-05-27 23:20:08.000000 jaanca_utils_os-0.1.1/jaanca_utils_os/utils/helpers/environment_parser_loader.py
+-rw-rw-rw-   0        0        0     6835 2024-05-27 22:01:52.000000 jaanca_utils_os-0.1.1/jaanca_utils_os/utils/helpers/file_folder_management.py
+-rw-rw-rw-   0        0        0     3289 2024-05-27 22:09:16.000000 jaanca_utils_os-0.1.1/jaanca_utils_os/utils/helpers/file_properties.py
+-rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.1.1/jaanca_utils_os/utils/helpers/parse_bool.py
+-rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.1.1/jaanca_utils_os/utils/helpers/parse_types.py
+drwxrwxrwx   0        0        0        0 2024-05-27 23:23:51.341794 jaanca_utils_os-0.1.1/jaanca_utils_os.egg-info/
+-rw-rw-rw-   0        0        0    10964 2024-05-27 23:23:51.000000 jaanca_utils_os-0.1.1/jaanca_utils_os.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      591 2024-05-27 23:23:51.000000 jaanca_utils_os-0.1.1/jaanca_utils_os.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 23:23:51.000000 jaanca_utils_os-0.1.1/jaanca_utils_os.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-27 23:23:51.000000 jaanca_utils_os-0.1.1/jaanca_utils_os.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-27 23:23:51.000000 jaanca_utils_os-0.1.1/jaanca_utils_os.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 23:23:51.345792 jaanca_utils_os-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1756 2024-05-27 23:23:06.000000 jaanca_utils_os-0.1.1/setup.py
```

### Comparing `jaanca_utils_os-0.1.0/LICENSE.txt` & `jaanca_utils_os-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.0/PKG-INFO` & `jaanca_utils_os-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,7 @@
-Metadata-Version: 2.1
-Name: jaanca-utils-os
-Version: 0.1.0
-Summary: A tool library created by jaanca with operating system help functions such as reading environment variables, reading/writing files, file properties, among others.
-Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
-Author: Jaime Andres Cardona Carrillo
-Author-email: jacardona@outlook.com
-License: MIT License
-Keywords: datetime,utc
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: System :: Monitoring
-Classifier: Topic :: Software Development
-Classifier: Typing :: Typed
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Provides-Extra: dotenv
-Requires-Dist: python-dotenv>=1.0.1; extra == "dotenv"
-
 <p align="center">
     <em>jaanca public libraries</em>
 </p>
 
 <p align="center">
 <a href="https://pypi.org/project/jaanca-utils-os" target="_blank">
     <img src="https://img.shields.io/pypi/v/jaanca-utils-os?color=blue&label=PyPI%20Package" alt="Package version">
@@ -48,15 +17,15 @@
 #  A tool library created by jaanca
 
 * **Python library**: A tool library created by jaanca with operating system help functions such as reading environment variables, reading/writing files, file properties, among others.
 * **EnvironmentParserLoader**: A class that loads, parses, and manages system environment variables into various data types.
     General Functionality
 
     ## The EnvironmentParserLoader class would be designed to:
-    - Read the systemâ€™s environment variables.
+    - Read the system’s environment variables.
     - Parse (convert) these variables into specific data types (such as int, float, bool, str, list, dict).
     - Manage and provide centralized methods to access these environment variables in a typed and secure manner.
     - If the environment variable does not exist or has a value of None and a default value is not assigned, a KeyError exception will be returned.
 * **FileFolderManagement**: To write files, use the write_to_disk() method
 * **FileProperties**: Functionalities to read properties of an operating system file, such as: modification date, creation, size in bytes, among others.
 
 [Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os)
@@ -69,18 +38,32 @@
 ```console
 pip install jaanca_utils_os --upgrade
 ```
 
 ---
 # environment_parser_loader: Example of use
 
+### Considerations on environmental variables
+- An object must be specified with the variables that you want to create.
+- The attributes of these objects will be loaded with the environment variables, according to the name assigned to them.
+- If the attribute is mandatory, it will only be of type str and will contain the name of the environment variable to read.
+- If the environment variable is optional or may not exist, the attribute must be of type tuple or list, where the first element is the environment variable to read and the second the default value to assign.
+
+- Example:
+```Python
+class Environment:
+    ENV_VAR_NO_EXIT = ("VARIABLE","Not Exist")
+    ENV_VAR_IS_MANDATORY = "VARIABLE" 
+```
+
+### Prerequisites
 ```console    
-pip install prettytable==3.10.0
-pip install python-dotenv==1.0.1
-pip install jaanca_utils_os[dotenv]==0.1.0
+pip install prettytable>=3.10.0
+pip install python-dotenv>=1.0.0
+pip install jaanca_utils_os[dotenv]>=0.1.1
 ```
 
 ### File with environments vars .env
 ```console
 ENGINE_POSTGRES_CONN_HOST=psqlt
 ENGINE_POSTGRES_CONN_DB=test
 ENGINE_POSTGRES_CONN_PASSWORD=es3bv3v3
```

#### html2text {}

```diff
@@ -1,58 +1,49 @@
-Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.0 Summary: A tool
-library created by jaanca with operating system help functions such as reading
-environment variables, reading/writing files, file properties, among others.
-Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
-Author: Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com
-License: MIT License Keywords: datetime,utc Classifier: Development Status :: 4
-- Beta Classifier: Intended Audience :: Developers Classifier: Intended
-Audience :: Information Technology Classifier: Intended Audience :: System
-Administrators Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-:: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Classifier: Topic :: System :: Monitoring
-Classifier: Topic :: Software Development Classifier: Typing :: Typed Requires-
-Python: >=3.8 Description-Content-Type: text/markdown License-File: LICENSE.txt
-Provides-Extra: dotenv Requires-Dist: python-dotenv>=1.0.1; extra == "dotenv"
                             jjaaaannccaa ppuubblliicc lliibbrraarriieess
                            _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]
 --- # A tool library created by jaanca * **Python library**: A tool library
 created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others. *
 **EnvironmentParserLoader**: A class that loads, parses, and manages system
 environment variables into various data types. General Functionality ## The
-EnvironmentParserLoader class would be designed to: - Read the systemÃ¢â¬â¢s
+EnvironmentParserLoader class would be designed to: - Read the systemâs
 environment variables. - Parse (convert) these variables into specific data
 types (such as int, float, bool, str, list, dict). - Manage and provide
 centralized methods to access these environment variables in a typed and secure
 manner. - If the environment variable does not exist or has a value of None and
 a default value is not assigned, a KeyError exception will be returned. *
 **FileFolderManagement**: To write files, use the write_to_disk() method *
 **FileProperties**: Functionalities to read properties of an operating system
 file, such as: modification date, creation, size in bytes, among others.
 [Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca-
 utils-os) | [Package (PyPI)](https://pypi.org/project/jaanca-utils-os/) |
 [Samples](https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os/
 samples) --- # library installation ```console pip install jaanca_utils_os --
-upgrade ``` --- # environment_parser_loader: Example of use ```console pip
-install prettytable==3.10.0 pip install python-dotenv==1.0.1 pip install
-jaanca_utils_os[dotenv]==0.1.0 ``` ### File with environments vars .env
-```console ENGINE_POSTGRES_CONN_HOST=psqlt ENGINE_POSTGRES_CONN_DB=test
-ENGINE_POSTGRES_CONN_PASSWORD=es3bv3v3 ENGINE_POSTGRES_CONN_PORT=5432
-ENGINE_POSTGRES_CONN_USER=postgres ENGINE_POSTGRES_CONN_SSL=false FLOAT=3.3
-LIST=[1,2,3,"4","5"] DICT='{"one": "one", "two": 2}' BOOL_TRUE = true
-BOOL_TRUE_ONE = 1 BOOL_TRUE_TWO = "1" BOOL_FALSE_ONE = 0 BOOL_FALSE_TWO = "0"
-BOOL_FALSE_INCORRECT = "incorrect" ``` ### Example ```Python from
-jaanca_utils_os import EnvironmentParserLoader, FileFolderManagement from
-prettytable import PrettyTable class Environment: HOST =
-"ENGINE_POSTGRES_CONN_HOST" DB_NAME = "ENGINE_POSTGRES_CONN_DB" PASSWORD =
-"ENGINE_POSTGRES_CONN_PASSWORD" PORT = "ENGINE_POSTGRES_CONN_PORT" USER =
+upgrade ``` --- # environment_parser_loader: Example of use ### Considerations
+on environmental variables - An object must be specified with the variables
+that you want to create. - The attributes of these objects will be loaded with
+the environment variables, according to the name assigned to them. - If the
+attribute is mandatory, it will only be of type str and will contain the name
+of the environment variable to read. - If the environment variable is optional
+or may not exist, the attribute must be of type tuple or list, where the first
+element is the environment variable to read and the second the default value to
+assign. - Example: ```Python class Environment: ENV_VAR_NO_EXIT =
+("VARIABLE","Not Exist") ENV_VAR_IS_MANDATORY = "VARIABLE" ``` ###
+Prerequisites ```console pip install prettytable>=3.10.0 pip install python-
+dotenv>=1.0.0 pip install jaanca_utils_os[dotenv]>=0.1.1 ``` ### File with
+environments vars .env ```console ENGINE_POSTGRES_CONN_HOST=psqlt
+ENGINE_POSTGRES_CONN_DB=test ENGINE_POSTGRES_CONN_PASSWORD=es3bv3v3
+ENGINE_POSTGRES_CONN_PORT=5432 ENGINE_POSTGRES_CONN_USER=postgres
+ENGINE_POSTGRES_CONN_SSL=false FLOAT=3.3 LIST=[1,2,3,"4","5"] DICT='{"one":
+"one", "two": 2}' BOOL_TRUE = true BOOL_TRUE_ONE = 1 BOOL_TRUE_TWO = "1"
+BOOL_FALSE_ONE = 0 BOOL_FALSE_TWO = "0" BOOL_FALSE_INCORRECT = "incorrect" ```
+### Example ```Python from jaanca_utils_os import EnvironmentParserLoader,
+FileFolderManagement from prettytable import PrettyTable class Environment:
+HOST = "ENGINE_POSTGRES_CONN_HOST" DB_NAME = "ENGINE_POSTGRES_CONN_DB" PASSWORD
+= "ENGINE_POSTGRES_CONN_PASSWORD" PORT = "ENGINE_POSTGRES_CONN_PORT" USER =
 "ENGINE_POSTGRES_CONN_USER" SSL = "ENGINE_POSTGRES_CONN_SSL" FLOAT = "FLOAT"
 LIST = "LIST" DICT = "DICT" BOOL_TRUE = "BOOL_TRUE" BOOL_TRUE_ONE =
 "BOOL_TRUE_ONE" BOOL_TRUE_TWO = "BOOL_TRUE_TWO" BOOL_FALSE_ONE =
 "BOOL_FALSE_ONE" BOOL_FALSE_TWO = "BOOL_FALSE_TWO" BOOL_FALSE_INCORRECT =
 "BOOL_FALSE_INCORRECT" NO_DATA_TUPLE = ("VARIABLE","Not Exist") NO_DATA_LIST =
 ["VARIABLE","Not Exist"] NO_DATA_BOOL = ["VARIABLE","1"] # Load varibles from
 current folder env_full_path =
```

### Comparing `jaanca_utils_os-0.1.0/jaanca_utils_os/__init__.py` & `jaanca_utils_os-0.1.1/jaanca_utils_os/__init__.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.0/jaanca_utils_os/utils/helpers/environment_parser_loader.py` & `jaanca_utils_os-0.1.1/jaanca_utils_os/utils/helpers/environment_parser_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,25 @@
 
     ## The EnvironmentParserLoader class would be designed to:
     - Read the system’s environment variables.
     - Parse (convert) these variables into specific data types (such as int, float, bool, str, list, dict).
     - Manage and provide centralized methods to access these environment variables in a typed and secure manner.
     - If the environment variable does not exist or has a value of None and a default value is not assigned, a KeyError exception will be returned.
 
+    ## Considerations on environmental variables
+    - An object must be specified with the variables that you want to create.
+    - The attributes of these objects will be loaded with the environment variables, according to the name assigned to them.
+    - If the attribute is mandatory, it will only be of type str and will contain the name of the environment variable to read.
+    - If the environment variable is optional or may not exist, the attribute must be of type tuple or list, where the first element is the environment variable to read and the second the default value to assign.
+
+    Example:
+    class Environment:
+        ENV_VAR_NO_EXIT = ("VARIABLE","Not Exist")
+        ENV_VAR_IS_MANDATORY = "VARIABLE"    
+    
     ### Example: Prerequisites
     ```console    
     pip install prettytable==3.10.0
     pip install python-dotenv==1.0.1
     ```
 
     ### File with environments vars .env
```

### Comparing `jaanca_utils_os-0.1.0/jaanca_utils_os/utils/helpers/file_folder_management.py` & `jaanca_utils_os-0.1.1/jaanca_utils_os/utils/helpers/file_folder_management.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.0/jaanca_utils_os/utils/helpers/file_properties.py` & `jaanca_utils_os-0.1.1/jaanca_utils_os/utils/helpers/file_properties.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.0/jaanca_utils_os/utils/helpers/parse_bool.py` & `jaanca_utils_os-0.1.1/jaanca_utils_os/utils/helpers/parse_bool.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.0/jaanca_utils_os/utils/helpers/parse_types.py` & `jaanca_utils_os-0.1.1/jaanca_utils_os/utils/helpers/parse_types.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.0/jaanca_utils_os.egg-info/PKG-INFO` & `jaanca_utils_os-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-utils-os
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool library created by jaanca with operating system help functions such as reading environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: datetime,utc
 Classifier: Development Status :: 4 - Beta
@@ -69,18 +69,32 @@
 ```console
 pip install jaanca_utils_os --upgrade
 ```
 
 ---
 # environment_parser_loader: Example of use
 
+### Considerations on environmental variables
+- An object must be specified with the variables that you want to create.
+- The attributes of these objects will be loaded with the environment variables, according to the name assigned to them.
+- If the attribute is mandatory, it will only be of type str and will contain the name of the environment variable to read.
+- If the environment variable is optional or may not exist, the attribute must be of type tuple or list, where the first element is the environment variable to read and the second the default value to assign.
+
+- Example:
+```Python
+class Environment:
+    ENV_VAR_NO_EXIT = ("VARIABLE","Not Exist")
+    ENV_VAR_IS_MANDATORY = "VARIABLE" 
+```
+
+### Prerequisites
 ```console    
-pip install prettytable==3.10.0
-pip install python-dotenv==1.0.1
-pip install jaanca_utils_os[dotenv]==0.1.0
+pip install prettytable>=3.10.0
+pip install python-dotenv>=1.0.0
+pip install jaanca_utils_os[dotenv]>=0.1.1
 ```
 
 ### File with environments vars .env
 ```console
 ENGINE_POSTGRES_CONN_HOST=psqlt
 ENGINE_POSTGRES_CONN_DB=test
 ENGINE_POSTGRES_CONN_PASSWORD=es3bv3v3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.0 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.1 Summary: A tool
 library created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com
 License: MIT License Keywords: datetime,utc Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
@@ -32,27 +32,36 @@
 **FileFolderManagement**: To write files, use the write_to_disk() method *
 **FileProperties**: Functionalities to read properties of an operating system
 file, such as: modification date, creation, size in bytes, among others.
 [Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca-
 utils-os) | [Package (PyPI)](https://pypi.org/project/jaanca-utils-os/) |
 [Samples](https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os/
 samples) --- # library installation ```console pip install jaanca_utils_os --
-upgrade ``` --- # environment_parser_loader: Example of use ```console pip
-install prettytable==3.10.0 pip install python-dotenv==1.0.1 pip install
-jaanca_utils_os[dotenv]==0.1.0 ``` ### File with environments vars .env
-```console ENGINE_POSTGRES_CONN_HOST=psqlt ENGINE_POSTGRES_CONN_DB=test
-ENGINE_POSTGRES_CONN_PASSWORD=es3bv3v3 ENGINE_POSTGRES_CONN_PORT=5432
-ENGINE_POSTGRES_CONN_USER=postgres ENGINE_POSTGRES_CONN_SSL=false FLOAT=3.3
-LIST=[1,2,3,"4","5"] DICT='{"one": "one", "two": 2}' BOOL_TRUE = true
-BOOL_TRUE_ONE = 1 BOOL_TRUE_TWO = "1" BOOL_FALSE_ONE = 0 BOOL_FALSE_TWO = "0"
-BOOL_FALSE_INCORRECT = "incorrect" ``` ### Example ```Python from
-jaanca_utils_os import EnvironmentParserLoader, FileFolderManagement from
-prettytable import PrettyTable class Environment: HOST =
-"ENGINE_POSTGRES_CONN_HOST" DB_NAME = "ENGINE_POSTGRES_CONN_DB" PASSWORD =
-"ENGINE_POSTGRES_CONN_PASSWORD" PORT = "ENGINE_POSTGRES_CONN_PORT" USER =
+upgrade ``` --- # environment_parser_loader: Example of use ### Considerations
+on environmental variables - An object must be specified with the variables
+that you want to create. - The attributes of these objects will be loaded with
+the environment variables, according to the name assigned to them. - If the
+attribute is mandatory, it will only be of type str and will contain the name
+of the environment variable to read. - If the environment variable is optional
+or may not exist, the attribute must be of type tuple or list, where the first
+element is the environment variable to read and the second the default value to
+assign. - Example: ```Python class Environment: ENV_VAR_NO_EXIT =
+("VARIABLE","Not Exist") ENV_VAR_IS_MANDATORY = "VARIABLE" ``` ###
+Prerequisites ```console pip install prettytable>=3.10.0 pip install python-
+dotenv>=1.0.0 pip install jaanca_utils_os[dotenv]>=0.1.1 ``` ### File with
+environments vars .env ```console ENGINE_POSTGRES_CONN_HOST=psqlt
+ENGINE_POSTGRES_CONN_DB=test ENGINE_POSTGRES_CONN_PASSWORD=es3bv3v3
+ENGINE_POSTGRES_CONN_PORT=5432 ENGINE_POSTGRES_CONN_USER=postgres
+ENGINE_POSTGRES_CONN_SSL=false FLOAT=3.3 LIST=[1,2,3,"4","5"] DICT='{"one":
+"one", "two": 2}' BOOL_TRUE = true BOOL_TRUE_ONE = 1 BOOL_TRUE_TWO = "1"
+BOOL_FALSE_ONE = 0 BOOL_FALSE_TWO = "0" BOOL_FALSE_INCORRECT = "incorrect" ```
+### Example ```Python from jaanca_utils_os import EnvironmentParserLoader,
+FileFolderManagement from prettytable import PrettyTable class Environment:
+HOST = "ENGINE_POSTGRES_CONN_HOST" DB_NAME = "ENGINE_POSTGRES_CONN_DB" PASSWORD
+= "ENGINE_POSTGRES_CONN_PASSWORD" PORT = "ENGINE_POSTGRES_CONN_PORT" USER =
 "ENGINE_POSTGRES_CONN_USER" SSL = "ENGINE_POSTGRES_CONN_SSL" FLOAT = "FLOAT"
 LIST = "LIST" DICT = "DICT" BOOL_TRUE = "BOOL_TRUE" BOOL_TRUE_ONE =
 "BOOL_TRUE_ONE" BOOL_TRUE_TWO = "BOOL_TRUE_TWO" BOOL_FALSE_ONE =
 "BOOL_FALSE_ONE" BOOL_FALSE_TWO = "BOOL_FALSE_TWO" BOOL_FALSE_INCORRECT =
 "BOOL_FALSE_INCORRECT" NO_DATA_TUPLE = ("VARIABLE","Not Exist") NO_DATA_LIST =
 ["VARIABLE","Not Exist"] NO_DATA_BOOL = ["VARIABLE","1"] # Load varibles from
 current folder env_full_path =
```

### Comparing `jaanca_utils_os-0.1.0/jaanca_utils_os.egg-info/SOURCES.txt` & `jaanca_utils_os-0.1.1/jaanca_utils_os.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.0/setup.py` & `jaanca_utils_os-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca-utils-os"
-VERSION = "0.1.0"
+VERSION = "0.1.1"
 
 install_requires = [""]
 extras_require = {
     "dotenv": "python-dotenv>=1.0.1"
 }
 
 setup(
```

