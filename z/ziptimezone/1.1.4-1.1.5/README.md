# Comparing `tmp/ziptimezone-1.1.4.tar.gz` & `tmp/ziptimezone-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziptimezone-1.1.4.tar", max compression
+gzip compressed data, was "ziptimezone-1.1.5.tar", max compression
```

## Comparing `ziptimezone-1.1.4.tar` & `ziptimezone-1.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-1.1.4/LICENSE
--rw-r--r--   0        0        0      843 2024-05-28 10:06:08.101969 ziptimezone-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1944 2024-05-19 09:21:03.238230 ziptimezone-1.1.4/README.rst
--rw-r--r--   0        0        0     1395 2024-05-13 11:45:23.443070 ziptimezone-1.1.4/ziptimezone/__init__.py
--rw-r--r--   0        0        0     3598 2024-04-24 12:28:21.581939 ziptimezone-1.1.4/ziptimezone/batch_processor.py
--rw-r--r--   0        0        0     4325 2024-05-19 09:28:26.628819 ziptimezone-1.1.4/ziptimezone/core.py
--rw-r--r--   0        0        0     2780 2024-04-21 13:54:36.749759 ziptimezone-1.1.4/ziptimezone/data_manager.py
--rw-r--r--   0        0        0     1101 2024-04-21 13:54:36.749759 ziptimezone-1.1.4/ziptimezone/geocode.py
--rw-r--r--   0        0        0     1645 2024-04-21 13:54:36.749759 ziptimezone-1.1.4/ziptimezone/globals.py
--rw-r--r--   0        0        0     1874 2024-04-21 13:54:36.749759 ziptimezone-1.1.4/ziptimezone/mappings.py
--rw-r--r--   0        0        0     2618 1970-01-01 00:00:00.000000 ziptimezone-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-1.1.5/LICENSE
+-rw-r--r--   0        0        0      859 2024-05-28 10:11:28.326709 ziptimezone-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1944 2024-05-19 09:21:03.238230 ziptimezone-1.1.5/README.rst
+-rw-r--r--   0        0        0     1395 2024-05-13 11:45:23.443070 ziptimezone-1.1.5/ziptimezone/__init__.py
+-rw-r--r--   0        0        0     3598 2024-04-24 12:28:21.581939 ziptimezone-1.1.5/ziptimezone/batch_processor.py
+-rw-r--r--   0        0        0     4325 2024-05-19 09:28:26.628819 ziptimezone-1.1.5/ziptimezone/core.py
+-rw-r--r--   0        0        0     2780 2024-04-21 13:54:36.749759 ziptimezone-1.1.5/ziptimezone/data_manager.py
+-rw-r--r--   0        0        0     1101 2024-04-21 13:54:36.749759 ziptimezone-1.1.5/ziptimezone/geocode.py
+-rw-r--r--   0        0        0     1645 2024-04-21 13:54:36.749759 ziptimezone-1.1.5/ziptimezone/globals.py
+-rw-r--r--   0        0        0     1874 2024-04-21 13:54:36.749759 ziptimezone-1.1.5/ziptimezone/mappings.py
+-rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 ziptimezone-1.1.5/PKG-INFO
```

### Comparing `ziptimezone-1.1.4/pyproject.toml` & `ziptimezone-1.1.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "ziptimezone"
-version = "1.1.4"
+version = "1.1.5"
 description = "A package to convert ZIP codes to time zones and get geographic coordinates."
 readme = "README.rst"
 authors = ["Manjunath Bettadapura <manjunathbettadapura412@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <4.0"
 requests = "^2.31.0"
 timezonefinder = ">=6.1.5, <=6.5.0"
 python-dateutil = "^2.8"
+pytz="^2024.1"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ziptimezone-1.1.4/README.rst` & `ziptimezone-1.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.1.4/ziptimezone/__init__.py` & `ziptimezone-1.1.5/ziptimezone/__init__.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.1.4/ziptimezone/batch_processor.py` & `ziptimezone-1.1.5/ziptimezone/batch_processor.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.1.4/ziptimezone/core.py` & `ziptimezone-1.1.5/ziptimezone/core.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.1.4/ziptimezone/data_manager.py` & `ziptimezone-1.1.5/ziptimezone/data_manager.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.1.4/ziptimezone/geocode.py` & `ziptimezone-1.1.5/ziptimezone/geocode.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.1.4/ziptimezone/globals.py` & `ziptimezone-1.1.5/ziptimezone/globals.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.1.4/ziptimezone/mappings.py` & `ziptimezone-1.1.5/ziptimezone/mappings.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.1.4/PKG-INFO` & `ziptimezone-1.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: ziptimezone
-Version: 1.1.4
+Version: 1.1.5
 Summary: A package to convert ZIP codes to time zones and get geographic coordinates.
 License: MIT
 Author: Manjunath Bettadapura
 Author-email: manjunathbettadapura412@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: python-dateutil (>=2.8,<3.0)
+Requires-Dist: pytz (>=2024.1,<2025.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: timezonefinder (>=6.1.5,<=6.5.0)
 Description-Content-Type: text/x-rst
 
 ==============
 timezonefinder
 ==============
```

