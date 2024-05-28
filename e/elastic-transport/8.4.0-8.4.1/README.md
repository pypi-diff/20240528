# Comparing `tmp/elastic-transport-8.4.0.tar.gz` & `tmp/elastic-transport-8.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elastic-transport-8.4.0.tar", last modified: Thu Aug 25 15:42:24 2022, max compression
+gzip compressed data, was "elastic-transport-8.4.1.tar", last modified: Mon Sep 25 20:02:51 2023, max compression
```

## Comparing `elastic-transport-8.4.0.tar` & `elastic-transport-8.4.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 sethmlarson  (1000) sethmlarson  (1000)        0 2022-08-25 15:42:24.060541 elastic-transport-8.4.0/
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     4470 2022-08-16 17:04:47.000000 elastic-transport-8.4.0/CHANGELOG.md
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    10143 2020-08-19 19:54:09.000000 elastic-transport-8.4.0/LICENSE
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)      219 2021-12-27 18:46:12.000000 elastic-transport-8.4.0/MANIFEST.in
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     2731 2022-08-25 15:42:24.064541 elastic-transport-8.4.0/PKG-INFO
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     1355 2021-12-27 18:46:12.000000 elastic-transport-8.4.0/README.md
-drwxrwxr-x   0 sethmlarson  (1000) sethmlarson  (1000)        0 2022-08-25 15:42:24.060541 elastic-transport-8.4.0/elastic_transport/
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     3737 2022-02-03 00:10:23.000000 elastic-transport-8.4.0/elastic_transport/__init__.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    19828 2022-02-03 00:38:32.000000 elastic-transport-8.4.0/elastic_transport/_async_transport.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     3865 2021-12-28 00:09:46.000000 elastic-transport-8.4.0/elastic_transport/_compat.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     3871 2022-01-19 20:20:15.000000 elastic-transport-8.4.0/elastic_transport/_exceptions.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    12858 2022-02-02 22:10:26.000000 elastic-transport-8.4.0/elastic_transport/_models.py
-drwxrwxr-x   0 sethmlarson  (1000) sethmlarson  (1000)        0 2022-08-25 15:42:24.060541 elastic-transport-8.4.0/elastic_transport/_node/
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     1148 2022-02-03 00:38:32.000000 elastic-transport-8.4.0/elastic_transport/_node/__init__.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    11208 2022-04-19 14:20:22.000000 elastic-transport-8.4.0/elastic_transport/_node/_base.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     1510 2022-02-03 00:38:32.000000 elastic-transport-8.4.0/elastic_transport/_node/_base_async.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    10373 2022-03-09 20:04:54.000000 elastic-transport-8.4.0/elastic_transport/_node/_http_aiohttp.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     9981 2022-08-25 14:35:50.000000 elastic-transport-8.4.0/elastic_transport/_node/_http_requests.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     7998 2022-08-25 14:35:50.000000 elastic-transport-8.4.0/elastic_transport/_node/_http_urllib3.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     5272 2022-01-12 20:51:52.000000 elastic-transport-8.4.0/elastic_transport/_node/_urllib3_chain_certs.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    14924 2021-12-28 00:09:46.000000 elastic-transport-8.4.0/elastic_transport/_node_pool.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     6249 2022-03-30 22:40:40.000000 elastic-transport-8.4.0/elastic_transport/_response.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     7753 2022-03-30 22:40:40.000000 elastic-transport-8.4.0/elastic_transport/_serializer.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)    22852 2022-02-03 00:38:32.000000 elastic-transport-8.4.0/elastic_transport/_transport.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     3359 2022-04-19 14:21:22.000000 elastic-transport-8.4.0/elastic_transport/_utils.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)      810 2022-08-25 14:35:45.000000 elastic-transport-8.4.0/elastic_transport/_version.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     7926 2022-08-25 14:35:50.000000 elastic-transport-8.4.0/elastic_transport/client_utils.py
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)        0 2021-12-27 18:46:12.000000 elastic-transport-8.4.0/elastic_transport/py.typed
-drwxrwxr-x   0 sethmlarson  (1000) sethmlarson  (1000)        0 2022-08-25 15:42:24.060541 elastic-transport-8.4.0/elastic_transport.egg-info/
--rw-r--r--   0 sethmlarson  (1000) sethmlarson  (1000)     2731 2022-08-25 15:42:24.000000 elastic-transport-8.4.0/elastic_transport.egg-info/PKG-INFO
--rw-r--r--   0 sethmlarson  (1000) sethmlarson  (1000)      951 2022-08-25 15:42:24.000000 elastic-transport-8.4.0/elastic_transport.egg-info/SOURCES.txt
--rw-r--r--   0 sethmlarson  (1000) sethmlarson  (1000)        1 2022-08-25 15:42:24.000000 elastic-transport-8.4.0/elastic_transport.egg-info/dependency_links.txt
--rw-r--r--   0 sethmlarson  (1000) sethmlarson  (1000)      170 2022-08-25 15:42:24.000000 elastic-transport-8.4.0/elastic_transport.egg-info/requires.txt
--rw-r--r--   0 sethmlarson  (1000) sethmlarson  (1000)       18 2022-08-25 15:42:24.000000 elastic-transport-8.4.0/elastic_transport.egg-info/top_level.txt
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)      200 2022-08-25 15:42:24.064541 elastic-transport-8.4.0/setup.cfg
--rw-rw-r--   0 sethmlarson  (1000) sethmlarson  (1000)     3194 2022-04-19 14:20:22.000000 elastic-transport-8.4.0/setup.py
+drwxr-xr-x   0 joshmock  (1000) joshmock  (1000)        0 2023-09-25 20:02:51.109956 elastic-transport-8.4.1/
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)     4744 2023-09-25 19:51:24.000000 elastic-transport-8.4.1/CHANGELOG.md
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)    10143 2023-08-10 19:03:30.000000 elastic-transport-8.4.1/LICENSE
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)      219 2023-08-10 19:03:30.000000 elastic-transport-8.4.1/MANIFEST.in
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)     3458 2023-09-25 20:02:51.109956 elastic-transport-8.4.1/PKG-INFO
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)     1362 2023-09-18 15:05:21.000000 elastic-transport-8.4.1/README.md
+drwxr-xr-x   0 joshmock  (1000) joshmock  (1000)        0 2023-09-25 20:02:51.106623 elastic-transport-8.4.1/elastic_transport/
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)     3737 2023-08-10 19:03:30.000000 elastic-transport-8.4.1/elastic_transport/__init__.py
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)    19827 2023-08-10 19:03:30.000000 elastic-transport-8.4.1/elastic_transport/_async_transport.py
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)     3865 2023-08-10 19:03:30.000000 elastic-transport-8.4.1/elastic_transport/_compat.py
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)     3871 2023-08-10 19:03:30.000000 elastic-transport-8.4.1/elastic_transport/_exceptions.py
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)    12858 2023-08-10 19:03:30.000000 elastic-transport-8.4.1/elastic_transport/_models.py
+drwxr-xr-x   0 joshmock  (1000) joshmock  (1000)        0 2023-09-25 20:02:51.109956 elastic-transport-8.4.1/elastic_transport/_node/
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)     1148 2023-08-10 19:03:30.000000 elastic-transport-8.4.1/elastic_transport/_node/__init__.py
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)    11208 2023-08-10 19:03:30.000000 elastic-transport-8.4.1/elastic_transport/_node/_base.py
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)     1510 2023-08-10 19:03:30.000000 elastic-transport-8.4.1/elastic_transport/_node/_base_async.py
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)    10373 2023-08-10 19:03:30.000000 elastic-transport-8.4.1/elastic_transport/_node/_http_aiohttp.py
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)     9979 2023-08-10 19:03:30.000000 elastic-transport-8.4.1/elastic_transport/_node/_http_requests.py
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)     7996 2023-08-10 19:03:30.000000 elastic-transport-8.4.1/elastic_transport/_node/_http_urllib3.py
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)     5272 2023-08-10 19:03:30.000000 elastic-transport-8.4.1/elastic_transport/_node/_urllib3_chain_certs.py
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)    15033 2023-09-18 15:05:21.000000 elastic-transport-8.4.1/elastic_transport/_node_pool.py
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)     6482 2023-08-10 19:03:30.000000 elastic-transport-8.4.1/elastic_transport/_response.py
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)     7753 2023-08-10 19:03:30.000000 elastic-transport-8.4.1/elastic_transport/_serializer.py
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)    22851 2023-08-10 19:03:30.000000 elastic-transport-8.4.1/elastic_transport/_transport.py
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)     3359 2023-08-10 19:03:30.000000 elastic-transport-8.4.1/elastic_transport/_utils.py
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)      810 2023-09-25 19:51:24.000000 elastic-transport-8.4.1/elastic_transport/_version.py
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)     7846 2023-09-18 15:05:21.000000 elastic-transport-8.4.1/elastic_transport/client_utils.py
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)        0 2023-08-10 19:03:30.000000 elastic-transport-8.4.1/elastic_transport/py.typed
+drwxr-xr-x   0 joshmock  (1000) joshmock  (1000)        0 2023-09-25 20:02:51.106623 elastic-transport-8.4.1/elastic_transport.egg-info/
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)     3458 2023-09-25 20:02:51.000000 elastic-transport-8.4.1/elastic_transport.egg-info/PKG-INFO
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)      951 2023-09-25 20:02:51.000000 elastic-transport-8.4.1/elastic_transport.egg-info/SOURCES.txt
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)        1 2023-09-25 20:02:51.000000 elastic-transport-8.4.1/elastic_transport.egg-info/dependency_links.txt
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)      209 2023-09-25 20:02:51.000000 elastic-transport-8.4.1/elastic_transport.egg-info/requires.txt
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)       18 2023-09-25 20:02:51.000000 elastic-transport-8.4.1/elastic_transport.egg-info/top_level.txt
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)      200 2023-09-25 20:02:51.109956 elastic-transport-8.4.1/setup.cfg
+-rw-r--r--   0 joshmock  (1000) joshmock  (1000)     3380 2023-09-25 19:51:24.000000 elastic-transport-8.4.1/setup.py
```

### Comparing `elastic-transport-8.4.0/CHANGELOG.md` & `elastic-transport-8.4.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 # Changelog
 
+## 8.4.1
+
+- Fixed an issue where a large number of consecutive failures to connect to a node would raise an `OverflowError`.
+- Fixed an issue to ensure that `ApiResponse` can be pickled.
+
+## 8.4.0
+
+### Added
+
+- Added method for clients to use default ports for URL scheme.
+
 ## 8.1.2
 
 ### Fixed
 
 - Fixed issue when connecting to an IP address with HTTPS enabled would result in a `ValueError` for a mismatch between `check_hostname` and `server_hostname`.
 
 ## 8.1.1
```

### Comparing `elastic-transport-8.4.0/LICENSE` & `elastic-transport-8.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elastic-transport-8.4.0/README.md` & `elastic-transport-8.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # elastic-transport-python
 
 [![PyPI](https://img.shields.io/pypi/v/elastic-transport)](https://pypi.org/elastic-transport)
 [![Python Versions](https://img.shields.io/pypi/pyversions/elastic-transport)](https://pypi.org/elastic-transport)
-[![PyPI Downloads](https://pepy.tech/badge/elastic-transport)](https://pepy.tech/project/elastic-transport)
+[![PyPI Downloads](https://static.pepy.tech/badge/elastic-transport)](https://pepy.tech/project/elastic-transport)
 [![CI Status](https://img.shields.io/github/workflow/status/elastic/elastic-transport-python/CI/main)](https://github.com/elastic/elastic-transport-python/actions)
 
 Transport classes and utilities shared among Python Elastic client libraries
 
 This library was lifted from [`elasticsearch-py`](https://github.com/elastic/elasticsearch-py)
 and then transformed to be used across all Elastic services
 rather than only Elasticsearch.
```

### Comparing `elastic-transport-8.4.0/elastic_transport/__init__.py` & `elastic-transport-8.4.1/elastic_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-transport-8.4.0/elastic_transport/_async_transport.py` & `elastic-transport-8.4.1/elastic_transport/_async_transport.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,14 @@
         else:
             request_body = None
 
         # Errors are stored from (oldest->newest)
         errors: List[Exception] = []
 
         for attempt in range(max_retries + 1):
-
             # If we sniff before requests are made we want to do so before
             # 'node_pool.get()' is called so our sniffed nodes show up in the pool.
             if self._sniff_before_requests:
                 await self.sniff(False)
 
             retry = False
             node_failure = False
```

### Comparing `elastic-transport-8.4.0/elastic_transport/_compat.py` & `elastic-transport-8.4.1/elastic_transport/_compat.py`

 * *Files identical despite different names*

### Comparing `elastic-transport-8.4.0/elastic_transport/_exceptions.py` & `elastic-transport-8.4.1/elastic_transport/_exceptions.py`

 * *Files identical despite different names*

### Comparing `elastic-transport-8.4.0/elastic_transport/_models.py` & `elastic-transport-8.4.1/elastic_transport/_models.py`

 * *Files identical despite different names*

### Comparing `elastic-transport-8.4.0/elastic_transport/_node/__init__.py` & `elastic-transport-8.4.1/elastic_transport/_node/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-transport-8.4.0/elastic_transport/_node/_base.py` & `elastic-transport-8.4.1/elastic_transport/_node/_base.py`

 * *Files identical despite different names*

### Comparing `elastic-transport-8.4.0/elastic_transport/_node/_base_async.py` & `elastic-transport-8.4.1/elastic_transport/_node/_base_async.py`

 * *Files identical despite different names*

### Comparing `elastic-transport-8.4.0/elastic_transport/_node/_http_aiohttp.py` & `elastic-transport-8.4.1/elastic_transport/_node/_http_aiohttp.py`

 * *Files identical despite different names*

### Comparing `elastic-transport-8.4.0/elastic_transport/_node/_http_requests.py` & `elastic-transport-8.4.1/elastic_transport/_node/_http_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,25 +57,23 @@
         def init_poolmanager(
             self,
             connections: Any,
             maxsize: int,
             block: bool = False,
             **pool_kwargs: Any,
         ) -> None:
-
             if self._node_config.scheme == "https":
                 ssl_context = ssl_context_from_node_config(self._node_config)
                 pool_kwargs.setdefault("ssl_context", ssl_context)
 
                 # Fingerprint verification doesn't require CA certificates being loaded.
                 # We also want to disable other verification methods as we only care
                 # about the fingerprint of the certificates, not whether they form
                 # a verified chain to a trust anchor.
                 if self._node_config.ssl_assert_fingerprint:
-
                     # Manually disable these in the right order on the SSLContext
                     # so urllib3 won't think we want conflicting things.
                     ssl_context.check_hostname = False
                     ssl_context.verify_mode = ssl.CERT_NONE
 
                     pool_kwargs[
                         "assert_fingerprint"
```

### Comparing `elastic-transport-8.4.0/elastic_transport/_node/_http_urllib3.py` & `elastic-transport-8.4.1/elastic_transport/_node/_http_urllib3.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,14 @@
                 )
 
             # Fingerprint verification doesn't require CA certificates being loaded.
             # We also want to disable other verification methods as we only care
             # about the fingerprint of the certificates, not whether they form
             # a verified chain to a trust anchor.
             elif config.ssl_assert_fingerprint:
-
                 # Manually disable these in the right order on the SSLContext
                 # so urllib3 won't think we want conflicting things.
                 ssl_context.check_hostname = False
                 ssl_context.verify_mode = ssl.CERT_NONE
 
                 kw.update(
                     {
@@ -133,15 +132,14 @@
         self,
         method: str,
         target: str,
         body: Optional[bytes] = None,
         headers: Optional[HttpHeaders] = None,
         request_timeout: Union[DefaultType, Optional[float]] = DEFAULT,
     ) -> NodeApiResponse:
-
         if self.path_prefix:
             target = f"{self.path_prefix}{target}"
 
         start = time.time()
         try:
             kw = {}
             if request_timeout is not DEFAULT:
```

### Comparing `elastic-transport-8.4.0/elastic_transport/_node/_urllib3_chain_certs.py` & `elastic-transport-8.4.1/elastic_transport/_node/_urllib3_chain_certs.py`

 * *Files identical despite different names*

### Comparing `elastic-transport-8.4.0/elastic_transport/_node_pool.py` & `elastic-transport-8.4.1/elastic_transport/_node_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,18 +234,21 @@
         now: float = _now if _now is not None else time.time()
         try:
             del self._alive_nodes[node.config]
         except KeyError:
             pass
         consecutive_failures = self._dead_consecutive_failures[node.config] + 1
         self._dead_consecutive_failures[node.config] = consecutive_failures
-        timeout = min(
-            self._dead_node_backoff_factor * (2 ** (consecutive_failures - 1)),
-            self._max_dead_node_backoff,
-        )
+        try:
+            timeout = min(
+                self._dead_node_backoff_factor * (2 ** (consecutive_failures - 1)),
+                self._max_dead_node_backoff,
+            )
+        except OverflowError:
+            timeout = self._max_dead_node_backoff
         self._dead_nodes.put((now + timeout, node))
         _logger.warning(
             "Node %r has failed for %i times in a row, putting on %i second timeout",
             node,
             consecutive_failures,
             timeout,
         )
```

### Comparing `elastic-transport-8.4.0/elastic_transport/_response.py` & `elastic-transport-8.4.1/elastic_transport/_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     Any,
     Dict,
     Generic,
     Iterable,
     Iterator,
     List,
     NoReturn,
+    Tuple,
     TypeVar,
     Union,
     overload,
 )
 
 from ._models import ApiResponseMeta
 
@@ -93,14 +94,20 @@
 
     def __getitem__(self, item: Any) -> Any:
         return self._body[item]
 
     def __getattr__(self, attr: str) -> Any:
         return getattr(self._body, attr)
 
+    def __getstate__(self) -> Tuple[_BodyType, ApiResponseMeta]:
+        return self._body, self._meta
+
+    def __setstate__(self, state: Tuple[_BodyType, ApiResponseMeta]) -> None:
+        self._body, self._meta = state
+
     def __len__(self) -> int:
         return len(self._body)
 
     def __iter__(self) -> Iterable[Any]:
         return iter(self._body)  # type: ignore[no-any-return]
 
     def __str__(self) -> str:
```

### Comparing `elastic-transport-8.4.0/elastic_transport/_serializer.py` & `elastic-transport-8.4.1/elastic_transport/_serializer.py`

 * *Files identical despite different names*

### Comparing `elastic-transport-8.4.0/elastic_transport/_transport.py` & `elastic-transport-8.4.1/elastic_transport/_transport.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,15 +310,14 @@
         else:
             request_body = None
 
         # Errors are stored from (oldest->newest)
         errors: List[Exception] = []
 
         for attempt in range(max_retries + 1):
-
             # If we sniff before requests are made we want to do so before
             # 'node_pool.get()' is called so our sniffed nodes show up in the pool.
             if self._sniff_before_requests:
                 self.sniff(False)
 
             retry = False
             node_failure = False
```

### Comparing `elastic-transport-8.4.0/elastic_transport/_utils.py` & `elastic-transport-8.4.1/elastic_transport/_utils.py`

 * *Files identical despite different names*

### Comparing `elastic-transport-8.4.0/elastic_transport/_version.py` & `elastic-transport-8.4.1/elastic_transport/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
-__version__ = "8.4.0"
+__version__ = "8.4.1"
```

### Comparing `elastic-transport-8.4.0/elastic_transport/client_utils.py` & `elastic-transport-8.4.1/elastic_transport/client_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -132,25 +132,25 @@
         kibana_address=(kibana_host, port) if kibana_host else None,
     )
 
 
 def to_str(
     value: Union[str, bytes], encoding: str = "utf-8", errors: str = "strict"
 ) -> str:
-    if type(value) == bytes:
+    if isinstance(value, bytes):
         return value.decode(encoding, errors)
-    return value  # type: ignore[return-value]
+    return value
 
 
 def to_bytes(
     value: Union[str, bytes], encoding: str = "utf-8", errors: str = "strict"
 ) -> bytes:
-    if type(value) == str:
+    if isinstance(value, str):
         return value.encode(encoding, errors)
-    return value  # type: ignore[return-value]
+    return value
 
 
 # Python 3.7 added '~' to the safe list for urllib.parse.quote()
 _QUOTE_ALWAYS_SAFE = frozenset(
     "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789_.-~"
 )
 
@@ -194,15 +194,15 @@
     try:
         parsed_url = parse_url(url)
     except LocationParseError:
         raise ValueError(f"Could not parse URL {url!r}") from None
 
     # Only fill in a default port for HTTP and HTTPS
     # when we know the scheme is one of those two.
-    parsed_port: Optional[int] = parsed_url.port  # type: ignore[assignment]
+    parsed_port: Optional[int] = parsed_url.port
     if (
         parsed_url.port is None
         and parsed_url.scheme is not None
         and use_default_ports_for_scheme is True
     ):
         if parsed_url.scheme == "https":
             parsed_port = 443
```

### Comparing `elastic-transport-8.4.0/elastic_transport.egg-info/SOURCES.txt` & `elastic-transport-8.4.1/elastic_transport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elastic-transport-8.4.0/setup.py` & `elastic-transport-8.4.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,18 +33,16 @@
 
 setup(
     name="elastic-transport",
     description="Transport classes and utilities shared among Python Elastic client libraries",
     long_description=long_description,
     long_description_content_type="text/markdown",
     version=version,
-    author="Elastic",
-    author_email="support@elastic.co",
-    maintainer="Seth Michael Larson",
-    maintainer_email="seth.larson@elastic.co",
+    author="Elastic Client Library Maintainers",
+    author_email="client-libs@elastic.co",
     url="https://github.com/elastic/elastic-transport-python",
     project_urls={
         "Source Code": "https://github.com/elastic/elastic-transport-python",
         "Issue Tracker": "https://github.com/elastic/elastic-transport-python/issues",
         "Documentation": "https://elastic-transport-python.readthedocs.io",
     },
     package_data={"elastic_transport": ["py.typed"]},
@@ -62,25 +60,31 @@
             "pytest-mock",
             "pytest-asyncio",
             "pytest-httpserver",
             "trustme",
             "mock",
             "requests",
             "aiohttp",
+            # Override Read the Docs default (sphinx<2)
+            "sphinx>2",
+            "furo",
+            "sphinx-autodoc-typehints",
         ],
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
 )
```

