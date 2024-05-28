# Comparing `tmp/drf_audit_trail-0.1.4.tar.gz` & `tmp/drf_audit_trail-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_audit_trail-0.1.4.tar", max compression
+gzip compressed data, was "drf_audit_trail-0.1.5.tar", max compression
```

## Comparing `drf_audit_trail-0.1.4.tar` & `drf_audit_trail-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1087 2024-05-22 13:39:48.438874 drf_audit_trail-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-05-08 01:49:41.058976 drf_audit_trail-0.1.4/drf_audit_trail/__init__.py
--rw-r--r--   0        0        0     1169 2024-05-21 21:34:03.481866 drf_audit_trail-0.1.4/drf_audit_trail/admin.py
--rw-r--r--   0        0        0      255 2024-05-10 20:28:23.293537 drf_audit_trail-0.1.4/drf_audit_trail/apps.py
--rw-r--r--   0        0        0        0 2024-05-08 23:42:25.366271 drf_audit_trail-0.1.4/drf_audit_trail/integrations/__init__.py
--rw-r--r--   0        0        0     1038 2024-05-21 23:07:13.612121 drf_audit_trail-0.1.4/drf_audit_trail/integrations/rest_framework_simplejwt.py
--rw-r--r--   0        0        0      106 2024-05-09 18:15:40.126054 drf_audit_trail-0.1.4/drf_audit_trail/managers/__init__.py
--rw-r--r--   0        0        0     1301 2024-05-09 18:19:21.825227 drf_audit_trail-0.1.4/drf_audit_trail/managers/request_audit_event_manager.py
--rw-r--r--   0        0        0      120 2024-05-09 01:34:50.633399 drf_audit_trail-0.1.4/drf_audit_trail/middleware/__init__.py
--rw-r--r--   0        0        0     5589 2024-05-21 23:03:26.544696 drf_audit_trail-0.1.4/drf_audit_trail/middleware/request_login_audit_event.py
--rw-r--r--   0        0        0     5511 2024-05-21 21:41:30.726036 drf_audit_trail-0.1.4/drf_audit_trail/migrations/0001_initial.py
--rw-r--r--   0        0        0      547 2024-05-22 01:12:33.248504 drf_audit_trail-0.1.4/drf_audit_trail/migrations/0002_alter_loginauditevent_request.py
--rw-r--r--   0        0        0        0 2024-05-08 01:49:41.058976 drf_audit_trail-0.1.4/drf_audit_trail/migrations/__init__.py
--rw-r--r--   0        0        0      433 2024-05-21 21:33:32.240334 drf_audit_trail-0.1.4/drf_audit_trail/mixins.py
--rw-r--r--   0        0        0      150 2024-05-09 17:52:36.716410 drf_audit_trail-0.1.4/drf_audit_trail/models/__init__.py
--rw-r--r--   0        0        0      792 2024-05-22 01:12:11.888359 drf_audit_trail-0.1.4/drf_audit_trail/models/login_audit_event.py
--rw-r--r--   0        0        0     1932 2024-05-21 22:15:20.337476 drf_audit_trail-0.1.4/drf_audit_trail/models/request_audit_event.py
--rw-r--r--   0        0        0      700 2024-05-10 00:12:08.881038 drf_audit_trail-0.1.4/drf_audit_trail/settings.py
--rw-r--r--   0        0        0       60 2024-05-08 01:49:41.058976 drf_audit_trail-0.1.4/drf_audit_trail/tests.py
--rw-r--r--   0        0        0      709 2024-05-09 18:22:22.004405 drf_audit_trail-0.1.4/drf_audit_trail/utils.py
--rw-r--r--   0        0        0      575 2024-05-22 13:39:55.458999 drf_audit_trail-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1837 1970-01-01 00:00:00.000000 drf_audit_trail-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-05-22 13:39:48.438874 drf_audit_trail-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 01:49:41.058976 drf_audit_trail-0.1.5/drf_audit_trail/__init__.py
+-rw-r--r--   0        0        0     1169 2024-05-28 13:08:30.611976 drf_audit_trail-0.1.5/drf_audit_trail/admin.py
+-rw-r--r--   0        0        0      255 2024-05-10 20:28:23.293537 drf_audit_trail-0.1.5/drf_audit_trail/apps.py
+-rw-r--r--   0        0        0        0 2024-05-08 23:42:25.366271 drf_audit_trail-0.1.5/drf_audit_trail/integrations/__init__.py
+-rw-r--r--   0        0        0     1038 2024-05-21 23:07:13.612121 drf_audit_trail-0.1.5/drf_audit_trail/integrations/rest_framework_simplejwt.py
+-rw-r--r--   0        0        0      106 2024-05-09 18:15:40.126054 drf_audit_trail-0.1.5/drf_audit_trail/managers/__init__.py
+-rw-r--r--   0        0        0     1301 2024-05-09 18:19:21.825227 drf_audit_trail-0.1.5/drf_audit_trail/managers/request_audit_event_manager.py
+-rw-r--r--   0        0        0      120 2024-05-09 01:34:50.633399 drf_audit_trail-0.1.5/drf_audit_trail/middleware/__init__.py
+-rw-r--r--   0        0        0     5595 2024-05-28 13:09:20.584473 drf_audit_trail-0.1.5/drf_audit_trail/middleware/request_login_audit_event.py
+-rw-r--r--   0        0        0     5511 2024-05-28 13:08:30.611976 drf_audit_trail-0.1.5/drf_audit_trail/migrations/0001_initial.py
+-rw-r--r--   0        0        0      547 2024-05-28 13:08:30.611976 drf_audit_trail-0.1.5/drf_audit_trail/migrations/0002_alter_loginauditevent_request.py
+-rw-r--r--   0        0        0        0 2024-05-08 01:49:41.058976 drf_audit_trail-0.1.5/drf_audit_trail/migrations/__init__.py
+-rw-r--r--   0        0        0      433 2024-05-21 21:33:32.240334 drf_audit_trail-0.1.5/drf_audit_trail/mixins.py
+-rw-r--r--   0        0        0      150 2024-05-09 17:52:36.716410 drf_audit_trail-0.1.5/drf_audit_trail/models/__init__.py
+-rw-r--r--   0        0        0      792 2024-05-22 01:12:11.888359 drf_audit_trail-0.1.5/drf_audit_trail/models/login_audit_event.py
+-rw-r--r--   0        0        0     1932 2024-05-28 13:08:30.611976 drf_audit_trail-0.1.5/drf_audit_trail/models/request_audit_event.py
+-rw-r--r--   0        0        0      700 2024-05-10 00:12:08.881038 drf_audit_trail-0.1.5/drf_audit_trail/settings.py
+-rw-r--r--   0        0        0       60 2024-05-08 01:49:41.058976 drf_audit_trail-0.1.5/drf_audit_trail/tests.py
+-rw-r--r--   0        0        0      709 2024-05-09 18:22:22.004405 drf_audit_trail-0.1.5/drf_audit_trail/utils.py
+-rw-r--r--   0        0        0      575 2024-05-28 13:09:38.512652 drf_audit_trail-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1837 1970-01-01 00:00:00.000000 drf_audit_trail-0.1.5/PKG-INFO
```

### Comparing `drf_audit_trail-0.1.4/README.md` & `drf_audit_trail-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.1.4/drf_audit_trail/admin.py` & `drf_audit_trail-0.1.5/drf_audit_trail/admin.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.1.4/drf_audit_trail/integrations/rest_framework_simplejwt.py` & `drf_audit_trail-0.1.5/drf_audit_trail/integrations/rest_framework_simplejwt.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.1.4/drf_audit_trail/managers/request_audit_event_manager.py` & `drf_audit_trail-0.1.5/drf_audit_trail/managers/request_audit_event_manager.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.1.4/drf_audit_trail/middleware/request_login_audit_event.py` & `drf_audit_trail-0.1.5/drf_audit_trail/middleware/request_login_audit_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                     method=self._method,
                     query_params=self._query_params,
                     ip_addresses=self._ip_addresses,
                     request_type=self._schema,
                     user=authenticated_user,
                     response_time=time() - self._start_time,
                     response_size=get_response_size(response),
-                    status_code=getattr(response, "status_code"),
+                    status_code=getattr(response, "status_code", None),
                     error_type=self.drf_request_audit_event.get("error_type"),
                     error_message=self.drf_request_audit_event.get("error_message"),
                     error_stacktrace=self.drf_request_audit_event.get(
                         "error_stacktrace"
                     ),
                     extra_informations=extra_informations,
                 )
```

### Comparing `drf_audit_trail-0.1.4/drf_audit_trail/migrations/0001_initial.py` & `drf_audit_trail-0.1.5/drf_audit_trail/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.1.4/drf_audit_trail/migrations/0002_alter_loginauditevent_request.py` & `drf_audit_trail-0.1.5/drf_audit_trail/migrations/0002_alter_loginauditevent_request.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.1.4/drf_audit_trail/models/login_audit_event.py` & `drf_audit_trail-0.1.5/drf_audit_trail/models/login_audit_event.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.1.4/drf_audit_trail/models/request_audit_event.py` & `drf_audit_trail-0.1.5/drf_audit_trail/models/request_audit_event.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.1.4/drf_audit_trail/settings.py` & `drf_audit_trail-0.1.5/drf_audit_trail/settings.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.1.4/drf_audit_trail/utils.py` & `drf_audit_trail-0.1.5/drf_audit_trail/utils.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.1.4/pyproject.toml` & `drf_audit_trail-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-audit-trail"
-version = "0.1.4"
+version = "0.1.5"
 description = "A reusable django [DRF] application that handles auditing of requests and logins"
 authors = ["Talismar Fernandes Costa <talismar788.una@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Talismar/drf-audit-trail"
 
 
 [tool.poetry.dependencies]
```

### Comparing `drf_audit_trail-0.1.4/PKG-INFO` & `drf_audit_trail-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-audit-trail
-Version: 0.1.4
+Version: 0.1.5
 Summary: A reusable django [DRF] application that handles auditing of requests and logins
 Home-page: https://github.com/Talismar/drf-audit-trail
 Author: Talismar Fernandes Costa
 Author-email: talismar788.una@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

