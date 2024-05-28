# Comparing `tmp/langtrace_python_sdk-2.0.9.tar.gz` & `tmp/langtrace_python_sdk-2.1.0.tar.gz`

## Comparing `langtrace_python_sdk-2.0.9.tar` & `langtrace_python_sdk-2.1.0.tar`

### file list

```diff
@@ -1,140 +1,146 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/__init__.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/run_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/anthropic_example/__init__.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/anthropic_example/completion.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/chroma_example/__init__.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/chroma_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/cohere_example/__init__.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/cohere_example/chat.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/cohere_example/chat_stream.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/cohere_example/embed.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/cohere_example/rerank.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/cohere_example/tools.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/fastapi_example/basic_route.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/hiveagent_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/langchain_example/__init__.py
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/langchain_example/basic.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/langchain_example/groq_example.py
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/langchain_example/langgraph_example.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/langchain_example/tool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/llamaindex_example/__init__.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/llamaindex_example/agent.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/llamaindex_example/basic.py
--rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/llamaindex_example/data/abramov.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/openai_example/__init__.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/openai_example/async_tool_calling_nonstreaming.py
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/openai_example/async_tool_calling_streaming.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/openai_example/chat_completion.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/openai_example/embeddings_create.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/openai_example/function_calling.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/openai_example/images_generate.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/openai_example/tool_calling.py
--rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/openai_example/tool_calling_nonstreaming.py
--rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/openai_example/tool_calling_streaming.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/perplexity_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/pinecone_example/__init__.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/pinecone_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/qdrant_example/__init__.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/examples/qdrant_example/basic.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/__init__.py
--rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/langtrace.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/constants/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/constants/instrumentation/__init__.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/constants/instrumentation/chroma.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/constants/instrumentation/cohere.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/constants/instrumentation/common.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/constants/instrumentation/groq.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/constants/instrumentation/openai.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/constants/instrumentation/qdrant.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/extensions/__init__.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/extensions/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
--rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/chroma/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
--rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/cohere/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/groq/__init__.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py
--rw-r--r--   0        0        0    26068 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/groq/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/langchain/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
--rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
--rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/langgraph/__init__.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py
--rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/langgraph/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
--rw-r--r--   0        0        0     4189 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
--rw-r--r--   0        0        0    37263 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/openai/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/qdrant/__init__.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py
--rw-r--r--   0        0        0     3883 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/qdrant/patch.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/types/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/utils/__init__.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/utils/llm.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/utils/prompt_registry.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/utils/silently_fail.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/utils/types.py
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/utils/with_root_span.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/__init__.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/conftest.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/utils.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/anthropic/conftest.py
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/anthropic/test_anthropic.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/anthropic/cassettes/test_anthropic.yaml
--rw-r--r--   0        0        0    11675 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml
--rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/chroma/conftest.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/chroma/test_chroma.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/cohere/conftest.py
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/cohere/test_cohere_chat.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/cohere/test_cohere_embed.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/cohere/test_cohere_rerank.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/cohere/cassettes/test_cohere_chat.yaml
--rw-r--r--   0        0        0    10610 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml
--rw-r--r--   0        0        0    27312 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/cohere/cassettes/test_cohere_embed.yaml
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/cohere/cassettes/test_cohere_rerank.yaml
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/langchain/test_langchain.py
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/langchain/test_langchain_community.py
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/langchain/test_langchain_core.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/openai/conftest.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/openai/test_chat_completion.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/openai/test_embeddings.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/openai/test_image_generation.py
--rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/openai/cassettes/test_async_image_generation.yaml
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/openai/cassettes/test_chat_completion.yaml
--rw-r--r--   0        0        0  2592394 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/openai/cassettes/test_chat_completion_streaming.yaml
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/openai/cassettes/test_image_generation.yaml
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/pinecone/conftest.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/pinecone/test_pinecone.py
--rw-r--r--   0        0        0   103821 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/pinecone/cassettes/test_query.yaml
--rw-r--r--   0        0        0    38607 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/pinecone/cassettes/test_upsert.yaml
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/qdrant/conftest.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/src/tests/qdrant/test_qdrant.py
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/LICENSE
--rw-r--r--   0        0        0     8740 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/README.md
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/pyproject.toml
--rw-r--r--   0        0        0    10097 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.9/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/__init__.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/run_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/anthropic_example/__init__.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/anthropic_example/completion.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/chroma_example/__init__.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/chroma_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/cohere_example/__init__.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/cohere_example/chat.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/cohere_example/chat_stream.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/cohere_example/embed.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/cohere_example/rerank.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/cohere_example/tools.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/fastapi_example/basic_route.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/hiveagent_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/langchain_example/__init__.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/langchain_example/basic.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/langchain_example/groq_example.py
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/langchain_example/langgraph_example.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/langchain_example/tool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/llamaindex_example/__init__.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/llamaindex_example/agent.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/llamaindex_example/basic.py
+-rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/llamaindex_example/data/abramov.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/openai_example/__init__.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/openai_example/async_tool_calling_nonstreaming.py
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/openai_example/async_tool_calling_streaming.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/openai_example/chat_completion.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/openai_example/embeddings_create.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/openai_example/function_calling.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/openai_example/images_generate.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/openai_example/tool_calling.py
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/openai_example/tool_calling_nonstreaming.py
+-rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/openai_example/tool_calling_streaming.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/perplexity_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/pinecone_example/__init__.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/pinecone_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/qdrant_example/__init__.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/qdrant_example/basic.py
+-rw-r--r--   0        0        0    64533 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/examples/weaviate_example/query_text.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/__init__.py
+-rw-r--r--   0        0        0     6993 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/langtrace.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/constants/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/constants/instrumentation/__init__.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/constants/instrumentation/chroma.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/constants/instrumentation/cohere.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/constants/instrumentation/common.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/constants/instrumentation/groq.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/constants/instrumentation/openai.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/constants/instrumentation/qdrant.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/constants/instrumentation/weaviate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/extensions/__init__.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/extensions/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
+-rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
+-rw-r--r--   0        0        0     8750 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/chroma/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
+-rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/cohere/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/groq/__init__.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py
+-rw-r--r--   0        0        0    26068 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/groq/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/langchain/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
+-rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
+-rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/langgraph/__init__.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py
+-rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/langgraph/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
+-rw-r--r--   0        0        0     4189 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
+-rw-r--r--   0        0        0    37288 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/openai/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
+-rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/qdrant/__init__.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/qdrant/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/weaviate/__init__.py
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/weaviate/instrumentation.py
+-rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/weaviate/patch.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/types/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/utils/llm.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/utils/misc.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/utils/prompt_registry.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/utils/silently_fail.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/utils/types.py
+-rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/utils/with_root_span.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/__init__.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/conftest.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/utils.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/anthropic/conftest.py
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/anthropic/test_anthropic.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/anthropic/cassettes/test_anthropic.yaml
+-rw-r--r--   0        0        0    11675 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml
+-rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/chroma/conftest.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/chroma/test_chroma.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/cohere/conftest.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/cohere/test_cohere_chat.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/cohere/test_cohere_embed.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/cohere/test_cohere_rerank.py
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/cohere/cassettes/test_cohere_chat.yaml
+-rw-r--r--   0        0        0     8174 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml
+-rw-r--r--   0        0        0    27320 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/cohere/cassettes/test_cohere_embed.yaml
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/cohere/cassettes/test_cohere_rerank.yaml
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/langchain/test_langchain.py
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/langchain/test_langchain_community.py
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/langchain/test_langchain_core.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/openai/conftest.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/openai/test_chat_completion.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/openai/test_embeddings.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/openai/test_image_generation.py
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/openai/cassettes/test_async_image_generation.yaml
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/openai/cassettes/test_chat_completion.yaml
+-rw-r--r--   0        0        0  2592394 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/openai/cassettes/test_chat_completion_streaming.yaml
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/openai/cassettes/test_image_generation.yaml
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/pinecone/conftest.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/pinecone/test_pinecone.py
+-rw-r--r--   0        0        0   103821 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/pinecone/cassettes/test_query.yaml
+-rw-r--r--   0        0        0    38607 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/pinecone/cassettes/test_upsert.yaml
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/qdrant/conftest.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/src/tests/qdrant/test_qdrant.py
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/LICENSE
+-rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/README.md
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.1.0/PKG-INFO
```

### Comparing `langtrace_python_sdk-2.0.9/src/run_example.py` & `langtrace_python_sdk-2.1.0/src/run_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/examples/anthropic_example/completion.py` & `langtrace_python_sdk-2.1.0/src/examples/anthropic_example/completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/examples/chroma_example/basic.py` & `langtrace_python_sdk-2.1.0/src/examples/chroma_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/examples/cohere_example/chat.py` & `langtrace_python_sdk-2.1.0/src/examples/cohere_example/chat.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/examples/cohere_example/chat_stream.py` & `langtrace_python_sdk-2.1.0/src/examples/cohere_example/chat_stream.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/examples/cohere_example/embed.py` & `langtrace_python_sdk-2.1.0/src/examples/cohere_example/embed.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/examples/cohere_example/rerank.py` & `langtrace_python_sdk-2.1.0/src/examples/cohere_example/rerank.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/examples/cohere_example/tools.py` & `langtrace_python_sdk-2.1.0/src/examples/cohere_example/tools.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/examples/fastapi_example/basic_route.py` & `langtrace_python_sdk-2.1.0/src/examples/fastapi_example/basic_route.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/examples/langchain_example/basic.py` & `langtrace_python_sdk-2.1.0/src/examples/langchain_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/examples/langchain_example/groq_example.py` & `langtrace_python_sdk-2.1.0/src/examples/langchain_example/groq_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/examples/langchain_example/langgraph_example.py` & `langtrace_python_sdk-2.1.0/src/examples/langchain_example/langgraph_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/examples/langchain_example/tool.py` & `langtrace_python_sdk-2.1.0/src/examples/langchain_example/tool.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/examples/llamaindex_example/agent.py` & `langtrace_python_sdk-2.1.0/src/examples/llamaindex_example/agent.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/examples/llamaindex_example/basic.py` & `langtrace_python_sdk-2.1.0/src/examples/llamaindex_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/examples/llamaindex_example/data/abramov.txt` & `langtrace_python_sdk-2.1.0/src/examples/llamaindex_example/data/abramov.txt`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/examples/openai_example/async_tool_calling_nonstreaming.py` & `langtrace_python_sdk-2.1.0/src/examples/openai_example/async_tool_calling_nonstreaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/examples/openai_example/async_tool_calling_streaming.py` & `langtrace_python_sdk-2.1.0/src/examples/openai_example/async_tool_calling_streaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/examples/openai_example/chat_completion.py` & `langtrace_python_sdk-2.1.0/src/examples/openai_example/chat_completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/examples/openai_example/function_calling.py` & `langtrace_python_sdk-2.1.0/src/examples/openai_example/function_calling.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/examples/openai_example/tool_calling.py` & `langtrace_python_sdk-2.1.0/src/examples/openai_example/tool_calling.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/examples/openai_example/tool_calling_nonstreaming.py` & `langtrace_python_sdk-2.1.0/src/examples/openai_example/tool_calling_nonstreaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/examples/openai_example/tool_calling_streaming.py` & `langtrace_python_sdk-2.1.0/src/examples/openai_example/tool_calling_streaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/examples/perplexity_example/basic.py` & `langtrace_python_sdk-2.1.0/src/examples/perplexity_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/examples/pinecone_example/basic.py` & `langtrace_python_sdk-2.1.0/src/examples/pinecone_example/basic.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 """
 
 from langtrace_python_sdk import langtrace
 from dotenv import find_dotenv, load_dotenv
 from openai import OpenAI
 from pinecone import Pinecone
 
-from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
+
+from langtrace_python_sdk import with_langtrace_root_span, send_user_feedback
 
 _ = load_dotenv(find_dotenv())
 
 langtrace.init()
 
 client = OpenAI()
 pinecone = Pinecone()
 
 
 @with_langtrace_root_span()
-def basic():
+def basic(span_id, trace_id):
+
     result = client.embeddings.create(
         model="text-embedding-ada-002",
         input="Some random text string goes here",
         encoding_format="float",
     )
 
     embedding = result.data[0].embedding
@@ -33,8 +35,11 @@
     index = pinecone.Index("test-index")
     res = index.upsert(vectors=[data_to_upsert], namespace="test-namespace")
     print("res", res)
 
     resp = index.query(
         vector=embedding, top_k=1, include_values=False, namespace="test-namespace"
     )
+    send_user_feedback(
+        {"spanId": span_id, "traceId": trace_id, "userScore": 1, "userId": "123"}
+    )
     print(resp)
```

### Comparing `langtrace_python_sdk-2.0.9/src/examples/qdrant_example/basic.py` & `langtrace_python_sdk-2.1.0/src/examples/qdrant_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/__init__.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,9 +13,15 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from langtrace_python_sdk import langtrace
 from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
 from langtrace_python_sdk.utils.prompt_registry import get_prompt_from_registry
+from langtrace_python_sdk.utils.with_root_span import send_user_feedback
 
-__all__ = ["langtrace", "with_langtrace_root_span", "get_prompt_from_registry"]
+__all__ = [
+    "langtrace",
+    "with_langtrace_root_span",
+    "get_prompt_from_registry",
+    "send_user_feedback",
+]
```

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/langtrace.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/langtrace.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,17 @@
 )
 from langtrace_python_sdk.instrumentation.pinecone.instrumentation import (
     PineconeInstrumentation,
 )
 from langtrace_python_sdk.instrumentation.qdrant.instrumentation import (
     QdrantInstrumentation,
 )
+from langtrace_python_sdk.instrumentation.weaviate.instrumentation import (
+    WeaviateInstrumentation,
+)
 
 
 def init(
     api_key: str = None,
     batch: bool = True,
     write_spans_to_console: bool = False,
     custom_remote_exporter=None,
@@ -115,14 +118,15 @@
         "qdrant": QdrantInstrumentation(),
         "langchain": LangchainInstrumentation(),
         "langchain_core": LangchainCoreInstrumentation(),
         "langchain_community": LangchainCommunityInstrumentation(),
         "langgraph": LanggraphInstrumentation(),
         "anthropic": AnthropicInstrumentation(),
         "cohere": CohereInstrumentation(),
+        "weaviate": WeaviateInstrumentation(),
     }
 
     init_instrumentations(disable_instrumentations, all_instrumentations)
 
 
 def init_instrumentations(
     disable_instrumentations: DisableInstrumentations, all_instrumentations: dict
```

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/constants/instrumentation/chroma.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/constants/instrumentation/chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/constants/instrumentation/cohere.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/constants/instrumentation/cohere.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/constants/instrumentation/common.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/constants/instrumentation/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,10 +18,11 @@
     "LANGGRAPH": "Langgraph",
     "LLAMAINDEX": "LlamaIndex",
     "OPENAI": "OpenAI",
     "PINECONE": "Pinecone",
     "COHERE": "Cohere",
     "PPLX": "Perplexity",
     "QDRANT": "Qdrant",
+    "WEAVIATE": "Weaviate",
 }
 
 LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY = "langtrace_additional_attributes"
```

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/constants/instrumentation/openai.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/constants/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/constants/instrumentation/qdrant.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/constants/instrumentation/qdrant.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/extensions/langtrace_exporter.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/extensions/langtrace_exporter.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/anthropic/patch.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/anthropic/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/chroma/patch.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,65 +10,100 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from langtrace.trace_attributes import DatabaseSpanAttributes
+from langtrace.trace_attributes import FrameworkSpanAttributes
 from opentelemetry import baggage
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
 
-from langtrace_python_sdk.constants.instrumentation.chroma import APIS
 from langtrace_python_sdk.constants.instrumentation.common import (
     LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY,
     SERVICE_PROVIDERS,
 )
 
 
-def collection_patch(method, version, tracer):
-    """
-    A generic patch method that wraps a function with a span
+def generic_patch(method, task, tracer, version):
     """
+    A generic patch method that wraps a function with a span"""
 
     def traced_method(wrapped, instance, args, kwargs):
-        api = APIS[method]
-        service_provider = SERVICE_PROVIDERS["CHROMA"]
+        service_provider = SERVICE_PROVIDERS["LLAMAINDEX"]
         extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
 
         span_attributes = {
             "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
-            "langtrace.service.type": "vectordb",
+            "langtrace.service.type": "framework",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
-            "db.system": "chromadb",
-            "db.operation": api["OPERATION"],
+            "llamaindex.task.name": task,
             **(extra_attributes if extra_attributes is not None else {}),
         }
 
-        if hasattr(instance, "name") and instance.name is not None:
-            span_attributes["db.collection.name"] = instance.name
-
-        attributes = DatabaseSpanAttributes(**span_attributes)
+        attributes = FrameworkSpanAttributes(**span_attributes)
 
-        with tracer.start_as_current_span(api["METHOD"], kind=SpanKind.CLIENT) as span:
+        with tracer.start_as_current_span(method, kind=SpanKind.CLIENT) as span:
             for field, value in attributes.model_dump(by_alias=True).items():
                 if value is not None:
                     span.set_attribute(field, value)
             try:
                 # Attempt to call the original method
                 result = wrapped(*args, **kwargs)
                 span.set_status(StatusCode.OK)
                 return result
             except Exception as err:
                 # Record the exception in the span
                 span.record_exception(err)
 
                 # Set the span status to indicate an error
+                span.set_status(Status(StatusCode.ERROR, str(err)))
+
+                # Reraise the exception to ensure it's not swallowed
+                raise
+
+    return traced_method
+
+
+def async_generic_patch(method, task, tracer, version):
+    """
+    A generic patch method that wraps a function with a span"""
+
+    async def traced_method(wrapped, instance, args, kwargs):
+        service_provider = SERVICE_PROVIDERS["LLAMAINDEX"]
+        extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
+
+        span_attributes = {
+            "langtrace.sdk.name": "langtrace-python-sdk",
+            "langtrace.service.name": service_provider,
+            "langtrace.service.type": "framework",
+            "langtrace.service.version": version,
+            "langtrace.version": "1.0.0",
+            "llamaindex.task.name": task,
+            **(extra_attributes if extra_attributes is not None else {}),
+        }
+
+        attributes = FrameworkSpanAttributes(**span_attributes)
+
+        with tracer.start_as_current_span(method, kind=SpanKind.CLIENT) as span:
+            async for field, value in attributes.model_dump(by_alias=True).items():
+                if value is not None:
+                    span.set_attribute(field, value)
+            try:
+                # Attempt to call the original method
+                result = await wrapped(*args, **kwargs)
+                span.set_status(StatusCode.OK)
+                return result
+            except Exception as err:
+                # Record the exception in the span
+                span.record_exception(err)
+
+                # Set the span status to indicate an error
                 span.set_status(Status(StatusCode.ERROR, str(err)))
 
                 # Reraise the exception to ensure it's not swallowed
                 raise
 
     return traced_method
```

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/cohere/patch.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/cohere/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/groq/patch.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/groq/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/langchain/patch.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/langchain/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/langgraph/patch.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/langgraph/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/pinecone/patch.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,100 +10,118 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from langtrace.trace_attributes import FrameworkSpanAttributes
+from langtrace.trace_attributes import DatabaseSpanAttributes
+from langtrace_python_sdk.utils import set_span_attribute
+from langtrace_python_sdk.utils.silently_fail import silently_fail
 from opentelemetry import baggage
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
 
 from langtrace_python_sdk.constants.instrumentation.common import (
     LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY,
     SERVICE_PROVIDERS,
 )
+from langtrace_python_sdk.constants.instrumentation.pinecone import APIS
+import json
 
 
-def generic_patch(method, task, tracer, version):
+def generic_patch(original_method, method, version, tracer):
     """
     A generic patch method that wraps a function with a span"""
 
     def traced_method(wrapped, instance, args, kwargs):
-        service_provider = SERVICE_PROVIDERS["LLAMAINDEX"]
+        api = APIS[method]
+        service_provider = SERVICE_PROVIDERS["PINECONE"]
         extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
 
         span_attributes = {
             "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
-            "langtrace.service.type": "framework",
+            "langtrace.service.type": "vectordb",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
-            "llamaindex.task.name": task,
+            "db.system": "pinecone",
+            "db.operation": api["OPERATION"],
+            "db.query": json.dumps(kwargs.get("query")),
             **(extra_attributes if extra_attributes is not None else {}),
         }
 
-        attributes = FrameworkSpanAttributes(**span_attributes)
+        attributes = DatabaseSpanAttributes(**span_attributes)
 
-        with tracer.start_as_current_span(method, kind=SpanKind.CLIENT) as span:
-            for field, value in attributes.model_dump(by_alias=True).items():
-                if value is not None:
-                    span.set_attribute(field, value)
-            try:
-                # Attempt to call the original method
-                result = wrapped(*args, **kwargs)
-                span.set_status(StatusCode.OK)
-                return result
-            except Exception as err:
-                # Record the exception in the span
-                span.record_exception(err)
-
-                # Set the span status to indicate an error
-                span.set_status(Status(StatusCode.ERROR, str(err)))
-
-                # Reraise the exception to ensure it's not swallowed
-                raise
-
-    return traced_method
+        with tracer.start_as_current_span(api["METHOD"], kind=SpanKind.CLIENT) as span:
 
+            if span.is_recording():
+                set_span_attribute(span, "server.address", instance._config.host)
+                if method == "QUERY":
+                    set_query_input_attributes(span, kwargs)
 
-def async_generic_patch(method, task, tracer, version):
-    """
-    A generic patch method that wraps a function with a span"""
-
-    async def traced_method(wrapped, instance, args, kwargs):
-        service_provider = SERVICE_PROVIDERS["LLAMAINDEX"]
-        extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
-
-        span_attributes = {
-            "langtrace.sdk.name": "langtrace-python-sdk",
-            "langtrace.service.name": service_provider,
-            "langtrace.service.type": "framework",
-            "langtrace.service.version": version,
-            "langtrace.version": "1.0.0",
-            "llamaindex.task.name": task,
-            **(extra_attributes if extra_attributes is not None else {}),
-        }
-
-        attributes = FrameworkSpanAttributes(**span_attributes)
-
-        with tracer.start_as_current_span(method, kind=SpanKind.CLIENT) as span:
-            async for field, value in attributes.model_dump(by_alias=True).items():
+            for field, value in attributes.model_dump(by_alias=True).items():
                 if value is not None:
                     span.set_attribute(field, value)
             try:
                 # Attempt to call the original method
-                result = await wrapped(*args, **kwargs)
+                result = original_method(instance, *args, **kwargs)
+                if result:
+                    if span.is_recording():
+                        set_query_response_attributes(span, result)
                 span.set_status(StatusCode.OK)
                 return result
             except Exception as err:
                 # Record the exception in the span
                 span.record_exception(err)
 
                 # Set the span status to indicate an error
                 span.set_status(Status(StatusCode.ERROR, str(err)))
 
                 # Reraise the exception to ensure it's not swallowed
                 raise
 
+    @silently_fail
+    def set_query_input_attributes(span, kwargs):
+        set_span_attribute(span, "db.query.top_k", kwargs.get("top_k"))
+        set_span_attribute(span, "db.query.namespace", kwargs.get("namespace"))
+        set_span_attribute(span, "db.query.id", kwargs.get("id"))
+        filter = (
+            json.dumps(kwargs.get("filter"))
+            if isinstance(kwargs.get("filter"), dict)
+            else kwargs.get("filter")
+        )
+        set_span_attribute(span, "db.query.filter", filter)
+        set_span_attribute(
+            span, "db.query.include_values", kwargs.get("include_values")
+        )
+        set_span_attribute(
+            span, "db.query.include_metadata", kwargs.get("include_metadata")
+        )
+
+    @silently_fail
+    def set_query_response_attributes(span, response):
+        matches = response.get("matches")
+
+        usage = response.get("usage")
+        for match in matches:
+            span.add_event(
+                name="db.query.match",
+                attributes={
+                    "db.query.match.id": match.get("id"),
+                    "db.query.match.score": match.get("score"),
+                    "db.query.match.metadata": match.get("metadata"),
+                    # "db.query.match.values": match.get("values"),
+                },
+            )
+
+        if "read_units" in usage:
+            set_span_attribute(
+                span, "db.query.usage.read_units", usage.get("read_units")
+            )
+
+        if "write_units" in usage:
+            set_span_attribute(
+                span, "db.query.usage.write_units", usage.get("write_units")
+            )
+
     return traced_method
```

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/openai/patch.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/openai/patch.py`

 * *Files 0% similar despite different names*

```diff
@@ -612,14 +612,15 @@
         result, span, prompt_tokens, function_call=False, tool_calls=False
     ):
         """Process and yield streaming response chunks."""
         result_content = []
         span.add_event(Event.STREAM_START.value)
         completion_tokens = 0
         try:
+            content = []
             async for chunk in result:
                 if hasattr(chunk, "model") and chunk.model is not None:
                     span.set_attribute("llm.model", chunk.model)
                 if hasattr(chunk, "choices") and chunk.choices is not None:
                     if not function_call and not tool_calls:
                         for choice in chunk.choices:
                             if choice.delta and choice.delta.content is not None:
```

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/pinecone/patch.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/qdrant/patch.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,117 +10,121 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+import json
 from langtrace.trace_attributes import DatabaseSpanAttributes
-from langtrace_python_sdk.utils import set_span_attribute
 from langtrace_python_sdk.utils.silently_fail import silently_fail
+from langtrace_python_sdk.utils.llm import set_span_attributes
 from opentelemetry import baggage
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace.status import Status, StatusCode
 
 from langtrace_python_sdk.constants.instrumentation.common import (
     LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY,
     SERVICE_PROVIDERS,
 )
-from langtrace_python_sdk.constants.instrumentation.pinecone import APIS
-import json
+from langtrace_python_sdk.constants.instrumentation.qdrant import APIS
 
 
-def generic_patch(original_method, method, version, tracer):
+def collection_patch(method, version, tracer):
+    """
+    A generic patch method that wraps a function with a span
     """
-    A generic patch method that wraps a function with a span"""
 
     def traced_method(wrapped, instance, args, kwargs):
         api = APIS[method]
-        service_provider = SERVICE_PROVIDERS["PINECONE"]
+        service_provider = SERVICE_PROVIDERS["QDRANT"]
         extra_attributes = baggage.get_baggage(LANGTRACE_ADDITIONAL_SPAN_ATTRIBUTES_KEY)
 
         span_attributes = {
             "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "vectordb",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
-            "db.system": "pinecone",
+            "db.system": "qdrant",
             "db.operation": api["OPERATION"],
+            "db.query": json.dumps(kwargs.get("query")),
             **(extra_attributes if extra_attributes is not None else {}),
         }
 
         attributes = DatabaseSpanAttributes(**span_attributes)
 
         with tracer.start_as_current_span(api["METHOD"], kind=SpanKind.CLIENT) as span:
-
-            if span.is_recording():
-                set_span_attribute(span, "server.address", instance._config.host)
-                if method == "QUERY":
-                    set_query_input_attributes(span, kwargs)
+            collection_name = kwargs.get("collection_name") or args[0]
+            operation = api["OPERATION"]
+            set_span_attributes(span, "db.collection.name", collection_name)
+
+            if operation == "add":
+                _set_upload_attributes(span, args, kwargs, "documents")
+
+            elif operation == "upsert":
+                _set_upsert_attributes(span, args, kwargs)
+
+            elif operation in ["query", "discover", "recommend", "retrieve", "search"]:
+                _set_search_attributes(span, args, kwargs)
+            elif operation in [
+                "query_batch",
+                "discover_batch",
+                "recommend_batch",
+                "search_batch",
+            ]:
+                _set_batch_search_attributes(span, args, kwargs, operation)
 
             for field, value in attributes.model_dump(by_alias=True).items():
                 if value is not None:
                     span.set_attribute(field, value)
             try:
                 # Attempt to call the original method
-                result = original_method(instance, *args, **kwargs)
-                if result:
-                    if span.is_recording():
-                        set_query_response_attributes(span, result)
+                result = wrapped(*args, **kwargs)
                 span.set_status(StatusCode.OK)
                 return result
             except Exception as err:
                 # Record the exception in the span
                 span.record_exception(err)
 
                 # Set the span status to indicate an error
                 span.set_status(Status(StatusCode.ERROR, str(err)))
 
                 # Reraise the exception to ensure it's not swallowed
                 raise
 
-    @silently_fail
-    def set_query_input_attributes(span, kwargs):
-        set_span_attribute(span, "db.query.top_k", kwargs.get("top_k"))
-        set_span_attribute(span, "db.query.namespace", kwargs.get("namespace"))
-        set_span_attribute(span, "db.query.id", kwargs.get("id"))
-        filter = (
-            json.dumps(kwargs.get("filter"))
-            if isinstance(kwargs.get("filter"), dict)
-            else kwargs.get("filter")
-        )
-        set_span_attribute(span, "db.query.filter", filter)
-        set_span_attribute(
-            span, "db.query.include_values", kwargs.get("include_values")
-        )
-        set_span_attribute(
-            span, "db.query.include_metadata", kwargs.get("include_metadata")
-        )
-
-    @silently_fail
-    def set_query_response_attributes(span, response):
-        matches = response.get("matches")
-
-        usage = response.get("usage")
-        for match in matches:
-            span.add_event(
-                name="db.query.match",
-                attributes={
-                    "db.query.match.id": match.get("id"),
-                    "db.query.match.score": match.get("score"),
-                    "db.query.match.metadata": match.get("metadata"),
-                    # "db.query.match.values": match.get("values"),
-                },
-            )
-
-        if "read_units" in usage:
-            set_span_attribute(
-                span, "db.query.usage.read_units", usage.get("read_units")
-            )
-
-        if "write_units" in usage:
-            set_span_attribute(
-                span, "db.query.usage.write_units", usage.get("write_units")
-            )
-
     return traced_method
+
+
+@silently_fail
+def _set_upsert_attributes(span, args, kwargs):
+    points = kwargs.get("points") or args[1]
+    if isinstance(points, list):
+        length = len(points)
+    else:
+        # In case of using Batch.
+        length = len(points.ids)
+    set_span_attributes(span, "db.upsert.points_count", length)
+
+
+@silently_fail
+def _set_upload_attributes(span, args, kwargs, field):
+    docs = kwargs.get(field) or args[0]
+    if isinstance(docs, list):
+        length = len(docs)
+    else:
+        # In case of using Batch.
+        length = len(docs.ids)
+
+    set_span_attributes(span, f"db.upload.{field}_count", length)
+
+
+@silently_fail
+def _set_search_attributes(span, args, kwargs):
+    limit = kwargs.get("limit") or 10
+    set_span_attributes(span, "db.query.top_k", limit)
+
+
+@silently_fail
+def _set_batch_search_attributes(span, args, kwargs, method):
+    requests = kwargs.get("requests") or []
+    set_span_attributes(span, f"db.{method}.requests_count", len(requests))
```

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/types/__init__.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     LLAMAINDEX = "llamaindex"
     CHROMADB = "chromadb"
     QDRANT = "qdrant"
     LANGCHAIN = "langchain"
     LANGCHAIN_CORE = "langchain_core"
     LANGCHAIN_COMMUNITY = "langchain_community"
     LANGGRAPH = "langgraph"
+    WEAVIATE = "weaviate"
 
     @staticmethod
     def from_string(value: str):
         try:
             return InstrumentationType[value.upper()]
         except KeyError:
             raise ValueError(f"Invalid value for InstrumentationType: {value}")
```

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/utils/llm.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/utils/llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,8 +61,7 @@
 
 
 def set_span_attributes(span, name, value):
     if value is not None:
         if value != "":
             span.set_attribute(name, value)
     return
-
```

### Comparing `langtrace_python_sdk-2.0.9/src/langtrace_python_sdk/utils/prompt_registry.py` & `langtrace_python_sdk-2.1.0/src/langtrace_python_sdk/utils/prompt_registry.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/conftest.py` & `langtrace_python_sdk-2.1.0/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/utils.py` & `langtrace_python_sdk-2.1.0/src/tests/utils.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/anthropic/conftest.py` & `langtrace_python_sdk-2.1.0/src/tests/anthropic/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/anthropic/test_anthropic.py` & `langtrace_python_sdk-2.1.0/src/tests/anthropic/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/anthropic/cassettes/test_anthropic.yaml` & `langtrace_python_sdk-2.1.0/src/tests/anthropic/cassettes/test_anthropic.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml` & `langtrace_python_sdk-2.1.0/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml` & `langtrace_python_sdk-2.1.0/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/chroma/test_chroma.py` & `langtrace_python_sdk-2.1.0/src/tests/chroma/test_chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/cohere/conftest.py` & `langtrace_python_sdk-2.1.0/src/tests/cohere/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/cohere/test_cohere_chat.py` & `langtrace_python_sdk-2.1.0/src/tests/cohere/test_cohere_chat.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/cohere/test_cohere_embed.py` & `langtrace_python_sdk-2.1.0/src/tests/cohere/test_cohere_embed.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/cohere/test_cohere_rerank.py` & `langtrace_python_sdk-2.1.0/src/tests/cohere/test_cohere_rerank.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/cohere/cassettes/test_cohere_chat.yaml` & `langtrace_python_sdk-2.1.0/src/tests/cohere/cassettes/test_cohere_chat.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -13,79 +13,77 @@
       connection:
       - keep-alive
       content-length:
       - '370'
       content-type:
       - application/json
       host:
-      - api.cohere.ai
+      - api.cohere.com
       user-agent:
       - python-httpx/0.27.0
       x-fern-language:
       - Python
       x-fern-sdk-name:
       - cohere
       x-fern-sdk-version:
-      - 5.3.2
+      - 5.5.3
     method: POST
-    uri: https://api.cohere.ai/v1/chat
+    uri: https://api.cohere.com/v1/chat
   response:
     body:
-      string: '{"response_id":"27cf0e2e-b4d5-427b-9866-d108307022de","text":"Argh,
+      string: '{"response_id":"6b2a2c29-2cd4-4e79-a05a-db8a6019b757","text":"Argh,
         many years ago, a bold explorer named Isaac Newton sat beneath an apple tree
-        for many hours, contemplating the nature of the universe and the motions of
-        the heavenly bodies. He posited that all objects in the universe are attracted
-        to each other. Then one day, his theory was proven true when a juicy apple
-        fell from the tree and struck him on the head, inspiring his theory of gravity
-        and changing science forever.","generation_id":"2a7babaa-f1da-468f-9891-5171f137ba04","chat_history":[{"role":"USER","message":"Who
+        for many hours, contemplating the nature of the universe. Suddenly, an apple
+        fell from the sky, striking him on the head. This inspired him to devise a
+        theory about the forces that govern objects on Earth and altered our understanding
+        of the universe forevermore.","generation_id":"f3b5a0d7-409b-45a7-9324-5b89c944457e","chat_history":[{"role":"USER","message":"Who
         discovered gravity?"},{"role":"CHATBOT","message":"The man who is widely credited
         with discovering gravity is Sir Isaac Newton"},{"role":"USER","message":"Tell
         me a story in 3 sentences or less?"},{"role":"CHATBOT","message":"Argh, many
         years ago, a bold explorer named Isaac Newton sat beneath an apple tree for
-        many hours, contemplating the nature of the universe and the motions of the
-        heavenly bodies. He posited that all objects in the universe are attracted
-        to each other. Then one day, his theory was proven true when a juicy apple
-        fell from the tree and struck him on the head, inspiring his theory of gravity
-        and changing science forever."}],"finish_reason":"COMPLETE","meta":{"api_version":{"version":"1"},"billed_units":{"input_tokens":31,"output_tokens":85},"tokens":{"input_tokens":49,"output_tokens":85}},"documents":[]}'
+        many hours, contemplating the nature of the universe. Suddenly, an apple fell
+        from the sky, striking him on the head. This inspired him to devise a theory
+        about the forces that govern objects on Earth and altered our understanding
+        of the universe forevermore."}],"finish_reason":"COMPLETE","meta":{"api_version":{"version":"1"},"billed_units":{"input_tokens":31,"output_tokens":69},"tokens":{"input_tokens":49,"output_tokens":69}},"documents":[]}'
     headers:
       Alt-Svc:
       - h3=":443"; ma=2592000,h3-29=":443"; ma=2592000
       Via:
       - 1.1 google
       access-control-expose-headers:
       - X-Debug-Trace-ID
       cache-control:
       - no-cache, no-store, no-transform, must-revalidate, private, max-age=0
       content-length:
-      - '1420'
+      - '1270'
       content-type:
       - application/json
       date:
-      - Fri, 26 Apr 2024 13:51:11 GMT
+      - Fri, 24 May 2024 09:38:02 GMT
       expires:
       - Thu, 01 Jan 1970 00:00:00 UTC
       num_chars:
       - '220'
       num_tokens:
-      - '116'
+      - '100'
       pragma:
       - no-cache
       server:
       - envoy
       vary:
       - Origin
       x-accel-expires:
       - '0'
       x-debug-trace-id:
-      - 6e0f777a5f86c8b5453bf374fd3fadbd
+      - 68cf0a1a2924c2a2534e350092097d49
       x-endpoint-monthly-call-limit:
       - '1000'
       x-envoy-upstream-service-time:
-      - '3037'
+      - '2573'
       x-trial-endpoint-call-limit:
-      - '40'
+      - '10'
       x-trial-endpoint-call-remaining:
-      - '39'
+      - '9'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `langtrace_python_sdk-2.0.9/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml` & `langtrace_python_sdk-2.1.0/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -3,273 +3,211 @@
     body: '{"message": "Tell me a story in 3 sentences or less?", "stream": true,
       "model": "command", "preamble": "answer like a pirate", "chat_history": [{"role":
       "USER", "message": "Who discovered gravity?"}, {"role": "CHATBOT", "message":
       "The man who is widely credited with discovering gravity is Sir Isaac Newton"}],
       "connectors": [{"id": "web-search"}], "temperature": 0.1}'
     headers:
       accept:
-      - '*/*, text/event-stream, application/stream+json'
+      - '*/*'
       accept-encoding:
       - gzip, deflate
       connection:
       - keep-alive
       content-length:
       - '369'
       content-type:
       - application/json
       host:
-      - api.cohere.ai
+      - api.cohere.com
       user-agent:
       - python-httpx/0.27.0
       x-fern-language:
       - Python
       x-fern-sdk-name:
       - cohere
       x-fern-sdk-version:
-      - 5.3.2
+      - 5.5.3
     method: POST
-    uri: https://api.cohere.ai/v1/chat
+    uri: https://api.cohere.com/v1/chat
   response:
     body:
-      string: '{"is_finished":false,"event_type":"stream-start","generation_id":"1d521296-3008-42bf-8062-8b744d997ba0"}
+      string: '{"is_finished":false,"event_type":"stream-start","generation_id":"79644b13-2cc8-462e-93be-f03cc16aed9a"}
 
         {"is_finished":false,"event_type":"text-generation","text":"Ar"}
 
         {"is_finished":false,"event_type":"text-generation","text":"gh"}
 
         {"is_finished":false,"event_type":"text-generation","text":","}
 
-        {"is_finished":false,"event_type":"text-generation","text":" here"}
+        {"is_finished":false,"event_type":"text-generation","text":" many"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" be"}
+        {"is_finished":false,"event_type":"text-generation","text":" years"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" the"}
-
-        {"is_finished":false,"event_type":"text-generation","text":" story"}
-
-        {"is_finished":false,"event_type":"text-generation","text":" of"}
-
-        {"is_finished":false,"event_type":"text-generation","text":" Gold"}
-
-        {"is_finished":false,"event_type":"text-generation","text":"il"}
-
-        {"is_finished":false,"event_type":"text-generation","text":"ocks"}
-
-        {"is_finished":false,"event_type":"text-generation","text":" and"}
-
-        {"is_finished":false,"event_type":"text-generation","text":" the"}
-
-        {"is_finished":false,"event_type":"text-generation","text":" Three"}
-
-        {"is_finished":false,"event_type":"text-generation","text":" Bears"}
-
-        {"is_finished":false,"event_type":"text-generation","text":" told"}
-
-        {"is_finished":false,"event_type":"text-generation","text":" in"}
-
-        {"is_finished":false,"event_type":"text-generation","text":" three"}
-
-        {"is_finished":false,"event_type":"text-generation","text":" sentences"}
-
-        {"is_finished":false,"event_type":"text-generation","text":" or"}
-
-        {"is_finished":false,"event_type":"text-generation","text":" less"}
-
-        {"is_finished":false,"event_type":"text-generation","text":":"}
-
-        {"is_finished":false,"event_type":"text-generation","text":"\n\nOnce"}
-
-        {"is_finished":false,"event_type":"text-generation","text":" upon"}
-
-        {"is_finished":false,"event_type":"text-generation","text":" a"}
-
-        {"is_finished":false,"event_type":"text-generation","text":" time"}
+        {"is_finished":false,"event_type":"text-generation","text":" ago"}
 
         {"is_finished":false,"event_type":"text-generation","text":","}
 
         {"is_finished":false,"event_type":"text-generation","text":" a"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" little"}
-
-        {"is_finished":false,"event_type":"text-generation","text":" girl"}
+        {"is_finished":false,"event_type":"text-generation","text":" man"}
 
         {"is_finished":false,"event_type":"text-generation","text":" named"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" Gold"}
-
-        {"is_finished":false,"event_type":"text-generation","text":"il"}
-
-        {"is_finished":false,"event_type":"text-generation","text":"ocks"}
+        {"is_finished":false,"event_type":"text-generation","text":" Isaac"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" stumbled"}
+        {"is_finished":false,"event_type":"text-generation","text":" Newton"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" into"}
+        {"is_finished":false,"event_type":"text-generation","text":" sat"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" the"}
-
-        {"is_finished":false,"event_type":"text-generation","text":" home"}
+        {"is_finished":false,"event_type":"text-generation","text":" beneath"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" of"}
+        {"is_finished":false,"event_type":"text-generation","text":" an"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" three"}
+        {"is_finished":false,"event_type":"text-generation","text":" apple"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" bears"}
+        {"is_finished":false,"event_type":"text-generation","text":" tree"}
 
         {"is_finished":false,"event_type":"text-generation","text":","}
 
-        {"is_finished":false,"event_type":"text-generation","text":" she"}
-
-        {"is_finished":false,"event_type":"text-generation","text":" ate"}
+        {"is_finished":false,"event_type":"text-generation","text":" observing"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" their"}
+        {"is_finished":false,"event_type":"text-generation","text":" an"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" food"}
+        {"is_finished":false,"event_type":"text-generation","text":" apple"}
 
-        {"is_finished":false,"event_type":"text-generation","text":","}
-
-        {"is_finished":false,"event_type":"text-generation","text":" broke"}
+        {"is_finished":false,"event_type":"text-generation","text":" fall"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" their"}
+        {"is_finished":false,"event_type":"text-generation","text":" to"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" chairs"}
-
-        {"is_finished":false,"event_type":"text-generation","text":","}
-
-        {"is_finished":false,"event_type":"text-generation","text":" and"}
-
-        {"is_finished":false,"event_type":"text-generation","text":" slept"}
-
-        {"is_finished":false,"event_type":"text-generation","text":" in"}
-
-        {"is_finished":false,"event_type":"text-generation","text":" their"}
+        {"is_finished":false,"event_type":"text-generation","text":" the"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" beds"}
+        {"is_finished":false,"event_type":"text-generation","text":" ground"}
 
         {"is_finished":false,"event_type":"text-generation","text":"."}
 
-        {"is_finished":false,"event_type":"text-generation","text":" When"}
+        {"is_finished":false,"event_type":"text-generation","text":" This"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" the"}
+        {"is_finished":false,"event_type":"text-generation","text":" inspired"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" three"}
+        {"is_finished":false,"event_type":"text-generation","text":" him"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" bears"}
+        {"is_finished":false,"event_type":"text-generation","text":" to"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" returned"}
+        {"is_finished":false,"event_type":"text-generation","text":" ponder"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" they"}
-
-        {"is_finished":false,"event_type":"text-generation","text":" were"}
-
-        {"is_finished":false,"event_type":"text-generation","text":" outraged"}
+        {"is_finished":false,"event_type":"text-generation","text":" upon"}
 
-        {"is_finished":false,"event_type":"text-generation","text":","}
+        {"is_finished":false,"event_type":"text-generation","text":" the"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" but"}
+        {"is_finished":false,"event_type":"text-generation","text":" concept"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" Gold"}
+        {"is_finished":false,"event_type":"text-generation","text":" of"}
 
-        {"is_finished":false,"event_type":"text-generation","text":"il"}
+        {"is_finished":false,"event_type":"text-generation","text":" gravity"}
 
-        {"is_finished":false,"event_type":"text-generation","text":"ocks"}
+        {"is_finished":false,"event_type":"text-generation","text":" and"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" had"}
+        {"is_finished":false,"event_type":"text-generation","text":" eventually"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" disappeared"}
+        {"is_finished":false,"event_type":"text-generation","text":" formulated"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" -"}
+        {"is_finished":false,"event_type":"text-generation","text":" his"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" she"}
+        {"is_finished":false,"event_type":"text-generation","text":" theories"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" had"}
+        {"is_finished":false,"event_type":"text-generation","text":" on"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" run"}
+        {"is_finished":false,"event_type":"text-generation","text":" the"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" away"}
+        {"is_finished":false,"event_type":"text-generation","text":" matter"}
 
         {"is_finished":false,"event_type":"text-generation","text":"."}
 
-        {"is_finished":false,"event_type":"text-generation","text":"\n\nAr"}
+        {"is_finished":false,"event_type":"text-generation","text":" Ar"}
 
         {"is_finished":false,"event_type":"text-generation","text":"gh"}
 
         {"is_finished":false,"event_type":"text-generation","text":","}
 
-        {"is_finished":false,"event_type":"text-generation","text":" that"}
+        {"is_finished":false,"event_type":"text-generation","text":" thus"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" be"}
+        {"is_finished":false,"event_type":"text-generation","text":" began"}
 
         {"is_finished":false,"event_type":"text-generation","text":" the"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" end"}
+        {"is_finished":false,"event_type":"text-generation","text":" world"}
+
+        {"is_finished":false,"event_type":"text-generation","text":"''s"}
+
+        {"is_finished":false,"event_type":"text-generation","text":" understanding"}
 
         {"is_finished":false,"event_type":"text-generation","text":" of"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" the"}
+        {"is_finished":false,"event_type":"text-generation","text":" gravity"}
+
+        {"is_finished":false,"event_type":"text-generation","text":","}
+
+        {"is_finished":false,"event_type":"text-generation","text":" thanks"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" story"}
+        {"is_finished":false,"event_type":"text-generation","text":" to"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" me"}
+        {"is_finished":false,"event_type":"text-generation","text":" this"}
 
-        {"is_finished":false,"event_type":"text-generation","text":" heart"}
+        {"is_finished":false,"event_type":"text-generation","text":" curious"}
 
-        {"is_finished":false,"event_type":"text-generation","text":"ies"}
+        {"is_finished":false,"event_type":"text-generation","text":" chap"}
 
         {"is_finished":false,"event_type":"text-generation","text":"!"}
 
-        {"is_finished":true,"event_type":"stream-end","response":{"response_id":"86b73a20-0cfa-414b-b148-e7857669ef3e","text":"Argh,
-        here be the story of Goldilocks and the Three Bears told in three sentences
-        or less:\n\nOnce upon a time, a little girl named Goldilocks stumbled into
-        the home of three bears, she ate their food, broke their chairs, and slept
-        in their beds. When the three bears returned they were outraged, but Goldilocks
-        had disappeared - she had run away.\n\nArgh, that be the end of the story
-        me hearties!","generation_id":"1d521296-3008-42bf-8062-8b744d997ba0","chat_history":[{"role":"USER","message":"Who
+        {"is_finished":true,"event_type":"stream-end","response":{"response_id":"7fdfb159-de9d-4cef-856b-cb2b801668db","text":"Argh,
+        many years ago, a man named Isaac Newton sat beneath an apple tree, observing
+        an apple fall to the ground. This inspired him to ponder upon the concept
+        of gravity and eventually formulated his theories on the matter. Argh, thus
+        began the world''s understanding of gravity, thanks to this curious chap!","generation_id":"79644b13-2cc8-462e-93be-f03cc16aed9a","chat_history":[{"role":"USER","message":"Who
         discovered gravity?"},{"role":"CHATBOT","message":"The man who is widely credited
         with discovering gravity is Sir Isaac Newton"},{"role":"USER","message":"Tell
-        me a story in 3 sentences or less?"},{"role":"CHATBOT","message":"Argh, here
-        be the story of Goldilocks and the Three Bears told in three sentences or
-        less:\n\nOnce upon a time, a little girl named Goldilocks stumbled into the
-        home of three bears, she ate their food, broke their chairs, and slept in
-        their beds. When the three bears returned they were outraged, but Goldilocks
-        had disappeared - she had run away.\n\nArgh, that be the end of the story
-        me hearties!"}],"finish_reason":"COMPLETE","meta":{"api_version":{"version":"1"},"billed_units":{"input_tokens":31,"output_tokens":96},"tokens":{"input_tokens":49,"output_tokens":96}},"documents":[]},"finish_reason":"COMPLETE"}
+        me a story in 3 sentences or less?"},{"role":"CHATBOT","message":"Argh, many
+        years ago, a man named Isaac Newton sat beneath an apple tree, observing an
+        apple fall to the ground. This inspired him to ponder upon the concept of
+        gravity and eventually formulated his theories on the matter. Argh, thus began
+        the world''s understanding of gravity, thanks to this curious chap!"}],"finish_reason":"COMPLETE","meta":{"api_version":{"version":"1"},"billed_units":{"input_tokens":31,"output_tokens":63},"tokens":{"input_tokens":49,"output_tokens":63}},"documents":[]},"finish_reason":"COMPLETE"}
 
         '
     headers:
       Alt-Svc:
       - h3=":443"; ma=2592000,h3-29=":443"; ma=2592000
       Via:
       - 1.1 google
       access-control-expose-headers:
       - X-Debug-Trace-ID
       cache-control:
       - no-cache, no-store, no-transform, must-revalidate, private, max-age=0
       content-type:
       - application/stream+json
       date:
-      - Fri, 26 Apr 2024 13:59:03 GMT
+      - Fri, 24 May 2024 09:38:03 GMT
       expires:
       - Thu, 01 Jan 1970 00:00:00 UTC
       pragma:
       - no-cache
       server:
       - envoy
       transfer-encoding:
       - chunked
       vary:
       - Origin
       x-accel-expires:
       - '0'
       x-debug-trace-id:
-      - 2803337aa161b7c4f034921bb2bb1444
+      - 7a2dadc471ebb9e4e0050988183969e1
       x-endpoint-monthly-call-limit:
       - '1000'
       x-envoy-upstream-service-time:
-      - '66'
+      - '85'
       x-trial-endpoint-call-limit:
-      - '40'
+      - '10'
       x-trial-endpoint-call-remaining:
-      - '39'
+      - '8'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `langtrace_python_sdk-2.0.9/src/tests/cohere/cassettes/test_cohere_embed.yaml` & `langtrace_python_sdk-2.1.0/src/tests/cohere/cassettes/test_cohere_embed.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -10,41 +10,41 @@
       connection:
       - keep-alive
       content-length:
       - '94'
       content-type:
       - application/json
       host:
-      - api.cohere.ai
+      - api.cohere.com
       user-agent:
       - python-httpx/0.27.0
       x-fern-language:
       - Python
       x-fern-sdk-name:
       - cohere
       x-fern-sdk-version:
-      - 5.3.2
+      - 5.5.3
     method: POST
-    uri: https://api.cohere.ai/v1/embed
+    uri: https://api.cohere.com/v1/embed
   response:
     body:
-      string: '{"id":"2c1ede34-c4c7-4cdd-a74e-ce035af81e20","texts":["hello","goodbye"],"embeddings":[[0.016296387,-0.008354187,-0.04699707,-0.07104492,0.00013196468,-0.014892578,-0.018661499,0.019134521,0.008476257,0.04159546,-0.036895752,-0.00048303604,0.06414795,-0.036346436,0.045806885,-0.03125,0.03793335,0.048583984,0.0062179565,0.0071144104,-0.020935059,0.04196167,-0.039398193,0.03463745,0.051879883,0.030838013,-0.0048103333,-0.00036287308,-0.017944336,-0.039611816,0.013389587,0.0044021606,0.018951416,0.020767212,-0.0025997162,0.0904541,-0.0121154785,-0.026184082,0.012413025,0.004119873,0.030654907,-0.030792236,-0.041107178,-0.02368164,-0.043304443,-0.00077438354,-0.017074585,-0.019729614,0.078125,-0.031585693,0.020217896,-0.01524353,0.017471313,-0.0008010864,-0.03717041,0.011062622,-0.072143555,-0.013175964,0.01058197,0.030853271,0.044799805,0.0045928955,0.03253174,0.047698975,-0.0039024353,-0.01965332,0.024475098,-0.013755798,0.018951416,-0.015487671,0.015594482,0.00096321106,-0.006450653,-0.04748535,-0.021972656,0.06323242,-0.009498596,0.014297485,0.0038471222,-0.023117065,-0.02180481,-0.01928711,-0.08758545,-0.04852295,0.029510498,0.011276245,-0.013504028,-0.009391785,-0.0064468384,0.010978699,-0.014404297,0.053741455,0.046569824,0.00042700768,-0.037719727,0.011985779,-0.009643555,0.0067749023,0.008071899,0.018829346,-0.05419922,-0.020950317,-0.02659607,-0.028869629,-0.015716553,0.022705078,-0.0046958923,0.02192688,0.032440186,0.048034668,-0.006843567,0.045074463,-0.02293396,0.010238647,-0.04534912,0.01638794,-0.00680542,0.0038871765,-0.032836914,0.051361084,0.0395813,0.032928467,-0.00843811,0.007858276,-0.040802002,-0.008346558,-0.013252258,-0.046173096,0.051727295,-0.027175903,-0.011497498,0.04940796,-0.095214844,-0.0345459,-0.021453857,0.0051002502,-0.01725769,-0.045196533,-0.0016956329,0.021575928,0.07720947,-0.00094270706,0.020904541,0.05001831,-0.033111572,0.032287598,-0.0052833557,-0.00007402897,0.035125732,0.019424438,-0.06665039,-0.02557373,0.010887146,0.05807495,0.015022278,0.0657959,-0.015350342,0.008468628,-0.017944336,0.029388428,-0.005126953,0.015914917,0.051879883,-0.015975952,-0.039031982,-0.012374878,0.0032424927,0.0008568764,0.014579773,0.021530151,-0.0061912537,0.028717041,0.046844482,0.032836914,0.0071372986,-0.023406982,-0.03717041,0.016723633,0.03994751,0.025390625,0.03427124,-0.01914978,-0.026000977,0.07342529,-0.03213501,-0.058258057,0.029144287,0.001042366,0.030517578,0.011474609,0.058410645,0.005027771,-0.038635254,-0.015029907,-0.015655518,-0.03918457,-0.016342163,-0.020858765,-0.0043907166,0.03857422,0.007423401,-0.0473938,0.04257202,-0.043823242,-0.03842163,-0.033691406,-0.010925293,0.012260437,0.0009822845,0.0058937073,-0.008644104,-0.031585693,0.0055618286,-0.06976318,-0.030578613,-0.038970947,-0.08880615,-0.00315094,0.00020766258,0.04058838,0.0028266907,-0.0018129349,-0.01625061,-0.022277832,-0.008956909,-0.009292603,-0.040771484,-0.008705139,-0.065979004,-0.010414124,-0.0152282715,0.033447266,-0.033599854,-0.008049011,-0.020828247,0.0053901672,0.0002875328,0.037078857,0.015159607,-0.0016326904,0.012397766,0.0026817322,-0.032196045,-0.0079422,0.03567505,-0.0010242462,0.03652954,-0.0035171509,0.01802063,0.026641846,0.0107421875,-0.021942139,0.035095215,-0.0236969,-0.015975952,0.039215088,0.0038166046,0.020462036,-0.039764404,0.035888672,-0.038604736,-0.008621216,-0.012619019,-0.014602661,-0.036102295,-0.02368164,-0.0121536255,-0.0054512024,-0.015701294,-0.016296387,0.016433716,-0.005672455,-0.019332886,0.00025129318,0.0803833,0.04248047,-0.05960083,-0.009147644,-0.0021247864,0.012481689,-0.015129089,-0.021133423,-0.01878357,0.0027332306,0.036956787,-0.0053253174,-0.0007238388,0.016983032,-0.0034694672,0.059387207,0.076660156,0.015312195,-0.015823364,0.02456665,0.012901306,0.020126343,-0.032440186,0.011291504,-0.001876831,-0.052215576,0.004634857,0.036956787,0.006164551,-0.023422241,-0.025619507,0.024261475,0.023849487,0.015007019,0.020050049,-0.044067383,0.030029297,0.021377563,0.011657715,0.017196655,-0.032318115,-0.031555176,-0.00982666,-0.0039787292,-0.079589844,-0.006416321,0.00844574,-0.007434845,-0.045013428,-0.02557373,-0.01537323,0.027633667,-0.076538086,-0.0025749207,-0.05279541,0.029373169,0.047912598,0.00083875656,-0.01234436,-0.017059326,0.01159668,0.014228821,0.029571533,-0.055114746,0.006389618,0.028869629,0.09375,-0.014251709,0.029418945,0.007633209,0.010848999,-0.004055023,-0.02116394,0.007194519,-0.0062217712,-0.01209259,0.024749756,-0.037506104,-0.029510498,-0.028442383,0.03189087,0.0008239746,0.007419586,-0.016723633,0.06964111,-0.07232666,0.022201538,-0.019882202,-0.0385437,-0.022567749,0.010353088,-0.027755737,-0.006713867,-0.023406982,-0.025054932,-0.013076782,0.015808105,-0.0073165894,0.02949524,-0.036499023,-0.07287598,-0.01876831,-0.02709961,-0.06567383,0.050567627,0.004047394,0.030471802,0.025405884,0.046783447,0.01763916,0.053466797,0.049072266,-0.015197754,0.0013389587,0.049591064,0.006965637,-0.00014233589,0.01335907,-0.04675293,-0.026733398,0.03024292,0.0012464523,-0.037200928,0.030166626,-0.08544922,-0.013893127,-0.014823914,0.0014219284,-0.023620605,-0.0010480881,-0.072387695,0.057922363,-0.04067993,-0.025299072,0.020446777,0.06451416,0.007205963,0.015838623,-0.008674622,0.0002270937,-0.026321411,0.027130127,-0.01828003,-0.011482239,0.03463745,0.00724411,-0.010406494,0.025268555,-0.023651123,0.04034424,-0.036834717,0.05014038,-0.026184082,0.036376953,0.03253174,-0.01828003,-0.023376465,-0.034576416,-0.00598526,-0.023239136,-0.032409668,0.07672119,-0.038604736,0.056884766,-0.012550354,-0.03778076,-0.013061523,0.017105103,0.010482788,-0.005077362,-0.010719299,-0.018661499,0.019760132,0.022018433,-0.058746338,0.03564453,-0.0892334,0.025421143,-0.015716553,0.07910156,-0.009361267,0.016921997,0.048736572,0.035247803,0.01864624,0.011413574,0.018295288,0.00052690506,-0.07122803,-0.01890564,-0.017669678,0.027694702,0.0152282715,0.006511688,-0.045837402,-0.009765625,0.013877869,-0.0146102905,0.033294678,-0.0019874573,0.023040771,0.025619507,-0.015823364,-0.020858765,-0.023529053,0.0070152283,-0.0647583,0.036224365,0.0023403168,-0.062286377,-0.036315918,0.021209717,-0.037353516,-0.03656006,0.01889038,0.023239136,0.011764526,0.005970001,0.049346924,-0.006893158,-0.015068054,-0.0008716583,-0.0034999847,0.04034424,0.017913818,-0.06707764,-0.07531738,0.00042319298,-0.00680542,-0.0023174286,0.04425049,-0.05105591,-0.016967773,0.020507812,0.038604736,0.029846191,0.04309082,-0.00084733963,-0.008911133,0.0082092285,-0.0050239563,0.05038452,0.014595032,0.015182495,0.007247925,-0.04046631,-0.011169434,-0.010292053,0.068603516,0.02470398,-0.0023403168,0.005996704,-0.0010709763,0.008178711,-0.029205322,-0.025253296,0.05822754,0.04269409,0.059295654,-0.0011911392,-0.031311035,0.023712158,-0.037506104,0.004589081,0.014923096,-0.019866943,-0.019180298,-0.0020999908,-0.008972168,0.01348114,0.014801025,-0.02645874,0.019897461,0.081970215,-0.05822754,0.09399414,0.001209259,-0.050750732,0.062316895,-0.014892578,-0.019104004,-0.036987305,-0.040618896,-0.008163452,-0.0035247803,0.06774902,-0.001420021,-0.0013103485,-0.031799316,-0.0023651123,0.012298584,0.003583908,0.050964355,-0.01802063,-0.007091522,0.01448822,-0.016159058,-0.019439697,-0.022491455,-0.036346436,-0.03491211,-0.0032920837,0.003528595,-0.0016469955,0.01612854,-0.003709793,0.012840271,0.0043182373,-0.030456543,0.007369995,0.0039787292,0.036499023,0.021362305,0.00062942505,0.0047073364,0.026382446,-0.0020542145,-0.038757324,-0.00095272064,0.0019435883,0.007232666,-0.0031471252,0.019943237,-0.062042236,0.010826111,0.0026607513,-0.04727173,0.020126343,0.046417236,-0.03881836,0.011222839,0.011428833,-0.056396484,0.010879517,-0.011772156,-0.0038414001,0.010246277,-0.020141602,-0.011169434,0.006916046,-0.022659302,0.010299683,0.046966553,0.0234375,-0.0016288757,-0.03262329,-0.01689148,-0.00031924248,0.028152466,0.004234314,0.03878784,-0.03579712,0.007457733,-0.0036907196,0.0073051453,-0.00028276443,-0.0067100525,0.003206253,-0.0021209717,-0.05960083,0.024337769,0.076171875,-0.012062073,-0.0032787323,-0.08380127,0.024917603,0.019073486,-0.012031555,-0.03237915,-0.0042686462,-0.01525116,-0.0158844,-0.0014514923,-0.024429321,-0.028442383,0.020843506,0.007133484,0.024230957,0.0002002716,-0.005466461,-0.0032367706,0.012718201,0.032806396,0.062042236,-0.040283203,-0.025497437,0.045013428,0.054473877,-0.033599854,-0.0039482117,0.02268982,-0.0012645721,0.045166016,0.0501709,-0.0022602081,0.019897461,0.007926941,0.017364502,0.011650085,-0.042510986,-0.059448242,0.030014038,0.039611816,0.015571594,0.04031372,-0.0006723404,-0.03353882,-0.05569458,0.040283203,0.019058228,-0.032592773,0.004470825,0.06359863,0.029693604,0.01826477,-0.0104522705,-0.043945312,-0.01802063,0.0075187683,-0.02456665,0.02798462,0.0047340393,-0.017623901,-0.014335632,-0.04550171,-0.0039711,0.023864746,-0.015281677,0.055755615,-0.04864502,0.033599854,0.024810791,-0.03048706,-0.043121338,0.011291504,0.024932861,-0.0020275116,0.032287598,-0.0234375,0.006942749,-0.007221222,-0.03869629,-0.03765869,-0.03475952,-0.046936035,0.03012085,-0.021362305,-0.023452759,0.051239014,-0.009925842,0.04925537,-0.00944519,-0.040008545,-0.019485474,-0.00022566319,-0.017028809,0.03277588,0.0066375732,-0.013328552,0.01864624,-0.011726379,0.023849487,0.04006958,0.03793335,0.060821533,0.005504608,-0.0395813,-0.010131836,0.046539307,0.030136108,0.002231598,0.042236328,0.014755249,0.047058105,-0.017318726,0.008598328,0.01966858,0.0064430237,0.03616333,-0.011985779,-0.003446579,-0.06616211,-0.0657959,0.014137268,0.044677734,-0.03515625,-0.05215454,-0.012710571,0.0047416687,0.05368042,0.013900757,0.05001831,0.027709961,0.02557373,-0.025512695,0.0031032562,0.072143555,0.018829346,0.0073928833,0.009269714,-0.011299133,0.0048828125,0.014808655,-0.0184021,-0.00089359283,-0.0015716553,-0.012863159,0.0074386597,-0.020767212,0.02204895,-0.027404785,-0.021972656,0.02494812,0.044006348,-0.011581421,0.06298828,0.009010315,0.03842163,-0.00005555153,0.06774902,0.036254883,-0.016311646,-0.000004887581,0.0057373047,0.03704834,-0.041503906,0.0074043274,-0.012290955,-0.020263672,-0.0057792664,-0.025878906,-0.021652222,-0.008079529,0.022613525,-0.012069702,0.050079346,-0.004283905,-0.021118164,-0.010559082,-0.0041160583,-0.00026345253,-0.01260376,0.050628662,-0.03137207,0.027526855,-0.052642822,-0.0046463013,0.04937744,-0.0017156601,0.014625549,-0.022476196,0.02571106,0.043884277,-0.016952515,-0.021011353,0.056396484,0.056762695,0.013473511,-0.02357483,0.043792725,0.032470703,-0.052612305,-0.017837524,-0.000067055225,0.039276123,-0.012283325,-0.0029888153,-0.024719238,0.012870789,-0.032287598,0.028839111,0.008056641,0.011100769,-0.034210205,0.028198242,0.01940918,0.029052734,0.030303955,0.03475952,-0.03982544,0.026870728,0.02079773,0.03012085,-0.044281006,0.006462097,-0.008705139,-0.024734497,0.02458191,-0.050201416,-0.028778076,0.036956787,0.025634766,-0.025650024,0.020629883,-0.04385376,0.009536743,-0.0027256012,0.031158447,0.008712769,-0.039855957,-0.018249512,-0.011268616,0.009689331,-0.032073975,0.023010254,0.04925537,0.013168335,0.02734375,0.031707764,-0.024032593,-0.010604858,-0.00258255,0.0054092407,0.033569336,0.0068359375,0.019882202,0.018096924,-0.05392456,-0.0030059814,-0.01374054,-0.008483887,0.016494751,-0.015487671,0.016143799,-0.028198242,-0.016326904,-0.013160706,-0.046905518,0.026428223,-0.02420044,-0.022262573,0.041748047,0.05557251,-0.0044059753,-0.030960083,-0.023544312,0.0103302,-0.013534546,-0.016830444,0.028167725,0.0061950684,0.02178955,-0.06945801,-0.040039062,-0.0024642944,-0.06359863,-0.020812988,0.029006958,0.0072364807,-0.028747559,-0.057891846,0.022155762,-0.035369873,-0.025909424,-0.04095459,0.0019893646,-0.0038146973,-0.030639648,-0.038970947,-0.0026626587,-0.0047454834,-0.014816284,0.008575439,-0.032165527,-0.011062622,0.003622055,-0.0129852295,-0.0007658005,-0.009902954,0.03704834,-0.02456665,0.020385742,0.0019044876,-0.008552551,-0.028137207,-0.006500244,0.017227173,-0.0077285767,-0.05496216,0.038024902,-0.0335083,0.047668457,-0.02998352,-0.0395813,-0.0068359375,-0.024627686,-0.005756378,0.025863647,0.032104492,-0.029022217,-0.08685303,-0.014724731,-0.035583496,0.024002075,0.008422852,0.012931824,-0.0055656433,-0.013748169,-0.021530151,-0.034332275,-0.008766174,-0.025222778,0.019836426,-0.011619568,-0.037963867,0.013519287,-0.035736084,0.049102783,-0.011398315,0.050598145,-0.066833496,0.080566406,-0.061553955,-0.041778564,0.01864624,0.014907837,-0.010482788,0.035217285,-0.0473938,-0.031951904,0.052886963,-0.022109985,0.031677246,-0.01977539,0.08282471,0.012901306,-0.009490967,0.0030956268,0.023895264,0.012611389,-0.0011844635,-0.007633209,0.019195557,-0.05404663,0.006187439,-0.06762695,-0.049468994,0.028121948,-0.004032135,-0.043151855,0.028121948,-0.0058555603,0.019454956,0.0028438568,-0.0036354065,-0.015411377,-0.026535034,0.03704834,-0.01802063,0.009765625],[0.04663086,-0.023239136,0.008163452,-0.03945923,-0.018051147,-0.011123657,0.0022335052,-0.0015516281,-0.002336502,0.031799316,-0.049591064,-0.049835205,0.019317627,-0.013328552,-0.01838684,-0.067871094,0.02671814,0.038085938,0.03265381,-0.0043907166,0.026321411,0.0070114136,-0.037628174,0.008026123,0.015525818,0.066589355,-0.018005371,-0.0017309189,-0.052368164,-0.055511475,-0.00504303,0.043029785,-0.013328552,0.08581543,-0.038269043,0.051971436,-0.04675293,0.038146973,0.05328369,-0.028762817,0.01625061,-0.008644104,-0.060150146,-0.0259552,-0.05432129,-0.00680542,-0.012649536,0.0025501251,0.060272217,-0.013168335,0.046691895,0.030395508,0.039733887,0.00044679642,-0.034240723,0.01828003,-0.047546387,-0.036499023,0.024505615,0.027374268,0.015197754,-0.003932953,0.03475952,0.013633728,0.020858765,-0.025344849,-0.056732178,0.008178711,0.043304443,0.014625549,-0.0020503998,-0.033569336,-0.00178051,-0.0446167,-0.045837402,0.089538574,0.00440979,0.03741455,0.0015287399,-0.035339355,0.017654419,-0.008956909,-0.035064697,-0.014251709,0.008331299,0.0077781677,0.0020999908,-0.021636963,-0.014625549,-0.0209198,-0.009429932,0.070617676,0.013923645,-0.025558472,-0.0519104,-0.0049552917,0.000998497,-0.01448822,-0.027175903,-0.04083252,-0.032043457,-0.0096588135,-0.047088623,-0.0012331009,-0.025878906,0.031799316,-0.023712158,0.015701294,0.017730713,0.062927246,0.009178162,-0.046295166,-0.014701843,-0.007751465,-0.021148682,0.033966064,-0.013664246,0.03945923,-0.02520752,0.08905029,-0.039520264,-0.012435913,-0.057403564,0.007068634,0.006061554,-0.040161133,-0.015548706,0.080078125,0.08862305,0.008003235,-0.048339844,0.037750244,-0.04498291,-0.065979004,-0.032470703,-0.03225708,0.004890442,-0.013023376,-0.020965576,0.035095215,0.035491943,-0.01486969,0.027023315,0.009552002,-0.01285553,0.044891357,0.00062322617,-0.030639648,0.024108887,0.0035648346,-0.06585693,-0.011070251,0.037506104,0.05697632,-0.027236938,0.03475952,0.0143585205,-0.014442444,-0.011405945,-0.013648987,-0.028625488,0.024902344,0.09387207,-0.012741089,-0.040985107,-0.018814087,0.0046920776,-0.017715454,0.013839722,0.0022621155,0.0024433136,-0.028366089,-0.0046310425,0.028717041,-0.00013160706,0.006690979,-0.053863525,0.03302002,0.040802002,0.03201294,0.032073975,-0.03125,-0.005241394,0.048828125,-0.016204834,-0.0014667511,-0.013572693,0.007949829,0.019744873,-0.004776001,-0.0022506714,0.033111572,0.00039958954,0.008369446,-0.021057129,-0.033935547,-0.03692627,0.0042762756,-0.030380249,-0.01876831,-0.023529053,0.004764557,0.026947021,-0.013267517,-0.023666382,0.0024929047,-0.017990112,0.035217285,0.0034389496,0.030380249,0.02015686,-0.013061523,-0.047790527,0.042633057,0.009559631,-0.03186035,-0.02796936,-0.0151901245,-0.0039482117,0.0345459,-0.018096924,0.012062073,-0.02180481,0.031402588,0.041412354,-0.052459717,0.006286621,-0.033203125,-0.0013237,-0.012466431,-0.041748047,0.027313232,-0.0284729,-0.05682373,-0.02809143,0.030899048,0.023773193,0.044677734,-0.0064353943,-0.0000064373016,0.011512756,0.0028190613,-0.041870117,-0.028182983,0.014595032,-0.0143966675,0.022949219,-0.004371643,0.01461792,0.0035171509,0.01398468,-0.04473877,0.04232788,-0.033599854,-0.000647068,0.034606934,0.006160736,-0.014640808,0.028137207,-0.02470398,0.0043563843,0.00039553642,-0.039886475,0.014251709,-0.035736084,-0.021347046,-0.029663086,-0.011688232,-0.038085938,-0.0034008026,0.029144287,-0.010948181,-0.024978638,0.009468079,0.093933105,0.014205933,-0.08569336,-0.011657715,0.02027893,0.0063095093,-0.0035533905,0.020446777,0.029968262,-0.002008438,0.03253174,0.029891968,0.019577026,-0.002922058,-0.009994507,0.029418945,0.049987793,0.046295166,-0.0072898865,0.019638062,0.042816162,0.0066108704,0.06591797,0.04714966,-0.026062012,-0.019470215,0.009979248,0.018081665,0.000009059906,-0.043060303,-0.0043907166,0.064331055,0.051605225,-0.0040893555,0.018081665,-0.024749756,-0.014915466,-0.048614502,0.023483276,0.013282776,-0.011741638,-0.036346436,-0.0076293945,0.023086548,-0.051849365,0.023223877,0.033721924,-0.003929138,-0.044647217,0.020019531,-0.029678345,-0.0031986237,0.030548096,-0.040161133,-0.020874023,0.028793335,0.037872314,0.011314392,-0.030838013,-0.051818848,-0.007774353,0.0070724487,0.02507019,-0.0112838745,0.014930725,0.010543823,0.085998535,0.019332886,0.0107803345,0.00014901161,0.001613617,-0.024993896,-0.04940796,0.010643005,0.04269409,-0.02571106,0.001124382,-0.018844604,-0.014953613,0.027786255,0.033447266,0.0038719177,0.011268616,0.004295349,0.028656006,-0.078063965,-0.012619019,-0.03527832,-0.061279297,0.0625,0.038116455,-0.008308411,-0.017913818,0.031311035,-0.018722534,0.0362854,-0.019363403,0.021362305,-0.0029010773,-0.030288696,-0.07293701,0.008544922,0.006755829,-0.068237305,0.0491333,0.016494751,-0.021621704,0.020980835,0.026443481,0.051879883,0.035583496,0.030548096,-0.03366089,-0.017532349,0.066101074,0.03930664,0.013633728,-0.008621216,0.031982422,-0.042388916,-0.00042247772,-0.020492554,0.04006958,0.052825928,-0.0044136047,-0.02243042,-0.04260254,0.02418518,-0.020584106,-0.0027770996,-0.05908203,0.026611328,-0.046051025,-0.03451538,0.017944336,0.054260254,0.019348145,0.0070114136,0.014205933,-0.019454956,-0.021514893,0.010383606,0.050109863,0.020584106,-0.031677246,-0.048187256,0.01449585,0.04650879,0.025222778,0.004135132,0.02017212,0.044311523,-0.03427124,-0.023757935,0.03479004,-0.012031555,-0.030380249,-0.021560669,-0.010375977,-0.05041504,-0.060821533,0.012283325,-0.026367188,0.061920166,0.026367188,-0.037078857,-0.015136719,0.033355713,-0.010055542,0.025314331,-0.027893066,-0.010032654,0.017684937,-0.00002783537,-0.061157227,0.030273438,-0.103759766,0.035583496,-0.028167725,0.07171631,-0.0211792,-0.013725281,0.04437256,0.041137695,0.027145386,0.032073975,0.008926392,-0.021560669,0.007381439,0.019165039,0.0012969971,-0.01928711,0.026672363,-0.01222229,-0.056365967,0.010398865,-0.02255249,0.00093221664,-0.009353638,0.016082764,0.022872925,0.025024414,-0.024459839,0.040618896,-0.049224854,-0.0035133362,-0.047698975,0.01727295,0.034057617,-0.004096985,-0.009361267,0.011291504,-0.010093689,-0.017990112,0.04107666,-0.058563232,-0.03387451,-0.046905518,0.015411377,-0.02003479,-0.010528564,-0.01689148,0.010391235,-0.040618896,0.029205322,-0.020492554,-0.082092285,0.0004811287,0.043518066,-0.044830322,0.020141602,-0.02319336,0.0024662018,0.012825012,0.04977417,0.06225586,0.027801514,0.005153656,0.04147339,0.0011873245,0.004486084,-0.02494812,0.061706543,0.012184143,-0.0027637482,-0.018447876,-0.008987427,-0.0362854,0.10205078,0.026138306,-0.056549072,0.015899658,0.04449463,-0.017837524,-0.0044898987,-0.04348755,0.06689453,0.008728027,0.047454834,0.03289795,-0.034851074,0.04675293,-0.058807373,0.03164673,0.01322937,-0.06958008,-0.042816162,-0.022918701,-0.019760132,0.008293152,0.02709961,-0.05822754,0.011459351,-0.0008597374,-0.01574707,0.027954102,-0.029785156,-0.03665161,0.017562866,-0.027297974,-0.024017334,-0.0423584,-0.039245605,0.0028457642,-0.0010719299,0.01763916,0.009902954,-0.023849487,-0.009399414,-0.016464233,0.045074463,-0.0056762695,0.04537964,-0.04397583,-0.025817871,0.037353516,-0.018737793,0.01084137,0.0038528442,-0.04547119,-0.024475098,-0.05545044,-0.005756378,0.008132935,0.014541626,-0.0020751953,0.03793335,-0.004421234,-0.037261963,-0.00818634,0.026733398,0.04776001,-0.012313843,0.0019369125,-0.0006084442,0.01335907,-0.033813477,-0.024459839,0.046783447,-0.006389618,-0.055999756,-0.059295654,0.008743286,-0.033966064,0.022537231,-0.018722534,-0.041259766,0.040039062,0.028747559,-0.03515625,0.0019016266,0.041778564,-0.0046539307,0.00014257431,0.011451721,0.016998291,0.00522995,-0.04837036,-0.024520874,0.025466919,-0.020706177,0.017608643,0.062042236,-0.0039596558,-0.021911621,-0.013893127,-0.0000885129,0.00075626373,0.03414917,0.011314392,0.018661499,-0.009719849,0.012748718,-0.026809692,-0.01436615,0.021469116,-0.036254883,0.00907135,-0.026016235,-0.01625061,0.030075073,0.011817932,-0.0038528442,-0.0028858185,-0.021820068,0.037475586,0.0115356445,-0.0077285767,-0.05328369,-0.051361084,0.040649414,-0.005958557,-0.02279663,0.01953125,-0.016937256,0.03781128,-0.0016212463,0.015098572,-0.01626587,0.0067443848,0.027175903,0.011459351,0.038513184,0.06222534,-0.0073547363,-0.010383606,0.0017681122,0.045043945,-0.044921875,-0.0104599,0.035858154,-0.008323669,0.0025901794,0.021514893,-0.010971069,0.016738892,0.0018157959,-0.0071258545,-0.029022217,-0.047027588,-0.02670288,0.029220581,-0.022750854,0.025054932,-0.008544922,0.006164551,-0.029052734,-0.031066895,0.06304932,-0.044647217,-0.017562866,-0.0068511963,0.06604004,0.039916992,-0.007041931,-0.02772522,-0.05795288,-0.022247314,-0.02810669,-0.03845215,0.045074463,-0.014060974,-0.016174316,0.046722412,-0.0006046295,-0.019500732,-0.025985718,0.032989502,0.028366089,0.0021324158,0.0020503998,0.051574707,0.009117126,-0.03112793,-0.006565094,0.019226074,0.009971619,-0.0064735413,-0.017700195,0.0024414062,-0.0008454323,-0.04071045,-0.034820557,-0.031066895,-0.044677734,0.039398193,-0.012580872,-0.06549072,0.027130127,-0.0309906,0.023727417,-0.019760132,0.0066490173,-0.004798889,0.009155273,-0.009902954,0.047576904,0.005466461,0.001537323,0.014862061,-0.0027828217,-0.0079956055,0.043182373,0.0051841736,0.034484863,-0.028015137,-0.012870789,-0.019714355,0.036071777,0.015716553,-0.016860962,0.0034122467,-0.014289856,0.039031982,0.017730713,-0.013549805,0.046691895,0.022094727,0.04647827,0.008033752,0.028747559,-0.030288696,-0.018722534,-0.015113831,0.051971436,-0.040893555,-0.039978027,-0.0042266846,-0.008346558,0.059814453,0.0011167526,0.056030273,-0.08166504,-0.059631348,-0.015731812,0.009529114,0.025756836,0.022232056,-0.0049819946,0.021118164,-0.020446777,0.0032253265,0.017105103,-0.030944824,0.010154724,-0.021881104,-0.018081665,0.029342651,0.024047852,0.017700195,-0.02268982,0.018356323,0.026519775,0.032226562,-0.004711151,0.018753052,0.007789612,0.033172607,-0.034423828,0.035247803,-0.019729614,-0.021194458,0.0071411133,-0.014549255,-0.0073165894,-0.05596924,0.015060425,-0.014305115,-0.030090332,0.001613617,-0.026809692,-0.02571106,-0.0041275024,0.027389526,-0.0059509277,0.0473938,-0.0002002716,0.00037145615,0.0031642914,-0.0044441223,0.0023765564,0.0121154785,0.04260254,-0.035736084,0.019424438,-0.005558014,0.0038166046,0.03717041,-0.0031261444,0.0446167,0.015098572,-0.0022087097,0.0385437,0.024505615,-0.03353882,-0.028533936,0.06048584,-0.019332886,-0.046539307,0.007232666,-0.031585693,0.02168274,0.0046195984,-0.041412354,0.032592773,0.056671143,0.031173706,-0.011398315,0.033416748,0.01802063,-0.0259552,-0.0028705597,0.046539307,-0.040008545,0.022567749,0.020980835,0.024383545,0.02861023,0.010574341,-0.008300781,0.024261475,0.030319214,-0.011238098,-0.030197144,0.013389587,0.010879517,-0.031311035,0.035308838,-0.014755249,0.01612854,0.05722046,-0.019470215,-0.014045715,0.022842407,-0.085998535,0.017166138,0.011474609,0.018325806,0.010398865,0.00434494,-0.013153076,0.025482178,0.007217407,-0.0017223358,0.041046143,0.036895752,-0.028656006,-0.008026123,0.026550293,-0.0146102905,0.0053215027,-0.057037354,0.008743286,0.018066406,0.0025310516,-0.0035171509,-0.02230835,-0.018218994,0.0069618225,-0.006111145,0.017532349,0.034210205,-0.040496826,0.031433105,-0.006587982,-0.031097412,-0.0154418945,-0.009414673,0.006729126,0.004711151,0.00920105,0.0025501251,-0.0016479492,-0.0107803345,-0.070129395,-0.046203613,0.06616211,-0.019622803,-0.06298828,-0.022628784,0.04156494,0.026672363,-0.11505127,-0.080200195,-0.0491333,-0.03744507,-0.0178833,0.016326904,0.03201294,-0.013259888,-0.042114258,0.0023727417,0.005683899,-0.027908325,0.040039062,-0.055847168,-0.03781128,-0.018753052,0.03274536,0.0121536255,0.04360962,-0.0110321045,0.017913818,-0.0231781,-0.018936157,-0.002658844,0.011222839,-0.0082473755,-0.0039043427,0.011512756,-0.014328003,0.037994385,-0.020767212,0.025314331,-0.023727417,0.030303955,0.03302002,0.0040512085,-0.074401855,0.027450562,-0.030838013,0.042053223,-0.04425049,-0.022613525,0.0025463104,0.029449463,-0.0023975372,0.03717041,0.020751953,-0.000009357929,-0.06842041,-0.045074463,-0.035980225,0.03060913,0.00049352646,-0.0013618469,0.018676758,0.00070238113,-0.015472412,-0.035736084,-0.008995056,0.008773804,0.009635925,0.023330688,-0.027008057,-0.0074501038,-0.0040893555,0.010391235,-0.030014038,-0.04119873,-0.06329346,0.049926758,-0.016952515,-0.015045166,-0.0010814667,0.020309448,-0.0034770966,0.05996704,-0.043273926,-0.035491943,0.017654419,0.033325195,-0.015403748,0.03942871,-0.003692627,-0.008995056,-0.012290955,-0.004722595,0.010276794,-0.027023315,-0.0052871704,0.019729614,0.026519775,-0.029541016,-0.05505371,0.007499695,-0.030639648,0.00042963028,-0.016693115,0.03125,0.03543091,0.010482788,0.018081665,0.030441284,0.030960083,-0.008422852,-0.00983429,0.047332764,0.0023212433,0.0052719116]],"meta":{"api_version":{"version":"1"},"billed_units":{"input_tokens":2}},"response_type":"embeddings_floats"}'
+      string: '{"id":"9fafb8cb-848d-4649-9a42-e2eb0c1b8899","texts":["hello","goodbye"],"embeddings":[[0.016220093,-0.00856781,-0.048736572,-0.070495605,0.00013661385,-0.014945984,-0.019195557,0.019256592,0.009284973,0.041656494,-0.0368042,0.00033402443,0.06329346,-0.03564453,0.045013428,-0.030380249,0.037109375,0.048980713,0.005420685,0.007293701,-0.02104187,0.04107666,-0.04006958,0.03527832,0.05102539,0.029876709,-0.0044441223,-0.0008635521,-0.018676758,-0.0395813,0.012878418,0.005531311,0.018630981,0.020507812,-0.0020656586,0.090148926,-0.012680054,-0.02609253,0.012260437,0.004333496,0.030944824,-0.03086853,-0.040649414,-0.023620605,-0.043273926,0.00033903122,-0.017807007,-0.018798828,0.0791626,-0.031036377,0.02015686,-0.014778137,0.017028809,-0.0012159348,-0.03756714,0.011207581,-0.07330322,-0.013168335,0.010421753,0.031188965,0.04537964,0.004573822,0.032592773,0.047088623,-0.0040626526,-0.019042969,0.023605347,-0.01322937,0.019485474,-0.015655518,0.016159058,0.0017547607,-0.0062713623,-0.047973633,-0.022567749,0.06378174,-0.009857178,0.014282227,0.004421234,-0.022628784,-0.021636963,-0.018814087,-0.08648682,-0.049102783,0.029541016,0.010398865,-0.013000488,-0.010253906,-0.0060157776,0.010528564,-0.014694214,0.053833008,0.045806885,0.0011043549,-0.038482666,0.011932373,-0.008918762,0.007537842,0.006767273,0.019165039,-0.054504395,-0.021408081,-0.02607727,-0.028457642,-0.015808105,0.02357483,-0.004650116,0.021743774,0.031921387,0.04788208,-0.0076942444,0.044921875,-0.023666382,0.010124207,-0.045654297,0.016708374,-0.0069503784,0.0038871765,-0.03237915,0.05166626,0.038970947,0.032440186,-0.008872986,0.007637024,-0.040008545,-0.008171082,-0.013618469,-0.044799805,0.051849365,-0.027770996,-0.01121521,0.050811768,-0.096191406,-0.034851074,-0.021942139,0.004573822,-0.017089844,-0.044128418,-0.00198555,0.022521973,0.07727051,-0.00026535988,0.0211792,0.050079346,-0.033721924,0.031982422,-0.0060157776,0.00000846386,0.0340271,0.019134521,-0.06665039,-0.026626587,0.010513306,0.057922363,0.015617371,0.06542969,-0.015670776,0.008834839,-0.01776123,0.028930664,-0.005382538,0.016403198,0.051605225,-0.014724731,-0.03781128,-0.012870789,0.003030777,0.0006828308,0.015304565,0.022628784,-0.0057144165,0.028518677,0.04763794,0.03189087,0.0070495605,-0.023727417,-0.037231445,0.017730713,0.04031372,0.025787354,0.033416748,-0.019973755,-0.025360107,0.07293701,-0.031234741,-0.05706787,0.029067993,0.0018968582,0.030456543,0.012321472,0.058532715,0.005176544,-0.039367676,-0.015731812,-0.015899658,-0.038116455,-0.017059326,-0.020446777,-0.004585266,0.039398193,0.007068634,-0.046936035,0.04257202,-0.043151855,-0.03857422,-0.033203125,-0.0110321045,0.011955261,0.0008773804,0.005947113,-0.008407593,-0.031402588,0.0045204163,-0.069885254,-0.030578613,-0.038513184,-0.08862305,-0.0025577545,-0.00082063675,0.04119873,0.0031108856,-0.0020809174,-0.016357422,-0.021865845,-0.008583069,-0.009765625,-0.04107666,-0.0079422,-0.06536865,-0.011009216,-0.015617371,0.033935547,-0.03451538,-0.008628845,-0.020584106,0.005104065,0.00046157837,0.03717041,0.01474762,-0.0011959076,0.012557983,0.002319336,-0.032348633,-0.0068855286,0.035827637,-0.00060653687,0.036987305,-0.0031471252,0.018997192,0.026931763,0.011146545,-0.021652222,0.035308838,-0.024749756,-0.016464233,0.039642334,0.0039482117,0.019958496,-0.03945923,0.036376953,-0.039245605,-0.008544922,-0.012649536,-0.0149002075,-0.036895752,-0.023651123,-0.012382507,-0.0057640076,-0.016189575,-0.015823364,0.016616821,-0.005092621,-0.01890564,0.00065374374,0.080322266,0.041809082,-0.059692383,-0.009223938,-0.001042366,0.012275696,-0.016220093,-0.02142334,-0.016738892,0.0015039444,0.03656006,-0.005722046,0.00073862076,0.01586914,-0.004020691,0.059906006,0.076416016,0.015556335,-0.015274048,0.024505615,0.013572693,0.020355225,-0.03149414,0.012023926,-0.002254486,-0.052001953,0.0055770874,0.037841797,0.0056991577,-0.023376465,-0.02508545,0.024093628,0.0234375,0.014305115,0.020202637,-0.04446411,0.02961731,0.022003174,0.011772156,0.016555786,-0.03213501,-0.031234741,-0.009468079,-0.0037574768,-0.08062744,-0.0067214966,0.008323669,-0.0077705383,-0.04437256,-0.025634766,-0.015144348,0.027450562,-0.0769043,-0.0029239655,-0.05206299,0.029144287,0.047973633,0.0004143715,-0.0127334595,-0.017333984,0.011650085,0.0143966675,0.029220581,-0.055999756,0.006614685,0.028518677,0.09436035,-0.013725281,0.029327393,0.0072021484,0.012756348,-0.005542755,-0.02079773,0.00705719,-0.006511688,-0.0112838745,0.024230957,-0.037384033,-0.030059814,-0.028961182,0.031829834,0.0005097389,0.007205963,-0.016662598,0.06945801,-0.07196045,0.022460938,-0.019302368,-0.038024902,-0.022232056,0.010238647,-0.027511597,-0.006298065,-0.022537231,-0.024429321,-0.01260376,0.015594482,-0.006717682,0.029525757,-0.0357666,-0.072631836,-0.01890564,-0.02758789,-0.066589355,0.05053711,0.003189087,0.029434204,0.025894165,0.045837402,0.018173218,0.052947998,0.04977417,-0.014701843,0.0014753342,0.0491333,0.008285522,-0.000705719,0.013122559,-0.045776367,-0.02684021,0.02986145,0.0010538101,-0.03753662,0.030685425,-0.086120605,-0.015083313,-0.015022278,0.0019445419,-0.023071289,-0.0015773773,-0.07287598,0.0579834,-0.040740967,-0.025039673,0.020050049,0.063964844,0.007286072,0.015342712,-0.009346008,-0.000021159649,-0.026672363,0.026473999,-0.017868042,-0.011947632,0.03466797,0.0074691772,-0.010932922,0.025360107,-0.023803711,0.040618896,-0.03778076,0.049804688,-0.026260376,0.03652954,0.032592773,-0.018585205,-0.02331543,-0.035125732,-0.005886078,-0.023208618,-0.033203125,0.07696533,-0.03842163,0.057617188,-0.0119018555,-0.037994385,-0.01184082,0.016845703,0.00868988,-0.005622864,-0.01096344,-0.019195557,0.019744873,0.022567749,-0.058685303,0.03552246,-0.090026855,0.026489258,-0.015090942,0.079711914,-0.009780884,0.01689148,0.047546387,0.036010742,0.019348145,0.011497498,0.0181427,-0.00010752678,-0.07080078,-0.01751709,-0.017120361,0.027160645,0.014961243,0.0068244934,-0.04638672,-0.010009766,0.014923096,-0.015563965,0.03286743,-0.0026741028,0.02331543,0.025009155,-0.015319824,-0.020889282,-0.02331543,0.006629944,-0.06451416,0.035980225,0.002840042,-0.06112671,-0.035491943,0.02166748,-0.036956787,-0.037078857,0.01852417,0.02330017,0.010620117,0.005836487,0.049621582,-0.006500244,-0.01499939,-0.0007419586,-0.0038070679,0.040039062,0.018173218,-0.066833496,-0.076171875,0.00052404404,-0.0073165894,-0.0011053085,0.045196533,-0.051879883,-0.017974854,0.020614624,0.039154053,0.030929565,0.04336548,-0.0009570122,-0.009338379,0.008399963,-0.0050201416,0.050994873,0.013626099,0.014808655,0.007881165,-0.040283203,-0.012359619,-0.010688782,0.068847656,0.023895264,-0.0020141602,0.005657196,-0.0011339188,0.008560181,-0.029220581,-0.025741577,0.058044434,0.04232788,0.059814453,-0.00046777725,-0.030960083,0.023910522,-0.03704834,0.0044784546,0.016342163,-0.01979065,-0.01876831,-0.0030288696,-0.008888245,0.012954712,0.014923096,-0.026504517,0.019546509,0.08105469,-0.058563232,0.09375,0.0008111,-0.0513916,0.062316895,-0.015136719,-0.02003479,-0.037322998,-0.04159546,-0.007980347,-0.003112793,0.06878662,-0.0019893646,-0.0018978119,-0.03265381,-0.0030822754,0.012306213,0.0032787323,0.051483154,-0.017684937,-0.007751465,0.013572693,-0.016616821,-0.018859863,-0.022201538,-0.03692627,-0.034484863,-0.0030269623,0.003540039,-0.0008559227,0.016464233,-0.004108429,0.012863159,0.004005432,-0.030975342,0.0074043274,0.0037631989,0.0362854,0.0211792,-0.00037264824,0.004108429,0.025909424,-0.0021820068,-0.038238525,-0.00089788437,0.00084495544,0.00756073,-0.0030460358,0.020050049,-0.061798096,0.0104599,0.0032310486,-0.046539307,0.019470215,0.046051025,-0.0385437,0.011550903,0.012535095,-0.05609131,0.01133728,-0.010757446,-0.0043029785,0.009170532,-0.020370483,-0.011161804,0.0074539185,-0.022262573,0.010192871,0.046936035,0.023132324,-0.0021438599,-0.03201294,-0.016723633,-0.0007214546,0.028671265,0.0033130646,0.038635254,-0.035247803,0.007659912,-0.0033283234,0.006477356,0.00011563301,-0.0059394836,0.0040130615,-0.0026359558,-0.059173584,0.024627686,0.076293945,-0.012969971,-0.0029964447,-0.08453369,0.025543213,0.019119263,-0.012283325,-0.033721924,-0.0042152405,-0.014717102,-0.0158844,-0.0025043488,-0.02444458,-0.028182983,0.02067566,0.008178711,0.024597168,-0.000062704086,-0.006427765,-0.0044136047,0.011650085,0.032928467,0.062805176,-0.040222168,-0.025634766,0.04397583,0.05517578,-0.03439331,-0.003929138,0.023086548,-0.0017929077,0.044677734,0.04977417,-0.0024414062,0.019485474,0.0090408325,0.016647339,0.011871338,-0.04348755,-0.059570312,0.0309906,0.039154053,0.016296387,0.039764404,-0.0009880066,-0.032806396,-0.05444336,0.04006958,0.019958496,-0.032409668,0.0044288635,0.062927246,0.029510498,0.0181427,-0.011482239,-0.044128418,-0.017745972,0.0070266724,-0.024215698,0.029006958,0.0055999756,-0.01689148,-0.014419556,-0.043945312,-0.0040664673,0.024398804,-0.015655518,0.05505371,-0.049987793,0.03466797,0.025268555,-0.031677246,-0.043029785,0.012062073,0.024810791,-0.0017004013,0.032562256,-0.0231781,0.0073242188,-0.0072135925,-0.03878784,-0.037353516,-0.034606934,-0.047424316,0.030151367,-0.020904541,-0.024047852,0.051879883,-0.010597229,0.048828125,-0.009399414,-0.039520264,-0.019500732,-0.0003476143,-0.016403198,0.03289795,0.007221222,-0.01335144,0.01889038,-0.011581421,0.022583008,0.04055786,0.037872314,0.060333252,0.0069007874,-0.04135132,-0.010391235,0.04638672,0.029052734,0.0013456345,0.0413208,0.013252258,0.04815674,-0.016693115,0.008125305,0.018844604,0.007232666,0.03692627,-0.01247406,-0.003168106,-0.06567383,-0.066223145,0.013595581,0.044067383,-0.03479004,-0.051849365,-0.012176514,0.0052986145,0.054016113,0.013893127,0.050689697,0.026855469,0.02532959,-0.026519775,0.0028381348,0.07244873,0.018508911,0.0070228577,0.010299683,-0.012268066,0.0053138733,0.0155181885,-0.018157959,-0.00034809113,-0.001496315,-0.012634277,0.0069465637,-0.021697998,0.022018433,-0.028518677,-0.021057129,0.024597168,0.043823242,-0.011833191,0.06298828,0.008956909,0.039093018,0.00029230118,0.068481445,0.03640747,-0.016815186,0.000015735626,0.00447464,0.036499023,-0.042175293,0.007408142,-0.011802673,-0.020492554,-0.0056877136,-0.026321411,-0.02178955,-0.008071899,0.021697998,-0.013023376,0.050079346,-0.0037403107,-0.021408081,-0.009773254,-0.004306793,-0.00023305416,-0.012878418,0.051483154,-0.032043457,0.026809692,-0.05255127,-0.0051345825,0.0496521,-0.0015707016,0.015365601,-0.022872925,0.02545166,0.043273926,-0.01625061,-0.021347046,0.055999756,0.057403564,0.013923645,-0.023544312,0.0440979,0.03302002,-0.052978516,-0.017959595,0.00036597252,0.037719727,-0.011886597,-0.0031528473,-0.025283813,0.012817383,-0.032684326,0.028045654,0.006996155,0.012207031,-0.03479004,0.028411865,0.01914978,0.028793335,0.028442383,0.035491943,-0.03866577,0.02658081,0.020355225,0.030960083,-0.045013428,0.0056037903,-0.009819031,-0.02331543,0.023788452,-0.05029297,-0.0284729,0.03692627,0.025253296,-0.025924683,0.021224976,-0.044067383,0.009643555,-0.0025806427,0.031036377,0.00932312,-0.040100098,-0.01902771,-0.0115737915,0.009902954,-0.031585693,0.022399902,0.051879883,0.014266968,0.027938843,0.03253174,-0.023864746,-0.01134491,-0.003211975,0.004890442,0.033416748,0.007019043,0.01927185,0.017425537,-0.054351807,-0.003736496,-0.013885498,-0.008834839,0.01625061,-0.015655518,0.015670776,-0.028244019,-0.015541077,-0.013084412,-0.046905518,0.026412964,-0.0234375,-0.023025513,0.042114258,0.055908203,-0.0041885376,-0.0309906,-0.022659302,0.011314392,-0.013656616,-0.016159058,0.028259277,0.0063705444,0.021392822,-0.06878662,-0.039398193,-0.002670288,-0.063964844,-0.020980835,0.028747559,0.006931305,-0.02861023,-0.057769775,0.022857666,-0.03564453,-0.0262146,-0.04196167,0.0015220642,-0.0031604767,-0.030700684,-0.037475586,-0.0019798279,-0.0045661926,-0.014556885,0.0074806213,-0.032196045,-0.010253906,0.0027389526,-0.0127334595,-0.00082826614,-0.010650635,0.03842163,-0.024993896,0.019836426,0.0021972656,-0.008918762,-0.02848816,-0.0059890747,0.016235352,-0.008277893,-0.054901123,0.038909912,-0.033233643,0.047027588,-0.029830933,-0.039794922,-0.007003784,-0.023895264,-0.005176544,0.025283813,0.032104492,-0.027801514,-0.08691406,-0.015167236,-0.03579712,0.022216797,0.007385254,0.012229919,-0.0051002502,-0.01423645,-0.021606445,-0.03451538,-0.008285522,-0.02545166,0.019699097,-0.012016296,-0.03829956,0.013587952,-0.035583496,0.04925537,-0.011436462,0.051330566,-0.066467285,0.080200195,-0.061065674,-0.04232788,0.01802063,0.015777588,-0.0113220215,0.03540039,-0.04788208,-0.032409668,0.052520752,-0.021987915,0.03164673,-0.020080566,0.082092285,0.01285553,-0.008506775,0.0024719238,0.023483276,0.012001038,-0.001666069,-0.0067977905,0.018249512,-0.054260254,0.0054626465,-0.06793213,-0.04989624,0.027923584,-0.0046539307,-0.042297363,0.028198242,-0.0067977905,0.019851685,0.0014095306,-0.0030536652,-0.015365601,-0.026428223,0.03677368,-0.018493652,0.01008606],[0.046539307,-0.022583008,0.008972168,-0.0395813,-0.018188477,-0.011512756,0.0028266907,-0.0020771027,-0.0019168854,0.032165527,-0.050720215,-0.04937744,0.020004272,-0.0129852295,-0.019042969,-0.067993164,0.02684021,0.039123535,0.032592773,-0.004043579,0.026397705,0.007381439,-0.038635254,0.008041382,0.015625,0.06744385,-0.017547607,-0.0014400482,-0.052886963,-0.055847168,-0.005012512,0.042907715,-0.0129852295,0.08538818,-0.038970947,0.051116943,-0.046569824,0.037475586,0.052978516,-0.028945923,0.015556335,-0.008361816,-0.060668945,-0.026062012,-0.054779053,-0.0071983337,-0.0124435425,0.0025539398,0.061035156,-0.012702942,0.046783447,0.030471802,0.040374756,-0.0008983612,-0.03463745,0.018554688,-0.047729492,-0.03543091,0.024475098,0.026947021,0.015403748,-0.0037517548,0.034729004,0.013900757,0.021575928,-0.025772095,-0.057403564,0.008522034,0.042541504,0.015197754,-0.0019454956,-0.03353882,-0.0021343231,-0.044433594,-0.045043945,0.08947754,0.0030994415,0.03741455,0.0016508102,-0.0345459,0.018371582,-0.008918762,-0.03564453,-0.014045715,0.008308411,0.008056641,0.0021018982,-0.022506714,-0.01448822,-0.020645142,-0.009513855,0.07104492,0.013954163,-0.025253296,-0.0524292,-0.004737854,0.0012722015,-0.014976501,-0.026824951,-0.040618896,-0.03262329,-0.010047913,-0.046081543,-0.0016231537,-0.026123047,0.03125,-0.023895264,0.016418457,0.017669678,0.06347656,0.009300232,-0.046020508,-0.014427185,-0.0074539185,-0.021194458,0.034088135,-0.0132751465,0.038970947,-0.025436401,0.08917236,-0.03955078,-0.011116028,-0.05795288,0.0066833496,0.006134033,-0.040283203,-0.0149383545,0.07891846,0.08898926,0.0079193115,-0.04916382,0.037963867,-0.044677734,-0.06555176,-0.032440186,-0.032226562,0.0042686462,-0.013679504,-0.021331787,0.03552246,0.036376953,-0.013900757,0.026885986,0.009681702,-0.012084961,0.045196533,0.00044250488,-0.030166626,0.025100708,0.003107071,-0.06549072,-0.0112838745,0.037384033,0.056854248,-0.026641846,0.03439331,0.015655518,-0.014633179,-0.011512756,-0.013710022,-0.028533936,0.02508545,0.09442139,-0.012939453,-0.04168701,-0.01928711,0.005344391,-0.018508911,0.013893127,0.0017175674,0.002714157,-0.02810669,-0.0053253174,0.02960205,0.00063943863,0.006816864,-0.05328369,0.032287598,0.04135132,0.0317688,0.03125,-0.031341553,-0.0064697266,0.04800415,-0.016342163,-0.0013685226,-0.012832642,0.008918762,0.018661499,-0.0040245056,-0.0025806427,0.03390503,0.00081014633,0.007972717,-0.021759033,-0.033355713,-0.036834717,0.0050354004,-0.030731201,-0.018234253,-0.023666382,0.0048675537,0.026931763,-0.013427734,-0.024047852,0.002046585,-0.017959595,0.034820557,0.003042221,0.030517578,0.020065308,-0.013145447,-0.04751587,0.04147339,0.009353638,-0.03173828,-0.028442383,-0.015403748,-0.0042762756,0.034820557,-0.01878357,0.012046814,-0.022521973,0.03125,0.041656494,-0.052642822,0.005844116,-0.03390503,-0.0018539429,-0.012771606,-0.04159546,0.02809143,-0.0287323,-0.0574646,-0.028549194,0.031921387,0.024261475,0.044891357,-0.0071105957,0.00003862381,0.011512756,0.0022945404,-0.042175293,-0.027435303,0.013893127,-0.013961792,0.0231781,-0.0036678314,0.014480591,0.004108429,0.013847351,-0.045135498,0.042419434,-0.034362793,-0.0010766983,0.034332275,0.005756378,-0.015274048,0.02809143,-0.024246216,0.0036392212,-0.000024139881,-0.039367676,0.01361084,-0.03567505,-0.021942139,-0.029037476,-0.012809753,-0.03805542,-0.0036392212,0.029510498,-0.011116028,-0.024978638,0.010215759,0.09307861,0.014328003,-0.08642578,-0.011352539,0.019973755,0.006412506,-0.0034542084,0.020248413,0.029525757,-0.0024166107,0.03366089,0.030227661,0.018615723,-0.0030593872,-0.011184692,0.02960205,0.049987793,0.046844482,-0.007663727,0.019378662,0.042816162,0.0075035095,0.06719971,0.046051025,-0.026107788,-0.019714355,0.011230469,0.018218994,-0.000086426735,-0.043701172,-0.00356102,0.062805176,0.052734375,-0.004459381,0.018066406,-0.02458191,-0.015411377,-0.047454834,0.02394104,0.013153076,-0.011123657,-0.036346436,-0.0075912476,0.023345947,-0.052368164,0.02281189,0.032989502,-0.003238678,-0.044677734,0.019851685,-0.029815674,-0.002861023,0.030700684,-0.040130615,-0.020614624,0.028167725,0.037902832,0.0109939575,-0.031051636,-0.051940918,-0.0067481995,0.007457733,0.025314331,-0.0101623535,0.014854431,0.010513306,0.08642578,0.019424438,0.010917664,-0.00037670135,0.0024719238,-0.02558899,-0.049102783,0.009773254,0.042236328,-0.024765015,0.0015716553,-0.018707275,-0.014671326,0.027511597,0.03378296,0.0035648346,0.0109939575,0.005218506,0.029129028,-0.07824707,-0.013122559,-0.03527832,-0.061462402,0.061798096,0.037475586,-0.007896423,-0.017807007,0.031188965,-0.01802063,0.037628174,-0.018554688,0.02079773,-0.0021190643,-0.030334473,-0.07287598,0.008171082,0.006504059,-0.067993164,0.048553467,0.015960693,-0.021087646,0.02142334,0.026672363,0.052001953,0.03552246,0.030731201,-0.035217285,-0.017913818,0.06628418,0.039398193,0.013877869,-0.008529663,0.030838013,-0.042388916,-0.0008792877,-0.0209198,0.040893555,0.05316162,-0.0048446655,-0.02229309,-0.042541504,0.024246216,-0.02053833,-0.0032405853,-0.059387207,0.026184082,-0.046447754,-0.035186768,0.017425537,0.05456543,0.018722534,0.0063819885,0.012870789,-0.019882202,-0.0209198,0.010322571,0.04949951,0.020980835,-0.030563354,-0.04815674,0.013893127,0.047546387,0.024871826,0.0046958923,0.019943237,0.044403076,-0.033996582,-0.023513794,0.03427124,-0.011016846,-0.029922485,-0.021728516,-0.010513306,-0.05014038,-0.060699463,0.013519287,-0.025909424,0.06286621,0.027053833,-0.03717041,-0.014839172,0.033569336,-0.010345459,0.02458191,-0.028167725,-0.010894775,0.018371582,0.00028562546,-0.060455322,0.030670166,-0.103637695,0.03491211,-0.0289917,0.07141113,-0.021453857,-0.012573242,0.04348755,0.040924072,0.026901245,0.03186035,0.009063721,-0.021102905,0.0066986084,0.018341064,0.0014219284,-0.019104004,0.027557373,-0.0115356445,-0.055755615,0.010551453,-0.021850586,0.00014603138,-0.008956909,0.015991211,0.023223877,0.024276733,-0.024246216,0.040161133,-0.04815674,-0.002943039,-0.04748535,0.017349243,0.03414917,-0.0035266876,-0.008857727,0.010612488,-0.009536743,-0.017562866,0.041229248,-0.059173584,-0.03289795,-0.047424316,0.015266418,-0.02029419,-0.010307312,-0.01802063,0.00995636,-0.04006958,0.029190063,-0.020950317,-0.081970215,-0.0001322031,0.043273926,-0.045562744,0.0206604,-0.023605347,0.0020694733,0.0129776,0.049926758,0.061828613,0.027999878,0.0048065186,0.041503906,0.0011987686,0.004306793,-0.024246216,0.06161499,0.012138367,-0.0019340515,-0.01876831,-0.00894928,-0.036621094,0.10217285,0.026412964,-0.055480957,0.015388489,0.045074463,-0.018035889,-0.0039367676,-0.04333496,0.0670166,0.008102417,0.047027588,0.033233643,-0.034454346,0.046325684,-0.058807373,0.032165527,0.013969421,-0.06958008,-0.042938232,-0.0234375,-0.019805908,0.008102417,0.02659607,-0.058929443,0.011680603,-0.0007176399,-0.015838623,0.028182983,-0.029937744,-0.03778076,0.017303467,-0.027374268,-0.024169922,-0.0418396,-0.039276123,0.0032348633,-0.0011034012,0.018325806,0.009719849,-0.0231781,-0.009414673,-0.016159058,0.04421997,-0.0056762695,0.04498291,-0.04473877,-0.026535034,0.037322998,-0.018218994,0.01071167,0.003932953,-0.045440674,-0.025039673,-0.055541992,-0.005710602,0.008148193,0.015258789,-0.0021839142,0.037017822,-0.0048980713,-0.03729248,-0.008880615,0.026351929,0.048950195,-0.012428284,0.0016965866,-0.00065231323,0.01474762,-0.03265381,-0.02418518,0.046936035,-0.006427765,-0.056274414,-0.0597229,0.0090789795,-0.03286743,0.022842407,-0.019058228,-0.04208374,0.03994751,0.028640747,-0.035339355,0.0027751923,0.04196167,-0.0049934387,-0.00021135807,0.0107803345,0.016555786,0.0060691833,-0.04864502,-0.024414062,0.024963379,-0.021469116,0.017929077,0.061309814,-0.0038223267,-0.022369385,-0.014045715,-0.00019526482,0.00020384789,0.034423828,0.011497498,0.018325806,-0.009346008,0.012542725,-0.026062012,-0.014099121,0.02217102,-0.03564453,0.008911133,-0.025817871,-0.016662598,0.029006958,0.011817932,-0.0034389496,-0.0036144257,-0.021316528,0.037139893,0.011497498,-0.0077285767,-0.053649902,-0.05142212,0.04058838,-0.0055885315,-0.02331543,0.019165039,-0.018508911,0.037750244,-0.0011787415,0.015533447,-0.01637268,0.0072517395,0.02722168,0.010543823,0.037750244,0.06329346,-0.0067710876,-0.009864807,0.0011739731,0.046142578,-0.044830322,-0.010543823,0.035980225,-0.009399414,0.0026226044,0.021820068,-0.011459351,0.01727295,0.0019159317,-0.007434845,-0.02809143,-0.047576904,-0.027755737,0.028793335,-0.02217102,0.02494812,-0.008270264,0.0056648254,-0.029403687,-0.03137207,0.06323242,-0.044036865,-0.017852783,-0.006061554,0.06677246,0.039611816,-0.007286072,-0.027740479,-0.057403564,-0.021148682,-0.027923584,-0.037628174,0.04522705,-0.0140686035,-0.016418457,0.048553467,-0.000998497,-0.019241333,-0.025527954,0.034423828,0.027511597,0.0022830963,0.0021705627,0.05227661,0.008583069,-0.030197144,-0.007030487,0.018920898,0.010467529,-0.005760193,-0.017166138,0.002494812,-0.0012168884,-0.040771484,-0.035308838,-0.030456543,-0.044433594,0.039489746,-0.0126571655,-0.06561279,0.026138306,-0.031463623,0.023010254,-0.01953125,0.0056152344,-0.0047454834,0.009185791,-0.009841919,0.047058105,0.005130768,0.00043201447,0.015151978,-0.0018987656,-0.007774353,0.04321289,0.0052604675,0.034454346,-0.027328491,-0.013130188,-0.019546509,0.03656006,0.016220093,-0.01637268,0.003665924,-0.013809204,0.038848877,0.01737976,-0.013587952,0.046539307,0.02204895,0.045654297,0.008575439,0.029281616,-0.029907227,-0.019973755,-0.0149383545,0.052093506,-0.04067993,-0.04083252,-0.0043754578,-0.00774765,0.059509277,0.0018844604,0.054870605,-0.08300781,-0.059143066,-0.015487671,0.009887695,0.0256958,0.02168274,-0.005153656,0.020370483,-0.019851685,0.004383087,0.017150879,-0.030914307,0.009391785,-0.022903442,-0.017807007,0.028274536,0.024246216,0.018630981,-0.022735596,0.01902771,0.026565552,0.032470703,-0.0059890747,0.01739502,0.00724411,0.034088135,-0.034729004,0.035064697,-0.019577026,-0.021194458,0.006324768,-0.014595032,-0.0066070557,-0.056274414,0.014625549,-0.014602661,-0.030151367,0.0013685226,-0.02607727,-0.02607727,-0.004386902,0.027740479,-0.0060424805,0.047180176,-0.00067043304,0.0006160736,0.0038070679,-0.004875183,0.0014781952,0.011177063,0.042816162,-0.0357666,0.01878357,-0.0063438416,0.0031414032,0.03665161,-0.0032787323,0.04425049,0.013641357,-0.0026760101,0.038726807,0.024291992,-0.033233643,-0.028381348,0.060150146,-0.019622803,-0.0473938,0.006916046,-0.031921387,0.020477295,0.0051116943,-0.04156494,0.033569336,0.056549072,0.031097412,-0.011619568,0.032958984,0.017288208,-0.025405884,-0.0036773682,0.045806885,-0.040008545,0.023620605,0.020523071,0.024856567,0.0287323,0.010810852,-0.009422302,0.024902344,0.030548096,-0.011550903,-0.03062439,0.013931274,0.011451721,-0.030563354,0.034820557,-0.01612854,0.015007019,0.056884766,-0.019821167,-0.014060974,0.022491455,-0.085998535,0.017120361,0.01184845,0.018051147,0.01146698,0.0041046143,-0.013832092,0.025512695,0.0072898865,-0.002084732,0.040924072,0.037841797,-0.028625488,-0.008453369,0.026321411,-0.014846802,0.005218506,-0.057434082,0.0088272095,0.017532349,0.0023937225,-0.0033740997,-0.022064209,-0.018661499,0.007293701,-0.006641388,0.018569946,0.03366089,-0.04046631,0.030639648,-0.006340027,-0.031677246,-0.015777588,-0.008575439,0.0068130493,0.0039138794,0.009223938,0.00283432,-0.0010385513,-0.010276794,-0.07055664,-0.04660034,0.0657959,-0.01966858,-0.062927246,-0.022903442,0.04144287,0.027114868,-0.114868164,-0.079711914,-0.04940796,-0.036743164,-0.017578125,0.015731812,0.032440186,-0.0137786865,-0.041412354,0.0026302338,0.006980896,-0.027664185,0.039916992,-0.055023193,-0.037841797,-0.018722534,0.03213501,0.01197052,0.043304443,-0.01108551,0.017974854,-0.023101807,-0.018798828,-0.0014486313,0.011161804,-0.008972168,-0.003873825,0.010948181,-0.01448822,0.03717041,-0.020248413,0.025756836,-0.024383545,0.030426025,0.03201294,0.003774643,-0.07421875,0.027877808,-0.031280518,0.041900635,-0.043792725,-0.0231781,0.0018749237,0.028427124,-0.002199173,0.036315918,0.021469116,0.00023794174,-0.06890869,-0.04547119,-0.036102295,0.030944824,0.0006055832,-0.00031113625,0.019195557,0.0007367134,-0.015319824,-0.036895752,-0.010009766,0.008285522,0.009475708,0.024139404,-0.026184082,-0.006717682,-0.004627228,0.011199951,-0.030792236,-0.0413208,-0.062927246,0.050231934,-0.01727295,-0.014381409,-0.0013246536,0.020202637,-0.0032100677,0.059692383,-0.044067383,-0.03604126,0.017837524,0.034210205,-0.015197754,0.037597656,-0.0037765503,-0.0079193115,-0.013694763,-0.0048713684,0.010055542,-0.02822876,-0.0045928955,0.020095825,0.026748657,-0.029464722,-0.05496216,0.0070533752,-0.030303955,-0.00049448013,-0.016815186,0.03164673,0.035949707,0.011009216,0.017684937,0.02961731,0.031799316,-0.008552551,-0.009292603,0.047180176,0.002313614,0.005973816]],"meta":{"api_version":{"version":"1"},"billed_units":{"input_tokens":2}},"response_type":"embeddings_floats"}'
     headers:
       Alt-Svc:
       - h3=":443"; ma=2592000,h3-29=":443"; ma=2592000
       Via:
       - 1.1 google
       access-control-expose-headers:
       - X-Debug-Trace-ID
       cache-control:
       - no-cache, no-store, no-transform, must-revalidate, private, max-age=0
       content-type:
       - application/json
       date:
-      - Fri, 26 Apr 2024 13:51:32 GMT
+      - Fri, 24 May 2024 09:38:05 GMT
       expires:
       - Thu, 01 Jan 1970 00:00:00 UTC
       num_chars:
       - '12'
       num_tokens:
       - '2'
       pragma:
@@ -54,20 +54,20 @@
       transfer-encoding:
       - chunked
       vary:
       - Origin
       x-accel-expires:
       - '0'
       x-debug-trace-id:
-      - a4a9481da87382f77e640a8707065fbe
+      - 7332694a5013a7531cb9886818a5d508
       x-endpoint-monthly-call-limit:
       - '1000'
       x-envoy-upstream-service-time:
-      - '69'
+      - '131'
       x-trial-endpoint-call-limit:
-      - '40'
+      - '100'
       x-trial-endpoint-call-remaining:
-      - '39'
+      - '99'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `langtrace_python_sdk-2.0.9/src/tests/cohere/cassettes/test_cohere_rerank.yaml` & `langtrace_python_sdk-2.1.0/src/tests/cohere/cassettes/test_cohere_rerank.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -17,60 +17,60 @@
       connection:
       - keep-alive
       content-length:
       - '653'
       content-type:
       - application/json
       host:
-      - api.cohere.ai
+      - api.cohere.com
       user-agent:
       - python-httpx/0.27.0
       x-fern-language:
       - Python
       x-fern-sdk-name:
       - cohere
       x-fern-sdk-version:
-      - 5.3.2
+      - 5.5.3
     method: POST
-    uri: https://api.cohere.ai/v1/rerank
+    uri: https://api.cohere.com/v1/rerank
   response:
     body:
-      string: '{"id":"81824c15-b198-48cb-843c-08058b40a39e","results":[{"index":2,"relevance_score":0.98005307},{"index":3,"relevance_score":0.27904198},{"index":0,"relevance_score":0.10194652}],"meta":{"api_version":{"version":"1"},"billed_units":{"search_units":1}}}'
+      string: '{"id":"f176327d-f9d3-4c49-aa20-bf5e8345cf81","results":[{"index":2,"relevance_score":0.98005307},{"index":3,"relevance_score":0.27904198},{"index":0,"relevance_score":0.10194652}],"meta":{"api_version":{"version":"1"},"billed_units":{"search_units":1}}}'
     headers:
       Alt-Svc:
       - h3=":443"; ma=2592000,h3-29=":443"; ma=2592000
       Via:
       - 1.1 google
       access-control-expose-headers:
       - X-Debug-Trace-ID
       cache-control:
       - no-cache, no-store, no-transform, must-revalidate, private, max-age=0
       content-length:
       - '253'
       content-type:
       - application/json
       date:
-      - Fri, 26 Apr 2024 13:51:19 GMT
+      - Fri, 24 May 2024 09:38:06 GMT
       expires:
       - Thu, 01 Jan 1970 00:00:00 UTC
       pragma:
       - no-cache
       server:
       - envoy
       vary:
       - Origin
       x-accel-expires:
       - '0'
       x-debug-trace-id:
-      - 8063c83d2452d0fa74f6798659d96da8
+      - a3f78056e94ceceefe9d31dc8103ba2b
       x-endpoint-monthly-call-limit:
       - '1000'
       x-envoy-upstream-service-time:
       - '40'
       x-trial-endpoint-call-limit:
-      - '40'
+      - '10'
       x-trial-endpoint-call-remaining:
-      - '39'
+      - '9'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `langtrace_python_sdk-2.0.9/src/tests/langchain/test_langchain.py` & `langtrace_python_sdk-2.1.0/src/tests/langchain/test_langchain.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/langchain/test_langchain_community.py` & `langtrace_python_sdk-2.1.0/src/tests/langchain/test_langchain_community.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/langchain/test_langchain_core.py` & `langtrace_python_sdk-2.1.0/src/tests/langchain/test_langchain_core.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/openai/conftest.py` & `langtrace_python_sdk-2.1.0/src/tests/openai/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/openai/test_chat_completion.py` & `langtrace_python_sdk-2.1.0/src/tests/openai/test_chat_completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/openai/test_image_generation.py` & `langtrace_python_sdk-2.1.0/src/tests/openai/test_image_generation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml` & `langtrace_python_sdk-2.1.0/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/openai/cassettes/test_async_image_generation.yaml` & `langtrace_python_sdk-2.1.0/src/tests/openai/cassettes/test_async_image_generation.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/openai/cassettes/test_chat_completion.yaml` & `langtrace_python_sdk-2.1.0/src/tests/openai/cassettes/test_chat_completion.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/openai/cassettes/test_chat_completion_streaming.yaml` & `langtrace_python_sdk-2.1.0/src/tests/openai/cassettes/test_chat_completion_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/openai/cassettes/test_image_generation.yaml` & `langtrace_python_sdk-2.1.0/src/tests/openai/cassettes/test_image_generation.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/pinecone/conftest.py` & `langtrace_python_sdk-2.1.0/src/tests/pinecone/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/pinecone/test_pinecone.py` & `langtrace_python_sdk-2.1.0/src/tests/pinecone/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/pinecone/cassettes/test_query.yaml` & `langtrace_python_sdk-2.1.0/src/tests/pinecone/cassettes/test_query.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/pinecone/cassettes/test_upsert.yaml` & `langtrace_python_sdk-2.1.0/src/tests/pinecone/cassettes/test_upsert.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/src/tests/qdrant/test_qdrant.py` & `langtrace_python_sdk-2.1.0/src/tests/qdrant/test_qdrant.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/.gitignore` & `langtrace_python_sdk-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/LICENSE` & `langtrace_python_sdk-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.9/README.md` & `langtrace_python_sdk-2.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -24,32 +24,33 @@
 4. In your application, install the Langtrace SDK and initialize it with the API key you generated in the step 3.
 5. The code for installing and setting up the SDK is shown below
 
 ## Getting Started
 
 Get started by adding simply three lines to your code!
 
-``` python
+```python
 pip install langtrace-python-sdk
 ```
 
-``` python
+```python
 from langtrace_python_sdk import langtrace # Must precede any llm module imports
 langtrace.init(api_key=<your_api_key>)
 ```
 
 OR
 
-``` python
+```python
 from langtrace_python_sdk import langtrace # Must precede any llm module imports
 langtrace.init() # LANGTRACE_API_KEY as an ENVIRONMENT variable
 ```
 
 ## FastAPI Quick Start
-Initialize FastAPI project and add this inside the ```main.py``` file
+
+Initialize FastAPI project and add this inside the `main.py` file
 
 ```python
 from fastapi import FastAPI
 from langtrace_python_sdk import langtrace
 from openai import OpenAI
 
 langtrace.init()
@@ -63,15 +64,17 @@
         messages=[{"role": "user", "content": "Say this is a test three times"}],
         stream=False,
     )
     return {"Hello": "World"}
 ```
 
 ## Django Quick Start
-Initialize django project and add this inside the ```__init.py__``` file
+
+Initialize django project and add this inside the `__init.py__` file
+
 ```python
 from langtrace_python_sdk import langtrace
 from openai import OpenAI
 
 
 langtrace.init()
 client = OpenAI()
@@ -81,15 +84,17 @@
     messages=[{"role": "user", "content": "Say this is a test three times"}],
     stream=False,
 )
 
 ```
 
 ## Flask Quick Start
-Initialize flask project and this inside ```app.py``` file
+
+Initialize flask project and this inside `app.py` file
+
 ```python
 from flask import Flask
 from langtrace_python_sdk import langtrace
 from openai import OpenAI
 
 langtrace.init()
 client = OpenAI()
@@ -106,36 +111,47 @@
     return "Hello, World!"
 ```
 
 ## Langtrace Self Hosted
 
 Get started by adding simply two lines to your code and see traces being logged to the console!
 
-``` python
+```python
 pip install langtrace-python-sdk
 ```
 
-``` python
+```python
 from langtrace_python_sdk import langtrace # Must precede any llm module imports
 langtrace.init(write_spans_to_console=True)
 ```
 
 ## Langtrace self hosted custom exporter
 
 Get started by adding simply three lines to your code and see traces being exported to your remote location!
 
-``` python
+```python
 pip install langtrace-python-sdk
 ```
 
-``` python
+```python
 from langtrace_python_sdk import langtrace # Must precede any llm module imports
 langtrace.init(custom_remote_exporter=<your_exporter>, batch=<True or False>)
 ```
 
+### Configure Langtrace
+
+| Parameter                  | Type                                | Default Value                 | Description                                                                    |
+| -------------------------- | ----------------------------------- | ----------------------------- | ------------------------------------------------------------------------------ |
+| `api_key`                  | `str`                               | `LANGTRACE_API_KEY` or `None` | The API key for authentication.                                                |
+| `batch`                    | `bool`                              | `True`                        | Whether to batch spans before sending them.                                    |
+| `write_spans_to_console`   | `bool`                              | `False`                       | Whether to write spans to the console.                                         |
+| `custom_remote_exporter`   | `Optional[Exporter]`                | `None`                        | Custom remote exporter. If `None`, a default `LangTraceExporter` will be used. |
+| `api_host`                 | `Optional[str]`                     | `https://langtrace.ai/`       | The API host for the remote exporter.                                          |
+| `disable_instrumentations` | `Optional[DisableInstrumentations]` | `None`                        | You can pass an object to disable instrumentation for specific vendors ex: `{'only': ['openai']}` or `{'all_except': ['openai']}`
+
 ### Additional Customization
 
 - `@with_langtrace_root_span` - this decorator is designed to organize and relate different spans, in a hierarchical manner. When you're performing multiple operations that you want to monitor together as a unit, this function helps by establishing a "parent" (`LangtraceRootSpan` or whatever is passed to `name`) span. Then, any calls to the LLM APIs made within the given function (fn) will be considered "children" of this parent span. This setup is especially useful for tracking the performance or behavior of a group of operations collectively, rather than individually.
 
 ```python
 from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
 
@@ -145,15 +161,14 @@
         model="gpt-4",
         messages=[{"role": "user", "content": "Say this is a test three times"}],
         stream=False,
     )
     return response
 ```
 
-
 - `with_additional_attributes` - this function is designed to enhance the traces by adding custom attributes to the current context. These custom attributes provide extra details about the operations being performed, making it easier to analyze and understand their behavior.
 
 ```python
 from langtrace_python_sdk.utils.with_root_span import (
     with_langtrace_root_span,
     with_additional_attributes,
 )
@@ -182,15 +197,14 @@
 def chat_completion():
    api_call1()
    api_call2()
 ```
 
 - `get_prompt_from_registry` - this function is designed to fetch the desired prompt from the `Prompt Registry`. You can pass two options for filtering `prompt_version` & `variables`.
 
-
 ```python
 from langtrace_python_sdk import get_prompt_from_registry
 
 prompt = get_prompt_from_registry(<Registry ID>, options={"prompt_version": 1, "variables": {"foo": "bar"} })
 ```
 
 ## Supported integrations
```

### Comparing `langtrace_python_sdk-2.0.9/pyproject.toml` & `langtrace_python_sdk-2.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -14,44 +14,48 @@
 license = "Apache-2.0"
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  'trace-attributes>=3.0.5',
+  'trace-attributes>=4.0.2',
   'opentelemetry-api',
   'opentelemetry-sdk',
   'opentelemetry-instrumentation',
   'pinecone-client',
-  'tiktoken'
+  'tiktoken',
+  'opentelemetry-exporter-otlp-proto-http>=1.24.0',
+  'opentelemetry-exporter-otlp-proto-grpc>=1.24.0',
+  'weaviate-client',
 ]
 
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = [
     "openai",
     "anthropic",
+    "chromadb",
+    'qdrant-client',
     "python-dotenv",
     "langchain",
     'langchain-community',
     "langchain-openai",
-    "llama-index",
     "langchain-openai",
     "chromadb",
     "cohere",
-    "qdrant_client"
+    "qdrant_client",
+    "weaviate-client",
 ]
 
 test = [
     "pytest",
     "pytest-vcr",
     "pytest-asyncio",
-    "protobuf==3.20.0",
 ]
 
 
 
 [project.urls]
 Homepage = "https://github.com/Scale3-Labs/langtrace-python-sdk"
```

### Comparing `langtrace_python_sdk-2.0.9/PKG-INFO` & `langtrace_python_sdk-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.3
 Name: langtrace-python-sdk
-Version: 2.0.9
+Version: 2.1.0
 Summary: Python SDK for LangTrace
 Project-URL: Homepage, https://github.com/Scale3-Labs/langtrace-python-sdk
 Author-email: Scale3 Labs <engineering@scale3labs.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: opentelemetry-api
+Requires-Dist: opentelemetry-exporter-otlp-proto-grpc>=1.24.0
+Requires-Dist: opentelemetry-exporter-otlp-proto-http>=1.24.0
 Requires-Dist: opentelemetry-instrumentation
 Requires-Dist: opentelemetry-sdk
 Requires-Dist: pinecone-client
 Requires-Dist: tiktoken
-Requires-Dist: trace-attributes>=3.0.5
+Requires-Dist: trace-attributes>=4.0.2
+Requires-Dist: weaviate-client
 Provides-Extra: dev
 Requires-Dist: anthropic; extra == 'dev'
 Requires-Dist: chromadb; extra == 'dev'
 Requires-Dist: cohere; extra == 'dev'
 Requires-Dist: langchain; extra == 'dev'
 Requires-Dist: langchain-community; extra == 'dev'
 Requires-Dist: langchain-openai; extra == 'dev'
-Requires-Dist: llama-index; extra == 'dev'
 Requires-Dist: openai; extra == 'dev'
 Requires-Dist: python-dotenv; extra == 'dev'
 Requires-Dist: qdrant-client; extra == 'dev'
+Requires-Dist: weaviate-client; extra == 'dev'
 Provides-Extra: test
-Requires-Dist: protobuf==3.20.0; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: pytest-vcr; extra == 'test'
 Description-Content-Type: text/markdown
 
 # [Langtrace](https://www.langtrace.ai)
 
@@ -60,32 +62,33 @@
 4. In your application, install the Langtrace SDK and initialize it with the API key you generated in the step 3.
 5. The code for installing and setting up the SDK is shown below
 
 ## Getting Started
 
 Get started by adding simply three lines to your code!
 
-``` python
+```python
 pip install langtrace-python-sdk
 ```
 
-``` python
+```python
 from langtrace_python_sdk import langtrace # Must precede any llm module imports
 langtrace.init(api_key=<your_api_key>)
 ```
 
 OR
 
-``` python
+```python
 from langtrace_python_sdk import langtrace # Must precede any llm module imports
 langtrace.init() # LANGTRACE_API_KEY as an ENVIRONMENT variable
 ```
 
 ## FastAPI Quick Start
-Initialize FastAPI project and add this inside the ```main.py``` file
+
+Initialize FastAPI project and add this inside the `main.py` file
 
 ```python
 from fastapi import FastAPI
 from langtrace_python_sdk import langtrace
 from openai import OpenAI
 
 langtrace.init()
@@ -99,15 +102,17 @@
         messages=[{"role": "user", "content": "Say this is a test three times"}],
         stream=False,
     )
     return {"Hello": "World"}
 ```
 
 ## Django Quick Start
-Initialize django project and add this inside the ```__init.py__``` file
+
+Initialize django project and add this inside the `__init.py__` file
+
 ```python
 from langtrace_python_sdk import langtrace
 from openai import OpenAI
 
 
 langtrace.init()
 client = OpenAI()
@@ -117,15 +122,17 @@
     messages=[{"role": "user", "content": "Say this is a test three times"}],
     stream=False,
 )
 
 ```
 
 ## Flask Quick Start
-Initialize flask project and this inside ```app.py``` file
+
+Initialize flask project and this inside `app.py` file
+
 ```python
 from flask import Flask
 from langtrace_python_sdk import langtrace
 from openai import OpenAI
 
 langtrace.init()
 client = OpenAI()
@@ -142,36 +149,47 @@
     return "Hello, World!"
 ```
 
 ## Langtrace Self Hosted
 
 Get started by adding simply two lines to your code and see traces being logged to the console!
 
-``` python
+```python
 pip install langtrace-python-sdk
 ```
 
-``` python
+```python
 from langtrace_python_sdk import langtrace # Must precede any llm module imports
 langtrace.init(write_spans_to_console=True)
 ```
 
 ## Langtrace self hosted custom exporter
 
 Get started by adding simply three lines to your code and see traces being exported to your remote location!
 
-``` python
+```python
 pip install langtrace-python-sdk
 ```
 
-``` python
+```python
 from langtrace_python_sdk import langtrace # Must precede any llm module imports
 langtrace.init(custom_remote_exporter=<your_exporter>, batch=<True or False>)
 ```
 
+### Configure Langtrace
+
+| Parameter                  | Type                                | Default Value                 | Description                                                                    |
+| -------------------------- | ----------------------------------- | ----------------------------- | ------------------------------------------------------------------------------ |
+| `api_key`                  | `str`                               | `LANGTRACE_API_KEY` or `None` | The API key for authentication.                                                |
+| `batch`                    | `bool`                              | `True`                        | Whether to batch spans before sending them.                                    |
+| `write_spans_to_console`   | `bool`                              | `False`                       | Whether to write spans to the console.                                         |
+| `custom_remote_exporter`   | `Optional[Exporter]`                | `None`                        | Custom remote exporter. If `None`, a default `LangTraceExporter` will be used. |
+| `api_host`                 | `Optional[str]`                     | `https://langtrace.ai/`       | The API host for the remote exporter.                                          |
+| `disable_instrumentations` | `Optional[DisableInstrumentations]` | `None`                        | You can pass an object to disable instrumentation for specific vendors ex: `{'only': ['openai']}` or `{'all_except': ['openai']}`
+
 ### Additional Customization
 
 - `@with_langtrace_root_span` - this decorator is designed to organize and relate different spans, in a hierarchical manner. When you're performing multiple operations that you want to monitor together as a unit, this function helps by establishing a "parent" (`LangtraceRootSpan` or whatever is passed to `name`) span. Then, any calls to the LLM APIs made within the given function (fn) will be considered "children" of this parent span. This setup is especially useful for tracking the performance or behavior of a group of operations collectively, rather than individually.
 
 ```python
 from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
 
@@ -181,15 +199,14 @@
         model="gpt-4",
         messages=[{"role": "user", "content": "Say this is a test three times"}],
         stream=False,
     )
     return response
 ```
 
-
 - `with_additional_attributes` - this function is designed to enhance the traces by adding custom attributes to the current context. These custom attributes provide extra details about the operations being performed, making it easier to analyze and understand their behavior.
 
 ```python
 from langtrace_python_sdk.utils.with_root_span import (
     with_langtrace_root_span,
     with_additional_attributes,
 )
@@ -218,15 +235,14 @@
 def chat_completion():
    api_call1()
    api_call2()
 ```
 
 - `get_prompt_from_registry` - this function is designed to fetch the desired prompt from the `Prompt Registry`. You can pass two options for filtering `prompt_version` & `variables`.
 
-
 ```python
 from langtrace_python_sdk import get_prompt_from_registry
 
 prompt = get_prompt_from_registry(<Registry ID>, options={"prompt_version": 1, "variables": {"foo": "bar"} })
 ```
 
 ## Supported integrations
```

