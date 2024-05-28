# Comparing `tmp/stldim-0.3.1.tar.gz` & `tmp/stldim-0.3.2.tar.gz`

## Comparing `stldim-0.3.1.tar` & `stldim-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 stldim-0.3.1/Makefile
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 stldim-0.3.1/dev-requirements.txt
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 stldim-0.3.1/requirements.txt
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 stldim-0.3.1/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 stldim-0.3.1/.github/workflows/pytest.yml
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 stldim-0.3.1/.github/workflows/pytest_coverage.yml
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 stldim-0.3.1/src/stldim/__init__.py
--rwxr-xr-x   0        0        0     1317 2020-02-02 00:00:00.000000 stldim-0.3.1/src/stldim/__main__.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 stldim-0.3.1/src/stldim/version.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 stldim-0.3.1/src/stldim/templates/openscad_lib.jinja2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stldim-0.3.1/src/stldim/tests/__init__.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 stldim-0.3.1/src/stldim/tests/test_get_varname.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 stldim-0.3.1/src/stldim/tests/test_mesh_with_bounds.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 stldim-0.3.1/src/stldim/tests/test_sanitize_filename.py
--rw-r--r--   0        0        0 11285384 2020-02-02 00:00:00.000000 stldim-0.3.1/tests/3DBenchy.stl
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 stldim-0.3.1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 stldim-0.3.1/LICENSE.md
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 stldim-0.3.1/README.md
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 stldim-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 stldim-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 stldim-0.3.2/Makefile
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 stldim-0.3.2/dev-requirements.txt
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 stldim-0.3.2/requirements.txt
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 stldim-0.3.2/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 stldim-0.3.2/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 stldim-0.3.2/.github/workflows/pytest_coverage.yml
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 stldim-0.3.2/src/stldim/__init__.py
+-rwxr-xr-x   0        0        0     1317 2020-02-02 00:00:00.000000 stldim-0.3.2/src/stldim/__main__.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 stldim-0.3.2/src/stldim/version.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 stldim-0.3.2/src/stldim/templates/openscad_lib.jinja2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stldim-0.3.2/src/stldim/tests/__init__.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 stldim-0.3.2/src/stldim/tests/test_get_varname.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 stldim-0.3.2/src/stldim/tests/test_mesh_with_bounds.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 stldim-0.3.2/src/stldim/tests/test_sanitize_filename.py
+-rw-r--r--   0        0        0 11285384 2020-02-02 00:00:00.000000 stldim-0.3.2/tests/3DBenchy.stl
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 stldim-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 stldim-0.3.2/LICENSE.md
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 stldim-0.3.2/README.md
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 stldim-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 stldim-0.3.2/PKG-INFO
```

### Comparing `stldim-0.3.1/.github/workflows/pylint.yml` & `stldim-0.3.2/.github/workflows/pylint.yml`

 * *Files 3% similar despite different names*

```diff
@@ -18,8 +18,8 @@
       run: |
         python -m pip install --upgrade pip
         pip install -r requirements.txt
         pip install -r dev-requirements.txt
 
     - name: Analysing the code with pylint
       run: |
-        pylint --max-statements=70 $(git ls-files '*.py')
+        pylint $(git ls-files '*.py')
```

### Comparing `stldim-0.3.1/.github/workflows/pytest.yml` & `stldim-0.3.2/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `stldim-0.3.1/.github/workflows/pytest_coverage.yml` & `stldim-0.3.2/.github/workflows/pytest_coverage.yml`

 * *Files identical despite different names*

### Comparing `stldim-0.3.1/src/stldim/__init__.py` & `stldim-0.3.2/src/stldim/__init__.py`

 * *Files identical despite different names*

### Comparing `stldim-0.3.1/src/stldim/__main__.py` & `stldim-0.3.2/src/stldim/__main__.py`

 * *Files identical despite different names*

### Comparing `stldim-0.3.1/src/stldim/templates/openscad_lib.jinja2` & `stldim-0.3.2/src/stldim/templates/openscad_lib.jinja2`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 // File: {{ stlfile }}
-obj = ['\t\timport("', stlfile, '");']
 
-{{ varname }}_xsize = {{ stl_dimensions['xsize'] }}
-{{ varname }}_ysize = {{ stl_dimensions['ysize'] }}
-{{ varname }}_zsize = {{ stl_dimensions['zsize'] }}
-{{ varname }}_xposition = {{ stl_dimensions['minx'] }}
-{{ varname }}_yposition = {{ stl_dimensions['miny'] }}
-{{ varname }}_zposition = {{ stl_dimensions['minz'] }}
+{{ varname }}_xsize = {{ stl_dimensions['xsize'] }};
+{{ varname }}_ysize = {{ stl_dimensions['ysize'] }};
+{{ varname }}_zsize = {{ stl_dimensions['zsize'] }};
+{{ varname }}_xposition = {{ stl_dimensions['minx'] }};
+{{ varname }}_yposition = {{ stl_dimensions['miny'] }};
+{{ varname }}_zposition = {{ stl_dimensions['minz'] }};
 
 
-# --------------------
 NE=1; NW=2; SW=3; SE=4; CTR=5; CTRXY=6;
 
 module {{varname}}_obj2origin (where) {
     if (where == NE) {
         {{varname}}_objNE ();
     }
 
     if (where == NW) {
-        translate(-{{stl_dimensions['xsize']}},0,0])
+        translate([-{{stl_dimensions['xsize']}},0,0])
         {{varname}}_objNE ();
     }
 
     if (where == SW) {
-        translate(-{{stl_dimensions['xsize']}},-{{stl_dimensions['xsize']}},0])
+        translate([-{{stl_dimensions['xsize']}},-{{stl_dimensions['xsize']}},0])
         {{varname}}_objNE ();
     }
 
     if (where == SE) {
         translate([0,-{{stl_dimensions['ysize']}},0])
         {{varname}}_objNE ();
     }
```

### Comparing `stldim-0.3.1/src/stldim/tests/test_mesh_with_bounds.py` & `stldim-0.3.2/src/stldim/tests/test_mesh_with_bounds.py`

 * *Files identical despite different names*

### Comparing `stldim-0.3.1/src/stldim/tests/test_sanitize_filename.py` & `stldim-0.3.2/src/stldim/tests/test_sanitize_filename.py`

 * *Files identical despite different names*

### Comparing `stldim-0.3.1/tests/3DBenchy.stl` & `stldim-0.3.2/tests/3DBenchy.stl`

 * *Files identical despite different names*

### Comparing `stldim-0.3.1/LICENSE.md` & `stldim-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stldim-0.3.1/README.md` & `stldim-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `stldim-0.3.1/pyproject.toml` & `stldim-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stldim-0.3.1/PKG-INFO` & `stldim-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: stldim
-Version: 0.3.1
+Version: 0.3.2
 Summary: Get dimensions of an STL file
 Project-URL: Homepage, https://github.com/nomike/stldim
 Project-URL: Issues, https://github.com/nomike/stldim/issues
 Author-email: nomike Postmann <nomike@nomike.com>
 License-File: LICENSE.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

