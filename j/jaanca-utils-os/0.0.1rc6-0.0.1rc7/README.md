# Comparing `tmp/jaanca_utils_os-0.0.1rc6.tar.gz` & `tmp/jaanca_utils_os-0.0.1rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca_utils_os-0.0.1rc6.tar", last modified: Mon May 27 22:12:21 2024, max compression
+gzip compressed data, was "jaanca_utils_os-0.0.1rc7.tar", last modified: Mon May 27 22:17:33 2024, max compression
```

## Comparing `jaanca_utils_os-0.0.1rc6.tar` & `jaanca_utils_os-0.0.1rc7.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 22:12:21.446790 jaanca_utils_os-0.0.1rc6/
--rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc6/LICENSE.txt
--rw-rw-rw-   0        0        0    10105 2024-05-27 22:12:21.445790 jaanca_utils_os-0.0.1rc6/PKG-INFO
--rw-rw-rw-   0        0        0     8775 2024-05-27 22:11:48.000000 jaanca_utils_os-0.0.1rc6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 22:12:21.421789 jaanca_utils_os-0.0.1rc6/jaanca_utils_os/
--rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.0.1rc6/jaanca_utils_os/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 22:12:21.430790 jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 22:12:21.441789 jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     4699 2024-05-27 21:37:19.000000 jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/helpers/environment_parser_loader.py
--rw-rw-rw-   0        0        0     6835 2024-05-27 22:01:52.000000 jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/helpers/file_folder_management.py
--rw-rw-rw-   0        0        0     3289 2024-05-27 22:09:16.000000 jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/helpers/file_properties.py
--rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/helpers/parse_bool.py
--rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/helpers/parse_types.py
-drwxrwxrwx   0        0        0        0 2024-05-27 22:12:21.444790 jaanca_utils_os-0.0.1rc6/jaanca_utils_os.egg-info/
--rw-rw-rw-   0        0        0    10105 2024-05-27 22:12:21.000000 jaanca_utils_os-0.0.1rc6/jaanca_utils_os.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2024-05-27 22:12:21.000000 jaanca_utils_os-0.0.1rc6/jaanca_utils_os.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 22:12:21.000000 jaanca_utils_os-0.0.1rc6/jaanca_utils_os.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-27 22:12:21.000000 jaanca_utils_os-0.0.1rc6/jaanca_utils_os.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 22:12:21.447792 jaanca_utils_os-0.0.1rc6/setup.cfg
--rw-rw-rw-   0        0        0     1662 2024-05-27 22:12:16.000000 jaanca_utils_os-0.0.1rc6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:17:33.015960 jaanca_utils_os-0.0.1rc7/
+-rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc7/LICENSE.txt
+-rw-rw-rw-   0        0        0    10229 2024-05-27 22:17:33.014959 jaanca_utils_os-0.0.1rc7/PKG-INFO
+-rw-rw-rw-   0        0        0     8819 2024-05-27 22:17:09.000000 jaanca_utils_os-0.0.1rc7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 22:17:32.987960 jaanca_utils_os-0.0.1rc7/jaanca_utils_os/
+-rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:17:32.999962 jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:17:33.010959 jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     4699 2024-05-27 21:37:19.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/helpers/environment_parser_loader.py
+-rw-rw-rw-   0        0        0     6835 2024-05-27 22:01:52.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/helpers/file_folder_management.py
+-rw-rw-rw-   0        0        0     3289 2024-05-27 22:09:16.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/helpers/file_properties.py
+-rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/helpers/parse_bool.py
+-rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/helpers/parse_types.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:17:33.012962 jaanca_utils_os-0.0.1rc7/jaanca_utils_os.egg-info/
+-rw-rw-rw-   0        0        0    10229 2024-05-27 22:17:32.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      591 2024-05-27 22:17:32.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 22:17:32.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-27 22:17:32.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-27 22:17:32.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 22:17:33.016960 jaanca_utils_os-0.0.1rc7/setup.cfg
+-rw-rw-rw-   0        0        0     1759 2024-05-27 22:17:27.000000 jaanca_utils_os-0.0.1rc7/setup.py
```

### Comparing `jaanca_utils_os-0.0.1rc6/LICENSE.txt` & `jaanca_utils_os-0.0.1rc7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc6/PKG-INFO` & `jaanca_utils_os-0.0.1rc7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-utils-os
-Version: 0.0.1rc6
+Version: 0.0.1rc7
 Summary: A tool library created by jaanca with operating system help functions such as reading environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: datetime,utc
 Classifier: Development Status :: 4 - Beta
@@ -22,14 +22,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Provides-Extra: dotenv
+Requires-Dist: python-dotenv>=1.0.1; extra == "dotenv"
 
 <p align="center">
     <em>jaanca public libraries</em>
 </p>
 
 <p align="center">
 <a href="https://pypi.org/project/jaanca-utils-os" target="_blank">
@@ -70,14 +72,15 @@
 
 ---
 # environment_parser_loader: Example of use
 
 ```console    
 pip install prettytable==3.10.0
 pip install python-dotenv==1.0.1
+pip install jaanca_utils_os[dotenv]==0.1.0
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
-Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.0.1rc6 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.0.1rc7 Summary: A tool
 library created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com
 License: MIT License Keywords: datetime,utc Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
@@ -11,14 +11,15 @@
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Software Development Classifier: Typing :: Typed Requires-
 Python: >=3.8 Description-Content-Type: text/markdown License-File: LICENSE.txt
+Provides-Extra: dotenv Requires-Dist: python-dotenv>=1.0.1; extra == "dotenv"
                             jjaaaannccaa ppuubblliicc lliibbrraarriieess
                            _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]
 --- # A tool library created by jaanca * **Python library**: A tool library
 created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others. *
 **EnvironmentParserLoader**: A class that loads, parses, and manages system
 environment variables into various data types. General Functionality ## The
@@ -32,25 +33,26 @@
 **FileProperties**: Functionalities to read properties of an operating system
 file, such as: modification date, creation, size in bytes, among others.
 [Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca-
 utils-os) | [Package (PyPI)](https://pypi.org/project/jaanca-utils-os/) |
 [Samples](https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os/
 samples) --- # library installation ```console pip install jaanca_utils_os --
 upgrade ``` --- # environment_parser_loader: Example of use ```console pip
-install prettytable==3.10.0 pip install python-dotenv==1.0.1 ``` ### File with
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
+install prettytable==3.10.0 pip install python-dotenv==1.0.1 pip install
+jaanca_utils_os[dotenv]==0.1.0 ``` ### File with environments vars .env
+```console ENGINE_POSTGRES_CONN_HOST=psqlt ENGINE_POSTGRES_CONN_DB=test
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
```

### Comparing `jaanca_utils_os-0.0.1rc6/README.md` & `jaanca_utils_os-0.0.1rc7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
 ---
 # environment_parser_loader: Example of use
 
 ```console    
 pip install prettytable==3.10.0
 pip install python-dotenv==1.0.1
+pip install jaanca_utils_os[dotenv]==0.1.0
 ```
 
 ### File with environments vars .env
 ```console
 ENGINE_POSTGRES_CONN_HOST=psqlt
 ENGINE_POSTGRES_CONN_DB=test
 ENGINE_POSTGRES_CONN_PASSWORD=es3bv3v3
```

#### html2text {}

```diff
@@ -15,25 +15,26 @@
 **FileProperties**: Functionalities to read properties of an operating system
 file, such as: modification date, creation, size in bytes, among others.
 [Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca-
 utils-os) | [Package (PyPI)](https://pypi.org/project/jaanca-utils-os/) |
 [Samples](https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os/
 samples) --- # library installation ```console pip install jaanca_utils_os --
 upgrade ``` --- # environment_parser_loader: Example of use ```console pip
-install prettytable==3.10.0 pip install python-dotenv==1.0.1 ``` ### File with
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
+install prettytable==3.10.0 pip install python-dotenv==1.0.1 pip install
+jaanca_utils_os[dotenv]==0.1.0 ``` ### File with environments vars .env
+```console ENGINE_POSTGRES_CONN_HOST=psqlt ENGINE_POSTGRES_CONN_DB=test
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
```

### Comparing `jaanca_utils_os-0.0.1rc6/jaanca_utils_os/__init__.py` & `jaanca_utils_os-0.0.1rc7/jaanca_utils_os/__init__.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/helpers/environment_parser_loader.py` & `jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/helpers/environment_parser_loader.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/helpers/file_folder_management.py` & `jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/helpers/file_folder_management.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/helpers/file_properties.py` & `jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/helpers/file_properties.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/helpers/parse_bool.py` & `jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/helpers/parse_bool.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc6/jaanca_utils_os/utils/helpers/parse_types.py` & `jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/helpers/parse_types.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc6/jaanca_utils_os.egg-info/PKG-INFO` & `jaanca_utils_os-0.0.1rc7/jaanca_utils_os.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-utils-os
-Version: 0.0.1rc6
+Version: 0.0.1rc7
 Summary: A tool library created by jaanca with operating system help functions such as reading environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: datetime,utc
 Classifier: Development Status :: 4 - Beta
@@ -22,14 +22,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Provides-Extra: dotenv
+Requires-Dist: python-dotenv>=1.0.1; extra == "dotenv"
 
 <p align="center">
     <em>jaanca public libraries</em>
 </p>
 
 <p align="center">
 <a href="https://pypi.org/project/jaanca-utils-os" target="_blank">
@@ -70,14 +72,15 @@
 
 ---
 # environment_parser_loader: Example of use
 
 ```console    
 pip install prettytable==3.10.0
 pip install python-dotenv==1.0.1
+pip install jaanca_utils_os[dotenv]==0.1.0
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
-Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.0.1rc6 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.0.1rc7 Summary: A tool
 library created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com
 License: MIT License Keywords: datetime,utc Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
@@ -11,14 +11,15 @@
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Software Development Classifier: Typing :: Typed Requires-
 Python: >=3.8 Description-Content-Type: text/markdown License-File: LICENSE.txt
+Provides-Extra: dotenv Requires-Dist: python-dotenv>=1.0.1; extra == "dotenv"
                             jjaaaannccaa ppuubblliicc lliibbrraarriieess
                            _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]
 --- # A tool library created by jaanca * **Python library**: A tool library
 created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others. *
 **EnvironmentParserLoader**: A class that loads, parses, and manages system
 environment variables into various data types. General Functionality ## The
@@ -32,25 +33,26 @@
 **FileProperties**: Functionalities to read properties of an operating system
 file, such as: modification date, creation, size in bytes, among others.
 [Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca-
 utils-os) | [Package (PyPI)](https://pypi.org/project/jaanca-utils-os/) |
 [Samples](https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os/
 samples) --- # library installation ```console pip install jaanca_utils_os --
 upgrade ``` --- # environment_parser_loader: Example of use ```console pip
-install prettytable==3.10.0 pip install python-dotenv==1.0.1 ``` ### File with
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
+install prettytable==3.10.0 pip install python-dotenv==1.0.1 pip install
+jaanca_utils_os[dotenv]==0.1.0 ``` ### File with environments vars .env
+```console ENGINE_POSTGRES_CONN_HOST=psqlt ENGINE_POSTGRES_CONN_DB=test
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
```

### Comparing `jaanca_utils_os-0.0.1rc6/jaanca_utils_os.egg-info/SOURCES.txt` & `jaanca_utils_os-0.0.1rc7/jaanca_utils_os.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.cfg
 setup.py
 jaanca_utils_os/__init__.py
 jaanca_utils_os.egg-info/PKG-INFO
 jaanca_utils_os.egg-info/SOURCES.txt
 jaanca_utils_os.egg-info/dependency_links.txt
+jaanca_utils_os.egg-info/requires.txt
 jaanca_utils_os.egg-info/top_level.txt
 jaanca_utils_os/utils/__init__.py
 jaanca_utils_os/utils/helpers/__init__.py
 jaanca_utils_os/utils/helpers/environment_parser_loader.py
 jaanca_utils_os/utils/helpers/file_folder_management.py
 jaanca_utils_os/utils/helpers/file_properties.py
 jaanca_utils_os/utils/helpers/parse_bool.py
```

### Comparing `jaanca_utils_os-0.0.1rc6/setup.py` & `jaanca_utils_os-0.0.1rc7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca-utils-os"
-VERSION = "0.0.1rc6"
+VERSION = "0.0.1rc7"
 
 install_requires = [""]
+extras_require = {
+    "dotenv": "python-dotenv>=1.0.1"
+}
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'A tool library created by {COMPANY_NAME} with operating system help functions such as reading environment variables, reading/writing files, file properties, among others.',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
@@ -35,8 +38,9 @@
         "Topic :: System :: Monitoring",
         "Topic :: Software Development",
         "Typing :: Typed",
     ],
     packages=find_packages(),
     python_requires=">=3.8",
     install_requires=install_requires,
+    extras_require=extras_require,
 )
```

