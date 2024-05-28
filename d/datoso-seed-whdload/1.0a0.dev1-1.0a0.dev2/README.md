# Comparing `tmp/datoso_seed_whdload-1.0a0.dev1.tar.gz` & `tmp/datoso_seed_whdload-1.0a0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso_seed_whdload-1.0a0.dev1.tar", last modified: Tue May 28 01:04:30 2024, max compression
+gzip compressed data, was "datoso_seed_whdload-1.0a0.dev2.tar", last modified: Tue May 28 01:11:40 2024, max compression
```

## Comparing `datoso_seed_whdload-1.0a0.dev1.tar` & `datoso_seed_whdload-1.0a0.dev2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:04:30.113327 datoso_seed_whdload-1.0a0.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-28 01:04:24.000000 datoso_seed_whdload-1.0a0.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-28 01:04:30.113327 datoso_seed_whdload-1.0a0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-28 01:04:24.000000 datoso_seed_whdload-1.0a0.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-28 01:04:24.000000 datoso_seed_whdload-1.0a0.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-28 01:04:30.113327 datoso_seed_whdload-1.0a0.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:04:30.109326 datoso_seed_whdload-1.0a0.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:04:30.113327 datoso_seed_whdload-1.0a0.dev1/src/datoso_seed_whdload/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-28 01:04:24.000000 datoso_seed_whdload-1.0a0.dev1/src/datoso_seed_whdload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-28 01:04:24.000000 datoso_seed_whdload-1.0a0.dev1/src/datoso_seed_whdload/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-28 01:04:24.000000 datoso_seed_whdload-1.0a0.dev1/src/datoso_seed_whdload/dats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-28 01:04:24.000000 datoso_seed_whdload-1.0a0.dev1/src/datoso_seed_whdload/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-28 01:04:24.000000 datoso_seed_whdload-1.0a0.dev1/src/datoso_seed_whdload/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:04:30.113327 datoso_seed_whdload-1.0a0.dev1/src/datoso_seed_whdload.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-28 01:04:30.000000 datoso_seed_whdload-1.0a0.dev1/src/datoso_seed_whdload.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-28 01:04:30.000000 datoso_seed_whdload-1.0a0.dev1/src/datoso_seed_whdload.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:04:30.000000 datoso_seed_whdload-1.0a0.dev1/src/datoso_seed_whdload.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 01:04:30.000000 datoso_seed_whdload-1.0a0.dev1/src/datoso_seed_whdload.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 01:04:30.000000 datoso_seed_whdload-1.0a0.dev1/src/datoso_seed_whdload.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:11:40.881752 datoso_seed_whdload-1.0a0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-28 01:11:31.000000 datoso_seed_whdload-1.0a0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-28 01:11:40.881752 datoso_seed_whdload-1.0a0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-28 01:11:31.000000 datoso_seed_whdload-1.0a0.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-28 01:11:31.000000 datoso_seed_whdload-1.0a0.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-28 01:11:40.885752 datoso_seed_whdload-1.0a0.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:11:40.881752 datoso_seed_whdload-1.0a0.dev2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:11:40.881752 datoso_seed_whdload-1.0a0.dev2/src/datoso_seed_whdload/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-28 01:11:31.000000 datoso_seed_whdload-1.0a0.dev2/src/datoso_seed_whdload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-28 01:11:31.000000 datoso_seed_whdload-1.0a0.dev2/src/datoso_seed_whdload/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-28 01:11:31.000000 datoso_seed_whdload-1.0a0.dev2/src/datoso_seed_whdload/dats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-28 01:11:31.000000 datoso_seed_whdload-1.0a0.dev2/src/datoso_seed_whdload/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-28 01:11:31.000000 datoso_seed_whdload-1.0a0.dev2/src/datoso_seed_whdload/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:11:40.881752 datoso_seed_whdload-1.0a0.dev2/src/datoso_seed_whdload.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-28 01:11:40.000000 datoso_seed_whdload-1.0a0.dev2/src/datoso_seed_whdload.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-28 01:11:40.000000 datoso_seed_whdload-1.0a0.dev2/src/datoso_seed_whdload.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:11:40.000000 datoso_seed_whdload-1.0a0.dev2/src/datoso_seed_whdload.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 01:11:40.000000 datoso_seed_whdload-1.0a0.dev2/src/datoso_seed_whdload.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 01:11:40.000000 datoso_seed_whdload-1.0a0.dev2/src/datoso_seed_whdload.egg-info/top_level.txt
```

### Comparing `datoso_seed_whdload-1.0a0.dev1/LICENSE` & `datoso_seed_whdload-1.0a0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso_seed_whdload-1.0a0.dev1/PKG-INFO` & `datoso_seed_whdload-1.0a0.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso_seed_whdload
-Version: 1.0a0.dev1
+Version: 1.0a0.dev2
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_whdload
 Keywords: emulators,roms
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `datoso_seed_whdload-1.0a0.dev1/README.md` & `datoso_seed_whdload-1.0a0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `datoso_seed_whdload-1.0a0.dev1/pyproject.toml` & `datoso_seed_whdload-1.0a0.dev2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Environment :: Console",
     'License :: OSI Approved :: MIT License',
     "Operating System :: POSIX :: Linux",
     'Programming Language :: Python :: 3',
     'Topic :: System :: Emulators',
 ]
 dependencies = [
-    "datoso>=1.0a0.dev1",
+    "datoso>=1.0a0.dev2",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Source Code"       = "https://github.com/laromicas/datoso_seed_whdload"
 
 [tool.setuptools]
```

### Comparing `datoso_seed_whdload-1.0a0.dev1/src/datoso_seed_whdload/dats.py` & `datoso_seed_whdload-1.0a0.dev2/src/datoso_seed_whdload/dats.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_whdload-1.0a0.dev1/src/datoso_seed_whdload/fetch.py` & `datoso_seed_whdload-1.0a0.dev2/src/datoso_seed_whdload/fetch.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_whdload-1.0a0.dev1/src/datoso_seed_whdload/rules.py` & `datoso_seed_whdload-1.0a0.dev2/src/datoso_seed_whdload/rules.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_whdload-1.0a0.dev1/src/datoso_seed_whdload.egg-info/PKG-INFO` & `datoso_seed_whdload-1.0a0.dev2/src/datoso_seed_whdload.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso-seed-whdload
-Version: 1.0a0.dev1
+Version: 1.0a0.dev2
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_whdload
 Keywords: emulators,roms
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

