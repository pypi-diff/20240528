# Comparing `tmp/jaanca_utils_os-0.0.1rc4.tar.gz` & `tmp/jaanca_utils_os-0.0.1rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca_utils_os-0.0.1rc4.tar", last modified: Mon May 27 21:26:36 2024, max compression
+gzip compressed data, was "jaanca_utils_os-0.0.1rc5.tar", last modified: Mon May 27 21:28:24 2024, max compression
```

## Comparing `jaanca_utils_os-0.0.1rc4.tar` & `jaanca_utils_os-0.0.1rc5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 21:26:36.558267 jaanca_utils_os-0.0.1rc4/
--rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc4/LICENSE.txt
--rw-rw-rw-   0        0        0     3980 2024-05-27 21:26:36.557267 jaanca_utils_os-0.0.1rc4/PKG-INFO
--rw-rw-rw-   0        0        0     2655 2024-05-27 20:05:31.000000 jaanca_utils_os-0.0.1rc4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 21:26:36.531266 jaanca_utils_os-0.0.1rc4/jaanca_utils_os/
--rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.0.1rc4/jaanca_utils_os/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 21:26:36.541270 jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 21:26:36.552269 jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     2145 2024-05-27 20:38:54.000000 jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/helpers/environment_parser_loader.py
--rw-rw-rw-   0        0        0     6786 2024-05-27 21:23:44.000000 jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/helpers/file_folder_management.py
--rw-rw-rw-   0        0        0     3213 2024-05-27 19:49:12.000000 jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/helpers/file_properties.py
--rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/helpers/parse_bool.py
--rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/helpers/parse_types.py
-drwxrwxrwx   0        0        0        0 2024-05-27 21:26:36.556268 jaanca_utils_os-0.0.1rc4/jaanca_utils_os.egg-info/
--rw-rw-rw-   0        0        0     3980 2024-05-27 21:26:36.000000 jaanca_utils_os-0.0.1rc4/jaanca_utils_os.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2024-05-27 21:26:36.000000 jaanca_utils_os-0.0.1rc4/jaanca_utils_os.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 21:26:36.000000 jaanca_utils_os-0.0.1rc4/jaanca_utils_os.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-27 21:26:36.000000 jaanca_utils_os-0.0.1rc4/jaanca_utils_os.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 21:26:36.559267 jaanca_utils_os-0.0.1rc4/setup.cfg
--rw-rw-rw-   0        0        0     1662 2024-05-27 21:26:29.000000 jaanca_utils_os-0.0.1rc4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 21:28:24.359658 jaanca_utils_os-0.0.1rc5/
+-rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc5/LICENSE.txt
+-rw-rw-rw-   0        0        0     3980 2024-05-27 21:28:24.359658 jaanca_utils_os-0.0.1rc5/PKG-INFO
+-rw-rw-rw-   0        0        0     2655 2024-05-27 20:05:31.000000 jaanca_utils_os-0.0.1rc5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 21:28:24.333657 jaanca_utils_os-0.0.1rc5/jaanca_utils_os/
+-rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.0.1rc5/jaanca_utils_os/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 21:28:24.344658 jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 21:28:24.355659 jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     2130 2024-05-27 21:28:03.000000 jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/helpers/environment_parser_loader.py
+-rw-rw-rw-   0        0        0     6786 2024-05-27 21:23:44.000000 jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/helpers/file_folder_management.py
+-rw-rw-rw-   0        0        0     3213 2024-05-27 19:49:12.000000 jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/helpers/file_properties.py
+-rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/helpers/parse_bool.py
+-rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/helpers/parse_types.py
+drwxrwxrwx   0        0        0        0 2024-05-27 21:28:24.357660 jaanca_utils_os-0.0.1rc5/jaanca_utils_os.egg-info/
+-rw-rw-rw-   0        0        0     3980 2024-05-27 21:28:24.000000 jaanca_utils_os-0.0.1rc5/jaanca_utils_os.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2024-05-27 21:28:24.000000 jaanca_utils_os-0.0.1rc5/jaanca_utils_os.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 21:28:24.000000 jaanca_utils_os-0.0.1rc5/jaanca_utils_os.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-27 21:28:24.000000 jaanca_utils_os-0.0.1rc5/jaanca_utils_os.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 21:28:24.361658 jaanca_utils_os-0.0.1rc5/setup.cfg
+-rw-rw-rw-   0        0        0     1662 2024-05-27 21:28:14.000000 jaanca_utils_os-0.0.1rc5/setup.py
```

### Comparing `jaanca_utils_os-0.0.1rc4/LICENSE.txt` & `jaanca_utils_os-0.0.1rc5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc4/PKG-INFO` & `jaanca_utils_os-0.0.1rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-utils-os
-Version: 0.0.1rc4
+Version: 0.0.1rc5
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
-Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.0.1rc4 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.0.1rc5 Summary: A tool
 library created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com
 License: MIT License Keywords: datetime,utc Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
```

### Comparing `jaanca_utils_os-0.0.1rc4/README.md` & `jaanca_utils_os-0.0.1rc5/README.md`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc4/jaanca_utils_os/__init__.py` & `jaanca_utils_os-0.0.1rc5/jaanca_utils_os/__init__.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/helpers/environment_parser_loader.py` & `jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/helpers/environment_parser_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,17 +21,16 @@
 
     ## The EnvironmentParserLoader class would be designed to:
     - Read the system’s environment variables.
     - Parse (convert) these variables into specific data types (such as int, float, bool, str, list, dict).
     - Manage and provide centralized methods to access these environment variables in a typed and secure manner.
     - If the environment variable does not exist or has a value of None and a default value is not assigned, a KeyError exception will be returned.
     '''
-    def __init__(self,cls):
-        env_path= Path('.') / '.env'
-        load_dotenv(dotenv_path=env_path)
+    def __init__(self,cls,env_full_path:str):
+        load_dotenv(dotenv_path=env_full_path)
         for key, value in vars(cls).items():
             if not key.startswith('__'):
                 default_value = None
                 if isinstance(value,tuple) or isinstance(value,list):
                     default_value=value[1]
                     value=value[0]
                 env_data=parse_types(os.getenv(value,default_value))
```

### Comparing `jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/helpers/file_folder_management.py` & `jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/helpers/file_folder_management.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/helpers/file_properties.py` & `jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/helpers/file_properties.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/helpers/parse_bool.py` & `jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/helpers/parse_bool.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc4/jaanca_utils_os/utils/helpers/parse_types.py` & `jaanca_utils_os-0.0.1rc5/jaanca_utils_os/utils/helpers/parse_types.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc4/jaanca_utils_os.egg-info/PKG-INFO` & `jaanca_utils_os-0.0.1rc5/jaanca_utils_os.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-utils-os
-Version: 0.0.1rc4
+Version: 0.0.1rc5
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
-Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.0.1rc4 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.0.1rc5 Summary: A tool
 library created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com
 License: MIT License Keywords: datetime,utc Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
```

### Comparing `jaanca_utils_os-0.0.1rc4/jaanca_utils_os.egg-info/SOURCES.txt` & `jaanca_utils_os-0.0.1rc5/jaanca_utils_os.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc4/setup.py` & `jaanca_utils_os-0.0.1rc5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca-utils-os"
-VERSION = "0.0.1rc4"
+VERSION = "0.0.1rc5"
 
 install_requires = [""]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'A tool library created by {COMPANY_NAME} with operating system help functions such as reading environment variables, reading/writing files, file properties, among others.',
```

