# Comparing `tmp/chili-2.8.4.tar.gz` & `tmp/chili-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chili-2.8.4.tar", max compression
+gzip compressed data, was "chili-2.9.0.tar", max compression
```

## Comparing `chili-2.8.4.tar` & `chili-2.9.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1085 2023-12-06 12:55:08.896296 chili-2.8.4/LICENSE
--rw-r--r--   0        0        0    21762 2023-12-06 12:55:08.896296 chili-2.8.4/README.md
--rw-r--r--   0        0        0      614 2023-12-06 12:55:08.896296 chili-2.8.4/chili/__init__.py
--rw-r--r--   0        0        0       22 2023-12-06 12:55:08.896296 chili-2.8.4/chili/__version__.py
--rw-r--r--   0        0        0    21716 2023-12-06 12:55:08.900296 chili-2.8.4/chili/decoder.py
--rw-r--r--   0        0        0    18048 2023-12-06 12:55:08.900296 chili-2.8.4/chili/encoder.py
--rw-r--r--   0        0        0      442 2023-12-06 12:55:08.900296 chili-2.8.4/chili/error.py
--rw-r--r--   0        0        0     5740 2023-12-06 12:55:08.900296 chili-2.8.4/chili/iso_datetime.py
--rw-r--r--   0        0        0     1093 2023-12-06 12:55:08.900296 chili-2.8.4/chili/json_support.py
--rw-r--r--   0        0        0     3422 2023-12-06 12:55:08.900296 chili-2.8.4/chili/mapper.py
--rw-r--r--   0        0        0        0 2023-12-06 12:55:08.900296 chili-2.8.4/chili/py.typed
--rw-r--r--   0        0        0     1986 2023-12-06 12:55:08.900296 chili-2.8.4/chili/serializer.py
--rw-r--r--   0        0        0      260 2023-12-06 12:55:08.900296 chili-2.8.4/chili/state.py
--rw-r--r--   0        0        0     7394 2023-12-06 12:55:08.900296 chili-2.8.4/chili/typing.py
--rw-r--r--   0        0        0     2118 2023-12-06 12:55:08.900296 chili-2.8.4/pyproject.toml
--rw-r--r--   0        0        0    23108 1970-01-01 00:00:00.000000 chili-2.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-05-28 05:13:59.240968 chili-2.9.0/LICENSE
+-rw-r--r--   0        0        0    21762 2024-05-28 05:13:59.240968 chili-2.9.0/README.md
+-rw-r--r--   0        0        0      614 2024-05-28 05:13:59.240968 chili-2.9.0/chili/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-28 05:13:59.240968 chili-2.9.0/chili/__version__.py
+-rw-r--r--   0        0        0    21799 2024-05-28 05:13:59.240968 chili-2.9.0/chili/decoder.py
+-rw-r--r--   0        0        0    18109 2024-05-28 05:13:59.240968 chili-2.9.0/chili/encoder.py
+-rw-r--r--   0        0        0      442 2024-05-28 05:13:59.240968 chili-2.9.0/chili/error.py
+-rw-r--r--   0        0        0     5740 2024-05-28 05:13:59.240968 chili-2.9.0/chili/iso_datetime.py
+-rw-r--r--   0        0        0     1093 2024-05-28 05:13:59.244968 chili-2.9.0/chili/json_support.py
+-rw-r--r--   0        0        0     3422 2024-05-28 05:13:59.244968 chili-2.9.0/chili/mapper.py
+-rw-r--r--   0        0        0        0 2024-05-28 05:13:59.244968 chili-2.9.0/chili/py.typed
+-rw-r--r--   0        0        0     1986 2024-05-28 05:13:59.244968 chili-2.9.0/chili/serializer.py
+-rw-r--r--   0        0        0      260 2024-05-28 05:13:59.244968 chili-2.9.0/chili/state.py
+-rw-r--r--   0        0        0     7706 2024-05-28 05:13:59.244968 chili-2.9.0/chili/typing.py
+-rw-r--r--   0        0        0     2118 2024-05-28 05:13:59.244968 chili-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0    23108 1970-01-01 00:00:00.000000 chili-2.9.0/PKG-INFO
```

### Comparing `chili-2.8.4/LICENSE` & `chili-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chili-2.8.4/README.md` & `chili-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `chili-2.8.4/chili/__init__.py` & `chili-2.9.0/chili/__init__.py`

 * *Files identical despite different names*

### Comparing `chili-2.8.4/chili/decoder.py` & `chili-2.9.0/chili/decoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,15 +401,15 @@
         super().__init__(type_)
 
     def _build_type_decoder(self, a_type: Type) -> TypeDecoder:
         return build_type_decoder(
             map_generic_type(a_type, self._generic_parameters),
             self._extra_decoders,
             self._generic_type.__module__,
-            self.force
+            self.force,
         )
 
 
 class EnumDecoder(TypeDecoder, Generic[E]):
     def __init__(self, class_name: Type):
         self.class_name = class_name
 
@@ -440,24 +440,28 @@
             decoded_values.append(item)
 
         return tuple(decoded_values)
 
     def _build(self) -> None:
         field_types = self.class_name.__annotations__
         for item_type in field_types.values():
-            self._arg_decoders.append(build_type_decoder(item_type, self._extra_decoders, self.class_name.__module__, self.force))
+            self._arg_decoders.append(
+                build_type_decoder(item_type, self._extra_decoders, self.class_name.__module__, self.force)
+            )
 
 
 class TypedDictDecoder(TypeDecoder):
     def __init__(self, class_name: Type, extra_decoders: TypeDecoders = None, force: bool = False):
         self.class_name = class_name
         self._key_decoders = {}
         self._extra_decoders = extra_decoders
         for key_name, key_type in class_name.__annotations__.items():
-            self._key_decoders[key_name] = build_type_decoder(key_type, self._extra_decoders, class_name.__module__, force)
+            self._key_decoders[key_name] = build_type_decoder(
+                key_type, self._extra_decoders, class_name.__module__, force
+            )
 
     def decode(self, value: dict) -> dict:
         return {key: self._key_decoders[key].decode(item) for key, item in value.items()}
 
 
 class OptionalTypeDecoder(TypeDecoder):
     def __init__(self, type_decoder: TypeDecoder):
@@ -542,15 +546,17 @@
     if get_origin(origin_type) is not None:
         raise DecoderError.invalid_type(a_type)
 
     if hasattr(origin_type, _PROPERTIES):
         return Decoder[origin_type](decoders=extra_decoders)  # type: ignore
 
     if is_optional(a_type):
-        return OptionalTypeDecoder(build_type_decoder(unpack_optional(a_type), extra_decoders, module, force))  # type: ignore
+        return OptionalTypeDecoder(
+            build_type_decoder(unpack_optional(a_type), extra_decoders, module, force)  # type: ignore
+        )
 
     if origin_type not in _supported_generics:
         if force and is_class(origin_type):
             return Decoder[origin_type](extra_decoders)  # type: ignore
         raise DecoderError.invalid_type(a_type)
 
     type_attributes: List[Union[TypeDecoder, Any]] = [
```

### Comparing `chili-2.8.4/chili/encoder.py` & `chili-2.9.0/chili/encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,15 +277,15 @@
         super().__init__(type_)
 
     def _build_type_encoder(self, a_type: Type) -> TypeEncoder:
         return build_type_encoder(
             map_generic_type(a_type, self._generic_parameters),
             self._extra_encoders,
             self._generic_type.__module__,
-            self.force
+            self.force,
         )
 
 
 class EnumEncoder(TypeEncoder, Generic[E]):
     def __init__(self, enum_type: Type):
         self.enum_type = enum_type
 
@@ -314,24 +314,28 @@
             self._arg_encoders[index].encode(item) if index < len(self._arg_encoders) else item
             for index, item in enumerate(value)
         ]
 
     def _build(self) -> None:
         field_types = self.type.__annotations__
         for item_type in field_types.values():
-            self._arg_encoders.append(build_type_encoder(item_type, self._extra_encoders, self.type.__module__, self.force))
+            self._arg_encoders.append(
+                build_type_encoder(item_type, self._extra_encoders, self.type.__module__, self.force)
+            )
 
 
 class TypedDictEncoder(TypeEncoder):
     def __init__(self, class_name: Type, extra_encoders: TypeEncoders = None, force: bool = False):
         self.type = class_name
         self._key_encoders = {}
         self.force = force
         for key_name, key_type in class_name.__annotations__.items():
-            self._key_encoders[key_name] = build_type_encoder(key_type, extra_encoders, class_name.__module__, self.force)
+            self._key_encoders[key_name] = build_type_encoder(
+                key_type, extra_encoders, class_name.__module__, self.force
+            )
 
     def encode(self, value: dict) -> dict:
         return {key: self._key_encoders[key].encode(item) for key, item in value.items()}
 
 
 class OptionalTypeEncoder(TypeEncoder):
     def __init__(self, type_encoder: TypeEncoder):
```

### Comparing `chili-2.8.4/chili/iso_datetime.py` & `chili-2.9.0/chili/iso_datetime.py`

 * *Files identical despite different names*

### Comparing `chili-2.8.4/chili/json_support.py` & `chili-2.9.0/chili/json_support.py`

 * *Files identical despite different names*

### Comparing `chili-2.8.4/chili/mapper.py` & `chili-2.9.0/chili/mapper.py`

 * *Files identical despite different names*

### Comparing `chili-2.8.4/chili/serializer.py` & `chili-2.9.0/chili/serializer.py`

 * *Files identical despite different names*

### Comparing `chili-2.8.4/chili/typing.py` & `chili-2.9.0/chili/typing.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,23 @@
 from enum import Enum
 from functools import lru_cache
 from inspect import isclass as is_class
 from typing import Any, Callable, ClassVar, Dict, List, NewType, Optional, Type, Union, get_type_hints
 
 from chili.error import SerialisationError
 
+try:
+    from types import UnionType  # type: ignore
+
+    _SUPPORT_NEW_UNION = True
+except ImportError:
+    _SUPPORT_NEW_UNION = False
+    UnionType = object()
+
+
 AnnotatedTypeNames = {"AnnotatedMeta", "_AnnotatedAlias"}
 _GenericAlias = getattr(typing, "_GenericAlias")
 _PROPERTIES = "__typed_properties__"
 _DECODE_MAPPER = "__decode_mapper__"
 _ENCODE_MAPPER = "__encode_mapper__"
 _ENCODABLE = "__encodable__"
 _DECODABLE = "__decodable__"
@@ -70,16 +79,19 @@
 
 
 def is_serialisable(type_name: Type) -> bool:
     return is_class(type_name) and hasattr(type_name, _DECODABLE) and hasattr(type_name, _ENCODABLE)
 
 
 def is_optional(type_name: Type) -> bool:
+    is_new_union = False
+    if _SUPPORT_NEW_UNION:
+        is_new_union = type(type_name) is UnionType
     return (
-        get_origin_type(type_name) is Union
+        (get_origin_type(type_name) is Union or type(type_name) is Union or is_new_union)
         and bool(get_type_args(type_name))
         and get_type_args(type_name)[-1] is type(None)  # noqa
     )
 
 
 def is_newtype(type_name: Type) -> bool:
     if sys.version_info >= (3, 10):
```

### Comparing `chili-2.8.4/pyproject.toml` & `chili-2.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 documentation = "https://github.com/kodemore/chili"
 homepage = "https://github.com/kodemore/chili"
 keywords = ["class", "decode", "deserialise", "encode", "object", "serialise"]
 license = "MIT"
 name = "chili"
 readme = "README.md"
 repository = "https://github.com/kodemore/chili"
-version = "2.8.4"
+version = "2.9.0"
 
 [tool.poetry.dependencies]
 gaffe = ">=0.3.0"
 python = "^3.8"
 typing-extensions = "^4.2"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `chili-2.8.4/PKG-INFO` & `chili-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chili
-Version: 2.8.4
+Version: 2.9.0
 Summary: Chili is serialisation library. It can serialise/deserialise almost any object.
 Home-page: https://github.com/kodemore/chili
 License: MIT
 Keywords: class,decode,deserialise,encode,object,serialise
 Author: Dawid Kraczkowski
 Author-email: dawid.kraczkowski@gmail.com
 Requires-Python: >=3.8,<4.0
```

