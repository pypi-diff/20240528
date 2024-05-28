# Comparing `tmp/pancho-1.0.5.tar.gz` & `tmp/pancho-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pancho-1.0.5.tar", max compression
+gzip compressed data, was "pancho-1.0.6.tar", max compression
```

## Comparing `pancho-1.0.5.tar` & `pancho-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-01-04 14:53:25.782768 pancho-1.0.5/LICENSE
--rw-r--r--   0        0        0       39 2024-04-15 11:57:48.480093 pancho-1.0.5/README.md
--rw-r--r--   0        0        0      130 2024-04-02 15:23:42.891832 pancho-1.0.5/pancho/__init__.py
--rw-r--r--   0        0        0       36 2023-10-20 11:24:28.509021 pancho-1.0.5/pancho/definition/__init__.py
--rw-r--r--   0        0        0     2628 2024-04-30 08:52:46.883848 pancho-1.0.5/pancho/definition/contracts.py
--rw-r--r--   0        0        0     1520 2024-04-02 15:23:42.892185 pancho-1.0.5/pancho/definition/exceptions.py
--rw-r--r--   0        0        0      122 2024-04-02 15:23:42.892333 pancho-1.0.5/pancho/implementation/__init__.py
--rw-r--r--   0        0        0     1076 2024-04-30 08:53:29.357119 pancho-1.0.5/pancho/implementation/factory.py
--rw-r--r--   0        0        0     5573 2024-04-05 08:07:40.295161 pancho-1.0.5/pancho/implementation/processing.py
--rw-r--r--   0        0        0     7615 2024-04-05 16:44:15.824108 pancho-1.0.5/pancho/implementation/registry.py
--rw-r--r--   0        0        0      358 2024-04-30 08:53:07.930017 pancho-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 pancho-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-01-04 14:53:25.782768 pancho-1.0.6/LICENSE
+-rw-r--r--   0        0        0       39 2024-04-15 11:57:48.480093 pancho-1.0.6/README.md
+-rw-r--r--   0        0        0      130 2024-04-02 15:23:42.891832 pancho-1.0.6/pancho/__init__.py
+-rw-r--r--   0        0        0       36 2023-10-20 11:24:28.509021 pancho-1.0.6/pancho/definition/__init__.py
+-rw-r--r--   0        0        0     2628 2024-04-30 08:52:46.883848 pancho-1.0.6/pancho/definition/contracts.py
+-rw-r--r--   0        0        0     1520 2024-04-02 15:23:42.892185 pancho-1.0.6/pancho/definition/exceptions.py
+-rw-r--r--   0        0        0      122 2024-04-02 15:23:42.892333 pancho-1.0.6/pancho/implementation/__init__.py
+-rw-r--r--   0        0        0     1076 2024-04-30 08:53:29.357119 pancho-1.0.6/pancho/implementation/factory.py
+-rw-r--r--   0        0        0     5573 2024-04-05 08:07:40.295161 pancho-1.0.6/pancho/implementation/processing.py
+-rw-r--r--   0        0        0     7615 2024-04-05 16:44:15.824108 pancho-1.0.6/pancho/implementation/registry.py
+-rw-r--r--   0        0        0      358 2024-05-28 08:47:49.615072 pancho-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 pancho-1.0.6/PKG-INFO
```

### Comparing `pancho-1.0.5/LICENSE` & `pancho-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pancho-1.0.5/pancho/definition/contracts.py` & `pancho-1.0.6/pancho/definition/contracts.py`

 * *Files identical despite different names*

### Comparing `pancho-1.0.5/pancho/definition/exceptions.py` & `pancho-1.0.6/pancho/definition/exceptions.py`

 * *Files identical despite different names*

### Comparing `pancho-1.0.5/pancho/implementation/factory.py` & `pancho-1.0.6/pancho/implementation/factory.py`

 * *Files identical despite different names*

### Comparing `pancho-1.0.5/pancho/implementation/processing.py` & `pancho-1.0.6/pancho/implementation/processing.py`

 * *Files identical despite different names*

### Comparing `pancho-1.0.5/pancho/implementation/registry.py` & `pancho-1.0.6/pancho/implementation/registry.py`

 * *Files identical despite different names*

### Comparing `pancho-1.0.5/PKG-INFO` & `pancho-1.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pancho
-Version: 1.0.5
+Version: 1.0.6
 Summary: Commands and queries processor
 Home-page: https://github.com/smairon/pancho
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: zodchy (>=0.2.3,<0.3.0)
+Requires-Dist: zodchy (>=0.3.0,<0.4.0)
 Project-URL: Repository, https://github.com/smairon/pancho
 Description-Content-Type: text/markdown
 
 # Pancho
 Commands and queries processor
```

