# Comparing `tmp/habslib-0.1.3.tar.gz` & `tmp/habslib-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habslib-0.1.3.tar", last modified: Tue May 28 15:32:15 2024, max compression
+gzip compressed data, was "habslib-0.1.4.tar", last modified: Tue May 28 15:38:11 2024, max compression
```

## Comparing `habslib-0.1.3.tar` & `habslib-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 15:32:15.663011 habslib-0.1.3/
-drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 15:32:15.661539 habslib-0.1.3/HABSlib/
--rw-r--r--   0 do         (501) staff       (20)      126 2024-05-23 15:47:32.000000 habslib-0.1.3/HABSlib/__init__.py
--rwxr-xr-x   0 do         (501) staff       (20)     6925 2024-05-28 14:44:06.000000 habslib-0.1.3/HABSlib/board_manager.py
--rw-r--r--   0 do         (501) staff       (20)      131 2024-05-23 15:47:32.000000 habslib-0.1.3/HABSlib/config.py
--rw-r--r--   0 do         (501) staff       (20)     3706 2024-05-23 15:47:32.000000 habslib-0.1.3/HABSlib/crypt.py
--rw-r--r--   0 do         (501) staff       (20)    15597 2024-05-28 14:43:17.000000 habslib-0.1.3/HABSlib/service.py
--rwxr-xr-x   0 do         (501) staff       (20)      962 2024-05-23 15:47:32.000000 habslib-0.1.3/HABSlib/utils.py
-drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 15:32:15.662641 habslib-0.1.3/HABSlib.egg-info/
--rw-r--r--   0 do         (501) staff       (20)     2222 2024-05-28 15:32:15.000000 habslib-0.1.3/HABSlib.egg-info/PKG-INFO
--rw-r--r--   0 do         (501) staff       (20)      399 2024-05-28 15:32:15.000000 habslib-0.1.3/HABSlib.egg-info/SOURCES.txt
--rw-r--r--   0 do         (501) staff       (20)        1 2024-05-28 15:32:15.000000 habslib-0.1.3/HABSlib.egg-info/dependency_links.txt
--rw-r--r--   0 do         (501) staff       (20)      185 2024-05-28 15:32:15.000000 habslib-0.1.3/HABSlib.egg-info/requires.txt
--rw-r--r--   0 do         (501) staff       (20)       14 2024-05-28 15:32:15.000000 habslib-0.1.3/HABSlib.egg-info/top_level.txt
--rw-r--r--   0 do         (501) staff       (20)     1060 2024-05-28 10:05:57.000000 habslib-0.1.3/LICENCE
--rw-r--r--   0 do         (501) staff       (20)       42 2024-05-27 22:43:14.000000 habslib-0.1.3/MANIFEST.in
--rw-r--r--   0 do         (501) staff       (20)     2222 2024-05-28 15:32:15.662823 habslib-0.1.3/PKG-INFO
--rw-r--r--   0 do         (501) staff       (20)     1364 2024-05-28 15:31:52.000000 habslib-0.1.3/README.md
--rw-r--r--   0 do         (501) staff       (20)      182 2024-05-27 22:49:36.000000 habslib-0.1.3/requirements.txt
--rw-r--r--   0 do         (501) staff       (20)       38 2024-05-28 15:32:15.663047 habslib-0.1.3/setup.cfg
--rw-r--r--   0 do         (501) staff       (20)     1058 2024-05-28 15:30:11.000000 habslib-0.1.3/setup.py
-drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 15:32:15.662465 habslib-0.1.3/tests/
--rw-r--r--   0 do         (501) staff       (20)       62 2024-05-23 15:47:32.000000 habslib-0.1.3/tests/__init__.py
--rw-r--r--   0 do         (501) staff       (20)      131 2024-05-23 15:47:32.000000 habslib-0.1.3/tests/config.py
--rw-r--r--   0 do         (501) staff       (20)     1934 2024-05-23 15:47:32.000000 habslib-0.1.3/tests/conftest.py
--rw-r--r--   0 do         (501) staff       (20)     8908 2024-05-25 11:02:00.000000 habslib-0.1.3/tests/test_habslib.py
+drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 15:38:11.299661 habslib-0.1.4/
+drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 15:38:11.298129 habslib-0.1.4/HABSlib/
+-rw-r--r--   0 do         (501) staff       (20)      126 2024-05-23 15:47:32.000000 habslib-0.1.4/HABSlib/__init__.py
+-rwxr-xr-x   0 do         (501) staff       (20)     6925 2024-05-28 14:44:06.000000 habslib-0.1.4/HABSlib/board_manager.py
+-rw-r--r--   0 do         (501) staff       (20)      131 2024-05-23 15:47:32.000000 habslib-0.1.4/HABSlib/config.py
+-rw-r--r--   0 do         (501) staff       (20)     3706 2024-05-23 15:47:32.000000 habslib-0.1.4/HABSlib/crypt.py
+-rw-r--r--   0 do         (501) staff       (20)    15597 2024-05-28 14:43:17.000000 habslib-0.1.4/HABSlib/service.py
+-rwxr-xr-x   0 do         (501) staff       (20)      962 2024-05-23 15:47:32.000000 habslib-0.1.4/HABSlib/utils.py
+drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 15:38:11.299293 habslib-0.1.4/HABSlib.egg-info/
+-rw-r--r--   0 do         (501) staff       (20)     2073 2024-05-28 15:38:11.000000 habslib-0.1.4/HABSlib.egg-info/PKG-INFO
+-rw-r--r--   0 do         (501) staff       (20)      399 2024-05-28 15:38:11.000000 habslib-0.1.4/HABSlib.egg-info/SOURCES.txt
+-rw-r--r--   0 do         (501) staff       (20)        1 2024-05-28 15:38:11.000000 habslib-0.1.4/HABSlib.egg-info/dependency_links.txt
+-rw-r--r--   0 do         (501) staff       (20)      185 2024-05-28 15:38:11.000000 habslib-0.1.4/HABSlib.egg-info/requires.txt
+-rw-r--r--   0 do         (501) staff       (20)       14 2024-05-28 15:38:11.000000 habslib-0.1.4/HABSlib.egg-info/top_level.txt
+-rw-r--r--   0 do         (501) staff       (20)     1060 2024-05-28 10:05:57.000000 habslib-0.1.4/LICENCE
+-rw-r--r--   0 do         (501) staff       (20)       42 2024-05-27 22:43:14.000000 habslib-0.1.4/MANIFEST.in
+-rw-r--r--   0 do         (501) staff       (20)     2073 2024-05-28 15:38:11.299496 habslib-0.1.4/PKG-INFO
+-rw-r--r--   0 do         (501) staff       (20)     1215 2024-05-28 15:35:25.000000 habslib-0.1.4/README.md
+-rw-r--r--   0 do         (501) staff       (20)      182 2024-05-27 22:49:36.000000 habslib-0.1.4/requirements.txt
+-rw-r--r--   0 do         (501) staff       (20)       38 2024-05-28 15:38:11.299699 habslib-0.1.4/setup.cfg
+-rw-r--r--   0 do         (501) staff       (20)     1058 2024-05-28 15:35:38.000000 habslib-0.1.4/setup.py
+drwxr-xr-x   0 do         (501) staff       (20)        0 2024-05-28 15:38:11.299100 habslib-0.1.4/tests/
+-rw-r--r--   0 do         (501) staff       (20)       62 2024-05-23 15:47:32.000000 habslib-0.1.4/tests/__init__.py
+-rw-r--r--   0 do         (501) staff       (20)      131 2024-05-23 15:47:32.000000 habslib-0.1.4/tests/config.py
+-rw-r--r--   0 do         (501) staff       (20)     1934 2024-05-23 15:47:32.000000 habslib-0.1.4/tests/conftest.py
+-rw-r--r--   0 do         (501) staff       (20)     8908 2024-05-25 11:02:00.000000 habslib-0.1.4/tests/test_habslib.py
```

### Comparing `habslib-0.1.3/HABSlib/board_manager.py` & `habslib-0.1.4/HABSlib/board_manager.py`

 * *Files identical despite different names*

### Comparing `habslib-0.1.3/HABSlib/crypt.py` & `habslib-0.1.4/HABSlib/crypt.py`

 * *Files identical despite different names*

### Comparing `habslib-0.1.3/HABSlib/service.py` & `habslib-0.1.4/HABSlib/service.py`

 * *Files identical despite different names*

### Comparing `habslib-0.1.3/HABSlib/utils.py` & `habslib-0.1.4/HABSlib/utils.py`

 * *Files identical despite different names*

### Comparing `habslib-0.1.3/HABSlib.egg-info/PKG-INFO` & `habslib-0.1.4/HABSlib.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HABSlib
-Version: 0.1.3
+Version: 0.1.4
 Summary: A library for interacting with the HABS BrainOS API.
 Home-page: https://github.com/Olocufier/HABS.git
 Author: Domenico Guarino
 Author-email: domenico@habs.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -27,21 +27,14 @@
 Requires-Dist: pytest-dependency
 Requires-Dist: py-feat
 
 # HABSlib
 
 Habslib is a Python library for interacting with a remote API, handling complexities like encryption, authentication, and more, so you can focus on building your application.
 
-## Table of Contents
-
-- [Installation](#installation)
-- [Usage](#usage)
-- [Contributing](#contributing)
-- [License](#license)
-- [Contact](#contact)
 
 ## Installation
 
 You can install habslib using pip:
 
 ```
 pip install HABSlib
@@ -84,8 +77,8 @@
 
 ## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 ## Contact
 
-If you have any questions or need support, please open an issue on GitHub or contact info@habs.ai.
+If you have any questions or need support, please open an issue on GitHub or contact dev@habs.ai.
```

### Comparing `habslib-0.1.3/LICENCE` & `habslib-0.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `habslib-0.1.3/PKG-INFO` & `habslib-0.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HABSlib
-Version: 0.1.3
+Version: 0.1.4
 Summary: A library for interacting with the HABS BrainOS API.
 Home-page: https://github.com/Olocufier/HABS.git
 Author: Domenico Guarino
 Author-email: domenico@habs.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -27,21 +27,14 @@
 Requires-Dist: pytest-dependency
 Requires-Dist: py-feat
 
 # HABSlib
 
 Habslib is a Python library for interacting with a remote API, handling complexities like encryption, authentication, and more, so you can focus on building your application.
 
-## Table of Contents
-
-- [Installation](#installation)
-- [Usage](#usage)
-- [Contributing](#contributing)
-- [License](#license)
-- [Contact](#contact)
 
 ## Installation
 
 You can install habslib using pip:
 
 ```
 pip install HABSlib
@@ -84,8 +77,8 @@
 
 ## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
 
 ## Contact
 
-If you have any questions or need support, please open an issue on GitHub or contact info@habs.ai.
+If you have any questions or need support, please open an issue on GitHub or contact dev@habs.ai.
```

### Comparing `habslib-0.1.3/setup.py` & `habslib-0.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="HABSlib",
-    version="0.1.3",
+    version="0.1.4",
     author="Domenico Guarino",
     author_email="domenico@habs.ai",
     description="A library for interacting with the HABS BrainOS API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Olocufier/HABS.git",
     packages=find_packages(),
```

### Comparing `habslib-0.1.3/tests/conftest.py` & `habslib-0.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `habslib-0.1.3/tests/test_habslib.py` & `habslib-0.1.4/tests/test_habslib.py`

 * *Files identical despite different names*

