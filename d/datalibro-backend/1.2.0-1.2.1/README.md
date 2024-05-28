# Comparing `tmp/datalibro_backend-1.2.0.tar.gz` & `tmp/datalibro_backend-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalibro_backend-1.2.0.tar", last modified: Fri May 17 05:41:01 2024, max compression
+gzip compressed data, was "datalibro_backend-1.2.1.tar", last modified: Tue May 28 04:15:10 2024, max compression
```

## Comparing `datalibro_backend-1.2.0.tar` & `datalibro_backend-1.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-17 05:41:01.928910 datalibro_backend-1.2.0/
--rw-r--r--   0 zhoulucy   (501) staff       (20)     1070 2023-12-08 09:34:06.000000 datalibro_backend-1.2.0/LICENSE.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-05-17 05:41:01.928320 datalibro_backend-1.2.0/PKG-INFO
--rw-r--r--   0 zhoulucy   (501) staff       (20)     1683 2023-12-08 09:30:25.000000 datalibro_backend-1.2.0/README.md
-drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-17 05:41:01.926719 datalibro_backend-1.2.0/datalibro_backend/
--rw-r--r--   0 zhoulucy   (501) staff       (20)      207 2024-02-01 06:19:04.000000 datalibro_backend-1.2.0/datalibro_backend/__init__.py
--rw-r--r--   0 zhoulucy   (501) staff       (20)    15413 2024-05-17 05:40:12.000000 datalibro_backend-1.2.0/datalibro_backend/quality_check.py
--rw-r--r--   0 zhoulucy   (501) staff       (20)    12946 2024-05-15 06:17:37.000000 datalibro_backend-1.2.0/datalibro_backend/read_file.py
-drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-17 05:41:01.927494 datalibro_backend-1.2.0/datalibro_backend.egg-info/
--rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-05-17 05:41:01.000000 datalibro_backend-1.2.0/datalibro_backend.egg-info/PKG-INFO
--rw-r--r--   0 zhoulucy   (501) staff       (20)      290 2024-05-17 05:41:01.000000 datalibro_backend-1.2.0/datalibro_backend.egg-info/SOURCES.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)        1 2024-05-17 05:41:01.000000 datalibro_backend-1.2.0/datalibro_backend.egg-info/dependency_links.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)       18 2024-05-17 05:41:01.000000 datalibro_backend-1.2.0/datalibro_backend.egg-info/top_level.txt
--rw-r--r--   0 zhoulucy   (501) staff       (20)       38 2024-05-17 05:41:01.929232 datalibro_backend-1.2.0/setup.cfg
--rw-r--r--   0 zhoulucy   (501) staff       (20)      594 2024-05-17 05:40:36.000000 datalibro_backend-1.2.0/setup.py
+drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-28 04:15:10.825117 datalibro_backend-1.2.1/
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     1070 2023-12-08 09:34:06.000000 datalibro_backend-1.2.1/LICENSE.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-05-28 04:15:10.824785 datalibro_backend-1.2.1/PKG-INFO
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     1683 2023-12-08 09:30:25.000000 datalibro_backend-1.2.1/README.md
+drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-28 04:15:10.821911 datalibro_backend-1.2.1/datalibro_backend/
+-rw-r--r--   0 zhoulucy   (501) staff       (20)      311 2024-05-28 04:14:48.000000 datalibro_backend-1.2.1/datalibro_backend/__init__.py
+-rw-r--r--   0 zhoulucy   (501) staff       (20)    15413 2024-05-17 05:40:12.000000 datalibro_backend-1.2.1/datalibro_backend/quality_check.py
+-rw-r--r--   0 zhoulucy   (501) staff       (20)    12946 2024-05-15 06:17:37.000000 datalibro_backend-1.2.1/datalibro_backend/read_file.py
+drwxr-xr-x   0 zhoulucy   (501) staff       (20)        0 2024-05-28 04:15:10.824530 datalibro_backend-1.2.1/datalibro_backend.egg-info/
+-rw-r--r--   0 zhoulucy   (501) staff       (20)     2112 2024-05-28 04:15:10.000000 datalibro_backend-1.2.1/datalibro_backend.egg-info/PKG-INFO
+-rw-r--r--   0 zhoulucy   (501) staff       (20)      290 2024-05-28 04:15:10.000000 datalibro_backend-1.2.1/datalibro_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)        1 2024-05-28 04:15:10.000000 datalibro_backend-1.2.1/datalibro_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)       18 2024-05-28 04:15:10.000000 datalibro_backend-1.2.1/datalibro_backend.egg-info/top_level.txt
+-rw-r--r--   0 zhoulucy   (501) staff       (20)       38 2024-05-28 04:15:10.825188 datalibro_backend-1.2.1/setup.cfg
+-rw-r--r--   0 zhoulucy   (501) staff       (20)      594 2024-05-28 04:14:52.000000 datalibro_backend-1.2.1/setup.py
```

### Comparing `datalibro_backend-1.2.0/LICENSE.txt` & `datalibro_backend-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datalibro_backend-1.2.0/PKG-INFO` & `datalibro_backend-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalibro_backend
-Version: 1.2.0
+Version: 1.2.1
 Summary: A small package for your backend service
 Home-page: https://github.com/DesignLibro/datalibro_backend
 Author: lucy
 Author-email: lucy@petlibro.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datalibro_backend-1.2.0/README.md` & `datalibro_backend-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `datalibro_backend-1.2.0/datalibro_backend/quality_check.py` & `datalibro_backend-1.2.1/datalibro_backend/quality_check.py`

 * *Files identical despite different names*

### Comparing `datalibro_backend-1.2.0/datalibro_backend/read_file.py` & `datalibro_backend-1.2.1/datalibro_backend/read_file.py`

 * *Files identical despite different names*

### Comparing `datalibro_backend-1.2.0/datalibro_backend.egg-info/PKG-INFO` & `datalibro_backend-1.2.1/datalibro_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalibro-backend
-Version: 1.2.0
+Version: 1.2.1
 Summary: A small package for your backend service
 Home-page: https://github.com/DesignLibro/datalibro_backend
 Author: lucy
 Author-email: lucy@petlibro.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datalibro_backend-1.2.0/setup.py` & `datalibro_backend-1.2.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="datalibro_backend",
-  version="1.2.0",
+  version="1.2.1",
   author="lucy",
   author_email="lucy@petlibro.com",
   description="A small package for your backend service",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/DesignLibro/datalibro_backend",
   packages=setuptools.find_packages(),
```

