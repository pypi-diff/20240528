# Comparing `tmp/Authomatic-1.2.1.tar.gz` & `tmp/authomatic-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Authomatic-1.2.1.tar", last modified: Thu Jun  8 18:08:22 2023, max compression
+gzip compressed data, was "authomatic-1.3.0.tar", last modified: Tue May 28 14:05:55 2024, max compression
```

## Comparing `Authomatic-1.2.1.tar` & `authomatic-1.3.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:08:22.898323 Authomatic-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:08:22.894323 Authomatic-1.2.1/Authomatic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-06-08 18:08:22.000000 Authomatic-1.2.1/Authomatic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-08 18:08:22.000000 Authomatic-1.2.1/Authomatic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:08:22.000000 Authomatic-1.2.1/Authomatic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-08 18:08:22.000000 Authomatic-1.2.1/Authomatic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 18:08:22.000000 Authomatic-1.2.1/Authomatic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-06-08 18:07:16.000000 Authomatic-1.2.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-08 18:07:16.000000 Authomatic-1.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-08 18:07:16.000000 Authomatic-1.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-08 18:07:16.000000 Authomatic-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-06-08 18:08:22.898323 Authomatic-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-08 18:07:16.000000 Authomatic-1.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-08 18:07:16.000000 Authomatic-1.2.1/RELEASE.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:08:22.894323 Authomatic-1.2.1/authomatic/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-08 18:07:16.000000 Authomatic-1.2.1/authomatic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-06-08 18:07:16.000000 Authomatic-1.2.1/authomatic/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)    53269 2023-06-08 18:07:16.000000 Authomatic-1.2.1/authomatic/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-08 18:07:16.000000 Authomatic-1.2.1/authomatic/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:08:22.894323 Authomatic-1.2.1/authomatic/extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:07:16.000000 Authomatic-1.2.1/authomatic/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-08 18:07:16.000000 Authomatic-1.2.1/authomatic/extras/flask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:08:22.894323 Authomatic-1.2.1/authomatic/extras/gae/
--rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-06-08 18:07:16.000000 Authomatic-1.2.1/authomatic/extras/gae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-06-08 18:07:16.000000 Authomatic-1.2.1/authomatic/extras/gae/openid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-08 18:07:16.000000 Authomatic-1.2.1/authomatic/extras/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:08:22.898323 Authomatic-1.2.1/authomatic/providers/
--rw-r--r--   0 runner    (1001) docker     (123)    30309 2023-06-08 18:07:16.000000 Authomatic-1.2.1/authomatic/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-06-08 18:07:16.000000 Authomatic-1.2.1/authomatic/providers/gaeopenid.py
--rw-r--r--   0 runner    (1001) docker     (123)    38857 2023-06-08 18:07:16.000000 Authomatic-1.2.1/authomatic/providers/oauth1.py
--rw-r--r--   0 runner    (1001) docker     (123)    61564 2023-06-08 18:07:16.000000 Authomatic-1.2.1/authomatic/providers/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17262 2023-06-08 18:07:16.000000 Authomatic-1.2.1/authomatic/providers/openid.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-08 18:07:16.000000 Authomatic-1.2.1/authomatic/providers/persona.py
--rw-r--r--   0 runner    (1001) docker     (123)    29751 2023-06-08 18:07:16.000000 Authomatic-1.2.1/authomatic/six.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-08 18:07:16.000000 Authomatic-1.2.1/config-template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:08:22.898323 Authomatic-1.2.1/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)    16582 2023-06-08 18:07:16.000000 Authomatic-1.2.1/javascript/authomatic.js
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-06-08 18:07:16.000000 Authomatic-1.2.1/javascript/authomatic.map
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-08 18:08:22.898323 Authomatic-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-08 18:07:16.000000 Authomatic-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:05:55.301877 authomatic-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:05:55.301877 authomatic-1.3.0/Authomatic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-05-28 14:05:55.000000 authomatic-1.3.0/Authomatic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-28 14:05:55.000000 authomatic-1.3.0/Authomatic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:05:55.000000 authomatic-1.3.0/Authomatic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-28 14:05:55.000000 authomatic-1.3.0/Authomatic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-28 14:05:55.000000 authomatic-1.3.0/Authomatic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-05-28 14:05:18.000000 authomatic-1.3.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-28 14:05:18.000000 authomatic-1.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-28 14:05:18.000000 authomatic-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-28 14:05:18.000000 authomatic-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-05-28 14:05:55.301877 authomatic-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-28 14:05:18.000000 authomatic-1.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-28 14:05:18.000000 authomatic-1.3.0/RELEASE.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:05:55.297877 authomatic-1.3.0/authomatic/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-28 14:05:18.000000 authomatic-1.3.0/authomatic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-28 14:05:18.000000 authomatic-1.3.0/authomatic/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53208 2024-05-28 14:05:18.000000 authomatic-1.3.0/authomatic/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-28 14:05:18.000000 authomatic-1.3.0/authomatic/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:05:55.297877 authomatic-1.3.0/authomatic/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:05:18.000000 authomatic-1.3.0/authomatic/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-28 14:05:18.000000 authomatic-1.3.0/authomatic/extras/flask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:05:55.297877 authomatic-1.3.0/authomatic/extras/gae/
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-05-28 14:05:18.000000 authomatic-1.3.0/authomatic/extras/gae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-05-28 14:05:18.000000 authomatic-1.3.0/authomatic/extras/gae/openid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-28 14:05:18.000000 authomatic-1.3.0/authomatic/extras/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:05:55.301877 authomatic-1.3.0/authomatic/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)    32339 2024-05-28 14:05:18.000000 authomatic-1.3.0/authomatic/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-28 14:05:18.000000 authomatic-1.3.0/authomatic/providers/gaeopenid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38857 2024-05-28 14:05:18.000000 authomatic-1.3.0/authomatic/providers/oauth1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62147 2024-05-28 14:05:18.000000 authomatic-1.3.0/authomatic/providers/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17262 2024-05-28 14:05:18.000000 authomatic-1.3.0/authomatic/providers/openid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-28 14:05:18.000000 authomatic-1.3.0/authomatic/providers/persona.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34549 2024-05-28 14:05:18.000000 authomatic-1.3.0/authomatic/six.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-28 14:05:18.000000 authomatic-1.3.0/config-template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:05:55.301877 authomatic-1.3.0/javascript/
+-rw-r--r--   0 runner    (1001) docker     (127)    16582 2024-05-28 14:05:18.000000 authomatic-1.3.0/javascript/authomatic.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-05-28 14:05:18.000000 authomatic-1.3.0/javascript/authomatic.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-28 14:05:55.301877 authomatic-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-28 14:05:18.000000 authomatic-1.3.0/setup.py
```

### Comparing `Authomatic-1.2.1/Authomatic.egg-info/PKG-INFO` & `authomatic-1.3.0/Authomatic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Authomatic
-Version: 1.2.1
+Version: 1.3.0
 Summary: Authorization / authentication client library for Python web applications
 Author: Peter Hudec
 Author-email: peterhudec@peterhudec.com
 Maintainer: Authomatic Project Community
 Maintainer-email: authomaticproject@protonmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/authomatic/authomatic/issues
@@ -21,16 +21,18 @@
 Classifier: Programming Language :: JavaScript
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: CGI Tools/Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Provides-Extra: OpenID
 License-File: LICENSE.txt
+Provides-Extra: openid
+Requires-Dist: python-openid; python_version < "3" and extra == "openid"
+Requires-Dist: python3-openid; python_version >= "3" and extra == "openid"
 
 .. |gae| replace:: Google App Engine
 .. _gae: https://developers.google.com/appengine/
 
 .. |webapp2| replace:: Webapp2
 .. _webapp2: http://webapp-improved.appspot.com/
```

### Comparing `Authomatic-1.2.1/Authomatic.egg-info/SOURCES.txt` & `authomatic-1.3.0/Authomatic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Authomatic-1.2.1/CHANGES.rst` & `authomatic-1.3.0/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `Authomatic-1.2.1/LICENSE.txt` & `authomatic-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Authomatic-1.2.1/PKG-INFO` & `authomatic-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Authomatic
-Version: 1.2.1
+Version: 1.3.0
 Summary: Authorization / authentication client library for Python web applications
 Author: Peter Hudec
 Author-email: peterhudec@peterhudec.com
 Maintainer: Authomatic Project Community
 Maintainer-email: authomaticproject@protonmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/authomatic/authomatic/issues
@@ -21,16 +21,18 @@
 Classifier: Programming Language :: JavaScript
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: CGI Tools/Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Systems Administration :: Authentication/Directory
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Provides-Extra: OpenID
 License-File: LICENSE.txt
+Provides-Extra: openid
+Requires-Dist: python-openid; python_version < "3" and extra == "openid"
+Requires-Dist: python3-openid; python_version >= "3" and extra == "openid"
 
 .. |gae| replace:: Google App Engine
 .. _gae: https://developers.google.com/appengine/
 
 .. |webapp2| replace:: Webapp2
 .. _webapp2: http://webapp-improved.appspot.com/
```

### Comparing `Authomatic-1.2.1/README.rst` & `authomatic-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `Authomatic-1.2.1/RELEASE.rst` & `authomatic-1.3.0/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `Authomatic-1.2.1/authomatic/adapters.py` & `authomatic-1.3.0/authomatic/adapters.py`

 * *Files identical despite different names*

### Comparing `Authomatic-1.2.1/authomatic/core.py` & `authomatic-1.3.0/authomatic/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1324,18 +1324,15 @@
         self.session = session
         self.session_save_method = session_save_method
         self.report_errors = report_errors
         self.debug = debug
         self.logging_level = logging_level
         self.prefix = prefix
         self._logger = logger or logging.getLogger(str(id(self)))
-
-        # Set logging level.
-        if logger is None:
-            self._logger.setLevel(logging_level)
+        self._logger.setLevel(logging_level)
 
     def login(self, adapter, provider_name, callback=None,
               session=None, session_saver=None, **kwargs):
         """
         If :data:`provider_name` specified, launches the login procedure for
         corresponding :doc:`provider </reference/providers>` and returns
         :class:`.LoginResult`.
```

### Comparing `Authomatic-1.2.1/authomatic/exceptions.py` & `authomatic-1.3.0/authomatic/exceptions.py`

 * *Files identical despite different names*

### Comparing `Authomatic-1.2.1/authomatic/extras/flask.py` & `authomatic-1.3.0/authomatic/extras/flask.py`

 * *Files identical despite different names*

### Comparing `Authomatic-1.2.1/authomatic/extras/gae/__init__.py` & `authomatic-1.3.0/authomatic/extras/gae/__init__.py`

 * *Files identical despite different names*

### Comparing `Authomatic-1.2.1/authomatic/extras/gae/openid.py` & `authomatic-1.3.0/authomatic/extras/gae/openid.py`

 * *Files identical despite different names*

### Comparing `Authomatic-1.2.1/authomatic/extras/interfaces.py` & `authomatic-1.3.0/authomatic/extras/interfaces.py`

 * *Files identical despite different names*

### Comparing `Authomatic-1.2.1/authomatic/providers/__init__.py` & `authomatic-1.3.0/authomatic/providers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,27 +20,27 @@
 """
 
 import abc
 import base64
 import hashlib
 import logging
 import random
+import ssl
 import sys
 import traceback
 import uuid
 
 import authomatic.core
 from authomatic.exceptions import (
     ConfigError,
     FetchError,
     CredentialsError,
 )
 from authomatic import six
-from authomatic.six.moves import urllib_parse as parse
-from authomatic.six.moves import http_client
+from authomatic.six.moves import urllib_parse as parse, http_client
 from authomatic.exceptions import CancellationError
 
 __all__ = [
     'BaseProvider',
     'AuthorizationProvider',
     'AuthenticationProvider',
     'login_decorator']
@@ -276,19 +276,26 @@
 
         :param dict kwargs:
             Keyword arguments dictionary.
         :param str kwname:
             Name of the desired keyword argument.
 
         """
-
-        return kwargs.get(kwname) or \
-            self.settings.config.get(self.name, {}).get(kwname) or \
-            self.settings.config.get('__defaults__', {}).get(kwname) or \
-            default
+        # check against `None` instead of multiple 'or' in case default value
+        # is `False`, which could be considered a valid 'found' value
+        getters = [
+            lambda: kwargs.get(kwname),
+            lambda: self.settings.config.get(self.name, {}).get(kwname),
+            lambda: self.settings.config.get('__defaults__', {}).get(kwname),
+        ]
+        for get in getters:
+            value = get()
+            if value is not None:
+                return value
+        return default
 
     def _session_key(self, key):
         """
         Generates session key string.
 
         :param str key:
             e.g. ``"authomatic:facebook:key"``
@@ -348,16 +355,44 @@
         """
 
         logger = getattr(cls, '_logger', None) or authomatic.core._logger
         logger.log(
             level, ': '.join(
                 ('authomatic', cls.__name__, msg)), **kwargs)
 
+    @classmethod
+    def _log_param(cls, param, value='', last=None,
+                   level=logging.DEBUG, **kwargs):
+        """
+        Same as :meth:`_log` but in DEBUG, and with option indicator in front
+        of the message according to :param:`last`.
+
+        :param str param:
+            Parameter name.
+
+        :param Any value:
+            Parameter value.
+
+        :param bool last:
+            "|-" like character if `False`, "|_" if `True`, None if `None`.
+
+        :param int level:
+            Logging level as specified in the
+            `login module <http://docs.python.org/2/library/logging.html>`_ of
+            Python standard library.
+
+        """
+        info_style = u' \u251C\u2500 '
+        last_style = u' \u2514\u2500 '
+        style = u'' if last is None else last_style if last else info_style
+        cls._log(logging.DEBUG, u'{0}{1}: {2!s}'.format(style, param, value))
+
     def _fetch(self, url, method='GET', params=None, headers=None,
-               body='', max_redirects=5, content_parser=None):
+               body='', max_redirects=5, content_parser=None,
+               certificate_file=None, ssl_verify=True):
         """
         Fetches a URL.
 
         :param str url:
             The URL to fetch.
 
         :param str method:
@@ -375,49 +410,62 @@
         :param int max_redirects:
             Number of maximum HTTP redirects to follow.
 
         :param function content_parser:
             A callable to be used to parse the :attr:`.Response.data`
             from :attr:`.Response.content`.
 
+        :param str certificate_file:
+            Optional certificate file to be used for HTTPS connection.
+
+        :param bool ssl_verify:
+            Verify SSL on HTTPS connection.
         """
         # 'magic' using _kwarg method
         # pylint:disable=no-member
         params = params or {}
         params.update(self.access_params)
 
         headers = headers or {}
         headers.update(self.access_headers)
 
-        scheme, host, path, query, fragment = parse.urlsplit(url)
+        url_parsed = parse.urlsplit(url)
         query = parse.urlencode(params)
 
         if method in ('POST', 'PUT', 'PATCH'):
             if not body:
                 # Put querystring to body
                 body = query
                 query = ''
                 headers.update(
                     {'Content-Type': 'application/x-www-form-urlencoded'})
-        request_path = parse.urlunsplit(('', '', path or '', query or '', ''))
+        request_path = parse.urlunsplit(
+            ('', '', url_parsed.path or '', query or '', ''))
 
-        self._log(logging.DEBUG, u' \u251C\u2500 host: {0}'.format(host))
-        self._log(
-            logging.DEBUG,
-            u' \u251C\u2500 path: {0}'.format(request_path))
-        self._log(logging.DEBUG, u' \u251C\u2500 method: {0}'.format(method))
-        self._log(logging.DEBUG, u' \u251C\u2500 body: {0}'.format(body))
-        self._log(logging.DEBUG, u' \u251C\u2500 params: {0}'.format(params))
-        self._log(logging.DEBUG, u' \u2514\u2500 headers: {0}'.format(headers))
+        self._log_param('host', url_parsed.hostname, last=False)
+        self._log_param('method', method, last=False)
+        self._log_param('body', body, last=False)
+        self._log_param('params', params, last=False)
+        self._log_param('headers', headers, last=False)
+        self._log_param('certificate', certificate_file, last=False)
+        self._log_param('SSL verify', ssl_verify, last=True)
 
         # Connect
-        if scheme.lower() == 'https':
-            connection = http_client.HTTPSConnection(host)
+        if url_parsed.scheme.lower() == 'https':
+            context = None if ssl_verify else ssl._create_unverified_context()
+            cert_file = certificate_file if ssl_verify else None
+            connection = http_client.HTTPSConnection(
+                url_parsed.hostname,
+                port=url_parsed.port,
+                cert_file=cert_file,
+                context=context)
         else:
-            connection = http_client.HTTPConnection(host)
+            connection = http_client.HTTPConnection(
+                url_parsed.hostname,
+                port=url_parsed.port)
 
         try:
             connection.request(method, request_path, body, headers)
         except Exception as e:
             raise FetchError('Fetching URL failed',
                              original_message=str(e),
                              url=request_path)
@@ -430,40 +478,35 @@
                 raise FetchError('Url redirects to itself!',
                                  url=location,
                                  status=response.status)
 
             elif max_redirects > 0:
                 remaining_redirects = max_redirects - 1
 
-                self._log(logging.DEBUG, u'Redirecting to {0}'.format(url))
-                self._log(logging.DEBUG, u'Remaining redirects: {0}'
-                          .format(remaining_redirects))
+                self._log_param('Redirecting to', url)
+                self._log_param('Remaining redirects', remaining_redirects)
 
                 # Call this method again.
                 response = self._fetch(url=location,
                                        params=params,
                                        method=method,
                                        headers=headers,
-                                       max_redirects=remaining_redirects)
+                                       max_redirects=remaining_redirects,
+                                       certificate_file=certificate_file,
+                                       ssl_verify=ssl_verify)
 
             else:
                 raise FetchError('Max redirects reached!',
                                  url=location,
                                  status=response.status)
         else:
-            self._log(logging.DEBUG, u'Got response:')
-            self._log(logging.DEBUG, u' \u251C\u2500 url: {0}'.format(url))
-            self._log(
-                logging.DEBUG,
-                u' \u251C\u2500 status: {0}'.format(
-                    response.status))
-            self._log(
-                logging.DEBUG,
-                u' \u2514\u2500 headers: {0}'.format(
-                    response.getheaders()))
+            self._log_param('Got response')
+            self._log_param('url', url, last=False)
+            self._log_param('status', response.status, last=False)
+            self._log_param('headers', response.getheaders(), last=True)
 
         return authomatic.core.Response(response, content_parser)
 
     def _update_or_create_user(self, data, credentials=None, content=None):
         """
         Updates or creates :attr:`.user`.
 
@@ -769,72 +812,77 @@
         cls = self.__class__
         mod = sys.modules.get(cls.__module__)
 
         return str(self.PROVIDER_TYPE_ID) + '-' + \
             str(mod.PROVIDER_ID_MAP.index(cls))
 
     def access(self, url, params=None, method='GET', headers=None,
-               body='', max_redirects=5, content_parser=None):
+               body='', max_redirects=5, content_parser=None,
+               certificate_file=None, ssl_verify=True):
         """
         Fetches the **protected resource** of an authenticated **user**.
 
-        :param credentials:
-            The **user's** :class:`.Credentials` (serialized or normal).
-
         :param str url:
             The URL of the **protected resource**.
 
         :param str method:
             HTTP method of the request.
 
+        :param dict params:
+            Dictionary of request parameters.
+
         :param dict headers:
             HTTP headers of the request.
 
         :param str body:
             Body of ``POST``, ``PUT`` and ``PATCH`` requests.
 
         :param int max_redirects:
             Maximum number of HTTP redirects to follow.
 
         :param function content_parser:
             A function to be used to parse the :attr:`.Response.data`
             from :attr:`.Response.content`.
 
+        :param str certificate_file:
+            Optional certificate file to be used for HTTPS connection.
+
+        :param bool ssl_verify:
+            Verify SSL on HTTPS connection.
+
         :returns:
             :class:`.Response`
 
         """
 
         if not self.user and not self.credentials:
             raise CredentialsError(u'There is no authenticated user!')
 
         headers = headers or {}
 
-        self._log(
-            logging.INFO,
-            u'Accessing protected resource {0}.'.format(url))
+        self._log_param('Accessing protected resource', url, level=logging.INFO)
 
         request_elements = self.create_request_elements(
             request_type=self.PROTECTED_RESOURCE_REQUEST_TYPE,
             credentials=self.credentials,
             url=url,
             body=body,
             params=params,
             headers=headers,
             method=method
         )
 
         response = self._fetch(*request_elements,
                                max_redirects=max_redirects,
-                               content_parser=content_parser)
+                               content_parser=content_parser,
+                               certificate_file=certificate_file,
+                               ssl_verify=ssl_verify)
 
-        self._log(
-            logging.INFO,
-            u'Got response. HTTP status = {0}.'.format(
-                response.status))
+        status = response.status
+        self._log_param('Got response. HTTP status', status, level=logging.INFO)
         return response
 
     def async_access(self, *args, **kwargs):
         """
         Same as :meth:`.access` but runs asynchronously in a separate thread.
 
         .. warning::
@@ -972,15 +1020,17 @@
         Accesses the :attr:`.user_info_url`.
 
         :returns:
             :class:`.UserInfoResponse`
 
         """
         url = self.user_info_url.format(**self.user.__dict__)
-        return self.access(url)
+        cert = self._kwarg({}, 'certificate_file', None)
+        verify = self._kwarg({}, 'ssl_verify', True)
+        return self.access(url, certificate_file=cert, ssl_verify=verify)
 
 
 class AuthenticationProvider(BaseProvider):
     """
     Base provider for *authentication protocols* i.e. protocols which allow a
     **provider** to authenticate a *claimed identity* of a **user**.
```

### Comparing `Authomatic-1.2.1/authomatic/providers/gaeopenid.py` & `authomatic-1.3.0/authomatic/providers/gaeopenid.py`

 * *Files identical despite different names*

### Comparing `Authomatic-1.2.1/authomatic/providers/oauth1.py` & `authomatic-1.3.0/authomatic/providers/oauth1.py`

 * *Files identical despite different names*

### Comparing `Authomatic-1.2.1/authomatic/providers/oauth2.py` & `authomatic-1.3.0/authomatic/providers/oauth2.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,23 +79,31 @@
             `OAuth 2.0 spec <http://tools.ietf.org/html/rfc6749#section-3.3>`_.
 
         :param bool offline:
             If ``True`` the **provider** will be set up to request an
             *offline access token*.
             Default is ``False``.
 
+        :param str certificate_file:
+            Certificate file to employ for HTTPS connection where needed.
+
+        :param bool ssl_verify:
+            Certificate file to employ for HTTPS connection where needed.
+
         As well as those inherited from :class:`.AuthorizationProvider`
         constructor.
 
         """
 
         super(OAuth2, self).__init__(*args, **kwargs)
 
         self.scope = self._kwarg(kwargs, 'scope', [])
         self.offline = self._kwarg(kwargs, 'offline', False)
+        self.cert = self._kwarg(kwargs, 'certificate_file', None)
+        self.verify = self._kwarg(kwargs, 'ssl_verify', True)
 
     # ========================================================================
     # Internal methods
     # ========================================================================
 
     def _x_scope_parser(self, scope):
         """
@@ -308,15 +316,17 @@
             request_type=self.REFRESH_TOKEN_REQUEST_TYPE,
             credentials=credentials,
             url=self.access_token_url,
             method='POST'
         )
 
         self._log(logging.INFO, u'Refreshing credentials.')
-        response = self._fetch(*request_elements)
+        response = self._fetch(*request_elements,
+                               certificate_file=self.cert,
+                               ssl_verify=self.verify)
 
         # We no longer need consumer info.
         credentials.consumer_key = None
         credentials.consumer_secret = None
 
         # Extract the refreshed data.
         access_token = response.data.get('access_token')
@@ -406,15 +416,17 @@
                 url=self.access_token_url,
                 method=self.token_request_method,
                 redirect_uri=self.url,
                 params=self.access_token_params,
                 headers=self.access_token_headers
             )
 
-            response = self._fetch(*request_elements)
+            response = self._fetch(*request_elements,
+                                   certificate_file=self.cert,
+                                   ssl_verify=self.verify)
             self.access_token_response = response
 
             access_token = response.data.get('access_token', '')
             refresh_token = response.data.get('refresh_token', '')
 
             if response.status != 200 or not access_token:
                 raise FailureError(
```

### Comparing `Authomatic-1.2.1/authomatic/providers/openid.py` & `authomatic-1.3.0/authomatic/providers/openid.py`

 * *Files identical despite different names*

### Comparing `Authomatic-1.2.1/authomatic/six.py` & `authomatic-1.3.0/authomatic/six.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-# -*- coding: utf-8 -*-
-"""Utilities for writing code that runs on Python 2 and 3"""
-
-# Copyright (c) 2010-2015 Benjamin Peterson
+# Copyright (c) 2010-2020 Benjamin Peterson
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,29 +14,32 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+"""Utilities for writing code that runs on Python 2 and 3"""
+
 from __future__ import absolute_import
 
 import functools
 import itertools
 import operator
 import sys
 import types
 
 __author__ = "Benjamin Peterson <benjamin@python.org>"
-__version__ = "1.9.0"
+__version__ = "1.16.0"
 
 
 # Useful for very coarse version differentiation.
 PY2 = sys.version_info[0] == 2
 PY3 = sys.version_info[0] == 3
+PY34 = sys.version_info[0:2] >= (3, 4)
 
 if PY3:
     string_types = str,
     integer_types = int,
     class_types = type,
     text_type = str
     binary_type = bytes
@@ -54,26 +54,32 @@
 
     if sys.platform.startswith("java"):
         # Jython always uses 32 bits.
         MAXSIZE = int((1 << 31) - 1)
     else:
         # It's possible to have sizeof(long) != sizeof(Py_ssize_t).
         class X(object):
+
             def __len__(self):
                 return 1 << 31
         try:
             len(X())
         except OverflowError:
             # 32-bit
             MAXSIZE = int((1 << 31) - 1)
         else:
             # 64-bit
             MAXSIZE = int((1 << 63) - 1)
         del X
 
+if PY34:
+    from importlib.util import spec_from_loader
+else:
+    spec_from_loader = None
+
 
 def _add_doc(func, doc):
     """Add documentation to a function."""
     func.__doc__ = doc
 
 
 def _import_module(name):
@@ -157,20 +163,22 @@
 
     def _resolve(self):
         module = _import_module(self.mod)
         return getattr(module, self.attr)
 
 
 class _SixMetaPathImporter(object):
+
     """
     A meta path importer to import six.moves and its submodules.
 
     This class implements a PEP302 finder and loader. It should be compatible
     with Python 2.5 and all existing versions of Python3
     """
+
     def __init__(self, six_module_name):
         self.name = six_module_name
         self.known_modules = {}
 
     def _add_module(self, mod, *fullnames):
         for fullname in fullnames:
             self.known_modules[self.name + "." + fullname] = mod
@@ -179,14 +187,19 @@
         return self.known_modules[self.name + "." + fullname]
 
     def find_module(self, fullname, path=None):
         if fullname in self.known_modules:
             return self
         return None
 
+    def find_spec(self, fullname, path, target=None):
+        if fullname in self.known_modules:
+            return spec_from_loader(fullname, self)
+        return None
+
     def __get_module(self, fullname):
         try:
             return self.known_modules[fullname]
         except KeyError:
             raise ImportError("This loader does not know module " + fullname)
 
     def load_module(self, fullname):
@@ -216,56 +229,67 @@
         """Return None
 
         Required, if is_package is implemented"""
         self.__get_module(fullname)  # eventually raises ImportError
         return None
     get_source = get_code  # same as get_code
 
+    def create_module(self, spec):
+        return self.load_module(spec.name)
+
+    def exec_module(self, module):
+        pass
 
 _importer = _SixMetaPathImporter(__name__)
 
 
 class _MovedItems(_LazyModule):
+
     """Lazy loading of moved objects"""
     __path__ = []  # mark as package
 
 
 _moved_attributes = [
     MovedAttribute("cStringIO", "cStringIO", "io", "StringIO"),
     MovedAttribute("filter", "itertools", "builtins", "ifilter", "filter"),
     MovedAttribute("filterfalse", "itertools", "itertools", "ifilterfalse", "filterfalse"),
     MovedAttribute("input", "__builtin__", "builtins", "raw_input", "input"),
     MovedAttribute("intern", "__builtin__", "sys"),
     MovedAttribute("map", "itertools", "builtins", "imap", "map"),
+    MovedAttribute("getcwd", "os", "os", "getcwdu", "getcwd"),
+    MovedAttribute("getcwdb", "os", "os", "getcwd", "getcwdb"),
+    MovedAttribute("getoutput", "commands", "subprocess"),
     MovedAttribute("range", "__builtin__", "builtins", "xrange", "range"),
-    MovedAttribute("reload_module", "__builtin__", "imp", "reload"),
+    MovedAttribute("reload_module", "__builtin__", "importlib" if PY34 else "imp", "reload"),
     MovedAttribute("reduce", "__builtin__", "functools"),
     MovedAttribute("shlex_quote", "pipes", "shlex", "quote"),
     MovedAttribute("StringIO", "StringIO", "io"),
     MovedAttribute("UserDict", "UserDict", "collections"),
     MovedAttribute("UserList", "UserList", "collections"),
     MovedAttribute("UserString", "UserString", "collections"),
     MovedAttribute("xrange", "__builtin__", "builtins", "xrange", "range"),
     MovedAttribute("zip", "itertools", "builtins", "izip", "zip"),
     MovedAttribute("zip_longest", "itertools", "itertools", "izip_longest", "zip_longest"),
-
     MovedModule("builtins", "__builtin__"),
     MovedModule("configparser", "ConfigParser"),
+    MovedModule("collections_abc", "collections", "collections.abc" if sys.version_info >= (3, 3) else "collections"),
     MovedModule("copyreg", "copy_reg"),
     MovedModule("dbm_gnu", "gdbm", "dbm.gnu"),
-    MovedModule("_dummy_thread", "dummy_thread", "_dummy_thread"),
+    MovedModule("dbm_ndbm", "dbm", "dbm.ndbm"),
+    MovedModule("_dummy_thread", "dummy_thread", "_dummy_thread" if sys.version_info < (3, 9) else "_thread"),
     MovedModule("http_cookiejar", "cookielib", "http.cookiejar"),
     MovedModule("http_cookies", "Cookie", "http.cookies"),
     MovedModule("html_entities", "htmlentitydefs", "html.entities"),
     MovedModule("html_parser", "HTMLParser", "html.parser"),
     MovedModule("http_client", "httplib", "http.client"),
+    MovedModule("email_mime_base", "email.MIMEBase", "email.mime.base"),
+    MovedModule("email_mime_image", "email.MIMEImage", "email.mime.image"),
     MovedModule("email_mime_multipart", "email.MIMEMultipart", "email.mime.multipart"),
     MovedModule("email_mime_nonmultipart", "email.MIMENonMultipart", "email.mime.nonmultipart"),
     MovedModule("email_mime_text", "email.MIMEText", "email.mime.text"),
-    MovedModule("email_mime_base", "email.MIMEBase", "email.mime.base"),
     MovedModule("BaseHTTPServer", "BaseHTTPServer", "http.server"),
     MovedModule("CGIHTTPServer", "CGIHTTPServer", "http.server"),
     MovedModule("SimpleHTTPServer", "SimpleHTTPServer", "http.server"),
     MovedModule("cPickle", "cPickle", "pickle"),
     MovedModule("queue", "Queue"),
     MovedModule("reprlib", "repr"),
     MovedModule("socketserver", "SocketServer"),
@@ -290,29 +314,35 @@
                 "tkinter.simpledialog"),
     MovedModule("urllib_parse", __name__ + ".moves.urllib_parse", "urllib.parse"),
     MovedModule("urllib_error", __name__ + ".moves.urllib_error", "urllib.error"),
     MovedModule("urllib", __name__ + ".moves.urllib", __name__ + ".moves.urllib"),
     MovedModule("urllib_robotparser", "robotparser", "urllib.robotparser"),
     MovedModule("xmlrpc_client", "xmlrpclib", "xmlrpc.client"),
     MovedModule("xmlrpc_server", "SimpleXMLRPCServer", "xmlrpc.server"),
-    MovedModule("winreg", "_winreg"),
 ]
+# Add windows specific modules.
+if sys.platform == "win32":
+    _moved_attributes += [
+        MovedModule("winreg", "_winreg"),
+    ]
+
 for attr in _moved_attributes:
     setattr(_MovedItems, attr.name, attr)
     if isinstance(attr, MovedModule):
         _importer._add_module(attr, "moves." + attr.name)
 del attr
 
 _MovedItems._moved_attributes = _moved_attributes
 
 moves = _MovedItems(__name__ + ".moves")
 _importer._add_module(moves, "moves")
 
 
 class Module_six_moves_urllib_parse(_LazyModule):
+
     """Lazy loading of moved objects in six.moves.urllib_parse"""
 
 
 _urllib_parse_moved_attributes = [
     MovedAttribute("ParseResult", "urlparse", "urllib.parse"),
     MovedAttribute("SplitResult", "urlparse", "urllib.parse"),
     MovedAttribute("parse_qs", "urlparse", "urllib.parse"),
@@ -323,18 +353,20 @@
     MovedAttribute("urlsplit", "urlparse", "urllib.parse"),
     MovedAttribute("urlunparse", "urlparse", "urllib.parse"),
     MovedAttribute("urlunsplit", "urlparse", "urllib.parse"),
     MovedAttribute("quote", "urllib", "urllib.parse"),
     MovedAttribute("quote_plus", "urllib", "urllib.parse"),
     MovedAttribute("unquote", "urllib", "urllib.parse"),
     MovedAttribute("unquote_plus", "urllib", "urllib.parse"),
+    MovedAttribute("unquote_to_bytes", "urllib", "urllib.parse", "unquote", "unquote_to_bytes"),
     MovedAttribute("urlencode", "urllib", "urllib.parse"),
     MovedAttribute("splitquery", "urllib", "urllib.parse"),
     MovedAttribute("splittag", "urllib", "urllib.parse"),
     MovedAttribute("splituser", "urllib", "urllib.parse"),
+    MovedAttribute("splitvalue", "urllib", "urllib.parse"),
     MovedAttribute("uses_fragment", "urlparse", "urllib.parse"),
     MovedAttribute("uses_netloc", "urlparse", "urllib.parse"),
     MovedAttribute("uses_params", "urlparse", "urllib.parse"),
     MovedAttribute("uses_query", "urlparse", "urllib.parse"),
     MovedAttribute("uses_relative", "urlparse", "urllib.parse"),
 ]
 for attr in _urllib_parse_moved_attributes:
@@ -344,14 +376,15 @@
 Module_six_moves_urllib_parse._moved_attributes = _urllib_parse_moved_attributes
 
 _importer._add_module(Module_six_moves_urllib_parse(__name__ + ".moves.urllib_parse"),
                       "moves.urllib_parse", "moves.urllib.parse")
 
 
 class Module_six_moves_urllib_error(_LazyModule):
+
     """Lazy loading of moved objects in six.moves.urllib_error"""
 
 
 _urllib_error_moved_attributes = [
     MovedAttribute("URLError", "urllib2", "urllib.error"),
     MovedAttribute("HTTPError", "urllib2", "urllib.error"),
     MovedAttribute("ContentTooShortError", "urllib", "urllib.error"),
@@ -363,14 +396,15 @@
 Module_six_moves_urllib_error._moved_attributes = _urllib_error_moved_attributes
 
 _importer._add_module(Module_six_moves_urllib_error(__name__ + ".moves.urllib.error"),
                       "moves.urllib_error", "moves.urllib.error")
 
 
 class Module_six_moves_urllib_request(_LazyModule):
+
     """Lazy loading of moved objects in six.moves.urllib_request"""
 
 
 _urllib_request_moved_attributes = [
     MovedAttribute("urlopen", "urllib2", "urllib.request"),
     MovedAttribute("install_opener", "urllib2", "urllib.request"),
     MovedAttribute("build_opener", "urllib2", "urllib.request"),
@@ -400,26 +434,29 @@
     MovedAttribute("UnknownHandler", "urllib2", "urllib.request"),
     MovedAttribute("HTTPErrorProcessor", "urllib2", "urllib.request"),
     MovedAttribute("urlretrieve", "urllib", "urllib.request"),
     MovedAttribute("urlcleanup", "urllib", "urllib.request"),
     MovedAttribute("URLopener", "urllib", "urllib.request"),
     MovedAttribute("FancyURLopener", "urllib", "urllib.request"),
     MovedAttribute("proxy_bypass", "urllib", "urllib.request"),
+    MovedAttribute("parse_http_list", "urllib2", "urllib.request"),
+    MovedAttribute("parse_keqv_list", "urllib2", "urllib.request"),
 ]
 for attr in _urllib_request_moved_attributes:
     setattr(Module_six_moves_urllib_request, attr.name, attr)
 del attr
 
 Module_six_moves_urllib_request._moved_attributes = _urllib_request_moved_attributes
 
 _importer._add_module(Module_six_moves_urllib_request(__name__ + ".moves.urllib.request"),
                       "moves.urllib_request", "moves.urllib.request")
 
 
 class Module_six_moves_urllib_response(_LazyModule):
+
     """Lazy loading of moved objects in six.moves.urllib_response"""
 
 
 _urllib_response_moved_attributes = [
     MovedAttribute("addbase", "urllib", "urllib.response"),
     MovedAttribute("addclosehook", "urllib", "urllib.response"),
     MovedAttribute("addinfo", "urllib", "urllib.response"),
@@ -432,14 +469,15 @@
 Module_six_moves_urllib_response._moved_attributes = _urllib_response_moved_attributes
 
 _importer._add_module(Module_six_moves_urllib_response(__name__ + ".moves.urllib.response"),
                       "moves.urllib_response", "moves.urllib.response")
 
 
 class Module_six_moves_urllib_robotparser(_LazyModule):
+
     """Lazy loading of moved objects in six.moves.urllib_robotparser"""
 
 
 _urllib_robotparser_moved_attributes = [
     MovedAttribute("RobotFileParser", "robotparser", "urllib.robotparser"),
 ]
 for attr in _urllib_robotparser_moved_attributes:
@@ -449,26 +487,26 @@
 Module_six_moves_urllib_robotparser._moved_attributes = _urllib_robotparser_moved_attributes
 
 _importer._add_module(Module_six_moves_urllib_robotparser(__name__ + ".moves.urllib.robotparser"),
                       "moves.urllib_robotparser", "moves.urllib.robotparser")
 
 
 class Module_six_moves_urllib(types.ModuleType):
+
     """Create a six.moves.urllib namespace that resembles the Python 3 namespace"""
     __path__ = []  # mark as package
     parse = _importer._get_module("moves.urllib_parse")
     error = _importer._get_module("moves.urllib_error")
     request = _importer._get_module("moves.urllib_request")
     response = _importer._get_module("moves.urllib_response")
     robotparser = _importer._get_module("moves.urllib_robotparser")
 
     def __dir__(self):
         return ['parse', 'error', 'request', 'response', 'robotparser']
 
-
 _importer._add_module(Module_six_moves_urllib(__name__ + ".moves.urllib"),
                       "moves.urllib")
 
 
 def add_move(move):
     """Add an item to six.moves."""
     setattr(_MovedItems, move.name, move)
@@ -520,22 +558,28 @@
 
 if PY3:
     def get_unbound_function(unbound):
         return unbound
 
     create_bound_method = types.MethodType
 
+    def create_unbound_method(func, cls):
+        return func
+
     Iterator = object
 else:
     def get_unbound_function(unbound):
         return unbound.im_func
 
     def create_bound_method(func, obj):
         return types.MethodType(func, obj, obj.__class__)
 
+    def create_unbound_method(func, cls):
+        return types.MethodType(func, None, cls)
+
     class Iterator(object):
 
         def next(self):
             return type(self).__next__(self)
 
     callable = callable
 _add_doc(get_unbound_function,
@@ -566,24 +610,24 @@
     viewkeys = operator.methodcaller("keys")
 
     viewvalues = operator.methodcaller("values")
 
     viewitems = operator.methodcaller("items")
 else:
     def iterkeys(d, **kw):
-        return iter(d.iterkeys(**kw))
+        return d.iterkeys(**kw)
 
     def itervalues(d, **kw):
-        return iter(d.itervalues(**kw))
+        return d.itervalues(**kw)
 
     def iteritems(d, **kw):
-        return iter(d.iteritems(**kw))
+        return d.iteritems(**kw)
 
     def iterlists(d, **kw):
-        return iter(d.iterlists(**kw))
+        return d.iterlists(**kw)
 
     viewkeys = operator.methodcaller("viewkeys")
 
     viewvalues = operator.methodcaller("viewvalues")
 
     viewitems = operator.methodcaller("viewitems")
 
@@ -597,54 +641,56 @@
 
 if PY3:
     def b(s):
         return s.encode("latin-1")
 
     def u(s):
         return s
-
     unichr = chr
-    if sys.version_info[1] <= 1:
-        def int2byte(i):
-            return bytes((i,))
-    else:
-        # This is about 2x faster than the implementation above on 3.2+
-        int2byte = operator.methodcaller("to_bytes", 1, "big")
+    import struct
+    int2byte = struct.Struct(">B").pack
+    del struct
     byte2int = operator.itemgetter(0)
     indexbytes = operator.getitem
     iterbytes = iter
     import io
     StringIO = io.StringIO
     BytesIO = io.BytesIO
+    del io
     _assertCountEqual = "assertCountEqual"
-    _assertRaisesRegex = "assertRaisesRegex"
-    _assertRegex = "assertRegex"
+    if sys.version_info[1] <= 1:
+        _assertRaisesRegex = "assertRaisesRegexp"
+        _assertRegex = "assertRegexpMatches"
+        _assertNotRegex = "assertNotRegexpMatches"
+    else:
+        _assertRaisesRegex = "assertRaisesRegex"
+        _assertRegex = "assertRegex"
+        _assertNotRegex = "assertNotRegex"
 else:
     def b(s):
         return s
-
     # Workaround for standalone backslash
+
     def u(s):
         return unicode(s.replace(r'\\', r'\\\\'), "unicode_escape")
-
     unichr = unichr
     int2byte = chr
 
     def byte2int(bs):
         return ord(bs[0])
 
     def indexbytes(buf, i):
         return ord(buf[i])
-
     iterbytes = functools.partial(itertools.imap, ord)
     import StringIO
     StringIO = BytesIO = StringIO.StringIO
     _assertCountEqual = "assertItemsEqual"
     _assertRaisesRegex = "assertRaisesRegexp"
     _assertRegex = "assertRegexpMatches"
+    _assertNotRegex = "assertNotRegexpMatches"
 _add_doc(b, """Byte literal""")
 _add_doc(u, """Text literal""")
 
 
 def assertCountEqual(self, *args, **kwargs):
     return getattr(self, _assertCountEqual)(*args, **kwargs)
 
@@ -653,23 +699,31 @@
     return getattr(self, _assertRaisesRegex)(*args, **kwargs)
 
 
 def assertRegex(self, *args, **kwargs):
     return getattr(self, _assertRegex)(*args, **kwargs)
 
 
+def assertNotRegex(self, *args, **kwargs):
+    return getattr(self, _assertNotRegex)(*args, **kwargs)
+
+
 if PY3:
     exec_ = getattr(moves.builtins, "exec")
 
     def reraise(tp, value, tb=None):
-        if value is None:
-            value = tp()
-        if value.__traceback__ is not tb:
-            raise value.with_traceback(tb)
-        raise value
+        try:
+            if value is None:
+                value = tp()
+            if value.__traceback__ is not tb:
+                raise value.with_traceback(tb)
+            raise value
+        finally:
+            value = None
+            tb = None
 
 else:
     def exec_(_code_, _globs_=None, _locs_=None):
         """Execute code in a namespace."""
         if _globs_ is None:
             frame = sys._getframe(1)
             _globs_ = frame.f_globals
@@ -677,27 +731,27 @@
                 _locs_ = frame.f_locals
             del frame
         elif _locs_ is None:
             _locs_ = _globs_
         exec("""exec _code_ in _globs_, _locs_""")
 
     exec_("""def reraise(tp, value, tb=None):
-    raise tp, value, tb
+    try:
+        raise tp, value, tb
+    finally:
+        tb = None
 """)
 
 
-if sys.version_info[:2] == (3, 2):
-    exec_("""def raise_from(value, from_value):
-    if from_value is None:
-        raise value
-    raise value from from_value
-""")
-elif sys.version_info[:2] > (3, 2):
+if sys.version_info[:2] > (3,):
     exec_("""def raise_from(value, from_value):
-    raise value from from_value
+    try:
+        raise value from from_value
+    finally:
+        value = None
 """)
 else:
     def raise_from(value, from_value):
         raise value
 
 
 print_ = getattr(moves.builtins, "print", None)
@@ -708,19 +762,17 @@
         if fp is None:
             return
 
         def write(data):
             if not isinstance(data, basestring):
                 data = str(data)
             # If the file has an encoding, encode unicode with it.
-            if (
-                isinstance(fp, file)
-                and isinstance(data, unicode)
-                and fp.encoding is not None
-            ):
+            if (isinstance(fp, file) and
+                    isinstance(data, unicode) and
+                    fp.encoding is not None):
                 errors = getattr(fp, "errors", None)
                 if errors is None:
                     errors = "strict"
                 data = data.encode(fp.encoding, errors)
             fp.write(data)
         want_unicode = False
         sep = kwargs.pop("sep", None)
@@ -766,33 +818,66 @@
         _print(*args, **kwargs)
         if flush and fp is not None:
             fp.flush()
 
 _add_doc(reraise, """Reraise an exception.""")
 
 if sys.version_info[0:2] < (3, 4):
+    # This does exactly the same what the :func:`py3:functools.update_wrapper`
+    # function does on Python versions after 3.2. It sets the ``__wrapped__``
+    # attribute on ``wrapper`` object and it doesn't raise an error if any of
+    # the attributes mentioned in ``assigned`` and ``updated`` are missing on
+    # ``wrapped`` object.
+    def _update_wrapper(wrapper, wrapped,
+                        assigned=functools.WRAPPER_ASSIGNMENTS,
+                        updated=functools.WRAPPER_UPDATES):
+        for attr in assigned:
+            try:
+                value = getattr(wrapped, attr)
+            except AttributeError:
+                continue
+            else:
+                setattr(wrapper, attr, value)
+        for attr in updated:
+            getattr(wrapper, attr).update(getattr(wrapped, attr, {}))
+        wrapper.__wrapped__ = wrapped
+        return wrapper
+    _update_wrapper.__doc__ = functools.update_wrapper.__doc__
+
     def wraps(wrapped, assigned=functools.WRAPPER_ASSIGNMENTS,
               updated=functools.WRAPPER_UPDATES):
-        def wrapper(f):
-            f = functools.wraps(wrapped, assigned, updated)(f)
-            f.__wrapped__ = wrapped
-            return f
-        return wrapper
+        return functools.partial(_update_wrapper, wrapped=wrapped,
+                                 assigned=assigned, updated=updated)
+    wraps.__doc__ = functools.wraps.__doc__
+
 else:
     wraps = functools.wraps
 
 
 def with_metaclass(meta, *bases):
     """Create a base class with a metaclass."""
     # This requires a bit of explanation: the basic idea is to make a dummy
     # metaclass for one level of class instantiation that replaces itself with
     # the actual metaclass.
-    class metaclass(meta):
+    class metaclass(type):
+
         def __new__(cls, name, this_bases, d):
-            return meta(name, bases, d)
+            if sys.version_info[:2] >= (3, 7):
+                # This version introduced PEP 560 that requires a bit
+                # of extra care (we mimic what is done by __build_class__).
+                resolved_bases = types.resolve_bases(bases)
+                if resolved_bases is not bases:
+                    d['__orig_bases__'] = bases
+            else:
+                resolved_bases = bases
+            return meta(name, resolved_bases, d)
+
+        @classmethod
+        def __prepare__(cls, name, this_bases):
+            return meta.__prepare__(name, bases)
     return type.__new__(metaclass, 'temporary_class', (), {})
 
 
 def add_metaclass(metaclass):
     """Class decorator for creating a class with a metaclass."""
     def wrapper(cls):
         orig_vars = cls.__dict__.copy()
@@ -800,21 +885,83 @@
         if slots is not None:
             if isinstance(slots, str):
                 slots = [slots]
             for slots_var in slots:
                 orig_vars.pop(slots_var)
         orig_vars.pop('__dict__', None)
         orig_vars.pop('__weakref__', None)
+        if hasattr(cls, '__qualname__'):
+            orig_vars['__qualname__'] = cls.__qualname__
         return metaclass(cls.__name__, cls.__bases__, orig_vars)
     return wrapper
 
 
+def ensure_binary(s, encoding='utf-8', errors='strict'):
+    """Coerce **s** to six.binary_type.
+
+    For Python 2:
+      - `unicode` -> encoded to `str`
+      - `str` -> `str`
+
+    For Python 3:
+      - `str` -> encoded to `bytes`
+      - `bytes` -> `bytes`
+    """
+    if isinstance(s, binary_type):
+        return s
+    if isinstance(s, text_type):
+        return s.encode(encoding, errors)
+    raise TypeError("not expecting type '%s'" % type(s))
+
+
+def ensure_str(s, encoding='utf-8', errors='strict'):
+    """Coerce *s* to `str`.
+
+    For Python 2:
+      - `unicode` -> encoded to `str`
+      - `str` -> `str`
+
+    For Python 3:
+      - `str` -> `str`
+      - `bytes` -> decoded to `str`
+    """
+    # Optimization: Fast return for the common case.
+    if type(s) is str:
+        return s
+    if PY2 and isinstance(s, text_type):
+        return s.encode(encoding, errors)
+    elif PY3 and isinstance(s, binary_type):
+        return s.decode(encoding, errors)
+    elif not isinstance(s, (text_type, binary_type)):
+        raise TypeError("not expecting type '%s'" % type(s))
+    return s
+
+
+def ensure_text(s, encoding='utf-8', errors='strict'):
+    """Coerce *s* to six.text_type.
+
+    For Python 2:
+      - `unicode` -> `unicode`
+      - `str` -> `unicode`
+
+    For Python 3:
+      - `str` -> `str`
+      - `bytes` -> decoded to `str`
+    """
+    if isinstance(s, binary_type):
+        return s.decode(encoding, errors)
+    elif isinstance(s, text_type):
+        return s
+    else:
+        raise TypeError("not expecting type '%s'" % type(s))
+
+
 def python_2_unicode_compatible(klass):
     """
-    A decorator that defines __unicode__ and __str__ methods under Python 2.
+    A class decorator that defines __unicode__ and __str__ methods under Python 2.
     Under Python 3 it does nothing.
 
     To support Python 2 and 3 with a single code base, define a __str__ method
     returning text and apply this decorator to the class.
     """
     if PY2:
         if '__str__' not in klass.__dict__:
@@ -838,16 +985,14 @@
 # this for some reason.)
 if sys.meta_path:
     for i, importer in enumerate(sys.meta_path):
         # Here's some real nastiness: Another "instance" of the six module might
         # be floating around. Therefore, we can't use isinstance() to check for
         # the six meta path importer, since the other six instance will have
         # inserted an importer with different class.
-        if (
-            type(importer).__name__ == "_SixMetaPathImporter"
-            and importer.name == __name__
-        ):
+        if (type(importer).__name__ == "_SixMetaPathImporter" and
+                importer.name == __name__):
             del sys.meta_path[i]
             break
     del i, importer
 # Finally, add the importer to the meta path import hook.
 sys.meta_path.append(_importer)
```

### Comparing `Authomatic-1.2.1/config-template.py` & `authomatic-1.3.0/config-template.py`

 * *Files identical despite different names*

### Comparing `Authomatic-1.2.1/javascript/authomatic.js` & `authomatic-1.3.0/javascript/authomatic.js`

 * *Files identical despite different names*

### Comparing `Authomatic-1.2.1/javascript/authomatic.map` & `authomatic-1.3.0/javascript/authomatic.map`

 * *Files identical despite different names*

### Comparing `Authomatic-1.2.1/setup.cfg` & `authomatic-1.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.2.1
+version = 1.3.0
 name = Authomatic
 description = Authorization / authentication client library for Python web applications
 long_description = file: README.rst
 author = Peter Hudec
 author_email = peterhudec@peterhudec.com
 maintainer = Authomatic Project Community
 maintainer_email = authomaticproject@protonmail.com
```

