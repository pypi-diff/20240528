# Comparing `tmp/mango-framework-1.4.2.tar.gz` & `tmp/mango-framework-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-framework-1.4.2.tar", last modified: Sun Mar 10 14:52:29 2024, max compression
+gzip compressed data, was "mango-framework-1.5.0.tar", last modified: Tue May 28 15:03:26 2024, max compression
```

## Comparing `mango-framework-1.4.2.tar` & `mango-framework-1.5.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2024-03-10 14:52:29.404670 mango-framework-1.4.2/
--rw-r--r--   0 mohammed   (501) staff       (20)     9687 2024-03-10 14:52:29.404417 mango-framework-1.4.2/PKG-INFO
--rw-r--r--   0 mohammed   (501) staff       (20)     9028 2024-03-10 14:17:53.000000 mango-framework-1.4.2/README.md
--rw-r--r--   0 mohammed   (501) staff       (20)    22625 2024-03-10 14:52:01.000000 mango-framework-1.4.2/mango.py
-drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2024-03-10 14:52:29.403937 mango-framework-1.4.2/mango_framework.egg-info/
--rw-r--r--   0 mohammed   (501) staff       (20)     9687 2024-03-10 14:52:29.000000 mango-framework-1.4.2/mango_framework.egg-info/PKG-INFO
--rw-r--r--   0 mohammed   (501) staff       (20)      190 2024-03-10 14:52:29.000000 mango-framework-1.4.2/mango_framework.egg-info/SOURCES.txt
--rw-r--r--   0 mohammed   (501) staff       (20)        1 2024-03-10 14:52:29.000000 mango-framework-1.4.2/mango_framework.egg-info/dependency_links.txt
--rw-r--r--   0 mohammed   (501) staff       (20)        1 2024-03-10 14:52:29.000000 mango-framework-1.4.2/mango_framework.egg-info/top_level.txt
--rw-r--r--   0 mohammed   (501) staff       (20)       98 2024-03-10 14:20:31.000000 mango-framework-1.4.2/req.py
--rw-r--r--   0 mohammed   (501) staff       (20)       38 2024-03-10 14:52:29.404728 mango-framework-1.4.2/setup.cfg
--rw-r--r--   0 mohammed   (501) staff       (20)      903 2024-03-08 10:47:41.000000 mango-framework-1.4.2/setup.py
+drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2024-05-28 15:03:26.538116 mango-framework-1.5.0/
+-rw-r--r--   0 mohammed   (501) staff       (20)     9687 2024-05-28 15:03:26.537918 mango-framework-1.5.0/PKG-INFO
+-rw-r--r--   0 mohammed   (501) staff       (20)     9028 2024-03-10 14:17:53.000000 mango-framework-1.5.0/README.md
+-rw-r--r--   0 mohammed   (501) staff       (20)    24833 2024-05-28 15:01:10.000000 mango-framework-1.5.0/mango.py
+-rw-r--r--   0 mohammed   (501) staff       (20)     1615 2024-03-13 14:56:15.000000 mango-framework-1.5.0/mango_async.py
+drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2024-05-28 15:03:26.537624 mango-framework-1.5.0/mango_framework.egg-info/
+-rw-r--r--   0 mohammed   (501) staff       (20)     9687 2024-05-28 15:03:26.000000 mango-framework-1.5.0/mango_framework.egg-info/PKG-INFO
+-rw-r--r--   0 mohammed   (501) staff       (20)      205 2024-05-28 15:03:26.000000 mango-framework-1.5.0/mango_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)        1 2024-05-28 15:03:26.000000 mango-framework-1.5.0/mango_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)        1 2024-05-28 15:03:26.000000 mango-framework-1.5.0/mango_framework.egg-info/top_level.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)     2930 2024-03-25 07:37:34.000000 mango-framework-1.5.0/req.py
+-rw-r--r--   0 mohammed   (501) staff       (20)       38 2024-05-28 15:03:26.538163 mango-framework-1.5.0/setup.cfg
+-rw-r--r--   0 mohammed   (501) staff       (20)      903 2024-03-08 10:47:41.000000 mango-framework-1.5.0/setup.py
```

### Comparing `mango-framework-1.4.2/PKG-INFO` & `mango-framework-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-framework
-Version: 1.4.2
+Version: 1.5.0
 Summary: A lightweight and highly customizable Python framework for building web applications
 Home-page: https://github.com/momo-AUX1/mango
 Author: Mohammed
 Author-email: fdlnaal@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `mango-framework-1.4.2/README.md` & `mango-framework-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mango-framework-1.4.2/mango.py` & `mango-framework-1.5.0/mango.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,23 @@
+import threading
 from wsgiref.simple_server import make_server
 import json
 from os.path import join
 from urllib.parse import parse_qs
 import mimetypes
 import cgi
+import os
+import sys
+import time
+
+try:
+   from jinja2 import Environment, FileSystemLoader, select_autoescape, TemplateNotFound
+   __jinja2__ = True
+except:
+    pass
 
 templates_path : str = 'templates'
 
 files_path : str = 'files'
 
 static_path : str = 'static'
 
@@ -17,18 +27,21 @@
 
 static_permissive : bool = False
 
 debug : bool = False
 
 debug_info : str = ""
 
-__version__ : str = '1.4.2'
+__version__ : str = '1.5.0'
 
 __app_url__ : str = 'https://pypi.org/project/mango-framework/'
 
+if __jinja2__:
+    env = Environment(loader=FileSystemLoader(templates_path), autoescape=select_autoescape(['html', 'xml']))
+
 # Default route
 
 def index():
   return html
 
 routes : dict = {'/': index}
 
@@ -68,14 +81,16 @@
 page_500 : str = "<h1>500 Internal Server Error</h1>"
 
 
 # ANSI escape codes to set text color
 ESC = "\x1b["  # ANSI escape code
 YELLOW_TEXT = ESC + "33;1m"  # Bright Yellow
 BLUE_TEXT = ESC + "34;1m"  # Bright Blue
+RED_TEXT = ESC + "35;1m" # Bright Red
+GREEN_TEXT = ESC + "32;1m" # Bright Green
 RESET = ESC + "0m"  # Reset to default color
 
 
 # Main application function
 
 def app(environ, start_response):
   try:
@@ -84,14 +99,15 @@
     method = environ['REQUEST_METHOD']
     req = environ['CONTENT_TYPE']
     query_string = environ.get('QUERY_STRING', '')
     
     if '=' in query_string:
       get_params_unsanitzed = parse_qs(query_string)
       get_params = {k: v[0] if len(v) == 1 else v for k, v in get_params_unsanitzed.items()}
+      print("get_params", get_params)
     else:
       get_params = {}
 
 
     if path in routes and method == 'POST':
       if req == 'application/json':
         length = int(environ.get('CONTENT_LENGTH', 0))
@@ -187,15 +203,15 @@
               return [response_data.encode('utf-8')]
       return [response.encode()]
     except:
       return [response]
   
   except Exception as e:
     global debug_info
-    print("Error: ", e)
+    print(f"{RED_TEXT}Error: {e} {RESET}")
     debug_info = str(e)  
     start_response(*INTERNAL_SERVER_ERROR)
     if debug:
         response_body = html_500.format(debug_info=debug_info, __version__=__version__, __app_url__=__app_url__)
     else:
         response_body = page_500
     return [response_body.encode()]
@@ -204,23 +220,37 @@
 
 def run(host:str = '127.0.0.1', port:int = 5000, debug_mode=False) -> None:
   "Function to run the application. expects host in string format and port in integer format. If debug mode is set to True, it will show the error 500 page with the error details. Returns None"
   global debug
   debug = debug_mode
   server = make_server(host, port, app)
   print(f"{YELLOW_TEXT}This is a development server. Do not use it in a production deployment.{RESET}")
+
+  if __jinja2__:
+    print(f"{GREEN_TEXT}Jinja2 is installed. The app will use it to render templates.{RESET}")
+
   if debug:
     print(f"{BLUE_TEXT}Debug mode is on. The server will show debug info when a 404 or 500 errors occurs.{RESET}")
+    monitor_thread = threading.Thread(target=monitor_changes, args=('.',), daemon=True)
+    monitor_thread.start()
+
   print(f'Running at http://{host}:{port}')
   server.serve_forever()
 
 # Helper functions
 
 def render(template:str, context:dict = None) -> str :
-    "Function to render a template. Expects template name and context as dictionary. Returns a string."
+    "Function to render a template. Expects template name and context as dictionary. Returns a string. If jinja2 is not found it will only handle simple contexts otherwise it will handle jinja2 templates."
+    if __jinja2__:
+        try:
+            template = env.get_template(template)
+            return template.render(context)
+        except TemplateNotFound:
+            template = env.from_string(template)
+            return template.render(context)
     try:
       with open(join(templates_path, template), 'r') as f:
         template = f.read()
     except:
       try:
         with open(template, 'r') as f:
           template = f.read()
@@ -346,14 +376,19 @@
    static_url = url
 
 def set_static_folder(path:str) -> None:
     "Function to set the static folder. Expects a string. Returns a None."
     global static_path
     static_path = path
 
+def set_templates_folder(path:str) -> None:
+    "Function to set the templates folder. Expects a string. Returns a None. Useful if jinja2 is installed to tell it where to find the template otherwise it isn't needed."
+    global templates_path
+    templates_path = path
+
 def set_routes(paths:dict) -> None:
     "Function to set the routes manually. Expects a dictionary. Returns a None. Useful if you want to do it more akin to django's seperation of concerns."
     global routes
     routes = paths
 
 def set_static_permissive(value:bool = None) -> None:
     "Function to set the static permissive. Expects a boolean. Returns a None."
@@ -404,14 +439,34 @@
             print(f"Registered new route: {path} with dynamic handler for {handler_type}")
 
     print("Finished loading routes from JSON. Current routes dictionary:")
     for route_path, func in routes.items():
         print(f"Path: {route_path}, Handler Function: {func.__name__ if hasattr(func, '__name__') else 'Anonymous Function'}")
 
 
+def monitor_changes(directory: str, interval: int=1) -> None:
+    """Monitor the directory for changes and restart the server if a change is detected."""
+    mtimes = {}
+    while True:
+        for root, _, files in os.walk(directory):
+            for filename in files:
+                if filename.endswith('.py'):
+                    filepath = os.path.join(root, filename)
+                    try:
+                        mtime = os.path.getmtime(filepath)
+                        if filepath not in mtimes:
+                            mtimes[filepath] = mtime
+                        elif mtime != mtimes[filepath]:
+                            print(f"{YELLOW_TEXT}Detected change in {filepath}. Reloading...{RESET}")
+                            os.execv(sys.executable, ['python'] + sys.argv)
+                    except FileNotFoundError:
+                        pass
+        time.sleep(interval)
+
+
 
 
 # Default page
 
 html : str = f"""
 <!DOCTYPE html>
 <html>
@@ -699,8 +754,11 @@
     <footer>
         Version: {__version__}
         <br>
         <a href="{__app_url__}" class="link">Check out the development!</a>
     </footer>
 </body>
 </html>
-"""
+"""
+
+
+
```

### Comparing `mango-framework-1.4.2/mango_framework.egg-info/PKG-INFO` & `mango-framework-1.5.0/mango_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-framework
-Version: 1.4.2
+Version: 1.5.0
 Summary: A lightweight and highly customizable Python framework for building web applications
 Home-page: https://github.com/momo-AUX1/mango
 Author: Mohammed
 Author-email: fdlnaal@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `mango-framework-1.4.2/setup.py` & `mango-framework-1.5.0/setup.py`

 * *Files identical despite different names*

