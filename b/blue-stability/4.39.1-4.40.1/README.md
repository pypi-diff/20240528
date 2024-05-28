# Comparing `tmp/blue_stability-4.39.1.tar.gz` & `tmp/blue_stability-4.40.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blue_stability-4.39.1.tar", last modified: Tue May 28 01:06:16 2024, max compression
+gzip compressed data, was "blue_stability-4.40.1.tar", last modified: Tue May 28 01:32:13 2024, max compression
```

## Comparing `blue_stability-4.39.1.tar` & `blue_stability-4.40.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-28 01:06:16.170496 blue_stability-4.39.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2022-12-05 02:50:06.000000 blue_stability-4.39.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-24 02:08:53.000000 blue_stability-4.39.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     2846 2024-05-28 01:06:16.170019 blue_stability-4.39.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     1831 2024-03-04 07:34:46.000000 blue_stability-4.39.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-28 01:06:16.164907 blue_stability-4.39.1/blue_stability/
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-28 01:06:16.168438 blue_stability-4.39.1/blue_stability/.abcli/
--rw-r--r--   0 kamangir   (502) staff       (20)      158 2024-05-26 18:58:00.000000 blue_stability-4.39.1/blue_stability/.abcli/actions.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      321 2024-05-26 18:58:00.000000 blue_stability-4.39.1/blue_stability/.abcli/aiart.sh
--rw-r--r--   0 kamangir   (502) staff       (20)       65 2024-05-26 18:58:00.000000 blue_stability-4.39.1/blue_stability/.abcli/aka.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)      855 2024-05-26 18:58:00.000000 blue_stability-4.39.1/blue_stability/.abcli/blue_stability.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1393 2024-05-26 18:58:00.000000 blue_stability-4.39.1/blue_stability/.abcli/generate_function.sh
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-28 01:06:16.168757 blue_stability-4.39.1/blue_stability/.abcli/tests/
--rw-r--r--   0 kamangir   (502) staff       (20)      222 2024-05-26 18:58:00.000000 blue_stability-4.39.1/blue_stability/.abcli/tests/version.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      121 2024-05-28 01:06:11.000000 blue_stability-4.39.1/blue_stability/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      255 2024-05-28 00:59:55.000000 blue_stability-4.39.1/blue_stability/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       95 2024-03-24 00:16:18.000000 blue_stability-4.39.1/blue_stability/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2022-12-05 02:50:06.000000 blue_stability-4.39.1/blue_stability/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-28 01:06:16.169294 blue_stability-4.39.1/blue_stability.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     2846 2024-05-28 01:06:16.000000 blue_stability-4.39.1/blue_stability.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      576 2024-05-28 01:06:16.000000 blue_stability-4.39.1/blue_stability.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-28 01:06:16.000000 blue_stability-4.39.1/blue_stability.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      157 2024-05-28 01:06:16.000000 blue_stability-4.39.1/blue_stability.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       15 2024-05-28 01:06:16.000000 blue_stability-4.39.1/blue_stability.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-24 02:08:53.000000 blue_stability-4.39.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      157 2024-05-25 01:42:30.000000 blue_stability-4.39.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-28 01:06:16.170578 blue_stability-4.39.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      352 2024-05-26 20:36:16.000000 blue_stability-4.39.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-28 01:32:13.173737 blue_stability-4.40.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2022-12-05 02:50:06.000000 blue_stability-4.40.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-24 02:08:53.000000 blue_stability-4.40.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     2846 2024-05-28 01:32:13.173174 blue_stability-4.40.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     1831 2024-03-04 07:34:46.000000 blue_stability-4.40.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-28 01:32:13.167696 blue_stability-4.40.1/blue_stability/
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-28 01:32:13.171749 blue_stability-4.40.1/blue_stability/.abcli/
+-rw-r--r--   0 kamangir   (502) staff       (20)      158 2024-05-26 18:58:00.000000 blue_stability-4.40.1/blue_stability/.abcli/actions.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      321 2024-05-26 18:58:00.000000 blue_stability-4.40.1/blue_stability/.abcli/aiart.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)       65 2024-05-26 18:58:00.000000 blue_stability-4.40.1/blue_stability/.abcli/aka.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)      855 2024-05-26 18:58:00.000000 blue_stability-4.40.1/blue_stability/.abcli/blue_stability.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1393 2024-05-26 18:58:00.000000 blue_stability-4.40.1/blue_stability/.abcli/generate_function.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-28 01:32:13.172142 blue_stability-4.40.1/blue_stability/.abcli/tests/
+-rw-r--r--   0 kamangir   (502) staff       (20)      222 2024-05-26 18:58:00.000000 blue_stability-4.40.1/blue_stability/.abcli/tests/version.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      121 2024-05-28 01:32:07.000000 blue_stability-4.40.1/blue_stability/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      255 2024-05-28 00:59:55.000000 blue_stability-4.40.1/blue_stability/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       95 2024-03-24 00:16:18.000000 blue_stability-4.40.1/blue_stability/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2022-12-05 02:50:06.000000 blue_stability-4.40.1/blue_stability/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-28 01:32:13.172596 blue_stability-4.40.1/blue_stability.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     2846 2024-05-28 01:32:13.000000 blue_stability-4.40.1/blue_stability.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      576 2024-05-28 01:32:13.000000 blue_stability-4.40.1/blue_stability.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-28 01:32:13.000000 blue_stability-4.40.1/blue_stability.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      157 2024-05-28 01:32:13.000000 blue_stability-4.40.1/blue_stability.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       15 2024-05-28 01:32:13.000000 blue_stability-4.40.1/blue_stability.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-24 02:08:53.000000 blue_stability-4.40.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      157 2024-05-25 01:42:30.000000 blue_stability-4.40.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-28 01:32:13.173836 blue_stability-4.40.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      352 2024-05-26 20:36:16.000000 blue_stability-4.40.1/setup.py
```

### Comparing `blue_stability-4.39.1/LICENSE` & `blue_stability-4.40.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blue_stability-4.39.1/PKG-INFO` & `blue_stability-4.40.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blue_stability
-Version: 4.39.1
+Version: 4.40.1
 Summary: 🟦 a command interface to stability.ai.
 Home-page: https://github.com/kamangir/blue-stability
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `blue_stability-4.39.1/README.md` & `blue_stability-4.40.1/README.md`

 * *Files identical despite different names*

### Comparing `blue_stability-4.39.1/blue_stability/.abcli/blue_stability.sh` & `blue_stability-4.40.1/blue_stability/.abcli/blue_stability.sh`

 * *Files identical despite different names*

### Comparing `blue_stability-4.39.1/blue_stability/.abcli/generate_function.sh` & `blue_stability-4.40.1/blue_stability/.abcli/generate_function.sh`

 * *Files identical despite different names*

### Comparing `blue_stability-4.39.1/blue_stability.egg-info/PKG-INFO` & `blue_stability-4.40.1/blue_stability.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blue_stability
-Version: 4.39.1
+Version: 4.40.1
 Summary: 🟦 a command interface to stability.ai.
 Home-page: https://github.com/kamangir/blue-stability
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `blue_stability-4.39.1/blue_stability.egg-info/SOURCES.txt` & `blue_stability-4.40.1/blue_stability.egg-info/SOURCES.txt`

 * *Files identical despite different names*

