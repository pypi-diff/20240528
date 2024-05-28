# Comparing `tmp/data_testing_package-1.0.0.tar.gz` & `tmp/data_testing_package-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_testing_package-1.0.0.tar", max compression
+gzip compressed data, was "data_testing_package-1.0.1.tar", max compression
```

## Comparing `data_testing_package-1.0.0.tar` & `data_testing_package-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      689 2024-05-22 10:56:23.657844 data_testing_package-1.0.0/README.md
--rw-r--r--   0        0        0      977 2024-05-23 14:41:46.772837 data_testing_package-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       66 2024-05-22 09:40:27.131008 data_testing_package-1.0.0/src/data_testing_package/__init__.py
--rw-r--r--   0        0        0       73 2024-05-22 09:40:27.131281 data_testing_package-1.0.0/src/data_testing_package/common_methods/__init__.py
--rw-r--r--   0        0        0    16310 2024-05-24 14:48:00.942153 data_testing_package-1.0.0/src/data_testing_package/common_methods/parquet_handler.py
--rw-r--r--   0        0        0    11514 2024-05-24 14:24:02.354711 data_testing_package-1.0.0/src/data_testing_package/common_methods/utilities.py
--rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 data_testing_package-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      853 2024-05-28 08:53:57.647640 data_testing_package-1.0.1/README.md
+-rw-r--r--   0        0        0      977 2024-05-28 08:59:38.278053 data_testing_package-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       66 2024-05-22 09:40:27.131008 data_testing_package-1.0.1/src/data_testing_package/__init__.py
+-rw-r--r--   0        0        0       73 2024-05-22 09:40:27.131281 data_testing_package-1.0.1/src/data_testing_package/common_methods/__init__.py
+-rw-r--r--   0        0        0    16310 2024-05-24 14:48:00.942153 data_testing_package-1.0.1/src/data_testing_package/common_methods/parquet_handler.py
+-rw-r--r--   0        0        0    11514 2024-05-24 14:24:02.354711 data_testing_package-1.0.1/src/data_testing_package/common_methods/utilities.py
+-rw-r--r--   0        0        0     2028 1970-01-01 00:00:00.000000 data_testing_package-1.0.1/PKG-INFO
```

### Comparing `data_testing_package-1.0.0/README.md` & `data_testing_package-1.0.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -10,8 +10,12 @@
 
 To activate virtual environment run `poetry shell`
 
 To come out of your virtual environment run `deactivate`
 
 More information on poetry `https://www.youtube.com/watch?v=0f3moPe_bhk`
 
-You can find the dependencies included in the `pyproject.toml`
+You can find the dependencies included in the `pyproject.toml`
+
+To publish a package using poetry: 'https://python-poetry.org/docs/repositories/#configuring-credentials'
+
+To use the published package: Poetry add 'package-name'
```

### Comparing `data_testing_package-1.0.0/pyproject.toml` & `data_testing_package-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-testing-package"
-version = "1.0.0"
+version = "1.0.1"
 description = "BJSS Testing Package"
 authors = ["Babatunde Salaam <tunde.salaam@bjss.com>", "Richa Jha <richa.jha@bjss.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "~3.8.10"
 allure-behave = "^2.8.6"
```

### Comparing `data_testing_package-1.0.0/src/data_testing_package/common_methods/parquet_handler.py` & `data_testing_package-1.0.1/src/data_testing_package/common_methods/parquet_handler.py`

 * *Files identical despite different names*

### Comparing `data_testing_package-1.0.0/src/data_testing_package/common_methods/utilities.py` & `data_testing_package-1.0.1/src/data_testing_package/common_methods/utilities.py`

 * *Files identical despite different names*

### Comparing `data_testing_package-1.0.0/PKG-INFO` & `data_testing_package-1.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-testing-package
-Version: 1.0.0
+Version: 1.0.1
 Summary: BJSS Testing Package
 Author: Babatunde Salaam
 Author-email: tunde.salaam@bjss.com
 Requires-Python: >=3.8.10,<3.9.0
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: Faker (>=15.3.3,<16.0.0)
 Requires-Dist: allure-behave (>=2.8.6,<3.0.0)
@@ -41,7 +41,11 @@
 To activate virtual environment run `poetry shell`
 
 To come out of your virtual environment run `deactivate`
 
 More information on poetry `https://www.youtube.com/watch?v=0f3moPe_bhk`
 
 You can find the dependencies included in the `pyproject.toml`
+
+To publish a package using poetry: 'https://python-poetry.org/docs/repositories/#configuring-credentials'
+
+To use the published package: Poetry add 'package-name'
```

