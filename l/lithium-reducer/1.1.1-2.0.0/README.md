# Comparing `tmp/lithium-reducer-1.1.1.tar.gz` & `tmp/lithium-reducer-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lithium-reducer-1.1.1.tar", last modified: Fri Dec 29 19:55:13 2023, max compression
+gzip compressed data, was "lithium-reducer-2.0.0.tar", last modified: Tue May 28 19:33:33 2024, max compression
```

## Comparing `lithium-reducer-1.1.1.tar` & `lithium-reducer-2.0.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-12-29 19:55:13.724723 lithium-reducer-1.1.1/
--rw-r--r--   0 worker    (1000) worker    (1000)      238 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/.gitattributes
--rw-r--r--   0 worker    (1000) worker    (1000)      416 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/.gitignore
--rw-r--r--   0 worker    (1000) worker    (1000)     1753 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0 worker    (1000) worker    (1000)     3314 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/.taskcluster.yml
--rw-r--r--   0 worker    (1000) worker    (1000)      689 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 worker    (1000) worker    (1000)    16725 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/LICENSE
--rw-r--r--   0 worker    (1000) worker    (1000)     7119 2023-12-29 19:55:13.724723 lithium-reducer-1.1.1/PKG-INFO
--rw-r--r--   0 worker    (1000) worker    (1000)     6302 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/README.md
--rw-r--r--   0 worker    (1000) worker    (1000)      996 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/pyproject.toml
--rw-r--r--   0 worker    (1000) worker    (1000)     1753 2023-12-29 19:55:13.724723 lithium-reducer-1.1.1/setup.cfg
--rwxr-xr-x   0 worker    (1000) worker    (1000)      370 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/setup.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-12-29 19:55:13.712723 lithium-reducer-1.1.1/src/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-12-29 19:55:13.716723 lithium-reducer-1.1.1/src/lithium/
--rw-r--r--   0 worker    (1000) worker    (1000)      395 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/src/lithium/__init__.py
--rw-r--r--   0 worker    (1000) worker    (1000)      281 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/src/lithium/__main__.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-12-29 19:55:13.720723 lithium-reducer-1.1.1/src/lithium/docs/
--rw-r--r--   0 worker    (1000) worker    (1000)     6367 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/src/lithium/docs/algorithm.md
--rw-r--r--   0 worker    (1000) worker    (1000)     1484 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/src/lithium/docs/creating-tests.md
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-12-29 19:55:13.720723 lithium-reducer-1.1.1/src/lithium/docs/examples/
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-12-29 19:55:13.720723 lithium-reducer-1.1.1/src/lithium/docs/examples/arithmetic/
--rw-r--r--   0 worker    (1000) worker    (1000)       48 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/src/lithium/docs/examples/arithmetic/11.txt
--rw-r--r--   0 worker    (1000) worker    (1000)     1000 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/src/lithium/docs/examples/arithmetic/product_divides.py
--rw-r--r--   0 worker    (1000) worker    (1000)       50 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/src/lithium/docs/examples/crash.c
--rw-r--r--   0 worker    (1000) worker    (1000)      205 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/src/lithium/docs/related.txt
--rw-r--r--   0 worker    (1000) worker    (1000)     3912 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/src/lithium/docs/using-for-firefox.md
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-12-29 19:55:13.720723 lithium-reducer-1.1.1/src/lithium/interestingness/
--rw-r--r--   0 worker    (1000) worker    (1000)        0 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/src/lithium/interestingness/__init__.py
--rw-r--r--   0 worker    (1000) worker    (1000)     1470 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/src/lithium/interestingness/crashes.py
--rw-r--r--   0 worker    (1000) worker    (1000)     3715 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/src/lithium/interestingness/diff_test.py
--rw-r--r--   0 worker    (1000) worker    (1000)     1465 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/src/lithium/interestingness/hangs.py
--rw-r--r--   0 worker    (1000) worker    (1000)     2735 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/src/lithium/interestingness/outputs.py
--rw-r--r--   0 worker    (1000) worker    (1000)     2824 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/src/lithium/interestingness/repeat.py
--rw-r--r--   0 worker    (1000) worker    (1000)     6960 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/src/lithium/interestingness/timed_run.py
--rw-r--r--   0 worker    (1000) worker    (1000)     4282 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/src/lithium/interestingness/utils.py
--rw-r--r--   0 worker    (1000) worker    (1000)        0 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/src/lithium/py.typed
--rw-r--r--   0 worker    (1000) worker    (1000)    11514 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/src/lithium/reducer.py
--rw-r--r--   0 worker    (1000) worker    (1000)    63708 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/src/lithium/strategies.py
--rw-r--r--   0 worker    (1000) worker    (1000)    18226 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/src/lithium/testcases.py
--rw-r--r--   0 worker    (1000) worker    (1000)     2115 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/src/lithium/util.py
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-12-29 19:55:13.724723 lithium-reducer-1.1.1/src/lithium_reducer.egg-info/
--rw-r--r--   0 worker    (1000) worker    (1000)     7119 2023-12-29 19:55:13.000000 lithium-reducer-1.1.1/src/lithium_reducer.egg-info/PKG-INFO
--rw-r--r--   0 worker    (1000) worker    (1000)     1326 2023-12-29 19:55:13.000000 lithium-reducer-1.1.1/src/lithium_reducer.egg-info/SOURCES.txt
--rw-r--r--   0 worker    (1000) worker    (1000)        1 2023-12-29 19:55:13.000000 lithium-reducer-1.1.1/src/lithium_reducer.egg-info/dependency_links.txt
--rw-r--r--   0 worker    (1000) worker    (1000)      733 2023-12-29 19:55:13.000000 lithium-reducer-1.1.1/src/lithium_reducer.egg-info/entry_points.txt
--rw-r--r--   0 worker    (1000) worker    (1000)        1 2023-12-29 19:55:13.000000 lithium-reducer-1.1.1/src/lithium_reducer.egg-info/not-zip-safe
--rw-r--r--   0 worker    (1000) worker    (1000)       39 2023-12-29 19:55:13.000000 lithium-reducer-1.1.1/src/lithium_reducer.egg-info/requires.txt
--rw-r--r--   0 worker    (1000) worker    (1000)        8 2023-12-29 19:55:13.000000 lithium-reducer-1.1.1/src/lithium_reducer.egg-info/top_level.txt
-drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2023-12-29 19:55:13.724723 lithium-reducer-1.1.1/tests/
--rw-r--r--   0 worker    (1000) worker    (1000)     1812 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/tests/conftest.py
--rw-r--r--   0 worker    (1000) worker    (1000)    12529 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/tests/test_interestingness.py
--rw-r--r--   0 worker    (1000) worker    (1000)     3018 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/tests/test_lithium.py
--rw-r--r--   0 worker    (1000) worker    (1000)     9921 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/tests/test_strategies.py
--rw-r--r--   0 worker    (1000) worker    (1000)    16807 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/tests/test_testcases.py
--rw-r--r--   0 worker    (1000) worker    (1000)     4257 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/tests/test_util.py
--rw-r--r--   0 worker    (1000) worker    (1000)     1276 2023-12-29 19:55:07.000000 lithium-reducer-1.1.1/tox.ini
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-05-28 19:33:33.790715 lithium-reducer-2.0.0/
+-rw-r--r--   0 worker    (1000) worker    (1000)      238 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/.gitattributes
+-rw-r--r--   0 worker    (1000) worker    (1000)      416 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/.gitignore
+-rw-r--r--   0 worker    (1000) worker    (1000)     1753 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 worker    (1000) worker    (1000)     3314 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/.taskcluster.yml
+-rw-r--r--   0 worker    (1000) worker    (1000)      689 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 worker    (1000) worker    (1000)    16725 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/LICENSE
+-rw-r--r--   0 worker    (1000) worker    (1000)     7119 2024-05-28 19:33:33.790715 lithium-reducer-2.0.0/PKG-INFO
+-rw-r--r--   0 worker    (1000) worker    (1000)     6302 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/README.md
+-rw-r--r--   0 worker    (1000) worker    (1000)      996 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/pyproject.toml
+-rw-r--r--   0 worker    (1000) worker    (1000)     1753 2024-05-28 19:33:33.790715 lithium-reducer-2.0.0/setup.cfg
+-rwxr-xr-x   0 worker    (1000) worker    (1000)      370 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/setup.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-05-28 19:33:33.778715 lithium-reducer-2.0.0/src/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-05-28 19:33:33.782715 lithium-reducer-2.0.0/src/lithium/
+-rw-r--r--   0 worker    (1000) worker    (1000)      395 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/src/lithium/__init__.py
+-rw-r--r--   0 worker    (1000) worker    (1000)      281 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/src/lithium/__main__.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-05-28 19:33:33.782715 lithium-reducer-2.0.0/src/lithium/docs/
+-rw-r--r--   0 worker    (1000) worker    (1000)     6367 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/src/lithium/docs/algorithm.md
+-rw-r--r--   0 worker    (1000) worker    (1000)     1484 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/src/lithium/docs/creating-tests.md
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-05-28 19:33:33.782715 lithium-reducer-2.0.0/src/lithium/docs/examples/
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-05-28 19:33:33.782715 lithium-reducer-2.0.0/src/lithium/docs/examples/arithmetic/
+-rw-r--r--   0 worker    (1000) worker    (1000)       48 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/src/lithium/docs/examples/arithmetic/11.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)     1000 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/src/lithium/docs/examples/arithmetic/product_divides.py
+-rw-r--r--   0 worker    (1000) worker    (1000)       50 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/src/lithium/docs/examples/crash.c
+-rw-r--r--   0 worker    (1000) worker    (1000)      205 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/src/lithium/docs/related.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)     3912 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/src/lithium/docs/using-for-firefox.md
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-05-28 19:33:33.786715 lithium-reducer-2.0.0/src/lithium/interestingness/
+-rw-r--r--   0 worker    (1000) worker    (1000)        0 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/src/lithium/interestingness/__init__.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     1470 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/src/lithium/interestingness/crashes.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     3715 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/src/lithium/interestingness/diff_test.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     1465 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/src/lithium/interestingness/hangs.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     2735 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/src/lithium/interestingness/outputs.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     2824 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/src/lithium/interestingness/repeat.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     6960 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/src/lithium/interestingness/timed_run.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     4282 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/src/lithium/interestingness/utils.py
+-rw-r--r--   0 worker    (1000) worker    (1000)        0 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/src/lithium/py.typed
+-rw-r--r--   0 worker    (1000) worker    (1000)    11514 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/src/lithium/reducer.py
+-rw-r--r--   0 worker    (1000) worker    (1000)    63711 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/src/lithium/strategies.py
+-rw-r--r--   0 worker    (1000) worker    (1000)    18226 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/src/lithium/testcases.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     2115 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/src/lithium/util.py
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-05-28 19:33:33.786715 lithium-reducer-2.0.0/src/lithium_reducer.egg-info/
+-rw-r--r--   0 worker    (1000) worker    (1000)     7119 2024-05-28 19:33:33.000000 lithium-reducer-2.0.0/src/lithium_reducer.egg-info/PKG-INFO
+-rw-r--r--   0 worker    (1000) worker    (1000)     1326 2024-05-28 19:33:33.000000 lithium-reducer-2.0.0/src/lithium_reducer.egg-info/SOURCES.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)        1 2024-05-28 19:33:33.000000 lithium-reducer-2.0.0/src/lithium_reducer.egg-info/dependency_links.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)      733 2024-05-28 19:33:33.000000 lithium-reducer-2.0.0/src/lithium_reducer.egg-info/entry_points.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)        1 2024-05-28 19:33:33.000000 lithium-reducer-2.0.0/src/lithium_reducer.egg-info/not-zip-safe
+-rw-r--r--   0 worker    (1000) worker    (1000)       39 2024-05-28 19:33:33.000000 lithium-reducer-2.0.0/src/lithium_reducer.egg-info/requires.txt
+-rw-r--r--   0 worker    (1000) worker    (1000)        8 2024-05-28 19:33:33.000000 lithium-reducer-2.0.0/src/lithium_reducer.egg-info/top_level.txt
+drwxr-xr-x   0 worker    (1000) worker    (1000)        0 2024-05-28 19:33:33.786715 lithium-reducer-2.0.0/tests/
+-rw-r--r--   0 worker    (1000) worker    (1000)     1812 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/tests/conftest.py
+-rw-r--r--   0 worker    (1000) worker    (1000)    12529 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/tests/test_interestingness.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     3018 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/tests/test_lithium.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     9921 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/tests/test_strategies.py
+-rw-r--r--   0 worker    (1000) worker    (1000)    16807 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/tests/test_testcases.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     4257 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/tests/test_util.py
+-rw-r--r--   0 worker    (1000) worker    (1000)     1276 2024-05-28 19:33:26.000000 lithium-reducer-2.0.0/tox.ini
```

### Comparing `lithium-reducer-1.1.1/.pre-commit-config.yaml` & `lithium-reducer-2.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/.taskcluster.yml` & `lithium-reducer-2.0.0/.taskcluster.yml`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/CODE_OF_CONDUCT.md` & `lithium-reducer-2.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/LICENSE` & `lithium-reducer-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/PKG-INFO` & `lithium-reducer-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lithium-reducer
-Version: 1.1.1
+Version: 2.0.0
 Summary: Lithium is an automated testcase reduction tool
 Home-page: https://github.com/MozillaSecurity/lithium
 Author: Jesse Ruderman
 Maintainer: Mozilla Fuzzing Team
 Maintainer-email: fuzzing@mozilla.com
 License: MPL 2.0
 Keywords: fuzz,fuzzing,reduce,reducer,reduction,security,test,testing
```

### Comparing `lithium-reducer-1.1.1/README.md` & `lithium-reducer-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/pyproject.toml` & `lithium-reducer-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/setup.cfg` & `lithium-reducer-2.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/src/lithium/docs/algorithm.md` & `lithium-reducer-2.0.0/src/lithium/docs/algorithm.md`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/src/lithium/docs/creating-tests.md` & `lithium-reducer-2.0.0/src/lithium/docs/creating-tests.md`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/src/lithium/docs/examples/arithmetic/product_divides.py` & `lithium-reducer-2.0.0/src/lithium/docs/examples/arithmetic/product_divides.py`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/src/lithium/docs/using-for-firefox.md` & `lithium-reducer-2.0.0/src/lithium/docs/using-for-firefox.md`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/src/lithium/interestingness/crashes.py` & `lithium-reducer-2.0.0/src/lithium/interestingness/crashes.py`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/src/lithium/interestingness/diff_test.py` & `lithium-reducer-2.0.0/src/lithium/interestingness/diff_test.py`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/src/lithium/interestingness/hangs.py` & `lithium-reducer-2.0.0/src/lithium/interestingness/hangs.py`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/src/lithium/interestingness/outputs.py` & `lithium-reducer-2.0.0/src/lithium/interestingness/outputs.py`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/src/lithium/interestingness/repeat.py` & `lithium-reducer-2.0.0/src/lithium/interestingness/repeat.py`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/src/lithium/interestingness/timed_run.py` & `lithium-reducer-2.0.0/src/lithium/interestingness/timed_run.py`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/src/lithium/interestingness/utils.py` & `lithium-reducer-2.0.0/src/lithium/interestingness/utils.py`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/src/lithium/reducer.py` & `lithium-reducer-2.0.0/src/lithium/reducer.py`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/src/lithium/strategies.py` & `lithium-reducer-2.0.0/src/lithium/strategies.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,36 +49,36 @@
 
     def __init__(self, testcase: Testcase) -> None:
         self._best_testcase = testcase
         self._testcase_attempt: Optional[Testcase] = None
         self._any_success: bool = False
         self._last_success: Optional[bool] = None
         self._description: str = "Reduction"
-        self._tried: Set[str] = set()
+        self._tried: Set[bytes] = set()
 
     @property
     def last_feedback(self) -> bool:
         """Get the feedback value from the latest attempt.
 
         Returns:
             The value last passed to `self.feedback()`
         """
         assert self._last_success is not None, "No feedback received yet"
         return self._last_success
 
-    def update_tried(self, tried: Iterable[str]) -> None:
+    def update_tried(self, tried: Iterable[bytes]) -> None:
         """Update the list of tried hashes. Testcases are hashed with SHA-512
         and digested to bytes (`hashlib.sha512(testcase).digest()`)
 
         Args:
             tried: Set of already tried testcase hashes.
         """
         self._tried.update(frozenset(tried))
 
-    def get_tried(self) -> FrozenSet[str]:
+    def get_tried(self) -> FrozenSet[bytes]:
         """Return the set of tried testcase hashes. Testcases are hashed with SHA-512
         and digested to bytes (`hashlib.sha512(testcase).digest()`)
 
         Returns:
             Testcase hashes.
         """
         return frozenset(self._tried)
@@ -113,15 +113,15 @@
         # include before/after since different testcase types
         #   may split them inconsistently.
         tc_hasher = hashlib.sha512()
         tc_hasher.update(testcase.before)
         for part in testcase.parts:
             tc_hasher.update(part)
         tc_hasher.update(testcase.after)
-        tc_hash = tc_hasher.hexdigest()
+        tc_hash = tc_hasher.digest()
         if tc_hash not in self._tried:
             self._tried.add(tc_hash)
             self._last_success = None
             self._testcase_attempt = testcase
             self._description = description
             yield self._testcase_attempt
```

### Comparing `lithium-reducer-1.1.1/src/lithium/testcases.py` & `lithium-reducer-2.0.0/src/lithium/testcases.py`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/src/lithium/util.py` & `lithium-reducer-2.0.0/src/lithium/util.py`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/src/lithium_reducer.egg-info/PKG-INFO` & `lithium-reducer-2.0.0/src/lithium_reducer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lithium-reducer
-Version: 1.1.1
+Version: 2.0.0
 Summary: Lithium is an automated testcase reduction tool
 Home-page: https://github.com/MozillaSecurity/lithium
 Author: Jesse Ruderman
 Maintainer: Mozilla Fuzzing Team
 Maintainer-email: fuzzing@mozilla.com
 License: MPL 2.0
 Keywords: fuzz,fuzzing,reduce,reducer,reduction,security,test,testing
```

### Comparing `lithium-reducer-1.1.1/src/lithium_reducer.egg-info/SOURCES.txt` & `lithium-reducer-2.0.0/src/lithium_reducer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/src/lithium_reducer.egg-info/entry_points.txt` & `lithium-reducer-2.0.0/src/lithium_reducer.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/tests/conftest.py` & `lithium-reducer-2.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/tests/test_interestingness.py` & `lithium-reducer-2.0.0/tests/test_interestingness.py`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/tests/test_lithium.py` & `lithium-reducer-2.0.0/tests/test_lithium.py`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/tests/test_strategies.py` & `lithium-reducer-2.0.0/tests/test_strategies.py`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/tests/test_testcases.py` & `lithium-reducer-2.0.0/tests/test_testcases.py`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/tests/test_util.py` & `lithium-reducer-2.0.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `lithium-reducer-1.1.1/tox.ini` & `lithium-reducer-2.0.0/tox.ini`

 * *Files identical despite different names*

