# Comparing `tmp/parepy_toolbox-0.0.0.tar.gz` & `tmp/parepy_toolbox-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parepy_toolbox-0.0.0.tar", max compression
+gzip compressed data, was "parepy_toolbox-0.0.1.tar", max compression
```

## Comparing `parepy_toolbox-0.0.0.tar` & `parepy_toolbox-0.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1088 2024-04-27 16:39:26.213349 parepy_toolbox-0.0.0/license.md
--rw-r--r--   0        0        0       50 2024-04-27 16:39:26.228990 parepy_toolbox-0.0.0/parepy_toolbox/__init__.py
--rw-r--r--   0        0        0    21439 2024-05-05 16:46:47.731282 parepy_toolbox-0.0.0/parepy_toolbox/common_library.py
--rw-r--r--   0        0        0    17530 2024-05-05 17:06:03.417088 parepy_toolbox-0.0.0/parepy_toolbox/pare.py
--rw-r--r--   0        0        0      411 2024-05-05 17:10:35.944615 parepy_toolbox-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      147 2024-05-05 17:04:19.399242 parepy_toolbox-0.0.0/readme.md
--rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 parepy_toolbox-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2024-02-29 17:02:45.276036 parepy_toolbox-0.0.1/license.md
+-rw-r--r--   0        0        0       50 2024-02-09 15:16:05.334898 parepy_toolbox-0.0.1/parepy_toolbox/__init__.py
+-rw-r--r--   0        0        0    21439 2024-05-28 11:40:41.104919 parepy_toolbox-0.0.1/parepy_toolbox/common_library.py
+-rw-r--r--   0        0        0    17530 2024-05-28 11:40:41.104919 parepy_toolbox-0.0.1/parepy_toolbox/pare.py
+-rw-r--r--   0        0        0      411 2024-05-28 11:41:46.781249 parepy_toolbox-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      147 2024-05-28 11:40:41.107920 parepy_toolbox-0.0.1/readme.md
+-rw-r--r--   0        0        0      752 1970-01-01 00:00:00.000000 parepy_toolbox-0.0.1/PKG-INFO
```

### Comparing `parepy_toolbox-0.0.0/license.md` & `parepy_toolbox-0.0.1/license.md`

 * *Files identical despite different names*

### Comparing `parepy_toolbox-0.0.0/parepy_toolbox/common_library.py` & `parepy_toolbox-0.0.1/parepy_toolbox/common_library.py`

 * *Files identical despite different names*

### Comparing `parepy_toolbox-0.0.0/parepy_toolbox/pare.py` & `parepy_toolbox-0.0.1/parepy_toolbox/pare.py`

 * *Files identical despite different names*

### Comparing `parepy_toolbox-0.0.0/PKG-INFO` & `parepy_toolbox-0.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: parepy-toolbox
-Version: 0.0.0
+Version: 0.0.1
 Summary: 
 Author: wmpjrufg
 Author-email: wanderlei_junior@ufcat.edu.br
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: scipy (>=1.13.0,<2.0.0)
```

