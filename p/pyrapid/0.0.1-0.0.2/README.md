# Comparing `tmp/pyrapid-0.0.1.tar.gz` & `tmp/pyrapid-0.0.2.tar.gz`

## Comparing `pyrapid-0.0.1.tar` & `pyrapid-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pyrapid-0.0.1/.python-version
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 pyrapid-0.0.1/requirements-dev.lock
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pyrapid-0.0.1/requirements.lock
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pyrapid-0.0.1/src/r/main.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyrapid-0.0.1/.gitignore
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 pyrapid-0.0.1/README.md
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 pyrapid-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 pyrapid-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pyrapid-0.0.2/.python-version
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 pyrapid-0.0.2/requirements-dev.lock
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pyrapid-0.0.2/requirements.lock
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 pyrapid-0.0.2/src/r/main.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyrapid-0.0.2/.gitignore
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 pyrapid-0.0.2/README.md
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 pyrapid-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pyrapid-0.0.2/PKG-INFO
```

### Comparing `pyrapid-0.0.1/pyproject.toml` & `pyrapid-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyrapid"
-version = "0.0.1"
+version = "0.0.2"
 description = "Build native apps in Python"
 authors = [
     { name = "Avetik Kazhoyan", email = "kazhoyan@gmail.com" }
 ]
 dependencies = []
 readme = "README.md"
 requires-python = ">= 3.12.3"
```

### Comparing `pyrapid-0.0.1/PKG-INFO` & `pyrapid-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.3
 Name: pyrapid
-Version: 0.0.1
+Version: 0.0.2
 Summary: Build native apps in Python
 Author-email: Avetik Kazhoyan <kazhoyan@gmail.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12.3
 Description-Content-Type: text/markdown
 
 # pyrapid
 Build native apps in Python.
 
-[![PyPI - Version](https://img.shields.io/pypi/v/r.svg)](https://pypi.org/project/r)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/r.svg)](https://pypi.org/project/r)
+[![PyPI - Version](https://img.shields.io/pypi/v/pyrapid.svg)](https://pypi.org/project/pyrapid)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyrapid.svg)](https://pypi.org/project/pyrapid)
 
 -----
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [License](#license)
```

