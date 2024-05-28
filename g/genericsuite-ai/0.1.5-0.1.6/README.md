# Comparing `tmp/genericsuite_ai-0.1.5.tar.gz` & `tmp/genericsuite_ai-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genericsuite_ai-0.1.5.tar", max compression
+gzip compressed data, was "genericsuite_ai-0.1.6.tar", max compression
```

## Comparing `genericsuite_ai-0.1.5.tar` & `genericsuite_ai-0.1.6.tar`

### file list

```diff
@@ -1,40 +1,42 @@
--rw-r--r--   0        0        0      747 2024-03-31 23:36:18.812667 genericsuite_ai-0.1.5/LICENSE
--rw-r--r--   0        0        0    11807 2024-04-19 09:16:32.145792 genericsuite_ai-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-03-03 23:59:15.113581 genericsuite_ai-0.1.5/genericsuite_ai/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 13:12:24.883757 genericsuite_ai-0.1.5/genericsuite_ai/chalicelib/endpoints/__init__.py
--rw-r--r--   0        0        0     2551 2024-02-29 10:54:59.765849 genericsuite_ai-0.1.5/genericsuite_ai/chalicelib/endpoints/ai_chatbot_endpoint.py
--rw-r--r--   0        0        0        0 2024-03-03 12:55:02.975460 genericsuite_ai-0.1.5/genericsuite_ai/chalicelib/util/__init__.py
--rw-r--r--   0        0        0      676 2024-03-03 13:05:09.210706 genericsuite_ai-0.1.5/genericsuite_ai/chalicelib/util/create_app.py
--rw-r--r--   0        0        0        0 2024-02-26 12:41:31.668394 genericsuite_ai-0.1.5/genericsuite_ai/config/__init__.py
--rw-r--r--   0        0        0    13917 2024-03-02 15:15:40.872623 genericsuite_ai-0.1.5/genericsuite_ai/config/config.py
--rw-r--r--   0        0        0        0 2023-07-28 18:42:59.199879 genericsuite_ai-0.1.5/genericsuite_ai/lib/__init__.py
--rw-r--r--   0        0        0    22004 2024-03-03 02:48:34.133168 genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_audio_processing.py
--rw-r--r--   0        0        0     9346 2024-02-29 10:54:59.738325 genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_chatbot_commons.py
--rw-r--r--   0        0        0    11016 2024-02-29 10:54:59.763617 genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_chatbot_endpoint.py
--rw-r--r--   0        0        0    17788 2024-03-03 15:37:39.063166 genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_chatbot_main_langchain.py
--rw-r--r--   0        0        0    18309 2024-03-03 02:47:59.470955 genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_chatbot_main_langchain_OLD.py
--rw-r--r--   0        0        0     5022 2024-03-03 02:47:59.470981 genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_chatbot_main_openai.py
--rw-r--r--   0        0        0    11019 2024-02-29 11:11:26.462600 genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_conversations.py
--rw-r--r--   0        0        0     4994 2024-02-29 10:54:59.759569 genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_embeddings.py
--rw-r--r--   0        0        0     3783 2024-02-29 12:27:31.428912 genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_gpt_fn_conversations.py
--rw-r--r--   0        0        0    16283 2024-03-02 17:40:43.234533 genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_gpt_functions.py
--rw-r--r--   0        0        0    15750 2024-03-03 02:47:59.470989 genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_image_generator.py
--rw-r--r--   0        0        0    13375 2024-03-03 15:55:15.380883 genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_langchain_models.py
--rw-r--r--   0        0        0     7222 2024-03-02 15:58:44.288898 genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_langchain_tools.py
--rw-r--r--   0        0        0     3171 2024-02-29 10:54:59.764343 genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_sub_bots.py
--rw-r--r--   0        0        0     7475 2024-03-02 15:00:32.355696 genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_utilities.py
--rw-r--r--   0        0        0    14434 2024-03-03 02:47:59.470968 genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_vision.py
--rw-r--r--   0        0        0    32697 2024-02-28 13:38:30.271183 genericsuite_ai-0.1.5/genericsuite_ai/lib/clarifai.py
--rw-r--r--   0        0        0     5487 2024-02-25 11:54:38.786458 genericsuite_ai-0.1.5/genericsuite_ai/lib/git_reader.py
--rw-r--r--   0        0        0     5723 2024-02-29 13:08:21.289363 genericsuite_ai-0.1.5/genericsuite_ai/lib/json_reader.py
--rw-r--r--   0        0        0     1076 2024-02-29 12:42:27.485181 genericsuite_ai-0.1.5/genericsuite_ai/lib/pdf_reader.py
--rw-r--r--   0        0        0     4112 2024-02-23 00:45:13.048529 genericsuite_ai-0.1.5/genericsuite_ai/lib/translator.py
--rw-r--r--   0        0        0    12133 2024-03-02 18:51:08.649645 genericsuite_ai-0.1.5/genericsuite_ai/lib/vector_index.py
--rw-r--r--   0        0        0     7779 2024-03-03 02:46:02.072630 genericsuite_ai-0.1.5/genericsuite_ai/lib/web_scraping.py
--rw-r--r--   0        0        0     6600 2024-02-29 10:54:59.759814 genericsuite_ai-0.1.5/genericsuite_ai/lib/web_search.py
--rw-r--r--   0        0        0      844 2024-02-29 12:42:39.130214 genericsuite_ai-0.1.5/genericsuite_ai/lib/youtube_reader.py
--rw-r--r--   0        0        0        0 2024-02-24 04:05:41.201010 genericsuite_ai-0.1.5/genericsuite_ai/models/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 01:53:51.743753 genericsuite_ai-0.1.5/genericsuite_ai/models/billing/__init__.py
--rw-r--r--   0        0        0     1687 2024-03-14 13:37:54.631329 genericsuite_ai-0.1.5/genericsuite_ai/models/billing/billing_utilities.py
--rw-r--r--   0        0        0     1816 2024-04-21 00:22:25.277898 genericsuite_ai-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    13500 1970-01-01 00:00:00.000000 genericsuite_ai-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      747 2024-03-31 23:36:18.812667 genericsuite_ai-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1691 2024-05-05 12:09:46.885898 genericsuite_ai-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-03-03 23:59:15.113581 genericsuite_ai-0.1.6/genericsuite_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 13:12:24.883757 genericsuite_ai-0.1.6/genericsuite_ai/chalicelib/endpoints/__init__.py
+-rw-r--r--   0        0        0     2697 2024-05-16 00:31:55.506670 genericsuite_ai-0.1.6/genericsuite_ai/chalicelib/endpoints/ai_chatbot_endpoint.py
+-rw-r--r--   0        0        0     2550 2024-05-17 12:36:12.417582 genericsuite_ai-0.1.6/genericsuite_ai/chalicelib/endpoints/ai_conversations_conversion.py
+-rw-r--r--   0        0        0        0 2024-03-03 12:55:02.975460 genericsuite_ai-0.1.6/genericsuite_ai/chalicelib/util/__init__.py
+-rw-r--r--   0        0        0      676 2024-03-03 13:05:09.210706 genericsuite_ai-0.1.6/genericsuite_ai/chalicelib/util/create_app.py
+-rw-r--r--   0        0        0        0 2024-02-26 12:41:31.668394 genericsuite_ai-0.1.6/genericsuite_ai/config/__init__.py
+-rw-r--r--   0        0        0    14407 2024-05-26 19:21:59.985160 genericsuite_ai-0.1.6/genericsuite_ai/config/config.py
+-rw-r--r--   0        0        0        0 2023-07-28 18:42:59.199879 genericsuite_ai-0.1.6/genericsuite_ai/lib/__init__.py
+-rw-r--r--   0        0        0    22279 2024-05-10 02:39:58.407434 genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_audio_processing.py
+-rw-r--r--   0        0        0     9347 2024-05-25 17:59:03.375972 genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_chatbot_commons.py
+-rw-r--r--   0        0        0    11304 2024-05-16 01:51:45.549956 genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_chatbot_endpoint.py
+-rw-r--r--   0        0        0    27089 2024-05-26 18:28:51.586398 genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_chatbot_main_langchain.py
+-rw-r--r--   0        0        0    18330 2024-05-25 18:02:31.851163 genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_chatbot_main_langchain_ca.py
+-rw-r--r--   0        0        0     5022 2024-03-03 02:47:59.470981 genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_chatbot_main_openai.py
+-rw-r--r--   0        0        0    11019 2024-05-13 11:25:32.079615 genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_conversations.py
+-rw-r--r--   0        0        0     5952 2024-05-13 22:25:51.206253 genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_conversations_conversion.py
+-rw-r--r--   0        0        0     5083 2024-05-14 01:28:34.679370 genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_embeddings.py
+-rw-r--r--   0        0        0     3783 2024-02-29 12:27:31.428912 genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_gpt_fn_conversations.py
+-rw-r--r--   0        0        0    16282 2024-05-25 20:07:47.589607 genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_gpt_functions.py
+-rw-r--r--   0        0        0    16370 2024-05-09 01:25:41.139567 genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_image_generator.py
+-rw-r--r--   0        0        0    13221 2024-05-14 01:33:57.061514 genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_langchain_models.py
+-rw-r--r--   0        0        0     7440 2024-05-26 00:12:53.700434 genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_langchain_tools.py
+-rw-r--r--   0        0        0     3171 2024-02-29 10:54:59.764343 genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_sub_bots.py
+-rw-r--r--   0        0        0     7475 2024-03-02 15:00:32.355696 genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_utilities.py
+-rw-r--r--   0        0        0    16180 2024-05-25 20:07:53.042916 genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_vision.py
+-rw-r--r--   0        0        0    32728 2024-05-09 01:13:48.664679 genericsuite_ai-0.1.6/genericsuite_ai/lib/clarifai.py
+-rw-r--r--   0        0        0     5487 2024-02-25 11:54:38.786458 genericsuite_ai-0.1.6/genericsuite_ai/lib/git_reader.py
+-rw-r--r--   0        0        0     5723 2024-02-29 13:08:21.289363 genericsuite_ai-0.1.6/genericsuite_ai/lib/json_reader.py
+-rw-r--r--   0        0        0     1076 2024-02-29 12:42:27.485181 genericsuite_ai-0.1.6/genericsuite_ai/lib/pdf_reader.py
+-rw-r--r--   0        0        0     4112 2024-02-23 00:45:13.048529 genericsuite_ai-0.1.6/genericsuite_ai/lib/translator.py
+-rw-r--r--   0        0        0    12141 2024-05-14 01:34:31.950452 genericsuite_ai-0.1.6/genericsuite_ai/lib/vector_index.py
+-rw-r--r--   0        0        0     7788 2024-05-25 20:08:30.217909 genericsuite_ai-0.1.6/genericsuite_ai/lib/web_scraping.py
+-rw-r--r--   0        0        0     9013 2024-05-26 18:50:01.076753 genericsuite_ai-0.1.6/genericsuite_ai/lib/web_search.py
+-rw-r--r--   0        0        0      844 2024-02-29 12:42:39.130214 genericsuite_ai-0.1.6/genericsuite_ai/lib/youtube_reader.py
+-rw-r--r--   0        0        0        0 2024-02-24 04:05:41.201010 genericsuite_ai-0.1.6/genericsuite_ai/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 01:53:51.743753 genericsuite_ai-0.1.6/genericsuite_ai/models/billing/__init__.py
+-rw-r--r--   0        0        0     1687 2024-03-14 13:37:54.631329 genericsuite_ai-0.1.6/genericsuite_ai/models/billing/billing_utilities.py
+-rw-r--r--   0        0        0     1823 2024-05-26 00:05:18.779658 genericsuite_ai-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 genericsuite_ai-0.1.6/PKG-INFO
```

### Comparing `genericsuite_ai-0.1.5/LICENSE` & `genericsuite_ai-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/chalicelib/endpoints/ai_chatbot_endpoint.py` & `genericsuite_ai-0.1.6/genericsuite_ai/chalicelib/endpoints/ai_chatbot_endpoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 AI Endpoints
 """
 from typing import Optional
 
 # from chalice.app import Response
-from genericsuite.util.framework_abs_layer import Response
 
-from genericsuite.util.blueprint_one import BlueprintOne
+# from genericsuite.util.blueprint_one import BlueprintOne
+from genericsuite.util.framework_abs_layer import Response, BlueprintOne
+
 from genericsuite.util.jwt import (
     request_authentication,
     AuthorizedRequest
 )
 from genericsuite_ai.lib.ai_chatbot_endpoint import (
     ai_chatbot_endpoint as ai_chatbot_endpoint_model,
     vision_image_analyzer_endpoint as vision_image_analyzer_endpoint_model,
@@ -37,15 +38,16 @@
     conversation with the AI chatbot.
     It then returns the AI chatbot's response.
 
     :param request: The request from the user.
     :param other_params: Other parameters that may be needed.
     :return: The response from the AI chatbot.
     """
-    return ai_chatbot_endpoint_model(request, other_params)
+    return ai_chatbot_endpoint_model(request=request, blueprint=bp,
+        other_params=other_params)
 
 
 @bp.route(
     '/image_to_text',
     methods=['POST'],
     authorizor=request_authentication(),
     content_types=['multipart/form-data']
@@ -58,15 +60,16 @@
     This endpoint receives an image file, saves it to a temporary directory
     with a uuid4 .jpg | .png filename, calls @vision_image_analyzer with
     the file path, and returns the result.
 
     :param request: The request containing the image file.
     :return: The text with the image analysis.
     """
-    return vision_image_analyzer_endpoint_model(request, other_params)
+    return vision_image_analyzer_endpoint_model(request=request, blueprint=bp,
+        other_params=other_params)
 
 
 @bp.route(
     '/voice_to_text',
     methods=['POST'],
     authorizor=request_authentication(),
     content_types=['multipart/form-data']
@@ -79,8 +82,9 @@
     This endpoint receives an audio file, saves it to a temporary directory
     with a uuid4 .mp3 filename, calls @audio_to_text_transcript with
     the file path, and returns the result.
 
     :param request: The request containing the audio file.
     :return: The transcription result.
     """
-    return transcribe_audio_endpoint_model(request, other_params)
+    return transcribe_audio_endpoint_model(request=request, blueprint=bp,
+        other_params=other_params)
```

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/chalicelib/util/create_app.py` & `genericsuite_ai-0.1.6/genericsuite_ai/chalicelib/util/create_app.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/config/config.py` & `genericsuite_ai-0.1.6/genericsuite_ai/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,21 @@
         )
 
         self.AI_ADDITIONAL_MODELS = self.get_env(
             # 'AI_ADDITIONAL_MODELS', '1'   # Add aditional models to the LLM
             'AI_ADDITIONAL_MODELS', '0'
         )
 
+        self.WEBSEARCH_DEFAULT_PROVIDER = self.get_env(
+            'WEBSEARCH_DEFAULT_PROVIDER', ''    # First try with DDG, if error, try Google
+            # 'WEBSEARCH_DEFAULT_PROVIDER', 'ddg'   # DuckDuckGo
+            # 'WEBSEARCH_DEFAULT_PROVIDER', 'google'   # Google
+        )
+
+
         """
         --------------------------------
         AI general configuration - END
         """
 
         # Langchain credentials and other parameters
 
@@ -107,20 +114,26 @@
         self.LANGCHAIN_TRACING_V2 = self.get_env(
             'LANGCHAIN_TRACING_V2', 'true'
         )
 
         # Agent configuration
 
         self.LANGCHAIN_AGENT_TYPE = self.get_env(
-            'LANGCHAIN_AGENT_TYPE', "react_chat_agent"
+            'LANGCHAIN_AGENT_TYPE', "lcel"
+            # 'LANGCHAIN_AGENT_TYPE', "react_chat_agent"
             # 'LANGCHAIN_AGENT_TYPE', "react_agent"
             # 'LANGCHAIN_AGENT_TYPE', "structured_chat_agent"
             # 'LANGCHAIN_AGENT_TYPE', "LLMSingleActionAgent"
         )
 
+        self.LANGCHAIN_MAX_CONV_MESSAGES = self.get_env(
+            'LANGCHAIN_MAX_CONV_MESSAGES', '30'     # Default: preserve all
+            # 'LANGCHAIN_MAX_CONV_MESSAGES', '-1'     # Default: preserve all
+        )
+
         self.LANGCHAIN_MAX_ITERATIONS = self.get_env(
             'LANGCHAIN_MAX_ITERATIONS', '8'     # Default: 15
         )
         self.LANGCHAIN_EARLY_STOPPING_METHOD = self.get_env(
             'LANGCHAIN_EARLY_STOPPING_METHOD', 'force'
             # 'LANGCHAIN_EARLY_STOPPING_METHOD', 'generate'
         )
@@ -156,21 +169,24 @@
 
         self.OPENAI_API_KEY = self.get_env('OPENAI_API_KEY', '')
 
         self.OPENAI_MODEL = self.get_env(
             'OPENAI_MODEL', 'gpt-3.5-turbo'
         )
         self.OPENAI_MODEL_PREMIUM = self.get_env(
-            'OPENAI_MODEL_PREMIUM', 'gpt-4-turbo-preview'   # TODO implement this param
+            'OPENAI_MODEL_PREMIUM', 'gpt-4o'
+            # 'OPENAI_MODEL_PREMIUM', 'gpt-4-turbo'
         )
         self.OPENAI_MODEL_INSTRUCT = self.get_env(
             'OPENAI_MODEL_INSTRUCT', 'gpt-3.5-turbo-instruct'
         )
         self.OPENAI_VISION_MODEL = self.get_env(
-            'OPENAI_VISION_MODEL', 'gpt-4-vision-preview'
+            'OPENAI_VISION_MODEL', 'gpt-4o'
+            # 'OPENAI_VISION_MODEL', 'gpt-4-turbo'
+            # 'OPENAI_VISION_MODEL', 'gpt-4-vision-preview'
         )
         self.OPENAI_IMAGE_GEN_MODEL = self.get_env(
             'OPENAI_IMAGE_GEN_MODEL', 'dall-e-3'
         )
         self.OPENAI_VOICE_MODEL = self.get_env(
             'OPENAI_VOICE_MODEL', 'whisper-1'
         )
@@ -178,29 +194,27 @@
             'OPENAI_TEXT_TO_AUDIO_MODEL', 'tts-1'
         )
         self.OPENAI_TEXT_TO_AUDIO_VOICE = self.get_env(
             'OPENAI_TEXT_TO_AUDIO_VOICE', 'onyx'
             # 'OPENAI_TEXT_TO_AUDIO_VOICE', 'alloy' | 'echo', 'fable', 'onyx', 'nova', 'shimmer'
         )
         self.OPENAI_EMBEDDINGS_MODEL = self.get_env(
-            # # TODO: 2024-02-11 | Warning: model not found. Using cl100k_base encoding.
-            # In: GVI2_3) GET_VECTOR_INDEX | get Vectorstore from a list of documents...
-            # 'OPENAI_EMBEDDINGS_MODEL', 'text-embedding-3-small'
-            'OPENAI_EMBEDDINGS_MODEL', 'text-embedding-ada-002'
+            'OPENAI_EMBEDDINGS_MODEL', 'text-embedding-3-small'
+            # 'OPENAI_EMBEDDINGS_MODEL', 'text-embedding-ada-002'
         )
         self.OPENAI_EMBEDDINGS_MODEL_PREMIUM = self.get_env(
             'OPENAI_EMBEDDINGS_MODEL_PREMIUM', 'text-embedding-3-large'   # TODO implement this param
         )
 
         self.OPENAI_TEMPERATURE = self.get_env('OPENAI_TEMPERATURE', '0.7')
         self.OPENAI_MAX_TOKENS = self.get_env('OPENAI_MAX_TOKENS', '500')
 
         # Anthropic credentials and other parameters
 
-        self.ANTHROPIC_MODEL = self.get_env('ANTHROPIC_MODEL', 'claude-2')
+        self.ANTHROPIC_MODEL = self.get_env('ANTHROPIC_MODEL', 'claude-3-sonnet')
         self.ANTHROPIC_API_KEY = self.get_env('ANTHROPIC_API_KEY', '')
 
         # AWS credentials and other parameters
 
         self.AWS_REGION = self.get_env('AWS_REGION', 'us-east-1')
         self.AWS_S3_CHATBOT_ATTACHMENTS_BUCKET = \
             self.get_env('AWS_S3_CHATBOT_ATTACHMENTS_BUCKET')
```

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_audio_processing.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_audio_processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """AI Audio Library"""
-from typing import Any, Optional
+from typing import Any, Optional, Dict
 import os
 from uuid import uuid4
 
 import urllib.request
 import urllib.parse
 
 from openai import OpenAI
@@ -132,31 +132,34 @@
         if DEBUG:
             log_debug('process_audio_url | ' +
                       f'AWS_S3_CHATBOT_ATTACHMENTS_BUCKET: {str(bucket_name)}')
         if not bucket_name:
             resultset["error"] = True
             resultset["error_message"] = "AWS_S3_CHATBOT_ATTACHMENTS_BUCKET is not configured [1]"
         else:
-            public_url, final_filename, error = upload_nodup_file_to_s3(
+            upload_result = upload_nodup_file_to_s3(
                 file_path=sound_filespec,
                 original_filename=os.path.basename(sound_filespec),
                 bucket_name=bucket_name,
                 sub_dir=user_id,
             )
-            if error:
+            if upload_result['error']:
                 resultset["error"] = True
-                resultset["error_message"] = error
+                resultset["error_message"] = upload_result["error_message"]
             else:
-                params[url_par_name] = public_url
+                params[url_par_name] = upload_result['public_url']
                 resultset = call_to(**params)
                 if rm_after_proc:
-                    remove_from_s3(
+                    remove_result = remove_from_s3(
                         bucket_name=bucket_name,
-                        key=f"{user_id}/{final_filename}",
+                        key=f"{user_id}/{upload_result['final_filename']}",
                     )
+                    if remove_result['error']:
+                        resultset["error"] = True
+                        resultset["error_message"] = remove_result["error_message"]
     return resultset
 
 
 def get_att_name() -> str:
     """ Returns the Audio-to-text configured technology name """
     settings = Config(cac.get())
     if settings.AI_AUDIO_TO_TEXT_TECHNOLOGY == "clarifai":
@@ -190,15 +193,15 @@
     """
     settings = Config(cac.get())
     billing = BillingUtilities(cac.get())
     log_debug("get_att_response | AI_AUDIO_TO_TEXT_TECHNOLOGY:" +
               f" {settings.AI_AUDIO_TO_TEXT_TECHNOLOGY}")
     try:
         if settings.AI_AUDIO_TO_TEXT_TECHNOLOGY == "clarifai":
-            audio_proc_par = {}
+            audio_proc_par: Dict[str, Any] = {}
             transcript = process_audio_url(
                 sound_filespec=sound_filespec,
                 call_to=clarifai_audio_to_text,
                 params=audio_proc_par,
                 url_par_name="audio_url",
                 rm_after_proc=True,
             )
```

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_chatbot_commons.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_chatbot_commons.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     get_response_lang,
     get_assistant_you_are,
 )
 from genericsuite_ai.lib.ai_gpt_fn_conversations import (
     get_current_date_time
 )
 
-DEBUG = False
+DEBUG = True
 
 
 def get_role(v):
     """
     Returns the role from the conversation item and show debug
     """
     if DEBUG:
@@ -149,15 +149,15 @@
     request = app_context.get_request()
     query_params = get_request_body(request)
     conv_response = get_default_resultset()
 
     # conversation is a json string comes from the frontend
     # must be converted with json to a list of strings
     # before sending to the endpoint
-    if 'conversation' not in query_params:
+    if not query_params.get('conversation'):
         conv_response["error"] = True
         conv_response["error_message"] = "No conversation provided" + \
                                          f" [AICC-E010] Stack: {lld['code']}"
         return report_error(conv_response)
 
     if DEBUG:
         log_debug(f"{lld['code']}-1) RUN_CONVERSATION_{lld['name']}" +
```

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_chatbot_endpoint.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_chatbot_endpoint.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 AI Endpoints
 """
 from typing import Optional
 
 # from chalice.app import Response
-from genericsuite.util.framework_abs_layer import Response
+from genericsuite.util.framework_abs_layer import Response, BlueprintOne
 
 from genericsuite.util.app_logger import log_debug
 from genericsuite.util.jwt import AuthorizedRequest
 from genericsuite.util.parse_multipart import file_upload_handler
 from genericsuite.util.utilities import (
     return_resultset_jsonified_or_exception,
     get_default_resultset,
@@ -43,14 +43,15 @@
 from genericsuite_ai.models.billing.billing_utilities import BillingUtilities
 
 DEBUG = False
 
 
 def ai_chatbot_endpoint(
     request: AuthorizedRequest,
+    blueprint: BlueprintOne,
     other_params: Optional[dict] = None,
     additional_callable: Optional[callable] = None,
 ) -> Response:
     """
     This function is the endpoint for the AI chatbot.
     It takes in a request and other parameters,
     logs the request, retrieves the user data, and runs the
@@ -59,21 +60,20 @@
 
     :param request: The request from the user.
     :param other_params: Other parameters that may be needed.
     :return: The response from the AI chatbot.
     """
     if DEBUG:
         log_debug(f'AICBEP-1) AI_CHATBOT - request: {request.to_dict()}')
-        # log_debug(f'3) bp.current_app.api.binary_types: {bp.get_current_app().api.binary_types}')
 
     if other_params is None:
         other_params = {}
 
     # Set environment variables from the database configurations.
-    app_context = app_context_and_set_env(request)
+    app_context = app_context_and_set_env(request=request, blueprint=blueprint)
     if app_context.has_error():
         return return_resultset_jsonified_or_exception(
             app_context.get_error_resultset()
         )
     if additional_callable:
         additional_callable(app_context)
 
@@ -144,28 +144,30 @@
     return return_resultset_jsonified_or_exception(
         ai_chatbot_response
     )
 
 
 def vision_image_analyzer_endpoint(
     request: AuthorizedRequest,
+    blueprint: BlueprintOne,
     other_params: Optional[dict] = None,
     additional_callable: Optional[callable] = None,
+    uploaded_file_path: Optional[str] = None,
 ) -> Response:
     """
     This endpoint receives an image file, saves it to a temporary directory
     with a uuid4 .jpg | .png filename, calls @vision_image_analyzer with
     the file path, and returns the result.
 
     :param request: The request containing the image file.
     :return: The text with the image analysis.
     """
 
     # Set environment variables from the database configurations.
-    app_context = app_context_and_set_env(request)
+    app_context = app_context_and_set_env(request=request, blueprint=blueprint)
     if app_context.has_error():
         return return_resultset_jsonified_or_exception(
             app_context.get_error_resultset()
         )
     if additional_callable:
         additional_callable(app_context)
 
@@ -219,14 +221,15 @@
 
     cac_vision.set(app_context)
     cac_clarifai.set(app_context)
 
     return file_upload_handler(
         app_context=app_context,
         p={
+            "uploaded_file_path": uploaded_file_path,
             "extension": get_file_extension(query_params["file_name"]),
             "handler_function": vision_image_analyzer,
             "unique_param_name": "params",
             "file_path_param_name": "image_path",
             "other_params": {
                 "params": {
                     "question": query_params["question"],
@@ -238,28 +241,30 @@
             }
         },
     )
 
 
 def transcribe_audio_endpoint(
     request: AuthorizedRequest,
+    blueprint: BlueprintOne,
     other_params: Optional[dict] = None,
     additional_callable: Optional[callable] = None,
+    uploaded_file_path: Optional[str] = None,
 ) -> Response:
     """
     This endpoint receives an audio file, saves it to a temporary directory
     with a uuid4 .mp3 filename, calls @audio_to_text_transcript with
     the file path, and returns the result.
 
     :param request: The request containing the audio file.
     :return: The transcription result.
     """
 
     # Set environment variables from the database configurations.
-    app_context = app_context_and_set_env(request)
+    app_context = app_context_and_set_env(request=request, blueprint=blueprint)
     if app_context.has_error():
         return return_resultset_jsonified_or_exception(
             app_context.get_error_resultset()
         )
     if additional_callable:
         additional_callable(app_context)
 
@@ -305,14 +310,15 @@
     if source_lang == "get_user_lang":
         source_lang = get_user_lang_code(app_context)
     other_options = query_params.get("other", '')
 
     return file_upload_handler(
         app_context=app_context,
         p={
+            "uploaded_file_path": uploaded_file_path,
             "extension": file_extension,
             "handler_function": audio_to_text_transcript,
             "unique_param_name": "params",
             "file_path_param_name": "sound_filespec",
             # "delete_file_after_processing": False,
             "other_params": {
                 "params": {
```

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_chatbot_main_langchain.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_chatbot_main_langchain.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 """
-Implementation of the AI Chatbot API using Langchain.
+Implementation of the AI Chatbot API using Langchain - LCEL or Agents.
 """
-from typing import Any, Union
+from typing import Any, Union, Dict, Tuple
 import os
 
 from langchain import hub
 from langchain.agents import (
     AgentExecutor,
     create_structured_chat_agent,
     create_react_agent,
     # create_openai_functions_agent,
     # create_openai_tools_agent,
     # create_self_ask_with_search_agent,
 )
 from langchain.prompts import PromptTemplate
+# from langchain_community.chat_message_histories import ChatMessageHistory
+# from langchain_core.output_parsers.openai_tools import PydanticToolsParser
 from langchain_core.output_parsers import StrOutputParser
-from langchain_core.runnables import RunnablePassthrough
+from langchain_core.chat_history import BaseChatMessageHistory
+from langchain_core.messages import HumanMessage, ToolMessage
+from langchain_core.prompts import ChatPromptTemplate, MessagesPlaceholder
+from langchain_core.runnables import RunnablePassthrough, RunnableConfig
+from langchain_core.runnables.base import Runnable
+from langchain_core.runnables.history import RunnableWithMessageHistory
+from langchain_core.runnables.utils import Output
 
 from genericsuite.util.app_context import (
     AppContext,
     CommonAppContext,
 )
 from genericsuite.util.app_logger import log_debug
 from genericsuite.util.utilities import (
@@ -38,35 +46,42 @@
 )
 from genericsuite_ai.lib.ai_chatbot_commons import (
     start_run_conversation,
     finish_run_conversation,
 )
 from genericsuite_ai.lib.ai_gpt_functions import (
     get_function_list,
+    get_functions_dict,
     gpt_func_appcontext_assignment,
 )
 from genericsuite_ai.lib.ai_langchain_tools import (
     messages_to_langchain_fmt,
+    ExistingChatMessageHistory,
 )
 from genericsuite_ai.lib.ai_langchain_models import (
     get_model_obj,
     get_model_load_error,
     # get_chat_engine_desc,
 )
 from genericsuite_ai.lib.ai_gpt_fn_conversations import (
     get_current_date_time
 )
 from genericsuite_ai.lib.translator import translate
 from genericsuite_ai.models.billing.billing_utilities import BillingUtilities
 
 
-DEBUG = False
+DEBUG = True
 
 NON_AI_TRANSLATOR = 'google_translate'
+NON_AGENT_PROMPT = 'mediabros/gs_non_agent_lcel'
+START_PHRASE_PROMPT_TOKEN = "Assistant is a large language model trained by OpenAI"
+BEGIN_PROMPT_TOKEN = "Begin!"
+
 cac = CommonAppContext()
+session_history_store: Dict[str, Any] = {}
 
 
 def translate_using(input_text: str, llm: Any) -> dict:
     """
     Translate the input text using the configured translator.
     to the user's preferred language.
 
@@ -136,31 +151,34 @@
     Returns:
         bool: True if the user's prefferred language is not English
     """
     lang = get_response_lang(cac.app_context)
     return lang.lower() != "english"
 
 
-def get_prompt(prompt_code: str) -> Any:
+def get_self_base_prompt(prompt_code: str) -> str:
     """
-    Set up the base template
+    Get the "self" (not from langsmith hub) base template text according to prompt_code.
     """
-    settings = Config(cac.app_context)
-    use_langsmith_hub = settings.LANGCHAIN_USE_LANGSMITH_HUB == "1"
-    if use_langsmith_hub:
-        try:
-            prompt: PromptTemplate = hub.pull(prompt_code)
-            base_prompt = prompt.template
-            input_variables = prompt.input_variables
-        except ConnectionError:
-            use_langsmith_hub = False
-        except Exception as err:
-            raise Exception(f"[AI_GP-E010] Error: {err}") from err
-    if not use_langsmith_hub:
-        input_variables = ['agent_scratchpad', 'chat_history', 'input', 'tool_names', 'tools']
+    _ = DEBUG and log_debug(f'>>> GET_SELF_BASE_PROMPT | prompt_code: {prompt_code}')
+    if prompt_code == NON_AGENT_PROMPT:
+        # Non-agent prompt
+        base_prompt = \
+"""
+Assistant is a large language model trained by OpenAI.
+
+Assistant is designed to be able to assist with a wide range of tasks, from answering simple questions to providing in-depth explanations and discussions on a wide range of topics. As a language model, Assistant is able to generate human-like text based on the input it receives, allowing it to engage in natural-sounding conversations and provide responses that are coherent and relevant to the topic at hand.
+
+Assistant is constantly learning and improving, and its capabilities are constantly evolving. It is able to process and understand large amounts of text, and can use this knowledge to provide accurate and informative responses to a wide range of questions. Additionally, Assistant is able to generate its own text based on the input it receives, allowing it to engage in discussions and provide explanations and descriptions on a wide range of topics.
+
+Overall, Assistant is a powerful tool that can help with a wide range of tasks and provide valuable insights and information on a wide range of topics. Whether you need help with a specific question or just want to have a conversation about a particular topic, Assistant is here to assist.
+
+Begin!
+"""
+    else:
         base_prompt = \
 """
 Assistant is a large language model trained by OpenAI.
 
 Assistant is designed to be able to assist with a wide range of tasks, from answering simple questions to providing in-depth explanations and discussions on a wide range of topics. As a language model, Assistant is able to generate human-like text based on the input it receives, allowing it to engage in natural-sounding conversations and provide responses that are coherent and relevant to the topic at hand.
 
 Assistant is constantly learning and improving, and its capabilities are constantly evolving. It is able to process and understand large amounts of text, and can use this knowledge to provide accurate and informative responses to a wide range of questions. Additionally, Assistant is able to generate its own text based on the input it receives, allowing it to engage in discussions and provide explanations and descriptions on a wide range of topics.
@@ -194,129 +212,176 @@
 
 Previous conversation history:
 {chat_history}
 
 New input: {input}
 {agent_scratchpad}
 """
-    # chat_engine_desc = get_chat_engine_desc(cac.app_context)
-    # model_name = chat_engine_desc["model"]
+    return base_prompt
+
+
+def build_gs_prompt(base_prompt: str) -> str:
+    """
+    Prepare the base prompt for the agent
+    """
+    _ = DEBUG and log_debug(f'>>> BUILD_GS_PROMPT | base_prompt: {base_prompt}')
+    settings = Config(cac.app_context)
+
     parent_model = cac.app_context.get_other_data("model_type")
     model_name = cac.app_context.get_other_data("model_name")
     model_manufacturer = cac.app_context.get_other_data("model_manufacturer")
     lang = get_response_lang(cac.app_context)
     bottom_line_prompt = get_constant("AI_PROMPT_TEMPLATES", "BOTTOM_LINE", "")
+
     translate_method = settings.LANGCHAIN_TRANSLATE_USING
-    # if chat_engine_desc["parent_model"] in ['gemini'] or \
-    #    chat_engine_desc["model"] in ['gemini']:
     if parent_model in ['gemini'] or model_name in ['gemini']:
         # Enforce translation of final answer before send it to the user
         # outside the Agent run for Models that translates the format
         # elements phrases like "Final Answer:" or "Thought:"
         translate_method = NON_AI_TRANSLATOR
     translate_answer_flag = needs_answer_translation() \
         and translate_method == 'initial_prompt'
+
     prefix = ""
     suffix = ""
     prefix += \
         f"Assistant is named {get_assistant_you_are(cac.app_context)}\n"
     suffix += \
         "\n" + \
         "ADDITIONAL GUIDELINES:\n" + \
         "----------------------\n" + \
         "\n"
+
     if translate_answer_flag:
         prefix += \
             "\n" + \
             "Think and act entirelly in english, but at the end response" + \
             f" to the Human in {lang}, no matter his/her input language.\n" + \
             "\n"
+
+    _ = DEBUG and log_debug('>>> Before get_current_date_time')
     suffix += \
-        f"For date references, {get_current_date_time({})}.\n" + \
+        f"For date references, {get_current_date_time.invoke({})}.\n" + \
         "\n" + \
         f"If the called Tool result has '{gpt_func_error('')}'," + \
         " stop processing and report the error, otherwise the" + \
         " called Tool response is Ok.\n" + \
         "\n" + \
         "Always use a json structure in the 'Action Input'" + \
         " when calling the Tool," + \
         " enclosing all attributes with curly braces.\n" + \
         bottom_line_prompt + \
         "\n"
+    _ = DEBUG and log_debug('>>> After get_current_date_time')
+
     new_prompt = base_prompt
     model_desc = f"Assistant is a large language model '{model_name}'" + \
         f" trained by '{model_manufacturer}'"
-    if "Assistant is a large language model trained by OpenAI" in new_prompt:
+
+    if START_PHRASE_PROMPT_TOKEN in new_prompt:
         new_prompt = new_prompt.replace(
-            "Assistant is a large language model trained by OpenAI",
+            START_PHRASE_PROMPT_TOKEN,
             model_desc
         )
     else:
         prefix += "\n" + model_desc
-    new_prompt = prefix + new_prompt.replace("Begin!", suffix + "Begin!")
 
+    new_prompt = prefix + new_prompt.replace(BEGIN_PROMPT_TOKEN,
+        suffix + BEGIN_PROMPT_TOKEN)
+    _ = DEBUG and log_debug(f'>>> BUILD_GS_PROMPT | new_prompt: {new_prompt}')
+    return new_prompt
+
+
+def get_agent_prompt(prompt_code: str) -> Any:
+    """
+    Set up the base template
+    """
+    _ = DEBUG and log_debug(f'>>> 1) GET_AGENT_PROMPT | prompt_code: {prompt_code}')
+    settings = Config(cac.app_context)
+    use_langsmith_hub = settings.LANGCHAIN_USE_LANGSMITH_HUB == "1"
+    if use_langsmith_hub:
+        try:
+            prompt: PromptTemplate = hub.pull(prompt_code)
+            base_prompt = prompt.template
+            input_variables = prompt.input_variables
+        except ConnectionError:
+            use_langsmith_hub = False
+        except Exception as err:
+            raise Exception(f"[AI_GP-E010] Error: {err}") from err
+    if not use_langsmith_hub:
+        input_variables = ['agent_scratchpad', 'chat_history', 'input', 'tool_names', 'tools']
+        base_prompt = get_self_base_prompt(prompt_code)
+    new_prompt = build_gs_prompt(base_prompt)
     prompt = PromptTemplate(
         input_variables=input_variables,
         template=new_prompt,
     )
     # prompt.input_variables = input_variables
     if DEBUG:
-        log_debug('>>> GET_PROMPT' +
+        log_debug('>>> 2) GET_AGENT_PROMPT' +
                   f'\n | prompt_code: {prompt_code}' +
                   f'\n | input_variables: {input_variables}' +
                   f'\n | Prompt object:\n   {prompt}')
     return prompt
 
 
 def get_agent_executor(
     agent_type: str,
     llm: Any,
     tools: list,
     messages: list,
-) -> (AgentExecutor, Union[list, str]):
-    """ Get the prompt to use and construct the agent """
+) -> Tuple[AgentExecutor, Union[list, str]]:
+    """
+    Get the prompt to use and construct the agent executor
+    """
     settings = Config(cac.app_context)
     agent_executor = None
     memory = None
     if DEBUG:
-        log_debug(f'>>> GET_AGENT | agent_type: {agent_type}')
+        log_debug(f'>>> GET_AGENT_EXECUTOR | agent_type: {agent_type}')
 
-    if agent_type == "structured_chat_agent":
+    # Agent types
+    # https://python.langchain.com/docs/modules/agents/agent_types/
+
+    # Call pipe example (LCEL):
+    # https://python.langchain.com/v0.1/docs/modules/agents/how_to/custom_agent/#create-the-agent
+
+    elif agent_type == "structured_chat_agent":
         # Structured Chat Agent
         # https://python.langchain.com/docs/modules/agents/agent_types/structured_chat
-        prompt = get_prompt("hwchase17/structured-chat-agent")
+        prompt = get_agent_prompt("hwchase17/structured-chat-agent")
         agent = create_structured_chat_agent(llm, tools, prompt)
 
     # elif agent_type == "openai_tools_agent":
     #     # https://python.langchain.com/docs/modules/agents/agent_types/openai_tools
     #     # REJECTION REASON: Doesn't accept long Tool descriptions
-    #     prompt = get_prompt("hwchase17/openai-tools-agent")
+    #     prompt = get_agent_prompt("hwchase17/openai-tools-agent")
     #     agent = create_openai_tools_agent(llm, tools, prompt)
 
     # elif agent_type == "openai_functions_agent":
     #     # https://python.langchain.com/docs/modules/agents/agent_types/openai_functions_agent
     #     # REJECTION REASON: Doesn't accept long Tool descriptions
-    #     prompt = get_prompt("hwchase17/openai-functions-agent")
+    #     prompt = get_agent_prompt("hwchase17/openai-functions-agent")
     #     agent = create_openai_functions_agent(llm, tools, prompt)
 
     # elif agent_type == "self_ask_with_search_agent":
     #     # https://python.langchain.com/docs/modules/agents/agent_types/self_ask_with_search
     #     # REJECTION REASON: ValueError: This agent expects exactly one tool
-    #     prompt = get_prompt("hwchase17/self-ask-with-search")
+    #     prompt = get_agent_prompt("hwchase17/self-ask-with-search")
     #     agent = create_self_ask_with_search_agent(llm, tools, prompt)
 
     elif agent_type in ('react_agent', 'react_chat_agent'):
         # ReAct agent
         # https://python.langchain.com/docs/modules/agents/agent_types/react
         # https://react-lm.github.io/
 
         if agent_type == "react_agent":
-            prompt = get_prompt("hwchase17/react")
+            prompt = get_agent_prompt("hwchase17/react")
         else:
-            prompt = get_prompt("hwchase17/react-chat")
+            prompt = get_agent_prompt("hwchase17/react-chat")
             # Notice that chat_history is a string, since this prompt is aimed at LLMs,
             # not chat models.
             memory = messages_to_langchain_fmt(messages, "text")
         agent = create_react_agent(llm, tools, prompt)
     else:
         raise Exception(f"[AI_GAE-E010] Invalid agent_type {agent_type}")
     if not memory:
@@ -333,14 +398,206 @@
             ),
             # early_stopping_method=settings.LANGCHAIN_EARLY_STOPPING_METHOD,
             # max_iterations=int(settings.LANGCHAIN_MAX_ITERATIONS),
         )
     return agent_executor, memory
 
 
+def filter_messages(messages, k_par: int = 10):
+    """
+    Filter messages to keep only the last k_par
+    """
+    settings = Config(cac.app_context)
+    qty_msg_to_keep = settings.LANGCHAIN_MAX_CONV_MESSAGES or k_par
+    _ = DEBUG and log_debug(f'>>> filter_messages | k: {qty_msg_to_keep}')
+    if isinstance(qty_msg_to_keep, str):
+        qty_msg_to_keep = int(qty_msg_to_keep)
+    if qty_msg_to_keep == -1:
+        return messages
+    return messages[-qty_msg_to_keep:]
+
+
+def get_session_history(session_id: str) -> BaseChatMessageHistory:
+    """
+    Get the session history for the given session_id.
+    """
+    _ = DEBUG and log_debug(f'>>> 1) GET_SESSION_HISTORY | session_id: {session_id}')
+    if session_id not in session_history_store:
+        # session_history_store[session_id] = ChatMessageHistory()
+        # https://python.langchain.com/v0.1/docs/modules/memory/
+        messages = cac.app_context.get_other_data("conv_data")["messages"]
+        _ = DEBUG and log_debug('>>> 2) GET_SESSION_HISTORY' +
+            f'\n| messages: {messages}')
+        session_history_store[session_id] = ExistingChatMessageHistory(
+            messages=messages_to_langchain_fmt(filter_messages(messages))
+        )
+    _ = DEBUG and log_debug('>>> 3) GET_SESSION_HISTORY' +
+        f'\n| Result: {session_history_store[session_id]}')
+    return session_history_store[session_id]
+
+
+def get_lcel_chain(
+    llm: Any,
+    tools: list,
+) -> Runnable:
+    """
+    Get the prompt to use and construct the LCEL chain
+    """
+    _ = DEBUG and log_debug('>>> GET_LCEL_CHAIN')
+    _ = DEBUG and log_debug(f'Tools: {tools}')
+
+    # 2024-05-21 | For LCEL:
+    # https://python.langchain.com/v0.2/docs/how_to/tool_calling/
+    llm_with_tools = llm.bind_tools(tools)
+    new_prompt = build_gs_prompt(get_self_base_prompt(NON_AGENT_PROMPT))
+    _ = DEBUG and log_debug('Start call to ChatPromptTemplate.from_messages()')
+    prompt = ChatPromptTemplate.from_messages([
+        ("system", new_prompt,),
+        MessagesPlaceholder(variable_name="messages"),
+    ])
+    _ = DEBUG and log_debug('Start chain = prompt | llm_with_tools')
+    # Build a Chatbot
+    # https://python.langchain.com/v0.2/docs/tutorials/chatbot/#message-history
+    chain = prompt | llm_with_tools
+    _ = DEBUG and log_debug('Return chain')
+    return chain
+
+
+def run_lcel_chain(
+    agent_executor: RunnableWithMessageHistory,
+    question: str,
+) -> Output:
+    """
+    Run the LCEL chain and returns the .invoke() results.
+    """
+    tools_dict = get_functions_dict(cac.app_context)
+
+    session_id = cac.app_context.get_other_data("cid")
+    config = RunnableConfig({
+        "configurable": {
+            "session_id": session_id
+        }
+    })
+    lcel_messages = [HumanMessage(content=question)]
+    exec_result = agent_executor.invoke(
+        lcel_messages,
+        config=config,
+    )
+    _ = DEBUG and \
+        log_debug('>>> 3.1) RUN_ASSISTANT | LCEL | exec_result.tool_calls:' +
+                    f' {exec_result.tool_calls}')
+
+    if exec_result.tool_calls:
+        _ = DEBUG and \
+            log_debug('>>> 3.3) RUN_ASSISTANT | Calling exec_result.tool_calls...')
+
+        # https://python.langchain.com/v0.2/docs/how_to/tool_calling/#passing-tool-outputs-to-the-model
+        lcel_messages.append(exec_result)
+        for tool_call in exec_result.tool_calls:
+            selected_tool = tools_dict[tool_call["name"].lower()]
+            if isinstance(tool_call["args"], dict) \
+                    and 'params' not in tool_call["args"]:
+                tool_args = {
+                    'params': tool_call["args"].copy()
+                }
+            else:
+                tool_args = tool_call["args"].copy()
+            _ = DEBUG and \
+                log_debug('>>> 3.3) RUN_ASSISTANT | LCEL' +
+                    f' | tool_name: {tool_call["name"].lower()}' +
+                    f'\n| tool_call["args"]: {tool_call["args"]}' +
+                    f'\n| tool_call["args"] TYPE: {type(tool_call["args"])}' +
+                    f'\n| tool_args: {tool_args}' +
+                    f'\n| tool_args TYPE: {type(tool_args)}' +
+                    f'\n| selected_tool: {selected_tool}')
+            tool_output = selected_tool.invoke(tool_args)
+            lcel_messages.append(ToolMessage(tool_output,
+                tool_call_id=tool_call["id"]))
+            session_history_store[session_id].add_message(ToolMessage(tool_output,
+                tool_call_id=tool_call["id"]))
+            _ = DEBUG and \
+                log_debug('>>> 3.4) RUN_ASSISTANT | LCEL' +
+                    f'\n| tool_output:\n{tool_output}' +
+                    '\n| session_history_store[session_id]:' +
+                    f'\n{session_history_store[session_id]}')
+
+        # Call de assistant again with tools results...
+        exec_result = agent_executor.invoke(
+            lcel_messages,
+            config=config,
+        )
+    return exec_result
+
+
+def run_assistant(
+    conv_response: dict,
+    llm: Any,
+    tools: list,
+    messages: list,
+    question: str,
+) -> dict:
+    """
+    Run the assistant
+    """
+    settings = Config(cac.app_context)
+    _ = DEBUG and \
+        log_debug('>>> 1) RUN_ASSISTANT | LANGCHAIN_AGENT_TYPE:' +
+            f' {settings.LANGCHAIN_AGENT_TYPE}')
+
+    if conv_response["error"]:
+        return conv_response
+
+    if settings.LANGCHAIN_AGENT_TYPE == 'lcel':
+        # LCEL implementation (no agent, just a LLM call)
+        agent_executor = RunnableWithMessageHistory(
+            get_lcel_chain(llm=llm, tools=tools),
+            # Build a Chatbot
+            # https://python.langchain.com/v0.2/docs/tutorials/chatbot/#message-history
+            get_session_history
+        )
+    else:
+        # Get the prompt to use and construct the agent
+        agent_executor, memory = get_agent_executor(
+            agent_type=settings.LANGCHAIN_AGENT_TYPE,
+            llm=llm,
+            tools=tools,
+            messages=messages,
+        )
+
+    # Run Agent
+    _ = DEBUG and \
+        log_debug('>>> 2) RUN_ASSISTANT | Start chain/agent execution...')
+    try:
+        if settings.LANGCHAIN_AGENT_TYPE == 'lcel':
+            # LCEL implementation (no agent, just a LLM call)
+            exec_result = run_lcel_chain(agent_executor, question)
+            conv_response["response"] = exec_result.content \
+                if hasattr(exec_result, 'content') else \
+                "ERROR - Empty response from Assistant [AIRCLC-E030]"
+        else:
+            # Chat Agent implementation
+            exec_result = agent_executor.invoke({
+                "input": question,
+                "chat_history": memory,
+            })
+            conv_response["response"] = exec_result.get(
+                "output",
+                "ERROR - Empty response from Agent [AIRCLC-E035]"
+            )
+        _ = DEBUG and \
+            log_debug('>>> 4) RUN_ASSISTANT | LANGCHAIN_AGENT_TYPE:' +
+                f' {settings.LANGCHAIN_AGENT_TYPE} |' +
+                f' exec_result: {exec_result}')
+    except Exception as error:
+        conv_response["error"] = True
+        conv_response["error_message"] = \
+            get_standard_base_exception_msg(error, "AIRCLC-E020")
+    return conv_response
+
+
 def run_conversation(app_context: AppContext) -> dict:
     """
     LangChain conversation run.
 
     Args:
         app_context (AppContext): the application context.
 
@@ -379,84 +636,55 @@
     question = conv_response["question"]["content"]
 
     # Removes the last message, because it's the user's question,
     # which is already in conv_response["question"] and
     # we want the last message to be "The next question is: {topic}"
     messages = messages[:-1]
 
-    # ............................
-    # ............................
-
-    # Agent types
-    # https://python.langchain.com/docs/modules/agents/agent_types/
-
-    # Call pipe example:
-    # https://python.langchain.com/docs/modules/agents/how_to/custom_agent
-
-    # ............................
-    # ............................
-
     # Initialize Tools
 
     # Defining custom Tools
     # https://python.langchain.com/docs/modules/agents/tools/custom_tools
     tools = get_function_list(cac.app_context)
 
     # Get the model according to user's billing plan
     billing = BillingUtilities(app_context)
     if billing.is_free_plan():
         if not billing.get_openai_api_key():
+            # No API key found
             conv_response["error"] = True
             conv_response["error_message"] = "You must specify your OPENAI_API_KEY in your" + \
                 " profile or upgrade to a paid plan [AIRCOA-E010]"
+            # Cancels the translation method
             translate_method = NON_AI_TRANSLATOR
         else:
             model_type = 'chat_openai'
     else:
         model_type = settings.LANGCHAIN_DEFAULT_MODEL
 
     # Choose the LLM that will drive the agent
     if not conv_response["error"]:
         llm = get_model_obj(cac.app_context, model_type)
         if not llm:
+            # No model found
             conv_response["error"] = True
             conv_response["error_message"] = get_model_load_error(
                 app_context=cac.app_context,
                 error_code="AIRCLC-E010"
             )
+            # Cancels the translation method
             translate_method = NON_AI_TRANSLATOR
 
-    if not conv_response["error"]:
-        # Get the prompt to use and construct the agent
-        agent_executor, memory = get_agent_executor(
-            agent_type=settings.LANGCHAIN_AGENT_TYPE,
-            llm=llm,
-            tools=tools,
-            messages=messages,
-        )
-
-        # Run Agent
-        try:
-            exec_result = agent_executor.invoke({
-                "input": question,
-                "chat_history": memory,
-            })
-            conv_response["response"] = exec_result.get(
-                "output",
-                "ERROR - Empty response from Agent [AIRCLC-E030]"
-            )
-            if DEBUG:
-                log_debug('>>> CHAT AGENT | LANGCHAIN_AGENT_TYPE:' +
-                          f' {settings.LANGCHAIN_AGENT_TYPE} |' +
-                          f' exec_result: {exec_result}')
-
-        except Exception as error:
-            conv_response["error"] = True
-            conv_response["error_message"] = \
-                get_standard_base_exception_msg(error, "AIRCLC-E020")
+    conv_response = run_assistant(
+        conv_response=conv_response,
+        llm=llm,
+        tools=tools,
+        messages=messages,
+        question=question,
+    )
 
     if not conv_response["error"] and \
        needs_answer_translation() and \
        translate_method in [NON_AI_TRANSLATOR, 'same_model']:
         # Translate response to the user's preferred language
         trans_response = translate_using(conv_response["response"],
                                           llm=llm)
```

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_chatbot_main_langchain_OLD.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_chatbot_main_langchain_ca.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Implementation of the AI Chatbot API using Langchain.
+Implementation of the AI Chatbot API using Langchain - Custom Agent (_ca).
 """
 import re
 import json
 from typing import Union, Callable
 
 from openai import PermissionDeniedError
```

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_chatbot_main_openai.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_chatbot_main_openai.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_conversations.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_conversations.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_embeddings.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_embeddings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Embeddings engine
 """
 from typing import List
 
 from langchain_openai import OpenAIEmbeddings
-from langchain.embeddings.huggingface import HuggingFaceEmbeddings
-from langchain.embeddings.clarifai import ClarifaiEmbeddings
-from langchain.embeddings.bedrock import BedrockEmbeddings
-from langchain.embeddings.cohere import CohereEmbeddings
-from langchain.embeddings.ollama import OllamaEmbeddings
+from langchain_community.embeddings import HuggingFaceEmbeddings
+from langchain_community.embeddings import ClarifaiEmbeddings
+from langchain_community.embeddings import BedrockEmbeddings
+from langchain_community.embeddings import CohereEmbeddings
+from langchain_community.embeddings import OllamaEmbeddings
 
 from genericsuite.util.app_context import AppContext
 from genericsuite.util.utilities import log_debug
 
 from genericsuite_ai.config.config import Config
 from genericsuite_ai.lib.clarifai import (
     get_model_config,
@@ -97,14 +97,16 @@
         )
     elif embedding_engine == "openai":
         # https://python.langchain.com/docs/integrations/text_embedding/openai
         response["engine"] = OpenAIEmbeddings(
             openai_api_key=openai_api_key,
             model=settings.OPENAI_EMBEDDINGS_MODEL,
         )
+    log_debug("GET_EMBEDDINGS_ENGINE |" +
+              f" response: {response}")
     return response
 
 
 def messages_to_embeddings(
     app_context: AppContext,
     conversation: list
 ) -> List[List[float]]:
```

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_gpt_fn_conversations.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_gpt_fn_conversations.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_gpt_functions.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_gpt_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -431,15 +431,15 @@
                     },
                 },
             }
         },
         "required": ["input_text"],
     }, {
         "name": "webpage_analyzer",
-        "description": "Usefull to answer a question about a" +
+        "description": "Useful to answer a question about a" +
         " given webpage URL.",
         "parameters": {
             "type": "object",
             "properties": {
                 "url": {
                     "description": "webpage URL",
                     "type": "string",
```

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_image_generator.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_image_generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 from openai.resources.images import ImagesResponse
 
 from langchain.agents import tool
 from langchain.pydantic_v1 import BaseModel, Field
 from langchain_core.messages import HumanMessage
 from langchain_google_genai import ChatGoogleGenerativeAI
 
-from genericsuite_ai.config.config import Config
 from genericsuite.util.aws import save_file_from_url
 from genericsuite.util.utilities import (
     get_default_resultset,
     get_default_value,
     get_mime_type,
     get_file_size,
     deduce_filename_from_url,
     # interpret_any,
 )
 from genericsuite.util.app_logger import log_debug
 from genericsuite.util.app_context import CommonAppContext
+
+from genericsuite_ai.config.config import Config
 from genericsuite_ai.lib.ai_conversations import (
     update_conversation_db,
     start_conversation,
 )
 from genericsuite_ai.lib.ai_langchain_tools import (
     interpret_tool_params,
 )
@@ -75,47 +76,58 @@
     return file_name, file_type
 
 
 def save_image(
     url: str,
     user_id: str,
     original_filename: str = None,
-) -> (str, str, int, str):
+) -> dict:
+# ) -> (str, str, int, str):
     """
     Save an image from a URL generated by DALL-E to AWS S3
 
     Args:
         url (str): The URL to get the image.
         user_id (str): User ID to store the file in it's S3 space.
         Defaults to None.
         original_filename (str): original file name. Defaults to None.
 
     Returns:
-        (str, str, int, str): a tuple with the following elements:
-        attachment_url (str): URL for the image.
-        final_filename (str): file name of the image with date/time added.
-        file_size (int): the file size in bytes.
-        error (str): the eventual error message or None if no errors
+        dict: A dictionary with the following elements:
+            attachment_url (str): URL for the image.
+            final_filename (str): file name of the image with date/time added.
+            file_size (int): the file size in bytes.
+            error (bool): True if there was an error, False otherwise.
+            error_message (str): the eventual error message or None if no errors
     """
     settings = Config(cac.get())
-    attachment_url = None
-    final_filename = None
-    file_size = None
+    result = get_default_resultset()
+    result['attachment_url'] = None
+    result['final_filename'] = None
+    result['file_size'] = None
     bucket_name = settings.AWS_S3_CHATBOT_ATTACHMENTS_BUCKET
     if not bucket_name:
-        error = "AWS_S3_CHATBOT_ATTACHMENTS_BUCKET is not configured [2]"
+        result['error'] = True
+        result['error_message'] = "AWS_S3_CHATBOT_ATTACHMENTS_BUCKET is not configured [2]"
     else:
-        public_url, final_filename, file_size, error = save_file_from_url(
+        # public_url, final_filename, file_size, error = save_file_from_url(
+        save_result = save_file_from_url(
             url=url,
             bucket_name=bucket_name,
             sub_dir=user_id,
             original_filename=original_filename,
         )
-        attachment_url = public_url
-    return attachment_url, final_filename, file_size, error
+        # attachment_url = ublic_url
+        result['error'] = save_result['error']
+        result['error_message'] = save_result['error_message']
+        result['attachment_url'] = save_result['public_url']
+        result['final_filename'] = save_result['final_filename']
+        result['file_size'] = save_result['file_size']
+    return result
+    # return attachment_url, final_filename, file_size, error
 
 
 def get_img_gen_name() -> str:
     """ Returns the Image Generator configured technology name """
     settings = Config(cac.get())
     if settings.AI_IMG_GEN_TECHNOLOGY == "gemini":
         model_name = "Google Gemini"
@@ -325,29 +337,29 @@
         if isinstance(response["response"], str):
             response["response"] = [response["response"]]
         public_url_list = []
         for url in response["response"]:
             # Images generated must be saved because the URL returned by the model
             # expires.
             file_name, file_type = get_filename_from_dalle_url(url)
-            public_url, final_filename, file_size, error = save_image(
+            save_result = save_image(
                 url=url,
                 user_id=cac.app_context.get_user_id(),
                 original_filename=file_name
             )
-            if error:
+            if save_result['error']:
                 response['error'] = True
-                response['error_message'] = f"ERROR [IAIG-020]: {str(error)}"
+                response['error_message'] = f"ERROR [IAIG-020]: {str(save_result['error_message'])}"
                 break
             public_url_list.append({
                 "file_name": file_name,
                 "file_type": file_type,
-                "public_url": public_url,
-                "final_filename": final_filename,
-                "file_size": file_size,
+                "public_url": save_result['public_url'],
+                "final_filename": save_result['final_filename'],
+                "file_size": save_result['file_size'],
             })
 
     if not response['error']:
         response['response'] = public_url_list
 
     if "cid" in other:
         if not response['error']:
```

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_langchain_models.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_langchain_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,18 @@
 """
 Langchain models
 """
 from typing import Union, Optional
 
 from langchain_openai import OpenAI
 from langchain_openai import ChatOpenAI
-from langchain.llms.clarifai import Clarifai
+from langchain_community.llms import Clarifai
 
-from langchain.chat_models.anthropic import ChatAnthropic
-# from langchain.chat_models.cohere import ChatCohere
-# from langchain.chat_models.google_palm import ChatGooglePalm
-# from langchain.chat_models.vertexai import ChatVertexAI
-from langchain.chat_models.ollama import ChatOllama
+from langchain_community.chat_models.anthropic import ChatAnthropic
+from langchain_community.chat_models.ollama import ChatOllama
 
 from langchain_community.llms.huggingface_text_gen_inference import (
     HuggingFaceTextGenInference
 )
 
 from langchain_core.runnables.utils import (
     ConfigurableField,
```

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_langchain_tools.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_langchain_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 
     Returns:
         ConversationBufferMemory: Buffer for storing conversation memory.
     """
     chat_memory = ExistingChatMessageHistory(
         messages=messages_to_langchain_fmt(messages)
     )
+    # https://python.langchain.com/v0.1/docs/modules/memory/
     memory = ConversationBufferMemory(
         memory_key="chat_history",
         chat_memory=chat_memory,
     )
     # memory = load_conversarion_messages_to_buffer(memory, messages)
     return memory
 
@@ -175,30 +176,35 @@
         first_param_name (str): first param name, for those cases when the
             Agent pass only a string (no JSON) and it'll be assigned as
             the 1st required parameter
 
     Returns:
         dict: The interpreted tool params.
     """
+
     self_debug = DEBUG or is_under_test()
+    # self_debug = True
     _ = self_debug and \
         log_debug("INTERPRET_TOOL_PARAMS" +
             f"\n | tool_params: {tool_params}" + 
             f"\n | tool_params type: {type(tool_params)}"
             f"\n | schema: {schema}" +
             f"\n | first_param_name: {first_param_name}")
     if not tool_params:
         return tool_params
+    if isinstance(tool_params, dict) and 'params' in tool_params:
+        tool_params = tool_params['params'].copy()
     if isinstance(tool_params, str):
         # if tool_params has a "\n" and a additional line with anything
         # like "```" or "Observation", apart the last } and \n,
         # that extra info must be removed...
         for _ in range(3):
             if "\n" in tool_params:
-                tool_params = tool_params.rsplit("\n", 1)[0]  # Remove last line if it exists after a newline
+                # Remove last line if it exists after a newline
+                tool_params = tool_params.rsplit("\n", 1)[0]
         if tool_params.endswith("```"):
             tool_params = tool_params[:-3]  # Remove the trailing characters
         if tool_params.endswith("Observation"):
             tool_params = tool_params[:-11]  # Remove the trailing characters
         try:
             tool_params = json.loads(tool_params)
         except json.decoder.JSONDecodeError:
```

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_sub_bots.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_sub_bots.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_utilities.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_utilities.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/ai_vision.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/ai_vision.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 from openai import OpenAI
 
 from langchain.agents import tool
 from langchain.pydantic_v1 import BaseModel, Field
 from langchain_core.messages import HumanMessage
 from langchain_google_genai import ChatGoogleGenerativeAI
 
-from genericsuite.util.aws import upload_nodup_file_to_s3
+from genericsuite.util.aws import (
+    upload_nodup_file_to_s3,
+    prepare_asset_url,
+)
 from genericsuite.util.utilities import (
     get_default_resultset,
     get_file_size,
     is_an_url,
     get_default_value,
     get_mime_type,
     deduce_filename_from_url,
@@ -38,15 +41,15 @@
     gpt_func_error,
 )
 from genericsuite_ai.lib.clarifai import (
     clarifai_vision,
 )
 from genericsuite_ai.models.billing.billing_utilities import BillingUtilities
 
-DEBUG = False
+DEBUG = True
 cac = CommonAppContext()
 
 
 class VisionParams(BaseModel):
     """
     Vision parameters structure
     """
@@ -70,86 +73,97 @@
 
 
 def get_vision_image_url(
     image_path: str,
     original_filename: str = None,
     use_s3: bool = False,
     user_id: str = None,
-):
+) -> dict:
     """
     Get the URL for the specified image for the GPT4 vision message content.
 
     Args:
         image_path (str): The path to the image.
         original_filename (str): original file name.
         use_s3 (bool): True to use AWS S3 storage. Defaults to False.
         user_id (str): User ID to store the file in it's S3 space.
         Defaults to None.
 
     Returns:
-        attachment_url (str): URL for the image.
-        final_filename (str): file name of the image with date/time added.
-        error (str): the eventual error message or None if no errors
+        dict = A dictionary with the following elements:
+            attachment_url (str): URL for the image.
+            final_filename (str): file name of the image with date/time added.
+            error (bool): True if an error occurred.
+            error_message (str): the eventual error message or None if no errors
     """
+    result = get_default_resultset()
     settings = Config(cac.get())
     attachment_url = None
     final_filename = None
-    error = None
     # Check if the image path is a URL
     if is_an_url(image_path):
         attachment_url = image_path
         final_filename = deduce_filename_from_url(image_path)
     # Local file...
     elif use_s3:
         bucket_name = settings.AWS_S3_CHATBOT_ATTACHMENTS_BUCKET
         if DEBUG:
             log_debug('get_vision_image_url | ' +
                       f'AWS_S3_CHATBOT_ATTACHMENTS_BUCKET: {str(bucket_name)}')
         if not bucket_name:
-            error = "AWS_S3_CHATBOT_ATTACHMENTS_BUCKET is not configured [1]"
+            result['error'] = True
+            result['error_message'] = "AWS_S3_CHATBOT_ATTACHMENTS_BUCKET is not configured [1]"
         else:
-            public_url, final_filename, error = upload_nodup_file_to_s3(
+            upload_result = upload_nodup_file_to_s3(
                 file_path=image_path,
                 original_filename=original_filename,
                 bucket_name=bucket_name,
                 sub_dir=user_id,
             )
-            attachment_url = public_url
+            attachment_url = upload_result['public_url']
+            final_filename = upload_result['final_filename']
+            result['error'] = upload_result['error']
+            result['error_message'] = upload_result['error_message']
     else:
         # Get the base64 string
         base64_image = encode_image(image_path)
         attachment_url = f"data:{get_mime_type(image_path)};" + \
                          f"base64,{base64_image}"
-    return attachment_url, final_filename, error
+    result['attachment_url'] = attachment_url
+    result['final_filename'] = final_filename
+    return result
+    # return attachment_url, final_filename, error
 
 
 def get_vision_name() -> str:
     """ Returns the Vision configured technology name """
     settings = Config(cac.get())
     if settings.AI_VISION_TECHNOLOGY == "gemini":
         model_name = "Google Gemini Vision"
     elif settings.AI_VISION_TECHNOLOGY == "clarifai":
         model_name = "Clarifai Vision: " + \
             f"{settings.AI_CLARIFAI_DEFAULT_VISION_MODEL}"
     else:
-        model_name = "OpenAI GPT4 Vision"
-    log_debug("get_vision_name | AI_VISION_TECHNOLOGY:" +
-              f" {settings.AI_VISION_TECHNOLOGY}"
-              f" | model_name: {model_name}")
+        model_name = "OpenAI GPT4 Vision: " + \
+            f"{settings.OPENAI_VISION_MODEL}"
+    if DEBUG:
+        log_debug("get_vision_name | AI_VISION_TECHNOLOGY:" +
+            f" {settings.AI_VISION_TECHNOLOGY}"
+            f" | model_name: {model_name}")
     return model_name
 
 
 def get_vision_response(response: dict, other: dict) -> dict:
     """ Returns the Vision configured technology response """
 
     settings = Config(cac.get())
     billing = BillingUtilities(cac.get())
     # Maximun tokens to be used by the model. Defaults to 500.
     max_tokens = get_default_value("max_tokens", other,
-                                   settings.OPENAI_MAX_TOKENS)
+                                   int(settings.OPENAI_MAX_TOKENS))
     log_debug("get_vision_response | AI_VISION_TECHNOLOGY:" +
               f" {settings.AI_VISION_TECHNOLOGY}")
     try:
         if settings.AI_VISION_TECHNOLOGY == "gemini":
             client = ChatGoogleGenerativeAI(
                 # model="gemini-pro-vision"
                 model=settings.GOOGLE_VISION_MODEL,
@@ -218,14 +232,15 @@
 
     Returns:
         dict: a standard response with the question answered by the model.
     """
     # Reference:
     # https://platform.openai.com/docs/guides/vision
 
+    settings = Config(cac.get())
     if DEBUG:
         log_debug("vision_image_analyzer | params: " +
                   str(params))
     params = interpret_tool_params(tool_params=params,
                                    first_param_name="image_path",
                                    schema=VisionParams)
 
@@ -291,35 +306,57 @@
                     f"Question: {question}\n" +
                     f"Other parameters: {other}\n")
 
         # Sometimes ChatGPT only needs the image description...
         # so the question received is None
         question = "" if not question else question
 
-        attachment_url, final_filename, error = get_vision_image_url(
+        image_url_result = get_vision_image_url(
             image_path,
             original_filename,
             use_s3,
             cac.app_context.get_user_id(),
         )
-        if error:
+        if image_url_result['error']:
             response['error'] = True
-            response['error_message'] = error
+            response['error_message'] = image_url_result['error_message']
             return response
+
         response["question"] = [
             {
                 "type": "text",
                 "text": question,
             },
-            {
-                "type": "image_url",
-                "image_url": attachment_url
-            },
         ]
 
+        # GPT-4-turbo vision API recognizes image_url as base64 encoded image data
+        # https://community.openai.com/t/gpt-4-turbo-vision-api-recognizes-image-url-as-base64-encoded-image-data/734243
+        resolution = "auto"  # "auto" | "low" | "high"
+        if settings.AI_VISION_TECHNOLOGY == "openai":
+            if settings.OPENAI_VISION_MODEL == "gpt-4o":
+                response["question"].append(
+                    {
+                        "type": "image_url",
+                        "image_url": {
+                            "url": prepare_asset_url(
+                                image_url_result['attachment_url']),
+                            "detail": resolution,
+                        }
+                    },
+                )
+            else:
+                # For legacy model "gpt-4-vision-preview"
+                response["question"].append(
+                    {
+                        "type": "image_url",
+                        "image_url": prepare_asset_url(
+                            image_url_result['attachment_url'])
+                    },
+                )
+
         if DEBUG:
             log_debug(f"\nQuestion for {get_vision_name()}:" +
                     f'{response["question"]}\n')
 
         if other["mock_error"] == "1":
             response["error"] = True
             response["error_message"] = "---ON PURPOSE ERROR---"
@@ -337,24 +374,24 @@
     if "cid" in other:
         if not response['error']:
             response["add_msg_after"] = [
                 {
                     "role": "user",
                     "type": "file_name",
                     "sub_type": (
-                        get_mime_type(final_filename)
-                        if get_mime_type(final_filename)
+                        get_mime_type(image_url_result['final_filename'])
+                        if get_mime_type(image_url_result['final_filename'])
                         else "image"
                     ),
                     "file_name": (
                         f'"{original_filename}" (' +
                         f'{get_file_size(file_size, "mb")})'
                     ),
-                    "attachment_url": attachment_url,
-                    "final_filename": final_filename,
+                    "attachment_url": image_url_result['attachment_url'],
+                    "final_filename": image_url_result['final_filename'],
                 }
             ]
             if DEBUG:
                 log_debug("\nVISION_IMAGE_ANALYZER | Question fixed for" +
                           f' update_conversation_db: {response["question"]}')
         response = update_conversation_db(
             app_context=cac.app_context,
@@ -362,15 +399,15 @@
         )
     return response
 
 
 @tool
 def vision_image_analyzer_text_response(params: Any) -> str:
     """
-Usefull to process an specified image and answer a question about it. There must be an explitcit image URL specified by the Human or in the conversation.
+Useful to process an specified image and answer a question about it. There must be an explitcit image URL specified by the Human or in the conversation.
 Args: params (dict): Tool parameters. Must contain:
 "image_path" (str): image URL.
 "question" (str): question about the image.
     """
     return vision_image_analyzer_text_response_func(params)
```

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/clarifai.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/clarifai.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,24 +384,24 @@
     sub_dir = cac.app_context.get_user_id()
     original_filename = "gen-image.jpg"
 
     image_filename = f"/tmp/{original_filename}"
     with open(image_filename, 'wb') as f:
         f.write(output)
 
-    public_url, final_filename, error = upload_nodup_file_to_s3(
+    upload_result = upload_nodup_file_to_s3(
         file_path=image_filename,
         original_filename=original_filename,
         bucket_name=bucket_name,
         sub_dir=sub_dir,
     )
-    if error:
-        raise Exception("AWS S3 upload error:: " + error)
+    if upload_result['error']:
+        raise Exception("AWS S3 upload error:: " + upload_result['error'])
 
-    result = public_url
+    result = upload_result['public_url']
     os.remove(image_filename)  # Clean up the temporary file
 
     if DEBUG:
         log_debug('CF-IGRAW-2) Clarifai - clarifai_img_gen_raw' +
                   " | result: " + result)
         # Uncomment this line to print the full Response JSON
         # log_debug('CF-IGRAW-4) Clarifai - clarifai_img_gen_raw' +
```

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/git_reader.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/git_reader.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/json_reader.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/json_reader.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/pdf_reader.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/pdf_reader.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/translator.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/translator.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/vector_index.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/vector_index.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 from langchain.chains.conversational_retrieval.base import (
     ConversationalRetrievalChain
 )
 from langchain.indexes.vectorstore import VectorStoreIndexWrapper
 from langchain.schema import Document
 from langchain.text_splitter import CharacterTextSplitter
 
-from langchain.vectorstores.mongodb_atlas import MongoDBAtlasVectorSearch
-from langchain.vectorstores.chroma import Chroma
-from langchain.vectorstores.clarifai import Clarifai
-# from langchain.vectorstores.pinecone import Pinecone
-from langchain.vectorstores.vectara import Vectara
-from langchain.vectorstores.weaviate import Weaviate
-from langchain.vectorstores.faiss import FAISS
+from langchain_community.vectorstores import MongoDBAtlasVectorSearch
+from langchain_community.vectorstores import Chroma
+from langchain_community.vectorstores import Clarifai
+# from langchain_community.vectorstores import Pinecone
+from langchain_community.vectorstores import Vectara
+from langchain_community.vectorstores import Weaviate
+from langchain_community.vectorstores import FAISS
 
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_core.vectorstores import (
     VectorStoreRetriever,
     # VectorStore
 )
 from langchain_core.output_parsers import StrOutputParser
```

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/web_scraping.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/web_scraping.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     if not result["error"]:
         llm = get_model_obj(cac.app_context)
         if not llm:
             result = error_resultset(get_model_load_error(
                 app_context=cac.app_context,
                 error_code="WS_GQC-E010"))
 
-    qa_chain = None
+    result["qa_chain"] = None
     if not result["error"]:
         # Build a QA chain
         vectorstore = get_vectorstore["vector_store"]
         result["qa_chain"] = RetrievalQA.from_chain_type(
             # llm="gpt-3.5-turbo",  # Specify the LLM model you want to use
             llm=llm,  # Specify the LLM model you want to use
 
@@ -191,15 +191,15 @@
             "\n")
     return result
 
 
 @tool
 def webpage_analyzer_text_response(params: Any) -> str:
     """
-Usefull to answer a question about a given webpage URL.
+Useful to answer a question about a given webpage URL.
 Args: params (dict): Tool parameters. Must contain:
 "url" (str): webpage URL.
 "question" (str): question about the webpage.
     """
     return webpage_analyzer_text_response_func(params)
```

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/web_search.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/web_search.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 """
 
 from typing import Union, Any, Optional
 import json
 import time
 # from itertools import islice
 
-from httpx._exceptions import HTTPError
+# from httpx._exceptions import HTTPError
 
 # Pypi: pip install duckduckgo-search
 from duckduckgo_search import DDGS
 
 from langchain_community.tools.ddg_search.tool import DuckDuckGoSearchResults
+from langchain_community.utilities import DuckDuckGoSearchAPIWrapper
+from langchain_google_community import GoogleSearchAPIWrapper
 from langchain.agents import tool
 from langchain.pydantic_v1 import BaseModel, Field
-from langchain.utilities.duckduckgo_search import DuckDuckGoSearchAPIWrapper
-from langchain.utilities.google_search import GoogleSearchAPIWrapper
 
 from genericsuite.util.app_logger import log_debug
 from genericsuite.util.app_context import CommonAppContext
 from genericsuite_ai.lib.ai_langchain_tools import (
     interpret_tool_params,
 )
 from genericsuite_ai.lib.ai_utilities import (
     gpt_func_error,
 )
 from genericsuite_ai.config.config import Config
 
-DEBUG = False
+DEBUG = True
 
 cac = CommonAppContext()
 
 DUCKDUCKGO_MAX_ATTEMPTS = 3
 
 
 # from ..registry import ability
@@ -59,15 +59,15 @@
     query: str = Field(description="The search query")
     num_results: Optional[int] = Field(default=20, description="The number of results to return.")
 
 
 @tool
 def web_search(params: Any) -> str:
     """
-Usefull when you need to perform a web search to have access to real-time information, and/or answer questions about recent events.
+Useful when you need to perform a web search to have access to real-time information, and/or answer questions about recent events.
 Args: params (dict): Tool parameter. Must contain:
 "query" (str): The search query.
 "num_results" (int): number of results to return. Defaults to 20.
     """
     return web_search_func(params)
 
 
@@ -80,25 +80,33 @@
         params (dict): Tool parameter. Must contain:
             "query" (str): The search query.
             "num_results" (int): number of results to return. Defaults to 20.
 
     Returns:
         str: The results of the search or [FUNC+ERROR] {error_message}
     """
+    settings = Config(cac.get())
     params = interpret_tool_params(
         tool_params=params,
         first_param_name="query",
         schema=WebSearch,
     )
     query = params.query
     num_results = params.num_results
+    func_error_token = gpt_func_error('').strip()
 
-    result = web_search_ddg_lc(query, num_results)
-    if not result or "ERROR:" in result:
+    if settings.WEBSEARCH_DEFAULT_PROVIDER == "ddg":
+        result = web_search_ddg_lc(query, num_results)
+    elif settings.WEBSEARCH_DEFAULT_PROVIDER == "google":
         result = web_search_google(query, num_results)
+    else:
+        result = web_search_ddg_lc(query, num_results)
+        if not result or func_error_token in result:
+            result = web_search_google(query, num_results)
+
     return result
 
 
 def web_search_google(query: str, num_results: int = 20) -> str:
     """
     Return the results of a Google search with a call to
     the langchain wrapper.
@@ -108,31 +116,37 @@
         num_results (int): The number of results to return.
 
     Returns:
         str: The results of the search.
     """
     settings = Config(cac.get())
     if DEBUG:
-        log_debug(f"\n\n>> WEB_SEARCH_GOOGLE | query: {query}\n\n")
-        log_debug(f"\n\ngoogle_api_key: {settings.GOOGLE_API_KEY}\n\n")
-        log_debug(f"\n\ngoogle_cse_id: {settings.GOOGLE_CSE_ID}\n\n")
+        log_debug(f">> 1) WEB_SEARCH_GOOGLE | query: {query}" +
+            f"\ngoogle_api_key: {settings.GOOGLE_API_KEY}" +
+            f"\ngoogle_cse_id: {settings.GOOGLE_CSE_ID}")
+
+    # https://stackoverflow.com/questions/76547862/why-is-my-google-custom-search-api-call-from-python-not-working
+    # To fix the error "'Request contains an invalid argument.',
+    #   'domain': 'global', 'reason': 'badRequest'"
+    max_results = max(int(num_results), 10)
 
     # https://python.langchain.com/docs/integrations/tools/google_search#number-of-results
     try:
         search = GoogleSearchAPIWrapper(
             google_api_key=settings.GOOGLE_API_KEY,
             google_cse_id=settings.GOOGLE_CSE_ID,
+            k=max_results
         )
-        results_list = search.results(query, num_results)
+        results_list = search.results(query, max_results)
         results = safe_google_results(results_list)
     except Exception as error:
         results = gpt_func_error(error)
 
     if DEBUG:
-        log_debug("\n\n>> WEB_SEARCH_GOOGLE | " +
+        log_debug(">> 2) WEB_SEARCH_GOOGLE | " +
                   f" results: {results}\n\n")
 
     return results
 
 
 def web_search_ddg_lc(query: str, num_results: int = 20) -> str:
     """
@@ -149,19 +163,20 @@
     if DEBUG:
         log_debug(f"\n\n>> WEB_SEARCH_LANGCHAIN_DDG | query: {query}\n\n")
 
     wrapper = DuckDuckGoSearchAPIWrapper(max_results=num_results)
     search = DuckDuckGoSearchResults(api_wrapper=wrapper)
     try:
         results_list = search.run(query)
-        results = safe_google_results(results_list)
-    except HTTPError as error:
+        results = safe_ddg_results(results_list)
+    # except HTTPError as error:
+    except Exception as error:
         log_debug("\n\n>> WEB_SEARCH_LANGCHAIN_DDG" +
                   f" | error: {error}\n\n")
-        results = gpt_func_error(error)
+        results = gpt_func_error(f'{error}')
 
     if DEBUG:
         log_debug(f"\n\n>> WEB_SEARCH_LANGCHAIN_DDG | results: {results}\n\n")
 
     return results
 
 
@@ -173,15 +188,15 @@
     Args:
         query (str): The search query.
         num_results (int): The number of results to return.
 
     Returns:
         str: The results of the search.
     """
-    search_results = []
+    search_results: list[Any] = []
     attempts = 0
 
     if DEBUG:
         log_debug("")
         log_debug(f">> WEB_SEARCH | query: {query}")
         log_debug("")
 
@@ -193,15 +208,15 @@
                 search_results = list(ddgs.text(query, max_results=num_results))
             if search_results:
                 break
             time.sleep(1)
             attempts += 1
         results = safe_google_results(search_results)
     except Exception as error:
-        results = gpt_func_error(error)
+        results = gpt_func_error(f'{error}')
 
     if DEBUG:
         log_debug(f">> WEB_SEARCH | results: {results}")
         log_debug("")
 
     return results
 
@@ -212,20 +227,59 @@
 
     Args:
         results (str | list): The search results.
 
     Returns:
         str: The results of the search.
     """
+    _ = DEBUG and \
+        log_debug(f">> 1) SAFE_GOOGLE_RESULTS | results: {results}")
     if isinstance(results, list):
         safe_message = json.dumps({
-            "results": [result.encode("utf-8", "ignore").decode("utf-8")
-                        for result in results],
+            # "results": [result.encode("utf-8", "ignore").decode("utf-8")
+            #             for result in results],
+            "results": [{
+                'Result': result.get('Result', '').encode("utf-8", "ignore").decode("utf-8"),
+            } if 'Result' in result else {
+                'snippet': result.get('snippet', '').encode("utf-8", "ignore").decode("utf-8"),
+                'title': result.get('title', '').encode("utf-8", "ignore").decode("utf-8"),
+                'link': result.get('link', '').encode("utf-8", "ignore").decode("utf-8"),
+            } for result in results],
         })
     else:
         safe_message = results.encode("utf-8", "ignore").decode("utf-8")
+    _ = DEBUG and \
+        log_debug(f">> 2) SAFE_GOOGLE_RESULTS | results: {results}")
+    return safe_message
 
-    if DEBUG:
-        log_debug(f">> WEB_SEARCH | results: {results}")
-        log_debug("")
 
+def safe_ddg_results(results: Union[str, list]) -> str:
+    """
+        Return the results of a DuckduckGo search in a safe format.
+
+    Args:
+        results (str | list): The search results.
+
+    Returns:
+        str: The results of the search.
+    """
+    _ = DEBUG and \
+        log_debug(">> 1) SAFE_DDG_RESULTS" +
+            f"\n | results TYPE: {type(results)}" +
+            f"\n | results: {results}")
+    if isinstance(results, list):
+        safe_message = json.dumps({
+            "results": [{
+                'Result': result.Result.encode("utf-8", "ignore").decode("utf-8"),
+            } if hasattr(result, 'Result') else {
+                'snippet': result.snippet.encode("utf-8", "ignore").decode("utf-8"),
+                'title': result.title.encode("utf-8", "ignore").decode("utf-8"),
+                'link': result.link.encode("utf-8", "ignore").decode("utf-8"),
+            } for result in results],
+        })
+    else:
+        safe_message = results.encode("utf-8", "ignore").decode("utf-8")
+    _ = DEBUG and \
+        log_debug(">> 2) SAFE_DDG_RESULTS" +
+            f"\n | results TYPE: {type(results)}" +
+            f"\n | results: {results}")
     return safe_message
```

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/lib/youtube_reader.py` & `genericsuite_ai-0.1.6/genericsuite_ai/lib/youtube_reader.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.5/genericsuite_ai/models/billing/billing_utilities.py` & `genericsuite_ai-0.1.6/genericsuite_ai/models/billing/billing_utilities.py`

 * *Files identical despite different names*

### Comparing `genericsuite_ai-0.1.5/pyproject.toml` & `genericsuite_ai-0.1.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "genericsuite_ai"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
     { name="Carlos J. Ramirez", email="<tomkat_cr@yahoo.com>" }
 ]
 description = "The GenericSuite AI for Python (backend version)"
 readme = "README.md"
 requires-python = ">=3.9,<4.0"
 classifiers = [
@@ -15,49 +15,48 @@
 
 [project.urls]
 Homepage = "https://genericsuite.carlosjramirez.com/Backend-Development/GenericSuite-AI/"
 Issues = "https://github.com/tomkat-cr/genericsuite-be-ai/issues"
 
 [tool.poetry]
 name = "genericsuite_ai"
-version = "0.1.5"
+version = "0.1.6"
 description = "The GenericSuite AI for Python (backend version)"
 authors = ["Carlos J. Ramirez <tomkat_cr@yahoo.com>"]
 license = "ISC"
 readme = "README.md"
 repository = "https://github.com/tomkat-cr/genericsuite-be-ai.git"
 homepage = "https://genericsuite.carlosjramirez.com/Backend-Development/GenericSuite-AI/"
 packages = [
     { include = "genericsuite_ai" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 openai = "^1.7.2"
-langchain = "^0.1.1"
+langchain = "^0.1.20"
 click = "^8.1.7"
 jmespath = "^1.0.1"
 pyyaml = "^6.0.1"
 setuptools = "^65.5.1"
 six = "^1.16.0"
 typing-extensions = "^4.8.0"
-duckduckgo-search = "^4.1.1"
+duckduckgo-search = "^6.1.1"
 requests-toolbelt = "^1.0.0"
-tiktoken = "^0.5.2"
+tiktoken = "0.6"
 faiss-cpu = "^1.7.4"
 google-api-python-client = "^2.111.0"
-langchain-google-genai = "^0.0.5"
+langchain-google-genai = {version = "^1.0.3", extras = ["images"]}
 pillow = "^10.1.0"
 clarifai = "^10.1.0"
-langchain-openai = "^0.0.8"
-langchainhub = "^0.1.14"
+langchain-openai = "^0.1.6"
+langchainhub = "^0.1.15"
 jq = "^1.6.0"
 transformers = "^4.38.2"
 text-generation = "^0.6.1"
-genericsuite = "^0.1.5"
 
 [tool.poetry.group.dev.dependencies]
 changelog-cli = "^0.7.1"
 mypy = "^0.931"
 pylint = "^3.1.0"
 pytest = "^7.0.1"
 pytest-cov = "^3.0.0"
```

