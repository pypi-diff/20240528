# Comparing `tmp/hermitage_alchemy-0.2.4.tar.gz` & `tmp/hermitage_alchemy-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermitage_alchemy-0.2.4.tar", max compression
+gzip compressed data, was "hermitage_alchemy-0.2.5.tar", max compression
```

## Comparing `hermitage_alchemy-0.2.4.tar` & `hermitage_alchemy-0.2.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      120 2024-04-15 11:40:18.155284 hermitage_alchemy-0.2.4/README.md
--rw-r--r--   0        0        0      504 2024-05-25 14:24:50.954908 hermitage_alchemy-0.2.4/hermitage_alchemy/__init__.py
--rw-r--r--   0        0        0    10439 2024-05-27 14:15:43.102033 hermitage_alchemy-0.2.4/hermitage_alchemy/assembling.py
--rw-r--r--   0        0        0      826 2024-04-13 14:00:09.650913 hermitage_alchemy-0.2.4/hermitage_alchemy/bootstraping.py
--rw-r--r--   0        0        0     6852 2024-05-25 14:24:50.956155 hermitage_alchemy-0.2.4/hermitage_alchemy/configuration.py
--rw-r--r--   0        0        0       24 2024-05-25 14:24:50.956586 hermitage_alchemy-0.2.4/hermitage_alchemy/definition/__init__.py
--rw-r--r--   0        0        0      718 2024-05-26 13:12:45.022518 hermitage_alchemy-0.2.4/hermitage_alchemy/definition/contracts.py
--rw-r--r--   0        0        0       60 2024-05-25 14:24:50.957143 hermitage_alchemy-0.2.4/hermitage_alchemy/execution/__init__.py
--rw-r--r--   0        0        0     6991 2024-05-25 14:24:50.957364 hermitage_alchemy-0.2.4/hermitage_alchemy/execution/read.py
--rw-r--r--   0        0        0     1840 2024-05-27 17:39:40.830848 hermitage_alchemy-0.2.4/hermitage_alchemy/execution/write.py
--rw-r--r--   0        0        0      415 2024-05-27 17:39:45.580692 hermitage_alchemy-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 hermitage_alchemy-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      120 2024-04-15 11:40:18.155284 hermitage_alchemy-0.2.5/README.md
+-rw-r--r--   0        0        0      504 2024-05-25 14:24:50.954908 hermitage_alchemy-0.2.5/hermitage_alchemy/__init__.py
+-rw-r--r--   0        0        0    10439 2024-05-27 14:15:43.102033 hermitage_alchemy-0.2.5/hermitage_alchemy/assembling.py
+-rw-r--r--   0        0        0      826 2024-04-13 14:00:09.650913 hermitage_alchemy-0.2.5/hermitage_alchemy/bootstraping.py
+-rw-r--r--   0        0        0     7409 2024-05-27 18:32:27.541366 hermitage_alchemy-0.2.5/hermitage_alchemy/configuration.py
+-rw-r--r--   0        0        0       24 2024-05-25 14:24:50.956586 hermitage_alchemy-0.2.5/hermitage_alchemy/definition/__init__.py
+-rw-r--r--   0        0        0      718 2024-05-26 13:12:45.022518 hermitage_alchemy-0.2.5/hermitage_alchemy/definition/contracts.py
+-rw-r--r--   0        0        0       60 2024-05-25 14:24:50.957143 hermitage_alchemy-0.2.5/hermitage_alchemy/execution/__init__.py
+-rw-r--r--   0        0        0     6991 2024-05-25 14:24:50.957364 hermitage_alchemy-0.2.5/hermitage_alchemy/execution/read.py
+-rw-r--r--   0        0        0     1840 2024-05-27 17:39:40.830848 hermitage_alchemy-0.2.5/hermitage_alchemy/execution/write.py
+-rw-r--r--   0        0        0      415 2024-05-27 18:33:33.512379 hermitage_alchemy-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 hermitage_alchemy-0.2.5/PKG-INFO
```

### Comparing `hermitage_alchemy-0.2.4/hermitage_alchemy/assembling.py` & `hermitage_alchemy-0.2.5/hermitage_alchemy/assembling.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.2.4/hermitage_alchemy/bootstraping.py` & `hermitage_alchemy-0.2.5/hermitage_alchemy/bootstraping.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.2.4/hermitage_alchemy/configuration.py` & `hermitage_alchemy-0.2.5/hermitage_alchemy/configuration.py`

 * *Files 9% similar despite different names*

```diff
@@ -125,20 +125,22 @@
             other.qua is None or f'{other.qua}_id' == self.parent_address.name
         )
 
 
 class Schema:
     def __init__(
         self,
-        tables: collections.abc.Iterable[sqlalchemy.Table]
+        tables: collections.abc.Iterable[sqlalchemy.Table],
+        *foreign_keys: tuple[sqlalchemy.Column, sqlalchemy.Column]
     ):
         self._graph = collections.defaultdict(set)
         self._tables = {}
         self._cache = {}
         self._index_tables(tables)
+        self._index_custom_foreign_keys(*foreign_keys)
 
     def get_link(
         self,
         source_space: Space,
         target_space: Space
     ):
         link = self._get_m2o(source_space, target_space)
@@ -183,14 +185,23 @@
                 self._graph[fk.parent.table.name].add(
                     Fk(
                         target_address=Address(name=fk.column.name, space=Space(fk.column.table.name)),
                         parent_address=Address(name=fk.parent.name, space=Space(fk.parent.table.name))
                     )
                 )
 
+    def _index_custom_foreign_keys(self, *foreign_keys: tuple[sqlalchemy.Column, sqlalchemy.Column]):
+        for parent, target in foreign_keys:
+            self._graph[parent.table.name].add(
+                Fk(
+                    parent_address=Address(name=parent.name, space=Space(parent.table.name)),
+                    target_address=Address(name=target.name, space=Space(target.table.name))
+                )
+            )
+
     def _get_m2o(
         self,
         source_space: Space,
         target_space: Space
     ) -> M2O | None:
         for t, fks in self._graph.items():
             if source_space.last == t:
```

### Comparing `hermitage_alchemy-0.2.4/hermitage_alchemy/definition/contracts.py` & `hermitage_alchemy-0.2.5/hermitage_alchemy/definition/contracts.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.2.4/hermitage_alchemy/execution/read.py` & `hermitage_alchemy-0.2.5/hermitage_alchemy/execution/read.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.2.4/hermitage_alchemy/execution/write.py` & `hermitage_alchemy-0.2.5/hermitage_alchemy/execution/write.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.2.4/PKG-INFO` & `hermitage_alchemy-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hermitage-alchemy
-Version: 0.2.4
+Version: 0.2.5
 Summary: Implementation of hermitage contracts for sqlalchemy engine
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

