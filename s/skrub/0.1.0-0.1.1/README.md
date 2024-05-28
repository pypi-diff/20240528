# Comparing `tmp/skrub-0.1.0.tar.gz` & `tmp/skrub-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skrub-0.1.0.tar", last modified: Wed Dec 13 11:03:21 2023, max compression
+gzip compressed data, was "skrub-0.1.1.tar", last modified: Tue May 28 14:06:09 2024, max compression
```

## Comparing `skrub-0.1.0.tar` & `skrub-0.1.1.tar`

### file list

```diff
@@ -1,94 +1,78 @@
-drwxr-xr-x   0 vincentmaladiere   (501) staff       (20)        0 2023-12-13 11:03:21.077992 skrub-0.1.0/
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     1562 2023-11-09 10:46:54.000000 skrub-0.1.0/LICENSE.txt
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     6647 2023-12-13 11:03:21.077719 skrub-0.1.0/PKG-INFO
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     3834 2023-12-09 16:54:25.000000 skrub-0.1.0/README.rst
-drwxr-xr-x   0 vincentmaladiere   (501) staff       (20)        0 2023-12-13 11:03:21.041641 skrub-0.1.0/benchmarks/
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)        0 2023-11-09 10:46:02.000000 skrub-0.1.0/benchmarks/__init__.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)    13160 2023-11-09 10:46:54.000000 skrub-0.1.0/benchmarks/bench_fuzzy_join_count_vs_hash.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)    21784 2023-11-17 14:30:10.000000 skrub-0.1.0/benchmarks/bench_fuzzy_join_sparse_vs_dense.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     5570 2023-12-12 15:04:56.000000 skrub-0.1.0/benchmarks/bench_fuzzy_join_vs_others.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)    10778 2023-12-11 14:51:16.000000 skrub-0.1.0/benchmarks/bench_gap_divergence.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     5066 2023-11-30 14:53:47.000000 skrub-0.1.0/benchmarks/bench_gap_encoder_hp.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)    10945 2023-11-17 14:30:10.000000 skrub-0.1.0/benchmarks/bench_gap_es_score.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)    15249 2023-11-17 14:30:10.000000 skrub-0.1.0/benchmarks/bench_minhash_batch_number.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     3792 2023-12-11 14:51:16.000000 skrub-0.1.0/benchmarks/bench_tablevectorizer_tuning.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     7480 2023-12-11 14:51:16.000000 skrub-0.1.0/benchmarks/run_on_openml_datasets.py
-drwxr-xr-x   0 vincentmaladiere   (501) staff       (20)        0 2023-12-13 11:03:21.046817 skrub-0.1.0/benchmarks/utils/
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)      384 2023-11-17 14:30:10.000000 skrub-0.1.0/benchmarks/utils/__init__.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)      657 2023-11-09 10:46:02.000000 skrub-0.1.0/benchmarks/utils/_argparser.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     2565 2023-11-17 14:30:10.000000 skrub-0.1.0/benchmarks/utils/_various.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     5812 2023-11-17 14:30:10.000000 skrub-0.1.0/benchmarks/utils/join.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)    14249 2023-11-17 14:30:10.000000 skrub-0.1.0/benchmarks/utils/monitor.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     1398 2023-12-11 14:51:16.000000 skrub-0.1.0/pyproject.toml
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     1950 2023-12-13 11:03:21.079039 skrub-0.1.0/setup.cfg
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)       69 2023-11-17 14:30:10.000000 skrub-0.1.0/setup.py
-drwxr-xr-x   0 vincentmaladiere   (501) staff       (20)        0 2023-12-13 11:03:21.055804 skrub-0.1.0/skrub/
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)        6 2023-12-13 10:10:20.000000 skrub-0.1.0/skrub/VERSION.txt
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     1094 2023-12-09 16:54:25.000000 skrub-0.1.0/skrub/__init__.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)    19266 2023-11-30 14:53:47.000000 skrub-0.1.0/skrub/_agg_joiner.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)      980 2023-11-17 14:30:10.000000 skrub-0.1.0/skrub/_check_dependencies.py
-drwxr-xr-x   0 vincentmaladiere   (501) staff       (20)        0 2023-12-13 11:03:21.060899 skrub-0.1.0/skrub/_dataframe/
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)        0 2023-11-30 14:53:47.000000 skrub-0.1.0/skrub/_dataframe/__init__.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     2769 2023-11-30 14:53:47.000000 skrub-0.1.0/skrub/_dataframe/_namespace.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     9851 2023-12-12 15:04:56.000000 skrub-0.1.0/skrub/_dataframe/_pandas.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     7926 2023-12-12 15:04:56.000000 skrub-0.1.0/skrub/_dataframe/_polars.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)      124 2023-12-09 16:54:25.000000 skrub-0.1.0/skrub/_dataframe/_test_utils.py
-drwxr-xr-x   0 vincentmaladiere   (501) staff       (20)        0 2023-12-13 11:03:21.062458 skrub-0.1.0/skrub/_dataframe/tests/
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)        0 2023-11-30 14:53:47.000000 skrub-0.1.0/skrub/_dataframe/tests/__init__.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     1294 2023-11-30 14:53:47.000000 skrub-0.1.0/skrub/_dataframe/tests/test_namespace.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     3539 2023-12-12 15:04:56.000000 skrub-0.1.0/skrub/_dataframe/tests/test_pandas.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     3254 2023-12-12 15:04:56.000000 skrub-0.1.0/skrub/_dataframe/tests/test_polars.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)    25574 2023-12-10 10:16:56.000000 skrub-0.1.0/skrub/_datetime_encoder.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     8939 2023-12-09 16:54:25.000000 skrub-0.1.0/skrub/_deduplicate.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     3086 2023-11-09 10:46:54.000000 skrub-0.1.0/skrub/_fast_hash.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     8783 2023-12-12 15:04:56.000000 skrub-0.1.0/skrub/_fuzzy_join.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)    44417 2023-12-09 16:54:25.000000 skrub-0.1.0/skrub/_gap_encoder.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)    17559 2023-12-12 15:04:56.000000 skrub-0.1.0/skrub/_interpolation_joiner.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     5421 2023-12-12 15:04:56.000000 skrub-0.1.0/skrub/_join_utils.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)    14156 2023-12-12 15:04:56.000000 skrub-0.1.0/skrub/_joiner.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     6623 2023-12-12 15:04:56.000000 skrub-0.1.0/skrub/_matching.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)    14613 2023-12-09 16:54:25.000000 skrub-0.1.0/skrub/_minhash_encoder.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     5150 2023-11-30 14:53:47.000000 skrub-0.1.0/skrub/_select_cols.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)    21407 2023-11-30 14:53:47.000000 skrub-0.1.0/skrub/_similarity_encoder.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     3386 2023-11-09 10:46:54.000000 skrub-0.1.0/skrub/_string_distances.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)    33249 2023-12-12 15:04:56.000000 skrub-0.1.0/skrub/_table_vectorizer.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     4576 2023-11-30 14:53:47.000000 skrub-0.1.0/skrub/_utils.py
-drwxr-xr-x   0 vincentmaladiere   (501) staff       (20)        0 2023-12-13 11:03:21.064275 skrub-0.1.0/skrub/datasets/
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)      965 2023-11-30 14:53:47.000000 skrub-0.1.0/skrub/datasets/__init__.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)    35278 2023-11-30 14:53:47.000000 skrub-0.1.0/skrub/datasets/_fetching.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     2119 2023-11-30 14:53:47.000000 skrub-0.1.0/skrub/datasets/_generating.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)    10869 2023-11-30 14:53:47.000000 skrub-0.1.0/skrub/datasets/_ken_embeddings.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     1758 2023-11-17 14:30:10.000000 skrub-0.1.0/skrub/datasets/_utils.py
-drwxr-xr-x   0 vincentmaladiere   (501) staff       (20)        0 2023-12-13 11:03:21.066803 skrub-0.1.0/skrub/datasets/tests/
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)        0 2023-11-09 10:46:02.000000 skrub-0.1.0/skrub/datasets/tests/__init__.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     8397 2023-11-30 14:53:47.000000 skrub-0.1.0/skrub/datasets/tests/test_fetching.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)      568 2023-11-09 10:46:02.000000 skrub-0.1.0/skrub/datasets/tests/test_generating.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     1969 2023-11-17 14:30:10.000000 skrub-0.1.0/skrub/datasets/tests/test_ken_embeddings.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     1522 2023-11-17 14:30:10.000000 skrub-0.1.0/skrub/datasets/tests/test_utils.py
-drwxr-xr-x   0 vincentmaladiere   (501) staff       (20)        0 2023-12-13 11:03:21.073862 skrub-0.1.0/skrub/tests/
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)        0 2023-11-09 10:46:02.000000 skrub-0.1.0/skrub/tests/__init__.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)    11018 2023-12-09 16:54:25.000000 skrub-0.1.0/skrub/tests/test_agg_joiner.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)    15282 2023-12-10 10:16:56.000000 skrub-0.1.0/skrub/tests/test_datetime_encoder.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     5541 2023-12-09 16:54:25.000000 skrub-0.1.0/skrub/tests/test_deduplicate.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     7326 2023-11-09 10:46:54.000000 skrub-0.1.0/skrub/tests/test_docstrings.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)      533 2023-11-09 10:46:02.000000 skrub-0.1.0/skrub/tests/test_fast_hash.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)    16928 2023-12-12 15:04:56.000000 skrub-0.1.0/skrub/tests/test_fuzzy_join.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)    10268 2023-12-09 16:54:25.000000 skrub-0.1.0/skrub/tests/test_gap_encoder.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)    11573 2023-12-09 16:54:25.000000 skrub-0.1.0/skrub/tests/test_interpolation_join.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     2500 2023-12-12 15:04:56.000000 skrub-0.1.0/skrub/tests/test_join_utils.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     3619 2023-12-12 15:04:56.000000 skrub-0.1.0/skrub/tests/test_joiner.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)      830 2023-12-12 15:04:56.000000 skrub-0.1.0/skrub/tests/test_matching.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)    10161 2023-12-09 16:54:25.000000 skrub-0.1.0/skrub/tests/test_minhash_encoder.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     2313 2023-11-30 14:53:47.000000 skrub-0.1.0/skrub/tests/test_select_cols.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)    10591 2023-12-09 16:54:25.000000 skrub-0.1.0/skrub/tests/test_similarity_encoder.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     2787 2023-12-09 16:54:25.000000 skrub-0.1.0/skrub/tests/test_sklearn.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     1320 2023-11-09 10:46:54.000000 skrub-0.1.0/skrub/tests/test_string_distances.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)    26667 2023-12-12 15:04:56.000000 skrub-0.1.0/skrub/tests/test_table_vectorizer.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     1021 2023-11-09 10:46:54.000000 skrub-0.1.0/skrub/tests/test_utils.py
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     3896 2023-12-11 14:51:16.000000 skrub-0.1.0/skrub/tests/utils.py
-drwxr-xr-x   0 vincentmaladiere   (501) staff       (20)        0 2023-12-13 11:03:21.058523 skrub-0.1.0/skrub.egg-info/
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     6647 2023-12-13 11:03:20.000000 skrub-0.1.0/skrub.egg-info/PKG-INFO
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)     2419 2023-12-13 11:03:20.000000 skrub-0.1.0/skrub.egg-info/SOURCES.txt
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)        1 2023-12-13 11:03:20.000000 skrub-0.1.0/skrub.egg-info/dependency_links.txt
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)      564 2023-12-13 11:03:20.000000 skrub-0.1.0/skrub.egg-info/requires.txt
--rw-r--r--   0 vincentmaladiere   (501) staff       (20)        6 2023-12-13 11:03:20.000000 skrub-0.1.0/skrub.egg-info/top_level.txt
+drwxrwxr-x   0 jerome    (1000) jerome    (1000)        0 2024-05-28 14:06:09.513027 skrub-0.1.1/
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     1562 2023-09-05 16:11:15.000000 skrub-0.1.1/LICENSE.txt
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     6737 2024-05-28 14:06:09.513027 skrub-0.1.1/PKG-INFO
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     3924 2024-05-28 13:51:25.000000 skrub-0.1.1/README.rst
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     1768 2024-05-28 13:51:25.000000 skrub-0.1.1/pyproject.toml
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     1950 2024-05-28 14:06:09.513027 skrub-0.1.1/setup.cfg
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)       69 2023-12-18 14:40:28.000000 skrub-0.1.1/setup.py
+drwxrwxr-x   0 jerome    (1000) jerome    (1000)        0 2024-05-28 14:06:09.509027 skrub-0.1.1/skrub/
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)        6 2024-05-28 13:51:25.000000 skrub-0.1.1/skrub/VERSION.txt
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     1094 2024-05-28 11:32:14.000000 skrub-0.1.1/skrub/__init__.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)    19321 2024-05-28 13:51:25.000000 skrub-0.1.1/skrub/_agg_joiner.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)      980 2024-05-27 10:38:23.000000 skrub-0.1.1/skrub/_check_dependencies.py
+drwxrwxr-x   0 jerome    (1000) jerome    (1000)        0 2024-05-28 14:06:09.509027 skrub-0.1.1/skrub/_dataframe/
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)        0 2024-05-28 11:32:14.000000 skrub-0.1.1/skrub/_dataframe/__init__.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     2769 2024-05-27 10:38:23.000000 skrub-0.1.1/skrub/_dataframe/_namespace.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     9874 2024-05-28 13:51:25.000000 skrub-0.1.1/skrub/_dataframe/_pandas.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     7938 2024-05-28 13:51:25.000000 skrub-0.1.1/skrub/_dataframe/_polars.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)      124 2024-05-28 11:32:14.000000 skrub-0.1.1/skrub/_dataframe/_test_utils.py
+drwxrwxr-x   0 jerome    (1000) jerome    (1000)        0 2024-05-28 14:06:09.509027 skrub-0.1.1/skrub/_dataframe/tests/
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)        0 2024-05-27 10:38:23.000000 skrub-0.1.1/skrub/_dataframe/tests/__init__.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     1294 2024-05-27 10:38:23.000000 skrub-0.1.1/skrub/_dataframe/tests/test_namespace.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     3539 2024-05-27 10:38:23.000000 skrub-0.1.1/skrub/_dataframe/tests/test_pandas.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     3254 2024-05-27 10:38:23.000000 skrub-0.1.1/skrub/_dataframe/tests/test_polars.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)    25685 2024-05-28 13:51:25.000000 skrub-0.1.1/skrub/_datetime_encoder.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     8977 2024-05-28 13:51:25.000000 skrub-0.1.1/skrub/_deduplicate.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     3086 2024-05-27 10:38:23.000000 skrub-0.1.1/skrub/_fast_hash.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     8824 2024-05-28 13:51:25.000000 skrub-0.1.1/skrub/_fuzzy_join.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)    44453 2024-05-28 13:51:25.000000 skrub-0.1.1/skrub/_gap_encoder.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)    17678 2024-05-28 13:51:25.000000 skrub-0.1.1/skrub/_interpolation_joiner.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     5476 2024-05-28 13:51:25.000000 skrub-0.1.1/skrub/_join_utils.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)    14487 2024-05-28 13:51:25.000000 skrub-0.1.1/skrub/_joiner.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     6623 2024-05-27 10:38:23.000000 skrub-0.1.1/skrub/_matching.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)    14653 2024-05-28 13:51:25.000000 skrub-0.1.1/skrub/_minhash_encoder.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     5222 2024-05-28 13:51:25.000000 skrub-0.1.1/skrub/_select_cols.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)    21456 2024-05-28 13:51:25.000000 skrub-0.1.1/skrub/_similarity_encoder.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     3386 2024-05-27 10:38:23.000000 skrub-0.1.1/skrub/_string_distances.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)    33732 2024-05-28 13:51:25.000000 skrub-0.1.1/skrub/_table_vectorizer.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     4649 2024-05-28 13:51:25.000000 skrub-0.1.1/skrub/_utils.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)       69 2024-05-28 13:51:25.000000 skrub-0.1.1/skrub/conftest.py
+drwxrwxr-x   0 jerome    (1000) jerome    (1000)        0 2024-05-28 14:06:09.509027 skrub-0.1.1/skrub/datasets/
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)      965 2024-05-27 10:38:23.000000 skrub-0.1.1/skrub/datasets/__init__.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)    35284 2024-05-28 13:51:25.000000 skrub-0.1.1/skrub/datasets/_fetching.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     2119 2024-05-27 10:38:23.000000 skrub-0.1.1/skrub/datasets/_generating.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)    10815 2024-05-28 13:51:25.000000 skrub-0.1.1/skrub/datasets/_ken_embeddings.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     1758 2024-05-27 10:38:23.000000 skrub-0.1.1/skrub/datasets/_utils.py
+drwxrwxr-x   0 jerome    (1000) jerome    (1000)        0 2024-05-28 14:06:09.509027 skrub-0.1.1/skrub/datasets/tests/
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)        0 2024-05-27 10:38:23.000000 skrub-0.1.1/skrub/datasets/tests/__init__.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     8397 2024-05-27 10:38:23.000000 skrub-0.1.1/skrub/datasets/tests/test_fetching.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)      568 2024-05-27 10:38:23.000000 skrub-0.1.1/skrub/datasets/tests/test_generating.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     2379 2024-05-28 13:51:25.000000 skrub-0.1.1/skrub/datasets/tests/test_ken_embeddings.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     1522 2024-05-27 10:38:23.000000 skrub-0.1.1/skrub/datasets/tests/test_utils.py
+drwxrwxr-x   0 jerome    (1000) jerome    (1000)        0 2024-05-28 14:06:09.509027 skrub-0.1.1/skrub/tests/
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)        0 2024-05-27 10:38:23.000000 skrub-0.1.1/skrub/tests/__init__.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)    11018 2024-05-28 11:32:14.000000 skrub-0.1.1/skrub/tests/test_agg_joiner.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)    15282 2024-05-28 11:32:14.000000 skrub-0.1.1/skrub/tests/test_datetime_encoder.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     5541 2024-05-27 10:38:23.000000 skrub-0.1.1/skrub/tests/test_deduplicate.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     7326 2024-05-28 09:38:42.000000 skrub-0.1.1/skrub/tests/test_docstrings.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)      533 2024-05-27 10:38:23.000000 skrub-0.1.1/skrub/tests/test_fast_hash.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)    16928 2024-05-28 11:32:14.000000 skrub-0.1.1/skrub/tests/test_fuzzy_join.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)    10268 2024-05-28 11:32:14.000000 skrub-0.1.1/skrub/tests/test_gap_encoder.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)    11573 2024-05-28 11:32:14.000000 skrub-0.1.1/skrub/tests/test_interpolation_join.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     2500 2024-05-27 10:38:23.000000 skrub-0.1.1/skrub/tests/test_join_utils.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     3621 2024-05-28 13:51:25.000000 skrub-0.1.1/skrub/tests/test_joiner.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)      830 2024-05-27 10:38:23.000000 skrub-0.1.1/skrub/tests/test_matching.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)    10161 2024-05-28 11:32:14.000000 skrub-0.1.1/skrub/tests/test_minhash_encoder.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     2313 2024-05-28 11:32:14.000000 skrub-0.1.1/skrub/tests/test_select_cols.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)    10591 2024-05-28 11:32:14.000000 skrub-0.1.1/skrub/tests/test_similarity_encoder.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     2674 2024-05-28 13:51:25.000000 skrub-0.1.1/skrub/tests/test_sklearn.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     1320 2024-05-27 10:38:23.000000 skrub-0.1.1/skrub/tests/test_string_distances.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)    27690 2024-05-28 13:51:25.000000 skrub-0.1.1/skrub/tests/test_table_vectorizer.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     1021 2024-05-27 10:38:23.000000 skrub-0.1.1/skrub/tests/test_utils.py
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     3896 2024-05-27 10:38:23.000000 skrub-0.1.1/skrub/tests/utils.py
+drwxrwxr-x   0 jerome    (1000) jerome    (1000)        0 2024-05-28 14:06:09.509027 skrub-0.1.1/skrub.egg-info/
+-rw-r--r--   0 jerome    (1000) jerome    (1000)     6737 2024-05-28 14:06:09.000000 skrub-0.1.1/skrub.egg-info/PKG-INFO
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)     1915 2024-05-28 14:06:09.000000 skrub-0.1.1/skrub.egg-info/SOURCES.txt
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)        1 2024-05-28 14:06:09.000000 skrub-0.1.1/skrub.egg-info/dependency_links.txt
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)      564 2024-05-28 14:06:09.000000 skrub-0.1.1/skrub.egg-info/requires.txt
+-rw-rw-r--   0 jerome    (1000) jerome    (1000)        6 2024-05-28 14:06:09.000000 skrub-0.1.1/skrub.egg-info/top_level.txt
```

### Comparing `skrub-0.1.0/LICENSE.txt` & `skrub-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/PKG-INFO` & `skrub-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skrub
-Version: 0.1.0
+Version: 0.1.1
 Summary: Prepping tables for machine learning
 Author: Patricio Cerda
 Author-email: patricio.cerda@inria.fr
 License: BSD
 Project-URL: Homepage, https://skrub-data.org/
 Project-URL: Source, https://github.com/skrub-data/skrub
 Classifier: Development Status :: 5 - Production/Stable
@@ -116,23 +116,33 @@
 
 `skrub` can still help with handling typos and variations in this kind of setting.
 
 For a detailed description of the problem of encoding dirty categorical data, see
 `Similarity encoding for learning with dirty categorical variables <https://hal.inria.fr/hal-01806175>`_ [1]_
 and `Encoding high-cardinality string categorical variables <https://hal.inria.fr/hal-02171256v4>`_ [2]_.
 
-Installation (WIP)
-------------------
+Installation
+------------
 
-There are currently no PiPy releases.
-You can still install the package from the GitHub repository with:
+The easiest way to install skrub is via `pip`:
 
 .. code-block:: shell
 
-    pip install git+https://github.com/skrub-data/skrub.git
+    pip install skrub -U
+
+
+or `conda`:
+
+.. code-block:: shell
+
+    conda install -c conda-forge skrub
+
+
+The documentation includes more detailed `installation instructions <https://skrub-data.github.io/install.html>`_.
+
 
 
 Dependencies
 ~~~~~~~~~~~~
 
 Dependencies and minimal versions are listed in the `setup <https://github.com/skrub-data/skrub/blob/main/setup.cfg#L27>`_ file.
```

### Comparing `skrub-0.1.0/README.rst` & `skrub-0.1.1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -45,23 +45,33 @@
 
 `skrub` can still help with handling typos and variations in this kind of setting.
 
 For a detailed description of the problem of encoding dirty categorical data, see
 `Similarity encoding for learning with dirty categorical variables <https://hal.inria.fr/hal-01806175>`_ [1]_
 and `Encoding high-cardinality string categorical variables <https://hal.inria.fr/hal-02171256v4>`_ [2]_.
 
-Installation (WIP)
-------------------
+Installation
+------------
 
-There are currently no PiPy releases.
-You can still install the package from the GitHub repository with:
+The easiest way to install skrub is via `pip`:
 
 .. code-block:: shell
 
-    pip install git+https://github.com/skrub-data/skrub.git
+    pip install skrub -U
+
+
+or `conda`:
+
+.. code-block:: shell
+
+    conda install -c conda-forge skrub
+
+
+The documentation includes more detailed `installation instructions <https://skrub-data.github.io/install.html>`_.
+
 
 
 Dependencies
 ~~~~~~~~~~~~
 
 Dependencies and minimal versions are listed in the `setup <https://github.com/skrub-data/skrub/blob/main/setup.cfg#L27>`_ file.
```

### Comparing `skrub-0.1.0/benchmarks/bench_minhash_batch_number.py` & `skrub-0.1.1/skrub/_minhash_encoder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,148 +1,146 @@
 """
-Testing the performance of the MinHashEncoder based on the number of batches used.
-On the main branch, we only kept the best version of the MinHashEncoder
-which is the batched version with batch_per_job=1
-(the batch_per_job parameter has no effect on the results)
-
-Date: February 2023
+Implements the MinHashEncoder, which encodes string categorical features by
+applying the MinHash method to n-gram decompositions of strings.
 """
+from __future__ import annotations
 
-import pickle
-from argparse import ArgumentParser
 from collections.abc import Callable, Collection
-from pathlib import Path
 from typing import Literal
 
-import matplotlib.pyplot as plt
 import numpy as np
-import pandas as pd
-import seaborn as sns
 from joblib import Parallel, delayed, effective_n_jobs
+from numpy.typing import ArrayLike, NDArray
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils import gen_even_slices, murmurhash3_32
-from utils import default_parser, find_result, monitor
+from sklearn.utils.validation import _check_feature_names_in, check_is_fitted
 
-from skrub._fast_hash import ngram_min_hash
-from skrub._string_distances import get_unique_ngrams
-from skrub._utils import LRUDict, check_input
-from skrub.tests.utils import generate_data
+from ._fast_hash import ngram_min_hash
+from ._string_distances import get_unique_ngrams
+from ._utils import LRUDict, check_input
 
 NoneType = type(None)
 
 
-# Ignore lines too long, as links can't be cut
-# flake8: noqa: E501
-
-
-class MinHashEncoder(BaseEstimator, TransformerMixin):
-    """
-    Encode string categorical features as a numeric array, minhash method
-    applied to ngram decomposition of strings based on ngram decomposition
-    of the string.
+class MinHashEncoder(TransformerMixin, BaseEstimator):
+    """Encode string categorical features by applying the MinHash method to n-gram \
+    decompositions of strings.
+
+    The principle is as follows:
+
+    1. A string is viewed as a succession of numbers (the ASCII or UTF8
+       representation of its elements).
+    2. The string is then decomposed into a set of n-grams, i.e.
+       n-dimensional vectors of integers.
+    3. A hashing function is used to assign an integer to each n-gram.
+       The minimum of the hashes over all n-grams is used in the encoding.
+    4. This process is repeated with `N` hashing functions to form
+       N-dimensional encodings.
+
+    Maxhash encodings can be computed similarly by taking the maximum hash
+    instead.
+    With this procedure, strings that share many n-grams have a greater
+    probability of having the same encoding value. These encodings thus capture
+    morphological similarities between strings.
 
     Parameters
     ----------
     n_components : int, default=30
         The number of dimension of encoded strings. Numbers around 300 tend to
         lead to good prediction performance, but with more computational cost.
-    ngram_range : typing.Tuple[int, int], default=(2, 4)
-        The lower and upper boundary of the range of n-values for different
-        n-grams to be extracted. All values of n such that min_n <= n <= max_n.
-        will be used.
-    hashing : typing.Literal["fast", "murmur"], default=fast
-        Hashing function. fast is faster but
+    ngram_range : 2-tuple of int, default=(2, 4)
+        The lower and upper boundaries of the range of n-values for different
+        n-grams used in the string similarity. All values of `n` such
+        that ``min_n <= n <= max_n`` will be used.
+    hashing : {'fast', 'murmur'}, default='fast'
+        Hashing function. `fast` is faster than `murmur` but
         might have some concern with its entropy.
     minmax_hash : bool, default=False
-        if True, return min hash and max hash concatenated.
-    handle_missing : typing.Literal["error", "zero_impute"], default=zero_impute
+        If `True`, returns the min and max hashes concatenated.
+    handle_missing : {'error', 'zero_impute'}, default='zero_impute'
         Whether to raise an error or encode missing values (NaN) with
         vectors filled with zeros.
-    batch: bool, default=False
-        If False, parallelize the computation of the hash of each unique
-        element. If True, parallelize the computation of the hash of each
-        batch of elements.
-    batch_per_job: int, default=1
-        Number of batches to be processed in each job.
-    n_jobs : int, default=None
+    n_jobs : int, optional
         The number of jobs to run in parallel.
         The hash computations for all unique elements are parallelized.
-        None means 1 unless in a
-        `joblib.parallel_backend context <https://joblib.readthedocs.io/en/latest/parallel.html>`_.
+        `None` means 1 unless in a joblib.parallel_backend.
         -1 means using all processors.
-        See `Scikit-learn Glossary <https://scikit-learn.org/stable/glossary.html#term-n_jobs>`_
-        for more details.
+        See :term:`n_jobs` for more details.
 
     Attributes
     ----------
     hash_dict_ : LRUDict
         Computed hashes.
+    n_features_in_ : int
+        Number of features seen during :term:`fit`.
+    feature_names_in_ : ndarray of shape (n_features_in,)
+        Names of features seen during :term:`fit`.
+
+    See Also
+    --------
+    GapEncoder
+        Encodes dirty categories (strings) by constructing latent topics with
+        continuous encoding.
+    SimilarityEncoder
+        Encode string columns as a numeric array with n-gram string similarity.
+    deduplicate
+        Deduplicate data by hierarchically clustering similar strings.
+
+    References
+    ----------
+    For a detailed description of the method, see
+    `Encoding high-cardinality string categorical variables
+    <https://hal.inria.fr/hal-02171256v4>`_ by Cerda, Varoquaux (2019).
 
     Examples
     --------
+    >>> from skrub import MinHashEncoder
     >>> enc = MinHashEncoder(n_components=5)
 
     Let's encode the following non-normalized data:
 
     >>> X = [['paris, FR'], ['Paris'], ['London, UK'], ['London']]
-
     >>> enc.fit(X)
-    MinHashEncoder()
+    MinHashEncoder(n_components=5)
 
     The encoded data with 5 components are:
 
     >>> enc.transform(X)
     array([[-1.78337518e+09, -1.58827021e+09, -1.66359234e+09,
             -1.81988679e+09, -1.96259387e+09],
            [-8.48046971e+08, -1.76657887e+09, -1.55891205e+09,
             -1.48574446e+09, -1.68729890e+09],
            [-1.97582893e+09, -2.09500033e+09, -1.59652117e+09,
             -1.81759383e+09, -2.09569333e+09],
            [-1.97582893e+09, -2.09500033e+09, -1.53072052e+09,
             -1.45918266e+09, -1.58098831e+09]])
-
-    References
-    ----------
-    For a detailed description of the method, see
-    `Encoding high-cardinality string categorical variables
-    <https://hal.inria.fr/hal-02171256v4>`_ by Cerda, Varoquaux (2019).
-
     """
 
     hash_dict_: LRUDict
 
     _capacity: int = 2**10
 
     def __init__(
         self,
+        *,
         n_components: int = 30,
         ngram_range: tuple[int, int] = (2, 4),
         hashing: Literal["fast", "murmur"] = "fast",
         minmax_hash: bool = False,
         handle_missing: Literal["error", "zero_impute"] = "zero_impute",
-        batch: bool = False,
-        batch_per_job: int = 1,
         n_jobs: int = None,
     ):
         self.ngram_range = ngram_range
         self.n_components = n_components
         self.hashing = hashing
         self.minmax_hash = minmax_hash
         self.handle_missing = handle_missing
-        self.batch = batch
-        self.batch_per_job = batch_per_job
         self.n_jobs = n_jobs
 
-    def _more_tags(self) -> dict[str, list[str]]:
-        """
-        Used internally by sklearn to ease the estimator checks.
-        """
-        return {"X_types": ["categorical"]}
-
-    def _get_murmur_hash(self, string: str) -> np.array:
+    def _get_murmur_hash(self, string: str) -> NDArray:
         """
         Encode a string using murmur hashing function.
 
         Parameters
         ----------
         string : str
             The string to encode.
@@ -162,18 +160,18 @@
                     murmurhash3_32("".join(gram), seed=d, positive=True)
                     for d in range(self.n_components)
                 ]
             )
             min_hashes = np.minimum(min_hashes, hash_array)
         return min_hashes / (2**32 - 1)
 
-    def _get_fast_hash(self, string: str) -> np.array:
-        """
-        Encode a string with fast hashing function.
-        fast hashing supports both min_hash and minmax_hash encoding.
+    def _get_fast_hash(self, string: str) -> NDArray:
+        """Encode a string with fast hashing function.
+
+        Fast hashing supports both min_hash and minmax_hash encoding.
 
         Parameters
         ----------
         string : str
             The string to encode.
 
         Returns
@@ -192,116 +190,97 @@
             return np.array(
                 [
                     ngram_min_hash(string, self.ngram_range, seed)
                     for seed in range(self.n_components)
                 ]
             )
 
-    def _compute_hash(
-        self, string: str, hash_func: Callable[[str], np.ndarray]
-    ) -> np.ndarray:
-        """Function called to compute the hash of a string.
-
-        Check if the string is in the hash dictionary, if not, scompute the hash using
-        the specified hashing function and add it to the dictionary.
-
-        Parameters
-        ----------
-        string : str
-            The string to encode.
-        hash_func : callable
-            Hashing function to use on the string.
-
-        Returns
-        -------
-        np.array of shape (n_components, )
-            The encoded string, using specified encoding scheme.
-        """
-        if string not in self.hash_dict_:
-            if string == "NAN":  # true if x is a missing value
-                self.hash_dict_[string] = np.zeros(self.n_components)
-            else:
-                self.hash_dict_[string] = hash_func(string)
-        return self.hash_dict_[string]
-
     def _compute_hash_batched(
-        self, batch: Collection[str], hash_func: Callable[[str], np.ndarray]
-    ):
+        self, batch: Collection[str], hash_func: Callable[[str], NDArray]
+    ) -> NDArray:
         """Function called to compute the hashes of a batch of strings.
 
-        Check if the string is in the hash dictionary, if not, compute the hash using
-        the specified hashing function and add it to the dictionary.
+        Check if the string is in the hash dictionary, if not, compute the hash
+        using the specified hashing function and add it to the dictionary.
 
         Parameters
         ----------
-        batch : iterable of str
+        batch : collection of str
             The batch of strings to encode.
         hash_func : callable
             Hashing function to use on the string.
 
         Returns
         -------
-        np.array of shape (n_samples, n_components)
+        ndarray of shape (n_samples, n_components)
             The encoded strings, using specified encoding scheme.
         """
         res = np.zeros((len(batch), self.n_components))
         for i, string in enumerate(batch):
             if string not in self.hash_dict_:
                 if string == "NAN":  # true if x is a missing value
                     self.hash_dict_[string] = np.zeros(self.n_components)
                 else:
                     self.hash_dict_[string] = hash_func(string)
             res[i] = self.hash_dict_[string]
         return res
 
-    def fit(self, X, y=None) -> "MinHashEncoder":
-        """
-        Fit the MinHashEncoder to X. In practice, just initializes a dictionary
+    def fit(self, X: ArrayLike, y=None) -> "MinHashEncoder":
+        """Fit the MinHashEncoder to `X`.
+
+        In practice, just initializes a dictionary
         to store encodings to speed up computation.
 
         Parameters
         ----------
-        X : array-like, shape (n_samples, ) or (n_samples, 1)
+        X : array-like, shape (n_samples, ) or (n_samples, n_columns)
             The string data to encode. Only here for compatibility.
         y : None
             Unused, only here for compatibility.
 
         Returns
         -------
         MinHashEncoder
-            The fitted MinHashEncoder instance.
+            The fitted MinHashEncoder instance (self).
         """
+        self._check_feature_names(X, reset=True)
+        X = check_input(X)
+        self._check_n_features(X, reset=True)
+
         if self.hashing not in ["fast", "murmur"]:
             raise ValueError(
                 f"Got hashing={self.hashing!r}, "
                 "but expected any of {'fast', 'murmur'}. "
             )
         if self.handle_missing not in ["error", "zero_impute"]:
             raise ValueError(
                 f"Got handle_missing={self.handle_missing!r}, but expected "
                 "any of {'error', 'zero_impute'}. "
             )
         self.hash_dict_ = LRUDict(capacity=self._capacity)
         return self
 
-    def transform(self, X) -> np.array:
+    def transform(self, X: ArrayLike) -> NDArray:
         """
-        Transform X using specified encoding scheme.
+        Transform `X` using specified encoding scheme.
 
         Parameters
         ----------
-        X : array-like, shape (n_samples, ) or (n_samples, 1)
+        X : array-like, shape (n_samples, ) or (n_samples, n_columns)
             The string data to encode.
 
         Returns
         -------
-        ndarray of shape (n_samples, n_components)
+        ndarray of shape (n_samples, n_columns * n_components)
             Transformed input.
         """
+        check_is_fitted(self, "hash_dict_")
+        self._check_feature_names(X, reset=False)
         X = check_input(X)
+        self._check_n_features(X, reset=False)
         if self.minmax_hash:
             if self.n_components % 2 != 0:
                 raise ValueError(
                     "n_components should be even when using"
                     f"minmax_hash encoding, got {self.n_components}"
                 )
         if self.hashing == "murmur":
@@ -315,15 +294,15 @@
                 "handle_missing should be either "
                 f"'error' or 'zero_impute', got {self.handle_missing!r}"
             )
 
         # Handle missing values
         missing_mask = (
             ~(X == X)  # Find np.nan
-            | (X == None)  # Find None. Note: `X is None` doesn't work.
+            | (X == None)  # noqa: E711 Find None. Note: `X is None` doesn't work.
             | (X == "")  # Find empty strings
         )
 
         if missing_mask.any():  # contains at least one missing value
             if self.handle_missing == "error":
                 raise ValueError(
                     "Found missing values in input data; set "
@@ -343,109 +322,80 @@
                 f"got {self.hashing!r}"
             )
 
         # Compute the hashes for unique values
         unique_x, indices_x = np.unique(X, return_inverse=True)
         n_jobs = effective_n_jobs(self.n_jobs)
 
-        if self.batch:
-            unique_x_trans = Parallel(n_jobs=n_jobs)(
-                delayed(self._compute_hash_batched)(
-                    unique_x[idx_slice],
-                    hash_func,
-                )
-                for idx_slice in gen_even_slices(
-                    len(unique_x), n_jobs * self.batch_per_job
-                )
-            )
-            # Match the hashes of the unique value to the original values
-            X_out = np.concatenate(unique_x_trans)[indices_x].reshape(
-                len(X), X.shape[1] * self.n_components
-            )
-        else:
-            unique_x_trans = Parallel(n_jobs=n_jobs)(
-                delayed(self._compute_hash)(x, hash_func) for x in unique_x
-            )
-            # Match the hashes of the unique value to the original values
-            X_out = np.stack(unique_x_trans)[indices_x].reshape(
-                len(X), X.shape[1] * self.n_components
+        # Compute the hashes in parallel on n_jobs batches
+        unique_x_trans = Parallel(n_jobs=n_jobs)(
+            delayed(self._compute_hash_batched)(
+                unique_x[idx_slice],
+                hash_func,
             )
+            for idx_slice in gen_even_slices(len(unique_x), n_jobs)
+        )
+
+        # Match the hashes of the unique value to the original values
+        X_out = np.concatenate(unique_x_trans)[indices_x].reshape(
+            len(X), X.shape[1] * self.n_components
+        )
 
         return X_out.astype(np.float64)  # The output is an int32 before conversion
 
+    def get_feature_names_out(
+        self, input_features: ArrayLike | str | None = None
+    ) -> NDArray[np.str_]:
+        """Get output feature names for transformation.
+
+        The output feature names look like:
+        ``["x0_0", "x0_1", ..., "x0_(n_components - 1)",
+        "x1_0", ..., "x1_(n_components - 1)", ...,
+        "x(n_features_out - 1)_(n_components - 1)"]``
 
-benchmark_name = "bench_minhash_batch_number"
+        Parameters
+        ----------
+        input_features : array-like of str or None, default=None
+            Input features.
 
+            - If ``input_features`` is ``None``, then ``feature_names_in_`` is
+              used as feature names in. If ``feature_names_in_`` is not defined,
+              then the following input feature names are generated:
+              ``["x0", "x1", ..., "x(n_features_in_ - 1)"]``.
+            - If ``input_features`` is an array-like, then ``input_features`` must
+              match ``feature_names_in_`` if ``feature_names_in_`` is defined.
 
-@monitor(
-    memory=True,
-    time=True,
-    parametrize={
-        "dataset_size": ["medium"],
-        "batched": [True, False],
-        "n_jobs": [1, 4, 8, 16, 32, 64],
-        "batch_per_job": [1, 2, 4],
-    },
-    save_as=benchmark_name,
-    repeat=10,
-)
-def benchmark(
-    dataset_size: str,
-    batched: bool,
-    n_jobs: int,
-    batch_per_job: int,
-) -> None:
-    X = data[dataset_size]
-    MinHashEncoder(batch=batched, n_jobs=n_jobs, batch_per_job=batch_per_job).fit(
-        X
-    ).transform(X)
-
-
-def plot(df: pd.DataFrame):
-    sns.set_theme(style="ticks", palette="pastel")
-
-    # Create a new columns merging batched and batch_per_job
-    # If batch is False, ignore batch_per_job
-    df["config"] = df.apply(
-        lambda row: f"batched={row['batched']}, batch_per_job={row['batch_per_job']}"
-        if row["batched"]
-        else "batched=False",
-        axis=1,
-    )
-    sns.boxplot(x="n_jobs", y="time", hue="config", data=df)
-    # Log scale for the y-axis
-    plt.yscale("log")
-    plt.tight_layout()
-    plt.show()
-
-
-if __name__ == "__main__":
-    _args = ArgumentParser(
-        description="Benchmark for the batch feature of the MinHashEncoder.",
-        parents=[default_parser],
-    ).parse_args()
-
-    # Generate the data if not already on disk, and keep them in memory.
-    data = {}  # Will hold the datasets in memory.
-    _data_info = {
-        "small": 10_000,
-        "medium": 100_000,
-    }
-    for name, size in _data_info.items():
-        data_file = Path(f"data_{name}.pkl")
-        if data_file.is_file():
-            with data_file.open("rb") as fl:
-                data.update({name: pickle.load(fl)})
-        else:
-            with data_file.open("wb") as fl:
-                _gen = generate_data(size).reshape(-1, 1)
-                pickle.dump(_gen, fl)
-                data.update({name: _gen})
-
-    if _args.run:
-        df = benchmark()
-    else:
-        result_file = find_result(benchmark_name)
-        df = pd.read_parquet(result_file)
+        Returns
+        -------
+        feature_names_out : ndarray of str objects
+            Transformed feature names.
+        """
+
+        check_is_fitted(self)
+        input_features = _check_feature_names_in(self, input_features)
+
+        feature_names = []
+        for feature in input_features:
+            for i in range(self.n_components):
+                feature_names.append(f"{feature}_{i}")
 
-    if _args.plot:
-        plot(df)
+        return np.asarray(feature_names, dtype=object)
+
+    def _more_tags(self):
+        """
+        Used internally by sklearn to ease the estimator checks.
+        """
+        return {
+            "X_types": ["2darray", "categorical", "string"],
+            "preserves_dtype": [],
+            "allow_nan": True,
+            "_xfail_checks": {
+                "check_estimator_sparse_data": (
+                    "Cannot create sparse matrix with strings."
+                ),
+                "check_estimators_dtypes": "We only support string dtypes.",
+            },
+            "univariate": True,  # whether the estimator is univariate and can be
+            # applied column by column. This is useful for the TableVectorizer,
+            # to decide whether to apply the transformer on each column separately
+            # and thus improve the parallelization when the transformer is slow enough.
+        }
```

### Comparing `skrub-0.1.0/pyproject.toml` & `skrub-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -41,10 +41,15 @@
     'ignore:.*utcfromtimestamp\(\) is deprecated.*:DeprecationWarning',
     # TODO remove when joblib min version >= 1.4.0
     'ignore:.*ast\.Num is deprecated.*:DeprecationWarning',
     # TODO remove when joblib min version >= 1.4.0
     'ignore:.*ast\.NameConstant is deprecated.*:DeprecationWarning',
     # TODO remove when joblib min version >= 1.4.0
     'ignore:.*Attribute n is deprecated.*:DeprecationWarning',
+    # FIXME we need to decided what to do with pyarrow that is required by pandas >= 3.0
+    'ignore:(?s).*Pyarrow will become a required dependency of pandas.*:DeprecationWarning',
+    # accessing .values on a pandas dataframe raises this warning after numpy 1.25;
+    # should be addressed in pandas
+    'ignore:np.find_common_type is deprecated.*:DeprecationWarning'
 ]
 addopts = "--doctest-modules"
 doctest_optionflags = "NORMALIZE_WHITESPACE ELLIPSIS"
```

### Comparing `skrub-0.1.0/setup.cfg` & `skrub-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/__init__.py` & `skrub-0.1.1/skrub/__init__.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/_agg_joiner.py` & `skrub-0.1.1/skrub/_agg_joiner.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 
 class AggJoiner(BaseEstimator, TransformerMixin):
     """Aggregate auxiliary dataframes before joining them on a base dataframe.
 
     Apply numerical and categorical aggregation operations on the columns
     to aggregate, selected by dtypes. See the list of supported operations
-    at the parameter `agg_ops`.
+    at the parameter `operation`.
 
     The grouping columns used during the aggregation are the columns used
     as keys for joining.
 
     Accepts :obj:`pandas.DataFrame` and :class:`polars.DataFrame` inputs.
 
     Parameters
@@ -103,15 +103,15 @@
         the aggregation operations.
         If None, cols are all columns from table, except `aux_key`.
 
     operation : str or iterable of str, default=None
         Aggregation operations to perform on the auxiliary table.
 
         numerical : {"sum", "mean", "std", "min", "max", "hist", "value_counts"}
-            'hist' and 'value_counts' accepts an integer argument to parametrize
+            'hist' and 'value_counts' accept an integer argument to parametrize
             the binning.
 
         categorical : {"mode", "count", "value_counts"}
 
         If set to None (the default), ['mean', 'mode'] will be used.
 
     suffix : str or iterable of str, default=None
@@ -130,14 +130,15 @@
     Joiner :
         Augments a main table by automatically joining multiple
         auxiliary tables on it.
 
     Examples
     --------
     >>> import pandas as pd
+    >>> from skrub import AggJoiner
     >>> main = pd.DataFrame({
     ...     "airportId": [1, 2],
     ...     "airportName": ["Paris CDG", "NY JFK"],
     ... })
     >>> aux = pd.DataFrame({
     ...     "flightId": range(1, 7),
     ...     "from_airport": [1, 1, 1, 2, 2, 2],
@@ -379,16 +380,16 @@
         Otherwise, if main_key is a list of keys, the target will be
         aggregated using each key separately, then each aggregation of
         the target will be joined on the main table.
 
     operation : str or iterable of str, optional
         Aggregation operations to perform on the auxiliary table.
 
-        numerical : {"sum", "mean", "std", "min", "max", "hist(3)", "value_counts"}
-            'hist' and 'value_counts' accepts an integer argument to parametrize
+        numerical : {"sum", "mean", "std", "min", "max", "hist", "value_counts"}
+            'hist' and 'value_counts' accept an integer argument to parametrize
             the binning.
 
         categorical : {"mode", "count", "value_counts"}
 
         If set to None (the default), ['mean', 'mode'] will be used.
 
     suffix : str, optional
@@ -405,14 +406,16 @@
     Joiner :
         Augments a main table by automatically joining multiple
         auxiliary tables on it.
 
     Examples
     --------
     >>> import pandas as pd
+    >>> import numpy as np
+    >>> from skrub import AggTarget
     >>> X = pd.DataFrame({
     ...     "flightId": range(1, 7),
     ...     "from_airport": [1, 1, 1, 2, 2, 2],
     ...     "total_passengers": [90, 120, 100, 70, 80, 90],
     ...     "company": ["DL", "AF", "AF", "DL", "DL", "TR"],
     ... })
     >>> y = np.array([1, 1, 0, 0, 1, 1])
@@ -424,16 +427,14 @@
        flightId  from_airport  ...  y_0_max_target y_0_mean_target
     0         1             1  ...               1        0.666667
     1         2             1  ...               1        0.500000
     2         3             1  ...               1        0.500000
     3         4             2  ...               1        0.666667
     4         5             2  ...               1        0.666667
     5         6             2  ...               1        1.000000
-    <BLANKLINE>
-    [6 rows x 6 columns]
     """
 
     def __init__(
         self,
         main_key: str | Iterable[str],
         operation: str | Iterable[str] | None = None,
         suffix: str | None = None,
```

### Comparing `skrub-0.1.0/skrub/_check_dependencies.py` & `skrub-0.1.1/skrub/_check_dependencies.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/_dataframe/_namespace.py` & `skrub-0.1.1/skrub/_dataframe/_namespace.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/_dataframe/_pandas.py` & `skrub-0.1.1/skrub/_dataframe/_pandas.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Pandas specialization of the aggregate and join operation.
+Pandas specialization of the aggregate and join operations.
 """
 import re
 from itertools import product
 
 import numpy as np
 import pandas as pd
 
@@ -22,31 +22,31 @@
         The index of the dataframe.
 
     dtypes : str, data type, Series or Mapping of column name -> data type, default=None
         Use a str, numpy.dtype, pandas.ExtensionDtype or Python type to
         cast entire pandas object to the same type. Alternatively, use a
         mapping, e.g. {col: dtype, ...}, where col is a column label and dtype is
         a numpy.dtype or Python type to cast one or more of the DataFrame's
-        columns to column-specific types
+        columns to column-specific types.
 
     Returns
     -------
-    X : Pandas dataframe
+    X : pd.DataFrame
         Converted output.
     """
     df = pd.DataFrame(X, index=index)
     if dtypes is not None:
         # 'df.astype(None)' might raise a ValueError because
         # it tries to cast all columns to floats.
         df = df.astype(dtypes)
     return df
 
 
 def make_series(X, index=None, name=None, dtype=None):
-    """Convert an 1d array into a Pandas series.
+    """Convert a 1d array into a Pandas series.
 
     Parameters
     ----------
     X : 1d iterable
         Input data to convert.
 
     index : 1d array-like, default=None
@@ -77,37 +77,37 @@
 ):
     """Aggregates a :obj:`pandas.DataFrame`.
 
     This function uses the ``dataframe.groupby(key).agg`` method from Pandas.
 
     Parameters
     ----------
-    table : pd.DataFrame,
+    table : pd.DataFrame
         The input dataframe to aggregate.
 
-    key : str or Iterable[str],
+    key : str or Iterable[str]
         The columns used as keys to aggregate on.
 
-    cols_to_agg : str or Iterable[str],
+    cols_to_agg : str or Iterable[str]
         The columns to aggregate.
 
-    num_operations : str or Iterable[str],
+    num_operations : str or Iterable[str], default=("mean",)
         The reduction functions to apply on numerical columns
         in ``cols_to_agg`` during the aggregation.
 
-    categ_operations : str or Iterable[str],
+    categ_operations : str or Iterable[str], default=("mode",)
         The reduction functions to apply on categorical columns
         in ``cols_to_agg`` during the aggregation.
 
     suffix : str, optional
         The suffix appended to output columns.
 
     Returns
     -------
-    group : pd.DataFrame,
+    group : pd.DataFrame
         The aggregated output.
     """
     if not isinstance(table, pd.DataFrame):
         raise TypeError(f"'table' must be a pandas dataframe, got {type(table)!r}.")
 
     key = atleast_1d_or_none(key)
     cols_to_agg = atleast_1d_or_none(cols_to_agg)
@@ -169,18 +169,18 @@
 ):
     """Left join two :obj:`pandas.DataFrame`.
 
     This function uses the ``dataframe.merge`` method from Pandas.
 
     Parameters
     ----------
-    left : pd.DataFrame,
+    left : pd.DataFrame
         The left dataframe to left-join.
 
-    right : pd.DataFrame,
+    right : pd.DataFrame
         The right dataframe to left-join.
 
     left_on : str or Iterable[str]
         Left keys to merge on.
 
     right_on : str or Iterable[str]
         Right keys to merge on.
@@ -205,68 +205,68 @@
 
 def get_named_agg(table, cols, operations):
     """Map aggregation tuples to their output key.
 
     The dictionary has the form: output_key = (column, aggfunc).
     This is used as input for the ``dataframe.agg`` method from Pandas.
 
-    'value_counts' and 'hist' operation require to pivot
+    'value_counts' and 'hist' operations require to pivot
     the tables and treated in a separate mapping.
 
     Parameters
     ----------
-    table : pd.DataFrame,
+    table : pd.DataFrame
         Input dataframe, only used to compute bins values if
         'value_counts' or 'hist' are operations.
 
-    cols : list,
+    cols : list
         The columns to aggregate.
 
-    operations : list,
+    operations : list
         The reduce operations to perform.
 
     Returns
     -------
-    named_agg : dict,
+    named_agg : dict
         Named aggregation mapping.
 
-    value_counts : dict,
+    value_counts : dict
         ``value_counts`` operations mapping.
     """
     named_agg, value_counts = {}, {}
     for col, operation in product(cols, operations):
         op_root, bin_args = _parse_argument(operation)
         aggfunc, bin_args = _get_aggfunc(table[col], op_root, bin_args)
 
         output_key = f"{col}_{op_root}"
-        # 'value_counts' change the index of the resulting frame
+        # 'value_counts' changes the index of the resulting frame
         # and must be treated separately.
         if aggfunc == "value_counts":
             value_counts[output_key] = (col, bin_args)
         else:
             named_agg[output_key] = (col, aggfunc)
 
     return named_agg, value_counts
 
 
 def _parse_argument(operation):
     """Split a text input into a function name and its argument.
 
     Parameters
     ----------
-    operation : str,
+    operation : str
         The operation to parse.
 
     Returns
     -------
-    operation_root : str,
+    operation_root : str
         The name of the operation before parenthesis, if any.
 
-    bin_args : int,
-        The number of bin to create for ``hist`` or ``value_counts``.
+    bin_args : int
+        The number of bin to create for 'hist' or 'value_counts'.
 
     Examples
     --------
     >>> _parse_argument("hist(10)")
     ('hist', 10)
     """
     split = re.split("\\(.+\\)", operation)
@@ -294,30 +294,30 @@
     """Map operation roots to their pandas agg functions.
 
     When args is provided for histogram or value_counts,
     we create args
 
     Parameters
     ----------
-    serie : pd.Series,
-        Input series, used to compute the bins if n_bins is provided.
+    serie : pd.Series
+        Input series, used to compute the bins if `n_bins` is provided.
 
-    op_root : str,
+    op_root : str
         Operation root, the operation without the bin argument, if any.
 
-    n_bins : int,
-        The number of bin to create when value_counts or hist operation are used.
+    n_bins : int
+        The number of bin to create when 'value_counts' or 'hist' operation are used.
 
     Returns
     -------
-    aggfunc : str or callable,
-        The pandas agg functions to perform
+    aggfunc : str or callable
+        The pandas agg functions to perform.
 
-    bins_args : dict,
-        The bins to create when using value_counts or hist.
+    bins_args : dict
+        The bins to create when using 'value_counts' or 'hist'.
     """
     aggfunc = PANDAS_OPS_MAPPING.get(op_root, op_root)
 
     if n_bins is not None:
         # histogram and value_counts
         if aggfunc == "value_counts":
             # If bins is a number, we need to set a fix bin range,
```

### Comparing `skrub-0.1.0/skrub/_dataframe/_polars.py` & `skrub-0.1.1/skrub/_dataframe/_polars.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     dtypes : DataType or mapping of column names to DataType, default=None
         Mapping of column names (or selector) to dtypes, or a single dtype
         to which all columns will be cast.
 
     Returns
     -------
-    X : Polars dataframe
+    X : pl.DataFrame
         Converted output.
     """
     if index is not None:
         raise ValueError(
             "Polars dataframes don't have an index, but "
             f"the Polars dataframe maker was called with {index=!r}."
         )
@@ -62,15 +62,15 @@
         The name of the series.
 
     dtype : DataType, default=None
         Polars dtype of the Series data.
 
     Returns
     -------
-    X : Polars series
+    X : pl.Series
         Converted output.
     """
     if index is not None:
         raise ValueError(
             "Polars series don't have an index, but "
             f"the Polars series maker was called with {index=!r}."
         )
@@ -88,28 +88,28 @@
 ):
     """Aggregate a :obj:`polars.DataFrame` or :obj:`polars.LazyFrame`.
 
     This function uses the ``dataframe.group_by(key).agg`` method from Polars.
 
     Parameters
     ----------
-    table : pl.DataFrame or pl.LazyFrame,
+    table : pl.DataFrame or pl.LazyFrame
         The input dataframe to aggregate.
 
-    key : str or Iterable[str],
+    key : str or Iterable[str]
         The columns used as keys to aggregate on.
 
-    cols_to_agg : str or Iterable[str],
+    cols_to_agg : str or Iterable[str]
         The columns to aggregate.
 
-    num_operations : str or Iterable[str],
+    num_operations : str or Iterable[str], default=("mean",)
         The reduction functions to apply on numerical columns
         in ``cols_to_agg`` during the aggregation.
 
-    categ_operations : str or Iterable[str],
+    categ_operations : str or Iterable[str], default=("mode",)
         The reduction functions to apply on categorical columns
         in ``cols_to_agg`` during the aggregation.
 
     suffix : str,
         The suffix appended to output columns.
 
     Returns
@@ -159,29 +159,29 @@
     Note that the input dataframes type must agree: either both
     Polars dataframes or both Polars lazyframes.
 
     Mixing polars dataframe with lazyframe will raise an error.
 
     Parameters
     ----------
-    left : pl.DataFrame or pl.LazyFrame,
+    left : pl.DataFrame or pl.LazyFrame
         The left dataframe of the left-join.
 
-    right : pl.DataFrame or pl.LazyFrame,
+    right : pl.DataFrame or pl.LazyFrame
         The right dataframe of the left-join.
 
-    left_on : str or Iterable[str],
+    left_on : str or Iterable[str]
         Left keys to merge on.
 
-    right_on : str or Iterable[str],
+    right_on : str or Iterable[str]
         Right keys to merge on.
 
     Returns
     -------
-    merged : pl.DataFrame or pl.LazyFrame,
+    merged : pl.DataFrame or pl.LazyFrame
         The merged output.
     """
     is_dataframe = isinstance(left, pl.DataFrame) and isinstance(right, pl.DataFrame)
     is_lazyframe = isinstance(left, pl.LazyFrame) and isinstance(right, pl.LazyFrame)
     if is_dataframe or is_lazyframe:
         return left.join(
             right,
@@ -200,26 +200,26 @@
     """List Polars aggregation functions.
 
     The list is used as input for the ``dataframe.group_by().agg()`` method from Polars.
     The 'mode' operation needs a flattening post-processing.
 
     Parameters
     ----------
-    cols : list,
+    cols : list
         The columns to aggregate.
 
-    operations : list,
+    operations : list
         The reduce operations to perform.
 
     Returns
     -------
-    aggfuncs : list,
+    aggfuncs : list
         Named aggregation list.
 
-    mode_cols : list,
+    mode_cols : list
         Output keys to post-process after 'mode' aggregation.
     """
     aggfuncs, mode_cols = [], []
     for col, operation in product(cols, operations):
         output_key = f"{col}_{operation}"
         aggfunc = _polars_ops_mapping(col, operation, output_key)
         aggfuncs.append(aggfunc)
@@ -231,24 +231,24 @@
 
 
 def _polars_ops_mapping(col, operation, output_key):
     """Map an operation to its Polars expression.
 
     Parameters
     ----------
-    col : str,
+    col : str
         Name of the column to aggregate.
-    operation : str,
+    operation : str
         Name of the reduce function.
-    output_key : str,
+    output_key : str
         Name of the reduced column.
 
     Returns
     -------
-    aggfunc: polars.Expression,
+    aggfunc: polars.Expression
         The expression to apply.
     """
     polars_aggfuncs = {
         "mean": pl.col(col).mean(),
         "std": pl.col(col).std(),
         "sum": pl.col(col).sum(),
         "min": pl.col(col).min(),
```

### Comparing `skrub-0.1.0/skrub/_dataframe/tests/test_namespace.py` & `skrub-0.1.1/skrub/_dataframe/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/_dataframe/tests/test_pandas.py` & `skrub-0.1.1/skrub/_dataframe/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/_dataframe/tests/test_polars.py` & `skrub-0.1.1/skrub/_dataframe/tests/test_polars.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/_datetime_encoder.py` & `skrub-0.1.1/skrub/_datetime_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,16 @@
     See Also
     --------
     :func:`pandas.to_datetime`
         Convert argument to datetime.
 
     Examples
     --------
+    >>> import pandas as pd
+    >>> from skrub import to_datetime
     >>> X = pd.DataFrame(dict(a=[1, 2], b=["2021-01-01", "2021-02-02"]))
     >>> X
        a          b
     0  1 2021-01-01
     1  2 2021-02-02
     >>> to_datetime(X)
        a          b
@@ -493,22 +495,22 @@
         X_col.astype("int64") / 1e9,
         np.nan,
     )
 
 
 class DatetimeEncoder(TransformerMixin, BaseEstimator):
     """Transforms each datetime column into several numeric columns \
-    for temporal features (e.g year, month, day...).
+    for temporal features (e.g. year, month, day...).
 
     If the dates are timezone aware, all the features extracted will correspond
     to the provided timezone.
 
     Parameters
     ----------
-    resolution : {"year", "month", "day", "hour", "minute", "second",
+    resolution : {"year", "month", "day", "hour", "minute", "second", \
         "microsecond", "nanosecond", None}, default="hour"
         Extract up to this resolution.
         E.g., ``resolution="day"`` generates the features "year", "month",
         "day" only.
         If ``None``, no such feature will be created (but day of the week and \
             total seconds may still be extracted, see below).
 
@@ -549,14 +551,15 @@
         Encode string columns as a numeric array with the minhash method.
 
     SimilarityEncoder :
         Encode string columns as a numeric array with n-gram string similarity.
 
     Examples
     --------
+    >>> from skrub import DatetimeEncoder
     >>> enc = DatetimeEncoder(add_total_seconds=False)
     >>> X = [['2022-10-15'], ['2021-12-25'], ['2020-05-18'], ['2019-10-15 12:00:00']]
     >>> enc.fit(X)
     DatetimeEncoder(add_total_seconds=False)
 
     The encoder will output a transformed array
     with four columns ("year", "month", "day", "hour"):
```

### Comparing `skrub-0.1.0/skrub/_deduplicate.py` & `skrub-0.1.1/skrub/_deduplicate.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
     ngram_range=(2, 4),
     analyzer="char_wb",
     linkage_method="average",
     n_jobs=None,
 ):
     """Deduplicate categorical data by hierarchically clustering similar strings.
 
-    This works best if there is a number of underlying categories that
+    This works best if there are a number of underlying categories that
     sometimes appear in the data with small variations and/or misspellings.
 
     Parameters
     ----------
     X : sequence of str
         The data to be deduplicated.
     n_clusters : int, default=None
@@ -197,21 +197,21 @@
     Examples
     --------
     >>> from skrub.datasets import make_deduplication_data
     >>> duplicated = make_deduplication_data(examples=['black', 'white'],
     ...                                      entries_per_example=[5, 5],
     ...                                      prob_mistake_per_letter=0.3,
     ...                                      random_state=42)
-
     >>> duplicated
     ['blacs', 'black', 'black', 'black', 'black', \
 'uhibe', 'white', 'white', 'white', 'white']
 
     To deduplicate the data, we can build a correspondence matrix:
 
+    >>> from skrub import deduplicate
     >>> deduplicate_correspondence = deduplicate(duplicated)
     >>> deduplicate_correspondence
     blacs    black
     black    black
     black    black
     black    black
     black    black
```

### Comparing `skrub-0.1.0/skrub/_fast_hash.py` & `skrub-0.1.1/skrub/_fast_hash.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/_fuzzy_join.py` & `skrub-0.1.1/skrub/_fuzzy_join.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     left table, unless ``drop_unmatched`` is ``True``, in which case rows that
     are too far from their closest match will not appear in the result. Each
     row from the left table appears at most once in the result; if there are
     several equally good matching rows in the right table one of them will be
     used; which one is unspecified.
 
     To identify the best match for each row, values from the matching columns
-    (``left_key`` and ``right_key``) are vectorized, ie represented by vectors of
+    (``left_key`` and ``right_key``) are vectorized, i.e. represented by vectors of
     continuous values. Then, the Euclidean distances between these vectors are
     computed to find, for each left table row, its nearest neighbor within the
     right table.
 
     Optionally, a maximum distance threshold, ``max_dist``, can be set. Matches
     between vectors that are separated by a distance (strictly) greater than
     ``max_dist`` will be rejected. We will consider that left table rows that
@@ -54,21 +54,21 @@
         those distances.
 
     'second_neighbor'
         The reference distance is the distance to the *second* nearest neighbor
         in the right table.
 
     'self_join_neighbor'
-        Once the match candidate (ie the nearest neigbor from the right
+        Once the match candidate (i.e. the nearest neigbor from the right
         table) has been found, we find its nearest neighbor in the right
         table (excluding itself). The reference distance is the distance that
         separates those 2 right rows.
 
     'no_rescaling'
-        The reference distance is 1.0, ie no rescaling of the distances is
+        The reference distance is 1.0, i.e. no rescaling of the distances is
         applied.
 
     Parameters
     ----------
     left : :obj:`~pandas.DataFrame`
         Left operand of the join.
     right : :obj:`~pandas.DataFrame`
@@ -111,15 +111,15 @@
     add_match_info : bool, default=False
         Insert columns whose names start with `skrub_Joiner` containing
         the distance, rescaled distance and whether the rescaled distance is
         above the threshold. Those values can be helpful for an estimator that
         uses the joined features, or to inspect the result of the join and set
         a ``max_dist`` threshold.
     drop_unmatched : bool, default=False
-        Remove rows for which a match was not found in the right table (ie for
+        Remove rows for which a match was not found in the right table (i.e. for
         which the nearest neighbor is further than `max_dist`).
 
     Returns
     -------
     :obj:`~pandas.DataFrame`
         The joined tables.
 
@@ -127,63 +127,64 @@
     --------
     Joiner :
         Same as fuzzy_join but as a scikit-learn transformer.
 
     Examples
     --------
     >>> import pandas as pd
-    >>> left_table = pd.DataFrame({"Country": ["France", "Italia", "Spain"]})
+    >>> from skrub import fuzzy_join
+    >>> left_table = pd.DataFrame({"Country": ["France", "Italia", "Georgia"]})
     >>> right_table = pd.DataFrame( {"Country": ["Germany", "France", "Italy"],
     ...                            "Capital": ["Berlin", "Paris", "Rome"]} )
     >>> left_table
       Country
     0  France
     1  Italia
-    2   Spain
+    2  Georgia
     >>> right_table
        Country Capital
     0  Germany  Berlin
     1   France   Paris
     2    Italy    Rome
     >>> fuzzy_join(
     ...     left_table,
     ...     right_table,
     ...     on="Country",
-    ...     suffix="_capitals",
-    ...     max_dist=1.0,
+    ...     suffix="_right",
+    ...     max_dist=0.8,
     ...     add_match_info=False,
     ... )
-      Country Country_capitals Capital_capitals
+      Country    Country_right    Capital_right
     0  France           France            Paris
     1  Italia            Italy             Rome
-    2   Spain              NaN              NaN
+    2   Georgia              NaN              NaN
     >>> fuzzy_join(
     ...     left_table,
     ...     right_table,
     ...     on="Country",
-    ...     suffix="_capitals",
+    ...     suffix="_right",
     ...     drop_unmatched=True,
-    ...     max_dist=1.0,
+    ...     max_dist=0.8,
     ...     add_match_info=False,
     ... )
-      Country Country_capitals Capital_capitals
+      Country    Country_right    Capital_right
     0  France           France            Paris
     1  Italia            Italy             Rome
     >>> fuzzy_join(
     ...     left_table,
     ...     right_table,
     ...     on="Country",
-    ...     suffix="_capitals",
+    ...     suffix="_right",
     ...     max_dist=float("inf"),
     ...     add_match_info=False,
     ... )
-      Country Country_capitals Capital_capitals
+      Country    Country_right    Capital_right
     0  France           France            Paris
-    1  Italia            Italy             Rome
-    2   Spain          Germany           Berlin
+    1  Italia           Italy             Rome
+    2  Georgia          Germany           Berlin
     """
     # duplicate the key checks performed by the Joiner so we can get better
     # names in error messages
     left_key, right_key = _join_utils.check_key(
         left_on,
         right_on,
         on,
```

### Comparing `skrub-0.1.0/skrub/_gap_encoder.py` & `skrub-0.1.1/skrub/_gap_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -712,21 +712,21 @@
     ----------
     For a detailed description of the method, see
     `Encoding high-cardinality string categorical variables
     <https://hal.inria.fr/hal-02171256v4>`_ by Cerda, Varoquaux (2019).
 
     Examples
     --------
+    >>> from skrub import GapEncoder
     >>> enc = GapEncoder(n_components=2, random_state=0)
 
     Let's encode the following non-normalized data:
 
     >>> X = [['paris, FR'], ['Paris'], ['London, UK'], ['Paris, France'],
     ...      ['london'], ['London, England'], ['London'], ['Pqris']]
-
     >>> enc.fit(X)
     GapEncoder(n_components=2, random_state=0)
 
     The GapEncoder has found the following two topics:
 
     >>> enc.get_feature_names_out()
     array(['england, london, uk', 'france, paris, pqris'], dtype=object)
```

### Comparing `skrub-0.1.0/skrub/_interpolation_joiner.py` & `skrub-0.1.1/skrub/_interpolation_joiner.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,18 @@
         argument of ``transform``). ``aux_table`` is used to train a model that
         takes as inputs the contents of the columns listed in ``aux_key``, and
         predicts the contents of the other columns. In the example above, we
         want our transformer to add temperature data to the table it is
         operating on. Therefore, ``aux_table`` is the ``annual_avg_temp``
         table.
 
+    key : list of str, or str
+        Column names to use for both `main_key` and `aux_key`, when they are
+        the same. Provide either `key` (only) or both `main_key` and `aux_key`.
+
     main_key : list of str, or str
         The columns in the main table used for joining. The main table is the
         argument of ``transform``, to which we add information inferred using
         ``aux_table``. The column names listed in ``main_key`` will provide the
         inputs (features) of the interpolators at prediction (joining) time. In
         the example above, ``main_key`` is ``["latitude", "longitude"]``, which
         refer to columns in the ``buildings`` table. When joining on a single
@@ -65,18 +69,14 @@
     aux_key : list of str, or str
         The columns in ``aux_table`` used for joining. Their number and types
         must match those of the ``main_key`` columns in the main table. These
         columns provide the features for the estimators to be fitted. As for
         ``main_key``, it is possible to pass a string when using a single
         column.
 
-    key : list of str, or str
-        Column names to use for both `main_key` and `aux_key`, when they are
-        the same. Provide either `key` (only) or both `main_key` and `aux_key`.
-
     suffix : str
         Suffix to append to the ``aux_table``'s column names. You can use it
         to avoid duplicate column names in the join.
 
     regressor : scikit-learn regressor
         Model used to predict the numerical columns of ``aux_table``.
 
@@ -132,57 +132,58 @@
     --------
     Joiner :
         Works in a similar way but instead of inferring values, picks the
         closest row from the auxiliary table.
 
     Examples
     --------
+    >>> import pandas as pd
     >>> buildings = pd.DataFrame(
     ...     {"latitude": [1.0, 2.0], "longitude": [1.0, 2.0], "n_stories": [3, 7]}
     ... )
     >>> annual_avg_temp = pd.DataFrame(
     ...     {
     ...         "latitude": [1.2, 0.9, 1.9, 1.7, 5.0],
     ...         "longitude": [0.8, 1.1, 1.8, 1.8, 5.0],
     ...         "avg_temp": [10.0, 11.0, 15.0, 16.0, 20.0],
     ...     }
     ... )
-
     >>> buildings
        latitude  longitude  n_stories
     0       1.0        1.0          3
     1       2.0        2.0          7
-
     >>> annual_avg_temp
        latitude  longitude  avg_temp
     0       1.2        0.8      10.0
     1       0.9        1.1      11.0
     2       1.9        1.8      15.0
     3       1.7        1.8      16.0
     4       5.0        5.0      20.0
 
-    >>> from sklearn.neighbors import KNeighborsRegressor
+    Let's interpolate the average temperature:
 
+    >>> from sklearn.neighbors import KNeighborsRegressor
+    >>> from skrub import InterpolationJoiner
     >>> InterpolationJoiner(
     ...     annual_avg_temp,
     ...     key=["latitude", "longitude"],
     ...     regressor=KNeighborsRegressor(2),
     ... ).fit_transform(buildings)
        latitude  longitude  n_stories  avg_temp
     0       1.0        1.0          3      10.5
     1       2.0        2.0          7      15.5
     """
 
     def __init__(
         self,
         aux_table,
         *,
+        key=None,
         main_key=None,
         aux_key=None,
-        key=None,
         suffix="",
         regressor=DEFAULT_REGRESSOR,
         classifier=DEFAULT_CLASSIFIER,
         vectorizer=DEFAULT_VECTORIZER,
         n_jobs=None,
         on_estimator_failure="warn",
     ):
```

### Comparing `skrub-0.1.0/skrub/_join_utils.py` & `skrub-0.1.1/skrub/_join_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,29 +21,30 @@
     the `main_key` and `aux_key` to use, as lists of strings.
 
     Parameters
     ----------
     main_key : list of str, str, or None
         Matching columns in the main table. Can be a single column name (str)
         if matching on a single column: ``"User_ID"`` is the same as
-        ``"[User_ID]"``.
+        ``["User_ID"]``.
     aux_key : list of str, str, or None
         Matching columns in the auxiliary table. Can be a single column name (str)
         if matching on a single column: ``"User_ID"`` is the same as
-        ``"[User_ID]"``.
+        ``["User_ID"]``.
     key : list of str, str, or None
         Can be provided in place of `main_key` and `aux_key` when they are the
         same. We must provide non-``None`` values for either `key` or both
         `main_key` and `aux_key`.
-    main_key_name : str
+    main_key_name : str, default="main_key"
         How to refer to `main_key` in error messages.
-    aux_key_name : str
+    aux_key_name : str, default="aux_key"
         How to refer to `aux_key` in error messages.
-    key_name : str
+    key_name : str, default="key"
         How to refer to `key` in error messages.
+
     Returns
     -------
     main_key, aux_key : pair (tuple) of lists of str
         The correct sets of matching columns to use, each provided as a list of
         column names.
     """
     if key is not None:
```

### Comparing `skrub-0.1.0/skrub/_joiner.py` & `skrub-0.1.1/skrub/_joiner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 The Joiner provides fuzzy joining as a scikit-learn transformer.
 """
+
 import numpy as np
 import pandas as pd
 from sklearn.base import BaseEstimator, TransformerMixin, clone
 from sklearn.compose import make_column_transformer
 from sklearn.feature_extraction.text import HashingVectorizer, TfidfTransformer
 from sklearn.pipeline import make_pipeline
 from sklearn.preprocessing import FunctionTransformer, StandardScaler
 from sklearn.utils.validation import check_is_fitted
 
-from skrub import _join_utils, _matching
+from skrub import _join_utils, _matching, _utils
 from skrub._dataframe._namespace import is_pandas, is_polars
 from skrub._datetime_encoder import DatetimeEncoder
 
 
 def _as_str(column):
     return column.fillna("").astype(str)
 
@@ -37,15 +38,15 @@
 
 
 def _make_vectorizer(table, string_encoder, rescale):
     """Construct the transformer used to vectorize joining columns.
 
     The resulting ColumnTransformer applies TFIDF transformation to string
     columns, DatetimeEncoder to datetimes and passthrough to numeric columns.
-    In addition if ``rescale`` is ``True``, a StandardScaler is applied to
+    In addition if `rescale` is `True`, a StandardScaler is applied to
     numeric and datetime columns.
     """
     transformers = [
         (clone(string_encoder), c)
         for c in table.select_dtypes(include=["string", "category", "object"]).columns
     ]
     num_columns = table.select_dtypes(include="number").columns
@@ -66,175 +67,176 @@
         )
     return make_column_transformer(*transformers)
 
 
 class Joiner(TransformerMixin, BaseEstimator):
     """Augment features in a main table by fuzzy-joining an auxiliary table to it.
 
-    This transformer is initialized with an auxiliary table ``aux_table``. It
+    This transformer is initialized with an auxiliary table `aux_table`. It
     transforms a main table by joining it, with approximate ("fuzzy") matching,
-    to the auxiliary table. The output of ``transform`` has the same rows as
-    the main table (ie as the argument passed to ``transform``), but each row
+    to the auxiliary table. The output of `transform` has the same rows as
+    the main table (i.e. as the argument passed to `transform`), but each row
     is augmented with values from the best match in the auxiliary table.
 
     To identify the best match for each row, values from the matching columns
-    (``main_key`` and ``aux_key``) are vectorized, ie represented by vectors of
+    (`main_key` and `aux_key`) are vectorized, i.e. represented by vectors of
     continuous values. Then, the Euclidean distances between these vectors are
     computed to find, for each main table row, its nearest neighbor within the
     auxiliary table.
 
-    Optionally, a maximum distance threshold, ``max_dist``, can be set. Matches
+    Optionally, a maximum distance threshold, `max_dist`, can be set. Matches
     between vectors that are separated by a distance (strictly) greater than
-    ``max_dist`` will be rejected. We will consider that main table rows that
-    are farther than ``max_dist`` from their nearest neighbor do not have a
+    `max_dist` will be rejected. We will consider that main table rows that
+    are farther than `max_dist` from their nearest neighbor do not have a
     matching row in the auxiliary table, and the output will contain nulls for
     the entries that would normally have come from the auxiliary table (as in a
     traditional left join).
 
-    To make it easier to set a ``max_dist`` threshold, the distances are
+    To make it easier to set a `max_dist` threshold, the distances are
     rescaled by dividing them by a reference distance, which can be chosen with
-    ``ref_dist``. The default is ``'random_pairs'``. The possible choices are:
+    `ref_dist`. The default is `'random_pairs'`. The possible choices are:
 
     'random_pairs'
         Pairs of rows are sampled randomly from the auxiliary table and their
         distance is computed. The reference distance is the first quartile of
         those distances.
 
     'second_neighbor'
         The reference distance is the distance to the *second* nearest neighbor
         in the auxiliary table.
 
     'self_join_neighbor'
-        Once the match candidate (ie the nearest neigbor from the auxiliary
+        Once the match candidate (i.e. the nearest neigbor from the auxiliary
         table) has been found, we find its nearest neighbor in the auxiliary
         table (excluding itself). The reference distance is the distance that
         separates those 2 auxiliary rows.
 
     'no_rescaling'
-        The reference distance is 1.0, ie no rescaling of the distances is
+        The reference distance is 1.0, i.e. no rescaling of the distances is
         applied.
 
     Parameters
     ----------
     aux_table : :obj:`~pandas.DataFrame`
         The auxiliary table, which will be fuzzy-joined to the main table when
-        calling ``transform``.
-    main_key : str or list of str, default=None
+        calling `transform`.
+    key : str or iterable of str, default=None
+        The column names to use for both `main_key` and `aux_key` when they
+        are the same. Provide either `key` or both `main_key` and `aux_key`.
+    main_key : str or iterable of str, default=None
         The column names in the main table on which the join will be performed.
         Can be a string if joining on a single column.
-        If ``None``, `aux_key` must also be ``None`` and `key` must be provided.
-    aux_key : str or list of str, default=None
+        If `None`, `aux_key` must also be `None` and `key` must be provided.
+    aux_key : str or iterable of str, default=None
         The column names in the auxiliary table on which the join will
         be performed. Can be a string if joining on a single column.
-        If ``None``, `main_key` must also be ``None`` and `key` must be provided.
-    key : str or list of str, default=None
-        The column names to use for both ``main_key`` and ``aux_key`` when they
-        are the same. Provide either ``key`` or both ``main_key`` and ``aux_key``.
+        If `None`, `main_key` must also be `None` and `key` must be provided.
     suffix : str, default=""
-        Suffix to append to the ``aux_table``'s column names. You can use it
+        Suffix to append to the `aux_table`'s column names. You can use it
         to avoid duplicate column names in the join.
     max_dist : float, default=np.inf
         Maximum acceptable (rescaled) distance between a row in the
-        ``main_table`` and its nearest neighbor in the ``aux_table``. Rows that
+        `main_table` and its nearest neighbor in the `aux_table`. Rows that
         are farther apart are not considered to match. By default, the distance
         is rescaled so that a value between 0 and 1 is typically a good choice,
         although rescaled distances can be greater than 1 for some choices of
-        ``ref_dist``. ``None``, ``"inf"``, ``float("inf")`` or ``numpy.inf``
+        `ref_dist`. `None`, `"inf"`, `float("inf")` or `numpy.inf`
         mean that no matches are rejected.
     ref_dist : reference distance for rescaling, default = 'random_pairs'
         Options are {"random_pairs", "second_neighbor", "self_join_neighbor",
         "no_rescaling"}. See above for a description of each option. To
-        facilitate the choice of ``max_dist``, distances between rows in
-        ``main_table`` and their nearest neighbor in ``aux_table`` will be
+        facilitate the choice of `max_dist`, distances between rows in
+        `main_table` and their nearest neighbor in `aux_table` will be
         rescaled by this reference distance.
     string_encoder : scikit-learn transformer used to vectorize text columns
-        By default a ``HashingVectorizer`` combined with a ``TfidfTransformer``
+        By default a `HashingVectorizer` combined with a `TfidfTransformer`
         is used. Here we use raw TF-IDF features rather than transforming them
-        for example with ``GapEncoder`` or ``MinHashEncoder`` because it is
+        for example with `GapEncoder` or `MinHashEncoder` because it is
         faster, these features are only used to find nearest neighbors and not
         used by downstream estimators, and distances between TF-IDF vectors
         have a somewhat simpler interpretation.
     add_match_info : bool, default=True
         Insert some columns whose names start with `skrub_Joiner` containing
         the distance, rescaled distance and whether the rescaled distance is
         above the threshold. Those values can be helpful for an estimator that
         uses the joined features, or to inspect the result of the join and set
-        a ``max_dist`` threshold.
+        a `max_dist` threshold.
 
     Attributes
     ----------
     max_dist_ : the maximum distance for a match to be accepted
-        Equal to the parameter ``max_dist`` except that ``"inf"`` and ``None``
-        are mapped to ``np.inf`` (ie accept all matches).
+        Equal to the parameter `max_dist` except that `"inf"` and `None`
+        are mapped to `np.inf` (i.e. accept all matches).
 
     vectorizer_ : scikit-learn ColumnTransformer
         The fitted transformer used to transform the matching columns into
         numerical vectors.
 
     See Also
     --------
     AggJoiner :
         Aggregate auxiliary dataframes before joining them on a base dataframe.
 
     fuzzy_join :
         Join two tables (dataframes) based on approximate column matching. This
-        is the same functionality as provided by the ``Joiner`` but exposed as
+        is the same functionality as provided by the `Joiner` but exposed as
         a function rather than a transformer.
 
     Examples
     --------
     >>> import pandas as pd
-    >>> main_table = pd.DataFrame({"Country": ["France", "Italia", "Spain"]})
+    >>> from skrub import Joiner
+    >>> main_table = pd.DataFrame({"Country": ["France", "Italia", "Georgia"]})
     >>> aux_table = pd.DataFrame( {"Country": ["Germany", "France", "Italy"],
     ...                            "Capital": ["Berlin", "Paris", "Rome"]} )
     >>> main_table
       Country
     0  France
     1  Italia
-    2   Spain
+    2   Georgia
     >>> aux_table
        Country Capital
     0  Germany  Berlin
     1   France   Paris
     2    Italy    Rome
     >>> joiner = Joiner(
     ...     aux_table,
     ...     key="Country",
-    ...     suffix="_capitals",
-    ...     max_dist=0.9,
+    ...     suffix="_aux",
+    ...     max_dist=0.8,
     ...     add_match_info=False,
     ... )
     >>> joiner.fit_transform(main_table)
-      Country Country_capitals Capital_capitals
+      Country      Country_aux      Capital_aux
     0  France           France            Paris
     1  Italia            Italy             Rome
-    2   Spain              NaN              NaN
+    2  Georgia              NaN              NaN
     """
 
     _match_info_keys = ["distance", "rescaled_distance", "match_accepted"]
     _match_info_key_renaming = {k: f"skrub_Joiner_{k}" for k in _match_info_keys}
     match_info_columns = list(_match_info_key_renaming.values())
 
     def __init__(
         self,
         aux_table,
         *,
+        key=None,
         main_key=None,
         aux_key=None,
-        key=None,
         suffix="",
         max_dist=np.inf,
         ref_dist=DEFAULT_REF_DIST,
         string_encoder=DEFAULT_STRING_ENCODER,
         add_match_info=True,
     ):
         self.aux_table = aux_table
+        self.key = key
         self.main_key = main_key
         self.aux_key = aux_key
-        self.key = key
         self.suffix = suffix
         self.max_dist = max_dist
         self.ref_dist = ref_dist
         self.string_encoder = (
             clone(string_encoder)
             if string_encoder is DEFAULT_STRING_ENCODER
             else string_encoder
@@ -319,38 +321,44 @@
 
         Returns
         -------
         :obj:`~pandas.DataFrame`
             The final joined table.
         """
         del y
+        check_is_fitted(self, "vectorizer_")
         input_is_polars = is_polars(X)
         X = self._check_dataframe(X)
-        check_is_fitted(self, "vectorizer_")
         _join_utils.check_missing_columns(X, self._main_key, "'X' (the main table)")
         _join_utils.check_column_name_duplicates(
             X, self._aux_table, self.suffix, main_table_name="X"
         )
         main = self.vectorizer_.transform(
             X[self._main_key].set_axis(self._aux_key, axis="columns")
         )
         match_result = self._matching.match(main, self.max_dist_)
         aux_table = _join_utils.add_column_name_suffix(
             self._aux_table, self.suffix
         ).reset_index(drop=True)
         matching_col = match_result["index"].copy()
         matching_col[~match_result["match_accepted"]] = -1
+        token = _utils.random_string()
+        left_key_name = f"skrub_left_key_{token}"
+        right_key_name = f"skrub_right_key_{token}"
+        left = X.assign(**{left_key_name: matching_col})
+        right = aux_table.assign(**{right_key_name: np.arange(aux_table.shape[0])})
         join = pd.merge(
-            X,
-            aux_table,
-            left_on=matching_col,
-            right_index=True,
+            left,
+            right,
+            left_on=left_key_name,
+            right_on=right_key_name,
             suffixes=("", ""),
             how="left",
         )
+        join = join.drop([left_key_name, right_key_name], axis=1)
         if self.add_match_info:
             for info_key, info_col_name in self._match_info_key_renaming.items():
                 join[info_col_name] = match_result[info_key]
         if input_is_polars:
             import polars as pl
 
             join = pl.from_pandas(join)
```

### Comparing `skrub-0.1.0/skrub/_matching.py` & `skrub-0.1.1/skrub/_matching.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/_select_cols.py` & `skrub-0.1.1/skrub/_select_cols.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     cols : list of str or str
         The columns to select. A single column name can be passed as a ``str``:
         ``"col_name"`` is the same as ``["col_name"]``.
 
     Examples
     --------
     >>> import pandas as pd
+    >>> from skrub import SelectCols
     >>> df = pd.DataFrame({"A": [1, 2], "B": [10, 20], "C": ["x", "y"]})
     >>> df
        A   B  C
     0  1  10  x
     1  2  20  y
     >>> SelectCols(["C", "A"]).fit_transform(df)
        C  A
@@ -118,14 +119,15 @@
     cols : list of str or str
         The columns to drop. A single column name can be passed as a ``str``:
         ``"col_name"`` is the same as ``["col_name"]``.
 
     Examples
     --------
     >>> import pandas as pd
+    >>> from skrub import DropCols
     >>> df = pd.DataFrame({"A": [1, 2], "B": [10, 20], "C": ["x", "y"]})
     >>> df
        A   B  C
     0  1  10  x
     1  2  20  y
     >>> DropCols(["A", "C"]).fit_transform(df)
         B
```

### Comparing `skrub-0.1.0/skrub/_similarity_encoder.py` & `skrub-0.1.1/skrub/_similarity_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import pandas as pd
 import sklearn
 from joblib import Parallel, delayed
 from numpy.typing import ArrayLike, NDArray
 from scipy import sparse
 from sklearn.feature_extraction.text import CountVectorizer, HashingVectorizer
 from sklearn.preprocessing import OneHotEncoder
-from sklearn.utils import parse_version
+from sklearn.utils.fixes import parse_version
 from sklearn.utils.validation import check_is_fitted
 
 from ._string_distances import get_ngram_count, preprocess
 
 # Ignore lines too long, first docstring lines can't be cut
 # flake8: noqa: E501
 
@@ -235,14 +235,15 @@
     For a detailed description of the method, see
     `Similarity encoding for learning with dirty categorical variables
     <https://hal.inria.fr/hal-01806175>`_ by Cerda, Varoquaux, Kegl. 2018
     (Machine Learning journal, Springer).
 
     Examples
     --------
+    >>> from skrub import SimilarityEncoder
     >>> enc = SimilarityEncoder()
     >>> X = [['Male', 1], ['Female', 3], ['Female', 2]]
     >>> enc.fit(X)
     SimilarityEncoder()
 
     It inherits the same methods as theOneHotEncoder:
 
@@ -251,15 +252,14 @@
 
     But it provides a continuous encoding based on similarity
     instead of a discrete one based on exact matches:
 
     >>> enc.transform([['Female', 1], ['Male', 4]])
     array([[1.        , 0.42..., 1.        , 0.        , 0.        ],
            [0.42..., 1.        , 0.        , 0.        , 0.        ]])
-
     >>> enc.get_feature_names_out(['gender', 'group'])
     array(['gender_Female', 'gender_Male', 'group_1', 'group_2', 'group_3'],
           dtype=object)
     """
 
     categories_: list[NDArray]
     n_features_in_: int
```

### Comparing `skrub-0.1.0/skrub/_string_distances.py` & `skrub-0.1.1/skrub/_string_distances.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/_table_vectorizer.py` & `skrub-0.1.1/skrub/_table_vectorizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 )
 from scipy import sparse
 from sklearn.base import BaseEstimator, TransformerMixin, clone
 from sklearn.compose import ColumnTransformer
 from sklearn.compose._column_transformer import _get_transformer_list
 from sklearn.preprocessing import OneHotEncoder
 from sklearn.utils import Bunch
+from sklearn.utils._set_output import _get_output_config, _safe_set_output
 from sklearn.utils.validation import check_is_fitted
 
 from skrub import DatetimeEncoder, GapEncoder, to_datetime
 from skrub._utils import clone_if_default
 
 HIGH_CARDINALITY_TRANSFORMER = GapEncoder(n_components=30)
 LOW_CARDINALITY_TRANSFORMER = OneHotEncoder(
@@ -190,28 +191,30 @@
         (so they count in the cardinality).
 
     low_cardinality_transformer : {'drop', 'remainder', 'passthrough'} \
         or Transformer, optional
         Transformer used on categorical/string features with low cardinality
         (threshold is defined by `cardinality_threshold`).
         Can either be a:
-        - transformer object instance (e.g. OneHotEncoder)
-        - a Pipeline containing the preprocessing steps
-        - 'drop' for dropping the columns
-        - 'remainder' for applying `remainder`
-        - 'passthrough' to return the unencoded columns
 
-        The default transformer is
-            ```
+        * transformer object instance (e.g. ``OneHotEncoder``)
+        * a Pipeline containing the preprocessing steps
+        * 'drop' for dropping the columns
+        * 'remainder' for applying `remainder`
+        * 'passthrough' to return the unencoded columns
+
+        The default transformer is:
+
+        .. code-block::
+
             OneHotEncoder(
                 handle_unknown='ignore',
                 drop='if_binary',
                 sparse_output=False,
             )
-            ```
 
         When the downstream estimator is a tree-based model
         (e.g., scikit-learn HistGradientBoostingRegressor), the OneHotEncoder
         may lead to lower performances than other transformers,
         such as the OrdinalEncoder.
 
     high_cardinality_transformer : {'drop', 'remainder', 'passthrough'} \
@@ -249,29 +252,31 @@
         On top of the default column type classification (see parameters above),
         this parameter allows you to manually specify transformers for
         specific columns.
         This is equivalent to using a ColumnTransformer for assigning the
         column-specific transformers, and passing the ``TableVectorizer``
         as the ``remainder``.
         This parameter can take two different formats, either:
-        - a list of 2-tuples (transformer, column names or indices)
-        - a list of 3-tuple (name, transformer, column names or indices)
+
+        * a list of 2-tuples (transformer, column names or indices)
+        * a list of 3-tuple (name, transformer, column names or indices)
         In the latter format, you can specify the name of the assignment.
         Mixing the two is not supported.
 
     auto_cast : bool, default=True
         If set to ``True``, calling ``fit``, ``transform`` or ``fit_transform``
         will call ``_auto_cast`` to convert each column to the "optimal" dtype
         for scikit-learn estimators.
         The main heuristics are the following:
-        - pandas extension dtypes conversion to numpy dtype
-        - datetime conversion using ``skrub.to_datetime``
-        - numeric conversion using ``pandas.to_numeric``
-        - numeric columns with missing values are converted to float to input np.nan
-        - categorical columns dtypes are updated with the new entries (if any)
+
+        * pandas extension dtypes conversion to numpy dtype
+        * datetime conversion using ``skrub.to_datetime``
+        * numeric conversion using ``pandas.to_numeric``
+        * numeric columns with missing values are converted to float to input np.nan
+        * categorical columns dtypes are updated with the new entries (if any) \
           during transform.
 
     remainder : {'drop', 'passthrough'} or Transformer, default='passthrough'
         By default, all remaining columns that were not specified in `transformers`
         will be automatically passed through. This subset of columns is concatenated
         with the output of the transformers. (default 'passthrough').
         By specifying ``remainder='drop'``, only the specified columns
@@ -360,24 +365,24 @@
     >>> from skrub.datasets import fetch_employee_salaries
     >>> ds = fetch_employee_salaries()
     >>> ds.X.head(3)
       gender department  ... date_first_hired year_first_hired
     0      F        POL  ...       09/22/1986             1986
     1      M        POL  ...       09/12/1988             1988
     2      F        HHS  ...       11/19/1989             1989
-    [3 rows x 8 columns]
 
+    >>> from skrub import TableVectorizer
     >>> tv = TableVectorizer()
     >>> tv.fit(ds.X)
     TableVectorizer()
 
     Now, we can inspect the transformers assigned to each column:
 
     >>> tv.transformers_
-    [('numeric', 'passthrough', ['year_first_hired']), \
+    [('numeric', ..., ['year_first_hired']), \
 ('datetime', DatetimeEncoder(), ['date_first_hired']), \
 ('low_cardinality', OneHotEncoder(drop='if_binary', handle_unknown='ignore', \
 sparse_output=False), \
 ['gender', 'department', 'department_name', 'assignment_category']), \
 ('high_cardinality', GapEncoder(n_components=30), \
     ['division', 'employee_position_title'])]
     """
@@ -560,15 +565,20 @@
             if X_array.ndim == 1:
                 raise ValueError(
                     f"Expected 2D array, got 1D array instead:\narray={X}.\n"
                     "Reshape your data either using array.reshape(-1, 1) if "
                     "your data has a single feature or array.reshape(1, -1) "
                     "if it contains a single sample."
                 )
-            feature_names = getattr(self, "feature_names_in_", None)
+            feature_names = getattr(
+                self,
+                "feature_names_in_",
+                # by default, we will use "x0", "x1", ...
+                np.asarray([f"x{i}" for i in range(X_array.shape[1])], dtype=object),
+            )
             X = pd.DataFrame(X_array, columns=feature_names)
         else:
             # Create a copy to avoid altering the original data.
             X = X.copy()
 
         # Check for duplicate column names.
         duplicate_columns = {k for k, v in Counter(X.columns).items() if v > 1}
@@ -713,14 +723,19 @@
             remainder=self.remainder,
             sparse_threshold=self.sparse_threshold,
             n_jobs=1,  # we don't parallelize the outer loop
             transformer_weights=self.transformer_weights,
             verbose=self.verbose,
             verbose_feature_names_out=self.verbose_feature_names_out,
         )
+        if hasattr(self, "_sklearn_output_config"):
+            _safe_set_output(
+                self._column_transformer,
+                transform=_get_output_config("transform", self)["dense"],
+            )
 
         X_enc = self._column_transformer.fit_transform(X, y=y)
 
         return X_enc
 
     def transform(self, X):
         """Transform ``X`` by applying the fitted transformers on the columns.
```

### Comparing `skrub-0.1.0/skrub/_utils.py` & `skrub-0.1.1/skrub/_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import collections
 import importlib
 import re
+import secrets
 from collections.abc import Hashable
 from typing import Any, Iterable
 
 import numpy as np
 from numpy.typing import NDArray
 from sklearn.base import clone
 from sklearn.utils import check_array
@@ -158,7 +159,11 @@
     # 1d array
     else:
         return [x]
 
 
 def clone_if_default(estimator, default_estimator):
     return clone(estimator) if estimator is default_estimator else estimator
+
+
+def random_string():
+    return secrets.token_hex()[:8]
```

### Comparing `skrub-0.1.0/skrub/datasets/__init__.py` & `skrub-0.1.1/skrub/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/datasets/_fetching.py` & `skrub-0.1.1/skrub/datasets/_fetching.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from urllib.error import URLError
 from zipfile import BadZipFile, ZipFile
 
 import pandas as pd
 from sklearn import __version__ as sklearn_version
 from sklearn.datasets import fetch_openml
 from sklearn.datasets._base import _sha256
-from sklearn.utils import parse_version
+from sklearn.utils.fixes import parse_version
 
 from skrub._utils import import_optional_dependency
 from skrub.datasets._utils import get_data_dir
 
 # Ignore lines too long, first docstring lines can't be cut
 # flake8: noqa: E501
```

### Comparing `skrub-0.1.0/skrub/datasets/_generating.py` & `skrub-0.1.1/skrub/datasets/_generating.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/datasets/_ken_embeddings.py` & `skrub-0.1.1/skrub/datasets/_ken_embeddings.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,14 @@
     >>> games_embedding.head() # doctest: +SKIP
                              Entity  ...      X199
     0             A_Little_Princess  ...  0.04...
     1                 The_Dark_Half  ... -0.00...
     2                  Frankenstein  ... -0.11...
     3                 Albert_Wesker  ... -0.16...
     4  Harukanaru_Toki_no_Naka_de_3  ...  0.14...
-    [5 rows x 202 columns]
 
     Extracts all embeddings with the "games" type.
     For the list of existing types see fetch_ken_types.
 
     Some tables are available pre-filtered for us using the
     `embedding_table_id` parameter:
 
@@ -236,15 +235,14 @@
     >>> games_embedding_fast.head() # doctest: +SKIP
                          Entity  ...      X199
     0              R-Type_Delta  ...  0.04...
     1  Just_Add_Water_(company)  ... -0.02...
     2                 Li_Xiayan  ...  0.00...
     3             Vampire_Night  ... -0.14...
     4               Shatterhand  ...  0.19...
-    [5 rows x 202 columns]
 
     It takes less time to load the wanted output, and is more precise as the
     types have been carefully filtered out.
     For a list of pre-filtered tables, see func:`fetch_ken_table_aliases`.
     """
     if embedding_table_id in fetch_ken_table_aliases():
         correspondence = pd.read_csv(_correspondence_table_url)
```

### Comparing `skrub-0.1.0/skrub/datasets/_utils.py` & `skrub-0.1.1/skrub/datasets/_utils.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/datasets/tests/test_fetching.py` & `skrub-0.1.1/skrub/datasets/tests/test_fetching.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/datasets/tests/test_generating.py` & `skrub-0.1.1/skrub/datasets/tests/test_generating.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/datasets/tests/test_ken_embeddings.py` & `skrub-0.1.1/skrub/datasets/tests/test_ken_embeddings.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,14 +29,17 @@
     types2 = fetch_ken_types(search="game")
     assert types2.shape[0] == 2540
     # Tests the negative filter works
     types3 = fetch_ken_types(search="game", exclude="card")
     assert types3.shape[0] == 2532
 
 
+# TODO: mock download in test & make download more robust & better error messages
+# See https://github.com/skrub-data/skrub/issues/900
+@pytest.mark.skip("Downloads large files and fails CI unpredictably")
 def test_small_ken_embeddings():
     """
     Test if small sized embeddings were fetched correctly
     """
     pytest.importorskip("pyarrow")
     emb = fetch_ken_embeddings(
         search_types="game_designers",
@@ -50,14 +53,17 @@
         embedding_table_id="39254360",
         embedding_type_id="39266678",
         pca_components=5,
     )
     assert emb2.shape[1] == 7
 
 
+# TODO: mock download in test & make download more robust & better error messages
+# See https://github.com/skrub-data/skrub/issues/900
+@pytest.mark.skip("Downloads large files and fails CI unpredictably")
 def test_big_ken_embeddings():
     """
     Test if bigger sized embeddings were fetched correctly
     """
     pytest.importorskip("pyarrow")
     # With custom figshare ID's:
     emb3 = fetch_ken_embeddings(
```

### Comparing `skrub-0.1.0/skrub/datasets/tests/test_utils.py` & `skrub-0.1.1/skrub/datasets/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/tests/test_agg_joiner.py` & `skrub-0.1.1/skrub/tests/test_agg_joiner.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/tests/test_datetime_encoder.py` & `skrub-0.1.1/skrub/tests/test_datetime_encoder.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/tests/test_deduplicate.py` & `skrub-0.1.1/skrub/tests/test_deduplicate.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/tests/test_docstrings.py` & `skrub-0.1.1/skrub/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/tests/test_fast_hash.py` & `skrub-0.1.1/skrub/tests/test_fast_hash.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/tests/test_fuzzy_join.py` & `skrub-0.1.1/skrub/tests/test_fuzzy_join.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/tests/test_gap_encoder.py` & `skrub-0.1.1/skrub/tests/test_gap_encoder.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/tests/test_interpolation_join.py` & `skrub-0.1.1/skrub/tests/test_interpolation_join.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/tests/test_join_utils.py` & `skrub-0.1.1/skrub/tests/test_join_utils.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/tests/test_joiner.py` & `skrub-0.1.1/skrub/tests/test_joiner.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         aux_table=df2, aux_key="CA", main_key="Ca", add_match_info=False
     )
     result = joiner_list.fit_transform(df)
     assert_frame_equal_(result, expected)
 
 
 def test_pandas_aux_table_index():
-    main_table = pd.DataFrame({"Country": ["France", "Italia", "Spain"]})
+    main_table = pd.DataFrame({"Country": ["France", "Italia", "Georgia"]})
     aux_table = pd.DataFrame(
         {
             "Country": ["Germany", "France", "Italy"],
             "Capital": ["Berlin", "Paris", "Rome"],
         }
     )
     aux_table.index = [2, 1, 0]
```

### Comparing `skrub-0.1.0/skrub/tests/test_matching.py` & `skrub-0.1.1/skrub/tests/test_matching.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/tests/test_minhash_encoder.py` & `skrub-0.1.1/skrub/tests/test_minhash_encoder.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/tests/test_select_cols.py` & `skrub-0.1.1/skrub/tests/test_select_cols.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/tests/test_similarity_encoder.py` & `skrub-0.1.1/skrub/tests/test_similarity_encoder.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/tests/test_sklearn.py` & `skrub-0.1.1/skrub/tests/test_sklearn.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import numpy as np
 import pytest
 import sklearn
 from sklearn.metrics.pairwise import linear_kernel, pairwise_distances
-from sklearn.utils import parse_version
 from sklearn.utils._tags import _safe_tags
 from sklearn.utils.estimator_checks import _is_pairwise_metric, parametrize_with_checks
 
 from skrub import (  # isort:skip
     DatetimeEncoder,
     # Joiner,
     GapEncoder,
@@ -70,14 +69,13 @@
     ]:
         yield Estimator()
 
 
 # TODO: remove the skip when the scikit-learn common test will be more lenient towards
 # the string categorical data:
 # xref: https://github.com/scikit-learn/scikit-learn/pull/26860
-@pytest.mark.skipif(
-    parse_version(sklearn.__version__) < parse_version("1.4"),
-    reason="Common tests in scikit-learn are not allowing for categorical string data.",
+@pytest.mark.skip(
+    "Common tests in scikit-learn are not allowing for categorical string data."
 )
 @parametrize_with_checks(list(_tested_estimators()))
 def test_estimators_compatibility_sklearn(estimator, check, request):
     check(estimator)
```

### Comparing `skrub-0.1.0/skrub/tests/test_string_distances.py` & `skrub-0.1.1/skrub/tests/test_string_distances.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/tests/test_table_vectorizer.py` & `skrub-0.1.1/skrub/tests/test_table_vectorizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 import joblib
 import numpy as np
 import pandas as pd
 import pytest
+import sklearn
 from numpy.testing import assert_array_almost_equal, assert_array_equal, assert_raises
 from pandas.testing import assert_frame_equal
 from scipy.sparse import csr_matrix
 from sklearn.preprocessing import FunctionTransformer, OneHotEncoder, StandardScaler
 from sklearn.utils._testing import skip_if_no_parallel
+from sklearn.utils.fixes import parse_version
 
 from skrub._datetime_encoder import DatetimeEncoder, _is_pandas_format_mixed_available
 from skrub._gap_encoder import GapEncoder
 from skrub._minhash_encoder import MinHashEncoder
 from skrub._table_vectorizer import LOW_CARDINALITY_TRANSFORMER, TableVectorizer
 from skrub.tests.utils import transformers_list_equal
 
 MSG_PANDAS_DEPRECATED_WARNING = "Skip deprecation warning"
 
+if parse_version(sklearn.__version__) < parse_version("1.4"):
+    PASSTHROUGH = "passthrough"
+else:
+    PASSTHROUGH = FunctionTransformer(
+        accept_sparse=True, check_inverse=False, feature_names_out="one-to-one"
+    )
+
 
 def type_equality(expected_type, actual_type):
     """
     Checks that the expected type is equal to the actual type,
     assuming object and str types are equivalent
     (considered as categorical by the TableVectorizer).
     """
@@ -159,16 +168,17 @@
     vectorizer = TableVectorizer()
     vectorizer.fit(X)
 
     low_cardinality_cols = ["str1", "str2", "cat1", "cat2"]
     low_cardinality_transformer = LOW_CARDINALITY_TRANSFORMER.fit(
         X[low_cardinality_cols]
     )
+
     expected_transformers = [
-        ("numeric", "passthrough", ["int", "float"]),
+        ("numeric", PASSTHROUGH, ["int", "float"]),
         ("low_cardinality", low_cardinality_transformer, low_cardinality_cols),
     ]
 
     assert transformers_list_equal(
         expected_transformers,
         vectorizer.transformers_,
         ignore_params=["categories_"],  # list of array of different lengths
@@ -391,15 +401,15 @@
         datetime_transformer="passthrough",
         numerical_transformer="passthrough",
         auto_cast=False,
     )
     vectorizer.set_output(transform="pandas")
     X_trans = vectorizer.fit_transform(X)
 
-    assert_frame_equal(X.astype("object"), X_trans)
+    assert_frame_equal(X, X_trans)
 
 
 def test_handle_unknown_category():
     X = _get_clean_dataframe()
     # Treat all columns as low cardinality
     table_vec = TableVectorizer(cardinality_threshold=6).fit(X)
     X_unknown = pd.DataFrame(
@@ -445,23 +455,43 @@
 
 @pytest.mark.parametrize(
     ["specific_transformers", "expected_transformers_"],
     [
         (
             (MinHashEncoder(), ["str1", "str2"]),
             [
-                ("numeric", "passthrough", ["int", "float"]),
+                (
+                    "numeric",
+                    (
+                        # Replace by "FunctionTransformer" when only supporting
+                        # sklearn >= 1.4
+                        PASSTHROUGH
+                        if isinstance(PASSTHROUGH, str)
+                        else PASSTHROUGH.__class__.__name__
+                    ),
+                    ["int", "float"],
+                ),
                 ("minhashencoder", "MinHashEncoder", ["str1", "str2"]),
                 ("low_cardinality", "OneHotEncoder", ["cat1", "cat2"]),
             ],
         ),
         (
             ("mh_cat1", MinHashEncoder(), ["cat1"]),
             [
-                ("numeric", "passthrough", ["int", "float"]),
+                (
+                    "numeric",
+                    (
+                        # Replace by "FunctionTransformer" when only supporting
+                        # sklearn >= 1.4
+                        PASSTHROUGH
+                        if isinstance(PASSTHROUGH, str)
+                        else PASSTHROUGH.__class__.__name__
+                    ),
+                    ["int", "float"],
+                ),
                 ("mh_cat1", "MinHashEncoder", ["cat1"]),
                 ("low_cardinality", "OneHotEncoder", ["str1", "str2", "cat2"]),
             ],
         ),
     ],
 )
 def test_specifying_specific_column_transformer(
@@ -611,16 +641,16 @@
 
 
 def test_changing_types_int_float() -> None:
     """
     The TableVectorizer shouldn't cast floats to ints
     even if only ints were seen during fit
     """
-    X_train = pd.DataFrame([[1], [2], [3]])
-    X_test = pd.DataFrame([[1], [2], [3.3]])
+    X_train = pd.DataFrame([[1], [2], [3]], columns=["a"])
+    X_test = pd.DataFrame([[1], [2], [3.3]], columns=["a"])
     vectorizer = TableVectorizer().fit(X_train)
     X_trans = vectorizer.transform(X_test)
     expected_X_trans = np.array([[1.0], [2.0], [3.3]])
     assert_array_almost_equal(X_trans, expected_X_trans)
 
 
 def test_column_by_column():
```

### Comparing `skrub-0.1.0/skrub/tests/test_utils.py` & `skrub-0.1.1/skrub/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub/tests/utils.py` & `skrub-0.1.1/skrub/tests/utils.py`

 * *Files identical despite different names*

### Comparing `skrub-0.1.0/skrub.egg-info/PKG-INFO` & `skrub-0.1.1/skrub.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skrub
-Version: 0.1.0
+Version: 0.1.1
 Summary: Prepping tables for machine learning
 Author: Patricio Cerda
 Author-email: patricio.cerda@inria.fr
 License: BSD
 Project-URL: Homepage, https://skrub-data.org/
 Project-URL: Source, https://github.com/skrub-data/skrub
 Classifier: Development Status :: 5 - Production/Stable
@@ -116,23 +116,33 @@
 
 `skrub` can still help with handling typos and variations in this kind of setting.
 
 For a detailed description of the problem of encoding dirty categorical data, see
 `Similarity encoding for learning with dirty categorical variables <https://hal.inria.fr/hal-01806175>`_ [1]_
 and `Encoding high-cardinality string categorical variables <https://hal.inria.fr/hal-02171256v4>`_ [2]_.
 
-Installation (WIP)
-------------------
+Installation
+------------
 
-There are currently no PiPy releases.
-You can still install the package from the GitHub repository with:
+The easiest way to install skrub is via `pip`:
 
 .. code-block:: shell
 
-    pip install git+https://github.com/skrub-data/skrub.git
+    pip install skrub -U
+
+
+or `conda`:
+
+.. code-block:: shell
+
+    conda install -c conda-forge skrub
+
+
+The documentation includes more detailed `installation instructions <https://skrub-data.github.io/install.html>`_.
+
 
 
 Dependencies
 ~~~~~~~~~~~~
 
 Dependencies and minimal versions are listed in the `setup <https://github.com/skrub-data/skrub/blob/main/setup.cfg#L27>`_ file.
```

### Comparing `skrub-0.1.0/skrub.egg-info/SOURCES.txt` & `skrub-0.1.1/skrub.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,12 @@
 LICENSE.txt
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
-benchmarks/__init__.py
-benchmarks/bench_fuzzy_join_count_vs_hash.py
-benchmarks/bench_fuzzy_join_sparse_vs_dense.py
-benchmarks/bench_fuzzy_join_vs_others.py
-benchmarks/bench_gap_divergence.py
-benchmarks/bench_gap_encoder_hp.py
-benchmarks/bench_gap_es_score.py
-benchmarks/bench_minhash_batch_number.py
-benchmarks/bench_tablevectorizer_tuning.py
-benchmarks/run_on_openml_datasets.py
-benchmarks/utils/__init__.py
-benchmarks/utils/_argparser.py
-benchmarks/utils/_various.py
-benchmarks/utils/join.py
-benchmarks/utils/monitor.py
 skrub/VERSION.txt
 skrub/__init__.py
 skrub/_agg_joiner.py
 skrub/_check_dependencies.py
 skrub/_datetime_encoder.py
 skrub/_deduplicate.py
 skrub/_fast_hash.py
@@ -33,14 +18,15 @@
 skrub/_matching.py
 skrub/_minhash_encoder.py
 skrub/_select_cols.py
 skrub/_similarity_encoder.py
 skrub/_string_distances.py
 skrub/_table_vectorizer.py
 skrub/_utils.py
+skrub/conftest.py
 skrub.egg-info/PKG-INFO
 skrub.egg-info/SOURCES.txt
 skrub.egg-info/dependency_links.txt
 skrub.egg-info/requires.txt
 skrub.egg-info/top_level.txt
 skrub/_dataframe/__init__.py
 skrub/_dataframe/_namespace.py
```

### Comparing `skrub-0.1.0/skrub.egg-info/requires.txt` & `skrub-0.1.1/skrub.egg-info/requires.txt`

 * *Files identical despite different names*

