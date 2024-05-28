# Comparing `tmp/fastapi_cruddy_framework-1.4.9.tar.gz` & `tmp/fastapi_cruddy_framework-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_cruddy_framework-1.4.9.tar", max compression
+gzip compressed data, was "fastapi_cruddy_framework-1.5.0.tar", max compression
```

## Comparing `fastapi_cruddy_framework-1.4.9.tar` & `fastapi_cruddy_framework-1.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1074 2023-03-03 18:31:12.339513 fastapi_cruddy_framework-1.4.9/LICENSE
--rw-r--r--   0        0        0    54833 2024-05-03 12:50:05.846036 fastapi_cruddy_framework-1.4.9/README.md
--rw-r--r--   0        0        0     2483 2024-03-20 18:15:08.576001 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/__init__.py
--rw-r--r--   0        0        0     6865 2024-05-15 17:30:32.709889 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/adapters.py
--rw-r--r--   0        0        0    44781 2024-04-12 17:41:34.217544 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/controller.py
--rw-r--r--   0        0        0    15521 2024-04-03 20:42:09.978482 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/graphql.py
--rw-r--r--   0        0        0       46 2023-03-03 18:31:12.343965 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/inflector.py
--rw-r--r--   0        0        0     3575 2024-01-06 19:00:34.485202 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/pubsub.py
--rw-r--r--   0        0        0    36269 2024-05-06 18:59:15.284432 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/repository.py
--rw-r--r--   0        0        0    31716 2024-04-10 18:04:33.796733 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/resource.py
--rw-r--r--   0        0        0     2375 2023-10-24 11:53:06.377545 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/router.py
--rw-r--r--   0        0        0     5687 2024-04-03 17:41:13.269559 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/schemas.py
--rw-r--r--   0        0        0    11050 2023-12-12 17:22:31.207802 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/test_helpers.py
--rw-r--r--   0        0        0     8260 2024-04-10 15:33:48.817894 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/util.py
--rw-r--r--   0        0        0    16184 2024-01-30 17:02:35.391956 fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/websocket_manager.py
--rw-r--r--   0        0        0     2252 2024-05-15 17:34:29.752719 fastapi_cruddy_framework-1.4.9/pyproject.toml
--rw-r--r--   0        0        0    56461 1970-01-01 00:00:00.000000 fastapi_cruddy_framework-1.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-03 18:31:12.339513 fastapi_cruddy_framework-1.5.0/LICENSE
+-rw-r--r--   0        0        0    56451 2024-05-28 18:49:51.024376 fastapi_cruddy_framework-1.5.0/README.md
+-rw-r--r--   0        0        0     2508 2024-05-16 15:25:50.903161 fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/__init__.py
+-rw-r--r--   0        0        0     7060 2024-05-28 18:49:51.028803 fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/adapters.py
+-rw-r--r--   0        0        0    45459 2024-05-28 18:49:51.029227 fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/controller.py
+-rw-r--r--   0        0        0    15521 2024-04-03 20:42:09.978482 fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/graphql.py
+-rw-r--r--   0        0        0       46 2023-03-03 18:31:12.343965 fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/inflector.py
+-rw-r--r--   0        0        0     3575 2024-01-06 19:00:34.485202 fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/pubsub.py
+-rw-r--r--   0        0        0    36616 2024-05-28 18:49:51.029757 fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/repository.py
+-rw-r--r--   0        0        0    33952 2024-05-28 18:49:51.030163 fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/resource.py
+-rw-r--r--   0        0        0     2375 2023-10-24 11:53:06.377545 fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/router.py
+-rw-r--r--   0        0        0     6556 2024-05-16 15:28:03.928695 fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/schemas.py
+-rw-r--r--   0        0        0    11050 2023-12-12 17:22:31.207802 fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/test_helpers.py
+-rw-r--r--   0        0        0     8260 2024-04-10 15:33:48.817894 fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/util.py
+-rw-r--r--   0        0        0    16184 2024-01-30 17:02:35.391956 fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/websocket_manager.py
+-rw-r--r--   0        0        0     2252 2024-05-28 18:49:51.031706 fastapi_cruddy_framework-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0    58079 1970-01-01 00:00:00.000000 fastapi_cruddy_framework-1.5.0/PKG-INFO
```

### Comparing `fastapi_cruddy_framework-1.4.9/LICENSE` & `fastapi_cruddy_framework-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.9/README.md` & `fastapi_cruddy_framework-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,15 @@
 PageResponse
 ResponseSchema
 CruddyModel
 CruddyCreatedUpdatedSignature
 CruddyCreatedUpdatedMixin
 CruddyIntIDModel
 CruddyUUIDModel
+CruddyStringIDModel
 SocketMessage
 SocketRoomConfiguration
 ExampleUpdate
 ExampleCreate
 ExampleView
 Example
 # WEBSOCKET MODULES
@@ -445,14 +446,20 @@
 # developercould set disable_update to True, which would cause the resource to abort building a route
 # for PATCH resource/{id}. Be aware of the overall impact of endpoints you totally disable!
 disable_create: bool = False,
 disable_update: bool = False,
 disable_delete: bool = False,
 disable_get_one: bool = False,
 disable_get_many: bool = False,
+# The disable_relationship_getters list allow app developers to instruct the framework to NOT hoist
+# an automatic GET route for a list of specific named relationships. Note, that any relationship name
+# you disable will also cause the corresponding "link" entry that would point out that relationship
+# to be removed from Swagger documentation, as well as from any returned link objects in real-world
+# response payloads. This would effectively make a relationship invisble in GET routing.
+disable_relationship_getters: list[str] = [],
 # The disable_nested_objects flag prevents users from sending dictionaries inside of relationship arrays
 # which the server will automatically unpack by default into an attempted create or update of the related
 # resource. Any nested objects sent will still flow through the entire policy chain of the target resource!
 # Any dictionary send with a primary key field will be handled as if it is an update. To create a new
 # object via an embedded relationship, send the nested object without a primary key set!
 disable_nested_objects: bool = False,
 # Default limit will only set a limit on incoming queries if the user DOES NOT specify one. You should
@@ -461,14 +468,25 @@
 # by overriding any limit query parameter sent by the user with a maximum number if the user value is
 # above whatever the max limit should be.
 default_limit: int = 10,
 # 'controller_extension' is the mount point for user-defined actions to-be-added to this resource's
 # controller/router. Pass in your class definition and it will be instantiated at the appropriate
 # time! See "CruddyController" example below!
 controller_extension: CruddyController = None,
+# 'custom_sql_identity_function' is an insertion point where you can pass in a lambda function or
+# other SYNCHRONOUS callable that will return some sqlalchemy query segment that determines the identity
+# of the resource in question. This is used for any CRUD actions that need to determine the identity
+# of a single record. Your lambda function / callable will be passed the {id} param from the controller.
+# You can use this to enable things like composite keys, and use {id} to capture <part a>.<part b>.
+custom_sql_identity_function: Callable[..., Any] | None = None,
+# 'custom_link_identity' is similar to custom_sql_identity_function, but is used specifically for building
+# the {id} segment of a 'link' value in the response JSON. The custom_link_identity function you pass in
+# will receive a record's value dictionary, which you can use to build a custom link {id} segment if needed.
+# You can use this to enable things like composite keys, and format {id} as <record value a>.<record value b>.
+custom_link_identity: Callable[..., str] | None = None,
 # The following REPOSITORY lifecycle hooks can each recieve an async function which will be invoked
 # before or after the target lifecycle event. Generally, whatever values are passed to the lifecycle
 # hook are alterable WITHIN the hook so that userspace code can alter the behavior of the lifecycle
 # based on app level concerns. This allows apps to do things like: hash a user password, force certain
 # relationships to always exist, force "many" queries to obey sensible limits, commit log entries,
 # send messages to queues for processing based on CRUD events, or generally handle unforseen
 # circumstances.
```

#### html2text {}

```diff
@@ -62,19 +62,19 @@
 # DATABASE ADAPTERS BaseAdapter SqliteAdapter MysqlAdapter PostgresqlAdapter #
 CONSTANTS BROADCAST_EVENT CONTROL_EVENT ROOM_EVENT CLIENT_EVENT
 KILL_SOCKET_BY_ID KILL_SOCKET_BY_CLIENT KILL_ROOM_BY_ID JOIN_SOCKET_BY_ID
 JOIN_SOCKET_BY_CLIENT LEAVE_SOCKET_BY_ID LEAVE_SOCKET_BY_CLIENT
 CLIENT_MESSAGE_EVENT DISCONNECT_EVENT # TYPES / MODELS / SCHEMAS T UUID
 RelationshipConfig CruddyGenericModel BulkDTO, MetaObject PageResponse
 ResponseSchema CruddyModel CruddyCreatedUpdatedSignature
-CruddyCreatedUpdatedMixin CruddyIntIDModel CruddyUUIDModel SocketMessage
-SocketRoomConfiguration ExampleUpdate ExampleCreate ExampleView Example #
-WEBSOCKET MODULES PubSub WebsocketConnectionManager RedisAdapter # MODULE
-LOADER HELPERS getModuleDir getDirectoryModules # HELPERS pluralizer uuid7
-field_checkers field_validators field_errors get_pk possible_id_types
+CruddyCreatedUpdatedMixin CruddyIntIDModel CruddyUUIDModel CruddyStringIDModel
+SocketMessage SocketRoomConfiguration ExampleUpdate ExampleCreate ExampleView
+Example # WEBSOCKET MODULES PubSub WebsocketConnectionManager RedisAdapter #
+MODULE LOADER HELPERS getModuleDir getDirectoryModules # HELPERS pluralizer
+uuid7 field_checkers field_validators field_errors get_pk possible_id_types
 lifecycle_types build_tz_aware_date parse_datetime coerce_to_utc_datetime
 parse_and_coerce_to_utc_datetime validate_utc_datetime json_serial
 to_json_string to_json_object get_state set_state # TEST HELPERS
 BrowserTestClient TestClient WebSocketSession # GRAPHQL EXPORTS
 GraphQLController GraphQLRequestCache GraphQLResolverService
 create_module_resolver graphql_where_synthesizer generate_gql_loader_and_type
 GQL_WHERE_REPLACEMENT_CHARACTER CruddyGQLDateTime CruddyGQLObject
@@ -300,52 +300,73 @@
 [Callable] = [], policies_get_many: Sequence[Callable] = [], # The disable_
 options allow app developers to simply abort automatic generation of select #
 CRUD endpoints on the resource's controller. For instance, to make a write-once
 collection a # developercould set disable_update to True, which would cause the
 resource to abort building a route # for PATCH resource/{id}. Be aware of the
 overall impact of endpoints you totally disable! disable_create: bool = False,
 disable_update: bool = False, disable_delete: bool = False, disable_get_one:
-bool = False, disable_get_many: bool = False, # The disable_nested_objects flag
-prevents users from sending dictionaries inside of relationship arrays # which
-the server will automatically unpack by default into an attempted create or
-update of the related # resource. Any nested objects sent will still flow
-through the entire policy chain of the target resource! # Any dictionary send
-with a primary key field will be handled as if it is an update. To create a new
-# object via an embedded relationship, send the nested object without a primary
-key set! disable_nested_objects: bool = False, # Default limit will only set a
-limit on incoming queries if the user DOES NOT specify one. You should #
-implement POLICIES to enforce a MAX limit, as you will ultimately have to re-
-use any max limit # policies in your own custom controller functions for
-consistency. Max limit policies can be implemented # by overriding any limit
-query parameter sent by the user with a maximum number if the user value is #
-above whatever the max limit should be. default_limit: int = 10, #
-'controller_extension' is the mount point for user-defined actions to-be-added
-to this resource's # controller/router. Pass in your class definition and it
-will be instantiated at the appropriate # time! See "CruddyController" example
-below! controller_extension: CruddyController = None, # The following
-REPOSITORY lifecycle hooks can each recieve an async function which will be
-invoked # before or after the target lifecycle event. Generally, whatever
-values are passed to the lifecycle # hook are alterable WITHIN the hook so that
-userspace code can alter the behavior of the lifecycle # based on app level
-concerns. This allows apps to do things like: hash a user password, force
-certain # relationships to always exist, force "many" queries to obey sensible
-limits, commit log entries, # send messages to queues for processing based on
-CRUD events, or generally handle unforseen # circumstances.
-lifecycle_before_create: Callable[..., Coroutine[Any, Any, Any]] | None = None,
-lifecycle_after_create: Callable[..., Coroutine[Any, Any, Any]] | None = None,
-lifecycle_before_update: Callable[..., Coroutine[Any, Any, Any]] | None = None,
-lifecycle_after_update: Callable[..., Coroutine[Any, Any, Any]] | None = None,
-lifecycle_before_delete: Callable[..., Coroutine[Any, Any, Any]] | None = None,
-lifecycle_after_delete: Callable[..., Coroutine[Any, Any, Any]] | None = None,
-lifecycle_before_get_one: Callable[..., Coroutine[Any, Any, Any]] | None =
-None, lifecycle_after_get_one: Callable[..., Coroutine[Any, Any, Any]] | None =
-None, lifecycle_before_get_all: Callable[..., Coroutine[Any, Any, Any]] | None
-= None, lifecycle_after_get_all: Callable[..., Coroutine[Any, Any, Any]] | None
-= None, lifecycle_before_set_relations: Callable[..., Coroutine[Any, Any, Any]]
-| None = None, lifecycle_after_set_relations: Callable[..., Coroutine[Any, Any,
+bool = False, disable_get_many: bool = False, # The
+disable_relationship_getters list allow app developers to instruct the
+framework to NOT hoist # an automatic GET route for a list of specific named
+relationships. Note, that any relationship name # you disable will also cause
+the corresponding "link" entry that would point out that relationship # to be
+removed from Swagger documentation, as well as from any returned link objects
+in real-world # response payloads. This would effectively make a relationship
+invisble in GET routing. disable_relationship_getters: list[str] = [], # The
+disable_nested_objects flag prevents users from sending dictionaries inside of
+relationship arrays # which the server will automatically unpack by default
+into an attempted create or update of the related # resource. Any nested
+objects sent will still flow through the entire policy chain of the target
+resource! # Any dictionary send with a primary key field will be handled as if
+it is an update. To create a new # object via an embedded relationship, send
+the nested object without a primary key set! disable_nested_objects: bool =
+False, # Default limit will only set a limit on incoming queries if the user
+DOES NOT specify one. You should # implement POLICIES to enforce a MAX limit,
+as you will ultimately have to re-use any max limit # policies in your own
+custom controller functions for consistency. Max limit policies can be
+implemented # by overriding any limit query parameter sent by the user with a
+maximum number if the user value is # above whatever the max limit should be.
+default_limit: int = 10, # 'controller_extension' is the mount point for user-
+defined actions to-be-added to this resource's # controller/router. Pass in
+your class definition and it will be instantiated at the appropriate # time!
+See "CruddyController" example below! controller_extension: CruddyController =
+None, # 'custom_sql_identity_function' is an insertion point where you can pass
+in a lambda function or # other SYNCHRONOUS callable that will return some
+sqlalchemy query segment that determines the identity # of the resource in
+question. This is used for any CRUD actions that need to determine the identity
+# of a single record. Your lambda function / callable will be passed the {id}
+param from the controller. # You can use this to enable things like composite
+keys, and use {id} to capture .. custom_sql_identity_function: Callable[...,
+Any] | None = None, # 'custom_link_identity' is similar to
+custom_sql_identity_function, but is used specifically for building # the {id}
+segment of a 'link' value in the response JSON. The custom_link_identity
+function you pass in # will receive a record's value dictionary, which you can
+use to build a custom link {id} segment if needed. # You can use this to enable
+things like composite keys, and format {id} as .. custom_link_identity:
+Callable[..., str] | None = None, # The following REPOSITORY lifecycle hooks
+can each recieve an async function which will be invoked # before or after the
+target lifecycle event. Generally, whatever values are passed to the lifecycle
+# hook are alterable WITHIN the hook so that userspace code can alter the
+behavior of the lifecycle # based on app level concerns. This allows apps to do
+things like: hash a user password, force certain # relationships to always
+exist, force "many" queries to obey sensible limits, commit log entries, # send
+messages to queues for processing based on CRUD events, or generally handle
+unforseen # circumstances. lifecycle_before_create: Callable[..., Coroutine
+[Any, Any, Any]] | None = None, lifecycle_after_create: Callable[..., Coroutine
+[Any, Any, Any]] | None = None, lifecycle_before_update: Callable[...,
+Coroutine[Any, Any, Any]] | None = None, lifecycle_after_update: Callable[...,
+Coroutine[Any, Any, Any]] | None = None, lifecycle_before_delete: Callable[...,
+Coroutine[Any, Any, Any]] | None = None, lifecycle_after_delete: Callable[...,
+Coroutine[Any, Any, Any]] | None = None, lifecycle_before_get_one: Callable
+[..., Coroutine[Any, Any, Any]] | None = None, lifecycle_after_get_one:
+Callable[..., Coroutine[Any, Any, Any]] | None = None,
+lifecycle_before_get_all: Callable[..., Coroutine[Any, Any, Any]] | None =
+None, lifecycle_after_get_all: Callable[..., Coroutine[Any, Any, Any]] | None =
+None, lifecycle_before_set_relations: Callable[..., Coroutine[Any, Any, Any]] |
+None = None, lifecycle_after_set_relations: Callable[..., Coroutine[Any, Any,
 Any]] | None = None, # The following CONTROLLER lifecycle hooks can each
 recieve an async function which will be invoked # before or after the target
 lifecycle event. Generally, whatever values are passed to the lifecycle # hook
 are alterable WITHIN the hook so that userspace code can alter the behavior of
 the lifecycle # based on app level concerns. CONTROLLER lifecycles hooks will
 also receive the REQUEST context, # allowing the hook to take actions that
 consider the user and their priveleges, while still # interleaving that logic
```

### Comparing `fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/__init__.py` & `fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     CruddyModel,
     CruddyCreatedUpdatedSignature,
     CruddyCreatedUpdatedGQLOverrides,
     CruddyCreatedUpdatedMixin,
     CruddyGQLOverrides,
     CruddyIntIDModel,
     CruddyUUIDModel,
+    CruddyStringIDModel,
     ExampleUpdate,
     ExampleCreate,
     ExampleView,
     Example,
     SocketMessage,
     SocketRoomConfiguration,
     uuid7,
```

### Comparing `fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/adapters.py` & `fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 from typing import AsyncIterator, Literal
 from contextlib import asynccontextmanager
 from redis.asyncio import Redis, from_url
 from fakeredis.aioredis import FakeRedis
+from sqlalchemy import text
 from sqlalchemy.pool import StaticPool
 from sqlalchemy.ext.asyncio import create_async_engine, AsyncEngine, async_sessionmaker
 from sqlmodel import text
 from sqlmodel.ext.asyncio.session import AsyncSession
 from .schemas import CruddyModel
 
 
@@ -133,14 +134,18 @@
             connect_args={"check_same_thread": False},
             poolclass=StaticPool,
             echo=echo,
             future=True,
             **kwargs,
         )
 
+    async def enable_foreignkey_constraints(self):
+        async with self.getSession() as session:
+            await session.execute(text("PRAGMA foreign_keys=ON"))
+
 
 # -------------------------------------------------------------------------------------------
 # REDIS ADAPTER
 # -------------------------------------------------------------------------------------------
 # The adapter for all things websocket
 class RedisAdapter:
     client: Redis | None = None
```

### Comparing `fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/controller.py` & `fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     Depends,
     HTTPException,
     status,
 )
 from .test_helpers import TestClient, BrowserTestClient
 from sqlalchemy import Row
 from sqlalchemy.sql.schema import Column, ForeignKey
-from sqlalchemy.sql.elements import ColumnElement
 from sqlalchemy.orm import (
     RelationshipDirection,
     ONETOMANY,
     MANYTOMANY,
     MANYTOONE,
 )
 from pydantic.types import Json
@@ -645,19 +644,27 @@
     repository: "AbstractRepository",
     id_type: possible_id_types,
     relationship_prop: str,
     config: RelationshipConfig,
     policies_universal: list,
     policies_get_one: list,
 ):
-    col: ColumnElement = next(iter(config.orm_relationship.local_columns))
-    far_side: ForeignKey = next(iter(col.foreign_keys))
-    far_col: Column = far_side.column
-    far_col_name = far_col.name
-    near_col_name = col.name
+    col_tuples = []
+    for col in iter(config.orm_relationship.local_columns):
+        far_side: ForeignKey = next(iter(col.foreign_keys))
+        far_col: Column = far_side.column
+        far_col_name = far_col.name
+        near_col_name = col.name
+        col_tuples.append(
+            (
+                near_col_name,
+                far_col_name,
+            )
+        )
+
     resource_model_name = f"{repository.model.__name__}".lower()
     foreign_model_name = f"{config.foreign_resource.repository.model.__name__}".lower()
 
     # Merge three policy sets onto this endpoint:
     # 1. Universal policies
     # 2. Primary resource policies
     # 3. Related resource policies
@@ -682,60 +689,67 @@
 
         # Consider raising 404 here and in get by ID
         if origin_record == None:
             raise HTTPException(
                 status_code=status.HTTP_404_NOT_FOUND, detail=f"Record {id} not found"
             )
 
-        # Build a query to use foreign resource to find related objects
-
-        tgt_id = origin_record.model_dump()[near_col_name]
-
         _repo_lifecycle_before = None
         foreign_repo_lifecycle_before = config.foreign_resource.repository.lifecycle[
             "before_get_one"
         ]
         foreign_repo_lifecycle_after = config.foreign_resource.repository.lifecycle[
             "after_get_one"
         ]
+
+        # Build a query to use foreign resource to find related objects
+        dumped_record = origin_record.model_dump()
+        # what to do here?
+        must_be = []
+        tgt_vals = []
+        for matches in col_tuples:
+            value = dumped_record[matches[0]]
+            tgt_vals.append(value)
+            must_be.append({matches[1]: {"*eq": value}})
+
         context_data = {
             DATA_KEY: {
-                "id": tgt_id,
+                "id": tgt_vals,
                 "where": where,
             },
             META_KEY: None,
         }
         # Execute the foreign controller lifecycle!
         if config.foreign_resource.controller_lifecycles["before_get_one"]:
             # If there is a user space lifecycle hook, run it (allows context mutations)
             await config.foreign_resource.controller_lifecycles["before_get_one"](
                 request, context_data
             )
 
-        must_be = {far_col_name: {"*eq": context_data[DATA_KEY]["id"]}}
-
         if foreign_repo_lifecycle_before:
 
             async def _shimmed_repo_lifecycle_before(query_conf: dict):
                 shim_where = query_conf["where"]
                 await foreign_repo_lifecycle_before(
                     context_data[DATA_KEY]["id"], shim_where
                 )
                 shim_where = (
-                    must_be if shim_where is None else {"*and": [must_be, shim_where]}
+                    {"*and": must_be}
+                    if shim_where is None
+                    else {"*and": must_be + [shim_where]}
                 )
                 query_conf["where"] = shim_where
                 return
 
             _repo_lifecycle_before = _shimmed_repo_lifecycle_before
         else:
             context_data[DATA_KEY]["where"] = (
-                must_be
+                {"*and": must_be}
                 if context_data[DATA_KEY]["where"] is None
-                else {"*and": [must_be, context_data[DATA_KEY]["where"]]}
+                else {"*and": must_be + [context_data[DATA_KEY]["where"]]}
             )
 
         # Collect the bulk data transfer object from the query
         result: BulkDTO = await config.foreign_resource.repository.get_all(
             page=1,
             limit=1,
             columns=columns,
@@ -784,18 +798,27 @@
     relationship_prop: str,
     config: RelationshipConfig,
     meta_schema: Type[CruddyModel] | Type[CruddyGenericModel] = MetaObject,
     policies_universal: list = [],
     policies_get_one: list = [],
     default_limit: int = 10,
 ):
-    far_col: ColumnElement = next(iter(config.orm_relationship.remote_side))
-    col: ColumnElement = next(iter(config.orm_relationship.local_columns))
-    far_col_name = far_col.name
-    near_col_name = col.name
+    col_tuples = []
+    for far_col in iter(config.orm_relationship.remote_side):
+        far_side: ForeignKey = next(iter(far_col.foreign_keys))
+        col: Column = far_side.column
+        far_col_name = far_col.name
+        near_col_name = col.name
+        col_tuples.append(
+            (
+                near_col_name,
+                far_col_name,
+            )
+        )
+
     resource_model_name = f"{repository.model.__name__}".lower()
     foreign_model_name = pluralizer.plural(
         f"{config.foreign_resource.repository.model.__name__}".lower()  # type: ignore
     )
 
     # Merge three policy sets onto this endpoint:
     # 1. Universal policies
@@ -825,18 +848,21 @@
 
         # Consider raising 404 here and in get by ID
         if origin_record == None:
             raise HTTPException(
                 status_code=status.HTTP_404_NOT_FOUND, detail=f"Record {id} not found"
             )
 
+        dumped_record = origin_record.model_dump()
+
         # Build a query to use foreign resource to find related objects
-        additional_where = {
-            far_col_name: {"*eq": origin_record.model_dump()[near_col_name]}
-        }
+        must_be = []
+        for matches in col_tuples:
+            value = dumped_record[matches[0]]
+            must_be.append({matches[1]: {"*eq": value}})
 
         _repo_lifecycle_before = None
         foreign_repo_lifecycle_before = config.foreign_resource.repository.lifecycle[
             "before_get_all"
         ]
 
         context_data = {
@@ -861,26 +887,26 @@
         # This is good because a lifecycle hook should only be concerned about its own resource.
         if foreign_repo_lifecycle_before:
 
             async def _shimmed_repo_lifecycle_before(query_conf):
                 await foreign_repo_lifecycle_before(query_conf)
                 shim_where = query_conf["where"]
                 query_conf["where"] = (
-                    additional_where
+                    {"*and": must_be}
                     if shim_where is None
-                    else {"*and": [additional_where, shim_where]}
+                    else {"*and": must_be + [shim_where]}
                 )
                 return
 
             _repo_lifecycle_before = _shimmed_repo_lifecycle_before
         else:
             context_data[DATA_KEY]["where"] = (
-                additional_where
+                {"*and": must_be}
                 if context_data[DATA_KEY]["where"] is None
-                else {"*and": [additional_where, context_data[DATA_KEY]["where"]]}
+                else {"*and": must_be + [context_data[DATA_KEY]["where"]]}
             )
 
         # Collect the bulk data transfer object from the query
         result: BulkDTO = await config.foreign_resource.repository.get_all(
             **context_data[DATA_KEY],
             _lifecycle_before=_repo_lifecycle_before,
             _lifecycle_after=config.foreign_resource.repository.lifecycle[
@@ -1036,14 +1062,15 @@
     policies_get_one=[],
     policies_get_many=[],
     disable_create=False,
     disable_update=False,
     disable_delete=False,
     disable_get_one=False,
     disable_get_many=False,
+    disable_relationship_getters=[],
 ) -> APIRouter:
     if not disable_create:
         controller.post(
             "",
             description=f"Create a single '{single_name}'",
             response_model=single_schema,
             response_model_exclude_none=True,
@@ -1086,14 +1113,16 @@
             dependencies=assemble_policies(policies_universal, policies_get_many),
         )(actions.get_all)
 
     # Add relationship link endpoints starting here...
     # Maybe add way to disable these getters?
     # Maybe add way to wrangle this unknown number of functions into the actions map?
     for key, config in relations.items():
+        if key in disable_relationship_getters:
+            continue
         if config.orm_relationship.direction == ONETOMANY:
             _ControllerConfigOneToMany(
                 controller=controller,
                 repository=repository,
                 id_type=id_type,
                 relationship_prop=key,
                 config=config,
```

### Comparing `fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/graphql.py` & `fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/graphql.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/pubsub.py` & `fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/pubsub.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/repository.py` & `fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import math
-from typing import Any
+from typing import Any, Callable
 from asyncio import TaskGroup
 from logging import getLogger
 from sqlalchemy import (
     update as _update,
     delete as _delete,
     or_,
     and_,
@@ -188,14 +188,15 @@
 class AbstractRepository:
     adapter: BaseAdapter | SqliteAdapter | MysqlAdapter | PostgresqlAdapter
     update_model: Type[CruddyModel]
     create_model: Type[CruddyModel]
     model: Type[CruddyModel]
     id_type: possible_id_types
     primary_key: str | None = None
+    identity_function: Callable[..., Any]
     lifecycle: dict[str, lifecycle_types] = {
         "before_create": None,
         "after_create": None,
         "before_update": None,
         "after_update": None,
         "before_delete": None,
         "after_delete": None,
@@ -212,14 +213,15 @@
     def __init__(
         self,
         adapter: BaseAdapter | SqliteAdapter | MysqlAdapter | PostgresqlAdapter,
         update_model: Type[CruddyModel],
         create_model: Type[CruddyModel],
         model: Type[CruddyModel],
         id_type: possible_id_types = int,
+        custom_sql_identity_function: Callable | None = None,
         lifecycle_before_create: lifecycle_types = None,
         lifecycle_after_create: lifecycle_types = None,
         lifecycle_before_update: lifecycle_types = None,
         lifecycle_after_update: lifecycle_types = None,
         lifecycle_before_delete: lifecycle_types = None,
         lifecycle_after_delete: lifecycle_types = None,
         lifecycle_before_get_one: lifecycle_types = None,
@@ -249,14 +251,22 @@
             "before_get_one": lifecycle_before_get_one,
             "after_get_one": lifecycle_after_get_one,
             "before_get_all": lifecycle_before_get_all,
             "after_get_all": lifecycle_after_get_all,
             "before_set_relations": lifecycle_before_set_relations,
             "after_set_relations": lifecycle_after_set_relations,
         }
+        self.identity_function = (
+            custom_sql_identity_function
+            if custom_sql_identity_function is not None
+            else self._default_identity_function
+        )
+
+    def _default_identity_function(self, id: possible_id_types):
+        return getattr(self.model, str(self.primary_key)) == id
 
     def resolve(self):
         # Can't do this until all models are defined, otherwise mappers break
         self.primary_key = get_pk(self.model)
 
     async def create(self, data: CruddyModel) -> CruddyModel:
         # create user data
@@ -273,15 +283,15 @@
     async def get_by_id(self, id: possible_id_values, where: Json = None) -> Any | None:
         # retrieve user data by id
         async with self.adapter.getSession() as session:
             if self.lifecycle["before_get_one"]:
                 await self.lifecycle["before_get_one"](id, where)
             query = select(self.model).where(
                 and_(
-                    getattr(self.model, str(self.primary_key)) == id,
+                    self.identity_function(id),
                     *self.query_forge(model=self.model, where=where),
                 )
             )
             result = (await session.execute(query)).scalar_one_or_none()
         if self.lifecycle["after_get_one"]:
             await self.lifecycle["after_get_one"](result)
         return result
@@ -289,15 +299,15 @@
     async def update(self, id: possible_id_values, data: CruddyModel):
         # update user data
         values = data.model_dump()
         if self.lifecycle["before_update"]:
             await self.lifecycle["before_update"](values, id)
         query = (
             _update(self.model)
-            .where(getattr(self.model, str(self.primary_key)) == id)
+            .where(self.identity_function(id))
             .values(**values)
             .execution_options(synchronize_session="fetch")
         )
         async with self.adapter.getSession() as session:
             result = await session.execute(query)
         if result.rowcount == 1:  # type: ignore
             updated_record = await self.get_by_id(id=id)
@@ -310,15 +320,15 @@
     async def delete(self, id: possible_id_values):
         # delete user data by id
         record = await self.get_by_id(id=id)
         if self.lifecycle["before_delete"]:
             await self.lifecycle["before_delete"](record)
         query = (
             _delete(self.model)
-            .where(getattr(self.model, str(self.primary_key)) == id)
+            .where(self.identity_function(id))
             .execution_options(synchronize_session="fetch")
         )
         async with self.adapter.getSession() as session:
             result = await session.execute(query)
 
         if result.rowcount == 1:  # type: ignore
             if self.lifecycle["after_delete"]:
@@ -468,15 +478,15 @@
 
         select_items = [getattr(relation_model, x) for x in get_columns]
 
         query = select(*select_items)
 
         query = query.join(getattr(self.model, relation))
 
-        joinable = [getattr(self.model, str(self.primary_key)) == id]
+        joinable = [self.identity_function(id)]
 
         if isinstance(query_conf["where"], dict) or isinstance(
             query_conf["where"], list
         ):
             joinable.extend(
                 self.query_forge(model=relation_model, where=query_conf["where"])
             )
```

### Comparing `fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/resource.py` & `fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 # -------------------------------------------------------------------------------------------
 # APPLICATION RESOURCE
 # -------------------------------------------------------------------------------------------
 class Resource:
     _registry: "ResourceRegistry"
     _link_prefix: str = ""
     _relations: dict[str, RelationshipConfig] = {}
+    _relational_getters: list[str] = []
     _resource_path: str = "/example"
     _tags: list[str | Enum] = ["example"]
     _create_schema: Type[CruddyModel]
     _update_schema: Type[CruddyModel]
     _response_schema: Type[CruddyModel]
     _meta_schema: Type[CruddyModel] | Type[CruddyGenericModel]
     _id_type: possible_id_types = int
@@ -76,16 +77,18 @@
     _artificial_relationship_paths: list[str]
     _default_limit: int
     adapter: BaseAdapter | SqliteAdapter | MysqlAdapter | PostgresqlAdapter
     actions: Actions
     repository: AbstractRepository
     controller: APIRouter
     controller_extension: Type[CruddyController] | None = None
+    link_identity: Callable[..., str]
     policies: dict[str, Sequence[Callable]]
     disabled_endpoints: dict[str, bool]
+    disabled_relationship_getters: list[str]
     disable_nested_objects: bool
     schemas: SchemaDict
     controller_lifecycles: dict[str, lifecycle_types]
 
     def __init__(
         self,
         # Only id_type, adapter, resource_create_model, resource_update_model, resource_model, and response_schema are required
@@ -115,19 +118,22 @@
         artificial_relationship_paths: list[str] = [],
         policies_universal: Sequence[Callable] = [],
         policies_create: Sequence[Callable] = [],
         policies_update: Sequence[Callable] = [],
         policies_delete: Sequence[Callable] = [],
         policies_get_one: Sequence[Callable] = [],
         policies_get_many: Sequence[Callable] = [],
+        custom_sql_identity_function: Callable[..., Any] | None = None,
+        custom_link_identity: Callable[..., str] | None = None,
         disable_create: bool = False,
         disable_update: bool = False,
         disable_delete: bool = False,
         disable_get_one: bool = False,
         disable_get_many: bool = False,
+        disable_relationship_getters: list[str] = [],
         disable_nested_objects: bool = False,
         default_limit: int = 10,
         # Repository lifecycle actions
         lifecycle_before_create: lifecycle_types = None,
         lifecycle_after_create: lifecycle_types = None,
         lifecycle_before_update: lifecycle_types = None,
         lifecycle_after_update: lifecycle_types = None,
@@ -160,20 +166,27 @@
         self._tags = [possible_tag] if tags == None else tags
         self._response_schema = response_schema
         self._update_schema = resource_update_model
         self._create_schema = resource_create_model
         self._meta_schema = response_meta_schema
         self._id_type = id_type
         self._relations = {}
+        self._relational_getters = []
         self._protected_relationships = protected_relationships
         self._protected_create_relationships = protected_create_relationships
         self._protected_update_relationships = protected_update_relationships
         self._artificial_relationship_paths = artificial_relationship_paths
         self._default_limit = default_limit
 
+        self.link_identity = (
+            custom_link_identity
+            if custom_link_identity is not None
+            else self._default_link_identity
+        )
+
         self.policies = {
             "universal": policies_universal,
             "create": policies_create,
             "update": policies_update,
             "delete": policies_delete,
             "get_one": policies_get_one,
             "get_many": policies_get_many,
@@ -183,14 +196,16 @@
             "create": disable_create,
             "update": disable_update,
             "delete": disable_delete,
             "get_one": disable_get_one,
             "get_many": disable_get_many,
         }
 
+        self.disabled_relationship_getters = disable_relationship_getters
+
         self.controller_lifecycles = {
             "before_create": lifecycle_before_controller_create,
             "after_create": lifecycle_after_controller_create,
             "before_update": lifecycle_before_controller_update,
             "after_update": lifecycle_after_controller_update,
             "before_delete": lifecycle_before_controller_delete,
             "after_delete": lifecycle_after_controller_delete,
@@ -213,14 +228,15 @@
 
         self.repository = AbstractRepository(
             adapter=self.adapter,  # type: ignore
             update_model=resource_update_model,
             create_model=resource_create_model,
             model=resource_model,
             id_type=id_type,
+            custom_sql_identity_function=custom_sql_identity_function,
             lifecycle_before_create=lifecycle_before_create,
             lifecycle_after_create=lifecycle_after_create,
             lifecycle_before_update=lifecycle_before_update,
             lifecycle_after_update=lifecycle_after_update,
             lifecycle_before_delete=lifecycle_before_delete,
             lifecycle_after_delete=lifecycle_after_delete,
             lifecycle_before_get_one=lifecycle_before_get_one,
@@ -250,50 +266,26 @@
         self._relations[f"{relationship.key}"] = RelationshipConfig(
             orm_relationship=relationship, foreign_resource=foreign_resource
         )
 
     def set_local_link_prefix(self, prefix: str):
         self._link_prefix = prefix
 
-    # The response schema factory
-    # Converting this section a plugin pattern will allow
-    # other response formats, like JSON API.
-    # Alterations will also require ControllerConfigurator
-    # to be modified somehow...
+    def _format_example_id(self, value: Any):
+        return int(str(value)) if self.repository.id_type == int else str(value)
 
-    def generate_internal_schemas(self):
-        local_resource = self
+    def _setup_example_id(self, id: str | UUID | int | bytes):
+        example_id = id
         response_schema: CruddyModel = self._response_schema
-        create_schema = self._create_schema
-        update_schema = self._update_schema
-        response_meta_schema = self._meta_schema
-        resource_model_name = f"{self.repository.model.__name__}".lower()
-        resource_model_plural = pluralizer.plural(resource_model_name)  # type: ignore
-        resource_response_name = response_schema.__name__
-        resource_create_name = create_schema.__name__
-        resource_update_name = update_schema.__name__
-
-        self._model_name_single = resource_model_name
-        self._model_name_plural = resource_model_plural
-
-        # Attempt to align swagger example uuids if possible (non-critical)
-        example_id = uuid7() if self.repository.id_type == UUID else 123
-        if self.repository.id_type == str:
-            example_id = str(example_id)
-        possible_id = response_schema.model_fields.get("id", None)
+        possible_id = response_schema.model_fields.get(
+            self.repository.primary_key or "id", None
+        )
         if possible_id is not None and issubclass(
             self.repository.id_type, possible_id.annotation  # type: ignore
         ):
-            example_dict = {
-                "example": (
-                    int(str(example_id))
-                    if self.repository.id_type == int
-                    else str(example_id)
-                )
-            }
             if possible_id.json_schema_extra is not None:
                 possible_id_examples = possible_id.json_schema_extra.get(
                     "examples", None
                 )
                 if not isinstance(possible_id_examples, list):
                     possible_id_examples = []
                 possible_id_example = possible_id.json_schema_extra.get("example", None)
@@ -305,30 +297,35 @@
                     possible_id.default, PydanticUndefinedType
                 ):
                     example_id = possible_id.default
                 elif possible_id.default_factory is not None:
                     temp_example = possible_id.default_factory()
                     if not isinstance(temp_example, PydanticUndefinedType):
                         example_id = temp_example
-                possible_id.json_schema_extra.update(example_dict)
+                possible_id.json_schema_extra.update(
+                    {"example": self._format_example_id(example_id)}
+                )
             else:
-                possible_id.json_schema_extra = example_dict  # type: ignore
+                possible_id.json_schema_extra = {  # type: ignore
+                    "example": self._format_example_id(example_id)
+                }
+        return example_id
 
-        # Create shared link model
+    def _setup_support_classes(self, id: Any):
+        view_example_dict = {}
         link_object = {}
         false_create_attrs = {}
         false_update_attrs = {}
-        view_example_dict = {}
+        response_schema: CruddyModel = self._response_schema
         create_protected_relationships = (
             self._protected_relationships + self._protected_create_relationships
         )
         update_protected_relationships = (
             self._protected_relationships + self._protected_update_relationships
         )
-
         for k, v in response_schema.model_fields.items():
             default_example = None
             if v.json_schema_extra is not None:
                 possible_examples = v.json_schema_extra.get("examples", None)
                 possible_example = v.json_schema_extra.get("example", None)
                 if isinstance(possible_examples, list) and len(possible_examples) > 0:
                     default_example = possible_examples[0]
@@ -342,36 +339,79 @@
                 default_example = v.default_factory()
                 if isinstance(default_example, PydanticUndefinedType):
                     default_example = None
             if default_example is None:
                 default_example = estimate_simple_example(v.annotation)
             view_example_dict[k] = squash_type(default_example)
         view_example_dict["links"] = {}
+
         for k, v in self._relations.items():
-            ex_link = self._single_link(id=str(example_id), relationship=k)
-            link_object[k] = (
-                str,
-                Field(schema_extra={"json_schema_extra": {"example": ex_link}}),
-            )
-            view_example_dict["links"][k] = ex_link
             rel_def = self._derive_shadow_relationship(
                 v.orm_relationship.direction, v.foreign_resource._id_type
             )
             if k not in create_protected_relationships:
                 false_create_attrs[k] = rel_def
             if k not in update_protected_relationships:
                 false_update_attrs[k] = rel_def
+            if k in self.disabled_relationship_getters:
+                continue
+            self._relational_getters.append(k)
+            ex_link = self._single_link(
+                id=self.link_identity(view_example_dict), relationship=k
+            )
+            link_object[k] = (
+                str,
+                Field(schema_extra={"json_schema_extra": {"example": ex_link}}),
+            )
+            view_example_dict["links"][k] = ex_link
+
         for item in self._artificial_relationship_paths:
-            ex_link = self._single_link(id=str(example_id), relationship=item)
+            ex_link = self._single_link(
+                id=self.link_identity(view_example_dict), relationship=item
+            )
             link_object[item] = (
                 str,
                 Field(schema_extra={"json_schema_extra": {"example": ex_link}}),
             )
             view_example_dict["links"][item] = ex_link
         link_object["__base__"] = CruddyModel
+
+        return link_object, view_example_dict, false_create_attrs, false_update_attrs
+
+    # The response schema factory
+    # Converting this section a plugin pattern will allow
+    # other response formats, like JSON API.
+    # Alterations will also require ControllerConfigurator
+    # to be modified somehow...
+    def generate_internal_schemas(self):
+        self.repository.resolve()
+        response_schema: CruddyModel = self._response_schema
+        create_schema = self._create_schema
+        update_schema = self._update_schema
+        response_meta_schema = self._meta_schema
+        resource_model_name = f"{self.repository.model.__name__}".lower()
+        resource_model_plural = pluralizer.plural(resource_model_name)  # type: ignore
+        resource_response_name = response_schema.__name__
+        resource_create_name = create_schema.__name__
+        resource_update_name = update_schema.__name__
+
+        self._model_name_single = resource_model_name
+        self._model_name_plural = resource_model_plural
+
+        # Attempt to align swagger example uuids if possible (non-critical)
+        example_id = uuid7() if self.repository.id_type == UUID else 123
+        if self.repository.id_type != int:
+            example_id = str(example_id)
+        example_id = self._setup_example_id(example_id)
+
+        # Create shared link model
+        link_object, view_example_dict, false_create_attrs, false_update_attrs = (
+            self._setup_support_classes(example_id)
+        )
+
         LinkModel = create_model(f"{resource_model_name}Links", **link_object)
         # End shared link model
 
         SingleCreateSchema = create_model(
             f"{resource_create_name}Proxy", __base__=create_schema, **false_create_attrs
         )
 
@@ -471,26 +511,27 @@
                     ),
                 ),
             },  # type: ignore
             meta=(response_meta_schema, ...),
         )
 
         old_many_init = ManySchemaEnvelope.__init__
+        local_resource = self
 
         def new_many_init(self, *args, **kwargs):
             old_many_init(
                 self,
                 *args,
                 **{
                     resource_model_plural: (
                         [
                             SingleSchemaLinked(
                                 **x._mapping,
                                 links=local_resource._link_builder(  # type: ignore
-                                    id=x._mapping[local_resource.repository.primary_key]
+                                    fields=x._mapping
                                 ),
                             )
                             for x in kwargs["data"]
                         ]
                         if resource_model_plural not in kwargs
                         else kwargs[resource_model_plural]
                     ),
@@ -499,15 +540,14 @@
                 },
             )
 
         ManySchemaEnvelope.__init__ = new_many_init
         # End many records return payload
 
         # Expose the following schemas for further use
-
         self.schemas = {  # type: ignore
             "single": SingleSchemaEnvelope,
             "many": ManySchemaEnvelope,
             "create": SingleCreateEnvelope,
             "create_relations": SingleCreateSchema,
             "update": SingleUpdateEnvelope,
             "update_relations": SingleUpdateSchema,
@@ -524,24 +564,32 @@
             if direction in [MANYTOMANY, ONETOMANY]
             else (
                 dict | id_type | None,
                 None,
             )
         )
 
-    def _link_builder(self, id: possible_id_values):
+    def _default_link_identity(self, fields: dict[str, Any]):
+        if self.repository.primary_key is None:
+            raise RuntimeError("Resource was not properly initialized!")
+        id = fields[self.repository.primary_key]
+        if (self.repository.id_type == UUID and type(id) == str) and not "-" in id:
+            id = re.sub(r"(\S{8})(\S{4})(\S{4})(\S{4})(.*)", r"\1-\2-\3-\4-\5", id)
+        return id
+
+    def _link_builder(
+        self, fields: dict[str, Any]
+    ):  # id: possible_id_values, fields: dict[str, Any]):
         # During "many" lookups, and depending on DB type, the id value return is a mapping
         # from the DB, so the id value is not properly "dasherized" into UUID format. This
         # REGEX fixes the issue without adding the CPU overhead of transforming each row
         # into a record instance.
-        if (self.repository.id_type == UUID and type(id) == str) and not "-" in id:
-            id = re.sub(r"(\S{8})(\S{4})(\S{4})(\S{4})(.*)", r"\1-\2-\3-\4-\5", id)
-
+        id = self.link_identity(fields)
         new_link_object = {}
-        for k, v in self._relations.items():
+        for k in self._relational_getters:
             new_link_object[k] = self._single_link(id=id, relationship=k)
         for item in self._artificial_relationship_paths:
             new_link_object[item] = self._single_link(id=id, relationship=item)
         return new_link_object
 
     def _single_link(self, id: possible_id_values = "", relationship: str = ""):
         return f"{self._link_prefix}{self._resource_path}/{id}/{relationship}"
@@ -574,29 +622,27 @@
                     "data": None,
                 }
 
             if key_count == 1 and args["data"] == None:
                 return {"data": None, "meta": meta}
 
             thing_to_convert = data_destructure(args["data"])
-            id = thing_to_convert[self.repository.primary_key]
+            # id = thing_to_convert[self.repository.primary_key]
             return {
                 resource_model_name: single_schema_linked(
                     **thing_to_convert,
-                    links=self._link_builder(id=id),
+                    links=self._link_builder(fields=thing_to_convert),  # id=id,
                 ),
                 "meta": meta,
                 "data": None,
             }
 
         return handle_data_or_none
 
     def resolve(self):
-        self.repository.resolve()
-
         self.actions = Actions(
             id_type=self._id_type,
             disable_nested_objects=self.disable_nested_objects,
             single_name=self._model_name_single,
             repository=self.repository,
             create_model=self.schemas["create"],
             create_model_proxy=self._create_schema,
@@ -639,14 +685,15 @@
             policies_get_one=self.policies["get_one"],
             policies_get_many=self.policies["get_many"],
             disable_create=self.disabled_endpoints["create"],
             disable_update=self.disabled_endpoints["update"],
             disable_delete=self.disabled_endpoints["delete"],
             disable_get_one=self.disabled_endpoints["get_one"],
             disable_get_many=self.disabled_endpoints["get_many"],
+            disable_relationship_getters=self.disabled_relationship_getters,
         )
 
         if callable(self._on_resolution):
             self._on_resolution()
 
     @staticmethod
     def _set_registry(reg: "ResourceRegistry"):
@@ -739,28 +786,30 @@
             base_model = resource.repository.model
             # Get the human friendly name for this model
             map_name = base_model.__name__
             # Inspect the fully loaded model class for relationships
             relationships = inspect(base_model).relationships
             rel_map = {}
 
+            # This loop will inject relationships into all resources that need them
             for relation in relationships:
                 rel_map[relation.key] = relation
                 # this seems unsafe...
                 target_resource_name = relation.entity.class_.__name__
                 target_resource = self._resources_via_models[target_resource_name]
                 resource.inject_relationship(
                     relationship=relation, foreign_resource=target_resource
                 )
 
             self._rels_via_models[map_name] = rel_map
+            # generating schemas will also cause the repository classes to resolve (needed for primary key determination)
             resource.generate_internal_schemas()
 
         # Build routes
-        # These have to be separated to ensure all schemas are ready
+        # These have to be separated to ensure all schemas are ready from generate_internal_schemas()
         for resource in self._resources:
             resource.resolve()
 
         self._resolver_completed = True
         # Clear this debouncer so any future dynamic resources can try to resolve
         self._resolver_invoked = False
```

### Comparing `fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/router.py` & `fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/schemas.py` & `fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,28 +3,31 @@
     Type,
     TypeVar,
     Generic,
     Sequence,
     NewType,
     TYPE_CHECKING,
 )
+from re import match
 from datetime import datetime
 from uuid import UUID
 from uuid_extensions import uuid7
+from fastapi import HTTPException, status
 from sqlalchemy import Column
 from sqlalchemy.orm import declared_attr, RelationshipProperty
 from sqlalchemy.engine.row import Row
 from pydantic import BaseModel, ConfigDict, field_validator
 from strawberry import scalar
 from sqlmodel import Field, SQLModel, DateTime
 from .util import build_tz_aware_date, parse_and_coerce_to_utc_datetime
 
 if TYPE_CHECKING:
     from .resource import Resource
 
+HTTP_422_UNPROCESSABLE_ENTITY = status.HTTP_422_UNPROCESSABLE_ENTITY
 
 # -------------------------------------------------------------------------------------------
 # SCHEMAS / MODELS
 # -------------------------------------------------------------------------------------------
 BROADCAST_EVENT = "broadcast"
 CONTROL_EVENT = "control"
 DISCONNECT_EVENT = "disconnect"
@@ -141,14 +144,37 @@
         default_factory=uuid7,
         primary_key=True,
         index=True,
         nullable=False,
     )
 
 
+class CruddyStringIDModel(CruddyModel):
+    id: str = Field(
+        default=None,
+        primary_key=True,
+        index=True,
+        nullable=False,
+    )
+
+    @field_validator("id", mode="before")
+    @classmethod
+    def validate_id(cls, v: Any) -> str:
+        if not isinstance(v, str):
+            raise HTTPException(
+                status_code=HTTP_422_UNPROCESSABLE_ENTITY, detail=f"{v} is not a string"
+            )
+        if not match(r"^[a-zA-Z0-9_-]+( [a-zA-Z0-9_-]+)*$", v):
+            raise HTTPException(
+                status_code=HTTP_422_UNPROCESSABLE_ENTITY,
+                detail=f"{v} must be alphanumeric, with dashes or underscores and only one space max between words",
+            )
+        return v
+
+
 class CruddyCreatedUpdatedSignature(CruddyModel):
     created_at: datetime | None = None
     updated_at: datetime | None = None
 
 
 def CruddyCreatedUpdatedMixin() -> type[CruddyCreatedUpdatedSignature]:
     class CruddyCreatedUpdatedInstance(CruddyCreatedUpdatedSignature):
```

### Comparing `fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/test_helpers.py` & `fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/test_helpers.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/util.py` & `fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/util.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.9/fastapi_cruddy_framework/websocket_manager.py` & `fastapi_cruddy_framework-1.5.0/fastapi_cruddy_framework/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.9/pyproject.toml` & `fastapi_cruddy_framework-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-cruddy-framework"
-version = "1.4.9"
+version = "1.5.0"
 description = "A holistic CRUD/MVC framework for FastAPI, with endpoint policies and relationships"
 authors = ["mdconaway <mdconaway@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "fastapi_cruddy_framework"}]
 homepage = "https://github.com/mdconaway/fastapi-cruddy-framework"
 repository = "https://github.com/mdconaway/fastapi-cruddy-framework"
 keywords = ["fastapi", "crud", "mvc", "orm", "ember", "sails", "json"]
```

### Comparing `fastapi_cruddy_framework-1.4.9/PKG-INFO` & `fastapi_cruddy_framework-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-cruddy-framework
-Version: 1.4.9
+Version: 1.5.0
 Summary: A holistic CRUD/MVC framework for FastAPI, with endpoint policies and relationships
 Home-page: https://github.com/mdconaway/fastapi-cruddy-framework
 Keywords: fastapi,crud,mvc,orm,ember,sails,json
 Author: mdconaway
 Author-email: mdconaway@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -164,14 +164,15 @@
 PageResponse
 ResponseSchema
 CruddyModel
 CruddyCreatedUpdatedSignature
 CruddyCreatedUpdatedMixin
 CruddyIntIDModel
 CruddyUUIDModel
+CruddyStringIDModel
 SocketMessage
 SocketRoomConfiguration
 ExampleUpdate
 ExampleCreate
 ExampleView
 Example
 # WEBSOCKET MODULES
@@ -481,14 +482,20 @@
 # developercould set disable_update to True, which would cause the resource to abort building a route
 # for PATCH resource/{id}. Be aware of the overall impact of endpoints you totally disable!
 disable_create: bool = False,
 disable_update: bool = False,
 disable_delete: bool = False,
 disable_get_one: bool = False,
 disable_get_many: bool = False,
+# The disable_relationship_getters list allow app developers to instruct the framework to NOT hoist
+# an automatic GET route for a list of specific named relationships. Note, that any relationship name
+# you disable will also cause the corresponding "link" entry that would point out that relationship
+# to be removed from Swagger documentation, as well as from any returned link objects in real-world
+# response payloads. This would effectively make a relationship invisble in GET routing.
+disable_relationship_getters: list[str] = [],
 # The disable_nested_objects flag prevents users from sending dictionaries inside of relationship arrays
 # which the server will automatically unpack by default into an attempted create or update of the related
 # resource. Any nested objects sent will still flow through the entire policy chain of the target resource!
 # Any dictionary send with a primary key field will be handled as if it is an update. To create a new
 # object via an embedded relationship, send the nested object without a primary key set!
 disable_nested_objects: bool = False,
 # Default limit will only set a limit on incoming queries if the user DOES NOT specify one. You should
@@ -497,14 +504,25 @@
 # by overriding any limit query parameter sent by the user with a maximum number if the user value is
 # above whatever the max limit should be.
 default_limit: int = 10,
 # 'controller_extension' is the mount point for user-defined actions to-be-added to this resource's
 # controller/router. Pass in your class definition and it will be instantiated at the appropriate
 # time! See "CruddyController" example below!
 controller_extension: CruddyController = None,
+# 'custom_sql_identity_function' is an insertion point where you can pass in a lambda function or
+# other SYNCHRONOUS callable that will return some sqlalchemy query segment that determines the identity
+# of the resource in question. This is used for any CRUD actions that need to determine the identity
+# of a single record. Your lambda function / callable will be passed the {id} param from the controller.
+# You can use this to enable things like composite keys, and use {id} to capture <part a>.<part b>.
+custom_sql_identity_function: Callable[..., Any] | None = None,
+# 'custom_link_identity' is similar to custom_sql_identity_function, but is used specifically for building
+# the {id} segment of a 'link' value in the response JSON. The custom_link_identity function you pass in
+# will receive a record's value dictionary, which you can use to build a custom link {id} segment if needed.
+# You can use this to enable things like composite keys, and format {id} as <record value a>.<record value b>.
+custom_link_identity: Callable[..., str] | None = None,
 # The following REPOSITORY lifecycle hooks can each recieve an async function which will be invoked
 # before or after the target lifecycle event. Generally, whatever values are passed to the lifecycle
 # hook are alterable WITHIN the hook so that userspace code can alter the behavior of the lifecycle
 # based on app level concerns. This allows apps to do things like: hash a user password, force certain
 # relationships to always exist, force "many" queries to obey sensible limits, commit log entries,
 # send messages to queues for processing based on CRUD events, or generally handle unforseen
 # circumstances.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-cruddy-framework Version: 1.4.9 Summary: A
+Metadata-Version: 2.1 Name: fastapi-cruddy-framework Version: 1.5.0 Summary: A
 holistic CRUD/MVC framework for FastAPI, with endpoint policies and
 relationships Home-page: https://github.com/mdconaway/fastapi-cruddy-framework
 Keywords: fastapi,crud,mvc,orm,ember,sails,json Author: mdconaway Author-email:
 mdconaway@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
@@ -84,19 +84,19 @@
 # DATABASE ADAPTERS BaseAdapter SqliteAdapter MysqlAdapter PostgresqlAdapter #
 CONSTANTS BROADCAST_EVENT CONTROL_EVENT ROOM_EVENT CLIENT_EVENT
 KILL_SOCKET_BY_ID KILL_SOCKET_BY_CLIENT KILL_ROOM_BY_ID JOIN_SOCKET_BY_ID
 JOIN_SOCKET_BY_CLIENT LEAVE_SOCKET_BY_ID LEAVE_SOCKET_BY_CLIENT
 CLIENT_MESSAGE_EVENT DISCONNECT_EVENT # TYPES / MODELS / SCHEMAS T UUID
 RelationshipConfig CruddyGenericModel BulkDTO, MetaObject PageResponse
 ResponseSchema CruddyModel CruddyCreatedUpdatedSignature
-CruddyCreatedUpdatedMixin CruddyIntIDModel CruddyUUIDModel SocketMessage
-SocketRoomConfiguration ExampleUpdate ExampleCreate ExampleView Example #
-WEBSOCKET MODULES PubSub WebsocketConnectionManager RedisAdapter # MODULE
-LOADER HELPERS getModuleDir getDirectoryModules # HELPERS pluralizer uuid7
-field_checkers field_validators field_errors get_pk possible_id_types
+CruddyCreatedUpdatedMixin CruddyIntIDModel CruddyUUIDModel CruddyStringIDModel
+SocketMessage SocketRoomConfiguration ExampleUpdate ExampleCreate ExampleView
+Example # WEBSOCKET MODULES PubSub WebsocketConnectionManager RedisAdapter #
+MODULE LOADER HELPERS getModuleDir getDirectoryModules # HELPERS pluralizer
+uuid7 field_checkers field_validators field_errors get_pk possible_id_types
 lifecycle_types build_tz_aware_date parse_datetime coerce_to_utc_datetime
 parse_and_coerce_to_utc_datetime validate_utc_datetime json_serial
 to_json_string to_json_object get_state set_state # TEST HELPERS
 BrowserTestClient TestClient WebSocketSession # GRAPHQL EXPORTS
 GraphQLController GraphQLRequestCache GraphQLResolverService
 create_module_resolver graphql_where_synthesizer generate_gql_loader_and_type
 GQL_WHERE_REPLACEMENT_CHARACTER CruddyGQLDateTime CruddyGQLObject
@@ -322,52 +322,73 @@
 [Callable] = [], policies_get_many: Sequence[Callable] = [], # The disable_
 options allow app developers to simply abort automatic generation of select #
 CRUD endpoints on the resource's controller. For instance, to make a write-once
 collection a # developercould set disable_update to True, which would cause the
 resource to abort building a route # for PATCH resource/{id}. Be aware of the
 overall impact of endpoints you totally disable! disable_create: bool = False,
 disable_update: bool = False, disable_delete: bool = False, disable_get_one:
-bool = False, disable_get_many: bool = False, # The disable_nested_objects flag
-prevents users from sending dictionaries inside of relationship arrays # which
-the server will automatically unpack by default into an attempted create or
-update of the related # resource. Any nested objects sent will still flow
-through the entire policy chain of the target resource! # Any dictionary send
-with a primary key field will be handled as if it is an update. To create a new
-# object via an embedded relationship, send the nested object without a primary
-key set! disable_nested_objects: bool = False, # Default limit will only set a
-limit on incoming queries if the user DOES NOT specify one. You should #
-implement POLICIES to enforce a MAX limit, as you will ultimately have to re-
-use any max limit # policies in your own custom controller functions for
-consistency. Max limit policies can be implemented # by overriding any limit
-query parameter sent by the user with a maximum number if the user value is #
-above whatever the max limit should be. default_limit: int = 10, #
-'controller_extension' is the mount point for user-defined actions to-be-added
-to this resource's # controller/router. Pass in your class definition and it
-will be instantiated at the appropriate # time! See "CruddyController" example
-below! controller_extension: CruddyController = None, # The following
-REPOSITORY lifecycle hooks can each recieve an async function which will be
-invoked # before or after the target lifecycle event. Generally, whatever
-values are passed to the lifecycle # hook are alterable WITHIN the hook so that
-userspace code can alter the behavior of the lifecycle # based on app level
-concerns. This allows apps to do things like: hash a user password, force
-certain # relationships to always exist, force "many" queries to obey sensible
-limits, commit log entries, # send messages to queues for processing based on
-CRUD events, or generally handle unforseen # circumstances.
-lifecycle_before_create: Callable[..., Coroutine[Any, Any, Any]] | None = None,
-lifecycle_after_create: Callable[..., Coroutine[Any, Any, Any]] | None = None,
-lifecycle_before_update: Callable[..., Coroutine[Any, Any, Any]] | None = None,
-lifecycle_after_update: Callable[..., Coroutine[Any, Any, Any]] | None = None,
-lifecycle_before_delete: Callable[..., Coroutine[Any, Any, Any]] | None = None,
-lifecycle_after_delete: Callable[..., Coroutine[Any, Any, Any]] | None = None,
-lifecycle_before_get_one: Callable[..., Coroutine[Any, Any, Any]] | None =
-None, lifecycle_after_get_one: Callable[..., Coroutine[Any, Any, Any]] | None =
-None, lifecycle_before_get_all: Callable[..., Coroutine[Any, Any, Any]] | None
-= None, lifecycle_after_get_all: Callable[..., Coroutine[Any, Any, Any]] | None
-= None, lifecycle_before_set_relations: Callable[..., Coroutine[Any, Any, Any]]
-| None = None, lifecycle_after_set_relations: Callable[..., Coroutine[Any, Any,
+bool = False, disable_get_many: bool = False, # The
+disable_relationship_getters list allow app developers to instruct the
+framework to NOT hoist # an automatic GET route for a list of specific named
+relationships. Note, that any relationship name # you disable will also cause
+the corresponding "link" entry that would point out that relationship # to be
+removed from Swagger documentation, as well as from any returned link objects
+in real-world # response payloads. This would effectively make a relationship
+invisble in GET routing. disable_relationship_getters: list[str] = [], # The
+disable_nested_objects flag prevents users from sending dictionaries inside of
+relationship arrays # which the server will automatically unpack by default
+into an attempted create or update of the related # resource. Any nested
+objects sent will still flow through the entire policy chain of the target
+resource! # Any dictionary send with a primary key field will be handled as if
+it is an update. To create a new # object via an embedded relationship, send
+the nested object without a primary key set! disable_nested_objects: bool =
+False, # Default limit will only set a limit on incoming queries if the user
+DOES NOT specify one. You should # implement POLICIES to enforce a MAX limit,
+as you will ultimately have to re-use any max limit # policies in your own
+custom controller functions for consistency. Max limit policies can be
+implemented # by overriding any limit query parameter sent by the user with a
+maximum number if the user value is # above whatever the max limit should be.
+default_limit: int = 10, # 'controller_extension' is the mount point for user-
+defined actions to-be-added to this resource's # controller/router. Pass in
+your class definition and it will be instantiated at the appropriate # time!
+See "CruddyController" example below! controller_extension: CruddyController =
+None, # 'custom_sql_identity_function' is an insertion point where you can pass
+in a lambda function or # other SYNCHRONOUS callable that will return some
+sqlalchemy query segment that determines the identity # of the resource in
+question. This is used for any CRUD actions that need to determine the identity
+# of a single record. Your lambda function / callable will be passed the {id}
+param from the controller. # You can use this to enable things like composite
+keys, and use {id} to capture .. custom_sql_identity_function: Callable[...,
+Any] | None = None, # 'custom_link_identity' is similar to
+custom_sql_identity_function, but is used specifically for building # the {id}
+segment of a 'link' value in the response JSON. The custom_link_identity
+function you pass in # will receive a record's value dictionary, which you can
+use to build a custom link {id} segment if needed. # You can use this to enable
+things like composite keys, and format {id} as .. custom_link_identity:
+Callable[..., str] | None = None, # The following REPOSITORY lifecycle hooks
+can each recieve an async function which will be invoked # before or after the
+target lifecycle event. Generally, whatever values are passed to the lifecycle
+# hook are alterable WITHIN the hook so that userspace code can alter the
+behavior of the lifecycle # based on app level concerns. This allows apps to do
+things like: hash a user password, force certain # relationships to always
+exist, force "many" queries to obey sensible limits, commit log entries, # send
+messages to queues for processing based on CRUD events, or generally handle
+unforseen # circumstances. lifecycle_before_create: Callable[..., Coroutine
+[Any, Any, Any]] | None = None, lifecycle_after_create: Callable[..., Coroutine
+[Any, Any, Any]] | None = None, lifecycle_before_update: Callable[...,
+Coroutine[Any, Any, Any]] | None = None, lifecycle_after_update: Callable[...,
+Coroutine[Any, Any, Any]] | None = None, lifecycle_before_delete: Callable[...,
+Coroutine[Any, Any, Any]] | None = None, lifecycle_after_delete: Callable[...,
+Coroutine[Any, Any, Any]] | None = None, lifecycle_before_get_one: Callable
+[..., Coroutine[Any, Any, Any]] | None = None, lifecycle_after_get_one:
+Callable[..., Coroutine[Any, Any, Any]] | None = None,
+lifecycle_before_get_all: Callable[..., Coroutine[Any, Any, Any]] | None =
+None, lifecycle_after_get_all: Callable[..., Coroutine[Any, Any, Any]] | None =
+None, lifecycle_before_set_relations: Callable[..., Coroutine[Any, Any, Any]] |
+None = None, lifecycle_after_set_relations: Callable[..., Coroutine[Any, Any,
 Any]] | None = None, # The following CONTROLLER lifecycle hooks can each
 recieve an async function which will be invoked # before or after the target
 lifecycle event. Generally, whatever values are passed to the lifecycle # hook
 are alterable WITHIN the hook so that userspace code can alter the behavior of
 the lifecycle # based on app level concerns. CONTROLLER lifecycles hooks will
 also receive the REQUEST context, # allowing the hook to take actions that
 consider the user and their priveleges, while still # interleaving that logic
```

