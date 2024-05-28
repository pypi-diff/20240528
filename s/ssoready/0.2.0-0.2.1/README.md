# Comparing `tmp/ssoready-0.2.0.tar.gz` & `tmp/ssoready-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssoready-0.2.0.tar", max compression
+gzip compressed data, was "ssoready-0.2.1.tar", max compression
```

## Comparing `ssoready-0.2.0.tar` & `ssoready-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     3902 2024-05-28 16:34:55.853289 ssoready-0.2.0/README.md
--rw-r--r--   0        0        0     1337 2024-05-28 16:34:55.853289 ssoready-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      447 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/__init__.py
--rw-r--r--   0        0        0     5535 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/client.py
--rw-r--r--   0        0        0      973 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/core/api_error.py
--rw-r--r--   0        0        0     2093 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/core/file.py
--rw-r--r--   0        0        0     5059 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/core/jsonable_encoder.py
--rw-r--r--   0        0        0      748 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/core/pydantic_utilities.py
--rw-r--r--   0        0        0     1266 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/core/query_encoder.py
--rw-r--r--   0        0        0      330 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/core/request_options.py
--rw-r--r--   0        0        0      178 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/environment.py
--rw-r--r--   0        0        0        0 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/py.typed
--rw-r--r--   0        0        0       65 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/saml/__init__.py
--rw-r--r--   0        0        0    14472 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/saml/client.py
--rw-r--r--   0        0        0      394 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/types/__init__.py
--rw-r--r--   0        0        0     1363 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/types/get_saml_redirect_url_response.py
--rw-r--r--   0        0        0     1453 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/types/google_protobuf_any.py
--rw-r--r--   0        0        0     2208 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/types/redeem_saml_access_code_response.py
--rw-r--r--   0        0        0     2315 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/types/status.py
--rw-r--r--   0        0        0       76 2024-05-28 16:34:55.857289 ssoready-0.2.0/src/ssoready/version.py
--rw-r--r--   0        0        0     4855 1970-01-01 00:00:00.000000 ssoready-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-28 19:12:01.933037 ssoready-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2940 2024-05-28 19:12:01.933037 ssoready-0.2.1/README.md
+-rw-r--r--   0        0        0     1398 2024-05-28 19:12:01.933037 ssoready-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      447 2024-05-28 19:12:01.933037 ssoready-0.2.1/src/ssoready/__init__.py
+-rw-r--r--   0        0        0     5535 2024-05-28 19:12:01.933037 ssoready-0.2.1/src/ssoready/client.py
+-rw-r--r--   0        0        0      973 2024-05-28 19:12:01.933037 ssoready-0.2.1/src/ssoready/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-28 19:12:01.933037 ssoready-0.2.1/src/ssoready/core/api_error.py
+-rw-r--r--   0        0        0     2093 2024-05-28 19:12:01.933037 ssoready-0.2.1/src/ssoready/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-28 19:12:01.933037 ssoready-0.2.1/src/ssoready/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-28 19:12:01.933037 ssoready-0.2.1/src/ssoready/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-28 19:12:01.933037 ssoready-0.2.1/src/ssoready/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-28 19:12:01.933037 ssoready-0.2.1/src/ssoready/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      748 2024-05-28 19:12:01.937037 ssoready-0.2.1/src/ssoready/core/pydantic_utilities.py
+-rw-r--r--   0        0        0     1266 2024-05-28 19:12:01.937037 ssoready-0.2.1/src/ssoready/core/query_encoder.py
+-rw-r--r--   0        0        0      330 2024-05-28 19:12:01.937037 ssoready-0.2.1/src/ssoready/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-28 19:12:01.937037 ssoready-0.2.1/src/ssoready/core/request_options.py
+-rw-r--r--   0        0        0      158 2024-05-28 19:12:01.937037 ssoready-0.2.1/src/ssoready/environment.py
+-rw-r--r--   0        0        0        0 2024-05-28 19:12:01.937037 ssoready-0.2.1/src/ssoready/py.typed
+-rw-r--r--   0        0        0       65 2024-05-28 19:12:01.937037 ssoready-0.2.1/src/ssoready/saml/__init__.py
+-rw-r--r--   0        0        0    14472 2024-05-28 19:12:01.937037 ssoready-0.2.1/src/ssoready/saml/client.py
+-rw-r--r--   0        0        0      394 2024-05-28 19:12:01.937037 ssoready-0.2.1/src/ssoready/types/__init__.py
+-rw-r--r--   0        0        0     1363 2024-05-28 19:12:01.937037 ssoready-0.2.1/src/ssoready/types/get_saml_redirect_url_response.py
+-rw-r--r--   0        0        0     1453 2024-05-28 19:12:01.937037 ssoready-0.2.1/src/ssoready/types/google_protobuf_any.py
+-rw-r--r--   0        0        0     2208 2024-05-28 19:12:01.937037 ssoready-0.2.1/src/ssoready/types/redeem_saml_access_code_response.py
+-rw-r--r--   0        0        0     2315 2024-05-28 19:12:01.937037 ssoready-0.2.1/src/ssoready/types/status.py
+-rw-r--r--   0        0        0       76 2024-05-28 19:12:01.937037 ssoready-0.2.1/src/ssoready/version.py
+-rw-r--r--   0        0        0     3957 1970-01-01 00:00:00.000000 ssoready-0.2.1/PKG-INFO
```

### Comparing `ssoready-0.2.0/pyproject.toml` & `ssoready-0.2.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "ssoready"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 readme = "README.md"
 authors = []
 keywords = []
-
+license = "MIT"
 classifiers = [
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -17,15 +17,16 @@
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
     "Operating System :: POSIX",
     "Operating System :: MacOS",
     "Operating System :: POSIX :: Linux",
     "Operating System :: Microsoft :: Windows",
     "Topic :: Software Development :: Libraries :: Python Modules",
-    "Typing :: Typed"
+    "Typing :: Typed",
+    "License :: OSI Approved :: MIT License"
 ]
 packages = [
     { include = "ssoready", from = "src"}
 ]
 
 [project.urls]
 Repository = 'https://github.com/ssoready/ssoready-python'
```

### Comparing `ssoready-0.2.0/src/ssoready/client.py` & `ssoready-0.2.1/src/ssoready/client.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.2.0/src/ssoready/core/__init__.py` & `ssoready-0.2.1/src/ssoready/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.2.0/src/ssoready/core/client_wrapper.py` & `ssoready-0.2.1/src/ssoready/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "ssoready",
-            "X-Fern-SDK-Version": "0.2.0",
+            "X-Fern-SDK-Version": "0.2.1",
         }
         api_key = self._get_api_key()
         if api_key is not None:
             headers["Authorization"] = f"Bearer {api_key}"
         return headers
 
     def _get_api_key(self) -> typing.Optional[str]:
```

### Comparing `ssoready-0.2.0/src/ssoready/core/datetime_utils.py` & `ssoready-0.2.1/src/ssoready/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.2.0/src/ssoready/core/file.py` & `ssoready-0.2.1/src/ssoready/core/file.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.2.0/src/ssoready/core/http_client.py` & `ssoready-0.2.1/src/ssoready/core/http_client.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.2.0/src/ssoready/core/jsonable_encoder.py` & `ssoready-0.2.1/src/ssoready/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.2.0/src/ssoready/core/pydantic_utilities.py` & `ssoready-0.2.1/src/ssoready/core/pydantic_utilities.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.2.0/src/ssoready/core/query_encoder.py` & `ssoready-0.2.1/src/ssoready/core/query_encoder.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.2.0/src/ssoready/core/request_options.py` & `ssoready-0.2.1/src/ssoready/core/request_options.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.2.0/src/ssoready/saml/client.py` & `ssoready-0.2.1/src/ssoready/saml/client.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.2.0/src/ssoready/types/get_saml_redirect_url_response.py` & `ssoready-0.2.1/src/ssoready/types/get_saml_redirect_url_response.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.2.0/src/ssoready/types/google_protobuf_any.py` & `ssoready-0.2.1/src/ssoready/types/google_protobuf_any.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.2.0/src/ssoready/types/redeem_saml_access_code_response.py` & `ssoready-0.2.1/src/ssoready/types/redeem_saml_access_code_response.py`

 * *Files identical despite different names*

### Comparing `ssoready-0.2.0/src/ssoready/types/status.py` & `ssoready-0.2.1/src/ssoready/types/status.py`

 * *Files identical despite different names*

