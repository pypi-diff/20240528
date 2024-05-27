# Comparing `tmp/memary-0.1.2.tar.gz` & `tmp/memary-0.1.3.tar.gz`

## Comparing `memary-0.1.2.tar` & `memary-0.1.3.tar`

### file list

```diff
@@ -1,109 +1,111 @@
--rw-r--r--   0        0        0    17450 2020-02-02 00:00:00.000000 memary-0.1.2/README.md
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 memary-0.1.2/requirements.txt
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/openrc
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/data/past_chat.json
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/data/system_persona.txt
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/data/user_persona.txt
--rw-r--r--   0        0        0    25928 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/data/chapter/1.txt
--rw-r--r--   0        0        0    19179 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/data/chapter/2.txt
--rw-r--r--   0        0        0    21567 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/data/chapter/3.txt
--rw-r--r--   0        0        0    20428 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/data/chapter/4.txt
--rw-r--r--   0        0        0    37700 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/data/chapter/5.txt
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/docs/update_021924.md
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/docs/update_022024.md
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/docs/update_022524.md
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/docs/update_022924.md
--rw-r--r--   0        0        0    81673 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/docs/src/0225_chapter1and2.png
--rw-r--r--   0        0        0   126281 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/docs/src/0225_update_with_chapter3.png
--rw-r--r--   0        0        0   180800 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/docs/src/GraphRAG.png
--rw-r--r--   0        0        0   161852 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/docs/src/chapter1_2.png
--rw-r--r--   0        0        0   197194 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/docs/src/chapter1_2_3.png
--rw-r--r--   0        0        0   106885 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/docs/src/memory_stream_Q1.png
--rw-r--r--   0        0        0   110531 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/docs/src/memory_stream_Q2.png
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2/default__vector_store.json
--rw-r--r--   0        0        0   152568 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2/docstore.json
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2/image__vector_store.json
--rw-r--r--   0        0        0     7487 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2/index_store.json
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2_3/default__vector_store.json
--rw-r--r--   0        0        0   450485 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2_3/docstore.json
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2_3/image__vector_store.json
--rw-r--r--   0        0        0    24222 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2_3/index_store.json
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2_3_4/default__vector_store.json
--rw-r--r--   0        0        0   521199 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2_3_4/docstore.json
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2_3_4/image__vector_store.json
--rw-r--r--   0        0        0    24667 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2_3_4/index_store.json
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/tests/memory/test_entity_knowledge_store.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/tests/memory/test_memory.json
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 memary-0.1.2/dev/KG_memory_stream/tests/memory/test_memory_stream.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 memary-0.1.2/dev/legacy_routing_agent/get_location.ipynb
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 memary-0.1.2/dev/legacy_routing_agent/main.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 memary-0.1.2/dev/legacy_routing_agent/ml.py
--rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 memary-0.1.2/dev/legacy_routing_agent/readme.md
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 memary-0.1.2/dev/legacy_routing_agent/tool_spec.ipynb
--rw-r--r--   0        0        0     7834 2020-02-02 00:00:00.000000 memary-0.1.2/dev/legacy_routing_agent/utils.py
--rw-r--r--   0        0        0     7269 2020-02-02 00:00:00.000000 memary-0.1.2/dev/query_decomposition/MS-SQ.ipynb
--rw-r--r--   0        0        0     8316 2020-02-02 00:00:00.000000 memary-0.1.2/dev/query_decomposition/MS_finetuning.ipynb
--rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 memary-0.1.2/dev/query_decomposition/SQ-MS.ipynb
--rw-r--r--   0        0        0    10205 2020-02-02 00:00:00.000000 memary-0.1.2/dev/query_decomposition/langchain_ms.ipynb
--rw-r--r--   0        0        0    12581 2020-02-02 00:00:00.000000 memary-0.1.2/dev/query_decomposition/routing_and_multistep.ipynb
--rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/external_perplexity.ipynb
--rw-r--r--   0        0        0    18983 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/recurse.ipynb
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/requirements.txt
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/benchmarking/benchmark.py
--rw-r--r--   0        0        0   109937 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/benchmarking/get_results.ipynb
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/benchmarking/judge.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/benchmarking/ollama_quality.ipynb
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/benchmarking/ollama_test.ipynb
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/benchmarking/output.py
--rw-r--r--   0        0        0     4542 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/benchmarking/perplexity_quality.ipynb
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/benchmarking/perplexity_test.ipynb
--rw-r--r--   0        0        0    25928 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/data/external_response.txt
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/docs/cypher.md
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/docs/implementation.md
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/docs/updates.md
--rw-r--r--   0        0        0   265458 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/docs/images/harry_subgraph.png
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/entity_extraction/entity_extraction.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/entity_extraction/output.py
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/langchain_retrieval/retrieve.ipynb
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/langchain_retrieval/retrieve.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/synonym_expand/output.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 memary-0.1.2/dev/recursive_retrieval/synonym_expand/synonym.py
--rw-r--r--   0        0        0    73358 2020-02-02 00:00:00.000000 memary-0.1.2/dev/reranking/Reranking.ipynb
--rw-r--r--   0        0        0   262686 2020-02-02 00:00:00.000000 memary-0.1.2/diagrams/final.png
--rw-r--r--   0        0        0   135432 2020-02-02 00:00:00.000000 memary-0.1.2/diagrams/kg.png
--rw-r--r--   0        0        0   123706 2020-02-02 00:00:00.000000 memary-0.1.2/diagrams/memary_logo.png
--rw-r--r--   0        0        0    94297 2020-02-02 00:00:00.000000 memary-0.1.2/diagrams/memory.png
--rw-r--r--   0        0        0    55143 2020-02-02 00:00:00.000000 memary-0.1.2/diagrams/memory_compression.png
--rw-r--r--   0        0        0    62869 2020-02-02 00:00:00.000000 memary-0.1.2/diagrams/memory_module.png
--rw-r--r--   0        0        0    26496 2020-02-02 00:00:00.000000 memary-0.1.2/diagrams/query_decomposition.png
--rw-r--r--   0        0        0    41373 2020-02-02 00:00:00.000000 memary-0.1.2/diagrams/reranking_diagram.png
--rw-r--r--   0        0        0    16029 2020-02-02 00:00:00.000000 memary-0.1.2/diagrams/routing_agent.png
--rw-r--r--   0        0        0   216730 2020-02-02 00:00:00.000000 memary-0.1.2/diagrams/system.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/agent/__init__.py
--rw-r--r--   0        0        0    16844 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/agent/base_agent.py
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/agent/chat_agent.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/agent/data_types.py
--rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/agent/llm_api/tools.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/memory/__init__.py
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/memory/base_memory.py
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/memory/entity_knowledge_store.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/memory/memory_stream.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/memory/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/synonym_expand/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/synonym_expand/output.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 memary-0.1.2/src/memary/synonym_expand/synonym.py
--rw-r--r--   0        0        0     7671 2020-02-02 00:00:00.000000 memary-0.1.2/streamlit_app/app.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 memary-0.1.2/streamlit_app/data/entity_knowledge_store.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 memary-0.1.2/streamlit_app/data/external_response.txt
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 memary-0.1.2/streamlit_app/data/memory_stream.json
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 memary-0.1.2/streamlit_app/data/past_chat.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 memary-0.1.2/streamlit_app/data/routing_response.txt
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 memary-0.1.2/streamlit_app/data/system_persona.txt
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 memary-0.1.2/streamlit_app/data/user_persona.txt
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 memary-0.1.2/streamlit_app/data/user_persona_template.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 memary-0.1.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 memary-0.1.2/LICENSE
--rw-r--r--   0        0        0    15882 2020-02-02 00:00:00.000000 memary-0.1.2/README_hidden.md
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 memary-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    17449 2020-02-02 00:00:00.000000 memary-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    18578 2020-02-02 00:00:00.000000 memary-0.1.3/README.md
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 memary-0.1.3/requirements.txt
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/openrc
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/data/past_chat.json
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/data/system_persona.txt
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/data/user_persona.txt
+-rw-r--r--   0        0        0    25928 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/data/chapter/1.txt
+-rw-r--r--   0        0        0    19179 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/data/chapter/2.txt
+-rw-r--r--   0        0        0    21567 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/data/chapter/3.txt
+-rw-r--r--   0        0        0    20428 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/data/chapter/4.txt
+-rw-r--r--   0        0        0    37700 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/data/chapter/5.txt
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/docs/update_021924.md
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/docs/update_022024.md
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/docs/update_022524.md
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/docs/update_022924.md
+-rw-r--r--   0        0        0    81673 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/docs/src/0225_chapter1and2.png
+-rw-r--r--   0        0        0   126281 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/docs/src/0225_update_with_chapter3.png
+-rw-r--r--   0        0        0   180800 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/docs/src/GraphRAG.png
+-rw-r--r--   0        0        0   161852 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/docs/src/chapter1_2.png
+-rw-r--r--   0        0        0   197194 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/docs/src/chapter1_2_3.png
+-rw-r--r--   0        0        0   106885 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/docs/src/memory_stream_Q1.png
+-rw-r--r--   0        0        0   110531 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/docs/src/memory_stream_Q2.png
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/storage_graph/ch1_2/default__vector_store.json
+-rw-r--r--   0        0        0   152568 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/storage_graph/ch1_2/docstore.json
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/storage_graph/ch1_2/image__vector_store.json
+-rw-r--r--   0        0        0     7487 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/storage_graph/ch1_2/index_store.json
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/storage_graph/ch1_2_3/default__vector_store.json
+-rw-r--r--   0        0        0   450485 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/storage_graph/ch1_2_3/docstore.json
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/storage_graph/ch1_2_3/image__vector_store.json
+-rw-r--r--   0        0        0    24222 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/storage_graph/ch1_2_3/index_store.json
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/storage_graph/ch1_2_3_4/default__vector_store.json
+-rw-r--r--   0        0        0   521199 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/storage_graph/ch1_2_3_4/docstore.json
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/storage_graph/ch1_2_3_4/image__vector_store.json
+-rw-r--r--   0        0        0    24667 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/storage_graph/ch1_2_3_4/index_store.json
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/tests/memory/test_entity_knowledge_store.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/tests/memory/test_memory.json
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 memary-0.1.3/dev/KG_memory_stream/tests/memory/test_memory_stream.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 memary-0.1.3/dev/legacy_routing_agent/get_location.ipynb
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 memary-0.1.3/dev/legacy_routing_agent/main.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 memary-0.1.3/dev/legacy_routing_agent/ml.py
+-rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 memary-0.1.3/dev/legacy_routing_agent/readme.md
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 memary-0.1.3/dev/legacy_routing_agent/tool_spec.ipynb
+-rw-r--r--   0        0        0     7834 2020-02-02 00:00:00.000000 memary-0.1.3/dev/legacy_routing_agent/utils.py
+-rw-r--r--   0        0        0     7269 2020-02-02 00:00:00.000000 memary-0.1.3/dev/query_decomposition/MS-SQ.ipynb
+-rw-r--r--   0        0        0     8316 2020-02-02 00:00:00.000000 memary-0.1.3/dev/query_decomposition/MS_finetuning.ipynb
+-rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 memary-0.1.3/dev/query_decomposition/SQ-MS.ipynb
+-rw-r--r--   0        0        0    10205 2020-02-02 00:00:00.000000 memary-0.1.3/dev/query_decomposition/langchain_ms.ipynb
+-rw-r--r--   0        0        0    12581 2020-02-02 00:00:00.000000 memary-0.1.3/dev/query_decomposition/routing_and_multistep.ipynb
+-rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 memary-0.1.3/dev/recursive_retrieval/external_perplexity.ipynb
+-rw-r--r--   0        0        0    18983 2020-02-02 00:00:00.000000 memary-0.1.3/dev/recursive_retrieval/recurse.ipynb
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 memary-0.1.3/dev/recursive_retrieval/requirements.txt
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 memary-0.1.3/dev/recursive_retrieval/benchmarking/benchmark.py
+-rw-r--r--   0        0        0   109937 2020-02-02 00:00:00.000000 memary-0.1.3/dev/recursive_retrieval/benchmarking/get_results.ipynb
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 memary-0.1.3/dev/recursive_retrieval/benchmarking/judge.py
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 memary-0.1.3/dev/recursive_retrieval/benchmarking/ollama_quality.ipynb
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 memary-0.1.3/dev/recursive_retrieval/benchmarking/ollama_test.ipynb
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 memary-0.1.3/dev/recursive_retrieval/benchmarking/output.py
+-rw-r--r--   0        0        0     4542 2020-02-02 00:00:00.000000 memary-0.1.3/dev/recursive_retrieval/benchmarking/perplexity_quality.ipynb
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 memary-0.1.3/dev/recursive_retrieval/benchmarking/perplexity_test.ipynb
+-rw-r--r--   0        0        0    25928 2020-02-02 00:00:00.000000 memary-0.1.3/dev/recursive_retrieval/data/external_response.txt
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 memary-0.1.3/dev/recursive_retrieval/docs/cypher.md
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 memary-0.1.3/dev/recursive_retrieval/docs/implementation.md
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 memary-0.1.3/dev/recursive_retrieval/docs/updates.md
+-rw-r--r--   0        0        0   265458 2020-02-02 00:00:00.000000 memary-0.1.3/dev/recursive_retrieval/docs/images/harry_subgraph.png
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 memary-0.1.3/dev/recursive_retrieval/entity_extraction/entity_extraction.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 memary-0.1.3/dev/recursive_retrieval/entity_extraction/output.py
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 memary-0.1.3/dev/recursive_retrieval/langchain_retrieval/retrieve.ipynb
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 memary-0.1.3/dev/recursive_retrieval/langchain_retrieval/retrieve.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 memary-0.1.3/dev/recursive_retrieval/synonym_expand/output.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 memary-0.1.3/dev/recursive_retrieval/synonym_expand/synonym.py
+-rw-r--r--   0        0        0    73358 2020-02-02 00:00:00.000000 memary-0.1.3/dev/reranking/Reranking.ipynb
+-rw-r--r--   0        0        0   162023 2020-02-02 00:00:00.000000 memary-0.1.3/diagrams/context_window.png
+-rw-r--r--   0        0        0   262686 2020-02-02 00:00:00.000000 memary-0.1.3/diagrams/final.png
+-rw-r--r--   0        0        0   135432 2020-02-02 00:00:00.000000 memary-0.1.3/diagrams/kg.png
+-rw-r--r--   0        0        0   123706 2020-02-02 00:00:00.000000 memary-0.1.3/diagrams/memary_logo.png
+-rw-r--r--   0        0        0    49173 2020-02-02 00:00:00.000000 memary-0.1.3/diagrams/memary_logo_bw.png
+-rw-r--r--   0        0        0    94297 2020-02-02 00:00:00.000000 memary-0.1.3/diagrams/memory.png
+-rw-r--r--   0        0        0    55143 2020-02-02 00:00:00.000000 memary-0.1.3/diagrams/memory_compression.png
+-rw-r--r--   0        0        0    62869 2020-02-02 00:00:00.000000 memary-0.1.3/diagrams/memory_module.png
+-rw-r--r--   0        0        0    26496 2020-02-02 00:00:00.000000 memary-0.1.3/diagrams/query_decomposition.png
+-rw-r--r--   0        0        0    41373 2020-02-02 00:00:00.000000 memary-0.1.3/diagrams/reranking_diagram.png
+-rw-r--r--   0        0        0    16029 2020-02-02 00:00:00.000000 memary-0.1.3/diagrams/routing_agent.png
+-rw-r--r--   0        0        0   216730 2020-02-02 00:00:00.000000 memary-0.1.3/diagrams/system.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 memary-0.1.3/src/memary/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 memary-0.1.3/src/memary/agent/__init__.py
+-rw-r--r--   0        0        0    18318 2020-02-02 00:00:00.000000 memary-0.1.3/src/memary/agent/base_agent.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 memary-0.1.3/src/memary/agent/chat_agent.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 memary-0.1.3/src/memary/agent/data_types.py
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 memary-0.1.3/src/memary/agent/llm_api/tools.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 memary-0.1.3/src/memary/memory/__init__.py
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 memary-0.1.3/src/memary/memory/base_memory.py
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 memary-0.1.3/src/memary/memory/entity_knowledge_store.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 memary-0.1.3/src/memary/memory/memory_stream.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 memary-0.1.3/src/memary/memory/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 memary-0.1.3/src/memary/synonym_expand/__init__.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 memary-0.1.3/src/memary/synonym_expand/output.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 memary-0.1.3/src/memary/synonym_expand/synonym.py
+-rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 memary-0.1.3/streamlit_app/app.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 memary-0.1.3/streamlit_app/data/entity_knowledge_store.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 memary-0.1.3/streamlit_app/data/external_response.txt
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 memary-0.1.3/streamlit_app/data/memory_stream.json
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 memary-0.1.3/streamlit_app/data/past_chat.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 memary-0.1.3/streamlit_app/data/routing_response.txt
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 memary-0.1.3/streamlit_app/data/system_persona.txt
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 memary-0.1.3/streamlit_app/data/user_persona.txt
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 memary-0.1.3/streamlit_app/data/user_persona_template.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 memary-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 memary-0.1.3/LICENSE
+-rw-r--r--   0        0        0    16942 2020-02-02 00:00:00.000000 memary-0.1.3/README_hidden.md
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 memary-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    18531 2020-02-02 00:00:00.000000 memary-0.1.3/PKG-INFO
```

### Comparing `memary-0.1.2/README.md` & `memary-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -36,16 +36,16 @@
    2. Install Python dependencies:
    ```
    pip install -r requirements.txt
    ```
 
 ## Demo
 **Notes:** memary currently assumes the local installation method and currently supports any models available through Ollama:
-- LLM running locally using Ollama **OR** `gpt-3.5-turbo`
-- Vision model running locally using Ollama **OR** `gpt-4-vision-preview`
+- LLM running locally using Ollama (Llama 3 8B/40B as suggested defaults) **OR** `gpt-3.5-turbo`
+- Vision model running locally using Ollama (LLaVA as suggested default) **OR** `gpt-4-vision-preview`
 
 memary will default to the locally run models unless explicitly specified.
 
 **To run the Streamlit app:**
 1. [Optional] If running models locally using Ollama, follow this the instructions in this [repo](https://github.com/ollama/ollama).
 
 2. Ensure that a `.env` exists with any necessary API keys and Neo4j credentials.
@@ -85,14 +85,48 @@
 6. Run:
 
 ```
 cd streamlit_app
 streamlit run app.py
 ```
 
+## Usage
+```python
+from memary.agent.chat_agent import ChatAgent
+
+system_persona_txt = "data/system_persona.txt"
+user_persona_txt = "data/user_persona.txt"
+past_chat_json = "data/past_chat.json"
+memory_stream_json = "data/memory_stream.json"
+entity_knowledge_store_json = "data/entity_knowledge_store.json"
+chat_agent = ChatAgent(
+    "Personal Agent",
+    memory_stream_json,
+    entity_knowledge_store_json,
+    system_persona_txt,
+    user_persona_txt,
+    past_chat_json,
+)
+```
+Pass in subset of `['search', 'vision', 'locate', 'stocks']` as `include_from_defaults` for different set of default tools upon initialization.
+### Adding Custom Tools
+```python
+def multiply(a: int, b: int) -> int:
+    """Multiply two integers and returns the result integer"""
+    return a * b
+
+chat_agent.add_tool({"multiply": multiply})
+```
+More information about creating custom tools for the LlamaIndex ReAct Agent  can be found [here](https://docs.llamaindex.ai/en/stable/examples/agent/react_agent/).
+
+### Removing Tools
+```python
+chat_agent.remove_tool("multiply")
+```
+
 ## Detailed Component Breakdown
 
 ### Routing Agent
 
 ![agent diagram](diagrams/routing_agent.png)
 
 - Uses the [ReAct agent](https://react-lm.github.io/) to plan and execute a query given the tools provided. This type of agent can reason over which of the tools to use next to further the response, feed inputs into the selected tool, and repeat the process with the output until it determines that the answer is satisfactory.
```

### Comparing `memary-0.1.2/requirements.txt` & `memary-0.1.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/data/system_persona.txt` & `memary-0.1.3/dev/KG_memory_stream/data/system_persona.txt`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/data/user_persona.txt` & `memary-0.1.3/dev/KG_memory_stream/data/user_persona.txt`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/data/chapter/1.txt` & `memary-0.1.3/dev/KG_memory_stream/data/chapter/1.txt`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/data/chapter/2.txt` & `memary-0.1.3/dev/KG_memory_stream/data/chapter/2.txt`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/data/chapter/3.txt` & `memary-0.1.3/dev/KG_memory_stream/data/chapter/3.txt`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/data/chapter/4.txt` & `memary-0.1.3/dev/KG_memory_stream/data/chapter/4.txt`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/data/chapter/5.txt` & `memary-0.1.3/dev/KG_memory_stream/data/chapter/5.txt`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/docs/update_021924.md` & `memary-0.1.3/dev/KG_memory_stream/docs/update_021924.md`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/docs/update_022024.md` & `memary-0.1.3/dev/KG_memory_stream/docs/update_022024.md`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/docs/update_022524.md` & `memary-0.1.3/dev/KG_memory_stream/docs/update_022524.md`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/docs/update_022924.md` & `memary-0.1.3/dev/KG_memory_stream/docs/update_022924.md`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/docs/src/0225_chapter1and2.png` & `memary-0.1.3/dev/KG_memory_stream/docs/src/0225_chapter1and2.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/docs/src/0225_update_with_chapter3.png` & `memary-0.1.3/dev/KG_memory_stream/docs/src/0225_update_with_chapter3.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/docs/src/GraphRAG.png` & `memary-0.1.3/dev/KG_memory_stream/docs/src/GraphRAG.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/docs/src/chapter1_2.png` & `memary-0.1.3/dev/KG_memory_stream/docs/src/chapter1_2.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/docs/src/chapter1_2_3.png` & `memary-0.1.3/dev/KG_memory_stream/docs/src/chapter1_2_3.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/docs/src/memory_stream_Q1.png` & `memary-0.1.3/dev/KG_memory_stream/docs/src/memory_stream_Q1.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/docs/src/memory_stream_Q2.png` & `memary-0.1.3/dev/KG_memory_stream/docs/src/memory_stream_Q2.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2/docstore.json` & `memary-0.1.3/dev/KG_memory_stream/storage_graph/ch1_2/docstore.json`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2/index_store.json` & `memary-0.1.3/dev/KG_memory_stream/storage_graph/ch1_2/index_store.json`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2_3/docstore.json` & `memary-0.1.3/dev/KG_memory_stream/storage_graph/ch1_2_3/docstore.json`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2_3/index_store.json` & `memary-0.1.3/dev/KG_memory_stream/storage_graph/ch1_2_3/index_store.json`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2_3_4/docstore.json` & `memary-0.1.3/dev/KG_memory_stream/storage_graph/ch1_2_3_4/docstore.json`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/storage_graph/ch1_2_3_4/index_store.json` & `memary-0.1.3/dev/KG_memory_stream/storage_graph/ch1_2_3_4/index_store.json`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/tests/memory/test_entity_knowledge_store.py` & `memary-0.1.3/dev/KG_memory_stream/tests/memory/test_entity_knowledge_store.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/KG_memory_stream/tests/memory/test_memory_stream.py` & `memary-0.1.3/dev/KG_memory_stream/tests/memory/test_memory_stream.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/legacy_routing_agent/get_location.ipynb` & `memary-0.1.3/dev/legacy_routing_agent/get_location.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/legacy_routing_agent/main.py` & `memary-0.1.3/dev/legacy_routing_agent/main.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/legacy_routing_agent/ml.py` & `memary-0.1.3/dev/legacy_routing_agent/ml.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/legacy_routing_agent/readme.md` & `memary-0.1.3/dev/legacy_routing_agent/readme.md`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/legacy_routing_agent/tool_spec.ipynb` & `memary-0.1.3/dev/legacy_routing_agent/tool_spec.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/legacy_routing_agent/utils.py` & `memary-0.1.3/dev/legacy_routing_agent/utils.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/query_decomposition/MS-SQ.ipynb` & `memary-0.1.3/dev/query_decomposition/MS-SQ.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/query_decomposition/MS_finetuning.ipynb` & `memary-0.1.3/dev/query_decomposition/MS_finetuning.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/query_decomposition/SQ-MS.ipynb` & `memary-0.1.3/dev/query_decomposition/SQ-MS.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/query_decomposition/langchain_ms.ipynb` & `memary-0.1.3/dev/query_decomposition/langchain_ms.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/query_decomposition/routing_and_multistep.ipynb` & `memary-0.1.3/dev/query_decomposition/routing_and_multistep.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/recursive_retrieval/external_perplexity.ipynb` & `memary-0.1.3/dev/recursive_retrieval/external_perplexity.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/recursive_retrieval/recurse.ipynb` & `memary-0.1.3/dev/recursive_retrieval/recurse.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/recursive_retrieval/requirements.txt` & `memary-0.1.3/dev/recursive_retrieval/requirements.txt`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/recursive_retrieval/benchmarking/benchmark.py` & `memary-0.1.3/dev/recursive_retrieval/benchmarking/benchmark.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/recursive_retrieval/benchmarking/get_results.ipynb` & `memary-0.1.3/dev/recursive_retrieval/benchmarking/get_results.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/recursive_retrieval/benchmarking/judge.py` & `memary-0.1.3/dev/recursive_retrieval/benchmarking/judge.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/recursive_retrieval/benchmarking/ollama_quality.ipynb` & `memary-0.1.3/dev/recursive_retrieval/benchmarking/ollama_quality.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/recursive_retrieval/benchmarking/ollama_test.ipynb` & `memary-0.1.3/dev/recursive_retrieval/benchmarking/ollama_test.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/recursive_retrieval/benchmarking/output.py` & `memary-0.1.3/dev/recursive_retrieval/benchmarking/output.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/recursive_retrieval/benchmarking/perplexity_quality.ipynb` & `memary-0.1.3/dev/recursive_retrieval/benchmarking/perplexity_quality.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/recursive_retrieval/benchmarking/perplexity_test.ipynb` & `memary-0.1.3/dev/recursive_retrieval/benchmarking/perplexity_test.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/recursive_retrieval/data/external_response.txt` & `memary-0.1.3/dev/recursive_retrieval/data/external_response.txt`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/recursive_retrieval/docs/updates.md` & `memary-0.1.3/dev/recursive_retrieval/docs/updates.md`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/recursive_retrieval/docs/images/harry_subgraph.png` & `memary-0.1.3/dev/recursive_retrieval/docs/images/harry_subgraph.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/recursive_retrieval/entity_extraction/entity_extraction.py` & `memary-0.1.3/dev/recursive_retrieval/entity_extraction/entity_extraction.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/recursive_retrieval/langchain_retrieval/retrieve.ipynb` & `memary-0.1.3/dev/recursive_retrieval/langchain_retrieval/retrieve.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/recursive_retrieval/langchain_retrieval/retrieve.py` & `memary-0.1.3/dev/recursive_retrieval/langchain_retrieval/retrieve.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/recursive_retrieval/synonym_expand/synonym.py` & `memary-0.1.3/dev/recursive_retrieval/synonym_expand/synonym.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/dev/reranking/Reranking.ipynb` & `memary-0.1.3/dev/reranking/Reranking.ipynb`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/diagrams/final.png` & `memary-0.1.3/diagrams/final.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/diagrams/kg.png` & `memary-0.1.3/diagrams/kg.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/diagrams/memary_logo.png` & `memary-0.1.3/diagrams/memary_logo.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/diagrams/memory.png` & `memary-0.1.3/diagrams/memory.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/diagrams/memory_compression.png` & `memary-0.1.3/diagrams/memory_compression.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/diagrams/memory_module.png` & `memary-0.1.3/diagrams/memory_module.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/diagrams/query_decomposition.png` & `memary-0.1.3/diagrams/query_decomposition.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/diagrams/reranking_diagram.png` & `memary-0.1.3/diagrams/reranking_diagram.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/diagrams/routing_agent.png` & `memary-0.1.3/diagrams/routing_agent.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/diagrams/system.png` & `memary-0.1.3/diagrams/system.png`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/src/memary/agent/base_agent.py` & `memary-0.1.3/src/memary/agent/base_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 import logging
 import os
 import sys
 from pathlib import Path
+from typing import Any, Callable, Dict, List
 
 import geocoder
 import googlemaps
 import numpy as np
 import requests
 from ansistrip import ansi_strip
 from dotenv import load_dotenv
-from llama_index.core import (
-    KnowledgeGraphIndex,
-    Settings,
-    SimpleDirectoryReader,
-    StorageContext,
-)
+from llama_index.core import (KnowledgeGraphIndex, Settings,
+                              SimpleDirectoryReader, StorageContext)
 from llama_index.core.agent import ReActAgent
 from llama_index.core.llms import ChatMessage
 from llama_index.core.query_engine import RetrieverQueryEngine
 from llama_index.core.retrievers import KnowledgeGraphRAGRetriever
 from llama_index.core.tools import FunctionTool
 from llama_index.graph_stores.neo4j import Neo4jGraphStore
 from llama_index.llms.ollama import Ollama
 from llama_index.llms.openai import OpenAI
 from llama_index.llms.perplexity import Perplexity
 from llama_index.multi_modal_llms.ollama import OllamaMultiModal
 from llama_index.multi_modal_llms.openai import OpenAIMultiModal
 
 from memary.agent.data_types import Context, Message
-from memary.agent.llm_api.tools import (
-    ollama_chat_completions_request,
-    openai_chat_completions_request,
-)
+from memary.agent.llm_api.tools import (ollama_chat_completions_request,
+                                        openai_chat_completions_request)
 from memary.memory import EntityKnowledgeStore, MemoryStream
 from memary.synonym_expand.synonym import custom_synonym_expand_fn
 
 MAX_ENTITIES_FROM_KG = 5
 ENTITY_EXCEPTIONS = ["Unknown relation"]
 # LLM token limits
 CONTEXT_LENGTH = 4096
@@ -61,14 +56,15 @@
         memory_stream_json,
         entity_knowledge_store_json,
         system_persona_txt,
         user_persona_txt,
         past_chat_json,
         llm_model_name="llama3",
         vision_model_name="llava",
+        include_from_defaults=["search", "locate", "vision", "stocks"],
         debug=True,
     ):
         load_dotenv()
         self.name = name
         self.model = llm_model_name
 
         googlemaps_api_key = os.getenv("GOOGLEMAPS_API_KEY")
@@ -95,15 +91,14 @@
             username=self.neo4j_username,
             password=self.neo4j_password,
             url=self.neo4j_url,
             database=database,
         )
 
         self.vantage_key = os.getenv("ALPHA_VANTAGE_API_KEY")
-        # self.news_data_key = os.getenv("NEWS_DATA_API_KEY")
 
         self.storage_context = StorageContext.from_defaults(
             graph_store=self.graph_store
         )
         graph_rag_retriever = KnowledgeGraphRAGRetriever(
             storage_context=self.storage_context,
             verbose=True,
@@ -112,26 +107,17 @@
             synonym_expand_fn=custom_synonym_expand_fn,
         )
 
         self.query_engine = RetrieverQueryEngine.from_args(
             graph_rag_retriever,
         )
 
-        search_tool = FunctionTool.from_defaults(fn=self.search)
-        locate_tool = FunctionTool.from_defaults(fn=self.locate)
-        vision_tool = FunctionTool.from_defaults(fn=self.vision)
-        stock_tool = FunctionTool.from_defaults(fn=self.stock_price)
-        # news_tool = FunctionTool.from_defaults(fn=self.get_news)
-
         self.debug = debug
-        self.routing_agent = ReActAgent.from_tools(
-            [search_tool, locate_tool, vision_tool, stock_tool],
-            llm=self.llm,
-            verbose=True,
-        )
+        self.tools = {}
+        self._init_default_tools(default_tools=include_from_defaults)
 
         self.memory_stream = MemoryStream(memory_stream_json)
         self.entity_knowledge_store = EntityKnowledgeStore(entity_knowledge_store_json)
 
         self.message = Message(
             system_persona_txt, user_persona_txt, past_chat_json, self.model
         )
@@ -207,15 +193,15 @@
         image_documents = SimpleDirectoryReader(query_image_dir_path).load_data()
 
         response = self.mm_model.complete(prompt=query, image_documents=image_documents)
 
         os.remove(query_image_path)  # delete image after use
         return response
 
-    def stock_price(self, query: str) -> str:
+    def stocks(self, query: str) -> str:
         """Get the stock price of the company given the ticker"""
         request_api = requests.get(
             r"https://www.alphavantage.co/query?function=GLOBAL_QUOTE&symbol="
             + query
             + r"&apikey="
             + self.vantage_key
         )
@@ -431,23 +417,71 @@
                 break
         entities = list(set(entities))
         for exceptions in ENTITY_EXCEPTIONS:
             if exceptions in entities:
                 entities.remove(exceptions)
         return entities
 
-    def update_tools(self, updatedTools):
-        print("recieved update tools")
-        tools = []
-        for tool in updatedTools:
-            if tool == "Search":
-                tools.append(FunctionTool.from_defaults(fn=self.search))
-            elif tool == "Location":
-                tools.append(FunctionTool.from_defaults(fn=self.locate))
-            elif tool == "Vision":
-                tools.append(FunctionTool.from_defaults(fn=self.vision))
-            elif tool == "Stocks":
-                tools.append(FunctionTool.from_defaults(fn=self.stock_price))
-            # elif tool == "News":
-            #     tools.append(FunctionTool.from_defaults(fn=self.get_news))
+    def _init_ReAct_agent(self):
+        """Initializes ReAct Agent with list of tools in self.tools."""
+        tool_fns = []
+        for func in self.tools.values():
+            tool_fns.append(FunctionTool.from_defaults(fn=func))
+        self.routing_agent = ReActAgent.from_tools(tool_fns, llm=self.llm, verbose=True)
+
+    def _init_default_tools(self, default_tools: List[str]):
+        """Initializes ReAct Agent from the default list of tools memary provides.
+        List of strings passed in during initialization denoting which default tools to include.
+        Args:
+            default_tools (list(str)): list of tool names in string form
+        """
+
+        for tool in default_tools:
+            if tool == "search":
+                self.tools["search"] = self.search
+            elif tool == "locate":
+                self.tools["locate"] = self.locate
+            elif tool == "vision":
+                self.tools["vision"] = self.vision
+            elif tool == "stocks":
+                self.tools["stocks"] = self.stocks
+        self._init_ReAct_agent()
+
+    def add_tool(self, tool_additions: Dict[str, Callable[..., Any]]):
+        """Adds specified tools to be used by the ReAct Agent.
+        Args:
+            tools (dict(str, func)): dictionary of tools with names as keys and associated functions as values
+        """
+
+        for tool_name in tool_additions:
+            self.tools[tool_name] = tool_additions[tool_name]
+        self._init_ReAct_agent()
+
+    def remove_tool(self, tool_name: str):
+        """Removes specified tool from list of available tools for use by the ReAct Agent.
+        Args:
+            tool_name (str): name of tool to be removed in string form
+        """
+
+        if tool_name in self.tools:
+            del self.tools[tool_name]
+            self._init_ReAct_agent()
+        else:
+            raise ("Unknown tool_name provided for removal.")
+
+    def update_tools(self, updated_tools: List[str]):
+        """Resets ReAct Agent tools to only include subset of default tools.
+        Args:
+            updated_tools (list(str)): list of default tools to include
+        """
 
-        self.routing_agent = ReActAgent.from_tools(tools, llm=self.llm, verbose=True)
+        self.tools.clear()
+        for tool in updated_tools:
+            if tool == "search":
+                self.tools["search"] = self.search
+            elif tool == "locate":
+                self.tools["locate"] = self.locate
+            elif tool == "vision":
+                self.tools["vision"] = self.vision
+            elif tool == "stocks":
+                self.tools["stocks"] = self.stocks
+        self._init_ReAct_agent()
```

### Comparing `memary-0.1.2/src/memary/agent/chat_agent.py` & `memary-0.1.3/src/memary/agent/chat_agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,83 @@
 from typing import Optional, List
 
 from memary.agent.base_agent import Agent
+import logging
 
 
 class ChatAgent(Agent):
     """ChatAgent currently able to support Llama3 running on Ollama (default) and gpt-3.5-turbo for llm models,
     and LLaVA running on Ollama (default) and gpt-4-vision-preview for the vision tool.
     """
-    def __init__(self, name, memory_stream_json, entity_knowledge_store_json,
-                 system_persona_txt, user_persona_txt, past_chat_json, llm_model_name="llama3", vision_model_name="llava"):
-        super().__init__(name, memory_stream_json, entity_knowledge_store_json,
-                         system_persona_txt, user_persona_txt, past_chat_json, llm_model_name, vision_model_name)
-        
-
-    def add_chat(self,
-                 role: str,
-                 content: str,
-                 entities: Optional[List[str]] = None):
+
+    def __init__(
+        self,
+        name,
+        memory_stream_json,
+        entity_knowledge_store_json,
+        system_persona_txt,
+        user_persona_txt,
+        past_chat_json,
+        llm_model_name="llama3",
+        vision_model_name="llava",
+        include_from_defaults=["search", "locate", "vision", "stocks"],
+    ):
+        super().__init__(
+            name,
+            memory_stream_json,
+            entity_knowledge_store_json,
+            system_persona_txt,
+            user_persona_txt,
+            past_chat_json,
+            llm_model_name,
+            vision_model_name,
+            include_from_defaults,
+        )
+
+    def add_chat(self, role: str, content: str, entities: Optional[List[str]] = None):
         """Add a chat to the agent's memory.
 
         Args:
             role (str): 'system' or 'user'
             content (str): content of the chat
             entities (Optional[List[str]], optional): entities from Memory systems. Defaults to None.
         """
         # Add a chat to the agent's memory.
         self._add_contexts_to_llm_message(role, content)
 
         if entities:
             self.memory_stream.add_memory(entities)
             self.memory_stream.save_memory()
-            self.entity_knowledge_store.add_memory(
-                self.memory_stream.get_memory())
+            self.entity_knowledge_store.add_memory(self.memory_stream.get_memory())
             self.entity_knowledge_store.save_memory()
 
         self._replace_memory_from_llm_message()
         self._replace_eks_to_from_message()
 
     def get_chat(self):
         return self.contexts
 
     def clearMemory(self):
+        """Clears Neo4j database and memory stream/entity knowledge store."""
+
+        logging.info("Deleting memory stream and entity knowledge store...")
         self.memory_stream.clear_memory()
         self.entity_knowledge_store.clear_memory()
-        
-       # print("removed from mem stream and entity knowdlege store ")
-        "clears knowledge neo4j database"
 
-        print("Deleting nodes from Neo4j...")
+        logging.info("Deleting nodes from Neo4j...")
         try:
             self.graph_store.query("MATCH (n) DETACH DELETE n")
         except Exception as e:
-            print(f"Error deleting nodes: {e}")
-        print("Nodes deleted from Neo4j.")
+            logging.error(f"Error deleting nodes: {e}")
+        logging.info("Nodes deleted from Neo4j.")
 
     def _replace_memory_from_llm_message(self):
         """Replace the memory_stream from the llm_message."""
-        self.message.llm_message[
-            "memory_stream"] = self.memory_stream.get_memory()
+        self.message.llm_message["memory_stream"] = self.memory_stream.get_memory()
 
     def _replace_eks_to_from_message(self):
         """Replace the entity knowledge store from the llm_message.
         eks = entity knowledge store"""
 
-        self.message.llm_message[
-            "knowledge_entity_store"] = self.entity_knowledge_store.get_memory(
-            )
+        self.message.llm_message["knowledge_entity_store"] = (
+            self.entity_knowledge_store.get_memory()
+        )
```

### Comparing `memary-0.1.2/src/memary/agent/data_types.py` & `memary-0.1.3/src/memary/agent/data_types.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/src/memary/agent/llm_api/tools.py` & `memary-0.1.3/src/memary/agent/llm_api/tools.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/src/memary/memory/base_memory.py` & `memary-0.1.3/src/memary/memory/base_memory.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/src/memary/memory/entity_knowledge_store.py` & `memary-0.1.3/src/memary/memory/entity_knowledge_store.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/src/memary/memory/memory_stream.py` & `memary-0.1.3/src/memary/memory/memory_stream.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/src/memary/memory/types.py` & `memary-0.1.3/src/memary/memory/types.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/src/memary/synonym_expand/synonym.py` & `memary-0.1.3/src/memary/synonym_expand/synonym.py`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/streamlit_app/app.py` & `memary-0.1.3/streamlit_app/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,21 +132,20 @@
 
     st.write(" ")
     clear_memory = st.button("Clear Memory DB")
     query = st.text_input("Ask a question")
 
     tools = st.multiselect(
         "Select tools to include:",
-        # ["Search", "Location", "Vision", "Stocks", "News"], #all options available
-        # ["Search", "Location", "Vision", "Stocks", "News"],) #options that are selected by default
-        ["Search", "Location", "Vision", "Stocks"],  # all options available
-        ["Search", "Location", "Vision", "Stocks"],
-    )  # options that are selected by default
+        ["search", "locate", "vision", "stocks"], # all options available
+        ["search", "locate", "vision", "stocks"], # options that are selected by default
+    )  
 
-    if "Vision" in tools:
+    img_url = ""
+    if "vision" in tools:
         img_url = st.text_input("URL of image, leave blank if no image to provide")
         if img_url:
             st.image(img_url, caption="Uploaded Image", use_column_width=True)
 
     generate_clicked = st.button("Generate")
     st.write("")
 
@@ -163,15 +162,14 @@
 
         # get tools
         print("tools enabled: ", tools)
         if len(tools) == 0:
             st.write("Please select at least one tool")
             st.stop()
 
-        print("start update tools")
         chat_agent.update_tools(tools)
 
         if img_url:
             query += "Image URL: " + img_url
         react_response = ""
         rag_response = (
             "There was no information in knowledge_graph to answer your question."
```

### Comparing `memary-0.1.2/streamlit_app/data/system_persona.txt` & `memary-0.1.3/streamlit_app/data/system_persona.txt`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/streamlit_app/data/user_persona.txt` & `memary-0.1.3/streamlit_app/data/user_persona.txt`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/streamlit_app/data/user_persona_template.txt` & `memary-0.1.3/streamlit_app/data/user_persona_template.txt`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/LICENSE` & `memary-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `memary-0.1.2/README_hidden.md` & `memary-0.1.3/README_hidden.md`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,48 @@
 6. Run:
 
 ```
 cd streamlit_app
 streamlit run app.py
 ```
 
+## Usage
+```python
+from memary.agent.chat_agent import ChatAgent
+
+system_persona_txt = "data/system_persona.txt"
+user_persona_txt = "data/user_persona.txt"
+past_chat_json = "data/past_chat.json"
+memory_stream_json = "data/memory_stream.json"
+entity_knowledge_store_json = "data/entity_knowledge_store.json"
+chat_agent = ChatAgent(
+    "Personal Agent",
+    memory_stream_json,
+    entity_knowledge_store_json,
+    system_persona_txt,
+    user_persona_txt,
+    past_chat_json,
+)
+```
+Pass in subset of `['search', 'vision', 'locate', 'stocks']` as `include_from_defaults` for different set of default tools upon initialization.
+### Adding Custom Tools
+```python
+def multiply(a: int, b: int) -> int:
+    """Multiply two integers and returns the result integer"""
+    return a * b
+
+chat_agent.add_tool({"multiply": multiply})
+```
+More information about creating custom tools for the LlamaIndex ReAct Agent  can be found [here](https://docs.llamaindex.ai/en/stable/examples/agent/react_agent/).
+
+### Removing Tools
+```python
+chat_agent.remove_tool("multiply")
+```
+
 ## Detailed Component Breakdown
 
 ### Routing Agent
 
 - Uses the [ReAct agent](https://react-lm.github.io/) to plan and execute a query given the tools provided. This type of agent can reason over which of the tools to use next to further the response, feed inputs into the selected tool, and repeat the process with the output until it determines that the answer is satisfactory.
 - Current tool suite:
   While we didn't emphasize equipping the agent with many tools, we hope to see memary help agents in the community equipped with a vast array of tools covering multi-modalities.
```

### Comparing `memary-0.1.2/pyproject.toml` & `memary-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "memary"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="memary Labs", email="hello@memarylabs.com" },
 ]
 description = "Longterm Memory for Autonomous Agents"
 readme = "README_hidden.md"
 requires-python = ">=3.8, <=3.11.9"
 classifiers = [
@@ -41,12 +41,13 @@
     "llama-index-multi-modal-llms-ollama==0.1.3",
     "llama-index-llms-ollama==0.1.2",
     "pandas",
     "geocoder",
     "googlemaps",
     "ansistrip",
     "numpy",
+    "ollama",
 ]
 
 [project.urls]
 Homepage = "https://github.com/kingjulio8238/memary"
 Issues = "https://github.com/kingjulio8238/memary/issues"
```

### Comparing `memary-0.1.2/PKG-INFO` & `memary-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: memary
-Version: 0.1.2
+Version: 0.1.3
 Summary: Longterm Memory for Autonomous Agents
 Project-URL: Homepage, https://github.com/kingjulio8238/memary
 Project-URL: Issues, https://github.com/kingjulio8238/memary/issues
 Author-email: memary Labs <hello@memarylabs.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,14 +28,15 @@
 Requires-Dist: llama-index-multi-modal-llms-openai==0.1.3
 Requires-Dist: llama-index-program-openai==0.1.3
 Requires-Dist: llama-index-question-gen-openai==0.1.2
 Requires-Dist: llama-index-readers-file==0.1.4
 Requires-Dist: llama-index==0.10.11
 Requires-Dist: neo4j==5.17.0
 Requires-Dist: numpy
+Requires-Dist: ollama
 Requires-Dist: pandas
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: pyvis==0.3.2
 Requires-Dist: streamlit==1.31.1
 Description-Content-Type: text/markdown
 
 # memary: Open-Source Longterm Memory for Autonomous Agents
@@ -98,14 +99,48 @@
 6. Run:
 
 ```
 cd streamlit_app
 streamlit run app.py
 ```
 
+## Usage
+```python
+from memary.agent.chat_agent import ChatAgent
+
+system_persona_txt = "data/system_persona.txt"
+user_persona_txt = "data/user_persona.txt"
+past_chat_json = "data/past_chat.json"
+memory_stream_json = "data/memory_stream.json"
+entity_knowledge_store_json = "data/entity_knowledge_store.json"
+chat_agent = ChatAgent(
+    "Personal Agent",
+    memory_stream_json,
+    entity_knowledge_store_json,
+    system_persona_txt,
+    user_persona_txt,
+    past_chat_json,
+)
+```
+Pass in subset of `['search', 'vision', 'locate', 'stocks']` as `include_from_defaults` for different set of default tools upon initialization.
+### Adding Custom Tools
+```python
+def multiply(a: int, b: int) -> int:
+    """Multiply two integers and returns the result integer"""
+    return a * b
+
+chat_agent.add_tool({"multiply": multiply})
+```
+More information about creating custom tools for the LlamaIndex ReAct Agent  can be found [here](https://docs.llamaindex.ai/en/stable/examples/agent/react_agent/).
+
+### Removing Tools
+```python
+chat_agent.remove_tool("multiply")
+```
+
 ## Detailed Component Breakdown
 
 ### Routing Agent
 
 - Uses the [ReAct agent](https://react-lm.github.io/) to plan and execute a query given the tools provided. This type of agent can reason over which of the tools to use next to further the response, feed inputs into the selected tool, and repeat the process with the output until it determines that the answer is satisfactory.
 - Current tool suite:
   While we didn't emphasize equipping the agent with many tools, we hope to see memary help agents in the community equipped with a vast array of tools covering multi-modalities.
```

