# Comparing `tmp/littlehorse_client-0.9.0.tar.gz` & `tmp/littlehorse_client-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "littlehorse_client-0.9.0.tar", max compression
+gzip compressed data, was "littlehorse_client-0.9.1.tar", max compression
```

## Comparing `littlehorse_client-0.9.0.tar` & `littlehorse_client-0.9.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      860 2024-05-14 20:00:04.504316 littlehorse_client-0.9.0/README.md
--rw-r--r--   0        0        0      648 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/__init__.py
--rw-r--r--   0        0        0     5262 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/auth.py
--rw-r--r--   0        0        0    13731 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/config.py
--rw-r--r--   0        0        0      868 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/exceptions.py
--rw-r--r--   0        0        0     4676 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/acls_pb2.py
--rw-r--r--   0        0        0     5206 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/acls_pb2.pyi
--rw-r--r--   0        0        0     3031 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/common_enums_pb2.py
--rw-r--r--   0        0        0     3194 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/common_enums_pb2.pyi
--rw-r--r--   0        0        0     6656 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/common_wfspec_pb2.py
--rw-r--r--   0        0        0     8613 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/common_wfspec_pb2.pyi
--rw-r--r--   0        0        0     2583 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/external_event_pb2.py
--rw-r--r--   0        0        0     2248 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/external_event_pb2.pyi
--rw-r--r--   0        0        0     7014 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/node_run_pb2.py
--rw-r--r--   0        0        0     9762 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/node_run_pb2.pyi
--rw-r--r--   0        0        0     5304 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/object_id_pb2.py
--rw-r--r--   0        0        0     6398 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/object_id_pb2.pyi
--rw-r--r--   0        0        0    36601 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/service_pb2.py
--rw-r--r--   0        0        0    43385 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/service_pb2.pyi
--rw-r--r--   0        0        0    96335 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/service_pb2_grpc.py
--rw-r--r--   0        0        0     1687 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/task_def_pb2.py
--rw-r--r--   0        0        0     1151 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/task_def_pb2.pyi
--rw-r--r--   0        0        0     4867 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/task_run_pb2.py
--rw-r--r--   0        0        0     6233 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/task_run_pb2.pyi
--rw-r--r--   0        0        0     7136 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/user_tasks_pb2.py
--rw-r--r--   0        0        0     8973 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/user_tasks_pb2.pyi
--rw-r--r--   0        0        0     2120 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/variable_pb2.py
--rw-r--r--   0        0        0     1807 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/variable_pb2.pyi
--rw-r--r--   0        0        0     6480 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/wf_run_pb2.py
--rw-r--r--   0        0        0     9647 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/wf_run_pb2.pyi
--rw-r--r--   0        0        0    14804 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/wf_spec_pb2.py
--rw-r--r--   0        0        0    20694 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/wf_spec_pb2.pyi
--rw-r--r--   0        0        0     2150 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/workflow_event_pb2.py
--rw-r--r--   0        0        0     1643 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/workflow_event_pb2.pyi
--rw-r--r--   0        0        0     5539 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/utils.py
--rw-r--r--   0        0        0    22629 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/worker.py
--rw-r--r--   0        0        0    69098 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/workflow.py
--rw-r--r--   0        0        0     1343 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1940 1970-01-01 00:00:00.000000 littlehorse_client-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      860 2024-05-27 22:49:46.846199 littlehorse_client-0.9.1/README.md
+-rw-r--r--   0        0        0      648 2024-05-27 22:49:46.846199 littlehorse_client-0.9.1/littlehorse/__init__.py
+-rw-r--r--   0        0        0     5262 2024-05-27 22:49:46.846199 littlehorse_client-0.9.1/littlehorse/auth.py
+-rw-r--r--   0        0        0    13731 2024-05-27 22:49:46.846199 littlehorse_client-0.9.1/littlehorse/config.py
+-rw-r--r--   0        0        0      868 2024-05-27 22:49:46.846199 littlehorse_client-0.9.1/littlehorse/exceptions.py
+-rw-r--r--   0        0        0     4709 2024-05-27 22:49:46.846199 littlehorse_client-0.9.1/littlehorse/model/acls_pb2.py
+-rw-r--r--   0        0        0     5270 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/acls_pb2.pyi
+-rw-r--r--   0        0        0     3031 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/common_enums_pb2.py
+-rw-r--r--   0        0        0     3194 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/common_enums_pb2.pyi
+-rw-r--r--   0        0        0     6656 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/common_wfspec_pb2.py
+-rw-r--r--   0        0        0     8613 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/common_wfspec_pb2.pyi
+-rw-r--r--   0        0        0     2583 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/external_event_pb2.py
+-rw-r--r--   0        0        0     2248 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/external_event_pb2.pyi
+-rw-r--r--   0        0        0     7014 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/node_run_pb2.py
+-rw-r--r--   0        0        0     9762 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/node_run_pb2.pyi
+-rw-r--r--   0        0        0     5304 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/object_id_pb2.py
+-rw-r--r--   0        0        0     6398 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/object_id_pb2.pyi
+-rw-r--r--   0        0        0    36792 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/service_pb2.py
+-rw-r--r--   0        0        0    43385 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/service_pb2.pyi
+-rw-r--r--   0        0        0    99609 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/service_pb2_grpc.py
+-rw-r--r--   0        0        0     1687 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/task_def_pb2.py
+-rw-r--r--   0        0        0     1151 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/task_def_pb2.pyi
+-rw-r--r--   0        0        0     4867 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/task_run_pb2.py
+-rw-r--r--   0        0        0     6233 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/task_run_pb2.pyi
+-rw-r--r--   0        0        0     7136 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/user_tasks_pb2.py
+-rw-r--r--   0        0        0     8973 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/user_tasks_pb2.pyi
+-rw-r--r--   0        0        0     2120 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/variable_pb2.py
+-rw-r--r--   0        0        0     1807 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/variable_pb2.pyi
+-rw-r--r--   0        0        0     6480 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/wf_run_pb2.py
+-rw-r--r--   0        0        0     9647 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/wf_run_pb2.pyi
+-rw-r--r--   0        0        0    14804 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/wf_spec_pb2.py
+-rw-r--r--   0        0        0    20694 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/wf_spec_pb2.pyi
+-rw-r--r--   0        0        0     2150 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/workflow_event_pb2.py
+-rw-r--r--   0        0        0     1643 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/model/workflow_event_pb2.pyi
+-rw-r--r--   0        0        0     5539 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/utils.py
+-rw-r--r--   0        0        0    22629 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/worker.py
+-rw-r--r--   0        0        0    69098 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/littlehorse/workflow.py
+-rw-r--r--   0        0        0     1343 2024-05-27 22:49:46.850199 littlehorse_client-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1940 1970-01-01 00:00:00.000000 littlehorse_client-0.9.1/PKG-INFO
```

### Comparing `littlehorse_client-0.9.0/README.md` & `littlehorse_client-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/__init__.py` & `littlehorse_client-0.9.1/littlehorse/__init__.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/auth.py` & `littlehorse_client-0.9.1/littlehorse/auth.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/config.py` & `littlehorse_client-0.9.1/littlehorse/config.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/exceptions.py` & `littlehorse_client-0.9.1/littlehorse/exceptions.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/acls_pb2.py` & `littlehorse_client-0.9.1/littlehorse/model/acls_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 import littlehorse.model.object_id_pb2 as object__id__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\nacls.proto\x12\x0blittlehorse\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x0fobject_id.proto\"\xa2\x02\n\tPrincipal\x12$\n\x02id\x18\x01 \x01(\x0b\x32\x18.littlehorse.PrincipalId\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x42\n\x0fper_tenant_acls\x18\x03 \x03(\x0b\x32).littlehorse.Principal.PerTenantAclsEntry\x12,\n\x0bglobal_acls\x18\x04 \x01(\x0b\x32\x17.littlehorse.ServerACLs\x1aM\n\x12PerTenantAclsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.littlehorse.ServerACLs:\x02\x38\x01\"[\n\x06Tenant\x12!\n\x02id\x18\x01 \x01(\x0b\x32\x15.littlehorse.TenantId\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"2\n\nServerACLs\x12$\n\x04\x61\x63ls\x18\x01 \x03(\x0b\x32\x16.littlehorse.ServerACL\"\x9e\x01\n\tServerACL\x12+\n\tresources\x18\x01 \x03(\x0e\x32\x18.littlehorse.ACLResource\x12/\n\x0f\x61llowed_actions\x18\x02 \x03(\x0e\x32\x16.littlehorse.ACLAction\x12\x0e\n\x04name\x18\x03 \x01(\tH\x00\x12\x10\n\x06prefix\x18\x04 \x01(\tH\x00\x42\x11\n\x0fresource_filter\"\xff\x01\n\x13PutPrincipalRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12L\n\x0fper_tenant_acls\x18\x02 \x03(\x0b\x32\x33.littlehorse.PutPrincipalRequest.PerTenantAclsEntry\x12,\n\x0bglobal_acls\x18\x03 \x01(\x0b\x32\x17.littlehorse.ServerACLs\x12\x11\n\toverwrite\x18\x05 \x01(\x08\x1aM\n\x12PerTenantAclsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.littlehorse.ServerACLs:\x02\x38\x01\"$\n\x16\x44\x65letePrincipalRequest\x12\n\n\x02id\x18\x01 \x01(\t\"\x1e\n\x10PutTenantRequest\x12\n\n\x02id\x18\x01 \x01(\t*\xad\x01\n\x0b\x41\x43LResource\x12\x10\n\x0c\x41\x43L_WORKFLOW\x10\x00\x12\x0c\n\x08\x41\x43L_TASK\x10\x01\x12\x16\n\x12\x41\x43L_EXTERNAL_EVENT\x10\x02\x12\x11\n\rACL_USER_TASK\x10\x03\x12\x11\n\rACL_PRINCIPAL\x10\x04\x12\x0e\n\nACL_TENANT\x10\x05\x12\x15\n\x11\x41\x43L_ALL_RESOURCES\x10\x06\x12\x19\n\x15\x41\x43L_TASK_WORKER_GROUP\x10\x07*C\n\tACLAction\x12\x08\n\x04READ\x10\x00\x12\x07\n\x03RUN\x10\x01\x12\x12\n\x0eWRITE_METADATA\x10\x02\x12\x0f\n\x0b\x41LL_ACTIONS\x10\x03\x42G\n\x1fio.littlehorse.sdk.common.protoP\x01Z\x07.;model\xaa\x02\x18LittleHorse.Common.Protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\nacls.proto\x12\x0blittlehorse\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x0fobject_id.proto\"\xa2\x02\n\tPrincipal\x12$\n\x02id\x18\x01 \x01(\x0b\x32\x18.littlehorse.PrincipalId\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x42\n\x0fper_tenant_acls\x18\x03 \x03(\x0b\x32).littlehorse.Principal.PerTenantAclsEntry\x12,\n\x0bglobal_acls\x18\x04 \x01(\x0b\x32\x17.littlehorse.ServerACLs\x1aM\n\x12PerTenantAclsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.littlehorse.ServerACLs:\x02\x38\x01\"[\n\x06Tenant\x12!\n\x02id\x18\x01 \x01(\x0b\x32\x15.littlehorse.TenantId\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"2\n\nServerACLs\x12$\n\x04\x61\x63ls\x18\x01 \x03(\x0b\x32\x16.littlehorse.ServerACL\"\x9e\x01\n\tServerACL\x12+\n\tresources\x18\x01 \x03(\x0e\x32\x18.littlehorse.ACLResource\x12/\n\x0f\x61llowed_actions\x18\x02 \x03(\x0e\x32\x16.littlehorse.ACLAction\x12\x0e\n\x04name\x18\x03 \x01(\tH\x00\x12\x10\n\x06prefix\x18\x04 \x01(\tH\x00\x42\x11\n\x0fresource_filter\"\xff\x01\n\x13PutPrincipalRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12L\n\x0fper_tenant_acls\x18\x02 \x03(\x0b\x32\x33.littlehorse.PutPrincipalRequest.PerTenantAclsEntry\x12,\n\x0bglobal_acls\x18\x03 \x01(\x0b\x32\x17.littlehorse.ServerACLs\x12\x11\n\toverwrite\x18\x05 \x01(\x08\x1aM\n\x12PerTenantAclsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.littlehorse.ServerACLs:\x02\x38\x01\">\n\x16\x44\x65letePrincipalRequest\x12$\n\x02id\x18\x01 \x01(\x0b\x32\x18.littlehorse.PrincipalId\"\x1e\n\x10PutTenantRequest\x12\n\n\x02id\x18\x01 \x01(\t*\xad\x01\n\x0b\x41\x43LResource\x12\x10\n\x0c\x41\x43L_WORKFLOW\x10\x00\x12\x0c\n\x08\x41\x43L_TASK\x10\x01\x12\x16\n\x12\x41\x43L_EXTERNAL_EVENT\x10\x02\x12\x11\n\rACL_USER_TASK\x10\x03\x12\x11\n\rACL_PRINCIPAL\x10\x04\x12\x0e\n\nACL_TENANT\x10\x05\x12\x15\n\x11\x41\x43L_ALL_RESOURCES\x10\x06\x12\x19\n\x15\x41\x43L_TASK_WORKER_GROUP\x10\x07*C\n\tACLAction\x12\x08\n\x04READ\x10\x00\x12\x07\n\x03RUN\x10\x01\x12\x12\n\x0eWRITE_METADATA\x10\x02\x12\x0f\n\x0b\x41LL_ACTIONS\x10\x03\x42G\n\x1fio.littlehorse.sdk.common.protoP\x01Z\x07.;model\xaa\x02\x18LittleHorse.Common.Protob\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'acls_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\037io.littlehorse.sdk.common.protoP\001Z\007.;model\252\002\030LittleHorse.Common.Proto'
   _PRINCIPAL_PERTENANTACLSENTRY._options = None
   _PRINCIPAL_PERTENANTACLSENTRY._serialized_options = b'8\001'
   _PUTPRINCIPALREQUEST_PERTENANTACLSENTRY._options = None
   _PUTPRINCIPALREQUEST_PERTENANTACLSENTRY._serialized_options = b'8\001'
-  _globals['_ACLRESOURCE']._serialized_start=1005
-  _globals['_ACLRESOURCE']._serialized_end=1178
-  _globals['_ACLACTION']._serialized_start=1180
-  _globals['_ACLACTION']._serialized_end=1247
+  _globals['_ACLRESOURCE']._serialized_start=1031
+  _globals['_ACLRESOURCE']._serialized_end=1204
+  _globals['_ACLACTION']._serialized_start=1206
+  _globals['_ACLACTION']._serialized_end=1273
   _globals['_PRINCIPAL']._serialized_start=78
   _globals['_PRINCIPAL']._serialized_end=368
   _globals['_PRINCIPAL_PERTENANTACLSENTRY']._serialized_start=291
   _globals['_PRINCIPAL_PERTENANTACLSENTRY']._serialized_end=368
   _globals['_TENANT']._serialized_start=370
   _globals['_TENANT']._serialized_end=461
   _globals['_SERVERACLS']._serialized_start=463
@@ -43,11 +43,11 @@
   _globals['_SERVERACL']._serialized_start=516
   _globals['_SERVERACL']._serialized_end=674
   _globals['_PUTPRINCIPALREQUEST']._serialized_start=677
   _globals['_PUTPRINCIPALREQUEST']._serialized_end=932
   _globals['_PUTPRINCIPALREQUEST_PERTENANTACLSENTRY']._serialized_start=291
   _globals['_PUTPRINCIPALREQUEST_PERTENANTACLSENTRY']._serialized_end=368
   _globals['_DELETEPRINCIPALREQUEST']._serialized_start=934
-  _globals['_DELETEPRINCIPALREQUEST']._serialized_end=970
-  _globals['_PUTTENANTREQUEST']._serialized_start=972
-  _globals['_PUTTENANTREQUEST']._serialized_end=1002
+  _globals['_DELETEPRINCIPALREQUEST']._serialized_end=996
+  _globals['_PUTTENANTREQUEST']._serialized_start=998
+  _globals['_PUTTENANTREQUEST']._serialized_end=1028
 # @@protoc_insertion_point(module_scope)
```

### Comparing `littlehorse_client-0.9.0/littlehorse/model/acls_pb2.pyi` & `littlehorse_client-0.9.1/littlehorse/model/acls_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     global_acls: ServerACLs
     overwrite: bool
     def __init__(self, id: _Optional[str] = ..., per_tenant_acls: _Optional[_Mapping[str, ServerACLs]] = ..., global_acls: _Optional[_Union[ServerACLs, _Mapping]] = ..., overwrite: bool = ...) -> None: ...
 
 class DeletePrincipalRequest(_message.Message):
     __slots__ = ["id"]
     ID_FIELD_NUMBER: _ClassVar[int]
-    id: str
-    def __init__(self, id: _Optional[str] = ...) -> None: ...
+    id: _object_id_pb2.PrincipalId
+    def __init__(self, id: _Optional[_Union[_object_id_pb2.PrincipalId, _Mapping]] = ...) -> None: ...
 
 class PutTenantRequest(_message.Message):
     __slots__ = ["id"]
     ID_FIELD_NUMBER: _ClassVar[int]
     id: str
     def __init__(self, id: _Optional[str] = ...) -> None: ...
```

### Comparing `littlehorse_client-0.9.0/littlehorse/model/common_enums_pb2.py` & `littlehorse_client-0.9.1/littlehorse/model/common_enums_pb2.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/common_enums_pb2.pyi` & `littlehorse_client-0.9.1/littlehorse/model/common_enums_pb2.pyi`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/common_wfspec_pb2.py` & `littlehorse_client-0.9.1/littlehorse/model/common_wfspec_pb2.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/common_wfspec_pb2.pyi` & `littlehorse_client-0.9.1/littlehorse/model/common_wfspec_pb2.pyi`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/external_event_pb2.py` & `littlehorse_client-0.9.1/littlehorse/model/external_event_pb2.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/external_event_pb2.pyi` & `littlehorse_client-0.9.1/littlehorse/model/external_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/node_run_pb2.py` & `littlehorse_client-0.9.1/littlehorse/model/node_run_pb2.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/node_run_pb2.pyi` & `littlehorse_client-0.9.1/littlehorse/model/node_run_pb2.pyi`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/object_id_pb2.py` & `littlehorse_client-0.9.1/littlehorse/model/object_id_pb2.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/object_id_pb2.pyi` & `littlehorse_client-0.9.1/littlehorse/model/object_id_pb2.pyi`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/service_pb2.py` & `littlehorse_client-0.9.1/littlehorse/model/service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import littlehorse.model.user_tasks_pb2 as user__tasks__pb2
 import littlehorse.model.wf_spec_pb2 as wf__spec__pb2
 import littlehorse.model.task_def_pb2 as task__def__pb2
 import littlehorse.model.acls_pb2 as acls__pb2
 import littlehorse.model.workflow_event_pb2 as workflow__event__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rservice.proto\x12\x0blittlehorse\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x13\x63ommon_wfspec.proto\x1a\x12\x63ommon_enums.proto\x1a\x0fobject_id.proto\x1a\x0evariable.proto\x1a\x14\x65xternal_event.proto\x1a\x0cwf_run.proto\x1a\x0enode_run.proto\x1a\x0etask_run.proto\x1a\x10user_tasks.proto\x1a\rwf_spec.proto\x1a\x0etask_def.proto\x1a\nacls.proto\x1a\x14workflow_event.proto\"+\n\x1bGetLatestUserTaskDefRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xd3\x03\n\x10PutWfSpecRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x44\n\x0cthread_specs\x18\x05 \x03(\x0b\x32..littlehorse.PutWfSpecRequest.ThreadSpecsEntry\x12\x1e\n\x16\x65ntrypoint_thread_name\x18\x06 \x01(\t\x12\x43\n\x10retention_policy\x18\x08 \x01(\x0b\x32$.littlehorse.WorkflowRetentionPolicyH\x00\x88\x01\x01\x12\x46\n\x0eparent_wf_spec\x18\t \x01(\x0b\x32).littlehorse.WfSpec.ParentWfSpecReferenceH\x01\x88\x01\x01\x12\x37\n\x0f\x61llowed_updates\x18\n \x01(\x0e\x32\x1e.littlehorse.AllowedUpdateType\x1aK\n\x10ThreadSpecsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.littlehorse.ThreadSpec:\x02\x38\x01\x42\x13\n\x11_retention_policyB\x11\n\x0f_parent_wf_specJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05\"O\n\x11PutTaskDefRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12,\n\ninput_vars\x18\x02 \x03(\x0b\x32\x18.littlehorse.VariableDef\"S\n\x1aPutWorkflowEventDefRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\'\n\x04type\x18\x02 \x01(\x0e\x32\x19.littlehorse.VariableType\"{\n\x15PutUserTaskDefRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12*\n\x06\x66ields\x18\x02 \x03(\x0b\x32\x1a.littlehorse.UserTaskField\x12\x18\n\x0b\x64\x65scription\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\x0e\n\x0c_description\"o\n\x1aPutExternalEventDefRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x43\n\x10retention_policy\x18\x02 \x01(\x0b\x32).littlehorse.ExternalEventRetentionPolicy\"\xc3\x02\n\x17PutExternalEventRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\x12>\n\x15\x65xternal_event_def_id\x18\x02 \x01(\x0b\x32\x1f.littlehorse.ExternalEventDefId\x12\x11\n\x04guid\x18\x03 \x01(\tH\x00\x88\x01\x01\x12+\n\x07\x63ontent\x18\x05 \x01(\x0b\x32\x1a.littlehorse.VariableValue\x12\x1e\n\x11thread_run_number\x18\x06 \x01(\x05H\x01\x88\x01\x01\x12\x1e\n\x11node_run_position\x18\x07 \x01(\x05H\x02\x88\x01\x01\x42\x07\n\x05_guidB\x14\n\x12_thread_run_numberB\x14\n\x12_node_run_positionJ\x04\x08\x04\x10\x05J\x04\x08\x08\x10\t\"F\n\x1a\x44\x65leteExternalEventRequest\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.littlehorse.ExternalEventId\"6\n\x12\x44\x65leteWfRunRequest\x12 \n\x02id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\":\n\x14\x44\x65leteTaskDefRequest\x12\"\n\x02id\x18\x01 \x01(\x0b\x32\x16.littlehorse.TaskDefId\"B\n\x18\x44\x65leteUserTaskDefRequest\x12&\n\x02id\x18\x01 \x01(\x0b\x32\x1a.littlehorse.UserTaskDefId\"8\n\x13\x44\x65leteWfSpecRequest\x12!\n\x02id\x18\x01 \x01(\x0b\x32\x15.littlehorse.WfSpecId\"L\n\x1d\x44\x65leteExternalEventDefRequest\x12+\n\x02id\x18\x01 \x01(\x0b\x32\x1f.littlehorse.ExternalEventDefId\"\xe3\x02\n\x0cRunWfRequest\x12\x14\n\x0cwf_spec_name\x18\x01 \x01(\t\x12\x1a\n\rmajor_version\x18\x02 \x01(\x05H\x00\x88\x01\x01\x12\x15\n\x08revision\x18\x03 \x01(\x05H\x01\x88\x01\x01\x12;\n\tvariables\x18\x04 \x03(\x0b\x32(.littlehorse.RunWfRequest.VariablesEntry\x12\x0f\n\x02id\x18\x05 \x01(\tH\x02\x88\x01\x01\x12\x33\n\x10parent_wf_run_id\x18\x06 \x01(\x0b\x32\x14.littlehorse.WfRunIdH\x03\x88\x01\x01\x1aL\n\x0eVariablesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.littlehorse.VariableValue:\x02\x38\x01\x42\x10\n\x0e_major_versionB\x0b\n\t_revisionB\x05\n\x03_idB\x13\n\x11_parent_wf_run_id\"L\n\rVariableMatch\x12\x10\n\x08var_name\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.littlehorse.VariableValue\"\xbd\x01\n\x19\x41waitWorkflowEventRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\x12\x36\n\revent_def_ids\x18\x02 \x03(\x0b\x32\x1f.littlehorse.WorkflowEventDefId\x12?\n\x19workflow_events_to_ignore\x18\x03 \x03(\x0b\x32\x1c.littlehorse.WorkflowEventId\"\xdf\x03\n\x12SearchWfRunRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x14\n\x0cwf_spec_name\x18\x03 \x01(\t\x12\"\n\x15wf_spec_major_version\x18\x04 \x01(\x05H\x02\x88\x01\x01\x12\x1d\n\x10wf_spec_revision\x18\x05 \x01(\x05H\x03\x88\x01\x01\x12*\n\x06status\x18\x06 \x01(\x0e\x32\x15.littlehorse.LHStatusH\x04\x88\x01\x01\x12\x37\n\x0e\x65\x61rliest_start\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x05\x88\x01\x01\x12\x35\n\x0clatest_start\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x06\x88\x01\x01\x12\x34\n\x10variable_filters\x18\t \x03(\x0b\x32\x1a.littlehorse.VariableMatchB\x0b\n\t_bookmarkB\x08\n\x06_limitB\x18\n\x16_wf_spec_major_versionB\x13\n\x11_wf_spec_revisionB\t\n\x07_statusB\x11\n\x0f_earliest_startB\x0f\n\r_latest_start\"X\n\x0bWfRunIdList\x12%\n\x07results\x18\x01 \x03(\x0b\x32\x14.littlehorse.WfRunId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\xbc\x02\n\x14SearchTaskRunRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x15\n\rtask_def_name\x18\x03 \x01(\t\x12,\n\x06status\x18\x04 \x01(\x0e\x32\x17.littlehorse.TaskStatusH\x02\x88\x01\x01\x12\x37\n\x0e\x65\x61rliest_start\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x03\x88\x01\x01\x12\x35\n\x0clatest_start\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x04\x88\x01\x01\x42\x0b\n\t_bookmarkB\x08\n\x06_limitB\t\n\x07_statusB\x11\n\x0f_earliest_startB\x0f\n\r_latest_start\"\\\n\rTaskRunIdList\x12\'\n\x07results\x18\x01 \x03(\x0b\x32\x16.littlehorse.TaskRunId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\xf1\x03\n\x14SearchNodeRunRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x37\n\x0e\x65\x61rliest_start\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x02\x88\x01\x01\x12\x35\n\x0clatest_start\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x03\x88\x01\x01\x12=\n\tnode_type\x18\x05 \x01(\x0e\x32*.littlehorse.SearchNodeRunRequest.NodeType\x12%\n\x06status\x18\x06 \x01(\x0e\x32\x15.littlehorse.LHStatus\"\x9c\x01\n\x08NodeType\x12\x08\n\x04TASK\x10\x00\x12\x12\n\x0e\x45XTERNAL_EVENT\x10\x01\x12\x0e\n\nENTRYPOINT\x10\x02\x12\x08\n\x04\x45XIT\x10\x03\x12\x10\n\x0cSTART_THREAD\x10\x04\x12\x10\n\x0cWAIT_THREADS\x10\x05\x12\t\n\x05SLEEP\x10\x06\x12\r\n\tUSER_TASK\x10\x07\x12\x1a\n\x16START_MULTIPLE_THREADS\x10\x08\x42\x0b\n\t_bookmarkB\x08\n\x06_limitB\x11\n\x0f_earliest_startB\x0f\n\r_latest_start\"\\\n\rNodeRunIdList\x12\'\n\x07results\x18\x01 \x03(\x0b\x32\x16.littlehorse.NodeRunId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\xb2\x03\n\x18SearchUserTaskRunRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x33\n\x06status\x18\x03 \x01(\x0e\x32\x1e.littlehorse.UserTaskRunStatusH\x02\x88\x01\x01\x12\x1f\n\x12user_task_def_name\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x14\n\x07user_id\x18\x05 \x01(\tH\x04\x88\x01\x01\x12\x17\n\nuser_group\x18\x06 \x01(\tH\x05\x88\x01\x01\x12\x37\n\x0e\x65\x61rliest_start\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x06\x88\x01\x01\x12\x35\n\x0clatest_start\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x07\x88\x01\x01\x42\x0b\n\t_bookmarkB\x08\n\x06_limitB\t\n\x07_statusB\x15\n\x13_user_task_def_nameB\n\n\x08_user_idB\r\n\x0b_user_groupB\x11\n\x0f_earliest_startB\x0f\n\r_latest_start\"d\n\x11UserTaskRunIdList\x12+\n\x07results\x18\x01 \x03(\x0b\x32\x1a.littlehorse.UserTaskRunId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\x9e\x02\n\x15SearchVariableRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12)\n\x05value\x18\x03 \x01(\x0b\x32\x1a.littlehorse.VariableValue\x12\"\n\x15wf_spec_major_version\x18\x04 \x01(\x05H\x02\x88\x01\x01\x12\x1d\n\x10wf_spec_revision\x18\x05 \x01(\x05H\x03\x88\x01\x01\x12\x10\n\x08var_name\x18\x06 \x01(\t\x12\x14\n\x0cwf_spec_name\x18\x07 \x01(\tB\x0b\n\t_bookmarkB\x08\n\x06_limitB\x18\n\x16_wf_spec_major_versionB\x13\n\x11_wf_spec_revision\"^\n\x0eVariableIdList\x12(\n\x07results\x18\x01 \x03(\x0b\x32\x17.littlehorse.VariableId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"x\n\x14SearchTaskDefRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x13\n\x06prefix\x18\x03 \x01(\tH\x02\x88\x01\x01\x42\x0b\n\t_bookmarkB\x08\n\x06_limitB\t\n\x07_prefix\"\\\n\rTaskDefIdList\x12\'\n\x07results\x18\x01 \x03(\x0b\x32\x16.littlehorse.TaskDefId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\x98\x01\n\x18SearchUserTaskDefRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x01\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x02\x88\x01\x01\x12\x10\n\x06prefix\x18\x03 \x01(\tH\x00\x12\x0e\n\x04name\x18\x04 \x01(\tH\x00\x42\x18\n\x16user_task_def_criteriaB\x0b\n\t_bookmarkB\x08\n\x06_limit\"d\n\x11UserTaskDefIdList\x12+\n\x07results\x18\x01 \x03(\x0b\x32\x1a.littlehorse.UserTaskDefId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\xa6\x01\n\x13SearchWfSpecRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x01\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x02\x88\x01\x01\x12\x0e\n\x04name\x18\x03 \x01(\tH\x00\x12\x10\n\x06prefix\x18\x04 \x01(\tH\x00\x12\x17\n\rtask_def_name\x18\x05 \x01(\tH\x00\x42\x12\n\x10wf_spec_criteriaB\x0b\n\t_bookmarkB\x08\n\x06_limit\"Z\n\x0cWfSpecIdList\x12&\n\x07results\x18\x01 \x03(\x0b\x32\x15.littlehorse.WfSpecId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\x81\x01\n\x1dSearchExternalEventDefRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x13\n\x06prefix\x18\x03 \x01(\tH\x02\x88\x01\x01\x42\x0b\n\t_bookmarkB\x08\n\x06_limitB\t\n\x07_prefix\"n\n\x16\x45xternalEventDefIdList\x12\x30\n\x07results\x18\x01 \x03(\x0b\x32\x1f.littlehorse.ExternalEventDefId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"W\n\x13SearchTenantRequest\x12\x12\n\x05limit\x18\x01 \x01(\x05H\x00\x88\x01\x01\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x01\x88\x01\x01\x42\x08\n\x06_limitB\x0b\n\t_bookmark\"Z\n\x0cTenantIdList\x12&\n\x07results\x18\x01 \x03(\x0b\x32\x15.littlehorse.TenantId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\x80\x03\n\x1aSearchExternalEventRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x01\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x02\x88\x01\x01\x12)\n\twf_run_id\x18\x03 \x01(\x0b\x32\x14.littlehorse.WfRunIdH\x00\x12u\n\"external_event_def_name_and_status\x18\x04 \x01(\x0b\x32G.littlehorse.SearchExternalEventRequest.ByExtEvtDefNameAndStatusRequestH\x00\x1aj\n\x1f\x42yExtEvtDefNameAndStatusRequest\x12\x1f\n\x17\x65xternal_event_def_name\x18\x01 \x01(\t\x12\x17\n\nis_claimed\x18\x02 \x01(\x08H\x00\x88\x01\x01\x42\r\n\x0b_is_claimedB\x12\n\x10\x65xt_evt_criteriaB\x0b\n\t_bookmarkB\x08\n\x06_limit\"h\n\x13\x45xternalEventIdList\x12-\n\x07results\x18\x01 \x03(\x0b\x32\x1c.littlehorse.ExternalEventId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\xb6\x01\n\x13ListNodeRunsRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\x12\x1e\n\x11thread_run_number\x18\x02 \x01(\x05H\x00\x88\x01\x01\x12\x15\n\x08\x62ookmark\x18\x03 \x01(\x0cH\x01\x88\x01\x01\x12\x12\n\x05limit\x18\x04 \x01(\x05H\x02\x88\x01\x01\x42\x14\n\x12_thread_run_numberB\x0b\n\t_bookmarkB\x08\n\x06_limit\"X\n\x0bNodeRunList\x12%\n\x07results\x18\x01 \x03(\x0b\x32\x14.littlehorse.NodeRun\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"?\n\x14ListVariablesRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\"6\n\x0cVariableList\x12&\n\x07results\x18\x01 \x03(\x0b\x32\x15.littlehorse.Variable\"D\n\x19ListExternalEventsRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\"@\n\x11\x45xternalEventList\x12+\n\x07results\x18\x01 \x03(\x0b\x32\x1a.littlehorse.ExternalEvent\"w\n\x19RegisterTaskWorkerRequest\x12\x16\n\x0etask_worker_id\x18\x01 \x01(\t\x12+\n\x0btask_def_id\x18\x02 \x01(\x0b\x32\x16.littlehorse.TaskDefId\x12\x15\n\rlistener_name\x18\x03 \x01(\t\"s\n\x1aTaskWorkerHeartBeatRequest\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12+\n\x0btask_def_id\x18\x02 \x01(\x0b\x32\x16.littlehorse.TaskDefId\x12\x15\n\rlistener_name\x18\x03 \x01(\t\"\x81\x01\n\x1aRegisterTaskWorkerResponse\x12+\n\nyour_hosts\x18\x01 \x03(\x0b\x32\x17.littlehorse.LHHostInfo\x12\x1f\n\x12is_cluster_healthy\x18\x02 \x01(\x08H\x00\x88\x01\x01\x42\x15\n\x13_is_cluster_healthy\"(\n\nLHHostInfo\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"\x8b\x01\n\x0fPollTaskRequest\x12+\n\x0btask_def_id\x18\x01 \x01(\x0b\x32\x16.littlehorse.TaskDefId\x12\x11\n\tclient_id\x18\x02 \x01(\t\x12 \n\x13task_worker_version\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\x16\n\x14_task_worker_version\"\x8c\x02\n\rScheduledTask\x12+\n\x0btask_run_id\x18\x01 \x01(\x0b\x32\x16.littlehorse.TaskRunId\x12+\n\x0btask_def_id\x18\x02 \x01(\x0b\x32\x16.littlehorse.TaskDefId\x12\x16\n\x0e\x61ttempt_number\x18\x03 \x01(\x05\x12-\n\tvariables\x18\x04 \x03(\x0b\x32\x1a.littlehorse.VarNameAndVal\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x06source\x18\x06 \x01(\x0b\x32\x1a.littlehorse.TaskRunSource\"N\n\x10PollTaskResponse\x12/\n\x06result\x18\x01 \x01(\x0b\x32\x1a.littlehorse.ScheduledTaskH\x00\x88\x01\x01\x42\t\n\x07_result\"\x81\x03\n\rReportTaskRun\x12+\n\x0btask_run_id\x18\x01 \x01(\x0b\x32\x16.littlehorse.TaskRunId\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\x06status\x18\x03 \x01(\x0e\x32\x17.littlehorse.TaskStatus\x12\x33\n\nlog_output\x18\x05 \x01(\x0b\x32\x1a.littlehorse.VariableValueH\x01\x88\x01\x01\x12\x16\n\x0e\x61ttempt_number\x18\x06 \x01(\x05\x12,\n\x06output\x18\x04 \x01(\x0b\x32\x1a.littlehorse.VariableValueH\x00\x12)\n\x05\x65rror\x18\x07 \x01(\x0b\x32\x18.littlehorse.LHTaskErrorH\x00\x12\x31\n\texception\x18\x08 \x01(\x0b\x32\x1c.littlehorse.LHTaskExceptionH\x00\x42\x08\n\x06resultB\r\n\x0b_log_output\"V\n\x10StopWfRunRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\x12\x19\n\x11thread_run_number\x18\x02 \x01(\x05\"X\n\x12ResumeWfRunRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\x12\x19\n\x11thread_run_number\x18\x02 \x01(\x05\"\xb3\x01\n\x1aTaskDefMetricsQueryRequest\x12\x30\n\x0cwindow_start\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x0bwindow_type\x18\x02 \x01(\x0e\x32 .littlehorse.MetricsWindowLength\x12\x1a\n\rtask_def_name\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\x10\n\x0e_task_def_name\"\xca\x01\n\x16ListTaskMetricsRequest\x12+\n\x0btask_def_id\x18\x01 \x01(\x0b\x32\x16.littlehorse.TaskDefId\x12\x35\n\x11last_window_start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\rwindow_length\x18\x03 \x01(\x0e\x32 .littlehorse.MetricsWindowLength\x12\x13\n\x0bnum_windows\x18\x04 \x01(\x05\"G\n\x17ListTaskMetricsResponse\x12,\n\x07results\x18\x01 \x03(\x0b\x32\x1b.littlehorse.TaskDefMetrics\"\xb1\x01\n\x19WfSpecMetricsQueryRequest\x12)\n\nwf_spec_id\x18\x01 \x01(\x0b\x32\x15.littlehorse.WfSpecId\x12\x30\n\x0cwindow_start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\rwindow_length\x18\x03 \x01(\x0e\x32 .littlehorse.MetricsWindowLength\"\xc6\x01\n\x14ListWfMetricsRequest\x12)\n\nwf_spec_id\x18\x01 \x01(\x0b\x32\x15.littlehorse.WfSpecId\x12\x35\n\x11last_window_start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\rwindow_length\x18\x03 \x01(\x0e\x32 .littlehorse.MetricsWindowLength\x12\x13\n\x0bnum_windows\x18\x04 \x01(\x05\"D\n\x15ListWfMetricsResponse\x12+\n\x07results\x18\x01 \x03(\x0b\x32\x1a.littlehorse.WfSpecMetrics\"\xfb\x02\n\x0eTaskDefMetrics\x12+\n\x0btask_def_id\x18\x01 \x01(\x0b\x32\x16.littlehorse.TaskDefId\x12\x30\n\x0cwindow_start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\x04type\x18\x03 \x01(\x0e\x32 .littlehorse.MetricsWindowLength\x12\x1d\n\x15schedule_to_start_max\x18\x04 \x01(\x03\x12\x1d\n\x15schedule_to_start_avg\x18\x05 \x01(\x03\x12\x1d\n\x15start_to_complete_max\x18\x06 \x01(\x03\x12\x1d\n\x15start_to_complete_avg\x18\x07 \x01(\x03\x12\x17\n\x0ftotal_completed\x18\x08 \x01(\x03\x12\x15\n\rtotal_errored\x18\t \x01(\x03\x12\x15\n\rtotal_started\x18\n \x01(\x03\x12\x17\n\x0ftotal_scheduled\x18\x0b \x01(\x03\"\xa1\x02\n\rWfSpecMetrics\x12)\n\nwf_spec_id\x18\x01 \x01(\x0b\x32\x15.littlehorse.WfSpecId\x12\x30\n\x0cwindow_start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\x04type\x18\x03 \x01(\x0e\x32 .littlehorse.MetricsWindowLength\x12\x15\n\rtotal_started\x18\x04 \x01(\x03\x12\x17\n\x0ftotal_completed\x18\x05 \x01(\x03\x12\x15\n\rtotal_errored\x18\x06 \x01(\x03\x12\x1d\n\x15start_to_complete_max\x18\x07 \x01(\x03\x12\x1d\n\x15start_to_complete_avg\x18\x08 \x01(\x03\"A\n\x16ListUserTaskRunRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\"<\n\x0fUserTaskRunList\x12)\n\x07results\x18\x01 \x03(\x0b\x32\x18.littlehorse.UserTaskRun\"\x8a\x01\n\x12TaskWorkerMetadata\x12\x16\n\x0etask_worker_id\x18\x01 \x01(\t\x12\x34\n\x10latest_heartbeat\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12&\n\x05hosts\x18\x03 \x03(\x0b\x32\x17.littlehorse.LHHostInfo\"\x87\x02\n\x0fTaskWorkerGroup\x12*\n\x02id\x18\x01 \x01(\x0b\x32\x1e.littlehorse.TaskWorkerGroupId\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x43\n\x0ctask_workers\x18\x03 \x03(\x0b\x32-.littlehorse.TaskWorkerGroup.TaskWorkersEntry\x1aS\n\x10TaskWorkersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12.\n\x05value\x18\x02 \x01(\x0b\x32\x1f.littlehorse.TaskWorkerMetadata:\x02\x38\x01\">\n\x13ListTaskRunsRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\"4\n\x0bTaskRunList\x12%\n\x07results\x18\x01 \x03(\x0b\x32\x14.littlehorse.TaskRun\"z\n\x14MigrateWfSpecRequest\x12*\n\x0bold_wf_spec\x18\x01 \x01(\x0b\x32\x15.littlehorse.WfSpecId\x12\x36\n\tmigration\x18\x02 \x01(\x0b\x32#.littlehorse.WfSpecVersionMigration\"T\n\x16GetLatestWfSpecRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1a\n\rmajor_version\x18\x02 \x01(\x05H\x00\x88\x01\x01\x42\x10\n\x0e_major_version\"\x9c\x01\n\x15ServerVersionResponse\x12\x15\n\rmajor_version\x18\x01 \x01(\x05\x12\x15\n\rminor_version\x18\x02 \x01(\x05\x12\x15\n\rpatch_version\x18\x03 \x01(\x05\x12#\n\x16pre_release_identifier\x18\x04 \x01(\tH\x00\x88\x01\x01\x42\x19\n\x17_pre_release_identifier*P\n\x11\x41llowedUpdateType\x12\x0f\n\x0b\x41LL_UPDATES\x10\x00\x12\x1a\n\x16MINOR_REVISION_UPDATES\x10\x01\x12\x0e\n\nNO_UPDATES\x10\x02\x32\xbe%\n\x0bLittleHorse\x12\x44\n\nPutTaskDef\x12\x1e.littlehorse.PutTaskDefRequest\x1a\x14.littlehorse.TaskDef\"\x00\x12<\n\nGetTaskDef\x12\x16.littlehorse.TaskDefId\x1a\x14.littlehorse.TaskDef\"\x00\x12L\n\x12GetTaskWorkerGroup\x12\x16.littlehorse.TaskDefId\x1a\x1c.littlehorse.TaskWorkerGroup\"\x00\x12_\n\x13PutExternalEventDef\x12\'.littlehorse.PutExternalEventDefRequest\x1a\x1d.littlehorse.ExternalEventDef\"\x00\x12W\n\x13GetExternalEventDef\x12\x1f.littlehorse.ExternalEventDefId\x1a\x1d.littlehorse.ExternalEventDef\"\x00\x12_\n\x13PutWorkflowEventDef\x12\'.littlehorse.PutWorkflowEventDefRequest\x1a\x1d.littlehorse.WorkflowEventDef\"\x00\x12\x41\n\tPutWfSpec\x12\x1d.littlehorse.PutWfSpecRequest\x1a\x13.littlehorse.WfSpec\"\x00\x12\x39\n\tGetWfSpec\x12\x15.littlehorse.WfSpecId\x1a\x13.littlehorse.WfSpec\"\x00\x12M\n\x0fGetLatestWfSpec\x12#.littlehorse.GetLatestWfSpecRequest\x1a\x13.littlehorse.WfSpec\"\x00\x12I\n\rMigrateWfSpec\x12!.littlehorse.MigrateWfSpecRequest\x1a\x13.littlehorse.WfSpec\"\x00\x12P\n\x0ePutUserTaskDef\x12\".littlehorse.PutUserTaskDefRequest\x1a\x18.littlehorse.UserTaskDef\"\x00\x12H\n\x0eGetUserTaskDef\x12\x1a.littlehorse.UserTaskDefId\x1a\x18.littlehorse.UserTaskDef\"\x00\x12\\\n\x14GetLatestUserTaskDef\x12(.littlehorse.GetLatestUserTaskDefRequest\x1a\x18.littlehorse.UserTaskDef\"\x00\x12\x38\n\x05RunWf\x12\x19.littlehorse.RunWfRequest\x1a\x12.littlehorse.WfRun\"\x00\x12\x36\n\x08GetWfRun\x12\x14.littlehorse.WfRunId\x1a\x12.littlehorse.WfRun\"\x00\x12H\n\x0eGetUserTaskRun\x12\x1a.littlehorse.UserTaskRunId\x1a\x18.littlehorse.UserTaskRun\"\x00\x12T\n\x11\x41ssignUserTaskRun\x12%.littlehorse.AssignUserTaskRunRequest\x1a\x16.google.protobuf.Empty\"\x00\x12X\n\x13\x43ompleteUserTaskRun\x12\'.littlehorse.CompleteUserTaskRunRequest\x1a\x16.google.protobuf.Empty\"\x00\x12T\n\x11\x43\x61ncelUserTaskRun\x12%.littlehorse.CancelUserTaskRunRequest\x1a\x16.google.protobuf.Empty\"\x00\x12W\n\x10ListUserTaskRuns\x12#.littlehorse.ListUserTaskRunRequest\x1a\x1c.littlehorse.UserTaskRunList\"\x00\x12<\n\nGetNodeRun\x12\x16.littlehorse.NodeRunId\x1a\x14.littlehorse.NodeRun\"\x00\x12L\n\x0cListNodeRuns\x12 .littlehorse.ListNodeRunsRequest\x1a\x18.littlehorse.NodeRunList\"\x00\x12<\n\nGetTaskRun\x12\x16.littlehorse.TaskRunId\x1a\x14.littlehorse.TaskRun\"\x00\x12L\n\x0cListTaskRuns\x12 .littlehorse.ListTaskRunsRequest\x1a\x18.littlehorse.TaskRunList\"\x00\x12?\n\x0bGetVariable\x12\x17.littlehorse.VariableId\x1a\x15.littlehorse.Variable\"\x00\x12O\n\rListVariables\x12!.littlehorse.ListVariablesRequest\x1a\x19.littlehorse.VariableList\"\x00\x12V\n\x10PutExternalEvent\x12$.littlehorse.PutExternalEventRequest\x1a\x1a.littlehorse.ExternalEvent\"\x00\x12N\n\x10GetExternalEvent\x12\x1c.littlehorse.ExternalEventId\x1a\x1a.littlehorse.ExternalEvent\"\x00\x12Z\n\x12\x41waitWorkflowEvent\x12&.littlehorse.AwaitWorkflowEventRequest\x1a\x1a.littlehorse.WorkflowEvent\"\x00\x12^\n\x12ListExternalEvents\x12&.littlehorse.ListExternalEventsRequest\x1a\x1e.littlehorse.ExternalEventList\"\x00\x12J\n\x0bSearchWfRun\x12\x1f.littlehorse.SearchWfRunRequest\x1a\x18.littlehorse.WfRunIdList\"\x00\x12P\n\rSearchNodeRun\x12!.littlehorse.SearchNodeRunRequest\x1a\x1a.littlehorse.NodeRunIdList\"\x00\x12P\n\rSearchTaskRun\x12!.littlehorse.SearchTaskRunRequest\x1a\x1a.littlehorse.TaskRunIdList\"\x00\x12\\\n\x11SearchUserTaskRun\x12%.littlehorse.SearchUserTaskRunRequest\x1a\x1e.littlehorse.UserTaskRunIdList\"\x00\x12S\n\x0eSearchVariable\x12\".littlehorse.SearchVariableRequest\x1a\x1b.littlehorse.VariableIdList\"\x00\x12\x62\n\x13SearchExternalEvent\x12\'.littlehorse.SearchExternalEventRequest\x1a .littlehorse.ExternalEventIdList\"\x00\x12P\n\rSearchTaskDef\x12!.littlehorse.SearchTaskDefRequest\x1a\x1a.littlehorse.TaskDefIdList\"\x00\x12\\\n\x11SearchUserTaskDef\x12%.littlehorse.SearchUserTaskDefRequest\x1a\x1e.littlehorse.UserTaskDefIdList\"\x00\x12M\n\x0cSearchWfSpec\x12 .littlehorse.SearchWfSpecRequest\x1a\x19.littlehorse.WfSpecIdList\"\x00\x12k\n\x16SearchExternalEventDef\x12*.littlehorse.SearchExternalEventDefRequest\x1a#.littlehorse.ExternalEventDefIdList\"\x00\x12M\n\x0cSearchTenant\x12 .littlehorse.SearchTenantRequest\x1a\x19.littlehorse.TenantIdList\"\x00\x12g\n\x12RegisterTaskWorker\x12&.littlehorse.RegisterTaskWorkerRequest\x1a\'.littlehorse.RegisterTaskWorkerResponse\"\x00\x12M\n\x08PollTask\x12\x1c.littlehorse.PollTaskRequest\x1a\x1d.littlehorse.PollTaskResponse\"\x00(\x01\x30\x01\x12\x42\n\nReportTask\x12\x1a.littlehorse.ReportTaskRun\x1a\x16.google.protobuf.Empty\"\x00\x12\x44\n\tStopWfRun\x12\x1d.littlehorse.StopWfRunRequest\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x0bResumeWfRun\x12\x1f.littlehorse.ResumeWfRunRequest\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x0b\x44\x65leteWfRun\x12\x1f.littlehorse.DeleteWfRunRequest\x1a\x16.google.protobuf.Empty\"\x00\x12L\n\rDeleteTaskDef\x12!.littlehorse.DeleteTaskDefRequest\x1a\x16.google.protobuf.Empty\"\x00\x12J\n\x0c\x44\x65leteWfSpec\x12 .littlehorse.DeleteWfSpecRequest\x1a\x16.google.protobuf.Empty\"\x00\x12T\n\x11\x44\x65leteUserTaskDef\x12%.littlehorse.DeleteUserTaskDefRequest\x1a\x16.google.protobuf.Empty\"\x00\x12^\n\x16\x44\x65leteExternalEventDef\x12*.littlehorse.DeleteExternalEventDefRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x61\n\x17GetTaskDefMetricsWindow\x12\'.littlehorse.TaskDefMetricsQueryRequest\x1a\x1b.littlehorse.TaskDefMetrics\"\x00\x12^\n\x16GetWfSpecMetricsWindow\x12&.littlehorse.WfSpecMetricsQueryRequest\x1a\x1a.littlehorse.WfSpecMetrics\"\x00\x12\x61\n\x12ListTaskDefMetrics\x12#.littlehorse.ListTaskMetricsRequest\x1a$.littlehorse.ListTaskMetricsResponse\"\x00\x12\\\n\x11ListWfSpecMetrics\x12!.littlehorse.ListWfMetricsRequest\x1a\".littlehorse.ListWfMetricsResponse\"\x00\x12\x41\n\tPutTenant\x12\x1d.littlehorse.PutTenantRequest\x1a\x13.littlehorse.Tenant\"\x00\x12J\n\x0cPutPrincipal\x12 .littlehorse.PutPrincipalRequest\x1a\x16.littlehorse.Principal\"\x00\x12:\n\x06Whoami\x12\x16.google.protobuf.Empty\x1a\x16.littlehorse.Principal\"\x00\x12P\n\x10GetServerVersion\x12\x16.google.protobuf.Empty\x1a\".littlehorse.ServerVersionResponse\"\x00\x42G\n\x1fio.littlehorse.sdk.common.protoP\x01Z\x07.;model\xaa\x02\x18LittleHorse.Common.Protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rservice.proto\x12\x0blittlehorse\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x13\x63ommon_wfspec.proto\x1a\x12\x63ommon_enums.proto\x1a\x0fobject_id.proto\x1a\x0evariable.proto\x1a\x14\x65xternal_event.proto\x1a\x0cwf_run.proto\x1a\x0enode_run.proto\x1a\x0etask_run.proto\x1a\x10user_tasks.proto\x1a\rwf_spec.proto\x1a\x0etask_def.proto\x1a\nacls.proto\x1a\x14workflow_event.proto\"+\n\x1bGetLatestUserTaskDefRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xd3\x03\n\x10PutWfSpecRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x44\n\x0cthread_specs\x18\x05 \x03(\x0b\x32..littlehorse.PutWfSpecRequest.ThreadSpecsEntry\x12\x1e\n\x16\x65ntrypoint_thread_name\x18\x06 \x01(\t\x12\x43\n\x10retention_policy\x18\x08 \x01(\x0b\x32$.littlehorse.WorkflowRetentionPolicyH\x00\x88\x01\x01\x12\x46\n\x0eparent_wf_spec\x18\t \x01(\x0b\x32).littlehorse.WfSpec.ParentWfSpecReferenceH\x01\x88\x01\x01\x12\x37\n\x0f\x61llowed_updates\x18\n \x01(\x0e\x32\x1e.littlehorse.AllowedUpdateType\x1aK\n\x10ThreadSpecsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.littlehorse.ThreadSpec:\x02\x38\x01\x42\x13\n\x11_retention_policyB\x11\n\x0f_parent_wf_specJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05\"O\n\x11PutTaskDefRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12,\n\ninput_vars\x18\x02 \x03(\x0b\x32\x18.littlehorse.VariableDef\"S\n\x1aPutWorkflowEventDefRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\'\n\x04type\x18\x02 \x01(\x0e\x32\x19.littlehorse.VariableType\"{\n\x15PutUserTaskDefRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12*\n\x06\x66ields\x18\x02 \x03(\x0b\x32\x1a.littlehorse.UserTaskField\x12\x18\n\x0b\x64\x65scription\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\x0e\n\x0c_description\"o\n\x1aPutExternalEventDefRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x43\n\x10retention_policy\x18\x02 \x01(\x0b\x32).littlehorse.ExternalEventRetentionPolicy\"\xc3\x02\n\x17PutExternalEventRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\x12>\n\x15\x65xternal_event_def_id\x18\x02 \x01(\x0b\x32\x1f.littlehorse.ExternalEventDefId\x12\x11\n\x04guid\x18\x03 \x01(\tH\x00\x88\x01\x01\x12+\n\x07\x63ontent\x18\x05 \x01(\x0b\x32\x1a.littlehorse.VariableValue\x12\x1e\n\x11thread_run_number\x18\x06 \x01(\x05H\x01\x88\x01\x01\x12\x1e\n\x11node_run_position\x18\x07 \x01(\x05H\x02\x88\x01\x01\x42\x07\n\x05_guidB\x14\n\x12_thread_run_numberB\x14\n\x12_node_run_positionJ\x04\x08\x04\x10\x05J\x04\x08\x08\x10\t\"F\n\x1a\x44\x65leteExternalEventRequest\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.littlehorse.ExternalEventId\"6\n\x12\x44\x65leteWfRunRequest\x12 \n\x02id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\":\n\x14\x44\x65leteTaskDefRequest\x12\"\n\x02id\x18\x01 \x01(\x0b\x32\x16.littlehorse.TaskDefId\"B\n\x18\x44\x65leteUserTaskDefRequest\x12&\n\x02id\x18\x01 \x01(\x0b\x32\x1a.littlehorse.UserTaskDefId\"8\n\x13\x44\x65leteWfSpecRequest\x12!\n\x02id\x18\x01 \x01(\x0b\x32\x15.littlehorse.WfSpecId\"L\n\x1d\x44\x65leteExternalEventDefRequest\x12+\n\x02id\x18\x01 \x01(\x0b\x32\x1f.littlehorse.ExternalEventDefId\"\xe3\x02\n\x0cRunWfRequest\x12\x14\n\x0cwf_spec_name\x18\x01 \x01(\t\x12\x1a\n\rmajor_version\x18\x02 \x01(\x05H\x00\x88\x01\x01\x12\x15\n\x08revision\x18\x03 \x01(\x05H\x01\x88\x01\x01\x12;\n\tvariables\x18\x04 \x03(\x0b\x32(.littlehorse.RunWfRequest.VariablesEntry\x12\x0f\n\x02id\x18\x05 \x01(\tH\x02\x88\x01\x01\x12\x33\n\x10parent_wf_run_id\x18\x06 \x01(\x0b\x32\x14.littlehorse.WfRunIdH\x03\x88\x01\x01\x1aL\n\x0eVariablesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.littlehorse.VariableValue:\x02\x38\x01\x42\x10\n\x0e_major_versionB\x0b\n\t_revisionB\x05\n\x03_idB\x13\n\x11_parent_wf_run_id\"L\n\rVariableMatch\x12\x10\n\x08var_name\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.littlehorse.VariableValue\"\xbd\x01\n\x19\x41waitWorkflowEventRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\x12\x36\n\revent_def_ids\x18\x02 \x03(\x0b\x32\x1f.littlehorse.WorkflowEventDefId\x12?\n\x19workflow_events_to_ignore\x18\x03 \x03(\x0b\x32\x1c.littlehorse.WorkflowEventId\"\xdf\x03\n\x12SearchWfRunRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x14\n\x0cwf_spec_name\x18\x03 \x01(\t\x12\"\n\x15wf_spec_major_version\x18\x04 \x01(\x05H\x02\x88\x01\x01\x12\x1d\n\x10wf_spec_revision\x18\x05 \x01(\x05H\x03\x88\x01\x01\x12*\n\x06status\x18\x06 \x01(\x0e\x32\x15.littlehorse.LHStatusH\x04\x88\x01\x01\x12\x37\n\x0e\x65\x61rliest_start\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x05\x88\x01\x01\x12\x35\n\x0clatest_start\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x06\x88\x01\x01\x12\x34\n\x10variable_filters\x18\t \x03(\x0b\x32\x1a.littlehorse.VariableMatchB\x0b\n\t_bookmarkB\x08\n\x06_limitB\x18\n\x16_wf_spec_major_versionB\x13\n\x11_wf_spec_revisionB\t\n\x07_statusB\x11\n\x0f_earliest_startB\x0f\n\r_latest_start\"X\n\x0bWfRunIdList\x12%\n\x07results\x18\x01 \x03(\x0b\x32\x14.littlehorse.WfRunId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\xbc\x02\n\x14SearchTaskRunRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x15\n\rtask_def_name\x18\x03 \x01(\t\x12,\n\x06status\x18\x04 \x01(\x0e\x32\x17.littlehorse.TaskStatusH\x02\x88\x01\x01\x12\x37\n\x0e\x65\x61rliest_start\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x03\x88\x01\x01\x12\x35\n\x0clatest_start\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x04\x88\x01\x01\x42\x0b\n\t_bookmarkB\x08\n\x06_limitB\t\n\x07_statusB\x11\n\x0f_earliest_startB\x0f\n\r_latest_start\"\\\n\rTaskRunIdList\x12\'\n\x07results\x18\x01 \x03(\x0b\x32\x16.littlehorse.TaskRunId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\xf1\x03\n\x14SearchNodeRunRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x37\n\x0e\x65\x61rliest_start\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x02\x88\x01\x01\x12\x35\n\x0clatest_start\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x03\x88\x01\x01\x12=\n\tnode_type\x18\x05 \x01(\x0e\x32*.littlehorse.SearchNodeRunRequest.NodeType\x12%\n\x06status\x18\x06 \x01(\x0e\x32\x15.littlehorse.LHStatus\"\x9c\x01\n\x08NodeType\x12\x08\n\x04TASK\x10\x00\x12\x12\n\x0e\x45XTERNAL_EVENT\x10\x01\x12\x0e\n\nENTRYPOINT\x10\x02\x12\x08\n\x04\x45XIT\x10\x03\x12\x10\n\x0cSTART_THREAD\x10\x04\x12\x10\n\x0cWAIT_THREADS\x10\x05\x12\t\n\x05SLEEP\x10\x06\x12\r\n\tUSER_TASK\x10\x07\x12\x1a\n\x16START_MULTIPLE_THREADS\x10\x08\x42\x0b\n\t_bookmarkB\x08\n\x06_limitB\x11\n\x0f_earliest_startB\x0f\n\r_latest_start\"\\\n\rNodeRunIdList\x12\'\n\x07results\x18\x01 \x03(\x0b\x32\x16.littlehorse.NodeRunId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\xb2\x03\n\x18SearchUserTaskRunRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x33\n\x06status\x18\x03 \x01(\x0e\x32\x1e.littlehorse.UserTaskRunStatusH\x02\x88\x01\x01\x12\x1f\n\x12user_task_def_name\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x14\n\x07user_id\x18\x05 \x01(\tH\x04\x88\x01\x01\x12\x17\n\nuser_group\x18\x06 \x01(\tH\x05\x88\x01\x01\x12\x37\n\x0e\x65\x61rliest_start\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x06\x88\x01\x01\x12\x35\n\x0clatest_start\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x07\x88\x01\x01\x42\x0b\n\t_bookmarkB\x08\n\x06_limitB\t\n\x07_statusB\x15\n\x13_user_task_def_nameB\n\n\x08_user_idB\r\n\x0b_user_groupB\x11\n\x0f_earliest_startB\x0f\n\r_latest_start\"d\n\x11UserTaskRunIdList\x12+\n\x07results\x18\x01 \x03(\x0b\x32\x1a.littlehorse.UserTaskRunId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\x9e\x02\n\x15SearchVariableRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12)\n\x05value\x18\x03 \x01(\x0b\x32\x1a.littlehorse.VariableValue\x12\"\n\x15wf_spec_major_version\x18\x04 \x01(\x05H\x02\x88\x01\x01\x12\x1d\n\x10wf_spec_revision\x18\x05 \x01(\x05H\x03\x88\x01\x01\x12\x10\n\x08var_name\x18\x06 \x01(\t\x12\x14\n\x0cwf_spec_name\x18\x07 \x01(\tB\x0b\n\t_bookmarkB\x08\n\x06_limitB\x18\n\x16_wf_spec_major_versionB\x13\n\x11_wf_spec_revision\"^\n\x0eVariableIdList\x12(\n\x07results\x18\x01 \x03(\x0b\x32\x17.littlehorse.VariableId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"x\n\x14SearchTaskDefRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x13\n\x06prefix\x18\x03 \x01(\tH\x02\x88\x01\x01\x42\x0b\n\t_bookmarkB\x08\n\x06_limitB\t\n\x07_prefix\"\\\n\rTaskDefIdList\x12\'\n\x07results\x18\x01 \x03(\x0b\x32\x16.littlehorse.TaskDefId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\x98\x01\n\x18SearchUserTaskDefRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x01\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x02\x88\x01\x01\x12\x10\n\x06prefix\x18\x03 \x01(\tH\x00\x12\x0e\n\x04name\x18\x04 \x01(\tH\x00\x42\x18\n\x16user_task_def_criteriaB\x0b\n\t_bookmarkB\x08\n\x06_limit\"d\n\x11UserTaskDefIdList\x12+\n\x07results\x18\x01 \x03(\x0b\x32\x1a.littlehorse.UserTaskDefId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\xa6\x01\n\x13SearchWfSpecRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x01\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x02\x88\x01\x01\x12\x0e\n\x04name\x18\x03 \x01(\tH\x00\x12\x10\n\x06prefix\x18\x04 \x01(\tH\x00\x12\x17\n\rtask_def_name\x18\x05 \x01(\tH\x00\x42\x12\n\x10wf_spec_criteriaB\x0b\n\t_bookmarkB\x08\n\x06_limit\"Z\n\x0cWfSpecIdList\x12&\n\x07results\x18\x01 \x03(\x0b\x32\x15.littlehorse.WfSpecId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\x81\x01\n\x1dSearchExternalEventDefRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x13\n\x06prefix\x18\x03 \x01(\tH\x02\x88\x01\x01\x42\x0b\n\t_bookmarkB\x08\n\x06_limitB\t\n\x07_prefix\"n\n\x16\x45xternalEventDefIdList\x12\x30\n\x07results\x18\x01 \x03(\x0b\x32\x1f.littlehorse.ExternalEventDefId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"W\n\x13SearchTenantRequest\x12\x12\n\x05limit\x18\x01 \x01(\x05H\x00\x88\x01\x01\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x01\x88\x01\x01\x42\x08\n\x06_limitB\x0b\n\t_bookmark\"Z\n\x0cTenantIdList\x12&\n\x07results\x18\x01 \x03(\x0b\x32\x15.littlehorse.TenantId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\x80\x03\n\x1aSearchExternalEventRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x01\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x02\x88\x01\x01\x12)\n\twf_run_id\x18\x03 \x01(\x0b\x32\x14.littlehorse.WfRunIdH\x00\x12u\n\"external_event_def_name_and_status\x18\x04 \x01(\x0b\x32G.littlehorse.SearchExternalEventRequest.ByExtEvtDefNameAndStatusRequestH\x00\x1aj\n\x1f\x42yExtEvtDefNameAndStatusRequest\x12\x1f\n\x17\x65xternal_event_def_name\x18\x01 \x01(\t\x12\x17\n\nis_claimed\x18\x02 \x01(\x08H\x00\x88\x01\x01\x42\r\n\x0b_is_claimedB\x12\n\x10\x65xt_evt_criteriaB\x0b\n\t_bookmarkB\x08\n\x06_limit\"h\n\x13\x45xternalEventIdList\x12-\n\x07results\x18\x01 \x03(\x0b\x32\x1c.littlehorse.ExternalEventId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\xb6\x01\n\x13ListNodeRunsRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\x12\x1e\n\x11thread_run_number\x18\x02 \x01(\x05H\x00\x88\x01\x01\x12\x15\n\x08\x62ookmark\x18\x03 \x01(\x0cH\x01\x88\x01\x01\x12\x12\n\x05limit\x18\x04 \x01(\x05H\x02\x88\x01\x01\x42\x14\n\x12_thread_run_numberB\x0b\n\t_bookmarkB\x08\n\x06_limit\"X\n\x0bNodeRunList\x12%\n\x07results\x18\x01 \x03(\x0b\x32\x14.littlehorse.NodeRun\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"?\n\x14ListVariablesRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\"6\n\x0cVariableList\x12&\n\x07results\x18\x01 \x03(\x0b\x32\x15.littlehorse.Variable\"D\n\x19ListExternalEventsRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\"@\n\x11\x45xternalEventList\x12+\n\x07results\x18\x01 \x03(\x0b\x32\x1a.littlehorse.ExternalEvent\"w\n\x19RegisterTaskWorkerRequest\x12\x16\n\x0etask_worker_id\x18\x01 \x01(\t\x12+\n\x0btask_def_id\x18\x02 \x01(\x0b\x32\x16.littlehorse.TaskDefId\x12\x15\n\rlistener_name\x18\x03 \x01(\t\"s\n\x1aTaskWorkerHeartBeatRequest\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12+\n\x0btask_def_id\x18\x02 \x01(\x0b\x32\x16.littlehorse.TaskDefId\x12\x15\n\rlistener_name\x18\x03 \x01(\t\"\x81\x01\n\x1aRegisterTaskWorkerResponse\x12+\n\nyour_hosts\x18\x01 \x03(\x0b\x32\x17.littlehorse.LHHostInfo\x12\x1f\n\x12is_cluster_healthy\x18\x02 \x01(\x08H\x00\x88\x01\x01\x42\x15\n\x13_is_cluster_healthy\"(\n\nLHHostInfo\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"\x8b\x01\n\x0fPollTaskRequest\x12+\n\x0btask_def_id\x18\x01 \x01(\x0b\x32\x16.littlehorse.TaskDefId\x12\x11\n\tclient_id\x18\x02 \x01(\t\x12 \n\x13task_worker_version\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\x16\n\x14_task_worker_version\"\x8c\x02\n\rScheduledTask\x12+\n\x0btask_run_id\x18\x01 \x01(\x0b\x32\x16.littlehorse.TaskRunId\x12+\n\x0btask_def_id\x18\x02 \x01(\x0b\x32\x16.littlehorse.TaskDefId\x12\x16\n\x0e\x61ttempt_number\x18\x03 \x01(\x05\x12-\n\tvariables\x18\x04 \x03(\x0b\x32\x1a.littlehorse.VarNameAndVal\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x06source\x18\x06 \x01(\x0b\x32\x1a.littlehorse.TaskRunSource\"N\n\x10PollTaskResponse\x12/\n\x06result\x18\x01 \x01(\x0b\x32\x1a.littlehorse.ScheduledTaskH\x00\x88\x01\x01\x42\t\n\x07_result\"\x81\x03\n\rReportTaskRun\x12+\n\x0btask_run_id\x18\x01 \x01(\x0b\x32\x16.littlehorse.TaskRunId\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\x06status\x18\x03 \x01(\x0e\x32\x17.littlehorse.TaskStatus\x12\x33\n\nlog_output\x18\x05 \x01(\x0b\x32\x1a.littlehorse.VariableValueH\x01\x88\x01\x01\x12\x16\n\x0e\x61ttempt_number\x18\x06 \x01(\x05\x12,\n\x06output\x18\x04 \x01(\x0b\x32\x1a.littlehorse.VariableValueH\x00\x12)\n\x05\x65rror\x18\x07 \x01(\x0b\x32\x18.littlehorse.LHTaskErrorH\x00\x12\x31\n\texception\x18\x08 \x01(\x0b\x32\x1c.littlehorse.LHTaskExceptionH\x00\x42\x08\n\x06resultB\r\n\x0b_log_output\"V\n\x10StopWfRunRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\x12\x19\n\x11thread_run_number\x18\x02 \x01(\x05\"X\n\x12ResumeWfRunRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\x12\x19\n\x11thread_run_number\x18\x02 \x01(\x05\"\xb3\x01\n\x1aTaskDefMetricsQueryRequest\x12\x30\n\x0cwindow_start\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x0bwindow_type\x18\x02 \x01(\x0e\x32 .littlehorse.MetricsWindowLength\x12\x1a\n\rtask_def_name\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\x10\n\x0e_task_def_name\"\xca\x01\n\x16ListTaskMetricsRequest\x12+\n\x0btask_def_id\x18\x01 \x01(\x0b\x32\x16.littlehorse.TaskDefId\x12\x35\n\x11last_window_start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\rwindow_length\x18\x03 \x01(\x0e\x32 .littlehorse.MetricsWindowLength\x12\x13\n\x0bnum_windows\x18\x04 \x01(\x05\"G\n\x17ListTaskMetricsResponse\x12,\n\x07results\x18\x01 \x03(\x0b\x32\x1b.littlehorse.TaskDefMetrics\"\xb1\x01\n\x19WfSpecMetricsQueryRequest\x12)\n\nwf_spec_id\x18\x01 \x01(\x0b\x32\x15.littlehorse.WfSpecId\x12\x30\n\x0cwindow_start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\rwindow_length\x18\x03 \x01(\x0e\x32 .littlehorse.MetricsWindowLength\"\xc6\x01\n\x14ListWfMetricsRequest\x12)\n\nwf_spec_id\x18\x01 \x01(\x0b\x32\x15.littlehorse.WfSpecId\x12\x35\n\x11last_window_start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\rwindow_length\x18\x03 \x01(\x0e\x32 .littlehorse.MetricsWindowLength\x12\x13\n\x0bnum_windows\x18\x04 \x01(\x05\"D\n\x15ListWfMetricsResponse\x12+\n\x07results\x18\x01 \x03(\x0b\x32\x1a.littlehorse.WfSpecMetrics\"\xfb\x02\n\x0eTaskDefMetrics\x12+\n\x0btask_def_id\x18\x01 \x01(\x0b\x32\x16.littlehorse.TaskDefId\x12\x30\n\x0cwindow_start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\x04type\x18\x03 \x01(\x0e\x32 .littlehorse.MetricsWindowLength\x12\x1d\n\x15schedule_to_start_max\x18\x04 \x01(\x03\x12\x1d\n\x15schedule_to_start_avg\x18\x05 \x01(\x03\x12\x1d\n\x15start_to_complete_max\x18\x06 \x01(\x03\x12\x1d\n\x15start_to_complete_avg\x18\x07 \x01(\x03\x12\x17\n\x0ftotal_completed\x18\x08 \x01(\x03\x12\x15\n\rtotal_errored\x18\t \x01(\x03\x12\x15\n\rtotal_started\x18\n \x01(\x03\x12\x17\n\x0ftotal_scheduled\x18\x0b \x01(\x03\"\xa1\x02\n\rWfSpecMetrics\x12)\n\nwf_spec_id\x18\x01 \x01(\x0b\x32\x15.littlehorse.WfSpecId\x12\x30\n\x0cwindow_start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\x04type\x18\x03 \x01(\x0e\x32 .littlehorse.MetricsWindowLength\x12\x15\n\rtotal_started\x18\x04 \x01(\x03\x12\x17\n\x0ftotal_completed\x18\x05 \x01(\x03\x12\x15\n\rtotal_errored\x18\x06 \x01(\x03\x12\x1d\n\x15start_to_complete_max\x18\x07 \x01(\x03\x12\x1d\n\x15start_to_complete_avg\x18\x08 \x01(\x03\"A\n\x16ListUserTaskRunRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\"<\n\x0fUserTaskRunList\x12)\n\x07results\x18\x01 \x03(\x0b\x32\x18.littlehorse.UserTaskRun\"\x8a\x01\n\x12TaskWorkerMetadata\x12\x16\n\x0etask_worker_id\x18\x01 \x01(\t\x12\x34\n\x10latest_heartbeat\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12&\n\x05hosts\x18\x03 \x03(\x0b\x32\x17.littlehorse.LHHostInfo\"\x87\x02\n\x0fTaskWorkerGroup\x12*\n\x02id\x18\x01 \x01(\x0b\x32\x1e.littlehorse.TaskWorkerGroupId\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x43\n\x0ctask_workers\x18\x03 \x03(\x0b\x32-.littlehorse.TaskWorkerGroup.TaskWorkersEntry\x1aS\n\x10TaskWorkersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12.\n\x05value\x18\x02 \x01(\x0b\x32\x1f.littlehorse.TaskWorkerMetadata:\x02\x38\x01\">\n\x13ListTaskRunsRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\"4\n\x0bTaskRunList\x12%\n\x07results\x18\x01 \x03(\x0b\x32\x14.littlehorse.TaskRun\"z\n\x14MigrateWfSpecRequest\x12*\n\x0bold_wf_spec\x18\x01 \x01(\x0b\x32\x15.littlehorse.WfSpecId\x12\x36\n\tmigration\x18\x02 \x01(\x0b\x32#.littlehorse.WfSpecVersionMigration\"T\n\x16GetLatestWfSpecRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1a\n\rmajor_version\x18\x02 \x01(\x05H\x00\x88\x01\x01\x42\x10\n\x0e_major_version\"\x9c\x01\n\x15ServerVersionResponse\x12\x15\n\rmajor_version\x18\x01 \x01(\x05\x12\x15\n\rminor_version\x18\x02 \x01(\x05\x12\x15\n\rpatch_version\x18\x03 \x01(\x05\x12#\n\x16pre_release_identifier\x18\x04 \x01(\tH\x00\x88\x01\x01\x42\x19\n\x17_pre_release_identifier*P\n\x11\x41llowedUpdateType\x12\x0f\n\x0b\x41LL_UPDATES\x10\x00\x12\x1a\n\x16MINOR_REVISION_UPDATES\x10\x01\x12\x0e\n\nNO_UPDATES\x10\x02\x32\xcb&\n\x0bLittleHorse\x12\x44\n\nPutTaskDef\x12\x1e.littlehorse.PutTaskDefRequest\x1a\x14.littlehorse.TaskDef\"\x00\x12<\n\nGetTaskDef\x12\x16.littlehorse.TaskDefId\x1a\x14.littlehorse.TaskDef\"\x00\x12L\n\x12GetTaskWorkerGroup\x12\x16.littlehorse.TaskDefId\x1a\x1c.littlehorse.TaskWorkerGroup\"\x00\x12_\n\x13PutExternalEventDef\x12\'.littlehorse.PutExternalEventDefRequest\x1a\x1d.littlehorse.ExternalEventDef\"\x00\x12W\n\x13GetExternalEventDef\x12\x1f.littlehorse.ExternalEventDefId\x1a\x1d.littlehorse.ExternalEventDef\"\x00\x12_\n\x13PutWorkflowEventDef\x12\'.littlehorse.PutWorkflowEventDefRequest\x1a\x1d.littlehorse.WorkflowEventDef\"\x00\x12\x41\n\tPutWfSpec\x12\x1d.littlehorse.PutWfSpecRequest\x1a\x13.littlehorse.WfSpec\"\x00\x12\x39\n\tGetWfSpec\x12\x15.littlehorse.WfSpecId\x1a\x13.littlehorse.WfSpec\"\x00\x12M\n\x0fGetLatestWfSpec\x12#.littlehorse.GetLatestWfSpecRequest\x1a\x13.littlehorse.WfSpec\"\x00\x12I\n\rMigrateWfSpec\x12!.littlehorse.MigrateWfSpecRequest\x1a\x13.littlehorse.WfSpec\"\x00\x12P\n\x0ePutUserTaskDef\x12\".littlehorse.PutUserTaskDefRequest\x1a\x18.littlehorse.UserTaskDef\"\x00\x12H\n\x0eGetUserTaskDef\x12\x1a.littlehorse.UserTaskDefId\x1a\x18.littlehorse.UserTaskDef\"\x00\x12\\\n\x14GetLatestUserTaskDef\x12(.littlehorse.GetLatestUserTaskDefRequest\x1a\x18.littlehorse.UserTaskDef\"\x00\x12\x38\n\x05RunWf\x12\x19.littlehorse.RunWfRequest\x1a\x12.littlehorse.WfRun\"\x00\x12\x36\n\x08GetWfRun\x12\x14.littlehorse.WfRunId\x1a\x12.littlehorse.WfRun\"\x00\x12H\n\x0eGetUserTaskRun\x12\x1a.littlehorse.UserTaskRunId\x1a\x18.littlehorse.UserTaskRun\"\x00\x12T\n\x11\x41ssignUserTaskRun\x12%.littlehorse.AssignUserTaskRunRequest\x1a\x16.google.protobuf.Empty\"\x00\x12X\n\x13\x43ompleteUserTaskRun\x12\'.littlehorse.CompleteUserTaskRunRequest\x1a\x16.google.protobuf.Empty\"\x00\x12T\n\x11\x43\x61ncelUserTaskRun\x12%.littlehorse.CancelUserTaskRunRequest\x1a\x16.google.protobuf.Empty\"\x00\x12W\n\x10ListUserTaskRuns\x12#.littlehorse.ListUserTaskRunRequest\x1a\x1c.littlehorse.UserTaskRunList\"\x00\x12<\n\nGetNodeRun\x12\x16.littlehorse.NodeRunId\x1a\x14.littlehorse.NodeRun\"\x00\x12L\n\x0cListNodeRuns\x12 .littlehorse.ListNodeRunsRequest\x1a\x18.littlehorse.NodeRunList\"\x00\x12<\n\nGetTaskRun\x12\x16.littlehorse.TaskRunId\x1a\x14.littlehorse.TaskRun\"\x00\x12L\n\x0cListTaskRuns\x12 .littlehorse.ListTaskRunsRequest\x1a\x18.littlehorse.TaskRunList\"\x00\x12?\n\x0bGetVariable\x12\x17.littlehorse.VariableId\x1a\x15.littlehorse.Variable\"\x00\x12O\n\rListVariables\x12!.littlehorse.ListVariablesRequest\x1a\x19.littlehorse.VariableList\"\x00\x12V\n\x10PutExternalEvent\x12$.littlehorse.PutExternalEventRequest\x1a\x1a.littlehorse.ExternalEvent\"\x00\x12N\n\x10GetExternalEvent\x12\x1c.littlehorse.ExternalEventId\x1a\x1a.littlehorse.ExternalEvent\"\x00\x12Z\n\x12\x41waitWorkflowEvent\x12&.littlehorse.AwaitWorkflowEventRequest\x1a\x1a.littlehorse.WorkflowEvent\"\x00\x12^\n\x12ListExternalEvents\x12&.littlehorse.ListExternalEventsRequest\x1a\x1e.littlehorse.ExternalEventList\"\x00\x12J\n\x0bSearchWfRun\x12\x1f.littlehorse.SearchWfRunRequest\x1a\x18.littlehorse.WfRunIdList\"\x00\x12P\n\rSearchNodeRun\x12!.littlehorse.SearchNodeRunRequest\x1a\x1a.littlehorse.NodeRunIdList\"\x00\x12P\n\rSearchTaskRun\x12!.littlehorse.SearchTaskRunRequest\x1a\x1a.littlehorse.TaskRunIdList\"\x00\x12\\\n\x11SearchUserTaskRun\x12%.littlehorse.SearchUserTaskRunRequest\x1a\x1e.littlehorse.UserTaskRunIdList\"\x00\x12S\n\x0eSearchVariable\x12\".littlehorse.SearchVariableRequest\x1a\x1b.littlehorse.VariableIdList\"\x00\x12\x62\n\x13SearchExternalEvent\x12\'.littlehorse.SearchExternalEventRequest\x1a .littlehorse.ExternalEventIdList\"\x00\x12P\n\rSearchTaskDef\x12!.littlehorse.SearchTaskDefRequest\x1a\x1a.littlehorse.TaskDefIdList\"\x00\x12\\\n\x11SearchUserTaskDef\x12%.littlehorse.SearchUserTaskDefRequest\x1a\x1e.littlehorse.UserTaskDefIdList\"\x00\x12M\n\x0cSearchWfSpec\x12 .littlehorse.SearchWfSpecRequest\x1a\x19.littlehorse.WfSpecIdList\"\x00\x12k\n\x16SearchExternalEventDef\x12*.littlehorse.SearchExternalEventDefRequest\x1a#.littlehorse.ExternalEventDefIdList\"\x00\x12M\n\x0cSearchTenant\x12 .littlehorse.SearchTenantRequest\x1a\x19.littlehorse.TenantIdList\"\x00\x12g\n\x12RegisterTaskWorker\x12&.littlehorse.RegisterTaskWorkerRequest\x1a\'.littlehorse.RegisterTaskWorkerResponse\"\x00\x12M\n\x08PollTask\x12\x1c.littlehorse.PollTaskRequest\x1a\x1d.littlehorse.PollTaskResponse\"\x00(\x01\x30\x01\x12\x42\n\nReportTask\x12\x1a.littlehorse.ReportTaskRun\x1a\x16.google.protobuf.Empty\"\x00\x12\x44\n\tStopWfRun\x12\x1d.littlehorse.StopWfRunRequest\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x0bResumeWfRun\x12\x1f.littlehorse.ResumeWfRunRequest\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x0b\x44\x65leteWfRun\x12\x1f.littlehorse.DeleteWfRunRequest\x1a\x16.google.protobuf.Empty\"\x00\x12L\n\rDeleteTaskDef\x12!.littlehorse.DeleteTaskDefRequest\x1a\x16.google.protobuf.Empty\"\x00\x12J\n\x0c\x44\x65leteWfSpec\x12 .littlehorse.DeleteWfSpecRequest\x1a\x16.google.protobuf.Empty\"\x00\x12T\n\x11\x44\x65leteUserTaskDef\x12%.littlehorse.DeleteUserTaskDefRequest\x1a\x16.google.protobuf.Empty\"\x00\x12^\n\x16\x44\x65leteExternalEventDef\x12*.littlehorse.DeleteExternalEventDefRequest\x1a\x16.google.protobuf.Empty\"\x00\x12P\n\x0f\x44\x65letePrincipal\x12#.littlehorse.DeletePrincipalRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x61\n\x17GetTaskDefMetricsWindow\x12\'.littlehorse.TaskDefMetricsQueryRequest\x1a\x1b.littlehorse.TaskDefMetrics\"\x00\x12^\n\x16GetWfSpecMetricsWindow\x12&.littlehorse.WfSpecMetricsQueryRequest\x1a\x1a.littlehorse.WfSpecMetrics\"\x00\x12\x61\n\x12ListTaskDefMetrics\x12#.littlehorse.ListTaskMetricsRequest\x1a$.littlehorse.ListTaskMetricsResponse\"\x00\x12\\\n\x11ListWfSpecMetrics\x12!.littlehorse.ListWfMetricsRequest\x1a\".littlehorse.ListWfMetricsResponse\"\x00\x12\x41\n\tPutTenant\x12\x1d.littlehorse.PutTenantRequest\x1a\x13.littlehorse.Tenant\"\x00\x12\x39\n\tGetTenant\x12\x15.littlehorse.TenantId\x1a\x13.littlehorse.Tenant\"\x00\x12J\n\x0cPutPrincipal\x12 .littlehorse.PutPrincipalRequest\x1a\x16.littlehorse.Principal\"\x00\x12:\n\x06Whoami\x12\x16.google.protobuf.Empty\x1a\x16.littlehorse.Principal\"\x00\x12P\n\x10GetServerVersion\x12\x16.google.protobuf.Empty\x1a\".littlehorse.ServerVersionResponse\"\x00\x42G\n\x1fio.littlehorse.sdk.common.protoP\x01Z\x07.;model\xaa\x02\x18LittleHorse.Common.Protob\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
@@ -194,9 +194,9 @@
   _globals['_MIGRATEWFSPECREQUEST']._serialized_start=10979
   _globals['_MIGRATEWFSPECREQUEST']._serialized_end=11101
   _globals['_GETLATESTWFSPECREQUEST']._serialized_start=11103
   _globals['_GETLATESTWFSPECREQUEST']._serialized_end=11187
   _globals['_SERVERVERSIONRESPONSE']._serialized_start=11190
   _globals['_SERVERVERSIONRESPONSE']._serialized_end=11346
   _globals['_LITTLEHORSE']._serialized_start=11431
-  _globals['_LITTLEHORSE']._serialized_end=16229
+  _globals['_LITTLEHORSE']._serialized_end=16370
 # @@protoc_insertion_point(module_scope)
```

### Comparing `littlehorse_client-0.9.0/littlehorse/model/service_pb2.pyi` & `littlehorse_client-0.9.1/littlehorse/model/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/service_pb2_grpc.py` & `littlehorse_client-0.9.1/littlehorse/model/service_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,14 +277,19 @@
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
         self.DeleteExternalEventDef = channel.unary_unary(
                 '/littlehorse.LittleHorse/DeleteExternalEventDef',
                 request_serializer=service__pb2.DeleteExternalEventDefRequest.SerializeToString,
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
+        self.DeletePrincipal = channel.unary_unary(
+                '/littlehorse.LittleHorse/DeletePrincipal',
+                request_serializer=acls__pb2.DeletePrincipalRequest.SerializeToString,
+                response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                )
         self.GetTaskDefMetricsWindow = channel.unary_unary(
                 '/littlehorse.LittleHorse/GetTaskDefMetricsWindow',
                 request_serializer=service__pb2.TaskDefMetricsQueryRequest.SerializeToString,
                 response_deserializer=service__pb2.TaskDefMetrics.FromString,
                 )
         self.GetWfSpecMetricsWindow = channel.unary_unary(
                 '/littlehorse.LittleHorse/GetWfSpecMetricsWindow',
@@ -302,14 +307,19 @@
                 response_deserializer=service__pb2.ListWfMetricsResponse.FromString,
                 )
         self.PutTenant = channel.unary_unary(
                 '/littlehorse.LittleHorse/PutTenant',
                 request_serializer=acls__pb2.PutTenantRequest.SerializeToString,
                 response_deserializer=acls__pb2.Tenant.FromString,
                 )
+        self.GetTenant = channel.unary_unary(
+                '/littlehorse.LittleHorse/GetTenant',
+                request_serializer=object__id__pb2.TenantId.SerializeToString,
+                response_deserializer=acls__pb2.Tenant.FromString,
+                )
         self.PutPrincipal = channel.unary_unary(
                 '/littlehorse.LittleHorse/PutPrincipal',
                 request_serializer=acls__pb2.PutPrincipalRequest.SerializeToString,
                 response_deserializer=acls__pb2.Principal.FromString,
                 )
         self.Whoami = channel.unary_unary(
                 '/littlehorse.LittleHorse/Whoami',
@@ -718,14 +728,23 @@
     def DeleteExternalEventDef(self, request, context):
         """Deletes an ExternalEventDef.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def DeletePrincipal(self, request, context):
+        """Deletes a `Principal`. Fails with `FAILED_PRECONDITION` if the specified `Principal`
+        is the last remaining `Principal` with admin permissions. Admin permissions are defined
+        as having the `global_acls` of `ALL_ACTIONS` over the `ACL_ALL_RESOURCES` scope.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def GetTaskDefMetricsWindow(self, request, context):
         """Returns TaskDef Metrics for a specific TaskDef and a specific time window.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -753,14 +772,21 @@
     def PutTenant(self, request, context):
         """EXPERIMENTAL: Creates another Tenant in the LH Server.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetTenant(self, request, context):
+        """EXPERIMENTAL: Gets a Tenant from the LH Server.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def PutPrincipal(self, request, context):
         """EXPERIMENTAL: Creates an Principal.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -1032,14 +1058,19 @@
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
             'DeleteExternalEventDef': grpc.unary_unary_rpc_method_handler(
                     servicer.DeleteExternalEventDef,
                     request_deserializer=service__pb2.DeleteExternalEventDefRequest.FromString,
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
+            'DeletePrincipal': grpc.unary_unary_rpc_method_handler(
+                    servicer.DeletePrincipal,
+                    request_deserializer=acls__pb2.DeletePrincipalRequest.FromString,
+                    response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ),
             'GetTaskDefMetricsWindow': grpc.unary_unary_rpc_method_handler(
                     servicer.GetTaskDefMetricsWindow,
                     request_deserializer=service__pb2.TaskDefMetricsQueryRequest.FromString,
                     response_serializer=service__pb2.TaskDefMetrics.SerializeToString,
             ),
             'GetWfSpecMetricsWindow': grpc.unary_unary_rpc_method_handler(
                     servicer.GetWfSpecMetricsWindow,
@@ -1057,14 +1088,19 @@
                     response_serializer=service__pb2.ListWfMetricsResponse.SerializeToString,
             ),
             'PutTenant': grpc.unary_unary_rpc_method_handler(
                     servicer.PutTenant,
                     request_deserializer=acls__pb2.PutTenantRequest.FromString,
                     response_serializer=acls__pb2.Tenant.SerializeToString,
             ),
+            'GetTenant': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetTenant,
+                    request_deserializer=object__id__pb2.TenantId.FromString,
+                    response_serializer=acls__pb2.Tenant.SerializeToString,
+            ),
             'PutPrincipal': grpc.unary_unary_rpc_method_handler(
                     servicer.PutPrincipal,
                     request_deserializer=acls__pb2.PutPrincipalRequest.FromString,
                     response_serializer=acls__pb2.Principal.SerializeToString,
             ),
             'Whoami': grpc.unary_unary_rpc_method_handler(
                     servicer.Whoami,
@@ -1950,14 +1986,31 @@
         return grpc.experimental.unary_unary(request, target, '/littlehorse.LittleHorse/DeleteExternalEventDef',
             service__pb2.DeleteExternalEventDefRequest.SerializeToString,
             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def DeletePrincipal(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/littlehorse.LittleHorse/DeletePrincipal',
+            acls__pb2.DeletePrincipalRequest.SerializeToString,
+            google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def GetTaskDefMetricsWindow(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -2035,14 +2088,31 @@
         return grpc.experimental.unary_unary(request, target, '/littlehorse.LittleHorse/PutTenant',
             acls__pb2.PutTenantRequest.SerializeToString,
             acls__pb2.Tenant.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GetTenant(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/littlehorse.LittleHorse/GetTenant',
+            object__id__pb2.TenantId.SerializeToString,
+            acls__pb2.Tenant.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def PutPrincipal(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `littlehorse_client-0.9.0/littlehorse/model/task_def_pb2.py` & `littlehorse_client-0.9.1/littlehorse/model/task_def_pb2.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/task_def_pb2.pyi` & `littlehorse_client-0.9.1/littlehorse/model/task_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/task_run_pb2.py` & `littlehorse_client-0.9.1/littlehorse/model/task_run_pb2.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/task_run_pb2.pyi` & `littlehorse_client-0.9.1/littlehorse/model/task_run_pb2.pyi`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/user_tasks_pb2.py` & `littlehorse_client-0.9.1/littlehorse/model/user_tasks_pb2.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/user_tasks_pb2.pyi` & `littlehorse_client-0.9.1/littlehorse/model/user_tasks_pb2.pyi`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/variable_pb2.py` & `littlehorse_client-0.9.1/littlehorse/model/variable_pb2.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/variable_pb2.pyi` & `littlehorse_client-0.9.1/littlehorse/model/variable_pb2.pyi`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/wf_run_pb2.py` & `littlehorse_client-0.9.1/littlehorse/model/wf_run_pb2.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/wf_run_pb2.pyi` & `littlehorse_client-0.9.1/littlehorse/model/wf_run_pb2.pyi`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/wf_spec_pb2.py` & `littlehorse_client-0.9.1/littlehorse/model/wf_spec_pb2.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/wf_spec_pb2.pyi` & `littlehorse_client-0.9.1/littlehorse/model/wf_spec_pb2.pyi`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/workflow_event_pb2.py` & `littlehorse_client-0.9.1/littlehorse/model/workflow_event_pb2.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/model/workflow_event_pb2.pyi` & `littlehorse_client-0.9.1/littlehorse/model/workflow_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/utils.py` & `littlehorse_client-0.9.1/littlehorse/utils.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/worker.py` & `littlehorse_client-0.9.1/littlehorse/worker.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/littlehorse/workflow.py` & `littlehorse_client-0.9.1/littlehorse/workflow.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.9.0/pyproject.toml` & `littlehorse_client-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "littlehorse-client"
-version = "0.9.0"
+version = "0.9.1"
 description = "LittleHorse is a high-performance microservice orchestration engine that allows developers to build scalable, maintainable, and observable applications"
 authors = [ "LittleHorse Engineering <engineering@littlehorse.io>",]
 readme = "README.md"
 license = "SSPL-1.0"
 homepage = "https://littlehorse.dev"
 repository = "https://github.com/littlehorse-enterprises/littlehorse"
 documentation = "https://littlehorse.dev/docs/Overview"
```

### Comparing `littlehorse_client-0.9.0/PKG-INFO` & `littlehorse_client-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: littlehorse-client
-Version: 0.9.0
+Version: 0.9.1
 Summary: LittleHorse is a high-performance microservice orchestration engine that allows developers to build scalable, maintainable, and observable applications
 Home-page: https://littlehorse.dev
 License: SSPL-1.0
 Keywords: littlehorse
 Author: LittleHorse Engineering
 Author-email: engineering@littlehorse.io
 Requires-Python: >=3.9,<3.13
```

