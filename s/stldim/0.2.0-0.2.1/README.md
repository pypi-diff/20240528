# Comparing `tmp/stldim-0.2.0.tar.gz` & `tmp/stldim-0.2.1.tar.gz`

## Comparing `stldim-0.2.0.tar` & `stldim-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 stldim-0.2.0/Makefile
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 stldim-0.2.0/requirements.txt
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 stldim-0.2.0/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 stldim-0.2.0/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 stldim-0.2.0/src/stldim/__init__.py
--rwxr-xr-x   0        0        0     3630 2020-02-02 00:00:00.000000 stldim-0.2.0/src/stldim/__main__.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 stldim-0.2.0/src/stldim/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stldim-0.2.0/src/stldim/tests/__init__.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 stldim-0.2.0/src/stldim/tests/test_get_varname.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 stldim-0.2.0/src/stldim/tests/test_mesh_with_bounds.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 stldim-0.2.0/src/stldim/tests/test_sanitize_filename.py
--rw-r--r--   0        0        0 11285384 2020-02-02 00:00:00.000000 stldim-0.2.0/tests/3DBenchy.stl
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 stldim-0.2.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 stldim-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 stldim-0.2.0/README.md
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 stldim-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 stldim-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 stldim-0.2.1/Makefile
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 stldim-0.2.1/dev-requirements.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 stldim-0.2.1/requirements.txt
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 stldim-0.2.1/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 stldim-0.2.1/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 stldim-0.2.1/.github/workflows/pytest_coverage.yml
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 stldim-0.2.1/src/stldim/__init__.py
+-rwxr-xr-x   0        0        0     3630 2020-02-02 00:00:00.000000 stldim-0.2.1/src/stldim/__main__.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 stldim-0.2.1/src/stldim/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stldim-0.2.1/src/stldim/tests/__init__.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 stldim-0.2.1/src/stldim/tests/test_get_varname.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 stldim-0.2.1/src/stldim/tests/test_mesh_with_bounds.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 stldim-0.2.1/src/stldim/tests/test_sanitize_filename.py
+-rw-r--r--   0        0        0 11285384 2020-02-02 00:00:00.000000 stldim-0.2.1/tests/3DBenchy.stl
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 stldim-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 stldim-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 stldim-0.2.1/README.md
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 stldim-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 stldim-0.2.1/PKG-INFO
```

### Comparing `stldim-0.2.0/.github/workflows/pylint.yml` & `stldim-0.2.1/.github/workflows/pylint.yml`

 * *Files 26% similar despite different names*

```diff
@@ -7,19 +7,19 @@
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -r requirements.txt
-        pip install pylint pytest
+        pip install -r dev-requirements.txt
 
     - name: Analysing the code with pylint
       run: |
         pylint --max-statements=70 $(git ls-files '*.py')
```

### Comparing `stldim-0.2.0/.github/workflows/pytest.yml` & `stldim-0.2.1/.github/workflows/pytest.yml`

 * *Files 26% similar despite different names*

```diff
@@ -7,19 +7,19 @@
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -r requirements.txt
-        pip install pytest
+        pip install -r dev-requirements.txt
 
     - name: Test the code with pytest
       run: |
         pytest
```

### Comparing `stldim-0.2.0/src/stldim/__init__.py` & `stldim-0.2.1/src/stldim/__init__.py`

 * *Files identical despite different names*

### Comparing `stldim-0.2.0/src/stldim/__main__.py` & `stldim-0.2.1/src/stldim/__main__.py`

 * *Files identical despite different names*

### Comparing `stldim-0.2.0/src/stldim/tests/test_mesh_with_bounds.py` & `stldim-0.2.1/src/stldim/tests/test_mesh_with_bounds.py`

 * *Files identical despite different names*

### Comparing `stldim-0.2.0/src/stldim/tests/test_sanitize_filename.py` & `stldim-0.2.1/src/stldim/tests/test_sanitize_filename.py`

 * *Files identical despite different names*

### Comparing `stldim-0.2.0/tests/3DBenchy.stl` & `stldim-0.2.1/tests/3DBenchy.stl`

 * *Files identical despite different names*

### Comparing `stldim-0.2.0/LICENSE.md` & `stldim-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stldim-0.2.0/README.md` & `stldim-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `stldim-0.2.0/pyproject.toml` & `stldim-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stldim-0.2.0/PKG-INFO` & `stldim-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: stldim
-Version: 0.2.0
+Version: 0.2.1
 Summary: Get dimensions of an STL file
 Project-URL: Homepage, https://github.com/nomike/stldim
 Project-URL: Issues, https://github.com/nomike/stldim/issues
 Author-email: nomike Postmann <nomike@nomike.com>
 License-File: LICENSE.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

