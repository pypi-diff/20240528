# Comparing `tmp/duckframes-0.0.2.tar.gz` & `tmp/duckframes-0.0.3.tar.gz`

## Comparing `duckframes-0.0.2.tar` & `duckframes-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 duckframes-0.0.2/dev-requirements.txt
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 duckframes-0.0.2/justfile
--rw-r--r--   0        0        0   284955 2020-02-02 00:00:00.000000 duckframes-0.0.2/logo.png
--rw-r--r--   0        0        0    15367 2020-02-02 00:00:00.000000 duckframes-0.0.2/penguins.csv
--rw-r--r--   0        0        0     5482 2020-02-02 00:00:00.000000 duckframes-0.0.2/penguins.parquet
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 duckframes-0.0.2/.vscode/settings.json
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 duckframes-0.0.2/src/duckframes/__init__.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 duckframes-0.0.2/.gitignore
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 duckframes-0.0.2/LICENSE
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 duckframes-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 duckframes-0.0.2/readme.md
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 duckframes-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 duckframes-0.0.3/dev-requirements.txt
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 duckframes-0.0.3/justfile
+-rw-r--r--   0        0        0   284955 2020-02-02 00:00:00.000000 duckframes-0.0.3/logo.png
+-rw-r--r--   0        0        0    15367 2020-02-02 00:00:00.000000 duckframes-0.0.3/penguins.csv
+-rw-r--r--   0        0        0     5482 2020-02-02 00:00:00.000000 duckframes-0.0.3/penguins.parquet
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 duckframes-0.0.3/.vscode/settings.json
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 duckframes-0.0.3/src/duckframes/__init__.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 duckframes-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 duckframes-0.0.3/LICENSE
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 duckframes-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 duckframes-0.0.3/readme.md
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 duckframes-0.0.3/PKG-INFO
```

### Comparing `duckframes-0.0.2/justfile` & `duckframes-0.0.3/justfile`

 * *Files identical despite different names*

### Comparing `duckframes-0.0.2/logo.png` & `duckframes-0.0.3/logo.png`

 * *Files identical despite different names*

### Comparing `duckframes-0.0.2/penguins.csv` & `duckframes-0.0.3/penguins.csv`

 * *Files identical despite different names*

### Comparing `duckframes-0.0.2/penguins.parquet` & `duckframes-0.0.3/penguins.parquet`

 * *Files identical despite different names*

### Comparing `duckframes-0.0.2/LICENSE` & `duckframes-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `duckframes-0.0.2/pyproject.toml` & `duckframes-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "duckframes"
-version = "0.0.2"
+version = "0.0.3"
 authors = [{ name = "Cody", email = "cody@dkdc.dev" }]
 description = "coming soon?"
 readme = "readme.md"
 requires-python = ">=3.9"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `duckframes-0.0.2/PKG-INFO` & `duckframes-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: duckframes
-Version: 0.0.2
+Version: 0.0.3
 Summary: coming soon?
 Project-URL: Homepage, https://github.com/lostmygithubaccount/duckframes
 Project-URL: Bug Tracker, https://github.com/lostmygithubaccount/duckframes
 Author-email: Cody <cody@dkdc.dev>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

