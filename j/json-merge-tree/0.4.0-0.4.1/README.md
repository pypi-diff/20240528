# Comparing `tmp/json_merge_tree-0.4.0.tar.gz` & `tmp/json_merge_tree-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_merge_tree-0.4.0.tar", max compression
+gzip compressed data, was "json_merge_tree-0.4.1.tar", max compression
```

## Comparing `json_merge_tree-0.4.0.tar` & `json_merge_tree-0.4.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3718 2023-12-18 17:32:30.296169 json_merge_tree-0.4.0/README.md
--rw-r--r--   0        0        0      154 2023-12-18 17:32:30.296169 json_merge_tree-0.4.0/json_merge_tree/__init__.py
--rw-r--r--   0        0        0     4669 2023-12-18 17:32:30.296169 json_merge_tree-0.4.0/json_merge_tree/json_objects.py
--rw-r--r--   0        0        0     3806 2023-12-18 17:32:30.296169 json_merge_tree-0.4.0/json_merge_tree/merged.py
--rw-r--r--   0        0        0      665 2023-12-18 17:32:30.296169 json_merge_tree-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4477 1970-01-01 00:00:00.000000 json_merge_tree-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     3718 2024-05-28 15:08:31.422797 json_merge_tree-0.4.1/README.md
+-rw-r--r--   0        0        0      154 2024-05-28 15:08:31.422797 json_merge_tree-0.4.1/json_merge_tree/__init__.py
+-rw-r--r--   0        0        0     4667 2024-05-28 15:08:31.422797 json_merge_tree-0.4.1/json_merge_tree/json_objects.py
+-rw-r--r--   0        0        0     3806 2024-05-28 15:08:31.422797 json_merge_tree-0.4.1/json_merge_tree/merged.py
+-rw-r--r--   0        0        0      658 2024-05-28 15:08:31.422797 json_merge_tree-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 json_merge_tree-0.4.1/PKG-INFO
```

### Comparing `json_merge_tree-0.4.0/README.md` & `json_merge_tree-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `json_merge_tree-0.4.0/json_merge_tree/json_objects.py` & `json_merge_tree-0.4.1/json_merge_tree/json_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
      at the top.
     """
     c = table.columns
     # These filters will be used to get the resource record here, and also the slug records later
     query_filters: tuple = (c.resource_id == resource_id,)
     if filters is not None:
         query_filters = query_filters + filters
-    query = select([table]).where(*query_filters)
+    query = select(table).where(*query_filters)
     record = get_resource_record(db, query.where(c.slug.is_(None)).order_by(c.created_at))
 
     if parent_getter is not None and getattr(record, 'inherits', True):
         # If this resource isn't the top of the hierarchy, recurse upwards...
         for parent_id, grandparent_getter in parent_getter(resource_id):
             # ...with the parent's ID and a generator of that resource's immediate ancestors
             yield from get_json_objects(db, table, parent_id, json_field, grandparent_getter, slugs,
```

### Comparing `json_merge_tree-0.4.0/json_merge_tree/merged.py` & `json_merge_tree-0.4.1/json_merge_tree/merged.py`

 * *Files identical despite different names*

### Comparing `json_merge_tree-0.4.0/pyproject.toml` & `json_merge_tree-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "json-merge-tree"
-version = "0.4.0"
+version = "0.4.1"
 description = "JSON Merge Tree (built on top of jsonmerge) merges JSON objects in a hierarchy, allowing customization of how objects are merged."
 readme = "README.md"
 license = "MIT"
 authors = ["Marcy Buccellato <mbuccellato@hearst.com>", "Nic Wolff <nwolff@hearst.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 dotty-dict = ">=1.3.0"
 jsonmerge = ">=1.8.0"
-sqlalchemy = ">=1.3.0,<2.0.0"
+sqlalchemy = ">=2.0.0"
 
 [tool.poetry.dev-dependencies]
 coverage = "~=7.3"
 flake8 = "~=5.0.4"
 isort = "~=5.12"
 mypy = "~=1.5"
 pytest = "~=7.1"
```

### Comparing `json_merge_tree-0.4.0/PKG-INFO` & `json_merge_tree-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: json-merge-tree
-Version: 0.4.0
+Version: 0.4.1
 Summary: JSON Merge Tree (built on top of jsonmerge) merges JSON objects in a hierarchy, allowing customization of how objects are merged.
 License: MIT
 Author: Marcy Buccellato
 Author-email: mbuccellato@hearst.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: dotty-dict (>=1.3.0)
 Requires-Dist: jsonmerge (>=1.8.0)
-Requires-Dist: sqlalchemy (>=1.3.0,<2.0.0)
+Requires-Dist: sqlalchemy (>=2.0.0)
 Description-Content-Type: text/markdown
 
 # json-merge-tree
 
 JSON Merge Tree (built on top of [`jsonmerge`](https://github.com/avian2/jsonmerge)) merges JSON objects in a hierarchy, 
 allowing customization of how objects are merged.
```

