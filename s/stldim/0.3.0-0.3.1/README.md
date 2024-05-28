# Comparing `tmp/stldim-0.3.0.tar.gz` & `tmp/stldim-0.3.1.tar.gz`

## Comparing `stldim-0.3.0.tar` & `stldim-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 stldim-0.3.0/Makefile
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 stldim-0.3.0/dev-requirements.txt
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 stldim-0.3.0/requirements.txt
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 stldim-0.3.0/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 stldim-0.3.0/.github/workflows/pytest.yml
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 stldim-0.3.0/.github/workflows/pytest_coverage.yml
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 stldim-0.3.0/src/stldim/__init__.py
--rwxr-xr-x   0        0        0     1319 2020-02-02 00:00:00.000000 stldim-0.3.0/src/stldim/__main__.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 stldim-0.3.0/src/stldim/version.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 stldim-0.3.0/src/stldim/templates/openscad_lib.jinja2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stldim-0.3.0/src/stldim/tests/__init__.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 stldim-0.3.0/src/stldim/tests/test_get_varname.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 stldim-0.3.0/src/stldim/tests/test_mesh_with_bounds.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 stldim-0.3.0/src/stldim/tests/test_sanitize_filename.py
--rw-r--r--   0        0        0 11285384 2020-02-02 00:00:00.000000 stldim-0.3.0/tests/3DBenchy.stl
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 stldim-0.3.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 stldim-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 stldim-0.3.0/README.md
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 stldim-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 stldim-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 stldim-0.3.1/Makefile
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 stldim-0.3.1/dev-requirements.txt
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 stldim-0.3.1/requirements.txt
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 stldim-0.3.1/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 stldim-0.3.1/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 stldim-0.3.1/.github/workflows/pytest_coverage.yml
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 stldim-0.3.1/src/stldim/__init__.py
+-rwxr-xr-x   0        0        0     1317 2020-02-02 00:00:00.000000 stldim-0.3.1/src/stldim/__main__.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 stldim-0.3.1/src/stldim/version.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 stldim-0.3.1/src/stldim/templates/openscad_lib.jinja2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stldim-0.3.1/src/stldim/tests/__init__.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 stldim-0.3.1/src/stldim/tests/test_get_varname.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 stldim-0.3.1/src/stldim/tests/test_mesh_with_bounds.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 stldim-0.3.1/src/stldim/tests/test_sanitize_filename.py
+-rw-r--r--   0        0        0 11285384 2020-02-02 00:00:00.000000 stldim-0.3.1/tests/3DBenchy.stl
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 stldim-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 stldim-0.3.1/LICENSE.md
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 stldim-0.3.1/README.md
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 stldim-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 stldim-0.3.1/PKG-INFO
```

### Comparing `stldim-0.3.0/.github/workflows/pylint.yml` & `stldim-0.3.1/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `stldim-0.3.0/.github/workflows/pytest.yml` & `stldim-0.3.1/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `stldim-0.3.0/.github/workflows/pytest_coverage.yml` & `stldim-0.3.1/.github/workflows/pytest_coverage.yml`

 * *Files identical despite different names*

### Comparing `stldim-0.3.0/src/stldim/__init__.py` & `stldim-0.3.1/src/stldim/__init__.py`

 * *Files identical despite different names*

### Comparing `stldim-0.3.0/src/stldim/__main__.py` & `stldim-0.3.1/src/stldim/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
 from stldim import MeshWithBounds, get_varname, version
 
 def generate_openscad_lib(stl_dimensions, varname, stlfile):
     """
     Generate an OpenSCAD library file with the dimensions of the STL file
     """
-    environment = jinja2.Environment(loader=jinja2.FileSystemLoader('.'))
-    template = environment.get_template('stldim/templates/openscad_lib.jinja2')
+    environment = jinja2.Environment(loader=jinja2.PackageLoader('stldim', 'templates'))
+    template = environment.get_template('openscad_lib.jinja2')
     print(template.render(stl_dimensions=stl_dimensions, varname=varname, stlfile=stlfile))
 
 def main():
     """
     Main function
     """
     args = docopt(__doc__, version=version.__str__)
```

### Comparing `stldim-0.3.0/src/stldim/templates/openscad_lib.jinja2` & `stldim-0.3.1/src/stldim/templates/openscad_lib.jinja2`

 * *Files identical despite different names*

### Comparing `stldim-0.3.0/src/stldim/tests/test_mesh_with_bounds.py` & `stldim-0.3.1/src/stldim/tests/test_mesh_with_bounds.py`

 * *Files identical despite different names*

### Comparing `stldim-0.3.0/src/stldim/tests/test_sanitize_filename.py` & `stldim-0.3.1/src/stldim/tests/test_sanitize_filename.py`

 * *Files identical despite different names*

### Comparing `stldim-0.3.0/tests/3DBenchy.stl` & `stldim-0.3.1/tests/3DBenchy.stl`

 * *Files identical despite different names*

### Comparing `stldim-0.3.0/LICENSE.md` & `stldim-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stldim-0.3.0/README.md` & `stldim-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `stldim-0.3.0/pyproject.toml` & `stldim-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stldim-0.3.0/PKG-INFO` & `stldim-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: stldim
-Version: 0.3.0
+Version: 0.3.1
 Summary: Get dimensions of an STL file
 Project-URL: Homepage, https://github.com/nomike/stldim
 Project-URL: Issues, https://github.com/nomike/stldim/issues
 Author-email: nomike Postmann <nomike@nomike.com>
 License-File: LICENSE.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

