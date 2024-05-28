# Comparing `tmp/celestical-0.18.5-py3-none-any.whl.zip` & `tmp/celestical-0.9.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,57 +1,61 @@
-Zip file size: 115471 bytes, number of entries: 55
+Zip file size: 115023 bytes, number of entries: 59
 -rw-r--r--  2.0 unx    35150 b- defN 80-Jan-01 00:00 COPYING
 -rw-r--r--  2.0 unx     7653 b- defN 80-Jan-01 00:00 COPYING.LESSER
 -rw-r--r--  2.0 unx      108 b- defN 80-Jan-01 00:00 LICENSE
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 celestical/__init__.py
--rw-r--r--  2.0 unx     2647 b- defN 80-Jan-01 00:00 celestical/api/__init__.py
+-rw-r--r--  2.0 unx     2650 b- defN 80-Jan-01 00:00 celestical/api/__init__.py
 -rw-r--r--  2.0 unx      246 b- defN 80-Jan-01 00:00 celestical/api/api/__init__.py
--rw-r--r--  2.0 unx    51131 b- defN 80-Jan-01 00:00 celestical/api/api/app_api.py
--rw-r--r--  2.0 unx    79145 b- defN 80-Jan-01 00:00 celestical/api/api/auth_api.py
--rw-r--r--  2.0 unx     9886 b- defN 80-Jan-01 00:00 celestical/api/api/default_api.py
--rw-r--r--  2.0 unx    51169 b- defN 80-Jan-01 00:00 celestical/api/api/users_api.py
--rw-r--r--  2.0 unx    24570 b- defN 80-Jan-01 00:00 celestical/api/api_client.py
+-rw-r--r--  2.0 unx    51215 b- defN 80-Jan-01 00:00 celestical/api/api/app_api.py
+-rw-r--r--  2.0 unx    79144 b- defN 80-Jan-01 00:00 celestical/api/api/auth_api.py
+-rw-r--r--  2.0 unx     9885 b- defN 80-Jan-01 00:00 celestical/api/api/default_api.py
+-rw-r--r--  2.0 unx    10780 b- defN 80-Jan-01 00:00 celestical/api/api/stacy_api.py
+-rw-r--r--  2.0 unx    51168 b- defN 80-Jan-01 00:00 celestical/api/api/users_api.py
+-rw-r--r--  2.0 unx    24568 b- defN 80-Jan-01 00:00 celestical/api/api_client.py
 -rw-r--r--  2.0 unx      674 b- defN 80-Jan-01 00:00 celestical/api/api_response.py
--rw-r--r--  2.0 unx    14610 b- defN 80-Jan-01 00:00 celestical/api/configuration.py
--rw-r--r--  2.0 unx     5940 b- defN 80-Jan-01 00:00 celestical/api/exceptions.py
--rw-r--r--  2.0 unx     1905 b- defN 80-Jan-01 00:00 celestical/api/models/__init__.py
--rw-r--r--  2.0 unx     3731 b- defN 80-Jan-01 00:00 celestical/api/models/app.py
--rw-r--r--  2.0 unx     2939 b- defN 80-Jan-01 00:00 celestical/api/models/bearer_response.py
--rw-r--r--  2.0 unx     2691 b- defN 80-Jan-01 00:00 celestical/api/models/body_reset_forgot_password_auth_forgot_password_post.py
--rw-r--r--  2.0 unx     2983 b- defN 80-Jan-01 00:00 celestical/api/models/body_reset_reset_password_auth_reset_password_post.py
--rw-r--r--  2.0 unx     2703 b- defN 80-Jan-01 00:00 celestical/api/models/body_verify_request_token_auth_request_verify_token_post.py
--rw-r--r--  2.0 unx     2631 b- defN 80-Jan-01 00:00 celestical/api/models/body_verify_verify_auth_verify_post.py
--rw-r--r--  2.0 unx     4815 b- defN 80-Jan-01 00:00 celestical/api/models/client_id.py
--rw-r--r--  2.0 unx     4843 b- defN 80-Jan-01 00:00 celestical/api/models/client_secret.py
--rw-r--r--  2.0 unx     4787 b- defN 80-Jan-01 00:00 celestical/api/models/code.py
--rw-r--r--  2.0 unx     2975 b- defN 80-Jan-01 00:00 celestical/api/models/compose.py
--rw-r--r--  2.0 unx     4801 b- defN 80-Jan-01 00:00 celestical/api/models/deploy.py
--rw-r--r--  2.0 unx     4912 b- defN 80-Jan-01 00:00 celestical/api/models/detail.py
--rw-r--r--  2.0 unx     2605 b- defN 80-Jan-01 00:00 celestical/api/models/error_model.py
--rw-r--r--  2.0 unx     4822 b- defN 80-Jan-01 00:00 celestical/api/models/grant_type.py
--rw-r--r--  2.0 unx     2602 b- defN 80-Jan-01 00:00 celestical/api/models/http_validation_error.py
--rw-r--r--  2.0 unx     4815 b- defN 80-Jan-01 00:00 celestical/api/models/is_active.py
--rw-r--r--  2.0 unx     4836 b- defN 80-Jan-01 00:00 celestical/api/models/is_superuser.py
--rw-r--r--  2.0 unx     4829 b- defN 80-Jan-01 00:00 celestical/api/models/is_verified.py
--rw-r--r--  2.0 unx     2639 b- defN 80-Jan-01 00:00 celestical/api/models/missing_images.py
--rw-r--r--  2.0 unx     4787 b- defN 80-Jan-01 00:00 celestical/api/models/name.py
--rw-r--r--  2.0 unx     2920 b- defN 80-Jan-01 00:00 celestical/api/models/uploaded_image.py
--rw-r--r--  2.0 unx     4757 b- defN 80-Jan-01 00:00 celestical/api/models/user_create.py
--rw-r--r--  2.0 unx     4111 b- defN 80-Jan-01 00:00 celestical/api/models/user_read.py
--rw-r--r--  2.0 unx     3083 b- defN 80-Jan-01 00:00 celestical/api/models/validation_error.py
+-rw-r--r--  2.0 unx    14608 b- defN 80-Jan-01 00:00 celestical/api/configuration.py
+-rw-r--r--  2.0 unx     5939 b- defN 80-Jan-01 00:00 celestical/api/exceptions.py
+-rw-r--r--  2.0 unx     1908 b- defN 80-Jan-01 00:00 celestical/api/models/__init__.py
+-rw-r--r--  2.0 unx     3730 b- defN 80-Jan-01 00:00 celestical/api/models/app.py
+-rw-r--r--  2.0 unx     2938 b- defN 80-Jan-01 00:00 celestical/api/models/bearer_response.py
+-rw-r--r--  2.0 unx     2690 b- defN 80-Jan-01 00:00 celestical/api/models/body_reset_forgot_password_auth_forgot_password_post.py
+-rw-r--r--  2.0 unx     2982 b- defN 80-Jan-01 00:00 celestical/api/models/body_reset_reset_password_auth_reset_password_post.py
+-rw-r--r--  2.0 unx     2702 b- defN 80-Jan-01 00:00 celestical/api/models/body_verify_request_token_auth_request_verify_token_post.py
+-rw-r--r--  2.0 unx     2630 b- defN 80-Jan-01 00:00 celestical/api/models/body_verify_verify_auth_verify_post.py
+-rw-r--r--  2.0 unx     4814 b- defN 80-Jan-01 00:00 celestical/api/models/client_id.py
+-rw-r--r--  2.0 unx     4842 b- defN 80-Jan-01 00:00 celestical/api/models/client_secret.py
+-rw-r--r--  2.0 unx     3040 b- defN 80-Jan-01 00:00 celestical/api/models/compose.py
+-rw-r--r--  2.0 unx     4800 b- defN 80-Jan-01 00:00 celestical/api/models/deploy.py
+-rw-r--r--  2.0 unx     4911 b- defN 80-Jan-01 00:00 celestical/api/models/detail.py
+-rw-r--r--  2.0 unx     2604 b- defN 80-Jan-01 00:00 celestical/api/models/error_model.py
+-rw-r--r--  2.0 unx     4842 b- defN 80-Jan-01 00:00 celestical/api/models/first_creator.py
+-rw-r--r--  2.0 unx     4821 b- defN 80-Jan-01 00:00 celestical/api/models/grant_type.py
+-rw-r--r--  2.0 unx     2601 b- defN 80-Jan-01 00:00 celestical/api/models/http_validation_error.py
+-rw-r--r--  2.0 unx     4814 b- defN 80-Jan-01 00:00 celestical/api/models/is_active.py
+-rw-r--r--  2.0 unx     4835 b- defN 80-Jan-01 00:00 celestical/api/models/is_superuser.py
+-rw-r--r--  2.0 unx     4828 b- defN 80-Jan-01 00:00 celestical/api/models/is_verified.py
+-rw-r--r--  2.0 unx     2622 b- defN 80-Jan-01 00:00 celestical/api/models/missing_apps.py
+-rw-r--r--  2.0 unx     2638 b- defN 80-Jan-01 00:00 celestical/api/models/missing_images.py
+-rw-r--r--  2.0 unx     4786 b- defN 80-Jan-01 00:00 celestical/api/models/name.py
+-rw-r--r--  2.0 unx     4225 b- defN 80-Jan-01 00:00 celestical/api/models/stack.py
+-rw-r--r--  2.0 unx     2919 b- defN 80-Jan-01 00:00 celestical/api/models/uploaded_image.py
+-rw-r--r--  2.0 unx     4425 b- defN 80-Jan-01 00:00 celestical/api/models/user_create.py
+-rw-r--r--  2.0 unx     4110 b- defN 80-Jan-01 00:00 celestical/api/models/user_read.py
+-rw-r--r--  2.0 unx     3082 b- defN 80-Jan-01 00:00 celestical/api/models/validation_error.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 celestical/api/py.typed
--rw-r--r--  2.0 unx     9782 b- defN 80-Jan-01 00:00 celestical/api/rest.py
--rw-r--r--  2.0 unx     1594 b- defN 80-Jan-01 00:00 celestical/apps.py
--rw-r--r--  2.0 unx     2520 b- defN 80-Jan-01 00:00 celestical/cli.py
--rw-r--r--  2.0 unx    23666 b- defN 80-Jan-01 00:00 celestical/compose.py
--rw-r--r--  2.0 unx     6974 b- defN 80-Jan-01 00:00 celestical/configuration.py
--rw-r--r--  2.0 unx    10101 b- defN 80-Jan-01 00:00 celestical/docker_local.py
--rw-r--r--  2.0 unx     9811 b- defN 80-Jan-01 00:00 celestical/helper.py
--rw-r--r--  2.0 unx     7436 b- defN 80-Jan-01 00:00 celestical/user.py
--rw-r--r--  2.0 unx    35150 b- defN 80-Jan-01 00:00 celestical-0.18.5.dist-info/COPYING
--rw-r--r--  2.0 unx     7653 b- defN 80-Jan-01 00:00 celestical-0.18.5.dist-info/COPYING.LESSER
--rw-r--r--  2.0 unx      108 b- defN 80-Jan-01 00:00 celestical-0.18.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     2587 b- defN 80-Jan-01 00:00 celestical-0.18.5.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 celestical-0.18.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 80-Jan-01 00:00 celestical-0.18.5.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     4904 b- defN 16-Jan-01 00:00 celestical-0.18.5.dist-info/RECORD
-55 files, 498874 bytes uncompressed, 107613 bytes compressed:  78.4%
+-rw-r--r--  2.0 unx     9781 b- defN 80-Jan-01 00:00 celestical/api/rest.py
+-rw-r--r--  2.0 unx     1533 b- defN 80-Jan-01 00:00 celestical/apps.py
+-rw-r--r--  2.0 unx     2425 b- defN 80-Jan-01 00:00 celestical/cli.py
+-rw-r--r--  2.0 unx    17341 b- defN 80-Jan-01 00:00 celestical/compose.py
+-rw-r--r--  2.0 unx     3900 b- defN 80-Jan-01 00:00 celestical/configuration.py
+-rw-r--r--  2.0 unx     6138 b- defN 80-Jan-01 00:00 celestical/docker_local.py
+-rw-r--r--  2.0 unx     6457 b- defN 80-Jan-01 00:00 celestical/helper.py
+-rw-r--r--  2.0 unx        9 b- defN 80-Jan-01 00:00 celestical/stack_upload.py
+-rw-r--r--  2.0 unx     6428 b- defN 80-Jan-01 00:00 celestical/user.py
+-rw-r--r--  2.0 unx    35150 b- defN 80-Jan-01 00:00 celestical-0.9.2.dist-info/COPYING
+-rw-r--r--  2.0 unx     7653 b- defN 80-Jan-01 00:00 celestical-0.9.2.dist-info/COPYING.LESSER
+-rw-r--r--  2.0 unx      108 b- defN 80-Jan-01 00:00 celestical-0.9.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1959 b- defN 80-Jan-01 00:00 celestical-0.9.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 celestical-0.9.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 80-Jan-01 00:00 celestical-0.9.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     5255 b- defN 16-Jan-01 00:00 celestical-0.9.2.dist-info/RECORD
+59 files, 498201 bytes uncompressed, 106609 bytes compressed:  78.6%
```

## zipnote {}

```diff
@@ -21,14 +21,17 @@
 
 Filename: celestical/api/api/auth_api.py
 Comment: 
 
 Filename: celestical/api/api/default_api.py
 Comment: 
 
+Filename: celestical/api/api/stacy_api.py
+Comment: 
+
 Filename: celestical/api/api/users_api.py
 Comment: 
 
 Filename: celestical/api/api_client.py
 Comment: 
 
 Filename: celestical/api/api_response.py
@@ -63,29 +66,29 @@
 
 Filename: celestical/api/models/client_id.py
 Comment: 
 
 Filename: celestical/api/models/client_secret.py
 Comment: 
 
-Filename: celestical/api/models/code.py
-Comment: 
-
 Filename: celestical/api/models/compose.py
 Comment: 
 
 Filename: celestical/api/models/deploy.py
 Comment: 
 
 Filename: celestical/api/models/detail.py
 Comment: 
 
 Filename: celestical/api/models/error_model.py
 Comment: 
 
+Filename: celestical/api/models/first_creator.py
+Comment: 
+
 Filename: celestical/api/models/grant_type.py
 Comment: 
 
 Filename: celestical/api/models/http_validation_error.py
 Comment: 
 
 Filename: celestical/api/models/is_active.py
@@ -93,20 +96,26 @@
 
 Filename: celestical/api/models/is_superuser.py
 Comment: 
 
 Filename: celestical/api/models/is_verified.py
 Comment: 
 
+Filename: celestical/api/models/missing_apps.py
+Comment: 
+
 Filename: celestical/api/models/missing_images.py
 Comment: 
 
 Filename: celestical/api/models/name.py
 Comment: 
 
+Filename: celestical/api/models/stack.py
+Comment: 
+
 Filename: celestical/api/models/uploaded_image.py
 Comment: 
 
 Filename: celestical/api/models/user_create.py
 Comment: 
 
 Filename: celestical/api/models/user_read.py
@@ -135,32 +144,35 @@
 
 Filename: celestical/docker_local.py
 Comment: 
 
 Filename: celestical/helper.py
 Comment: 
 
+Filename: celestical/stack_upload.py
+Comment: 
+
 Filename: celestical/user.py
 Comment: 
 
-Filename: celestical-0.18.5.dist-info/COPYING
+Filename: celestical-0.9.2.dist-info/COPYING
 Comment: 
 
-Filename: celestical-0.18.5.dist-info/COPYING.LESSER
+Filename: celestical-0.9.2.dist-info/COPYING.LESSER
 Comment: 
 
-Filename: celestical-0.18.5.dist-info/LICENSE
+Filename: celestical-0.9.2.dist-info/LICENSE
 Comment: 
 
-Filename: celestical-0.18.5.dist-info/METADATA
+Filename: celestical-0.9.2.dist-info/METADATA
 Comment: 
 
-Filename: celestical-0.18.5.dist-info/WHEEL
+Filename: celestical-0.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: celestical-0.18.5.dist-info/entry_points.txt
+Filename: celestical-0.9.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: celestical-0.18.5.dist-info/RECORD
+Filename: celestical-0.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## celestical/api/__init__.py

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 __version__ = "1.0.0"
@@ -38,16 +38,16 @@
 from celestical.api.models.bearer_response import BearerResponse
 from celestical.api.models.body_reset_forgot_password_auth_forgot_password_post import BodyResetForgotPasswordAuthForgotPasswordPost
 from celestical.api.models.body_reset_reset_password_auth_reset_password_post import BodyResetResetPasswordAuthResetPasswordPost
 from celestical.api.models.body_verify_request_token_auth_request_verify_token_post import BodyVerifyRequestTokenAuthRequestVerifyTokenPost
 from celestical.api.models.body_verify_verify_auth_verify_post import BodyVerifyVerifyAuthVerifyPost
 from celestical.api.models.client_id import ClientId
 from celestical.api.models.client_secret import ClientSecret
-from celestical.api.models.code import Code
 from celestical.api.models.compose import Compose
+from celestical.api.models.deploy import Deploy
 from celestical.api.models.detail import Detail
 from celestical.api.models.error_model import ErrorModel
 from celestical.api.models.grant_type import GrantType
 from celestical.api.models.http_validation_error import HTTPValidationError
 from celestical.api.models.is_active import IsActive
 from celestical.api.models.is_superuser import IsSuperuser
 from celestical.api.models.is_verified import IsVerified
```

## celestical/api/api/app_api.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
@@ -561,30 +561,30 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def get_user_apps_app_get(
+    def get_latest_created_apps_app_get(
         self,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> object:
-        """Get User Apps
+    ) -> App:
+        """Get Latest Created Apps
 
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -601,52 +601,52 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_user_apps_app_get_serialize(
+        _param = self._get_latest_created_apps_app_get_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "App",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def get_user_apps_app_get_with_http_info(
+    def get_latest_created_apps_app_get_with_http_info(
         self,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[object]:
-        """Get User Apps
+    ) -> ApiResponse[App]:
+        """Get Latest Created Apps
 
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -663,52 +663,52 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_user_apps_app_get_serialize(
+        _param = self._get_latest_created_apps_app_get_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "App",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def get_user_apps_app_get_without_preload_content(
+    def get_latest_created_apps_app_get_without_preload_content(
         self,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Get User Apps
+        """Get Latest Created Apps
 
 
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
@@ -725,32 +725,32 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_user_apps_app_get_serialize(
+        _param = self._get_latest_created_apps_app_get_serialize(
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "object",
+            '200': "App",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _get_user_apps_app_get_serialize(
+    def _get_latest_created_apps_app_get_serialize(
         self,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
```

## celestical/api/api/auth_api.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

## celestical/api/api/default_api.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

## celestical/api/api/users_api.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

## celestical/api/api_client.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import atexit
@@ -82,15 +82,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'celestical/py/0.18.5'
+        self.user_agent = 'celestical/py/0.6.6'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

## celestical/api/configuration.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import copy
@@ -371,15 +371,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.16.3\n"\
+               "Version of the API: 0.8.1\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

## celestical/api/exceptions.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from typing import Any, Optional
```

## celestical/api/models/__init__.py

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
@@ -18,16 +18,16 @@
 from celestical.api.models.bearer_response import BearerResponse
 from celestical.api.models.body_reset_forgot_password_auth_forgot_password_post import BodyResetForgotPasswordAuthForgotPasswordPost
 from celestical.api.models.body_reset_reset_password_auth_reset_password_post import BodyResetResetPasswordAuthResetPasswordPost
 from celestical.api.models.body_verify_request_token_auth_request_verify_token_post import BodyVerifyRequestTokenAuthRequestVerifyTokenPost
 from celestical.api.models.body_verify_verify_auth_verify_post import BodyVerifyVerifyAuthVerifyPost
 from celestical.api.models.client_id import ClientId
 from celestical.api.models.client_secret import ClientSecret
-from celestical.api.models.code import Code
 from celestical.api.models.compose import Compose
+from celestical.api.models.deploy import Deploy
 from celestical.api.models.detail import Detail
 from celestical.api.models.error_model import ErrorModel
 from celestical.api.models.grant_type import GrantType
 from celestical.api.models.http_validation_error import HTTPValidationError
 from celestical.api.models.is_active import IsActive
 from celestical.api.models.is_superuser import IsSuperuser
 from celestical.api.models.is_verified import IsVerified
```

## celestical/api/models/app.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/bearer_response.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/body_reset_forgot_password_auth_forgot_password_post.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/body_reset_reset_password_auth_reset_password_post.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/body_verify_request_token_auth_request_verify_token_post.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/body_verify_verify_auth_verify_post.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/client_id.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/client_secret.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/compose.py

```diff
@@ -1,40 +1,41 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
 from pydantic import BaseModel
+from celestical.api.models.deploy import Deploy
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 class Compose(BaseModel):
     """
     Manages enriched compose info including which App they represent
     """ # noqa: E501
     enriched_compose: Optional[Any]
-    deploy: Optional[Any] = None
+    deploy: Optional[Deploy] = None
     __properties: ClassVar[List[str]] = ["enriched_compose", "deploy"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
@@ -66,35 +67,33 @@
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={
             },
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of deploy
+        if self.deploy:
+            _dict['deploy'] = self.deploy.to_dict()
         # set to None if enriched_compose (nullable) is None
         # and model_fields_set contains the field
         if self.enriched_compose is None and "enriched_compose" in self.model_fields_set:
             _dict['enriched_compose'] = None
 
-        # set to None if deploy (nullable) is None
-        # and model_fields_set contains the field
-        if self.deploy is None and "deploy" in self.model_fields_set:
-            _dict['deploy'] = None
-
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of Compose from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "enriched_compose": obj.get("enriched_compose"),
-            "deploy": obj.get("deploy")
+            "deploy": Deploy.from_dict(obj.get("deploy")) if obj.get("deploy") is not None else None
         })
         return _obj
```

## celestical/api/models/deploy.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.15.2
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/detail.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/error_model.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/grant_type.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/http_validation_error.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/is_active.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/is_superuser.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/is_verified.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/missing_images.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/name.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/uploaded_image.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/user_create.py

```diff
@@ -1,30 +1,29 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
 from pydantic import BaseModel
-from celestical.api.models.code import Code
 from celestical.api.models.is_active import IsActive
 from celestical.api.models.is_superuser import IsSuperuser
 from celestical.api.models.is_verified import IsVerified
 from celestical.api.models.name import Name
 try:
     from typing import Self
 except ImportError:
@@ -36,16 +35,15 @@
     """ # noqa: E501
     email: Optional[Any]
     password: Optional[Any]
     is_active: Optional[IsActive] = None
     is_superuser: Optional[IsSuperuser] = None
     is_verified: Optional[IsVerified] = None
     name: Optional[Name] = None
-    code: Optional[Code] = None
-    __properties: ClassVar[List[str]] = ["email", "password", "is_active", "is_superuser", "is_verified", "name", "code"]
+    __properties: ClassVar[List[str]] = ["email", "password", "is_active", "is_superuser", "is_verified", "name"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -88,17 +86,14 @@
             _dict['is_superuser'] = self.is_superuser.to_dict()
         # override the default output from pydantic by calling `to_dict()` of is_verified
         if self.is_verified:
             _dict['is_verified'] = self.is_verified.to_dict()
         # override the default output from pydantic by calling `to_dict()` of name
         if self.name:
             _dict['name'] = self.name.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of code
-        if self.code:
-            _dict['code'] = self.code.to_dict()
         # set to None if email (nullable) is None
         # and model_fields_set contains the field
         if self.email is None and "email" in self.model_fields_set:
             _dict['email'] = None
 
         # set to None if password (nullable) is None
         # and model_fields_set contains the field
@@ -118,13 +113,12 @@
 
         _obj = cls.model_validate({
             "email": obj.get("email"),
             "password": obj.get("password"),
             "is_active": IsActive.from_dict(obj.get("is_active")) if obj.get("is_active") is not None else None,
             "is_superuser": IsSuperuser.from_dict(obj.get("is_superuser")) if obj.get("is_superuser") is not None else None,
             "is_verified": IsVerified.from_dict(obj.get("is_verified")) if obj.get("is_verified") is not None else None,
-            "name": Name.from_dict(obj.get("name")) if obj.get("name") is not None else None,
-            "code": Code.from_dict(obj.get("code")) if obj.get("code") is not None else None
+            "name": Name.from_dict(obj.get("name")) if obj.get("name") is not None else None
         })
         return _obj
```

## celestical/api/models/user_read.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/models/validation_error.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
```

## celestical/api/rest.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.8.1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import io
```

## celestical/apps.py

```diff
@@ -1,34 +1,33 @@
 """ Apps related actions
 """
 from celestical.configuration import (
-    API_URL, cli_logger)
+    apiconf, cli_logger)
 from celestical.helper import cli_panel
 from celestical import api
 from celestical.api.exceptions import UnauthorizedException
 from celestical.user import load_user_creds
 
 # logging.basicConfig(encoding='utf-8', level=LOGGING_LEVEL)
 
 
 def list_creator_apps() -> bool:
     """ List /app/ the latest created apps """
- 
-    apiconf = api.Configuration(host=API_URL)
+
     setcred, msg = load_user_creds(apiconf)
     if setcred is False:
         cli_panel(msg)
         return False
 
     api_response = None
     with api.ApiClient(apiconf) as api_client:
         app_api = api.AppApi(api_client)
 
         try:
-            api_response = app_api.get_user_apps_app_get()
+            api_response = app_api.get_latest_created_apps_app_get()
 
         except UnauthorizedException as oops:
             cli_panel("You might have to login again, Your token expired.")
             return False
         except Exception as oops:
             cli_logger.debug(oops)
             cli_panel("Could not connect; check your connection.")
@@ -40,13 +39,13 @@
 
     msg = "\n"
     deployed_wip = False
     for app in show_res:
         dcolor = "red"
         if deployed_wip is True:
             dcolor = "blue"
-        msg += f" - [{dcolor}][underline]{app.get('url','[no url]')}[/underline][/{dcolor}]"
-        msg += f" [yellow]{app['id']}[/yellow]"
-        msg += f" created on {app['created_date']}\n"
+        msg += f" - [{dcolor}][underline]{app.url}[/underline][/{dcolor}]"
+        msg += f" [yellow]{app.id}[/yellow]"
+        msg += f" created on {app.created_date}\n"
 
     cli_panel(msg, _title="Celestical - Your apps")
     return True
```

## celestical/cli.py

```diff
@@ -6,58 +6,58 @@
 
 import typer
 
 from celestical.compose import (
     upload_compose,
     upload_images)
 from celestical.docker_local import list_local_images
-from celestical.helper import cli_panel, print_text, print_feedback
-from celestical.configuration import cli_logger, welcome
+from celestical.helper import cli_panel, welcome_message
+from celestical.configuration import cli_logger
 from celestical.user import user_login, user_register
 from celestical.apps import list_creator_apps
 
 
 cli_logger.info("Starting CLI.")
 
 app = typer.Typer(pretty_exceptions_short=False,
                   no_args_is_help=True,
-                  help=welcome(),
+                  help=welcome_message,
                   rich_markup_mode="rich")
+cli_logger.debug("Typer created successfully.")
 
 # @app.callback(invoke_without_command=True)
 @app.command()
 def apps():
     """List all apps from current user."""
     list_creator_apps()
 
 
 @app.command()
 def login() -> None:
     """Login to Parametry's Celestical Cloud Services via the CLI."""
+    cli_logger.debug("Entering the login function")
     user_login()
 
 
 @app.command()
 def register():
     """Register as a user for Celestical Cloud Services via the CLI."""
-    if not user_register():
-        print_text("User already exists or We could not connect.")
-    else:
-        print_feedback("Your account has been created.")
+    user_register()
 
 
 @app.command()
 def images():
     """ List all local docker images for you.
         Similar to 'docker image ls'.
     """
-    table = list_local_images()
+    table, err_msg = list_local_images()
 
-    if table is None:
-        cli_panel("Docker service is [red]unaccessible[/red]\n")
+    if table is None or err_msg != "":
+        cli_panel("Docker service is [red]unaccessible[/red]\n\n"
+                 +f"{err_msg}")
     else:
         cli_panel("The following are your local docker images\n"
                  +f"{table}")
 
 
 @app.command()
 def deploy(compose_path: Annotated[Optional[str], typer.Argument()] = "./"):
@@ -70,15 +70,13 @@
     # --- Upload images according to response
     # 1- read response, and feedback user on status
     # 2- if 200, select the list of images in response.
     # 3- compress concerned images
     # 4- upload concerned images
     # .. keep feedback to user whenever progress is made
     if enriched_compose is None:
-        msg = "To continue with deployment you need a celestical account.\n"
-        msg += "see command: [yellow]celestical register[/yellow]"
-        cli_panel(msg)
+        cli_panel("Stopping here - could not enriched compose file")
         return
 
     upload_images(app_uuid=enriched_compose["celestical"]["app_id"], e_compose=enriched_compose)
```

## celestical/compose.py

```diff
@@ -1,10 +1,9 @@
 """ File to manage docker compose file and their enrichment """
 import sys
-import os
 from pathlib import Path
 from typing import Tuple
 
 import uuid
 import yaml
 import typer
 import docker
@@ -27,252 +26,73 @@
     cli_panel,
     prompt_user,
     confirm_user,
     print_text,
     print_feedback,
     guess_service_type_by_name,
     save_yaml,
-    get_most_recent_file,
-    extract_all_dollars,
-    dict_to_list_env,
     SERVICE_TYPES)
 
 from celestical.configuration import (
     HOTLINE,
-    API_URL,
+    apiconf,
     cli_logger,
     load_config)
 
 
-#class ComposeEnricher():
-#    def __init__():
-#
-#        # Keep a dictionary of missing variables with their
-#        # name as key and $REF_IN_ENV as value.
-#        missing_variables = {}
+def get_image_hash(image_name_tag:str) -> str:
+    """Get the hash for a certain docker image name and tag."""
 
-def _get_api_with_auth():
-    apiconf = api.Configuration(host=API_URL)
-    setcred, mesg = load_user_creds(apiconf)
-    if setcred is False:
-        cli_panel(mesg)
-        return None
-    return apiconf
+    client = docker.from_env()
+    image = client.images.get(image_name_tag)
+    return image.id
+
+
+def get_ports(image_id, docker_client):
+    """Get ports from containers created from the specified image."""
+    ports = set()
+    for container in docker_client.containers.list(all=True):
+        if container.image.id == image_id:
+            port_data = container.attrs['HostConfig']['PortBindings']
+            if port_data:
+                for port, bindings in port_data.items():
+                    # get only the port number, not the protocol
+                    ports.add(port.split('/')[0])
+    return ', '.join(sorted(ports))
 
 
 def richformat_services(services:dict) -> str:
     """Create a rich formatted string to display a bullet list for services
     """
     s_info = ""
     for serv in services:
         if "image" not in services[serv]:
             services[serv]["image"] = "-undefined-"
         s_info += f"\t- [yellow]{serv}[/yellow] (image)--> "
         s_info += f"{services[serv]['image']}\n"
     return s_info
 
 
-def load_dot_env(env_dir:Path) -> dict:
-    """ Read the .env file and extract all variables
-
-    Returns:
-        a dictionary of key value of these env variables.
-    """
-    env_file = env_dir / ".env"
-    return load_env_file(env_file)
-
-
-def load_env_file(env_file:Path) -> dict:
-    """ Read the env_file and extract all variables name and value
-
-    Returns:
-        a dictionary of key value of these env variables.
-    """
-    loaded_env = {}
-
-    # - load the content of .env
-    if not env_file.is_file():
-        return loaded_env
-
-    with env_file.open(mode="r") as fdesc:
-        for line in fdesc:
-            line = line.strip()
-            if not line:
-                continue
-
-            if line[0] == '#':
-                continue
-
-            split_line = line.split('=', 1)
-            if len(split_line) == 2:
-                k, v = split_line
-                loaded_env[k] = v
-            # else line is ignored
-            # .env file is supposed to define stuffs
-    return loaded_env
-
-
-def _apply_os_env(denv:dict) -> dict:
-    """ For key value dictionary where value is empty (None)
-     - set the potential value from key as variable in the the OS/Shell environment
-     OR
-     - set it to "1" as required in the docker reference.
-
-     None must be set prior to processing here as an empty string might be what
-     a user exactly wants. None or empty value are the same when read by
-     yaml.safe_load.
-
-     Requirement all output values must be strings
-
-    """
-    for key in denv:
-        if denv[key] is None:
-            if key in os.environ:
-                denv[key] = os.environ[key]
-            else:
-                denv[key] = "1"
-    return denv
-
-
-def _separate_kvpairs(env:list) -> dict:
-    """ For an input list of "KEY=VALUE" separate everything in a dictionary
-    for accessing KEY: VALUE easily
-     - if no value is found just set a the value of a KEY as an empty string
-
-    """
-    compose_env = {}
-
-    for vardef in env:
-        vardef = vardef.strip()
-        varsplit = vardef.split('=', 1)
-        if len(varsplit) == 2:
-            compose_env[varsplit[0]] = varsplit[1]
-        elif len(varsplit) == 1:
-            compose_env[varsplit[0]] = None
-
-    compose_env = _apply_os_env(compose_env)
-
-    return compose_env
-
-
-def _apply_variables(env:list|dict, loaded_env:dict) -> list:
-    """ Read the .env file and replace all variables in the env list with their
-    compose_env = {}
-
-    Params:
-        env(list): is the list of strings from environment field in
-        the docker-compose file
-        loaded_env
-    """
-    # - loading the content of env list of strings
-    compose_env = {}
-
-    if isinstance(env, list):
-        compose_env = _separate_kvpairs(env)
-    elif isinstance(env, dict):
-        compose_env = _apply_os_env(env)
-
-    # - now applying .env (loaded_env) to compose_env
-    for k in compose_env:
-        if "$" in compose_env[k]:
-            # v2d var to dollars
-            v2d = extract_all_dollars(compose_env[k])
-            for v in v2d:
-                if v in loaded_env:
-                    # replace the dollar variable
-                    # with loaded_env corresponding value
-                    compose_env[k] = compose_env[k].replace(
-                                        v2d[v],
-                                        loaded_env[v])
-                elif v in os.environ:
-                    compose_env[k] = compose_env[k].replace(
-                                        v2d[v],
-                                        os.environ[v])
-
-    # - join both env and return, update loaded with modified compose_env
-    #loaded_env.update(compose_env)
-
-    return compose_env
-
-
-def integrate_all_env(comp:dict, env_dir:Path) -> dict:
-    """Read all files from docker-compose environment and env_files
-       and loads their content to re-express it in the compose environment list
-       of each services.
-
-    Returns:
-        the fully integrated compose dictionary
-    """
-    dot_env = load_dot_env(env_dir)
-
-    for key in comp.get("services", {}):
-        # Variables to develop
-        env = comp["services"][key].get("environment", None)
-        if env is not None:
-            comp["services"][key]["environment"] = _apply_variables(
-                env,
-                dot_env)
-
-        # environt from envfiles to add
-        env_files = comp["services"][key].get("env_files", [])
-        key_env = {}
-        for efile in env_files:
-            key_env.update(load_env_file(env_dir / efile))
-
-        if env is None:
-            comp["services"][key]["environment"] = key_env
-        else:
-            comp["services"][key]["environment"].update(key_env)
-
-    return comp
-
-
-def read_docker_compose(fullpath:Path, integrate_env_files:bool=True) -> dict:
-    """ Read a docker-compose.yml file.
-        and integrates environment variables from files.
+def read_docker_compose(fullpath: Path) -> dict:
+    """Read the docker-compose.yml file.
 
     Params:
         fullpath(Path): absolut path to the docker-compose.yml file
     Returns:
         (dict): docker-compose.yml file content
     """
 
-    compose = {}
-    msg = ""
-    if not isinstance(fullpath, Path):
-        fullpath = Path(str(fullpath))
-
-    def logerror(message:str):
-        print_text(message)
-        cli_logger.error(message)
-
-    if fullpath.is_dir():
-        logerror(f"Path is not a file: {fullpath}")
-        return {}
-
-    if fullpath.is_file():
-        try:
-            with fullpath.open(mode='r') as f:
-                compose = yaml.safe_load(f)
-                if compose is None:
-                    compose = {}
-        except FileNotFoundError:
-            logerror(f"No file found at given path: {fullpath}")
-            return {}
-    else:
-        logerror(f"No file found at given path: {fullpath}")
-        return {}
-
-    if compose == {}:
-        # - nothing is to be done here
-        return compose
-
-    # - loading potential environment variables and files
-    compose = integrate_all_env(compose, fullpath.parent)
-
+    compose = None
+    try:
+        with open(fullpath, 'r') as f:
+            compose = yaml.safe_load(f)
+    except FileNotFoundError:
+        msg = f"No file found at given path: {fullpath}"
+        print_text(msg)
+        cli_logger.error(msg)
     return compose
 
 
 def enrich_compose(
     compose: dict,
     prev_comp:dict = {},
     ecomp_path:Path = None) -> Path:
@@ -396,50 +216,14 @@
         # enriched_compose["services"][service_name]["celestical_image_hash"] = service_name["image"]
         counter += 1
 
     save_path: Path = save_yaml(data=enriched_compose, yml_file=ecomp_path)
     return save_path
 
 
-def define_compose_path(input_path:str) -> Tuple[Path, Path]:
-    """ Form the paths to docker-compose file and its enrichment
-        according to the type of the input_path
-
-        returns (compose_filepath, enriched_filepath)
-    """
-    # use current directory if nothing provided
-    docker_compose_path = Path.cwd()
-    docker_ecompose_path = Path.cwd() / 'docker-compose-enriched_TBD-noexist.yml'
-
-    if input_path is not None:
-        if input_path != "":
-            docker_compose_path = Path(input_path)
-
-    # if we get a directory, complete full path
-    selected_path = None
-    # if input is directory we have to find the file
-    if docker_compose_path.is_dir():
-        docker_ecompose_path = docker_compose_path / \
-          '.docker-compose-enriched.yml'
-        docker_compose_path = docker_compose_path / 'docker-compose.yml'
-        if not docker_compose_path.is_file():
-            docker_compose_path = docker_compose_path.parent / 'compose.yml'
-            # further checks will be done later
-    elif docker_compose_path.is_file():
-        # we consider docker_compose_path a valid file set from user
-        # We try to find the enriched file
-        file_dir = docker_compose_path.parent
-        docker_ecompose_path = file_dir / '.docker-compose-enriched.yml'
-    else:
-        # provided path is neither a directory or file, e_xit info
-        return (None, None)
-
-    return (docker_compose_path, docker_ecompose_path)
-
-
 def check_for_enrichment(compose_path:str) -> Tuple[Path, dict, dict]:
     """ Find the compose file in the given folder if it is a folder and decide
     where the enriched compose file will be. Check with the user if enrichment
     is necessary when already present
 
         Returns: three elements:
          - the path to the found most recent docker-compose or enriched
@@ -447,138 +231,151 @@
          - the python dictionary of that most recent compose file content with
            first metadata containing info if user wants to enrich or not.
            From confirmation ask thanks to timestamp comparison.
          - the python dictionary of the enriched file anyway found, so it can be
            used for default values while enrichiing to fasten and ease the
            process.
     """
-    compose_path, ecompose_path = define_compose_path(compose_path)
 
-    # in case file name could not be defined
-    # (different from file does not exist)
-    if compose_path is None or ecompose_path is None:
-        cli_panel("docker-compose.yml or compose.yml files are not valid files:\n"
+    # use current directory if nothing provided
+    docker_compose_path = Path.cwd()
+    docker_ecompose_path = Path.cwd() / 'docker-compose-enriched_dpath.yml'
+    if compose_path is not None:
+        if compose_path != "":
+            docker_compose_path = Path(compose_path)
+
+    # if we get a directory, complete full path
+    selected_path = None
+    prev_compose = {}
+    if docker_compose_path.is_dir():
+        docker_ecompose_path = docker_compose_path / \
+          'docker-compose-enriched.yml'
+        docker_compose_path = docker_compose_path / 'docker-compose.yml'
+    elif docker_compose_path.is_file():
+        # we consider docker_compose_path a valid file set from user
+        # We try to find the enriched file
+        file_dir = docker_compose_path.parent
+        docker_ecompose_path = file_dir / 'docker-compose-enriched.yml'
+    else:
+        # provided path is neither a directory or file, e_xit.
+        cli_panel("docker-compose.yml file is not a valid file:\n"
+                 +f"{docker_compose_path}\n\n"
                  +"Give another docker-compose path on command line: \n"
                  +"\t=> [yellow]celestical deploy "
                  +"/path/to/docker-compose.yml[/yellow]")
-        cli_logger.debug("exiting as provided docker compose path is wrong")
-        raise typer.Abort()
+        cli_logger.debug("exiting as provider docker compose path is wrong")
+        sys.exit(4)
 
     # --- selecting most recent valid path
-    selected_path = get_most_recent_file(compose_path, ecompose_path)
-    prev_compose = read_docker_compose(fullpath=ecompose_path)
+    comp_time = 1.0
+    if docker_compose_path.is_file():
+        comp_time = docker_compose_path.stat().st_mtime
+
+    ecomp_time = 0.0
+    if docker_ecompose_path.is_file():
+        prev_compose = read_docker_compose(fullpath=docker_ecompose_path)
+        ecomp_time = docker_ecompose_path.stat().st_mtime
+
+    if ecomp_time > comp_time:
+        selected_path = docker_ecompose_path
+    else:
+        selected_path = docker_compose_path
 
     # --- selected process compose file
     if selected_path.is_file():
         c_dict = read_docker_compose(fullpath=selected_path)
 
         s_info = "\n* Services found in detected docker-compose file: \n"
         s_info += f"\t[green]{selected_path}[/green]\n\n"
 
         if "services" in c_dict:
             s_info += richformat_services(c_dict["services"])
 
         if "celestical" in c_dict:
-            # s_info += f"\n* [underline]App name[/underline]: " \
-            #          +f"[green]{c_dict['celestical']['name']}[/green]\n"
+            s_info += f"\n* [underline]App name[/underline]: " \
+                     +f"[green]{c_dict['celestical']['name']}[/green]\n"
             s_info += f"* [underline]App URL[/underline]: " \
                      +f"[blue]{c_dict['celestical']['base_domain']}[/blue]\n\n"
 
+
+
         cli_panel(s_info)
 
-        # - case where we are on an enriched file
         if "celestical" in c_dict:
             msg = "(Yes) To deploy now | (No) To reset info"
             answer = confirm_user(msg, default=True)
 
             if answer:
                 # Skip enrichment
                 c_dict["celestical"]["skip_enrich"] = True
-                return ecompose_path, c_dict, prev_compose
+                return docker_ecompose_path, c_dict, prev_compose
             # else will lead to enrichment (reset)
             c_dict["celestical"]["skip_enrich"] = False
-            return ecompose_path, c_dict, prev_compose
+            return docker_ecompose_path, c_dict, prev_compose
 
-        # - case where we are on an user compose file
         answer = confirm_user("Continue with this file", default=True)
         if answer:
-            return ecompose_path, c_dict, prev_compose
-
-        # - case where we exit for another file
+            return docker_ecompose_path, c_dict, prev_compose
+        # else we exit for another file
         cli_panel("Give another path on command line: \n"
                  +"\t=> celestical deploy /path/to/docker-compose.yml")
-        raise typer.Abort()
-
+        sys.exit(0)
     else:
         cli_panel("No docker-compose.yml file was found at:\n"
                  +f"{selected_path}\n\n"
                  +"Give another docker-compose path on command line: \n"
                  +"\t=> [yellow]celestical deploy /path/to/docker-compose.yml[/yellow]")
         cli_logger.debug("exiting as no docker compose file found")
-        raise typer.Abort()
+        sys.exit(2)
 
     return None, None, {}
 
 
 def upload_images(app_uuid:uuid.UUID, compose_path:Path|None=None, e_compose:dict|None=None) -> bool:
     """Upload the enriched compose file to the Celestical Cloud."""
 
-    cli_panel("Now uploading your App's images to Celestical")
+    cli_panel("Let's start uploading your App's images to Celestical")
 
     if compose_path is not None:
         e_compose = read_docker_compose(fullpath=compose_path)
     elif e_compose is None:
-        return False
-
-    # Build the compressed tar file for services images
-    image_names = [
-        e_compose["services"][service_name]["image"]
-        for service_name in e_compose["services"]
-    ]
+        return False 
 
-    image_paths = compress_image(images=image_names, project_name=e_compose["celestical"]["name"])
+    # Build the compressed tar file for each service
+    image_paths = []
+    for service_name in e_compose["services"]:
+        # typer.echo(service_name)
+        #typer.confirm("Do you wish to proceed setting the image_name?")
+        #image_name = e_compose["services"][service_name]["image"].split(':')[0]
+        image_name = e_compose["services"][service_name]["image"]
+        #typer.echo(image_name)
+        #typer.confirm("Do you wish to proceed compressing?")
+        ipath = compress_image(image_name=image_name, project_name=e_compose["celestical"]["name"])
+        image_paths.append(ipath)
 
     api_ires = None
-    apiconf = _get_api_with_auth()
-    if apiconf is None:
-        return False
-
     with api.ApiClient(apiconf) as api_client:
         app_api = api.AppApi(api_client)
+
         for ipath in image_paths:
             try:
                 with ipath.open(mode="rb") as ipath_desc:
-                    # This form won't work:
-                    # upfile = {"upload_file": (ipath.name, ipath_desc.read())}
-                    upfile = (ipath.name, ipath_desc.read())
-                    cli_logger.debug("Making image upload request")
-                    # with_http_info returns an HTTP response with status code
-                    api_ires = app_api.upload_image_compressed_file_app_app_uuid_upload_image_post_with_http_info(
+                    # upfile = {"file": ipath.name, ipath_desc, "multipart/form-data")}
+                    upfile = {"file": ipath_desc}
+                    cli_logger.debug("Making compose info push request")
+                    api_ires = app_api.upload_image_compressed_file_app_app_uuid_upload_image_post( \
                         app_uuid=app_uuid,
                         image_file=upfile)
 
-                    # Print feedback to user
-                    if api_ires is not None:
-                        msg = " uploaded" \
-                              if (api_ires.status_code == 200) \
-                              else " not uploaded"
-                        msg = str(ipath.name)+msg
-                        print_feedback(msg)
-
             except Exception as oops:
-                cli_logger.debug(f"Exception in uploading image {ipath}")
-                cli_logger.debug(type(oops))
-                print_text(f"Could not upload file {ipath.name}")
-                continue
-
-    return True
-
+                cli_logger.debug(oops)
+                pass
 
 
-def upload_compose(compose_path:str, call_nbr:int = 1) -> dict|None:
+def upload_compose(compose_path:str, call_nbr:int = 1) -> dict:
     """ This function find the compose file and ask the user for enrichment
         unless an enriched file is already present in case user is asked
         if they want to reset the enrichment.
 
         - compose_path:str: string of the folder to deploy, it should contain
           a docker compose file. It is where the enriched file will be saved
         - call_nbr:str: in case we are missing authentication we are trying to
@@ -593,28 +390,27 @@
         if "skip_enrich" in comp_dict["celestical"]:
             if comp_dict["celestical"]["skip_enrich"] is True:
                 do_enrich = False
 
     # --- Get info from user to enrich context
     enriched_compose = {}
     if do_enrich:
-        enriched_compose_path = enrich_compose(comp_dict, prev_comp, ecomp_path)
-        # we reread the compose so that we can audit what is posted
-        enriched_compose = read_docker_compose(fullpath=enriched_compose_path)
+        enriched_compose = enrich_compose(comp_dict, prev_comp, ecomp_path)
     else:
         enriched_compose = comp_dict
 
     # --- Posting the body package for Compose file
     compose_pack = {}
     compose_pack["enriched_compose"] = enriched_compose
     # optional in case we want to upload compose for later deployment
     compose_pack["deploy"] = True
 
-    apiconf = _get_api_with_auth()
-    if apiconf is None:
+    setcred, mesg = load_user_creds(apiconf)
+    if setcred is False:
+        cli_panel(msg)
         return None
 
     api_response = None
     with api.ApiClient(apiconf) as api_client:
         app_api = api.AppApi(api_client)
 
         try:
@@ -625,33 +421,31 @@
             cli_logger.debug("Making compose info push request")
             api_response = app_api.upload_compose_file_app_compose_post( \
                 compose_to_post)
 
         except UnauthorizedException as oops:
             # Let's try to relog again and relaunch that function
             if call_nbr > 1:
-                msg = "[red]Access not authorized for now[/red]\n\n"
-                msg += "Make sure a payment method is installed\n"
-                msg += f"If problem persists please contact us: {HOTLINE}"
+                msg = "Please check your connection and credentials\n"
+                msg += "[red]no access authorized for now[/red]\n\n"
+                msg += "You might need to register with: "
+                msg += "[yellow]celestical register[/yellow]\n\n"
+                msg += "If problem persists please contact us: {HOTLINE}"
                 cli_panel(msg)
                 return None
             # else
-            cli_panel("Unauthorized access, your token may have expired." \
+            cli_panel("You have to log in again, your token may have expired." \
                       +" (signing out automatically)")
-            if not user_login(force_relog=True):
-                if not user_login(force_relog=True):
-                    print_text("Please start over again checking your credentials carefully.",
-                        worry_level="ohno")
-                    return None
+            user_login(force_relog=True)
             call_nbr += 1
             cli_logger.debug(oops)
             return upload_compose(compose_path, call_nbr)
         except Exception as oops:
-            print_text("No connection yet possible to deploy your app.")
-            cli_logger.error("Error during posting of the enriched compose file")
+            cli_panel("Something undefined happened: Check your connection.")
+            cli_logger.error("Error during post of enriched compose file")
             cli_logger.error(oops)
             return None
 
     if (not isinstance(api_response, App)):
         cli_logger.error("API response is not an App.")
         msg = "Try to login again, your token might have expired.\n"
         msg += "--> [underline]celestical login[/underline]"
```

## celestical/configuration.py

```diff
@@ -1,96 +1,35 @@
-"""
-Managing the configuration for the Celestical services
-"""
+# Managing the configuration for the Celestical services
 import json
 import os
 import logging
-import importlib.metadata
-import datetime
+from logging import Logger
 from pathlib import Path
 
 import typer
 from prettytable import PrettyTable, ALL
 
 import celestical.api as api
+from celestical.helper import print_text
 
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
-API_URL = "https://moon.celestical.net"
-
-
-current_celestical_version = importlib.metadata.version('celestical')
+apiconf = api.Configuration(
+        host = "http://localhost:8000"
+)
 
 # LOGGING_LEVEL = logging.DEBUG
 # logging.basicConfig(encoding='utf-8', level=LOGGING_LEVEL)
 
 HOTLINE = "starship@celestical.net"
 PRODUCTION = False
-BATCH_MODE = False
-
-def get_batch_mode():
-    return BATCH_MODE
-
-
-def celestical_date() -> str:
-    return str(datetime.datetime.now(datetime.UTC).strftime('%Y-%m-%dT%H:%M:%S'))
-
-
-def get_login_status() -> str:
-    login_status = ""
-    # [{wcol}]colored text[/{wcol}]
-    wcol = "purple"
-
-    udata = load_config()
-    if not (udata is None or udata == {}):
-        # else message that config cannot be loaded will be shown.
-        tok = udata["access_token"]
-        uname = udata["username"]
-        if uname != "":
-            login_status += f"\n\t* Current user: [{wcol}]{uname}[/{wcol}]"
-        else:
-            login_status += f"\n\t* No current user [{wcol}]logged in[/{wcol}]"
-        if tok != "":
-            # TODO checked the created date field to announce
-            # if relogging is necessary.
-            login_status += f"\n\t* [{wcol}]Already logged in[/{wcol}] once"
-
-    return login_status
-
-
-def welcome(verbose:int=2) -> str:
-    """ Return a global welcome message
-
-        verbose from 0 (short) to 2 (long)
-    """
-    wcol = "purple"
-    welcome_message:str = f"[{wcol}]Direct deployment of containers or compose" \
-                          +" files to an independent green cloud made by space" \
-                          +f" engineers[/{wcol}] " \
-                          +f"(version: {current_celestical_version})\n"
-
-    if verbose > 0:
-        welcome_message += get_login_status()
-
 
-    if verbose > 1:
-        welcome_message += "\n [underline]Usual workflow steps[/underline]" \
-                        +"\n\t [1] (only once) Register with command " \
-                        +f"[{wcol}]celestical register[/{wcol}]" \
-                        +"\n\t [2] Login with command " \
-                        +f"[{wcol}]celestical login[/{wcol}]" \
-                        +"\n\t [3] Deploy with command " \
-                        +f"[{wcol}]celestical deploy[/{wcol}]"
 
-    return welcome_message
-
-
-# Service types definitions
 def get_default_config_dir() -> Path:
-    path = Path.home() / ".config" / "celestical"
+    path = Path.home() / ".config" / "celestical" 
     return path
 
 
 def get_default_config_path() -> Path:
     """Return the default config path for this application
 
     Returns:
@@ -106,39 +45,14 @@
     Returns:
         Path typed path to the log file
     """
     path = get_default_config_dir() / "celestical.log"
     return path
 
 
-def _get_default_config_data() -> dict:
-    data = {
-        "created": celestical_date(),
-        "username": "",
-        "access_token": "",
-        "token_type": "",
-        "batch": False
-    }
-    return data
-
-
-def reset_config():
-    """ Reset config is used to logout and start login protocol from scratch
-    """
-    # Similar to a logout: forgetting token
-    data = {
-        "created": celestical_date(),
-        "username": "",
-        "access_token": "",
-        "token_type": "",
-        "batch": False
-    }
-    return save_config(data)
-
-
 def load_config(config_path: str = "") -> dict:
     """Load config file from config_path.
 
     Params:
         config_path(str): non-default absolute path of the configuration.
     Returns:
         (dict): configuration content
@@ -149,98 +63,83 @@
 
     user_data = {}
     if path.exists():
         try:
             with open(path, 'r') as f_desc:
                 user_data = json.load(f_desc)
         except:
-            # Use only standard print function
-            print(" *** could not read the celestical configuration file.")
-            user_data = {}
-
-    default_data = _get_default_config_data()
-    for key in default_data:
-        if key not in user_data:
-            user_data[key] = default_data[key]
+            print_text("Could not read the configuration file.")
+    else:
+        print_text("The configuration file does not exist yet.")
 
     return user_data
 
 
-def save_config(config:dict) -> bool:
+def save_config(config:dict):
     """Save config file to the default_config_path.
 
     Params:
         config(dict): configuration.
     Returns:
-        (bool): True if saving process went fine
+        (str): configuration absolut path
     """
     cpath = get_default_config_path()
 
     try:
         if not cpath.parent.exists():
             os.makedirs(cpath.parent, exist_ok=True)
-    except Exception as oops:
-        cli_logger.debug("save_config: directory couldn't be created.")
-        cli_logger.debug(oops)
-        return False
+    except Exception as e:
+        typer.echo("Config directory couldn't be created successfully")
 
-    # Check if all fields are saved for uniformization
-    if "created" not in config:
-        config["created"] = celestical_date()
-    if "username" not in config:
-        config["username"] = ""
-    if "access_token" not in config:
-        config["access_token"] = ""
-    if "token_type" not in config:
-        config["token_type"] = ""
-    if "batch" not in config:
-        config["batch"] = False
-
-    try: 
-        with cpath.open(mode='w') as fdescr:
-            json.dump(config, fdescr, indent=4)
-    except Exception as oops:
-        cli_logger.debug("save_config: config file couldn't be written.")
-        cli_logger.debug(oops)
-        return False
+    with open(cpath, 'w') as f:
+        json.dump(config, f, indent=4)
 
-    return True
+    typer.echo(f"Login credentials safely updated in: {cpath}")
+    return cpath
 
 
 def cli_setup() -> bool:
     """ Setup necessary directories.
     """
     config_path = get_default_config_dir()
     try:
         config_path.mkdir(parents=True, exist_ok=True)
     except Exception as oops:
         return False
     return True
 
 
-def create_logger(production: bool=False) -> logging.Logger :
+def create_logger(production: bool=False) -> Logger :
     """A function to create and configure the logger for the Celestical CLI
     Params:
         production(bool): if False, set log level to debug
     Returns:
         (logger): the logger object
     """
     log_format = "%(asctime)s --%(levelname)s: %(message)s"
     log_location = get_default_log_path()
-
+    if production is False:
+        logging.basicConfig(
+            encoding='utf-8',
+            filename=log_location,
+            format=log_format,
+            filemode="a",
+            level=logging.DEBUG,
+        )
+        logger = logging.getLogger(name="Celestical CLI")
+        logger.warning(f"Starting Logger in DEBUG Mode: {log_location}")
+        return logger
+    
     logging.basicConfig(
         encoding='utf-8',
         filename=log_location,
         format=log_format,
         filemode="a",
-        level=logging.WARNING if production else logging.DEBUG,
+        level=logging.WARNING,
     )
     logger = logging.getLogger(name="Celestical CLI")
-    if production is False:
-        logger.debug(f"Starting Logger in DEBUG Mode: {log_location}")
-    else:
-        logger.warning(f"Starting Logger in WARNING Mode: {log_location}")
+    logger.warning(f"Starting Logger in WARNING Mode: {log_location}")
     return logger
 
 cli_setup()
 # Creation of the CLI-wide logger -> celestical.log
 cli_logger = create_logger(production=PRODUCTION)
```

## celestical/docker_local.py

```diff
@@ -1,172 +1,77 @@
 """ Handling all the local docker functionalities
 """
 import os
 from pathlib import Path
-import shutil
+import shutil 
 from typing import Tuple
 
 import docker
 import gzip
 from tqdm import tqdm
 from prettytable import PrettyTable, ALL
 import typer
 from celestical.configuration import cli_logger
-from celestical.helper import print_text, confirm_user
+from celestical.helper import print_text
 
-
-def _build_unix_socket(socket_path: Path) -> str:
-    return 'unix://' + str(socket_path.resolve())
-
-
-def _connect_docker_colima() -> docker.APIClient:
-    """ Try to establish client connection with
-    """
-    home_dir = Path.home()
-    colima_dir = home_dir / ".colima"
-    colima_default = colima_dir / "default"
-
-    if not colima_dir.is_dir():
-        return None
-
-    sock_1 = _build_unix_socket(colima_dir / "docker.sock" )
-
-    sock_2 = None
-    if colima_default.is_dir():
-        sock_2 = _build_unix_socket(colima_default / "docker.sock" )
-
-    client = None
-    try:
-        client = docker.APIClient(base_url=sock_1)
-    except Exception as oops:
-        cli_logger.error(oops)
-        client = None
-
-    if client is None and sock_2 is not None:
-        try:
-            client = docker.APIClient(base_url=sock_2)
-        except Exception as oops:
-            cli_logger.error(oops)
-            client = None
-
-    return client
+# logging.basicConfig(encoding='utf-8', level=LOGGING_LEVEL)
 
 def get_docker_client():
-    """ Returns a docker client taken from local environment """
     client = None
+    err_msg = ""
     try:
         client = docker.from_env()
-    except Exception as oops:
+    except:
         err_msg = "Could not connect to the docker service. Is it really running?"
-        cli_logger.debug(err_msg)
-        cli_logger.error(oops)
-        client = None
-
-    # alternative to finding docker 
-    if client is None:
-        try:
-            client = docker.APIClient(base_url='unix:///var/run/docker.sock')
-        except Exception as oops:
-            cli_logger.error(oops)
-            client = None
-
-    # alternative to finding docker on Mac or Linux running Colima
-    if client is None:
-        client = _connect_docker_colima()
-
-    return client
-
-
-def get_image_hash(image_name_tag:str) -> str|None:
-    """ Get the hash for a certain docker image name and tag.
-
-        Params:
-            image_name_tag(str): docker tag of the image to extract hash from
-        Returns:
+    return client, err_msg
+
+
+def get_ports(docker_client, image_id):
     """
-    client = get_docker_client()
-    if client is None:
-        # Something weird happened with Docker connection
-        return None
-    image = client.images.get(image_name_tag)
-    if image is None:
-        return None
-    return image.id
-
-
-def get_ports(image_id:str,
-              docker_client:any=None,
-              proto:str="tcp") -> str:
-    """ Get ports from containers created from the specified image.
-        else get the ExposedPorts info from the image itself.
-
-        Params:
-            image_id(str): should the string hash of the image
-            docker_clienti(any): a docker client
-            proto(str): ports for a that specific protocol, by default 'tcp'
+        Get ports from containers created from the specified image.
 
-        Returns:
-            a string for a joint list of ports
+        returns a string for a joint list of ports
     """
     if docker_client is None:
-        docker_client = get_docker_client()
-        if docker_client is None:
-            return ""
-        # else continue
+        return ""
 
     ports = set()
-
-    # Checking from containers
     for container in docker_client.containers.list(all=True):
         if container.image.id == image_id:
             port_data = container.attrs['HostConfig']['PortBindings']
             if port_data:
                 for port, bindings in port_data.items():
                     # get only the port number, not the protocol
-                    ports.add(str(port.split('/')[0]))
-
-    # Checking from listed images
-    if len(ports) == 0:
-        try:
-            img = docker_client.images.get(image_id)
-            for tcpport in [str(attr).split("/")[0]
-                            for attr in
-                            img.attrs["Config"]["ExposedPorts"]
-                            if "tcp" in attr]:
-                ports.add(tcpport)
-        except Exception as oops:
-            # The image_id is not found
-            # The ports set remains empty and that's all ok.
-            cli_logger.debug(oops)
+                    ports.add(port.split('/')[0])
+    return ', '.join(sorted(ports)) 
 
-    return ",".join(sorted(ports))
 
-
-def list_local_images() -> PrettyTable:
+def list_local_images() -> Tuple[PrettyTable, str]:
     """List all docker images locally available with port information.
 
     Returns:
         PrettyTable of formatted table of docker images
+        and an error message
     """
-    docker_client = get_docker_client()
+    docker_client, err_msg = get_docker_client()
     if docker_client == None:
-        return None
+        return None, err_msg
 
     table = PrettyTable()
     table.field_names = ["Image ID", "Image Name", "Tags", "Ports"]
     table.hrules = ALL  # Add horizontal rules between rows
 
     images = []
     terminal_width = 100
     try:
         terminal_width, _ = shutil.get_terminal_size()
         images = docker_client.images.list()
     except Exception as whathappened:
-        cli_logger.error(whathappened)
-        return table
+        # logging.error(whathappened)
+        return table, err_msg
 
     # Adjust column widths based on the terminal width
     # divide by 2 for two lines
     id_width = max(len(image.id) for image in images) // 2 + 1
     name_width = max(len(image.tags[0].split(':')[0])
                      if image.tags
                      else 0 for image in images)
@@ -186,119 +91,83 @@
     for image in images:
         # Split the Image ID into two lines
         half_length = len(image.id) # // 2
         formatted_id = f'{image.id[:half_length]}\n{image.id[half_length:]}'
         # Extract image name from the tags
         image_name = image.tags[0].split(':')[0] if image.tags else 'N/A'
         # Get ports
-        ports = get_ports(image.id, docker_client)
+        ports = get_ports(docker_client, image.id)
         table.add_row([formatted_id, image_name, ', '.join(image.tags), ports])
 
-    return table
+    return table, err_msg
 
 
-def compress_image(images: str|list[str], project_name: str) -> list[Path]:
+def compress_image(image_name: str, project_name: str) -> Path:
     """Compress a Docker image.
-
-    Params:
-        images: string or list of strings of image full tag names
-                as they should appear in the "image" field of each service
-        project_name: a string given to name the project, usually the base
-                domain name
-    Returns:
-        A list of path to gzipped images to be uploaded
     """
 
-    image_names = []
-    gz_paths = []
-
-    # --- Getting docker client
-    client = get_docker_client()
-    if client is None:
-        return gz_paths
+    client = docker.from_env()
 
-    # --- preparing save directory
     save_path = Path(f"/tmp/celestical/{project_name}/")
     # Create the save_path directory and any necessary parent directories
     save_path.mkdir(parents=True, exist_ok=True)
 
-    # --- preparing list of images, or of 1 image
-    if isinstance(images, str):
-        image_names = [images]
-    else:
-        image_names = images
-
-    # --- Compressing all images in different gzips
-    for image_name in image_names:
-        tar_filename = save_path / f'{image_name}.tar'
-        gz_filename = save_path / f'{image_name}.tar.gz'
-
-        # Step 1: Calculate the total size of the image
-        # for chunk in client.images.get(image).save(named=True):
-        #     tar_file.write(chunk)
-        print_text(f"Working on {image_name}...")
-        img = None
-        try:
-            img = client.images.get(image_name)
-        except Exception as oops:
-            cli_logger.debug(oops)
-            img = None
-
-        if img is None:
-            msg = f"Image {image_name} not found for project: {project_name}"
-            print_text(msg,
-                       worry_level="ohno")
-            cli_logger.debug(msg)
-            continue
-
-        image_data = img.save(named=True)
-        total_size = sum(len(chunk) for chunk in image_data)
-        total_size_mb = total_size / (1024 * 1024)
-
-        # Reset the image data iterator
-        image_data = img.save(named=True)
-
-        print_text(f"Image Tag Found: {image_name}"
-                   +f"\n\timage size: {total_size_mb:.2f} MB"
-                   +f"\n\tsaving in: {save_path}"
-                   +f"\n\tas file name: {gz_filename}")
-
-        # Prompt user for confirmation before proceeding with compression
-        if gz_filename.is_file():
-            if not confirm_user(f"[yellow]{image_name}[/yellow] already prepared,"
-                               +f"\n\trenew and overwrite {gz_filename} ?"):
-                print_text(f" * Ok, using ready file: {gz_filename}\n")
-                gz_paths.append(gz_filename)
-                continue
-
-        # Save the Docker image to a tar file with a progress bar
-        print_text(f"Export image to archive tar file {tar_filename} ...")
-        with open(tar_filename, 'wb') as tar_file:
-            with tqdm(total=total_size,
-                      unit='B',
-                      unit_scale=True,
-                      desc="archiving") as pbar:
-                for chunk in image_data:
-                    tar_file.write(chunk)
-                    pbar.update(len(chunk))
+    tar_filename = save_path / f'{image_name}.tar'
+    gz_filename = save_path / f'{image_name}.tar.gz'
 
 
-        # Step 2: Compress the tar file using gzip
-        print_text(f"Compressing exported tar image (gzip) to {gz_filename} ...")
-        file_size = os.path.getsize(tar_filename)
-        with open(tar_filename, 'rb') as tar_file:
-            with gzip.open(gz_filename, 'wb') as gz_file:
-                with tqdm(total=file_size,
-                          unit='B',
-                          unit_scale=True,
-                          desc="gzipping") as pbar:
-                    # Define a chunk size (e.g., 1 MiB)
-                    chunk_size = 1024 * 1024
-                    # Read, compress, and write data in chunks
-                    while chunk := tar_file.read(chunk_size):
-                        gz_file.write(chunk)
-                        pbar.update(len(chunk))
+    # Step 1: Save the Docker image to a tar file
+    # image = f'{image_name}:{tag}'
+    # tar_filename = f'{image_name}_{tag}.tar'
+    # with open(tar_filename, 'wb') as tar_file:
+    #     for chunk in client.images.get(image).save(named=True):
+    #         tar_file.write(chunk)
+
+    print_text("Calculating total image size ..")
+
+    # Step 1: Calculate the total size of the image
+    image_data = client.images.get(image_name).save(named=True)
+    total_size = sum(len(chunk) for chunk in image_data)
+    total_size_mb = total_size / (1024 * 1024)
+
+
+    # Reset the image data iterator
+    image_data = client.images.get(image_name).save(named=True)
+
+    print_text("\n============================================\n")
+    print_text(f"Image Name:Tag: {image_name} \t Image Size: {total_size_mb:.2f} MB")
+    print_text(f"Saving in: {save_path} \t File Name: {gz_filename}")
+    # print_text(f"App context: {context} \t Domain: {domain}")
+    print_text("\n============================================\n")
+
+    # Prompt user for confirmation before proceeding with compression
+    if not typer.confirm("Would you like to proceed with saving and compressing the image?"):
+        print_text("Aborting the program.")
+        raise typer.Abort()
+
+    print_text("Starting to save the image .. ")
+    # Save the Docker image to a tar file with a progress bar
+    with open(tar_filename, 'wb') as tar_file:
+        with tqdm(total=total_size, unit='B', unit_scale=True, desc='Saving') as pbar:
+            for chunk in image_data:
+                tar_file.write(chunk)
+                pbar.update(len(chunk))
+
+    print_text("Compressing exported tar image (gzip)...")
+
+    # Step 2: Compress the tar file using gzip
+    file_size = os.path.getsize(tar_filename)
+    with open(tar_filename, 'rb') as tar_file:
+        with gzip.open(gz_filename, 'wb') as gz_file:
+            with tqdm(total=file_size, unit='B', unit_scale=True, desc='Compressing') as pbar:
+                # Define a chunk size (e.g., 1 MiB)
+                chunk_size = 1024 * 1024
+                # Read, compress, and write data in chunks
+                while chunk := tar_file.read(chunk_size):
+                    gz_file.write(chunk)
+                    pbar.update(len(chunk))
 
-        gz_paths.append(gz_filename)
-        print_text(f"[green]succesfully prepared[/green]: {gz_filename}")
+    print_text("\n============================================\n")
+    print_text(f"Image {image_name} compressed successfully in {save_path}!")
+    print_text("\n============================================\n")
 
-    return gz_paths
+    return gz_filename
```

## celestical/helper.py

```diff
@@ -1,31 +1,34 @@
 """Helper functions for the celestical app"""
-import string
+import os
 import json
-import yaml
 from pathlib import Path
-import typer
 
+import typer
+import yaml
 
 from prettytable import PrettyTable, ALL
 from rich.console import Console
 from rich.panel import Panel
 from rich.table import Table
 from rich.prompt import Prompt, Confirm
-from celestical.configuration import get_batch_mode
 
 console = Console()
 
+welcome_message:str = "[purple]Direct deployment of containers or compose" \
+                      +"files to a green cloud made by space engineers[/purple]"
 
+# Service types definitions
+#
 # For each service type there is a list of keywords to detect them
 SERVICE_TYPES = {
     "FRONTEND": ["web", "www", "frontend", "traefik", "haproxy", "apache", "nginx"],
     "API": ["api", "backend", "service", "node"],
     "DB": ["database", "redis", "mongo", "mariadb", "postgre"],
-    "BATCH": ["process", "hidden", "compute"],
+    "BATCH": ["hidden", "compute"],
     "OTHER": []
 }
 
 
 # Building a table in the terminal
 def create_empty_table(columns_labels):
     """Create an empty table with specified columns."""
@@ -57,25 +60,22 @@
 
     for key, value in data.items():
         table.add_row(str(key), str(value))
 
     return table
 
 
-def cli_panel(message: str, _type="info", _title:str="Celestical Message", batch:bool=get_batch_mode()) -> None:
+def cli_panel(message: str, _type="info", _title:str="Celestical Message") -> None:
     """Display a message in a panel.
     Params:
         message(str): message to be displayed
     Returns:
         None
     """
 
-    if batch:
-        return
-
     # Note: here is hwo to join *args
     # buffer = "\n".join(str(arg) for arg in args)
 
     if _type == "info":
         title = _title
         panel = Panel(message, title=f"[bold purple]{title}[/bold purple]",
                     border_style="purple",
@@ -88,159 +88,128 @@
             expand=True,
             title_align='left')
 
 
     console.print(panel)
 
 
-def save_json(data: dict, batch:bool=get_batch_mode()) -> bool:
+def save_json(data: dict) -> bool:
     """Helper function to save the complete stack info.
     Params:
         data(dict): complete info about the stack (name, compose ..)
     Returns:
 
     """
     if "name" not in data:
         return False
 
     json_file = f'stack_{data["name"]}.json'
     try:
         with open(json_file, 'w') as jfile:
             json.dump(data, jfile, indent=4)
-    except Exception as oops:
-        if not batch:
-            print_text(f"Error: JSON file could not be saved f'stack_{data['name']}.json'")
-        cli_logger.debug(oops)
-        return False
+        print_text("Json saved successfully.")
+        return True
+    except Exception as e:
+        print(f"Error: Unable to save data to f'stack_{data['name']}.json'")
+        print(f'Error details: {e}')
 
-    return True
+    return False
 
 
-def save_yaml(data: dict, yml_file:Path = None, batch:bool=get_batch_mode()) -> Path|None:
+def save_yaml(data: dict, yml_file:Path = None):
     """Helper function to save the complete stack info.
     Params:
-        data(dict): complete info about the stack (name, compose ..)
-        yml_file(Path):  Path where to save the file
+        stack_info(dict): complete info about the stack (name, compose ..)
     Returns:
 
     """
     #yml_file = "docker-compose.yml"
     if yml_file is None:
-        yml_file = Path("./.docker-compose-enriched.yml")
+        yml_file = Path("./docker-compose-enriched.yml")
 
     try:
         with yml_file.open(mode='w') as yfile:
             yaml.dump(data, yfile, default_flow_style=False)
-        if not batch:
-            print_text(f"YAML file created successfully: [green]{yml_file}[/green]")
+        print_text(f"YAML file created successfully: [green]{yml_file}[/green]")
 
-    except Exception as eoops:
-        msg = f'Error: Unable to save data to {yml_file}'
-        cli_logger.error(msg)
-        cli_logger.error(eoops)
-        return None
+    except Exception as e:
+        print(f'Error: Unable to save data to {yml_file}')
+        print(f'Error details: {e}')
 
     # return the Path object of the saved file
     return Path(yml_file)
 
 
-def print_nested_dict(dictionary: dict, batch:bool=get_batch_mode()):
+def print_nested_dict(dictionary: dict):
     """Print a nested dictionary in a readable format."""
-    if batch:
-        return
     for key, value in dictionary.items():
         if isinstance(value, dict):
             print_nested_dict(value)
         else:
             print(f"{key}: {value}")
 
 
-def print_feedback(used_input:str, batch:bool=get_batch_mode()):
+def print_feedback(used_input: str):
     """ Show users what they have input """
-    if batch:
-        return
     console.print(f" :heavy_check_mark: - {used_input}")
 
 
-def print_help(help_text: str, batch:bool=get_batch_mode()):
+def print_help(help_text: str):
     """ Show users a help text """
-    if batch:
-        return
     console.print(" [dodger_blue3]<:information:>[/dodger_blue3] "
                 +f"[gray30]{help_text}[/gray30]")
 
 
-def prompt_user(prompt: str,
-                default:str=None,
-                helptxt:str="",
-                batch:bool=get_batch_mode()) -> str:
+def prompt_user(prompt: str, default:str=None, helptxt:str="") -> str:
     """Prompt the user for input.
     Params:
         prompt(str): the prompt text invitation
     Returns:
         str: the user input
 
     """
-    if batch:
-        return default
-
     more_help = ""
     if helptxt != "":
         if len(helptxt) <= 20:
             more_help = f" [gray30]({helptxt})[/gray30]"
         else:
             more_help = " [gray30](type ? for more help)[/gray30]"
     resp = Prompt.ask(f"\n [green_yellow]===[/green_yellow] {prompt}{more_help}", default=default)
 
     if resp is None:
         resp = ""
 
     if resp == "?":
         print_help(helptxt)
         return prompt_user(prompt, default, helptxt)
-
+        
     return resp
 
 
-def confirm_user(prompt: str, default:bool = True, batch:bool=get_batch_mode()) -> str:
+def confirm_user(prompt: str, default:bool = True) -> str:
     """Prompt the user for yes no answer.
     Params:
         prompt(str): the prompt text invitation
     Returns:
         bool: the user confirmation
     """
-    if batch:
-        return default
-
     confirmation:bool = Confirm.ask(f"\n === {prompt} ", default=default)
     if confirmation is None:
         confirmation = False
     return confirmation
 
 
-def print_text(text: str, worry_level="chill", batch:bool=get_batch_mode()):
+def print_text(text: str):
     """Print text to the CLI.
         Params:
             text(str): the text to print
-            worry_level(str): a level of worries that would change the color; chill, oops, ohno
         Returns:
             str: the text to print
     """
-    if batch:
-        return
-
-    msg = f"{text}"
-    if worry_level == "oops":
-        msg = f"[orange]{text}[/orange]"
-    elif worry_level == "ohno":
-        msg = f"[red]{text}[/red]"
-
-    # add prefix
-    msg = " --- " + msg
-
+    msg = f"\n --- {text}"
     return console.print(msg)
 
 
 def guess_service_type_by_name(service_name: str, img_name:str=""):
     """ Quick guess of service type
     """
 
@@ -260,100 +229,7 @@
             for guesser in SERVICE_TYPES[stype]:
                 if guesser in img_name:
                     return stype
 
     # if nothing found
     return "OTHER"
 
-
-def get_most_recent_file(file1:Path,
-                         file2:Path) -> Path:
-    """ Will compare modification time between file1 and file2
-        and return most recent one.
-        If no file exist
-
-    Params:
-        - file1(str): file Path
-        - file2(str): file Path
-    """
-    # --- cover cases if one or both are null
-    if file1 is None:
-        if file2 is None:
-            return None
-        else:
-            return file2
-    elif file2 is None:
-        return file1
-        # else keep going
-
-    # --- select last modified or file1
-    selected_path = file1
-    ftime1 = 1.0
-    if file1.is_file():
-        ftime1 = file1.stat().st_mtime
-
-    ftime2 = 0.0
-    if file2.is_file():
-        ftime2 = file2.stat().st_mtime
-
-    if ftime2 > ftime1:
-        selected_path = file2
-
-    return selected_path
-
-
-def dict_to_list_env(d_in:dict) -> list:
-    env_list = []
-    for key in d_in:
-        env_list.append(key+"="+str(d_in[key]))
-    return env_list
-
-
-def extract_all_dollars(str_in:str) -> dict:
-    """ Extract all dollar variables names from the string
-
-    Returns:
-        A dictionary that has  pure variable names as keys
-        as they would be found defined in an shell env or .env file
-        and they representation in strings as $variables or ${variables}.
-
-    """
-    # - split the strings and manage where to start
-    splits = str_in.strip() # we dont need whitespaces
-
-    if len(splits) <= 1:
-        # we need at least 2 characters to work out at least one $variable
-        return {}
-
-    s_idx = 1
-    if splits[0] == '$':
-        # use first split, so start at index 0
-        s_idx = 0
-
-    splits = str_in.split("$")
-    if len(splits) <= 1:
-        return {}
-
-    used_vars = {}
-    accepted_chars = string.ascii_letters + string.digits + "_"
-    # - each split start with a variable or '{'
-    for spp in splits[s_idx:]:
-        var = ""
-        if len(spp) > 1:
-            if spp[0] == '{':
-                # get all up to next first '}'
-                idx = spp.find('}')
-                if idx > 1:
-                    var = spp[1:idx]
-                    used_vars[var] = "${"+var+"}"
-                # else not adding the var.
-            else:
-                for char in spp:
-                    if char in accepted_chars:
-                        var += char
-                    else:
-                        # stop at first unaccepted char
-                        break
-                if len(var) >= 1:
-                    used_vars[var] = "$"+var
-
-    return used_vars
```

## celestical/user.py

```diff
@@ -1,200 +1,168 @@
 """ user related functions
 
     This file holds the routines to login, register
     and manage user data and configuration.
 """
 import getpass
+from datetime import datetime
 from typing import Tuple
 
-from celestical import api
 from celestical.api import (
     ApiClient,
     AuthApi,
     ApiException,
-    Code,
     UserCreate)
 from celestical.configuration import (
-    API_URL,
+    apiconf,
     load_config,
     save_config,
-    reset_config,
-    celestical_date,
     cli_logger)
 from celestical.helper import (
     cli_panel,
-    print_text,
     prompt_user,
     confirm_user)
 
 
-def register_form(ask:str = "Register with or without a [b]special code[/b]",
-    default_code:str = ""
-    ) -> str:
-    if ask != "":
-        print_text(ask)
-    user_code = prompt_user("[b]special code[/b] (optional)", default=default_code)
-    return user_code
-
-
-def login_form(ask:str = "Please enter your [i]celestical[/i] credentials",
-               default_email:str = None
-              ) -> Tuple[str, str]:
-    """ The username/password form to login and register """
-
-    if ask != "":
-        print_text(ask)
-
-    # -------------- username
-    user_mail = prompt_user("work email", default=default_email)
+def login_form(ask:str = "Please enter your wonderful Celestical credentials",
+    default_email:str = None
+    ) -> Tuple[str, str]:
+    cli_panel(ask)
+    user_mail = prompt_user("User Mail", default=default_email)
     if "@" not in user_mail:
         cli_logger.error("Entered email address is missing a '@'")
         cli_panel(message="Email is incorrect: no @ sign found.", _type="error")
         return login_form(ask)
 
-    # -------------- password
-    password = getpass.getpass(" *** password: ")
+    password = getpass.getpass(" *** Password: ")
     cli_logger.info("Password succesfully created.")
 
-    if len(password) == 0:
-        cli_logger.error("Password was empty")
-        cli_panel(message="Password was empty!", _type="error")
-        return login_form(ask="Please re-enter your [i]celestical[/i] credentials")
-
     if len(password) <= 7:
-        cli_logger.error("Password is too short - less than 8 chars")
-        cli_panel(message="Password too short - less than 8 chars!", _type="error")
-        return login_form(ask="Please re-enter your [i]celestical[/i] credentials")
-
+        cli_logger.error("Password is too short!")
+        cli_panel(message="Password too short!", _type="error")
+        return login_form(ask)
     return (user_mail, password)
 
 
 def user_login(default_email:str = None,
                force_relog:bool = False,
                ) -> bool:
     """Login to Parametry's Celestical Cloud Services via the CLI.
 
     Returns:
         bool
     """
     cli_logger.info("Entering user login function in user.py")
-    user_data = load_config()
-    if default_email is not None:
-        user_data['username'] = default_email
-
-    prask = ""
+    user_data = {}
+    if default_email is None:
+        user_data = load_config()
+
+    use_user = False
+    if "access_token" in user_data:
+        if len(user_data["access_token"]) > 10:
+            if "username" not in user_data:
+                cli_logger.warning("Oh no it seems config was manually edited.")
+            elif force_relog == False:
+                cli_panel(f"You are logged in as {user_data['username']}")
+                use_user = confirm_user("Do you want to continue" \
+                    + f" with user [yellow]{user_data['username']}[/yellow]")
+                if use_user:
+                    cli_panel("\t --> continuing as " \
+                        +f"[yellow]{user_data['username']}[/yellow]")
+                    return True
 
-    if force_relog:
-        if not reset_config():
-            return False
+        if force_relog:
+            # Similar to a logout: forgetting token
+            data = {
+                "created": datetime.utcnow().strftime('%Y-%m-%d_%H:%M:%S'),
+                "username": "",
+                "access_token": "",
+                "token_type": ""
+            }
+            save_config(data)
 
-        # user_data was loaded before the reset
-        if "username" in user_data:
-            if user_data['username'] is None or user_data['username'] == "":
-                return user_login(default_email=None)
-            # else we've got a previous email info
-            return user_login(default_email=user_data['username'])
-        return user_login()
-    elif len(user_data["access_token"]) > 10 and  len(user_data["username"]) > 3:
-        use_user = confirm_user("Do you want to continue with logged " \
-            + f"in user: [yellow]{user_data['username']}[/yellow]")
-        if use_user:
-            default_email = user_data["username"]
-            prask = f"Ok login again with [i]{default_email}[/i]" 
-
-    if prask != "":
-        (username, password) = login_form(ask=prask, default_email=default_email)
-    else:
-        (username, password) = login_form(default_email=default_email)
+            if "username" in user_data:
+                if user_data['username'] is None or user_data['username'] == "":
+                    return user_login(default_email=None)
+                # else we've got a previous email info
+                return user_login(default_email=user_data['username'])
+            return user_login()
 
-    apiconf = api.Configuration(host=API_URL)
     with ApiClient(apiconf) as api_client:
         # Create an instance of the API class
         api_instance = AuthApi(api_client)
 
-        save_ok = False
+        (username, password) = login_form(default_email=default_email)
+
         try:
             # Auth:Jwt.Login
             api_response = api_instance.auth_jwt_login_auth_jwt_login_post(username, password)
-            cli_logger.debug("We did get a login api response")
+            cli_logger.debug("we did get a api response")
             if api_response.token_type != "bearer":
                 cli_logger.debug("This client does not handle non bearer type token")
                 return False
 
             if len(api_response.access_token) < 10:
                 cli_logger.debug("Received token seems invalid")
                 return False
 
             # Collect all user data and save it
             cli_logger.debug("Creating and saving user data/conf.")
             data = {
-                "created": celestical_date(),
+                "created": datetime.utcnow().strftime('%Y-%m-%d_%H:%M:%S'),
                 "username": username,
                 "access_token": api_response.access_token,
                 "token_type": api_response.token_type
             }
-            save_ok = save_config(data)
+            save_config(data)
         except ApiException as api_exp:
-            cli_logger.error("Code Enceladus: ApiException when logging in. Assuming wrong user,password tuple.")
+            cli_logger.error("Code Enceladus: ApiException when logging in.")
             cli_logger.debug(api_exp)
-            print_text("Sorry user/password are not matching. Not logged in",
-                       worry_level="ohno")
+            cli_panel("Sorry we could not log you in at the moment")
             return False
         except Exception as oops:
             cli_logger.error("Code Mars: could not connect, try again after checking your connection.")
             cli_logger.debug(oops)
-            print_text("Sorry we could not log you in, please try again.",
-                       worry_level="ohno")
             return False
 
-    cli_panel("\t --> You are now logged in as user: "
-              +f"[yellow]{username}[/yellow]"
-              +"\n\n\t     You use other celestical commands"
-              +"\n\t     as long as your login token is valid.")
     return True
 
 
 def user_register() -> bool:
     """Register as a user for Parametry Cloud Services via the CLI."""
 
-    user_code = register_form()
-
-    (user_mail, password) = login_form("")
-
-    apiconf = api.Configuration(host=API_URL)
     with ApiClient(apiconf) as api_client:
         auth = AuthApi(api_client=api_client)
 
+        (user_mail, password) = login_form("Please enter new Celestical credentials")
+
         apires = None
         try:
             apires = auth.register_register_auth_register_post(
                     user_create=UserCreate(
-                        email=user_mail,
-                        password=password,
-                        code=Code(user_code)
+                        email= user_mail,
+                        password=password
                         )
                     )
         except ApiException as api_err:
             msg = f"---- Registration error ({api_err.status})"
             cli_logger.error(msg)
             cli_logger.debug(apires)
             if api_err.body:
                 cli_logger.debug(api_err.body)
             else:
                 cli_logger.debug(api_err.reason)
             return False
-        except Exception as oops:
-            cli_logger.error(oops)
-            return False
 
+        cli_panel("You are now registered and must verify your email")
         return True
 
 
 def load_user_creds(_apiconf) -> Tuple[bool, str]:
-    """ Reads user creds from config and set access token
+    """ Reads user creds from config and set access token 
 
         _apiconf from api.Configuration()
         is set with latest access token.
     """
     user_data = load_config()
 
     if user_data is not None and isinstance(user_data, dict):
@@ -204,11 +172,11 @@
         _apiconf.api_key_prefix['Authorization'] = \
           user_data.get("token_type", "bearer")
         # cover the case of an http+bearer type security
         # (this is current default on celestical's API side
         _apiconf.access_token = user_data.get("access_token", "")
         return True, "Loaded creds for API request"
 
-    msg = "[red] You need to login or relogin before proceeding[/red]\n"
-    msg += ">>> [underline]celestical login[/underline]"
+    msg = "[red]Could not upload you deployment config you need to login first[/red]\n"
+    msg += "--> [underline]celestical login[/underline]"
     return False, msg
```

## Comparing `celestical/api/models/code.py` & `celestical/api/models/first_creator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     CELESTICAL API
 
      CELESTICAL API gives control over your serverless web services. 
 
-    The version of the OpenAPI document: 0.16.3
+    The version of the OpenAPI document: 0.5.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
@@ -24,30 +24,30 @@
 from typing_extensions import Literal
 from pydantic import StrictStr, Field
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-CODE_ANY_OF_SCHEMAS = ["object"]
+FIRSTCREATOR_ANY_OF_SCHEMAS = ["object"]
 
-class Code(BaseModel):
+class FirstCreator(BaseModel):
     """
-    Code
+    FirstCreator
     """
 
     # data type: object
     anyof_schema_1_validator: Optional[Any] = None
     # data type: object
     anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
         actual_instance: Optional[Union[object]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Literal[CODE_ANY_OF_SCHEMAS]
+    any_of_schemas: List[str] = Literal[FIRSTCREATOR_ANY_OF_SCHEMAS]
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -58,15 +58,15 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = Code.model_construct()
+        instance = FirstCreator.model_construct()
         error_messages = []
         # validate data type: object
         try:
             instance.anyof_schema_1_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
@@ -74,15 +74,15 @@
         try:
             instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in Code with anyOf schemas: object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in FirstCreator with anyOf schemas: object. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: dict) -> Self:
         return cls.from_json(json.dumps(obj))
 
@@ -108,15 +108,15 @@
             instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into Code with anyOf schemas: object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into FirstCreator with anyOf schemas: object. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
```

## Comparing `celestical-0.18.5.dist-info/COPYING` & `celestical-0.9.2.dist-info/COPYING`

 * *Files identical despite different names*

## Comparing `celestical-0.18.5.dist-info/COPYING.LESSER` & `celestical-0.9.2.dist-info/COPYING.LESSER`

 * *Files identical despite different names*

## Comparing `celestical-0.18.5.dist-info/RECORD` & `celestical-0.9.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 COPYING,sha256=5X8cMguM-HmKfS_4Om-eBqM6A1hfbgZf6pfx2G24QFI,35150
 COPYING.LESSER,sha256=GkWx0KhgPf4s_GRPnauXCxdi-Sur4qrG6y9dRXLEpoA,7653
 LICENSE,sha256=l4pgftTXn9aA9oyWYwUdY8St5XfN8v5bCjhSUZhNmfo,108
 celestical/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-celestical/api/__init__.py,sha256=lOTq8g_uOUImrCIv7GClr9EGw-NBQVpqOZPOkIs7i5g,2647
+celestical/api/__init__.py,sha256=hiZKsKSLCshfs_KFaMciEPOkZ-jZrBcZprs_sxo6Y60,2650
 celestical/api/api/__init__.py,sha256=IdA2DY2zidKnvzu-ZsR19fS-l0tkZ3Nw0OCWxMYoq1E,246
-celestical/api/api/app_api.py,sha256=itMv7WJ4Tv4OH6H4GWB3AuUWruZagnSGn2JM0UA88jw,51131
-celestical/api/api/auth_api.py,sha256=BEVxhLz6xxOxbPYJG0ITjOl_6zWfX24hNs6Eq4v0AiI,79145
-celestical/api/api/default_api.py,sha256=n4-OzEUKvgpu6lcsnegCvd4cgsp7YhwjLfpvwWppdDY,9886
-celestical/api/api/users_api.py,sha256=1xkEIqj5YimzLK4jQ6dDwucDL619xbQJy3Uaqmso9GU,51169
-celestical/api/api_client.py,sha256=SvBQw9xU_gSXv9Xj8x4Q2cMCOiBug7wTrGIOCdzwtxE,24570
+celestical/api/api/app_api.py,sha256=ZX6XXaM-fgo0gyICD9Z49m6W8Ikh29lQ0J5OPQTR-ec,51215
+celestical/api/api/auth_api.py,sha256=pwgr8PW1jpX9IrR9dN_gM7DqTit2BCEx1gSQqBZUHIA,79144
+celestical/api/api/default_api.py,sha256=SAMCrG6WYSawFkrePeKBqAZW9pt4IcA0xYgYxwCp9K4,9885
+celestical/api/api/stacy_api.py,sha256=eiQLPA7IhHBEGW9mtWx6fbxEMjSeUxnym9vyWFenR1A,10780
+celestical/api/api/users_api.py,sha256=RjS4Jd52f6T6TQgCGBjcSHcydr3m0Qq4pVvape8HtKg,51168
+celestical/api/api_client.py,sha256=H6fIscBiFiNaPUHDGPqUOFD5cdnU3GkQKeJOFYx8Frg,24568
 celestical/api/api_response.py,sha256=A7O_XgliD6y7jEv82fgIaxR3T8KiwaOqHR6djpZyh_o,674
-celestical/api/configuration.py,sha256=tcnbjsRQnX2aarLtiPbg6Vnl-lIY24HEIOSB6zAiHis,14610
-celestical/api/exceptions.py,sha256=p05CW3fA4WJB-2LJf8qLTw5yGw3Lkx5FKtOHl0FNR08,5940
-celestical/api/models/__init__.py,sha256=1MumE5tYtX_TCvhis9eC4Hllv9XLNlZpymf_5D2IVWU,1905
-celestical/api/models/app.py,sha256=HNVSoddoeyldcm0lbcgB1NCNE6CublDZSG_vVlxNRac,3731
-celestical/api/models/bearer_response.py,sha256=E2vbRsTfrs549k3k3hwc-VW_0B3KczhHTE1nIPbvxxg,2939
-celestical/api/models/body_reset_forgot_password_auth_forgot_password_post.py,sha256=aqxWLL2liupkUk-vZEZcmvjmczmrb3Zq_xBmNpwT8SY,2691
-celestical/api/models/body_reset_reset_password_auth_reset_password_post.py,sha256=COCymDeMlpMMaSsTBRib9u1tycgFFyokOP72Y3LtJdA,2983
-celestical/api/models/body_verify_request_token_auth_request_verify_token_post.py,sha256=_GxVbNi-SvuwyUGf-KQMgwyW2B0HIUoUUBK7MGIEaCw,2703
-celestical/api/models/body_verify_verify_auth_verify_post.py,sha256=GX8zo2VCHmcbSVOpMDjalowv0c_6330r3DVyLemIbS0,2631
-celestical/api/models/client_id.py,sha256=6wNPw6cvYTU_XFG1hhmFHz6Je-CMK9GIFUbFPJovlYs,4815
-celestical/api/models/client_secret.py,sha256=0Ye7JMzH69SWnAuYKEqnlkU9FvqAtRSExydbG1l_mlM,4843
-celestical/api/models/code.py,sha256=HLYZMJgzkship3uGb3npx7Gn1Veenb3ei9njZ8vmV_U,4787
-celestical/api/models/compose.py,sha256=HyQbHAAvz4W8pfXIsL8ZHtXbBniIP5KIDox2kUwQqTk,2975
-celestical/api/models/deploy.py,sha256=UPyvyZ5Oh8oo4oEKQKsxgpn3OMNYqksCg7q_Lrq7kmk,4801
-celestical/api/models/detail.py,sha256=HGCP71CjaVAMFD0ud---y6WutMVfK-67y0K613TMWJU,4912
-celestical/api/models/error_model.py,sha256=Iw6JnlDzp2pMLnpJiDyhEu9Ig6KRrB6Ih8IPtMGqHBw,2605
-celestical/api/models/grant_type.py,sha256=vK92ViqFfqNlgtBioSWKI5lYEZ2hAb1avPMb1CKZzcA,4822
-celestical/api/models/http_validation_error.py,sha256=3C9IYCBtrfvo5HpJyhexWe-Ebv5n-DOqwQXWS9OQ1sA,2602
-celestical/api/models/is_active.py,sha256=pUYHZGgvmEytZGUwn-xRuyKJPxRP7JXv4xQNnhtOB1I,4815
-celestical/api/models/is_superuser.py,sha256=HpGmgCkw9gpvsoAiV2AX9lGlXLN8jheCi3dwSleuowY,4836
-celestical/api/models/is_verified.py,sha256=KRn1zw5-zxa4aZ2g7vwvS0oEahvPj5YlW1JfMpMsJJ0,4829
-celestical/api/models/missing_images.py,sha256=qA5CrdNtYPq3uyaEg_slqNRYYuyLA9F4DlacBUCtAv0,2639
-celestical/api/models/name.py,sha256=8NLt0OxB6lpLtfrENLw6vE0604UjdC9tOhpelsdWfis,4787
-celestical/api/models/uploaded_image.py,sha256=acgb7dbEy0tQVEys7skVtkiQLScubQEXwgS1yAFkftg,2920
-celestical/api/models/user_create.py,sha256=luOSCzYT8t6dyGU6aN5tzpavPsRQp5JsIsIbiiSr03s,4757
-celestical/api/models/user_read.py,sha256=T5UAW8TXUJxziINILK3-p0ZeXpTj18ojQowsyUlBjoY,4111
-celestical/api/models/validation_error.py,sha256=GuE0fstDa6LMwqogA55-T9YgjB94fvE-0QwQAvzyeYs,3083
+celestical/api/configuration.py,sha256=iNAihwpPKK7ziPI0pS7w9g8rASM1biNVbJ64IrGEk_w,14608
+celestical/api/exceptions.py,sha256=fT4ddGM3PkDKY-s_ARQg-U3HWUlm2Rj8zf_X53lXY2I,5939
+celestical/api/models/__init__.py,sha256=3xXSsSE49e7oEXwCeYQbglhvaj3WbVJwQtbR7Rio3wE,1908
+celestical/api/models/app.py,sha256=GCyA7wTkd91nSZaZLkBjECuGBLr47UzcwRylV_M25_o,3730
+celestical/api/models/bearer_response.py,sha256=NJ9sh54KeNdxyaGNudlX5ykYU3JjM8P3650mAuyJjRI,2938
+celestical/api/models/body_reset_forgot_password_auth_forgot_password_post.py,sha256=79ut-GVpE4RiQFFSDBgDR4H75RrT3rX-c8jt79jwgps,2690
+celestical/api/models/body_reset_reset_password_auth_reset_password_post.py,sha256=XbMhpcOHtiq-IUzwD7rsya0kyDIIBgHAr3Oe48fZJls,2982
+celestical/api/models/body_verify_request_token_auth_request_verify_token_post.py,sha256=RDqmi4Qne2KosantcQe-GQV3HbFxv7QIQJNC2xv49xQ,2702
+celestical/api/models/body_verify_verify_auth_verify_post.py,sha256=HXlcfWtKa1qLnWqiQ56hIsMKTIA9IAdjY2HrWb-Bg1E,2630
+celestical/api/models/client_id.py,sha256=RV7NcjIoJGSo_MMmVJlCYlFS4XMgyGFjLGXr_a7IAWU,4814
+celestical/api/models/client_secret.py,sha256=nOfYUMPD7nf8HlnIumVD1dD2-l0dzwuL7Bt-3DAxHcY,4842
+celestical/api/models/compose.py,sha256=cGK0C6_q8gWjhpgTyXoEri4GjxNAFsREbhnNNS1hg6k,3040
+celestical/api/models/deploy.py,sha256=0rUsci8wT75aOuBZM4ZMlqDBGb3mVFYb_7eCEuq0z50,4800
+celestical/api/models/detail.py,sha256=MX74EXNEXY_MuiCqK0wAxNKLN2Av8sTjUNtQ4NzGv4c,4911
+celestical/api/models/error_model.py,sha256=p5qNIA8MWobgK_JcEtImXZSOZ-K1qXk4UYJmk_4RjEk,2604
+celestical/api/models/first_creator.py,sha256=xRGK5to0X5GEEJPEkth6ORR1dxiwAC0bvmnfOM0m3zc,4842
+celestical/api/models/grant_type.py,sha256=-TKOZraKiAEZUMcRVrBkuukJ2V08Nl2ieT45OU37r10,4821
+celestical/api/models/http_validation_error.py,sha256=_Qo9y6bbKoLxIcJKI0m2iFbtlg-2B1GXOq--zm6-46Q,2601
+celestical/api/models/is_active.py,sha256=HYbzs3PQ3UeIPNWHmHnKdbp_uRruOIrY_Gae86tsm1Y,4814
+celestical/api/models/is_superuser.py,sha256=nxy44eJY3vLmtY8LuBdL2KrXWoYF9LvzMbVLlvy-9oY,4835
+celestical/api/models/is_verified.py,sha256=7A6Qfgztk5WuQDirb_sUsXGO9OsTWX-VM_hzFkhFMuQ,4828
+celestical/api/models/missing_apps.py,sha256=55P7VuHS4RXJ9o3G9d1xr_GKJ0ShEbdzNwzfXx504qI,2622
+celestical/api/models/missing_images.py,sha256=xh0ao8lMgJPT7bjGReOIJQah8GH2ZodZM8Rgr6UanrQ,2638
+celestical/api/models/name.py,sha256=RZe8rI7BkHRHhlWqKTxTKutdd58sMEWoJA30f78TvfQ,4786
+celestical/api/models/stack.py,sha256=Me8Qmj00_w1Ct7OcVNqYxdxrc2doHLEIOTRLPupeRIs,4225
+celestical/api/models/uploaded_image.py,sha256=-hVIIANC_nN7cjT5HgVgFytU8NmLEDQ6NHd_05VqUHY,2919
+celestical/api/models/user_create.py,sha256=szqBUrafzkpwNVv0bHvjIcVflKVuvu__6mbuK7j532Q,4425
+celestical/api/models/user_read.py,sha256=P6eCgdHAG3UHaTtT8yNrF7zpCLAeRqo2VPW19OwxHm8,4110
+celestical/api/models/validation_error.py,sha256=J7OyFxZwfrSv1AXgJJLrfFk3thtgs4K0kz78eivYBtE,3082
 celestical/api/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-celestical/api/rest.py,sha256=-B_yo7qUBGjdfkhhgOVaKmBeKzf4R5Iy0QSWvfDqzMc,9782
-celestical/apps.py,sha256=a2t9d2Vh3WgNzTNtESkmzEDcSvGkFb1A-CqLzm8aw6M,1594
-celestical/cli.py,sha256=1nvF30Xd1p84Sw5RA5ypKIYhucFNYKzX6aDiPAII_1Q,2520
-celestical/compose.py,sha256=IXFP-N80ujMLI86Isgrqenf4NUNX8TcyYl60HgMQNg4,23666
-celestical/configuration.py,sha256=u7S5cPAkkAFY1v_MgnIOlE13SXUg2WwdiKCBzVne1Rs,6974
-celestical/docker_local.py,sha256=o-yJ_WcjQzMbt_5J6sY2HKGF6L-OukcC6ixeFT-Fdq0,10101
-celestical/helper.py,sha256=S4PCbwrZ0-KnmTpQR8NyecaEqH53FXG8jP60xLm0GT0,9811
-celestical/user.py,sha256=Yb0nyq-TyNdr_aPnhyaBYPMRnQA3_BqP9Su7G96X_I4,7436
-celestical-0.18.5.dist-info/COPYING,sha256=5X8cMguM-HmKfS_4Om-eBqM6A1hfbgZf6pfx2G24QFI,35150
-celestical-0.18.5.dist-info/COPYING.LESSER,sha256=GkWx0KhgPf4s_GRPnauXCxdi-Sur4qrG6y9dRXLEpoA,7653
-celestical-0.18.5.dist-info/LICENSE,sha256=l4pgftTXn9aA9oyWYwUdY8St5XfN8v5bCjhSUZhNmfo,108
-celestical-0.18.5.dist-info/METADATA,sha256=bDD0FIcFb-fXo_faDAJv7KGxNCoK9SQ5_Q-bPAOnd_8,2587
-celestical-0.18.5.dist-info/WHEEL,sha256=d2fvjOD7sXsVzChCqf0Ty0JbHKBaLYwDbGQDwQTnJ50,88
-celestical-0.18.5.dist-info/entry_points.txt,sha256=I9_Hd8RvzIQVnSpFYLGSdlXl1SYrs2lg_4m8Rnghi1M,49
-celestical-0.18.5.dist-info/RECORD,,
+celestical/api/rest.py,sha256=BVDpxA9MvCU3oRg5PD1xbyFzq2i2NtefRqEf-9J4thM,9781
+celestical/apps.py,sha256=efrH9WcFLwtuLo9TFB7U5jAmHGCiQtfJHMEvVZjbofg,1533
+celestical/cli.py,sha256=GrP4lFfw-HXAwMFD7eo4o0cvWROA3o-qjz0MK_1JVTo,2425
+celestical/compose.py,sha256=0jzvhRW83W-xbDSExO7PUdaws9zOR71eO44qhRMw1E8,17341
+celestical/configuration.py,sha256=mVGYayYGvgQuhSP4T_0xAMoF5BXn72kCav-_UyONYkU,3900
+celestical/docker_local.py,sha256=A6tCVj3FIWmfGdB2b6Vz_apsWrzRA4eRF-PHSSjj2Jw,6138
+celestical/helper.py,sha256=krDgEOa0BtjuCSA4Wa3poP92THjTrC5pDV7iJBYpK20,6457
+celestical/stack_upload.py,sha256=y7WbQy-pgH0jI4vOiVmeHASQ_5tcLUjvK5h13PAspGI,9
+celestical/user.py,sha256=9Iz8GoMoQJe7wqHWcedp57vFLY5Bb9cutGesQ-XVbtk,6428
+celestical-0.9.2.dist-info/COPYING,sha256=5X8cMguM-HmKfS_4Om-eBqM6A1hfbgZf6pfx2G24QFI,35150
+celestical-0.9.2.dist-info/COPYING.LESSER,sha256=GkWx0KhgPf4s_GRPnauXCxdi-Sur4qrG6y9dRXLEpoA,7653
+celestical-0.9.2.dist-info/LICENSE,sha256=l4pgftTXn9aA9oyWYwUdY8St5XfN8v5bCjhSUZhNmfo,108
+celestical-0.9.2.dist-info/METADATA,sha256=U20NPz92MQJX6-DGECdzrM17RvOApDP1ybQQZcEd-Gk,1959
+celestical-0.9.2.dist-info/WHEEL,sha256=d2fvjOD7sXsVzChCqf0Ty0JbHKBaLYwDbGQDwQTnJ50,88
+celestical-0.9.2.dist-info/entry_points.txt,sha256=I9_Hd8RvzIQVnSpFYLGSdlXl1SYrs2lg_4m8Rnghi1M,49
+celestical-0.9.2.dist-info/RECORD,,
```

