# Comparing `tmp/scalexi-0.4.6.1.tar.gz` & `tmp/scalexi-0.4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalexi-0.4.6.1.tar", last modified: Sat May 25 09:48:57 2024, max compression
+gzip compressed data, was "scalexi-0.4.7.0.tar", last modified: Tue May 28 07:35:53 2024, max compression
```

## Comparing `scalexi-0.4.6.1.tar` & `scalexi-0.4.7.0.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-25 09:48:57.219951 scalexi-0.4.6.1/
--rw-r--r--   0 akoubaa    (501) staff       (20)     2751 2023-11-18 18:27:29.000000 scalexi-0.4.6.1/LICENSE
--rw-r--r--   0 akoubaa    (501) staff       (20)     4525 2024-05-25 09:48:57.219819 scalexi-0.4.6.1/PKG-INFO
--rw-r--r--   0 akoubaa    (501) staff       (20)    15922 2023-11-22 16:53:27.000000 scalexi-0.4.6.1/README.md
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-25 09:48:57.211962 scalexi-0.4.6.1/scalexi/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.6.1/scalexi/__init__.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-25 09:48:57.213302 scalexi-0.4.6.1/scalexi/data/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.6.1/scalexi/data/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     3517 2024-05-20 20:35:19.000000 scalexi-0.4.6.1/scalexi/data/openai_pricing.json
--rw-r--r--   0 akoubaa    (501) staff       (20)     3723 2024-03-11 15:00:18.000000 scalexi-0.4.6.1/scalexi/data/openai_pricing_v1.json
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-25 09:48:57.213644 scalexi-0.4.6.1/scalexi/dataset_generation/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.6.1/scalexi/dataset_generation/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    32752 2023-11-20 18:15:53.000000 scalexi-0.4.6.1/scalexi/dataset_generation/prompt_completion.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-25 09:48:57.214541 scalexi-0.4.6.1/scalexi/document_loaders/
--rw-r--r--   0 akoubaa    (501) staff       (20)        0 2023-11-15 19:31:52.000000 scalexi-0.4.6.1/scalexi/document_loaders/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     3944 2023-11-20 17:59:39.000000 scalexi-0.4.6.1/scalexi/document_loaders/context_loaders.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     2167 2024-05-23 19:27:41.000000 scalexi-0.4.6.1/scalexi/document_loaders/pdf_loaders.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-25 09:48:57.215272 scalexi-0.4.6.1/scalexi/llm/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.6.1/scalexi/llm/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     4214 2024-01-29 23:03:40.000000 scalexi-0.4.6.1/scalexi/llm/google_gemini.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     9996 2024-01-29 23:59:01.000000 scalexi-0.4.6.1/scalexi/llm/openai_gpt.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-25 09:48:57.215869 scalexi-0.4.6.1/scalexi/llm_evaluation/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.6.1/scalexi/llm_evaluation/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    36889 2023-11-22 13:28:34.000000 scalexi-0.4.6.1/scalexi/llm_evaluation/evaluate.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-25 09:48:57.217476 scalexi-0.4.6.1/scalexi/openai/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.6.1/scalexi/openai/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    29566 2023-11-23 15:04:13.000000 scalexi-0.4.6.1/scalexi/openai/fine_tuning_api.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    34682 2024-05-24 20:16:32.000000 scalexi-0.4.6.1/scalexi/openai/pricing.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-25 09:48:57.219367 scalexi-0.4.6.1/scalexi/utilities/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.6.1/scalexi/utilities/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     1040 2024-05-25 09:44:04.000000 scalexi-0.4.6.1/scalexi/utilities/api.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    38655 2024-01-29 19:28:25.000000 scalexi-0.4.6.1/scalexi/utilities/data_formatter.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     2728 2024-01-29 21:41:32.000000 scalexi-0.4.6.1/scalexi/utilities/logger.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    16806 2024-05-24 20:53:21.000000 scalexi-0.4.6.1/scalexi/utilities/text_processing.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-25 09:48:57.212705 scalexi-0.4.6.1/scalexi.egg-info/
--rw-r--r--   0 akoubaa    (501) staff       (20)     4525 2024-05-25 09:48:57.000000 scalexi-0.4.6.1/scalexi.egg-info/PKG-INFO
--rw-r--r--   0 akoubaa    (501) staff       (20)      894 2024-05-25 09:48:57.000000 scalexi-0.4.6.1/scalexi.egg-info/SOURCES.txt
--rw-r--r--   0 akoubaa    (501) staff       (20)        1 2024-05-25 09:48:57.000000 scalexi-0.4.6.1/scalexi.egg-info/dependency_links.txt
--rw-r--r--   0 akoubaa    (501) staff       (20)      130 2024-05-25 09:48:57.000000 scalexi-0.4.6.1/scalexi.egg-info/requires.txt
--rw-r--r--   0 akoubaa    (501) staff       (20)        8 2024-05-25 09:48:57.000000 scalexi-0.4.6.1/scalexi.egg-info/top_level.txt
--rw-r--r--   0 akoubaa    (501) staff       (20)       38 2024-05-25 09:48:57.220064 scalexi-0.4.6.1/setup.cfg
--rw-r--r--   0 akoubaa    (501) staff       (20)     5404 2024-05-25 09:48:49.000000 scalexi-0.4.6.1/setup.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-28 07:35:53.886297 scalexi-0.4.7.0/
+-rw-r--r--   0 akoubaa    (501) staff       (20)     2751 2023-11-18 18:27:29.000000 scalexi-0.4.7.0/LICENSE
+-rw-r--r--   0 akoubaa    (501) staff       (20)     4525 2024-05-28 07:35:53.886165 scalexi-0.4.7.0/PKG-INFO
+-rw-r--r--   0 akoubaa    (501) staff       (20)    15922 2023-11-22 16:53:27.000000 scalexi-0.4.7.0/README.md
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-28 07:35:53.870551 scalexi-0.4.7.0/scalexi/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.0/scalexi/__init__.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-28 07:35:53.872286 scalexi-0.4.7.0/scalexi/data/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.0/scalexi/data/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     4882 2024-05-27 15:01:35.000000 scalexi-0.4.7.0/scalexi/data/openai_pricing.json
+-rw-r--r--   0 akoubaa    (501) staff       (20)     3723 2024-03-11 15:00:18.000000 scalexi-0.4.7.0/scalexi/data/openai_pricing_v1.json
+-rw-r--r--   0 akoubaa    (501) staff       (20)     3517 2024-05-27 15:01:06.000000 scalexi-0.4.7.0/scalexi/data/openai_pricing_v2.json
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-28 07:35:53.872547 scalexi-0.4.7.0/scalexi/dataset_generation/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.0/scalexi/dataset_generation/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    32752 2023-11-20 18:15:53.000000 scalexi-0.4.7.0/scalexi/dataset_generation/prompt_completion.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-28 07:35:53.873353 scalexi-0.4.7.0/scalexi/document_loaders/
+-rw-r--r--   0 akoubaa    (501) staff       (20)        0 2023-11-15 19:31:52.000000 scalexi-0.4.7.0/scalexi/document_loaders/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     3944 2023-11-20 17:59:39.000000 scalexi-0.4.7.0/scalexi/document_loaders/context_loaders.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     2167 2024-05-23 19:27:41.000000 scalexi-0.4.7.0/scalexi/document_loaders/pdf_loaders.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-28 07:35:53.875768 scalexi-0.4.7.0/scalexi/llm/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.0/scalexi/llm/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     4214 2024-01-29 23:03:40.000000 scalexi-0.4.7.0/scalexi/llm/google_gemini.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     9996 2024-01-29 23:59:01.000000 scalexi-0.4.7.0/scalexi/llm/openai_gpt.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-28 07:35:53.876700 scalexi-0.4.7.0/scalexi/llm_evaluation/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.0/scalexi/llm_evaluation/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    36889 2023-11-22 13:28:34.000000 scalexi-0.4.7.0/scalexi/llm_evaluation/evaluate.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-28 07:35:53.883692 scalexi-0.4.7.0/scalexi/openai/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.0/scalexi/openai/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    29566 2023-11-23 15:04:13.000000 scalexi-0.4.7.0/scalexi/openai/fine_tuning_api.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    34682 2024-05-27 16:10:27.000000 scalexi-0.4.7.0/scalexi/openai/pricing.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    12977 2024-05-27 16:28:54.000000 scalexi-0.4.7.0/scalexi/openai/utilities.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-28 07:35:53.885874 scalexi-0.4.7.0/scalexi/utilities/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.0/scalexi/utilities/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     1040 2024-05-25 09:44:04.000000 scalexi-0.4.7.0/scalexi/utilities/api.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    38655 2024-01-29 19:28:25.000000 scalexi-0.4.7.0/scalexi/utilities/data_formatter.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     2728 2024-01-29 21:41:32.000000 scalexi-0.4.7.0/scalexi/utilities/logger.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    19552 2024-05-27 15:18:11.000000 scalexi-0.4.7.0/scalexi/utilities/text_processing.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-28 07:35:53.871391 scalexi-0.4.7.0/scalexi.egg-info/
+-rw-r--r--   0 akoubaa    (501) staff       (20)     4525 2024-05-28 07:35:53.000000 scalexi-0.4.7.0/scalexi.egg-info/PKG-INFO
+-rw-r--r--   0 akoubaa    (501) staff       (20)      958 2024-05-28 07:35:53.000000 scalexi-0.4.7.0/scalexi.egg-info/SOURCES.txt
+-rw-r--r--   0 akoubaa    (501) staff       (20)        1 2024-05-28 07:35:53.000000 scalexi-0.4.7.0/scalexi.egg-info/dependency_links.txt
+-rw-r--r--   0 akoubaa    (501) staff       (20)      130 2024-05-28 07:35:53.000000 scalexi-0.4.7.0/scalexi.egg-info/requires.txt
+-rw-r--r--   0 akoubaa    (501) staff       (20)        8 2024-05-28 07:35:53.000000 scalexi-0.4.7.0/scalexi.egg-info/top_level.txt
+-rw-r--r--   0 akoubaa    (501) staff       (20)       38 2024-05-28 07:35:53.886333 scalexi-0.4.7.0/setup.cfg
+-rw-r--r--   0 akoubaa    (501) staff       (20)     5404 2024-05-28 07:35:47.000000 scalexi-0.4.7.0/setup.py
```

### Comparing `scalexi-0.4.6.1/LICENSE` & `scalexi-0.4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.6.1/PKG-INFO` & `scalexi-0.4.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalexi
-Version: 0.4.6.1
+Version: 0.4.7.0
 Summary: The scalexi package is a versatile open-source Python library that focuses on facilitating low-code development and fine-tuning of diverse Large Language Models (LLMs). It extends beyond its initial OpenAI models integration, offering a scalable framework for various LLMs.
 Home-page: https://github.com/scalexi/scalexi
 Author: ScaleX Innovation
 Author-email: akoubaa@scalexi.ai
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `scalexi-0.4.6.1/README.md` & `scalexi-0.4.7.0/README.md`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.6.1/scalexi/data/openai_pricing.json` & `scalexi-0.4.7.0/scalexi/data/openai_pricing_v2.json`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.6.1/scalexi/data/openai_pricing_v1.json` & `scalexi-0.4.7.0/scalexi/data/openai_pricing_v1.json`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.6.1/scalexi/dataset_generation/prompt_completion.py` & `scalexi-0.4.7.0/scalexi/dataset_generation/prompt_completion.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.6.1/scalexi/document_loaders/context_loaders.py` & `scalexi-0.4.7.0/scalexi/document_loaders/context_loaders.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.6.1/scalexi/document_loaders/pdf_loaders.py` & `scalexi-0.4.7.0/scalexi/document_loaders/pdf_loaders.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.6.1/scalexi/llm/google_gemini.py` & `scalexi-0.4.7.0/scalexi/llm/google_gemini.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.6.1/scalexi/llm/openai_gpt.py` & `scalexi-0.4.7.0/scalexi/llm/openai_gpt.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.6.1/scalexi/llm_evaluation/evaluate.py` & `scalexi-0.4.7.0/scalexi/llm_evaluation/evaluate.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.6.1/scalexi/openai/fine_tuning_api.py` & `scalexi-0.4.7.0/scalexi/openai/fine_tuning_api.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.6.1/scalexi/openai/pricing.py` & `scalexi-0.4.7.0/scalexi/openai/pricing.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.6.1/scalexi/utilities/api.py` & `scalexi-0.4.7.0/scalexi/utilities/api.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.6.1/scalexi/utilities/data_formatter.py` & `scalexi-0.4.7.0/scalexi/utilities/data_formatter.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.6.1/scalexi/utilities/logger.py` & `scalexi-0.4.7.0/scalexi/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.6.1/scalexi/utilities/text_processing.py` & `scalexi-0.4.7.0/scalexi/utilities/text_processing.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,25 +21,14 @@
 logger = Logger().get_logger()
 
 data = pkgutil.get_data('scalexi', 'data/openai_pricing.json')
 pricing_info = json.loads(data)
 #print(dfm.json_to_yaml(pricing_info))
 pricing = OpenAIPricing(pricing_info)
 
-
-
-
-# Create a logger file
-logger = Logger().get_logger()
-
-data = pkgutil.get_data('scalexi', 'data/openai_pricing.json')
-pricing_info = json.loads(data)
-#print(dfm.json_to_yaml(pricing_info))
-pricing = OpenAIPricing(pricing_info)
-
 def remove_latex_constructs(context: str) -> str:
     # Remove LaTeX comment lines
     context = re.sub(r'%.*', '', context)
     
     # Replace LaTeX citation commands with [Citation]
     context = re.sub(r'~\\cite\{.*?\}', '[Citation]', context)
 
@@ -371,15 +360,15 @@
         
         logger.info(f'[SCALEXI-classify_text] returning response, pricing, token_usage, execution_time')
         return final_result
     except Exception as e:
         logger.error(f"Error during text classification: {str(e)}")
         return json.dumps({"error": str(e)})
 
-def get_text_statistics(pdf_path, model_name="gpt-4"):
+def get_text_statistics_basic(pdf_path, model_name="gpt-4"):
     """
     Provides descriptive statistics about the extracted text from a PDF.
 
     :param pdf_path: The path to the PDF file to analyze.
     :param model_name: The name of the model to use for token calculation.
 
     :return: A dictionary containing descriptive statistics about the text.
@@ -424,8 +413,97 @@
         "num_sentences": num_sentences,
         "most_common_words": str(most_common_words),
         "num_tokens": num_tokens,
         "num_pages": num_pages,
         "words_per_page": str(words_per_page)
     }
     
-    return stats
+    return stats
+
+
+def get_openai_pricing():
+    """
+    Returns the pricing information for OpenAI models.
+
+    :return: A dictionary containing the pricing information for OpenAI models.
+    """
+    data = pkgutil.get_data('scalexi', 'data/openai_pricing.json')
+    pricing_info = json.loads(data)
+    pricing = OpenAIPricing(pricing_info)
+    return pricing
+  
+def get_openai_pricing_info():
+    """
+    Returns the pricing information for OpenAI models.
+
+    :return: A dictionary containing the pricing information for OpenAI models.
+    """
+    data = pkgutil.get_data('scalexi', 'data/openai_pricing.json')
+    pricing_info = json.loads(data)
+    return pricing_info
+  
+
+def get_text_statistics(pdf_path, model_name="gpt-4"):
+        """
+        Provides descriptive statistics about the extracted text from a PDF.
+
+        :param pdf_path: The path to the PDF file to analyze.
+        :param model_name: The name of the model to use for token calculation.
+
+        :return: A dictionary containing descriptive statistics about the text.
+        """
+        # Initialize variables for collecting text and word counts per page
+        all_text = ""
+        words_per_page = []
+        num_pages = 0
+
+        with pdfplumber.open(pdf_path) as pdf:
+            num_pages = len(pdf.pages)
+            for page in pdf.pages:
+                page_text = page.extract_text()
+                all_text += page_text
+                
+                # Count words per page
+                words = re.findall(r'\w+', page_text)
+                words_per_page.append(len(words))
+
+        # Number of characters
+        num_chars = len(all_text)
+        
+        # Number of words
+        words = re.findall(r'\w+', all_text)
+        num_words = len(words)
+        
+        # Number of sentences
+        sentences = re.split(r'[.!?]+', all_text)
+        num_sentences = len(sentences) - 1  # Adjust for possible trailing empty string
+        
+        # Most common words
+        word_freq = Counter(words)
+        most_common_words = word_freq.most_common(10)
+        print('most_common_words:', most_common_words)
+        # Token count
+        num_tokens = pricing.calculate_token_usage_for_text(all_text, model_name)
+        
+        # Get file size in bytes
+        try:
+            file_size = os.path.getsize(pdf_path)
+        except Exception as e:
+            logger.error(f"An error occurred while getting file size: {e}")
+            stats["file_size"] = None
+        
+        # Generate statistics dictionary
+        stats = {
+            "num_chars": num_chars,
+            "num_words": num_words,
+            "num_sentences": num_sentences,
+            "most_common_words": str(most_common_words),
+            "num_tokens": num_tokens,
+            "num_pages": num_pages,
+            "words_per_page": str(words_per_page),
+            "file_size": file_size,
+            "file_path": pdf_path,
+            "model_name": model_name
+        }   
+        
+        
+        return stats
```

### Comparing `scalexi-0.4.6.1/scalexi.egg-info/PKG-INFO` & `scalexi-0.4.7.0/scalexi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalexi
-Version: 0.4.6.1
+Version: 0.4.7.0
 Summary: The scalexi package is a versatile open-source Python library that focuses on facilitating low-code development and fine-tuning of diverse Large Language Models (LLMs). It extends beyond its initial OpenAI models integration, offering a scalable framework for various LLMs.
 Home-page: https://github.com/scalexi/scalexi
 Author: ScaleX Innovation
 Author-email: akoubaa@scalexi.ai
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `scalexi-0.4.6.1/scalexi.egg-info/SOURCES.txt` & `scalexi-0.4.7.0/scalexi.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 scalexi.egg-info/SOURCES.txt
 scalexi.egg-info/dependency_links.txt
 scalexi.egg-info/requires.txt
 scalexi.egg-info/top_level.txt
 scalexi/data/__init__.py
 scalexi/data/openai_pricing.json
 scalexi/data/openai_pricing_v1.json
+scalexi/data/openai_pricing_v2.json
 scalexi/dataset_generation/__init__.py
 scalexi/dataset_generation/prompt_completion.py
 scalexi/document_loaders/__init__.py
 scalexi/document_loaders/context_loaders.py
 scalexi/document_loaders/pdf_loaders.py
 scalexi/llm/__init__.py
 scalexi/llm/google_gemini.py
 scalexi/llm/openai_gpt.py
 scalexi/llm_evaluation/__init__.py
 scalexi/llm_evaluation/evaluate.py
 scalexi/openai/__init__.py
 scalexi/openai/fine_tuning_api.py
 scalexi/openai/pricing.py
+scalexi/openai/utilities.py
 scalexi/utilities/__init__.py
 scalexi/utilities/api.py
 scalexi/utilities/data_formatter.py
 scalexi/utilities/logger.py
 scalexi/utilities/text_processing.py
```

### Comparing `scalexi-0.4.6.1/setup.py` & `scalexi-0.4.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="scalexi",
-    version="0.4.6.1",
+    version="0.4.7.0",
     packages=find_packages(),
     include_package_data=True,
     package_data={'scalexi': ['data/*']},
     install_requires=[
         "pandas",  # Add any package dependencies here
         "openai>=1.10.0", #this package is not compatible with earlier versions of openai
         "sphinx",   # Add any other dependencies as needed
```

