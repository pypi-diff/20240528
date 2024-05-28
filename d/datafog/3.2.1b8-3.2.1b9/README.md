# Comparing `tmp/datafog-3.2.1b8.tar.gz` & `tmp/datafog-3.2.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-3.2.1b8.tar", last modified: Mon May 27 23:04:57 2024, max compression
+gzip compressed data, was "datafog-3.2.1b9.tar", last modified: Tue May 28 03:34:07 2024, max compression
```

## Comparing `datafog-3.2.1b8.tar` & `datafog-3.2.1b9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 23:04:57.463732 datafog-3.2.1b8/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-18 18:25:55.000000 datafog-3.2.1b8/LICENSE
--rw-r--r--   0 sidmohan   (501) staff       (20)     8252 2024-05-27 23:04:57.463348 datafog-3.2.1b8/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)     6738 2024-05-18 21:12:05.000000 datafog-3.2.1b8/README.md
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 23:04:57.458846 datafog-3.2.1b8/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-18 21:02:49.000000 datafog-3.2.1b8/datafog/__about__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      907 2024-05-18 21:08:14.000000 datafog-3.2.1b8/datafog/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      190 2024-05-18 19:53:32.000000 datafog-3.2.1b8/datafog/config.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     8117 2024-05-27 23:03:41.000000 datafog-3.2.1b8/datafog/main.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 23:04:57.460038 datafog-3.2.1b8/datafog/processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)      400 2024-05-18 21:08:14.000000 datafog-3.2.1b8/datafog/processing/__init__.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 23:04:57.460616 datafog-3.2.1b8/datafog/processing/image_processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)      146 2024-05-18 18:25:55.000000 datafog-3.2.1b8/datafog/processing/image_processing/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2872 2024-05-18 18:25:55.000000 datafog-3.2.1b8/datafog/processing/image_processing/donut_processor.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      787 2024-05-18 18:25:55.000000 datafog-3.2.1b8/datafog/processing/image_processing/image_downloader.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      297 2024-05-18 18:25:55.000000 datafog-3.2.1b8/datafog/processing/image_processing/pytesseract_processor.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 23:04:57.460924 datafog-3.2.1b8/datafog/processing/spark_processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)      225 2024-05-18 19:53:34.000000 datafog-3.2.1b8/datafog/processing/spark_processing/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2204 2024-05-18 21:08:15.000000 datafog-3.2.1b8/datafog/processing/spark_processing/pyspark_udfs.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 23:04:57.461323 datafog-3.2.1b8/datafog/processing/text_processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)       51 2024-05-18 18:25:55.000000 datafog-3.2.1b8/datafog/processing/text_processing/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1300 2024-05-18 18:25:55.000000 datafog-3.2.1b8/datafog/processing/text_processing/spacy_pii_annotator.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 23:04:57.462050 datafog-3.2.1b8/datafog/services/
--rw-r--r--   0 sidmohan   (501) staff       (20)      118 2024-05-18 18:25:55.000000 datafog-3.2.1b8/datafog/services/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1802 2024-05-18 21:08:15.000000 datafog-3.2.1b8/datafog/services/image_service.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1030 2024-05-18 19:53:34.000000 datafog-3.2.1b8/datafog/services/spark_service.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      633 2024-05-18 21:08:14.000000 datafog-3.2.1b8/datafog/services/text_service.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 23:04:57.462382 datafog-3.2.1b8/datafog/telemetry/
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-18 20:37:26.000000 datafog-3.2.1b8/datafog/telemetry/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     3232 2024-05-27 22:26:07.000000 datafog-3.2.1b8/datafog/telemetry/open_telemetry.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 23:04:57.463000 datafog-3.2.1b8/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     8252 2024-05-27 23:04:57.000000 datafog-3.2.1b8/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      972 2024-05-27 23:04:57.000000 datafog-3.2.1b8/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-27 23:04:57.000000 datafog-3.2.1b8/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)      145 2024-05-27 23:04:57.000000 datafog-3.2.1b8/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       14 2024-05-27 23:04:57.000000 datafog-3.2.1b8/datafog.egg-info/top_level.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-27 23:04:57.463782 datafog-3.2.1b8/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)     1945 2024-05-27 23:04:52.000000 datafog-3.2.1b8/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 23:04:57.462786 datafog-3.2.1b8/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)        0 2024-05-18 18:25:55.000000 datafog-3.2.1b8/tests/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2543 2024-05-27 22:18:14.000000 datafog-3.2.1b8/tests/test_image_service.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2785 2024-05-18 19:55:12.000000 datafog-3.2.1b8/tests/test_main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-28 03:34:07.501092 datafog-3.2.1b9/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-18 18:25:55.000000 datafog-3.2.1b9/LICENSE
+-rw-r--r--   0 sidmohan   (501) staff       (20)     8419 2024-05-28 03:34:07.500703 datafog-3.2.1b9/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6738 2024-05-18 21:12:05.000000 datafog-3.2.1b9/README.md
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-28 03:34:07.491034 datafog-3.2.1b9/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-18 21:02:49.000000 datafog-3.2.1b9/datafog/__about__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      907 2024-05-18 21:08:14.000000 datafog-3.2.1b9/datafog/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      190 2024-05-18 19:53:32.000000 datafog-3.2.1b9/datafog/config.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6528 2024-05-28 03:26:03.000000 datafog-3.2.1b9/datafog/main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-28 03:34:07.492127 datafog-3.2.1b9/datafog/processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      400 2024-05-18 21:08:14.000000 datafog-3.2.1b9/datafog/processing/__init__.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-28 03:34:07.495534 datafog-3.2.1b9/datafog/processing/image_processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      146 2024-05-18 18:25:55.000000 datafog-3.2.1b9/datafog/processing/image_processing/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2872 2024-05-18 18:25:55.000000 datafog-3.2.1b9/datafog/processing/image_processing/donut_processor.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      787 2024-05-18 18:25:55.000000 datafog-3.2.1b9/datafog/processing/image_processing/image_downloader.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      297 2024-05-18 18:25:55.000000 datafog-3.2.1b9/datafog/processing/image_processing/pytesseract_processor.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-28 03:34:07.496863 datafog-3.2.1b9/datafog/processing/spark_processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      225 2024-05-18 19:53:34.000000 datafog-3.2.1b9/datafog/processing/spark_processing/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2204 2024-05-18 21:08:15.000000 datafog-3.2.1b9/datafog/processing/spark_processing/pyspark_udfs.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-28 03:34:07.497293 datafog-3.2.1b9/datafog/processing/text_processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       51 2024-05-18 18:25:55.000000 datafog-3.2.1b9/datafog/processing/text_processing/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1300 2024-05-18 18:25:55.000000 datafog-3.2.1b9/datafog/processing/text_processing/spacy_pii_annotator.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-28 03:34:07.498277 datafog-3.2.1b9/datafog/services/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      118 2024-05-18 18:25:55.000000 datafog-3.2.1b9/datafog/services/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1802 2024-05-18 21:08:15.000000 datafog-3.2.1b9/datafog/services/image_service.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1030 2024-05-18 19:53:34.000000 datafog-3.2.1b9/datafog/services/spark_service.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      633 2024-05-18 21:08:14.000000 datafog-3.2.1b9/datafog/services/text_service.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-28 03:34:07.498620 datafog-3.2.1b9/datafog/telemetry/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-18 20:37:26.000000 datafog-3.2.1b9/datafog/telemetry/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2728 2024-05-28 03:28:44.000000 datafog-3.2.1b9/datafog/telemetry/open_telemetry.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-28 03:34:07.500348 datafog-3.2.1b9/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     8419 2024-05-28 03:34:07.000000 datafog-3.2.1b9/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      972 2024-05-28 03:34:07.000000 datafog-3.2.1b9/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-28 03:34:07.000000 datafog-3.2.1b9/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)      252 2024-05-28 03:34:07.000000 datafog-3.2.1b9/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       14 2024-05-28 03:34:07.000000 datafog-3.2.1b9/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-28 03:34:07.501149 datafog-3.2.1b9/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2095 2024-05-28 03:33:15.000000 datafog-3.2.1b9/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-28 03:34:07.500099 datafog-3.2.1b9/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)        0 2024-05-18 18:25:55.000000 datafog-3.2.1b9/tests/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2543 2024-05-27 22:18:14.000000 datafog-3.2.1b9/tests/test_image_service.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2785 2024-05-18 19:55:12.000000 datafog-3.2.1b9/tests/test_main.py
```

### Comparing `datafog-3.2.1b8/LICENSE` & `datafog-3.2.1b9/LICENSE`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b8/PKG-INFO` & `datafog-3.2.1b9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.2.1b8
+Version: 3.2.1b9
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: Sid Mohan
 Author-email: sid@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
@@ -34,14 +34,18 @@
 Requires-Dist: pydantic==1.10.15
 Requires-Dist: Pillow
 Requires-Dist: sentencepiece
 Requires-Dist: protobuf
 Requires-Dist: pytesseract
 Requires-Dist: aiohttp
 Requires-Dist: pytest-asyncio
+Requires-Dist: python-dotenv
+Requires-Dist: azure-monitor-opentelemetry-exporter==1.0.0b25
+Requires-Dist: opentelemetry-sdk
+Requires-Dist: azure-monitor-opentelemetry
 
 <p align="center">
   <a href="https://www.datafog.ai"><img src="public/colorlogo.png" alt="DataFog logo"></a>
 </p>
 
 <p align="center">
     <b>Open-source DevSecOps for Generative AI Systems</b>. <br />
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datafog Version: 3.2.1b8 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.2.1b9 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: Sid Mohan
 Author-email: sid@datafog.ai Maintainer: DataFog Maintainer-email:
 hi@datafog.ai License: MIT Project-URL: Homepage, https://datafog.ai Project-
 URL: Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
@@ -13,15 +13,17 @@
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pandas Requires-Dist: Requests==2.31.0 Requires-Dist: spacy==3.4.4 Requires-
 Dist: en_spacy_pii_fast==0.0.0 Requires-Dist: pydantic==1.10.15 Requires-Dist:
 Pillow Requires-Dist: sentencepiece Requires-Dist: protobuf Requires-Dist:
-pytesseract Requires-Dist: aiohttp Requires-Dist: pytest-asyncio
+pytesseract Requires-Dist: aiohttp Requires-Dist: pytest-asyncio Requires-Dist:
+python-dotenv Requires-Dist: azure-monitor-opentelemetry-exporter==1.0.0b25
+Requires-Dist: opentelemetry-sdk Requires-Dist: azure-monitor-opentelemetry
                                 _[_D_a_t_a_F_o_g_ _l_o_g_o_]
                OOppeenn--ssoouurrccee DDeevvSSeeccOOppss ffoorr GGeenneerraattiivvee AAII SSyysstteemmss.
   _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _p_y_v_e_r_s_i_o_n_s_]_[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_P_y_P_i_ _d_o_w_n_l_o_a_d_s_]_[_D_i_s_c_o_r_d_]_[_C_o_d_e
                      _s_t_y_l_e_:_ _b_l_a_c_k_]_[_c_o_d_e_c_o_v_]_[_G_i_t_H_u_b_ _I_s_s_u_e_s_]
 ## Overview ### What is DataFog? DataFog is an open-source DevSecOps platform
 that lets you scan and redact Personally Identifiable Information (PII) out of
 your Generative AI applications. ### Core Problem ![image](https://github.com/
```

### Comparing `datafog-3.2.1b8/README.md` & `datafog-3.2.1b9/README.md`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b8/datafog/__init__.py` & `datafog-3.2.1b9/datafog/__init__.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b8/datafog/main.py` & `datafog-3.2.1b9/datafog/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,63 +25,26 @@
 import platform
 from opentelemetry.trace import Status, StatusCode
 
 # Use environment variable if available, otherwise fall back to hardcoded value
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
+from logging import INFO, getLogger
+from dotenv import load_dotenv
 import logging
 
-# class DataFog:
-#     def __init__(
-#         self,
-#         image_service=ImageService(),
-#         text_service=TextService(),
-#         spark_service=None,
-#         operations: List[OperationType] = [OperationType.ANNOTATE_PII],
-#     ):
-#         self.image_service = image_service
-#         self.text_service = text_service
-#         self.spark_service: SparkService = spark_service
-#         self.operations: List[OperationType] = operations
-#         self.trace = trace.get_tracer(__name__)
-#         self.trace.start_as_current_span("datafog_class_init")
-
-
-
-#     async def run_ocr_pipeline(self, image_urls: List[str]):
-#         """Run the OCR pipeline asynchronously."""
-#         with self.trace.start_as_current_span("run_ocr_pipeline"):
-
-#             extracted_text = await self.image_service.ocr_extract(image_urls)
-#             if OperationType.ANNOTATE_PII in self.operations:
-#                 annotated_text = await self.text_service.batch_annotate_texts(
-#                     extracted_text
-#                 )
-#                 return annotated_text
-#             return extracted_text
-
-#     async def run_text_pipeline(self, texts: List[str]):
-#         """Run the text pipeline asynchronously."""
-#         if OperationType.ANNOTATE_PII in self.operations:
-#             annotated_text = await self.text_service.batch_annotate_texts(texts)
-#             return annotated_text
-#         return texts
-
-# Initialize telemetry
-APPLICATIONINSIGHTS_CONNECTION_STRING = os.getenv(
-    "APPLICATIONINSIGHTS_CONNECTION_STRING",
-    "InstrumentationKey=00bea047-1836-46fa-9652-26d43d63a3fa;IngestionEndpoint=https://eastus-8.in.applicationinsights.azure.com/;LiveEndpoint=https://eastus.livediagnostics.monitor.azure.com/;ApplicationId=959cc365-c112-491b-af69-b196d0943ca4"
-)
+load_dotenv()  # Load environment variables from .env file
+APPLICATIONINSIGHTS_CONNECTION_STRING = os.getenv("APPLICATIONINSIGHTS_CONNECTION_STRING")
 configure_azure_monitor(connection_string=APPLICATIONINSIGHTS_CONNECTION_STRING)
 trace.set_tracer_provider(TracerProvider())
 exporter = AzureMonitorTraceExporter(connection_string=APPLICATIONINSIGHTS_CONNECTION_STRING)
 trace.get_tracer_provider().add_span_processor(BatchSpanProcessor(exporter))
-logger = logging.getLogger(__name__)
-logging.basicConfig(level=logging.INFO)
+logger = logging.getLogger("datafog_logger")
+logger.setLevel(INFO)
 
 class DataFog:
     def __init__(
         self,
         image_service=ImageService(),
         text_service=TextService(),
         spark_service=None,
```

### Comparing `datafog-3.2.1b8/datafog/processing/image_processing/donut_processor.py` & `datafog-3.2.1b9/datafog/processing/image_processing/donut_processor.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b8/datafog/processing/image_processing/image_downloader.py` & `datafog-3.2.1b9/datafog/processing/image_processing/image_downloader.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b8/datafog/processing/spark_processing/pyspark_udfs.py` & `datafog-3.2.1b9/datafog/processing/spark_processing/pyspark_udfs.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b8/datafog/processing/text_processing/spacy_pii_annotator.py` & `datafog-3.2.1b9/datafog/processing/text_processing/spacy_pii_annotator.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b8/datafog/services/image_service.py` & `datafog-3.2.1b9/datafog/services/image_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b8/datafog/services/spark_service.py` & `datafog-3.2.1b9/datafog/services/spark_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b8/datafog/services/text_service.py` & `datafog-3.2.1b9/datafog/services/text_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b8/datafog/telemetry/open_telemetry.py` & `datafog-3.2.1b9/datafog/telemetry/open_telemetry.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,31 +7,36 @@
 import platform
 from opentelemetry.trace import Status, StatusCode
 
 # Use environment variable if available, otherwise fall back to hardcoded value
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
-APPLICATIONINSIGHTS_CONNECTION_STRING = os.getenv("APPLICATIONINSIGHTS_CONNECTION_STRING", "InstrumentationKey=00bea047-1836-46fa-9652-26d43d63a3fa;IngestionEndpoint=https://eastus-8.in.applicationinsights.azure.com/;LiveEndpoint=https://eastus.livediagnostics.monitor.azure.com/;ApplicationId=959cc365-c112-491b-af69-b196d0943ca4")
+from logging import INFO, getLogger
+from dotenv import load_dotenv
+from azure.monitor.opentelemetry import configure_azure_monitor
+load_dotenv()
+
+APPLICATIONINSIGHTS_CONNECTION_STRING = os.getenv("APPLICATIONINSIGHTS_CONNECTION_STRING")
 
 class Telemetry:
     def __init__(self):
         self.ready = False
         self.trace_set = False
         try:
             # Create a new TracerProvider and set it as the global trace provider
             tracer_provider = TracerProvider()
             trace.set_tracer_provider(tracer_provider)
 
             # Configure Azure Monitor with the connection string from environment variables
-            configure_azure_monitor(connection_string=os.environ["APPLICATIONINSIGHTS_CONNECTION_STRING"])
+            configure_azure_monitor(connection_string=APPLICATIONINSIGHTS_CONNECTION_STRING, logger_name="datafog_logger")
 
             # Create an exporter that sends data to Application Insights
             exporter = AzureMonitorTraceExporter(
-                connection_string=os.environ["APPLICATIONINSIGHTS_CONNECTION_STRING"]
+                connection_string=APPLICATIONINSIGHTS_CONNECTION_STRING
             )
 
             # Create a span processor and add it to the tracer provider
             span_processor = BatchSpanProcessor(exporter)
             tracer_provider.add_span_processor(span_processor)
 
             # Get a tracer
@@ -40,24 +45,14 @@
             self.ready = True
             self.trace_set = True
 
         except Exception as e:
             print(f"Error setting up Azure Monitor: {e}")
 
 
-    def setup_tracing():
-        # Set up the OpenTelemetry tracer provider
-        trace.set_tracer_provider(TracerProvider())
-
-        # Create an Azure Monitor exporter
-        exporter = AzureMonitorTraceExporter(connection_string=APPLICATIONINSIGHTS_CONNECTION_STRING)
-
-        # Add the exporter to the trace provider
-        trace.get_tracer_provider().add_span_processor(BatchSpanProcessor(exporter))
-
 
     def datafog_creation(self, name: str):
         if self.ready:
             try:
                 tracer = trace.get_tracer(__name__)
                 span = tracer.start_span("datafog object created")
                 self._add_attribute(span, "datafog_name", name)
```

### Comparing `datafog-3.2.1b8/datafog.egg-info/PKG-INFO` & `datafog-3.2.1b9/datafog.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.2.1b8
+Version: 3.2.1b9
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: Sid Mohan
 Author-email: sid@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
@@ -34,14 +34,18 @@
 Requires-Dist: pydantic==1.10.15
 Requires-Dist: Pillow
 Requires-Dist: sentencepiece
 Requires-Dist: protobuf
 Requires-Dist: pytesseract
 Requires-Dist: aiohttp
 Requires-Dist: pytest-asyncio
+Requires-Dist: python-dotenv
+Requires-Dist: azure-monitor-opentelemetry-exporter==1.0.0b25
+Requires-Dist: opentelemetry-sdk
+Requires-Dist: azure-monitor-opentelemetry
 
 <p align="center">
   <a href="https://www.datafog.ai"><img src="public/colorlogo.png" alt="DataFog logo"></a>
 </p>
 
 <p align="center">
     <b>Open-source DevSecOps for Generative AI Systems</b>. <br />
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datafog Version: 3.2.1b8 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.2.1b9 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: Sid Mohan
 Author-email: sid@datafog.ai Maintainer: DataFog Maintainer-email:
 hi@datafog.ai License: MIT Project-URL: Homepage, https://datafog.ai Project-
 URL: Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
@@ -13,15 +13,17 @@
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 pandas Requires-Dist: Requests==2.31.0 Requires-Dist: spacy==3.4.4 Requires-
 Dist: en_spacy_pii_fast==0.0.0 Requires-Dist: pydantic==1.10.15 Requires-Dist:
 Pillow Requires-Dist: sentencepiece Requires-Dist: protobuf Requires-Dist:
-pytesseract Requires-Dist: aiohttp Requires-Dist: pytest-asyncio
+pytesseract Requires-Dist: aiohttp Requires-Dist: pytest-asyncio Requires-Dist:
+python-dotenv Requires-Dist: azure-monitor-opentelemetry-exporter==1.0.0b25
+Requires-Dist: opentelemetry-sdk Requires-Dist: azure-monitor-opentelemetry
                                 _[_D_a_t_a_F_o_g_ _l_o_g_o_]
                OOppeenn--ssoouurrccee DDeevvSSeeccOOppss ffoorr GGeenneerraattiivvee AAII SSyysstteemmss.
   _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _p_y_v_e_r_s_i_o_n_s_]_[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_P_y_P_i_ _d_o_w_n_l_o_a_d_s_]_[_D_i_s_c_o_r_d_]_[_C_o_d_e
                      _s_t_y_l_e_:_ _b_l_a_c_k_]_[_c_o_d_e_c_o_v_]_[_G_i_t_H_u_b_ _I_s_s_u_e_s_]
 ## Overview ### What is DataFog? DataFog is an open-source DevSecOps platform
 that lets you scan and redact Personally Identifiable Information (PII) out of
 your Generative AI applications. ### Core Problem ![image](https://github.com/
```

### Comparing `datafog-3.2.1b8/datafog.egg-info/SOURCES.txt` & `datafog-3.2.1b9/datafog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b8/setup.py` & `datafog-3.2.1b9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read README for the long description
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 def __version__():
-    return "3.2.1b8"
+    return "3.2.1b9"
 
 
 project_urls = {
     "Homepage": "https://datafog.ai",
     "Documentation": "https://docs.datafog.ai",
     "Discord": "https://discord.gg/bzDth394R4",
     "Twitter": "https://twitter.com/datafoginc",
@@ -38,14 +38,18 @@
         "pydantic==1.10.15",
         "Pillow",
         "sentencepiece",
         "protobuf",
         "pytesseract",
         "aiohttp",
         "pytest-asyncio",
+        "python-dotenv",
+        "azure-monitor-opentelemetry-exporter==1.0.0b25",
+        "opentelemetry-sdk",
+        "azure-monitor-opentelemetry"
     ],
     python_requires=">=3.10",
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `datafog-3.2.1b8/tests/test_image_service.py` & `datafog-3.2.1b9/tests/test_image_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b8/tests/test_main.py` & `datafog-3.2.1b9/tests/test_main.py`

 * *Files identical despite different names*

