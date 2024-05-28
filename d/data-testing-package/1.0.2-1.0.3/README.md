# Comparing `tmp/data_testing_package-1.0.2.tar.gz` & `tmp/data_testing_package-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_testing_package-1.0.2.tar", max compression
+gzip compressed data, was "data_testing_package-1.0.3.tar", max compression
```

## Comparing `data_testing_package-1.0.2.tar` & `data_testing_package-1.0.3.tar`

### file list

```diff
@@ -1,7 +1,17 @@
--rw-r--r--   0        0        0      853 2024-05-28 08:53:57.647640 data_testing_package-1.0.2/README.md
--rw-r--r--   0        0        0      977 2024-05-28 09:06:21.483603 data_testing_package-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       66 2024-05-22 09:40:27.131008 data_testing_package-1.0.2/src/data_testing_package/__init__.py
--rw-r--r--   0        0        0       73 2024-05-22 09:40:27.131281 data_testing_package-1.0.2/src/data_testing_package/common_methods/__init__.py
--rw-r--r--   0        0        0    16310 2024-05-24 14:48:00.942153 data_testing_package-1.0.2/src/data_testing_package/common_methods/parquet_handler.py
--rw-r--r--   0        0        0    11514 2024-05-24 14:24:02.354711 data_testing_package-1.0.2/src/data_testing_package/common_methods/utilities.py
--rw-r--r--   0        0        0     2028 1970-01-01 00:00:00.000000 data_testing_package-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      853 2024-05-28 08:53:57.647640 data_testing_package-1.0.3/README.md
+-rw-r--r--   0        0        0      977 2024-05-28 09:13:33.160821 data_testing_package-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       66 2024-05-22 09:40:27.131008 data_testing_package-1.0.3/src/data_testing_package/__init__.py
+-rw-r--r--   0        0        0       73 2024-05-22 09:40:27.131281 data_testing_package-1.0.3/src/data_testing_package/common_methods/__init__.py
+-rw-r--r--   0        0        0    16310 2024-05-24 14:48:00.942153 data_testing_package-1.0.3/src/data_testing_package/common_methods/parquet_handler.py
+-rw-r--r--   0        0        0    11514 2024-05-24 14:24:02.354711 data_testing_package-1.0.3/src/data_testing_package/common_methods/utilities.py
+-rw-r--r--   0        0        0       42 2024-05-28 08:55:35.167926 data_testing_package-1.0.3/src/data_testing_package/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 09:40:27.132042 data_testing_package-1.0.3/src/data_testing_package/tests/folder_for_file_check/sample.file
+-rw-r--r--   0        0        0      139 2024-05-23 14:41:46.774051 data_testing_package-1.0.3/src/data_testing_package/tests/missing_column.csv
+-rw-r--r--   0        0        0      155 2024-05-24 14:48:00.943056 data_testing_package-1.0.3/src/data_testing_package/tests/no_missing_column.csv
+-rw-r--r--   0        0        0      243 2024-05-22 09:40:27.132206 data_testing_package-1.0.3/src/data_testing_package/tests/sample.csv
+-rw-r--r--   0        0        0     1308 2024-05-22 09:40:27.132356 data_testing_package-1.0.3/src/data_testing_package/tests/sample.parquet
+-rw-r--r--   0        0        0      242 2024-05-22 09:40:27.132503 data_testing_package-1.0.3/src/data_testing_package/tests/sample2.csv
+-rw-r--r--   0        0        0       23 2024-05-22 09:40:27.132681 data_testing_package-1.0.3/src/data_testing_package/tests/test.json
+-rw-r--r--   0        0        0     3709 2024-05-24 14:48:00.943923 data_testing_package-1.0.3/src/data_testing_package/tests/test_common_methods_parquet_handler.py
+-rw-r--r--   0        0        0     7897 2024-05-24 14:48:00.946377 data_testing_package-1.0.3/src/data_testing_package/tests/test_generic_utilities.py
+-rw-r--r--   0        0        0     2028 1970-01-01 00:00:00.000000 data_testing_package-1.0.3/PKG-INFO
```

### Comparing `data_testing_package-1.0.2/README.md` & `data_testing_package-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `data_testing_package-1.0.2/pyproject.toml` & `data_testing_package-1.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-testing-package"
-version = "1.0.2"
+version = "1.0.3"
 description = "BJSS Testing Package"
 authors = ["Babatunde Salaam <tunde.salaam@bjss.com>", "Richa Jha <richa.jha@bjss.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "~3.8.10"
 allure-behave = "^2.8.6"
```

### Comparing `data_testing_package-1.0.2/src/data_testing_package/common_methods/parquet_handler.py` & `data_testing_package-1.0.3/src/data_testing_package/common_methods/parquet_handler.py`

 * *Files identical despite different names*

### Comparing `data_testing_package-1.0.2/src/data_testing_package/common_methods/utilities.py` & `data_testing_package-1.0.3/src/data_testing_package/common_methods/utilities.py`

 * *Files identical despite different names*

### Comparing `data_testing_package-1.0.2/PKG-INFO` & `data_testing_package-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-testing-package
-Version: 1.0.2
+Version: 1.0.3
 Summary: BJSS Testing Package
 Author: Babatunde Salaam
 Author-email: tunde.salaam@bjss.com
 Requires-Python: >=3.8.10,<3.9.0
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: Faker (>=15.3.3,<16.0.0)
 Requires-Dist: allure-behave (>=2.8.6,<3.0.0)
```

