# Comparing `tmp/klarda_python_sdk-1.0.1.tar.gz` & `tmp/klarda_python_sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klarda_python_sdk-1.0.1.tar", max compression
+gzip compressed data, was "klarda_python_sdk-1.0.2.tar", max compression
```

## Comparing `klarda_python_sdk-1.0.1.tar` & `klarda_python_sdk-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       83 2024-05-14 08:37:06.860766 klarda_python_sdk-1.0.1/klarda/__init__.py
--rw-r--r--   0        0        0     4723 2024-05-15 13:41:28.464251 klarda_python_sdk-1.0.1/klarda/apis.py
--rw-r--r--   0        0        0      221 2024-05-14 08:37:11.111959 klarda_python_sdk-1.0.1/klarda/exceptions.py
--rw-r--r--   0        0        0     2072 2024-05-15 12:17:18.329932 klarda_python_sdk-1.0.1/klarda/providers.py
--rw-r--r--   0        0        0    11278 2024-05-15 13:40:47.654696 klarda_python_sdk-1.0.1/klarda/types.py
--rw-r--r--   0        0        0     1092 2024-05-13 13:05:54.423560 klarda_python_sdk-1.0.1/LICENSE
--rw-r--r--   0        0        0      878 2024-05-16 06:40:19.549729 klarda_python_sdk-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1356 2024-05-16 06:37:20.889343 klarda_python_sdk-1.0.1/README.md
--rw-r--r--   0        0        0     2306 1970-01-01 00:00:00.000000 klarda_python_sdk-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       83 2024-05-14 08:37:06.860766 klarda_python_sdk-1.0.2/klarda/__init__.py
+-rw-r--r--   0        0        0    19573 2024-05-22 04:01:42.461896 klarda_python_sdk-1.0.2/klarda/apis.py
+-rw-r--r--   0        0        0      221 2024-05-14 08:37:11.111959 klarda_python_sdk-1.0.2/klarda/exceptions.py
+-rw-r--r--   0        0        0     2663 2024-05-28 14:20:10.291660 klarda_python_sdk-1.0.2/klarda/providers.py
+-rw-r--r--   0        0        0    69784 2024-05-28 14:19:46.064210 klarda_python_sdk-1.0.2/klarda/types.py
+-rw-r--r--   0        0        0     1092 2024-05-13 13:05:54.423560 klarda_python_sdk-1.0.2/LICENSE
+-rw-r--r--   0        0        0      878 2024-05-28 14:32:21.872919 klarda_python_sdk-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1356 2024-05-16 06:37:20.889343 klarda_python_sdk-1.0.2/README.md
+-rw-r--r--   0        0        0     2306 1970-01-01 00:00:00.000000 klarda_python_sdk-1.0.2/PKG-INFO
```

### Comparing `klarda_python_sdk-1.0.1/klarda/providers.py` & `klarda_python_sdk-1.0.2/klarda/providers.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,34 +17,46 @@
         self.api_key = api_key
 
     def make_request(self, method_url: str, params: Optional[Any], reply: Optional[Any]) -> Optional[Any]:
         if not isinstance(params, dict):
             params = params.to_dict()
         params["api_key"] = self.api_key
         response = requests.get(self.endpoint_uri + method_url, params=params).json()
-        reply = [reply.from_dict(**item) for item in response["data"]]
+        reply = [reply.from_dict(**item).to_dict() for item in response["data"]]
         if response.get("error"):
             raise APIError(response["error"])
         if len(response["data"]) == 0:
             raise APIError("returned no result")
         return reply
     
     def make_request_with_total(self, method_url: str, params: Optional[Any], reply: Optional[Any]) -> Optional[Any]:
         if not isinstance(params, dict):
             params = params.to_dict()
         params["api_key"] = self.api_key
         response = requests.get(self.endpoint_uri + method_url, params=params).json()
-        reply = [reply.from_dict(**item) for item in response["data"]["result"]]
+        reply = [reply.from_dict(item).to_dict() for item in response["data"]["result"]]
         if response.get("error"):
             raise APIError(response["error"])
         if len(response["data"]["result"]) == 0:
             raise APIError("returned no result")
         result = {"total": response["data"]["total"], "result": reply}
         return result
     
     def make_request_without_params(self, method_url: str) -> Optional[Any]:
         params = {}
         params["api_key"] = self.api_key
         response = requests.get(self.endpoint_uri + method_url, params=params).json()
         if response.get("error"):
             raise APIError(response["error"])
         return response
+    
+    def make_request_with_dict_return(self, method_url: str, params: Optional[Any], reply: Optional[Any]) -> Optional[Any]:
+        if not isinstance(params, dict):
+            params = params.to_dict()
+        params["api_key"] = self.api_key
+        response = requests.get(self.endpoint_uri + method_url, params=params).json()
+        reply = response["data"]
+        if response.get("error"):
+            raise APIError(response["error"])
+        # if len(response["data"]) == 0:
+        #     raise APIError("returned no result")
+        return reply
```

### Comparing `klarda_python_sdk-1.0.1/LICENSE` & `klarda_python_sdk-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `klarda_python_sdk-1.0.1/pyproject.toml` & `klarda_python_sdk-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "klarda-python-sdk"
-version = "1.0.1"
+version = "1.0.2"
 description = "Refined Python library for interaction with Klarda's APIs."
 authors = [
     "Thinh Q.D. Pham <thinh.pham@klarda.com> <pqducthinhbka@gmail.com>",
 ]
 license = "MIT License"
 
 homepage = "https://klarda.com/"
```

### Comparing `klarda_python_sdk-1.0.1/README.md` & `klarda_python_sdk-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `klarda_python_sdk-1.0.1/PKG-INFO` & `klarda_python_sdk-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klarda-python-sdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: Refined Python library for interaction with Klarda's APIs.
 Home-page: https://klarda.com/
 License: MIT
 Keywords: klarda,sdk,blockchain,token
 Author: Thinh Q.D. Pham
 Author-email: thinh.pham@klarda.com> <pqducthinhbka@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

