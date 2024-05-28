# Comparing `tmp/pyeventengine-0.3.0.tar.gz` & `tmp/pyeventengine-0.3.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeventengine-0.3.0.tar", last modified: Tue May 28 10:27:56 2024, max compression
+gzip compressed data, was "pyeventengine-0.3.0.post1.tar", last modified: Tue May 28 10:43:55 2024, max compression
```

## Comparing `pyeventengine-0.3.0.tar` & `pyeventengine-0.3.0.post1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 10:27:56.222565 pyeventengine-0.3.0/
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 10:27:56.121041 pyeventengine-0.3.0/EventEngine/
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 10:27:56.154549 pyeventengine-0.3.0/EventEngine/Core/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3227 2024-05-28 10:24:33.000000 pyeventengine-0.3.0/EventEngine/Core/__init__.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)    13778 2024-05-28 10:17:54.000000 pyeventengine-0.3.0/EventEngine/Core/_event.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     4525 2024-05-28 10:21:19.000000 pyeventengine-0.3.0/EventEngine/Core/_topic.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3001 2024-05-28 06:54:14.000000 pyeventengine-0.3.0/EventEngine/Core/_topic_c.py
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       43 2024-05-28 10:24:33.000000 pyeventengine-0.3.0/EventEngine/__init__.py
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 10:27:56.163058 pyeventengine-0.3.0/EventEngine/cpp/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     9271 2024-05-28 06:20:25.000000 pyeventengine-0.3.0/EventEngine/cpp/topic_api.cpp
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1066 2024-05-28 06:20:25.000000 pyeventengine-0.3.0/LICENSE
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     2103 2024-05-28 10:27:56.220564 pyeventengine-0.3.0/PKG-INFO
-drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 10:27:56.217565 pyeventengine-0.3.0/PyEventEngine.egg-info/
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     2103 2024-05-28 10:27:56.000000 pyeventengine-0.3.0/PyEventEngine.egg-info/PKG-INFO
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)      350 2024-05-28 10:27:56.000000 pyeventengine-0.3.0/PyEventEngine.egg-info/SOURCES.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2024-05-28 10:27:56.000000 pyeventengine-0.3.0/PyEventEngine.egg-info/dependency_links.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       12 2024-05-28 10:27:56.000000 pyeventengine-0.3.0/PyEventEngine.egg-info/top_level.txt
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1507 2024-05-28 06:20:25.000000 pyeventengine-0.3.0/README.md
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)       79 2024-05-28 10:27:56.224565 pyeventengine-0.3.0/setup.cfg
--rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1733 2024-05-28 10:24:33.000000 pyeventengine-0.3.0/setup.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 10:43:55.460847 pyeventengine-0.3.0.post1/
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 10:43:54.999170 pyeventengine-0.3.0.post1/EventEngine/
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 10:43:55.152214 pyeventengine-0.3.0.post1/EventEngine/Core/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3227 2024-05-28 10:24:33.000000 pyeventengine-0.3.0.post1/EventEngine/Core/__init__.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)    13778 2024-05-28 10:17:54.000000 pyeventengine-0.3.0.post1/EventEngine/Core/_event.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     4525 2024-05-28 10:21:19.000000 pyeventengine-0.3.0.post1/EventEngine/Core/_topic.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     3001 2024-05-28 06:54:14.000000 pyeventengine-0.3.0.post1/EventEngine/Core/_topic_c.py
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       49 2024-05-28 10:43:18.000000 pyeventengine-0.3.0.post1/EventEngine/__init__.py
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 10:43:55.224277 pyeventengine-0.3.0.post1/EventEngine/cpp/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     9271 2024-05-28 06:20:25.000000 pyeventengine-0.3.0.post1/EventEngine/cpp/topic_api.cpp
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1066 2024-05-28 06:20:25.000000 pyeventengine-0.3.0.post1/LICENSE
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     2109 2024-05-28 10:43:55.455847 pyeventengine-0.3.0.post1/PKG-INFO
+drwxrwxrwx   0 bolun     (1000) bolun     (1000)        0 2024-05-28 10:43:55.430847 pyeventengine-0.3.0.post1/PyEventEngine.egg-info/
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     2109 2024-05-28 10:43:54.000000 pyeventengine-0.3.0.post1/PyEventEngine.egg-info/PKG-INFO
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)      350 2024-05-28 10:43:54.000000 pyeventengine-0.3.0.post1/PyEventEngine.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)        1 2024-05-28 10:43:54.000000 pyeventengine-0.3.0.post1/PyEventEngine.egg-info/dependency_links.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       12 2024-05-28 10:43:54.000000 pyeventengine-0.3.0.post1/PyEventEngine.egg-info/top_level.txt
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1507 2024-05-28 06:20:25.000000 pyeventengine-0.3.0.post1/README.md
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)       79 2024-05-28 10:43:55.463847 pyeventengine-0.3.0.post1/setup.cfg
+-rwxrwxrwx   0 bolun     (1000) bolun     (1000)     1733 2024-05-28 10:24:33.000000 pyeventengine-0.3.0.post1/setup.py
```

### Comparing `pyeventengine-0.3.0/EventEngine/Core/__init__.py` & `pyeventengine-0.3.0.post1/EventEngine/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyeventengine-0.3.0/EventEngine/Core/_event.py` & `pyeventengine-0.3.0.post1/EventEngine/Core/_event.py`

 * *Files identical despite different names*

### Comparing `pyeventengine-0.3.0/EventEngine/Core/_topic.py` & `pyeventengine-0.3.0.post1/EventEngine/Core/_topic.py`

 * *Files identical despite different names*

### Comparing `pyeventengine-0.3.0/EventEngine/Core/_topic_c.py` & `pyeventengine-0.3.0.post1/EventEngine/Core/_topic_c.py`

 * *Files identical despite different names*

### Comparing `pyeventengine-0.3.0/EventEngine/cpp/topic_api.cpp` & `pyeventengine-0.3.0.post1/EventEngine/cpp/topic_api.cpp`

 * *Files identical despite different names*

### Comparing `pyeventengine-0.3.0/LICENSE` & `pyeventengine-0.3.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyeventengine-0.3.0/PKG-INFO` & `pyeventengine-0.3.0.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyEventEngine
-Version: 0.3.0
+Version: 0.3.0.post1
 Summary: Basic event engine
 Home-page: https://github.com/BolunHan/PyEventEngine.git
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyeventengine-0.3.0/PyEventEngine.egg-info/PKG-INFO` & `pyeventengine-0.3.0.post1/PyEventEngine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyEventEngine
-Version: 0.3.0
+Version: 0.3.0.post1
 Summary: Basic event engine
 Home-page: https://github.com/BolunHan/PyEventEngine.git
 Author: Bolun.Han
 Author-email: Bolun.Han@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyeventengine-0.3.0/README.md` & `pyeventengine-0.3.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `pyeventengine-0.3.0/setup.py` & `pyeventengine-0.3.0.post1/setup.py`

 * *Files identical despite different names*

