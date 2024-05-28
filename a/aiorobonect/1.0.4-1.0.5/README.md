# Comparing `tmp/aiorobonect-1.0.4.tar.gz` & `tmp/aiorobonect-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiorobonect-1.0.4.tar", last modified: Fri May 24 07:39:32 2024, max compression
+gzip compressed data, was "aiorobonect-1.0.5.tar", last modified: Tue May 28 09:42:00 2024, max compression
```

## Comparing `aiorobonect-1.0.4.tar` & `aiorobonect-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:39:32.722325 aiorobonect-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-24 07:39:10.000000 aiorobonect-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-24 07:39:32.722325 aiorobonect-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-24 07:39:10.000000 aiorobonect-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:39:32.722325 aiorobonect-1.0.4/aiorobonect/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-24 07:39:10.000000 aiorobonect-1.0.4/aiorobonect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-24 07:39:10.000000 aiorobonect-1.0.4/aiorobonect/client.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-24 07:39:10.000000 aiorobonect-1.0.4/aiorobonect/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-24 07:39:10.000000 aiorobonect-1.0.4/aiorobonect/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:39:32.722325 aiorobonect-1.0.4/aiorobonect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-24 07:39:32.000000 aiorobonect-1.0.4/aiorobonect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-24 07:39:32.000000 aiorobonect-1.0.4/aiorobonect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 07:39:32.000000 aiorobonect-1.0.4/aiorobonect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-24 07:39:32.000000 aiorobonect-1.0.4/aiorobonect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 07:39:32.000000 aiorobonect-1.0.4/aiorobonect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-24 07:39:32.722325 aiorobonect-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-24 07:39:14.000000 aiorobonect-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:42:00.758483 aiorobonect-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-28 09:41:40.000000 aiorobonect-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-28 09:42:00.758483 aiorobonect-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-28 09:41:40.000000 aiorobonect-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:42:00.754483 aiorobonect-1.0.5/aiorobonect/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 09:41:40.000000 aiorobonect-1.0.5/aiorobonect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-05-28 09:41:40.000000 aiorobonect-1.0.5/aiorobonect/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-28 09:41:40.000000 aiorobonect-1.0.5/aiorobonect/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-28 09:41:40.000000 aiorobonect-1.0.5/aiorobonect/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:42:00.758483 aiorobonect-1.0.5/aiorobonect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-28 09:42:00.000000 aiorobonect-1.0.5/aiorobonect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-28 09:42:00.000000 aiorobonect-1.0.5/aiorobonect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:42:00.000000 aiorobonect-1.0.5/aiorobonect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-28 09:42:00.000000 aiorobonect-1.0.5/aiorobonect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 09:42:00.000000 aiorobonect-1.0.5/aiorobonect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-28 09:42:00.758483 aiorobonect-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-28 09:41:42.000000 aiorobonect-1.0.5/setup.py
```

### Comparing `aiorobonect-1.0.4/LICENSE` & `aiorobonect-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aiorobonect-1.0.4/PKG-INFO` & `aiorobonect-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 1.0.4
+Version: 1.0.5
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-1.0.4/README.md` & `aiorobonect-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `aiorobonect-1.0.4/aiorobonect/client.py` & `aiorobonect-1.0.5/aiorobonect/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Robonect library using aiohttp."""
+
 from __future__ import annotations
 
 from datetime import datetime
 import json
 import logging
 import urllib.parse
 
@@ -108,16 +109,16 @@
                     break  # Exit the loop on successful or error response
                 elif 300 <= response.status_code < 400:
                     _LOGGER.debug(
                         f"Received redirect status code {response.status_code}, continuing to next scheme"
                     )
                     continue  # Continue loop on redirect (3xx)
             except httpx.RequestError as e:
-                _LOGGER.error(
-                    f"Failed to connect using {scheme.upper()}://{self.host}: {e}"
+                _LOGGER.warning(
+                    f"Failed to connect using {scheme}://{self.host} - HTTP STATUS {response.status_code}, {e}"
                 )
                 continue  # Continue to the next scheme on connection error
 
         if response and response.status_code == 200:
             result_text = response.text
             _LOGGER.debug(f"Rest API call result for {command}: {result_text}")
             result_json = json.loads(result_text)
```

### Comparing `aiorobonect-1.0.4/aiorobonect.egg-info/PKG-INFO` & `aiorobonect-1.0.5/aiorobonect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 1.0.4
+Version: 1.0.5
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-1.0.4/setup.cfg` & `aiorobonect-1.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `aiorobonect-1.0.4/setup.py` & `aiorobonect-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Setuptools for aiorobonect."""
+
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aiorobonect",
@@ -16,9 +17,9 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     install_requires=[val.strip() for val in open("requirements.txt")],
-    version="v1.0.4",
+    version="v1.0.5",
 )
```

