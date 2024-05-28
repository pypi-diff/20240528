# Comparing `tmp/stldim-0.2.2.tar.gz` & `tmp/stldim-0.3.0.tar.gz`

## Comparing `stldim-0.2.2.tar` & `stldim-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 stldim-0.2.2/Makefile
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 stldim-0.2.2/dev-requirements.txt
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 stldim-0.2.2/requirements.txt
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 stldim-0.2.2/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 stldim-0.2.2/.github/workflows/pytest.yml
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 stldim-0.2.2/.github/workflows/pytest_coverage.yml
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 stldim-0.2.2/src/stldim/__init__.py
--rwxr-xr-x   0        0        0     3134 2020-02-02 00:00:00.000000 stldim-0.2.2/src/stldim/__main__.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 stldim-0.2.2/src/stldim/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stldim-0.2.2/src/stldim/tests/__init__.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 stldim-0.2.2/src/stldim/tests/test_get_varname.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 stldim-0.2.2/src/stldim/tests/test_mesh_with_bounds.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 stldim-0.2.2/src/stldim/tests/test_sanitize_filename.py
--rw-r--r--   0        0        0 11285384 2020-02-02 00:00:00.000000 stldim-0.2.2/tests/3DBenchy.stl
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 stldim-0.2.2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 stldim-0.2.2/LICENSE.md
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 stldim-0.2.2/README.md
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 stldim-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 stldim-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 stldim-0.3.0/Makefile
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 stldim-0.3.0/dev-requirements.txt
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 stldim-0.3.0/requirements.txt
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 stldim-0.3.0/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 stldim-0.3.0/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 stldim-0.3.0/.github/workflows/pytest_coverage.yml
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 stldim-0.3.0/src/stldim/__init__.py
+-rwxr-xr-x   0        0        0     1319 2020-02-02 00:00:00.000000 stldim-0.3.0/src/stldim/__main__.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 stldim-0.3.0/src/stldim/version.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 stldim-0.3.0/src/stldim/templates/openscad_lib.jinja2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stldim-0.3.0/src/stldim/tests/__init__.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 stldim-0.3.0/src/stldim/tests/test_get_varname.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 stldim-0.3.0/src/stldim/tests/test_mesh_with_bounds.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 stldim-0.3.0/src/stldim/tests/test_sanitize_filename.py
+-rw-r--r--   0        0        0 11285384 2020-02-02 00:00:00.000000 stldim-0.3.0/tests/3DBenchy.stl
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 stldim-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 stldim-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 stldim-0.3.0/README.md
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 stldim-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 stldim-0.3.0/PKG-INFO
```

### Comparing `stldim-0.2.2/.github/workflows/pylint.yml` & `stldim-0.3.0/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `stldim-0.2.2/.github/workflows/pytest.yml` & `stldim-0.3.0/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `stldim-0.2.2/.github/workflows/pytest_coverage.yml` & `stldim-0.3.0/.github/workflows/pytest_coverage.yml`

 * *Files identical despite different names*

### Comparing `stldim-0.2.2/src/stldim/__init__.py` & `stldim-0.3.0/src/stldim/__init__.py`

 * *Files identical despite different names*

### Comparing `stldim-0.2.2/src/stldim/tests/test_mesh_with_bounds.py` & `stldim-0.3.0/src/stldim/tests/test_mesh_with_bounds.py`

 * *Files identical despite different names*

### Comparing `stldim-0.2.2/src/stldim/tests/test_sanitize_filename.py` & `stldim-0.3.0/src/stldim/tests/test_sanitize_filename.py`

 * *Files identical despite different names*

### Comparing `stldim-0.2.2/tests/3DBenchy.stl` & `stldim-0.3.0/tests/3DBenchy.stl`

 * *Files identical despite different names*

### Comparing `stldim-0.2.2/LICENSE.md` & `stldim-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stldim-0.2.2/README.md` & `stldim-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `stldim-0.2.2/pyproject.toml` & `stldim-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 authors = [
     { name="nomike Postmann", email="nomike@nomike.com" },
 ]
 dependencies = [
     "docopt",
     "numpy-stl",
+    "jinja2",
 ]
 description = "Get dimensions of an STL file"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
@@ -36,7 +37,12 @@
 
 [project.urls]
 Homepage = "https://github.com/nomike/stldim"
 Issues = "https://github.com/nomike/stldim/issues"
 
 [tool.hatch.version]
 path = "src/stldim/version.py"
+
+[tool.pytest.ini_options]
+filterwarnings = [
+    "ignore::FutureWarning",
+]
```

### Comparing `stldim-0.2.2/PKG-INFO` & `stldim-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: stldim
-Version: 0.2.2
+Version: 0.3.0
 Summary: Get dimensions of an STL file
 Project-URL: Homepage, https://github.com/nomike/stldim
 Project-URL: Issues, https://github.com/nomike/stldim/issues
 Author-email: nomike Postmann <nomike@nomike.com>
 License-File: LICENSE.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: docopt
+Requires-Dist: jinja2
 Requires-Dist: numpy-stl
 Description-Content-Type: text/markdown
 
 # stldim
 
 A tool for mesuring the dimensions of an STL file.
```

