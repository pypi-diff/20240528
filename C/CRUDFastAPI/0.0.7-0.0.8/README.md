# Comparing `tmp/crudfastapi-0.0.7.tar.gz` & `tmp/crudfastapi-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crudfastapi-0.0.7.tar", max compression
+gzip compressed data, was "crudfastapi-0.0.8.tar", max compression
```

## Comparing `crudfastapi-0.0.7.tar` & `crudfastapi-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      403 2024-05-14 02:36:21.061981 crudfastapi-0.0.7/CRUDFastAPI/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.7/CRUDFastAPI/crud/__init__.py
--rw-r--r--   0        0        0    73001 2024-05-22 08:26:56.293132 crudfastapi-0.0.7/CRUDFastAPI/crud/fast_crud.py
--rw-r--r--   0        0        0     6121 2024-05-15 05:35:59.523525 crudfastapi-0.0.7/CRUDFastAPI/crud/helper.py
--rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.7/CRUDFastAPI/endpoint/__init__.py
--rw-r--r--   0        0        0    10362 2024-05-14 02:36:21.061981 crudfastapi-0.0.7/CRUDFastAPI/endpoint/crud_router.py
--rw-r--r--   0        0        0    24496 2024-05-14 02:36:21.061981 crudfastapi-0.0.7/CRUDFastAPI/endpoint/endpoint_creator.py
--rw-r--r--   0        0        0     3993 2024-05-14 02:36:21.061981 crudfastapi-0.0.7/CRUDFastAPI/endpoint/helper.py
--rw-r--r--   0        0        0       64 2024-05-14 02:36:21.061981 crudfastapi-0.0.7/CRUDFastAPI/exceptions/__init__.py
--rw-r--r--   0        0        0     2105 2024-05-14 02:36:21.061981 crudfastapi-0.0.7/CRUDFastAPI/exceptions/http_exceptions.py
--rw-r--r--   0        0        0      255 2024-05-14 02:36:21.061981 crudfastapi-0.0.7/CRUDFastAPI/paginated/__init__.py
--rw-r--r--   0        0        0      821 2024-05-14 02:36:21.061981 crudfastapi-0.0.7/CRUDFastAPI/paginated/helper.py
--rw-r--r--   0        0        0     1034 2024-05-14 02:36:21.061981 crudfastapi-0.0.7/CRUDFastAPI/paginated/response.py
--rw-r--r--   0        0        0      397 2024-05-14 02:36:21.061981 crudfastapi-0.0.7/CRUDFastAPI/paginated/schemas.py
--rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.7/CRUDFastAPI/py.typed
--rw-r--r--   0        0        0     1088 2024-05-14 02:36:21.061981 crudfastapi-0.0.7/LICENSE
--rw-r--r--   0        0        0     1498 2024-05-22 08:27:02.632723 crudfastapi-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     8347 2024-05-14 02:36:21.061981 crudfastapi-0.0.7/README.md
--rw-r--r--   0        0        0     9370 1970-01-01 00:00:00.000000 crudfastapi-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      403 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/crud/__init__.py
+-rw-r--r--   0        0        0    73026 2024-05-28 08:04:14.443842 crudfastapi-0.0.8/CRUDFastAPI/crud/fast_crud.py
+-rw-r--r--   0        0        0     6121 2024-05-15 05:35:59.523525 crudfastapi-0.0.8/CRUDFastAPI/crud/helper.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/endpoint/__init__.py
+-rw-r--r--   0        0        0    10362 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/endpoint/crud_router.py
+-rw-r--r--   0        0        0    24496 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/endpoint/endpoint_creator.py
+-rw-r--r--   0        0        0     3993 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/endpoint/helper.py
+-rw-r--r--   0        0        0       64 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/exceptions/__init__.py
+-rw-r--r--   0        0        0     2105 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/exceptions/http_exceptions.py
+-rw-r--r--   0        0        0      255 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/paginated/__init__.py
+-rw-r--r--   0        0        0      821 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/paginated/helper.py
+-rw-r--r--   0        0        0     1034 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/paginated/response.py
+-rw-r--r--   0        0        0      397 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/paginated/schemas.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/CRUDFastAPI/py.typed
+-rw-r--r--   0        0        0     1088 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1498 2024-05-28 08:03:28.031007 crudfastapi-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     8347 2024-05-14 02:36:21.061981 crudfastapi-0.0.8/README.md
+-rw-r--r--   0        0        0     9370 1970-01-01 00:00:00.000000 crudfastapi-0.0.8/PKG-INFO
```

### Comparing `crudfastapi-0.0.7/CRUDFastAPI/crud/fast_crud.py` & `crudfastapi-0.0.8/CRUDFastAPI/crud/fast_crud.py`

 * *Files 0% similar despite different names*

```diff
@@ -1306,15 +1306,15 @@
                 "Cannot use both single join parameters and joins_config simultaneously."
             )
         elif not joins_config and not join_model:
             raise ValueError("You need one of join_model or joins_config.")
 
         if (limit is not None and limit < 0) or offset < 0:
             raise ValueError("Limit and offset must be non-negative.")
-        if join_on is None:
+        if join_on is None and joins_config is None:
             join_on = _auto_detect_join_condition(self.model, join_model)
 
         primary_select = _extract_matching_columns_from_schema(
             model=self.model, schema=schema_to_select
         )
         stmt: Select = select(*primary_select)
```

### Comparing `crudfastapi-0.0.7/CRUDFastAPI/crud/helper.py` & `crudfastapi-0.0.8/CRUDFastAPI/crud/helper.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.7/CRUDFastAPI/endpoint/crud_router.py` & `crudfastapi-0.0.8/CRUDFastAPI/endpoint/crud_router.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.7/CRUDFastAPI/endpoint/endpoint_creator.py` & `crudfastapi-0.0.8/CRUDFastAPI/endpoint/endpoint_creator.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.7/CRUDFastAPI/endpoint/helper.py` & `crudfastapi-0.0.8/CRUDFastAPI/endpoint/helper.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.7/CRUDFastAPI/exceptions/http_exceptions.py` & `crudfastapi-0.0.8/CRUDFastAPI/exceptions/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.7/CRUDFastAPI/paginated/helper.py` & `crudfastapi-0.0.8/CRUDFastAPI/paginated/helper.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.7/CRUDFastAPI/paginated/response.py` & `crudfastapi-0.0.8/CRUDFastAPI/paginated/response.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.7/LICENSE` & `crudfastapi-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.7/pyproject.toml` & `crudfastapi-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "CRUDFastAPI"
-version = "0.0.7"
+version = "0.0.8"
 description = "CRUDFastAPI is a Python package for FastAPI, offering robust async CRUD operations and flexible endpoint creation utilities."
 authors = ["Mithun Thomas <mithunthomas003@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mithun2003/CRUDFastAPI"
 include = ["LICENSE"]
```

### Comparing `crudfastapi-0.0.7/README.md` & `crudfastapi-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.7/PKG-INFO` & `crudfastapi-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CRUDFastAPI
-Version: 0.0.7
+Version: 0.0.8
 Summary: CRUDFastAPI is a Python package for FastAPI, offering robust async CRUD operations and flexible endpoint creation utilities.
 Home-page: https://github.com/mithun2003/CRUDFastAPI
 License: MIT
 Keywords: fastapi,crud,async,sqlalchemy,pydantic,fastcrud,crudfastapi
 Author: Mithun Thomas
 Author-email: mithunthomas003@gmail.com
 Requires-Python: >=3.9,<4.0
```

