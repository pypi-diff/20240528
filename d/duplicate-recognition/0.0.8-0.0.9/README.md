# Comparing `tmp/duplicate_recognition-0.0.8-py3-none-any.whl.zip` & `tmp/duplicate_recognition-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 10247 bytes, number of entries: 9
--rw-r--r--  2.0 unx      205 b- defN 20-Feb-02 00:00 duplicate_recognition/__init__.py
--rw-r--r--  2.0 unx     8467 b- defN 20-Feb-02 00:00 duplicate_recognition/entity_algorithm.py
+Zip file size: 10516 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      191 b- defN 20-Feb-02 00:00 duplicate_recognition/__init__.py
+-rw-r--r--  2.0 unx    10371 b- defN 20-Feb-02 00:00 duplicate_recognition/entity_algorithm.py
 -rw-r--r--  2.0 unx     4512 b- defN 20-Feb-02 00:00 duplicate_recognition/field_algorythm.py
 -rw-r--r--  2.0 unx     3058 b- defN 20-Feb-02 00:00 duplicate_recognition/statistics.py
--rw-r--r--  2.0 unx      474 b- defN 20-Feb-02 00:00 duplicate_recognition/utils.py
-?rw-r--r--  2.0 unx     6321 b- defN 20-Feb-02 00:00 duplicate_recognition-0.0.8.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 duplicate_recognition-0.0.8.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1058 b- defN 20-Feb-02 00:00 duplicate_recognition-0.0.8.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      821 b- defN 20-Feb-02 00:00 duplicate_recognition-0.0.8.dist-info/RECORD
-9 files, 25003 bytes uncompressed, 8809 bytes compressed:  64.8%
+-rw-r--r--  2.0 unx      161 b- defN 20-Feb-02 00:00 duplicate_recognition/utils.py
+?rw-r--r--  2.0 unx     6321 b- defN 20-Feb-02 00:00 duplicate_recognition-0.0.9.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 duplicate_recognition-0.0.9.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1058 b- defN 20-Feb-02 00:00 duplicate_recognition-0.0.9.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      822 b- defN 20-Feb-02 00:00 duplicate_recognition-0.0.9.dist-info/RECORD
+9 files, 26581 bytes uncompressed, 9078 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: duplicate_recognition/statistics.py
 Comment: 
 
 Filename: duplicate_recognition/utils.py
 Comment: 
 
-Filename: duplicate_recognition-0.0.8.dist-info/METADATA
+Filename: duplicate_recognition-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: duplicate_recognition-0.0.8.dist-info/WHEEL
+Filename: duplicate_recognition-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: duplicate_recognition-0.0.8.dist-info/licenses/LICENSE
+Filename: duplicate_recognition-0.0.9.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: duplicate_recognition-0.0.8.dist-info/RECORD
+Filename: duplicate_recognition-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## duplicate_recognition/__init__.py

```diff
@@ -1,6 +1,6 @@
-from .utils import Algorithm, Comparison
-from .entity_algorithm import DuplicateRecognition
+from .utils import Algorithm
+from .entity_algorithm import DuplicateRecognition, Comparison
 from .statistics import STATISTICS
 
 
-__all__ = ["Algorithm", "Comparison", "DuplicateRecognition", "STATISTICS"]
+__all__ = ["Algorithm", "DuplicateRecognition", "STATISTICS"]
```

## duplicate_recognition/entity_algorithm.py

```diff
@@ -1,15 +1,18 @@
+from __future__ import annotations
+
 import logging
 from collections import defaultdict
+from dataclasses import dataclass, field
 from functools import lru_cache
 from typing import Generator, Tuple, Set, List, Dict, Any
 from typing import Optional
 
 from .field_algorythm import compare_fields
-from .utils import Comparison, Algorithm
+from .utils import Algorithm
 from .statistics import STATISTICS, clear_stats
 
 
 class EntityDict(dict):
     # https://stackoverflow.com/a/6229253/16804841
     def __init__(self, entity_generator: Generator[Tuple[int, Dict[str, Any]], None, None], *args, **kwargs):
         self.entity_generator = entity_generator
@@ -19,37 +22,80 @@
         for entity_id, entity in self.entity_generator:
             self[entity_id] = entity
             if entity_id == key:
                 return entity
         return key
 
 
+@dataclass
+class Comparison:
+    duplicate_recognition: DuplicateRecognition
+    entity: Dict[str, Any]
+    other_entity: Dict[str, Any]
+
+    field_scores: Dict[str, float] = field(default_factory=dict)
+    f_score_sum: float = 0
+    count: int = 0
+
+    score: float = 0
+
+    @property
+    @lru_cache()
+    def pair(self) -> Tuple[int, int]:
+        _entity = super().__getattribute__("entity")
+        _other_entity = super().__getattribute__("other_entity")
+        _id_column = super().__getattribute__("duplicate_recognition").ID_COLUMN
+
+        return _entity[_id_column], _other_entity[_id_column]
+
+    def __hash__(self):
+        _entity = super().__getattribute__("entity")
+        _other_entity = super().__getattribute__("other_entity")
+        _id_column = super().__getattribute__("duplicate_recognition").ID_COLUMN
+
+        return _entity[_id_column] ^ _other_entity[_id_column]
+
+    def commit(self):
+        a, b = self.pair
+
+        def check_for_best(v: int):
+            _s = self.duplicate_recognition.best_matches.get(v, None)
+            if _s is None or _s.score < self.score:
+                self.duplicate_recognition.best_matches[v] = self
+
+        check_for_best(a)
+        check_for_best(b)
+
+
 class DuplicateRecognition:
     """
     Here are all objects, that are used for dependency injection.
 
     TERMINOLOGY:
     - entity: usually a row in the database (e.g. an exhibitor, or a contact)
     - pair: two entity id, that need to be compared
     - comparison: an entity id (entity) and a list of entity ids (entity_pool), that need to be compared with a
     - uncompared: a list of entity ids, that are not compared yet
     - relevant_entities: all the entities, that need to be compared.
       It doesn't matter in which run (if ran with a limit)
     """
+    THRESHOLD = 0.7
     F_SCORE_FOR_EXACT_MATCH = 10
 
     ID_COLUMN: str = "id"
     F_SCORES: Dict[str, float] = defaultdict(lambda: 0)
     MATCHING_ALGORITHM: Dict[str, Algorithm] = defaultdict(lambda: Algorithm.EQUALITY)
     THRESHOLDS: Dict[str, float] = defaultdict(lambda: 0)
     NEGATIVE_FIELDS: Set[str] = set()
 
     def __init__(self, logger: logging.Logger = None):
         self.kwargs = locals()
 
+        self.best_matches: Dict[int, Comparison] = {}
+
         self.logger = logger or logging.getLogger(f"{self.__class__.__name__}Duplicates")
 
     def get_relevant_entities(self) -> Generator[Dict[str, Any], None, None]:
         yield from ()
 
     def get_refresh_pairs(self) -> Generator[Tuple[int, int], None, None]:
         yield from ()
@@ -60,14 +106,17 @@
     def get_uncompared(self) -> Generator[int, None, None]:
         yield from ()
 
     @STATISTICS.silent_timeit
     def write_comparisons(self, comparisons: Generator[Comparison, None, None]):
         yield from ()
 
+    def write_best_comparisons(self, comparisons: Generator[Tuple[int, int, Comparison], None, None]):
+        yield from ()
+
     @STATISTICS.timeit
     def _map_relevant_entities(self) -> Generator[Tuple[int, Dict[str, Any]], None, None]:
         """
         :return: A dictionary mapping the id of an entity to the entity itself.
 
         This maps the relevant entities.
         """
@@ -169,18 +218,18 @@
     def _compare(self, entity: Dict[str, Any], entity_pool: List[Dict[str, Any]]) -> Generator[Comparison, None, None]:
         """
         :param entity: The entity to compare
         :param entity_pool: The entities to compare the entity with
 
         :return: A list of tuples (entity_id, f_score) representing the matches.
         """
-        best_match: Comparison = Comparison({}, {})
+        best_match: Comparison = Comparison(self, {}, {})
         for other_entity in entity_pool:
             STATISTICS.compared_entity_total += 1
-            comparison = Comparison(entity, other_entity)
+            comparison = Comparison(self, entity, other_entity)
 
             for key in entity.keys():
                 if key not in other_entity:
                     continue
 
                 STATISTICS.compared_field_total += 1
                 a = entity[key]
@@ -200,38 +249,53 @@
 
                 comparison.f_score_sum += f_score
                 comparison.score += temp
                 comparison.count += 1
 
             comparison.score = comparison.score / comparison.count if comparison.count > 0 else 0
 
+            comparison.commit()
             yield comparison
 
             if comparison.score > best_match.score:
                 best_match = comparison
 
         self.logger.debug(f"Comparing {entity[self.ID_COLUMN]} {'(' + entity.get('firma', '') + ')':<50} "
                           f"with {len(entity_pool)} entities. "
                           f"{best_match.score:.2f}: {best_match.other_entity.get('firma', '')}")
 
+    def _get_best_comparison_pairs(self) -> Generator[Tuple[int, int, Comparison], None, None]:
+        for i, comp in self.best_matches.items():
+            _pair = comp.pair
+            j = _pair[1] if _pair[0] == i else _pair[0]
+            yield i, j, comp
+
+
     @STATISTICS.timeit
     def execute(self, limit: Optional[int] = None):
         clear_stats()
         DuplicateRecognition.__init__(**self.kwargs)
 
         def _decrement_limit() -> bool:
             nonlocal limit
             limit -= 1
             return limit < 1
 
         decrement_limit = _decrement_limit if limit is not None else lambda: False
-
         id_to_entity = EntityDict(self._map_relevant_entities())
 
         for _field in self.NEGATIVE_FIELDS:
             self.F_SCORES[_field] = -1 * self.F_SCORES[_field]
 
         for a, existing in self._generate_comparisons():
             self.write_comparisons(self._compare(id_to_entity[a], [id_to_entity[b] for b in existing]))
 
             if decrement_limit():
                 break
+
+        self.write_best_comparisons(self._get_best_comparison_pairs())
+
+
+
+
+    def __del__(self):
+        pass
```

## duplicate_recognition/utils.py

```diff
@@ -1,25 +1,11 @@
-from typing import Dict, Any, Generator, Tuple
 from enum import Enum
-from dataclasses import dataclass, field
 
 
 class Algorithm(Enum):
     EQUALITY = 1
     PHONETIC_DISTANCE = 2
     URL = 3
     COUNTRY = 4
     VAT_ID = 5
     PHONE = 6
     EMAIL = 7
-
-
-@dataclass
-class Comparison:
-    entity: Dict[str, Any]
-    other_entity: Dict[str, Any]
-
-    field_scores: Dict[str, float] = field(default_factory=dict)
-    f_score_sum: float = 0
-    count: int = 0
-
-    score: float = 0
```

## Comparing `duplicate_recognition-0.0.8.dist-info/METADATA` & `duplicate_recognition-0.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duplicate_recognition
-Version: 0.0.8
+Version: 0.0.9
 Summary: This Project uses the calculation of similarities scores of a set of entities in an edge list. To allow for versatile usage, it uses dependency injection to implement it into any application.
 Project-URL: Homepage, https://github.com/HeIIow2/Duplicate-Recognition
 Project-URL: Issues, https://github.com/HeIIow2/Duplicate-Recognition/issues
 Author-email: Hazel <Hazel.Noack@proton.me>
 License: MIT License
         
         Copyright (c) 2024 _
```

## Comparing `duplicate_recognition-0.0.8.dist-info/licenses/LICENSE` & `duplicate_recognition-0.0.9.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `duplicate_recognition-0.0.8.dist-info/RECORD` & `duplicate_recognition-0.0.9.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-duplicate_recognition/__init__.py,sha256=OvhyotzxytH8eEg45ZpdMsQ6u6yWDpLsqibOtYm9isc,205
-duplicate_recognition/entity_algorithm.py,sha256=Ps8bejpIGK52gXibPtT1EpT4qHiXBY70ZB_6tDocIqg,8467
+duplicate_recognition/__init__.py,sha256=SGEZ5qK38QM7_A_rvD3dV5DiTvAhRwGGR_pyMS9QJBA,191
+duplicate_recognition/entity_algorithm.py,sha256=9Y57vWV2dPBVcjoU2rX2NOOk0ZVClA45DubkZz2iNjk,10371
 duplicate_recognition/field_algorythm.py,sha256=8ittxf3gJvi2aT8A3uoVyqsCS4hftpQOsqLJFUIifk4,4512
 duplicate_recognition/statistics.py,sha256=YCjfuUAPfRRLD1DN22bg59lLscRLutTts6kbt4frJFc,3058
-duplicate_recognition/utils.py,sha256=vKfDJBxhupvk5qoC-9PcHGvm8MEKHHdM_-IGc0xObas,474
-duplicate_recognition-0.0.8.dist-info/METADATA,sha256=Oc5zy0eag7Hq5xexlvpQA-v8MsYLGerp6jbh_lOFFvE,6321
-duplicate_recognition-0.0.8.dist-info/WHEEL,sha256=TJPnKdtrSue7xZ_AVGkp9YXcvDrobsjBds1du3Nx6dc,87
-duplicate_recognition-0.0.8.dist-info/licenses/LICENSE,sha256=Fn-N910XD2VlqttoD73-a8lQqmD7QKqICxD9sL9u0PU,1058
-duplicate_recognition-0.0.8.dist-info/RECORD,,
+duplicate_recognition/utils.py,sha256=ey3YAU_gojssKDFrfdHRjVQ0fJu3DlzYaoC3ud0xjtA,161
+duplicate_recognition-0.0.9.dist-info/METADATA,sha256=moHHtFJrP9rb7E6fvXknBwRYMWkLKzV1RrAwmvgZL_Q,6321
+duplicate_recognition-0.0.9.dist-info/WHEEL,sha256=TJPnKdtrSue7xZ_AVGkp9YXcvDrobsjBds1du3Nx6dc,87
+duplicate_recognition-0.0.9.dist-info/licenses/LICENSE,sha256=Fn-N910XD2VlqttoD73-a8lQqmD7QKqICxD9sL9u0PU,1058
+duplicate_recognition-0.0.9.dist-info/RECORD,,
```

