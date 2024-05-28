# Comparing `tmp/tha-0.1.1.tar.gz` & `tmp/tha-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tha-0.1.1.tar", last modified: Tue May 28 08:24:12 2024, max compression
+gzip compressed data, was "tha-0.1.2.tar", last modified: Tue May 28 08:33:44 2024, max compression
```

## Comparing `tha-0.1.1.tar` & `tha-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-28 08:24:12.554610 tha-0.1.1/
--rw-r--r--   0 seanghay   (501) staff       (20)    11343 2024-05-26 09:50:16.000000 tha-0.1.1/LICENSE
--rw-r--r--   0 seanghay   (501) staff       (20)     6577 2024-05-28 08:24:12.554501 tha-0.1.1/PKG-INFO
--rw-r--r--   0 seanghay   (501) staff       (20)     5160 2024-05-26 09:59:52.000000 tha-0.1.1/README.md
--rw-r--r--   0 seanghay   (501) staff       (20)       38 2024-05-28 08:24:12.554647 tha-0.1.1/setup.cfg
--rw-r--r--   0 seanghay   (501) staff       (20)      759 2024-05-28 08:24:00.000000 tha-0.1.1/setup.py
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-28 08:24:12.553787 tha-0.1.1/tha/
--rw-r--r--   0 seanghay   (501) staff       (20)        0 2024-05-26 10:06:59.000000 tha-0.1.1/tha/__init__.py
--rw-r--r--   0 seanghay   (501) staff       (20)      144 2024-05-26 10:06:59.000000 tha-0.1.1/tha/ascii_lines.py
--rw-r--r--   0 seanghay   (501) staff       (20)     2027 2024-05-26 10:06:59.000000 tha-0.1.1/tha/cardinals.py
--rw-r--r--   0 seanghay   (501) staff       (20)     2043 2024-05-26 10:06:59.000000 tha-0.1.1/tha/currency.py
--rw-r--r--   0 seanghay   (501) staff       (20)     1127 2024-05-26 10:06:59.000000 tha-0.1.1/tha/datetime.py
--rw-r--r--   0 seanghay   (501) staff       (20)      824 2024-05-27 13:53:12.000000 tha-0.1.1/tha/decimals.py
--rw-r--r--   0 seanghay   (501) staff       (20)      161 2024-05-26 10:06:59.000000 tha-0.1.1/tha/hashtags.py
--rw-r--r--   0 seanghay   (501) staff       (20)      438 2024-05-26 10:06:59.000000 tha-0.1.1/tha/license_plate.py
--rw-r--r--   0 seanghay   (501) staff       (20)    17337 2024-05-26 10:06:59.000000 tha-0.1.1/tha/normalize.py
--rw-r--r--   0 seanghay   (501) staff       (20)      304 2024-05-26 10:06:59.000000 tha-0.1.1/tha/ordinals.py
--rw-r--r--   0 seanghay   (501) staff       (20)      164 2024-05-26 10:06:59.000000 tha-0.1.1/tha/parenthesis.py
--rw-r--r--   0 seanghay   (501) staff       (20)     1018 2024-05-26 10:06:59.000000 tha-0.1.1/tha/phone_numbers.py
--rw-r--r--   0 seanghay   (501) staff       (20)      631 2024-05-28 08:19:34.000000 tha-0.1.1/tha/punctuations.py
--rw-r--r--   0 seanghay   (501) staff       (20)     2309 2024-05-26 10:06:59.000000 tha-0.1.1/tha/repeater.py
--rw-r--r--   0 seanghay   (501) staff       (20)      243 2024-05-26 10:06:59.000000 tha-0.1.1/tha/strings.py
--rw-r--r--   0 seanghay   (501) staff       (20)     1016 2024-05-26 10:06:59.000000 tha-0.1.1/tha/urls.py
--rw-r--r--   0 seanghay   (501) staff       (20)     2957 2024-05-26 10:06:59.000000 tha-0.1.1/tha/verbatim.py
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-28 08:24:12.554299 tha-0.1.1/tha.egg-info/
--rw-r--r--   0 seanghay   (501) staff       (20)     6577 2024-05-28 08:24:12.000000 tha-0.1.1/tha.egg-info/PKG-INFO
--rw-r--r--   0 seanghay   (501) staff       (20)      449 2024-05-28 08:24:12.000000 tha-0.1.1/tha.egg-info/SOURCES.txt
--rw-r--r--   0 seanghay   (501) staff       (20)        1 2024-05-28 08:24:12.000000 tha-0.1.1/tha.egg-info/dependency_links.txt
--rw-r--r--   0 seanghay   (501) staff       (20)       35 2024-05-28 08:24:12.000000 tha-0.1.1/tha.egg-info/requires.txt
--rw-r--r--   0 seanghay   (501) staff       (20)        1 2024-05-28 08:24:12.000000 tha-0.1.1/tha.egg-info/top_level.txt
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-28 08:33:44.334361 tha-0.1.2/
+-rw-r--r--   0 seanghay   (501) staff       (20)    11343 2024-05-26 09:50:16.000000 tha-0.1.2/LICENSE
+-rw-r--r--   0 seanghay   (501) staff       (20)     6577 2024-05-28 08:33:44.334247 tha-0.1.2/PKG-INFO
+-rw-r--r--   0 seanghay   (501) staff       (20)     5160 2024-05-26 09:59:52.000000 tha-0.1.2/README.md
+-rw-r--r--   0 seanghay   (501) staff       (20)       38 2024-05-28 08:33:44.334397 tha-0.1.2/setup.cfg
+-rw-r--r--   0 seanghay   (501) staff       (20)      798 2024-05-28 08:33:38.000000 tha-0.1.2/setup.py
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-28 08:33:44.333443 tha-0.1.2/tha/
+-rw-r--r--   0 seanghay   (501) staff       (20)        0 2024-05-26 10:06:59.000000 tha-0.1.2/tha/__init__.py
+-rw-r--r--   0 seanghay   (501) staff       (20)      144 2024-05-26 10:06:59.000000 tha-0.1.2/tha/ascii_lines.py
+-rw-r--r--   0 seanghay   (501) staff       (20)     2027 2024-05-26 10:06:59.000000 tha-0.1.2/tha/cardinals.py
+-rw-r--r--   0 seanghay   (501) staff       (20)     2043 2024-05-26 10:06:59.000000 tha-0.1.2/tha/currency.py
+-rw-r--r--   0 seanghay   (501) staff       (20)     1127 2024-05-26 10:06:59.000000 tha-0.1.2/tha/datetime.py
+-rw-r--r--   0 seanghay   (501) staff       (20)      824 2024-05-27 13:53:12.000000 tha-0.1.2/tha/decimals.py
+-rw-r--r--   0 seanghay   (501) staff       (20)      161 2024-05-26 10:06:59.000000 tha-0.1.2/tha/hashtags.py
+-rw-r--r--   0 seanghay   (501) staff       (20)      438 2024-05-26 10:06:59.000000 tha-0.1.2/tha/license_plate.py
+-rw-r--r--   0 seanghay   (501) staff       (20)    17337 2024-05-26 10:06:59.000000 tha-0.1.2/tha/normalize.py
+-rw-r--r--   0 seanghay   (501) staff       (20)      304 2024-05-26 10:06:59.000000 tha-0.1.2/tha/ordinals.py
+-rw-r--r--   0 seanghay   (501) staff       (20)      164 2024-05-26 10:06:59.000000 tha-0.1.2/tha/parenthesis.py
+-rw-r--r--   0 seanghay   (501) staff       (20)     1018 2024-05-26 10:06:59.000000 tha-0.1.2/tha/phone_numbers.py
+-rw-r--r--   0 seanghay   (501) staff       (20)      631 2024-05-28 08:19:34.000000 tha-0.1.2/tha/punctuations.py
+-rw-r--r--   0 seanghay   (501) staff       (20)      158 2024-05-28 08:05:30.000000 tha-0.1.2/tha/quotings.py
+-rw-r--r--   0 seanghay   (501) staff       (20)     2309 2024-05-26 10:06:59.000000 tha-0.1.2/tha/repeater.py
+-rw-r--r--   0 seanghay   (501) staff       (20)      243 2024-05-26 10:06:59.000000 tha-0.1.2/tha/strings.py
+-rw-r--r--   0 seanghay   (501) staff       (20)     1016 2024-05-26 10:06:59.000000 tha-0.1.2/tha/urls.py
+-rw-r--r--   0 seanghay   (501) staff       (20)     2957 2024-05-26 10:06:59.000000 tha-0.1.2/tha/verbatim.py
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-28 08:33:44.334018 tha-0.1.2/tha.egg-info/
+-rw-r--r--   0 seanghay   (501) staff       (20)     6577 2024-05-28 08:33:44.000000 tha-0.1.2/tha.egg-info/PKG-INFO
+-rw-r--r--   0 seanghay   (501) staff       (20)      465 2024-05-28 08:33:44.000000 tha-0.1.2/tha.egg-info/SOURCES.txt
+-rw-r--r--   0 seanghay   (501) staff       (20)        1 2024-05-28 08:33:44.000000 tha-0.1.2/tha.egg-info/dependency_links.txt
+-rw-r--r--   0 seanghay   (501) staff       (20)       35 2024-05-28 08:33:44.000000 tha-0.1.2/tha.egg-info/requires.txt
+-rw-r--r--   0 seanghay   (501) staff       (20)        4 2024-05-28 08:33:44.000000 tha-0.1.2/tha.egg-info/top_level.txt
```

### Comparing `tha-0.1.1/LICENSE` & `tha-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tha-0.1.1/PKG-INFO` & `tha-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tha
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Khmer Text Normalization and Verbalization Toolkit.
 Home-page: https://github.com/seanghay/tha
 Author: Seanghay Yath
 Author-email: seanghay.dev@gmail.com
 License: Apache License 2.0
 Description: ## Tha (ថា)
```

### Comparing `tha-0.1.1/README.md` & `tha-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tha-0.1.1/setup.py` & `tha-0.1.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import setuptools
 
 with open("README.md", "r") as f:
   long_description = f.read()
 
 setuptools.setup(
   name="tha",
-  version="0.1.1",
+  version="0.1.2",
   description="A Khmer Text Normalization and Verbalization Toolkit.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/seanghay/tha",
   author="Seanghay Yath",
   author_email="seanghay.dev@gmail.com",
   license="Apache License 2.0",
   classifiers=[
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Natural Language :: English",
   ],
   python_requires=">3.5",
+  packages=setuptools.find_packages(),
   package_dir={"tha": "tha"},
   install_requires=[
     "urlextract",
     "phonenumbers",
     "regex",
     "ftfy",
   ],
```

### Comparing `tha-0.1.1/tha/cardinals.py` & `tha-0.1.2/tha/cardinals.py`

 * *Files identical despite different names*

### Comparing `tha-0.1.1/tha/currency.py` & `tha-0.1.2/tha/currency.py`

 * *Files identical despite different names*

### Comparing `tha-0.1.1/tha/datetime.py` & `tha-0.1.2/tha/datetime.py`

 * *Files identical despite different names*

### Comparing `tha-0.1.1/tha/decimals.py` & `tha-0.1.2/tha/decimals.py`

 * *Files identical despite different names*

### Comparing `tha-0.1.1/tha/normalize.py` & `tha-0.1.2/tha/normalize.py`

 * *Files identical despite different names*

### Comparing `tha-0.1.1/tha/phone_numbers.py` & `tha-0.1.2/tha/phone_numbers.py`

 * *Files identical despite different names*

### Comparing `tha-0.1.1/tha/punctuations.py` & `tha-0.1.2/tha/punctuations.py`

 * *Files identical despite different names*

### Comparing `tha-0.1.1/tha/repeater.py` & `tha-0.1.2/tha/repeater.py`

 * *Files identical despite different names*

### Comparing `tha-0.1.1/tha/urls.py` & `tha-0.1.2/tha/urls.py`

 * *Files identical despite different names*

### Comparing `tha-0.1.1/tha/verbatim.py` & `tha-0.1.2/tha/verbatim.py`

 * *Files identical despite different names*

### Comparing `tha-0.1.1/tha.egg-info/PKG-INFO` & `tha-0.1.2/tha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tha
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Khmer Text Normalization and Verbalization Toolkit.
 Home-page: https://github.com/seanghay/tha
 Author: Seanghay Yath
 Author-email: seanghay.dev@gmail.com
 License: Apache License 2.0
 Description: ## Tha (ថា)
```

