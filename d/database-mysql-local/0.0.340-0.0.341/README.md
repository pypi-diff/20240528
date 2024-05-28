# Comparing `tmp/database_mysql_local-0.0.340.tar.gz` & `tmp/database_mysql_local-0.0.341.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.340.tar", last modified: Sun May 26 14:54:39 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.341.tar", last modified: Tue May 28 16:25:03 2024, max compression
```

## Comparing `database_mysql_local-0.0.340.tar` & `database_mysql_local-0.0.341.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:54:39.410602 database_mysql_local-0.0.340/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 14:53:41.000000 database_mysql_local-0.0.340/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 14:54:39.410602 database_mysql_local-0.0.340/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-26 14:53:41.000000 database_mysql_local-0.0.340/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:54:39.406602 database_mysql_local-0.0.340/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:54:39.410602 database_mysql_local-0.0.340/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 14:53:41.000000 database_mysql_local-0.0.340/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-26 14:53:41.000000 database_mysql_local-0.0.340/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-26 14:53:41.000000 database_mysql_local-0.0.340/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-26 14:53:41.000000 database_mysql_local-0.0.340/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-26 14:53:41.000000 database_mysql_local-0.0.340/database_mysql_local/src/generate_table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)    56809 2024-05-26 14:53:41.000000 database_mysql_local-0.0.340/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    31229 2024-05-26 14:53:41.000000 database_mysql_local-0.0.340/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-05-26 14:53:41.000000 database_mysql_local-0.0.340/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-26 14:53:41.000000 database_mysql_local-0.0.340/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-26 14:53:41.000000 database_mysql_local-0.0.340/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-26 14:53:41.000000 database_mysql_local-0.0.340/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   243072 2024-05-26 14:53:41.000000 database_mysql_local-0.0.340/database_mysql_local/src/table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)   652104 2024-05-26 14:54:07.000000 database_mysql_local-0.0.340/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-26 14:53:41.000000 database_mysql_local-0.0.340/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     9554 2024-05-26 14:53:41.000000 database_mysql_local-0.0.340/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 14:54:39.410602 database_mysql_local-0.0.340/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-26 14:54:39.000000 database_mysql_local-0.0.340/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-26 14:54:39.000000 database_mysql_local-0.0.340/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 14:54:39.000000 database_mysql_local-0.0.340/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-26 14:54:39.000000 database_mysql_local-0.0.340/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 14:54:39.000000 database_mysql_local-0.0.340/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-26 14:53:50.000000 database_mysql_local-0.0.340/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 14:54:39.410602 database_mysql_local-0.0.340/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-26 14:53:41.000000 database_mysql_local-0.0.340/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:25:03.871961 database_mysql_local-0.0.341/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:24:01.000000 database_mysql_local-0.0.341/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-28 16:25:03.871961 database_mysql_local-0.0.341/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-28 16:24:01.000000 database_mysql_local-0.0.341/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:25:03.867962 database_mysql_local-0.0.341/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:25:03.871961 database_mysql_local-0.0.341/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 16:24:01.000000 database_mysql_local-0.0.341/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-28 16:24:01.000000 database_mysql_local-0.0.341/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-28 16:24:01.000000 database_mysql_local-0.0.341/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-28 16:24:01.000000 database_mysql_local-0.0.341/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-28 16:24:01.000000 database_mysql_local-0.0.341/database_mysql_local/src/generate_table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58532 2024-05-28 16:24:01.000000 database_mysql_local-0.0.341/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31229 2024-05-28 16:24:01.000000 database_mysql_local-0.0.341/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-05-28 16:24:01.000000 database_mysql_local-0.0.341/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-28 16:24:01.000000 database_mysql_local-0.0.341/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-28 16:24:01.000000 database_mysql_local-0.0.341/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-05-28 16:24:01.000000 database_mysql_local-0.0.341/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   243072 2024-05-28 16:24:01.000000 database_mysql_local-0.0.341/database_mysql_local/src/table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   652104 2024-05-28 16:24:27.000000 database_mysql_local-0.0.341/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-28 16:24:01.000000 database_mysql_local-0.0.341/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9554 2024-05-28 16:24:01.000000 database_mysql_local-0.0.341/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:25:03.871961 database_mysql_local-0.0.341/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-28 16:25:03.000000 database_mysql_local-0.0.341/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-28 16:25:03.000000 database_mysql_local-0.0.341/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 16:25:03.000000 database_mysql_local-0.0.341/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-28 16:25:03.000000 database_mysql_local-0.0.341/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 16:25:03.000000 database_mysql_local-0.0.341/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-28 16:24:09.000000 database_mysql_local-0.0.341/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 16:25:03.871961 database_mysql_local-0.0.341/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-28 16:24:01.000000 database_mysql_local-0.0.341/setup.py
```

### Comparing `database_mysql_local-0.0.340/PKG-INFO` & `database_mysql_local-0.0.341/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.340
+Version: 0.0.341
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.340/README.md` & `database_mysql_local-0.0.341/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.340/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.341/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.340/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.341/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.340/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.341/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.340/database_mysql_local/src/generate_table_columns.py` & `database_mysql_local-0.0.341/database_mysql_local/src/generate_table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.340/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.341/database_mysql_local/src/generic_crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,14 +123,42 @@
                 inserted_id = self._get_existing_duplicate_id(schema_name, table_name, exception)
             else:
                 raise exception
         finally:
             self.logger.debug(object=locals())
         return inserted_id
 
+    def insert_if_not_exists(self, *, schema_name: str = None, table_name: str = None, data_dict: dict = None,
+                             data_dict_compare: dict = None, view_table_name: str = None,
+                             commit_changes: bool = True, compare_with_or: bool = False) -> int:
+        """Inserts a new row into the table if a row with the same values does not exist,
+        and returns the id of the new row or None if an error occurred."""
+        schema_name = schema_name or self.default_schema_name
+        table_name = table_name or self.default_table_name
+        view_table_name = view_table_name or self.default_view_table_name
+        data_dict_compare = data_dict_compare or data_dict
+        self._validate_args(args=locals())
+
+        # Try to select
+        where_clause, params = process_upsert_data_dict(data_dict=data_dict_compare, compare_with_or=compare_with_or)
+        row_tuple = self.select_one_tuple_by_where(
+            schema_name=schema_name, view_table_name=view_table_name, select_clause_value="*",
+            where=where_clause, params=params)
+        if row_tuple:
+            entity_id = row_tuple[0]
+            self.logger.info(f"GenericCRUD.insert_if_not_exists: row already exists, returning id {entity_id}",
+                             object={"id": entity_id})
+            return entity_id
+        else:
+            entity_id = self.insert(schema_name=schema_name, table_name=table_name, data_dict=data_dict,
+                                    commit_changes=commit_changes)
+            self.logger.info(f"GenericCRUD.insert_if_not_exists: row inserted with id {entity_id}",
+                             object={"id": entity_id})
+            return entity_id
+
     def insert_many_dicts(self, *, schema_name: str = None, table_name: str = None, data_dicts: list[dict],
                           commit_changes: bool = True) -> int:
         """Inserts multiple rows into the table.
         data_dicts should be in the following format: [{col1: val1, col2: val2}, {col1: val3, col2: val4}, ...]
         Returns the number of inserted rows.
         """
         if not data_dicts:
```

### Comparing `database_mysql_local-0.0.340/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.341/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.340/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.341/database_mysql_local/src/generic_mapping.py`

 * *Files 20% similar despite different names*

```diff
@@ -46,14 +46,69 @@
         data_dict = data_dict or {}
         data_dict[f"{entity_name1}_id"] = entity_id1
         data_dict[f"{entity_name2}_id"] = entity_id2
         mapping_id = super().insert(schema_name=schema_name, data_dict=data_dict, table_name=table_name,
                                     ignore_duplicate=ignore_duplicate)
         return mapping_id
 
+    def insert_mapping_if_not_exists(self, *, entity_id1: int, entity_id2: int,
+                                     entity_name1: str = None, entity_name2: str = None,
+                                     schema_name: str = None, data_dict: dict = None) -> int:
+        """Inserts a new link between two entities if it does not exist and returns the id of the
+            new row or -1 if an error occurred.
+        :param entity_name1: The name of the first entity's table.
+        :param entity_name2: The name of the second entity's table.
+        :param entity_id1: The id of the first entity.
+        :param entity_id2: The id of the second entity.
+        :param schema_name: The name of the schema.
+        :param data_dict: The data to insert.
+        :return: The id of the new row or -1 if an error occurred.
+        """
+        data_dict = data_dict or {}
+        entity_name1 = entity_name1 or self.default_entity_name1
+        entity_name2 = entity_name2 or self.default_entity_name2
+        schema_name = schema_name or self.default_schema_name
+        table_name = f"{entity_name1}_{entity_name2}_table"
+        data_dict[f"{entity_name1}_id"] = entity_id1
+        data_dict[f"{entity_name2}_id"] = entity_id2
+        data_dict_compare = {
+            f"{entity_name1}_id": entity_id1,
+            f"{entity_name2}_id": entity_id2
+        }
+        mapping_id = super().insert_if_not_exists(schema_name=schema_name, data_dict=data_dict, table_name=table_name,
+                                                  data_dict_compare=data_dict_compare)
+        return mapping_id
+
+
+    def upsert_mapping(self, *, entity_id1: int, entity_id2: int,
+                       entity_name1: str = None, entity_name2: str = None,
+                       schema_name: str = None, data_dict: dict = None,
+                       data_dict_compare: dict = None) -> int:
+        """Inserts a new link between two entities and returns the id of the
+            new row or -1 if an error occurred.
+        :param entity_name1: The name of the first entity's table.
+        :param entity_name2: The name of the second entity's table.
+        :param entity_id1: The id of the first entity.
+        :param entity_id2: The id of the second entity.
+        :param schema_name: The name of the schema.
+        :param data_dict: The data to insert.
+        :return: The id of the new row or -1 if an error occurred.
+        """
+        data_dict = data_dict or {}
+        data_dict_compare = data_dict_compare or {}
+        entity_name1 = entity_name1 or self.default_entity_name1
+        entity_name2 = entity_name2 or self.default_entity_name2
+        schema_name = schema_name or self.default_schema_name
+        table_name = f"{entity_name1}_{entity_name2}_table"
+        data_dict_compare[f"{entity_name1}_id"] = data_dict[f"{entity_name1}_id"] = entity_id1
+        data_dict_compare[f"{entity_name2}_id"] = data_dict[f"{entity_name2}_id"] = entity_id2
+        mapping_id = super().upsert(schema_name=schema_name, data_dict=data_dict, table_name=table_name)
+        return mapping_id
+
+
     # TODO: do we need delete_mapping_by_id?
     def delete_mapping_by_two_ids(self, *, entity_id1: int, entity_id2: int,
                                   entity_name1: str = None, entity_name2: str = None,
                                   schema_name: str = None) -> None:
         """ Deletes a link between two entities.
         :param entity_name1: The name of the first entity's table.
         :param entity_name2: The name of the second entity's table.
```

### Comparing `database_mysql_local-0.0.340/database_mysql_local/src/point.py` & `database_mysql_local-0.0.341/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.340/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.341/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.340/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.341/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.340/database_mysql_local/src/table_columns.py` & `database_mysql_local-0.0.341/database_mysql_local/src/table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.340/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.341/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.340/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.341/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.340/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.341/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.340/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.341/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.340
+Version: 0.0.341
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.340/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.341/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.340/pyproject.toml` & `database_mysql_local-0.0.341/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "database-mysql-local"
-version = "0.0.341" # https://pypi.org/project/database-mysql-local
+version = "0.0.342" # https://pypi.org/project/database-mysql-local
 description = "database-mysql-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
 
 # dephell deps convert --from pyproject.toml --from-format poetry --to setup.py --to-format setuppy
```

### Comparing `database_mysql_local-0.0.340/setup.py` & `database_mysql_local-0.0.341/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.340',
+    version='0.0.341',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

