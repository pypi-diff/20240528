# Comparing `tmp/zodchy_fastapi-0.3.2.tar.gz` & `tmp/zodchy_fastapi-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodchy_fastapi-0.3.2.tar", max compression
+gzip compressed data, was "zodchy_fastapi-0.3.3.tar", max compression
```

## Comparing `zodchy_fastapi-0.3.2.tar` & `zodchy_fastapi-0.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       16 2024-04-13 13:32:10.912348 zodchy_fastapi-0.3.2/README.md
--rw-r--r--   0        0        0      466 2024-05-26 13:56:18.165686 zodchy_fastapi-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      129 2024-05-02 14:57:10.856896 zodchy_fastapi-0.3.2/zodchy_fastapi/__init__.py
--rw-r--r--   0        0        0      232 2024-05-02 13:34:11.382181 zodchy_fastapi-0.3.2/zodchy_fastapi/contracts.py
--rw-r--r--   0        0        0       90 2024-05-02 13:34:11.371712 zodchy_fastapi-0.3.2/zodchy_fastapi/middleware/__init__.py
--rw-r--r--   0        0        0     1343 2024-05-02 13:34:11.364678 zodchy_fastapi-0.3.2/zodchy_fastapi/middleware/handlers.py
--rw-r--r--   0        0        0       79 2024-05-26 13:25:07.157731 zodchy_fastapi-0.3.2/zodchy_fastapi/request/__init__.py
--rw-r--r--   0        0        0     2061 2024-05-02 14:57:10.836323 zodchy_fastapi-0.3.2/zodchy_fastapi/request/adapter.py
--rw-r--r--   0        0        0      553 2024-05-02 13:10:41.930229 zodchy_fastapi-0.3.2/zodchy_fastapi/request/schema.py
--rw-r--r--   0        0        0       79 2024-05-02 13:34:11.354249 zodchy_fastapi-0.3.2/zodchy_fastapi/response/__init__.py
--rw-r--r--   0        0        0     1399 2024-05-02 13:34:11.421798 zodchy_fastapi-0.3.2/zodchy_fastapi/response/adapter.py
--rw-r--r--   0        0        0      597 2024-05-26 13:56:18.171632 zodchy_fastapi-0.3.2/zodchy_fastapi/response/schema.py
--rw-r--r--   0        0        0       61 2024-05-02 13:34:11.359388 zodchy_fastapi-0.3.2/zodchy_fastapi/routing/__init__.py
--rw-r--r--   0        0        0      766 2024-05-02 13:34:11.357096 zodchy_fastapi-0.3.2/zodchy_fastapi/routing/schema.py
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 zodchy_fastapi-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0       16 2024-04-13 13:32:10.912348 zodchy_fastapi-0.3.3/README.md
+-rw-r--r--   0        0        0      466 2024-05-28 08:33:27.333329 zodchy_fastapi-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      129 2024-05-02 14:57:10.856896 zodchy_fastapi-0.3.3/zodchy_fastapi/__init__.py
+-rw-r--r--   0        0        0      232 2024-05-02 13:34:11.382181 zodchy_fastapi-0.3.3/zodchy_fastapi/contracts.py
+-rw-r--r--   0        0        0       90 2024-05-02 13:34:11.371712 zodchy_fastapi-0.3.3/zodchy_fastapi/middleware/__init__.py
+-rw-r--r--   0        0        0     1343 2024-05-02 13:34:11.364678 zodchy_fastapi-0.3.3/zodchy_fastapi/middleware/handlers.py
+-rw-r--r--   0        0        0       79 2024-05-26 13:25:07.157731 zodchy_fastapi-0.3.3/zodchy_fastapi/request/__init__.py
+-rw-r--r--   0        0        0     2061 2024-05-02 14:57:10.836323 zodchy_fastapi-0.3.3/zodchy_fastapi/request/adapter.py
+-rw-r--r--   0        0        0      553 2024-05-02 13:10:41.930229 zodchy_fastapi-0.3.3/zodchy_fastapi/request/schema.py
+-rw-r--r--   0        0        0       79 2024-05-02 13:34:11.354249 zodchy_fastapi-0.3.3/zodchy_fastapi/response/__init__.py
+-rw-r--r--   0        0        0     1399 2024-05-02 13:34:11.421798 zodchy_fastapi-0.3.3/zodchy_fastapi/response/adapter.py
+-rw-r--r--   0        0        0      597 2024-05-26 13:56:18.171632 zodchy_fastapi-0.3.3/zodchy_fastapi/response/schema.py
+-rw-r--r--   0        0        0       61 2024-05-02 13:34:11.359388 zodchy_fastapi-0.3.3/zodchy_fastapi/routing/__init__.py
+-rw-r--r--   0        0        0      766 2024-05-02 13:34:11.357096 zodchy_fastapi-0.3.3/zodchy_fastapi/routing/schema.py
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 zodchy_fastapi-0.3.3/PKG-INFO
```

### Comparing `zodchy_fastapi-0.3.2/zodchy_fastapi/middleware/handlers.py` & `zodchy_fastapi-0.3.3/zodchy_fastapi/middleware/handlers.py`

 * *Files identical despite different names*

### Comparing `zodchy_fastapi-0.3.2/zodchy_fastapi/request/adapter.py` & `zodchy_fastapi-0.3.3/zodchy_fastapi/request/adapter.py`

 * *Files identical despite different names*

### Comparing `zodchy_fastapi-0.3.2/zodchy_fastapi/request/schema.py` & `zodchy_fastapi-0.3.3/zodchy_fastapi/request/schema.py`

 * *Files identical despite different names*

### Comparing `zodchy_fastapi-0.3.2/zodchy_fastapi/response/adapter.py` & `zodchy_fastapi-0.3.3/zodchy_fastapi/response/adapter.py`

 * *Files identical despite different names*

### Comparing `zodchy_fastapi-0.3.2/zodchy_fastapi/response/schema.py` & `zodchy_fastapi-0.3.3/zodchy_fastapi/response/schema.py`

 * *Files identical despite different names*

### Comparing `zodchy_fastapi-0.3.2/zodchy_fastapi/routing/schema.py` & `zodchy_fastapi-0.3.3/zodchy_fastapi/routing/schema.py`

 * *Files identical despite different names*

### Comparing `zodchy_fastapi-0.3.2/PKG-INFO` & `zodchy_fastapi-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: zodchy-fastapi
-Version: 0.3.2
+Version: 0.3.3
 Summary: Collection of tools to integrate fastapi to zodchy architecture
 Home-page: https://github.com/smairon/zodchy-fastapi
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: fastapi (>=0.110.2,<0.111.0)
-Requires-Dist: zodchy (>=0.2.3,<0.3.0)
+Requires-Dist: zodchy (>=0.3.0,<0.4.0)
 Project-URL: Repository, https://github.com/smairon/zodchy-fastapi
 Description-Content-Type: text/markdown
 
 # Zodchy fastapi
```

