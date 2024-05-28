# Comparing `tmp/habslib-0.1.4.tar.gz` & `tmp/habslib-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habslib-0.1.4.tar", last modified: Tue May 28 15:38:11 2024, max compression
+gzip compressed data, was "habslib-0.1.5.tar", last modified: Tue May 28 15:59:01 2024, max compression
```

## Comparing `habslib-0.1.4.tar` & `habslib-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 15:38:11.299661 habslib-0.1.4/
-drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 15:38:11.298129 habslib-0.1.4/HABSlib/
--rw-r--r--   0 do         (501) staff       (20)      126 2024-05-23 15:47:32.000000 habslib-0.1.4/HABSlib/__init__.py
--rwxr-xr-x   0 do         (501) staff       (20)     6925 2024-05-28 14:44:06.000000 habslib-0.1.4/HABSlib/board_manager.py
--rw-r--r--   0 do         (501) staff       (20)      131 2024-05-23 15:47:32.000000 habslib-0.1.4/HABSlib/config.py
--rw-r--r--   0 do         (501) staff       (20)     3706 2024-05-23 15:47:32.000000 habslib-0.1.4/HABSlib/crypt.py
--rw-r--r--   0 do         (501) staff       (20)    15597 2024-05-28 14:43:17.000000 habslib-0.1.4/HABSlib/service.py
--rwxr-xr-x   0 do         (501) staff       (20)      962 2024-05-23 15:47:32.000000 habslib-0.1.4/HABSlib/utils.py
-drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 15:38:11.299293 habslib-0.1.4/HABSlib.egg-info/
--rw-r--r--   0 do         (501) staff       (20)     2073 2024-05-28 15:38:11.000000 habslib-0.1.4/HABSlib.egg-info/PKG-INFO
--rw-r--r--   0 do         (501) staff       (20)      399 2024-05-28 15:38:11.000000 habslib-0.1.4/HABSlib.egg-info/SOURCES.txt
--rw-r--r--   0 do         (501) staff       (20)        1 2024-05-28 15:38:11.000000 habslib-0.1.4/HABSlib.egg-info/dependency_links.txt
--rw-r--r--   0 do         (501) staff       (20)      185 2024-05-28 15:38:11.000000 habslib-0.1.4/HABSlib.egg-info/requires.txt
--rw-r--r--   0 do         (501) staff       (20)       14 2024-05-28 15:38:11.000000 habslib-0.1.4/HABSlib.egg-info/top_level.txt
--rw-r--r--   0 do         (501) staff       (20)     1060 2024-05-28 10:05:57.000000 habslib-0.1.4/LICENCE
--rw-r--r--   0 do         (501) staff       (20)       42 2024-05-27 22:43:14.000000 habslib-0.1.4/MANIFEST.in
--rw-r--r--   0 do         (501) staff       (20)     2073 2024-05-28 15:38:11.299496 habslib-0.1.4/PKG-INFO
--rw-r--r--   0 do         (501) staff       (20)     1215 2024-05-28 15:35:25.000000 habslib-0.1.4/README.md
--rw-r--r--   0 do         (501) staff       (20)      182 2024-05-27 22:49:36.000000 habslib-0.1.4/requirements.txt
--rw-r--r--   0 do         (501) staff       (20)       38 2024-05-28 15:38:11.299699 habslib-0.1.4/setup.cfg
--rw-r--r--   0 do         (501) staff       (20)     1058 2024-05-28 15:35:38.000000 habslib-0.1.4/setup.py
-drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 15:38:11.299100 habslib-0.1.4/tests/
--rw-r--r--   0 do         (501) staff       (20)       62 2024-05-23 15:47:32.000000 habslib-0.1.4/tests/__init__.py
--rw-r--r--   0 do         (501) staff       (20)      131 2024-05-23 15:47:32.000000 habslib-0.1.4/tests/config.py
--rw-r--r--   0 do         (501) staff       (20)     1934 2024-05-23 15:47:32.000000 habslib-0.1.4/tests/conftest.py
--rw-r--r--   0 do         (501) staff       (20)     8908 2024-05-25 11:02:00.000000 habslib-0.1.4/tests/test_habslib.py
+drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 15:59:01.671680 habslib-0.1.5/
+drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 15:59:01.670113 habslib-0.1.5/HABSlib/
+-rw-r--r--   0 do         (501) staff       (20)      126 2024-05-23 15:47:32.000000 habslib-0.1.5/HABSlib/__init__.py
+-rwxr-xr-x   0 do         (501) staff       (20)     6925 2024-05-28 14:44:06.000000 habslib-0.1.5/HABSlib/board_manager.py
+-rw-r--r--   0 do         (501) staff       (20)      131 2024-05-23 15:47:32.000000 habslib-0.1.5/HABSlib/config.py
+-rw-r--r--   0 do         (501) staff       (20)     3706 2024-05-23 15:47:32.000000 habslib-0.1.5/HABSlib/crypt.py
+-rw-r--r--   0 do         (501) staff       (20)    15597 2024-05-28 14:43:17.000000 habslib-0.1.5/HABSlib/service.py
+-rwxr-xr-x   0 do         (501) staff       (20)      962 2024-05-23 15:47:32.000000 habslib-0.1.5/HABSlib/utils.py
+drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 15:59:01.671310 habslib-0.1.5/HABSlib.egg-info/
+-rw-r--r--   0 do         (501) staff       (20)     2025 2024-05-28 15:59:01.000000 habslib-0.1.5/HABSlib.egg-info/PKG-INFO
+-rw-r--r--   0 do         (501) staff       (20)      399 2024-05-28 15:59:01.000000 habslib-0.1.5/HABSlib.egg-info/SOURCES.txt
+-rw-r--r--   0 do         (501) staff       (20)        1 2024-05-28 15:59:01.000000 habslib-0.1.5/HABSlib.egg-info/dependency_links.txt
+-rw-r--r--   0 do         (501) staff       (20)      167 2024-05-28 15:59:01.000000 habslib-0.1.5/HABSlib.egg-info/requires.txt
+-rw-r--r--   0 do         (501) staff       (20)       14 2024-05-28 15:59:01.000000 habslib-0.1.5/HABSlib.egg-info/top_level.txt
+-rw-r--r--   0 do         (501) staff       (20)     1060 2024-05-28 10:05:57.000000 habslib-0.1.5/LICENCE
+-rw-r--r--   0 do         (501) staff       (20)       42 2024-05-27 22:43:14.000000 habslib-0.1.5/MANIFEST.in
+-rw-r--r--   0 do         (501) staff       (20)     2025 2024-05-28 15:59:01.671505 habslib-0.1.5/PKG-INFO
+-rw-r--r--   0 do         (501) staff       (20)     1215 2024-05-28 15:35:25.000000 habslib-0.1.5/README.md
+-rw-r--r--   0 do         (501) staff       (20)      172 2024-05-28 15:44:25.000000 habslib-0.1.5/requirements.txt
+-rw-r--r--   0 do         (501) staff       (20)       38 2024-05-28 15:59:01.671715 habslib-0.1.5/setup.cfg
+-rw-r--r--   0 do         (501) staff       (20)     1018 2024-05-28 15:57:22.000000 habslib-0.1.5/setup.py
+drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 15:59:01.671134 habslib-0.1.5/tests/
+-rw-r--r--   0 do         (501) staff       (20)       62 2024-05-23 15:47:32.000000 habslib-0.1.5/tests/__init__.py
+-rw-r--r--   0 do         (501) staff       (20)      131 2024-05-23 15:47:32.000000 habslib-0.1.5/tests/config.py
+-rw-r--r--   0 do         (501) staff       (20)     1934 2024-05-23 15:47:32.000000 habslib-0.1.5/tests/conftest.py
+-rw-r--r--   0 do         (501) staff       (20)     8909 2024-05-28 15:51:37.000000 habslib-0.1.5/tests/test_habslib.py
```

### Comparing `habslib-0.1.4/HABSlib/board_manager.py` & `habslib-0.1.5/HABSlib/board_manager.py`

 * *Files identical despite different names*

### Comparing `habslib-0.1.4/HABSlib/crypt.py` & `habslib-0.1.5/HABSlib/crypt.py`

 * *Files identical despite different names*

### Comparing `habslib-0.1.4/HABSlib/service.py` & `habslib-0.1.5/HABSlib/service.py`

 * *Files identical despite different names*

### Comparing `habslib-0.1.4/HABSlib/utils.py` & `habslib-0.1.5/HABSlib/utils.py`

 * *Files identical despite different names*

### Comparing `habslib-0.1.4/HABSlib.egg-info/PKG-INFO` & `habslib-0.1.5/HABSlib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HABSlib
-Version: 0.1.4
+Version: 0.1.5
 Summary: A library for interacting with the HABS BrainOS API.
 Home-page: https://github.com/Olocufier/HABS.git
 Author: Domenico Guarino
 Author-email: domenico@habs.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,22 +14,20 @@
 License-File: LICENCE
 Requires-Dist: asyncio==3.4.3
 Requires-Dist: brainflow==5.12.1
 Requires-Dist: numpy==1.26.4
 Requires-Dist: requests==2.31.0
 Requires-Dist: scipy==1.13.0
 Requires-Dist: urllib3==2.2.1
-Requires-Dist: mediapipe
 Requires-Dist: jsonschema
 Requires-Dist: cryptography
 Requires-Dist: pytest
 Requires-Dist: pytest-html
 Requires-Dist: pytest-order
 Requires-Dist: pytest-dependency
-Requires-Dist: py-feat
 
 # HABSlib
 
 Habslib is a Python library for interacting with a remote API, handling complexities like encryption, authentication, and more, so you can focus on building your application.
 
 
 ## Installation
```

### Comparing `habslib-0.1.4/LICENCE` & `habslib-0.1.5/LICENCE`

 * *Files identical despite different names*

### Comparing `habslib-0.1.4/PKG-INFO` & `habslib-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HABSlib
-Version: 0.1.4
+Version: 0.1.5
 Summary: A library for interacting with the HABS BrainOS API.
 Home-page: https://github.com/Olocufier/HABS.git
 Author: Domenico Guarino
 Author-email: domenico@habs.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,22 +14,20 @@
 License-File: LICENCE
 Requires-Dist: asyncio==3.4.3
 Requires-Dist: brainflow==5.12.1
 Requires-Dist: numpy==1.26.4
 Requires-Dist: requests==2.31.0
 Requires-Dist: scipy==1.13.0
 Requires-Dist: urllib3==2.2.1
-Requires-Dist: mediapipe
 Requires-Dist: jsonschema
 Requires-Dist: cryptography
 Requires-Dist: pytest
 Requires-Dist: pytest-html
 Requires-Dist: pytest-order
 Requires-Dist: pytest-dependency
-Requires-Dist: py-feat
 
 # HABSlib
 
 Habslib is a Python library for interacting with a remote API, handling complexities like encryption, authentication, and more, so you can focus on building your application.
 
 
 ## Installation
```

### Comparing `habslib-0.1.4/README.md` & `habslib-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `habslib-0.1.4/setup.py` & `habslib-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="HABSlib",
-    version="0.1.4",
+    version="0.1.5",
     author="Domenico Guarino",
     author_email="domenico@habs.ai",
     description="A library for interacting with the HABS BrainOS API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Olocufier/HABS.git",
     packages=find_packages(),
     install_requires=[
         "asyncio==3.4.3",
         "brainflow==5.12.1",
         "numpy==1.26.4",
         "requests==2.31.0",
         "scipy==1.13.0",
         "urllib3==2.2.1",
-        "mediapipe",
         "jsonschema",
         "cryptography",
         "pytest",
         "pytest-html",
         "pytest-order",
         "pytest-dependency",
-        "py-feat",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     license="MIT",
```

### Comparing `habslib-0.1.4/tests/conftest.py` & `habslib-0.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `habslib-0.1.4/tests/test_habslib.py` & `habslib-0.1.5/tests/test_habslib.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     assert bson.objectid.ObjectId.is_valid(user_id)
     if bson.objectid.ObjectId.is_valid(user_id):
         global g_user_id
         g_user_id = user_id
     print("g_user_id",g_user_id)
 
 
+
 #################################################################
 # Get user data by id
 # - if the user is found, should reply {'status': 'success', 'user_data': document}
 # - if the user is not found, should reply {'status': 'error', 'message': 'User not found'}
 
 @pytest.mark.order(3)
 @pytest.mark.dependency(depends=["test_handshake"])
```

