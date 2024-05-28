# Comparing `tmp/django-learngual-0.37.tar.gz` & `tmp/django_learngual-0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-learngual-0.37.tar", last modified: Sun Apr  7 11:37:18 2024, max compression
+gzip compressed data, was "django_learngual-0.38.tar", last modified: Tue May 28 08:05:08 2024, max compression
```

## Comparing `django-learngual-0.37.tar` & `django_learngual-0.38.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:37:18.949346 django-learngual-0.37/
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-07 11:36:20.000000 django-learngual-0.37/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-07 11:36:20.000000 django-learngual-0.37/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-07 11:37:18.949346 django-learngual-0.37/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-07 11:36:20.000000 django-learngual-0.37/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:37:18.949346 django-learngual-0.37/django_learngual.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-07 11:37:18.000000 django-learngual-0.37/django_learngual.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-07 11:37:18.000000 django-learngual-0.37/django_learngual.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 11:37:18.000000 django-learngual-0.37/django_learngual.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-07 11:37:18.000000 django-learngual-0.37/django_learngual.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:37:18.945345 django-learngual-0.37/learngual/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 11:37:17.000000 django-learngual-0.37/learngual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 11:37:17.000000 django-learngual-0.37/learngual/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:37:18.945345 django-learngual-0.37/learngual/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 11:37:17.000000 django-learngual-0.37/learngual/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 11:37:17.000000 django-learngual-0.37/learngual/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 11:37:17.000000 django-learngual-0.37/learngual/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-07 11:37:17.000000 django-learngual-0.37/learngual/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-04-07 11:37:17.000000 django-learngual-0.37/learngual/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-07 11:37:17.000000 django-learngual-0.37/learngual/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-07 11:37:17.000000 django-learngual-0.37/learngual/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-07 11:37:17.000000 django-learngual-0.37/learngual/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:37:18.945345 django-learngual-0.37/learngual/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 11:37:17.000000 django-learngual-0.37/learngual/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 11:37:17.000000 django-learngual-0.37/learngual/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-07 11:37:17.000000 django-learngual-0.37/learngual/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-07 11:37:17.000000 django-learngual-0.37/learngual/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-04-07 11:37:17.000000 django-learngual-0.37/learngual/service_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 11:37:17.000000 django-learngual-0.37/learngual/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:37:18.949346 django-learngual-0.37/learngual/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 11:37:17.000000 django-learngual-0.37/learngual/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 11:37:17.000000 django-learngual-0.37/learngual/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-07 11:37:17.000000 django-learngual-0.37/learngual/tests/request_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-07 11:37:17.000000 django-learngual-0.37/learngual/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 11:37:17.000000 django-learngual-0.37/learngual/tests/test_drf_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-04-07 11:37:17.000000 django-learngual-0.37/learngual/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-07 11:37:17.000000 django-learngual-0.37/learngual/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    20829 2024-04-07 11:37:17.000000 django-learngual-0.37/learngual/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-07 11:37:18.949346 django-learngual-0.37/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 11:36:20.000000 django-learngual-0.37/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:08.345072 django_learngual-0.38/
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-28 08:03:40.000000 django_learngual-0.38/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-28 08:03:40.000000 django_learngual-0.38/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-28 08:05:08.345072 django_learngual-0.38/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-28 08:03:40.000000 django_learngual-0.38/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:08.345072 django_learngual-0.38/django_learngual.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-28 08:05:08.000000 django_learngual-0.38/django_learngual.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-28 08:05:08.000000 django_learngual-0.38/django_learngual.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 08:05:08.000000 django_learngual-0.38/django_learngual.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 08:05:08.000000 django_learngual-0.38/django_learngual.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:08.341072 django_learngual-0.38/learngual/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9769 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/custom_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:08.341072 django_learngual-0.38/learngual/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/service_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:08.345072 django_learngual-0.38/learngual/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/tests/request_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/tests/test_drf_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20829 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:08.345072 django_learngual-0.38/learngual/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/v1/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:05:06.000000 django_learngual-0.38/learngual/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-28 08:05:08.345072 django_learngual-0.38/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 08:03:40.000000 django_learngual-0.38/setup.py
```

### Comparing `django-learngual-0.37/LICENSE` & `django_learngual-0.38/LICENSE`

 * *Files identical despite different names*

### Comparing `django-learngual-0.37/PKG-INFO` & `django_learngual-0.38/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.37
+Version: 0.38
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
```

### Comparing `django-learngual-0.37/README.rst` & `django_learngual-0.38/README.rst`

 * *Files identical despite different names*

### Comparing `django-learngual-0.37/django_learngual.egg-info/PKG-INFO` & `django_learngual-0.38/django_learngual.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.37
+Version: 0.38
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
```

### Comparing `django-learngual-0.37/learngual/apps.py` & `django_learngual-0.38/learngual/apps.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.37/learngual/authentication.py` & `django_learngual-0.38/learngual/authentication.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 from logging import getLogger
 
 import requests
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.db import models
 from django.utils.translation import gettext_lazy as _
-from rest_framework import authentication, exceptions
+from rest_framework import authentication
 from rest_framework.request import Request
 
+from . import custom_exceptions
+
 logger = getLogger(__file__)
 
 User = get_user_model()
 
 LEARNGUAL_SERVICE_API_KEY = getattr(
     settings, "LEARNGUAL_SERVICE_API_KEY", None
 ) or os.getenv("LEARNGUAL_SERVICE_API_KEY", None)
@@ -131,51 +133,49 @@
 
     @classmethod
     def get_query_str(cls, request: Request):
         return "?{query}".format(query=request.META.get("QUERY_STRING", ""))
 
     def authenticate(self, request):
         # this is for test mode
-
         service_key = str(
             request.META.get("HTTP_SERVICE_KEY", "")
             or request.GET.get("service-key", "")
             or request.GET.get("_service-key", "")
         )
         if service_key:
             logger.info("authentication send with service account")
             if service_key == LEARNGUAL_SERVICE_API_KEY:
                 service_user = User(id="service", username="service")
                 service_user.is_service = True
                 return service_user, service_key
-            logger.warn("invalid service key")
+            logger.warning("invalid service key")
             msg = _("Invalid service key")
-            raise exceptions.AuthenticationFailed(msg)
+            raise custom_exceptions.UnAuthenticated(msg)
 
         header = self.get_header(request)
         logger.info(
             "retrieve required authentication header during authentication -> %s",
             header,
         )
         if not header.get("authorization"):
-            logger.warn("no authorization")
-            return None
+            logger.warning("no authorization")
+            return
+
         headers = self.get_http_headers(request)
         logger.info("get django request header for forwarding -> %s", headers)
 
         query_str = self.get_query_str(request)
         logger.info("query string for forwarding -> %s", query_str)
         logger.info(f"{LEARNGUAL_AUTH_RETRIEVE_URL =}")
         res = requests.get(LEARNGUAL_AUTH_RETRIEVE_URL + query_str, headers=headers)
         if not res.ok:
-            logging.warn("request to IAM service did not go through")
-            return None
-        logging.info("verify auth response data -> %s", res.content)
+            logging.warning("request to IAM service did not go through")
+            raise custom_exceptions.UnAuthenticated("Service is down.")
         res_data = res.json()
-        logging.info("verify auth response json data -> %s", res_data)
         return (
             get_user(res_data),
             header.get("api_key") or header.get("authorization").split(" ")[-1],
         )
 
     def get_header(self, request):
         """
```

### Comparing `django-learngual-0.37/learngual/enums.py` & `django_learngual-0.38/learngual/enums.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.37/learngual/middleware.py` & `django_learngual-0.38/learngual/middleware.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.37/learngual/schema.py` & `django_learngual-0.38/learngual/schema.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.37/learngual/service_requests.py` & `django_learngual-0.38/learngual/service_requests.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.37/learngual/tests/request_mock.py` & `django_learngual-0.38/learngual/tests/request_mock.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.37/learngual/tests/test_authentication.py` & `django_learngual-0.38/learngual/tests/test_authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from unittest.mock import patch
 
 from django.contrib.auth import get_user_model
-from rest_framework import exceptions
 from rest_framework.test import APIClient, APIRequestFactory
 
+from .. import custom_exceptions
 from ..authentication import LearngualAuthentication, LearngualFakeAuthentication
 from .request_mock import requests as mock_requests
 
 factory = APIRequestFactory()
 User = get_user_model()
 
 
@@ -134,9 +134,9 @@
     # Create an instance of the custom authentication class
     auth = LearngualAuthentication()
 
     try:
         # Authenticate the request using the custom authentication class
         authenticated = auth.authenticate(request)
         assert authenticated
-    except exceptions.AuthenticationFailed:
+    except custom_exceptions.UnAuthenticated:
         assert True
```

### Comparing `django-learngual-0.37/learngual/tests/test_utils.py` & `django_learngual-0.38/learngual/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.37/learngual/utils.py` & `django_learngual-0.38/learngual/utils.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.37/setup.cfg` & `django_learngual-0.38/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-learngual
-version = 0.37
+version = 0.38
 author = learngual
 author_email = developer@leanrgual.com
 maintainer = Aniekutmfon
 maintainer_email = aniekutmfonekere@gmail.com
 description = Learngual helper package
 long_description = file:README.rst
 long_description_content_type = text/x-rst
```

