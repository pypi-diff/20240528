# Comparing `tmp/camel_ai-0.1.3.tar.gz` & `tmp/camel_ai-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camel_ai-0.1.3.tar", max compression
+gzip compressed data, was "camel_ai-0.1.4.tar", max compression
```

## Comparing `camel_ai-0.1.3.tar` & `camel_ai-0.1.4.tar`

### file list

```diff
@@ -1,101 +1,119 @@
--rw-r--r--   0        0        0    17382 2024-04-30 23:45:40.883950 camel_ai-0.1.3/README.md
--rw-r--r--   0        0        0      778 2024-04-30 23:45:40.883950 camel_ai-0.1.3/camel/__init__.py
--rw-r--r--   0        0        0     1412 2024-04-30 23:45:40.883950 camel_ai-0.1.3/camel/agents/__init__.py
--rw-r--r--   0        0        0     1130 2024-04-30 23:45:40.883950 camel_ai-0.1.3/camel/agents/base.py
--rw-r--r--   0        0        0    22379 2024-04-30 23:45:40.883950 camel_ai-0.1.3/camel/agents/chat_agent.py
--rw-r--r--   0        0        0     7377 2024-04-30 23:45:40.883950 camel_ai-0.1.3/camel/agents/critic_agent.py
--rw-r--r--   0        0        0    13050 2024-04-30 23:45:40.883950 camel_ai-0.1.3/camel/agents/deductive_reasoner_agent.py
--rw-r--r--   0        0        0     7322 2024-04-30 23:45:40.883950 camel_ai-0.1.3/camel/agents/embodied_agent.py
--rw-r--r--   0        0        0     4879 2024-04-30 23:45:40.883950 camel_ai-0.1.3/camel/agents/role_assignment_agent.py
--rw-r--r--   0        0        0    14907 2024-04-30 23:45:40.883950 camel_ai-0.1.3/camel/agents/task_agent.py
--rw-r--r--   0        0        0      862 2024-04-30 23:45:40.883950 camel_ai-0.1.3/camel/agents/tool_agents/__init__.py
--rw-r--r--   0        0        0     1399 2024-04-30 23:45:40.883950 camel_ai-0.1.3/camel/agents/tool_agents/base.py
--rw-r--r--   0        0        0     8723 2024-04-30 23:45:40.883950 camel_ai-0.1.3/camel/agents/tool_agents/hugging_face_tool_agent.py
--rw-r--r--   0        0        0    12684 2024-04-30 23:45:40.883950 camel_ai-0.1.3/camel/configs.py
--rw-r--r--   0        0        0      952 2024-04-30 23:45:40.883950 camel_ai-0.1.3/camel/embeddings/__init__.py
--rw-r--r--   0        0        0     2208 2024-04-30 23:45:40.883950 camel_ai-0.1.3/camel/embeddings/base.py
--rw-r--r--   0        0        0     2574 2024-04-30 23:45:40.883950 camel_ai-0.1.3/camel/embeddings/openai_embedding.py
--rw-r--r--   0        0        0     2312 2024-04-30 23:45:40.883950 camel_ai-0.1.3/camel/embeddings/sentence_transformers_embeddings.py
--rw-r--r--   0        0        0     1310 2024-04-30 23:45:40.883950 camel_ai-0.1.3/camel/functions/__init__.py
--rw-r--r--   0        0        0    12468 2024-04-30 23:45:40.883950 camel_ai-0.1.3/camel/functions/google_maps_function.py
--rw-r--r--   0        0        0     1703 2024-04-30 23:45:40.883950 camel_ai-0.1.3/camel/functions/math_functions.py
--rw-r--r--   0        0        0    14873 2024-04-30 23:45:40.883950 camel_ai-0.1.3/camel/functions/openai_function.py
--rw-r--r--   0        0        0    12639 2024-04-30 23:45:40.883950 camel_ai-0.1.3/camel/functions/search_functions.py
--rw-r--r--   0        0        0    17254 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/functions/twitter_function.py
--rw-r--r--   0        0        0     5881 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/functions/weather_functions.py
--rw-r--r--   0        0        0    10437 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/generators.py
--rw-r--r--   0        0        0     4949 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/human.py
--rw-r--r--   0        0        0     1040 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/interpreters/__init__.py
--rw-r--r--   0        0        0     1904 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/interpreters/base.py
--rw-r--r--   0        0        0    21866 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/interpreters/internal_python_interpreter.py
--rw-r--r--   0        0        0      886 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/interpreters/interpreter_error.py
--rw-r--r--   0        0        0     6835 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/interpreters/subprocess_interpreter.py
--rw-r--r--   0        0        0      856 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/loaders/__init__.py
--rw-r--r--   0        0        0     8664 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/loaders/base_io.py
--rw-r--r--   0        0        0    25870 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/loaders/unstructured_io.py
--rw-r--r--   0        0        0     1364 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/memories/__init__.py
--rw-r--r--   0        0        0     6110 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/memories/agent_memories.py
--rw-r--r--   0        0        0     5003 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/memories/base.py
--rw-r--r--   0        0        0      860 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/memories/blocks/__init__.py
--rw-r--r--   0        0        0     4609 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/memories/blocks/chat_history_block.py
--rw-r--r--   0        0        0     3850 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/memories/blocks/vectordb_block.py
--rw-r--r--   0        0        0      806 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/memories/context_creators/__init__.py
--rw-r--r--   0        0        0     5378 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/memories/context_creators/score_based.py
--rw-r--r--   0        0        0     3618 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/memories/records.py
--rw-r--r--   0        0        0     1468 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/messages/__init__.py
--rw-r--r--   0        0        0    10131 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/messages/base.py
--rw-r--r--   0        0        0     3841 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/messages/func_message.py
--rw-r--r--   0        0        0     1092 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/models/__init__.py
--rw-r--r--   0        0        0     4552 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/models/anthropic_model.py
--rw-r--r--   0        0        0     3700 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/models/base_model.py
--rw-r--r--   0        0        0     2245 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/models/model_factory.py
--rw-r--r--   0        0        0     5856 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/models/open_source_model.py
--rw-r--r--   0        0        0     3893 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/models/openai_model.py
--rw-r--r--   0        0        0     3543 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/models/stub_model.py
--rw-r--r--   0        0        0     1790 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/prompts/__init__.py
--rw-r--r--   0        0        0     6306 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/prompts/ai_society.py
--rw-r--r--   0        0        0     8452 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/prompts/base.py
--rw-r--r--   0        0        0     5865 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/prompts/code.py
--rw-r--r--   0        0        0     1596 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/prompts/evaluation.py
--rw-r--r--   0        0        0     4537 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/prompts/misalignment.py
--rw-r--r--   0        0        0     1422 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/prompts/object_recognition.py
--rw-r--r--   0        0        0     4134 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/prompts/prompt_templates.py
--rw-r--r--   0        0        0     2544 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/prompts/role_description_prompt_template.py
--rw-r--r--   0        0        0     2109 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/prompts/solution_extraction.py
--rw-r--r--   0        0        0     2590 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/prompts/task_prompt_template.py
--rw-r--r--   0        0        0     1902 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/prompts/translation.py
--rw-r--r--   0        0        0      795 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/responses/__init__.py
--rw-r--r--   0        0        0     1714 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/responses/agent_responses.py
--rw-r--r--   0        0        0      971 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/retrievers/__init__.py
--rw-r--r--   0        0        0    12600 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/retrievers/auto_retriever.py
--rw-r--r--   0        0        0     2382 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/retrievers/base.py
--rw-r--r--   0        0        0     5404 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/retrievers/bm25_retriever.py
--rw-r--r--   0        0        0     6643 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/retrievers/vector_retriever.py
--rw-r--r--   0        0        0      832 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/societies/__init__.py
--rw-r--r--   0        0        0    11770 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/societies/babyagi_playing.py
--rw-r--r--   0        0        0    22079 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/societies/role_playing.py
--rw-r--r--   0        0        0     1480 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/storages/__init__.py
--rw-r--r--   0        0        0      897 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/storages/graph_storages/__init__.py
--rw-r--r--   0        0        0     2857 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/storages/graph_storages/base.py
--rw-r--r--   0        0        0     2356 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/storages/graph_storages/graph_element.py
--rw-r--r--   0        0        0    22055 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/storages/graph_storages/neo4j_graph.py
--rw-r--r--   0        0        0      916 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/storages/key_value_storages/__init__.py
--rw-r--r--   0        0        0     2183 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/storages/key_value_storages/base.py
--rw-r--r--   0        0        0     1955 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/storages/key_value_storages/in_memory.py
--rw-r--r--   0        0        0     3471 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/storages/key_value_storages/json.py
--rw-r--r--   0        0        0     1076 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/storages/vectordb_storages/__init__.py
--rw-r--r--   0        0        0     6001 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/storages/vectordb_storages/base.py
--rw-r--r--   0        0        0    13589 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/storages/vectordb_storages/milvus.py
--rw-r--r--   0        0        0    13480 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/storages/vectordb_storages/qdrant.py
--rw-r--r--   0        0        0      997 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/terminators/__init__.py
--rw-r--r--   0        0        0     1396 2024-04-30 23:45:40.887950 camel_ai-0.1.3/camel/terminators/base.py
--rw-r--r--   0        0        0     4951 2024-04-30 23:45:40.891950 camel_ai-0.1.3/camel/terminators/response_terminator.py
--rw-r--r--   0        0        0     2087 2024-04-30 23:45:40.891950 camel_ai-0.1.3/camel/terminators/token_limit_terminator.py
--rw-r--r--   0        0        0     1792 2024-04-30 23:45:40.891950 camel_ai-0.1.3/camel/types/__init__.py
--rw-r--r--   0        0        0     7446 2024-04-30 23:45:40.891950 camel_ai-0.1.3/camel/types/enums.py
--rw-r--r--   0        0        0     2045 2024-04-30 23:45:40.891950 camel_ai-0.1.3/camel/types/openai_types.py
--rw-r--r--   0        0        0     1578 2024-04-30 23:45:40.891950 camel_ai-0.1.3/camel/utils/__init__.py
--rw-r--r--   0        0        0    12891 2024-04-30 23:45:40.891950 camel_ai-0.1.3/camel/utils/commons.py
--rw-r--r--   0        0        0    12674 2024-04-30 23:45:40.891950 camel_ai-0.1.3/camel/utils/token_counting.py
--rw-r--r--   0        0        0     5593 2024-04-30 23:45:40.899950 camel_ai-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    20689 1970-01-01 00:00:00.000000 camel_ai-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    17382 2024-05-28 12:37:14.418125 camel_ai-0.1.4/README.md
+-rw-r--r--   0        0        0      778 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/__init__.py
+-rw-r--r--   0        0        0     1494 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/agents/__init__.py
+-rw-r--r--   0        0        0     1130 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/agents/base.py
+-rw-r--r--   0        0        0    21701 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/agents/chat_agent.py
+-rw-r--r--   0        0        0     7377 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/agents/critic_agent.py
+-rw-r--r--   0        0        0    13050 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/agents/deductive_reasoner_agent.py
+-rw-r--r--   0        0        0     7322 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/agents/embodied_agent.py
+-rw-r--r--   0        0        0     8783 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/agents/knowledge_graph_agent.py
+-rw-r--r--   0        0        0     4879 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/agents/role_assignment_agent.py
+-rw-r--r--   0        0        0    14907 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/agents/task_agent.py
+-rw-r--r--   0        0        0      862 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/agents/tool_agents/__init__.py
+-rw-r--r--   0        0        0     1399 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/agents/tool_agents/base.py
+-rw-r--r--   0        0        0     8723 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/agents/tool_agents/hugging_face_tool_agent.py
+-rw-r--r--   0        0        0     1061 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/configs/__init__.py
+-rw-r--r--   0        0        0     3315 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/configs/anthropic_config.py
+-rw-r--r--   0        0        0      870 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/configs/base_config.py
+-rw-r--r--   0        0        0     6603 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/configs/openai_config.py
+-rw-r--r--   0        0        0      952 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/embeddings/__init__.py
+-rw-r--r--   0        0        0     2208 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/embeddings/base.py
+-rw-r--r--   0        0        0     2873 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/embeddings/openai_embedding.py
+-rw-r--r--   0        0        0     2312 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/embeddings/sentence_transformers_embeddings.py
+-rw-r--r--   0        0        0     1452 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/functions/__init__.py
+-rw-r--r--   0        0        0    12468 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/functions/google_maps_function.py
+-rw-r--r--   0        0        0     1703 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/functions/math_functions.py
+-rw-r--r--   0        0        0    15036 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/functions/open_api_function.py
+-rw-r--r--   0        0        0      708 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/functions/open_api_specs/coursera/__init__.py
+-rw-r--r--   0        0        0     1981 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/functions/open_api_specs/coursera/openapi.yaml
+-rw-r--r--   0        0        0      708 2024-05-28 12:37:14.418125 camel_ai-0.1.4/camel/functions/open_api_specs/klarna/__init__.py
+-rw-r--r--   0        0        0     2887 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/functions/open_api_specs/klarna/openapi.yaml
+-rw-r--r--   0        0        0      708 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/functions/open_api_specs/speak/__init__.py
+-rw-r--r--   0        0        0     6557 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/functions/open_api_specs/speak/openapi.yaml
+-rw-r--r--   0        0        0    14933 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/functions/openai_function.py
+-rw-r--r--   0        0        0     2281 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/functions/retrieval_functions.py
+-rw-r--r--   0        0        0    12639 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/functions/search_functions.py
+-rw-r--r--   0        0        0     8789 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/functions/slack_functions.py
+-rw-r--r--   0        0        0    17254 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/functions/twitter_function.py
+-rw-r--r--   0        0        0     5881 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/functions/weather_functions.py
+-rw-r--r--   0        0        0    10437 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/generators.py
+-rw-r--r--   0        0        0     4949 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/human.py
+-rw-r--r--   0        0        0     1040 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/interpreters/__init__.py
+-rw-r--r--   0        0        0     1904 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/interpreters/base.py
+-rw-r--r--   0        0        0    21866 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/interpreters/internal_python_interpreter.py
+-rw-r--r--   0        0        0      886 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/interpreters/interpreter_error.py
+-rw-r--r--   0        0        0     6835 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/interpreters/subprocess_interpreter.py
+-rw-r--r--   0        0        0      856 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/loaders/__init__.py
+-rw-r--r--   0        0        0     8664 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/loaders/base_io.py
+-rw-r--r--   0        0        0    25870 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/loaders/unstructured_io.py
+-rw-r--r--   0        0        0     1364 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/memories/__init__.py
+-rw-r--r--   0        0        0     6110 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/memories/agent_memories.py
+-rw-r--r--   0        0        0     5003 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/memories/base.py
+-rw-r--r--   0        0        0      860 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/memories/blocks/__init__.py
+-rw-r--r--   0        0        0     4609 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/memories/blocks/chat_history_block.py
+-rw-r--r--   0        0        0     3850 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/memories/blocks/vectordb_block.py
+-rw-r--r--   0        0        0      806 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/memories/context_creators/__init__.py
+-rw-r--r--   0        0        0     5378 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/memories/context_creators/score_based.py
+-rw-r--r--   0        0        0     3618 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/memories/records.py
+-rw-r--r--   0        0        0     1468 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/messages/__init__.py
+-rw-r--r--   0        0        0    10131 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/messages/base.py
+-rw-r--r--   0        0        0     3841 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/messages/func_message.py
+-rw-r--r--   0        0        0     1168 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/models/__init__.py
+-rw-r--r--   0        0        0     5112 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/models/anthropic_model.py
+-rw-r--r--   0        0        0     3904 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/models/base_model.py
+-rw-r--r--   0        0        0     2418 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/models/model_factory.py
+-rw-r--r--   0        0        0     5856 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/models/open_source_model.py
+-rw-r--r--   0        0        0     9799 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/models/openai_audio_models.py
+-rw-r--r--   0        0        0     4164 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/models/openai_model.py
+-rw-r--r--   0        0        0     3631 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/models/stub_model.py
+-rw-r--r--   0        0        0     1790 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/prompts/__init__.py
+-rw-r--r--   0        0        0     6306 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/prompts/ai_society.py
+-rw-r--r--   0        0        0     8452 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/prompts/base.py
+-rw-r--r--   0        0        0     5865 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/prompts/code.py
+-rw-r--r--   0        0        0     1596 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/prompts/evaluation.py
+-rw-r--r--   0        0        0     4537 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/prompts/misalignment.py
+-rw-r--r--   0        0        0     1422 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/prompts/object_recognition.py
+-rw-r--r--   0        0        0     4134 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/prompts/prompt_templates.py
+-rw-r--r--   0        0        0     2544 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/prompts/role_description_prompt_template.py
+-rw-r--r--   0        0        0     2109 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/prompts/solution_extraction.py
+-rw-r--r--   0        0        0     2590 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/prompts/task_prompt_template.py
+-rw-r--r--   0        0        0     1902 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/prompts/translation.py
+-rw-r--r--   0        0        0      795 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/responses/__init__.py
+-rw-r--r--   0        0        0     1714 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/responses/agent_responses.py
+-rw-r--r--   0        0        0     1059 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/retrievers/__init__.py
+-rw-r--r--   0        0        0    13364 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/retrievers/auto_retriever.py
+-rw-r--r--   0        0        0     2624 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/retrievers/base.py
+-rw-r--r--   0        0        0     5180 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/retrievers/bm25_retriever.py
+-rw-r--r--   0        0        0     4123 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/retrievers/cohere_rerank_retriever.py
+-rw-r--r--   0        0        0     7185 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/retrievers/vector_retriever.py
+-rw-r--r--   0        0        0      832 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/societies/__init__.py
+-rw-r--r--   0        0        0    11770 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/societies/babyagi_playing.py
+-rw-r--r--   0        0        0    22079 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/societies/role_playing.py
+-rw-r--r--   0        0        0     1480 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/storages/__init__.py
+-rw-r--r--   0        0        0      897 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/storages/graph_storages/__init__.py
+-rw-r--r--   0        0        0     2857 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/storages/graph_storages/base.py
+-rw-r--r--   0        0        0     2356 2024-05-28 12:37:14.422125 camel_ai-0.1.4/camel/storages/graph_storages/graph_element.py
+-rw-r--r--   0        0        0    22055 2024-05-28 12:37:14.426125 camel_ai-0.1.4/camel/storages/graph_storages/neo4j_graph.py
+-rw-r--r--   0        0        0      916 2024-05-28 12:37:14.426125 camel_ai-0.1.4/camel/storages/key_value_storages/__init__.py
+-rw-r--r--   0        0        0     2183 2024-05-28 12:37:14.426125 camel_ai-0.1.4/camel/storages/key_value_storages/base.py
+-rw-r--r--   0        0        0     1955 2024-05-28 12:37:14.426125 camel_ai-0.1.4/camel/storages/key_value_storages/in_memory.py
+-rw-r--r--   0        0        0     3471 2024-05-28 12:37:14.426125 camel_ai-0.1.4/camel/storages/key_value_storages/json.py
+-rw-r--r--   0        0        0     1076 2024-05-28 12:37:14.426125 camel_ai-0.1.4/camel/storages/vectordb_storages/__init__.py
+-rw-r--r--   0        0        0     6001 2024-05-28 12:37:14.426125 camel_ai-0.1.4/camel/storages/vectordb_storages/base.py
+-rw-r--r--   0        0        0    13589 2024-05-28 12:37:14.426125 camel_ai-0.1.4/camel/storages/vectordb_storages/milvus.py
+-rw-r--r--   0        0        0    13618 2024-05-28 12:37:14.426125 camel_ai-0.1.4/camel/storages/vectordb_storages/qdrant.py
+-rw-r--r--   0        0        0      997 2024-05-28 12:37:14.426125 camel_ai-0.1.4/camel/terminators/__init__.py
+-rw-r--r--   0        0        0     1396 2024-05-28 12:37:14.426125 camel_ai-0.1.4/camel/terminators/base.py
+-rw-r--r--   0        0        0     4951 2024-05-28 12:37:14.426125 camel_ai-0.1.4/camel/terminators/response_terminator.py
+-rw-r--r--   0        0        0     2087 2024-05-28 12:37:14.426125 camel_ai-0.1.4/camel/terminators/token_limit_terminator.py
+-rw-r--r--   0        0        0      836 2024-05-28 12:37:14.426125 camel_ai-0.1.4/camel/toolkits/__init__.py
+-rw-r--r--   0        0        0      923 2024-05-28 12:37:14.426125 camel_ai-0.1.4/camel/toolkits/base.py
+-rw-r--r--   0        0        0     8822 2024-05-28 12:37:14.426125 camel_ai-0.1.4/camel/toolkits/github_toolkit.py
+-rw-r--r--   0        0        0     1902 2024-05-28 12:37:14.426125 camel_ai-0.1.4/camel/types/__init__.py
+-rw-r--r--   0        0        0     8302 2024-05-28 12:37:14.426125 camel_ai-0.1.4/camel/types/enums.py
+-rw-r--r--   0        0        0     2045 2024-05-28 12:37:14.426125 camel_ai-0.1.4/camel/types/openai_types.py
+-rw-r--r--   0        0        0     1616 2024-05-28 12:37:14.426125 camel_ai-0.1.4/camel/utils/__init__.py
+-rw-r--r--   0        0        0     9930 2024-05-28 12:37:14.426125 camel_ai-0.1.4/camel/utils/commons.py
+-rw-r--r--   0        0        0    12674 2024-05-28 12:37:14.426125 camel_ai-0.1.4/camel/utils/token_counting.py
+-rw-r--r--   0        0        0     6244 2024-05-28 12:37:14.434125 camel_ai-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    21185 1970-01-01 00:00:00.000000 camel_ai-0.1.4/PKG-INFO
```

### Comparing `camel_ai-0.1.3/README.md` & `camel_ai-0.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 # Create a conda virtual environment
 conda create --name camel python=3.10
 
 # Activate camel conda environment
 conda activate camel
 
 # Clone github repo
-git clone -b v0.1.3 https://github.com/camel-ai/camel.git
+git clone -b v0.1.4 https://github.com/camel-ai/camel.git
 
 # Change directory into project directory
 cd camel
 
 # Install camel from source
 pip install -e .
```

#### html2text {}

```diff
@@ -55,15 +55,15 @@
 github.com/camel-ai/camel.git # Change directory into project directory cd
 camel # Activate camel virtual environment poetry shell # Install camel from
 source # It takes about 90 seconds to resolve dependencies poetry install # Or
 if you want to use all other extra packages poetry install -E all # (Optional)
 # Exit the virtual environment exit ``` Install `CAMEL` from source with conda
 and pip: ```sh # Create a conda virtual environment conda create --name camel
 python=3.10 # Activate camel conda environment conda activate camel # Clone
-github repo git clone -b v0.1.3 https://github.com/camel-ai/camel.git # Change
+github repo git clone -b v0.1.4 https://github.com/camel-ai/camel.git # Change
 directory into project directory cd camel # Install camel from source pip
 install -e . # Or if you want to use all other extra packages pip install -e .
 [all] # (Optional) ``` ## Documentation [CAMEL package documentation pages]
 (https://camel-ai.github.io/camel/). ## Example You can find a list of tasks
 for different sets of assistant and user role pairs [here](https://
 drive.google.com/file/d/194PPaSTBR07m-PzjS-Ty6KlPLdFIPQDd/view?usp=share_link).
 As an example, to run the `role_playing.py` script: First, you need to add your
```

### Comparing `camel_ai-0.1.3/camel/__init__.py` & `camel_ai-0.1.4/camel/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
 
-__version__ = '0.1.3'
+__version__ = '0.1.4'
 
 __all__ = [
     '__version__',
     'camel',
 ]
```

### Comparing `camel_ai-0.1.3/camel/agents/__init__.py` & `camel_ai-0.1.4/camel/agents/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
 from .base import BaseAgent
 from .chat_agent import ChatAgent
 from .critic_agent import CriticAgent
 from .embodied_agent import EmbodiedAgent
+from .knowledge_graph_agent import KnowledgeGraphAgent
 from .role_assignment_agent import RoleAssignmentAgent
 from .task_agent import (
     TaskCreationAgent,
     TaskPlannerAgent,
     TaskPrioritizationAgent,
     TaskSpecifyAgent,
 )
@@ -33,8 +34,9 @@
     'TaskCreationAgent',
     'TaskPrioritizationAgent',
     'CriticAgent',
     'BaseToolAgent',
     'HuggingFaceToolAgent',
     'EmbodiedAgent',
     'RoleAssignmentAgent',
+    'KnowledgeGraphAgent',
 ]
```

### Comparing `camel_ai-0.1.3/camel/agents/base.py` & `camel_ai-0.1.4/camel/agents/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/agents/chat_agent.py` & `camel_ai-0.1.4/camel/agents/chat_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import json
 from collections import defaultdict
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple
 
 from camel.agents.base import BaseAgent
-from camel.configs import ChatGPTConfig, ChatGPTVisionConfig
+from camel.configs import ChatGPTConfig
 from camel.memories import (
     AgentMemory,
     ChatHistoryMemory,
     MemoryRecord,
     ScoreBasedContextCreator,
 )
 from camel.messages import BaseMessage, FunctionCallingMessage, OpenAIMessage
@@ -80,43 +80,47 @@
 
     Args:
         system_message (BaseMessage): The system message for the chat agent.
         model_type (ModelType, optional): The LLM model to use for generating
             responses. (default :obj:`ModelType.GPT_3_5_TURBO`)
         model_config (BaseConfig, optional): Configuration options for the
             LLM model. (default: :obj:`None`)
+        api_key (str, optional): The API key for authenticating with the
+            LLM service. Only OpenAI and Anthropic model supported (default:
+            :obj:`None`)
         memory (AgentMemory, optional): The agent memory for managing chat
             messages. If `None`, a :obj:`ChatHistoryMemory` will be used.
             (default: :obj:`None`)
         message_window_size (int, optional): The maximum number of previous
             messages to include in the context window. If `None`, no windowing
             is performed. (default: :obj:`None`)
         token_limit (int, optional): The maximum number of tokens in a context.
             The context will be automatically pruned to fulfill the limitation.
             If `None`, it will be set according to the backend model.
             (default: :obj:`None`)
         output_language (str, optional): The language to be output by the
             agent. (default: :obj:`None`)
-        function_list (List[OpenAIFunction], optional): List of available
+        tools (List[OpenAIFunction], optional): List of available
             :obj:`OpenAIFunction`. (default: :obj:`None`)
         response_terminators (List[ResponseTerminator], optional): List of
             :obj:`ResponseTerminator` bind to one chat agent.
             (default: :obj:`None`)
     """
 
     def __init__(
         self,
         system_message: BaseMessage,
         model_type: Optional[ModelType] = None,
         model_config: Optional[BaseConfig] = None,
+        api_key: Optional[str] = None,
         memory: Optional[AgentMemory] = None,
         message_window_size: Optional[int] = None,
         token_limit: Optional[int] = None,
         output_language: Optional[str] = None,
-        function_list: Optional[List[OpenAIFunction]] = None,
+        tools: Optional[List[OpenAIFunction]] = None,
         response_terminators: Optional[List[ResponseTerminator]] = None,
     ) -> None:
         self.orig_sys_message: BaseMessage = system_message
         self.system_message = system_message
         self.role_name: str = system_message.role_name
         self.role_type: RoleType = system_message.role_type
         self.output_language: Optional[str] = output_language
@@ -124,42 +128,22 @@
             self.set_output_language(self.output_language)
 
         self.model_type: ModelType = (
             model_type if model_type is not None else ModelType.GPT_3_5_TURBO
         )
 
         self.func_dict: Dict[str, Callable] = {}
-        if function_list is not None:
-            for func in function_list:
+        if tools is not None:
+            for func in tools:
                 self.func_dict[func.get_function_name()] = func.func
 
-        self.model_config: BaseConfig
-        if self.model_type == ModelType.GPT_4_TURBO_VISION:
-            if model_config is not None and not isinstance(
-                model_config, ChatGPTVisionConfig
-            ):
-                raise ValueError(
-                    "Please use `ChatGPTVisionConfig` as "
-                    "the `model_config` when `model_type` "
-                    "is `GPT_4_TURBO_VISION`"
-                )
-            self.model_config = model_config or ChatGPTVisionConfig()
-        else:
-            if model_config is not None and isinstance(
-                model_config, ChatGPTVisionConfig
-            ):
-                raise ValueError(
-                    "Please don't use `ChatGPTVisionConfig` as "
-                    "the `model_config` when `model_type` "
-                    "is not `GPT_4_TURBO_VISION`"
-                )
-            self.model_config = model_config or ChatGPTConfig()
-
+        self.model_config = model_config or ChatGPTConfig()
+        self._api_key = api_key
         self.model_backend: BaseModelBackend = ModelFactory.create(
-            self.model_type, self.model_config.__dict__
+            self.model_type, self.model_config.__dict__, self._api_key
         )
         self.model_token_limit = token_limit or self.model_backend.token_limit
         context_creator = ScoreBasedContextCreator(
             self.model_backend.token_counter,
             self.model_token_limit,
         )
         self.memory: AgentMemory = memory or ChatHistoryMemory(
@@ -197,20 +181,20 @@
 
         Args:
             message (BaseMessage): The message to be set as the
                 new system message of this agent.
         """
         self._system_message = message
 
-    def is_function_calling_enabled(self) -> bool:
+    def is_tools_added(self) -> bool:
         r"""Whether OpenAI function calling is enabled for this agent.
 
         Returns:
             bool: Whether OpenAI function calling is enabled for this
-                agent, determined by whether the dictionary of functions
+                agent, determined by whether the dictionary of tools
                 is empty.
         """
         return len(self.func_dict) > 0
 
     def update_memory(
         self, message: BaseMessage, role: OpenAIBackendRole
     ) -> None:
@@ -245,38 +229,38 @@
 
     def get_info(
         self,
         id: Optional[str],
         usage: Optional[Dict[str, int]],
         termination_reasons: List[str],
         num_tokens: int,
-        called_funcs: List[FunctionCallingRecord],
+        tool_calls: List[FunctionCallingRecord],
     ) -> Dict[str, Any]:
         r"""Returns a dictionary containing information about the chat session.
 
         Args:
             id (str, optional): The ID of the chat session.
             usage (Dict[str, int], optional): Information about the usage of
                 the LLM model.
             termination_reasons (List[str]): The reasons for the termination
                 of the chat session.
             num_tokens (int): The number of tokens used in the chat session.
-            called_funcs (List[FunctionCallingRecord]): The list of function
+            tool_calls (List[FunctionCallingRecord]): The list of function
                 calling records, containing the information of called
-                functions.
+                tools.
 
         Returns:
             Dict[str, Any]: The chat session information.
         """
         return {
             "id": id,
             "usage": usage,
             "termination_reasons": termination_reasons,
             "num_tokens": num_tokens,
-            "called_functions": called_funcs,
+            "tool_calls": tool_calls,
         }
 
     def init_messages(self) -> None:
         r"""Initializes the stored messages list with the initial system
         message.
         """
         system_record = MemoryRecord(
@@ -301,37 +285,38 @@
         input_message: BaseMessage,
     ) -> ChatAgentResponse:
         r"""Performs a single step in the chat session by generating a response
         to the input message.
 
         Args:
             input_message (BaseMessage): The input message to the agent.
-            Its `role` field that specifies the role at backend may be either
-            `user` or `assistant` but it will be set to `user` anyway since
-            for the self agent any incoming message is external.
+                Its `role` field that specifies the role at backend may be
+                either `user` or `assistant` but it will be set to `user`
+                anyway since for the self agent any incoming message is
+                external.
 
         Returns:
             ChatAgentResponse: A struct containing the output messages,
                 a boolean indicating whether the chat session has terminated,
                 and information about the chat session.
         """
         self.update_memory(input_message, OpenAIBackendRole.USER)
 
         output_messages: List[BaseMessage]
         info: Dict[str, Any]
-        called_funcs: List[FunctionCallingRecord] = []
+        tool_calls: List[FunctionCallingRecord] = []
         while True:
             # Format messages and get the token number
             openai_messages: Optional[List[OpenAIMessage]]
 
             try:
                 openai_messages, num_tokens = self.memory.get_context()
             except RuntimeError as e:
                 return self.step_token_exceed(
-                    e.args[1], called_funcs, "max_tokens_exceeded"
+                    e.args[1], tool_calls, "max_tokens_exceeded"
                 )
 
             # Obtain the model's response
             response = self.model_backend.run(openai_messages)
 
             if isinstance(response, ChatCompletion):
                 output_messages, finish_reasons, usage_dict, response_id = (
@@ -339,31 +324,34 @@
                 )
             else:
                 output_messages, finish_reasons, usage_dict, response_id = (
                     self.handle_stream_response(response, num_tokens)
                 )
 
             if (
-                self.is_function_calling_enabled()
-                and finish_reasons[0] == 'function_call'
+                self.is_tools_added()
                 and isinstance(response, ChatCompletion)
+                and response.choices[0].message.tool_calls is not None
             ):
+                # Tools added for function calling and not in stream mode
+
                 # Do function calling
                 func_assistant_msg, func_result_msg, func_record = (
-                    self.step_function_call(response)
+                    self.step_tool_call(response)
                 )
 
                 # Update the messages
                 self.update_memory(
                     func_assistant_msg, OpenAIBackendRole.ASSISTANT
                 )
                 self.update_memory(func_result_msg, OpenAIBackendRole.FUNCTION)
 
                 # Record the function calling
-                called_funcs.append(func_record)
+                tool_calls.append(func_record)
+
             else:
                 # Function calling disabled or not a function calling
 
                 # Loop over responses terminators, get list of termination
                 # tuples with whether the terminator terminates the agent
                 # and termination reason
                 termination = [
@@ -384,15 +372,15 @@
                     finish_reasons = [termination_reason] * len(finish_reasons)
 
                 info = self.get_info(
                     response_id,
                     usage_dict,
                     finish_reasons,
                     num_tokens,
-                    called_funcs,
+                    tool_calls,
                 )
                 break
 
         return ChatAgentResponse(output_messages, self.terminated, info)
 
     def handle_batch_response(
         self, response: ChatCompletion
@@ -471,23 +459,23 @@
         ]
         usage_dict = self.get_usage_dict(output_messages, prompt_tokens)
         return output_messages, finish_reasons, usage_dict, response_id
 
     def step_token_exceed(
         self,
         num_tokens: int,
-        called_funcs: List[FunctionCallingRecord],
+        tool_calls: List[FunctionCallingRecord],
         termination_reason: str,
     ) -> ChatAgentResponse:
         r"""Return trivial response containing number of tokens and information
         of called functions when the number of tokens exceeds.
 
         Args:
             num_tokens (int): Number of tokens in the messages.
-            called_funcs (List[FunctionCallingRecord]): List of information
+            tool_calls (List[FunctionCallingRecord]): List of information
                 objects of functions called in the current step.
             termination_reason (str): String of termination reason.
 
         Returns:
             ChatAgentResponse: The struct containing trivial outputs and
                 information about token number and called functions.
         """
@@ -495,24 +483,24 @@
         output_messages: List[BaseMessage] = []
 
         info = self.get_info(
             None,
             None,
             [termination_reason],
             num_tokens,
-            called_funcs,
+            tool_calls,
         )
 
         return ChatAgentResponse(
             output_messages,
             self.terminated,
             info,
         )
 
-    def step_function_call(
+    def step_tool_call(
         self,
         response: ChatCompletion,
     ) -> Tuple[
         FunctionCallingMessage, FunctionCallingMessage, FunctionCallingRecord
     ]:
         r"""Execute the function with arguments following the model's response.
 
@@ -522,22 +510,21 @@
 
         Returns:
             tuple: A tuple consisting of two obj:`FunctionCallingMessage`,
                 one about the arguments and the other about the execution
                 result, and a struct for logging information about this
                 function call.
         """
-        # Note that when function calling is enabled, `n` is set to 1.
         choice = response.choices[0]
-        if choice.message.function_call is None:
-            raise RuntimeError("Function call is None")
-        func_name = choice.message.function_call.name
+        if choice.message.tool_calls is None:
+            raise RuntimeError("Tool calls is None")
+        func_name = choice.message.tool_calls[0].function.name
         func = self.func_dict[func_name]
 
-        args_str: str = choice.message.function_call.arguments
+        args_str: str = choice.message.tool_calls[0].function.arguments
         args = json.loads(args_str.replace("'", "\""))
 
         # Pass the extracted arguments to the indicated function
         try:
             result = func(**args)
         except Exception:
             raise ValueError(
```

### Comparing `camel_ai-0.1.3/camel/agents/critic_agent.py` & `camel_ai-0.1.4/camel/agents/critic_agent.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/agents/deductive_reasoner_agent.py` & `camel_ai-0.1.4/camel/agents/deductive_reasoner_agent.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/agents/embodied_agent.py` & `camel_ai-0.1.4/camel/agents/embodied_agent.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/agents/role_assignment_agent.py` & `camel_ai-0.1.4/camel/agents/role_assignment_agent.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/agents/task_agent.py` & `camel_ai-0.1.4/camel/agents/task_agent.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/agents/tool_agents/__init__.py` & `camel_ai-0.1.4/camel/agents/tool_agents/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/agents/tool_agents/base.py` & `camel_ai-0.1.4/camel/agents/tool_agents/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/agents/tool_agents/hugging_face_tool_agent.py` & `camel_ai-0.1.4/camel/agents/tool_agents/hugging_face_tool_agent.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/embeddings/__init__.py` & `camel_ai-0.1.4/camel/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/embeddings/base.py` & `camel_ai-0.1.4/camel/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/embeddings/openai_embedding.py` & `camel_ai-0.1.4/camel/embeddings/openai_embedding.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,43 +7,48 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
-from typing import Any, List
+import os
+from typing import Any, List, Optional
 
 from openai import OpenAI
 
 from camel.embeddings.base import BaseEmbedding
 from camel.types import EmbeddingModelType
 from camel.utils import api_key_required
 
 
 class OpenAIEmbedding(BaseEmbedding[str]):
     r"""Provides text embedding functionalities using OpenAI's models.
 
     Args:
         model (OpenAiEmbeddingModel, optional): The model type to be used for
             generating embeddings. (default: :obj:`ModelType.ADA_2`)
+        api_key (Optional[str]): The API key for authenticating with the
+            OpenAI service. (default: :obj:`None`)
 
     Raises:
         RuntimeError: If an unsupported model type is specified.
     """
 
     def __init__(
         self,
         model_type: EmbeddingModelType = EmbeddingModelType.ADA_2,
+        api_key: Optional[str] = None,
     ) -> None:
         if not model_type.is_openai:
             raise ValueError("Invalid OpenAI embedding model type.")
         self.model_type = model_type
         self.output_dim = model_type.output_dim
-        self.client = OpenAI()
+        self._api_key = api_key or os.environ.get("OPENAI_API_KEY")
+        self.client = OpenAI(timeout=60, max_retries=3, api_key=self._api_key)
 
     @api_key_required
     def embed_list(
         self,
         objs: List[str],
         **kwargs: Any,
     ) -> List[List[float]]:
```

### Comparing `camel_ai-0.1.3/camel/embeddings/sentence_transformers_embeddings.py` & `camel_ai-0.1.4/camel/embeddings/sentence_transformers_embeddings.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/functions/__init__.py` & `camel_ai-0.1.4/camel/functions/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,31 +7,36 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
-
-from ..loaders.unstructured_io import UnstructuredIO
-from .google_maps_function import MAP_FUNCS
-from .math_functions import MATH_FUNCS
+# ruff: noqa: I001
 from .openai_function import (
     OpenAIFunction,
     get_openai_function_schema,
     get_openai_tool_schema,
 )
+
+from .google_maps_function import MAP_FUNCS
+from .math_functions import MATH_FUNCS
+from .open_api_function import OPENAPI_FUNCS
+from .retrieval_functions import RETRIEVAL_FUNCS
 from .search_functions import SEARCH_FUNCS
 from .twitter_function import TWITTER_FUNCS
 from .weather_functions import WEATHER_FUNCS
+from .slack_functions import SLACK_FUNCS
 
 __all__ = [
     'OpenAIFunction',
-    'get_openai_tool_schema',
     'get_openai_function_schema',
+    'get_openai_tool_schema',
+    'MAP_FUNCS',
     'MATH_FUNCS',
+    'OPENAPI_FUNCS',
+    'RETRIEVAL_FUNCS',
     'SEARCH_FUNCS',
-    'WEATHER_FUNCS',
-    'MAP_FUNCS',
     'TWITTER_FUNCS',
-    'UnstructuredIO',
+    'WEATHER_FUNCS',
+    'SLACK_FUNCS',
 ]
```

### Comparing `camel_ai-0.1.3/camel/functions/google_maps_function.py` & `camel_ai-0.1.4/camel/functions/google_maps_function.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/functions/math_functions.py` & `camel_ai-0.1.4/camel/functions/math_functions.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/functions/openai_function.py` & `camel_ai-0.1.4/camel/functions/openai_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,14 @@
         func: Callable,
         openai_tool_schema: Optional[Dict[str, Any]] = None,
     ) -> None:
         self.func = func
         self.openai_tool_schema = openai_tool_schema or get_openai_tool_schema(
             func
         )
-        self.properties = self.openai_tool_schema
 
     @staticmethod
     def validate_openai_tool_schema(openai_tool_schema: Dict[str, Any]) -> None:
         r"""Validates the OpenAI tool schema against
         :obj:`ToolAssistantToolsFunction`.
         This function checks if the provided :obj:`openai_tool_schema` adheres
         to the specifications required by OpenAI's
@@ -189,14 +188,17 @@
             ValidationError: If the schema does not comply with the
                 specifications.
             ValueError: If the function description or parameter descriptions
                 are missing in the schema.
             SchemaError: If the parameters do not meet JSON Schema reference
                 specifications.
         """
+        # Check the type
+        if not openai_tool_schema["type"]:
+            raise ValueError("miss type")
         # Check the function description
         if not openai_tool_schema["function"]["description"]:
             raise ValueError("miss function description")
 
         # Validate whether parameters
         # meet the JSON Schema reference specifications.
         # See https://platform.openai.com/docs/guides/gpt/function-calling
```

### Comparing `camel_ai-0.1.3/camel/functions/search_functions.py` & `camel_ai-0.1.4/camel/functions/search_functions.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/functions/twitter_function.py` & `camel_ai-0.1.4/camel/functions/twitter_function.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/functions/weather_functions.py` & `camel_ai-0.1.4/camel/functions/weather_functions.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/generators.py` & `camel_ai-0.1.4/camel/generators.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/human.py` & `camel_ai-0.1.4/camel/human.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/interpreters/__init__.py` & `camel_ai-0.1.4/camel/interpreters/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/interpreters/base.py` & `camel_ai-0.1.4/camel/interpreters/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/interpreters/internal_python_interpreter.py` & `camel_ai-0.1.4/camel/interpreters/internal_python_interpreter.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/interpreters/interpreter_error.py` & `camel_ai-0.1.4/camel/interpreters/interpreter_error.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/interpreters/subprocess_interpreter.py` & `camel_ai-0.1.4/camel/interpreters/subprocess_interpreter.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/loaders/__init__.py` & `camel_ai-0.1.4/camel/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/loaders/base_io.py` & `camel_ai-0.1.4/camel/loaders/base_io.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/loaders/unstructured_io.py` & `camel_ai-0.1.4/camel/loaders/unstructured_io.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/memories/__init__.py` & `camel_ai-0.1.4/camel/memories/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/memories/agent_memories.py` & `camel_ai-0.1.4/camel/memories/agent_memories.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/memories/base.py` & `camel_ai-0.1.4/camel/memories/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/memories/blocks/__init__.py` & `camel_ai-0.1.4/camel/memories/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/memories/blocks/chat_history_block.py` & `camel_ai-0.1.4/camel/memories/blocks/chat_history_block.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/memories/blocks/vectordb_block.py` & `camel_ai-0.1.4/camel/memories/blocks/vectordb_block.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/memories/context_creators/__init__.py` & `camel_ai-0.1.4/camel/memories/context_creators/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/memories/context_creators/score_based.py` & `camel_ai-0.1.4/camel/memories/context_creators/score_based.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/memories/records.py` & `camel_ai-0.1.4/camel/memories/records.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/messages/__init__.py` & `camel_ai-0.1.4/camel/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/messages/base.py` & `camel_ai-0.1.4/camel/messages/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/messages/func_message.py` & `camel_ai-0.1.4/camel/messages/func_message.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/models/__init__.py` & `camel_ai-0.1.4/camel/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
 from .anthropic_model import AnthropicModel
 from .base_model import BaseModelBackend
 from .model_factory import ModelFactory
 from .open_source_model import OpenSourceModel
+from .openai_audio_models import OpenAIAudioModels
 from .openai_model import OpenAIModel
 from .stub_model import StubModel
 
 __all__ = [
     'BaseModelBackend',
     'OpenAIModel',
     'AnthropicModel',
     'StubModel',
     'OpenSourceModel',
     'ModelFactory',
+    'OpenAIAudioModels',
 ]
```

### Comparing `camel_ai-0.1.3/camel/models/anthropic_model.py` & `camel_ai-0.1.4/camel/models/openai_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,125 +8,103 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
 import os
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional, Union
 
-from anthropic import Anthropic
-from anthropic._types import NOT_GIVEN
+from openai import OpenAI, Stream
 
-from camel.configs import ANTHROPIC_API_PARAMS
-from camel.models.base_model import BaseModelBackend
-from camel.types import ChatCompletion, ModelType
-from camel.utils import AnthropicTokenCounter, BaseTokenCounter
+from camel.configs import OPENAI_API_PARAMS
+from camel.messages import OpenAIMessage
+from camel.models import BaseModelBackend
+from camel.types import ChatCompletion, ChatCompletionChunk, ModelType
+from camel.utils import BaseTokenCounter, OpenAITokenCounter, api_key_required
 
 
-class AnthropicModel(BaseModelBackend):
-    r"""Anthropic API in a unified BaseModelBackend interface."""
+class OpenAIModel(BaseModelBackend):
+    r"""OpenAI API in a unified BaseModelBackend interface."""
 
     def __init__(
-        self, model_type: ModelType, model_config_dict: Dict[str, Any]
+        self,
+        model_type: ModelType,
+        model_config_dict: Dict[str, Any],
+        api_key: Optional[str] = None,
     ) -> None:
-        super().__init__(model_type, model_config_dict)
-        self.client = Anthropic(api_key=os.environ["ANTHROPIC_API_KEY"])
-        self._token_counter: Optional[BaseTokenCounter] = None
+        r"""Constructor for OpenAI backend.
 
-    def _convert_response_from_anthropic_to_openai(self, response):
-        # openai ^1.0.0 format, reference openai/types/chat/chat_completion.py
-        obj = ChatCompletion.construct(
-            id=None,
-            choices=[
-                dict(
-                    index=0,
-                    message={
-                        "role": "assistant",
-                        "content": response.content[0].text,
-                    },
-                    finish_reason=response.stop_reason,
-                )
-            ],
-            created=None,
-            model=response.model,
-            object="chat.completion",
+        Args:
+            model_type (ModelType): Model for which a backend is created,
+                one of GPT_* series.
+            model_config_dict (Dict[str, Any]): A dictionary that will
+                be fed into openai.ChatCompletion.create().
+            api_key (Optional[str]): The API key for authenticating with the
+                OpenAI service. (default: :obj:`None`)
+        """
+        super().__init__(model_type, model_config_dict)
+        url = os.environ.get('OPENAI_API_BASE_URL', None)
+        self._api_key = api_key or os.environ.get("OPENAI_API_KEY")
+        self._client = OpenAI(
+            timeout=60, max_retries=3, base_url=url, api_key=self._api_key
         )
-        return obj
+        self._token_counter: Optional[BaseTokenCounter] = None
 
     @property
     def token_counter(self) -> BaseTokenCounter:
         r"""Initialize the token counter for the model backend.
 
         Returns:
             BaseTokenCounter: The token counter following the model's
                 tokenization style.
         """
         if not self._token_counter:
-            self._token_counter = AnthropicTokenCounter(self.model_type)
+            self._token_counter = OpenAITokenCounter(self.model_type)
         return self._token_counter
 
-    def count_tokens_from_prompt(self, prompt: str) -> int:
-        r"""Count the number of tokens from a prompt.
-
-        Args:
-            prompt (str): The prompt string.
-
-        Returns:
-            int: The number of tokens in the prompt.
-        """
-        return self.client.count_tokens(prompt)
-
+    @api_key_required
     def run(
         self,
-        messages,
-    ):
-        r"""Run inference of Anthropic chat completion.
+        messages: List[OpenAIMessage],
+    ) -> Union[ChatCompletion, Stream[ChatCompletionChunk]]:
+        r"""Runs inference of OpenAI chat completion.
 
         Args:
-            messages (List[Dict]): Message list with the chat history
+            messages (List[OpenAIMessage]): Message list with the chat history
                 in OpenAI API format.
 
         Returns:
-            Dict[str, Any]: Response in the OpenAI API format.
+            Union[ChatCompletion, Stream[ChatCompletionChunk]]:
+                `ChatCompletion` in the non-stream mode, or
+                `Stream[ChatCompletionChunk]` in the stream mode.
         """
-
-        if messages[0]["role"] == "system":
-            sys_msg = messages.pop(0)["content"]
-        else:
-            sys_msg = NOT_GIVEN
-        response = self.client.messages.create(
-            model=self.model_type.value,
-            system=sys_msg,
+        response = self._client.chat.completions.create(
             messages=messages,
+            model=self.model_type.value,
             **self.model_config_dict,
         )
-
-        # format response to openai format
-        response = self._convert_response_from_anthropic_to_openai(response)
-
         return response
 
     def check_model_config(self):
-        r"""Check whether the model configuration is valid for anthropic
-        model backends.
+        r"""Check whether the model configuration contains any
+        unexpected arguments to OpenAI API.
 
         Raises:
             ValueError: If the model configuration dictionary contains any
-                unexpected arguments to OpenAI API, or it does not contain
-                :obj:`model_path` or :obj:`server_url`.
+                unexpected arguments to OpenAI API.
         """
         for param in self.model_config_dict:
-            if param not in ANTHROPIC_API_PARAMS:
+            if param not in OPENAI_API_PARAMS:
                 raise ValueError(
                     f"Unexpected argument `{param}` is "
-                    "input into Anthropic model backend."
+                    "input into OpenAI model backend."
                 )
 
     @property
     def stream(self) -> bool:
         r"""Returns whether the model is in stream mode,
             which sends partial results each time.
         Returns:
             bool: Whether the model is in stream mode.
         """
-        return self.model_config_dict.get("stream", False)
+        return self.model_config_dict.get('stream', False)
```

### Comparing `camel_ai-0.1.3/camel/models/base_model.py` & `camel_ai-0.1.4/camel/models/base_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,40 +8,46 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
 from abc import ABC, abstractmethod
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List, Optional, Union
 
 from openai import Stream
 
 from camel.messages import OpenAIMessage
 from camel.types import ChatCompletion, ChatCompletionChunk, ModelType
 from camel.utils import BaseTokenCounter
 
 
 class BaseModelBackend(ABC):
     r"""Base class for different model backends.
     May be OpenAI API, a local LLM, a stub for unit tests, etc.
     """
 
     def __init__(
-        self, model_type: ModelType, model_config_dict: Dict[str, Any]
+        self,
+        model_type: ModelType,
+        model_config_dict: Dict[str, Any],
+        api_key: Optional[str] = None,
     ) -> None:
         r"""Constructor for the model backend.
 
         Args:
             model_type (ModelType): Model for which a backend is created.
             model_config_dict (Dict[str, Any]): A config dictionary.
+            api_key (Optional[str]): The API key for authenticating with the
+                LLM service.
         """
         self.model_type = model_type
 
         self.model_config_dict = model_config_dict
+        self._api_key = api_key
         self.check_model_config()
 
     @property
     @abstractmethod
     def token_counter(self) -> BaseTokenCounter:
         r"""Initialize the token counter for the model backend.
```

### Comparing `camel_ai-0.1.3/camel/models/model_factory.py` & `camel_ai-0.1.4/camel/models/model_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 
 from camel.models.anthropic_model import AnthropicModel
 from camel.models.base_model import BaseModelBackend
 from camel.models.open_source_model import OpenSourceModel
 from camel.models.openai_model import OpenAIModel
 from camel.models.stub_model import StubModel
 from camel.types import ModelType
@@ -26,22 +26,26 @@
 
     Raises:
         ValueError: in case the provided model type is unknown.
     """
 
     @staticmethod
     def create(
-        model_type: ModelType, model_config_dict: Dict
+        model_type: ModelType,
+        model_config_dict: Dict,
+        api_key: Optional[str] = None,
     ) -> BaseModelBackend:
         r"""Creates an instance of `BaseModelBackend` of the specified type.
 
         Args:
             model_type (ModelType): Model for which a backend is created.
             model_config_dict (Dict): A dictionary that will be fed into
                 the backend constructor.
+            api_key (Optional[str]): The API key for authenticating with the
+                LLM service.
 
         Raises:
             ValueError: If there is not backend for the model.
 
         Returns:
             BaseModelBackend: The initialized backend.
         """
@@ -53,9 +57,9 @@
         elif model_type.is_open_source:
             model_class = OpenSourceModel
         elif model_type.is_anthropic:
             model_class = AnthropicModel
         else:
             raise ValueError(f"Unknown model type `{model_type}` is input")
 
-        inst = model_class(model_type, model_config_dict)
+        inst = model_class(model_type, model_config_dict, api_key)
         return inst
```

### Comparing `camel_ai-0.1.3/camel/models/open_source_model.py` & `camel_ai-0.1.4/camel/models/open_source_model.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/models/stub_model.py` & `camel_ai-0.1.4/camel/models/stub_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,19 +46,23 @@
 
 class StubModel(BaseModelBackend):
     r"""A dummy model used for unit tests."""
 
     model_type = ModelType.STUB
 
     def __init__(
-        self, model_type: ModelType, model_config_dict: Dict[str, Any]
+        self,
+        model_type: ModelType,
+        model_config_dict: Dict[str, Any],
+        api_key: Optional[str] = None,
     ) -> None:
         r"""All arguments are unused for the dummy model."""
         super().__init__(model_type, model_config_dict)
         self._token_counter: Optional[BaseTokenCounter] = None
+        self._api_key = api_key
 
     @property
     def token_counter(self) -> BaseTokenCounter:
         r"""Initialize the token counter for the model backend.
 
         Returns:
             BaseTokenCounter: The token counter following the model's
```

### Comparing `camel_ai-0.1.3/camel/prompts/__init__.py` & `camel_ai-0.1.4/camel/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/prompts/ai_society.py` & `camel_ai-0.1.4/camel/prompts/ai_society.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/prompts/base.py` & `camel_ai-0.1.4/camel/prompts/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/prompts/code.py` & `camel_ai-0.1.4/camel/prompts/code.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/prompts/evaluation.py` & `camel_ai-0.1.4/camel/prompts/evaluation.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/prompts/misalignment.py` & `camel_ai-0.1.4/camel/prompts/misalignment.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/prompts/object_recognition.py` & `camel_ai-0.1.4/camel/prompts/object_recognition.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/prompts/prompt_templates.py` & `camel_ai-0.1.4/camel/prompts/prompt_templates.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/prompts/role_description_prompt_template.py` & `camel_ai-0.1.4/camel/prompts/role_description_prompt_template.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/prompts/solution_extraction.py` & `camel_ai-0.1.4/camel/prompts/solution_extraction.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/prompts/task_prompt_template.py` & `camel_ai-0.1.4/camel/prompts/task_prompt_template.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/prompts/translation.py` & `camel_ai-0.1.4/camel/prompts/translation.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/responses/__init__.py` & `camel_ai-0.1.4/camel/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/responses/agent_responses.py` & `camel_ai-0.1.4/camel/responses/agent_responses.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/retrievers/__init__.py` & `camel_ai-0.1.4/camel/toolkits/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,18 +7,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
-from .auto_retriever import AutoRetriever
-from .base import BaseRetriever
-from .bm25_retriever import BM25Retriever
-from .vector_retriever import VectorRetriever
+
+from .base import BaseToolkit
+from .github_toolkit import GithubToolkit
 
 __all__ = [
-    'BaseRetriever',
-    'VectorRetriever',
-    'AutoRetriever',
-    'BM25Retriever',
+    'BaseToolkit',
+    'GithubToolkit',
 ]
```

### Comparing `camel_ai-0.1.3/camel/retrievers/auto_retriever.py` & `camel_ai-0.1.4/camel/retrievers/auto_retriever.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,15 +59,16 @@
         self.vector_storage_local_path = vector_storage_local_path
         self.url_and_api_key = url_and_api_key
 
     def _initialize_vector_storage(
         self,
         collection_name: Optional[str] = None,
     ) -> BaseVectorStorage:
-        r"""Sets up and returns a vector storage instance with specified parameters.
+        r"""Sets up and returns a vector storage instance with specified
+        parameters.
 
         Args:
             collection_name (Optional[str]): Name of the collection in the
                 vector storage.
 
         Returns:
             BaseVectorStorage: Configured vector storage instance.
@@ -191,15 +192,16 @@
         self,
         query: str,
         content_input_paths: Union[str, List[str]],
         top_k: int = DEFAULT_TOP_K_RESULTS,
         similarity_threshold: float = DEFAULT_SIMILARITY_THRESHOLD,
         return_detailed_info: bool = False,
     ) -> str:
-        r"""Executes the automatic vector retriever process using vector storage.
+        r"""Executes the automatic vector retriever process using vector
+        storage.
 
         Args:
             query (str): Query string for information retriever.
             content_input_paths (Union[str, List[str]]): Paths to local
                 files or remote URLs.
             top_k (int, optional): The number of top results to return during
                 retrieve. Must be a positive integer. Defaults to
@@ -229,17 +231,15 @@
             [content_input_paths]
             if isinstance(content_input_paths, str)
             else content_input_paths
         )
 
         vr = VectorRetriever()
 
-        retrieved_infos = ""
-        retrieved_infos_text = ""
-
+        all_retrieved_info = []
         for content_input_path in content_input_paths:
             # Generate a valid collection name
             collection_name = self._collection_name_generator(
                 content_input_path
             )
             try:
                 vector_storage_instance = self._initialize_vector_storage(
@@ -274,46 +274,57 @@
                 if (
                     vector_storage_instance.status().vector_count == 0
                     or file_is_modified
                 ):
                     # Clear the vector storage
                     vector_storage_instance.clear()
                     # Process and store the content to the vector storage
-                    vr.process(content_input_path, vector_storage_instance)
+                    vr = VectorRetriever(
+                        storage=vector_storage_instance,
+                        similarity_threshold=similarity_threshold,
+                    )
+                    vr.process(content_input_path)
+                else:
+                    vr = VectorRetriever(
+                        storage=vector_storage_instance,
+                        similarity_threshold=similarity_threshold,
+                    )
                 # Retrieve info by given query from the vector storage
-                retrieved_info = vr.query(
-                    query, vector_storage_instance, top_k, similarity_threshold
-                )
-                # Reorganize the retrieved info with original query
-                for info in retrieved_info:
-                    retrieved_infos += "\n" + str(info)
-                    retrieved_infos_text += "\n" + str(info['text'])
-                output = (
-                    "Original Query:"
-                    + "\n"
-                    + "{"
-                    + query
-                    + "}"
-                    + "\n"
-                    + "Retrieved Context:"
-                    + retrieved_infos
-                )
-                output_text = (
-                    "Original Query:"
-                    + "\n"
-                    + "{"
-                    + query
-                    + "}"
-                    + "\n"
-                    + "Retrieved Context:"
-                    + retrieved_infos_text
-                )
-
+                retrieved_info = vr.query(query, top_k)
+                all_retrieved_info.extend(retrieved_info)
             except Exception as e:
                 raise RuntimeError(
                     f"Error in auto vector retriever processing: {e!s}"
                 ) from e
 
+        # Split records into those with and without a 'similarity_score'
+        # Records with 'similarity_score' lower than 'similarity_threshold'
+        # will not have a 'similarity_score' in the output content
+        with_score = [
+            info for info in all_retrieved_info if 'similarity score' in info
+        ]
+        without_score = [
+            info
+            for info in all_retrieved_info
+            if 'similarity score' not in info
+        ]
+        # Sort only the list with scores
+        with_score_sorted = sorted(
+            with_score, key=lambda x: x['similarity score'], reverse=True
+        )
+        # Merge back the sorted scored items with the non-scored items
+        all_retrieved_info_sorted = with_score_sorted + without_score
+        # Select the 'top_k' results
+        all_retrieved_info = all_retrieved_info_sorted[:top_k]
+
+        retrieved_infos = "\n".join(str(info) for info in all_retrieved_info)
+        retrieved_infos_text = "\n".join(
+            info['text'] for info in all_retrieved_info if 'text' in info
+        )
+
+        detailed_info = f"Original Query:\n{{ {query} }}\nRetrieved Context:\n{retrieved_infos}"
+        text_info = f"Original Query:\n{{ {query} }}\nRetrieved Context:\n{retrieved_infos_text}"
+
         if return_detailed_info:
-            return output
+            return detailed_info
         else:
-            return output_text
+            return text_info
```

### Comparing `camel_ai-0.1.3/camel/retrievers/base.py` & `camel_ai-0.1.4/camel/retrievers/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,57 +8,62 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
 from abc import ABC, abstractmethod
-from typing import Any, Dict, List
+from typing import Any, Callable
 
 DEFAULT_TOP_K_RESULTS = 1
 
 
-class BaseRetriever(ABC):
-    r"""Abstract base class for implementing various types of information
-    retrievers.
+def _query_unimplemented(self, *input: Any) -> None:
+    r"""Defines the query behavior performed at every call.
+
+    Query the results. Subclasses should implement this
+        method according to their specific needs.
+
+    It should be overridden by all subclasses.
+
+    .. note::
+        Although the recipe for forward pass needs to be defined within
+        this function, one should call the :class:`BaseRetriever` instance
+        afterwards instead of this since the former takes care of running the
+        registered hooks while the latter silently ignores them.
     """
+    raise NotImplementedError(
+        f"Retriever [{type(self).__name__}] is missing the required \"query\" function"
+    )
 
-    @abstractmethod
-    def __init__(self) -> None:
-        pass
 
-    @abstractmethod
-    def process(
-        self,
-        content_input_path: str,
-        chunk_type: str = "chunk_by_title",
-        **kwargs: Any,
-    ) -> None:
-        r"""Processes content from a file or URL, divides it into chunks by
+def _process_unimplemented(self, *input: Any) -> None:
+    r"""Defines the process behavior performed at every call.
+
+    Processes content from a file or URL, divides it into chunks by
         using `Unstructured IO`,then stored internally. This method must be
         called before executing queries with the retriever.
 
-        Args:
-            content_input_path (str): File path or URL of the content to be
-                processed.
-            chunk_type (str): Type of chunking going to apply. Defaults to
-                "chunk_by_title".
-            **kwargs (Any): Additional keyword arguments for content parsing.
-        """
-        pass
+    Should be overridden by all subclasses.
 
-    @abstractmethod
-    def query(
-        self, query: str, top_k: int = DEFAULT_TOP_K_RESULTS, **kwargs: Any
-    ) -> List[Dict[str, Any]]:
-        r"""Query the results. Subclasses should implement this
-        method according to their specific needs.
+    .. note::
+        Although the recipe for forward pass needs to be defined within
+        this function, one should call the :class:`BaseRetriever` instance
+        afterwards instead of this since the former takes care of running the
+        registered hooks while the latter silently ignores them.
+    """
+    raise NotImplementedError(
+        f"Retriever [{type(self).__name__}] is missing the required \"process\" function"
+    )
+
+
+class BaseRetriever(ABC):
+    r"""Abstract base class for implementing various types of information
+    retrievers.
+    """
 
-        Args:
-            query (str): Query string for information retriever.
-            top_k (int, optional): The number of top results to return during
-                retriever. Must be a positive integer. Defaults to
-                `DEFAULT_TOP_K_RESULTS`.
-            **kwargs (Any): Flexible keyword arguments for additional
-                parameters, like `similarity_threshold`.
-        """
+    @abstractmethod
+    def __init__(self) -> None:
         pass
+
+    process: Callable[..., Any] = _process_unimplemented
+    query: Callable[..., Any] = _query_unimplemented
```

### Comparing `camel_ai-0.1.3/camel/retrievers/bm25_retriever.py` & `camel_ai-0.1.4/camel/retrievers/bm25_retriever.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,35 +29,34 @@
     frequency of the query terms.
 
     Attributes:
         bm25 (BM25Okapi): An instance of the BM25Okapi class used for
             calculating document scores.
         content_input_path (str): The path to the content that has been
             processed and stored.
-        chunks (List[Any]): A list of document chunks processed from the
-            input content.
+        unstructured_modules (UnstructuredIO): A module for parsing files and
+            URLs and chunking content based on specified parameters.
 
     References:
         https://github.com/dorianbrown/rank_bm25
     """
 
     def __init__(self) -> None:
         r"""Initializes the BM25Retriever."""
 
         try:
             from rank_bm25 import BM25Okapi
         except ImportError as e:
             raise ImportError(
-                "Package `rank_bm25` not installed, install by running"
-                " 'pip install rank_bm25'"
+                "Package `rank_bm25` not installed, install by running 'pip install rank_bm25'"
             ) from e
 
         self.bm25: BM25Okapi = None
         self.content_input_path: str = ""
-        self.chunks: List[Any] = []
+        self.unstructured_modules: UnstructuredIO = UnstructuredIO()
 
     def process(
         self,
         content_input_path: str,
         chunk_type: str = "chunk_by_title",
         **kwargs: Any,
     ) -> None:
@@ -72,27 +71,26 @@
                 "chunk_by_title".
             **kwargs (Any): Additional keyword arguments for content parsing.
         """
         from rank_bm25 import BM25Okapi
 
         # Load and preprocess documents
         self.content_input_path = content_input_path
-        unstructured_modules = UnstructuredIO()
-        elements = unstructured_modules.parse_file_or_url(
+        elements = self.unstructured_modules.parse_file_or_url(
             content_input_path, **kwargs
         )
-        self.chunks = unstructured_modules.chunk_elements(
+        self.chunks = self.unstructured_modules.chunk_elements(
             chunk_type=chunk_type, elements=elements
         )
 
         # Convert chunks to a list of strings for tokenization
         tokenized_corpus = [str(chunk).split(" ") for chunk in self.chunks]
         self.bm25 = BM25Okapi(tokenized_corpus)
 
-    def query(  # type: ignore[override]
+    def query(
         self,
         query: str,
         top_k: int = DEFAULT_TOP_K_RESULTS,
     ) -> List[Dict[str, Any]]:
         r"""Executes a query and compiles the results.
 
         Args:
@@ -102,30 +100,23 @@
                 `DEFAULT_TOP_K_RESULTS`.
 
         Returns:
             List[Dict[str]]: Concatenated list of the query results.
 
         Raises:
             ValueError: If `top_k` is less than or equal to 0, if the BM25
-                model has not been initialized by calling `process_and_store`
+                model has not been initialized by calling `process`
                 first.
-
-        Note:
-            `storage` and `kwargs` parameters are included to maintain
-            compatibility with the `BaseRetriever` interface but are not used
-            in this implementation.
         """
 
         if top_k <= 0:
             raise ValueError("top_k must be a positive integer.")
-
-        if self.bm25 is None:
+        if self.bm25 is None or not self.chunks:
             raise ValueError(
-                "BM25 model is not initialized. Call `process_and_store`"
-                " first."
+                "BM25 model is not initialized. Call `process` first."
             )
 
         # Preprocess query similarly to how documents were processed
         processed_query = query.split(" ")
         # Retrieve documents based on BM25 scores
         scores = self.bm25.get_scores(processed_query)
```

### Comparing `camel_ai-0.1.3/camel/retrievers/vector_retriever.py` & `camel_ai-0.1.4/camel/retrievers/vector_retriever.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,17 +10,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
 from typing import Any, Dict, List, Optional
 
 from camel.embeddings import BaseEmbedding, OpenAIEmbedding
-from camel.functions import UnstructuredIO
+from camel.loaders import UnstructuredIO
 from camel.retrievers.base import BaseRetriever
-from camel.storages import BaseVectorStorage, VectorDBQuery, VectorRecord
+from camel.storages import (
+    BaseVectorStorage,
+    QdrantStorage,
+    VectorDBQuery,
+    VectorRecord,
+)
 
 DEFAULT_TOP_K_RESULTS = 1
 DEFAULT_SIMILARITY_THRESHOLD = 0.75
 
 
 class VectorRetriever(BaseRetriever):
     r"""An implementation of the `BaseRetriever` by using vector storage and
@@ -28,47 +33,68 @@
 
     This class facilitates the retriever of relevant information using a
     query-based approach, backed by vector embeddings.
 
     Attributes:
         embedding_model (BaseEmbedding): Embedding model used to generate
             vector embeddings.
+        storage (BaseVectorStorage): Vector storage to query.
+        similarity_threshold (float, optional): The similarity threshold
+            for filtering results. Defaults to `DEFAULT_SIMILARITY_THRESHOLD`.
+        unstructured_modules (UnstructuredIO): A module for parsing files and
+            URLs and chunking content based on specified parameters.
     """
 
-    def __init__(self, embedding_model: Optional[BaseEmbedding] = None) -> None:
+    def __init__(
+        self,
+        similarity_threshold: float = DEFAULT_SIMILARITY_THRESHOLD,
+        embedding_model: Optional[BaseEmbedding] = None,
+        storage: Optional[BaseVectorStorage] = None,
+    ) -> None:
         r"""Initializes the retriever class with an optional embedding model.
 
         Args:
+            similarity_threshold (float, optional): The similarity threshold
+                for filtering results. Defaults to
+                `DEFAULT_SIMILARITY_THRESHOLD`.
             embedding_model (Optional[BaseEmbedding]): The embedding model
                 instance. Defaults to `OpenAIEmbedding` if not provided.
+            storage (BaseVectorStorage): Vector storage to query.
         """
         self.embedding_model = embedding_model or OpenAIEmbedding()
+        self.storage = (
+            storage
+            if storage is not None
+            else QdrantStorage(vector_dim=self.embedding_model.get_output_dim())
+        )
+        self.similarity_threshold = similarity_threshold
+        self.unstructured_modules: UnstructuredIO = UnstructuredIO()
 
-    def process(  # type: ignore[override]
+    def process(
         self,
         content_input_path: str,
-        storage: BaseVectorStorage,
         chunk_type: str = "chunk_by_title",
         **kwargs: Any,
     ) -> None:
         r"""Processes content from a file or URL, divides it into chunks by
         using `Unstructured IO`, and stores their embeddings in the specified
         vector storage.
 
         Args:
             content_input_path (str): File path or URL of the content to be
                 processed.
             chunk_type (str): Type of chunking going to apply. Defaults to
                 "chunk_by_title".
-            **kwargs (Any): Additional keyword arguments for elements chunking.
+            **kwargs (Any): Additional keyword arguments for content parsing.
         """
-        unstructured_modules = UnstructuredIO()
-        elements = unstructured_modules.parse_file_or_url(content_input_path)
-        chunks = unstructured_modules.chunk_elements(
-            chunk_type=chunk_type, elements=elements, **kwargs
+        elements = self.unstructured_modules.parse_file_or_url(
+            content_input_path, **kwargs
+        )
+        chunks = self.unstructured_modules.chunk_elements(
+            chunk_type=chunk_type, elements=elements
         )
         # Iterate to process and store embeddings, set batch of 50
         for i in range(0, len(chunks), 50):
             batch_chunks = chunks[i : i + 50]
             batch_vectors = self.embedding_model.embed_list(
                 objs=[str(chunk) for chunk in batch_chunks]
             )
@@ -86,66 +112,57 @@
                     **chunk_text,
                 }
 
                 records.append(
                     VectorRecord(vector=vector, payload=combined_dict)
                 )
 
-            storage.add(records=records)
+            self.storage.add(records=records)
 
-    def query(  # type: ignore[override]
+    def query(
         self,
         query: str,
-        storage: BaseVectorStorage,
         top_k: int = DEFAULT_TOP_K_RESULTS,
-        similarity_threshold: float = DEFAULT_SIMILARITY_THRESHOLD,
-        **kwargs: Any,
     ) -> List[Dict[str, Any]]:
         r"""Executes a query in vector storage and compiles the retrieved
         results into a dictionary.
 
         Args:
             query (str): Query string for information retriever.
-            storage (BaseVectorStorage): Vector storage to query.
             top_k (int, optional): The number of top results to return during
                 retriever. Must be a positive integer. Defaults to 1.
-            similarity_threshold (float, optional): The similarity threshold
-                for filtering results. Defaults to 0.75.
-            **kwargs (Any): Additional keyword arguments for vector storage
-                query.
 
         Returns:
             List[Dict[str, Any]]: Concatenated list of the query results.
 
         Raises:
             ValueError: If 'top_k' is less than or equal to 0, if vector
                 storage is empty, if payload of vector storage is None.
         """
 
         if top_k <= 0:
             raise ValueError("top_k must be a positive integer.")
 
         # Load the storage incase it's hosted remote
-        storage.load()
+        self.storage.load()
 
         query_vector = self.embedding_model.embed(obj=query)
         db_query = VectorDBQuery(query_vector=query_vector, top_k=top_k)
-        query_results = storage.query(query=db_query, **kwargs)
+        query_results = self.storage.query(query=db_query)
 
         if query_results[0].record.payload is None:
             raise ValueError(
-                "Payload of vector storage is None, please check"
-                " the collection."
+                "Payload of vector storage is None, please check the collection."
             )
 
         # format the results
         formatted_results = []
         for result in query_results:
             if (
-                result.similarity >= similarity_threshold
+                result.similarity >= self.similarity_threshold
                 and result.record.payload is not None
             ):
                 result_dict = {
                     'similarity score': str(result.similarity),
                     'content path': result.record.payload.get(
                         'content path', ''
                     ),
@@ -156,11 +173,11 @@
 
         content_path = query_results[0].record.payload.get('content path', '')
 
         if not formatted_results:
             return [
                 {
                     'text': f"""No suitable information retrieved from {content_path} \
-                with similarity_threshold = {similarity_threshold}."""
+                with similarity_threshold = {self.similarity_threshold}."""
                 }
             ]
         return formatted_results
```

### Comparing `camel_ai-0.1.3/camel/societies/__init__.py` & `camel_ai-0.1.4/camel/societies/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/societies/babyagi_playing.py` & `camel_ai-0.1.4/camel/societies/babyagi_playing.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/societies/role_playing.py` & `camel_ai-0.1.4/camel/societies/role_playing.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/storages/__init__.py` & `camel_ai-0.1.4/camel/storages/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/storages/graph_storages/__init__.py` & `camel_ai-0.1.4/camel/storages/graph_storages/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/storages/graph_storages/base.py` & `camel_ai-0.1.4/camel/storages/graph_storages/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/storages/graph_storages/graph_element.py` & `camel_ai-0.1.4/camel/storages/graph_storages/graph_element.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/storages/graph_storages/neo4j_graph.py` & `camel_ai-0.1.4/camel/storages/graph_storages/neo4j_graph.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/storages/key_value_storages/__init__.py` & `camel_ai-0.1.4/camel/storages/key_value_storages/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/storages/key_value_storages/base.py` & `camel_ai-0.1.4/camel/storages/key_value_storages/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/storages/key_value_storages/in_memory.py` & `camel_ai-0.1.4/camel/storages/key_value_storages/in_memory.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/storages/key_value_storages/json.py` & `camel_ai-0.1.4/camel/storages/key_value_storages/json.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/storages/vectordb_storages/__init__.py` & `camel_ai-0.1.4/camel/storages/vectordb_storages/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/storages/vectordb_storages/base.py` & `camel_ai-0.1.4/camel/storages/vectordb_storages/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/storages/vectordb_storages/milvus.py` & `camel_ai-0.1.4/camel/storages/vectordb_storages/milvus.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/storages/vectordb_storages/qdrant.py` & `camel_ai-0.1.4/camel/storages/vectordb_storages/qdrant.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,17 @@
         from qdrant_client.http.models import Distance, VectorParams
 
         distance_map = {
             VectorDistance.DOT: Distance.DOT,
             VectorDistance.COSINE: Distance.COSINE,
             VectorDistance.EUCLIDEAN: Distance.EUCLID,
         }
-        self._client.recreate_collection(
+        # Since `recreate_collection` method will be removed in the future
+        # by Qdrant, `create_collection` is recommended instead.
+        self._client.create_collection(
             collection_name=collection_name,
             vectors_config=VectorParams(
                 size=size,
                 distance=distance_map[distance],
             ),
             **kwargs,
         )
```

### Comparing `camel_ai-0.1.3/camel/terminators/__init__.py` & `camel_ai-0.1.4/camel/terminators/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/terminators/base.py` & `camel_ai-0.1.4/camel/terminators/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/terminators/response_terminator.py` & `camel_ai-0.1.4/camel/terminators/response_terminator.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/terminators/token_limit_terminator.py` & `camel_ai-0.1.4/camel/terminators/token_limit_terminator.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/types/__init__.py` & `camel_ai-0.1.4/camel/types/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,24 +8,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
 from .enums import (
+    AudioModelType,
     EmbeddingModelType,
     ModelType,
     OpenAIBackendRole,
     OpenAIImageDetailType,
     OpenAIImageType,
+    OpenAPIName,
     RoleType,
     StorageType,
     TaskType,
     TerminationMode,
     VectorDistance,
+    VoiceType,
 )
 from .openai_types import (
     ChatCompletion,
     ChatCompletionAssistantMessageParam,
     ChatCompletionChunk,
     ChatCompletionFunctionMessageParam,
     ChatCompletionMessage,
@@ -53,8 +56,11 @@
     'ChatCompletionSystemMessageParam',
     'ChatCompletionUserMessageParam',
     'ChatCompletionAssistantMessageParam',
     'ChatCompletionFunctionMessageParam',
     'CompletionUsage',
     'OpenAIImageType',
     'OpenAIImageDetailType',
+    'OpenAPIName',
+    'AudioModelType',
+    'VoiceType',
 ]
```

### Comparing `camel_ai-0.1.3/camel/types/enums.py` & `camel_ai-0.1.4/camel/types/enums.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 class ModelType(Enum):
     GPT_3_5_TURBO = "gpt-3.5-turbo"
     GPT_4 = "gpt-4"
     GPT_4_32K = "gpt-4-32k"
     GPT_4_TURBO = "gpt-4-turbo"
-    GPT_4_TURBO_VISION = "gpt-4-turbo"
+    GPT_4O = "gpt-4o"
 
     STUB = "stub"
 
     LLAMA_2 = "llama-2"
     VICUNA = "vicuna"
     VICUNA_16K = "vicuna-16k"
 
@@ -55,15 +55,15 @@
     def is_openai(self) -> bool:
         r"""Returns whether this type of models is an OpenAI-released model."""
         return self in {
             ModelType.GPT_3_5_TURBO,
             ModelType.GPT_4,
             ModelType.GPT_4_32K,
             ModelType.GPT_4_TURBO,
-            ModelType.GPT_4_TURBO_VISION,
+            ModelType.GPT_4O,
         }
 
     @property
     def is_open_source(self) -> bool:
         r"""Returns whether this type of models is open-source."""
         return self in {
             ModelType.LLAMA_2,
@@ -97,15 +97,15 @@
             return 16385
         elif self is ModelType.GPT_4:
             return 8192
         elif self is ModelType.GPT_4_32K:
             return 32768
         elif self is ModelType.GPT_4_TURBO:
             return 128000
-        elif self is ModelType.GPT_4_TURBO_VISION:
+        elif self is ModelType.GPT_4O:
             return 128000
         elif self is ModelType.STUB:
             return 4096
         elif self is ModelType.LLAMA_2:
             return 4096
         elif self is ModelType.VICUNA:
             # reference: https://lmsys.org/blog/2023-03-30-vicuna/
@@ -243,7 +243,48 @@
     LOW = "low"
     HIGH = "high"
 
 
 class StorageType(Enum):
     MILVUS = "milvus"
     QDRANT = "qdrant"
+
+
+class OpenAPIName(Enum):
+    COURSERA = "coursera"
+    KLARNA = "klarna"
+    SPEAK = "speak"
+
+
+class AudioModelType(Enum):
+    TTS_1 = "tts-1"
+    TTS_1_HD = "tts-1-hd"
+
+    @property
+    def is_openai(self) -> bool:
+        r"""Returns whether this type of audio models is an OpenAI-released
+        model."""
+        return self in {
+            AudioModelType.TTS_1,
+            AudioModelType.TTS_1_HD,
+        }
+
+
+class VoiceType(Enum):
+    ALLOY = "alloy"
+    ECHO = "echo"
+    FABLE = "fable"
+    ONYX = "onyx"
+    NOVA = "nova"
+    SHIMMER = "shimmer"
+
+    @property
+    def is_openai(self) -> bool:
+        r"""Returns whether this type of voice is an OpenAI-released voice."""
+        return self in {
+            VoiceType.ALLOY,
+            VoiceType.ECHO,
+            VoiceType.FABLE,
+            VoiceType.ONYX,
+            VoiceType.NOVA,
+            VoiceType.SHIMMER,
+        }
```

### Comparing `camel_ai-0.1.3/camel/types/openai_types.py` & `camel_ai-0.1.4/camel/types/openai_types.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/camel/utils/__init__.py` & `camel_ai-0.1.4/camel/utils/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,22 +10,23 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
 from .commons import (
     PYDANTIC_V2,
     api_key_required,
+    api_keys_required,
     check_server_running,
+    dependencies_required,
     download_tasks,
     get_first_int,
     get_prompt_template_key_words,
     get_system_information,
     get_task_list,
     print_text_animated,
-    role_playing_with_function,
     to_pascal,
 )
 from .token_counting import (
     AnthropicTokenCounter,
     BaseTokenCounter,
     OpenAITokenCounter,
     OpenSourceTokenCounter,
@@ -44,9 +45,10 @@
     'get_system_information',
     'to_pascal',
     'PYDANTIC_V2',
     'get_model_encoding',
     'BaseTokenCounter',
     'OpenAITokenCounter',
     'OpenSourceTokenCounter',
-    'role_playing_with_function',
+    'dependencies_required',
+    'api_keys_required',
 ]
```

### Comparing `camel_ai-0.1.3/camel/utils/commons.py` & `camel_ai-0.1.4/camel/utils/commons.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
+import importlib
 import os
 import platform
 import re
 import socket
 import time
 import zipfile
 from functools import wraps
@@ -25,59 +26,32 @@
 import requests
 
 from camel.types import TaskType
 
 F = TypeVar('F', bound=Callable[..., Any])
 
 
-# Set lazy import
-def get_lazy_imported_functions_module():
-    from camel.functions import (
-        MAP_FUNCS,
-        MATH_FUNCS,
-        SEARCH_FUNCS,
-        TWITTER_FUNCS,
-        WEATHER_FUNCS,
-    )
-
-    return [
-        *MATH_FUNCS,
-        *SEARCH_FUNCS,
-        *WEATHER_FUNCS,
-        *MAP_FUNCS,
-        *TWITTER_FUNCS,
-    ]
-
-
-# Set lazy import
-def get_lazy_imported_types_module():
-    from camel.types import ModelType
-
-    return ModelType.GPT_4_TURBO
-
-
 def api_key_required(func: F) -> F:
-    r"""Decorator that checks if the OpenAI API key is available in the
-    environment variables.
+    r"""Decorator that checks if the API key is available either as an environment variable or passed directly.
 
     Args:
         func (callable): The function to be wrapped.
 
     Returns:
         callable: The decorated function.
 
     Raises:
-        ValueError: If the OpenAI API key is not found in the environment
-            variables.
+        ValueError: If the API key is not found, either as an environment
+            variable or directly passed.
     """
 
     @wraps(func)
     def wrapper(self, *args, **kwargs):
         if self.model_type.is_openai:
-            if 'OPENAI_API_KEY' not in os.environ:
+            if not self._api_key and 'OPENAI_API_KEY' not in os.environ:
                 raise ValueError('OpenAI API key not found.')
             return func(self, *args, **kwargs)
         elif self.model_type.is_anthropic:
             if 'ANTHROPIC_API_KEY' not in os.environ:
                 raise ValueError('Anthropic API key not found.')
             return func(self, *args, **kwargs)
         else:
@@ -212,14 +186,106 @@
     result = sock.connect_ex(url_tuple)
     sock.close()
 
     # if the port is open, the result should be 0.
     return result == 0
 
 
+def dependencies_required(*required_modules: str) -> Callable[[F], F]:
+    r"""A decorator to ensure that specified Python modules
+    are available before a function executes.
+
+    Args:
+        required_modules (str): The required modules to be checked for
+            availability.
+
+    Returns:
+        Callable[[F], F]: The original function with the added check for
+            required module dependencies.
+
+    Raises:
+        ImportError: If any of the required modules are not available.
+
+    Example:
+        ::
+
+            @dependencies_required('numpy', 'pandas')
+            def data_processing_function():
+                # Function implementation...
+    """
+
+    def decorator(func: F) -> F:
+        @wraps(func)
+        def wrapper(*args: Any, **kwargs: Any) -> Any:
+            missing_modules = [
+                m for m in required_modules if not is_module_available(m)
+            ]
+            if missing_modules:
+                raise ImportError(
+                    f"Missing required modules: {', '.join(missing_modules)}"
+                )
+            return func(*args, **kwargs)
+
+        return cast(F, wrapper)
+
+    return decorator
+
+
+def is_module_available(module_name: str) -> bool:
+    r"""Check if a module is available for import.
+
+    Args:
+        module_name (str): The name of the module to check for availability.
+
+    Returns:
+        bool: True if the module can be imported, False otherwise.
+    """
+    try:
+        importlib.import_module(module_name)
+        return True
+    except ImportError:
+        return False
+
+
+def api_keys_required(*required_keys: str) -> Callable[[F], F]:
+    r"""A decorator to check if the required API keys are
+    present in the environment variables.
+
+    Args:
+        required_keys (str): The required API keys to be checked.
+
+    Returns:
+        Callable[[F], F]: The original function with the added check
+            for required API keys.
+
+    Raises:
+        ValueError: If any of the required API keys are missing in the
+            environment variables.
+
+    Example:
+        ::
+
+            @api_keys_required('API_KEY_1', 'API_KEY_2')
+            def some_api_function():
+                # Function implementation...
+    """
+
+    def decorator(func: F) -> F:
+        @wraps(func)
+        def wrapper(*args: Any, **kwargs: Any) -> Any:
+            missing_keys = [k for k in required_keys if k not in os.environ]
+            if missing_keys:
+                raise ValueError(f"Missing API keys: {', '.join(missing_keys)}")
+            return func(*args, **kwargs)
+
+        return cast(F, wrapper)
+
+    return decorator
+
+
 def get_system_information():
     r"""Gathers information about the operating system.
 
     Returns:
         dict: A dictionary containing various pieces of OS information.
     """
     sys_info = {
@@ -256,149 +322,7 @@
         '_([0-9A-Za-z])',
         lambda m: m.group(1).upper(),
         snake.title(),
     )
 
 
 PYDANTIC_V2 = pydantic.VERSION.startswith("2.")
-
-
-def role_playing_with_function(
-    task_prompt: str = (
-        "Assume now is 2024 in the Gregorian calendar, "
-        "estimate the current age of University of Oxford "
-        "and then add 10 more years to this age, "
-        "and get the current weather of the city where "
-        "the University is located. And tell me what time "
-        "zone University of Oxford is in. And use my twitter "
-        "account infomation to create a tweet. "
-    ),
-    function_list: Optional[List] = None,
-    model_type=None,
-    chat_turn_limit=10,
-    assistant_role_name: str = "Searcher",
-    user_role_name: str = "Professor",
-) -> None:
-    r"""Initializes and conducts a `RolePlaying` with `FunctionCallingConfig`
-    session. The function creates an interactive and dynamic role-play session
-    where the AI Assistant and User engage based on the given task, roles, and
-    available functions. It demonstrates the versatility of AI in handling
-    diverse tasks and user interactions within a structured `RolePlaying`
-    framework.
-
-    Args:
-        task_prompt (str): The initial task or scenario description to start
-            the `RolePlaying` session. Defaults to a prompt involving the
-            estimation of KAUST's age and weather information.
-        function_list (list): A list of functions that the agent can utilize
-            during the session. Defaults to a combination of math, search, and
-            weather functions.
-        model_type (ModelType): The type of chatbot model used for both the
-            assistant and the user. Defaults to `GPT-4 Turbo`.
-        chat_turn_limit (int): The maximum number of turns (exchanges) in the
-            chat session. Defaults to 10.
-        assistant_role_name (str): The role name assigned to the AI Assistant.
-            Defaults to 'Searcher'.
-        user_role_name (str): The role name assigned to the User. Defaults to
-            'Professor'.
-
-    Returns:
-        None: This function does not return any value but prints out the
-            session's dialogues and outputs.
-    """
-
-    # Run lazy import
-    if function_list is None:
-        function_list = get_lazy_imported_functions_module()
-    if model_type is None:
-        model_type = get_lazy_imported_types_module()
-
-    from colorama import Fore
-
-    from camel.agents.chat_agent import FunctionCallingRecord
-    from camel.configs import ChatGPTConfig, FunctionCallingConfig
-    from camel.societies import RolePlaying
-
-    task_prompt = task_prompt
-    user_model_config = ChatGPTConfig(temperature=0.0)
-
-    function_list = function_list
-    assistant_model_config = FunctionCallingConfig.from_openai_function_list(
-        function_list=function_list,
-        kwargs=dict(temperature=0.0),
-    )
-
-    role_play_session = RolePlaying(
-        assistant_role_name=assistant_role_name,
-        user_role_name=user_role_name,
-        assistant_agent_kwargs=dict(
-            model_type=model_type,
-            model_config=assistant_model_config,
-            function_list=function_list,
-        ),
-        user_agent_kwargs=dict(
-            model_type=model_type,
-            model_config=user_model_config,
-        ),
-        task_prompt=task_prompt,
-        with_task_specify=False,
-    )
-
-    print(
-        Fore.GREEN
-        + f"AI Assistant sys message:\n{role_play_session.assistant_sys_msg}\n"
-    )
-    print(
-        Fore.BLUE + f"AI User sys message:\n{role_play_session.user_sys_msg}\n"
-    )
-
-    print(Fore.YELLOW + f"Original task prompt:\n{task_prompt}\n")
-    print(
-        Fore.CYAN
-        + f"Specified task prompt:\n{role_play_session.specified_task_prompt}\n"
-    )
-    print(Fore.RED + f"Final task prompt:\n{role_play_session.task_prompt}\n")
-
-    n = 0
-    input_msg = role_play_session.init_chat()
-    while n < chat_turn_limit:
-        n += 1
-        assistant_response, user_response = role_play_session.step(input_msg)
-
-        if assistant_response.terminated:
-            print(
-                Fore.GREEN
-                + (
-                    "AI Assistant terminated. Reason: "
-                    f"{assistant_response.info['termination_reasons']}."
-                )
-            )
-            break
-        if user_response.terminated:
-            print(
-                Fore.GREEN
-                + (
-                    "AI User terminated. "
-                    f"Reason: {user_response.info['termination_reasons']}."
-                )
-            )
-            break
-
-        # Print output from the user
-        print_text_animated(
-            Fore.BLUE + f"AI User:\n\n{user_response.msg.content}\n"
-        )
-
-        # Print output from the assistant, including any function
-        # execution information
-        print_text_animated(Fore.GREEN + "AI Assistant:")
-        called_functions: List[FunctionCallingRecord] = assistant_response.info[
-            'called_functions'
-        ]
-        for func_record in called_functions:
-            print_text_animated(f"{func_record}")
-        print_text_animated(f"{assistant_response.msg.content}\n")
-
-        if "CAMEL_TASK_DONE" in user_response.msg.content:
-            break
-
-        input_msg = assistant_response.msg
```

### Comparing `camel_ai-0.1.3/camel/utils/token_counting.py` & `camel_ai-0.1.4/camel/utils/token_counting.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.3/pyproject.toml` & `camel_ai-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "camel-ai"
-version = "0.1.3"
+version = "0.1.4"
 authors = ["CAMEL-AI.org"]
 description = "Communicative Agents for AI Society Study"
 readme = "README.md"
 keywords = [
     "communicative-ai",
     "ai-societies",
     "artificial-intelligence",
@@ -26,15 +26,15 @@
 repository = "https://github.com/camel-ai/camel"
 documentation = "https://docs.camel-ai.org"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 numpy = "^1"
 openai = "^1.2.3"
-tiktoken = "^0"
+tiktoken = "^0.7.0"
 colorama = "^0"
 jsonschema = "^4"
 protobuf = "^4"
 pathlib = "^1.0.1"   
 anthropic = "^0.21.3"
 docstring-parser = "^0.15"
 pydantic = ">=1.9,<3"
@@ -54,28 +54,34 @@
 docx2txt = { version = "^0.8", optional = true }
 PyMuPDF = { version = "^1.22.5", optional = true }
 wikipedia = { version = "^1", optional = true }
 wolframalpha = { version = "^5.0.0", optional = true }
 pyowm = { version = "^3.3.0", optional = true }
 googlemaps = { version = "^4.10.0", optional = true }
 requests_oauthlib = { version = "^1.3.1", optional = true }
+prance = { version = "^23.6.21.0", optional = true }
+openapi-spec-validator = { version = "^0.7.1", optional = true }
 unstructured = { extras = ["all-docs"], version = "^0.10.30", optional = true }
+slack-sdk = { version = "^3.27.2", optional = true }
+pydub = { version = "^0.25.1", optional = true }
+pygithub = { version = "^2.3.0", optional = true }
 
 # encoders
 sentence-transformers = { version = "^2.2.2", optional = true }
 
 # vector-databases
 qdrant-client = { version = "^1.9.0", optional = true }
 pymilvus = { version = "^2.4.0", optional = true }
 
 # graph-storages
 neo4j = { version = "^5.18.0", optional = true }
 
 # retrievers
 rank-bm25 = { version = "^0.2.2", optional = true }
+cohere = { version = "^4.56", optional = true }
 
 # test
 pytest = { version = "^7", optional = true}
 mock = { version = "^5", optional = true}
 
 
 [tool.poetry.extras]
@@ -101,28 +107,34 @@
     "docx2txt",
     "PyMuPDF",
     "wikipedia",
     "wolframalpha",
     "pyowm",
     "googlemaps",
     "requests_oauthlib",
+    "prance",
+    "openapi-spec-validator",
     "unstructured",
+    "slack-sdk",
+    "pydub",
+    "pygithub",
 ]
 
 vector-databases = [
     "qdrant-client",
     "pymilvus",
 ]
 
 graph-storages = [
     "neo4j",
 ]
 
 retrievers = [
     "rank-bm25",
+    "cohere",
 ]
 
 all = [
     # huggingface-agent
     "transformers",
     "diffusers",
     "accelerate",
@@ -130,24 +142,31 @@
     "torch",
     "soundfile",
     "sentencepiece",
     "opencv-python",
     # tools
     "beautifulsoup4",
     "docx2txt",
+    "pygithub",
     "PyMuPDF",
     "wikipedia",
     "wolframalpha",
     "pyowm",
     "googlemaps",
     "requests_oauthlib",
+    "prance",
+    "openapi-spec-validator",
     "unstructured",
+    "slack-sdk",
+    "pydub",
     # vector-database
     "qdrant-client",
     "pymilvus",
+    # retrievers
+    "cohere",
     # encoders
     "sentence-transformers",
     # graph-storages
     "neo4j",
     # retrievers
     "rank-bm25",
 ]
@@ -240,19 +259,25 @@
     "huggingface_hub",
     "huggingface_hub.utils._errors",
     "wikipedia",
     "wolframalpha",
     "pyowm",
     "googlemaps",
     "requests_oauthlib",
+    "prance",
+    "openapi-spec-validator",
     "jsonschema.*",
     "bs4.*",
     "docx2txt",
     "PyMuPDF",
     "fitz",
     "qdrant_client.*",
     "unstructured.*",
     "rank_bm25",
+    "cohere",
     "sentence_transformers.*",
     "pymilvus",
+    "slack-sdk",
+    "pydub",
+    "pygithub"
 ]
 ignore_missing_imports = true
```

### Comparing `camel_ai-0.1.3/PKG-INFO` & `camel_ai-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6361 6d65  : 2.1.Name: came
 00000020: 6c2d 6169 0a56 6572 7369 6f6e 3a20 302e  l-ai.Version: 0.
-00000030: 312e 330a 5375 6d6d 6172 793a 2043 6f6d  1.3.Summary: Com
+00000030: 312e 340a 5375 6d6d 6172 793a 2043 6f6d  1.4.Summary: Com
 00000040: 6d75 6e69 6361 7469 7665 2041 6765 6e74  municative Agent
 00000050: 7320 666f 7220 4149 2053 6f63 6965 7479  s for AI Society
 00000060: 2053 7475 6479 0a48 6f6d 652d 7061 6765   Study.Home-page
 00000070: 3a20 6874 7470 733a 2f2f 7777 772e 6361  : https://www.ca
 00000080: 6d65 6c2d 6169 2e6f 7267 2f0a 4c69 6365  mel-ai.org/.Lice
 00000090: 6e73 653a 2041 7061 6368 652d 322e 300a  nse: Apache-2.0.
 000000a0: 4b65 7977 6f72 6473 3a20 636f 6d6d 756e  Keywords: commun
@@ -65,1230 +65,1261 @@
 00000400: 7374 3a20 616e 7468 726f 7069 6320 283e  st: anthropic (>
 00000410: 3d30 2e32 312e 332c 3c30 2e32 322e 3029  =0.21.3,<0.22.0)
 00000420: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
 00000430: 6265 6175 7469 6675 6c73 6f75 7034 2028  beautifulsoup4 (
 00000440: 3e3d 342c 3c35 2920 3b20 6578 7472 6120  >=4,<5) ; extra 
 00000450: 3d3d 2022 746f 6f6c 7322 206f 7220 6578  == "tools" or ex
 00000460: 7472 6120 3d3d 2022 616c 6c22 0a52 6571  tra == "all".Req
-00000470: 7569 7265 732d 4469 7374 3a20 636f 6c6f  uires-Dist: colo
-00000480: 7261 6d61 2028 3e3d 302c 3c31 290a 5265  rama (>=0,<1).Re
-00000490: 7175 6972 6573 2d44 6973 743a 2064 6174  quires-Dist: dat
-000004a0: 6173 6574 7320 283e 3d32 2c3c 3329 203b  asets (>=2,<3) ;
-000004b0: 2065 7874 7261 203d 3d20 2268 7567 6769   extra == "huggi
-000004c0: 6e67 6661 6365 2d61 6765 6e74 2220 6f72  ngface-agent" or
-000004d0: 2065 7874 7261 203d 3d20 2261 6c6c 220a   extra == "all".
-000004e0: 5265 7175 6972 6573 2d44 6973 743a 2064  Requires-Dist: d
-000004f0: 6966 6675 7365 7273 2028 3e3d 302c 3c31  iffusers (>=0,<1
-00000500: 2920 3b20 6578 7472 6120 3d3d 2022 6875  ) ; extra == "hu
-00000510: 6767 696e 6766 6163 652d 6167 656e 7422  ggingface-agent"
-00000520: 206f 7220 6578 7472 6120 3d3d 2022 616c   or extra == "al
-00000530: 6c22 0a52 6571 7569 7265 732d 4469 7374  l".Requires-Dist
-00000540: 3a20 646f 6373 7472 696e 672d 7061 7273  : docstring-pars
-00000550: 6572 2028 3e3d 302e 3135 2c3c 302e 3136  er (>=0.15,<0.16
-00000560: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
-00000570: 2064 6f63 7832 7478 7420 283e 3d30 2e38   docx2txt (>=0.8
-00000580: 2c3c 302e 3929 203b 2065 7874 7261 203d  ,<0.9) ; extra =
-00000590: 3d20 2274 6f6f 6c73 2220 6f72 2065 7874  = "tools" or ext
-000005a0: 7261 203d 3d20 2261 6c6c 220a 5265 7175  ra == "all".Requ
-000005b0: 6972 6573 2d44 6973 743a 2067 6f6f 676c  ires-Dist: googl
-000005c0: 656d 6170 7320 283e 3d34 2e31 302e 302c  emaps (>=4.10.0,
-000005d0: 3c35 2e30 2e30 2920 3b20 6578 7472 6120  <5.0.0) ; extra 
-000005e0: 3d3d 2022 746f 6f6c 7322 206f 7220 6578  == "tools" or ex
-000005f0: 7472 6120 3d3d 2022 616c 6c22 0a52 6571  tra == "all".Req
-00000600: 7569 7265 732d 4469 7374 3a20 6a73 6f6e  uires-Dist: json
-00000610: 7363 6865 6d61 2028 3e3d 342c 3c35 290a  schema (>=4,<5).
-00000620: 5265 7175 6972 6573 2d44 6973 743a 206d  Requires-Dist: m
-00000630: 6f63 6b20 283e 3d35 2c3c 3629 203b 2065  ock (>=5,<6) ; e
-00000640: 7874 7261 203d 3d20 2274 6573 7422 0a52  xtra == "test".R
-00000650: 6571 7569 7265 732d 4469 7374 3a20 6e65  equires-Dist: ne
-00000660: 6f34 6a20 283e 3d35 2e31 382e 302c 3c36  o4j (>=5.18.0,<6
-00000670: 2e30 2e30 2920 3b20 6578 7472 6120 3d3d  .0.0) ; extra ==
-00000680: 2022 6772 6170 682d 7374 6f72 6167 6573   "graph-storages
-00000690: 2220 6f72 2065 7874 7261 203d 3d20 2261  " or extra == "a
-000006a0: 6c6c 220a 5265 7175 6972 6573 2d44 6973  ll".Requires-Dis
-000006b0: 743a 206e 756d 7079 2028 3e3d 312c 3c32  t: numpy (>=1,<2
-000006c0: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
-000006d0: 206f 7065 6e61 6920 283e 3d31 2e32 2e33   openai (>=1.2.3
-000006e0: 2c3c 322e 302e 3029 0a52 6571 7569 7265  ,<2.0.0).Require
-000006f0: 732d 4469 7374 3a20 6f70 656e 6376 2d70  s-Dist: opencv-p
-00000700: 7974 686f 6e20 283e 3d34 2c3c 3529 203b  ython (>=4,<5) ;
-00000710: 2065 7874 7261 203d 3d20 2268 7567 6769   extra == "huggi
-00000720: 6e67 6661 6365 2d61 6765 6e74 2220 6f72  ngface-agent" or
-00000730: 2065 7874 7261 203d 3d20 2261 6c6c 220a   extra == "all".
-00000740: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
-00000750: 6174 686c 6962 2028 3e3d 312e 302e 312c  athlib (>=1.0.1,
-00000760: 3c32 2e30 2e30 290a 5265 7175 6972 6573  <2.0.0).Requires
-00000770: 2d44 6973 743a 2070 726f 746f 6275 6620  -Dist: protobuf 
-00000780: 283e 3d34 2c3c 3529 0a52 6571 7569 7265  (>=4,<5).Require
-00000790: 732d 4469 7374 3a20 7079 6461 6e74 6963  s-Dist: pydantic
-000007a0: 2028 3e3d 312e 392c 3c33 290a 5265 7175   (>=1.9,<3).Requ
-000007b0: 6972 6573 2d44 6973 743a 2070 796d 696c  ires-Dist: pymil
-000007c0: 7675 7320 283e 3d32 2e34 2e30 2c3c 332e  vus (>=2.4.0,<3.
-000007d0: 302e 3029 203b 2065 7874 7261 203d 3d20  0.0) ; extra == 
-000007e0: 2276 6563 746f 722d 6461 7461 6261 7365  "vector-database
-000007f0: 7322 206f 7220 6578 7472 6120 3d3d 2022  s" or extra == "
-00000800: 616c 6c22 0a52 6571 7569 7265 732d 4469  all".Requires-Di
-00000810: 7374 3a20 7079 6f77 6d20 283e 3d33 2e33  st: pyowm (>=3.3
-00000820: 2e30 2c3c 342e 302e 3029 203b 2065 7874  .0,<4.0.0) ; ext
-00000830: 7261 203d 3d20 2274 6f6f 6c73 2220 6f72  ra == "tools" or
-00000840: 2065 7874 7261 203d 3d20 2261 6c6c 220a   extra == "all".
-00000850: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
-00000860: 7974 6573 7420 283e 3d37 2c3c 3829 203b  ytest (>=7,<8) ;
-00000870: 2065 7874 7261 203d 3d20 2274 6573 7422   extra == "test"
-00000880: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000890: 7164 7261 6e74 2d63 6c69 656e 7420 283e  qdrant-client (>
-000008a0: 3d31 2e39 2e30 2c3c 322e 302e 3029 203b  =1.9.0,<2.0.0) ;
-000008b0: 2065 7874 7261 203d 3d20 2276 6563 746f   extra == "vecto
-000008c0: 722d 6461 7461 6261 7365 7322 206f 7220  r-databases" or 
-000008d0: 6578 7472 6120 3d3d 2022 616c 6c22 0a52  extra == "all".R
-000008e0: 6571 7569 7265 732d 4469 7374 3a20 7261  equires-Dist: ra
-000008f0: 6e6b 2d62 6d32 3520 283e 3d30 2e32 2e32  nk-bm25 (>=0.2.2
-00000900: 2c3c 302e 332e 3029 203b 2065 7874 7261  ,<0.3.0) ; extra
-00000910: 203d 3d20 2272 6574 7269 6576 6572 7322   == "retrievers"
-00000920: 206f 7220 6578 7472 6120 3d3d 2022 616c   or extra == "al
-00000930: 6c22 0a52 6571 7569 7265 732d 4469 7374  l".Requires-Dist
-00000940: 3a20 7265 7175 6573 7473 5f6f 6175 7468  : requests_oauth
-00000950: 6c69 6220 283e 3d31 2e33 2e31 2c3c 322e  lib (>=1.3.1,<2.
-00000960: 302e 3029 203b 2065 7874 7261 203d 3d20  0.0) ; extra == 
-00000970: 2274 6f6f 6c73 2220 6f72 2065 7874 7261  "tools" or extra
-00000980: 203d 3d20 2261 6c6c 220a 5265 7175 6972   == "all".Requir
-00000990: 6573 2d44 6973 743a 2073 656e 7465 6e63  es-Dist: sentenc
-000009a0: 652d 7472 616e 7366 6f72 6d65 7273 2028  e-transformers (
-000009b0: 3e3d 322e 322e 322c 3c33 2e30 2e30 2920  >=2.2.2,<3.0.0) 
-000009c0: 3b20 6578 7472 6120 3d3d 2022 656e 636f  ; extra == "enco
-000009d0: 6465 7273 2220 6f72 2065 7874 7261 203d  ders" or extra =
+00000470: 7569 7265 732d 4469 7374 3a20 636f 6865  uires-Dist: cohe
+00000480: 7265 2028 3e3d 342e 3536 2c3c 352e 3029  re (>=4.56,<5.0)
+00000490: 203b 2065 7874 7261 203d 3d20 2272 6574   ; extra == "ret
+000004a0: 7269 6576 6572 7322 206f 7220 6578 7472  rievers" or extr
+000004b0: 6120 3d3d 2022 616c 6c22 0a52 6571 7569  a == "all".Requi
+000004c0: 7265 732d 4469 7374 3a20 636f 6c6f 7261  res-Dist: colora
+000004d0: 6d61 2028 3e3d 302c 3c31 290a 5265 7175  ma (>=0,<1).Requ
+000004e0: 6972 6573 2d44 6973 743a 2064 6174 6173  ires-Dist: datas
+000004f0: 6574 7320 283e 3d32 2c3c 3329 203b 2065  ets (>=2,<3) ; e
+00000500: 7874 7261 203d 3d20 2268 7567 6769 6e67  xtra == "hugging
+00000510: 6661 6365 2d61 6765 6e74 2220 6f72 2065  face-agent" or e
+00000520: 7874 7261 203d 3d20 2261 6c6c 220a 5265  xtra == "all".Re
+00000530: 7175 6972 6573 2d44 6973 743a 2064 6966  quires-Dist: dif
+00000540: 6675 7365 7273 2028 3e3d 302c 3c31 2920  fusers (>=0,<1) 
+00000550: 3b20 6578 7472 6120 3d3d 2022 6875 6767  ; extra == "hugg
+00000560: 696e 6766 6163 652d 6167 656e 7422 206f  ingface-agent" o
+00000570: 7220 6578 7472 6120 3d3d 2022 616c 6c22  r extra == "all"
+00000580: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000590: 646f 6373 7472 696e 672d 7061 7273 6572  docstring-parser
+000005a0: 2028 3e3d 302e 3135 2c3c 302e 3136 290a   (>=0.15,<0.16).
+000005b0: 5265 7175 6972 6573 2d44 6973 743a 2064  Requires-Dist: d
+000005c0: 6f63 7832 7478 7420 283e 3d30 2e38 2c3c  ocx2txt (>=0.8,<
+000005d0: 302e 3929 203b 2065 7874 7261 203d 3d20  0.9) ; extra == 
+000005e0: 2274 6f6f 6c73 2220 6f72 2065 7874 7261  "tools" or extra
+000005f0: 203d 3d20 2261 6c6c 220a 5265 7175 6972   == "all".Requir
+00000600: 6573 2d44 6973 743a 2067 6f6f 676c 656d  es-Dist: googlem
+00000610: 6170 7320 283e 3d34 2e31 302e 302c 3c35  aps (>=4.10.0,<5
+00000620: 2e30 2e30 2920 3b20 6578 7472 6120 3d3d  .0.0) ; extra ==
+00000630: 2022 746f 6f6c 7322 206f 7220 6578 7472   "tools" or extr
+00000640: 6120 3d3d 2022 616c 6c22 0a52 6571 7569  a == "all".Requi
+00000650: 7265 732d 4469 7374 3a20 6a73 6f6e 7363  res-Dist: jsonsc
+00000660: 6865 6d61 2028 3e3d 342c 3c35 290a 5265  hema (>=4,<5).Re
+00000670: 7175 6972 6573 2d44 6973 743a 206d 6f63  quires-Dist: moc
+00000680: 6b20 283e 3d35 2c3c 3629 203b 2065 7874  k (>=5,<6) ; ext
+00000690: 7261 203d 3d20 2274 6573 7422 0a52 6571  ra == "test".Req
+000006a0: 7569 7265 732d 4469 7374 3a20 6e65 6f34  uires-Dist: neo4
+000006b0: 6a20 283e 3d35 2e31 382e 302c 3c36 2e30  j (>=5.18.0,<6.0
+000006c0: 2e30 2920 3b20 6578 7472 6120 3d3d 2022  .0) ; extra == "
+000006d0: 6772 6170 682d 7374 6f72 6167 6573 2220  graph-storages" 
+000006e0: 6f72 2065 7874 7261 203d 3d20 2261 6c6c  or extra == "all
+000006f0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000700: 206e 756d 7079 2028 3e3d 312c 3c32 290a   numpy (>=1,<2).
+00000710: 5265 7175 6972 6573 2d44 6973 743a 206f  Requires-Dist: o
+00000720: 7065 6e61 6920 283e 3d31 2e32 2e33 2c3c  penai (>=1.2.3,<
+00000730: 322e 302e 3029 0a52 6571 7569 7265 732d  2.0.0).Requires-
+00000740: 4469 7374 3a20 6f70 656e 6170 692d 7370  Dist: openapi-sp
+00000750: 6563 2d76 616c 6964 6174 6f72 2028 3e3d  ec-validator (>=
+00000760: 302e 372e 312c 3c30 2e38 2e30 2920 3b20  0.7.1,<0.8.0) ; 
+00000770: 6578 7472 6120 3d3d 2022 746f 6f6c 7322  extra == "tools"
+00000780: 206f 7220 6578 7472 6120 3d3d 2022 616c   or extra == "al
+00000790: 6c22 0a52 6571 7569 7265 732d 4469 7374  l".Requires-Dist
+000007a0: 3a20 6f70 656e 6376 2d70 7974 686f 6e20  : opencv-python 
+000007b0: 283e 3d34 2c3c 3529 203b 2065 7874 7261  (>=4,<5) ; extra
+000007c0: 203d 3d20 2268 7567 6769 6e67 6661 6365   == "huggingface
+000007d0: 2d61 6765 6e74 2220 6f72 2065 7874 7261  -agent" or extra
+000007e0: 203d 3d20 2261 6c6c 220a 5265 7175 6972   == "all".Requir
+000007f0: 6573 2d44 6973 743a 2070 6174 686c 6962  es-Dist: pathlib
+00000800: 2028 3e3d 312e 302e 312c 3c32 2e30 2e30   (>=1.0.1,<2.0.0
+00000810: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
+00000820: 2070 7261 6e63 6520 283e 3d32 332e 362e   prance (>=23.6.
+00000830: 3231 2e30 2c3c 3234 2e30 2e30 2e30 2920  21.0,<24.0.0.0) 
+00000840: 3b20 6578 7472 6120 3d3d 2022 746f 6f6c  ; extra == "tool
+00000850: 7322 206f 7220 6578 7472 6120 3d3d 2022  s" or extra == "
+00000860: 616c 6c22 0a52 6571 7569 7265 732d 4469  all".Requires-Di
+00000870: 7374 3a20 7072 6f74 6f62 7566 2028 3e3d  st: protobuf (>=
+00000880: 342c 3c35 290a 5265 7175 6972 6573 2d44  4,<5).Requires-D
+00000890: 6973 743a 2070 7964 616e 7469 6320 283e  ist: pydantic (>
+000008a0: 3d31 2e39 2c3c 3329 0a52 6571 7569 7265  =1.9,<3).Require
+000008b0: 732d 4469 7374 3a20 7079 6475 6220 283e  s-Dist: pydub (>
+000008c0: 3d30 2e32 352e 312c 3c30 2e32 362e 3029  =0.25.1,<0.26.0)
+000008d0: 203b 2065 7874 7261 203d 3d20 2274 6f6f   ; extra == "too
+000008e0: 6c73 2220 6f72 2065 7874 7261 203d 3d20  ls" or extra == 
+000008f0: 2261 6c6c 220a 5265 7175 6972 6573 2d44  "all".Requires-D
+00000900: 6973 743a 2070 7967 6974 6875 6220 283e  ist: pygithub (>
+00000910: 3d32 2e33 2e30 2c3c 332e 302e 3029 203b  =2.3.0,<3.0.0) ;
+00000920: 2065 7874 7261 203d 3d20 2274 6f6f 6c73   extra == "tools
+00000930: 2220 6f72 2065 7874 7261 203d 3d20 2261  " or extra == "a
+00000940: 6c6c 220a 5265 7175 6972 6573 2d44 6973  ll".Requires-Dis
+00000950: 743a 2070 796d 696c 7675 7320 283e 3d32  t: pymilvus (>=2
+00000960: 2e34 2e30 2c3c 332e 302e 3029 203b 2065  .4.0,<3.0.0) ; e
+00000970: 7874 7261 203d 3d20 2276 6563 746f 722d  xtra == "vector-
+00000980: 6461 7461 6261 7365 7322 206f 7220 6578  databases" or ex
+00000990: 7472 6120 3d3d 2022 616c 6c22 0a52 6571  tra == "all".Req
+000009a0: 7569 7265 732d 4469 7374 3a20 7079 6f77  uires-Dist: pyow
+000009b0: 6d20 283e 3d33 2e33 2e30 2c3c 342e 302e  m (>=3.3.0,<4.0.
+000009c0: 3029 203b 2065 7874 7261 203d 3d20 2274  0) ; extra == "t
+000009d0: 6f6f 6c73 2220 6f72 2065 7874 7261 203d  ools" or extra =
 000009e0: 3d20 2261 6c6c 220a 5265 7175 6972 6573  = "all".Requires
-000009f0: 2d44 6973 743a 2073 656e 7465 6e63 6570  -Dist: sentencep
-00000a00: 6965 6365 2028 3e3d 302c 3c31 2920 3b20  iece (>=0,<1) ; 
-00000a10: 6578 7472 6120 3d3d 2022 6875 6767 696e  extra == "huggin
-00000a20: 6766 6163 652d 6167 656e 7422 206f 7220  gface-agent" or 
-00000a30: 6578 7472 6120 3d3d 2022 616c 6c22 0a52  extra == "all".R
-00000a40: 6571 7569 7265 732d 4469 7374 3a20 736f  equires-Dist: so
-00000a50: 756e 6466 696c 6520 283e 3d30 2c3c 3129  undfile (>=0,<1)
-00000a60: 203b 2065 7874 7261 203d 3d20 2268 7567   ; extra == "hug
-00000a70: 6769 6e67 6661 6365 2d61 6765 6e74 2220  gingface-agent" 
-00000a80: 6f72 2065 7874 7261 203d 3d20 2261 6c6c  or extra == "all
-00000a90: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-00000aa0: 2074 696b 746f 6b65 6e20 283e 3d30 2c3c   tiktoken (>=0,<
-00000ab0: 3129 0a52 6571 7569 7265 732d 4469 7374  1).Requires-Dist
-00000ac0: 3a20 746f 7263 6820 283e 3d31 2c3c 3229  : torch (>=1,<2)
-00000ad0: 203b 2065 7874 7261 203d 3d20 2268 7567   ; extra == "hug
-00000ae0: 6769 6e67 6661 6365 2d61 6765 6e74 2220  gingface-agent" 
-00000af0: 6f72 2065 7874 7261 203d 3d20 2261 6c6c  or extra == "all
-00000b00: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-00000b10: 2074 7261 6e73 666f 726d 6572 7320 283e   transformers (>
-00000b20: 3d34 2c3c 3529 203b 2065 7874 7261 203d  =4,<5) ; extra =
-00000b30: 3d20 2268 7567 6769 6e67 6661 6365 2d61  = "huggingface-a
-00000b40: 6765 6e74 2220 6f72 2065 7874 7261 203d  gent" or extra =
-00000b50: 3d20 2261 6c6c 220a 5265 7175 6972 6573  = "all".Requires
-00000b60: 2d44 6973 743a 2075 6e73 7472 7563 7475  -Dist: unstructu
-00000b70: 7265 645b 616c 6c2d 646f 6373 5d20 283e  red[all-docs] (>
-00000b80: 3d30 2e31 302e 3330 2c3c 302e 3131 2e30  =0.10.30,<0.11.0
-00000b90: 2920 3b20 6578 7472 6120 3d3d 2022 746f  ) ; extra == "to
-00000ba0: 6f6c 7322 206f 7220 6578 7472 6120 3d3d  ols" or extra ==
-00000bb0: 2022 616c 6c22 0a52 6571 7569 7265 732d   "all".Requires-
-00000bc0: 4469 7374 3a20 7769 6b69 7065 6469 6120  Dist: wikipedia 
-00000bd0: 283e 3d31 2c3c 3229 203b 2065 7874 7261  (>=1,<2) ; extra
-00000be0: 203d 3d20 2274 6f6f 6c73 2220 6f72 2065   == "tools" or e
-00000bf0: 7874 7261 203d 3d20 2261 6c6c 220a 5265  xtra == "all".Re
-00000c00: 7175 6972 6573 2d44 6973 743a 2077 6f6c  quires-Dist: wol
-00000c10: 6672 616d 616c 7068 6120 283e 3d35 2e30  framalpha (>=5.0
-00000c20: 2e30 2c3c 362e 302e 3029 203b 2065 7874  .0,<6.0.0) ; ext
-00000c30: 7261 203d 3d20 2274 6f6f 6c73 2220 6f72  ra == "tools" or
-00000c40: 2065 7874 7261 203d 3d20 2261 6c6c 220a   extra == "all".
-00000c50: 5072 6f6a 6563 742d 5552 4c3a 2044 6f63  Project-URL: Doc
-00000c60: 756d 656e 7461 7469 6f6e 2c20 6874 7470  umentation, http
-00000c70: 733a 2f2f 646f 6373 2e63 616d 656c 2d61  s://docs.camel-a
-00000c80: 692e 6f72 670a 5072 6f6a 6563 742d 5552  i.org.Project-UR
-00000c90: 4c3a 2052 6570 6f73 6974 6f72 792c 2068  L: Repository, h
-00000ca0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000cb0: 6d2f 6361 6d65 6c2d 6169 2f63 616d 656c  m/camel-ai/camel
-00000cc0: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
-00000cd0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
-00000ce0: 6d61 726b 646f 776e 0a0a 5b21 5b43 6f6c  markdown..[![Col
-00000cf0: 6162 5d5b 636f 6c61 622d 696d 6167 655d  ab][colab-image]
-00000d00: 5d5b 636f 6c61 622d 7572 6c5d 0a5b 215b  ][colab-url].[![
-00000d10: 4875 6767 696e 6720 4661 6365 5d5b 6875  Hugging Face][hu
-00000d20: 6767 696e 6766 6163 652d 696d 6167 655d  ggingface-image]
-00000d30: 5d5b 6875 6767 696e 6766 6163 652d 7572  ][huggingface-ur
-00000d40: 6c5d 0a5b 215b 536c 6163 6b5d 5b73 6c61  l].[![Slack][sla
-00000d50: 636b 2d69 6d61 6765 5d5d 5b73 6c61 636b  ck-image]][slack
-00000d60: 2d75 726c 5d0a 5b21 5b44 6973 636f 7264  -url].[![Discord
-00000d70: 5d5b 6469 7363 6f72 642d 696d 6167 655d  ][discord-image]
-00000d80: 5d5b 6469 7363 6f72 642d 7572 6c5d 0a5b  ][discord-url].[
-00000d90: 215b 5765 6368 6174 5d5b 7765 6368 6174  ![Wechat][wechat
-00000da0: 2d69 6d61 6765 5d5d 5b77 6563 6861 742d  -image]][wechat-
-00000db0: 7572 6c5d 0a5b 215b 5477 6974 7465 725d  url].[![Twitter]
-00000dc0: 5b74 7769 7474 6572 2d69 6d61 6765 5d5d  [twitter-image]]
-00000dd0: 5b74 7769 7474 6572 2d75 726c 5d0a 0a5f  [twitter-url].._
-00000de0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00000df0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00000e00: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00000e10: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
-00000e20: 5f5f 5f5f 5f0a 0a23 2043 414d 454c 3a20  _____..# CAMEL: 
-00000e30: 436f 6d6d 756e 6963 6174 6976 6520 4167  Communicative Ag
-00000e40: 656e 7473 2066 6f72 20e2 809c 4d69 6e64  ents for ...Mind
-00000e50: e280 9d20 4578 706c 6f72 6174 696f 6e20  ... Exploration 
-00000e60: 6f66 204c 6172 6765 204c 616e 6775 6167  of Large Languag
-00000e70: 6520 4d6f 6465 6c20 536f 6369 6574 790a  e Model Society.
-00000e80: 0a5b 215b 5079 7468 6f6e 2056 6572 7369  .[![Python Versi
-00000e90: 6f6e 5d5b 7079 7468 6f6e 2d69 6d61 6765  on][python-image
-00000ea0: 5d5d 5b70 7974 686f 6e2d 7572 6c5d 0a5b  ]][python-url].[
-00000eb0: 215b 5079 5465 7374 2053 7461 7475 735d  ![PyTest Status]
-00000ec0: 5b70 7974 6573 742d 696d 6167 655d 5d5b  [pytest-image]][
-00000ed0: 7079 7465 7374 2d75 726c 5d0a 5b21 5b44  pytest-url].[![D
-00000ee0: 6f63 756d 656e 7461 7469 6f6e 5d5b 646f  ocumentation][do
-00000ef0: 6373 2d69 6d61 6765 5d5d 5b64 6f63 732d  cs-image]][docs-
-00000f00: 7572 6c5d 0a5b 215b 5374 6172 5d5b 7374  url].[![Star][st
-00000f10: 6172 2d69 6d61 6765 5d5d 5b73 7461 722d  ar-image]][star-
-00000f20: 7572 6c5d 0a5b 215b 5061 636b 6167 6520  url].[![Package 
-00000f30: 4c69 6365 6e73 655d 5b70 6163 6b61 6765  License][package
-00000f40: 2d6c 6963 656e 7365 2d69 6d61 6765 5d5d  -license-image]]
-00000f50: 5b70 6163 6b61 6765 2d6c 6963 656e 7365  [package-license
-00000f60: 2d75 726c 5d0a 5b21 5b44 6174 6120 4c69  -url].[![Data Li
-00000f70: 6365 6e73 655d 5b64 6174 612d 6c69 6365  cense][data-lice
-00000f80: 6e73 652d 696d 6167 655d 5d5b 6461 7461  nse-image]][data
-00000f90: 2d6c 6963 656e 7365 2d75 726c 5d0a 0a3c  -license-url]..<
-00000fa0: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
-00000fb0: 3e0a 2020 3c61 2068 7265 663d 2268 7474  >.  <a href="htt
-00000fc0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000fd0: 6361 6d65 6c2d 6169 2f63 616d 656c 2363  camel-ai/camel#c
-00000fe0: 6f6d 6d75 6e69 7479 223e 436f 6d6d 756e  ommunity">Commun
-00000ff0: 6974 793c 2f61 3e20 7c0a 2020 3c61 2068  ity</a> |.  <a h
-00001000: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-00001010: 6875 622e 636f 6d2f 6361 6d65 6c2d 6169  hub.com/camel-ai
-00001020: 2f63 616d 656c 2369 6e73 7461 6c6c 6174  /camel#installat
-00001030: 696f 6e22 3e49 6e73 7461 6c6c 6174 696f  ion">Installatio
-00001040: 6e3c 2f61 3e20 7c0a 2020 3c61 2068 7265  n</a> |.  <a hre
-00001050: 663d 2268 7474 7073 3a2f 2f63 616d 656c  f="https://camel
-00001060: 2d61 692e 6769 7468 7562 2e69 6f2f 6361  -ai.github.io/ca
-00001070: 6d65 6c2f 223e 446f 6375 6d65 6e74 6174  mel/">Documentat
-00001080: 696f 6e3c 2f61 3e20 7c0a 2020 3c61 2068  ion</a> |.  <a h
-00001090: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
-000010a0: 6875 622e 636f 6d2f 6361 6d65 6c2d 6169  hub.com/camel-ai
-000010b0: 2f63 616d 656c 2f74 7265 652f 4845 4144  /camel/tree/HEAD
-000010c0: 2f65 7861 6d70 6c65 7322 3e45 7861 6d70  /examples">Examp
-000010d0: 6c65 733c 2f61 3e20 7c0a 2020 3c61 2068  les</a> |.  <a h
-000010e0: 7265 663d 2268 7474 7073 3a2f 2f61 7278  ref="https://arx
-000010f0: 6976 2e6f 7267 2f61 6273 2f32 3330 332e  iv.org/abs/2303.
-00001100: 3137 3736 3022 3e50 6170 6572 3c2f 613e  17760">Paper</a>
-00001110: 207c 0a20 203c 6120 6872 6566 3d22 6874   |.  <a href="ht
-00001120: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001130: 2f63 616d 656c 2d61 692f 6361 6d65 6c23  /camel-ai/camel#
-00001140: 6369 7461 7469 6f6e 223e 4369 7461 7469  citation">Citati
-00001150: 6f6e 3c2f 613e 207c 0a20 203c 6120 6872  on</a> |.  <a hr
-00001160: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-00001170: 7562 2e63 6f6d 2f63 616d 656c 2d61 692f  ub.com/camel-ai/
-00001180: 6361 6d65 6c23 636f 6e74 7269 6275 7469  camel#contributi
-00001190: 6e67 2d74 6f2d 6361 6d65 6c2d 223e 436f  ng-to-camel-">Co
-000011a0: 6e74 7269 6275 7469 6e67 3c2f 613e 207c  ntributing</a> |
-000011b0: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
-000011c0: 733a 2f2f 7777 772e 6361 6d65 6c2d 6169  s://www.camel-ai
-000011d0: 2e6f 7267 2f22 3e43 414d 454c 2d41 493c  .org/">CAMEL-AI<
-000011e0: 2f61 3e0a 3c2f 703e 0a0a 3c70 2061 6c69  /a>.</p>..<p ali
-000011f0: 676e 3d22 6365 6e74 6572 223e 0a20 203c  gn="center">.  <
-00001200: 696d 6720 7372 633d 2768 7474 7073 3a2f  img src='https:/
-00001210: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-00001220: 6f6e 7465 6e74 2e63 6f6d 2f63 616d 656c  ontent.com/camel
-00001230: 2d61 692f 6361 6d65 6c2f 6d61 7374 6572  -ai/camel/master
-00001240: 2f6d 6973 632f 7072 696d 6172 795f 6c6f  /misc/primary_lo
-00001250: 676f 2e70 6e67 2720 7769 6474 683d 3830  go.png' width=80
-00001260: 303e 0a3c 2f70 3e0a 0a23 2320 4f76 6572  0>.</p>..## Over
-00001270: 7669 6577 0a54 6865 2072 6170 6964 2061  view.The rapid a
-00001280: 6476 616e 6365 6d65 6e74 206f 6620 636f  dvancement of co
-00001290: 6e76 6572 7361 7469 6f6e 616c 2061 6e64  nversational and
-000012a0: 2063 6861 742d 6261 7365 6420 6c61 6e67   chat-based lang
-000012b0: 7561 6765 206d 6f64 656c 7320 6861 7320  uage models has 
-000012c0: 6c65 6420 746f 2072 656d 6172 6b61 626c  led to remarkabl
-000012d0: 6520 7072 6f67 7265 7373 2069 6e20 636f  e progress in co
-000012e0: 6d70 6c65 7820 7461 736b 2d73 6f6c 7669  mplex task-solvi
-000012f0: 6e67 2e20 486f 7765 7665 722c 2074 6865  ng. However, the
-00001300: 6972 2073 7563 6365 7373 2068 6561 7669  ir success heavi
-00001310: 6c79 2072 656c 6965 7320 6f6e 2068 756d  ly relies on hum
-00001320: 616e 2069 6e70 7574 2074 6f20 6775 6964  an input to guid
-00001330: 6520 7468 6520 636f 6e76 6572 7361 7469  e the conversati
-00001340: 6f6e 2c20 7768 6963 6820 6361 6e20 6265  on, which can be
-00001350: 2063 6861 6c6c 656e 6769 6e67 2061 6e64   challenging and
-00001360: 2074 696d 652d 636f 6e73 756d 696e 672e   time-consuming.
-00001370: 2054 6869 7320 7061 7065 7220 6578 706c   This paper expl
-00001380: 6f72 6573 2074 6865 2070 6f74 656e 7469  ores the potenti
-00001390: 616c 206f 6620 6275 696c 6469 6e67 2073  al of building s
-000013a0: 6361 6c61 626c 6520 7465 6368 6e69 7175  calable techniqu
-000013b0: 6573 2074 6f20 6661 6369 6c69 7461 7465  es to facilitate
-000013c0: 2061 7574 6f6e 6f6d 6f75 7320 636f 6f70   autonomous coop
-000013d0: 6572 6174 696f 6e20 616d 6f6e 6720 636f  eration among co
-000013e0: 6d6d 756e 6963 6174 6976 6520 6167 656e  mmunicative agen
-000013f0: 7473 2061 6e64 2070 726f 7669 6465 2069  ts and provide i
-00001400: 6e73 6967 6874 2069 6e74 6f20 7468 6569  nsight into thei
-00001410: 7220 2263 6f67 6e69 7469 7665 2220 7072  r "cognitive" pr
-00001420: 6f63 6573 7365 732e 2054 6f20 6164 6472  ocesses. To addr
-00001430: 6573 7320 7468 6520 6368 616c 6c65 6e67  ess the challeng
-00001440: 6573 206f 6620 6163 6869 6576 696e 6720  es of achieving 
-00001450: 6175 746f 6e6f 6d6f 7573 2063 6f6f 7065  autonomous coope
-00001460: 7261 7469 6f6e 2c20 7765 2070 726f 706f  ration, we propo
-00001470: 7365 2061 206e 6f76 656c 2063 6f6d 6d75  se a novel commu
-00001480: 6e69 6361 7469 7665 2061 6765 6e74 2066  nicative agent f
-00001490: 7261 6d65 776f 726b 206e 616d 6564 202a  ramework named *
-000014a0: 726f 6c65 2d70 6c61 7969 6e67 2a2e 204f  role-playing*. O
-000014b0: 7572 2061 7070 726f 6163 6820 696e 766f  ur approach invo
-000014c0: 6c76 6573 2075 7369 6e67 202a 696e 6365  lves using *ince
-000014d0: 7074 696f 6e20 7072 6f6d 7074 696e 672a  ption prompting*
-000014e0: 2074 6f20 6775 6964 6520 6368 6174 2061   to guide chat a
-000014f0: 6765 6e74 7320 746f 7761 7264 2074 6173  gents toward tas
-00001500: 6b20 636f 6d70 6c65 7469 6f6e 2077 6869  k completion whi
-00001510: 6c65 206d 6169 6e74 6169 6e69 6e67 2063  le maintaining c
-00001520: 6f6e 7369 7374 656e 6379 2077 6974 6820  onsistency with 
-00001530: 6875 6d61 6e20 696e 7465 6e74 696f 6e73  human intentions
-00001540: 2e20 5765 2073 686f 7763 6173 6520 686f  . We showcase ho
-00001550: 7720 726f 6c65 2d70 6c61 7969 6e67 2063  w role-playing c
-00001560: 616e 2062 6520 7573 6564 2074 6f20 6765  an be used to ge
-00001570: 6e65 7261 7465 2063 6f6e 7665 7273 6174  nerate conversat
-00001580: 696f 6e61 6c20 6461 7461 2066 6f72 2073  ional data for s
-00001590: 7475 6479 696e 6720 7468 6520 6265 6861  tudying the beha
-000015a0: 7669 6f72 7320 616e 6420 6361 7061 6269  viors and capabi
-000015b0: 6c69 7469 6573 206f 6620 6368 6174 2061  lities of chat a
-000015c0: 6765 6e74 732c 2070 726f 7669 6469 6e67  gents, providing
-000015d0: 2061 2076 616c 7561 626c 6520 7265 736f   a valuable reso
-000015e0: 7572 6365 2066 6f72 2069 6e76 6573 7469  urce for investi
-000015f0: 6761 7469 6e67 2063 6f6e 7665 7273 6174  gating conversat
-00001600: 696f 6e61 6c20 6c61 6e67 7561 6765 206d  ional language m
-00001610: 6f64 656c 732e 204f 7572 2063 6f6e 7472  odels. Our contr
-00001620: 6962 7574 696f 6e73 2069 6e63 6c75 6465  ibutions include
-00001630: 2069 6e74 726f 6475 6369 6e67 2061 206e   introducing a n
-00001640: 6f76 656c 2063 6f6d 6d75 6e69 6361 7469  ovel communicati
-00001650: 7665 2061 6765 6e74 2066 7261 6d65 776f  ve agent framewo
-00001660: 726b 2c20 6f66 6665 7269 6e67 2061 2073  rk, offering a s
-00001670: 6361 6c61 626c 6520 6170 7072 6f61 6368  calable approach
-00001680: 2066 6f72 2073 7475 6479 696e 6720 7468   for studying th
-00001690: 6520 636f 6f70 6572 6174 6976 6520 6265  e cooperative be
-000016a0: 6861 7669 6f72 7320 616e 6420 6361 7061  haviors and capa
-000016b0: 6269 6c69 7469 6573 206f 6620 6d75 6c74  bilities of mult
-000016c0: 692d 6167 656e 7420 7379 7374 656d 732c  i-agent systems,
-000016d0: 2061 6e64 206f 7065 6e2d 736f 7572 6369   and open-sourci
-000016e0: 6e67 206f 7572 206c 6962 7261 7279 2074  ng our library t
-000016f0: 6f20 7375 7070 6f72 7420 7265 7365 6172  o support resear
-00001700: 6368 206f 6e20 636f 6d6d 756e 6963 6174  ch on communicat
-00001710: 6976 6520 6167 656e 7473 2061 6e64 2062  ive agents and b
-00001720: 6579 6f6e 642e 2054 6865 2047 6974 4875  eyond. The GitHu
-00001730: 6220 7265 706f 7369 746f 7279 206f 6620  b repository of 
-00001740: 7468 6973 2070 726f 6a65 6374 2069 7320  this project is 
-00001750: 6d61 6465 2070 7562 6c69 636c 7920 6176  made publicly av
-00001760: 6169 6c61 626c 6520 6f6e 3a20 5b68 7474  ailable on: [htt
-00001770: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001780: 6361 6d65 6c2d 6169 2f63 616d 656c 5d28  camel-ai/camel](
-00001790: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000017a0: 6f6d 2f63 616d 656c 2d61 692f 6361 6d65  om/camel-ai/came
-000017b0: 6c29 2e0a 0a23 2320 436f 6d6d 756e 6974  l)...## Communit
-000017c0: 790a f09f 90ab 2043 414d 454c 2069 7320  y..... CAMEL is 
-000017d0: 616e 206f 7065 6e2d 736f 7572 6365 206c  an open-source l
-000017e0: 6962 7261 7279 2064 6573 6967 6e65 6420  ibrary designed 
-000017f0: 666f 7220 7468 6520 7374 7564 7920 6f66  for the study of
-00001800: 2061 7574 6f6e 6f6d 6f75 7320 616e 6420   autonomous and 
-00001810: 636f 6d6d 756e 6963 6174 6976 6520 6167  communicative ag
-00001820: 656e 7473 2e20 5765 2062 656c 6965 7665  ents. We believe
-00001830: 2074 6861 7420 7374 7564 7969 6e67 2074   that studying t
-00001840: 6865 7365 2061 6765 6e74 7320 6f6e 2061  hese agents on a
-00001850: 206c 6172 6765 2073 6361 6c65 206f 6666   large scale off
-00001860: 6572 7320 7661 6c75 6162 6c65 2069 6e73  ers valuable ins
-00001870: 6967 6874 7320 696e 746f 2074 6865 6972  ights into their
-00001880: 2062 6568 6176 696f 7273 2c20 6361 7061   behaviors, capa
-00001890: 6269 6c69 7469 6573 2c20 616e 6420 706f  bilities, and po
-000018a0: 7465 6e74 6961 6c20 7269 736b 732e 2054  tential risks. T
-000018b0: 6f20 6661 6369 6c69 7461 7465 2072 6573  o facilitate res
-000018c0: 6561 7263 6820 696e 2074 6869 7320 6669  earch in this fi
-000018d0: 656c 642c 2077 6520 696d 706c 656d 656e  eld, we implemen
-000018e0: 7420 616e 6420 7375 7070 6f72 7420 7661  t and support va
-000018f0: 7269 6f75 7320 7479 7065 7320 6f66 2061  rious types of a
-00001900: 6765 6e74 732c 2074 6173 6b73 2c20 7072  gents, tasks, pr
-00001910: 6f6d 7074 732c 206d 6f64 656c 732c 2061  ompts, models, a
-00001920: 6e64 2073 696d 756c 6174 6564 2065 6e76  nd simulated env
-00001930: 6972 6f6e 6d65 6e74 732e 0a0a 4a6f 696e  ironments...Join
-00001940: 2075 7320 285b 2a53 6c61 636b 2a5d 2868   us ([*Slack*](h
-00001950: 7474 7073 3a2f 2f6a 6f69 6e2e 736c 6163  ttps://join.slac
-00001960: 6b2e 636f 6d2f 742f 6361 6d65 6c2d 6169  k.com/t/camel-ai
-00001970: 2f73 6861 7265 645f 696e 7669 7465 2f7a  /shared_invite/z
-00001980: 742d 3267 3778 6334 3167 792d 5f37 7263  t-2g7xc41gy-_7rc
-00001990: 724e 4e41 4172 4950 3673 4c51 716c 646b  rNNAArIP6sLQqldk
-000019a0: 7151 292c 205b 2a44 6973 636f 7264 2a5d  qQ), [*Discord*]
-000019b0: 2868 7474 7073 3a2f 2f64 6973 636f 7264  (https://discord
-000019c0: 2e67 672f 434e 634e 7071 7579 4463 2920  .gg/CNcNpquyDc) 
-000019d0: 6f72 205b 2a57 6543 6861 742a 5d28 6874  or [*WeChat*](ht
-000019e0: 7470 733a 2f2f 6768 6c69 2e6f 7267 2f63  tps://ghli.org/c
-000019f0: 616d 656c 2f77 6563 6861 742e 706e 6729  amel/wechat.png)
-00001a00: 2920 696e 2070 7573 6869 6e67 2074 6865  ) in pushing the
-00001a10: 2062 6f75 6e64 6172 6965 7320 6f66 2062   boundaries of b
-00001a20: 7569 6c64 696e 6720 4149 2053 6f63 6965  uilding AI Socie
-00001a30: 7479 2e0a 0a23 2320 5472 7920 6974 2079  ty...## Try it y
-00001a40: 6f75 7273 656c 660a 5765 2070 726f 7669  ourself.We provi
-00001a50: 6465 2061 205b 215b 476f 6f67 6c65 2043  de a [![Google C
-00001a60: 6f6c 6162 5d28 6874 7470 733a 2f2f 636f  olab](https://co
-00001a70: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
-00001a80: 676c 652e 636f 6d2f 6173 7365 7473 2f63  gle.com/assets/c
-00001a90: 6f6c 6162 2d62 6164 6765 2e73 7667 295d  olab-badge.svg)]
-00001aa0: 2868 7474 7073 3a2f 2f63 6f6c 6162 2e72  (https://colab.r
-00001ab0: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
-00001ac0: 6f6d 2f64 7269 7665 2f31 417a 5033 334f  om/drive/1AzP33O
-00001ad0: 3872 6e4d 575f 5f37 6f63 574a 6856 4258  8rnMW__7ocWJhVBX
-00001ae0: 6a4b 7a69 4a58 5074 696d 3f75 7370 3d73  jKziJXPtim?usp=s
-00001af0: 6861 7269 6e67 2920 6465 6d6f 2073 686f  haring) demo sho
-00001b00: 7763 6173 696e 6720 6120 636f 6e76 6572  wcasing a conver
-00001b10: 7361 7469 6f6e 2062 6574 7765 656e 2074  sation between t
-00001b20: 776f 2043 6861 7447 5054 2061 6765 6e74  wo ChatGPT agent
-00001b30: 7320 706c 6179 696e 6720 726f 6c65 7320  s playing roles 
-00001b40: 6173 2061 2070 7974 686f 6e20 7072 6f67  as a python prog
-00001b50: 7261 6d6d 6572 2061 6e64 2061 2073 746f  rammer and a sto
-00001b60: 636b 2074 7261 6465 7220 636f 6c6c 6162  ck trader collab
-00001b70: 6f72 6174 696e 6720 6f6e 2064 6576 656c  orating on devel
-00001b80: 6f70 696e 6720 6120 7472 6164 696e 6720  oping a trading 
-00001b90: 626f 7420 666f 7220 7374 6f63 6b20 6d61  bot for stock ma
-00001ba0: 726b 6574 2e0a 0a3c 7020 616c 6967 6e3d  rket...<p align=
-00001bb0: 2263 656e 7465 7222 3e0a 2020 3c69 6d67  "center">.  <img
-00001bc0: 2073 7263 3d27 6874 7470 733a 2f2f 7261   src='https://ra
-00001bd0: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-00001be0: 656e 742e 636f 6d2f 6361 6d65 6c2d 6169  ent.com/camel-ai
-00001bf0: 2f63 616d 656c 2f6d 6173 7465 722f 6d69  /camel/master/mi
-00001c00: 7363 2f66 7261 6d65 776f 726b 2e70 6e67  sc/framework.png
-00001c10: 2720 7769 6474 683d 3830 303e 0a3c 2f70  ' width=800>.</p
-00001c20: 3e0a 0a23 2320 496e 7374 616c 6c61 7469  >..## Installati
-00001c30: 6f6e 0a0a 2323 2320 4672 6f6d 2050 7950  on..### From PyP
-00001c40: 490a 0a54 6f20 696e 7374 616c 6c20 7468  I..To install th
-00001c50: 6520 6261 7365 2043 414d 454c 206c 6962  e base CAMEL lib
-00001c60: 7261 7279 3a0a 6060 6062 6173 680a 7069  rary:.```bash.pi
-00001c70: 7020 696e 7374 616c 6c20 6361 6d65 6c2d  p install camel-
-00001c80: 6169 0a60 6060 0a53 6f6d 6520 6665 6174  ai.```.Some feat
-00001c90: 7572 6573 2072 6571 7569 7265 2065 7874  ures require ext
-00001ca0: 7261 2064 6570 656e 6465 6e63 6965 733a  ra dependencies:
-00001cb0: 0a2d 2054 6f20 7573 6520 7468 6520 4875  .- To use the Hu
-00001cc0: 6767 696e 6746 6163 6520 6167 656e 7473  ggingFace agents
-00001cd0: 3a0a 2020 2020 6060 6062 6173 680a 2020  :.    ```bash.  
-00001ce0: 2020 7069 7020 696e 7374 616c 6c20 2763    pip install 'c
-00001cf0: 616d 656c 2d61 695b 6875 6767 696e 6766  amel-ai[huggingf
-00001d00: 6163 652d 6167 656e 745d 270a 2020 2020  ace-agent]'.    
-00001d10: 6060 600a 2d20 546f 2065 6e61 626c 6520  ```.- To enable 
-00001d20: 5241 4720 6f72 2075 7365 2061 6765 6e74  RAG or use agent
-00001d30: 206d 656d 6f72 793a 0a20 2020 2060 6060   memory:.    ```
-00001d40: 6261 7368 0a20 2020 2070 6970 2069 6e73  bash.    pip ins
-00001d50: 7461 6c6c 2027 6361 6d65 6c2d 6169 5b74  tall 'camel-ai[t
-00001d60: 6f6f 6c73 5d27 0a20 2020 2060 6060 0a2d  ools]'.    ```.-
-00001d70: 2054 6f20 696e 7374 616c 6c20 7769 7468   To install with
-00001d80: 2061 6c6c 2064 6570 656e 6465 6e63 6965   all dependencie
-00001d90: 733a 0a20 2020 2060 6060 6261 7368 0a20  s:.    ```bash. 
-00001da0: 2020 2070 6970 2069 6e73 7461 6c6c 2027     pip install '
-00001db0: 6361 6d65 6c2d 6169 5b61 6c6c 5d27 0a20  camel-ai[all]'. 
-00001dc0: 2020 2060 6060 0a0a 2323 2320 4672 6f6d     ```..### From
-00001dd0: 2053 6f75 7263 650a 0a49 6e73 7461 6c6c   Source..Install
-00001de0: 2060 4341 4d45 4c60 2066 726f 6d20 736f   `CAMEL` from so
-00001df0: 7572 6365 2077 6974 6820 706f 6574 7279  urce with poetry
-00001e00: 2028 5265 636f 6d6d 656e 6465 6429 3a0a   (Recommended):.
-00001e10: 6060 6073 680a 2320 4d61 6b65 2073 7572  ```sh.# Make sur
-00001e20: 6520 796f 7572 2070 7974 686f 6e20 7665  e your python ve
-00001e30: 7273 696f 6e20 6973 206c 6174 6572 2074  rsion is later t
-00001e40: 6861 6e20 332e 390a 2320 596f 7520 6361  han 3.9.# You ca
-00001e50: 6e20 7573 6520 7079 656e 7620 746f 206d  n use pyenv to m
-00001e60: 616e 6167 6520 6d75 6c74 6970 6c65 2070  anage multiple p
-00001e70: 7974 686f 6e20 7665 7269 736f 6e73 2069  ython verisons i
-00001e80: 6e20 796f 7572 2073 7974 7374 656d 0a0a  n your sytstem..
-00001e90: 2320 436c 6f6e 6520 6769 7468 7562 2072  # Clone github r
-00001ea0: 6570 6f0a 6769 7420 636c 6f6e 6520 6874  epo.git clone ht
-00001eb0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001ec0: 2f63 616d 656c 2d61 692f 6361 6d65 6c2e  /camel-ai/camel.
-00001ed0: 6769 740a 0a23 2043 6861 6e67 6520 6469  git..# Change di
-00001ee0: 7265 6374 6f72 7920 696e 746f 2070 726f  rectory into pro
-00001ef0: 6a65 6374 2064 6972 6563 746f 7279 0a63  ject directory.c
-00001f00: 6420 6361 6d65 6c0a 0a23 2041 6374 6976  d camel..# Activ
-00001f10: 6174 6520 6361 6d65 6c20 7669 7274 7561  ate camel virtua
-00001f20: 6c20 656e 7669 726f 6e6d 656e 740a 706f  l environment.po
-00001f30: 6574 7279 2073 6865 6c6c 0a0a 2320 496e  etry shell..# In
-00001f40: 7374 616c 6c20 6361 6d65 6c20 6672 6f6d  stall camel from
-00001f50: 2073 6f75 7263 650a 2320 4974 2074 616b   source.# It tak
-00001f60: 6573 2061 626f 7574 2039 3020 7365 636f  es about 90 seco
-00001f70: 6e64 7320 746f 2072 6573 6f6c 7665 2064  nds to resolve d
-00001f80: 6570 656e 6465 6e63 6965 730a 706f 6574  ependencies.poet
-00001f90: 7279 2069 6e73 7461 6c6c 0a0a 2320 4f72  ry install..# Or
-00001fa0: 2069 6620 796f 7520 7761 6e74 2074 6f20   if you want to 
-00001fb0: 7573 6520 616c 6c20 6f74 6865 7220 6578  use all other ex
-00001fc0: 7472 6120 7061 636b 6167 6573 0a70 6f65  tra packages.poe
-00001fd0: 7472 7920 696e 7374 616c 6c20 2d45 2061  try install -E a
-00001fe0: 6c6c 2020 2320 284f 7074 696f 6e61 6c29  ll  # (Optional)
-00001ff0: 0a0a 2320 4578 6974 2074 6865 2076 6972  ..# Exit the vir
-00002000: 7475 616c 2065 6e76 6972 6f6e 6d65 6e74  tual environment
-00002010: 0a65 7869 740a 6060 600a 0a49 6e73 7461  .exit.```..Insta
-00002020: 6c6c 2060 4341 4d45 4c60 2066 726f 6d20  ll `CAMEL` from 
-00002030: 736f 7572 6365 2077 6974 6820 636f 6e64  source with cond
-00002040: 6120 616e 6420 7069 703a 0a60 6060 7368  a and pip:.```sh
-00002050: 0a23 2043 7265 6174 6520 6120 636f 6e64  .# Create a cond
-00002060: 6120 7669 7274 7561 6c20 656e 7669 726f  a virtual enviro
-00002070: 6e6d 656e 740a 636f 6e64 6120 6372 6561  nment.conda crea
-00002080: 7465 202d 2d6e 616d 6520 6361 6d65 6c20  te --name camel 
-00002090: 7079 7468 6f6e 3d33 2e31 300a 0a23 2041  python=3.10..# A
-000020a0: 6374 6976 6174 6520 6361 6d65 6c20 636f  ctivate camel co
-000020b0: 6e64 6120 656e 7669 726f 6e6d 656e 740a  nda environment.
-000020c0: 636f 6e64 6120 6163 7469 7661 7465 2063  conda activate c
-000020d0: 616d 656c 0a0a 2320 436c 6f6e 6520 6769  amel..# Clone gi
-000020e0: 7468 7562 2072 6570 6f0a 6769 7420 636c  thub repo.git cl
-000020f0: 6f6e 6520 2d62 2076 302e 312e 3320 6874  one -b v0.1.3 ht
-00002100: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00002110: 2f63 616d 656c 2d61 692f 6361 6d65 6c2e  /camel-ai/camel.
-00002120: 6769 740a 0a23 2043 6861 6e67 6520 6469  git..# Change di
-00002130: 7265 6374 6f72 7920 696e 746f 2070 726f  rectory into pro
-00002140: 6a65 6374 2064 6972 6563 746f 7279 0a63  ject directory.c
-00002150: 6420 6361 6d65 6c0a 0a23 2049 6e73 7461  d camel..# Insta
-00002160: 6c6c 2063 616d 656c 2066 726f 6d20 736f  ll camel from so
-00002170: 7572 6365 0a70 6970 2069 6e73 7461 6c6c  urce.pip install
-00002180: 202d 6520 2e0a 0a23 204f 7220 6966 2079   -e ...# Or if y
-00002190: 6f75 2077 616e 7420 746f 2075 7365 2061  ou want to use a
-000021a0: 6c6c 206f 7468 6572 2065 7874 7261 2070  ll other extra p
-000021b0: 6163 6b61 6765 730a 7069 7020 696e 7374  ackages.pip inst
-000021c0: 616c 6c20 2d65 202e 5b61 6c6c 5d20 2320  all -e .[all] # 
-000021d0: 284f 7074 696f 6e61 6c29 0a60 6060 0a0a  (Optional).```..
-000021e0: 2323 2044 6f63 756d 656e 7461 7469 6f6e  ## Documentation
-000021f0: 0a0a 5b43 414d 454c 2070 6163 6b61 6765  ..[CAMEL package
-00002200: 2064 6f63 756d 656e 7461 7469 6f6e 2070   documentation p
-00002210: 6167 6573 5d28 6874 7470 733a 2f2f 6361  ages](https://ca
-00002220: 6d65 6c2d 6169 2e67 6974 6875 622e 696f  mel-ai.github.io
-00002230: 2f63 616d 656c 2f29 2e0a 0a23 2320 4578  /camel/)...## Ex
-00002240: 616d 706c 650a 0a59 6f75 2063 616e 2066  ample..You can f
-00002250: 696e 6420 6120 6c69 7374 206f 6620 7461  ind a list of ta
-00002260: 736b 7320 666f 7220 6469 6666 6572 656e  sks for differen
-00002270: 7420 7365 7473 206f 6620 6173 7369 7374  t sets of assist
-00002280: 616e 7420 616e 6420 7573 6572 2072 6f6c  ant and user rol
-00002290: 6520 7061 6972 7320 5b68 6572 655d 2868  e pairs [here](h
-000022a0: 7474 7073 3a2f 2f64 7269 7665 2e67 6f6f  ttps://drive.goo
-000022b0: 676c 652e 636f 6d2f 6669 6c65 2f64 2f31  gle.com/file/d/1
-000022c0: 3934 5050 6153 5442 5230 376d 2d50 7a6a  94PPaSTBR07m-Pzj
-000022d0: 532d 5479 364b 6c50 4c64 4649 5051 4464  S-Ty6KlPLdFIPQDd
-000022e0: 2f76 6965 773f 7573 703d 7368 6172 655f  /view?usp=share_
-000022f0: 6c69 6e6b 292e 0a0a 4173 2061 6e20 6578  link)...As an ex
-00002300: 616d 706c 652c 2074 6f20 7275 6e20 7468  ample, to run th
-00002310: 6520 6072 6f6c 655f 706c 6179 696e 672e  e `role_playing.
-00002320: 7079 6020 7363 7269 7074 3a0a 0a46 6972  py` script:..Fir
-00002330: 7374 2c20 796f 7520 6e65 6564 2074 6f20  st, you need to 
-00002340: 6164 6420 796f 7572 204f 7065 6e41 4920  add your OpenAI 
-00002350: 4150 4920 6b65 7920 746f 2073 7973 7465  API key to syste
-00002360: 6d20 656e 7669 726f 6e6d 656e 7420 7661  m environment va
-00002370: 7269 6162 6c65 732e 2054 6865 206d 6574  riables. The met
-00002380: 686f 6420 746f 2064 6f20 7468 6973 2064  hod to do this d
-00002390: 6570 656e 6473 206f 6e20 796f 7572 206f  epends on your o
-000023a0: 7065 7261 7469 6e67 2073 7973 7465 6d20  perating system 
-000023b0: 616e 6420 7468 6520 7368 656c 6c20 796f  and the shell yo
-000023c0: 7527 7265 2075 7369 6e67 2e0a 0a2a 2a46  u're using...**F
-000023d0: 6f72 2042 6173 6820 7368 656c 6c20 284c  or Bash shell (L
-000023e0: 696e 7578 2c20 6d61 634f 532c 2047 6974  inux, macOS, Git
-000023f0: 2042 6173 6820 6f6e 2057 696e 646f 7773   Bash on Windows
-00002400: 293a 2a2a 0a0a 6060 6062 6173 680a 2320  ):**..```bash.# 
-00002410: 4578 706f 7274 2079 6f75 7220 4f70 656e  Export your Open
-00002420: 4149 2041 5049 206b 6579 0a65 7870 6f72  AI API key.expor
-00002430: 7420 4f50 454e 4149 5f41 5049 5f4b 4559  t OPENAI_API_KEY
-00002440: 3d3c 696e 7365 7274 2079 6f75 7220 4f70  =<insert your Op
-00002450: 656e 4149 2041 5049 206b 6579 3e0a 4f50  enAI API key>.OP
-00002460: 454e 4149 5f41 5049 5f42 4153 455f 5552  ENAI_API_BASE_UR
-00002470: 4c3d 3c69 6e65 7274 2079 6f75 7220 4f70  L=<inert your Op
-00002480: 656e 4149 2041 5049 2042 4153 4520 5552  enAI API BASE UR
-00002490: 4c3e 2020 2328 5368 6f75 6c64 2079 6f75  L>  #(Should you
-000024a0: 2075 7469 6c69 7a65 2061 6e20 4f70 656e   utilize an Open
-000024b0: 4149 2070 726f 7879 2073 6572 7669 6365  AI proxy service
-000024c0: 2c20 6b69 6e64 6c79 2073 7065 6369 6679  , kindly specify
-000024d0: 2074 6869 7329 0a60 6060 0a0a 2a2a 466f   this).```..**Fo
-000024e0: 7220 5769 6e64 6f77 7320 436f 6d6d 616e  r Windows Comman
-000024f0: 6420 5072 6f6d 7074 3a2a 2a0a 0a60 6060  d Prompt:**..```
-00002500: 636d 640a 5245 4d20 6578 706f 7274 2079  cmd.REM export y
-00002510: 6f75 7220 4f70 656e 4149 2041 5049 206b  our OpenAI API k
-00002520: 6579 0a73 6574 204f 5045 4e41 495f 4150  ey.set OPENAI_AP
-00002530: 495f 4b45 593d 3c69 6e73 6572 7420 796f  I_KEY=<insert yo
-00002540: 7572 204f 7065 6e41 4920 4150 4920 6b65  ur OpenAI API ke
-00002550: 793e 0a73 6574 204f 5045 4e41 495f 4150  y>.set OPENAI_AP
-00002560: 495f 4241 5345 5f55 524c 3d3c 696e 6572  I_BASE_URL=<iner
-00002570: 7420 796f 7572 204f 7065 6e41 4920 4150  t your OpenAI AP
-00002580: 4920 4241 5345 2055 524c 3e20 2023 2853  I BASE URL>  #(S
-00002590: 686f 756c 6420 796f 7520 7574 696c 697a  hould you utiliz
-000025a0: 6520 616e 204f 7065 6e41 4920 7072 6f78  e an OpenAI prox
-000025b0: 7920 7365 7276 6963 652c 206b 696e 646c  y service, kindl
-000025c0: 7920 7370 6563 6966 7920 7468 6973 290a  y specify this).
-000025d0: 6060 600a 0a2a 2a46 6f72 2057 696e 646f  ```..**For Windo
-000025e0: 7773 2050 6f77 6572 5368 656c 6c3a 2a2a  ws PowerShell:**
-000025f0: 0a0a 6060 6070 6f77 6572 7368 656c 6c0a  ..```powershell.
-00002600: 2320 4578 706f 7274 2079 6f75 7220 4f70  # Export your Op
-00002610: 656e 4149 2041 5049 206b 6579 0a24 656e  enAI API key.$en
-00002620: 763a 4f50 454e 4149 5f41 5049 5f4b 4559  v:OPENAI_API_KEY
-00002630: 3d22 3c69 6e73 6572 7420 796f 7572 204f  ="<insert your O
-00002640: 7065 6e41 4920 4150 4920 6b65 793e 220a  penAI API key>".
-00002650: 2465 6e76 3a4f 5045 4e41 495f 4150 495f  $env:OPENAI_API_
-00002660: 4241 5345 5f55 524c 3d22 3c69 6e65 7274  BASE_URL="<inert
-00002670: 2079 6f75 7220 4f70 656e 4149 2041 5049   your OpenAI API
-00002680: 2042 4153 4520 5552 4c3e 2220 2023 2853   BASE URL>"  #(S
-00002690: 686f 756c 6420 796f 7520 7574 696c 697a  hould you utiliz
-000026a0: 6520 616e 204f 7065 6e41 4920 7072 6f78  e an OpenAI prox
-000026b0: 7920 7365 7276 6963 652c 206b 696e 646c  y service, kindl
-000026c0: 7920 7370 6563 6966 7920 7468 6973 290a  y specify this).
-000026d0: 6060 600a 0a52 6570 6c61 6365 2060 3c69  ```..Replace `<i
-000026e0: 6e73 6572 7420 796f 7572 204f 7065 6e41  nsert your OpenA
-000026f0: 4920 4150 4920 6b65 793e 6020 7769 7468  I API key>` with
-00002700: 2079 6f75 7220 6163 7475 616c 204f 7065   your actual Ope
-00002710: 6e41 4920 4150 4920 6b65 7920 696e 2065  nAI API key in e
-00002720: 6163 6820 6361 7365 2e20 4d61 6b65 2073  ach case. Make s
-00002730: 7572 6520 7468 6572 6520 6172 6520 6e6f  ure there are no
-00002740: 2073 7061 6365 7320 6172 6f75 6e64 2074   spaces around t
-00002750: 6865 2060 3d60 2073 6967 6e2e 0a0a 4166  he `=` sign...Af
-00002760: 7465 7220 7365 7474 696e 6720 7468 6520  ter setting the 
-00002770: 4f70 656e 4149 2041 5049 206b 6579 2c20  OpenAI API key, 
-00002780: 796f 7520 6361 6e20 7275 6e20 7468 6520  you can run the 
-00002790: 7363 7269 7074 3a0a 0a60 6060 6261 7368  script:..```bash
-000027a0: 0a23 2059 6f75 2063 616e 2063 6861 6e67  .# You can chang
-000027b0: 6520 7468 6520 726f 6c65 2070 6169 7220  e the role pair 
-000027c0: 616e 6420 696e 6974 6961 6c20 7072 6f6d  and initial prom
-000027d0: 7074 2069 6e20 726f 6c65 5f70 6c61 7969  pt in role_playi
-000027e0: 6e67 2e70 790a 7079 7468 6f6e 2065 7861  ng.py.python exa
-000027f0: 6d70 6c65 732f 6169 5f73 6f63 6965 7479  mples/ai_society
-00002800: 2f72 6f6c 655f 706c 6179 696e 672e 7079  /role_playing.py
-00002810: 0a60 6060 0a0a 506c 6561 7365 206e 6f74  .```..Please not
-00002820: 6520 7468 6174 2074 6865 2065 6e76 6972  e that the envir
-00002830: 6f6e 6d65 6e74 2076 6172 6961 626c 6520  onment variable 
-00002840: 6973 2073 6573 7369 6f6e 2d73 7065 6369  is session-speci
-00002850: 6669 632e 2049 6620 796f 7520 6f70 656e  fic. If you open
-00002860: 2061 206e 6577 2074 6572 6d69 6e61 6c20   a new terminal 
-00002870: 7769 6e64 6f77 206f 7220 7461 622c 2079  window or tab, y
-00002880: 6f75 2077 696c 6c20 6e65 6564 2074 6f20  ou will need to 
-00002890: 7365 7420 7468 6520 4150 4920 6b65 7920  set the API key 
-000028a0: 6167 6169 6e20 696e 2074 6861 7420 6e65  again in that ne
-000028b0: 7720 7365 7373 696f 6e2e 0a0a 0a23 2320  w session....## 
-000028c0: 5573 6520 4f70 656e 2d53 6f75 7263 6520  Use Open-Source 
-000028d0: 4d6f 6465 6c73 2061 7320 4261 636b 656e  Models as Backen
-000028e0: 6473 0a0a 5468 6520 6261 7369 6320 776f  ds..The basic wo
-000028f0: 726b 666c 6f77 206f 6620 7573 696e 6720  rkflow of using 
-00002900: 616e 206f 7065 6e2d 736f 7572 6365 6420  an open-sourced 
-00002910: 6d6f 6465 6c20 6173 2074 6865 2062 6163  model as the bac
-00002920: 6b65 6e64 2069 7320 6261 7365 6420 6f6e  kend is based on
-00002930: 2061 6e20 6578 7465 726e 616c 2073 6572   an external ser
-00002940: 7665 7220 7275 6e6e 696e 6720 4c4c 4d20  ver running LLM 
-00002950: 696e 6665 7265 6e63 6520 7365 7276 6963  inference servic
-00002960: 652c 2065 2e67 2e20 6475 7269 6e67 2074  e, e.g. during t
-00002970: 6865 2064 6576 656c 6f70 6d65 6e74 2077  he development w
-00002980: 6520 6368 6f73 6520 5b46 6173 7443 6861  e chose [FastCha
-00002990: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
-000029a0: 622e 636f 6d2f 6c6d 2d73 7973 2f46 6173  b.com/lm-sys/Fas
-000029b0: 7443 6861 7429 2074 6f20 7275 6e20 7468  tChat) to run th
-000029c0: 6520 7365 7276 6963 652e 0a0a 5765 2064  e service...We d
-000029d0: 6f20 6e6f 7420 6669 7820 7468 6520 6368  o not fix the ch
-000029e0: 6f69 6365 206f 6620 7365 7276 6572 2074  oice of server t
-000029f0: 6f20 6465 636f 7570 6c65 2074 6865 2069  o decouple the i
-00002a00: 6d70 6c65 6d65 6e74 6174 696f 6e20 6f66  mplementation of
-00002a10: 2061 6e79 2073 7065 6369 6669 6320 4c4c   any specific LL
-00002a20: 4d20 696e 6665 7265 6e63 6520 7365 7276  M inference serv
-00002a30: 6572 2077 6974 6820 4341 4d45 4c20 2869  er with CAMEL (i
-00002a40: 6e64 6963 6174 696e 6720 7468 6520 7365  ndicating the se
-00002a50: 7276 6572 206e 6565 6473 2074 6f20 6265  rver needs to be
-00002a60: 2064 6570 6c6f 7965 6420 6279 2074 6865   deployed by the
-00002a70: 2075 7365 7220 6869 6d73 656c 6629 2e20   user himself). 
-00002a80: 4275 7420 7468 6520 7365 7276 6572 2074  But the server t
-00002a90: 6f20 6265 2064 6570 6c6f 7965 6420 6d75  o be deployed mu
-00002aa0: 7374 2073 6174 6973 6679 2074 6861 7420  st satisfy that 
-00002ab0: 2a2a 6974 2073 7570 706f 7274 7320 4f70  **it supports Op
-00002ac0: 656e 4149 2d63 6f6d 7061 7469 626c 6520  enAI-compatible 
-00002ad0: 4150 4973 2c20 6573 7065 6369 616c 6c79  APIs, especially
-00002ae0: 2074 6865 206d 6574 686f 6420 606f 7065   the method `ope
-00002af0: 6e61 692e 4368 6174 436f 6d70 6c65 7469  nai.ChatCompleti
-00002b00: 6f6e 2e63 7265 6174 6560 2a2a 2e0a 0a48  on.create`**...H
-00002b10: 6572 6520 6172 6520 736f 6d65 2069 6e73  ere are some ins
-00002b20: 7472 7563 7469 6f6e 7320 666f 7220 656e  tructions for en
-00002b30: 6162 6c69 6e67 206f 7065 6e2d 736f 7572  abling open-sour
-00002b40: 6365 2062 6163 6b65 6e64 732c 2077 6865  ce backends, whe
-00002b50: 7265 2077 6520 7573 6520 7468 6520 5b46  re we use the [F
-00002b60: 6173 7443 6861 745d 2868 7474 7073 3a2f  astChat](https:/
-00002b70: 2f67 6974 6875 622e 636f 6d2f 6c6d 2d73  /github.com/lm-s
-00002b80: 7973 2f46 6173 7443 6861 7429 2061 6e64  ys/FastChat) and
-00002b90: 2061 204c 4c61 4d41 322d 6261 7365 6420   a LLaMA2-based 
-00002ba0: 6d6f 6465 6c20 285b 606d 6574 612d 6c6c  model ([`meta-ll
-00002bb0: 616d 612f 4c6c 616d 612d 322d 3762 2d63  ama/Llama-2-7b-c
-00002bc0: 6861 742d 6866 605d 2868 7474 7073 3a2f  hat-hf`](https:/
-00002bd0: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
-00002be0: 6d65 7461 2d6c 6c61 6d61 2f4c 6c61 6d61  meta-llama/Llama
-00002bf0: 2d32 2d37 622d 6368 6174 2d68 6629 2920  -2-7b-chat-hf)) 
-00002c00: 696e 2074 6865 2065 7861 6d70 6c65 2e20  in the example. 
-00002c10: 506c 6561 7365 2069 6e73 7461 6c6c 2046  Please install F
-00002c20: 6173 7443 6861 7420 696e 2061 6476 616e  astChat in advan
-00002c30: 6365 2066 6f6c 6c6f 7769 6e67 2074 6865  ce following the
-00002c40: 6972 2069 6e73 7461 6c6c 6174 696f 6e20  ir installation 
-00002c50: 6775 6964 616e 6365 2e0a 0a31 2e20 4265  guidance...1. Be
-00002c60: 666f 7265 2072 756e 6e69 6e67 2043 414d  fore running CAM
-00002c70: 454c 2c20 7765 2073 686f 756c 6420 6669  EL, we should fi
-00002c80: 7273 746c 7920 6c61 756e 6368 2046 6173  rstly launch Fas
-00002c90: 7443 6861 7420 7365 7276 6572 2066 6f6c  tChat server fol
-00002ca0: 6c6f 7769 6e67 2074 6865 2067 7569 6461  lowing the guida
-00002cb0: 6e63 6520 6f6e 2068 7474 7073 3a2f 2f67  nce on https://g
-00002cc0: 6974 6875 622e 636f 6d2f 6c6d 2d73 7973  ithub.com/lm-sys
-00002cd0: 2f46 6173 7443 6861 742f 626c 6f62 2f6d  /FastChat/blob/m
-00002ce0: 6169 6e2f 646f 6373 2f6f 7065 6e61 695f  ain/docs/openai_
-00002cf0: 6170 692e 6d64 2e20 5468 6520 696e 7374  api.md. The inst
-00002d00: 7275 6374 696f 6e73 2073 756d 6d61 7269  ructions summari
-00002d10: 7a65 6420 6265 6c6f 7720 7368 6f75 6c64  zed below should
-00002d20: 2062 6520 6b65 7074 2072 756e 6e69 6e67   be kept running
-00002d30: 202a 2a69 6e20 7365 7061 7261 7465 2070   **in separate p
-00002d40: 726f 6365 7373 6573 2a2a 3a0a 0a60 6060  rocesses**:..```
-00002d50: 7368 0a23 204c 6175 6e63 6820 7468 6520  sh.# Launch the 
-00002d60: 636f 6e74 726f 6c6c 6572 0a70 7974 686f  controller.pytho
-00002d70: 6e20 2d6d 2066 6173 7463 6861 742e 7365  n -m fastchat.se
-00002d80: 7276 652e 636f 6e74 726f 6c6c 6572 0a0a  rve.controller..
-00002d90: 2320 4c61 756e 6368 2074 6865 206d 6f64  # Launch the mod
-00002da0: 656c 2077 6f72 6b65 7228 7329 0a70 7974  el worker(s).pyt
-00002db0: 686f 6e33 202d 6d20 6661 7374 6368 6174  hon3 -m fastchat
-00002dc0: 2e73 6572 7665 2e6d 6f64 656c 5f77 6f72  .serve.model_wor
-00002dd0: 6b65 7220 2d2d 6d6f 6465 6c2d 7061 7468  ker --model-path
-00002de0: 206d 6574 612d 6c6c 616d 612f 4c6c 616d   meta-llama/Llam
-00002df0: 612d 322d 3762 2d63 6861 742d 6866 0a0a  a-2-7b-chat-hf..
-00002e00: 2320 4c61 756e 6368 2074 6865 2052 4553  # Launch the RES
-00002e10: 5466 756c 2041 5049 2073 6572 7665 720a  Tful API server.
-00002e20: 7079 7468 6f6e 3320 2d6d 2066 6173 7463  python3 -m fastc
-00002e30: 6861 742e 7365 7276 652e 6f70 656e 6169  hat.serve.openai
-00002e40: 5f61 7069 5f73 6572 7665 7220 2d2d 686f  _api_server --ho
-00002e50: 7374 206c 6f63 616c 686f 7374 202d 2d70  st localhost --p
-00002e60: 6f72 7420 3830 3030 0a60 6060 0a0a 322e  ort 8000.```..2.
-00002e70: 2041 6674 6572 206f 6273 6572 7669 6e67   After observing
-00002e80: 2074 6865 2063 6f6e 7472 6f6c 6c65 7220   the controller 
-00002e90: 7375 6363 6573 7366 756c 6c79 2072 6563  successfully rec
-00002ea0: 6569 7669 6e67 2074 6865 2068 6561 7274  eiving the heart
-00002eb0: 2062 6561 7420 7369 676e 616c 2066 726f   beat signal fro
-00002ec0: 6d20 7468 6520 776f 726b 6572 2c20 7468  m the worker, th
-00002ed0: 6520 7365 7276 6572 2073 686f 756c 6420  e server should 
-00002ee0: 6265 2072 6561 6479 2066 6f72 2075 7365  be ready for use
-00002ef0: 2061 7420 6874 7470 3a2f 2f6c 6f63 616c   at http://local
-00002f00: 686f 7374 3a38 3030 302f 7631 2e0a 0a33  host:8000/v1...3
-00002f10: 2e20 5468 656e 2077 6520 6361 6e20 7472  . Then we can tr
-00002f20: 7920 6f6e 2072 756e 6e69 6e67 2060 726f  y on running `ro
-00002f30: 6c65 5f70 6c61 7969 6e67 5f77 6974 685f  le_playing_with_
-00002f40: 6f70 656e 5f73 6f75 7263 655f 6d6f 6465  open_source_mode
-00002f50: 6c2e 7079 602c 2077 6865 7265 2065 6163  l.py`, where eac
-00002f60: 6820 6167 656e 7420 696e 2074 6869 7320  h agent in this 
-00002f70: 6578 616d 706c 6520 6973 2069 6e69 7469  example is initi
-00002f80: 616c 697a 6564 2077 6974 6820 7370 6563  alized with spec
-00002f90: 6966 7969 6e67 2074 6865 2060 6d6f 6465  ifying the `mode
-00002fa0: 6c5f 7061 7468 6020 616e 6420 6073 6572  l_path` and `ser
-00002fb0: 7665 725f 7572 6c60 2c20 7369 6d69 6c61  ver_url`, simila
-00002fc0: 7220 746f 2074 6865 2065 7861 6d70 6c65  r to the example
-00002fd0: 2063 6f64 6520 6265 6c6f 773a 0a0a 6060   code below:..``
-00002fe0: 6070 7974 686f 6e0a 7379 7374 656d 5f6d  `python.system_m
-00002ff0: 6573 7361 6765 203d 2023 202e 2e2e 0a0a  essage = # .....
-00003000: 6167 656e 745f 6b77 6172 6773 203d 2064  agent_kwargs = d
-00003010: 6963 7428 0a20 2020 206d 6f64 656c 3d6d  ict(.    model=m
-00003020: 6f64 656c 5f74 7970 652c 0a20 2020 206d  odel_type,.    m
-00003030: 6f64 656c 5f63 6f6e 6669 673d 4f70 656e  odel_config=Open
-00003040: 536f 7572 6365 436f 6e66 6967 280a 2020  SourceConfig(.  
-00003050: 2020 2020 2020 6d6f 6465 6c5f 7061 7468        model_path
-00003060: 3d22 6d65 7461 2d6c 6c61 6d61 2f4c 6c61  ="meta-llama/Lla
-00003070: 6d61 2d32 2d37 622d 6368 6174 2d68 6622  ma-2-7b-chat-hf"
-00003080: 2c0a 2020 2020 2020 2020 7365 7276 6572  ,.        server
-00003090: 5f75 726c 3d22 6874 7470 3a2f 2f6c 6f63  _url="http://loc
-000030a0: 616c 686f 7374 3a38 3030 302f 7631 222c  alhost:8000/v1",
-000030b0: 0a20 2020 2029 2c0a 290a 0a61 6765 6e74  .    ),.)..agent
-000030c0: 203d 2043 6861 7441 6765 6e74 280a 2020   = ChatAgent(.  
-000030d0: 2020 7379 7374 656d 5f6d 6573 7361 6765    system_message
-000030e0: 2c0a 2020 2020 2a2a 6167 656e 745f 6b77  ,.    **agent_kw
-000030f0: 6172 6773 2c0a 290a 6060 600a 0a23 2323  args,.).```..###
-00003100: 2053 7570 706f 7274 6564 204d 6f64 656c   Supported Model
-00003110: 730a 0a2d 204c 4c61 4d41 322d 6261 7365  s..- LLaMA2-base
-00003120: 6420 6d6f 6465 6c73 0a20 202d 2065 7861  d models.  - exa
-00003130: 6d70 6c65 3a20 5b6d 6574 612d 6c6c 616d  mple: [meta-llam
-00003140: 612f 4c6c 616d 612d 322d 3762 2d63 6861  a/Llama-2-7b-cha
-00003150: 742d 6866 5d28 6874 7470 733a 2f2f 6875  t-hf](https://hu
-00003160: 6767 696e 6766 6163 652e 636f 2f6d 6574  ggingface.co/met
-00003170: 612d 6c6c 616d 612f 4c6c 616d 612d 322d  a-llama/Llama-2-
-00003180: 3762 2d63 6861 742d 6866 290a 2d20 5669  7b-chat-hf).- Vi
-00003190: 6375 6e61 2d62 6173 6564 206d 6f64 656c  cuna-based model
-000031a0: 730a 2020 2d20 6578 616d 706c 653a 205b  s.  - example: [
-000031b0: 6c6d 7379 732f 7669 6375 6e61 2d37 622d  lmsys/vicuna-7b-
-000031c0: 7631 2e35 5d28 6874 7470 733a 2f2f 6875  v1.5](https://hu
-000031d0: 6767 696e 6766 6163 652e 636f 2f6c 6d73  ggingface.co/lms
-000031e0: 7973 2f76 6963 756e 612d 3762 2d76 312e  ys/vicuna-7b-v1.
-000031f0: 3529 0a0a 2323 2044 6174 6120 2848 6f73  5)..## Data (Hos
-00003200: 7465 6420 6f6e 2048 7567 6769 6e67 2046  ted on Hugging F
-00003210: 6163 6529 0a7c 2044 6174 6173 6574 2020  ace).| Dataset  
-00003220: 2020 2020 2020 7c20 4368 6174 2066 6f72        | Chat for
-00003230: 6d61 7420 2020 2020 2020 2020 2020 2020  mat             
-00003240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003280: 2020 2020 2020 2020 2020 2020 7c20 496e              | In
-00003290: 7374 7275 6374 696f 6e20 666f 726d 6174  struction format
-000032a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032f0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00003300: 2043 6861 7420 666f 726d 6174 2028 7472   Chat format (tr
-00003310: 616e 736c 6174 6564 2920 2020 2020 2020  anslated)       
-00003320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003350: 2020 2020 2020 2020 2020 2020 7c0a 7c2d              |.|-
-00003360: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
-00003370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000033a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000033b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000033c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000033d0: 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d  -----|----------
-000033e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000033f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003440: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
-00003450: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003470: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000034a0: 2d2d 2d2d 2d7c 0a7c 202a 2a41 4920 536f  -----|.| **AI So
-000034b0: 6369 6574 792a 2a20 7c20 5b43 6861 7420  ciety** | [Chat 
-000034c0: 666f 726d 6174 5d28 6874 7470 733a 2f2f  format](https://
-000034d0: 6875 6767 696e 6766 6163 652e 636f 2f64  huggingface.co/d
-000034e0: 6174 6173 6574 732f 6361 6d65 6c2d 6169  atasets/camel-ai
-000034f0: 2f61 695f 736f 6369 6574 792f 626c 6f62  /ai_society/blob
-00003500: 2f6d 6169 6e2f 6169 5f73 6f63 6965 7479  /main/ai_society
-00003510: 5f63 6861 742e 7461 722e 677a 2920 7c20  _chat.tar.gz) | 
-00003520: 5b49 6e73 7472 7563 7469 6f6e 2066 6f72  [Instruction for
-00003530: 6d61 745d 2868 7474 7073 3a2f 2f68 7567  mat](https://hug
-00003540: 6769 6e67 6661 6365 2e63 6f2f 6461 7461  gingface.co/data
-00003550: 7365 7473 2f63 616d 656c 2d61 692f 6169  sets/camel-ai/ai
-00003560: 5f73 6f63 6965 7479 2f62 6c6f 622f 6d61  _society/blob/ma
-00003570: 696e 2f61 695f 736f 6369 6574 795f 696e  in/ai_society_in
-00003580: 7374 7275 6374 696f 6e73 2e6a 736f 6e29  structions.json)
-00003590: 207c 205b 4368 6174 2066 6f72 6d61 7420   | [Chat format 
-000035a0: 2874 7261 6e73 6c61 7465 6429 5d28 6874  (translated)](ht
-000035b0: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
-000035c0: 652e 636f 2f64 6174 6173 6574 732f 6361  e.co/datasets/ca
-000035d0: 6d65 6c2d 6169 2f61 695f 736f 6369 6574  mel-ai/ai_societ
-000035e0: 795f 7472 616e 736c 6174 6564 2920 7c0a  y_translated) |.
-000035f0: 7c20 2a2a 436f 6465 2a2a 2020 2020 2020  | **Code**      
-00003600: 207c 205b 4368 6174 2066 6f72 6d61 745d   | [Chat format]
-00003610: 2868 7474 7073 3a2f 2f68 7567 6769 6e67  (https://hugging
-00003620: 6661 6365 2e63 6f2f 6461 7461 7365 7473  face.co/datasets
-00003630: 2f63 616d 656c 2d61 692f 636f 6465 2f62  /camel-ai/code/b
-00003640: 6c6f 622f 6d61 696e 2f63 6f64 655f 6368  lob/main/code_ch
-00003650: 6174 2e74 6172 2e67 7a29 2020 2020 2020  at.tar.gz)      
-00003660: 2020 2020 2020 207c 205b 496e 7374 7275         | [Instru
-00003670: 6374 696f 6e20 666f 726d 6174 5d28 6874  ction format](ht
-00003680: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
-00003690: 652e 636f 2f64 6174 6173 6574 732f 6361  e.co/datasets/ca
-000036a0: 6d65 6c2d 6169 2f63 6f64 652f 626c 6f62  mel-ai/code/blob
-000036b0: 2f6d 6169 6e2f 636f 6465 5f69 6e73 7472  /main/code_instr
-000036c0: 7563 7469 6f6e 732e 6a73 6f6e 2920 2020  uctions.json)   
-000036d0: 2020 2020 2020 2020 2020 7c20 7820 2020            | x   
-000036e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003730: 2020 2020 2020 207c 0a7c 202a 2a4d 6174         |.| **Mat
-00003740: 682a 2a20 2020 2020 2020 7c20 5b43 6861  h**       | [Cha
-00003750: 7420 666f 726d 6174 5d28 6874 7470 733a  t format](https:
-00003760: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
-00003770: 2f64 6174 6173 6574 732f 6361 6d65 6c2d  /datasets/camel-
-00003780: 6169 2f6d 6174 6829 2020 2020 2020 2020  ai/math)        
-00003790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037b0: 7c20 7820 2020 2020 2020 2020 2020 2020  | x             
-000037c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003820: 2020 207c 2078 2020 2020 2020 2020 2020     | x          
-00003830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003880: 7c0a 7c20 2a2a 5068 7973 6963 732a 2a20  |.| **Physics** 
-00003890: 2020 207c 205b 4368 6174 2066 6f72 6d61     | [Chat forma
-000038a0: 745d 2868 7474 7073 3a2f 2f68 7567 6769  t](https://huggi
-000038b0: 6e67 6661 6365 2e63 6f2f 6461 7461 7365  ngface.co/datase
-000038c0: 7473 2f63 616d 656c 2d61 692f 7068 7973  ts/camel-ai/phys
-000038d0: 6963 7329 2020 2020 2020 2020 2020 2020  ics)            
+000009f0: 2d44 6973 743a 2070 7974 6573 7420 283e  -Dist: pytest (>
+00000a00: 3d37 2c3c 3829 203b 2065 7874 7261 203d  =7,<8) ; extra =
+00000a10: 3d20 2274 6573 7422 0a52 6571 7569 7265  = "test".Require
+00000a20: 732d 4469 7374 3a20 7164 7261 6e74 2d63  s-Dist: qdrant-c
+00000a30: 6c69 656e 7420 283e 3d31 2e39 2e30 2c3c  lient (>=1.9.0,<
+00000a40: 322e 302e 3029 203b 2065 7874 7261 203d  2.0.0) ; extra =
+00000a50: 3d20 2276 6563 746f 722d 6461 7461 6261  = "vector-databa
+00000a60: 7365 7322 206f 7220 6578 7472 6120 3d3d  ses" or extra ==
+00000a70: 2022 616c 6c22 0a52 6571 7569 7265 732d   "all".Requires-
+00000a80: 4469 7374 3a20 7261 6e6b 2d62 6d32 3520  Dist: rank-bm25 
+00000a90: 283e 3d30 2e32 2e32 2c3c 302e 332e 3029  (>=0.2.2,<0.3.0)
+00000aa0: 203b 2065 7874 7261 203d 3d20 2272 6574   ; extra == "ret
+00000ab0: 7269 6576 6572 7322 206f 7220 6578 7472  rievers" or extr
+00000ac0: 6120 3d3d 2022 616c 6c22 0a52 6571 7569  a == "all".Requi
+00000ad0: 7265 732d 4469 7374 3a20 7265 7175 6573  res-Dist: reques
+00000ae0: 7473 5f6f 6175 7468 6c69 6220 283e 3d31  ts_oauthlib (>=1
+00000af0: 2e33 2e31 2c3c 322e 302e 3029 203b 2065  .3.1,<2.0.0) ; e
+00000b00: 7874 7261 203d 3d20 2274 6f6f 6c73 2220  xtra == "tools" 
+00000b10: 6f72 2065 7874 7261 203d 3d20 2261 6c6c  or extra == "all
+00000b20: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000b30: 2073 656e 7465 6e63 652d 7472 616e 7366   sentence-transf
+00000b40: 6f72 6d65 7273 2028 3e3d 322e 322e 322c  ormers (>=2.2.2,
+00000b50: 3c33 2e30 2e30 2920 3b20 6578 7472 6120  <3.0.0) ; extra 
+00000b60: 3d3d 2022 656e 636f 6465 7273 2220 6f72  == "encoders" or
+00000b70: 2065 7874 7261 203d 3d20 2261 6c6c 220a   extra == "all".
+00000b80: 5265 7175 6972 6573 2d44 6973 743a 2073  Requires-Dist: s
+00000b90: 656e 7465 6e63 6570 6965 6365 2028 3e3d  entencepiece (>=
+00000ba0: 302c 3c31 2920 3b20 6578 7472 6120 3d3d  0,<1) ; extra ==
+00000bb0: 2022 6875 6767 696e 6766 6163 652d 6167   "huggingface-ag
+00000bc0: 656e 7422 206f 7220 6578 7472 6120 3d3d  ent" or extra ==
+00000bd0: 2022 616c 6c22 0a52 6571 7569 7265 732d   "all".Requires-
+00000be0: 4469 7374 3a20 736c 6163 6b2d 7364 6b20  Dist: slack-sdk 
+00000bf0: 283e 3d33 2e32 372e 322c 3c34 2e30 2e30  (>=3.27.2,<4.0.0
+00000c00: 2920 3b20 6578 7472 6120 3d3d 2022 746f  ) ; extra == "to
+00000c10: 6f6c 7322 206f 7220 6578 7472 6120 3d3d  ols" or extra ==
+00000c20: 2022 616c 6c22 0a52 6571 7569 7265 732d   "all".Requires-
+00000c30: 4469 7374 3a20 736f 756e 6466 696c 6520  Dist: soundfile 
+00000c40: 283e 3d30 2c3c 3129 203b 2065 7874 7261  (>=0,<1) ; extra
+00000c50: 203d 3d20 2268 7567 6769 6e67 6661 6365   == "huggingface
+00000c60: 2d61 6765 6e74 2220 6f72 2065 7874 7261  -agent" or extra
+00000c70: 203d 3d20 2261 6c6c 220a 5265 7175 6972   == "all".Requir
+00000c80: 6573 2d44 6973 743a 2074 696b 746f 6b65  es-Dist: tiktoke
+00000c90: 6e20 283e 3d30 2e37 2e30 2c3c 302e 382e  n (>=0.7.0,<0.8.
+00000ca0: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
+00000cb0: 3a20 746f 7263 6820 283e 3d31 2c3c 3229  : torch (>=1,<2)
+00000cc0: 203b 2065 7874 7261 203d 3d20 2268 7567   ; extra == "hug
+00000cd0: 6769 6e67 6661 6365 2d61 6765 6e74 2220  gingface-agent" 
+00000ce0: 6f72 2065 7874 7261 203d 3d20 2261 6c6c  or extra == "all
+00000cf0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000d00: 2074 7261 6e73 666f 726d 6572 7320 283e   transformers (>
+00000d10: 3d34 2c3c 3529 203b 2065 7874 7261 203d  =4,<5) ; extra =
+00000d20: 3d20 2268 7567 6769 6e67 6661 6365 2d61  = "huggingface-a
+00000d30: 6765 6e74 2220 6f72 2065 7874 7261 203d  gent" or extra =
+00000d40: 3d20 2261 6c6c 220a 5265 7175 6972 6573  = "all".Requires
+00000d50: 2d44 6973 743a 2075 6e73 7472 7563 7475  -Dist: unstructu
+00000d60: 7265 645b 616c 6c2d 646f 6373 5d20 283e  red[all-docs] (>
+00000d70: 3d30 2e31 302e 3330 2c3c 302e 3131 2e30  =0.10.30,<0.11.0
+00000d80: 2920 3b20 6578 7472 6120 3d3d 2022 746f  ) ; extra == "to
+00000d90: 6f6c 7322 206f 7220 6578 7472 6120 3d3d  ols" or extra ==
+00000da0: 2022 616c 6c22 0a52 6571 7569 7265 732d   "all".Requires-
+00000db0: 4469 7374 3a20 7769 6b69 7065 6469 6120  Dist: wikipedia 
+00000dc0: 283e 3d31 2c3c 3229 203b 2065 7874 7261  (>=1,<2) ; extra
+00000dd0: 203d 3d20 2274 6f6f 6c73 2220 6f72 2065   == "tools" or e
+00000de0: 7874 7261 203d 3d20 2261 6c6c 220a 5265  xtra == "all".Re
+00000df0: 7175 6972 6573 2d44 6973 743a 2077 6f6c  quires-Dist: wol
+00000e00: 6672 616d 616c 7068 6120 283e 3d35 2e30  framalpha (>=5.0
+00000e10: 2e30 2c3c 362e 302e 3029 203b 2065 7874  .0,<6.0.0) ; ext
+00000e20: 7261 203d 3d20 2274 6f6f 6c73 2220 6f72  ra == "tools" or
+00000e30: 2065 7874 7261 203d 3d20 2261 6c6c 220a   extra == "all".
+00000e40: 5072 6f6a 6563 742d 5552 4c3a 2044 6f63  Project-URL: Doc
+00000e50: 756d 656e 7461 7469 6f6e 2c20 6874 7470  umentation, http
+00000e60: 733a 2f2f 646f 6373 2e63 616d 656c 2d61  s://docs.camel-a
+00000e70: 692e 6f72 670a 5072 6f6a 6563 742d 5552  i.org.Project-UR
+00000e80: 4c3a 2052 6570 6f73 6974 6f72 792c 2068  L: Repository, h
+00000e90: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000ea0: 6d2f 6361 6d65 6c2d 6169 2f63 616d 656c  m/camel-ai/camel
+00000eb0: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
+00000ec0: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
+00000ed0: 6d61 726b 646f 776e 0a0a 5b21 5b43 6f6c  markdown..[![Col
+00000ee0: 6162 5d5b 636f 6c61 622d 696d 6167 655d  ab][colab-image]
+00000ef0: 5d5b 636f 6c61 622d 7572 6c5d 0a5b 215b  ][colab-url].[![
+00000f00: 4875 6767 696e 6720 4661 6365 5d5b 6875  Hugging Face][hu
+00000f10: 6767 696e 6766 6163 652d 696d 6167 655d  ggingface-image]
+00000f20: 5d5b 6875 6767 696e 6766 6163 652d 7572  ][huggingface-ur
+00000f30: 6c5d 0a5b 215b 536c 6163 6b5d 5b73 6c61  l].[![Slack][sla
+00000f40: 636b 2d69 6d61 6765 5d5d 5b73 6c61 636b  ck-image]][slack
+00000f50: 2d75 726c 5d0a 5b21 5b44 6973 636f 7264  -url].[![Discord
+00000f60: 5d5b 6469 7363 6f72 642d 696d 6167 655d  ][discord-image]
+00000f70: 5d5b 6469 7363 6f72 642d 7572 6c5d 0a5b  ][discord-url].[
+00000f80: 215b 5765 6368 6174 5d5b 7765 6368 6174  ![Wechat][wechat
+00000f90: 2d69 6d61 6765 5d5d 5b77 6563 6861 742d  -image]][wechat-
+00000fa0: 7572 6c5d 0a5b 215b 5477 6974 7465 725d  url].[![Twitter]
+00000fb0: 5b74 7769 7474 6572 2d69 6d61 6765 5d5d  [twitter-image]]
+00000fc0: 5b74 7769 7474 6572 2d75 726c 5d0a 0a5f  [twitter-url].._
+00000fd0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00000fe0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00000ff0: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001000: 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f 5f5f  ________________
+00001010: 5f5f 5f5f 5f0a 0a23 2043 414d 454c 3a20  _____..# CAMEL: 
+00001020: 436f 6d6d 756e 6963 6174 6976 6520 4167  Communicative Ag
+00001030: 656e 7473 2066 6f72 20e2 809c 4d69 6e64  ents for ...Mind
+00001040: e280 9d20 4578 706c 6f72 6174 696f 6e20  ... Exploration 
+00001050: 6f66 204c 6172 6765 204c 616e 6775 6167  of Large Languag
+00001060: 6520 4d6f 6465 6c20 536f 6369 6574 790a  e Model Society.
+00001070: 0a5b 215b 5079 7468 6f6e 2056 6572 7369  .[![Python Versi
+00001080: 6f6e 5d5b 7079 7468 6f6e 2d69 6d61 6765  on][python-image
+00001090: 5d5d 5b70 7974 686f 6e2d 7572 6c5d 0a5b  ]][python-url].[
+000010a0: 215b 5079 5465 7374 2053 7461 7475 735d  ![PyTest Status]
+000010b0: 5b70 7974 6573 742d 696d 6167 655d 5d5b  [pytest-image]][
+000010c0: 7079 7465 7374 2d75 726c 5d0a 5b21 5b44  pytest-url].[![D
+000010d0: 6f63 756d 656e 7461 7469 6f6e 5d5b 646f  ocumentation][do
+000010e0: 6373 2d69 6d61 6765 5d5d 5b64 6f63 732d  cs-image]][docs-
+000010f0: 7572 6c5d 0a5b 215b 5374 6172 5d5b 7374  url].[![Star][st
+00001100: 6172 2d69 6d61 6765 5d5d 5b73 7461 722d  ar-image]][star-
+00001110: 7572 6c5d 0a5b 215b 5061 636b 6167 6520  url].[![Package 
+00001120: 4c69 6365 6e73 655d 5b70 6163 6b61 6765  License][package
+00001130: 2d6c 6963 656e 7365 2d69 6d61 6765 5d5d  -license-image]]
+00001140: 5b70 6163 6b61 6765 2d6c 6963 656e 7365  [package-license
+00001150: 2d75 726c 5d0a 5b21 5b44 6174 6120 4c69  -url].[![Data Li
+00001160: 6365 6e73 655d 5b64 6174 612d 6c69 6365  cense][data-lice
+00001170: 6e73 652d 696d 6167 655d 5d5b 6461 7461  nse-image]][data
+00001180: 2d6c 6963 656e 7365 2d75 726c 5d0a 0a3c  -license-url]..<
+00001190: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+000011a0: 3e0a 2020 3c61 2068 7265 663d 2268 7474  >.  <a href="htt
+000011b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000011c0: 6361 6d65 6c2d 6169 2f63 616d 656c 2363  camel-ai/camel#c
+000011d0: 6f6d 6d75 6e69 7479 223e 436f 6d6d 756e  ommunity">Commun
+000011e0: 6974 793c 2f61 3e20 7c0a 2020 3c61 2068  ity</a> |.  <a h
+000011f0: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00001200: 6875 622e 636f 6d2f 6361 6d65 6c2d 6169  hub.com/camel-ai
+00001210: 2f63 616d 656c 2369 6e73 7461 6c6c 6174  /camel#installat
+00001220: 696f 6e22 3e49 6e73 7461 6c6c 6174 696f  ion">Installatio
+00001230: 6e3c 2f61 3e20 7c0a 2020 3c61 2068 7265  n</a> |.  <a hre
+00001240: 663d 2268 7474 7073 3a2f 2f63 616d 656c  f="https://camel
+00001250: 2d61 692e 6769 7468 7562 2e69 6f2f 6361  -ai.github.io/ca
+00001260: 6d65 6c2f 223e 446f 6375 6d65 6e74 6174  mel/">Documentat
+00001270: 696f 6e3c 2f61 3e20 7c0a 2020 3c61 2068  ion</a> |.  <a h
+00001280: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00001290: 6875 622e 636f 6d2f 6361 6d65 6c2d 6169  hub.com/camel-ai
+000012a0: 2f63 616d 656c 2f74 7265 652f 4845 4144  /camel/tree/HEAD
+000012b0: 2f65 7861 6d70 6c65 7322 3e45 7861 6d70  /examples">Examp
+000012c0: 6c65 733c 2f61 3e20 7c0a 2020 3c61 2068  les</a> |.  <a h
+000012d0: 7265 663d 2268 7474 7073 3a2f 2f61 7278  ref="https://arx
+000012e0: 6976 2e6f 7267 2f61 6273 2f32 3330 332e  iv.org/abs/2303.
+000012f0: 3137 3736 3022 3e50 6170 6572 3c2f 613e  17760">Paper</a>
+00001300: 207c 0a20 203c 6120 6872 6566 3d22 6874   |.  <a href="ht
+00001310: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001320: 2f63 616d 656c 2d61 692f 6361 6d65 6c23  /camel-ai/camel#
+00001330: 6369 7461 7469 6f6e 223e 4369 7461 7469  citation">Citati
+00001340: 6f6e 3c2f 613e 207c 0a20 203c 6120 6872  on</a> |.  <a hr
+00001350: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00001360: 7562 2e63 6f6d 2f63 616d 656c 2d61 692f  ub.com/camel-ai/
+00001370: 6361 6d65 6c23 636f 6e74 7269 6275 7469  camel#contributi
+00001380: 6e67 2d74 6f2d 6361 6d65 6c2d 223e 436f  ng-to-camel-">Co
+00001390: 6e74 7269 6275 7469 6e67 3c2f 613e 207c  ntributing</a> |
+000013a0: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+000013b0: 733a 2f2f 7777 772e 6361 6d65 6c2d 6169  s://www.camel-ai
+000013c0: 2e6f 7267 2f22 3e43 414d 454c 2d41 493c  .org/">CAMEL-AI<
+000013d0: 2f61 3e0a 3c2f 703e 0a0a 3c70 2061 6c69  /a>.</p>..<p ali
+000013e0: 676e 3d22 6365 6e74 6572 223e 0a20 203c  gn="center">.  <
+000013f0: 696d 6720 7372 633d 2768 7474 7073 3a2f  img src='https:/
+00001400: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+00001410: 6f6e 7465 6e74 2e63 6f6d 2f63 616d 656c  ontent.com/camel
+00001420: 2d61 692f 6361 6d65 6c2f 6d61 7374 6572  -ai/camel/master
+00001430: 2f6d 6973 632f 7072 696d 6172 795f 6c6f  /misc/primary_lo
+00001440: 676f 2e70 6e67 2720 7769 6474 683d 3830  go.png' width=80
+00001450: 303e 0a3c 2f70 3e0a 0a23 2320 4f76 6572  0>.</p>..## Over
+00001460: 7669 6577 0a54 6865 2072 6170 6964 2061  view.The rapid a
+00001470: 6476 616e 6365 6d65 6e74 206f 6620 636f  dvancement of co
+00001480: 6e76 6572 7361 7469 6f6e 616c 2061 6e64  nversational and
+00001490: 2063 6861 742d 6261 7365 6420 6c61 6e67   chat-based lang
+000014a0: 7561 6765 206d 6f64 656c 7320 6861 7320  uage models has 
+000014b0: 6c65 6420 746f 2072 656d 6172 6b61 626c  led to remarkabl
+000014c0: 6520 7072 6f67 7265 7373 2069 6e20 636f  e progress in co
+000014d0: 6d70 6c65 7820 7461 736b 2d73 6f6c 7669  mplex task-solvi
+000014e0: 6e67 2e20 486f 7765 7665 722c 2074 6865  ng. However, the
+000014f0: 6972 2073 7563 6365 7373 2068 6561 7669  ir success heavi
+00001500: 6c79 2072 656c 6965 7320 6f6e 2068 756d  ly relies on hum
+00001510: 616e 2069 6e70 7574 2074 6f20 6775 6964  an input to guid
+00001520: 6520 7468 6520 636f 6e76 6572 7361 7469  e the conversati
+00001530: 6f6e 2c20 7768 6963 6820 6361 6e20 6265  on, which can be
+00001540: 2063 6861 6c6c 656e 6769 6e67 2061 6e64   challenging and
+00001550: 2074 696d 652d 636f 6e73 756d 696e 672e   time-consuming.
+00001560: 2054 6869 7320 7061 7065 7220 6578 706c   This paper expl
+00001570: 6f72 6573 2074 6865 2070 6f74 656e 7469  ores the potenti
+00001580: 616c 206f 6620 6275 696c 6469 6e67 2073  al of building s
+00001590: 6361 6c61 626c 6520 7465 6368 6e69 7175  calable techniqu
+000015a0: 6573 2074 6f20 6661 6369 6c69 7461 7465  es to facilitate
+000015b0: 2061 7574 6f6e 6f6d 6f75 7320 636f 6f70   autonomous coop
+000015c0: 6572 6174 696f 6e20 616d 6f6e 6720 636f  eration among co
+000015d0: 6d6d 756e 6963 6174 6976 6520 6167 656e  mmunicative agen
+000015e0: 7473 2061 6e64 2070 726f 7669 6465 2069  ts and provide i
+000015f0: 6e73 6967 6874 2069 6e74 6f20 7468 6569  nsight into thei
+00001600: 7220 2263 6f67 6e69 7469 7665 2220 7072  r "cognitive" pr
+00001610: 6f63 6573 7365 732e 2054 6f20 6164 6472  ocesses. To addr
+00001620: 6573 7320 7468 6520 6368 616c 6c65 6e67  ess the challeng
+00001630: 6573 206f 6620 6163 6869 6576 696e 6720  es of achieving 
+00001640: 6175 746f 6e6f 6d6f 7573 2063 6f6f 7065  autonomous coope
+00001650: 7261 7469 6f6e 2c20 7765 2070 726f 706f  ration, we propo
+00001660: 7365 2061 206e 6f76 656c 2063 6f6d 6d75  se a novel commu
+00001670: 6e69 6361 7469 7665 2061 6765 6e74 2066  nicative agent f
+00001680: 7261 6d65 776f 726b 206e 616d 6564 202a  ramework named *
+00001690: 726f 6c65 2d70 6c61 7969 6e67 2a2e 204f  role-playing*. O
+000016a0: 7572 2061 7070 726f 6163 6820 696e 766f  ur approach invo
+000016b0: 6c76 6573 2075 7369 6e67 202a 696e 6365  lves using *ince
+000016c0: 7074 696f 6e20 7072 6f6d 7074 696e 672a  ption prompting*
+000016d0: 2074 6f20 6775 6964 6520 6368 6174 2061   to guide chat a
+000016e0: 6765 6e74 7320 746f 7761 7264 2074 6173  gents toward tas
+000016f0: 6b20 636f 6d70 6c65 7469 6f6e 2077 6869  k completion whi
+00001700: 6c65 206d 6169 6e74 6169 6e69 6e67 2063  le maintaining c
+00001710: 6f6e 7369 7374 656e 6379 2077 6974 6820  onsistency with 
+00001720: 6875 6d61 6e20 696e 7465 6e74 696f 6e73  human intentions
+00001730: 2e20 5765 2073 686f 7763 6173 6520 686f  . We showcase ho
+00001740: 7720 726f 6c65 2d70 6c61 7969 6e67 2063  w role-playing c
+00001750: 616e 2062 6520 7573 6564 2074 6f20 6765  an be used to ge
+00001760: 6e65 7261 7465 2063 6f6e 7665 7273 6174  nerate conversat
+00001770: 696f 6e61 6c20 6461 7461 2066 6f72 2073  ional data for s
+00001780: 7475 6479 696e 6720 7468 6520 6265 6861  tudying the beha
+00001790: 7669 6f72 7320 616e 6420 6361 7061 6269  viors and capabi
+000017a0: 6c69 7469 6573 206f 6620 6368 6174 2061  lities of chat a
+000017b0: 6765 6e74 732c 2070 726f 7669 6469 6e67  gents, providing
+000017c0: 2061 2076 616c 7561 626c 6520 7265 736f   a valuable reso
+000017d0: 7572 6365 2066 6f72 2069 6e76 6573 7469  urce for investi
+000017e0: 6761 7469 6e67 2063 6f6e 7665 7273 6174  gating conversat
+000017f0: 696f 6e61 6c20 6c61 6e67 7561 6765 206d  ional language m
+00001800: 6f64 656c 732e 204f 7572 2063 6f6e 7472  odels. Our contr
+00001810: 6962 7574 696f 6e73 2069 6e63 6c75 6465  ibutions include
+00001820: 2069 6e74 726f 6475 6369 6e67 2061 206e   introducing a n
+00001830: 6f76 656c 2063 6f6d 6d75 6e69 6361 7469  ovel communicati
+00001840: 7665 2061 6765 6e74 2066 7261 6d65 776f  ve agent framewo
+00001850: 726b 2c20 6f66 6665 7269 6e67 2061 2073  rk, offering a s
+00001860: 6361 6c61 626c 6520 6170 7072 6f61 6368  calable approach
+00001870: 2066 6f72 2073 7475 6479 696e 6720 7468   for studying th
+00001880: 6520 636f 6f70 6572 6174 6976 6520 6265  e cooperative be
+00001890: 6861 7669 6f72 7320 616e 6420 6361 7061  haviors and capa
+000018a0: 6269 6c69 7469 6573 206f 6620 6d75 6c74  bilities of mult
+000018b0: 692d 6167 656e 7420 7379 7374 656d 732c  i-agent systems,
+000018c0: 2061 6e64 206f 7065 6e2d 736f 7572 6369   and open-sourci
+000018d0: 6e67 206f 7572 206c 6962 7261 7279 2074  ng our library t
+000018e0: 6f20 7375 7070 6f72 7420 7265 7365 6172  o support resear
+000018f0: 6368 206f 6e20 636f 6d6d 756e 6963 6174  ch on communicat
+00001900: 6976 6520 6167 656e 7473 2061 6e64 2062  ive agents and b
+00001910: 6579 6f6e 642e 2054 6865 2047 6974 4875  eyond. The GitHu
+00001920: 6220 7265 706f 7369 746f 7279 206f 6620  b repository of 
+00001930: 7468 6973 2070 726f 6a65 6374 2069 7320  this project is 
+00001940: 6d61 6465 2070 7562 6c69 636c 7920 6176  made publicly av
+00001950: 6169 6c61 626c 6520 6f6e 3a20 5b68 7474  ailable on: [htt
+00001960: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001970: 6361 6d65 6c2d 6169 2f63 616d 656c 5d28  camel-ai/camel](
+00001980: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001990: 6f6d 2f63 616d 656c 2d61 692f 6361 6d65  om/camel-ai/came
+000019a0: 6c29 2e0a 0a23 2320 436f 6d6d 756e 6974  l)...## Communit
+000019b0: 790a f09f 90ab 2043 414d 454c 2069 7320  y..... CAMEL is 
+000019c0: 616e 206f 7065 6e2d 736f 7572 6365 206c  an open-source l
+000019d0: 6962 7261 7279 2064 6573 6967 6e65 6420  ibrary designed 
+000019e0: 666f 7220 7468 6520 7374 7564 7920 6f66  for the study of
+000019f0: 2061 7574 6f6e 6f6d 6f75 7320 616e 6420   autonomous and 
+00001a00: 636f 6d6d 756e 6963 6174 6976 6520 6167  communicative ag
+00001a10: 656e 7473 2e20 5765 2062 656c 6965 7665  ents. We believe
+00001a20: 2074 6861 7420 7374 7564 7969 6e67 2074   that studying t
+00001a30: 6865 7365 2061 6765 6e74 7320 6f6e 2061  hese agents on a
+00001a40: 206c 6172 6765 2073 6361 6c65 206f 6666   large scale off
+00001a50: 6572 7320 7661 6c75 6162 6c65 2069 6e73  ers valuable ins
+00001a60: 6967 6874 7320 696e 746f 2074 6865 6972  ights into their
+00001a70: 2062 6568 6176 696f 7273 2c20 6361 7061   behaviors, capa
+00001a80: 6269 6c69 7469 6573 2c20 616e 6420 706f  bilities, and po
+00001a90: 7465 6e74 6961 6c20 7269 736b 732e 2054  tential risks. T
+00001aa0: 6f20 6661 6369 6c69 7461 7465 2072 6573  o facilitate res
+00001ab0: 6561 7263 6820 696e 2074 6869 7320 6669  earch in this fi
+00001ac0: 656c 642c 2077 6520 696d 706c 656d 656e  eld, we implemen
+00001ad0: 7420 616e 6420 7375 7070 6f72 7420 7661  t and support va
+00001ae0: 7269 6f75 7320 7479 7065 7320 6f66 2061  rious types of a
+00001af0: 6765 6e74 732c 2074 6173 6b73 2c20 7072  gents, tasks, pr
+00001b00: 6f6d 7074 732c 206d 6f64 656c 732c 2061  ompts, models, a
+00001b10: 6e64 2073 696d 756c 6174 6564 2065 6e76  nd simulated env
+00001b20: 6972 6f6e 6d65 6e74 732e 0a0a 4a6f 696e  ironments...Join
+00001b30: 2075 7320 285b 2a53 6c61 636b 2a5d 2868   us ([*Slack*](h
+00001b40: 7474 7073 3a2f 2f6a 6f69 6e2e 736c 6163  ttps://join.slac
+00001b50: 6b2e 636f 6d2f 742f 6361 6d65 6c2d 6169  k.com/t/camel-ai
+00001b60: 2f73 6861 7265 645f 696e 7669 7465 2f7a  /shared_invite/z
+00001b70: 742d 3267 3778 6334 3167 792d 5f37 7263  t-2g7xc41gy-_7rc
+00001b80: 724e 4e41 4172 4950 3673 4c51 716c 646b  rNNAArIP6sLQqldk
+00001b90: 7151 292c 205b 2a44 6973 636f 7264 2a5d  qQ), [*Discord*]
+00001ba0: 2868 7474 7073 3a2f 2f64 6973 636f 7264  (https://discord
+00001bb0: 2e67 672f 434e 634e 7071 7579 4463 2920  .gg/CNcNpquyDc) 
+00001bc0: 6f72 205b 2a57 6543 6861 742a 5d28 6874  or [*WeChat*](ht
+00001bd0: 7470 733a 2f2f 6768 6c69 2e6f 7267 2f63  tps://ghli.org/c
+00001be0: 616d 656c 2f77 6563 6861 742e 706e 6729  amel/wechat.png)
+00001bf0: 2920 696e 2070 7573 6869 6e67 2074 6865  ) in pushing the
+00001c00: 2062 6f75 6e64 6172 6965 7320 6f66 2062   boundaries of b
+00001c10: 7569 6c64 696e 6720 4149 2053 6f63 6965  uilding AI Socie
+00001c20: 7479 2e0a 0a23 2320 5472 7920 6974 2079  ty...## Try it y
+00001c30: 6f75 7273 656c 660a 5765 2070 726f 7669  ourself.We provi
+00001c40: 6465 2061 205b 215b 476f 6f67 6c65 2043  de a [![Google C
+00001c50: 6f6c 6162 5d28 6874 7470 733a 2f2f 636f  olab](https://co
+00001c60: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
+00001c70: 676c 652e 636f 6d2f 6173 7365 7473 2f63  gle.com/assets/c
+00001c80: 6f6c 6162 2d62 6164 6765 2e73 7667 295d  olab-badge.svg)]
+00001c90: 2868 7474 7073 3a2f 2f63 6f6c 6162 2e72  (https://colab.r
+00001ca0: 6573 6561 7263 682e 676f 6f67 6c65 2e63  esearch.google.c
+00001cb0: 6f6d 2f64 7269 7665 2f31 417a 5033 334f  om/drive/1AzP33O
+00001cc0: 3872 6e4d 575f 5f37 6f63 574a 6856 4258  8rnMW__7ocWJhVBX
+00001cd0: 6a4b 7a69 4a58 5074 696d 3f75 7370 3d73  jKziJXPtim?usp=s
+00001ce0: 6861 7269 6e67 2920 6465 6d6f 2073 686f  haring) demo sho
+00001cf0: 7763 6173 696e 6720 6120 636f 6e76 6572  wcasing a conver
+00001d00: 7361 7469 6f6e 2062 6574 7765 656e 2074  sation between t
+00001d10: 776f 2043 6861 7447 5054 2061 6765 6e74  wo ChatGPT agent
+00001d20: 7320 706c 6179 696e 6720 726f 6c65 7320  s playing roles 
+00001d30: 6173 2061 2070 7974 686f 6e20 7072 6f67  as a python prog
+00001d40: 7261 6d6d 6572 2061 6e64 2061 2073 746f  rammer and a sto
+00001d50: 636b 2074 7261 6465 7220 636f 6c6c 6162  ck trader collab
+00001d60: 6f72 6174 696e 6720 6f6e 2064 6576 656c  orating on devel
+00001d70: 6f70 696e 6720 6120 7472 6164 696e 6720  oping a trading 
+00001d80: 626f 7420 666f 7220 7374 6f63 6b20 6d61  bot for stock ma
+00001d90: 726b 6574 2e0a 0a3c 7020 616c 6967 6e3d  rket...<p align=
+00001da0: 2263 656e 7465 7222 3e0a 2020 3c69 6d67  "center">.  <img
+00001db0: 2073 7263 3d27 6874 7470 733a 2f2f 7261   src='https://ra
+00001dc0: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
+00001dd0: 656e 742e 636f 6d2f 6361 6d65 6c2d 6169  ent.com/camel-ai
+00001de0: 2f63 616d 656c 2f6d 6173 7465 722f 6d69  /camel/master/mi
+00001df0: 7363 2f66 7261 6d65 776f 726b 2e70 6e67  sc/framework.png
+00001e00: 2720 7769 6474 683d 3830 303e 0a3c 2f70  ' width=800>.</p
+00001e10: 3e0a 0a23 2320 496e 7374 616c 6c61 7469  >..## Installati
+00001e20: 6f6e 0a0a 2323 2320 4672 6f6d 2050 7950  on..### From PyP
+00001e30: 490a 0a54 6f20 696e 7374 616c 6c20 7468  I..To install th
+00001e40: 6520 6261 7365 2043 414d 454c 206c 6962  e base CAMEL lib
+00001e50: 7261 7279 3a0a 6060 6062 6173 680a 7069  rary:.```bash.pi
+00001e60: 7020 696e 7374 616c 6c20 6361 6d65 6c2d  p install camel-
+00001e70: 6169 0a60 6060 0a53 6f6d 6520 6665 6174  ai.```.Some feat
+00001e80: 7572 6573 2072 6571 7569 7265 2065 7874  ures require ext
+00001e90: 7261 2064 6570 656e 6465 6e63 6965 733a  ra dependencies:
+00001ea0: 0a2d 2054 6f20 7573 6520 7468 6520 4875  .- To use the Hu
+00001eb0: 6767 696e 6746 6163 6520 6167 656e 7473  ggingFace agents
+00001ec0: 3a0a 2020 2020 6060 6062 6173 680a 2020  :.    ```bash.  
+00001ed0: 2020 7069 7020 696e 7374 616c 6c20 2763    pip install 'c
+00001ee0: 616d 656c 2d61 695b 6875 6767 696e 6766  amel-ai[huggingf
+00001ef0: 6163 652d 6167 656e 745d 270a 2020 2020  ace-agent]'.    
+00001f00: 6060 600a 2d20 546f 2065 6e61 626c 6520  ```.- To enable 
+00001f10: 5241 4720 6f72 2075 7365 2061 6765 6e74  RAG or use agent
+00001f20: 206d 656d 6f72 793a 0a20 2020 2060 6060   memory:.    ```
+00001f30: 6261 7368 0a20 2020 2070 6970 2069 6e73  bash.    pip ins
+00001f40: 7461 6c6c 2027 6361 6d65 6c2d 6169 5b74  tall 'camel-ai[t
+00001f50: 6f6f 6c73 5d27 0a20 2020 2060 6060 0a2d  ools]'.    ```.-
+00001f60: 2054 6f20 696e 7374 616c 6c20 7769 7468   To install with
+00001f70: 2061 6c6c 2064 6570 656e 6465 6e63 6965   all dependencie
+00001f80: 733a 0a20 2020 2060 6060 6261 7368 0a20  s:.    ```bash. 
+00001f90: 2020 2070 6970 2069 6e73 7461 6c6c 2027     pip install '
+00001fa0: 6361 6d65 6c2d 6169 5b61 6c6c 5d27 0a20  camel-ai[all]'. 
+00001fb0: 2020 2060 6060 0a0a 2323 2320 4672 6f6d     ```..### From
+00001fc0: 2053 6f75 7263 650a 0a49 6e73 7461 6c6c   Source..Install
+00001fd0: 2060 4341 4d45 4c60 2066 726f 6d20 736f   `CAMEL` from so
+00001fe0: 7572 6365 2077 6974 6820 706f 6574 7279  urce with poetry
+00001ff0: 2028 5265 636f 6d6d 656e 6465 6429 3a0a   (Recommended):.
+00002000: 6060 6073 680a 2320 4d61 6b65 2073 7572  ```sh.# Make sur
+00002010: 6520 796f 7572 2070 7974 686f 6e20 7665  e your python ve
+00002020: 7273 696f 6e20 6973 206c 6174 6572 2074  rsion is later t
+00002030: 6861 6e20 332e 390a 2320 596f 7520 6361  han 3.9.# You ca
+00002040: 6e20 7573 6520 7079 656e 7620 746f 206d  n use pyenv to m
+00002050: 616e 6167 6520 6d75 6c74 6970 6c65 2070  anage multiple p
+00002060: 7974 686f 6e20 7665 7269 736f 6e73 2069  ython verisons i
+00002070: 6e20 796f 7572 2073 7974 7374 656d 0a0a  n your sytstem..
+00002080: 2320 436c 6f6e 6520 6769 7468 7562 2072  # Clone github r
+00002090: 6570 6f0a 6769 7420 636c 6f6e 6520 6874  epo.git clone ht
+000020a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000020b0: 2f63 616d 656c 2d61 692f 6361 6d65 6c2e  /camel-ai/camel.
+000020c0: 6769 740a 0a23 2043 6861 6e67 6520 6469  git..# Change di
+000020d0: 7265 6374 6f72 7920 696e 746f 2070 726f  rectory into pro
+000020e0: 6a65 6374 2064 6972 6563 746f 7279 0a63  ject directory.c
+000020f0: 6420 6361 6d65 6c0a 0a23 2041 6374 6976  d camel..# Activ
+00002100: 6174 6520 6361 6d65 6c20 7669 7274 7561  ate camel virtua
+00002110: 6c20 656e 7669 726f 6e6d 656e 740a 706f  l environment.po
+00002120: 6574 7279 2073 6865 6c6c 0a0a 2320 496e  etry shell..# In
+00002130: 7374 616c 6c20 6361 6d65 6c20 6672 6f6d  stall camel from
+00002140: 2073 6f75 7263 650a 2320 4974 2074 616b   source.# It tak
+00002150: 6573 2061 626f 7574 2039 3020 7365 636f  es about 90 seco
+00002160: 6e64 7320 746f 2072 6573 6f6c 7665 2064  nds to resolve d
+00002170: 6570 656e 6465 6e63 6965 730a 706f 6574  ependencies.poet
+00002180: 7279 2069 6e73 7461 6c6c 0a0a 2320 4f72  ry install..# Or
+00002190: 2069 6620 796f 7520 7761 6e74 2074 6f20   if you want to 
+000021a0: 7573 6520 616c 6c20 6f74 6865 7220 6578  use all other ex
+000021b0: 7472 6120 7061 636b 6167 6573 0a70 6f65  tra packages.poe
+000021c0: 7472 7920 696e 7374 616c 6c20 2d45 2061  try install -E a
+000021d0: 6c6c 2020 2320 284f 7074 696f 6e61 6c29  ll  # (Optional)
+000021e0: 0a0a 2320 4578 6974 2074 6865 2076 6972  ..# Exit the vir
+000021f0: 7475 616c 2065 6e76 6972 6f6e 6d65 6e74  tual environment
+00002200: 0a65 7869 740a 6060 600a 0a49 6e73 7461  .exit.```..Insta
+00002210: 6c6c 2060 4341 4d45 4c60 2066 726f 6d20  ll `CAMEL` from 
+00002220: 736f 7572 6365 2077 6974 6820 636f 6e64  source with cond
+00002230: 6120 616e 6420 7069 703a 0a60 6060 7368  a and pip:.```sh
+00002240: 0a23 2043 7265 6174 6520 6120 636f 6e64  .# Create a cond
+00002250: 6120 7669 7274 7561 6c20 656e 7669 726f  a virtual enviro
+00002260: 6e6d 656e 740a 636f 6e64 6120 6372 6561  nment.conda crea
+00002270: 7465 202d 2d6e 616d 6520 6361 6d65 6c20  te --name camel 
+00002280: 7079 7468 6f6e 3d33 2e31 300a 0a23 2041  python=3.10..# A
+00002290: 6374 6976 6174 6520 6361 6d65 6c20 636f  ctivate camel co
+000022a0: 6e64 6120 656e 7669 726f 6e6d 656e 740a  nda environment.
+000022b0: 636f 6e64 6120 6163 7469 7661 7465 2063  conda activate c
+000022c0: 616d 656c 0a0a 2320 436c 6f6e 6520 6769  amel..# Clone gi
+000022d0: 7468 7562 2072 6570 6f0a 6769 7420 636c  thub repo.git cl
+000022e0: 6f6e 6520 2d62 2076 302e 312e 3420 6874  one -b v0.1.4 ht
+000022f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002300: 2f63 616d 656c 2d61 692f 6361 6d65 6c2e  /camel-ai/camel.
+00002310: 6769 740a 0a23 2043 6861 6e67 6520 6469  git..# Change di
+00002320: 7265 6374 6f72 7920 696e 746f 2070 726f  rectory into pro
+00002330: 6a65 6374 2064 6972 6563 746f 7279 0a63  ject directory.c
+00002340: 6420 6361 6d65 6c0a 0a23 2049 6e73 7461  d camel..# Insta
+00002350: 6c6c 2063 616d 656c 2066 726f 6d20 736f  ll camel from so
+00002360: 7572 6365 0a70 6970 2069 6e73 7461 6c6c  urce.pip install
+00002370: 202d 6520 2e0a 0a23 204f 7220 6966 2079   -e ...# Or if y
+00002380: 6f75 2077 616e 7420 746f 2075 7365 2061  ou want to use a
+00002390: 6c6c 206f 7468 6572 2065 7874 7261 2070  ll other extra p
+000023a0: 6163 6b61 6765 730a 7069 7020 696e 7374  ackages.pip inst
+000023b0: 616c 6c20 2d65 202e 5b61 6c6c 5d20 2320  all -e .[all] # 
+000023c0: 284f 7074 696f 6e61 6c29 0a60 6060 0a0a  (Optional).```..
+000023d0: 2323 2044 6f63 756d 656e 7461 7469 6f6e  ## Documentation
+000023e0: 0a0a 5b43 414d 454c 2070 6163 6b61 6765  ..[CAMEL package
+000023f0: 2064 6f63 756d 656e 7461 7469 6f6e 2070   documentation p
+00002400: 6167 6573 5d28 6874 7470 733a 2f2f 6361  ages](https://ca
+00002410: 6d65 6c2d 6169 2e67 6974 6875 622e 696f  mel-ai.github.io
+00002420: 2f63 616d 656c 2f29 2e0a 0a23 2320 4578  /camel/)...## Ex
+00002430: 616d 706c 650a 0a59 6f75 2063 616e 2066  ample..You can f
+00002440: 696e 6420 6120 6c69 7374 206f 6620 7461  ind a list of ta
+00002450: 736b 7320 666f 7220 6469 6666 6572 656e  sks for differen
+00002460: 7420 7365 7473 206f 6620 6173 7369 7374  t sets of assist
+00002470: 616e 7420 616e 6420 7573 6572 2072 6f6c  ant and user rol
+00002480: 6520 7061 6972 7320 5b68 6572 655d 2868  e pairs [here](h
+00002490: 7474 7073 3a2f 2f64 7269 7665 2e67 6f6f  ttps://drive.goo
+000024a0: 676c 652e 636f 6d2f 6669 6c65 2f64 2f31  gle.com/file/d/1
+000024b0: 3934 5050 6153 5442 5230 376d 2d50 7a6a  94PPaSTBR07m-Pzj
+000024c0: 532d 5479 364b 6c50 4c64 4649 5051 4464  S-Ty6KlPLdFIPQDd
+000024d0: 2f76 6965 773f 7573 703d 7368 6172 655f  /view?usp=share_
+000024e0: 6c69 6e6b 292e 0a0a 4173 2061 6e20 6578  link)...As an ex
+000024f0: 616d 706c 652c 2074 6f20 7275 6e20 7468  ample, to run th
+00002500: 6520 6072 6f6c 655f 706c 6179 696e 672e  e `role_playing.
+00002510: 7079 6020 7363 7269 7074 3a0a 0a46 6972  py` script:..Fir
+00002520: 7374 2c20 796f 7520 6e65 6564 2074 6f20  st, you need to 
+00002530: 6164 6420 796f 7572 204f 7065 6e41 4920  add your OpenAI 
+00002540: 4150 4920 6b65 7920 746f 2073 7973 7465  API key to syste
+00002550: 6d20 656e 7669 726f 6e6d 656e 7420 7661  m environment va
+00002560: 7269 6162 6c65 732e 2054 6865 206d 6574  riables. The met
+00002570: 686f 6420 746f 2064 6f20 7468 6973 2064  hod to do this d
+00002580: 6570 656e 6473 206f 6e20 796f 7572 206f  epends on your o
+00002590: 7065 7261 7469 6e67 2073 7973 7465 6d20  perating system 
+000025a0: 616e 6420 7468 6520 7368 656c 6c20 796f  and the shell yo
+000025b0: 7527 7265 2075 7369 6e67 2e0a 0a2a 2a46  u're using...**F
+000025c0: 6f72 2042 6173 6820 7368 656c 6c20 284c  or Bash shell (L
+000025d0: 696e 7578 2c20 6d61 634f 532c 2047 6974  inux, macOS, Git
+000025e0: 2042 6173 6820 6f6e 2057 696e 646f 7773   Bash on Windows
+000025f0: 293a 2a2a 0a0a 6060 6062 6173 680a 2320  ):**..```bash.# 
+00002600: 4578 706f 7274 2079 6f75 7220 4f70 656e  Export your Open
+00002610: 4149 2041 5049 206b 6579 0a65 7870 6f72  AI API key.expor
+00002620: 7420 4f50 454e 4149 5f41 5049 5f4b 4559  t OPENAI_API_KEY
+00002630: 3d3c 696e 7365 7274 2079 6f75 7220 4f70  =<insert your Op
+00002640: 656e 4149 2041 5049 206b 6579 3e0a 4f50  enAI API key>.OP
+00002650: 454e 4149 5f41 5049 5f42 4153 455f 5552  ENAI_API_BASE_UR
+00002660: 4c3d 3c69 6e65 7274 2079 6f75 7220 4f70  L=<inert your Op
+00002670: 656e 4149 2041 5049 2042 4153 4520 5552  enAI API BASE UR
+00002680: 4c3e 2020 2328 5368 6f75 6c64 2079 6f75  L>  #(Should you
+00002690: 2075 7469 6c69 7a65 2061 6e20 4f70 656e   utilize an Open
+000026a0: 4149 2070 726f 7879 2073 6572 7669 6365  AI proxy service
+000026b0: 2c20 6b69 6e64 6c79 2073 7065 6369 6679  , kindly specify
+000026c0: 2074 6869 7329 0a60 6060 0a0a 2a2a 466f   this).```..**Fo
+000026d0: 7220 5769 6e64 6f77 7320 436f 6d6d 616e  r Windows Comman
+000026e0: 6420 5072 6f6d 7074 3a2a 2a0a 0a60 6060  d Prompt:**..```
+000026f0: 636d 640a 5245 4d20 6578 706f 7274 2079  cmd.REM export y
+00002700: 6f75 7220 4f70 656e 4149 2041 5049 206b  our OpenAI API k
+00002710: 6579 0a73 6574 204f 5045 4e41 495f 4150  ey.set OPENAI_AP
+00002720: 495f 4b45 593d 3c69 6e73 6572 7420 796f  I_KEY=<insert yo
+00002730: 7572 204f 7065 6e41 4920 4150 4920 6b65  ur OpenAI API ke
+00002740: 793e 0a73 6574 204f 5045 4e41 495f 4150  y>.set OPENAI_AP
+00002750: 495f 4241 5345 5f55 524c 3d3c 696e 6572  I_BASE_URL=<iner
+00002760: 7420 796f 7572 204f 7065 6e41 4920 4150  t your OpenAI AP
+00002770: 4920 4241 5345 2055 524c 3e20 2023 2853  I BASE URL>  #(S
+00002780: 686f 756c 6420 796f 7520 7574 696c 697a  hould you utiliz
+00002790: 6520 616e 204f 7065 6e41 4920 7072 6f78  e an OpenAI prox
+000027a0: 7920 7365 7276 6963 652c 206b 696e 646c  y service, kindl
+000027b0: 7920 7370 6563 6966 7920 7468 6973 290a  y specify this).
+000027c0: 6060 600a 0a2a 2a46 6f72 2057 696e 646f  ```..**For Windo
+000027d0: 7773 2050 6f77 6572 5368 656c 6c3a 2a2a  ws PowerShell:**
+000027e0: 0a0a 6060 6070 6f77 6572 7368 656c 6c0a  ..```powershell.
+000027f0: 2320 4578 706f 7274 2079 6f75 7220 4f70  # Export your Op
+00002800: 656e 4149 2041 5049 206b 6579 0a24 656e  enAI API key.$en
+00002810: 763a 4f50 454e 4149 5f41 5049 5f4b 4559  v:OPENAI_API_KEY
+00002820: 3d22 3c69 6e73 6572 7420 796f 7572 204f  ="<insert your O
+00002830: 7065 6e41 4920 4150 4920 6b65 793e 220a  penAI API key>".
+00002840: 2465 6e76 3a4f 5045 4e41 495f 4150 495f  $env:OPENAI_API_
+00002850: 4241 5345 5f55 524c 3d22 3c69 6e65 7274  BASE_URL="<inert
+00002860: 2079 6f75 7220 4f70 656e 4149 2041 5049   your OpenAI API
+00002870: 2042 4153 4520 5552 4c3e 2220 2023 2853   BASE URL>"  #(S
+00002880: 686f 756c 6420 796f 7520 7574 696c 697a  hould you utiliz
+00002890: 6520 616e 204f 7065 6e41 4920 7072 6f78  e an OpenAI prox
+000028a0: 7920 7365 7276 6963 652c 206b 696e 646c  y service, kindl
+000028b0: 7920 7370 6563 6966 7920 7468 6973 290a  y specify this).
+000028c0: 6060 600a 0a52 6570 6c61 6365 2060 3c69  ```..Replace `<i
+000028d0: 6e73 6572 7420 796f 7572 204f 7065 6e41  nsert your OpenA
+000028e0: 4920 4150 4920 6b65 793e 6020 7769 7468  I API key>` with
+000028f0: 2079 6f75 7220 6163 7475 616c 204f 7065   your actual Ope
+00002900: 6e41 4920 4150 4920 6b65 7920 696e 2065  nAI API key in e
+00002910: 6163 6820 6361 7365 2e20 4d61 6b65 2073  ach case. Make s
+00002920: 7572 6520 7468 6572 6520 6172 6520 6e6f  ure there are no
+00002930: 2073 7061 6365 7320 6172 6f75 6e64 2074   spaces around t
+00002940: 6865 2060 3d60 2073 6967 6e2e 0a0a 4166  he `=` sign...Af
+00002950: 7465 7220 7365 7474 696e 6720 7468 6520  ter setting the 
+00002960: 4f70 656e 4149 2041 5049 206b 6579 2c20  OpenAI API key, 
+00002970: 796f 7520 6361 6e20 7275 6e20 7468 6520  you can run the 
+00002980: 7363 7269 7074 3a0a 0a60 6060 6261 7368  script:..```bash
+00002990: 0a23 2059 6f75 2063 616e 2063 6861 6e67  .# You can chang
+000029a0: 6520 7468 6520 726f 6c65 2070 6169 7220  e the role pair 
+000029b0: 616e 6420 696e 6974 6961 6c20 7072 6f6d  and initial prom
+000029c0: 7074 2069 6e20 726f 6c65 5f70 6c61 7969  pt in role_playi
+000029d0: 6e67 2e70 790a 7079 7468 6f6e 2065 7861  ng.py.python exa
+000029e0: 6d70 6c65 732f 6169 5f73 6f63 6965 7479  mples/ai_society
+000029f0: 2f72 6f6c 655f 706c 6179 696e 672e 7079  /role_playing.py
+00002a00: 0a60 6060 0a0a 506c 6561 7365 206e 6f74  .```..Please not
+00002a10: 6520 7468 6174 2074 6865 2065 6e76 6972  e that the envir
+00002a20: 6f6e 6d65 6e74 2076 6172 6961 626c 6520  onment variable 
+00002a30: 6973 2073 6573 7369 6f6e 2d73 7065 6369  is session-speci
+00002a40: 6669 632e 2049 6620 796f 7520 6f70 656e  fic. If you open
+00002a50: 2061 206e 6577 2074 6572 6d69 6e61 6c20   a new terminal 
+00002a60: 7769 6e64 6f77 206f 7220 7461 622c 2079  window or tab, y
+00002a70: 6f75 2077 696c 6c20 6e65 6564 2074 6f20  ou will need to 
+00002a80: 7365 7420 7468 6520 4150 4920 6b65 7920  set the API key 
+00002a90: 6167 6169 6e20 696e 2074 6861 7420 6e65  again in that ne
+00002aa0: 7720 7365 7373 696f 6e2e 0a0a 0a23 2320  w session....## 
+00002ab0: 5573 6520 4f70 656e 2d53 6f75 7263 6520  Use Open-Source 
+00002ac0: 4d6f 6465 6c73 2061 7320 4261 636b 656e  Models as Backen
+00002ad0: 6473 0a0a 5468 6520 6261 7369 6320 776f  ds..The basic wo
+00002ae0: 726b 666c 6f77 206f 6620 7573 696e 6720  rkflow of using 
+00002af0: 616e 206f 7065 6e2d 736f 7572 6365 6420  an open-sourced 
+00002b00: 6d6f 6465 6c20 6173 2074 6865 2062 6163  model as the bac
+00002b10: 6b65 6e64 2069 7320 6261 7365 6420 6f6e  kend is based on
+00002b20: 2061 6e20 6578 7465 726e 616c 2073 6572   an external ser
+00002b30: 7665 7220 7275 6e6e 696e 6720 4c4c 4d20  ver running LLM 
+00002b40: 696e 6665 7265 6e63 6520 7365 7276 6963  inference servic
+00002b50: 652c 2065 2e67 2e20 6475 7269 6e67 2074  e, e.g. during t
+00002b60: 6865 2064 6576 656c 6f70 6d65 6e74 2077  he development w
+00002b70: 6520 6368 6f73 6520 5b46 6173 7443 6861  e chose [FastCha
+00002b80: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
+00002b90: 622e 636f 6d2f 6c6d 2d73 7973 2f46 6173  b.com/lm-sys/Fas
+00002ba0: 7443 6861 7429 2074 6f20 7275 6e20 7468  tChat) to run th
+00002bb0: 6520 7365 7276 6963 652e 0a0a 5765 2064  e service...We d
+00002bc0: 6f20 6e6f 7420 6669 7820 7468 6520 6368  o not fix the ch
+00002bd0: 6f69 6365 206f 6620 7365 7276 6572 2074  oice of server t
+00002be0: 6f20 6465 636f 7570 6c65 2074 6865 2069  o decouple the i
+00002bf0: 6d70 6c65 6d65 6e74 6174 696f 6e20 6f66  mplementation of
+00002c00: 2061 6e79 2073 7065 6369 6669 6320 4c4c   any specific LL
+00002c10: 4d20 696e 6665 7265 6e63 6520 7365 7276  M inference serv
+00002c20: 6572 2077 6974 6820 4341 4d45 4c20 2869  er with CAMEL (i
+00002c30: 6e64 6963 6174 696e 6720 7468 6520 7365  ndicating the se
+00002c40: 7276 6572 206e 6565 6473 2074 6f20 6265  rver needs to be
+00002c50: 2064 6570 6c6f 7965 6420 6279 2074 6865   deployed by the
+00002c60: 2075 7365 7220 6869 6d73 656c 6629 2e20   user himself). 
+00002c70: 4275 7420 7468 6520 7365 7276 6572 2074  But the server t
+00002c80: 6f20 6265 2064 6570 6c6f 7965 6420 6d75  o be deployed mu
+00002c90: 7374 2073 6174 6973 6679 2074 6861 7420  st satisfy that 
+00002ca0: 2a2a 6974 2073 7570 706f 7274 7320 4f70  **it supports Op
+00002cb0: 656e 4149 2d63 6f6d 7061 7469 626c 6520  enAI-compatible 
+00002cc0: 4150 4973 2c20 6573 7065 6369 616c 6c79  APIs, especially
+00002cd0: 2074 6865 206d 6574 686f 6420 606f 7065   the method `ope
+00002ce0: 6e61 692e 4368 6174 436f 6d70 6c65 7469  nai.ChatCompleti
+00002cf0: 6f6e 2e63 7265 6174 6560 2a2a 2e0a 0a48  on.create`**...H
+00002d00: 6572 6520 6172 6520 736f 6d65 2069 6e73  ere are some ins
+00002d10: 7472 7563 7469 6f6e 7320 666f 7220 656e  tructions for en
+00002d20: 6162 6c69 6e67 206f 7065 6e2d 736f 7572  abling open-sour
+00002d30: 6365 2062 6163 6b65 6e64 732c 2077 6865  ce backends, whe
+00002d40: 7265 2077 6520 7573 6520 7468 6520 5b46  re we use the [F
+00002d50: 6173 7443 6861 745d 2868 7474 7073 3a2f  astChat](https:/
+00002d60: 2f67 6974 6875 622e 636f 6d2f 6c6d 2d73  /github.com/lm-s
+00002d70: 7973 2f46 6173 7443 6861 7429 2061 6e64  ys/FastChat) and
+00002d80: 2061 204c 4c61 4d41 322d 6261 7365 6420   a LLaMA2-based 
+00002d90: 6d6f 6465 6c20 285b 606d 6574 612d 6c6c  model ([`meta-ll
+00002da0: 616d 612f 4c6c 616d 612d 322d 3762 2d63  ama/Llama-2-7b-c
+00002db0: 6861 742d 6866 605d 2868 7474 7073 3a2f  hat-hf`](https:/
+00002dc0: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
+00002dd0: 6d65 7461 2d6c 6c61 6d61 2f4c 6c61 6d61  meta-llama/Llama
+00002de0: 2d32 2d37 622d 6368 6174 2d68 6629 2920  -2-7b-chat-hf)) 
+00002df0: 696e 2074 6865 2065 7861 6d70 6c65 2e20  in the example. 
+00002e00: 506c 6561 7365 2069 6e73 7461 6c6c 2046  Please install F
+00002e10: 6173 7443 6861 7420 696e 2061 6476 616e  astChat in advan
+00002e20: 6365 2066 6f6c 6c6f 7769 6e67 2074 6865  ce following the
+00002e30: 6972 2069 6e73 7461 6c6c 6174 696f 6e20  ir installation 
+00002e40: 6775 6964 616e 6365 2e0a 0a31 2e20 4265  guidance...1. Be
+00002e50: 666f 7265 2072 756e 6e69 6e67 2043 414d  fore running CAM
+00002e60: 454c 2c20 7765 2073 686f 756c 6420 6669  EL, we should fi
+00002e70: 7273 746c 7920 6c61 756e 6368 2046 6173  rstly launch Fas
+00002e80: 7443 6861 7420 7365 7276 6572 2066 6f6c  tChat server fol
+00002e90: 6c6f 7769 6e67 2074 6865 2067 7569 6461  lowing the guida
+00002ea0: 6e63 6520 6f6e 2068 7474 7073 3a2f 2f67  nce on https://g
+00002eb0: 6974 6875 622e 636f 6d2f 6c6d 2d73 7973  ithub.com/lm-sys
+00002ec0: 2f46 6173 7443 6861 742f 626c 6f62 2f6d  /FastChat/blob/m
+00002ed0: 6169 6e2f 646f 6373 2f6f 7065 6e61 695f  ain/docs/openai_
+00002ee0: 6170 692e 6d64 2e20 5468 6520 696e 7374  api.md. The inst
+00002ef0: 7275 6374 696f 6e73 2073 756d 6d61 7269  ructions summari
+00002f00: 7a65 6420 6265 6c6f 7720 7368 6f75 6c64  zed below should
+00002f10: 2062 6520 6b65 7074 2072 756e 6e69 6e67   be kept running
+00002f20: 202a 2a69 6e20 7365 7061 7261 7465 2070   **in separate p
+00002f30: 726f 6365 7373 6573 2a2a 3a0a 0a60 6060  rocesses**:..```
+00002f40: 7368 0a23 204c 6175 6e63 6820 7468 6520  sh.# Launch the 
+00002f50: 636f 6e74 726f 6c6c 6572 0a70 7974 686f  controller.pytho
+00002f60: 6e20 2d6d 2066 6173 7463 6861 742e 7365  n -m fastchat.se
+00002f70: 7276 652e 636f 6e74 726f 6c6c 6572 0a0a  rve.controller..
+00002f80: 2320 4c61 756e 6368 2074 6865 206d 6f64  # Launch the mod
+00002f90: 656c 2077 6f72 6b65 7228 7329 0a70 7974  el worker(s).pyt
+00002fa0: 686f 6e33 202d 6d20 6661 7374 6368 6174  hon3 -m fastchat
+00002fb0: 2e73 6572 7665 2e6d 6f64 656c 5f77 6f72  .serve.model_wor
+00002fc0: 6b65 7220 2d2d 6d6f 6465 6c2d 7061 7468  ker --model-path
+00002fd0: 206d 6574 612d 6c6c 616d 612f 4c6c 616d   meta-llama/Llam
+00002fe0: 612d 322d 3762 2d63 6861 742d 6866 0a0a  a-2-7b-chat-hf..
+00002ff0: 2320 4c61 756e 6368 2074 6865 2052 4553  # Launch the RES
+00003000: 5466 756c 2041 5049 2073 6572 7665 720a  Tful API server.
+00003010: 7079 7468 6f6e 3320 2d6d 2066 6173 7463  python3 -m fastc
+00003020: 6861 742e 7365 7276 652e 6f70 656e 6169  hat.serve.openai
+00003030: 5f61 7069 5f73 6572 7665 7220 2d2d 686f  _api_server --ho
+00003040: 7374 206c 6f63 616c 686f 7374 202d 2d70  st localhost --p
+00003050: 6f72 7420 3830 3030 0a60 6060 0a0a 322e  ort 8000.```..2.
+00003060: 2041 6674 6572 206f 6273 6572 7669 6e67   After observing
+00003070: 2074 6865 2063 6f6e 7472 6f6c 6c65 7220   the controller 
+00003080: 7375 6363 6573 7366 756c 6c79 2072 6563  successfully rec
+00003090: 6569 7669 6e67 2074 6865 2068 6561 7274  eiving the heart
+000030a0: 2062 6561 7420 7369 676e 616c 2066 726f   beat signal fro
+000030b0: 6d20 7468 6520 776f 726b 6572 2c20 7468  m the worker, th
+000030c0: 6520 7365 7276 6572 2073 686f 756c 6420  e server should 
+000030d0: 6265 2072 6561 6479 2066 6f72 2075 7365  be ready for use
+000030e0: 2061 7420 6874 7470 3a2f 2f6c 6f63 616c   at http://local
+000030f0: 686f 7374 3a38 3030 302f 7631 2e0a 0a33  host:8000/v1...3
+00003100: 2e20 5468 656e 2077 6520 6361 6e20 7472  . Then we can tr
+00003110: 7920 6f6e 2072 756e 6e69 6e67 2060 726f  y on running `ro
+00003120: 6c65 5f70 6c61 7969 6e67 5f77 6974 685f  le_playing_with_
+00003130: 6f70 656e 5f73 6f75 7263 655f 6d6f 6465  open_source_mode
+00003140: 6c2e 7079 602c 2077 6865 7265 2065 6163  l.py`, where eac
+00003150: 6820 6167 656e 7420 696e 2074 6869 7320  h agent in this 
+00003160: 6578 616d 706c 6520 6973 2069 6e69 7469  example is initi
+00003170: 616c 697a 6564 2077 6974 6820 7370 6563  alized with spec
+00003180: 6966 7969 6e67 2074 6865 2060 6d6f 6465  ifying the `mode
+00003190: 6c5f 7061 7468 6020 616e 6420 6073 6572  l_path` and `ser
+000031a0: 7665 725f 7572 6c60 2c20 7369 6d69 6c61  ver_url`, simila
+000031b0: 7220 746f 2074 6865 2065 7861 6d70 6c65  r to the example
+000031c0: 2063 6f64 6520 6265 6c6f 773a 0a0a 6060   code below:..``
+000031d0: 6070 7974 686f 6e0a 7379 7374 656d 5f6d  `python.system_m
+000031e0: 6573 7361 6765 203d 2023 202e 2e2e 0a0a  essage = # .....
+000031f0: 6167 656e 745f 6b77 6172 6773 203d 2064  agent_kwargs = d
+00003200: 6963 7428 0a20 2020 206d 6f64 656c 3d6d  ict(.    model=m
+00003210: 6f64 656c 5f74 7970 652c 0a20 2020 206d  odel_type,.    m
+00003220: 6f64 656c 5f63 6f6e 6669 673d 4f70 656e  odel_config=Open
+00003230: 536f 7572 6365 436f 6e66 6967 280a 2020  SourceConfig(.  
+00003240: 2020 2020 2020 6d6f 6465 6c5f 7061 7468        model_path
+00003250: 3d22 6d65 7461 2d6c 6c61 6d61 2f4c 6c61  ="meta-llama/Lla
+00003260: 6d61 2d32 2d37 622d 6368 6174 2d68 6622  ma-2-7b-chat-hf"
+00003270: 2c0a 2020 2020 2020 2020 7365 7276 6572  ,.        server
+00003280: 5f75 726c 3d22 6874 7470 3a2f 2f6c 6f63  _url="http://loc
+00003290: 616c 686f 7374 3a38 3030 302f 7631 222c  alhost:8000/v1",
+000032a0: 0a20 2020 2029 2c0a 290a 0a61 6765 6e74  .    ),.)..agent
+000032b0: 203d 2043 6861 7441 6765 6e74 280a 2020   = ChatAgent(.  
+000032c0: 2020 7379 7374 656d 5f6d 6573 7361 6765    system_message
+000032d0: 2c0a 2020 2020 2a2a 6167 656e 745f 6b77  ,.    **agent_kw
+000032e0: 6172 6773 2c0a 290a 6060 600a 0a23 2323  args,.).```..###
+000032f0: 2053 7570 706f 7274 6564 204d 6f64 656c   Supported Model
+00003300: 730a 0a2d 204c 4c61 4d41 322d 6261 7365  s..- LLaMA2-base
+00003310: 6420 6d6f 6465 6c73 0a20 202d 2065 7861  d models.  - exa
+00003320: 6d70 6c65 3a20 5b6d 6574 612d 6c6c 616d  mple: [meta-llam
+00003330: 612f 4c6c 616d 612d 322d 3762 2d63 6861  a/Llama-2-7b-cha
+00003340: 742d 6866 5d28 6874 7470 733a 2f2f 6875  t-hf](https://hu
+00003350: 6767 696e 6766 6163 652e 636f 2f6d 6574  ggingface.co/met
+00003360: 612d 6c6c 616d 612f 4c6c 616d 612d 322d  a-llama/Llama-2-
+00003370: 3762 2d63 6861 742d 6866 290a 2d20 5669  7b-chat-hf).- Vi
+00003380: 6375 6e61 2d62 6173 6564 206d 6f64 656c  cuna-based model
+00003390: 730a 2020 2d20 6578 616d 706c 653a 205b  s.  - example: [
+000033a0: 6c6d 7379 732f 7669 6375 6e61 2d37 622d  lmsys/vicuna-7b-
+000033b0: 7631 2e35 5d28 6874 7470 733a 2f2f 6875  v1.5](https://hu
+000033c0: 6767 696e 6766 6163 652e 636f 2f6c 6d73  ggingface.co/lms
+000033d0: 7973 2f76 6963 756e 612d 3762 2d76 312e  ys/vicuna-7b-v1.
+000033e0: 3529 0a0a 2323 2044 6174 6120 2848 6f73  5)..## Data (Hos
+000033f0: 7465 6420 6f6e 2048 7567 6769 6e67 2046  ted on Hugging F
+00003400: 6163 6529 0a7c 2044 6174 6173 6574 2020  ace).| Dataset  
+00003410: 2020 2020 2020 7c20 4368 6174 2066 6f72        | Chat for
+00003420: 6d61 7420 2020 2020 2020 2020 2020 2020  mat             
+00003430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003470: 2020 2020 2020 2020 2020 2020 7c20 496e              | In
+00003480: 7374 7275 6374 696f 6e20 666f 726d 6174  struction format
+00003490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034e0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000034f0: 2043 6861 7420 666f 726d 6174 2028 7472   Chat format (tr
+00003500: 616e 736c 6174 6564 2920 2020 2020 2020  anslated)       
+00003510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003540: 2020 2020 2020 2020 2020 2020 7c0a 7c2d              |.|-
+00003550: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
+00003560: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003570: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003580: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003590: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000035a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000035b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000035c0: 2d2d 2d2d 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d  -----|----------
+000035d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000035e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000035f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003620: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003630: 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d 2d2d  --------|-------
+00003640: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003670: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003690: 2d2d 2d2d 2d7c 0a7c 202a 2a41 4920 536f  -----|.| **AI So
+000036a0: 6369 6574 792a 2a20 7c20 5b43 6861 7420  ciety** | [Chat 
+000036b0: 666f 726d 6174 5d28 6874 7470 733a 2f2f  format](https://
+000036c0: 6875 6767 696e 6766 6163 652e 636f 2f64  huggingface.co/d
+000036d0: 6174 6173 6574 732f 6361 6d65 6c2d 6169  atasets/camel-ai
+000036e0: 2f61 695f 736f 6369 6574 792f 626c 6f62  /ai_society/blob
+000036f0: 2f6d 6169 6e2f 6169 5f73 6f63 6965 7479  /main/ai_society
+00003700: 5f63 6861 742e 7461 722e 677a 2920 7c20  _chat.tar.gz) | 
+00003710: 5b49 6e73 7472 7563 7469 6f6e 2066 6f72  [Instruction for
+00003720: 6d61 745d 2868 7474 7073 3a2f 2f68 7567  mat](https://hug
+00003730: 6769 6e67 6661 6365 2e63 6f2f 6461 7461  gingface.co/data
+00003740: 7365 7473 2f63 616d 656c 2d61 692f 6169  sets/camel-ai/ai
+00003750: 5f73 6f63 6965 7479 2f62 6c6f 622f 6d61  _society/blob/ma
+00003760: 696e 2f61 695f 736f 6369 6574 795f 696e  in/ai_society_in
+00003770: 7374 7275 6374 696f 6e73 2e6a 736f 6e29  structions.json)
+00003780: 207c 205b 4368 6174 2066 6f72 6d61 7420   | [Chat format 
+00003790: 2874 7261 6e73 6c61 7465 6429 5d28 6874  (translated)](ht
+000037a0: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
+000037b0: 652e 636f 2f64 6174 6173 6574 732f 6361  e.co/datasets/ca
+000037c0: 6d65 6c2d 6169 2f61 695f 736f 6369 6574  mel-ai/ai_societ
+000037d0: 795f 7472 616e 736c 6174 6564 2920 7c0a  y_translated) |.
+000037e0: 7c20 2a2a 436f 6465 2a2a 2020 2020 2020  | **Code**      
+000037f0: 207c 205b 4368 6174 2066 6f72 6d61 745d   | [Chat format]
+00003800: 2868 7474 7073 3a2f 2f68 7567 6769 6e67  (https://hugging
+00003810: 6661 6365 2e63 6f2f 6461 7461 7365 7473  face.co/datasets
+00003820: 2f63 616d 656c 2d61 692f 636f 6465 2f62  /camel-ai/code/b
+00003830: 6c6f 622f 6d61 696e 2f63 6f64 655f 6368  lob/main/code_ch
+00003840: 6174 2e74 6172 2e67 7a29 2020 2020 2020  at.tar.gz)      
+00003850: 2020 2020 2020 207c 205b 496e 7374 7275         | [Instru
+00003860: 6374 696f 6e20 666f 726d 6174 5d28 6874  ction format](ht
+00003870: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
+00003880: 652e 636f 2f64 6174 6173 6574 732f 6361  e.co/datasets/ca
+00003890: 6d65 6c2d 6169 2f63 6f64 652f 626c 6f62  mel-ai/code/blob
+000038a0: 2f6d 6169 6e2f 636f 6465 5f69 6e73 7472  /main/code_instr
+000038b0: 7563 7469 6f6e 732e 6a73 6f6e 2920 2020  uctions.json)   
+000038c0: 2020 2020 2020 2020 2020 7c20 7820 2020            | x   
+000038d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000038e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038f0: 2020 2020 2020 2020 207c 2078 2020 2020           | x    
+000038f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003900: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003960: 2020 2020 2020 2020 2020 2020 7c20 7820              | x 
-00003970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003920: 2020 2020 2020 207c 0a7c 202a 2a4d 6174         |.| **Mat
+00003930: 682a 2a20 2020 2020 2020 7c20 5b43 6861  h**       | [Cha
+00003940: 7420 666f 726d 6174 5d28 6874 7470 733a  t format](https:
+00003950: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
+00003960: 2f64 6174 6173 6574 732f 6361 6d65 6c2d  /datasets/camel-
+00003970: 6169 2f6d 6174 6829 2020 2020 2020 2020  ai/math)        
 00003980: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039a0: 7c20 7820 2020 2020 2020 2020 2020 2020  | x             
 000039b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039c0: 2020 2020 2020 2020 207c 0a7c 202a 2a43           |.| **C
-000039d0: 6865 6d69 7374 7279 2a2a 2020 7c20 5b43  hemistry**  | [C
-000039e0: 6861 7420 666f 726d 6174 5d28 6874 7470  hat format](http
-000039f0: 733a 2f2f 6875 6767 696e 6766 6163 652e  s://huggingface.
-00003a00: 636f 2f64 6174 6173 6574 732f 6361 6d65  co/datasets/came
-00003a10: 6c2d 6169 2f63 6865 6d69 7374 7279 2920  l-ai/chemistry) 
+000039c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a10: 2020 207c 2078 2020 2020 2020 2020 2020     | x          
 00003a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a40: 2020 7c20 7820 2020 2020 2020 2020 2020    | x           
+00003a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ab0: 2020 2020 207c 2078 2020 2020 2020 2020       | x        
-00003ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a70: 7c0a 7c20 2a2a 5068 7973 6963 732a 2a20  |.| **Physics** 
+00003a80: 2020 207c 205b 4368 6174 2066 6f72 6d61     | [Chat forma
+00003a90: 745d 2868 7474 7073 3a2f 2f68 7567 6769  t](https://huggi
+00003aa0: 6e67 6661 6365 2e63 6f2f 6461 7461 7365  ngface.co/datase
+00003ab0: 7473 2f63 616d 656c 2d61 692f 7068 7973  ts/camel-ai/phys
+00003ac0: 6963 7329 2020 2020 2020 2020 2020 2020  ics)            
 00003ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ae0: 2020 2020 2020 2020 207c 2078 2020 2020           | x    
 00003af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b10: 2020 7c0a 7c20 2a2a 4269 6f6c 6f67 792a    |.| **Biology*
-00003b20: 2a20 2020 207c 205b 4368 6174 2066 6f72  *    | [Chat for
-00003b30: 6d61 745d 2868 7474 7073 3a2f 2f68 7567  mat](https://hug
-00003b40: 6769 6e67 6661 6365 2e63 6f2f 6461 7461  gingface.co/data
-00003b50: 7365 7473 2f63 616d 656c 2d61 692f 6269  sets/camel-ai/bi
-00003b60: 6f6c 6f67 7929 2020 2020 2020 2020 2020  ology)          
+00003b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b50: 2020 2020 2020 2020 2020 2020 7c20 7820              | x 
+00003b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b80: 2020 2020 2020 2020 2020 207c 2078 2020             | x  
+00003b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bf0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00003c00: 7820 2020 2020 2020 2020 2020 2020 2020  x               
+00003bb0: 2020 2020 2020 2020 207c 0a7c 202a 2a43           |.| **C
+00003bc0: 6865 6d69 7374 7279 2a2a 2020 7c20 5b43  hemistry**  | [C
+00003bd0: 6861 7420 666f 726d 6174 5d28 6874 7470  hat format](http
+00003be0: 733a 2f2f 6875 6767 696e 6766 6163 652e  s://huggingface.
+00003bf0: 636f 2f64 6174 6173 6574 732f 6361 6d65  co/datasets/came
+00003c00: 6c2d 6169 2f63 6865 6d69 7374 7279 2920  l-ai/chemistry) 
 00003c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c30: 2020 7c20 7820 2020 2020 2020 2020 2020    | x           
 00003c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c50: 2020 2020 2020 2020 2020 207c 0a0a 2323             |..##
-00003c60: 2056 6973 7561 6c69 7a61 7469 6f6e 7320   Visualizations 
-00003c70: 6f66 2049 6e73 7472 7563 7469 6f6e 7320  of Instructions 
-00003c80: 616e 6420 5461 736b 730a 0a7c 2044 6174  and Tasks..| Dat
-00003c90: 6173 6574 2020 2020 2020 2020 2020 7c20  aset          | 
-00003ca0: 496e 7374 7275 6374 696f 6e73 2020 2020  Instructions    
+00003c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ca0: 2020 2020 207c 2078 2020 2020 2020 2020       | x        
 00003cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d10: 2020 2020 207c 2054 6173 6b73 2020 2020       | Tasks    
-00003d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d00: 2020 7c0a 7c20 2a2a 4269 6f6c 6f67 792a    |.| **Biology*
+00003d10: 2a20 2020 207c 205b 4368 6174 2066 6f72  *    | [Chat for
+00003d20: 6d61 745d 2868 7474 7073 3a2f 2f68 7567  mat](https://hug
+00003d30: 6769 6e67 6661 6365 2e63 6f2f 6461 7461  gingface.co/data
+00003d40: 7365 7473 2f63 616d 656c 2d61 692f 6269  sets/camel-ai/bi
+00003d50: 6f6c 6f67 7929 2020 2020 2020 2020 2020  ology)          
 00003d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d80: 2020 2020 207c 0a7c 2d2d 2d2d 2d2d 2d2d       |.|--------
-00003d90: 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d  ----------|-----
-00003da0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003db0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003dd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003de0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003df0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003e00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003e10: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|--------------
-00003e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003e30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003e50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003e70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003e80: 2d7c 0a7c 202a 2a41 4920 536f 6369 6574  -|.| **AI Societ
-00003e90: 792a 2a20 2020 7c20 5b49 6e73 7472 7563  y**   | [Instruc
-00003ea0: 7469 6f6e 735d 2868 7474 7073 3a2f 2f61  tions](https://a
-00003eb0: 746c 6173 2e6e 6f6d 6963 2e61 692f 6d61  tlas.nomic.ai/ma
-00003ec0: 702f 3361 3535 3961 3036 2d38 3764 302d  p/3a559a06-87d0-
-00003ed0: 3434 3736 2d61 3837 392d 3936 3236 3536  4476-a879-962656
-00003ee0: 3234 3234 3532 2f64 6239 3631 3931 352d  242452/db961915-
-00003ef0: 6232 3534 2d34 3865 382d 3865 3563 2d39  b254-48e8-8e5c-9
-00003f00: 3137 6638 3237 6237 3463 3629 207c 205b  17f827b74c6) | [
-00003f10: 5461 736b 735d 2868 7474 7073 3a2f 2f61  Tasks](https://a
-00003f20: 746c 6173 2e6e 6f6d 6963 2e61 692f 6d61  tlas.nomic.ai/ma
-00003f30: 702f 6362 3936 6634 3162 2d61 3666 642d  p/cb96f41b-a6fd-
-00003f40: 3466 6534 2d61 6334 302d 3038 6531 3031  4fe4-ac40-08e101
-00003f50: 3731 3434 3833 2f61 6530 3631 3536 632d  714483/ae06156c-
-00003f60: 6135 3732 2d34 3665 392d 3833 3435 2d65  a572-46e9-8345-e
-00003f70: 6265 3138 3538 3664 3032 6229 207c 0a7c  be18586d02b) |.|
-00003f80: 202a 2a43 6f64 652a 2a20 2020 2020 2020   **Code**       
-00003f90: 2020 7c20 5b49 6e73 7472 7563 7469 6f6e    | [Instruction
-00003fa0: 735d 2868 7474 7073 3a2f 2f61 746c 6173  s](https://atlas
-00003fb0: 2e6e 6f6d 6963 2e61 692f 6d61 702f 3930  .nomic.ai/map/90
-00003fc0: 3264 3663 6362 2d30 6262 622d 3432 3934  2d6ccb-0bbb-4294
-00003fd0: 2d38 3361 382d 3163 3764 3264 6165 3033  -83a8-1c7d2dae03
-00003fe0: 6338 2f61 6365 3265 3134 362d 6534 3966  c8/ace2e146-e49f
-00003ff0: 2d34 3164 622d 6131 6634 2d32 3561 3263  -41db-a1f4-25a2c
-00004000: 3462 6532 3435 3729 207c 205b 5461 736b  4be2457) | [Task
-00004010: 735d 2868 7474 7073 3a2f 2f61 746c 6173  s](https://atlas
-00004020: 2e6e 6f6d 6963 2e61 692f 6d61 702f 6566  .nomic.ai/map/ef
-00004030: 6333 3836 3137 2d39 3138 302d 3439 3061  c38617-9180-490a
-00004040: 2d38 3633 302d 3433 6130 3562 3335 6432  -8630-43a05b35d2
-00004050: 3264 2f32 3537 3661 6464 662d 6131 3333  2d/2576addf-a133
-00004060: 2d34 3564 352d 3839 6139 2d36 6230 3637  -45d5-89a9-6b067
-00004070: 6236 3635 3264 6429 207c 0a7c 202a 2a4d  b6652dd) |.| **M
-00004080: 6973 616c 6967 6e6d 656e 742a 2a20 7c20  isalignment** | 
-00004090: 5b49 6e73 7472 7563 7469 6f6e 735d 2868  [Instructions](h
-000040a0: 7474 7073 3a2f 2f61 746c 6173 2e6e 6f6d  ttps://atlas.nom
-000040b0: 6963 2e61 692f 6d61 702f 3563 3439 3130  ic.ai/map/5c4910
-000040c0: 3335 2d61 3236 652d 3461 3035 2d39 3539  35-a26e-4a05-959
-000040d0: 332d 3832 6666 6232 6333 6162 3430 2f32  3-82ffb2c3ab40/2
-000040e0: 6264 3938 3839 362d 3839 3465 2d34 3830  bd98896-894e-480
-000040f0: 372d 3965 6438 2d61 3230 3363 6362 3134  7-9ed8-a203ccb14
-00004100: 6435 6529 207c 205b 5461 736b 735d 2868  d5e) | [Tasks](h
-00004110: 7474 7073 3a2f 2f61 746c 6173 2e6e 6f6d  ttps://atlas.nom
-00004120: 6963 2e61 692f 6d61 702f 6162 6333 3537  ic.ai/map/abc357
-00004130: 6464 2d39 6330 342d 3439 3133 2d39 3534  dd-9c04-4913-954
-00004140: 312d 3633 6532 3539 6437 6163 3166 2f38  1-63e259d7ac1f/8
-00004150: 3235 3133 3961 342d 6166 3636 2d34 3237  25139a4-af66-427
-00004160: 632d 3964 3065 2d66 3336 6235 3439 3261  c-9d0e-f36b5492a
-00004170: 6233 6629 207c 0a0a 2323 2049 6d70 6c65  b3f) |..## Imple
-00004180: 6d65 6e74 6564 2052 6573 6561 7263 6820  mented Research 
-00004190: 4964 6561 7320 6672 6f6d 204f 7468 6572  Ideas from Other
-000041a0: 2057 6f72 6b73 0a57 6520 696d 706c 656d   Works.We implem
-000041b0: 656e 7465 6420 616d 617a 696e 6720 7265  ented amazing re
-000041c0: 7365 6172 6368 2069 6465 6173 2066 726f  search ideas fro
-000041d0: 6d20 6f74 6865 7220 776f 726b 7320 666f  m other works fo
-000041e0: 7220 796f 7520 746f 2062 7569 6c64 2c20  r you to build, 
-000041f0: 636f 6d70 6172 6520 616e 6420 6375 7374  compare and cust
-00004200: 6f6d 697a 6520 796f 7572 2061 6765 6e74  omize your agent
-00004210: 732e 2049 6620 796f 7520 7573 6520 616e  s. If you use an
-00004220: 7920 6f66 2074 6865 7365 206d 6f64 756c  y of these modul
-00004230: 6573 2c20 706c 6561 7365 206b 696e 646c  es, please kindl
-00004240: 7920 6369 7465 2074 6865 206f 7269 6769  y cite the origi
-00004250: 6e61 6c20 776f 726b 733a 0a2d 2060 5461  nal works:.- `Ta
-00004260: 736b 4372 6561 7469 6f6e 4167 656e 7460  skCreationAgent`
-00004270: 2c20 6054 6173 6b50 7269 6f72 6974 697a  , `TaskPrioritiz
-00004280: 6174 696f 6e41 6765 6e74 6020 616e 6420  ationAgent` and 
-00004290: 6042 6162 7941 4749 6020 6672 6f6d 202a  `BabyAGI` from *
-000042a0: 4e61 6b61 6a69 6d61 2065 7420 616c 2e2a  Nakajima et al.*
-000042b0: 3a20 5b54 6173 6b2d 4472 6976 656e 2041  : [Task-Driven A
-000042c0: 7574 6f6e 6f6d 6f75 7320 4167 656e 745d  utonomous Agent]
-000042d0: 2868 7474 7073 3a2f 2f79 6f68 6569 6e61  (https://yoheina
-000042e0: 6b61 6a69 6d61 2e63 6f6d 2f74 6173 6b2d  kajima.com/task-
-000042f0: 6472 6976 656e 2d61 7574 6f6e 6f6d 6f75  driven-autonomou
-00004300: 732d 6167 656e 742d 7574 696c 697a 696e  s-agent-utilizin
-00004310: 672d 6770 742d 342d 7069 6e65 636f 6e65  g-gpt-4-pinecone
-00004320: 2d61 6e64 2d6c 616e 6763 6861 696e 2d66  -and-langchain-f
-00004330: 6f72 2d64 6976 6572 7365 2d61 7070 6c69  or-diverse-appli
-00004340: 6361 7469 6f6e 732f 292e 205b 5b45 7861  cations/). [[Exa
-00004350: 6d70 6c65 5d28 6874 7470 733a 2f2f 6769  mple](https://gi
-00004360: 7468 7562 2e63 6f6d 2f63 616d 656c 2d61  thub.com/camel-a
-00004370: 692f 6361 6d65 6c2f 626c 6f62 2f6d 6173  i/camel/blob/mas
-00004380: 7465 722f 6578 616d 706c 6573 2f61 695f  ter/examples/ai_
-00004390: 736f 6369 6574 792f 6261 6279 6167 695f  society/babyagi_
-000043a0: 706c 6179 696e 672e 7079 295d 0a0a 2323  playing.py)]..##
-000043b0: 204e 6577 730a 2d20 5265 6c65 6173 6564   News.- Released
-000043c0: 2041 4920 536f 6369 6574 7920 616e 6420   AI Society and 
-000043d0: 436f 6465 2064 6174 6173 6574 2028 4170  Code dataset (Ap
-000043e0: 7269 6c20 322c 2032 3032 3329 0a2d 2049  ril 2, 2023).- I
-000043f0: 6e69 7469 616c 2072 656c 6561 7365 206f  nitial release o
-00004400: 6620 6043 414d 454c 6020 7079 7468 6f6e  f `CAMEL` python
-00004410: 206c 6962 7261 7279 2028 4d61 7263 6820   library (March 
-00004420: 3231 2c20 3230 3233 290a 0a23 2320 4369  21, 2023)..## Ci
-00004430: 7461 7469 6f6e 0a60 6060 0a40 696e 7072  tation.```.@inpr
-00004440: 6f63 6565 6469 6e67 737b 6c69 3230 3233  oceedings{li2023
-00004450: 6361 6d65 6c2c 0a20 2074 6974 6c65 3d7b  camel,.  title={
-00004460: 4341 4d45 4c3a 2043 6f6d 6d75 6e69 6361  CAMEL: Communica
-00004470: 7469 7665 2041 6765 6e74 7320 666f 7220  tive Agents for 
-00004480: 224d 696e 6422 2045 7870 6c6f 7261 7469  "Mind" Explorati
-00004490: 6f6e 206f 6620 4c61 7267 6520 4c61 6e67  on of Large Lang
-000044a0: 7561 6765 204d 6f64 656c 2053 6f63 6965  uage Model Socie
-000044b0: 7479 7d2c 0a20 2061 7574 686f 723d 7b4c  ty},.  author={L
-000044c0: 692c 2047 756f 6861 6f20 616e 6420 4861  i, Guohao and Ha
-000044d0: 6d6d 6f75 642c 2048 6173 616e 2041 6265  mmoud, Hasan Abe
-000044e0: 6420 416c 204b 6164 6572 2061 6e64 2049  d Al Kader and I
-000044f0: 7461 6e69 2c20 4861 6e69 2061 6e64 204b  tani, Hani and K
-00004500: 6869 7a62 756c 6c69 6e2c 2044 6d69 7472  hizbullin, Dmitr
-00004510: 6969 2061 6e64 2047 6861 6e65 6d2c 2042  ii and Ghanem, B
-00004520: 6572 6e61 7264 7d2c 0a20 2062 6f6f 6b74  ernard},.  bookt
-00004530: 6974 6c65 3d7b 5468 6972 7479 2d73 6576  itle={Thirty-sev
-00004540: 656e 7468 2043 6f6e 6665 7265 6e63 6520  enth Conference 
-00004550: 6f6e 204e 6575 7261 6c20 496e 666f 726d  on Neural Inform
-00004560: 6174 696f 6e20 5072 6f63 6573 7369 6e67  ation Processing
-00004570: 2053 7973 7465 6d73 7d2c 0a20 2079 6561   Systems},.  yea
-00004580: 723d 7b32 3032 337d 0a7d 0a60 6060 0a23  r={2023}.}.```.#
-00004590: 2320 4163 6b6e 6f77 6c65 6467 656d 656e  # Acknowledgemen
-000045a0: 740a 5370 6563 6961 6c20 7468 616e 6b73  t.Special thanks
-000045b0: 2074 6f20 5b4e 6f6d 6963 2041 495d 2868   to [Nomic AI](h
-000045c0: 7474 7073 3a2f 2f68 6f6d 652e 6e6f 6d69  ttps://home.nomi
-000045d0: 632e 6169 2f29 2066 6f72 2067 6976 696e  c.ai/) for givin
-000045e0: 6720 7573 2065 7874 656e 6465 6420 6163  g us extended ac
-000045f0: 6365 7373 2074 6f20 7468 6569 7220 6461  cess to their da
-00004600: 7461 2073 6574 2065 7870 6c6f 7261 7469  ta set explorati
-00004610: 6f6e 2074 6f6f 6c20 2841 746c 6173 292e  on tool (Atlas).
-00004620: 0a0a 5765 2077 6f75 6c64 2061 6c73 6f20  ..We would also 
-00004630: 6c69 6b65 2074 6f20 7468 616e 6b20 4861  like to thank Ha
-00004640: 7961 2048 616d 6d6f 7564 2066 6f72 2064  ya Hammoud for d
-00004650: 6573 6967 6e69 6e67 2074 6865 2069 6e69  esigning the ini
-00004660: 7469 616c 206c 6f67 6f20 6f66 206f 7572  tial logo of our
-00004670: 2070 726f 6a65 6374 2e0a 0a23 2320 4c69   project...## Li
-00004680: 6365 6e73 650a 0a54 6865 2073 6f75 7263  cense..The sourc
-00004690: 6520 636f 6465 2069 7320 6c69 6365 6e73  e code is licens
-000046a0: 6564 2075 6e64 6572 2041 7061 6368 6520  ed under Apache 
-000046b0: 322e 302e 0a0a 5468 6520 6461 7461 7365  2.0...The datase
-000046c0: 7473 2061 7265 206c 6963 656e 7365 6420  ts are licensed 
-000046d0: 756e 6465 7220 4343 2042 5920 4e43 2034  under CC BY NC 4
-000046e0: 2e30 2c20 7768 6963 6820 7065 726d 6974  .0, which permit
-000046f0: 7320 6f6e 6c79 206e 6f6e 2d63 6f6d 6d65  s only non-comme
-00004700: 7263 6961 6c20 7573 6167 652e 2049 7420  rcial usage. It 
-00004710: 6973 2061 6476 6973 6564 2074 6861 7420  is advised that 
-00004720: 616e 7920 6d6f 6465 6c73 2074 7261 696e  any models train
-00004730: 6564 2075 7369 6e67 2074 6865 2064 6174  ed using the dat
-00004740: 6173 6574 2073 686f 756c 6420 6e6f 7420  aset should not 
-00004750: 6265 2075 7469 6c69 7a65 6420 666f 7220  be utilized for 
-00004760: 616e 7974 6869 6e67 206f 7468 6572 2074  anything other t
-00004770: 6861 6e20 7265 7365 6172 6368 2070 7572  han research pur
-00004780: 706f 7365 732e 0a0a 2323 2043 6f6e 7472  poses...## Contr
-00004790: 6962 7574 696e 6720 746f 2043 414d 454c  ibuting to CAMEL
-000047a0: 20f0 9f90 ab0a 5765 2061 7070 7265 6369   .....We appreci
-000047b0: 6174 6520 796f 7572 2069 6e74 6572 6573  ate your interes
-000047c0: 7420 696e 2063 6f6e 7472 6962 7574 696e  t in contributin
-000047d0: 6720 746f 206f 7572 206f 7065 6e2d 736f  g to our open-so
-000047e0: 7572 6365 2069 6e69 7469 6174 6976 652e  urce initiative.
-000047f0: 2057 6520 7072 6f76 6964 6520 6120 646f   We provide a do
-00004800: 6375 6d65 6e74 206f 6620 5b63 6f6e 7472  cument of [contr
-00004810: 6962 7574 696e 6720 6775 6964 656c 696e  ibuting guidelin
-00004820: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
-00004830: 7562 2e63 6f6d 2f63 616d 656c 2d61 692f  ub.com/camel-ai/
-00004840: 6361 6d65 6c2f 626c 6f62 2f6d 6173 7465  camel/blob/maste
-00004850: 722f 434f 4e54 5249 4255 5449 4e47 2e6d  r/CONTRIBUTING.m
-00004860: 6429 2077 6869 6368 206f 7574 6c69 6e65  d) which outline
-00004870: 7320 7468 6520 7374 6570 7320 666f 7220  s the steps for 
-00004880: 636f 6e74 7269 6275 7469 6e67 2074 6f20  contributing to 
-00004890: 4341 4d45 4c2e 2050 6c65 6173 6520 7265  CAMEL. Please re
-000048a0: 6665 7220 746f 2074 6869 7320 6775 6964  fer to this guid
-000048b0: 6520 746f 2065 6e73 7572 6520 736d 6f6f  e to ensure smoo
-000048c0: 7468 2063 6f6c 6c61 626f 7261 7469 6f6e  th collaboration
-000048d0: 2061 6e64 2073 7563 6365 7373 6675 6c20   and successful 
-000048e0: 636f 6e74 7269 6275 7469 6f6e 732e 20f0  contributions. .
-000048f0: 9fa4 9df0 9f9a 800a 0a23 2320 436f 6e74  .........## Cont
-00004900: 6163 740a 466f 7220 6d6f 7265 2069 6e66  act.For more inf
-00004910: 6f72 6d61 7469 6f6e 2070 6c65 6173 6520  ormation please 
-00004920: 636f 6e74 6163 7420 6361 6d65 6c2e 6169  contact camel.ai
-00004930: 2e74 6561 6d40 676d 6169 6c2e 636f 6d2e  .team@gmail.com.
-00004940: 0a0a 5b70 7974 686f 6e2d 696d 6167 655d  ..[python-image]
-00004950: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
-00004960: 6965 6c64 732e 696f 2f62 6164 6765 2f50  ields.io/badge/P
-00004970: 7974 686f 6e2d 332e 3925 3242 2d62 7269  ython-3.9%2B-bri
-00004980: 6768 7467 7265 656e 2e73 7667 0a5b 7079  ghtgreen.svg.[py
-00004990: 7468 6f6e 2d75 726c 5d3a 2068 7474 7073  thon-url]: https
-000049a0: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
-000049b0: 7267 2f33 2e39 2f0a 5b70 7974 6573 742d  rg/3.9/.[pytest-
-000049c0: 696d 6167 655d 3a20 6874 7470 733a 2f2f  image]: https://
-000049d0: 6769 7468 7562 2e63 6f6d 2f63 616d 656c  github.com/camel
-000049e0: 2d61 692f 6361 6d65 6c2f 6163 7469 6f6e  -ai/camel/action
-000049f0: 732f 776f 726b 666c 6f77 732f 7079 7465  s/workflows/pyte
-00004a00: 7374 5f70 6163 6b61 6765 2e79 6d6c 2f62  st_package.yml/b
-00004a10: 6164 6765 2e73 7667 0a5b 7079 7465 7374  adge.svg.[pytest
-00004a20: 2d75 726c 5d3a 2068 7474 7073 3a2f 2f67  -url]: https://g
-00004a30: 6974 6875 622e 636f 6d2f 6361 6d65 6c2d  ithub.com/camel-
-00004a40: 6169 2f63 616d 656c 2f61 6374 696f 6e73  ai/camel/actions
-00004a50: 2f77 6f72 6b66 6c6f 7773 2f70 7974 6573  /workflows/pytes
-00004a60: 745f 7061 636b 6167 652e 796d 6c0a 5b64  t_package.yml.[d
-00004a70: 6f63 732d 696d 6167 655d 3a20 6874 7470  ocs-image]: http
-00004a80: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00004a90: 696f 2f62 6164 6765 2f44 6f63 756d 656e  io/badge/Documen
-00004aa0: 7461 7469 6f6e 2d67 7265 792e 7376 673f  tation-grey.svg?
-00004ab0: 6c6f 676f 3d67 6974 6875 620a 5b64 6f63  logo=github.[doc
-00004ac0: 732d 7572 6c5d 3a20 6874 7470 733a 2f2f  s-url]: https://
-00004ad0: 6361 6d65 6c2d 6169 2e67 6974 6875 622e  camel-ai.github.
-00004ae0: 696f 2f63 616d 656c 2f69 6e64 6578 2e68  io/camel/index.h
-00004af0: 746d 6c0a 5b73 7461 722d 696d 6167 655d  tml.[star-image]
-00004b00: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
-00004b10: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
-00004b20: 7374 6172 732f 6361 6d65 6c2d 6169 2f63  stars/camel-ai/c
-00004b30: 616d 656c 3f6c 6162 656c 3d73 7461 7273  amel?label=stars
-00004b40: 266c 6f67 6f3d 6769 7468 7562 2663 6f6c  &logo=github&col
-00004b50: 6f72 3d62 7269 6768 7467 7265 656e 0a5b  or=brightgreen.[
-00004b60: 7374 6172 2d75 726c 5d3a 2068 7474 7073  star-url]: https
-00004b70: 3a2f 2f67 6974 6875 622e 636f 6d2f 6361  ://github.com/ca
-00004b80: 6d65 6c2d 6169 2f63 616d 656c 2f73 7461  mel-ai/camel/sta
-00004b90: 7267 617a 6572 730a 5b70 6163 6b61 6765  rgazers.[package
-00004ba0: 2d6c 6963 656e 7365 2d69 6d61 6765 5d3a  -license-image]:
-00004bb0: 2068 7474 7073 3a2f 2f69 6d67 2e73 6869   https://img.shi
-00004bc0: 656c 6473 2e69 6f2f 6261 6467 652f 4c69  elds.io/badge/Li
-00004bd0: 6365 6e73 652d 4170 6163 6865 5f32 2e30  cense-Apache_2.0
-00004be0: 2d62 6c75 652e 7376 670a 5b70 6163 6b61  -blue.svg.[packa
-00004bf0: 6765 2d6c 6963 656e 7365 2d75 726c 5d3a  ge-license-url]:
-00004c00: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00004c10: 636f 6d2f 6361 6d65 6c2d 6169 2f63 616d  com/camel-ai/cam
-00004c20: 656c 2f62 6c6f 622f 6d61 7374 6572 2f6c  el/blob/master/l
-00004c30: 6963 656e 7365 732f 4c49 4345 4e53 450a  icenses/LICENSE.
-00004c40: 5b64 6174 612d 6c69 6365 6e73 652d 696d  [data-license-im
-00004c50: 6167 655d 3a20 6874 7470 733a 2f2f 696d  age]: https://im
-00004c60: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00004c70: 6765 2f4c 6963 656e 7365 2d43 435f 4259  ge/License-CC_BY
-00004c80: 2d2d 4e43 5f34 2e30 2d6c 6967 6874 6772  --NC_4.0-lightgr
-00004c90: 6579 2e73 7667 0a5b 6461 7461 2d6c 6963  ey.svg.[data-lic
-00004ca0: 656e 7365 2d75 726c 5d3a 2068 7474 7073  ense-url]: https
-00004cb0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6361  ://github.com/ca
-00004cc0: 6d65 6c2d 6169 2f63 616d 656c 2f62 6c6f  mel-ai/camel/blo
-00004cd0: 622f 6d61 7374 6572 2f6c 6963 656e 7365  b/master/license
-00004ce0: 732f 4441 5441 5f4c 4943 454e 5345 0a0a  s/DATA_LICENSE..
-00004cf0: 5b63 6f6c 6162 2d75 726c 5d3a 2068 7474  [colab-url]: htt
-00004d00: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
-00004d10: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f64  rch.google.com/d
-00004d20: 7269 7665 2f31 417a 5033 334f 3872 6e4d  rive/1AzP33O8rnM
-00004d30: 575f 5f37 6f63 574a 6856 4258 6a4b 7a69  W__7ocWJhVBXjKzi
-00004d40: 4a58 5074 696d 3f75 7370 3d73 6861 7269  JXPtim?usp=shari
-00004d50: 6e67 0a5b 636f 6c61 622d 696d 6167 655d  ng.[colab-image]
-00004d60: 3a20 6874 7470 733a 2f2f 636f 6c61 622e  : https://colab.
-00004d70: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
-00004d80: 636f 6d2f 6173 7365 7473 2f63 6f6c 6162  com/assets/colab
-00004d90: 2d62 6164 6765 2e73 7667 0a5b 6875 6767  -badge.svg.[hugg
-00004da0: 696e 6766 6163 652d 7572 6c5d 3a20 6874  ingface-url]: ht
-00004db0: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
-00004dc0: 652e 636f 2f63 616d 656c 2d61 690a 5b68  e.co/camel-ai.[h
-00004dd0: 7567 6769 6e67 6661 6365 2d69 6d61 6765  uggingface-image
-00004de0: 5d3a 2068 7474 7073 3a2f 2f69 6d67 2e73  ]: https://img.s
-00004df0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-00004e00: 2546 3025 3946 2541 3425 3937 2532 3048  %F0%9F%A4%97%20H
-00004e10: 7567 6769 6e67 2532 3046 6163 652d 4341  ugging%20Face-CA
-00004e20: 4d45 4c2d 2d41 492d 6666 6331 3037 3f63  MEL--AI-ffc107?c
-00004e30: 6f6c 6f72 3d66 6663 3130 3726 6c6f 676f  olor=ffc107&logo
-00004e40: 436f 6c6f 723d 7768 6974 650a 5b73 6c61  Color=white.[sla
-00004e50: 636b 2d75 726c 5d3a 2068 7474 7073 3a2f  ck-url]: https:/
-00004e60: 2f6a 6f69 6e2e 736c 6163 6b2e 636f 6d2f  /join.slack.com/
-00004e70: 742f 6361 6d65 6c2d 6169 2f73 6861 7265  t/camel-ai/share
-00004e80: 645f 696e 7669 7465 2f7a 742d 3267 3778  d_invite/zt-2g7x
-00004e90: 6334 3167 792d 5f37 7263 724e 4e41 4172  c41gy-_7rcrNNAAr
-00004ea0: 4950 3673 4c51 716c 646b 7151 0a5b 736c  IP6sLQqldkqQ.[sl
-00004eb0: 6163 6b2d 696d 6167 655d 3a20 6874 7470  ack-image]: http
-00004ec0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00004ed0: 696f 2f62 6164 6765 2f53 6c61 636b 2d43  io/badge/Slack-C
-00004ee0: 414d 454c 2d2d 4149 2d62 6c75 6576 696f  AMEL--AI-bluevio
-00004ef0: 6c65 743f 6c6f 676f 3d73 6c61 636b 0a5b  let?logo=slack.[
-00004f00: 6469 7363 6f72 642d 7572 6c5d 3a20 6874  discord-url]: ht
-00004f10: 7470 733a 2f2f 6469 7363 6f72 642e 6767  tps://discord.gg
-00004f20: 2f43 4e63 4e70 7175 7944 630a 5b64 6973  /CNcNpquyDc.[dis
-00004f30: 636f 7264 2d69 6d61 6765 5d3a 2068 7474  cord-image]: htt
-00004f40: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00004f50: 2e69 6f2f 6261 6467 652f 4469 7363 6f72  .io/badge/Discor
-00004f60: 642d 4341 4d45 4c2d 2d41 492d 3732 3839  d-CAMEL--AI-7289
-00004f70: 6461 3f6c 6f67 6f3d 6469 7363 6f72 6426  da?logo=discord&
-00004f80: 6c6f 676f 436f 6c6f 723d 7768 6974 6526  logoColor=white&
-00004f90: 636f 6c6f 723d 3732 3839 6461 0a5b 7765  color=7289da.[we
-00004fa0: 6368 6174 2d75 726c 5d3a 2068 7474 7073  chat-url]: https
-00004fb0: 3a2f 2f67 686c 692e 6f72 672f 6361 6d65  ://ghli.org/came
-00004fc0: 6c2f 7765 6368 6174 2e70 6e67 0a5b 7765  l/wechat.png.[we
-00004fd0: 6368 6174 2d69 6d61 6765 5d3a 2068 7474  chat-image]: htt
-00004fe0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00004ff0: 2e69 6f2f 6261 6467 652f 5765 4368 6174  .io/badge/WeChat
-00005000: 2d43 616d 656c 4149 4f72 672d 6272 6967  -CamelAIOrg-brig
-00005010: 6874 6772 6565 6e3f 6c6f 676f 3d77 6563  htgreen?logo=wec
-00005020: 6861 7426 6c6f 676f 436f 6c6f 723d 7768  hat&logoColor=wh
-00005030: 6974 650a 5b74 7769 7474 6572 2d75 726c  ite.[twitter-url
-00005040: 5d3a 2068 7474 7073 3a2f 2f74 7769 7474  ]: https://twitt
-00005050: 6572 2e63 6f6d 2f43 616d 656c 4149 4f72  er.com/CamelAIOr
-00005060: 670a 5b74 7769 7474 6572 2d69 6d61 6765  g.[twitter-image
-00005070: 5d3a 2068 7474 7073 3a2f 2f69 6d67 2e73  ]: https://img.s
-00005080: 6869 656c 6473 2e69 6f2f 7477 6974 7465  hields.io/twitte
-00005090: 722f 666f 6c6c 6f77 2f43 616d 656c 4149  r/follow/CamelAI
-000050a0: 4f72 673f 7374 796c 653d 736f 6369 616c  Org?style=social
-000050b0: 2663 6f6c 6f72 3d62 7269 6768 7467 7265  &color=brightgre
-000050c0: 656e 266c 6f67 6f3d 7477 6974 7465 720a  en&logo=twitter.
-000050d0: 0a                                       .
+00003d70: 2020 2020 2020 2020 2020 207c 2078 2020             | x  
+00003d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003de0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00003df0: 7820 2020 2020 2020 2020 2020 2020 2020  x               
+00003e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e40: 2020 2020 2020 2020 2020 207c 0a0a 2323             |..##
+00003e50: 2056 6973 7561 6c69 7a61 7469 6f6e 7320   Visualizations 
+00003e60: 6f66 2049 6e73 7472 7563 7469 6f6e 7320  of Instructions 
+00003e70: 616e 6420 5461 736b 730a 0a7c 2044 6174  and Tasks..| Dat
+00003e80: 6173 6574 2020 2020 2020 2020 2020 7c20  aset          | 
+00003e90: 496e 7374 7275 6374 696f 6e73 2020 2020  Instructions    
+00003ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f00: 2020 2020 207c 2054 6173 6b73 2020 2020       | Tasks    
+00003f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f70: 2020 2020 207c 0a7c 2d2d 2d2d 2d2d 2d2d       |.|--------
+00003f80: 2d2d 2d2d 2d2d 2d2d 2d2d 7c2d 2d2d 2d2d  ----------|-----
+00003f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003fa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003fb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003fc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003fd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003fe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003ff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004000: 2d7c 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -|--------------
+00004010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004060: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004070: 2d7c 0a7c 202a 2a41 4920 536f 6369 6574  -|.| **AI Societ
+00004080: 792a 2a20 2020 7c20 5b49 6e73 7472 7563  y**   | [Instruc
+00004090: 7469 6f6e 735d 2868 7474 7073 3a2f 2f61  tions](https://a
+000040a0: 746c 6173 2e6e 6f6d 6963 2e61 692f 6d61  tlas.nomic.ai/ma
+000040b0: 702f 3361 3535 3961 3036 2d38 3764 302d  p/3a559a06-87d0-
+000040c0: 3434 3736 2d61 3837 392d 3936 3236 3536  4476-a879-962656
+000040d0: 3234 3234 3532 2f64 6239 3631 3931 352d  242452/db961915-
+000040e0: 6232 3534 2d34 3865 382d 3865 3563 2d39  b254-48e8-8e5c-9
+000040f0: 3137 6638 3237 6237 3463 3629 207c 205b  17f827b74c6) | [
+00004100: 5461 736b 735d 2868 7474 7073 3a2f 2f61  Tasks](https://a
+00004110: 746c 6173 2e6e 6f6d 6963 2e61 692f 6d61  tlas.nomic.ai/ma
+00004120: 702f 6362 3936 6634 3162 2d61 3666 642d  p/cb96f41b-a6fd-
+00004130: 3466 6534 2d61 6334 302d 3038 6531 3031  4fe4-ac40-08e101
+00004140: 3731 3434 3833 2f61 6530 3631 3536 632d  714483/ae06156c-
+00004150: 6135 3732 2d34 3665 392d 3833 3435 2d65  a572-46e9-8345-e
+00004160: 6265 3138 3538 3664 3032 6229 207c 0a7c  be18586d02b) |.|
+00004170: 202a 2a43 6f64 652a 2a20 2020 2020 2020   **Code**       
+00004180: 2020 7c20 5b49 6e73 7472 7563 7469 6f6e    | [Instruction
+00004190: 735d 2868 7474 7073 3a2f 2f61 746c 6173  s](https://atlas
+000041a0: 2e6e 6f6d 6963 2e61 692f 6d61 702f 3930  .nomic.ai/map/90
+000041b0: 3264 3663 6362 2d30 6262 622d 3432 3934  2d6ccb-0bbb-4294
+000041c0: 2d38 3361 382d 3163 3764 3264 6165 3033  -83a8-1c7d2dae03
+000041d0: 6338 2f61 6365 3265 3134 362d 6534 3966  c8/ace2e146-e49f
+000041e0: 2d34 3164 622d 6131 6634 2d32 3561 3263  -41db-a1f4-25a2c
+000041f0: 3462 6532 3435 3729 207c 205b 5461 736b  4be2457) | [Task
+00004200: 735d 2868 7474 7073 3a2f 2f61 746c 6173  s](https://atlas
+00004210: 2e6e 6f6d 6963 2e61 692f 6d61 702f 6566  .nomic.ai/map/ef
+00004220: 6333 3836 3137 2d39 3138 302d 3439 3061  c38617-9180-490a
+00004230: 2d38 3633 302d 3433 6130 3562 3335 6432  -8630-43a05b35d2
+00004240: 3264 2f32 3537 3661 6464 662d 6131 3333  2d/2576addf-a133
+00004250: 2d34 3564 352d 3839 6139 2d36 6230 3637  -45d5-89a9-6b067
+00004260: 6236 3635 3264 6429 207c 0a7c 202a 2a4d  b6652dd) |.| **M
+00004270: 6973 616c 6967 6e6d 656e 742a 2a20 7c20  isalignment** | 
+00004280: 5b49 6e73 7472 7563 7469 6f6e 735d 2868  [Instructions](h
+00004290: 7474 7073 3a2f 2f61 746c 6173 2e6e 6f6d  ttps://atlas.nom
+000042a0: 6963 2e61 692f 6d61 702f 3563 3439 3130  ic.ai/map/5c4910
+000042b0: 3335 2d61 3236 652d 3461 3035 2d39 3539  35-a26e-4a05-959
+000042c0: 332d 3832 6666 6232 6333 6162 3430 2f32  3-82ffb2c3ab40/2
+000042d0: 6264 3938 3839 362d 3839 3465 2d34 3830  bd98896-894e-480
+000042e0: 372d 3965 6438 2d61 3230 3363 6362 3134  7-9ed8-a203ccb14
+000042f0: 6435 6529 207c 205b 5461 736b 735d 2868  d5e) | [Tasks](h
+00004300: 7474 7073 3a2f 2f61 746c 6173 2e6e 6f6d  ttps://atlas.nom
+00004310: 6963 2e61 692f 6d61 702f 6162 6333 3537  ic.ai/map/abc357
+00004320: 6464 2d39 6330 342d 3439 3133 2d39 3534  dd-9c04-4913-954
+00004330: 312d 3633 6532 3539 6437 6163 3166 2f38  1-63e259d7ac1f/8
+00004340: 3235 3133 3961 342d 6166 3636 2d34 3237  25139a4-af66-427
+00004350: 632d 3964 3065 2d66 3336 6235 3439 3261  c-9d0e-f36b5492a
+00004360: 6233 6629 207c 0a0a 2323 2049 6d70 6c65  b3f) |..## Imple
+00004370: 6d65 6e74 6564 2052 6573 6561 7263 6820  mented Research 
+00004380: 4964 6561 7320 6672 6f6d 204f 7468 6572  Ideas from Other
+00004390: 2057 6f72 6b73 0a57 6520 696d 706c 656d   Works.We implem
+000043a0: 656e 7465 6420 616d 617a 696e 6720 7265  ented amazing re
+000043b0: 7365 6172 6368 2069 6465 6173 2066 726f  search ideas fro
+000043c0: 6d20 6f74 6865 7220 776f 726b 7320 666f  m other works fo
+000043d0: 7220 796f 7520 746f 2062 7569 6c64 2c20  r you to build, 
+000043e0: 636f 6d70 6172 6520 616e 6420 6375 7374  compare and cust
+000043f0: 6f6d 697a 6520 796f 7572 2061 6765 6e74  omize your agent
+00004400: 732e 2049 6620 796f 7520 7573 6520 616e  s. If you use an
+00004410: 7920 6f66 2074 6865 7365 206d 6f64 756c  y of these modul
+00004420: 6573 2c20 706c 6561 7365 206b 696e 646c  es, please kindl
+00004430: 7920 6369 7465 2074 6865 206f 7269 6769  y cite the origi
+00004440: 6e61 6c20 776f 726b 733a 0a2d 2060 5461  nal works:.- `Ta
+00004450: 736b 4372 6561 7469 6f6e 4167 656e 7460  skCreationAgent`
+00004460: 2c20 6054 6173 6b50 7269 6f72 6974 697a  , `TaskPrioritiz
+00004470: 6174 696f 6e41 6765 6e74 6020 616e 6420  ationAgent` and 
+00004480: 6042 6162 7941 4749 6020 6672 6f6d 202a  `BabyAGI` from *
+00004490: 4e61 6b61 6a69 6d61 2065 7420 616c 2e2a  Nakajima et al.*
+000044a0: 3a20 5b54 6173 6b2d 4472 6976 656e 2041  : [Task-Driven A
+000044b0: 7574 6f6e 6f6d 6f75 7320 4167 656e 745d  utonomous Agent]
+000044c0: 2868 7474 7073 3a2f 2f79 6f68 6569 6e61  (https://yoheina
+000044d0: 6b61 6a69 6d61 2e63 6f6d 2f74 6173 6b2d  kajima.com/task-
+000044e0: 6472 6976 656e 2d61 7574 6f6e 6f6d 6f75  driven-autonomou
+000044f0: 732d 6167 656e 742d 7574 696c 697a 696e  s-agent-utilizin
+00004500: 672d 6770 742d 342d 7069 6e65 636f 6e65  g-gpt-4-pinecone
+00004510: 2d61 6e64 2d6c 616e 6763 6861 696e 2d66  -and-langchain-f
+00004520: 6f72 2d64 6976 6572 7365 2d61 7070 6c69  or-diverse-appli
+00004530: 6361 7469 6f6e 732f 292e 205b 5b45 7861  cations/). [[Exa
+00004540: 6d70 6c65 5d28 6874 7470 733a 2f2f 6769  mple](https://gi
+00004550: 7468 7562 2e63 6f6d 2f63 616d 656c 2d61  thub.com/camel-a
+00004560: 692f 6361 6d65 6c2f 626c 6f62 2f6d 6173  i/camel/blob/mas
+00004570: 7465 722f 6578 616d 706c 6573 2f61 695f  ter/examples/ai_
+00004580: 736f 6369 6574 792f 6261 6279 6167 695f  society/babyagi_
+00004590: 706c 6179 696e 672e 7079 295d 0a0a 2323  playing.py)]..##
+000045a0: 204e 6577 730a 2d20 5265 6c65 6173 6564   News.- Released
+000045b0: 2041 4920 536f 6369 6574 7920 616e 6420   AI Society and 
+000045c0: 436f 6465 2064 6174 6173 6574 2028 4170  Code dataset (Ap
+000045d0: 7269 6c20 322c 2032 3032 3329 0a2d 2049  ril 2, 2023).- I
+000045e0: 6e69 7469 616c 2072 656c 6561 7365 206f  nitial release o
+000045f0: 6620 6043 414d 454c 6020 7079 7468 6f6e  f `CAMEL` python
+00004600: 206c 6962 7261 7279 2028 4d61 7263 6820   library (March 
+00004610: 3231 2c20 3230 3233 290a 0a23 2320 4369  21, 2023)..## Ci
+00004620: 7461 7469 6f6e 0a60 6060 0a40 696e 7072  tation.```.@inpr
+00004630: 6f63 6565 6469 6e67 737b 6c69 3230 3233  oceedings{li2023
+00004640: 6361 6d65 6c2c 0a20 2074 6974 6c65 3d7b  camel,.  title={
+00004650: 4341 4d45 4c3a 2043 6f6d 6d75 6e69 6361  CAMEL: Communica
+00004660: 7469 7665 2041 6765 6e74 7320 666f 7220  tive Agents for 
+00004670: 224d 696e 6422 2045 7870 6c6f 7261 7469  "Mind" Explorati
+00004680: 6f6e 206f 6620 4c61 7267 6520 4c61 6e67  on of Large Lang
+00004690: 7561 6765 204d 6f64 656c 2053 6f63 6965  uage Model Socie
+000046a0: 7479 7d2c 0a20 2061 7574 686f 723d 7b4c  ty},.  author={L
+000046b0: 692c 2047 756f 6861 6f20 616e 6420 4861  i, Guohao and Ha
+000046c0: 6d6d 6f75 642c 2048 6173 616e 2041 6265  mmoud, Hasan Abe
+000046d0: 6420 416c 204b 6164 6572 2061 6e64 2049  d Al Kader and I
+000046e0: 7461 6e69 2c20 4861 6e69 2061 6e64 204b  tani, Hani and K
+000046f0: 6869 7a62 756c 6c69 6e2c 2044 6d69 7472  hizbullin, Dmitr
+00004700: 6969 2061 6e64 2047 6861 6e65 6d2c 2042  ii and Ghanem, B
+00004710: 6572 6e61 7264 7d2c 0a20 2062 6f6f 6b74  ernard},.  bookt
+00004720: 6974 6c65 3d7b 5468 6972 7479 2d73 6576  itle={Thirty-sev
+00004730: 656e 7468 2043 6f6e 6665 7265 6e63 6520  enth Conference 
+00004740: 6f6e 204e 6575 7261 6c20 496e 666f 726d  on Neural Inform
+00004750: 6174 696f 6e20 5072 6f63 6573 7369 6e67  ation Processing
+00004760: 2053 7973 7465 6d73 7d2c 0a20 2079 6561   Systems},.  yea
+00004770: 723d 7b32 3032 337d 0a7d 0a60 6060 0a23  r={2023}.}.```.#
+00004780: 2320 4163 6b6e 6f77 6c65 6467 656d 656e  # Acknowledgemen
+00004790: 740a 5370 6563 6961 6c20 7468 616e 6b73  t.Special thanks
+000047a0: 2074 6f20 5b4e 6f6d 6963 2041 495d 2868   to [Nomic AI](h
+000047b0: 7474 7073 3a2f 2f68 6f6d 652e 6e6f 6d69  ttps://home.nomi
+000047c0: 632e 6169 2f29 2066 6f72 2067 6976 696e  c.ai/) for givin
+000047d0: 6720 7573 2065 7874 656e 6465 6420 6163  g us extended ac
+000047e0: 6365 7373 2074 6f20 7468 6569 7220 6461  cess to their da
+000047f0: 7461 2073 6574 2065 7870 6c6f 7261 7469  ta set explorati
+00004800: 6f6e 2074 6f6f 6c20 2841 746c 6173 292e  on tool (Atlas).
+00004810: 0a0a 5765 2077 6f75 6c64 2061 6c73 6f20  ..We would also 
+00004820: 6c69 6b65 2074 6f20 7468 616e 6b20 4861  like to thank Ha
+00004830: 7961 2048 616d 6d6f 7564 2066 6f72 2064  ya Hammoud for d
+00004840: 6573 6967 6e69 6e67 2074 6865 2069 6e69  esigning the ini
+00004850: 7469 616c 206c 6f67 6f20 6f66 206f 7572  tial logo of our
+00004860: 2070 726f 6a65 6374 2e0a 0a23 2320 4c69   project...## Li
+00004870: 6365 6e73 650a 0a54 6865 2073 6f75 7263  cense..The sourc
+00004880: 6520 636f 6465 2069 7320 6c69 6365 6e73  e code is licens
+00004890: 6564 2075 6e64 6572 2041 7061 6368 6520  ed under Apache 
+000048a0: 322e 302e 0a0a 5468 6520 6461 7461 7365  2.0...The datase
+000048b0: 7473 2061 7265 206c 6963 656e 7365 6420  ts are licensed 
+000048c0: 756e 6465 7220 4343 2042 5920 4e43 2034  under CC BY NC 4
+000048d0: 2e30 2c20 7768 6963 6820 7065 726d 6974  .0, which permit
+000048e0: 7320 6f6e 6c79 206e 6f6e 2d63 6f6d 6d65  s only non-comme
+000048f0: 7263 6961 6c20 7573 6167 652e 2049 7420  rcial usage. It 
+00004900: 6973 2061 6476 6973 6564 2074 6861 7420  is advised that 
+00004910: 616e 7920 6d6f 6465 6c73 2074 7261 696e  any models train
+00004920: 6564 2075 7369 6e67 2074 6865 2064 6174  ed using the dat
+00004930: 6173 6574 2073 686f 756c 6420 6e6f 7420  aset should not 
+00004940: 6265 2075 7469 6c69 7a65 6420 666f 7220  be utilized for 
+00004950: 616e 7974 6869 6e67 206f 7468 6572 2074  anything other t
+00004960: 6861 6e20 7265 7365 6172 6368 2070 7572  han research pur
+00004970: 706f 7365 732e 0a0a 2323 2043 6f6e 7472  poses...## Contr
+00004980: 6962 7574 696e 6720 746f 2043 414d 454c  ibuting to CAMEL
+00004990: 20f0 9f90 ab0a 5765 2061 7070 7265 6369   .....We appreci
+000049a0: 6174 6520 796f 7572 2069 6e74 6572 6573  ate your interes
+000049b0: 7420 696e 2063 6f6e 7472 6962 7574 696e  t in contributin
+000049c0: 6720 746f 206f 7572 206f 7065 6e2d 736f  g to our open-so
+000049d0: 7572 6365 2069 6e69 7469 6174 6976 652e  urce initiative.
+000049e0: 2057 6520 7072 6f76 6964 6520 6120 646f   We provide a do
+000049f0: 6375 6d65 6e74 206f 6620 5b63 6f6e 7472  cument of [contr
+00004a00: 6962 7574 696e 6720 6775 6964 656c 696e  ibuting guidelin
+00004a10: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
+00004a20: 7562 2e63 6f6d 2f63 616d 656c 2d61 692f  ub.com/camel-ai/
+00004a30: 6361 6d65 6c2f 626c 6f62 2f6d 6173 7465  camel/blob/maste
+00004a40: 722f 434f 4e54 5249 4255 5449 4e47 2e6d  r/CONTRIBUTING.m
+00004a50: 6429 2077 6869 6368 206f 7574 6c69 6e65  d) which outline
+00004a60: 7320 7468 6520 7374 6570 7320 666f 7220  s the steps for 
+00004a70: 636f 6e74 7269 6275 7469 6e67 2074 6f20  contributing to 
+00004a80: 4341 4d45 4c2e 2050 6c65 6173 6520 7265  CAMEL. Please re
+00004a90: 6665 7220 746f 2074 6869 7320 6775 6964  fer to this guid
+00004aa0: 6520 746f 2065 6e73 7572 6520 736d 6f6f  e to ensure smoo
+00004ab0: 7468 2063 6f6c 6c61 626f 7261 7469 6f6e  th collaboration
+00004ac0: 2061 6e64 2073 7563 6365 7373 6675 6c20   and successful 
+00004ad0: 636f 6e74 7269 6275 7469 6f6e 732e 20f0  contributions. .
+00004ae0: 9fa4 9df0 9f9a 800a 0a23 2320 436f 6e74  .........## Cont
+00004af0: 6163 740a 466f 7220 6d6f 7265 2069 6e66  act.For more inf
+00004b00: 6f72 6d61 7469 6f6e 2070 6c65 6173 6520  ormation please 
+00004b10: 636f 6e74 6163 7420 6361 6d65 6c2e 6169  contact camel.ai
+00004b20: 2e74 6561 6d40 676d 6169 6c2e 636f 6d2e  .team@gmail.com.
+00004b30: 0a0a 5b70 7974 686f 6e2d 696d 6167 655d  ..[python-image]
+00004b40: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
+00004b50: 6965 6c64 732e 696f 2f62 6164 6765 2f50  ields.io/badge/P
+00004b60: 7974 686f 6e2d 332e 3925 3242 2d62 7269  ython-3.9%2B-bri
+00004b70: 6768 7467 7265 656e 2e73 7667 0a5b 7079  ghtgreen.svg.[py
+00004b80: 7468 6f6e 2d75 726c 5d3a 2068 7474 7073  thon-url]: https
+00004b90: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
+00004ba0: 7267 2f33 2e39 2f0a 5b70 7974 6573 742d  rg/3.9/.[pytest-
+00004bb0: 696d 6167 655d 3a20 6874 7470 733a 2f2f  image]: https://
+00004bc0: 6769 7468 7562 2e63 6f6d 2f63 616d 656c  github.com/camel
+00004bd0: 2d61 692f 6361 6d65 6c2f 6163 7469 6f6e  -ai/camel/action
+00004be0: 732f 776f 726b 666c 6f77 732f 7079 7465  s/workflows/pyte
+00004bf0: 7374 5f70 6163 6b61 6765 2e79 6d6c 2f62  st_package.yml/b
+00004c00: 6164 6765 2e73 7667 0a5b 7079 7465 7374  adge.svg.[pytest
+00004c10: 2d75 726c 5d3a 2068 7474 7073 3a2f 2f67  -url]: https://g
+00004c20: 6974 6875 622e 636f 6d2f 6361 6d65 6c2d  ithub.com/camel-
+00004c30: 6169 2f63 616d 656c 2f61 6374 696f 6e73  ai/camel/actions
+00004c40: 2f77 6f72 6b66 6c6f 7773 2f70 7974 6573  /workflows/pytes
+00004c50: 745f 7061 636b 6167 652e 796d 6c0a 5b64  t_package.yml.[d
+00004c60: 6f63 732d 696d 6167 655d 3a20 6874 7470  ocs-image]: http
+00004c70: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00004c80: 696f 2f62 6164 6765 2f44 6f63 756d 656e  io/badge/Documen
+00004c90: 7461 7469 6f6e 2d67 7265 792e 7376 673f  tation-grey.svg?
+00004ca0: 6c6f 676f 3d67 6974 6875 620a 5b64 6f63  logo=github.[doc
+00004cb0: 732d 7572 6c5d 3a20 6874 7470 733a 2f2f  s-url]: https://
+00004cc0: 6361 6d65 6c2d 6169 2e67 6974 6875 622e  camel-ai.github.
+00004cd0: 696f 2f63 616d 656c 2f69 6e64 6578 2e68  io/camel/index.h
+00004ce0: 746d 6c0a 5b73 7461 722d 696d 6167 655d  tml.[star-image]
+00004cf0: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
+00004d00: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
+00004d10: 7374 6172 732f 6361 6d65 6c2d 6169 2f63  stars/camel-ai/c
+00004d20: 616d 656c 3f6c 6162 656c 3d73 7461 7273  amel?label=stars
+00004d30: 266c 6f67 6f3d 6769 7468 7562 2663 6f6c  &logo=github&col
+00004d40: 6f72 3d62 7269 6768 7467 7265 656e 0a5b  or=brightgreen.[
+00004d50: 7374 6172 2d75 726c 5d3a 2068 7474 7073  star-url]: https
+00004d60: 3a2f 2f67 6974 6875 622e 636f 6d2f 6361  ://github.com/ca
+00004d70: 6d65 6c2d 6169 2f63 616d 656c 2f73 7461  mel-ai/camel/sta
+00004d80: 7267 617a 6572 730a 5b70 6163 6b61 6765  rgazers.[package
+00004d90: 2d6c 6963 656e 7365 2d69 6d61 6765 5d3a  -license-image]:
+00004da0: 2068 7474 7073 3a2f 2f69 6d67 2e73 6869   https://img.shi
+00004db0: 656c 6473 2e69 6f2f 6261 6467 652f 4c69  elds.io/badge/Li
+00004dc0: 6365 6e73 652d 4170 6163 6865 5f32 2e30  cense-Apache_2.0
+00004dd0: 2d62 6c75 652e 7376 670a 5b70 6163 6b61  -blue.svg.[packa
+00004de0: 6765 2d6c 6963 656e 7365 2d75 726c 5d3a  ge-license-url]:
+00004df0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00004e00: 636f 6d2f 6361 6d65 6c2d 6169 2f63 616d  com/camel-ai/cam
+00004e10: 656c 2f62 6c6f 622f 6d61 7374 6572 2f6c  el/blob/master/l
+00004e20: 6963 656e 7365 732f 4c49 4345 4e53 450a  icenses/LICENSE.
+00004e30: 5b64 6174 612d 6c69 6365 6e73 652d 696d  [data-license-im
+00004e40: 6167 655d 3a20 6874 7470 733a 2f2f 696d  age]: https://im
+00004e50: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00004e60: 6765 2f4c 6963 656e 7365 2d43 435f 4259  ge/License-CC_BY
+00004e70: 2d2d 4e43 5f34 2e30 2d6c 6967 6874 6772  --NC_4.0-lightgr
+00004e80: 6579 2e73 7667 0a5b 6461 7461 2d6c 6963  ey.svg.[data-lic
+00004e90: 656e 7365 2d75 726c 5d3a 2068 7474 7073  ense-url]: https
+00004ea0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6361  ://github.com/ca
+00004eb0: 6d65 6c2d 6169 2f63 616d 656c 2f62 6c6f  mel-ai/camel/blo
+00004ec0: 622f 6d61 7374 6572 2f6c 6963 656e 7365  b/master/license
+00004ed0: 732f 4441 5441 5f4c 4943 454e 5345 0a0a  s/DATA_LICENSE..
+00004ee0: 5b63 6f6c 6162 2d75 726c 5d3a 2068 7474  [colab-url]: htt
+00004ef0: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
+00004f00: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f64  rch.google.com/d
+00004f10: 7269 7665 2f31 417a 5033 334f 3872 6e4d  rive/1AzP33O8rnM
+00004f20: 575f 5f37 6f63 574a 6856 4258 6a4b 7a69  W__7ocWJhVBXjKzi
+00004f30: 4a58 5074 696d 3f75 7370 3d73 6861 7269  JXPtim?usp=shari
+00004f40: 6e67 0a5b 636f 6c61 622d 696d 6167 655d  ng.[colab-image]
+00004f50: 3a20 6874 7470 733a 2f2f 636f 6c61 622e  : https://colab.
+00004f60: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
+00004f70: 636f 6d2f 6173 7365 7473 2f63 6f6c 6162  com/assets/colab
+00004f80: 2d62 6164 6765 2e73 7667 0a5b 6875 6767  -badge.svg.[hugg
+00004f90: 696e 6766 6163 652d 7572 6c5d 3a20 6874  ingface-url]: ht
+00004fa0: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
+00004fb0: 652e 636f 2f63 616d 656c 2d61 690a 5b68  e.co/camel-ai.[h
+00004fc0: 7567 6769 6e67 6661 6365 2d69 6d61 6765  uggingface-image
+00004fd0: 5d3a 2068 7474 7073 3a2f 2f69 6d67 2e73  ]: https://img.s
+00004fe0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00004ff0: 2546 3025 3946 2541 3425 3937 2532 3048  %F0%9F%A4%97%20H
+00005000: 7567 6769 6e67 2532 3046 6163 652d 4341  ugging%20Face-CA
+00005010: 4d45 4c2d 2d41 492d 6666 6331 3037 3f63  MEL--AI-ffc107?c
+00005020: 6f6c 6f72 3d66 6663 3130 3726 6c6f 676f  olor=ffc107&logo
+00005030: 436f 6c6f 723d 7768 6974 650a 5b73 6c61  Color=white.[sla
+00005040: 636b 2d75 726c 5d3a 2068 7474 7073 3a2f  ck-url]: https:/
+00005050: 2f6a 6f69 6e2e 736c 6163 6b2e 636f 6d2f  /join.slack.com/
+00005060: 742f 6361 6d65 6c2d 6169 2f73 6861 7265  t/camel-ai/share
+00005070: 645f 696e 7669 7465 2f7a 742d 3267 3778  d_invite/zt-2g7x
+00005080: 6334 3167 792d 5f37 7263 724e 4e41 4172  c41gy-_7rcrNNAAr
+00005090: 4950 3673 4c51 716c 646b 7151 0a5b 736c  IP6sLQqldkqQ.[sl
+000050a0: 6163 6b2d 696d 6167 655d 3a20 6874 7470  ack-image]: http
+000050b0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000050c0: 696f 2f62 6164 6765 2f53 6c61 636b 2d43  io/badge/Slack-C
+000050d0: 414d 454c 2d2d 4149 2d62 6c75 6576 696f  AMEL--AI-bluevio
+000050e0: 6c65 743f 6c6f 676f 3d73 6c61 636b 0a5b  let?logo=slack.[
+000050f0: 6469 7363 6f72 642d 7572 6c5d 3a20 6874  discord-url]: ht
+00005100: 7470 733a 2f2f 6469 7363 6f72 642e 6767  tps://discord.gg
+00005110: 2f43 4e63 4e70 7175 7944 630a 5b64 6973  /CNcNpquyDc.[dis
+00005120: 636f 7264 2d69 6d61 6765 5d3a 2068 7474  cord-image]: htt
+00005130: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00005140: 2e69 6f2f 6261 6467 652f 4469 7363 6f72  .io/badge/Discor
+00005150: 642d 4341 4d45 4c2d 2d41 492d 3732 3839  d-CAMEL--AI-7289
+00005160: 6461 3f6c 6f67 6f3d 6469 7363 6f72 6426  da?logo=discord&
+00005170: 6c6f 676f 436f 6c6f 723d 7768 6974 6526  logoColor=white&
+00005180: 636f 6c6f 723d 3732 3839 6461 0a5b 7765  color=7289da.[we
+00005190: 6368 6174 2d75 726c 5d3a 2068 7474 7073  chat-url]: https
+000051a0: 3a2f 2f67 686c 692e 6f72 672f 6361 6d65  ://ghli.org/came
+000051b0: 6c2f 7765 6368 6174 2e70 6e67 0a5b 7765  l/wechat.png.[we
+000051c0: 6368 6174 2d69 6d61 6765 5d3a 2068 7474  chat-image]: htt
+000051d0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000051e0: 2e69 6f2f 6261 6467 652f 5765 4368 6174  .io/badge/WeChat
+000051f0: 2d43 616d 656c 4149 4f72 672d 6272 6967  -CamelAIOrg-brig
+00005200: 6874 6772 6565 6e3f 6c6f 676f 3d77 6563  htgreen?logo=wec
+00005210: 6861 7426 6c6f 676f 436f 6c6f 723d 7768  hat&logoColor=wh
+00005220: 6974 650a 5b74 7769 7474 6572 2d75 726c  ite.[twitter-url
+00005230: 5d3a 2068 7474 7073 3a2f 2f74 7769 7474  ]: https://twitt
+00005240: 6572 2e63 6f6d 2f43 616d 656c 4149 4f72  er.com/CamelAIOr
+00005250: 670a 5b74 7769 7474 6572 2d69 6d61 6765  g.[twitter-image
+00005260: 5d3a 2068 7474 7073 3a2f 2f69 6d67 2e73  ]: https://img.s
+00005270: 6869 656c 6473 2e69 6f2f 7477 6974 7465  hields.io/twitte
+00005280: 722f 666f 6c6c 6f77 2f43 616d 656c 4149  r/follow/CamelAI
+00005290: 4f72 673f 7374 796c 653d 736f 6369 616c  Org?style=social
+000052a0: 2663 6f6c 6f72 3d62 7269 6768 7467 7265  &color=brightgre
+000052b0: 656e 266c 6f67 6f3d 7477 6974 7465 720a  en&logo=twitter.
+000052c0: 0a                                       .
```

