# Comparing `tmp/streamlit-deephaven-0.0.5.tar.gz` & `tmp/streamlit-deephaven-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-deephaven-0.0.5.tar", last modified: Mon Apr 10 16:32:55 2023, max compression
+gzip compressed data, was "streamlit-deephaven-0.0.6.tar", last modified: Tue May 28 19:50:48 2024, max compression
```

## Comparing `streamlit-deephaven-0.0.5.tar` & `streamlit-deephaven-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 bender     (501) staff       (20)        0 2023-04-10 16:32:55.492190 streamlit-deephaven-0.0.5/
--rw-r--r--   0 bender     (501) staff       (20)     1063 2023-04-02 02:44:37.000000 streamlit-deephaven-0.0.5/LICENSE
--rw-r--r--   0 bender     (501) staff       (20)      359 2023-04-10 16:32:55.492052 streamlit-deephaven-0.0.5/PKG-INFO
--rw-r--r--   0 bender     (501) staff       (20)     1105 2023-04-10 16:31:53.000000 streamlit-deephaven-0.0.5/README.md
--rw-r--r--   0 bender     (501) staff       (20)       38 2023-04-10 16:32:55.492230 streamlit-deephaven-0.0.5/setup.cfg
--rw-r--r--   0 bender     (501) staff       (20)      768 2023-04-10 16:32:30.000000 streamlit-deephaven-0.0.5/setup.py
-drwxr-xr-x   0 bender     (501) staff       (20)        0 2023-04-10 16:32:55.491183 streamlit-deephaven-0.0.5/streamlit_deephaven/
--rw-r--r--   0 bender     (501) staff       (20)     5048 2023-04-10 16:31:53.000000 streamlit-deephaven-0.0.5/streamlit_deephaven/__init__.py
-drwxr-xr-x   0 bender     (501) staff       (20)        0 2023-04-10 16:32:55.491860 streamlit-deephaven-0.0.5/streamlit_deephaven.egg-info/
--rw-r--r--   0 bender     (501) staff       (20)      359 2023-04-10 16:32:55.000000 streamlit-deephaven-0.0.5/streamlit_deephaven.egg-info/PKG-INFO
--rw-r--r--   0 bender     (501) staff       (20)      272 2023-04-10 16:32:55.000000 streamlit-deephaven-0.0.5/streamlit_deephaven.egg-info/SOURCES.txt
--rw-r--r--   0 bender     (501) staff       (20)        1 2023-04-10 16:32:55.000000 streamlit-deephaven-0.0.5/streamlit_deephaven.egg-info/dependency_links.txt
--rw-r--r--   0 bender     (501) staff       (20)       41 2023-04-10 16:32:55.000000 streamlit-deephaven-0.0.5/streamlit_deephaven.egg-info/requires.txt
--rw-r--r--   0 bender     (501) staff       (20)       20 2023-04-10 16:32:55.000000 streamlit-deephaven-0.0.5/streamlit_deephaven.egg-info/top_level.txt
+drwxrwxr-x   0 bender    (1000) bender    (1000)        0 2024-05-28 19:50:48.290757 streamlit-deephaven-0.0.6/
+-rw-rw-r--   0 bender    (1000) bender    (1000)     1063 2023-04-06 19:05:25.000000 streamlit-deephaven-0.0.6/LICENSE
+-rw-rw-r--   0 bender    (1000) bender    (1000)      395 2024-05-28 19:50:48.290757 streamlit-deephaven-0.0.6/PKG-INFO
+-rw-rw-r--   0 bender    (1000) bender    (1000)     1549 2024-05-28 19:47:56.000000 streamlit-deephaven-0.0.6/README.md
+-rw-rw-r--   0 bender    (1000) bender    (1000)       38 2024-05-28 19:50:48.290757 streamlit-deephaven-0.0.6/setup.cfg
+-rw-rw-r--   0 bender    (1000) bender    (1000)      768 2024-05-28 19:47:56.000000 streamlit-deephaven-0.0.6/setup.py
+drwxrwxr-x   0 bender    (1000) bender    (1000)        0 2024-05-28 19:50:48.290757 streamlit-deephaven-0.0.6/streamlit_deephaven/
+-rw-rw-r--   0 bender    (1000) bender    (1000)     6917 2024-05-28 19:47:56.000000 streamlit-deephaven-0.0.6/streamlit_deephaven/__init__.py
+drwxrwxr-x   0 bender    (1000) bender    (1000)        0 2024-05-28 19:50:48.290757 streamlit-deephaven-0.0.6/streamlit_deephaven.egg-info/
+-rw-rw-r--   0 bender    (1000) bender    (1000)      395 2024-05-28 19:50:48.000000 streamlit-deephaven-0.0.6/streamlit_deephaven.egg-info/PKG-INFO
+-rw-rw-r--   0 bender    (1000) bender    (1000)      272 2024-05-28 19:50:48.000000 streamlit-deephaven-0.0.6/streamlit_deephaven.egg-info/SOURCES.txt
+-rw-rw-r--   0 bender    (1000) bender    (1000)        1 2024-05-28 19:50:48.000000 streamlit-deephaven-0.0.6/streamlit_deephaven.egg-info/dependency_links.txt
+-rw-rw-r--   0 bender    (1000) bender    (1000)       41 2024-05-28 19:50:48.000000 streamlit-deephaven-0.0.6/streamlit_deephaven.egg-info/requires.txt
+-rw-rw-r--   0 bender    (1000) bender    (1000)       20 2024-05-28 19:50:48.000000 streamlit-deephaven-0.0.6/streamlit_deephaven.egg-info/top_level.txt
```

### Comparing `streamlit-deephaven-0.0.5/LICENSE` & `streamlit-deephaven-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-deephaven-0.0.5/README.md` & `streamlit-deephaven-0.0.6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -33,12 +33,19 @@
 
 3. Run the streamlit application:
 
 ```
 streamlit run deephaven_app.py
 ```
 
+## Alternate Deephaven Server URL
+By default, the Deephaven server is located at `http://localhost:{port}`, where `{port}` is the port set in the Deephaven server creation call. If the server is not there, such as when running Streamlit in a Docker container, modify the `DEEPHAVEN_ST_URL` environmental variable to the correct URL before calling `display_dh`. 
+```python
+import os
+os.environ["DEEPHAVEN_ST_URL"] = "http://localhost:1234"
+```
+
 For more information on running Streamlit, see the [Streamlit documentation](https://docs.streamlit.io/).
 
 ## Development
 
 See [development guide](./development.md) for instructions on how to develop this package.
```

### Comparing `streamlit-deephaven-0.0.5/setup.py` & `streamlit-deephaven-0.0.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit-deephaven",
-    version="0.0.5",
+    version="0.0.6",
     author="Deephaven Data Labs",
     author_email="support@deephaven.io",
     description="Streamlit Deephaven Component",
     long_description="Use Deephaven within Streamlit and display widgets",
     long_description_content_type="text/plain",
     url="https://github.com/deephaven/streamlit-deephaven",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-deephaven-0.0.5/streamlit_deephaven/__init__.py` & `streamlit-deephaven-0.0.6/streamlit_deephaven/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,77 +1,85 @@
 import __main__
 import os
 import streamlit.components.v1 as components
 from uuid import uuid4
-import streamlit as st
-from typing import Dict, List, Optional
+from typing import List, Optional
+import base64
+
+TABLE_TYPES = {"deephaven.table.Table", "pandas.core.frame.DataFrame", "pydeephaven.table.Table"}
+FIGURE_TYPES = {"deephaven.plot.figure.Figure"}
 
 DEV_MODE = os.environ.get("DH_DEV_MODE", False)
 
 def _str_object_type(obj):
   """Returns the object type as a string value"""
   return f"{obj.__class__.__module__}.{obj.__class__.__name__}"
 
 def _path_for_object(obj):
   """Return the iframe path for the specified object. Inspects the class name to determine."""
   name = _str_object_type(obj)
 
-  if name in ('deephaven.table.Table', 'pandas.core.frame.DataFrame'):
-    return 'table'
-  if name == 'deephaven.plot.figure.Figure':
-    return 'chart'
-  raise TypeError(f"Unknown object type: {name}")
+  if name in TABLE_TYPES:
+      return "table"
+  if name in FIGURE_TYPES:
+      return "chart"
+
+  # No special handling for this type, just try it as a widget
+  return "widget"
 
 def open_ctx():
   """Open the Deephaven execution context. Required before performing any operations on the server."""
   from deephaven_server import Server
   # We store the execution context as an attribute on the server instance
   if not hasattr(Server.instance, '__deephaven_ctx'):
     print("Initializing Context...")
 
     from deephaven.execution_context import get_exec_ctx
     Server.instance.__deephaven_ctx = get_exec_ctx()
   print("Opening context...")
   Server.instance.__deephaven_ctx.j_exec_ctx.open()
   return Server.instance.__deephaven_ctx
 
-def start_server(host: Optional[str] = None, port: Optional[int] = None, jvm_args: Optional[List[str]] = None, dh_args: Dict[str, str] = {}):
+def start_server(host: Optional[str] = None, port: Optional[int] = None, jvm_args: Optional[List[str]] = None):
   """Initialize the Deephaven server. This will start the server if it is not already running."""
   from deephaven_server import Server
   if Server.instance is None:
     print("Initializing Deephaven Server...")
-    s = Server(host=host, port=port, jvm_args=jvm_args, dh_args=dh_args)
+    s = Server(host=host, port=port, jvm_args=jvm_args)
     s.start()
     print("Deephaven Server listening on port", s.port)
 
   open_ctx()
   return Server.instance
 
 # Create a wrapper function for the component. This is an optional
 # best practice - we could simply expose the component function returned by
 # `declare_component` and call it done. The wrapper allows us to customize
 # our component's API: we can pre-process its input args, post-process its
 # output value, and add a docstring for users.
-def display_dh(widget, height=600, width=None, object_id=None, key=None):
+def display_dh(widget, height=600, width=None, object_id=None, key=None, session=None):
     """Display a Deephaven widget.
 
     Parameters
     ----------
-    widget: deephaven.table.Table | deephaven.plot.figure.Figure | pandas.core.frame.DataFrame
-        The Deephaven widget we want to display
+    widget: deephaven.table.Table | deephaven.plot.figure.Figure | pandas.core.frame.DataFrame | str
+        The Deephaven widget we want to display. If a string is passed, a session must be specified.
     height: int
         The height of the widget in pixels
     width: int
         The width of the widget in pixels
     object_id: string
-        The variable name of the Deephaven widget we want to display
+        The variable name of the Deephaven widget we want to display.
     key: str or None
         An optional key that uniquely identifies this component. If this is
         None, and the component's arguments are changed, the component will
         be re-mounted in the Streamlit frontend and lose its current state.
+    session: pydeephaven.Session
+        The session to use when displaying a remote Deephaven widget by name.
+        Must be specified if a string is passed as the widget parameter.
 
     Returns
     -------
     string
         The object_id of the created object
 
     """
@@ -81,24 +89,70 @@
     # will be sent to the frontend, where they'll be available in an "args"
     # dictionary.
     #
     # "default" is a special argument that specifies the initial return
     # value of the component before the user has interacted with it.
 
     # Generate a new table ID using a UUID prepended with a `__w_` prefix if name not specified
-    if object_id is None:
+
+    if isinstance(widget, str):
+        # a string widget must match the object_id
+        object_id = widget
+    elif object_id is None:
         object_id = f"__w_{str(uuid4()).replace('-', '_')}"
 
-    # Generate the iframe_url from the object type
-    server_url = f"http://localhost:{Server.instance.port}"
-    iframe_url = f"{server_url}/iframe/{_path_for_object(widget)}/?name={object_id}"
-    object_type = _str_object_type(widget)
 
-    # Add the table to the main modules globals list so it can be retrieved by the iframe
-    __main__.__dict__[object_id] = widget
+    params = {"name": object_id}
+
+    if isinstance(widget, str):
+        if session is None:
+            raise ValueError(
+                "session must be specified when using a remote pydeephaven object by name"
+            )
+        port = session.port
+        server_url = f"http://{session.host}:{port}/"
+    elif _str_object_type(widget) == "pydeephaven.table.Table":
+        session = widget.session
+
+        if b"envoy-prefix" in session._extra_headers:
+            params["envoyPrefix"] = session._extra_headers[b"envoy-prefix"].decode(
+                "ascii"
+            )
+
+        port = widget.session.port
+        server_url = f"http://{widget.session.host}:{port}/"
+
+        if hasattr(session, "session_manager"):
+            params["authProvider"] = "parent"
+            # We have a DnD session, and we can get the authentication and connection details from the session manager
+            token = base64.b64encode(
+                session.session_manager.auth_client.get_token(
+                    "RemoteQueryProcessor"
+                ).SerializeToString()
+            ).decode("us-ascii")
+            server_url = (
+                widget.session.pqinfo().state.connectionDetails.staticUrl
+            )
+
+        session.bind_table(object_id, widget)
+    else:
+        port = Server.instance.port
+        server_url = f"http://localhost:{port}/"
+
+        # Add the table to the main modules globals list so it can be retrieved by the iframe
+        __main__.__dict__[object_id] = widget
+
+    if "DEEPHAVEN_ST_URL" in os.environ:
+      server_url = os.environ["DEEPHAVEN_ST_URL"]
+
+    if not server_url.endswith("/"):
+      server_url = f"{server_url}/"
+
+    # Generate the iframe_url from the object type
+    iframe_url = f"{server_url}iframe/{_path_for_object(widget)}/?name={object_id}"
 
     # We don't really need the component value in the Deephaven example, since we're just creating a display widget...
     # Maybe if we were making a one click widget, that would make sense...
     # component_value = _component_func(iframe_url=iframe_url, object_type=object_type, width=width, height=height, key=key, default=0)
     return components.iframe(iframe_url, height=height, width=width)
```

