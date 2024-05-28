# Comparing `tmp/sqla_async_orm_queries-1.1.4.tar.gz` & `tmp/sqla_async_orm_queries-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqla_async_orm_queries-1.1.4.tar", max compression
+gzip compressed data, was "sqla_async_orm_queries-1.1.5.tar", max compression
```

## Comparing `sqla_async_orm_queries-1.1.4.tar` & `sqla_async_orm_queries-1.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2024-05-23 11:34:13.461425 sqla_async_orm_queries-1.1.4/LICENCE.md
--rw-r--r--   0        0        0     2610 2024-05-23 11:34:13.461425 sqla_async_orm_queries-1.1.4/README.md
--rw-r--r--   0        0        0      909 2024-05-23 11:34:24.205391 sqla_async_orm_queries-1.1.4/pyproject.toml
--rw-r--r--   0        0        0       72 2024-05-23 11:34:13.461425 sqla_async_orm_queries-1.1.4/sqla_async_orm_queries/__init__.py
--rw-r--r--   0        0        0     6977 2024-05-23 11:34:13.461425 sqla_async_orm_queries-1.1.4/sqla_async_orm_queries/models.py
--rw-r--r--   0        0        0     3709 1970-01-01 00:00:00.000000 sqla_async_orm_queries-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-28 11:22:47.179269 sqla_async_orm_queries-1.1.5/LICENCE.md
+-rw-r--r--   0        0        0     2610 2024-05-28 11:22:47.179269 sqla_async_orm_queries-1.1.5/README.md
+-rw-r--r--   0        0        0      909 2024-05-28 11:22:58.575348 sqla_async_orm_queries-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0       72 2024-05-28 11:22:47.179269 sqla_async_orm_queries-1.1.5/sqla_async_orm_queries/__init__.py
+-rw-r--r--   0        0        0     6987 2024-05-28 11:22:47.179269 sqla_async_orm_queries-1.1.5/sqla_async_orm_queries/models.py
+-rw-r--r--   0        0        0     3709 1970-01-01 00:00:00.000000 sqla_async_orm_queries-1.1.5/PKG-INFO
```

### Comparing `sqla_async_orm_queries-1.1.4/LICENCE.md` & `sqla_async_orm_queries-1.1.5/LICENCE.md`

 * *Files identical despite different names*

### Comparing `sqla_async_orm_queries-1.1.4/README.md` & `sqla_async_orm_queries-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `sqla_async_orm_queries-1.1.4/pyproject.toml` & `sqla_async_orm_queries-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqla-async-orm-queries"
-version = "v1.1.4"
+version = "v1.1.5"
 description = "Base model for SqlAlchemy async orm queries"
 authors = ["Amrah <bagirovemrah97@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/amrahhh/sqla_async_orm_queries"
 repository = "https://github.com/amrahhh/sqla_async_orm_queries"
 classifiers = [
```

### Comparing `sqla_async_orm_queries-1.1.4/sqla_async_orm_queries/models.py` & `sqla_async_orm_queries-1.1.5/sqla_async_orm_queries/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,15 +106,15 @@
                 selected_columns = [getattr(cls, col) for col in columns]
                 query = select(*selected_columns).where(*args).options(*loaders)
             else:
                 query = select(cls).where(*args).options(*loaders)
 
             query = cls._order_by(query, order_by)
             result = await session.execute(query)
-            data = result.all()
+            data = result.scalars().all()
 
         return data
 
     @classmethod
     async def update(cls, data: dict, *args: BinaryExpression):
         async with SessionLocal() as session:
             try:
```

### Comparing `sqla_async_orm_queries-1.1.4/PKG-INFO` & `sqla_async_orm_queries-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqla-async-orm-queries
-Version: 1.1.4
+Version: 1.1.5
 Summary: Base model for SqlAlchemy async orm queries
 Home-page: https://github.com/amrahhh/sqla_async_orm_queries
 License: MIT
 Author: Amrah
 Author-email: bagirovemrah97@gmail.com
 Requires-Python: >=3.8.2,<4.0.0
 Classifier: Intended Audience :: Developers
```

