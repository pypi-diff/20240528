# Comparing `tmp/temper_core-0.2.1.tar.gz` & `tmp/temper_core-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temper_core-0.2.1.tar", max compression
+gzip compressed data, was "temper_core-0.3.0.tar", max compression
```

## Comparing `temper_core-0.2.1.tar` & `temper_core-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0      428 2024-04-23 22:22:25.555323 temper_core-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    36160 2024-04-23 22:22:25.585323 temper_core-0.2.1/temper_core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 22:22:25.555323 temper_core-0.2.1/temper_core/py.typed
--rw-r--r--   0        0        0     1555 2024-04-23 22:22:25.585323 temper_core-0.2.1/temper_core/regex.py
--rw-r--r--   0        0        0     3552 2024-04-23 22:22:25.585323 temper_core-0.2.1/temper_core/testing.py
--rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 temper_core-0.2.1/setup.py
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 temper_core-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      428 2024-05-28 15:06:57.427438 temper_core-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    39283 2024-05-28 15:06:57.437438 temper_core-0.3.0/temper_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 15:06:57.427438 temper_core-0.3.0/temper_core/py.typed
+-rw-r--r--   0        0        0     1519 2024-05-28 15:06:57.437438 temper_core-0.3.0/temper_core/regex.py
+-rw-r--r--   0        0        0     3552 2024-05-28 15:06:57.437438 temper_core-0.3.0/temper_core/testing.py
+-rw-r--r--   0        0        0      546 1970-01-01 00:00:00.000000 temper_core-0.3.0/PKG-INFO
```

### Comparing `temper_core-0.2.1/temper_core/__init__.py` & `temper_core-0.3.0/temper_core/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Implementation of many of the connected methods in temper.
 """
 
 import sys
 import logging
 from abc import abstractmethod
+from functools import reduce
 from logging import getLogger, INFO
 from math import copysign, inf, isclose, isinf, isnan, nan
 from typing import (
     Union,
     Any,
     Callable,
     Iterable,
@@ -16,14 +17,15 @@
     TypeVar,
     Sequence,
     Generic,
     Protocol,
     Mapping,
     Optional,
     MutableSequence,
+    cast,
 )
 from sys import float_info
 from datetime import date as Date, datetime, timezone
 from types import MappingProxyType
 
 Unset = None
 "Abstraction used for tracking unset args."
@@ -268,49 +270,14 @@
 def cast_by_test(val: T, predicate: Callable[[T], bool]) -> Any:
     "This cast validates that a temper function meets some predicate, e.g. callable."
     if not predicate(val):
         raise ValueError()
     return val
 
 
-def adapt_generator(generator):
-    """
-    May be applied as a decorator to turn a Generator into a turn function.
-    """
-    # TODO: need type info for generator and result.
-    return lambda *args: GeneratorToStepFunctionAdapter(generator(*args))
-
-
-class GeneratorToStepFunctionAdapter(object):
-    """
-    Construct a callable function that calls next on an iterator.
-    """
-
-    __slots__ = ("_iterator", "value", "done")
-
-    # TODO: need a type on iterable and _iterator.
-    def __init__(self, iterable):
-        self._iterator = iter(iterable)
-        self.value = None
-        self.done = False
-
-    def __call__(self):
-        if not self.done:
-            try:
-                self.value = next(self._iterator)
-            except StopIteration as exc:
-                self.done = True
-                # TODO Retain original StopIteration? In what contexts used?
-                raise RuntimeError() from exc
-            except Exception as exc:
-                self.done = True
-                raise exc
-        return None
-
-
 class Label(BaseException):
     "A label enables labled breaks with reasonably readable python."
     __slots__ = ()
 
     def __enter__(self) -> "Label":
         return self
 
@@ -396,14 +363,22 @@
     def __iter__(self):
         raise NotImplementedError()
 
     def advance(self, count: int) -> "StringSlice":
         "Move the cursor forward by the given number of characters."
         raise NotImplementedError()
 
+    def intersect(self, other: "StringSlice") -> "StringSlice":
+        "The code units that are both in self and in other"
+        raise NotImplementedError()
+
+    def exclude_after(self, other: "StringSlice") -> "StringSlice":
+        "The code units in this before the left of other"
+        raise NotImplementedError()
+
     def _left_plus(self, count):
         raise NotImplementedError()
 
     def __bool__(self) -> bool:
         raise NotImplementedError()
 
     def __len__(self) -> int:
@@ -515,14 +490,45 @@
         left, right, content = self._left, self._left_plus(count), self._content
         if left >= right:
             left, right, content = 0, 0, ""
         if right == self._right:
             return self
         return Utf8StringSlice(left, right, content)
 
+    def intersect(self, other: StringSlice) -> "Utf8StringSlice":
+        content, left, right = self._content, self._left, self._right
+        other_typed = cast(Utf8StringSlice, other)
+        other_left, other_right = other_typed._left, other_typed._right
+
+        # Derivation of this in StringSliceHelpers
+        if other_left >= right:
+            new_left = right
+            new_right = right
+        elif other_right <= left:
+            new_left = left
+            new_right = left
+        else:
+            new_left = max(left, other_left)
+            new_right = min(right, other_right)
+
+        if new_left == left and new_right == right:
+            return self
+        else:
+            return Utf8StringSlice(new_left, new_right, content)
+
+    def exclude_after(self, other: StringSlice) -> "Utf8StringSlice":
+        content, left, right = self._content, self._left, self._right
+        other_typed = cast(Utf8StringSlice, other)
+        other_left = other_typed._left
+        new_right = max(left, min(right, other_left))
+        if right == new_right:
+            return self
+        else:
+            return Utf8StringSlice(left, new_right, content)
+
     def to_json(self):
         "Convert the Object into a JSON-compatable form."
         left, right, content = self._left, self._right, self._content
         return {"left": left, "right": right, "content": content}
 
     def __str__(self) -> str:
         left, right, content = self._left, self._right, self._content
@@ -628,14 +634,45 @@
         left, right, content = self._left, self._left_plus(count), self._content
         if left >= right:
             left, right, content = 0, 0, ""
         if right == self._right:
             return self
         return Utf16StringSlice(left, right, content)
 
+    def intersect(self, other: StringSlice) -> "Utf16StringSlice":
+        content, left, right = self._content, self._left, self._right
+        other_typed = cast(Utf16StringSlice, other)
+        other_left, other_right = other_typed._left, other_typed._right
+
+        # Derivation of this in StringSliceHelpers
+        if other_left >= right:
+            new_left = right
+            new_right = right
+        elif other_right <= left:
+            new_left = left
+            new_right = left
+        else:
+            new_left = max(left, other_left)
+            new_right = min(right, other_right)
+
+        if new_left == left and new_right == right:
+            return self
+        else:
+            return Utf16StringSlice(new_left, new_right, content)
+
+    def exclude_after(self, other: StringSlice) -> "Utf16StringSlice":
+        content, left, right = self._content, self._left, self._right
+        other_typed = cast(Utf16StringSlice, other)
+        other_left = other_typed._left
+        new_right = max(left, min(right, other_left))
+        if right == new_right:
+            return self
+        else:
+            return Utf16StringSlice(left, new_right, content)
+
     def to_json(self):
         "Convert the Object into a JSON-compatable form."
         left, right, content = self._left, self._right, self._content
         return {"left": left, "right": right, "content": content}
 
     def __str__(self) -> str:
         left, right, content = self._left, self._right, self._content
@@ -652,15 +689,15 @@
         if rsub:
             post = "\ufffd"
         else:
             post = ""
         return pre + content[lidx:ridx] + post
 
 
-class CodePointsStringSlice(StringSlice):
+class CodePointStringSlice(StringSlice):
     "Implementation of a StringSlice that advances over complete utf32 codePoints."
     __slots__ = ("_content", "_left", "_right")
     _left: int
     _right: int
     _content: str
 
     def __init__(self, left: int, right: int, content: str):
@@ -683,35 +720,66 @@
     def __bool__(self) -> bool:
         return bool(self._content)
 
     def _left_plus(self, count: int) -> int:
         left = self._left + count
         return -1 if left > len(self._content) else min(left, self._right)
 
-    def advance(self, count: int) -> "CodePointsStringSlice":
+    def advance(self, count: int) -> "CodePointStringSlice":
         if count <= 0:
             result = self
         else:
             left, right, content = self._left_plus(count), self._right, self._content
             if left < 0:
                 left, right, content = 0, 0, ""
-            result = CodePointsStringSlice(left, right, content)
+            result = CodePointStringSlice(left, right, content)
         return result
 
-    def limit(self, count: int) -> "CodePointsStringSlice":
+    def limit(self, count: int) -> "CodePointStringSlice":
         "Similar to advance, but moves the end count away from the current advance"
         if count <= 0:
-            result = CodePointsStringSlice(0, 0, "")
+            result = CodePointStringSlice(0, 0, "")
         else:
             left, right, content = self._left, self._left_plus(count), self._content
             if right <= self._left:
                 left, right, content = 0, 0, ""
-            result = CodePointsStringSlice(left, right, content)
+            result = CodePointStringSlice(left, right, content)
         return result
 
+    def intersect(self, other: StringSlice) -> "CodePointStringSlice":
+        content, left, right = self._content, self._left, self._right
+        other_typed = cast(CodePointStringSlice, other)
+        other_left, other_right = other_typed._left, other_typed._right
+
+        # Derivation of this in StringSliceHelpers
+        if other_left >= right:
+            new_left = right
+            new_right = right
+        elif other_right <= left:
+            new_left = left
+            new_right = left
+        else:
+            new_left = max(left, other_left)
+            new_right = min(right, other_right)
+
+        if new_left == left and new_right == right:
+            return self
+        else:
+            return CodePointStringSlice(new_left, new_right, content)
+
+    def exclude_after(self, other: StringSlice) -> "CodePointStringSlice":
+        content, left, right = self._content, self._left, self._right
+        other_typed = cast(CodePointStringSlice, other)
+        other_left = other_typed._left
+        new_right = max(left, min(right, other_left))
+        if right == new_right:
+            return self
+        else:
+            return CodePointStringSlice(left, new_right, content)
+
     def __str__(self) -> str:
         return self._content[self._left : self._right]
 
     def to_json(self):
         "Convert the Object into a JSON-compatable form."
         return {"left": self._left, "right": self._right, "content": self._content}
 
@@ -766,17 +834,17 @@
 
 
 def string_utf16(string: str) -> Utf16StringSlice:
     "Implements connected method String::utf16."
     return Utf16StringSlice(0, len(string) << 1, string)
 
 
-def string_code_points(string: str) -> CodePointsStringSlice:
+def string_code_points(string: str) -> CodePointStringSlice:
     "Implements connected method String::codePoints."
-    return CodePointsStringSlice(0, len(string), string)
+    return CodePointStringSlice(0, len(string), string)
 
 
 # Connected methods
 
 
 def int_to_float64(value: int) -> float:
     "Implements connected method Int::toFloat64."
@@ -1048,14 +1116,24 @@
     lst: Sequence[T], start_inclusive: int, end_exclusive: int
 ) -> Sequence[T]:
     "Almost exactly a Python slice, but indices are constrained to be >= 0."
     # TODO(tjp): Cheaper to always say tuple here, or separate out for ListBuilder use?
     return tuple(lst[max(start_inclusive, 0) : max(end_exclusive, 0)])
 
 
+def listed_reduce(lst: Sequence[T], accumulate: Callable[[T, T], T]) -> T:
+    return reduce(accumulate, lst)
+
+
+def listed_reduce_from(
+    lst: Sequence[T], initial: U, accumulate: Callable[[U, T], U]
+) -> U:
+    return reduce(accumulate, lst, initial)
+
+
 def listed_to_list(lst: Sequence[T]) -> Sequence[T]:
     if isinstance(lst, tuple):
         return lst
     else:
         return tuple(lst)
```

### Comparing `temper_core-0.2.1/temper_core/regex.py` & `temper_core-0.3.0/temper_core/regex.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import typing
 import types
 
 
-def compiled_regex_compiled_find(_, compiled: re.Pattern, text: str, regex_refs):
+def regex_compiled_find(_, compiled: re.Pattern, text: str, regex_refs):
     match = compiled.search(text)
     if match is None:
         raise RuntimeError()
     return _convert_match(match, regex_refs)
 
 
 def _convert_match(match, regex_refs):
@@ -18,32 +18,32 @@
     if "full" not in groups:
         result["full"] = Group("full", match.group(), match.start())
     for name, value in groups.items():
         result[name] = Group(name, value or "", match.start(name))
     return result
 
 
-def compiled_regex_compiled_found(_, compiled: re.Pattern, text: str):
+def regex_compiled_found(_, compiled: re.Pattern, text: str):
     return compiled.search(text) is not None
 
 
-def compiled_regex_compiled_replace(
+def regex_compiled_replace(
     _,
     compiled: re.Pattern,
     text: str,
     format: typing.Callable[[types.MappingProxyType[str, typing.Any]], str],
     regex_refs,
 ):
     def adapted_format(match):
         return format(_convert_match(match, regex_refs))
 
     return compiled.sub(adapted_format, text)
 
 
-def compiled_regex_compile_formatted(_, formatted: str):
+def regex_compile_formatted(_, formatted: str):
     return re.compile(formatted, re.ASCII)
 
 
 def regex_formatter_push_capture_name(_, out: typing.MutableSequence[str], name: str):
     out.append(rf"?P<{name}>")
```

### Comparing `temper_core-0.2.1/temper_core/testing.py` & `temper_core-0.3.0/temper_core/testing.py`

 * *Files identical despite different names*

