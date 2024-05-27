# Comparing `tmp/datafog-3.2.1b4.tar.gz` & `tmp/datafog-3.2.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-3.2.1b4.tar", last modified: Mon May 27 19:25:19 2024, max compression
+gzip compressed data, was "datafog-3.2.1b5.tar", last modified: Mon May 27 19:34:02 2024, max compression
```

## Comparing `datafog-3.2.1b4.tar` & `datafog-3.2.1b5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:25:19.214212 datafog-3.2.1b4/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-18 18:25:55.000000 datafog-3.2.1b4/LICENSE
--rw-r--r--   0 sidmohan   (501) staff       (20)     8252 2024-05-27 19:25:19.213889 datafog-3.2.1b4/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)     6738 2024-05-18 21:12:05.000000 datafog-3.2.1b4/README.md
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:25:19.209778 datafog-3.2.1b4/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-18 21:02:49.000000 datafog-3.2.1b4/datafog/__about__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      907 2024-05-18 21:08:14.000000 datafog-3.2.1b4/datafog/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      190 2024-05-18 19:53:32.000000 datafog-3.2.1b4/datafog/config.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     3450 2024-05-27 19:24:27.000000 datafog-3.2.1b4/datafog/main.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:25:19.210920 datafog-3.2.1b4/datafog/processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)      400 2024-05-18 21:08:14.000000 datafog-3.2.1b4/datafog/processing/__init__.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:25:19.211528 datafog-3.2.1b4/datafog/processing/image_processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)      146 2024-05-18 18:25:55.000000 datafog-3.2.1b4/datafog/processing/image_processing/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2872 2024-05-18 18:25:55.000000 datafog-3.2.1b4/datafog/processing/image_processing/donut_processor.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      787 2024-05-18 18:25:55.000000 datafog-3.2.1b4/datafog/processing/image_processing/image_downloader.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      297 2024-05-18 18:25:55.000000 datafog-3.2.1b4/datafog/processing/image_processing/pytesseract_processor.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:25:19.211809 datafog-3.2.1b4/datafog/processing/spark_processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)      225 2024-05-18 19:53:34.000000 datafog-3.2.1b4/datafog/processing/spark_processing/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2204 2024-05-18 21:08:15.000000 datafog-3.2.1b4/datafog/processing/spark_processing/pyspark_udfs.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:25:19.212106 datafog-3.2.1b4/datafog/processing/text_processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)       51 2024-05-18 18:25:55.000000 datafog-3.2.1b4/datafog/processing/text_processing/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1300 2024-05-18 18:25:55.000000 datafog-3.2.1b4/datafog/processing/text_processing/spacy_pii_annotator.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:25:19.212661 datafog-3.2.1b4/datafog/services/
--rw-r--r--   0 sidmohan   (501) staff       (20)      118 2024-05-18 18:25:55.000000 datafog-3.2.1b4/datafog/services/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1802 2024-05-18 21:08:15.000000 datafog-3.2.1b4/datafog/services/image_service.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1030 2024-05-18 19:53:34.000000 datafog-3.2.1b4/datafog/services/spark_service.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      633 2024-05-18 21:08:14.000000 datafog-3.2.1b4/datafog/services/text_service.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:25:19.212952 datafog-3.2.1b4/datafog/telemetry/
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-18 20:37:26.000000 datafog-3.2.1b4/datafog/telemetry/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2549 2024-05-27 19:21:35.000000 datafog-3.2.1b4/datafog/telemetry/open_telemetry.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:25:19.213576 datafog-3.2.1b4/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     8252 2024-05-27 19:25:19.000000 datafog-3.2.1b4/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      972 2024-05-27 19:25:19.000000 datafog-3.2.1b4/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-27 19:25:19.000000 datafog-3.2.1b4/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)      145 2024-05-27 19:25:19.000000 datafog-3.2.1b4/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       14 2024-05-27 19:25:19.000000 datafog-3.2.1b4/datafog.egg-info/top_level.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-27 19:25:19.214269 datafog-3.2.1b4/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)     1945 2024-05-27 19:05:19.000000 datafog-3.2.1b4/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:25:19.213376 datafog-3.2.1b4/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)        0 2024-05-18 18:25:55.000000 datafog-3.2.1b4/tests/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2447 2024-05-18 18:25:55.000000 datafog-3.2.1b4/tests/test_image_service.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2785 2024-05-18 19:55:12.000000 datafog-3.2.1b4/tests/test_main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:34:02.075925 datafog-3.2.1b5/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-18 18:25:55.000000 datafog-3.2.1b5/LICENSE
+-rw-r--r--   0 sidmohan   (501) staff       (20)     8252 2024-05-27 19:34:02.075572 datafog-3.2.1b5/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6738 2024-05-18 21:12:05.000000 datafog-3.2.1b5/README.md
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:34:02.068574 datafog-3.2.1b5/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-18 21:02:49.000000 datafog-3.2.1b5/datafog/__about__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      907 2024-05-18 21:08:14.000000 datafog-3.2.1b5/datafog/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      190 2024-05-18 19:53:32.000000 datafog-3.2.1b5/datafog/config.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     3450 2024-05-27 19:24:27.000000 datafog-3.2.1b5/datafog/main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:34:02.069479 datafog-3.2.1b5/datafog/processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      400 2024-05-18 21:08:14.000000 datafog-3.2.1b5/datafog/processing/__init__.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:34:02.070473 datafog-3.2.1b5/datafog/processing/image_processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      146 2024-05-18 18:25:55.000000 datafog-3.2.1b5/datafog/processing/image_processing/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2872 2024-05-18 18:25:55.000000 datafog-3.2.1b5/datafog/processing/image_processing/donut_processor.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      787 2024-05-18 18:25:55.000000 datafog-3.2.1b5/datafog/processing/image_processing/image_downloader.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      297 2024-05-18 18:25:55.000000 datafog-3.2.1b5/datafog/processing/image_processing/pytesseract_processor.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:34:02.071614 datafog-3.2.1b5/datafog/processing/spark_processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      225 2024-05-18 19:53:34.000000 datafog-3.2.1b5/datafog/processing/spark_processing/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2204 2024-05-18 21:08:15.000000 datafog-3.2.1b5/datafog/processing/spark_processing/pyspark_udfs.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:34:02.072165 datafog-3.2.1b5/datafog/processing/text_processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       51 2024-05-18 18:25:55.000000 datafog-3.2.1b5/datafog/processing/text_processing/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1300 2024-05-18 18:25:55.000000 datafog-3.2.1b5/datafog/processing/text_processing/spacy_pii_annotator.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:34:02.073217 datafog-3.2.1b5/datafog/services/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      118 2024-05-18 18:25:55.000000 datafog-3.2.1b5/datafog/services/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1802 2024-05-18 21:08:15.000000 datafog-3.2.1b5/datafog/services/image_service.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1030 2024-05-18 19:53:34.000000 datafog-3.2.1b5/datafog/services/spark_service.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      633 2024-05-18 21:08:14.000000 datafog-3.2.1b5/datafog/services/text_service.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:34:02.073901 datafog-3.2.1b5/datafog/telemetry/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-18 20:37:26.000000 datafog-3.2.1b5/datafog/telemetry/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2963 2024-05-27 19:33:09.000000 datafog-3.2.1b5/datafog/telemetry/open_telemetry.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:34:02.075199 datafog-3.2.1b5/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     8252 2024-05-27 19:34:02.000000 datafog-3.2.1b5/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      972 2024-05-27 19:34:02.000000 datafog-3.2.1b5/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-27 19:34:02.000000 datafog-3.2.1b5/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)      145 2024-05-27 19:34:02.000000 datafog-3.2.1b5/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       14 2024-05-27 19:34:02.000000 datafog-3.2.1b5/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-27 19:34:02.075983 datafog-3.2.1b5/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1945 2024-05-27 19:33:20.000000 datafog-3.2.1b5/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:34:02.074811 datafog-3.2.1b5/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)        0 2024-05-18 18:25:55.000000 datafog-3.2.1b5/tests/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2447 2024-05-18 18:25:55.000000 datafog-3.2.1b5/tests/test_image_service.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2785 2024-05-18 19:55:12.000000 datafog-3.2.1b5/tests/test_main.py
```

### Comparing `datafog-3.2.1b4/LICENSE` & `datafog-3.2.1b5/LICENSE`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b4/PKG-INFO` & `datafog-3.2.1b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.2.1b4
+Version: 3.2.1b5
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
-Metadata-Version: 2.1 Name: datafog Version: 3.2.1b4 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.2.1b5 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: Sid Mohan
 Author-email: sid@datafog.ai Maintainer: DataFog Maintainer-email:
 hi@datafog.ai License: MIT Project-URL: Homepage, https://datafog.ai Project-
 URL: Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
```

### Comparing `datafog-3.2.1b4/README.md` & `datafog-3.2.1b5/README.md`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b4/datafog/__init__.py` & `datafog-3.2.1b5/datafog/__init__.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b4/datafog/main.py` & `datafog-3.2.1b5/datafog/main.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b4/datafog/processing/image_processing/donut_processor.py` & `datafog-3.2.1b5/datafog/processing/image_processing/donut_processor.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b4/datafog/processing/image_processing/image_downloader.py` & `datafog-3.2.1b5/datafog/processing/image_processing/image_downloader.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b4/datafog/processing/spark_processing/pyspark_udfs.py` & `datafog-3.2.1b5/datafog/processing/spark_processing/pyspark_udfs.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b4/datafog/processing/text_processing/spacy_pii_annotator.py` & `datafog-3.2.1b5/datafog/processing/text_processing/spacy_pii_annotator.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b4/datafog/services/image_service.py` & `datafog-3.2.1b5/datafog/services/image_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b4/datafog/services/spark_service.py` & `datafog-3.2.1b5/datafog/services/spark_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b4/datafog/services/text_service.py` & `datafog-3.2.1b5/datafog/services/text_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b4/datafog.egg-info/PKG-INFO` & `datafog-3.2.1b5/datafog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.2.1b4
+Version: 3.2.1b5
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
-Metadata-Version: 2.1 Name: datafog Version: 3.2.1b4 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.2.1b5 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: Sid Mohan
 Author-email: sid@datafog.ai Maintainer: DataFog Maintainer-email:
 hi@datafog.ai License: MIT Project-URL: Homepage, https://datafog.ai Project-
 URL: Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
```

### Comparing `datafog-3.2.1b4/datafog.egg-info/SOURCES.txt` & `datafog-3.2.1b5/datafog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b4/setup.py` & `datafog-3.2.1b5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read README for the long description
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 def __version__():
-    return "3.2.1b4"
+    return "3.2.1b5"
 
 
 project_urls = {
     "Homepage": "https://datafog.ai",
     "Documentation": "https://docs.datafog.ai",
     "Discord": "https://discord.gg/bzDth394R4",
     "Twitter": "https://twitter.com/datafoginc",
```

### Comparing `datafog-3.2.1b4/tests/test_image_service.py` & `datafog-3.2.1b5/tests/test_image_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b4/tests/test_main.py` & `datafog-3.2.1b5/tests/test_main.py`

 * *Files identical despite different names*

