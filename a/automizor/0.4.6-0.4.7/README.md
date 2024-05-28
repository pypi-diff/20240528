# Comparing `tmp/automizor-0.4.6.tar.gz` & `tmp/automizor-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automizor-0.4.6.tar", last modified: Fri May 24 15:04:33 2024, max compression
+gzip compressed data, was "automizor-0.4.7.tar", last modified: Tue May 28 12:37:35 2024, max compression
```

## Comparing `automizor-0.4.6.tar` & `automizor-0.4.7.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:04:33.675586 automizor-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-24 15:04:25.000000 automizor-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-24 15:04:25.000000 automizor-0.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-24 15:04:33.675586 automizor-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-24 15:04:25.000000 automizor-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:04:33.671586 automizor-0.4.6/automizor/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-24 15:04:25.000000 automizor-0.4.6/automizor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:04:33.671586 automizor-0.4.6/automizor/datastore/
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-24 15:04:25.000000 automizor-0.4.6/automizor/datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-24 15:04:25.000000 automizor-0.4.6/automizor/datastore/_datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-24 15:04:25.000000 automizor-0.4.6/automizor/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:04:33.671586 automizor-0.4.6/automizor/job/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-24 15:04:25.000000 automizor-0.4.6/automizor/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-24 15:04:25.000000 automizor-0.4.6/automizor/job/_job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:04:33.671586 automizor-0.4.6/automizor/log/
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-24 15:04:25.000000 automizor-0.4.6/automizor/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-24 15:04:25.000000 automizor-0.4.6/automizor/log/_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:04:33.671586 automizor-0.4.6/automizor/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-24 15:04:25.000000 automizor-0.4.6/automizor/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-05-24 15:04:25.000000 automizor-0.4.6/automizor/storage/_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:04:33.671586 automizor-0.4.6/automizor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-24 15:04:25.000000 automizor-0.4.6/automizor/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:04:33.675586 automizor-0.4.6/automizor/vault/
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-24 15:04:25.000000 automizor-0.4.6/automizor/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-24 15:04:25.000000 automizor-0.4.6/automizor/vault/_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-24 15:04:25.000000 automizor-0.4.6/automizor/vault/_vault.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:04:33.675586 automizor-0.4.6/automizor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-24 15:04:33.000000 automizor-0.4.6/automizor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-24 15:04:33.000000 automizor-0.4.6/automizor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:04:33.000000 automizor-0.4.6/automizor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 15:04:33.000000 automizor-0.4.6/automizor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 15:04:33.000000 automizor-0.4.6/automizor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-24 15:04:33.675586 automizor-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-24 15:04:25.000000 automizor-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:37:35.387237 automizor-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-28 12:37:27.000000 automizor-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-28 12:37:27.000000 automizor-0.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-28 12:37:35.387237 automizor-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 12:37:27.000000 automizor-0.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:37:35.383237 automizor-0.4.7/automizor/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 12:37:27.000000 automizor-0.4.7/automizor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:37:35.383237 automizor-0.4.7/automizor/datastore/
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-28 12:37:27.000000 automizor-0.4.7/automizor/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-28 12:37:27.000000 automizor-0.4.7/automizor/datastore/_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-28 12:37:27.000000 automizor-0.4.7/automizor/datastore/_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-28 12:37:27.000000 automizor-0.4.7/automizor/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:37:35.383237 automizor-0.4.7/automizor/job/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-28 12:37:27.000000 automizor-0.4.7/automizor/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-28 12:37:27.000000 automizor-0.4.7/automizor/job/_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:37:35.387237 automizor-0.4.7/automizor/log/
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-28 12:37:27.000000 automizor-0.4.7/automizor/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-28 12:37:27.000000 automizor-0.4.7/automizor/log/_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:37:35.387237 automizor-0.4.7/automizor/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-28 12:37:27.000000 automizor-0.4.7/automizor/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-05-28 12:37:27.000000 automizor-0.4.7/automizor/storage/_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:37:35.387237 automizor-0.4.7/automizor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-28 12:37:27.000000 automizor-0.4.7/automizor/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:37:35.387237 automizor-0.4.7/automizor/vault/
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-28 12:37:27.000000 automizor-0.4.7/automizor/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-28 12:37:27.000000 automizor-0.4.7/automizor/vault/_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-28 12:37:27.000000 automizor-0.4.7/automizor/vault/_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:37:35.387237 automizor-0.4.7/automizor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-28 12:37:35.000000 automizor-0.4.7/automizor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-28 12:37:35.000000 automizor-0.4.7/automizor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:37:35.000000 automizor-0.4.7/automizor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 12:37:35.000000 automizor-0.4.7/automizor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 12:37:35.000000 automizor-0.4.7/automizor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-28 12:37:35.387237 automizor-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-28 12:37:27.000000 automizor-0.4.7/setup.py
```

### Comparing `automizor-0.4.6/LICENSE` & `automizor-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `automizor-0.4.6/PKG-INFO` & `automizor-0.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automizor
-Version: 0.4.6
+Version: 0.4.7
 Summary: Python Automizor framework
 Home-page: https://github.com/automizor/automizor-python
 Author: Christian Fischer
 Author-email: christian@automizor.io
 License: Apache License
 Keywords: automizor framework
 Classifier: Intended Audience :: Developers
```

### Comparing `automizor-0.4.6/automizor/datastore/_datastore.py` & `automizor-0.4.7/automizor/datastore/_datastore.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 from automizor.utils import get_api_config, get_headers
 
 JSON = Union[str, int, float, bool, None, Dict[str, "JSON"], List["JSON"]]
 
 
 class DataStore:
     """
-    `DataStore` is a class designed to interface with the `Automizor Platform` to manage and
-    manipulate data stored in various formats. It supports operations to retrieve and update
-    data using a unified API.
-
-    The class initializes an HTTP session with the necessary headers for authentication, and
-    provides methods to retrieve values, and set values in the store.
+    `DataStore` is a class designed to interface with the `Automizor Platform`
+    to manage and manipulate data stored in various formats. It supports
+    operations to retrieve and update data using a unified API.
+
+    The class initializes an HTTP session with the necessary headers for
+    authentication, and provides methods to retrieve values, and set values in
+    the store.
 
     Attributes:
         url (str): The base URL for the API endpoint.
         token (str): The authentication token for API access.
-        session (requests.Session): The HTTP session used for making API requests.
+        session (requests.Session): The HTTP session used to make API requests.
     """
 
     def __init__(self):
         self.url, self.token = get_api_config()
         self.session = requests.Session()
         self.session.headers.update(get_headers(self.token))
 
@@ -35,16 +36,16 @@
         secondary_key: str | None = None,
     ) -> JSON:
         """
         Retrieves values from the specified data store.
 
         Parameters:
             name (str): The name of the data store.
-            primary_key (str, optional): The primary key for the values. Defaults to None.
-            secondary_key (str, optional): The secondary key for the values. Defaults to None.
+            primary_key (str, optional): The primary key for the values.
+            secondary_key (str, optional): The secondary key for the values.
 
         Returns:
             JSON: The values from the data store.
         """
 
         return self._get_values(name, primary_key, secondary_key)
 
@@ -60,15 +61,15 @@
         return self._set_values(name, values)
 
     def _get_values(
         self,
         name: str,
         primary_key: str | None = None,
         secondary_key: str | None = None,
-    ) -> dict:
+    ) -> JSON:
         params = (
             {"primary_key": primary_key, "secondary_key": secondary_key}
             if primary_key or secondary_key
             else {}
         )
         url = f"https://{self.url}/api/v1/workflow/datastore/{name}/values/"
         try:
```

### Comparing `automizor-0.4.6/automizor/exceptions.py` & `automizor-0.4.7/automizor/exceptions.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.6/automizor/job/__init__.py` & `automizor-0.4.7/automizor/job/__init__.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.6/automizor/job/_job.py` & `automizor-0.4.7/automizor/job/_job.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.6/automizor/log/__init__.py` & `automizor-0.4.7/automizor/log/__init__.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.6/automizor/log/_log.py` & `automizor-0.4.7/automizor/log/_log.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.6/automizor/storage/__init__.py` & `automizor-0.4.7/automizor/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.6/automizor/storage/_storage.py` & `automizor-0.4.7/automizor/storage/_storage.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.6/automizor/utils/__init__.py` & `automizor-0.4.7/automizor/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.6/automizor/vault/__init__.py` & `automizor-0.4.7/automizor/vault/__init__.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.6/automizor/vault/_container.py` & `automizor-0.4.7/automizor/vault/_container.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.6/automizor/vault/_vault.py` & `automizor-0.4.7/automizor/vault/_vault.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.6/automizor.egg-info/PKG-INFO` & `automizor-0.4.7/automizor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automizor
-Version: 0.4.6
+Version: 0.4.7
 Summary: Python Automizor framework
 Home-page: https://github.com/automizor/automizor-python
 Author: Christian Fischer
 Author-email: christian@automizor.io
 License: Apache License
 Keywords: automizor framework
 Classifier: Intended Audience :: Developers
```

### Comparing `automizor-0.4.6/automizor.egg-info/SOURCES.txt` & `automizor-0.4.7/automizor.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 automizor/exceptions.py
 automizor.egg-info/PKG-INFO
 automizor.egg-info/SOURCES.txt
 automizor.egg-info/dependency_links.txt
 automizor.egg-info/requires.txt
 automizor.egg-info/top_level.txt
 automizor/datastore/__init__.py
+automizor/datastore/_container.py
 automizor/datastore/_datastore.py
 automizor/job/__init__.py
 automizor/job/_job.py
 automizor/log/__init__.py
 automizor/log/_log.py
 automizor/storage/__init__.py
 automizor/storage/_storage.py
```

### Comparing `automizor-0.4.6/setup.py` & `automizor-0.4.7/setup.py`

 * *Files identical despite different names*

