# Comparing `tmp/py_grpcio-1.5.3.tar.gz` & `tmp/py_grpcio-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_grpcio-1.5.3.tar", max compression
+gzip compressed data, was "py_grpcio-1.5.4.tar", max compression
```

## Comparing `py_grpcio-1.5.3.tar` & `py_grpcio-1.5.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1076 2024-05-24 22:10:26.230874 py_grpcio-1.5.3/LICENSE
--rw-r--r--   0        0        0     4581 2024-05-24 22:10:26.230874 py_grpcio-1.5.3/README.md
--rw-r--r--   0        0        0      307 2024-05-24 22:10:26.234874 py_grpcio-1.5.3/py_grpcio/__init__.py
--rw-r--r--   0        0        0       60 2024-05-24 22:10:26.234874 py_grpcio-1.5.3/py_grpcio/__meta__.py
--rw-r--r--   0        0        0      796 2024-05-24 22:10:26.234874 py_grpcio-1.5.3/py_grpcio/exceptions.py
--rw-r--r--   0        0        0     1961 2024-05-24 22:10:26.234874 py_grpcio-1.5.3/py_grpcio/interceptor.py
--rw-r--r--   0        0        0     5670 2024-05-24 22:10:26.234874 py_grpcio-1.5.3/py_grpcio/method.py
--rw-r--r--   0        0        0     1148 2024-05-24 22:10:26.234874 py_grpcio-1.5.3/py_grpcio/middleware.py
--rw-r--r--   0        0        0     5588 2024-05-24 22:10:26.234874 py_grpcio-1.5.3/py_grpcio/models.py
--rw-r--r--   0        0        0      114 2024-05-24 22:10:26.234874 py_grpcio-1.5.3/py_grpcio/proto/__init__.py
--rw-r--r--   0        0        0      483 2024-05-24 22:10:26.234874 py_grpcio-1.5.3/py_grpcio/proto/enums.py
--rw-r--r--   0        0        0     3882 2024-05-24 22:10:26.234874 py_grpcio-1.5.3/py_grpcio/proto/parser.py
--rw-r--r--   0        0        0      686 2024-05-24 22:10:26.234874 py_grpcio-1.5.3/py_grpcio/proto/templates/service.proto.template
--rw-r--r--   0        0        0     2798 2024-05-24 22:10:26.234874 py_grpcio-1.5.3/py_grpcio/server.py
--rw-r--r--   0        0        0      924 2024-05-24 22:10:26.234874 py_grpcio-1.5.3/py_grpcio/service.py
--rw-r--r--   0        0        0     2727 2024-05-24 22:10:26.234874 py_grpcio-1.5.3/py_grpcio/service_meta.py
--rw-r--r--   0        0        0      582 2024-05-24 22:10:26.234874 py_grpcio-1.5.3/py_grpcio/utils.py
--rw-r--r--   0        0        0      573 2024-05-24 22:10:26.234874 py_grpcio-1.5.3/pyproject.toml
--rw-r--r--   0        0        0     5322 1970-01-01 00:00:00.000000 py_grpcio-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-27 22:48:45.660909 py_grpcio-1.5.4/LICENSE
+-rw-r--r--   0        0        0     4581 2024-05-27 22:48:45.660909 py_grpcio-1.5.4/README.md
+-rw-r--r--   0        0        0      307 2024-05-27 22:48:45.664909 py_grpcio-1.5.4/py_grpcio/__init__.py
+-rw-r--r--   0        0        0       60 2024-05-27 22:48:45.664909 py_grpcio-1.5.4/py_grpcio/__meta__.py
+-rw-r--r--   0        0        0      796 2024-05-27 22:48:45.664909 py_grpcio-1.5.4/py_grpcio/exceptions.py
+-rw-r--r--   0        0        0     1961 2024-05-27 22:48:45.664909 py_grpcio-1.5.4/py_grpcio/interceptor.py
+-rw-r--r--   0        0        0     5859 2024-05-27 22:48:45.664909 py_grpcio-1.5.4/py_grpcio/method.py
+-rw-r--r--   0        0        0     1148 2024-05-27 22:48:45.664909 py_grpcio-1.5.4/py_grpcio/middleware.py
+-rw-r--r--   0        0        0     5588 2024-05-27 22:48:45.664909 py_grpcio-1.5.4/py_grpcio/models.py
+-rw-r--r--   0        0        0      114 2024-05-27 22:48:45.664909 py_grpcio-1.5.4/py_grpcio/proto/__init__.py
+-rw-r--r--   0        0        0      483 2024-05-27 22:48:45.664909 py_grpcio-1.5.4/py_grpcio/proto/enums.py
+-rw-r--r--   0        0        0     3958 2024-05-27 22:48:45.664909 py_grpcio-1.5.4/py_grpcio/proto/parser.py
+-rw-r--r--   0        0        0      686 2024-05-27 22:48:45.664909 py_grpcio-1.5.4/py_grpcio/proto/templates/service.proto.template
+-rw-r--r--   0        0        0     2798 2024-05-27 22:48:45.664909 py_grpcio-1.5.4/py_grpcio/server.py
+-rw-r--r--   0        0        0     1214 2024-05-27 22:48:45.664909 py_grpcio-1.5.4/py_grpcio/service.py
+-rw-r--r--   0        0        0     2727 2024-05-27 22:48:45.664909 py_grpcio-1.5.4/py_grpcio/service_meta.py
+-rw-r--r--   0        0        0      582 2024-05-27 22:48:45.664909 py_grpcio-1.5.4/py_grpcio/utils.py
+-rw-r--r--   0        0        0      573 2024-05-27 22:48:45.664909 py_grpcio-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0     5322 1970-01-01 00:00:00.000000 py_grpcio-1.5.4/PKG-INFO
```

### Comparing `py_grpcio-1.5.3/LICENSE` & `py_grpcio-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.5.3/README.md` & `py_grpcio-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.5.3/py_grpcio/exceptions.py` & `py_grpcio-1.5.4/py_grpcio/exceptions.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.5.3/py_grpcio/interceptor.py` & `py_grpcio-1.5.4/py_grpcio/interceptor.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.5.3/py_grpcio/method.py` & `py_grpcio-1.5.4/py_grpcio/method.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from py_grpcio.models import Target, Method, Message
 from py_grpcio.exceptions import SendEmpty, RunTimeServerError
 
 from py_grpcio.middleware import BaseMiddleware
 
 from py_grpcio.proto.enums import ProtoBufTypes
 
+type Delay = float
 type Service = type
 type MethodType = Callable[[ProtoMessage, str, bool], ProtoMessage]
 
 
 class MethodGRPC:
     def __init__(self: 'MethodGRPC', method: Method):
         self.method: Method = method
@@ -105,20 +106,28 @@
                 raise SendEmpty(text='Method did not return anything')
             return self.pydantic_to_proto(message=response, model=self.method.proto_response, method=self.method)
         except ValidationError as exc:
             raise RunTimeServerError(details={'validation_error': exc.json()})
 
 
 class ClientMethodGRPC(MethodGRPC):
-    def __init__(self: 'ClientMethodGRPC', method: Method, service_name: str, host: str, port: int = 50051):
+    def __init__(
+        self: 'ClientMethodGRPC',
+        method: Method,
+        service_name: str,
+        host: str,
+        port: int = 50051,
+        timeout_delay: Delay = 1
+    ):
         super().__init__(method=method)
         self.method: Method = method
         self.service_name: str = service_name
         self.host: str = host
         self.port: int = port
+        self.timeout_delay: Delay = timeout_delay
 
     @property
     def service(self: 'ClientMethodGRPC') -> Service:
         return getattr(self.method.services, f'{self.service_name}')
 
     @classmethod
     async def call_grpc_method(cls: Type['ClientMethodGRPC'], method: MethodType, **kwargs) -> ProtoMessage:
@@ -132,10 +141,11 @@
             method=self.method
         )
         method: Callable = getattr(self.service, snake_to_camel(self.method.target.func.__name__))
         proto_response: ProtoMessage = await self.call_grpc_method(
             method=method,
             request=proto_request,
             target=f'{self.host}:{self.port}',
-            insecure=True
+            insecure=True,
+            timeout=self.timeout_delay
         )
         return self.proto_to_pydantic(message=proto_response, model=self.method.response, method=self.method)
```

### Comparing `py_grpcio-1.5.3/py_grpcio/middleware.py` & `py_grpcio-1.5.4/py_grpcio/middleware.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.5.3/py_grpcio/models.py` & `py_grpcio-1.5.4/py_grpcio/models.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.5.3/py_grpcio/proto/parser.py` & `py_grpcio-1.5.4/py_grpcio/proto/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from uuid import UUID
 from enum import Enum
 from inspect import isclass
-from datetime import datetime
+from datetime import date, time, datetime
 
 from pydantic import BaseModel
 
 from types import UnionType, NoneType, GenericAlias
 from typing import Any, Annotated, Union, Iterable, get_origin
 
 from py_grpcio.proto import ProtoBufTypes
@@ -15,14 +15,16 @@
     float: ProtoBufTypes.DOUBLE,
     bool: ProtoBufTypes.BOOL,
     str: ProtoBufTypes.STRING,
     bytes: ProtoBufTypes.BYTES,
     dict: ProtoBufTypes.MAP,
 
     UUID: ProtoBufTypes.STRING,
+    date: ProtoBufTypes.STRING,
+    time: ProtoBufTypes.STRING,
     datetime: ProtoBufTypes.STRING,
 }
 
 
 def parse_type(field_name: str, python_value: Any, field_type: type, allow_model: bool = True) -> ProtoBufTypes | str:
     if python_value in TYPE_MAPPING:
         return TYPE_MAPPING[python_value]
```

### Comparing `py_grpcio-1.5.3/py_grpcio/proto/templates/service.proto.template` & `py_grpcio-1.5.4/py_grpcio/proto/templates/service.proto.template`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.5.3/py_grpcio/server.py` & `py_grpcio-1.5.4/py_grpcio/server.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.5.3/py_grpcio/service.py` & `py_grpcio-1.5.4/py_grpcio/service.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,36 @@
 from typing import Any
 from pathlib import Path
 
 from py_grpcio.models import Method
 from py_grpcio.method import ClientMethodGRPC
 from py_grpcio.service_meta import BaseServiceMeta
 
+type Delay = float
+
 
 class BaseService(metaclass=BaseServiceMeta):
-    def __init__(self: 'BaseService', host='localhost', port: int = 50051, proto_dir: Path = Path('proto')):
+    def __init__(
+            self: 'BaseService',
+            host='localhost',
+            port: int = 50051,
+            proto_dir: Path = Path('proto'),
+            timeout_delay: Delay = 1
+    ):
         self.host: str = host
         self.port: int = port
         self.proto_dir: Path = proto_dir
         self.proto_dir.mkdir(exist_ok=True)
+        self.timeout_delay: Delay = timeout_delay
         self.__class__.init_protos_and_services(proto_dir=self.proto_dir)
 
     def __getattribute__(self: 'BaseService', attr_name: str) -> ClientMethodGRPC | Any:
         methods: dict[str, Method] = super().__getattribute__('methods')
         if method := methods.get(attr_name):
-            return ClientMethodGRPC(method=method, service_name=self.name, host=self.host, port=self.port)
+            return ClientMethodGRPC(
+                method=method,
+                service_name=self.name,
+                host=self.host,
+                port=self.port,
+                timeout_delay=self.timeout_delay
+            )
         return super().__getattribute__(attr_name)
```

### Comparing `py_grpcio-1.5.3/py_grpcio/service_meta.py` & `py_grpcio-1.5.4/py_grpcio/service_meta.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.5.3/py_grpcio/utils.py` & `py_grpcio-1.5.4/py_grpcio/utils.py`

 * *Files identical despite different names*

### Comparing `py_grpcio-1.5.3/pyproject.toml` & `py_grpcio-1.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-grpcio"
-version = "1.5.3"
+version = "1.5.4"
 description = "gRPC with autogen by Pydantic models"
 authors = ["Yurii <ykolibroda@lytvynov-production.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
   { include = "py_grpcio" },
 ]
```

### Comparing `py_grpcio-1.5.3/PKG-INFO` & `py_grpcio-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-grpcio
-Version: 1.5.3
+Version: 1.5.4
 Summary: gRPC with autogen by Pydantic models
 License: MIT
 Author: Yurii
 Author-email: ykolibroda@lytvynov-production.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

