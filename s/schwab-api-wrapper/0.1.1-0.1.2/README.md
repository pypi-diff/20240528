# Comparing `tmp/schwab_api_wrapper-0.1.1.tar.gz` & `tmp/schwab_api_wrapper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schwab_api_wrapper-0.1.1.tar", last modified: Mon May 27 21:29:12 2024, max compression
+gzip compressed data, was "schwab_api_wrapper-0.1.2.tar", last modified: Mon May 27 22:37:15 2024, max compression
```

## Comparing `schwab_api_wrapper-0.1.1.tar` & `schwab_api_wrapper-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 21:29:12.697395 schwab_api_wrapper-0.1.1/
--rw-r--r--   0 owengordon   (501) staff       (20)     1068 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.1/LICENSE
--rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-27 21:29:12.697140 schwab_api_wrapper-0.1.1/PKG-INFO
--rw-r--r--   0 owengordon   (501) staff       (20)       42 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.1/README.md
--rw-r--r--   0 owengordon   (501) staff       (20)      622 2024-05-27 21:28:51.000000 schwab_api_wrapper-0.1.1/pyproject.toml
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 21:29:12.692963 schwab_api_wrapper-0.1.1/schwab_api_wrapper/
--rw-r--r--   0 owengordon   (501) staff       (20)      125 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1691 2024-05-27 21:27:42.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/__main__.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 21:29:12.694622 schwab_api_wrapper-0.1.1/schwab_api_wrapper/market_data/
--rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/market_data/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1421 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/market_data/errors_schema.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1181 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/market_data/market_hours_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      599 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/market_data/price_history_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)    10268 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/market_data/quotes_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      248 2024-05-27 20:30:46.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/oauth_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1920 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/response_aware_retry.py
--rw-r--r--   0 owengordon   (501) staff       (20)    37118 2024-05-27 21:15:34.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/schwab.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 21:29:12.695874 schwab_api_wrapper-0.1.1/schwab_api_wrapper/trader_api/
--rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/trader_api/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     8019 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/trader_api/accounts_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      411 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/trader_api/errors_schema.py
--rw-r--r--   0 owengordon   (501) staff       (20)     9148 2024-05-27 15:05:40.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/trader_api/orders_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     6225 2024-05-27 17:27:34.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/trader_api/transactions_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     8190 2024-05-27 20:38:24.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/utils.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 21:29:12.696880 schwab_api_wrapper-0.1.1/schwab_api_wrapper.egg-info/
--rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-27 21:29:12.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 owengordon   (501) staff       (20)      915 2024-05-27 21:29:12.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 owengordon   (501) staff       (20)        1 2024-05-27 21:29:12.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 owengordon   (501) staff       (20)       19 2024-05-27 21:29:12.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper.egg-info/top_level.txt
--rw-r--r--   0 owengordon   (501) staff       (20)       38 2024-05-27 21:29:12.697442 schwab_api_wrapper-0.1.1/setup.cfg
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 21:29:12.696226 schwab_api_wrapper-0.1.1/tests/
--rw-r--r--   0 owengordon   (501) staff       (20)    46341 2024-05-27 20:52:23.000000 schwab_api_wrapper-0.1.1/tests/test_schawb_api.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 22:37:15.991520 schwab_api_wrapper-0.1.2/
+-rw-r--r--   0 owengordon   (501) staff       (20)     1068 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.2/LICENSE
+-rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-27 22:37:15.991251 schwab_api_wrapper-0.1.2/PKG-INFO
+-rw-r--r--   0 owengordon   (501) staff       (20)       42 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.2/README.md
+-rw-r--r--   0 owengordon   (501) staff       (20)      622 2024-05-27 22:36:34.000000 schwab_api_wrapper-0.1.2/pyproject.toml
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 22:37:15.987248 schwab_api_wrapper-0.1.2/schwab_api_wrapper/
+-rw-r--r--   0 owengordon   (501) staff       (20)      125 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1691 2024-05-27 21:27:42.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/__main__.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 22:37:15.988828 schwab_api_wrapper-0.1.2/schwab_api_wrapper/market_data/
+-rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/market_data/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1421 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/market_data/errors_schema.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1181 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/market_data/market_hours_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      599 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/market_data/price_history_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)    10268 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/market_data/quotes_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      248 2024-05-27 20:30:46.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/oauth_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1920 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/response_aware_retry.py
+-rw-r--r--   0 owengordon   (501) staff       (20)    37206 2024-05-27 22:35:28.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/schwab.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 22:37:15.990017 schwab_api_wrapper-0.1.2/schwab_api_wrapper/trader_api/
+-rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/trader_api/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     8019 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/trader_api/accounts_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      411 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/trader_api/errors_schema.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     9148 2024-05-27 15:05:40.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/trader_api/orders_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     6225 2024-05-27 17:27:34.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/trader_api/transactions_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     8190 2024-05-27 20:38:24.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper/utils.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 22:37:15.990838 schwab_api_wrapper-0.1.2/schwab_api_wrapper.egg-info/
+-rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-27 22:37:15.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 owengordon   (501) staff       (20)      915 2024-05-27 22:37:15.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)        1 2024-05-27 22:37:15.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)       19 2024-05-27 22:37:15.000000 schwab_api_wrapper-0.1.2/schwab_api_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)       38 2024-05-27 22:37:15.991572 schwab_api_wrapper-0.1.2/setup.cfg
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 22:37:15.990284 schwab_api_wrapper-0.1.2/tests/
+-rw-r--r--   0 owengordon   (501) staff       (20)    46341 2024-05-27 20:52:23.000000 schwab_api_wrapper-0.1.2/tests/test_schawb_api.py
```

### Comparing `schwab_api_wrapper-0.1.1/LICENSE` & `schwab_api_wrapper-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.1/PKG-INFO` & `schwab_api_wrapper-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab_api_wrapper
-Version: 0.1.1
+Version: 0.1.2
 Summary: A wrapper package around the schwab http api
 Author-email: Owen Gordon <owengordon330@outlook.com>
 Project-URL: Homepage, https://github.com/OwenGordon/schwab-api-wrapper
 Project-URL: Issues, https://github.com/OwenGordon/schwab-api-wrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `schwab_api_wrapper-0.1.1/pyproject.toml` & `schwab_api_wrapper-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schwab_api_wrapper"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Owen Gordon", email="owengordon330@outlook.com" },
 ]
 description = "A wrapper package around the schwab http api"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

### Comparing `schwab_api_wrapper-0.1.1/schwab_api_wrapper/__main__.py` & `schwab_api_wrapper-0.1.2/schwab_api_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.1/schwab_api_wrapper/market_data/errors_schema.py` & `schwab_api_wrapper-0.1.2/schwab_api_wrapper/market_data/errors_schema.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.1/schwab_api_wrapper/market_data/market_hours_schemas.py` & `schwab_api_wrapper-0.1.2/schwab_api_wrapper/market_data/market_hours_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.1/schwab_api_wrapper/market_data/price_history_schemas.py` & `schwab_api_wrapper-0.1.2/schwab_api_wrapper/market_data/price_history_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.1/schwab_api_wrapper/market_data/quotes_schemas.py` & `schwab_api_wrapper-0.1.2/schwab_api_wrapper/market_data/quotes_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.1/schwab_api_wrapper/response_aware_retry.py` & `schwab_api_wrapper-0.1.2/schwab_api_wrapper/response_aware_retry.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.1/schwab_api_wrapper/schwab.py` & `schwab_api_wrapper-0.1.2/schwab_api_wrapper/schwab.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 from .trader_api.orders_schemas import Order, OrderRequest, PreviewOrder, OrderResponse
 from .trader_api.errors_schema import AccountsAndTradingError
 
 from .oauth_schemas import Token, OAuthError
 
 
 class OAuthException(Exception):
-    def __init__(self, title, error: OAuthError):
+    def __init__(self, title, error: OAuthError, parameters: dict):
         super().__init__(title)
         self.title = title
         self.error = error
-
+        self.parameters = parameters
 
 
 # TODO if the response doesn't have a .json() field it will error at us
 # I think we just let it fail in this case because pydantic verification will fail anyways too
 # Either this or we specifically check for a missing json field in an otherwise well-formed response
 
 
@@ -148,15 +148,15 @@
     def get_refresh_token_expiration(self) -> datetime:
         return self.refresh_token_valid_until
 
     def refresh(self):
         token, error = self.refresh_access_token()
 
         if error is not None:
-            raise OAuthException(f"Unable to generate refresh token", error)
+            raise OAuthException(f"Unable to generate refresh token", error, self.parameters)
         
         self.save_token(token)
 
         self.retry_session = requests.Session()
         self.retry_session.mount("http://", self.adapter)
         self.retry_session.mount("https://", self.adapter)
 
@@ -249,15 +249,15 @@
         url = input("Enter resulting redirected URL here: ")
 
         authorization_code, session_id = get_code_from_url(url)
 
         token, error = self.generate_refresh_token(authorization_code)
 
         if error is not None:
-            raise OAuthException(f"Unable to generate refresh token", error)
+            raise OAuthException(f"Unable to generate refresh token", error, self.parameters)
         
         self.save_token(token)
 
     def save_token(self, token: Token):
         self.refresh_token = token.refresh_token # valid for 7 days
         self.refresh_token_valid_until = datetime.now(timezone.utc) + timedelta(
             days=7
```

### Comparing `schwab_api_wrapper-0.1.1/schwab_api_wrapper/trader_api/accounts_schemas.py` & `schwab_api_wrapper-0.1.2/schwab_api_wrapper/trader_api/accounts_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.1/schwab_api_wrapper/trader_api/orders_schemas.py` & `schwab_api_wrapper-0.1.2/schwab_api_wrapper/trader_api/orders_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.1/schwab_api_wrapper/trader_api/transactions_schemas.py` & `schwab_api_wrapper-0.1.2/schwab_api_wrapper/trader_api/transactions_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.1/schwab_api_wrapper/utils.py` & `schwab_api_wrapper-0.1.2/schwab_api_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.1/schwab_api_wrapper.egg-info/PKG-INFO` & `schwab_api_wrapper-0.1.2/schwab_api_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab_api_wrapper
-Version: 0.1.1
+Version: 0.1.2
 Summary: A wrapper package around the schwab http api
 Author-email: Owen Gordon <owengordon330@outlook.com>
 Project-URL: Homepage, https://github.com/OwenGordon/schwab-api-wrapper
 Project-URL: Issues, https://github.com/OwenGordon/schwab-api-wrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `schwab_api_wrapper-0.1.1/schwab_api_wrapper.egg-info/SOURCES.txt` & `schwab_api_wrapper-0.1.2/schwab_api_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.1/tests/test_schawb_api.py` & `schwab_api_wrapper-0.1.2/tests/test_schawb_api.py`

 * *Files identical despite different names*

