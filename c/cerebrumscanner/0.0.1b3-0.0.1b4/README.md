# Comparing `tmp/cerebrumscanner-0.0.1b3.tar.gz` & `tmp/cerebrumscanner-0.0.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrumscanner-0.0.1b3.tar", last modified: Tue May 28 05:59:39 2024, max compression
+gzip compressed data, was "cerebrumscanner-0.0.1b4.tar", last modified: Tue May 28 06:05:14 2024, max compression
```

## Comparing `cerebrumscanner-0.0.1b3.tar` & `cerebrumscanner-0.0.1b4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 05:59:39.969767 cerebrumscanner-0.0.1b3/
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       63 2024-05-27 08:15:33.000000 cerebrumscanner-0.0.1b3/LICENSE
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       24 2024-05-27 09:23:20.000000 cerebrumscanner-0.0.1b3/MANIFEST.in
--rw-r--r--   0 nekodu-01  (1000) nekodu-01  (1000)     6618 2024-05-28 05:59:39.969767 cerebrumscanner-0.0.1b3/PKG-INFO
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)     6239 2024-05-27 08:02:00.000000 cerebrumscanner-0.0.1b3/README.md
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        6 2024-05-27 09:20:05.000000 cerebrumscanner-0.0.1b3/requirements.txt
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       38 2024-05-28 05:59:39.969767 cerebrumscanner-0.0.1b3/setup.cfg
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)      976 2024-05-28 05:58:17.000000 cerebrumscanner-0.0.1b3/setup.py
-drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 05:59:39.969767 cerebrumscanner-0.0.1b3/src/
-drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 05:59:39.969767 cerebrumscanner-0.0.1b3/src/cerebrumscanner/
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-27 08:46:33.000000 cerebrumscanner-0.0.1b3/src/cerebrumscanner/__init__.py
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       87 2024-05-27 08:46:58.000000 cerebrumscanner-0.0.1b3/src/cerebrumscanner/dummy_module3.py
-drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 05:59:39.969767 cerebrumscanner-0.0.1b3/src/cerebrumscanner/lib/
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       87 2024-05-27 08:23:20.000000 cerebrumscanner-0.0.1b3/src/cerebrumscanner/lib/dummy_module2.py
-drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 05:59:39.969767 cerebrumscanner-0.0.1b3/src/cerebrumscanner.egg-info/
--rw-r--r--   0 nekodu-01  (1000) nekodu-01  (1000)     6618 2024-05-28 05:59:39.000000 cerebrumscanner-0.0.1b3/src/cerebrumscanner.egg-info/PKG-INFO
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)      434 2024-05-28 05:59:39.000000 cerebrumscanner-0.0.1b3/src/cerebrumscanner.egg-info/SOURCES.txt
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        1 2024-05-28 05:59:39.000000 cerebrumscanner-0.0.1b3/src/cerebrumscanner.egg-info/dependency_links.txt
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        1 2024-05-28 05:59:39.000000 cerebrumscanner-0.0.1b3/src/cerebrumscanner.egg-info/not-zip-safe
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        7 2024-05-28 05:59:39.000000 cerebrumscanner-0.0.1b3/src/cerebrumscanner.egg-info/requires.txt
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       16 2024-05-28 05:59:39.000000 cerebrumscanner-0.0.1b3/src/cerebrumscanner.egg-info/top_level.txt
-drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 05:59:39.969767 cerebrumscanner-0.0.1b3/test/
--rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       59 2024-05-27 08:09:56.000000 cerebrumscanner-0.0.1b3/test/test.py
+drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 06:05:14.707198 cerebrumscanner-0.0.1b4/
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       63 2024-05-27 08:15:33.000000 cerebrumscanner-0.0.1b4/LICENSE
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       24 2024-05-27 09:23:20.000000 cerebrumscanner-0.0.1b4/MANIFEST.in
+-rw-r--r--   0 nekodu-01  (1000) nekodu-01  (1000)     6618 2024-05-28 06:05:14.707198 cerebrumscanner-0.0.1b4/PKG-INFO
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)     6239 2024-05-27 08:02:00.000000 cerebrumscanner-0.0.1b4/README.md
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        6 2024-05-27 09:20:05.000000 cerebrumscanner-0.0.1b4/requirements.txt
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       38 2024-05-28 06:05:14.707198 cerebrumscanner-0.0.1b4/setup.cfg
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)      976 2024-05-28 06:05:02.000000 cerebrumscanner-0.0.1b4/setup.py
+drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 06:05:14.703199 cerebrumscanner-0.0.1b4/src/
+drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 06:05:14.703199 cerebrumscanner-0.0.1b4/src/cerebrumscanner/
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-27 08:46:33.000000 cerebrumscanner-0.0.1b4/src/cerebrumscanner/__init__.py
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       87 2024-05-27 08:46:58.000000 cerebrumscanner-0.0.1b4/src/cerebrumscanner/dummy_module3.py
+drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 06:05:14.707198 cerebrumscanner-0.0.1b4/src/cerebrumscanner/lib/
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-27 08:46:33.000000 cerebrumscanner-0.0.1b4/src/cerebrumscanner/lib/__init__.py
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       87 2024-05-27 08:23:20.000000 cerebrumscanner-0.0.1b4/src/cerebrumscanner/lib/dummy_module2.py
+drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 06:05:14.707198 cerebrumscanner-0.0.1b4/src/cerebrumscanner.egg-info/
+-rw-r--r--   0 nekodu-01  (1000) nekodu-01  (1000)     6618 2024-05-28 06:05:14.000000 cerebrumscanner-0.0.1b4/src/cerebrumscanner.egg-info/PKG-INFO
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)      470 2024-05-28 06:05:14.000000 cerebrumscanner-0.0.1b4/src/cerebrumscanner.egg-info/SOURCES.txt
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        1 2024-05-28 06:05:14.000000 cerebrumscanner-0.0.1b4/src/cerebrumscanner.egg-info/dependency_links.txt
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        1 2024-05-28 06:05:14.000000 cerebrumscanner-0.0.1b4/src/cerebrumscanner.egg-info/not-zip-safe
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        7 2024-05-28 06:05:14.000000 cerebrumscanner-0.0.1b4/src/cerebrumscanner.egg-info/requires.txt
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       16 2024-05-28 06:05:14.000000 cerebrumscanner-0.0.1b4/src/cerebrumscanner.egg-info/top_level.txt
+drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 06:05:14.707198 cerebrumscanner-0.0.1b4/test/
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       59 2024-05-27 08:09:56.000000 cerebrumscanner-0.0.1b4/test/test.py
```

### Comparing `cerebrumscanner-0.0.1b3/PKG-INFO` & `cerebrumscanner-0.0.1b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrumscanner
-Version: 0.0.1b3
+Version: 0.0.1b4
 Summary: Cerebrum Scanner Project
 Home-page: https://gitlab.com/nekodu/cerebrumscanner/cerebrum-scanner
 Author: Nekodu Technology
 Author-email: info@nekodu.com
 License: Nekodu Technology Inc - © Copyright 2023. All Rights Reserved.
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cerebrumscanner-0.0.1b3/README.md` & `cerebrumscanner-0.0.1b4/README.md`

 * *Files identical despite different names*

### Comparing `cerebrumscanner-0.0.1b3/setup.py` & `cerebrumscanner-0.0.1b4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ) as readme_file, open("requirements.txt", encoding="utf-8") as requirements_file:
     package_license = license_file.read()
     long_description = readme_file.read()
     install_requires = requirements_file.read().split("\n")[0:]
 
 setup(
     name="cerebrumscanner",
-    version="0.0.1.b3",
+    version="0.0.1.b4",
     url="https://gitlab.com/nekodu/cerebrumscanner/cerebrum-scanner",
     license=package_license,
     author="Nekodu Technology",
     author_email="info@nekodu.com",
     description=(
         "Cerebrum Scanner Project"
     ),
```

### Comparing `cerebrumscanner-0.0.1b3/src/cerebrumscanner.egg-info/PKG-INFO` & `cerebrumscanner-0.0.1b4/src/cerebrumscanner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrumscanner
-Version: 0.0.1b3
+Version: 0.0.1b4
 Summary: Cerebrum Scanner Project
 Home-page: https://gitlab.com/nekodu/cerebrumscanner/cerebrum-scanner
 Author: Nekodu Technology
 Author-email: info@nekodu.com
 License: Nekodu Technology Inc - © Copyright 2023. All Rights Reserved.
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

