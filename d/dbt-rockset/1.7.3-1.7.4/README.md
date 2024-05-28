# Comparing `tmp/dbt_rockset-1.7.3.tar.gz` & `tmp/dbt_rockset-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_rockset-1.7.3.tar", last modified: Tue Apr 23 17:41:15 2024, max compression
+gzip compressed data, was "dbt_rockset-1.7.4.tar", last modified: Tue May 28 18:48:32 2024, max compression
```

## Comparing `dbt_rockset-1.7.3.tar` & `dbt_rockset-1.7.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-04-23 17:41:15.935008 dbt_rockset-1.7.3/
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)       47 2024-03-22 21:23:22.000000 dbt_rockset-1.7.3/MANIFEST.in
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)      315 2024-04-23 17:41:15.935008 dbt_rockset-1.7.3/PKG-INFO
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)    11253 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/README.md
-drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-04-23 17:41:15.923008 dbt_rockset-1.7.3/dbt/
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)       65 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/dbt/__init__.py
-drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-04-23 17:41:15.923008 dbt_rockset-1.7.3/dbt/adapters/
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)       65 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/dbt/adapters/__init__.py
-drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-04-23 17:41:15.927008 dbt_rockset-1.7.3/dbt/adapters/rockset/
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)      507 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/dbt/adapters/rockset/__init__.py
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)       18 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/dbt/adapters/rockset/__version__.py
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)      694 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/dbt/adapters/rockset/column.py
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)     4653 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/dbt/adapters/rockset/connections.py
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)    37792 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/dbt/adapters/rockset/impl.py
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)     1157 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/dbt/adapters/rockset/relation.py
-drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-04-23 17:41:15.927008 dbt_rockset-1.7.3/dbt/include/
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)       65 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/dbt/include/__init__.py
-drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-04-23 17:41:15.927008 dbt_rockset-1.7.3/dbt/include/rockset/
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)       52 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/dbt/include/rockset/__init__.py
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)       91 2024-01-12 19:22:23.000000 dbt_rockset-1.7.3/dbt/include/rockset/dbt_project.yml
-drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-04-23 17:41:15.931008 dbt_rockset-1.7.3/dbt/include/rockset/macros/
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)      132 2024-01-12 19:22:23.000000 dbt_rockset-1.7.3/dbt/include/rockset/macros/catalog.sql
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)       82 2024-03-22 21:23:22.000000 dbt_rockset-1.7.3/dbt/include/rockset/macros/current_ts.sql
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)      475 2024-03-22 21:23:22.000000 dbt_rockset-1.7.3/dbt/include/rockset/macros/macros.sql
-drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-04-23 17:41:15.931008 dbt_rockset-1.7.3/dbt/include/rockset/macros/materializations/
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)     1040 2024-03-22 21:23:22.000000 dbt_rockset-1.7.3/dbt/include/rockset/macros/materializations/incremental.sql
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)      664 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/dbt/include/rockset/macros/materializations/query_lambda.sql
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)     1605 2024-03-22 21:23:22.000000 dbt_rockset-1.7.3/dbt/include/rockset/macros/materializations/seed.sql
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)      658 2024-03-22 21:23:22.000000 dbt_rockset-1.7.3/dbt/include/rockset/macros/materializations/table.sql
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)      934 2024-03-22 21:23:22.000000 dbt_rockset-1.7.3/dbt/include/rockset/macros/materializations/view.sql
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)      463 2024-03-22 21:23:22.000000 dbt_rockset-1.7.3/dbt/include/rockset/profile_template.yml
-drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-04-23 17:41:15.935008 dbt_rockset-1.7.3/dbt_rockset.egg-info/
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)      315 2024-04-23 17:41:15.000000 dbt_rockset-1.7.3/dbt_rockset.egg-info/PKG-INFO
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)      976 2024-04-23 17:41:15.000000 dbt_rockset-1.7.3/dbt_rockset.egg-info/SOURCES.txt
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)        1 2024-04-23 17:41:15.000000 dbt_rockset-1.7.3/dbt_rockset.egg-info/dependency_links.txt
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)       42 2024-04-23 17:41:15.000000 dbt_rockset-1.7.3/dbt_rockset.egg-info/requires.txt
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)        4 2024-04-23 17:41:15.000000 dbt_rockset-1.7.3/dbt_rockset.egg-info/top_level.txt
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)       38 2024-04-23 17:41:15.935008 dbt_rockset-1.7.3/setup.cfg
--rw-r--r--   0 sbaldwin (10051) rockset  (10000)      668 2024-04-23 17:40:35.000000 dbt_rockset-1.7.3/setup.py
+drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-05-28 18:48:32.569880 dbt_rockset-1.7.4/
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)       47 2024-03-22 21:23:22.000000 dbt_rockset-1.7.4/MANIFEST.in
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)      343 2024-05-28 18:48:32.565880 dbt_rockset-1.7.4/PKG-INFO
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)    12023 2024-05-23 23:04:49.000000 dbt_rockset-1.7.4/README.md
+drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-05-28 18:48:32.557880 dbt_rockset-1.7.4/dbt/
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)       65 2024-04-23 17:40:35.000000 dbt_rockset-1.7.4/dbt/__init__.py
+drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-05-28 18:48:32.557880 dbt_rockset-1.7.4/dbt/adapters/
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)       65 2024-04-23 17:40:35.000000 dbt_rockset-1.7.4/dbt/adapters/__init__.py
+drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-05-28 18:48:32.561880 dbt_rockset-1.7.4/dbt/adapters/rockset/
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)      507 2024-04-23 17:40:35.000000 dbt_rockset-1.7.4/dbt/adapters/rockset/__init__.py
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)       18 2024-05-28 18:45:50.000000 dbt_rockset-1.7.4/dbt/adapters/rockset/__version__.py
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)      694 2024-04-23 17:40:35.000000 dbt_rockset-1.7.4/dbt/adapters/rockset/column.py
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)     4653 2024-04-23 17:40:35.000000 dbt_rockset-1.7.4/dbt/adapters/rockset/connections.py
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)    38108 2024-05-28 18:45:50.000000 dbt_rockset-1.7.4/dbt/adapters/rockset/impl.py
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)     1157 2024-04-23 17:40:35.000000 dbt_rockset-1.7.4/dbt/adapters/rockset/relation.py
+drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-05-28 18:48:32.561880 dbt_rockset-1.7.4/dbt/include/
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)       65 2024-04-23 17:40:35.000000 dbt_rockset-1.7.4/dbt/include/__init__.py
+drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-05-28 18:48:32.561880 dbt_rockset-1.7.4/dbt/include/rockset/
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)       52 2024-04-23 17:40:35.000000 dbt_rockset-1.7.4/dbt/include/rockset/__init__.py
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)       91 2024-01-12 19:22:23.000000 dbt_rockset-1.7.4/dbt/include/rockset/dbt_project.yml
+drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-05-28 18:48:32.565880 dbt_rockset-1.7.4/dbt/include/rockset/macros/
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)      132 2024-01-12 19:22:23.000000 dbt_rockset-1.7.4/dbt/include/rockset/macros/catalog.sql
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)       82 2024-03-22 21:23:22.000000 dbt_rockset-1.7.4/dbt/include/rockset/macros/current_ts.sql
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)      475 2024-03-22 21:23:22.000000 dbt_rockset-1.7.4/dbt/include/rockset/macros/macros.sql
+drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-05-28 18:48:32.565880 dbt_rockset-1.7.4/dbt/include/rockset/macros/materializations/
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)     1040 2024-03-22 21:23:22.000000 dbt_rockset-1.7.4/dbt/include/rockset/macros/materializations/incremental.sql
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)      664 2024-04-23 17:40:35.000000 dbt_rockset-1.7.4/dbt/include/rockset/macros/materializations/query_lambda.sql
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)     1605 2024-03-22 21:23:22.000000 dbt_rockset-1.7.4/dbt/include/rockset/macros/materializations/seed.sql
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)      658 2024-03-22 21:23:22.000000 dbt_rockset-1.7.4/dbt/include/rockset/macros/materializations/table.sql
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)      934 2024-03-22 21:23:22.000000 dbt_rockset-1.7.4/dbt/include/rockset/macros/materializations/view.sql
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)      463 2024-03-22 21:23:22.000000 dbt_rockset-1.7.4/dbt/include/rockset/profile_template.yml
+drwxr-xr-x   0 sbaldwin (10051) rockset  (10000)        0 2024-05-28 18:48:32.565880 dbt_rockset-1.7.4/dbt_rockset.egg-info/
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)      343 2024-05-28 18:48:32.000000 dbt_rockset-1.7.4/dbt_rockset.egg-info/PKG-INFO
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)      976 2024-05-28 18:48:32.000000 dbt_rockset-1.7.4/dbt_rockset.egg-info/SOURCES.txt
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)        1 2024-05-28 18:48:32.000000 dbt_rockset-1.7.4/dbt_rockset.egg-info/dependency_links.txt
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)       55 2024-05-28 18:48:32.000000 dbt_rockset-1.7.4/dbt_rockset.egg-info/requires.txt
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)        4 2024-05-28 18:48:32.000000 dbt_rockset-1.7.4/dbt_rockset.egg-info/top_level.txt
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)       38 2024-05-28 18:48:32.569880 dbt_rockset-1.7.4/setup.cfg
+-rw-r--r--   0 sbaldwin (10051) rockset  (10000)      684 2024-05-28 18:45:50.000000 dbt_rockset-1.7.4/setup.py
```

### Comparing `dbt_rockset-1.7.3/README.md` & `dbt_rockset-1.7.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,39 @@
 Type | Supported? | Details
 -----|------------|----------------
 [Table](https://docs.getdbt.com/docs/building-a-dbt-project/building-models/materializations#table) | YES | Creates a [Rockset collection](https://docs.rockset.com/collections/).
 [View](https://docs.getdbt.com/docs/building-a-dbt-project/building-models/materializations#view) | YES | Creates a [Rockset view](https://rockset.com/docs/views/#gatsby-focus-wrapper).
 [Ephemeral](https://docs.getdbt.com/docs/building-a-dbt-project/building-models/materializations#ephemeral) | Yes | Create a CTE.
 [Incremental](https://docs.getdbt.com/docs/building-a-dbt-project/building-models/materializations#incremental) | YES | Creates a [Rockset collection](https://docs.rockset.com/collections/) if it doesn't exist, and writes to it.
 
-Query Lambda can be created and updated using dbt. See the tests for an example usage.
+### Query Lambda Configuration
+[Query Lambdas](https://docs.rockset.com/documentation/docs/query-lambdas) can be created and updated using dbt. 
+To manage a Query Lamdba using dbt, a materialization of 'query_lambda' should be used.
+For example,
+```
+{{
+    config(
+        materialized='query_lambda',
+        tags=['example_tag'],
+        parameters=[
+            {'name': 'order_id', 'type': 'string', 'value': 'xyz'},
+            {'name': 'limit', 'type': 'int', 'value': '10'},
+        ]
+    )
+}}
+
+select * from {{ ref('orders') }} 
+where order_id = :order_id
+order by order_time
+limit :limit
+```
+
+See the [tests](https://github.com/rockset/dbt-rockset/blob/master/tests/functional/adapter/test_query_lambda.py) for more example usages.
+
+>:warning: Query Lambdas cannot be referenced as a model in other dbt models as they cannot be executed from dbt. 
 
 ## Real-Time Streaming ELT Using dbt + Rockset
 
 As data is ingested, Rockset performs the following:
 * The data is automatically indexed in at least three different ways using Rockset’s [Converged Index™](https://rockset.com/blog/converged-indexing-the-secret-sauce-behind-rocksets-fast-queries/) technology.
 * Your write-time data transformations are performed.
 * The data is made available for queries within seconds.
```

### Comparing `dbt_rockset-1.7.3/dbt/adapters/rockset/column.py` & `dbt_rockset-1.7.4/dbt/adapters/rockset/column.py`

 * *Files identical despite different names*

### Comparing `dbt_rockset-1.7.3/dbt/adapters/rockset/connections.py` & `dbt_rockset-1.7.4/dbt/adapters/rockset/connections.py`

 * *Files identical despite different names*

### Comparing `dbt_rockset-1.7.3/dbt/adapters/rockset/impl.py` & `dbt_rockset-1.7.4/dbt/adapters/rockset/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import agate
 import datetime
 import dbt
 import json
 import collections
 import requests
 import rockset
+import backoff
 from rockset.models import *
 from rockset import ApiException
 from decimal import Decimal
 from time import sleep
 from typing import List, Optional, Set
 
 
@@ -28,14 +29,21 @@
 ASYNC_OPTIONS = {
     "client_timeout_ms": 1000,  # arbitrary
     "timeout_ms": 1800000,
     "max_initial_results": 1,
 }
 
 
+def fatal_code(e: ApiException):
+    if e.status == 429:
+        return False
+    else:
+        return 400 <= e.status < 500
+
+
 class RocksetAdapter(BaseAdapter):
     RELATION_TYPES = {
         "TABLE": RelationType.Table,
     }
 
     Relation = RocksetRelation
     Column = RocksetColumn
@@ -376,14 +384,15 @@
 
     @available.parse(lambda *a, **k: "")
     def apply_snapshot(self, relation, sql):
         raise dbt.exceptions.Exception("Snapshots unsupported")
 
     # Query Lambda materialization
     @available.parse(lambda *a, **k: "")
+    @backoff.on_exception(backoff.expo, ApiException, max_tries=20, giveup=fatal_code)
     def create_or_update_query_lambda(self, relation, sql, tags, parameters):
         ws = relation.schema
         name = relation.identifier
         # Ensure workspace exists
         self.create_schema(relation)
 
         if self._query_lambda_exists(ws, name):
@@ -724,14 +733,15 @@
 
             if wait_until_deleted:
                 self._wait_until_collection_deleted(ws, cname)
         except Exception as e:
             if hasattr(e, "status") and e.status != NOT_FOUND:
                 raise e  # Unexpected error
 
+    @backoff.on_exception(backoff.expo, ApiException, max_tries=20, giveup=fatal_code)
     def _delete_ql(self, ws, ql):
         rs = self._rs_client()
         try:
             rs.QueryLambdas.delete_query_lambda(query_lambda=ql, workspace=ws)
             self._wait_until_ql_deleted(ws, ql)
         except Exception as e:
             if hasattr(e, "status") and e.status != NOT_FOUND:
```

### Comparing `dbt_rockset-1.7.3/dbt/adapters/rockset/relation.py` & `dbt_rockset-1.7.4/dbt/adapters/rockset/relation.py`

 * *Files identical despite different names*

### Comparing `dbt_rockset-1.7.3/dbt/include/rockset/macros/materializations/incremental.sql` & `dbt_rockset-1.7.4/dbt/include/rockset/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_rockset-1.7.3/dbt/include/rockset/macros/materializations/query_lambda.sql` & `dbt_rockset-1.7.4/dbt/include/rockset/macros/materializations/query_lambda.sql`

 * *Files identical despite different names*

### Comparing `dbt_rockset-1.7.3/dbt/include/rockset/macros/materializations/seed.sql` & `dbt_rockset-1.7.4/dbt/include/rockset/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt_rockset-1.7.3/dbt/include/rockset/macros/materializations/table.sql` & `dbt_rockset-1.7.4/dbt/include/rockset/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_rockset-1.7.3/dbt/include/rockset/macros/materializations/view.sql` & `dbt_rockset-1.7.4/dbt/include/rockset/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt_rockset-1.7.3/dbt_rockset.egg-info/SOURCES.txt` & `dbt_rockset-1.7.4/dbt_rockset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt_rockset-1.7.3/setup.py` & `dbt_rockset-1.7.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python
 from setuptools import find_namespace_packages, setup
 
 package_name = "dbt-rockset"
 # make sure this always matches dbt/adapters/{adapter}/__version__.py
-package_version = "1.7.3"
+package_version = "1.7.4"
 description = """The Rockset adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
     long_description=description,
     author="Steven Baldwin",
     author_email="sbaldwin@rockset.com",
     url="https://github.com/rockset/dbt-rockset",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
-    install_requires=["dbt-core~=1.7.0", "rockset_sqlalchemy~=0.0.1"],
+    install_requires=["dbt-core~=1.7.0", "rockset_sqlalchemy~=0.0.1", "backoff==2.*"],
 )
```

