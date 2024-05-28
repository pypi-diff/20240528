# Comparing `tmp/pytest_when-1.1.5.tar.gz` & `tmp/pytest_when-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_when-1.1.5.tar", last modified: Fri Mar 22 17:00:21 2024, max compression
+gzip compressed data, was "pytest_when-2.0.0.tar", last modified: Tue May 28 18:47:13 2024, max compression
```

## Comparing `pytest_when-1.1.5.tar` & `pytest_when-2.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1069 2024-03-22 17:00:03.435420 pytest_when-1.1.5/LICENSE
--rw-r--r--   0        0        0     5198 2024-03-22 17:00:03.435420 pytest_when-1.1.5/README.md
--rw-r--r--   0        0        0     2801 2024-03-22 17:00:21.975327 pytest_when-1.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-22 17:00:03.435420 pytest_when-1.1.5/pytest_when/__init__.py
--rw-r--r--   0        0        0       45 2024-03-22 17:00:03.435420 pytest_when-1.1.5/pytest_when/plugin.py
--rw-r--r--   0        0        0        0 2024-03-22 17:00:03.435420 pytest_when-1.1.5/pytest_when/py.typed
--rw-r--r--   0        0        0    11204 2024-03-22 17:00:03.435420 pytest_when-1.1.5/pytest_when/when.py
--rw-r--r--   0        0        0        0 2024-03-22 17:00:03.435420 pytest_when-1.1.5/tests/resources/__init__.py
--rw-r--r--   0        0        0      294 2024-03-22 17:00:03.435420 pytest_when-1.1.5/tests/resources/example_module.py
--rw-r--r--   0        0        0     3795 2024-03-22 17:00:03.435420 pytest_when-1.1.5/tests/test_create_call_key.py
--rw-r--r--   0        0        0     6560 2024-03-22 17:00:03.435420 pytest_when-1.1.5/tests/test_integration.py
--rw-r--r--   0        0        0     5617 1970-01-01 00:00:00.000000 pytest_when-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-28 18:46:55.662285 pytest_when-2.0.0/LICENSE
+-rw-r--r--   0        0        0     5198 2024-05-28 18:46:55.662285 pytest_when-2.0.0/README.md
+-rw-r--r--   0        0        0     2804 2024-05-28 18:47:13.602476 pytest_when-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-28 18:46:55.662285 pytest_when-2.0.0/pytest_when/__init__.py
+-rw-r--r--   0        0        0       45 2024-05-28 18:46:55.662285 pytest_when-2.0.0/pytest_when/plugin.py
+-rw-r--r--   0        0        0        0 2024-05-28 18:46:55.662285 pytest_when-2.0.0/pytest_when/py.typed
+-rw-r--r--   0        0        0    11689 2024-05-28 18:46:55.662285 pytest_when-2.0.0/pytest_when/when.py
+-rw-r--r--   0        0        0        0 2024-05-28 18:46:55.662285 pytest_when-2.0.0/tests/resources/__init__.py
+-rw-r--r--   0        0        0      294 2024-05-28 18:46:55.662285 pytest_when-2.0.0/tests/resources/example_module.py
+-rw-r--r--   0        0        0     3795 2024-05-28 18:46:55.662285 pytest_when-2.0.0/tests/test_create_call_key.py
+-rw-r--r--   0        0        0     7095 2024-05-28 18:46:55.662285 pytest_when-2.0.0/tests/test_integration.py
+-rw-r--r--   0        0        0     5618 1970-01-01 00:00:00.000000 pytest_when-2.0.0/PKG-INFO
```

### Comparing `pytest_when-1.1.5/LICENSE` & `pytest_when-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_when-1.1.5/README.md` & `pytest_when-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_when-1.1.5/pyproject.toml` & `pytest_when-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.black]
 line-length = 79
 target-version = [
-    "py38",
+    "py310",
 ]
 
 [tool.ruff]
-target-version = "py38"
+target-version = "py310"
 
 [tool.ruff.lint]
 ignore = [
     "E501",
     "D107",
     "D203",
     "D211",
@@ -154,17 +154,17 @@
     { name = "zhukovgreen", email = "iam+pytest-when@zhukovgreen.pro" },
 ]
 dependencies = [
     "pytest>=7.3.1",
     "pytest-mock>=3.14.0",
     "typing-extensions>=4.5.0",
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 readme = "README.md"
-version = "1.1.5"
+version = "2.0.0"
 
 [project.entry-points.pytest11]
 pytest-when = "pytest_when.plugin"
 
 [project.urls]
 repository = "https://github.com/zhukovgreen/pytest-when"
```

### Comparing `pytest_when-1.1.5/pytest_when/when.py` & `pytest_when-2.0.0/pytest_when/when.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,14 @@
 import enum
 import functools
 import inspect
 
 from collections import deque
-from collections.abc import Mapping
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    Generic,
-    Hashable,
-    List,
-    Protocol,
-    Set,
-    Tuple,
-    TypeVar,
-    Union,
-)
+from collections.abc import Callable, Hashable, Mapping
+from typing import Any, Generic, Protocol, TypeVar
 from unittest.mock import MagicMock
 
 import pytest
 
 from pytest_mock import MockerFixture
 from pytest_mock.plugin import MockCacheItem
 from typing_extensions import ParamSpec
@@ -29,53 +17,53 @@
 class HasNameDunder(Protocol):
     __name__: str
 
 
 _TargetClsType = TypeVar("_TargetClsType", bound=HasNameDunder)
 _TargetMethodParams = ParamSpec("_TargetMethodParams")
 _TargetMethodReturn = TypeVar("_TargetMethodReturn")
-_TargetMethodKey = Tuple[str, str]
+_TargetMethodKey = tuple[str, str]
 
-_TargetMethodArgs = Tuple[Any, ...]
-_TargetMethodKwargs = Dict[str, Any]
+_TargetMethodArgs = tuple[Any, ...]
+_TargetMethodKwargs = dict[str, Any]
 
-_CallKeyParamDef = Tuple[str, Any]
-_CallKey = Tuple[_CallKeyParamDef, ...]
+_CallKeyParamDef = tuple[str, Any]
+_CallKey = tuple[_CallKeyParamDef, ...]
 
 
 class Markers(enum.Enum):
     """Markers for defining When.called_with arguments.
 
     Markers.any - means the argument could be anything
     """
 
     any: str = "any"
 
 
 def make_container_hashable(
-    container: Tuple[Tuple[str, Any], ...]
-) -> Tuple[Tuple[str, Any], ...]:
+    container: tuple[tuple[str, Any], ...]
+) -> tuple[tuple[str, Any], ...]:
     """Make call signature hashable recursively."""
     return tuple((arg, make_hashable(value)) for arg, value in container)
 
 
 @functools.singledispatch
 def make_hashable(val) -> Hashable:
     """Single dispatch function to ensure the generic val is hashable."""
     return val
 
 
 @make_hashable.register
-def _(val: Mapping) -> Tuple[Tuple[str, Any], ...]:
+def _(val: Mapping) -> tuple[tuple[str, Any], ...]:
     return tuple((k, make_hashable(v)) for k, v in val.items())
 
 
 @make_hashable.register(list)
 @make_hashable.register(set)
-def _(val: Union[List[Any], Set[Any]]) -> Tuple[Any, ...]:
+def _(val: list[Any] | set[Any]) -> tuple[Any, ...]:
     return tuple(map(make_hashable, val))
 
 
 def create_call_key(
     original_callable_sig: inspect.Signature,
     *args: _TargetMethodArgs,
     **kwargs: _TargetMethodKwargs,
@@ -91,15 +79,15 @@
     call = original_callable_sig.bind(*args, **kwargs)
 
     return make_container_hashable(tuple(call.arguments.items()))
 
 
 def get_mocked_call_result(
     original_callable_sig: inspect.Signature,
-    mocked_calls: Dict[
+    mocked_calls: dict[
         _CallKey,
         _TargetMethodReturn,
     ],
     *args: _TargetMethodArgs,
     **kwargs: _TargetMethodKwargs,
 ) -> _TargetMethodReturn:
     call_key = create_call_key(
@@ -108,34 +96,47 @@
         **kwargs,
     )
 
     def params_are_compatible(
         param_in_mocked_calls: _CallKeyParamDef,
         param_in_call: _CallKeyParamDef,
     ) -> bool:
+        # sanitize ("kwargs", ((..., ...))) calls. This call
+        #   structure comes when parameter is missed in the func signature,
+        #   but can be specified due to **kwargs. Then we need to check
+        #   each ... pair separately
+        if param_in_call[0] == "kwargs":
+            return all(
+                params_are_compatible(_mocked_call, _call)
+                for _mocked_call, _call in zip(
+                    param_in_mocked_calls[1], param_in_call[1], strict=False
+                )
+            )
         assert param_in_mocked_calls[0] == param_in_call[0]
         return (
             param_in_mocked_calls[1] is Markers.any
             or param_in_mocked_calls[1] == param_in_call[1]
         )
 
     def call_matched_call_key(mocked_call_key: _CallKey) -> bool:
         return all(
             params_are_compatible(param_1, param_2)
-            for param_1, param_2 in zip(mocked_call_key, call_key)
+            for param_1, param_2 in zip(
+                mocked_call_key, call_key, strict=False
+            )
         )
 
     for call in filter(call_matched_call_key, mocked_calls):
         return mocked_calls[call]
     raise KeyError(f"Call {call_key} is not in mocked_calls {mocked_calls}")
 
 
 def side_effect_factory(
     origin_callable: Callable[_TargetMethodParams, _TargetMethodReturn],
-    mocked_calls: Dict[_CallKey, _TargetMethodReturn],
+    mocked_calls: dict[_CallKey, _TargetMethodReturn],
 ) -> Callable[_TargetMethodParams, _TargetMethodReturn]:
     def side_effect(
         *args: _TargetMethodParams.args,
         **kwargs: _TargetMethodParams.kwargs,
     ) -> _TargetMethodReturn:
         try:
             return get_mocked_call_result(
@@ -153,17 +154,17 @@
 class MockedCalls(
     Generic[
         _TargetClsType,
         _TargetMethodParams,
         _TargetMethodReturn,
     ]
 ):
-    mocked_calls_registry: Dict[
+    mocked_calls_registry: dict[
         _TargetMethodKey,
-        Dict[_CallKey, _TargetMethodReturn],
+        dict[_CallKey, _TargetMethodReturn],
     ] = {}  # noqa: RUF012
 
     def __init__(self, mocker: MockerFixture) -> None:
         self.mocker = mocker
 
     def add_call(
         self,
```

### Comparing `pytest_when-1.1.5/tests/test_create_call_key.py` & `pytest_when-2.0.0/tests/test_create_call_key.py`

 * *Files identical despite different names*

### Comparing `pytest_when-1.1.5/tests/test_integration.py` & `pytest_when-2.0.0/tests/test_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -306,7 +306,27 @@
     patched_foo = (
         when(example_module, "some_foo_without_args")
         .called_with()
         .then_return("Mocked")
     )
     assert example_module.some_foo_without_args() == "Mocked"
     patched_foo.assert_called()
+
+
+def test_should_work_with_star_kwargs(when, mocker):
+    class _:  # noqa: N801
+        @staticmethod
+        def foo(a, **kwargs):  # noqa: ARG004
+            return "Not mocked"
+
+    patched_foo = (
+        when(_, "foo")
+        .called_with(
+            1,
+            kwarg_a=when.markers.any,
+            kwarg_b="bbb",
+        )
+        .then_return("Mocked")
+    )
+    assert _.foo(1, kwarg_a="aaa", kwarg_b="bbb") == "Mocked"
+    assert _.foo(2, kwarg_a="aaa", kwarg_b="bbb") == "Not mocked"
+    patched_foo.assert_called()
```

### Comparing `pytest_when-1.1.5/PKG-INFO` & `pytest_when-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pytest-when
-Version: 1.1.5
+Version: 2.0.0
 Summary: Utility which makes mocking more readable and controllable
 Author-Email: zhukovgreen <iam+pytest-when@zhukovgreen.pro>
 Project-URL: Repository, https://github.com/zhukovgreen/pytest-when
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Requires-Dist: pytest>=7.3.1
 Requires-Dist: pytest-mock>=3.14.0
 Requires-Dist: typing-extensions>=4.5.0
 Description-Content-Type: text/markdown
 
 [![PyPI](https://img.shields.io/pypi/v/pytest-when.svg)](https://pypi.python.org/pypi/pytest-when)
 [![Build](https://github.com/Tinche/tightwrap/workflows/CI/badge.svg)](https://github.com/zhukovgreen/pytest-when/actions/workflows/test-lint.yml?query=workflow:%22Test+Action%22)
```

