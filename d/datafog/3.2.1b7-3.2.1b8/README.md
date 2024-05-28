# Comparing `tmp/datafog-3.2.1b7.tar.gz` & `tmp/datafog-3.2.1b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-3.2.1b7.tar", last modified: Mon May 27 22:30:35 2024, max compression
+gzip compressed data, was "datafog-3.2.1b8.tar", last modified: Mon May 27 23:04:57 2024, max compression
```

## Comparing `datafog-3.2.1b7.tar` & `datafog-3.2.1b8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:30:35.562404 datafog-3.2.1b7/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-18 18:25:55.000000 datafog-3.2.1b7/LICENSE
--rw-r--r--   0 sidmohan   (501) staff       (20)     8252 2024-05-27 22:30:35.561817 datafog-3.2.1b7/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)     6738 2024-05-18 21:12:05.000000 datafog-3.2.1b7/README.md
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:30:35.555103 datafog-3.2.1b7/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-18 21:02:49.000000 datafog-3.2.1b7/datafog/__about__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      907 2024-05-18 21:08:14.000000 datafog-3.2.1b7/datafog/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      190 2024-05-18 19:53:32.000000 datafog-3.2.1b7/datafog/config.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     7543 2024-05-27 22:30:10.000000 datafog-3.2.1b7/datafog/main.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:30:35.556084 datafog-3.2.1b7/datafog/processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)      400 2024-05-18 21:08:14.000000 datafog-3.2.1b7/datafog/processing/__init__.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:30:35.557096 datafog-3.2.1b7/datafog/processing/image_processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)      146 2024-05-18 18:25:55.000000 datafog-3.2.1b7/datafog/processing/image_processing/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2872 2024-05-18 18:25:55.000000 datafog-3.2.1b7/datafog/processing/image_processing/donut_processor.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      787 2024-05-18 18:25:55.000000 datafog-3.2.1b7/datafog/processing/image_processing/image_downloader.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      297 2024-05-18 18:25:55.000000 datafog-3.2.1b7/datafog/processing/image_processing/pytesseract_processor.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:30:35.558324 datafog-3.2.1b7/datafog/processing/spark_processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)      225 2024-05-18 19:53:34.000000 datafog-3.2.1b7/datafog/processing/spark_processing/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2204 2024-05-18 21:08:15.000000 datafog-3.2.1b7/datafog/processing/spark_processing/pyspark_udfs.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:30:35.558853 datafog-3.2.1b7/datafog/processing/text_processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)       51 2024-05-18 18:25:55.000000 datafog-3.2.1b7/datafog/processing/text_processing/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1300 2024-05-18 18:25:55.000000 datafog-3.2.1b7/datafog/processing/text_processing/spacy_pii_annotator.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:30:35.559931 datafog-3.2.1b7/datafog/services/
--rw-r--r--   0 sidmohan   (501) staff       (20)      118 2024-05-18 18:25:55.000000 datafog-3.2.1b7/datafog/services/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1802 2024-05-18 21:08:15.000000 datafog-3.2.1b7/datafog/services/image_service.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1030 2024-05-18 19:53:34.000000 datafog-3.2.1b7/datafog/services/spark_service.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      633 2024-05-18 21:08:14.000000 datafog-3.2.1b7/datafog/services/text_service.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:30:35.560384 datafog-3.2.1b7/datafog/telemetry/
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-18 20:37:26.000000 datafog-3.2.1b7/datafog/telemetry/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     3232 2024-05-27 22:26:07.000000 datafog-3.2.1b7/datafog/telemetry/open_telemetry.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:30:35.561486 datafog-3.2.1b7/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     8252 2024-05-27 22:30:35.000000 datafog-3.2.1b7/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      972 2024-05-27 22:30:35.000000 datafog-3.2.1b7/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-27 22:30:35.000000 datafog-3.2.1b7/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)      145 2024-05-27 22:30:35.000000 datafog-3.2.1b7/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       14 2024-05-27 22:30:35.000000 datafog-3.2.1b7/datafog.egg-info/top_level.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-27 22:30:35.562459 datafog-3.2.1b7/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)     1945 2024-05-27 22:30:28.000000 datafog-3.2.1b7/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 22:30:35.561024 datafog-3.2.1b7/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)        0 2024-05-18 18:25:55.000000 datafog-3.2.1b7/tests/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2543 2024-05-27 22:18:14.000000 datafog-3.2.1b7/tests/test_image_service.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2785 2024-05-18 19:55:12.000000 datafog-3.2.1b7/tests/test_main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 23:04:57.463732 datafog-3.2.1b8/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-18 18:25:55.000000 datafog-3.2.1b8/LICENSE
+-rw-r--r--   0 sidmohan   (501) staff       (20)     8252 2024-05-27 23:04:57.463348 datafog-3.2.1b8/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6738 2024-05-18 21:12:05.000000 datafog-3.2.1b8/README.md
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 23:04:57.458846 datafog-3.2.1b8/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-18 21:02:49.000000 datafog-3.2.1b8/datafog/__about__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      907 2024-05-18 21:08:14.000000 datafog-3.2.1b8/datafog/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      190 2024-05-18 19:53:32.000000 datafog-3.2.1b8/datafog/config.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     8117 2024-05-27 23:03:41.000000 datafog-3.2.1b8/datafog/main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 23:04:57.460038 datafog-3.2.1b8/datafog/processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      400 2024-05-18 21:08:14.000000 datafog-3.2.1b8/datafog/processing/__init__.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 23:04:57.460616 datafog-3.2.1b8/datafog/processing/image_processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      146 2024-05-18 18:25:55.000000 datafog-3.2.1b8/datafog/processing/image_processing/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2872 2024-05-18 18:25:55.000000 datafog-3.2.1b8/datafog/processing/image_processing/donut_processor.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      787 2024-05-18 18:25:55.000000 datafog-3.2.1b8/datafog/processing/image_processing/image_downloader.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      297 2024-05-18 18:25:55.000000 datafog-3.2.1b8/datafog/processing/image_processing/pytesseract_processor.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 23:04:57.460924 datafog-3.2.1b8/datafog/processing/spark_processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      225 2024-05-18 19:53:34.000000 datafog-3.2.1b8/datafog/processing/spark_processing/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2204 2024-05-18 21:08:15.000000 datafog-3.2.1b8/datafog/processing/spark_processing/pyspark_udfs.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 23:04:57.461323 datafog-3.2.1b8/datafog/processing/text_processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       51 2024-05-18 18:25:55.000000 datafog-3.2.1b8/datafog/processing/text_processing/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1300 2024-05-18 18:25:55.000000 datafog-3.2.1b8/datafog/processing/text_processing/spacy_pii_annotator.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 23:04:57.462050 datafog-3.2.1b8/datafog/services/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      118 2024-05-18 18:25:55.000000 datafog-3.2.1b8/datafog/services/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1802 2024-05-18 21:08:15.000000 datafog-3.2.1b8/datafog/services/image_service.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1030 2024-05-18 19:53:34.000000 datafog-3.2.1b8/datafog/services/spark_service.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      633 2024-05-18 21:08:14.000000 datafog-3.2.1b8/datafog/services/text_service.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 23:04:57.462382 datafog-3.2.1b8/datafog/telemetry/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-18 20:37:26.000000 datafog-3.2.1b8/datafog/telemetry/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     3232 2024-05-27 22:26:07.000000 datafog-3.2.1b8/datafog/telemetry/open_telemetry.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 23:04:57.463000 datafog-3.2.1b8/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     8252 2024-05-27 23:04:57.000000 datafog-3.2.1b8/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      972 2024-05-27 23:04:57.000000 datafog-3.2.1b8/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-27 23:04:57.000000 datafog-3.2.1b8/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)      145 2024-05-27 23:04:57.000000 datafog-3.2.1b8/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       14 2024-05-27 23:04:57.000000 datafog-3.2.1b8/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-27 23:04:57.463782 datafog-3.2.1b8/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1945 2024-05-27 23:04:52.000000 datafog-3.2.1b8/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 23:04:57.462786 datafog-3.2.1b8/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)        0 2024-05-18 18:25:55.000000 datafog-3.2.1b8/tests/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2543 2024-05-27 22:18:14.000000 datafog-3.2.1b8/tests/test_image_service.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2785 2024-05-18 19:55:12.000000 datafog-3.2.1b8/tests/test_main.py
```

### Comparing `datafog-3.2.1b7/LICENSE` & `datafog-3.2.1b8/LICENSE`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b7/PKG-INFO` & `datafog-3.2.1b8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.2.1b7
+Version: 3.2.1b8
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
-Metadata-Version: 2.1 Name: datafog Version: 3.2.1b7 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.2.1b8 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: Sid Mohan
 Author-email: sid@datafog.ai Maintainer: DataFog Maintainer-email:
 hi@datafog.ai License: MIT Project-URL: Homepage, https://datafog.ai Project-
 URL: Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
```

### Comparing `datafog-3.2.1b7/README.md` & `datafog-3.2.1b8/README.md`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b7/datafog/__init__.py` & `datafog-3.2.1b8/datafog/__init__.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b7/datafog/main.py` & `datafog-3.2.1b8/datafog/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import platform
 from opentelemetry.trace import Status, StatusCode
 
 # Use environment variable if available, otherwise fall back to hardcoded value
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
+import logging
 
 # class DataFog:
 #     def __init__(
 #         self,
 #         image_service=ImageService(),
 #         text_service=TextService(),
 #         spark_service=None,
@@ -67,73 +68,75 @@
 #         return texts
 
 # Initialize telemetry
 APPLICATIONINSIGHTS_CONNECTION_STRING = os.getenv(
     "APPLICATIONINSIGHTS_CONNECTION_STRING",
     "InstrumentationKey=00bea047-1836-46fa-9652-26d43d63a3fa;IngestionEndpoint=https://eastus-8.in.applicationinsights.azure.com/;LiveEndpoint=https://eastus.livediagnostics.monitor.azure.com/;ApplicationId=959cc365-c112-491b-af69-b196d0943ca4"
 )
-
+configure_azure_monitor(connection_string=APPLICATIONINSIGHTS_CONNECTION_STRING)
 trace.set_tracer_provider(TracerProvider())
 exporter = AzureMonitorTraceExporter(connection_string=APPLICATIONINSIGHTS_CONNECTION_STRING)
 trace.get_tracer_provider().add_span_processor(BatchSpanProcessor(exporter))
+logger = logging.getLogger(__name__)
+logging.basicConfig(level=logging.INFO)
 
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
+        self.logger = logging.getLogger(__name__)
+        self.logger.info("Initializing DataFog class with the following services and operations:")
+        self.logger.info(f"Image Service: {type(image_service)}")
+        self.logger.info(f"Text Service: {type(text_service)}")
+        self.logger.info(f"Spark Service: {type(spark_service) if spark_service else 'None'}")
+        self.logger.info(f"Operations: {operations}")
         self.tracer = trace.get_tracer(__name__)
-        with self.tracer.start_as_current_span("datafog_class_init") as span:
-            self._add_attributes(span, {
-                "image_service": str(type(image_service)),
-                "text_service": str(type(text_service)),
-                "spark_service": str(type(spark_service)) if spark_service else "None",
-                "operations": str(operations)
-            })
 
     async def run_ocr_pipeline(self, image_urls: List[str]):
         """Run the OCR pipeline asynchronously."""
         with self.tracer.start_as_current_span("run_ocr_pipeline") as span:
             try:
                 extracted_text = await self.image_service.ocr_extract(image_urls)
-                span.set_attribute("num_images", len(image_urls))
-                span.set_attribute("extracted_text_length", sum(len(text) for text in extracted_text))
+                self.logger.info(f"OCR extraction completed for {len(image_urls)} images.")
+                self.logger.debug(f"Total length of extracted text: {sum(len(text) for text in extracted_text)}")
 
                 if OperationType.ANNOTATE_PII in self.operations:
                     annotated_text = await self.text_service.batch_annotate_texts(extracted_text)
-                    span.set_attribute("num_annotations", len(annotated_text))
+                    self.logger.info(f"Text annotation completed with {len(annotated_text)} annotations.")
                     return annotated_text
                 
                 return extracted_text
             except Exception as e:
+                self.logger.error(f"Error in run_ocr_pipeline: {str(e)}")
                 span.set_status(Status(StatusCode.ERROR, str(e)))
                 raise
-
     async def run_text_pipeline(self, texts: List[str]):
         """Run the text pipeline asynchronously."""
         with self.tracer.start_as_current_span("run_text_pipeline") as span:
             try:
-                span.set_attribute("num_texts", len(texts))
+                self.logger.info(f"Starting text pipeline with {len(texts)} texts.")
                 if OperationType.ANNOTATE_PII in self.operations:
                     annotated_text = await self.text_service.batch_annotate_texts(texts)
-                    span.set_attribute("num_annotations", len(annotated_text))
+                    self.logger.info(f"Text annotation completed with {len(annotated_text)} annotations.")
                     return annotated_text
                 
+                self.logger.info("No annotation operation found; returning original texts.")
                 return texts
             except Exception as e:
+                self.logger.error(f"Error in run_text_pipeline: {str(e)}")
                 span.set_status(Status(StatusCode.ERROR, str(e)))
                 raise
-
     def _add_attributes(self, span, attributes: dict):
         """Add multiple attributes to a span."""
         for key, value in attributes.items():
             span.set_attribute(key, value)
 
 
 class OCRPIIAnnotator:
```

### Comparing `datafog-3.2.1b7/datafog/processing/image_processing/donut_processor.py` & `datafog-3.2.1b8/datafog/processing/image_processing/donut_processor.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b7/datafog/processing/image_processing/image_downloader.py` & `datafog-3.2.1b8/datafog/processing/image_processing/image_downloader.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b7/datafog/processing/spark_processing/pyspark_udfs.py` & `datafog-3.2.1b8/datafog/processing/spark_processing/pyspark_udfs.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b7/datafog/processing/text_processing/spacy_pii_annotator.py` & `datafog-3.2.1b8/datafog/processing/text_processing/spacy_pii_annotator.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b7/datafog/services/image_service.py` & `datafog-3.2.1b8/datafog/services/image_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b7/datafog/services/spark_service.py` & `datafog-3.2.1b8/datafog/services/spark_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b7/datafog/services/text_service.py` & `datafog-3.2.1b8/datafog/services/text_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b7/datafog/telemetry/open_telemetry.py` & `datafog-3.2.1b8/datafog/telemetry/open_telemetry.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b7/datafog.egg-info/PKG-INFO` & `datafog-3.2.1b8/datafog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.2.1b7
+Version: 3.2.1b8
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
-Metadata-Version: 2.1 Name: datafog Version: 3.2.1b7 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.2.1b8 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: Sid Mohan
 Author-email: sid@datafog.ai Maintainer: DataFog Maintainer-email:
 hi@datafog.ai License: MIT Project-URL: Homepage, https://datafog.ai Project-
 URL: Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
```

### Comparing `datafog-3.2.1b7/datafog.egg-info/SOURCES.txt` & `datafog-3.2.1b8/datafog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b7/setup.py` & `datafog-3.2.1b8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read README for the long description
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 def __version__():
-    return "3.2.1b7"
+    return "3.2.1b8"
 
 
 project_urls = {
     "Homepage": "https://datafog.ai",
     "Documentation": "https://docs.datafog.ai",
     "Discord": "https://discord.gg/bzDth394R4",
     "Twitter": "https://twitter.com/datafoginc",
```

### Comparing `datafog-3.2.1b7/tests/test_image_service.py` & `datafog-3.2.1b8/tests/test_image_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b7/tests/test_main.py` & `datafog-3.2.1b8/tests/test_main.py`

 * *Files identical despite different names*

