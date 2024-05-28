# Comparing `tmp/python-waldur-client-0.2.9.tar.gz` & `tmp/python-waldur-client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-waldur-client-0.2.9.tar", last modified: Wed Dec 13 16:59:04 2023, max compression
+gzip compressed data, was "python-waldur-client-0.3.0.tar", last modified: Tue May 28 16:54:48 2024, max compression
```

## Comparing `python-waldur-client-0.2.9.tar` & `python-waldur-client-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 16:59:04.830222 python-waldur-client-0.2.9/
--rw-rw-rw-   0 root         (0) root         (0)     1074 2023-12-13 16:57:42.000000 python-waldur-client-0.2.9/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      672 2023-12-13 16:59:04.830222 python-waldur-client-0.2.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-12-13 16:57:42.000000 python-waldur-client-0.2.9/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-12-13 16:59:04.830222 python-waldur-client-0.2.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-12-13 16:59:04.000000 python-waldur-client-0.2.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 16:59:04.830222 python-waldur-client-0.2.9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 16:59:04.830222 python-waldur-client-0.2.9/src/python_waldur_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      672 2023-12-13 16:59:04.000000 python-waldur-client-0.2.9/src/python_waldur_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      289 2023-12-13 16:59:04.000000 python-waldur-client-0.2.9/src/python_waldur_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-13 16:59:04.000000 python-waldur-client-0.2.9/src/python_waldur_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-12-13 16:59:04.000000 python-waldur-client-0.2.9/src/python_waldur_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-12-13 16:59:04.000000 python-waldur-client-0.2.9/src/python_waldur_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    77759 2023-12-13 16:57:42.000000 python-waldur-client-0.2.9/src/waldur_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:54:48.430096 python-waldur-client-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2024-05-28 16:53:36.000000 python-waldur-client-0.3.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      672 2024-05-28 16:54:48.430096 python-waldur-client-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      237 2024-05-28 16:53:36.000000 python-waldur-client-0.3.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 16:54:48.430096 python-waldur-client-0.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      799 2024-05-28 16:54:48.000000 python-waldur-client-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:54:48.430096 python-waldur-client-0.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 16:54:48.430096 python-waldur-client-0.3.0/src/python_waldur_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      672 2024-05-28 16:54:48.000000 python-waldur-client-0.3.0/src/python_waldur_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      289 2024-05-28 16:54:48.000000 python-waldur-client-0.3.0/src/python_waldur_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 16:54:48.000000 python-waldur-client-0.3.0/src/python_waldur_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-28 16:54:48.000000 python-waldur-client-0.3.0/src/python_waldur_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-28 16:54:48.000000 python-waldur-client-0.3.0/src/python_waldur_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    78399 2024-05-28 16:53:36.000000 python-waldur-client-0.3.0/src/waldur_client.py
```

### Comparing `python-waldur-client-0.2.9/LICENSE.md` & `python-waldur-client-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `python-waldur-client-0.2.9/PKG-INFO` & `python-waldur-client-0.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-waldur-client
-Version: 0.2.9
+Version: 0.3.0
 Summary: REST client for the Waldur API.
 Home-page: https://waldur.com
 Author: OpenNode Team
 Author-email: info@opennodecloud.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `python-waldur-client-0.2.9/setup.py` & `python-waldur-client-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 tests_requires = [
     "responses>=0.5.0",
     "pytest>=6.2.5",
 ]
 
 setup(
     name="python-waldur-client",
-    version="0.2.9",
+    version="0.3.0",
     author="OpenNode Team",
     author_email="info@opennodecloud.com",
     url="https://waldur.com",
     license="MIT",
     description="REST client for the Waldur API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `python-waldur-client-0.2.9/src/python_waldur_client.egg-info/PKG-INFO` & `python-waldur-client-0.3.0/src/python_waldur_client.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-waldur-client
-Version: 0.2.9
+Version: 0.3.0
 Summary: REST client for the Waldur API.
 Home-page: https://waldur.com
 Author: OpenNode Team
 Author-email: info@opennodecloud.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `python-waldur-client-0.2.9/src/waldur_client.py` & `python-waldur-client-0.3.0/src/waldur_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,17 +115,17 @@
     ADMINISTRATOR = "admin"
     MANAGER = "manager"
     MEMBER = "member"
 
 
 class SlurmAllocationState(Enum):
     CREATING = "creating"
-    UPDATE_SCHEDULED = "updating"
-    UPDATING = "deletion_scheduled"
-    DELETION_SCHEDULED = "update_scheduled"
+    UPDATE_SCHEDULED = "update_scheduled"
+    UPDATING = "updating"
+    DELETION_SCHEDULED = "deletion_scheduled"
     DELETING = "deleting"
     OK = "ok"
     ERRED = "erred"
 
 
 class PaymentProfileType(Enum):
     FIXED_PRICE = "fixed_price"
@@ -190,26 +190,28 @@
         SupportComments = "support-comments"
 
     marketplaceScopeEndpoints = {
         "OpenStackTenant.Instance": Endpoints.Instance,
         "OpenStackTenant.Volume": Endpoints.Volume,
     }
 
-    def __init__(self, api_url, access_token):
+    def __init__(self, api_url, access_token, user_agent=None):
         """
         Initializes a Waldur client
         :param api_url: a fully qualified URL to the Waldur API. Example: https://waldur.example.com:8000/api
         :param access_token: an access token to be used to communicate with the API.
         """
 
         self.api_url = self._ensure_trailing_slash(api_url)
         self.headers = {
             "Authorization": "token %s" % access_token,
             "Content-Type": "application/json",
         }
+        if user_agent is not None:
+            self.headers["User-Agent"] = user_agent
 
     def _ensure_trailing_slash(self, url):
         return url if url[-1] == "/" else "%s/" % url
 
     def _build_url(self, endpoint, action=None):
         parts = [endpoint]
         if action:
@@ -1783,21 +1785,42 @@
                 "resource_uuid": resource_uuid,
                 "date_after": date_after,
                 "date_before": date_before,
             },
         )
 
     def create_component_usages(
-        self, plan_period_uuid: str, usages: List[ComponentUsage]
+        self,
+        plan_period_uuid: str = None,
+        usages: List[ComponentUsage] = [],
+        resource_uuid=None,
     ):
         url = self._build_url(f"{self.Endpoints.ComponentUsage}/set_usage/")
         payload = {
-            "plan_period": plan_period_uuid,
             "usages": [dataclasses.asdict(usage) for usage in usages],
         }
+
+        if plan_period_uuid is not None:
+            payload.update(
+                {
+                    "plan_period": plan_period_uuid,
+                }
+            )
+        else:
+            if resource_uuid is not None:
+                payload.update(
+                    {
+                        "resource": resource_uuid,
+                    }
+                )
+            else:
+                raise ValidationError(
+                    "Neither plan_period_uuid nor resource_uuid provided"
+                )
+
         return self._post(url, valid_states=[201], json=payload)
 
     def get_remote_eduteams_user(self, cuid):
         return self._create_resource(
             self.Endpoints.RemoteEduteams,
             {
                 "cuid": cuid,
```

