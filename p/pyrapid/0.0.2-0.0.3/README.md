# Comparing `tmp/pyrapid-0.0.2.tar.gz` & `tmp/pyrapid-0.0.3.tar.gz`

## Comparing `pyrapid-0.0.2.tar` & `pyrapid-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pyrapid-0.0.2/.python-version
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 pyrapid-0.0.2/requirements-dev.lock
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pyrapid-0.0.2/requirements.lock
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pyrapid-0.0.2/src/r/main.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyrapid-0.0.2/.gitignore
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 pyrapid-0.0.2/README.md
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 pyrapid-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pyrapid-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pyrapid-0.0.3/.python-version
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 pyrapid-0.0.3/requirements-dev.lock
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pyrapid-0.0.3/requirements.lock
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pyrapid-0.0.3/src/r/main.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyrapid-0.0.3/.gitignore
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pyrapid-0.0.3/README.md
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 pyrapid-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 pyrapid-0.0.3/PKG-INFO
```

### Comparing `pyrapid-0.0.2/pyproject.toml` & `pyrapid-0.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyrapid"
-version = "0.0.2"
+version = "0.0.3"
 description = "Build native apps in Python"
 authors = [
     { name = "Avetik Kazhoyan", email = "kazhoyan@gmail.com" }
 ]
 dependencies = []
 readme = "README.md"
 requires-python = ">= 3.12.3"
```

### Comparing `pyrapid-0.0.2/PKG-INFO` & `pyrapid-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyrapid
-Version: 0.0.2
+Version: 0.0.3
 Summary: Build native apps in Python
 Author-email: Avetik Kazhoyan <kazhoyan@gmail.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12.3
@@ -22,13 +22,13 @@
 
 - [Installation](#installation)
 - [License](#license)
 
 ## Installation
 
 ```console
-pip install r
+pip install pyrapid
 ```
 
 ## License
 
-`r` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+`pyrapid` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

