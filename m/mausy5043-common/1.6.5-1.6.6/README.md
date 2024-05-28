# Comparing `tmp/mausy5043_common-1.6.5.tar.gz` & `tmp/mausy5043_common-1.6.6.tar.gz`

## Comparing `mausy5043_common-1.6.5.tar` & `mausy5043_common-1.6.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/.editorconfig
--rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/.pylintrc
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/BUILDING.md
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/environment.yml
--rwxr-xr-x   0        0        0     2292 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/mkbld
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/requirements.txt
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/tox.ini
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/.github/dependabot.yml
--rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/src/mausy5043_common/__init__.py
--rwxr-xr-x   0        0        0     1089 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/src/mausy5043_common/funfile.py
--rwxr-xr-x   0        0        0     1419 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/src/mausy5043_common/funmeteo.py
--rwxr-xr-x   0        0        0      700 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/src/mausy5043_common/libsignals.py
--rwxr-xr-x   0        0        0     9000 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/src/mausy5043_common/libsqlite3.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/src/mausy5043_common/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/tests/.placeholder
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/LICENSE
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/README.md
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/pyproject.toml
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 mausy5043_common-1.6.5/PKG-INFO
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 mausy5043_common-1.6.6/.editorconfig
+-rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 mausy5043_common-1.6.6/.pylintrc
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 mausy5043_common-1.6.6/BUILDING.md
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 mausy5043_common-1.6.6/environment.yml
+-rwxr-xr-x   0        0        0     2292 2020-02-02 00:00:00.000000 mausy5043_common-1.6.6/mkbld
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 mausy5043_common-1.6.6/requirements.txt
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 mausy5043_common-1.6.6/tox.ini
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 mausy5043_common-1.6.6/.github/dependabot.yml
+-rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 mausy5043_common-1.6.6/src/mausy5043_common/__init__.py
+-rwxr-xr-x   0        0        0     1089 2020-02-02 00:00:00.000000 mausy5043_common-1.6.6/src/mausy5043_common/funfile.py
+-rwxr-xr-x   0        0        0     1419 2020-02-02 00:00:00.000000 mausy5043_common-1.6.6/src/mausy5043_common/funmeteo.py
+-rwxr-xr-x   0        0        0      700 2020-02-02 00:00:00.000000 mausy5043_common-1.6.6/src/mausy5043_common/libsignals.py
+-rwxr-xr-x   0        0        0     9000 2020-02-02 00:00:00.000000 mausy5043_common-1.6.6/src/mausy5043_common/libsqlite3.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mausy5043_common-1.6.6/src/mausy5043_common/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mausy5043_common-1.6.6/tests/.placeholder
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 mausy5043_common-1.6.6/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mausy5043_common-1.6.6/LICENSE
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 mausy5043_common-1.6.6/README.md
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 mausy5043_common-1.6.6/pyproject.toml
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 mausy5043_common-1.6.6/PKG-INFO
```

### Comparing `mausy5043_common-1.6.5/.pylintrc` & `mausy5043_common-1.6.6/.pylintrc`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.6.5/BUILDING.md` & `mausy5043_common-1.6.6/BUILDING.md`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.6.5/mkbld` & `mausy5043_common-1.6.6/mkbld`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.6.5/tox.ini` & `mausy5043_common-1.6.6/tox.ini`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.6.5/src/mausy5043_common/funfile.py` & `mausy5043_common-1.6.6/src/mausy5043_common/funfile.py`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.6.5/src/mausy5043_common/funmeteo.py` & `mausy5043_common-1.6.6/src/mausy5043_common/funmeteo.py`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.6.5/src/mausy5043_common/libsignals.py` & `mausy5043_common-1.6.6/src/mausy5043_common/libsignals.py`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.6.5/src/mausy5043_common/libsqlite3.py` & `mausy5043_common-1.6.6/src/mausy5043_common/libsqlite3.py`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.6.5/.gitignore` & `mausy5043_common-1.6.6/.gitignore`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.6.5/LICENSE` & `mausy5043_common-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.6.5/README.md` & `mausy5043_common-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `mausy5043_common-1.6.5/pyproject.toml` & `mausy5043_common-1.6.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mausy5043-common"
-version = "1.6.5"  # latest production version
+version = "1.6.6"  # latest production version
 # version = "1.5.4" # latest test version
 description = "Common python functions"
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 authors = [
   { name="Mausy5043" },
```

### Comparing `mausy5043_common-1.6.5/PKG-INFO` & `mausy5043_common-1.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mausy5043-common
-Version: 1.6.5
+Version: 1.6.6
 Summary: Common python functions
 Project-URL: Homepage, https://github.com/Mausy5043/mausy5043-common
 Project-URL: Bug Tracker, https://github.com/Mausy5043/mausy5043-common/issues
 Author: Mausy5043
 License-Expression: MIT
 License-File: LICENSE
 Keywords: Raspberry Pi,private
```

