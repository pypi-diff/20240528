# Comparing `tmp/jaanca_utils_os-0.1.3.tar.gz` & `tmp/jaanca_utils_os-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca_utils_os-0.1.3.tar", last modified: Mon May 27 23:58:34 2024, max compression
+gzip compressed data, was "jaanca_utils_os-0.1.4.tar", last modified: Tue May 28 00:00:29 2024, max compression
```

## Comparing `jaanca_utils_os-0.1.3.tar` & `jaanca_utils_os-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 23:58:34.725446 jaanca_utils_os-0.1.3/
--rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0    10969 2024-05-27 23:58:34.724449 jaanca_utils_os-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     9562 2024-05-27 23:58:13.000000 jaanca_utils_os-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 23:58:34.695574 jaanca_utils_os-0.1.3/jaanca_utils_os/
--rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.1.3/jaanca_utils_os/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 23:58:34.707450 jaanca_utils_os-0.1.3/jaanca_utils_os/utils/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.3/jaanca_utils_os/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 23:58:34.719446 jaanca_utils_os-0.1.3/jaanca_utils_os/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.3/jaanca_utils_os/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     5671 2024-05-27 23:53:55.000000 jaanca_utils_os-0.1.3/jaanca_utils_os/utils/helpers/environment_parser_loader.py
--rw-rw-rw-   0        0        0     6835 2024-05-27 22:01:52.000000 jaanca_utils_os-0.1.3/jaanca_utils_os/utils/helpers/file_folder_management.py
--rw-rw-rw-   0        0        0     3289 2024-05-27 22:09:16.000000 jaanca_utils_os-0.1.3/jaanca_utils_os/utils/helpers/file_properties.py
--rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.1.3/jaanca_utils_os/utils/helpers/parse_bool.py
--rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.1.3/jaanca_utils_os/utils/helpers/parse_types.py
-drwxrwxrwx   0        0        0        0 2024-05-27 23:58:34.722447 jaanca_utils_os-0.1.3/jaanca_utils_os.egg-info/
--rw-rw-rw-   0        0        0    10969 2024-05-27 23:58:34.000000 jaanca_utils_os-0.1.3/jaanca_utils_os.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      591 2024-05-27 23:58:34.000000 jaanca_utils_os-0.1.3/jaanca_utils_os.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 23:58:34.000000 jaanca_utils_os-0.1.3/jaanca_utils_os.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-27 23:58:34.000000 jaanca_utils_os-0.1.3/jaanca_utils_os.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-27 23:58:34.000000 jaanca_utils_os-0.1.3/jaanca_utils_os.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 23:58:34.726448 jaanca_utils_os-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1756 2024-05-27 23:55:33.000000 jaanca_utils_os-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 00:00:29.772829 jaanca_utils_os-0.1.4/
+-rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0    10892 2024-05-28 00:00:29.771827 jaanca_utils_os-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9485 2024-05-28 00:00:21.000000 jaanca_utils_os-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 00:00:29.745129 jaanca_utils_os-0.1.4/jaanca_utils_os/
+-rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.1.4/jaanca_utils_os/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 00:00:29.757577 jaanca_utils_os-0.1.4/jaanca_utils_os/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.4/jaanca_utils_os/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 00:00:29.767928 jaanca_utils_os-0.1.4/jaanca_utils_os/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.4/jaanca_utils_os/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     5671 2024-05-27 23:53:55.000000 jaanca_utils_os-0.1.4/jaanca_utils_os/utils/helpers/environment_parser_loader.py
+-rw-rw-rw-   0        0        0     6835 2024-05-27 22:01:52.000000 jaanca_utils_os-0.1.4/jaanca_utils_os/utils/helpers/file_folder_management.py
+-rw-rw-rw-   0        0        0     3289 2024-05-27 22:09:16.000000 jaanca_utils_os-0.1.4/jaanca_utils_os/utils/helpers/file_properties.py
+-rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.1.4/jaanca_utils_os/utils/helpers/parse_bool.py
+-rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.1.4/jaanca_utils_os/utils/helpers/parse_types.py
+drwxrwxrwx   0        0        0        0 2024-05-28 00:00:29.769827 jaanca_utils_os-0.1.4/jaanca_utils_os.egg-info/
+-rw-rw-rw-   0        0        0    10892 2024-05-28 00:00:29.000000 jaanca_utils_os-0.1.4/jaanca_utils_os.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      591 2024-05-28 00:00:29.000000 jaanca_utils_os-0.1.4/jaanca_utils_os.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 00:00:29.000000 jaanca_utils_os-0.1.4/jaanca_utils_os.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-28 00:00:29.000000 jaanca_utils_os-0.1.4/jaanca_utils_os.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-28 00:00:29.000000 jaanca_utils_os-0.1.4/jaanca_utils_os.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 00:00:29.773827 jaanca_utils_os-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1756 2024-05-27 23:59:47.000000 jaanca_utils_os-0.1.4/setup.py
```

### Comparing `jaanca_utils_os-0.1.3/LICENSE.txt` & `jaanca_utils_os-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.3/PKG-INFO` & `jaanca_utils_os-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-utils-os
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool library created by jaanca with operating system help functions such as reading environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: datetime,utc
 Classifier: Development Status :: 4 - Beta
@@ -62,16 +62,18 @@
 [Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os)
 | [Package (PyPI)](https://pypi.org/project/jaanca-utils-os/)
 | [Samples](https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os/samples)
 
 ---
 
 # library installation
-```console
-pip install jaanca_utils_os --upgrade
+```console    
+pip install prettytable==3.10.0
+pip install python-dotenv==1.0.0
+pip install jaanca_utils_os[dotenv] --upgrade
 ```
 
 ---
 # environment_parser_loader: Example of use
 
 ### Considerations on environmental variables
 - An object must be specified with the variables that you want to create.
@@ -82,21 +84,14 @@
 - Example:
 ```Python
 class Environment:
     ENV_VAR_NO_EXIT = ("VARIABLE","Not Exist")
     ENV_VAR_IS_MANDATORY = "VARIABLE" 
 ```
 
-### Prerequisites
-```console    
-pip install prettytable==3.10.0
-pip install python-dotenv==1.0.0
-pip install jaanca_utils_os[dotenv] --upgrade
-```
-
 ### File with environments vars .env
 ```console
 ENGINE_POSTGRES_CONN_HOST=psqlt
 ENGINE_POSTGRES_CONN_DB=test
 ENGINE_POSTGRES_CONN_PASSWORD=es3bv3v3
 ENGINE_POSTGRES_CONN_PORT=5432
 ENGINE_POSTGRES_CONN_USER=postgres
@@ -269,11 +264,11 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 ## [0.0.1rcX] - 2024-05-27
 ### Added
 - First tests using pypi.org in develop environment.
 
-## [0.1.1-3] - 2024-05-27
+## [0.1.1-4] - 2024-05-27
 ### Added
 - Completion of testing and launch into production.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.3 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.4 Summary: A tool
 library created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com
 License: MIT License Keywords: datetime,utc Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
@@ -31,27 +31,26 @@
 a default value is not assigned, a KeyError exception will be returned. *
 **FileFolderManagement**: To write files, use the write_to_disk() method *
 **FileProperties**: Functionalities to read properties of an operating system
 file, such as: modification date, creation, size in bytes, among others.
 [Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca-
 utils-os) | [Package (PyPI)](https://pypi.org/project/jaanca-utils-os/) |
 [Samples](https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os/
-samples) --- # library installation ```console pip install jaanca_utils_os --
-upgrade ``` --- # environment_parser_loader: Example of use ### Considerations
-on environmental variables - An object must be specified with the variables
-that you want to create. - The attributes of these objects will be loaded with
-the environment variables, according to the name assigned to them. - If the
+samples) --- # library installation ```console pip install prettytable==3.10.0
+pip install python-dotenv==1.0.0 pip install jaanca_utils_os[dotenv] --upgrade
+``` --- # environment_parser_loader: Example of use ### Considerations on
+environmental variables - An object must be specified with the variables that
+you want to create. - The attributes of these objects will be loaded with the
+environment variables, according to the name assigned to them. - If the
 attribute is mandatory, it will only be of type str and will contain the name
 of the environment variable to read. - If the environment variable is optional
 or may not exist, the attribute must be of type tuple or list, where the first
 element is the environment variable to read and the second the default value to
 assign. - Example: ```Python class Environment: ENV_VAR_NO_EXIT =
-("VARIABLE","Not Exist") ENV_VAR_IS_MANDATORY = "VARIABLE" ``` ###
-Prerequisites ```console pip install prettytable==3.10.0 pip install python-
-dotenv==1.0.0 pip install jaanca_utils_os[dotenv] --upgrade ``` ### File with
+("VARIABLE","Not Exist") ENV_VAR_IS_MANDATORY = "VARIABLE" ``` ### File with
 environments vars .env ```console ENGINE_POSTGRES_CONN_HOST=psqlt
 ENGINE_POSTGRES_CONN_DB=test ENGINE_POSTGRES_CONN_PASSWORD=es3bv3v3
 ENGINE_POSTGRES_CONN_PORT=5432 ENGINE_POSTGRES_CONN_USER=postgres
 ENGINE_POSTGRES_CONN_SSL=false FLOAT=3.3 LIST=[1,2,3,"4","5"] DICT='{"one":
 "one", "two": 2}' BOOL_TRUE = true BOOL_TRUE_ONE = 1 BOOL_TRUE_TWO = "1"
 BOOL_FALSE_ONE = 0 BOOL_FALSE_TWO = "0" BOOL_FALSE_INCORRECT = "incorrect" ```
 ### Example ```Python from jaanca_utils_os import EnvironmentParserLoader,
@@ -122,8 +121,8 @@
 will be documented in this file. The format is based on [Keep a Changelog]
 (https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic
 Versioning](https://semver.org/spec/v2.0.0.html). ## Types of changes - Added
 for new features. - Changed for changes in existing functionality. - Deprecated
 for soon-to-be removed features. - Removed for now removed features. - Fixed
 for any bug fixes. - Security in case of vulnerabilities. ## [0.0.1rcX] - 2024-
 05-27 ### Added - First tests using pypi.org in develop environment. ## [0.1.1-
-3] - 2024-05-27 ### Added - Completion of testing and launch into production.
+4] - 2024-05-27 ### Added - Completion of testing and launch into production.
```

### Comparing `jaanca_utils_os-0.1.3/README.md` & `jaanca_utils_os-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,18 @@
 [Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os)
 | [Package (PyPI)](https://pypi.org/project/jaanca-utils-os/)
 | [Samples](https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os/samples)
 
 ---
 
 # library installation
-```console
-pip install jaanca_utils_os --upgrade
+```console    
+pip install prettytable==3.10.0
+pip install python-dotenv==1.0.0
+pip install jaanca_utils_os[dotenv] --upgrade
 ```
 
 ---
 # environment_parser_loader: Example of use
 
 ### Considerations on environmental variables
 - An object must be specified with the variables that you want to create.
@@ -51,21 +53,14 @@
 - Example:
 ```Python
 class Environment:
     ENV_VAR_NO_EXIT = ("VARIABLE","Not Exist")
     ENV_VAR_IS_MANDATORY = "VARIABLE" 
 ```
 
-### Prerequisites
-```console    
-pip install prettytable==3.10.0
-pip install python-dotenv==1.0.0
-pip install jaanca_utils_os[dotenv] --upgrade
-```
-
 ### File with environments vars .env
 ```console
 ENGINE_POSTGRES_CONN_HOST=psqlt
 ENGINE_POSTGRES_CONN_DB=test
 ENGINE_POSTGRES_CONN_PASSWORD=es3bv3v3
 ENGINE_POSTGRES_CONN_PORT=5432
 ENGINE_POSTGRES_CONN_USER=postgres
@@ -238,11 +233,11 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 ## [0.0.1rcX] - 2024-05-27
 ### Added
 - First tests using pypi.org in develop environment.
 
-## [0.1.1-3] - 2024-05-27
+## [0.1.1-4] - 2024-05-27
 ### Added
 - Completion of testing and launch into production.
```

#### html2text {}

```diff
@@ -13,27 +13,26 @@
 a default value is not assigned, a KeyError exception will be returned. *
 **FileFolderManagement**: To write files, use the write_to_disk() method *
 **FileProperties**: Functionalities to read properties of an operating system
 file, such as: modification date, creation, size in bytes, among others.
 [Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca-
 utils-os) | [Package (PyPI)](https://pypi.org/project/jaanca-utils-os/) |
 [Samples](https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os/
-samples) --- # library installation ```console pip install jaanca_utils_os --
-upgrade ``` --- # environment_parser_loader: Example of use ### Considerations
-on environmental variables - An object must be specified with the variables
-that you want to create. - The attributes of these objects will be loaded with
-the environment variables, according to the name assigned to them. - If the
+samples) --- # library installation ```console pip install prettytable==3.10.0
+pip install python-dotenv==1.0.0 pip install jaanca_utils_os[dotenv] --upgrade
+``` --- # environment_parser_loader: Example of use ### Considerations on
+environmental variables - An object must be specified with the variables that
+you want to create. - The attributes of these objects will be loaded with the
+environment variables, according to the name assigned to them. - If the
 attribute is mandatory, it will only be of type str and will contain the name
 of the environment variable to read. - If the environment variable is optional
 or may not exist, the attribute must be of type tuple or list, where the first
 element is the environment variable to read and the second the default value to
 assign. - Example: ```Python class Environment: ENV_VAR_NO_EXIT =
-("VARIABLE","Not Exist") ENV_VAR_IS_MANDATORY = "VARIABLE" ``` ###
-Prerequisites ```console pip install prettytable==3.10.0 pip install python-
-dotenv==1.0.0 pip install jaanca_utils_os[dotenv] --upgrade ``` ### File with
+("VARIABLE","Not Exist") ENV_VAR_IS_MANDATORY = "VARIABLE" ``` ### File with
 environments vars .env ```console ENGINE_POSTGRES_CONN_HOST=psqlt
 ENGINE_POSTGRES_CONN_DB=test ENGINE_POSTGRES_CONN_PASSWORD=es3bv3v3
 ENGINE_POSTGRES_CONN_PORT=5432 ENGINE_POSTGRES_CONN_USER=postgres
 ENGINE_POSTGRES_CONN_SSL=false FLOAT=3.3 LIST=[1,2,3,"4","5"] DICT='{"one":
 "one", "two": 2}' BOOL_TRUE = true BOOL_TRUE_ONE = 1 BOOL_TRUE_TWO = "1"
 BOOL_FALSE_ONE = 0 BOOL_FALSE_TWO = "0" BOOL_FALSE_INCORRECT = "incorrect" ```
 ### Example ```Python from jaanca_utils_os import EnvironmentParserLoader,
@@ -104,8 +103,8 @@
 will be documented in this file. The format is based on [Keep a Changelog]
 (https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic
 Versioning](https://semver.org/spec/v2.0.0.html). ## Types of changes - Added
 for new features. - Changed for changes in existing functionality. - Deprecated
 for soon-to-be removed features. - Removed for now removed features. - Fixed
 for any bug fixes. - Security in case of vulnerabilities. ## [0.0.1rcX] - 2024-
 05-27 ### Added - First tests using pypi.org in develop environment. ## [0.1.1-
-3] - 2024-05-27 ### Added - Completion of testing and launch into production.
+4] - 2024-05-27 ### Added - Completion of testing and launch into production.
```

### Comparing `jaanca_utils_os-0.1.3/jaanca_utils_os/__init__.py` & `jaanca_utils_os-0.1.4/jaanca_utils_os/__init__.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.3/jaanca_utils_os/utils/helpers/environment_parser_loader.py` & `jaanca_utils_os-0.1.4/jaanca_utils_os/utils/helpers/environment_parser_loader.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.3/jaanca_utils_os/utils/helpers/file_folder_management.py` & `jaanca_utils_os-0.1.4/jaanca_utils_os/utils/helpers/file_folder_management.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.3/jaanca_utils_os/utils/helpers/file_properties.py` & `jaanca_utils_os-0.1.4/jaanca_utils_os/utils/helpers/file_properties.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.3/jaanca_utils_os/utils/helpers/parse_bool.py` & `jaanca_utils_os-0.1.4/jaanca_utils_os/utils/helpers/parse_bool.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.3/jaanca_utils_os/utils/helpers/parse_types.py` & `jaanca_utils_os-0.1.4/jaanca_utils_os/utils/helpers/parse_types.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.3/jaanca_utils_os.egg-info/PKG-INFO` & `jaanca_utils_os-0.1.4/jaanca_utils_os.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-utils-os
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool library created by jaanca with operating system help functions such as reading environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: datetime,utc
 Classifier: Development Status :: 4 - Beta
@@ -62,16 +62,18 @@
 [Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os)
 | [Package (PyPI)](https://pypi.org/project/jaanca-utils-os/)
 | [Samples](https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os/samples)
 
 ---
 
 # library installation
-```console
-pip install jaanca_utils_os --upgrade
+```console    
+pip install prettytable==3.10.0
+pip install python-dotenv==1.0.0
+pip install jaanca_utils_os[dotenv] --upgrade
 ```
 
 ---
 # environment_parser_loader: Example of use
 
 ### Considerations on environmental variables
 - An object must be specified with the variables that you want to create.
@@ -82,21 +84,14 @@
 - Example:
 ```Python
 class Environment:
     ENV_VAR_NO_EXIT = ("VARIABLE","Not Exist")
     ENV_VAR_IS_MANDATORY = "VARIABLE" 
 ```
 
-### Prerequisites
-```console    
-pip install prettytable==3.10.0
-pip install python-dotenv==1.0.0
-pip install jaanca_utils_os[dotenv] --upgrade
-```
-
 ### File with environments vars .env
 ```console
 ENGINE_POSTGRES_CONN_HOST=psqlt
 ENGINE_POSTGRES_CONN_DB=test
 ENGINE_POSTGRES_CONN_PASSWORD=es3bv3v3
 ENGINE_POSTGRES_CONN_PORT=5432
 ENGINE_POSTGRES_CONN_USER=postgres
@@ -269,11 +264,11 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 ## [0.0.1rcX] - 2024-05-27
 ### Added
 - First tests using pypi.org in develop environment.
 
-## [0.1.1-3] - 2024-05-27
+## [0.1.1-4] - 2024-05-27
 ### Added
 - Completion of testing and launch into production.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.3 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.4 Summary: A tool
 library created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com
 License: MIT License Keywords: datetime,utc Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
@@ -31,27 +31,26 @@
 a default value is not assigned, a KeyError exception will be returned. *
 **FileFolderManagement**: To write files, use the write_to_disk() method *
 **FileProperties**: Functionalities to read properties of an operating system
 file, such as: modification date, creation, size in bytes, among others.
 [Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca-
 utils-os) | [Package (PyPI)](https://pypi.org/project/jaanca-utils-os/) |
 [Samples](https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os/
-samples) --- # library installation ```console pip install jaanca_utils_os --
-upgrade ``` --- # environment_parser_loader: Example of use ### Considerations
-on environmental variables - An object must be specified with the variables
-that you want to create. - The attributes of these objects will be loaded with
-the environment variables, according to the name assigned to them. - If the
+samples) --- # library installation ```console pip install prettytable==3.10.0
+pip install python-dotenv==1.0.0 pip install jaanca_utils_os[dotenv] --upgrade
+``` --- # environment_parser_loader: Example of use ### Considerations on
+environmental variables - An object must be specified with the variables that
+you want to create. - The attributes of these objects will be loaded with the
+environment variables, according to the name assigned to them. - If the
 attribute is mandatory, it will only be of type str and will contain the name
 of the environment variable to read. - If the environment variable is optional
 or may not exist, the attribute must be of type tuple or list, where the first
 element is the environment variable to read and the second the default value to
 assign. - Example: ```Python class Environment: ENV_VAR_NO_EXIT =
-("VARIABLE","Not Exist") ENV_VAR_IS_MANDATORY = "VARIABLE" ``` ###
-Prerequisites ```console pip install prettytable==3.10.0 pip install python-
-dotenv==1.0.0 pip install jaanca_utils_os[dotenv] --upgrade ``` ### File with
+("VARIABLE","Not Exist") ENV_VAR_IS_MANDATORY = "VARIABLE" ``` ### File with
 environments vars .env ```console ENGINE_POSTGRES_CONN_HOST=psqlt
 ENGINE_POSTGRES_CONN_DB=test ENGINE_POSTGRES_CONN_PASSWORD=es3bv3v3
 ENGINE_POSTGRES_CONN_PORT=5432 ENGINE_POSTGRES_CONN_USER=postgres
 ENGINE_POSTGRES_CONN_SSL=false FLOAT=3.3 LIST=[1,2,3,"4","5"] DICT='{"one":
 "one", "two": 2}' BOOL_TRUE = true BOOL_TRUE_ONE = 1 BOOL_TRUE_TWO = "1"
 BOOL_FALSE_ONE = 0 BOOL_FALSE_TWO = "0" BOOL_FALSE_INCORRECT = "incorrect" ```
 ### Example ```Python from jaanca_utils_os import EnvironmentParserLoader,
@@ -122,8 +121,8 @@
 will be documented in this file. The format is based on [Keep a Changelog]
 (https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic
 Versioning](https://semver.org/spec/v2.0.0.html). ## Types of changes - Added
 for new features. - Changed for changes in existing functionality. - Deprecated
 for soon-to-be removed features. - Removed for now removed features. - Fixed
 for any bug fixes. - Security in case of vulnerabilities. ## [0.0.1rcX] - 2024-
 05-27 ### Added - First tests using pypi.org in develop environment. ## [0.1.1-
-3] - 2024-05-27 ### Added - Completion of testing and launch into production.
+4] - 2024-05-27 ### Added - Completion of testing and launch into production.
```

### Comparing `jaanca_utils_os-0.1.3/jaanca_utils_os.egg-info/SOURCES.txt` & `jaanca_utils_os-0.1.4/jaanca_utils_os.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.1.3/setup.py` & `jaanca_utils_os-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca-utils-os"
-VERSION = "0.1.3"
+VERSION = "0.1.4"
 
 install_requires = [""]
 extras_require = {
     "dotenv": "python-dotenv>=1.0.0"
 }
 
 setup(
```
