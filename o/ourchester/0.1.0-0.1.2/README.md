# Comparing `tmp/ourchester-0.1.0.tar.gz` & `tmp/ourchester-0.1.2.tar.gz`

## Comparing `ourchester-0.1.0.tar` & `ourchester-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ourchester-0.1.0/Makefile
--rwxr-xr-x   0        0        0     1206 2020-02-02 00:00:00.000000 ourchester-0.1.0/make_txtar.sh
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ourchester-0.1.0/ourchester.code-workspace
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 ourchester-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 ourchester-0.1.0/requirements.lock
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 ourchester-0.1.0/src/ourchester/__init__.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 ourchester-0.1.0/src/ourchester/cli.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 ourchester-0.1.0/src/ourchester/indexer.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 ourchester-0.1.0/src/ourchester/log.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 ourchester-0.1.0/src/ourchester/searcher.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ourchester-0.1.0/testdata/file1.md
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 ourchester-0.1.0/testdata/file10.md
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ourchester-0.1.0/testdata/file2.md
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 ourchester-0.1.0/testdata/file3.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ourchester-0.1.0/testdata/file4.md
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 ourchester-0.1.0/testdata/file5.md
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 ourchester-0.1.0/testdata/file6.md
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ourchester-0.1.0/testdata/file7.md
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ourchester-0.1.0/testdata/file8.md
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ourchester-0.1.0/testdata/file9.md
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 ourchester-0.1.0/.gitignore
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 ourchester-0.1.0/README.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 ourchester-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ourchester-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 ourchester-0.1.2/.bumpversion.cfg
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 ourchester-0.1.2/Makefile
+-rwxr-xr-x   0        0        0     1206 2020-02-02 00:00:00.000000 ourchester-0.1.2/make_txtar.sh
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ourchester-0.1.2/ourchester.code-workspace
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 ourchester-0.1.2/requirements-dev.lock
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 ourchester-0.1.2/requirements.lock
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 ourchester-0.1.2/src/ourchester/__init__.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 ourchester-0.1.2/src/ourchester/cli.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 ourchester-0.1.2/src/ourchester/indexer.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 ourchester-0.1.2/src/ourchester/log.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 ourchester-0.1.2/src/ourchester/searcher.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ourchester-0.1.2/testdata/file1.md
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 ourchester-0.1.2/testdata/file10.md
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ourchester-0.1.2/testdata/file2.md
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 ourchester-0.1.2/testdata/file3.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ourchester-0.1.2/testdata/file4.md
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 ourchester-0.1.2/testdata/file5.md
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 ourchester-0.1.2/testdata/file6.md
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 ourchester-0.1.2/testdata/file7.md
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ourchester-0.1.2/testdata/file8.md
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ourchester-0.1.2/testdata/file9.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ourchester-0.1.2/.gitignore
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 ourchester-0.1.2/README.md
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 ourchester-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 ourchester-0.1.2/PKG-INFO
```

### Comparing `ourchester-0.1.0/make_txtar.sh` & `ourchester-0.1.2/make_txtar.sh`

 * *Files identical despite different names*

### Comparing `ourchester-0.1.0/requirements-dev.lock` & `ourchester-0.1.2/requirements-dev.lock`

 * *Files 17% similar despite different names*

```diff
@@ -27,11 +27,12 @@
     # via black
 packaging==24.0
     # via black
 pathspec==0.12.1
     # via black
 platformdirs==4.2.2
     # via black
+    # via ourchester
 pytimeparse==1.1.8
     # via fishhoof
 whoosh==2.7.4
     # via ourchester
```

### Comparing `ourchester-0.1.0/src/ourchester/__init__.py` & `ourchester-0.1.2/src/ourchester/__init__.py`

 * *Files identical despite different names*

### Comparing `ourchester-0.1.0/src/ourchester/cli.py` & `ourchester-0.1.2/src/ourchester/cli.py`

 * *Files identical despite different names*

### Comparing `ourchester-0.1.0/src/ourchester/indexer.py` & `ourchester-0.1.2/src/ourchester/indexer.py`

 * *Files identical despite different names*

### Comparing `ourchester-0.1.0/pyproject.toml` & `ourchester-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [project]
 name = "ourchester"
-version = "0.1.0"
+version = "0.1.2"
 description = "Add your description here"
 authors = [
     { name = "Taylor Monacelli", email = "taylormonacelli@gmail.com" }
 ]
 dependencies = [
     "jinja2>=3.1.3",
     "whoosh>=2.7.4",
     "ivylantern>=0.1.0",
     "fishhoof>=0.0.2",
+    "platformdirs>=4.2.2",
 ]
 readme = "README.md"
 requires-python = ">= 3.12"
 
 [project.scripts]
 ourchester = "ourchester:main"
```

### Comparing `ourchester-0.1.0/PKG-INFO` & `ourchester-0.1.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.3
 Name: ourchester
-Version: 0.1.0
+Version: 0.1.2
 Summary: Add your description here
 Author-email: Taylor Monacelli <taylormonacelli@gmail.com>
 Requires-Python: >=3.12
 Requires-Dist: fishhoof>=0.0.2
 Requires-Dist: ivylantern>=0.1.0
 Requires-Dist: jinja2>=3.1.3
+Requires-Dist: platformdirs>=4.2.2
 Requires-Dist: whoosh>=2.7.4
 Description-Content-Type: text/markdown
 
 # ourchester
 
 ## Usage example
```

