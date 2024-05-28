# Comparing `tmp/mosqlient-1.0.1.tar.gz` & `tmp/mosqlient-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosqlient-1.0.1.tar", max compression
+gzip compressed data, was "mosqlient-1.1.0.tar", max compression
```

## Comparing `mosqlient-1.0.1.tar` & `mosqlient-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0   329588 2024-05-27 18:05:49.618548 mosqlient-1.0.1/LICENSE
--rw-r--r--   0        0        0      852 2024-05-27 18:05:49.618548 mosqlient-1.0.1/README.md
--rw-r--r--   0        0        0      577 2024-05-27 18:05:49.618548 mosqlient-1.0.1/mosqlient/__init__.py
--rw-r--r--   0        0        0      353 2024-05-27 18:05:49.618548 mosqlient-1.0.1/mosqlient/__main__.py
--rw-r--r--   0        0        0     1222 2024-05-27 18:05:49.618548 mosqlient-1.0.1/mosqlient/cli.py
--rw-r--r--   0        0        0      927 2024-05-27 18:05:49.618548 mosqlient-1.0.1/mosqlient/client.py
--rw-r--r--   0        0        0      204 2024-05-27 18:05:49.618548 mosqlient-1.0.1/mosqlient/config.py
--rw-r--r--   0        0        0        0 2024-05-27 18:05:49.618548 mosqlient-1.0.1/mosqlient/datastore/__init__.py
--rw-r--r--   0        0        0        0 2024-05-27 18:05:49.618548 mosqlient-1.0.1/mosqlient/datastore/predictions.py
--rw-r--r--   0        0        0      891 2024-05-27 18:05:49.618548 mosqlient-1.0.1/mosqlient/errors.py
--rw-r--r--   0        0        0      651 2024-05-27 18:05:49.618548 mosqlient-1.0.1/mosqlient/models/__init__.py
--rw-r--r--   0        0        0      133 2024-05-27 18:05:49.618548 mosqlient-1.0.1/mosqlient/models/temporal.py
--rw-r--r--   0        0        0       30 2024-05-27 18:05:49.618548 mosqlient-1.0.1/mosqlient/predictions/__init__.py
--rw-r--r--   0        0        0       26 2024-05-27 18:05:49.618548 mosqlient-1.0.1/mosqlient/registry/__init__.py
--rw-r--r--   0        0        0     5376 2024-05-27 18:05:49.618548 mosqlient-1.0.1/mosqlient/registry/models.py
--rw-r--r--   0        0        0     2860 2024-05-27 18:05:49.618548 mosqlient-1.0.1/mosqlient/requests.py
--rw-r--r--   0        0        0        0 2024-05-27 18:05:49.618548 mosqlient-1.0.1/mosqlient/tests/__init__.py
--rw-r--r--   0        0        0      238 2024-05-27 18:05:49.618548 mosqlient-1.0.1/mosqlient/utils/validate.py
--rw-r--r--   0        0        0     2128 2024-05-27 18:06:51.134756 mosqlient-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1745 1970-01-01 00:00:00.000000 mosqlient-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0   329588 2024-05-28 21:32:31.485807 mosqlient-1.1.0/LICENSE
+-rw-r--r--   0        0        0      852 2024-05-28 21:32:31.485807 mosqlient-1.1.0/README.md
+-rw-r--r--   0        0        0      578 2024-05-28 21:32:31.489807 mosqlient-1.1.0/mosqlient/__init__.py
+-rw-r--r--   0        0        0      344 2024-05-28 21:32:31.489807 mosqlient-1.1.0/mosqlient/__main__.py
+-rw-r--r--   0        0        0     1222 2024-05-28 21:32:31.489807 mosqlient-1.1.0/mosqlient/cli.py
+-rw-r--r--   0        0        0      823 2024-05-28 21:32:31.489807 mosqlient-1.1.0/mosqlient/client.py
+-rw-r--r--   0        0        0      204 2024-05-28 21:32:31.489807 mosqlient-1.1.0/mosqlient/config.py
+-rw-r--r--   0        0        0       47 2024-05-28 21:32:31.489807 mosqlient-1.1.0/mosqlient/datastore/__init__.py
+-rw-r--r--   0        0        0     2554 2024-05-28 21:32:31.489807 mosqlient-1.1.0/mosqlient/datastore/api.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:32:31.489807 mosqlient-1.1.0/mosqlient/datastore/predictions.py
+-rw-r--r--   0        0        0      869 2024-05-28 21:32:31.489807 mosqlient-1.1.0/mosqlient/errors.py
+-rw-r--r--   0        0        0      651 2024-05-28 21:32:31.489807 mosqlient-1.1.0/mosqlient/models/__init__.py
+-rw-r--r--   0        0        0      129 2024-05-28 21:32:31.489807 mosqlient-1.1.0/mosqlient/models/temporal.py
+-rw-r--r--   0        0        0       26 2024-05-28 21:32:31.489807 mosqlient-1.1.0/mosqlient/predictions/__init__.py
+-rw-r--r--   0        0        0       33 2024-05-28 21:32:31.489807 mosqlient-1.1.0/mosqlient/registry/__init__.py
+-rw-r--r--   0        0        0     5078 2024-05-28 21:32:31.489807 mosqlient-1.1.0/mosqlient/registry/models.py
+-rw-r--r--   0        0        0     4940 2024-05-28 21:32:31.489807 mosqlient-1.1.0/mosqlient/requests.py
+-rw-r--r--   0        0        0        0 2024-05-28 21:32:31.489807 mosqlient-1.1.0/mosqlient/tests/__init__.py
+-rw-r--r--   0        0        0      204 2024-05-28 21:32:31.489807 mosqlient-1.1.0/mosqlient/utils/validate.py
+-rw-r--r--   0        0        0     2128 2024-05-28 21:33:37.229861 mosqlient-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1745 1970-01-01 00:00:00.000000 mosqlient-1.1.0/PKG-INFO
```

### Comparing `mosqlient-1.0.1/LICENSE` & `mosqlient-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mosqlient-1.0.1/README.md` & `mosqlient-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mosqlient-1.0.1/mosqlient/__init__.py` & `mosqlient-1.1.0/mosqlient/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Mosqlimate client package.
 
 client library for the Mosqlimate project data platform.
 """
+
 from importlib import metadata as importlib_metadata
 from typing import List
 
 from mosqlient.client import PlatformClient as Client  # noqa
 
 
 def get_version() -> str:
```

### Comparing `mosqlient-1.0.1/mosqlient/cli.py` & `mosqlient-1.1.0/mosqlient/cli.py`

 * *Files identical despite different names*

### Comparing `mosqlient-1.0.1/mosqlient/client.py` & `mosqlient-1.1.0/mosqlient/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,25 +13,17 @@
         return self.username
 
     @property
     def X_UID_KEY(self):
         return f"{self.username}:{self.uid_key}"
 
     def _check_username(self):
-        author = get(
-            "registry",
-            "authors",
-            {"username": self.username},
-            pagination=False
-        )
+        author = get("registry", "authors", {"username": self.username}, pagination=False)
 
         if author.status_code != 200:
-            raise ValueError(
-                f"Could not get user '{self.username}' info. "
-                f"Status code: {author.status_code}"
-            )
+            raise ValueError(f"Could not get user '{self.username}' info. " f"Status code: {author.status_code}")
 
     def _check_uuid4(self):
         try:
             uuid.UUID(self.uid_key, version=4)
         except ValueError:
             raise ValueError("uid_key is not a valid key")
```

### Comparing `mosqlient-1.0.1/mosqlient/errors.py` & `mosqlient-1.1.0/mosqlient/errors.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-from typing import Iterable, Union, Any
+from typing import Any, Iterable, Union
 
 
 class ValidationErrorBase(Exception):
     """Base exception class for validation errors"""
 
     def __init__(self, message=None):
         super().__init__(message or "A validation error occurred")
 
 
 class FieldTypeError(ValidationErrorBase):
     """Exception raised for errors in a specific field."""
 
     def __init__(self, field: str, _type: Union[Iterable, Any]):
         self.field = field
-        super().__init__(
-            f"Incorrect type for field: '{field}'. Expected type(s): '{_type}'"
-        )
+        super().__init__(f"Incorrect type for field: '{field}'. Expected type(s): '{_type}'")
 
     def __str__(self):
         return f"{self.field}: {self.args[0]}"
 
 
 class ClientError(Exception):
     def __init__(self, message=None):
```

### Comparing `mosqlient-1.0.1/mosqlient/models/__init__.py` & `mosqlient-1.1.0/mosqlient/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mosqlient-1.0.1/mosqlient/registry/models.py` & `mosqlient-1.1.0/mosqlient/registry/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import asyncio
+from typing import Any, Literal, Optional
 from urllib.parse import urlparse
-from typing import Literal, Optional, Any
 
-import requests
 import nest_asyncio
+import requests
 
 from mosqlient import Client
-from mosqlient.config import API_PROD_URL, API_DEV_URL
-from mosqlient.requests import get_all
+from mosqlient.config import API_DEV_URL, API_PROD_URL
 from mosqlient.errors import ClientError, ModelPostError
+from mosqlient.requests import get_all
 
 nest_asyncio.apply()
 
 
 def _params(**kwargs) -> dict[str, Any]:
     params = {}
     for k, v in kwargs.items():
@@ -54,15 +54,15 @@
         implementation_language: str,
         disease: Literal["dengue", "chikungunya", "zika"],
         temporal: bool,
         spatial: bool,
         categorical: bool,
         adm_level: Literal[0, 1, 2, 3],
         time_resolution: Literal["day", "week", "month", "year"],
-        _env: Literal["dev", "prod"] = "prod"
+        _env: Literal["dev", "prod"] = "prod",
     ):
         if self.client is None:
             raise ClientError(
                 "A Client instance must be provided, please instantiate Model "
                 "passing your Mosqlimate's credentials. For more infor about "
                 "retrieving or inserting data from Mosqlimate, please see the "
                 "API Documentation"
@@ -73,28 +73,27 @@
             "repository": repository,
             "implementation_language": implementation_language,
             "disease": disease,
             "temporal": temporal,
             "spatial": spatial,
             "categorical": categorical,
             "ADM_level": adm_level,
-            "time_resolution": time_resolution
+            "time_resolution": time_resolution,
         }
 
         self._validate_fields(**params)
-        params = _params(**params)
+
         base_url = API_DEV_URL if _env == "dev" else API_PROD_URL
         url = base_url + "/".join(("registry", "models")) + "/"
         headers = {"X-UID-Key": self.client.X_UID_KEY}
         resp = requests.post(url, json=params, headers=headers, timeout=60)
 
         if resp.status_code != 201:
-            raise ModelPostError(
-                f"POST request returned status code {resp.status_code}"
-            )
+            
+            raise ModelPostError(f"POST request returned status code {resp.status_code} \n {resp.reason}")
 
         return resp
 
     @staticmethod
     def _validate_fields(**kwargs) -> None:
         ModelFieldValidator(**kwargs)
 
@@ -122,51 +121,39 @@
 
     def __init__(self, **kwargs):
         for k, v in kwargs.items():
             if v is None:
                 continue
 
             if not isinstance(v, self.FIELDS[k]):
-                raise TypeError(
-                    f"Field '{k}' must have instance of "
-                    f"{' or '.join(self.FIELDS[k])}"
-                )
+                raise TypeError(f"Field '{k}' must have instance of " f"{' or '.join(self.FIELDS[k])}")
 
             if k == "id":
                 if v <= 0:
                     raise ValueError("Incorrect value for field 'id'")
 
             if k == "description":
                 if not v:
                     raise ValueError("A Model description must be provided")
                 if len(v) > 500:
                     raise ValueError("Model description too long")
 
             if k == "repository":
                 repo_url = urlparse(v)
                 if repo_url.netloc != "github.com":
-                    raise ValueError(
-                        "'repository' must be a valid GitHub repository"
-                    )
+                    raise ValueError("'repository' must be a valid GitHub repository")
 
             if k == "disease":
                 if v == "chik":
                     v = "chikungunya"
 
                 if v not in self.DISEASES:
-                    raise ValueError(
-                        f"Unkown 'disease'. Options: {self.DISEASES}"
-                    )
+                    raise ValueError(f"Unkown 'disease'. Options: {self.DISEASES}")
 
             if k == "ADM_level":
                 v = int(v)
                 if v not in self.ADM_LEVELS:
-                    raise ValueError(
-                        f"Unkown 'ADM_level'. Options: {self.ADM_LEVELS}"
-                    )
+                    raise ValueError(f"Unkown 'ADM_level'. Options: {self.ADM_LEVELS}")
 
             if k == "time_resolution":
                 if v not in self.TIME_RESOLUTIONS:
-                    raise ValueError(
-                        "Unkown 'time_resolution'. "
-                        f"Options: {self.TIME_RESOLUTIONS}"
-                    )
+                    raise ValueError("Unkown 'time_resolution'. " f"Options: {self.TIME_RESOLUTIONS}")
```

### Comparing `mosqlient-1.0.1/pyproject.toml` & `mosqlient-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mosqlient"
-version = "1.0.1"  # changed by semantic-release
+version = "1.1.0"  # changed by semantic-release
 description = "client library for the mosqlimate client library"
 authors = ["Flávio Codeço Coelho <fccoelho@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 repository = "https://github.com/Mosqlimate-project/mosqlimate-client"
 homepage = "https://github.com/Mosqlimate-project/mosqlimate-client"
 keywords = ["data science", "epidemiology", "forecasting"]
```

### Comparing `mosqlient-1.0.1/PKG-INFO` & `mosqlient-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosqlient
-Version: 1.0.1
+Version: 1.1.0
 Summary: client library for the mosqlimate client library
 Home-page: https://github.com/Mosqlimate-project/mosqlimate-client
 License: GPLv3
 Keywords: data science,epidemiology,forecasting
 Author: Flávio Codeço Coelho
 Author-email: fccoelho@gmail.com
 Requires-Python: >=3.10,<4.0
```

