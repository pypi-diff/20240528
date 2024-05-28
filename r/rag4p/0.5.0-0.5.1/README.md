# Comparing `tmp/rag4p-0.5.0.tar.gz` & `tmp/rag4p-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rag4p-0.5.0.tar", max compression
+gzip compressed data, was "rag4p-0.5.1.tar", max compression
```

## Comparing `rag4p-0.5.0.tar` & `rag4p-0.5.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0     3266 2024-05-20 08:34:12.059855 rag4p-0.5.0/README.md
--rw-r--r--   0        0        0      781 2024-05-28 12:14:29.227445 rag4p-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-17 15:16:40.886501 rag4p-0.5.0/rag4p/__init__.py
--rw-r--r--   0        0        0     3546 2024-05-11 10:19:26.281070 rag4p-0.5.0/rag4p/app_complete_local.py
--rw-r--r--   0        0        0     3224 2024-02-15 14:42:08.665322 rag4p-0.5.0/rag4p/app_complete_weaviate.py
--rw-r--r--   0        0        0     1154 2024-02-15 14:50:41.830101 rag4p-0.5.0/rag4p/app_generation_answer_generator.py
--rw-r--r--   0        0        0     1318 2024-05-11 10:19:26.290206 rag4p-0.5.0/rag4p/app_generation_answer_quality.py
--rw-r--r--   0        0        0     1292 2024-05-11 10:24:23.583279 rag4p-0.5.0/rag4p/app_generation_answer_quality_ollama.py
--rw-r--r--   0        0        0     2708 2024-02-15 15:49:18.900194 rag4p-0.5.0/rag4p/app_generation_question_generator.py
--rw-r--r--   0        0        0     1432 2024-02-15 15:31:45.716697 rag4p-0.5.0/rag4p/app_generation_questions_generator_vasa.py
--rw-r--r--   0        0        0     1214 2024-02-15 15:59:09.706810 rag4p-0.5.0/rag4p/app_indexing_local.py
--rw-r--r--   0        0        0     2330 2024-03-11 09:33:23.161900 rag4p-0.5.0/rag4p/app_indexing_weaviate.py
--rw-r--r--   0        0        0     1254 2024-02-15 15:31:45.728308 rag4p-0.5.0/rag4p/app_retrieval_quality_vasa.py
--rw-r--r--   0        0        0     1514 2024-05-15 14:45:34.878603 rag4p-0.5.0/rag4p/app_retrieval_retriever_local.py
--rw-r--r--   0        0        0     1800 2024-05-21 18:57:47.887764 rag4p-0.5.0/rag4p/app_retrieval_retriever_weaviate.py
--rw-r--r--   0        0        0     1878 2024-02-15 15:31:45.712149 rag4p-0.5.0/rag4p/app_retrieval_strategy.py
--rw-r--r--   0        0        0      429 2024-01-31 07:51:24.674544 rag4p-0.5.0/rag4p/app_weaviate_info.py
--rw-r--r--   0        0        0        0 2024-01-17 15:16:40.886501 rag4p-0.5.0/rag4p/indexing/__init__.py
--rw-r--r--   0        0        0      512 2024-05-26 09:53:31.685711 rag4p-0.5.0/rag4p/indexing/content_reader.py
--rw-r--r--   0        0        0      793 2024-05-26 09:53:31.672641 rag4p-0.5.0/rag4p/indexing/indexing_service.py
--rw-r--r--   0        0        0      232 2024-01-17 15:25:27.590307 rag4p-0.5.0/rag4p/indexing/input_document.py
--rw-r--r--   0        0        0      876 2024-05-26 09:53:31.688377 rag4p-0.5.0/rag4p/indexing/jsonl_content_reader.py
--rw-r--r--   0        0        0      285 2024-02-13 20:32:37.812960 rag4p-0.5.0/rag4p/indexing/splitter.py
--rw-r--r--   0        0        0        0 2024-02-13 19:57:32.062188 rag4p-0.5.0/rag4p/indexing/splitters/__init__.py
--rw-r--r--   0        0        0     1356 2024-02-13 20:28:11.172941 rag4p-0.5.0/rag4p/indexing/splitters/max_token_splitter.py
--rw-r--r--   0        0        0      671 2024-02-13 20:32:37.826115 rag4p-0.5.0/rag4p/indexing/splitters/sentence_splitter.py
--rw-r--r--   0        0        0      474 2024-02-13 20:32:37.822569 rag4p-0.5.0/rag4p/indexing/splitters/single_chunk_splitter.py
--rw-r--r--   0        0        0        0 2024-02-13 20:16:16.212988 rag4p-0.5.0/rag4p/integrations/__init__.py
--rw-r--r--   0        0        0      204 2024-05-10 14:28:00.181901 rag4p-0.5.0/rag4p/integrations/ollama/__init__.py
--rw-r--r--   0        0        0     2361 2024-05-10 15:59:57.265154 rag4p-0.5.0/rag4p/integrations/ollama/access_ollama.py
--rw-r--r--   0        0        0      808 2024-05-13 07:17:37.558316 rag4p-0.5.0/rag4p/integrations/ollama/ollama_answer_generator.py
--rw-r--r--   0        0        0      628 2024-05-28 10:35:20.924650 rag4p-0.5.0/rag4p/integrations/ollama/ollama_embedder.py
--rw-r--r--   0        0        0     1456 2024-05-13 07:17:37.553472 rag4p-0.5.0/rag4p/integrations/ollama/ollama_question_generator.py
--rw-r--r--   0        0        0        0 2024-05-11 10:09:25.775349 rag4p-0.5.0/rag4p/integrations/ollama/quality/__init__.py
--rw-r--r--   0        0        0     1429 2024-05-11 10:36:04.986424 rag4p-0.5.0/rag4p/integrations/ollama/quality/ollama_answer_quality_service.py
--rw-r--r--   0        0        0      429 2024-05-11 10:04:59.548674 rag4p-0.5.0/rag4p/integrations/openai/__init__.py
--rw-r--r--   0        0        0     1311 2024-05-11 09:33:48.693626 rag4p-0.5.0/rag4p/integrations/openai/openai_answer_generator.py
--rw-r--r--   0        0        0     1034 2024-05-28 10:35:20.912497 rag4p-0.5.0/rag4p/integrations/openai/openai_embedder.py
--rw-r--r--   0        0        0     1709 2024-02-13 21:03:08.339951 rag4p-0.5.0/rag4p/integrations/openai/openai_question_generator.py
--rw-r--r--   0        0        0        0 2024-05-11 09:39:07.588936 rag4p-0.5.0/rag4p/integrations/openai/quality/__init__.py
--rw-r--r--   0        0        0     1828 2024-05-11 10:32:57.682591 rag4p-0.5.0/rag4p/integrations/openai/quality/openai_answer_quality_service.py
--rw-r--r--   0        0        0       26 2024-03-11 09:33:23.149502 rag4p-0.5.0/rag4p/integrations/weaviate/__init__.py
--rw-r--r--   0        0        0     2930 2024-03-11 09:33:23.144857 rag4p-0.5.0/rag4p/integrations/weaviate/access_weaviate.py
--rw-r--r--   0        0        0     1001 2024-02-06 22:07:59.527805 rag4p-0.5.0/rag4p/integrations/weaviate/chunk_collection.py
--rw-r--r--   0        0        0     1369 2024-05-28 10:35:20.920986 rag4p-0.5.0/rag4p/integrations/weaviate/weaviate_content_store.py
--rw-r--r--   0        0        0     4610 2024-05-21 18:55:01.151138 rag4p-0.5.0/rag4p/integrations/weaviate/weaviate_retriever.py
--rw-r--r--   0        0        0        0 2024-02-13 20:01:14.586737 rag4p-0.5.0/rag4p/rag/__init__.py
--rw-r--r--   0        0        0        0 2024-02-13 20:01:31.907902 rag4p-0.5.0/rag4p/rag/embedding/__init__.py
--rw-r--r--   0        0        0      257 2024-05-28 10:35:20.929707 rag4p-0.5.0/rag4p/rag/embedding/embedder.py
--rw-r--r--   0        0        0        0 2024-02-13 20:01:59.778652 rag4p-0.5.0/rag4p/rag/embedding/local/__init__.py
--rw-r--r--   0        0        0     1500 2024-05-28 10:35:20.944520 rag4p-0.5.0/rag4p/rag/embedding/local/onnx_embedder.py
--rw-r--r--   0        0        0        0 2024-02-13 20:03:17.496572 rag4p-0.5.0/rag4p/rag/generation/__init__.py
--rw-r--r--   0        0        0      262 2024-02-13 22:23:33.009410 rag4p-0.5.0/rag4p/rag/generation/answer_generator.py
--rw-r--r--   0        0        0        0 2024-02-13 22:24:49.086889 rag4p-0.5.0/rag4p/rag/generation/chat/__init__.py
--rw-r--r--   0        0        0      875 2024-02-13 22:46:03.836482 rag4p-0.5.0/rag4p/rag/generation/chat/chat_prompt.py
--rw-r--r--   0        0        0      592 2024-02-15 14:06:38.894059 rag4p-0.5.0/rag4p/rag/generation/observed_answer_generator.py
--rw-r--r--   0        0        0        0 2024-02-13 20:08:51.049910 rag4p-0.5.0/rag4p/rag/generation/quality/__init__.py
--rw-r--r--   0        0        0      178 2024-01-21 10:12:21.187448 rag4p-0.5.0/rag4p/rag/generation/quality/answer_from_context_quality.py
--rw-r--r--   0        0        0      532 2024-02-13 22:23:33.021369 rag4p-0.5.0/rag4p/rag/generation/quality/answer_quality.py
--rw-r--r--   0        0        0     4371 2024-05-18 10:20:51.530679 rag4p-0.5.0/rag4p/rag/generation/quality/answer_quality_service.py
--rw-r--r--   0        0        0      418 2024-01-21 09:11:19.307021 rag4p-0.5.0/rag4p/rag/generation/quality/answer_to_question_quality.py
--rw-r--r--   0        0        0      155 2024-01-28 16:24:26.211097 rag4p-0.5.0/rag4p/rag/generation/question_generator.py
--rw-r--r--   0        0        0     1710 2024-02-15 14:10:18.771548 rag4p-0.5.0/rag4p/rag/generation/question_generator_service.py
--rw-r--r--   0        0        0        0 2024-02-13 20:18:42.944968 rag4p-0.5.0/rag4p/rag/model/__init__.py
--rw-r--r--   0        0        0      494 2024-01-21 16:30:55.882221 rag4p-0.5.0/rag4p/rag/model/chunk.py
--rw-r--r--   0        0        0      282 2024-02-15 14:10:18.764160 rag4p-0.5.0/rag4p/rag/model/relevant_chunk.py
--rw-r--r--   0        0        0        0 2024-02-13 20:10:33.450731 rag4p-0.5.0/rag4p/rag/retrieval/__init__.py
--rw-r--r--   0        0        0      917 2024-02-15 14:20:29.071323 rag4p-0.5.0/rag4p/rag/retrieval/observed_retriever.py
--rw-r--r--   0        0        0        0 2024-02-13 20:11:00.416743 rag4p-0.5.0/rag4p/rag/retrieval/quality/__init__.py
--rw-r--r--   0        0        0      259 2024-01-21 12:16:35.290144 rag4p-0.5.0/rag4p/rag/retrieval/quality/question_answer_record.py
--rw-r--r--   0        0        0      337 2024-01-21 11:47:35.273879 rag4p-0.5.0/rag4p/rag/retrieval/quality/retrieval_quality.py
--rw-r--r--   0        0        0     1759 2024-05-17 15:11:07.973126 rag4p-0.5.0/rag4p/rag/retrieval/quality/retrieval_quality_service.py
--rw-r--r--   0        0        0      481 2024-01-17 15:45:56.775642 rag4p-0.5.0/rag4p/rag/retrieval/retrieval_output.py
--rw-r--r--   0        0        0      500 2024-02-15 14:20:29.076513 rag4p-0.5.0/rag4p/rag/retrieval/retrieval_strategy.py
--rw-r--r--   0        0        0      897 2024-02-15 14:33:56.290130 rag4p-0.5.0/rag4p/rag/retrieval/retriever.py
--rw-r--r--   0        0        0        0 2024-02-13 20:13:14.325777 rag4p-0.5.0/rag4p/rag/retrieval/strategies/__init__.py
--rw-r--r--   0        0        0     4133 2024-05-20 08:02:56.131116 rag4p-0.5.0/rag4p/rag/retrieval/strategies/document_retrieval_strategy.py
--rw-r--r--   0        0        0     1346 2024-02-15 14:18:36.054148 rag4p-0.5.0/rag4p/rag/retrieval/strategies/topn_retrieval_strategy.py
--rw-r--r--   0        0        0     2563 2024-02-15 14:18:36.048293 rag4p-0.5.0/rag4p/rag/retrieval/strategies/window_retrieval_strategy.py
--rw-r--r--   0        0        0        0 2024-02-13 20:14:17.876016 rag4p-0.5.0/rag4p/rag/store/__init__.py
--rw-r--r--   0        0        0      527 2024-05-28 10:35:20.940585 rag4p-0.5.0/rag4p/rag/store/content_store.py
--rw-r--r--   0        0        0        0 2024-02-13 20:14:47.220156 rag4p-0.5.0/rag4p/rag/store/local/__init__.py
--rw-r--r--   0        0        0     3782 2024-05-28 12:10:21.269060 rag4p-0.5.0/rag4p/rag/store/local/internal_content_store.py
--rw-r--r--   0        0        0        0 2024-01-18 17:24:10.044644 rag4p-0.5.0/rag4p/rag/tracker/__init__.py
--rw-r--r--   0        0        0     1304 2024-01-21 14:50:45.211063 rag4p-0.5.0/rag4p/rag/tracker/rag_observer.py
--rw-r--r--   0        0        0      108 2024-02-15 14:33:56.284091 rag4p-0.5.0/rag4p/rag/tracker/rag_tracker.py
--rw-r--r--   0        0        0        0 2024-01-17 16:06:54.281693 rag4p-0.5.0/rag4p/util/__init__.py
--rw-r--r--   0        0        0     3363 2024-01-21 09:28:32.748688 rag4p-0.5.0/rag4p/util/key_loader.py
--rw-r--r--   0        0        0      665 2024-05-26 09:38:07.538060 rag4p-0.5.0/rag4p/vasa_content_reader.py
--rw-r--r--   0        0        0     4337 1970-01-01 00:00:00.000000 rag4p-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     3266 2024-05-20 08:34:12.059855 rag4p-0.5.1/README.md
+-rw-r--r--   0        0        0      781 2024-05-28 14:33:42.398918 rag4p-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-17 15:16:40.886501 rag4p-0.5.1/rag4p/__init__.py
+-rw-r--r--   0        0        0     3546 2024-05-11 10:19:26.281070 rag4p-0.5.1/rag4p/app_complete_local.py
+-rw-r--r--   0        0        0     3224 2024-02-15 14:42:08.665322 rag4p-0.5.1/rag4p/app_complete_weaviate.py
+-rw-r--r--   0        0        0     1154 2024-02-15 14:50:41.830101 rag4p-0.5.1/rag4p/app_generation_answer_generator.py
+-rw-r--r--   0        0        0     1318 2024-05-11 10:19:26.290206 rag4p-0.5.1/rag4p/app_generation_answer_quality.py
+-rw-r--r--   0        0        0     1292 2024-05-11 10:24:23.583279 rag4p-0.5.1/rag4p/app_generation_answer_quality_ollama.py
+-rw-r--r--   0        0        0     2708 2024-02-15 15:49:18.900194 rag4p-0.5.1/rag4p/app_generation_question_generator.py
+-rw-r--r--   0        0        0     1432 2024-02-15 15:31:45.716697 rag4p-0.5.1/rag4p/app_generation_questions_generator_vasa.py
+-rw-r--r--   0        0        0     1214 2024-02-15 15:59:09.706810 rag4p-0.5.1/rag4p/app_indexing_local.py
+-rw-r--r--   0        0        0     2330 2024-03-11 09:33:23.161900 rag4p-0.5.1/rag4p/app_indexing_weaviate.py
+-rw-r--r--   0        0        0     1254 2024-02-15 15:31:45.728308 rag4p-0.5.1/rag4p/app_retrieval_quality_vasa.py
+-rw-r--r--   0        0        0     1514 2024-05-15 14:45:34.878603 rag4p-0.5.1/rag4p/app_retrieval_retriever_local.py
+-rw-r--r--   0        0        0     1800 2024-05-21 18:57:47.887764 rag4p-0.5.1/rag4p/app_retrieval_retriever_weaviate.py
+-rw-r--r--   0        0        0     1878 2024-02-15 15:31:45.712149 rag4p-0.5.1/rag4p/app_retrieval_strategy.py
+-rw-r--r--   0        0        0      429 2024-01-31 07:51:24.674544 rag4p-0.5.1/rag4p/app_weaviate_info.py
+-rw-r--r--   0        0        0        0 2024-01-17 15:16:40.886501 rag4p-0.5.1/rag4p/indexing/__init__.py
+-rw-r--r--   0        0        0      512 2024-05-26 09:53:31.685711 rag4p-0.5.1/rag4p/indexing/content_reader.py
+-rw-r--r--   0        0        0      793 2024-05-26 09:53:31.672641 rag4p-0.5.1/rag4p/indexing/indexing_service.py
+-rw-r--r--   0        0        0      232 2024-01-17 15:25:27.590307 rag4p-0.5.1/rag4p/indexing/input_document.py
+-rw-r--r--   0        0        0      876 2024-05-26 09:53:31.688377 rag4p-0.5.1/rag4p/indexing/jsonl_content_reader.py
+-rw-r--r--   0        0        0      285 2024-02-13 20:32:37.812960 rag4p-0.5.1/rag4p/indexing/splitter.py
+-rw-r--r--   0        0        0        0 2024-02-13 19:57:32.062188 rag4p-0.5.1/rag4p/indexing/splitters/__init__.py
+-rw-r--r--   0        0        0     1356 2024-02-13 20:28:11.172941 rag4p-0.5.1/rag4p/indexing/splitters/max_token_splitter.py
+-rw-r--r--   0        0        0      671 2024-02-13 20:32:37.826115 rag4p-0.5.1/rag4p/indexing/splitters/sentence_splitter.py
+-rw-r--r--   0        0        0      474 2024-02-13 20:32:37.822569 rag4p-0.5.1/rag4p/indexing/splitters/single_chunk_splitter.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:16:16.212988 rag4p-0.5.1/rag4p/integrations/__init__.py
+-rw-r--r--   0        0        0      204 2024-05-10 14:28:00.181901 rag4p-0.5.1/rag4p/integrations/ollama/__init__.py
+-rw-r--r--   0        0        0     2361 2024-05-10 15:59:57.265154 rag4p-0.5.1/rag4p/integrations/ollama/access_ollama.py
+-rw-r--r--   0        0        0      808 2024-05-13 07:17:37.558316 rag4p-0.5.1/rag4p/integrations/ollama/ollama_answer_generator.py
+-rw-r--r--   0        0        0      780 2024-05-28 14:18:48.166037 rag4p-0.5.1/rag4p/integrations/ollama/ollama_embedder.py
+-rw-r--r--   0        0        0     1456 2024-05-13 07:17:37.553472 rag4p-0.5.1/rag4p/integrations/ollama/ollama_question_generator.py
+-rw-r--r--   0        0        0        0 2024-05-11 10:09:25.775349 rag4p-0.5.1/rag4p/integrations/ollama/quality/__init__.py
+-rw-r--r--   0        0        0     1429 2024-05-11 10:36:04.986424 rag4p-0.5.1/rag4p/integrations/ollama/quality/ollama_answer_quality_service.py
+-rw-r--r--   0        0        0      429 2024-05-11 10:04:59.548674 rag4p-0.5.1/rag4p/integrations/openai/__init__.py
+-rw-r--r--   0        0        0     1311 2024-05-11 09:33:48.693626 rag4p-0.5.1/rag4p/integrations/openai/openai_answer_generator.py
+-rw-r--r--   0        0        0     1196 2024-05-28 14:18:48.157834 rag4p-0.5.1/rag4p/integrations/openai/openai_embedder.py
+-rw-r--r--   0        0        0     1709 2024-02-13 21:03:08.339951 rag4p-0.5.1/rag4p/integrations/openai/openai_question_generator.py
+-rw-r--r--   0        0        0        0 2024-05-11 09:39:07.588936 rag4p-0.5.1/rag4p/integrations/openai/quality/__init__.py
+-rw-r--r--   0        0        0     1828 2024-05-11 10:32:57.682591 rag4p-0.5.1/rag4p/integrations/openai/quality/openai_answer_quality_service.py
+-rw-r--r--   0        0        0       26 2024-03-11 09:33:23.149502 rag4p-0.5.1/rag4p/integrations/weaviate/__init__.py
+-rw-r--r--   0        0        0     2930 2024-03-11 09:33:23.144857 rag4p-0.5.1/rag4p/integrations/weaviate/access_weaviate.py
+-rw-r--r--   0        0        0     1001 2024-02-06 22:07:59.527805 rag4p-0.5.1/rag4p/integrations/weaviate/chunk_collection.py
+-rw-r--r--   0        0        0     1369 2024-05-28 10:35:20.920986 rag4p-0.5.1/rag4p/integrations/weaviate/weaviate_content_store.py
+-rw-r--r--   0        0        0     4610 2024-05-21 18:55:01.151138 rag4p-0.5.1/rag4p/integrations/weaviate/weaviate_retriever.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:01:14.586737 rag4p-0.5.1/rag4p/rag/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:01:31.907902 rag4p-0.5.1/rag4p/rag/embedding/__init__.py
+-rw-r--r--   0        0        0      378 2024-05-28 14:18:48.170020 rag4p-0.5.1/rag4p/rag/embedding/embedder.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:01:59.778652 rag4p-0.5.1/rag4p/rag/embedding/local/__init__.py
+-rw-r--r--   0        0        0     1621 2024-05-28 14:18:48.174257 rag4p-0.5.1/rag4p/rag/embedding/local/onnx_embedder.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:03:17.496572 rag4p-0.5.1/rag4p/rag/generation/__init__.py
+-rw-r--r--   0        0        0      262 2024-02-13 22:23:33.009410 rag4p-0.5.1/rag4p/rag/generation/answer_generator.py
+-rw-r--r--   0        0        0        0 2024-02-13 22:24:49.086889 rag4p-0.5.1/rag4p/rag/generation/chat/__init__.py
+-rw-r--r--   0        0        0      875 2024-02-13 22:46:03.836482 rag4p-0.5.1/rag4p/rag/generation/chat/chat_prompt.py
+-rw-r--r--   0        0        0      592 2024-02-15 14:06:38.894059 rag4p-0.5.1/rag4p/rag/generation/observed_answer_generator.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:08:51.049910 rag4p-0.5.1/rag4p/rag/generation/quality/__init__.py
+-rw-r--r--   0        0        0      178 2024-01-21 10:12:21.187448 rag4p-0.5.1/rag4p/rag/generation/quality/answer_from_context_quality.py
+-rw-r--r--   0        0        0      532 2024-02-13 22:23:33.021369 rag4p-0.5.1/rag4p/rag/generation/quality/answer_quality.py
+-rw-r--r--   0        0        0     4371 2024-05-18 10:20:51.530679 rag4p-0.5.1/rag4p/rag/generation/quality/answer_quality_service.py
+-rw-r--r--   0        0        0      418 2024-01-21 09:11:19.307021 rag4p-0.5.1/rag4p/rag/generation/quality/answer_to_question_quality.py
+-rw-r--r--   0        0        0      155 2024-01-28 16:24:26.211097 rag4p-0.5.1/rag4p/rag/generation/question_generator.py
+-rw-r--r--   0        0        0     1710 2024-02-15 14:10:18.771548 rag4p-0.5.1/rag4p/rag/generation/question_generator_service.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:18:42.944968 rag4p-0.5.1/rag4p/rag/model/__init__.py
+-rw-r--r--   0        0        0      494 2024-01-21 16:30:55.882221 rag4p-0.5.1/rag4p/rag/model/chunk.py
+-rw-r--r--   0        0        0      282 2024-02-15 14:10:18.764160 rag4p-0.5.1/rag4p/rag/model/relevant_chunk.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:10:33.450731 rag4p-0.5.1/rag4p/rag/retrieval/__init__.py
+-rw-r--r--   0        0        0      917 2024-02-15 14:20:29.071323 rag4p-0.5.1/rag4p/rag/retrieval/observed_retriever.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:11:00.416743 rag4p-0.5.1/rag4p/rag/retrieval/quality/__init__.py
+-rw-r--r--   0        0        0      259 2024-01-21 12:16:35.290144 rag4p-0.5.1/rag4p/rag/retrieval/quality/question_answer_record.py
+-rw-r--r--   0        0        0      337 2024-01-21 11:47:35.273879 rag4p-0.5.1/rag4p/rag/retrieval/quality/retrieval_quality.py
+-rw-r--r--   0        0        0     1759 2024-05-17 15:11:07.973126 rag4p-0.5.1/rag4p/rag/retrieval/quality/retrieval_quality_service.py
+-rw-r--r--   0        0        0      481 2024-01-17 15:45:56.775642 rag4p-0.5.1/rag4p/rag/retrieval/retrieval_output.py
+-rw-r--r--   0        0        0      500 2024-02-15 14:20:29.076513 rag4p-0.5.1/rag4p/rag/retrieval/retrieval_strategy.py
+-rw-r--r--   0        0        0      897 2024-02-15 14:33:56.290130 rag4p-0.5.1/rag4p/rag/retrieval/retriever.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:13:14.325777 rag4p-0.5.1/rag4p/rag/retrieval/strategies/__init__.py
+-rw-r--r--   0        0        0     4133 2024-05-20 08:02:56.131116 rag4p-0.5.1/rag4p/rag/retrieval/strategies/document_retrieval_strategy.py
+-rw-r--r--   0        0        0     1346 2024-02-15 14:18:36.054148 rag4p-0.5.1/rag4p/rag/retrieval/strategies/topn_retrieval_strategy.py
+-rw-r--r--   0        0        0     2563 2024-02-15 14:18:36.048293 rag4p-0.5.1/rag4p/rag/retrieval/strategies/window_retrieval_strategy.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:14:17.876016 rag4p-0.5.1/rag4p/rag/store/__init__.py
+-rw-r--r--   0        0        0      527 2024-05-28 10:35:20.940585 rag4p-0.5.1/rag4p/rag/store/content_store.py
+-rw-r--r--   0        0        0        0 2024-02-13 20:14:47.220156 rag4p-0.5.1/rag4p/rag/store/local/__init__.py
+-rw-r--r--   0        0        0     4183 2024-05-28 14:32:17.740894 rag4p-0.5.1/rag4p/rag/store/local/internal_content_store.py
+-rw-r--r--   0        0        0        0 2024-01-18 17:24:10.044644 rag4p-0.5.1/rag4p/rag/tracker/__init__.py
+-rw-r--r--   0        0        0     1304 2024-01-21 14:50:45.211063 rag4p-0.5.1/rag4p/rag/tracker/rag_observer.py
+-rw-r--r--   0        0        0      108 2024-02-15 14:33:56.284091 rag4p-0.5.1/rag4p/rag/tracker/rag_tracker.py
+-rw-r--r--   0        0        0        0 2024-01-17 16:06:54.281693 rag4p-0.5.1/rag4p/util/__init__.py
+-rw-r--r--   0        0        0     3363 2024-01-21 09:28:32.748688 rag4p-0.5.1/rag4p/util/key_loader.py
+-rw-r--r--   0        0        0      665 2024-05-26 09:38:07.538060 rag4p-0.5.1/rag4p/vasa_content_reader.py
+-rw-r--r--   0        0        0     4337 1970-01-01 00:00:00.000000 rag4p-0.5.1/PKG-INFO
```

### Comparing `rag4p-0.5.0/README.md` & `rag4p-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/pyproject.toml` & `rag4p-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rag4p"
-version = "0.5.0"
+version = "0.5.1"
 description = "This project I use a lot for workshops, it contains some utils for splitters, tokenizers, and a weaviate client that I reuse a lot"
 authors = ["Jettro Coenradie <jettro.coenradie@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 nltk = "^3.8.1"
```

### Comparing `rag4p-0.5.0/rag4p/app_complete_local.py` & `rag4p-0.5.1/rag4p/app_complete_local.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/app_complete_weaviate.py` & `rag4p-0.5.1/rag4p/app_complete_weaviate.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/app_generation_answer_generator.py` & `rag4p-0.5.1/rag4p/app_generation_answer_generator.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/app_generation_answer_quality.py` & `rag4p-0.5.1/rag4p/app_generation_answer_quality.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/app_generation_answer_quality_ollama.py` & `rag4p-0.5.1/rag4p/app_generation_answer_quality_ollama.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/app_generation_question_generator.py` & `rag4p-0.5.1/rag4p/app_generation_question_generator.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/app_generation_questions_generator_vasa.py` & `rag4p-0.5.1/rag4p/app_generation_questions_generator_vasa.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/app_indexing_local.py` & `rag4p-0.5.1/rag4p/app_indexing_local.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/app_indexing_weaviate.py` & `rag4p-0.5.1/rag4p/app_indexing_weaviate.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/app_retrieval_quality_vasa.py` & `rag4p-0.5.1/rag4p/app_retrieval_quality_vasa.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/app_retrieval_retriever_local.py` & `rag4p-0.5.1/rag4p/app_retrieval_retriever_local.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/app_retrieval_retriever_weaviate.py` & `rag4p-0.5.1/rag4p/app_retrieval_retriever_weaviate.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/app_retrieval_strategy.py` & `rag4p-0.5.1/rag4p/app_retrieval_strategy.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/indexing/content_reader.py` & `rag4p-0.5.1/rag4p/indexing/content_reader.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/indexing/indexing_service.py` & `rag4p-0.5.1/rag4p/indexing/indexing_service.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/indexing/jsonl_content_reader.py` & `rag4p-0.5.1/rag4p/indexing/jsonl_content_reader.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/indexing/splitters/max_token_splitter.py` & `rag4p-0.5.1/rag4p/indexing/splitters/max_token_splitter.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/indexing/splitters/sentence_splitter.py` & `rag4p-0.5.1/rag4p/indexing/splitters/sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/integrations/ollama/access_ollama.py` & `rag4p-0.5.1/rag4p/integrations/ollama/access_ollama.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/integrations/ollama/ollama_answer_generator.py` & `rag4p-0.5.1/rag4p/integrations/ollama/ollama_answer_generator.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/integrations/ollama/ollama_embedder.py` & `rag4p-0.5.1/rag4p/integrations/ollama/ollama_embedder.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,12 +8,19 @@
     Embedder that uses Ollama's API to embed text.
     """
 
     def __init__(self, access_ollama: AccessOllama, model: str = DEFAULT_EMBEDDING_MODEL):
         self.ollama = access_ollama
         self.model = model
 
+    def model(self) -> str:
+        return self.model
+
     def identifier(self) -> str:
-        return f"ollama-embedder-{self.model}"
+        return f"{self.supplier().lower()}-embedder-{self.model.lower()}"
 
     def embed(self, text: str) -> [float]:
         return self.ollama.generate_embedding(text, model=self.model)
+
+    @staticmethod
+    def supplier() -> str:
+        return "Ollama"
```

### Comparing `rag4p-0.5.0/rag4p/integrations/ollama/ollama_question_generator.py` & `rag4p-0.5.1/rag4p/integrations/ollama/ollama_question_generator.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/integrations/ollama/quality/ollama_answer_quality_service.py` & `rag4p-0.5.1/rag4p/integrations/ollama/quality/ollama_answer_quality_service.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/integrations/openai/openai_answer_generator.py` & `rag4p-0.5.1/rag4p/integrations/openai/openai_answer_generator.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/integrations/openai/openai_embedder.py` & `rag4p-0.5.1/rag4p/integrations/openai/openai_embedder.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,15 +15,22 @@
         self.client = OpenAI(
             # This is the default and can be omitted
             api_key=api_key,
         )
 
         self.embedding_model = embedding_model
 
+    def model(self) -> str:
+        return self.embedding_model
+
     def identifier(self) -> str:
-        return f"openai-embedder-{self.embedding_model}"
+        return f"{self.supplier().lower()}-embedder-{self.embedding_model.lower()}"
 
     def embed(self, text: str) -> [float]:
         response = self.client.embeddings.create(input=text, model=self.embedding_model, encoding_format="float")
         embeddings = response.data
 
         return embeddings[0].embedding
+
+    @staticmethod
+    def supplier() -> str:
+        return "OpenAI"
```

### Comparing `rag4p-0.5.0/rag4p/integrations/openai/openai_question_generator.py` & `rag4p-0.5.1/rag4p/integrations/openai/openai_question_generator.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/integrations/openai/quality/openai_answer_quality_service.py` & `rag4p-0.5.1/rag4p/integrations/openai/quality/openai_answer_quality_service.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/integrations/weaviate/access_weaviate.py` & `rag4p-0.5.1/rag4p/integrations/weaviate/access_weaviate.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/integrations/weaviate/chunk_collection.py` & `rag4p-0.5.1/rag4p/integrations/weaviate/chunk_collection.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/integrations/weaviate/weaviate_content_store.py` & `rag4p-0.5.1/rag4p/integrations/weaviate/weaviate_content_store.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/integrations/weaviate/weaviate_retriever.py` & `rag4p-0.5.1/rag4p/integrations/weaviate/weaviate_retriever.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/rag/embedding/local/onnx_embedder.py` & `rag4p-0.5.1/rag4p/rag/embedding/local/onnx_embedder.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,17 @@
     def __init__(self, max_length: int = 512):
         self.max_length = max_length
         self.tokenizer = Tokenizer.from_file("../data/tokenizer.json")
         self.tokenizer.enable_truncation(max_length=max_length)
         self.tokenizer.enable_padding(pad_to_multiple_of=1)
         self.ort_sess = ort.InferenceSession('../data/all-minilm-l6-v2-q.onnx')
 
+    def model(self) -> str:
+        return "MiniLM"
+
     def identifier(self) -> str:
         return "onnx-embedder-mini-lm"
 
     def embed(self, text: str) -> List[float]:
         tokens = self.tokenizer.encode(text, add_special_tokens=True)
 
         # Inference
@@ -33,7 +36,11 @@
             'token_type_ids': (np.array([tokens.type_ids])),
         })
         token_embeddings = np.array(token_embeddings)
 
         # Mean Pooling (note: assumes that there are no padded elements)
         embeddings = np.mean(token_embeddings, axis=2)
         return embeddings[0][0]
+
+    @staticmethod
+    def supplier() -> str:
+        return "ONNX"
```

### Comparing `rag4p-0.5.0/rag4p/rag/generation/chat/chat_prompt.py` & `rag4p-0.5.1/rag4p/rag/generation/chat/chat_prompt.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/rag/generation/observed_answer_generator.py` & `rag4p-0.5.1/rag4p/rag/generation/observed_answer_generator.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/rag/generation/quality/answer_quality.py` & `rag4p-0.5.1/rag4p/rag/generation/quality/answer_quality.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/rag/generation/quality/answer_quality_service.py` & `rag4p-0.5.1/rag4p/rag/generation/quality/answer_quality_service.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/rag/generation/question_generator_service.py` & `rag4p-0.5.1/rag4p/rag/generation/question_generator_service.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/rag/retrieval/observed_retriever.py` & `rag4p-0.5.1/rag4p/rag/retrieval/observed_retriever.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/rag/retrieval/quality/retrieval_quality_service.py` & `rag4p-0.5.1/rag4p/rag/retrieval/quality/retrieval_quality_service.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/rag/retrieval/retriever.py` & `rag4p-0.5.1/rag4p/rag/retrieval/retriever.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/rag/retrieval/strategies/document_retrieval_strategy.py` & `rag4p-0.5.1/rag4p/rag/retrieval/strategies/document_retrieval_strategy.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/rag/retrieval/strategies/topn_retrieval_strategy.py` & `rag4p-0.5.1/rag4p/rag/retrieval/strategies/topn_retrieval_strategy.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/rag/retrieval/strategies/window_retrieval_strategy.py` & `rag4p-0.5.1/rag4p/rag/retrieval/strategies/window_retrieval_strategy.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/rag/store/content_store.py` & `rag4p-0.5.1/rag4p/rag/store/content_store.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/rag/store/local/internal_content_store.py` & `rag4p-0.5.1/rag4p/rag/store/local/internal_content_store.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,24 @@
 
 
 class InternalContentStore(ContentStore, Retriever):
     """
     The internal content stores stores the chunks in memory, it acts as a normal content store, but it als contains
     all the methods from a retriever, so it can be used as a retriever as well. This is useful for testing purposes.
     """
+
     def __init__(self, embedder: Embedder):
-        super().__init__({'name': 'internal-content-store', 'embedder': embedder.identifier()})
+        super().__init__(
+            {
+                'name': 'internal-content-store',
+                'embedder': embedder.identifier(),
+                'supplier': embedder.supplier(),
+                'model': embedder.model()
+            }
+        )
         self.embedder = embedder
         self.vector_store = pd.DataFrame(columns=['chunk_id', 'chunk', 'embedding'])
 
     def store(self, chunks: List[Chunk]):
         for chunk in chunks:
             self.__store_chunk(chunk)
 
@@ -67,30 +75,35 @@
 
         return found_chunk.iloc[0]['chunk']
 
     def loop_over_chunks(self):
         for index, row in self.vector_store.iterrows():
             yield row['chunk']
 
-    def backup(self, path: str = 'internal_content_store'):
+    def backup(self, path: str):
         # Save the DataFrame to a pickle file
         with open(f'{path}.pickle', 'wb') as f:
             pickle.dump(self.vector_store, f)
 
         # Save the metadata to a JSON file
         with open(f'{path}_metadata.json', 'w') as f:
             json.dump(self._metadata, f)
 
     @classmethod
-    def load_from_backup(cls, embedder: Embedder, path: str = 'internal_content_store'):
+    def load_from_backup(cls, embedder: Embedder, path: str):
         # Create an instance of the class
         instance = cls(embedder)
 
         # Load the DataFrame from the pickle file
         with open(f'{path}.pickle', 'rb') as f:
             instance.vector_store = pickle.load(f)
 
         # Load the metadata from the JSON file
         with open(f'{path}_metadata.json', 'r') as f:
             instance._metadata = json.load(f)
 
+        if 'embedder' in instance._metadata:
+            if instance._metadata['embedder'] != embedder.identifier():
+                raise Exception(f"Embedder {embedder.identifier()} does not match the one in the backup: "
+                                f"{instance._metadata['embedder']}")
+
         return instance
```

### Comparing `rag4p-0.5.0/rag4p/rag/tracker/rag_observer.py` & `rag4p-0.5.1/rag4p/rag/tracker/rag_observer.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/util/key_loader.py` & `rag4p-0.5.1/rag4p/util/key_loader.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/rag4p/vasa_content_reader.py` & `rag4p-0.5.1/rag4p/vasa_content_reader.py`

 * *Files identical despite different names*

### Comparing `rag4p-0.5.0/PKG-INFO` & `rag4p-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rag4p
-Version: 0.5.0
+Version: 0.5.1
 Summary: This project I use a lot for workshops, it contains some utils for splitters, tokenizers, and a weaviate client that I reuse a lot
 Author: Jettro Coenradie
 Author-email: jettro.coenradie@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

