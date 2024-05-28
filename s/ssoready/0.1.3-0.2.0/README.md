# Comparing `tmp/ssoready-0.1.3.tar.gz` & `tmp/ssoready-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssoready-0.1.3.tar", max compression
+gzip compressed data, was "ssoready-0.2.0.tar", max compression
```

## Comparing `ssoready-0.1.3.tar` & `ssoready-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     3902 2024-05-24 16:49:55.924524 ssoready-0.1.3/README.md
--rw-r--r--   0        0        0     1337 2024-05-24 16:49:55.924524 ssoready-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      447 2024-05-24 16:49:55.924524 ssoready-0.1.3/src/ssoready/__init__.py
--rw-r--r--   0        0        0     5535 2024-05-24 16:49:55.924524 ssoready-0.1.3/src/ssoready/client.py
--rw-r--r--   0        0        0      973 2024-05-24 16:49:55.924524 ssoready-0.1.3/src/ssoready/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-24 16:49:55.924524 ssoready-0.1.3/src/ssoready/core/api_error.py
--rw-r--r--   0        0        0     2093 2024-05-24 16:49:55.924524 ssoready-0.1.3/src/ssoready/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-24 16:49:55.924524 ssoready-0.1.3/src/ssoready/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-05-24 16:49:55.924524 ssoready-0.1.3/src/ssoready/core/file.py
--rw-r--r--   0        0        0     5059 2024-05-24 16:49:55.924524 ssoready-0.1.3/src/ssoready/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-05-24 16:49:55.924524 ssoready-0.1.3/src/ssoready/core/jsonable_encoder.py
--rw-r--r--   0        0        0      748 2024-05-24 16:49:55.924524 ssoready-0.1.3/src/ssoready/core/pydantic_utilities.py
--rw-r--r--   0        0        0     1266 2024-05-24 16:49:55.924524 ssoready-0.1.3/src/ssoready/core/query_encoder.py
--rw-r--r--   0        0        0      330 2024-05-24 16:49:55.924524 ssoready-0.1.3/src/ssoready/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-05-24 16:49:55.924524 ssoready-0.1.3/src/ssoready/core/request_options.py
--rw-r--r--   0        0        0      178 2024-05-24 16:49:55.924524 ssoready-0.1.3/src/ssoready/environment.py
--rw-r--r--   0        0        0        0 2024-05-24 16:49:55.924524 ssoready-0.1.3/src/ssoready/py.typed
--rw-r--r--   0        0        0       65 2024-05-24 16:49:55.924524 ssoready-0.1.3/src/ssoready/saml/__init__.py
--rw-r--r--   0        0        0    14610 2024-05-24 16:49:55.924524 ssoready-0.1.3/src/ssoready/saml/client.py
--rw-r--r--   0        0        0      394 2024-05-24 16:49:55.924524 ssoready-0.1.3/src/ssoready/types/__init__.py
--rw-r--r--   0        0        0     1363 2024-05-24 16:49:55.924524 ssoready-0.1.3/src/ssoready/types/get_saml_redirect_url_response.py
--rw-r--r--   0        0        0     1453 2024-05-24 16:49:55.924524 ssoready-0.1.3/src/ssoready/types/google_protobuf_any.py
--rw-r--r--   0        0        0     2208 2024-05-24 16:49:55.924524 ssoready-0.1.3/src/ssoready/types/redeem_saml_access_code_response.py
--rw-r--r--   0        0        0     2315 2024-05-24 16:49:55.924524 ssoready-0.1.3/src/ssoready/types/status.py
--rw-r--r--   0        0        0       76 2024-05-24 16:49:55.924524 ssoready-0.1.3/src/ssoready/version.py
--rw-r--r--   0        0        0     4855 1970-01-01 00:00:00.000000 ssoready-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3902 2024-05-28 16:34:55.853289 ssoready-0.2.0/README.md
+-rw-r--r--   0        0        0     1337 2024-05-28 16:34:55.853289 ssoready-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      447 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/__init__.py
+-rw-r--r--   0        0        0     5535 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/client.py
+-rw-r--r--   0        0        0      973 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/core/api_error.py
+-rw-r--r--   0        0        0     2093 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      748 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/core/pydantic_utilities.py
+-rw-r--r--   0        0        0     1266 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/core/query_encoder.py
+-rw-r--r--   0        0        0      330 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/core/request_options.py
+-rw-r--r--   0        0        0      178 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/environment.py
+-rw-r--r--   0        0        0        0 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/py.typed
+-rw-r--r--   0        0        0       65 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/saml/__init__.py
+-rw-r--r--   0        0        0    14472 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/saml/client.py
+-rw-r--r--   0        0        0      394 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/types/__init__.py
+-rw-r--r--   0        0        0     1363 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/types/get_saml_redirect_url_response.py
+-rw-r--r--   0        0        0     1453 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/types/google_protobuf_any.py
+-rw-r--r--   0        0        0     2208 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/types/redeem_saml_access_code_response.py
+-rw-r--r--   0        0        0     2315 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/types/status.py
+-rw-r--r--   0        0        0       76 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/version.py
+-rw-r--r--   0        0        0     4855 1970-01-01 00:00:00.000000 ssoready-0.2.0/PKG-INFO
```

### Comparing `ssoready-0.1.3/README.md` & `ssoready-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ssoready-0.1.3/pyproject.toml` & `ssoready-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssoready"
-version = "0.1.3"
+version = "0.2.0"
 description = ""
 readme = "README.md"
 authors = []
 keywords = []
 
 classifiers = [
     "Intended Audience :: Developers",
```

### Comparing `ssoready-0.1.3/src/ssoready/client.py` & `ssoready-0.2.0/src/ssoready/client.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.1.3/src/ssoready/core/__init__.py` & `ssoready-0.2.0/src/ssoready/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.1.3/src/ssoready/core/client_wrapper.py` & `ssoready-0.2.0/src/ssoready/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "ssoready",
-            "X-Fern-SDK-Version": "0.1.3",
+            "X-Fern-SDK-Version": "0.2.0",
         }
         api_key = self._get_api_key()
         if api_key is not None:
             headers["Authorization"] = f"Bearer {api_key}"
         return headers
 
     def _get_api_key(self) -> typing.Optional[str]:
```

### Comparing `ssoready-0.1.3/src/ssoready/core/datetime_utils.py` & `ssoready-0.2.0/src/ssoready/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.1.3/src/ssoready/core/file.py` & `ssoready-0.2.0/src/ssoready/core/file.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.1.3/src/ssoready/core/http_client.py` & `ssoready-0.2.0/src/ssoready/core/http_client.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.1.3/src/ssoready/core/jsonable_encoder.py` & `ssoready-0.2.0/src/ssoready/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.1.3/src/ssoready/core/pydantic_utilities.py` & `ssoready-0.2.0/src/ssoready/core/pydantic_utilities.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.1.3/src/ssoready/core/query_encoder.py` & `ssoready-0.2.0/src/ssoready/core/query_encoder.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.1.3/src/ssoready/core/request_options.py` & `ssoready-0.2.0/src/ssoready/core/request_options.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.1.3/src/ssoready/saml/client.py` & `ssoready-0.2.0/src/ssoready/saml/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 OMIT = typing.cast(typing.Any, ...)
 
 
 class SamlClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def redeem_access_code(
+    def redeem_saml_access_code(
         self, *, saml_access_code: typing.Optional[str] = OMIT, request_options: typing.Optional[RequestOptions] = None
     ) -> RedeemSamlAccessCodeResponse:
         """
         Exchange a SAML access code for details about a SAML login.
 
         Parameters
         ----------
@@ -43,16 +43,16 @@
         Examples
         --------
         from ssoready.client import SSOReady
 
         client = SSOReady(
             api_key="YOUR_API_KEY",
         )
-        client.saml.redeem_access_code(
-            saml_access_code="saml_access_code_94d90b43a2027a9084bfc792",
+        client.saml.redeem_saml_access_code(
+            saml_access_code="saml_access_code_...",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if saml_access_code is not OMIT:
             _request["samlAccessCode"] = saml_access_code
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
@@ -86,15 +86,15 @@
             return pydantic_v1.parse_obj_as(RedeemSamlAccessCodeResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_redirect_url(
+    def get_saml_redirect_url(
         self,
         *,
         saml_connection_id: typing.Optional[str] = OMIT,
         organization_id: typing.Optional[str] = OMIT,
         organization_external_id: typing.Optional[str] = OMIT,
         state: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
@@ -133,17 +133,16 @@
         Examples
         --------
         from ssoready.client import SSOReady
 
         client = SSOReady(
             api_key="YOUR_API_KEY",
         )
-        client.saml.get_redirect_url(
-            saml_connection_id="saml_conn_ac3bzzoqhaa88ozk29hhv12l",
-            organization_id="org_7cu5hsy9vrbi5d2k1qvbh19lj",
+        client.saml.get_saml_redirect_url(
+            organization_external_id="my_custom_external_id",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if saml_connection_id is not OMIT:
             _request["samlConnectionId"] = saml_connection_id
         if organization_id is not OMIT:
             _request["organizationId"] = organization_id
@@ -188,15 +187,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncSamlClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def redeem_access_code(
+    async def redeem_saml_access_code(
         self, *, saml_access_code: typing.Optional[str] = OMIT, request_options: typing.Optional[RequestOptions] = None
     ) -> RedeemSamlAccessCodeResponse:
         """
         Exchange a SAML access code for details about a SAML login.
 
         Parameters
         ----------
@@ -213,16 +212,16 @@
         Examples
         --------
         from ssoready.client import AsyncSSOReady
 
         client = AsyncSSOReady(
             api_key="YOUR_API_KEY",
         )
-        await client.saml.redeem_access_code(
-            saml_access_code="saml_access_code_94d90b43a2027a9084bfc792",
+        await client.saml.redeem_saml_access_code(
+            saml_access_code="saml_access_code_...",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if saml_access_code is not OMIT:
             _request["samlAccessCode"] = saml_access_code
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
@@ -256,15 +255,15 @@
             return pydantic_v1.parse_obj_as(RedeemSamlAccessCodeResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_redirect_url(
+    async def get_saml_redirect_url(
         self,
         *,
         saml_connection_id: typing.Optional[str] = OMIT,
         organization_id: typing.Optional[str] = OMIT,
         organization_external_id: typing.Optional[str] = OMIT,
         state: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
@@ -303,17 +302,16 @@
         Examples
         --------
         from ssoready.client import AsyncSSOReady
 
         client = AsyncSSOReady(
             api_key="YOUR_API_KEY",
         )
-        await client.saml.get_redirect_url(
-            saml_connection_id="saml_conn_ac3bzzoqhaa88ozk29hhv12l",
-            organization_id="org_7cu5hsy9vrbi5d2k1qvbh19lj",
+        await client.saml.get_saml_redirect_url(
+            organization_external_id="my_custom_external_id",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if saml_connection_id is not OMIT:
             _request["samlConnectionId"] = saml_connection_id
         if organization_id is not OMIT:
             _request["organizationId"] = organization_id
```

### Comparing `ssoready-0.1.3/src/ssoready/types/get_saml_redirect_url_response.py` & `ssoready-0.2.0/src/ssoready/types/get_saml_redirect_url_response.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.1.3/src/ssoready/types/google_protobuf_any.py` & `ssoready-0.2.0/src/ssoready/types/google_protobuf_any.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.1.3/src/ssoready/types/redeem_saml_access_code_response.py` & `ssoready-0.2.0/src/ssoready/types/redeem_saml_access_code_response.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.1.3/src/ssoready/types/status.py` & `ssoready-0.2.0/src/ssoready/types/status.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.1.3/PKG-INFO` & `ssoready-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssoready
-Version: 0.1.3
+Version: 0.2.0
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX
```

