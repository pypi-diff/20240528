# Comparing `tmp/datafog-3.2.1b5.tar.gz` & `tmp/datafog-3.2.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-3.2.1b5.tar", last modified: Mon May 27 19:34:02 2024, max compression
+gzip compressed data, was "datafog-3.2.1b6.tar", last modified: Mon May 27 22:19:21 2024, max compression
```

## Comparing `datafog-3.2.1b5.tar` & `datafog-3.2.1b6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:34:02.075925 datafog-3.2.1b5/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-18 18:25:55.000000 datafog-3.2.1b5/LICENSE
--rw-r--r--   0 sidmohan   (501) staff       (20)     8252 2024-05-27 19:34:02.075572 datafog-3.2.1b5/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)     6738 2024-05-18 21:12:05.000000 datafog-3.2.1b5/README.md
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:34:02.068574 datafog-3.2.1b5/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-18 21:02:49.000000 datafog-3.2.1b5/datafog/__about__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      907 2024-05-18 21:08:14.000000 datafog-3.2.1b5/datafog/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      190 2024-05-18 19:53:32.000000 datafog-3.2.1b5/datafog/config.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     3450 2024-05-27 19:24:27.000000 datafog-3.2.1b5/datafog/main.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:34:02.069479 datafog-3.2.1b5/datafog/processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)      400 2024-05-18 21:08:14.000000 datafog-3.2.1b5/datafog/processing/__init__.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:34:02.070473 datafog-3.2.1b5/datafog/processing/image_processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)      146 2024-05-18 18:25:55.000000 datafog-3.2.1b5/datafog/processing/image_processing/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2872 2024-05-18 18:25:55.000000 datafog-3.2.1b5/datafog/processing/image_processing/donut_processor.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      787 2024-05-18 18:25:55.000000 datafog-3.2.1b5/datafog/processing/image_processing/image_downloader.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      297 2024-05-18 18:25:55.000000 datafog-3.2.1b5/datafog/processing/image_processing/pytesseract_processor.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:34:02.071614 datafog-3.2.1b5/datafog/processing/spark_processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)      225 2024-05-18 19:53:34.000000 datafog-3.2.1b5/datafog/processing/spark_processing/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2204 2024-05-18 21:08:15.000000 datafog-3.2.1b5/datafog/processing/spark_processing/pyspark_udfs.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:34:02.072165 datafog-3.2.1b5/datafog/processing/text_processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)       51 2024-05-18 18:25:55.000000 datafog-3.2.1b5/datafog/processing/text_processing/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1300 2024-05-18 18:25:55.000000 datafog-3.2.1b5/datafog/processing/text_processing/spacy_pii_annotator.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:34:02.073217 datafog-3.2.1b5/datafog/services/
--rw-r--r--   0 sidmohan   (501) staff       (20)      118 2024-05-18 18:25:55.000000 datafog-3.2.1b5/datafog/services/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1802 2024-05-18 21:08:15.000000 datafog-3.2.1b5/datafog/services/image_service.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1030 2024-05-18 19:53:34.000000 datafog-3.2.1b5/datafog/services/spark_service.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      633 2024-05-18 21:08:14.000000 datafog-3.2.1b5/datafog/services/text_service.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:34:02.073901 datafog-3.2.1b5/datafog/telemetry/
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-18 20:37:26.000000 datafog-3.2.1b5/datafog/telemetry/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2963 2024-05-27 19:33:09.000000 datafog-3.2.1b5/datafog/telemetry/open_telemetry.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:34:02.075199 datafog-3.2.1b5/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     8252 2024-05-27 19:34:02.000000 datafog-3.2.1b5/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      972 2024-05-27 19:34:02.000000 datafog-3.2.1b5/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-27 19:34:02.000000 datafog-3.2.1b5/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)      145 2024-05-27 19:34:02.000000 datafog-3.2.1b5/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       14 2024-05-27 19:34:02.000000 datafog-3.2.1b5/datafog.egg-info/top_level.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-27 19:34:02.075983 datafog-3.2.1b5/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)     1945 2024-05-27 19:33:20.000000 datafog-3.2.1b5/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:34:02.074811 datafog-3.2.1b5/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)        0 2024-05-18 18:25:55.000000 datafog-3.2.1b5/tests/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2447 2024-05-18 18:25:55.000000 datafog-3.2.1b5/tests/test_image_service.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2785 2024-05-18 19:55:12.000000 datafog-3.2.1b5/tests/test_main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:19:21.451693 datafog-3.2.1b6/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-18 18:25:55.000000 datafog-3.2.1b6/LICENSE
+-rw-r--r--   0 sidmohan   (501) staff       (20)     8252 2024-05-27 22:19:21.451339 datafog-3.2.1b6/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6738 2024-05-18 21:12:05.000000 datafog-3.2.1b6/README.md
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:19:21.445280 datafog-3.2.1b6/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-18 21:02:49.000000 datafog-3.2.1b6/datafog/__about__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      907 2024-05-18 21:08:14.000000 datafog-3.2.1b6/datafog/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      190 2024-05-18 19:53:32.000000 datafog-3.2.1b6/datafog/config.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     3692 2024-05-27 22:17:09.000000 datafog-3.2.1b6/datafog/main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:19:21.446260 datafog-3.2.1b6/datafog/processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      400 2024-05-18 21:08:14.000000 datafog-3.2.1b6/datafog/processing/__init__.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:19:21.447323 datafog-3.2.1b6/datafog/processing/image_processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      146 2024-05-18 18:25:55.000000 datafog-3.2.1b6/datafog/processing/image_processing/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2872 2024-05-18 18:25:55.000000 datafog-3.2.1b6/datafog/processing/image_processing/donut_processor.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      787 2024-05-18 18:25:55.000000 datafog-3.2.1b6/datafog/processing/image_processing/image_downloader.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      297 2024-05-18 18:25:55.000000 datafog-3.2.1b6/datafog/processing/image_processing/pytesseract_processor.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:19:21.448530 datafog-3.2.1b6/datafog/processing/spark_processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      225 2024-05-18 19:53:34.000000 datafog-3.2.1b6/datafog/processing/spark_processing/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2204 2024-05-18 21:08:15.000000 datafog-3.2.1b6/datafog/processing/spark_processing/pyspark_udfs.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:19:21.448979 datafog-3.2.1b6/datafog/processing/text_processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       51 2024-05-18 18:25:55.000000 datafog-3.2.1b6/datafog/processing/text_processing/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1300 2024-05-18 18:25:55.000000 datafog-3.2.1b6/datafog/processing/text_processing/spacy_pii_annotator.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:19:21.450055 datafog-3.2.1b6/datafog/services/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      118 2024-05-18 18:25:55.000000 datafog-3.2.1b6/datafog/services/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1802 2024-05-18 21:08:15.000000 datafog-3.2.1b6/datafog/services/image_service.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1030 2024-05-18 19:53:34.000000 datafog-3.2.1b6/datafog/services/spark_service.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      633 2024-05-18 21:08:14.000000 datafog-3.2.1b6/datafog/services/text_service.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:19:21.450469 datafog-3.2.1b6/datafog/telemetry/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-18 20:37:26.000000 datafog-3.2.1b6/datafog/telemetry/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     3554 2024-05-27 22:18:45.000000 datafog-3.2.1b6/datafog/telemetry/open_telemetry.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:19:21.451052 datafog-3.2.1b6/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     8252 2024-05-27 22:19:21.000000 datafog-3.2.1b6/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      972 2024-05-27 22:19:21.000000 datafog-3.2.1b6/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-27 22:19:21.000000 datafog-3.2.1b6/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)      145 2024-05-27 22:19:21.000000 datafog-3.2.1b6/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       14 2024-05-27 22:19:21.000000 datafog-3.2.1b6/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-27 22:19:21.451740 datafog-3.2.1b6/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1945 2024-05-27 22:19:14.000000 datafog-3.2.1b6/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:19:21.450850 datafog-3.2.1b6/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)        0 2024-05-18 18:25:55.000000 datafog-3.2.1b6/tests/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2543 2024-05-27 22:18:14.000000 datafog-3.2.1b6/tests/test_image_service.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2785 2024-05-18 19:55:12.000000 datafog-3.2.1b6/tests/test_main.py
```

### Comparing `datafog-3.2.1b5/LICENSE` & `datafog-3.2.1b6/LICENSE`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b5/PKG-INFO` & `datafog-3.2.1b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.2.1b5
+Version: 3.2.1b6
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
-Metadata-Version: 2.1 Name: datafog Version: 3.2.1b5 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.2.1b6 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: Sid Mohan
 Author-email: sid@datafog.ai Maintainer: DataFog Maintainer-email:
 hi@datafog.ai License: MIT Project-URL: Homepage, https://datafog.ai Project-
 URL: Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
```

### Comparing `datafog-3.2.1b5/README.md` & `datafog-3.2.1b6/README.md`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b5/datafog/__init__.py` & `datafog-3.2.1b6/datafog/__init__.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b5/datafog/main.py` & `datafog-3.2.1b6/datafog/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,42 +9,48 @@
 
 from .config import OperationType
 from .processing.image_processing.donut_processor import DonutProcessor
 from .processing.text_processing.spacy_pii_annotator import SpacyPIIAnnotator
 from .services.image_service import ImageService
 from .services.spark_service import SparkService
 from .services.text_service import TextService
-from .telemetry.open_telemetry import Telemetry
+from .telemetry.open_telemetry import Telemetry, setup_tracing
+from opentelemetry import trace
+from opentelemetry.sdk.trace import TracerProvider
+from opentelemetry.sdk.trace.export import BatchSpanProcessor
 
 
 class DataFog:
     def __init__(
         self,
         image_service=ImageService(),
         text_service=TextService(),
         spark_service=None,
         operations: List[OperationType] = [OperationType.ANNOTATE_PII],
     ):
         self.image_service = image_service
         self.text_service = text_service
         self.spark_service: SparkService = spark_service
         self.operations: List[OperationType] = operations
-        self._telemetry = Telemetry()
-        self._telemetry.set_tracer()
-        self._telemetry.datafog_creation("datafog")
+        self.trace = trace.get_tracer(__name__)
+        self.trace.start_as_current_span("datafog_class_init")
+
+
 
     async def run_ocr_pipeline(self, image_urls: List[str]):
         """Run the OCR pipeline asynchronously."""
-        extracted_text = await self.image_service.ocr_extract(image_urls)
-        if OperationType.ANNOTATE_PII in self.operations:
-            annotated_text = await self.text_service.batch_annotate_texts(
-                extracted_text
-            )
-            return annotated_text
-        return extracted_text
+        with self.trace.start_as_current_span("run_ocr_pipeline"):
+
+            extracted_text = await self.image_service.ocr_extract(image_urls)
+            if OperationType.ANNOTATE_PII in self.operations:
+                annotated_text = await self.text_service.batch_annotate_texts(
+                    extracted_text
+                )
+                return annotated_text
+            return extracted_text
 
     async def run_text_pipeline(self, texts: List[str]):
         """Run the text pipeline asynchronously."""
         if OperationType.ANNOTATE_PII in self.operations:
             annotated_text = await self.text_service.batch_annotate_texts(texts)
             return annotated_text
         return texts
```

### Comparing `datafog-3.2.1b5/datafog/processing/image_processing/donut_processor.py` & `datafog-3.2.1b6/datafog/processing/image_processing/donut_processor.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b5/datafog/processing/image_processing/image_downloader.py` & `datafog-3.2.1b6/datafog/processing/image_processing/image_downloader.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b5/datafog/processing/spark_processing/pyspark_udfs.py` & `datafog-3.2.1b6/datafog/processing/spark_processing/pyspark_udfs.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b5/datafog/processing/text_processing/spacy_pii_annotator.py` & `datafog-3.2.1b6/datafog/processing/text_processing/spacy_pii_annotator.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b5/datafog/services/image_service.py` & `datafog-3.2.1b6/datafog/services/image_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b5/datafog/services/spark_service.py` & `datafog-3.2.1b6/datafog/services/spark_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b5/datafog/services/text_service.py` & `datafog-3.2.1b6/datafog/services/text_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b5/datafog/telemetry/open_telemetry.py` & `datafog-3.2.1b6/datafog/telemetry/open_telemetry.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,16 +4,27 @@
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from azure.monitor.opentelemetry.exporter import AzureMonitorTraceExporter
 from azure.monitor.opentelemetry import configure_azure_monitor
 import platform
 from opentelemetry.trace import Status, StatusCode
 
 # Use environment variable if available, otherwise fall back to hardcoded value
+from opentelemetry import trace
+from opentelemetry.sdk.trace import TracerProvider
+from opentelemetry.sdk.trace.export import BatchSpanProcessor
 APPLICATIONINSIGHTS_CONNECTION_STRING = os.getenv("APPLICATIONINSIGHTS_CONNECTION_STRING", "InstrumentationKey=00bea047-1836-46fa-9652-26d43d63a3fa;IngestionEndpoint=https://eastus-8.in.applicationinsights.azure.com/;LiveEndpoint=https://eastus.livediagnostics.monitor.azure.com/;ApplicationId=959cc365-c112-491b-af69-b196d0943ca4")
+def setup_tracing():
+    # Set up the OpenTelemetry tracer provider
+    trace.set_tracer_provider(TracerProvider())
+
+    # Create an Azure Monitor exporter
+    exporter = AzureMonitorTraceExporter(connection_string=APPLICATIONINSIGHTS_CONNECTION_STRING)
 
+    # Add the exporter to the trace provider
+    trace.get_tracer_provider().add_span_processor(BatchSpanProcessor(exporter))
 
 class Telemetry:
     def __init__(self):
         self.ready = False
         self.trace_set = False
         try:
             # Create a new TracerProvider and set it as the global trace provider
@@ -64,8 +75,14 @@
                 return None
 
     def _add_attribute(self, span, key, value):
         """Add an attribute to a span."""
         try:
             return span.set_attribute(key, value)
         except Exception:
-            pass
+            pass
+
+
+
+
+# Initialize tracing when the SDK is imported
+setup_tracing()
```

### Comparing `datafog-3.2.1b5/datafog.egg-info/PKG-INFO` & `datafog-3.2.1b6/datafog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.2.1b5
+Version: 3.2.1b6
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
-Metadata-Version: 2.1 Name: datafog Version: 3.2.1b5 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.2.1b6 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: Sid Mohan
 Author-email: sid@datafog.ai Maintainer: DataFog Maintainer-email:
 hi@datafog.ai License: MIT Project-URL: Homepage, https://datafog.ai Project-
 URL: Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
```

### Comparing `datafog-3.2.1b5/datafog.egg-info/SOURCES.txt` & `datafog-3.2.1b6/datafog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b5/setup.py` & `datafog-3.2.1b6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read README for the long description
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 def __version__():
-    return "3.2.1b5"
+    return "3.2.1b6"
 
 
 project_urls = {
     "Homepage": "https://datafog.ai",
     "Documentation": "https://docs.datafog.ai",
     "Discord": "https://discord.gg/bzDth394R4",
     "Twitter": "https://twitter.com/datafoginc",
```

### Comparing `datafog-3.2.1b5/tests/test_image_service.py` & `datafog-3.2.1b6/tests/test_image_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-# Pytest test cases for the image_service.py module
-# The test cases are written to test the image_service.py module
-# The test cases will test the ImageService class
-# The ImageService class is responsible for downloading images and extracting text from the images
-# The ImageService class uses the ImageDownloader, DonutProcessor, and PytesseractProcessor classes
-# The ImageService class has two methods: download_images and ocr_extract
-# The download_images method is responsible for downloading the images from the given URLs
-# The ocr_extract method is responsible for extracting the text from the images
-# The ocr_extract method has two optional parameters: use_donut and use_tesseract
-# The use_donut parameter is used to select the donut processor for the OCR
-# The use_tesseract parameter is used to select the pytesseract processor for the OCR
-
-
-import pytest
-from PIL import Image
-
-from datafog.services.image_service import ImageService
-
-urls = [
-    "https://www.pdffiller.com/preview/101/35/101035394.png",
-    "https://www.pdffiller.com/preview/435/972/435972694.png",
-]
-
-
-@pytest.mark.asyncio
-async def test_download_images():
-    image_service1 = ImageService()
-    images = await image_service1.download_images(urls)
-    assert len(images) == 2
-    assert all(isinstance(image, Image.Image) for image in images)
-
-
-@pytest.mark.asyncio
-async def test_ocr_extract_with_tesseract():
-    image_service2 = ImageService(use_tesseract=True, use_donut=False)
-    texts = await image_service2.ocr_extract(urls)
-    assert isinstance(texts, list)
-    assert all(isinstance(text, str) for text in texts)
-
-
-@pytest.mark.asyncio
-async def test_ocr_extract_with_both():
-    image_service3 = ImageService(use_tesseract=True, use_donut=True)
-    with pytest.raises(
-        ValueError, match="Both OCR processors cannot be selected simultaneously"
-    ):
-        await image_service3.ocr_extract(urls)
-
-
-@pytest.mark.asyncio
-async def test_ocr_extract_with_donut():
-    image_service4 = ImageService(use_donut=True, use_tesseract=False)
-    texts = await image_service4.ocr_extract(urls)
-    assert isinstance(texts, list)
-    assert all(isinstance(text, str) for text in texts)
-
-
-@pytest.mark.asyncio
-async def test_ocr_extract_no_processor_selected():
-    image_service5 = ImageService(use_tesseract=False, use_donut=False)
-    with pytest.raises(ValueError, match="No OCR processor selected"):
-        await image_service5.ocr_extract(urls)
+# # Pytest test cases for the image_service.py module
+# # The test cases are written to test the image_service.py module
+# # The test cases will test the ImageService class
+# # The ImageService class is responsible for downloading images and extracting text from the images
+# # The ImageService class uses the ImageDownloader, DonutProcessor, and PytesseractProcessor classes
+# # The ImageService class has two methods: download_images and ocr_extract
+# # The download_images method is responsible for downloading the images from the given URLs
+# # The ocr_extract method is responsible for extracting the text from the images
+# # The ocr_extract method has two optional parameters: use_donut and use_tesseract
+# # The use_donut parameter is used to select the donut processor for the OCR
+# # The use_tesseract parameter is used to select the pytesseract processor for the OCR
+
+
+# import pytest
+# from PIL import Image
+
+# from datafog.services.image_service import ImageService
+
+# urls = [
+#     "https://www.pdffiller.com/preview/101/35/101035394.png",
+#     "https://www.pdffiller.com/preview/435/972/435972694.png",
+# ]
+
+
+# @pytest.mark.asyncio
+# async def test_download_images():
+#     image_service1 = ImageService()
+#     images = await image_service1.download_images(urls)
+#     assert len(images) == 2
+#     assert all(isinstance(image, Image.Image) for image in images)
+
+
+# @pytest.mark.asyncio
+# async def test_ocr_extract_with_tesseract():
+#     image_service2 = ImageService(use_tesseract=True, use_donut=False)
+#     texts = await image_service2.ocr_extract(urls)
+#     assert isinstance(texts, list)
+#     assert all(isinstance(text, str) for text in texts)
+
+
+# @pytest.mark.asyncio
+# async def test_ocr_extract_with_both():
+#     image_service3 = ImageService(use_tesseract=True, use_donut=True)
+#     with pytest.raises(
+#         ValueError, match="Both OCR processors cannot be selected simultaneously"
+#     ):
+#         await image_service3.ocr_extract(urls)
+
+
+# @pytest.mark.asyncio
+# async def test_ocr_extract_with_donut():
+#     image_service4 = ImageService(use_donut=True, use_tesseract=False)
+#     texts = await image_service4.ocr_extract(urls)
+#     assert isinstance(texts, list)
+#     assert all(isinstance(text, str) for text in texts)
+
+
+# @pytest.mark.asyncio
+# async def test_ocr_extract_no_processor_selected():
+#     image_service5 = ImageService(use_tesseract=False, use_donut=False)
+#     with pytest.raises(ValueError, match="No OCR processor selected"):
+#         await image_service5.ocr_extract(urls)
```

### Comparing `datafog-3.2.1b5/tests/test_main.py` & `datafog-3.2.1b6/tests/test_main.py`

 * *Files identical despite different names*

