# Comparing `tmp/openeo_fastapi-2024.4.2.tar.gz` & `tmp/openeo_fastapi-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openeo_fastapi-2024.4.2.tar", max compression
+gzip compressed data, was "openeo_fastapi-2024.5.1.tar", max compression
```

## Comparing `openeo_fastapi-2024.4.2.tar` & `openeo_fastapi-2024.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11358 2024-04-08 12:15:36.919231 openeo_fastapi-2024.4.2/LICENSE
--rw-r--r--   0        0        0     2191 2024-04-08 12:15:36.919231 openeo_fastapi-2024.4.2/README.md
--rw-r--r--   0        0        0        0 2024-04-08 12:15:36.923231 openeo_fastapi-2024.4.2/openeo_fastapi/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 12:15:36.923231 openeo_fastapi-2024.4.2/openeo_fastapi/api/__init__.py
--rw-r--r--   0        0        0    19123 2024-04-08 12:15:36.923231 openeo_fastapi-2024.4.2/openeo_fastapi/api/app.py
--rw-r--r--   0        0        0    21803 2024-04-08 12:15:36.923231 openeo_fastapi-2024.4.2/openeo_fastapi/api/models.py
--rw-r--r--   0        0        0    18134 2024-04-08 12:15:36.923231 openeo_fastapi-2024.4.2/openeo_fastapi/api/types.py
--rw-r--r--   0        0        0     1778 2024-04-08 12:15:36.923231 openeo_fastapi-2024.4.2/openeo_fastapi/cli.py
--rw-r--r--   0        0        0        0 2024-04-08 12:15:36.923231 openeo_fastapi-2024.4.2/openeo_fastapi/client/__init__.py
--rw-r--r--   0        0        0     7732 2024-04-08 12:15:36.923231 openeo_fastapi-2024.4.2/openeo_fastapi/client/auth.py
--rw-r--r--   0        0        0     6469 2024-04-08 12:15:36.923231 openeo_fastapi-2024.4.2/openeo_fastapi/client/collections.py
--rw-r--r--   0        0        0     6361 2024-04-08 12:15:36.923231 openeo_fastapi-2024.4.2/openeo_fastapi/client/core.py
--rw-r--r--   0        0        0     3408 2024-04-08 12:15:36.923231 openeo_fastapi-2024.4.2/openeo_fastapi/client/files.py
--rw-r--r--   0        0        0    13680 2024-04-08 12:15:36.923231 openeo_fastapi-2024.4.2/openeo_fastapi/client/jobs.py
--rw-r--r--   0        0        0    11239 2024-04-08 12:15:36.923231 openeo_fastapi-2024.4.2/openeo_fastapi/client/processes.py
--rw-r--r--   0        0        0        0 2024-04-08 12:15:36.923231 openeo_fastapi-2024.4.2/openeo_fastapi/client/psql/__init__.py
--rw-r--r--   0        0        0     5077 2024-04-08 12:15:36.923231 openeo_fastapi-2024.4.2/openeo_fastapi/client/psql/engine.py
--rw-r--r--   0        0        0     2493 2024-04-08 12:15:36.923231 openeo_fastapi-2024.4.2/openeo_fastapi/client/psql/models.py
--rw-r--r--   0        0        0      828 2024-04-08 12:15:36.923231 openeo_fastapi-2024.4.2/openeo_fastapi/client/psql/settings.py
--rw-r--r--   0        0        0      737 2024-04-08 12:15:36.923231 openeo_fastapi-2024.4.2/openeo_fastapi/client/register.py
--rw-r--r--   0        0        0     2257 2024-04-08 12:15:36.923231 openeo_fastapi-2024.4.2/openeo_fastapi/client/settings.py
--rw-r--r--   0        0        0     1426 2024-04-08 12:15:36.923231 openeo_fastapi-2024.4.2/openeo_fastapi/templates.py
--rw-r--r--   0        0        0     1525 2024-04-08 12:15:36.923231 openeo_fastapi-2024.4.2/pyproject.toml
--rw-r--r--   0        0        0     3738 1970-01-01 00:00:00.000000 openeo_fastapi-2024.4.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/LICENSE
+-rw-r--r--   0        0        0     2191 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/api/__init__.py
+-rw-r--r--   0        0        0    19273 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/api/app.py
+-rw-r--r--   0        0        0    21803 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/api/models.py
+-rw-r--r--   0        0        0    18134 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/api/types.py
+-rw-r--r--   0        0        0     1778 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/cli.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/client/__init__.py
+-rw-r--r--   0        0        0     7848 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/client/auth.py
+-rw-r--r--   0        0        0     6469 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/client/collections.py
+-rw-r--r--   0        0        0     6260 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/client/core.py
+-rw-r--r--   0        0        0     3408 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/client/files.py
+-rw-r--r--   0        0        0    13680 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/client/jobs.py
+-rw-r--r--   0        0        0    11239 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/client/processes.py
+-rw-r--r--   0        0        0        0 2024-05-28 09:57:54.465145 openeo_fastapi-2024.5.1/openeo_fastapi/client/psql/__init__.py
+-rw-r--r--   0        0        0     5077 2024-05-28 09:57:54.469145 openeo_fastapi-2024.5.1/openeo_fastapi/client/psql/engine.py
+-rw-r--r--   0        0        0     2493 2024-05-28 09:57:54.469145 openeo_fastapi-2024.5.1/openeo_fastapi/client/psql/models.py
+-rw-r--r--   0        0        0      828 2024-05-28 09:57:54.469145 openeo_fastapi-2024.5.1/openeo_fastapi/client/psql/settings.py
+-rw-r--r--   0        0        0      737 2024-05-28 09:57:54.469145 openeo_fastapi-2024.5.1/openeo_fastapi/client/register.py
+-rw-r--r--   0        0        0     2257 2024-05-28 09:57:54.469145 openeo_fastapi-2024.5.1/openeo_fastapi/client/settings.py
+-rw-r--r--   0        0        0     1426 2024-05-28 09:57:54.469145 openeo_fastapi-2024.5.1/openeo_fastapi/templates.py
+-rw-r--r--   0        0        0     1388 2024-05-28 09:57:54.469145 openeo_fastapi-2024.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 openeo_fastapi-2024.5.1/PKG-INFO
```

### Comparing `openeo_fastapi-2024.4.2/LICENSE` & `openeo_fastapi-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.4.2/README.md` & `openeo_fastapi-2024.5.1/README.md`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.4.2/openeo_fastapi/api/app.py` & `openeo_fastapi-2024.5.1/openeo_fastapi/api/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 """OpenEO Api class for preparing the FastApi object from the client that is provided by the user.
 """
 import attr
-from fastapi import APIRouter, HTTPException, Response
+from fastapi import APIRouter, Depends, HTTPException, Response
 from starlette.responses import JSONResponse
 
 from openeo_fastapi.api import models
+from openeo_fastapi.client.auth import Authenticator
 
 HIDDEN_PATHS = ["/openapi.json", "/docs", "/docs/oauth2-redirect", "/redoc"]
 
+
 @attr.define
 class OpenEOApi:
     """Factory for creating FastApi applications conformant to the OpenEO Api specification."""
 
     client: attr.field
     app: attr.field
     router: APIRouter = attr.ib(default=attr.Factory(APIRouter))
     response_class: type[Response] = attr.ib(default=JSONResponse)
 
+    def override_authentication(self, func):
+        self.app.dependency_overrides[Authenticator.validate] = func
+
     def register_well_known(self):
-        """Register well known endpoint (GET /.well-known/openeo).
-        """
+        """Register well known endpoint (GET /.well-known/openeo)."""
         self.router.add_api_route(
             name=".well-known",
             path="/.well-known/openeo",
             response_model=models.WellKnownOpeneoGetResponse,
             response_model_exclude_unset=False,
             response_model_exclude_none=True,
             methods=["GET"],
@@ -406,15 +410,15 @@
             response_model_exclude_none=True,
             methods=["DELETE"],
             endpoint=self.client.files.delete_file,
         )
 
     def register_core(self):
         """
-            Add application logic to the API layer.
+        Add application logic to the API layer.
         """
         self.register_get_conformance()
         self.register_get_health()
         self.register_get_user_info()
         self.register_run_sync_job()
         self.register_get_udf_runtimes()
         self.register_validate_user_process_graph()
@@ -442,31 +446,32 @@
         self.register_download_file()
         self.register_upload_file()
         self.register_delete_file()
         self.register_well_known()
 
     def http_exception_handler(self, request, exception):
         """
-            Register exception handler to turn python exceptions into expected OpenEO error output.
+        Register exception handler to turn python exceptions into expected OpenEO error output.
         """
-        
+
         exception_headers = {
             "allow_origin": "*",
             "allow_credentials": "true",
             "allow_methods": "*",
         }
         from fastapi.encoders import jsonable_encoder
+
         return JSONResponse(
             headers=exception_headers,
             status_code=exception.status_code,
             content=jsonable_encoder(exception.detail),
         )
 
     def __attrs_post_init__(self):
         """
-            Post-init hook responsible for setting up the application upon instantiation of the class.
+        Post-init hook responsible for setting up the application upon instantiation of the class.
         """
         # Register core endpoints
         self.register_core()
         self.register_get_capabilities()
         self.app.include_router(router=self.router)
         self.app.add_exception_handler(HTTPException, self.http_exception_handler)
```

### Comparing `openeo_fastapi-2024.4.2/openeo_fastapi/api/models.py` & `openeo_fastapi-2024.5.1/openeo_fastapi/api/models.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.4.2/openeo_fastapi/api/types.py` & `openeo_fastapi-2024.5.1/openeo_fastapi/api/types.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.4.2/openeo_fastapi/cli.py` & `openeo_fastapi-2024.5.1/openeo_fastapi/cli.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.4.2/openeo_fastapi/client/auth.py` & `openeo_fastapi-2024.5.1/openeo_fastapi/client/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,30 +29,31 @@
     """Pydantic model manipulating users."""
 
     user_id: uuid.UUID
     oidc_sub: str
     created_at: datetime.datetime = datetime.datetime.utcnow()
 
     class Config:
-        """Pydantic model class config."""    
+        """Pydantic model class config."""
+
         orm_mode = True
         arbitrary_types_allowed = True
         extra = "ignore"
 
     @classmethod
     def get_orm(cls):
         """Get the ORM model for this pydantic model."""
         return UserORM
 
 
 # TODO Might make more sense to merge with IssueHandler class.
 # TODO The validate function needs to be easier to overwrite and inject into the OpenEO Core client.
 class Authenticator(ABC):
-    """Basic class to hold the validation call to be used by the api endpoints requiring authentication.
-    """
+    """Basic class to hold the validation call to be used by the api endpoints requiring authentication."""
+
     # Authenticator validate method needs to know what decisions to make based on user info response from the issuer handler.
     # This will be different for different backends, so just put it as ABC for now. We might be able to define this if we want
     # to specify an auth config when initialising the backend.
     @abstractmethod
     def validate(authorization: str = Header()):
         """Validate the authorisation header and create a new user. This method can be overwritten as needed.
 
@@ -78,15 +79,14 @@
 
         if found_user:
             return found_user
 
         user = User(user_id=uuid.uuid4(), oidc_sub=user_info["sub"])
 
         create(create_object=user)
-            
         return user
 
 
 class AuthMethod(Enum):
     """Enum defining known auth methods."""
 
     BASIC = "basic"
@@ -182,24 +182,29 @@
         """
 
         issuer_oidc_config = self._get_issuer_config()
 
         if issuer_oidc_config.status_code != 200:
             raise HTTPException(
                 status_code=500,
-                detail=Error(code="InvalidIssuerConfig", message=f"The issuer config is not available. Tokens cannot be validated currently. Try again later."),
+                detail=Error(
+                    code="InvalidIssuerConfig",
+                    message=f"The issuer config is not available. Tokens cannot be validated currently. Try again later.",
+                ),
             )
 
         userinfo_url = issuer_oidc_config.json()[OIDC_USERINFO]
         resp = self._get_user_info(userinfo_url, token)
 
         if resp.status_code != 200:
             raise HTTPException(
                 status_code=500,
-                detail=Error(code="TokenInvalid", message=f"The provided token is not valid."),
+                detail=Error(
+                    code="TokenInvalid", message=f"The provided token is not valid."
+                ),
             )
 
         return resp.json()
 
     def validate_token(self, token: str):
         """Try to validate the token against the give OIDC provider.
 
@@ -213,12 +218,15 @@
             The JSON as dictionary from _validate_oidc_token.
         """
         # TODO Handle validation exceptions
         parsed_token = AuthToken.from_token(token)
 
         if parsed_token.method.value == AuthMethod.OIDC.value:
             return self._validate_oidc_token(parsed_token.token)
-        
+
         raise HTTPException(
             status_code=500,
-            detail=Error(code="TokenCantBeValidated", message=f"The provided token cannot be validated."),
+            detail=Error(
+                code="TokenCantBeValidated",
+                message=f"The provided token cannot be validated.",
+            ),
         )
```

### Comparing `openeo_fastapi-2024.4.2/openeo_fastapi/client/collections.py` & `openeo_fastapi-2024.5.1/openeo_fastapi/client/collections.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.4.2/openeo_fastapi/client/core.py` & `openeo_fastapi-2024.5.1/openeo_fastapi/client/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,18 @@
 from fastapi import Depends, HTTPException, Response
 
 from openeo_fastapi.api.models import (
     Capabilities,
     ConformanceGetResponse,
     FileFormatsGetResponse,
     MeGetResponse,
+    UdfRuntimesGetResponse,
     WellKnownOpeneoGetResponse,
-    UdfRuntimesGetResponse
-)
-from openeo_fastapi.api.types import (
-    Error,
-    STACConformanceClasses,
-    Version,
 )
+from openeo_fastapi.api.types import Error, STACConformanceClasses, Version
 from openeo_fastapi.client.auth import Authenticator, User
 from openeo_fastapi.client.collections import CollectionRegister
 from openeo_fastapi.client.files import FilesRegister
 from openeo_fastapi.client.jobs import JobsRegister
 from openeo_fastapi.client.processes import ProcessRegister
 from openeo_fastapi.client.settings import AppSettings
 
@@ -46,26 +42,25 @@
 
     collections: Optional[CollectionRegister] = None
     files: Optional[FilesRegister] = None
     jobs: Optional[JobsRegister] = None
     processes: Optional[ProcessRegister] = None
 
     def __attrs_post_init__(self):
-        """Post init hook to set the client registers, if none where provided by the user set to the defaults!
-        """
+        """Post init hook to set the client registers, if none where provided by the user set to the defaults!"""
         self.settings = AppSettings()
-        
+
         self.collections = self.collections or CollectionRegister(self.settings)
         self.files = self.files or FilesRegister(self.settings, self.links)
         self.jobs = self.jobs or JobsRegister(self.settings, self.links)
         self.processes = self.processes or ProcessRegister(self.links)
 
     def _combine_endpoints(self):
         """For the various registers that hold endpoint functions, concat those endpoints to register in get_capabilities.
-        
+
         Returns:
             List: A list of all the endpoints that will be supported by this api deployment.
         """
         registers = [self.collections, self.files, self.jobs, self.processes]
 
         endpoints = []
         for register in registers:
@@ -96,18 +91,18 @@
 
         Returns:
             ConformanceGetResponse: The conformance classes that this Api wil of the api based off what the user provided.
         """
         return ConformanceGetResponse(
             conformsTo=[
                 STACConformanceClasses.CORE.value,
-                STACConformanceClasses.COLLECTIONS.value
+                STACConformanceClasses.COLLECTIONS.value,
             ]
         )
-        
+
     def get_file_formats(self) -> FileFormatsGetResponse:
         """Get the supported file formats for processing input and output.
 
         Returns:
             FileFormatsGetResponse: The response defining the input and output formats.
         """
         return FileFormatsGetResponse(
@@ -127,21 +122,21 @@
         self, user: User = Depends(Authenticator.validate)
     ) -> MeGetResponse:
         """Get the supported file formats for processing input and output.
 
         Returns:
             MeGetResponse: The user information for the validated user.
         """
-        return MeGetResponse(user_id=user.user_id.__str__())
-    
+        return MeGetResponse(user_id=user.user_id)
+
     def get_well_known(self) -> WellKnownOpeneoGetResponse:
         """Get the supported file formats for processing input and output.
 
         Returns:
-            WellKnownOpeneoGetResponse: The api/s which are exposed at this server. 
+            WellKnownOpeneoGetResponse: The api/s which are exposed at this server.
         """
         prefix = "https" if self.settings.API_TLS else "http"
 
         Components = namedtuple(
             typename="Components",
             field_names=["scheme", "netloc", "url", "path", "query", "fragment"],
         )
@@ -167,17 +162,15 @@
         )
 
     def get_udf_runtimes(self) -> UdfRuntimesGetResponse:
         """Get the supported file formats for processing input and output.
 
         Raises:
             HTTPException: Raises an exception with relevant status code and descriptive message of failure.
-        
+
         Returns:
             UdfRuntimesGetResponse: The metadata for the requested BatchJob.
         """
         raise HTTPException(
             status_code=501,
-            detail=Error(
-                code="FeatureUnsupported", message="Feature not supported."
-            ),
+            detail=Error(code="FeatureUnsupported", message="Feature not supported."),
         )
```

### Comparing `openeo_fastapi-2024.4.2/openeo_fastapi/client/files.py` & `openeo_fastapi-2024.5.1/openeo_fastapi/client/files.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.4.2/openeo_fastapi/client/jobs.py` & `openeo_fastapi-2024.5.1/openeo_fastapi/client/jobs.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.4.2/openeo_fastapi/client/processes.py` & `openeo_fastapi-2024.5.1/openeo_fastapi/client/processes.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.4.2/openeo_fastapi/client/psql/engine.py` & `openeo_fastapi-2024.5.1/openeo_fastapi/client/psql/engine.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.4.2/openeo_fastapi/client/psql/models.py` & `openeo_fastapi-2024.5.1/openeo_fastapi/client/psql/models.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.4.2/openeo_fastapi/client/psql/settings.py` & `openeo_fastapi-2024.5.1/openeo_fastapi/client/psql/settings.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.4.2/openeo_fastapi/client/register.py` & `openeo_fastapi-2024.5.1/openeo_fastapi/client/register.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.4.2/openeo_fastapi/client/settings.py` & `openeo_fastapi-2024.5.1/openeo_fastapi/client/settings.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.4.2/openeo_fastapi/templates.py` & `openeo_fastapi-2024.5.1/openeo_fastapi/templates.py`

 * *Files identical despite different names*

### Comparing `openeo_fastapi-2024.4.2/pyproject.toml` & `openeo_fastapi-2024.5.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openeo-fastapi"
-version = "2024.4.2"
+version = "2024.5.1"
 description = "FastApi implementation conforming to the OpenEO Api specification."
 authors = ["Sean Hoyal <sean.hoyal@external.eodc.eu>"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
@@ -13,47 +13,41 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
+pip = "^23.3.2"
+alembic = "^1.13.1"
+uvicorn = "^0.29.0"
 fastapi = "^0.95.1"
 pydantic = "<2"
 attrs = "^23.1.0"
 httpx = "^0.24.1"
 aiohttp = ">3.9"
 pystac-client = ">=0.7.5"
 openeo-pg-parser-networkx = ">=2024.1.1"
 openeo-processes-dask = ">=2023.11.6"
-odc-stac = ">=0.3.8"
-dask-geopandas = ">=0.3.1"
-rioxarray = ">=0.15.0"
-xvec = ">=0.2.0"
 joblib = ">=1.3.2"
-planetary_computer = ">=1.0.0"
-stackstac = ">=0.5.0"
-stac-validator = ">=3.3.2"
-pip = "^23.3.2"
 requests = "^2.31.0"
 SQLAlchemy = "^2.0.27"
+fsspec = "^2024.3.1"
 psycopg2-binary = "^2.9.5"
-alembic = "^1.13.1"
 click = "8.1.7"
-poetry = "1.8.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 ipykernel = "^6.15.1"
 pre-commit = "^2.20.0"
 pytest-cov = "^4.0.0"
 pytest-asyncio = "^0.23.0"
 aioresponses = "^0.7.5"
-pytest-postgresql = ">=4.1.1"
-sphinx = "7.2.6"
+pytest-postgresql= ">=4.1.1"
+pydoc-markdown = "4.8.2"
 
 [tool.poetry.scripts]
 openeo_fastapi = "openeo_fastapi.cli:cli"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openeo_fastapi-2024.4.2/PKG-INFO` & `openeo_fastapi-2024.5.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openeo-fastapi
-Version: 2024.4.2
+Version: 2024.5.1
 Summary: FastApi implementation conforming to the OpenEO Api specification.
 Author: Sean Hoyal
 Author-email: sean.hoyal@external.eodc.eu
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
@@ -14,32 +14,26 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: SQLAlchemy (>=2.0.27,<3.0.0)
 Requires-Dist: aiohttp (>3.9)
 Requires-Dist: alembic (>=1.13.1,<2.0.0)
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
 Requires-Dist: click (==8.1.7)
-Requires-Dist: dask-geopandas (>=0.3.1)
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
+Requires-Dist: fsspec (>=2024.3.1,<2025.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: joblib (>=1.3.2)
-Requires-Dist: odc-stac (>=0.3.8)
 Requires-Dist: openeo-pg-parser-networkx (>=2024.1.1)
 Requires-Dist: openeo-processes-dask (>=2023.11.6)
 Requires-Dist: pip (>=23.3.2,<24.0.0)
-Requires-Dist: planetary_computer (>=1.0.0)
-Requires-Dist: poetry (==1.8.2)
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
 Requires-Dist: pydantic (<2)
 Requires-Dist: pystac-client (>=0.7.5)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: rioxarray (>=0.15.0)
-Requires-Dist: stac-validator (>=3.3.2)
-Requires-Dist: stackstac (>=0.5.0)
-Requires-Dist: xvec (>=0.2.0)
+Requires-Dist: uvicorn (>=0.29.0,<0.30.0)
 Description-Content-Type: text/markdown
 
 # OpenEO FastAPI
 ![PyPI - Status](https://img.shields.io/pypi/status/openeo-fastapi)
 ![PyPI](https://img.shields.io/pypi/v/openeo-fastapi)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openeo-fastapi)
```

