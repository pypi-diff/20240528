# Comparing `tmp/django_honeypot-1.1.0.tar.gz` & `tmp/django_honeypot-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_honeypot-1.1.0.tar", max compression
+gzip compressed data, was "django_honeypot-1.2.0.tar", max compression
```

## Comparing `django_honeypot-1.1.0.tar` & `django_honeypot-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1334 2023-11-17 21:03:54.457146 django_honeypot-1.1.0/LICENSE
--rw-r--r--   0        0        0     5658 2023-12-09 07:23:25.563226 django_honeypot-1.1.0/README.rst
--rw-r--r--   0        0        0       22 2023-12-09 07:28:29.916103 django_honeypot-1.1.0/honeypot/__init__.py
--rw-r--r--   0        0        0      244 2023-12-09 07:23:25.563373 django_honeypot-1.1.0/honeypot/apps.py
--rw-r--r--   0        0        0      902 2023-12-09 07:23:25.563505 django_honeypot-1.1.0/honeypot/checks.py
--rw-r--r--   0        0        0     2192 2023-11-17 21:16:57.697343 django_honeypot-1.1.0/honeypot/decorators.py
--rw-r--r--   0        0        0     2623 2023-11-17 21:15:37.571405 django_honeypot-1.1.0/honeypot/middleware.py
--rw-r--r--   0        0        0      113 2023-11-17 21:03:54.457721 django_honeypot-1.1.0/honeypot/templates/honeypot/honeypot_error.html
--rw-r--r--   0        0        0      262 2023-11-17 21:03:54.457828 django_honeypot-1.1.0/honeypot/templates/honeypot/honeypot_field.html
--rw-r--r--   0        0        0        0 2023-11-17 21:03:54.457908 django_honeypot-1.1.0/honeypot/templatetags/__init__.py
--rw-r--r--   0        0        0      515 2023-11-17 21:03:54.458003 django_honeypot-1.1.0/honeypot/templatetags/honeypot.py
--rw-r--r--   0        0        0     9100 2023-12-09 07:23:25.563696 django_honeypot-1.1.0/honeypot/tests.py
--rw-r--r--   0        0        0     1525 2023-12-09 07:28:08.239182 django_honeypot-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6787 1970-01-01 00:00:00.000000 django_honeypot-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1334 2023-11-17 21:03:54.457146 django_honeypot-1.2.0/LICENSE
+-rw-r--r--   0        0        0     6503 2024-05-28 18:11:42.008855 django_honeypot-1.2.0/README.rst
+-rw-r--r--   0        0        0       22 2023-12-09 07:28:29.916103 django_honeypot-1.2.0/honeypot/__init__.py
+-rw-r--r--   0        0        0      244 2023-12-09 07:23:25.563373 django_honeypot-1.2.0/honeypot/apps.py
+-rw-r--r--   0        0        0      902 2023-12-09 07:23:25.563505 django_honeypot-1.2.0/honeypot/checks.py
+-rw-r--r--   0        0        0     2450 2024-05-28 18:11:42.009788 django_honeypot-1.2.0/honeypot/decorators.py
+-rw-r--r--   0        0        0     2623 2023-11-17 21:15:37.571405 django_honeypot-1.2.0/honeypot/middleware.py
+-rw-r--r--   0        0        0      113 2023-11-17 21:03:54.457721 django_honeypot-1.2.0/honeypot/templates/honeypot/honeypot_error.html
+-rw-r--r--   0        0        0      262 2023-11-17 21:03:54.457828 django_honeypot-1.2.0/honeypot/templates/honeypot/honeypot_field.html
+-rw-r--r--   0        0        0        0 2023-11-17 21:03:54.457908 django_honeypot-1.2.0/honeypot/templatetags/__init__.py
+-rw-r--r--   0        0        0      515 2023-11-17 21:03:54.458003 django_honeypot-1.2.0/honeypot/templatetags/honeypot.py
+-rw-r--r--   0        0        0     9658 2024-05-28 18:21:45.902480 django_honeypot-1.2.0/honeypot/tests.py
+-rw-r--r--   0        0        0     1398 2024-05-28 18:19:58.972013 django_honeypot-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7683 1970-01-01 00:00:00.000000 django_honeypot-1.2.0/PKG-INFO
```

### Comparing `django_honeypot-1.1.0/LICENSE` & `django_honeypot-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_honeypot-1.1.0/README.rst` & `django_honeypot-1.2.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 
 You will almost always need to define ``HONEYPOT_FIELD_NAME`` which is the name to use for the honeypot field.  Some sophisticated bots will attempt to avoid fields named honeypot, so it may be wise to name the field something slightly more realistic such as "phonenumber" or "body2".
 
 ``HONEYPOT_VALUE`` is an option that you can specify to populate the honeypot field, by default the honeypot field will be empty and any text entered into it will result in a failed POST.  ``HONEYPOT_VALUE`` can be a string or a callable that takes no arguments.
 
 ``HONEYPOT_VERIFIER`` is an advanced option that you can specify to validate the honeypot.  The default verifier ensures that the contents of the honeypot field matches ``HONEYPOT_VALUE``.  Using a combination of a callable for ``HONEYPOT_VALUE`` and ``HONEYPOT_VERIFIER`` it is possible to implement a more advanced technique such as using timestamps.
 
+``HONEYPOT_RESPONDER`` can be used to replace the default response in case of an invalid honeypot.
+
 Adding honeypot fields to specific forms and views
 --------------------------------------------------
 
 It is possible to add honeypot fields to specific forms and ensure that specific views check for a valid honeypotin ``request.POST``.  This can be accomplished by using the ``render_honeypot_field`` template tag:
 
 At the top of a template file include the line::
 
@@ -69,18 +71,18 @@
 Adding honeypot fields to class-based-views
 -------------------------------------------
 
 The same as above for `Adding honeypot fields to specific forms and views`_ but add the decorator to the post method making use of django's `method_decorator <https://docs.djangoproject.com/en/3.2/topics/class-based-views/intro/#decorating-the-class>`_.
 
 
 .. code:: python
-    
+
     from django.utils.decorators import method_decorator
     from honeypot.decorators import check_honeypot
-    
+
     @method_decorator(check_honeypot, name='post')
     class MyView(FormView):
         ...
 
 Adding honeypot fields site-wide
 --------------------------------
 
@@ -99,7 +101,28 @@
 
 There are two templates used by django-honeypot that can be used to control various aspects of how the honeypot functionality is presented to the user.
 
 ``honeypot/honeypot_field.html`` is used to render the honeypot field.  It is given two context variables ``fieldname`` and ``value``, corresponding to ``HONEYPOT_FIELD_NAME`` and ``HONEYPOT_VALUE`` or any overrides in effect (such as a custom field name passed to the template tag).
 
 ``honeypot/honeypot_error.html`` is the error page rendered when a bad request is intercepted.  It is given the context variable ``fieldname`` representing the name of the honeypot field.
 
+To completely change the error page or what happens when a bad request is intercepted set ``HONEYPOT_RESPONDER`` to a function accepting ``request`` and ``context`` kwargs and returning a ``HttpResponse``.
+
+.. code:: python
+
+    # mypackage.py
+    from honeypot.decorators import honeypot_error
+
+    def custom_honeypot_error(request, context):
+        # custom responder logging the event
+        log.warning("gotcha!")
+        # call built-in responder to send default HttpResponseBadRequest
+        return honeypot_error(request, context)
+        # or ...
+        # raise Http404
+
+.. code:: python
+
+    # settings.py
+    from django.utils.module_loading import import_string
+
+    HONEYPOT_RESPONDER = import_string('mypackage.custom_honeypot_error')
```

### Comparing `django_honeypot-1.1.0/honeypot/checks.py` & `django_honeypot-1.2.0/honeypot/checks.py`

 * *Files identical despite different names*

### Comparing `django_honeypot-1.1.0/honeypot/decorators.py` & `django_honeypot-1.2.0/honeypot/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,31 +12,40 @@
     """
     expected = getattr(settings, "HONEYPOT_VALUE", "")
     if callable(expected):
         expected = expected()
     return val == expected
 
 
+def honeypot_error(request, context):
+    """
+    Default responder used if HONEYPOT_RESPONDER is not specified.
+    Return HttpResponseBadRequest for invalid honeypot.
+    """
+    resp = render_to_string(
+        "honeypot/honeypot_error.html",
+        context=context,
+        request=request,
+    )
+    return HttpResponseBadRequest(resp)
+
+
 def verify_honeypot_value(request, field_name):
     """
     Verify that request.POST[field_name] is a valid honeypot.
 
     Ensures that the field exists and passes verification according to
     HONEYPOT_VERIFIER.
     """
     verifier = getattr(settings, "HONEYPOT_VERIFIER", honeypot_equals)
+    responder = getattr(settings, "HONEYPOT_RESPONDER", honeypot_error)
     if request.method == "POST":
         field = field_name or settings.HONEYPOT_FIELD_NAME
         if field not in request.POST or not verifier(request.POST[field]):
-            resp = render_to_string(
-                "honeypot/honeypot_error.html",
-                {"fieldname": field},
-                request=request,
-            )
-            return HttpResponseBadRequest(resp)
+            return responder(request, {"fieldname": field})
     return None
 
 
 def check_honeypot(func=None, field_name=None):
     """
     Check request.POST for valid honeypot field.
```

### Comparing `django_honeypot-1.1.0/honeypot/middleware.py` & `django_honeypot-1.2.0/honeypot/middleware.py`

 * *Files identical despite different names*

### Comparing `django_honeypot-1.1.0/honeypot/templatetags/honeypot.py` & `django_honeypot-1.2.0/honeypot/templatetags/honeypot.py`

 * *Files identical despite different names*

### Comparing `django_honeypot-1.1.0/honeypot/tests.py` & `django_honeypot-1.2.0/honeypot/tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 from django.conf import settings
 from django.core import checks
-from django.http import HttpRequest, HttpResponse, HttpResponseBadRequest
+from django.http import (
+    HttpRequest,
+    HttpResponse,
+    HttpResponseBadRequest,
+    HttpResponseNotFound,
+)
 from django.template import Context, Template
 from django.template.loader import render_to_string
 from django.test import TestCase, override_settings
 
 from honeypot.checks import check_middleware_order
 from honeypot.decorators import check_honeypot, honeypot_exempt, verify_honeypot_value
 from honeypot.middleware import HoneypotResponseMiddleware, HoneypotViewMiddleware
 
 
-def _get_GET_request():
+def _get_GET_request():  # noqa: N802
     return HttpRequest()
 
 
-def _get_POST_request():
+def _get_POST_request():  # noqa: N802
     req = HttpRequest()
     req.method = "POST"
     return req
 
 
 def view_func(request):
     return HttpResponse()
@@ -26,14 +31,16 @@
 
 class HoneypotTestCase(TestCase):
     def setUp(self):
         if hasattr(settings, "HONEYPOT_VALUE"):
             delattr(settings, "HONEYPOT_VALUE")
         if hasattr(settings, "HONEYPOT_VERIFIER"):
             delattr(settings, "HONEYPOT_VERIFIER")
+        if hasattr(settings, "HONEYPOT_RESPONDER"):
+            delattr(settings, "HONEYPOT_RESPONDER")
         settings.HONEYPOT_FIELD_NAME = "honeypot"
 
 
 class VerifyHoneypotValue(HoneypotTestCase):
     def test_no_call_on_get(self):
         """test that verify_honeypot_value is not called when request.method == GET"""
         request = _get_GET_request()
@@ -45,37 +52,46 @@
         request = _get_POST_request()
         request.POST[settings.HONEYPOT_FIELD_NAME] = ""
         settings.HONEYPOT_VERIFIER = lambda x: False
         resp = verify_honeypot_value(request, None)
         self.assertEqual(resp.__class__, HttpResponseBadRequest)
 
     def test_field_missing(self):
-        """test that verify_honeypot_value succeeds when HONEYPOT_FIELD_NAME is missing from
+        """test that verify_honeypot_value fails when HONEYPOT_FIELD_NAME is missing from
         request.POST"""
         request = _get_POST_request()
         resp = verify_honeypot_value(request, None)
         self.assertEqual(resp.__class__, HttpResponseBadRequest)
 
+    def test_custom_responder(self):
+        """test custom response, when verify_honeypot_value fails"""
+        request = _get_POST_request()
+        settings.HONEYPOT_RESPONDER = lambda x, y: HttpResponseNotFound()
+        resp = verify_honeypot_value(request, None)
+        self.assertEqual(resp.__class__, HttpResponseNotFound)
+
     def test_field_blank(self):
         """test that verify_honeypot_value succeeds when HONEYPOT_VALUE is blank"""
         request = _get_POST_request()
         request.POST[settings.HONEYPOT_FIELD_NAME] = ""
         resp = verify_honeypot_value(request, None)
         self.assertEqual(resp, None)
 
     def test_honeypot_value_string(self):
-        """test that verify_honeypot_value succeeds when HONEYPOT_VALUE is a string"""
+        """test that verify_honeypot_value succeeds when HONEYPOT_VALUE is the expected
+        string"""
         request = _get_POST_request()
         settings.HONEYPOT_VALUE = "(test string)"
         request.POST[settings.HONEYPOT_FIELD_NAME] = settings.HONEYPOT_VALUE
         resp = verify_honeypot_value(request, None)
         self.assertEqual(resp, None)
 
     def test_honeypot_value_callable(self):
-        """test that verify_honeypot_value succeeds when HONEYPOT_VALUE is a callable"""
+        """test that verify_honeypot_value succeeds when HONEYPOT_VALUE is the expected
+        return value of a callable"""
         request = _get_POST_request()
         settings.HONEYPOT_VALUE = lambda: "(test string)"
         request.POST[settings.HONEYPOT_FIELD_NAME] = settings.HONEYPOT_VALUE()
         resp = verify_honeypot_value(request, None)
         self.assertEqual(resp, None)
 
 
@@ -158,15 +174,15 @@
     def test_response_middleware_rewrite(self):
         """ensure POST forms are rewritten"""
         request = _get_POST_request()
         request.POST[settings.HONEYPOT_FIELD_NAME] = ""
         response = HttpResponse(self._response_body)
         HoneypotResponseMiddleware(lambda request: response)(request)
         self.assertNotContains(response, self._response_body)
-        self.assertContains(response, 'name="%s"' % settings.HONEYPOT_FIELD_NAME)
+        self.assertContains(response, f'name="{settings.HONEYPOT_FIELD_NAME}"')
 
     def test_response_middleware_contenttype_exclusion(self):
         """ensure POST forms are not rewritten for non-html content types"""
         request = _get_POST_request()
         request.POST[settings.HONEYPOT_FIELD_NAME] = ""
         response = HttpResponse(self._response_body, content_type="text/javascript")
         HoneypotResponseMiddleware(lambda request: response)(request)
@@ -175,15 +191,15 @@
     def test_response_middleware_unicode(self):
         """ensure that POST form rewriting works with unicode templates"""
         request = _get_GET_request()
         unicode_body = "\u2603" + self._response_body  # add unicode snowman
         response = HttpResponse(unicode_body)
         HoneypotResponseMiddleware(lambda request: response)(request)
         self.assertNotContains(response, unicode_body)
-        self.assertContains(response, 'name="%s"' % settings.HONEYPOT_FIELD_NAME)
+        self.assertContains(response, f'name="{settings.HONEYPOT_FIELD_NAME}"')
 
     def test_exempt_view(self):
         """call view no matter what if view is exempt"""
         request = _get_POST_request()
         exempt_view_func = honeypot_exempt(view_func)
         assert exempt_view_func.honeypot_exempt is True
         retval = HoneypotViewMiddleware(lambda request: None).process_view(
```

### Comparing `django_honeypot-1.1.0/pyproject.toml` & `django_honeypot-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "django-honeypot"
 packages = [
      { include = "honeypot" },
 ]
-version = "1.1.0"
+version = "1.2.0"
 description = "Django honeypot field utilities"
 authors = ["James Turk <dev@jamesturk.net>"]
 license = "BSD-2-Clause"
 readme = "README.rst"
 repository = "https://github.com/jamesturk/django-honeypot/"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -23,27 +23,27 @@
 ]
 
 [tool.poetry.dependencies]
 Django = ">=3.2,<5.1"
 python = "^3.8"
 
 [tool.poetry.dev-dependencies]
-black = "^23.1.0"
-ruff = "^0.1.6"
+black = "^24.1.1"
+ruff = "^0.4.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
-select = [
+lint.select = [
     "A",
     "B",
     "BLE",
-    "C4",
+    "C40",
     "C90",
     "DJ",
     "DTZ",
     "E",
     "EM",
     "ERA",
     "EXE",
@@ -61,26 +61,20 @@
     "PIE",
     "PL",
     "PTH",
     "PYI",
     "Q",
     "RSE",
     "RUF",
-    "S",
     "SIM",
     "SLF",
     "T10",
     "T20",
     "TCH",
     "TID",
     "TRY",
     "UP",
     "W",
     "YTT"
 ]
 line-length = 93
 target-version = "py37"
-
-[tool.ruff.per-file-ignores]
-"honeypot/middleware.py" = ["S308"]
-"honeypot/tests.py" = ["N802"]
-"test*" = ["S101", "S105"]
```

### Comparing `django_honeypot-1.1.0/PKG-INFO` & `django_honeypot-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-honeypot
-Version: 1.1.0
+Version: 1.2.0
 Summary: Django honeypot field utilities
 Home-page: https://github.com/jamesturk/django-honeypot/
 License: BSD-2-Clause
 Author: James Turk
 Author-email: dev@jamesturk.net
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,14 +19,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Django (>=3.2,<5.1)
 Project-URL: Repository, https://github.com/jamesturk/django-honeypot/
 Description-Content-Type: text/x-rst
 
 ===============
 django-honeypot
 ===============
@@ -60,14 +61,16 @@
 
 You will almost always need to define ``HONEYPOT_FIELD_NAME`` which is the name to use for the honeypot field.  Some sophisticated bots will attempt to avoid fields named honeypot, so it may be wise to name the field something slightly more realistic such as "phonenumber" or "body2".
 
 ``HONEYPOT_VALUE`` is an option that you can specify to populate the honeypot field, by default the honeypot field will be empty and any text entered into it will result in a failed POST.  ``HONEYPOT_VALUE`` can be a string or a callable that takes no arguments.
 
 ``HONEYPOT_VERIFIER`` is an advanced option that you can specify to validate the honeypot.  The default verifier ensures that the contents of the honeypot field matches ``HONEYPOT_VALUE``.  Using a combination of a callable for ``HONEYPOT_VALUE`` and ``HONEYPOT_VERIFIER`` it is possible to implement a more advanced technique such as using timestamps.
 
+``HONEYPOT_RESPONDER`` can be used to replace the default response in case of an invalid honeypot.
+
 Adding honeypot fields to specific forms and views
 --------------------------------------------------
 
 It is possible to add honeypot fields to specific forms and ensure that specific views check for a valid honeypotin ``request.POST``.  This can be accomplished by using the ``render_honeypot_field`` template tag:
 
 At the top of a template file include the line::
 
@@ -98,18 +101,18 @@
 Adding honeypot fields to class-based-views
 -------------------------------------------
 
 The same as above for `Adding honeypot fields to specific forms and views`_ but add the decorator to the post method making use of django's `method_decorator <https://docs.djangoproject.com/en/3.2/topics/class-based-views/intro/#decorating-the-class>`_.
 
 
 .. code:: python
-    
+
     from django.utils.decorators import method_decorator
     from honeypot.decorators import check_honeypot
-    
+
     @method_decorator(check_honeypot, name='post')
     class MyView(FormView):
         ...
 
 Adding honeypot fields site-wide
 --------------------------------
 
@@ -128,8 +131,29 @@
 
 There are two templates used by django-honeypot that can be used to control various aspects of how the honeypot functionality is presented to the user.
 
 ``honeypot/honeypot_field.html`` is used to render the honeypot field.  It is given two context variables ``fieldname`` and ``value``, corresponding to ``HONEYPOT_FIELD_NAME`` and ``HONEYPOT_VALUE`` or any overrides in effect (such as a custom field name passed to the template tag).
 
 ``honeypot/honeypot_error.html`` is the error page rendered when a bad request is intercepted.  It is given the context variable ``fieldname`` representing the name of the honeypot field.
 
+To completely change the error page or what happens when a bad request is intercepted set ``HONEYPOT_RESPONDER`` to a function accepting ``request`` and ``context`` kwargs and returning a ``HttpResponse``.
+
+.. code:: python
+
+    # mypackage.py
+    from honeypot.decorators import honeypot_error
+
+    def custom_honeypot_error(request, context):
+        # custom responder logging the event
+        log.warning("gotcha!")
+        # call built-in responder to send default HttpResponseBadRequest
+        return honeypot_error(request, context)
+        # or ...
+        # raise Http404
+
+.. code:: python
+
+    # settings.py
+    from django.utils.module_loading import import_string
+
+    HONEYPOT_RESPONDER = import_string('mypackage.custom_honeypot_error')
```

