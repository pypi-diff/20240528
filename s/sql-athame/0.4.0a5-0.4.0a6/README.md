# Comparing `tmp/sql_athame-0.4.0a5.tar.gz` & `tmp/sql_athame-0.4.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_athame-0.4.0a5.tar", max compression
+gzip compressed data, was "sql_athame-0.4.0a6.tar", max compression
```

## Comparing `sql_athame-0.4.0a5.tar` & `sql_athame-0.4.0a6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1076 2024-04-18 14:38:46.803742 sql_athame-0.4.0a5/LICENSE
--rw-r--r--   0        0        0    12086 2024-04-18 14:38:46.803742 sql_athame-0.4.0a5/README.md
--rw-r--r--   0        0        0      751 2024-04-18 14:38:46.807742 sql_athame-0.4.0a5/pyproject.toml
--rw-r--r--   0        0        0      130 2024-04-18 14:38:46.807742 sql_athame-0.4.0a5/sql_athame/__init__.py
--rw-r--r--   0        0        0    10350 2024-04-18 14:38:46.807742 sql_athame-0.4.0a5/sql_athame/base.py
--rw-r--r--   0        0        0    20442 2024-04-18 14:38:46.807742 sql_athame-0.4.0a5/sql_athame/dataclasses.py
--rw-r--r--   0        0        0      743 2024-04-18 14:38:46.807742 sql_athame-0.4.0a5/sql_athame/escape.py
--rw-r--r--   0        0        0        0 2024-04-18 14:38:46.807742 sql_athame-0.4.0a5/sql_athame/py.typed
--rw-r--r--   0        0        0     1305 2024-04-18 14:38:46.807742 sql_athame-0.4.0a5/sql_athame/sqlalchemy.py
--rw-r--r--   0        0        0      412 2024-04-18 14:38:46.807742 sql_athame-0.4.0a5/sql_athame/types.py
--rw-r--r--   0        0        0    12845 1970-01-01 00:00:00.000000 sql_athame-0.4.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-28 00:52:05.048582 sql_athame-0.4.0a6/LICENSE
+-rw-r--r--   0        0        0    12086 2024-05-28 00:52:05.048582 sql_athame-0.4.0a6/README.md
+-rw-r--r--   0        0        0     2067 2024-05-28 00:52:05.048582 sql_athame-0.4.0a6/pyproject.toml
+-rw-r--r--   0        0        0       79 2024-05-28 00:52:05.048582 sql_athame-0.4.0a6/sql_athame/__init__.py
+-rw-r--r--   0        0        0    10293 2024-05-28 00:52:05.048582 sql_athame-0.4.0a6/sql_athame/base.py
+-rw-r--r--   0        0        0    20848 2024-05-28 00:52:05.048582 sql_athame-0.4.0a6/sql_athame/dataclasses.py
+-rw-r--r--   0        0        0      758 2024-05-28 00:52:05.048582 sql_athame-0.4.0a6/sql_athame/escape.py
+-rw-r--r--   0        0        0        0 2024-05-28 00:52:05.048582 sql_athame-0.4.0a6/sql_athame/py.typed
+-rw-r--r--   0        0        0     1293 2024-05-28 00:52:05.048582 sql_athame-0.4.0a6/sql_athame/sqlalchemy.py
+-rw-r--r--   0        0        0      475 2024-05-28 00:52:05.048582 sql_athame-0.4.0a6/sql_athame/types.py
+-rw-r--r--   0        0        0    12845 1970-01-01 00:00:00.000000 sql_athame-0.4.0a6/PKG-INFO
```

### Comparing `sql_athame-0.4.0a5/LICENSE` & `sql_athame-0.4.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a5/README.md` & `sql_athame-0.4.0a6/README.md`

 * *Files identical despite different names*

### Comparing `sql_athame-0.4.0a5/sql_athame/base.py` & `sql_athame-0.4.0a6/sql_athame/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 import dataclasses
 import json
 import re
 import string
+from collections.abc import Iterable, Iterator, Sequence
 from typing import (
     Any,
     Callable,
-    Dict,
-    Iterable,
-    Iterator,
-    List,
     Optional,
-    Sequence,
-    Tuple,
     Union,
     cast,
     overload,
 )
 
 from typing_extensions import Literal
 
@@ -30,30 +25,30 @@
 def auto_numbered(field_name):
     return not auto_numbered_re.match(field_name)
 
 
 def process_slot_value(
     name: str,
     value: Any,
-    placeholders: Dict[str, Placeholder],
+    placeholders: dict[str, Placeholder],
 ) -> Union["Fragment", Placeholder]:
     if isinstance(value, Fragment):
         return value
     else:
         if name not in placeholders:
             placeholders[name] = Placeholder(name, value)
         return placeholders[name]
 
 
 @dataclasses.dataclass
 class Fragment:
     __slots__ = ["parts"]
-    parts: List[Part]
+    parts: list[Part]
 
-    def flatten_into(self, parts: List[FlatPart]) -> None:
+    def flatten_into(self, parts: list[FlatPart]) -> None:
         for part in self.parts:
             if isinstance(part, Fragment):
                 part.flatten_into(parts)
             else:
                 parts.append(part)
 
     def compile(self) -> Callable[..., "Fragment"]:
@@ -66,100 +61,100 @@
             "def compiled(**slots):",
             " placeholders = {}",
             " return Fragment([",
         ]
         for i, part in enumerate(flattened.parts):
             if isinstance(part, Slot):
                 func.append(
-                    f"  process_slot_value({repr(part.name)}, slots[{repr(part.name)}], placeholders),"
+                    f"  process_slot_value({part.name!r}, slots[{part.name!r}], placeholders),"
                 )
             elif isinstance(part, str):
-                func.append(f"  {repr(part)},")
+                func.append(f"  {part!r},")
             else:
                 env[f"part_{i}"] = part
                 func.append(f"  part_{i},")
         func += [" ])"]
         exec("\n".join(func), env)
         return env["compiled"]  # type: ignore
 
     def flatten(self) -> "Fragment":
-        parts: List[FlatPart] = []
+        parts: list[FlatPart] = []
         self.flatten_into(parts)
-        out_parts: List[Part] = []
+        out_parts: list[Part] = []
         for part in parts:
             if isinstance(part, str) and out_parts and isinstance(out_parts[-1], str):
                 out_parts[-1] += part
             else:
                 out_parts.append(part)
         return Fragment(out_parts)
 
     def fill(self, **kwargs: Any) -> "Fragment":
-        parts: List[Part] = []
-        self.flatten_into(cast(List[FlatPart], parts))
-        placeholders: Dict[str, Placeholder] = {}
+        parts: list[Part] = []
+        self.flatten_into(cast(list[FlatPart], parts))
+        placeholders: dict[str, Placeholder] = {}
         for i, part in enumerate(parts):
             if isinstance(part, Slot):
                 parts[i] = process_slot_value(
                     part.name, kwargs[part.name], placeholders
                 )
         return Fragment(parts)
 
     @overload
     def prep_query(
         self, allow_slots: Literal[True]
-    ) -> Tuple[str, List[Union[Placeholder, Slot]]]: ...  # pragma: no cover
+    ) -> tuple[str, list[Union[Placeholder, Slot]]]: ...  # pragma: no cover
 
     @overload
     def prep_query(
         self, allow_slots: Literal[False] = False
-    ) -> Tuple[str, List[Placeholder]]: ...  # pragma: no cover
+    ) -> tuple[str, list[Placeholder]]: ...  # pragma: no cover
 
-    def prep_query(self, allow_slots: bool = False) -> Tuple[str, List[Any]]:
-        parts: List[FlatPart] = []
+    def prep_query(self, allow_slots: bool = False) -> tuple[str, list[Any]]:
+        parts: list[FlatPart] = []
         self.flatten_into(parts)
-        args: List[Union[Placeholder, Slot]] = []
-        placeholder_ids: Dict[Placeholder, int] = {}
-        slot_ids: Dict[Slot, int] = {}
-        out_parts: List[str] = []
+        args: list[Union[Placeholder, Slot]] = []
+        placeholder_ids: dict[Placeholder, int] = {}
+        slot_ids: dict[Slot, int] = {}
+        out_parts: list[str] = []
         for part in parts:
             if isinstance(part, Slot):
                 if not allow_slots:
-                    raise ValueError(f"Unfilled slot: {repr(part.name)}")
+                    raise ValueError(f"Unfilled slot: {part.name!r}")
                 if part not in slot_ids:
                     args.append(part)
                     slot_ids[part] = len(args)
                 out_parts.append(f"${slot_ids[part]}")
             elif isinstance(part, Placeholder):
                 if part not in placeholder_ids:
                     args.append(part)
                     placeholder_ids[part] = len(args)
                 out_parts.append(f"${placeholder_ids[part]}")
             else:
                 assert isinstance(part, str)
                 out_parts.append(part)
         return "".join(out_parts).strip(), args
 
-    def query(self) -> Tuple[str, List[Any]]:
+    def query(self) -> tuple[str, list[Any]]:
         query, args = self.prep_query()
         placeholder_values = [arg.value for arg in args]
         return query, placeholder_values
 
     def sqlalchemy_text(self) -> Any:
         return sqlalchemy_text_from_fragment(self)
 
-    def prepare(self) -> Tuple[str, Callable[..., List[Any]]]:
+    def prepare(self) -> tuple[str, Callable[..., list[Any]]]:
         query, args = self.prep_query(allow_slots=True)
-        env = dict()
+        env = {}
         func = [
             "def generate_args(**kwargs):",
             " return [",
         ]
         for i, arg in enumerate(args):
             if isinstance(arg, Slot):
-                func.append(f"  kwargs[{repr(arg.name)}],")
+                func.append(f"  kwargs[{arg.name!r}],")
             else:
                 env[f"value_{i}"] = arg.value
                 func.append(f"  value_{i},")
         func += [" ]"]
         exec("\n".join(func), env)
         return query, env["generate_args"]  # type: ignore
 
@@ -174,18 +169,18 @@
 class SQLFormatter:
     def __call__(
         self, fmt: str, *args: Any, preserve_formatting: bool = False, **kwargs: Any
     ) -> Fragment:
         if not preserve_formatting:
             fmt = newline_whitespace_re.sub(" ", fmt)
         fmtr = string.Formatter()
-        parts: List[Part] = []
-        placeholders: Dict[str, Placeholder] = {}
+        parts: list[Part] = []
+        placeholders: dict[str, Placeholder] = {}
         next_auto_field = 0
-        for literal_text, field_name, format_spec, conversion in fmtr.parse(fmt):
+        for literal_text, field_name, _format_spec, _conversion in fmtr.parse(fmt):
             parts.append(literal_text)
             if field_name is not None:
                 if auto_numbered(field_name):
                     field_name = f"{next_auto_field}{field_name}"
                     next_auto_field += 1
                 try:
                     value = fmtr.get_field(field_name, args, kwargs)[0]
@@ -254,20 +249,19 @@
     def list(self, *parts: Fragment) -> Fragment: ...  # pragma: no cover
 
     def list(self, *parts) -> Fragment:  # type: ignore
         if parts and not isinstance(parts[0], Fragment):
             parts = parts[0]
         return Fragment(list(join_parts(parts, infix=", ")))
 
-    @staticmethod
-    def unnest(data: Iterable[Sequence[Any]], types: Iterable[str]) -> Fragment:
-        nested = list(nest_for_type(x, t) for x, t in zip(zip(*data), types))
+    def unnest(self, data: Iterable[Sequence[Any]], types: Iterable[str]) -> Fragment:
+        nested = [nest_for_type(x, t) for x, t in zip(zip(*data), types)]
         if not nested:
-            nested = list(nest_for_type([], t) for t in types)
-        return Fragment(["UNNEST(", sql.list(nested), ")"])
+            nested = [nest_for_type([], t) for t in types]
+        return Fragment(["UNNEST(", self.list(nested), ")"])
 
 
 sql = SQLFormatter()
 
 
 json_types = ("JSON", "JSONB")
 
@@ -292,15 +286,15 @@
         return Fragment([Placeholder("data", data), f"::{typename}[]"])
 
 
 def lit(text: str) -> Fragment:
     return Fragment([text])
 
 
-def any_all(frags: List[Fragment], op: str, base_case: str) -> Fragment:
+def any_all(frags: list[Fragment], op: str, base_case: str) -> Fragment:
     if not frags:
         return lit(base_case)
     parts = join_parts(frags, prefix="(", infix=f") {op} (", suffix=")")
     return Fragment(list(parts))
 
 
 def join_parts(
```

### Comparing `sql_athame-0.4.0a5/sql_athame/dataclasses.py` & `sql_athame-0.4.0a6/sql_athame/dataclasses.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,110 +1,101 @@
 import datetime
 import uuid
-from dataclasses import dataclass, field, fields
+from collections.abc import AsyncGenerator, Iterable, Mapping
+from dataclasses import Field, InitVar, dataclass, fields
 from typing import (
+    Annotated,
     Any,
-    AsyncGenerator,
     Callable,
-    Dict,
-    Iterable,
-    Iterator,
-    List,
-    Mapping,
     Optional,
-    Set,
-    Tuple,
-    Type,
     TypeVar,
     Union,
+    get_origin,
+    get_type_hints,
 )
 
+from typing_extensions import TypeAlias
+
 from .base import Fragment, sql
 
-Where = Union[Fragment, Iterable[Fragment]]
+Where: TypeAlias = Union[Fragment, Iterable[Fragment]]
 # KLUDGE to avoid a string argument being valid
-SequenceOfStrings = Union[List[str], Tuple[str, ...]]
-FieldNames = SequenceOfStrings
-FieldNamesSet = Union[SequenceOfStrings, Set[str]]
+SequenceOfStrings: TypeAlias = Union[list[str], tuple[str, ...]]
+FieldNames: TypeAlias = SequenceOfStrings
+FieldNamesSet: TypeAlias = Union[SequenceOfStrings, set[str]]
 
-Connection = Any
-Pool = Any
+Connection: TypeAlias = Any
+Pool: TypeAlias = Any
 
 
 @dataclass
 class ColumnInfo:
     type: str
-    create_type: str
-    constraints: Tuple[str, ...]
-
-    def create_table_string(self):
-        return " ".join((self.create_type, *self.constraints))
-
-
-def model_field_metadata(
-    type: str, constraints: Union[str, Iterable[str]] = ()
-) -> Dict[str, Any]:
-    if isinstance(constraints, str):
-        constraints = (constraints,)
-    info = ColumnInfo(
-        sql_create_type_map.get(type.upper(), type), type, tuple(constraints)
-    )
-    return {"sql_athame": info}
-
-
-def model_field(
-    *, type: str, constraints: Union[str, Iterable[str]] = (), **kwargs: Any
-) -> Any:
-    return field(**kwargs, metadata=model_field_metadata(type, constraints))
+    create_type: str = ""
+    nullable: bool = False
+    _constraints: tuple[str, ...] = ()
+
+    constraints: InitVar[Union[str, Iterable[str], None]] = None
+
+    def __post_init__(self, constraints: Union[str, Iterable[str], None]) -> None:
+        if self.create_type == "":
+            self.create_type = self.type
+            self.type = sql_create_type_map.get(self.type.upper(), self.type)
+        if constraints is not None:
+            if type(constraints) is str:
+                constraints = (constraints,)
+            self._constraints = tuple(constraints)
+
+    def create_table_string(self) -> str:
+        parts = (
+            self.create_type,
+            *(() if self.nullable else ("NOT NULL",)),
+            *self._constraints,
+        )
+        return " ".join(parts)
 
 
 sql_create_type_map = {
     "BIGSERIAL": "BIGINT",
     "SERIAL": "INTEGER",
     "SMALLSERIAL": "SMALLINT",
 }
 
 
-sql_type_map = {
-    Optional[bool]: ("BOOLEAN",),
-    Optional[bytes]: ("BYTEA",),
-    Optional[datetime.date]: ("DATE",),
-    Optional[datetime.datetime]: ("TIMESTAMP",),
-    Optional[float]: ("DOUBLE PRECISION",),
-    Optional[int]: ("INTEGER",),
-    Optional[str]: ("TEXT",),
-    Optional[uuid.UUID]: ("UUID",),
-    bool: ("BOOLEAN", "NOT NULL"),
-    bytes: ("BYTEA", "NOT NULL"),
-    datetime.date: ("DATE", "NOT NULL"),
-    datetime.datetime: ("TIMESTAMP", "NOT NULL"),
-    float: ("DOUBLE PRECISION", "NOT NULL"),
-    int: ("INTEGER", "NOT NULL"),
-    str: ("TEXT", "NOT NULL"),
-    uuid.UUID: ("UUID", "NOT NULL"),
+sql_type_map: dict[Any, tuple[str, bool]] = {
+    Optional[bool]: ("BOOLEAN", True),
+    Optional[bytes]: ("BYTEA", True),
+    Optional[datetime.date]: ("DATE", True),
+    Optional[datetime.datetime]: ("TIMESTAMP", True),
+    Optional[float]: ("DOUBLE PRECISION", True),
+    Optional[int]: ("INTEGER", True),
+    Optional[str]: ("TEXT", True),
+    Optional[uuid.UUID]: ("UUID", True),
+    bool: ("BOOLEAN", False),
+    bytes: ("BYTEA", False),
+    datetime.date: ("DATE", False),
+    datetime.datetime: ("TIMESTAMP", False),
+    float: ("DOUBLE PRECISION", False),
+    int: ("INTEGER", False),
+    str: ("TEXT", False),
+    uuid.UUID: ("UUID", False),
 }
 
 
-def column_info_for_field(field):
-    if "sql_athame" in field.metadata:
-        return field.metadata["sql_athame"]
-    type, *constraints = sql_type_map[field.type]
-    return ColumnInfo(type, type, tuple(constraints))
-
-
 T = TypeVar("T", bound="ModelBase")
 U = TypeVar("U")
 
 
-class ModelBase(Mapping[str, Any]):
-    _column_info: Optional[Dict[str, ColumnInfo]]
-    _cache: Dict[tuple, Any]
+class ModelBase:
+    _column_info: Optional[dict[str, ColumnInfo]]
+    _cache: dict[tuple, Any]
     table_name: str
-    primary_key_names: Tuple[str, ...]
+    primary_key_names: tuple[str, ...]
     array_safe_insert: bool
+    _type_hints: dict[str, type]
 
     def __init_subclass__(
         cls,
         *,
         table_name: str,
         primary_key: Union[FieldNames, str] = (),
         insert_multiple_mode: str = "unnest",
@@ -134,109 +125,116 @@
     def _cached(cls, key: tuple, thunk: Callable[[], U]) -> U:
         try:
             return cls._cache[key]
         except KeyError:
             cls._cache[key] = thunk()
             return cls._cache[key]
 
-    def keys(self):
-        return self.field_names()
-
-    def __getitem__(self, key: str) -> Any:
-        return getattr(self, key)
-
-    def __iter__(self) -> Iterator[Any]:
-        return iter(self.keys())
-
-    def __len__(self) -> int:
-        return len(self.keys())
+    @classmethod
+    def type_hints(cls) -> dict[str, type]:
+        try:
+            return cls._type_hints
+        except AttributeError:
+            cls._type_hints = get_type_hints(cls, include_extras=True)
+            return cls._type_hints
 
-    def get(self, key: str, default: Any = None) -> Any:
-        return getattr(self, key, default)
+    @classmethod
+    def column_info_for_field(cls, field: Field) -> ColumnInfo:
+        type_info = cls.type_hints()[field.name]
+        base_type = type_info
+        if get_origin(type_info) is Annotated:
+            base_type = type_info.__origin__  # type: ignore
+            for md in type_info.__metadata__:  # type: ignore
+                if isinstance(md, ColumnInfo):
+                    return md
+        type, nullable = sql_type_map[base_type]
+        return ColumnInfo(type=type, nullable=nullable)
 
     @classmethod
     def column_info(cls, column: str) -> ColumnInfo:
         try:
             return cls._column_info[column]  # type: ignore
         except AttributeError:
-            cls._column_info = {f.name: column_info_for_field(f) for f in cls._fields()}
+            cls._column_info = {
+                f.name: cls.column_info_for_field(f) for f in cls._fields()
+            }
             return cls._column_info[column]
 
     @classmethod
     def table_name_sql(cls, *, prefix: Optional[str] = None) -> Fragment:
         return sql.identifier(cls.table_name, prefix=prefix)
 
     @classmethod
-    def primary_key_names_sql(cls, *, prefix: Optional[str] = None) -> List[Fragment]:
+    def primary_key_names_sql(cls, *, prefix: Optional[str] = None) -> list[Fragment]:
         return [sql.identifier(pk, prefix=prefix) for pk in cls.primary_key_names]
 
     @classmethod
-    def field_names(cls, *, exclude: FieldNamesSet = ()) -> List[str]:
+    def field_names(cls, *, exclude: FieldNamesSet = ()) -> list[str]:
         return [f.name for f in cls._fields() if f.name not in exclude]
 
     @classmethod
     def field_names_sql(
         cls, *, prefix: Optional[str] = None, exclude: FieldNamesSet = ()
-    ) -> List[Fragment]:
+    ) -> list[Fragment]:
         return [
             sql.identifier(f, prefix=prefix) for f in cls.field_names(exclude=exclude)
         ]
 
     def primary_key(self) -> tuple:
         return tuple(getattr(self, pk) for pk in self.primary_key_names)
 
     @classmethod
     def _get_field_values_fn(
-        cls: Type[T], exclude: FieldNamesSet = ()
-    ) -> Callable[[T], List[Any]]:
-        env: Dict[str, Any] = dict()
+        cls: type[T], exclude: FieldNamesSet = ()
+    ) -> Callable[[T], list[Any]]:
+        env: dict[str, Any] = {}
         func = ["def get_field_values(self): return ["]
         for f in cls._fields():
             if f.name not in exclude:
                 func.append(f"self.{f.name},")
         func += ["]"]
         exec(" ".join(func), env)
         return env["get_field_values"]
 
-    def field_values(self, *, exclude: FieldNamesSet = ()) -> List[Any]:
+    def field_values(self, *, exclude: FieldNamesSet = ()) -> list[Any]:
         get_field_values = self._cached(
             ("get_field_values", tuple(sorted(exclude))),
             lambda: self._get_field_values_fn(exclude),
         )
         return get_field_values(self)
 
     def field_values_sql(
         self, *, exclude: FieldNamesSet = (), default_none: bool = False
-    ) -> List[Fragment]:
+    ) -> list[Fragment]:
         if default_none:
             return [
                 sql.literal("DEFAULT") if value is None else sql.value(value)
                 for value in self.field_values()
             ]
         else:
             return [sql.value(value) for value in self.field_values()]
 
     @classmethod
     def from_tuple(
-        cls: Type[T], tup: tuple, *, offset: int = 0, exclude: FieldNamesSet = ()
+        cls: type[T], tup: tuple, *, offset: int = 0, exclude: FieldNamesSet = ()
     ) -> T:
         names = (f.name for f in cls._fields() if f.name not in exclude)
         kwargs = {name: tup[offset] for offset, name in enumerate(names, start=offset)}
         return cls(**kwargs)
 
     @classmethod
     def from_dict(
-        cls: Type[T], dct: Dict[str, Any], *, exclude: FieldNamesSet = ()
+        cls: type[T], dct: dict[str, Any], *, exclude: FieldNamesSet = ()
     ) -> T:
         names = {f.name for f in cls._fields() if f.name not in exclude}
         kwargs = {k: v for k, v in dct.items() if k in names}
         return cls(**kwargs)
 
     @classmethod
-    def ensure_model(cls: Type[T], row: Union[T, Mapping[str, Any]]) -> T:
+    def ensure_model(cls: type[T], row: Union[T, Mapping[str, Any]]) -> T:
         if isinstance(row, cls):
             return row
         return cls(**row)
 
     @classmethod
     def create_table_sql(cls) -> Fragment:
         entries = [
@@ -282,55 +280,55 @@
         query = cached(where=where)
         if for_update:
             query = Fragment([query, " FOR UPDATE"])
         return query
 
     @classmethod
     async def select_cursor(
-        cls: Type[T],
+        cls: type[T],
         connection: Connection,
         order_by: Union[FieldNames, str] = (),
         for_update: bool = False,
         where: Where = (),
         prefetch: int = 1000,
     ) -> AsyncGenerator[T, None]:
         async for row in connection.cursor(
             *cls.select_sql(order_by=order_by, for_update=for_update, where=where),
             prefetch=prefetch,
         ):
             yield cls(**row)
 
     @classmethod
     async def select(
-        cls: Type[T],
+        cls: type[T],
         connection_or_pool: Union[Connection, Pool],
         order_by: Union[FieldNames, str] = (),
         for_update: bool = False,
         where: Where = (),
-    ) -> List[T]:
+    ) -> list[T]:
         return [
             cls(**row)
             for row in await connection_or_pool.fetch(
                 *cls.select_sql(order_by=order_by, for_update=for_update, where=where)
             )
         ]
 
     @classmethod
-    def create_sql(cls: Type[T], **kwargs: Any) -> Fragment:
+    def create_sql(cls: type[T], **kwargs: Any) -> Fragment:
         return sql(
             "INSERT INTO {table} ({fields}) VALUES ({values}) RETURNING {out_fields}",
             table=cls.table_name_sql(),
             fields=sql.list(sql.identifier(x) for x in kwargs.keys()),
             values=sql.list(sql.value(x) for x in kwargs.values()),
             out_fields=sql.list(cls.field_names_sql()),
         )
 
     @classmethod
     async def create(
-        cls: Type[T], connection_or_pool: Union[Connection, Pool], **kwargs: Any
+        cls: type[T], connection_or_pool: Union[Connection, Pool], **kwargs: Any
     ) -> T:
         row = await connection_or_pool.fetchrow(*cls.create_sql(**kwargs))
         return cls(**row)
 
     def insert_sql(self, exclude: FieldNamesSet = ()) -> Fragment:
         cached = self._cached(
             ("insert_sql", tuple(sorted(exclude))),
@@ -371,19 +369,18 @@
         self, connection_or_pool: Union[Connection, Pool], exclude: FieldNamesSet = ()
     ) -> bool:
         query = sql(
             "{} RETURNING xmax",
             self.upsert_sql(self.insert_sql(exclude=exclude), exclude=exclude),
         )
         result = await connection_or_pool.fetchrow(*query)
-        is_update = result["xmax"] != 0
-        return is_update
+        return result["xmax"] != 0
 
     @classmethod
-    def delete_multiple_sql(cls: Type[T], rows: Iterable[T]) -> Fragment:
+    def delete_multiple_sql(cls: type[T], rows: Iterable[T]) -> Fragment:
         cached = cls._cached(
             ("delete_multiple_sql",),
             lambda: sql(
                 "DELETE FROM {table} WHERE ({pks}) IN (SELECT * FROM {unnest})",
                 table=cls.table_name_sql(),
                 pks=sql.list(sql.identifier(pk) for pk in cls.primary_key_names),
             ).compile(),
@@ -393,20 +390,20 @@
                 (row.primary_key() for row in rows),
                 (cls.column_info(pk).type for pk in cls.primary_key_names),
             ),
         )
 
     @classmethod
     async def delete_multiple(
-        cls: Type[T], connection_or_pool: Union[Connection, Pool], rows: Iterable[T]
+        cls: type[T], connection_or_pool: Union[Connection, Pool], rows: Iterable[T]
     ) -> str:
         return await connection_or_pool.execute(*cls.delete_multiple_sql(rows))
 
     @classmethod
-    def insert_multiple_sql(cls: Type[T], rows: Iterable[T]) -> Fragment:
+    def insert_multiple_sql(cls: type[T], rows: Iterable[T]) -> Fragment:
         cached = cls._cached(
             ("insert_multiple_sql",),
             lambda: sql(
                 "INSERT INTO {table} ({fields}) SELECT * FROM {unnest}",
                 table=cls.table_name_sql(),
                 fields=sql.list(cls.field_names_sql()),
             ).compile(),
@@ -415,65 +412,65 @@
             unnest=sql.unnest(
                 (row.field_values() for row in rows),
                 (cls.column_info(name).type for name in cls.field_names()),
             ),
         )
 
     @classmethod
-    def insert_multiple_array_safe_sql(cls: Type[T], rows: Iterable[T]) -> Fragment:
+    def insert_multiple_array_safe_sql(cls: type[T], rows: Iterable[T]) -> Fragment:
         return sql(
             "INSERT INTO {table} ({fields}) VALUES {values}",
             table=cls.table_name_sql(),
             fields=sql.list(cls.field_names_sql()),
             values=sql.list(
                 sql("({})", sql.list(row.field_values_sql(default_none=True)))
                 for row in rows
             ),
         )
 
     @classmethod
     async def insert_multiple_unnest(
-        cls: Type[T], connection_or_pool: Union[Connection, Pool], rows: Iterable[T]
+        cls: type[T], connection_or_pool: Union[Connection, Pool], rows: Iterable[T]
     ) -> str:
         return await connection_or_pool.execute(*cls.insert_multiple_sql(rows))
 
     @classmethod
     async def insert_multiple_array_safe(
-        cls: Type[T], connection_or_pool: Union[Connection, Pool], rows: Iterable[T]
+        cls: type[T], connection_or_pool: Union[Connection, Pool], rows: Iterable[T]
     ) -> str:
         last = ""
         for chunk in chunked(rows, 100):
             last = await connection_or_pool.execute(
                 *cls.insert_multiple_array_safe_sql(chunk)
             )
         return last
 
     @classmethod
     async def insert_multiple(
-        cls: Type[T], connection_or_pool: Union[Connection, Pool], rows: Iterable[T]
+        cls: type[T], connection_or_pool: Union[Connection, Pool], rows: Iterable[T]
     ) -> str:
         if cls.array_safe_insert:
             return await cls.insert_multiple_array_safe(connection_or_pool, rows)
         else:
             return await cls.insert_multiple_unnest(connection_or_pool, rows)
 
     @classmethod
     async def upsert_multiple_unnest(
-        cls: Type[T],
+        cls: type[T],
         connection_or_pool: Union[Connection, Pool],
         rows: Iterable[T],
         insert_only: FieldNamesSet = (),
     ) -> str:
         return await connection_or_pool.execute(
             *cls.upsert_sql(cls.insert_multiple_sql(rows), exclude=insert_only)
         )
 
     @classmethod
     async def upsert_multiple_array_safe(
-        cls: Type[T],
+        cls: type[T],
         connection_or_pool: Union[Connection, Pool],
         rows: Iterable[T],
         insert_only: FieldNamesSet = (),
     ) -> str:
         last = ""
         for chunk in chunked(rows, 100):
             last = await connection_or_pool.execute(
@@ -481,15 +478,15 @@
                     cls.insert_multiple_array_safe_sql(chunk), exclude=insert_only
                 )
             )
         return last
 
     @classmethod
     async def upsert_multiple(
-        cls: Type[T],
+        cls: type[T],
         connection_or_pool: Union[Connection, Pool],
         rows: Iterable[T],
         insert_only: FieldNamesSet = (),
     ) -> str:
         if cls.array_safe_insert:
             return await cls.upsert_multiple_array_safe(
                 connection_or_pool, rows, insert_only=insert_only
@@ -497,35 +494,35 @@
         else:
             return await cls.upsert_multiple_unnest(
                 connection_or_pool, rows, insert_only=insert_only
             )
 
     @classmethod
     def _get_equal_ignoring_fn(
-        cls: Type[T], ignore: FieldNamesSet = ()
+        cls: type[T], ignore: FieldNamesSet = ()
     ) -> Callable[[T, T], bool]:
-        env: Dict[str, Any] = dict()
+        env: dict[str, Any] = {}
         func = ["def equal_ignoring(a, b):"]
         for f in cls._fields():
             if f.name not in ignore:
                 func.append(f" if a.{f.name} != b.{f.name}: return False")
         func += [" return True"]
         exec("\n".join(func), env)
         return env["equal_ignoring"]
 
     @classmethod
     async def replace_multiple(
-        cls: Type[T],
+        cls: type[T],
         connection: Connection,
         rows: Union[Iterable[T], Iterable[Mapping[str, Any]]],
         *,
         where: Where,
         ignore: FieldNamesSet = (),
         insert_only: FieldNamesSet = (),
-    ) -> Tuple[List[T], List[T], List[T]]:
+    ) -> tuple[list[T], list[T], list[T]]:
         ignore = sorted(set(ignore) | set(insert_only))
         equal_ignoring = cls._cached(
             ("equal_ignoring", tuple(ignore)),
             lambda: cls._get_equal_ignoring_fn(ignore),
         )
         pending = {row.primary_key(): row for row in map(cls.ensure_model, rows)}
 
@@ -552,40 +549,38 @@
         if deleted:
             await cls.delete_multiple(connection, deleted)
 
         return created, updated, deleted
 
     @classmethod
     def _get_differences_ignoring_fn(
-        cls: Type[T], ignore: FieldNamesSet = ()
-    ) -> Callable[[T, T], List[str]]:
-        env: Dict[str, Any] = dict()
+        cls: type[T], ignore: FieldNamesSet = ()
+    ) -> Callable[[T, T], list[str]]:
+        env: dict[str, Any] = {}
         func = [
             "def differences_ignoring(a, b):",
             " diffs = []",
         ]
         for f in cls._fields():
             if f.name not in ignore:
-                func.append(
-                    f" if a.{f.name} != b.{f.name}: diffs.append({repr(f.name)})"
-                )
+                func.append(f" if a.{f.name} != b.{f.name}: diffs.append({f.name!r})")
         func += [" return diffs"]
         exec("\n".join(func), env)
         return env["differences_ignoring"]
 
     @classmethod
     async def replace_multiple_reporting_differences(
-        cls: Type[T],
+        cls: type[T],
         connection: Connection,
         rows: Union[Iterable[T], Iterable[Mapping[str, Any]]],
         *,
         where: Where,
         ignore: FieldNamesSet = (),
         insert_only: FieldNamesSet = (),
-    ) -> Tuple[List[T], List[Tuple[T, T, List[str]]], List[T]]:
+    ) -> tuple[list[T], list[tuple[T, T, list[str]]], list[T]]:
         ignore = sorted(set(ignore) | set(insert_only))
         differences_ignoring = cls._cached(
             ("differences_ignoring", tuple(ignore)),
             lambda: cls._get_differences_ignoring_fn(ignore),
         )
 
         pending = {row.primary_key(): row for row in map(cls.ensure_model, rows)}
```

### Comparing `sql_athame-0.4.0a5/sql_athame/escape.py` & `sql_athame-0.4.0a6/sql_athame/escape.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import math
 import uuid
-from typing import Any, Sequence
+from collections.abc import Sequence
+from typing import Any
 
 
 def escape(value: Any) -> str:
     if isinstance(value, str):
-        return f"E{repr(value)}"
+        return f"E{value!r}"
     elif isinstance(value, float) or isinstance(value, int):
         if math.isnan(value):
             raise ValueError("Can't escape NaN float")
         elif math.isinf(value):
             raise ValueError("Can't escape infinite float")
-        return f"{repr(value)}"
+        return f"{value!r}"
     elif isinstance(value, uuid.UUID):
-        return f"{repr(str(value))}::UUID"
+        return f"{str(value)!r}::UUID"
     elif isinstance(value, Sequence):
         args = ", ".join(escape(x) for x in value)
         return f"ARRAY[{args}]"
     elif value is None:
         return "NULL"
     else:
         raise TypeError(f"Can't escape type {type(value)}")
```

### Comparing `sql_athame-0.4.0a5/sql_athame/sqlalchemy.py` & `sql_athame-0.4.0a6/sql_athame/sqlalchemy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from typing import TYPE_CHECKING, Any, Dict, List
+from typing import TYPE_CHECKING, Any
 
 from .types import FlatPart, Placeholder, Slot
 
 try:
     from sqlalchemy.sql import bindparam, text
     from sqlalchemy.sql.elements import BindParameter
 
     def sqlalchemy_text_from_fragment(self: "Fragment") -> Any:
-        parts: List[FlatPart] = []
+        parts: list[FlatPart] = []
         self.flatten_into(parts)
-        bindparams: Dict[str, Any] = {}
-        out_parts: List[str] = []
+        bindparams: dict[str, Any] = {}
+        out_parts: list[str] = []
         for part in parts:
             if isinstance(part, Slot):
                 out_parts.append(f"(:{part.name})")
             elif isinstance(part, Placeholder):
                 key = f"_arg_{part.name}_{id(part)}"
                 if isinstance(part.value, BindParameter):
                     bindparams[key] = bindparam(key, part.value.value, part.value.type)
```

### Comparing `sql_athame-0.4.0a5/PKG-INFO` & `sql_athame-0.4.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-athame
-Version: 0.4.0a5
+Version: 0.4.0a6
 Summary: Python tool for slicing and dicing SQL
 Home-page: https://github.com/bdowning/sql-athame
 License: MIT
 Author: Brian Downing
 Author-email: bdowning@lavos.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

