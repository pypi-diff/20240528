# Comparing `tmp/impact-stack-observability-0.2.0.tar.gz` & `tmp/impact_stack_observability-0.3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impact-stack-observability-0.2.0.tar", last modified: Fri Jun  2 08:15:39 2023, max compression
+gzip compressed data, was "impact_stack_observability-0.3.0a1.tar", last modified: Tue May 28 19:04:42 2024, max compression
```

## Comparing `impact-stack-observability-0.2.0.tar` & `impact_stack_observability-0.3.0a1.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2023-06-02 08:15:39.793650 impact-stack-observability-0.2.0/
--rw-r--r--   0 devel     (1001) devel     (1001)    35149 2023-01-23 11:48:29.000000 impact-stack-observability-0.2.0/LICENSE
--rw-r--r--   0 devel     (1001) devel     (1001)    44584 2023-06-02 08:15:39.793650 impact-stack-observability-0.2.0/PKG-INFO
--rw-r--r--   0 devel     (1001) devel     (1001)     3372 2023-06-02 08:09:11.000000 impact-stack-observability-0.2.0/README.md
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2023-06-02 08:15:39.789650 impact-stack-observability-0.2.0/impact_stack/
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2023-06-02 08:15:39.789650 impact-stack-observability-0.2.0/impact_stack/observability/
--rw-r--r--   0 devel     (1001) devel     (1001)       52 2023-02-27 12:07:54.000000 impact-stack-observability-0.2.0/impact_stack/observability/__init__.py
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2023-06-02 08:15:39.793650 impact-stack-observability-0.2.0/impact_stack/observability/health/
--rw-r--r--   0 devel     (1001) devel     (1001)      259 2023-03-13 13:19:20.000000 impact-stack-observability-0.2.0/impact_stack/observability/health/__init__.py
--rw-r--r--   0 devel     (1001) devel     (1001)     3214 2023-06-02 08:09:11.000000 impact-stack-observability-0.2.0/impact_stack/observability/health/blueprint.py
--rw-r--r--   0 devel     (1001) devel     (1001)     1548 2023-03-13 13:19:20.000000 impact-stack-observability-0.2.0/impact_stack/observability/health/checks.py
--rw-r--r--   0 devel     (1001) devel     (1001)     1741 2023-03-13 13:19:20.000000 impact-stack-observability-0.2.0/impact_stack/observability/health/extension.py
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2023-06-02 08:15:39.793650 impact-stack-observability-0.2.0/impact_stack_observability.egg-info/
--rw-r--r--   0 devel     (1001) devel     (1001)    44584 2023-06-02 08:15:39.000000 impact-stack-observability-0.2.0/impact_stack_observability.egg-info/PKG-INFO
--rw-r--r--   0 devel     (1001) devel     (1001)      504 2023-06-02 08:15:39.000000 impact-stack-observability-0.2.0/impact_stack_observability.egg-info/SOURCES.txt
--rw-r--r--   0 devel     (1001) devel     (1001)        1 2023-06-02 08:15:39.000000 impact-stack-observability-0.2.0/impact_stack_observability.egg-info/dependency_links.txt
--rw-r--r--   0 devel     (1001) devel     (1001)      130 2023-06-02 08:15:39.000000 impact-stack-observability-0.2.0/impact_stack_observability.egg-info/requires.txt
--rw-r--r--   0 devel     (1001) devel     (1001)       13 2023-06-02 08:15:39.000000 impact-stack-observability-0.2.0/impact_stack_observability.egg-info/top_level.txt
--rw-r--r--   0 devel     (1001) devel     (1001)     1446 2023-06-02 08:09:48.000000 impact-stack-observability-0.2.0/pyproject.toml
--rw-r--r--   0 devel     (1001) devel     (1001)       38 2023-06-02 08:15:39.793650 impact-stack-observability-0.2.0/setup.cfg
+drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2024-05-28 19:04:42.160405 impact_stack_observability-0.3.0a1/
+-rw-r--r--   0 devel     (1001) devel     (1001)    35149 2023-01-23 11:48:29.000000 impact_stack_observability-0.3.0a1/LICENSE
+-rw-r--r--   0 devel     (1001) devel     (1001)    46537 2024-05-28 19:04:42.160405 impact_stack_observability-0.3.0a1/PKG-INFO
+-rw-r--r--   0 devel     (1001) devel     (1001)     4205 2024-05-28 19:03:23.000000 impact_stack_observability-0.3.0a1/README.md
+drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2024-05-28 19:04:42.152405 impact_stack_observability-0.3.0a1/impact_stack/
+drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2024-05-28 19:04:42.152405 impact_stack_observability-0.3.0a1/impact_stack/observability/
+-rw-r--r--   0 devel     (1001) devel     (1001)       52 2023-02-27 12:07:54.000000 impact_stack_observability-0.3.0a1/impact_stack/observability/__init__.py
+drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2024-05-28 19:04:42.156406 impact_stack_observability-0.3.0a1/impact_stack/observability/health/
+-rw-r--r--   0 devel     (1001) devel     (1001)      259 2023-03-13 13:19:20.000000 impact_stack_observability-0.3.0a1/impact_stack/observability/health/__init__.py
+-rw-r--r--   0 devel     (1001) devel     (1001)     3214 2024-04-29 13:50:40.000000 impact_stack_observability-0.3.0a1/impact_stack/observability/health/blueprint.py
+-rw-r--r--   0 devel     (1001) devel     (1001)     1548 2023-03-13 13:19:20.000000 impact_stack_observability-0.3.0a1/impact_stack/observability/health/checks.py
+-rw-r--r--   0 devel     (1001) devel     (1001)     1741 2023-03-13 13:19:20.000000 impact_stack_observability-0.3.0a1/impact_stack/observability/health/extension.py
+drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2024-05-28 19:04:42.156406 impact_stack_observability-0.3.0a1/impact_stack/observability/tracing/
+-rw-r--r--   0 devel     (1001) devel     (1001)      207 2024-05-28 19:01:19.000000 impact_stack_observability-0.3.0a1/impact_stack/observability/tracing/__init__.py
+-rw-r--r--   0 devel     (1001) devel     (1001)      727 2024-05-28 18:58:02.000000 impact_stack_observability-0.3.0a1/impact_stack/observability/tracing/extension.py
+-rw-r--r--   0 devel     (1001) devel     (1001)    11617 2024-05-28 19:01:19.000000 impact_stack_observability-0.3.0a1/impact_stack/observability/tracing/utils.py
+drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2024-05-28 19:04:42.156406 impact_stack_observability-0.3.0a1/impact_stack_observability.egg-info/
+-rw-r--r--   0 devel     (1001) devel     (1001)    46537 2024-05-28 19:04:42.000000 impact_stack_observability-0.3.0a1/impact_stack_observability.egg-info/PKG-INFO
+-rw-r--r--   0 devel     (1001) devel     (1001)      643 2024-05-28 19:04:42.000000 impact_stack_observability-0.3.0a1/impact_stack_observability.egg-info/SOURCES.txt
+-rw-r--r--   0 devel     (1001) devel     (1001)        1 2024-05-28 19:04:42.000000 impact_stack_observability-0.3.0a1/impact_stack_observability.egg-info/dependency_links.txt
+-rw-r--r--   0 devel     (1001) devel     (1001)      483 2024-05-28 19:04:42.000000 impact_stack_observability-0.3.0a1/impact_stack_observability.egg-info/requires.txt
+-rw-r--r--   0 devel     (1001) devel     (1001)       13 2024-05-28 19:04:42.000000 impact_stack_observability-0.3.0a1/impact_stack_observability.egg-info/top_level.txt
+-rw-r--r--   0 devel     (1001) devel     (1001)     1851 2024-05-28 19:01:22.000000 impact_stack_observability-0.3.0a1/pyproject.toml
+-rw-r--r--   0 devel     (1001) devel     (1001)       38 2024-05-28 19:04:42.160405 impact_stack_observability-0.3.0a1/setup.cfg
```

### Comparing `impact-stack-observability-0.2.0/LICENSE` & `impact_stack_observability-0.3.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `impact-stack-observability-0.2.0/PKG-INFO` & `impact_stack_observability-0.3.0a1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impact-stack-observability
-Version: 0.2.0
+Version: 0.3.0a1
 Summary: Observability for Impact Stack
 Author-email: Alex Berger <alex@more-onion.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -685,16 +685,41 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: flask
+Requires-Dist: requests
+Requires-Dist: opentelemetry-api>=1.24.0
+Requires-Dist: opentelemetry-sdk>=1.24.0
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: celery[redis]; extra == "dev"
+Requires-Dist: flask-sqlalchemy; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: pip-tools; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pydocstyle[toml]>=6; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-flask; extra == "dev"
+Provides-Extra: celery
+Requires-Dist: opentelemetry-instrumentation-celery>=0.45b0; extra == "celery"
+Provides-Extra: flask
+Requires-Dist: opentelemetry-instrumentation-flask>=0.45b0; extra == "flask"
+Provides-Extra: logging
+Requires-Dist: opentelemetry-instrumentation-logging>=0.45b0; extra == "logging"
+Provides-Extra: requests
+Requires-Dist: opentelemetry-instrumentation-requests>=0.45b0; extra == "requests"
+Provides-Extra: sqlalchemy
+Requires-Dist: opentelemetry-instrumentation-sqlalchemy>=0.45b0; extra == "sqlalchemy"
 
 # Observability for Impact Stack
 
 A package providing observability features for Flask apps.
 
 ## Health checks
 
@@ -826,7 +851,30 @@
 
 Set the required config variable `HEALTH_URL_SECRET` to a (random) string and
 use the GET param `auth` in calls to the endpoint.
 Returns `401` if the secret does not match.
 Raises a `RuntimeError` if not set.
 
 If the `HEALTH_URL_SECRET` is set to `None`, checking the secret is disabled.
+
+## Tracing
+
+https://opentelemetry.io/docs/languages/python/instrumentation/
+
+### Autoinstrumentations
+
+Tested and supported
+- flask https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/flask/flask.html
+- celery https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/celery/celery.html
+- sqlalchemy https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/sqlalchemy/sqlalchemy.html
+- requests https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/requests/requests.html
+
+instrument_app(app) after Flask() is initiated
+or instrument() before Flask() is initiated
+
+## Tests
+
+needs sqlalchemy, Postgresql
+redis
+
+multiple tracers
+https://opentelemetry.io/docs/languages/python/cookbook/#using-multiple-tracer-providers-with-different-resource
```

### Comparing `impact-stack-observability-0.2.0/README.md` & `impact_stack_observability-0.3.0a1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -132,7 +132,30 @@
 
 Set the required config variable `HEALTH_URL_SECRET` to a (random) string and
 use the GET param `auth` in calls to the endpoint.
 Returns `401` if the secret does not match.
 Raises a `RuntimeError` if not set.
 
 If the `HEALTH_URL_SECRET` is set to `None`, checking the secret is disabled.
+
+## Tracing
+
+https://opentelemetry.io/docs/languages/python/instrumentation/
+
+### Autoinstrumentations
+
+Tested and supported
+- flask https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/flask/flask.html
+- celery https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/celery/celery.html
+- sqlalchemy https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/sqlalchemy/sqlalchemy.html
+- requests https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/requests/requests.html
+
+instrument_app(app) after Flask() is initiated
+or instrument() before Flask() is initiated
+
+## Tests
+
+needs sqlalchemy, Postgresql
+redis
+
+multiple tracers
+https://opentelemetry.io/docs/languages/python/cookbook/#using-multiple-tracer-providers-with-different-resource
```

### Comparing `impact-stack-observability-0.2.0/impact_stack/observability/health/blueprint.py` & `impact_stack_observability-0.3.0a1/impact_stack/observability/health/blueprint.py`

 * *Files identical despite different names*

### Comparing `impact-stack-observability-0.2.0/impact_stack/observability/health/checks.py` & `impact_stack_observability-0.3.0a1/impact_stack/observability/health/checks.py`

 * *Files identical despite different names*

### Comparing `impact-stack-observability-0.2.0/impact_stack/observability/health/extension.py` & `impact_stack_observability-0.3.0a1/impact_stack/observability/health/extension.py`

 * *Files identical despite different names*

### Comparing `impact-stack-observability-0.2.0/impact_stack_observability.egg-info/PKG-INFO` & `impact_stack_observability-0.3.0a1/impact_stack_observability.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impact-stack-observability
-Version: 0.2.0
+Version: 0.3.0a1
 Summary: Observability for Impact Stack
 Author-email: Alex Berger <alex@more-onion.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -685,16 +685,41 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: flask
+Requires-Dist: requests
+Requires-Dist: opentelemetry-api>=1.24.0
+Requires-Dist: opentelemetry-sdk>=1.24.0
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: celery[redis]; extra == "dev"
+Requires-Dist: flask-sqlalchemy; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: pip-tools; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pydocstyle[toml]>=6; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-flask; extra == "dev"
+Provides-Extra: celery
+Requires-Dist: opentelemetry-instrumentation-celery>=0.45b0; extra == "celery"
+Provides-Extra: flask
+Requires-Dist: opentelemetry-instrumentation-flask>=0.45b0; extra == "flask"
+Provides-Extra: logging
+Requires-Dist: opentelemetry-instrumentation-logging>=0.45b0; extra == "logging"
+Provides-Extra: requests
+Requires-Dist: opentelemetry-instrumentation-requests>=0.45b0; extra == "requests"
+Provides-Extra: sqlalchemy
+Requires-Dist: opentelemetry-instrumentation-sqlalchemy>=0.45b0; extra == "sqlalchemy"
 
 # Observability for Impact Stack
 
 A package providing observability features for Flask apps.
 
 ## Health checks
 
@@ -826,7 +851,30 @@
 
 Set the required config variable `HEALTH_URL_SECRET` to a (random) string and
 use the GET param `auth` in calls to the endpoint.
 Returns `401` if the secret does not match.
 Raises a `RuntimeError` if not set.
 
 If the `HEALTH_URL_SECRET` is set to `None`, checking the secret is disabled.
+
+## Tracing
+
+https://opentelemetry.io/docs/languages/python/instrumentation/
+
+### Autoinstrumentations
+
+Tested and supported
+- flask https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/flask/flask.html
+- celery https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/celery/celery.html
+- sqlalchemy https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/sqlalchemy/sqlalchemy.html
+- requests https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/requests/requests.html
+
+instrument_app(app) after Flask() is initiated
+or instrument() before Flask() is initiated
+
+## Tests
+
+needs sqlalchemy, Postgresql
+redis
+
+multiple tracers
+https://opentelemetry.io/docs/languages/python/cookbook/#using-multiple-tracer-providers-with-different-resource
```

### Comparing `impact-stack-observability-0.2.0/pyproject.toml` & `impact_stack_observability-0.3.0a1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [project]
 name = "impact-stack-observability"
-version = "0.2.0"
+version = "0.3.0a1"
 description = "Observability for Impact Stack"
 dependencies = [
   "flask",
   "requests",
+  "opentelemetry-api>=1.24.0",
+  "opentelemetry-sdk>=1.24.0",
 ]
 authors = [
   { name = "Alex Berger", email = "alex@more-onion.com" },
 ]
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
@@ -22,24 +24,40 @@
   "Programming Language :: Python",
   "Topic :: Software Development",
 ]
 
 [project.optional-dependencies]
 dev = [
   "black",
+  "celery[redis]",
   "flask-sqlalchemy",
   "isort",
   "pip-tools",
   "pre-commit",
   "pydocstyle[toml]>=6",
   "pylint",
   "pytest",
   "pytest-cov",
   "pytest-flask",
 ]
+celery = [
+  "opentelemetry-instrumentation-celery>=0.45b0"
+]
+flask = [
+  "opentelemetry-instrumentation-flask>=0.45b0"
+]
+logging = [
+  "opentelemetry-instrumentation-logging>=0.45b0"
+]
+requests = [
+  "opentelemetry-instrumentation-requests>=0.45b0"
+]
+sqlalchemy = [
+  "opentelemetry-instrumentation-sqlalchemy>=0.45b0"
+]
 
 [build-system]
 requires = [
   "setuptools>=42",
   "wheel",
 ]
 build-backend = "setuptools.build_meta"
```

