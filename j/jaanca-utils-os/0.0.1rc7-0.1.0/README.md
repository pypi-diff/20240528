# Comparing `tmp/jaanca_utils_os-0.0.1rc7.tar.gz` & `tmp/jaanca_utils_os-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca_utils_os-0.0.1rc7.tar", last modified: Mon May 27 22:17:33 2024, max compression
+gzip compressed data, was "jaanca_utils_os-0.1.0.tar", last modified: Mon May 27 22:22:43 2024, max compression
```

## Comparing `jaanca_utils_os-0.0.1rc7.tar` & `jaanca_utils_os-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 22:17:33.015960 jaanca_utils_os-0.0.1rc7/
--rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc7/LICENSE.txt
--rw-rw-rw-   0        0        0    10229 2024-05-27 22:17:33.014959 jaanca_utils_os-0.0.1rc7/PKG-INFO
--rw-rw-rw-   0        0        0     8819 2024-05-27 22:17:09.000000 jaanca_utils_os-0.0.1rc7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 22:17:32.987960 jaanca_utils_os-0.0.1rc7/jaanca_utils_os/
--rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 22:17:32.999962 jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 22:17:33.010959 jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     4699 2024-05-27 21:37:19.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/helpers/environment_parser_loader.py
--rw-rw-rw-   0        0        0     6835 2024-05-27 22:01:52.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/helpers/file_folder_management.py
--rw-rw-rw-   0        0        0     3289 2024-05-27 22:09:16.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/helpers/file_properties.py
--rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/helpers/parse_bool.py
--rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/helpers/parse_types.py
-drwxrwxrwx   0        0        0        0 2024-05-27 22:17:33.012962 jaanca_utils_os-0.0.1rc7/jaanca_utils_os.egg-info/
--rw-rw-rw-   0        0        0    10229 2024-05-27 22:17:32.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      591 2024-05-27 22:17:32.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 22:17:32.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-27 22:17:32.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-27 22:17:32.000000 jaanca_utils_os-0.0.1rc7/jaanca_utils_os.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 22:17:33.016960 jaanca_utils_os-0.0.1rc7/setup.cfg
--rw-rw-rw-   0        0        0     1759 2024-05-27 22:17:27.000000 jaanca_utils_os-0.0.1rc7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:22:43.115286 jaanca_utils_os-0.1.0/
+-rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0    10226 2024-05-27 22:22:43.115286 jaanca_utils_os-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8819 2024-05-27 22:17:09.000000 jaanca_utils_os-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 22:22:43.088285 jaanca_utils_os-0.1.0/jaanca_utils_os/
+-rw-rw-rw-   0        0        0      575 2024-05-27 19:53:46.000000 jaanca_utils_os-0.1.0/jaanca_utils_os/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:22:43.099287 jaanca_utils_os-0.1.0/jaanca_utils_os/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.0/jaanca_utils_os/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:22:43.111286 jaanca_utils_os-0.1.0/jaanca_utils_os/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca_utils_os-0.1.0/jaanca_utils_os/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     4699 2024-05-27 21:37:19.000000 jaanca_utils_os-0.1.0/jaanca_utils_os/utils/helpers/environment_parser_loader.py
+-rw-rw-rw-   0        0        0     6835 2024-05-27 22:01:52.000000 jaanca_utils_os-0.1.0/jaanca_utils_os/utils/helpers/file_folder_management.py
+-rw-rw-rw-   0        0        0     3289 2024-05-27 22:09:16.000000 jaanca_utils_os-0.1.0/jaanca_utils_os/utils/helpers/file_properties.py
+-rw-rw-rw-   0        0        0     1083 2024-05-24 15:06:57.000000 jaanca_utils_os-0.1.0/jaanca_utils_os/utils/helpers/parse_bool.py
+-rw-rw-rw-   0        0        0     1223 2024-05-27 20:39:10.000000 jaanca_utils_os-0.1.0/jaanca_utils_os/utils/helpers/parse_types.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:22:43.113285 jaanca_utils_os-0.1.0/jaanca_utils_os.egg-info/
+-rw-rw-rw-   0        0        0    10226 2024-05-27 22:22:43.000000 jaanca_utils_os-0.1.0/jaanca_utils_os.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      591 2024-05-27 22:22:43.000000 jaanca_utils_os-0.1.0/jaanca_utils_os.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 22:22:43.000000 jaanca_utils_os-0.1.0/jaanca_utils_os.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-27 22:22:43.000000 jaanca_utils_os-0.1.0/jaanca_utils_os.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-27 22:22:43.000000 jaanca_utils_os-0.1.0/jaanca_utils_os.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 22:22:43.117285 jaanca_utils_os-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1756 2024-05-27 22:19:24.000000 jaanca_utils_os-0.1.0/setup.py
```

### Comparing `jaanca_utils_os-0.0.1rc7/LICENSE.txt` & `jaanca_utils_os-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc7/PKG-INFO` & `jaanca_utils_os-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-utils-os
-Version: 0.0.1rc7
+Version: 0.1.0
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
-Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.0.1rc7 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.0 Summary: A tool
 library created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com
 License: MIT License Keywords: datetime,utc Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
```

### Comparing `jaanca_utils_os-0.0.1rc7/README.md` & `jaanca_utils_os-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc7/jaanca_utils_os/__init__.py` & `jaanca_utils_os-0.1.0/jaanca_utils_os/__init__.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/helpers/environment_parser_loader.py` & `jaanca_utils_os-0.1.0/jaanca_utils_os/utils/helpers/environment_parser_loader.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/helpers/file_folder_management.py` & `jaanca_utils_os-0.1.0/jaanca_utils_os/utils/helpers/file_folder_management.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/helpers/file_properties.py` & `jaanca_utils_os-0.1.0/jaanca_utils_os/utils/helpers/file_properties.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/helpers/parse_bool.py` & `jaanca_utils_os-0.1.0/jaanca_utils_os/utils/helpers/parse_bool.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc7/jaanca_utils_os/utils/helpers/parse_types.py` & `jaanca_utils_os-0.1.0/jaanca_utils_os/utils/helpers/parse_types.py`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc7/jaanca_utils_os.egg-info/PKG-INFO` & `jaanca_utils_os-0.1.0/jaanca_utils_os.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-utils-os
-Version: 0.0.1rc7
+Version: 0.1.0
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
-Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.0.1rc7 Summary: A tool
+Metadata-Version: 2.1 Name: jaanca-utils-os Version: 0.1.0 Summary: A tool
 library created by jaanca with operating system help functions such as reading
 environment variables, reading/writing files, file properties, among others.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-utils-os
 Author: Jaime Andres Cardona Carrillo Author-email: jacardona@outlook.com
 License: MIT License Keywords: datetime,utc Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: System
```

### Comparing `jaanca_utils_os-0.0.1rc7/jaanca_utils_os.egg-info/SOURCES.txt` & `jaanca_utils_os-0.1.0/jaanca_utils_os.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaanca_utils_os-0.0.1rc7/setup.py` & `jaanca_utils_os-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca-utils-os"
-VERSION = "0.0.1rc7"
+VERSION = "0.1.0"
 
 install_requires = [""]
 extras_require = {
     "dotenv": "python-dotenv>=1.0.1"
 }
 
 setup(
```

