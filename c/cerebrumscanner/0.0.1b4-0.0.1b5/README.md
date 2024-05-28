# Comparing `tmp/cerebrumscanner-0.0.1b4.tar.gz` & `tmp/cerebrumscanner-0.0.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrumscanner-0.0.1b4.tar", last modified: Tue May 28 06:05:14 2024, max compression
+gzip compressed data, was "cerebrumscanner-0.0.1b5.tar", last modified: Tue May 28 06:25:36 2024, max compression
```

## Comparing `cerebrumscanner-0.0.1b4.tar` & `cerebrumscanner-0.0.1b5.tar`

### file list

```diff
@@ -1,24 +1,17 @@
-drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 06:05:14.707198 cerebrumscanner-0.0.1b4/
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       63 2024-05-27 08:15:33.000000 cerebrumscanner-0.0.1b4/LICENSE
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       24 2024-05-27 09:23:20.000000 cerebrumscanner-0.0.1b4/MANIFEST.in
--rw-r--r--   0 nekodu-01  (1000) nekodu-01  (1000)     6618 2024-05-28 06:05:14.707198 cerebrumscanner-0.0.1b4/PKG-INFO
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)     6239 2024-05-27 08:02:00.000000 cerebrumscanner-0.0.1b4/README.md
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        6 2024-05-27 09:20:05.000000 cerebrumscanner-0.0.1b4/requirements.txt
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       38 2024-05-28 06:05:14.707198 cerebrumscanner-0.0.1b4/setup.cfg
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)      976 2024-05-28 06:05:02.000000 cerebrumscanner-0.0.1b4/setup.py
-drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 06:05:14.703199 cerebrumscanner-0.0.1b4/src/
-drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 06:05:14.703199 cerebrumscanner-0.0.1b4/src/cerebrumscanner/
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-27 08:46:33.000000 cerebrumscanner-0.0.1b4/src/cerebrumscanner/__init__.py
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       87 2024-05-27 08:46:58.000000 cerebrumscanner-0.0.1b4/src/cerebrumscanner/dummy_module3.py
-drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 06:05:14.707198 cerebrumscanner-0.0.1b4/src/cerebrumscanner/lib/
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-27 08:46:33.000000 cerebrumscanner-0.0.1b4/src/cerebrumscanner/lib/__init__.py
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       87 2024-05-27 08:23:20.000000 cerebrumscanner-0.0.1b4/src/cerebrumscanner/lib/dummy_module2.py
-drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 06:05:14.707198 cerebrumscanner-0.0.1b4/src/cerebrumscanner.egg-info/
--rw-r--r--   0 nekodu-01  (1000) nekodu-01  (1000)     6618 2024-05-28 06:05:14.000000 cerebrumscanner-0.0.1b4/src/cerebrumscanner.egg-info/PKG-INFO
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)      470 2024-05-28 06:05:14.000000 cerebrumscanner-0.0.1b4/src/cerebrumscanner.egg-info/SOURCES.txt
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        1 2024-05-28 06:05:14.000000 cerebrumscanner-0.0.1b4/src/cerebrumscanner.egg-info/dependency_links.txt
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        1 2024-05-28 06:05:14.000000 cerebrumscanner-0.0.1b4/src/cerebrumscanner.egg-info/not-zip-safe
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        7 2024-05-28 06:05:14.000000 cerebrumscanner-0.0.1b4/src/cerebrumscanner.egg-info/requires.txt
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       16 2024-05-28 06:05:14.000000 cerebrumscanner-0.0.1b4/src/cerebrumscanner.egg-info/top_level.txt
-drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 06:05:14.707198 cerebrumscanner-0.0.1b4/test/
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       59 2024-05-27 08:09:56.000000 cerebrumscanner-0.0.1b4/test/test.py
+drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 06:25:36.090840 cerebrumscanner-0.0.1b5/
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       63 2024-05-27 08:15:33.000000 cerebrumscanner-0.0.1b5/LICENSE
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       24 2024-05-27 09:23:20.000000 cerebrumscanner-0.0.1b5/MANIFEST.in
+-rw-r--r--   0 nekodu-01  (1000) nekodu-01  (1000)     6618 2024-05-28 06:25:36.090840 cerebrumscanner-0.0.1b5/PKG-INFO
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)     6239 2024-05-27 08:02:00.000000 cerebrumscanner-0.0.1b5/README.md
+drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 06:25:36.090840 cerebrumscanner-0.0.1b5/cerebrumscanner.egg-info/
+-rw-r--r--   0 nekodu-01  (1000) nekodu-01  (1000)     6618 2024-05-28 06:25:36.000000 cerebrumscanner-0.0.1b5/cerebrumscanner.egg-info/PKG-INFO
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)      300 2024-05-28 06:25:36.000000 cerebrumscanner-0.0.1b5/cerebrumscanner.egg-info/SOURCES.txt
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        1 2024-05-28 06:25:36.000000 cerebrumscanner-0.0.1b5/cerebrumscanner.egg-info/dependency_links.txt
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        1 2024-05-28 06:25:36.000000 cerebrumscanner-0.0.1b5/cerebrumscanner.egg-info/not-zip-safe
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        7 2024-05-28 06:25:36.000000 cerebrumscanner-0.0.1b5/cerebrumscanner.egg-info/requires.txt
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        1 2024-05-28 06:25:36.000000 cerebrumscanner-0.0.1b5/cerebrumscanner.egg-info/top_level.txt
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        6 2024-05-27 09:20:05.000000 cerebrumscanner-0.0.1b5/requirements.txt
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       38 2024-05-28 06:25:36.090840 cerebrumscanner-0.0.1b5/setup.cfg
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)      941 2024-05-28 06:24:28.000000 cerebrumscanner-0.0.1b5/setup.py
+drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 06:25:36.090840 cerebrumscanner-0.0.1b5/test/
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       59 2024-05-27 08:09:56.000000 cerebrumscanner-0.0.1b5/test/test.py
```

### Comparing `cerebrumscanner-0.0.1b4/PKG-INFO` & `cerebrumscanner-0.0.1b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrumscanner
-Version: 0.0.1b4
+Version: 0.0.1b5
 Summary: Cerebrum Scanner Project
 Home-page: https://gitlab.com/nekodu/cerebrumscanner/cerebrum-scanner
 Author: Nekodu Technology
 Author-email: info@nekodu.com
 License: Nekodu Technology Inc - © Copyright 2023. All Rights Reserved.
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cerebrumscanner-0.0.1b4/README.md` & `cerebrumscanner-0.0.1b5/README.md`

 * *Files identical despite different names*

### Comparing `cerebrumscanner-0.0.1b4/setup.py` & `cerebrumscanner-0.0.1b5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-from setuptools import find_namespace_packages, setup
+from setuptools import find_namespace_packages, find_packages, setup
 
 package_license: str = ""
 long_description: str = ""
 install_requires = []
 
 with open("LICENSE", encoding="utf-8") as license_file, open(
     "README.md", encoding="utf-8"
 ) as readme_file, open("requirements.txt", encoding="utf-8") as requirements_file:
     package_license = license_file.read()
     long_description = readme_file.read()
     install_requires = requirements_file.read().split("\n")[0:]
 
 setup(
     name="cerebrumscanner",
-    version="0.0.1.b4",
+    version="0.0.1.b5",
     url="https://gitlab.com/nekodu/cerebrumscanner/cerebrum-scanner",
     license=package_license,
     author="Nekodu Technology",
     author_email="info@nekodu.com",
     description=(
         "Cerebrum Scanner Project"
     ),
-    package_dir={"": "src"},
-    packages=find_namespace_packages(where="src"),
+    packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=install_requires,
     zip_safe=False,
 )
```

### Comparing `cerebrumscanner-0.0.1b4/src/cerebrumscanner.egg-info/PKG-INFO` & `cerebrumscanner-0.0.1b5/cerebrumscanner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrumscanner
-Version: 0.0.1b4
+Version: 0.0.1b5
 Summary: Cerebrum Scanner Project
 Home-page: https://gitlab.com/nekodu/cerebrumscanner/cerebrum-scanner
 Author: Nekodu Technology
 Author-email: info@nekodu.com
 License: Nekodu Technology Inc - © Copyright 2023. All Rights Reserved.
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

