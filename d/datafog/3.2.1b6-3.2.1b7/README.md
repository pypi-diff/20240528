# Comparing `tmp/datafog-3.2.1b6.tar.gz` & `tmp/datafog-3.2.1b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-3.2.1b6.tar", last modified: Mon May 27 22:19:21 2024, max compression
+gzip compressed data, was "datafog-3.2.1b7.tar", last modified: Mon May 27 22:30:35 2024, max compression
```

## Comparing `datafog-3.2.1b6.tar` & `datafog-3.2.1b7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:19:21.451693 datafog-3.2.1b6/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-18 18:25:55.000000 datafog-3.2.1b6/LICENSE
--rw-r--r--   0 sidmohan   (501) staff       (20)     8252 2024-05-27 22:19:21.451339 datafog-3.2.1b6/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)     6738 2024-05-18 21:12:05.000000 datafog-3.2.1b6/README.md
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:19:21.445280 datafog-3.2.1b6/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-18 21:02:49.000000 datafog-3.2.1b6/datafog/__about__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      907 2024-05-18 21:08:14.000000 datafog-3.2.1b6/datafog/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      190 2024-05-18 19:53:32.000000 datafog-3.2.1b6/datafog/config.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     3692 2024-05-27 22:17:09.000000 datafog-3.2.1b6/datafog/main.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:19:21.446260 datafog-3.2.1b6/datafog/processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)      400 2024-05-18 21:08:14.000000 datafog-3.2.1b6/datafog/processing/__init__.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:19:21.447323 datafog-3.2.1b6/datafog/processing/image_processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)      146 2024-05-18 18:25:55.000000 datafog-3.2.1b6/datafog/processing/image_processing/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2872 2024-05-18 18:25:55.000000 datafog-3.2.1b6/datafog/processing/image_processing/donut_processor.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      787 2024-05-18 18:25:55.000000 datafog-3.2.1b6/datafog/processing/image_processing/image_downloader.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      297 2024-05-18 18:25:55.000000 datafog-3.2.1b6/datafog/processing/image_processing/pytesseract_processor.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:19:21.448530 datafog-3.2.1b6/datafog/processing/spark_processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)      225 2024-05-18 19:53:34.000000 datafog-3.2.1b6/datafog/processing/spark_processing/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2204 2024-05-18 21:08:15.000000 datafog-3.2.1b6/datafog/processing/spark_processing/pyspark_udfs.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:19:21.448979 datafog-3.2.1b6/datafog/processing/text_processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)       51 2024-05-18 18:25:55.000000 datafog-3.2.1b6/datafog/processing/text_processing/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1300 2024-05-18 18:25:55.000000 datafog-3.2.1b6/datafog/processing/text_processing/spacy_pii_annotator.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:19:21.450055 datafog-3.2.1b6/datafog/services/
--rw-r--r--   0 sidmohan   (501) staff       (20)      118 2024-05-18 18:25:55.000000 datafog-3.2.1b6/datafog/services/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1802 2024-05-18 21:08:15.000000 datafog-3.2.1b6/datafog/services/image_service.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1030 2024-05-18 19:53:34.000000 datafog-3.2.1b6/datafog/services/spark_service.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      633 2024-05-18 21:08:14.000000 datafog-3.2.1b6/datafog/services/text_service.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:19:21.450469 datafog-3.2.1b6/datafog/telemetry/
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-18 20:37:26.000000 datafog-3.2.1b6/datafog/telemetry/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     3554 2024-05-27 22:18:45.000000 datafog-3.2.1b6/datafog/telemetry/open_telemetry.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:19:21.451052 datafog-3.2.1b6/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     8252 2024-05-27 22:19:21.000000 datafog-3.2.1b6/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      972 2024-05-27 22:19:21.000000 datafog-3.2.1b6/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-27 22:19:21.000000 datafog-3.2.1b6/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)      145 2024-05-27 22:19:21.000000 datafog-3.2.1b6/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       14 2024-05-27 22:19:21.000000 datafog-3.2.1b6/datafog.egg-info/top_level.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-27 22:19:21.451740 datafog-3.2.1b6/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)     1945 2024-05-27 22:19:14.000000 datafog-3.2.1b6/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:19:21.450850 datafog-3.2.1b6/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)        0 2024-05-18 18:25:55.000000 datafog-3.2.1b6/tests/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2543 2024-05-27 22:18:14.000000 datafog-3.2.1b6/tests/test_image_service.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2785 2024-05-18 19:55:12.000000 datafog-3.2.1b6/tests/test_main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:30:35.562404 datafog-3.2.1b7/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-18 18:25:55.000000 datafog-3.2.1b7/LICENSE
+-rw-r--r--   0 sidmohan   (501) staff       (20)     8252 2024-05-27 22:30:35.561817 datafog-3.2.1b7/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6738 2024-05-18 21:12:05.000000 datafog-3.2.1b7/README.md
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:30:35.555103 datafog-3.2.1b7/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-18 21:02:49.000000 datafog-3.2.1b7/datafog/__about__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      907 2024-05-18 21:08:14.000000 datafog-3.2.1b7/datafog/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      190 2024-05-18 19:53:32.000000 datafog-3.2.1b7/datafog/config.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     7543 2024-05-27 22:30:10.000000 datafog-3.2.1b7/datafog/main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:30:35.556084 datafog-3.2.1b7/datafog/processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      400 2024-05-18 21:08:14.000000 datafog-3.2.1b7/datafog/processing/__init__.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:30:35.557096 datafog-3.2.1b7/datafog/processing/image_processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      146 2024-05-18 18:25:55.000000 datafog-3.2.1b7/datafog/processing/image_processing/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2872 2024-05-18 18:25:55.000000 datafog-3.2.1b7/datafog/processing/image_processing/donut_processor.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      787 2024-05-18 18:25:55.000000 datafog-3.2.1b7/datafog/processing/image_processing/image_downloader.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      297 2024-05-18 18:25:55.000000 datafog-3.2.1b7/datafog/processing/image_processing/pytesseract_processor.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:30:35.558324 datafog-3.2.1b7/datafog/processing/spark_processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      225 2024-05-18 19:53:34.000000 datafog-3.2.1b7/datafog/processing/spark_processing/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2204 2024-05-18 21:08:15.000000 datafog-3.2.1b7/datafog/processing/spark_processing/pyspark_udfs.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:30:35.558853 datafog-3.2.1b7/datafog/processing/text_processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       51 2024-05-18 18:25:55.000000 datafog-3.2.1b7/datafog/processing/text_processing/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1300 2024-05-18 18:25:55.000000 datafog-3.2.1b7/datafog/processing/text_processing/spacy_pii_annotator.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:30:35.559931 datafog-3.2.1b7/datafog/services/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      118 2024-05-18 18:25:55.000000 datafog-3.2.1b7/datafog/services/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1802 2024-05-18 21:08:15.000000 datafog-3.2.1b7/datafog/services/image_service.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1030 2024-05-18 19:53:34.000000 datafog-3.2.1b7/datafog/services/spark_service.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      633 2024-05-18 21:08:14.000000 datafog-3.2.1b7/datafog/services/text_service.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:30:35.560384 datafog-3.2.1b7/datafog/telemetry/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-18 20:37:26.000000 datafog-3.2.1b7/datafog/telemetry/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     3232 2024-05-27 22:26:07.000000 datafog-3.2.1b7/datafog/telemetry/open_telemetry.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:30:35.561486 datafog-3.2.1b7/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     8252 2024-05-27 22:30:35.000000 datafog-3.2.1b7/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      972 2024-05-27 22:30:35.000000 datafog-3.2.1b7/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-27 22:30:35.000000 datafog-3.2.1b7/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)      145 2024-05-27 22:30:35.000000 datafog-3.2.1b7/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       14 2024-05-27 22:30:35.000000 datafog-3.2.1b7/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-27 22:30:35.562459 datafog-3.2.1b7/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1945 2024-05-27 22:30:28.000000 datafog-3.2.1b7/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:30:35.561024 datafog-3.2.1b7/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)        0 2024-05-18 18:25:55.000000 datafog-3.2.1b7/tests/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2543 2024-05-27 22:18:14.000000 datafog-3.2.1b7/tests/test_image_service.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2785 2024-05-18 19:55:12.000000 datafog-3.2.1b7/tests/test_main.py
```

### Comparing `datafog-3.2.1b6/LICENSE` & `datafog-3.2.1b7/LICENSE`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b6/PKG-INFO` & `datafog-3.2.1b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.2.1b6
+Version: 3.2.1b7
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: Sid Mohan
 Author-email: sid@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datafog Version: 3.2.1b6 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.2.1b7 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: Sid Mohan
 Author-email: sid@datafog.ai Maintainer: DataFog Maintainer-email:
 hi@datafog.ai License: MIT Project-URL: Homepage, https://datafog.ai Project-
 URL: Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
```

### Comparing `datafog-3.2.1b6/README.md` & `datafog-3.2.1b7/README.md`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b6/datafog/__init__.py` & `datafog-3.2.1b7/datafog/__init__.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b6/datafog/processing/image_processing/donut_processor.py` & `datafog-3.2.1b7/datafog/processing/image_processing/donut_processor.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b6/datafog/processing/image_processing/image_downloader.py` & `datafog-3.2.1b7/datafog/processing/image_processing/image_downloader.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b6/datafog/processing/spark_processing/pyspark_udfs.py` & `datafog-3.2.1b7/datafog/processing/spark_processing/pyspark_udfs.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b6/datafog/processing/text_processing/spacy_pii_annotator.py` & `datafog-3.2.1b7/datafog/processing/text_processing/spacy_pii_annotator.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b6/datafog/services/image_service.py` & `datafog-3.2.1b7/datafog/services/image_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b6/datafog/services/spark_service.py` & `datafog-3.2.1b7/datafog/services/spark_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b6/datafog/services/text_service.py` & `datafog-3.2.1b7/datafog/services/text_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b6/datafog/telemetry/open_telemetry.py` & `datafog-3.2.1b7/datafog/telemetry/open_telemetry.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,23 +8,14 @@
 from opentelemetry.trace import Status, StatusCode
 
 # Use environment variable if available, otherwise fall back to hardcoded value
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 APPLICATIONINSIGHTS_CONNECTION_STRING = os.getenv("APPLICATIONINSIGHTS_CONNECTION_STRING", "InstrumentationKey=00bea047-1836-46fa-9652-26d43d63a3fa;IngestionEndpoint=https://eastus-8.in.applicationinsights.azure.com/;LiveEndpoint=https://eastus.livediagnostics.monitor.azure.com/;ApplicationId=959cc365-c112-491b-af69-b196d0943ca4")
-def setup_tracing():
-    # Set up the OpenTelemetry tracer provider
-    trace.set_tracer_provider(TracerProvider())
-
-    # Create an Azure Monitor exporter
-    exporter = AzureMonitorTraceExporter(connection_string=APPLICATIONINSIGHTS_CONNECTION_STRING)
-
-    # Add the exporter to the trace provider
-    trace.get_tracer_provider().add_span_processor(BatchSpanProcessor(exporter))
 
 class Telemetry:
     def __init__(self):
         self.ready = False
         self.trace_set = False
         try:
             # Create a new TracerProvider and set it as the global trace provider
@@ -48,22 +39,25 @@
 
             self.ready = True
             self.trace_set = True
 
         except Exception as e:
             print(f"Error setting up Azure Monitor: {e}")
 
-    def set_tracer(self):
-        if self.ready and not self.trace_set:
-            try:
-                trace.set_tracer_provider(self.provider)
-                self.trace_set = True
-            except Exception:
-                self.ready = False
-                self.trace_set = False
+
+    def setup_tracing():
+        # Set up the OpenTelemetry tracer provider
+        trace.set_tracer_provider(TracerProvider())
+
+        # Create an Azure Monitor exporter
+        exporter = AzureMonitorTraceExporter(connection_string=APPLICATIONINSIGHTS_CONNECTION_STRING)
+
+        # Add the exporter to the trace provider
+        trace.get_tracer_provider().add_span_processor(BatchSpanProcessor(exporter))
+
 
     def datafog_creation(self, name: str):
         if self.ready:
             try:
                 tracer = trace.get_tracer(__name__)
                 span = tracer.start_span("datafog object created")
                 self._add_attribute(span, "datafog_name", name)
@@ -77,12 +71,7 @@
     def _add_attribute(self, span, key, value):
         """Add an attribute to a span."""
         try:
             return span.set_attribute(key, value)
         except Exception:
             pass
 
-
-
-
-# Initialize tracing when the SDK is imported
-setup_tracing()
```

### Comparing `datafog-3.2.1b6/datafog.egg-info/PKG-INFO` & `datafog-3.2.1b7/datafog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.2.1b6
+Version: 3.2.1b7
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: Sid Mohan
 Author-email: sid@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datafog Version: 3.2.1b6 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.2.1b7 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: Sid Mohan
 Author-email: sid@datafog.ai Maintainer: DataFog Maintainer-email:
 hi@datafog.ai License: MIT Project-URL: Homepage, https://datafog.ai Project-
 URL: Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
```

### Comparing `datafog-3.2.1b6/datafog.egg-info/SOURCES.txt` & `datafog-3.2.1b7/datafog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b6/setup.py` & `datafog-3.2.1b7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read README for the long description
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 def __version__():
-    return "3.2.1b6"
+    return "3.2.1b7"
 
 
 project_urls = {
     "Homepage": "https://datafog.ai",
     "Documentation": "https://docs.datafog.ai",
     "Discord": "https://discord.gg/bzDth394R4",
     "Twitter": "https://twitter.com/datafoginc",
```

### Comparing `datafog-3.2.1b6/tests/test_image_service.py` & `datafog-3.2.1b7/tests/test_image_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b6/tests/test_main.py` & `datafog-3.2.1b7/tests/test_main.py`

 * *Files identical despite different names*

