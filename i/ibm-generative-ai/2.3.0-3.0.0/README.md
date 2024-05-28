# Comparing `tmp/ibm_generative_ai-2.3.0.tar.gz` & `tmp/ibm_generative_ai-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibm_generative_ai-2.3.0.tar", max compression
+gzip compressed data, was "ibm_generative_ai-3.0.0.tar", max compression
```

## Comparing `ibm_generative_ai-2.3.0.tar` & `ibm_generative_ai-3.0.0.tar`

### file list

```diff
@@ -1,111 +1,114 @@
--rw-r--r--   0        0        0    11357 2024-03-22 18:43:52.830625 ibm_generative_ai-2.3.0/LICENSE
--rw-r--r--   0        0        0     2781 2024-03-22 18:43:52.830625 ibm_generative_ai-2.3.0/README.md
--rw-r--r--   0        0        0     8594 2024-03-22 18:44:42.915022 ibm_generative_ai-2.3.0/pyproject.toml
--rw-r--r--   0        0        0      347 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/__init__.py
--rw-r--r--   0        0        0     1530 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_types.py
--rw-r--r--   0        0        0        0 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/__init__.py
--rw-r--r--   0        0        0     6170 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/api_client.py
--rw-r--r--   0        0        0     6044 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/async_executor.py
--rw-r--r--   0        0        0     1514 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/asyncio_future.py
--rw-r--r--   0        0        0     1141 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/deprecated_schema_import.py
--rw-r--r--   0        0        0     5704 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/general.py
--rw-r--r--   0        0        0        0 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/http_client/__init__.py
--rw-r--r--   0        0        0     3467 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/http_client/httpx_client.py
--rw-r--r--   0        0        0     3073 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/http_client/rate_limit_transport.py
--rw-r--r--   0        0        0     7168 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/http_client/retry_transport.py
--rw-r--r--   0        0        0     4042 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/limiters/adjustable_semaphor.py
--rw-r--r--   0        0        0      532 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/limiters/base_limiter.py
--rw-r--r--   0        0        0     1927 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/limiters/container_limiter.py
--rw-r--r--   0        0        0      182 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/limiters/dummy_limiter.py
--rw-r--r--   0        0        0     2760 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/limiters/external_limiter.py
--rw-r--r--   0        0        0     1117 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/limiters/local_limiter.py
--rw-r--r--   0        0        0     1034 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/limiters/shared_limiter.py
--rw-r--r--   0        0        0      505 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/queues/flushable_queue.py
--rw-r--r--   0        0        0     2269 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/queues/ordered_queue.py
--rw-r--r--   0        0        0     1276 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/responses.py
--rw-r--r--   0        0        0       92 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/service/__init__.py
--rw-r--r--   0        0        0     4215 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/service/base_service.py
--rw-r--r--   0        0        0     1931 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/service/metadata.py
--rw-r--r--   0        0        0     2593 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/shared_instance.py
--rw-r--r--   0        0        0     2100 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/shared_loop.py
--rw-r--r--   0        0        0     1542 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/shared_options.py
--rw-r--r--   0        0        0      575 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/_utils/validators.py
--rw-r--r--   0        0        0       91 2024-03-22 18:44:42.915022 ibm_generative_ai-2.3.0/src/genai/_version.py
--rw-r--r--   0        0        0     5965 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/client.py
--rw-r--r--   0        0        0     2070 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/credentials.py
--rw-r--r--   0        0        0     2266 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/exceptions.py
--rw-r--r--   0        0        0       82 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/extensions/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/extensions/_common/__init__.py
--rw-r--r--   0        0        0     2693 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/extensions/_common/utils.py
--rw-r--r--   0        0        0      132 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/extensions/huggingface/__init__.py
--rw-r--r--   0        0        0     2038 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/extensions/huggingface/agent.py
--rw-r--r--   0        0        0     1342 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/extensions/langchain/__init__.py
--rw-r--r--   0        0        0    10474 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/extensions/langchain/chat_llm.py
--rw-r--r--   0        0        0     2790 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/extensions/langchain/embeddings.py
--rw-r--r--   0        0        0     9753 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/extensions/langchain/llm.py
--rw-r--r--   0        0        0      498 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/extensions/langchain/template.py
--rw-r--r--   0        0        0     4855 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/extensions/langchain/utils.py
--rw-r--r--   0        0        0      249 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/extensions/llama_index/__init__.py
--rw-r--r--   0        0        0     2101 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/extensions/llama_index/embeddings.py
--rw-r--r--   0        0        0     8500 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/extensions/llama_index/llm.py
--rw-r--r--   0        0        0      285 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/extensions/localserver/__init__.py
--rw-r--r--   0        0        0     8807 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/extensions/localserver/local_api_server.py
--rw-r--r--   0        0        0     1750 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/extensions/localserver/local_base_model.py
--rw-r--r--   0        0        0     1158 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/extensions/localserver/schema.py
--rw-r--r--   0        0        0      461 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/file/__init__.py
--rw-r--r--   0        0        0     9102 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/file/file_service.py
--rw-r--r--   0        0        0      103 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/folder/__init__.py
--rw-r--r--   0        0        0     4355 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/folder/folder_service.py
--rw-r--r--   0        0        0      442 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/model/__init__.py
--rw-r--r--   0        0        0     2856 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/model/model_service.py
--rw-r--r--   0        0        0      444 2024-03-22 18:43:52.838625 ibm_generative_ai-2.3.0/src/genai/prompt/__init__.py
--rw-r--r--   0        0        0     9963 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/prompt/prompt_service.py
--rw-r--r--   0        0        0        0 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/py.typed
--rw-r--r--   0        0        0      468 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/request/__init__.py
--rw-r--r--   0        0        0      473 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/request/feedback/__init__.py
--rw-r--r--   0        0        0     5861 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/request/feedback/feedback_service.py
--rw-r--r--   0        0        0     6364 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/request/request_service.py
--rw-r--r--   0        0        0     1191 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/schema/__init__.py
--rw-r--r--   0        0        0    67798 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/schema/_api.py
--rw-r--r--   0        0        0     1607 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/schema/_api_removed_schemas.py
--rw-r--r--   0        0        0    10044 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/schema/_endpoints.py
--rw-r--r--   0        0        0      326 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/schema/_extensions.py
--rw-r--r--   0        0        0      124 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/system_prompt/__init__.py
--rw-r--r--   0        0        0     5478 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/system_prompt/system_prompt_service.py
--rw-r--r--   0        0        0       94 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/tag/__init__.py
--rw-r--r--   0        0        0     1550 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/tag/tag_service.py
--rw-r--r--   0        0        0      119 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/task/__init__.py
--rw-r--r--   0        0        0     1263 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/task/task_service.py
--rw-r--r--   0        0        0      149 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/__init__.py
--rw-r--r--   0        0        0      469 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/chat/__init__.py
--rw-r--r--   0        0        0     8085 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/chat/chat_generation_service.py
--rw-r--r--   0        0        0      462 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/embedding/__init__.py
--rw-r--r--   0        0        0     6873 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/embedding/embedding_service.py
--rw-r--r--   0        0        0      480 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/embedding/limit/__init__.py
--rw-r--r--   0        0        0     2086 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/embedding/limit/limit_service.py
--rw-r--r--   0        0        0        0 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/experimental/__init__.py
--rw-r--r--   0        0        0       76 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/experimental/classification/__init__.py
--rw-r--r--   0        0        0     1480 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/experimental/classification/classification_service.py
--rw-r--r--   0        0        0     1877 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/experimental/experimental_service.py
--rw-r--r--   0        0        0       60 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/experimental/rerank/__init__.py
--rw-r--r--   0        0        0     1483 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/experimental/rerank/rerank_service.py
--rw-r--r--   0        0        0       86 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/experimental/sentence_similarity/__init__.py
--rw-r--r--   0        0        0     1736 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/experimental/sentence_similarity/sentence_similarity_service.py
--rw-r--r--   0        0        0      465 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/generation/__init__.py
--rw-r--r--   0        0        0      661 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/generation/_generation_utils.py
--rw-r--r--   0        0        0      481 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/generation/feedback/__init__.py
--rw-r--r--   0        0        0     5859 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/generation/feedback/feedback_service.py
--rw-r--r--   0        0        0    13934 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/generation/generation_service.py
--rw-r--r--   0        0        0      483 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/generation/limits/__init__.py
--rw-r--r--   0        0        0     2176 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/generation/limits/limit_service.py
--rw-r--r--   0        0        0      465 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/moderation/__init__.py
--rw-r--r--   0        0        0     4641 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/moderation/moderation_service.py
--rw-r--r--   0        0        0     2128 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/text_service.py
--rw-r--r--   0        0        0      471 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/tokenization/__init__.py
--rw-r--r--   0        0        0     5105 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/text/tokenization/tokenization_service.py
--rw-r--r--   0        0        0      427 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/tune/__init__.py
--rw-r--r--   0        0        0     8298 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/tune/tune_service.py
--rw-r--r--   0        0        0      446 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/user/__init__.py
--rw-r--r--   0        0        0     3703 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/user/user_service.py
--rw-r--r--   0        0        0      188 2024-03-22 18:43:52.842625 ibm_generative_ai-2.3.0/src/genai/utils.py
--rw-r--r--   0        0        0     4192 1970-01-01 00:00:00.000000 ibm_generative_ai-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-28 13:16:14.822692 ibm_generative_ai-3.0.0/LICENSE
+-rw-r--r--   0        0        0     2884 2024-05-28 13:16:14.822692 ibm_generative_ai-3.0.0/README.md
+-rw-r--r--   0        0        0     8870 2024-05-28 13:17:39.153635 ibm_generative_ai-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0      347 2024-05-28 13:16:14.830692 ibm_generative_ai-3.0.0/src/genai/__init__.py
+-rw-r--r--   0        0        0     1530 2024-05-28 13:16:14.830692 ibm_generative_ai-3.0.0/src/genai/_types.py
+-rw-r--r--   0        0        0        0 2024-05-28 13:16:14.830692 ibm_generative_ai-3.0.0/src/genai/_utils/__init__.py
+-rw-r--r--   0        0        0     6170 2024-05-28 13:16:14.830692 ibm_generative_ai-3.0.0/src/genai/_utils/api_client.py
+-rw-r--r--   0        0        0     6044 2024-05-28 13:16:14.830692 ibm_generative_ai-3.0.0/src/genai/_utils/async_executor.py
+-rw-r--r--   0        0        0     1514 2024-05-28 13:16:14.830692 ibm_generative_ai-3.0.0/src/genai/_utils/asyncio_future.py
+-rw-r--r--   0        0        0      471 2024-05-28 13:16:14.830692 ibm_generative_ai-3.0.0/src/genai/_utils/deprecation.py
+-rw-r--r--   0        0        0     5704 2024-05-28 13:16:14.830692 ibm_generative_ai-3.0.0/src/genai/_utils/general.py
+-rw-r--r--   0        0        0        0 2024-05-28 13:16:14.830692 ibm_generative_ai-3.0.0/src/genai/_utils/http_client/__init__.py
+-rw-r--r--   0        0        0     3467 2024-05-28 13:16:14.830692 ibm_generative_ai-3.0.0/src/genai/_utils/http_client/httpx_client.py
+-rw-r--r--   0        0        0     3073 2024-05-28 13:16:14.830692 ibm_generative_ai-3.0.0/src/genai/_utils/http_client/rate_limit_transport.py
+-rw-r--r--   0        0        0     7168 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/_utils/http_client/retry_transport.py
+-rw-r--r--   0        0        0     4042 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/_utils/limiters/adjustable_semaphor.py
+-rw-r--r--   0        0        0      532 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/_utils/limiters/base_limiter.py
+-rw-r--r--   0        0        0     1927 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/_utils/limiters/container_limiter.py
+-rw-r--r--   0        0        0      182 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/_utils/limiters/dummy_limiter.py
+-rw-r--r--   0        0        0     2760 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/_utils/limiters/external_limiter.py
+-rw-r--r--   0        0        0     1117 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/_utils/limiters/local_limiter.py
+-rw-r--r--   0        0        0     1034 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/_utils/limiters/shared_limiter.py
+-rw-r--r--   0        0        0      505 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/_utils/queues/flushable_queue.py
+-rw-r--r--   0        0        0     2269 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/_utils/queues/ordered_queue.py
+-rw-r--r--   0        0        0     1276 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/_utils/responses.py
+-rw-r--r--   0        0        0       92 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/_utils/service/__init__.py
+-rw-r--r--   0        0        0     4202 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/_utils/service/base_service.py
+-rw-r--r--   0        0        0     1931 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/_utils/service/metadata.py
+-rw-r--r--   0        0        0     2593 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/_utils/shared_instance.py
+-rw-r--r--   0        0        0     2100 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/_utils/shared_loop.py
+-rw-r--r--   0        0        0     1542 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/_utils/shared_options.py
+-rw-r--r--   0        0        0      575 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/_utils/validators.py
+-rw-r--r--   0        0        0       91 2024-05-28 13:17:39.157635 ibm_generative_ai-3.0.0/src/genai/_version.py
+-rw-r--r--   0        0        0     6179 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/client.py
+-rw-r--r--   0        0        0     2070 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/credentials.py
+-rw-r--r--   0        0        0       95 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/deployment/__init__.py
+-rw-r--r--   0        0        0     4124 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/deployment/deployment_service.py
+-rw-r--r--   0        0        0     2266 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/exceptions.py
+-rw-r--r--   0        0        0       82 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/extensions/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/extensions/_common/__init__.py
+-rw-r--r--   0        0        0     2693 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/extensions/_common/utils.py
+-rw-r--r--   0        0        0      132 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/extensions/huggingface/__init__.py
+-rw-r--r--   0        0        0     2038 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/extensions/huggingface/agent.py
+-rw-r--r--   0        0        0     1342 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/extensions/langchain/__init__.py
+-rw-r--r--   0        0        0    10480 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/extensions/langchain/chat_llm.py
+-rw-r--r--   0        0        0     2867 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/extensions/langchain/embeddings.py
+-rw-r--r--   0        0        0     9758 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/extensions/langchain/llm.py
+-rw-r--r--   0        0        0      498 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/extensions/langchain/template.py
+-rw-r--r--   0        0        0     4855 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/extensions/langchain/utils.py
+-rw-r--r--   0        0        0      249 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/extensions/llama_index/__init__.py
+-rw-r--r--   0        0        0     2419 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/extensions/llama_index/embeddings.py
+-rw-r--r--   0        0        0     8502 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/extensions/llama_index/llm.py
+-rw-r--r--   0        0        0        0 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/extensions/lm_eval/__init__.py
+-rw-r--r--   0        0        0      684 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/extensions/lm_eval/__main__.py
+-rw-r--r--   0        0        0    14432 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/extensions/lm_eval/model.py
+-rw-r--r--   0        0        0      285 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/extensions/localserver/__init__.py
+-rw-r--r--   0        0        0     8807 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/extensions/localserver/local_api_server.py
+-rw-r--r--   0        0        0     1750 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/extensions/localserver/local_base_model.py
+-rw-r--r--   0        0        0     1158 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/extensions/localserver/schema.py
+-rw-r--r--   0        0        0      120 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/file/__init__.py
+-rw-r--r--   0        0        0     9102 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/file/file_service.py
+-rw-r--r--   0        0        0      103 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/folder/__init__.py
+-rw-r--r--   0        0        0     4355 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/folder/folder_service.py
+-rw-r--r--   0        0        0      101 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/model/__init__.py
+-rw-r--r--   0        0        0     2856 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/model/model_service.py
+-rw-r--r--   0        0        0      103 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/prompt/__init__.py
+-rw-r--r--   0        0        0     9963 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/prompt/prompt_service.py
+-rw-r--r--   0        0        0        0 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/py.typed
+-rw-r--r--   0        0        0      127 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/request/__init__.py
+-rw-r--r--   0        0        0      132 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/request/feedback/__init__.py
+-rw-r--r--   0        0        0     5861 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/request/feedback/feedback_service.py
+-rw-r--r--   0        0        0     6364 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/request/request_service.py
+-rw-r--r--   0        0        0      957 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/schema/__init__.py
+-rw-r--r--   0        0        0    71374 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/schema/_api.py
+-rw-r--r--   0        0        0      131 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/schema/_api_removed_schemas.py
+-rw-r--r--   0        0        0    12995 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/schema/_endpoints.py
+-rw-r--r--   0        0        0      326 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/schema/_extensions.py
+-rw-r--r--   0        0        0      124 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/system_prompt/__init__.py
+-rw-r--r--   0        0        0     5478 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/system_prompt/system_prompt_service.py
+-rw-r--r--   0        0        0       94 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/tag/__init__.py
+-rw-r--r--   0        0        0     1550 2024-05-28 13:16:14.834692 ibm_generative_ai-3.0.0/src/genai/tag/tag_service.py
+-rw-r--r--   0        0        0      119 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/task/__init__.py
+-rw-r--r--   0        0        0     1263 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/task/task_service.py
+-rw-r--r--   0        0        0      149 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/__init__.py
+-rw-r--r--   0        0        0      128 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/chat/__init__.py
+-rw-r--r--   0        0        0     7917 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/chat/chat_generation_service.py
+-rw-r--r--   0        0        0      121 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/embedding/__init__.py
+-rw-r--r--   0        0        0     6873 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/embedding/embedding_service.py
+-rw-r--r--   0        0        0      139 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/embedding/limit/__init__.py
+-rw-r--r--   0        0        0     2086 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/embedding/limit/limit_service.py
+-rw-r--r--   0        0        0        0 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/experimental/__init__.py
+-rw-r--r--   0        0        0       76 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/experimental/classification/__init__.py
+-rw-r--r--   0        0        0     1480 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/experimental/classification/classification_service.py
+-rw-r--r--   0        0        0     1877 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/experimental/experimental_service.py
+-rw-r--r--   0        0        0       60 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/experimental/rerank/__init__.py
+-rw-r--r--   0        0        0     1483 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/experimental/rerank/rerank_service.py
+-rw-r--r--   0        0        0       86 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/experimental/sentence_similarity/__init__.py
+-rw-r--r--   0        0        0     1736 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/experimental/sentence_similarity/sentence_similarity_service.py
+-rw-r--r--   0        0        0      124 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/generation/__init__.py
+-rw-r--r--   0        0        0      661 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/generation/_generation_utils.py
+-rw-r--r--   0        0        0    13243 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/generation/generation_service.py
+-rw-r--r--   0        0        0      142 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/generation/limits/__init__.py
+-rw-r--r--   0        0        0     2176 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/generation/limits/limit_service.py
+-rw-r--r--   0        0        0      124 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/moderation/__init__.py
+-rw-r--r--   0        0        0     4080 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/moderation/moderation_service.py
+-rw-r--r--   0        0        0     2128 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/text_service.py
+-rw-r--r--   0        0        0      130 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/tokenization/__init__.py
+-rw-r--r--   0        0        0     5105 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/text/tokenization/tokenization_service.py
+-rw-r--r--   0        0        0       86 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/tune/__init__.py
+-rw-r--r--   0        0        0     8298 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/tune/tune_service.py
+-rw-r--r--   0        0        0      105 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/user/__init__.py
+-rw-r--r--   0        0        0     3703 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/user/user_service.py
+-rw-r--r--   0        0        0      188 2024-05-28 13:16:14.838692 ibm_generative_ai-3.0.0/src/genai/utils.py
+-rw-r--r--   0        0        0     4372 1970-01-01 00:00:00.000000 ibm_generative_ai-3.0.0/PKG-INFO
```

### Comparing `ibm_generative_ai-2.3.0/LICENSE` & `ibm_generative_ai-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/README.md` & `ibm_generative_ai-3.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 ```
 
 
 ### [📚 Documentation](https://ibm.github.io/ibm-generative-ai/)
 
 ### [📚 Examples](https://ibm.github.io/ibm-generative-ai/latest/rst_source/examples.html)
 
+### [📚 V3 Migration Guide](https://ibm.github.io/ibm-generative-ai/latest/v3_migration_guide.html)
+
 ### [📚 V2 Migration Guide](https://ibm.github.io/ibm-generative-ai/latest/v2_migration_guide.html)
 
 
 ## Important Information for Contributors
 - Do you want to contribute to the project? IBM Generative AI is an open-source project that welcomes the community to contribute with documentation, tests, bug corrections, and new functionality in the form of [extensions](EXTENSIONS.md). Please read our [code of conduct](CODE_OF_CONDUCT.md) to learn the expected behavior from participants that contribute to the project, and our [contribution guide](./CONTRIBUTING.md) to learn the gitflow and steps to submit pull requests.
 
 <!-- vscode-markdown-toc-config
```

### Comparing `ibm_generative_ai-2.3.0/pyproject.toml` & `ibm_generative_ai-3.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 maintainers = [
   "Tomas Dvorak <tomas.dvorak@ibm.com>",
   "Radek Jezek <radek.jezek@ibm.com>",
 ]
 description = "IBM Generative AI is a Python library built on IBM's large language model REST interface."
 readme = "README.md"
-version = "2.3.0"
+version = "3.0.0"
 packages = [{include = "genai", from="src"}]
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning>=1.0.0,<2.0.0"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
@@ -29,25 +29,26 @@
 folders = [
   { path = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = "^2.0.0"
-httpx = "^0.26.0"
+httpx = "^0.27.0"
 aiolimiter = "^1.1.0"
-httpx-sse = "^0.3.0"
+httpx-sse = "^0.4.0"
 langchain-core = { version = "^0.1.0", optional = true }
 pyyaml = { version = "^6.0.0", optional = true }
-datasets = { version = "^2.13.0",  optional = true }
 transformers = { version = "^4.33.3",  optional = true, extras=["agents"] }
 llama-index-core = { version = "^0.10.0", optional = true }
 uvicorn = { version = "^0.22.0",  optional = true }
 fastapi = { version = "^0.100.0",  optional = true }
 deprecated = "^1.2.14"
+lm-eval = { version = "^0.4.2",  optional = true }
+tqdm = { version = "^4.66.1", optional = true }
 
 [tool.black] # left for IDE compatibility (pycharm)
 line-length = 120
 
 [tool.ruff]
 line-length = 120
 extend-exclude = ['src/genai/_version.py']
@@ -73,55 +74,58 @@
 "src/genai/schema/_api.py" = ["E501"] # Generated can include long lines
 "tests/unit/docs_examples_generator/assets/**/*.py" = ["T201"] # Allow prints
 
 [tool.ruff.lint.isort]
 known-first-party = ["genai"]
 
 [tool.poetry.group.dev.dependencies]
-python-dotenv = "^1.0.0"
-pytest = "^7.3.2"
+python-dotenv = "^1.0.1"
+datasets = "^2.18.0"
+pytest = "^8.1.1"
 pytest-dotenv = "^0.5.2"
-pre-commit = "^3.3.2"
+pre-commit = "^3.6.2"
 pytest-cov = "^4.1.0"
-sphinx = "^6.1.3"
+sphinx = "^7.2.6"
 furo = "^2024.1.29"
 pytest-asyncio = "^0.21.1"
-pytest-mock = "^3.10.0"
-pytest-httpx = "^0.28.0"
+pytest-mock = "^3.14.0"
 datamodel-code-generator = { version="^0.25.2", extras=["http"] }
-vcrpy = "^6.0.0"
+vcrpy = "^6.0.1"
 pytest-recording = "^0.13.1"
 pytest-subtests = "^0.11.0"
-autodoc_pydantic = "^2.0.0"
+autodoc_pydantic = "^2.1.0"
 ruff = "^0.3.3"
 poethepoet = "^0.24.4"
-pandas = "^2.0.0"
-pyyaml = "^6.0.0"
-tqdm = "^4.66.1"
+pandas = "^2.2.1"
+pyyaml = "^6.0.1"
+tqdm = "^4.66.2"
 sphinx-toolbox = "3.5.0"
 git-changelog = "2.4.0"
 gitchangelog = "3.0.4"
 pystache = "0.6.5"
 tabulate = "0.9.0"
 m2r = "^0.3.1"
 sphinx-multiversion = {path = "external/sphinx_multiversion"}
 sphinx-copybutton = "^0.5.2"
 sphinx-notfound-page = "^1.0.0"
 langchain = "^0.1.4"
-sqlalchemy = "^2.0.25"
+sqlalchemy = "^2.0.28"
+pytest-httpx = "^0.30.0"
 
 
 [tool.poetry.extras]
 langchain = ["langchain-core", "pyyaml"]
 huggingface = ["datasets", "transformers"]
 llama-index = ["llama-index-core"]
+lm-eval = ["lm-eval", "tqdm"]
 localserver = ["uvicorn", "fastapi"]
 
 [tool.pytest.ini_options]
 addopts = "--cov --cov-report term-missing --cov-fail-under 80 -v"
+testpaths = ["tests"]
 markers = [
     "unit",
     "integration",
     "e2e",
     "extension"
 ]
 env_files = [
@@ -147,14 +151,18 @@
 init_typed = true
 warn_required_dynamic_aliases = true
 
 [tool.poe.tasks.install]
 help = "Install dependencies for the SDK core and it's extensions"
 cmd = "poetry install --all-extras --without dev"
 
+[tool.poe.tasks.lm_eval]
+help = "Run lm_eval with support for genai models"
+cmd = "python -m genai.extensions.lm_eval"
+
 [tool.poe.tasks.install-dev]
 help = "Install dependencies and related tooling for development"
 sequence = [{ cmd = "poetry install --all-extras" }, { cmd = "pre-commit install" }]
 deps = ["install"]
 
 [tool.poe.tasks.clean]
 help = "Remove all artifacts and builds"
@@ -241,15 +249,15 @@
     case = "update"
     help = "Update unreleased changelog section"
     env = { "PYTHONPATH" = "scripts" }
     cmd = "python scripts/docs_changelog_generator/generate_changelog.py --debug"
 
     [[tool.poe.tasks.changelog.switch]]
     case = "release"
-    help = "Remove build"
+    help = "Sets version to the latest entry in the CHANGELOG"
     env = { "PYTHONPATH" = "scripts" }
     cmd = "python scripts/docs_changelog_generator/release_changelog.py $version"
 
 [tool.poe.tasks.test]
 args = ["type"]
 control.expr = "type"
```

### Comparing `ibm_generative_ai-2.3.0/src/genai/_types.py` & `ibm_generative_ai-3.0.0/src/genai/_types.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/_utils/api_client.py` & `ibm_generative_ai-3.0.0/src/genai/_utils/api_client.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/_utils/async_executor.py` & `ibm_generative_ai-3.0.0/src/genai/_utils/async_executor.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/_utils/asyncio_future.py` & `ibm_generative_ai-3.0.0/src/genai/_utils/asyncio_future.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/_utils/general.py` & `ibm_generative_ai-3.0.0/src/genai/_utils/general.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/_utils/http_client/httpx_client.py` & `ibm_generative_ai-3.0.0/src/genai/_utils/http_client/httpx_client.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/_utils/http_client/rate_limit_transport.py` & `ibm_generative_ai-3.0.0/src/genai/_utils/http_client/rate_limit_transport.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/_utils/http_client/retry_transport.py` & `ibm_generative_ai-3.0.0/src/genai/_utils/http_client/retry_transport.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/_utils/limiters/adjustable_semaphor.py` & `ibm_generative_ai-3.0.0/src/genai/_utils/limiters/adjustable_semaphor.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/_utils/limiters/base_limiter.py` & `ibm_generative_ai-3.0.0/src/genai/_utils/limiters/base_limiter.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/_utils/limiters/container_limiter.py` & `ibm_generative_ai-3.0.0/src/genai/_utils/limiters/container_limiter.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/_utils/limiters/external_limiter.py` & `ibm_generative_ai-3.0.0/src/genai/_utils/limiters/external_limiter.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/_utils/limiters/local_limiter.py` & `ibm_generative_ai-3.0.0/src/genai/_utils/limiters/local_limiter.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/_utils/limiters/shared_limiter.py` & `ibm_generative_ai-3.0.0/src/genai/_utils/limiters/shared_limiter.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/_utils/queues/ordered_queue.py` & `ibm_generative_ai-3.0.0/src/genai/_utils/queues/ordered_queue.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/_utils/responses.py` & `ibm_generative_ai-3.0.0/src/genai/_utils/responses.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/_utils/service/base_service.py` & `ibm_generative_ai-3.0.0/src/genai/_utils/service/base_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from enum import Enum
 from typing import Generic, Optional, TypeVar, Union, cast
 from urllib.parse import quote
 
 from pydantic import BaseModel, ConfigDict
 
 from genai._utils.api_client import ApiClient
-from genai._utils.deprecated_schema_import import _print_deprecation_warning
+from genai._utils.deprecation import _print_deprecation_warning
 from genai._utils.general import to_model_instance
 from genai._utils.http_client.httpx_client import AsyncHttpxClient, HttpxClient
 from genai._utils.service.metadata import inherit_metadata
 from genai._utils.shared_options import CommonExecutionOptions
 from genai._utils.validators import assert_is_not_empty_string
 from genai.schema._endpoints import ApiEndpoint
```

### Comparing `ibm_generative_ai-2.3.0/src/genai/_utils/service/metadata.py` & `ibm_generative_ai-3.0.0/src/genai/_utils/service/metadata.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/_utils/shared_instance.py` & `ibm_generative_ai-3.0.0/src/genai/_utils/shared_instance.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/_utils/shared_loop.py` & `ibm_generative_ai-3.0.0/src/genai/_utils/shared_loop.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/_utils/shared_options.py` & `ibm_generative_ai-3.0.0/src/genai/_utils/shared_options.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/_utils/validators.py` & `ibm_generative_ai-3.0.0/src/genai/_utils/validators.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/client.py` & `ibm_generative_ai-3.0.0/src/genai/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from genai._utils.general import to_model_instance
 from genai._utils.service import (
     BaseService,
     BaseServiceConfig,
     BaseServiceServices,
 )
 from genai.credentials import Credentials
+from genai.deployment import DeploymentService as _DeploymentService
 from genai.file import FileService as _FileService
 from genai.folder import FolderService as _FolderService
 from genai.model import ModelService as _ModelService
 from genai.prompt import PromptService as _PromptService
 from genai.request import RequestService as _RequestService
 from genai.system_prompt import SystemPromptService as _SystemPromptService
 from genai.tag import TagService as _TagService
@@ -37,14 +38,15 @@
     FileService: type[_FileService] = _FileService
     PromptService: type[_PromptService] = _PromptService
     SystemPromptService: type[_SystemPromptService] = _SystemPromptService
     UserService: type[_UserService] = _UserService
     TagService: type[_TagService] = _TagService
     FolderService: type[_FolderService] = _FolderService
     TaskService: type[_TaskService] = _TaskService
+    DeploymentService: type[_DeploymentService] = _DeploymentService
 
 
 class BaseConfig(BaseServiceConfig):
     """Client's configuration model"""
 
     api_client_config: Optional[ModelLike[ApiClientConfig]] = None
 
@@ -140,7 +142,8 @@
         self.file = services.FileService(api_client=api_client)
         self.prompt = services.PromptService(api_client=api_client)
         self.system_prompt = services.SystemPromptService(api_client=api_client)
         self.user = services.UserService(api_client=api_client)
         self.tag = services.TagService(api_client=api_client)
         self.folder = services.FolderService(api_client=api_client)
         self.task = services.TaskService(api_client=api_client)
+        self.deployment = services.DeploymentService(api_client=api_client)
```

### Comparing `ibm_generative_ai-2.3.0/src/genai/credentials.py` & `ibm_generative_ai-3.0.0/src/genai/credentials.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/exceptions.py` & `ibm_generative_ai-3.0.0/src/genai/exceptions.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/extensions/_common/utils.py` & `ibm_generative_ai-3.0.0/src/genai/extensions/_common/utils.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/extensions/huggingface/agent.py` & `ibm_generative_ai-3.0.0/src/genai/extensions/huggingface/agent.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/extensions/langchain/__init__.py` & `ibm_generative_ai-3.0.0/src/genai/extensions/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/extensions/langchain/chat_llm.py` & `ibm_generative_ai-3.0.0/src/genai/extensions/langchain/chat_llm.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         from genai.extensions.langchain import LangChainChatInterface
         from langchain_core.messages import HumanMessage, SystemMessage
         from genai.schema import TextGenerationParameters
 
         client = Client(credentials=Credentials.from_env())
         llm = LangChainChatInterface(
             client=client,
-            model_id="meta-llama/llama-2-70b-chat",
+            model_id="meta-llama/llama-3-70b-instruct",
             parameters=TextGenerationParameters(
                 max_new_tokens=250,
             )
         )
 
         response = chat_model.generate(messages=[HumanMessage(content="Hello world!")])
         print(response)
@@ -178,16 +178,16 @@
                     generation_info=generation_info,
                 )
                 yield chunk
                 if run_manager:
                     run_manager.on_llm_new_token(token=text, chunk=chunk, response=response)  # noqa: B023
                     # Function definition does not bind loop variable `response`: linter is probably just confused here
 
-            if response.moderation:
-                generation_info = create_generation_info_from_response(response, result=response.moderation)
+            if response.moderations:
+                generation_info = create_generation_info_from_response(response, result=response.moderations)
                 yield from send_chunk(generation_info=generation_info)
 
             for result in response.results or []:
                 generation_info = create_generation_info_from_response(response, result=result)
                 yield from send_chunk(text=result.generated_text or "", generation_info=generation_info)
 
     def _generate(
```

### Comparing `ibm_generative_ai-2.3.0/src/genai/extensions/langchain/embeddings.py` & `ibm_generative_ai-3.0.0/src/genai/extensions/langchain/embeddings.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,13 +64,14 @@
         return await run_in_executor(None, self.embed_documents, texts)
 
     def _get_embeddings(self, texts: list[str]) -> list[list[float]]:
         embeddings: list[list[float]] = []
         for response in self.client.text.embedding.create(
             model_id=self.model_id, inputs=texts, parameters=self.parameters, execution_options=self.execution_options
         ):
-            embeddings.extend(response.results)
+            embedding_list = [result.embedding for result in response.results]
+            embeddings.extend(embedding_list)
 
         return embeddings
 
 
 LangChainEmbeddingsInterface.model_rebuild()
```

### Comparing `ibm_generative_ai-2.3.0/src/genai/extensions/langchain/llm.py` & `ibm_generative_ai-3.0.0/src/genai/extensions/langchain/llm.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         from genai import Client, Credentials
         from genai.extensions.langchain import LangChainInterface
         from genai.schema import TextGenerationParameters
 
         client = Client(credentials=Credentials.from_env())
         llm = LangChainInterface(
             client=client,
-            model_id="meta-llama/llama-2-70b-chat",
+            model_id="meta-llama/llama-3-70b-instruct",
             parameters=TextGenerationParameters(max_new_tokens=50)
         )
 
         response = chat_model.generate(prompts=["Hello world!"])
         print(response)
     """
 
@@ -237,15 +237,15 @@
             yield chunk
             if run_manager:
                 run_manager.on_llm_new_token(token=chunk.text, chunk=chunk, response=response)
 
         for response in self.client.text.generation.create_stream(
             **self._prepare_stream_request(input=prompt, stop=stop, **kwargs)
         ):
-            if response.moderation:
+            if response.moderations:
                 generation_info = create_generation_info_from_response(response, result=response.moderation)
                 yield from send_chunk(generation_info=generation_info, response=response)
 
             for result in response.results or []:
                 generation_info = create_generation_info_from_response(response, result=result)
                 yield from send_chunk(text=result.generated_text, generation_info=generation_info, response=response)
```

### Comparing `ibm_generative_ai-2.3.0/src/genai/extensions/langchain/utils.py` & `ibm_generative_ai-3.0.0/src/genai/extensions/langchain/utils.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/extensions/llama_index/embeddings.py` & `ibm_generative_ai-3.0.0/src/genai/extensions/llama_index/embeddings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import asyncio
 from typing import Optional
 
+from pydantic import Field
+
 from genai._types import ModelLike
 from genai.client import Client
 from genai.schema import TextEmbeddingParameters
 from genai.text.embedding.embedding_service import CreateExecutionOptions
 
 try:
     from llama_index.core.base.embeddings.base import BaseEmbedding, Embedding
@@ -13,14 +15,17 @@
 
 
 class IBMGenAILlamaIndexEmbedding(BaseEmbedding):
     client: Client
     model_id: str
     parameters: Optional[ModelLike[TextEmbeddingParameters]] = None
     execution_options: Optional[ModelLike[CreateExecutionOptions]] = None
+    # Batch size is set to 100000 to avoid batching in
+    # LlamaIndex as it is handled by the SDK itself
+    embed_batch_size: int = Field(default=10000, description="The batch size for embedding calls.", gt=0)
 
     @classmethod
     def class_name(cls) -> str:
         return "IBMGenAIEmbedding"
 
     def _get_query_embedding(self, query: str) -> Embedding:
         response = self._get_embeddings([query])
@@ -44,10 +49,11 @@
         return await asyncio.get_running_loop().run_in_executor(None, self._get_text_embeddings, texts)
 
     def _get_embeddings(self, texts: list[str]) -> list[Embedding]:
         embeddings: list[list[float]] = []
         for response in self.client.text.embedding.create(
             model_id=self.model_id, inputs=texts, parameters=self.parameters, execution_options=self.execution_options
         ):
-            embeddings.extend(response.results)
+            embedding_list = [result.embedding for result in response.results]
+            embeddings.extend(embedding_list)
 
         return embeddings
```

### Comparing `ibm_generative_ai-2.3.0/src/genai/extensions/llama_index/llm.py` & `ibm_generative_ai-3.0.0/src/genai/extensions/llama_index/llm.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,16 +188,16 @@
     @llm_chat_callback()
     def stream_chat(self, messages: Sequence[ChatMessage], formatted: bool = False, **kwargs: Any) -> ChatResponseGen:
         text = ""
 
         for response in self.client.text.chat.create_stream(
             **self._prepare_request(self._identifying_chat_params)(messages=to_genai_messages(messages), **kwargs)
         ):
-            if response.moderation:
-                generation_info = create_generation_info_from_response(response, result=response.moderation)
+            if response.moderations:
+                generation_info = create_generation_info_from_response(response, result=response.moderations)
                 message = ChatMessage(role=MessageRole.ASSISTANT, content=text)
                 yield ChatResponse(message=message, delta="", additional_kwargs=generation_info)
 
             for result in response.results or []:
                 generated_text = result.generated_text or ""
                 generation_info = create_generation_info_from_response(response, result=result)
                 text += generated_text
```

### Comparing `ibm_generative_ai-2.3.0/src/genai/extensions/localserver/local_api_server.py` & `ibm_generative_ai-3.0.0/src/genai/extensions/localserver/local_api_server.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/extensions/localserver/local_base_model.py` & `ibm_generative_ai-3.0.0/src/genai/extensions/localserver/local_base_model.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/extensions/localserver/schema.py` & `ibm_generative_ai-3.0.0/src/genai/extensions/localserver/schema.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/file/file_service.py` & `ibm_generative_ai-3.0.0/src/genai/file/file_service.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/folder/folder_service.py` & `ibm_generative_ai-3.0.0/src/genai/folder/folder_service.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/model/model_service.py` & `ibm_generative_ai-3.0.0/src/genai/model/model_service.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/prompt/prompt_service.py` & `ibm_generative_ai-3.0.0/src/genai/prompt/prompt_service.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/request/feedback/feedback_service.py` & `ibm_generative_ai-3.0.0/src/genai/request/feedback/feedback_service.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/request/request_service.py` & `ibm_generative_ai-3.0.0/src/genai/request/request_service.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/schema/_api.py` & `ibm_generative_ai-3.0.0/src/genai/schema/_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # generated by datamodel-codegen:
-#   filename:  2024-03-22_openapi_schema
+#   filename:  2024-05-22_openapi_schema
 
 from __future__ import annotations
 
 from datetime import date
 from enum import Enum
 from typing import Any, Literal, Optional, Union
 
-import deprecated
-from pydantic import AwareDatetime, Field, RootModel, computed_field, field_validator
+from pydantic import AwareDatetime, Field, RootModel
 
 from genai._types import ApiBaseModel
-from genai._utils.deprecated_schema_import import _print_deprecation_warning
 
 
 class ApiKeyResult(ApiBaseModel):
     created_at: AwareDatetime
     generated_at: AwareDatetime
     last_used_at: Optional[AwareDatetime] = None
     value: str
@@ -34,19 +32,14 @@
 
 
 class BaseMessage(ApiBaseModel):
     content: str
     files: Optional[list[MessageFile]] = None
     role: ChatRole
 
-    @computed_field
-    @deprecated.deprecated(reason="'file_ids' property is deprecated, use 'files' instead!")
-    def file_ids(self) -> Optional[list[str]]:
-        return [file.id for file in self.files] if self.files is not None else None
-
 
 class BaseTokens(ApiBaseModel):
     logprob: Optional[Union[float, str]] = None
     rank: Optional[int] = None
     text: Optional[str] = None
     top_tokens: Optional[list[GeneratedToken]] = None
 
@@ -63,14 +56,138 @@
 
 
 class DecodingMethod(str, Enum):
     GREEDY = "greedy"
     SAMPLE = "sample"
 
 
+class DeploymentResult(ApiBaseModel):
+    created_at: AwareDatetime
+    deployed_at: Optional[AwareDatetime] = None
+    expires_at: Optional[AwareDatetime] = None
+    id: str
+    status: DeploymentStatus
+    tune_id: Optional[str] = None
+    updated_at: AwareDatetime
+
+
+class DeploymentStatus(str, Enum):
+    QUEUED = "queued"
+    INITIALIZING = "initializing"
+    READY = "ready"
+    FAILED = "failed"
+    EXPIRED = "expired"
+
+
+class EvaluationExperiment(ApiBaseModel):
+    created_at: AwareDatetime
+    description: Optional[str] = None
+    evaluations_count: float
+    file: Optional[EvaluationFile] = None
+    id: str
+    name: str
+    task: EvaluationTask
+    template_id: str
+
+
+class EvaluationExperimentSortBy(str, Enum):
+    NAME = "name"
+    ID = "id"
+    TEMPLATE = "template"
+
+
+class EvaluationFieldOperation(ApiBaseModel):
+    type: EvaluationOperationType
+
+
+class EvaluationFile(ApiBaseModel):
+    bytes: int
+    created_at: AwareDatetime
+    file_name: str
+    id: str
+    metadata: Optional[FileMetadata] = None
+
+
+class EvaluationInstanceResult(ApiBaseModel):
+    generation_info: Optional[dict[str, Any]] = Field(None, title="Generation Info")
+    score: dict[str, Any]
+
+
+class EvaluationLimit(ApiBaseModel):
+    concurrency: ConcurrencyLimit
+
+
+class EvaluationOperationType(str, Enum):
+    RENAME_FIELDS = "rename_fields"
+    ADD_FIELDS = "add_fields"
+    SHUFFLE = "shuffle"
+
+
+class EvaluationParentTask(ApiBaseModel):
+    id: str
+    name: str
+
+
+class EvaluationPrompt(ApiBaseModel):
+    id: str
+    input: Optional[str] = None
+    metadata: Optional[dict[str, Any]] = None
+    name: str
+
+
+class EvaluationResult(ApiBaseModel):
+    created_at: AwareDatetime
+    description: Optional[str] = None
+    experiment_id: str
+    file: Optional[EvaluationFile] = None
+    finished_at: Optional[AwareDatetime] = None
+    id: str
+    model_id: str
+    name: str
+    parameters: Optional[dict[str, Any]] = None
+    prompt: EvaluationPrompt
+    result: dict[str, Any]
+    started_at: Optional[AwareDatetime] = None
+    status: EvaluationStatus
+    status_message: Optional[str] = None
+    task_id: str
+    template_id: str
+    template_name: str
+
+
+class EvaluationSortBy(str, Enum):
+    NAME = "name"
+    ID = "id"
+    TEMPLATE = "template"
+
+
+class EvaluationStatus(str, Enum):
+    PENDING = "pending"
+    QUEUED = "queued"
+    RUNNING = "running"
+    COMPLETED = "completed"
+    FAILED = "failed"
+
+
+class EvaluationTask(ApiBaseModel):
+    id: str
+    name: str
+    parent_task: Optional[EvaluationParentTask] = None
+
+
+class EvaluationTemplate(ApiBaseModel):
+    dataset_fields: dict[str, Any]
+    default_prompt_ids: Optional[list[str]] = None
+    id: str
+    metrics: list[Union[list[Metric], Metrics]]
+    name: str
+    postprocessors: list[str]
+    task: Optional[EvaluationTask] = None
+
+
 class Extensions(BaseErrorExtension):
     code: Literal["INVALID_INPUT"] = "INVALID_INPUT"
 
 
 class Extensions1(BaseErrorExtension):
     code: Literal["INTERNAL_SERVER_ERROR"] = "INTERNAL_SERVER_ERROR"
 
@@ -101,28 +218,39 @@
 
 
 class FileListSortBy(str, Enum):
     NAME = "name"
     CREATED_AT = "created_at"
 
 
+class FileMetadata(ApiBaseModel):
+    stats: FileMetadataStats
+
+
+class FileMetadataStats(ApiBaseModel):
+    columns: list[str]
+    records_count: float
+
+
 class FilePurpose(str, Enum):
     TUNE = "tune"
     TEMPLATE = "template"
     TUNE_IMPORT = "tune_import"
     EXTRACTION = "extraction"
+    GENERIC_STRUCTURED = "generic_structured"
 
 
 class FileResult(ApiBaseModel):
     bytes: int
     created_at: AwareDatetime
     descendants: Optional[list[FileDescendant]] = None
     file_formats: Optional[list[FileFormat]] = None
     file_name: str
     id: str
+    metadata: Optional[FileMetadata] = None
     origin: Optional[FileDescendant] = None
     purpose: FilePurpose
     storage_provider_location: StorageProviderLocation
     updated_at: AwareDatetime
 
 
 class FolderResult(ApiBaseModel):
@@ -163,14 +291,24 @@
 
 
 class MessageFile(ApiBaseModel):
     content: Optional[str] = None
     id: Optional[str] = None
 
 
+class Metric(ApiBaseModel):
+    description: str
+    id: str
+    name: str
+
+
+class Metrics(ApiBaseModel):
+    pass
+
+
 class ModelFacet(ApiBaseModel):
     id: str
     name: str
     type: ModelFacetType
 
 
 class ModelFacetType(str, Enum):
@@ -188,20 +326,22 @@
     system_prompt: Optional[str] = None
 
 
 class ModelIdRetrieveResult(ApiBaseModel):
     description: Optional[str] = None
     developer: Optional[str] = None
     disabled: bool
+    facets: Optional[list[ModelFacet]] = None
     id: str
     is_live: bool
     label: str
     model_family: ModelFamily
     name: str
     preferred: bool
+    prompt_builder_example: Optional[dict[str, Any]] = None
     size: str
     source_model_id: Optional[str] = None
     system_prompt: Optional[str] = None
     system_prompt_id: Optional[int] = None
     tags: list[str]
     tasks: list[Tasks]
     token_limits: list[ModelTokenLimits]
@@ -231,57 +371,14 @@
     TUNE = "tune"
 
 
 class ModerationHAP(ApiBaseModel):
     input: Optional[ModerationHAPInput] = None
     output: Optional[ModerationHAPOutput] = None
 
-    # TODO: remove in next major release
-    @field_validator("input", mode="before")
-    @classmethod
-    def _validate_input(cls, value: Any):
-        if isinstance(value, bool):
-            _print_deprecation_warning(
-                "(ModerationHAP): passing boolean value to the 'input' parameter is deprecated, use 'ModerationHAPInput' class instead."
-            )
-            return ModerationHAPInput(enabled=value)
-        else:
-            return value
-
-    # TODO: remove in next major release
-    @field_validator("output", mode="before")
-    @classmethod
-    def _validate_output(cls, value: Any):
-        if isinstance(value, bool):
-            _print_deprecation_warning(
-                "(ModerationHAP): passing boolean value to the 'output' parameter is deprecated, use 'ModerationHAPOutput' class instead."
-            )
-            return ModerationHAPOutput(enabled=value)
-        else:
-            return value
-
-    # TODO: remove in next major release
-    def model_post_init(self, __context: Any) -> None:
-        deprecated_attrs = {
-            name: getattr(self, name) for name in ["threshold", "send_tokens"] if getattr(self, name, None) is not None
-        }
-        if deprecated_attrs:
-            if self.input is None:
-                self.input = ModerationHAPInput(enabled=True)
-            if self.output is None:
-                self.output = ModerationHAPOutput(enabled=True)
-
-            for name, value in deprecated_attrs.items():
-                _print_deprecation_warning(
-                    f"(ModerationHAP): '{name}' is deprecated! Use 'input' parameter (ModerationHAPInput) / 'output' parameter parameter (ModerationHAPOutput) instead.",
-                )
-                setattr(self.input, name, value)
-                setattr(self.output, name, value)
-                delattr(self, name)
-
 
 class ModerationHAPInput(ApiBaseModel):
     enabled: Optional[bool] = False
     """
     Detects HAP (hateful, abusive, or profane language).
     """
     send_tokens: Optional[bool] = False
@@ -303,118 +400,31 @@
     """
 
 
 class ModerationImplicitHate(ApiBaseModel):
     input: Optional[ModerationImplicitHateInput] = None
     output: Optional[ModerationImplicitHateOutput] = None
 
-    # TODO: remove in next major release
-    @field_validator("input", mode="before")
-    @classmethod
-    def _validate_input(cls, value: Any):
-        if isinstance(value, bool):
-            _print_deprecation_warning(
-                "(ModerationImplicitHate): passing boolean value to the 'input' parameter is deprecated, use 'ModerationImplicitHateInput' class instead."
-            )
-            return ModerationImplicitHateInput(enabled=value)
-        else:
-            return value
-
-    # TODO: remove in next major release
-    @field_validator("output", mode="before")
-    @classmethod
-    def _validate_output(cls, value: Any):
-        if isinstance(value, bool):
-            _print_deprecation_warning(
-                "(ModerationImplicitHate): passing boolean value to the 'output' parameter is deprecated, use 'ModerationImplicitHateOutput' class instead."
-            )
-            return ModerationImplicitHateOutput(enabled=value)
-        else:
-            return value
-
-    # TODO: remove in next major release
-    def model_post_init(self, __context: Any) -> None:
-        deprecated_attrs = {
-            name: getattr(self, name) for name in ["threshold", "send_tokens"] if getattr(self, name, None) is not None
-        }
-        if deprecated_attrs:
-            if self.input is None:
-                self.input = ModerationImplicitHateInput(enabled=True)
-            if self.output is None:
-                self.output = ModerationImplicitHateOutput(enabled=True)
-
-            for name, value in deprecated_attrs.items():
-                _print_deprecation_warning(
-                    f"(ModerationImplicitHate): '{name}' is deprecated! Use 'input' parameter (ModerationImplicitHateInput) / 'output' parameter parameter (ModerationImplicitHateOutput) instead.",
-                )
-                setattr(self.input, name, value)
-                setattr(self.output, name, value)
-                delattr(self, name)
-
 
 class ModerationImplicitHateInput(ApiBaseModel):
-    enabled: bool = False
-    send_tokens: Optional[bool] = False
+    enabled: bool
+    send_tokens: Optional[bool] = None
     threshold: Optional[float] = Field(0.75, gt=0.0, lt=1.0)
 
 
 class ModerationImplicitHateOutput(ApiBaseModel):
-    enabled: bool = False
-    send_tokens: Optional[bool] = False
+    enabled: bool
+    send_tokens: Optional[bool] = None
     threshold: Optional[float] = Field(0.75, gt=0.0, lt=1.0)
 
 
 class ModerationParameters(ApiBaseModel):
     hap: Optional[ModerationHAP] = None
     social_bias: Optional[ModerationSocialBias] = None
 
-    # TODO: remove in next major release
-    def model_post_init(self, __context: Any) -> None:
-        for name in ["stigma", "implicit_hate"]:
-            if hasattr(self, name):
-                _print_deprecation_warning(
-                    f'({type(self).__name__}): "{name}" has been deprecated, use "social_bias" instead.'
-                )
-
-    # TODO: remove in next major release
-    def remove_deprecated(self) -> None:
-        """Remove attributes which are not supported anymore"""
-        for name in ["stigma", "implicit_hate"]:
-            if hasattr(self, name):
-                _print_deprecation_warning(
-                    f'({type(self).__name__} class): "{name}" has been deprecated, use "social_bias" instead.',
-                )
-                delattr(self, name)
-
-    # TODO: remove in next major release
-    @field_validator("hap", mode="before")
-    @classmethod
-    def _validate_hap(cls, value: Any):
-        if isinstance(value, bool):
-            _print_deprecation_warning(
-                "(ModerationParameters): passing boolean value to the 'hap' parameter is deprecated, use 'ModerationHAP' class instead."
-            )
-            return ModerationHAP(input=ModerationHAPInput(enabled=value), output=ModerationHAPOutput(enabled=value))
-        else:
-            return value
-
-    # TODO: remove in next major release
-    @field_validator("social_bias", mode="before")
-    @classmethod
-    def _validate_social_bias(cls, value: Any):
-        if isinstance(value, bool):
-            _print_deprecation_warning(
-                "(ModerationParameters): passing boolean value to the 'social_bias' parameter is deprecated, use 'ModerationSocialBias' class instead."
-            )
-            return ModerationSocialBias(
-                input=ModerationSocialBiasInput(enabled=value), output=ModerationSocialBiasOutput(enabled=value)
-            )
-        else:
-            return value
-
 
 class ModerationPosition(ApiBaseModel):
     end: int
     start: int
 
 
 class ModerationSocialBias(ApiBaseModel):
@@ -446,67 +456,24 @@
     """
 
 
 class ModerationStigma(ApiBaseModel):
     input: Optional[ModerationStigmaInput] = None
     output: Optional[ModerationStigmaOutput] = None
 
-    # TODO: remove in next major release
-    @field_validator("input", mode="before")
-    @classmethod
-    def _validate_input(cls, value: Any):
-        if isinstance(value, bool):
-            _print_deprecation_warning(
-                "(ModerationStigma): passing boolean value to the 'input' parameter is deprecated, use 'ModerationStigmaInput' class instead."
-            )
-            return ModerationStigmaInput(enabled=value)
-        else:
-            return value
-
-    # TODO: remove in next major release
-    @field_validator("output", mode="before")
-    @classmethod
-    def _validate_output(cls, value: Any):
-        if isinstance(value, bool):
-            _print_deprecation_warning(
-                "(ModerationStigma): passing boolean value to the 'output' parameter is deprecated, use 'ModerationStigmaOutput' class instead."
-            )
-            return ModerationStigmaOutput(enabled=value)
-        else:
-            return value
-
-    # TODO: remove in next major release
-    def model_post_init(self, __context: Any) -> None:
-        deprecated_attrs = {
-            name: getattr(self, name) for name in ["threshold", "send_tokens"] if getattr(self, name, None) is not None
-        }
-        if deprecated_attrs:
-            if self.input is None:
-                self.input = ModerationStigmaInput(enabled=True)
-            if self.output is None:
-                self.output = ModerationStigmaOutput(enabled=True)
-
-            for name, value in deprecated_attrs.items():
-                _print_deprecation_warning(
-                    f"(ModerationStigma): '{name}' is deprecated! Use 'input' parameter (ModerationStigmaInput) / 'output' parameter parameter (ModerationStigmaOutput) instead.",
-                )
-                setattr(self.input, name, value)
-                setattr(self.output, name, value)
-                delattr(self, name)
-
 
 class ModerationStigmaInput(ApiBaseModel):
-    enabled: bool = False
-    send_tokens: Optional[bool] = False
+    enabled: bool
+    send_tokens: Optional[bool] = None
     threshold: Optional[float] = Field(0.75, gt=0.0, lt=1.0)
 
 
 class ModerationStigmaOutput(ApiBaseModel):
-    enabled: bool = False
-    send_tokens: Optional[bool] = False
+    enabled: bool
+    send_tokens: Optional[bool] = None
     threshold: Optional[float] = Field(0.75, gt=0.0, lt=1.0)
 
 
 class ModerationTokens(ApiBaseModel):
     index: Optional[int] = None
     score: Optional[float] = None
     token: Optional[str] = None
@@ -529,39 +496,199 @@
     version: Literal["2023-11-22"] = "2023-11-22"
 
 
 class ApiKeyRetrieveResponse(ApiBaseModel):
     result: Optional[ApiKeyResult] = None
 
 
-class _BetaTimeSerieForecastingCreateParametersQuery(ApiBaseModel):
+class _DeploymentCreateParametersQuery(ApiBaseModel):
     version: Literal["2023-11-22"] = "2023-11-22"
 
 
-class _BetaTimeSerieForecastingCreateRequest(ApiBaseModel):
-    columns: _BetaTimeSerieForecastingCreateRequestColumns
-    data: str
-    future_data: str
-    model_id: str
+class _DeploymentCreateRequest(ApiBaseModel):
+    tune_id: str
+
+
+class DeploymentCreateResponse(ApiBaseModel):
+    result: DeploymentResult
+
+
+class _DeploymentIdDeleteParametersQuery(ApiBaseModel):
+    version: Literal["2023-11-22"] = "2023-11-22"
+
+
+class _DeploymentIdRetrieveParametersQuery(ApiBaseModel):
+    version: Literal["2023-11-22"] = "2023-11-22"
+
+
+class DeploymentIdRetrieveResponse(ApiBaseModel):
+    result: DeploymentResult
+
+
+class _DeploymentRetrieveParametersQuery(ApiBaseModel):
+    id: Optional[list[str]] = None
+    limit: Optional[int] = Field(100, ge=1, le=100)
+    offset: Optional[int] = Field(0, ge=0)
+    version: Literal["2023-11-22"] = "2023-11-22"
 
 
-class BetaTimeSerieForecastingCreateResponse(ApiBaseModel):
-    result: _BetaTimeSerieForecastingCreateResult
+class DeploymentRetrieveResponse(ApiBaseModel):
+    results: list[DeploymentResult]
+    total_count: float
 
 
-class _BetaTimeSerieLimitRetrieveParametersQuery(ApiBaseModel):
+class _EvaluationCreateParametersQuery(ApiBaseModel):
     version: Literal["2023-11-22"] = "2023-11-22"
 
 
-class BetaTimeSerieLimitRetrieveResponse(ApiBaseModel):
-    result: _BetaTimeSerieLimitRetrieveResult
+class _EvaluationCreateRequest(ApiBaseModel):
+    dataset_file_id: str
+    description: Optional[str] = None
+    experiment_id: Optional[str] = None
+    field_operations: Optional[list[EvaluationFieldOperation]] = None
+    metrics: list[str]
+    model_id: Optional[str] = None
+    name: str
+    parameters: Optional[TextGenerationParameters] = None
+    postprocessors: Optional[list[str]] = None
+    prompt_id: str
+    template_id: str
+
+
+class EvaluationCreateResponse(ApiBaseModel):
+    result: EvaluationResult
+
+
+class _EvaluationExperimentCreateParametersQuery(ApiBaseModel):
+    version: Literal["2023-11-22"] = "2023-11-22"
+
+
+class _EvaluationExperimentCreateRequest(ApiBaseModel):
+    dataset_file_id: str
+    description: Optional[str] = None
+    name: str
+    template_id: str
+
+
+class EvaluationExperimentCreateResponse(ApiBaseModel):
+    result: EvaluationExperiment
+
+
+class _EvaluationExperimentIdDeleteParametersQuery(ApiBaseModel):
+    version: Literal["2023-11-22"] = "2023-11-22"
+
+
+class _EvaluationExperimentIdRetrieveParametersQuery(ApiBaseModel):
+    version: Literal["2023-11-22"] = "2023-11-22"
+
+
+class EvaluationExperimentIdRetrieveResponse(ApiBaseModel):
+    result: EvaluationResult
+
+
+class _EvaluationExperimentRetrieveParametersQuery(ApiBaseModel):
+    limit: Optional[int] = Field(100, ge=1, le=100)
+    offset: Optional[int] = Field(0, ge=0)
+    sort_by: Optional[EvaluationExperimentSortBy] = None
+    direction: Optional[SortDirection] = None
+    version: Literal["2023-11-22"] = "2023-11-22"
+
+
+class EvaluationExperimentRetrieveResponse(ApiBaseModel):
+    results: list[EvaluationExperiment]
+    total_count: int
+
+
+class _EvaluationIdDeleteParametersQuery(ApiBaseModel):
+    version: Literal["2023-11-22"] = "2023-11-22"
+
+
+class _EvaluationIdInstanceResultRetrieveParametersQuery(ApiBaseModel):
+    limit: Optional[int] = Field(100, ge=1, le=100)
+    offset: Optional[int] = Field(0, ge=0)
+    version: Literal["2023-11-22"] = "2023-11-22"
+
+
+class EvaluationIdInstanceResultRetrieveResponse(ApiBaseModel):
+    results: list[EvaluationInstanceResult]
+    total_count: int
+
+
+class _EvaluationIdRetrieveParametersQuery(ApiBaseModel):
+    version: Literal["2023-11-22"] = "2023-11-22"
+
+
+class EvaluationIdRetrieveResponse(ApiBaseModel):
+    result: EvaluationResult
+
+
+class _EvaluationLimitRetrieveParametersQuery(ApiBaseModel):
+    version: Literal["2023-11-22"] = "2023-11-22"
+
+
+class EvaluationLimitRetrieveResponse(ApiBaseModel):
+    result: EvaluationLimit
+
+
+class _EvaluationPreviewCreateParametersQuery(ApiBaseModel):
+    limit: Optional[int] = Field(3, ge=1, le=10)
+    version: Literal["2023-11-22"] = "2023-11-22"
+
+
+class _EvaluationPreviewCreateRequest(ApiBaseModel):
+    dataset_file_id: str
+    description: Optional[str] = None
+    experiment_id: Optional[str] = None
+    field_operations: Optional[list[EvaluationFieldOperation]] = None
+    metrics: list[str]
+    model_id: Optional[str] = None
+    name: str
+    parameters: Optional[TextGenerationParameters] = None
+    postprocessors: Optional[list[str]] = None
+    prompt_id: str
+    template_id: str
+
+
+class EvaluationPreviewCreateResponse(ApiBaseModel):
+    results: list[EvaluationInstanceResult]
+    total_count: int
+
+
+class _EvaluationRetrieveParametersQuery(ApiBaseModel):
+    limit: Optional[int] = Field(100, ge=1, le=100)
+    offset: Optional[int] = Field(0, ge=0)
+    sort_by: Optional[EvaluationSortBy] = None
+    direction: Optional[SortDirection] = None
+    experiment_id: Optional[str] = None
+    version: Literal["2023-11-22"] = "2023-11-22"
+
+
+class EvaluationRetrieveResponse(ApiBaseModel):
+    results: list[EvaluationResult]
+    total_count: int
+
+
+class _EvaluationTemplateIdRetrieveParametersQuery(ApiBaseModel):
+    version: Literal["2023-11-22"] = "2023-11-22"
+
+
+class EvaluationTemplateIdRetrieveResponse(ApiBaseModel):
+    result: EvaluationTemplate
+
+
+class _EvaluationTemplateRetrieveParametersQuery(ApiBaseModel):
+    version: Literal["2023-11-22"] = "2023-11-22"
+
+
+class EvaluationTemplateRetrieveResponse(ApiBaseModel):
+    results: list[EvaluationTemplate]
 
 
 class _FileCreateParametersQuery(ApiBaseModel):
-    version: Literal["2023-12-15"] = "2023-12-15"
+    version: Literal["2024-05-13"] = "2024-05-13"
 
 
 class _FileCreateRequest(ApiBaseModel):
     file: bytes
     origin_id: Optional[str] = None
     purpose: FilePurpose
 
@@ -587,30 +714,30 @@
 
 
 class FileIdPatchResponse(ApiBaseModel):
     result: FileResult
 
 
 class _FileIdRetrieveParametersQuery(ApiBaseModel):
-    version: Literal["2023-12-15"] = "2023-12-15"
+    version: Literal["2024-05-13"] = "2024-05-13"
 
 
 class FileIdRetrieveResponse(ApiBaseModel):
     result: FileResult
 
 
 class _FileRetrieveParametersQuery(ApiBaseModel):
     limit: Optional[int] = Field(100, ge=1, le=100)
     offset: Optional[int] = Field(0, ge=0)
     sort_by: Optional[FileListSortBy] = None
     direction: Optional[SortDirection] = None
     search: Optional[str] = None
     purpose: Optional[FilePurpose] = None
     format_id: Optional[int] = None
-    version: Literal["2023-12-15"] = "2023-12-15"
+    version: Literal["2024-05-13"] = "2024-05-13"
 
 
 class FileRetrieveResponse(ApiBaseModel):
     results: list[FileResult]
     total_count: int
 
 
@@ -1007,19 +1134,14 @@
     created_at: Optional[AwareDatetime] = None
     id: Optional[str] = None
     input_parameters: Optional[dict[str, Any]] = None
     model_id: Optional[str] = None
     moderations: Optional[TextCreateResponseModeration] = None
     results: Optional[list[TextChatGenerationStreamResult]] = None
 
-    @computed_field
-    @deprecated.deprecated(reason="'moderation' property is deprecated, use 'moderations' instead!")
-    def moderation(self) -> Optional[TextCreateResponseModeration]:
-        return self.moderations
-
 
 class _TextClassificationCreateParametersQuery(ApiBaseModel):
     version: Literal["2023-11-22"] = "2023-11-22"
 
 
 class _TextClassificationCreateRequest(ApiBaseModel):
     data: list[TextClassificationCreateData] = Field(..., min_length=1)
@@ -1028,25 +1150,27 @@
 
 
 class TextClassificationCreateResponse(ApiBaseModel):
     result: TextClassificationResult
 
 
 class _TextEmbeddingCreateParametersQuery(ApiBaseModel):
-    version: Literal["2023-11-22"] = "2023-11-22"
+    version: Literal["2024-04-15"] = "2024-04-15"
 
 
 class _TextEmbeddingCreateRequest(ApiBaseModel):
     input: Union[str, Input]
     model_id: str
     parameters: Optional[TextEmbeddingParameters] = None
 
 
 class TextEmbeddingCreateResponse(ApiBaseModel):
-    results: list[list[float]]
+    created_at: AwareDatetime
+    model_id: str
+    results: list[_TextEmbeddingCreateResults]
 
 
 class _TextEmbeddingLimitRetrieveParametersQuery(ApiBaseModel):
     version: Literal["2023-11-22"] = "2023-11-22"
 
 
 class TextEmbeddingLimitRetrieveResponse(ApiBaseModel):
@@ -1185,19 +1309,14 @@
     created_at: Optional[AwareDatetime] = None
     id: Optional[str] = None
     input_parameters: Optional[dict[str, Any]] = None
     model_id: str
     moderations: Optional[TextCreateResponseModeration] = None
     results: Optional[list[TextGenerationStreamResult]] = None
 
-    @computed_field
-    @deprecated.deprecated(reason="'moderation' property is deprecated, use 'moderations' instead!")
-    def moderation(self) -> Optional[TextCreateResponseModeration]:
-        return self.moderations
-
 
 class _TextModerationCreateParametersQuery(ApiBaseModel):
     version: Literal["2024-03-19"] = "2024-03-19"
 
 
 class _TextModerationCreateRequest(ApiBaseModel):
     hap: Optional[HAPOptions] = None
@@ -1253,14 +1372,80 @@
 
 class TextTokenizationCreateResponse(ApiBaseModel):
     created_at: str
     model_id: str
     results: list[TextTokenizationCreateResults]
 
 
+class _TimeSerieForecastingCreateParametersQuery(ApiBaseModel):
+    version: Literal["2023-11-22"] = "2023-11-22"
+
+
+class _TimeSerieForecastingCreateRequest(ApiBaseModel):
+    conditional_columns: Optional[list[str]] = Field(None, max_length=500, min_length=0, title="Conditional Columns")
+    """
+    An optional array of column headings which constitute the conditional variables.
+    """
+    context_length: Optional[int] = Field(None, title="Context Length")
+    """
+    Context length of the forecast.
+    """
+    control_columns: Optional[list[str]] = Field(None, max_length=500, min_length=0, title="Control Columns")
+    """
+    An optional array of column headings which constitute the control variables.
+    """
+    data: str = Field(..., max_length=50000, min_length=1, title="Data")
+    """
+    Base64 encoded string of data.
+    """
+    future_data: Optional[str] = Field(None, max_length=50000, min_length=0, title="Future Data")
+    """
+    Base64 encoded string of data for future supporting features.
+    """
+    id_columns: Optional[list[str]] = Field(None, max_length=10, min_length=0, title="Id Columns")
+    """
+    Columns that define a unique key for time series.
+    """
+    model_id: str
+    observable_columns: Optional[list[str]] = Field(None, max_length=500, min_length=0, title="Observable Columns")
+    """
+    An optional array of column headings which constitute the observable variables.
+    """
+    prediction_length: Optional[int] = Field(None, title="Prediction Length")
+    """
+    The prediction length for the forecast.
+    """
+    static_categorical_columns: Optional[list[str]] = Field(
+        None, max_length=500, min_length=0, title="Static Categorical Columns"
+    )
+    """
+    An optional array of column headings which constitute the static categorical variables.
+    """
+    target_columns: Optional[list[str]] = Field(None, max_length=500, min_length=0, title="Target Columns")
+    """
+    An array of column headings which constitute the target variables.
+    """
+    timestamp_column: str = Field(..., max_length=100, min_length=1, title="Timestamp Column")
+    """
+    A valid column in the data that should be treated as the timestamp.
+    """
+
+
+class TimeSerieForecastingCreateResponse(ApiBaseModel):
+    result: _TimeSerieForecastingCreateResult
+
+
+class _TimeSerieLimitRetrieveParametersQuery(ApiBaseModel):
+    version: Literal["2023-11-22"] = "2023-11-22"
+
+
+class TimeSerieLimitRetrieveResponse(ApiBaseModel):
+    result: TimeSeriesLimit
+
+
 class _TuneCreateParametersQuery(ApiBaseModel):
     version: Literal["2023-11-22"] = "2023-11-22"
 
 
 class _TuneCreateRequest(ApiBaseModel):
     evaluation_file_ids: Optional[list[str]] = None
     model_id: str
@@ -1285,14 +1470,19 @@
     name: str
 
 
 class TuneFromFileCreateResponse(ApiBaseModel):
     result: TuneResult
 
 
+class _TuneIdContentRetrieveParametersQuery(ApiBaseModel):
+    content: str
+    version: Literal["2023-11-22"] = "2023-11-22"
+
+
 class _TuneIdContentTypeRetrieveParametersQuery(ApiBaseModel):
     version: Literal["2023-12-15"] = "2023-12-15"
 
 
 class _TuneIdDeleteParametersQuery(ApiBaseModel):
     version: Literal["2023-11-22"] = "2023-11-22"
 
@@ -1314,14 +1504,33 @@
     version: Literal["2023-11-22"] = "2023-11-22"
 
 
 class TuneIdRetrieveResponse(ApiBaseModel):
     result: TuneResult
 
 
+class _TunePreflightCreateParametersQuery(ApiBaseModel):
+    version: Literal["2023-11-22"] = "2023-11-22"
+
+
+class _TunePreflightCreateRequest(ApiBaseModel):
+    evaluation_file_ids: Optional[list[str]] = None
+    model_id: str
+    name: str
+    parameters: Optional[TuneParameters] = None
+    task_id: str
+    training_file_ids: list[str]
+    tuning_type: str
+    validation_file_ids: Optional[list[str]] = None
+
+
+class TunePreflightCreateResponse(ApiBaseModel):
+    result: _TunePreflightCreateResult
+
+
 class _TuneRetrieveParametersQuery(ApiBaseModel):
     limit: Optional[int] = Field(100, ge=1, le=100)
     offset: Optional[int] = Field(0, ge=0)
     status: Optional[TuneStatus] = None
     search: Optional[str] = None
     sort_by: Optional[TuneListSortBy] = None
     direction: Optional[SortDirection] = None
@@ -1375,40 +1584,35 @@
     version: Literal["2023-11-22"] = "2023-11-22"
 
 
 class UserRetrieveResponse(ApiBaseModel):
     result: UserResult
 
 
-class _BetaTimeSerieForecastingCreateRequestColumns(ApiBaseModel):
-    conditional: Optional[list[str]] = None
-    control: Optional[list[str]] = None
-    id: Optional[list[str]] = None
-    observable: Optional[list[str]] = None
-    static_categorical: Optional[list[str]] = None
-    target: Optional[list[str]] = None
-    timestamp: str
+class _TextEmbeddingCreateRequestParametersReturnOptions(ApiBaseModel):
+    input_text: Optional[bool] = None
 
 
-class _BetaTimeSerieForecastingCreateResult(ApiBaseModel):
-    predictions: str
+class _TextEmbeddingCreateResults(ApiBaseModel):
+    embedding: list[float]
+    input_text: Optional[str] = None
 
 
-class _BetaTimeSerieLimitRetrieveResult(ApiBaseModel):
-    concurrency: _BetaTimeSerieLimitRetrieveResultConcurrency
+class _TextRerankCreateResult(ApiBaseModel):
+    query: Optional[str] = None
+    results: list[TextRerankResult]
 
 
-class _BetaTimeSerieLimitRetrieveResultConcurrency(ApiBaseModel):
-    limit: int
-    remaining: int
+class _TimeSerieForecastingCreateResult(ApiBaseModel):
+    predictions: str
 
 
-class _TextRerankCreateResult(ApiBaseModel):
-    query: Optional[str] = None
-    results: list[TextRerankResult]
+class _TunePreflightCreateResult(ApiBaseModel):
+    training_file_preview: Optional[list[dict[str, Any]]] = None
+    validation_file_preview: Optional[list[dict[str, Any]]] = None
 
 
 class PromptListSortBy(str, Enum):
     TYPE = "type"
     MODEL_TASK = "model_task"
     UPDATED_AT = "updated_at"
     CREATED_AT = "created_at"
@@ -1678,30 +1882,21 @@
     BINARY = "binary"
 
 
 class TextCreateResponseModeration(ApiBaseModel):
     hap: Optional[list[TextModeration]] = None
     social_bias: Optional[list[TextModeration]] = None
 
-    @computed_field
-    @deprecated.deprecated(reason="'stigma' property is deprecated, use 'social_bias' instead!")
-    def stigma(self) -> Optional[list[TextModeration]]:
-        return None
-
-    @computed_field
-    @deprecated.deprecated(reason="'implicit_hate' property is deprecated, use 'social_bias' instead!")
-    def implicit_hate(self) -> Optional[list[TextModeration]]:
-        return None
-
 
 class TextEmbeddingLimit(ApiBaseModel):
     concurrency: ConcurrencyLimit
 
 
 class TextEmbeddingParameters(ApiBaseModel):
+    return_options: Optional[_TextEmbeddingCreateRequestParametersReturnOptions] = None
     truncate_input_tokens: Optional[bool] = None
 
 
 class TextGenerationComparisonCreateRequestRequest(ApiBaseModel):
     data: Optional[PromptTemplateData] = None
     input: str
     model_id: Optional[str] = None
@@ -1845,19 +2040,14 @@
     input_token_count: Optional[int] = None
     input_tokens: Optional[list[BaseTokens]] = None
     moderations: Optional[TextCreateResponseModeration] = None
     seed: Optional[float] = None
     stop_reason: StopReason
     stop_sequence: Optional[str] = None
 
-    @computed_field
-    @deprecated.deprecated(reason="'moderation' property is deprecated, use 'moderations' instead!")
-    def moderation(self) -> Optional[TextCreateResponseModeration]:
-        return self.moderations
-
 
 class TextGenerationReturnOptions(ApiBaseModel):
     generated_tokens: Optional[bool] = Field(False, title="Generated Tokens")
     """
     Include list of individual generated tokens
     """
     input_parameters: Optional[bool] = None
@@ -1937,14 +2127,18 @@
 
 
 class TextTokenizationReturnOptions(ApiBaseModel):
     input_text: Optional[bool] = None
     tokens: Optional[bool] = None
 
 
+class TimeSeriesLimit(ApiBaseModel):
+    concurrency: ConcurrencyLimit
+
+
 class TooManyRequestsResponse(BaseErrorResponse):
     extensions: Extensions3
     status_code: Literal[429] = 429
 
 
 class TrimMethod(str, Enum):
     FLOATING_WINDOW = "floating_window"
@@ -1973,19 +2167,21 @@
     max_output_tokens: Optional[int] = None
     num_epochs: Optional[int] = None
     num_virtual_tokens: Optional[int] = None
     verbalizer: Optional[str] = None
 
 
 class TuneResult(ApiBaseModel):
+    contents: Optional[list[TuneResultContent]] = None
     created_at: AwareDatetime
-    datapoints: Optional[TuneResultDatapoints] = None
+    datapoints: Optional[TuneResultDatapoint] = None
     evaluation_files: Optional[list[TuneResultFiles]] = None
     finished_at: Optional[AwareDatetime] = None
     id: str
+    last_used_at: Optional[AwareDatetime] = None
     model_id: str
     model_name: str
     name: str
     parameters: Optional[dict[str, Any]] = None
     preferred: bool
     started_at: Optional[AwareDatetime] = None
     status: TuneStatus
@@ -1994,22 +2190,38 @@
     task_name: str
     training_files: Optional[list[TuneResultFiles]] = None
     tuning_type: str
     validation_files: Optional[list[TuneResultFiles]] = None
     vectors: Optional[str] = None
 
 
-class TuneResultDatapointLoss(ApiBaseModel):
+class TuneResultContent(ApiBaseModel):
+    name: str
+
+
+class TuneResultDatapoint(ApiBaseModel):
+    loss: list[TunesResultDatapointLoss]
+    validation_loss: Optional[list[TuneResultDatapointValidationLoss]] = None
+
+
+class TuneResultDatapointLossData(ApiBaseModel):
     epoch: int
     step: Optional[int] = None
     value: float
 
 
-class TuneResultDatapoints(ApiBaseModel):
-    loss: list[TunesResultDatapointLoss]
+class TuneResultDatapointValidationLoss(ApiBaseModel):
+    data: TuneResultDatapointValidationLossData
+    timestamp: AwareDatetime
+
+
+class TuneResultDatapointValidationLossData(ApiBaseModel):
+    epoch: int
+    step: Optional[int] = None
+    value: float
 
 
 class TuneResultFiles(ApiBaseModel):
     created_at: Optional[AwareDatetime] = None
     file_name: str
     id: str
 
@@ -2022,15 +2234,15 @@
     RUNNING = "running"
     QUEUED = "queued"
     COMPLETED = "completed"
     FAILED = "failed"
 
 
 class TunesResultDatapointLoss(ApiBaseModel):
-    data: TuneResultDatapointLoss
+    data: TuneResultDatapointLossData
     timestamp: AwareDatetime
 
 
 class TuningTypeRetrieveResults(ApiBaseModel):
     id: Optional[str] = None
     model_ids: Optional[list[str]] = None
     name: Optional[str] = None
@@ -2096,31 +2308,61 @@
     "ApiKeyResult",
     "ApiKeyRetrieveResponse",
     "BadRequestResponse",
     "BaseErrorExtension",
     "BaseErrorResponse",
     "BaseMessage",
     "BaseTokens",
-    "BetaTimeSerieForecastingCreateResponse",
-    "BetaTimeSerieLimitRetrieveResponse",
     "ChatRole",
     "ConcurrencyLimit",
     "DecodingMethod",
+    "DeploymentCreateResponse",
+    "DeploymentIdRetrieveResponse",
+    "DeploymentResult",
+    "DeploymentRetrieveResponse",
+    "DeploymentStatus",
+    "EvaluationCreateResponse",
+    "EvaluationExperiment",
+    "EvaluationExperimentCreateResponse",
+    "EvaluationExperimentIdRetrieveResponse",
+    "EvaluationExperimentRetrieveResponse",
+    "EvaluationExperimentSortBy",
+    "EvaluationFieldOperation",
+    "EvaluationFile",
+    "EvaluationIdInstanceResultRetrieveResponse",
+    "EvaluationIdRetrieveResponse",
+    "EvaluationInstanceResult",
+    "EvaluationLimit",
+    "EvaluationLimitRetrieveResponse",
+    "EvaluationOperationType",
+    "EvaluationParentTask",
+    "EvaluationPreviewCreateResponse",
+    "EvaluationPrompt",
+    "EvaluationResult",
+    "EvaluationRetrieveResponse",
+    "EvaluationSortBy",
+    "EvaluationStatus",
+    "EvaluationTask",
+    "EvaluationTemplate",
+    "EvaluationTemplateIdRetrieveResponse",
+    "EvaluationTemplateRetrieveResponse",
     "Extensions",
     "Extensions1",
     "Extensions2",
     "Extensions3",
     "Extensions4",
     "Extensions5",
     "FileCreateResponse",
     "FileDescendant",
     "FileFormat",
     "FileIdPatchResponse",
     "FileIdRetrieveResponse",
     "FileListSortBy",
+    "FileMetadata",
+    "FileMetadataStats",
     "FilePurpose",
     "FileResult",
     "FileRetrieveResponse",
     "FolderCreateResponse",
     "FolderIdPatchResponse",
     "FolderIdRetrieveResponse",
     "FolderIdUpdateResponse",
@@ -2128,14 +2370,16 @@
     "FolderRetrieveResponse",
     "GeneratedToken",
     "HAPOptions",
     "Input",
     "InternalServerErrorResponse",
     "LengthPenalty",
     "MessageFile",
+    "Metric",
+    "Metrics",
     "ModelFacet",
     "ModelFacetType",
     "ModelFamily",
     "ModelIdRetrieveResponse",
     "ModelIdRetrieveResult",
     "ModelRetrieveResponse",
     "ModelRetrieveResults",
@@ -2248,26 +2492,33 @@
     "TextSentenceSimilarityCreateResponse",
     "TextSentenceSimilarityCreateResult",
     "TextSentenceSimilarityParameters",
     "TextTokenizationCreateResponse",
     "TextTokenizationCreateResults",
     "TextTokenizationParameters",
     "TextTokenizationReturnOptions",
+    "TimeSerieForecastingCreateResponse",
+    "TimeSerieLimitRetrieveResponse",
+    "TimeSeriesLimit",
     "TooManyRequestsResponse",
     "TrimMethod",
     "TuneAssetType",
     "TuneCreateResponse",
     "TuneFromFileCreateResponse",
     "TuneIdPatchResponse",
     "TuneIdRetrieveResponse",
     "TuneListSortBy",
     "TuneParameters",
+    "TunePreflightCreateResponse",
     "TuneResult",
-    "TuneResultDatapointLoss",
-    "TuneResultDatapoints",
+    "TuneResultContent",
+    "TuneResultDatapoint",
+    "TuneResultDatapointLossData",
+    "TuneResultDatapointValidationLoss",
+    "TuneResultDatapointValidationLossData",
     "TuneResultFiles",
     "TuneRetrieveResponse",
     "TuneStatus",
     "TunesResultDatapointLoss",
     "TuningTypeRetrieveResponse",
     "TuningTypeRetrieveResults",
     "UnauthorizedResponse",
```

### Comparing `ibm_generative_ai-2.3.0/src/genai/schema/_endpoints.py` & `ibm_generative_ai-3.0.0/src/genai/schema/_endpoints.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,92 @@
 
 class ApiKeyRegenerateCreateEndpoint(ApiEndpoint):
     path: str = "/v2/api_key/regenerate"
     method: str = "POST"
     version: str = "2023-11-22"
 
 
+class EvaluationRetrieveEndpoint(ApiEndpoint):
+    path: str = "/v2/beta/evaluations"
+    method: str = "GET"
+    version: str = "2023-11-22"
+
+
+class EvaluationCreateEndpoint(ApiEndpoint):
+    path: str = "/v2/beta/evaluations"
+    method: str = "POST"
+    version: str = "2023-11-22"
+
+
+class EvaluationExperimentRetrieveEndpoint(ApiEndpoint):
+    path: str = "/v2/beta/evaluations/experiments"
+    method: str = "GET"
+    version: str = "2023-11-22"
+
+
+class EvaluationExperimentCreateEndpoint(ApiEndpoint):
+    path: str = "/v2/beta/evaluations/experiments"
+    method: str = "POST"
+    version: str = "2023-11-22"
+
+
+class EvaluationExperimentIdDeleteEndpoint(ApiEndpoint):
+    path: str = "/v2/beta/evaluations/experiments/{id}"
+    method: str = "DELETE"
+    version: str = "2023-11-22"
+
+
+class EvaluationExperimentIdRetrieveEndpoint(ApiEndpoint):
+    path: str = "/v2/beta/evaluations/experiments/{id}"
+    method: str = "GET"
+    version: str = "2023-11-22"
+
+
+class EvaluationLimitRetrieveEndpoint(ApiEndpoint):
+    path: str = "/v2/beta/evaluations/limits"
+    method: str = "GET"
+    version: str = "2023-11-22"
+
+
+class EvaluationPreviewCreateEndpoint(ApiEndpoint):
+    path: str = "/v2/beta/evaluations/preview"
+    method: str = "POST"
+    version: str = "2023-11-22"
+
+
+class EvaluationTemplateRetrieveEndpoint(ApiEndpoint):
+    path: str = "/v2/beta/evaluations/templates"
+    method: str = "GET"
+    version: str = "2023-11-22"
+
+
+class EvaluationTemplateIdRetrieveEndpoint(ApiEndpoint):
+    path: str = "/v2/beta/evaluations/templates/{id}"
+    method: str = "GET"
+    version: str = "2023-11-22"
+
+
+class EvaluationIdDeleteEndpoint(ApiEndpoint):
+    path: str = "/v2/beta/evaluations/{id}"
+    method: str = "DELETE"
+    version: str = "2023-11-22"
+
+
+class EvaluationIdRetrieveEndpoint(ApiEndpoint):
+    path: str = "/v2/beta/evaluations/{id}"
+    method: str = "GET"
+    version: str = "2023-11-22"
+
+
+class EvaluationIdInstanceResultRetrieveEndpoint(ApiEndpoint):
+    path: str = "/v2/beta/evaluations/{id}/instance_results"
+    method: str = "GET"
+    version: str = "2023-11-22"
+
+
 class TextClassificationCreateEndpoint(ApiEndpoint):
     path: str = "/v2/beta/text/classification"
     method: str = "POST"
     version: str = "2023-11-22"
 
 
 class TextRerankCreateEndpoint(ApiEndpoint):
@@ -32,48 +110,72 @@
 
 class TextSentenceSimilarityCreateEndpoint(ApiEndpoint):
     path: str = "/v2/beta/text/sentence-similarity"
     method: str = "POST"
     version: str = "2023-11-22"
 
 
-class BetaTimeSerieForecastingCreateEndpoint(ApiEndpoint):
+class TimeSerieForecastingCreateEndpoint(ApiEndpoint):
     path: str = "/v2/beta/time_series/forecasting"
     method: str = "POST"
     version: str = "2023-11-22"
 
 
-class BetaTimeSerieLimitRetrieveEndpoint(ApiEndpoint):
+class TimeSerieLimitRetrieveEndpoint(ApiEndpoint):
     path: str = "/v2/beta/time_series/limits"
     method: str = "GET"
     version: str = "2023-11-22"
 
 
+class DeploymentRetrieveEndpoint(ApiEndpoint):
+    path: str = "/v2/deployments"
+    method: str = "GET"
+    version: str = "2023-11-22"
+
+
+class DeploymentCreateEndpoint(ApiEndpoint):
+    path: str = "/v2/deployments"
+    method: str = "POST"
+    version: str = "2023-11-22"
+
+
+class DeploymentIdDeleteEndpoint(ApiEndpoint):
+    path: str = "/v2/deployments/{id}"
+    method: str = "DELETE"
+    version: str = "2023-11-22"
+
+
+class DeploymentIdRetrieveEndpoint(ApiEndpoint):
+    path: str = "/v2/deployments/{id}"
+    method: str = "GET"
+    version: str = "2023-11-22"
+
+
 class FileRetrieveEndpoint(ApiEndpoint):
     path: str = "/v2/files"
     method: str = "GET"
-    version: str = "2023-12-15"
+    version: str = "2024-05-13"
 
 
 class FileCreateEndpoint(ApiEndpoint):
     path: str = "/v2/files"
     method: str = "POST"
-    version: str = "2023-12-15"
+    version: str = "2024-05-13"
 
 
 class FileIdDeleteEndpoint(ApiEndpoint):
     path: str = "/v2/files/{id}"
     method: str = "DELETE"
     version: str = "2023-11-22"
 
 
 class FileIdRetrieveEndpoint(ApiEndpoint):
     path: str = "/v2/files/{id}"
     method: str = "GET"
-    version: str = "2023-12-15"
+    version: str = "2024-05-13"
 
 
 class FileIdPatchEndpoint(ApiEndpoint):
     path: str = "/v2/files/{id}"
     method: str = "PATCH"
     version: str = "2023-11-22"
 
@@ -269,15 +371,15 @@
     method: str = "POST"
     version: str = "2024-03-19"
 
 
 class TextEmbeddingCreateEndpoint(ApiEndpoint):
     path: str = "/v2/text/embeddings"
     method: str = "POST"
-    version: str = "2023-11-22"
+    version: str = "2024-04-15"
 
 
 class TextEmbeddingLimitRetrieveEndpoint(ApiEndpoint):
     path: str = "/v2/text/embeddings/limits"
     method: str = "GET"
     version: str = "2023-11-22"
 
@@ -362,14 +464,20 @@
 
 class TuneFromFileCreateEndpoint(ApiEndpoint):
     path: str = "/v2/tunes/import"
     method: str = "POST"
     version: str = "2023-11-22"
 
 
+class TunePreflightCreateEndpoint(ApiEndpoint):
+    path: str = "/v2/tunes/preflight"
+    method: str = "POST"
+    version: str = "2023-11-22"
+
+
 class TuneIdDeleteEndpoint(ApiEndpoint):
     path: str = "/v2/tunes/{id}"
     method: str = "DELETE"
     version: str = "2023-11-22"
 
 
 class TuneIdRetrieveEndpoint(ApiEndpoint):
@@ -380,14 +488,20 @@
 
 class TuneIdPatchEndpoint(ApiEndpoint):
     path: str = "/v2/tunes/{id}"
     method: str = "PATCH"
     version: str = "2023-11-22"
 
 
+class TuneIdContentRetrieveEndpoint(ApiEndpoint):
+    path: str = "/v2/tunes/{id}/content"
+    method: str = "GET"
+    version: str = "2023-11-22"
+
+
 class TuneIdContentTypeRetrieveEndpoint(ApiEndpoint):
     path: str = "/v2/tunes/{id}/content/{type}"
     method: str = "GET"
     version: str = "2023-12-15"
 
 
 class TuningTypeRetrieveEndpoint(ApiEndpoint):
```

### Comparing `ibm_generative_ai-2.3.0/src/genai/system_prompt/system_prompt_service.py` & `ibm_generative_ai-3.0.0/src/genai/system_prompt/system_prompt_service.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/tag/tag_service.py` & `ibm_generative_ai-3.0.0/src/genai/tag/tag_service.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/task/task_service.py` & `ibm_generative_ai-3.0.0/src/genai/task/task_service.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/text/chat/chat_generation_service.py` & `ibm_generative_ai-3.0.0/src/genai/text/chat/chat_generation_service.py`

 * *Files 11% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             from genai import Client, Credentials
             from genai.text.chat import HumanMessage, TextGenerationParameters
 
             client = Client(credentials=Credentials.from_env())
 
             # Create a new conversation
             response = client.text.chat.create(
-                model_id="meta-llama/llama-2-70b-chat",
+                model_id="meta-llama/llama-3-70b-instruct",
                 messages=[HumanMessage(content="Describe the game Chess?")],
                 parameters=TextGenerationParameters(max_token_limit=100)
             )
             conversation_id = response.conversation_id
             print(f"Response: {response.results[0].generated_text}")
 
             # Continue in the conversation
@@ -97,16 +97,14 @@
         Raises:
             ApiResponseException: In case of a known API error.
             ApiNetworkException: In case of unhandled network error.
             ValidationError: In case of provided parameters are invalid.
         """
         metadata = get_service_action_metadata(self.create)
         moderations_formatted = to_model_optional(moderations, ModerationParameters, copy=True)
-        if moderations_formatted:
-            moderations_formatted.remove_deprecated()
 
         request_body = _TextChatCreateRequest(
             model_id=model_id,
             conversation_id=conversation_id,
             messages=self._prepare_messages(messages) if messages is not None else None,
             moderations=moderations_formatted,
             parameters=to_model_optional(parameters, TextGenerationParameters),
@@ -148,29 +146,27 @@
             from genai import Client, Credentials
             from genai.text.chat import HumanMessage, TextGenerationParameters
 
             client = Client(credentials=Credentials.from_env())
 
             # Create a new conversation
             for response in client.text.chat.create_stream(
-                    model_id="meta-llama/llama-2-70b-chat",
+                    model_id="meta-llama/llama-3-70b-instruct",
                     messages=[HumanMessage(content="Describe the game Chess?")],
                     parameters=TextGenerationParameters(max_token_limit=100)
                 ):
                 print(f"Chunk retrieved: {response.results[0].generated_text}")
 
         Raises:
             ApiResponseException: In case of a known API error.
             ApiNetworkException: In case of unhandled network error.
             ValidationError: In case of provided parameters are invalid.
         """
         metadata = get_service_action_metadata(self.create_stream)
         moderations_formatted = to_model_optional(moderations, ModerationParameters, copy=True)
-        if moderations_formatted:
-            moderations_formatted.remove_deprecated()
 
         request_body = _TextChatStreamCreateRequest(
             model_id=model_id,
             conversation_id=conversation_id,
             messages=self._prepare_messages(messages) if messages is not None else None,
             moderations=moderations_formatted,
             parameters=to_model_optional(parameters, TextGenerationParameters),
```

### Comparing `ibm_generative_ai-2.3.0/src/genai/text/embedding/embedding_service.py` & `ibm_generative_ai-3.0.0/src/genai/text/embedding/embedding_service.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/text/embedding/limit/limit_service.py` & `ibm_generative_ai-3.0.0/src/genai/text/embedding/limit/limit_service.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/text/experimental/classification/classification_service.py` & `ibm_generative_ai-3.0.0/src/genai/text/experimental/classification/classification_service.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/text/experimental/experimental_service.py` & `ibm_generative_ai-3.0.0/src/genai/text/experimental/experimental_service.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/text/experimental/rerank/rerank_service.py` & `ibm_generative_ai-3.0.0/src/genai/text/experimental/rerank/rerank_service.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/text/experimental/sentence_similarity/sentence_similarity_service.py` & `ibm_generative_ai-3.0.0/src/genai/text/experimental/sentence_similarity/sentence_similarity_service.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/text/generation/_generation_utils.py` & `ibm_generative_ai-3.0.0/src/genai/text/generation/_generation_utils.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/text/generation/generation_service.py` & `ibm_generative_ai-3.0.0/src/genai/text/generation/generation_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Generator, Optional, Union
 
 import httpx
-from deprecated import deprecated
 from httpx import AsyncClient, HTTPStatusError
 from pydantic import BaseModel
 
 from genai._types import ModelLike
 from genai._utils.api_client import ApiClient
 from genai._utils.async_executor import execute_async
 from genai._utils.general import cast_list, to_model_instance, to_model_optional
@@ -35,30 +34,28 @@
     _TextGenerationComparisonCreateRequest,
     _TextGenerationCreateParametersQuery,
     _TextGenerationCreateRequest,
     _TextGenerationStreamCreateParametersQuery,
     _TextGenerationStreamCreateRequest,
 )
 from genai.text.generation._generation_utils import generation_stream_handler
-from genai.text.generation.feedback.feedback_service import FeedbackService as _FeedbackService
 from genai.text.generation.limits.limit_service import LimitService as _LimitService
 
 __all__ = ["GenerationService", "BaseConfig", "BaseServices", "CreateExecutionOptions"]
 
 
 from genai._utils.http_client.retry_transport import BaseRetryTransport
 from genai._utils.limiters.base_limiter import BaseLimiter
 from genai._utils.limiters.external_limiter import ConcurrencyResponse, ExternalLimiter
 from genai._utils.limiters.local_limiter import LocalLimiter
 from genai._utils.limiters.shared_limiter import LoopBoundLimiter
 
 
 class BaseServices(BaseServiceServices):
     LimitService: type[_LimitService] = _LimitService
-    FeedbackService: type[_FeedbackService] = _FeedbackService
 
 
 class CreateExecutionOptions(BaseModel):
     throw_on_error: CommonExecutionOptions.throw_on_error = True
     ordered: CommonExecutionOptions.ordered = True
     concurrency_limit: CommonExecutionOptions.concurrency_limit = None
     callback: CommonExecutionOptions.callback[
@@ -83,22 +80,16 @@
     ):
         super().__init__(api_client=api_client, config=config)
 
         if not services:
             services = BaseServices()
 
         self._concurrency_limiter = self._get_concurrency_limiter()
-        self._feedback = services.FeedbackService(api_client=api_client)
         self.limit = services.LimitService(api_client=api_client)
 
-    @property
-    @deprecated(reason="Use 'client.request.feedback' service instead.")
-    def feedback(self):
-        return self._feedback
-
     def _get_concurrency_limiter(self) -> LoopBoundLimiter:
         async def handler():
             response = await self.limit.aretrieve()
             return ConcurrencyResponse(
                 limit=response.result.concurrency.limit,
                 remaining=response.result.concurrency.remaining,
             )
@@ -148,17 +139,14 @@
         )
         if not prompts and not prompt_id:
             raise ValueError("At least one of the following parameters input/inputs/prompt_id must be specified!")
 
         metadata = get_service_action_metadata(self.create)
         parameters_formatted = to_model_optional(parameters, TextGenerationParameters)
         moderations_formatted = to_model_optional(moderations, ModerationParameters, copy=True)
-        if moderations_formatted:
-            moderations_formatted.remove_deprecated()
-
         template_formatted = to_model_optional(data, PromptTemplateData)
         execution_options_formatted = to_model_instance(
             [self.config.create_execution_options, execution_options], CreateExecutionOptions
         )
         assert execution_options_formatted
 
         self._log_method_execution(
@@ -254,17 +242,14 @@
             ApiResponseException: In case of a known API error.
             ApiNetworkException: In case of unhandled network error.
             ValidationError: In case of provided parameters are invalid.
         """
         metadata = get_service_action_metadata(self.create_stream)
         parameters_formatted = to_model_optional(parameters, TextGenerationParameters)
         moderations_formatted = to_model_optional(moderations, ModerationParameters, copy=True)
-        if moderations_formatted:
-            moderations_formatted.remove_deprecated()
-
         template_formatted = to_model_optional(data, PromptTemplateData)
 
         self._log_method_execution(
             "Generate Create Stream",
             input=input,
             parameters=parameters_formatted,
             moderations=moderations_formatted,
@@ -301,17 +286,14 @@
         Raises:
             ApiResponseException: In case of a known API error.
             ApiNetworkException: In case of unhandled network error.
             ValidationError: In case of provided parameters are invalid.
         """
         metadata = get_service_action_metadata(self.compare)
         request_formatted = to_model_instance(request, TextGenerationComparisonCreateRequestRequest, copy=True)
-        if request_formatted.moderations:
-            request_formatted.moderations.remove_deprecated()
-
         compare_parameters_formatted = to_model_instance(compare_parameters, TextGenerationComparisonParameters)
 
         self._log_method_execution(
             "Text Generation Compare",
             input=input,
             requests=request_formatted,
             parameters=compare_parameters_formatted,
```

### Comparing `ibm_generative_ai-2.3.0/src/genai/text/generation/limits/limit_service.py` & `ibm_generative_ai-3.0.0/src/genai/text/generation/limits/limit_service.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/text/moderation/moderation_service.py` & `ibm_generative_ai-3.0.0/src/genai/text/moderation/moderation_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,26 +40,22 @@
 
     @set_service_action_metadata(endpoint=TextModerationCreateEndpoint)
     def create(
         self,
         inputs: Union[str, list[str]],
         *,
         hap: Optional[ModelLike[HAPOptions]] = None,
-        implicit_hate: Optional[ModelLike] = None,
-        stigma: Optional[ModelLike] = None,
         social_bias: Optional[ModelLike[SocialBiasOptions]] = None,
         execution_options: Optional[ModelLike[CreateExecutionOptions]] = None,
     ) -> Generator[TextModerationCreateResponse, None, None]:
         """
         Args:
             inputs: Prompt/Prompts for text moderation.
             hap: HAP configuration (hate, abuse, profanity).
             social_bias: Social Bias configuration.
-            implicit_hate: Implicit Hate configuration (deprecated, use 'social_bias' instead).
-            stigma: Stigma configuration (deprecated, use 'social_bias' instead).
             execution_options: Configuration processing.
 
         Example:
             from genai import Client, Credentials
             from genai.text.moderation import HAPOptions
 
             client = Client(credentials=Credentials.from_env())
@@ -73,18 +69,14 @@
                     print(f"Response for {input}", result.hap)
 
         Raises:
             ApiResponseException: In case of a known API error.
             ApiNetworkException: In case of unhandled network error.
             ValidationError: In case of provided parameters are invalid.
         """
-        if implicit_hate is not None:
-            self._log_deprecation_warning("'implicit_hate' parameter is deprecated, use 'social_bias' instead!")
-        if stigma is not None:
-            self._log_deprecation_warning("'stigma' parameter is deprecated, use 'social_bias' instead!")
 
         metadata = get_service_action_metadata(self.create)
         execution_options_formatted = to_model_instance(
             [self.config.create_execution_options, execution_options], CreateExecutionOptions
         )
         self._log_method_execution(
             "Moderation Create",
```

### Comparing `ibm_generative_ai-2.3.0/src/genai/text/text_service.py` & `ibm_generative_ai-3.0.0/src/genai/text/text_service.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/text/tokenization/tokenization_service.py` & `ibm_generative_ai-3.0.0/src/genai/text/tokenization/tokenization_service.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/tune/tune_service.py` & `ibm_generative_ai-3.0.0/src/genai/tune/tune_service.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/src/genai/user/user_service.py` & `ibm_generative_ai-3.0.0/src/genai/user/user_service.py`

 * *Files identical despite different names*

### Comparing `ibm_generative_ai-2.3.0/PKG-INFO` & `ibm_generative_ai-3.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: ibm-generative-ai
-Version: 2.3.0
+Version: 3.0.0
 Summary: IBM Generative AI is a Python library built on IBM's large language model REST interface.
 Author: Tomas Dvorak
 Author-email: tomas.dvorak@ibm.com
 Maintainer: Tomas Dvorak
 Maintainer-email: tomas.dvorak@ibm.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: huggingface
 Provides-Extra: langchain
 Provides-Extra: llama-index
+Provides-Extra: lm-eval
 Provides-Extra: localserver
 Requires-Dist: aiolimiter (>=1.1.0,<2.0.0)
-Requires-Dist: datasets (>=2.13.0,<3.0.0) ; extra == "huggingface"
 Requires-Dist: deprecated (>=1.2.14,<2.0.0)
 Requires-Dist: fastapi (>=0.100.0,<0.101.0) ; extra == "localserver"
-Requires-Dist: httpx (>=0.26.0,<0.27.0)
-Requires-Dist: httpx-sse (>=0.3.0,<0.4.0)
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
+Requires-Dist: httpx-sse (>=0.4.0,<0.5.0)
 Requires-Dist: langchain-core (>=0.1.0,<0.2.0) ; extra == "langchain"
 Requires-Dist: llama-index-core (>=0.10.0,<0.11.0) ; extra == "llama-index"
+Requires-Dist: lm-eval (>=0.4.2,<0.5.0) ; extra == "lm-eval"
 Requires-Dist: pydantic (>=2.0.0,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.0,<7.0.0) ; extra == "langchain"
+Requires-Dist: tqdm (>=4.66.1,<5.0.0) ; extra == "lm-eval"
 Requires-Dist: transformers[agents] (>=4.33.3,<5.0.0) ; extra == "huggingface"
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0) ; extra == "localserver"
 Description-Content-Type: text/markdown
 
 # IBM Generative AI Python SDK (Tech Preview)
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/IBM/ibm-generative-ai/blob/main/LICENSE)
@@ -60,14 +62,16 @@
 ```
 
 
 ### [📚 Documentation](https://ibm.github.io/ibm-generative-ai/)
 
 ### [📚 Examples](https://ibm.github.io/ibm-generative-ai/latest/rst_source/examples.html)
 
+### [📚 V3 Migration Guide](https://ibm.github.io/ibm-generative-ai/latest/v3_migration_guide.html)
+
 ### [📚 V2 Migration Guide](https://ibm.github.io/ibm-generative-ai/latest/v2_migration_guide.html)
 
 
 ## Important Information for Contributors
 - Do you want to contribute to the project? IBM Generative AI is an open-source project that welcomes the community to contribute with documentation, tests, bug corrections, and new functionality in the form of [extensions](EXTENSIONS.md). Please read our [code of conduct](CODE_OF_CONDUCT.md) to learn the expected behavior from participants that contribute to the project, and our [contribution guide](./CONTRIBUTING.md) to learn the gitflow and steps to submit pull requests.
 
 <!-- vscode-markdown-toc-config
```

