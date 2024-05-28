# Comparing `tmp/cheeseapi_websocket-1.0.2.tar.gz` & `tmp/cheeseapi_websocket-1.0.3.tar.gz`

## Comparing `cheeseapi_websocket-1.0.2.tar` & `cheeseapi_websocket-1.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.2/CheeseAPI_Websocket/__init__.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.2/CheeseAPI_Websocket/handle.py
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.2/CheeseAPI_Websocket/websocket.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.2/LICENSE
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.2/README.md
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.3/CheeseAPI_Websocket/__init__.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.3/CheeseAPI_Websocket/handle.py
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.3/CheeseAPI_Websocket/websocket.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.3/README.md
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.3/PKG-INFO
```

### Comparing `cheeseapi_websocket-1.0.2/CheeseAPI_Websocket/handle.py` & `cheeseapi_websocket-1.0.3/CheeseAPI_Websocket/handle.py`

 * *Files identical despite different names*

### Comparing `cheeseapi_websocket-1.0.2/CheeseAPI_Websocket/websocket.py` & `cheeseapi_websocket-1.0.3/CheeseAPI_Websocket/websocket.py`

 * *Files identical despite different names*

### Comparing `cheeseapi_websocket-1.0.2/LICENSE` & `cheeseapi_websocket-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cheeseapi_websocket-1.0.2/README.md` & `cheeseapi_websocket-1.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,42 @@
+Metadata-Version: 2.3
+Name: CheeseAPI_Websocket
+Version: 1.0.3
+Summary: 一款基于CheeseAPI的升级款Websocket插件。
+Project-URL: Source, https://github.com/CheeseUnknown/CheeseAPI_Websocket
+Author-email: Cheese Unknown <cheese@cheese.ren>
+License-File: LICENSE
+Keywords: CheeseAPI,websocket
+Requires-Dist: cheeseapi==1.3.*
+Requires-Dist: redis
+Description-Content-Type: text/markdown
+
 # **CheeseAPI_Websocket**
 
 ## **介绍**
 
 一款基于[CheeseAPI](https://github.com/CheeseUnknown/CheeseAPI)的升级款Websocket插件，它能够解决在多worker下websocket的通讯问题，前提是需要引入redis。
 
 ## **安装**
 
 目前仅保证支持3.11及以上的python。
 
 ```bash
 pip install CheeseAPI_Websocket
 ```
 
+对应CheeseAPI版本：
+
+| 版本 | CheeseAPI版本 |
+| - | - |
+| 1.0.3 | 1.3.* |
+| 1.0.2 | 1.2.* |
+| 1.0.1 | 1.1.* |
+| 1.0.0 | 1.0.* |
+
 ## **使用**
 
 CheeseAPI_Websocket是[CheeseAPI](https://github.com/CheeseUnknown/CheeseAPI)的一款插件，它需要依赖于[CheeseAPI](https://github.com/CheeseUnknown/CheeseAPI)才能运行。
 
 ```python
 import threading, time
```

### Comparing `cheeseapi_websocket-1.0.2/pyproject.toml` & `cheeseapi_websocket-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = [ "hatchling" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "CheeseAPI_Websocket"
-version = "1.0.2"
+version = "1.0.3"
 description = "一款基于CheeseAPI的升级款Websocket插件。"
 readme = "README.md"
 license-files = { paths = [ "LICENSE" ] }
 authors = [
     { name = "Cheese Unknown", email = "cheese@cheese.ren" }
 ]
 keywords = [ 'CheeseAPI', 'websocket' ]
 
 dependencies = [
-    "CheeseAPI==1.2.*",
+    "CheeseAPI==1.3.*",
     "redis"
 ]
 
 [project.urls]
 Source = "https://github.com/CheeseUnknown/CheeseAPI_Websocket"
 
 [tool.hatch.build.targets.sdist]
```

### Comparing `cheeseapi_websocket-1.0.2/PKG-INFO` & `cheeseapi_websocket-1.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-Metadata-Version: 2.3
-Name: CheeseAPI_Websocket
-Version: 1.0.2
-Summary: 一款基于CheeseAPI的升级款Websocket插件。
-Project-URL: Source, https://github.com/CheeseUnknown/CheeseAPI_Websocket
-Author-email: Cheese Unknown <cheese@cheese.ren>
-License-File: LICENSE
-Keywords: CheeseAPI,websocket
-Requires-Dist: cheeseapi==1.2.*
-Requires-Dist: redis
-Description-Content-Type: text/markdown
-
 # **CheeseAPI_Websocket**
 
 ## **介绍**
 
 一款基于[CheeseAPI](https://github.com/CheeseUnknown/CheeseAPI)的升级款Websocket插件，它能够解决在多worker下websocket的通讯问题，前提是需要引入redis。
 
 ## **安装**
 
 目前仅保证支持3.11及以上的python。
 
 ```bash
 pip install CheeseAPI_Websocket
 ```
 
+对应CheeseAPI版本：
+
+| 版本 | CheeseAPI版本 |
+| - | - |
+| 1.0.3 | 1.3.* |
+| 1.0.2 | 1.2.* |
+| 1.0.1 | 1.1.* |
+| 1.0.0 | 1.0.* |
+
 ## **使用**
 
 CheeseAPI_Websocket是[CheeseAPI](https://github.com/CheeseUnknown/CheeseAPI)的一款插件，它需要依赖于[CheeseAPI](https://github.com/CheeseUnknown/CheeseAPI)才能运行。
 
 ```python
 import threading, time
```

