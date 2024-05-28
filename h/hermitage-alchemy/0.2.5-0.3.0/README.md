# Comparing `tmp/hermitage_alchemy-0.2.5.tar.gz` & `tmp/hermitage_alchemy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermitage_alchemy-0.2.5.tar", max compression
+gzip compressed data, was "hermitage_alchemy-0.3.0.tar", max compression
```

## Comparing `hermitage_alchemy-0.2.5.tar` & `hermitage_alchemy-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      120 2024-04-15 11:40:18.155284 hermitage_alchemy-0.2.5/README.md
--rw-r--r--   0        0        0      504 2024-05-25 14:24:50.954908 hermitage_alchemy-0.2.5/hermitage_alchemy/__init__.py
--rw-r--r--   0        0        0    10439 2024-05-27 14:15:43.102033 hermitage_alchemy-0.2.5/hermitage_alchemy/assembling.py
--rw-r--r--   0        0        0      826 2024-04-13 14:00:09.650913 hermitage_alchemy-0.2.5/hermitage_alchemy/bootstraping.py
--rw-r--r--   0        0        0     7409 2024-05-27 18:32:27.541366 hermitage_alchemy-0.2.5/hermitage_alchemy/configuration.py
--rw-r--r--   0        0        0       24 2024-05-25 14:24:50.956586 hermitage_alchemy-0.2.5/hermitage_alchemy/definition/__init__.py
--rw-r--r--   0        0        0      718 2024-05-26 13:12:45.022518 hermitage_alchemy-0.2.5/hermitage_alchemy/definition/contracts.py
--rw-r--r--   0        0        0       60 2024-05-25 14:24:50.957143 hermitage_alchemy-0.2.5/hermitage_alchemy/execution/__init__.py
--rw-r--r--   0        0        0     6991 2024-05-25 14:24:50.957364 hermitage_alchemy-0.2.5/hermitage_alchemy/execution/read.py
--rw-r--r--   0        0        0     1840 2024-05-27 17:39:40.830848 hermitage_alchemy-0.2.5/hermitage_alchemy/execution/write.py
--rw-r--r--   0        0        0      415 2024-05-27 18:33:33.512379 hermitage_alchemy-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 hermitage_alchemy-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      120 2024-04-15 11:40:18.155284 hermitage_alchemy-0.3.0/README.md
+-rw-r--r--   0        0        0      504 2024-05-25 14:24:50.954908 hermitage_alchemy-0.3.0/hermitage_alchemy/__init__.py
+-rw-r--r--   0        0        0    10393 2024-05-28 08:51:26.557813 hermitage_alchemy-0.3.0/hermitage_alchemy/assembling.py
+-rw-r--r--   0        0        0      826 2024-04-13 14:00:09.650913 hermitage_alchemy-0.3.0/hermitage_alchemy/bootstraping.py
+-rw-r--r--   0        0        0     7409 2024-05-27 18:32:27.541366 hermitage_alchemy-0.3.0/hermitage_alchemy/configuration.py
+-rw-r--r--   0        0        0       24 2024-05-25 14:24:50.956586 hermitage_alchemy-0.3.0/hermitage_alchemy/definition/__init__.py
+-rw-r--r--   0        0        0      718 2024-05-26 13:12:45.022518 hermitage_alchemy-0.3.0/hermitage_alchemy/definition/contracts.py
+-rw-r--r--   0        0        0       60 2024-05-25 14:24:50.957143 hermitage_alchemy-0.3.0/hermitage_alchemy/execution/__init__.py
+-rw-r--r--   0        0        0     6987 2024-05-28 08:51:26.552502 hermitage_alchemy-0.3.0/hermitage_alchemy/execution/read.py
+-rw-r--r--   0        0        0     1840 2024-05-27 17:39:40.830848 hermitage_alchemy-0.3.0/hermitage_alchemy/execution/write.py
+-rw-r--r--   0        0        0      415 2024-05-28 08:31:33.385070 hermitage_alchemy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 hermitage_alchemy-0.3.0/PKG-INFO
```

### Comparing `hermitage_alchemy-0.2.5/hermitage_alchemy/assembling.py` & `hermitage_alchemy-0.3.0/hermitage_alchemy/assembling.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,25 +47,25 @@
     def _compile(self, expression: ClauseExpression) -> sqlalchemy.ClauseElement: ...
 
 
 class FilterCompiler(ClauseCompiler):
     @property
     def _operations(self):
         return {
-            zodchy.codex.query.EQ: self._simple_clause(operator.eq),
-            zodchy.codex.query.NE: self._simple_clause(operator.ne),
-            zodchy.codex.query.LE: self._simple_clause(operator.le),
-            zodchy.codex.query.LT: self._simple_clause(operator.lt),
-            zodchy.codex.query.GE: self._simple_clause(operator.ge),
-            zodchy.codex.query.GT: self._simple_clause(operator.gt),
-            zodchy.codex.query.IS: lambda v: self._get_column(v).is_(v.operation.value),
-            zodchy.codex.query.LIKE: self._like_clause,
-            zodchy.codex.query.NOT: self._not_clause,
-            zodchy.codex.query.SET: self._set_clause,
-            zodchy.codex.query.RANGE: self._range_clause,
+            zodchy.operators.EQ: self._simple_clause(operator.eq),
+            zodchy.operators.NE: self._simple_clause(operator.ne),
+            zodchy.operators.LE: self._simple_clause(operator.le),
+            zodchy.operators.LT: self._simple_clause(operator.lt),
+            zodchy.operators.GE: self._simple_clause(operator.ge),
+            zodchy.operators.GT: self._simple_clause(operator.gt),
+            zodchy.operators.IS: lambda v: self._get_column(v).is_(v.operation.value),
+            zodchy.operators.LIKE: self._like_clause,
+            zodchy.operators.NOT: self._not_clause,
+            zodchy.operators.SET: self._set_clause,
+            zodchy.operators.RANGE: self._range_clause,
         }
 
     def _compile(self, expression: ClauseExpression) -> sqlalchemy.ClauseElement:
         stack = deque()
         for element in expression:
             if element is AND:
                 a = stack.pop()
@@ -78,24 +78,24 @@
 
         return stack.pop()
 
     def _get_column(self, clause: Clause) -> sqlalchemy.Column:
         return self._schema.get_column(Address(clause.name, self._space))
 
     def _not_clause(self, clause: Clause):
-        if isinstance(clause.operation, zodchy.codex.query.IS):
+        if isinstance(clause.operation, zodchy.operators.IS):
             return self._get_column(clause).isnot(clause.operation.value)
-        elif isinstance(clause.operation, zodchy.codex.query.EQ):
+        elif isinstance(clause.operation, zodchy.operators.EQ):
             return operator.ne(self._get_column(clause), clause.operation.value)
-        elif isinstance(clause.operation, zodchy.codex.query.LIKE):
+        elif isinstance(clause.operation, zodchy.operators.LIKE):
             return self._like_clause(
                 Clause(clause.name, clause.operation),
                 inversion=True
             )
-        elif isinstance(clause.operation, zodchy.codex.query.SET):
+        elif isinstance(clause.operation, zodchy.operators.SET):
             return self._set_clause(
                 Clause(clause.name, clause.operation),
                 inversion=True
             )
         else:
             return sqlalchemy.not_(self._compile(clause)),
 
@@ -137,16 +137,16 @@
     def __call__(self, clause: ClauseExpression) -> list[sqlalchemy.ClauseElement]:
         result = self._compile(clause)
         return result
 
     @property
     def _operations(self):
         return {
-            zodchy.codex.query.ASC: sqlalchemy.asc,
-            zodchy.codex.query.DESC: sqlalchemy.desc
+            zodchy.operators.ASC: sqlalchemy.asc,
+            zodchy.operators.DESC: sqlalchemy.desc
         }
 
     def _compile(self, expression: ClauseExpression) -> list[sqlalchemy.ClauseElement]:
         stack = deque()
         result = []
         for element in expression or ():
             if element is AND:
@@ -239,27 +239,27 @@
                 elif isinstance(_value, collections.abc.Mapping):
                     self._values.append(_value)
             elif isinstance(element, Total):
                 self._select.append(
                     sqlalchemy.text(f"count(*) over () as {TOTAL_QUERY_FIELD}")
                 )
             elif isinstance(element, Clause):
-                if isinstance(element.operation, zodchy.codex.query.FilterBit):
+                if isinstance(element.operation, zodchy.operators.FilterBit):
                     _filter_clause = ClauseExpression(element) if _filter_clause is None else _filter_clause & element
-                elif isinstance(element.operation, zodchy.codex.query.OrderBit):
+                elif isinstance(element.operation, zodchy.operators.OrderBit):
                     _order_clause = ClauseExpression(element) if _order_clause is None else _order_clause & element
             elif isinstance(element, Slice):
-                if isinstance(element.operation, zodchy.codex.query.Limit):
+                if isinstance(element.operation, zodchy.operators.Limit):
                     _limit_clause = element.operation.value
-                elif isinstance(element.operation, zodchy.codex.query.Offset):
+                elif isinstance(element.operation, zodchy.operators.Offset):
                     _offset_clause = element.operation.value
             elif isinstance(element, ClauseExpression):
-                if isinstance(element[0].operation, zodchy.codex.query.FilterBit):
+                if isinstance(element[0].operation, zodchy.operators.FilterBit):
                     _filter_clause = element if _filter_clause is None else _filter_clause & element
-                elif isinstance(element[0].operation, zodchy.codex.query.OrderBit):
+                elif isinstance(element[0].operation, zodchy.operators.OrderBit):
                     _order_clause = element if _order_clause is None else _order_clause & element
 
         if _filter_clause:
             filter_compiler = self._filter_compiler.get_instance(bucket_space)
             self._filters.append(filter_compiler(_filter_clause))
 
         if _order_clause:
```

### Comparing `hermitage_alchemy-0.2.5/hermitage_alchemy/bootstraping.py` & `hermitage_alchemy-0.3.0/hermitage_alchemy/bootstraping.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.2.5/hermitage_alchemy/configuration.py` & `hermitage_alchemy-0.3.0/hermitage_alchemy/configuration.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.2.5/hermitage_alchemy/definition/contracts.py` & `hermitage_alchemy-0.3.0/hermitage_alchemy/definition/contracts.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.2.5/hermitage_alchemy/execution/read.py` & `hermitage_alchemy-0.3.0/hermitage_alchemy/execution/read.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         # Nested buckets calculation
         for nested_bucket, link, substitution_name in nested_buckets:
             if isinstance(link, O2M):
                 index_key = (substitution_name, link.source_address.name)
                 nested_bucket += Item(link.target_address.name)
                 nested_bucket += Clause(
                     link.target_address.name,
-                    zodchy.codex.query.SET(*(e[link.source_address.name] for e in bucket_data))
+                    zodchy.operators.SET(*(e[link.source_address.name] for e in bucket_data))
                 )
                 nested_view = await self(nested_bucket, True)
                 nested_indexed_data[index_key] = self._index_data(
                     data=nested_view.data,
                     key=link.target_address.name,
                     transformer=lambda r: {
                         k: v
@@ -131,15 +131,15 @@
             elif isinstance(link, M2M):
                 index_key = (substitution_name, link.source_address.name)
                 nested_bucket = Bucket(
                     link.interim_source_address.space.last,
                     Item(link.interim_source_address.name),
                     Clause(
                         link.interim_source_address.name,
-                        zodchy.codex.query.SET(*(e[link.source_address.name] for e in bucket_data))
+                        zodchy.operators.SET(*(e[link.source_address.name] for e in bucket_data))
                     ),
                     nested_bucket + Item(link.target_address.name)
                 )
                 nested_view = await self(nested_bucket, True)
                 nested_indexed_data[index_key] = self._index_data(
                     data=nested_view.data,
                     key=link.interim_source_address.name,
```

### Comparing `hermitage_alchemy-0.2.5/hermitage_alchemy/execution/write.py` & `hermitage_alchemy-0.3.0/hermitage_alchemy/execution/write.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.2.5/PKG-INFO` & `hermitage_alchemy-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: hermitage-alchemy
-Version: 0.2.5
+Version: 0.3.0
 Summary: Implementation of hermitage contracts for sqlalchemy engine
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: hermitage (>=0.2.0,<0.3.0)
+Requires-Dist: hermitage (>=0.3.0,<0.4.0)
 Requires-Dist: sqlalchemy (>=2.0.20,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Hermitage Alchemy
 
 Implementation of [hermitage](https://github.com/smairon/hermitage) contracts for sqlalchemy engine
```

