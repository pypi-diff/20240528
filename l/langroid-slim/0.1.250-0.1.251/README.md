# Comparing `tmp/langroid_slim-0.1.250.tar.gz` & `tmp/langroid-slim-0.1.251.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langroid_slim-0.1.250.tar", last modified: Mon May 27 22:41:20 2024, max compression
+gzip compressed data, was "langroid-slim-0.1.251.tar", last modified: Mon May 27 23:06:30 2024, max compression
```

## Comparing `langroid_slim-0.1.250.tar` & `langroid-slim-0.1.251.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:41:20.349482 langroid_slim-0.1.250/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1065 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/LICENSE
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1872 2024-05-27 22:41:20.349482 langroid_slim-0.1.250/PKG-INFO
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    44357 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/README.md
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:41:20.306482 langroid_slim-0.1.250/langroid/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1679 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/__init__.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:41:20.308482 langroid_slim-0.1.250/langroid/agent/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      785 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    35652 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/base.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    10040 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/batch.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:41:20.308482 langroid_slim-0.1.250/langroid/agent/callbacks/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/callbacks/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    21067 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/callbacks/chainlit.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    39592 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/chat_agent.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     9316 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/chat_document.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    33056 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/openai_assistant.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:41:20.309482 langroid_slim-0.1.250/langroid/agent/special/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1207 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/special/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    55320 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/special/doc_chat_agent.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    10175 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/special/lance_doc_chat_agent.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:41:20.310482 langroid_slim-0.1.250/langroid/agent/special/lance_rag/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      174 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/special/lance_rag/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     6871 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/special/lance_rag/critic_agent.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2889 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/special/lance_rag/lance_rag_task.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     9816 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/special/lance_rag/query_planner_agent.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1456 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/special/lance_tools.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:41:20.311482 langroid_slim-0.1.250/langroid/agent/special/neo4j/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/special/neo4j/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     6374 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/special/neo4j/csv_kg_chat.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    13092 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/special/neo4j/neo4j_chat_agent.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:41:20.311482 langroid_slim-0.1.250/langroid/agent/special/neo4j/utils/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/special/neo4j/utils/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2242 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/special/neo4j/utils/system_message.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4796 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/special/relevance_extractor_agent.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1868 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/special/retriever_agent.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:41:20.311482 langroid_slim-0.1.250/langroid/agent/special/sql/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      207 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/special/sql/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    13746 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/special/sql/sql_chat_agent.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:41:20.312482 langroid_slim-0.1.250/langroid/agent/special/sql/utils/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      447 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/special/sql/utils/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     6381 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/special/sql/utils/description_extractors.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2987 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/special/sql/utils/populate_metadata.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1885 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/special/sql/utils/system_message.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1332 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/special/sql/utils/tools.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     9624 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/special/table_chat_agent.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    54020 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/task.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     8304 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/tool_message.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:41:20.313482 langroid_slim-0.1.250/langroid/agent/tools/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      304 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/tools/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1900 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/tools/duckduckgo_search_tool.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1421 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/tools/google_search_tool.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2454 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/tools/metaphor_search_tool.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     9171 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/tools/recipient_tool.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      836 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/tools/retrieval_tool.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1285 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/agent/tools/segment_extract_tool.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:41:20.314482 langroid_slim-0.1.250/langroid/cachedb/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      148 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/cachedb/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1229 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/cachedb/base.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2998 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/cachedb/momento_cachedb.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4993 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/cachedb/redis_cachedb.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:41:20.315482 langroid_slim-0.1.250/langroid/embedding_models/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      714 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/embedding_models/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1818 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/embedding_models/base.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     7144 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/embedding_models/models.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:41:20.316482 langroid_slim-0.1.250/langroid/embedding_models/protoc/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/embedding_models/protoc/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1662 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/embedding_models/protoc/embeddings_pb2.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1475 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/embedding_models/protoc/embeddings_pb2.pyi
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2452 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/embedding_models/protoc/embeddings_pb2_grpc.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     5151 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/embedding_models/remote_embeds.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:41:20.318482 langroid_slim-0.1.250/langroid/language_models/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      821 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/language_models/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     5989 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/language_models/azure_openai.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    21131 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/language_models/base.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      366 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/language_models/config.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    50668 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/language_models/openai_gpt.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:41:20.319482 langroid_slim-0.1.250/langroid/language_models/prompt_formatter/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      352 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/language_models/prompt_formatter/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1221 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/language_models/prompt_formatter/base.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     5217 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/language_models/prompt_formatter/hf_formatter.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2899 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/language_models/prompt_formatter/llama2_formatter.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4803 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/language_models/utils.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2614 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/mytypes.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:41:20.324482 langroid_slim-0.1.250/langroid/parsing/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      870 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/parsing/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1068 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/parsing/agent_chats.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     3727 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/parsing/code_parser.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    23049 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/parsing/document_parser.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2000 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/parsing/para_sentence_split.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4230 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/parsing/parse_json.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    10743 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/parsing/parser.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    29361 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/parsing/repo_loader.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     8846 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/parsing/search.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     3043 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/parsing/spider.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     3410 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/parsing/table_loader.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4472 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/parsing/url_loader.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     7975 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/parsing/urls.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    12746 2024-05-27 22:30:20.000000 langroid_slim-0.1.250/langroid/parsing/utils.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4759 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/parsing/web_search.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:41:20.326482 langroid_slim-0.1.250/langroid/prompts/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      185 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/prompts/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      331 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/prompts/dialog.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      131 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/prompts/prompts_config.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     6314 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/prompts/templates.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2706 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/prompts/transforms.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:41:20.330482 langroid_slim-0.1.250/langroid/utils/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      300 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/utils/__init__.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:41:20.331482 langroid_slim-0.1.250/langroid/utils/algorithms/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)       41 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/utils/algorithms/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2866 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/utils/algorithms/graph.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     3201 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/utils/configuration.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      563 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/utils/constants.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1343 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/utils/globals.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     3917 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/utils/logging.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:41:20.333482 langroid_slim-0.1.250/langroid/utils/output/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      341 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/utils/output/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2872 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/utils/output/printing.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1049 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/utils/output/status.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      755 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/utils/pandas_utils.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    21728 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/utils/pydantic_utils.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4546 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/utils/system.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:41:20.336482 langroid_slim-0.1.250/langroid/vector_store/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      831 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/vector_store/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    13469 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/vector_store/base.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     8109 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/vector_store/chromadb.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    18537 2024-05-27 22:32:47.000000 langroid_slim-0.1.250/langroid/vector_store/lancedb.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    11390 2024-05-27 22:33:00.000000 langroid_slim-0.1.250/langroid/vector_store/meilisearch.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    10045 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/vector_store/momento.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    16802 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/langroid/vector_store/qdrantdb.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:41:20.341482 langroid_slim-0.1.250/langroid_slim.egg-info/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1872 2024-05-27 22:41:20.000000 langroid_slim-0.1.250/langroid_slim.egg-info/PKG-INFO
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4184 2024-05-27 22:41:20.000000 langroid_slim-0.1.250/langroid_slim.egg-info/SOURCES.txt
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)        1 2024-05-27 22:41:20.000000 langroid_slim-0.1.250/langroid_slim.egg-info/dependency_links.txt
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      747 2024-05-27 22:41:20.000000 langroid_slim-0.1.250/langroid_slim.egg-info/requires.txt
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)       15 2024-05-27 22:41:20.000000 langroid_slim-0.1.250/langroid_slim.egg-info/top_level.txt
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     5649 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/pyproject.toml
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      138 2024-05-27 22:41:20.350483 langroid_slim-0.1.250/setup.cfg
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1700 2024-05-27 22:38:12.000000 langroid_slim-0.1.250/setup.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:41:20.340482 langroid_slim-0.1.250/tests/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/tests/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1930 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/tests/conftest.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1851 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/tests/test_pdf_parser_extra.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1087 2024-05-27 22:27:16.000000 langroid_slim-0.1.250/tests/utils.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:06:30.440034 langroid-slim-0.1.251/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1065 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/LICENSE
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      279 2024-05-27 23:06:30.440034 langroid-slim-0.1.251/PKG-INFO
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    44357 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/README.md
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:06:30.429033 langroid-slim-0.1.251/langroid/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1679 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/__init__.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:06:30.430033 langroid-slim-0.1.251/langroid/agent/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      787 2024-05-27 23:04:30.000000 langroid-slim-0.1.251/langroid/agent/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    35652 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/base.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    10040 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/batch.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:06:30.430033 langroid-slim-0.1.251/langroid/agent/callbacks/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/callbacks/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    21067 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/callbacks/chainlit.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    39592 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/chat_agent.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     9316 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/chat_document.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    33056 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/openai_assistant.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:06:30.431033 langroid-slim-0.1.251/langroid/agent/special/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1207 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/special/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    55320 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/special/doc_chat_agent.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    10175 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/special/lance_doc_chat_agent.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:06:30.431033 langroid-slim-0.1.251/langroid/agent/special/lance_rag/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      174 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/special/lance_rag/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     6871 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/special/lance_rag/critic_agent.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2889 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/special/lance_rag/lance_rag_task.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     9816 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/special/lance_rag/query_planner_agent.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1456 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/special/lance_tools.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:06:30.432033 langroid-slim-0.1.251/langroid/agent/special/neo4j/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/special/neo4j/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     6374 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/special/neo4j/csv_kg_chat.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    13092 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/special/neo4j/neo4j_chat_agent.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:06:30.432033 langroid-slim-0.1.251/langroid/agent/special/neo4j/utils/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/special/neo4j/utils/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2242 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/special/neo4j/utils/system_message.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4796 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/special/relevance_extractor_agent.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1868 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/special/retriever_agent.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:06:30.432033 langroid-slim-0.1.251/langroid/agent/special/sql/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      207 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/special/sql/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    13746 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/special/sql/sql_chat_agent.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:06:30.433034 langroid-slim-0.1.251/langroid/agent/special/sql/utils/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      447 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/special/sql/utils/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     6381 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/special/sql/utils/description_extractors.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2987 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/special/sql/utils/populate_metadata.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1885 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/special/sql/utils/system_message.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1332 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/special/sql/utils/tools.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     9624 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/special/table_chat_agent.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    54020 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/task.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     8304 2024-05-27 23:03:37.000000 langroid-slim-0.1.251/langroid/agent/tool_message.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:06:30.433034 langroid-slim-0.1.251/langroid/agent/tools/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      304 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/tools/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1900 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/tools/duckduckgo_search_tool.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1421 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/tools/google_search_tool.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2454 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/tools/metaphor_search_tool.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     9171 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/tools/recipient_tool.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      836 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/tools/retrieval_tool.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1285 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/agent/tools/segment_extract_tool.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:06:30.434033 langroid-slim-0.1.251/langroid/cachedb/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      148 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/cachedb/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1229 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/cachedb/base.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     3040 2024-05-27 22:59:15.000000 langroid-slim-0.1.251/langroid/cachedb/momento_cachedb.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4993 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/cachedb/redis_cachedb.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:06:30.434033 langroid-slim-0.1.251/langroid/embedding_models/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      714 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/embedding_models/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1818 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/embedding_models/base.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     7144 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/embedding_models/models.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:06:30.434033 langroid-slim-0.1.251/langroid/embedding_models/protoc/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/embedding_models/protoc/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1662 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/embedding_models/protoc/embeddings_pb2.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1475 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/embedding_models/protoc/embeddings_pb2.pyi
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2452 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/embedding_models/protoc/embeddings_pb2_grpc.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     5151 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/embedding_models/remote_embeds.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:06:30.435033 langroid-slim-0.1.251/langroid/language_models/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      821 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/language_models/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     5989 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/language_models/azure_openai.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    21131 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/language_models/base.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      366 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/language_models/config.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    50668 2024-05-27 22:59:24.000000 langroid-slim-0.1.251/langroid/language_models/openai_gpt.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:06:30.435033 langroid-slim-0.1.251/langroid/language_models/prompt_formatter/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      352 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/language_models/prompt_formatter/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1221 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/language_models/prompt_formatter/base.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     5217 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/language_models/prompt_formatter/hf_formatter.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2899 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/language_models/prompt_formatter/llama2_formatter.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4803 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/language_models/utils.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2614 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/mytypes.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:06:30.437034 langroid-slim-0.1.251/langroid/parsing/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      870 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/parsing/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1068 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/parsing/agent_chats.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     3727 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/parsing/code_parser.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    23425 2024-05-27 22:52:06.000000 langroid-slim-0.1.251/langroid/parsing/document_parser.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2000 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/parsing/para_sentence_split.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4230 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/parsing/parse_json.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    10743 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/parsing/parser.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    29361 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/parsing/repo_loader.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     8846 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/parsing/search.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     3233 2024-05-27 22:58:25.000000 langroid-slim-0.1.251/langroid/parsing/spider.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     3410 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/parsing/table_loader.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4514 2024-05-27 22:54:19.000000 langroid-slim-0.1.251/langroid/parsing/url_loader.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     7977 2024-05-27 22:54:25.000000 langroid-slim-0.1.251/langroid/parsing/urls.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    12746 2024-05-27 22:55:23.000000 langroid-slim-0.1.251/langroid/parsing/utils.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4805 2024-05-27 22:57:48.000000 langroid-slim-0.1.251/langroid/parsing/web_search.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:06:30.437034 langroid-slim-0.1.251/langroid/prompts/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      185 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/prompts/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      331 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/prompts/dialog.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      131 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/prompts/prompts_config.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     6314 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/prompts/templates.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2706 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/prompts/transforms.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:06:30.438034 langroid-slim-0.1.251/langroid/utils/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      300 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/utils/__init__.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:06:30.438034 langroid-slim-0.1.251/langroid/utils/algorithms/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)       41 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/utils/algorithms/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2866 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/utils/algorithms/graph.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     3201 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/utils/configuration.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      563 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/utils/constants.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1343 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/utils/globals.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     3917 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/utils/logging.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:06:30.438034 langroid-slim-0.1.251/langroid/utils/output/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      341 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/utils/output/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2872 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/utils/output/printing.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1049 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/utils/output/status.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      755 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/utils/pandas_utils.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    21728 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/utils/pydantic_utils.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4546 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/utils/system.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:06:30.439034 langroid-slim-0.1.251/langroid/vector_store/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      839 2024-05-27 23:03:10.000000 langroid-slim-0.1.251/langroid/vector_store/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    13469 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/vector_store/base.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     8109 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/vector_store/chromadb.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    18537 2024-05-27 22:32:47.000000 langroid-slim-0.1.251/langroid/vector_store/lancedb.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    11369 2024-05-27 23:02:32.000000 langroid-slim-0.1.251/langroid/vector_store/meilisearch.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    10045 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/vector_store/momento.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    16802 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/langroid/vector_store/qdrantdb.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:06:30.439034 langroid-slim-0.1.251/langroid_slim.egg-info/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      279 2024-05-27 23:06:30.000000 langroid-slim-0.1.251/langroid_slim.egg-info/PKG-INFO
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4184 2024-05-27 23:06:30.000000 langroid-slim-0.1.251/langroid_slim.egg-info/SOURCES.txt
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)        1 2024-05-27 23:06:30.000000 langroid-slim-0.1.251/langroid_slim.egg-info/dependency_links.txt
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      839 2024-05-27 23:06:30.000000 langroid-slim-0.1.251/langroid_slim.egg-info/requires.txt
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)       15 2024-05-27 23:06:30.000000 langroid-slim-0.1.251/langroid_slim.egg-info/top_level.txt
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     5649 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/pyproject.toml
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      138 2024-05-27 23:06:30.440034 langroid-slim-0.1.251/setup.cfg
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1858 2024-05-27 23:06:14.000000 langroid-slim-0.1.251/setup.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:06:30.439034 langroid-slim-0.1.251/tests/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/tests/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1930 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/tests/conftest.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1851 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/tests/test_pdf_parser_extra.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1087 2024-05-27 22:27:16.000000 langroid-slim-0.1.251/tests/utils.py
```

### Comparing `langroid_slim-0.1.250/LICENSE` & `langroid-slim-0.1.251/LICENSE`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/README.md` & `langroid-slim-0.1.251/README.md`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/__init__.py` & `langroid-slim-0.1.251/langroid/__init__.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/__init__.py` & `langroid-slim-0.1.251/langroid/agent/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from . import base
 from . import chat_document
 from . import chat_agent
 from . import task
 from . import batch
 from . import tool_message
 from . import tools
-from . import special
+# from . import special
 
 __all__ = [
     "Agent",
     "AgentConfig",
     "ChatDocAttachment",
     "ChatDocMetaData",
     "ChatDocLoggerFields",
```

### Comparing `langroid_slim-0.1.250/langroid/agent/base.py` & `langroid-slim-0.1.251/langroid/agent/base.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/batch.py` & `langroid-slim-0.1.251/langroid/agent/batch.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/callbacks/chainlit.py` & `langroid-slim-0.1.251/langroid/agent/callbacks/chainlit.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/chat_agent.py` & `langroid-slim-0.1.251/langroid/agent/chat_agent.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/chat_document.py` & `langroid-slim-0.1.251/langroid/agent/chat_document.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/openai_assistant.py` & `langroid-slim-0.1.251/langroid/agent/openai_assistant.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/special/__init__.py` & `langroid-slim-0.1.251/langroid/agent/special/__init__.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/special/doc_chat_agent.py` & `langroid-slim-0.1.251/langroid/agent/special/doc_chat_agent.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/special/lance_doc_chat_agent.py` & `langroid-slim-0.1.251/langroid/agent/special/lance_doc_chat_agent.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/special/lance_rag/critic_agent.py` & `langroid-slim-0.1.251/langroid/agent/special/lance_rag/critic_agent.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/special/lance_rag/lance_rag_task.py` & `langroid-slim-0.1.251/langroid/agent/special/lance_rag/lance_rag_task.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/special/lance_rag/query_planner_agent.py` & `langroid-slim-0.1.251/langroid/agent/special/lance_rag/query_planner_agent.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/special/lance_tools.py` & `langroid-slim-0.1.251/langroid/agent/special/lance_tools.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/special/neo4j/csv_kg_chat.py` & `langroid-slim-0.1.251/langroid/agent/special/neo4j/csv_kg_chat.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/special/neo4j/neo4j_chat_agent.py` & `langroid-slim-0.1.251/langroid/agent/special/neo4j/neo4j_chat_agent.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/special/neo4j/utils/system_message.py` & `langroid-slim-0.1.251/langroid/agent/special/neo4j/utils/system_message.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/special/relevance_extractor_agent.py` & `langroid-slim-0.1.251/langroid/agent/special/relevance_extractor_agent.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/special/retriever_agent.py` & `langroid-slim-0.1.251/langroid/agent/special/retriever_agent.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/special/sql/sql_chat_agent.py` & `langroid-slim-0.1.251/langroid/agent/special/sql/sql_chat_agent.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/special/sql/utils/description_extractors.py` & `langroid-slim-0.1.251/langroid/agent/special/sql/utils/description_extractors.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/special/sql/utils/populate_metadata.py` & `langroid-slim-0.1.251/langroid/agent/special/sql/utils/populate_metadata.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/special/sql/utils/system_message.py` & `langroid-slim-0.1.251/langroid/agent/special/sql/utils/system_message.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/special/sql/utils/tools.py` & `langroid-slim-0.1.251/langroid/agent/special/sql/utils/tools.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/special/table_chat_agent.py` & `langroid-slim-0.1.251/langroid/agent/special/table_chat_agent.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/task.py` & `langroid-slim-0.1.251/langroid/agent/task.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/tool_message.py` & `langroid-slim-0.1.251/langroid/agent/tool_message.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/tools/duckduckgo_search_tool.py` & `langroid-slim-0.1.251/langroid/agent/tools/duckduckgo_search_tool.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/tools/google_search_tool.py` & `langroid-slim-0.1.251/langroid/agent/tools/google_search_tool.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/tools/metaphor_search_tool.py` & `langroid-slim-0.1.251/langroid/agent/tools/metaphor_search_tool.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/tools/recipient_tool.py` & `langroid-slim-0.1.251/langroid/agent/tools/recipient_tool.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/tools/retrieval_tool.py` & `langroid-slim-0.1.251/langroid/agent/tools/retrieval_tool.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/agent/tools/segment_extract_tool.py` & `langroid-slim-0.1.251/langroid/agent/tools/segment_extract_tool.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/cachedb/base.py` & `langroid-slim-0.1.251/langroid/cachedb/base.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/cachedb/momento_cachedb.py` & `langroid-slim-0.1.251/langroid/cachedb/momento_cachedb.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import json
 import logging
 import os
 from datetime import timedelta
 from typing import Any, Dict, List
 
-import momento
+try:
+    import momento
+    from momento.responses import CacheGet
+except ImportError:
+    pass
 from dotenv import load_dotenv
-from momento.responses import CacheGet
 from pydantic import BaseModel
 
 from langroid.cachedb.base import CacheDB
 
 logger = logging.getLogger(__name__)
```

### Comparing `langroid_slim-0.1.250/langroid/cachedb/redis_cachedb.py` & `langroid-slim-0.1.251/langroid/cachedb/redis_cachedb.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/embedding_models/__init__.py` & `langroid-slim-0.1.251/langroid/embedding_models/__init__.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/embedding_models/base.py` & `langroid-slim-0.1.251/langroid/embedding_models/base.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/embedding_models/models.py` & `langroid-slim-0.1.251/langroid/embedding_models/models.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/embedding_models/protoc/embeddings_pb2.py` & `langroid-slim-0.1.251/langroid/embedding_models/protoc/embeddings_pb2.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/embedding_models/protoc/embeddings_pb2.pyi` & `langroid-slim-0.1.251/langroid/embedding_models/protoc/embeddings_pb2.pyi`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/embedding_models/protoc/embeddings_pb2_grpc.py` & `langroid-slim-0.1.251/langroid/embedding_models/protoc/embeddings_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/embedding_models/remote_embeds.py` & `langroid-slim-0.1.251/langroid/embedding_models/remote_embeds.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/language_models/__init__.py` & `langroid-slim-0.1.251/langroid/language_models/__init__.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/language_models/azure_openai.py` & `langroid-slim-0.1.251/langroid/language_models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/language_models/base.py` & `langroid-slim-0.1.251/langroid/language_models/base.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/language_models/openai_gpt.py` & `langroid-slim-0.1.251/langroid/language_models/openai_gpt.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/language_models/prompt_formatter/base.py` & `langroid-slim-0.1.251/langroid/language_models/prompt_formatter/base.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/language_models/prompt_formatter/hf_formatter.py` & `langroid-slim-0.1.251/langroid/language_models/prompt_formatter/hf_formatter.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/language_models/prompt_formatter/llama2_formatter.py` & `langroid-slim-0.1.251/langroid/language_models/prompt_formatter/llama2_formatter.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/language_models/utils.py` & `langroid-slim-0.1.251/langroid/language_models/utils.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/mytypes.py` & `langroid-slim-0.1.251/langroid/mytypes.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/parsing/__init__.py` & `langroid-slim-0.1.251/langroid/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/parsing/agent_chats.py` & `langroid-slim-0.1.251/langroid/parsing/agent_chats.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/parsing/code_parser.py` & `langroid-slim-0.1.251/langroid/parsing/code_parser.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/parsing/document_parser.py` & `langroid-slim-0.1.251/langroid/parsing/document_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 import itertools
 import logging
 import re
 from enum import Enum
 from io import BytesIO
 from typing import Any, Generator, List, Tuple
 
-import fitz
-import pdfplumber
-import pypdf
+try:
+    import fitz
+    import pdfplumber
+    import pypdf
+except ImportError:
+    pass
+
 import requests
 from bs4 import BeautifulSoup
-from PIL import Image
+try:
+    from PIL import Image
+except ImportError:
+    pass
+
 
 from langroid.mytypes import DocMetaData, Document
 from langroid.parsing.parser import Parser, ParsingConfig
 
 logger = logging.getLogger(__name__)
 
 
@@ -354,195 +362,195 @@
                     ),
                 )
             )
         self.add_window_ids(docs)
         return docs
 
 
-class FitzPDFParser(DocumentParser):
-    """
-    Parser for processing PDFs using the `fitz` library.
-    """
-
-    def iterate_pages(self) -> Generator[Tuple[int, fitz.Page], None, None]:
-        """
-        Yield each page in the PDF using `fitz`.
-
-        Returns:
-            Generator[fitz.Page]: Generator yielding each page.
-        """
-        doc = fitz.open(stream=self.doc_bytes, filetype="pdf")
-        for i, page in enumerate(doc):
-            yield i, page
-        doc.close()
-
-    def extract_text_from_page(self, page: fitz.Page) -> str:
-        """
-        Extract text from a given `fitz` page.
-
-        Args:
-            page (fitz.Page): The `fitz` page object.
-
-        Returns:
-            str: Extracted text from the page.
-        """
-        return self.fix_text(page.get_text())
-
-
-class PyPDFParser(DocumentParser):
-    """
-    Parser for processing PDFs using the `pypdf` library.
-    """
-
-    def iterate_pages(self) -> Generator[Tuple[int, pypdf.PageObject], None, None]:
-        """
-        Yield each page in the PDF using `pypdf`.
-
-        Returns:
-            Generator[pypdf.pdf.PageObject]: Generator yielding each page.
-        """
-        reader = pypdf.PdfReader(self.doc_bytes)
-        for i, page in enumerate(reader.pages):
-            yield i, page
-
-    def extract_text_from_page(self, page: pypdf.PageObject) -> str:
-        """
-        Extract text from a given `pypdf` page.
-
-        Args:
-            page (pypdf.pdf.PageObject): The `pypdf` page object.
-
-        Returns:
-            str: Extracted text from the page.
-        """
-        return self.fix_text(page.extract_text())
-
-
-class PDFPlumberParser(DocumentParser):
-    """
-    Parser for processing PDFs using the `pdfplumber` library.
-    """
-
-    def iterate_pages(
-        self,
-    ) -> (Generator)[Tuple[int, pdfplumber.pdf.Page], None, None]:  # type: ignore
-        """
-        Yield each page in the PDF using `pdfplumber`.
-
-        Returns:
-            Generator[pdfplumber.Page]: Generator yielding each page.
-        """
-        with pdfplumber.open(self.doc_bytes) as pdf:
-            for i, page in enumerate(pdf.pages):
-                yield i, page
-
-    def extract_text_from_page(self, page: pdfplumber.pdf.Page) -> str:  # type: ignore
-        """
-        Extract text from a given `pdfplumber` page.
-
-        Args:
-            page (pdfplumber.Page): The `pdfplumber` page object.
-
-        Returns:
-            str: Extracted text from the page.
-        """
-        return self.fix_text(page.extract_text())
-
-
-class ImagePdfParser(DocumentParser):
-    """
-    Parser for processing PDFs that are images, i.e. not "true" PDFs.
-    """
-
-    def iterate_pages(
-        self,
-    ) -> Generator[Tuple[int, "Image"], None, None]:  # type: ignore
-        from pdf2image import convert_from_bytes
-
-        images = convert_from_bytes(self.doc_bytes.getvalue())
-        for i, image in enumerate(images):
-            yield i, image
-
-    def extract_text_from_page(self, page: "Image") -> str:  # type: ignore
-        """
-        Extract text from a given `pdf2image` page.
-
-        Args:
-            page (Image): The PIL Image object.
-
-        Returns:
-            str: Extracted text from the image.
-        """
-        import pytesseract
-
-        text = pytesseract.image_to_string(page)
-        return self.fix_text(text)
-
-
-class UnstructuredPDFParser(DocumentParser):
-    """
-    Parser for processing PDF files using the `unstructured` library.
-    """
-
-    def iterate_pages(self) -> Generator[Tuple[int, Any], None, None]:  # type: ignore
-        try:
-            from unstructured.partition.pdf import partition_pdf
-        except ImportError:
-            raise ImportError(
-                """
-                The `unstructured` library is not installed by default with langroid.
-                To include this library, please install langroid with the
-                `unstructured` extra by running `pip install "langroid[unstructured]"`
-                or equivalent.
-                """
-            )
-
-        # from unstructured.chunking.title import chunk_by_title
-
-        try:
-            elements = partition_pdf(file=self.doc_bytes, include_page_breaks=True)
-        except Exception as e:
-            raise Exception(
-                f"""
-                Error parsing PDF: {e}
-                The `unstructured` library failed to parse the pdf.
-                Please try a different library by setting the `library` field
-                in the `pdf` section of the `parsing` field in the config file.
-                Supported libraries are:
-                fitz, pypdf, pdfplumber, unstructured
-                """
-            )
-
-        # elements = chunk_by_title(elements)
-        page_number = 1
-        page_elements = []  # type: ignore
-        for el in elements:
-            if el.category == "PageBreak":
-                if page_elements:  # Avoid yielding empty pages at the start
-                    yield page_number, page_elements
-                page_number += 1
-                page_elements = []
-            else:
-                page_elements.append(el)
-        # Yield the last page if it's not empty
-        if page_elements:
-            yield page_number, page_elements
-
-    def extract_text_from_page(self, page: Any) -> str:
-        """
-        Extract text from a given `unstructured` element.
-
-        Args:
-            page (unstructured element): The `unstructured` element object.
-
-        Returns:
-            str: Extracted text from the element.
-        """
-        text = " ".join(el.text for el in page)
-        return self.fix_text(text)
+# class FitzPDFParser(DocumentParser):
+#     """
+#     Parser for processing PDFs using the `fitz` library.
+#     """
+
+#     def iterate_pages(self) -> Generator[Tuple[int, fitz.Page], None, None]:
+#         """
+#         Yield each page in the PDF using `fitz`.
+
+#         Returns:
+#             Generator[fitz.Page]: Generator yielding each page.
+#         """
+#         doc = fitz.open(stream=self.doc_bytes, filetype="pdf")
+#         for i, page in enumerate(doc):
+#             yield i, page
+#         doc.close()
+
+#     def extract_text_from_page(self, page: fitz.Page) -> str:
+#         """
+#         Extract text from a given `fitz` page.
+
+#         Args:
+#             page (fitz.Page): The `fitz` page object.
+
+#         Returns:
+#             str: Extracted text from the page.
+#         """
+#         return self.fix_text(page.get_text())
+
+
+# class PyPDFParser(DocumentParser):
+#     """
+#     Parser for processing PDFs using the `pypdf` library.
+#     """
+
+#     def iterate_pages(self) -> Generator[Tuple[int, pypdf.PageObject], None, None]:
+#         """
+#         Yield each page in the PDF using `pypdf`.
+
+#         Returns:
+#             Generator[pypdf.pdf.PageObject]: Generator yielding each page.
+#         """
+#         reader = pypdf.PdfReader(self.doc_bytes)
+#         for i, page in enumerate(reader.pages):
+#             yield i, page
+
+#     def extract_text_from_page(self, page: pypdf.PageObject) -> str:
+#         """
+#         Extract text from a given `pypdf` page.
+
+#         Args:
+#             page (pypdf.pdf.PageObject): The `pypdf` page object.
+
+#         Returns:
+#             str: Extracted text from the page.
+#         """
+#         return self.fix_text(page.extract_text())
+
+
+# class PDFPlumberParser(DocumentParser):
+#     """
+#     Parser for processing PDFs using the `pdfplumber` library.
+#     """
+
+#     def iterate_pages(
+#         self,
+#     ) -> (Generator)[Tuple[int, pdfplumber.pdf.Page], None, None]:  # type: ignore
+#         """
+#         Yield each page in the PDF using `pdfplumber`.
+
+#         Returns:
+#             Generator[pdfplumber.Page]: Generator yielding each page.
+#         """
+#         with pdfplumber.open(self.doc_bytes) as pdf:
+#             for i, page in enumerate(pdf.pages):
+#                 yield i, page
+
+#     def extract_text_from_page(self, page: pdfplumber.pdf.Page) -> str:  # type: ignore
+#         """
+#         Extract text from a given `pdfplumber` page.
+
+#         Args:
+#             page (pdfplumber.Page): The `pdfplumber` page object.
+
+#         Returns:
+#             str: Extracted text from the page.
+#         """
+#         return self.fix_text(page.extract_text())
+
+
+# class ImagePdfParser(DocumentParser):
+#     """
+#     Parser for processing PDFs that are images, i.e. not "true" PDFs.
+#     """
+
+#     def iterate_pages(
+#         self,
+#     ) -> Generator[Tuple[int, "Image"], None, None]:  # type: ignore
+#         from pdf2image import convert_from_bytes
+
+#         images = convert_from_bytes(self.doc_bytes.getvalue())
+#         for i, image in enumerate(images):
+#             yield i, image
+
+#     def extract_text_from_page(self, page: "Image") -> str:  # type: ignore
+#         """
+#         Extract text from a given `pdf2image` page.
+
+#         Args:
+#             page (Image): The PIL Image object.
+
+#         Returns:
+#             str: Extracted text from the image.
+#         """
+#         import pytesseract
+
+#         text = pytesseract.image_to_string(page)
+#         return self.fix_text(text)
+
+
+# class UnstructuredPDFParser(DocumentParser):
+#     """
+#     Parser for processing PDF files using the `unstructured` library.
+#     """
+
+#     def iterate_pages(self) -> Generator[Tuple[int, Any], None, None]:  # type: ignore
+#         try:
+#             from unstructured.partition.pdf import partition_pdf
+#         except ImportError:
+#             raise ImportError(
+#                 """
+#                 The `unstructured` library is not installed by default with langroid.
+#                 To include this library, please install langroid with the
+#                 `unstructured` extra by running `pip install "langroid[unstructured]"`
+#                 or equivalent.
+#                 """
+#             )
+
+#         # from unstructured.chunking.title import chunk_by_title
+
+#         try:
+#             elements = partition_pdf(file=self.doc_bytes, include_page_breaks=True)
+#         except Exception as e:
+#             raise Exception(
+#                 f"""
+#                 Error parsing PDF: {e}
+#                 The `unstructured` library failed to parse the pdf.
+#                 Please try a different library by setting the `library` field
+#                 in the `pdf` section of the `parsing` field in the config file.
+#                 Supported libraries are:
+#                 fitz, pypdf, pdfplumber, unstructured
+#                 """
+#             )
+
+#         # elements = chunk_by_title(elements)
+#         page_number = 1
+#         page_elements = []  # type: ignore
+#         for el in elements:
+#             if el.category == "PageBreak":
+#                 if page_elements:  # Avoid yielding empty pages at the start
+#                     yield page_number, page_elements
+#                 page_number += 1
+#                 page_elements = []
+#             else:
+#                 page_elements.append(el)
+#         # Yield the last page if it's not empty
+#         if page_elements:
+#             yield page_number, page_elements
+
+#     def extract_text_from_page(self, page: Any) -> str:
+#         """
+#         Extract text from a given `unstructured` element.
+
+#         Args:
+#             page (unstructured element): The `unstructured` element object.
+
+#         Returns:
+#             str: Extracted text from the element.
+#         """
+#         text = " ".join(el.text for el in page)
+#         return self.fix_text(text)
 
 
 class UnstructuredDocxParser(DocumentParser):
     """
     Parser for processing DOCX files using the `unstructured` library.
     """
```

### Comparing `langroid_slim-0.1.250/langroid/parsing/para_sentence_split.py` & `langroid-slim-0.1.251/langroid/parsing/para_sentence_split.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/parsing/parse_json.py` & `langroid-slim-0.1.251/langroid/parsing/parse_json.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/parsing/parser.py` & `langroid-slim-0.1.251/langroid/parsing/parser.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/parsing/repo_loader.py` & `langroid-slim-0.1.251/langroid/parsing/repo_loader.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/parsing/search.py` & `langroid-slim-0.1.251/langroid/parsing/search.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/parsing/spider.py` & `langroid-slim-0.1.251/langroid/parsing/spider.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,97 +1,100 @@
 from typing import List, Set, no_type_check
 from urllib.parse import urlparse
 
-from pydispatch import dispatcher
-from scrapy import signals
-from scrapy.crawler import CrawlerRunner
-from scrapy.http import Response
-from scrapy.linkextractors import LinkExtractor
-from scrapy.spiders import CrawlSpider, Rule
-from twisted.internet import defer, reactor
-
-
-@no_type_check
-class DomainSpecificSpider(CrawlSpider):  # type: ignore
-    name = "domain_specific_spider"
-
-    custom_settings = {"DEPTH_LIMIT": 1, "CLOSESPIDER_ITEMCOUNT": 20}
-
-    rules = (Rule(LinkExtractor(), callback="parse_item", follow=True),)
-
-    def __init__(self, start_url: str, k: int = 20, *args, **kwargs):  # type: ignore
-        """Initialize the spider with start_url and k.
-
-        Args:
-            start_url (str): The starting URL.
-            k (int, optional): The max desired final URLs. Defaults to 20.
-        """
-        super(DomainSpecificSpider, self).__init__(*args, **kwargs)
-        self.start_urls = [start_url]
-        self.allowed_domains = [urlparse(start_url).netloc]
-        self.k = k
-        self.visited_urls: Set[str] = set()
-
-    def parse_item(self, response: Response):  # type: ignore
-        """Extracts URLs that are within the same domain.
-
-        Args:
-            response: The scrapy response object.
-        """
-        for link in LinkExtractor(allow_domains=self.allowed_domains).extract_links(
-            response
-        ):
-            if len(self.visited_urls) < self.k:
-                self.visited_urls.add(link.url)
-                yield {"url": link.url}
-
-
-@no_type_check
-def scrapy_fetch_urls(url: str, k: int = 20) -> List[str]:
-    """Fetches up to k URLs reachable from the input URL using Scrapy.
-
-    Args:
-        url (str): The starting URL.
-        k (int, optional): The max desired final URLs. Defaults to 20.
-
-    Returns:
-        List[str]: List of URLs within the same domain as the input URL.
-    """
-    urls = []
-
-    def _collect_urls(spider):
-        """Handler for the spider_closed signal. Collects the visited URLs."""
-        nonlocal urls
-        urls.extend(list(spider.visited_urls))
-
-    # Connect the spider_closed signal with our handler
-    dispatcher.connect(_collect_urls, signal=signals.spider_closed)
-
-    runner = CrawlerRunner(
-        {
-            "USER_AGENT": "Mozilla/5.0 (compatible; Googlebot/2.1; +http://www.google.com/bot.html)"
-        }
-    )
-
-    d = runner.crawl(DomainSpecificSpider, start_url=url, k=k)
-
-    # Block until crawling is done and then stop the reactor
-    crawl_deferred = defer.Deferred()
-
-    def _crawl_done(_):
-        reactor.stop()
-        crawl_deferred.callback(urls)
-
-    d.addBoth(_crawl_done)
-
-    # Start the reactor, it will stop once the crawl is done
-    reactor.run(installSignalHandlers=0)
-
-    # This will block until the deferred gets a result
-    return crawl_deferred.result
-
-
-# Test the function
-if __name__ == "__main__":
-    fetched_urls = scrapy_fetch_urls("https://example.com", 5)
-    for url in fetched_urls:
-        print(url)
+try:
+    from pydispatch import dispatcher
+    from scrapy import signals
+    from scrapy.crawler import CrawlerRunner
+    from scrapy.http import Response
+    from scrapy.linkextractors import LinkExtractor
+    from scrapy.spiders import CrawlSpider, Rule
+    from twisted.internet import defer, reactor
+except ImportError:
+    pass
+
+
+# @no_type_check
+# class DomainSpecificSpider(CrawlSpider):  # type: ignore
+#     name = "domain_specific_spider"
+
+#     custom_settings = {"DEPTH_LIMIT": 1, "CLOSESPIDER_ITEMCOUNT": 20}
+
+#     rules = (Rule(LinkExtractor(), callback="parse_item", follow=True),)
+
+#     def __init__(self, start_url: str, k: int = 20, *args, **kwargs):  # type: ignore
+#         """Initialize the spider with start_url and k.
+
+#         Args:
+#             start_url (str): The starting URL.
+#             k (int, optional): The max desired final URLs. Defaults to 20.
+#         """
+#         super(DomainSpecificSpider, self).__init__(*args, **kwargs)
+#         self.start_urls = [start_url]
+#         self.allowed_domains = [urlparse(start_url).netloc]
+#         self.k = k
+#         self.visited_urls: Set[str] = set()
+
+#     def parse_item(self, response: Response):  # type: ignore
+#         """Extracts URLs that are within the same domain.
+
+#         Args:
+#             response: The scrapy response object.
+#         """
+#         for link in LinkExtractor(allow_domains=self.allowed_domains).extract_links(
+#             response
+#         ):
+#             if len(self.visited_urls) < self.k:
+#                 self.visited_urls.add(link.url)
+#                 yield {"url": link.url}
+
+
+# @no_type_check
+# def scrapy_fetch_urls(url: str, k: int = 20) -> List[str]:
+#     """Fetches up to k URLs reachable from the input URL using Scrapy.
+
+#     Args:
+#         url (str): The starting URL.
+#         k (int, optional): The max desired final URLs. Defaults to 20.
+
+#     Returns:
+#         List[str]: List of URLs within the same domain as the input URL.
+#     """
+#     urls = []
+
+#     def _collect_urls(spider):
+#         """Handler for the spider_closed signal. Collects the visited URLs."""
+#         nonlocal urls
+#         urls.extend(list(spider.visited_urls))
+
+#     # Connect the spider_closed signal with our handler
+#     dispatcher.connect(_collect_urls, signal=signals.spider_closed)
+
+#     runner = CrawlerRunner(
+#         {
+#             "USER_AGENT": "Mozilla/5.0 (compatible; Googlebot/2.1; +http://www.google.com/bot.html)"
+#         }
+#     )
+
+#     d = runner.crawl(DomainSpecificSpider, start_url=url, k=k)
+
+#     # Block until crawling is done and then stop the reactor
+#     crawl_deferred = defer.Deferred()
+
+#     def _crawl_done(_):
+#         reactor.stop()
+#         crawl_deferred.callback(urls)
+
+#     d.addBoth(_crawl_done)
+
+#     # Start the reactor, it will stop once the crawl is done
+#     reactor.run(installSignalHandlers=0)
+
+#     # This will block until the deferred gets a result
+#     return crawl_deferred.result
+
+
+# # Test the function
+# if __name__ == "__main__":
+#     fetched_urls = scrapy_fetch_urls("https://example.com", 5)
+#     for url in fetched_urls:
+#         print(url)
```

### Comparing `langroid_slim-0.1.250/langroid/parsing/table_loader.py` & `langroid-slim-0.1.251/langroid/parsing/table_loader.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/parsing/url_loader.py` & `langroid-slim-0.1.251/langroid/parsing/url_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import logging
 import os
 from tempfile import NamedTemporaryFile
 from typing import List, no_type_check
 
 import requests
-import trafilatura
-from trafilatura.downloads import (
-    add_to_compressed_dict,
-    buffered_downloads,
-    load_download_buffer,
-)
+try:
+    import trafilatura
+    from trafilatura.downloads import (
+        add_to_compressed_dict,
+        buffered_downloads,
+        load_download_buffer,
+    )
+except ImportError:
+    pass
 
 from langroid.mytypes import DocMetaData, Document
-from langroid.parsing.document_parser import DocumentParser, ImagePdfParser
+from langroid.parsing.document_parser import DocumentParser
 from langroid.parsing.parser import Parser, ParsingConfig
 
 logging.getLogger("trafilatura").setLevel(logging.ERROR)
 
 
 class URLLoader:
     """
```

### Comparing `langroid_slim-0.1.250/langroid/parsing/urls.py` & `langroid-slim-0.1.251/langroid/parsing/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import fire
 import requests
 from bs4 import BeautifulSoup
 from pydantic import BaseModel, HttpUrl, ValidationError, parse_obj_as
 from rich import print
 from rich.prompt import Prompt
-from trafilatura.spider import focused_crawler
+# from trafilatura.spider import focused_crawler
 
 logger = logging.getLogger(__name__)
 
 
 def url_to_tempfile(url: str) -> str:
     """
     Fetch content from the given URL and save it to a temporary local file.
```

### Comparing `langroid_slim-0.1.250/langroid/parsing/utils.py` & `langroid-slim-0.1.251/langroid/parsing/utils.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/parsing/web_search.py` & `langroid-slim-0.1.251/langroid/parsing/web_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,20 @@
 
 import os
 from typing import Dict, List
 
 import requests
 from bs4 import BeautifulSoup
 from dotenv import load_dotenv
-from duckduckgo_search import DDGS
-from googleapiclient.discovery import Resource, build
-from requests.models import Response
+try:
+    from duckduckgo_search import DDGS
+    from googleapiclient.discovery import Resource, build
+    from requests.models import Response
+except ImportError:
+    pass
 
 
 class WebSearchResult:
     """
     Class representing a Web Search result, containing the title, link,
     summary and full content of the result.
     """
```

### Comparing `langroid_slim-0.1.250/langroid/prompts/templates.py` & `langroid-slim-0.1.251/langroid/prompts/templates.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/prompts/transforms.py` & `langroid-slim-0.1.251/langroid/prompts/transforms.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/utils/algorithms/graph.py` & `langroid-slim-0.1.251/langroid/utils/algorithms/graph.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/utils/configuration.py` & `langroid-slim-0.1.251/langroid/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/utils/constants.py` & `langroid-slim-0.1.251/langroid/utils/constants.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/utils/globals.py` & `langroid-slim-0.1.251/langroid/utils/globals.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/utils/logging.py` & `langroid-slim-0.1.251/langroid/utils/logging.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/utils/output/printing.py` & `langroid-slim-0.1.251/langroid/utils/output/printing.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/utils/output/status.py` & `langroid-slim-0.1.251/langroid/utils/output/status.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/utils/pandas_utils.py` & `langroid-slim-0.1.251/langroid/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/utils/pydantic_utils.py` & `langroid-slim-0.1.251/langroid/utils/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/utils/system.py` & `langroid-slim-0.1.251/langroid/utils/system.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/vector_store/__init__.py` & `langroid-slim-0.1.251/langroid/vector_store/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from . import base
 
 from . import qdrantdb
-from . import meilisearch
-from . import lancedb
+# from . import meilisearch
+# from . import lancedb
 
 from .base import VectorStoreConfig, VectorStore
 from .qdrantdb import QdrantDBConfig, QdrantDB
-from .meilisearch import MeiliSearch, MeiliSearchConfig
-from .lancedb import LanceDB, LanceDBConfig
+# from .meilisearch import MeiliSearch, MeiliSearchConfig
+# from .lancedb import LanceDB, LanceDBConfig
 
 has_chromadb = False
 try:
     from . import chromadb
     from .chromadb import ChromaDBConfig, ChromaDB
 
     chromadb  # silence linters
```

### Comparing `langroid_slim-0.1.250/langroid/vector_store/base.py` & `langroid-slim-0.1.251/langroid/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/vector_store/chromadb.py` & `langroid-slim-0.1.251/langroid/vector_store/chromadb.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/vector_store/lancedb.py` & `langroid-slim-0.1.251/langroid/vector_store/lancedb.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/vector_store/meilisearch.py` & `langroid-slim-0.1.251/langroid/vector_store/meilisearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,20 +94,20 @@
         """
         List all collections, including empty ones.
         Returns:
             List of collection names.
         """
         return self.list_collections()
 
-    async def _async_get_indexes(self) -> List[AsyncIndex]:
+    async def _async_get_indexes(self) -> List[Any]:
         async with self.client() as client:
             indexes = await client.get_indexes(limit=10_000)
         return [] if indexes is None else indexes
 
-    async def _async_get_index(self, index_uid: str) -> AsyncIndex:
+    async def _async_get_index(self, index_uid: str) -> Any:
         async with self.client() as client:
             index = await client.get_index(index_uid)
         return index
 
     def list_collections(self, empty: bool = False) -> List[str]:
         """
         Returns:
@@ -115,15 +115,15 @@
         """
         indexes = asyncio.run(self._async_get_indexes())
         if len(indexes) == 0:
             return []
         else:
             return [ind.uid for ind in indexes]
 
-    async def _async_create_index(self, collection_name: str) -> AsyncIndex:
+    async def _async_create_index(self, collection_name: str) -> Any:
         async with self.client() as client:
             index = await client.create_index(
                 uid=collection_name,
                 primary_key=self.config.primary_key,
             )
         return index
```

### Comparing `langroid_slim-0.1.250/langroid/vector_store/momento.py` & `langroid-slim-0.1.251/langroid/vector_store/momento.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid/vector_store/qdrantdb.py` & `langroid-slim-0.1.251/langroid/vector_store/qdrantdb.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid_slim.egg-info/SOURCES.txt` & `langroid-slim-0.1.251/langroid_slim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/langroid_slim.egg-info/requires.txt` & `langroid-slim-0.1.251/langroid_slim.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 requests>=2.31.0
 types-redis>=4.5.5.2
 types-requests>=2.31.0.1
 pyparsing>=3.0.9
 nltk>=3.8.1
 qdrant-client>=1.8.0
 pydantic==1.10.13
+pandas>=2.1.3
+pyyaml>=6.0
+rank-bm25>=0.2.2
+groq>=0.5.0
+jinja2>=3.1.2
+docstring-parser>=0.15
 
 [docs]
 mkdocs>=1.4.2
 mkdocs-material>=9.1.5
 mkdocstrings[python]>=0.21.2
 mkdocs-awesome-pages-plugin>=2.8.0
 mkdocs-rss-plugin>=1.8.0
```

### Comparing `langroid_slim-0.1.250/pyproject.toml` & `langroid-slim-0.1.251/pyproject.toml`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/setup.py` & `langroid-slim-0.1.251/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """A minimal setup.py for Langroid
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name="langroid-slim",
-    version="0.1.250",
+    version="0.1.251",
     description="Harness LLMs with Multi-Agent Programming",
     author="Prasad Chalasani",
     author_email="pchalasani@gmail.com",
     license="MIT",
     packages=find_packages(),
     install_requires=[
         "onnxruntime==1.16.1",
@@ -30,15 +30,21 @@
         "fakeredis>=2.12.1",
         "requests>=2.31.0",
         "types-redis>=4.5.5.2",
         "types-requests>=2.31.0.1",
         "pyparsing>=3.0.9",
         "nltk>=3.8.1",
         "qdrant-client>=1.8.0",
-        "pydantic==1.10.13"
+        "pydantic==1.10.13",
+        "pandas>=2.1.3",
+        "pyyaml>=6.0",
+        "rank-bm25>=0.2.2",
+        "groq>=0.5.0",
+        "jinja2>=3.1.2",
+        "docstring-parser>=0.15"
     ],
     python_requires=">=3.10, <3.12",
     extras_require={
         "extra":[
             "ruff>=0.2.2",
             "pre-commit>=3.3.2",
             "flake8>=6.0.0",
```

### Comparing `langroid_slim-0.1.250/tests/conftest.py` & `langroid-slim-0.1.251/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/tests/test_pdf_parser_extra.py` & `langroid-slim-0.1.251/tests/test_pdf_parser_extra.py`

 * *Files identical despite different names*

### Comparing `langroid_slim-0.1.250/tests/utils.py` & `langroid-slim-0.1.251/tests/utils.py`

 * *Files identical despite different names*

