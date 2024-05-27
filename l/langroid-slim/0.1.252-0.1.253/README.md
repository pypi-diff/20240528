# Comparing `tmp/langroid-slim-0.1.252.tar.gz` & `tmp/langroid-slim-0.1.253.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langroid-slim-0.1.252.tar", last modified: Mon May 27 23:15:41 2024, max compression
+gzip compressed data, was "langroid-slim-0.1.253.tar", last modified: Mon May 27 23:20:15 2024, max compression
```

## Comparing `langroid-slim-0.1.252.tar` & `langroid-slim-0.1.253.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:15:41.538592 langroid-slim-0.1.252/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1065 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/LICENSE
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      279 2024-05-27 23:15:41.538592 langroid-slim-0.1.252/PKG-INFO
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    44357 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/README.md
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:15:41.517591 langroid-slim-0.1.252/langroid/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1679 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/__init__.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:15:41.518591 langroid-slim-0.1.252/langroid/agent/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      787 2024-05-27 23:04:30.000000 langroid-slim-0.1.252/langroid/agent/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    35652 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/base.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    10040 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/batch.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:15:41.519591 langroid-slim-0.1.252/langroid/agent/callbacks/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/callbacks/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    21067 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/callbacks/chainlit.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    39592 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/chat_agent.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     9316 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/chat_document.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    33056 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/openai_assistant.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:15:41.520591 langroid-slim-0.1.252/langroid/agent/special/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1207 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/special/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    55320 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/special/doc_chat_agent.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    10175 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/special/lance_doc_chat_agent.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:15:41.520591 langroid-slim-0.1.252/langroid/agent/special/lance_rag/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      174 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/special/lance_rag/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     6871 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/special/lance_rag/critic_agent.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2889 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/special/lance_rag/lance_rag_task.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     9816 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/special/lance_rag/query_planner_agent.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1456 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/special/lance_tools.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:15:41.521592 langroid-slim-0.1.252/langroid/agent/special/neo4j/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/special/neo4j/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     6374 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/special/neo4j/csv_kg_chat.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    13092 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/special/neo4j/neo4j_chat_agent.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:15:41.521592 langroid-slim-0.1.252/langroid/agent/special/neo4j/utils/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/special/neo4j/utils/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2242 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/special/neo4j/utils/system_message.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4796 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/special/relevance_extractor_agent.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1868 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/special/retriever_agent.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:15:41.522591 langroid-slim-0.1.252/langroid/agent/special/sql/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      207 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/special/sql/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    13746 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/special/sql/sql_chat_agent.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:15:41.523591 langroid-slim-0.1.252/langroid/agent/special/sql/utils/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      447 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/special/sql/utils/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     6381 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/special/sql/utils/description_extractors.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2987 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/special/sql/utils/populate_metadata.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1885 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/special/sql/utils/system_message.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1332 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/special/sql/utils/tools.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     9624 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/special/table_chat_agent.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    54020 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/task.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     8304 2024-05-27 23:03:37.000000 langroid-slim-0.1.252/langroid/agent/tool_message.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:15:41.525591 langroid-slim-0.1.252/langroid/agent/tools/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      304 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/tools/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1900 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/tools/duckduckgo_search_tool.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1421 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/tools/google_search_tool.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2454 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/tools/metaphor_search_tool.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     9171 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/tools/recipient_tool.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      836 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/tools/retrieval_tool.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1285 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/agent/tools/segment_extract_tool.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:15:41.526592 langroid-slim-0.1.252/langroid/cachedb/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      148 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/cachedb/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1229 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/cachedb/base.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     3040 2024-05-27 22:59:15.000000 langroid-slim-0.1.252/langroid/cachedb/momento_cachedb.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4993 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/cachedb/redis_cachedb.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:15:41.527592 langroid-slim-0.1.252/langroid/embedding_models/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      714 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/embedding_models/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1818 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/embedding_models/base.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     7144 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/embedding_models/models.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:15:41.528591 langroid-slim-0.1.252/langroid/embedding_models/protoc/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/embedding_models/protoc/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1662 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/embedding_models/protoc/embeddings_pb2.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1475 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/embedding_models/protoc/embeddings_pb2.pyi
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2452 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/embedding_models/protoc/embeddings_pb2_grpc.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     5151 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/embedding_models/remote_embeds.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:15:41.530592 langroid-slim-0.1.252/langroid/language_models/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      821 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/language_models/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     5989 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/language_models/azure_openai.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    21131 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/language_models/base.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      366 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/language_models/config.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    50668 2024-05-27 22:59:24.000000 langroid-slim-0.1.252/langroid/language_models/openai_gpt.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:15:41.531592 langroid-slim-0.1.252/langroid/language_models/prompt_formatter/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      352 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/language_models/prompt_formatter/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1221 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/language_models/prompt_formatter/base.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     5217 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/language_models/prompt_formatter/hf_formatter.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2899 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/language_models/prompt_formatter/llama2_formatter.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4803 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/language_models/utils.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2614 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/mytypes.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:15:41.534592 langroid-slim-0.1.252/langroid/parsing/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      870 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/parsing/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1068 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/parsing/agent_chats.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     3727 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/parsing/code_parser.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    23425 2024-05-27 22:52:06.000000 langroid-slim-0.1.252/langroid/parsing/document_parser.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2000 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/parsing/para_sentence_split.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4230 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/parsing/parse_json.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    10743 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/parsing/parser.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    29361 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/parsing/repo_loader.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     8846 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/parsing/search.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     3233 2024-05-27 22:58:25.000000 langroid-slim-0.1.252/langroid/parsing/spider.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     3410 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/parsing/table_loader.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4514 2024-05-27 22:54:19.000000 langroid-slim-0.1.252/langroid/parsing/url_loader.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     7977 2024-05-27 22:54:25.000000 langroid-slim-0.1.252/langroid/parsing/urls.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    12746 2024-05-27 22:55:23.000000 langroid-slim-0.1.252/langroid/parsing/utils.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4805 2024-05-27 22:57:48.000000 langroid-slim-0.1.252/langroid/parsing/web_search.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:15:41.535592 langroid-slim-0.1.252/langroid/prompts/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      185 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/prompts/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      331 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/prompts/dialog.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      131 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/prompts/prompts_config.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     6314 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/prompts/templates.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2706 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/prompts/transforms.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:15:41.536592 langroid-slim-0.1.252/langroid/utils/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      300 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/utils/__init__.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:15:41.536592 langroid-slim-0.1.252/langroid/utils/algorithms/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)       41 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/utils/algorithms/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2866 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/utils/algorithms/graph.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     3201 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/utils/configuration.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      563 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/utils/constants.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1343 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/utils/globals.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     3917 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/utils/logging.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:15:41.536592 langroid-slim-0.1.252/langroid/utils/output/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      341 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/utils/output/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2872 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/utils/output/printing.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1049 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/utils/output/status.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      755 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/utils/pandas_utils.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    21728 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/utils/pydantic_utils.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4546 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/utils/system.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:15:41.537592 langroid-slim-0.1.252/langroid/vector_store/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      839 2024-05-27 23:03:10.000000 langroid-slim-0.1.252/langroid/vector_store/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    13469 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/vector_store/base.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     8109 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/vector_store/chromadb.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    18537 2024-05-27 22:32:47.000000 langroid-slim-0.1.252/langroid/vector_store/lancedb.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    11369 2024-05-27 23:02:32.000000 langroid-slim-0.1.252/langroid/vector_store/meilisearch.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    10045 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/vector_store/momento.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)    16802 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/langroid/vector_store/qdrantdb.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:15:41.538592 langroid-slim-0.1.252/langroid_slim.egg-info/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      279 2024-05-27 23:15:41.000000 langroid-slim-0.1.252/langroid_slim.egg-info/PKG-INFO
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4184 2024-05-27 23:15:41.000000 langroid-slim-0.1.252/langroid_slim.egg-info/SOURCES.txt
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)        1 2024-05-27 23:15:41.000000 langroid-slim-0.1.252/langroid_slim.egg-info/dependency_links.txt
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      839 2024-05-27 23:15:41.000000 langroid-slim-0.1.252/langroid_slim.egg-info/requires.txt
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)       15 2024-05-27 23:15:41.000000 langroid-slim-0.1.252/langroid_slim.egg-info/top_level.txt
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     5649 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/pyproject.toml
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)      138 2024-05-27 23:15:41.539592 langroid-slim-0.1.252/setup.cfg
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1858 2024-05-27 23:15:33.000000 langroid-slim-0.1.252/setup.py
-drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:15:41.538592 langroid-slim-0.1.252/tests/
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/tests/__init__.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1930 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/tests/conftest.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1851 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/tests/test_pdf_parser_extra.py
--rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1087 2024-05-27 22:27:16.000000 langroid-slim-0.1.252/tests/utils.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:20:15.940593 langroid-slim-0.1.253/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1065 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/LICENSE
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      279 2024-05-27 23:20:15.940593 langroid-slim-0.1.253/PKG-INFO
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    44357 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/README.md
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:20:15.861591 langroid-slim-0.1.253/langroid/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1679 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/__init__.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:20:15.869592 langroid-slim-0.1.253/langroid/agent/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      787 2024-05-27 23:04:30.000000 langroid-slim-0.1.253/langroid/agent/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    35652 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/base.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    10040 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/batch.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:20:15.871592 langroid-slim-0.1.253/langroid/agent/callbacks/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/callbacks/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    21067 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/callbacks/chainlit.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    39592 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/chat_agent.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     9316 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/chat_document.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    33056 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/openai_assistant.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:20:15.876592 langroid-slim-0.1.253/langroid/agent/special/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1207 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/special/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    55320 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/special/doc_chat_agent.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    10175 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/special/lance_doc_chat_agent.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:20:15.879592 langroid-slim-0.1.253/langroid/agent/special/lance_rag/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      174 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/special/lance_rag/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     6871 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/special/lance_rag/critic_agent.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2889 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/special/lance_rag/lance_rag_task.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     9816 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/special/lance_rag/query_planner_agent.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1456 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/special/lance_tools.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:20:15.881592 langroid-slim-0.1.253/langroid/agent/special/neo4j/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/special/neo4j/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     6374 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/special/neo4j/csv_kg_chat.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    13092 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/special/neo4j/neo4j_chat_agent.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:20:15.883592 langroid-slim-0.1.253/langroid/agent/special/neo4j/utils/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/special/neo4j/utils/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2242 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/special/neo4j/utils/system_message.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4796 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/special/relevance_extractor_agent.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1868 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/special/retriever_agent.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:20:15.884592 langroid-slim-0.1.253/langroid/agent/special/sql/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      207 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/special/sql/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    13746 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/special/sql/sql_chat_agent.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:20:15.888592 langroid-slim-0.1.253/langroid/agent/special/sql/utils/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      447 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/special/sql/utils/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     6381 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/special/sql/utils/description_extractors.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2987 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/special/sql/utils/populate_metadata.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1885 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/special/sql/utils/system_message.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1332 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/special/sql/utils/tools.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     9624 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/special/table_chat_agent.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    54020 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/task.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     8304 2024-05-27 23:03:37.000000 langroid-slim-0.1.253/langroid/agent/tool_message.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:20:15.893592 langroid-slim-0.1.253/langroid/agent/tools/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      304 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/tools/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1900 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/tools/duckduckgo_search_tool.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1421 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/tools/google_search_tool.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2454 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/tools/metaphor_search_tool.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     9171 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/tools/recipient_tool.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      836 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/tools/retrieval_tool.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1285 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/agent/tools/segment_extract_tool.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:20:15.896592 langroid-slim-0.1.253/langroid/cachedb/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      148 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/cachedb/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1229 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/cachedb/base.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     3040 2024-05-27 22:59:15.000000 langroid-slim-0.1.253/langroid/cachedb/momento_cachedb.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4993 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/cachedb/redis_cachedb.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:20:15.900592 langroid-slim-0.1.253/langroid/embedding_models/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      714 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/embedding_models/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1818 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/embedding_models/base.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     7144 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/embedding_models/models.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:20:15.902593 langroid-slim-0.1.253/langroid/embedding_models/protoc/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/embedding_models/protoc/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1662 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/embedding_models/protoc/embeddings_pb2.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1475 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/embedding_models/protoc/embeddings_pb2.pyi
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2452 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/embedding_models/protoc/embeddings_pb2_grpc.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     5151 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/embedding_models/remote_embeds.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:20:15.909592 langroid-slim-0.1.253/langroid/language_models/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      821 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/language_models/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     5989 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/language_models/azure_openai.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    21131 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/language_models/base.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      366 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/language_models/config.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    50668 2024-05-27 22:59:24.000000 langroid-slim-0.1.253/langroid/language_models/openai_gpt.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:20:15.911593 langroid-slim-0.1.253/langroid/language_models/prompt_formatter/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      352 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/language_models/prompt_formatter/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1221 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/language_models/prompt_formatter/base.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     5217 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/language_models/prompt_formatter/hf_formatter.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2899 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/language_models/prompt_formatter/llama2_formatter.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4803 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/language_models/utils.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2614 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/mytypes.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:20:15.924593 langroid-slim-0.1.253/langroid/parsing/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      870 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/parsing/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1068 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/parsing/agent_chats.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     3727 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/parsing/code_parser.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    23425 2024-05-27 22:52:06.000000 langroid-slim-0.1.253/langroid/parsing/document_parser.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2000 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/parsing/para_sentence_split.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4230 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/parsing/parse_json.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    10743 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/parsing/parser.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    29361 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/parsing/repo_loader.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     8846 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/parsing/search.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     3233 2024-05-27 22:58:25.000000 langroid-slim-0.1.253/langroid/parsing/spider.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     3410 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/parsing/table_loader.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4514 2024-05-27 22:54:19.000000 langroid-slim-0.1.253/langroid/parsing/url_loader.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     7977 2024-05-27 22:54:25.000000 langroid-slim-0.1.253/langroid/parsing/urls.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    12746 2024-05-27 22:55:23.000000 langroid-slim-0.1.253/langroid/parsing/utils.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4805 2024-05-27 22:57:48.000000 langroid-slim-0.1.253/langroid/parsing/web_search.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:20:15.928593 langroid-slim-0.1.253/langroid/prompts/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      185 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/prompts/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      331 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/prompts/dialog.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      131 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/prompts/prompts_config.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     6314 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/prompts/templates.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2706 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/prompts/transforms.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:20:15.933593 langroid-slim-0.1.253/langroid/utils/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      300 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/utils/__init__.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:20:15.934593 langroid-slim-0.1.253/langroid/utils/algorithms/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)       41 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/utils/algorithms/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2866 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/utils/algorithms/graph.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     3201 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/utils/configuration.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      563 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/utils/constants.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1343 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/utils/globals.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     3917 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/utils/logging.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:20:15.934593 langroid-slim-0.1.253/langroid/utils/output/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      341 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/utils/output/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     2872 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/utils/output/printing.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1049 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/utils/output/status.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      755 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/utils/pandas_utils.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    21728 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/utils/pydantic_utils.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4546 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/utils/system.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:20:15.937593 langroid-slim-0.1.253/langroid/vector_store/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      839 2024-05-27 23:03:10.000000 langroid-slim-0.1.253/langroid/vector_store/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    13469 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/vector_store/base.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     8109 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/vector_store/chromadb.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    18537 2024-05-27 22:32:47.000000 langroid-slim-0.1.253/langroid/vector_store/lancedb.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    11369 2024-05-27 23:02:32.000000 langroid-slim-0.1.253/langroid/vector_store/meilisearch.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    10045 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/vector_store/momento.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)    16802 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/langroid/vector_store/qdrantdb.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:20:15.938593 langroid-slim-0.1.253/langroid_slim.egg-info/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      279 2024-05-27 23:20:15.000000 langroid-slim-0.1.253/langroid_slim.egg-info/PKG-INFO
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     4184 2024-05-27 23:20:15.000000 langroid-slim-0.1.253/langroid_slim.egg-info/SOURCES.txt
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)        1 2024-05-27 23:20:15.000000 langroid-slim-0.1.253/langroid_slim.egg-info/dependency_links.txt
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      839 2024-05-27 23:20:15.000000 langroid-slim-0.1.253/langroid_slim.egg-info/requires.txt
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)       15 2024-05-27 23:20:15.000000 langroid-slim-0.1.253/langroid_slim.egg-info/top_level.txt
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     5649 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/pyproject.toml
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)      138 2024-05-27 23:20:15.941594 langroid-slim-0.1.253/setup.cfg
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1858 2024-05-27 23:20:11.000000 langroid-slim-0.1.253/setup.py
+drwxr-xr-x   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 23:20:15.939593 langroid-slim-0.1.253/tests/
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)        0 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/tests/__init__.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1930 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/tests/conftest.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1851 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/tests/test_pdf_parser_extra.py
+-rw-r--r--   0 jackywong  (1001) jackywong  (1001)     1087 2024-05-27 22:27:16.000000 langroid-slim-0.1.253/tests/utils.py
```

### Comparing `langroid-slim-0.1.252/LICENSE` & `langroid-slim-0.1.253/LICENSE`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/README.md` & `langroid-slim-0.1.253/README.md`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/__init__.py` & `langroid-slim-0.1.253/langroid/__init__.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/__init__.py` & `langroid-slim-0.1.253/langroid/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/base.py` & `langroid-slim-0.1.253/langroid/agent/base.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/batch.py` & `langroid-slim-0.1.253/langroid/agent/batch.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/callbacks/chainlit.py` & `langroid-slim-0.1.253/langroid/agent/callbacks/chainlit.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/chat_agent.py` & `langroid-slim-0.1.253/langroid/agent/chat_agent.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/chat_document.py` & `langroid-slim-0.1.253/langroid/agent/chat_document.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/openai_assistant.py` & `langroid-slim-0.1.253/langroid/agent/openai_assistant.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/special/__init__.py` & `langroid-slim-0.1.253/langroid/agent/special/__init__.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/special/doc_chat_agent.py` & `langroid-slim-0.1.253/langroid/agent/special/doc_chat_agent.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/special/lance_doc_chat_agent.py` & `langroid-slim-0.1.253/langroid/agent/special/lance_doc_chat_agent.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/special/lance_rag/critic_agent.py` & `langroid-slim-0.1.253/langroid/agent/special/lance_rag/critic_agent.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/special/lance_rag/lance_rag_task.py` & `langroid-slim-0.1.253/langroid/agent/special/lance_rag/lance_rag_task.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/special/lance_rag/query_planner_agent.py` & `langroid-slim-0.1.253/langroid/agent/special/lance_rag/query_planner_agent.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/special/lance_tools.py` & `langroid-slim-0.1.253/langroid/agent/special/lance_tools.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/special/neo4j/csv_kg_chat.py` & `langroid-slim-0.1.253/langroid/agent/special/neo4j/csv_kg_chat.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/special/neo4j/neo4j_chat_agent.py` & `langroid-slim-0.1.253/langroid/agent/special/neo4j/neo4j_chat_agent.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/special/neo4j/utils/system_message.py` & `langroid-slim-0.1.253/langroid/agent/special/neo4j/utils/system_message.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/special/relevance_extractor_agent.py` & `langroid-slim-0.1.253/langroid/agent/special/relevance_extractor_agent.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/special/retriever_agent.py` & `langroid-slim-0.1.253/langroid/agent/special/retriever_agent.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/special/sql/sql_chat_agent.py` & `langroid-slim-0.1.253/langroid/agent/special/sql/sql_chat_agent.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/special/sql/utils/description_extractors.py` & `langroid-slim-0.1.253/langroid/agent/special/sql/utils/description_extractors.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/special/sql/utils/populate_metadata.py` & `langroid-slim-0.1.253/langroid/agent/special/sql/utils/populate_metadata.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/special/sql/utils/system_message.py` & `langroid-slim-0.1.253/langroid/agent/special/sql/utils/system_message.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/special/sql/utils/tools.py` & `langroid-slim-0.1.253/langroid/agent/special/sql/utils/tools.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/special/table_chat_agent.py` & `langroid-slim-0.1.253/langroid/agent/special/table_chat_agent.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/task.py` & `langroid-slim-0.1.253/langroid/agent/task.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/tool_message.py` & `langroid-slim-0.1.253/langroid/agent/tool_message.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/tools/duckduckgo_search_tool.py` & `langroid-slim-0.1.253/langroid/agent/tools/duckduckgo_search_tool.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/tools/google_search_tool.py` & `langroid-slim-0.1.253/langroid/agent/tools/google_search_tool.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/tools/metaphor_search_tool.py` & `langroid-slim-0.1.253/langroid/agent/tools/metaphor_search_tool.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/tools/recipient_tool.py` & `langroid-slim-0.1.253/langroid/agent/tools/recipient_tool.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/tools/retrieval_tool.py` & `langroid-slim-0.1.253/langroid/agent/tools/retrieval_tool.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/agent/tools/segment_extract_tool.py` & `langroid-slim-0.1.253/langroid/agent/tools/segment_extract_tool.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/cachedb/base.py` & `langroid-slim-0.1.253/langroid/cachedb/base.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/cachedb/momento_cachedb.py` & `langroid-slim-0.1.253/langroid/cachedb/momento_cachedb.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/cachedb/redis_cachedb.py` & `langroid-slim-0.1.253/langroid/cachedb/redis_cachedb.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/embedding_models/__init__.py` & `langroid-slim-0.1.253/langroid/embedding_models/__init__.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/embedding_models/base.py` & `langroid-slim-0.1.253/langroid/embedding_models/base.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/embedding_models/models.py` & `langroid-slim-0.1.253/langroid/embedding_models/models.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/embedding_models/protoc/embeddings_pb2.py` & `langroid-slim-0.1.253/langroid/embedding_models/protoc/embeddings_pb2.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/embedding_models/protoc/embeddings_pb2.pyi` & `langroid-slim-0.1.253/langroid/embedding_models/protoc/embeddings_pb2.pyi`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/embedding_models/protoc/embeddings_pb2_grpc.py` & `langroid-slim-0.1.253/langroid/embedding_models/protoc/embeddings_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/embedding_models/remote_embeds.py` & `langroid-slim-0.1.253/langroid/embedding_models/remote_embeds.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/language_models/__init__.py` & `langroid-slim-0.1.253/langroid/language_models/__init__.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/language_models/azure_openai.py` & `langroid-slim-0.1.253/langroid/language_models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/language_models/base.py` & `langroid-slim-0.1.253/langroid/language_models/base.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/language_models/openai_gpt.py` & `langroid-slim-0.1.253/langroid/language_models/openai_gpt.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/language_models/prompt_formatter/base.py` & `langroid-slim-0.1.253/langroid/language_models/prompt_formatter/base.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/language_models/prompt_formatter/hf_formatter.py` & `langroid-slim-0.1.253/langroid/language_models/prompt_formatter/hf_formatter.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/language_models/prompt_formatter/llama2_formatter.py` & `langroid-slim-0.1.253/langroid/language_models/prompt_formatter/llama2_formatter.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/language_models/utils.py` & `langroid-slim-0.1.253/langroid/language_models/utils.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/mytypes.py` & `langroid-slim-0.1.253/langroid/mytypes.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/parsing/__init__.py` & `langroid-slim-0.1.253/langroid/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/parsing/agent_chats.py` & `langroid-slim-0.1.253/langroid/parsing/agent_chats.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/parsing/code_parser.py` & `langroid-slim-0.1.253/langroid/parsing/code_parser.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/parsing/document_parser.py` & `langroid-slim-0.1.253/langroid/parsing/document_parser.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/parsing/para_sentence_split.py` & `langroid-slim-0.1.253/langroid/parsing/para_sentence_split.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/parsing/parse_json.py` & `langroid-slim-0.1.253/langroid/parsing/parse_json.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/parsing/parser.py` & `langroid-slim-0.1.253/langroid/parsing/parser.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/parsing/repo_loader.py` & `langroid-slim-0.1.253/langroid/parsing/repo_loader.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/parsing/search.py` & `langroid-slim-0.1.253/langroid/parsing/search.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/parsing/spider.py` & `langroid-slim-0.1.253/langroid/parsing/spider.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/parsing/table_loader.py` & `langroid-slim-0.1.253/langroid/parsing/table_loader.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/parsing/url_loader.py` & `langroid-slim-0.1.253/langroid/parsing/url_loader.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/parsing/urls.py` & `langroid-slim-0.1.253/langroid/parsing/urls.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/parsing/utils.py` & `langroid-slim-0.1.253/langroid/parsing/utils.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/parsing/web_search.py` & `langroid-slim-0.1.253/langroid/parsing/web_search.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/prompts/templates.py` & `langroid-slim-0.1.253/langroid/prompts/templates.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/prompts/transforms.py` & `langroid-slim-0.1.253/langroid/prompts/transforms.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/utils/algorithms/graph.py` & `langroid-slim-0.1.253/langroid/utils/algorithms/graph.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/utils/configuration.py` & `langroid-slim-0.1.253/langroid/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/utils/constants.py` & `langroid-slim-0.1.253/langroid/utils/constants.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/utils/globals.py` & `langroid-slim-0.1.253/langroid/utils/globals.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/utils/logging.py` & `langroid-slim-0.1.253/langroid/utils/logging.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/utils/output/printing.py` & `langroid-slim-0.1.253/langroid/utils/output/printing.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/utils/output/status.py` & `langroid-slim-0.1.253/langroid/utils/output/status.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/utils/pandas_utils.py` & `langroid-slim-0.1.253/langroid/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/utils/pydantic_utils.py` & `langroid-slim-0.1.253/langroid/utils/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/utils/system.py` & `langroid-slim-0.1.253/langroid/utils/system.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/vector_store/__init__.py` & `langroid-slim-0.1.253/langroid/vector_store/__init__.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/vector_store/base.py` & `langroid-slim-0.1.253/langroid/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/vector_store/chromadb.py` & `langroid-slim-0.1.253/langroid/vector_store/chromadb.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/vector_store/lancedb.py` & `langroid-slim-0.1.253/langroid/vector_store/lancedb.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/vector_store/meilisearch.py` & `langroid-slim-0.1.253/langroid/vector_store/meilisearch.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/vector_store/momento.py` & `langroid-slim-0.1.253/langroid/vector_store/momento.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid/vector_store/qdrantdb.py` & `langroid-slim-0.1.253/langroid/vector_store/qdrantdb.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid_slim.egg-info/SOURCES.txt` & `langroid-slim-0.1.253/langroid_slim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/langroid_slim.egg-info/requires.txt` & `langroid-slim-0.1.253/langroid_slim.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/pyproject.toml` & `langroid-slim-0.1.253/pyproject.toml`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/setup.py` & `langroid-slim-0.1.253/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """A minimal setup.py for Langroid
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name="langroid-slim",
-    version="0.1.252",
+    version="0.1.253",
     description="Harness LLMs with Multi-Agent Programming",
     author="Prasad Chalasani",
     author_email="pchalasani@gmail.com",
     license="MIT",
     packages=find_packages(),
     install_requires=[
         "onnxruntime==1.16.1",
```

### Comparing `langroid-slim-0.1.252/tests/conftest.py` & `langroid-slim-0.1.253/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/tests/test_pdf_parser_extra.py` & `langroid-slim-0.1.253/tests/test_pdf_parser_extra.py`

 * *Files identical despite different names*

### Comparing `langroid-slim-0.1.252/tests/utils.py` & `langroid-slim-0.1.253/tests/utils.py`

 * *Files identical despite different names*

