# Comparing `tmp/cerebrumscanner-0.0.1b1.tar.gz` & `tmp/cerebrumscanner-0.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrumscanner-0.0.1b1.tar", last modified: Tue May 28 05:30:47 2024, max compression
+gzip compressed data, was "cerebrumscanner-0.0.1b2.tar", last modified: Tue May 28 05:44:06 2024, max compression
```

## Comparing `cerebrumscanner-0.0.1b1.tar` & `cerebrumscanner-0.0.1b2.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 05:30:47.329984 cerebrumscanner-0.0.1b1/
--rw-rw-rw-   0        0        0    35823 2023-09-10 19:28:05.000000 cerebrumscanner-0.0.1b1/LICENSE
--rw-rw-rw-   0        0        0       24 2024-05-27 12:55:40.000000 cerebrumscanner-0.0.1b1/MANIFEST.in
--rw-rw-rw-   0        0        0    45314 2024-05-28 05:30:47.328983 cerebrumscanner-0.0.1b1/PKG-INFO
--rw-rw-rw-   0        0        0     3382 2024-02-21 06:32:05.000000 cerebrumscanner-0.0.1b1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 05:30:47.286250 cerebrumscanner-0.0.1b1/cerebrumscanner/
-drwxrwxrwx   0        0        0        0 2024-05-28 05:30:47.318466 cerebrumscanner-0.0.1b1/cerebrumscanner/cerebrumscanner.egg-info/
--rw-rw-rw-   0        0        0    45314 2024-05-28 05:30:47.000000 cerebrumscanner-0.0.1b1/cerebrumscanner/cerebrumscanner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      557 2024-05-28 05:30:47.000000 cerebrumscanner-0.0.1b1/cerebrumscanner/cerebrumscanner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 05:30:47.000000 cerebrumscanner-0.0.1b1/cerebrumscanner/cerebrumscanner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-28 05:30:47.000000 cerebrumscanner-0.0.1b1/cerebrumscanner/cerebrumscanner.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      172 2024-05-28 05:30:47.000000 cerebrumscanner-0.0.1b1/cerebrumscanner/cerebrumscanner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       46 2024-05-28 05:30:47.000000 cerebrumscanner-0.0.1b1/cerebrumscanner/cerebrumscanner.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-28 05:30:47.320440 cerebrumscanner-0.0.1b1/cerebrumscanner/configs/
--rw-rw-rw-   0        0        0    11498 2023-07-18 14:52:05.000000 cerebrumscanner-0.0.1b1/cerebrumscanner/configs/resnet50_classification_hemorrhage.py
-drwxrwxrwx   0        0        0        0 2024-05-28 05:30:47.325985 cerebrumscanner-0.0.1b1/cerebrumscanner/lib/
--rw-rw-rw-   0        0        0     5663 2024-05-06 13:47:03.000000 cerebrumscanner-0.0.1b1/cerebrumscanner/lib/database_manager.py
--rw-rw-rw-   0        0        0     1460 2024-05-07 07:27:54.000000 cerebrumscanner-0.0.1b1/cerebrumscanner/lib/image_processor.py
--rw-rw-rw-   0        0        0     3370 2023-08-01 10:12:18.000000 cerebrumscanner-0.0.1b1/cerebrumscanner/lib/processor.py
--rw-rw-rw-   0        0        0      206 2024-04-16 10:48:57.000000 cerebrumscanner-0.0.1b1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 05:30:47.329984 cerebrumscanner-0.0.1b1/setup.cfg
--rw-rw-rw-   0        0        0     1030 2024-05-28 05:29:52.000000 cerebrumscanner-0.0.1b1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 05:44:06.579619 cerebrumscanner-0.0.1b2/
+-rw-rw-rw-   0        0        0    35823 2023-09-10 19:28:05.000000 cerebrumscanner-0.0.1b2/LICENSE
+-rw-rw-rw-   0        0        0       24 2024-05-27 12:55:40.000000 cerebrumscanner-0.0.1b2/MANIFEST.in
+-rw-rw-rw-   0        0        0    45314 2024-05-28 05:44:06.578620 cerebrumscanner-0.0.1b2/PKG-INFO
+-rw-rw-rw-   0        0        0     3382 2024-02-21 06:32:05.000000 cerebrumscanner-0.0.1b2/README.md
+-rw-rw-rw-   0        0        0      206 2024-04-16 10:48:57.000000 cerebrumscanner-0.0.1b2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 05:44:06.579619 cerebrumscanner-0.0.1b2/setup.cfg
+-rw-rw-rw-   0        0        0     1006 2024-05-28 05:43:14.000000 cerebrumscanner-0.0.1b2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 05:44:06.522948 cerebrumscanner-0.0.1b2/src/
+drwxrwxrwx   0        0        0        0 2024-05-28 05:44:06.533459 cerebrumscanner-0.0.1b2/src/cerebrumscanner/
+-rw-rw-rw-   0        0        0        0 2024-05-27 12:45:46.000000 cerebrumscanner-0.0.1b2/src/cerebrumscanner/__init__.py
+-rw-rw-rw-   0        0        0     1742 2024-05-06 13:46:43.000000 cerebrumscanner-0.0.1b2/src/cerebrumscanner/_global_paths.py
+drwxrwxrwx   0        0        0        0 2024-05-28 05:44:06.571600 cerebrumscanner-0.0.1b2/src/cerebrumscanner/configs/
+-rw-rw-rw-   0        0        0    11498 2023-07-18 14:52:05.000000 cerebrumscanner-0.0.1b2/src/cerebrumscanner/configs/resnet50_classification_hemorrhage.py
+drwxrwxrwx   0        0        0        0 2024-05-28 05:44:06.576622 cerebrumscanner-0.0.1b2/src/cerebrumscanner/lib/
+-rw-rw-rw-   0        0        0     5663 2024-05-06 13:47:03.000000 cerebrumscanner-0.0.1b2/src/cerebrumscanner/lib/database_manager.py
+-rw-rw-rw-   0        0        0     1460 2024-05-07 07:27:54.000000 cerebrumscanner-0.0.1b2/src/cerebrumscanner/lib/image_processor.py
+-rw-rw-rw-   0        0        0     3370 2023-08-01 10:12:18.000000 cerebrumscanner-0.0.1b2/src/cerebrumscanner/lib/processor.py
+drwxrwxrwx   0        0        0        0 2024-05-28 05:44:06.568094 cerebrumscanner-0.0.1b2/src/cerebrumscanner.egg-info/
+-rw-rw-rw-   0        0        0    45314 2024-05-28 05:44:06.000000 cerebrumscanner-0.0.1b2/src/cerebrumscanner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      570 2024-05-28 05:44:06.000000 cerebrumscanner-0.0.1b2/src/cerebrumscanner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 05:44:06.000000 cerebrumscanner-0.0.1b2/src/cerebrumscanner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-28 05:44:06.000000 cerebrumscanner-0.0.1b2/src/cerebrumscanner.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      172 2024-05-28 05:44:06.000000 cerebrumscanner-0.0.1b2/src/cerebrumscanner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-28 05:44:06.000000 cerebrumscanner-0.0.1b2/src/cerebrumscanner.egg-info/top_level.txt
```

### Comparing `cerebrumscanner-0.0.1b1/LICENSE` & `cerebrumscanner-0.0.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrumscanner-0.0.1b1/PKG-INFO` & `cerebrumscanner-0.0.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrumscanner
-Version: 0.0.1b1
+Version: 0.0.1b2
 Summary: Cerebrum Scanner Project
 Home-page: https://gitlab.com/nekodu/cerebrumscanner/cerebrum-scanner
 Author: Nekodu Technology
 Author-email: info@nekodu.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `cerebrumscanner-0.0.1b1/README.md` & `cerebrumscanner-0.0.1b2/README.md`

 * *Files identical despite different names*

### Comparing `cerebrumscanner-0.0.1b1/cerebrumscanner/cerebrumscanner.egg-info/PKG-INFO` & `cerebrumscanner-0.0.1b2/src/cerebrumscanner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrumscanner
-Version: 0.0.1b1
+Version: 0.0.1b2
 Summary: Cerebrum Scanner Project
 Home-page: https://gitlab.com/nekodu/cerebrumscanner/cerebrum-scanner
 Author: Nekodu Technology
 Author-email: info@nekodu.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `cerebrumscanner-0.0.1b1/cerebrumscanner/cerebrumscanner.egg-info/SOURCES.txt` & `cerebrumscanner-0.0.1b2/src/cerebrumscanner.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
-cerebrumscanner/cerebrumscanner.egg-info/PKG-INFO
-cerebrumscanner/cerebrumscanner.egg-info/SOURCES.txt
-cerebrumscanner/cerebrumscanner.egg-info/dependency_links.txt
-cerebrumscanner/cerebrumscanner.egg-info/not-zip-safe
-cerebrumscanner/cerebrumscanner.egg-info/requires.txt
-cerebrumscanner/cerebrumscanner.egg-info/top_level.txt
-cerebrumscanner/configs/resnet50_classification_hemorrhage.py
-cerebrumscanner/lib/database_manager.py
-cerebrumscanner/lib/image_processor.py
-cerebrumscanner/lib/processor.py
+src/cerebrumscanner/__init__.py
+src/cerebrumscanner/_global_paths.py
+src/cerebrumscanner.egg-info/PKG-INFO
+src/cerebrumscanner.egg-info/SOURCES.txt
+src/cerebrumscanner.egg-info/dependency_links.txt
+src/cerebrumscanner.egg-info/not-zip-safe
+src/cerebrumscanner.egg-info/requires.txt
+src/cerebrumscanner.egg-info/top_level.txt
+src/cerebrumscanner/configs/resnet50_classification_hemorrhage.py
+src/cerebrumscanner/lib/database_manager.py
+src/cerebrumscanner/lib/image_processor.py
+src/cerebrumscanner/lib/processor.py
```

### Comparing `cerebrumscanner-0.0.1b1/cerebrumscanner/configs/resnet50_classification_hemorrhage.py` & `cerebrumscanner-0.0.1b2/src/cerebrumscanner/configs/resnet50_classification_hemorrhage.py`

 * *Files identical despite different names*

### Comparing `cerebrumscanner-0.0.1b1/cerebrumscanner/lib/database_manager.py` & `cerebrumscanner-0.0.1b2/src/cerebrumscanner/lib/database_manager.py`

 * *Files identical despite different names*

### Comparing `cerebrumscanner-0.0.1b1/cerebrumscanner/lib/image_processor.py` & `cerebrumscanner-0.0.1b2/src/cerebrumscanner/lib/image_processor.py`

 * *Files identical despite different names*

### Comparing `cerebrumscanner-0.0.1b1/cerebrumscanner/lib/processor.py` & `cerebrumscanner-0.0.1b2/src/cerebrumscanner/lib/processor.py`

 * *Files identical despite different names*

### Comparing `cerebrumscanner-0.0.1b1/setup.py` & `cerebrumscanner-0.0.1b2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 ) as readme_file, open("requirements.txt", encoding="utf-8") as requirements_file:
     package_license = license_file.read()
     long_description = readme_file.read()
     install_requires = requirements_file.read().split("\n")[0:]
 
 setup(
     name="cerebrumscanner",
-    version="0.0.1.b1",
+    version="0.0.1.b2",
     url="https://gitlab.com/nekodu/cerebrumscanner/cerebrum-scanner",
     license=package_license,
     author="Nekodu Technology",
     author_email="info@nekodu.com",
     description=(
         "Cerebrum Scanner Project"
     ),
-    package_dir={"": "cerebrumscanner"},
-    packages=find_namespace_packages(where="cerebrumscanner"),
+    package_dir={"": "src"},
+    packages=find_namespace_packages(where="src"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=install_requires,
     zip_safe=False,
 )
```

