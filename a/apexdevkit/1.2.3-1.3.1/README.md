# Comparing `tmp/apexdevkit-1.2.3.tar.gz` & `tmp/apexdevkit-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apexdevkit-1.2.3.tar", max compression
+gzip compressed data, was "apexdevkit-1.3.1.tar", max compression
```

## Comparing `apexdevkit-1.2.3.tar` & `apexdevkit-1.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    35149 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/LICENSE
--rw-r--r--   0        0        0       12 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/README.md
--rw-r--r--   0        0        0        0 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/__init__.py
--rw-r--r--   0        0        0       81 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/annotation/__init__.py
--rw-r--r--   0        0        0     1475 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/annotation/deprecate.py
--rw-r--r--   0        0        0      903 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/error.py
--rw-r--r--   0        0        0      597 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/fastapi/__init__.py
--rw-r--r--   0        0        0      970 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/fastapi/builder.py
--rw-r--r--   0        0        0      255 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/fastapi/dependable.py
--rw-r--r--   0        0        0      233 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/fastapi/docs.py
--rw-r--r--   0        0        0     1699 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/fastapi/response.py
--rw-r--r--   0        0        0     7745 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/fastapi/router.py
--rw-r--r--   0        0        0     3603 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/fastapi/schema.py
--rw-r--r--   0        0        0     2616 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/fastapi/service.py
--rw-r--r--   0        0        0      398 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/http/__init__.py
--rw-r--r--   0        0        0     2022 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/http/fake.py
--rw-r--r--   0        0        0     3060 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/http/fluent.py
--rw-r--r--   0        0        0     2763 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/http/httpx.py
--rw-r--r--   0        0        0     1026 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/http/json.py
--rw-r--r--   0        0        0      201 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/http/url.py
--rw-r--r--   0        0        0        0 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/py.typed
--rw-r--r--   0        0        0      334 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/repository/__init__.py
--rw-r--r--   0        0        0      772 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/repository/connector.py
--rw-r--r--   0        0        0     2362 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/repository/database.py
--rw-r--r--   0        0        0     3388 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/repository/in_memory.py
--rw-r--r--   0        0        0      653 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/repository/interface.py
--rw-r--r--   0        0        0      238 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/testing/__init__.py
--rw-r--r--   0        0        0     1305 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/testing/database.py
--rw-r--r--   0        0        0     7774 2024-05-27 16:08:48.780302 apexdevkit-1.2.3/apexdevkit/testing/rest.py
--rw-r--r--   0        0        0      992 2024-05-27 16:09:03.192213 apexdevkit-1.2.3/pyproject.toml
--rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 apexdevkit-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-28 14:01:14.698180 apexdevkit-1.3.1/LICENSE
+-rw-r--r--   0        0        0       12 2024-05-28 14:01:14.698180 apexdevkit-1.3.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 14:01:14.698180 apexdevkit-1.3.1/apexdevkit/__init__.py
+-rw-r--r--   0        0        0       81 2024-05-28 14:01:14.698180 apexdevkit-1.3.1/apexdevkit/annotation/__init__.py
+-rw-r--r--   0        0        0     1475 2024-05-28 14:01:14.698180 apexdevkit-1.3.1/apexdevkit/annotation/deprecate.py
+-rw-r--r--   0        0        0      903 2024-05-28 14:01:14.698180 apexdevkit-1.3.1/apexdevkit/error.py
+-rw-r--r--   0        0        0      597 2024-05-28 14:01:14.698180 apexdevkit-1.3.1/apexdevkit/fastapi/__init__.py
+-rw-r--r--   0        0        0      970 2024-05-28 14:01:14.698180 apexdevkit-1.3.1/apexdevkit/fastapi/builder.py
+-rw-r--r--   0        0        0      255 2024-05-28 14:01:14.698180 apexdevkit-1.3.1/apexdevkit/fastapi/dependable.py
+-rw-r--r--   0        0        0      233 2024-05-28 14:01:14.698180 apexdevkit-1.3.1/apexdevkit/fastapi/docs.py
+-rw-r--r--   0        0        0     1699 2024-05-28 14:01:14.698180 apexdevkit-1.3.1/apexdevkit/fastapi/response.py
+-rw-r--r--   0        0        0     7667 2024-05-28 14:01:14.698180 apexdevkit-1.3.1/apexdevkit/fastapi/router.py
+-rw-r--r--   0        0        0     3909 2024-05-28 14:01:14.698180 apexdevkit-1.3.1/apexdevkit/fastapi/schema.py
+-rw-r--r--   0        0        0     2616 2024-05-28 14:01:14.698180 apexdevkit-1.3.1/apexdevkit/fastapi/service.py
+-rw-r--r--   0        0        0      398 2024-05-28 14:01:14.698180 apexdevkit-1.3.1/apexdevkit/http/__init__.py
+-rw-r--r--   0        0        0     2022 2024-05-28 14:01:14.698180 apexdevkit-1.3.1/apexdevkit/http/fake.py
+-rw-r--r--   0        0        0     3060 2024-05-28 14:01:14.698180 apexdevkit-1.3.1/apexdevkit/http/fluent.py
+-rw-r--r--   0        0        0     2763 2024-05-28 14:01:14.702180 apexdevkit-1.3.1/apexdevkit/http/httpx.py
+-rw-r--r--   0        0        0     1026 2024-05-28 14:01:14.702180 apexdevkit-1.3.1/apexdevkit/http/json.py
+-rw-r--r--   0        0        0      201 2024-05-28 14:01:14.702180 apexdevkit-1.3.1/apexdevkit/http/url.py
+-rw-r--r--   0        0        0        0 2024-05-28 14:01:14.702180 apexdevkit-1.3.1/apexdevkit/py.typed
+-rw-r--r--   0        0        0      334 2024-05-28 14:01:14.702180 apexdevkit-1.3.1/apexdevkit/repository/__init__.py
+-rw-r--r--   0        0        0      772 2024-05-28 14:01:14.702180 apexdevkit-1.3.1/apexdevkit/repository/connector.py
+-rw-r--r--   0        0        0     2362 2024-05-28 14:01:14.702180 apexdevkit-1.3.1/apexdevkit/repository/database.py
+-rw-r--r--   0        0        0     3388 2024-05-28 14:01:14.702180 apexdevkit-1.3.1/apexdevkit/repository/in_memory.py
+-rw-r--r--   0        0        0      653 2024-05-28 14:01:14.702180 apexdevkit-1.3.1/apexdevkit/repository/interface.py
+-rw-r--r--   0        0        0      238 2024-05-28 14:01:14.702180 apexdevkit-1.3.1/apexdevkit/testing/__init__.py
+-rw-r--r--   0        0        0     1305 2024-05-28 14:01:14.702180 apexdevkit-1.3.1/apexdevkit/testing/database.py
+-rw-r--r--   0        0        0     7774 2024-05-28 14:01:14.702180 apexdevkit-1.3.1/apexdevkit/testing/rest.py
+-rw-r--r--   0        0        0      992 2024-05-28 14:01:26.974208 apexdevkit-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 apexdevkit-1.3.1/PKG-INFO
```

### Comparing `apexdevkit-1.2.3/LICENSE` & `apexdevkit-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.3/apexdevkit/annotation/deprecate.py` & `apexdevkit-1.3.1/apexdevkit/annotation/deprecate.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.3/apexdevkit/error.py` & `apexdevkit-1.3.1/apexdevkit/error.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.3/apexdevkit/fastapi/__init__.py` & `apexdevkit-1.3.1/apexdevkit/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.3/apexdevkit/fastapi/builder.py` & `apexdevkit-1.3.1/apexdevkit/fastapi/builder.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.3/apexdevkit/fastapi/response.py` & `apexdevkit-1.3.1/apexdevkit/fastapi/response.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.3/apexdevkit/fastapi/router.py` & `apexdevkit-1.3.1/apexdevkit/fastapi/router.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 from dataclasses import dataclass, field
+from functools import cached_property
 from typing import Annotated, Any, Iterable, Self, TypeVar
 
 from fastapi import APIRouter, Depends
 from fastapi.responses import JSONResponse
 
 from apexdevkit.error import DoesNotExistError, ExistsError
-from apexdevkit.fastapi.schema import RestfulSchema
+from apexdevkit.fastapi.schema import DataclassFields, RestfulSchema, SchemaFields
 from apexdevkit.fastapi.service import RawCollection, RawItem, RestfulService
 from apexdevkit.testing import RestfulName
 
 _Response = JSONResponse | dict[str, Any]
 
 
 @dataclass
 class RestfulResponse:
     name: RestfulName
 
-    @classmethod
-    def from_dataclass(cls, value: type[Any]) -> "RestfulResponse":
-        return cls(name=RestfulName(value.__name__.lower()))
-
     def _response(self, code: int, data: Any, error: str = "") -> dict[str, Any]:
         content: dict[str, Any] = {"code": code, "status": "success"}
 
         if error:
             content["status"] = "fail"
             content["error"] = {"message": error}
 
@@ -72,40 +69,41 @@
 
 
 T = TypeVar("T")
 
 
 @dataclass
 class RestfulRouter:
-    schema: RestfulSchema = field(init=False)
-    response: RestfulResponse = field(init=False)
-    service: RestfulService = field(init=False)
-
-    router: APIRouter = field(init=False, default_factory=APIRouter)
-
-    @classmethod
-    def from_dataclass(cls, value: Any) -> "RestfulRouter":
-        return (
-            cls()
-            .with_schema(RestfulSchema.from_dataclass(value))
-            .with_response(RestfulResponse.from_dataclass(value))
-        )
+    service: RestfulService
 
-    def with_schema(self, value: RestfulSchema) -> Self:
-        self.schema = value
+    router: APIRouter = field(default_factory=APIRouter)
 
-        return self
+    name: RestfulName = field(init=False)
+    fields: SchemaFields = field(init=False)
+
+    @cached_property
+    def response(self) -> RestfulResponse:
+        return RestfulResponse(name=self.name)
+
+    @cached_property
+    def schema(self) -> RestfulSchema:
+        return RestfulSchema(name=self.name, fields=self.fields)
+
+    def with_dataclass(self, value: Any) -> Self:
+        return self.with_name(RestfulName(value.__name__.lower())).with_fields(
+            DataclassFields(value)
+        )
 
-    def with_response(self, value: RestfulResponse) -> Self:
-        self.response = value
+    def with_name(self, value: RestfulName) -> Self:
+        self.name = value
 
         return self
 
-    def with_service(self, value: RestfulService) -> Self:
-        self.service = value
+    def with_fields(self, value: SchemaFields) -> Self:
+        self.fields = value
 
         return self
 
     def with_create_one_endpoint(self, is_documented: bool = True) -> Self:
         schema = self.schema.for_create_one()
 
         @self.router.post(
```

### Comparing `apexdevkit-1.2.3/apexdevkit/fastapi/schema.py` & `apexdevkit-1.3.1/apexdevkit/fastapi/schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,47 @@
-from dataclasses import dataclass, field
+from abc import ABC, abstractmethod
+from dataclasses import dataclass
+from functools import cached_property
 from typing import Any, Callable, Iterable, List
 
 from pydantic import BaseModel, create_model
 
 from apexdevkit.http import JsonDict
 from apexdevkit.testing import RestfulName
 
 
+class SchemaFields(ABC):
+    def writable(self) -> JsonDict:
+        return self.editable()
+
+    def editable(self) -> JsonDict:
+        return self.readable().drop("id")
+
+    @abstractmethod
+    def readable(self) -> JsonDict:
+        pass
+
+
+@dataclass
+class DataclassFields(SchemaFields):
+    source: Any
+
+    def readable(self) -> JsonDict:
+        return JsonDict(self.source.__annotations__)
+
+
 @dataclass
 class RestfulSchema:
     name: RestfulName
-    fields: JsonDict
-
-    schemas: dict[str, type[BaseModel]] = field(default_factory=dict)
+    fields: SchemaFields
 
     def __post_init__(self) -> None:
-        schema = self._schema_for("", self.fields)
-        create_schema = self._schema_for("Create", self.fields.drop("id"))
-        self._schema_for("Update", self.fields.drop("id"))
+        schema = self._schema_for("", self.fields.readable())
+        create_schema = self._schema_for("Create", self.fields.writable())
+        self._schema_for("Update", self.fields.editable())
 
         self._schema_for(
             "Item",
             JsonDict({self.name.singular: schema}),
         )
         self._schema_for(
             "Collection",
@@ -33,20 +53,29 @@
             JsonDict({self.name.plural: List[create_schema]}),
         )
         self._schema_for(
             "UpdateMany",
             JsonDict({self.name.plural: List[schema]}),
         )
 
-    @classmethod
-    def from_dataclass(cls, value: Any) -> "RestfulSchema":
-        return cls(
-            name=RestfulName(value.__name__.lower()),
-            fields=JsonDict(value.__annotations__),
-        )
+    def _schema_for(self, action: str, fields: dict[str, Any]) -> type[BaseModel]:
+        if action not in self.schemas:
+            self.schemas[action] = create_model(
+                self.name.singular.capitalize() + action,
+                **{
+                    field_name: (field_type, ...)
+                    for field_name, field_type in fields.items()
+                },
+            )
+
+        return self.schemas[action]
+
+    @cached_property
+    def schemas(self) -> dict[str, type[BaseModel]]:
+        return {}
 
     def for_no_data(self) -> type[BaseModel]:
         class NoData(BaseModel):
             pass
 
         return self._schema_for(
             "NoDataResponse",
@@ -98,19 +127,7 @@
     def for_update_many(self) -> Callable[[BaseModel], Iterable[dict[str, Any]]]:
         schema = self.schemas["UpdateMany"]
 
         def _(request: schema) -> Iterable[dict[str, Any]]:
             return [dict(item) for item in request.model_dump()[self.name.plural]]
 
         return _
-
-    def _schema_for(self, action: str, fields: dict[str, Any]) -> type[BaseModel]:
-        if action not in self.schemas:
-            self.schemas[action] = create_model(
-                self.name.singular.capitalize() + action,
-                **{
-                    field_name: (field_type, ...)
-                    for field_name, field_type in fields.items()
-                },
-            )
-
-        return self.schemas[action]
```

### Comparing `apexdevkit-1.2.3/apexdevkit/fastapi/service.py` & `apexdevkit-1.3.1/apexdevkit/fastapi/service.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.3/apexdevkit/http/fake.py` & `apexdevkit-1.3.1/apexdevkit/http/fake.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.3/apexdevkit/http/fluent.py` & `apexdevkit-1.3.1/apexdevkit/http/fluent.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.3/apexdevkit/http/httpx.py` & `apexdevkit-1.3.1/apexdevkit/http/httpx.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.3/apexdevkit/http/json.py` & `apexdevkit-1.3.1/apexdevkit/http/json.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.3/apexdevkit/repository/connector.py` & `apexdevkit-1.3.1/apexdevkit/repository/connector.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.3/apexdevkit/repository/database.py` & `apexdevkit-1.3.1/apexdevkit/repository/database.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.3/apexdevkit/repository/in_memory.py` & `apexdevkit-1.3.1/apexdevkit/repository/in_memory.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.3/apexdevkit/repository/interface.py` & `apexdevkit-1.3.1/apexdevkit/repository/interface.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.3/apexdevkit/testing/database.py` & `apexdevkit-1.3.1/apexdevkit/testing/database.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.3/apexdevkit/testing/rest.py` & `apexdevkit-1.3.1/apexdevkit/testing/rest.py`

 * *Files identical despite different names*

### Comparing `apexdevkit-1.2.3/pyproject.toml` & `apexdevkit-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apexdevkit"
-version = "1.2.3"
+version = "1.3.1"
 description = "Apex Development Tools for python."
 authors = ["Apex Dev <dev@apex.ge>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 httpx = "*"
```

