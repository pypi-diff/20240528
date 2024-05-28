# Comparing `tmp/stldim-0.2.1.tar.gz` & `tmp/stldim-0.2.2.tar.gz`

## Comparing `stldim-0.2.1.tar` & `stldim-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 stldim-0.2.1/Makefile
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 stldim-0.2.1/dev-requirements.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 stldim-0.2.1/requirements.txt
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 stldim-0.2.1/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 stldim-0.2.1/.github/workflows/pytest.yml
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 stldim-0.2.1/.github/workflows/pytest_coverage.yml
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 stldim-0.2.1/src/stldim/__init__.py
--rwxr-xr-x   0        0        0     3630 2020-02-02 00:00:00.000000 stldim-0.2.1/src/stldim/__main__.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 stldim-0.2.1/src/stldim/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stldim-0.2.1/src/stldim/tests/__init__.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 stldim-0.2.1/src/stldim/tests/test_get_varname.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 stldim-0.2.1/src/stldim/tests/test_mesh_with_bounds.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 stldim-0.2.1/src/stldim/tests/test_sanitize_filename.py
--rw-r--r--   0        0        0 11285384 2020-02-02 00:00:00.000000 stldim-0.2.1/tests/3DBenchy.stl
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 stldim-0.2.1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 stldim-0.2.1/LICENSE.md
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 stldim-0.2.1/README.md
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 stldim-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 stldim-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 stldim-0.2.2/Makefile
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 stldim-0.2.2/dev-requirements.txt
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 stldim-0.2.2/requirements.txt
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 stldim-0.2.2/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 stldim-0.2.2/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 stldim-0.2.2/.github/workflows/pytest_coverage.yml
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 stldim-0.2.2/src/stldim/__init__.py
+-rwxr-xr-x   0        0        0     3134 2020-02-02 00:00:00.000000 stldim-0.2.2/src/stldim/__main__.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 stldim-0.2.2/src/stldim/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stldim-0.2.2/src/stldim/tests/__init__.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 stldim-0.2.2/src/stldim/tests/test_get_varname.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 stldim-0.2.2/src/stldim/tests/test_mesh_with_bounds.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 stldim-0.2.2/src/stldim/tests/test_sanitize_filename.py
+-rw-r--r--   0        0        0 11285384 2020-02-02 00:00:00.000000 stldim-0.2.2/tests/3DBenchy.stl
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 stldim-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 stldim-0.2.2/LICENSE.md
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 stldim-0.2.2/README.md
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 stldim-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 stldim-0.2.2/PKG-INFO
```

### Comparing `stldim-0.2.1/.github/workflows/pylint.yml` & `stldim-0.2.2/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `stldim-0.2.1/.github/workflows/pytest.yml` & `stldim-0.2.2/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `stldim-0.2.1/.github/workflows/pytest_coverage.yml` & `stldim-0.2.2/.github/workflows/pytest_coverage.yml`

 * *Files identical despite different names*

### Comparing `stldim-0.2.1/src/stldim/__init__.py` & `stldim-0.2.2/src/stldim/__init__.py`

 * *Files identical despite different names*

### Comparing `stldim-0.2.1/src/stldim/__main__.py` & `stldim-0.2.2/src/stldim/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,50 +7,39 @@
     Options:
         -h --help       Show this screen.
         --version       Show version.
         --name=<name>   Name of the object [defaults to the filename with non alpha-numeric\
 characters replaced with underscores].
 """
 
-import argparse
 import os
 import sys
 
-from stldim import version
-from stldim import get_varname, MeshWithBounds
+from docopt import docopt
+
+from stldim import MeshWithBounds, get_varname, version
 
 
 def main():
     """
     Main function
     """
+    args = docopt(__doc__, version=version.__str__)
 
-    parser = argparse.ArgumentParser(prog="stldim",
-                                     description="Get dimensions of an STL file")
-
-    parser.add_argument("stlfile", type=str, help="Path to the STL file")
-    parser.add_argument("--version", action="version",
-                        help="Show version", version=version.__str__)
-    parser.add_argument("--name", type=str, default=None,
-                        help="Name of the object (defaults to filename with special characters \
-                            replaced by underscores")
-
-    args = parser.parse_args()
-
-    if not os.path.exists(args.stlfile):
-        sys.exit(f'ERROR: file {args.stlfile} was not found!')
-    varname = get_varname(args.stlfile, args.name)
+    if not os.path.exists(args['<stlfile>']):
+        sys.exit(f"ERROR: file {args['<stlfile>']} was not found!")
+    varname = get_varname(args['<stlfile>'], args['--name'])
 
-    stl_dimensions = MeshWithBounds.from_file(args.stlfile)
+    stl_dimensions = MeshWithBounds.from_file(args['<stlfile>'])
 
 
 # the logic is easy from there
 
-    print("// File:", args.stlfile)
-    obj = ['\t\timport("', args.stlfile, '");']
+    print("// File:", args['<stlfile>'])
+    obj = ['\t\timport("', args['<stlfile>'], '");']
 
     print("// X size:", stl_dimensions['xsize'])
     print(f"{varname}_xsize = {stl_dimensions['xsize']};")
     print("// Y size:", stl_dimensions['ysize'])
     print(f"{varname}_ysize = {stl_dimensions['ysize']};")
     print("// Z size:", stl_dimensions['zsize'])
     print(f"{varname}_zsize = {stl_dimensions['zsize']};")
```

### Comparing `stldim-0.2.1/src/stldim/tests/test_mesh_with_bounds.py` & `stldim-0.2.2/src/stldim/tests/test_mesh_with_bounds.py`

 * *Files identical despite different names*

### Comparing `stldim-0.2.1/src/stldim/tests/test_sanitize_filename.py` & `stldim-0.2.2/src/stldim/tests/test_sanitize_filename.py`

 * *Files identical despite different names*

### Comparing `stldim-0.2.1/tests/3DBenchy.stl` & `stldim-0.2.2/tests/3DBenchy.stl`

 * *Files identical despite different names*

### Comparing `stldim-0.2.1/LICENSE.md` & `stldim-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stldim-0.2.1/README.md` & `stldim-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `stldim-0.2.1/pyproject.toml` & `stldim-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "stldim"
 dynamic = ["version"]
 
 authors = [
     { name="nomike Postmann", email="nomike@nomike.com" },
 ]
 dependencies = [
-    "argparse",
+    "docopt",
     "numpy-stl",
 ]
 description = "Get dimensions of an STL file"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `stldim-0.2.1/PKG-INFO` & `stldim-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: stldim
-Version: 0.2.1
+Version: 0.2.2
 Summary: Get dimensions of an STL file
 Project-URL: Homepage, https://github.com/nomike/stldim
 Project-URL: Issues, https://github.com/nomike/stldim/issues
 Author-email: nomike Postmann <nomike@nomike.com>
 License-File: LICENSE.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
-Requires-Dist: argparse
+Requires-Dist: docopt
 Requires-Dist: numpy-stl
 Description-Content-Type: text/markdown
 
 # stldim
 
 A tool for mesuring the dimensions of an STL file.
```

