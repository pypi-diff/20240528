# Comparing `tmp/flytekitplugins_mmcloud-1.12.1b3.tar.gz` & `tmp/flytekitplugins_mmcloud-1.12.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins_mmcloud-1.12.1b3.tar", last modified: Wed May 22 18:21:12 2024, max compression
+gzip compressed data, was "flytekitplugins_mmcloud-1.12.1b4.tar", last modified: Tue May 28 15:50:27 2024, max compression
```

## Comparing `flytekitplugins_mmcloud-1.12.1b3.tar` & `flytekitplugins_mmcloud-1.12.1b4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:12.674878 flytekitplugins_mmcloud-1.12.1b3/
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-22 18:21:12.674878 flytekitplugins_mmcloud-1.12.1b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-22 18:20:42.000000 flytekitplugins_mmcloud-1.12.1b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:12.674878 flytekitplugins_mmcloud-1.12.1b3/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:12.674878 flytekitplugins_mmcloud-1.12.1b3/flytekitplugins/mmcloud/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-22 18:20:42.000000 flytekitplugins_mmcloud-1.12.1b3/flytekitplugins/mmcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-05-22 18:20:42.000000 flytekitplugins_mmcloud-1.12.1b3/flytekitplugins/mmcloud/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-22 18:20:42.000000 flytekitplugins_mmcloud-1.12.1b3/flytekitplugins/mmcloud/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-22 18:20:42.000000 flytekitplugins_mmcloud-1.12.1b3/flytekitplugins/mmcloud/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:12.674878 flytekitplugins_mmcloud-1.12.1b3/flytekitplugins_mmcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-22 18:21:12.000000 flytekitplugins_mmcloud-1.12.1b3/flytekitplugins_mmcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-22 18:21:12.000000 flytekitplugins_mmcloud-1.12.1b3/flytekitplugins_mmcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 18:21:12.000000 flytekitplugins_mmcloud-1.12.1b3/flytekitplugins_mmcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 18:21:12.000000 flytekitplugins_mmcloud-1.12.1b3/flytekitplugins_mmcloud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 18:21:12.000000 flytekitplugins_mmcloud-1.12.1b3/flytekitplugins_mmcloud.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-22 18:21:12.000000 flytekitplugins_mmcloud-1.12.1b3/flytekitplugins_mmcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 18:21:12.000000 flytekitplugins_mmcloud-1.12.1b3/flytekitplugins_mmcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 18:21:12.674878 flytekitplugins_mmcloud-1.12.1b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-22 18:21:06.000000 flytekitplugins_mmcloud-1.12.1b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:12.674878 flytekitplugins_mmcloud-1.12.1b3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-05-22 18:20:42.000000 flytekitplugins_mmcloud-1.12.1b3/tests/test_mmcloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:27.303387 flytekitplugins_mmcloud-1.12.1b4/
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-28 15:50:27.303387 flytekitplugins_mmcloud-1.12.1b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-28 15:49:57.000000 flytekitplugins_mmcloud-1.12.1b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:27.299387 flytekitplugins_mmcloud-1.12.1b4/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:27.299387 flytekitplugins_mmcloud-1.12.1b4/flytekitplugins/mmcloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-28 15:49:57.000000 flytekitplugins_mmcloud-1.12.1b4/flytekitplugins/mmcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-05-28 15:49:57.000000 flytekitplugins_mmcloud-1.12.1b4/flytekitplugins/mmcloud/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-28 15:49:57.000000 flytekitplugins_mmcloud-1.12.1b4/flytekitplugins/mmcloud/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-28 15:49:57.000000 flytekitplugins_mmcloud-1.12.1b4/flytekitplugins/mmcloud/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:27.303387 flytekitplugins_mmcloud-1.12.1b4/flytekitplugins_mmcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-28 15:50:27.000000 flytekitplugins_mmcloud-1.12.1b4/flytekitplugins_mmcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-28 15:50:27.000000 flytekitplugins_mmcloud-1.12.1b4/flytekitplugins_mmcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:50:27.000000 flytekitplugins_mmcloud-1.12.1b4/flytekitplugins_mmcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 15:50:27.000000 flytekitplugins_mmcloud-1.12.1b4/flytekitplugins_mmcloud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 15:50:27.000000 flytekitplugins_mmcloud-1.12.1b4/flytekitplugins_mmcloud.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 15:50:27.000000 flytekitplugins_mmcloud-1.12.1b4/flytekitplugins_mmcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 15:50:27.000000 flytekitplugins_mmcloud-1.12.1b4/flytekitplugins_mmcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:50:27.303387 flytekitplugins_mmcloud-1.12.1b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-28 15:50:20.000000 flytekitplugins_mmcloud-1.12.1b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:27.303387 flytekitplugins_mmcloud-1.12.1b4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-05-28 15:49:57.000000 flytekitplugins_mmcloud-1.12.1b4/tests/test_mmcloud.py
```

### Comparing `flytekitplugins_mmcloud-1.12.1b3/PKG-INFO` & `flytekitplugins_mmcloud-1.12.1b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-mmcloud
-Version: 1.12.1b3
+Version: 1.12.1b4
 Summary: MemVerge Flyte plugin
 Author: Edwin Yu, Helen Zhang
 Author-email: helen.zhang@memverge.com
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins_mmcloud-1.12.1b3/README.md` & `flytekitplugins_mmcloud-1.12.1b4/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins_mmcloud-1.12.1b3/flytekitplugins/mmcloud/agent.py` & `flytekitplugins_mmcloud-1.12.1b4/flytekitplugins/mmcloud/agent.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins_mmcloud-1.12.1b3/flytekitplugins/mmcloud/task.py` & `flytekitplugins_mmcloud-1.12.1b4/flytekitplugins/mmcloud/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins_mmcloud-1.12.1b3/flytekitplugins/mmcloud/utils.py` & `flytekitplugins_mmcloud-1.12.1b4/flytekitplugins/mmcloud/utils.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins_mmcloud-1.12.1b3/flytekitplugins_mmcloud.egg-info/PKG-INFO` & `flytekitplugins_mmcloud-1.12.1b4/flytekitplugins_mmcloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-mmcloud
-Version: 1.12.1b3
+Version: 1.12.1b4
 Summary: MemVerge Flyte plugin
 Author: Edwin Yu, Helen Zhang
 Author-email: helen.zhang@memverge.com
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins_mmcloud-1.12.1b3/flytekitplugins_mmcloud.egg-info/SOURCES.txt` & `flytekitplugins_mmcloud-1.12.1b4/flytekitplugins_mmcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekitplugins_mmcloud-1.12.1b3/setup.py` & `flytekitplugins_mmcloud-1.12.1b4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "mmcloud"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.9.1,<2.0.0", "kubernetes"]
 
-__version__ = "1.12.1b3"
+__version__ = "1.12.1b4"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="Edwin Yu, Helen Zhang",
     author_email="helen.zhang@memverge.com",
     description="MemVerge Flyte plugin",
```

### Comparing `flytekitplugins_mmcloud-1.12.1b3/tests/test_mmcloud.py` & `flytekitplugins_mmcloud-1.12.1b4/tests/test_mmcloud.py`

 * *Files identical despite different names*

