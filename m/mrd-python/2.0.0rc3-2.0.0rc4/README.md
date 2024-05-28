# Comparing `tmp/mrd_python-2.0.0rc3.tar.gz` & `tmp/mrd_python-2.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrd_python-2.0.0rc3.tar", last modified: Mon May 27 15:59:49 2024, max compression
+gzip compressed data, was "mrd_python-2.0.0rc4.tar", last modified: Tue May 28 02:17:32 2024, max compression
```

## Comparing `mrd_python-2.0.0rc3.tar` & `mrd_python-2.0.0rc4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:59:49.455181 mrd_python-2.0.0rc3/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-27 15:59:49.455181 mrd_python-2.0.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:59:49.451182 mrd_python-2.0.0rc3/mrd/
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46614 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/_dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    39791 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/_ndjson.py
--rw-r--r--   0 runner    (1001) docker     (127)    53801 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)   169451 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/ndjson.py
--rw-r--r--   0 runner    (1001) docker     (127)    23566 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:59:49.451182 mrd_python-2.0.0rc3/mrd/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/tools/export_png_images.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/tools/minimal_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/tools/phantom.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/tools/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8396 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/tools/stream_recon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/tools/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)    97266 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/mrd/yardl_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:59:49.455181 mrd_python-2.0.0rc3/mrd_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-27 15:59:49.000000 mrd_python-2.0.0rc3/mrd_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-27 15:59:49.000000 mrd_python-2.0.0rc3/mrd_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 15:59:49.000000 mrd_python-2.0.0rc3/mrd_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-27 15:59:49.000000 mrd_python-2.0.0rc3/mrd_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-27 15:59:49.000000 mrd_python-2.0.0rc3/mrd_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 15:59:49.455181 mrd_python-2.0.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-27 15:59:44.000000 mrd_python-2.0.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:17:32.471093 mrd_python-2.0.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-28 02:17:32.471093 mrd_python-2.0.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 02:17:24.000000 mrd_python-2.0.0rc4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:17:32.471093 mrd_python-2.0.0rc4/mrd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-28 02:17:24.000000 mrd_python-2.0.0rc4/mrd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46614 2024-05-28 02:17:24.000000 mrd_python-2.0.0rc4/mrd/_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-28 02:17:24.000000 mrd_python-2.0.0rc4/mrd/_dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39791 2024-05-28 02:17:24.000000 mrd_python-2.0.0rc4/mrd/_ndjson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53801 2024-05-28 02:17:24.000000 mrd_python-2.0.0rc4/mrd/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)   169451 2024-05-28 02:17:24.000000 mrd_python-2.0.0rc4/mrd/ndjson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23566 2024-05-28 02:17:24.000000 mrd_python-2.0.0rc4/mrd/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:17:32.471093 mrd_python-2.0.0rc4/mrd/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-28 02:17:24.000000 mrd_python-2.0.0rc4/mrd/tools/export_png_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-28 02:17:24.000000 mrd_python-2.0.0rc4/mrd/tools/minimal_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-05-28 02:17:24.000000 mrd_python-2.0.0rc4/mrd/tools/phantom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-28 02:17:24.000000 mrd_python-2.0.0rc4/mrd/tools/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8396 2024-05-28 02:17:24.000000 mrd_python-2.0.0rc4/mrd/tools/stream_recon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-28 02:17:24.000000 mrd_python-2.0.0rc4/mrd/tools/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97266 2024-05-28 02:17:24.000000 mrd_python-2.0.0rc4/mrd/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-05-28 02:17:24.000000 mrd_python-2.0.0rc4/mrd/yardl_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 02:17:32.471093 mrd_python-2.0.0rc4/mrd_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-28 02:17:32.000000 mrd_python-2.0.0rc4/mrd_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-28 02:17:32.000000 mrd_python-2.0.0rc4/mrd_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 02:17:32.000000 mrd_python-2.0.0rc4/mrd_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-28 02:17:32.000000 mrd_python-2.0.0rc4/mrd_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-28 02:17:32.000000 mrd_python-2.0.0rc4/mrd_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-28 02:17:24.000000 mrd_python-2.0.0rc4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 02:17:32.471093 mrd_python-2.0.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-28 02:17:24.000000 mrd_python-2.0.0rc4/setup.py
```

### Comparing `mrd_python-2.0.0rc3/PKG-INFO` & `mrd_python-2.0.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrd-python
-Version: 2.0.0rc3
+Version: 2.0.0rc4
 Summary: Library and tools for working with data in the ISMRM Raw Data (MRD) format.
 Project-URL: Homepage, https://ismrmrd.github.io/mrd
 Project-URL: Documentation, https://ismrmrd.github.io/mrd
 Project-URL: Repository, https://github.com/ismrmrd/mrd
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mrd_python-2.0.0rc3/mrd/__init__.py` & `mrd_python-2.0.0rc4/mrd/__init__.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc3/mrd/_binary.py` & `mrd_python-2.0.0rc4/mrd/_binary.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc3/mrd/_dtypes.py` & `mrd_python-2.0.0rc4/mrd/_dtypes.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc3/mrd/_ndjson.py` & `mrd_python-2.0.0rc4/mrd/_ndjson.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc3/mrd/binary.py` & `mrd_python-2.0.0rc4/mrd/binary.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc3/mrd/ndjson.py` & `mrd_python-2.0.0rc4/mrd/ndjson.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc3/mrd/protocols.py` & `mrd_python-2.0.0rc4/mrd/protocols.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc3/mrd/tools/export_png_images.py` & `mrd_python-2.0.0rc4/mrd/tools/export_png_images.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc3/mrd/tools/minimal_example.py` & `mrd_python-2.0.0rc4/mrd/tools/minimal_example.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc3/mrd/tools/phantom.py` & `mrd_python-2.0.0rc4/mrd/tools/phantom.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc3/mrd/tools/simulation.py` & `mrd_python-2.0.0rc4/mrd/tools/simulation.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc3/mrd/tools/stream_recon.py` & `mrd_python-2.0.0rc4/mrd/tools/stream_recon.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc3/mrd/tools/transform.py` & `mrd_python-2.0.0rc4/mrd/tools/transform.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc3/mrd/types.py` & `mrd_python-2.0.0rc4/mrd/types.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc3/mrd/yardl_types.py` & `mrd_python-2.0.0rc4/mrd/yardl_types.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc3/mrd_python.egg-info/PKG-INFO` & `mrd_python-2.0.0rc4/mrd_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrd-python
-Version: 2.0.0rc3
+Version: 2.0.0rc4
 Summary: Library and tools for working with data in the ISMRM Raw Data (MRD) format.
 Project-URL: Homepage, https://ismrmrd.github.io/mrd
 Project-URL: Documentation, https://ismrmrd.github.io/mrd
 Project-URL: Repository, https://github.com/ismrmrd/mrd
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mrd_python-2.0.0rc3/pyproject.toml` & `mrd_python-2.0.0rc4/pyproject.toml`

 * *Files identical despite different names*

