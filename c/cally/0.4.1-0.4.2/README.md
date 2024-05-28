# Comparing `tmp/cally-0.4.1.tar.gz` & `tmp/cally-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cally-0.4.1.tar", last modified: Tue May 28 09:11:50 2024, max compression
+gzip compressed data, was "cally-0.4.2.tar", last modified: Tue May 28 09:19:57 2024, max compression
```

## Comparing `cally-0.4.1.tar` & `cally-0.4.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:50.448250 cally-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-28 09:11:46.000000 cally-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    27576 2024-05-28 09:11:50.448250 cally-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-05-28 09:11:46.000000 cally-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-28 09:11:46.000000 cally-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 09:11:50.448250 cally-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:50.440250 cally-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:50.440250 cally-0.4.1/src/cally/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:50.444250 cally-0.4.1/src/cally/cdk/
--rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:50.444250 cally-0.4.1/src/cally/cdk/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cdk/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:50.444250 cally-0.4.1/src/cally/cdk/stacks/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cdk/stacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:50.444250 cally-0.4.1/src/cally/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:50.444250 cally-0.4.1/src/cally/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/commands/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/commands/tf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:50.444250 cally-0.4.1/src/cally/cli/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/config/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/config/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/config/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:50.448250 cally-0.4.1/src/cally/cli/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/tools/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/cli/tools/terraform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:50.448250 cally-0.4.1/src/cally/testing/
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/testing/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/testing/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:46.000000 cally-0.4.1/src/cally/testing/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:11:50.448250 cally-0.4.1/src/cally.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27576 2024-05-28 09:11:50.000000 cally-0.4.1/src/cally.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-28 09:11:50.000000 cally-0.4.1/src/cally.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:11:50.000000 cally-0.4.1/src/cally.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-28 09:11:50.000000 cally-0.4.1/src/cally.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-28 09:11:50.000000 cally-0.4.1/src/cally.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 09:11:50.000000 cally-0.4.1/src/cally.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:19:57.236372 cally-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-28 09:19:44.000000 cally-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    27576 2024-05-28 09:19:57.236372 cally-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-05-28 09:19:44.000000 cally-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-28 09:19:44.000000 cally-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 09:19:57.236372 cally-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:19:57.228372 cally-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:19:57.228372 cally-0.4.2/src/cally/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:19:57.232372 cally-0.4.2/src/cally/cdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-05-28 09:19:44.000000 cally-0.4.2/src/cally/cdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:19:44.000000 cally-0.4.2/src/cally/cdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:19:57.232372 cally-0.4.2/src/cally/cdk/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:19:44.000000 cally-0.4.2/src/cally/cdk/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:19:57.232372 cally-0.4.2/src/cally/cdk/stacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-28 09:19:44.000000 cally-0.4.2/src/cally/cdk/stacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:19:57.232372 cally-0.4.2/src/cally/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-28 09:19:44.000000 cally-0.4.2/src/cally/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 09:19:44.000000 cally-0.4.2/src/cally/cli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:19:57.232372 cally-0.4.2/src/cally/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:19:44.000000 cally-0.4.2/src/cally/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-28 09:19:44.000000 cally-0.4.2/src/cally/cli/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-28 09:19:44.000000 cally-0.4.2/src/cally/cli/commands/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-28 09:19:44.000000 cally-0.4.2/src/cally/cli/commands/tf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:19:57.232372 cally-0.4.2/src/cally/cli/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-28 09:19:44.000000 cally-0.4.2/src/cally/cli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-28 09:19:44.000000 cally-0.4.2/src/cally/cli/config/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-28 09:19:44.000000 cally-0.4.2/src/cally/cli/config/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-28 09:19:44.000000 cally-0.4.2/src/cally/cli/config/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-28 09:19:44.000000 cally-0.4.2/src/cally/cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:19:44.000000 cally-0.4.2/src/cally/cli/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:19:57.236372 cally-0.4.2/src/cally/cli/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:19:44.000000 cally-0.4.2/src/cally/cli/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-28 09:19:44.000000 cally-0.4.2/src/cally/cli/tools/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-28 09:19:44.000000 cally-0.4.2/src/cally/cli/tools/terraform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:19:57.236372 cally-0.4.2/src/cally/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-28 09:19:44.000000 cally-0.4.2/src/cally/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-28 09:19:44.000000 cally-0.4.2/src/cally/testing/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 09:19:44.000000 cally-0.4.2/src/cally/testing/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 09:19:44.000000 cally-0.4.2/src/cally/testing/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:19:57.236372 cally-0.4.2/src/cally.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27576 2024-05-28 09:19:57.000000 cally-0.4.2/src/cally.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-28 09:19:57.000000 cally-0.4.2/src/cally.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:19:57.000000 cally-0.4.2/src/cally.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-28 09:19:57.000000 cally-0.4.2/src/cally.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-28 09:19:57.000000 cally-0.4.2/src/cally.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 09:19:57.000000 cally-0.4.2/src/cally.egg-info/top_level.txt
```

### Comparing `cally-0.4.1/LICENSE` & `cally-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cally-0.4.1/PKG-INFO` & `cally-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cally
-Version: 0.4.1
+Version: 0.4.2
 Summary: A config as infrastructure foundation for your Internal Developer Platform
 Author-email: Leon Wright <techman83@gmail.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

### Comparing `cally-0.4.1/README.md` & `cally-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `cally-0.4.1/pyproject.toml` & `cally-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cally-0.4.1/src/cally/cdk/__init__.py` & `cally-0.4.2/src/cally/cdk/__init__.py`

 * *Files identical despite different names*

### Comparing `cally-0.4.1/src/cally/cdk/stacks/__init__.py` & `cally-0.4.2/src/cally/cdk/stacks/__init__.py`

 * *Files identical despite different names*

### Comparing `cally-0.4.1/src/cally/cli/__init__.py` & `cally-0.4.2/src/cally/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cally-0.4.1/src/cally/cli/commands/tf.py` & `cally-0.4.2/src/cally/cli/commands/tf.py`

 * *Files identical despite different names*

### Comparing `cally-0.4.1/src/cally/cli/config/__init__.py` & `cally-0.4.2/src/cally/cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cally-0.4.1/src/cally/cli/config/loader.py` & `cally-0.4.2/src/cally/cli/config/loader.py`

 * *Files identical despite different names*

### Comparing `cally-0.4.1/src/cally/cli/config/types.py` & `cally-0.4.2/src/cally/cli/config/types.py`

 * *Files identical despite different names*

### Comparing `cally-0.4.1/src/cally/cli/config/validators.py` & `cally-0.4.2/src/cally/cli/config/validators.py`

 * *Files identical despite different names*

### Comparing `cally-0.4.1/src/cally/cli/constants.py` & `cally-0.4.2/src/cally/cli/constants.py`

 * *Files identical despite different names*

### Comparing `cally-0.4.1/src/cally/cli/tools/provider.py` & `cally-0.4.2/src/cally/cli/tools/provider.py`

 * *Files identical despite different names*

### Comparing `cally-0.4.1/src/cally/cli/tools/terraform.py` & `cally-0.4.2/src/cally/cli/tools/terraform.py`

 * *Files identical despite different names*

### Comparing `cally-0.4.1/src/cally/testing/__init__.py` & `cally-0.4.2/src/cally/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `cally-0.4.1/src/cally.egg-info/PKG-INFO` & `cally-0.4.2/src/cally.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cally
-Version: 0.4.1
+Version: 0.4.2
 Summary: A config as infrastructure foundation for your Internal Developer Platform
 Author-email: Leon Wright <techman83@gmail.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

### Comparing `cally-0.4.1/src/cally.egg-info/SOURCES.txt` & `cally-0.4.2/src/cally.egg-info/SOURCES.txt`

 * *Files identical despite different names*

