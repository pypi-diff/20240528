# Comparing `tmp/cognito_pyauth-1.3.3.tar.gz` & `tmp/cognito_pyauth-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognito_pyauth-1.3.3.tar", max compression
+gzip compressed data, was "cognito_pyauth-1.3.4.tar", max compression
```

## Comparing `cognito_pyauth-1.3.3.tar` & `cognito_pyauth-1.3.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0       18 2022-11-09 08:30:18.908944 cognito_pyauth-1.3.3/README.md
--rwxr-xr-x   0        0        0      123 2023-03-29 01:00:12.484272 cognito_pyauth-1.3.3/cognito_pyauth/__init__.py
--rwxr-xr-x   0        0        0     5083 2022-11-09 08:30:18.909454 cognito_pyauth-1.3.3/cognito_pyauth/auth.py
--rwxr-xr-x   0        0        0     1260 2022-11-09 08:30:18.909454 cognito_pyauth-1.3.3/cognito_pyauth/config.py
--rwxr-xr-x   0        0        0      368 2022-11-09 08:30:18.909958 cognito_pyauth-1.3.3/cognito_pyauth/exceptions.py
--rwxr-xr-x   0        0        0       53 2022-11-09 08:30:18.909958 cognito_pyauth-1.3.3/cognito_pyauth/logger.py
--rwxr-xr-x   0        0        0     1909 2023-03-29 01:00:12.486318 cognito_pyauth-1.3.3/cognito_pyauth/schemas.py
--rwxr-xr-x   0        0        0      329 2022-11-09 08:30:18.910457 cognito_pyauth-1.3.3/cognito_pyauth/utils.py
--rwxr-xr-x   0        0        0      945 2023-03-29 01:00:12.486834 cognito_pyauth-1.3.3/pyproject.toml
--rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 cognito_pyauth-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0       18 2022-02-23 10:37:41.712735 cognito_pyauth-1.3.4/README.md
+-rw-r--r--   0        0        0      123 2023-03-28 10:32:58.246251 cognito_pyauth-1.3.4/cognito_pyauth/__init__.py
+-rw-r--r--   0        0        0     5156 2024-05-28 06:26:11.741512 cognito_pyauth-1.3.4/cognito_pyauth/auth.py
+-rw-r--r--   0        0        0     1271 2024-05-28 05:44:50.400887 cognito_pyauth-1.3.4/cognito_pyauth/config.py
+-rw-r--r--   0        0        0      368 2022-02-25 07:28:18.503064 cognito_pyauth-1.3.4/cognito_pyauth/exceptions.py
+-rw-r--r--   0        0        0       53 2022-02-24 01:24:22.394593 cognito_pyauth-1.3.4/cognito_pyauth/logger.py
+-rw-r--r--   0        0        0     1999 2024-05-28 06:09:18.888371 cognito_pyauth-1.3.4/cognito_pyauth/schemas.py
+-rw-r--r--   0        0        0      329 2022-02-23 10:35:30.111272 cognito_pyauth-1.3.4/cognito_pyauth/utils.py
+-rw-r--r--   0        0        0      945 2024-05-28 05:39:29.650061 cognito_pyauth-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 cognito_pyauth-1.3.4/PKG-INFO
```

### Comparing `cognito_pyauth-1.3.3/cognito_pyauth/auth.py` & `cognito_pyauth-1.3.4/cognito_pyauth/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import boto3
 import jwt
 from fastapi import Depends
 
 from cognito_pyauth import exceptions, schemas
 from cognito_pyauth.config import Config
 from cognito_pyauth.utils import get_api_token
+from cognito_pyauth.logger import logger
 
 
 class Auth:
     config: Config
     client: Any
 
     def __init__(self, config: Config) -> None:
@@ -36,15 +37,16 @@
                 options={"require_exp": True},
                 audience=self.config.client_id,
             )
             return schemas.Payload(
                 **decoded,
                 username=decoded["cognito:username"],
             )
-        except Exception:
+        except Exception as e:
+            logger.info(e)
             raise exceptions.NotAuthorizedException()
 
     def get_payload_depends(
         self,
         token: str = Depends(get_api_token),
     ) -> schemas.Payload:
         try:
```

### Comparing `cognito_pyauth-1.3.3/cognito_pyauth/config.py` & `cognito_pyauth-1.3.4/cognito_pyauth/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         self.cognito_jwk_url = f"{self.cognito_url}/.well-known/jwks.json"
 
         self._init_public_keys()
 
     def get_public_key(self, kid: str) -> str:
         for key in self.public_keys:
             if key.kid == kid:
-                return jwt.algorithms.RSAAlgorithm.from_jwk(key.json())
+                return jwt.algorithms.RSAAlgorithm.from_jwk(key.model_dump_json())
         else:
             raise Exception("not found public key")
 
     def _init_public_keys(self) -> None:
         res = requests.get(self.cognito_jwk_url)
         for key in res.json()["keys"]:
             self.public_keys.append(Key(**key))
```

### Comparing `cognito_pyauth-1.3.3/cognito_pyauth/schemas.py` & `cognito_pyauth-1.3.4/cognito_pyauth/schemas.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional
-from pydantic import BaseModel, Field, SecretStr, validator
+from pydantic import BaseModel, Field, SecretStr, field_validator, ConfigDict
 
 
 class Payload(BaseModel):
     sub: str
     email_verified: Optional[bool]
     iss: str
     username: str
@@ -12,15 +12,17 @@
     event_id: str
     token_use: str
     auth_time: str
     exp: str
     iat: str
     jti: str
     email: Optional[str]
-    preferred_username: Optional[str]
+    preferred_username: Optional[str] = None
+
+    model_config = ConfigDict(coerce_numbers_to_str=True)
 
 
 class AuthenticationResult(BaseModel):
     access_token: str = Field(title="アクセストークン")
     id_token: str = Field(title="IDトークン")
     refresh_token: str = Field(title="更新トークン")
     token_type: str = Field(title="トークンタイプ")
@@ -44,15 +46,15 @@
     password: SecretStr = Field(title="パスワード", min_length=4)
 
 
 class ConfirmSignupRequest(BaseModel):
     username: str = Field(title="ユーザー名")
     confirmation_code: str = Field(title="検証コード", min_length=6, max_length=6)
 
-    @validator("confirmation_code")
+    @field_validator("confirmation_code")
     def confirmation_code_validator(cls, v: str) -> str:
         if not v.isnumeric():
             raise ValueError("検証コードは6桁の数字です")
         return v
 
 
 class ResendConfirmationCodeRequest(BaseModel):
```

### Comparing `cognito_pyauth-1.3.3/pyproject.toml` & `cognito_pyauth-1.3.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "cognito-pyauth"
-version = "1.3.3"
+version = "1.3.4"
 description = ""
 readme = "README.md"
 authors = ["fuuga"]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
+python = ">=3.8,<4.0"
 requests = ">=2.0,<3.0"
 PyJWT = {version = ">=2.0,<3.0", extras = ["crypto"]}
-pydantic = ">=1.0,<2.0"
+pydantic = ">=2.0,<3.0"
 fastapi = ">=0.75.0,<1.0"
 boto3 = ">=1.0,<2.0"
 
 [tool.poetry.dev-dependencies]
 mypy = "^0.930"
 flake8 = "^4.0.1"
 black = "^22.1.0"
```

### Comparing `cognito_pyauth-1.3.3/PKG-INFO` & `cognito_pyauth-1.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: cognito-pyauth
-Version: 1.3.3
+Version: 1.3.4
 Summary: 
 Author: fuuga
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyJWT[crypto] (>=2.0,<3.0)
 Requires-Dist: boto3 (>=1.0,<2.0)
 Requires-Dist: fastapi (>=0.75.0,<1.0)
-Requires-Dist: pydantic (>=1.0,<2.0)
+Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: requests (>=2.0,<3.0)
 Description-Content-Type: text/markdown
 
 # cognito-pyauth
```

