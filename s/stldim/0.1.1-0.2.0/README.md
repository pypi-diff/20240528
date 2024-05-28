# Comparing `tmp/stldim-0.1.1.tar.gz` & `tmp/stldim-0.2.0.tar.gz`

## Comparing `stldim-0.1.1.tar` & `stldim-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 stldim-0.1.1/Makefile
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 stldim-0.1.1/requirements.txt
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 stldim-0.1.1/src/stldim/__init__.py
--rwxr-xr-x   0        0        0     3608 2020-02-02 00:00:00.000000 stldim-0.1.1/src/stldim/__main__.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 stldim-0.1.1/src/stldim/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stldim-0.1.1/src/stldim/tests/__init__.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 stldim-0.1.1/src/stldim/tests/test_find_mins_maxs.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 stldim-0.1.1/src/stldim/tests/test_get_stl_dimensions.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 stldim-0.1.1/src/stldim/tests/test_get_varname.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 stldim-0.1.1/src/stldim/tests/test_sanitize_filename.py
--rw-r--r--   0        0        0 11285384 2020-02-02 00:00:00.000000 stldim-0.1.1/tests/3DBenchy.stl
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 stldim-0.1.1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 stldim-0.1.1/LICENSE.md
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 stldim-0.1.1/README.md
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 stldim-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 stldim-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 stldim-0.2.0/Makefile
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 stldim-0.2.0/requirements.txt
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 stldim-0.2.0/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 stldim-0.2.0/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 stldim-0.2.0/src/stldim/__init__.py
+-rwxr-xr-x   0        0        0     3630 2020-02-02 00:00:00.000000 stldim-0.2.0/src/stldim/__main__.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 stldim-0.2.0/src/stldim/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stldim-0.2.0/src/stldim/tests/__init__.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 stldim-0.2.0/src/stldim/tests/test_get_varname.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 stldim-0.2.0/src/stldim/tests/test_mesh_with_bounds.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 stldim-0.2.0/src/stldim/tests/test_sanitize_filename.py
+-rw-r--r--   0        0        0 11285384 2020-02-02 00:00:00.000000 stldim-0.2.0/tests/3DBenchy.stl
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 stldim-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 stldim-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 stldim-0.2.0/README.md
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 stldim-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 stldim-0.2.0/PKG-INFO
```

### Comparing `stldim-0.1.1/src/stldim/__main__.py` & `stldim-0.2.0/src/stldim/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,47 +3,53 @@
     stldim - Get dimensions of an STL file
     Usage:
         stldim.py [options] <stlfile>
 
     Options:
         -h --help       Show this screen.
         --version       Show version.
-        --name=<name>   Name of the object [defaults to the filename with non alpha-numeric characters replaced with underscores].
+        --name=<name>   Name of the object [defaults to the filename with non alpha-numeric\
+characters replaced with underscores].
 """
 
 import argparse
 import os
 import sys
 
-import stldim.version as version
-from stldim import get_varname, get_stl_dimensions
+from stldim import version
+from stldim import get_varname, MeshWithBounds
+
 
 def main():
+    """
+    Main function
+    """
+
     parser = argparse.ArgumentParser(prog="stldim",
                                      description="Get dimensions of an STL file")
 
     parser.add_argument("stlfile", type=str, help="Path to the STL file")
     parser.add_argument("--version", action="version",
                         help="Show version", version=version.__str__)
     parser.add_argument("--name", type=str, default=None,
-                        help="Name of the object (defaults to filename with special characters replaced by underscores")
+                        help="Name of the object (defaults to filename with special characters \
+                            replaced by underscores")
 
     args = parser.parse_args()
 
     if not os.path.exists(args.stlfile):
-        sys.exit(f'ERROR: file args.stlfile was not found!')
+        sys.exit(f'ERROR: file {args.stlfile} was not found!')
     varname = get_varname(args.stlfile, args.name)
 
-    stl_dimensions = get_stl_dimensions(args.stlfile)
+    stl_dimensions = MeshWithBounds.from_file(args.stlfile)
 
 
 # the logic is easy from there
 
     print("// File:", args.stlfile)
-    lst = ['obj =("', args.stlfile, '");']
     obj = ['\t\timport("', args.stlfile, '");']
 
     print("// X size:", stl_dimensions['xsize'])
     print(f"{varname}_xsize = {stl_dimensions['xsize']};")
     print("// Y size:", stl_dimensions['ysize'])
     print(f"{varname}_ysize = {stl_dimensions['ysize']};")
     print("// Z size:", stl_dimensions['zsize'])
```

### Comparing `stldim-0.1.1/tests/3DBenchy.stl` & `stldim-0.2.0/tests/3DBenchy.stl`

 * *Files identical despite different names*

### Comparing `stldim-0.1.1/LICENSE.md` & `stldim-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stldim-0.1.1/README.md` & `stldim-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `stldim-0.1.1/pyproject.toml` & `stldim-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stldim-0.1.1/PKG-INFO` & `stldim-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: stldim
-Version: 0.1.1
+Version: 0.2.0
 Summary: Get dimensions of an STL file
 Project-URL: Homepage, https://github.com/nomike/stldim
 Project-URL: Issues, https://github.com/nomike/stldim/issues
 Author-email: nomike Postmann <nomike@nomike.com>
 License-File: LICENSE.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

