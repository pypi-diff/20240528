# Comparing `tmp/clients_core-2.3.1-py3-none-any.whl.zip` & `tmp/clients_core-2.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,22 @@
-Zip file size: 11832 bytes, number of entries: 19
--rw-r--r--  2.0 unx      506 b- defN 23-Jul-03 11:29 clients_core/__init__.py
--rw-r--r--  2.0 unx     4847 b- defN 23-Jul-03 11:23 clients_core/api_match_client.py
--rw-r--r--  2.0 unx      464 b- defN 23-Jul-03 11:23 clients_core/exceptions.py
--rw-r--r--  2.0 unx     1157 b- defN 23-Jul-03 11:23 clients_core/rest_client.py
--rw-r--r--  2.0 unx     1196 b- defN 23-Jul-03 11:23 clients_core/secured_rest_client.py
--rw-r--r--  2.0 unx     2360 b- defN 23-Jul-03 11:23 clients_core/service_clients.py
--rw-r--r--  2.0 unx     1887 b- defN 23-Jul-03 11:23 clients_core/service_list_provider.py
--rw-r--r--  2.0 unx      830 b- defN 23-Jul-03 11:23 clients_core/settings.py
--rw-r--r--  2.0 unx     2883 b- defN 23-Jul-03 11:23 clients_core/simple_rest_client.py
--rw-r--r--  2.0 unx     1668 b- defN 23-Jul-03 11:23 clients_core/utils.py
--rw-r--r--  2.0 unx       13 b- defN 23-Jul-03 11:23 clients_core/authentication/__init__.py
--rw-r--r--  2.0 unx     1398 b- defN 23-Jul-03 11:23 clients_core/authentication/cache.py
--rw-r--r--  2.0 unx     1327 b- defN 23-Jul-03 11:23 clients_core/authentication/token_cache.py
--rw-r--r--  2.0 unx     1862 b- defN 23-Jul-03 11:23 clients_core/authentication/token_handler.py
--rw-rw-rw-  2.0 unx      575 b- defN 23-Jul-03 12:10 clients_core-2.3.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      979 b- defN 23-Jul-03 12:10 clients_core-2.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 12:10 clients_core-2.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Jul-03 12:10 clients_core-2.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1658 b- defN 23-Jul-03 12:10 clients_core-2.3.1.dist-info/RECORD
-19 files, 25715 bytes uncompressed, 9086 bytes compressed:  64.7%
+Zip file size: 12795 bytes, number of entries: 20
+-rw-r--r--  2.0 unx      575 b- defN 24-May-28 10:55 clients_core/__init__.py
+-rw-r--r--  2.0 unx     4847 b- defN 23-Jan-26 09:27 clients_core/api_match_client.py
+-rw-r--r--  2.0 unx      464 b- defN 23-Jan-26 09:27 clients_core/exceptions.py
+-rw-r--r--  2.0 unx     2765 b- defN 24-May-28 10:55 clients_core/models.py
+-rw-r--r--  2.0 unx     1157 b- defN 22-Nov-23 10:19 clients_core/rest_client.py
+-rw-r--r--  2.0 unx     1196 b- defN 23-Jan-26 09:27 clients_core/secured_rest_client.py
+-rw-r--r--  2.0 unx     2360 b- defN 23-Mar-09 15:55 clients_core/service_clients.py
+-rw-r--r--  2.0 unx     1887 b- defN 23-Jan-26 09:27 clients_core/service_list_provider.py
+-rw-r--r--  2.0 unx      830 b- defN 23-Jan-26 09:27 clients_core/settings.py
+-rw-r--r--  2.0 unx     2883 b- defN 23-Jan-26 10:46 clients_core/simple_rest_client.py
+-rw-r--r--  2.0 unx     1668 b- defN 23-Jan-26 09:27 clients_core/utils.py
+-rw-r--r--  2.0 unx       13 b- defN 22-Nov-23 10:19 clients_core/authentication/__init__.py
+-rw-r--r--  2.0 unx     1402 b- defN 24-May-28 10:55 clients_core/authentication/cache.py
+-rw-r--r--  2.0 unx     1327 b- defN 23-Jan-26 09:27 clients_core/authentication/token_cache.py
+-rw-r--r--  2.0 unx     1862 b- defN 23-Jan-26 09:27 clients_core/authentication/token_handler.py
+-rw-rw-rw-  2.0 unx      575 b- defN 24-May-28 11:11 clients_core-2.4.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      979 b- defN 24-May-28 11:11 clients_core-2.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 11:11 clients_core-2.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-May-28 11:11 clients_core-2.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1737 b- defN 24-May-28 11:11 clients_core-2.4.0.dist-info/RECORD
+20 files, 28632 bytes uncompressed, 9929 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -3,14 +3,17 @@
 
 Filename: clients_core/api_match_client.py
 Comment: 
 
 Filename: clients_core/exceptions.py
 Comment: 
 
+Filename: clients_core/models.py
+Comment: 
+
 Filename: clients_core/rest_client.py
 Comment: 
 
 Filename: clients_core/secured_rest_client.py
 Comment: 
 
 Filename: clients_core/service_clients.py
@@ -36,23 +39,23 @@
 
 Filename: clients_core/authentication/token_cache.py
 Comment: 
 
 Filename: clients_core/authentication/token_handler.py
 Comment: 
 
-Filename: clients_core-2.3.1.dist-info/LICENSE.txt
+Filename: clients_core-2.4.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: clients_core-2.3.1.dist-info/METADATA
+Filename: clients_core-2.4.0.dist-info/METADATA
 Comment: 
 
-Filename: clients_core-2.3.1.dist-info/WHEEL
+Filename: clients_core-2.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: clients_core-2.3.1.dist-info/top_level.txt
+Filename: clients_core-2.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: clients_core-2.3.1.dist-info/RECORD
+Filename: clients_core-2.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## clients_core/__init__.py

```diff
@@ -1,21 +1,23 @@
-__version__ = "2.3.1"
+__version__ = "2.4.0"
 
 __all__ = [
     "authentication",
     "SimpleRestClient",
     "SecuredRestClient",
     "RestClient",
     "ApiMatchClient",
     "ServiceDirectoryMatchClient",
     "GatewayMatchClient",
+    "JsonPatchModel",
 ]
 
 
-from clients_core.simple_rest_client import SimpleRestClient
-from clients_core.secured_rest_client import SecuredRestClient
-from clients_core.rest_client import RestClient
 from clients_core.api_match_client import (
     ApiMatchClient,
-    ServiceDirectoryMatchClient,
     GatewayMatchClient,
+    ServiceDirectoryMatchClient,
 )
+from clients_core.models import JsonPatchModel
+from clients_core.rest_client import RestClient
+from clients_core.secured_rest_client import SecuredRestClient
+from clients_core.simple_rest_client import SimpleRestClient
```

## clients_core/authentication/cache.py

```diff
@@ -34,12 +34,12 @@
         self.connection = Redis.from_url(connection_url)
 
     def get(self, key: str) -> Optional[bytes]:
         return self.connection.get(key)
 
     def set(self, key: str, value: str, **kwargs: dict) -> Optional[bool]:
         ex = kwargs.pop("ex", None)
-        if ex is not None and not type(ex) == int:
+        if ex is not None and not isinstance(ex, int):
             raise ValueError(
                 "Expire flag `ex` is in seconds, and must be an integer or None"
             )
         return self.connection.set(key, value, ex=cast(Optional[int], ex))
```

## Comparing `clients_core-2.3.1.dist-info/LICENSE.txt` & `clients_core-2.4.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `clients_core-2.3.1.dist-info/METADATA` & `clients_core-2.4.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clients-core
-Version: 2.3.1
+Version: 2.4.0
 Summary: A collection of Python connection clients for E360 Microservices
 Author: IQVIA
 Author-email: e360pypi@iqvia.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `clients_core-2.3.1.dist-info/RECORD` & `clients_core-2.4.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-clients_core/__init__.py,sha256=E3zkeTJTBeg6PmpKFVn4BPt93j_JN_WLk0jMYiQFDlM,506
+clients_core/__init__.py,sha256=e_cJosd0F6HMpEPDZ-PFIDO7mfoJv1EW4epc5vNwKzU,575
 clients_core/api_match_client.py,sha256=t3KBckPIGg1j2yR9oauC3MlKgI9ZfLh_1gfKSO2Je7A,4847
 clients_core/exceptions.py,sha256=EJWQTldusInf274aLEJwtRnaNaY49QF2shebIb1V4dM,464
+clients_core/models.py,sha256=uF0MfuR-fw-GQ5zkFTCB3H5BzZp_TKpAPnMgSWTkxG4,2765
 clients_core/rest_client.py,sha256=I7tKOcpl8PY757UbFGOC15ximiWJqHue9Gx-NKZF11Y,1157
 clients_core/secured_rest_client.py,sha256=4AeqizH4vRJjlYL0AMKNuEjEkXA05f5NyshcxD44src,1196
 clients_core/service_clients.py,sha256=3ycHcAXfKeAXEU8-jXbH3ilqRJK1TjW9w7Q-wvCIJ9o,2360
 clients_core/service_list_provider.py,sha256=jNNxHGxf5B4QK-GeMjnhm3bCH9PJixwNqiTmLz5J3A8,1887
 clients_core/settings.py,sha256=w2CRV-b7WIZEIeAXlc39f86-Uui1tOt4_A_ZYOrLM0k,830
 clients_core/simple_rest_client.py,sha256=kVTCD_9lpfYWGE0iouTooxDVrib8eLJ2Vvu8jhzKHTs,2883
 clients_core/utils.py,sha256=ANwfyjEebtUQNS8kyWhZLTPAaAttny9Ch82PORY8wG4,1668
 clients_core/authentication/__init__.py,sha256=pPJwUwfJkKZehdjBxubZlUB6TRIrO1cSX5zLf4qjRYY,13
-clients_core/authentication/cache.py,sha256=-KeYyXJBPyqW5s7pwm6AfrZhWR8x4NOHqm0GuhUL2wU,1398
+clients_core/authentication/cache.py,sha256=cuy3XJENDPsAmQWAZkwOpnsIkbcA6-5VfOTs7W3YhjE,1402
 clients_core/authentication/token_cache.py,sha256=woTGb302nzIHcxqr7sQA2QU7Ittrqa9l2AmYy9Dd9JM,1327
 clients_core/authentication/token_handler.py,sha256=PDe1wV8qyFfcOVY-FpcJw0cfuZV40d2bxdYPshIO9dY,1862
-clients_core-2.3.1.dist-info/LICENSE.txt,sha256=uoI1G5lxk8h5Ua5OqmR7137DhTctSXGt9z7EBa1yclI,575
-clients_core-2.3.1.dist-info/METADATA,sha256=kpGCQtv4JT86qDXHtDM0CAsAG827x2eWRNWlWZhmLhU,979
-clients_core-2.3.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-clients_core-2.3.1.dist-info/top_level.txt,sha256=s6fAKq7CM_84hchGIP9ZKqbTzn_4RuMf6gp_aGL8D6s,13
-clients_core-2.3.1.dist-info/RECORD,,
+clients_core-2.4.0.dist-info/LICENSE.txt,sha256=uoI1G5lxk8h5Ua5OqmR7137DhTctSXGt9z7EBa1yclI,575
+clients_core-2.4.0.dist-info/METADATA,sha256=kpbLcBO6EThXCsuUdA9WTVK-jSYfcQYOYt_DqhjAC2I,979
+clients_core-2.4.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+clients_core-2.4.0.dist-info/top_level.txt,sha256=s6fAKq7CM_84hchGIP9ZKqbTzn_4RuMf6gp_aGL8D6s,13
+clients_core-2.4.0.dist-info/RECORD,,
```

