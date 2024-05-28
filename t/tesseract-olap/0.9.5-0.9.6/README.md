# Comparing `tmp/tesseract_olap-0.9.5.tar.gz` & `tmp/tesseract_olap-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tesseract_olap-0.9.5.tar", max compression
+gzip compressed data, was "tesseract_olap-0.9.6.tar", max compression
```

## Comparing `tesseract_olap-0.9.5.tar` & `tesseract_olap-0.9.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     2589 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/PACKAGE.md
--rw-r--r--   0        0        0     1320 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/pyproject.toml
--rw-r--r--   0        0        0      562 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/__init__.py
--rw-r--r--   0        0        0      377 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/backend/__init__.py
--rw-r--r--   0        0        0     2707 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/backend/cache.py
--rw-r--r--   0        0        0       79 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/backend/clickhouse/__init__.py
--rw-r--r--   0        0        0     7219 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/backend/clickhouse/backend.py
--rw-r--r--   0        0        0     2714 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/backend/clickhouse/dialect.py
--rw-r--r--   0        0        0    20624 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/backend/clickhouse/sqlbuild.py
--rw-r--r--   0        0        0     3743 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/backend/models.py
--rw-r--r--   0        0        0     2761 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/backend/valkey.py
--rw-r--r--   0        0        0      571 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/common/__init__.py
--rw-r--r--   0        0        0     2461 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/common/strings.py
--rw-r--r--   0        0        0      385 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/common/types.py
--rw-r--r--   0        0        0      787 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/exceptions/__init__.py
--rw-r--r--   0        0        0     1596 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/exceptions/backend.py
--rw-r--r--   0        0        0     3682 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/exceptions/query.py
--rw-r--r--   0        0        0     3712 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/exceptions/schema.py
--rw-r--r--   0        0        0      741 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/exceptions/server.py
--rw-r--r--   0        0        0      511 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/logiclayer/__init__.py
--rw-r--r--   0        0        0    11052 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/logiclayer/dependencies.py
--rw-r--r--   0        0        0     6259 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/logiclayer/module.py
--rw-r--r--   0        0        0     4284 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/logiclayer/response.py
--rw-r--r--   0        0        0     1166 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/query/__init__.py
--rw-r--r--   0        0        0     3318 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/query/enums.py
--rw-r--r--   0        0        0    12543 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/query/models.py
--rw-r--r--   0        0        0    13039 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/query/queries.py
--rw-r--r--   0        0        0    10178 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/query/requests.py
--rw-r--r--   0        0        0     1763 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/schema/__init__.py
--rw-r--r--   0        0        0     5432 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/schema/aggregators.py
--rw-r--r--   0        0        0     3587 2024-05-04 02:06:21.692989 tesseract_olap-0.9.5/tesseract_olap/schema/csv.py
--rw-r--r--   0        0        0     4744 2024-05-04 02:06:21.696989 tesseract_olap-0.9.5/tesseract_olap/schema/enums.py
--rw-r--r--   0        0        0     2542 2024-05-04 02:06:21.696989 tesseract_olap-0.9.5/tesseract_olap/schema/json.py
--rw-r--r--   0        0        0     9796 2024-05-04 02:06:21.696989 tesseract_olap-0.9.5/tesseract_olap/schema/models.py
--rw-r--r--   0        0        0    11992 2024-05-04 02:06:21.696989 tesseract_olap-0.9.5/tesseract_olap/schema/parser.py
--rw-r--r--   0        0        0     5576 2024-05-04 02:06:21.696989 tesseract_olap-0.9.5/tesseract_olap/schema/public.py
--rw-r--r--   0        0        0     4824 2024-05-04 02:06:21.696989 tesseract_olap-0.9.5/tesseract_olap/schema/schema.xsd
--rw-r--r--   0        0        0    23758 2024-05-04 02:06:21.696989 tesseract_olap-0.9.5/tesseract_olap/schema/traverse.py
--rw-r--r--   0        0        0    18520 2024-05-04 02:06:21.696989 tesseract_olap-0.9.5/tesseract_olap/schema/xml.py
--rw-r--r--   0        0        0       64 2024-05-04 02:06:21.696989 tesseract_olap-0.9.5/tesseract_olap/server/__init__.py
--rw-r--r--   0        0        0     4674 2024-05-04 02:06:21.696989 tesseract_olap-0.9.5/tesseract_olap/server/schema.py
--rw-r--r--   0        0        0     3713 2024-05-04 02:06:21.696989 tesseract_olap-0.9.5/tesseract_olap/server/server.py
--rw-r--r--   0        0        0     4003 1970-01-01 00:00:00.000000 tesseract_olap-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0     2589 2024-05-28 17:03:37.368934 tesseract_olap-0.9.6/PACKAGE.md
+-rw-r--r--   0        0        0     1425 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0      650 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/__init__.py
+-rw-r--r--   0        0        0      377 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/backend/__init__.py
+-rw-r--r--   0        0        0     2707 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/backend/cache.py
+-rw-r--r--   0        0        0       79 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/backend/clickhouse/__init__.py
+-rw-r--r--   0        0        0     7298 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/backend/clickhouse/backend.py
+-rw-r--r--   0        0        0     2714 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/backend/clickhouse/dialect.py
+-rw-r--r--   0        0        0    20624 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/backend/clickhouse/sqlbuild.py
+-rw-r--r--   0        0        0     3743 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/backend/models.py
+-rw-r--r--   0        0        0     2611 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/backend/valkey.py
+-rw-r--r--   0        0        0      571 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/common/__init__.py
+-rw-r--r--   0        0        0     2461 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/common/strings.py
+-rw-r--r--   0        0        0      385 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/common/types.py
+-rw-r--r--   0        0        0      787 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/exceptions/__init__.py
+-rw-r--r--   0        0        0     1741 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/exceptions/backend.py
+-rw-r--r--   0        0        0     3660 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/exceptions/query.py
+-rw-r--r--   0        0        0     3949 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/exceptions/schema.py
+-rw-r--r--   0        0        0      741 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/exceptions/server.py
+-rw-r--r--   0        0        0      511 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/logiclayer/__init__.py
+-rw-r--r--   0        0        0    11057 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/logiclayer/dependencies.py
+-rw-r--r--   0        0        0     6463 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/logiclayer/module.py
+-rw-r--r--   0        0        0     4284 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/logiclayer/response.py
+-rw-r--r--   0        0        0     1166 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/query/__init__.py
+-rw-r--r--   0        0        0     3318 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/query/enums.py
+-rw-r--r--   0        0        0    12543 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/query/models.py
+-rw-r--r--   0        0        0    13039 2024-05-28 17:03:37.372933 tesseract_olap-0.9.6/tesseract_olap/query/queries.py
+-rw-r--r--   0        0        0    10178 2024-05-28 17:03:37.376933 tesseract_olap-0.9.6/tesseract_olap/query/requests.py
+-rw-r--r--   0        0        0     1763 2024-05-28 17:03:37.376933 tesseract_olap-0.9.6/tesseract_olap/schema/__init__.py
+-rw-r--r--   0        0        0     5432 2024-05-28 17:03:37.376933 tesseract_olap-0.9.6/tesseract_olap/schema/aggregators.py
+-rw-r--r--   0        0        0     3587 2024-05-28 17:03:37.376933 tesseract_olap-0.9.6/tesseract_olap/schema/csv.py
+-rw-r--r--   0        0        0     4744 2024-05-28 17:03:37.376933 tesseract_olap-0.9.6/tesseract_olap/schema/enums.py
+-rw-r--r--   0        0        0     2542 2024-05-28 17:03:37.376933 tesseract_olap-0.9.6/tesseract_olap/schema/json.py
+-rw-r--r--   0        0        0     9796 2024-05-28 17:03:37.376933 tesseract_olap-0.9.6/tesseract_olap/schema/models.py
+-rw-r--r--   0        0        0    11992 2024-05-28 17:03:37.376933 tesseract_olap-0.9.6/tesseract_olap/schema/parser.py
+-rw-r--r--   0        0        0     5576 2024-05-28 17:03:37.376933 tesseract_olap-0.9.6/tesseract_olap/schema/public.py
+-rw-r--r--   0        0        0     4824 2024-05-28 17:03:37.376933 tesseract_olap-0.9.6/tesseract_olap/schema/schema.xsd
+-rw-r--r--   0        0        0    23758 2024-05-28 17:03:37.376933 tesseract_olap-0.9.6/tesseract_olap/schema/traverse.py
+-rw-r--r--   0        0        0    20861 2024-05-28 17:03:37.376933 tesseract_olap-0.9.6/tesseract_olap/schema/xml.py
+-rw-r--r--   0        0        0       64 2024-05-28 17:03:37.376933 tesseract_olap-0.9.6/tesseract_olap/server/__init__.py
+-rw-r--r--   0        0        0     4674 2024-05-28 17:03:37.376933 tesseract_olap-0.9.6/tesseract_olap/server/schema.py
+-rw-r--r--   0        0        0     3713 2024-05-28 17:03:37.376933 tesseract_olap-0.9.6/tesseract_olap/server/server.py
+-rw-r--r--   0        0        0     4003 1970-01-01 00:00:00.000000 tesseract_olap-0.9.6/PKG-INFO
```

### Comparing `tesseract_olap-0.9.5/PACKAGE.md` & `tesseract_olap-0.9.6/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/backend/cache.py` & `tesseract_olap-0.9.6/tesseract_olap/backend/cache.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/backend/clickhouse/backend.py` & `tesseract_olap-0.9.6/tesseract_olap/backend/clickhouse/backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,19 +92,23 @@
         self.dsn = dsn
 
     def __repr__(self):
         return f"{type(self).__name__}(dsn='{hide_dsn_password(self.dsn)}')"
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         result = super().__exit__(exc_type, exc_val, exc_tb)
+        try:
+            args = getattr(exc_val, "args")
+        except AttributeError:
+            args = tuple()
 
         if exc_type is InterfaceError:
-            raise UpstreamNotPrepared(*exc_val.args).with_traceback(exc_tb)
+            raise UpstreamNotPrepared(*args) from exc_val
         if exc_type is DatabaseError:
-            raise UpstreamInternalError(*exc_val.args).with_traceback(exc_tb)
+            raise UpstreamInternalError(*args) from exc_val
 
         return result
 
     def connect(self):
         self._cache = self.cache.connect()
         self._connection = chdr.connect(dsn=self.dsn, compression="lz4")
```

### Comparing `tesseract_olap-0.9.5/tesseract_olap/backend/clickhouse/dialect.py` & `tesseract_olap-0.9.6/tesseract_olap/backend/clickhouse/dialect.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/backend/clickhouse/sqlbuild.py` & `tesseract_olap-0.9.6/tesseract_olap/backend/clickhouse/sqlbuild.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/backend/models.py` & `tesseract_olap-0.9.6/tesseract_olap/backend/models.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/common/__init__.py` & `tesseract_olap-0.9.6/tesseract_olap/common/__init__.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/common/strings.py` & `tesseract_olap-0.9.6/tesseract_olap/common/strings.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/exceptions/__init__.py` & `tesseract_olap-0.9.6/tesseract_olap/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/exceptions/backend.py` & `tesseract_olap-0.9.6/tesseract_olap/exceptions/backend.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,25 +12,30 @@
     """This error happens when there's a connection attempt done against a
     backend which is unable to accept connections.
 
     The user must avoid race conditions and ensure connections and cursors are
     in usable state.
     """
 
-    def __init__(self) -> None:
+    def __init__(self, *args) -> None:
         super().__init__("The configured Backend isn't ready yet.")
+        self.args = args
 
 
 class UpstreamInternalError(BackendError):
     """This error occurs when a remote server returns a valid response, but the
     contents give details about an internal server error.
 
     This must be caught and reported to the administrator.
     """
 
+    def __init__(self, message: str, *args) -> None:
+        super().__init__(message)
+        self.args = args
+
 
 class UnexpectedResponseError(BackendError):
     """This error occurs when the response sent by the remote server doesn't
     adjust to the expected shape, and the database driver has problems to handle
     it.
 
     This must be caught and logged, but usually is related to a malformed query,
```

### Comparing `tesseract_olap-0.9.5/tesseract_olap/exceptions/query.py` & `tesseract_olap-0.9.6/tesseract_olap/exceptions/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,11 +103,11 @@
     """
 
     code = 403
 
     def __init__(self, resource: str, roles: Iterable[str]) -> None:
         super().__init__(
             f"Requested resource '{resource}' is not allowed for the roles "
-            f"provided by authorization credentials: '{', '.join(roles)}'"
+            f"provided by credentials: '{', '.join(roles)}'"
         )
         self.resource = resource
-        self.request_roles = roles
+        self.roles = roles
```

### Comparing `tesseract_olap-0.9.5/tesseract_olap/exceptions/schema.py` & `tesseract_olap-0.9.6/tesseract_olap/exceptions/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,14 +90,22 @@
         message = (
             "There's a {1} with an invalid name '{2}' in the cube '{0}'. "
             "Entity names can't contain the following characters: , ; :"
         ).format(cube, entity, name)
         super().__init__(message)
 
 
+class DuplicateKeyError(SchemaError):
+    """The key of some property in the schema is shared in two nodes."""
+
+    def __init__(self, key: str) -> None:
+        message = f"Key '{key}' is duplicated"
+        super().__init__(message)
+
+
 class DuplicatedNameError(SchemaError):
     """The name of an Entity is duplicated across its parent cube."""
 
     def __init__(self, cube: str, entity_prev: str, entity: str, name: str):
         message = (
             "In the cube '{0}' a {1} and a {2} share the same name '{3}'. "
             "Names of Measures, Levels and Properties must be unique across its cube."
```

### Comparing `tesseract_olap-0.9.5/tesseract_olap/exceptions/server.py` & `tesseract_olap-0.9.6/tesseract_olap/exceptions/server.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/logiclayer/dependencies.py` & `tesseract_olap-0.9.6/tesseract_olap/logiclayer/dependencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     header_auth: Annotated[Optional[str], Header(alias="authorization")] = None,
     header_jwt: Annotated[Optional[str], Header(alias="x-tesseract-jwt")] = None,
     query_token: Annotated[Optional[str], Query(alias="token")] = None,
 ):
     if header_jwt:
         return AuthToken(AuthTokenType.JWTOKEN, header_jwt)
     if query_token:
-        return AuthToken(AuthTokenType.APIKEY, query_token)
+        return AuthToken(AuthTokenType.SEARCHPARAM, query_token)
     if header_auth:
         if header_auth.startswith("Bearer "):
             return AuthToken(AuthTokenType.JWTOKEN, header_auth[7:])
         if header_auth.startswith("Basic "):
             return AuthToken(AuthTokenType.BASIC, header_auth[6:])
         if header_auth.startswith("Digest "):
             return AuthToken(AuthTokenType.DIGEST, header_auth[7:])
```

### Comparing `tesseract_olap-0.9.5/tesseract_olap/logiclayer/module.py` & `tesseract_olap-0.9.6/tesseract_olap/logiclayer/module.py`

 * *Files 5% similar despite different names*

```diff
@@ -157,17 +157,20 @@
     def exc_tesseracterror(self, request: Request, exc: TesseractError):
         content = {"error": True, "detail": "Backend error"}
 
         if self.debug:
             content["type"] = type(exc).__name__
 
         if isinstance(exc, NotAuthorized):
-            content["detail"] = (
-                exc.message
-                if self.debug
-                else "You don't have authorization to access this resource."
-            )
+            roles = tuple(exc.roles)
+            if len(roles) == 0 or "visitor" in roles:
+                exc.code = 401
+                wall = "The requested resource needs authorization."
+            else:
+                exc.code = 403
+                wall = "You don't have authorization to access this resource."
+            content["detail"] = exc.message if self.debug else wall
 
         elif isinstance(exc, QueryError):
             content["detail"] = exc.message
 
         return JSONResponse(content, status_code=exc.code)
```

### Comparing `tesseract_olap-0.9.5/tesseract_olap/logiclayer/response.py` & `tesseract_olap-0.9.6/tesseract_olap/logiclayer/response.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/query/__init__.py` & `tesseract_olap-0.9.6/tesseract_olap/query/__init__.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/query/enums.py` & `tesseract_olap-0.9.6/tesseract_olap/query/enums.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/query/models.py` & `tesseract_olap-0.9.6/tesseract_olap/query/models.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/query/queries.py` & `tesseract_olap-0.9.6/tesseract_olap/query/queries.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/query/requests.py` & `tesseract_olap-0.9.6/tesseract_olap/query/requests.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/schema/__init__.py` & `tesseract_olap-0.9.6/tesseract_olap/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/schema/aggregators.py` & `tesseract_olap-0.9.6/tesseract_olap/schema/aggregators.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/schema/csv.py` & `tesseract_olap-0.9.6/tesseract_olap/schema/csv.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/schema/enums.py` & `tesseract_olap-0.9.6/tesseract_olap/schema/enums.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/schema/json.py` & `tesseract_olap-0.9.6/tesseract_olap/schema/json.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/schema/models.py` & `tesseract_olap-0.9.6/tesseract_olap/schema/models.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/schema/parser.py` & `tesseract_olap-0.9.6/tesseract_olap/schema/parser.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/schema/public.py` & `tesseract_olap-0.9.6/tesseract_olap/schema/public.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/schema/schema.xsd` & `tesseract_olap-0.9.6/tesseract_olap/schema/schema.xsd`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/schema/traverse.py` & `tesseract_olap-0.9.6/tesseract_olap/schema/traverse.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/schema/xml.py` & `tesseract_olap-0.9.6/tesseract_olap/schema/xml.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,16 +18,17 @@
     TypeVar,
     Union,
 )
 
 import immutables as immu
 from lxml import etree
 
-from tesseract_olap.common import is_numeric, numerify
+from tesseract_olap.common import TRUTHY_STRINGS, T, is_numeric, numerify
 from tesseract_olap.exceptions.schema import (
+    DuplicateKeyError,
     InvalidXMLAttributeValue,
     MissingXMLAttribute,
     MissingXMLNode,
 )
 
 from . import models
 from .aggregators import Aggregator
@@ -48,56 +49,61 @@
     "XMLLevelUsage",
     "XMLPropertyUsage",
     "XMLPrivateDimension",
     "XMLMeasure",
     "XMLCalculatedMeasure",
 ]
 
+AnyXMLDimension = TypeVar(
+    "AnyXMLDimension", bound=Union["XMLSharedDimension", "XMLPrivateDimension"]
+)
 AnyXMLEntity = TypeVar("AnyXMLEntity", bound=XMLEntity)
 
 
 class XMLSchema(models.Schema):
     tag = "Schema"
 
     @classmethod
     def parse(cls, node: etree._Element, index: int = 0):
         """Parse a <Schema> XML node."""
         name = _get_attr(node, "name")
         logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
 
-        cube_gen = _yield_children_nodes(node, XMLCube)
-        shareddim_gen = _yield_children_nodes(node, XMLSharedDimension)
-        sharedtbl_gen = _yield_children_nodes(node, XMLInlineTable)
-
         return cls(
             name=name,
-            cube_map=OrderedDict(cube_gen),
-            shared_dimension_map=immu.Map(shareddim_gen),
-            shared_table_map=immu.Map(sharedtbl_gen),
+            cube_map=OrderedDict(
+                _raise_if_duplicate(_yield_children_nodes(node, XMLCube))
+            ),
+            shared_dimension_map=immu.Map(
+                _raise_if_duplicate(_yield_children_nodes(node, XMLSharedDimension))
+            ),
+            shared_table_map=immu.Map(
+                _raise_if_duplicate(_yield_children_nodes(node, XMLInlineTable))
+            ),
             default_locale=node.get("default_locale", "xx"),
             annotations=immu.Map(_yield_annotations(node)),
         )
 
 
 class XMLAccessControl(models.AccessControl):
     tag = "Access"
 
     @classmethod
     def parse(cls, node: etree._Element):
         """Parse all <Access> XML node that are directly under this node."""
 
-        rules_gen = (
-            (role, _get_attr(item, "rule") == "allow")
-            for item in node.iterchildren(cls.tag)
-            for role in _get_attr(item, "roles").split(",")
-        )
-
         return cls(
-            public=node.get("public", "true") == "true",
-            rules=immu.Map(rules_gen),
+            public=_get_boolean(node, "public", True),
+            rules=immu.Map(
+                _raise_if_duplicate(
+                    (role, _get_attr(item, "rule") == "allow")
+                    for item in node.iterchildren(cls.tag)
+                    for role in _get_attr(item, "roles").split(",")
+                )
+            ),
         )
 
 
 class XMLCube(models.Cube):
     tag = "Cube"
 
     @classmethod
@@ -107,35 +113,41 @@
         logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
 
         table = _find_table_ref(node)
         if table is None:
             raise MissingXMLNode(node.tag, name, "Table")
 
         dimension_map = OrderedDict(
-            _yield_children_nodes(node, XMLPrivateDimension, XMLDimensionUsage)
+            _raise_if_duplicate(
+                _yield_children_nodes(node, XMLPrivateDimension, XMLDimensionUsage)
+            )
         )
         if len(dimension_map) == 0:
             raise MissingXMLNode(node.tag, name, "Dimension")
 
         measure_map = OrderedDict(
-            _yield_children_nodes(node, XMLMeasure, XMLCalculatedMeasure)
+            _raise_if_duplicate(
+                _yield_children_nodes(node, XMLMeasure, XMLCalculatedMeasure)
+            )
         )
         if len(measure_map) == 0:
             raise MissingXMLNode(node.tag, name, "Measure")
 
         return cls(
             name=name,
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            captions=immu.Map(
+                _raise_if_duplicate(_yield_locale_pairs(node, "caption"))
+            ),
             acl=XMLAccessControl.parse(node),
             dimension_map=dimension_map,
             measure_map=measure_map,
             table=table,
             annotations=immu.Map(_yield_annotations(node)),
-            subset_table=node.get("subset_table", "false").lower() != "false",
-            visible=node.get("visible", "true").lower() != "false",
+            subset_table=_get_boolean(node, "subset_table", False),
+            visible=_get_boolean(node, "visible", True),
         )
 
 
 class XMLDimensionUsage(models.DimensionUsage):
     tag = "DimensionUsage"
 
     @classmethod
@@ -145,18 +157,23 @@
         logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
 
         return cls(
             name=name,
             source=_get_attr(node, "source"),
             foreign_key=_get_attr(node, "foreign_key"),
             annotations=immu.Map(_yield_annotations(node)),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            captions=immu.Map(
+                _raise_if_duplicate(_yield_locale_pairs(node, "caption"))
+            ),
             hierarchy_map=OrderedDict(
-                _yield_children_nodes(node, XMLHierarchyUsage, attr="source")
+                _raise_if_duplicate(
+                    _yield_children_nodes(node, XMLHierarchyUsage, attr="source")
+                )
             ),
+            visible=_get_boolean(node, "visible", True),
         )
 
 
 class XMLHierarchyUsage(models.HierarchyUsage):
     tag = "HierarchyUsage"
 
     @classmethod
@@ -165,18 +182,23 @@
         name = _get_attr(node, "name")
         logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
 
         return cls(
             name=name,
             source=_get_attr(node, "source"),
             annotations=immu.Map(_yield_annotations(node)),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            captions=immu.Map(
+                _raise_if_duplicate(_yield_locale_pairs(node, "caption"))
+            ),
             level_map=OrderedDict(
-                _yield_children_nodes(node, XMLLevelUsage, attr="source")
+                _raise_if_duplicate(
+                    _yield_children_nodes(node, XMLLevelUsage, attr="source")
+                )
             ),
+            visible=_get_boolean(node, "visible", True),
         )
 
 
 class XMLLevelUsage(models.LevelUsage):
     tag = "LevelUsage"
 
     @classmethod
@@ -185,18 +207,23 @@
         name = _get_attr(node, "name")
         logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
 
         return cls(
             name=name,
             source=_get_attr(node, "source"),
             annotations=immu.Map(_yield_annotations(node)),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            captions=immu.Map(
+                _raise_if_duplicate(_yield_locale_pairs(node, "caption"))
+            ),
             property_map=OrderedDict(
-                _yield_children_nodes(node, XMLPropertyUsage, attr="source")
+                _raise_if_duplicate(
+                    _yield_children_nodes(node, XMLPropertyUsage, attr="source")
+                )
             ),
+            visible=_get_boolean(node, "visible", True),
         )
 
 
 class XMLPropertyUsage(models.PropertyUsage):
     tag = "PropertyUsage"
 
     @classmethod
@@ -205,15 +232,18 @@
         name = _get_attr(node, "name")
         logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
 
         return cls(
             name=name,
             source=_get_attr(node, "source"),
             annotations=immu.Map(_yield_annotations(node)),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            captions=immu.Map(
+                _raise_if_duplicate(_yield_locale_pairs(node, "caption"))
+            ),
+            visible=_get_boolean(node, "visible", True),
         )
 
 
 class XMLTable(models.Table):
     tag = "Table"
 
     @classmethod
@@ -282,49 +312,56 @@
         # at least 2 rows must be present: a header list and a data row
         if len(children) < 2:
             raise MissingXMLNode(node.tag, _get_attr(node, "name"), "Row")
         headers = tuple(str(item) for item in children[0])
         return headers, children[1:]
 
 
-class XMLSharedDimension(models.Dimension):
-    tag = "SharedDimension"
+class XMLDimension(models.Dimension):
+    tag = "Dimension"
 
     @classmethod
     def parse(cls, node: etree._Element, index: int):
-        """Parse a Shared <Dimension> XML node."""
+        """Parse a <Dimension> XML node."""
         name = _get_attr(node, "name")
         logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
 
         dim_type = node.get("type")
 
-        hierarchy_map = OrderedDict(_yield_children_nodes(node, XMLHierarchy))
+        hierarchy_map = OrderedDict(
+            _raise_if_duplicate(_yield_children_nodes(node, XMLHierarchy))
+        )
 
         default_hierarchy = node.get("default_hierarchy")
         if default_hierarchy not in hierarchy_map:
             default_hierarchy = next(iter(hierarchy_map.keys()))
 
         return cls(
             name=name,
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            captions=immu.Map(
+                _raise_if_duplicate(_yield_locale_pairs(node, "caption"))
+            ),
             default_hierarchy=default_hierarchy,
             dim_type=DimensionType.from_str(dim_type),
             foreign_key=node.get("foreign_key"),
             hierarchy_map=hierarchy_map,
             annotations=immu.Map(_yield_annotations(node)),
+            visible=_get_boolean(node, "visible", True),
         )
 
 
-class XMLPrivateDimension(models.Dimension):
-    tag = "Dimension"
+class XMLSharedDimension(XMLDimension):
+    tag = "SharedDimension"
+
 
+class XMLPrivateDimension(XMLDimension):
     @classmethod
     def parse(cls, node: etree._Element, index: int):
         """Parse a Private <Dimension> XML node."""
-        dimension: cls = XMLSharedDimension.parse.__func__(cls, node, index)
+        dimension = super().parse(node, index)
 
         # foreign keys are required in Private Dimensions
         if dimension.foreign_key is None:
             raise MissingXMLAttribute(node.tag, "foreign_key")
 
         return dimension
 
@@ -334,30 +371,35 @@
 
     @classmethod
     def parse(cls, node: etree._Element, index: int):
         """Parse a <Hierarchy> XML node."""
         name = _get_attr(node, "name")
         logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
 
-        level_map = OrderedDict(_yield_children_nodes(node, XMLLevel))
+        level_map = OrderedDict(
+            _raise_if_duplicate(_yield_children_nodes(node, XMLLevel))
+        )
         if len(level_map) == 0:
             raise MissingXMLNode(node.tag, name, "Level")
 
         default_pk = ""
         for item in level_map.values():
             default_pk = item.key_column
 
         return cls(
             name=name,
             primary_key=node.get("primary_key", default_pk),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            captions=immu.Map(
+                _raise_if_duplicate(_yield_locale_pairs(node, "caption"))
+            ),
             table=_find_table_ref(node),
             level_map=level_map,
             default_member=cls._parse_default_member(node),
             annotations=immu.Map(_yield_annotations(node)),
+            visible=_get_boolean(node, "visible", True),
         )
 
     @staticmethod
     def _parse_default_member(node: etree._Element):
         items: List[str] = node.get("default_member", "").split(".", maxsplit=1)
         return (items[0], items[1]) if len(items) == 2 else None
 
@@ -374,42 +416,54 @@
         key_type = node.get("key_type")
 
         return cls(
             name=name,
             depth=index + 1,
             key_column=_get_attr(node, "key_column"),
             key_type=MemberType.from_str(key_type),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-            name_column_map=immu.Map(_yield_locale_pairs(node, "name_column")),
-            property_map=OrderedDict(_yield_children_nodes(node, XMLProperty)),
+            captions=immu.Map(
+                _raise_if_duplicate(_yield_locale_pairs(node, "caption"))
+            ),
+            name_column_map=immu.Map(
+                _raise_if_duplicate(_yield_locale_pairs(node, "name_column"))
+            ),
+            property_map=OrderedDict(
+                _raise_if_duplicate(_yield_children_nodes(node, XMLProperty))
+            ),
             annotations=immu.Map(_yield_annotations(node)),
+            visible=_get_boolean(node, "visible", True),
         )
 
 
 class XMLProperty(models.Property):
     tag = "Property"
 
     @classmethod
     def parse(cls, node: etree._Element, index: int):
         """Parse a <Property> XML node."""
         name = _get_attr(node, "name")
         logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
 
         key_type = node.get("key_type")
 
-        keycol_map = immu.Map(_yield_locale_pairs(node, "key_column"))
+        keycol_map = immu.Map(
+            _raise_if_duplicate(_yield_locale_pairs(node, "key_column"))
+        )
         if len(keycol_map) == 0:
             raise MissingXMLAttribute(node.tag, "key_column")
 
         return cls(
             name=name,
             annotations=immu.Map(_yield_annotations(node)),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            captions=immu.Map(
+                _raise_if_duplicate(_yield_locale_pairs(node, "caption"))
+            ),
             key_column_map=keycol_map,
             key_type=MemberType.from_str(key_type),
+            visible=_get_boolean(node, "visible", True),
         )
 
 
 class XMLMeasure(models.Measure):
     tag = "Measure"
 
     @classmethod
@@ -419,16 +473,19 @@
         logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
 
         return cls(
             name=name,
             key_column=_get_attr(node, "key_column"),
             aggregator=cls._get_aggregator(node),
             annotations=immu.Map(_yield_annotations(node)),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
-            submeasures=immu.Map(_yield_children_nodes(node, cls)),
+            captions=immu.Map(
+                _raise_if_duplicate(_yield_locale_pairs(node, "caption"))
+            ),
+            submeasures=immu.Map(_raise_if_duplicate(_yield_children_nodes(node, cls))),
+            visible=_get_boolean(node, "visible", True),
         )
 
     @staticmethod
     def _get_aggregator(mea_node: etree._Element) -> Aggregator:
         """
         Raises:
             :class:`MissingXMLAttribute` --
@@ -439,15 +496,17 @@
                 If the aggregator defined for this node has an unexpected value.
         """
 
         agg_node = mea_node.find("Aggregation")
 
         # if there's an <Aggregation> node, get its `type`
         # else get the `<Measure>`'s `aggregator` attribute
-        node, attr = (mea_node, "aggregator") if agg_node is None else (agg_node, "type")
+        node, attr = (
+            (mea_node, "aggregator") if agg_node is None else (agg_node, "type")
+        )
         value = _get_attr(node, attr)
 
         try:
             agg_type = AggregatorType.from_str(value)
         except ValueError:
             node_name = _get_attr(mea_node, "name")
             raise InvalidXMLAttributeValue(node.tag, node_name, attr, value)
@@ -469,20 +528,25 @@
         name = _get_attr(node, "name")
         logger.debug("Parsing node <%s name='%s' />", cls.tag, name)
 
         return cls(
             name=name,
             formula=cls._parse_formula(_get_attr(node, "formula")),
             annotations=immu.Map(_yield_annotations(node)),
-            captions=immu.Map(_yield_locale_pairs(node, "caption")),
+            captions=immu.Map(
+                _raise_if_duplicate(_yield_locale_pairs(node, "caption"))
+            ),
+            visible=_get_boolean(node, "visible", True),
         )
 
 
 def _find_table_ref(node: etree._Element):
-    gen_tables = (item for item in node.iterchildren("InlineTable", "Table", "TableUsage"))
+    gen_tables = (
+        item for item in node.iterchildren("InlineTable", "Table", "TableUsage")
+    )
     table_node = next(gen_tables, None)
 
     if table_node is None:
         return None
     elif table_node.tag == "InlineTable":
         return XMLInlineTable.parse(table_node, 0)
     elif table_node.tag == "Table":
@@ -502,19 +566,35 @@
         value = node.attrib[attr]
     except KeyError as exc:
         raise MissingXMLAttribute(node.tag, attr) from exc
     else:
         return str(value)
 
 
+def _get_boolean(node: etree._Element, attr: str, default: bool) -> bool:
+    value = node.get(attr)
+    return default if value is None else (value.lower() in TRUTHY_STRINGS)
+
+
+def _raise_if_duplicate(
+    generator: Iterable[Tuple[str, T]],
+    exc_cls: Type[DuplicateKeyError] = DuplicateKeyError,
+):
+    seen_keys = set()
+    for key, value in generator:
+        if key in seen_keys:
+            raise exc_cls(key)
+        seen_keys.add(key)
+        yield key, value
+
+
 def _yield_annotations(node: etree._Element) -> Iterable[Tuple[str, Optional[str]]]:
     """Yields a pair of (name, value) for each Annotation in the node."""
-    return (
-        (_get_attr(item, "name"), item.text)
-        for item in node.iterchildren("Annotation")
+    return _raise_if_duplicate(
+        (_get_attr(item, "name"), item.text) for item in node.iterchildren("Annotation")
     )
 
 
 def _yield_children_nodes(
     node: etree._Element,
     *children: Type[AnyXMLEntity],
     attr: str = "name",
@@ -522,16 +602,17 @@
     tags = (item.tag for item in children)
     parsers = {item.tag: item.parse for item in children}
     for index, item in enumerate(node.iterchildren(*tags)):
         reducer = parsers[item.tag]
         yield _get_attr(item, attr), reducer(item, index)
 
 
-def _yield_locale_pairs(node: etree._Element,
-                        attribute: str) -> Generator[Tuple[str, str], None, None]:
+def _yield_locale_pairs(
+    node: etree._Element, attribute: str
+) -> Generator[Tuple[str, str], None, None]:
     attr_value = node.get(attribute)
     if attr_value is not None:
         yield ("xx", attr_value)
 
     for child_node in node.iterchildren("LocalizedAttr"):
         child_attr = _get_attr(child_node, "attr")
         if child_attr != attribute:
@@ -546,17 +627,17 @@
     """Attempts to parse an object into a XMLSchema.
 
     This function accepts:
     - A raw XML :class:`str`
     - A local path (as a :class:`pathlib.Path`) to a XML file
     - A not-binary read-only :class:`TextIO` instance for a file-like object
     """
-    parser = etree.XMLParser(encoding="utf-8",
-                             remove_blank_text=True,
-                             remove_comments=True)
+    parser = etree.XMLParser(
+        encoding="utf-8", remove_blank_text=True, remove_comments=True
+    )
 
     # if argument is str, is assumed to be a raw XML string
     if isinstance(source, str):
         root = etree.fromstring(source, parser)
         return XMLSchema.parse(root)
 
     # if argument is pathlib.Path or TextIO, open it and parse contents
```

### Comparing `tesseract_olap-0.9.5/tesseract_olap/server/schema.py` & `tesseract_olap-0.9.6/tesseract_olap/server/schema.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/tesseract_olap/server/server.py` & `tesseract_olap-0.9.6/tesseract_olap/server/server.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.9.5/PKG-INFO` & `tesseract_olap-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tesseract-olap
-Version: 0.9.5
+Version: 0.9.6
 Summary: A simple OLAP library.
 Home-page: https://github.com/Datawheel/tesseract-python
 License: MIT
 Author: Francisco Abarzua
 Author-email: francisco@datawheel.us
 Maintainer: Francisco Abarzua
 Maintainer-email: francisco@datawheel.us
```

