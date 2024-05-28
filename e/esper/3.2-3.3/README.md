# Comparing `tmp/esper-3.2.tar.gz` & `tmp/esper-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esper-3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "esper-3.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `esper-3.2.tar` & `esper-3.3.tar`

### file list

```diff
@@ -1,34 +1,33 @@
--rw-r--r--   0        0        0      487 2022-10-01 12:58:49.246506 esper-3.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      472 2022-10-01 12:58:49.246506 esper-3.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      121 2022-10-05 08:42:57.922654 esper-3.2/.github/ISSUE_TEMPLATE/question-or-comment.md
--rw-r--r--   0        0        0      649 2023-12-21 01:38:55.194778 esper-3.2/.github/workflows/type-checking.yml
--rw-r--r--   0        0        0      670 2023-12-21 01:38:55.198111 esper-3.2/.github/workflows/unit-tests.yml
--rw-r--r--   0        0        0      425 2023-11-21 08:19:48.464810 esper-3.2/.gitignore
--rw-r--r--   0        0        0      450 2024-01-05 06:27:43.568268 esper-3.2/.mypy.ini
--rw-r--r--   0        0        0      368 2023-11-15 05:24:24.130203 esper-3.2/.readthedocs.yaml
--rw-r--r--   0        0        0      118 2023-09-23 13:23:26.504867 esper-3.2/.ruff.toml
--rw-r--r--   0        0        0     1081 2023-11-21 08:11:35.333048 esper-3.2/LICENSE
--rw-r--r--   0        0        0       35 2018-05-28 13:41:03.000000 esper-3.2/MANIFEST.in
--rw-r--r--   0        0        0    16868 2023-12-21 05:11:34.434821 esper-3.2/README.md
--rw-r--r--   0        0        0     4248 2023-12-21 04:43:05.796860 esper-3.2/RELEASE_NOTES
--rw-r--r--   0        0        0      634 2019-08-24 11:00:40.000000 esper-3.2/docs/Makefile
--rw-r--r--   0        0        0     1962 2022-03-15 09:31:20.011281 esper-3.2/docs/conf.py
--rw-r--r--   0        0        0     1668 2023-09-23 13:23:26.504867 esper-3.2/docs/index.rst
--rw-r--r--   0        0        0      795 2019-08-24 11:00:40.000000 esper-3.2/docs/make.bat
--rw-r--r--   0        0        0    19167 2024-01-05 06:34:23.971915 esper-3.2/esper/__init__.py
--rw-r--r--   0        0        0        0 2021-10-01 09:10:51.270566 esper-3.2/esper/py.typed
--rw-r--r--   0        0        0     4683 2023-09-23 13:23:26.504867 esper-3.2/examples/benchmark.py
--rw-r--r--   0        0        0     3369 2023-09-23 13:23:26.504867 esper-3.2/examples/benchmark_cache.py
--rw-r--r--   0        0        0      215 2016-01-02 11:48:39.000000 esper-3.2/examples/bluesquare.png
--rw-r--r--   0        0        0     1476 2023-09-23 13:23:26.504867 esper-3.2/examples/headless_example.py
--rw-r--r--   0        0        0     4778 2023-09-23 13:23:26.504867 esper-3.2/examples/pygame_example.py
--rw-r--r--   0        0        0     4378 2023-09-23 13:23:26.504867 esper-3.2/examples/pyglet_example.py
--rwxr-xr-x   0        0        0     8264 2023-09-23 13:23:26.504867 esper-3.2/examples/pyglet_example_batch.py
--rw-r--r--   0        0        0     5766 2023-09-23 13:23:26.504867 esper-3.2/examples/pysdl2_example.py
--rw-r--r--   0        0        0     2042 2016-04-19 12:26:15.000000 esper-3.2/examples/pythonista_ios_example.py
--rw-r--r--   0        0        0      218 2016-01-02 11:48:15.000000 esper-3.2/examples/redsquare.png
--rwxr-xr-x   0        0        0     1238 2023-11-21 08:30:03.902927 esper-3.2/make.py
--rw-r--r--   0        0        0      416 2023-11-21 08:28:29.680659 esper-3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-20 00:18:39.000571 esper-3.2/tests/__init__.py
--rw-r--r--   0        0        0    17239 2023-12-21 04:43:05.800193 esper-3.2/tests/test_world.py
--rw-r--r--   0        0        0    17233 1970-01-01 00:00:00.000000 esper-3.2/PKG-INFO
+-rw-r--r--   0        0        0      487 2022-10-01 12:58:49.246506 esper-3.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      472 2022-10-01 12:58:49.246506 esper-3.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      121 2022-10-05 08:42:57.922654 esper-3.3/.github/ISSUE_TEMPLATE/question-or-comment.md
+-rw-r--r--   0        0        0      649 2023-12-21 01:38:55.194778 esper-3.3/.github/workflows/type-checking.yml
+-rw-r--r--   0        0        0      670 2023-12-21 01:38:55.198111 esper-3.3/.github/workflows/unit-tests.yml
+-rw-r--r--   0        0        0      425 2023-11-21 08:19:48.464810 esper-3.3/.gitignore
+-rw-r--r--   0        0        0      450 2024-01-05 06:27:43.568268 esper-3.3/.mypy.ini
+-rw-r--r--   0        0        0      368 2023-11-15 05:24:24.130203 esper-3.3/.readthedocs.yaml
+-rw-r--r--   0        0        0      127 2024-05-28 00:35:43.344550 esper-3.3/.ruff.toml
+-rw-r--r--   0        0        0     1081 2024-05-28 00:38:13.125005 esper-3.3/LICENSE
+-rw-r--r--   0        0        0       35 2018-05-28 13:41:03.000000 esper-3.3/MANIFEST.in
+-rw-r--r--   0        0        0    16866 2024-05-28 00:43:58.971919 esper-3.3/README.md
+-rw-r--r--   0        0        0     4465 2024-05-28 00:43:47.821725 esper-3.3/RELEASE_NOTES
+-rw-r--r--   0        0        0      634 2019-08-24 11:00:40.000000 esper-3.3/docs/Makefile
+-rw-r--r--   0        0        0     1962 2022-03-15 09:31:20.011281 esper-3.3/docs/conf.py
+-rw-r--r--   0        0        0     1668 2023-09-23 13:23:26.504867 esper-3.3/docs/index.rst
+-rw-r--r--   0        0        0      795 2019-08-24 11:00:40.000000 esper-3.3/docs/make.bat
+-rw-r--r--   0        0        0    19254 2024-05-28 00:36:56.743151 esper-3.3/esper/__init__.py
+-rw-r--r--   0        0        0        0 2021-10-01 09:10:51.270566 esper-3.3/esper/py.typed
+-rw-r--r--   0        0        0     4683 2023-09-23 13:23:26.504867 esper-3.3/examples/benchmark.py
+-rw-r--r--   0        0        0     3369 2023-09-23 13:23:26.504867 esper-3.3/examples/benchmark_cache.py
+-rw-r--r--   0        0        0      215 2016-01-02 11:48:39.000000 esper-3.3/examples/bluesquare.png
+-rw-r--r--   0        0        0     1476 2023-09-23 13:23:26.504867 esper-3.3/examples/headless_example.py
+-rw-r--r--   0        0        0     4778 2023-09-23 13:23:26.504867 esper-3.3/examples/pygame_example.py
+-rw-r--r--   0        0        0     4377 2024-05-28 00:41:46.666177 esper-3.3/examples/pyglet_example.py
+-rw-r--r--   0        0        0     5766 2023-09-23 13:23:26.504867 esper-3.3/examples/pysdl2_example.py
+-rw-r--r--   0        0        0     2042 2016-04-19 12:26:15.000000 esper-3.3/examples/pythonista_ios_example.py
+-rw-r--r--   0        0        0      218 2016-01-02 11:48:15.000000 esper-3.3/examples/redsquare.png
+-rwxr-xr-x   0        0        0     1238 2023-11-21 08:30:03.902927 esper-3.3/make.py
+-rw-r--r--   0        0        0      416 2023-11-21 08:28:29.680659 esper-3.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-20 00:18:39.000571 esper-3.3/tests/__init__.py
+-rw-r--r--   0        0        0    17239 2023-12-21 04:43:05.800193 esper-3.3/tests/test_world.py
+-rw-r--r--   0        0        0    17231 1970-01-01 00:00:00.000000 esper-3.3/PKG-INFO
```

### Comparing `esper-3.2/.github/workflows/type-checking.yml` & `esper-3.3/.github/workflows/type-checking.yml`

 * *Files identical despite different names*

### Comparing `esper-3.2/.github/workflows/unit-tests.yml` & `esper-3.3/.github/workflows/unit-tests.yml`

 * *Files identical despite different names*

### Comparing `esper-3.2/LICENSE` & `esper-3.3/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2023 Benjamin Moran
+Copyright (c) 2024 Benjamin Moran
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `esper-3.2/README.md` & `esper-3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: esper
+Version: 3.3
+Summary: esper is a lightweight Entity System (ECS) for Python, with a focus on performance
+Author-email: Benjamin Moran <benmoran@protonmail.com>
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Classifier: License :: OSI Approved :: MIT License
+Project-URL: Home, https://github.com/benmoran56/esper
+
 [![pypi](https://badge.fury.io/py/esper.svg)](https://pypi.python.org/pypi/esper)
 [![rtd](https://readthedocs.org/projects/esper/badge/?version=latest)](https://esper.readthedocs.io)
 [![PyTest](https://github.com/benmoran56/esper/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/benmoran56/esper/actions/workflows/unit-tests.yml)
 
 Esper is a lightweight Entity System module for Python, with a focus on performance
 ===================================================================================
 
@@ -61,15 +71,15 @@
 
 Design
 ======
 
 * World Context
 
 Esper uses the concept of "World" contexts. When you first `import esper`, a default context is
-active. You create Entities, assign Components, register Processesors, etc., by calling functions
+active. You create Entities, assign Components, register Processors, etc., by calling functions
 on the `esper` module. Entities, Components and Processors can be created, assigned, or deleted
 while your game is running. A simple call to `esper.process()` is all that's needed for each
 iteration of your game loop. Advanced users can switch contexts, which can be useful for
 isolating different game scenes that have different Processor requirements.
 
 
 * Entities 
@@ -393,7 +403,8 @@
 - Try to target all non-EOL Python versions. Exceptions can be made if there is a compelling reason.
 - Avoid bloat as much as possible. New features will be considered if they are commonly useful. Generally speaking, we don't want to add functionality that is better served by another module or library. 
 - Performance is preferrable to readability. The public API should remain clean, but ugly internal code is acceptable if it provides a performance benefit. Every cycle counts! 
 
 If you have any questions before contributing, feel free to [open an issue].
 
 [open an issue]: https://github.com/benmoran56/esper/issues
+
```

### Comparing `esper-3.2/RELEASE_NOTES` & `esper-3.3/RELEASE_NOTES`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+esper 3.3
+=========
+Maintenance release
+
+Changes
+-------
+- Fix unreadable `esper.current_world` property. (#100)
+- Minor typing configuration updates.
+- Remove outdated pyglet example. (Another one already exists).
+
+
 esper 3.2
 =========
 Maintenance release
 
 Changes
 -------
 - Add `esper.current_world` property to easily check the current World context.
```

### Comparing `esper-3.2/docs/Makefile` & `esper-3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `esper-3.2/docs/conf.py` & `esper-3.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `esper-3.2/docs/index.rst` & `esper-3.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `esper-3.2/docs/make.bat` & `esper-3.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `esper-3.2/esper/__init__.py` & `esper-3.3/esper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from typing import overload as _overload
 
 from weakref import ref as _ref
 from weakref import WeakMethod as _WeakMethod
 
 from itertools import count as _count
 
-__version__ = version = '3.2'
+__version__ = version = '3.3'
 
 
 ###################
 #  Event system
 ###################
 
 
@@ -127,26 +127,34 @@
         raise NotImplementedError
 
 
 ###################
 #   ECS functions
 ###################
 
-_current_context: str = "default"
+_current_world: str = "default"
 _entity_count: "_count[int]" = _count(start=1)
 _components: _Dict[_Type[_Any], _Set[_Any]] = {}
 _entities: _Dict[int, _Dict[_Type[_Any], _Any]] = {}
 _dead_entities: _Set[int] = set()
 _get_component_cache: _Dict[_Type[_Any], _List[_Any]] = {}
 _get_components_cache: _Dict[_Tuple[_Type[_Any], ...], _List[_Any]] = {}
 _processors: _List[Processor] = []
 process_times: _Dict[str, int] = {}
 event_registry: _Dict[str, _Any] = {}
+current_world: str = "default"
+"""The name of the currently active World context.
 
-# {context_name: (entity_count, components, entities, dead_entities, comp_cache, comps_cache, processors, process_times, event_registry)}
+This attribute can be checked to confirm the name of the
+currently active World context. Modifying this has no effect;
+to switch Worlds, use the :py:func:`~switch_world` function.
+"""
+
+# {context_name: (entity_count, components, entities, dead_entities,
+#                 comp_cache, comps_cache, processors, process_times, event_registry)}
 _context_map: _Dict[str, _Tuple[
     "_count[int]",
     _Dict[_Type[_Any], _Set[_Any]],
     _Dict[int, _Dict[_Type[_Any], _Any]],
     _Set[int],
     _Dict[_Type[_Any], _List[_Any]],
     _Dict[_Tuple[_Type[_Any], ...], _List[_Any]],
@@ -383,43 +391,39 @@
 
 
 def get_component(component_type: _Type[_C]) -> _List[_Tuple[int, _C]]:
     """Get an iterator for Entity, Component pairs."""
     try:
         return _get_component_cache[component_type]
     except KeyError:
-        return _get_component_cache.setdefault(
-            component_type, list(_get_component(component_type))
-        )
+        return _get_component_cache.setdefault(component_type, list(_get_component(component_type)))
 
 
 @_overload
 def get_components(__c1: _Type[_C], __c2: _Type[_C2]) -> _List[_Tuple[int, _Tuple[_C, _C2]]]:
     ...
 
 
 @_overload
 def get_components(__c1: _Type[_C], __c2: _Type[_C2], __c3: _Type[_C3]) -> _List[_Tuple[int, _Tuple[_C, _C2, _C3]]]:
     ...
 
 
 @_overload
 def get_components(__c1: _Type[_C], __c2: _Type[_C2], __c3: _Type[_C3], __c4: _Type[_C4]) -> _List[
-    _Tuple[int, _Tuple[_C, _C2, _C3, _C4]]]:
+                   _Tuple[int, _Tuple[_C, _C2, _C3, _C4]]]:
     ...
 
 
 def get_components(*component_types: _Type[_Any]) -> _Iterable[_Tuple[int, _Tuple[_Any, ...]]]:
     """Get an iterator for Entity and multiple Component sets."""
     try:
         return _get_components_cache[component_types]
     except KeyError:
-        return _get_components_cache.setdefault(
-            component_types, list(_get_components(*component_types))
-        )
+        return _get_components_cache.setdefault(component_types, list(_get_components(*component_types)))
 
 
 def try_component(entity: int, component_type: _Type[_C]) -> _Optional[_C]:
     """Try to get a single component type for an Entity.
 
     This function will return the requested Component if it exists,
     or None if it does not. This allows a way to access optional Components
@@ -521,15 +525,15 @@
 
     This will completely delete the World, including all entities
     that are contained within it.
 
     Raises `PermissionError` if you attempt to delete the currently
     active World context.
     """
-    if _current_context == name:
+    if _current_world == name:
         raise PermissionError("The active World context cannot be deleted.")
 
     del _context_map[name]
 
 
 def switch_world(name: str) -> None:
     """Switch to a new World context by name.
@@ -546,31 +550,23 @@
 
     .. note:: At startup, a "default" World context is active.
     """
     if name not in _context_map:
         # Create a new context if the name does not already exist:
         _context_map[name] = (_count(start=1), {}, {}, set(), {}, {}, [], {}, {})
 
-    global _current_context
+    global _current_world
     global _entity_count
     global _components
     global _entities
     global _dead_entities
     global _get_component_cache
     global _get_components_cache
     global _processors
     global process_times
     global event_registry
+    global current_world
 
     # switch the references to the objects in the named context_map:
     (_entity_count, _components, _entities, _dead_entities, _get_component_cache,
      _get_components_cache, _processors, process_times, event_registry) = _context_map[name]
-    _current_context = name
-
-
-@property   # type: ignore
-def current_world() -> str:
-    """The currently active World context.
-
-    To switch World contexts, see :py:func:`esper.switch_world`.
-    """
-    return _current_context
+    _current_world = current_world = name
```

### Comparing `esper-3.2/examples/benchmark.py` & `esper-3.3/examples/benchmark.py`

 * *Files identical despite different names*

### Comparing `esper-3.2/examples/benchmark_cache.py` & `esper-3.3/examples/benchmark_cache.py`

 * *Files identical despite different names*

### Comparing `esper-3.2/examples/headless_example.py` & `esper-3.3/examples/headless_example.py`

 * *Files identical despite different names*

### Comparing `esper-3.2/examples/pygame_example.py` & `esper-3.3/examples/pygame_example.py`

 * *Files identical despite different names*

### Comparing `esper-3.2/examples/pyglet_example.py` & `esper-3.3/examples/pyglet_example.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         self.miny = miny
         self.maxx = maxx
         self.maxy = maxy
 
     def process(self, dt):
         # This will iterate over every Entity that has BOTH of these components:
         for ent, (vel, rend) in esper.get_components(Velocity, Renderable):
-            # Update the Renderable Component's position by it's Velocity:
+            # Update the Renderable Component's position by its Velocity:
             # An example of keeping the sprite inside screen boundaries. Basically,
             # adjust the position back inside screen boundaries if it is outside:
             new_x = max(self.minx, rend.sprite.x + vel.x)
             new_y = max(self.miny, rend.sprite.y + vel.y)
             new_x = min(self.maxx - rend.w, new_x)
             new_y = min(self.maxy - rend.h, new_y)
             rend.sprite.position = new_x, new_y, rend.sprite.z
```

### Comparing `esper-3.2/examples/pysdl2_example.py` & `esper-3.3/examples/pysdl2_example.py`

 * *Files identical despite different names*

### Comparing `esper-3.2/examples/pythonista_ios_example.py` & `esper-3.3/examples/pythonista_ios_example.py`

 * *Files identical despite different names*

### Comparing `esper-3.2/make.py` & `esper-3.3/make.py`

 * *Files identical despite different names*

### Comparing `esper-3.2/tests/test_world.py` & `esper-3.3/tests/test_world.py`

 * *Files identical despite different names*

### Comparing `esper-3.2/PKG-INFO` & `esper-3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: esper
-Version: 3.2
-Summary: esper is a lightweight Entity System (ECS) for Python, with a focus on performance
-Author-email: Benjamin Moran <benmoran@protonmail.com>
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Classifier: License :: OSI Approved :: MIT License
-Project-URL: Home, https://github.com/benmoran56/esper
-
 [![pypi](https://badge.fury.io/py/esper.svg)](https://pypi.python.org/pypi/esper)
 [![rtd](https://readthedocs.org/projects/esper/badge/?version=latest)](https://esper.readthedocs.io)
 [![PyTest](https://github.com/benmoran56/esper/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/benmoran56/esper/actions/workflows/unit-tests.yml)
 
 Esper is a lightweight Entity System module for Python, with a focus on performance
 ===================================================================================
 
@@ -71,15 +61,15 @@
 
 Design
 ======
 
 * World Context
 
 Esper uses the concept of "World" contexts. When you first `import esper`, a default context is
-active. You create Entities, assign Components, register Processesors, etc., by calling functions
+active. You create Entities, assign Components, register Processors, etc., by calling functions
 on the `esper` module. Entities, Components and Processors can be created, assigned, or deleted
 while your game is running. A simple call to `esper.process()` is all that's needed for each
 iteration of your game loop. Advanced users can switch contexts, which can be useful for
 isolating different game scenes that have different Processor requirements.
 
 
 * Entities 
@@ -403,8 +393,7 @@
 - Try to target all non-EOL Python versions. Exceptions can be made if there is a compelling reason.
 - Avoid bloat as much as possible. New features will be considered if they are commonly useful. Generally speaking, we don't want to add functionality that is better served by another module or library. 
 - Performance is preferrable to readability. The public API should remain clean, but ugly internal code is acceptable if it provides a performance benefit. Every cycle counts! 
 
 If you have any questions before contributing, feel free to [open an issue].
 
 [open an issue]: https://github.com/benmoran56/esper/issues
-
```

