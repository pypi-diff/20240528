# Comparing `tmp/sqlalchemy_schema_factory-0.1.4.tar.gz` & `tmp/sqlalchemy_schema_factory-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_schema_factory-0.1.4.tar", max compression
+gzip compressed data, was "sqlalchemy_schema_factory-0.2.0.tar", max compression
```

## Comparing `sqlalchemy_schema_factory-0.1.4.tar` & `sqlalchemy_schema_factory-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,7 @@
--rw-r--r--   0        0        0       79 2024-04-15 12:07:12.792817 sqlalchemy_schema_factory-0.1.4/README.md
--rw-r--r--   0        0        0      510 2024-04-17 08:15:39.935124 sqlalchemy_schema_factory-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       80 2024-01-11 09:14:13.699175 sqlalchemy_schema_factory-0.1.4/sqlalchemy_schema_factory/__init__.py
--rw-r--r--   0        0        0      807 2022-07-27 17:35:59.300000 sqlalchemy_schema_factory-0.1.4/sqlalchemy_schema_factory/auxiliary.py
--rw-r--r--   0        0        0      699 2022-07-27 17:35:59.303000 sqlalchemy_schema_factory-0.1.4/sqlalchemy_schema_factory/conventions.py
--rw-r--r--   0        0        0     7236 2023-10-22 17:21:00.808619 sqlalchemy_schema_factory-0.1.4/sqlalchemy_schema_factory/factory.py
--rw-r--r--   0        0        0       58 2024-01-11 09:14:13.699423 sqlalchemy_schema_factory-0.1.4/sqlalchemy_schema_factory/jsonb/__init__.py
--rw-r--r--   0        0        0      538 2024-01-11 09:14:13.699814 sqlalchemy_schema_factory-0.1.4/sqlalchemy_schema_factory/jsonb/decoding.py
--rw-r--r--   0        0        0      669 2024-01-11 09:14:13.699968 sqlalchemy_schema_factory-0.1.4/sqlalchemy_schema_factory/jsonb/encoding.py
--rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 sqlalchemy_schema_factory-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       79 2024-04-15 12:07:12.792817 sqlalchemy_schema_factory-0.2.0/README.md
+-rw-r--r--   0        0        0      510 2024-05-28 09:18:37.786897 sqlalchemy_schema_factory-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       69 2024-05-28 09:17:37.622004 sqlalchemy_schema_factory-0.2.0/sqlalchemy_schema_factory/__init__.py
+-rw-r--r--   0        0        0      807 2022-07-27 17:35:59.300000 sqlalchemy_schema_factory-0.2.0/sqlalchemy_schema_factory/auxiliary.py
+-rw-r--r--   0        0        0      699 2022-07-27 17:35:59.303000 sqlalchemy_schema_factory-0.2.0/sqlalchemy_schema_factory/conventions.py
+-rw-r--r--   0        0        0     7236 2023-10-22 17:21:00.808619 sqlalchemy_schema_factory-0.2.0/sqlalchemy_schema_factory/factory.py
+-rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 sqlalchemy_schema_factory-0.2.0/PKG-INFO
```

### Comparing `sqlalchemy_schema_factory-0.1.4/sqlalchemy_schema_factory/auxiliary.py` & `sqlalchemy_schema_factory-0.2.0/sqlalchemy_schema_factory/auxiliary.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_schema_factory-0.1.4/sqlalchemy_schema_factory/conventions.py` & `sqlalchemy_schema_factory-0.2.0/sqlalchemy_schema_factory/conventions.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_schema_factory-0.1.4/sqlalchemy_schema_factory/factory.py` & `sqlalchemy_schema_factory-0.2.0/sqlalchemy_schema_factory/factory.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_schema_factory-0.1.4/PKG-INFO` & `sqlalchemy_schema_factory-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-schema-factory
-Version: 0.1.4
+Version: 0.2.0
 Summary: Collection of tools for building sqlalchemy schemas
 Home-page: https://github.com/smairon/sqlalchemy-schema-factory
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

