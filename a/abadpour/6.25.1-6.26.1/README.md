# Comparing `tmp/abadpour-6.25.1.tar.gz` & `tmp/abadpour-6.26.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abadpour-6.25.1.tar", last modified: Sun May 26 22:00:01 2024, max compression
+gzip compressed data, was "abadpour-6.26.1.tar", last modified: Tue May 28 01:37:18 2024, max compression
```

## Comparing `abadpour-6.25.1.tar` & `abadpour-6.26.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 22:00:01.196024 abadpour-6.25.1/
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-26 17:51:52.000000 abadpour-6.25.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     1156 2024-05-26 22:00:01.195568 abadpour-6.25.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      502 2024-05-26 17:51:52.000000 abadpour-6.25.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 22:00:01.188200 abadpour-6.25.1/abadpour/
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 22:00:01.193877 abadpour-6.25.1/abadpour/.abcli/
--rwxr-xr-x   0 kamangir   (502) staff       (20)      267 2024-05-26 17:51:52.000000 abadpour-6.25.1/abadpour/.abcli/CV.sh
--rw-r--r--   0 kamangir   (502) staff       (20)       95 2024-05-26 17:51:52.000000 abadpour-6.25.1/abadpour/.abcli/abcli.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      134 2024-05-26 17:51:52.000000 abadpour-6.25.1/abadpour/.abcli/actions.sh
--rw-r--r--   0 kamangir   (502) staff       (20)       56 2024-05-26 17:51:52.000000 abadpour-6.25.1/abadpour/.abcli/aka.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1315 2024-05-26 17:51:52.000000 abadpour-6.25.1/abadpour/.abcli/build.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      353 2024-05-26 17:51:52.000000 abadpour-6.25.1/abadpour/.abcli/clean.sh
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 22:00:01.194537 abadpour-6.25.1/abadpour/.abcli/tests/
--rw-r--r--   0 kamangir   (502) staff       (20)      204 2024-05-26 17:51:52.000000 abadpour-6.25.1/abadpour/.abcli/tests/build.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      198 2024-05-26 17:51:52.000000 abadpour-6.25.1/abadpour/.abcli/tests/version.sh
--rw-r--r--   0 kamangir   (502) staff       (20)       99 2024-05-26 21:59:55.000000 abadpour-6.25.1/abadpour/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      573 2024-05-26 17:51:52.000000 abadpour-6.25.1/abadpour/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      211 2024-05-26 17:51:52.000000 abadpour-6.25.1/abadpour/build.py
--rw-r--r--   0 kamangir   (502) staff       (20)       89 2024-05-26 17:51:52.000000 abadpour-6.25.1/abadpour/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-26 17:51:52.000000 abadpour-6.25.1/abadpour/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-26 22:00:01.194898 abadpour-6.25.1/abadpour.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     1156 2024-05-26 22:00:01.000000 abadpour-6.25.1/abadpour.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      528 2024-05-26 22:00:01.000000 abadpour-6.25.1/abadpour.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-26 22:00:01.000000 abadpour-6.25.1/abadpour.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       79 2024-05-26 22:00:01.000000 abadpour-6.25.1/abadpour.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-05-26 22:00:01.000000 abadpour-6.25.1/abadpour.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-26 17:51:52.000000 abadpour-6.25.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)       78 2024-05-26 17:51:52.000000 abadpour-6.25.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-26 22:00:01.196129 abadpour-6.25.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      333 2024-05-26 20:37:26.000000 abadpour-6.25.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-28 01:37:18.703690 abadpour-6.26.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-26 17:51:52.000000 abadpour-6.26.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     1156 2024-05-28 01:37:18.703067 abadpour-6.26.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      502 2024-05-26 17:51:52.000000 abadpour-6.26.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-28 01:37:18.696212 abadpour-6.26.1/abadpour/
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-28 01:37:18.700867 abadpour-6.26.1/abadpour/.abcli/
+-rwxr-xr-x   0 kamangir   (502) staff       (20)      267 2024-05-26 17:51:52.000000 abadpour-6.26.1/abadpour/.abcli/CV.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)       95 2024-05-26 17:51:52.000000 abadpour-6.26.1/abadpour/.abcli/abcli.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      134 2024-05-26 17:51:52.000000 abadpour-6.26.1/abadpour/.abcli/actions.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)       56 2024-05-26 17:51:52.000000 abadpour-6.26.1/abadpour/.abcli/aka.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1315 2024-05-26 17:51:52.000000 abadpour-6.26.1/abadpour/.abcli/build.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      353 2024-05-26 17:51:52.000000 abadpour-6.26.1/abadpour/.abcli/clean.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-28 01:37:18.701763 abadpour-6.26.1/abadpour/.abcli/tests/
+-rw-r--r--   0 kamangir   (502) staff       (20)      204 2024-05-26 17:51:52.000000 abadpour-6.26.1/abadpour/.abcli/tests/build.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      212 2024-05-28 01:33:19.000000 abadpour-6.26.1/abadpour/.abcli/tests/version.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)       99 2024-05-28 01:37:13.000000 abadpour-6.26.1/abadpour/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      573 2024-05-26 17:51:52.000000 abadpour-6.26.1/abadpour/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      211 2024-05-26 17:51:52.000000 abadpour-6.26.1/abadpour/build.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       89 2024-05-26 17:51:52.000000 abadpour-6.26.1/abadpour/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-26 17:51:52.000000 abadpour-6.26.1/abadpour/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-28 01:37:18.702398 abadpour-6.26.1/abadpour.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     1156 2024-05-28 01:37:18.000000 abadpour-6.26.1/abadpour.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      528 2024-05-28 01:37:18.000000 abadpour-6.26.1/abadpour.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-28 01:37:18.000000 abadpour-6.26.1/abadpour.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       79 2024-05-28 01:37:18.000000 abadpour-6.26.1/abadpour.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-05-28 01:37:18.000000 abadpour-6.26.1/abadpour.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-26 17:51:52.000000 abadpour-6.26.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)       78 2024-05-26 17:51:52.000000 abadpour-6.26.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-28 01:37:18.703815 abadpour-6.26.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      333 2024-05-26 20:37:26.000000 abadpour-6.26.1/setup.py
```

### Comparing `abadpour-6.25.1/PKG-INFO` & `abadpour-6.26.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abadpour
-Version: 6.25.1
+Version: 6.26.1
 Summary: 📜 Arash Abadpour's CV.
 Home-page: https://github.com/kamangir/CV
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `abadpour-6.25.1/abadpour/.abcli/build.sh` & `abadpour-6.26.1/abadpour/.abcli/build.sh`

 * *Files identical despite different names*

### Comparing `abadpour-6.25.1/abadpour/__main__.py` & `abadpour-6.26.1/abadpour/__main__.py`

 * *Files identical despite different names*

### Comparing `abadpour-6.25.1/abadpour.egg-info/PKG-INFO` & `abadpour-6.26.1/abadpour.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abadpour
-Version: 6.25.1
+Version: 6.26.1
 Summary: 📜 Arash Abadpour's CV.
 Home-page: https://github.com/kamangir/CV
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `abadpour-6.25.1/abadpour.egg-info/SOURCES.txt` & `abadpour-6.26.1/abadpour.egg-info/SOURCES.txt`

 * *Files identical despite different names*

