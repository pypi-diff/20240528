# Comparing `tmp/flytekitplugins_async_fsspec-1.12.1b3.tar.gz` & `tmp/flytekitplugins_async_fsspec-1.12.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins_async_fsspec-1.12.1b3.tar", last modified: Wed May 22 18:21:06 2024, max compression
+gzip compressed data, was "flytekitplugins_async_fsspec-1.12.1b4.tar", last modified: Tue May 28 15:50:21 2024, max compression
```

## Comparing `flytekitplugins_async_fsspec-1.12.1b3.tar` & `flytekitplugins_async_fsspec-1.12.1b4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:06.786828 flytekitplugins_async_fsspec-1.12.1b3/
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-22 18:21:06.786828 flytekitplugins_async_fsspec-1.12.1b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-22 18:20:42.000000 flytekitplugins_async_fsspec-1.12.1b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:06.782828 flytekitplugins_async_fsspec-1.12.1b3/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:06.782828 flytekitplugins_async_fsspec-1.12.1b3/flytekitplugins/async_fsspec/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-22 18:20:42.000000 flytekitplugins_async_fsspec-1.12.1b3/flytekitplugins/async_fsspec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:06.782828 flytekitplugins_async_fsspec-1.12.1b3/flytekitplugins/async_fsspec/s3fs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:20:42.000000 flytekitplugins_async_fsspec-1.12.1b3/flytekitplugins/async_fsspec/s3fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-22 18:20:42.000000 flytekitplugins_async_fsspec-1.12.1b3/flytekitplugins/async_fsspec/s3fs/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-05-22 18:20:42.000000 flytekitplugins_async_fsspec-1.12.1b3/flytekitplugins/async_fsspec/s3fs/s3fs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:06.786828 flytekitplugins_async_fsspec-1.12.1b3/flytekitplugins_async_fsspec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-22 18:21:06.000000 flytekitplugins_async_fsspec-1.12.1b3/flytekitplugins_async_fsspec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-22 18:21:06.000000 flytekitplugins_async_fsspec-1.12.1b3/flytekitplugins_async_fsspec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 18:21:06.000000 flytekitplugins_async_fsspec-1.12.1b3/flytekitplugins_async_fsspec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 18:21:06.000000 flytekitplugins_async_fsspec-1.12.1b3/flytekitplugins_async_fsspec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 18:21:06.000000 flytekitplugins_async_fsspec-1.12.1b3/flytekitplugins_async_fsspec.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 18:21:06.000000 flytekitplugins_async_fsspec-1.12.1b3/flytekitplugins_async_fsspec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 18:21:06.000000 flytekitplugins_async_fsspec-1.12.1b3/flytekitplugins_async_fsspec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 18:21:06.786828 flytekitplugins_async_fsspec-1.12.1b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-22 18:21:06.000000 flytekitplugins_async_fsspec-1.12.1b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:21:06.786828 flytekitplugins_async_fsspec-1.12.1b3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-05-22 18:20:42.000000 flytekitplugins_async_fsspec-1.12.1b3/tests/test_s3fs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:21.355360 flytekitplugins_async_fsspec-1.12.1b4/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-28 15:50:21.355360 flytekitplugins_async_fsspec-1.12.1b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-28 15:49:57.000000 flytekitplugins_async_fsspec-1.12.1b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:21.351360 flytekitplugins_async_fsspec-1.12.1b4/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:21.355360 flytekitplugins_async_fsspec-1.12.1b4/flytekitplugins/async_fsspec/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-28 15:49:57.000000 flytekitplugins_async_fsspec-1.12.1b4/flytekitplugins/async_fsspec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:21.355360 flytekitplugins_async_fsspec-1.12.1b4/flytekitplugins/async_fsspec/s3fs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 15:49:57.000000 flytekitplugins_async_fsspec-1.12.1b4/flytekitplugins/async_fsspec/s3fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-28 15:49:57.000000 flytekitplugins_async_fsspec-1.12.1b4/flytekitplugins/async_fsspec/s3fs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-05-28 15:49:57.000000 flytekitplugins_async_fsspec-1.12.1b4/flytekitplugins/async_fsspec/s3fs/s3fs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:21.355360 flytekitplugins_async_fsspec-1.12.1b4/flytekitplugins_async_fsspec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-28 15:50:21.000000 flytekitplugins_async_fsspec-1.12.1b4/flytekitplugins_async_fsspec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-28 15:50:21.000000 flytekitplugins_async_fsspec-1.12.1b4/flytekitplugins_async_fsspec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:50:21.000000 flytekitplugins_async_fsspec-1.12.1b4/flytekitplugins_async_fsspec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-28 15:50:21.000000 flytekitplugins_async_fsspec-1.12.1b4/flytekitplugins_async_fsspec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 15:50:21.000000 flytekitplugins_async_fsspec-1.12.1b4/flytekitplugins_async_fsspec.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 15:50:21.000000 flytekitplugins_async_fsspec-1.12.1b4/flytekitplugins_async_fsspec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 15:50:21.000000 flytekitplugins_async_fsspec-1.12.1b4/flytekitplugins_async_fsspec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:50:21.355360 flytekitplugins_async_fsspec-1.12.1b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-28 15:50:20.000000 flytekitplugins_async_fsspec-1.12.1b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:50:21.355360 flytekitplugins_async_fsspec-1.12.1b4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-05-28 15:49:57.000000 flytekitplugins_async_fsspec-1.12.1b4/tests/test_s3fs.py
```

### Comparing `flytekitplugins_async_fsspec-1.12.1b3/PKG-INFO` & `flytekitplugins_async_fsspec-1.12.1b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-async-fsspec
-Version: 1.12.1b3
+Version: 1.12.1b4
 Summary: This package holds the data persistence plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins_async_fsspec-1.12.1b3/README.md` & `flytekitplugins_async_fsspec-1.12.1b4/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins_async_fsspec-1.12.1b3/flytekitplugins/async_fsspec/s3fs/s3fs.py` & `flytekitplugins_async_fsspec-1.12.1b4/flytekitplugins/async_fsspec/s3fs/s3fs.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins_async_fsspec-1.12.1b3/flytekitplugins_async_fsspec.egg-info/PKG-INFO` & `flytekitplugins_async_fsspec-1.12.1b4/flytekitplugins_async_fsspec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-async-fsspec
-Version: 1.12.1b3
+Version: 1.12.1b4
 Summary: This package holds the data persistence plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins_async_fsspec-1.12.1b3/flytekitplugins_async_fsspec.egg-info/SOURCES.txt` & `flytekitplugins_async_fsspec-1.12.1b4/flytekitplugins_async_fsspec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekitplugins_async_fsspec-1.12.1b3/setup.py` & `flytekitplugins_async_fsspec-1.12.1b4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "async_fsspec"
 
 microlib_name = "flytekitplugins-async-fsspec"
 
 plugin_requires = ["flytekit"]
 
-__version__ = "1.12.1b3"
+__version__ = "1.12.1b4"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the data persistence plugins for flytekit",
```

### Comparing `flytekitplugins_async_fsspec-1.12.1b3/tests/test_s3fs.py` & `flytekitplugins_async_fsspec-1.12.1b4/tests/test_s3fs.py`

 * *Files identical despite different names*
