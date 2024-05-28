# Comparing `tmp/evtx2es-1.6.0.tar.gz` & `tmp/evtx2es-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evtx2es-1.6.0.tar", max compression
+gzip compressed data, was "evtx2es-1.6.1.tar", max compression
```

## Comparing `evtx2es-1.6.0.tar` & `evtx2es-1.6.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1065 2023-11-26 03:09:49.441118 evtx2es-1.6.0/LICENSE
--rw-r--r--   0        0        0     6557 2023-11-26 03:09:49.441118 evtx2es-1.6.0/README.md
--rw-r--r--   0        0        0      842 2023-11-26 03:09:49.441118 evtx2es-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     2673 2023-11-26 03:09:49.441118 evtx2es-1.6.0/src/evtx2es/__init__.py
--rw-r--r--   0        0        0     1520 2023-11-26 03:09:49.441118 evtx2es-1.6.0/src/evtx2es/models/ElasticsearchUtils.py
--rw-r--r--   0        0        0     7603 2023-11-26 03:09:49.441118 evtx2es-1.6.0/src/evtx2es/models/Evtx2es.py
--rw-r--r--   0        0        0      203 2023-11-26 03:09:49.441118 evtx2es-1.6.0/src/evtx2es/models/MetaData.py
--rw-r--r--   0        0        0     1784 2023-11-26 03:09:49.441118 evtx2es-1.6.0/src/evtx2es/presenters/Evtx2esPresenter.py
--rw-r--r--   0        0        0     1373 2023-11-26 03:09:49.441118 evtx2es-1.6.0/src/evtx2es/presenters/Evtx2jsonPresenter.py
--rw-r--r--   0        0        0      938 2023-11-26 03:09:49.441118 evtx2es-1.6.0/src/evtx2es/views/BaseView.py
--rw-r--r--   0        0        0     3169 2023-11-26 03:09:49.441118 evtx2es-1.6.0/src/evtx2es/views/Evtx2esView.py
--rw-r--r--   0        0        0     1672 2023-11-26 03:09:49.441118 evtx2es-1.6.0/src/evtx2es/views/Evtx2jsonView.py
--rw-r--r--   0        0        0     7357 1970-01-01 00:00:00.000000 evtx2es-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-28 20:07:31.216270 evtx2es-1.6.1/LICENSE
+-rw-r--r--   0        0        0     6557 2024-05-28 20:07:31.216270 evtx2es-1.6.1/README.md
+-rw-r--r--   0        0        0      842 2024-05-28 20:07:31.216270 evtx2es-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2673 2024-05-28 20:07:31.220270 evtx2es-1.6.1/src/evtx2es/__init__.py
+-rw-r--r--   0        0        0     1520 2024-05-28 20:07:31.220270 evtx2es-1.6.1/src/evtx2es/models/ElasticsearchUtils.py
+-rw-r--r--   0        0        0     7384 2024-05-28 20:07:31.220270 evtx2es-1.6.1/src/evtx2es/models/Evtx2es.py
+-rw-r--r--   0        0        0      203 2024-05-28 20:07:31.220270 evtx2es-1.6.1/src/evtx2es/models/MetaData.py
+-rw-r--r--   0        0        0     1784 2024-05-28 20:07:31.220270 evtx2es-1.6.1/src/evtx2es/presenters/Evtx2esPresenter.py
+-rw-r--r--   0        0        0     1373 2024-05-28 20:07:31.220270 evtx2es-1.6.1/src/evtx2es/presenters/Evtx2jsonPresenter.py
+-rw-r--r--   0        0        0      938 2024-05-28 20:07:31.220270 evtx2es-1.6.1/src/evtx2es/views/BaseView.py
+-rw-r--r--   0        0        0     3169 2024-05-28 20:07:31.220270 evtx2es-1.6.1/src/evtx2es/views/Evtx2esView.py
+-rw-r--r--   0        0        0     1672 2024-05-28 20:07:31.220270 evtx2es-1.6.1/src/evtx2es/views/Evtx2jsonView.py
+-rw-r--r--   0        0        0     7357 1970-01-01 00:00:00.000000 evtx2es-1.6.1/PKG-INFO
```

### Comparing `evtx2es-1.6.0/LICENSE` & `evtx2es-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `evtx2es-1.6.0/README.md` & `evtx2es-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `evtx2es-1.6.0/pyproject.toml` & `evtx2es-1.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "evtx2es"
-version = "1.6.0"
+version = "1.6.1"
 description = "Fast import of Windows EventLogs(.evtx) into Elasticsearch."
 authors = ["sumeshi <sum3sh1@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 repository = "https://github.com/sumeshi/evtx2es"
 homepage = "https://github.com/sumeshi/evtx2es"
```

### Comparing `evtx2es-1.6.0/src/evtx2es/__init__.py` & `evtx2es-1.6.1/src/evtx2es/__init__.py`

 * *Files identical despite different names*

### Comparing `evtx2es-1.6.0/src/evtx2es/models/ElasticsearchUtils.py` & `evtx2es-1.6.1/src/evtx2es/models/ElasticsearchUtils.py`

 * *Files identical despite different names*

### Comparing `evtx2es-1.6.0/src/evtx2es/models/Evtx2es.py` & `evtx2es-1.6.1/src/evtx2es/models/Evtx2es.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,21 +79,17 @@
     except KeyError:
         pass
 
     except TypeError:
         pass
 
     try:
-        record["userdata"] = {
-            "address": record["data"]["Event"]["UserData"]["EventXML"]["Address"],
-            "sessionid": record["data"]["Event"]["UserData"]["EventXML"][
-                "SessionID"
-            ],
-            "user": record["data"]["Event"]["UserData"]["EventXML"]["User"],
-        }
+        record["userdata"] = record["data"]["Event"].get(
+            "UserData", dict()
+        )
     except KeyError:
         pass
 
     except TypeError:
         pass
 
     record.update(
```

### Comparing `evtx2es-1.6.0/src/evtx2es/presenters/Evtx2esPresenter.py` & `evtx2es-1.6.1/src/evtx2es/presenters/Evtx2esPresenter.py`

 * *Files identical despite different names*

### Comparing `evtx2es-1.6.0/src/evtx2es/presenters/Evtx2jsonPresenter.py` & `evtx2es-1.6.1/src/evtx2es/presenters/Evtx2jsonPresenter.py`

 * *Files identical despite different names*

### Comparing `evtx2es-1.6.0/src/evtx2es/views/BaseView.py` & `evtx2es-1.6.1/src/evtx2es/views/BaseView.py`

 * *Files identical despite different names*

### Comparing `evtx2es-1.6.0/src/evtx2es/views/Evtx2esView.py` & `evtx2es-1.6.1/src/evtx2es/views/Evtx2esView.py`

 * *Files identical despite different names*

### Comparing `evtx2es-1.6.0/src/evtx2es/views/Evtx2jsonView.py` & `evtx2es-1.6.1/src/evtx2es/views/Evtx2jsonView.py`

 * *Files identical despite different names*

### Comparing `evtx2es-1.6.0/PKG-INFO` & `evtx2es-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evtx2es
-Version: 1.6.0
+Version: 1.6.1
 Summary: Fast import of Windows EventLogs(.evtx) into Elasticsearch.
 Home-page: https://github.com/sumeshi/evtx2es
 License: MIT
 Keywords: evtx,elasticsearch,json
 Author: sumeshi
 Author-email: sum3sh1@protonmail.com
 Requires-Python: >=3.11,<4.0
```

