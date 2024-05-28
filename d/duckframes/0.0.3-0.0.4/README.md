# Comparing `tmp/duckframes-0.0.3.tar.gz` & `tmp/duckframes-0.0.4.tar.gz`

## Comparing `duckframes-0.0.3.tar` & `duckframes-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 duckframes-0.0.3/dev-requirements.txt
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 duckframes-0.0.3/justfile
--rw-r--r--   0        0        0   284955 2020-02-02 00:00:00.000000 duckframes-0.0.3/logo.png
--rw-r--r--   0        0        0    15367 2020-02-02 00:00:00.000000 duckframes-0.0.3/penguins.csv
--rw-r--r--   0        0        0     5482 2020-02-02 00:00:00.000000 duckframes-0.0.3/penguins.parquet
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 duckframes-0.0.3/.vscode/settings.json
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 duckframes-0.0.3/src/duckframes/__init__.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 duckframes-0.0.3/.gitignore
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 duckframes-0.0.3/LICENSE
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 duckframes-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 duckframes-0.0.3/readme.md
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 duckframes-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 duckframes-0.0.4/dev-requirements.txt
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 duckframes-0.0.4/justfile
+-rw-r--r--   0        0        0    16267 2020-02-02 00:00:00.000000 duckframes-0.0.4/logo.png
+-rw-r--r--   0        0        0    14115 2020-02-02 00:00:00.000000 duckframes-0.0.4/logo.svg
+-rw-r--r--   0        0        0    15367 2020-02-02 00:00:00.000000 duckframes-0.0.4/penguins.csv
+-rw-r--r--   0        0        0     5482 2020-02-02 00:00:00.000000 duckframes-0.0.4/penguins.parquet
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 duckframes-0.0.4/.vscode/settings.json
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 duckframes-0.0.4/src/duckframes/__init__.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 duckframes-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 duckframes-0.0.4/LICENSE
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 duckframes-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 duckframes-0.0.4/readme.md
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 duckframes-0.0.4/PKG-INFO
```

### Comparing `duckframes-0.0.3/justfile` & `duckframes-0.0.4/justfile`

 * *Files identical despite different names*

### Comparing `duckframes-0.0.3/penguins.csv` & `duckframes-0.0.4/penguins.csv`

 * *Files identical despite different names*

### Comparing `duckframes-0.0.3/penguins.parquet` & `duckframes-0.0.4/penguins.parquet`

 * *Files identical despite different names*

### Comparing `duckframes-0.0.3/LICENSE` & `duckframes-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `duckframes-0.0.3/pyproject.toml` & `duckframes-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "duckframes"
-version = "0.0.3"
+version = "0.0.4"
 authors = [{ name = "Cody", email = "cody@dkdc.dev" }]
 description = "coming soon?"
 readme = "readme.md"
 requires-python = ">=3.9"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `duckframes-0.0.3/PKG-INFO` & `duckframes-0.0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: duckframes
-Version: 0.0.3
+Version: 0.0.4
 Summary: coming soon?
 Project-URL: Homepage, https://github.com/lostmygithubaccount/duckframes
 Project-URL: Bug Tracker, https://github.com/lostmygithubaccount/duckframes
 Author-email: Cody <cody@dkdc.dev>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

