# Comparing `tmp/langchain_iris-0.1.3b2.tar.gz` & `tmp/langchain_iris-0.1.3b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_iris-0.1.3b2.tar", last modified: Wed May  8 10:53:37 2024, max compression
+gzip compressed data, was "langchain_iris-0.1.3b3.tar", last modified: Tue May 28 15:51:55 2024, max compression
```

## Comparing `langchain_iris-0.1.3b2.tar` & `langchain_iris-0.1.3b3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:53:37.745136 langchain_iris-0.1.3b2/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 10:53:12.000000 langchain_iris-0.1.3b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-08 10:53:37.745136 langchain_iris-0.1.3b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-08 10:53:12.000000 langchain_iris-0.1.3b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:53:37.745136 langchain_iris-0.1.3b2/langchain_iris/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-08 10:53:12.000000 langchain_iris-0.1.3b2/langchain_iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19886 2024-05-08 10:53:12.000000 langchain_iris-0.1.3b2/langchain_iris/vectorstores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:53:37.745136 langchain_iris-0.1.3b2/langchain_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-08 10:53:37.000000 langchain_iris-0.1.3b2/langchain_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-08 10:53:37.000000 langchain_iris-0.1.3b2/langchain_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:53:37.000000 langchain_iris-0.1.3b2/langchain_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-08 10:53:37.000000 langchain_iris-0.1.3b2/langchain_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 10:53:37.000000 langchain_iris-0.1.3b2/langchain_iris.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-08 10:53:37.745136 langchain_iris-0.1.3b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-08 10:53:12.000000 langchain_iris-0.1.3b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:53:37.745136 langchain_iris-0.1.3b2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10436 2024-05-08 10:53:12.000000 langchain_iris-0.1.3b2/tests/test_vectorstores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:51:55.255956 langchain_iris-0.1.3b3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-28 15:51:36.000000 langchain_iris-0.1.3b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-28 15:51:55.255956 langchain_iris-0.1.3b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-28 15:51:36.000000 langchain_iris-0.1.3b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:51:55.251956 langchain_iris-0.1.3b3/langchain_iris/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-28 15:51:36.000000 langchain_iris-0.1.3b3/langchain_iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19886 2024-05-28 15:51:36.000000 langchain_iris-0.1.3b3/langchain_iris/vectorstores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:51:55.255956 langchain_iris-0.1.3b3/langchain_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-28 15:51:55.000000 langchain_iris-0.1.3b3/langchain_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-28 15:51:55.000000 langchain_iris-0.1.3b3/langchain_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:51:55.000000 langchain_iris-0.1.3b3/langchain_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 15:51:55.000000 langchain_iris-0.1.3b3/langchain_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 15:51:55.000000 langchain_iris-0.1.3b3/langchain_iris.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-28 15:51:55.255956 langchain_iris-0.1.3b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-28 15:51:36.000000 langchain_iris-0.1.3b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:51:55.255956 langchain_iris-0.1.3b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-05-28 15:51:36.000000 langchain_iris-0.1.3b3/tests/test_vectorstores.py
```

### Comparing `langchain_iris-0.1.3b2/LICENSE` & `langchain_iris-0.1.3b3/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_iris-0.1.3b2/PKG-INFO` & `langchain_iris-0.1.3b3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-iris
-Version: 0.1.3b2
+Version: 0.1.3b3
 Summary: The InterSystems IRIS adoption for Langchain
 Home-page: https://github.com/caretdev/langchain-iris
 Project-URL: Source, https://github.com/caretdev/langchain-iris
 Project-URL: Tracker, https://github.com/caretdev/langchain-iris/issues
 Keywords: "InterSystems IRIS"
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,16 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: langchain>=0.0.348
-Requires-Dist: sqlalchemy-iris>=0.13.0
+Requires-Dist: langchain-community>=0.2.1
+Requires-Dist: sqlalchemy-iris>=0.14.0
 
 # Langchain with InterSystems IRIS
 
 [Langchain](https://github.com/langchain-ai/langchain) with support for InterSystems IRIS
 
 
 ## Install
```

### Comparing `langchain_iris-0.1.3b2/README.md` & `langchain_iris-0.1.3b3/README.md`

 * *Files identical despite different names*

### Comparing `langchain_iris-0.1.3b2/langchain_iris/vectorstores.py` & `langchain_iris-0.1.3b3/langchain_iris/vectorstores.py`

 * *Files identical despite different names*

### Comparing `langchain_iris-0.1.3b2/langchain_iris.egg-info/PKG-INFO` & `langchain_iris-0.1.3b3/langchain_iris.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-iris
-Version: 0.1.3b2
+Version: 0.1.3b3
 Summary: The InterSystems IRIS adoption for Langchain
 Home-page: https://github.com/caretdev/langchain-iris
 Project-URL: Source, https://github.com/caretdev/langchain-iris
 Project-URL: Tracker, https://github.com/caretdev/langchain-iris/issues
 Keywords: "InterSystems IRIS"
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,16 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: langchain>=0.0.348
-Requires-Dist: sqlalchemy-iris>=0.13.0
+Requires-Dist: langchain-community>=0.2.1
+Requires-Dist: sqlalchemy-iris>=0.14.0
 
 # Langchain with InterSystems IRIS
 
 [Langchain](https://github.com/langchain-ai/langchain) with support for InterSystems IRIS
 
 
 ## Install
```

### Comparing `langchain_iris-0.1.3b2/setup.cfg` & `langchain_iris-0.1.3b3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = langchain-iris
-version = 0.1.3b2
+version = 0.1.3b3
 description = The InterSystems IRIS adoption for Langchain
 long_description = file: README.md
 url = https://github.com/caretdev/langchain-iris
 long_description_content_type = text/markdown
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
```

### Comparing `langchain_iris-0.1.3b2/tests/test_vectorstores.py` & `langchain_iris-0.1.3b3/tests/test_vectorstores.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import pytest
 
 from langchain.docstore.document import Document
 from sqlalchemy.orm import Session
 
 from langchain_iris import IRISVector
-from langchain.embeddings.fake import DeterministicFakeEmbedding
+from langchain_community.embeddings import DeterministicFakeEmbedding
 
 
 class FakeEmbeddings(DeterministicFakeEmbedding):
     size = 200
 
 
 class FakeEmbeddingsWithAdaDimension(FakeEmbeddings):
```

