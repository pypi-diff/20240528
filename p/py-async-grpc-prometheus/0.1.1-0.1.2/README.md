# Comparing `tmp/py_async_grpc_prometheus-0.1.1.tar.gz` & `tmp/py_async_grpc_prometheus-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_async_grpc_prometheus-0.1.1.tar", last modified: Tue May 28 10:46:24 2024, max compression
+gzip compressed data, was "py_async_grpc_prometheus-0.1.2.tar", last modified: Tue May 28 11:19:24 2024, max compression
```

## Comparing `py_async_grpc_prometheus-0.1.1.tar` & `py_async_grpc_prometheus-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:46:24.858388 py_async_grpc_prometheus-0.1.1/
--rwxrwxrwx   0 root         (0) root         (0)    11357 2024-05-28 10:24:41.000000 py_async_grpc_prometheus-0.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5591 2024-05-28 10:46:24.844083 py_async_grpc_prometheus-0.1.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5186 2024-05-28 10:42:16.000000 py_async_grpc_prometheus-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:46:24.608465 py_async_grpc_prometheus-0.1.1/py_async_grpc_prometheus/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 10:24:41.000000 py_async_grpc_prometheus-0.1.1/py_async_grpc_prometheus/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2696 2024-05-28 10:24:41.000000 py_async_grpc_prometheus-0.1.1/py_async_grpc_prometheus/client_metrics.py
--rwxrwxrwx   0 root         (0) root         (0)     1487 2024-05-28 10:24:41.000000 py_async_grpc_prometheus-0.1.1/py_async_grpc_prometheus/grpc_utils.py
--rwxrwxrwx   0 root         (0) root         (0)     7675 2024-05-28 10:24:41.000000 py_async_grpc_prometheus-0.1.1/py_async_grpc_prometheus/prometheus_async_client_interceptor.py
--rwxrwxrwx   0 root         (0) root         (0)     9865 2024-05-28 10:24:41.000000 py_async_grpc_prometheus-0.1.1/py_async_grpc_prometheus/prometheus_async_server_interceptor.py
--rwxrwxrwx   0 root         (0) root         (0)     2109 2024-05-28 10:24:41.000000 py_async_grpc_prometheus-0.1.1/py_async_grpc_prometheus/server_metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 10:46:24.826963 py_async_grpc_prometheus-0.1.1/py_async_grpc_prometheus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5591 2024-05-28 10:46:24.000000 py_async_grpc_prometheus-0.1.1/py_async_grpc_prometheus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      555 2024-05-28 10:46:24.000000 py_async_grpc_prometheus-0.1.1/py_async_grpc_prometheus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 10:46:24.000000 py_async_grpc_prometheus-0.1.1/py_async_grpc_prometheus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2024-05-28 10:46:24.000000 py_async_grpc_prometheus-0.1.1/py_async_grpc_prometheus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-28 10:46:24.000000 py_async_grpc_prometheus-0.1.1/py_async_grpc_prometheus.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 10:46:24.860395 py_async_grpc_prometheus-0.1.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      710 2024-05-28 10:46:19.000000 py_async_grpc_prometheus-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:19:24.127534 py_async_grpc_prometheus-0.1.2/
+-rwxrwxrwx   0 root         (0) root         (0)    11357 2024-05-28 10:24:41.000000 py_async_grpc_prometheus-0.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5591 2024-05-28 11:19:24.112444 py_async_grpc_prometheus-0.1.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5186 2024-05-28 10:42:16.000000 py_async_grpc_prometheus-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:19:23.897907 py_async_grpc_prometheus-0.1.2/py_async_grpc_prometheus/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 10:24:41.000000 py_async_grpc_prometheus-0.1.2/py_async_grpc_prometheus/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2696 2024-05-28 10:24:41.000000 py_async_grpc_prometheus-0.1.2/py_async_grpc_prometheus/client_metrics.py
+-rwxrwxrwx   0 root         (0) root         (0)     1487 2024-05-28 10:24:41.000000 py_async_grpc_prometheus-0.1.2/py_async_grpc_prometheus/grpc_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     7675 2024-05-28 10:24:41.000000 py_async_grpc_prometheus-0.1.2/py_async_grpc_prometheus/prometheus_async_client_interceptor.py
+-rwxrwxrwx   0 root         (0) root         (0)    10058 2024-05-28 11:19:15.000000 py_async_grpc_prometheus-0.1.2/py_async_grpc_prometheus/prometheus_async_server_interceptor.py
+-rwxrwxrwx   0 root         (0) root         (0)     2109 2024-05-28 10:24:41.000000 py_async_grpc_prometheus-0.1.2/py_async_grpc_prometheus/server_metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:19:24.097768 py_async_grpc_prometheus-0.1.2/py_async_grpc_prometheus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5591 2024-05-28 11:19:23.000000 py_async_grpc_prometheus-0.1.2/py_async_grpc_prometheus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      555 2024-05-28 11:19:23.000000 py_async_grpc_prometheus-0.1.2/py_async_grpc_prometheus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 11:19:23.000000 py_async_grpc_prometheus-0.1.2/py_async_grpc_prometheus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2024-05-28 11:19:23.000000 py_async_grpc_prometheus-0.1.2/py_async_grpc_prometheus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-28 11:19:23.000000 py_async_grpc_prometheus-0.1.2/py_async_grpc_prometheus.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 11:19:24.129157 py_async_grpc_prometheus-0.1.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      710 2024-05-28 11:19:15.000000 py_async_grpc_prometheus-0.1.2/setup.py
```

### Comparing `py_async_grpc_prometheus-0.1.1/LICENSE` & `py_async_grpc_prometheus-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_async_grpc_prometheus-0.1.1/PKG-INFO` & `py_async_grpc_prometheus-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_async_grpc_prometheus
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python async gRPC Prometheus Interceptors
 Home-page: https://github.com/taranisag/py-async-grpc-prometheus
 Author: Taranis
 Author-email: avi.klaiman@taranis.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools>=39.0.1
```

### Comparing `py_async_grpc_prometheus-0.1.1/README.md` & `py_async_grpc_prometheus-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `py_async_grpc_prometheus-0.1.1/py_async_grpc_prometheus/client_metrics.py` & `py_async_grpc_prometheus-0.1.2/py_async_grpc_prometheus/client_metrics.py`

 * *Files identical despite different names*

### Comparing `py_async_grpc_prometheus-0.1.1/py_async_grpc_prometheus/grpc_utils.py` & `py_async_grpc_prometheus-0.1.2/py_async_grpc_prometheus/grpc_utils.py`

 * *Files identical despite different names*

### Comparing `py_async_grpc_prometheus-0.1.1/py_async_grpc_prometheus/prometheus_async_client_interceptor.py` & `py_async_grpc_prometheus-0.1.2/py_async_grpc_prometheus/prometheus_async_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `py_async_grpc_prometheus-0.1.1/py_async_grpc_prometheus/prometheus_async_server_interceptor.py` & `py_async_grpc_prometheus-0.1.2/py_async_grpc_prometheus/prometheus_async_server_interceptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     self._grpc_server_handled_total_counter = server_metrics.get_grpc_server_handled_counter(
         self._legacy,
         registry
     )
     self._metrics = server_metrics.init_metrics(registry)
     self._skip_exceptions = skip_exceptions
     self._log_exceptions = log_exceptions
+    self._code_to_status_mapping = {x.value[0]: x for x in grpc.StatusCode}
 
   async def intercept_service(self, continuation, handler_call_details):
     """
     Intercepts the server function calls.
 
     This implements referred to:
     https://github.com/census-instrumentation/opencensus-python/blob/master/opencensus/
@@ -160,15 +161,16 @@
 
     return optional_any
 
   # pylint: disable=protected-access
   def _compute_status_code(self, servicer_context):
     if servicer_context.code() is None:
       return StatusCode.OK
-
+    elif isinstance(servicer_context.code(), int):
+      return self._code_to_status_mapping[servicer_context.code()]
     return servicer_context.code()
 
   def _compute_error_code(self, grpc_exception):
     if isinstance(grpc_exception, grpc.Call):
       return grpc_exception.code()
 
     return StatusCode.UNKNOWN
```

### Comparing `py_async_grpc_prometheus-0.1.1/py_async_grpc_prometheus/server_metrics.py` & `py_async_grpc_prometheus-0.1.2/py_async_grpc_prometheus/server_metrics.py`

 * *Files identical despite different names*

### Comparing `py_async_grpc_prometheus-0.1.1/py_async_grpc_prometheus.egg-info/PKG-INFO` & `py_async_grpc_prometheus-0.1.2/py_async_grpc_prometheus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_async_grpc_prometheus
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python async gRPC Prometheus Interceptors
 Home-page: https://github.com/taranisag/py-async-grpc-prometheus
 Author: Taranis
 Author-email: avi.klaiman@taranis.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools>=39.0.1
```

### Comparing `py_async_grpc_prometheus-0.1.1/py_async_grpc_prometheus.egg-info/SOURCES.txt` & `py_async_grpc_prometheus-0.1.2/py_async_grpc_prometheus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_async_grpc_prometheus-0.1.1/setup.py` & `py_async_grpc_prometheus-0.1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 from setuptools import setup
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setup(name="py_async_grpc_prometheus",
-      version="0.1.1",
+      version="0.1.2",
       description="Python async gRPC Prometheus Interceptors",
       long_description=long_description,
       long_description_content_type="text/markdown",
       author="Taranis",
       author_email="avi.klaiman@taranis.com",
       install_requires=[
           "setuptools>=39.0.1",
```

