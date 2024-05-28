# Comparing `tmp/cheeseapi-1.2.3.tar.gz` & `tmp/cheeseapi-1.3.0.tar.gz`

## Comparing `cheeseapi-1.2.3.tar` & `cheeseapi-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/__init__.py
--rw-r--r--   0        0        0     7512 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/app.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/cors.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/exception.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/file.py
--rw-r--r--   0        0        0    33258 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/handle.py
--rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/protocol.py
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/request.py
--rw-r--r--   0        0        0    17620 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/response.py
--rw-r--r--   0        0        0    13136 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/route.py
--rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/schedule.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/server.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/signal.py
--rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/text.py
--rw-r--r--   0        0        0    13085 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/validator.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/websocket.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/CheeseAPI/workspace.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/LICENSE
--rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 cheeseapi-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/__init__.py
+-rw-r--r--   0        0        0     7512 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/app.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/cors.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/exception.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/file.py
+-rw-r--r--   0        0        0    33258 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/handle.py
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/protocol.py
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/request.py
+-rw-r--r--   0        0        0    17620 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/response.py
+-rw-r--r--   0        0        0    13136 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/route.py
+-rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/schedule.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/server.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/signal.py
+-rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/text.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/validator.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/websocket.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/CheeseAPI/workspace.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/LICENSE
+-rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/README.md
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5532 2020-02-02 00:00:00.000000 cheeseapi-1.3.0/PKG-INFO
```

### Comparing `cheeseapi-1.2.3/CheeseAPI/app.py` & `cheeseapi-1.3.0/CheeseAPI/app.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.3/CheeseAPI/cors.py` & `cheeseapi-1.3.0/CheeseAPI/cors.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.3/CheeseAPI/exception.py` & `cheeseapi-1.3.0/CheeseAPI/exception.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.3/CheeseAPI/file.py` & `cheeseapi-1.3.0/CheeseAPI/file.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.3/CheeseAPI/handle.py` & `cheeseapi-1.3.0/CheeseAPI/handle.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.3/CheeseAPI/protocol.py` & `cheeseapi-1.3.0/CheeseAPI/protocol.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.3/CheeseAPI/request.py` & `cheeseapi-1.3.0/CheeseAPI/request.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.3/CheeseAPI/response.py` & `cheeseapi-1.3.0/CheeseAPI/response.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.3/CheeseAPI/route.py` & `cheeseapi-1.3.0/CheeseAPI/route.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.3/CheeseAPI/schedule.py` & `cheeseapi-1.3.0/CheeseAPI/schedule.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.3/CheeseAPI/server.py` & `cheeseapi-1.3.0/CheeseAPI/server.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.3/CheeseAPI/signal.py` & `cheeseapi-1.3.0/CheeseAPI/signal.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.3/CheeseAPI/text.py` & `cheeseapi-1.3.0/CheeseAPI/text.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.3/CheeseAPI/websocket.py` & `cheeseapi-1.3.0/CheeseAPI/websocket.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.3/CheeseAPI/workspace.py` & `cheeseapi-1.3.0/CheeseAPI/workspace.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.3/LICENSE` & `cheeseapi-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.3/README.md` & `cheeseapi-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cheeseapi-1.2.3/pyproject.toml` & `cheeseapi-1.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "hatchling" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "CheeseAPI"
-version = "1.2.3"
+version = "1.3.0"
 description = "一款web协程框架。"
 readme = "README.md"
 license-files = { paths = [ "LICENSE" ] }
 authors = [
     { name = "Cheese Unknown", email = "cheese@cheese.ren" }
 ]
 keywords = [ 'API', 'BackEnd' ]
@@ -16,15 +16,17 @@
 dependencies = [
     "CheeseLog==1.0.*",
     "xmltodict",
     "websockets",
     "uvloop",
     "httptools",
     "CheeseSignal==1.1.*",
-    "dill"
+    "dill",
+    "pydantic",
+    "email-validator"
 ]
 
 [project.urls]
 Source = "https://github.com/CheeseUnknown/CheeseAPI"
 
 [tool.hatch.build.targets.sdist]
 include = [ "/CheeseAPI" ]
```

### Comparing `cheeseapi-1.2.3/PKG-INFO` & `cheeseapi-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.3
 Name: CheeseAPI
-Version: 1.2.3
+Version: 1.3.0
 Summary: 一款web协程框架。
 Project-URL: Source, https://github.com/CheeseUnknown/CheeseAPI
 Author-email: Cheese Unknown <cheese@cheese.ren>
 License-File: LICENSE
 Keywords: API,BackEnd
 Requires-Dist: cheeselog==1.0.*
 Requires-Dist: cheesesignal==1.1.*
 Requires-Dist: dill
+Requires-Dist: email-validator
 Requires-Dist: httptools
+Requires-Dist: pydantic
 Requires-Dist: uvloop
 Requires-Dist: websockets
 Requires-Dist: xmltodict
 Description-Content-Type: text/markdown
 
 # **CheeseAPI**
```

