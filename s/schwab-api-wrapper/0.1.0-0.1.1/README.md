# Comparing `tmp/schwab_api_wrapper-0.1.0.tar.gz` & `tmp/schwab_api_wrapper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schwab_api_wrapper-0.1.0.tar", last modified: Mon May 27 20:54:31 2024, max compression
+gzip compressed data, was "schwab_api_wrapper-0.1.1.tar", last modified: Mon May 27 21:29:12 2024, max compression
```

## Comparing `schwab_api_wrapper-0.1.0.tar` & `schwab_api_wrapper-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 20:54:31.020486 schwab_api_wrapper-0.1.0/
--rw-r--r--   0 owengordon   (501) staff       (20)     1068 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/LICENSE
--rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-27 20:54:31.020263 schwab_api_wrapper-0.1.0/PKG-INFO
--rw-r--r--   0 owengordon   (501) staff       (20)       42 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/README.md
--rw-r--r--   0 owengordon   (501) staff       (20)      622 2024-05-27 20:54:01.000000 schwab_api_wrapper-0.1.0/pyproject.toml
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 20:54:31.017187 schwab_api_wrapper-0.1.0/schwab_api_wrapper/
--rw-r--r--   0 owengordon   (501) staff       (20)      125 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)      559 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/__main__.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 20:54:31.018435 schwab_api_wrapper-0.1.0/schwab_api_wrapper/market_data/
--rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/market_data/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1421 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/market_data/errors_schema.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1181 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/market_data/market_hours_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      599 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/market_data/price_history_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)    10268 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/market_data/quotes_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      248 2024-05-27 20:30:46.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/oauth_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1920 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/response_aware_retry.py
--rw-r--r--   0 owengordon   (501) staff       (20)    37772 2024-05-27 20:45:57.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/schwab.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 20:54:31.019540 schwab_api_wrapper-0.1.0/schwab_api_wrapper/trader_api/
--rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/trader_api/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     8019 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/trader_api/accounts_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      411 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/trader_api/errors_schema.py
--rw-r--r--   0 owengordon   (501) staff       (20)     9148 2024-05-27 15:05:40.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/trader_api/orders_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     6225 2024-05-27 17:27:34.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/trader_api/transactions_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     8190 2024-05-27 20:38:24.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper/utils.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 20:54:31.020046 schwab_api_wrapper-0.1.0/schwab_api_wrapper.egg-info/
--rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-27 20:54:31.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 owengordon   (501) staff       (20)      915 2024-05-27 20:54:31.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 owengordon   (501) staff       (20)        1 2024-05-27 20:54:31.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 owengordon   (501) staff       (20)       19 2024-05-27 20:54:31.000000 schwab_api_wrapper-0.1.0/schwab_api_wrapper.egg-info/top_level.txt
--rw-r--r--   0 owengordon   (501) staff       (20)       38 2024-05-27 20:54:31.020533 schwab_api_wrapper-0.1.0/setup.cfg
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 20:54:31.019836 schwab_api_wrapper-0.1.0/tests/
--rw-r--r--   0 owengordon   (501) staff       (20)    46341 2024-05-27 20:52:23.000000 schwab_api_wrapper-0.1.0/tests/test_schawb_api.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 21:29:12.697395 schwab_api_wrapper-0.1.1/
+-rw-r--r--   0 owengordon   (501) staff       (20)     1068 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.1/LICENSE
+-rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-27 21:29:12.697140 schwab_api_wrapper-0.1.1/PKG-INFO
+-rw-r--r--   0 owengordon   (501) staff       (20)       42 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.1/README.md
+-rw-r--r--   0 owengordon   (501) staff       (20)      622 2024-05-27 21:28:51.000000 schwab_api_wrapper-0.1.1/pyproject.toml
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 21:29:12.692963 schwab_api_wrapper-0.1.1/schwab_api_wrapper/
+-rw-r--r--   0 owengordon   (501) staff       (20)      125 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1691 2024-05-27 21:27:42.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/__main__.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 21:29:12.694622 schwab_api_wrapper-0.1.1/schwab_api_wrapper/market_data/
+-rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/market_data/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1421 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/market_data/errors_schema.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1181 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/market_data/market_hours_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      599 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/market_data/price_history_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)    10268 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/market_data/quotes_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      248 2024-05-27 20:30:46.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/oauth_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1920 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/response_aware_retry.py
+-rw-r--r--   0 owengordon   (501) staff       (20)    37118 2024-05-27 21:15:34.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/schwab.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 21:29:12.695874 schwab_api_wrapper-0.1.1/schwab_api_wrapper/trader_api/
+-rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/trader_api/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     8019 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/trader_api/accounts_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      411 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/trader_api/errors_schema.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     9148 2024-05-27 15:05:40.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/trader_api/orders_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     6225 2024-05-27 17:27:34.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/trader_api/transactions_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     8190 2024-05-27 20:38:24.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper/utils.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 21:29:12.696880 schwab_api_wrapper-0.1.1/schwab_api_wrapper.egg-info/
+-rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-27 21:29:12.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 owengordon   (501) staff       (20)      915 2024-05-27 21:29:12.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)        1 2024-05-27 21:29:12.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)       19 2024-05-27 21:29:12.000000 schwab_api_wrapper-0.1.1/schwab_api_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)       38 2024-05-27 21:29:12.697442 schwab_api_wrapper-0.1.1/setup.cfg
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-27 21:29:12.696226 schwab_api_wrapper-0.1.1/tests/
+-rw-r--r--   0 owengordon   (501) staff       (20)    46341 2024-05-27 20:52:23.000000 schwab_api_wrapper-0.1.1/tests/test_schawb_api.py
```

### Comparing `schwab_api_wrapper-0.1.0/LICENSE` & `schwab_api_wrapper-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.0/PKG-INFO` & `schwab_api_wrapper-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab_api_wrapper
-Version: 0.1.0
+Version: 0.1.1
 Summary: A wrapper package around the schwab http api
 Author-email: Owen Gordon <owengordon330@outlook.com>
 Project-URL: Homepage, https://github.com/OwenGordon/schwab-api-wrapper
 Project-URL: Issues, https://github.com/OwenGordon/schwab-api-wrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `schwab_api_wrapper-0.1.0/pyproject.toml` & `schwab_api_wrapper-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schwab_api_wrapper"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Owen Gordon", email="owengordon330@outlook.com" },
 ]
 description = "A wrapper package around the schwab http api"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

### Comparing `schwab_api_wrapper-0.1.0/schwab_api_wrapper/market_data/errors_schema.py` & `schwab_api_wrapper-0.1.1/schwab_api_wrapper/market_data/errors_schema.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.0/schwab_api_wrapper/market_data/market_hours_schemas.py` & `schwab_api_wrapper-0.1.1/schwab_api_wrapper/market_data/market_hours_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.0/schwab_api_wrapper/market_data/price_history_schemas.py` & `schwab_api_wrapper-0.1.1/schwab_api_wrapper/market_data/price_history_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.0/schwab_api_wrapper/market_data/quotes_schemas.py` & `schwab_api_wrapper-0.1.1/schwab_api_wrapper/market_data/quotes_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.0/schwab_api_wrapper/response_aware_retry.py` & `schwab_api_wrapper-0.1.1/schwab_api_wrapper/response_aware_retry.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.0/schwab_api_wrapper/schwab.py` & `schwab_api_wrapper-0.1.1/schwab_api_wrapper/schwab.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,31 +206,31 @@
             KEY_URI_REDIRECT: self.redirect_uri,
         }
 
         logging.getLogger(__name__).debug(
             "Generate Refresh Token Payload:\n" + pformat(payload)
         )
 
+        return self.__get_token(payload)
+
+    def __get_token(self, payload) -> tuple[Optional[Token], Optional[OAuthError]]:
         response = requests.post(
             TOKEN_URL,
             auth=HTTPBasicAuth(username=self.client_id, password=self.client_secret),
             data=payload,
         )
 
         logging.getLogger(__name__).info(
             f"Schwab API | POST `{TOKEN_URL}` | Status: {response.status_code}"
         )
 
         if response.status_code == STATUS_CODE_OK:
             token = Token(**response.json())
             logging.getLogger(__name__).debug("Response JSON:\n" + pformat(token))
 
-            print("New Token:")
-            pprint(token)
-
             return token, None
         else:
             error = OAuthError(**response.json())
             logging.getLogger(__name__).debug("Response JSON:\n" + pformat(error))
 
             return None, error
 
@@ -296,37 +296,15 @@
             KEY_TOKEN_REFRESH: self.refresh_token,
         }
 
         logging.getLogger(__name__).debug(
             "Refresh Access Token Payload:\n" + pformat(payload)
         )
 
-        response = requests.post(
-            TOKEN_URL,
-            auth=HTTPBasicAuth(username=self.client_id, password=self.client_secret),
-            data=payload,
-        )
-
-        logging.getLogger(__name__).info(
-            f"Schwab API | POST `{TOKEN_URL}` | Status: {response.status_code}"
-        )
-
-        if response.status_code == STATUS_CODE_OK:
-            token = Token(**response.json())
-            logging.getLogger(__name__).debug("Response JSON:\n" + pformat(token))
-
-            print("New Token:")
-            pprint(token)
-
-            return token, None
-        else:
-            error = OAuthError(**response.json())
-            logging.getLogger(__name__).debug("Response JSON:\n" + pformat(error))
-
-            return None, error
+        return self.__get_token(payload)
 
     def quotes(
         self,
         symbols: list[str],
         quotes_fields: Optional[list[QuotesField]] = None,
         indicative: bool = False,
         retry: bool = False,
```

### Comparing `schwab_api_wrapper-0.1.0/schwab_api_wrapper/trader_api/accounts_schemas.py` & `schwab_api_wrapper-0.1.1/schwab_api_wrapper/trader_api/accounts_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.0/schwab_api_wrapper/trader_api/orders_schemas.py` & `schwab_api_wrapper-0.1.1/schwab_api_wrapper/trader_api/orders_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.0/schwab_api_wrapper/trader_api/transactions_schemas.py` & `schwab_api_wrapper-0.1.1/schwab_api_wrapper/trader_api/transactions_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.0/schwab_api_wrapper/utils.py` & `schwab_api_wrapper-0.1.1/schwab_api_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.0/schwab_api_wrapper.egg-info/PKG-INFO` & `schwab_api_wrapper-0.1.1/schwab_api_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab_api_wrapper
-Version: 0.1.0
+Version: 0.1.1
 Summary: A wrapper package around the schwab http api
 Author-email: Owen Gordon <owengordon330@outlook.com>
 Project-URL: Homepage, https://github.com/OwenGordon/schwab-api-wrapper
 Project-URL: Issues, https://github.com/OwenGordon/schwab-api-wrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `schwab_api_wrapper-0.1.0/schwab_api_wrapper.egg-info/SOURCES.txt` & `schwab_api_wrapper-0.1.1/schwab_api_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.1.0/tests/test_schawb_api.py` & `schwab_api_wrapper-0.1.1/tests/test_schawb_api.py`

 * *Files identical despite different names*

