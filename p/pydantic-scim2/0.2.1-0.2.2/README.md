# Comparing `tmp/pydantic_scim2-0.2.1.tar.gz` & `tmp/pydantic_scim2-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_scim2-0.2.1.tar", max compression
+gzip compressed data, was "pydantic_scim2-0.2.2.tar", max compression
```

## Comparing `pydantic_scim2-0.2.1.tar` & `pydantic_scim2-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2024-05-24 08:22:28.918776 pydantic_scim2-0.2.1/LICENSE
--rw-r--r--   0        0        0     1188 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.1/README.md
--rw-r--r--   0        0        0     2999 2024-05-27 09:29:26.944868 pydantic_scim2-0.2.1/pydantic_scim2/__init__.py
--rw-r--r--   0        0        0      358 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.1/pydantic_scim2/base.py
--rw-r--r--   0        0        0        0 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.1/pydantic_scim2/rfc7643/__init__.py
--rw-r--r--   0        0        0     1485 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.1/pydantic_scim2/rfc7643/enterprise_user.py
--rw-r--r--   0        0        0      782 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.1/pydantic_scim2/rfc7643/group.py
--rw-r--r--   0        0        0     7109 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.1/pydantic_scim2/rfc7643/resource.py
--rw-r--r--   0        0        0     4085 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.1/pydantic_scim2/rfc7643/resource_type.py
--rw-r--r--   0        0        0     2881 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.1/pydantic_scim2/rfc7643/schema.py
--rw-r--r--   0        0        0     5742 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.1/pydantic_scim2/rfc7643/service_provider.py
--rw-r--r--   0        0        0     9225 2024-05-27 10:11:32.665005 pydantic_scim2-0.2.1/pydantic_scim2/rfc7643/user.py
--rw-r--r--   0        0        0        0 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.1/pydantic_scim2/rfc7644/__init__.py
--rw-r--r--   0        0        0     1949 2024-05-27 10:03:41.991788 pydantic_scim2-0.2.1/pydantic_scim2/rfc7644/bulk.py
--rw-r--r--   0        0        0     2997 2024-05-27 09:29:26.944868 pydantic_scim2-0.2.1/pydantic_scim2/rfc7644/error.py
--rw-r--r--   0        0        0      845 2024-05-27 09:54:02.902271 pydantic_scim2-0.2.1/pydantic_scim2/rfc7644/list_response.py
--rw-r--r--   0        0        0      973 2024-05-27 09:56:02.875382 pydantic_scim2-0.2.1/pydantic_scim2/rfc7644/patch_op.py
--rw-r--r--   0        0        0     1460 2024-05-27 10:11:17.115016 pydantic_scim2-0.2.1/pydantic_scim2/rfc7644/search_request.py
--rw-r--r--   0        0        0     2634 2024-05-27 10:22:12.767709 pydantic_scim2-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2342 1970-01-01 00:00:00.000000 pydantic_scim2-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-24 08:22:28.918776 pydantic_scim2-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1188 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.2/README.md
+-rw-r--r--   0        0        0     3123 2024-05-28 11:29:24.030796 pydantic_scim2-0.2.2/pydantic_scim2/__init__.py
+-rw-r--r--   0        0        0      436 2024-05-28 11:29:24.054129 pydantic_scim2-0.2.2/pydantic_scim2/base.py
+-rw-r--r--   0        0        0        0 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.2/pydantic_scim2/rfc7643/__init__.py
+-rw-r--r--   0        0        0     1485 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.2/pydantic_scim2/rfc7643/enterprise_user.py
+-rw-r--r--   0        0        0      782 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.2/pydantic_scim2/rfc7643/group.py
+-rw-r--r--   0        0        0     4898 2024-05-28 13:27:36.151951 pydantic_scim2-0.2.2/pydantic_scim2/rfc7643/resource.py
+-rw-r--r--   0        0        0     1572 2024-05-28 13:22:03.659195 pydantic_scim2-0.2.2/pydantic_scim2/rfc7643/resource_type.py
+-rw-r--r--   0        0        0     2881 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.2/pydantic_scim2/rfc7643/schema.py
+-rw-r--r--   0        0        0     3229 2024-05-28 13:22:03.659195 pydantic_scim2-0.2.2/pydantic_scim2/rfc7643/service_provider.py
+-rw-r--r--   0        0        0     9225 2024-05-27 10:11:32.665005 pydantic_scim2-0.2.2/pydantic_scim2/rfc7643/user.py
+-rw-r--r--   0        0        0        0 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.2/pydantic_scim2/rfc7644/__init__.py
+-rw-r--r--   0        0        0     1949 2024-05-27 10:03:41.991788 pydantic_scim2-0.2.2/pydantic_scim2/rfc7644/bulk.py
+-rw-r--r--   0        0        0     5668 2024-05-28 11:24:52.498268 pydantic_scim2-0.2.2/pydantic_scim2/rfc7644/error.py
+-rw-r--r--   0        0        0      823 2024-05-28 11:29:24.034129 pydantic_scim2-0.2.2/pydantic_scim2/rfc7644/list_response.py
+-rw-r--r--   0        0        0      973 2024-05-27 09:56:02.875382 pydantic_scim2-0.2.2/pydantic_scim2/rfc7644/patch_op.py
+-rw-r--r--   0        0        0     1460 2024-05-27 10:11:17.115016 pydantic_scim2-0.2.2/pydantic_scim2/rfc7644/search_request.py
+-rw-r--r--   0        0        0     2632 2024-05-28 14:13:02.211193 pydantic_scim2-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2342 1970-01-01 00:00:00.000000 pydantic_scim2-0.2.2/PKG-INFO
```

### Comparing `pydantic_scim2-0.2.1/LICENSE` & `pydantic_scim2-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_scim2-0.2.1/README.md` & `pydantic_scim2-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_scim2-0.2.1/pydantic_scim2/__init__.py` & `pydantic_scim2-0.2.2/pydantic_scim2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .rfc7643.enterprise_user import EnterpriseUser
 from .rfc7643.enterprise_user import Manager
 from .rfc7643.group import Group
 from .rfc7643.group import GroupMember
+from .rfc7643.resource import AnyResource
 from .rfc7643.resource import Meta
 from .rfc7643.resource import Resource
 from .rfc7643.resource_type import ResourceType
 from .rfc7643.resource_type import SchemaExtension
 from .rfc7643.schema import Attribute
 from .rfc7643.schema import Mutability
 from .rfc7643.schema import Returned
@@ -44,17 +45,19 @@
 from .rfc7644.error import TooManyError
 from .rfc7644.error import UniquenessError
 from .rfc7644.list_response import ListResponse
 from .rfc7644.patch_op import Op
 from .rfc7644.patch_op import PatchOp
 from .rfc7644.patch_op import PatchOperation
 from .rfc7644.search_request import SearchRequest
+from .rfc7644.search_request import SortOrder
 
 __all__ = [
     "Address",
+    "AnyResource",
     "Attribute",
     "AuthenticationScheme",
     "Bulk",
     "BulkOperation",
     "BulkRequest",
     "BulkResponse",
     "ChangePassword",
@@ -88,14 +91,15 @@
     "Resource",
     "ResourceType",
     "Returned",
     "Role",
     "Schema",
     "SchemaExtension",
     "SearchRequest",
+    "SortOrder",
     "SensitiveError",
     "ServiceProviderConfiguration",
     "Sort",
     "TooManyError",
     "Uniqueness",
     "UniquenessError",
     "User",
```

### Comparing `pydantic_scim2-0.2.1/pydantic_scim2/rfc7643/enterprise_user.py` & `pydantic_scim2-0.2.2/pydantic_scim2/rfc7643/enterprise_user.py`

 * *Files identical despite different names*

### Comparing `pydantic_scim2-0.2.1/pydantic_scim2/rfc7643/group.py` & `pydantic_scim2-0.2.2/pydantic_scim2/rfc7643/group.py`

 * *Files identical despite different names*

### Comparing `pydantic_scim2-0.2.1/pydantic_scim2/rfc7643/schema.py` & `pydantic_scim2-0.2.2/pydantic_scim2/rfc7643/schema.py`

 * *Files identical despite different names*

### Comparing `pydantic_scim2-0.2.1/pydantic_scim2/rfc7643/user.py` & `pydantic_scim2-0.2.2/pydantic_scim2/rfc7643/user.py`

 * *Files identical despite different names*

### Comparing `pydantic_scim2-0.2.1/pydantic_scim2/rfc7644/bulk.py` & `pydantic_scim2-0.2.2/pydantic_scim2/rfc7644/bulk.py`

 * *Files identical despite different names*

### Comparing `pydantic_scim2-0.2.1/pydantic_scim2/rfc7644/patch_op.py` & `pydantic_scim2-0.2.2/pydantic_scim2/rfc7644/patch_op.py`

 * *Files identical despite different names*

### Comparing `pydantic_scim2-0.2.1/pydantic_scim2/rfc7644/search_request.py` & `pydantic_scim2-0.2.2/pydantic_scim2/rfc7644/search_request.py`

 * *Files identical despite different names*

### Comparing `pydantic_scim2-0.2.1/pyproject.toml` & `pydantic_scim2-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pydantic-scim2"
-version = "0.2.1"
+version = "0.2.2"
 description = "SCIM2 models for pydantic"
 authors = ["Yaal Coop <contact@yaal.coop>"]
 license = "Apache"
 readme = "README.md"
 keywords = ["scim", "scim2", "provisioning", "pydantic"]
 documentation = "https://pydantic-scim2.readthedocs.io"
 repository = "https://github.com/yaal-coop/pydantic-scim2"
@@ -59,15 +59,15 @@
 ]
 
 [tool.ruff.lint]
 select = [
     "E", # pycodestyle
     "F", # pyflakes
     "I", # isort
-    # "UP", # pyupgrade
+    "UP", # pyupgrade
 ]
 ignore = [
     "E501", # line-too-long
     "E722", # bare-except
 ]
 
 [tool.ruff.lint.isort]
```

### Comparing `pydantic_scim2-0.2.1/PKG-INFO` & `pydantic_scim2-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-scim2
-Version: 0.2.1
+Version: 0.2.2
 Summary: SCIM2 models for pydantic
 Home-page: https://github.com/yaal-coop/pydantic-scim2
 License: Apache
 Keywords: scim,scim2,provisioning,pydantic
 Author: Yaal Coop
 Author-email: contact@yaal.coop
 Requires-Python: >=3.9,<4.0
```

