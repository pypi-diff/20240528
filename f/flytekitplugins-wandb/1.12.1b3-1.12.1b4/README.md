# Comparing `tmp/flytekitplugins_wandb-1.12.1b3.tar.gz` & `tmp/flytekitplugins_wandb-1.12.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins_wandb-1.12.1b3.tar", last modified: Wed May 22 18:21:16 2024, max compression
+gzip compressed data, was "flytekitplugins_wandb-1.12.1b4.tar", last modified: Tue May 28 15:50:31 2024, max compression
```

## Comparing `flytekitplugins_wandb-1.12.1b3.tar` & `flytekitplugins_wandb-1.12.1b4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:16.666911 flytekitplugins_wandb-1.12.1b3/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-22 18:21:16.666911 flytekitplugins_wandb-1.12.1b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-22 18:20:42.000000 flytekitplugins_wandb-1.12.1b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:16.666911 flytekitplugins_wandb-1.12.1b3/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:16.666911 flytekitplugins_wandb-1.12.1b3/flytekitplugins/wandb/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-22 18:20:42.000000 flytekitplugins_wandb-1.12.1b3/flytekitplugins/wandb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-22 18:20:42.000000 flytekitplugins_wandb-1.12.1b3/flytekitplugins/wandb/tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:16.666911 flytekitplugins_wandb-1.12.1b3/flytekitplugins_wandb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-22 18:21:16.000000 flytekitplugins_wandb-1.12.1b3/flytekitplugins_wandb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-22 18:21:16.000000 flytekitplugins_wandb-1.12.1b3/flytekitplugins_wandb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 18:21:16.000000 flytekitplugins_wandb-1.12.1b3/flytekitplugins_wandb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 18:21:16.000000 flytekitplugins_wandb-1.12.1b3/flytekitplugins_wandb.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 18:21:16.000000 flytekitplugins_wandb-1.12.1b3/flytekitplugins_wandb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 18:21:16.000000 flytekitplugins_wandb-1.12.1b3/flytekitplugins_wandb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 18:21:16.666911 flytekitplugins_wandb-1.12.1b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-22 18:21:06.000000 flytekitplugins_wandb-1.12.1b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:16.666911 flytekitplugins_wandb-1.12.1b3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-22 18:20:42.000000 flytekitplugins_wandb-1.12.1b3/tests/test_wandb_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:31.307405 flytekitplugins_wandb-1.12.1b4/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-28 15:50:31.307405 flytekitplugins_wandb-1.12.1b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-28 15:49:57.000000 flytekitplugins_wandb-1.12.1b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:31.307405 flytekitplugins_wandb-1.12.1b4/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:31.307405 flytekitplugins_wandb-1.12.1b4/flytekitplugins/wandb/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-28 15:49:57.000000 flytekitplugins_wandb-1.12.1b4/flytekitplugins/wandb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-28 15:49:57.000000 flytekitplugins_wandb-1.12.1b4/flytekitplugins/wandb/tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:31.307405 flytekitplugins_wandb-1.12.1b4/flytekitplugins_wandb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-28 15:50:31.000000 flytekitplugins_wandb-1.12.1b4/flytekitplugins_wandb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-28 15:50:31.000000 flytekitplugins_wandb-1.12.1b4/flytekitplugins_wandb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:50:31.000000 flytekitplugins_wandb-1.12.1b4/flytekitplugins_wandb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 15:50:31.000000 flytekitplugins_wandb-1.12.1b4/flytekitplugins_wandb.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:50:31.000000 flytekitplugins_wandb-1.12.1b4/flytekitplugins_wandb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 15:50:31.000000 flytekitplugins_wandb-1.12.1b4/flytekitplugins_wandb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:50:31.311405 flytekitplugins_wandb-1.12.1b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-28 15:50:20.000000 flytekitplugins_wandb-1.12.1b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:31.307405 flytekitplugins_wandb-1.12.1b4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-28 15:49:57.000000 flytekitplugins_wandb-1.12.1b4/tests/test_wandb_init.py
```

### Comparing `flytekitplugins_wandb-1.12.1b3/PKG-INFO` & `flytekitplugins_wandb-1.12.1b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-wandb
-Version: 1.12.1b3
+Version: 1.12.1b4
 Summary: This package enables seamless use of Weights & Biases within Flyte
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins_wandb-1.12.1b3/README.md` & `flytekitplugins_wandb-1.12.1b4/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins_wandb-1.12.1b3/flytekitplugins/wandb/tracking.py` & `flytekitplugins_wandb-1.12.1b4/flytekitplugins/wandb/tracking.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins_wandb-1.12.1b3/flytekitplugins_wandb.egg-info/PKG-INFO` & `flytekitplugins_wandb-1.12.1b4/flytekitplugins_wandb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-wandb
-Version: 1.12.1b3
+Version: 1.12.1b4
 Summary: This package enables seamless use of Weights & Biases within Flyte
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins_wandb-1.12.1b3/setup.py` & `flytekitplugins_wandb-1.12.1b4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "wandb"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.12.0,<2.0.0", "wandb>=0.17.0"]
 
-__version__ = "1.12.1b3"
+__version__ = "1.12.1b4"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package enables seamless use of Weights & Biases within Flyte",
```

### Comparing `flytekitplugins_wandb-1.12.1b3/tests/test_wandb_init.py` & `flytekitplugins_wandb-1.12.1b4/tests/test_wandb_init.py`

 * *Files identical despite different names*

