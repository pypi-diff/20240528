# Comparing `tmp/muffin-0.99.2.tar.gz` & `tmp/muffin-0.99.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin-0.99.2.tar", max compression
+gzip compressed data, was "muffin-0.99.3.tar", max compression
```

## Comparing `muffin-0.99.2.tar` & `muffin-0.99.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     9874 2023-08-07 14:02:33.282856 muffin-0.99.2/README.rst
--rw-r--r--   0        0        0     1016 2023-08-07 14:02:33.282856 muffin-0.99.2/muffin/__init__.py
--rw-r--r--   0        0        0     5213 2023-08-07 14:02:33.282856 muffin-0.99.2/muffin/app.py
--rw-r--r--   0        0        0       71 2023-08-07 14:02:33.282856 muffin-0.99.2/muffin/constants.py
--rw-r--r--   0        0        0      701 2023-08-07 14:02:33.282856 muffin-0.99.2/muffin/errors.py
--rw-r--r--   0        0        0     3755 2023-08-07 14:02:33.282856 muffin-0.99.2/muffin/handler.py
--rw-r--r--   0        0        0     8820 2023-08-07 14:02:33.282856 muffin-0.99.2/muffin/manage.py
--rw-r--r--   0        0        0     2877 2023-08-07 14:02:33.282856 muffin-0.99.2/muffin/plugins.py
--rw-r--r--   0        0        0        0 2023-08-07 14:02:33.282856 muffin-0.99.2/muffin/py.typed
--rw-r--r--   0        0        0     2692 2023-08-07 14:02:33.282856 muffin-0.99.2/muffin/pytest.py
--rw-r--r--   0        0        0      153 2023-08-07 14:02:33.282856 muffin-0.99.2/muffin/types.py
--rw-r--r--   0        0        0     2905 2023-08-07 14:02:33.286857 muffin-0.99.2/muffin/utils.py
--rw-r--r--   0        0        0     2992 2023-08-07 14:02:33.286857 muffin-0.99.2/pyproject.toml
--rw-r--r--   0        0        0    11329 1970-01-01 00:00:00.000000 muffin-0.99.2/PKG-INFO
+-rw-r--r--   0        0        0     9874 2023-08-18 05:46:33.438376 muffin-0.99.3/README.rst
+-rw-r--r--   0        0        0     1016 2023-08-18 05:46:33.442376 muffin-0.99.3/muffin/__init__.py
+-rw-r--r--   0        0        0     5213 2023-08-18 05:46:33.442376 muffin-0.99.3/muffin/app.py
+-rw-r--r--   0        0        0       71 2023-08-18 05:46:33.442376 muffin-0.99.3/muffin/constants.py
+-rw-r--r--   0        0        0      701 2023-08-18 05:46:33.442376 muffin-0.99.3/muffin/errors.py
+-rw-r--r--   0        0        0     3755 2023-08-18 05:46:33.442376 muffin-0.99.3/muffin/handler.py
+-rw-r--r--   0        0        0     8820 2023-08-18 05:46:33.442376 muffin-0.99.3/muffin/manage.py
+-rw-r--r--   0        0        0     2877 2023-08-18 05:46:33.442376 muffin-0.99.3/muffin/plugins.py
+-rw-r--r--   0        0        0        0 2023-08-18 05:46:33.442376 muffin-0.99.3/muffin/py.typed
+-rw-r--r--   0        0        0     2679 2023-08-18 05:46:33.442376 muffin-0.99.3/muffin/pytest.py
+-rw-r--r--   0        0        0      153 2023-08-18 05:46:33.442376 muffin-0.99.3/muffin/types.py
+-rw-r--r--   0        0        0     2905 2023-08-18 05:46:33.442376 muffin-0.99.3/muffin/utils.py
+-rw-r--r--   0        0        0     2992 2023-08-18 05:46:33.442376 muffin-0.99.3/pyproject.toml
+-rw-r--r--   0        0        0    11329 1970-01-01 00:00:00.000000 muffin-0.99.3/PKG-INFO
```

### Comparing `muffin-0.99.2/README.rst` & `muffin-0.99.3/README.rst`

 * *Files identical despite different names*

### Comparing `muffin-0.99.2/muffin/__init__.py` & `muffin-0.99.3/muffin/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin-0.99.2/muffin/app.py` & `muffin-0.99.3/muffin/app.py`

 * *Files identical despite different names*

### Comparing `muffin-0.99.2/muffin/errors.py` & `muffin-0.99.3/muffin/errors.py`

 * *Files identical despite different names*

### Comparing `muffin-0.99.2/muffin/handler.py` & `muffin-0.99.3/muffin/handler.py`

 * *Files identical despite different names*

### Comparing `muffin-0.99.2/muffin/manage.py` & `muffin-0.99.3/muffin/manage.py`

 * *Files identical despite different names*

### Comparing `muffin-0.99.2/muffin/plugins.py` & `muffin-0.99.3/muffin/plugins.py`

 * *Files identical despite different names*

### Comparing `muffin-0.99.2/muffin/pytest.py` & `muffin-0.99.3/muffin/pytest.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,18 +48,16 @@
 
 
 @pytest.fixture(scope="session")
 async def app(pytestconfig, request, aiolib):  # noqa: ARG001
     """Load an application, run lifespan events, prepare plugins."""
     if not pytestconfig.app:
         logging.warning(
-            (
-                "Improperly configured. Please set ``muffin_app`` in your pytest config. "
-                "Or use ``--muffin-app`` command option."
-            ),
+            "Improperly configured. Please set ``muffin_app`` in your pytest config. "
+            "Or use ``--muffin-app`` command option.",
         )
         return
 
     from muffin.utils import import_app
 
     muffin_app = import_app(pytestconfig.app)
     msg = f"Setup application '{muffin_app.cfg.name}'"
@@ -79,18 +77,19 @@
     plugin_conf = [
         plugin.conftest
         for plugin in app.plugins.values()
         if hasattr(plugin, "conftest") and plugin.conftest
     ]
 
     # Manage lifespan and prepare plugins
-    async with AsyncExitStack() as stack, manage_lifespan(app):
+    async with AsyncExitStack() as stack:
         for conftest in plugin_conf:
             await stack.enter_async_context(conftest())
 
-        yield app
+        async with manage_lifespan(app):
+            yield app
 
 
 @pytest.fixture()
 def client(app):
     """Generate a test client for the app."""
     return ASGITestClient(app)
```

### Comparing `muffin-0.99.2/muffin/utils.py` & `muffin-0.99.3/muffin/utils.py`

 * *Files identical despite different names*

### Comparing `muffin-0.99.2/pyproject.toml` & `muffin-0.99.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin"
-version = "0.99.2"
+version = "0.99.3"
 description = "Muffin is a fast, simple and asyncronous web-framework for Python 3 (asyncio, trio, curio)"
 readme = "README.rst"
 license = "MIT"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 keywords = ["asgi", "web", "web framework", "asyncio", "trio", "curio"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
```

### Comparing `muffin-0.99.2/PKG-INFO` & `muffin-0.99.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin
-Version: 0.99.2
+Version: 0.99.3
 Summary: Muffin is a fast, simple and asyncronous web-framework for Python 3 (asyncio, trio, curio)
 Home-page: https://github.com/klen/muffin
 License: MIT
 Keywords: asgi,web,web framework,asyncio,trio,curio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

