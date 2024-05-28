# Comparing `tmp/cerebrumscanner-0.0.1b2.tar.gz` & `tmp/cerebrumscanner-0.0.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrumscanner-0.0.1b2.tar", last modified: Tue May 28 05:44:06 2024, max compression
+gzip compressed data, was "cerebrumscanner-0.0.1b3.tar", last modified: Tue May 28 05:59:39 2024, max compression
```

## Comparing `cerebrumscanner-0.0.1b2.tar` & `cerebrumscanner-0.0.1b3.tar`

### file list

```diff
@@ -1,25 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 05:44:06.579619 cerebrumscanner-0.0.1b2/
--rw-rw-rw-   0        0        0    35823 2023-09-10 19:28:05.000000 cerebrumscanner-0.0.1b2/LICENSE
--rw-rw-rw-   0        0        0       24 2024-05-27 12:55:40.000000 cerebrumscanner-0.0.1b2/MANIFEST.in
--rw-rw-rw-   0        0        0    45314 2024-05-28 05:44:06.578620 cerebrumscanner-0.0.1b2/PKG-INFO
--rw-rw-rw-   0        0        0     3382 2024-02-21 06:32:05.000000 cerebrumscanner-0.0.1b2/README.md
--rw-rw-rw-   0        0        0      206 2024-04-16 10:48:57.000000 cerebrumscanner-0.0.1b2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 05:44:06.579619 cerebrumscanner-0.0.1b2/setup.cfg
--rw-rw-rw-   0        0        0     1006 2024-05-28 05:43:14.000000 cerebrumscanner-0.0.1b2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-28 05:44:06.522948 cerebrumscanner-0.0.1b2/src/
-drwxrwxrwx   0        0        0        0 2024-05-28 05:44:06.533459 cerebrumscanner-0.0.1b2/src/cerebrumscanner/
--rw-rw-rw-   0        0        0        0 2024-05-27 12:45:46.000000 cerebrumscanner-0.0.1b2/src/cerebrumscanner/__init__.py
--rw-rw-rw-   0        0        0     1742 2024-05-06 13:46:43.000000 cerebrumscanner-0.0.1b2/src/cerebrumscanner/_global_paths.py
-drwxrwxrwx   0        0        0        0 2024-05-28 05:44:06.571600 cerebrumscanner-0.0.1b2/src/cerebrumscanner/configs/
--rw-rw-rw-   0        0        0    11498 2023-07-18 14:52:05.000000 cerebrumscanner-0.0.1b2/src/cerebrumscanner/configs/resnet50_classification_hemorrhage.py
-drwxrwxrwx   0        0        0        0 2024-05-28 05:44:06.576622 cerebrumscanner-0.0.1b2/src/cerebrumscanner/lib/
--rw-rw-rw-   0        0        0     5663 2024-05-06 13:47:03.000000 cerebrumscanner-0.0.1b2/src/cerebrumscanner/lib/database_manager.py
--rw-rw-rw-   0        0        0     1460 2024-05-07 07:27:54.000000 cerebrumscanner-0.0.1b2/src/cerebrumscanner/lib/image_processor.py
--rw-rw-rw-   0        0        0     3370 2023-08-01 10:12:18.000000 cerebrumscanner-0.0.1b2/src/cerebrumscanner/lib/processor.py
-drwxrwxrwx   0        0        0        0 2024-05-28 05:44:06.568094 cerebrumscanner-0.0.1b2/src/cerebrumscanner.egg-info/
--rw-rw-rw-   0        0        0    45314 2024-05-28 05:44:06.000000 cerebrumscanner-0.0.1b2/src/cerebrumscanner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      570 2024-05-28 05:44:06.000000 cerebrumscanner-0.0.1b2/src/cerebrumscanner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 05:44:06.000000 cerebrumscanner-0.0.1b2/src/cerebrumscanner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-28 05:44:06.000000 cerebrumscanner-0.0.1b2/src/cerebrumscanner.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      172 2024-05-28 05:44:06.000000 cerebrumscanner-0.0.1b2/src/cerebrumscanner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-28 05:44:06.000000 cerebrumscanner-0.0.1b2/src/cerebrumscanner.egg-info/top_level.txt
+drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 05:59:39.969767 cerebrumscanner-0.0.1b3/
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       63 2024-05-27 08:15:33.000000 cerebrumscanner-0.0.1b3/LICENSE
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       24 2024-05-27 09:23:20.000000 cerebrumscanner-0.0.1b3/MANIFEST.in
+-rw-r--r--   0 nekodu-01  (1000) nekodu-01  (1000)     6618 2024-05-28 05:59:39.969767 cerebrumscanner-0.0.1b3/PKG-INFO
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)     6239 2024-05-27 08:02:00.000000 cerebrumscanner-0.0.1b3/README.md
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        6 2024-05-27 09:20:05.000000 cerebrumscanner-0.0.1b3/requirements.txt
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       38 2024-05-28 05:59:39.969767 cerebrumscanner-0.0.1b3/setup.cfg
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)      976 2024-05-28 05:58:17.000000 cerebrumscanner-0.0.1b3/setup.py
+drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 05:59:39.969767 cerebrumscanner-0.0.1b3/src/
+drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 05:59:39.969767 cerebrumscanner-0.0.1b3/src/cerebrumscanner/
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-27 08:46:33.000000 cerebrumscanner-0.0.1b3/src/cerebrumscanner/__init__.py
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       87 2024-05-27 08:46:58.000000 cerebrumscanner-0.0.1b3/src/cerebrumscanner/dummy_module3.py
+drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 05:59:39.969767 cerebrumscanner-0.0.1b3/src/cerebrumscanner/lib/
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       87 2024-05-27 08:23:20.000000 cerebrumscanner-0.0.1b3/src/cerebrumscanner/lib/dummy_module2.py
+drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 05:59:39.969767 cerebrumscanner-0.0.1b3/src/cerebrumscanner.egg-info/
+-rw-r--r--   0 nekodu-01  (1000) nekodu-01  (1000)     6618 2024-05-28 05:59:39.000000 cerebrumscanner-0.0.1b3/src/cerebrumscanner.egg-info/PKG-INFO
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)      434 2024-05-28 05:59:39.000000 cerebrumscanner-0.0.1b3/src/cerebrumscanner.egg-info/SOURCES.txt
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        1 2024-05-28 05:59:39.000000 cerebrumscanner-0.0.1b3/src/cerebrumscanner.egg-info/dependency_links.txt
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        1 2024-05-28 05:59:39.000000 cerebrumscanner-0.0.1b3/src/cerebrumscanner.egg-info/not-zip-safe
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)        7 2024-05-28 05:59:39.000000 cerebrumscanner-0.0.1b3/src/cerebrumscanner.egg-info/requires.txt
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       16 2024-05-28 05:59:39.000000 cerebrumscanner-0.0.1b3/src/cerebrumscanner.egg-info/top_level.txt
+drwxrwsr-x   0 nekodu-01  (1000) nekodu-01  (1000)        0 2024-05-28 05:59:39.969767 cerebrumscanner-0.0.1b3/test/
+-rw-rw-r--   0 nekodu-01  (1000) nekodu-01  (1000)       59 2024-05-27 08:09:56.000000 cerebrumscanner-0.0.1b3/test/test.py
```

### Comparing `cerebrumscanner-0.0.1b2/setup.py` & `cerebrumscanner-0.0.1b3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from setuptools import find_namespace_packages, setup
-
-package_license: str = ""
-long_description: str = ""
-install_requires = []
-
-with open("LICENSE", encoding="utf-8") as license_file, open(
-    "README.md", encoding="utf-8"
-) as readme_file, open("requirements.txt", encoding="utf-8") as requirements_file:
-    package_license = license_file.read()
-    long_description = readme_file.read()
-    install_requires = requirements_file.read().split("\n")[0:]
-
-setup(
-    name="cerebrumscanner",
-    version="0.0.1.b2",
-    url="https://gitlab.com/nekodu/cerebrumscanner/cerebrum-scanner",
-    license=package_license,
-    author="Nekodu Technology",
-    author_email="info@nekodu.com",
-    description=(
-        "Cerebrum Scanner Project"
-    ),
-    package_dir={"": "src"},
-    packages=find_namespace_packages(where="src"),
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    install_requires=install_requires,
-    zip_safe=False,
-)
+from setuptools import find_namespace_packages, setup
+
+package_license: str = ""
+long_description: str = ""
+install_requires = []
+
+with open("LICENSE", encoding="utf-8") as license_file, open(
+    "README.md", encoding="utf-8"
+) as readme_file, open("requirements.txt", encoding="utf-8") as requirements_file:
+    package_license = license_file.read()
+    long_description = readme_file.read()
+    install_requires = requirements_file.read().split("\n")[0:]
+
+setup(
+    name="cerebrumscanner",
+    version="0.0.1.b3",
+    url="https://gitlab.com/nekodu/cerebrumscanner/cerebrum-scanner",
+    license=package_license,
+    author="Nekodu Technology",
+    author_email="info@nekodu.com",
+    description=(
+        "Cerebrum Scanner Project"
+    ),
+    package_dir={"": "src"},
+    packages=find_namespace_packages(where="src"),
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    install_requires=install_requires,
+    zip_safe=False,
+)
```

