# Comparing `tmp/supabase-2.4.6.tar.gz` & `tmp/supabase-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supabase-2.4.6.tar", max compression
+gzip compressed data, was "supabase-2.5.0.tar", max compression
```

## Comparing `supabase-2.4.6.tar` & `supabase-2.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1067 2024-05-22 20:10:06.418868 supabase-2.4.6/LICENSE
--rw-r--r--   0        0        0     8244 2024-05-22 20:10:06.418868 supabase-2.4.6/README.md
--rw-r--r--   0        0        0     1892 2024-05-22 20:10:14.842875 supabase-2.4.6/pyproject.toml
--rw-r--r--   0        0        0     1224 2024-05-22 20:10:06.418868 supabase-2.4.6/supabase/__init__.py
--rw-r--r--   0        0        0       22 2024-05-22 20:10:14.842875 supabase-2.4.6/supabase/__version__.py
--rw-r--r--   0        0        0       35 2024-05-22 20:10:06.418868 supabase-2.4.6/supabase/_async/__init__.py
--rw-r--r--   0        0        0     1130 2024-05-22 20:10:06.418868 supabase-2.4.6/supabase/_async/auth_client.py
--rw-r--r--   0        0        0    10114 2024-05-22 20:10:06.418868 supabase-2.4.6/supabase/_async/client.py
--rw-r--r--   0        0        0       35 2024-05-22 20:10:06.418868 supabase-2.4.6/supabase/_sync/__init__.py
--rw-r--r--   0        0        0     1120 2024-05-22 20:10:06.418868 supabase-2.4.6/supabase/_sync/auth_client.py
--rw-r--r--   0        0        0    10081 2024-05-22 20:10:06.418868 supabase-2.4.6/supabase/_sync/client.py
--rw-r--r--   0        0        0     1172 2024-05-22 20:10:06.418868 supabase-2.4.6/supabase/client.py
--rw-r--r--   0        0        0      127 2024-05-22 20:10:06.418868 supabase-2.4.6/supabase/lib/__init__.py
--rw-r--r--   0        0        0     3135 2024-05-22 20:10:06.418868 supabase-2.4.6/supabase/lib/client_options.py
--rw-r--r--   0        0        0     1892 2024-05-22 20:10:06.418868 supabase-2.4.6/supabase/lib/realtime_client.py
--rw-r--r--   0        0        0        0 2024-05-22 20:10:06.418868 supabase-2.4.6/supabase/py.typed
--rw-r--r--   0        0        0     9313 1970-01-01 00:00:00.000000 supabase-2.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-28 12:17:36.874589 supabase-2.5.0/LICENSE
+-rw-r--r--   0        0        0     8244 2024-05-28 12:17:36.874589 supabase-2.5.0/README.md
+-rw-r--r--   0        0        0     1892 2024-05-28 12:17:45.018540 supabase-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1224 2024-05-28 12:17:36.874589 supabase-2.5.0/supabase/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-28 12:17:45.018540 supabase-2.5.0/supabase/__version__.py
+-rw-r--r--   0        0        0       35 2024-05-28 12:17:36.874589 supabase-2.5.0/supabase/_async/__init__.py
+-rw-r--r--   0        0        0     1130 2024-05-28 12:17:36.874589 supabase-2.5.0/supabase/_async/auth_client.py
+-rw-r--r--   0        0        0    10560 2024-05-28 12:17:36.874589 supabase-2.5.0/supabase/_async/client.py
+-rw-r--r--   0        0        0       35 2024-05-28 12:17:36.874589 supabase-2.5.0/supabase/_sync/__init__.py
+-rw-r--r--   0        0        0     1120 2024-05-28 12:17:36.874589 supabase-2.5.0/supabase/_sync/auth_client.py
+-rw-r--r--   0        0        0    10526 2024-05-28 12:17:36.874589 supabase-2.5.0/supabase/_sync/client.py
+-rw-r--r--   0        0        0     1172 2024-05-28 12:17:36.874589 supabase-2.5.0/supabase/client.py
+-rw-r--r--   0        0        0      127 2024-05-28 12:17:36.874589 supabase-2.5.0/supabase/lib/__init__.py
+-rw-r--r--   0        0        0     3135 2024-05-28 12:17:36.874589 supabase-2.5.0/supabase/lib/client_options.py
+-rw-r--r--   0        0        0     1892 2024-05-28 12:17:36.874589 supabase-2.5.0/supabase/lib/realtime_client.py
+-rw-r--r--   0        0        0        0 2024-05-28 12:17:36.874589 supabase-2.5.0/supabase/py.typed
+-rw-r--r--   0        0        0     9313 1970-01-01 00:00:00.000000 supabase-2.5.0/PKG-INFO
```

### Comparing `supabase-2.4.6/LICENSE` & `supabase-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `supabase-2.4.6/README.md` & `supabase-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `supabase-2.4.6/pyproject.toml` & `supabase-2.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "supabase"
-version = "2.4.6"
+version = "2.5.0"
 description = "Supabase client for Python."
 authors = ["Joel Lee <joel@joellee.org>", "Leon Fedden <leonfedden@gmail.com>", "Daniel Reinón García <danielreinon@outlook.com>", "Leynier Gutiérrez González <leynier41@gmail.com>", "Anand", "Andrew Smith <a.smith@silentworks.co.uk>"]
 homepage = "https://github.com/supabase-community/supabase-py"
 repository = "https://github.com/supabase-community/supabase-py"
 documentation = "https://github.com/supabase-community/supabase-py"
 readme = "README.md"
 license = "MIT"
```

### Comparing `supabase-2.4.6/supabase/__init__.py` & `supabase-2.5.0/supabase/__init__.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.6/supabase/_async/auth_client.py` & `supabase-2.5.0/supabase/_async/auth_client.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.6/supabase/_async/client.py` & `supabase-2.5.0/supabase/_async/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,14 @@
         self.options = options
         options.headers.update(self._get_auth_headers())
         self.rest_url = f"{supabase_url}/rest/v1"
         self.realtime_url = f"{supabase_url}/realtime/v1".replace("http", "ws")
         self.auth_url = f"{supabase_url}/auth/v1"
         self.storage_url = f"{supabase_url}/storage/v1"
         self.functions_url = f"{supabase_url}/functions/v1"
-        self.schema = options.schema
 
         # Instantiate clients.
         self.auth = self._init_supabase_auth_client(
             auth_url=self.auth_url,
             client_options=options,
         )
         # TODO: Bring up to parity with JS client.
@@ -106,14 +105,27 @@
 
         Note that the supabase client uses the `from` method, but in Python,
         this is a reserved keyword, so we have elected to use the name `table`.
         Alternatively you can use the `.from_()` method.
         """
         return self.from_(table_name)
 
+    def schema(self, schema: str) -> AsyncPostgrestClient:
+        """Select a schema to query or perform an function (rpc) call.
+
+        The schema needs to be on the list of exposed schemas inside Supabase.
+        """
+        self._postgrest = self._init_postgrest_client(
+            rest_url=self.rest_url,
+            headers=self.options.headers,
+            schema=schema,
+            timeout=self.options.postgrest_client_timeout,
+        )
+        return self._postgrest
+
     def from_(self, table_name: str) -> AsyncRequestBuilder:
         """Perform a table operation.
 
         See the `table` method.
         """
         return self.postgrest.from_(table_name)
```

### Comparing `supabase-2.4.6/supabase/_sync/auth_client.py` & `supabase-2.5.0/supabase/_sync/auth_client.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.6/supabase/_sync/client.py` & `supabase-2.5.0/supabase/_sync/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,14 @@
         self.options = options
         options.headers.update(self._get_auth_headers())
         self.rest_url = f"{supabase_url}/rest/v1"
         self.realtime_url = f"{supabase_url}/realtime/v1".replace("http", "ws")
         self.auth_url = f"{supabase_url}/auth/v1"
         self.storage_url = f"{supabase_url}/storage/v1"
         self.functions_url = f"{supabase_url}/functions/v1"
-        self.schema = options.schema
 
         # Instantiate clients.
         self.auth = self._init_supabase_auth_client(
             auth_url=self.auth_url,
             client_options=options,
         )
         # TODO: Bring up to parity with JS client.
@@ -106,14 +105,27 @@
 
         Note that the supabase client uses the `from` method, but in Python,
         this is a reserved keyword, so we have elected to use the name `table`.
         Alternatively you can use the `.from_()` method.
         """
         return self.from_(table_name)
 
+    def schema(self, schema: str) -> SyncPostgrestClient:
+        """Select a schema to query or perform an function (rpc) call.
+
+        The schema needs to be on the list of exposed schemas inside Supabase.
+        """
+        self._postgrest = self._init_postgrest_client(
+            rest_url=self.rest_url,
+            headers=self.options.headers,
+            schema=schema,
+            timeout=self.options.postgrest_client_timeout,
+        )
+        return self._postgrest
+
     def from_(self, table_name: str) -> SyncRequestBuilder:
         """Perform a table operation.
 
         See the `table` method.
         """
         return self.postgrest.from_(table_name)
```

### Comparing `supabase-2.4.6/supabase/client.py` & `supabase-2.5.0/supabase/client.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.6/supabase/lib/client_options.py` & `supabase-2.5.0/supabase/lib/client_options.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.6/supabase/lib/realtime_client.py` & `supabase-2.5.0/supabase/lib/realtime_client.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.6/PKG-INFO` & `supabase-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supabase
-Version: 2.4.6
+Version: 2.5.0
 Summary: Supabase client for Python.
 Home-page: https://github.com/supabase-community/supabase-py
 License: MIT
 Author: Joel Lee
 Author-email: joel@joellee.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

