# Comparing `tmp/backports_tarfile-1.1.0.tar.gz` & `tmp/backports_tarfile-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backports_tarfile-1.1.0.tar", last modified: Tue Apr 16 11:32:03 2024, max compression
+gzip compressed data, was "backports_tarfile-1.1.1.tar", last modified: Mon Apr 22 19:26:35 2024, max compression
```

## Comparing `backports_tarfile-1.1.0.tar` & `backports_tarfile-1.1.1.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:32:03.292290 backports_tarfile-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:32:03.284290 backports_tarfile-1.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:32:03.284290 backports_tarfile-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-16 11:32:03.292290 backports_tarfile-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:32:03.280290 backports_tarfile-1.1.0/backports/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:32:03.284290 backports_tarfile-1.1.0/backports/tarfile/
--rwxr-xr-x   0 runner    (1001) docker     (127)   106960 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/backports/tarfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/backports/tarfile/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:32:03.288290 backports_tarfile-1.1.0/backports/tarfile/compat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/backports/tarfile/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/backports/tarfile/compat/py38.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:32:03.292290 backports_tarfile-1.1.0/backports.tarfile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-16 11:32:03.000000 backports_tarfile-1.1.0/backports.tarfile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-16 11:32:03.000000 backports_tarfile-1.1.0/backports.tarfile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 11:32:03.000000 backports_tarfile-1.1.0/backports.tarfile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-16 11:32:03.000000 backports_tarfile-1.1.0/backports.tarfile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 11:32:03.000000 backports_tarfile-1.1.0/backports.tarfile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:32:03.288290 backports_tarfile-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-16 11:32:03.292290 backports_tarfile-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:32:03.288290 backports_tarfile-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:32:03.288290 backports_tarfile-1.1.0/tests/compat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/compat/archiver_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/compat/py310.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/compat/py38.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/compat/py39.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/recursion.tar
--rw-r--r--   0 runner    (1001) docker     (127)   162773 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/test_tarfile.py
--rw-r--r--   0 runner    (1001) docker     (127)   435200 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/testtar.tar
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/testtar.tar.xz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:32:03.292290 backports_tarfile-1.1.0/tests/tokenizedata/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/tokenizedata/tokenize_tests-no-coding-cookie-and-utf8-bom-sig-only.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/tokenizedata/tokenize_tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/zipdir.zip
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:26:35.600912 backports_tarfile-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:26:35.592912 backports_tarfile-1.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:26:35.592912 backports_tarfile-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-22 19:26:35.600912 backports_tarfile-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:26:35.592912 backports_tarfile-1.1.1/backports/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/backports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:26:35.596912 backports_tarfile-1.1.1/backports/tarfile/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   106960 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/backports/tarfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/backports/tarfile/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:26:35.596912 backports_tarfile-1.1.1/backports/tarfile/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/backports/tarfile/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/backports/tarfile/compat/py38.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:26:35.600912 backports_tarfile-1.1.1/backports.tarfile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-22 19:26:35.000000 backports_tarfile-1.1.1/backports.tarfile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-22 19:26:35.000000 backports_tarfile-1.1.1/backports.tarfile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:26:35.000000 backports_tarfile-1.1.1/backports.tarfile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-22 19:26:35.000000 backports_tarfile-1.1.1/backports.tarfile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-22 19:26:35.000000 backports_tarfile-1.1.1/backports.tarfile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:26:35.596912 backports_tarfile-1.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 19:26:35.600912 backports_tarfile-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:26:35.596912 backports_tarfile-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:26:35.600912 backports_tarfile-1.1.1/tests/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/tests/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/tests/compat/archiver_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/tests/compat/py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/tests/compat/py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/tests/compat/py39.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/tests/recursion.tar
+-rw-r--r--   0 runner    (1001) docker     (127)   162773 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/tests/test_tarfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)   435200 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/tests/testtar.tar
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/tests/testtar.tar.xz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:26:35.600912 backports_tarfile-1.1.1/tests/tokenizedata/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/tests/tokenizedata/tokenize_tests-no-coding-cookie-and-utf8-bom-sig-only.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/tests/tokenizedata/tokenize_tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/tests/zipdir.zip
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-22 19:26:16.000000 backports_tarfile-1.1.1/tox.ini
```

### Comparing `backports_tarfile-1.1.0/.github/workflows/main.yml` & `backports_tarfile-1.1.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `backports_tarfile-1.1.0/LICENSE` & `backports_tarfile-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `backports_tarfile-1.1.0/PKG-INFO` & `backports_tarfile-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: backports.tarfile
-Version: 1.1.0
+Version: 1.1.1
 Summary: Backport of CPython tarfile module
-Home-page: https://github.com/jaraco/backports.tarfile
-Author: Jason R. Coombs
-Author-email: jaraco@jaraco.com
+Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
+Project-URL: Homepage, https://github.com/jaraco/backports.tarfile
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Provides-Extra: testing
-Requires-Dist: pytest!=8.1.1,>=6; extra == "testing"
+Requires-Dist: pytest!=8.1.*,>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
 Requires-Dist: jaraco.test; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.5; extra == "docs"
 Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
```

### Comparing `backports_tarfile-1.1.0/README.rst` & `backports_tarfile-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `backports_tarfile-1.1.0/backports/tarfile/__init__.py` & `backports_tarfile-1.1.1/backports/tarfile/__init__.py`

 * *Files identical despite different names*

### Comparing `backports_tarfile-1.1.0/backports/tarfile/compat/py38.py` & `backports_tarfile-1.1.1/backports/tarfile/compat/py38.py`

 * *Files identical despite different names*

### Comparing `backports_tarfile-1.1.0/backports.tarfile.egg-info/PKG-INFO` & `backports_tarfile-1.1.1/backports.tarfile.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: backports.tarfile
-Version: 1.1.0
+Version: 1.1.1
 Summary: Backport of CPython tarfile module
-Home-page: https://github.com/jaraco/backports.tarfile
-Author: Jason R. Coombs
-Author-email: jaraco@jaraco.com
+Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
+Project-URL: Homepage, https://github.com/jaraco/backports.tarfile
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Provides-Extra: testing
-Requires-Dist: pytest!=8.1.1,>=6; extra == "testing"
+Requires-Dist: pytest!=8.1.*,>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
 Requires-Dist: jaraco.test; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.5; extra == "docs"
 Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
```

### Comparing `backports_tarfile-1.1.0/backports.tarfile.egg-info/SOURCES.txt` & `backports_tarfile-1.1.1/backports.tarfile.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 NEWS.rst
 README.rst
 conftest.py
 mypy.ini
 pyproject.toml
 pytest.ini
 ruff.toml
-setup.cfg
 towncrier.toml
 tox.ini
 .github/dependabot.yml
 .github/workflows/main.yml
+backports/__init__.py
 backports.tarfile.egg-info/PKG-INFO
 backports.tarfile.egg-info/SOURCES.txt
 backports.tarfile.egg-info/dependency_links.txt
 backports.tarfile.egg-info/requires.txt
 backports.tarfile.egg-info/top_level.txt
 backports/tarfile/__init__.py
 backports/tarfile/__main__.py
```

### Comparing `backports_tarfile-1.1.0/conftest.py` & `backports_tarfile-1.1.1/conftest.py`

 * *Files identical despite different names*

### Comparing `backports_tarfile-1.1.0/docs/conf.py` & `backports_tarfile-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `backports_tarfile-1.1.0/pytest.ini` & `backports_tarfile-1.1.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `backports_tarfile-1.1.0/tests/compat/archiver_tests.py` & `backports_tarfile-1.1.1/tests/compat/archiver_tests.py`

 * *Files identical despite different names*

### Comparing `backports_tarfile-1.1.0/tests/compat/py310.py` & `backports_tarfile-1.1.1/tests/compat/py310.py`

 * *Files identical despite different names*

### Comparing `backports_tarfile-1.1.0/tests/compat/py38.py` & `backports_tarfile-1.1.1/tests/compat/py38.py`

 * *Files identical despite different names*

### Comparing `backports_tarfile-1.1.0/tests/compat/py39.py` & `backports_tarfile-1.1.1/tests/compat/py39.py`

 * *Files identical despite different names*

### Comparing `backports_tarfile-1.1.0/tests/test_tarfile.py` & `backports_tarfile-1.1.1/tests/test_tarfile.py`

 * *Files identical despite different names*

### Comparing `backports_tarfile-1.1.0/tests/testtar.tar` & `backports_tarfile-1.1.1/tests/testtar.tar`

 * *Files identical despite different names*

### Comparing `backports_tarfile-1.1.0/tests/tokenizedata/tokenize_tests.txt` & `backports_tarfile-1.1.1/tests/tokenizedata/tokenize_tests.txt`

 * *Files identical despite different names*

### Comparing `backports_tarfile-1.1.0/tox.ini` & `backports_tarfile-1.1.1/tox.ini`

 * *Files identical despite different names*

