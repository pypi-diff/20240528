# Comparing `tmp/almasql-0.1.1.tar.gz` & `tmp/almasql-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almasql-0.1.1.tar", max compression
+gzip compressed data, was "almasql-0.1.2.tar", max compression
```

## Comparing `almasql-0.1.1.tar` & `almasql-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,14 @@
--rw-r--r--   0        0        0      953 2024-05-20 09:58:10.000000 almasql-0.1.1/README.md
--rw-r--r--   0        0        0      366 2024-05-20 09:57:11.000000 almasql-0.1.1/almasql/__init__.py
--rw-r--r--   0        0        0      332 2024-05-20 09:56:30.000000 almasql-0.1.1/almasql/_directives.py
--rw-r--r--   0        0        0     2283 2024-05-20 07:08:20.000000 almasql-0.1.1/almasql/_post_join.py
--rw-r--r--   0        0        0      571 2024-05-20 09:56:38.000000 almasql-0.1.1/almasql/_query.py
--rw-r--r--   0        0        0     2284 2024-05-20 07:29:09.000000 almasql-0.1.1/almasql/_transaction.py
--rw-r--r--   0        0        0     1200 2024-05-20 07:33:34.000000 almasql-0.1.1/almasql/_transactions_chain.py
--rw-r--r--   0        0        0      318 2024-05-20 23:20:04.958314 almasql-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1390 1970-01-01 00:00:00.000000 almasql-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-28 19:27:48.366693 almasql-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0      962 2024-05-28 19:28:06.292593 almasql-0.1.2/README.md
+-rw-r--r--   0        0        0      385 2024-05-28 18:46:59.871081 almasql-0.1.2/almasql/__init__.py
+-rw-r--r--   0        0        0      928 2024-05-28 19:04:54.119893 almasql-0.1.2/almasql/_directives_.py
+-rw-r--r--   0        0        0     2256 2024-05-28 19:11:47.055501 almasql-0.1.2/almasql/_post_join_.py
+-rw-r--r--   0        0        0     1139 2024-05-28 19:06:40.790858 almasql-0.1.2/almasql/_query_.py
+-rw-r--r--   0        0        0      135 2024-05-26 20:04:59.372398 almasql-0.1.2/almasql/_testing/_my_/__init__.py
+-rw-r--r--   0        0        0      538 2024-05-26 20:51:43.314925 almasql-0.1.2/almasql/_testing/_my_/_almasql_assert_.py
+-rw-r--r--   0        0        0       84 2024-05-28 19:06:08.300046 almasql-0.1.2/almasql/_testing/_my_/_settings_.py
+-rw-r--r--   0        0        0     2232 2024-05-28 19:13:12.803231 almasql-0.1.2/almasql/_testing/test_queries.py
+-rw-r--r--   0        0        0     2366 2024-05-28 17:18:02.314704 almasql-0.1.2/almasql/_transaction_.py
+-rw-r--r--   0        0        0     1174 2024-05-26 20:34:21.339461 almasql-0.1.2/almasql/_transactions_chain_.py
+-rw-r--r--   0        0        0      878 2024-05-28 19:36:14.034408 almasql-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1764 1970-01-01 00:00:00.000000 almasql-0.1.2/PKG-INFO
```

### Comparing `almasql-0.1.1/README.md` & `almasql-0.1.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,36 @@
+AlmaSQL
+
 <details>
 <summary>Directives</summary>
 
 Directives are functions that can extend AlmaSQL by customizing the way an expression renders.
 
 Using a directive in your template is as simple as calling a function in a template expression.
 
-AlmaSQL includes a number of built-in directives like `set_values_by` and `enumerate_values_by`.
+AlmaSQL includes a number of built-in directives like `set` and `values`.
 
 Users can also write their own custom directives.
 
 <details>
-<summary>set_values_by</summary>
+<summary>set</summary>
 
-Imagine table `book` and columns `id`, `title`, and `author`.
+Imagine table `book` and columns `id`, `title`, and `is_active`.
 And you want to update book by id.
 
 ```jinja
 UPDATE book
-SET title = :title, author = :author
+SET title = :title, is_active = :is_active
 WHERE id = :id
 ```
 
 But when you need to modify column, you need to change the query template.
 What if you forgot to do it? This will lead to unexpected bugs.
 So better to use directives that, depending on the arguments,
 will render the required columns and values.
 
 ```jinja
-UPDATE book
-{{ set_values_by(['title', 'author']) }}
+UPDATE book{{ set({'title': 'Why do I love almasql?', 'is_active': True}) }}
 WHERE id = :id
 ```
 </details>
 </details>
```

### Comparing `almasql-0.1.1/almasql/_post_join.py` & `almasql-0.1.2/almasql/_post_join_.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 async def post_join[LI: object, RI: object, K: typing.Any](
     _attribute_: str,
     _from_: typing.Callable[[set[K]], typing.Coroutine[typing.Any, typing.Any, typing.Iterable[RI]]],
     _where_: typing.Callable[[RI], K],
     _equal_: typing.Callable[[LI], K],
-    source: list[LI],
+    _source_: list[LI],
     /,
     many = False,
     default = Unset,
 ) -> None:
     """
     Joins list of subrecords from function to list of record by `_attribute_`.
     Group subrecords if many is True.
@@ -44,23 +44,21 @@
     )
     for b in books:
         list_of_authors = ', '.join([author.full_name for author in b.authors])
         print(f'book {b.name} published by {list_of_authors}')
     ```
     """
     source_map = {}
-    for source_item in source:
+    for source_item in _source_:
         fkey = _equal_(source_item)
         source_map[fkey] = source_item
         setattr(source_item, _attribute_, default)
 
-    _source_fkeys = set(source_map.keys())
-    _right_items_ = await _from_(_source_fkeys)
-
-    for right_item in _right_items_:
+    source_fkeys = set(source_map.keys())
+    for right_item in await _from_(source_fkeys):
         fkey = _where_(right_item)
 
         source_item = source_map.get(fkey)
         if source_item is None:
             continue
 
         if not many:
@@ -70,17 +68,17 @@
         nested_items = getattr(source_item, _attribute_, None)
         if nested_items is None:
             nested_items = []
             setattr(source_item, _attribute_, nested_items)
         nested_items.append(right_item)
 
     if default is Unset:
-        n = len(source)
+        n = len(_source_)
         i = 0
         while n > i:
-            source_item = source[i]
+            source_item = _source_[i]
             nested_items = getattr(source_item, _attribute_)
             if nested_items is Unset:
                 n -= 1
-                source.pop(i)
+                _source_.pop(i)
             else:
                 i += 1
```

### Comparing `almasql-0.1.1/almasql/_transaction.py` & `almasql-0.1.2/almasql/_transaction_.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,89 +3,97 @@
 
 import sqlalchemy as sqla
 from sqlalchemy.ext.asyncio import (
     AsyncConnection as sqla_connection,
     AsyncEngine as sqla_engine,
 )
 
-from . import _query
-from . import _transactions_chain
+from . import _query_
+from . import _transactions_chain_
 
 
 class active_transaction:
     """
     Represents an active transaction.
     """
 
     def __init__(
         self,
         sqlac: sqla_connection,
     ):
         self._sqlac = sqlac
 
+    async def _(
+        self,
+        q: _query_.query | str,
+        **parameters,
+    ) -> sqla.CursorResult:
+        if not isinstance(q, _query_.query):
+            q = _query_.query(q)
+        statement = q.compile(parameters)
+        return await self._sqlac.execute(statement, parameters)
+
     async def fetch_one(
         self,
-        q: _query.query,
+        q: _query_.query,
         **parameters,
     ) -> sqla.RowMapping | None:
         """
         Returns the first row of the query result.
         """
-        statement = q.render(**parameters)
-        result = await self._sqlac.execute(statement, parameters)
+        result = await self._(q, **parameters)
         mapping_result = result.mappings()
         row = mapping_result.first()
         return row
 
     async def fetch_many(
         self,
-        q: _query.query,
+        q: _query_.query,
         **parameters,
     ) -> typing.Sequence[sqla.RowMapping]:
         """
         Returns the list of the query result.
         """
-        statement = q.render(**parameters)
-        result = await self._sqlac.execute(statement, parameters)
+        result = await self._(q, **parameters)
         mapping_result = result.mappings()
         rows = mapping_result.all()
         return rows
 
     async def execute(
         self,
-        q: _query.query,
+        q: _query_.query,
         **parameters,
     ) -> sqla.Row | None:
         """
         Executes the query and returns the result.
         """
-        statement = q.render(**parameters)
-        result = await self._sqlac.execute(statement, parameters)
+        result = await self._(q, **parameters)
         if result.returns_rows:
             returning = result.one()
             return returning
 
 
 @asynccontextmanager
 async def _make_transaction(
     engine: sqla_engine,
-) -> typing.AsyncIterator[active_transaction]:
+):
     """
     Begin a new transaction.
     """
     async with engine.connect() as sqlac:
         async with sqlac.begin():
             yield active_transaction(sqlac)
 
 
 @asynccontextmanager
 async def new_transaction(
     engine: sqla_engine,
     *,
     use_last: bool = True,
-) -> typing.AsyncIterator[active_transaction]:
-    pretransaction = _make_transaction(engine)
-    async with _transactions_chain.add(
+    pretransaction_factory = _make_transaction
+):
+    pretransaction = pretransaction_factory(engine)
+    async with _transactions_chain_.add(
         pretransaction=pretransaction,
         use_last=use_last,
     ) as transaction:
         yield transaction
```

### Comparing `almasql-0.1.1/almasql/_transactions_chain.py` & `almasql-0.1.2/almasql/_transactions_chain_.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 
 
 @asynccontextmanager
 async def add[T: typing.AsyncContextManager](
     *,
     pretransaction: T,
     use_last: bool = False,
-) -> typing.AsyncIterator[T]:
+):
     """
     Adds a new transaction to the chain if `use_last` is `False` or last active transaction not found.
     Otherwise yields last active transaction.
 
     IMPORTANT! Begin new transaction if __aenter__ was called using `asyncio.create_task`.
 
     Args:
-        - pretransaction: A new transaction that is not began. Must implement `typing.AsyncConextManager`.
+        - pretransaction: A new transaction that is not began. Must implement `typing.AsyncContextManager`.
         - use_last: set `True` if you want to use last active transaction.
     """
     last_transaction = _context_last_transaction.get(None)
 
     if last_transaction is None:
         use_last = False
```

### Comparing `almasql-0.1.1/PKG-INFO` & `almasql-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,58 @@
 Metadata-Version: 2.1
 Name: almasql
-Version: 0.1.1
-Summary: 
+Version: 0.1.2
+Summary: Simple library for dynamic SQL queries
+Home-page: https://github.com/aturkenov/almasql
 License: MIT
+Keywords: SQL,AlmaSQL
 Author: aturkenov
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: greenlet (>=3.0.3,<4.0.0)
 Requires-Dist: jinja2 (>=3.1.4,<4.0.0)
 Requires-Dist: sqlalchemy (>=2.0.30,<3.0.0)
+Project-URL: Documentation, https://github.com/aturkenov/almasql
+Project-URL: Repository, https://github.com/aturkenov/almasql
 Description-Content-Type: text/markdown
 
+AlmaSQL
+
 <details>
 <summary>Directives</summary>
 
 Directives are functions that can extend AlmaSQL by customizing the way an expression renders.
 
 Using a directive in your template is as simple as calling a function in a template expression.
 
-AlmaSQL includes a number of built-in directives like `set_values_by` and `enumerate_values_by`.
+AlmaSQL includes a number of built-in directives like `set` and `values`.
 
 Users can also write their own custom directives.
 
 <details>
-<summary>set_values_by</summary>
+<summary>set</summary>
 
-Imagine table `book` and columns `id`, `title`, and `author`.
+Imagine table `book` and columns `id`, `title`, and `is_active`.
 And you want to update book by id.
 
 ```jinja
 UPDATE book
-SET title = :title, author = :author
+SET title = :title, is_active = :is_active
 WHERE id = :id
 ```
 
 But when you need to modify column, you need to change the query template.
 What if you forgot to do it? This will lead to unexpected bugs.
 So better to use directives that, depending on the arguments,
 will render the required columns and values.
 
 ```jinja
-UPDATE book
-{{ set_values_by(['title', 'author']) }}
+UPDATE book{{ set({'title': 'Why do I love almasql?', 'is_active': True}) }}
 WHERE id = :id
 ```
 </details>
 </details>
```

