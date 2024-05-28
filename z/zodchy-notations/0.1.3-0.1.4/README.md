# Comparing `tmp/zodchy_notations-0.1.3.tar.gz` & `tmp/zodchy_notations-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodchy_notations-0.1.3.tar", max compression
+gzip compressed data, was "zodchy_notations-0.1.4.tar", max compression
```

## Comparing `zodchy_notations-0.1.3.tar` & `zodchy_notations-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        7 2023-08-10 15:42:17.045483 zodchy_notations-0.1.3/README.md
--rw-r--r--   0        0        0      425 2024-05-25 17:34:33.528636 zodchy_notations-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       20 2024-04-27 06:57:44.545249 zodchy_notations-0.1.3/zodchy_notations/__init__.py
--rw-r--r--   0        0        0       19 2024-04-27 06:57:44.549266 zodchy_notations-0.1.3/zodchy_notations/query/__init__.py
--rw-r--r--   0        0        0     8571 2024-04-29 10:48:00.285679 zodchy_notations-0.1.3/zodchy_notations/query/math.py
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 zodchy_notations-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        7 2023-08-10 15:42:17.045483 zodchy_notations-0.1.4/README.md
+-rw-r--r--   0        0        0      425 2024-05-28 08:43:27.078289 zodchy_notations-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       20 2024-04-27 06:57:44.545249 zodchy_notations-0.1.4/zodchy_notations/__init__.py
+-rw-r--r--   0        0        0       19 2024-04-27 06:57:44.549266 zodchy_notations-0.1.4/zodchy_notations/query/__init__.py
+-rw-r--r--   0        0        0     8522 2024-05-28 08:41:25.886324 zodchy_notations-0.1.4/zodchy_notations/query/math.py
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 zodchy_notations-0.1.4/PKG-INFO
```

### Comparing `zodchy_notations-0.1.3/zodchy_notations/query/math.py` & `zodchy_notations-0.1.4/zodchy_notations/query/math.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import datetime
 import typing
 import types
 
 import dateutil.parser
 import functools
 
-from zodchy import codex
+from zodchy import codex, operators
 
 FieldName = str
 FieldType = type
 TypesMapType = codex.query.NotationTypesMap
 QueryType = codex.query.NotationQuery
 
 
@@ -90,33 +90,33 @@
             if v is None:
                 continue
             if k == self._parsing_schema.order_by:
                 yield from self._parse_order_param(v)
             elif k == self._parsing_schema.limit:
                 yield Param(
                     name=self._parsing_schema.limit,
-                    value=codex.query.Limit(int(v))
+                    value=operators.Limit(int(v))
                 )
             elif k == self._parsing_schema.offset:
                 yield Param(
                     name=self._parsing_schema.offset,
-                    value=codex.query.Offset(int(v))
+                    value=operators.Offset(int(v))
                 )
             else:
                 yield self._parse_filter_param(k, v.strip(), types_map)
 
     @staticmethod
     def _parse_order_param(
         names: FieldName
     ) -> collections.abc.Generator[Param, None, None]:
         priority = 0
         for name in names.split(','):
-            direction = codex.query.ASC
+            direction = operators.ASC
             if name.startswith('-'):
-                direction = codex.query.DESC
+                direction = operators.DESC
                 name = name[1:]
             yield Param(
                 name=name,
                 value=direction(priority)
             )
             priority += 1
 
@@ -134,16 +134,16 @@
                 return handler(name, mo.group(1))
 
     def _interval(
         self,
         field_name: str,
         field_value: str,
         operations: tuple[
-            type[codex.query.GT | codex.query.GE],
-            type[codex.query.LT | codex.query.LE]
+            type[operators.GT | operators.GE],
+            type[operators.LT | operators.LE]
         ],
         types_map: TypesMapType
     ) -> Param:
         if types_map[field_name] not in interval_types:
             raise TypeError(
                 f'Interval cannot be calculated for type {types_map[field_name]} for field {field_name}')
 
@@ -153,130 +153,130 @@
 
         left = None
         right = None
         if _data[0]:
             left = operations[0](self._cast(_data[0], types_map[field_name]))
         if _data[1]:
             right = operations[1](self._cast(_data[1], types_map[field_name]))
-        value = codex.query.RANGE(left, right)
+        value = operators.RANGE(left, right)
 
         return Param(name=field_name, value=value)
 
     def _multitude(
         self,
         field_name: str,
         field_value: str,
         types_map: TypesMapType,
         inversion: bool = False,
     ):
-        field_value = codex.query.SET(
+        field_value = operators.SET(
             *(
                 self._cast(v, types_map[field_name])
                 for v in field_value.split(',')
                 if v
             )
         )
 
         if inversion:
-            field_value = codex.query.NOT(field_value)
+            field_value = operators.NOT(field_value)
 
         return Param(
             name=field_name,
             value=field_value
         )
 
     def _literal(
         self,
         field_name: str,
         field_value: str,
-        operation: type[codex.query.FilterBit],
+        operation: type[operators.FilterBit],
         types_map: TypesMapType,
         inversion: bool = False
     ):
         field_value = operation(self._cast(field_value, types_map[field_name]))
 
         if inversion:
-            field_value = codex.query.NOT(field_value)
+            field_value = operators.NOT(field_value)
 
         return Param(
             name=field_name,
             value=field_value,
         )
 
     def _cast(self, value: str, type_: type):
         if cast := self._casting_map.get(type_):
             return cast(value)
         return type_(value)
 
     def _pattern_handler_map(self, types_map: TypesMapType):
         return {
-            re.compile('^(null)$'): lambda x, y: Param(name=x, value=codex.query.IS(None)),
-            re.compile('^(!null)$'): lambda x, y: Param(name=x, value=codex.query.NOT(codex.query.IS(None))),
+            re.compile('^(null)$'): lambda x, y: Param(name=x, value=operators.IS(None)),
+            re.compile('^(!null)$'): lambda x, y: Param(name=x, value=operators.NOT(operators.IS(None))),
             re.compile(r'^\(([\dTZ:\-,.]+)\)$'): functools.partial(
                 self._interval,
-                operations=(codex.query.GT, codex.query.LT),
+                operations=(operators.GT, operators.LT),
                 types_map=types_map
             ),
             re.compile(r'^\[([\dTZ:\-,.]+)\)$'): functools.partial(
                 self._interval,
-                operations=(codex.query.GE, codex.query.LT),
+                operations=(operators.GE, operators.LT),
                 types_map=types_map
             ),
             re.compile(r'^\(([\dTZ:\-,.]+)]$'): functools.partial(
                 self._interval,
-                operations=(codex.query.GT, codex.query.LE),
+                operations=(operators.GT, operators.LE),
                 types_map=types_map
             ),
             re.compile(r'^\[([\dTZ:\-,.]+)]$'): functools.partial(
                 self._interval,
-                operations=(codex.query.GE, codex.query.LE),
+                operations=(operators.GE, operators.LE),
                 types_map=types_map
             ),
             re.compile(r'^!{(.*)}$'): functools.partial(
                 self._multitude,
                 inversion=True,
                 types_map=types_map
             ),
             re.compile(r'^{(.*)}$'): functools.partial(
                 self._multitude,
                 types_map=types_map
             ),
             re.compile(r'^~{2}(.*)$'): functools.partial(
                 self._literal,
-                operation=codex.query.LIKE,
+                operation=operators.LIKE,
                 types_map=types_map
             ),
             re.compile(r'^![~]{2}(.*)$'): functools.partial(
                 self._literal,
-                operation=codex.query.LIKE,
+                operation=operators.LIKE,
                 inversion=True,
                 types_map=types_map
             ),
             re.compile(r'^~(.*)$'): functools.partial(
                 self._literal,
                 operation=functools.partial(
-                    codex.query.LIKE,
+                    operators.LIKE,
                     case_sensitive=True
                 ),
                 types_map=types_map
             ),
             re.compile(r'^!~(.*)$'): functools.partial(
                 self._literal,
                 operation=functools.partial(
-                    codex.query.LIKE,
+                    operators.LIKE,
                     case_sensitive=True
                 ),
                 inversion=True,
                 types_map=types_map
             ),
             re.compile(r'^!(.*)$'): functools.partial(
                 self._literal,
-                operation=codex.query.EQ,
+                operation=operators.EQ,
                 inversion=True,
                 types_map=types_map
             ),
             re.compile(r'(.*)'): functools.partial(
                 self._literal,
-                operation=codex.query.EQ,
+                operation=operators.EQ,
                 types_map=types_map
             )
         }
```

### Comparing `zodchy_notations-0.1.3/PKG-INFO` & `zodchy_notations-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: zodchy-notations
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Home-page: https://github.com/smairon/zodchy-notations
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: python-dateutil (>=2.9.0,<3.0.0)
-Requires-Dist: zodchy (>=0.2.3,<0.3.0)
+Requires-Dist: zodchy (>=0.3.0,<0.4.0)
 Project-URL: Repository, https://github.com/smairon/zodchy-notations
 Description-Content-Type: text/markdown
 
 # Hello
```

