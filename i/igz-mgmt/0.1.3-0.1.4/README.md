# Comparing `tmp/igz_mgmt-0.1.3.tar.gz` & `tmp/igz_mgmt-0.1.4.tar.gz`

## Comparing `igz_mgmt-0.1.3.tar` & `igz_mgmt-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/__init__.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/__version__.py
--rw-r--r--   0        0        0    16721 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/client.py
--rw-r--r--   0        0        0     7999 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/constants.py
--rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/cruds.py
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/exceptions.py
--rw-r--r--   0        0        0    10884 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/operations.py
--rw-r--r--   0        0        0    90860 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/resources.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/common/__init__.py
--rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/common/helpers.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/logger/__init__.py
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/logger/logger.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/schemas/__init__.py
--rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/schemas/app_services.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/schemas/events.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/igz_mgmt/schemas/manual_events.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/LICENSE
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/README.md
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 igz_mgmt-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/__init__.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/__version__.py
+-rw-r--r--   0        0        0    16721 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/client.py
+-rw-r--r--   0        0        0     7999 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/constants.py
+-rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/cruds.py
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/exceptions.py
+-rw-r--r--   0        0        0    10884 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/operations.py
+-rw-r--r--   0        0        0    92483 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/resources.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/common/__init__.py
+-rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/common/helpers.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/logger/__init__.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/logger/logger.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/schemas/__init__.py
+-rw-r--r--   0        0        0    13436 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/schemas/app_services.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/schemas/events.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/schemas/limits.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/igz_mgmt/schemas/manual_events.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/LICENSE
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/README.md
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 igz_mgmt-0.1.4/PKG-INFO
```

### Comparing `igz_mgmt-0.1.3/igz_mgmt/__init__.py` & `igz_mgmt-0.1.4/igz_mgmt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     AccessKey,
     AppServicesManifest,
     AuditEvent,
     CommunicationEvent,
     Event,
     Group,
     Job,
+    K8sConfig,
     Project,
     User,
 )
 
 # FOR BC
 ManualEventSchema = Event
 
@@ -69,14 +70,15 @@
     "AuditEvent",
     "CommunicationEvent",
     "ClusterConfigurations",
     "AppServicesManifest",
     "AppServiceBase",
     "AppServiceSpec",
     "AppServiceStatus",
+    "K8sConfig",
     "CustomAppServiceSpec",
     "JupyterSpec",
     "ScaleToZeroSpec",
     "ScaleResource",
     "ApplyServicesMode",
     "TenantManagementRoles",
     "ScaleToZeroMode",
```

### Comparing `igz_mgmt-0.1.3/igz_mgmt/__version__.py` & `igz_mgmt-0.1.4/igz_mgmt/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 #
 
 # version can be either one of the following:
 # x.y.z
 # x.y.z.rcN
 # x.y.zrcN
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
```

### Comparing `igz_mgmt-0.1.3/igz_mgmt/client.py` & `igz_mgmt-0.1.4/igz_mgmt/client.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.3/igz_mgmt/constants.py` & `igz_mgmt-0.1.4/igz_mgmt/constants.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.3/igz_mgmt/cruds.py` & `igz_mgmt-0.1.4/igz_mgmt/cruds.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,16 @@
             return _UserCrud
         elif crud_type == "user_group":
             return _UserGroupCrud
         elif crud_type == "access_key":
             return _AccessKeyCrud
         elif crud_type == "job":
             return _JobCrud
+        elif crud_type == "k8s_config":
+            return _K8sConfigCrud
         elif crud_type == "app_services_manifest":
             return _AppServicesManifestCrud
         elif crud_type == "project":
             return _ProjectCrud
         elif crud_type == "event":
             return _EventCrud
         elif crud_type == "audit_event":
@@ -184,14 +186,18 @@
     pass
 
 
 class _JobCrud(_BaseCrud):
     pass
 
 
+class _K8sConfigCrud(_BaseCrud):
+    pass
+
+
 class _AppServicesManifestCrud(_BaseCrud):
     __ALLOW_GET_DETAIL__ = False
 
 
 class _ProjectCrud(_BaseCrud):
     pass
```

### Comparing `igz_mgmt-0.1.3/igz_mgmt/exceptions.py` & `igz_mgmt-0.1.4/igz_mgmt/exceptions.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.3/igz_mgmt/operations.py` & `igz_mgmt-0.1.4/igz_mgmt/operations.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.3/igz_mgmt/resources.py` & `igz_mgmt-0.1.4/igz_mgmt/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 import igz_mgmt.common.helpers
 import igz_mgmt.constants
 import igz_mgmt.cruds
 import igz_mgmt.exceptions
 import igz_mgmt.schemas
 import igz_mgmt.schemas.app_services
 import igz_mgmt.schemas.events
+import igz_mgmt.schemas.limits
 
 
 class ResourceBaseModel(pydantic.BaseModel):
     """Base model for all resources."""
 
     type: str
     id: typing.Optional[typing.Union[int, str]]
@@ -1084,14 +1085,54 @@
             except Exception:
                 error_message += f", message: {job.result}"
 
             raise RuntimeError(error_message)
         http_client._logger.info_with("Job completed successfully", job_id=job_id)
 
 
+class K8sConfig(BaseResource):
+    """K8sConfig resource."""
+
+    type: str = "k8s_config"
+    namespace: str = ""
+    webapi_http_port: int = 0
+    webapi_https_port: int = 0
+    kubeconfig: str = ""
+    created_at: str = ""
+    updated_at: str = ""
+    services_spec: str = ""
+    services_status: str = ""
+    app_services_manifest: str = ""  # raw app services manifest
+    app_services: typing.List[igz_mgmt.schemas.app_services.AppServiceBase] = []
+    limit_range_spec: typing.Optional[igz_mgmt.schemas.limits.LimitRangeSpec] = None
+
+    @classmethod
+    def from_orm(cls, *args, **kwargs):
+        """Override this pydantic method to fill the app_services field."""
+        k8s_config = super().from_orm(*args, **kwargs)
+        app_services = json.loads(k8s_config.app_services_manifest)["app_services"]
+        for app_service in app_services:
+            # if app service dict contains status key but the value is empty dict we want to remove it
+            # because we want to cast it as pydantic AppServiceBase, and it doesn't support empty dict
+            if not app_service.get("status", True):
+                del app_service["status"]
+        k8s_config.app_services = app_services
+        return k8s_config
+
+    def delete(
+        self, http_client: igz_mgmt.client.APIClient, **kwargs
+    ) -> typing.Optional[Job]:
+        """This method is forbidden."""
+        raise igz_mgmt.exceptions.ResourceDeleteException
+
+    def update(self, http_client: igz_mgmt.client.APIClient, **kwargs):
+        """This method is not implemented yet."""
+        raise NotImplementedError
+
+
 class AppServicesManifest(BaseResource):
     """AppServicesManifest resource."""
 
     type: str = "app_services_manifest"
     cluster_name: str = ""
     tenant_name: str = ""
     tenant_id: str = ""
@@ -1151,15 +1192,15 @@
     def get(
         cls, http_client: igz_mgmt.client.APIClient, **kwargs
     ) -> "AppServicesManifest":
         """Gets the app services manifest from the API.
 
         Args:
             http_client (APIClient): The client to use.
-            **kwargs: Arbitrary keyword arguments (not in used).
+            **kwargs: Arbitrary keyword arguments (not used).
 
         Returns:
             AppServicesManifest: The app service manifest instance.
         """
         resource = cls._get_crud().list(http_client)
         return [
             cls.from_orm_with_client(http_client, {"data": item})
```

### Comparing `igz_mgmt-0.1.3/igz_mgmt/common/__init__.py` & `igz_mgmt-0.1.4/igz_mgmt/common/__init__.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.3/igz_mgmt/common/helpers.py` & `igz_mgmt-0.1.4/igz_mgmt/common/helpers.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.3/igz_mgmt/logger/__init__.py` & `igz_mgmt-0.1.4/igz_mgmt/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.3/igz_mgmt/logger/logger.py` & `igz_mgmt-0.1.4/igz_mgmt/logger/logger.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.3/igz_mgmt/schemas/__init__.py` & `igz_mgmt-0.1.4/igz_mgmt/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.3/igz_mgmt/schemas/app_services.py` & `igz_mgmt-0.1.4/igz_mgmt/schemas/app_services.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.3/igz_mgmt/schemas/events.py` & `igz_mgmt-0.1.4/igz_mgmt/schemas/events.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.3/igz_mgmt/schemas/manual_events.py` & `igz_mgmt-0.1.4/igz_mgmt/schemas/manual_events.py`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.3/LICENSE` & `igz_mgmt-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.3/pyproject.toml` & `igz_mgmt-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `igz_mgmt-0.1.3/PKG-INFO` & `igz_mgmt-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: igz-mgmt
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python SDK For Iguazio Management API
 Project-URL: Homepage, https://github.com/iguazio/igz-mgmt-sdk
 Author-email: Iguazio Platform Team <liranb@iguazio.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

