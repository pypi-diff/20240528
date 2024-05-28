# Comparing `tmp/cdk_webapp_skeleton-0.8.0.tar.gz` & `tmp/cdk_webapp_skeleton-0.8.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk_webapp_skeleton-0.8.0.tar", max compression
+gzip compressed data, was "cdk_webapp_skeleton-0.8.1.dev3.tar", max compression
```

## Comparing `cdk_webapp_skeleton-0.8.0.tar` & `cdk_webapp_skeleton-0.8.1.dev3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       64 2024-03-31 15:57:43.617603 cdk_webapp_skeleton-0.8.0/README.md
--rw-r--r--   0        0        0      463 2024-03-31 15:57:43.617603 cdk_webapp_skeleton-0.8.0/cdk_webapp_skeleton/__init__.py
--rw-r--r--   0        0        0     4307 2024-03-31 15:57:43.617603 cdk_webapp_skeleton-0.8.0/cdk_webapp_skeleton/auth_stack.py
--rw-r--r--   0        0        0     3070 2024-03-31 15:57:43.617603 cdk_webapp_skeleton-0.8.0/cdk_webapp_skeleton/branch_cicd_pipeline.py
--rw-r--r--   0        0        0     2593 2024-03-31 15:57:43.617603 cdk_webapp_skeleton-0.8.0/cdk_webapp_skeleton/branch_config.py
--rw-r--r--   0        0        0     4714 2024-03-31 15:57:43.617603 cdk_webapp_skeleton-0.8.0/cdk_webapp_skeleton/monitored_lambda_function.py
--rw-r--r--   0        0        0        0 2024-03-31 15:57:43.617603 cdk_webapp_skeleton-0.8.0/cdk_webapp_skeleton/py.typed
--rw-r--r--   0        0        0     4775 2024-03-31 15:57:43.617603 cdk_webapp_skeleton-0.8.0/cdk_webapp_skeleton/react_website.py
--rw-r--r--   0        0        0      447 2024-03-31 15:57:43.617603 cdk_webapp_skeleton-0.8.0/cdk_webapp_skeleton/test_utils.py
--rw-r--r--   0        0        0     5191 2024-03-31 15:57:43.617603 cdk_webapp_skeleton-0.8.0/cdk_webapp_skeleton/webapp_lambda.py
--rw-r--r--   0        0        0     1509 2024-03-31 15:58:00.597519 cdk_webapp_skeleton-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 cdk_webapp_skeleton-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       64 2024-05-28 04:02:38.152969 cdk_webapp_skeleton-0.8.1.dev3/README.md
+-rw-r--r--   0        0        0      463 2024-05-28 04:02:38.152969 cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/__init__.py
+-rw-r--r--   0        0        0     4144 2024-05-28 04:02:38.152969 cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/auth_stack.py
+-rw-r--r--   0        0        0     3070 2024-05-28 04:02:38.152969 cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/branch_cicd_pipeline.py
+-rw-r--r--   0        0        0     2996 2024-05-28 04:02:38.152969 cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/branch_config.py
+-rw-r--r--   0        0        0     4714 2024-05-28 04:02:38.152969 cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/monitored_lambda_function.py
+-rw-r--r--   0        0        0        0 2024-05-28 04:02:38.152969 cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/py.typed
+-rw-r--r--   0        0        0     4775 2024-05-28 04:02:38.152969 cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/react_website.py
+-rw-r--r--   0        0        0      447 2024-05-28 04:02:38.152969 cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/test_utils.py
+-rw-r--r--   0        0        0     5191 2024-05-28 04:02:38.152969 cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/webapp_lambda.py
+-rw-r--r--   0        0        0     1514 2024-05-28 04:03:28.536931 cdk_webapp_skeleton-0.8.1.dev3/pyproject.toml
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 cdk_webapp_skeleton-0.8.1.dev3/PKG-INFO
```

### Comparing `cdk_webapp_skeleton-0.8.0/cdk_webapp_skeleton/auth_stack.py` & `cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/auth_stack.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,22 +35,19 @@
         user_pool: cognito.IUserPool
 
         if branch_config.build_user_pool:
             user_pool = self.build_user_pool(branch_config)
         else:
             user_pool = self.find_user_pool()
 
-        development_signin_url = branch_config.dev_signin_redirect_url
-        production_signin_url = f"https://{branch_config.domain_name}/signin"
-
         frontend_pool_client = user_pool.add_client(
             "app-client",
             generate_secret=False,
             o_auth=cognito.OAuthSettings(
-                callback_urls=[development_signin_url, production_signin_url]
+                callback_urls=branch_config.signin_redirect_urls
             ),
             access_token_validity=cdk.Duration.days(1),
             refresh_token_validity=cdk.Duration.days(30),
         )
 
         self.outputs = AuthStackOutputs(
             cdk.CfnOutput(self, "UserPoolId", value=user_pool.user_pool_id),
```

### Comparing `cdk_webapp_skeleton-0.8.0/cdk_webapp_skeleton/branch_cicd_pipeline.py` & `cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/branch_cicd_pipeline.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.8.0/cdk_webapp_skeleton/branch_config.py` & `cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/branch_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import abc
+import warnings
 from abc import ABC
-from typing import Optional
+from typing import List, Optional
 
 from aws_cdk import aws_route53 as route53
 from aws_cdk import pipelines as pipelines
 from constructs import Construct
 
+HTTP_LOCALHOST_SIGNIN = "http://localhost:3000/signin"
+
 
 class BranchConfig(ABC):
     def __init__(self, branch_name: str):
         """
 
         :param branch_name:
         """
@@ -87,8 +90,17 @@
     def google_client_secret(self) -> Optional[str]:
         """Secret for Google OAuth."""
         return None
 
     @property
     def dev_signin_redirect_url(self) -> Optional[str]:
         """URL to redirect to after signing in during development."""
-        return "http://localhost:3000/signin"
+        warnings.warn(
+            "dev_signin_redirect_url will be deprecated in favor of overriding signin_redirect_urls",
+            DeprecationWarning,
+            stacklevel=3,
+        )
+        return HTTP_LOCALHOST_SIGNIN
+
+    @property
+    def signin_redirect_urls(self) -> List[str]:
+        return [HTTP_LOCALHOST_SIGNIN, f"https://{self.domain_name}/signin"]
```

### Comparing `cdk_webapp_skeleton-0.8.0/cdk_webapp_skeleton/monitored_lambda_function.py` & `cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/monitored_lambda_function.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.8.0/cdk_webapp_skeleton/react_website.py` & `cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/react_website.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.8.0/cdk_webapp_skeleton/webapp_lambda.py` & `cdk_webapp_skeleton-0.8.1.dev3/cdk_webapp_skeleton/webapp_lambda.py`

 * *Files identical despite different names*

### Comparing `cdk_webapp_skeleton-0.8.0/pyproject.toml` & `cdk_webapp_skeleton-0.8.1.dev3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cdk-webapp-skeleton"
-version = "0.8.0"
+version = "0.8.1.dev3"
 description = ""
 authors = ["Ilya Nekhay <nekhayiv@gmail.com>"]
 readme = "README.md"
 packages = [{include = "cdk_webapp_skeleton"}]
 
 [tool.poetry.dependencies]
 python = " >=3.8.1,<4"
```

### Comparing `cdk_webapp_skeleton-0.8.0/PKG-INFO` & `cdk_webapp_skeleton-0.8.1.dev3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-webapp-skeleton
-Version: 0.8.0
+Version: 0.8.1.dev3
 Summary: 
 Author: Ilya Nekhay
 Author-email: nekhayiv@gmail.com
 Requires-Python: >=3.8.1,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

