# Comparing `tmp/sql_athame-0.4.0a6.tar.gz` & `tmp/sql_athame-0.4.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_athame-0.4.0a6.tar", max compression
+gzip compressed data, was "sql_athame-0.4.0a7.tar", max compression
```

## Comparing `sql_athame-0.4.0a6.tar` & `sql_athame-0.4.0a7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1076 2024-05-28 00:52:05.048582 sql_athame-0.4.0a6/LICENSE
--rw-r--r--   0        0        0    12086 2024-05-28 00:52:05.048582 sql_athame-0.4.0a6/README.md
--rw-r--r--   0        0        0     2067 2024-05-28 00:52:05.048582 sql_athame-0.4.0a6/pyproject.toml
--rw-r--r--   0        0        0       79 2024-05-28 00:52:05.048582 sql_athame-0.4.0a6/sql_athame/__init__.py
--rw-r--r--   0        0        0    10293 2024-05-28 00:52:05.048582 sql_athame-0.4.0a6/sql_athame/base.py
--rw-r--r--   0        0        0    20848 2024-05-28 00:52:05.048582 sql_athame-0.4.0a6/sql_athame/dataclasses.py
--rw-r--r--   0        0        0      758 2024-05-28 00:52:05.048582 sql_athame-0.4.0a6/sql_athame/escape.py
--rw-r--r--   0        0        0        0 2024-05-28 00:52:05.048582 sql_athame-0.4.0a6/sql_athame/py.typed
--rw-r--r--   0        0        0     1293 2024-05-28 00:52:05.048582 sql_athame-0.4.0a6/sql_athame/sqlalchemy.py
--rw-r--r--   0        0        0      475 2024-05-28 00:52:05.048582 sql_athame-0.4.0a6/sql_athame/types.py
--rw-r--r--   0        0        0    12845 1970-01-01 00:00:00.000000 sql_athame-0.4.0a6/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-28 01:54:49.022634 sql_athame-0.4.0a7/LICENSE
+-rw-r--r--   0        0        0    12086 2024-05-28 01:54:49.022634 sql_athame-0.4.0a7/README.md
+-rw-r--r--   0        0        0     2067 2024-05-28 01:54:49.022634 sql_athame-0.4.0a7/pyproject.toml
+-rw-r--r--   0        0        0       79 2024-05-28 01:54:49.022634 sql_athame-0.4.0a7/sql_athame/__init__.py
+-rw-r--r--   0        0        0    10293 2024-05-28 01:54:49.022634 sql_athame-0.4.0a7/sql_athame/base.py
+-rw-r--r--   0        0        0    22193 2024-05-28 01:54:49.022634 sql_athame-0.4.0a7/sql_athame/dataclasses.py
+-rw-r--r--   0        0        0      758 2024-05-28 01:54:49.022634 sql_athame-0.4.0a7/sql_athame/escape.py
+-rw-r--r--   0        0        0        0 2024-05-28 01:54:49.022634 sql_athame-0.4.0a7/sql_athame/py.typed
+-rw-r--r--   0        0        0     1293 2024-05-28 01:54:49.022634 sql_athame-0.4.0a7/sql_athame/sqlalchemy.py
+-rw-r--r--   0        0        0      475 2024-05-28 01:54:49.022634 sql_athame-0.4.0a7/sql_athame/types.py
+-rw-r--r--   0        0        0    12845 1970-01-01 00:00:00.000000 sql_athame-0.4.0a7/PKG-INFO
```

### Comparing `sql_athame-0.4.0a6/LICENSE` & `sql_athame-0.4.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a6/README.md` & `sql_athame-0.4.0a7/README.md`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a6/pyproject.toml` & `sql_athame-0.4.0a7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql-athame"
-version = "0.4.0-alpha-6"
+version = "0.4.0-alpha-7"
 description = "Python tool for slicing and dicing SQL"
 authors = ["Brian Downing <bdowning@lavos.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bdowning/sql-athame"
 repository = "https://github.com/bdowning/sql-athame"
```

### Comparing `sql_athame-0.4.0a6/sql_athame/base.py` & `sql_athame-0.4.0a7/sql_athame/base.py`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a6/sql_athame/dataclasses.py` & `sql_athame-0.4.0a7/sql_athame/dataclasses.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+import functools
 import uuid
 from collections.abc import AsyncGenerator, Iterable, Mapping
 from dataclasses import Field, InitVar, dataclass, fields
 from typing import (
     Annotated,
     Any,
     Callable,
@@ -25,35 +26,64 @@
 
 Connection: TypeAlias = Any
 Pool: TypeAlias = Any
 
 
 @dataclass
 class ColumnInfo:
-    type: str
-    create_type: str = ""
-    nullable: bool = False
+    type: Optional[str] = None
+    create_type: Optional[str] = None
+    nullable: Optional[bool] = None
     _constraints: tuple[str, ...] = ()
 
     constraints: InitVar[Union[str, Iterable[str], None]] = None
 
     def __post_init__(self, constraints: Union[str, Iterable[str], None]) -> None:
-        if self.create_type == "":
-            self.create_type = self.type
-            self.type = sql_create_type_map.get(self.type.upper(), self.type)
         if constraints is not None:
             if type(constraints) is str:
                 constraints = (constraints,)
             self._constraints = tuple(constraints)
 
+    @staticmethod
+    def merge(a: "ColumnInfo", b: "ColumnInfo") -> "ColumnInfo":
+        return ColumnInfo(
+            type=b.type if b.type is not None else a.type,
+            create_type=b.create_type if b.create_type is not None else a.create_type,
+            nullable=b.nullable if b.nullable is not None else a.nullable,
+            _constraints=(*a._constraints, *b._constraints),
+        )
+
+
+@dataclass
+class ConcreteColumnInfo:
+    type: str
+    create_type: str
+    nullable: bool
+    constraints: tuple[str, ...]
+
+    @staticmethod
+    def from_column_info(name: str, *args: ColumnInfo) -> "ConcreteColumnInfo":
+        info = functools.reduce(ColumnInfo.merge, args, ColumnInfo())
+        if info.create_type is None and info.type is not None:
+            info.create_type = info.type
+            info.type = sql_create_type_map.get(info.type.upper(), info.type)
+        if type(info.type) is not str or type(info.create_type) is not str:
+            raise ValueError(f"Missing SQL type for column {name!r}")
+        return ConcreteColumnInfo(
+            type=info.type,
+            create_type=info.create_type,
+            nullable=bool(info.nullable),
+            constraints=info._constraints,
+        )
+
     def create_table_string(self) -> str:
         parts = (
             self.create_type,
             *(() if self.nullable else ("NOT NULL",)),
-            *self._constraints,
+            *self.constraints,
         )
         return " ".join(parts)
 
 
 sql_create_type_map = {
     "BIGSERIAL": "BIGINT",
     "SERIAL": "INTEGER",
@@ -82,15 +112,15 @@
 
 
 T = TypeVar("T", bound="ModelBase")
 U = TypeVar("U")
 
 
 class ModelBase:
-    _column_info: Optional[dict[str, ColumnInfo]]
+    _column_info: Optional[dict[str, ConcreteColumnInfo]]
     _cache: dict[tuple, Any]
     table_name: str
     primary_key_names: tuple[str, ...]
     array_safe_insert: bool
     _type_hints: dict[str, type]
 
     def __init_subclass__(
@@ -134,27 +164,31 @@
         try:
             return cls._type_hints
         except AttributeError:
             cls._type_hints = get_type_hints(cls, include_extras=True)
             return cls._type_hints
 
     @classmethod
-    def column_info_for_field(cls, field: Field) -> ColumnInfo:
+    def column_info_for_field(cls, field: Field) -> ConcreteColumnInfo:
         type_info = cls.type_hints()[field.name]
         base_type = type_info
         if get_origin(type_info) is Annotated:
             base_type = type_info.__origin__  # type: ignore
+        info = []
+        if base_type in sql_type_map:
+            _type, nullable = sql_type_map[base_type]
+            info.append(ColumnInfo(type=_type, nullable=nullable))
+        if get_origin(type_info) is Annotated:
             for md in type_info.__metadata__:  # type: ignore
                 if isinstance(md, ColumnInfo):
-                    return md
-        type, nullable = sql_type_map[base_type]
-        return ColumnInfo(type=type, nullable=nullable)
+                    info.append(md)
+        return ConcreteColumnInfo.from_column_info(field.name, *info)
 
     @classmethod
-    def column_info(cls, column: str) -> ColumnInfo:
+    def column_info(cls, column: str) -> ConcreteColumnInfo:
         try:
             return cls._column_info[column]  # type: ignore
         except AttributeError:
             cls._column_info = {
                 f.name: cls.column_info_for_field(f) for f in cls._fields()
             }
             return cls._column_info[column]
```

### Comparing `sql_athame-0.4.0a6/sql_athame/escape.py` & `sql_athame-0.4.0a7/sql_athame/escape.py`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a6/sql_athame/sqlalchemy.py` & `sql_athame-0.4.0a7/sql_athame/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a6/PKG-INFO` & `sql_athame-0.4.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-athame
-Version: 0.4.0a6
+Version: 0.4.0a7
 Summary: Python tool for slicing and dicing SQL
 Home-page: https://github.com/bdowning/sql-athame
 License: MIT
 Author: Brian Downing
 Author-email: bdowning@lavos.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

