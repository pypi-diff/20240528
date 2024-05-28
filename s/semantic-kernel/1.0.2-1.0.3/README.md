# Comparing `tmp/semantic_kernel-1.0.2.tar.gz` & `tmp/semantic_kernel-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-1.0.2.tar", max compression
+gzip compressed data, was "semantic_kernel-1.0.3.tar", max compression
```

## Comparing `semantic_kernel-1.0.2.tar` & `semantic_kernel-1.0.3.tar`

### file list

```diff
@@ -1,249 +1,249 @@
--rw-r--r--   0        0        0     1186 2024-03-13 15:37:17.045380 semantic_kernel-1.0.2/pip/README.md
--rw-r--r--   0        0        0     4591 2024-05-23 18:12:45.972757 semantic_kernel-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      113 2024-04-16 13:30:52.656626 semantic_kernel-1.0.2/semantic_kernel/__init__.py
--rw-r--r--   0        0        0       48 2024-03-13 15:37:17.045380 semantic_kernel-1.0.2/semantic_kernel/connectors/__init__.py
--rw-r--r--   0        0        0      180 2024-04-16 13:30:52.656626 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/__init__.py
--rw-r--r--   0        0        0     3242 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0      527 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0     7530 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/function_call_behavior.py
--rw-r--r--   0        0        0      768 2024-03-13 15:37:17.045380 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/google_palm/__init__.py
--rw-r--r--   0        0        0     1770 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py
--rw-r--r--   0        0        0    10522 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py
--rw-r--r--   0        0        0     4670 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py
--rw-r--r--   0        0        0     3208 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py
--rw-r--r--   0        0        0     1866 2024-05-16 18:28:06.371055 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/google_palm/settings/google_palm_settings.py
--rw-r--r--   0        0        0      533 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/hugging_face/__init__.py
--rw-r--r--   0        0        0     1163 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py
--rw-r--r--   0        0        0        0 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/hugging_face/services/__init__.py
--rw-r--r--   0        0        0     6673 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
--rw-r--r--   0        0        0     2193 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
--rw-r--r--   0        0        0      600 2024-04-16 13:30:52.656626 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/ollama/__init__.py
--rw-r--r--   0        0        0      779 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py
--rw-r--r--   0        0        0     8459 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py
--rw-r--r--   0        0        0     3991 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py
--rw-r--r--   0        0        0     1882 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py
--rw-r--r--   0        0        0      387 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/ollama/utils.py
--rw-r--r--   0        0        0     2036 2024-05-06 13:16:31.755032 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/__init__.py
--rw-r--r--   0        0        0      246 2024-05-16 18:28:06.371055 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/const.py
--rw-r--r--   0        0        0     2630 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py
--rw-r--r--   0        0        0     3676 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py
--rw-r--r--   0        0        0     3766 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py
--rw-r--r--   0        0        0    11076 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     5309 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py
--rw-r--r--   0        0        0     6096 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     6180 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     3604 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0    24919 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py
--rw-r--r--   0        0        0     3712 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py
--rw-r--r--   0        0        0     4011 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py
--rw-r--r--   0        0        0      230 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_model_types.py
--rw-r--r--   0        0        0     3807 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     6359 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py
--rw-r--r--   0        0        0     3743 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0     1984 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py
--rw-r--r--   0        0        0     3202 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/utils.py
--rw-r--r--   0        0        0     4169 2024-05-16 18:28:06.371055 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/settings/azure_open_ai_settings.py
--rw-r--r--   0        0        0     2060 2024-05-16 18:28:06.371055 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/settings/open_ai_settings.py
--rw-r--r--   0        0        0     3879 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/prompt_execution_settings.py
--rw-r--r--   0        0        0     1733 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/ai/text_completion_client_base.py
--rw-r--r--   0        0        0       48 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/__init__.py
--rw-r--r--   0        0        0      292 2024-05-16 18:28:06.371055 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/astradb/__init__.py
--rw-r--r--   0        0        0     6750 2024-05-22 16:18:31.535428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/astradb/astra_client.py
--rw-r--r--   0        0        0    13396 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py
--rw-r--r--   0        0        0      831 2024-05-21 00:02:54.747516 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/astradb/astradb_settings.py
--rw-r--r--   0        0        0     1601 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/astradb/utils.py
--rw-r--r--   0        0        0      383 2024-05-16 18:28:06.371055 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
--rw-r--r--   0        0        0     1256 2024-05-21 00:02:54.747516 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cognitive_search/azure_ai_search_settings.py
--rw-r--r--   0        0        0    17012 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
--rw-r--r--   0        0        0     7836 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
--rw-r--r--   0        0        0      345 2024-05-16 18:28:06.371055 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb/__init__.py
--rw-r--r--   0        0        0    11153 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py
--rw-r--r--   0        0        0     2295 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py
--rw-r--r--   0        0        0      634 2024-05-21 00:02:54.747516 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmosdb_settings.py
--rw-r--r--   0        0        0     1740 2024-05-21 00:02:54.747516 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py
--rw-r--r--   0        0        0    13097 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py
--rw-r--r--   0        0        0      236 2024-05-21 00:02:54.747516 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb_no_sql/__init__.py
--rw-r--r--   0        0        0     7720 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb_no_sql/azure_cosmosdb_no_sql_memory_store.py
--rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/chroma/__init__.py
--rw-r--r--   0        0        0    14357 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
--rw-r--r--   0        0        0     4597 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/chroma/utils.py
--rw-r--r--   0        0        0      657 2024-05-21 00:02:54.747516 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/memory_settings_base.py
--rw-r--r--   0        0        0      133 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/milvus/__init__.py
--rw-r--r--   0        0        0    16748 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
--rw-r--r--   0        0        0     1422 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/mongodb_atlas/README.md
--rw-r--r--   0        0        0      336 2024-05-16 18:28:06.381055 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/mongodb_atlas/__init__.py
--rw-r--r--   0        0        0    13206 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py
--rw-r--r--   0        0        0      614 2024-05-21 00:02:54.747516 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_settings.py
--rw-r--r--   0        0        0     2267 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/mongodb_atlas/utils.py
--rw-r--r--   0        0        0      309 2024-05-16 18:28:06.381055 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/pinecone/__init__.py
--rw-r--r--   0        0        0    15682 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
--rw-r--r--   0        0        0      556 2024-05-21 00:02:54.747516 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/pinecone/pinecone_settings.py
--rw-r--r--   0        0        0     1154 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/pinecone/utils.py
--rw-r--r--   0        0        0      300 2024-05-16 18:28:06.381055 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/postgres/__init__.py
--rw-r--r--   0        0        0    21197 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
--rw-r--r--   0        0        0      590 2024-05-21 00:02:54.747516 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/postgres/postgres_settings.py
--rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/qdrant/__init__.py
--rw-r--r--   0        0        0    11743 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
--rw-r--r--   0        0        0     1362 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/redis/README.md
--rw-r--r--   0        0        0      276 2024-05-16 18:28:06.381055 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/redis/__init__.py
--rw-r--r--   0        0        0    15945 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/redis/redis_memory_store.py
--rw-r--r--   0        0        0      582 2024-05-21 00:02:54.747516 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/redis/redis_settings.py
--rw-r--r--   0        0        0     3664 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/redis/utils.py
--rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/usearch/__init__.py
--rw-r--r--   0        0        0    23249 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py
--rw-r--r--   0        0        0      298 2024-05-16 18:28:06.381055 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/weaviate/__init__.py
--rw-r--r--   0        0        0    12561 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
--rw-r--r--   0        0        0     1004 2024-05-21 00:02:54.747516 semantic_kernel-1.0.2/semantic_kernel/connectors/memory/weaviate/weaviate_settings.py
--rw-r--r--   0        0        0      549 2024-04-16 13:30:52.656626 semantic_kernel-1.0.2/semantic_kernel/connectors/openai_plugin/__init__.py
--rw-r--r--   0        0        0      764 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py
--rw-r--r--   0        0        0      498 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/openai_plugin/openai_function_execution_parameters.py
--rw-r--r--   0        0        0      976 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/openai_plugin/openai_utils.py
--rw-r--r--   0        0        0      235 2024-04-16 13:30:52.656626 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/__init__.py
--rw-r--r--   0        0        0    11434 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation.py
--rw-r--r--   0        0        0      379 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_expected_response.py
--rw-r--r--   0        0        0     1418 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_parameter.py
--rw-r--r--   0        0        0      378 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_parameter_location.py
--rw-r--r--   0        0        0      236 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_parameter_style.py
--rw-r--r--   0        0        0      658 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_payload.py
--rw-r--r--   0        0        0      731 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_payload_property.py
--rw-r--r--   0        0        0      415 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_run_options.py
--rw-r--r--   0        0        0      426 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/models/rest_api_uri.py
--rw-r--r--   0        0        0     1350 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py
--rw-r--r--   0        0        0     6783 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/openapi_manager.py
--rw-r--r--   0        0        0     8579 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/openapi_parser.py
--rw-r--r--   0        0        0     7252 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/openapi_runner.py
--rw-r--r--   0        0        0      265 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/connectors/search_engine/__init__.py
--rw-r--r--   0        0        0     3401 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/search_engine/bing_connector.py
--rw-r--r--   0        0        0     1165 2024-05-16 18:28:06.381055 semantic_kernel-1.0.2/semantic_kernel/connectors/search_engine/bing_connector_settings.py
--rw-r--r--   0        0        0      299 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/search_engine/connector.py
--rw-r--r--   0        0        0     2954 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/search_engine/google_connector.py
--rw-r--r--   0        0        0     1105 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/telemetry.py
--rw-r--r--   0        0        0      155 2024-04-01 16:45:47.997053 semantic_kernel-1.0.2/semantic_kernel/connectors/utils/__init__.py
--rw-r--r--   0        0        0      906 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/connectors/utils/document_loader.py
--rw-r--r--   0        0        0      123 2024-05-16 18:28:06.381055 semantic_kernel-1.0.2/semantic_kernel/const.py
--rw-r--r--   0        0        0      865 2024-05-06 13:16:31.755032 semantic_kernel-1.0.2/semantic_kernel/contents/__init__.py
--rw-r--r--   0        0        0      215 2024-05-06 13:16:31.755032 semantic_kernel-1.0.2/semantic_kernel/contents/author_role.py
--rw-r--r--   0        0        0    14163 2024-05-22 16:18:31.545428 semantic_kernel-1.0.2/semantic_kernel/contents/chat_history.py
--rw-r--r--   0        0        0    12555 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/contents/chat_message_content.py
--rw-r--r--   0        0        0      364 2024-05-06 13:16:31.755032 semantic_kernel-1.0.2/semantic_kernel/contents/const.py
--rw-r--r--   0        0        0      277 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/contents/finish_reason.py
--rw-r--r--   0        0        0     3997 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/contents/function_call_content.py
--rw-r--r--   0        0        0     4521 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/contents/function_result_content.py
--rw-r--r--   0        0        0      737 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/contents/kernel_content.py
--rw-r--r--   0        0        0    10933 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/contents/streaming_chat_message_content.py
--rw-r--r--   0        0        0      565 2024-05-06 13:16:31.755032 semantic_kernel-1.0.2/semantic_kernel/contents/streaming_content_mixin.py
--rw-r--r--   0        0        0     2637 2024-05-06 13:16:31.755032 semantic_kernel-1.0.2/semantic_kernel/contents/streaming_text_content.py
--rw-r--r--   0        0        0     1976 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/contents/text_content.py
--rw-r--r--   0        0        0      740 2024-05-06 13:16:31.755032 semantic_kernel-1.0.2/semantic_kernel/contents/types.py
--rw-r--r--   0        0        0      886 2024-05-09 23:07:37.265180 semantic_kernel-1.0.2/semantic_kernel/core_plugins/__init__.py
--rw-r--r--   0        0        0     3336 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/core_plugins/conversation_summary_plugin.py
--rw-r--r--   0        0        0     3932 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/core_plugins/http_plugin.py
--rw-r--r--   0        0        0     2378 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/core_plugins/math_plugin.py
--rw-r--r--   0        0        0     5812 2024-05-16 18:28:06.381055 semantic_kernel-1.0.2/semantic_kernel/core_plugins/sessions_python_tool/README.md
--rw-r--r--   0        0        0      341 2024-05-09 23:07:37.265180 semantic_kernel-1.0.2/semantic_kernel/core_plugins/sessions_python_tool/__init__.py
--rw-r--r--   0        0        0     9946 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py
--rw-r--r--   0        0        0     1884 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_settings.py
--rw-r--r--   0        0        0      724 2024-05-09 23:07:37.265180 semantic_kernel-1.0.2/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py
--rw-r--r--   0        0        0     3662 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/core_plugins/text_memory_plugin.py
--rw-r--r--   0        0        0     2658 2024-05-06 13:16:31.765032 semantic_kernel-1.0.2/semantic_kernel/core_plugins/text_plugin.py
--rw-r--r--   0        0        0     8030 2024-05-06 13:16:31.765032 semantic_kernel-1.0.2/semantic_kernel/core_plugins/time_plugin.py
--rw-r--r--   0        0        0     1020 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/core_plugins/wait_plugin.py
--rw-r--r--   0        0        0     1652 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/core_plugins/web_search_engine_plugin.py
--rw-r--r--   0        0        0      626 2024-05-16 18:28:06.381055 semantic_kernel-1.0.2/semantic_kernel/exceptions/__init__.py
--rw-r--r--   0        0        0      727 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/exceptions/content_exceptions.py
--rw-r--r--   0        0        0     1270 2024-05-17 22:45:44.188248 semantic_kernel-1.0.2/semantic_kernel/exceptions/function_exceptions.py
--rw-r--r--   0        0        0     1417 2024-05-17 22:45:44.188248 semantic_kernel-1.0.2/semantic_kernel/exceptions/kernel_exceptions.py
--rw-r--r--   0        0        0      467 2024-05-16 18:28:06.381055 semantic_kernel-1.0.2/semantic_kernel/exceptions/memory_connector_exceptions.py
--rw-r--r--   0        0        0      690 2024-03-15 14:30:59.091994 semantic_kernel-1.0.2/semantic_kernel/exceptions/planner_exceptions.py
--rw-r--r--   0        0        0     1144 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/exceptions/service_exceptions.py
--rw-r--r--   0        0        0     2875 2024-03-15 14:30:59.091994 semantic_kernel-1.0.2/semantic_kernel/exceptions/template_engine_exceptions.py
--rw-r--r--   0        0        0      655 2024-05-17 22:45:44.198248 semantic_kernel-1.0.2/semantic_kernel/filters/auto_function_invocation/auto_function_invocation_context.py
--rw-r--r--   0        0        0      631 2024-05-17 22:45:44.198248 semantic_kernel-1.0.2/semantic_kernel/filters/filter_context_base.py
--rw-r--r--   0        0        0      386 2024-05-17 22:45:44.198248 semantic_kernel-1.0.2/semantic_kernel/filters/filter_types.py
--rw-r--r--   0        0        0      396 2024-05-17 22:45:44.198248 semantic_kernel-1.0.2/semantic_kernel/filters/functions/function_invocation_context.py
--rw-r--r--   0        0        0     6398 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/filters/kernel_filters_extension.py
--rw-r--r--   0        0        0      437 2024-05-17 22:45:44.198248 semantic_kernel-1.0.2/semantic_kernel/filters/prompts/prompt_render_context.py
--rw-r--r--   0        0        0     1009 2024-04-16 13:30:52.656626 semantic_kernel-1.0.2/semantic_kernel/functions/__init__.py
--rw-r--r--   0        0        0     2596 2024-05-23 18:12:45.982757 semantic_kernel-1.0.2/semantic_kernel/functions/function_result.py
--rw-r--r--   0        0        0     1711 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/functions/kernel_arguments.py
--rw-r--r--   0        0        0    10643 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/functions/kernel_function.py
--rw-r--r--   0        0        0     5607 2024-05-23 18:12:45.992757 semantic_kernel-1.0.2/semantic_kernel/functions/kernel_function_decorator.py
--rw-r--r--   0        0        0    18367 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/functions/kernel_function_extension.py
--rw-r--r--   0        0        0     8262 2024-05-23 18:12:45.992757 semantic_kernel-1.0.2/semantic_kernel/functions/kernel_function_from_method.py
--rw-r--r--   0        0        0    16879 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/functions/kernel_function_from_prompt.py
--rw-r--r--   0        0        0     1930 2024-05-23 18:12:45.992757 semantic_kernel-1.0.2/semantic_kernel/functions/kernel_function_metadata.py
--rw-r--r--   0        0        0     2229 2024-05-23 18:12:45.992757 semantic_kernel-1.0.2/semantic_kernel/functions/kernel_parameter_metadata.py
--rw-r--r--   0        0        0    23610 2024-05-23 18:12:45.992757 semantic_kernel-1.0.2/semantic_kernel/functions/kernel_plugin.py
--rw-r--r--   0        0        0      939 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/functions/prompt_rendering_result.py
--rw-r--r--   0        0        0      252 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/functions/types.py
--rw-r--r--   0        0        0    13830 2024-05-22 16:18:31.555428 semantic_kernel-1.0.2/semantic_kernel/kernel.py
--rw-r--r--   0        0        0      462 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/kernel_pydantic.py
--rw-r--r--   0        0        0      257 2024-04-16 13:30:52.656626 semantic_kernel-1.0.2/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     2582 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     4285 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0     7211 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1639 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     6571 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     3675 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0    12124 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0      903 2024-05-09 23:07:37.265180 semantic_kernel-1.0.2/semantic_kernel/planners/__init__.py
--rw-r--r--   0        0        0      605 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py
--rw-r--r--   0        0        0    12968 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py
--rw-r--r--   0        0        0     1667 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py
--rw-r--r--   0        0        0      797 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py
--rw-r--r--   0        0        0     1377 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml
--rw-r--r--   0        0        0      184 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/planners/function_calling_stepwise_planner/step_prompt.txt
--rw-r--r--   0        0        0    14329 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/planners/plan.py
--rw-r--r--   0        0        0     2770 2024-04-16 13:30:52.656626 semantic_kernel-1.0.2/semantic_kernel/planners/planner_extensions.py
--rw-r--r--   0        0        0      568 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/planners/planner_options.py
--rw-r--r--   0        0        0      718 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json
--rw-r--r--   0        0        0     3179 2024-03-15 14:30:59.091994 semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt
--rw-r--r--   0        0        0      142 2024-03-13 15:37:17.055380 semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/__init__.py
--rw-r--r--   0        0        0     5973 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/sequential_planner.py
--rw-r--r--   0        0        0     1125 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/sequential_planner_config.py
--rw-r--r--   0        0        0     4678 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py
--rw-r--r--   0        0        0     4973 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py
--rw-r--r--   0        0        0      634 2024-03-15 14:30:59.091994 semantic_kernel-1.0.2/semantic_kernel/prompt_template/__init__.py
--rw-r--r--   0        0        0      756 2024-05-06 13:16:31.765032 semantic_kernel-1.0.2/semantic_kernel/prompt_template/const.py
--rw-r--r--   0        0        0     4787 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/prompt_template/handlebars_prompt_template.py
--rw-r--r--   0        0        0      871 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/prompt_template/input_variable.py
--rw-r--r--   0        0        0     4972 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/prompt_template/jinja2_prompt_template.py
--rw-r--r--   0        0        0     6735 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/prompt_template/kernel_prompt_template.py
--rw-r--r--   0        0        0     2991 2024-05-16 18:28:06.381055 semantic_kernel-1.0.2/semantic_kernel/prompt_template/prompt_template_base.py
--rw-r--r--   0        0        0     5535 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/prompt_template/prompt_template_config.py
--rw-r--r--   0        0        0      477 2024-03-15 14:30:59.091994 semantic_kernel-1.0.2/semantic_kernel/prompt_template/utils/__init__.py
--rw-r--r--   0        0        0     4615 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py
--rw-r--r--   0        0        0     2450 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py
--rw-r--r--   0        0        0     2116 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/prompt_template/utils/template_function_helpers.py
--rw-r--r--   0        0        0        0 2024-04-01 16:45:47.997053 semantic_kernel-1.0.2/semantic_kernel/py.typed
--rw-r--r--   0        0        0      545 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/reliability/kernel_reliability_extension.py
--rw-r--r--   0        0        0      999 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      679 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/reliability/retry_mechanism_base.py
--rw-r--r--   0        0        0     2609 2024-05-23 18:12:45.992757 semantic_kernel-1.0.2/semantic_kernel/schema/kernel_json_schema_builder.py
--rw-r--r--   0        0        0      157 2024-04-16 13:30:52.656626 semantic_kernel-1.0.2/semantic_kernel/services/__init__.py
--rw-r--r--   0        0        0     1851 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/services/ai_service_client_base.py
--rw-r--r--   0        0        0     2624 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/services/ai_service_selector.py
--rw-r--r--   0        0        0     6202 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/services/kernel_services_extension.py
--rw-r--r--   0        0        0     1115 2024-03-13 15:37:17.065380 semantic_kernel-1.0.2/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      251 2024-03-13 15:37:17.065380 semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     7447 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2413 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0     3908 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/named_arg_block.py
--rw-r--r--   0        0        0      346 2024-03-13 15:37:17.065380 semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1672 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2376 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2924 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6569 2024-05-22 16:18:31.565428 semantic_kernel-1.0.2/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0      630 2024-03-13 15:37:17.065380 semantic_kernel-1.0.2/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0      673 2024-03-13 15:37:17.065380 semantic_kernel-1.0.2/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     6271 2024-05-22 16:18:31.575428 semantic_kernel-1.0.2/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      461 2024-03-13 15:37:17.065380 semantic_kernel-1.0.2/semantic_kernel/text/__init__.py
--rw-r--r--   0        0        0      654 2024-05-22 16:18:31.575428 semantic_kernel-1.0.2/semantic_kernel/text/function_extension.py
--rw-r--r--   0        0        0     8531 2024-05-22 16:18:31.575428 semantic_kernel-1.0.2/semantic_kernel/text/text_chunker.py
--rw-r--r--   0        0        0      498 2024-05-22 16:18:31.575428 semantic_kernel-1.0.2/semantic_kernel/utils/chat.py
--rw-r--r--   0        0        0      841 2024-05-22 16:18:31.575428 semantic_kernel-1.0.2/semantic_kernel/utils/experimental_decorator.py
--rw-r--r--   0        0        0      276 2024-03-13 15:37:17.065380 semantic_kernel-1.0.2/semantic_kernel/utils/logging.py
--rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-1.0.2/semantic_kernel/utils/naming.py
--rw-r--r--   0        0        0      269 2024-05-22 16:18:31.575428 semantic_kernel-1.0.2/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     4516 1970-01-01 00:00:00.000000 semantic_kernel-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1186 2024-03-13 15:37:17.045380 semantic_kernel-1.0.3/pip/README.md
+-rw-r--r--   0        0        0     4989 2024-05-28 20:52:31.838799 semantic_kernel-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      113 2024-04-16 13:30:52.656626 semantic_kernel-1.0.3/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0       48 2024-03-13 15:37:17.045380 semantic_kernel-1.0.3/semantic_kernel/connectors/__init__.py
+-rw-r--r--   0        0        0      180 2024-04-16 13:30:52.656626 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/__init__.py
+-rw-r--r--   0        0        0     3314 2024-05-28 20:52:31.838799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0      846 2024-05-28 20:52:31.838799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0     7531 2024-05-28 20:52:31.838799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/function_call_behavior.py
+-rw-r--r--   0        0        0      768 2024-03-13 15:37:17.045380 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/google_palm/__init__.py
+-rw-r--r--   0        0        0     1800 2024-05-28 20:52:31.838799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py
+-rw-r--r--   0        0        0     9817 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py
+-rw-r--r--   0        0        0     4825 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py
+-rw-r--r--   0        0        0     3024 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py
+-rw-r--r--   0        0        0     1957 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/google_palm/settings/google_palm_settings.py
+-rw-r--r--   0        0        0      533 2024-03-13 15:37:17.055380 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/hugging_face/__init__.py
+-rw-r--r--   0        0        0     1251 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py
+-rw-r--r--   0        0        0        0 2024-03-13 15:37:17.055380 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/hugging_face/services/__init__.py
+-rw-r--r--   0        0        0     6606 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
+-rw-r--r--   0        0        0     2080 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
+-rw-r--r--   0        0        0      600 2024-04-16 13:30:52.656626 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/ollama/__init__.py
+-rw-r--r--   0        0        0      779 2024-05-22 16:18:31.535428 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py
+-rw-r--r--   0        0        0     8316 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py
+-rw-r--r--   0        0        0     3939 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py
+-rw-r--r--   0        0        0     1782 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py
+-rw-r--r--   0        0        0      511 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/ollama/utils.py
+-rw-r--r--   0        0        0     2036 2024-05-06 13:16:31.755032 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0      166 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/const.py
+-rw-r--r--   0        0        0     2611 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py
+-rw-r--r--   0        0        0     3722 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py
+-rw-r--r--   0        0        0     3832 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py
+-rw-r--r--   0        0        0    11045 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     5424 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py
+-rw-r--r--   0        0        0     6034 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     6125 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     3545 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0    25019 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py
+-rw-r--r--   0        0        0     3832 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py
+-rw-r--r--   0        0        0     4030 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py
+-rw-r--r--   0        0        0      230 2024-03-13 15:37:17.055380 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/open_ai_model_types.py
+-rw-r--r--   0        0        0     3740 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     6329 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py
+-rw-r--r--   0        0        0     3672 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0     1669 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py
+-rw-r--r--   0        0        0     3202 2024-05-23 18:12:45.982757 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/utils.py
+-rw-r--r--   0        0        0     4265 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/settings/azure_open_ai_settings.py
+-rw-r--r--   0        0        0     2156 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/settings/open_ai_settings.py
+-rw-r--r--   0        0        0     4015 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/prompt_execution_settings.py
+-rw-r--r--   0        0        0     1689 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0       48 2024-03-13 15:37:17.055380 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/__init__.py
+-rw-r--r--   0        0        0      292 2024-05-16 18:28:06.371055 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/astradb/__init__.py
+-rw-r--r--   0        0        0     7475 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/astradb/astra_client.py
+-rw-r--r--   0        0        0    13392 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py
+-rw-r--r--   0        0        0      880 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/astradb/astradb_settings.py
+-rw-r--r--   0        0        0     1715 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/astradb/utils.py
+-rw-r--r--   0        0        0      383 2024-05-16 18:28:06.371055 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
+-rw-r--r--   0        0        0     1283 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/azure_cognitive_search/azure_ai_search_settings.py
+-rw-r--r--   0        0        0    16568 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
+-rw-r--r--   0        0        0     7901 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
+-rw-r--r--   0        0        0      345 2024-05-16 18:28:06.371055 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/azure_cosmosdb/__init__.py
+-rw-r--r--   0        0        0    10943 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py
+-rw-r--r--   0        0        0     7042 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py
+-rw-r--r--   0        0        0      679 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmosdb_settings.py
+-rw-r--r--   0        0        0     1858 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py
+-rw-r--r--   0        0        0    13450 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py
+-rw-r--r--   0        0        0      236 2024-05-21 00:02:54.747516 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/azure_cosmosdb_no_sql/__init__.py
+-rw-r--r--   0        0        0     8087 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/azure_cosmosdb_no_sql/azure_cosmosdb_no_sql_memory_store.py
+-rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/chroma/__init__.py
+-rw-r--r--   0        0        0    13353 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
+-rw-r--r--   0        0        0     4604 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/chroma/utils.py
+-rw-r--r--   0        0        0      752 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/memory_settings_base.py
+-rw-r--r--   0        0        0      133 2024-03-13 15:37:17.055380 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/milvus/__init__.py
+-rw-r--r--   0        0        0    16802 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
+-rw-r--r--   0        0        0     1422 2024-03-13 15:37:17.055380 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/mongodb_atlas/README.md
+-rw-r--r--   0        0        0      336 2024-05-16 18:28:06.381055 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/mongodb_atlas/__init__.py
+-rw-r--r--   0        0        0    13439 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py
+-rw-r--r--   0        0        0      659 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_settings.py
+-rw-r--r--   0        0        0     2312 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/mongodb_atlas/utils.py
+-rw-r--r--   0        0        0      309 2024-05-16 18:28:06.381055 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/pinecone/__init__.py
+-rw-r--r--   0        0        0    15801 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
+-rw-r--r--   0        0        0      598 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/pinecone/pinecone_settings.py
+-rw-r--r--   0        0        0     1134 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/pinecone/utils.py
+-rw-r--r--   0        0        0      300 2024-05-16 18:28:06.381055 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/postgres/__init__.py
+-rw-r--r--   0        0        0    20860 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
+-rw-r--r--   0        0        0      632 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/postgres/postgres_settings.py
+-rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/qdrant/__init__.py
+-rw-r--r--   0        0        0    10609 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
+-rw-r--r--   0        0        0     1362 2024-03-13 15:37:17.055380 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/redis/README.md
+-rw-r--r--   0        0        0      276 2024-05-16 18:28:06.381055 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/redis/__init__.py
+-rw-r--r--   0        0        0    15707 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/redis/redis_memory_store.py
+-rw-r--r--   0        0        0      615 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/redis/redis_settings.py
+-rw-r--r--   0        0        0     3786 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/redis/utils.py
+-rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/usearch/__init__.py
+-rw-r--r--   0        0        0    23327 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py
+-rw-r--r--   0        0        0      298 2024-05-16 18:28:06.381055 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/weaviate/__init__.py
+-rw-r--r--   0        0        0    13357 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
+-rw-r--r--   0        0        0     1117 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/memory/weaviate/weaviate_settings.py
+-rw-r--r--   0        0        0      549 2024-04-16 13:30:52.656626 semantic_kernel-1.0.3/semantic_kernel/connectors/openai_plugin/__init__.py
+-rw-r--r--   0        0        0      764 2024-05-22 16:18:31.545428 semantic_kernel-1.0.3/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py
+-rw-r--r--   0        0        0      498 2024-05-22 16:18:31.545428 semantic_kernel-1.0.3/semantic_kernel/connectors/openai_plugin/openai_function_execution_parameters.py
+-rw-r--r--   0        0        0      975 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/openai_plugin/openai_utils.py
+-rw-r--r--   0        0        0      235 2024-04-16 13:30:52.656626 semantic_kernel-1.0.3/semantic_kernel/connectors/openapi_plugin/__init__.py
+-rw-r--r--   0        0        0    12231 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation.py
+-rw-r--r--   0        0        0      442 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_expected_response.py
+-rw-r--r--   0        0        0     1474 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_parameter.py
+-rw-r--r--   0        0        0      378 2024-05-23 18:12:45.982757 semantic_kernel-1.0.3/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_parameter_location.py
+-rw-r--r--   0        0        0      236 2024-05-23 18:12:45.982757 semantic_kernel-1.0.3/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_parameter_style.py
+-rw-r--r--   0        0        0      712 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_payload.py
+-rw-r--r--   0        0        0      793 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_payload_property.py
+-rw-r--r--   0        0        0      476 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_run_options.py
+-rw-r--r--   0        0        0      503 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/openapi_plugin/models/rest_api_uri.py
+-rw-r--r--   0        0        0     1405 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py
+-rw-r--r--   0        0        0     6783 2024-05-23 18:12:45.982757 semantic_kernel-1.0.3/semantic_kernel/connectors/openapi_plugin/openapi_manager.py
+-rw-r--r--   0        0        0     8602 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/openapi_plugin/openapi_parser.py
+-rw-r--r--   0        0        0     7379 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/openapi_plugin/openapi_runner.py
+-rw-r--r--   0        0        0      265 2024-03-13 15:37:17.055380 semantic_kernel-1.0.3/semantic_kernel/connectors/search_engine/__init__.py
+-rw-r--r--   0        0        0     3124 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/search_engine/bing_connector.py
+-rw-r--r--   0        0        0     1293 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/search_engine/bing_connector_settings.py
+-rw-r--r--   0        0        0      387 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/search_engine/connector.py
+-rw-r--r--   0        0        0     2722 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/search_engine/google_connector.py
+-rw-r--r--   0        0        0     1099 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/telemetry.py
+-rw-r--r--   0        0        0      155 2024-04-01 16:45:47.997053 semantic_kernel-1.0.3/semantic_kernel/connectors/utils/__init__.py
+-rw-r--r--   0        0        0      907 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/connectors/utils/document_loader.py
+-rw-r--r--   0        0        0      123 2024-05-16 18:28:06.381055 semantic_kernel-1.0.3/semantic_kernel/const.py
+-rw-r--r--   0        0        0      865 2024-05-06 13:16:31.755032 semantic_kernel-1.0.3/semantic_kernel/contents/__init__.py
+-rw-r--r--   0        0        0      216 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/contents/author_role.py
+-rw-r--r--   0        0        0    14587 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/contents/chat_history.py
+-rw-r--r--   0        0        0    10987 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/contents/chat_message_content.py
+-rw-r--r--   0        0        0      364 2024-05-06 13:16:31.755032 semantic_kernel-1.0.3/semantic_kernel/contents/const.py
+-rw-r--r--   0        0        0      278 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/contents/finish_reason.py
+-rw-r--r--   0        0        0     4058 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/contents/function_call_content.py
+-rw-r--r--   0        0        0     4578 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/contents/function_result_content.py
+-rw-r--r--   0        0        0      952 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/contents/kernel_content.py
+-rw-r--r--   0        0        0     9365 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/contents/streaming_chat_message_content.py
+-rw-r--r--   0        0        0      693 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/contents/streaming_content_mixin.py
+-rw-r--r--   0        0        0     2712 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/contents/streaming_text_content.py
+-rw-r--r--   0        0        0     2033 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/contents/text_content.py
+-rw-r--r--   0        0        0      740 2024-05-06 13:16:31.755032 semantic_kernel-1.0.3/semantic_kernel/contents/types.py
+-rw-r--r--   0        0        0      886 2024-05-09 23:07:37.265180 semantic_kernel-1.0.3/semantic_kernel/core_plugins/__init__.py
+-rw-r--r--   0        0        0     3308 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/core_plugins/conversation_summary_plugin.py
+-rw-r--r--   0        0        0     3908 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/core_plugins/http_plugin.py
+-rw-r--r--   0        0        0     2355 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/core_plugins/math_plugin.py
+-rw-r--r--   0        0        0     5812 2024-05-16 18:28:06.381055 semantic_kernel-1.0.3/semantic_kernel/core_plugins/sessions_python_tool/README.md
+-rw-r--r--   0        0        0      341 2024-05-09 23:07:37.265180 semantic_kernel-1.0.3/semantic_kernel/core_plugins/sessions_python_tool/__init__.py
+-rw-r--r--   0        0        0     9943 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py
+-rw-r--r--   0        0        0     2041 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_settings.py
+-rw-r--r--   0        0        0      724 2024-05-09 23:07:37.265180 semantic_kernel-1.0.3/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py
+-rw-r--r--   0        0        0     3617 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/core_plugins/text_memory_plugin.py
+-rw-r--r--   0        0        0     2607 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/core_plugins/text_plugin.py
+-rw-r--r--   0        0        0     7750 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/core_plugins/time_plugin.py
+-rw-r--r--   0        0        0     1014 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/core_plugins/wait_plugin.py
+-rw-r--r--   0        0        0     1450 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/core_plugins/web_search_engine_plugin.py
+-rw-r--r--   0        0        0      626 2024-05-16 18:28:06.381055 semantic_kernel-1.0.3/semantic_kernel/exceptions/__init__.py
+-rw-r--r--   0        0        0      727 2024-03-13 15:37:17.055380 semantic_kernel-1.0.3/semantic_kernel/exceptions/content_exceptions.py
+-rw-r--r--   0        0        0     1334 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/exceptions/function_exceptions.py
+-rw-r--r--   0        0        0     1417 2024-05-17 22:45:44.188248 semantic_kernel-1.0.3/semantic_kernel/exceptions/kernel_exceptions.py
+-rw-r--r--   0        0        0      467 2024-05-16 18:28:06.381055 semantic_kernel-1.0.3/semantic_kernel/exceptions/memory_connector_exceptions.py
+-rw-r--r--   0        0        0      690 2024-03-15 14:30:59.091994 semantic_kernel-1.0.3/semantic_kernel/exceptions/planner_exceptions.py
+-rw-r--r--   0        0        0     1144 2024-03-13 15:37:17.055380 semantic_kernel-1.0.3/semantic_kernel/exceptions/service_exceptions.py
+-rw-r--r--   0        0        0     3143 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/exceptions/template_engine_exceptions.py
+-rw-r--r--   0        0        0      655 2024-05-17 22:45:44.198248 semantic_kernel-1.0.3/semantic_kernel/filters/auto_function_invocation/auto_function_invocation_context.py
+-rw-r--r--   0        0        0      631 2024-05-17 22:45:44.198248 semantic_kernel-1.0.3/semantic_kernel/filters/filter_context_base.py
+-rw-r--r--   0        0        0      386 2024-05-17 22:45:44.198248 semantic_kernel-1.0.3/semantic_kernel/filters/filter_types.py
+-rw-r--r--   0        0        0      396 2024-05-17 22:45:44.198248 semantic_kernel-1.0.3/semantic_kernel/filters/functions/function_invocation_context.py
+-rw-r--r--   0        0        0     6464 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/filters/kernel_filters_extension.py
+-rw-r--r--   0        0        0      437 2024-05-17 22:45:44.198248 semantic_kernel-1.0.3/semantic_kernel/filters/prompts/prompt_render_context.py
+-rw-r--r--   0        0        0     1009 2024-04-16 13:30:52.656626 semantic_kernel-1.0.3/semantic_kernel/functions/__init__.py
+-rw-r--r--   0        0        0     2586 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/functions/function_result.py
+-rw-r--r--   0        0        0     1703 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/functions/kernel_arguments.py
+-rw-r--r--   0        0        0    11134 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/functions/kernel_function.py
+-rw-r--r--   0        0        0     5760 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/functions/kernel_function_decorator.py
+-rw-r--r--   0        0        0    18204 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/functions/kernel_function_extension.py
+-rw-r--r--   0        0        0     8166 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/functions/kernel_function_from_method.py
+-rw-r--r--   0        0        0    16871 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/functions/kernel_function_from_prompt.py
+-rw-r--r--   0        0        0     1912 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/functions/kernel_function_metadata.py
+-rw-r--r--   0        0        0     2345 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/functions/kernel_parameter_metadata.py
+-rw-r--r--   0        0        0    23886 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/functions/kernel_plugin.py
+-rw-r--r--   0        0        0      934 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/functions/prompt_rendering_result.py
+-rw-r--r--   0        0        0      252 2024-05-22 16:18:31.555428 semantic_kernel-1.0.3/semantic_kernel/functions/types.py
+-rw-r--r--   0        0        0    13955 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0      462 2024-05-22 16:18:31.565428 semantic_kernel-1.0.3/semantic_kernel/kernel_pydantic.py
+-rw-r--r--   0        0        0      257 2024-04-16 13:30:52.656626 semantic_kernel-1.0.3/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     2630 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     4655 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0     7028 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1633 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     6846 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     3801 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0    11990 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0      903 2024-05-09 23:07:37.265180 semantic_kernel-1.0.3/semantic_kernel/planners/__init__.py
+-rw-r--r--   0        0        0      605 2024-03-13 15:37:17.055380 semantic_kernel-1.0.3/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py
+-rw-r--r--   0        0        0    12973 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py
+-rw-r--r--   0        0        0     1754 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py
+-rw-r--r--   0        0        0      847 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py
+-rw-r--r--   0        0        0     1377 2024-03-13 15:37:17.055380 semantic_kernel-1.0.3/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml
+-rw-r--r--   0        0        0      184 2024-03-13 15:37:17.055380 semantic_kernel-1.0.3/semantic_kernel/planners/function_calling_stepwise_planner/step_prompt.txt
+-rw-r--r--   0        0        0    15563 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/planners/plan.py
+-rw-r--r--   0        0        0     3034 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/planners/planner_extensions.py
+-rw-r--r--   0        0        0      569 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/planners/planner_options.py
+-rw-r--r--   0        0        0      718 2024-03-13 15:37:17.055380 semantic_kernel-1.0.3/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json
+-rw-r--r--   0        0        0     3179 2024-03-15 14:30:59.091994 semantic_kernel-1.0.3/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt
+-rw-r--r--   0        0        0      142 2024-03-13 15:37:17.055380 semantic_kernel-1.0.3/semantic_kernel/planners/sequential_planner/__init__.py
+-rw-r--r--   0        0        0     6013 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/planners/sequential_planner/sequential_planner.py
+-rw-r--r--   0        0        0     1204 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/planners/sequential_planner/sequential_planner_config.py
+-rw-r--r--   0        0        0     4959 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py
+-rw-r--r--   0        0        0     5099 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py
+-rw-r--r--   0        0        0      634 2024-03-15 14:30:59.091994 semantic_kernel-1.0.3/semantic_kernel/prompt_template/__init__.py
+-rw-r--r--   0        0        0      756 2024-05-06 13:16:31.765032 semantic_kernel-1.0.3/semantic_kernel/prompt_template/const.py
+-rw-r--r--   0        0        0     4890 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/prompt_template/handlebars_prompt_template.py
+-rw-r--r--   0        0        0      968 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/prompt_template/input_variable.py
+-rw-r--r--   0        0        0     5070 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/prompt_template/jinja2_prompt_template.py
+-rw-r--r--   0        0        0     6744 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/prompt_template/kernel_prompt_template.py
+-rw-r--r--   0        0        0     3024 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/prompt_template/prompt_template_base.py
+-rw-r--r--   0        0        0     5787 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/prompt_template/prompt_template_config.py
+-rw-r--r--   0        0        0      477 2024-03-15 14:30:59.091994 semantic_kernel-1.0.3/semantic_kernel/prompt_template/utils/__init__.py
+-rw-r--r--   0        0        0     4615 2024-05-22 16:18:31.565428 semantic_kernel-1.0.3/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py
+-rw-r--r--   0        0        0     2450 2024-05-22 16:18:31.565428 semantic_kernel-1.0.3/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py
+-rw-r--r--   0        0        0     2116 2024-05-22 16:18:31.565428 semantic_kernel-1.0.3/semantic_kernel/prompt_template/utils/template_function_helpers.py
+-rw-r--r--   0        0        0        0 2024-04-01 16:45:47.997053 semantic_kernel-1.0.3/semantic_kernel/py.typed
+-rw-r--r--   0        0        0      545 2024-05-22 16:18:31.565428 semantic_kernel-1.0.3/semantic_kernel/reliability/kernel_reliability_extension.py
+-rw-r--r--   0        0        0      990 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      670 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/reliability/retry_mechanism_base.py
+-rw-r--r--   0        0        0     5878 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/schema/kernel_json_schema_builder.py
+-rw-r--r--   0        0        0      157 2024-04-16 13:30:52.656626 semantic_kernel-1.0.3/semantic_kernel/services/__init__.py
+-rw-r--r--   0        0        0     1852 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/services/ai_service_client_base.py
+-rw-r--r--   0        0        0     2624 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/services/ai_service_selector.py
+-rw-r--r--   0        0        0     6504 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/services/kernel_services_extension.py
+-rw-r--r--   0        0        0     1115 2024-03-13 15:37:17.065380 semantic_kernel-1.0.3/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0      606 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      251 2024-03-13 15:37:17.065380 semantic_kernel-1.0.3/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     7449 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     2458 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0     3956 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/template_engine/blocks/named_arg_block.py
+-rw-r--r--   0        0        0      346 2024-03-13 15:37:17.065380 semantic_kernel-1.0.3/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1818 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2414 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2933 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6620 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0      611 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0      654 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     6308 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      461 2024-03-13 15:37:17.065380 semantic_kernel-1.0.3/semantic_kernel/text/__init__.py
+-rw-r--r--   0        0        0      644 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/text/function_extension.py
+-rw-r--r--   0        0        0     8495 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/text/text_chunker.py
+-rw-r--r--   0        0        0      498 2024-05-22 16:18:31.575428 semantic_kernel-1.0.3/semantic_kernel/utils/chat.py
+-rw-r--r--   0        0        0      950 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/utils/experimental_decorator.py
+-rw-r--r--   0        0        0      280 2024-05-28 20:52:31.848799 semantic_kernel-1.0.3/semantic_kernel/utils/logging.py
+-rw-r--r--   0        0        0      565 2024-05-28 20:52:31.858799 semantic_kernel-1.0.3/semantic_kernel/utils/naming.py
+-rw-r--r--   0        0        0      269 2024-05-22 16:18:31.575428 semantic_kernel-1.0.3/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     4516 1970-01-01 00:00:00.000000 semantic_kernel-1.0.3/PKG-INFO
```

### Comparing `semantic_kernel-1.0.2/pip/README.md` & `semantic_kernel-1.0.3/pip/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/pyproject.toml` & `semantic_kernel-1.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantic-kernel"
-version = "1.0.2"
+version = "1.0.3"
 description = "Semantic Kernel Python SDK"
 authors = ["Microsoft <SK-Support@microsoft.com>"]
 readme = "pip/README.md"
 packages = [{include = "semantic_kernel"}]
 
 [tool.poetry.dependencies]
 python = "^3.10,<3.13"
@@ -53,23 +53,22 @@
 azure-identity = { version = "^1.13.0", optional = true}
 azure-cosmos = { version = "^4.7.0", optional = true}
 usearch = { version = "^2.9", optional = true}
 pyarrow = { version = ">=12.0.1,<16.0.0", optional = true}
 
 # Groups are for development only (installed through Poetry)
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^3.5"
-black = "^24.2.0"
-ruff = ">=0.3.2,<0.5.0"
-ipykernel = "^6.29.3"
-pytest = "^8.1.1"
-pytest-asyncio = "^0.23.6"
+pre-commit = ">=3.7.1"
+ruff = ">=0.4.5"
+ipykernel = "^6.29.4"
+pytest = "^8.2.1"
+pytest-asyncio = "^0.23.7"
 snoop = "^0.4.3"
 pytest-cov = ">=5.0.0"
-mypy = ">=1.9.0"
+mypy = ">=1.10.0"
 types-PyYAML = "^6.0.12.20240311"
 
 [tool.poetry.group.unit-tests]
 optional = true
 
 [tool.poetry.group.unit-tests.dependencies]
 google-generativeai = { version = ">=0.1,<0.4" }
@@ -118,16 +117,33 @@
 redis = ["redis"]
 azure = ["azure-search-documents", "azure-core", "azure-identity", "azure-cosmos", "msgraph-sdk"]
 usearch = ["usearch", "pyarrow"]
 notebooks = ["ipykernel"]
 all = ["google-generativeai", "grpcio-status", "transformers", "sentence-transformers", "torch", "qdrant-client", "chromadb", "pymilvus", "milvus", "weaviate-client", "pinecone-client", "psycopg", "redis", "azure-search-documents", "azure-core", "azure-identity", "azure-cosmos", "usearch", "pyarrow", "ipykernel"]
 
 [tool.ruff]
-lint.select = ["E", "F", "I"]
 line-length = 120
+target-version = "py310"
+include = ["*.py", "*.pyi", "**/pyproject.toml", "*.ipynb"]
 
-[tool.black]
-line-length = 120
+[tool.ruff.lint]
+select = ["D", "E", "F", "I"]
+ignore = ["D100", "D101", "D104"]
+
+[tool.ruff.lint.pydocstyle]
+convention = "google"
+
+[tool.ruff.lint.per-file-ignores]
+# Ignore all directories named `tests`.
+"tests/**" = ["D"]
+"samples/**" = ["D"]
+# Ignore all files that end in `_test.py`.
+"*_test.py" = ["D"]
+
+[tool.bandit]
+targets = ["python/semantic_kernel"]
+exclude_dirs = ["python/tests"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/chat_completion_client_base.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/chat_completion_client_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,64 +17,64 @@
     @abstractmethod
     async def get_chat_message_contents(
         self,
         chat_history: "ChatHistory",
         settings: "PromptExecutionSettings",
         **kwargs: Any,
     ) -> list["ChatMessageContent"]:
-        """
-        This is the method that is called from the kernel to get a response from a chat-optimized LLM.
+        """This is the method that is called from the kernel to get a response from a chat-optimized LLM.
 
-        Arguments:
-            chat_history {ChatHistory} -- A list of chats in a chat_history object, that can be
+        Args:
+            chat_history (ChatHistory): A list of chats in a chat_history object, that can be
                 rendered into messages from system, user, assistant and tools.
-            settings {PromptExecutionSettings} -- Settings for the request.
-            kwargs {Dict[str, Any]} -- The optional arguments.
+            settings (PromptExecutionSettings): Settings for the request.
+            kwargs (Dict[str, Any]): The optional arguments.
 
         Returns:
-            Union[str, List[str]] -- A string or list of strings representing the response(s) from the LLM.
+            Union[str, List[str]]: A string or list of strings representing the response(s) from the LLM.
         """
         pass
 
     @abstractmethod
     def get_streaming_chat_message_contents(
         self,
         chat_history: "ChatHistory",
         settings: "PromptExecutionSettings",
         **kwargs: Any,
     ) -> AsyncGenerator[list["StreamingChatMessageContent"], Any]:
-        """
-        This is the method that is called from the kernel to get a stream response from a chat-optimized LLM.
+        """This is the method that is called from the kernel to get a stream response from a chat-optimized LLM.
 
-        Arguments:
-            chat_history {ChatHistory} -- A list of chat chat_history, that can be rendered into a
+        Args:
+            chat_history (ChatHistory): A list of chat chat_history, that can be rendered into a
                 set of chat_history, from system, user, assistant and function.
-            settings {PromptExecutionSettings} -- Settings for the request.
-            kwargs {Dict[str, Any]} -- The optional arguments.
+            settings (PromptExecutionSettings): Settings for the request.
+            kwargs (Dict[str, Any]): The optional arguments.
 
 
         Yields:
             A stream representing the response(s) from the LLM.
         """
         ...
 
     def _prepare_chat_history_for_request(
         self,
         chat_history: "ChatHistory",
         role_key: str = "role",
         content_key: str = "content",
     ) -> list[dict[str, str | None]]:
-        """
-        Prepare the chat history for a request, allowing customization of the key names for role/author,
-        and optionally overriding the role.
+        """Prepare the chat history for a request.
+
+        Allowing customization of the key names for role/author, and optionally overriding the role.
 
         ChatRole.TOOL messages need to be formatted different than system/user/assistant messages:
             They require a "tool_call_id" and (function) "name" key, and the "metadata" key should
             be removed. The "encoding" key should also be removed.
 
-        Arguments:
-            chat_history {ChatHistory} -- The chat history to prepare.
+        Args:
+            chat_history (ChatHistory): The chat history to prepare.
+            role_key (str): The key name for the role/author.
+            content_key (str): The key name for the content/message.
 
         Returns:
-            List[Dict[str, Optional[str]]] -- The prepared chat history.
+            List[Dict[str, Optional[str]]]: The prepared chat history.
         """
         return [message.to_dict(role_key=role_key, content_key=content_key) for message in chat_history.messages]
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/function_call_behavior.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/function_call_behavior.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         Using the base ToolCallBehavior means that you manually have to set tool_choice and tools.
 
         For different behaviors, use the subclasses of ToolCallBehavior:
             KernelFunctions (all functions in the Kernel)
             EnabledFunctions (filtered set of functions from the Kernel)
             RequiredFunction (a single function)
 
-        By default the update_settings_callback is called with FunctionCallConfiguration,
+        By default, the update_settings_callback is called with FunctionCallConfiguration,
         which contains a list of available functions or a list of required functions, it also
         takes the PromptExecutionSettings object.
 
         It should update the prompt execution settings with the available functions or required functions.
 
         Alternatively you can override this class and add your own logic in the configure method.
         """
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/google_palm/__init__.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/google_palm/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,12 +36,13 @@
     messages: MessagesOptions | None = None
     examples: ExampleOptions | None = None
     context: str | None = None
     token_selection_biases: dict[int, int] | None = None
 
     @model_validator(mode="after")
     def validate_input(self):
+        """Validate input."""
         if self.prompt is not None:
             if self.messages or self.context or self.examples:
                 raise ServiceInvalidExecutionSettingsError(
                     "Prompt cannot be used without messages, context or examples"
                 )
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,24 +34,23 @@
     def __init__(
         self,
         ai_model_id: str,
         api_key: str | None = None,
         message_history: ChatHistory | None = None,
         env_file_path: str | None = None,
     ):
-        """
-        Initializes a new instance of the GooglePalmChatCompletion class.
+        """Initializes a new instance of the GooglePalmChatCompletion class.
 
-        Arguments:
-            ai_model_id {str} -- GooglePalm model name, see
+        Args:
+            ai_model_id (str): GooglePalm model name, see
                 https://developers.generativeai.google/models/language
-            api_key {str | None} -- The optional API key to use. If not provided, will be read from either
+            api_key (str | None): The optional API key to use. If not provided, will be read from either
                 the env vars or the .env settings file
-            message_history {ChatHistory | None} -- The message history to use for context. (Optional)
-            env_file_path {str | None} -- Use the environment settings file as a fallback to
+            message_history (ChatHistory | None): The message history to use for context. (Optional)
+            env_file_path (str | None): Use the environment settings file as a fallback to
                 environment variables. (Optional)
         """
         google_palm_settings = None
         try:
             google_palm_settings = GooglePalmSettings.create(env_file_path=env_file_path)
         except ValidationError as e:
             logger.warning(f"Error loading Google Palm pydantic settings: {e}")
@@ -73,25 +72,24 @@
 
     async def get_chat_message_contents(
         self,
         chat_history: ChatHistory,
         settings: GooglePalmPromptExecutionSettings,
         **kwargs: Any,
     ) -> list[ChatMessageContent]:
-        """
-        This is the method that is called from the kernel to get a response from a chat-optimized LLM.
+        """This is the method that is called from the kernel to get a response from a chat-optimized LLM.
 
-        Arguments:
-            chat_history {List[ChatMessage]} -- A list of chat messages, that can be rendered into a
+        Args:
+            chat_history (List[ChatMessage]): A list of chat messages, that can be rendered into a
                 set of messages, from system, user, assistant and function.
-            settings {GooglePalmPromptExecutionSettings} -- Settings for the request.
-            kwargs {Dict[str, Any]} -- The optional arguments.
+            settings (GooglePalmPromptExecutionSettings): Settings for the request.
+            kwargs (Dict[str, Any]): The optional arguments.
 
         Returns:
-            List[ChatMessageContent] -- A list of ChatMessageContent objects representing the response(s) from the LLM.
+            List[ChatMessageContent]: A list of ChatMessageContent objects representing the response(s) from the LLM.
         """
         settings.messages = self._prepare_chat_history_for_request(chat_history, role_key="author")
         if not settings.ai_model_id:
             settings.ai_model_id = self.ai_model_id
         response = await self._send_chat_request(settings)
         return [
             self._create_chat_message_content(response, candidate, index)
@@ -99,19 +97,21 @@
         ]
 
     def _create_chat_message_content(
         self, response: ChatResponse, candidate: MessageDict, index: int
     ) -> ChatMessageContent:
         """Create a chat message content object from a response.
 
-        Arguments:
-            response {ChatResponse} -- The response to create the content from.
+        Args:
+            response (ChatResponse): The response to create the content from.
+            candidate (MessageDict): The candidate message to create the content from.
+            index (int): The index of the candidate message.
 
         Returns:
-            ChatMessageContent -- The created chat message content.
+            ChatMessageContent: The created chat message content.
         """
         metadata = {
             "citation_metadata": candidate.get("citation_metadata"),
             "filters": response.filters,
             "choice_index": index,
         }
         return ChatMessageContent(
@@ -124,95 +124,90 @@
 
     async def get_streaming_chat_message_contents(
         self,
         messages: list[tuple[str, str]],
         settings: GooglePalmPromptExecutionSettings,
         **kwargs: Any,
     ):
+        """Return a streaming chat message.
+
+        Raises:
+            NotImplementedError: Google Palm API does not currently support streaming
+        """
         raise NotImplementedError("Google Palm API does not currently support streaming")
 
     async def get_text_contents(
         self,
         prompt: str,
         settings: GooglePalmPromptExecutionSettings,
     ) -> list[TextContent]:
-        """
-        This is the method that is called from the kernel to get a response from a text-optimized LLM.
+        """This is the method that is called from the kernel to get a response from a text-optimized LLM.
 
-        Arguments:
-            prompt {str} -- The prompt to send to the LLM.
-            settings {GooglePalmPromptExecutionSettings} -- Settings for the request.
+        Args:
+            prompt (str): The prompt to send to the LLM.
+            settings (GooglePalmPromptExecutionSettings): Settings for the request.
 
         Returns:
-            List[TextContent] -- A list of TextContent objects representing the response(s) from the LLM.
+            List[TextContent]: A list of TextContent objects representing the response(s) from the LLM.
         """
         settings.messages = [{"author": "user", "content": prompt}]
         if not settings.ai_model_id:
             settings.ai_model_id = self.ai_model_id
         response = await self._send_chat_request(settings)
 
         return [self._create_text_content(response, candidate) for candidate in response.candidates]
 
     def _create_text_content(self, response: ChatResponse, candidate: MessageDict) -> TextContent:
         """Create a text content object from a response.
 
-        Arguments:
-            response {ChatResponse} -- The response to create the content from.
+        Args:
+            response (ChatResponse): The response to create the content from.
+            candidate (MessageDict): The candidate message to create the content from.
 
         Returns:
-            TextContent -- The created text content.
+            TextContent: The created text content.
         """
         metadata = {"citation_metadata": candidate.get("citation_metadata"), "filters": response.filters}
         return TextContent(
             inner_content=response,
             ai_model_id=self.ai_model_id,
             metadata=metadata,
             text=candidate.get("content"),
         )
 
     async def get_streaming_text_contents(
         self,
         prompt: str,
         settings: GooglePalmPromptExecutionSettings,
     ):
+        """Return a streaming text content.
+
+        Raises:
+            NotImplementedError: Google Palm API does not currently support streaming
+        """
         raise NotImplementedError("Google Palm API does not currently support streaming")
 
     async def _send_chat_request(
         self,
         settings: GooglePalmPromptExecutionSettings,
-    ):
-        """
-        Completes the given user message. If len(messages) > 1, and a
+    ) -> Any:
+        """Completes the given user message.
+
+        If len(messages) > 1, and a
         conversation has not been initiated yet, it is assumed that chat history
         is needed for context. All messages preceding the last message will be
         utilized for context. This also enables Google PaLM to utilize memory
         and plugins, which should be stored in the messages parameter as system
         messages.
 
-        Arguments:
-            messages {str} -- The message (from a user) to respond to.
-            settings {GooglePalmPromptExecutionSettings} -- The request settings.
-            context {str} -- Text that should be provided to the model first,
-            to ground the response. If a system message is provided, it will be
-            used as context.
-            examples {ExamplesOptions} -- 	Examples of what the model should
-            generate. This includes both the user input and the response that
-            the model should emulate. These examples are treated identically to
-            conversation messages except that they take precedence over the
-            history in messages: If the total input size exceeds the model's
-            input_token_limit the input will be truncated. Items will be dropped
-            from messages before examples
-            See: https://developers.generativeai.google/api/python/google/generativeai/types/ExampleOptions
-            prompt {MessagePromptOptions} -- 	You may pass a
-            types.MessagePromptOptions instead of a setting context/examples/messages,
-            but not both.
-            See: https://developers.generativeai.google/api/python/google/generativeai/types/MessagePromptOptions
+        Args:
+            settings (GooglePalmPromptExecutionSettings): The request settings.
 
         Returns:
-            str -- The completed text.
+            The completion.
         """
         if settings is None:
             raise ValueError("The request settings cannot be `None`")
 
         if settings.messages[-1]["author"] != "user":
             raise ServiceInvalidRequestError("The last message must be from the user")
         try:
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,23 +18,22 @@
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class GooglePalmTextCompletion(TextCompletionClientBase):
     api_key: Annotated[str, StringConstraints(strip_whitespace=True, min_length=1)]
 
     def __init__(self, ai_model_id: str, api_key: str | None = None, env_file_path: str | None = None):
-        """
-        Initializes a new instance of the GooglePalmTextCompletion class.
+        """Initializes a new instance of the GooglePalmTextCompletion class.
 
-        Arguments:
-            ai_model_id {str} -- GooglePalm model name, see
+        Args:
+            ai_model_id (str): GooglePalm model name, see
                 https://developers.generativeai.google/models/language
-            api_key {str | None} -- The optional API key to use. If not provided, will be
+            api_key (str | None): The optional API key to use. If not provided, will be
                 read from either the env vars or the .env settings file.
-            env_file_path {str | None} -- Use the environment settings file as a
+            env_file_path (str | None): Use the environment settings file as a
                 fallback to environment variables. (Optional)
         """
         try:
             google_palm_settings = GooglePalmSettings.create(env_file_path=env_file_path)
         except ValidationError as e:
             logger.warning(f"Error loading Google Palm pydantic settings: {e}")
 
@@ -48,23 +47,22 @@
         )
 
         super().__init__(ai_model_id=ai_model_id, api_key=api_key)
 
     async def get_text_contents(
         self, prompt: str, settings: GooglePalmTextPromptExecutionSettings
     ) -> list[TextContent]:
-        """
-        This is the method that is called from the kernel to get a response from a text-optimized LLM.
+        """This is the method that is called from the kernel to get a response from a text-optimized LLM.
 
-        Arguments:
-            prompt {str} -- The prompt to send to the LLM.
-            settings {GooglePalmTextPromptExecutionSettings} -- Settings for the request.
+        Args:
+            prompt (str): The prompt to send to the LLM.
+            settings (GooglePalmTextPromptExecutionSettings): Settings for the request.
 
         Returns:
-            List[TextContent] -- A list of TextContent objects representing the response(s) from the LLM.
+            List[TextContent]: A list of TextContent objects representing the response(s) from the LLM.
         """
         settings.prompt = prompt
         if not settings.ai_model_id:
             settings.ai_model_id = self.ai_model_id
         try:
             palm.configure(api_key=self.api_key)
         except Exception as ex:
@@ -96,12 +94,18 @@
         )
 
     async def get_streaming_text_contents(
         self,
         prompt: str,
         settings: GooglePalmTextPromptExecutionSettings,
     ):
+        """Get streaming text contents from the Google Palm API, unsupported.
+
+        Raises:
+            NotImplementedError: Google Palm API does not currently support streaming.
+
+        """
         raise NotImplementedError("Google Palm API does not currently support streaming")
 
     def get_prompt_execution_settings_class(self) -> "PromptExecutionSettings":
         """Create a request settings object."""
         return GooglePalmTextPromptExecutionSettings
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,23 +16,22 @@
 
 
 @experimental_class
 class GooglePalmTextEmbedding(EmbeddingGeneratorBase):
     api_key: Annotated[str, StringConstraints(strip_whitespace=True, min_length=1)]
 
     def __init__(self, ai_model_id: str, api_key: str | None = None, env_file_path: str | None = None) -> None:
-        """
-        Initializes a new instance of the GooglePalmTextEmbedding class.
+        """Initializes a new instance of the GooglePalmTextEmbedding class.
 
-        Arguments:
-            ai_model_id {str} -- GooglePalm model name, see
+        Args:
+            ai_model_id (str): GooglePalm model name, see
                 https://developers.generativeai.google/models/language
-            api_key {str | None} -- The optional API key to use. If not provided, will be
+            api_key (str | None): The optional API key to use. If not provided, will be
                 read from either the env vars or the .env settings file.
-            env_file_path {str | None} -- Use the environment settings file
+            env_file_path (str | None): Use the environment settings file
                 as a fallback to environment variables. (Optional)
         """
         try:
             google_palm_settings = GooglePalmSettings.create(env_file_path=env_file_path)
         except ValidationError as e:
             logger.error(f"Error loading Google Palm pydantic settings: {e}")
 
@@ -45,23 +44,15 @@
             google_palm_settings.embedding_model_id
             if google_palm_settings and google_palm_settings.embedding_model_id
             else None
         )
         super().__init__(ai_model_id=ai_model_id, api_key=api_key)
 
     async def generate_embeddings(self, texts: list[str], **kwargs: Any) -> ndarray:
-        """
-        Generates embeddings for a list of texts.
-
-        Arguments:
-            texts {List[str]} -- Texts to generate embeddings for.
-
-        Returns:
-            ndarray -- Embeddings for the texts.
-        """
+        """Generates embeddings for the given list of texts."""
         try:
             palm.configure(api_key=self.api_key)
         except Exception as ex:
             raise ServiceInvalidAuthError(
                 "Google PaLM service failed to configure. Invalid API key provided.",
                 ex,
             ) from ex
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/google_palm/settings/google_palm_settings.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/google_palm/settings/google_palm_settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from pydantic import SecretStr
 from pydantic_settings import BaseSettings
 
 
 class GooglePalmSettings(BaseSettings):
-    """Google Palm model settings
+    """Google Palm model settings.
 
     The settings are first loaded from environment variables with the prefix 'GOOGLE_PALM_'. If the
     environment variables are not found, the settings can be loaded from a .env file with the
     encoding 'utf-8'. If the settings are not found in the .env file, the settings are ignored;
     however, validation will fail alerting that the settings are missing.
 
     Optional settings for prefix 'GOOGLE_PALM_' are:
@@ -27,20 +27,23 @@
     env_file_path: str | None = None
     api_key: SecretStr | None = None
     chat_model_id: str | None = None
     text_model_id: str | None = None
     embedding_model_id: str | None = None
 
     class Config:
+        """Pydantic configuration settings."""
+
         env_prefix = "GOOGLE_PALM_"
         env_file = None
         env_file_encoding = "utf-8"
         extra = "ignore"
         case_sensitive = False
 
     @classmethod
     def create(cls, **kwargs):
+        """Create the settings object."""
         if "env_file_path" in kwargs and kwargs["env_file_path"]:
             cls.Config.env_file = kwargs["env_file_path"]
         else:
             cls.Config.env_file = None
         return cls(**kwargs)
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/hugging_face/__init__.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/hugging_face/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,24 +12,26 @@
     stop_sequences: Any = None
     pad_token_id: int = 50256
     eos_token_id: int = 50256
     temperature: float = 1.0
     top_p: float = 1.0
 
     def get_generation_config(self) -> GenerationConfig:
+        """Get the generation config."""
         return GenerationConfig(
             **self.model_dump(
                 include={"max_new_tokens", "pad_token_id", "eos_token_id", "temperature", "top_p"},
                 exclude_unset=False,
                 exclude_none=True,
                 by_alias=True,
             )
         )
 
     def prepare_settings_dict(self, **kwargs) -> dict[str, Any]:
+        """Prepare the settings dictionary."""
         gen_config = self.get_generation_config()
         settings = {
             "generation_config": gen_config,
             "num_return_sequences": self.num_return_sequences,
             "do_sample": self.do_sample,
         }
         settings.update(kwargs)
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,34 +30,33 @@
         ai_model_id: str,
         task: str | None = "text2text-generation",
         device: int | None = -1,
         service_id: str | None = None,
         model_kwargs: dict[str, Any] | None = None,
         pipeline_kwargs: dict[str, Any] | None = None,
     ) -> None:
-        """
-        Initializes a new instance of the HuggingFaceTextCompletion class.
+        """Initializes a new instance of the HuggingFaceTextCompletion class.
 
-        Arguments:
-            ai_model_id {str} -- Hugging Face model card string, see
+        Args:
+            ai_model_id (str): Hugging Face model card string, see
                 https://huggingface.co/models
-            device {Optional[int]} -- Device to run the model on, defaults to CPU, 0+ for GPU,
+            device (Optional[int]): Device to run the model on, defaults to CPU, 0+ for GPU,
                                    -- None if using device_map instead. (If both device and device_map
                                       are specified, device overrides device_map. If unintended,
                                       it can lead to unexpected behavior.)
-            service_id {Optional[str]} -- Service ID for the AI service.
-            task {Optional[str]} -- Model completion task type, options are:
+            service_id (Optional[str]): Service ID for the AI service.
+            task (Optional[str]): Model completion task type, options are:
                 - summarization: takes a long text and returns a shorter summary.
                 - text-generation: takes incomplete text and returns a set of completion candidates.
                 - text2text-generation (default): takes an input prompt and returns a completion.
                 text2text-generation is the default as it behaves more like GPT-3+.
-            log  -- Logger instance. (Deprecated)
-            model_kwargs {Optional[Dict[str, Any]]} -- Additional dictionary of keyword arguments
+            log : Logger instance. (Deprecated)
+            model_kwargs (Optional[Dict[str, Any]]): Additional dictionary of keyword arguments
                 passed along to the model's `from_pretrained(..., **model_kwargs)` function.
-            pipeline_kwargs {Optional[Dict[str, Any]]} -- Additional keyword arguments passed along
+            pipeline_kwargs (Optional[Dict[str, Any]]): Additional keyword arguments passed along
                 to the specific pipeline init (see the documentation for the corresponding pipeline class
                 for possible values).
 
         Note that this model will be downloaded from the Hugging Face model hub.
         """
         generator = pipeline(
             task=task,
@@ -75,23 +74,22 @@
         )
 
     async def get_text_contents(
         self,
         prompt: str,
         settings: HuggingFacePromptExecutionSettings,
     ) -> list[TextContent]:
-        """
-        This is the method that is called from the kernel to get a response from a text-optimized LLM.
+        """This is the method that is called from the kernel to get a response from a text-optimized LLM.
 
-        Arguments:
-            prompt {str} -- The prompt to send to the LLM.
-            settings {HuggingFacePromptExecutionSettings} -- Settings for the request.
+        Args:
+            prompt (str): The prompt to send to the LLM.
+            settings (HuggingFacePromptExecutionSettings): Settings for the request.
 
         Returns:
-            List[TextContent] -- A list of TextContent objects representing the response(s) from the LLM.
+            List[TextContent]: A list of TextContent objects representing the response(s) from the LLM.
         """
         try:
             results = self.generator(prompt, **settings.prepare_settings_dict())
         except Exception as e:
             raise ServiceResponseException("Hugging Face completion failed", e) from e
         if isinstance(results, list):
             return [self._create_text_content(results, result) for result in results]
@@ -105,24 +103,24 @@
         )
 
     async def get_streaming_text_contents(
         self,
         prompt: str,
         settings: HuggingFacePromptExecutionSettings,
     ) -> AsyncGenerator[list[StreamingTextContent], Any]:
-        """
-        Streams a text completion using a Hugging Face model.
+        """Streams a text completion using a Hugging Face model.
+
         Note that this method does not support multiple responses.
 
-        Arguments:
-            prompt {str} -- Prompt to complete.
-            settings {HuggingFacePromptExecutionSettings} -- Request settings.
+        Args:
+            prompt (str): Prompt to complete.
+            settings (HuggingFacePromptExecutionSettings): Request settings.
 
         Yields:
-            List[StreamingTextContent] -- List of StreamingTextContent objects.
+            List[StreamingTextContent]: List of StreamingTextContent objects.
         """
         if settings.num_return_sequences > 1:
             raise ServiceInvalidExecutionSettingsError(
                 "HuggingFace TextIteratorStreamer does not stream multiple responses in a parseable format. \
                     If you need multiple responses, please use the complete method.",
             )
         try:
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
+import sys
 from typing import Any
 
+if sys.version_info >= (3, 12):
+    from typing import override
+else:
+    from typing_extensions import override
+
 import sentence_transformers
 import torch
 from numpy import array, ndarray
 
 from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import EmbeddingGeneratorBase
 from semantic_kernel.exceptions import ServiceResponseException
 from semantic_kernel.utils.experimental_decorator import experimental_class
@@ -21,42 +27,33 @@
 
     def __init__(
         self,
         ai_model_id: str,
         device: int | None = -1,
         service_id: str | None = None,
     ) -> None:
-        """
-        Initializes a new instance of the HuggingFaceTextEmbedding class.
+        """Initializes a new instance of the HuggingFaceTextEmbedding class.
 
-        Arguments:
-            ai_model_id {str} -- Hugging Face model card string, see
+        Args:
+            ai_model_id (str): Hugging Face model card string, see
                 https://huggingface.co/sentence-transformers
-            device {Optional[int]} -- Device to run the model on, -1 for CPU, 0+ for GPU.
-            log  -- The logger instance to use. (Optional) (Deprecated)
+            device (Optional[int]): Device to run the model on, -1 for CPU, 0+ for GPU.
+            service_id (Optional[str]): Service ID for the model.
 
         Note that this model will be downloaded from the Hugging Face model hub.
         """
         resolved_device = f"cuda:{device}" if device >= 0 and torch.cuda.is_available() else "cpu"
         super().__init__(
             ai_model_id=ai_model_id,
             service_id=service_id,
             device=resolved_device,
             generator=sentence_transformers.SentenceTransformer(model_name_or_path=ai_model_id, device=resolved_device),
         )
 
+    @override
     async def generate_embeddings(self, texts: list[str], **kwargs: Any) -> ndarray:
-        """
-        Generates embeddings for a list of texts.
-
-        Arguments:
-            texts {List[str]} -- Texts to generate embeddings for.
-
-        Returns:
-            ndarray -- Embeddings for the texts.
-        """
         try:
             logger.info(f"Generating embeddings for {len(texts)} texts")
             embeddings = self.generator.encode(texts, **kwargs)
             return array(embeddings)
         except Exception as e:
             raise ServiceResponseException("Hugging Face embeddings failed", e) from e
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/ollama/__init__.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/ollama/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,45 +18,43 @@
 from semantic_kernel.contents.streaming_text_content import StreamingTextContent
 from semantic_kernel.contents.text_content import TextContent
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class OllamaChatCompletion(TextCompletionClientBase, ChatCompletionClientBase):
-    """
-    Initializes a new instance of the OllamaChatCompletion class.
+    """Initializes a new instance of the OllamaChatCompletion class.
 
     Make sure to have the ollama service running either locally or remotely.
 
-    Arguments:
-        ai_model_id {str} -- Ollama model name, see https://ollama.ai/library
-        url {Optional[Union[str, HttpUrl]]} -- URL of the Ollama server, defaults to http://localhost:11434/api/chat
-        session {Optional[aiohttp.ClientSession]} -- Optional client session to use for requests.
+    Args:
+        ai_model_id (str): Ollama model name, see https://ollama.ai/library
+        url (Optional[Union[str, HttpUrl]]): URL of the Ollama server, defaults to http://localhost:11434/api/chat
+        session (Optional[aiohttp.ClientSession]): Optional client session to use for requests.
     """
 
     url: HttpUrl = "http://localhost:11434/api/chat"
     session: aiohttp.ClientSession | None = None
 
     async def get_chat_message_contents(
         self,
         chat_history: ChatHistory,
         settings: OllamaChatPromptExecutionSettings,
         **kwargs: Any,
     ) -> list[ChatMessageContent]:
-        """
-        This is the method that is called from the kernel to get a response from a chat-optimized LLM.
+        """This is the method that is called from the kernel to get a response from a chat-optimized LLM.
 
-        Arguments:
-            chat_history {ChatHistory} -- A chat history that contains a list of chat messages,
+        Args:
+            chat_history (ChatHistory): A chat history that contains a list of chat messages,
                 that can be rendered into a set of messages, from system, user, assistant and function.
-            settings {PromptExecutionSettings} -- Settings for the request.
-            kwargs {Dict[str, Any]} -- The optional arguments.
+            settings (PromptExecutionSettings): Settings for the request.
+            kwargs (Dict[str, Any]): The optional arguments.
 
         Returns:
-            List[ChatMessageContent] -- A list of ChatMessageContent objects representing the response(s) from the LLM.
+            List[ChatMessageContent]: A list of ChatMessageContent objects representing the response(s) from the LLM.
         """
         if not settings.ai_model_id:
             settings.ai_model_id = self.ai_model_id
         settings.messages = self._prepare_chat_history_for_request(chat_history)
         settings.stream = False
         async with AsyncSession(self.session) as session:
             async with session.post(str(self.url), json=settings.prepare_settings_dict()) as response:
@@ -73,26 +71,26 @@
 
     async def get_streaming_chat_message_contents(
         self,
         chat_history: ChatHistory,
         settings: OllamaChatPromptExecutionSettings,
         **kwargs: Any,
     ) -> AsyncGenerator[list[StreamingChatMessageContent], Any]:
-        """
-        Streams a text completion using a Ollama model.
+        """Streams a text completion using an Ollama model.
+
         Note that this method does not support multiple responses.
 
-        Arguments:
-            chat_history {ChatHistory} -- A chat history that contains a list of chat messages,
+        Args:
+            chat_history (ChatHistory): A chat history that contains a list of chat messages,
                 that can be rendered into a set of messages, from system, user, assistant and function.
-            settings {OllamaChatPromptExecutionSettings} -- Request settings.
-            kwargs {Dict[str, Any]} -- The optional arguments.
+            settings (OllamaChatPromptExecutionSettings): Request settings.
+            kwargs (Dict[str, Any]): The optional arguments.
 
         Yields:
-            List[StreamingChatMessageContent] -- Stream of StreamingChatMessageContent objects.
+            List[StreamingChatMessageContent]: Stream of StreamingChatMessageContent objects.
         """
         if not settings.ai_model_id:
             settings.ai_model_id = self.ai_model_id
         settings.messages = self._prepare_chat_history_for_request(chat_history)
         settings.stream = True
         async with AsyncSession(self.session) as session:
             async with session.post(str(self.url), json=settings.prepare_settings_dict()) as response:
@@ -114,23 +112,22 @@
                         break
 
     async def get_text_contents(
         self,
         prompt: str,
         settings: OllamaChatPromptExecutionSettings,
     ) -> list[TextContent]:
-        """
-        This is the method that is called from the kernel to get a response from a text-optimized LLM.
+        """This is the method that is called from the kernel to get a response from a text-optimized LLM.
 
-        Arguments:
-            chat_history {ChatHistory} -- A chat history that contains the prompt to complete.
-            settings {OllamaChatPromptExecutionSettings} -- Settings for the request.
+        Args:
+            prompt (str): A prompt to complete
+            settings (OllamaChatPromptExecutionSettings): Settings for the request.
 
         Returns:
-            List["TextContent"] -- The completion result(s).
+            List["TextContent"]: The completion result(s).
         """
         if not settings.ai_model_id:
             settings.ai_model_id = self.ai_model_id
         settings.messages = [{"role": "user", "content": prompt}]
         settings.stream = False
         async with AsyncSession(self.session) as session:
             async with session.post(str(self.url), json=settings.prepare_settings_dict()) as response:
@@ -145,26 +142,25 @@
                 ]
 
     async def get_streaming_text_contents(
         self,
         prompt: str,
         settings: OllamaChatPromptExecutionSettings,
     ) -> AsyncGenerator[list[StreamingTextContent], Any]:
-        """
-        Streams a text completion using a Ollama model.
+        """Streams a text completion using an Ollama model.
+
         Note that this method does not support multiple responses.
 
-        Arguments:
-            prompt {str} -- A chat history that contains the prompt to complete.
-            settings {OllamaChatPromptExecutionSettings} -- Request settings.
+        Args:
+            prompt (str): A chat history that contains the prompt to complete.
+            settings (OllamaChatPromptExecutionSettings): Request settings.
 
         Yields:
-            List["StreamingTextContent"] -- The result stream made up of StreamingTextContent objects.
+            List["StreamingTextContent"]: The result stream made up of StreamingTextContent objects.
         """
-
         if not settings.ai_model_id:
             settings.ai_model_id = self.ai_model_id
         settings.messages = [{"role": "user", "content": prompt}]
         settings.stream = True
         async with AsyncSession(self.session) as session:
             async with session.post(str(self.url), json=settings.prepare_settings_dict()) as response:
                 response.raise_for_status()
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,41 +14,39 @@
 from semantic_kernel.contents.streaming_text_content import StreamingTextContent
 from semantic_kernel.contents.text_content import TextContent
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class OllamaTextCompletion(TextCompletionClientBase):
-    """
-    Initializes a new instance of the OllamaTextCompletion class.
+    """Initializes a new instance of the OllamaTextCompletion class.
 
     Make sure to have the ollama service running either locally or remotely.
 
-    Arguments:
-        ai_model_id {str} -- Ollama model name, see https://ollama.ai/library
-        url {Optional[Union[str, HttpUrl]]} -- URL of the Ollama server, defaults to http://localhost:11434/api/generate
+    Args:
+        ai_model_id (str): Ollama model name, see https://ollama.ai/library
+        url (Optional[Union[str, HttpUrl]]): URL of the Ollama server, defaults to http://localhost:11434/api/generate
     """
 
     url: HttpUrl = "http://localhost:11434/api/generate"
     session: aiohttp.ClientSession | None = None
 
     async def get_text_contents(
         self,
         prompt: str,
         settings: OllamaTextPromptExecutionSettings,
     ) -> list[TextContent]:
-        """
-        This is the method that is called from the kernel to get a response from a text-optimized LLM.
+        """This is the method that is called from the kernel to get a response from a text-optimized LLM.
 
-        Arguments:
-            prompt {str} -- The prompt to send to the LLM.
-            settings {OllamaTextPromptExecutionSettings} -- Settings for the request.
+        Args:
+            prompt (str): The prompt to send to the LLM.
+            settings (OllamaTextPromptExecutionSettings): Settings for the request.
 
         Returns:
-            List[TextContent] -- A list of TextContent objects representing the response(s) from the LLM.
+            List[TextContent]: A list of TextContent objects representing the response(s) from the LLM.
         """
         if not settings.ai_model_id:
             settings.ai_model_id = self.ai_model_id
         settings.prompt = prompt
         settings.stream = False
         async with AsyncSession(self.session) as session:
             async with session.post(self.url, json=settings.prepare_settings_dict()) as response:
@@ -58,25 +56,25 @@
                 return [TextContent(inner_content=inner_content, ai_model_id=self.ai_model_id, text=text)]
 
     async def get_streaming_text_contents(
         self,
         prompt: str,
         settings: OllamaTextPromptExecutionSettings,
     ) -> AsyncGenerator[list[StreamingTextContent], Any]:
-        """
-        Streams a text completion using a Ollama model.
+        """Streams a text completion using an Ollama model.
+
         Note that this method does not support multiple responses,
         but the result will be a list anyway.
 
-        Arguments:
-            prompt {str} -- Prompt to complete.
-            settings {OllamaTextPromptExecutionSettings} -- Request settings.
+        Args:
+            prompt (str): Prompt to complete.
+            settings (OllamaTextPromptExecutionSettings): Request settings.
 
         Yields:
-            List[StreamingTextContent] -- Completion result.
+            List[StreamingTextContent]: Completion result.
         """
         if not settings.ai_model_id:
             settings.ai_model_id = self.ai_model_id
         settings.prompt = prompt
         settings.stream = True
         async with AsyncSession(self.session) as session:
             async with session.post(self.url, json=settings.prepare_settings_dict()) as response:
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
+import sys
 from typing import Any
 
+if sys.version_info >= (3, 12):
+    from typing import override
+else:
+    from typing_extensions import override
+
 import aiohttp
 from numpy import array, ndarray
 from pydantic import HttpUrl
 
 from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import EmbeddingGeneratorBase
 from semantic_kernel.connectors.ai.ollama.utils import AsyncSession
 from semantic_kernel.utils.experimental_decorator import experimental_class
@@ -16,33 +22,25 @@
 
 @experimental_class
 class OllamaTextEmbedding(EmbeddingGeneratorBase):
     """Ollama embeddings client.
 
     Make sure to have the ollama service running either locally or remotely.
 
-    Arguments:
-        ai_model_id {str} -- Ollama model name, see https://ollama.ai/library
-        url {Optional[Union[str, HttpUrl]]} -- URL of the Ollama server, defaults to http://localhost:11434/api/embeddings
-        session {Optional[aiohttp.ClientSession]} -- Optional client session to use for requests.
+    Args:
+        ai_model_id (str): Ollama model name, see https://ollama.ai/library
+        url (Optional[Union[str, HttpUrl]]): URL of the Ollama server, defaults to http://localhost:11434/api/embeddings
+        session (Optional[aiohttp.ClientSession]): Optional client session to use for requests.
     """
 
     url: HttpUrl = "http://localhost:11434/api/embeddings"
     session: aiohttp.ClientSession | None = None
 
+    @override
     async def generate_embeddings(self, texts: list[str], **kwargs: Any) -> ndarray:
-        """
-        Generates embeddings for a list of texts.
-
-        Arguments:
-            texts {List[str]} -- Texts to generate embeddings for.
-
-        Returns:
-            ndarray -- Embeddings for the texts.
-        """
         result = []
         for text in texts:
             async with AsyncSession(self.session) as session:
                 async with session.post(
                     self.url,
                     json={"model": self.ai_model_id, "prompt": text, "options": kwargs},
                 ) as response:
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/__init__.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,20 +21,20 @@
     detected: bool = False
     severity: ContentFilterResultSeverity = ContentFilterResultSeverity.SAFE
 
     @classmethod
     def from_inner_error_result(cls, inner_error_results: dict[str, Any]) -> "ContentFilterResult":
         """Creates a ContentFilterResult from the inner error results.
 
-        Arguments:
-            key {str} -- The key to get the inner error result from.
-            inner_error_results {Dict[str, Any]} -- The inner error results.
+        Args:
+            key (str): The key to get the inner error result from.
+            inner_error_results (Dict[str, Any]): The inner error results.
 
         Returns:
-            ContentFilterResult -- The ContentFilterResult.
+            ContentFilterResult: The ContentFilterResult.
         """
         return cls(
             filtered=inner_error_results.get("filtered", False),
             detected=inner_error_results.get("detected", False),
             severity=ContentFilterResultSeverity(
                 inner_error_results.get("severity", ContentFilterResultSeverity.SAFE.value)
             ),
@@ -43,15 +43,15 @@
 
 class ContentFilterCodes(Enum):
     RESPONSIBLE_AI_POLICY_VIOLATION = "ResponsibleAIPolicyViolation"
 
 
 @dataclass
 class ContentFilterAIException(ServiceContentFilterException):
-    """AI exception for an error from Azure OpenAI's content filter"""
+    """AI exception for an error from Azure OpenAI's content filter."""
 
     # The parameter that caused the error.
     param: str
 
     # The error code specific to the content filter.
     content_filter_code: ContentFilterCodes
 
@@ -61,17 +61,17 @@
     def __init__(
         self,
         message: str,
         inner_exception: BadRequestError,
     ) -> None:
         """Initializes a new instance of the ContentFilterAIException class.
 
-        Arguments:
-            message {str} -- The error message.
-            inner_exception {Exception} -- The inner exception.
+        Args:
+            message (str): The error message.
+            inner_exception (Exception): The inner exception.
         """
         super().__init__(message)
 
         self.param = inner_exception.param
 
         inner_error = inner_exception.body.get("innererror", {})
         self.content_filter_code = ContentFilterCodes(
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 
 class ExtraBody(KernelBaseModel):
     data_sources: list[DataSource] | None = None
     input_language: str | None = Field(None, serialization_alias="inputLanguage")
     output_language: str | None = Field(None, serialization_alias="outputLanguage")
 
     def __getitem__(self, item):
+        """Get an item from the ExtraBody."""
         return getattr(self, item)
 
 
 class AzureChatPromptExecutionSettings(OpenAIChatPromptExecutionSettings):
     """Specific settings for the Azure OpenAI Chat Completion endpoint."""
 
     response_format: str | None = None
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     echo: bool = False
     logprobs: int | None = Field(None, ge=0, le=5)
     suffix: str | None = None
 
     @model_validator(mode="after")
     def check_best_of_and_n(self) -> "OpenAITextPromptExecutionSettings":
         """Check that the best_of parameter is not greater than the number_of_responses parameter."""
-
         best_of = self.best_of or self.extension_data.get("best_of")
         number_of_responses = self.number_of_responses or self.extension_data.get("number_of_responses")
 
         if best_of is not None and number_of_responses is not None and best_of < number_of_responses:
             raise ServiceInvalidExecutionSettingsError(
                 "When used with number_of_responses, best_of controls the number of candidate completions and n specifies how many to return, therefore best_of must be greater than number_of_responses."  # noqa: E501
             )
@@ -63,14 +62,15 @@
     functions: list[dict[str, Any]] | None = None
     messages: list[dict[str, Any]] | None = None
     function_call_behavior: FunctionCallBehavior | None = Field(None, exclude=True)
 
     @field_validator("functions", "function_call", mode="after")
     @classmethod
     def validate_function_call(cls, v: str | list[dict[str, Any]] | None = None):
+        """Validate the function_call and functions parameters."""
         if v is not None:
             logger.warning(
                 "The function_call and functions parameters are deprecated. Please use the tool_choice and tools parameters instead."  # noqa: E501
             )
         return v
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,35 +48,34 @@
         api_version: str | None = None,
         ad_token: str | None = None,
         ad_token_provider: AsyncAzureADTokenProvider | None = None,
         default_headers: Mapping[str, str] | None = None,
         async_client: AsyncAzureOpenAI | None = None,
         env_file_path: str | None = None,
     ) -> None:
-        """
-        Initialize an AzureChatCompletion service.
+        """Initialize an AzureChatCompletion service.
 
-        Arguments:
-            service_id {str | None}: The service ID for the Azure deployment. (Optional)
-            api_key  {str | None}: The optional api key. If provided, will override the value in the
+        Args:
+            service_id (str | None): The service ID for the Azure deployment. (Optional)
+            api_key  (str | None): The optional api key. If provided, will override the value in the
                 env vars or .env file.
-            deployment_name  {str | None}: The optional deployment. If provided, will override the value
+            deployment_name  (str | None): The optional deployment. If provided, will override the value
                 (chat_deployment_name) in the env vars or .env file.
-            endpoint {str | None}: The optional deployment endpoint. If provided will override the value
+            endpoint (str | None): The optional deployment endpoint. If provided will override the value
                 in the env vars or .env file.
-            base_url {str | None}: The optional deployment base_url. If provided will override the value
+            base_url (str | None): The optional deployment base_url. If provided will override the value
                 in the env vars or .env file.
-            api_version {str | None}: The optional deployment api version. If provided will override the value
+            api_version (str | None): The optional deployment api version. If provided will override the value
                 in the env vars or .env file.
-            ad_token {str | None}: The Azure Active Directory token. (Optional)
-            ad_token_provider {AsyncAzureADTokenProvider}: The Azure Active Directory token provider. (Optional)
-            default_headers {Mapping[str, str]}: The default headers mapping of string keys to
+            ad_token (str | None): The Azure Active Directory token. (Optional)
+            ad_token_provider (AsyncAzureADTokenProvider): The Azure Active Directory token provider. (Optional)
+            default_headers (Mapping[str, str]): The default headers mapping of string keys to
                 string values for HTTP requests. (Optional)
-            async_client {AsyncAzureOpenAI | None} -- An existing client to use. (Optional)
-            env_file_path {str | None} -- Use the environment settings file as a fallback to using env vars.
+            async_client (AsyncAzureOpenAI | None): An existing client to use. (Optional)
+            env_file_path (str | None): Use the environment settings file as a fallback to using env vars.
         """
         azure_openai_settings = None
         try:
             azure_openai_settings = AzureOpenAISettings.create(env_file_path=env_file_path)
         except ValidationError as e:
             logger.warning(f"Failed to load AzureOpenAI pydantic settings: {e}")
 
@@ -118,23 +117,21 @@
             default_headers=default_headers,
             ai_model_type=OpenAIModelTypes.CHAT,
             async_client=async_client,
         )
 
     @classmethod
     def from_dict(cls, settings: dict[str, str]) -> "AzureChatCompletion":
-        """
-        Initialize an Azure OpenAI service from a dictionary of settings.
+        """Initialize an Azure OpenAI service from a dictionary of settings.
 
-        Arguments:
+        Args:
             settings: A dictionary of settings for the service.
-                should contains keys: service_id, and optionally:
+                should contain keys: service_id, and optionally:
                     ad_auth, ad_token_provider, default_headers
         """
-
         return AzureChatCompletion(
             service_id=settings.get("service_id"),
             api_key=settings.get("api_key", None),
             deployment_name=settings.get("deployment_name", None),
             endpoint=settings.get("endpoint", None),
             base_url=settings.get("base_url", None),
             api_version=settings.get("api_version", None),
@@ -147,25 +144,25 @@
     def get_prompt_execution_settings_class(self) -> "PromptExecutionSettings":
         """Create a request settings object."""
         return AzureChatPromptExecutionSettings
 
     def _create_chat_message_content(
         self, response: ChatCompletion, choice: Choice, response_metadata: dict[str, Any]
     ) -> ChatMessageContent:
-        """Create a Azure chat message content object from a choice."""
+        """Create an Azure chat message content object from a choice."""
         content = super()._create_chat_message_content(response, choice, response_metadata)
         return self._add_tool_message_to_chat_message_content(content, choice)
 
     def _create_streaming_chat_message_content(
         self,
         chunk: ChatCompletionChunk,
         choice: ChunkChoice,
         chunk_metadata: dict[str, Any],
     ) -> "StreamingChatMessageContent":
-        """Create a Azure streaming chat message content object from a choice."""
+        """Create an Azure streaming chat message content object from a choice."""
         content = super()._create_streaming_chat_message_content(chunk, choice, chunk_metadata)
         return self._add_tool_message_to_chat_message_content(content, choice)
 
     def _add_tool_message_to_chat_message_content(
         self, content: ChatMessageContent | StreamingChatMessageContent, choice: Choice
     ) -> "ChatMessageContent | StreamingChatMessageContent":
         if tool_message := self._get_tool_message_from_chat_choice(choice=choice):
@@ -196,15 +193,15 @@
         if content.model_extra is not None and "context" in content.model_extra:
             return json.dumps(content.model_extra["context"])
 
         return None
 
     @staticmethod
     def split_message(message: "ChatMessageContent") -> list["ChatMessageContent"]:
-        """Split a Azure On Your Data response into separate ChatMessageContents.
+        """Split an Azure On Your Data response into separate ChatMessageContents.
 
         If the message does not have three contents, and those three are one each of:
         FunctionCallContent, FunctionResultContent, and TextContent,
         it will not return three messages, potentially only one or two.
 
         The order of the returned messages is as expected by OpenAI.
         """
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,29 +31,31 @@
         ad_token: str | None = None,
         ad_token_provider: Callable[[], str | Awaitable[str]] | None = None,
         default_headers: Mapping[str, str] | None = None,
         async_client: AsyncAzureOpenAI | None = None,
     ) -> None:
         """Internal class for configuring a connection to an Azure OpenAI service.
 
-        Arguments:
-            deployment_name {str} -- Name of the deployment.
-            ai_model_type {OpenAIModelTypes} -- The type of OpenAI model to deploy.
-            endpoint {Optional[HttpsUrl]} -- The specific endpoint URL for the deployment. (Optional)
-            base_url {Optional[HttpsUrl]} -- The base URL for Azure services. (Optional)
-            api_version {str} -- Azure API version. Defaults to the defined DEFAULT_AZURE_API_VERSION.
-            api_key {Optional[str]} -- API key for Azure services. (Optional)
-            ad_token {Optional[str]} -- Azure AD token for authentication. (Optional)
-            ad_token_provider {Optional[Callable[[], Union[str, Awaitable[str]]]]} -- A callable
-                or coroutine function providing Azure AD tokens. (Optional)
-            default_headers {Union[Mapping[str, str], None]} -- Default headers for HTTP requests. (Optional)
-            async_client {Optional[AsyncAzureOpenAI]} -- An existing client to use. (Optional)
-
         The `validate_call` decorator is used with a configuration that allows arbitrary types.
         This is necessary for types like `HttpsUrl` and `OpenAIModelTypes`.
+
+        Args:
+            deployment_name (str): Name of the deployment.
+            ai_model_type (OpenAIModelTypes): The type of OpenAI model to deploy.
+            endpoint (Optional[HttpsUrl]): The specific endpoint URL for the deployment. (Optional)
+            base_url (Optional[HttpsUrl]): The base URL for Azure services. (Optional)
+            api_version (str): Azure API version. Defaults to the defined DEFAULT_AZURE_API_VERSION.
+            service_id (Optional[str]): Service ID for the deployment. (Optional)
+            api_key (Optional[str]): API key for Azure services. (Optional)
+            ad_token (Optional[str]): Azure AD token for authentication. (Optional)
+            ad_token_provider (Optional[Callable[[], Union[str, Awaitable[str]]]]): A callable
+                or coroutine function providing Azure AD tokens. (Optional)
+            default_headers (Union[Mapping[str, str], None]): Default headers for HTTP requests. (Optional)
+            async_client (Optional[AsyncAzureOpenAI]): An existing client to use. (Optional)
+
         """
         # Merge APP_INFO into the headers if it exists
         merged_headers = default_headers.copy() if default_headers else {}
         if APP_INFO:
             merged_headers.update(APP_INFO)
             merged_headers = prepend_semantic_kernel_to_user_agent(merged_headers)
 
@@ -87,14 +89,15 @@
             "ai_model_type": ai_model_type,
         }
         if service_id:
             args["service_id"] = service_id
         super().__init__(**args)
 
     def to_dict(self) -> dict[str, str]:
+        """Convert the configuration to a dictionary."""
         client_settings = {
             "base_url": str(self.client.base_url),
             "api_version": self.client._custom_query["api-version"],
             "api_key": self.client.api_key,
             "ad_token": self.client._azure_ad_token,
             "ad_token_provider": self.client._azure_ad_token_provider,
             "default_headers": {k: v for k, v in self.client.default_headers.items() if k != USER_AGENT},
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 # Copyright (c) Microsoft. All rights reserved.
 
+
 import logging
 from collections.abc import Mapping
 
 from openai import AsyncAzureOpenAI
 from openai.lib.azure import AsyncAzureADTokenProvider
 from pydantic import ValidationError
 
 from semantic_kernel.connectors.ai.open_ai.const import DEFAULT_AZURE_API_VERSION
-from semantic_kernel.connectors.ai.open_ai.services.azure_config_base import (
-    AzureOpenAIConfigBase,
-)
-from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import (
-    OpenAIModelTypes,
-)
-from semantic_kernel.connectors.ai.open_ai.services.open_ai_text_completion_base import (
-    OpenAITextCompletionBase,
-)
+from semantic_kernel.connectors.ai.open_ai.services.azure_config_base import AzureOpenAIConfigBase
+from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import OpenAIModelTypes
+from semantic_kernel.connectors.ai.open_ai.services.open_ai_text_embedding_base import OpenAITextEmbeddingBase
 from semantic_kernel.connectors.ai.open_ai.settings.azure_open_ai_settings import AzureOpenAISettings
 from semantic_kernel.exceptions.service_exceptions import ServiceInitializationError
 from semantic_kernel.kernel_pydantic import HttpsUrl
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-class AzureTextCompletion(AzureOpenAIConfigBase, OpenAITextCompletionBase):
-    """Azure Text Completion class."""
+@experimental_class
+class AzureTextEmbedding(AzureOpenAIConfigBase, OpenAITextEmbeddingBase):
+    """Azure Text Embedding class."""
 
     def __init__(
         self,
         service_id: str | None = None,
         api_key: str | None = None,
         deployment_name: str | None = None,
         endpoint: str | None = None,
@@ -37,51 +34,50 @@
         api_version: str | None = None,
         ad_token: str | None = None,
         ad_token_provider: AsyncAzureADTokenProvider | None = None,
         default_headers: Mapping[str, str] | None = None,
         async_client: AsyncAzureOpenAI | None = None,
         env_file_path: str | None = None,
     ) -> None:
-        """
-        Initialize an AzureTextCompletion service.
+        """Initialize an AzureTextEmbedding service.
 
-        Arguments:
-            service_id: The service ID for the Azure deployment. (Optional)
-            api_key  {str | None}: The optional api key. If provided, will override the value in the
+        service_id: The service ID. (Optional)
+        api_key  {str | None}: The optional api key. If provided, will override the value in the
                 env vars or .env file.
-            deployment_name  {str | None}: The optional deployment. If provided, will override the value
-                (text_deployment_name) in the env vars or .env file.
-            endpoint {str | None}: The optional deployment endpoint. If provided will override the value
-                in the env vars or .env file.
-            base_url {str | None}: The optional deployment base_url. If provided will override the value
-                in the env vars or .env file.
-            api_version {str | None}: The optional deployment api version. If provided will override the value
-                in the env vars or .env file.
-            ad_token: The Azure Active Directory token. (Optional)
-            ad_token_provider: The Azure Active Directory token provider. (Optional)
-            default_headers: The default headers mapping of string keys to
+        deployment_name  {str | None}: The optional deployment. If provided, will override the value
+            (text_deployment_name) in the env vars or .env file.
+        endpoint {str | None}: The optional deployment endpoint. If provided will override the value
+            in the env vars or .env file.
+        base_url {str | None}: The optional deployment base_url. If provided will override the value
+            in the env vars or .env file.
+        api_version {str | None}: The optional deployment api version. If provided will override the value
+            in the env vars or .env file.
+        ad_token {str | None}: The Azure AD token for authentication. (Optional)
+        ad_auth {AsyncAzureADTokenProvider | None}: Whether to use Azure Active Directory authentication.
+            (Optional) The default value is False.
+        default_headers: The default headers mapping of string keys to
                 string values for HTTP requests. (Optional)
-            async_client {Optional[AsyncAzureOpenAI]} -- An existing client to use. (Optional)
-            env_file_path {str | None} -- Use the environment settings file as a fallback to
-                environment variables. (Optional)
+        async_client (Optional[AsyncAzureOpenAI]): An existing client to use. (Optional)
+        env_file_path (str | None): Use the environment settings file as a fallback to
+            environment variables. (Optional)
         """
         azure_openai_settings = None
         try:
             azure_openai_settings = AzureOpenAISettings.create(env_file_path=env_file_path)
         except ValidationError as e:
             logger.warning(f"Failed to load AzureOpenAI pydantic settings: {e}")
 
         base_url = base_url or (
             str(azure_openai_settings.base_url) if azure_openai_settings and azure_openai_settings.base_url else None
         )
         endpoint = endpoint or (
             str(azure_openai_settings.endpoint) if azure_openai_settings and azure_openai_settings.endpoint else None
         )
         deployment_name = deployment_name or (
-            azure_openai_settings.text_deployment_name if azure_openai_settings else None
+            azure_openai_settings.embedding_deployment_name if azure_openai_settings else None
         )
         api_version = api_version or (azure_openai_settings.api_version if azure_openai_settings else None)
         api_key = api_key or (
             azure_openai_settings.api_key.get_secret_value()
             if azure_openai_settings and azure_openai_settings.api_key
             else None
         )
@@ -103,30 +99,28 @@
             base_url=base_url,
             api_version=api_version,
             service_id=service_id,
             api_key=api_key,
             ad_token=ad_token,
             ad_token_provider=ad_token_provider,
             default_headers=default_headers,
-            ai_model_type=OpenAIModelTypes.TEXT,
+            ai_model_type=OpenAIModelTypes.EMBEDDING,
             async_client=async_client,
         )
 
     @classmethod
-    def from_dict(cls, settings: dict[str, str]) -> "AzureTextCompletion":
-        """
-        Initialize an Azure OpenAI service from a dictionary of settings.
+    def from_dict(cls, settings: dict[str, str]) -> "AzureTextEmbedding":
+        """Initialize an Azure OpenAI service from a dictionary of settings.
 
-        Arguments:
+        Args:
             settings: A dictionary of settings for the service.
-                should contains keys: deployment_name, endpoint, api_key
+                should contain keys: deployment_name, endpoint, api_key
                 and optionally: api_version, ad_auth
         """
-
-        return AzureTextCompletion(
+        return AzureTextEmbedding(
             service_id=settings.get("service_id"),
             api_key=settings.get("api_key", None),
             deployment_name=settings.get("deployment_name", None),
             endpoint=settings.get("endpoint", None),
             base_url=settings.get("base_url", None),
             api_version=settings.get("api_version", None),
             ad_token=settings.get("ad_token"),
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,29 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-
 import logging
 from collections.abc import Mapping
 
 from openai import AsyncAzureOpenAI
 from openai.lib.azure import AsyncAzureADTokenProvider
 from pydantic import ValidationError
 
 from semantic_kernel.connectors.ai.open_ai.const import DEFAULT_AZURE_API_VERSION
-from semantic_kernel.connectors.ai.open_ai.services.azure_config_base import (
-    AzureOpenAIConfigBase,
-)
-from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import (
-    OpenAIModelTypes,
-)
-from semantic_kernel.connectors.ai.open_ai.services.open_ai_text_embedding_base import (
-    OpenAITextEmbeddingBase,
-)
+from semantic_kernel.connectors.ai.open_ai.services.azure_config_base import AzureOpenAIConfigBase
+from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import OpenAIModelTypes
+from semantic_kernel.connectors.ai.open_ai.services.open_ai_text_completion_base import OpenAITextCompletionBase
 from semantic_kernel.connectors.ai.open_ai.settings.azure_open_ai_settings import AzureOpenAISettings
 from semantic_kernel.exceptions.service_exceptions import ServiceInitializationError
 from semantic_kernel.kernel_pydantic import HttpsUrl
-from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-@experimental_class
-class AzureTextEmbedding(AzureOpenAIConfigBase, OpenAITextEmbeddingBase):
-    """Azure Text Embedding class."""
+class AzureTextCompletion(AzureOpenAIConfigBase, OpenAITextCompletionBase):
+    """Azure Text Completion class."""
 
     def __init__(
         self,
         service_id: str | None = None,
         api_key: str | None = None,
         deployment_name: str | None = None,
         endpoint: str | None = None,
@@ -40,51 +31,50 @@
         api_version: str | None = None,
         ad_token: str | None = None,
         ad_token_provider: AsyncAzureADTokenProvider | None = None,
         default_headers: Mapping[str, str] | None = None,
         async_client: AsyncAzureOpenAI | None = None,
         env_file_path: str | None = None,
     ) -> None:
-        """
-        Initialize an AzureTextEmbedding service.
+        """Initialize an AzureTextCompletion service.
 
-        service_id: The service ID. (Optional)
-        api_key  {str | None}: The optional api key. If provided, will override the value in the
+        Args:
+            service_id: The service ID for the Azure deployment. (Optional)
+            api_key (str | None): The optional api key. If provided, will override the value in the
                 env vars or .env file.
-        deployment_name  {str | None}: The optional deployment. If provided, will override the value
-            (text_deployment_name) in the env vars or .env file.
-        endpoint {str | None}: The optional deployment endpoint. If provided will override the value
-            in the env vars or .env file.
-        base_url {str | None}: The optional deployment base_url. If provided will override the value
-            in the env vars or .env file.
-        api_version {str | None}: The optional deployment api version. If provided will override the value
-            in the env vars or .env file.
-        ad_token {str | None}: The Azure AD token for authentication. (Optional)
-        ad_auth {AsyncAzureADTokenProvider | None}: Whether to use Azure Active Directory authentication.
-            (Optional) The default value is False.
-        default_headers: The default headers mapping of string keys to
+            deployment_name  (str | None): The optional deployment. If provided, will override the value
+                (text_deployment_name) in the env vars or .env file.
+            endpoint (str | None): The optional deployment endpoint. If provided will override the value
+                in the env vars or .env file.
+            base_url (str | None): The optional deployment base_url. If provided will override the value
+                in the env vars or .env file.
+            api_version (str | None): The optional deployment api version. If provided will override the value
+                in the env vars or .env file.
+            ad_token: The Azure Active Directory token. (Optional)
+            ad_token_provider: The Azure Active Directory token provider. (Optional)
+            default_headers: The default headers mapping of string keys to
                 string values for HTTP requests. (Optional)
-        async_client {Optional[AsyncAzureOpenAI]} -- An existing client to use. (Optional)
-        env_file_path {str | None} -- Use the environment settings file as a fallback to
-            environment variables. (Optional)
+            async_client (Optional[AsyncAzureOpenAI]): An existing client to use. (Optional)
+            env_file_path (str | None): Use the environment settings file as a fallback to
+                environment variables. (Optional)
         """
         azure_openai_settings = None
         try:
             azure_openai_settings = AzureOpenAISettings.create(env_file_path=env_file_path)
         except ValidationError as e:
             logger.warning(f"Failed to load AzureOpenAI pydantic settings: {e}")
 
         base_url = base_url or (
             str(azure_openai_settings.base_url) if azure_openai_settings and azure_openai_settings.base_url else None
         )
         endpoint = endpoint or (
             str(azure_openai_settings.endpoint) if azure_openai_settings and azure_openai_settings.endpoint else None
         )
         deployment_name = deployment_name or (
-            azure_openai_settings.embedding_deployment_name if azure_openai_settings else None
+            azure_openai_settings.text_deployment_name if azure_openai_settings else None
         )
         api_version = api_version or (azure_openai_settings.api_version if azure_openai_settings else None)
         api_key = api_key or (
             azure_openai_settings.api_key.get_secret_value()
             if azure_openai_settings and azure_openai_settings.api_key
             else None
         )
@@ -106,29 +96,28 @@
             base_url=base_url,
             api_version=api_version,
             service_id=service_id,
             api_key=api_key,
             ad_token=ad_token,
             ad_token_provider=ad_token_provider,
             default_headers=default_headers,
-            ai_model_type=OpenAIModelTypes.EMBEDDING,
+            ai_model_type=OpenAIModelTypes.TEXT,
             async_client=async_client,
         )
 
     @classmethod
-    def from_dict(cls, settings: dict[str, str]) -> "AzureTextEmbedding":
-        """
-        Initialize an Azure OpenAI service from a dictionary of settings.
+    def from_dict(cls, settings: dict[str, str]) -> "AzureTextCompletion":
+        """Initialize an Azure OpenAI service from a dictionary of settings.
 
-        Arguments:
+        Args:
             settings: A dictionary of settings for the service.
-                should contains keys: deployment_name, endpoint, api_key
+                should contain keys: deployment_name, endpoint, api_key
                 and optionally: api_version, ad_auth
         """
-        return AzureTextEmbedding(
+        return AzureTextCompletion(
             service_id=settings.get("service_id"),
             api_key=settings.get("api_key", None),
             deployment_name=settings.get("deployment_name", None),
             endpoint=settings.get("endpoint", None),
             base_url=settings.get("base_url", None),
             api_version=settings.get("api_version", None),
             ad_token=settings.get("ad_token"),
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,20 +4,16 @@
 from collections.abc import Mapping
 
 from openai import AsyncOpenAI
 from pydantic import ValidationError
 
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_chat_completion_base import OpenAIChatCompletionBase
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_config_base import OpenAIConfigBase
-from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import (
-    OpenAIModelTypes,
-)
-from semantic_kernel.connectors.ai.open_ai.services.open_ai_text_completion_base import (
-    OpenAITextCompletionBase,
-)
+from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import OpenAIModelTypes
+from semantic_kernel.connectors.ai.open_ai.services.open_ai_text_completion_base import OpenAITextCompletionBase
 from semantic_kernel.connectors.ai.open_ai.settings.open_ai_settings import OpenAISettings
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class OpenAIChatCompletion(OpenAIConfigBase, OpenAIChatCompletionBase, OpenAITextCompletionBase):
     """OpenAI Chat completion class."""
@@ -28,29 +24,28 @@
         service_id: str | None = None,
         api_key: str | None = None,
         org_id: str | None = None,
         default_headers: Mapping[str, str] | None = None,
         async_client: AsyncOpenAI | None = None,
         env_file_path: str | None = None,
     ) -> None:
-        """
-        Initialize an OpenAIChatCompletion service.
+        """Initialize an OpenAIChatCompletion service.
 
-        Arguments:
-            ai_model_id {str} -- OpenAI model name, see
+        Args:
+            ai_model_id (str): OpenAI model name, see
                 https://platform.openai.com/docs/models
-            service_id {str | None} -- Service ID tied to the execution settings.
-            api_key {str | None} -- The optional API key to use. If provided will override,
+            service_id (str | None): Service ID tied to the execution settings.
+            api_key (str | None): The optional API key to use. If provided will override,
                 the env vars or .env file value.
-            org_id {str | None} -- The optional org ID to use. If provided will override,
+            org_id (str | None): The optional org ID to use. If provided will override,
                 the env vars or .env file value.
             default_headers: The default headers mapping of string keys to
                 string values for HTTP requests. (Optional)
-            async_client {Optional[AsyncOpenAI]} -- An existing client to use. (Optional)
-            env_file_path {str | None} -- Use the environment settings file as a fallback
+            async_client (Optional[AsyncOpenAI]): An existing client to use. (Optional)
+            env_file_path (str | None): Use the environment settings file as a fallback
                 to environment variables. (Optional)
         """
         openai_settings = None
         try:
             openai_settings = OpenAISettings.create(env_file_path=env_file_path)
         except ValidationError as e:
             logger.warning(f"Failed to load OpenAI pydantic settings: {e}")
@@ -71,19 +66,17 @@
             ai_model_type=OpenAIModelTypes.CHAT,
             default_headers=default_headers,
             async_client=async_client,
         )
 
     @classmethod
     def from_dict(cls, settings: dict[str, str]) -> "OpenAIChatCompletion":
-        """
-        Initialize an Open AI service from a dictionary of settings.
+        """Initialize an Open AI service from a dictionary of settings.
 
-        Arguments:
+        Args:
             settings: A dictionary of settings for the service.
         """
-
         return OpenAIChatCompletion(
             ai_model_id=settings["ai_model_id"],
             service_id=settings.get("service_id"),
             default_headers=settings.get("default_headers"),
         )
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,24 +73,23 @@
         self,
         chat_history: ChatHistory,
         settings: OpenAIChatPromptExecutionSettings,
         **kwargs: Any,
     ) -> list["ChatMessageContent"]:
         """Executes a chat completion request and returns the result.
 
-        Arguments:
-            chat_history {ChatHistory} -- The chat history to use for the chat completion.
-            settings {OpenAIChatPromptExecutionSettings | AzureChatPromptExecutionSettings} -- The settings to use
+        Args:
+            chat_history (ChatHistory): The chat history to use for the chat completion.
+            settings (OpenAIChatPromptExecutionSettings | AzureChatPromptExecutionSettings): The settings to use
                 for the chat completion request.
-            kwargs {Dict[str, Any]} -- The optional arguments.
+            kwargs (Dict[str, Any]): The optional arguments.
 
         Returns:
-            List[ChatMessageContent] -- The completion result(s).
+            List[ChatMessageContent]: The completion result(s).
         """
-
         kernel = kwargs.get("kernel", None)
         arguments = kwargs.get("arguments", None)
         if settings.function_call_behavior is not None and settings.function_call_behavior.auto_invoke_kernel_functions:
             if kernel is None or arguments is None:
                 raise ServiceInvalidExecutionSettingsError(
                     "The kernel and kernel arguments are required for auto invoking OpenAI tool calls."
                 )
@@ -150,22 +149,22 @@
         self,
         chat_history: ChatHistory,
         settings: OpenAIChatPromptExecutionSettings,
         **kwargs: Any,
     ) -> AsyncGenerator[list[StreamingChatMessageContent | None], Any]:
         """Executes a streaming chat completion request and returns the result.
 
-        Arguments:
-            chat_history {ChatHistory} -- The chat history to use for the chat completion.
-            settings {OpenAIChatPromptExecutionSettings | AzureChatPromptExecutionSettings} -- The settings to use
+        Args:
+            chat_history (ChatHistory): The chat history to use for the chat completion.
+            settings (OpenAIChatPromptExecutionSettings | AzureChatPromptExecutionSettings): The settings to use
                 for the chat completion request.
-            kwargs {Dict[str, Any]} -- The optional arguments.
+            kwargs (Dict[str, Any]): The optional arguments.
 
         Yields:
-            List[StreamingChatMessageContent] -- A stream of
+            List[StreamingChatMessageContent]: A stream of
                 StreamingChatMessageContent when using Azure.
         """
         kernel = kwargs.get("kernel", None)
         arguments = kwargs.get("arguments", None)
         if settings.function_call_behavior is not None and settings.function_call_behavior.auto_invoke_kernel_functions:
             if kernel is None or arguments is None:
                 raise ServiceInvalidExecutionSettingsError(
@@ -254,26 +253,26 @@
                 msg["name"] = message.metadata["function_name"]
         return msg
 
     # endregion
     # region internal handlers
 
     async def _send_chat_request(self, settings: OpenAIChatPromptExecutionSettings) -> list["ChatMessageContent"]:
-        """Send the chat request"""
+        """Send the chat request."""
         response = await self._send_request(request_settings=settings)
         response_metadata = self._get_metadata_from_chat_response(response)
         completions = [
             self._create_chat_message_content(response, choice, response_metadata) for choice in response.choices
         ]
         return completions
 
     async def _send_chat_stream_request(
         self, settings: OpenAIChatPromptExecutionSettings
     ) -> AsyncGenerator[list["StreamingChatMessageContent | None"], None]:
-        """Send the chat stream request"""
+        """Send the chat stream request."""
         response = await self._send_request(request_settings=settings)
         if not isinstance(response, AsyncStream):
             raise ServiceInvalidResponseError("Expected an AsyncStream[ChatCompletionChunk] response.")
         async for chunk in response:
             if len(chunk.choices) == 0:
                 continue
             chunk_metadata = self._get_metadata_from_streaming_chat_response(chunk)
@@ -522,13 +521,15 @@
         try:
             result = await context.function.invoke(context.kernel, context.arguments)
             if result:
                 context.function_result = result
         except Exception as exc:
             logger.exception(f"Error invoking function {context.function.fully_qualified_name}: {exc}.")
             value = f"An error occurred while invoking the function {context.function.fully_qualified_name}: {exc}"
-            assert context.function_result is not None
-            context.function_result.value = value
+            if context.function_result is not None:
+                context.function_result.value = value
+            else:
+                context.function_result = FunctionResult(function=context.function.metadata, value=value)
             return
 
 
 # endregion
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,25 +28,27 @@
         async_client: AsyncOpenAI | None = None,
     ) -> None:
         """Initialize a client for OpenAI services.
 
         This constructor sets up a client to interact with OpenAI's API, allowing for
         different types of AI model interactions, like chat or text completion.
 
-        Arguments:
-            ai_model_id {str} -- OpenAI model identifier. Must be non-empty.
+        Args:
+            ai_model_id (str): OpenAI model identifier. Must be non-empty.
                 Default to a preset value.
-            api_key {Optional[str]} -- OpenAI API key for authentication.
+            api_key (Optional[str]): OpenAI API key for authentication.
                 Must be non-empty. (Optional)
-            ai_model_type {Optional[OpenAIModelTypes]} -- The type of OpenAI
+            ai_model_type (Optional[OpenAIModelTypes]): The type of OpenAI
                 model to interact with. Defaults to CHAT.
-            org_id {Optional[str]} -- OpenAI organization ID. This is optional
+            org_id (Optional[str]): OpenAI organization ID. This is optional
                 unless the account belongs to multiple organizations.
-            default_headers {Optional[Mapping[str, str]]} -- Default headers
+            service_id (Optional[str]): OpenAI service ID. This is optional.
+            default_headers (Optional[Mapping[str, str]]): Default headers
                 for HTTP requests. (Optional)
+            async_client (Optional[AsyncOpenAI]): An existing OpenAI client
 
         """
         # Merge APP_INFO into the headers if it exists
         merged_headers = default_headers.copy() if default_headers else {}
         if APP_INFO:
             merged_headers.update(APP_INFO)
             merged_headers = prepend_semantic_kernel_to_user_agent(merged_headers)
@@ -65,17 +67,15 @@
             "ai_model_type": ai_model_type,
         }
         if service_id:
             args["service_id"] = service_id
         super().__init__(**args)
 
     def to_dict(self) -> dict[str, str]:
-        """
-        Create a dict of the service settings.
-        """
+        """Create a dict of the service settings."""
         client_settings = {
             "api_key": self.client.api_key,
             "default_headers": {k: v for k, v in self.client.default_headers.items() if k != USER_AGENT},
         }
         if self.client.organization:
             client_settings["org_id"] = self.client.organization
         base = self.model_dump(
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,20 @@
 from abc import ABC
 
 from numpy import array, ndarray
 from openai import AsyncOpenAI, AsyncStream, BadRequestError
 from openai.types import Completion
 from openai.types.chat import ChatCompletion, ChatCompletionChunk
 
-from semantic_kernel.connectors.ai.open_ai.exceptions.content_filter_ai_exception import (
-    ContentFilterAIException,
-)
+from semantic_kernel.connectors.ai.open_ai.exceptions.content_filter_ai_exception import ContentFilterAIException
 from semantic_kernel.connectors.ai.open_ai.prompt_execution_settings.open_ai_prompt_execution_settings import (
     OpenAIEmbeddingPromptExecutionSettings,
     OpenAIPromptExecutionSettings,
 )
-from semantic_kernel.connectors.ai.open_ai.services.open_ai_model_types import (
-    OpenAIModelTypes,
-)
+from semantic_kernel.connectors.ai.open_ai.services.open_ai_model_types import OpenAIModelTypes
 from semantic_kernel.exceptions import ServiceResponseException
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class OpenAIHandler(KernelBaseModel, ABC):
@@ -33,28 +29,27 @@
     completion_tokens: int = 0
     total_tokens: int = 0
 
     async def _send_request(
         self,
         request_settings: OpenAIPromptExecutionSettings,
     ) -> ChatCompletion | Completion | AsyncStream[ChatCompletionChunk] | AsyncStream[Completion]:
-        """
-        Completes the given prompt. Returns a single string completion.
+        """Completes the given prompt. Returns a single string completion.
+
         Cannot return multiple completions. Cannot return logprobs.
 
-        Arguments:
-            prompt {str} -- The prompt to complete.
-            messages {List[Tuple[str, str]]} -- A list of tuples, where each tuple is a role and content set.
-            request_settings {OpenAIPromptExecutionSettings} -- The request settings.
-            stream {bool} -- Whether to stream the response.
+        Args:
+            prompt (str): The prompt to complete.
+            messages (List[Tuple[str, str]]): A list of tuples, where each tuple is a role and content set.
+            request_settings (OpenAIPromptExecutionSettings): The request settings.
+            stream (bool): Whether to stream the response.
 
         Returns:
-            ChatCompletion, Completion, AsyncStream[Completion | ChatCompletionChunk] -- The completion response.
+            ChatCompletion, Completion, AsyncStream[Completion | ChatCompletionChunk]: The completion response.
         """
-
         try:
             if self.ai_model_type == OpenAIModelTypes.CHAT:
                 response = await self.client.chat.completions.create(**request_settings.prepare_settings_dict())
             else:
                 response = await self.client.completions.create(**request_settings.prepare_settings_dict())
             self.store_usage(response)
             return response
@@ -84,13 +79,14 @@
         except Exception as ex:
             raise ServiceResponseException(
                 f"{type(self)} service failed to generate embeddings",
                 ex,
             ) from ex
 
     def store_usage(self, response):
+        """Store the usage information from the response."""
         if not isinstance(response, AsyncStream):
             logger.info(f"OpenAI usage: {response.usage}")
             self.prompt_tokens += response.usage.prompt_tokens
             self.total_tokens += response.usage.total_tokens
             if hasattr(response.usage, "completion_tokens"):
                 self.completion_tokens += response.usage.completion_tokens
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,17 @@
 import json
 import logging
 from collections.abc import Mapping
 
 from openai import AsyncOpenAI
 from pydantic import ValidationError
 
-from semantic_kernel.connectors.ai.open_ai.services.open_ai_config_base import (
-    OpenAIConfigBase,
-)
-from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import (
-    OpenAIModelTypes,
-)
-from semantic_kernel.connectors.ai.open_ai.services.open_ai_text_completion_base import (
-    OpenAITextCompletionBase,
-)
+from semantic_kernel.connectors.ai.open_ai.services.open_ai_config_base import OpenAIConfigBase
+from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import OpenAIModelTypes
+from semantic_kernel.connectors.ai.open_ai.services.open_ai_text_completion_base import OpenAITextCompletionBase
 from semantic_kernel.connectors.ai.open_ai.settings.open_ai_settings import OpenAISettings
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class OpenAITextCompletion(OpenAITextCompletionBase, OpenAIConfigBase):
     """OpenAI Text Completion class."""
@@ -30,29 +24,28 @@
         api_key: str | None = None,
         org_id: str | None = None,
         service_id: str | None = None,
         default_headers: Mapping[str, str] | None = None,
         async_client: AsyncOpenAI | None = None,
         env_file_path: str | None = None,
     ) -> None:
-        """
-        Initialize an OpenAITextCompletion service.
+        """Initialize an OpenAITextCompletion service.
 
-        Arguments:
-            ai_model_id {str | None} -- OpenAI model name, see
+        Args:
+            ai_model_id (str | None): OpenAI model name, see
                 https://platform.openai.com/docs/models
-            service_id {str | None} -- Service ID tied to the execution settings.
-            api_key {str | None} -- The optional API key to use. If provided will override,
+            service_id (str | None): Service ID tied to the execution settings.
+            api_key (str | None): The optional API key to use. If provided will override,
                 the env vars or .env file value.
-            org_id {str | None} -- The optional org ID to use. If provided will override,
+            org_id (str | None): The optional org ID to use. If provided will override,
                 the env vars or .env file value.
             default_headers: The default headers mapping of string keys to
                 string values for HTTP requests. (Optional)
-            async_client {Optional[AsyncOpenAI]} -- An existing client to use. (Optional)
-            env_file_path {str | None} -- Use the environment settings file as a fallback to
+            async_client (Optional[AsyncOpenAI]): An existing client to use. (Optional)
+            env_file_path (str | None): Use the environment settings file as a fallback to
                 environment variables. (Optional)
         """
         try:
             openai_settings = OpenAISettings.create(env_file_path=env_file_path)
         except ValidationError as e:
             logger.warning(f"Failed to load OpenAI pydantic settings: {e}")
 
@@ -72,18 +65,17 @@
             ai_model_type=OpenAIModelTypes.TEXT,
             default_headers=default_headers,
             async_client=async_client,
         )
 
     @classmethod
     def from_dict(cls, settings: dict[str, str]) -> "OpenAITextCompletion":
-        """
-        Initialize an Open AI service from a dictionary of settings.
+        """Initialize an Open AI service from a dictionary of settings.
 
-        Arguments:
+        Args:
             settings: A dictionary of settings for the service.
         """
         if "default_headers" in settings and isinstance(settings["default_headers"], str):
             settings["default_headers"] = json.loads(settings["default_headers"])
         return OpenAITextCompletion(
             ai_model_id=settings.get("ai_model_id", None),
             api_key=settings.get("api_key", None),
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,20 +35,20 @@
     async def get_text_contents(
         self,
         prompt: str,
         settings: "OpenAIPromptExecutionSettings",
     ) -> list["TextContent"]:
         """Executes a completion request and returns the result.
 
-        Arguments:
-            prompt {str} -- The prompt to use for the completion request.
-            settings {OpenAITextPromptExecutionSettings} -- The settings to use for the completion request.
+        Args:
+            prompt (str): The prompt to use for the completion request.
+            settings (OpenAITextPromptExecutionSettings): The settings to use for the completion request.
 
         Returns:
-            List["TextContent"] -- The completion result(s).
+            List["TextContent"]: The completion result(s).
         """
         if isinstance(settings, OpenAITextPromptExecutionSettings):
             settings.prompt = prompt
         else:
             settings.messages = [{"role": "user", "content": prompt}]
         if settings.ai_model_id is None:
             settings.ai_model_id = self.ai_model_id
@@ -74,24 +74,24 @@
         )
 
     async def get_streaming_text_contents(
         self,
         prompt: str,
         settings: "OpenAIPromptExecutionSettings",
     ) -> AsyncGenerator[list["StreamingTextContent"], Any]:
-        """
-        Executes a completion request and streams the result.
+        """Executes a completion request and streams the result.
+
         Supports both chat completion and text completion.
 
-        Arguments:
-            prompt {str} -- The prompt to use for the completion request.
-            settings {OpenAITextPromptExecutionSettings} -- The settings to use for the completion request.
+        Args:
+            prompt (str): The prompt to use for the completion request.
+            settings (OpenAITextPromptExecutionSettings): The settings to use for the completion request.
 
         Yields:
-            List["StreamingTextContent"] -- The result stream made up of StreamingTextContent objects.
+            List["StreamingTextContent"]: The result stream made up of StreamingTextContent objects.
         """
         if "prompt" in settings.model_fields:
             settings.prompt = prompt
         if "messages" in settings.model_fields:
             if not settings.messages:
                 settings.messages = [{"role": "user", "content": prompt}]
             else:
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,17 @@
 
 import logging
 from collections.abc import Mapping
 
 from openai import AsyncOpenAI
 from pydantic import ValidationError
 
-from semantic_kernel.connectors.ai.open_ai.services.open_ai_config_base import (
-    OpenAIConfigBase,
-)
-from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import (
-    OpenAIModelTypes,
-)
-from semantic_kernel.connectors.ai.open_ai.services.open_ai_text_embedding_base import (
-    OpenAITextEmbeddingBase,
-)
+from semantic_kernel.connectors.ai.open_ai.services.open_ai_config_base import OpenAIConfigBase
+from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import OpenAIModelTypes
+from semantic_kernel.connectors.ai.open_ai.services.open_ai_text_embedding_base import OpenAITextEmbeddingBase
 from semantic_kernel.connectors.ai.open_ai.settings.open_ai_settings import OpenAISettings
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 @experimental_class
@@ -31,29 +25,28 @@
         api_key: str | None = None,
         org_id: str | None = None,
         service_id: str | None = None,
         default_headers: Mapping[str, str] | None = None,
         async_client: AsyncOpenAI | None = None,
         env_file_path: str | None = None,
     ) -> None:
-        """
-        Initializes a new instance of the OpenAITextCompletion class.
+        """Initializes a new instance of the OpenAITextCompletion class.
 
-        Arguments:
-            ai_model_id {str} -- OpenAI model name, see
+        Args:
+            ai_model_id (str): OpenAI model name, see
                 https://platform.openai.com/docs/models
-            service_id {str | None} -- Service ID tied to the execution settings.
-            api_key {str | None} -- The optional API key to use. If provided will override,
+            service_id (str | None): Service ID tied to the execution settings.
+            api_key (str | None): The optional API key to use. If provided will override,
                 the env vars or .env file value.
-            org_id {str | None} -- The optional org ID to use. If provided will override,
+            org_id (str | None): The optional org ID to use. If provided will override,
                 the env vars or .env file value.
-            default_headers {Optional[Mapping[str,str]]}: The default headers mapping of string keys to
+            default_headers (Mapping[str,str] | None): The default headers mapping of string keys to
                 string values for HTTP requests. (Optional)
-            async_client {Optional[AsyncOpenAI]} -- An existing client to use. (Optional)
-            env_file_path {str | None} -- Use the environment settings file as
+            async_client (Optional[AsyncOpenAI]): An existing client to use. (Optional)
+            env_file_path (str | None): Use the environment settings file as
                 a fallback to environment variables. (Optional)
         """
         try:
             openai_settings = OpenAISettings.create(env_file_path=env_file_path)
         except ValidationError as e:
             logger.warning(f"Failed to load OpenAI pydantic settings: {e}")
 
@@ -73,21 +66,19 @@
             service_id=service_id,
             default_headers=default_headers,
             async_client=async_client,
         )
 
     @classmethod
     def from_dict(cls, settings: dict[str, str]) -> "OpenAITextEmbedding":
-        """
-        Initialize an Open AI service from a dictionary of settings.
+        """Initialize an Open AI service from a dictionary of settings.
 
-        Arguments:
+        Args:
             settings: A dictionary of settings for the service.
         """
-
         return OpenAITextEmbedding(
             ai_model_id=settings["ai_model_id"],
             api_key=settings.get("api_key", None),
             org_id=settings.get("org_id", None),
             service_id=settings.get("service_id"),
             default_headers=settings.get("default_headers"),
             env_file_path=settings.get("env_file_path", None),
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 # Copyright (c) Microsoft. All rights reserved.
 
+import sys
 from typing import Any
 
 from numpy import array, ndarray
 
+if sys.version_info >= (3, 12):
+    from typing import override
+else:
+    from typing_extensions import override
+
 from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import EmbeddingGeneratorBase
 from semantic_kernel.connectors.ai.open_ai.prompt_execution_settings.open_ai_prompt_execution_settings import (
     OpenAIEmbeddingPromptExecutionSettings,
 )
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import OpenAIHandler
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
 @experimental_class
 class OpenAITextEmbeddingBase(OpenAIHandler, EmbeddingGeneratorBase):
+    @override
     async def generate_embeddings(self, texts: list[str], batch_size: int | None = None, **kwargs: Any) -> ndarray:
-        """Generates embeddings for the given texts.
-
-        Arguments:
-            texts {List[str]} -- The texts to generate embeddings for.
-            batch_size {Optional[int]} -- The batch size to use for the request.
-            kwargs {Dict[str, Any]} -- Additional arguments to pass to the request,
-                see OpenAIEmbeddingPromptExecutionSettings for the details.
-
-        Returns:
-            ndarray -- The embeddings for the text.
-
-        """
         settings = OpenAIEmbeddingPromptExecutionSettings(
             ai_model_id=self.ai_model_id,
             **kwargs,
         )
         raw_embeddings = []
         batch_size = batch_size or len(texts)
         for i in range(0, len(texts), batch_size):
@@ -39,9 +34,10 @@
             settings.input = batch
             raw_embedding = await self._send_embedding_request(
                 settings=settings,
             )
             raw_embeddings.extend(raw_embedding)
         return array(raw_embeddings)
 
+    @override
     def get_prompt_execution_settings_class(self) -> PromptExecutionSettings:
         return OpenAIEmbeddingPromptExecutionSettings
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/services/utils.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/services/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/settings/azure_open_ai_settings.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/settings/azure_open_ai_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pydantic import SecretStr
 from pydantic_settings import BaseSettings
 
 from semantic_kernel.kernel_pydantic import HttpsUrl
 
 
 class AzureOpenAISettings(BaseSettings):
-    """AzureOpenAI model settings
+    """AzureOpenAI model settings.
 
     The settings are first loaded from environment variables with the prefix 'AZURE_OPENAI_'.
     If the environment variables are not found, the settings can be loaded from a .env file
     with the encoding 'utf-8'. If the settings are not found in the .env file, the settings
     are ignored; however, validation will fail alerting that the settings are missing.
 
     Optional settings for prefix 'AZURE_OPENAI_' are:
@@ -60,20 +60,23 @@
     embedding_deployment_name: str | None = None
     endpoint: HttpsUrl | None = None
     base_url: HttpsUrl | None = None
     api_key: SecretStr | None = None
     api_version: str | None = None
 
     class Config:
+        """Pydantic configuration settings."""
+
         env_prefix = "AZURE_OPENAI_"
         env_file = None
         env_file_encoding = "utf-8"
         extra = "ignore"
         case_sensitive = False
 
     @classmethod
     def create(cls, **kwargs):
+        """Create an instance of the class."""
         if "env_file_path" in kwargs and kwargs["env_file_path"]:
             cls.Config.env_file = kwargs["env_file_path"]
         else:
             cls.Config.env_file = None
         return cls(**kwargs)
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/open_ai/settings/open_ai_settings.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/open_ai/settings/open_ai_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from pydantic import SecretStr
 from pydantic_settings import BaseSettings
 
 
 class OpenAISettings(BaseSettings):
-    """OpenAI model settings
+    """OpenAI model settings.
 
     The settings are first loaded from environment variables with the prefix 'OPENAI_'. If the
     environment variables are not found, the settings can be loaded from a .env file with the
     encoding 'utf-8'. If the settings are not found in the .env file, the settings are ignored;
     however, validation will fail alerting that the settings are missing.
 
     Optional settings for prefix 'OPENAI_' are:
@@ -30,20 +30,23 @@
     org_id: str | None = None
     api_key: SecretStr | None = None
     chat_model_id: str | None = None
     text_model_id: str | None = None
     embedding_model_id: str | None = None
 
     class Config:
+        """Pydantic configuration settings."""
+
         env_prefix = "OPENAI_"
         env_file = None
         env_file_encoding = "utf-8"
         extra = "ignore"
         case_sensitive = False
 
     @classmethod
     def create(cls, **kwargs):
+        """Create an instance of the class."""
         if "env_file_path" in kwargs and kwargs["env_file_path"]:
             cls.Config.env_file = kwargs["env_file_path"]
         else:
             cls.Config.env_file = None
         return cls(**kwargs)
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/prompt_execution_settings.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/prompt_execution_settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,32 +8,38 @@
 
 
 class PromptExecutionSettings(KernelBaseModel):
     """Base class for prompt execution settings.
 
     Can be used by itself or as a base class for other prompt execution settings. The methods are used to create
     specific prompt execution settings objects based on the keys in the extension_data field, this way you can
-    create a generic PromptExecutionSettings object in your application, which get's mapped into the keys of the
+    create a generic PromptExecutionSettings object in your application, which gets mapped into the keys of the
     prompt execution settings that each services returns by using the service.get_prompt_execution_settings() method.
 
-    Parameters:
-        service_id (str): The service ID to use for the request.
-        extension_data (Dict[str, Any], optional): Any additional data to send with the request. Defaults to None.
-        kwargs (Any): Additional keyword arguments,
-            these are attempted to parse into the keys of the specific prompt execution settings.
+    Attributes:
+        service_id (str | None): The service ID to use for the request.
+        extension_data (Dict[str, Any]): Any additional data to send with the request.
+
     Methods:
         prepare_settings_dict: Prepares the settings as a dictionary for sending to the AI service.
         update_from_prompt_execution_settings: Update the keys from another prompt execution settings object.
         from_prompt_execution_settings: Create a prompt execution settings from another prompt execution settings.
     """
 
     service_id: str | None = Field(None, min_length=1)
     extension_data: dict[str, Any] = Field(default_factory=dict)
 
     def __init__(self, service_id: str | None = None, **kwargs: Any):
+        """Initialize the prompt execution settings.
+
+        Args:
+            service_id (str): The service ID to use for the request.
+            kwargs (Any): Additional keyword arguments,
+                these are attempted to parse into the keys of the specific prompt execution settings.
+        """
         extension_data = kwargs.pop("extension_data", {})
         extension_data.update(kwargs)
         super().__init__(service_id=service_id, extension_data=extension_data)
         self.unpack_extension_data()
 
     @property
     def keys(self):
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/ai/text_completion_client_base.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/ai/text_completion_client_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,35 +16,33 @@
 
     @abstractmethod
     async def get_text_contents(
         self,
         prompt: str,
         settings: "PromptExecutionSettings",
     ) -> list["TextContent"]:
-        """
-        This is the method that is called from the kernel to get a response from a text-optimized LLM.
+        """This is the method that is called from the kernel to get a response from a text-optimized LLM.
 
-        Arguments:
-            prompt {str} -- The prompt to send to the LLM.
-            settings {PromptExecutionSettings} -- Settings for the request.
+        Args:
+            prompt (str): The prompt to send to the LLM.
+            settings (PromptExecutionSettings): Settings for the request.
 
-            Returns:
-            list[TextContent] -- A string or list of strings representing the response(s) from the LLM.
+        Returns:
+            list[TextContent]: A string or list of strings representing the response(s) from the LLM.
         """
 
     @abstractmethod
     def get_streaming_text_contents(
         self,
         prompt: str,
         settings: "PromptExecutionSettings",
     ) -> AsyncGenerator[list["StreamingTextContent"], Any]:
-        """
-        This is the method that is called from the kernel to get a stream response from a text-optimized LLM.
+        """This is the method that is called from the kernel to get a stream response from a text-optimized LLM.
 
-        Arguments:
-            prompt {str} -- The prompt to send to the LLM.
-            settings {PromptExecutionSettings} -- Settings for the request.
+        Args:
+            prompt (str): The prompt to send to the LLM.
+            settings (PromptExecutionSettings): Settings for the request.
 
         Yields:
-            list[StreamingTextContent] -- A stream representing the response(s) from the LLM.
+            list[StreamingTextContent]: A stream representing the response(s) from the LLM.
         """
         ...
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/astradb/astra_client.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/astradb/astra_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright (c) Microsoft. All rights reserved.
+
 import json
 
 import aiohttp
 
 from semantic_kernel.connectors.memory.astradb.utils import AsyncSession
 from semantic_kernel.connectors.telemetry import APP_INFO
 from semantic_kernel.exceptions import ServiceResponseException
@@ -23,14 +25,15 @@
         astra_region: str,
         astra_application_token: str,
         keyspace_name: str,
         embedding_dim: int,
         similarity_function: str,
         session: aiohttp.ClientSession | None = None,
     ):
+        """Initializes a new instance of the AstraClient class."""
         self.astra_id = astra_id
         self.astra_application_token = astra_application_token
         self.astra_region = astra_region
         self.keyspace_name = keyspace_name
         self.embedding_dim = embedding_dim
         self.similarity_function = similarity_function
 
@@ -53,33 +56,36 @@
                         raise ServiceResponseException(f"Astra DB request error - {response_dict['errors']}")
                     else:
                         return response_dict
                 else:
                     raise ServiceResponseException(f"Astra DB not available. Status : {response}")
 
     async def find_collections(self, include_detail: bool = True):
+        """Finds all collections in the keyspace."""
         query = {"findCollections": {"options": {"explain": include_detail}}}
         result = await self._run_query(self.request_base_url, query)
         return result["status"]["collections"]
 
     async def find_collection(self, collection_name: str):
+        """Finds a collection in the keyspace."""
         collections = await self.find_collections(False)
         found = False
         for collection in collections:
             if collection == collection_name:
                 found = True
                 break
         return found
 
     async def create_collection(
         self,
         collection_name: str,
         embedding_dim: int | None = None,
         similarity_function: str | None = None,
     ):
+        """Creates a new collection in the keyspace."""
         query = {
             "createCollection": {
                 "name": collection_name,
                 "options": {
                     "vector": {
                         "dimension": embedding_dim if embedding_dim is not None else self.embedding_dim,
                         "metric": similarity_function if similarity_function is not None else self.similarity_function,
@@ -87,14 +93,15 @@
                 },
             }
         }
         result = await self._run_query(self.request_base_url, query)
         return True if result["status"]["ok"] == 1 else False
 
     async def delete_collection(self, collection_name: str):
+        """Deletes a collection from the keyspace."""
         query = {"deleteCollection": {"name": collection_name}}
         result = await self._run_query(self.request_base_url, query)
         return True if result["status"]["ok"] == 1 else False
 
     def _build_request_collection_url(self, collection_name: str):
         return f"{self.request_base_url}/{collection_name}"
 
@@ -103,24 +110,27 @@
         collection_name: str,
         filter: dict | None = None,
         vector: list[float] | None = None,
         limit: int | None = None,
         include_vector: bool | None = None,
         include_similarity: bool | None = None,
     ) -> list[dict]:
+        """Finds all documents in the collection."""
         find_query = {}
 
         if filter is not None:
             find_query["filter"] = filter
 
         if vector is not None:
             find_query["sort"] = {"$vector": vector}
 
         if include_vector is not None and include_vector is False:
             find_query["projection"] = {"$vector": 0}
+        else:
+            find_query["projection"] = {"*": 1}
 
         if limit is not None:
             find_query["options"] = {"limit": limit}
 
         if include_similarity is not None:
             if "options" in find_query:
                 find_query["options"]["includeSimilarity"] = int(include_similarity)
@@ -128,41 +138,46 @@
                 find_query["options"] = {"includeSimilarity": int(include_similarity)}
 
         query = {"find": find_query}
         result = await self._run_query(self._build_request_collection_url(collection_name), query)
         return result["data"]["documents"]
 
     async def insert_document(self, collection_name: str, document: dict) -> str:
+        """Inserts a document into the collection."""
         query = {"insertOne": {"document": document}}
         result = await self._run_query(self._build_request_collection_url(collection_name), query)
         return result["status"]["insertedIds"][0]
 
     async def insert_documents(self, collection_name: str, documents: list[dict]) -> list[str]:
+        """Inserts multiple documents into the collection."""
         query = {"insertMany": {"documents": documents}}
         result = await self._run_query(self._build_request_collection_url(collection_name), query)
         return result["status"]["insertedIds"]
 
     async def update_document(self, collection_name: str, filter: dict, update: dict, upsert: bool = True) -> dict:
+        """Updates a document in the collection."""
         query = {
             "findOneAndUpdate": {
                 "filter": filter,
                 "update": update,
                 "options": {"returnDocument": "after", "upsert": upsert},
             }
         }
         result = await self._run_query(self._build_request_collection_url(collection_name), query)
         return result["status"]
 
     async def update_documents(self, collection_name: str, filter: dict, update: dict):
+        """Updates multiple documents in the collection."""
         query = {
             "updateMany": {
                 "filter": filter,
                 "update": update,
             }
         }
         result = await self._run_query(self._build_request_collection_url(collection_name), query)
         return result["status"]
 
     async def delete_documents(self, collection_name: str, filter: dict) -> int:
+        """Deletes documents from the collection."""
         query = {"deleteMany": {"filter": filter}}
         result = await self._run_query(self._build_request_collection_url(collection_name), query)
         return result["status"]["deletedCount"]
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import asyncio
 import logging
+import sys
 
 import aiohttp
 from numpy import ndarray
 from pydantic import ValidationError
 
+if sys.version_info >= (3, 12):
+    pass
+else:
+    pass
+
 from semantic_kernel.connectors.memory.astradb.astra_client import AstraClient
 from semantic_kernel.connectors.memory.astradb.astradb_settings import AstraDBSettings
-from semantic_kernel.connectors.memory.astradb.utils import (
-    build_payload,
-    parse_payload,
-)
+from semantic_kernel.connectors.memory.astradb.utils import build_payload, parse_payload
 from semantic_kernel.exceptions import MemoryConnectorInitializationError
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
 MAX_DIMENSIONALITY = 20000
 MAX_UPSERT_BATCH_SIZE = 100
@@ -41,46 +44,50 @@
         embedding_dim: int,
         similarity: str,
         session: aiohttp.ClientSession | None = None,
         env_file_path: str | None = None,
     ) -> None:
         """Initializes a new instance of the AstraDBMemoryStore class.
 
-        Arguments:
-            astra_application_token {str} -- The Astra application token.
-            astra_id {str} -- The Astra id of database.
-            astra_region {str} -- The Astra region
-            keyspace_name {str} -- The Astra keyspace
-            embedding_dim {int} -- The dimensionality to use for new collections.
-            similarity {str} -- TODO
-            session -- Optional session parameter
-            env_file_path {str | None} -- Use the environment settings file as a
+        Args:
+            astra_application_token (str): The Astra application token.
+            astra_id (str): The Astra id of database.
+            astra_region (str): The Astra region
+            keyspace_name (str): The Astra keyspace
+            embedding_dim (int): The dimensionality to use for new collections.
+            similarity (str): TODO
+            session: Optional session parameter
+            env_file_path (str | None): Use the environment settings file as a
                 fallback to environment variables. (Optional)
         """
         astradb_settings = None
         try:
             astradb_settings = AstraDBSettings.create(env_file_path=env_file_path)
         except ValidationError as e:
             logger.warning(f"Failed to load AstraDB pydantic settings: {e}")
 
         # Load the settings and validate
         astra_application_token = astra_application_token or (
             astradb_settings.app_token.get_secret_value() if astradb_settings and astradb_settings.app_token else None
         )
-        assert astra_application_token is not None, "The astra_application_token cannot be None."
+        if astra_application_token is None:
+            raise ValueError("The astra_application_token cannot be None.")
         astra_id = astra_id or (astradb_settings.db_id if astradb_settings and astradb_settings.db_id else None)
-        assert astra_id is not None, "The astra_id cannot be None."
+        if astra_id is None:
+            raise ValueError("The astra_id cannot be None.")
         astra_region = astra_region or (
             astradb_settings.region if astradb_settings and astradb_settings.region else None
         )
-        assert astra_region is not None, "The astra_region cannot be None."
+        if astra_region is None:
+            raise ValueError("The astra_region cannot be None.")
         keyspace_name = keyspace_name or (
             astradb_settings.keyspace if astradb_settings and astradb_settings.keyspace else None
         )
-        assert keyspace_name is not None, "The keyspace_name cannot be None."
+        if keyspace_name is None:
+            raise ValueError("The keyspace_name cannot be None.")
 
         self._embedding_dim = embedding_dim
         self._similarity = similarity
         self._session = session
 
         if self._embedding_dim > MAX_DIMENSIONALITY:
             raise MemoryConnectorInitializationError(
@@ -98,31 +105,32 @@
             session=self._session,
         )
 
     async def get_collections(self) -> list[str]:
         """Gets the list of collections.
 
         Returns:
-            List[str] -- The list of collections.
+            List[str]: The list of collections.
         """
         return await self._client.find_collections(False)
 
     async def create_collection(
         self,
         collection_name: str,
         dimension_num: int | None = None,
         distance_type: str | None = "cosine",
     ) -> None:
         """Creates a new collection in Astra if it does not exist.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to create.
-            dimension_num {int} -- The dimension of the vectors to be stored in this collection.
-            distance_type {str} -- Specifies the similarity metric to be used when querying or comparing vectors within
+        Args:
+            collection_name (str): The name of the collection to create.
+            dimension_num (int): The dimension of the vectors to be stored in this collection.
+            distance_type (str): Specifies the similarity metric to be used when querying or comparing vectors within
             this collection. The available options are dot_product, euclidean, and cosine.
+
         Returns:
             None
         """
         dimension_num = dimension_num if dimension_num is not None else self._embedding_dim
         distance_type = distance_type if distance_type is not None else self._similarity
 
         if dimension_num > MAX_DIMENSIONALITY:
@@ -133,79 +141,83 @@
         result = await self._client.create_collection(collection_name, dimension_num, distance_type)
         if result is True:
             logger.info(f"Collection {collection_name} created.")
 
     async def delete_collection(self, collection_name: str) -> None:
         """Deletes a collection.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to delete.
+        Args:
+            collection_name (str): The name of the collection to delete.
 
         Returns:
             None
         """
         result = await self._client.delete_collection(collection_name)
         logger.log(
             logging.INFO if result is True else logging.WARNING,
             f"Collection {collection_name} {'deleted.' if result is True else 'does not exist.'}",
         )
 
     async def does_collection_exist(self, collection_name: str) -> bool:
         """Checks if a collection exists.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to check.
+        Args:
+            collection_name (str): The name of the collection to check.
 
         Returns:
-            bool -- True if the collection exists; otherwise, False.
+            bool: True if the collection exists; otherwise, False.
         """
         return await self._client.find_collection(collection_name)
 
     async def upsert(self, collection_name: str, record: MemoryRecord) -> str:
-        """Upserts a memory record into the data store. Does not guarantee that the collection exists.
-            If the record already exists, it will be updated.
-            If the record does not exist, it will be created.
+        """Upsert a memory record into the data store.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
-            record {MemoryRecord} -- The memory record to upsert.
+        Does not guarantee that the collection exists.
+        If the record already exists, it will be updated.
+        If the record does not exist, it will be created.
+
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
+            record (MemoryRecord): The memory record to upsert.
 
         Returns:
-            str -- The unique identifier for the memory record.
+            str: The unique identifier for the memory record.
         """
         filter = {"_id": record._id}
         update = {"$set": build_payload(record)}
         status = await self._client.update_document(collection_name, filter, update, True)
 
         return status["upsertedId"] if "upsertedId" in status else record._id
 
     async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
-        """Upserts a batch of memory records into the data store. Does not guarantee that the collection exists.
-            If the record already exists, it will be updated.
-            If the record does not exist, it will be created.
+        """Upsert a batch of memory records into the data store.
+
+        Does not guarantee that the collection exists.
+        If the record already exists, it will be updated.
+        If the record does not exist, it will be created.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
-            records {List[MemoryRecord]} -- The memory records to upsert.
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
+            records (List[MemoryRecord]): The memory records to upsert.
 
         Returns:
-            List[str] -- The unique identifiers for the memory record.
+            List[str]: The unique identifiers for the memory record.
         """
         return await asyncio.gather(*[self.upsert(collection_name, record) for record in records])
 
     async def get(self, collection_name: str, key: str, with_embedding: bool = False) -> MemoryRecord:
         """Gets a record. Does not guarantee that the collection exists.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to get the record from.
-            key {str} -- The unique database key of the record.
-            with_embedding {bool} -- Whether to include the embedding in the result. (default: {False})
+        Args:
+            collection_name (str): The name of the collection to get the record from.
+            key (str): The unique database key of the record.
+            with_embedding (bool): Whether to include the embedding in the result. (default: {False})
 
         Returns:
-            MemoryRecord -- The record.
+            MemoryRecord: The record.
         """
         filter = {"_id": key}
         documents = await self._client.find_documents(
             collection_name=collection_name,
             filter=filter,
             include_vector=with_embedding,
         )
@@ -216,50 +228,49 @@
         return parse_payload(documents[0])
 
     async def get_batch(
         self, collection_name: str, keys: list[str], with_embeddings: bool = False
     ) -> list[MemoryRecord]:
         """Gets a batch of records. Does not guarantee that the collection exists.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to get the records from.
-            keys {List[str]} -- The unique database keys of the records.
-            with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
+        Args:
+            collection_name (str): The name of the collection to get the records from.
+            keys (List[str]): The unique database keys of the records.
+            with_embeddings (bool): Whether to include the embeddings in the results. (default: {False})
 
         Returns:
-            List[MemoryRecord] -- The records.
+            List[MemoryRecord]: The records.
         """
-
         filter = {"_id": {"$in": keys}}
         documents = await self._client.find_documents(
             collection_name=collection_name,
             filter=filter,
             include_vector=with_embeddings,
         )
         return [parse_payload(document) for document in documents]
 
     async def remove(self, collection_name: str, key: str) -> None:
         """Removes a memory record from the data store. Does not guarantee that the collection exists.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to remove the record from.
-            key {str} -- The unique id associated with the memory record to remove.
+        Args:
+            collection_name (str): The name of the collection to remove the record from.
+            key (str): The unique id associated with the memory record to remove.
 
         Returns:
             None
         """
         filter = {"_id": key}
         await self._client.delete_documents(collection_name, filter)
 
     async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         """Removes a batch of records. Does not guarantee that the collection exists.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to remove the records from.
-            keys {List[str]} -- The unique ids associated with the memory records to remove.
+        Args:
+            collection_name (str): The name of the collection to remove the records from.
+            keys (List[str]): The unique ids associated with the memory records to remove.
 
         Returns:
             None
         """
         filter = {"_id": {"$in": keys}}
         await self._client.delete_documents(collection_name, filter)
 
@@ -267,22 +278,23 @@
         self,
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float = 0.0,
         with_embedding: bool = False,
     ) -> tuple[MemoryRecord, float]:
         """Gets the nearest match to an embedding using cosine similarity.
-        Arguments:
-            collection_name {str} -- The name of the collection to get the nearest matches from.
-            embedding {ndarray} -- The embedding to find the nearest matches to.
-            min_relevance_score {float} -- The minimum relevance score of the matches. (default: {0.0})
-            with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
+
+        Args:
+            collection_name (str): The name of the collection to get the nearest matches from.
+            embedding (ndarray): The embedding to find the nearest matches to.
+            min_relevance_score (float): The minimum relevance score of the matches. (default: {0.0})
+            with_embedding (bool): Whether to include the embeddings in the results. (default: {False})
 
         Returns:
-            Tuple[MemoryRecord, float] -- The record and the relevance score.
+            Tuple[MemoryRecord, float]: The record and the relevance score.
         """
         matches = await self.get_nearest_matches(
             collection_name=collection_name,
             embedding=embedding,
             limit=1,
             min_relevance_score=min_relevance_score,
             with_embeddings=with_embedding,
@@ -294,23 +306,24 @@
         collection_name: str,
         embedding: ndarray,
         limit: int,
         min_relevance_score: float = 0.0,
         with_embeddings: bool = False,
     ) -> list[tuple[MemoryRecord, float]]:
         """Gets the nearest matches to an embedding using cosine similarity.
-        Arguments:
-            collection_name {str} -- The name of the collection to get the nearest matches from.
-            embedding {ndarray} -- The embedding to find the nearest matches to.
-            limit {int} -- The maximum number of matches to return.
-            min_relevance_score {float} -- The minimum relevance score of the matches. (default: {0.0})
-            with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
+
+        Args:
+            collection_name (str): The name of the collection to get the nearest matches from.
+            embedding (ndarray): The embedding to find the nearest matches to.
+            limit (int): The maximum number of matches to return.
+            min_relevance_score (float): The minimum relevance score of the matches. (default: {0.0})
+            with_embeddings (bool): Whether to include the embeddings in the results. (default: {False})
 
         Returns:
-            List[Tuple[MemoryRecord, float]] -- The records and their relevance scores.
+            List[Tuple[MemoryRecord, float]]: The records and their relevance scores.
         """
         matches = await self._client.find_documents(
             collection_name=collection_name,
             vector=embedding.tolist(),
             limit=limit,
             include_similarity=True,
             include_vector=with_embeddings,
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/astradb/astradb_settings.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/astradb/astradb_settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from semantic_kernel.connectors.memory.memory_settings_base import BaseModelSettings
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
 @experimental_class
 class AstraDBSettings(BaseModelSettings):
-    """AstraDB model settings
+    """AstraDB model settings.
 
     Optional:
     - app_token: SecretStr | None - AstraDB token
         (Env var ASTRADB_APP_TOKEN)
     - db_id: str | None - AstraDB database ID
         (Env var ASTRADB_DB_ID)
     - region: str | None - AstraDB region
@@ -23,8 +23,10 @@
 
     app_token: SecretStr
     db_id: str
     region: str
     keyspace: str
 
     class Config(BaseModelSettings.Config):
+        """Pydantic configuration settings."""
+
         env_prefix = "ASTRADB_"
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/astradb/utils.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/astradb/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,42 +5,41 @@
 import numpy
 
 from semantic_kernel.memory.memory_record import MemoryRecord
 
 
 class AsyncSession:
     def __init__(self, session: aiohttp.ClientSession = None):
+        """Initializes a new instance of the AsyncSession class."""
         self._session = session if session else aiohttp.ClientSession()
 
     async def __aenter__(self):
+        """Enter the session."""
         return await self._session.__aenter__()
 
     async def __aexit__(self, *args, **kwargs):
+        """Close the session."""
         await self._session.close()
 
 
 def build_payload(record: MemoryRecord) -> dict[str, Any]:
-    """
-    Builds a metadata payload to be sent to AstraDb from a MemoryRecord.
-    """
+    """Builds a metadata payload to be sent to AstraDb from a MemoryRecord."""
     payload: dict[str, Any] = {}
     payload["$vector"] = record.embedding.tolist()
     if record._text:
         payload["text"] = record._text
     if record._description:
         payload["description"] = record._description
     if record._additional_metadata:
         payload["additional_metadata"] = record._additional_metadata
     return payload
 
 
 def parse_payload(document: dict[str, Any]) -> MemoryRecord:
-    """
-    Parses a record from AstraDb into a MemoryRecord.
-    """
+    """Parses a record from AstraDb into a MemoryRecord."""
     text = document.get("text", None)
     description = document["description"] if "description" in document else None
     additional_metadata = document["additional_metadata"] if "additional_metadata" in document else None
 
     return MemoryRecord.local_record(
         id=document["_id"],
         description=description,
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cognitive_search/azure_ai_search_settings.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/azure_cognitive_search/azure_ai_search_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 from semantic_kernel.connectors.memory.memory_settings_base import BaseModelSettings
 from semantic_kernel.kernel_pydantic import HttpsUrl
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
 @experimental_class
 class AzureAISearchSettings(BaseModelSettings):
-    """Azure AI Search model settings currently used by the AzureCognitiveSearchMemoryStore connector
+    """Azure AI Search model settings currently used by the AzureCognitiveSearchMemoryStore connector.
 
-    Optional:
+    Args:
     - api_key: SecretStr - Azure AI Search API key (Env var AZURE_AI_SEARCH_API_KEY)
     - endpoint: HttpsUrl - Azure AI Search endpoint (Env var AZURE_AI_SEARCH_ENDPOINT)
     - index_name: str - Azure AI Search index name (Env var AZURE_AI_SEARCH_INDEX_NAME)
     """
 
     api_key: SecretStr | None = None
     endpoint: HttpsUrl | None = None
     index_name: str | None = None
 
     class Config(BaseModelSettings.Config):
+        """Pydantic configuration settings."""
+
         env_prefix = "AZURE_AI_SEARCH_"
 
     def model_dump(self):
-        """
-        Custom method to dump model data in the required format.
-        """
+        """Custom method to dump model data in the required format."""
         return {
             "api_key": self.api_key.get_secret_value() if self.api_key else None,
             "endpoint": str(self.endpoint),
             "index_name": self.index_name,
         }
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,433 +1,402 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-import uuid
-from inspect import isawaitable
+from typing import NamedTuple
 
-from azure.core.credentials import AzureKeyCredential, TokenCredential
-from azure.core.exceptions import ResourceNotFoundError
-from azure.search.documents.indexes.aio import SearchIndexClient
-from azure.search.documents.indexes.models import (
-    HnswAlgorithmConfiguration,
-    HnswParameters,
-    SearchIndex,
-    SearchResourceEncryptionKey,
-    VectorSearch,
-    VectorSearchProfile,
-)
-from azure.search.documents.models import VectorizedQuery
 from numpy import ndarray
+from pinecone import FetchResponse, IndexDescription, IndexList, Pinecone, ServerlessSpec
 from pydantic import ValidationError
 
-from semantic_kernel.connectors.memory.azure_cognitive_search.utils import (
-    SEARCH_FIELD_EMBEDDING,
-    SEARCH_FIELD_ID,
-    dict_to_memory_record,
-    encode_id,
-    get_field_selection,
-    get_index_schema,
-    get_search_index_async_client,
-    memory_record_to_search_record,
+from semantic_kernel.connectors.memory.pinecone.pinecone_settings import PineconeSettings
+from semantic_kernel.connectors.memory.pinecone.utils import build_payload, parse_payload
+from semantic_kernel.exceptions import (
+    ServiceInitializationError,
+    ServiceInvalidRequestError,
+    ServiceResourceNotFoundError,
+    ServiceResponseException,
 )
-from semantic_kernel.exceptions import MemoryConnectorInitializationError, MemoryConnectorResourceNotFound
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
+# Limitations set by Pinecone at https://docs.pinecone.io/reference/known-limitations
+MAX_DIMENSIONALITY = 20000
+MAX_UPSERT_BATCH_SIZE = 100
+MAX_QUERY_WITHOUT_METADATA_BATCH_SIZE = 10000
+MAX_QUERY_WITH_METADATA_BATCH_SIZE = 1000
+MAX_FETCH_BATCH_SIZE = 1000
+MAX_DELETE_BATCH_SIZE = 1000
+
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 @experimental_class
-class AzureCognitiveSearchMemoryStore(MemoryStoreBase):
-    _search_index_client: SearchIndexClient = None
-    _vector_size: int = None
+class PineconeMemoryStore(MemoryStoreBase):
+    """A memory store that uses Pinecone as the backend."""
+
+    _pinecone_api_key: str
+    _default_dimensionality: int
+
+    DEFAULT_INDEX_SPEC: ServerlessSpec = ServerlessSpec(
+        cloud="aws",
+        region="us-east-1",
+    )
 
     def __init__(
         self,
-        vector_size: int,
-        search_endpoint: str | None = None,
-        admin_key: str | None = None,
-        azure_credentials: AzureKeyCredential | None = None,
-        token_credentials: TokenCredential | None = None,
+        api_key: str,
+        default_dimensionality: int,
         env_file_path: str | None = None,
     ) -> None:
-        """Initializes a new instance of the AzureCognitiveSearchMemoryStore class.
+        """Initializes a new instance of the PineconeMemoryStore class.
 
-        Arguments:
-            vector_size {int}                                -- Embedding vector size.
-            search_endpoint {str | None}                  -- The endpoint of the Azure Cognitive Search service
-                                                                (default: {None}).
-            admin_key {str | None}                        -- Azure Cognitive Search API key (default: {None}).
-            azure_credentials {AzureKeyCredential | None} -- Azure Cognitive Search credentials (default: {None}).
-            token_credentials {TokenCredential | None}    -- Azure Cognitive Search token credentials
-                                                                (default: {None}).
-            env_file_path {str | None}                  -- Use the environment settings file as a fallback
-                                                                to environment variables
-
-        Instantiate using Async Context Manager:
-            async with AzureCognitiveSearchMemoryStore(<...>) as memory:
-                await memory.<...>
-        """
-        from semantic_kernel.connectors.memory.azure_cognitive_search import AzureAISearchSettings
+        Args:
+            api_key (str): The Pinecone API key.
+            default_dimensionality (int): The default dimensionality to use for new collections.
+            env_file_path (str | None): Use the environment settings file as a fallback
+                to environment variables. (Optional)
+        """
+        if default_dimensionality > MAX_DIMENSIONALITY:
+            raise ServiceInitializationError(
+                f"Dimensionality of {default_dimensionality} exceeds "
+                + f"the maximum allowed value of {MAX_DIMENSIONALITY}."
+            )
 
-        acs_memory_settings = None
+        pinecone_settings = None
         try:
-            acs_memory_settings = AzureAISearchSettings.create(env_file_path=env_file_path)
+            pinecone_settings = PineconeSettings.create(env_file_path=env_file_path)
         except ValidationError as e:
-            logger.warning(f"Failed to load AzureAISearch pydantic settings: {e}")
+            logger.warning(f"Failed to load the Pinecone pydantic settings: {e}")
 
-        admin_key = admin_key or (
-            acs_memory_settings.api_key.get_secret_value()
-            if acs_memory_settings and acs_memory_settings.api_key
-            else None
+        api_key = api_key or (
+            pinecone_settings.api_key.get_secret_value() if pinecone_settings and pinecone_settings.api_key else None
         )
-        assert admin_key, "The ACS admin_key is required to connect to Azure Cognitive Search."
-        search_endpoint = search_endpoint or (
-            acs_memory_settings.endpoint if acs_memory_settings and acs_memory_settings.endpoint else None
-        )
-        assert search_endpoint, "The ACS endpoint is required to connect to Azure Cognitive Search."
+        if not api_key:
+            raise ValueError("The Pinecone api_key cannot be None.")
 
-        self._vector_size = vector_size
-        self._search_index_client = get_search_index_async_client(
-            str(search_endpoint), admin_key, azure_credentials, token_credentials
-        )
+        self._pinecone_api_key = api_key
+        self._default_dimensionality = default_dimensionality
 
-    async def close(self):
-        """Async close connection, invoked by MemoryStoreBase.__aexit__()"""
-        if self._search_index_client is not None:
-            await self._search_index_client.close()
+        self.pinecone = Pinecone(api_key=self._pinecone_api_key)
+        self.collection_names_cache = set()
 
     async def create_collection(
         self,
         collection_name: str,
-        vector_config: HnswAlgorithmConfiguration | None = None,
-        search_resource_encryption_key: SearchResourceEncryptionKey | None = None,
+        dimension_num: int | None = None,
+        distance_type: str | None = "cosine",
+        index_spec: NamedTuple = DEFAULT_INDEX_SPEC,
     ) -> None:
-        """Creates a new collection if it does not exist.
+        """Creates a new collection in Pinecone if it does not exist.
 
-        Arguments:
-            collection_name {str}                              -- The name of the collection to create.
-            vector_config {HnswVectorSearchAlgorithmConfiguration} -- Optional search algorithm configuration
-                                                                      (default: {None}).
-            semantic_config {SemanticConfiguration}            -- Optional search index configuration (default: {None}).
-            search_resource_encryption_key {SearchResourceEncryptionKey}            -- Optional Search Encryption Key
-                                                                                       (default: {None}).
+        This function creates an index, by default the following index
+        settings are used: metric = cosine, cloud = aws, region = us-east-1.
 
-        Returns:
-            None
-        """
-
-        vector_search_profile_name = "az-vector-config"
-        if vector_config:
-            vector_search_profile = VectorSearchProfile(
-                name=vector_search_profile_name, algorithm_configuration_name=vector_config.name
+        Args:
+            collection_name (str): The name of the collection to create.
+                In Pinecone, a collection is represented as an index. The concept
+                of "collection" in Pinecone is just a static copy of an index.
+            dimension_num (int, optional): The dimensionality of the embeddings.
+            distance_type (str, optional): The distance metric to use for the index.
+                (default: {"cosine"})
+            index_spec (NamedTuple, optional): The index spec to use for the index.
+        """
+        if dimension_num is None:
+            dimension_num = self._default_dimensionality
+        if dimension_num > MAX_DIMENSIONALITY:
+            raise ServiceInitializationError(
+                f"Dimensionality of {dimension_num} exceeds " + f"the maximum allowed value of {MAX_DIMENSIONALITY}."
             )
-            vector_search = VectorSearch(profiles=[vector_search_profile], algorithms=[vector_config])
-        else:
-            vector_search_algorithm_name = "az-vector-hnsw-config"
-            vector_search_profile = VectorSearchProfile(
-                name=vector_search_profile_name, algorithm_configuration_name=vector_search_algorithm_name
-            )
-            vector_search = VectorSearch(
-                profiles=[vector_search_profile],
-                algorithms=[
-                    HnswAlgorithmConfiguration(
-                        name=vector_search_algorithm_name,
-                        kind="hnsw",
-                        parameters=HnswParameters(
-                            m=4,  # Number of bi-directional links, typically between 4 and 10
-                            ef_construction=400,  # Size during indexing, range: 100-1000
-                            ef_search=500,  # Size during search, range: 100-1000
-                            metric="cosine",  # Can be "cosine", "dotProduct", or "euclidean"
-                        ),
-                    )
-                ],
-            )
-
-        if not self._search_index_client:
-            raise MemoryConnectorInitializationError("Error: self._search_index_client not set 1.")
 
-        # Check to see if collection exists
-        collection_index = None
-        try:
-            collection_index = await self._search_index_client.get_index(collection_name.lower())
-        except ResourceNotFoundError:
-            pass
-
-        if not collection_index:
-            # Create the search index with the semantic settings
-            index = SearchIndex(
-                name=collection_name.lower(),
-                fields=get_index_schema(self._vector_size, vector_search_profile_name),
-                vector_search=vector_search,
-                encryption_key=search_resource_encryption_key,
+        if not await self.does_collection_exist(collection_name):
+            self.pinecone.create_index(
+                name=collection_name, dimension=dimension_num, metric=distance_type, spec=index_spec
             )
+            self.collection_names_cache.add(collection_name)
 
-            await self._search_index_client.create_index(index)
+    async def describe_collection(self, collection_name: str) -> IndexDescription | None:
+        """Gets the description of the index.
 
-    async def get_collections(self) -> list[str]:
-        """Gets the list of collections.
+        Args:
+            collection_name (str): The name of the index to get.
 
         Returns:
-            List[str] -- The list of collections.
+            Optional[dict]: The index.
         """
+        if await self.does_collection_exist(collection_name):
+            return self.pinecone.describe_index(collection_name)
+        return None
 
-        results_list = []
-        items = self._search_index_client.list_index_names()
-        if isawaitable(items):
-            items = await items
-
-        async for result in items:
-            results_list.append(result)
+    async def get_collections(
+        self,
+    ) -> IndexList:
+        """Gets the list of collections.
 
-        return results_list
+        Returns:
+            IndexList: The list of collections.
+        """
+        return self.pinecone.list_indexes()
 
     async def delete_collection(self, collection_name: str) -> None:
         """Deletes a collection.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to delete.
+        Args:
+            collection_name (str): The name of the collection to delete.
 
         Returns:
             None
         """
-        await self._search_index_client.delete_index(index=collection_name.lower())
+        if await self.does_collection_exist(collection_name):
+            self.pinecone.delete_index(collection_name)
+            self.collection_names_cache.discard(collection_name)
 
     async def does_collection_exist(self, collection_name: str) -> bool:
         """Checks if a collection exists.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to check.
+        Args:
+            collection_name (str): The name of the collection to check.
 
         Returns:
-            bool -- True if the collection exists; otherwise, False.
+            bool: True if the collection exists; otherwise, False.
         """
+        if collection_name in self.collection_names_cache:
+            return True
 
-        try:
-            collection_result = await self._search_index_client.get_index(name=collection_name.lower())
+        index_collection_names = self.pinecone.list_indexes().names()
+        self.collection_names_cache |= set(index_collection_names)
 
-            if collection_result:
-                return True
-            else:
-                return False
-        except ResourceNotFoundError:
-            return False
+        return collection_name in index_collection_names
 
     async def upsert(self, collection_name: str, record: MemoryRecord) -> str:
         """Upsert a record.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to upsert the record into.
-            record {MemoryRecord} -- The record to upsert.
+        Args:
+            collection_name (str): The name of the collection to upsert the record into.
+            record (MemoryRecord): The record to upsert.
 
         Returns:
-            str -- The unique record id of the record.
+            str: The unique database key of the record. In Pinecone, this is the record ID.
         """
+        if not await self.does_collection_exist(collection_name):
+            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
-        result = await self.upsert_batch(collection_name, [record])
-        if result:
-            return result[0]
-        return None
+        collection = self.pinecone.Index(collection_name)
+
+        upsert_response = collection.upsert(
+            vectors=[(record._id, record.embedding.tolist(), build_payload(record))],
+            namespace="",
+        )
+
+        if upsert_response.upserted_count is None:
+            raise ServiceResponseException(f"Error upserting record: {upsert_response.message}")
+
+        return record._id
 
     async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
         """Upsert a batch of records.
 
-        Arguments:
-            collection_name {str}        -- The name of the collection to upsert the records into.
-            records {List[MemoryRecord]} -- The records to upsert.
+        Args:
+            collection_name (str): The name of the collection to upsert the records into.
+            records (List[MemoryRecord]): The records to upsert.
 
         Returns:
-            List[str] -- The unique database keys of the records.
+            List[str]: The unique database keys of the records.
         """
+        if not await self.does_collection_exist(collection_name):
+            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
-        # Initialize search client here
-        # Look up Search client class to see if exists or create
-        search_client = self._search_index_client.get_search_client(collection_name.lower())
-
-        search_records = []
-        search_ids = []
+        collection = self.pinecone.Index(collection_name)
 
-        for record in records:
-            # Note:
-            # * Document id     = user provided value
-            # * MemoryRecord.id = base64(Document id)
-            if not record._id:
-                record._id = str(uuid.uuid4())
-
-            search_record = memory_record_to_search_record(record)
-            search_records.append(search_record)
-            search_ids.append(record._id)
+        vectors = [
+            (
+                record._id,
+                record.embedding.tolist(),
+                build_payload(record),
+            )
+            for record in records
+        ]
 
-        result = await search_client.upload_documents(documents=search_records)
-        await search_client.close()
+        upsert_response = collection.upsert(vectors, namespace="", batch_size=MAX_UPSERT_BATCH_SIZE)
 
-        if result[0].succeeded:
-            return search_ids
+        if upsert_response.upserted_count is None:
+            raise ServiceResponseException(f"Error upserting record: {upsert_response.message}")
         else:
-            return None
+            return [record._id for record in records]
 
     async def get(self, collection_name: str, key: str, with_embedding: bool = False) -> MemoryRecord:
         """Gets a record.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to get the record from.
-            key {str}             -- The unique database key of the record.
-            with_embedding {bool} -- Whether to include the embedding in the result. (default: {False})
+        Args:
+            collection_name (str): The name of the collection to get the record from.
+            key (str): The unique database key of the record.
+            with_embedding (bool): Whether to include the embedding in the result. (default: {False})
 
         Returns:
-            MemoryRecord -- The record.
+            MemoryRecord: The record.
         """
+        if not await self.does_collection_exist(collection_name):
+            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
-        # Look up Search client class to see if exists or create
-        search_client = self._search_index_client.get_search_client(collection_name.lower())
-
-        try:
-            search_result = await search_client.get_document(
-                key=encode_id(key), selected_fields=get_field_selection(with_embedding)
-            )
-        except ResourceNotFoundError as exc:
-            await search_client.close()
-            raise MemoryConnectorResourceNotFound("Memory record not found") from exc
+        collection = self.pinecone.Index(collection_name)
+        fetch_response = collection.fetch([key])
 
-        await search_client.close()
+        if len(fetch_response.vectors) == 0:
+            raise ServiceResourceNotFoundError(f"Record with key '{key}' does not exist")
 
-        # Create Memory record from document
-        return dict_to_memory_record(search_result, with_embedding)
+        return parse_payload(fetch_response.vectors[key], with_embedding)
 
     async def get_batch(
         self, collection_name: str, keys: list[str], with_embeddings: bool = False
     ) -> list[MemoryRecord]:
         """Gets a batch of records.
 
-        Arguments:
-            collection_name {str}  -- The name of the collection to get the records from.
-            keys {List[str]}       -- The unique database keys of the records.
-            with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
+        Args:
+            collection_name (str): The name of the collection to get the records from.
+            keys (List[str]): The unique database keys of the records.
+            with_embeddings (bool): Whether to include the embeddings in the results. (default: {False})
 
         Returns:
-            List[MemoryRecord] -- The records.
+            List[MemoryRecord]: The records.
         """
+        if not await self.does_collection_exist(collection_name):
+            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
-        search_results = []
-
-        for key in keys:
-            search_result = await self.get(
-                collection_name=collection_name.lower(),
-                key=key,
-                with_embedding=with_embeddings,
-            )
-            search_results.append(search_result)
-
-        return search_results
+        fetch_response = await self.__get_batch(collection_name, keys, with_embeddings)
+        return [parse_payload(fetch_response.vectors[key], with_embeddings) for key in fetch_response.vectors.keys()]
 
-    async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
-        """Removes a batch of records.
+    async def remove(self, collection_name: str, key: str) -> None:
+        """Removes a record.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to remove the records from.
-            keys {List[str]}      -- The unique database keys of the records to remove.
+        Args:
+            collection_name (str): The name of the collection to remove the record from.
+            key (str): The unique database key of the record to remove.
 
         Returns:
             None
         """
+        if not await self.does_collection_exist(collection_name):
+            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
-        for record_id in keys:
-            await self.remove(collection_name=collection_name.lower(), key=encode_id(record_id))
+        collection = self.pinecone.Index(collection_name)
+        collection.delete([key])
 
-    async def remove(self, collection_name: str, key: str) -> None:
-        """Removes a record.
+    async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
+        """Removes a batch of records.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to remove the record from.
-            key {str}             -- The unique database key of the record to remove.
+        Args:
+            collection_name (str): The name of the collection to remove the records from.
+            keys (List[str]): The unique database keys of the records to remove.
 
         Returns:
             None
         """
+        if not await self.does_collection_exist(collection_name):
+            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
-        # Look up Search client class to see if exists or create
-        search_client = self._search_index_client.get_search_client(collection_name.lower())
-        docs_to_delete = {SEARCH_FIELD_ID: encode_id(key)}
-
-        await search_client.delete_documents(documents=[docs_to_delete])
-        await search_client.close()
+        collection = self.pinecone.Index(collection_name)
+        for i in range(0, len(keys), MAX_DELETE_BATCH_SIZE):
+            collection.delete(keys[i : i + MAX_DELETE_BATCH_SIZE])
+        collection.delete(keys)
 
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float = 0.0,
         with_embedding: bool = False,
     ) -> tuple[MemoryRecord, float]:
-        """Gets the nearest match to an embedding using vector configuration parameters.
+        """Gets the nearest match to an embedding using cosine similarity.
 
-        Arguments:
-            collection_name {str}       -- The name of the collection to get the nearest match from.
-            embedding {ndarray}         -- The embedding to find the nearest match to.
-            min_relevance_score {float} -- The minimum relevance score of the match. (default: {0.0})
-            with_embedding {bool}       -- Whether to include the embedding in the result. (default: {False})
+        Args:
+            collection_name (str): The name of the collection to get the nearest match from.
+            embedding (ndarray): The embedding to find the nearest match to.
+            min_relevance_score (float): The minimum relevance score of the match. (default: {0.0})
+            with_embedding (bool): Whether to include the embedding in the result. (default: {False})
 
         Returns:
-            Tuple[MemoryRecord, float] -- The record and the relevance score.
+            Tuple[MemoryRecord, float]: The record and the relevance score.
         """
-
-        memory_records = await self.get_nearest_matches(
+        matches = await self.get_nearest_matches(
             collection_name=collection_name,
             embedding=embedding,
+            limit=1,
             min_relevance_score=min_relevance_score,
             with_embeddings=with_embedding,
-            limit=1,
         )
-
-        if len(memory_records) > 0:
-            return memory_records[0]
-        else:
-            return None
+        return matches[0]
 
     async def get_nearest_matches(
         self,
         collection_name: str,
         embedding: ndarray,
         limit: int,
         min_relevance_score: float = 0.0,
         with_embeddings: bool = False,
     ) -> list[tuple[MemoryRecord, float]]:
-        """Gets the nearest matches to an embedding using vector configuration.
+        """Gets the nearest matches to an embedding using cosine similarity.
 
-        Parameters:
-            collection_name (str)       -- The name of the collection to get the nearest matches from.
-            embedding (ndarray)         -- The embedding to find the nearest matches to.
-            limit {int}                 -- The maximum number of matches to return.
-            min_relevance_score {float} -- The minimum relevance score of the matches. (default: {0.0})
-            with_embeddings {bool}      -- Whether to include the embeddings in the results. (default: {False})
+        Args:
+            collection_name (str): The name of the collection to get the nearest matches from.
+            embedding (ndarray): The embedding to find the nearest matches to.
+            limit (int): The maximum number of matches to return.
+            min_relevance_score (float): The minimum relevance score of the matches. (default: {0.0})
+            with_embeddings (bool): Whether to include the embeddings in the results. (default: {False})
 
         Returns:
-            List[Tuple[MemoryRecord, float]] -- The records and their relevance scores.
+            List[Tuple[MemoryRecord, float]]: The records and their relevance scores.
         """
+        if not await self.does_collection_exist(collection_name):
+            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
-        # Look up Search client class to see if exists or create
-        search_client = self._search_index_client.get_search_client(collection_name.lower())
+        collection = self.pinecone.Index(collection_name)
 
-        vector = VectorizedQuery(vector=embedding.flatten(), k_nearest_neighbors=limit, fields=SEARCH_FIELD_EMBEDDING)
-
-        search_results = await search_client.search(
-            search_text="*",
-            select=get_field_selection(with_embeddings),
-            vector_queries=[vector],
+        if limit > MAX_QUERY_WITHOUT_METADATA_BATCH_SIZE:
+            raise ServiceInvalidRequestError(
+                "Limit must be less than or equal to " + f"{MAX_QUERY_WITHOUT_METADATA_BATCH_SIZE}"
+            )
+        elif limit > MAX_QUERY_WITH_METADATA_BATCH_SIZE:
+            query_response = collection.query(
+                vector=embedding.tolist(),
+                top_k=limit,
+                include_values=False,
+                include_metadata=False,
+            )
+            keys = [match.id for match in query_response.matches]
+            fetch_response = await self.__get_batch(collection_name, keys, with_embeddings)
+            vectors = fetch_response.vectors
+            for match in query_response.matches:
+                vectors[match.id].update(match)
+            matches = [vectors[key] for key in vectors.keys()]
+        else:
+            query_response = collection.query(
+                vector=embedding.tolist(),
+                top_k=limit,
+                include_values=with_embeddings,
+                include_metadata=True,
+            )
+            matches = query_response.matches
+        if min_relevance_score is not None:
+            matches = [match for match in matches if match.score >= min_relevance_score]
+        return (
+            [
+                (
+                    parse_payload(match, with_embeddings),
+                    match["score"],
+                )
+                for match in matches
+            ]
+            if len(matches) > 0
+            else []
         )
 
-        if not search_results or search_results is None:
-            await search_client.close()
-            return []
-
-        # Convert the results to MemoryRecords
-        nearest_results = []
-        async for search_record in search_results:
-            if search_record["@search.score"] < min_relevance_score:
-                continue
-
-            memory_record = dict_to_memory_record(search_record, with_embeddings)
-            nearest_results.append((memory_record, search_record["@search.score"]))
-
-        await search_client.close()
-        return nearest_results
+    async def __get_batch(
+        self, collection_name: str, keys: list[str], with_embeddings: bool = False
+    ) -> "FetchResponse":
+        index = self.pinecone.Index(collection_name)
+        if len(keys) > MAX_FETCH_BATCH_SIZE:
+            fetch_response = index.fetch(keys[0:MAX_FETCH_BATCH_SIZE])
+            for i in range(MAX_FETCH_BATCH_SIZE, len(keys), MAX_FETCH_BATCH_SIZE):
+                fetch_response.vectors.update(index.fetch(keys[i : i + MAX_FETCH_BATCH_SIZE]).vectors)
+        else:
+            fetch_response = index.fetch(keys)
+        return fetch_response
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,21 +25,20 @@
     search_endpoint: str | None = None,
     admin_key: str | None = None,
     azure_credential: AzureKeyCredential | None = None,
     token_credential: TokenCredential | None = None,
 ):
     """Return a client for Azure Cognitive Search.
 
-    Arguments:
-        search_endpoint {str}                 -- Optional endpoint (default: {None}).
-        admin_key {str}                       -- Optional API key (default: {None}).
-        azure_credential {AzureKeyCredential} -- Optional Azure credentials (default: {None}).
-        token_credential {TokenCredential}    -- Optional Token credential (default: {None}).
+    Args:
+        search_endpoint (str): Optional endpoint (default: {None}).
+        admin_key (str): Optional API key (default: {None}).
+        azure_credential (AzureKeyCredential): Optional Azure credentials (default: {None}).
+        token_credential (TokenCredential): Optional Token credential (default: {None}).
     """
-
     ENV_VAR_ENDPOINT = "AZURE_COGNITIVE_SEARCH_ENDPOINT"
     ENV_VAR_API_KEY = "AZURE_COGNITIVE_SEARCH_ADMIN_KEY"
 
     # Load environment variables
     load_dotenv()
 
     # Service endpoint
@@ -79,21 +78,21 @@
 
     raise ValueError("Error: unable to create Azure Cognitive Search client.")
 
 
 def get_index_schema(vector_size: int, vector_search_profile_name: str) -> list:
     """Return the schema of search indexes.
 
-    Arguments:
-        vector_size {int} -- The size of the vectors being stored in collection/index.
+    Args:
+        vector_size (int): The size of the vectors being stored in collection/index.
+        vector_search_profile_name (str): The name of the vector search profile.
 
     Returns:
-        list -- The Azure Cognitive Search schema as list type.
+        list: The Azure Cognitive Search schema as list type.
     """
-
     search_fields = [
         SimpleField(
             name=SEARCH_FIELD_ID,
             type=SearchFieldDataType.String,
             searchable=True,
             filterable=True,
             retrievable=True,
@@ -145,21 +144,20 @@
 
     return search_fields
 
 
 def get_field_selection(with_embeddings: bool) -> list[str]:
     """Get the list of fields to search and load.
 
-    Arguments:
-        with_embedding {bool} -- Whether to include the embedding vector field.
+    Args:
+        with_embeddings (bool): Whether to include the embedding vector field.
 
     Returns:
-        List[str] -- List of fields.
+        List[str]: List of fields.
     """
-
     field_selection = [
         SEARCH_FIELD_ID,
         SEARCH_FIELD_TEXT,
         SEARCH_FIELD_SRC,
         SEARCH_FIELD_DESC,
         SEARCH_FIELD_METADATA,
         SEARCH_FIELD_IS_REF,
@@ -170,21 +168,21 @@
 
     return field_selection
 
 
 def dict_to_memory_record(data: dict, with_embeddings: bool) -> MemoryRecord:
     """Converts a search result to a MemoryRecord.
 
-    Arguments:
-        data {dict} -- Azure Cognitive Search result data.
+    Args:
+        data (dict): Azure Cognitive Search result data.
+        with_embeddings (bool): Whether to include the embedding vector field.
 
     Returns:
-        MemoryRecord -- The MemoryRecord from Azure Cognitive Search Data Result.
+        MemoryRecord: The MemoryRecord from Azure Cognitive Search Data Result.
     """
-
     sk_result = MemoryRecord(
         id=decode_id(data[SEARCH_FIELD_ID]),
         key=data[SEARCH_FIELD_ID],
         text=data[SEARCH_FIELD_TEXT],
         external_source_name=data[SEARCH_FIELD_SRC],
         description=data[SEARCH_FIELD_DESC],
         additional_metadata=data[SEARCH_FIELD_METADATA],
@@ -192,23 +190,22 @@
         embedding=data[SEARCH_FIELD_EMBEDDING] if with_embeddings else None,
         timestamp=None,
     )
     return sk_result
 
 
 def memory_record_to_search_record(record: MemoryRecord) -> dict:
-    """Convert a MemoryRecord to a dictionary
+    """Convert a MemoryRecord to a dictionary.
 
-    Arguments:
-        record {MemoryRecord} -- The MemoryRecord from Azure Cognitive Search Data Result.
+    Args:
+        record (MemoryRecord): The MemoryRecord from Azure Cognitive Search Data Result.
 
     Returns:
-        data {dict} -- Dictionary data.
+        data (dict): Dictionary data.
     """
-
     return {
         SEARCH_FIELD_ID: encode_id(record._id),
         SEARCH_FIELD_TEXT: str(record._text),
         SEARCH_FIELD_SRC: record._external_source_name or "",
         SEARCH_FIELD_DESC: record._description or "",
         SEARCH_FIELD_METADATA: record._additional_metadata or "",
         SEARCH_FIELD_IS_REF: str(record._is_reference),
@@ -218,23 +215,21 @@
 
 def encode_id(id: str) -> str:
     """Encode a record id to ensure compatibility with Azure Cognitive Search.
 
     Azure Cognitive Search keys can contain only letters, digits, underscore, dash,
     equal sign, recommending to encode values with a URL-safe algorithm.
     """
-
     id_bytes = id.encode("ascii")
     base64_bytes = base64.b64encode(id_bytes)
     return base64_bytes.decode("ascii")
 
 
 def decode_id(base64_id: str) -> str:
     """Decode a record id to the original value.
 
     Azure Cognitive Search keys can contain only letters, digits, underscore, dash,
     equal sign, recommending to encode values with a URL-safe algorithm.
     """
-
     base64_bytes = base64_id.encode("ascii")
     message_bytes = base64.b64decode(base64_bytes)
     return message_bytes.decode("ascii")
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,20 +19,22 @@
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 @experimental_class
 class AzureCosmosDBMemoryStore(MemoryStoreBase):
-    """A memory store that uses AzureCosmosDB for MongoDB vCore, to perform vector similarity search on a fully
-    managed MongoDB compatible database service.
-    https://learn.microsoft.com/en-us/azure/cosmos-db/mongodb/vcore/vector-search"""
+    """A memory store that uses AzureCosmosDB for MongoDB vCore.
+
+    To perform vector similarity search on a fully managed MongoDB compatible database service.
+    https://learn.microsoft.com/en-us/azure/cosmos-db/mongodb/vcore/vector-search.
+    """
 
     # Right now this only supports Mongo, but set up to support more later.
-    apiStore: AzureCosmosDBStoreApi = None
+    api_store: AzureCosmosDBStoreApi = None
     mongodb_client = None
     database = None
     index_name = None
     vector_dimensions = None
     num_lists = None
     similarity = None
     collection_name = None
@@ -50,24 +52,23 @@
         num_lists: int = 100,
         similarity: CosmosDBSimilarityType = CosmosDBSimilarityType.COS,
         kind: CosmosDBVectorSearchType = CosmosDBVectorSearchType.VECTOR_HNSW,
         m: int = 16,
         ef_construction: int = 64,
         ef_search: int = 40,
     ):
+        """Initializes a new instance of the AzureCosmosDBMemoryStore class."""
         if vector_dimensions <= 0:
             raise MemoryConnectorInitializationError("Vector dimensions must be a positive number.")
-        # if connection_string is None:
-        #     raise ValueError("Connection String cannot be empty.")
         if database_name is None:
             raise MemoryConnectorInitializationError("Database Name cannot be empty.")
         if index_name is None:
             raise MemoryConnectorInitializationError("Index Name cannot be empty.")
 
-        self.cosmosStore = cosmosStore
+        self.cosmos_store = cosmosStore
         self.index_name = index_name
         self.num_lists = num_lists
         self.similarity = similarity
         self.kind = kind
         self.m = m
         self.ef_construction = ef_construction
         self.ef_search = ef_search
@@ -85,19 +86,18 @@
         similarity,
         kind,
         m,
         ef_construction,
         ef_search,
         env_file_path: str | None = None,
     ) -> MemoryStoreBase:
-        """Creates the underlying data store based on the API definition"""
+        """Creates the underlying data store based on the API definition."""
         # Right now this only supports Mongo, but set up to support more later.
         apiStore: AzureCosmosDBStoreApi = None
         if cosmos_api == "mongo-vcore":
-
             cosmosdb_settings = None
             try:
                 cosmosdb_settings = AzureCosmosDBSettings.create(env_file_path=env_file_path)
             except ValidationError as e:
                 logger.warning(f"Failed to load AzureCosmosDB pydantic settings: {e}")
 
             cosmos_connstr = cosmos_connstr or (
@@ -137,160 +137,160 @@
         )
         await store.create_collection(collection_name)
         return store
 
     async def create_collection(self, collection_name: str) -> None:
         """Creates a new collection in the data store.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
 
         Returns:
             None
         """
-        return await self.cosmosStore.create_collection(collection_name)
+        return await self.cosmos_store.create_collection(collection_name)
 
     async def get_collections(self) -> list[str]:
         """Gets the list of collections.
 
         Returns:
-            List[str] -- The list of collections.
+            List[str]: The list of collections.
         """
-        return await self.cosmosStore.get_collections()
+        return await self.cosmos_store.get_collections()
 
     async def delete_collection(self, collection_name: str) -> None:
         """Deletes a collection.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to delete.
+        Args:
+            collection_name (str): The name of the collection to delete.
 
         Returns:
             None
         """
-        return await self.cosmosStore.delete_collection("")
+        return await self.cosmos_store.delete_collection("")
 
     async def does_collection_exist(self, collection_name: str) -> bool:
         """Checks if a collection exists.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to check.
+        Args:
+            collection_name (str): The name of the collection to check.
 
         Returns:
-            bool -- True if the collection exists; otherwise, False.
+            bool: True if the collection exists; otherwise, False.
         """
-        return await self.cosmosStore.does_collection_exist("")
+        return await self.cosmos_store.does_collection_exist("")
 
     async def upsert(self, collection_name: str, record: MemoryRecord) -> str:
         """Upsert a record.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to upsert the record into.
-            record {MemoryRecord} -- The record to upsert.
+        Args:
+            collection_name (str): The name of the collection to upsert the record into.
+            record (MemoryRecord): The record to upsert.
 
         Returns:
-            str -- The unique record id of the record.
+            str: The unique record id of the record.
         """
-        return await self.cosmosStore.upsert("", record)
+        return await self.cosmos_store.upsert("", record)
 
     async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
         """Upsert a batch of records.
 
-        Arguments:
-            collection_name {str}        -- The name of the collection to upsert the records into.
-            records {List[MemoryRecord]} -- The records to upsert.
+        Args:
+            collection_name (str): The name of the collection to upsert the records into.
+            records (List[MemoryRecord]): The records to upsert.
 
         Returns:
-            List[str] -- The unique database keys of the records.
+            List[str]: The unique database keys of the records.
         """
-        return await self.cosmosStore.upsert_batch("", records)
+        return await self.cosmos_store.upsert_batch("", records)
 
     async def get(self, collection_name: str, key: str, with_embedding: bool) -> MemoryRecord:
         """Gets a record.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to get the record from.
-            key {str}             -- The unique database key of the record.
-            with_embedding {bool} -- Whether to include the embedding in the result. (default: {False})
+        Args:
+            collection_name (str): The name of the collection to get the record from.
+            key (str): The unique database key of the record.
+            with_embedding (bool): Whether to include the embedding in the result. (default: {False})
 
         Returns:
-            MemoryRecord -- The record.
+            MemoryRecord: The record.
         """
-        return await self.cosmosStore.get("", key, with_embedding)
+        return await self.cosmos_store.get("", key, with_embedding)
 
     async def get_batch(self, collection_name: str, keys: list[str], with_embeddings: bool) -> list[MemoryRecord]:
         """Gets a batch of records.
 
-        Arguments:
-            collection_name {str}  -- The name of the collection to get the records from.
-            keys {List[str]}       -- The unique database keys of the records.
-            with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
+        Args:
+            collection_name (str): The name of the collection to get the records from.
+            keys (List[str]): The unique database keys of the records.
+            with_embeddings (bool): Whether to include the embeddings in the results. (default: {False})
 
         Returns:
-            List[MemoryRecord] -- The records.
+            List[MemoryRecord]: The records.
         """
-        return await self.cosmosStore.get_batch("", keys, with_embeddings)
+        return await self.cosmos_store.get_batch("", keys, with_embeddings)
 
     async def remove(self, collection_name: str, key: str) -> None:
         """Removes a record.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to remove the record from.
-            key {str}             -- The unique database key of the record to remove.
+        Args:
+            collection_name (str): The name of the collection to remove the record from.
+            key (str): The unique database key of the record to remove.
 
         Returns:
             None
         """
-        return await self.cosmosStore.remove("", key)
+        return await self.cosmos_store.remove("", key)
 
     async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         """Removes a batch of records.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to remove the records from.
-            keys {List[str]}      -- The unique database keys of the records to remove.
+        Args:
+            collection_name (str): The name of the collection to remove the records from.
+            keys (List[str]): The unique database keys of the records to remove.
 
         Returns:
             None
         """
-        return await self.cosmosStore.remove_batch("", keys)
+        return await self.cosmos_store.remove_batch("", keys)
 
     async def get_nearest_matches(
         self,
         collection_name: str,
         embedding: ndarray,
         limit: int,
         min_relevance_score: float,
         with_embeddings: bool,
     ) -> list[tuple[MemoryRecord, float]]:
         """Gets the nearest matches to an embedding using vector configuration.
 
         Parameters:
-            collection_name (str)       -- The name of the collection to get the nearest matches from.
-            embedding (ndarray)         -- The embedding to find the nearest matches to.
-            limit {int}                 -- The maximum number of matches to return.
-            min_relevance_score {float} -- The minimum relevance score of the matches. (default: {0.0})
-            with_embeddings {bool}      -- Whether to include the embeddings in the results. (default: {False})
+            collection_name (str)      : The name of the collection to get the nearest matches from.
+            embedding (ndarray)        : The embedding to find the nearest matches to.
+            limit (int): The maximum number of matches to return.
+            min_relevance_score (float): The minimum relevance score of the matches. (default: {0.0})
+            with_embeddings (bool): Whether to include the embeddings in the results. (default: {False})
 
         Returns:
-            List[Tuple[MemoryRecord, float]] -- The records and their relevance scores.
+            List[Tuple[MemoryRecord, float]]: The records and their relevance scores.
         """
-        return await self.cosmosStore.get_nearest_matches("", embedding, limit, min_relevance_score, with_embeddings)
+        return await self.cosmos_store.get_nearest_matches("", embedding, limit, min_relevance_score, with_embeddings)
 
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float,
         with_embedding: bool,
     ) -> tuple[MemoryRecord, float]:
         """Gets the nearest match to an embedding using vector configuration parameters.
 
-        Arguments:
-            collection_name {str}       -- The name of the collection to get the nearest match from.
-            embedding {ndarray}         -- The embedding to find the nearest match to.
-            min_relevance_score {float} -- The minimum relevance score of the match. (default: {0.0})
-            with_embedding {bool}       -- Whether to include the embedding in the result. (default: {False})
+        Args:
+            collection_name (str): The name of the collection to get the nearest match from.
+            embedding (ndarray): The embedding to find the nearest match to.
+            min_relevance_score (float): The minimum relevance score of the match. (default: {0.0})
+            with_embedding (bool): Whether to include the embedding in the result. (default: {False})
 
         Returns:
-            Tuple[MemoryRecord, float] -- The record and the relevance score.
+            Tuple[MemoryRecord, float]: The record and the relevance score.
         """
-        return await self.cosmosStore.get_nearest_match("", embedding, min_relevance_score, with_embedding)
+        return await self.cosmos_store.get_nearest_match("", embedding, min_relevance_score, with_embedding)
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmosdb_settings.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmosdb_settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 
 from semantic_kernel.connectors.memory.memory_settings_base import BaseModelSettings
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
 @experimental_class
 class AzureCosmosDBSettings(BaseModelSettings):
-    """Azure CosmosDB model settings
+    """Azure CosmosDB model settings.
 
-    Optional:
+    Args:
     - connection_string: str - Azure CosmosDB connection string
         (Env var COSMOSDB_CONNECTION_STRING)
     """
 
     api: str | None = None
     connection_string: SecretStr | None = None
 
     class Config(BaseModelSettings.Config):
+        """Pydantic configuration settings."""
+
         env_prefix = "COSMOSDB_"
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,22 +30,21 @@
     """IVF vector index"""
     VECTOR_HNSW = "vector-hnsw"
     """HNSW vector index"""
 
 
 @experimental_function
 def get_mongodb_search_client(connection_string: str, application_name: str):
-    """
-    Returns a client for Azure Cosmos Mongo vCore Vector DB
+    """Returns a client for Azure Cosmos Mongo vCore Vector DB.
 
-    Arguments:
-        connection_string {str}
+    Args:
+        connection_string (str): The connection string for the Azure Cosmos Mongo vCore Vector DB.
+        application_name (str): The name of the application.
 
     """
-
     ENV_VAR_COSMOS_CONN_STR = "AZCOSMOS_CONNSTR"
 
     load_dotenv()
 
     # Cosmos connection string
     if connection_string:
         cosmos_conn_str = connection_string
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import json
+import sys
 from typing import Any
 
 import numpy as np
 
-from semantic_kernel.connectors.memory.azure_cosmosdb.azure_cosmos_db_store_api import (
-    AzureCosmosDBStoreApi,
-)
+if sys.version_info >= (3, 12):
+    from typing import override
+else:
+    from typing_extensions import override
+
+from semantic_kernel.connectors.memory.azure_cosmosdb.azure_cosmos_db_store_api import AzureCosmosDBStoreApi
 from semantic_kernel.connectors.memory.azure_cosmosdb.cosmosdb_utils import (
     CosmosDBSimilarityType,
     CosmosDBVectorSearchType,
 )
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
@@ -77,25 +81,27 @@
         similarity: CosmosDBSimilarityType,
         kind: CosmosDBVectorSearchType,
         m: int,
         ef_construction: int,
         ef_search: int,
         database=None,
     ):
+        """Initializes a new instance of the MongoStoreApi class."""
         self.database = database
         self.collection_name = collection_name
         self.index_name = index_name
         self.num_lists = num_lists
         self.similarity = similarity
         self.vector_dimensions = vector_dimensions
         self.kind = kind
         self.m = m
         self.ef_construction = ef_construction
         self.ef_search = ef_search
 
+    @override
     async def create_collection(self, collection_name: str) -> None:
         if not await self.does_collection_exist(collection_name):
             if self.index_name not in self.database[collection_name].list_indexes():
                 # check the kind of vector search to be performed
                 # prepare the command accordingly
                 create_index_commands = {}
                 if self.kind == CosmosDBVectorSearchType.VECTOR_IVF:
@@ -152,27 +158,32 @@
                         "dimensions": dimensions,
                     },
                 }
             ],
         }
         return command
 
+    @override
     async def get_collections(self) -> list[str]:
         return self.database.list_collection_names()
 
+    @override
     async def delete_collection(self, collection_name: str) -> None:
         return self.collection.drop()
 
+    @override
     async def does_collection_exist(self, collection_name: str) -> bool:
         return collection_name in self.database.list_collection_names()
 
+    @override
     async def upsert(self, collection_name: str, record: MemoryRecord) -> str:
         result = await self.upsert_batch(collection_name, [record])
         return result[0]
 
+    @override
     async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
         doc_ids: list[str] = []
         cosmosRecords: list[dict] = []
         for record in records:
             cosmosRecord: dict = {
                 "_id": record.id,
                 "embedding": record.embedding.tolist(),
@@ -184,28 +195,30 @@
                 cosmosRecord["timestamp"] = record.timestamp
 
             doc_ids.append(cosmosRecord["_id"])
             cosmosRecords.append(cosmosRecord)
         self.collection.insert_many(cosmosRecords)
         return doc_ids
 
+    @override
     async def get(self, collection_name: str, key: str, with_embedding: bool) -> MemoryRecord:
         if not with_embedding:
             result = self.collection.find_one({"_id": key}, {"embedding": 0})
         else:
             result = self.collection.find_one({"_id": key})
         return MemoryRecord.local_record(
             id=result["_id"],
             embedding=np.array(result["embedding"]) if with_embedding else np.array([]),
             text=result["text"],
             description=result["description"],
             additional_metadata=result["metadata"],
             timestamp=result.get("timestamp", None),
         )
 
+    @override
     async def get_batch(self, collection_name: str, keys: list[str], with_embeddings: bool) -> list[MemoryRecord]:
         if not with_embeddings:
             results = self.collection.find({"_id": {"$in": keys}}, {"embedding": 0})
         else:
             results = self.collection.find({"_id": {"$in": keys}})
 
         return [
@@ -216,20 +229,23 @@
                 description=result["description"],
                 additional_metadata=result["metadata"],
                 timestamp=result.get("timestamp", None),
             )
             for result in results
         ]
 
+    @override
     async def remove(self, collection_name: str, key: str) -> None:
         self.collection.delete_one({"_id": key})
 
+    @override
     async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         self.collection.delete_many({"_id": {"$in": keys}})
 
+    @override
     async def get_nearest_matches(
         self,
         collection_name: str,
         embedding: np.ndarray,
         limit: int,
         min_relevance_score: float,
         with_embeddings: bool,
@@ -299,14 +315,15 @@
                     "similarityScore": {"$meta": "searchScore"},
                     "document": "$$ROOT",
                 }
             },
         ]
         return pipeline
 
+    @override
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: np.ndarray,
         min_relevance_score: float,
         with_embedding: bool,
     ) -> tuple[MemoryRecord, float]:
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/azure_cosmosdb_no_sql/azure_cosmosdb_no_sql_memory_store.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/azure_cosmosdb_no_sql/azure_cosmosdb_no_sql_memory_store.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import json
+import sys
 from typing import Any
 
+if sys.version_info >= (3, 12):
+    from typing import override
+else:
+    from typing_extensions import override
+
 import numpy as np
 from azure.cosmos.aio import ContainerProxy, CosmosClient, DatabaseProxy
 from numpy import ndarray
 
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
-# You can read more about vector search using AzureCosmosDBNoSQL here.
-# https://aka.ms/CosmosVectorSearch
 @experimental_class
 class AzureCosmosDBNoSQLMemoryStore(MemoryStoreBase):
+    """You can read more about vector search using AzureCosmosDBNoSQL here: https://aka.ms/CosmosVectorSearch."""
+
     cosmos_client: CosmosClient = None
     database: DatabaseProxy
     container: ContainerProxy
     database_name: str = None
     partition_key: str = None
     vector_embedding_policy: dict[str, Any] | None = None
     indexing_policy: dict[str, Any] | None = None
@@ -30,51 +36,58 @@
         cosmos_client: CosmosClient,
         database_name: str,
         partition_key: str,
         vector_embedding_policy: dict[str, Any] | None = None,
         indexing_policy: dict[str, Any] | None = None,
         cosmos_container_properties: dict[str, Any] | None = None,
     ):
+        """Initializes a new instance of the AzureCosmosDBNoSQLMemoryStore class."""
         if indexing_policy["vectorIndexes"] is None or len(indexing_policy["vectorIndexes"]) == 0:
             raise ValueError("vectorIndexes cannot be null or empty in the indexing_policy.")
         if vector_embedding_policy is None or len(vector_embedding_policy["vectorEmbeddings"]) == 0:
             raise ValueError("vectorEmbeddings cannot be null or empty in the vector_embedding_policy.")
 
         self.cosmos_client = cosmos_client
         self.database_name = database_name
         self.partition_key = partition_key
         self.vector_embedding_policy = vector_embedding_policy
         self.indexing_policy = indexing_policy
         self.cosmos_container_properties = cosmos_container_properties
 
+    @override
     async def create_collection(self, collection_name: str) -> None:
         # Create the database if it already doesn't exist
         self.database = await self.cosmos_client.create_database_if_not_exists(id=self.database_name)
 
         # Create the collection if it already doesn't exist
         self.container = await self.database.create_container_if_not_exists(
             id=collection_name,
             partition_key=self.cosmos_container_properties["partition_key"],
             indexing_policy=self.indexing_policy,
             vector_embedding_policy=self.vector_embedding_policy,
         )
 
+    @override
     async def get_collections(self) -> list[str]:
         return [container["id"] async for container in self.database.list_containers()]
 
+    @override
     async def delete_collection(self, collection_name: str) -> None:
         return await self.database.delete_container(collection_name)
 
+    @override
     async def does_collection_exist(self, collection_name: str) -> bool:
         return collection_name in [container["id"] async for container in self.database.list_containers()]
 
+    @override
     async def upsert(self, collection_name: str, record: MemoryRecord) -> str:
         result = await self.upsert_batch(collection_name, [record])
         return result[0]
 
+    @override
     async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
         doc_ids: list[str] = []
         for record in records:
             cosmosRecord: dict = {
                 "id": record.id,
                 "embedding": record.embedding.tolist(),
                 "text": record.text,
@@ -84,25 +97,27 @@
             if record.timestamp is not None:
                 cosmosRecord["timeStamp"] = record.timestamp
 
             await self.container.create_item(cosmosRecord)
             doc_ids.append(cosmosRecord["id"])
         return doc_ids
 
+    @override
     async def get(self, collection_name: str, key: str, with_embedding: bool) -> MemoryRecord:
         item = await self.container.read_item(key, partition_key=key)
         return MemoryRecord.local_record(
             id=item["id"],
             embedding=np.array(item["embedding"]) if with_embedding else np.array([]),
             text=item["text"],
             description=item["description"],
             additional_metadata=item["metadata"],
             timestamp=item.get("timestamp", None),
         )
 
+    @override
     async def get_batch(self, collection_name: str, keys: list[str], with_embeddings: bool) -> list[MemoryRecord]:
         query = "SELECT * FROM c WHERE ARRAY_CONTAINS(@ids, c.id)"
         parameters = [{"name": "@ids", "value": keys}]
 
         all_results = []
         items = [item async for item in self.container.query_items(query, parameters=parameters)]
         for item in items:
@@ -113,31 +128,32 @@
                 description=item["description"],
                 additional_metadata=item["metadata"],
                 timestamp=item.get("timestamp", None),
             )
             all_results.append(item)
         return all_results
 
+    @override
     async def remove(self, collection_name: str, key: str) -> None:
         await self.container.delete_item(key, partition_key=key)
 
+    @override
     async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         for key in keys:
             await self.container.delete_item(key, partition_key=key)
 
+    @override
     async def get_nearest_matches(
         self, collection_name: str, embedding: ndarray, limit: int, min_relevance_score: float, with_embeddings: bool
     ) -> list[tuple[MemoryRecord, float]]:
         embedding_key = self.vector_embedding_policy["vectorEmbeddings"][0]["path"][1:]
         query = (
-            "SELECT TOP {} c.id, c.{}, c.text, c.description, c.metadata, "
-            "c.timestamp, VectorDistance(c.{}, {}) AS SimilarityScore FROM c ORDER BY "
-            "VectorDistance(c.{}, {})".format(
-                limit, embedding_key, embedding_key, embedding.tolist(), embedding_key, embedding.tolist()
-            )
+            f"SELECT TOP {limit} c.id, c.{embedding_key}, c.text, c.description, c.metadata, "  # nosec
+            f"c.timestamp, VectorDistance(c.{embedding_key}, {embedding.tolist()}) AS SimilarityScore FROM c ORDER BY "  # nosec
+            f"VectorDistance(c.{embedding_key}, {embedding.tolist()})"  # nosec
         )
 
         items = [item async for item in self.container.query_items(query=query)]
         nearest_results = []
         for item in items:
             score = item["SimilarityScore"]
             if score < min_relevance_score:
@@ -149,14 +165,15 @@
                 description=item["description"],
                 additional_metadata=item["metadata"],
                 timestamp=item.get("timestamp", None),
             )
             nearest_results.append((result, score))
         return nearest_results
 
+    @override
     async def get_nearest_match(
         self, collection_name: str, embedding: ndarray, min_relevance_score: float, with_embedding: bool
     ) -> tuple[MemoryRecord, float]:
         nearest_results = await self.get_nearest_matches(
             collection_name=collection_name,
             embedding=embedding,
             limit=1,
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import TYPE_CHECKING, Optional
+import sys
+from typing import TYPE_CHECKING, Any, Optional
 
 from numpy import array, ndarray
 
+if sys.version_info >= (3, 12):
+    from typing import override
+else:
+    from typing_extensions import override
+
 from semantic_kernel.connectors.memory.chroma.utils import chroma_compute_similarity_scores, query_results_to_records
 from semantic_kernel.exceptions import ServiceInitializationError, ServiceResourceNotFoundError
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
 if TYPE_CHECKING:
@@ -23,26 +29,28 @@
 class ChromaMemoryStore(MemoryStoreBase):
     _client: "chromadb.Client"
 
     def __init__(
         self,
         persist_directory: str | None = None,
         client_settings: Optional["chromadb.config.Settings"] = None,
-        **kwargs,
+        **kwargs: Any,
     ) -> None:
-        """
-        ChromaMemoryStore provides an interface to store and retrieve data using ChromaDB.
+        """ChromaMemoryStore provides an interface to store and retrieve data using ChromaDB.
+
         Collection names with uppercase characters are not supported by ChromaDB, they will be automatically converted.
 
         Args:
             persist_directory (Optional[str], optional): Path to the directory where data will be persisted.
                 Defaults to None, which means the default settings for ChromaDB will be used.
             client_settings (Optional["chromadb.config.Settings"], optional): A Settings instance to configure
                 the ChromaDB client. Defaults to None, which means the default settings for ChromaDB will be used.
             similarity_fetch_limit (int, optional): The maximum number of results to calculate cosine-similarity.
+            **kwargs: Additional keyword arguments.
+
         Example:
             # Create a ChromaMemoryStore with a local specified directory for data persistence
             chroma_local_data_store = ChromaMemoryStore(persist_directory='/path/to/persist/directory')
             # Create a ChromaMemoryStore with a custom Settings instance
             chroma_remote_data_store = ChromaMemoryStore(
                 client_settings=Settings(
                     chroma_api_impl="rest",
@@ -70,75 +78,77 @@
                 )
         self._client = chromadb.Client(self._client_settings)
         self._persist_directory = persist_directory
         self._default_query_includes = ["embeddings", "metadatas", "documents"]
 
     async def create_collection(self, collection_name: str) -> None:
         """Creates a new collection in Chroma if it does not exist.
-            To prevent downloading model file from embedding_function,
-            embedding_function is set to "DoNotUseChromaEmbeddingFunction".
 
-        Arguments:
-            collection_name {str} -- The name of the collection to create.
+        To prevent downloading model file from embedding_function,
+        embedding_function is set to "DoNotUseChromaEmbeddingFunction".
+
+        Args:
+            collection_name (str): The name of the collection to create.
             The name of the collection will be converted to snake case.
 
         Returns:
             None
         """
         self._client.create_collection(name=collection_name)
 
+    @override
     async def get_collection(self, collection_name: str) -> Optional["Collection"]:
         try:
             # Current version of ChromeDB rejects camel case collection names.
             return self._client.get_collection(name=collection_name)
         except ValueError:
             return None
 
     async def get_collections(self) -> list[str]:
         """Gets the list of collections.
 
         Returns:
-            List[str] -- The list of collections.
+            List[str]: The list of collections.
         """
         return [collection.name for collection in self._client.list_collections()]
 
     async def delete_collection(self, collection_name: str) -> None:
         """Deletes a collection.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to delete.
+        Args:
+            collection_name (str): The name of the collection to delete.
 
         Returns:
             None
         """
         self._client.delete_collection(name=collection_name)
 
     async def does_collection_exist(self, collection_name: str) -> bool:
         """Checks if a collection exists.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to check.
+        Args:
+            collection_name (str): The name of the collection to check.
 
         Returns:
-            bool -- True if the collection exists; otherwise, False.
+            bool: True if the collection exists; otherwise, False.
         """
         if await self.get_collection(collection_name) is None:
             return False
         else:
             return True
 
     async def upsert(self, collection_name: str, record: MemoryRecord) -> str:
-        """Upserts a single MemoryRecord.
+        """Upsert a single MemoryRecord.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to upsert the record into.
-            records {MemoryRecord} -- The record to upsert.
+        Args:
+            collection_name (str): The name of the collection to upsert the record into.
+            record (MemoryRecord): The record to upsert.
 
         Returns:
-            List[str] -- The unique database key of the record.
+            List[str]: The unique database key of the record.
         """
         collection = await self.get_collection(collection_name)
         if collection is None:
             raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
         record._key = record._id
         metadata = {
@@ -156,84 +166,84 @@
             embeddings=record.embedding.tolist(),
             documents=record._text,
             ids=record._key,
         )
         return record._key
 
     async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
-        """Upserts a batch of records.
+        """Upsert a batch of records.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to upsert the records into.
-            records {List[MemoryRecord]} -- The records to upsert.
+        Args:
+            collection_name (str): The name of the collection to upsert the records into.
+            records (List[MemoryRecord]): The records to upsert.
 
         Returns:
-            List[str] -- The unique database keys of the records. In Pinecone, these are the record IDs.
+            List[str]: The unique database keys of the records. In Pinecone, these are the record IDs.
         """
         # upsert is checking collection existence
         return [await self.upsert(collection_name, record) for record in records]
 
     async def get(self, collection_name: str, key: str, with_embedding: bool) -> MemoryRecord:
         """Gets a record.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to get the record from.
-            key {str} -- The unique database key of the record.
-            with_embedding {bool} -- Whether to include the embedding in the result. (default: {False})
+        Args:
+            collection_name (str): The name of the collection to get the record from.
+            key (str): The unique database key of the record.
+            with_embedding (bool): Whether to include the embedding in the result. (default: {False})
 
         Returns:
-            MemoryRecord -- The record.
+            MemoryRecord: The record.
         """
         records = await self.get_batch(collection_name, [key], with_embedding)
         try:
             return records[0]
         except IndexError as exc:
             raise ServiceResourceNotFoundError(
                 f"Record with key '{key}' does not exist in collection '{collection_name}'"
             ) from exc
 
     async def get_batch(self, collection_name: str, keys: list[str], with_embeddings: bool) -> list[MemoryRecord]:
         """Gets a batch of records.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to get the records from.
-            keys {List[str]} -- The unique database keys of the records.
-            with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
+        Args:
+            collection_name (str): The name of the collection to get the records from.
+            keys (List[str]): The unique database keys of the records.
+            with_embeddings (bool): Whether to include the embeddings in the results. (default: {False})
 
         Returns:
-            List[MemoryRecord] -- The records.
+            List[MemoryRecord]: The records.
         """
         collection = await self.get_collection(collection_name)
         if collection is None:
             raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
         query_includes = ["embeddings", "metadatas", "documents"] if with_embeddings else ["metadatas", "documents"]
 
         value = collection.get(ids=keys, include=query_includes)
         record = query_results_to_records(value, with_embeddings)
         return record
 
     async def remove(self, collection_name: str, key: str) -> None:
         """Removes a record.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to remove the record from.
-            key {str} -- The unique database key of the record to remove.
+        Args:
+            collection_name (str): The name of the collection to remove the record from.
+            key (str): The unique database key of the record to remove.
 
         Returns:
             None
         """
         await self.remove_batch(collection_name, [key])
 
     async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         """Removes a batch of records.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to remove the records from.
-            keys {List[str]} -- The unique database keys of the records to remove.
+        Args:
+            collection_name (str): The name of the collection to remove the records from.
+            keys (List[str]): The unique database keys of the records to remove.
 
         Returns:
             None
         """
         collection = await self.get_collection(collection_name=collection_name)
         if collection is not None:
             collection.delete(ids=keys)
@@ -244,23 +254,23 @@
         embedding: ndarray,
         limit: int,
         min_relevance_score: float = 0.0,
         with_embeddings: bool = True,
     ) -> list[tuple[MemoryRecord, float]]:
         """Gets the nearest matches to an embedding using cosine similarity.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to get the nearest matches from.
-            embedding {ndarray} -- The embedding to find the nearest matches to.
-            limit {int} -- The maximum number of matches to return.
-            min_relevance_score {float} -- The minimum relevance score of the matches. (default: {0.0})
-            with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
+        Args:
+            collection_name (str): The name of the collection to get the nearest matches from.
+            embedding (ndarray): The embedding to find the nearest matches to.
+            limit (int): The maximum number of matches to return.
+            min_relevance_score (float): The minimum relevance score of the matches. (default: {0.0})
+            with_embeddings (bool): Whether to include the embeddings in the results. (default: {False})
 
         Returns:
-            List[Tuple[MemoryRecord, float]] -- The records and their relevance scores.
+            List[Tuple[MemoryRecord, float]]: The records and their relevance scores.
         """
         if with_embeddings is False:
             logger.warning(
                 "Chroma returns distance score not cosine similarity score.\
                 So embeddings are automatically queried from database for calculation."
             )
         collection = await self.get_collection(collection_name)
@@ -311,59 +321,24 @@
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float = 0.0,
         with_embedding: bool = True,
     ) -> tuple[MemoryRecord, float]:
         """Gets the nearest match to an embedding using cosine similarity.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to get the nearest match from.
-            embedding {ndarray} -- The embedding to find the nearest match to.
-            min_relevance_score {float} -- The minimum relevance score of the match. (default: {0.0})
-            with_embedding {bool} -- Whether to include the embedding in the result. (default: {False})
+        Args:
+            collection_name (str): The name of the collection to get the nearest match from.
+            embedding (ndarray): The embedding to find the nearest match to.
+            min_relevance_score (float): The minimum relevance score of the match. (default: {0.0})
+            with_embedding (bool): Whether to include the embedding in the result. (default: {False})
 
         Returns:
-            Tuple[MemoryRecord, float] -- The record and the relevance score.
+            Tuple[MemoryRecord, float]: The record and the relevance score.
         """
         results = await self.get_nearest_matches(
             collection_name=collection_name,
             embedding=embedding,
             limit=1,
             min_relevance_score=min_relevance_score,
             with_embeddings=with_embedding,
         )
         return results[0]
-
-
-if __name__ == "__main__":
-    import asyncio
-
-    import numpy as np
-
-    memory = ChromaMemoryStore()
-    memory_record1 = MemoryRecord(
-        id="test_id1",
-        text="sample text1",
-        is_reference=False,
-        embedding=np.array([0.5, 0.5]),
-        description="description",
-        external_source_name="external source",
-        timestamp="timestamp",
-    )
-    memory_record2 = MemoryRecord(
-        id="test_id2",
-        text="sample text2",
-        is_reference=False,
-        embedding=np.array([0.25, 0.75]),
-        description="description",
-        external_source_name="external source",
-        timestamp="timestamp",
-    )
-
-    asyncio.run(memory.create_collection("test_collection"))
-    collection = asyncio.run(memory.get_collection("test_collection"))
-
-    asyncio.run(memory.upsert_batch(collection.name, [memory_record1, memory_record2]))
-
-    result = asyncio.run(memory.get(collection.name, "test_id1", True))
-    results = asyncio.run(memory.get_nearest_match("test_collection", np.array([0.5, 0.5])))
-    print(results)
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/chroma/utils.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/chroma/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 from numpy import array, linalg, ndarray
 
 from semantic_kernel.memory.memory_record import MemoryRecord
 
 if TYPE_CHECKING:
     from chromadb.api.types import QueryResult
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 def camel_to_snake(camel_str):
+    """Convert camel case to snake case."""
     snake_str = ""
     for i, char in enumerate(camel_str):
         if char.isupper():
             if i != 0 and camel_str[i - 1].islower():
                 snake_str += "_"
             if i != len(camel_str) - 1 and camel_str[i + 1].islower():
                 snake_str += "_"
         snake_str += char.lower()
     return snake_str
 
 
 def query_results_to_records(results: "QueryResult", with_embedding: bool) -> list[MemoryRecord]:
-    # if results has only one record, it will be a list instead of a nested list
-    # this is to make sure that results is always a nested list
-    # {'ids': ['test_id1'], 'embeddings': [[...]], 'documents': ['sample text1'], 'metadatas': [{...}]}
-    # => {'ids': [['test_id1']], 'embeddings': [[[...]]], 'documents': [['sample text1']], 'metadatas': [[{...}]]}
+    """Turn query results into Memory Records.
+
+    If results has only one record, it will be a list instead of a nested list
+    this is to make sure that results is always a nested list
+    {'ids': ['test_id1'], 'embeddings': [[...]], 'documents': ['sample text1'], 'metadatas': [{...}]}
+    => {'ids': [['test_id1']], 'embeddings': [[[...]]], 'documents': [['sample text1']], 'metadatas': [[{...}]]}
+    """
     try:
         if isinstance(results["ids"][0], str):
             for k, v in results.items():
                 results[k] = [v]
     except IndexError:
         return []
 
@@ -79,24 +83,25 @@
                 results["documents"][0],
                 results["metadatas"][0],
             )
         ]
     return memory_records
 
 
-def chroma_compute_similarity_scores(embedding: ndarray, embedding_array: ndarray, **kwargs) -> ndarray:
+def chroma_compute_similarity_scores(embedding: ndarray, embedding_array: ndarray, **kwargs: Any) -> ndarray:
     """Computes the cosine similarity scores between a query embedding and a group of embeddings.
-    Arguments:
-        embedding {ndarray} -- The query embedding.
-        embedding_array {ndarray} -- The group of embeddings.
+
+    Args:
+        embedding (ndarray): The query embedding.
+        embedding_array (ndarray): The group of embeddings.
+        **kwargs: Additional keyword arguments.
+
     Returns:
-        ndarray -- The cosine similarity scores.
+        ndarray: The cosine similarity scores.
     """
-    if kwargs.get("logger"):
-        logger.warning("The `logger` parameter is deprecated. Please use the `logging` module instead.")
     query_norm = linalg.norm(embedding)
     collection_norm = linalg.norm(embedding_array, axis=1)
 
     # Compute indices for which the similarity scores can be computed
     valid_indices = (query_norm != 0) & (collection_norm != 0)
 
     # Initialize the similarity scores with -1 to distinguish the cases
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/memory_settings_base.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/memory_settings_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,19 +6,22 @@
 
 
 @experimental_class
 class BaseModelSettings(BaseSettings):
     env_file_path: str | None = None
 
     class Config:
+        """Pydantic configuration settings."""
+
         env_file = None
         env_file_encoding = "utf-8"
         extra = "ignore"
         case_sensitive = False
 
     @classmethod
     def create(cls, **kwargs):
+        """Create an instance of the class."""
         if "env_file_path" in kwargs and kwargs["env_file_path"]:
             cls.Config.env_file = kwargs["env_file_path"]
         else:
             cls.Config.env_file = None
         return cls(**kwargs)
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     SEARCH_FIELD_TIMESTAMP,
 ]
 
 
 @experimental_function
 def memoryrecord_to_milvus_dict(mem: MemoryRecord) -> dict[str, Any]:
     """Convert a memoryrecord into a dict.
+
     Args:
         mem (MemoryRecord): MemoryRecord to convert.
 
     Returns:
         dict: Dict result.
     """
     ret_dict = {}
@@ -93,14 +94,15 @@
         key=milvus_dict.get("key", None),
         timestamp=milvus_dict.get(SEARCH_FIELD_TIMESTAMP, None),
     )
 
 
 @experimental_function
 def create_fields(dimensions: int) -> list[FieldSchema]:
+    """Create the fields for the Milvus collection."""
     return [
         FieldSchema(
             name=SEARCH_FIELD_ID,
             dtype=DataType.VARCHAR,
             is_primary=True,
             auto_id=False,
             max_length=100,
@@ -144,28 +146,29 @@
 
 @experimental_class
 class MilvusMemoryStore(MemoryStoreBase):
     def __init__(
         self,
         uri: str = "http://localhost:19530",
         token: str | None = None,
-        **kwargs,
+        **kwargs: Any,
     ) -> None:
-        """MilvusMemoryStore allows for searching for records using Milvus/Zilliz Cloud.
+        """Memory store based on Milvus.
 
         For more details on how to get the service started, take a look here:
-            Milvus: https://milvus.io/docs/get_started.md
-            Zilliz Cloud: https://docs.zilliz.com/docs/quick-start
+        - Milvus: https://milvus.io/docs/get_started.md
+        - Zilliz Cloud: https://docs.zilliz.com/docs/quick-start
 
 
         Args:
             uri (str, optional): The uri of the cluster. Defaults to
                 "http://localhost:19530".
             token (Optional[str], optional): The token to connect to the cluster if
                 authentication is required. Defaults to None.
+            **kwargs (Any): Unused.
         """
         connections.connect("default", uri=uri, token=token)
         self.collections: dict[str, Collection] = {}
 
     async def create_collection(
         self,
         collection_name: str,
@@ -255,15 +258,15 @@
             collection_name=collection_name,
             records=[record],
             batch_size=0,
         )
         return res[0]
 
     async def upsert_batch(self, collection_name: str, records: list[MemoryRecord], batch_size=100) -> list[str]:
-        """_summary_
+        """_summary_.
 
         Args:
             collection_name (str): The collection name.
             records (List[MemoryRecord]): A list of memory records.
             batch_size (int, optional): Batch size of the insert, 0 is a batch
                 size of total size. Defaults to 100.
 
@@ -299,15 +302,15 @@
         Returns:
             MemoryRecord: The MemoryRecord for the key.
         """
         res = await self.get_batch(collection_name=collection_name, keys=[key], with_embeddings=with_embedding)
         return res[0]
 
     async def get_batch(self, collection_name: str, keys: list[str], with_embeddings: bool) -> list[MemoryRecord]:
-        """Get the MemoryRecords corresponding to the keys
+        """Get the MemoryRecords corresponding to the keys.
 
         Args:
             collection_name (str): _description_
             keys (List[str]): _description_
             with_embeddings (bool): _description_
 
         Raises:
@@ -425,15 +428,15 @@
 
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float = 0.0,
         with_embedding: bool = False,
-    ) -> tuple[MemoryRecord, float]:
+    ) -> tuple[MemoryRecord, float] | None:
         """Find the nearest match for an embedding.
 
         Args:
             collection_name (str): The collection to search.
             embedding (ndarray): The embedding to search for.
             min_relevance_score (float, optional): T. Defaults to 0.0.
             with_embedding (bool, optional): Whether to include embedding in result. Defaults to False.
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/mongodb_atlas/README.md` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/mongodb_atlas/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 @experimental_class
 class MongoDBAtlasMemoryStore(MemoryStoreBase):
-    """Memory Store for MongoDB Atlas Vector Search Connections"""
+    """Memory Store for MongoDB Atlas Vector Search Connections."""
 
     __slots__ = ("_mongo_client", "__database_name")
 
     _mongo_client: motor_asyncio.AsyncIOMotorClient
     __database_name: str
     __index_name: str
 
@@ -42,14 +42,15 @@
         self,
         index_name: str | None = None,
         connection_string: str | None = None,
         database_name: str | None = None,
         read_preference: ReadPreference | None = ReadPreference.PRIMARY,
         env_file_path: str | None = None,
     ):
+        """Initializes a new instance of the MongoDBAtlasMemoryStore class."""
         from semantic_kernel.connectors.memory.mongodb_atlas import MongoDBAtlasSettings
 
         mongodb_settings = None
         try:
             mongodb_settings = MongoDBAtlasSettings.create(env_file_path=env_file_path)
         except ValidationError as e:
             logger.warning(f"Failed to load the MongoDBAtlas pydantic settings: {e}")
@@ -66,182 +67,190 @@
             driver=DriverInfo("Microsoft Semantic Kernel", metadata.version("semantic-kernel")),
         )
         self.__database_name = database_name or DEFAULT_DB_NAME
         self.__index_name = index_name or DEFAULT_SEARCH_INDEX_NAME
 
     @property
     def database_name(self) -> str:
+        """The name of the database."""
         return self.__database_name
 
     @property
     def database(self) -> core.AgnosticDatabase:
+        """The database object."""
         return self._mongo_client[self.database_name]
 
     @property
     def index_name(self) -> str:
+        """The name of the index."""
         return self.__index_name
 
     @property
     def num_candidates(self) -> int:
+        """The number of candidates to return."""
         return self.__num_candidates
 
     async def close(self):
-        """Async close connection, invoked by MemoryStoreBase.__aexit__()"""
+        """Async close connection, invoked by MemoryStoreBase.__aexit__()."""
         if self._mongo_client:
             self._mongo_client.close()
             self._mongo_client = None
 
     async def create_collection(self, collection_name: str) -> None:
         """Creates a new collection in the data store.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
 
         Returns:
             None
         """
         if not await self.does_collection_exist(collection_name):
             await self.database.create_collection(collection_name)
 
     async def get_collections(
         self,
     ) -> list[str]:
         """Gets all collection names in the data store.
 
         Returns:
-            List[str] -- A group of collection names.
+            List[str]: A group of collection names.
         """
         return await self.database.list_collection_names()
 
     async def delete_collection(self, collection_name: str) -> None:
         """Deletes a collection from the data store.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
 
         Returns:
             None
         """
         await self.database[collection_name].drop()
 
     async def does_collection_exist(self, collection_name: str) -> bool:
         """Determines if a collection exists in the data store.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
 
         Returns:
-            bool -- True if given collection exists, False if not.
+            bool: True if given collection exists, False if not.
         """
         return collection_name in (await self.get_collections())
 
     async def upsert(self, collection_name: str, record: MemoryRecord) -> str:
-        """Upserts a memory record into the data store. Does not guarantee that the collection exists.
+        """Upserts a memory record into the data store.
+
+        Does not guarantee that the collection exists.
             If the record already exists, it will be updated.
             If the record does not exist, it will be created.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
-            record {MemoryRecord} -- The memory record to upsert.
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
+            record (MemoryRecord): The memory record to upsert.
 
         Returns:
-            str -- The unique identifier for the memory record.
+            str: The unique identifier for the memory record.
         """
-
         document: Mapping[str, Any] = memory_record_to_mongo_document(record)
 
         update_result: results.UpdateResult = await self.database[collection_name].update_one(
             document, {"$set": document}, upsert=True
         )
 
-        assert update_result.acknowledged
+        if not update_result.acknowledged:
+            raise ValueError("Upsert failed")
         return record._id
 
     async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
-        """Upserts a group of memory records into the data store. Does not guarantee that the collection exists.
+        """Upserts a group of memory records into the data store.
+
+        Does not guarantee that the collection exists.
             If the record already exists, it will be updated.
             If the record does not exist, it will be created.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
-            records {MemoryRecord} -- The memory records to upsert.
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
+            records (MemoryRecord): The memory records to upsert.
 
         Returns:
-            List[str] -- The unique identifiers for the memory records.
+            List[str]: The unique identifiers for the memory records.
         """
-
         upserts: list[UpdateOne] = []
         for record in records:
             document = memory_record_to_mongo_document(record)
             upserts.append(UpdateOne(document, {"$set": document}, upsert=True))
         bulk_update_result: results.BulkWriteResult = await self.database[collection_name].bulk_write(
             upserts, ordered=False
         )
 
         # Assert the number matched and the number upserted equal the total batch updated
         logger.debug(
             "matched_count=%s, upserted_count=%s",
             bulk_update_result.matched_count,
             bulk_update_result.upserted_count,
         )
-        assert bulk_update_result.matched_count + bulk_update_result.upserted_count == len(records)
+        if bulk_update_result.matched_count + bulk_update_result.upserted_count != len(records):
+            raise ValueError("Batch upsert failed")
         return [record._id for record in records]
 
     async def get(self, collection_name: str, key: str, with_embedding: bool) -> MemoryRecord:
         """Gets a memory record from the data store. Does not guarantee that the collection exists.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
-            key {str} -- The unique id associated with the memory record to get.
-            with_embedding {bool} -- If true, the embedding will be returned in the memory record.
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
+            key (str): The unique id associated with the memory record to get.
+            with_embedding (bool): If true, the embedding will be returned in the memory record.
 
         Returns:
-            MemoryRecord -- The memory record if found
+            MemoryRecord: The memory record if found
         """
         document = await self.database[collection_name].find_one({MONGODB_FIELD_ID: key})
 
         return document_to_memory_record(document, with_embedding) if document else None
 
     async def get_batch(self, collection_name: str, keys: list[str], with_embeddings: bool) -> list[MemoryRecord]:
         """Gets a batch of memory records from the data store. Does not guarantee that the collection exists.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
-            keys {List[str]} -- The unique ids associated with the memory records to get.
-            with_embeddings {bool} -- If true, the embedding will be returned in the memory records.
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
+            keys (List[str]): The unique ids associated with the memory records to get.
+            with_embeddings (bool): If true, the embedding will be returned in the memory records.
 
         Returns:
-            List[MemoryRecord] -- The memory records associated with the unique keys provided.
+            List[MemoryRecord]: The memory records associated with the unique keys provided.
         """
         results = self.database[collection_name].find({MONGODB_FIELD_ID: {"$in": keys}})
 
         return [
             document_to_memory_record(result, with_embeddings) for result in await results.to_list(length=len(keys))
         ]
 
     async def remove(self, collection_name: str, key: str) -> None:
         """Removes a memory record from the data store. Does not guarantee that the collection exists.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
-            key {str} -- The unique id associated with the memory record to remove.
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
+            key (str): The unique id associated with the memory record to remove.
 
         Returns:
             None
         """
         if not await self.does_collection_exist(collection_name):
             raise ServiceResourceNotFoundError(f"collection {collection_name} not found")
         await self.database[collection_name].delete_one({MONGODB_FIELD_ID: key})
 
     async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         """Removes a batch of memory records from the data store. Does not guarantee that the collection exists.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
-            keys {List[str]} -- The unique ids associated with the memory records to remove.
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
+            keys (List[str]): The unique ids associated with the memory records to remove.
 
         Returns:
             None
         """
         if not await self.does_collection_exist(collection_name):
             raise ServiceResourceNotFoundError(f"collection {collection_name} not found")
         deletes: list[DeleteOne] = [DeleteOne({MONGODB_FIELD_ID: key}) for key in keys]
@@ -254,22 +263,23 @@
         embedding: ndarray,
         limit: int,
         with_embeddings: bool,
         min_relevance_score: float | None = None,
     ) -> list[tuple[MemoryRecord, float]]:
         """Gets the nearest matches to an embedding of type float. Does not guarantee that the collection exists.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
-            embedding {ndarray} -- The embedding to compare the collection's embeddings with.
-            limit {int} -- The maximum number of similarity results to return, defaults to 1.
-            min_relevance_score {float} -- The minimum relevance threshold for returned results.
-            with_embeddings {bool} -- If true, the embeddings will be returned in the memory records.
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
+            embedding (ndarray): The embedding to compare the collection's embeddings with.
+            limit (int): The maximum number of similarity results to return, defaults to 1.
+            min_relevance_score (float): The minimum relevance threshold for returned results.
+            with_embeddings (bool): If true, the embeddings will be returned in the memory records.
+
         Returns:
-            List[Tuple[MemoryRecord, float]] -- A list of tuples where item1 is a MemoryRecord and item2
+            List[Tuple[MemoryRecord, float]]: A list of tuples where item1 is a MemoryRecord and item2
                 is its similarity score as a float.
         """
         pipeline: list[dict[str, Any]] = []
         vector_search_query: list[Mapping[str, Any]] = {
             "$vectorSearch": {
                 "queryVector": embedding.tolist(),
                 "limit": limit,
@@ -301,22 +311,22 @@
         collection_name: str,
         embedding: ndarray,
         with_embedding: bool,
         min_relevance_score: float | None = None,
     ) -> tuple[MemoryRecord, float]:
         """Gets the nearest match to an embedding of type float. Does not guarantee that the collection exists.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
-            embedding {ndarray} -- The embedding to compare the collection's embeddings with.
-            min_relevance_score {float} -- The minimum relevance threshold for returned result.
-            with_embedding {bool} -- If true, the embeddings will be returned in the memory record.
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
+            embedding (ndarray): The embedding to compare the collection's embeddings with.
+            min_relevance_score (float): The minimum relevance threshold for returned result.
+            with_embedding (bool): If true, the embeddings will be returned in the memory record.
 
         Returns:
-            Tuple[MemoryRecord, float] -- A tuple consisting of the MemoryRecord and the similarity score as a float.
+            Tuple[MemoryRecord, float]: A tuple consisting of the MemoryRecord and the similarity score as a float.
         """
         matches: list[tuple[MemoryRecord, float]] = await self.get_nearest_matches(
             collection_name=collection_name,
             embedding=embedding,
             limit=1,
             min_relevance_score=min_relevance_score,
             with_embeddings=with_embedding,
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_settings.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 
 from semantic_kernel.connectors.memory.memory_settings_base import BaseModelSettings
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
 @experimental_class
 class MongoDBAtlasSettings(BaseModelSettings):
-    """MongoDB Atlas model settings
+    """MongoDB Atlas model settings.
 
-    Optional:
+    Args:
     - connection_string: str - MongoDB Atlas connection string
         (Env var MONGODB_ATLAS_CONNECTION_STRING)
     """
 
     connection_string: SecretStr | None = None
 
     class Config(BaseModelSettings.Config):
+        """Pydantic configuration settings."""
+
         env_prefix = "MONGODB_ATLAS_"
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/mongodb_atlas/utils.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/mongodb_atlas/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,19 +18,20 @@
 MONGODB_FIELD_KEY = "key"
 MONGODB_FIELD_TIMESTAMP = "timestamp"
 
 
 def document_to_memory_record(data: dict, with_embeddings: bool) -> MemoryRecord:
     """Converts a search result to a MemoryRecord.
 
-    Arguments:
-        data {dict} -- Azure Cognitive Search result data.
+    Args:
+        data (dict): Azure Cognitive Search result data.
+        with_embeddings (bool): Whether to include embeddings.
 
     Returns:
-        MemoryRecord -- The MemoryRecord from Azure Cognitive Search Data Result.
+        MemoryRecord: The MemoryRecord from Azure Cognitive Search Data Result.
     """
     meta = data.get(MONGODB_FIELD_METADATA, {})
 
     return MemoryRecord(
         id=meta.get(MONGODB_FIELD_ID),
         text=meta.get(MONGODB_FIELD_TEXT),
         external_source_name=meta.get(MONGODB_FIELD_SRC),
@@ -40,23 +41,22 @@
         embedding=array(data.get(MONGODB_FIELD_EMBEDDING)) if with_embeddings else None,
         timestamp=data.get(MONGODB_FIELD_TIMESTAMP),
         key=meta.get(MONGODB_FIELD_ID),
     )
 
 
 def memory_record_to_mongo_document(record: MemoryRecord) -> dict:
-    """Convert a MemoryRecord to a dictionary
+    """Convert a MemoryRecord to a dictionary.
 
-    Arguments:
-        record {MemoryRecord} -- The MemoryRecord from Azure Cognitive Search Data Result.
+    Args:
+        record (MemoryRecord): The MemoryRecord from Azure Cognitive Search Data Result.
 
     Returns:
-        data {dict} -- Dictionary data.
+        data (dict): Dictionary data.
     """
-
     return {
         MONGODB_FIELD_ID: record._id,
         MONGODB_FIELD_METADATA: {
             MONGODB_FIELD_ID: record._id,
             MONGODB_FIELD_TEXT: record._text,
             MONGODB_FIELD_SRC: record._external_source_name or "",
             MONGODB_FIELD_DESC: record._description or "",
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,400 +1,516 @@
 # Copyright (c) Microsoft. All rights reserved.
 
+import atexit
+import json
 import logging
-from typing import NamedTuple
 
+import numpy as np
 from numpy import ndarray
-from pinecone import FetchResponse, IndexDescription, IndexList, Pinecone, ServerlessSpec
+from psycopg import Cursor
+from psycopg.sql import SQL, Identifier
+from psycopg_pool import ConnectionPool
 from pydantic import ValidationError
 
-from semantic_kernel.connectors.memory.pinecone.pinecone_settings import PineconeSettings
-from semantic_kernel.connectors.memory.pinecone.utils import (
-    build_payload,
-    parse_payload,
-)
+from semantic_kernel.connectors.memory.postgres.postgres_settings import PostgresSettings
 from semantic_kernel.exceptions import (
     ServiceInitializationError,
-    ServiceInvalidRequestError,
     ServiceResourceNotFoundError,
     ServiceResponseException,
 )
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
-# Limitations set by Pinecone at https://docs.pinecone.io/reference/known-limitations
-MAX_DIMENSIONALITY = 20000
-MAX_UPSERT_BATCH_SIZE = 100
-MAX_QUERY_WITHOUT_METADATA_BATCH_SIZE = 10000
-MAX_QUERY_WITH_METADATA_BATCH_SIZE = 1000
-MAX_FETCH_BATCH_SIZE = 1000
-MAX_DELETE_BATCH_SIZE = 1000
+# Limitation based on pgvector documentation https://github.com/pgvector/pgvector#what-if-i-want-to-index-vectors-with-more-than-2000-dimensions
+MAX_DIMENSIONALITY = 2000
+DEFAULT_SCHEMA = "public"
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 @experimental_class
-class PineconeMemoryStore(MemoryStoreBase):
-    """A memory store that uses Pinecone as the backend."""
+class PostgresMemoryStore(MemoryStoreBase):
+    """A memory store that uses Postgres with pgvector as the backend."""
 
-    _pinecone_api_key: str
+    _connection_string: str
+    _connection_pool: ConnectionPool
     _default_dimensionality: int
-
-    DEFAULT_INDEX_SPEC: ServerlessSpec = ServerlessSpec(
-        cloud="aws",
-        region="us-east-1",
-    )
+    _schema: str
 
     def __init__(
         self,
-        api_key: str,
+        connection_string: str,
         default_dimensionality: int,
+        min_pool: int,
+        max_pool: int,
+        schema: str = DEFAULT_SCHEMA,
         env_file_path: str | None = None,
     ) -> None:
-        """Initializes a new instance of the PineconeMemoryStore class.
+        """Initializes a new instance of the PostgresMemoryStore class.
 
-        Arguments:
-            pinecone_api_key {str} -- The Pinecone API key.
-            default_dimensionality {int} -- The default dimensionality to use for new collections.
-            env_file_path {str | None} -- Use the environment settings file as a fallback
+        Args:
+            connection_string (str): The connection string to the Postgres database.
+            default_dimensionality (int): The default dimensionality of the embeddings.
+            min_pool (int): The minimum number of connections in the connection pool.
+            max_pool (int): The maximum number of connections in the connection pool.
+            schema (str): The schema to use. (default: {"public"})
+            env_file_path (str | None): Use the environment settings file as a fallback
                 to environment variables. (Optional)
         """
-        if default_dimensionality > MAX_DIMENSIONALITY:
-            raise ServiceInitializationError(
-                f"Dimensionality of {default_dimensionality} exceeds "
-                + f"the maximum allowed value of {MAX_DIMENSIONALITY}."
-            )
-
-        pinecone_settings = None
+        postgres_settings = None
         try:
-            pinecone_settings = PineconeSettings.create(env_file_path=env_file_path)
+            postgres_settings = PostgresSettings.create(env_file_path=env_file_path)
         except ValidationError as e:
-            logger.warning(f"Failed to load the Pinecone pydantic settings: {e}")
+            logger.warning(f"Failed to load Postgres pydantic settings: {e}")
 
-        api_key = api_key or (
-            pinecone_settings.api_key.get_secret_value() if pinecone_settings and pinecone_settings.api_key else None
+        connection_string = connection_string or (
+            postgres_settings.connection_string.get_secret_value()
+            if postgres_settings and postgres_settings.connection_string
+            else None
         )
-        assert api_key, "The Pinecone api_key cannot be None."
 
-        self._pinecone_api_key = api_key
-        self._default_dimensionality = default_dimensionality
+        self._check_dimensionality(default_dimensionality)
 
-        self.pinecone = Pinecone(api_key=self._pinecone_api_key)
-        self.collection_names_cache = set()
+        self._connection_string = connection_string
+        self._default_dimensionality = default_dimensionality
+        self._connection_pool = ConnectionPool(self._connection_string, min_size=min_pool, max_size=max_pool)
+        self._schema = schema
+        atexit.register(self._connection_pool.close)
 
     async def create_collection(
         self,
         collection_name: str,
         dimension_num: int | None = None,
-        distance_type: str | None = "cosine",
-        index_spec: NamedTuple = DEFAULT_INDEX_SPEC,
     ) -> None:
-        """Creates a new collection in Pinecone if it does not exist.
-            This function creates an index, by default the following index
-            settings are used: metric = cosine, cloud = aws, region = us-east-1.
-
-        Arguments:
-            collection_name {str} -- The name of the collection to create.
-            In Pinecone, a collection is represented as an index. The concept
-            of "collection" in Pinecone is just a static copy of an index.
+        r"""Creates a new collection.
+
+        Args:
+            collection_name (str): The name of the collection to create.\n
+            dimension_num (Optional[int]): The dimensionality of the embeddings. (default: {None})
+            Uses the default dimensionality when not provided
 
         Returns:
             None
         """
         if dimension_num is None:
             dimension_num = self._default_dimensionality
-        if dimension_num > MAX_DIMENSIONALITY:
-            raise ServiceInitializationError(
-                f"Dimensionality of {dimension_num} exceeds " + f"the maximum allowed value of {MAX_DIMENSIONALITY}."
-            )
-
-        if not await self.does_collection_exist(collection_name):
-            self.pinecone.create_index(
-                name=collection_name, dimension=dimension_num, metric=distance_type, spec=index_spec
-            )
-            self.collection_names_cache.add(collection_name)
+        else:
+            self._check_dimensionality(dimension_num)
 
-    async def describe_collection(self, collection_name: str) -> IndexDescription | None:
-        """Gets the description of the index.
-        Arguments:
-            collection_name {str} -- The name of the index to get.
-        Returns:
-            Optional[dict] -- The index.
-        """
-        if await self.does_collection_exist(collection_name):
-            return self.pinecone.describe_index(collection_name)
-        return None
+        with self._connection_pool.connection() as conn:
+            with conn.cursor() as cur:
+                cur.execute(
+                    SQL(
+                        """
+                        CREATE TABLE IF NOT EXISTS {scm}.{tbl} (
+                            key TEXT PRIMARY KEY,
+                            embedding vector({dim}),
+                            metadata JSONB,
+                            timestamp TIMESTAMP
+                        )"""
+                    ).format(
+                        scm=Identifier(self._schema),
+                        tbl=Identifier(collection_name),
+                        dim=dimension_num,
+                    ),
+                    (),
+                )
 
-    async def get_collections(
-        self,
-    ) -> IndexList:
+    async def get_collections(self) -> list[str]:
         """Gets the list of collections.
 
         Returns:
-            IndexList -- The list of collections.
+            List[str]: The list of collections.
         """
-        return self.pinecone.list_indexes()
+        with self._connection_pool.connection() as conn:
+            with conn.cursor() as cur:
+                return await self.__get_collections(cur)
 
     async def delete_collection(self, collection_name: str) -> None:
         """Deletes a collection.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to delete.
+        Args:
+            collection_name (str): The name of the collection to delete.
 
         Returns:
             None
         """
-        if await self.does_collection_exist(collection_name):
-            self.pinecone.delete_index(collection_name)
-            self.collection_names_cache.discard(collection_name)
+        with self._connection_pool.connection() as conn:
+            with conn.cursor() as cur:
+                cur.execute(
+                    SQL("DROP TABLE IF EXISTS {scm}.{tbl} CASCADE").format(
+                        scm=Identifier(self._schema), tbl=Identifier(collection_name)
+                    ),
+                )
 
     async def does_collection_exist(self, collection_name: str) -> bool:
         """Checks if a collection exists.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to check.
+        Args:
+            collection_name (str): The name of the collection to check.
 
         Returns:
-            bool -- True if the collection exists; otherwise, False.
+            bool: True if the collection exists; otherwise, False.
         """
-        if collection_name in self.collection_names_cache:
-            return True
-
-        index_collection_names = self.pinecone.list_indexes().names()
-        self.collection_names_cache |= set(index_collection_names)
-
-        return collection_name in index_collection_names
+        with self._connection_pool.connection() as conn:
+            with conn.cursor() as cur:
+                return await self.__does_collection_exist(cur, collection_name)
 
     async def upsert(self, collection_name: str, record: MemoryRecord) -> str:
-        """Upserts a record.
-
-        Arguments:
-            collection_name {str} -- The name of the collection to upsert the record into.
-            record {MemoryRecord} -- The record to upsert.
-
-        Returns:
-            str -- The unique database key of the record. In Pinecone, this is the record ID.
-        """
-        if not await self.does_collection_exist(collection_name):
-            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
-
-        collection = self.pinecone.Index(collection_name)
-
-        upsert_response = collection.upsert(
-            vectors=[(record._id, record.embedding.tolist(), build_payload(record))],
-            namespace="",
-        )
-
-        if upsert_response.upserted_count is None:
-            raise ServiceResponseException(f"Error upserting record: {upsert_response.message}")
+        r"""Upserts a record.
 
-        return record._id
+        Args:
+            collection_name (str): The name of the collection to upsert the record into.\n
+            record (MemoryRecord): The record to upsert.
+
+        Returns:
+            str: The unique database key of the record. In Pinecone, this is the record ID.
+        """
+        with self._connection_pool.connection() as conn:
+            with conn.cursor() as cur:
+                if not await self.__does_collection_exist(cur, collection_name):
+                    raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
+                cur.execute(
+                    SQL(
+                        """
+                        INSERT INTO {scm}.{tbl} (key, embedding, metadata, timestamp)
+                        VALUES (%s, %s, %s, %s)
+                        ON CONFLICT (key) DO UPDATE
+                        SET embedding = EXCLUDED.embedding,
+                            metadata = EXCLUDED.metadata,
+                            timestamp = EXCLUDED.timestamp
+                        RETURNING key
+                        """
+                    ).format(
+                        scm=Identifier(self._schema),
+                        tbl=Identifier(collection_name),
+                    ),
+                    (
+                        record._id,
+                        record.embedding.tolist(),
+                        self.__serialize_metadata(record),
+                        record._timestamp,
+                    ),
+                )
+                result = cur.fetchone()
+                if result is None:
+                    raise ServiceResponseException("Upsert failed")
+                return result[0]
 
     async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
         """Upserts a batch of records.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to upsert the records into.
-            records {List[MemoryRecord]} -- The records to upsert.
-
-        Returns:
-            List[str] -- The unique database keys of the records.
-        """
-        if not await self.does_collection_exist(collection_name):
-            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
-
-        collection = self.pinecone.Index(collection_name)
-
-        vectors = [
-            (
-                record._id,
-                record.embedding.tolist(),
-                build_payload(record),
-            )
-            for record in records
-        ]
-
-        upsert_response = collection.upsert(vectors, namespace="", batch_size=MAX_UPSERT_BATCH_SIZE)
+        Args:
+            collection_name (str): The name of the collection to upsert the records into.
+            records (List[MemoryRecord]): The records to upsert.
+
+        Returns:
+            List[str]: The unique database keys of the records.
+        """
+        with self._connection_pool.connection() as conn:
+            with conn.cursor() as cur:
+                if not await self.__does_collection_exist(cur, collection_name):
+                    raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
+                cur.nextset()
+                cur.executemany(
+                    SQL(
+                        """
+                        INSERT INTO {scm}.{tbl} (key, embedding, metadata, timestamp)
+                        VALUES (%s, %s, %s, %s)
+                        ON CONFLICT (key) DO UPDATE
+                        SET embedding = EXCLUDED.embedding,
+                            metadata = EXCLUDED.metadata,
+                            timestamp = EXCLUDED.timestamp
+                        RETURNING key
+                        """
+                    ).format(
+                        scm=Identifier(self._schema),
+                        tbl=Identifier(collection_name),
+                    ),
+                    [
+                        (
+                            record._id,
+                            record.embedding.tolist(),
+                            self.__serialize_metadata(record),
+                            record._timestamp,
+                        )
+                        for record in records
+                    ],
+                    returning=True,
+                )
 
-        if upsert_response.upserted_count is None:
-            raise ServiceResponseException(f"Error upserting record: {upsert_response.message}")
-        else:
-            return [record._id for record in records]
+                # collate results
+                results = [cur.fetchone()]
+                while cur.nextset():
+                    results.append(cur.fetchone())
+                if None in results:
+                    raise ServiceResponseException("Upsert failed")
+                return [result[0] for result in results if result is not None]
 
     async def get(self, collection_name: str, key: str, with_embedding: bool = False) -> MemoryRecord:
         """Gets a record.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to get the record from.
-            key {str} -- The unique database key of the record.
-            with_embedding {bool} -- Whether to include the embedding in the result. (default: {False})
-
-        Returns:
-            MemoryRecord -- The record.
-        """
-        if not await self.does_collection_exist(collection_name):
-            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
-
-        collection = self.pinecone.Index(collection_name)
-        fetch_response = collection.fetch([key])
-
-        if len(fetch_response.vectors) == 0:
-            raise ServiceResourceNotFoundError(f"Record with key '{key}' does not exist")
-
-        return parse_payload(fetch_response.vectors[key], with_embedding)
+        Args:
+            collection_name (str): The name of the collection to get the record from.
+            key (str): The unique database key of the record.
+            with_embedding (bool): Whether to include the embedding in the result. (default: {False})
+
+        Returns:
+            MemoryRecord: The record.
+        """
+        with self._connection_pool.connection() as conn:
+            with conn.cursor() as cur:
+                if not await self.__does_collection_exist(cur, collection_name):
+                    raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
+                cur.execute(
+                    SQL(
+                        """
+                        SELECT key, embedding, metadata, timestamp
+                        FROM {scm}.{tbl}
+                        WHERE key = %s
+                        """
+                    ).format(
+                        scm=Identifier(self._schema),
+                        tbl=Identifier(collection_name),
+                    ),
+                    (key,),
+                )
+                result = cur.fetchone()
+                if result is None:
+                    raise ServiceResourceNotFoundError("Key not found")
+                return MemoryRecord.local_record(
+                    id=result[0],
+                    embedding=(
+                        np.fromstring(result[1].strip("[]"), dtype=float, sep=",") if with_embedding else np.array([])
+                    ),
+                    text=result[2]["text"],
+                    description=result[2]["description"],
+                    additional_metadata=result[2]["additional_metadata"],
+                    timestamp=result[3],
+                )
 
     async def get_batch(
         self, collection_name: str, keys: list[str], with_embeddings: bool = False
     ) -> list[MemoryRecord]:
         """Gets a batch of records.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to get the records from.
-            keys {List[str]} -- The unique database keys of the records.
-            with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
-
-        Returns:
-            List[MemoryRecord] -- The records.
-        """
-        if not await self.does_collection_exist(collection_name):
-            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
-
-        fetch_response = await self.__get_batch(collection_name, keys, with_embeddings)
-        return [parse_payload(fetch_response.vectors[key], with_embeddings) for key in fetch_response.vectors.keys()]
+        Args:
+            collection_name (str): The name of the collection to get the records from.
+            keys (List[str]): The unique database keys of the records.
+            with_embeddings (bool): Whether to include the embeddings in the results. (default: {False})
+
+        Returns:
+            List[MemoryRecord]: The records that were found from list of keys, can be empty.
+        """
+        with self._connection_pool.connection() as conn:
+            with conn.cursor() as cur:
+                if not await self.__does_collection_exist(cur, collection_name):
+                    raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
+                cur.execute(
+                    SQL(
+                        """
+                        SELECT key, embedding, metadata, timestamp
+                        FROM {scm}.{tbl}
+                        WHERE key = ANY(%s)
+                        """
+                    ).format(
+                        scm=Identifier(self._schema),
+                        tbl=Identifier(collection_name),
+                    ),
+                    (list(keys),),
+                )
+                results = cur.fetchall()
+                return [
+                    MemoryRecord.local_record(
+                        id=result[0],
+                        embedding=(
+                            np.fromstring(result[1].strip("[]"), dtype=float, sep=",")
+                            if with_embeddings
+                            else np.array([])
+                        ),
+                        text=result[2]["text"],
+                        description=result[2]["description"],
+                        additional_metadata=result[2]["additional_metadata"],
+                        timestamp=result[3],
+                    )
+                    for result in results
+                ]
 
     async def remove(self, collection_name: str, key: str) -> None:
         """Removes a record.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to remove the record from.
-            key {str} -- The unique database key of the record to remove.
+        Args:
+            collection_name (str): The name of the collection to remove the record from.
+            key (str): The unique database key of the record to remove.
 
         Returns:
             None
         """
-        if not await self.does_collection_exist(collection_name):
-            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
-
-        collection = self.pinecone.Index(collection_name)
-        collection.delete([key])
+        with self._connection_pool.connection() as conn:
+            with conn.cursor() as cur:
+                if not await self.__does_collection_exist(cur, collection_name):
+                    raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
+                cur.execute(
+                    SQL(
+                        """
+                        DELETE FROM {scm}.{tbl}
+                        WHERE key = %s
+                        """
+                    ).format(scm=Identifier(self._schema), tbl=Identifier(collection_name)),
+                    (key,),
+                )
 
     async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         """Removes a batch of records.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to remove the records from.
-            keys {List[str]} -- The unique database keys of the records to remove.
+        Args:
+            collection_name (str): The name of the collection to remove the records from.
+            keys (List[str]): The unique database keys of the records to remove.
 
         Returns:
             None
         """
-        if not await self.does_collection_exist(collection_name):
-            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
+        with self._connection_pool.connection() as conn:
+            with conn.cursor() as cur:
+                if not await self.__does_collection_exist(cur, collection_name):
+                    raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
+                cur.execute(
+                    SQL(
+                        """
+                        DELETE FROM {scm}.{tbl}
+                        WHERE key = ANY(%s)
+                        """
+                    ).format(scm=Identifier(self._schema), tbl=Identifier(collection_name)),
+                    (list(keys),),
+                )
+
+    async def get_nearest_matches(
+        self,
+        collection_name: str,
+        embedding: ndarray,
+        limit: int,
+        min_relevance_score: float = 0.0,
+        with_embeddings: bool = False,
+    ) -> list[tuple[MemoryRecord, float]]:
+        """Gets the nearest matches to an embedding using cosine similarity.
 
-        collection = self.pinecone.Index(collection_name)
-        for i in range(0, len(keys), MAX_DELETE_BATCH_SIZE):
-            collection.delete(keys[i : i + MAX_DELETE_BATCH_SIZE])
-        collection.delete(keys)
+        Args:
+            collection_name (str): The name of the collection to get the nearest matches from.
+            embedding (ndarray): The embedding to find the nearest matches to.
+            limit (int): The maximum number of matches to return.
+            min_relevance_score (float): The minimum relevance score of the matches. (default: {0.0})
+            with_embeddings (bool): Whether to include the embeddings in the results. (default: {False})
+
+        Returns:
+            List[Tuple[MemoryRecord, float]]: The records and their relevance scores.
+        """
+        with self._connection_pool.connection() as conn:
+            with conn.cursor() as cur:
+                if not await self.__does_collection_exist(cur, collection_name):
+                    raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
+                cur.execute(
+                    SQL(
+                        """
+                        SELECT key,
+                            embedding,
+                            metadata,
+                            cosine_similarity,
+                            timestamp
+                        FROM (
+                            SELECT key, embedding, metadata, 1 - (embedding <=> '[{emb}]') \
+                                AS cosine_similarity, timestamp
+                            FROM {scm}.{tbl}
+                        ) AS subquery
+                        WHERE cosine_similarity >= {mrs}
+                        ORDER BY cosine_similarity DESC
+                        LIMIT {limit}
+                        """
+                    ).format(
+                        scm=Identifier(self._schema),
+                        tbl=Identifier(collection_name),
+                        mrs=min_relevance_score,
+                        limit=limit,
+                        emb=SQL(",").join(embedding.tolist()),
+                    )
+                )
+                results = cur.fetchall()
+
+                return [
+                    (
+                        MemoryRecord.local_record(
+                            id=result[0],
+                            embedding=(
+                                np.fromstring(result[1].strip("[]"), dtype=float, sep=",")
+                                if with_embeddings
+                                else np.array([])
+                            ),
+                            text=result[2]["text"],
+                            description=result[2]["description"],
+                            additional_metadata=result[2]["additional_metadata"],
+                            timestamp=result[4],
+                        ),
+                        result[3],
+                    )
+                    for result in results
+                ]
 
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float = 0.0,
         with_embedding: bool = False,
     ) -> tuple[MemoryRecord, float]:
         """Gets the nearest match to an embedding using cosine similarity.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to get the nearest match from.
-            embedding {ndarray} -- The embedding to find the nearest match to.
-            min_relevance_score {float} -- The minimum relevance score of the match. (default: {0.0})
-            with_embedding {bool} -- Whether to include the embedding in the result. (default: {False})
+        Args:
+            collection_name (str): The name of the collection to get the nearest match from.
+            embedding (ndarray): The embedding to find the nearest match to.
+            min_relevance_score (float): The minimum relevance score of the match. (default: {0.0})
+            with_embedding (bool): Whether to include the embedding in the result. (default: {False})
 
         Returns:
-            Tuple[MemoryRecord, float] -- The record and the relevance score.
+            Tuple[MemoryRecord, float]: The record and the relevance score.
         """
-        matches = await self.get_nearest_matches(
+        results = await self.get_nearest_matches(
             collection_name=collection_name,
             embedding=embedding,
             limit=1,
             min_relevance_score=min_relevance_score,
             with_embeddings=with_embedding,
         )
-        return matches[0]
-
-    async def get_nearest_matches(
-        self,
-        collection_name: str,
-        embedding: ndarray,
-        limit: int,
-        min_relevance_score: float = 0.0,
-        with_embeddings: bool = False,
-    ) -> list[tuple[MemoryRecord, float]]:
-        """Gets the nearest matches to an embedding using cosine similarity.
-
-        Arguments:
-            collection_name {str} -- The name of the collection to get the nearest matches from.
-            embedding {ndarray} -- The embedding to find the nearest matches to.
-            limit {int} -- The maximum number of matches to return.
-            min_relevance_score {float} -- The minimum relevance score of the matches. (default: {0.0})
-            with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
-
-        Returns:
-            List[Tuple[MemoryRecord, float]] -- The records and their relevance scores.
-        """
-        if not await self.does_collection_exist(collection_name):
-            raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
-
-        collection = self.pinecone.Index(collection_name)
+        if len(results) == 0:
+            raise ServiceResourceNotFoundError("No match found")
+        return results[0]
+
+    async def __does_collection_exist(self, cur: Cursor, collection_name: str) -> bool:
+        results = await self.__get_collections(cur)
+        return collection_name in results
+
+    async def __get_collections(self, cur: Cursor) -> list[str]:
+        cur.execute(
+            """
+            SELECT table_name
+            FROM information_schema.tables
+            WHERE table_schema = %s
+            """,
+            (self._schema,),
+        )
+        return [row[0] for row in cur.fetchall()]
 
-        if limit > MAX_QUERY_WITHOUT_METADATA_BATCH_SIZE:
-            raise ServiceInvalidRequestError(
-                "Limit must be less than or equal to " + f"{MAX_QUERY_WITHOUT_METADATA_BATCH_SIZE}"
-            )
-        elif limit > MAX_QUERY_WITH_METADATA_BATCH_SIZE:
-            query_response = collection.query(
-                vector=embedding.tolist(),
-                top_k=limit,
-                include_values=False,
-                include_metadata=False,
-            )
-            keys = [match.id for match in query_response.matches]
-            fetch_response = await self.__get_batch(collection_name, keys, with_embeddings)
-            vectors = fetch_response.vectors
-            for match in query_response.matches:
-                vectors[match.id].update(match)
-            matches = [vectors[key] for key in vectors.keys()]
-        else:
-            query_response = collection.query(
-                vector=embedding.tolist(),
-                top_k=limit,
-                include_values=with_embeddings,
-                include_metadata=True,
+    def _check_dimensionality(self, dimension_num):
+        if dimension_num > MAX_DIMENSIONALITY:
+            raise ServiceInitializationError(
+                f"Dimensionality of {dimension_num} exceeds " + f"the maximum allowed value of {MAX_DIMENSIONALITY}."
             )
-            matches = query_response.matches
-        if min_relevance_score is not None:
-            matches = [match for match in matches if match.score >= min_relevance_score]
-        return (
-            [
-                (
-                    parse_payload(match, with_embeddings),
-                    match["score"],
-                )
-                for match in matches
-            ]
-            if len(matches) > 0
-            else []
-        )
+        if dimension_num <= 0:
+            raise ServiceInitializationError("Dimensionality must be a positive integer. ")
 
-    async def __get_batch(
-        self, collection_name: str, keys: list[str], with_embeddings: bool = False
-    ) -> "FetchResponse":
-        index = self.pinecone.Index(collection_name)
-        if len(keys) > MAX_FETCH_BATCH_SIZE:
-            fetch_response = index.fetch(keys[0:MAX_FETCH_BATCH_SIZE])
-            for i in range(MAX_FETCH_BATCH_SIZE, len(keys), MAX_FETCH_BATCH_SIZE):
-                fetch_response.vectors.update(index.fetch(keys[i : i + MAX_FETCH_BATCH_SIZE]).vectors)
-        else:
-            fetch_response = index.fetch(keys)
-        return fetch_response
+    def __serialize_metadata(self, record: MemoryRecord) -> str:
+        return json.dumps(
+            {
+                "text": record._text,
+                "description": record._description,
+                "additional_metadata": record._additional_metadata,
+            }
+        )
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/pinecone/pinecone_settings.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/pinecone/pinecone_settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 
 from semantic_kernel.connectors.memory.memory_settings_base import BaseModelSettings
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
 @experimental_class
 class PineconeSettings(BaseModelSettings):
-    """Pinecone model settings
+    """Pinecone model settings.
 
-    Required:
+    Args:
     - api_key: SecretStr - Pinecone API key
         (Env var PINECONE_API_KEY)
     """
 
     api_key: SecretStr | None = None
 
     class Config(BaseModelSettings.Config):
+        """Config for Pinecone settings."""
+
         env_prefix = "PINECONE_"
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/pinecone/utils.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/pinecone/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,31 +3,27 @@
 import numpy
 from pinecone import Vector
 
 from semantic_kernel.memory.memory_record import MemoryRecord
 
 
 def build_payload(record: MemoryRecord) -> dict:
-    """
-    Builds a metadata payload to be sent to Pinecone from a MemoryRecord.
-    """
+    """Builds a metadata payload to be sent to Pinecone from a MemoryRecord."""
     payload: dict = {}
     if record._text:
         payload["text"] = record._text
     if record._description:
         payload["description"] = record._description
     if record._additional_metadata:
         payload["additional_metadata"] = record._additional_metadata
     return payload
 
 
 def parse_payload(record: Vector, with_embeddings: bool) -> MemoryRecord:
-    """
-    Parses a record from Pinecone into a MemoryRecord.
-    """
+    """Parses a record from Pinecone into a MemoryRecord."""
     payload = record.metadata
     description = payload.get("description", None)
     text = payload.get("text", None)
     additional_metadata = payload.get("additional_metadata", None)
     return MemoryRecord.local_record(
         id=record.id,
         description=description,
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/postgres/postgres_settings.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/postgres/postgres_settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 
 from semantic_kernel.connectors.memory.memory_settings_base import BaseModelSettings
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
 @experimental_class
 class PostgresSettings(BaseModelSettings):
-    """Postgres model settings
+    """Postgres model settings.
 
-    Required:
+    Args:
     - connection_string: str - Postgres connection string
         (Env var POSTGRES_CONNECTION_STRING)
     """
 
     connection_string: SecretStr | None = None
 
     class Config(BaseModelSettings.Config):
+        """Config for Postgres settings."""
+
         env_prefix = "POSTGRES_"
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-"""
-QdrantMemoryStore provides functionality to add Qdrant vector database to support Semantic Kernel memory.
-The QdrantMemoryStore inherits from MemoryStoreBase for persisting/retrieving data from a Qdrant Vector Database.
-"""
-
 import asyncio
 import logging
+import sys
 import uuid
 
 from numpy import ndarray
 from qdrant_client import QdrantClient
 from qdrant_client import models as qdrant_models
 
+if sys.version_info >= (3, 12):
+    from typing import override
+else:
+    from typing_extensions import override
+
 from semantic_kernel.exceptions import ServiceResponseException
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
@@ -30,100 +31,63 @@
         vector_size: int,
         url: str | None = None,
         port: int | None = 6333,
         local: bool | None = False,
         **kwargs,
     ) -> None:
         """Initializes a new instance of the QdrantMemoryStore class."""
-        if kwargs.get("logger"):
-            logger.warning("The `logger` parameter is deprecated. Please use the `logging` module instead.")
         if local:
             if url:
                 self._qdrantclient = QdrantClient(location=url)
             else:
                 self._qdrantclient = QdrantClient(location=":memory:")
         else:
             self._qdrantclient = QdrantClient(url=url, port=port)
 
         self._default_vector_size = vector_size
 
+    @override
     async def create_collection(self, collection_name: str) -> None:
-        """Creates a new collection if it does not exist.
-
-        Arguments:
-            collection_name {str} -- The name of the collection to create.
-            vector_size {int} -- The size of the vector.
-            distance {Optional[str]} -- The distance metric to use. (default: {"Cosine"})
-        Returns:
-            None
-        """
         self._qdrantclient.recreate_collection(
             collection_name=collection_name,
             vectors_config=qdrant_models.VectorParams(
                 size=self._default_vector_size, distance=qdrant_models.Distance.COSINE
             ),
         )
 
+    @override
     async def get_collections(
         self,
     ) -> list[str]:
-        """Gets the list of collections.
-
-        Returns:
-            List[str] -- The list of collections.
-        """
         collection_info = self._qdrantclient.get_collections()
         return [collection.name for collection in collection_info.collections]
 
     async def get_collection(self, collection_name: str) -> qdrant_models.CollectionInfo:
-        """Gets the a collections based upon collection name.
+        """Gets the collection based upon collection name.
 
         Returns:
             CollectionInfo -- Collection Information from Qdrant about collection.
         """
         collection_info = self._qdrantclient.get_collection(collection_name=collection_name)
         return collection_info
 
+    @override
     async def delete_collection(self, collection_name: str) -> None:
-        """Deletes a collection.
-
-        Arguments:
-            collection_name {str} -- The name of the collection to delete.
-
-        Returns:
-            None
-        """
-
         self._qdrantclient.delete_collection(collection_name=collection_name)
 
+    @override
     async def does_collection_exist(self, collection_name: str) -> bool:
-        """Checks if a collection exists.
-
-        Arguments:
-            collection_name {str} -- The name of the collection to check.
-
-        Returns:
-            bool -- True if the collection exists; otherwise, False.
-        """
         try:
             result = await self.get_collection(collection_name=collection_name)
             return result.status == qdrant_models.CollectionStatus.GREEN
         except ValueError:
             return False
 
+    @override
     async def upsert(self, collection_name: str, record: MemoryRecord) -> str:
-        """Upserts a record.
-
-        Arguments:
-            collection_name {str} -- The name of the collection to upsert the record into.
-            record {MemoryRecord} -- The record to upsert.
-
-        Returns:
-            str -- The unique database key of the record.
-        """
         data_to_upsert = await self._convert_from_memory_record(
             collection_name=collection_name,
             record=record,
         )
 
         result = self._qdrantclient.upsert(
             collection_name=collection_name,
@@ -131,14 +95,15 @@
         )
 
         if result.status == qdrant_models.UpdateStatus.COMPLETED:
             return data_to_upsert.id
         else:
             raise ServiceResponseException("Upsert failed")
 
+    @override
     async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
         tasks = []
         for record in records:
             tasks.append(
                 self._convert_from_memory_record(
                     collection_name=collection_name,
                     record=record,
@@ -153,14 +118,15 @@
         )
 
         if result.status == qdrant_models.UpdateStatus.COMPLETED:
             return [data.id for data in data_to_upsert]
         else:
             raise ServiceResponseException("Batch upsert failed")
 
+    @override
     async def get(self, collection_name: str, key: str, with_embedding: bool = False) -> MemoryRecord | None:
         result = await self._get_existing_record_by_payload_id(
             collection_name=collection_name,
             payload_id=key,
             with_embedding=with_embedding,
         )
 
@@ -175,41 +141,47 @@
                 embedding=result.vector,
                 key=result.id,
                 timestamp=result.payload["_timestamp"],
             )
         else:
             return None
 
+    @override
     async def get_batch(
-        self, collection_name: str, keys: list[str], with_embeddings: bool = False
+        self,
+        collection_name: str,
+        keys: list[str],
+        with_embeddings: bool = False,
     ) -> list[MemoryRecord]:
         tasks = []
         for key in keys:
             tasks.append(
                 self.get(
                     collection_name=collection_name,
                     key=key,
                     with_embedding=with_embeddings,
                 )
             )
         return await asyncio.gather(*tasks)
 
+    @override
     async def remove(self, collection_name: str, key: str) -> None:
         existing_record = await self._get_existing_record_by_payload_id(
             collection_name=collection_name,
             payload_id=key,
             with_embedding=False,
         )
 
         if existing_record:
             pointId = existing_record.id
             result = self._qdrantclient.delete(collection_name=collection_name, points_selector=[pointId])
             if result.status != qdrant_models.UpdateStatus.COMPLETED:
                 raise ServiceResponseException("Delete failed")
 
+    @override
     async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         tasks = []
         for key in keys:
             tasks.append(
                 self._get_existing_record_by_payload_id(
                     collection_name=collection_name,
                     payload_id=key,
@@ -223,14 +195,15 @@
             result = self._qdrantclient.delete(
                 collection_name=collection_name,
                 points_selector=[record.id for record in existing_records],
             )
             if result.status != qdrant_models.UpdateStatus.COMPLETED:
                 raise ServiceResponseException("Delete failed")
 
+    @override
     async def get_nearest_matches(
         self,
         collection_name: str,
         embedding: ndarray,
         limit: int,
         min_relevance_score: float,
         with_embeddings: bool = False,
@@ -257,14 +230,15 @@
                     timestamp=result.payload["_timestamp"],
                 ),
                 result.score,
             )
             for result in match_results
         ]
 
+    @override
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float,
         with_embedding: bool = False,
     ) -> tuple[MemoryRecord, float]:
@@ -281,20 +255,21 @@
         self,
         collection_name: str,
         payload_id: str,
         with_embedding: bool = False,
     ) -> qdrant_models.ScoredPoint | None:
         """Gets an existing record based upon payload id.
 
-        Arguments:
-            collection_name {str} -- The name of the collection.
-            payload_id {str} -- The payload id to search for.
+        Args:
+            collection_name (str): The name of the collection.
+            payload_id (str): The payload id to search for.
+            with_embedding (bool): If true, the embedding will be returned in the memory records.
 
         Returns:
-            Optional[ScoredPoint] -- The existing record if found; otherwise, None.
+            Optional[ScoredPoint]: The existing record if found; otherwise, None.
         """
         filter = qdrant_models.Filter(
             must=[
                 qdrant_models.FieldCondition(
                     key="_id",
                     match=qdrant_models.MatchText(text=payload_id),
                 )
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/redis/README.md` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/redis/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/redis/redis_memory_store.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/redis/redis_memory_store.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 @experimental_class
 class RedisMemoryStore(MemoryStoreBase):
-    """A memory store implementation using Redis"""
+    """A memory store implementation using Redis."""
 
     _database: "redis.Redis"
     _ft: "redis.Redis.ft"
     # Without RedisAI, it is currently not possible to retrieve index-specific vector attributes to have
     # fully independent collections.
     _query_dialect: int
     _vector_distance_metric: str
@@ -51,27 +51,27 @@
         vector_size: int = 1536,
         vector_distance_metric: str = "COSINE",
         vector_type: str = "FLOAT32",
         vector_index_algorithm: str = "HNSW",
         query_dialect: int = 2,
         env_file_path: str | None = None,
     ) -> None:
-        """
-        RedisMemoryStore is an abstracted interface to interact with a Redis node connection.
+        """RedisMemoryStore is an abstracted interface to interact with a Redis node connection.
+
         See documentation about connections: https://redis-py.readthedocs.io/en/stable/connections.html
-        See documentation about vector attributes: https://redis.io/docs/stack/search/reference/vectors
+        See documentation about vector attributes: https://redis.io/docs/stack/search/reference/vectors.
 
-        Arguments:
-            connection_string {str} -- Provide connection URL to a Redis instance
-            vector_size {str} -- Size of vectors, defaults to 1536
-            vector_distance_metric {str} -- Metric for measuring vector distances, defaults to COSINE
-            vector_type {str} -- Vector type, defaults to FLOAT32
-            vector_index_algorithm {str} -- Indexing algorithm for vectors, defaults to HNSW
-            query_dialect {int} -- Query dialect, must be 2 or greater for vector similarity searching, defaults to 2
-            env_file_path {str | None} -- Use the environment settings file as a fallback to
+        Args:
+            connection_string (str): Provide connection URL to a Redis instance
+            vector_size (str): Size of vectors, defaults to 1536
+            vector_distance_metric (str): Metric for measuring vector distances, defaults to COSINE
+            vector_type (str): Vector type, defaults to FLOAT32
+            vector_index_algorithm (str): Indexing algorithm for vectors, defaults to HNSW
+            query_dialect (int): Query dialect, must be 2 or greater for vector similarity searching, defaults to 2
+            env_file_path (str | None): Use the environment settings file as a fallback to
                 environment variables, defaults to False
         """
         redis_settings = None
         try:
             redis_settings = RedisSettings.create(env_file_path=env_file_path)
         except ValidationError as e:
             logger.warning(f"Failed to load Redis pydantic settings: {e}")
@@ -92,30 +92,27 @@
         self._vector_distance_metric = vector_distance_metric
         self._vector_index_algorithm = vector_index_algorithm
         self._vector_type_str = vector_type
         self._vector_type = np.float32 if vector_type == "FLOAT32" else np.float64
         self._vector_size = vector_size
 
     async def close(self):
-        """
-        Closes the Redis database connection
-        """
+        """Closes the Redis database connection."""
         logger.info("Closing Redis connection")
         self._database.close()
 
     async def create_collection(self, collection_name: str) -> None:
-        """
-        Creates a collection, implemented as a Redis index containing hashes
-        prefixed with "collection_name:".
+        """Creates a collection.
+
+        Implemented as a Redis index containing hashes prefixed with "collection_name:".
         If a collection of the name exists, it is left unchanged.
 
-        Arguments:
-            collection_name {str} -- Name for a collection of embeddings
+        Args:
+            collection_name (str): Name for a collection of embeddings
         """
-
         if await self.does_collection_exist(collection_name):
             logger.info(f'Collection "{collection_name}" already exists.')
         else:
             index_def = IndexDefinition(prefix=f"{collection_name}:", index_type=IndexType.HASH)
             schema = (
                 TextField(name="key"),
                 TextField(name="metadata"),
@@ -133,69 +130,66 @@
 
             try:
                 self._ft(collection_name).create_index(definition=index_def, fields=schema)
             except Exception as e:
                 raise ServiceResponseException(f"Failed to create collection {collection_name}") from e
 
     async def get_collections(self) -> list[str]:
-        """
-        Returns a list of names of all collection names present in the data store.
+        """Returns a list of names of all collection names present in the data store.
 
         Returns:
-            List[str] -- list of collection names
+            List[str]: list of collection names
         """
         # Note: FT._LIST is a temporary command that may be deprecated in the future according to Redis
         return [name.decode() for name in self._database.execute_command("FT._LIST")]
 
     async def delete_collection(self, collection_name: str, delete_records: bool = True) -> None:
-        """
-        Deletes a collection from the data store.
-        If the collection does not exist, the database is left unchanged.
+        """Deletes a collection from the data store.
 
-        Arguments:
-            collection_name {str} -- Name for a collection of embeddings
-            delete_records {bool} -- Delete all data associated with the collection, default to True
+        If the collection does not exist, the database is left unchanged.
 
+        Args:
+            collection_name (str): Name for a collection of embeddings
+            delete_records (bool): Delete all data associated with the collection, default to True
         """
         if await self.does_collection_exist(collection_name):
             self._ft(collection_name).dropindex(delete_documents=delete_records)
 
     async def does_collection_exist(self, collection_name: str) -> bool:
-        """
-        Determines if a collection exists in the data store.
+        """Determines if a collection exists in the data store.
 
-        Arguments:
-            collection_name {str} -- Name for a collection of embeddings
+        Args:
+            collection_name (str): Name for a collection of embeddings
 
         Returns:
             True if the collection exists, False if not
         """
         try:
             self._ft(collection_name).info()
             return True
         except ResponseError:
             return False
 
     async def upsert(self, collection_name: str, record: MemoryRecord) -> str:
-        """
-        Upsert a memory record into the data store. Does not guarantee that the collection exists.
+        """Upsert a memory record into the data store.
+
+        Does not guarantee that the collection exists.
             * If the record already exists, it will be updated.
             * If the record does not exist, it will be created.
 
         Note: if the record do not have the same dimensionality configured for the collection,
         it will not be detected to belong to the collection in Redis.
 
-        Arguments:
-            collection_name {str} -- Name for a collection of embeddings
-            record {MemoryRecord} -- Memory record to upsert
+        Args:
+            collection_name (str): Name for a collection of embeddings
+            record (MemoryRecord): Memory record to upsert
 
-        Returns
-            str -- Redis key associated with the upserted memory record
+        Returns:
+            str: Redis key associated with the upserted memory record
         """
-
         if not await self.does_collection_exist(collection_name):
             raise ServiceResourceNotFoundError(f'Collection "{collection_name}" does not exist')
 
         # Typical Redis key structure: collection_name:{some identifier}
         record._key = get_redis_key(collection_name, record._id)
 
         # Overwrites previous data or inserts new key if not present
@@ -206,50 +200,48 @@
                 mapping=serialize_record_to_redis(record, self._vector_type),
             )
             return record._key
         except Exception as e:
             raise ServiceResponseException("Could not upsert messages.") from e
 
     async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
-        """
-        Upserts a group of memory records into the data store. Does not guarantee that the collection exists.
+        """Upserts a group of memory records into the data store.
+
+        Does not guarantee that the collection exists.
             * If the record already exists, it will be updated.
             * If the record does not exist, it will be created.
 
         Note: if the records do not have the same dimensionality configured for the collection,
         they will not be detected to belong to the collection in Redis.
 
-        Arguments:
-            collection_name {str} -- Name for a collection of embeddings
-            records {List[MemoryRecord]} -- List of memory records to upsert
+        Args:
+            collection_name (str): Name for a collection of embeddings
+            records (List[MemoryRecord]): List of memory records to upsert
 
-        Returns
-            List[str] -- Redis keys associated with the upserted memory records
+        Returns:
+            List[str]: Redis keys associated with the upserted memory records
         """
-
         keys = list()
         for record in records:
             record_key = await self.upsert(collection_name, record)
             keys.append(record_key)
 
         return keys
 
     async def get(self, collection_name: str, key: str, with_embedding: bool = False) -> MemoryRecord:
-        """
-        Gets a memory record from the data store. Does not guarantee that the collection exists.
+        """Gets a memory record from the data store. Does not guarantee that the collection exists.
 
-        Arguments:
-            collection_name {str} -- Name for a collection of embeddings
-            key {str} -- ID associated with the memory to get
-            with_embedding {bool} -- Include embedding with the memory record, default to False
+        Args:
+            collection_name (str): Name for a collection of embeddings
+            key (str): ID associated with the memory to get
+            with_embedding (bool): Include embedding with the memory record, default to False
 
         Returns:
-            MemoryRecord -- The memory record if found, else None
+            MemoryRecord: The memory record if found, else None
         """
-
         if not await self.does_collection_exist(collection_name):
             raise ServiceResourceNotFoundError(f'Collection "{collection_name}" does not exist')
 
         internal_key = get_redis_key(collection_name, key)
         fields = self._database.hgetall(internal_key)
 
         # Did not find the record
@@ -260,81 +252,80 @@
         record._key = internal_key
 
         return record
 
     async def get_batch(
         self, collection_name: str, keys: list[str], with_embeddings: bool = False
     ) -> list[MemoryRecord]:
-        """
-        Gets a batch of memory records from the data store. Does not guarantee that the collection exists.
+        """Gets a batch of memory records from the data store.
 
-        Arguments:
-            collection_name {str} -- Name for a collection of embeddings
-            keys {List[str]} -- IDs associated with the memory records to get
-            with_embedding {bool} -- Include embeddings with the memory records, default to False
+        Does not guarantee that the collection exists.
+
+        Args:
+            collection_name (str): Name for a collection of embeddings
+            keys (List[str]): IDs associated with the memory records to get
+            with_embeddings (bool): Include embeddings with the memory records, default to False
 
         Returns:
-            List[MemoryRecord] -- The memory records if found, else an empty list
+            List[MemoryRecord]: The memory records if found, else an empty list
         """
-
         records = list()
         for key in keys:
             record = await self.get(collection_name, key, with_embeddings)
             if record:
                 records.append(record)
 
         return records
 
     async def remove(self, collection_name: str, key: str) -> None:
-        """
-        Removes a memory record from the data store. Does not guarantee that the collection exists.
+        """Removes a memory record from the data store.
+
+        Does not guarantee that the collection exists.
         If the key does not exist, do nothing.
 
-        Arguments:
-            collection_name {str} -- Name for a collection of embeddings
-            key {str} -- ID associated with the memory to remove
+        Args:
+            collection_name (str): Name for a collection of embeddings
+            key (str): ID associated with the memory to remove
         """
         if not await self.does_collection_exist(collection_name):
             raise ServiceResourceNotFoundError(f'Collection "{collection_name}" does not exist')
 
         self._database.delete(get_redis_key(collection_name, key))
 
     async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
-        """
-        Removes a batch of memory records from the data store. Does not guarantee that the collection exists.
+        """Removes a batch of memory records from the data store. Does not guarantee that the collection exists.
 
-        Arguments:
-            collection_name {str} -- Name for a collection of embeddings
-            keys {List[str]} -- IDs associated with the memory records to remove
+        Args:
+            collection_name (str): Name for a collection of embeddings
+            keys (List[str]): IDs associated with the memory records to remove
         """
         if not await self.does_collection_exist(collection_name):
             raise ServiceResourceNotFoundError(f'Collection "{collection_name}" does not exist')
 
         self._database.delete(*[get_redis_key(collection_name, key) for key in keys])
 
     async def get_nearest_matches(
         self,
         collection_name: str,
         embedding: ndarray,
         limit: int,
         min_relevance_score: float = 0.0,
         with_embeddings: bool = False,
     ) -> list[tuple[MemoryRecord, float]]:
-        """
-        Get the nearest matches to an embedding using the configured similarity algorithm.
+        """Get the nearest matches to an embedding using the configured similarity algorithm.
 
-        Arguments:
-            collection_name {str} -- Name for a collection of embeddings
-            embedding {ndarray} -- Embedding to find the nearest matches to
-            limit {int} -- Maximum number of matches to return
-            min_relevance_score {float} -- Minimum relevance score of the matches, default to 0.0
-            with_embeddings {bool} -- Include embeddings in the resultant memory records, default to False
+        Args:
+            collection_name (str): Name for a collection of embeddings
+            embedding (ndarray): Embedding to find the nearest matches to
+            limit (int): Maximum number of matches to return
+            min_relevance_score (float): Minimum relevance score of the matches, default to 0.0
+            with_embeddings (bool): Include embeddings in the resultant memory records, default to False
 
         Returns:
-            List[Tuple[MemoryRecord, float]] -- Records and their relevance scores by descending
+            List[Tuple[MemoryRecord, float]]: Records and their relevance scores by descending
                 order, or an empty list if no relevant matches are found
         """
         if not await self.does_collection_exist(collection_name):
             raise ServiceResourceNotFoundError(f'Collection "{collection_name}" does not exist')
 
         # Perform a k-nearest neighbors query, score by similarity
         query = (
@@ -368,25 +359,24 @@
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float = 0.0,
         with_embedding: bool = False,
     ) -> tuple[MemoryRecord, float]:
-        """
-        Get the nearest match to an embedding using the configured similarity algorithm.
+        """Get the nearest match to an embedding using the configured similarity algorithm.
 
-        Arguments:
-            collection_name {str} -- Name for a collection of embeddings
-            embedding {ndarray} -- Embedding to find the nearest match to
-            min_relevance_score {float} -- Minimum relevance score of the match, default to 0.0
-            with_embedding {bool} -- Include embedding in the resultant memory record, default to False
+        Args:
+            collection_name (str): Name for a collection of embeddings
+            embedding (ndarray): Embedding to find the nearest match to
+            min_relevance_score (float): Minimum relevance score of the match, default to 0.0
+            with_embedding (bool): Include embedding in the resultant memory record, default to False
 
         Returns:
-            Tuple[MemoryRecord, float] -- Record and the relevance score, or None if not found
+            Tuple[MemoryRecord, float]: Record and the relevance score, or None if not found
         """
         matches = await self.get_nearest_matches(
             collection_name=collection_name,
             embedding=embedding,
             limit=1,
             min_relevance_score=min_relevance_score,
             with_embeddings=with_embedding,
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/redis/redis_settings.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/redis/redis_settings.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 
 from semantic_kernel.connectors.memory.memory_settings_base import BaseModelSettings
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
 @experimental_class
 class RedisSettings(BaseModelSettings):
-    """Redis model settings
+    """Redis model settings.
 
-    Optional:
-    - connection_string: str | None - Redis connection string
-        (Env var REDIS_CONNECTION_STRING)
+    Args:
+    - connection_string (str | None):
+        Redis connection string (Env var REDIS_CONNECTION_STRING)
     """
 
     connection_string: SecretStr | None = None
 
     class Config(BaseModelSettings.Config):
+        """Model configuration."""
+
         env_prefix = "REDIS_"
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/redis/utils.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/redis/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,42 +8,41 @@
 from redis import Redis
 from redis.commands.search.document import Document
 
 from semantic_kernel.memory.memory_record import MemoryRecord
 
 
 def get_redis_key(collection_name: str, record_id: str) -> str:
-    """
-    Returns the Redis key for an element called record_id within collection_name
+    """Returns the Redis key for an element called record_id within collection_name.
 
-    Arguments:
-        collection_name {str} -- Name for a collection of embeddings
-        record_id {str} -- ID associated with a memory record
+    Args:
+        collection_name (str): Name for a collection of embeddings
+        record_id (str): ID associated with a memory record
 
     Returns:
-        str -- Redis key in the format collection_name:id
+        str: Redis key in the format collection_name:id
     """
     return f"{collection_name}:{record_id}"
 
 
 def split_redis_key(redis_key: str) -> tuple[str, str]:
-    """
-    Split a Redis key into its collection name and record ID
+    """Split a Redis key into its collection name and record ID.
 
-    Arguments:
-        collection_name {str} -- Redis key
+    Args:
+        redis_key (str): Redis key
 
     Returns:
-        Tuple[str, str] -- Tuple of the collection name and ID
+        tuple[str, str]: Tuple of the collection name and ID
     """
     collection, record_id = redis_key.split(":")
     return collection, record_id
 
 
 def serialize_record_to_redis(record: MemoryRecord, vector_type: np.dtype) -> dict[str, Any]:
+    """Serialize a MemoryRecord to Redis fields."""
     all_metadata = {
         "is_reference": record._is_reference,
         "external_source_name": record._external_source_name or "",
         "id": record._id or "",
         "description": record._description or "",
         "text": record._text or "",
         "additional_metadata": record._additional_metadata or "",
@@ -55,14 +54,15 @@
         "metadata": json.dumps(all_metadata),
         "embedding": (record._embedding.astype(vector_type).tobytes() if record._embedding is not None else ""),
     }
     return redis_mapping
 
 
 def deserialize_redis_to_record(fields: dict[str, Any], vector_type: np.dtype, with_embedding: bool) -> MemoryRecord:
+    """Deserialize Redis fields to a MemoryRecord."""
     metadata = json.loads(fields[b"metadata"])
     record = MemoryRecord(
         id=metadata["id"],
         is_reference=True if metadata["is_reference"] is True else False,
         description=metadata["description"],
         external_source_name=metadata["external_source_name"],
         text=metadata["text"],
@@ -79,14 +79,15 @@
 
     return record
 
 
 def deserialize_document_to_record(
     database: Redis, doc: Document, vector_type: np.dtype, with_embedding: bool
 ) -> MemoryRecord:
+    """Deserialize document to a MemoryRecord."""
     # Document's ID refers to the Redis key
     redis_key = doc["id"]
     _, id_str = split_redis_key(redis_key)
 
     metadata = json.loads(doc["metadata"])
     record = MemoryRecord(
         id=id_str,
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 _collection_file_extensions: dict[_CollectionFileType, str] = {
     _CollectionFileType.USEARCH: ".usearch",
     _CollectionFileType.PARQUET: ".parquet",
 }
 
 
 def memoryrecords_to_pyarrow_table(records: list[MemoryRecord]) -> pa.Table:
-    """Convert a list of `MemoryRecord` to a PyArrow Table"""
+    """Convert a list of `MemoryRecord` to a PyArrow Table."""
     records_pylist = [
         {attr: getattr(record, "_" + attr) for attr in _embeddings_data_schema.names} for record in records
     ]
     return pa.Table.from_pylist(records_pylist, schema=_embeddings_data_schema)
 
 
 def pyarrow_table_to_memoryrecords(table: pa.Table, vectors: ndarray | None = None) -> list[MemoryRecord]:
@@ -118,16 +118,15 @@
 
 @experimental_class
 class USearchMemoryStore(MemoryStoreBase):
     def __init__(
         self,
         persist_directory: os.PathLike | None = None,
     ) -> None:
-        """
-        Create a USearchMemoryStore instance.
+        """Create a USearchMemoryStore instance.
 
         This store helps searching embeddings with USearch, keeping collections in memory.
         To save collections to disk, provide the `persist_directory` param.
         Collections are saved when `close` is called.
 
         To both save collections and free up memory, call `close`.
         When `USearchMemoryStore` is used with a context manager, this will happen automatically.
@@ -140,16 +139,15 @@
         self._persist_directory = Path(persist_directory) if persist_directory is not None else None
 
         self._collections: dict[str, _USearchCollection] = {}
         if self._persist_directory:
             self._collections = self._read_collections_from_dir()
 
     def _get_collection_path(self, collection_name: str, *, file_type: _CollectionFileType) -> Path:
-        """
-        Get the path for the given collection name and file type.
+        """Get the path for the given collection name and file type.
 
         Args:
             collection_name (str): Name of the collection.
             file_type (_CollectionFileType): The file type.
 
         Returns:
             Path: Path to the collection file.
@@ -276,21 +274,23 @@
 
         Returns:
             List[str]: List of collection names.
         """
         return list(self._collections.keys())
 
     async def delete_collection(self, collection_name: str) -> None:
+        """Delete collection by name."""
         collection_name = collection_name.lower()
         collection = self._collections.pop(collection_name, None)
         if collection:
             collection.embeddings_index.reset()
         return None
 
     async def does_collection_exist(self, collection_name: str) -> bool:
+        """Check if collection exists."""
         collection_name = collection_name.lower()
         return collection_name in self._collections
 
     async def upsert(self, collection_name: str, record: MemoryRecord) -> str:
         """Upsert single MemoryRecord and return its ID."""
         collection_name = collection_name.lower()
         res = await self.upsert_batch(collection_name=collection_name, records=[record])
@@ -480,15 +480,15 @@
 
         Args:
             collection_name (str): Name of the collection to search within.
             embedding (ndarray): The embedding vector to search for.
             limit (int): maximum amount of embeddings to search for.
             min_relevance_score (float, optional): The minimum relevance score for vectors. Supposed to be from 0 to 1.
                 Only vectors with greater or equal relevance score are returned. Defaults to 0.0.
-            with_embedding (bool, optional): If True, include the embedding in the result. Defaults to True.
+            with_embeddings (bool, optional): If True, include the embedding in the result. Defaults to True.
             threads (int, optional): Optimal number of cores to use. Defaults to 0.
             exact (bool, optional): Perform exhaustive linear-time exact search. Defaults to False.
             log (Union[str, bool], optional): Whether to print the progress bar. Defaults to False.
             batch_size (int, optional): Number of vectors to process at once. Defaults to 0.
 
         Raises:
             KeyError: if a collection with specified name does not exist
@@ -503,15 +503,15 @@
             vectors=embedding,
             count=limit,
             threads=threads,
             exact=exact,
             log=log,
         )
 
-        assert isinstance(result, Matches)
+        # assert isinstance(result, Matches)  # nosec
 
         relevance_score = 1 / (result.distances + 1)
         filtered_labels = result.keys[np.where(relevance_score >= min_relevance_score)[0]]
 
         filtered_vectors: np.ndarray | None = None
         if with_embeddings:
             filtered_vectors = ucollection.embeddings_index.get(filtered_labels)
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,18 +71,17 @@
     url: str = None
     api_key: str = None
 
 
 @experimental_class
 class WeaviateMemoryStore(MemoryStoreBase):
     class FieldMapper:
-        """
-        This inner class is responsible for mapping attribute names between
-        the SK's memory record and weaviate's schema. It provides methods
-        for converting between the two naming conventions.
+        """This maps attribute names between the SK's memory record and weaviate's schema.
+
+        It provides methods for converting between the two naming conventions.
         """
 
         SK_TO_WEAVIATE_MAPPING = {
             "_key": "key",
             "_timestamp": "timestamp",
             "_is_reference": "isReference",
             "_external_source_name": "externalSourceName",
@@ -93,40 +92,39 @@
             "_embedding": "vector",
         }
 
         WEAVIATE_TO_SK_MAPPING = {v: k for k, v in SK_TO_WEAVIATE_MAPPING.items()}
 
         @classmethod
         def sk_to_weaviate(cls, sk_dict):
+            """Used to convert a MemoryRecord to a dict of attribute-values that can be used by Weaviate."""
             return {
                 cls.SK_TO_WEAVIATE_MAPPING.get(k, k): v for k, v in sk_dict.items() if k in cls.SK_TO_WEAVIATE_MAPPING
             }
 
         @classmethod
         def weaviate_to_sk(cls, weaviate_dict):
+            """Used to convert a Weaviate object to a dict that can be used to initialize a MemoryRecord."""
             return {
                 cls.WEAVIATE_TO_SK_MAPPING.get(k, k): v
                 for k, v in weaviate_dict.items()
                 if k in cls.WEAVIATE_TO_SK_MAPPING
             }
 
         @classmethod
         def remove_underscore_prefix(cls, sk_dict):
-            """
-            Used to initialize a MemoryRecord from a SK's dict of private attribute-values.
-            """
+            """Used to initialize a MemoryRecord from a SK's dict of private attribute-values."""
             return {key.lstrip("_"): value for key, value in sk_dict.items()}
 
     def __init__(self, config: WeaviateConfig | None = None, env_file_path: str | None = None):
-        """Initializes a new instance of the WeaviateMemoryStore
+        """Initializes a new instance of the WeaviateMemoryStore.
 
         Optional parameters:
-        - env_file_path {str | None} -- Whether to use the environment settings (.env) file. Defaults to False.
+        - env_file_path (str | None): Whether to use the environment settings (.env) file. Defaults to False.
         """
-
         # Initialize settings from environment variables or defaults defined in WeaviateSettings
         weaviate_settings = None
         try:
             weaviate_settings = WeaviateSettings.create(env_file_path=env_file_path)
         except ValidationError as e:
             logger.warning(f"Failed to load WeaviateSettings pydantic settings: {e}")
 
@@ -136,16 +134,15 @@
         else:
             self.settings = weaviate_settings
 
         self.settings.validate_settings()
         self.client = self._initialize_client()
 
     def merge_settings(self, default_settings: WeaviateSettings, config: WeaviateConfig) -> WeaviateSettings:
-        """
-        Merges default settings with configuration provided through WeaviateConfig.
+        """Merges default settings with configuration provided through WeaviateConfig.
 
         This function allows for manual overriding of settings from the config parameter.
         """
         return WeaviateSettings(
             url=config.url or (str(default_settings.url) if default_settings and default_settings.url else None),
             api_key=config.api_key
             or (default_settings.api_key.get_secret_value() if default_settings and default_settings.api_key else None),
@@ -153,44 +150,47 @@
                 config.use_embed
                 if config.use_embed is not None
                 else (default_settings.use_embed if default_settings and default_settings.use_embed else False)
             ),
         )
 
     def _initialize_client(self) -> weaviate.Client:
-        """
-        Initializes the Weaviate client based on the combined settings.
-        """
+        """Initializes the Weaviate client based on the combined settings."""
         if self.settings.use_embed:
             return weaviate.Client(embedded_options=weaviate.EmbeddedOptions())
 
         if self.settings.api_key:
             return weaviate.Client(
                 url=self.settings.url, auth_client_secret=weaviate.auth.AuthApiKey(api_key=self.settings.api_key)
             )
 
         return weaviate.Client(url=self.settings.url)
 
     async def create_collection(self, collection_name: str) -> None:
+        """Creates a new collection in Weaviate."""
         schema = SCHEMA.copy()
         schema["class"] = collection_name
         await asyncio.get_running_loop().run_in_executor(None, self.client.schema.create_class, schema)
 
     async def get_collections(self) -> list[str]:
+        """Returns a list of all collections in Weaviate."""
         schemas = await asyncio.get_running_loop().run_in_executor(None, self.client.schema.get)
         return [schema["class"] for schema in schemas["classes"]]
 
     async def delete_collection(self, collection_name: str) -> bool:
+        """Deletes a collection in Weaviate."""
         await asyncio.get_running_loop().run_in_executor(None, self.client.schema.delete_class, collection_name)
 
     async def does_collection_exist(self, collection_name: str) -> bool:
+        """Checks if a collection exists in Weaviate."""
         collections = await self.get_collections()
         return collection_name in collections
 
     async def upsert(self, collection_name: str, record: MemoryRecord) -> str:
+        """Upserts a record into Weaviate."""
         weaviate_record = self.FieldMapper.sk_to_weaviate(vars(record))
 
         vector = weaviate_record.pop("vector", None)
         weaviate_id = weaviate.util.generate_uuid5(weaviate_record, collection_name)
 
         return await asyncio.get_running_loop().run_in_executor(
             None,
@@ -198,14 +198,16 @@
             weaviate_record,
             collection_name,
             weaviate_id,
             vector,
         )
 
     async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
+        """Upserts a batch of records into Weaviate."""
+
         def _upsert_batch_inner():
             results = []
             with self.client.batch as batch:
                 for record in records:
                     weaviate_record = self.FieldMapper.sk_to_weaviate(vars(record))
                     vector = weaviate_record.pop("vector", None)
                     weaviate_id = weaviate.util.generate_uuid5(weaviate_record, collection_name)
@@ -218,19 +220,21 @@
                     results.append(weaviate_id)
 
             return results
 
         return await asyncio.get_running_loop().run_in_executor(None, _upsert_batch_inner)
 
     async def get(self, collection_name: str, key: str, with_embedding: bool) -> MemoryRecord:
+        """Gets a record from Weaviate by key."""
         # Call the batched version with a single key
         results = await self.get_batch(collection_name, [key], with_embedding)
         return results[0] if results else None
 
     async def get_batch(self, collection_name: str, keys: list[str], with_embedding: bool) -> list[MemoryRecord]:
+        """Gets a batch of records from Weaviate by keys."""
         queries = self._build_multi_get_query(collection_name, keys, with_embedding)
 
         results = await asyncio.get_running_loop().run_in_executor(None, self.client.query.multi_get(queries).do)
 
         get_dict = results.get("data", {}).get("Get", {})
 
         memory_records = [
@@ -263,17 +267,19 @@
         vector = weaviate_doc_copy.pop("_additional", {}).get("vector")
         weaviate_doc_copy["vector"] = np.array(vector) if vector else None
         sk_doc = self.FieldMapper.weaviate_to_sk(weaviate_doc_copy)
         mem_vals = self.FieldMapper.remove_underscore_prefix(sk_doc)
         return MemoryRecord(**mem_vals)
 
     async def remove(self, collection_name: str, key: str) -> None:
+        """Removes a record from Weaviate by key."""
         await self.remove_batch(collection_name, [key])
 
     async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
+        """Removes a batch of records from Weaviate by keys."""
         # TODO: Use In operator when it's available
         #       (https://github.com/weaviate/weaviate/issues/2387)
         #       and handle max delete objects
         #       (https://weaviate.io/developers/weaviate/api/rest/batch#maximum-number-of-deletes-per-query)
         for key in keys:
             where = {
                 "path": ["key"],
@@ -289,14 +295,15 @@
         self,
         collection_name: str,
         embedding: np.ndarray,
         limit: int,
         min_relevance_score: float,
         with_embeddings: bool,
     ) -> list[tuple[MemoryRecord, float]]:
+        """Gets the nearest matches to an embedding in Weaviate."""
         nearVector = {
             "vector": embedding,
             "certainty": min_relevance_score,
         }
 
         additional = ["certainty"]
         if with_embeddings:
@@ -328,14 +335,15 @@
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: np.ndarray,
         min_relevance_score: float,
         with_embedding: bool,
     ) -> tuple[MemoryRecord, float]:
+        """Gets the nearest match to an embedding in Weaviate."""
         results = await self.get_nearest_matches(
             collection_name,
             embedding,
             limit=1,
             min_relevance_score=min_relevance_score,
             with_embeddings=with_embedding,
         )
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/memory/weaviate/weaviate_settings.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/memory/weaviate/weaviate_settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,26 +5,29 @@
 from semantic_kernel.connectors.memory.memory_settings_base import BaseModelSettings
 from semantic_kernel.kernel_pydantic import HttpsUrl
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
 @experimental_class
 class WeaviateSettings(BaseModelSettings):
-    """Weaviate model settings
+    """Weaviate model settings.
 
-    Optional:
-    - url: HttpsUrl | None - Weaviate URL (Env var WEAVIATE_URL)
-    - api_key: SecretStr | None - Weaviate token (Env var WEAVIATE_API_KEY)
-    - use_embed: bool - Whether to use the client embedding options
-        (Env var WEAVIATE_USE_EMBED)
+    Args:
+        url: HttpsUrl | None - Weaviate URL (Env var WEAVIATE_URL)
+        api_key: SecretStr | None - Weaviate token (Env var WEAVIATE_API_KEY)
+        use_embed: bool - Whether to use the client embedding options
+          (Env var WEAVIATE_USE_EMBED)
     """
 
     url: HttpsUrl | None = None
     api_key: SecretStr | None = None
     use_embed: bool = False
 
     class Config(BaseModelSettings.Config):
+        """Configuration for the Weaviate model settings."""
+
         env_prefix = "WEAVIATE_"
 
     def validate_settings(self):
+        """Validate the Weaviate settings."""
         if not self.use_embed and not self.url:
             raise ValueError("Weaviate config must have either url or use_embed set")
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/openai_plugin/__init__.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/openai_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/openai_plugin/openai_utils.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/openai_plugin/openai_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 class OpenAIUtils:
     """Utility functions for OpenAI plugins."""
 
     @staticmethod
     def parse_openai_manifest_for_openapi_spec_url(plugin_json: dict[str, Any]) -> str:
         """Extract the OpenAPI Spec URL from the plugin JSON."""
-
         try:
             api_type = plugin_json["api"]["type"]
         except KeyError as ex:
             raise PluginInitializationError("OpenAI manifest is missing the API type.") from ex
 
         if api_type != "openapi":
             raise PluginInitializationError("OpenAI manifest is not of type OpenAPI.")
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation.py`

 * *Files 15% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         path: str,
         summary: str | None = None,
         description: str | None = None,
         params: list["RestApiOperationParameter"] | None = None,
         request_body: "RestApiOperationPayload | None" = None,
         responses: dict[str, "RestApiOperationExpectedResponse"] | None = None,
     ):
+        """Initialize the RestApiOperation."""
         self.id = id
         self.method = method.upper()
         self.server_url = server_url
         self.path = path
         self.summary = summary
         self.description = description
         self.parameters = params
@@ -74,14 +75,15 @@
             base_path = parsed_base.path + "/"
         else:
             base_path = parsed_base.path
         full_path = urljoin(base_path, path.lstrip("/"))
         return urlunparse(parsed_base._replace(path=full_path))
 
     def build_headers(self, arguments: dict[str, Any]) -> dict[str, str]:
+        """Build the headers for the operation."""
         headers = {}
 
         parameters = [p for p in self.parameters if p.location == RestApiOperationParameterLocation.HEADER]
 
         for parameter in parameters:
             argument = arguments.get(parameter.name)
 
@@ -94,19 +96,21 @@
                 continue
 
             headers[parameter.name] = str(argument)
 
         return headers
 
     def build_operation_url(self, arguments, server_url_override=None, api_host_url=None):
+        """Build the URL for the operation."""
         server_url = self.get_server_url(server_url_override, api_host_url)
         path = self.build_path(self.path, arguments)
         return urljoin(server_url.geturl(), path.lstrip("/"))
 
     def get_server_url(self, server_url_override=None, api_host_url=None):
+        """Get the server URL for the operation."""
         if server_url_override is not None and server_url_override.geturl() != b"":
             server_url_string = server_url_override.geturl()
         else:
             server_url_string = (
                 self.server_url.geturl()
                 if self.server_url
                 else api_host_url.geturl() if api_host_url else self._raise_invalid_operation_exception()
@@ -115,28 +119,30 @@
         # make sure the base URL ends with a trailing slash
         if not server_url_string.endswith("/"):
             server_url_string += "/"
 
         return urlparse(server_url_string)
 
     def build_path(self, path_template: str, arguments: dict[str, Any]) -> str:
+        """Build the path for the operation."""
         parameters = [p for p in self.parameters if p.location == RestApiOperationParameterLocation.PATH]
         for parameter in parameters:
             argument = arguments.get(parameter.name)
             if argument is None:
                 if parameter.is_required:
                     raise FunctionExecutionException(
                         f"No argument is provided for the `{parameter.name}` "
                         f"required parameter of the operation - `{self.id}`."
                     )
                 continue
             path_template = path_template.replace(f"{{{parameter.name}}}", str(argument))
         return path_template
 
     def build_query_string(self, arguments: dict[str, Any]) -> str:
+        """Build the query string for the operation."""
         segments = []
         parameters = [p for p in self.parameters if p.location == RestApiOperationParameterLocation.QUERY]
         for parameter in parameters:
             argument = arguments.get(parameter.name)
             if argument is None:
                 if parameter.is_required:
                     raise FunctionExecutionException(
@@ -144,22 +150,24 @@
                         f"required parameter of the operation - `{self.id}`."
                     )
                 continue
             segments.append((parameter.name, argument))
         return urlencode(segments)
 
     def replace_invalid_symbols(self, parameter_name):
+        """Replace invalid symbols in the parameter name with underscores."""
         return RestApiOperation.INVALID_SYMBOLS_REGEX.sub("_", parameter_name)
 
     def get_parameters(
         self,
         operation: "RestApiOperation",
         add_payload_params_from_metadata: bool = True,
         enable_payload_spacing: bool = False,
     ) -> list["RestApiOperationParameter"]:
+        """Get the parameters for the operation."""
         params = list(operation.parameters)
         if operation.request_body is not None:
             params.extend(
                 self.get_payload_parameters(
                     operation=operation,
                     use_parameters_from_metadata=add_payload_params_from_metadata,
                     enable_namespacing=enable_payload_spacing,
@@ -168,14 +176,15 @@
 
         for parameter in params:
             parameter.alternative_name = self.replace_invalid_symbols(parameter.name)
 
         return params
 
     def create_payload_artificial_parameter(self, operation: "RestApiOperation") -> "RestApiOperationParameter":
+        """Create an artificial parameter for the REST API request body."""
         return RestApiOperationParameter(
             name=self.PAYLOAD_ARGUMENT_NAME,
             type=(
                 "string"
                 if operation.request_body
                 and operation.request_body.media_type == RestApiOperation.MEDIA_TYPE_TEXT_PLAIN
                 else "object"
@@ -184,14 +193,15 @@
             location=RestApiOperationParameterLocation.BODY,
             style=RestApiOperationParameterStyle.SIMPLE,
             description=operation.request_body.description if operation.request_body else "REST API request body.",
             schema=operation.request_body.schema if operation.request_body else None,
         )
 
     def create_content_type_artificial_parameter(self) -> "RestApiOperationParameter":
+        """Create an artificial parameter for the content type of the REST API request body."""
         return RestApiOperationParameter(
             name=self.CONTENT_TYPE_ARGUMENT_NAME,
             type="string",
             is_required=False,
             location=RestApiOperationParameterLocation.BODY,
             style=RestApiOperationParameterStyle.SIMPLE,
             description="Content type of REST API request body.",
@@ -229,14 +239,15 @@
                 self._get_parameters_from_payload_metadata(property.properties, enable_namespacing, parameter_name)
             )
         return parameters
 
     def get_payload_parameters(
         self, operation: "RestApiOperation", use_parameters_from_metadata: bool, enable_namespacing: bool
     ):
+        """Get the payload parameters for the operation."""
         if use_parameters_from_metadata:
             if operation.request_body is None:
                 raise Exception(
                     f"Payload parameters cannot be retrieved from the `{operation.Id}` "
                     f"operation payload metadata because it is missing."
                 )
             if operation.request_body.media_type == RestApiOperation.MEDIA_TYPE_TEXT_PLAIN:
@@ -248,21 +259,25 @@
             self.create_payload_artificial_parameter(operation),
             self.create_content_type_artificial_parameter(operation),
         ]
 
     def get_default_response(
         self, responses: dict[str, RestApiOperationExpectedResponse], preferred_responses: list[str]
     ) -> RestApiOperationExpectedResponse | None:
+        """Get the default response for the operation.
+
+        If no appropriate response is found, returns None.
+        """
         for code in preferred_responses:
             if code in responses:
                 return responses[code]
-        # If no appropriate response is found, return None
         return None
 
     def get_default_return_parameter(self, preferred_responses: list[str] | None = None) -> KernelParameterMetadata:
+        """Get the default return parameter for the operation."""
         if preferred_responses is None:
             preferred_responses = self._preferred_responses
 
         rest_operation_response = self.get_default_response(self.responses, preferred_responses)
 
         if rest_operation_response:
             return KernelParameterMetadata(
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_parameter.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_parameter.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         alternative_name: str | None = None,
         description: str | None = None,
         is_required: bool = False,
         default_value: Any | None = None,
         schema: str | None = None,
         response: RestApiOperationExpectedResponse | None = None,
     ):
+        """Initialize the RestApiOperationParameter."""
         self.name = name
         self.type = type
         self.location = location
         self.style = style
         self.alternative_name = alternative_name
         self.description = description
         self.is_required = is_required
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_payload.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_payload.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,11 +11,12 @@
     def __init__(
         self,
         media_type: str,
         properties: list["RestApiOperationPayloadProperty"],
         description: str | None = None,
         schema: str | None = None,
     ):
+        """Initialize the RestApiOperationPayload."""
         self.media_type = media_type
         self.properties = properties
         self.description = description
         self.schema = schema
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_payload_property.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/openapi_plugin/models/rest_api_operation_payload_property.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         type: str,
         properties: "RestApiOperationPayloadProperty",
         description: str | None = None,
         is_required: bool = False,
         default_value: Any | None = None,
         schema: str | None = None,
     ):
+        """Initialize the RestApiOperationPayloadProperty."""
         self.name = name
         self.type = type
         self.properties = properties
         self.description = description
         self.is_required = is_required
         self.default_value = default_value
         self.schema = schema
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-
 from collections.abc import Awaitable, Callable
 from typing import Any
 from urllib.parse import urlparse
 
 import httpx
 from pydantic import Field
 
@@ -24,14 +23,15 @@
     ignore_non_compliant_errors: bool = False
     user_agent: str | None = None
     enable_dynamic_payload: bool = True
     enable_payload_namespacing: bool = False
     operations_to_exclude: list[str] = Field(default_factory=list)
 
     def model_post_init(self, __context: Any) -> None:
+        """Post initialization method for the model."""
         from semantic_kernel.connectors.telemetry import HTTP_USER_AGENT
 
         if self.server_url_override:
             parsed_url = urlparse(self.server_url_override)
             if not parsed_url.scheme or not parsed_url.netloc:
                 raise ValueError(f"Invalid server_url_override: {self.server_url_override}")
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/openapi_manager.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/openapi_plugin/openapi_manager.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/openapi_parser.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/openapi_plugin/openapi_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 from collections import OrderedDict
-from typing import TYPE_CHECKING, Any, Generator
+from collections.abc import Generator
+from typing import TYPE_CHECKING, Any
 from urllib.parse import urlparse
 
 from prance import ResolvingParser
 
 from semantic_kernel.connectors.openapi_plugin.models.rest_api_operation import RestApiOperation
 from semantic_kernel.connectors.openapi_plugin.models.rest_api_operation_expected_response import (
     RestApiOperationExpectedResponse,
@@ -31,16 +32,15 @@
     )
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 @experimental_class
 class OpenApiParser:
-    """
-    NOTE: SK Python only supports the OpenAPI Spec >=3.0
+    """NOTE: SK Python only supports the OpenAPI Spec >=3.0.
 
     Import an OpenAPI file.
 
     Args:
         openapi_file: The path to the OpenAPI file which can be local or a URL.
 
     Returns:
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/openapi_plugin/openapi_runner.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/openapi_plugin/openapi_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import json
 import logging
 from collections import OrderedDict
 from collections.abc import Callable, Mapping
-from typing import TYPE_CHECKING, Any
+from typing import Any
 from urllib.parse import urlparse, urlunparse
 
 import httpx
 from openapi_core import Spec
 
 from semantic_kernel.connectors.ai.open_ai.const import USER_AGENT
 from semantic_kernel.connectors.openapi_plugin.models.rest_api_operation import RestApiOperation
@@ -17,35 +17,33 @@
 )
 from semantic_kernel.connectors.openapi_plugin.models.rest_api_operation_payload import RestApiOperationPayload
 from semantic_kernel.connectors.openapi_plugin.models.rest_api_operation_run_options import RestApiOperationRunOptions
 from semantic_kernel.exceptions.function_exceptions import FunctionExecutionException
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
-if TYPE_CHECKING:
-    pass
-
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 @experimental_class
 class OpenApiRunner:
-    """The OpenApiRunner that runs the operations defined in the OpenAPI manifest"""
+    """The OpenApiRunner that runs the operations defined in the OpenAPI manifest."""
 
     payload_argument_name = "payload"
     media_type_application_json = "application/json"
 
     def __init__(
         self,
         parsed_openapi_document: Mapping[str, str],
         auth_callback: Callable[[dict[str, str]], dict[str, str]] | None = None,
         http_client: httpx.AsyncClient | None = None,
         enable_dynamic_payload: bool = True,
         enable_payload_namespacing: bool = False,
     ):
+        """Initialize the OpenApiRunner."""
         self.spec = Spec.from_dict(parsed_openapi_document)
         self.auth_callback = auth_callback
         self.http_client = http_client
         self.enable_dynamic_payload = enable_dynamic_payload
         self.enable_payload_namespacing = enable_payload_namespacing
 
     def build_full_url(self, base_url, query_string):
@@ -98,19 +96,21 @@
             if property_metadata.is_required:
                 raise FunctionExecutionException(
                     f"No argument is found for the '{property_metadata.name}' payload property."
                 )
         return result
 
     def build_operation_payload(self, operation: RestApiOperation, arguments: KernelArguments) -> tuple[str, str]:
+        """Build the operation payload."""
         if operation.request_body is None and self.payload_argument_name not in arguments:
             return None, None
         return self.build_json_payload(operation.request_body, arguments)
 
     def get_argument_name_for_payload(self, property_name, property_namespace=None):
+        """Get argument name for the payload."""
         if not self.enable_payload_namespacing:
             return property_name
         return f"{property_namespace}.{property_name}" if property_namespace else property_name
 
     def _get_first_response_media_type(self, responses: OrderedDict[str, RestApiOperationExpectedResponse]) -> str:
         if responses:
             first_response = next(iter(responses.values()))
@@ -119,14 +119,15 @@
 
     async def run_operation(
         self,
         operation: RestApiOperation,
         arguments: KernelArguments | None = None,
         options: RestApiOperationRunOptions | None = None,
     ) -> str:
+        """Run the operation."""
         from semantic_kernel.connectors.telemetry import HTTP_USER_AGENT
 
         url = self.build_operation_url(
             operation=operation,
             arguments=arguments,
             server_url_override=options.server_url_override,
             api_host_url=options.api_host_url,
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/search_engine/bing_connector.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/search_engine/bing_connector.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,50 +10,41 @@
 from semantic_kernel.connectors.search_engine.connector import ConnectorBase
 from semantic_kernel.exceptions import ServiceInvalidRequestError
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class BingConnector(ConnectorBase):
-    """
-    A search engine connector that uses the Bing Search API to perform a web search
-    """
+    """A search engine connector that uses the Bing Search API to perform a web search."""
 
     _api_key: str
 
     def __init__(self, api_key: str | None = None, env_file_path: str | None = None) -> None:
         """Initializes a new instance of the BingConnector class.
 
-        Arguments:
-            api_key {str | None}: The Bing Search API key. If provided, will override
+        Args:
+            api_key (str | None): The Bing Search API key. If provided, will override
                 the value in the env vars or .env file.
-            env_file_path {str | None}: The optional path to the .env file. If provided,
+            env_file_path (str | None): The optional path to the .env file. If provided,
                 the settings are read from this file path location.
         """
         bing_settings = None
         try:
             bing_settings = BingSettings(env_file_path=env_file_path)
         except ValidationError as e:
             logger.warning(f"Failed to load the Bing pydantic settings: {e}.")
 
         self._api_key = api_key or (
             bing_settings.api_key.get_secret_value() if bing_settings and bing_settings.api_key else None
         )
-        assert self._api_key, "API key cannot be 'None' or empty."
+        if not self._api_key:
+            raise ValueError("API key cannot be 'None' or empty.")
 
     async def search(self, query: str, num_results: int = 1, offset: int = 0) -> list[str]:
-        """
-        Returns the search results of the query provided by pinging the Bing web search API.
-        Returns `num_results` results and ignores the first `offset`.
-
-        :param query: search query
-        :param num_results: the number of search results to return
-        :param offset: the number of search results to ignore
-        :return: list of search results
-        """
+        """Returns the search results of the query provided by pinging the Bing web search API."""
         if not query:
             raise ServiceInvalidRequestError("query cannot be 'None' or empty.")
 
         if num_results <= 0:
             raise ServiceInvalidRequestError("num_results value must be greater than 0.")
         if num_results >= 50:
             raise ServiceInvalidRequestError("num_results value must be less than 50.")
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/search_engine/bing_connector_settings.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/search_engine/bing_connector_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from pydantic import SecretStr
 from pydantic_settings import BaseSettings
 
 
 class BingSettings(BaseSettings):
-    """Bing Connector settings
+    """Bing Connector settings.
 
     The settings are first loaded from environment variables with the prefix 'BING_'. If the
     environment variables are not found, the settings can be loaded from a .env file with the
     encoding 'utf-8'. If the settings are not found in the .env file, the settings are ignored;
     however, validation will fail alerting that the settings are missing.
 
     Optional settings for prefix 'BING_' are:
@@ -17,20 +17,23 @@
 
     """
 
     env_file_path: str | None = None
     api_key: SecretStr | None = None
 
     class Config:
+        """Configuration for the Bing Connector settings."""
+
         env_prefix = "BING_"
         env_file = None
         env_file_encoding = "utf-8"
         extra = "ignore"
         case_sensitive = False
 
     @classmethod
     def create(cls, **kwargs):
+        """Create an instance of the Bing Connector settings."""
         if "env_file_path" in kwargs and kwargs["env_file_path"]:
             cls.Config.env_file = kwargs["env_file_path"]
         else:
             cls.Config.env_file = None
         return cls(**kwargs)
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/search_engine/google_connector.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/search_engine/google_connector.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,41 +8,32 @@
 from semantic_kernel.connectors.search_engine.connector import ConnectorBase
 from semantic_kernel.exceptions import ServiceInitializationError, ServiceInvalidRequestError
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class GoogleConnector(ConnectorBase):
-    """
-    A search engine connector that uses the Google Custom Search API to perform a web search.
-    """
+    """A search engine connector that uses the Google Custom Search API to perform a web search."""
 
     _api_key: str
     _search_engine_id: str
 
     def __init__(self, api_key: str, search_engine_id: str) -> None:
+        """Initializes a new instance of the GoogleConnector class."""
         self._api_key = api_key
         self._search_engine_id = search_engine_id
 
         if not self._api_key:
             raise ServiceInitializationError("Google Custom Search API key cannot be null.")
 
         if not self._search_engine_id:
             raise ServiceInitializationError("Google search engine ID cannot be null.")
 
     async def search(self, query: str, num_results: int = 1, offset: int = 0) -> list[str]:
-        """
-        Returns the search results of the query provided by pinging the Google Custom search API.
-        Returns `num_results` results and ignores the first `offset`.
-
-        :param query: search query
-        :param num_results: the number of search results to return
-        :param offset: the number of search results to ignore
-        :return: list of search results
-        """
+        """Returns the search results of the query provided by pinging the Google Custom search API."""
         if not query:
             raise ServiceInvalidRequestError("query cannot be 'None' or empty.")
 
         if num_results <= 0:
             raise ServiceInvalidRequestError("num_results value must be greater than 0.")
         if num_results > 10:
             raise ServiceInvalidRequestError("num_results value must be less than or equal to 10.")
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/telemetry.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/telemetry.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,20 +23,18 @@
     }
     if IS_TELEMETRY_ENABLED
     else None
 )
 
 
 def prepend_semantic_kernel_to_user_agent(headers: dict[str, Any]):
-    """
-    Prepend "Semantic-Kernel" to the User-Agent in the headers.
+    """Prepend "Semantic-Kernel" to the User-Agent in the headers.
 
     Args:
         headers: The existing headers dictionary.
 
     Returns:
         The modified headers dictionary with "Semantic-Kernel" prepended to the User-Agent.
     """
-
     headers[USER_AGENT] = f"{HTTP_USER_AGENT} {headers[USER_AGENT]}" if USER_AGENT in headers else f"{HTTP_USER_AGENT}"
 
     return headers
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/connectors/utils/document_loader.py` & `semantic_kernel-1.0.3/semantic_kernel/connectors/utils/document_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     @staticmethod
     async def from_uri(
         url: str,
         http_client: httpx.AsyncClient,
         auth_callback: Callable[[Any], None] | None,
         user_agent: str | None = HTTP_USER_AGENT,
     ):
-        """Load the manifest from the given URL"""
+        """Load the manifest from the given URL."""
         headers = {"User-Agent": user_agent}
         async with http_client as client:
             if auth_callback:
                 await auth_callback(client, url)
 
             logger.info(f"Importing document from {url}")
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/contents/__init__.py` & `semantic_kernel-1.0.3/semantic_kernel/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/contents/chat_history.py` & `semantic_kernel-1.0.3/semantic_kernel/contents/chat_history.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 from collections.abc import Generator
 from functools import singledispatchmethod
 from html import unescape
 from typing import Any
-from xml.etree.ElementTree import Element, tostring
+from xml.etree.ElementTree import Element, tostring  # nosec
 
 from defusedxml.ElementTree import XML, ParseError
 from pydantic import field_validator
 
 from semantic_kernel.contents.author_role import AuthorRole
 from semantic_kernel.contents.chat_message_content import ChatMessageContent
 from semantic_kernel.contents.const import CHAT_HISTORY_TAG, CHAT_MESSAGE_CONTENT_TAG
@@ -17,48 +17,49 @@
 from semantic_kernel.exceptions import ContentInitializationError, ContentSerializationError
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 logger = logging.getLogger(__name__)
 
 
 class ChatHistory(KernelBaseModel):
-    """
-    This class holds the history of chat messages from a chat conversation.
+    """This class holds the history of chat messages from a chat conversation.
 
     Note: the constructor takes a system_message parameter, which is not part
     of the class definition. This is to allow the system_message to be passed in
     as a keyword argument, but not be part of the class definition.
 
     Attributes:
         messages (List[ChatMessageContent]): The list of chat messages in the history.
     """
 
     messages: list[ChatMessageContent]
 
     def __init__(self, **data: Any):
-        """
-        Initializes a new instance of the ChatHistory class, optionally incorporating a message and/or
-        a system message at the beginning of the chat history.
+        """Initializes a new instance of the ChatHistory class.
+
+        Optionally incorporating a message and/or a system message at the beginning of the chat history.
 
         This constructor allows for flexible initialization with chat messages and an optional messages or a
         system message. If both 'messages' (a list of ChatMessageContent instances) and 'system_message' are
         provided, the 'system_message' is prepended to the list of messages, ensuring it appears as the first
         message in the history. If only 'system_message' is provided without any 'messages', the chat history is
         initialized with the 'system_message' as its first item. If 'messages' are provided without a
         'system_message', the chat history is initialized with the provided messages as is.
 
-        Parameters:
-        - **data: Arbitrary keyword arguments. The constructor looks for two optional keys:
-            - 'messages': Optional[List[ChatMessageContent]], a list of chat messages to include in the history.
-            - 'system_message' Optional[str]: An optional string representing a system-generated message to be
-                included at the start of the chat history.
-
         Note: The 'system_message' is not retained as part of the class's attributes; it's used during
         initialization and then discarded. The rest of the keyword arguments are passed to the superclass
         constructor and handled according to the Pydantic model's behavior.
+
+        Args:
+            **data: Arbitrary keyword arguments.
+                The constructor looks for two optional keys:
+                - 'messages': Optional[List[ChatMessageContent]], a list of chat messages to include in the history.
+                - 'system_message' Optional[str]: An optional string representing a system-generated message to be
+                    included at the start of the chat history.
+
         """
         system_message_content = data.pop("system_message", None)
 
         if system_message_content:
             system_message = ChatMessageContent(role=AuthorRole.SYSTEM, content=system_message_content)
 
             if "messages" in data:
@@ -85,57 +86,65 @@
     @singledispatchmethod
     def add_system_message(self, content: str | list[KernelContent], **kwargs) -> None:
         """Add a system message to the chat history."""
         raise NotImplementedError
 
     @add_system_message.register
     def add_system_message_str(self, content: str, **kwargs: Any) -> None:
+        """Add a system message to the chat history."""
         self.add_message(message=self._prepare_for_add(role=AuthorRole.SYSTEM, content=content, **kwargs))
 
     @add_system_message.register(list)
     def add_system_message_list(self, content: list[KernelContent], **kwargs: Any) -> None:
+        """Add a system message to the chat history."""
         self.add_message(message=self._prepare_for_add(role=AuthorRole.SYSTEM, items=content, **kwargs))
 
     @singledispatchmethod
     def add_user_message(self, content: str | list[KernelContent], **kwargs: Any) -> None:
         """Add a user message to the chat history."""
         raise NotImplementedError
 
     @add_user_message.register
     def add_user_message_str(self, content: str, **kwargs: Any) -> None:
+        """Add a user message to the chat history."""
         self.add_message(message=self._prepare_for_add(role=AuthorRole.USER, content=content, **kwargs))
 
     @add_user_message.register(list)
     def add_user_message_list(self, content: list[KernelContent], **kwargs: Any) -> None:
+        """Add a user message to the chat history."""
         self.add_message(message=self._prepare_for_add(role=AuthorRole.USER, items=content, **kwargs))
 
     @singledispatchmethod
     def add_assistant_message(self, content: str | list[KernelContent], **kwargs: Any) -> None:
         """Add an assistant message to the chat history."""
         raise NotImplementedError
 
     @add_assistant_message.register
     def add_assistant_message_str(self, content: str, **kwargs: Any) -> None:
+        """Add an assistant message to the chat history."""
         self.add_message(message=self._prepare_for_add(role=AuthorRole.ASSISTANT, content=content, **kwargs))
 
     @add_assistant_message.register(list)
     def add_assistant_message_list(self, content: list[KernelContent], **kwargs: Any) -> None:
+        """Add an assistant message to the chat history."""
         self.add_message(message=self._prepare_for_add(role=AuthorRole.ASSISTANT, items=content, **kwargs))
 
     @singledispatchmethod
     def add_tool_message(self, content: str | list[KernelContent], **kwargs: Any) -> None:
         """Add a tool message to the chat history."""
         raise NotImplementedError
 
     @add_tool_message.register
     def add_tool_message_str(self, content: str, **kwargs: Any) -> None:
+        """Add a tool message to the chat history."""
         self.add_message(message=self._prepare_for_add(role=AuthorRole.TOOL, content=content, **kwargs))
 
     @add_tool_message.register(list)
     def add_tool_message_list(self, content: list[KernelContent], **kwargs: Any) -> None:
+        """Add a tool message to the chat history."""
         self.add_message(message=self._prepare_for_add(role=AuthorRole.TOOL, items=content, **kwargs))
 
     def add_message(
         self,
         message: ChatMessageContent | dict[str, Any],
         encoding: str | None = None,
         metadata: dict[str, Any] | None = None,
@@ -237,16 +246,15 @@
         if not isinstance(other, ChatHistory):
             return False
 
         return self.messages == other.messages
 
     @classmethod
     def from_rendered_prompt(cls, rendered_prompt: str) -> "ChatHistory":
-        """
-        Create a ChatHistory instance from a rendered prompt.
+        """Create a ChatHistory instance from a rendered prompt.
 
         Args:
             rendered_prompt (str): The rendered prompt to convert to a ChatHistory instance.
 
         Returns:
             ChatHistory: The ChatHistory instance created from the rendered prompt.
         """
@@ -269,32 +277,30 @@
             if item.tail and item.tail.strip():
                 messages.append(ChatMessageContent(role=AuthorRole.USER, content=unescape(item.tail.strip())))
         if len(messages) == 1 and messages[0].role == AuthorRole.SYSTEM:
             messages[0].role = AuthorRole.USER
         return cls(messages=messages)
 
     def serialize(self) -> str:
-        """
-        Serializes the ChatHistory instance to a JSON string.
+        """Serializes the ChatHistory instance to a JSON string.
 
         Returns:
             str: A JSON string representation of the ChatHistory instance.
 
         Raises:
             ValueError: If the ChatHistory instance cannot be serialized to JSON.
         """
         try:
             return self.model_dump_json(indent=2, exclude_none=True)
         except Exception as e:  # pragma: no cover
             raise ContentSerializationError(f"Unable to serialize ChatHistory to JSON: {e}") from e
 
     @classmethod
     def restore_chat_history(cls, chat_history_json: str) -> "ChatHistory":
-        """
-        Restores a ChatHistory instance from a JSON string.
+        """Restores a ChatHistory instance from a JSON string.
 
         Args:
             chat_history_json (str): The JSON string to deserialize
                 into a ChatHistory instance.
 
         Returns:
             ChatHistory: The deserialized ChatHistory instance.
@@ -305,28 +311,26 @@
         """
         try:
             return ChatHistory.model_validate_json(chat_history_json)
         except Exception as e:
             raise ContentInitializationError(f"Invalid JSON format: {e}")
 
     def store_chat_history_to_file(self, file_path: str) -> None:
-        """
-        Stores the serialized ChatHistory to a file.
+        """Stores the serialized ChatHistory to a file.
 
         Args:
             file_path (str): The path to the file where the serialized data will be stored.
         """
         json_str = self.serialize()
         with open(file_path, "w") as file:
             file.write(json_str)
 
     @classmethod
     def load_chat_history_from_file(cls, file_path: str) -> "ChatHistory":
-        """
-        Loads the ChatHistory from a file.
+        """Loads the ChatHistory from a file.
 
         Args:
             file_path (str): The path to the file from which to load the ChatHistory.
 
         Returns:
             ChatHistory: The deserialized ChatHistory instance.
         """
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/contents/chat_message_content.py` & `semantic_kernel-1.0.3/semantic_kernel/contents/chat_message_content.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 from enum import Enum
 from html import unescape
 from typing import Any, Union, overload
-from xml.etree.ElementTree import Element
+from xml.etree.ElementTree import Element  # nosec
 
 from defusedxml import ElementTree
 from pydantic import Field
 
 from semantic_kernel.contents.author_role import AuthorRole
 from semantic_kernel.contents.const import (
     CHAT_MESSAGE_CONTENT_TAG,
@@ -33,15 +33,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class ChatMessageContent(KernelContent):
     """This is the class for chat message response content.
 
-    All Chat Completion Services should return a instance of this class as response.
+    All Chat Completion Services should return an instance of this class as response.
     Or they can implement their own subclass of this class and return an instance.
 
     Args:
         inner_content: Optional[Any] - The inner content of the response,
             this should hold all the information from the response so even
             when not creating a subclass a developer can leverage the full thing.
         ai_model_id: Optional[str] - The id of the AI model that generated this response.
@@ -68,82 +68,58 @@
         name: str | None = None,
         inner_content: Any | None = None,
         encoding: str | None = None,
         finish_reason: FinishReason | None = None,
         ai_model_id: str | None = None,
         metadata: dict[str, Any] | None = None,
         **kwargs: Any,
-    ) -> None:
-        """All Chat Completion Services should return a instance of this class as response.
-        Or they can implement their own subclass of this class and return an instance.
-
-        Args:
-            inner_content: Optional[Any] - The inner content of the response,
-                this should hold all the information from the response so even
-                when not creating a subclass a developer can leverage the full thing.
-            ai_model_id: Optional[str] - The id of the AI model that generated this response.
-            metadata: Dict[str, Any] - Any metadata that should be attached to the response.
-            role: ChatRole - The role of the chat message.
-            items: list[TextContent, StreamingTextContent, FunctionCallContent, FunctionResultContent] - The content.
-            encoding: Optional[str] - The encoding of the text.
-        """
+    ) -> None: ...
 
     @overload
     def __init__(
         self,
         role: AuthorRole,
         content: str,
         name: str | None = None,
         inner_content: Any | None = None,
         encoding: str | None = None,
         finish_reason: FinishReason | None = None,
         ai_model_id: str | None = None,
         metadata: dict[str, Any] | None = None,
         **kwargs: Any,
-    ) -> None:
-        """All Chat Completion Services should return a instance of this class as response.
-        Or they can implement their own subclass of this class and return an instance.
-
-        Args:
-            inner_content: Optional[Any] - The inner content of the response,
-                this should hold all the information from the response so even
-                when not creating a subclass a developer can leverage the full thing.
-            ai_model_id: Optional[str] - The id of the AI model that generated this response.
-            metadata: Dict[str, Any] - Any metadata that should be attached to the response.
-            role: ChatRole - The role of the chat message.
-            content: str - The text of the response.
-            encoding: Optional[str] - The encoding of the text.
-        """
+    ) -> None: ...
 
     def __init__(  # type: ignore
         self,
         role: AuthorRole,
         items: list[ITEM_TYPES] | None = None,
         content: str | None = None,
         inner_content: Any | None = None,
         name: str | None = None,
         encoding: str | None = None,
         finish_reason: FinishReason | None = None,
         ai_model_id: str | None = None,
         metadata: dict[str, Any] | None = None,
         **kwargs: Any,
     ):
-        """All Chat Completion Services should return a instance of this class as response.
-        Or they can implement their own subclass of this class and return an instance.
+        """Create a ChatMessageContent instance.
 
         Args:
+            role: ChatRole - The role of the chat message.
+            items: list[TextContent, StreamingTextContent, FunctionCallContent, FunctionResultContent] - The content.
+            content: str - The text of the response.
             inner_content: Optional[Any] - The inner content of the response,
                 this should hold all the information from the response so even
                 when not creating a subclass a developer can leverage the full thing.
+            name: Optional[str] - The name of the response.
+            encoding: Optional[str] - The encoding of the text.
+            finish_reason: Optional[FinishReason] - The reason the response was finished.
             ai_model_id: Optional[str] - The id of the AI model that generated this response.
             metadata: Dict[str, Any] - Any metadata that should be attached to the response.
-            role: ChatRole - The role of the chat message.
-            content: str - The text of the response.
-            items: list[TextContent, StreamingTextContent, FunctionCallContent, FunctionResultContent] - The content.
-            encoding: Optional[str] - The encoding of the text.
+            **kwargs: Any - Any additional fields to set on the instance.
         """
         kwargs["role"] = role
         if encoding:
             kwargs["encoding"] = encoding
         if finish_reason:
             kwargs["finish_reason"] = finish_reason
         if name:
@@ -227,15 +203,15 @@
             root.set(field, value)
         for index, item in enumerate(self.items):
             root.insert(index, item.to_element())
         return root
 
     @classmethod
     def from_element(cls, element: Element) -> "ChatMessageContent":
-        """Create a new instance of ChatMessageContent from a XML element.
+        """Create a new instance of ChatMessageContent from an XML element.
 
         Args:
             element: Element - The XML Element to create the ChatMessageContent from.
 
         Returns:
             ChatMessageContent - The new instance of ChatMessageContent or a subclass.
         """
@@ -267,15 +243,14 @@
 
     def to_prompt(self) -> str:
         """Convert the ChatMessageContent to a prompt.
 
         Returns:
             str - The prompt from the ChatMessageContent.
         """
-
         root = self.to_element()
         return ElementTree.tostring(root, encoding=self.encoding or "unicode", short_empty_elements=False)
 
     def to_dict(self, role_key: str = "role", content_key: str = "content") -> dict[str, Any]:
         """Serialize the ChatMessageContent to a dictionary.
 
         Returns:
@@ -285,15 +260,15 @@
             role_key: self.role.value,
         }
         if self.role == AuthorRole.ASSISTANT and any(isinstance(item, FunctionCallContent) for item in self.items):
             ret["tool_calls"] = [item.to_dict() for item in self.items if isinstance(item, FunctionCallContent)]
         else:
             ret[content_key] = self._parse_items()
         if self.role == AuthorRole.TOOL:
-            assert isinstance(self.items[0], FunctionResultContent)
+            assert isinstance(self.items[0], FunctionResultContent)  # nosec
             ret["tool_call_id"] = self.items[0].id or ""
         if self.role != AuthorRole.TOOL and self.name:
             ret["name"] = self.name
         return ret
 
     def _parse_items(self) -> str | list[dict[str, Any]]:
         """Parse the items of the ChatMessageContent.
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/contents/function_call_content.py` & `semantic_kernel-1.0.3/semantic_kernel/contents/function_call_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import json
 import logging
 from functools import cached_property
 from typing import TYPE_CHECKING, Any
-from xml.etree.ElementTree import Element
+from xml.etree.ElementTree import Element  # nosec
 
 from semantic_kernel.contents.const import FUNCTION_CALL_CONTENT_TAG
 from semantic_kernel.contents.kernel_content import KernelContent
 from semantic_kernel.exceptions import FunctionCallInvalidArgumentsException, FunctionCallInvalidNameException
 
 if TYPE_CHECKING:
     from semantic_kernel.functions.kernel_arguments import KernelArguments
@@ -31,14 +31,15 @@
 
     @cached_property
     def plugin_name(self) -> str | None:
         """Get the plugin name."""
         return self.split_name()[0]
 
     def __str__(self) -> str:
+        """Return the function call as a string."""
         return f"{self.name}({self.arguments})"
 
     def __add__(self, other: "FunctionCallContent | None") -> "FunctionCallContent":
         """Add two function calls together, combines the arguments, ignores the name."""
         if not other:
             return self
         if self.id and other.id and self.id != other.id:
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/contents/function_result_content.py` & `semantic_kernel-1.0.3/semantic_kernel/contents/function_result_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from functools import cached_property
 from typing import TYPE_CHECKING, Any
-from xml.etree.ElementTree import Element
+from xml.etree.ElementTree import Element  # nosec
 
 from pydantic import field_validator
 
 from semantic_kernel.contents.const import FUNCTION_RESULT_CONTENT_TAG, TEXT_CONTENT_TAG
 from semantic_kernel.contents.kernel_content import KernelContent
 from semantic_kernel.contents.text_content import TextContent
 
@@ -19,15 +19,15 @@
     TEXT_CONTENT_TAG: TextContent,
 }
 
 
 class FunctionResultContent(KernelContent):
     """This is the base class for text response content.
 
-    All Text Completion Services should return a instance of this class as response.
+    All Text Completion Services should return an instance of this class as response.
     Or they can implement their own subclass of this class and return an instance.
 
     Args:
         inner_content: Any - The inner content of the response,
             this should hold all the information from the response so even
             when not creating a subclass a developer can leverage the full thing.
         ai_model_id: str | None - The id of the AI model that generated this response.
@@ -58,14 +58,15 @@
     @classmethod
     def _validate_result(cls, result: Any):
         if not isinstance(result, str):
             result = str(result)
         return result
 
     def __str__(self) -> str:
+        """Return the text of the response."""
         return self.result
 
     def to_element(self) -> Element:
         """Convert the instance to an Element."""
         element = Element(FUNCTION_RESULT_CONTENT_TAG)
         element.set("id", self.id)
         if self.name:
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/contents/kernel_content.py` & `semantic_kernel-1.0.3/semantic_kernel/contents/kernel_content.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,21 +13,25 @@
 
     inner_content: Any | None = None
     ai_model_id: str | None = None
     metadata: dict[str, Any] = Field(default_factory=dict)
 
     @abstractmethod
     def __str__(self) -> str:
+        """Return the string representation of the content."""
         pass
 
     @abstractmethod
     def to_element(self) -> Any:
+        """Convert the instance to an Element."""
         pass
 
     @classmethod
     @abstractmethod
     def from_element(cls, element: Any) -> "KernelContent":
+        """Create an instance from an Element."""
         pass
 
     @abstractmethod
     def to_dict(self) -> dict[str, Any]:
+        """Convert the instance to a dictionary."""
         pass
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/contents/streaming_chat_message_content.py` & `semantic_kernel-1.0.3/semantic_kernel/contents/streaming_chat_message_content.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from enum import Enum
 from typing import Any, Union, overload
-from xml.etree.ElementTree import Element
+from xml.etree.ElementTree import Element  # nosec
 
 from semantic_kernel.contents.author_role import AuthorRole
 from semantic_kernel.contents.chat_message_content import ChatMessageContent
 from semantic_kernel.contents.const import CHAT_MESSAGE_CONTENT_TAG
 from semantic_kernel.contents.finish_reason import FinishReason
 from semantic_kernel.contents.function_call_content import FunctionCallContent
 from semantic_kernel.contents.function_result_content import FunctionResultContent
@@ -16,16 +16,16 @@
 
 ITEM_TYPES = Union[StreamingTextContent, FunctionCallContent, FunctionResultContent]
 
 
 class StreamingChatMessageContent(ChatMessageContent, StreamingContentMixin):
     """This is the class for streaming chat message response content.
 
-    All Chat Completion Services should return a instance of this class as streaming response,
-    where each part of the response as it is streamed is converted to a instance of this class,
+    All Chat Completion Services should return an instance of this class as streaming response,
+    where each part of the response as it is streamed is converted to an instance of this class,
     the end-user will have to either do something directly or gather them and combine them into a
     new instance. A service can implement their own subclass of this class and return instances of that.
 
     Args:
         choice_index: int - The index of the choice that generated this response.
         inner_content: Optional[Any] - The inner content of the response,
             this should hold all the information from the response so even
@@ -50,82 +50,58 @@
         choice_index: int,
         name: str | None = None,
         inner_content: Any | None = None,
         encoding: str | None = None,
         finish_reason: FinishReason | None = None,
         ai_model_id: str | None = None,
         metadata: dict[str, Any] | None = None,
-    ) -> None:
-        """All Chat Completion Services should return a instance of this class as response for streaming.
-        Or they can implement their own subclass of this class and return an instance.
-
-        Args:
-            inner_content: Optional[Any] - The inner content of the response,
-                this should hold all the information from the response so even
-                when not creating a subclass a developer can leverage the full thing.
-            ai_model_id: Optional[str] - The id of the AI model that generated this response.
-            metadata: Dict[str, Any] - Any metadata that should be attached to the response.
-            role: ChatRole - The role of the chat message.
-            items: list[TextContent, FunctionCallContent, FunctionResultContent] - The content.
-            encoding: Optional[str] - The encoding of the text.
-        """
+    ) -> None: ...
 
     @overload
     def __init__(
         self,
         role: AuthorRole,
         content: str,
         choice_index: int,
         name: str | None = None,
         inner_content: Any | None = None,
         encoding: str | None = None,
         finish_reason: FinishReason | None = None,
         ai_model_id: str | None = None,
         metadata: dict[str, Any] | None = None,
-    ) -> None:
-        """All Chat Completion Services should return a instance of this class as response for streaming.
-        Or they can implement their own subclass of this class and return an instance.
-
-        Args:
-            inner_content: Optional[Any] - The inner content of the response,
-                this should hold all the information from the response so even
-                when not creating a subclass a developer can leverage the full thing.
-            ai_model_id: Optional[str] - The id of the AI model that generated this response.
-            metadata: Dict[str, Any] - Any metadata that should be attached to the response.
-            role: ChatRole - The role of the chat message.
-            content: str - The text of the response.
-            encoding: Optional[str] - The encoding of the text.
-        """
+    ) -> None: ...
 
     def __init__(  # type: ignore
         self,
         role: AuthorRole,
         choice_index: int,
         items: list[ITEM_TYPES] | None = None,
         content: str | None = None,
         inner_content: Any | None = None,
         name: str | None = None,
         encoding: str | None = None,
         finish_reason: FinishReason | None = None,
         ai_model_id: str | None = None,
         metadata: dict[str, Any] | None = None,
     ):
-        """All Chat Completion Services should return a instance of this class as response for streaming.
-        Or they can implement their own subclass of this class and return an instance.
+        """Create a new instance of StreamingChatMessageContent.
 
         Args:
+            role: ChatRole - The role of the chat message.
+            choice_index: int - The index of the choice that generated this response.
+            items: list[TextContent, FunctionCallContent, FunctionResultContent] - The content.
+            content: str - The text of the response.
             inner_content: Optional[Any] - The inner content of the response,
                 this should hold all the information from the response so even
                 when not creating a subclass a developer can leverage the full thing.
-            ai_model_id: Optional[str] - The id of the AI model that generated this response.
-            metadata: Dict[str, Any] - Any metadata that should be attached to the response.
-            role: ChatRole - The role of the chat message.
-            content: str - The text of the response.
-            items: list[TextContent, FunctionCallContent, FunctionResultContent] - The content.
+            name: Optional[str] - The name of the response.
             encoding: Optional[str] - The encoding of the text.
+            finish_reason: Optional[FinishReason] - The reason the response was finished.
+            metadata: Dict[str, Any] - Any metadata that should be attached to the response.
+            ai_model_id: Optional[str] - The id of the AI model that generated this response.
         """
         kwargs: dict[str, Any] = {
             "role": role,
             "choice_index": choice_index,
         }
         if encoding:
             kwargs["encoding"] = encoding
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/contents/streaming_text_content.py` & `semantic_kernel-1.0.3/semantic_kernel/contents/streaming_text_content.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from semantic_kernel.contents.text_content import TextContent
 from semantic_kernel.exceptions import ContentAdditionException
 
 
 class StreamingTextContent(StreamingContentMixin, TextContent):
     """This is the base class for streaming text response content.
 
-    All Text Completion Services should return a instance of this class as streaming response.
+    All Text Completion Services should return an instance of this class as streaming response.
     Or they can implement their own subclass of this class and return an instance.
 
     Args:
         choice_index: int - The index of the choice that generated this response.
         inner_content: Optional[Any] - The inner content of the response,
             this should hold all the information from the response so even
             when not creating a subclass a developer can leverage the full thing.
@@ -24,14 +24,15 @@
     Methods:
         __str__: Returns the text of the response.
         __bytes__: Returns the content of the response encoded in the encoding.
         __add__: Combines two StreamingTextContent instances.
     """
 
     def __bytes__(self) -> bytes:
+        """Return the content of the response encoded in the encoding."""
         return self.text.encode(self.encoding if self.encoding else "utf-8") if self.text else b""
 
     def __add__(self, other: "TextContent") -> "StreamingTextContent":
         """When combining two StreamingTextContent instances, the text fields are combined.
 
         The inner_content of the first one is used, choice_index, ai_model_id and encoding should be the same.
         """
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/contents/text_content.py` & `semantic_kernel-1.0.3/semantic_kernel/contents/text_content.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from html import unescape
-from xml.etree.ElementTree import Element
+from xml.etree.ElementTree import Element  # nosec
 
 from semantic_kernel.contents.const import TEXT_CONTENT_TAG
 from semantic_kernel.contents.kernel_content import KernelContent
 
 
 class TextContent(KernelContent):
     """This is the base class for text response content.
 
-    All Text Completion Services should return a instance of this class as response.
+    All Text Completion Services should return an instance of this class as response.
     Or they can implement their own subclass of this class and return an instance.
 
     Args:
         inner_content: Any - The inner content of the response,
             this should hold all the information from the response so even
             when not creating a subclass a developer can leverage the full thing.
         ai_model_id: str | None - The id of the AI model that generated this response.
@@ -26,14 +26,15 @@
         __str__: Returns the text of the response.
     """
 
     text: str
     encoding: str | None = None
 
     def __str__(self) -> str:
+        """Return the text of the response."""
         return self.text
 
     def to_element(self) -> Element:
         """Convert the instance to an Element."""
         element = Element(TEXT_CONTENT_TAG)
         element.text = self.text
         if self.encoding:
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/contents/types.py` & `semantic_kernel-1.0.3/semantic_kernel/contents/types.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/core_plugins/__init__.py` & `semantic_kernel-1.0.3/semantic_kernel/core_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/core_plugins/conversation_summary_plugin.py` & `semantic_kernel-1.0.3/semantic_kernel/core_plugins/conversation_summary_plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 if TYPE_CHECKING:
     from semantic_kernel.functions.kernel_arguments import KernelArguments
     from semantic_kernel.kernel import Kernel
     from semantic_kernel.prompt_template.prompt_template_config import PromptTemplateConfig
 
 
 class ConversationSummaryPlugin:
-    """
-    Semantic plugin that enables conversations summarization.
-    """
+    """Semantic plugin that enables conversations summarization."""
 
     from semantic_kernel.functions.kernel_function_decorator import kernel_function
 
     # The max tokens to process in a single semantic function call.
     _max_tokens = 1024
 
     _summarize_conversation_prompt_template = (
@@ -26,16 +24,15 @@
         " knowledge.\nSummary is in plain text, in complete sentences, with no markup"
         " or tags.\n\nBEGIN SUMMARY:\n"
     )
 
     def __init__(
         self, kernel: "Kernel", prompt_template_config: "PromptTemplateConfig", return_key: str = "summary"
     ) -> None:
-        """
-        Initializes a new instance of the ConversationSummaryPlugin class.
+        """Initializes a new instance of the ConversationSummaryPlugin class.
 
         :param kernel: The kernel instance.
         :param prompt_template_config: The prompt template configuration.
         :param return_key: The key to use for the return value.
         """
         self.return_key = return_key
         self._summarizeConversationFunction = kernel.add_function(
@@ -53,16 +50,15 @@
         self,
         input: Annotated[str, "A long conversation transcript."],
         kernel: Annotated["Kernel", "The kernel instance."],
         arguments: Annotated["KernelArguments", "Arguments used by the kernel."],
     ) -> Annotated[
         "KernelArguments", "KernelArguments with the summarized conversation result in key self.return_key."
     ]:
-        """
-        Given a long conversation transcript, summarize the conversation.
+        """Given a long conversation transcript, summarize the conversation.
 
         :param input: A long conversation transcript.
         :param kernel: The kernel for function execution.
         :param arguments: Arguments used by the kernel.
         :return: KernelArguments with the summarized conversation result in key self.return_key.
         """
         from semantic_kernel.text import text_chunker
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/core_plugins/http_plugin.py` & `semantic_kernel-1.0.3/semantic_kernel/core_plugins/http_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,36 +7,34 @@
 
 from semantic_kernel.exceptions import FunctionExecutionException
 from semantic_kernel.functions.kernel_function_decorator import kernel_function
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 
 class HttpPlugin(KernelBaseModel):
-    """
-    A plugin that provides HTTP functionality.
+    """A plugin that provides HTTP functionality.
 
     Usage:
         kernel.add_plugin(HttpPlugin(), "http")
 
     Examples:
-
         {{http.getAsync $url}}
         {{http.postAsync $url}}
         {{http.putAsync $url}}
         {{http.deleteAsync $url}}
     """
 
-    @kernel_function(description="Makes a GET request to a uri", name="getAsync")
-    async def get(self, url: Annotated[str, "The URI to send the request to."]) -> str:
-        """
-        Sends an HTTP GET request to the specified URI and returns
-        the response body as a string.
-        params:
-            uri: The URI to send the request to.
-        returns:
+    @kernel_function(description="Makes a GET request to a url", name="getAsync")
+    async def get(self, url: Annotated[str, "The URL to send the request to."]) -> str:
+        """Sends an HTTP GET request to the specified URI and returns the response body as a string.
+
+        Args:
+            url: The URL to send the request to.
+
+        Returns:
             The response body as a string.
         """
         if not url:
             raise FunctionExecutionException("url cannot be `None` or empty")
 
         async with aiohttp.ClientSession() as session:
             async with session.get(url, raise_for_status=True) as response:
@@ -44,18 +42,17 @@
 
     @kernel_function(description="Makes a POST request to a uri", name="postAsync")
     async def post(
         self,
         url: Annotated[str, "The URI to send the request to."],
         body: Annotated[dict[str, Any] | None, "The body of the request"] = {},
     ) -> str:
-        """
-        Sends an HTTP POST request to the specified URI and returns
-        the response body as a string.
-        params:
+        """Sends an HTTP POST request to the specified URI and returns the response body as a string.
+
+        Args:
             url: The URI to send the request to.
             body: Contains the body of the request
         returns:
             The response body as a string.
         """
         if not url:
             raise FunctionExecutionException("url cannot be `None` or empty")
@@ -68,39 +65,40 @@
 
     @kernel_function(description="Makes a PUT request to a uri", name="putAsync")
     async def put(
         self,
         url: Annotated[str, "The URI to send the request to."],
         body: Annotated[dict[str, Any] | None, "The body of the request"] = {},
     ) -> str:
-        """
-        Sends an HTTP PUT request to the specified URI and returns
-        the response body as a string.
-        params:
+        """Sends an HTTP PUT request to the specified URI and returns the response body as a string.
+
+        Args:
             url: The URI to send the request to.
-        returns:
+            body: Contains the body of the request
+
+        Returns:
             The response body as a string.
         """
         if not url:
             raise FunctionExecutionException("url cannot be `None` or empty")
 
         headers = {"Content-Type": "application/json"}
         data = json.dumps(body)
         async with aiohttp.ClientSession() as session:
             async with session.put(url, headers=headers, data=data, raise_for_status=True) as response:
                 return await response.text()
 
     @kernel_function(description="Makes a DELETE request to a uri", name="deleteAsync")
     async def delete(self, url: Annotated[str, "The URI to send the request to."]) -> str:
-        """
-        Sends an HTTP DELETE request to the specified URI and returns
-        the response body as a string.
-        params:
-            uri: The URI to send the request to.
-        returns:
+        """Sends an HTTP DELETE request to the specified URI and returns the response body as a string.
+
+        Args:
+            url: The URI to send the request to.
+
+        Returns:
             The response body as a string.
         """
         if not url:
             raise FunctionExecutionException("url cannot be `None` or empty")
         async with aiohttp.ClientSession() as session:
             async with session.delete(url, raise_for_status=True) as response:
                 return await response.text()
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/core_plugins/math_plugin.py` & `semantic_kernel-1.0.3/semantic_kernel/core_plugins/math_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 from typing import Annotated
 
 from semantic_kernel.functions.kernel_function_decorator import kernel_function
 
 
 class MathPlugin:
-    """
-    Description: MathPlugin provides a set of functions to make Math calculations.
+    """Description: MathPlugin provides a set of functions to make Math calculations.
 
     Usage:
         kernel.add_plugin(MathPlugin(), plugin_name="math")
 
     Examples:
         {{math.Add}} => Returns the sum of input and amount (provided in the KernelArguments)
         {{math.Subtract}} => Returns the difference of input and amount (provided in the KernelArguments)
@@ -35,31 +34,29 @@
         name="Subtract",
     )
     def subtract(
         self,
         input: Annotated[int, "the first number"],
         amount: Annotated[int, "the number to subtract"],
     ) -> int:
-        """
-        Returns the difference of numbers provided.
+        """Returns the difference of numbers provided.
 
         :param initial_value_text: Initial value as string to subtract the specified amount
         :param context: Contains the context to get the numbers from
         :return: The resulting subtraction as a string
         """
         if isinstance(input, str):
             input = int(input)
         if isinstance(amount, str):
             amount = int(amount)
         return MathPlugin.add_or_subtract(input, amount, add=False)
 
     @staticmethod
     def add_or_subtract(input: int, amount: int, add: bool) -> int:
-        """
-        Helper function to perform addition or subtraction based on the add flag.
+        """Helper function to perform addition or subtraction based on the add flag.
 
         :param initial_value_text: Initial value as string to add or subtract the specified amount
         :param context: Contains the context to get the numbers from
         :param add: If True, performs addition, otherwise performs subtraction
         :return: The resulting sum or subtraction as a string
         """
         return input + amount if add else input - amount
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/core_plugins/sessions_python_tool/README.md` & `semantic_kernel-1.0.3/semantic_kernel/core_plugins/sessions_python_tool/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py` & `semantic_kernel-1.0.3/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,32 +80,32 @@
         if not endpoint.endswith("/"):
             # Ensure the endpoint ends with a '/'
             endpoint = endpoint + "/"
         return endpoint
 
     async def _ensure_auth_token(self) -> str:
         """Ensure the auth token is valid."""
-
         try:
             auth_token = await self.auth_callback()
         except Exception as e:
             logger.error(f"Failed to retrieve the client auth token with message: {str(e)}")
             raise FunctionExecutionException(f"Failed to retrieve the client auth token with messages: {str(e)}") from e
 
         return auth_token
 
     def _sanitize_input(self, code: str) -> str:
         """Sanitize input to the python REPL.
-        Remove whitespace, backtick & python (if llm mistakes python console as terminal)
+
+        Remove whitespace, backtick & python (if llm mistakes python console as terminal).
+
         Args:
-            query: The query to sanitize
+            code: The query to sanitize
         Returns:
             str: The sanitized query
         """
-
         # Removes `, whitespace & python from start
         code = re.sub(r"^(\s|`)*(?i:python)?\s*", "", code)
         # Removes whitespace & ` from end
         code = re.sub(r"(\s|`)*$", "", code)
         return code
 
     @kernel_function(
@@ -116,24 +116,23 @@
                      Use \" to include double quotes within the code without ending the string.
                      Keep everything in a single line; the \\n sequences will represent line breaks
                      when the string is processed or displayed.
                      """,
         name="execute_code",
     )
     async def execute_code(self, code: Annotated[str, "The valid Python code to execute"]) -> str:
-        """
-        Executes the provided Python code
+        """Executes the provided Python code.
+
         Args:
             code (str): The valid Python code to execute
         Returns:
             str: The result of the Python code execution in the form of Result, Stdout, and Stderr
         Raises:
-            FunctionExecutionException: If the provided code is empty
+            FunctionExecutionException: If the provided code is empty.
         """
-
         if not code:
             raise FunctionExecutionException("The provided code is empty")
 
         if self.settings.sanitize_input:
             code = self._sanitize_input(code)
 
         auth_token = await self._ensure_auth_token()
@@ -164,22 +163,23 @@
         return f"Result:\n{result['result']}Stdout:\n{result['stdout']}Stderr:\n{result['stderr']}"  # noqa: E501
 
     @kernel_function(name="upload_file", description="Uploads a file for the current Session ID")
     async def upload_file(
         self, *, data: BufferedReader = None, remote_file_path: str = None, local_file_path: str = None
     ) -> SessionsRemoteFileMetadata:
         """Upload a file to the session pool.
+
         Args:
             data (BufferedReader): The file data to upload.
             remote_file_path (str): The path to the file in the session.
             local_file_path (str): The path to the file on the local machine.
+
         Returns:
             RemoteFileMetadata: The metadata of the uploaded file.
         """
-
         if data and local_file_path:
             raise ValueError("data and local_file_path cannot be provided together")
 
         if local_file_path:
             if not remote_file_path:
                 remote_file_path = os.path.basename(local_file_path)
             data = open(local_file_path, "rb")
@@ -203,14 +203,15 @@
 
         response_json = response.json()
         return SessionsRemoteFileMetadata.from_dict(response_json)
 
     @kernel_function(name="list_files", description="Lists all files in the provided Session ID")
     async def list_files(self) -> list[SessionsRemoteFileMetadata]:
         """List the files in the session pool.
+
         Returns:
             list[SessionsRemoteFileMetadata]: The metadata for the files in the session pool
         """
         auth_token = await self._ensure_auth_token()
         self.http_client.headers.update(
             {
                 "Authorization": f"Bearer {auth_token}",
@@ -224,18 +225,20 @@
         response.raise_for_status()
 
         response_json = response.json()
         return [SessionsRemoteFileMetadata.from_dict(entry) for entry in response_json["$values"]]
 
     async def download_file(self, *, remote_file_path: str, local_file_path: str = None) -> BufferedReader | None:
         """Download a file from the session pool.
+
         Args:
             remote_file_path: The path to download the file from, relative to `/mnt/data`.
             local_file_path: The path to save the downloaded file to. If not provided, the
                 file is returned as a BufferedReader.
+
         Returns:
             BufferedReader: The data of the downloaded file.
         """
         auth_token = await self.auth_callback()
         self.http_client.headers.update(
             {
                 "Authorization": f"Bearer {auth_token}",
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_settings.py` & `semantic_kernel-1.0.3/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,20 +42,23 @@
         (Env var ACA_POOL_MANAGEMENT_ENDPOINT)
     """
 
     env_file_path: str | None = None
     pool_management_endpoint: HttpsUrl
 
     class Config:
+        """Configuration for the Azure Container Apps sessions settings."""
+
         env_prefix = "ACA_"
         env_file = None
         env_file_encoding = "utf-8"
         extra = "ignore"
         case_sensitive = False
 
     @classmethod
     def create(cls, **kwargs):
+        """Create an instance of the Azure Container Apps sessions settings."""
         if "env_file_path" in kwargs and kwargs["env_file_path"]:
             cls.Config.env_file = kwargs["env_file_path"]
         else:
             cls.Config.env_file = None
         return cls(**kwargs)
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py` & `semantic_kernel-1.0.3/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/core_plugins/text_memory_plugin.py` & `semantic_kernel-1.0.3/semantic_kernel/core_plugins/text_memory_plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,20 +19,19 @@
 
 
 class TextMemoryPlugin(KernelBaseModel):
     memory: SemanticTextMemoryBase
     embeddings_kwargs: dict[str, Any] = Field(default_factory=dict)
 
     def __init__(self, memory: SemanticTextMemoryBase, embeddings_kwargs: dict[str, Any] = {}) -> None:
-        """
-        Initialize a new instance of the TextMemoryPlugin
+        """Initialize a new instance of the TextMemoryPlugin.
 
         Args:
-            memory (SemanticTextMemoryBase) - the underlying Semantic Text Memory to use
-            embeddings_kwargs (Optional[Dict[str, Any]]) - the keyword arguments to pass to the embedding generator
+            memory (SemanticTextMemoryBase): the underlying Semantic Text Memory to use
+            embeddings_kwargs (Optional[Dict[str, Any]]): the keyword arguments to pass to the embedding generator
         """
         super().__init__(memory=memory, embeddings_kwargs=embeddings_kwargs)
 
     @kernel_function(
         description="Recall a fact from the long term memory",
         name="recall",
     )
@@ -41,25 +40,24 @@
         ask: Annotated[str, "The information to retrieve"],
         collection: Annotated[str, "The collection to search for information."] = DEFAULT_COLLECTION,
         relevance: Annotated[
             float, "The relevance score, from 0.0 to 1.0; 1.0 means perfect match"
         ] = DEFAULT_RELEVANCE,
         limit: Annotated[int, "The maximum number of relevant memories to recall."] = DEFAULT_LIMIT,
     ) -> str:
-        """
-        Recall a fact from the long term memory.
+        """Recall a fact from the long term memory.
 
         Example:
             {{memory.recall $ask}} => "Paris"
 
         Args:
-            ask -- The question to ask the memory
-            collection -- The collection to search for information
-            relevance -- The relevance score, from 0.0 to 1.0; 1.0 means perfect match
-            limit -- The maximum number of relevant memories to recall
+            ask: The question to ask the memory
+            collection: The collection to search for information
+            relevance: The relevance score, from 0.0 to 1.0; 1.0 means perfect match
+            limit: The maximum number of relevant memories to recall
 
         Returns:
             The nearest item from the memory store as a string or empty string if not found.
         """
         results = await self.memory.search(
             collection=collection,
             query=ask,
@@ -78,21 +76,19 @@
     )
     async def save(
         self,
         text: Annotated[str, "The information to save."],
         key: Annotated[str, "The unique key to associate with the information."],
         collection: Annotated[str, "The collection to save the information."] = DEFAULT_COLLECTION,
     ) -> None:
-        """
-        Save a fact to the long term memory.
+        """Save a fact to the long term memory.
 
         Args:
-            text -- The text to save to the memory
-            kernel -- The kernel instance, that has a memory store
-            collection -- The collection to save the information
-            key -- The unique key to associate with the information
+            text: The text to save to the memory
+            kernel: The kernel instance, that has a memory store
+            collection: The collection to save the information
+            key: The unique key to associate with the information
 
         """
-
         await self.memory.save_information(
             collection=collection, text=text, id=key, embeddings_kwargs=self.embeddings_kwargs
         )
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/core_plugins/text_plugin.py` & `semantic_kernel-1.0.3/semantic_kernel/core_plugins/text_plugin.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,84 +1,78 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from semantic_kernel.functions.kernel_function_decorator import kernel_function
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 
 class TextPlugin(KernelBaseModel):
-    """
-    TextPlugin provides a set of functions to manipulate strings.
+    """TextPlugin provides a set of functions to manipulate strings.
 
     Usage:
         kernel.add_plugin(TextPlugin(), plugin_name="text")
 
     Examples:
         KernelArguments["input"] = "  hello world  "
         {{text.trim $input}} => "hello world"
 
         KernelArguments["input"] = "  hello world  "
-        {{text.trimStart $input} => "hello world  "
+        {{text.trimStart $input}} => "hello world  "
 
         KernelArguments["input"] = "  hello world  "
-        {{text.trimEnd $input} => "  hello world"
+        {{text.trimEnd $input}} => "  hello world"
 
         KernelArguments["input"] = "hello world"
         {{text.uppercase $input}} => "HELLO WORLD"
 
         KernelArguments["input"] = "HELLO WORLD"
         {{text.lowercase $input}} => "hello world"
     """
 
     @kernel_function(description="Trim whitespace from the start and end of a string.")
     def trim(self, input: str) -> str:
-        """
-        Trim whitespace from the start and end of a string.
+        """Trim whitespace from the start and end of a string.
 
         Example:
             KernelArguments["input"] = "  hello world  "
             {{text.trim $input}} => "hello world"
         """
         return input.strip()
 
     @kernel_function(description="Trim whitespace from the start of a string.")
     def trim_start(self, input: str) -> str:
-        """
-        Trim whitespace from the start of a string.
+        """Trim whitespace from the start of a string.
 
-         Example:
+        Example:
              KernelArguments["input"] = "  hello world  "
              {{input.trim $input}} => "hello world  "
         """
         return input.lstrip()
 
     @kernel_function(description="Trim whitespace from the end of a string.")
     def trim_end(self, input: str) -> str:
-        """
-        Trim whitespace from the end of a string.
+        """Trim whitespace from the end of a string.
 
-         Example:
+        Example:
              KernelArguments["input"] = "  hello world  "
              {{input.trim $input}} => "  hello world"
         """
         return input.rstrip()
 
     @kernel_function(description="Convert a string to uppercase.")
     def uppercase(self, input: str) -> str:
-        """
-        Convert a string to uppercase.
+        """Convert a string to uppercase.
 
         Example:
             KernelArguments["input"] = "hello world"
              {{input.uppercase $input}} => "HELLO WORLD"
         """
         return input.upper()
 
     @kernel_function(description="Convert a string to lowercase.")
     def lowercase(self, input: str) -> str:
-        """
-        Convert a string to lowercase.
+        """Convert a string to lowercase.
 
-         Example:
+        Example:
              KernelArguments["input"] = "HELLO WORLD"
              {{input.lowercase $input}} => "hello world"
         """
         return input.lower()
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/core_plugins/time_plugin.py` & `semantic_kernel-1.0.3/semantic_kernel/core_plugins/time_plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 
 from semantic_kernel.exceptions import FunctionExecutionException
 from semantic_kernel.functions.kernel_function_decorator import kernel_function
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 
 class TimePlugin(KernelBaseModel):
-    """
-    Description: TimePlugin provides a set of functions
-                 to get the current time and date.
+    """TimePlugin provides a set of functions to get the current time and date.
 
     Usage:
         kernel.add_plugin(TimePlugin(), plugin_name="time")
 
     Examples:
         {{time.date}}            => Sunday, 12 January, 2031
         {{time.today}}           => Sunday, 12 January, 2031
@@ -37,228 +35,208 @@
         {{time.seconds}}         => 7
         {{time.timeZoneOffset}}  => -0800
         {{time.timeZoneName}}    => PST
     """
 
     @kernel_function(description="Get the current date.")
     def date(self) -> str:
-        """
-        Get the current date
+        """Get the current date.
 
         Example:
             {{time.date}} => Sunday, 12 January, 2031
         """
         now = datetime.datetime.now()
         return now.strftime("%A, %d %B, %Y")
 
     @kernel_function(description="Get the current date.")
     def today(self) -> str:
-        """
-        Get the current date
+        """Get the current date.
 
         Example:
             {{time.today}} => Sunday, 12 January, 2031
         """
         return self.date()
 
     @kernel_function(description="Get the current date in iso format.")
     def iso_date(self) -> str:
-        """
-        Get the current date in iso format
+        """Get the current date in iso format.
 
         Example:
             {{time.iso_date}} => 2031-01-12
         """
         today = datetime.date.today()
         return today.isoformat()
 
     @kernel_function(description="Get the current date and time in the local time zone")
     def now(self) -> str:
-        """
-        Get the current date and time in the local time zone"
+        """Get the current date and time in the local time zone.
 
         Example:
             {{time.now}} => Sunday, January 12, 2031 9:15 PM
         """
         now = datetime.datetime.now()
         return now.strftime("%A, %B %d, %Y %I:%M %p")
 
     @kernel_function(description="Get the current date and time in UTC", name="utcNow")
     def utc_now(self) -> str:
-        """
-        Get the current date and time in UTC
+        """Get the current date and time in UTC.
 
         Example:
             {{time.utcNow}} => Sunday, January 13, 2031 5:15 AM
         """
         now = datetime.datetime.utcnow()
         return now.strftime("%A, %B %d, %Y %I:%M %p")
 
     @kernel_function(description="Get the current time in the local time zone")
     def time(self) -> str:
-        """
-        Get the current time in the local time zone
+        """Get the current time in the local time zone.
 
         Example:
             {{time.time}} => 09:15:07 PM
         """
         now = datetime.datetime.now()
         return now.strftime("%I:%M:%S %p")
 
     @kernel_function(description="Get the current year")
     def year(self) -> str:
-        """
-        Get the current year
+        """Get the current year.
 
         Example:
             {{time.year}} => 2031
         """
         now = datetime.datetime.now()
         return now.strftime("%Y")
 
     @kernel_function(description="Get the current month")
     def month(self) -> str:
-        """
-        Get the current month
+        """Get the current month.
 
         Example:
             {{time.month}} => January
         """
         now = datetime.datetime.now()
         return now.strftime("%B")
 
     @kernel_function(description="Get the current month number")
     def month_number(self) -> str:
-        """
-        Get the current month number
+        """Get the current month number.
 
         Example:
             {{time.monthNumber}} => 01
         """
         now = datetime.datetime.now()
         return now.strftime("%m")
 
     @kernel_function(description="Get the current day")
     def day(self) -> str:
-        """
-        Get the current day of the month
+        """Get the current day of the month.
 
         Example:
             {{time.day}} => 12
         """
         now = datetime.datetime.now()
         return now.strftime("%d")
 
     @kernel_function(description="Get the current day of the week", name="dayOfWeek")
     def day_of_week(self) -> str:
-        """
-        Get the current day of the week
+        """Get the current day of the week.
 
         Example:
             {{time.dayOfWeek}} => Sunday
         """
         now = datetime.datetime.now()
         return now.strftime("%A")
 
     @kernel_function(description="Get the current hour")
     def hour(self) -> str:
-        """
-        Get the current hour
+        """Get the current hour.
 
         Example:
             {{time.hour}} => 9 PM
         """
         now = datetime.datetime.now()
         return now.strftime("%I %p")
 
     @kernel_function(description="Get the current hour number", name="hourNumber")
     def hour_number(self) -> str:
-        """
-        Get the current hour number
+        """Get the current hour number.
 
         Example:
             {{time.hourNumber}} => 21
         """
         now = datetime.datetime.now()
         return now.strftime("%H")
 
     @kernel_function(description="Get the current minute")
     def minute(self) -> str:
-        """
-        Get the current minute
+        """Get the current minute.
 
         Example:
             {{time.minute}} => 15
         """
         now = datetime.datetime.now()
         return now.strftime("%M")
 
     @kernel_function(description="Get the date of offset from today by a provided number of days")
     def days_ago(self, days: str) -> str:
-        """
-        Get the date a provided number of days in the past
+        """Get the date a provided number of days in the past.
 
-        params:
+        Args:
             days: The number of days to offset from today
-        returns:
+        Returns:
             The date of the offset day.
 
         Example:
-             KernelContext["input"] = "3"
              {{time.days_ago $input}} => Sunday, 7 May, 2023
         """
         d = datetime.date.today() - datetime.timedelta(days=int(days))
         return d.strftime("%A, %d %B, %Y")
 
     @kernel_function(description="""Get the date of the last day matching the supplied week day name in English.""")
     def date_matching_last_day_name(self, day_name: str) -> str:
-        """
-        Get the date of the last day matching the supplied day name
+        """Get the date of the last day matching the supplied day name.
 
-        params:
+        Args:
             day_name: The day name to match with.
-        returns:
+
+        Returns:
             The date of the matching day.
 
         Example:
-             KernelContext["input"] = "Sunday"
              {{time.date_matching_last_day_name $input}} => Sunday, 7 May, 2023
         """
         d = datetime.date.today()
         for i in range(1, 8):
             d = d - datetime.timedelta(days=1)
             if d.strftime("%A") == day_name:
                 return d.strftime("%A, %d %B, %Y")
         raise FunctionExecutionException("day_name is not recognized")
 
     @kernel_function(description="Get the seconds on the current minute")
     def second(self) -> str:
-        """
-        Get the seconds on the current minute
+        """Get the seconds on the current minute.
 
         Example:
             {{time.second}} => 7
         """
         now = datetime.datetime.now()
         return now.strftime("%S")
 
     @kernel_function(description="Get the current time zone offset", name="timeZoneOffset")
     def time_zone_offset(self) -> str:
-        """
-        Get the current time zone offset
+        """Get the current time zone offset.
 
         Example:
             {{time.timeZoneOffset}} => -08:00
         """
         now = datetime.datetime.now()
         return now.strftime("%z")
 
     @kernel_function(description="Get the current time zone name", name="timeZoneName")
     def time_zone_name(self) -> str:
-        """
-        Get the current time zone name
+        """Get the current time zone name.
 
         Example:
             {{time.timeZoneName}} => PST
         """
         now = datetime.datetime.now()
         return now.strftime("%Z")
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/core_plugins/wait_plugin.py` & `semantic_kernel-1.0.3/semantic_kernel/core_plugins/wait_plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
 from semantic_kernel.exceptions import FunctionExecutionException
 from semantic_kernel.functions.kernel_function_decorator import kernel_function
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 
 class WaitPlugin(KernelBaseModel):
-    """
-    WaitPlugin provides a set of functions to wait for a certain amount of time.
+    """WaitPlugin provides a set of functions to wait for a certain amount of time.
 
     Usage:
         kernel.add_plugin(WaitPlugin(), plugin_name="wait")
 
     Examples:
         {{wait.wait 5}} => Wait for 5 seconds
     """
 
-    @kernel_function(description="Wait for a certain number of seconds.")
+    @kernel_function
     async def wait(self, input: Annotated[float | str, "The number of seconds to wait, can be str or float."]) -> None:
+        """Wait for a certain number of seconds."""
         if isinstance(input, str):
             try:
                 input = float(input)
             except ValueError as exc:
                 raise FunctionExecutionException("seconds text must be a number") from exc
         await asyncio.sleep(abs(input))
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/exceptions/__init__.py` & `semantic_kernel-1.0.3/semantic_kernel/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/exceptions/content_exceptions.py` & `semantic_kernel-1.0.3/semantic_kernel/exceptions/content_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/exceptions/function_exceptions.py` & `semantic_kernel-1.0.3/semantic_kernel/exceptions/function_exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 class FunctionSyntaxError(FunctionException):
     pass
 
 
 class FunctionInitializationError(FunctionException):
     def __init__(self, message: str):
+        """Raised when a KernelFunction fails to initialize."""
         super().__init__("KernelFunction failed to initialize: " + message)
 
 
 class PluginInitializationError(FunctionException):
     pass
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/exceptions/kernel_exceptions.py` & `semantic_kernel-1.0.3/semantic_kernel/exceptions/kernel_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/exceptions/planner_exceptions.py` & `semantic_kernel-1.0.3/semantic_kernel/exceptions/planner_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/exceptions/service_exceptions.py` & `semantic_kernel-1.0.3/semantic_kernel/exceptions/service_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/exceptions/template_engine_exceptions.py` & `semantic_kernel-1.0.3/semantic_kernel/exceptions/template_engine_exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,47 +14,51 @@
 
 class BlockRenderException(BlockException):
     pass
 
 
 class VarBlockSyntaxError(BlockSyntaxError):
     def __init__(self, content: str) -> None:
+        """Raised when the content of a VarBlock is invalid."""
         super().__init__(
             f"A VarBlock starts with a '$' followed by at least one letter, \
 number or underscore, anything else is invalid. \
 The content provided was: {content}",
         )
 
 
 class VarBlockRenderError(BlockRenderException):
     pass
 
 
 class ValBlockSyntaxError(BlockSyntaxError):
     def __init__(self, content: str) -> None:
+        """Raised when the content of a ValBlock is invalid."""
         super().__init__(
             f"A ValBlock starts with a single or double quote followed by at least one letter, \
 finishing with the same type of quote as the first one. \
 The content provided was: {content}",
         )
 
 
 class NamedArgBlockSyntaxError(BlockSyntaxError):
     def __init__(self, content: str) -> None:
+        """Raised when the content of a NamedArgBlock is invalid."""
         super().__init__(
             f"A NamedArgBlock starts with a name (letters, numbers or underscore) \
 followed by a single equal sign, then the value of the argument, \
 which can either be a VarBlock (starting with '$') \
 or a ValBlock (text surrounded by quotes). \
 The content provided was: {content}",
         )
 
 
 class FunctionIdBlockSyntaxError(BlockSyntaxError):
     def __init__(self, content: str) -> None:
+        """Raised when the content of a FunctionIdBlock is invalid."""
         super().__init__(
             f"A FunctionIdBlock is composed of either a plugin name and \
 function name separated by a single dot, or just a function name. \
 Both plugin and function names can only contain letters, numbers and underscores. \
 The content provided was: {content}",
         )
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/filters/auto_function_invocation/auto_function_invocation_context.py` & `semantic_kernel-1.0.3/semantic_kernel/filters/auto_function_invocation/auto_function_invocation_context.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/filters/filter_context_base.py` & `semantic_kernel-1.0.3/semantic_kernel/filters/filter_context_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/filters/kernel_filters_extension.py` & `semantic_kernel-1.0.3/semantic_kernel/filters/kernel_filters_extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,15 @@
                     return
 
     def construct_call_stack(
         self,
         filter_type: FilterTypes,
         inner_function: Callable[[FILTER_CONTEXT_TYPE], Coroutine[Any, Any, None]],
     ) -> Callable[[FILTER_CONTEXT_TYPE], Coroutine[Any, Any, None]]:
+        """Construct the call stack for the given filter type."""
         stack: list[Any] = [inner_function]
         for _, filter in getattr(self, FILTER_MAPPING[filter_type]):
             filter_with_next = partial(filter, next=stack[0])
             stack.insert(0, filter_with_next)
         return stack[0]
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/functions/__init__.py` & `semantic_kernel-1.0.3/semantic_kernel/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/functions/function_result.py` & `semantic_kernel-1.0.3/semantic_kernel/functions/function_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class FunctionResult(KernelBaseModel):
     """The result of a function.
 
-    Arguments:
+    Args:
         function (KernelFunctionMetadata): The metadata of the function that was invoked.
         value (Any): The value of the result.
         metadata (Mapping[str, Any]): The metadata of the result.
 
     Methods:
         __str__: Get the string representation of the result, will call str() on the value,
             or if the value is a list, will call str() on the first element of the list.
@@ -52,15 +52,15 @@
                 raise FunctionResultError(f"Failed to convert value to string: {e}") from e
         else:
             return ""
 
     def get_inner_content(self, index: int = 0) -> Any | None:
         """Get the inner content of the function result.
 
-        Arguments:
+        Args:
             index (int): The index of the inner content if the inner content is a list, default 0.
         """
         if isinstance(self.value, list):
             if isinstance(self.value[index], KernelContent):
                 return self.value[index].inner_content
         if isinstance(self.value, KernelContent):
             return self.value.inner_content
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/functions/kernel_arguments.py` & `semantic_kernel-1.0.3/semantic_kernel/functions/kernel_arguments.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,27 @@
     def __init__(
         self,
         settings: (
             "PromptExecutionSettings | list[PromptExecutionSettings] | dict[str, PromptExecutionSettings] | None"
         ) = None,
         **kwargs: Any,
     ):
-        """Initializes a new instance of the KernelArguments class,
-        this is a dict-like class with the additional field for the execution_settings.
+        """Initializes a new instance of the KernelArguments class.
+
+        This is a dict-like class with the additional field for the execution_settings.
 
         This class is derived from a dict, hence behaves the same way,
         just adds the execution_settings as a dict, with service_id and the settings.
 
-        Arguments:
-            settings (PromptExecutionSettings | List[PromptExecutionSettings] | None) --
+        Args:
+            settings (PromptExecutionSettings | List[PromptExecutionSettings] | None):
                 The settings for the execution.
                 If a list is given, make sure all items in the list have a unique service_id
                 as that is used as the key for the dict.
-            **kwargs (dict[str, Any]) -- The arguments for the function invocation, works similar to a regular dict.
+            **kwargs (dict[str, Any]): The arguments for the function invocation, works similar to a regular dict.
         """
         super().__init__(**kwargs)
         settings_dict = None
         if settings:
             settings_dict = {}
             if isinstance(settings, dict):
                 settings_dict = settings
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/functions/kernel_function.py` & `semantic_kernel-1.0.3/semantic_kernel/functions/kernel_function.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,16 +41,15 @@
     KERNEL_TEMPLATE_FORMAT_NAME: KernelPromptTemplate,
     HANDLEBARS_TEMPLATE_FORMAT_NAME: HandlebarsPromptTemplate,
     JINJA2_TEMPLATE_FORMAT_NAME: Jinja2PromptTemplate,
 }
 
 
 class KernelFunction(KernelBaseModel):
-    """
-    Semantic Kernel function.
+    """Semantic Kernel function.
 
     Attributes:
         name (str): The name of the function. Must be upper/lower case letters and
             underscores with a minimum length of 1.
         plugin_name (str): The name of the plugin that contains this function. Must be upper/lower
             case letters and underscores with a minimum length of 1.
         description (Optional[str]): The description of the function.
@@ -78,17 +77,15 @@
         template_format: TEMPLATE_FORMAT_TYPES = KERNEL_TEMPLATE_FORMAT_NAME,
         prompt_template: "PromptTemplateBase | None " = None,
         prompt_template_config: "PromptTemplateConfig | None" = None,
         prompt_execution_settings: (
             "PromptExecutionSettings | list[PromptExecutionSettings] | dict[str, PromptExecutionSettings] | None"
         ) = None,
     ) -> "KernelFunctionFromPrompt":
-        """
-        Create a new instance of the KernelFunctionFromPrompt class.
-        """
+        """Create a new instance of the KernelFunctionFromPrompt class."""
         from semantic_kernel.functions.kernel_function_from_prompt import KernelFunctionFromPrompt
 
         return KernelFunctionFromPrompt(
             function_name=function_name,
             plugin_name=plugin_name,
             description=description,
             prompt=prompt,
@@ -101,66 +98,72 @@
     @classmethod
     def from_method(
         cls,
         method: Callable[..., Any],
         plugin_name: str | None = None,
         stream_method: Callable[..., Any] | None = None,
     ) -> "KernelFunctionFromMethod":
-        """
-        Create a new instance of the KernelFunctionFromMethod class.
-        """
+        """Create a new instance of the KernelFunctionFromMethod class."""
         from semantic_kernel.functions.kernel_function_from_method import KernelFunctionFromMethod
 
         return KernelFunctionFromMethod(
             plugin_name=plugin_name,
             method=method,
             stream_method=stream_method,
         )
 
     @property
     def name(self) -> str:
+        """The name of the function."""
         return self.metadata.name
 
     @property
     def plugin_name(self) -> str:
+        """The name of the plugin that contains this function."""
         return self.metadata.plugin_name or ""
 
     @property
     def fully_qualified_name(self) -> str:
+        """The fully qualified name of the function."""
         return self.metadata.fully_qualified_name
 
     @property
     def description(self) -> str | None:
+        """The description of the function."""
         return self.metadata.description
 
     @property
     def is_prompt(self) -> bool:
+        """Whether the function is based on a prompt."""
         return self.metadata.is_prompt
 
     @property
     def parameters(self) -> list["KernelParameterMetadata"]:
+        """The parameters for the function."""
         return self.metadata.parameters
 
     @property
     def return_parameter(self) -> "KernelParameterMetadata | None":
+        """The return parameter for the function."""
         return self.metadata.return_parameter
 
     async def __call__(
         self,
         kernel: "Kernel",
         arguments: "KernelArguments | None" = None,
         metadata: dict[str, Any] = {},
         **kwargs: Any,
     ) -> FunctionResult | None:
         """Invoke the function with the given arguments.
 
         Args:
             kernel (Kernel): The kernel
-            arguments (Optional[KernelArguments]): The Kernel arguments.
+            arguments (KernelArguments | None): The Kernel arguments.
                 Optional, defaults to None.
+            metadata (Dict[str, Any]): Additional metadata.
             kwargs (Dict[str, Any]): Additional keyword arguments that will be
 
         Returns:
             FunctionResult: The result of the function
         """
         return await self.invoke(kernel, arguments, metadata, **kwargs)
 
@@ -185,14 +188,15 @@
         **kwargs: Any,
     ) -> "FunctionResult | None":
         """Invoke the function with the given arguments.
 
         Args:
             kernel (Kernel): The kernel
             arguments (KernelArguments): The Kernel arguments
+            metadata (Dict[str, Any]): Additional metadata.
             kwargs (Any): Additional keyword arguments that will be
                 added to the KernelArguments.
 
         Returns:
             FunctionResult: The result of the function
         """
         if arguments is None:
@@ -220,25 +224,25 @@
     async def invoke_stream(
         self,
         kernel: "Kernel",
         arguments: "KernelArguments | None" = None,
         metadata: dict[str, Any] = {},
         **kwargs: Any,
     ) -> "AsyncGenerator[FunctionResult | list[StreamingContentMixin | Any], Any]":
-        """
-        Invoke a stream async function with the given arguments.
+        """Invoke a stream async function with the given arguments.
 
         Args:
             kernel (Kernel): The kernel
             arguments (KernelArguments): The Kernel arguments
+            metadata (Dict[str, Any]): Additional metadata.
             kwargs (Any): Additional keyword arguments that will be
                 added to the KernelArguments.
 
         Yields:
-            KernelContent with the StreamingKernelMixin or FunctionResult --
+            KernelContent with the StreamingKernelMixin or FunctionResult:
                 The results of the function,
                 if there is an error a FunctionResult is yielded.
         """
         if arguments is None:
             arguments = KernelArguments(**kwargs)
         _rebuild_function_invocation_context()
         function_context = FunctionInvocationContext(function=self, kernel=kernel, arguments=arguments)
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/functions/kernel_function_decorator.py` & `semantic_kernel-1.0.3/semantic_kernel/functions/kernel_function_decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 
 
 def kernel_function(
     func: Callable[..., object] | None = None,
     name: str | None = None,
     description: str | None = None,
 ) -> Callable[..., Any]:
-    """
-    Decorator for kernel functions, can be used directly as @kernel_function
+    """Decorator for kernel functions.
+
+    Can be used directly as @kernel_function
     or with parameters @kernel_function(name='function', description='I am a function.').
 
     This decorator is used to mark a function as a kernel function. It also provides metadata for the function.
     The name and description can be left empty, and then the function name and docstring will be used.
 
     The parameters are parsed from the function signature, use typing.Annotated to provide a description for the
     parameter, in python 3.8, use typing_extensions.Annotated.
@@ -33,21 +34,23 @@
     and that is stored in __kernel_function_return_type__, __kernel_function_return_description__
     and __kernel_function_return_required__.
 
     It also checks if the function is a streaming type (generator or iterable, async or not),
     and that is stored as a bool in __kernel_function_streaming__.
 
     Args:
-        name (str | None) -- The name of the function, if not supplied, the function name will be used.
-        description (str | None) -- The description of the function,
+        func (Callable[..., object] | None): The function to decorate, can be None (if used as @kernel_function
+        name (str | None): The name of the function, if not supplied, the function name will be used.
+        description (str | None): The description of the function,
             if not supplied, the function docstring will be used, can be None.
 
     """
 
     def decorator(func: Callable[..., object]) -> Callable[..., object]:
+        """The actual decorator function."""
         setattr(func, "__kernel_function__", True)
         setattr(func, "__kernel_function_description__", description or func.__doc__)
         setattr(func, "__kernel_function_name__", name or getattr(func, "__name__", "unknown"))
         setattr(func, "__kernel_function_streaming__", isasyncgenfunction(func) or isgeneratorfunction(func))
         logger.debug(f"Parsing decorator for function: {getattr(func, '__kernel_function_name__')}")
         func_sig = signature(func, eval_str=True)
         annotations = []
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/functions/kernel_function_extension.py` & `semantic_kernel-1.0.3/semantic_kernel/functions/kernel_function_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,17 +51,17 @@
         self,
         plugin: KernelPlugin | object | dict[str, Any] | None = None,
         plugin_name: str | None = None,
         parent_directory: str | None = None,
         description: str | None = None,
         class_init_arguments: dict[str, dict[str, Any]] | None = None,
     ) -> "KernelPlugin":
-        """
-        Adds a plugin to the kernel's collection of plugins. If a plugin is provided,
-        it uses that instance instead of creating a new KernelPlugin.
+        """Adds a plugin to the kernel's collection of plugins.
+
+        If a plugin is provided, it uses that instance instead of creating a new KernelPlugin.
         See KernelPlugin.from_directory for more details on how the directory is parsed.
 
         Args:
             plugin (KernelPlugin | Any | dict[str, Any]): The plugin to add.
                 This can be a KernelPlugin, in which case it is added straightaway and other parameters are ignored,
                 a custom class that contains methods with the kernel_function decorator
                 or a dictionary of functions with the kernel_function decorator for one or
@@ -98,16 +98,15 @@
                 description=description,
                 class_init_arguments=class_init_arguments,
             )
             return self.plugins[plugin_name]
         raise ValueError("plugin or parent_directory must be provided.")
 
     def add_plugins(self, plugins: list[KernelPlugin] | dict[str, KernelPlugin | object]) -> None:
-        """
-        Adds a list of plugins to the kernel's collection of plugins.
+        """Adds a list of plugins to the kernel's collection of plugins.
 
         Args:
             plugins (list[KernelPlugin] | dict[str, KernelPlugin]): The plugins to add to the kernel
         """
         if isinstance(plugins, list):
             for plug in plugins:
                 self.add_plugin(plug)
@@ -127,28 +126,25 @@
             PromptExecutionSettings | list[PromptExecutionSettings] | dict[str, PromptExecutionSettings] | None
         ) = None,
         template_format: TEMPLATE_FORMAT_TYPES = KERNEL_TEMPLATE_FORMAT_NAME,
         prompt_template: PromptTemplateBase | None = None,
         return_plugin: bool = False,
         **kwargs: Any,
     ) -> "KernelFunction | KernelPlugin":
-        """
-        Adds a function to the specified plugin.
+        """Adds a function to the specified plugin.
 
         Args:
             plugin_name (str): The name of the plugin to add the function to
             function (KernelFunction | Callable[..., Any]): The function to add
             function_name (str): The name of the function
             plugin_name (str): The name of the plugin
             description (str | None): The description of the function
             prompt (str | None): The prompt template.
             prompt_template_config (PromptTemplateConfig | None): The prompt template configuration
-            prompt_execution_settings (PromptExecutionSettings  | list[PromptExecutionSettings]
-                | dict[str, PromptExecutionSettings] | None):
-                The execution settings, will be parsed into a dict.
+            prompt_execution_settings: The execution settings, will be parsed into a dict.
             template_format (str | None): The format of the prompt template
             prompt_template (PromptTemplateBase | None): The prompt template
             return_plugin (bool): If True, the plugin is returned instead of the function
             kwargs (Any): Additional arguments
 
         Returns:
             KernelFunction | KernelPlugin: The function that was added, or the plugin if return_plugin is True
@@ -186,16 +182,15 @@
         return self.plugins[plugin_name] if return_plugin else self.plugins[plugin_name][function.name]
 
     def add_functions(
         self,
         plugin_name: str,
         functions: "list[KERNEL_FUNCTION_TYPE] | dict[str, KERNEL_FUNCTION_TYPE]",
     ) -> "KernelPlugin":
-        """
-        Adds a list of functions to the specified plugin.
+        """Adds a list of functions to the specified plugin.
 
         Args:
             plugin_name (str): The name of the plugin to add the functions to
             functions (list[KernelFunction] | dict[str, KernelFunction]): The functions to add
 
         Returns:
             KernelPlugin: The plugin that the functions were added to.
@@ -213,17 +208,17 @@
         execution_settings: "OpenAPIFunctionExecutionParameters | None" = None,
         description: str | None = None,
     ) -> KernelPlugin:
         """Add a plugin from the Open AI manifest.
 
         Args:
             plugin_name (str): The name of the plugin
-            plugin_url (str | None): The URL of the plugin
-            plugin_str (str | None): The JSON string of the plugin
-            execution_parameters (OpenAIFunctionExecutionParameters | None): The execution parameters
+            openapi_document_path (str): The path to the OpenAPI document
+            execution_settings (OpenAPIFunctionExecutionParameters | None): The execution parameters
+            description (str | None): The description of the plugin
 
         Returns:
             KernelPlugin: The imported plugin
 
         Raises:
             PluginInitializationError: if the plugin URL or plugin JSON/YAML is not provided
         """
@@ -347,16 +342,15 @@
         """Get a list of all function metadata in the plugin collection."""
         raise NotImplementedError("This method is not implemented for the provided arguments.")
 
     @get_list_of_function_metadata.register(bool)
     def get_list_of_function_metadata_bool(
         self, include_prompt: bool = True, include_native: bool = True
     ) -> list["KernelFunctionMetadata"]:
-        """
-        Get a list of the function metadata in the plugin collection
+        """Get a list of the function metadata in the plugin collection.
 
         Args:
             include_prompt (bool): Whether to include semantic functions in the list.
             include_native (bool): Whether to include native functions in the list.
 
         Returns:
             A list of KernelFunctionMetadata objects in the collection.
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/functions/kernel_function_from_method.py` & `semantic_kernel-1.0.3/semantic_kernel/functions/kernel_function_from_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,30 +16,27 @@
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class KernelFunctionFromMethod(KernelFunction):
     """Semantic Kernel Function from a method."""
 
-    # some attributes are now properties, still listed here for documentation purposes
-
     method: Callable[..., Any]
     stream_method: Callable[..., Any] | None = None
 
     def __init__(
         self,
         method: Callable[..., Any],
         plugin_name: str | None = None,
         stream_method: Callable[..., Any] | None = None,
         parameters: list[KernelParameterMetadata] | None = None,
         return_parameter: KernelParameterMetadata | None = None,
         additional_metadata: dict[str, Any] | None = None,
     ) -> None:
-        """
-        Initializes a new instance of the KernelFunctionFromMethod class
+        """Initializes a new instance of the KernelFunctionFromMethod class.
 
         Args:
             method (Callable[..., Any]): The method to be called
             plugin_name (str | None): The name of the plugin
             stream_method (Callable[..., Any] | None): The stream method for the function
             parameters (list[KernelParameterMetadata] | None): The parameters of the function
             return_parameter (KernelParameterMetadata | None): The return parameter of the function
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/functions/kernel_function_from_prompt.py` & `semantic_kernel-1.0.3/semantic_kernel/functions/kernel_function_from_prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,16 +59,15 @@
         template_format: TEMPLATE_FORMAT_TYPES = KERNEL_TEMPLATE_FORMAT_NAME,
         prompt_template: PromptTemplateBase | None = None,
         prompt_template_config: PromptTemplateConfig | None = None,
         prompt_execution_settings: None | (
             PromptExecutionSettings | list[PromptExecutionSettings] | dict[str, PromptExecutionSettings]
         ) = None,
     ) -> None:
-        """
-        Initializes a new instance of the KernelFunctionFromPrompt class
+        """Initializes a new instance of the KernelFunctionFromPrompt class.
 
         Args:
             function_name (str): The name of the function
             plugin_name (str): The name of the plugin
             description (str): The description for the function
 
             prompt (Optional[str]): The prompt
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/functions/kernel_function_metadata.py` & `semantic_kernel-1.0.3/semantic_kernel/functions/kernel_function_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,23 @@
     is_prompt: bool
     is_asynchronous: bool | None = Field(default=True)
     return_parameter: KernelParameterMetadata | None = None
     additional_properties: dict[str, Any] | None = Field(default=None)
 
     @property
     def fully_qualified_name(self) -> str:
-        """
-        Get the fully qualified name of the function.
+        """Get the fully qualified name of the function.
 
         Returns:
             The fully qualified name of the function.
         """
         return f"{self.plugin_name}-{self.name}" if self.plugin_name else self.name
 
     def __eq__(self, other: object) -> bool:
-        """
-        Compare to another KernelFunctionMetadata instance.
+        """Compare to another KernelFunctionMetadata instance.
 
         Args:
             other (KernelFunctionMetadata): The other KernelFunctionMetadata instance.
 
         Returns:
             True if the two instances are equal, False otherwise.
         """
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/functions/kernel_parameter_metadata.py` & `semantic_kernel-1.0.3/semantic_kernel/functions/kernel_parameter_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-
 from typing import Any
 
 from pydantic import Field, model_validator
 
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 from semantic_kernel.schema.kernel_json_schema_builder import KernelJsonSchemaBuilder
 from semantic_kernel.utils.validation import FUNCTION_PARAM_NAME_REGEX
@@ -18,28 +17,30 @@
     is_required: bool | None = False
     type_object: Any | None = None
     schema_data: dict[str, Any] | None = None
 
     @model_validator(mode="before")
     @classmethod
     def form_schema(cls, data: Any) -> Any:
+        """Create a schema for the parameter metadata."""
         if isinstance(data, dict):
             if data.get("schema_data") is None:
                 type_object = data.get("type_object", None)
                 type_ = data.get("type_", None)
                 default_value = data.get("default_value", None)
                 description = data.get("description", None)
                 inferred_schema = cls.infer_schema(type_object, type_, default_value, description)
                 data["schema_data"] = inferred_schema
         return data
 
     @classmethod
     def infer_schema(
         cls, type_object: type | None, parameter_type: str | None, default_value: Any, description: str | None
     ) -> dict[str, Any] | None:
+        """Infer the schema for the parameter metadata."""
         schema = None
 
         if type_object is not None:
             schema = KernelJsonSchemaBuilder.build(type_object, description)
         elif parameter_type is not None:
             string_default = str(default_value) if default_value is not None else None
             if string_default and string_default.strip():
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/functions/kernel_plugin.py` & `semantic_kernel-1.0.3/semantic_kernel/functions/kernel_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,15 @@
     )
     from semantic_kernel.functions.kernel_function_metadata import KernelFunctionMetadata
 
 logger = logging.getLogger(__name__)
 
 
 class KernelPlugin(KernelBaseModel):
-    """
-    Represents a Kernel Plugin with functions.
+    """Represents a Kernel Plugin with functions.
 
     This class behaves mostly like a dictionary, with functions as values and their names as keys.
     When you add a function, through `.set` or `__setitem__`, the function is copied, the metadata is deep-copied
     and the name of the plugin is set in the metadata and added to the dict of functions.
     This is done in the same way as a normal dict, so a existing key will be overwritten.
 
     Attributes:
@@ -100,15 +99,15 @@
             KERNEL_FUNCTION_TYPE
             | "KernelPlugin"
             | list[KERNEL_FUNCTION_TYPE | "KernelPlugin"]
             | dict[str, KERNEL_FUNCTION_TYPE]
             | None
         ) = None,
     ):
-        """Create a KernelPlugin
+        """Create a KernelPlugin.
 
         Args:
             name: The name of the plugin. The name can be upper/lower
                 case letters and underscores.
             description: The description of the plugin.
             functions:
                 The functions in the plugin, will be rewritten to a dictionary of functions.
@@ -180,14 +179,15 @@
                 self.add(args[0].functions)
             else:
                 self.add(args[0])
         self.add(kwargs)
 
     @singledispatchmethod
     def add(self, functions: Any) -> None:
+        """Add functions to the plugin."""
         raise TypeError(f"Unknown type being added, type was {type(functions)}")
 
     @add.register(list)
     def add_list(self, functions: list[KERNEL_FUNCTION_TYPE | "KernelPlugin"]) -> None:
         """Add a list of functions to the plugin."""
         for function in functions:
             if isinstance(function, KernelPlugin):
@@ -199,54 +199,58 @@
     @add.register(dict)
     def add_dict(self, functions: dict[str, KERNEL_FUNCTION_TYPE]) -> None:
         """Add a dictionary of functions to the plugin."""
         for name, function in functions.items():
             self[name] = function
 
     def setdefault(self, key: str, value: KernelFunction | None = None):
+        """Set a default value for a key."""
         if key not in self.functions:
             if value is None:
                 raise ValueError("Value must be provided for new key.")
             self[key] = value
         return self[key]
 
     def __iter__(self) -> Generator[KernelFunction, None, None]:  # type: ignore
         """Iterate over the functions in the plugin."""
         yield from self.functions.values()
 
     def __contains__(self, key: str) -> bool:
+        """Check if a function is in the plugin."""
         return key in self.functions
 
     # endregion
     # region Properties
 
     def get_functions_metadata(self) -> list["KernelFunctionMetadata"]:
-        """
-        Get the metadata for the functions in the plugin.
+        """Get the metadata for the functions in the plugin.
 
         Returns:
             A list of KernelFunctionMetadata instances.
         """
         return [func.metadata for func in self]
 
     # endregion
     # region Class Methods
 
     @classmethod
     def from_object(
-        cls, plugin_name: str, plugin_instance: Any | dict[str, Any], description: str | None = None
+        cls,
+        plugin_name: str,
+        plugin_instance: Any | dict[str, Any],
+        description: str | None = None,
     ) -> "KernelPlugin":
-        """
-        Creates a plugin that wraps the specified target object and imports it into the kernel's plugin collection
+        """Creates a plugin that wraps the specified target object and imports it into the kernel's plugin collection.
 
         Args:
+            plugin_name (str): The name of the plugin. Allows chars: upper, lower ASCII and underscores.
             plugin_instance (Any | dict[str, Any]): The plugin instance. This can be a custom class or a
                 dictionary of classes that contains methods with the kernel_function decorator for one or
                 several methods. See `TextMemoryPlugin` as an example.
-            plugin_name (str): The name of the plugin. Allows chars: upper, lower ASCII and underscores.
+            description (str | None): The description of the plugin.
 
         Returns:
             KernelPlugin: The imported plugin of type KernelPlugin.
         """
         functions: list[KernelFunction] = []
         candidates: list[tuple[str, MethodType]] | ItemsView[str, Any] = []
 
@@ -361,26 +365,24 @@
         execution_settings: "OpenAPIFunctionExecutionParameters | None" = None,
         description: str | None = None,
     ) -> "KernelPlugin":
         """Create a plugin from an OpenAPI document.
 
         Args:
             plugin_name (str): The name of the plugin
-            plugin_url (str | None): The URL of the plugin
-            plugin_str (str | None): The JSON string of the plugin
-            execution_parameters (OpenAIFunctionExecutionParameters | None): The execution parameters
+            openapi_document_path (str): The path to the OpenAPI document
+            execution_settings (OpenAPIFunctionExecutionParameters | None): The execution parameters
             description (str | None): The description of the plugin
 
         Returns:
             KernelPlugin: The created plugin
 
         Raises:
             PluginInitializationError: if the plugin URL or plugin JSON/YAML is not provided
         """
-
         if not openapi_document_path:
             raise PluginInitializationError("OpenAPI document path is required.")
 
         return cls(  # type: ignore
             name=plugin_name,
             description=description,
             functions=create_functions_from_openapi(  # type: ignore
@@ -402,22 +404,22 @@
         """Create a plugin from the Open AI manifest.
 
         Args:
             plugin_name (str): The name of the plugin
             plugin_url (str | None): The URL of the plugin
             plugin_str (str | None): The JSON string of the plugin
             execution_parameters (OpenAIFunctionExecutionParameters | None): The execution parameters
+            description (str | None): The description of the plugin
 
         Returns:
             KernelPlugin: The created plugin
 
         Raises:
             PluginInitializationError: if the plugin URL or plugin JSON/YAML is not provided
         """
-
         if execution_parameters is None:
             execution_parameters = OpenAIFunctionExecutionParameters()
 
         if plugin_str is not None:
             # Load plugin from the provided JSON string/YAML string
             openai_manifest = plugin_str
         elif plugin_url is not None:
@@ -459,14 +461,15 @@
     def from_python_file(
         cls,
         plugin_name: str,
         py_file: str,
         description: str | None = None,
         class_init_arguments: dict[str, dict[str, Any]] | None = None,
     ) -> "KernelPlugin":
+        """Create a plugin from a Python file."""
         module_name = os.path.basename(py_file).replace(".py", "")
         spec = importlib.util.spec_from_file_location(module_name, py_file)
         if not spec:
             raise PluginInitializationError(f"Could not load spec from file {py_file}")
         module = importlib.util.module_from_spec(spec)
         if not module or not spec.loader:
             raise PluginInitializationError(f"No module found in file {py_file}")
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/functions/prompt_rendering_result.py` & `semantic_kernel-1.0.3/semantic_kernel/functions/prompt_rendering_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.functions.function_result import FunctionResult
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 from semantic_kernel.services.ai_service_client_base import AIServiceClientBase
 
 
 class PromptRenderingResult(KernelBaseModel):
-    """
-    Represents the result of rendering a prompt template.
+    """Represents the result of rendering a prompt template.
 
     Attributes:
         rendered_prompt (str): The rendered prompt.
         ai_service (Any): The AI service that rendered the prompt.
         execution_settings (PromptExecutionSettings): The execution settings for the prompt.
         function_result (FunctionResult): The result of executing the prompt.
     """
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/kernel.py` & `semantic_kernel-1.0.3/semantic_kernel/kernel.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,16 +28,17 @@
     from semantic_kernel.functions.kernel_function import KernelFunction
 
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class Kernel(KernelFilterExtension, KernelFunctionExtension, KernelServicesExtension, KernelReliabilityExtension):
-    """
-    The Kernel class is the main entry point for the Semantic Kernel. It provides the ability to run
+    """The main Kernel class of Semantic Kernel.
+
+    This is the main entry point for the Semantic Kernel. It provides the ability to run
     semantic/native functions, and manage plugins, memory, and AI services.
 
     Attributes:
         plugins (dict[str, KernelPlugin] | None): The plugins to be used by the kernel
         services (dict[str, AIServiceClientBase]): The services to be used by the kernel
         ai_service_selector (AIServiceSelector): The AI service selector to be used by the kernel
         retry_mechanism (RetryMechanismBase): The retry mechanism to be used by the kernel
@@ -48,23 +49,23 @@
         plugins: KernelPlugin | dict[str, KernelPlugin] | list[KernelPlugin] | None = None,
         services: (
             AI_SERVICE_CLIENT_TYPE | list[AI_SERVICE_CLIENT_TYPE] | dict[str, AI_SERVICE_CLIENT_TYPE] | None
         ) = None,
         ai_service_selector: AIServiceSelector | None = None,
         **kwargs: Any,
     ) -> None:
-        """
-        Initialize a new instance of the Kernel class.
+        """Initialize a new instance of the Kernel class.
 
         Args:
             plugins (KernelPlugin | dict[str, KernelPlugin] | list[KernelPlugin] | None):
                 The plugins to be used by the kernel, will be rewritten to a dict with plugin name as key
-            services (AIServiceClientBase | list[AIServiceClientBase] | dict[str, AIServiceClientBase] | None:
+            services (AIServiceClientBase | list[AIServiceClientBase] | dict[str, AIServiceClientBase] | None):
                 The services to be used by the kernel, will be rewritten to a dict with service_id as key
-            ai_service_selector (AIServiceSelector | None): The AI service selector to be used by the kernel,
+            ai_service_selector (AIServiceSelector | None):
+                The AI service selector to be used by the kernel,
                 default is based on order of execution settings.
             **kwargs (Any): Additional fields to be passed to the Kernel model,
                 these are limited to retry_mechanism and function_invoking_handlers
                 and function_invoked_handlers, the best way to add function_invoking_handlers
                 and function_invoked_handlers is to use the add_function_invoking_handler
                 and add_function_invoked_handler methods.
         """
@@ -88,19 +89,19 @@
         **kwargs: Any,
     ) -> AsyncGenerator[list["StreamingContentMixin"] | FunctionResult | list[FunctionResult], Any]:
         """Execute one or more stream functions.
 
         This will execute the functions in the order they are provided, if a list of functions is provided.
         When multiple functions are provided only the last one is streamed, the rest is executed as a pipeline.
 
-        Arguments:
-            functions (KernelFunction): The function or functions to execute,
-            this value has precedence when supplying both this and using function_name and plugin_name,
-            if this is none, function_name and plugin_name are used and cannot be None.
-            arguments (KernelArguments): The arguments to pass to the function(s), optional
+        Args:
+            function (KernelFunction): The function to execute,
+                this value has precedence when supplying both this and using function_name and plugin_name,
+                if this is none, function_name and plugin_name are used and cannot be None.
+            arguments (KernelArguments | None): The arguments to pass to the function(s), optional
             function_name (str | None): The name of the function to execute
             plugin_name (str | None): The name of the plugin to execute
             metadata (dict[str, Any]): The metadata to pass to the function(s)
             return_function_results (bool): If True, the function results are yielded as a list[FunctionResult]
             in addition to the streaming content, otherwise only the streaming content is yielded.
             kwargs (dict[str, Any]): arguments that can be used instead of supplying KernelArguments
 
@@ -147,15 +148,15 @@
         metadata: dict[str, Any] = {},
         **kwargs: Any,
     ) -> FunctionResult | None:
         """Execute one or more functions.
 
         When multiple functions are passed the FunctionResult of each is put into a list.
 
-        Arguments:
+        Args:
             function (KernelFunction): The function or functions to execute,
             this value has precedence when supplying both this and using function_name and plugin_name,
             if this is none, function_name and plugin_name are used and cannot be None.
             arguments (KernelArguments): The arguments to pass to the function(s), optional
             function_name (str | None): The name of the function to execute
             plugin_name (str | None): The name of the plugin to execute
             metadata (dict[str, Any]): The metadata to pass to the function(s)
@@ -197,16 +198,15 @@
         template_format: Literal[
             "semantic-kernel",
             "handlebars",
             "jinja2",
         ] = KERNEL_TEMPLATE_FORMAT_NAME,
         **kwargs: Any,
     ) -> FunctionResult | None:
-        """
-        Invoke a function from the provided prompt
+        """Invoke a function from the provided prompt.
 
         Args:
             function_name (str): The name of the function
             plugin_name (str): The name of the plugin
             prompt (str): The prompt to use
             arguments (KernelArguments | None): The arguments to pass to the function(s), optional
             template_format (str | None): The format of the prompt template
@@ -238,23 +238,23 @@
             "semantic-kernel",
             "handlebars",
             "jinja2",
         ] = KERNEL_TEMPLATE_FORMAT_NAME,
         return_function_results: bool | None = False,
         **kwargs: Any,
     ) -> AsyncIterable[list["StreamingContentMixin"] | FunctionResult | list[FunctionResult]]:
-        """
-        Invoke a function from the provided prompt and stream the results
+        """Invoke a function from the provided prompt and stream the results.
 
         Args:
             function_name (str): The name of the function
             plugin_name (str): The name of the plugin
             prompt (str): The prompt to use
             arguments (KernelArguments | None): The arguments to pass to the function(s), optional
             template_format (str | None): The format of the prompt template
+            return_function_results (bool): If True, the function results are yielded as a list[FunctionResult]
             kwargs (dict[str, Any]): arguments that can be used instead of supplying KernelArguments
 
         Returns:
             AsyncIterable[StreamingContentMixin]: The content of the stream of the last function provided.
         """
         if not arguments:
             arguments = KernelArguments(**kwargs)
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-1.0.3/semantic_kernel/memory/memory_query_result.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-
 from numpy import ndarray
 
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
 @experimental_class
@@ -27,25 +26,26 @@
         text: str | None,
         additional_metadata: str | None,
         embedding: ndarray | None,
         relevance: float,
     ) -> None:
         """Initialize a new instance of MemoryQueryResult.
 
-        Arguments:
-            is_reference {bool} -- Whether the record is a reference record.
-            external_source_name {Optional[str]} -- The name of the external source.
-            id {str} -- A unique for the record.
-            description {Optional[str]} -- The description of the record.
-            text {Optional[str]} -- The text of the record.
-            embedding {ndarray} -- The embedding of the record.
-            relevance {float} -- The relevance of the record to a known query.
+        Args:
+            is_reference (bool): Whether the record is a reference record.
+            external_source_name (Optional[str]): The name of the external source.
+            id (str): A unique for the record.
+            description (Optional[str]): The description of the record.
+            text (Optional[str]): The text of the record.
+            additional_metadata (Optional[str]): Custom metadata for the record.
+            embedding (ndarray): The embedding of the record.
+            relevance (float): The relevance of the record to a known query.
 
         Returns:
-            None -- None.
+            None: None.
         """
         self.is_reference = is_reference
         self.external_source_name = external_source_name
         self.id = id
         self.description = description
         self.text = text
         self.additional_metadata = additional_metadata
@@ -55,20 +55,20 @@
     @staticmethod
     def from_memory_record(
         record: MemoryRecord,
         relevance: float,
     ) -> "MemoryQueryResult":
         """Create a new instance of MemoryQueryResult from a MemoryRecord.
 
-        Arguments:
-            record {MemoryRecord} -- The MemoryRecord to create the MemoryQueryResult from.
-            relevance {float} -- The relevance of the record to a known query.
+        Args:
+            record (MemoryRecord): The MemoryRecord to create the MemoryQueryResult from.
+            relevance (float): The relevance of the record to a known query.
 
         Returns:
-            MemoryQueryResult -- The created MemoryQueryResult.
+            MemoryQueryResult: The created MemoryQueryResult.
         """
         return MemoryQueryResult(
             is_reference=record._is_reference,
             external_source_name=record._external_source_name,
             id=record._id,
             description=record._description,
             text=record._text,
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/memory/memory_record.py` & `semantic_kernel-1.0.3/semantic_kernel/memory/memory_record.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,25 +29,24 @@
         additional_metadata: str | None,
         embedding: ndarray | None,
         key: str | None = None,
         timestamp: datetime | None = None,
     ) -> None:
         """Initialize a new instance of MemoryRecord.
 
-        Arguments:
-            is_reference {bool} -- Whether the record is a reference record.
-            external_source_name {Optional[str]} -- The name of the external source.
-            id {str} -- A unique for the record.
-            description {Optional[str]} -- The description of the record.
-            text {Optional[str]} -- The text of the record.
-            additional_metadata {Optional[str]} -- Custom metadata for the record.
-            embedding {ndarray} -- The embedding of the record.
-
-        Returns:
-            None -- None.
+        Args:
+            is_reference (bool): Whether the record is a reference record.
+            external_source_name (Optional[str]): The name of the external source.
+            id (str): A unique for the record.
+            description (Optional[str]): The description of the record.
+            text (Optional[str]): The text of the record.
+            additional_metadata (Optional[str]): Custom metadata for the record.
+            embedding (ndarray): The embedding of the record.
+            key (Optional[str]): The key of the record.
+            timestamp (Optional[datetime]): The timestamp of the record.
         """
         self._key = key
         self._timestamp = timestamp
         self._is_reference = is_reference
         self._external_source_name = external_source_name
         self._id = id
         self._description = description
@@ -61,23 +60,23 @@
         source_name: str,
         description: str | None,
         additional_metadata: str | None,
         embedding: ndarray,
     ) -> "MemoryRecord":
         """Create a reference record.
 
-        Arguments:
-            external_id {str} -- The external id of the record.
-            source_name {str} -- The name of the external source.
-            description {Optional[str]} -- The description of the record.
-            additional_metadata {Optional[str]} -- Custom metadata for the record.
-            embedding {ndarray} -- The embedding of the record.
+        Args:
+            external_id (str): The external id of the record.
+            source_name (str): The name of the external source.
+            description (Optional[str]): The description of the record.
+            additional_metadata (Optional[str]): Custom metadata for the record.
+            embedding (ndarray): The embedding of the record.
 
         Returns:
-            MemoryRecord -- The reference record.
+            MemoryRecord: The reference record.
         """
         return MemoryRecord(
             is_reference=True,
             external_source_name=source_name,
             id=external_id,
             description=description,
             text=None,
@@ -92,52 +91,58 @@
         description: str | None,
         additional_metadata: str | None,
         embedding: ndarray,
         timestamp: datetime | None = None,
     ) -> "MemoryRecord":
         """Create a local record.
 
-        Arguments:
-            id {str} -- A unique for the record.
-            text {str} -- The text of the record.
-            description {Optional[str]} -- The description of the record.
-            additional_metadata {Optional[str]} -- Custom metadata for the record.
-            embedding {ndarray} -- The embedding of the record.
-            timestamp {Optional[datetime]} -- The timestamp of the record.
+        Args:
+            id (str): A unique for the record.
+            text (str): The text of the record.
+            description (Optional[str]): The description of the record.
+            additional_metadata (Optional[str]): Custom metadata for the record.
+            embedding (ndarray): The embedding of the record.
+            timestamp (Optional[datetime]): The timestamp of the record.
 
         Returns:
-            MemoryRecord -- The local record.
+            MemoryRecord: The local record.
         """
         return MemoryRecord(
             is_reference=False,
             external_source_name=None,
             id=id,
             description=description,
             text=text,
             additional_metadata=additional_metadata,
             timestamp=timestamp,
             embedding=embedding,
         )
 
     @property
     def id(self):
+        """Get the unique identifier for the memory record."""
         return self._id
 
     @property
     def embedding(self) -> ndarray:
+        """Get the embedding of the memory record."""
         return self._embedding
 
     @property
     def text(self):
+        """Get the text of the memory record."""
         return self._text
 
     @property
     def additional_metadata(self):
+        """Get the additional metadata of the memory record."""
         return self._additional_metadata
 
     @property
     def description(self):
+        """Get the description of the memory record."""
         return self._description
 
     @property
     def timestamp(self):
+        """Get the timestamp of the memory record."""
         return self._timestamp
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/memory/memory_store_base.py` & `semantic_kernel-1.0.3/semantic_kernel/memory/memory_store_base.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,192 +7,190 @@
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
 @experimental_class
 class MemoryStoreBase(ABC):
     async def __aenter__(self):
+        """Enter the context manager."""
         return self
 
     async def __aexit__(self, *args):
+        """Exit the context manager."""
         await self.close()
 
     async def close(self):
-        """Async close connection, invoked by MemoryStoreBase.__aexit__()"""
+        """Close the connection."""
         pass
 
     @abstractmethod
     async def create_collection(self, collection_name: str) -> None:
         """Creates a new collection in the data store.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
-
-        Returns:
-            None
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
         """
         pass
 
     @abstractmethod
     async def get_collections(
         self,
     ) -> list[str]:
         """Gets all collection names in the data store.
 
         Returns:
-            List[str] -- A group of collection names.
+            List[str]: A group of collection names.
         """
         pass
 
     @abstractmethod
     async def delete_collection(self, collection_name: str) -> None:
         """Deletes a collection from the data store.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
-
-        Returns:
-            None
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
         """
         pass
 
     @abstractmethod
     async def does_collection_exist(self, collection_name: str) -> bool:
         """Determines if a collection exists in the data store.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
 
         Returns:
-            bool -- True if given collection exists, False if not.
+            bool: True if given collection exists, False if not.
         """
-
         pass
 
     @abstractmethod
     async def upsert(self, collection_name: str, record: MemoryRecord) -> str:
-        """Upserts a memory record into the data store. Does not guarantee that the collection exists.
-            If the record already exists, it will be updated.
-            If the record does not exist, it will be created.
+        """Upserts a memory record into the data store.
+
+        Does not guarantee that the collection exists.
+        If the record already exists, it will be updated.
+        If the record does not exist, it will be created.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
-            record {MemoryRecord} -- The memory record to upsert.
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
+            record (MemoryRecord): The memory record to upsert.
 
         Returns:
-            str -- The unique identifier for the memory record.
+            str: The unique identifier for the memory record.
         """
         pass
 
     @abstractmethod
     async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
-        """Upserts a group of memory records into the data store. Does not guarantee that the collection exists.
-            If the record already exists, it will be updated.
-            If the record does not exist, it will be created.
+        """Upserts a group of memory records into the data store.
+
+        Does not guarantee that the collection exists.
+        If the record already exists, it will be updated.
+        If the record does not exist, it will be created.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
-            records {MemoryRecord} -- The memory records to upsert.
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
+            records (MemoryRecord): The memory records to upsert.
 
         Returns:
-            List[str] -- The unique identifiers for the memory records.
+            List[str]: The unique identifiers for the memory records.
         """
         pass
 
     @abstractmethod
     async def get(self, collection_name: str, key: str, with_embedding: bool) -> MemoryRecord:
         """Gets a memory record from the data store. Does not guarantee that the collection exists.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
-            key {str} -- The unique id associated with the memory record to get.
-            with_embedding {bool} -- If true, the embedding will be returned in the memory record.
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
+            key (str): The unique id associated with the memory record to get.
+            with_embedding (bool): If true, the embedding will be returned in the memory record.
 
         Returns:
-            MemoryRecord -- The memory record if found
+            MemoryRecord: The memory record if found
         """
         pass
 
     @abstractmethod
-    async def get_batch(self, collection_name: str, keys: list[str], with_embeddings: bool) -> list[MemoryRecord]:
+    async def get_batch(
+        self,
+        collection_name: str,
+        keys: list[str],
+        with_embeddings: bool,
+    ) -> list[MemoryRecord]:
         """Gets a batch of memory records from the data store. Does not guarantee that the collection exists.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
-            keys {List[str]} -- The unique ids associated with the memory records to get.
-            with_embeddings {bool} -- If true, the embedding will be returned in the memory records.
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
+            keys (List[str]): The unique ids associated with the memory records to get.
+            with_embeddings (bool): If true, the embedding will be returned in the memory records.
 
         Returns:
-            List[MemoryRecord] -- The memory records associated with the unique keys provided.
+            List[MemoryRecord]: The memory records associated with the unique keys provided.
         """
         pass
 
     @abstractmethod
     async def remove(self, collection_name: str, key: str) -> None:
         """Removes a memory record from the data store. Does not guarantee that the collection exists.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
-            key {str} -- The unique id associated with the memory record to remove.
-
-        Returns:
-            None
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
+            key (str): The unique id associated with the memory record to remove.
         """
         pass
 
     @abstractmethod
     async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         """Removes a batch of memory records from the data store. Does not guarantee that the collection exists.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
-            keys {List[str]} -- The unique ids associated with the memory records to remove.
-
-        Returns:
-            None
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
+            keys (List[str]): The unique ids associated with the memory records to remove.
         """
         pass
 
     @abstractmethod
     async def get_nearest_matches(
         self,
         collection_name: str,
         embedding: ndarray,
         limit: int,
         min_relevance_score: float,
         with_embeddings: bool,
     ) -> list[tuple[MemoryRecord, float]]:
         """Gets the nearest matches to an embedding of type float. Does not guarantee that the collection exists.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
-            embedding {ndarray} -- The embedding to compare the collection's embeddings with.
-            limit {int} -- The maximum number of similarity results to return.
-            min_relevance_score {float} -- The minimum relevance threshold for returned results.
-            with_embeddings {bool} -- If true, the embeddings will be returned in the memory records.
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
+            embedding (ndarray): The embedding to compare the collection's embeddings with.
+            limit (int): The maximum number of similarity results to return.
+            min_relevance_score (float): The minimum relevance threshold for returned results.
+            with_embeddings (bool): If true, the embeddings will be returned in the memory records.
 
         Returns:
-            List[Tuple[MemoryRecord, float]] -- A list of tuples where item1 is a MemoryRecord and item2
+            List[Tuple[MemoryRecord, float]]: A list of tuples where item1 is a MemoryRecord and item2
                 is its similarity score as a float.
         """
         pass
 
     @abstractmethod
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float,
         with_embedding: bool,
     ) -> tuple[MemoryRecord, float]:
         """Gets the nearest match to an embedding of type float. Does not guarantee that the collection exists.
 
-        Arguments:
-            collection_name {str} -- The name associated with a collection of embeddings.
-            embedding {ndarray} -- The embedding to compare the collection's embeddings with.
-            min_relevance_score {float} -- The minimum relevance threshold for returned result.
-            with_embedding {bool} -- If true, the embeddings will be returned in the memory record.
+        Args:
+            collection_name (str): The name associated with a collection of embeddings.
+            embedding (ndarray): The embedding to compare the collection's embeddings with.
+            min_relevance_score (float): The minimum relevance threshold for returned result.
+            with_embedding (bool): If true, the embeddings will be returned in the memory record.
 
         Returns:
-            Tuple[MemoryRecord, float] -- A tuple consisting of the MemoryRecord and the similarity score as a float.
+            Tuple[MemoryRecord, float]: A tuple consisting of the MemoryRecord and the similarity score as a float.
         """
         pass
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/memory/null_memory.py` & `semantic_kernel-1.0.3/semantic_kernel/memory/null_memory.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-
 from semantic_kernel.memory.memory_query_result import MemoryQueryResult
 from semantic_kernel.memory.semantic_text_memory_base import SemanticTextMemoryBase
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
 @experimental_class
 class NullMemory(SemanticTextMemoryBase):
@@ -12,42 +11,42 @@
         self,
         collection: str,
         text: str,
         id: str,
         description: str | None = None,
         additional_metadata: str | None = None,
     ) -> None:
-        """Nullifies behavior of SemanticTextMemoryBase.save_information()"""
+        """Nullifies behavior of SemanticTextMemoryBase save_information."""
         return None
 
     async def save_reference(
         self,
         collection: str,
         text: str,
         external_id: str,
         external_source_name: str,
         description: str | None = None,
         additional_metadata: str | None = None,
     ) -> None:
-        """Nullifies behavior of SemanticTextMemoryBase.save_reference()"""
+        """Nullifies behavior of SemanticTextMemoryBase save_reference."""
         return None
 
     async def get(self, collection: str, query: str) -> MemoryQueryResult | None:
-        """Nullifies behavior of SemanticTextMemoryBase.get()"""
+        """Nullifies behavior of SemanticTextMemoryBase get."""
         return None
 
     async def search(
         self,
         collection: str,
         query: str,
         limit: int = 1,
         min_relevance_score: float = 0.7,
     ) -> list[MemoryQueryResult]:
-        """Nullifies behavior of SemanticTextMemoryBase.search()"""
+        """Nullifies behavior of SemanticTextMemoryBase search."""
         return []
 
     async def get_collections(self) -> list[str]:
-        """Nullifies behavior of SemanticTextMemoryBase.get_collections()"""
+        """Nullifies behavior of SemanticTextMemoryBase get_collections."""
         return []
 
 
 NullMemory.instance = NullMemory()  # type: ignore
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-1.0.3/semantic_kernel/memory/semantic_text_memory.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,21 +17,18 @@
     _storage: MemoryStoreBase = PrivateAttr()
     # TODO: replace with kernel and service_selector pattern
     _embeddings_generator: EmbeddingGeneratorBase = PrivateAttr()
 
     def __init__(self, storage: MemoryStoreBase, embeddings_generator: EmbeddingGeneratorBase) -> None:
         """Initialize a new instance of SemanticTextMemory.
 
-        Arguments:
-            storage {MemoryStoreBase} -- The MemoryStoreBase to use for storage.
-            embeddings_generator {EmbeddingGeneratorBase} -- The EmbeddingGeneratorBase
+        Args:
+            storage (MemoryStoreBase): The MemoryStoreBase to use for storage.
+            embeddings_generator (EmbeddingGeneratorBase): The EmbeddingGeneratorBase
                 to use for generating embeddings.
-
-        Returns:
-            None -- None.
         """
         super().__init__()
         self._storage = storage
         self._embeddings_generator = embeddings_generator
 
     async def save_information(
         self,
@@ -40,22 +37,21 @@
         id: str,
         description: str | None = None,
         additional_metadata: str | None = None,
         embeddings_kwargs: dict[str, Any] | None = {},
     ) -> None:
         """Save information to the memory (calls the memory store's upsert method).
 
-        Arguments:
-            collection {str} -- The collection to save the information to.
-            text {str} -- The text to save.
-            id {str} -- The id of the information.
-            description {Optional[str]} -- The description of the information.
-
-        Returns:
-            None -- None.
+        Args:
+            collection (str): The collection to save the information to.
+            text (str): The text to save.
+            id (str): The id of the information.
+            description (Optional[str]): The description of the information.
+            additional_metadata (Optional[str]): Additional metadata of the information.
+            embeddings_kwargs (Optional[Dict[str, Any]]): The embeddings kwargs of the information.
         """
         # TODO: not the best place to create collection, but will address this behavior together with .NET SK
         if not await self._storage.does_collection_exist(collection_name=collection):
             await self._storage.create_collection(collection_name=collection)
 
         embedding = (await self._embeddings_generator.generate_embeddings([text], **embeddings_kwargs))[0]
         data = MemoryRecord.local_record(
@@ -76,23 +72,22 @@
         external_source_name: str,
         description: str | None = None,
         additional_metadata: str | None = None,
         embeddings_kwargs: dict[str, Any] | None = {},
     ) -> None:
         """Save a reference to the memory (calls the memory store's upsert method).
 
-        Arguments:
-            collection {str} -- The collection to save the reference to.
-            text {str} -- The text to save.
-            external_id {str} -- The external id of the reference.
-            external_source_name {str} -- The external source name of the reference.
-            description {Optional[str]} -- The description of the reference.
-
-        Returns:
-            None -- None.
+        Args:
+            collection (str): The collection to save the reference to.
+            text (str): The text to save.
+            external_id (str): The external id of the reference.
+            external_source_name (str): The external source name of the reference.
+            description (Optional[str]): The description of the reference.
+            additional_metadata (Optional[str]): Additional metadata of the reference.
+            embeddings_kwargs (Optional[Dict[str, Any]]): The embeddings kwargs of the reference.
         """
         # TODO: not the best place to create collection, but will address this behavior together with .NET SK
         if not await self._storage.does_collection_exist(collection_name=collection):
             await self._storage.create_collection(collection_name=collection)
 
         embedding = (await self._embeddings_generator.generate_embeddings([text], **embeddings_kwargs))[0]
         data = MemoryRecord.reference_record(
@@ -108,20 +103,20 @@
     async def get(
         self,
         collection: str,
         key: str,
     ) -> MemoryQueryResult | None:
         """Get information from the memory (calls the memory store's get method).
 
-        Arguments:
-            collection {str} -- The collection to get the information from.
-            key {str} -- The key of the information.
+        Args:
+            collection (str): The collection to get the information from.
+            key (str): The key of the information.
 
         Returns:
-            Optional[MemoryQueryResult] -- The MemoryQueryResult if found, None otherwise.
+            Optional[MemoryQueryResult]: The MemoryQueryResult if found, None otherwise.
         """
         record = await self._storage.get(collection_name=collection, key=key)
         return MemoryQueryResult.from_memory_record(record, 1.0) if record else None
 
     async def search(
         self,
         collection: str,
@@ -129,23 +124,24 @@
         limit: int = 1,
         min_relevance_score: float = 0.0,
         with_embeddings: bool = False,
         embeddings_kwargs: dict[str, Any] | None = {},
     ) -> list[MemoryQueryResult]:
         """Search the memory (calls the memory store's get_nearest_matches method).
 
-        Arguments:
-            collection {str} -- The collection to search in.
-            query {str} -- The query to search for.
-            limit {int} -- The maximum number of results to return. (default: {1})
-            min_relevance_score {float} -- The minimum relevance score to return. (default: {0.0})
-            with_embeddings {bool} -- Whether to return the embeddings of the results. (default: {False})
+        Args:
+            collection (str): The collection to search in.
+            query (str): The query to search for.
+            limit (int): The maximum number of results to return. (default: {1})
+            min_relevance_score (float): The minimum relevance score to return. (default: {0.0})
+            with_embeddings (bool): Whether to return the embeddings of the results. (default: {False})
+            embeddings_kwargs (Optional[Dict[str, Any]]): The embeddings kwargs of the information.
 
         Returns:
-            List[MemoryQueryResult] -- The list of MemoryQueryResult found.
+            List[MemoryQueryResult]: The list of MemoryQueryResult found.
         """
         query_embedding = (await self._embeddings_generator.generate_embeddings([query], **embeddings_kwargs))[0]
         results = await self._storage.get_nearest_matches(
             collection_name=collection,
             embedding=query_embedding,
             limit=limit,
             min_relevance_score=min_relevance_score,
@@ -154,10 +150,10 @@
 
         return [MemoryQueryResult.from_memory_record(r[0], r[1]) for r in results]
 
     async def get_collections(self) -> list[str]:
         """Get the list of collections in the memory (calls the memory store's get_collections method).
 
         Returns:
-            List[str] -- The list of all the memory collection names.
+            List[str]: The list of all the memory collection names.
         """
         return await self._storage.get_collections()
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-1.0.3/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from abc import abstractmethod
-from typing import Any, TypeVar
+from typing import TYPE_CHECKING, Any, TypeVar
 
 from semantic_kernel.kernel_pydantic import KernelBaseModel
-from semantic_kernel.memory.memory_query_result import MemoryQueryResult
 from semantic_kernel.utils.experimental_decorator import experimental_class
 
+if TYPE_CHECKING:
+    from semantic_kernel.memory.memory_query_result import MemoryQueryResult
+
 SemanticTextMemoryT = TypeVar("SemanticTextMemoryT", bound="SemanticTextMemoryBase")
 
 
 @experimental_class
 class SemanticTextMemoryBase(KernelBaseModel):
     @abstractmethod
     async def save_information(
         self,
         collection: str,
         text: str,
         id: str,
         description: str | None = None,
         additional_metadata: str | None = None,
         embeddings_kwargs: dict[str, Any] | None = None,
-        # TODO: ctoken?
     ) -> None:
         """Save information to the memory (calls the memory store's upsert method).
 
-        Arguments:
-            collection {str} -- The collection to save the information to.
-            text {str} -- The text to save.
-            id {str} -- The id of the information.
-            description {Optional[str]} -- The description of the information.
+        Args:
+            collection (str): The collection to save the information to.
+            text (str): The text to save.
+            id (str): The id of the information.
+            description (Optional[str]): The description of the information.
+            additional_metadata (Optional[str]): Additional metadata of the information.
+            embeddings_kwargs (Optional[Dict[str, Any]]): The embeddings kwargs of the information.
 
-        Returns:
-            None -- None.
         """
         pass
 
     @abstractmethod
     async def save_reference(
         self,
         collection: str,
@@ -44,68 +45,66 @@
         external_id: str,
         external_source_name: str,
         description: str | None = None,
         additional_metadata: str | None = None,
     ) -> None:
         """Save a reference to the memory (calls the memory store's upsert method).
 
-        Arguments:
-            collection {str} -- The collection to save the reference to.
-            text {str} -- The text to save.
-            external_id {str} -- The external id of the reference.
-            external_source_name {str} -- The external source name of the reference.
-            description {Optional[str]} -- The description of the reference.
+        Args:
+            collection (str): The collection to save the reference to.
+            text (str): The text to save.
+            external_id (str): The external id of the reference.
+            external_source_name (str): The external source name of the reference.
+            description (Optional[str]): The description of the reference.
+            additional_metadata (Optional[str]): Additional metadata of the reference.
 
-        Returns:
-            None -- None.
         """
         pass
 
     @abstractmethod
     async def get(
         self,
         collection: str,
         key: str,
         # TODO: with_embedding: bool,
-    ) -> MemoryQueryResult | None:
+    ) -> "MemoryQueryResult | None":
         """Get information from the memory (calls the memory store's get method).
 
-        Arguments:
-            collection {str} -- The collection to get the information from.
-            key {str} -- The key of the information.
+        Args:
+            collection (str): The collection to get the information from.
+            key (str): The key of the information.
 
         Returns:
-            Optional[MemoryQueryResult] -- The MemoryQueryResult if found, None otherwise.
+            Optional[MemoryQueryResult]: The MemoryQueryResult if found, None otherwise.
         """
         pass
 
     @abstractmethod
     async def search(
         self,
         collection: str,
         query: str,
         limit: int = 1,
         min_relevance_score: float = 0.7,
-        # TODO: ctoken?
-    ) -> list[MemoryQueryResult]:
+    ) -> list["MemoryQueryResult"]:
         """Search the memory (calls the memory store's get_nearest_matches method).
 
-        Arguments:
-            collection {str} -- The collection to search in.
-            query {str} -- The query to search for.
-            limit {int} -- The maximum number of results to return. (default: {1})
-            min_relevance_score {float} -- The minimum relevance score to return. (default: {0.0})
-            with_embeddings {bool} -- Whether to return the embeddings of the results. (default: {False})
+        Args:
+            collection (str): The collection to search in.
+            query (str): The query to search for.
+            limit (int): The maximum number of results to return. (default: {1})
+            min_relevance_score (float): The minimum relevance score to return. (default: {0.0})
+            with_embeddings (bool): Whether to return the embeddings of the results. (default: {False})
 
         Returns:
-            List[MemoryQueryResult] -- The list of MemoryQueryResult found.
+            List[MemoryQueryResult]: The list of MemoryQueryResult found.
         """
         pass
 
     @abstractmethod
     async def get_collections(self) -> list[str]:
         """Get the list of collections in the memory (calls the memory store's get_collections method).
 
         Returns:
-            List[str] -- The list of all the memory collection names.
+            List[str]: The list of all the memory collection names.
         """
         pass
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-1.0.3/semantic_kernel/memory/volatile_memory_store.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     def __init__(self) -> None:
         """Initializes a new instance of the VolatileMemoryStore class."""
         self._store = {}
 
     async def create_collection(self, collection_name: str) -> None:
         """Creates a new collection if it does not exist.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to create.
+        Args:
+            collection_name (str): The name of the collection to create.
 
         Returns:
             None
         """
         if collection_name in self._store:
             pass
         else:
@@ -37,86 +37,86 @@
 
     async def get_collections(
         self,
     ) -> list[str]:
         """Gets the list of collections.
 
         Returns:
-            List[str] -- The list of collections.
+            List[str]: The list of collections.
         """
         return list(self._store.keys())
 
     async def delete_collection(self, collection_name: str) -> None:
         """Deletes a collection.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to delete.
+        Args:
+            collection_name (str): The name of the collection to delete.
 
         Returns:
             None
         """
         if collection_name in self._store:
             del self._store[collection_name]
 
     async def does_collection_exist(self, collection_name: str) -> bool:
         """Checks if a collection exists.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to check.
+        Args:
+            collection_name (str): The name of the collection to check.
 
         Returns:
-            bool -- True if the collection exists; otherwise, False.
+            bool: True if the collection exists; otherwise, False.
         """
         return collection_name in self._store
 
     async def upsert(self, collection_name: str, record: MemoryRecord) -> str:
         """Upserts a record.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to upsert the record into.
-            record {MemoryRecord} -- The record to upsert.
+        Args:
+            collection_name (str): The name of the collection to upsert the record into.
+            record (MemoryRecord): The record to upsert.
 
         Returns:
-            str -- The unique database key of the record.
+            str: The unique database key of the record.
         """
         if collection_name not in self._store:
             raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
         record._key = record._id
         self._store[collection_name][record._key] = record
         return record._key
 
     async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
         """Upserts a batch of records.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to upsert the records into.
-            records {List[MemoryRecord]} -- The records to upsert.
+        Args:
+            collection_name (str): The name of the collection to upsert the records into.
+            records (List[MemoryRecord]): The records to upsert.
 
         Returns:
-            List[str] -- The unique database keys of the records.
+            List[str]: The unique database keys of the records.
         """
         if collection_name not in self._store:
             raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
         for record in records:
             record._key = record._id
             self._store[collection_name][record._key] = record
         return [record._key for record in records]
 
     async def get(self, collection_name: str, key: str, with_embedding: bool = False) -> MemoryRecord:
         """Gets a record.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to get the record from.
-            key {str} -- The unique database key of the record.
-            with_embedding {bool} -- Whether to include the embedding in the result. (default: {False})
+        Args:
+            collection_name (str): The name of the collection to get the record from.
+            key (str): The unique database key of the record.
+            with_embedding (bool): Whether to include the embedding in the result. (default: {False})
 
         Returns:
-            MemoryRecord -- The record.
+            MemoryRecord: The record.
         """
         if collection_name not in self._store:
             raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
         if key not in self._store[collection_name]:
             raise ServiceResourceNotFoundError(f"Key '{key}' not found in collection '{collection_name}'")
 
@@ -129,21 +129,21 @@
         return result
 
     async def get_batch(
         self, collection_name: str, keys: list[str], with_embeddings: bool = False
     ) -> list[MemoryRecord]:
         """Gets a batch of records.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to get the records from.
-            keys {List[str]} -- The unique database keys of the records.
-            with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
+        Args:
+            collection_name (str): The name of the collection to get the records from.
+            keys (List[str]): The unique database keys of the records.
+            with_embeddings (bool): Whether to include the embeddings in the results. (default: {False})
 
         Returns:
-            List[MemoryRecord] -- The records.
+            List[MemoryRecord]: The records.
         """
         if collection_name not in self._store:
             raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
         results = [self._store[collection_name][key] for key in keys if key in self._store[collection_name]]
 
         if not with_embeddings:
@@ -152,17 +152,17 @@
                 result = deepcopy(result)
                 result._embedding = None
         return results
 
     async def remove(self, collection_name: str, key: str) -> None:
         """Removes a record.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to remove the record from.
-            key {str} -- The unique database key of the record to remove.
+        Args:
+            collection_name (str): The name of the collection to remove the record from.
+            key (str): The unique database key of the record to remove.
 
         Returns:
             None
         """
         if collection_name not in self._store:
             raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
@@ -170,17 +170,17 @@
             raise ServiceResourceNotFoundError(f"Key '{key}' not found in collection '{collection_name}'")
 
         del self._store[collection_name][key]
 
     async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         """Removes a batch of records.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to remove the records from.
-            keys {List[str]} -- The unique database keys of the records to remove.
+        Args:
+            collection_name (str): The name of the collection to remove the records from.
+            keys (List[str]): The unique database keys of the records to remove.
 
         Returns:
             None
         """
         if collection_name not in self._store:
             raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
@@ -193,22 +193,22 @@
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float = 0.0,
         with_embedding: bool = False,
     ) -> tuple[MemoryRecord, float]:
         """Gets the nearest match to an embedding using cosine similarity.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to get the nearest match from.
-            embedding {ndarray} -- The embedding to find the nearest match to.
-            min_relevance_score {float} -- The minimum relevance score of the match. (default: {0.0})
-            with_embedding {bool} -- Whether to include the embedding in the result. (default: {False})
+        Args:
+            collection_name (str): The name of the collection to get the nearest match from.
+            embedding (ndarray): The embedding to find the nearest match to.
+            min_relevance_score (float): The minimum relevance score of the match. (default: {0.0})
+            with_embedding (bool): Whether to include the embedding in the result. (default: {False})
 
         Returns:
-            Tuple[MemoryRecord, float] -- The record and the relevance score.
+            Tuple[MemoryRecord, float]: The record and the relevance score.
         """
         return self.get_nearest_matches(
             collection_name=collection_name,
             embedding=embedding,
             limit=1,
             min_relevance_score=min_relevance_score,
             with_embeddings=with_embedding,
@@ -220,23 +220,23 @@
         embedding: ndarray,
         limit: int,
         min_relevance_score: float = 0.0,
         with_embeddings: bool = False,
     ) -> list[tuple[MemoryRecord, float]]:
         """Gets the nearest matches to an embedding using cosine similarity.
 
-        Arguments:
-            collection_name {str} -- The name of the collection to get the nearest matches from.
-            embedding {ndarray} -- The embedding to find the nearest matches to.
-            limit {int} -- The maximum number of matches to return.
-            min_relevance_score {float} -- The minimum relevance score of the matches. (default: {0.0})
-            with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
+        Args:
+            collection_name (str): The name of the collection to get the nearest matches from.
+            embedding (ndarray): The embedding to find the nearest matches to.
+            limit (int): The maximum number of matches to return.
+            min_relevance_score (float): The minimum relevance score of the matches. (default: {0.0})
+            with_embeddings (bool): Whether to include the embeddings in the results. (default: {False})
 
         Returns:
-            List[Tuple[MemoryRecord, float]] -- The records and their relevance scores.
+            List[Tuple[MemoryRecord, float]]: The records and their relevance scores.
         """
         if collection_name not in self._store:
             logger.warning(
                 f"Collection '{collection_name}' does not exist in collections: "
                 f"{', '.join([collection for collection in await self.get_collections()])}"
             )
             return []
@@ -278,20 +278,20 @@
                 result = deepcopy(result)
                 result[0]._embedding = None
         return top_results
 
     def compute_similarity_scores(self, embedding: ndarray, embedding_array: ndarray) -> ndarray:
         """Computes the cosine similarity scores between a query embedding and a group of embeddings.
 
-        Arguments:
-            embedding {ndarray} -- The query embedding.
-            embedding_array {ndarray} -- The group of embeddings.
+        Args:
+            embedding (ndarray): The query embedding.
+            embedding_array (ndarray): The group of embeddings.
 
         Returns:
-            ndarray -- The cosine similarity scores.
+            ndarray: The cosine similarity scores.
         """
         query_norm = linalg.norm(embedding)
         collection_norm = linalg.norm(embedding_array, axis=1)
 
         # Compute indices for which the similarity scores can be computed
         valid_indices = (query_norm != 0) & (collection_norm != 0)
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/planners/__init__.py` & `semantic_kernel-1.0.3/semantic_kernel/planners/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py` & `semantic_kernel-1.0.3/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py` & `semantic_kernel-1.0.3/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-
 import asyncio
 import logging
 import os
 from copy import copy
 from typing import Any
 
 import yaml
@@ -55,21 +54,21 @@
 class FunctionCallingStepwisePlanner(KernelBaseModel):
     service_id: str
     options: FunctionCallingStepwisePlannerOptions
     generate_plan_yaml: str
     step_prompt: str
 
     def __init__(self, service_id: str, options: FunctionCallingStepwisePlannerOptions | None = None):
-        """Initialize a new instance of the FunctionCallingStepwisePlanner
+        """Initialize a new instance of the FunctionCallingStepwisePlanner.
 
         The FunctionCallingStepwisePlanner is a planner based on top of an OpenAI Chat Completion service
         (whether it be AzureOpenAI or OpenAI), so that we can use tools.
 
         If the options are configured to use callbacks to get the initial plan and the step prompt,
-        the planner will use those provided callbacks to get that information. Otherwise it will
+        the planner will use those provided callbacks to get that information. Otherwise, it will
         read from the default yaml plan file and the step prompt file.
 
         Args:
             service_id (str): The service id
             options (Optional[FunctionCallingStepwisePlannerOptions], optional): The options for
                 the function calling stepwise planner. Defaults to None.
         """
@@ -90,16 +89,15 @@
     async def invoke(
         self,
         kernel: Kernel,
         question: str,
         arguments: KernelArguments | None = None,
         **kwargs: Any,
     ) -> FunctionCallingStepwisePlannerResult:
-        """
-        Execute the function calling stepwise planner
+        """Execute the function calling stepwise planner.
 
         Args:
             kernel: The kernel instance
             question: The input question
             arguments: (optional) The kernel arguments
             kwargs: (optional) Additional keyword arguments
 
@@ -222,15 +220,15 @@
         self,
         goal: str,
         initial_plan: str,
         kernel: Kernel,
         arguments: KernelArguments,
         service: OpenAIChatCompletion | AzureChatCompletion,
     ) -> ChatHistory:
-        """Build the chat history for the stepwise planner"""
+        """Build the chat history for the stepwise planner."""
         chat_history = ChatHistory()
         additional_arguments = KernelArguments(
             goal=goal,
             initial_plan=initial_plan,
         )
         arguments.update(additional_arguments)
         kernel_prompt_template = KernelPromptTemplate(
@@ -240,16 +238,18 @@
         )
         prompt = await kernel_prompt_template.render(kernel, arguments)
         chat_history = ChatHistory.from_rendered_prompt(prompt)
         return chat_history
 
     def _create_config_from_yaml(self, kernel: Kernel) -> "KernelFunction":
         """A temporary method to create a function from the yaml file.
+
         The yaml.safe_load will be replaced with the proper kernel
-        method later."""
+        method later.
+        """
         data = yaml.safe_load(self.generate_plan_yaml)
         prompt_template_config = PromptTemplateConfig(**data)
         if "default" in prompt_template_config.execution_settings:
             settings = prompt_template_config.execution_settings.pop("default")
             prompt_template_config.execution_settings[self.service_id] = settings
         return kernel.add_function(
             function_name="create_plan",
@@ -260,15 +260,15 @@
 
     async def _generate_plan(
         self,
         question: str,
         kernel: Kernel,
         arguments: KernelArguments,
     ) -> str:
-        """Generate the plan for the given question using the kernel"""
+        """Generate the plan for the given question using the kernel."""
         generate_plan_function = self._create_config_from_yaml(kernel)
         # TODO: revisit when function call behavior is finalized, and other function calling models are added
         functions_manual = [
             kernel_function_metadata_to_openai_tool_format(f)
             for f in kernel.get_list_of_function_metadata(
                 {"excluded_functions": [f"{self.service_id}", "sequential_planner-create_plan"]}
             )
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py` & `semantic_kernel-1.0.3/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     max_iterations: int | None = 15
     min_iteration_time_ms: int | None = 100
     execution_settings: OpenAIPromptExecutionSettings | None = None
 
     @model_validator(mode="before")
     @classmethod
     def calculate_token_limits(cls, data: Any) -> Any:
+        """Calculate the token limits based on the max_tokens and max_tokens_ratio."""
         if isinstance(data, dict):
             max_tokens = data.get("max_tokens")
             # Ensure max_tokens_ratio has a default value if not provided
             max_tokens_ratio = data.get("max_tokens_ratio", 0.1)
 
             if max_tokens is not None:
                 data["max_completion_tokens"] = int(max_tokens * max_tokens_ratio)
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py` & `semantic_kernel-1.0.3/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-
 from typing import Annotated
 
 from semantic_kernel.contents.chat_history import ChatHistory
 from semantic_kernel.functions.kernel_function_decorator import kernel_function
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 
 class FunctionCallingStepwisePlannerResult(KernelBaseModel):
-    """The result of the function calling stepwise planner"""
+    """The result of the function calling stepwise planner."""
 
     final_answer: str = ""
     chat_history: ChatHistory | None = None
     iterations: int = 0
 
 
 class UserInteraction:
-    """The Kernel Function used to interact with the user"""
+    """The Kernel Function used to interact with the user."""
 
     @kernel_function(description="The final answer to return to the user", name="SendFinalAnswer")
     def send_final_answer(self, answer: Annotated[str, "The final answer"]) -> str:
+        """Send the final answer to the user."""
         return "Thanks"
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml` & `semantic_kernel-1.0.3/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/planners/plan.py` & `semantic_kernel-1.0.3/semantic_kernel/planners/plan.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from copy import copy
 from typing import Any, ClassVar, Optional
 
 from pydantic import PrivateAttr
 
 from semantic_kernel import Kernel
 from semantic_kernel.connectors.ai import PromptExecutionSettings
-from semantic_kernel.exceptions import KernelInvokeException
+from semantic_kernel.exceptions import KernelFunctionNotFoundError, KernelInvokeException, KernelPluginNotFoundError
 from semantic_kernel.functions.function_result import FunctionResult
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.functions.kernel_function import KernelFunction
 from semantic_kernel.functions.kernel_function_metadata import KernelFunctionMetadata
 from semantic_kernel.utils.naming import generate_random_ascii_name
 
 logger: logging.Logger = logging.getLogger(__name__)
@@ -34,75 +34,88 @@
     _description: str = PrivateAttr()
     _is_prompt: bool = PrivateAttr()
     _prompt_execution_settings: PromptExecutionSettings = PrivateAttr()
     DEFAULT_RESULT_KEY: ClassVar[str] = "PLAN.RESULT"
 
     @property
     def name(self) -> str:
+        """Get the name for the plan."""
         return self._name
 
     @property
     def state(self) -> KernelArguments:
+        """Get the state for the plan."""
         return self._state
 
     @property
     def steps(self) -> list["Plan"]:
+        """Get the steps for the plan."""
         return self._steps
 
     @property
     def plugin_name(self) -> str:
+        """Get the plugin name for the plan."""
         return self._plugin_name
 
     @property
     def description(self) -> str:
+        """Get the description for the plan."""
         return self._description
 
     @property
     def function(self) -> Callable[..., Any]:
+        """Get the function for the plan."""
         return self._function
 
     @property
     def parameters(self) -> KernelArguments:
+        """Get the parameters for the plan."""
         return self._parameters
 
     @property
     def is_prompt(self) -> bool:
+        """Check if the plan is a prompt."""
         return self._is_prompt
 
     @property
     def is_native(self) -> bool:
+        """Check if the plan is native code."""
         if self._is_prompt is None:
             return None
         else:
             return not self._is_prompt
 
     @property
     def prompt_execution_settings(self) -> PromptExecutionSettings:
+        """Get the AI configuration for the plan."""
         return self._prompt_execution_settings
 
     @property
     def has_next_step(self) -> bool:
+        """Check if the plan has a next step."""
         return self._next_step_index < len(self._steps)
 
     @property
     def next_step_index(self) -> int:
+        """Get the next step index."""
         return self._next_step_index
 
     def __init__(
         self,
         name: str | None = None,
         plugin_name: str | None = None,
         description: str | None = None,
         next_step_index: int | None = None,
         state: KernelArguments | None = None,
         parameters: KernelArguments | None = None,
         outputs: list[str] | None = None,
         steps: list["Plan"] | None = None,
         function: KernelFunction | None = None,
     ) -> None:
+        """Initializes a new instance of the Plan class."""
         self._name = f"plan_{generate_random_ascii_name()}" if name is None else name
         self._plugin_name = f"p_{generate_random_ascii_name()}" if plugin_name is None else plugin_name
         self._description = "" if description is None else description
         self._next_step_index = 0 if next_step_index is None else next_step_index
         self._state = KernelArguments() if state is None else state
         self._parameters = KernelArguments() if parameters is None else parameters
         self._outputs = [] if outputs is None else outputs
@@ -113,40 +126,37 @@
         self._prompt_execution_settings = None
 
         if function is not None:
             self.set_function(function)
 
     @classmethod
     def from_goal(cls, goal: str) -> "Plan":
+        """Create a plan from a goal."""
         return cls(description=goal, plugin_name=cls.__name__)
 
     @classmethod
     def from_function(cls, function: KernelFunction) -> "Plan":
+        """Create a plan from a function."""
         plan = cls()
         plan.set_function(function)
         return plan
 
     async def invoke(
         self,
         kernel: Kernel,
         arguments: KernelArguments | None = None,
-        # TODO: cancellation_token: CancellationToken,
     ) -> FunctionResult:
-        """
-        Invoke the plan asynchronously.
+        """Invoke the plan asynchronously.
 
         Args:
-            input (str, optional): The input to the plan. Defaults to None.
+            kernel (Kernel): The kernel to use for invocation.
             arguments (KernelArguments, optional): The context to use. Defaults to None.
-            settings (PromptExecutionSettings, optional): The AI request settings to use. Defaults to None.
-            memory (SemanticTextMemoryBase, optional): The memory to use. Defaults to None.
-            **kwargs: Additional keyword arguments.
 
         Returns:
-            KernelContext: The updated context.
+            FunctionResult: The result of the function.
         """
         if not arguments:
             arguments = copy(self._state)
         if self._function is not None:
             try:
                 result = await self._function.invoke(kernel=kernel, arguments=arguments)
             except Exception as exc:
@@ -179,42 +189,49 @@
 
             return FunctionResult(function=self.metadata, value=result_string, metadata={"results": partial_results})
 
     def set_ai_configuration(
         self,
         settings: PromptExecutionSettings,
     ) -> None:
+        """Set the AI configuration for the plan."""
         self._prompt_execution_settings = settings
 
     @property
     def metadata(self) -> KernelFunctionMetadata:
+        """Get the metadata for the plan."""
         if self._function is not None:
             return self._function.metadata
         return KernelFunctionMetadata(
             name=self._name or "Plan",
             plugin_name=self._plugin_name,
             parameters=[],
             description=self._description,
             is_prompt=self._is_prompt or False,
         )
 
     def set_available_functions(self, plan: "Plan", kernel: "Kernel", arguments: "KernelArguments") -> "Plan":
+        """Set the available functions for the plan."""
         if len(plan.steps) == 0:
             try:
-                pluginFunction = kernel.plugins[plan.plugin_name][plan.name]
-                plan.set_function(pluginFunction)
-            except Exception:
+                plugin_function = kernel.get_function(plan.plugin_name, plan.name)
+                plan.set_function(plugin_function)
+            except (KernelFunctionNotFoundError, KernelPluginNotFoundError) as exc:
+                logger.error(
+                    f"Something went wrong when setting available functions in {self._plugin_name}.{self._name}:'{exc}'"
+                )
                 pass
         else:
             for step in plan.steps:
                 step = self.set_available_functions(step, kernel, arguments)
 
         return plan
 
     def add_steps(self, steps: list["Plan"] | list[KernelFunction]) -> None:
+        """Add steps to the plan."""
         for step in steps:
             if type(step) is Plan:
                 self._steps.append(step)
             else:
                 new_step = Plan(
                     name=step.name,
                     plugin_name=step.plugin_name,
@@ -225,30 +242,33 @@
                     outputs=[],
                     steps=[],
                 )
                 new_step.set_function(step)
                 self._steps.append(new_step)
 
     def set_function(self, function: KernelFunction) -> None:
+        """Set the function for the plan."""
         self._function = function
         self._name = function.name
         self._plugin_name = function.plugin_name
         self._description = function.description
         self._is_prompt = function.is_prompt
         if hasattr(function, "prompt_execution_settings"):
             self._prompt_execution_settings = function.prompt_execution_settings
 
     async def run_next_step(
         self,
         kernel: Kernel,
         arguments: KernelArguments,
     ) -> Optional["FunctionResult"]:
+        """Run the next step in the plan."""
         return await self.invoke_next_step(kernel, arguments)
 
     async def invoke_next_step(self, kernel: Kernel, arguments: KernelArguments) -> Optional["FunctionResult"]:
+        """Invoke the next step in the plan."""
         if not self.has_next_step:
             return None
         step = self._steps[self._next_step_index]
 
         # merge the state with the current context variables for step execution
         arguments = self.get_next_step_arguments(arguments, step)
 
@@ -271,19 +291,21 @@
             self._state[Plan.DEFAULT_RESULT_KEY] = current_plan_result.strip() + str(result)
 
         # Increment the step
         self._next_step_index += 1
         return result
 
     def add_variables_to_state(self, state: KernelArguments, variables: KernelArguments) -> None:
+        """Add variables to the state."""
         for key in variables.keys():
             if key not in state.keys():
                 state[key] = variables[key]
 
     def update_arguments_with_outputs(self, arguments: KernelArguments) -> KernelArguments:
+        """Update the arguments with the outputs from the current step."""
         if Plan.DEFAULT_RESULT_KEY in self._state:
             result_string = self._state[Plan.DEFAULT_RESULT_KEY]
         else:
             result_string = str(self._state)
 
         arguments["input"] = result_string
 
@@ -291,14 +313,15 @@
             if item in self._state:
                 arguments[item] = self._state[item]
             else:
                 arguments[item] = result_string
         return arguments
 
     def get_next_step_arguments(self, arguments: KernelArguments, step: "Plan") -> KernelArguments:
+        """Get the arguments for the next step."""
         # Priority for Input
         # - Parameters (expand from variables if needed)
         # - KernelArguments
         # - Plan.State
         # - Empty if sending to another plan
         # - Plan.Description
         input_ = None
@@ -352,14 +375,15 @@
                 step_arguments[item] = arguments[item]
 
         logger.debug(f"Final step arguments: {step_arguments}")
 
         return step_arguments
 
     def expand_from_arguments(self, arguments: KernelArguments, input_from_step: Any) -> str:
+        """Expand variables in the input from the step using the arguments."""
         result = input_from_step
         variables_regex = r"\$(?P<var>\w+)"
         matches = [m for m in re.finditer(variables_regex, str(input_from_step))]
         ordered_matches = sorted(matches, key=lambda m: len(m.group("var")), reverse=True)
 
         for match in ordered_matches:
             var_name = match.group("var")
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/planners/planner_extensions.py` & `semantic_kernel-1.0.3/semantic_kernel/planners/planner_extensions.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,38 +13,41 @@
 # The other sequential planner extensions will be left in right now for as long as we support that planner
 # and will be removed once we deprecate it.
 
 
 class PlannerFunctionExtension:
     @staticmethod
     def to_manual_string(function: KernelFunctionMetadata):
+        """Convert the function to a string that can be used in the manual."""
         inputs = [
             f"  - {parameter.name}: {parameter.description}"
             + (f" (default value: {parameter.default_value})" if parameter.default_value else "")
             for parameter in function.parameters
         ]
         inputs = "\n".join(inputs)
         return f"{function.fully_qualified_name}:\n  description: {function.description}\n  inputs:\n " f" {inputs}"
 
     @staticmethod
     def to_embedding_string(function: KernelFunctionMetadata):
+        """Convert the function to a string that can be used as an embedding."""
         inputs = "\n".join([f"    - {parameter.name}: {parameter.description}" for parameter in function.parameters])
         return f"{function.name}:\n  description: {function.description}\n " f" inputs:\n{inputs}"
 
 
 class PlannerKernelExtension:
     PLANNER_MEMORY_COLLECTION_NAME = " Planning.KernelFunctionManual"
     PLAN_KERNEL_FUNCTIONS_ARE_REMEMBERED = "Planning.KernelFunctionsAreRemembered"
 
     @staticmethod
     async def get_functions_manual(
         kernel: "Kernel",
         arguments: KernelArguments,
         options: PlannerOptions = None,
     ) -> str:
+        """Get the string of the function."""
         options = options or PlannerOptions()
 
         if options.get_available_functions is None:
             functions = await PlannerKernelExtension.get_available_functions(kernel, arguments, options)
         else:
             functions = await options.get_available_functions(options)
 
@@ -52,14 +55,15 @@
 
     @staticmethod
     async def get_available_functions(
         kernel: Kernel,
         arguments: KernelArguments,
         options: PlannerOptions,
     ):
+        """Get the available functions for the kernel."""
         excluded_plugins = options.excluded_plugins or []
         excluded_functions = options.excluded_functions or []
 
         available_functions = [
             func
             for func in kernel.get_list_of_function_metadata()
             if (func.plugin_name not in excluded_plugins and func.name not in excluded_functions)
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/planners/planner_options.py` & `semantic_kernel-1.0.3/semantic_kernel/planners/planner_options.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from collections.abc import Callable
 
 from semantic_kernel.functions.kernel_function_metadata import KernelFunctionMetadata
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 
 class PlannerOptions(KernelBaseModel):
-    """The default planner options that planners inherit from"""
+    """The default planner options that planners inherit from."""
 
     excluded_plugins: set[str] = set()
     excluded_functions: set[str] = set()
     get_available_functions: Callable[["PlannerOptions", str | None], list[KernelFunctionMetadata]] | None = None
     # TODO semantic_memory_config
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json` & `semantic_kernel-1.0.3/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt` & `semantic_kernel-1.0.3/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/sequential_planner.py` & `semantic_kernel-1.0.3/semantic_kernel/planners/sequential_planner/sequential_planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 CUR_DIR = os.path.dirname(os.path.realpath(__file__))
 PROMPT_CONFIG_FILE_PATH = os.path.join(CUR_DIR, "Plugins/SequentialPlanning/config.json")
 PROMPT_TEMPLATE_FILE_PATH = os.path.join(CUR_DIR, "Plugins/SequentialPlanning/skprompt.txt")
 
 
 def read_file(file_path: str) -> str:
+    """Reads the content of a file."""
     with open(file_path) as file:
         return file.read()
 
 
 class SequentialPlanner:
     RESTRICTED_PLUGIN_NAME = "SequentialPlanner_Excluded"
 
@@ -41,24 +42,22 @@
     def __init__(
         self,
         kernel: Kernel,
         service_id: str,
         config: SequentialPlannerConfig = None,
         prompt: str = None,
     ) -> None:
-        """
-        Initializes a new instance of the SequentialPlanner class.
+        """Initializes a new instance of the SequentialPlanner class.
 
         Args:
             kernel (Kernel): The kernel instance to use for planning
             service_id (str): The service id to use to get the AI service
             config (SequentialPlannerConfig, optional): The configuration to use for planning. Defaults to None.
             prompt (str, optional): The prompt to use for planning. Defaults to None.
         """
-        assert isinstance(kernel, Kernel)
         self.config = config or SequentialPlannerConfig()
 
         self.config.excluded_plugins.append(self.RESTRICTED_PLUGIN_NAME)
 
         self._kernel = kernel
         self._arguments = KernelArguments()
         self._function_flow_function = self._init_flow_function(prompt, service_id)
@@ -86,14 +85,15 @@
         return self._kernel.add_function(
             plugin_name=self.RESTRICTED_PLUGIN_NAME,
             function_name=self.RESTRICTED_PLUGIN_NAME,
             prompt_template_config=prompt_config,
         )
 
     async def create_plan(self, goal: str) -> Plan:
+        """Create a plan for the specified goal."""
         if len(goal) == 0:
             raise PlannerInvalidGoalError("The goal specified is empty")
 
         relevant_function_manual = await SequentialPlannerKernelExtension.get_functions_manual(
             self._kernel, self._arguments, goal, self.config
         )
         self._arguments["available_functions"] = relevant_function_manual
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/sequential_planner_config.py` & `semantic_kernel-1.0.3/semantic_kernel/planners/sequential_planner/sequential_planner_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
         excluded_functions: list[str] = None,
         included_functions: list[str] = None,
         max_tokens: int = 1024,
         allow_missing_functions: bool = False,
         get_available_functions: Callable = None,
         get_plugin_function: Callable = None,
     ):
+        """Initializes a new instance of the SequentialPlannerConfig class."""
         self.relevancy_threshold: float = relevancy_threshold
         self.max_relevant_functions: int = max_relevant_functions
         self.excluded_plugins: list[str] = excluded_plugins or []
         self.excluded_functions: list[str] = excluded_functions or []
         self.included_functions: list[str] = included_functions or []
         self.max_tokens: int = max_tokens
         self.allow_missing_functions: bool = allow_missing_functions
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py` & `semantic_kernel-1.0.3/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,24 +10,26 @@
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class SequentialPlannerFunctionExtension:
     @staticmethod
     def to_manual_string(function: KernelFunctionMetadata):
+        """Convert the function to a manual string."""
         inputs = [
             f"  - {parameter.name}: {parameter.description}"
             + (f" (default value: {parameter.default_value})" if parameter.default_value else "")
             for parameter in function.parameters
         ]
         inputs = "\n".join(inputs)
         return f"{function.fully_qualified_name}:\n  description: {function.description}\n  inputs:\n " f" {inputs}"
 
     @staticmethod
     def to_embedding_string(function: KernelFunctionMetadata):
+        """Convert the function to an embedding string."""
         inputs = "\n".join([f"    - {parameter.name}: {parameter.description}" for parameter in function.parameters])
         return f"{function.name}:\n  description: {function.description}\n " f" inputs:\n{inputs}"
 
 
 class SequentialPlannerKernelExtension:
     PLANNER_MEMORY_COLLECTION_NAME = " Planning.KernelFunctionManual"
     PLAN_KERNEL_FUNCTIONS_ARE_REMEMBERED = "Planning.KernelFunctionsAreRemembered"
@@ -35,14 +37,15 @@
     @staticmethod
     async def get_functions_manual(
         kernel: "Kernel",
         arguments: KernelArguments,
         semantic_query: str = None,
         config: SequentialPlannerConfig = None,
     ) -> str:
+        """Get the functions manual."""
         config = config or SequentialPlannerConfig()
 
         if config.get_available_functions is None:
             functions = await SequentialPlannerKernelExtension.get_available_functions(
                 kernel, arguments, config, semantic_query
             )
         else:
@@ -53,14 +56,15 @@
     @staticmethod
     async def get_available_functions(
         kernel: Kernel,
         arguments: KernelArguments,
         config: SequentialPlannerConfig,
         semantic_query: str | None = None,
     ):
+        """Get the available functions based on the semantic query."""
         excluded_plugins = config.excluded_plugins or []
         excluded_functions = config.excluded_functions or []
         included_functions = config.included_functions or []
 
         available_functions = [
             func
             for func in kernel.get_list_of_function_metadata({"excluded_plugins": excluded_plugins})
@@ -89,14 +93,15 @@
 
     @staticmethod
     async def get_relevant_functions(
         kernel: Kernel,
         available_functions: list[KernelFunctionMetadata],
         memories: list[MemoryQueryResult] | None = None,
     ) -> list[KernelFunctionMetadata]:
+        """Get relevant functions from the memories."""
         relevant_functions = []
         # TODO: cancellation
         if memories is None:
             return relevant_functions
         for memory_entry in memories:
             function = next(
                 (func for func in available_functions if func.fully_qualified_name == memory_entry.id),
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py` & `semantic_kernel-1.0.3/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     def to_plan_from_xml(
         xml_string: str,
         goal: str,
         kernel: Kernel,
         get_plugin_function: Callable[[str, str], KernelFunction | None] | None = None,
         allow_missing_functions: bool = False,
     ):
+        """Convert an xml string to a plan."""
         xml_string = "<xml>" + xml_string + "</xml>"
         try:
             xml_doc = ET.fromstring(xml_string)
         except ET.ParseError:
             # Attempt to parse <plan> out of it
             plan_regex = re.compile(r"<plan\b[^>]*>(.*?)</plan>", re.DOTALL)
             match = plan_regex.search(xml_string)
@@ -108,11 +109,12 @@
 
                 plan.add_steps([plan_step])
 
         return plan
 
     @staticmethod
     def get_plugin_function_names(plugin_function_name: str) -> tuple[str, str]:
+        """Get the plugin and function names from the plugin function name."""
         plugin_function_name_parts = plugin_function_name.split("-")
         plugin_name = plugin_function_name_parts[0] if len(plugin_function_name_parts) > 0 else ""
         function_name = plugin_function_name_parts[1] if len(plugin_function_name_parts) > 1 else plugin_function_name
         return plugin_name, function_name
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/prompt_template/__init__.py` & `semantic_kernel-1.0.3/semantic_kernel/prompt_template/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/prompt_template/const.py` & `semantic_kernel-1.0.3/semantic_kernel/prompt_template/const.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/prompt_template/handlebars_prompt_template.py` & `semantic_kernel-1.0.3/semantic_kernel/prompt_template/handlebars_prompt_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,32 +41,35 @@
     """
 
     _template_compiler: Any = PrivateAttr()
 
     @field_validator("prompt_template_config")
     @classmethod
     def validate_template_format(cls, v: "PromptTemplateConfig") -> "PromptTemplateConfig":
+        """Validate the template format."""
         if v.template_format != HANDLEBARS_TEMPLATE_FORMAT_NAME:
             raise ValueError(f"Invalid prompt template format: {v.template_format}. Expected: handlebars")
         return v
 
     def model_post_init(self, __context: Any) -> None:
+        """Post init model."""
         if not self.prompt_template_config.template:
             self._template_compiler = None
             return
         try:
             self._template_compiler = Compiler().compile(self.prompt_template_config.template)
         except PybarsError as e:
             logger.error(f"Invalid handlebars template: {self.prompt_template_config.template}")
             raise HandlebarsTemplateSyntaxError(
                 f"Invalid handlebars template: {self.prompt_template_config.template}"
             ) from e
 
     async def render(self, kernel: "Kernel", arguments: Optional["KernelArguments"] = None) -> str:
-        """
+        """Render the prompt template.
+
         Using the prompt template, replace the variables with their values
         and execute the functions replacing their reference with the
         function result.
 
         Args:
             kernel: The kernel instance
             arguments: The kernel arguments
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/prompt_template/jinja2_prompt_template.py` & `semantic_kernel-1.0.3/semantic_kernel/prompt_template/jinja2_prompt_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 if TYPE_CHECKING:
     from semantic_kernel.kernel import Kernel
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class Jinja2PromptTemplate(PromptTemplateBase):
-    """
-    Creates and renders Jinja2 prompt templates to text.
+    """Creates and renders Jinja2 prompt templates to text.
 
     Jinja2 templates support advanced features such as variable substitution, control structures,
     and inheritance, making it possible to dynamically generate text based on input arguments
     and predefined functions. This class leverages Jinja2's flexibility to render prompts that
     can include conditional logic, loops, and functions, based on the provided template configuration
     and arguments.
 
@@ -49,26 +48,29 @@
     """
 
     _env: ImmutableSandboxedEnvironment = PrivateAttr()
 
     @field_validator("prompt_template_config")
     @classmethod
     def validate_template_format(cls, v: "PromptTemplateConfig") -> "PromptTemplateConfig":
+        """Validate the template format."""
         if v.template_format != JINJA2_TEMPLATE_FORMAT_NAME:
             raise ValueError(f"Invalid prompt template format: {v.template_format}. Expected: jinja2")
         return v
 
     def model_post_init(self, _: Any) -> None:
+        """Post init model."""
         if not self.prompt_template_config.template:
             self._env = None
             return
         self._env = ImmutableSandboxedEnvironment(loader=BaseLoader())
 
     async def render(self, kernel: "Kernel", arguments: Optional["KernelArguments"] = None) -> str:
-        """
+        """Render the prompt template.
+
         Using the prompt template, replace the variables with their values
         and execute the functions replacing their reference with the
         function result.
 
         Args:
             kernel: The kernel instance
             arguments: The kernel arguments
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/prompt_template/kernel_prompt_template.py` & `semantic_kernel-1.0.3/semantic_kernel/prompt_template/kernel_prompt_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class KernelPromptTemplate(PromptTemplateBase):
     """Create a Kernel prompt template.
 
-    Arguments:
+    Args:
         prompt_template_config (PromptTemplateConfig): The prompt template configuration
             This includes the actual template to use.
         allow_dangerously_set_content (bool = False): Allow content without encoding throughout, this overrides
             the same settings in the prompt template config and input variables.
             This reverts the behavior to unencoded input.
 
     Raises:
@@ -38,19 +38,21 @@
     """
 
     _blocks: list[Block] = PrivateAttr(default_factory=list)
 
     @field_validator("prompt_template_config")
     @classmethod
     def validate_template_format(cls, v: "PromptTemplateConfig") -> "PromptTemplateConfig":
+        """Validate the template format."""
         if v.template_format != KERNEL_TEMPLATE_FORMAT_NAME:
             raise ValueError(f"Invalid prompt template format: {v.template_format}. Expected: semantic-kernel")
         return v
 
     def model_post_init(self, __context: Any) -> None:
+        """Post init model."""
         self._blocks = self.extract_blocks()
         # Add all of the existing input variables to our known set. We'll avoid adding any
         # dynamically discovered input variables with the same name.
         seen = {iv.name.lower() for iv in self.prompt_template_config.input_variables}
 
         # Enumerate every block in the template, adding any variables that are referenced.
         for block in self._blocks:
@@ -74,32 +76,28 @@
     def _add_if_missing(self, variable_name: str, seen: set | None = None):
         # Convert variable_name to lower case to handle case-insensitivity
         if variable_name and variable_name.lower() not in seen:
             seen.add(variable_name.lower())
             self.prompt_template_config.input_variables.append(InputVariable(name=variable_name))
 
     def extract_blocks(self) -> list[Block]:
-        """
-        Given a prompt template string, extract all the blocks
-        (text, variables, function calls).
-
-        Args:
-            template_text: Prompt template
+        """Given the prompt template, extract all the blocks (text, variables, function calls).
 
         Returns:
             A list of all the blocks, ie the template tokenized in
             text, variables and function calls
         """
         logger.debug(f"Extracting blocks from template: {self.prompt_template_config.template}")
         if not self.prompt_template_config.template:
             return []
         return TemplateTokenizer.tokenize(self.prompt_template_config.template)
 
     async def render(self, kernel: "Kernel", arguments: Optional["KernelArguments"] = None) -> str:
-        """
+        """Render the prompt template.
+
         Using the prompt template, replace the variables with their values
         and execute the functions replacing their reference with the
         function result.
 
         Args:
             kernel: The kernel instance
             arguments: The kernel arguments
@@ -108,16 +106,15 @@
             The prompt template ready to be used for an AI request
         """
         if arguments is None:
             arguments = KernelArguments()
         return await self.render_blocks(self._blocks, kernel, arguments)
 
     async def render_blocks(self, blocks: list[Block], kernel: "Kernel", arguments: "KernelArguments") -> str:
-        """
-        Given a list of blocks render each block and compose the final result.
+        """Given a list of blocks render each block and compose the final result.
 
         :param blocks: Template blocks generated by ExtractBlocks
         :param context: Access into the current kernel execution context
         :return: The prompt template ready to be used for an AI request
         """
         from semantic_kernel.template_engine.protocols.code_renderer import CodeRenderer
         from semantic_kernel.template_engine.protocols.text_renderer import TextRenderer
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/prompt_template/prompt_template_base.py` & `semantic_kernel-1.0.3/semantic_kernel/prompt_template/prompt_template_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 class PromptTemplateBase(KernelBaseModel, ABC):
     prompt_template_config: PromptTemplateConfig
     allow_dangerously_set_content: bool = False
 
     @abstractmethod
     async def render(self, kernel: "Kernel", arguments: "KernelArguments") -> str:
+        """Render the prompt template."""
         pass
 
     def _get_trusted_arguments(
         self,
         arguments: "KernelArguments",
     ) -> "KernelArguments":
         """Get the trusted arguments.
@@ -56,16 +57,15 @@
         """
         allow_unsafe_function_output = self.allow_dangerously_set_content
         if self.prompt_template_config.allow_dangerously_set_content:
             allow_unsafe_function_output = True
         return allow_unsafe_function_output
 
     def _should_escape(self, name: str, input_variables: list["InputVariable"]) -> bool:
-        """
-        Check if the variable should be escaped.
+        """Check if the variable should be escaped.
 
         If the PromptTemplate allows dangerously set content, then the variable will not be escaped,
         even if the input_variables does specify this.
 
         Otherwise, it checks the input_variables to see if the variable should be encoded.
 
         Otherwise, it will encode.
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/prompt_template/prompt_template_config.py` & `semantic_kernel-1.0.3/semantic_kernel/prompt_template/prompt_template_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,31 +20,32 @@
 
     Args:
         name: The name of the prompt template.
         description: The description of the prompt template.
         template: The template for the prompt.
         template_format: The format of the template, should be 'semantic-kernel', 'jinja2' or 'handlebars'.
         input_variables: The input variables for the prompt.
-        allow_dangerously_set_content (default: false): Allow content without encoding, this controls
-            if the output of functions called in the template is encoded before use.
+        allow_dangerously_set_content (bool = False): Allow content without encoding throughout, this overrides
+            the same settings in the prompt template config and input variables.
+            This reverts the behavior to unencoded input.
         execution_settings: The execution settings for the prompt.
 
     """
 
     name: str = ""
     description: str | None = ""
     template: str | None = None
     template_format: TEMPLATE_FORMAT_TYPES = KERNEL_TEMPLATE_FORMAT_NAME
     input_variables: list[InputVariable] = Field(default_factory=list)
     allow_dangerously_set_content: bool = False
     execution_settings: dict[str, PromptExecutionSettings] = Field(default_factory=dict)
 
     @model_validator(mode="after")
     def check_input_variables(self):
-        """Verify that input variable default values are string only"""
+        """Verify that input variable default values are string only."""
         for variable in self.input_variables:
             if variable.default and not isinstance(variable.default, str):
                 raise TypeError(f"Default value for input variable {variable.name} must be a string.")
         return self
 
     @field_validator("execution_settings", mode="before")
     @classmethod
@@ -107,16 +108,18 @@
     ) -> "PromptTemplateConfig":
         """Restore a PromptTemplateConfig instance from the specified parameters.
 
         Args:
             name: The name of the prompt template.
             description: The description of the prompt template.
             template: The template for the prompt.
+            template_format: The format of the template, should be 'semantic-kernel', 'jinja2' or 'handlebars'.
             input_variables: The input variables for the prompt.
             execution_settings: The execution settings for the prompt.
+            allow_dangerously_set_content: Allow content without encoding.
 
         Returns:
             A new PromptTemplateConfig instance.
         """
         return cls(
             name=name,
             description=description,
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py` & `semantic_kernel-1.0.3/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py` & `semantic_kernel-1.0.3/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/prompt_template/utils/template_function_helpers.py` & `semantic_kernel-1.0.3/semantic_kernel/prompt_template/utils/template_function_helpers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/reliability/kernel_reliability_extension.py` & `semantic_kernel-1.0.3/semantic_kernel/reliability/kernel_reliability_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-1.0.3/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 
 class PassThroughWithoutRetry(RetryMechanismBase, KernelBaseModel):
     """A retry mechanism that does not retry."""
 
     async def execute_with_retry(self, action: Callable[[], Awaitable[T]]) -> Awaitable[T]:
         """Executes the given action with retry logic.
 
-        Arguments:
-            action {Callable[[], Awaitable[T]]} -- The action to retry on exception.
+        Args:
+            action (Callable[[], Awaitable[T]]): The action to retry on exception.
 
         Returns:
-            Awaitable[T] -- An awaitable that will return the result of the action.
+            Awaitable[T]: An awaitable that will return the result of the action.
         """
         try:
             await action()
         except Exception as e:
             logger.warning(e, "Error executing action, not retrying")
             raise e
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/reliability/retry_mechanism_base.py` & `semantic_kernel-1.0.3/semantic_kernel/reliability/retry_mechanism_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,14 @@
 
 
 class RetryMechanismBase(ABC):
     @abstractmethod
     async def execute_with_retry(self, action: Callable[[], Awaitable[T]]) -> Awaitable[T]:
         """Executes the given action with retry logic.
 
-        Arguments:
-            action {Callable[[], Awaitable[T]]} -- The action to retry on exception.
+        Args:
+            action (Callable[[], Awaitable[T]]): The action to retry on exception.
 
         Returns:
-            Awaitable[T] -- An awaitable that will return the result of the action.
+            Awaitable[T]: An awaitable that will return the result of the action.
         """
         pass
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/services/ai_service_client_base.py` & `semantic_kernel-1.0.3/semantic_kernel/services/ai_service_client_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 
 class AIServiceClientBase(KernelBaseModel, ABC):
     """Base class for all AI Services.
 
-    Has a ai_model_id and service_id, any other fields have to be defined by the subclasses.
+    Has an ai_model_id and service_id, any other fields have to be defined by the subclasses.
 
     The ai_model_id can refer to a specific model, like 'gpt-35-turbo' for OpenAI,
     or can just be a string that is used to identify the model in the service.
 
     The service_id is used in Semantic Kernel to identify the service, if empty the ai_model_id is used.
     """
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/services/ai_service_selector.py` & `semantic_kernel-1.0.3/semantic_kernel/services/ai_service_selector.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,17 @@
     def select_ai_service(
         self,
         kernel: "Kernel",
         function: "KernelFunction",
         arguments: "KernelArguments",
         type_: type["AI_SERVICE_CLIENT_TYPE"] | None = None,
     ) -> tuple["AI_SERVICE_CLIENT_TYPE", "PromptExecutionSettings"]:
-        """Select a AI Service on a first come, first served basis,
-        starting with execution settings in the arguments,
+        """Select an AI Service on a first come, first served basis.
+
+        Starts with execution settings in the arguments,
         followed by the execution settings from the function.
         If the same service_id is in both, the one in the arguments will be used.
         """
         if type_ is None:
             from semantic_kernel.connectors.ai.chat_completion_client_base import ChatCompletionClientBase
             from semantic_kernel.connectors.ai.text_completion_client_base import TextCompletionClientBase
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/services/kernel_services_extension.py` & `semantic_kernel-1.0.3/semantic_kernel/services/kernel_services_extension.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,27 +103,34 @@
         if not (service := self.services.get(service_id)):
             raise KernelServiceNotFoundError(f"Service with service_id '{service_id}' does not exist")
         if type and not isinstance(service, type):
             raise ServiceInvalidTypeError(f"Service with service_id '{service_id}' is not of type {type}")
         return service
 
     def get_services_by_type(self, type: type[ALL_SERVICE_TYPES]) -> dict[str, ALL_SERVICE_TYPES]:
+        """Get all services of a specific type."""
         return {service.service_id: service for service in self.services.values() if isinstance(service, type)}  # type: ignore
 
     def get_prompt_execution_settings_from_service_id(
         self, service_id: str, type: type[ALL_SERVICE_TYPES] | None = None
     ) -> PromptExecutionSettings:
         """Get the specific request settings from the service, instantiated with the service_id and ai_model_id."""
         service = self.get_service(service_id, type=type)
         return service.instantiate_prompt_execution_settings(
             service_id=service_id,
             extension_data={"ai_model_id": service.ai_model_id},
         )
 
     def add_service(self, service: AIServiceClientBase, overwrite: bool = False) -> None:
+        """Add a single service to the Kernel.
+
+        Args:
+            service (AIServiceClientBase): The service to add.
+            overwrite (bool, optional): Whether to overwrite the service if it already exists. Defaults to False.
+        """
         if service.service_id not in self.services or overwrite:
             self.services[service.service_id] = service
         else:
             raise KernelFunctionAlreadyExistsError(f"Service with service_id '{service.service_id}' already exists")
 
     def remove_service(self, service_id: str) -> None:
         """Delete a single service from the Kernel."""
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/template_engine/README.md` & `semantic_kernel-1.0.3/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-1.0.3/semantic_kernel/template_engine/blocks/block.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 class Block(KernelBaseModel):
     type: ClassVar[BlockTypes] = BlockTypes.UNDEFINED
     content: str
 
     @field_validator("content", mode="before")
     @classmethod
     def content_strip(cls, content: str):
+        """Strip the content of the block."""
         return content.strip()
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-1.0.3/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     Raises:
         CodeBlockTokenError: If the content does not contain at least one token.
         CodeBlockTokenError: If the first token is a named argument.
         CodeBlockTokenError: If the second token is not a value or variable.
         CodeBlockTokenError: If a token is not a named argument after the second token.
         CodeBlockRenderError: If the plugin collection is not set in the kernel.
         CodeBlockRenderError: If the function is not found in the plugin collection.
-        CodeBlockRenderError: If the function does not take any arguments but it is being
+        CodeBlockRenderError: If the function does not take any arguments, but it is being
             called in the template with arguments.
     """
 
     type: ClassVar[BlockTypes] = BlockTypes.CODE
     tokens: list[Block] = Field(default_factory=list)
 
     @model_validator(mode="before")
@@ -100,15 +100,15 @@
                 )
         return tokens
 
     async def render_code(self, kernel: "Kernel", arguments: "KernelArguments") -> str:
         """Render the code block.
 
         If the first token is a function_id, it will call the function from the plugin collection.
-        Otherwise it is a value or variable and those are then rendered directly.
+        Otherwise, it is a value or variable and those are then rendered directly.
         """
         logger.debug(f"Rendering code: `{self.content}`")
         if self.tokens[0].type == BlockTypes.FUNCTION_ID:
             return await self._render_function_call(kernel, arguments)
         # validated that if the first token is not a function_id, it is a value or variable
         return self.tokens[0].render(kernel, arguments)
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-1.0.3/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 class FunctionIdBlock(Block):
     """Block to represent a function id. It can be used to call a function from a plugin.
 
     The content is parsed using a regex, that returns either a plugin and
     function name or just a function name, depending on the content.
 
-    Anything other then that and a ValueError is raised.
+    Anything other than that and a ValueError is raised.
 
     Args:
         content (str): The content of the block.
         function_name (Optional[str], optional): The function name.
         plugin_name (Optional[str], optional): The plugin name.
 
     Raises:
@@ -44,22 +44,23 @@
 
     @model_validator(mode="before")
     @classmethod
     def parse_content(cls, fields: dict[str, Any]) -> dict[str, Any]:
         """Parse the content of the function id block and extract the plugin and function name.
 
         If both are present in the fields, return the fields as is.
-        Otherwise use the regex to extract the plugin and function name.
+        Otherwise, use the regex to extract the plugin and function name.
         """
         if "plugin_name" in fields and "function_name" in fields:
             return fields
         content = fields.get("content", "").strip()
         matches = FUNCTION_ID_BLOCK_MATCHER.match(content)
         if not matches:
             raise FunctionIdBlockSyntaxError(content=content)
         if plugin := matches.groupdict().get("plugin"):
             fields["plugin_name"] = plugin
         fields["function_name"] = matches.group("function")
         return fields
 
     def render(self, *_: tuple["Kernel", Optional["KernelArguments"]]) -> str:
+        """Render the function id block."""
         return self.content
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/named_arg_block.py` & `semantic_kernel-1.0.3/semantic_kernel/template_engine/blocks/named_arg_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     @model_validator(mode="before")
     @classmethod
     def parse_content(cls, fields: Any) -> Any:
         """Parse the content of the named argument block and extract the name and value.
 
         If the name and either value or variable is present the parsing is skipped.
-        Otherwise the content is parsed using a regex to extract the name and value.
+        Otherwise, the content is parsed using a regex to extract the name and value.
         Those are then turned into Blocks.
 
         Raises:
             NamedArgBlockSyntaxError: If the content does not match the named argument syntax.
         """
         if isinstance(fields, Block) or ("name" in fields and ("value" in fields or "variable" in fields)):
             return fields
@@ -84,13 +84,14 @@
             if matches_dict.get("var_name"):
                 fields["variable"] = VarBlock(content=value, name=matches_dict["var_name"])
             elif matches_dict.get("val"):
                 fields["value"] = ValBlock(content=value, value=matches_dict["val"], quote=matches_dict["quote"])
         return fields
 
     def render(self, kernel: "Kernel", arguments: Optional["KernelArguments"] = None) -> Any:
+        """Render the named argument block."""
         if self.value:
             return self.value.render(kernel, arguments)
         if arguments is None:
             return ""
         if self.variable:
             return self.variable.render(kernel, arguments)
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-1.0.3/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,24 +17,28 @@
 
 class TextBlock(Block):
     type: ClassVar[BlockTypes] = BlockTypes.TEXT
 
     @field_validator("content", mode="before")
     @classmethod
     def content_strip(cls, content: str):
-        # overload strip method text blocks are not stripped.
+        """Strip the content of the text block.
+
+        Overload strip method, text blocks are not stripped.
+        """
         return content
 
     @classmethod
     def from_text(
         cls,
         text: str | None = None,
         start_index: int | None = None,
         stop_index: int | None = None,
     ):
+        """Create a text block from a string."""
         if text is None:
             return cls(content="")
         if start_index is not None and stop_index is not None:
             if start_index > stop_index:
                 raise ValueError(f"start_index ({start_index}) must be less than " f"stop_index ({stop_index})")
 
             if start_index < 0:
@@ -45,8 +49,9 @@
             text = text[start_index:]
         elif stop_index is not None:
             text = text[:stop_index]
 
         return cls(content=text)
 
     def render(self, *_: tuple[Optional["Kernel"], Optional["KernelArguments"]]) -> str:
+        """Render the text block."""
         return self.content
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-1.0.3/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,8 +66,9 @@
         if value := matches.groupdict().get("value"):
             fields["value"] = value
         if quote := matches.groupdict().get("quote"):
             fields["quote"] = quote
         return fields
 
     def render(self, *_: tuple["Kernel", Optional["KernelArguments"]]) -> str:
+        """Render the value block."""
         return self.value
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-1.0.3/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 VAR_BLOCK_MATCHER = compile(VAR_BLOCK_REGEX)
 
 
 class VarBlock(Block):
     """Create a variable block.
 
     A variable block is used to add a variable to a template.
-    It get's rendered from KernelArguments, if the variable is not found
+    It gets rendered from KernelArguments, if the variable is not found
     a warning is logged and an empty string is returned.
     The variable must start with $ and be followed by a valid variable name.
     A valid variable name is a string of letters, numbers and underscores.
 
     Examples:
         $var
         $test_var
@@ -63,15 +63,17 @@
             raise VarBlockSyntaxError(content=content)
         if name := matches.groupdict().get("name"):
             fields["name"] = name
         return fields
 
     def render(self, _: "Kernel", arguments: Optional["KernelArguments"] = None) -> str:
         """Render the variable block with the given arguments.
-        If the variable is not found in the arguments, return an empty string."""
+
+        If the variable is not found in the arguments, return an empty string.
+        """
         if arguments is None:
             return ""
         value = arguments.get(self.name, None)
         if value is None:
             logger.warning(f"Variable `{Symbols.VAR_PREFIX}: {self.name}` not found in the KernelArguments")
             return ""
         try:
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-1.0.3/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # [variable]       ::= "$" [valid-name]
 # [value]          ::= "'" [text] "'" | '"' [text] '"'
 # [function-call]  ::= [function-id] | [function-id] [parameter]
 # [parameter]      ::= [variable] | [value]
 class CodeTokenizer:
     @staticmethod
     def tokenize(text: str) -> list[Block]:
+        """Tokenize the code text into blocks."""
         # Remove spaces, which are ignored anyway
         text = text.strip() if text else ""
         # Render None/empty to []
         if not text:
             return []
         # 1 char only edge case, var and val blocks are invalid with one char, so it must be a function id block
         if len(text) == 1:
@@ -112,15 +113,15 @@
                     current_token_content.clear()
 
                 space_separator_found = True
                 current_token_type = None
 
                 continue
 
-            # If we're not inside a quoted value and we're not processing a space
+            # If we're not inside a quoted value, and we're not processing a space
             current_token_content.append(current_char)
 
             if current_token_type is None:
                 if not space_separator_found:
                     raise CodeBlockSyntaxError("Tokens must be separated by one space least")
 
                 if current_char in (Symbols.DBL_QUOTE, Symbols.SGL_QUOTE):
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-1.0.3/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,18 +5,15 @@
 if TYPE_CHECKING:
     from semantic_kernel import Kernel
     from semantic_kernel.functions.kernel_arguments import KernelArguments
 
 
 @runtime_checkable
 class CodeRenderer(Protocol):
-    """
-    Protocol for dynamic code blocks that need async IO to be rendered.
-    """
+    """Protocol for dynamic code blocks that need async IO to be rendered."""
 
     async def render_code(self, kernel: "Kernel", arguments: "KernelArguments") -> str:
-        """
-        Render the block using the given context.
+        """Render the block using the given context.
 
         :param context: kernel execution context
         :return: Rendered content
         """
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-1.0.3/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,15 @@
 if TYPE_CHECKING:
     from semantic_kernel import Kernel
     from semantic_kernel.functions.kernel_arguments import KernelArguments
 
 
 @runtime_checkable
 class TextRenderer(Protocol):
-    """
-    Protocol for static (text) blocks that don't need async rendering.
-    """
+    """Protocol for static (text) blocks that don't need async rendering."""
 
     def render(self, kernel: "Kernel", arguments: Optional["KernelArguments"] = None) -> str:
-        """
-        Render the block using only the given variables.
+        """Render the block using only the given variables.
 
         :param variables: Optional variables used to render the block
         :return: Rendered content
         """
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-1.0.3/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 
-from semantic_kernel.exceptions import (
-    BlockSyntaxError,
-    CodeBlockTokenError,
-    TemplateSyntaxError,
-)
+from semantic_kernel.exceptions import BlockSyntaxError, CodeBlockTokenError, TemplateSyntaxError
 from semantic_kernel.template_engine.blocks.block import Block
 from semantic_kernel.template_engine.blocks.block_types import BlockTypes
 from semantic_kernel.template_engine.blocks.code_block import CodeBlock
 from semantic_kernel.template_engine.blocks.symbols import Symbols
 from semantic_kernel.template_engine.blocks.text_block import TextBlock
 from semantic_kernel.template_engine.code_tokenizer import CodeTokenizer
 
@@ -24,14 +20,15 @@
 #                      | "{{" [value] "}}"
 #                      | "{{" [function-call] "}}"
 # [text-block]     ::= [any-char] | [any-char] [text-block]
 # [any-char]       ::= any char
 class TemplateTokenizer:
     @staticmethod
     def tokenize(text: str) -> list[Block]:
+        """Tokenize the template text into blocks."""
         code_tokenizer = CodeTokenizer()
         # An empty block consists of 4 chars: "{{}}"
         EMPTY_CODE_BLOCK_LENGTH = 4
         # A block shorter than 5 chars is either empty or
         # invalid, e.g. "{{ }}" and "{{$}}"
         MIN_CODE_BLOCK_LENGTH = EMPTY_CODE_BLOCK_LENGTH + 1
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/text/function_extension.py` & `semantic_kernel-1.0.3/semantic_kernel/text/function_extension.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 from semantic_kernel.functions.kernel_function import KernelFunction
 from semantic_kernel.kernel import Kernel
 
 
 async def aggregate_chunked_results(
     func: KernelFunction, chunked_results: list[str], kernel: Kernel, arguments: KernelArguments
 ) -> str:
-    """
-    Aggregate the results from the chunked results.
-    """
+    """Aggregate the results from the chunked results."""
     results = []
     for chunk in chunked_results:
         arguments["input"] = chunk
         result = await func.invoke(kernel, arguments)
 
         results.append(str(result))
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/text/text_chunker.py` & `semantic_kernel-1.0.3/semantic_kernel/text/text_chunker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Copyright (c) Microsoft. All rights reserved.
-"""
+"""A Text splitter.
+
 Split text in chunks, attempting to leave meaning intact.
 For plain text, split looking at new lines first, then periods, and so on.
 For markdown, split looking at punctuation first, and so on.
 """
 
 import os
 import re
@@ -35,55 +36,51 @@
     ["-"],
     ["\n", "\r"],
     None,
 ]
 
 
 def _token_counter(text: str) -> int:
-    """
-    Count the number of tokens in a string.
+    """Count the number of tokens in a string.
 
     TODO: chunking methods should be configurable to allow for different
           tokenization strategies depending on the model to be called.
           For now, we use an extremely rough estimate.
     """
     return len(text) // 4
 
 
 def split_plaintext_lines(text: str, max_token_per_line: int, token_counter: Callable = _token_counter) -> list[str]:
-    """
-    Split plain text into lines.
+    """Split plain text into lines.
+
     it will split on new lines first, and then on punctuation.
     """
     return _split_text_lines(
         text=text,
         max_token_per_line=max_token_per_line,
         trim=True,
         token_counter=token_counter,
     )
 
 
 def split_markdown_lines(text: str, max_token_per_line: int, token_counter: Callable = _token_counter) -> list[str]:
-    """
-    Split markdown into lines.
+    """Split markdown into lines.
+
     It will split on punctuation first, and then on space and new lines.
     """
     return _split_markdown_lines(
         text=text,
         max_token_per_line=max_token_per_line,
         trim=True,
         token_counter=token_counter,
     )
 
 
 def split_plaintext_paragraph(text: list[str], max_tokens: int, token_counter: Callable = _token_counter) -> list[str]:
-    """
-    Split plain text into paragraphs.
-    """
-
+    """Split plain text into paragraphs."""
     split_lines = []
     for line in text:
         split_lines.extend(
             _split_text_lines(
                 text=line,
                 max_token_per_line=max_tokens,
                 trim=True,
@@ -91,17 +88,15 @@
             )
         )
 
     return _split_text_paragraph(text=split_lines, max_tokens=max_tokens, token_counter=token_counter)
 
 
 def split_markdown_paragraph(text: list[str], max_tokens: int, token_counter: Callable = _token_counter) -> list[str]:
-    """
-    Split markdown into paragraphs.
-    """
+    """Split markdown into paragraphs."""
     split_lines = []
     for line in text:
         split_lines.extend(
             _split_markdown_lines(
                 text=line,
                 max_token_per_line=max_tokens,
                 trim=False,
@@ -109,17 +104,15 @@
             )
         )
 
     return _split_text_paragraph(text=split_lines, max_tokens=max_tokens, token_counter=token_counter)
 
 
 def _split_text_paragraph(text: list[str], max_tokens: int, token_counter: Callable = _token_counter) -> list[str]:
-    """
-    Split text into paragraphs.
-    """
+    """Split text into paragraphs."""
     if not text:
         return []
 
     paragraphs = []
     current_paragraph = []
 
     for line in text:
@@ -161,18 +154,15 @@
 
 def _split_markdown_lines(
     text: str,
     max_token_per_line: int,
     trim: bool,
     token_counter: Callable = _token_counter,
 ) -> list[str]:
-    """
-    Split markdown into lines.
-    """
-
+    """Split markdown into lines."""
     return _split_str_lines(
         text=text,
         max_tokens=max_token_per_line,
         separators=MD_SPLIT_OPTIONS,
         trim=trim,
         token_counter=token_counter,
     )
@@ -180,18 +170,15 @@
 
 def _split_text_lines(
     text: str,
     max_token_per_line: int,
     trim: bool,
     token_counter: Callable = _token_counter,
 ) -> list[str]:
-    """
-    Split text into lines.
-    """
-
+    """Split text into lines."""
     return _split_str_lines(
         text=text,
         max_tokens=max_token_per_line,
         separators=TEXT_SPLIT_OPTIONS,
         trim=trim,
         token_counter=token_counter,
     )
@@ -200,14 +187,15 @@
 def _split_str_lines(
     text: str,
     max_tokens: int,
     separators: list[list[str]],
     trim: bool,
     token_counter: Callable = _token_counter,
 ) -> list[str]:
+    """Split text into lines."""
     if not text:
         return []
 
     text = text.replace("\r\n", "\n")
     lines = []
     was_split = False
     for split_option in separators:
@@ -236,17 +224,15 @@
 def _split_str(
     text: str,
     max_tokens: int,
     separators: list[str],
     trim: bool,
     token_counter: Callable = _token_counter,
 ) -> tuple[list[str], bool]:
-    """
-    Split text into lines.
-    """
+    """Split text into lines."""
     input_was_split = False
     if not text:
         return [], input_was_split  # pragma: no cover
 
     if trim:
         text = text.strip()
 
@@ -297,17 +283,15 @@
 def _split_list(
     text: list[str],
     max_tokens: int,
     separators: list[str],
     trim: bool,
     token_counter: Callable = _token_counter,
 ) -> tuple[list[str], bool]:
-    """
-    Split list of string into lines.
-    """
+    """Split list of string into lines."""
     if not text:
         return [], False  # pragma: no cover
 
     lines = []
     input_was_split = False
     for line in text:
         split_str, was_split = _split_str(
```

### Comparing `semantic_kernel-1.0.2/semantic_kernel/utils/naming.py` & `semantic_kernel-1.0.3/semantic_kernel/utils/naming.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import random
 import string
 
 
 def generate_random_ascii_name(length: int = 16) -> str:
-    """
-    Generate a series of random ASCII characters of the specified length.
+    """Generate a series of random ASCII characters of the specified length.
+
     As example, plugin/function names can contain upper/lowercase letters, and underscores
 
     Args:
         length (int): The length of the string to generate.
 
     Returns:
         A string of random ASCII characters of the specified length.
     """
     letters = string.ascii_letters
-    return "".join(random.choices(letters, k=length))
+    return "".join(random.choices(letters, k=length))  # nosec
```

### Comparing `semantic_kernel-1.0.2/PKG-INFO` & `semantic_kernel-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-kernel
-Version: 1.0.2
+Version: 1.0.3
 Summary: Semantic Kernel Python SDK
 Author: Microsoft
 Author-email: SK-Support@microsoft.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

