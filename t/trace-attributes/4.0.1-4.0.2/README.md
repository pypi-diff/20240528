# Comparing `tmp/trace_attributes-4.0.1.tar.gz` & `tmp/trace_attributes-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trace_attributes-4.0.1.tar", last modified: Thu May 23 22:53:33 2024, max compression
+gzip compressed data, was "trace_attributes-4.0.2.tar", last modified: Tue May 28 11:00:00 2024, max compression
```

## Comparing `trace_attributes-4.0.1.tar` & `trace_attributes-4.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:53:33.307789 trace_attributes-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 22:53:22.000000 trace_attributes-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-23 22:53:33.307789 trace_attributes-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    47682 2024-05-23 22:53:22.000000 trace_attributes-4.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 22:53:33.307789 trace_attributes-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-23 22:53:22.000000 trace_attributes-4.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:53:33.303789 trace_attributes-4.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:53:33.303789 trace_attributes-4.0.1/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:53:33.307789 trace_attributes-4.0.1/src/python/langtrace/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-23 22:53:22.000000 trace_attributes-4.0.1/src/python/langtrace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:53:33.307789 trace_attributes-4.0.1/src/python/langtrace/trace_attributes/
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-23 22:53:22.000000 trace_attributes-4.0.1/src/python/langtrace/trace_attributes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:53:33.307789 trace_attributes-4.0.1/src/python/langtrace/trace_attributes/models/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-23 22:53:22.000000 trace_attributes-4.0.1/src/python/langtrace/trace_attributes/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-23 22:53:22.000000 trace_attributes-4.0.1/src/python/langtrace/trace_attributes/models/database_span_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-23 22:53:22.000000 trace_attributes-4.0.1/src/python/langtrace/trace_attributes/models/framework_span_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-23 22:53:22.000000 trace_attributes-4.0.1/src/python/langtrace/trace_attributes/models/llm_span_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:53:33.307789 trace_attributes-4.0.1/src/python/trace_attributes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-23 22:53:33.000000 trace_attributes-4.0.1/src/python/trace_attributes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-23 22:53:33.000000 trace_attributes-4.0.1/src/python/trace_attributes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:53:33.000000 trace_attributes-4.0.1/src/python/trace_attributes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 22:53:33.000000 trace_attributes-4.0.1/src/python/trace_attributes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 22:53:33.000000 trace_attributes-4.0.1/src/python/trace_attributes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:00:00.226292 trace_attributes-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 10:59:47.000000 trace_attributes-4.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-28 11:00:00.226292 trace_attributes-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    47682 2024-05-28 10:59:47.000000 trace_attributes-4.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 11:00:00.226292 trace_attributes-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-28 10:59:47.000000 trace_attributes-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:00:00.222292 trace_attributes-4.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:00:00.222292 trace_attributes-4.0.2/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:00:00.226292 trace_attributes-4.0.2/src/python/langtrace/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 10:59:47.000000 trace_attributes-4.0.2/src/python/langtrace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:00:00.226292 trace_attributes-4.0.2/src/python/langtrace/trace_attributes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-28 10:59:47.000000 trace_attributes-4.0.2/src/python/langtrace/trace_attributes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:00:00.226292 trace_attributes-4.0.2/src/python/langtrace/trace_attributes/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 10:59:47.000000 trace_attributes-4.0.2/src/python/langtrace/trace_attributes/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-28 10:59:47.000000 trace_attributes-4.0.2/src/python/langtrace/trace_attributes/models/database_span_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-28 10:59:47.000000 trace_attributes-4.0.2/src/python/langtrace/trace_attributes/models/framework_span_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-28 10:59:47.000000 trace_attributes-4.0.2/src/python/langtrace/trace_attributes/models/llm_span_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:00:00.226292 trace_attributes-4.0.2/src/python/trace_attributes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-28 11:00:00.000000 trace_attributes-4.0.2/src/python/trace_attributes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-28 11:00:00.000000 trace_attributes-4.0.2/src/python/trace_attributes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 11:00:00.000000 trace_attributes-4.0.2/src/python/trace_attributes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 11:00:00.000000 trace_attributes-4.0.2/src/python/trace_attributes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 11:00:00.000000 trace_attributes-4.0.2/src/python/trace_attributes.egg-info/top_level.txt
```

### Comparing `trace_attributes-4.0.1/LICENSE` & `trace_attributes-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trace_attributes-4.0.1/PKG-INFO` & `trace_attributes-4.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trace-attributes
-Version: 4.0.1
+Version: 4.0.2
 Summary: LangTrace - Trace Attributes
 Home-page: https://github.com/Scale3-Labs/langtrace-trace-attributes
 Author: Karthik Kalyanaraman
 Author-email: karthik@scale3labs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trace_attributes-4.0.1/README.md` & `trace_attributes-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `trace_attributes-4.0.1/setup.py` & `trace_attributes-4.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='trace-attributes',  # Choose a unique name for PyPI
-    version='4.0.1',
+    version='4.0.2',
     author='Karthik Kalyanaraman',
     author_email='karthik@scale3labs.com',
     description='LangTrace - Trace Attributes',
     long_description="LangTrace - Trace Attributes",
     long_description_content_type='text/markdown',
     url='https://github.com/Scale3-Labs/langtrace-trace-attributes',  # Project home page
     package_dir={'': 'src/python'},
```

### Comparing `trace_attributes-4.0.1/src/python/langtrace/trace_attributes/__init__.py` & `trace_attributes-4.0.2/src/python/langtrace/trace_attributes/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -53,10 +53,23 @@
 
 class PineconeMethods(Enum):
     UPSERT = "pinecone.index.upsert"
     QUERY = "pinecone.index.query"
     DELETE = "pinecone.index.delete"
 
 
+class WeaviateMethods(Enum):
+    QUERY_BM25 = "weaviate.collections.queries.bm25"
+    QUERY_FETCH_OBJECT_BY_ID = "weaviate.collections.queries.fetch_object_by_id"
+    QUERY_FETCH_OBJECTS = "weaviate.collections.queries.fetch_objects"
+    QUERY_HYBRID = "weaviate.collections.queries.hybrid"
+    QUERY_NEAR_IMAGE = "weaviate.collections.queries.near_image"
+    QUERY_NEAR_MEDIA = "weaviate.collections.queries.near_media"
+    QUERY_NEAR_OBJECT = "weaviate.collections.queries.near_object"
+    QUERY_NEAR_TEXT = "weaviate.collections.queries.near_text"
+    QUERY_NEAR_VECTOR = "weaviate.collections.queries.near_vector"
+    COLLECTIONS_OPERATIONS = "weaviate.collections.collections"
+
+
 # Export only what you want to be accessible directly through `import my_package`
 __all__ = ['LLMSpanAttributes', 'DatabaseSpanAttributes', 'FrameworkSpanAttributes', 'Event',
-           'OpenAIMethods', 'ChromaDBMethods', 'PineconeMethods']
+           'OpenAIMethods', 'ChromaDBMethods', 'PineconeMethods', 'WeaviateMethods']
```

### Comparing `trace_attributes-4.0.1/src/python/langtrace/trace_attributes/models/database_span_attributes.py` & `trace_attributes-4.0.2/src/python/langtrace/trace_attributes/models/database_span_attributes.py`

 * *Files identical despite different names*

### Comparing `trace_attributes-4.0.1/src/python/langtrace/trace_attributes/models/framework_span_attributes.py` & `trace_attributes-4.0.2/src/python/langtrace/trace_attributes/models/framework_span_attributes.py`

 * *Files identical despite different names*

### Comparing `trace_attributes-4.0.1/src/python/langtrace/trace_attributes/models/llm_span_attributes.py` & `trace_attributes-4.0.2/src/python/langtrace/trace_attributes/models/llm_span_attributes.py`

 * *Files identical despite different names*

### Comparing `trace_attributes-4.0.1/src/python/trace_attributes.egg-info/PKG-INFO` & `trace_attributes-4.0.2/src/python/trace_attributes.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trace-attributes
-Version: 4.0.1
+Version: 4.0.2
 Summary: LangTrace - Trace Attributes
 Home-page: https://github.com/Scale3-Labs/langtrace-trace-attributes
 Author: Karthik Kalyanaraman
 Author-email: karthik@scale3labs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trace_attributes-4.0.1/src/python/trace_attributes.egg-info/SOURCES.txt` & `trace_attributes-4.0.2/src/python/trace_attributes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

