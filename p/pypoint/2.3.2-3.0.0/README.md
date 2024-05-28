# Comparing `tmp/pypoint-2.3.2.tar.gz` & `tmp/pypoint-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypoint-2.3.2.tar", last modified: Sun Sep 24 20:53:16 2023, max compression
+gzip compressed data, was "pypoint-3.0.0.tar", last modified: Tue May 28 17:25:18 2024, max compression
```

## Comparing `pypoint-2.3.2.tar` & `pypoint-3.0.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 fer        (501) staff       (20)        0 2023-09-24 20:53:16.559836 pypoint-2.3.2/
--rw-r--r--   0 fer        (501) staff       (20)     1075 2018-10-30 12:16:50.000000 pypoint-2.3.2/LICENSE
--rw-r--r--   0 fer        (501) staff       (20)      962 2023-09-24 20:53:16.559904 pypoint-2.3.2/PKG-INFO
--rw-r--r--   0 fer        (501) staff       (20)      565 2019-11-12 21:59:20.000000 pypoint-2.3.2/README.md
-drwxr-xr-x   0 fer        (501) staff       (20)        0 2023-09-24 20:53:16.558809 pypoint-2.3.2/pypoint/
--rw-r--r--   0 fer        (501) staff       (20)    12703 2023-09-24 20:37:02.000000 pypoint-2.3.2/pypoint/__init__.py
-drwxr-xr-x   0 fer        (501) staff       (20)        0 2023-09-24 20:53:16.559707 pypoint-2.3.2/pypoint.egg-info/
--rw-r--r--   0 fer        (501) staff       (20)      962 2023-09-24 20:53:16.000000 pypoint-2.3.2/pypoint.egg-info/PKG-INFO
--rw-r--r--   0 fer        (501) staff       (20)      210 2023-09-24 20:53:16.000000 pypoint-2.3.2/pypoint.egg-info/SOURCES.txt
--rw-r--r--   0 fer        (501) staff       (20)        1 2023-09-24 20:53:16.000000 pypoint-2.3.2/pypoint.egg-info/dependency_links.txt
--rw-r--r--   0 fer        (501) staff       (20)       25 2023-09-24 20:53:16.000000 pypoint-2.3.2/pypoint.egg-info/requires.txt
--rw-r--r--   0 fer        (501) staff       (20)        8 2023-09-24 20:53:16.000000 pypoint-2.3.2/pypoint.egg-info/top_level.txt
--rw-r--r--   0 fer        (501) staff       (20)      507 2023-09-24 20:53:16.560195 pypoint-2.3.2/setup.cfg
--rw-r--r--   0 fer        (501) staff       (20)      692 2023-09-24 20:52:49.000000 pypoint-2.3.2/setup.py
+drwxr-xr-x   0 fer        (501) staff       (20)        0 2024-05-28 17:25:18.680254 pypoint-3.0.0/
+-rw-r--r--   0 fer        (501) staff       (20)     1075 2018-10-30 12:16:50.000000 pypoint-3.0.0/LICENSE
+-rw-r--r--   0 fer        (501) staff       (20)      962 2024-05-28 17:25:18.680448 pypoint-3.0.0/PKG-INFO
+-rw-r--r--   0 fer        (501) staff       (20)      565 2019-11-12 21:59:20.000000 pypoint-3.0.0/README.md
+drwxr-xr-x   0 fer        (501) staff       (20)        0 2024-05-28 17:25:18.679311 pypoint-3.0.0/pypoint/
+-rw-r--r--   0 fer        (501) staff       (20)     8300 2024-05-28 17:19:54.000000 pypoint-3.0.0/pypoint/__init__.py
+-rw-r--r--   0 fer        (501) staff       (20)     1881 2024-05-28 17:24:35.000000 pypoint-3.0.0/pypoint/auth.py
+-rw-r--r--   0 fer        (501) staff       (20)     2208 2024-05-28 17:24:35.000000 pypoint-3.0.0/pypoint/const.py
+drwxr-xr-x   0 fer        (501) staff       (20)        0 2024-05-28 17:25:18.680015 pypoint-3.0.0/pypoint.egg-info/
+-rw-r--r--   0 fer        (501) staff       (20)      962 2024-05-28 17:25:18.000000 pypoint-3.0.0/pypoint.egg-info/PKG-INFO
+-rw-r--r--   0 fer        (501) staff       (20)      243 2024-05-28 17:25:18.000000 pypoint-3.0.0/pypoint.egg-info/SOURCES.txt
+-rw-r--r--   0 fer        (501) staff       (20)        1 2024-05-28 17:25:18.000000 pypoint-3.0.0/pypoint.egg-info/dependency_links.txt
+-rw-r--r--   0 fer        (501) staff       (20)        8 2024-05-28 17:25:18.000000 pypoint-3.0.0/pypoint.egg-info/requires.txt
+-rw-r--r--   0 fer        (501) staff       (20)        8 2024-05-28 17:25:18.000000 pypoint-3.0.0/pypoint.egg-info/top_level.txt
+-rw-r--r--   0 fer        (501) staff       (20)      507 2024-05-28 17:25:18.680744 pypoint-3.0.0/setup.cfg
+-rw-r--r--   0 fer        (501) staff       (20)      664 2024-05-28 17:25:14.000000 pypoint-3.0.0/setup.py
```

### Comparing `pypoint-2.3.2/LICENSE` & `pypoint-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypoint-2.3.2/PKG-INFO` & `pypoint-3.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypoint
-Version: 2.3.2
+Version: 3.0.0
 Summary: API for Minut Point
 Home-page: https://github.com/fredrike/pypoint
 Author: Fredrik Erlandsson
 Author-email: fredrik.e@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pypoint-2.3.2/README.md` & `pypoint-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pypoint-2.3.2/pypoint.egg-info/PKG-INFO` & `pypoint-3.0.0/pypoint.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypoint
-Version: 2.3.2
+Version: 3.0.0
 Summary: API for Minut Point
 Home-page: https://github.com/fredrike/pypoint
 Author: Fredrik Erlandsson
 Author-email: fredrik.e@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pypoint-2.3.2/setup.py` & `pypoint-3.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,25 +2,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pypoint",
-    version="2.3.2",
+    version="3.0.0",
     author="Fredrik Erlandsson",
     author_email="fredrik.e@gmail.com",
     description="API for Minut Point",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fredrike/pypoint",
     packages=["pypoint"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        "authlib",
-        "httpx>=0.19.0,<1",
+        "aiohttp",
     ],
 )
```

