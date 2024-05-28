# Comparing `tmp/zodchy_patterns-0.3.0.tar.gz` & `tmp/zodchy_patterns-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodchy_patterns-0.3.0.tar", max compression
+gzip compressed data, was "zodchy_patterns-0.3.1.tar", max compression
```

## Comparing `zodchy_patterns-0.3.0.tar` & `zodchy_patterns-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       17 2024-04-13 13:27:36.273813 zodchy_patterns-0.3.0/README.md
--rw-r--r--   0        0        0      435 2024-05-26 13:58:06.446848 zodchy_patterns-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       42 2024-04-18 15:44:02.094165 zodchy_patterns-0.3.0/zodchy_patterns/__init__.py
--rw-r--r--   0        0        0      368 2024-04-18 15:44:02.102702 zodchy_patterns-0.3.0/zodchy_patterns/events/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 15:27:46.945461 zodchy_patterns-0.3.0/zodchy_patterns/events/io/__init__.py
--rw-r--r--   0        0        0     1776 2024-04-27 11:27:06.970090 zodchy_patterns-0.3.0/zodchy_patterns/events/io/error.py
--rw-r--r--   0        0        0      319 2024-04-27 11:27:06.976528 zodchy_patterns-0.3.0/zodchy_patterns/events/io/generic.py
--rw-r--r--   0        0        0     1095 2024-04-18 15:44:02.083540 zodchy_patterns-0.3.0/zodchy_patterns/events/io/info.py
--rw-r--r--   0        0        0      819 2024-05-23 16:43:52.142427 zodchy_patterns-0.3.0/zodchy_patterns/mapping.py
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 zodchy_patterns-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-04-13 13:27:36.273813 zodchy_patterns-0.3.1/README.md
+-rw-r--r--   0        0        0      435 2024-05-28 08:35:38.811710 zodchy_patterns-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-04-18 15:44:02.094165 zodchy_patterns-0.3.1/zodchy_patterns/__init__.py
+-rw-r--r--   0        0        0      368 2024-04-18 15:44:02.102702 zodchy_patterns-0.3.1/zodchy_patterns/events/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:27:46.945461 zodchy_patterns-0.3.1/zodchy_patterns/events/io/__init__.py
+-rw-r--r--   0        0        0     1776 2024-04-27 11:27:06.970090 zodchy_patterns-0.3.1/zodchy_patterns/events/io/error.py
+-rw-r--r--   0        0        0      319 2024-04-27 11:27:06.976528 zodchy_patterns-0.3.1/zodchy_patterns/events/io/generic.py
+-rw-r--r--   0        0        0     1095 2024-04-18 15:44:02.083540 zodchy_patterns-0.3.1/zodchy_patterns/events/io/info.py
+-rw-r--r--   0        0        0      819 2024-05-23 16:43:52.142427 zodchy_patterns-0.3.1/zodchy_patterns/mapping.py
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 zodchy_patterns-0.3.1/PKG-INFO
```

### Comparing `zodchy_patterns-0.3.0/zodchy_patterns/events/io/error.py` & `zodchy_patterns-0.3.1/zodchy_patterns/events/io/error.py`

 * *Files identical despite different names*

### Comparing `zodchy_patterns-0.3.0/zodchy_patterns/events/io/info.py` & `zodchy_patterns-0.3.1/zodchy_patterns/events/io/info.py`

 * *Files identical despite different names*

### Comparing `zodchy_patterns-0.3.0/zodchy_patterns/mapping.py` & `zodchy_patterns-0.3.1/zodchy_patterns/mapping.py`

 * *Files identical despite different names*

### Comparing `zodchy_patterns-0.3.0/PKG-INFO` & `zodchy_patterns-0.3.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: zodchy-patterns
-Version: 0.3.0
+Version: 0.3.1
 Summary: Collection of patterns to use in CQRS applications
 Home-page: https://github.com/smairon/zodchy-patterns
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: zodchy (>=0.2.4,<0.3.0)
+Requires-Dist: zodchy (>=0.3.0,<0.4.0)
 Project-URL: Repository, https://github.com/smairon/zodchy-patterns
 Description-Content-Type: text/markdown
 
 # Zodchy patterns
```

