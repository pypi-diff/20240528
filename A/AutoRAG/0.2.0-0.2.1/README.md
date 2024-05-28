# Comparing `tmp/autorag-0.2.0.tar.gz` & `tmp/autorag-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autorag-0.2.0.tar", last modified: Tue May 21 07:42:28 2024, max compression
+gzip compressed data, was "autorag-0.2.1.tar", last modified: Tue May 28 05:00:42 2024, max compression
```

## Comparing `autorag-0.2.0.tar` & `autorag-0.2.1.tar`

### file list

```diff
@@ -1,538 +1,544 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.839811 autorag-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.751811 autorag-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-21 07:42:18.000000 autorag-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.751811 autorag-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-21 07:42:18.000000 autorag-0.2.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-21 07:42:18.000000 autorag-0.2.0/.github/workflows/sphinx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-21 07:42:18.000000 autorag-0.2.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-21 07:42:18.000000 autorag-0.2.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.835811 autorag-0.2.0/AutoRAG.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25104 2024-05-21 07:42:28.000000 autorag-0.2.0/AutoRAG.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20826 2024-05-21 07:42:28.000000 autorag-0.2.0/AutoRAG.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 07:42:28.000000 autorag-0.2.0/AutoRAG.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 07:42:28.000000 autorag-0.2.0/AutoRAG.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-21 07:42:28.000000 autorag-0.2.0/AutoRAG.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 07:42:28.000000 autorag-0.2.0/AutoRAG.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-21 07:42:18.000000 autorag-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-21 07:42:18.000000 autorag-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-21 07:42:18.000000 autorag-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    25104 2024-05-21 07:42:28.839811 autorag-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-05-21 07:42:18.000000 autorag-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.755811 autorag-0.2.0/autorag/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.755811 autorag-0.2.0/autorag/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.755811 autorag-0.2.0/autorag/data/corpus/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/data/corpus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/data/corpus/langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/data/corpus/llama_index.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.755811 autorag-0.2.0/autorag/data/qacreation/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/data/qacreation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/data/qacreation/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/data/qacreation/llama_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/data/qacreation/llama_index_default_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/data/qacreation/ragas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/data/qacreation/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.755811 autorag-0.2.0/autorag/data/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/data/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/data/utils/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/deploy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.755811 autorag-0.2.0/autorag/evaluate/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.759811 autorag-0.2.0/autorag/evaluate/metric/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.759811 autorag-0.2.0/autorag/evaluate/metric/g_eval_prompts/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/metric/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/metric/retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/metric/retrieval_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/metric/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/retrieval_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluate/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    17782 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/node_line.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.759811 autorag-0.2.0/autorag/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.759811 autorag-0.2.0/autorag/nodes/generator/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/generator/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/generator/llama_index_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/generator/openai_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/generator/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/generator/vllm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.759811 autorag-0.2.0/autorag/nodes/passageaugmenter/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passageaugmenter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passageaugmenter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passageaugmenter/pass_passage_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passageaugmenter/prev_next_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passageaugmenter/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.759811 autorag-0.2.0/autorag/nodes/passagecompressor/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagecompressor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagecompressor/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagecompressor/pass_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagecompressor/refine.py
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagecompressor/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagecompressor/tree_summarize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.763811 autorag-0.2.0/autorag/nodes/passagefilter/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagefilter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagefilter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagefilter/pass_passage_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagefilter/percentile_cutoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagefilter/recency.py
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagefilter/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagefilter/similarity_percentile_cutoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagefilter/similarity_threshold_cutoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagefilter/threshold_cutoff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.763811 autorag-0.2.0/autorag/nodes/passagereranker/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/colbert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/flag_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/flag_embedding_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/jina.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/koreranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/monot5.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/pass_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/rankgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/sentence_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.767811 autorag-0.2.0/autorag/nodes/passagereranker/tart/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/tart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/tart/modeling_enc_t5.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/tart/tart.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/time_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/passagereranker/upr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.767811 autorag-0.2.0/autorag/nodes/promptmaker/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/promptmaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/promptmaker/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/promptmaker/fstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/promptmaker/long_context_reorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9455 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/promptmaker/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.767811 autorag-0.2.0/autorag/nodes/queryexpansion/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/queryexpansion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/queryexpansion/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/queryexpansion/hyde.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/queryexpansion/pass_query_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/queryexpansion/query_decompose.py
--rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/queryexpansion/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.767811 autorag-0.2.0/autorag/nodes/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/retrieval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/retrieval/bm25.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/retrieval/hybrid_cc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/retrieval/hybrid_dbsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/retrieval/hybrid_rrf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/retrieval/hybrid_rsf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/retrieval/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/nodes/retrieval/vectordb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.767811 autorag-0.2.0/autorag/schema/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/schema/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/schema/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.771811 autorag-0.2.0/autorag/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/utils/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    15273 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/utils/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-21 07:42:18.000000 autorag-0.2.0/autorag/web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.771811 autorag-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.771811 autorag-0.2.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.775811 autorag-0.2.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    57124 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/data_creation.png
--rw-r--r--   0 runner    (1001) docker     (127)    30770 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/data_folder.png
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/dcg.png
--rw-r--r--   0 runner    (1001) docker     (127)     9212 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/f1_score.png
--rw-r--r--   0 runner    (1001) docker     (127)    38900 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/map.png
--rw-r--r--   0 runner    (1001) docker     (127)    45576 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/mrr.png
--rw-r--r--   0 runner    (1001) docker     (127)    81810 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/ndcg.png
--rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/ndcg_formula.png
--rw-r--r--   0 runner    (1001) docker     (127)    31538 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/node_folder.png
--rw-r--r--   0 runner    (1001) docker     (127)    18941 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/node_line_folder.png
--rw-r--r--   0 runner    (1001) docker     (127)    42589 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/node_line_summary.png
--rw-r--r--   0 runner    (1001) docker     (127)    92939 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/node_lines.png
--rw-r--r--   0 runner    (1001) docker     (127)    95669 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/node_summary.png
--rw-r--r--   0 runner    (1001) docker     (127)    36728 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/project_folder_example.png
--rw-r--r--   0 runner    (1001) docker     (127)    19853 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/project_folders.png
--rw-r--r--   0 runner    (1001) docker     (127)    22432 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/resources_folder.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.779811 autorag-0.2.0/docs/source/_static/roadmap/
--rw-r--r--   0 runner    (1001) docker     (127)   159068 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/roadmap/RAG_paradigms.png
--rw-r--r--   0 runner    (1001) docker     (127)    38568 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/roadmap/advanced_RAG.png
--rw-r--r--   0 runner    (1001) docker     (127)    62853 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/roadmap/cycle.png
--rw-r--r--   0 runner    (1001) docker     (127)    75826 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/roadmap/merger.png
--rw-r--r--   0 runner    (1001) docker     (127)    82200 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/roadmap/node_line_modular.png
--rw-r--r--   0 runner    (1001) docker     (127)    69999 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/roadmap/policy.png
--rw-r--r--   0 runner    (1001) docker     (127)   567356 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/samsung_sundae.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)    37348 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/trial_folder.png
--rw-r--r--   0 runner    (1001) docker     (127)    25499 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/trial_json.png
--rw-r--r--   0 runner    (1001) docker     (127)   177107 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/trial_summary.png
--rw-r--r--   0 runner    (1001) docker     (127)   269046 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/_static/web_interface.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.783811 autorag-0.2.0/docs/source/api_spec/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.data.corpus.rst
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.data.qacreation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.data.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.evaluate.metric.rst
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.evaluate.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.nodes.generator.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.nodes.passageaugmenter.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.nodes.passagecompressor.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.nodes.passagefilter.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.nodes.passagereranker.rst
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.nodes.promptmaker.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.nodes.queryexpansion.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.nodes.retrieval.rst
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.nodes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.rst
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.schema.rst
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/autorag.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/api_spec/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.783811 autorag-0.2.0/docs/source/data_creation/
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/data_creation/data_format.md
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/data_creation/ragas.md
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/data_creation/tutorial.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.783811 autorag-0.2.0/docs/source/deploy/
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/deploy/api_endpoint.md
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/deploy/web.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.783811 autorag-0.2.0/docs/source/evaluate_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/evaluate_metrics/generation.md
--rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/evaluate_metrics/retrieval.md
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/evaluate_metrics/retrieval_contents.md
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/install.md
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/local_model.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.783811 autorag-0.2.0/docs/source/nodes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.783811 autorag-0.2.0/docs/source/nodes/generator/
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/generator/generator.md
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/generator/llama_index_llm.md
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/generator/openai_llm.md
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/generator/vllm.md
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.783811 autorag-0.2.0/docs/source/nodes/passage_augmenter/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_augmenter/passage_augmenter.md
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_augmenter/prev_next_augmenter.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.783811 autorag-0.2.0/docs/source/nodes/passage_compressor/
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_compressor/passage_compressor.md
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_compressor/refine.md
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_compressor/tree_summarize.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.787811 autorag-0.2.0/docs/source/nodes/passage_filter/
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_filter/passage_filter.md
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_filter/percentile_cutoff.md
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_filter/recency_filter.md
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_filter/threshold_cutoff.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.787811 autorag-0.2.0/docs/source/nodes/passage_reranker/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/cohere.md
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/colbert.md
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/flag_embedding_reranker.md
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/jina_reranker.md
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/koreranker.md
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/monot5.md
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/passage_reranker.md
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/rankgpt.md
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/tart.md
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/time_reranker.md
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/passage_reranker/upr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.787811 autorag-0.2.0/docs/source/nodes/prompt_maker/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/prompt_maker/fstring.md
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/prompt_maker/long_context_reorder.md
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/prompt_maker/prompt_maker.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.787811 autorag-0.2.0/docs/source/nodes/query_expansion/
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/query_expansion/hyde.md
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/query_expansion/query_decompose.md
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/query_expansion/query_expansion.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.791811 autorag-0.2.0/docs/source/nodes/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/retrieval/bm25.md
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/retrieval/hybrid_cc.md
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/retrieval/hybrid_dbsf.md
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/retrieval/hybrid_rrf.md
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/retrieval/hybrid_rsf.md
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/retrieval/retrieval.md
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/nodes/retrieval/vectordb.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.791811 autorag-0.2.0/docs/source/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/optimization/custom_config.md
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/optimization/folder_structure.md
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/optimization/optimization.md
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/optimization/sample_full_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/optimization/strategies.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.791811 autorag-0.2.0/docs/source/roadmap/
--rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/roadmap/modular_rag.md
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/structure.md
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/troubleshooting.md
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-21 07:42:18.000000 autorag-0.2.0/docs/source/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-21 07:42:18.000000 autorag-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-21 07:42:18.000000 autorag-0.2.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.791811 autorag-0.2.0/sample_config/
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-21 07:42:18.000000 autorag-0.2.0/sample_config/compact_local.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-21 07:42:18.000000 autorag-0.2.0/sample_config/compact_openai.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-21 07:42:18.000000 autorag-0.2.0/sample_config/config_korean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-21 07:42:18.000000 autorag-0.2.0/sample_config/extracted_sample.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-21 07:42:18.000000 autorag-0.2.0/sample_config/full.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-21 07:42:18.000000 autorag-0.2.0/sample_config/simple_local.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-21 07:42:18.000000 autorag-0.2.0/sample_config/simple_openai.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.791811 autorag-0.2.0/sample_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-21 07:42:18.000000 autorag-0.2.0/sample_dataset/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.791811 autorag-0.2.0/sample_dataset/eli5/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-21 07:42:18.000000 autorag-0.2.0/sample_dataset/eli5/load_eli5_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.791811 autorag-0.2.0/sample_dataset/msmarco/
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-21 07:42:18.000000 autorag-0.2.0/sample_dataset/msmarco/load_msmarco_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.791811 autorag-0.2.0/sample_dataset/triviaqa/
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-21 07:42:18.000000 autorag-0.2.0/sample_dataset/triviaqa/load_triviaqa_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 07:42:28.839811 autorag-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.795811 autorag-0.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.795811 autorag-0.2.0/tests/autorag/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.743811 autorag-0.2.0/tests/autorag/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.795811 autorag-0.2.0/tests/autorag/data/corpus/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/data/corpus/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/data/corpus/test_langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/data/corpus/test_llama_index_corpus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.795811 autorag-0.2.0/tests/autorag/data/qacreation/
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/data/qacreation/test_base_qacreation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/data/qacreation/test_llama_index_qacreation.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/data/qacreation/test_ragas_qa_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/data/qacreation/test_simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.795811 autorag-0.2.0/tests/autorag/evaluate/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.795811 autorag-0.2.0/tests/autorag/evaluate/metric/
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/evaluate/metric/test_generation_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/evaluate/metric/test_retrieval_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/evaluate/test_evaluate_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/evaluate/test_generation_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/evaluate/test_retrieval_contents_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/evaluate/test_retrieval_evaluate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.743811 autorag-0.2.0/tests/autorag/nodes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.799811 autorag-0.2.0/tests/autorag/nodes/generator/
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/generator/test_generator_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/generator/test_llama_index_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/generator/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/generator/test_run_generator_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/generator/test_vllm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.799811 autorag-0.2.0/tests/autorag/nodes/passageaugmenter/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.799811 autorag-0.2.0/tests/autorag/nodes/passagecompressor/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagecompressor/test_pass_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagecompressor/test_refine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagecompressor/test_tree_summarize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.799811 autorag-0.2.0/tests/autorag/nodes/passagefilter/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagefilter/test_passage_filter_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagefilter/test_passage_filter_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagefilter/test_recency_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagefilter/test_similarity_percentile_cutoff.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagefilter/test_similarity_threshold_cutoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.803811 autorag-0.2.0/tests/autorag/nodes/passagereranker/
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_cohere_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_colbert_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_flag_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_jina_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_koreranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_monot5.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_pass_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_rankgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_sentence_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_tart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_time_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/passagereranker/test_upr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.803811 autorag-0.2.0/tests/autorag/nodes/promptmaker/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/promptmaker/test_fstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/promptmaker/test_long_context_reorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.803811 autorag-0.2.0/tests/autorag/nodes/queryexpansion/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/queryexpansion/test_hyde.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/queryexpansion/test_query_decompose.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6969 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.807811 autorag-0.2.0/tests/autorag/nodes/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/retrieval/test_bm25.py
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/retrieval/test_hybrid_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/retrieval/test_hybrid_cc.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/retrieval/test_hybrid_rrf.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/retrieval/test_hybrid_rsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/retrieval/test_retrieval_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11272 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/retrieval/test_run_retrieval_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/nodes/retrieval/test_vectordb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.807811 autorag-0.2.0/tests/autorag/schema/
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/schema/test_module_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/schema/test_node_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)    15166 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/test_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/test_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/test_support.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/test_web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.807811 autorag-0.2.0/tests/autorag/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/utils/test_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    13545 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/autorag/utils/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/delete_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.807811 autorag-0.2.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   111931 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/corpus_data_sample.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.743811 autorag-0.2.0/tests/resources/data_creation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.811811 autorag-0.2.0/tests/resources/data_creation/raw_dir/
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/data_creation/raw_dir/sample1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/data_creation/raw_dir/sample2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/data_creation/raw_dir/sample3.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/full.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/qa_data_sample.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.811811 autorag-0.2.0/tests/resources/qa_gen_prompts/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/qa_gen_prompts/prompt1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/qa_gen_prompts/prompt2.txt
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/qa_gen_prompts/prompt3.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/qa_test_data_sample.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.811811 autorag-0.2.0/tests/resources/result_project/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.811811 autorag-0.2.0/tests/resources/result_project/0/
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.811811 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.811811 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/
--rw-r--r--   0 runner    (1001) docker     (127)    23516 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    26448 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    33716 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    14683 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    54234 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.811811 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    41557 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.811811 autorag-0.2.0/tests/resources/result_project/0/pre_retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.815811 autorag-0.2.0/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.815811 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.815811 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_compressor/
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    31124 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_compressor/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.815811 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_reranker/
--rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.815811 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/retrieval/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/0/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.815811 autorag-0.2.0/tests/resources/result_project/1/
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.819811 autorag-0.2.0/tests/resources/result_project/1/pre_retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.819811 autorag-0.2.0/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.747811 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.819811 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/passage_filter/
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/passage_filter/0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.819811 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/passage_reranker/
--rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.819811 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/retrieval/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.819811 autorag-0.2.0/tests/resources/result_project/2/
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.747811 autorag-0.2.0/tests/resources/result_project/2/post_retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.819811 autorag-0.2.0/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.819811 autorag-0.2.0/tests/resources/result_project/2/pre_retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.823811 autorag-0.2.0/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.823811 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.823811 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_compressor/
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    31124 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_compressor/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.823811 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_reranker/
--rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.823811 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/retrieval/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.823811 autorag-0.2.0/tests/resources/result_project/3/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/3/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/best.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.827811 autorag-0.2.0/tests/resources/result_project/data/
--rw-r--r--   0 runner    (1001) docker     (127)   111931 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/data/corpus.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/data/qa.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.827811 autorag-0.2.0/tests/resources/result_project/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    91651 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/resources/bm25_porter_stemmer.pkl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.827811 autorag-0.2.0/tests/resources/result_project/resources/chroma/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.835811 autorag-0.2.0/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/
--rw-r--r--   0 runner    (1001) docker     (127)  6284000 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/header.bin
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/link_lists.bin
--rw-r--r--   0 runner    (1001) docker     (127)   352256 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/resources/chroma/chroma.sqlite3
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/result_project/trial.json
--rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/sample_contents_nqa.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.747811 autorag-0.2.0/tests/resources/sample_project/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.835811 autorag-0.2.0/tests/resources/sample_project/data/
--rw-r--r--   0 runner    (1001) docker     (127)   115302 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/sample_project/data/corpus.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/sample_project/data/qa.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:42:28.835811 autorag-0.2.0/tests/resources/sample_project/resources/
--rw-r--r--   0 runner    (1001) docker     (127)   109478 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/sample_project/resources/bm25_gpt2.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    91651 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/sample_project/resources/bm25_porter_stemmer.pkl
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/simple.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    26773 2024-05-21 07:42:18.000000 autorag-0.2.0/tests/resources/test_bm25_retrieval.pkl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.700013 autorag-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.612012 autorag-0.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-28 05:00:31.000000 autorag-0.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.616012 autorag-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-28 05:00:31.000000 autorag-0.2.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-28 05:00:31.000000 autorag-0.2.1/.github/workflows/sphinx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-28 05:00:31.000000 autorag-0.2.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-28 05:00:31.000000 autorag-0.2.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.700013 autorag-0.2.1/AutoRAG.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25129 2024-05-28 05:00:42.000000 autorag-0.2.1/AutoRAG.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21167 2024-05-28 05:00:42.000000 autorag-0.2.1/AutoRAG.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 05:00:42.000000 autorag-0.2.1/AutoRAG.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 05:00:42.000000 autorag-0.2.1/AutoRAG.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-28 05:00:42.000000 autorag-0.2.1/AutoRAG.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 05:00:42.000000 autorag-0.2.1/AutoRAG.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-28 05:00:31.000000 autorag-0.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-28 05:00:31.000000 autorag-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 05:00:31.000000 autorag-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    25129 2024-05-28 05:00:42.700013 autorag-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-05-28 05:00:31.000000 autorag-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.616012 autorag-0.2.1/autorag/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.616012 autorag-0.2.1/autorag/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.620013 autorag-0.2.1/autorag/data/corpus/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/data/corpus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/data/corpus/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/data/corpus/llama_index.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.620013 autorag-0.2.1/autorag/data/qacreation/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/data/qacreation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/data/qacreation/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/data/qacreation/llama_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/data/qacreation/llama_index_default_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/data/qacreation/ragas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/data/qacreation/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.620013 autorag-0.2.1/autorag/data/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/data/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/data/utils/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.620013 autorag-0.2.1/autorag/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.620013 autorag-0.2.1/autorag/evaluate/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.624013 autorag-0.2.1/autorag/evaluate/metric/g_eval_prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/metric/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/metric/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/metric/retrieval_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/metric/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/retrieval_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluate/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17782 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/node_line.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.624013 autorag-0.2.1/autorag/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.624013 autorag-0.2.1/autorag/nodes/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/generator/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/generator/llama_index_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/generator/openai_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/generator/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/generator/vllm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.624013 autorag-0.2.1/autorag/nodes/passageaugmenter/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passageaugmenter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passageaugmenter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passageaugmenter/pass_passage_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passageaugmenter/prev_next_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passageaugmenter/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.624013 autorag-0.2.1/autorag/nodes/passagecompressor/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagecompressor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagecompressor/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagecompressor/longllmlingua.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagecompressor/pass_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagecompressor/refine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagecompressor/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagecompressor/tree_summarize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.628013 autorag-0.2.1/autorag/nodes/passagefilter/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagefilter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagefilter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagefilter/pass_passage_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagefilter/percentile_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagefilter/recency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagefilter/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagefilter/similarity_percentile_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagefilter/similarity_threshold_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagefilter/threshold_cutoff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.628013 autorag-0.2.1/autorag/nodes/passagereranker/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/colbert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/flag_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/flag_embedding_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/jina.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/koreranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/monot5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/pass_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/rankgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/sentence_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.632012 autorag-0.2.1/autorag/nodes/passagereranker/tart/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/tart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/tart/modeling_enc_t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/tart/tart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/time_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/passagereranker/upr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.632012 autorag-0.2.1/autorag/nodes/promptmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/promptmaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/promptmaker/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/promptmaker/fstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/promptmaker/long_context_reorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9455 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/promptmaker/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.632012 autorag-0.2.1/autorag/nodes/queryexpansion/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/queryexpansion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/queryexpansion/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/queryexpansion/hyde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/queryexpansion/multi_query_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/queryexpansion/pass_query_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/queryexpansion/query_decompose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/queryexpansion/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.632012 autorag-0.2.1/autorag/nodes/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/retrieval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/retrieval/bm25.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/retrieval/hybrid_cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/retrieval/hybrid_dbsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/retrieval/hybrid_rrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/retrieval/hybrid_rsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/retrieval/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/nodes/retrieval/vectordb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.636013 autorag-0.2.1/autorag/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/schema/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/schema/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.636013 autorag-0.2.1/autorag/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/utils/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15273 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/utils/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-28 05:00:31.000000 autorag-0.2.1/autorag/web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.636013 autorag-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.636013 autorag-0.2.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.640013 autorag-0.2.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    57124 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/data_creation.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30770 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/data_folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/dcg.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9212 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/f1_score.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38900 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/map.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45576 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/mrr.png
+-rw-r--r--   0 runner    (1001) docker     (127)    81810 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/ndcg.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/ndcg_formula.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31538 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/node_folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18941 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/node_line_folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    42589 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/node_line_summary.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92939 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/node_lines.png
+-rw-r--r--   0 runner    (1001) docker     (127)    95669 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/node_summary.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36728 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/project_folder_example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19853 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/project_folders.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22432 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/resources_folder.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.644013 autorag-0.2.1/docs/source/_static/roadmap/
+-rw-r--r--   0 runner    (1001) docker     (127)   159068 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/roadmap/RAG_paradigms.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38568 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/roadmap/advanced_RAG.png
+-rw-r--r--   0 runner    (1001) docker     (127)    62853 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/roadmap/cycle.png
+-rw-r--r--   0 runner    (1001) docker     (127)    75826 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/roadmap/merger.png
+-rw-r--r--   0 runner    (1001) docker     (127)    82200 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/roadmap/node_line_modular.png
+-rw-r--r--   0 runner    (1001) docker     (127)    69999 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/roadmap/policy.png
+-rw-r--r--   0 runner    (1001) docker     (127)   567356 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/samsung_sundae.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)    37348 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/trial_folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25499 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/trial_json.png
+-rw-r--r--   0 runner    (1001) docker     (127)   177107 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/trial_summary.png
+-rw-r--r--   0 runner    (1001) docker     (127)   269046 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/_static/web_interface.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.644013 autorag-0.2.1/docs/source/api_spec/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.data.corpus.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.data.qacreation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.data.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.evaluate.metric.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.evaluate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.nodes.generator.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.nodes.passageaugmenter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.nodes.passagecompressor.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.nodes.passagefilter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.nodes.passagereranker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.nodes.promptmaker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.nodes.queryexpansion.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.nodes.retrieval.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.nodes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.schema.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/autorag.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/api_spec/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.648012 autorag-0.2.1/docs/source/data_creation/
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/data_creation/data_format.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/data_creation/ragas.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/data_creation/tutorial.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.648012 autorag-0.2.1/docs/source/deploy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/deploy/api_endpoint.md
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/deploy/web.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.648012 autorag-0.2.1/docs/source/evaluate_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/evaluate_metrics/generation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/evaluate_metrics/retrieval.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/evaluate_metrics/retrieval_contents.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/local_model.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.648012 autorag-0.2.1/docs/source/nodes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.648012 autorag-0.2.1/docs/source/nodes/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/generator/generator.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/generator/llama_index_llm.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/generator/openai_llm.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/generator/vllm.md
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.648012 autorag-0.2.1/docs/source/nodes/passage_augmenter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_augmenter/passage_augmenter.md
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_augmenter/prev_next_augmenter.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.648012 autorag-0.2.1/docs/source/nodes/passage_compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_compressor/longllmlingua.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_compressor/passage_compressor.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_compressor/refine.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_compressor/tree_summarize.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.648012 autorag-0.2.1/docs/source/nodes/passage_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_filter/passage_filter.md
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_filter/percentile_cutoff.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_filter/recency_filter.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_filter/threshold_cutoff.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.652013 autorag-0.2.1/docs/source/nodes/passage_reranker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/cohere.md
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/colbert.md
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/flag_embedding_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/jina_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/koreranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/monot5.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/passage_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/rankgpt.md
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/tart.md
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/time_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/passage_reranker/upr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.652013 autorag-0.2.1/docs/source/nodes/prompt_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/prompt_maker/fstring.md
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/prompt_maker/long_context_reorder.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/prompt_maker/prompt_maker.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.652013 autorag-0.2.1/docs/source/nodes/query_expansion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/query_expansion/hyde.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/query_expansion/multi_query_expansion.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/query_expansion/query_decompose.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/query_expansion/query_expansion.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.656013 autorag-0.2.1/docs/source/nodes/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/retrieval/bm25.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/retrieval/hybrid_cc.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/retrieval/hybrid_dbsf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/retrieval/hybrid_rrf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/retrieval/hybrid_rsf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/retrieval/retrieval.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/nodes/retrieval/vectordb.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.656013 autorag-0.2.1/docs/source/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/optimization/custom_config.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/optimization/folder_structure.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/optimization/optimization.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/optimization/sample_full_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/optimization/strategies.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.656013 autorag-0.2.1/docs/source/roadmap/
+-rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/roadmap/modular_rag.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/structure.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/troubleshooting.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-28 05:00:31.000000 autorag-0.2.1/docs/source/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-28 05:00:31.000000 autorag-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-28 05:00:31.000000 autorag-0.2.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.656013 autorag-0.2.1/sample_config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-28 05:00:31.000000 autorag-0.2.1/sample_config/compact_local.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-28 05:00:31.000000 autorag-0.2.1/sample_config/compact_openai.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-28 05:00:31.000000 autorag-0.2.1/sample_config/config_korean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-28 05:00:31.000000 autorag-0.2.1/sample_config/extracted_sample.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-05-28 05:00:31.000000 autorag-0.2.1/sample_config/full.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-28 05:00:31.000000 autorag-0.2.1/sample_config/simple_local.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-28 05:00:31.000000 autorag-0.2.1/sample_config/simple_openai.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.656013 autorag-0.2.1/sample_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-28 05:00:31.000000 autorag-0.2.1/sample_dataset/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.656013 autorag-0.2.1/sample_dataset/eli5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-28 05:00:31.000000 autorag-0.2.1/sample_dataset/eli5/load_eli5_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.656013 autorag-0.2.1/sample_dataset/msmarco/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-28 05:00:31.000000 autorag-0.2.1/sample_dataset/msmarco/load_msmarco_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.656013 autorag-0.2.1/sample_dataset/triviaqa/
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-28 05:00:31.000000 autorag-0.2.1/sample_dataset/triviaqa/load_triviaqa_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 05:00:42.700013 autorag-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.656013 autorag-0.2.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.660013 autorag-0.2.1/tests/autorag/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.604013 autorag-0.2.1/tests/autorag/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.660013 autorag-0.2.1/tests/autorag/data/corpus/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/data/corpus/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/data/corpus/test_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/data/corpus/test_llama_index_corpus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.660013 autorag-0.2.1/tests/autorag/data/qacreation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/data/qacreation/test_base_qacreation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/data/qacreation/test_llama_index_qacreation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/data/qacreation/test_ragas_qa_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/data/qacreation/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.660013 autorag-0.2.1/tests/autorag/evaluate/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.660013 autorag-0.2.1/tests/autorag/evaluate/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/evaluate/metric/test_generation_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/evaluate/metric/test_retrieval_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/evaluate/test_evaluate_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/evaluate/test_generation_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/evaluate/test_retrieval_contents_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/evaluate/test_retrieval_evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.608013 autorag-0.2.1/tests/autorag/nodes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.660013 autorag-0.2.1/tests/autorag/nodes/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/generator/test_generator_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/generator/test_llama_index_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/generator/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/generator/test_run_generator_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/generator/test_vllm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.664013 autorag-0.2.1/tests/autorag/nodes/passageaugmenter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.664013 autorag-0.2.1/tests/autorag/nodes/passagecompressor/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagecompressor/test_longllmlingua.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagecompressor/test_pass_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagecompressor/test_refine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagecompressor/test_tree_summarize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.664013 autorag-0.2.1/tests/autorag/nodes/passagefilter/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagefilter/test_passage_filter_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagefilter/test_passage_filter_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagefilter/test_recency_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagefilter/test_similarity_percentile_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagefilter/test_similarity_threshold_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.668013 autorag-0.2.1/tests/autorag/nodes/passagereranker/
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_cohere_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_colbert_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_flag_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_jina_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_koreranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_monot5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_pass_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_rankgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_sentence_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_tart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_time_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/passagereranker/test_upr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.668013 autorag-0.2.1/tests/autorag/nodes/promptmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/promptmaker/test_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/promptmaker/test_long_context_reorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.668013 autorag-0.2.1/tests/autorag/nodes/queryexpansion/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/queryexpansion/test_hyde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/queryexpansion/test_multi_query_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/queryexpansion/test_query_decompose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.668013 autorag-0.2.1/tests/autorag/nodes/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/retrieval/test_bm25.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/retrieval/test_hybrid_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/retrieval/test_hybrid_cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/retrieval/test_hybrid_rrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/retrieval/test_hybrid_rsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/retrieval/test_retrieval_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11272 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/retrieval/test_run_retrieval_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/nodes/retrieval/test_vectordb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.672013 autorag-0.2.1/tests/autorag/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/schema/test_module_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/schema/test_node_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15166 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/test_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/test_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.672013 autorag-0.2.1/tests/autorag/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/utils/test_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13545 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/autorag/utils/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/delete_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.672013 autorag-0.2.1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   111931 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/corpus_data_sample.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.608013 autorag-0.2.1/tests/resources/data_creation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.672013 autorag-0.2.1/tests/resources/data_creation/raw_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/data_creation/raw_dir/sample1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/data_creation/raw_dir/sample2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/data_creation/raw_dir/sample3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/full.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/qa_data_sample.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.672013 autorag-0.2.1/tests/resources/qa_gen_prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/qa_gen_prompts/prompt1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/qa_gen_prompts/prompt2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/qa_gen_prompts/prompt3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/qa_test_data_sample.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.672013 autorag-0.2.1/tests/resources/result_project/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.672013 autorag-0.2.1/tests/resources/result_project/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.672013 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.676013 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)    23516 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    26448 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    33716 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14683 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    54234 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.676013 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    41557 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.676013 autorag-0.2.1/tests/resources/result_project/0/pre_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.676013 autorag-0.2.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.676013 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.676013 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    31124 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_compressor/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.680013 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.680013 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/retrieval/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/0/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.680013 autorag-0.2.1/tests/resources/result_project/1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.680013 autorag-0.2.1/tests/resources/result_project/1/pre_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.680013 autorag-0.2.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.608013 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.680013 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/passage_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/passage_filter/0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.680013 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.684013 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/retrieval/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.684013 autorag-0.2.1/tests/resources/result_project/2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.612012 autorag-0.2.1/tests/resources/result_project/2/post_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.684013 autorag-0.2.1/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.684013 autorag-0.2.1/tests/resources/result_project/2/pre_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.684013 autorag-0.2.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.684013 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.684013 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    31124 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_compressor/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.684013 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.688013 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/retrieval/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.688013 autorag-0.2.1/tests/resources/result_project/3/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/3/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/best.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.688013 autorag-0.2.1/tests/resources/result_project/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   111931 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/data/corpus.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/data/qa.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.688013 autorag-0.2.1/tests/resources/result_project/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    91651 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/resources/bm25_porter_stemmer.pkl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.688013 autorag-0.2.1/tests/resources/result_project/resources/chroma/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.696013 autorag-0.2.1/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/
+-rw-r--r--   0 runner    (1001) docker     (127)  6284000 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/header.bin
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/link_lists.bin
+-rw-r--r--   0 runner    (1001) docker     (127)   352256 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/resources/chroma/chroma.sqlite3
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/result_project/trial.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/sample_contents_nqa.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.612012 autorag-0.2.1/tests/resources/sample_project/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.696013 autorag-0.2.1/tests/resources/sample_project/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   115302 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/sample_project/data/corpus.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/sample_project/data/qa.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:00:42.700013 autorag-0.2.1/tests/resources/sample_project/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)   109478 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/sample_project/resources/bm25_gpt2.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    91651 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/sample_project/resources/bm25_porter_stemmer.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/simple.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    26773 2024-05-28 05:00:31.000000 autorag-0.2.1/tests/resources/test_bm25_retrieval.pkl
```

### Comparing `autorag-0.2.0/.github/workflows/publish.yml` & `autorag-0.2.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/.github/workflows/sphinx.yml` & `autorag-0.2.1/.github/workflows/sphinx.yml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/.github/workflows/test.yml` & `autorag-0.2.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/.gitignore` & `autorag-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/AutoRAG.egg-info/PKG-INFO` & `autorag-0.2.1/AutoRAG.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoRAG
-Version: 0.2.0
+Version: 0.2.1
 Summary: Automatically Evaluate RAG pipelines with your own data. Find optimal structure for new RAG product.
 Author-email: Marker-Inc <vkehfdl1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -246,14 +246,15 @@
 Requires-Dist: aiohttp
 Requires-Dist: bert_score
 Requires-Dist: sentence-transformers
 Requires-Dist: FlagEmbedding
 Requires-Dist: ragas
 Requires-Dist: ray
 Requires-Dist: kiwipiepy
+Requires-Dist: llmlingua
 Requires-Dist: llama-index>=0.10.1
 Requires-Dist: llama-index-core>=0.10.1
 Requires-Dist: llama-index-embeddings-openai
 Requires-Dist: llama-index-embeddings-huggingface
 Requires-Dist: llama-index-llms-openai
 Requires-Dist: llama-index-llms-huggingface
 Requires-Dist: llama-index-llms-openai-like
```

### Comparing `autorag-0.2.0/AutoRAG.egg-info/SOURCES.txt` & `autorag-0.2.1/AutoRAG.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 autorag/nodes/passageaugmenter/__init__.py
 autorag/nodes/passageaugmenter/base.py
 autorag/nodes/passageaugmenter/pass_passage_augmenter.py
 autorag/nodes/passageaugmenter/prev_next_augmenter.py
 autorag/nodes/passageaugmenter/run.py
 autorag/nodes/passagecompressor/__init__.py
 autorag/nodes/passagecompressor/base.py
+autorag/nodes/passagecompressor/longllmlingua.py
 autorag/nodes/passagecompressor/pass_compressor.py
 autorag/nodes/passagecompressor/refine.py
 autorag/nodes/passagecompressor/run.py
 autorag/nodes/passagecompressor/tree_summarize.py
 autorag/nodes/passagefilter/__init__.py
 autorag/nodes/passagefilter/base.py
 autorag/nodes/passagefilter/pass_passage_filter.py
@@ -101,14 +102,15 @@
 autorag/nodes/promptmaker/base.py
 autorag/nodes/promptmaker/fstring.py
 autorag/nodes/promptmaker/long_context_reorder.py
 autorag/nodes/promptmaker/run.py
 autorag/nodes/queryexpansion/__init__.py
 autorag/nodes/queryexpansion/base.py
 autorag/nodes/queryexpansion/hyde.py
+autorag/nodes/queryexpansion/multi_query_expansion.py
 autorag/nodes/queryexpansion/pass_query_expansion.py
 autorag/nodes/queryexpansion/query_decompose.py
 autorag/nodes/queryexpansion/run.py
 autorag/nodes/retrieval/__init__.py
 autorag/nodes/retrieval/base.py
 autorag/nodes/retrieval/bm25.py
 autorag/nodes/retrieval/hybrid_cc.py
@@ -191,14 +193,15 @@
 docs/source/nodes/index.md
 docs/source/nodes/generator/generator.md
 docs/source/nodes/generator/llama_index_llm.md
 docs/source/nodes/generator/openai_llm.md
 docs/source/nodes/generator/vllm.md
 docs/source/nodes/passage_augmenter/passage_augmenter.md
 docs/source/nodes/passage_augmenter/prev_next_augmenter.md
+docs/source/nodes/passage_compressor/longllmlingua.md
 docs/source/nodes/passage_compressor/passage_compressor.md
 docs/source/nodes/passage_compressor/refine.md
 docs/source/nodes/passage_compressor/tree_summarize.md
 docs/source/nodes/passage_filter/passage_filter.md
 docs/source/nodes/passage_filter/percentile_cutoff.md
 docs/source/nodes/passage_filter/recency_filter.md
 docs/source/nodes/passage_filter/similarity_percentile_cutoff.md
@@ -217,14 +220,15 @@
 docs/source/nodes/passage_reranker/tart.md
 docs/source/nodes/passage_reranker/time_reranker.md
 docs/source/nodes/passage_reranker/upr.md
 docs/source/nodes/prompt_maker/fstring.md
 docs/source/nodes/prompt_maker/long_context_reorder.md
 docs/source/nodes/prompt_maker/prompt_maker.md
 docs/source/nodes/query_expansion/hyde.md
+docs/source/nodes/query_expansion/multi_query_expansion.md
 docs/source/nodes/query_expansion/query_decompose.md
 docs/source/nodes/query_expansion/query_expansion.md
 docs/source/nodes/retrieval/bm25.md
 docs/source/nodes/retrieval/hybrid_cc.md
 docs/source/nodes/retrieval/hybrid_dbsf.md
 docs/source/nodes/retrieval/hybrid_rrf.md
 docs/source/nodes/retrieval/hybrid_rsf.md
@@ -278,14 +282,15 @@
 tests/autorag/nodes/generator/test_run_generator_node.py
 tests/autorag/nodes/generator/test_vllm.py
 tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py
 tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py
 tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py
 tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py
 tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py
+tests/autorag/nodes/passagecompressor/test_longllmlingua.py
 tests/autorag/nodes/passagecompressor/test_pass_compressor.py
 tests/autorag/nodes/passagecompressor/test_refine.py
 tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
 tests/autorag/nodes/passagecompressor/test_tree_summarize.py
 tests/autorag/nodes/passagefilter/test_pass_passage_filter.py
 tests/autorag/nodes/passagefilter/test_passage_filter_base.py
 tests/autorag/nodes/passagefilter/test_passage_filter_run.py
@@ -310,14 +315,15 @@
 tests/autorag/nodes/passagereranker/test_time_reranker.py
 tests/autorag/nodes/passagereranker/test_upr.py
 tests/autorag/nodes/promptmaker/test_fstring.py
 tests/autorag/nodes/promptmaker/test_long_context_reorder.py
 tests/autorag/nodes/promptmaker/test_prompt_maker_base.py
 tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
 tests/autorag/nodes/queryexpansion/test_hyde.py
+tests/autorag/nodes/queryexpansion/test_multi_query_expansion.py
 tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
 tests/autorag/nodes/queryexpansion/test_query_decompose.py
 tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
 tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
 tests/autorag/nodes/retrieval/test_bm25.py
 tests/autorag/nodes/retrieval/test_hybrid_base.py
 tests/autorag/nodes/retrieval/test_hybrid_cc.py
```

### Comparing `autorag-0.2.0/AutoRAG.egg-info/requires.txt` & `autorag-0.2.1/AutoRAG.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 aiohttp
 bert_score
 sentence-transformers
 FlagEmbedding
 ragas
 ray
 kiwipiepy
+llmlingua
 llama-index>=0.10.1
 llama-index-core>=0.10.1
 llama-index-embeddings-openai
 llama-index-embeddings-huggingface
 llama-index-llms-openai
 llama-index-llms-huggingface
 llama-index-llms-openai-like
```

### Comparing `autorag-0.2.0/CODE_OF_CONDUCT.md` & `autorag-0.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/CONTRIBUTING.md` & `autorag-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/LICENSE` & `autorag-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/PKG-INFO` & `autorag-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoRAG
-Version: 0.2.0
+Version: 0.2.1
 Summary: Automatically Evaluate RAG pipelines with your own data. Find optimal structure for new RAG product.
 Author-email: Marker-Inc <vkehfdl1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -246,14 +246,15 @@
 Requires-Dist: aiohttp
 Requires-Dist: bert_score
 Requires-Dist: sentence-transformers
 Requires-Dist: FlagEmbedding
 Requires-Dist: ragas
 Requires-Dist: ray
 Requires-Dist: kiwipiepy
+Requires-Dist: llmlingua
 Requires-Dist: llama-index>=0.10.1
 Requires-Dist: llama-index-core>=0.10.1
 Requires-Dist: llama-index-embeddings-openai
 Requires-Dist: llama-index-embeddings-huggingface
 Requires-Dist: llama-index-llms-openai
 Requires-Dist: llama-index-llms-huggingface
 Requires-Dist: llama-index-llms-openai-like
```

### Comparing `autorag-0.2.0/README.md` & `autorag-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/__init__.py` & `autorag-0.2.1/autorag/__init__.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/cli.py` & `autorag-0.2.1/autorag/cli.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/dashboard.py` & `autorag-0.2.1/autorag/dashboard.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/data/corpus/langchain.py` & `autorag-0.2.1/autorag/data/corpus/langchain.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/data/corpus/llama_index.py` & `autorag-0.2.1/autorag/data/corpus/llama_index.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/data/qacreation/base.py` & `autorag-0.2.1/autorag/data/qacreation/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/data/qacreation/llama_index.py` & `autorag-0.2.1/autorag/data/qacreation/llama_index.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/data/qacreation/llama_index_default_prompt.txt` & `autorag-0.2.1/autorag/data/qacreation/llama_index_default_prompt.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/data/qacreation/ragas.py` & `autorag-0.2.1/autorag/data/qacreation/ragas.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/data/qacreation/simple.py` & `autorag-0.2.1/autorag/data/qacreation/simple.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/data/utils/util.py` & `autorag-0.2.1/autorag/data/utils/util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/deploy.py` & `autorag-0.2.1/autorag/deploy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/evaluate/generation.py` & `autorag-0.2.1/autorag/evaluate/generation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt` & `autorag-0.2.1/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt` & `autorag-0.2.1/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt` & `autorag-0.2.1/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt` & `autorag-0.2.1/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/evaluate/metric/generation.py` & `autorag-0.2.1/autorag/evaluate/metric/generation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/evaluate/metric/retrieval.py` & `autorag-0.2.1/autorag/evaluate/metric/retrieval.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/evaluate/metric/retrieval_contents.py` & `autorag-0.2.1/autorag/evaluate/metric/retrieval_contents.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/evaluate/retrieval.py` & `autorag-0.2.1/autorag/evaluate/retrieval.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/evaluate/retrieval_contents.py` & `autorag-0.2.1/autorag/evaluate/retrieval_contents.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/evaluate/util.py` & `autorag-0.2.1/autorag/evaluate/util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/evaluator.py` & `autorag-0.2.1/autorag/evaluator.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/node_line.py` & `autorag-0.2.1/autorag/node_line.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/generator/base.py` & `autorag-0.2.1/autorag/nodes/generator/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/generator/llama_index_llm.py` & `autorag-0.2.1/autorag/nodes/generator/llama_index_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/generator/openai_llm.py` & `autorag-0.2.1/autorag/nodes/generator/openai_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/generator/run.py` & `autorag-0.2.1/autorag/nodes/generator/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/generator/vllm.py` & `autorag-0.2.1/autorag/nodes/generator/vllm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passageaugmenter/base.py` & `autorag-0.2.1/autorag/nodes/passageaugmenter/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passageaugmenter/prev_next_augmenter.py` & `autorag-0.2.1/autorag/nodes/passageaugmenter/prev_next_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passageaugmenter/run.py` & `autorag-0.2.1/autorag/nodes/passageaugmenter/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagecompressor/base.py` & `autorag-0.2.1/autorag/nodes/passagecompressor/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,23 @@
                 scores=retrieve_scores,
                 ids=retrieved_ids,
                 llm=llm,
                 **param_dict
             )
             del llm
             result = list(map(lambda x: [x], result))
+        elif func.__name__ == 'longllmlingua':
+            result = func(
+                queries=queries,
+                contents=retrieved_contents,
+                scores=retrieve_scores,
+                ids=retrieved_ids,
+                **kwargs
+            )
+            result = list(map(lambda x: [x], result))
         elif func.__name__ == 'pass_compressor':
             result = func(contents=retrieved_contents)
         else:
             raise ValueError(f"{func.__name__} is not supported in passage compressor node.")
 
         return result
```

### Comparing `autorag-0.2.0/autorag/nodes/passagecompressor/refine.py` & `autorag-0.2.1/autorag/nodes/passagecompressor/refine.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagecompressor/run.py` & `autorag-0.2.1/autorag/nodes/passagecompressor/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagecompressor/tree_summarize.py` & `autorag-0.2.1/autorag/nodes/passagecompressor/tree_summarize.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagefilter/base.py` & `autorag-0.2.1/autorag/nodes/passagefilter/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagefilter/percentile_cutoff.py` & `autorag-0.2.1/autorag/nodes/passagefilter/percentile_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagefilter/recency.py` & `autorag-0.2.1/autorag/nodes/passagefilter/recency.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagefilter/run.py` & `autorag-0.2.1/autorag/nodes/passagefilter/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagefilter/similarity_percentile_cutoff.py` & `autorag-0.2.1/autorag/nodes/passagefilter/similarity_percentile_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagefilter/similarity_threshold_cutoff.py` & `autorag-0.2.1/autorag/nodes/passagefilter/similarity_threshold_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagefilter/threshold_cutoff.py` & `autorag-0.2.1/autorag/nodes/passagefilter/threshold_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagereranker/base.py` & `autorag-0.2.1/autorag/nodes/passagereranker/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagereranker/cohere.py` & `autorag-0.2.1/autorag/nodes/passagereranker/cohere.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagereranker/colbert.py` & `autorag-0.2.1/autorag/nodes/passagereranker/colbert.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagereranker/flag_embedding.py` & `autorag-0.2.1/autorag/nodes/passagereranker/flag_embedding.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagereranker/flag_embedding_llm.py` & `autorag-0.2.1/autorag/nodes/passagereranker/flag_embedding_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagereranker/jina.py` & `autorag-0.2.1/autorag/nodes/passagereranker/jina.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagereranker/koreranker.py` & `autorag-0.2.1/autorag/nodes/passagereranker/koreranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagereranker/monot5.py` & `autorag-0.2.1/autorag/nodes/passagereranker/monot5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagereranker/pass_reranker.py` & `autorag-0.2.1/autorag/nodes/passagereranker/pass_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagereranker/rankgpt.py` & `autorag-0.2.1/autorag/nodes/passagereranker/rankgpt.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagereranker/run.py` & `autorag-0.2.1/autorag/nodes/passagereranker/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagereranker/sentence_transformer.py` & `autorag-0.2.1/autorag/nodes/passagereranker/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagereranker/tart/modeling_enc_t5.py` & `autorag-0.2.1/autorag/nodes/passagereranker/tart/modeling_enc_t5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagereranker/tart/tart.py` & `autorag-0.2.1/autorag/nodes/passagereranker/tart/tart.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py` & `autorag-0.2.1/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagereranker/time_reranker.py` & `autorag-0.2.1/autorag/nodes/passagereranker/time_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/passagereranker/upr.py` & `autorag-0.2.1/autorag/nodes/passagereranker/upr.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/promptmaker/base.py` & `autorag-0.2.1/autorag/nodes/promptmaker/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/promptmaker/fstring.py` & `autorag-0.2.1/autorag/nodes/promptmaker/fstring.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/promptmaker/long_context_reorder.py` & `autorag-0.2.1/autorag/nodes/promptmaker/long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/promptmaker/run.py` & `autorag-0.2.1/autorag/nodes/promptmaker/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/queryexpansion/base.py` & `autorag-0.2.1/autorag/nodes/queryexpansion/multi_query_expansion.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,52 @@
-import functools
-import logging
-from pathlib import Path
-from typing import List, Union
+from typing import List, Dict, Callable
 
 import pandas as pd
 
-from autorag import generator_models
-from autorag.utils import result_to_dataframe, validate_qa_dataset
+from autorag.nodes.queryexpansion.base import query_expansion_node
 
-logger = logging.getLogger("AutoRAG")
-
-
-def query_expansion_node(func):
-    @functools.wraps(func)
-    @result_to_dataframe(["queries"])
-    def wrapper(
-            project_dir: Union[str, Path],
-            previous_result: pd.DataFrame,
-            *args, **kwargs) -> List[List[str]]:
-        logger.info(f"Running query expansion node - {func.__name__} module...")
-        validate_qa_dataset(previous_result)
-
-        # find queries columns
-        assert "query" in previous_result.columns, "previous_result must have query column."
-        queries = previous_result["query"].tolist()
-
-        if func.__name__ == "pass_query_expansion":
-            return func(queries=queries)
-
-        # set module parameters
-        llm_str = kwargs.pop("llm")
-
-        # pop prompt from kwargs
-        if "prompt" in kwargs.keys():
-            prompt = kwargs.pop("prompt")
-        else:
-            prompt = ""
-
-        # pop batch from kwargs
-        if "batch" in kwargs.keys():
-            batch = kwargs.pop("batch")
+multi_query_expansion_prompt = """You are an AI language model assistant. 
+    Your task is to generate 3 different versions of the given user 
+    question to retrieve relevant documents from a vector  database. 
+    By generating multiple perspectives on the user question, 
+    your goal is to help the user overcome some of the limitations 
+    of distance-based similarity search. Provide these alternative 
+    questions separated by newlines. Original question: {question}"""
+
+
+@query_expansion_node
+def multi_query_expansion(queries: List[str],
+                          generator_func: Callable,
+                          generator_params: Dict,
+                          prompt: str = multi_query_expansion_prompt) -> List[List[str]]:
+    """
+    Expand a list of queries using a multi-query expansion approach.
+    LLM model generate 3 different versions queries for each input query.
+
+    :param queries: List[str], queries to decompose.
+    :param generator_func: Callable, generator functions.
+    :param generator_params: Dict, generator parameters.
+    :param prompt: str, prompt to use for multi-query expansion.
+        default prompt comes from langchain MultiQueryRetriever default query prompt.
+    :return: List[List[str]], list of expansion query.
+    """
+    full_prompts = []
+    for query in queries:
+        if bool(prompt):
+            full_prompt = f"prompt: {prompt}\n\n question: {query}"
         else:
-            batch = 16
-
-        # set llm model for query expansion
-        if llm_str in generator_models:
-            llm = generator_models[llm_str](**kwargs)
-        else:
-            logger.error(f"llm_str {llm_str} does not exist.")
-            raise KeyError(f"llm_str {llm_str} does not exist.")
-
-        # run query expansion function
-        expanded_queries = func(queries=queries, llm=llm, prompt=prompt, batch=batch)
-        del llm
-        return expanded_queries
-
-    return wrapper
+            full_prompt = multi_query_expansion_prompt.format(question=query)
+        full_prompts.append(full_prompt)
+    input_df = pd.DataFrame({"prompts": full_prompts})
+    result_df = generator_func(project_dir=None, previous_result=input_df, **generator_params)
+    answers = result_df['generated_texts'].tolist()
+    results = list(map(lambda x: get_multi_query_expansion(x[0], x[1]), zip(queries, answers)))
+    return results
+
+
+def get_multi_query_expansion(query: str, answer: str) -> List[str]:
+    try:
+        queries = answer.split("\n")
+        queries.insert(0, query)
+        return queries
+    except:
+        return [query]
```

### Comparing `autorag-0.2.0/autorag/nodes/queryexpansion/hyde.py` & `autorag-0.2.1/autorag/nodes/queryexpansion/hyde.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,31 @@
-import asyncio
-from typing import List
+from typing import List, Dict, Callable
 
-from llama_index.core.service_context_elements.llm_predictor import LLMPredictorType
+import pandas as pd
 
 from autorag.nodes.queryexpansion.base import query_expansion_node
-from autorag.utils.util import process_batch
 
 hyde_prompt = "Please write a passage to answer the question"
 
 
 @query_expansion_node
-def hyde(queries: List[str], llm: LLMPredictorType,
-         prompt: str = hyde_prompt,
-         batch: int = 16) -> List[List[str]]:
+def hyde(queries: List[str],
+         generator_func: Callable,
+         generator_params: Dict,
+         prompt: str = hyde_prompt) -> List[List[str]]:
     """
     HyDE, which inspired by "Precise Zero-shot Dense Retrieval without Relevance Labels" (https://arxiv.org/pdf/2212.10496.pdf)
     LLM model creates a hypothetical passage.
     And then, retrieve passages using hypothetical passage as a query.
     :param queries: List[str], queries to retrieve.
-    :param llm: llm to use for hypothetical passage generation.
+    :param generator_func: Callable, generator functions.
+    :param generator_params: Dict, generator parameters.
     :param prompt: prompt to use when generating hypothetical passage
-    :param batch: Batch size for llm.
-        Default is 16.
     :return: List[List[str]], List of hyde results.
     """
-    # Run async query_decompose_pure function
-    tasks = [hyde_pure(query, llm, prompt) for query in queries]
-    loop = asyncio.get_event_loop()
-    results = loop.run_until_complete(process_batch(tasks, batch_size=batch))
+    full_prompts = list(
+        map(lambda x: (prompt if not bool(prompt) else hyde_prompt) + f"\nQuestion: {x}\nPassage:", queries))
+    input_df = pd.DataFrame({"prompts": full_prompts})
+    result_df = generator_func(project_dir=None, previous_result=input_df, **generator_params)
+    answers = result_df['generated_texts'].tolist()
+    results = list(map(lambda x: [x], answers))
     return results
-
-
-async def hyde_pure(query: str, llm: LLMPredictorType,
-                    prompt: str = hyde_prompt) -> List[str]:
-    if prompt is "":
-        prompt = hyde_prompt
-    full_prompt = prompt + f"\nQuestion: {query}\nPassage:"
-    hyde_answer = await llm.acomplete(full_prompt)
-    return [hyde_answer.text]
```

### Comparing `autorag-0.2.0/autorag/nodes/queryexpansion/query_decompose.py` & `autorag-0.2.1/autorag/nodes/queryexpansion/query_decompose.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-import asyncio
-from typing import List
+from typing import List, Callable, Dict
 
-from llama_index.core.service_context_elements.llm_predictor import LLMPredictorType
+import pandas as pd
 
 from autorag.nodes.queryexpansion.base import query_expansion_node
-from autorag.utils.util import process_batch
 
 decompose_prompt = """Decompose a question in self-contained sub-questions. Use \"The question needs no decomposition\" when no decomposition is needed.
 
     Example 1:
 
     Question: Is Hamlet more common on IMDB than Comedy of Errors?
     Decompositions: 
@@ -50,52 +48,52 @@
     Question: {question}
 
     Decompositions:"
     """
 
 
 @query_expansion_node
-def query_decompose(queries: List[str], llm: LLMPredictorType,
-                    prompt: str = decompose_prompt,
-                    batch: int = 16) -> List[List[str]]:
+def query_decompose(queries: List[str],
+                    generator_func: Callable,
+                    generator_params: Dict,
+                    prompt: str = decompose_prompt) -> List[List[str]]:
     """
     decompose query to little piece of questions.
     :param queries: List[str], queries to decompose.
-    :param llm: LLMPredictorType, language model to use.
+    :param generator_func: Callable, generator functions.
+    :param generator_params: Dict, generator parameters.
     :param prompt: str, prompt to use for query decomposition.
         default prompt comes from Visconde's StrategyQA few-shot prompt.
-    :param batch: int, batch size for llm.
-        Default is 16.
     :return: List[List[str]], list of decomposed query. Return input query if query is not decomposable.
     """
-    # Run async query_decompose_pure function
-    tasks = [query_decompose_pure(query, llm, prompt) for query in queries]
-    loop = asyncio.get_event_loop()
-    results = loop.run_until_complete(process_batch(tasks, batch_size=batch))
+    full_prompts = []
+    for query in queries:
+        if bool(prompt):
+            full_prompt = f"prompt: {prompt}\n\n question: {query}"
+        else:
+            full_prompt = decompose_prompt.format(question=query)
+        full_prompts.append(full_prompt)
+    input_df = pd.DataFrame({"prompts": full_prompts})
+    result_df = generator_func(project_dir=None, previous_result=input_df, **generator_params)
+    answers = result_df['generated_texts'].tolist()
+    results = list(map(lambda x: get_query_decompose(x[0], x[1]), zip(queries, answers)))
     return results
 
 
-async def query_decompose_pure(query: str, llm: LLMPredictorType,
-                               prompt: str = decompose_prompt) -> List[str]:
+def get_query_decompose(query: str, answer: str) -> List[str]:
     """
     decompose query to little piece of questions.
     :param query: str, query to decompose.
-    :param llm: LLMPredictorType, language model to use.
-    :param prompt: str, prompt to use for query decomposition.
-        default prompt comes from Visconde's StrategyQA few-shot prompt.
+    :param answer: str, answer from query_decompose function.
     :return: List[str], list of a decomposed query. Return input query if query is not decomposable.
     """
-    if prompt == "":
-        prompt = decompose_prompt
-    full_prompt = "prompt: " + prompt + "\n\n" "question: " + query
-    answer = await llm.acomplete(full_prompt)
-    if answer.text == "the question needs no decomposition.":
+    if answer.lower() == "the question needs no decomposition":
         return [query]
     try:
-        lines = [line.strip() for line in answer.text.splitlines() if line.strip()]
+        lines = [line.strip() for line in answer.splitlines() if line.strip()]
         if lines[0].startswith("Decompositions:"):
             lines.pop(0)
         questions = [line.split(':', 1)[1].strip() for line in lines if ':' in line]
         if not questions:
             return [query]
         return questions
     except:
```

### Comparing `autorag-0.2.0/autorag/nodes/queryexpansion/run.py` & `autorag-0.2.1/autorag/nodes/queryexpansion/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/retrieval/base.py` & `autorag-0.2.1/autorag/nodes/retrieval/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/retrieval/bm25.py` & `autorag-0.2.1/autorag/nodes/retrieval/bm25.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/retrieval/hybrid_cc.py` & `autorag-0.2.1/autorag/nodes/retrieval/hybrid_cc.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/retrieval/hybrid_dbsf.py` & `autorag-0.2.1/autorag/nodes/retrieval/hybrid_dbsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/retrieval/hybrid_rrf.py` & `autorag-0.2.1/autorag/nodes/retrieval/hybrid_rrf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/retrieval/hybrid_rsf.py` & `autorag-0.2.1/autorag/nodes/retrieval/hybrid_rsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/retrieval/run.py` & `autorag-0.2.1/autorag/nodes/retrieval/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/nodes/retrieval/vectordb.py` & `autorag-0.2.1/autorag/nodes/retrieval/vectordb.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/schema/module.py` & `autorag-0.2.1/autorag/schema/module.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/schema/node.py` & `autorag-0.2.1/autorag/schema/node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/strategy.py` & `autorag-0.2.1/autorag/strategy.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,14 +89,15 @@
                 columns: Iterable[str],
                 metadatas: Optional[List[Any]] = None,
                 strategy_name: str = 'mean',
                 ) -> Tuple[pd.DataFrame, Any]:
     strategy_func_dict = {
         'mean': select_best_average,
         'rank': select_best_rr,
+        'normalize_mean': select_normalize_mean,
     }
     if strategy_name not in strategy_func_dict:
         raise ValueError(f'Input strategy name {strategy_name} is not in {strategy_func_dict.keys()}')
 
     return strategy_func_dict[strategy_name](results, columns, metadatas)
 
 
@@ -125,7 +126,17 @@
                    metadatas: Optional[List[Any]] = None) -> Tuple[pd.DataFrame, Any]:
     results, columns, metadatas = validate_strategy_inputs(results, columns, metadatas)
     each_average_df = pd.DataFrame([df[columns].mean(axis=0).to_dict() for df in results])
     rank_df = each_average_df.rank(ascending=False)
     rr_df = rank_df.applymap(lambda x: 1 / x)
     best_index = np.array(rr_df.sum(axis=1)).argmax()
     return results[best_index], metadatas[best_index]
+
+
+def select_normalize_mean(results: List[pd.DataFrame], columns: Iterable[str],
+                          metadatas: Optional[List[Any]] = None) -> Tuple[pd.DataFrame, Any]:
+    results, columns, metadatas = validate_strategy_inputs(results, columns, metadatas)
+    each_mean_df = pd.DataFrame([df[columns].mean(axis=0).to_dict() for df in results])
+    normalized_means = (each_mean_df - each_mean_df.min()) / (each_mean_df.max() - each_mean_df.min())
+    normalized_mean_sums = normalized_means.sum(axis=1)
+    best_index = normalized_mean_sums.argmax()
+    return results[best_index], metadatas[best_index]
```

### Comparing `autorag-0.2.0/autorag/support.py` & `autorag-0.2.1/autorag/support.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 def get_support_modules(module_name: str) -> Callable:
     support_modules = {
         # query_expansion
         'query_decompose': ('autorag.nodes.queryexpansion', 'query_decompose'),
         'hyde': ('autorag.nodes.queryexpansion', 'hyde'),
         'pass_query_expansion': ('autorag.nodes.queryexpansion', 'pass_query_expansion'),
+        'multi_query_expansion': ('autorag.nodes.queryexpansion', 'multi_query_expansion'),
         # retrieval
         'bm25': ('autorag.nodes.retrieval', 'bm25'),
         'vectordb': ('autorag.nodes.retrieval', 'vectordb'),
         'hybrid_rrf': ('autorag.nodes.retrieval', 'hybrid_rrf'),
         'hybrid_cc': ('autorag.nodes.retrieval', 'hybrid_cc'),
         'hybrid_rsf': ('autorag.nodes.retrieval', 'hybrid_rsf'),
         'hybrid_dbsf': ('autorag.nodes.retrieval', 'hybrid_dbsf'),
@@ -49,14 +50,15 @@
         'recency_filter': ('autorag.nodes.passagefilter', 'recency_filter'),
         'threshold_cutoff': ('autorag.nodes.passagefilter', 'threshold_cutoff'),
         'percentile_cutoff': ('autorag.nodes.passagefilter', 'percentile_cutoff'),
         # passage_compressor
         'tree_summarize': ('autorag.nodes.passagecompressor', 'tree_summarize'),
         'pass_compressor': ('autorag.nodes.passagecompressor', 'pass_compressor'),
         'refine': ('autorag.nodes.passagecompressor', 'refine'),
+        'longllmlingua': ('autorag.nodes.passagecompressor', 'longllmlingua'),
         # prompt_maker
         'fstring': ('autorag.nodes.promptmaker', 'fstring'),
         'long_context_reorder': ('autorag.nodes.promptmaker', 'long_context_reorder'),
         # generator
         'llama_index_llm': ('autorag.nodes.generator', 'llama_index_llm'),
         'vllm': ('autorag.nodes.generator', 'vllm'),
         'openai_llm': ('autorag.nodes.generator', 'openai_llm'),
```

### Comparing `autorag-0.2.0/autorag/utils/preprocess.py` & `autorag-0.2.1/autorag/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/utils/util.py` & `autorag-0.2.1/autorag/utils/util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/autorag/web.py` & `autorag-0.2.1/autorag/web.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/Makefile` & `autorag-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/make.bat` & `autorag-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/data_creation.png` & `autorag-0.2.1/docs/source/_static/data_creation.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/data_folder.png` & `autorag-0.2.1/docs/source/_static/data_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/dcg.png` & `autorag-0.2.1/docs/source/_static/dcg.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/f1_score.png` & `autorag-0.2.1/docs/source/_static/f1_score.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/map.png` & `autorag-0.2.1/docs/source/_static/map.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/mrr.png` & `autorag-0.2.1/docs/source/_static/mrr.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/ndcg.png` & `autorag-0.2.1/docs/source/_static/ndcg.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/ndcg_formula.png` & `autorag-0.2.1/docs/source/_static/ndcg_formula.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/node_folder.png` & `autorag-0.2.1/docs/source/_static/node_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/node_line_folder.png` & `autorag-0.2.1/docs/source/_static/node_line_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/node_line_summary.png` & `autorag-0.2.1/docs/source/_static/node_line_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/node_lines.png` & `autorag-0.2.1/docs/source/_static/node_lines.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/node_summary.png` & `autorag-0.2.1/docs/source/_static/node_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/project_folder_example.png` & `autorag-0.2.1/docs/source/_static/project_folder_example.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/project_folders.png` & `autorag-0.2.1/docs/source/_static/project_folders.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/resources_folder.png` & `autorag-0.2.1/docs/source/_static/resources_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/roadmap/RAG_paradigms.png` & `autorag-0.2.1/docs/source/_static/roadmap/RAG_paradigms.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/roadmap/advanced_RAG.png` & `autorag-0.2.1/docs/source/_static/roadmap/advanced_RAG.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/roadmap/cycle.png` & `autorag-0.2.1/docs/source/_static/roadmap/cycle.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/roadmap/merger.png` & `autorag-0.2.1/docs/source/_static/roadmap/merger.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/roadmap/node_line_modular.png` & `autorag-0.2.1/docs/source/_static/roadmap/node_line_modular.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/roadmap/policy.png` & `autorag-0.2.1/docs/source/_static/roadmap/policy.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/samsung_sundae.jpeg` & `autorag-0.2.1/docs/source/_static/samsung_sundae.jpeg`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/trial_folder.png` & `autorag-0.2.1/docs/source/_static/trial_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/trial_json.png` & `autorag-0.2.1/docs/source/_static/trial_json.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/trial_summary.png` & `autorag-0.2.1/docs/source/_static/trial_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/_static/web_interface.png` & `autorag-0.2.1/docs/source/_static/web_interface.png`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/api_spec/autorag.data.corpus.rst` & `autorag-0.2.1/docs/source/api_spec/autorag.data.corpus.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/api_spec/autorag.data.qacreation.rst` & `autorag-0.2.1/docs/source/api_spec/autorag.data.qacreation.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/api_spec/autorag.evaluate.metric.rst` & `autorag-0.2.1/docs/source/api_spec/autorag.evaluate.metric.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/api_spec/autorag.evaluate.rst` & `autorag-0.2.1/docs/source/api_spec/autorag.evaluate.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/api_spec/autorag.nodes.generator.rst` & `autorag-0.2.1/docs/source/api_spec/autorag.nodes.generator.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/api_spec/autorag.nodes.passageaugmenter.rst` & `autorag-0.2.1/docs/source/api_spec/autorag.nodes.passageaugmenter.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/api_spec/autorag.nodes.passagecompressor.rst` & `autorag-0.2.1/docs/source/api_spec/autorag.nodes.passagecompressor.rst`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 -------------------------------------------
 
 .. automodule:: autorag.nodes.passagecompressor.base
    :members:
    :undoc-members:
    :show-inheritance:
 
+autorag.nodes.passagecompressor.longllmlingua module
+----------------------------------------------------
+
+.. automodule:: autorag.nodes.passagecompressor.longllmlingua
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 autorag.nodes.passagecompressor.pass\_compressor module
 -------------------------------------------------------
 
 .. automodule:: autorag.nodes.passagecompressor.pass_compressor
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `autorag-0.2.0/docs/source/api_spec/autorag.nodes.passagefilter.rst` & `autorag-0.2.1/docs/source/api_spec/autorag.nodes.passagefilter.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/api_spec/autorag.nodes.passagereranker.rst` & `autorag-0.2.1/docs/source/api_spec/autorag.nodes.passagereranker.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst` & `autorag-0.2.1/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/api_spec/autorag.nodes.promptmaker.rst` & `autorag-0.2.1/docs/source/api_spec/autorag.nodes.promptmaker.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/api_spec/autorag.nodes.queryexpansion.rst` & `autorag-0.2.1/docs/source/api_spec/autorag.nodes.queryexpansion.rst`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,22 @@
 ----------------------------------------
 
 .. automodule:: autorag.nodes.queryexpansion.hyde
    :members:
    :undoc-members:
    :show-inheritance:
 
+autorag.nodes.queryexpansion.multi\_query\_expansion module
+-----------------------------------------------------------
+
+.. automodule:: autorag.nodes.queryexpansion.multi_query_expansion
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 autorag.nodes.queryexpansion.pass\_query\_expansion module
 ----------------------------------------------------------
 
 .. automodule:: autorag.nodes.queryexpansion.pass_query_expansion
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `autorag-0.2.0/docs/source/api_spec/autorag.nodes.retrieval.rst` & `autorag-0.2.1/docs/source/api_spec/autorag.nodes.retrieval.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/api_spec/autorag.rst` & `autorag-0.2.1/docs/source/api_spec/autorag.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/conf.py` & `autorag-0.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/data_creation/data_format.md` & `autorag-0.2.1/docs/source/data_creation/data_format.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/data_creation/ragas.md` & `autorag-0.2.1/docs/source/data_creation/ragas.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/data_creation/tutorial.md` & `autorag-0.2.1/docs/source/data_creation/tutorial.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/deploy/api_endpoint.md` & `autorag-0.2.1/docs/source/deploy/api_endpoint.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/deploy/web.md` & `autorag-0.2.1/docs/source/deploy/web.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/evaluate_metrics/generation.md` & `autorag-0.2.1/docs/source/evaluate_metrics/generation.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/evaluate_metrics/retrieval.md` & `autorag-0.2.1/docs/source/evaluate_metrics/retrieval.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/evaluate_metrics/retrieval_contents.md` & `autorag-0.2.1/docs/source/evaluate_metrics/retrieval_contents.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/index.rst` & `autorag-0.2.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/install.md` & `autorag-0.2.1/docs/source/install.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/local_model.md` & `autorag-0.2.1/docs/source/local_model.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/generator/generator.md` & `autorag-0.2.1/docs/source/nodes/generator/generator.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/generator/llama_index_llm.md` & `autorag-0.2.1/docs/source/nodes/generator/llama_index_llm.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/generator/openai_llm.md` & `autorag-0.2.1/docs/source/nodes/generator/openai_llm.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/generator/vllm.md` & `autorag-0.2.1/docs/source/nodes/generator/vllm.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/passage_augmenter/passage_augmenter.md` & `autorag-0.2.1/docs/source/nodes/passage_augmenter/passage_augmenter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/passage_augmenter/prev_next_augmenter.md` & `autorag-0.2.1/docs/source/nodes/passage_augmenter/prev_next_augmenter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/passage_compressor/passage_compressor.md` & `autorag-0.2.1/docs/source/nodes/passage_compressor/passage_compressor.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,8 +49,9 @@
 
 ```{toctree}
 ---
 maxdepth: 1
 ---
 tree_summarize.md
 refine.md
+longllmlingua.md
 ```
```

### Comparing `autorag-0.2.0/docs/source/nodes/passage_compressor/refine.md` & `autorag-0.2.1/docs/source/nodes/passage_compressor/refine.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/passage_compressor/tree_summarize.md` & `autorag-0.2.1/docs/source/nodes/passage_compressor/tree_summarize.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/passage_filter/passage_filter.md` & `autorag-0.2.1/docs/source/nodes/passage_filter/passage_filter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/passage_filter/percentile_cutoff.md` & `autorag-0.2.1/docs/source/nodes/passage_filter/percentile_cutoff.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/passage_filter/recency_filter.md` & `autorag-0.2.1/docs/source/nodes/passage_filter/recency_filter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md` & `autorag-0.2.1/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md` & `autorag-0.2.1/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/passage_filter/threshold_cutoff.md` & `autorag-0.2.1/docs/source/nodes/passage_filter/threshold_cutoff.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/passage_reranker/cohere.md` & `autorag-0.2.1/docs/source/nodes/passage_reranker/cohere.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/passage_reranker/colbert.md` & `autorag-0.2.1/docs/source/nodes/passage_reranker/colbert.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md` & `autorag-0.2.1/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/passage_reranker/flag_embedding_reranker.md` & `autorag-0.2.1/docs/source/nodes/passage_reranker/flag_embedding_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/passage_reranker/jina_reranker.md` & `autorag-0.2.1/docs/source/nodes/passage_reranker/jina_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/passage_reranker/monot5.md` & `autorag-0.2.1/docs/source/nodes/passage_reranker/monot5.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/passage_reranker/passage_reranker.md` & `autorag-0.2.1/docs/source/nodes/passage_reranker/passage_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/passage_reranker/rankgpt.md` & `autorag-0.2.1/docs/source/nodes/passage_reranker/rankgpt.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md` & `autorag-0.2.1/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/passage_reranker/tart.md` & `autorag-0.2.1/docs/source/nodes/passage_reranker/tart.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/passage_reranker/time_reranker.md` & `autorag-0.2.1/docs/source/nodes/passage_reranker/time_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/passage_reranker/upr.md` & `autorag-0.2.1/docs/source/nodes/passage_reranker/upr.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/prompt_maker/fstring.md` & `autorag-0.2.1/docs/source/nodes/prompt_maker/fstring.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/prompt_maker/long_context_reorder.md` & `autorag-0.2.1/docs/source/nodes/prompt_maker/long_context_reorder.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/prompt_maker/prompt_maker.md` & `autorag-0.2.1/docs/source/nodes/prompt_maker/prompt_maker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/query_expansion/query_expansion.md` & `autorag-0.2.1/docs/source/nodes/query_expansion/query_expansion.md`

 * *Files 2% similar despite different names*

```diff
@@ -67,8 +67,9 @@
 
 ```{toctree}
 ---
 maxdepth: 1
 ---
 query_decompose.md
 hyde.md
+multi_query_expansion.md
 ```
```

### Comparing `autorag-0.2.0/docs/source/nodes/retrieval/bm25.md` & `autorag-0.2.1/docs/source/nodes/retrieval/bm25.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/retrieval/hybrid_cc.md` & `autorag-0.2.1/docs/source/nodes/retrieval/hybrid_cc.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/retrieval/hybrid_dbsf.md` & `autorag-0.2.1/docs/source/nodes/retrieval/hybrid_dbsf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/retrieval/hybrid_rrf.md` & `autorag-0.2.1/docs/source/nodes/retrieval/hybrid_rrf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/retrieval/hybrid_rsf.md` & `autorag-0.2.1/docs/source/nodes/retrieval/hybrid_rsf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/retrieval/retrieval.md` & `autorag-0.2.1/docs/source/nodes/retrieval/retrieval.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/nodes/retrieval/vectordb.md` & `autorag-0.2.1/docs/source/nodes/retrieval/vectordb.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/optimization/custom_config.md` & `autorag-0.2.1/docs/source/optimization/custom_config.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/optimization/folder_structure.md` & `autorag-0.2.1/docs/source/optimization/folder_structure.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/optimization/optimization.md` & `autorag-0.2.1/docs/source/optimization/optimization.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/optimization/sample_full_config.yaml` & `autorag-0.2.1/docs/source/optimization/sample_full_config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/optimization/strategies.md` & `autorag-0.2.1/docs/source/optimization/strategies.md`

 * *Files 24% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 
 - mean: The default method. It calculates the mean value of all specified metrics for each module and compares these
   mean values to determine the best module.
 
 - rank: This method ranks each module's results per metric, calculates the reciprocal rank, and selects the best module
   based on these rank results.
 
+- normalize mean: This method normalizes each metric's values across modules to a common scale and then determines the
+  best module.
+
 ## Configuration
 
 To use the new strategy parameter, include it in the strategy section of your YAML configuration file.
 
 ### Example Configuration Using mean Strategy
 
 ```yaml
@@ -40,15 +43,29 @@
 ```yaml
 node_lines:
   - node_line_name: example_node_line_2
     nodes:
       - node_type: retrieval
         top_k: 5
         strategy:
-          metrics: [ precision, recall ]
+          metrics: [ retrieval_precision, retrieval_recall ]
           speed_threshold: 5
           strategy: rank
 ```
 
+### Example Configuration Using Normalize Mean Strategy
+
+```yaml
+node_lines:
+  - node_line_name: example_node_line_2
+    nodes:
+      - node_type: retrieval
+        top_k: 5
+        strategy:
+          metrics: [ retrieval_precision, retrieval_recall ]
+          speed_threshold: 5
+          strategy: normalize_mean
+```
+
 ```{tip}
 For more information, go to [custom config](./custom_config.md) and [optimization](./optimization.md) docs.
 ```
```

### Comparing `autorag-0.2.0/docs/source/roadmap/modular_rag.md` & `autorag-0.2.1/docs/source/roadmap/modular_rag.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/structure.md` & `autorag-0.2.1/docs/source/structure.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/troubleshooting.md` & `autorag-0.2.1/docs/source/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/docs/source/tutorial.md` & `autorag-0.2.1/docs/source/tutorial.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/pyproject.toml` & `autorag-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/requirements.txt` & `autorag-0.2.1/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 aiohttp # for async http requests
 bert_score # for bert score
 sentence-transformers # for sentence transformer reranker
 FlagEmbedding # for flag embedding reranker
 ragas # evaluation data generation & evaluation
 ray # for parallel processing
 kiwipiepy  # for BM25 Korean tokenizer
+llmlingua # for longllmlingua
 
 ### LlamaIndex ###
 llama-index>=0.10.1
 llama-index-core>=0.10.1
 # Embeddings
 llama-index-embeddings-openai
 llama-index-embeddings-huggingface
```

### Comparing `autorag-0.2.0/sample_config/compact_local.yaml` & `autorag-0.2.1/sample_config/compact_local.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/sample_config/compact_openai.yaml` & `autorag-0.2.1/sample_config/compact_openai.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/sample_config/config_korean.yaml` & `autorag-0.2.1/sample_config/config_korean.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/sample_config/extracted_sample.yaml` & `autorag-0.2.1/sample_config/extracted_sample.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/sample_config/full.yaml` & `autorag-0.2.1/sample_config/full.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -10,19 +10,26 @@
           - module_type: bm25
             bm25_tokenizer: [ porter_stemmer, ko_kiwi, space, gpt2 ]
           - module_type: vectordb
             embedding_model: openai
       modules:
         - module_type: pass_query_expansion
         - module_type: query_decompose
+          generator_module_type: llama_index_llm
           llm: openai
-          temperature: [0.2, 1.0]
+          model: [ gpt-3.5-turbo-16k, gpt-3.5-turbo-1106 ]
         - module_type: hyde
+          generator_module_type: llama_index_llm
           llm: openai
+          model: [ gpt-3.5-turbo-16k ]
           max_token: 64
+        - module_type: multi_query_expansion
+          generator_module_type: llama_index_llm
+          llm: openai
+          temperature: [ 0.2, 1.0 ]
 - node_line_name: retrieve_node_line  # Arbitrary node line name
   nodes:
     - node_type: retrieval
       strategy:
         metrics: [ retrieval_f1, retrieval_recall, retrieval_precision,
                    retrieval_ndcg, retrieval_map, retrieval_mrr ]
         speed_threshold: 10
@@ -104,14 +111,15 @@
         - module_type: pass_compressor
         - module_type: tree_summarize
           llm: openai
           model: gpt-3.5-turbo-16k
         - module_type: refine
           llm: openai
           model: gpt-3.5-turbo-16k
+        - module_type: longllmlingua
 - node_line_name: post_retrieve_node_line  # Arbitrary node line name
   nodes:
     - node_type: prompt_maker
       strategy:
         metrics:
           - metric_name: bleu
           - metric_name: meteor
```

### Comparing `autorag-0.2.0/sample_config/simple_local.yaml` & `autorag-0.2.1/sample_config/simple_local.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/sample_config/simple_openai.yaml` & `autorag-0.2.1/sample_config/simple_openai.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/sample_dataset/README.md` & `autorag-0.2.1/sample_dataset/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/sample_dataset/eli5/load_eli5_dataset.py` & `autorag-0.2.1/sample_dataset/eli5/load_eli5_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/sample_dataset/msmarco/load_msmarco_dataset.py` & `autorag-0.2.1/sample_dataset/msmarco/load_msmarco_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/sample_dataset/triviaqa/load_triviaqa_dataset.py` & `autorag-0.2.1/sample_dataset/triviaqa/load_triviaqa_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/data/corpus/test_base.py` & `autorag-0.2.1/tests/autorag/data/corpus/test_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/data/corpus/test_langchain.py` & `autorag-0.2.1/tests/autorag/data/corpus/test_langchain.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/data/corpus/test_llama_index_corpus.py` & `autorag-0.2.1/tests/autorag/data/corpus/test_llama_index_corpus.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/data/qacreation/test_base_qacreation.py` & `autorag-0.2.1/tests/autorag/data/qacreation/test_base_qacreation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/data/qacreation/test_llama_index_qacreation.py` & `autorag-0.2.1/tests/autorag/data/qacreation/test_llama_index_qacreation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/data/qacreation/test_ragas_qa_creation.py` & `autorag-0.2.1/tests/autorag/data/qacreation/test_ragas_qa_creation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/data/qacreation/test_simple.py` & `autorag-0.2.1/tests/autorag/data/qacreation/test_simple.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/evaluate/metric/test_generation_metric.py` & `autorag-0.2.1/tests/autorag/evaluate/metric/test_generation_metric.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py` & `autorag-0.2.1/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/evaluate/metric/test_retrieval_metric.py` & `autorag-0.2.1/tests/autorag/evaluate/metric/test_retrieval_metric.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/evaluate/test_evaluate_util.py` & `autorag-0.2.1/tests/autorag/evaluate/test_evaluate_util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/evaluate/test_generation_evaluate.py` & `autorag-0.2.1/tests/autorag/evaluate/test_generation_evaluate.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/evaluate/test_retrieval_contents_evaluate.py` & `autorag-0.2.1/tests/autorag/evaluate/test_retrieval_contents_evaluate.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/evaluate/test_retrieval_evaluate.py` & `autorag-0.2.1/tests/autorag/evaluate/test_retrieval_evaluate.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/generator/test_generator_base.py` & `autorag-0.2.1/tests/autorag/nodes/generator/test_generator_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/generator/test_llama_index_llm.py` & `autorag-0.2.1/tests/autorag/nodes/generator/test_llama_index_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/generator/test_openai.py` & `autorag-0.2.1/tests/autorag/nodes/generator/test_openai.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/generator/test_run_generator_node.py` & `autorag-0.2.1/tests/autorag/nodes/generator/test_run_generator_node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/generator/test_vllm.py` & `autorag-0.2.1/tests/autorag/nodes/generator/test_vllm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py` & `autorag-0.2.1/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py` & `autorag-0.2.1/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py` & `autorag-0.2.1/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py` & `autorag-0.2.1/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py` & `autorag-0.2.1/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagecompressor/test_pass_compressor.py` & `autorag-0.2.1/tests/autorag/nodes/passagecompressor/test_pass_compressor.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagecompressor/test_refine.py` & `autorag-0.2.1/tests/autorag/nodes/passagecompressor/test_refine.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py` & `autorag-0.2.1/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagecompressor/test_tree_summarize.py` & `autorag-0.2.1/tests/autorag/nodes/passagecompressor/test_tree_summarize.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py` & `autorag-0.2.1/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagefilter/test_passage_filter_base.py` & `autorag-0.2.1/tests/autorag/nodes/passagefilter/test_passage_filter_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagefilter/test_passage_filter_run.py` & `autorag-0.2.1/tests/autorag/nodes/passagefilter/test_passage_filter_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py` & `autorag-0.2.1/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagefilter/test_recency_filter.py` & `autorag-0.2.1/tests/autorag/nodes/passagefilter/test_recency_filter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagefilter/test_similarity_percentile_cutoff.py` & `autorag-0.2.1/tests/autorag/nodes/passagefilter/test_similarity_percentile_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagefilter/test_similarity_threshold_cutoff.py` & `autorag-0.2.1/tests/autorag/nodes/passagefilter/test_similarity_threshold_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py` & `autorag-0.2.1/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_cohere_reranker.py` & `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_cohere_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_colbert_reranker.py` & `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_colbert_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_flag_embedding.py` & `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_flag_embedding.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py` & `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_jina_reranker.py` & `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_jina_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_koreranker.py` & `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_koreranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_monot5.py` & `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_monot5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_pass_reranker.py` & `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_pass_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py` & `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py` & `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_rankgpt.py` & `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_rankgpt.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_sentence_transformer.py` & `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_tart.py` & `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_tart.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_time_reranker.py` & `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_time_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/passagereranker/test_upr.py` & `autorag-0.2.1/tests/autorag/nodes/passagereranker/test_upr.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/promptmaker/test_fstring.py` & `autorag-0.2.1/tests/autorag/nodes/promptmaker/test_fstring.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/promptmaker/test_long_context_reorder.py` & `autorag-0.2.1/tests/autorag/nodes/promptmaker/test_long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py` & `autorag-0.2.1/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py` & `autorag-0.2.1/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py` & `autorag-0.2.1/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py` & `autorag-0.2.1/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py` & `autorag-0.2.1/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import os.path
 import pathlib
 import shutil
 import tempfile
+from unittest.mock import patch
 
 import pandas as pd
 import pytest
+from llama_index.core.base.llms.types import CompletionResponse
+from llama_index.llms.openai import OpenAI
 
-from autorag import generator_models
 from autorag.nodes.queryexpansion import query_decompose, hyde
 from autorag.nodes.queryexpansion.run import evaluate_one_query_expansion_node
 from autorag.nodes.queryexpansion.run import run_query_expansion_node
 from autorag.nodes.retrieval import bm25
 from autorag.utils.util import load_summary_file
-from tests.mock import MockLLM
 
 root_dir = pathlib.PurePath(os.path.dirname(os.path.realpath(__file__))).parent.parent.parent
 resources_dir = os.path.join(root_dir, "resources")
 
 sample_expanded_queries = [
     ["What is the purpose of rushing up the middle in football?",
      "Why are the first two plays often used for rushing up the middle in football?",
@@ -72,66 +73,94 @@
     assert os.path.exists(summary_path)
     summary_df = load_summary_file(summary_path)
     assert set(summary_df.columns) == {'filename', 'query_expansion_retrieval_f1', 'query_expansion_retrieval_recall',
                                        'module_name', 'module_params', 'execution_time', 'is_best'}
     assert len(summary_df) == 2
     assert summary_df['filename'][0] == "0.parquet"
     assert summary_df['module_name'][0] == "query_decompose"
-    assert summary_df['module_params'][0] == {'llm': "mock", 'temperature': 0.2, 'batch': 7}
+    assert summary_df['module_params'][0] == {'generator_module_type': 'llama_index_llm', 'llm': "mock", 'batch': 7}
     assert summary_df['execution_time'][0] > 0
     assert summary_df['is_best'][0] == True or summary_df['is_best'][0] == False  # is_best is np.bool_
     # test the best file is saved properly
     best_filename = summary_df[summary_df['is_best']]['filename'].values[0]
     best_path = os.path.join(node_line_dir, "query_expansion", f"best_{best_filename}")
     assert os.path.exists(best_path)
     best_df = pd.read_parquet(best_path)
     assert all([expect_column in best_df.columns for expect_column in expect_columns])
 
 
 def test_run_query_expansion_node(node_line_dir):
-    generator_models['mock'] = MockLLM
     project_dir = pathlib.PurePath(node_line_dir).parent.parent
     qa_path = os.path.join(project_dir, "data", "qa.parquet")
     previous_result = pd.read_parquet(qa_path)
 
     modules = [query_decompose, hyde]
-    module_params = [{'llm': "mock", 'temperature': 0.2, 'batch': 7}, {'llm': "mock"}]
+    module_params = [{'generator_module_type': 'llama_index_llm', 'llm': "mock", 'batch': 7},
+                     {'generator_module_type': 'llama_index_llm', 'llm': "mock"}]
     strategies = {
         'metrics': metrics,
         'speed_threshold': 5,
         'top_k': 4,
         'retrieval_modules': [{'module_type': 'bm25', 'bm25_tokenizer': 'gpt2'}],
     }
     best_result = run_query_expansion_node(modules, module_params, previous_result, node_line_dir, strategies)
     base_query_expansion_test(best_result, node_line_dir)
 
 
 def test_run_query_expansion_node_default(node_line_dir):
-    generator_models['mock'] = MockLLM
     project_dir = pathlib.PurePath(node_line_dir).parent.parent
     qa_path = os.path.join(project_dir, "data", "qa.parquet")
     previous_result = pd.read_parquet(qa_path)
 
     modules = [query_decompose, hyde]
-    module_params = [{'llm': "mock", 'temperature': 0.2, 'batch': 7}, {'llm': "mock"}]
+    module_params = [{'generator_module_type': 'llama_index_llm', 'llm': "mock", 'batch': 7},
+                     {'generator_module_type': 'llama_index_llm', 'llm': "mock"}]
     strategies = {
         'metrics': metrics
     }
     best_result = run_query_expansion_node(modules, module_params, previous_result, node_line_dir, strategies)
     base_query_expansion_test(best_result, node_line_dir)
 
 
 def test_run_query_expansion_one_module(node_line_dir):
-    generator_models['mock'] = MockLLM
     project_dir = pathlib.PurePath(node_line_dir).parent.parent
     qa_path = os.path.join(project_dir, "data", "qa.parquet")
     previous_result = pd.read_parquet(qa_path)
 
     modules = [query_decompose]
-    module_params = [{'llm': "mock", 'temperature': 0.2}]
+    module_params = [{'generator_module_type': 'llama_index_llm', 'llm': "mock"}]
+    strategies = {
+        'metrics': metrics
+    }
+    best_result = run_query_expansion_node(modules, module_params, previous_result, node_line_dir, strategies)
+    assert set(best_result.columns) == {
+        'qid', 'query', 'generation_gt', 'retrieval_gt', 'queries'  # automatically skip evaluation
+    }
+    summary_filepath = os.path.join(node_line_dir, "query_expansion", "summary.csv")
+    assert os.path.exists(summary_filepath)
+    summary_df = load_summary_file(summary_filepath)
+    assert set(summary_df) == {
+        'filename', 'module_name', 'module_params', 'execution_time', 'is_best'
+    }
+    best_filepath = os.path.join(node_line_dir, "query_expansion", f"best_{summary_df['filename'].values[0]}")
+    assert os.path.exists(best_filepath)
+
+
+async def mock_acomplete(self, messages, **kwargs):
+    return CompletionResponse(text=messages)
+
+
+@patch.object(OpenAI, "acomplete", mock_acomplete)
+def test_run_query_expansion_no_generator(node_line_dir):
+    project_dir = pathlib.PurePath(node_line_dir).parent.parent
+    qa_path = os.path.join(project_dir, "data", "qa.parquet")
+    previous_result = pd.read_parquet(qa_path)
+
+    modules = [query_decompose]
+    module_params = [{}]
     strategies = {
         'metrics': metrics
     }
     best_result = run_query_expansion_node(modules, module_params, previous_result, node_line_dir, strategies)
     assert set(best_result.columns) == {
         'qid', 'query', 'generation_gt', 'retrieval_gt', 'queries'  # automatically skip evaluation
     }
```

### Comparing `autorag-0.2.0/tests/autorag/nodes/retrieval/test_bm25.py` & `autorag-0.2.1/tests/autorag/nodes/retrieval/test_bm25.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/retrieval/test_hybrid_base.py` & `autorag-0.2.1/tests/autorag/nodes/retrieval/test_hybrid_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/retrieval/test_hybrid_cc.py` & `autorag-0.2.1/tests/autorag/nodes/retrieval/test_hybrid_cc.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py` & `autorag-0.2.1/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/retrieval/test_hybrid_rrf.py` & `autorag-0.2.1/tests/autorag/nodes/retrieval/test_hybrid_rrf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/retrieval/test_hybrid_rsf.py` & `autorag-0.2.1/tests/autorag/nodes/retrieval/test_hybrid_rsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/retrieval/test_retrieval_base.py` & `autorag-0.2.1/tests/autorag/nodes/retrieval/test_retrieval_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/retrieval/test_run_retrieval_node.py` & `autorag-0.2.1/tests/autorag/nodes/retrieval/test_run_retrieval_node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/nodes/retrieval/test_vectordb.py` & `autorag-0.2.1/tests/autorag/nodes/retrieval/test_vectordb.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/schema/test_module_schema.py` & `autorag-0.2.1/tests/autorag/schema/test_module_schema.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/schema/test_node_schema.py` & `autorag-0.2.1/tests/autorag/schema/test_node_schema.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/test_cli.py` & `autorag-0.2.1/tests/autorag/test_cli.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/test_dashboard.py` & `autorag-0.2.1/tests/autorag/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/test_deploy.py` & `autorag-0.2.1/tests/autorag/test_deploy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/test_evaluator.py` & `autorag-0.2.1/tests/autorag/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/test_strategy.py` & `autorag-0.2.1/tests/autorag/test_strategy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import time
 
 import pandas as pd
 import pytest
 
-from autorag.strategy import measure_speed, filter_by_threshold, select_best_average, select_best_rr
+from autorag.strategy import (measure_speed, filter_by_threshold, select_best_average, select_best_rr,
+                              select_normalize_mean)
 
 sample_dfs = [
     pd.DataFrame(
         {'content': ['a', 'b', 'c'], 'retrieval_f1': [0.1, 0.2, 0.3], 'retrieval_recall': [0.1, 0.2, 0.3]}),
     pd.DataFrame(
         {'content': ['d', 'e', 'f'], 'retrieval_f1': [0.2, 0.3, 0.4], 'retrieval_recall': [0.2, 0.3, 0.4]}),
     pd.DataFrame(
@@ -61,7 +62,18 @@
     assert best_df['content'].tolist() == ['g', 'h', 'i']
     assert best_df['retrieval_f1'].tolist() == [0.3, 0.4, 0.5]
     assert best_df['retrieval_recall'].tolist() == [0.3, 0.4, 0.5]
     assert best_filename == 'c'
 
     best_df, _ = select_best_average(sample_dfs, ['retrieval_f1', 'retrieval_recall'])
     assert best_df['content'].tolist() == ['g', 'h', 'i']
+
+
+def test_select_normalize_mean():
+    best_df, best_filename = select_normalize_mean(sample_dfs, ['retrieval_f1', 'retrieval_recall'], sample_metadatas)
+    assert best_df['content'].tolist() == ['g', 'h', 'i']
+    assert best_df['retrieval_f1'].tolist() == [0.3, 0.4, 0.5]
+    assert best_df['retrieval_recall'].tolist() == [0.3, 0.4, 0.5]
+    assert best_filename == 'c'
+
+    best_df, _ = select_best_average(sample_dfs, ['retrieval_f1', 'retrieval_recall'])
+    assert best_df['content'].tolist() == ['g', 'h', 'i']
```

### Comparing `autorag-0.2.0/tests/autorag/test_web.py` & `autorag-0.2.1/tests/autorag/test_web.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/utils/test_preprocess.py` & `autorag-0.2.1/tests/autorag/utils/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/autorag/utils/test_util.py` & `autorag-0.2.1/tests/autorag/utils/test_util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/delete_tests.py` & `autorag-0.2.1/tests/delete_tests.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/mock.py` & `autorag-0.2.1/tests/mock.py`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/README.md` & `autorag-0.2.1/tests/resources/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/corpus_data_sample.parquet` & `autorag-0.2.1/tests/resources/corpus_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/data_creation/raw_dir/sample1.txt` & `autorag-0.2.1/tests/resources/data_creation/raw_dir/sample1.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/data_creation/raw_dir/sample2.txt` & `autorag-0.2.1/tests/resources/data_creation/raw_dir/sample2.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/data_creation/raw_dir/sample3.txt` & `autorag-0.2.1/tests/resources/data_creation/raw_dir/sample3.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/full.yaml` & `autorag-0.2.1/tests/resources/full.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -7,19 +7,20 @@
         speed_threshold: 10
         top_k: 10
         retrieval_modules:
           - module_type: bm25
           - module_type: vectordb
             embedding_model: openai
       modules:
-        - module_type: pass_query_expansion
         - module_type: query_decompose
+          generator_module_type: llama_index_llm
           llm: openai
-          temperature: [0.2, 1.0]
+          model: [ gpt-3.5-turbo-16k, gpt-3.5-turbo-1106 ]
         - module_type: hyde
+          generator_module_type: llama_index_llm
           llm: openai
           max_token: 64
 - node_line_name: retrieve_node_line  # Arbitrary node line name
   nodes:
     - node_type: retrieval
       strategy:
         metrics: [retrieval_f1, retrieval_recall, retrieval_precision]
@@ -52,14 +53,15 @@
         metrics: [retrieval_token_f1, retrieval_token_recall, retrieval_token_precision]
         speed_threshold: 10
       modules:
         - module_type: pass_compressor
         - module_type: tree_summarize
           llm: openai
           model: gpt-3.5-turbo-16k
+        - module_type: longllmlingua
 - node_line_name: post_retrieve_node_line  # Arbitrary node line name
   nodes:
     - node_type: prompt_maker
       strategy:
         metrics:
           - metric_name: bleu
             lowercase: true
```

### Comparing `autorag-0.2.0/tests/resources/qa_data_sample.parquet` & `autorag-0.2.1/tests/resources/qa_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/qa_test_data_sample.parquet` & `autorag-0.2.1/tests/resources/qa_test_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/config.yaml` & `autorag-0.2.1/tests/resources/result_project/0/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet` & `autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet` & `autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet` & `autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet` & `autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet` & `autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet` & `autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet` & `autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv` & `autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet` & `autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet` & `autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet` & `autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv` & `autorag-0.2.1/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.2.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.2.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.2.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.2.1/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet` & `autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet` & `autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet` & `autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.2.1/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/0/summary.csv` & `autorag-0.2.1/tests/resources/result_project/0/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/1/config.yaml` & `autorag-0.2.1/tests/resources/result_project/1/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.2.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.2.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.2.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.2.1/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/passage_filter/0.parquet` & `autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/passage_filter/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet` & `autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet` & `autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.2.1/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/2/config.yaml` & `autorag-0.2.1/tests/resources/result_project/2/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet` & `autorag-0.2.1/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.2.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.2.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.2.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.2.1/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet` & `autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet` & `autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet` & `autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.2.1/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/3/config.yaml` & `autorag-0.2.1/tests/resources/result_project/3/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/best.yaml` & `autorag-0.2.1/tests/resources/result_project/best.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/data/corpus.parquet` & `autorag-0.2.1/tests/resources/result_project/data/corpus.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/data/qa.parquet` & `autorag-0.2.1/tests/resources/result_project/data/qa.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/resources/bm25_porter_stemmer.pkl` & `autorag-0.2.1/tests/resources/result_project/resources/bm25_porter_stemmer.pkl`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin` & `autorag-0.2.1/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin` & `autorag-0.2.1/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/result_project/resources/chroma/chroma.sqlite3` & `autorag-0.2.1/tests/resources/result_project/resources/chroma/chroma.sqlite3`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/sample_contents_nqa.csv` & `autorag-0.2.1/tests/resources/sample_contents_nqa.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/sample_project/data/corpus.parquet` & `autorag-0.2.1/tests/resources/sample_project/data/corpus.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/sample_project/data/qa.parquet` & `autorag-0.2.1/tests/resources/sample_project/data/qa.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/sample_project/resources/bm25_gpt2.pkl` & `autorag-0.2.1/tests/resources/sample_project/resources/bm25_gpt2.pkl`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/sample_project/resources/bm25_porter_stemmer.pkl` & `autorag-0.2.1/tests/resources/sample_project/resources/bm25_porter_stemmer.pkl`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/simple.yaml` & `autorag-0.2.1/tests/resources/simple.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.2.0/tests/resources/test_bm25_retrieval.pkl` & `autorag-0.2.1/tests/resources/test_bm25_retrieval.pkl`

 * *Files identical despite different names*

