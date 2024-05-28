# Comparing `tmp/duckframes-0.0.1.tar.gz` & `tmp/duckframes-0.0.2.tar.gz`

## Comparing `duckframes-0.0.1.tar` & `duckframes-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 duckframes-0.0.1/dev-requirements.txt
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 duckframes-0.0.1/justfile
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 duckframes-0.0.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 duckframes-0.0.1/src/duckframes/__init__.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 duckframes-0.0.1/.gitignore
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 duckframes-0.0.1/LICENSE
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 duckframes-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 duckframes-0.0.1/readme.md
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 duckframes-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 duckframes-0.0.2/dev-requirements.txt
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 duckframes-0.0.2/justfile
+-rw-r--r--   0        0        0   284955 2020-02-02 00:00:00.000000 duckframes-0.0.2/logo.png
+-rw-r--r--   0        0        0    15367 2020-02-02 00:00:00.000000 duckframes-0.0.2/penguins.csv
+-rw-r--r--   0        0        0     5482 2020-02-02 00:00:00.000000 duckframes-0.0.2/penguins.parquet
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 duckframes-0.0.2/.vscode/settings.json
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 duckframes-0.0.2/src/duckframes/__init__.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 duckframes-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 duckframes-0.0.2/LICENSE
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 duckframes-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 duckframes-0.0.2/readme.md
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 duckframes-0.0.2/PKG-INFO
```

### Comparing `duckframes-0.0.1/justfile` & `duckframes-0.0.2/justfile`

 * *Files 4% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 
 # format
 format:
     @ruff format . || True
 
 # install
 install:
-    @uv pip install -e '.[all]' --reinstall-package dkdc
+    @uv pip install -e '.[all]' --reinstall-package duckframes
 
 # uninstall
 uninstall:
-    @uv pip uninstall dkdc -y
+    @uv pip uninstall duckframes -y
 
 # publish-test
 release-test:
     just build
     @twine upload --repository testpypi dist/* -u __token__ -p ${PYPI_TEST_TOKEN}
 
 # publish
```

### Comparing `duckframes-0.0.1/LICENSE` & `duckframes-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `duckframes-0.0.1/PKG-INFO` & `duckframes-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.3
 Name: duckframes
-Version: 0.0.1
+Version: 0.0.2
 Summary: coming soon?
-Project-URL: Homepage, https://github.com/ibis-project/duckframes
-Project-URL: Bug Tracker, https://github.com/ibis-project/duckframes
+Project-URL: Homepage, https://github.com/lostmygithubaccount/duckframes
+Project-URL: Bug Tracker, https://github.com/lostmygithubaccount/duckframes
 Author-email: Cody <cody@dkdc.dev>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Requires-Dist: ibis-framework[duckdb]
 Description-Content-Type: text/markdown
 
 # duckframes
 
 coming soon?
```

