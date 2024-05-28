# Comparing `tmp/eidolon_ai_sdk-0.1.56.tar.gz` & `tmp/eidolon_ai_sdk-0.1.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eidolon_ai_sdk-0.1.56.tar", max compression
+gzip compressed data, was "eidolon_ai_sdk-0.1.57.tar", max compression
```

## Comparing `eidolon_ai_sdk-0.1.56.tar` & `eidolon_ai_sdk-0.1.57.tar`

### file list

```diff
@@ -1,144 +1,145 @@
--rw-r--r--   0        0        0      701 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/README.md
--rw-r--r--   0        0        0        0 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/__init__.py
--rw-r--r--   0        0        0     2424 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/agent.py
--rw-r--r--   0        0        0     1311 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/audio_agent.py
--rw-r--r--   0        0        0        0 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/__init__.py
--rw-r--r--   0        0        0     3549 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/document_manager.py
--rw-r--r--   0        0        0     2865 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/document_processor.py
--rw-r--r--   0        0        0        0 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
--rw-r--r--   0        0        0      971 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
--rw-r--r--   0        0        0     3405 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
--rw-r--r--   0        0        0     4403 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
--rw-r--r--   0        0        0        0 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
--rw-r--r--   0        0        0     2817 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
--rw-r--r--   0        0        0     4519 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
--rw-r--r--   0        0        0        0 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
--rw-r--r--   0        0        0      448 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
--rw-r--r--   0        0        0     3699 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
--rw-r--r--   0        0        0     2053 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
--rw-r--r--   0        0        0     3212 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
--rw-r--r--   0        0        0     1647 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
--rw-r--r--   0        0        0     1328 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
--rw-r--r--   0        0        0     3356 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
--rw-r--r--   0        0        0     1400 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
--rw-r--r--   0        0        0        0 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
--rw-r--r--   0        0        0     1398 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
--rw-r--r--   0        0        0     4786 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
--rw-r--r--   0        0        0    43465 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
--rw-r--r--   0        0        0     4825 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/generic_agent.py
--rw-r--r--   0        0        0        0 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/retriever_agent/__init__.py
--rw-r--r--   0        0        0     2078 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
--rw-r--r--   0        0        0     1428 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
--rw-r--r--   0        0        0     2323 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
--rw-r--r--   0        0        0      559 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
--rw-r--r--   0        0        0     2864 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/retriever_agent/retriever.py
--rw-r--r--   0        0        0     3717 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
--rw-r--r--   0        0        0    13073 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/simple_agent.py
--rw-r--r--   0        0        0        0 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/tot_agent/__init__.py
--rw-r--r--   0        0        0     1809 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/tot_agent/checker.py
--rw-r--r--   0        0        0     2468 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/tot_agent/controller.py
--rw-r--r--   0        0        0     1503 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/tot_agent/memory.py
--rw-r--r--   0        0        0     1423 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/tot_agent/prompts.py
--rw-r--r--   0        0        0      364 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/tot_agent/thought.py
--rw-r--r--   0        0        0     4951 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
--rw-r--r--   0        0        0     7614 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
--rw-r--r--   0        0        0     4572 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent_os.py
--rw-r--r--   0        0        0    12735 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent_os_interfaces.py
--rw-r--r--   0        0        0        0 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/bin/__init__.py
--rwxr-xr-x   0        0        0     9545 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/bin/agent_creator.py
--rw-r--r--   0        0        0     8381 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/bin/agent_http_server.py
--rwxr-xr-x   0        0        0     3789 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/bin/replay.py
--rw-r--r--   0        0        0        0 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/__init__.py
--rw-r--r--   0        0        0     9073 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/code_builtins.py
--rw-r--r--   0        0        0        0 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/components/__init__.py
--rw-r--r--   0        0        0     2223 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/components/opentelemetry.py
--rw-r--r--   0        0        0     4256 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/components/usage.py
--rw-r--r--   0        0        0        0 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/logic_units/__init__.py
--rw-r--r--   0        0        0     1822 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/logic_units/playwrite_browser.py
--rw-r--r--   0        0        0     6517 2024-05-20 19:28:11.739036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/logic_units/web_search.py
--rw-r--r--   0        0        0      550 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
--rw-r--r--   0        0        0      601 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
--rw-r--r--   0        0        0      614 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
--rw-r--r--   0        0        0      181 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/resources/machine.yaml
--rw-r--r--   0        0        0      597 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
--rw-r--r--   0        0        0      547 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
--rw-r--r--   0        0        0      540 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
--rw-r--r--   0        0        0      595 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/resources/openai_35.yaml
--rw-r--r--   0        0        0      586 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/resources/openai_4.yaml
--rw-r--r--   0        0        0        0 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/__init__.py
--rw-r--r--   0        0        0     1843 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/agent_call_history.py
--rw-r--r--   0        0        0     3008 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/agent_io.py
--rw-r--r--   0        0        0     9128 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/agents_logic_unit.py
--rw-r--r--   0        0        0     5911 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/apu.py
--rw-r--r--   0        0        0     3790 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/audio_unit.py
--rw-r--r--   0        0        0      292 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/call_context.py
--rw-r--r--   0        0        0     2833 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/conversation_memory_unit.py
--rw-r--r--   0        0        0    14365 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/conversational_apu.py
--rw-r--r--   0        0        0     4841 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/image_unit.py
--rw-r--r--   0        0        0        0 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/llm/__init__.py
--rw-r--r--   0        0        0     9936 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
--rw-r--r--   0        0        0    11967 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
--rw-r--r--   0        0        0     4518 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py
--rw-r--r--   0        0        0     5753 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py
--rw-r--r--   0        0        0     9490 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
--rw-r--r--   0        0        0     3597 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
--rw-r--r--   0        0        0     3962 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/llm_message.py
--rw-r--r--   0        0        0     2421 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/llm_unit.py
--rw-r--r--   0        0        0     4491 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/logic_unit.py
--rw-r--r--   0        0        0     3541 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/memory_unit.py
--rw-r--r--   0        0        0      825 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/processing_unit.py
--rw-r--r--   0        0        0        0 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/io/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/__init__.py
--rw-r--r--   0        0        0     1193 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/agent_memory.py
--rw-r--r--   0        0        0     5309 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/chroma_vector_store.py
--rw-r--r--   0        0        0      641 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/document.py
--rw-r--r--   0        0        0     2766 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/embeddings.py
--rw-r--r--   0        0        0      907 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/file_memory.py
--rw-r--r--   0        0        0     4203 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/file_system_vector_store.py
--rw-r--r--   0        0        0     3974 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/in_memory_file_memory.py
--rw-r--r--   0        0        0     5788 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/local_file_memory.py
--rw-r--r--   0        0        0     4845 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/local_symbolic_memory.py
--rw-r--r--   0        0        0     3793 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
--rw-r--r--   0        0        0      996 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/noop_memory.py
--rw-r--r--   0        0        0     1984 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/s3_file_memory.py
--rw-r--r--   0        0        0      974 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/semantic_memory.py
--rw-r--r--   0        0        0     2809 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/similarity_memory.py
--rw-r--r--   0        0        0     1516 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/vector_store.py
--rw-r--r--   0        0        0        0 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/security/__init__.py
--rw-r--r--   0        0        0      771 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/security/authentication_processor.py
--rw-r--r--   0        0        0     2159 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/security/azure_authorizer.py
--rw-r--r--   0        0        0     1277 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/security/functional_authorizer.py
--rw-r--r--   0        0        0     2001 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/security/google_auth.py
--rw-r--r--   0        0        0     1867 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/security/jwt_processor.py
--rw-r--r--   0        0        0      484 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/security/okta_authorizor.py
--rw-r--r--   0        0        0     1017 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/security/permissions.py
--rw-r--r--   0        0        0     2508 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/security/process_authorizer.py
--rw-r--r--   0        0        0     2977 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/security/security_manager.py
--rw-r--r--   0        0        0     1035 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/security/security_middleware.py
--rw-r--r--   0        0        0      428 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/security/user.py
--rw-r--r--   0        0        0        0 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/system/__init__.py
--rw-r--r--   0        0        0     1473 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/system/agent_contract.py
--rw-r--r--   0        0        0    23004 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/system/agent_controller.py
--rw-r--r--   0        0        0    14196 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/system/agent_machine.py
--rw-r--r--   0        0        0     1149 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/system/dynamic_middleware.py
--rw-r--r--   0        0        0     3432 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/system/fn_handler.py
--rw-r--r--   0        0        0     4911 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/system/process_file_system.py
--rw-r--r--   0        0        0     4275 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/system/processes.py
--rw-r--r--   0        0        0     6895 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/system/reference_model.py
--rw-r--r--   0        0        0        0 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/system/resources/__init__.py
--rw-r--r--   0        0        0      314 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/system/resources/agent_resource.py
--rw-r--r--   0        0        0      414 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/system/resources/machine_resource.py
--rw-r--r--   0        0        0      684 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/system/resources/reference_resource.py
--rw-r--r--   0        0        0     1663 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/system/resources/resources_base.py
--rw-r--r--   0        0        0        0 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/util/__init__.py
--rw-r--r--   0        0        0      509 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/util/async_wrapper.py
--rw-r--r--   0        0        0     2806 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/util/class_utils.py
--rw-r--r--   0        0        0     1604 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/util/image_utils.py
--rw-r--r--   0        0        0     3808 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/util/replay.py
--rw-r--r--   0        0        0     6917 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/util/schema_to_model.py
--rw-r--r--   0        0        0      898 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/util/str_utils.py
--rw-r--r--   0        0        0     3445 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/util/stream_collector.py
--rw-r--r--   0        0        0      565 2024-05-20 19:28:11.743036 eidolon_ai_sdk-0.1.56/logging.conf
--rw-r--r--   0        0        0     2214 2024-05-20 19:28:11.747036 eidolon_ai_sdk-0.1.56/pyproject.toml
--rw-r--r--   0        0        0     2977 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.56/PKG-INFO
+-rw-r--r--   0        0        0      701 2024-05-28 17:23:10.577192 eidolon_ai_sdk-0.1.57/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 17:23:10.577192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:23:10.577192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/__init__.py
+-rw-r--r--   0        0        0     2424 2024-05-28 17:23:10.577192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/agent.py
+-rw-r--r--   0        0        0     1311 2024-05-28 17:23:10.577192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/audio_agent.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:23:10.577192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/__init__.py
+-rw-r--r--   0        0        0     3549 2024-05-28 17:23:10.577192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/document_manager.py
+-rw-r--r--   0        0        0     2865 2024-05-28 17:23:10.577192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/document_processor.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:23:10.577192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
+-rw-r--r--   0        0        0      971 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
+-rw-r--r--   0        0        0     3405 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
+-rw-r--r--   0        0        0     4403 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
+-rw-r--r--   0        0        0     2817 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
+-rw-r--r--   0        0        0     4519 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
+-rw-r--r--   0        0        0      448 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
+-rw-r--r--   0        0        0     3699 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
+-rw-r--r--   0        0        0     2053 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
+-rw-r--r--   0        0        0     3212 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
+-rw-r--r--   0        0        0     1647 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
+-rw-r--r--   0        0        0     1328 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
+-rw-r--r--   0        0        0     3356 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
+-rw-r--r--   0        0        0     1400 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
+-rw-r--r--   0        0        0     1398 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
+-rw-r--r--   0        0        0     4786 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
+-rw-r--r--   0        0        0    43465 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
+-rw-r--r--   0        0        0     4825 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/generic_agent.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/retriever_agent/__init__.py
+-rw-r--r--   0        0        0     2078 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
+-rw-r--r--   0        0        0     1428 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
+-rw-r--r--   0        0        0     2323 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
+-rw-r--r--   0        0        0      559 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
+-rw-r--r--   0        0        0     2864 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/retriever_agent/retriever.py
+-rw-r--r--   0        0        0     4142 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
+-rw-r--r--   0        0        0    13376 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/simple_agent.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/tot_agent/__init__.py
+-rw-r--r--   0        0        0     1809 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/tot_agent/checker.py
+-rw-r--r--   0        0        0     2468 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/tot_agent/controller.py
+-rw-r--r--   0        0        0     1503 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/tot_agent/memory.py
+-rw-r--r--   0        0        0     1423 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/tot_agent/prompts.py
+-rw-r--r--   0        0        0      364 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/tot_agent/thought.py
+-rw-r--r--   0        0        0     4951 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
+-rw-r--r--   0        0        0     7614 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
+-rw-r--r--   0        0        0     4572 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent_os.py
+-rw-r--r--   0        0        0    12735 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent_os_interfaces.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/bin/__init__.py
+-rwxr-xr-x   0        0        0     9545 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/bin/agent_creator.py
+-rw-r--r--   0        0        0     8381 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/bin/agent_http_server.py
+-rwxr-xr-x   0        0        0     3789 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/bin/replay.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/__init__.py
+-rw-r--r--   0        0        0     9194 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/code_builtins.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/components/__init__.py
+-rw-r--r--   0        0        0     2223 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/components/opentelemetry.py
+-rw-r--r--   0        0        0     4256 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/components/usage.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/logic_units/__init__.py
+-rw-r--r--   0        0        0     1822 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/logic_units/playwrite_browser.py
+-rw-r--r--   0        0        0     6517 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/logic_units/web_search.py
+-rw-r--r--   0        0        0      550 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
+-rw-r--r--   0        0        0      601 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
+-rw-r--r--   0        0        0      614 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
+-rw-r--r--   0        0        0      181 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/resources/machine.yaml
+-rw-r--r--   0        0        0      597 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
+-rw-r--r--   0        0        0      547 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
+-rw-r--r--   0        0        0      540 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
+-rw-r--r--   0        0        0      595 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/resources/openai_35.yaml
+-rw-r--r--   0        0        0      586 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/resources/openai_4.yaml
+-rw-r--r--   0        0        0        0 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/__init__.py
+-rw-r--r--   0        0        0     1843 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/agent_call_history.py
+-rw-r--r--   0        0        0     3008 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/agent_io.py
+-rw-r--r--   0        0        0     9128 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/agents_logic_unit.py
+-rw-r--r--   0        0        0     6039 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/apu.py
+-rw-r--r--   0        0        0     3790 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/audio_unit.py
+-rw-r--r--   0        0        0      292 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/call_context.py
+-rw-r--r--   0        0        0     2833 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/conversation_memory_unit.py
+-rw-r--r--   0        0        0    14187 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/conversational_apu.py
+-rw-r--r--   0        0        0     4841 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/image_unit.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/llm/__init__.py
+-rw-r--r--   0        0        0     9936 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
+-rw-r--r--   0        0        0    11967 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
+-rw-r--r--   0        0        0     4518 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py
+-rw-r--r--   0        0        0     5753 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py
+-rw-r--r--   0        0        0     9490 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
+-rw-r--r--   0        0        0     3597 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
+-rw-r--r--   0        0        0     3962 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/llm_message.py
+-rw-r--r--   0        0        0     3082 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/llm_unit.py
+-rw-r--r--   0        0        0     4491 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/logic_unit.py
+-rw-r--r--   0        0        0     3541 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/memory_unit.py
+-rw-r--r--   0        0        0      825 2024-05-28 17:23:10.581192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/processing_unit.py
+-rw-r--r--   0        0        0     5205 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/tool_call_unit.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/io/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/__init__.py
+-rw-r--r--   0        0        0     1193 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/agent_memory.py
+-rw-r--r--   0        0        0     5309 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/chroma_vector_store.py
+-rw-r--r--   0        0        0      641 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/document.py
+-rw-r--r--   0        0        0     2766 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/embeddings.py
+-rw-r--r--   0        0        0      907 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/file_memory.py
+-rw-r--r--   0        0        0     4203 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/file_system_vector_store.py
+-rw-r--r--   0        0        0     3974 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/in_memory_file_memory.py
+-rw-r--r--   0        0        0     5788 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/local_file_memory.py
+-rw-r--r--   0        0        0     4845 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/local_symbolic_memory.py
+-rw-r--r--   0        0        0     3793 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
+-rw-r--r--   0        0        0      996 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/noop_memory.py
+-rw-r--r--   0        0        0     1984 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/s3_file_memory.py
+-rw-r--r--   0        0        0      974 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/semantic_memory.py
+-rw-r--r--   0        0        0     2809 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/similarity_memory.py
+-rw-r--r--   0        0        0     1516 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/vector_store.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/security/__init__.py
+-rw-r--r--   0        0        0      771 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/security/authentication_processor.py
+-rw-r--r--   0        0        0     2159 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/security/azure_authorizer.py
+-rw-r--r--   0        0        0     1277 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/security/functional_authorizer.py
+-rw-r--r--   0        0        0     2001 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/security/google_auth.py
+-rw-r--r--   0        0        0     1867 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/security/jwt_processor.py
+-rw-r--r--   0        0        0      484 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/security/okta_authorizor.py
+-rw-r--r--   0        0        0     1017 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/security/permissions.py
+-rw-r--r--   0        0        0     2508 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/security/process_authorizer.py
+-rw-r--r--   0        0        0     2977 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/security/security_manager.py
+-rw-r--r--   0        0        0     1035 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/security/security_middleware.py
+-rw-r--r--   0        0        0      428 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/security/user.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/system/__init__.py
+-rw-r--r--   0        0        0     1473 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/system/agent_contract.py
+-rw-r--r--   0        0        0    23004 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/system/agent_controller.py
+-rw-r--r--   0        0        0    14196 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/system/agent_machine.py
+-rw-r--r--   0        0        0     1149 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/system/dynamic_middleware.py
+-rw-r--r--   0        0        0     3432 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/system/fn_handler.py
+-rw-r--r--   0        0        0     4911 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/system/process_file_system.py
+-rw-r--r--   0        0        0     4275 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/system/processes.py
+-rw-r--r--   0        0        0     7664 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/system/reference_model.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/system/resources/__init__.py
+-rw-r--r--   0        0        0      314 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/system/resources/agent_resource.py
+-rw-r--r--   0        0        0      414 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/system/resources/machine_resource.py
+-rw-r--r--   0        0        0      684 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/system/resources/reference_resource.py
+-rw-r--r--   0        0        0     1663 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/system/resources/resources_base.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/util/__init__.py
+-rw-r--r--   0        0        0      509 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/util/async_wrapper.py
+-rw-r--r--   0        0        0     2806 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/util/class_utils.py
+-rw-r--r--   0        0        0     1604 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/util/image_utils.py
+-rw-r--r--   0        0        0     3808 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/util/replay.py
+-rw-r--r--   0        0        0     6917 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/util/schema_to_model.py
+-rw-r--r--   0        0        0      898 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/util/str_utils.py
+-rw-r--r--   0        0        0     3445 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/util/stream_collector.py
+-rw-r--r--   0        0        0      565 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/logging.conf
+-rw-r--r--   0        0        0     2214 2024-05-28 17:23:10.585192 eidolon_ai_sdk-0.1.57/pyproject.toml
+-rw-r--r--   0        0        0     2977 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.57/PKG-INFO
```

### Comparing `eidolon_ai_sdk-0.1.56/README.md` & `eidolon_ai_sdk-0.1.57/README.md`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/agent.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/audio_agent.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/audio_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/document_manager.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/document_manager.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/document_processor.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/document_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/generic_agent.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/generic_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/retriever_agent/retriever.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/retriever_agent/retriever.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,19 @@
 
 def make_description(agent: object, _handler: FnHandler) -> str:
     # noinspection PyUnresolvedReferences
     return agent.spec.description
 
 
 class RetrieverAgentSpec(RetrieverSpec):
+    """
+    A RetrieverAgent is an agent that will take a query, rewrite it for better similarity vector search, and then perform the vector search on the document store.
+    The agent will dynamically load and embed files, so it is not performant for loading large bodies of files, but performs very well for small to medium-sized document stores (hundreds to thousands of documents) which are updating frequently.
+    """
+
     name: str = Field(description="The name of the document store to use.")
     description: str = Field(
         description="A detailed description of the the retriever including all necessary information for the calling agent to decide to call this agent, i.e. file type or location or etc..."
     )
     # these three fields are required and override the defaults of the subcomponents
     loader_root_location: str = Field(None, description="A URL specifying the root location of the loader.")
```

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/simple_agent.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/simple_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,20 @@
 class NamedCPU(BaseModel):
     title: Optional[str] = None
     apu: AnnotatedReference[APU]
     default: bool = False
 
 
 class SimpleAgentSpec(BaseModel):
+    """
+    The `SimpleAgentSpec` class defines the basic configuration for a SimpleAgent within the Eidolon framework. This
+    agent is designed to be a flexible, modular component that can interact with various processing units and perform a
+    range of actions based on its configuration.
+    """
+
     description: Optional[str] = None
     system_prompt: str = "You are a helpful assistant"
     agent_refs: List[str] = []
     actions: List[ActionDefinition] = [ActionDefinition()]
     apu: AnnotatedReference[APU] = None
     apus: List[NamedCPU] = []
     title_generation_mode: Literal["none", "on_request"] = "on_request"
```

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/tot_agent/checker.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/tot_agent/checker.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/tot_agent/controller.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/tot_agent/controller.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/tot_agent/memory.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/tot_agent/memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/tot_agent/prompts.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/tot_agent/prompts.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/tot_agent/thought_generators.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/tot_agent/thought_generators.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent/tot_agent/tot_agent.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent/tot_agent/tot_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent_os.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent_os.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/agent_os_interfaces.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/agent_os_interfaces.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/bin/agent_creator.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/bin/agent_creator.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/bin/agent_http_server.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/bin/agent_http_server.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/bin/replay.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/bin/replay.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/code_builtins.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/code_builtins.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,51 +5,52 @@
 from openai.lib.azure import AsyncAzureOpenAI
 from opentelemetry.exporter.otlp.proto.grpc.trace_exporter import OTLPSpanExporter
 from opentelemetry.sdk.trace import SpanProcessor
 from opentelemetry.sdk.trace.export import BatchSpanProcessor, SpanExporter
 from opentelemetry.sdk.trace.sampling import Sampler
 
 from eidolon_ai_client.util.logger import logger
+from eidolon_ai_sdk.agent.audio_agent import AutonomousSpeechAgent
 from eidolon_ai_sdk.agent.doc_manager.document_manager import DocumentManager
 from eidolon_ai_sdk.agent.doc_manager.document_processor import DocumentProcessor
 from eidolon_ai_sdk.agent.doc_manager.loaders.base_loader import DocumentLoader
 from eidolon_ai_sdk.agent.doc_manager.loaders.filesystem_loader import FilesystemLoader
 from eidolon_ai_sdk.agent.doc_manager.loaders.github_loader import GitHubLoader
 from eidolon_ai_sdk.agent.doc_manager.parsers.auto_parser import AutoParser
 from eidolon_ai_sdk.agent.doc_manager.parsers.base_parser import DocumentParser
 from eidolon_ai_sdk.agent.doc_manager.transformer.auto_transformer import AutoTransformer
 from eidolon_ai_sdk.agent.doc_manager.transformer.document_transformer import DocumentTransformer
 from eidolon_ai_sdk.agent.generic_agent import GenericAgent
-from eidolon_ai_sdk.agent.audio_agent import AutonomousSpeechAgent
 from eidolon_ai_sdk.agent.retriever_agent.document_reranker import RAGFusionReranker, DocumentReranker
 from eidolon_ai_sdk.agent.retriever_agent.multi_question_transformer import MultiQuestionTransformer
 from eidolon_ai_sdk.agent.retriever_agent.question_transformer import QuestionTransformer
 from eidolon_ai_sdk.agent.retriever_agent.retriever import Retriever
 from eidolon_ai_sdk.agent.retriever_agent.retriever_agent import RetrieverAgent
 from eidolon_ai_sdk.agent.simple_agent import SimpleAgent
 from eidolon_ai_sdk.agent.tot_agent.checker import ToTChecker
 from eidolon_ai_sdk.agent.tot_agent.thought_generators import ThoughtGenerationStrategy, ProposePromptStrategy
 from eidolon_ai_sdk.agent.tot_agent.tot_agent import TreeOfThoughtsAgent
+from eidolon_ai_sdk.agent_os_interfaces import FileMemory, SymbolicMemory, SimilarityMemory, SecurityManager
 from eidolon_ai_sdk.builtins.components.opentelemetry import OpenTelemetryManager, CustomSampler, NoopSpanExporter
 from eidolon_ai_sdk.builtins.components.usage import UsageMiddleware
 from eidolon_ai_sdk.builtins.logic_units.web_search import WebSearch, Browser, Search
 from eidolon_ai_sdk.cpu.apu import APU
 from eidolon_ai_sdk.cpu.agent_io import IOUnit
 from eidolon_ai_sdk.cpu.audio_unit import AudioUnit
 from eidolon_ai_sdk.cpu.conversation_memory_unit import RawMemoryUnit
 from eidolon_ai_sdk.cpu.conversational_apu import ConversationalAPU
-from eidolon_ai_sdk.agent_os_interfaces import FileMemory, SymbolicMemory, SimilarityMemory, SecurityManager
 from eidolon_ai_sdk.cpu.llm.anthropic_llm_unit import AnthropicLLMUnit
 from eidolon_ai_sdk.cpu.llm.mistral_llm_unit import MistralGPT
 from eidolon_ai_sdk.cpu.llm.open_ai_connection_handler import OpenAIConnectionHandler, AzureOpenAIConnectionHandler
 from eidolon_ai_sdk.cpu.llm.open_ai_image_unit import OpenAIImageUnit
 from eidolon_ai_sdk.cpu.llm.open_ai_llm_unit import OpenAIGPT
 from eidolon_ai_sdk.cpu.llm.open_ai_speech import OpenAiSpeech
 from eidolon_ai_sdk.cpu.llm_unit import LLMUnit, LLMModel
 from eidolon_ai_sdk.cpu.memory_unit import MemoryUnit
+from eidolon_ai_sdk.cpu.tool_call_unit import ToolCallLLMWrapper
 from eidolon_ai_sdk.memory.s3_file_memory import S3FileMemory
 from eidolon_ai_sdk.security.azure_authorizer import AzureJWTProcessor
 from eidolon_ai_sdk.security.google_auth import GoogleJWTProcessor
 from eidolon_ai_sdk.system.dynamic_middleware import Middleware, MultiMiddleware
 from eidolon_ai_sdk.system.process_file_system import ProcessFileSystem, ProcessFileSystemImpl
 from eidolon_ai_usage_client.client import UsageClient
 
@@ -133,14 +134,15 @@
         ConversationalAPU,
         # cpu components
         IOUnit,
         (LLMUnit, OpenAIGPT),
         OpenAIGPT,
         MistralGPT,
         AnthropicLLMUnit,
+        ToolCallLLMWrapper,
         LLMModel,
         (MemoryUnit, RawMemoryUnit),
         RawMemoryUnit,
         WebSearch,
         Search,
         Browser,
         Retriever,
@@ -195,13 +197,14 @@
         OpenAiSpeech,
         AsyncOpenAI,
         AsyncAzureOpenAI,
         UsageClient,
         OpenAIConnectionHandler,
         AzureOpenAIConnectionHandler,
         OpenAIImageUnit,
+        ToolCallLLMWrapper,
         DefaultAzureCredential,
         EnvironmentCredential,
         # config objects
         ReplayConfig,
     ]
     return [_to_resource(maybe_tuple) for maybe_tuple in builtin_list if maybe_tuple]
```

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/components/opentelemetry.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/components/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/components/usage.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/components/usage.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/logic_units/playwrite_browser.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/logic_units/playwrite_browser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/logic_units/web_search.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/logic_units/web_search.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/resources/claude_opus.yaml` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/resources/claude_opus.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/resources/mistral_large.yaml` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/resources/mistral_large.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/resources/mistral_small.yaml` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/resources/mistral_small.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/resources/openai_35.yaml` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/resources/openai_35.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/builtins/resources/openai_4.yaml` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/builtins/resources/openai_4.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/agent_call_history.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/agent_call_history.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/agent_io.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/agent_io.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/agents_logic_unit.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/agents_logic_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/apu.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/apu.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     )
 
 
 class APU(Specable[APUSpec], ABC):
     """
     The APU is the main interface for the Agent to interact with the LLM.
     The APU provides a set of capabilities that encapsulate LLM functionality and creates a clear separation between business logic and the underlying LLM implementation.
+
+    To learn more, check out our blog article APU: [What is it and how does it work?](https://www.eidolonai.com/what_is_apu/).
     """
 
     title: str
 
     def __init__(self, spec: T, **kwargs: object):
         super().__init__(spec, **kwargs)
         self.title = "default"
```

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/audio_unit.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/audio_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/conversation_memory_unit.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/conversation_memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/conversational_apu.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/conversational_apu.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from eidolon_ai_sdk.agent_os import AgentOS
 from eidolon_ai_sdk.cpu.apu import APU, APUSpec, Thread, APUException, APUCapabilities
 from eidolon_ai_sdk.cpu.agent_io import IOUnit, CPUMessageTypes
 from eidolon_ai_sdk.cpu.audio_unit import AudioUnit
 from eidolon_ai_sdk.cpu.call_context import CallContext
 from eidolon_ai_sdk.cpu.image_unit import ImageUnit
 from eidolon_ai_sdk.cpu.llm_message import (
-    AssistantMessage,
     ToolResponseMessage,
     LLMMessage,
     UserMessageFile,
     UserMessageAudio,
     UserMessageImage,
     UserMessageText,
     UserMessage,
@@ -65,14 +64,15 @@
         kwargs = dict(processing_unit_locator=self)
         self.io_unit = self.spec.io_unit.instantiate(**kwargs)
         self.memory_unit = self.spec.memory_unit.instantiate(**kwargs)
         self.llm_unit = self.spec.llm_unit.instantiate(**kwargs)
         self.logic_units = [logic_unit.instantiate(**kwargs) for logic_unit in self.spec.logic_units]
         self.audio_unit = self.spec.audio_unit.instantiate(**kwargs) if self.spec.audio_unit else None
         self.image_unit = self.spec.image_unit.instantiate(**kwargs) if self.spec.image_unit else None
+
         self.record_memory = self.spec.record_conversation
         self.document_processor = self.spec.document_processor.instantiate()
         if self.audio_unit:
             self.logic_units.append(self.audio_unit)
         if self.image_unit:
             self.logic_units.append(self.image_unit)
 
@@ -111,18 +111,18 @@
         raise ValueError(f"Could not locate {unit_type}")
 
     async def set_boot_messages(self, call_context: CallContext, boot_messages: List[CPUMessageTypes]):
         conversation_messages = await self.io_unit.process_request(call_context, boot_messages)
         await self.memory_unit.storeBootMessages(call_context, conversation_messages)
 
     async def schedule_request(
-        self,
-        call_context: CallContext,
-        prompts: List[CPUMessageTypes],
-        output_format: Union[Literal["str"], Dict[str, Any]] = "str",
+            self,
+            call_context: CallContext,
+            prompts: List[CPUMessageTypes],
+            output_format: Union[Literal["str"], Dict[str, Any]] = "str",
     ) -> AsyncIterator[StreamEvent]:
         try:
             conversation = await self.memory_unit.getConversationHistory(call_context)
             conversation_messages = await self.io_unit.process_request(call_context, prompts)
             if self.record_memory:
                 await self.memory_unit.storeMessages(call_context, conversation_messages)
             conversation.extend(conversation_messages)
@@ -133,18 +133,18 @@
         except APUException as e:
             raise e
         except Exception as e:
             logger.exception(e)
             raise APUException(f"{e.__class__.__name__} while processing request") from e
 
     async def _llm_execution_cycle(
-        self,
-        call_context: CallContext,
-        output_format: Union[Literal["str"], Dict[str, Any]],
-        conversation: List[LLMMessage],
+            self,
+            call_context: CallContext,
+            output_format: Union[Literal["str"], Dict[str, Any]],
+            conversation: List[LLMMessage],
     ) -> AsyncIterator[StreamEvent]:
         # first convert the conversation to fill in file data
         converted_conversation = []
         for event in conversation:
             if isinstance(event, UserMessage):
                 converted_messages = []
                 for message in event.content:
@@ -176,19 +176,16 @@
                 async for event in stream_collector:
                     if event.is_root_and_type(LLMToolCallRequestEvent):
                         tool_call_events.append(event)
                     yield event
             if stream_collector.get_content():
                 logger.info(f"LLM Response: {stream_collector.get_content()}")
 
-            assistant_message = AssistantMessage(
-                type="assistant",
-                content=stream_collector.get_content() or "",
-                tool_calls=[tce.tool_call for tce in tool_call_events],
-            )
+            assistant_message = self.llm_unit.create_assistant_message(call_context, stream_collector.get_content() or "", tool_call_events)
+
             if self.record_memory:
                 await self.memory_unit.storeMessages(call_context, [assistant_message])
             converted_conversation.append(assistant_message)
 
             if tool_call_events:
                 with tracer.start_as_current_span("tool calls"):
                     streams = [
@@ -198,19 +195,19 @@
                         yield e
             else:
                 return
 
         raise APUException(f"exceeded maximum number of function calls ({self.spec.max_num_function_calls})")
 
     async def _call_tool(
-        self,
-        call_context: CallContext,
-        tool_call_event: LLMToolCallRequestEvent,
-        tool_defs,
-        conversation: List[LLMMessage],
+            self,
+            call_context: CallContext,
+            tool_call_event: LLMToolCallRequestEvent,
+            tool_defs,
+            conversation: List[LLMMessage],
     ):
         tc = tool_call_event.tool_call
         logic_unit_wrapper = ["NaN"]
 
         if tc.name not in tool_defs:
             message = ToolResponseMessage(
                 logic_unit_name=logic_unit_wrapper[0],
@@ -245,20 +242,15 @@
                     yield event
             except ManagedContextError:
                 if self.spec.allow_tool_errors:
                     logger.warning("Error calling tool " + tool_call_event.tool_call.name, exc_info=True)
                 else:
                     raise
 
-            message = ToolResponseMessage(
-                logic_unit_name=logic_unit_wrapper[0],
-                tool_call_id=tc.tool_call_id,
-                result=tool_stream.get_content() or "",
-                name=tc.name,
-            )
+            message = self.llm_unit.create_tool_response_message(logic_unit_wrapper[0], tc, tool_stream.get_content() or "")
 
         if self.record_memory:
             await self.memory_unit.storeMessages(call_context, [message])
         conversation.append(message)
 
     async def process_audio_message(self, message: UserMessageAudio):
         if self.audio_unit is None:
```

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/image_unit.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/image_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/llm/open_ai_speech.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/llm/open_ai_speech.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/llm_message.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/llm_message.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/logic_unit.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/logic_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/memory_unit.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/cpu/processing_unit.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/cpu/processing_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/agent_memory.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/agent_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/chroma_vector_store.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/chroma_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/document.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/document.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/embeddings.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/file_memory.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/file_system_vector_store.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/file_system_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/in_memory_file_memory.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/in_memory_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/local_file_memory.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/local_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/local_symbolic_memory.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/local_symbolic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/mongo_symbolic_memory.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/mongo_symbolic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/noop_memory.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/noop_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/s3_file_memory.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/s3_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/semantic_memory.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/semantic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/similarity_memory.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/similarity_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/memory/vector_store.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/memory/vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/security/authentication_processor.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/security/authentication_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/security/azure_authorizer.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/security/azure_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/security/functional_authorizer.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/security/functional_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/security/google_auth.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/security/google_auth.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/security/jwt_processor.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/security/jwt_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/security/permissions.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/security/permissions.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/security/process_authorizer.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/security/process_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/security/security_manager.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/security/security_manager.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/security/security_middleware.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/security/security_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/system/agent_contract.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/system/agent_contract.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/system/agent_controller.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/system/agent_controller.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/system/agent_machine.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/system/agent_machine.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/system/dynamic_middleware.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/system/dynamic_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/system/fn_handler.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/system/fn_handler.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/system/process_file_system.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/system/process_file_system.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/system/processes.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/system/processes.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/system/reference_model.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/system/reference_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,27 @@
     """
 
     spec: T
 
     def __init__(self, spec: T, **kwargs: object):
         self.spec = spec
 
+    @classmethod
+    def model_json_schema(cls):
+        bases = getattr(cls, "__orig_bases__", [])
+        specable = next(
+            (base for base in bases if getattr(base, "__origin__", None) is Specable),
+            None,
+        )
+        if specable:
+            model = specable.__args__[0]
+            return model.model_json_schema()
+        else:
+            raise ValueError(f"Specable base {cls} not found")
+
 
 B = TypeVar("B")
 D = TypeVar("D")
 
 
 class Reference(BaseModel):
     """
@@ -65,14 +78,21 @@
         if not isinstance(params, tuple):
             params = (params, fqn(params))
 
         class _Reference(cls):
             _bound = params[0]
             _default = params[1]
 
+            class Config:
+                title = (params[0] if isinstance(params[0], str) else params[0].__name__) + " Reference"
+                json_schema_extra = {
+                    "type": f"Reference[{params[0] if isinstance(params[0], str) else params[0].__name__}]",
+                    "default": str(params[1]),
+                }
+
             @model_validator(mode="before")
             def _dump_ref(cls, value):
                 return value.model_dump(exclude_defaults=True) if isinstance(value, Reference) else value
 
             def __reduce__(self):
                 return (
                     _ReferenceGetter(),
```

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/system/resources/reference_resource.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/system/resources/reference_resource.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/system/resources/resources_base.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/system/resources/resources_base.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/util/class_utils.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/util/class_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/util/image_utils.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/util/image_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/util/replay.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/util/replay.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/util/schema_to_model.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/util/schema_to_model.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/util/str_utils.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/util/str_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/eidolon_ai_sdk/util/stream_collector.py` & `eidolon_ai_sdk-0.1.57/eidolon_ai_sdk/util/stream_collector.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/logging.conf` & `eidolon_ai_sdk-0.1.57/logging.conf`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.56/pyproject.toml` & `eidolon_ai_sdk-0.1.57/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "eidolon-ai-sdk"
-version = "0.1.56"
+version = "0.1.57"
 description = "An open source sgent service SDK"
 authors = [ "Luke Lalor <lukehlalor@gmail.com>",]
 readme = "README.md"
 include = [ "logging.conf",]
 
 [tool.ruff]
 line-length = 121
 
 [tool.eidolon]
 update-tag = "sdk"
-last-update-hash = "541685ffdf5642e3f5909d3c6c8e4098e83f83fd"
+last-update-hash = "714b630ad51a720327978063a76b437b05912b83"
 
 [tool.poetry.urls]
 Github = "https://github.com/eidolon-ai/eidolon"
 Website = "https://www.eidolonai.com/"
 
 [tool.poetry.scripts]
 eidolon-server = "eidolon_ai_sdk.bin.agent_http_server:main"
@@ -57,15 +57,15 @@
 httpx-sse = "^0.4.0"
 sse-starlette = "^2.0.0"
 dill = "^0.3.8"
 opentelemetry-instrumentation-fastapi = "^0.44b0"
 opentelemetry-instrumentation-logging = "^0.44b0"
 opentelemetry-sdk = "^1.23.0"
 eidolon-ai-mistralai = "^0.1.6a"
-eidolon-ai-client = "^0.1.21"
+eidolon-ai-client = "^0.1.22"
 eidolon-ai-usage-client = "^0.1.6"
 boto3 = "^1.34.74"
 azure-identity = "^1.16.0"
 playwright = "^1.43.0"
 
 [tool.pytest.ini_options]
 pythonpath = "project"
```

### Comparing `eidolon_ai_sdk-0.1.56/PKG-INFO` & `eidolon_ai_sdk-0.1.57/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: eidolon-ai-sdk
-Version: 0.1.56
+Version: 0.1.57
 Summary: An open source sgent service SDK
 Author: Luke Lalor
 Author-email: lukehlalor@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anthropic (>=0.21.3,<0.22.0)
 Requires-Dist: authlib (>=1.3.0,<2.0.0)
 Requires-Dist: azure-identity (>=1.16.0,<2.0.0)
 Requires-Dist: boto3 (>=1.34.74,<2.0.0)
 Requires-Dist: boto3-stubs[essential] (>=1.34.74,<2.0.0)
 Requires-Dist: chromadb (>=0.4.18,<0.5.0)
 Requires-Dist: dill (>=0.3.8,<0.4.0)
-Requires-Dist: eidolon-ai-client (>=0.1.21,<0.2.0)
+Requires-Dist: eidolon-ai-client (>=0.1.22,<0.2.0)
 Requires-Dist: eidolon-ai-mistralai (>=0.1.6a,<0.2.0)
 Requires-Dist: eidolon-ai-usage-client (>=0.1.6,<0.2.0)
 Requires-Dist: esprima (>=4.0.1,<5.0.0)
 Requires-Dist: fastapi (>=0.109.0,<0.110.0)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: httpx-sse (>=0.4.0,<0.5.0)
```

