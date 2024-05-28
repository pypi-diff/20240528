# Comparing `tmp/answerrocket_client-0.2.7.tar.gz` & `tmp/answerrocket_client-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "answerrocket_client-0.2.7.tar", last modified: Thu May 23 19:17:19 2024, max compression
+gzip compressed data, was "answerrocket_client-0.2.8.tar", last modified: Tue May 28 21:17:25 2024, max compression
```

## Comparing `answerrocket_client-0.2.7.tar` & `answerrocket_client-0.2.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:19.255149 answerrocket_client-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-23 19:17:19.255149 answerrocket_client-0.2.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:19.255149 answerrocket_client-0.2.7/answer_rocket/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    16137 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    19766 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/data.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:19.255149 answerrocket_client-0.2.7/answer_rocket/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/graphql/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    52290 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/graphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/graphql/sdk_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/skill.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/answer_rocket/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:19.255149 answerrocket_client-0.2.7/answerrocket_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-23 19:17:19.000000 answerrocket_client-0.2.7/answerrocket_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-23 19:17:19.000000 answerrocket_client-0.2.7/answerrocket_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:17:19.000000 answerrocket_client-0.2.7/answerrocket_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-23 19:17:19.000000 answerrocket_client-0.2.7/answerrocket_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 19:17:19.000000 answerrocket_client-0.2.7/answerrocket_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 19:17:19.255149 answerrocket_client-0.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:17:19.255149 answerrocket_client-0.2.7/test/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-23 19:17:15.000000 answerrocket_client-0.2.7/test/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:17:25.611218 answerrocket_client-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-28 21:17:25.611218 answerrocket_client-0.2.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:17:25.611218 answerrocket_client-0.2.8/answer_rocket/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-28 21:17:19.000000 answerrocket_client-0.2.8/answer_rocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-28 21:17:19.000000 answerrocket_client-0.2.8/answer_rocket/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16137 2024-05-28 21:17:19.000000 answerrocket_client-0.2.8/answer_rocket/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-28 21:17:19.000000 answerrocket_client-0.2.8/answer_rocket/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13228 2024-05-28 21:17:19.000000 answerrocket_client-0.2.8/answer_rocket/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19766 2024-05-28 21:17:19.000000 answerrocket_client-0.2.8/answer_rocket/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 21:17:19.000000 answerrocket_client-0.2.8/answer_rocket/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:17:25.611218 answerrocket_client-0.2.8/answer_rocket/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:17:19.000000 answerrocket_client-0.2.8/answer_rocket/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-28 21:17:19.000000 answerrocket_client-0.2.8/answer_rocket/graphql/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52407 2024-05-28 21:17:19.000000 answerrocket_client-0.2.8/answer_rocket/graphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-05-28 21:17:19.000000 answerrocket_client-0.2.8/answer_rocket/graphql/sdk_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-05-28 21:17:19.000000 answerrocket_client-0.2.8/answer_rocket/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-28 21:17:19.000000 answerrocket_client-0.2.8/answer_rocket/skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-28 21:17:19.000000 answerrocket_client-0.2.8/answer_rocket/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:17:25.611218 answerrocket_client-0.2.8/answerrocket_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-28 21:17:25.000000 answerrocket_client-0.2.8/answerrocket_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-28 21:17:25.000000 answerrocket_client-0.2.8/answerrocket_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 21:17:25.000000 answerrocket_client-0.2.8/answerrocket_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-28 21:17:25.000000 answerrocket_client-0.2.8/answerrocket_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-28 21:17:25.000000 answerrocket_client-0.2.8/answerrocket_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-28 21:17:19.000000 answerrocket_client-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-28 21:17:19.000000 answerrocket_client-0.2.8/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 21:17:25.611218 answerrocket_client-0.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:17:25.611218 answerrocket_client-0.2.8/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-28 21:17:19.000000 answerrocket_client-0.2.8/test/test_client.py
```

### Comparing `answerrocket_client-0.2.7/PKG-INFO` & `answerrocket_client-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: answerrocket-client
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python client for interacting with AnswerRocket's skill API
 Requires-Python: >=3.10.7
 Description-Content-Type: text/markdown
 Requires-Dist: sgqlc
 Requires-Dist: openai
 Requires-Dist: pandas>=1.5.1
 Requires-Dist: typing-extensions
```

### Comparing `answerrocket_client-0.2.7/answer_rocket/auth.py` & `answerrocket_client-0.2.8/answer_rocket/auth.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.7/answer_rocket/chat.py` & `answerrocket_client-0.2.8/answer_rocket/chat.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.7/answer_rocket/client.py` & `answerrocket_client-0.2.8/answer_rocket/client.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.7/answer_rocket/config.py` & `answerrocket_client-0.2.8/answer_rocket/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from typing import Optional
 from uuid import UUID
 
+from answer_rocket.graphql.sdk_operations import Operations
 from sgqlc.types import Variable, Arg, non_null, String
 
 from answer_rocket.auth import AuthHelper
 from answer_rocket.graphql.client import GraphQlClient
 from answer_rocket.graphql.schema import UUID as GQL_UUID, MaxCopilotSkillChatQuestion, MaxCopilotSkill, MaxCopilot, \
     MaxMutationResponse, CreateMaxCopilotSkillChatQuestionResponse, MaxCopilotQuestionInput, \
     MaxCreateCopilotQuestionResponse, MaxUser, MaxSkillComponent
@@ -93,31 +94,19 @@
     def get_copilot_skill(self) -> MaxCopilotSkill:
         try:
             query_args = {
                 'copilotId': self.copilot_id,
                 'copilotSkillId': self.copilot_skill_id,
             }
 
-            query_vars = {
-                'copilot_id': Arg(non_null(GQL_UUID)),
-                'copilot_skill_id': Arg(non_null(GQL_UUID)),
-            }
-
-            operation = self._gql_client.query(variables=query_vars)
-
-            gql_query = operation.get_copilot_skill(
-                copilot_id=Variable('copilot_id'),
-                copilot_skill_id=Variable('copilot_skill_id'),
-            )
-
-            result = self._gql_client.submit(operation, query_args)
+            op = Operations.query.get_copilot_skill
 
-            max_copilot_skill = result.get_copilot_skill
+            result = self._gql_client.submit(op, query_args)
 
-            return max_copilot_skill
+            return result.get_copilot_skill
         except Exception as e:
             return None
 
     def get_skill_components(self) -> [MaxSkillComponent]:
         try:
             query_args = {
             }
```

### Comparing `answerrocket_client-0.2.7/answer_rocket/data.py` & `answerrocket_client-0.2.8/answer_rocket/data.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.7/answer_rocket/graphql/client.py` & `answerrocket_client-0.2.8/answer_rocket/graphql/client.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.7/answer_rocket/graphql/schema.py` & `answerrocket_client-0.2.8/answer_rocket/graphql/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,15 +370,16 @@
     description = sgqlc.types.Field(String, graphql_name='description')
     user_data = sgqlc.types.Field(JSON, graphql_name='userData')
     node_connections = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('MaxCopilotSkillNodeConnection'))), graphql_name='nodeConnections')
 
 
 class MaxCopilotSkillNodeConnection(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('source_node_id', 'output_property')
+    __field_names__ = ('input_property', 'source_node_id', 'output_property')
+    input_property = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='inputProperty')
     source_node_id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='sourceNodeId')
     output_property = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='outputProperty')
 
 
 class MaxCreateCopilotQuestionResponse(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('copilot_question_id', 'success', 'code', 'errors')
```

### Comparing `answerrocket_client-0.2.7/answer_rocket/output.py` & `answerrocket_client-0.2.8/answer_rocket/output.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.7/answer_rocket/skill.py` & `answerrocket_client-0.2.8/answer_rocket/skill.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.7/answerrocket_client.egg-info/PKG-INFO` & `answerrocket_client-0.2.8/answerrocket_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: answerrocket-client
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python client for interacting with AnswerRocket's skill API
 Requires-Python: >=3.10.7
 Description-Content-Type: text/markdown
 Requires-Dist: sgqlc
 Requires-Dist: openai
 Requires-Dist: pandas>=1.5.1
 Requires-Dist: typing-extensions
```

### Comparing `answerrocket_client-0.2.7/answerrocket_client.egg-info/SOURCES.txt` & `answerrocket_client-0.2.8/answerrocket_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.7/readme.md` & `answerrocket_client-0.2.8/readme.md`

 * *Files identical despite different names*

