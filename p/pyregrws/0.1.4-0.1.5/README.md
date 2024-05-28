# Comparing `tmp/pyregrws-0.1.4.tar.gz` & `tmp/pyregrws-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyregrws-0.1.4.tar", max compression
+gzip compressed data, was "pyregrws-0.1.5.tar", max compression
```

## Comparing `pyregrws-0.1.4.tar` & `pyregrws-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0    11357 2023-01-05 16:07:04.424195 pyregrws-0.1.4/LICENSE
--rw-r--r--   0        0        0     1257 2023-02-20 14:27:14.489390 pyregrws-0.1.4/README.md
--rw-r--r--   0        0        0     1950 2023-03-07 17:06:41.142336 pyregrws-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      184 2023-02-14 16:19:41.987736 pyregrws-0.1.4/regrws/__init__.py
--rw-r--r--   0        0        0      151 2023-02-14 16:19:42.007736 pyregrws-0.1.4/regrws/api/__init__.py
--rw-r--r--   0        0        0       80 2023-02-07 20:49:31.103174 pyregrws-0.1.4/regrws/api/constants.py
--rw-r--r--   0        0        0     3320 2023-02-15 20:11:59.517176 pyregrws-0.1.4/regrws/api/core.py
--rw-r--r--   0        0        0     2903 2023-03-07 17:06:01.484675 pyregrws-0.1.4/regrws/api/manager.py
--rw-r--r--   0        0        0      352 2023-02-27 22:40:18.273841 pyregrws-0.1.4/regrws/arin_xml_encoder.py
--rw-r--r--   0        0        0      274 2023-02-15 20:11:59.517176 pyregrws-0.1.4/regrws/models/__init__.py
--rw-r--r--   0        0        0     2025 2023-02-15 15:55:47.590675 pyregrws-0.1.4/regrws/models/base.py
--rw-r--r--   0        0        0     2116 2023-02-15 20:11:59.517176 pyregrws-0.1.4/regrws/models/customer.py
--rw-r--r--   0        0        0     1017 2023-02-15 20:11:59.517176 pyregrws-0.1.4/regrws/models/error.py
--rw-r--r--   0        0        0     1322 2023-02-15 20:11:59.517176 pyregrws-0.1.4/regrws/models/nested.py
--rw-r--r--   0        0        0     7588 2023-02-27 22:40:18.273841 pyregrws-0.1.4/regrws/models/net.py
--rw-r--r--   0        0        0     1503 2023-02-15 20:11:59.517176 pyregrws-0.1.4/regrws/models/org.py
--rw-r--r--   0        0        0     2237 2023-02-15 20:11:59.517176 pyregrws-0.1.4/regrws/models/poc.py
--rw-r--r--   0        0        0     2823 2023-03-01 21:20:23.574010 pyregrws-0.1.4/regrws/models/tickets.py
--rw-r--r--   0        0        0     1392 2023-02-15 20:11:59.517176 pyregrws-0.1.4/regrws/models/types.py
--rw-r--r--   0        0        0      181 2023-02-07 20:49:50.753501 pyregrws-0.1.4/regrws/settings.py
--rw-r--r--   0        0        0     2111 1970-01-01 00:00:00.000000 pyregrws-0.1.4/setup.py
--rw-r--r--   0        0        0     2402 1970-01-01 00:00:00.000000 pyregrws-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-01-05 16:07:04.000000 pyregrws-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1257 2023-02-20 14:27:14.000000 pyregrws-0.1.5/README.md
+-rw-r--r--   0        0        0     1974 2024-05-28 03:18:39.368902 pyregrws-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      184 2023-02-14 16:19:41.000000 pyregrws-0.1.5/regrws/__init__.py
+-rw-r--r--   0        0        0      151 2023-02-14 16:19:42.000000 pyregrws-0.1.5/regrws/api/__init__.py
+-rw-r--r--   0        0        0       80 2023-02-07 20:49:31.000000 pyregrws-0.1.5/regrws/api/constants.py
+-rw-r--r--   0        0        0     3320 2023-02-15 20:11:59.000000 pyregrws-0.1.5/regrws/api/core.py
+-rw-r--r--   0        0        0     2903 2024-05-28 03:18:39.368902 pyregrws-0.1.5/regrws/api/manager.py
+-rw-r--r--   0        0        0      352 2024-05-28 03:18:39.368902 pyregrws-0.1.5/regrws/arin_xml_encoder.py
+-rw-r--r--   0        0        0      274 2023-02-15 20:11:59.000000 pyregrws-0.1.5/regrws/models/__init__.py
+-rw-r--r--   0        0        0     2025 2023-02-15 15:55:47.000000 pyregrws-0.1.5/regrws/models/base.py
+-rw-r--r--   0        0        0     2116 2023-02-15 20:11:59.000000 pyregrws-0.1.5/regrws/models/customer.py
+-rw-r--r--   0        0        0     1017 2023-02-15 20:11:59.000000 pyregrws-0.1.5/regrws/models/error.py
+-rw-r--r--   0        0        0     1334 2024-05-28 03:18:39.368902 pyregrws-0.1.5/regrws/models/nested.py
+-rw-r--r--   0        0        0     7588 2024-05-28 03:18:39.368902 pyregrws-0.1.5/regrws/models/net.py
+-rw-r--r--   0        0        0     1503 2023-02-15 20:11:59.000000 pyregrws-0.1.5/regrws/models/org.py
+-rw-r--r--   0        0        0     2237 2023-02-15 20:11:59.000000 pyregrws-0.1.5/regrws/models/poc.py
+-rw-r--r--   0        0        0     2823 2024-05-28 03:18:39.368902 pyregrws-0.1.5/regrws/models/tickets.py
+-rw-r--r--   0        0        0     1392 2023-02-15 20:11:59.000000 pyregrws-0.1.5/regrws/models/types.py
+-rw-r--r--   0        0        0      181 2023-02-07 20:49:50.000000 pyregrws-0.1.5/regrws/settings.py
+-rw-r--r--   0        0        0     2388 1970-01-01 00:00:00.000000 pyregrws-0.1.5/PKG-INFO
```

### Comparing `pyregrws-0.1.4/LICENSE` & `pyregrws-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyregrws-0.1.4/README.md` & `pyregrws-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pyregrws-0.1.4/pyproject.toml` & `pyregrws-0.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyregrws"
-version = "0.1.4"
+version = "0.1.5"
 description = "Python library to retrieve and modify records within ARIN's database through their Reg-RWS service"
 authors = ["Jonathan Senecal <contact@jonathansenecal.com>"]
 homepage = "https://github.com/jsenecal/pyregrws"
 license = "Apache 2.0"
 readme = "README.md"
 classifiers = [
   "Development Status :: 3 - Alpha",
@@ -21,14 +21,15 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.28.1"
 pydantic = { extras = ["dotenv"], version = "^1.10.4" }
 pydantic-xml = { extras = ["lxml"], version = "^0.5.0" }
+certifi = ">=2023.7.22"
 
 [tool.poetry.group.dev.dependencies]
 pytest-xdist = "^3.1.0"
 black = { version = "^23.1.0", allow-prereleases = true }
 ipython = "^8.10.0"
 pytest = "^7.2.0"
 xmldiff = "^2.4"
```

### Comparing `pyregrws-0.1.4/regrws/api/core.py` & `pyregrws-0.1.5/regrws/api/core.py`

 * *Files identical despite different names*

### Comparing `pyregrws-0.1.4/regrws/api/manager.py` & `pyregrws-0.1.5/regrws/api/manager.py`

 * *Files identical despite different names*

### Comparing `pyregrws-0.1.4/regrws/models/base.py` & `pyregrws-0.1.5/regrws/models/base.py`

 * *Files identical despite different names*

### Comparing `pyregrws-0.1.4/regrws/models/customer.py` & `pyregrws-0.1.5/regrws/models/customer.py`

 * *Files identical despite different names*

### Comparing `pyregrws-0.1.4/regrws/models/error.py` & `pyregrws-0.1.5/regrws/models/error.py`

 * *Files identical despite different names*

### Comparing `pyregrws-0.1.4/regrws/models/nested.py` & `pyregrws-0.1.5/regrws/models/nested.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     code2: code2_type = element()
     code3: code3_type = element()
     e164: int = element()
 
 
 class MultiLineElement(BaseModel):
     number: int = attr()
-    line: str
+    line: str | None = ''
 
 
 class Attachment(BaseModel, tag="attachment", nsmap=NSMAP):
     data: str = element()
     filename: str = element()
```

### Comparing `pyregrws-0.1.4/regrws/models/net.py` & `pyregrws-0.1.5/regrws/models/net.py`

 * *Files identical despite different names*

### Comparing `pyregrws-0.1.4/regrws/models/org.py` & `pyregrws-0.1.5/regrws/models/org.py`

 * *Files identical despite different names*

### Comparing `pyregrws-0.1.4/regrws/models/poc.py` & `pyregrws-0.1.5/regrws/models/poc.py`

 * *Files identical despite different names*

### Comparing `pyregrws-0.1.4/regrws/models/tickets.py` & `pyregrws-0.1.5/regrws/models/tickets.py`

 * *Files identical despite different names*

### Comparing `pyregrws-0.1.4/regrws/models/types.py` & `pyregrws-0.1.5/regrws/models/types.py`

 * *Files identical despite different names*

### Comparing `pyregrws-0.1.4/PKG-INFO` & `pyregrws-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyregrws
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python library to retrieve and modify records within ARIN's database through their Reg-RWS service
 Home-page: https://github.com/jsenecal/pyregrws
 License: Apache 2.0
 Author: Jonathan Senecal
 Author-email: contact@jonathansenecal.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -12,18 +12,18 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: certifi (>=2023.7.22)
 Requires-Dist: pydantic-xml[lxml] (>=0.5.0,<0.6.0)
 Requires-Dist: pydantic[dotenv] (>=1.10.4,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # pyregrws
```

