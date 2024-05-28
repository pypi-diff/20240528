# Comparing `tmp/snapatac2-2.6.3.tar.gz` & `tmp/snapatac2-2.6.4.tar.gz`

## Comparing `snapatac2-2.6.3.tar` & `snapatac2-2.6.4.tar`

### file list

```diff
@@ -1,98 +1,98 @@
--rw-r--r--   0     1001      127      965 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-core/Cargo.toml
--rw-r--r--   0     1001      127     1080 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-core/LICENSE
--rw-r--r--   0     1001      127      724 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-core/src/embedding.rs
--rw-r--r--   0     1001      127    12674 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-core/src/export.rs
--rw-r--r--   0     1001      127     2687 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-core/src/knn.rs
--rw-r--r--   0     1001      127      117 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-core/src/lib.rs
--rw-r--r--   0     1001      127    10767 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-core/src/motif.rs
--rw-r--r--   0     1001      127     2765 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-core/src/network.rs
--rw-r--r--   0     1001      127    19281 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-core/src/preprocessing/bam/mark_duplicates.rs
--rw-r--r--   0     1001      127     5170 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-core/src/preprocessing/bam.rs
--rw-r--r--   0     1001      127    18667 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-core/src/preprocessing/count_data/coverage.rs
--rw-r--r--   0     1001      127    31384 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-core/src/preprocessing/count_data/genome.rs
--rw-r--r--   0     1001      127     9610 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-core/src/preprocessing/count_data/import.rs
--rw-r--r--   0     1001      127     7967 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-core/src/preprocessing/count_data/matrix.rs
--rw-r--r--   0     1001      127     6990 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-core/src/preprocessing/count_data.rs
--rw-r--r--   0     1001      127      427 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-core/src/preprocessing/mod.rs
--rw-r--r--   0     1001      127    12046 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-core/src/preprocessing/qc.rs
--rw-r--r--   0     1001      127    13427 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-core/src/utils/similarity.rs
--rw-r--r--   0     1001      127     5385 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-core/src/utils.rs
--rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 snapatac2-2.6.3/snapatac2-python/Cargo.toml
--rw-r--r--   0     1001      127     1080 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/LICENSE
--rw-r--r--   0     1001      127       85 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/README.md
--rw-r--r--   0     1001      127      655 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/__init__.py
--rw-r--r--   0     1001      127     2616 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/_io.py
--rw-r--r--   0     1001      127     3767 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/_utils.py
--rw-r--r--   0     1001      127    11895 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/datasets.py
--rw-r--r--   0     1001      127     7376 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/export/__init__.py
--rw-r--r--   0     1001      127     6145 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/genome.py
--rw-r--r--   0     1001      127     7358 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/metrics/__init__.py
--rw-r--r--   0     1001      127    11034 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/plotting/__init__.py
--rw-r--r--   0     1001      127    16396 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/plotting/_base.py
--rw-r--r--   0     1001      127     2911 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/plotting/_network.py
--rw-r--r--   0     1001      127      204 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/preprocessing/__init__.py
--rw-r--r--   0     1001      127    37676 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/preprocessing/_basic.py
--rw-r--r--   0     1001      127     3509 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/preprocessing/_harmony.py
--rw-r--r--   0     1001      127     3031 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/preprocessing/_knn.py
--rw-r--r--   0     1001      127     6030 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/preprocessing/_mnn_correct.py
--rw-r--r--   0     1001      127     5005 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/preprocessing/_scanorama.py
--rw-r--r--   0     1001      127    14260 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/preprocessing/_scrublet.py
--rw-r--r--   0     1001      127      324 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/tools/__init__.py
--rw-r--r--   0     1001      127     8737 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/tools/_call_peaks.py
--rw-r--r--   0     1001      127    11325 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/tools/_clustering.py
--rw-r--r--   0     1001      127     9283 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/tools/_diff.py
--rw-r--r--   0     1001      127    19537 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/tools/_embedding.py
--rw-r--r--   0     1001      127     1251 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/tools/_integration.py
--rw-r--r--   0     1001      127    11022 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/tools/_misc.py
--rw-r--r--   0     1001      127     4509 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/tools/_motif.py
--rw-r--r--   0     1001      127    19618 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/tools/_network.py
--rw-r--r--   0     1001      127     2078 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/python/snapatac2/tools/_smooth.py
--rw-r--r--   0     1001      127    13935 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/src/call_peaks.rs
--rw-r--r--   0     1001      127    15184 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/src/embedding.rs
--rw-r--r--   0     1001      127     3156 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/src/export.rs
--rw-r--r--   0     1001      127      748 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/src/knn.rs
--rw-r--r--   0     1001      127     3451 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/src/lib.rs
--rw-r--r--   0     1001      127     4759 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/src/motif.rs
--rw-r--r--   0     1001      127     1195 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/src/network.rs
--rw-r--r--   0     1001      127    12235 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/src/preprocessing.rs
--rw-r--r--   0     1001      127     8499 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/src/utils/anndata.rs
--rw-r--r--   0     1001      127    10859 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/src/utils.rs
--rw-r--r--   0     1001      127     2015 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/tests/test_func.py
--rw-r--r--   0     1001      127     2195 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/tests/test_pipeline.py
--rw-r--r--   0     1001      127     4262 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/tests/test_similarity.py
--rw-r--r--   0     1001      127      132 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/tests/test_tools/test.bam
--rw-r--r--   0     1001      127      130 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/tests/test_tools/test.bed.gz
--rw-r--r--   0     1001      127      131 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/tests/test_tools/test_clean.tsv.gz
--rw-r--r--   0     1001      127     4686 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/tests/test_tools.py
--rw-r--r--   0     1001      127    95098 2024-05-15 16:23:08.000000 snapatac2-2.6.3/snapatac2-python/Cargo.lock
--rw-r--r--   0        0        0     1882 1970-01-01 00:00:00.000000 snapatac2-2.6.3/pyproject.toml
--rw-r--r--   0     1001      127    11325 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/tools/_clustering.py
--rw-r--r--   0     1001      127     1251 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/tools/_integration.py
--rw-r--r--   0     1001      127     8737 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/tools/_call_peaks.py
--rw-r--r--   0     1001      127     4509 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/tools/_motif.py
--rw-r--r--   0     1001      127     9283 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/tools/_diff.py
--rw-r--r--   0     1001      127     2078 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/tools/_smooth.py
--rw-r--r--   0     1001      127    19537 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/tools/_embedding.py
--rw-r--r--   0     1001      127      324 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/tools/__init__.py
--rw-r--r--   0     1001      127    19618 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/tools/_network.py
--rw-r--r--   0     1001      127    11022 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/tools/_misc.py
--rw-r--r--   0     1001      127    16396 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/plotting/_base.py
--rw-r--r--   0     1001      127    11034 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/plotting/__init__.py
--rw-r--r--   0     1001      127     2911 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/plotting/_network.py
--rw-r--r--   0     1001      127    11895 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/datasets.py
--rw-r--r--   0     1001      127     7358 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/metrics/__init__.py
--rw-r--r--   0     1001      127     2616 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/_io.py
--rw-r--r--   0     1001      127      655 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/__init__.py
--rw-r--r--   0     1001      127    14260 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/preprocessing/_scrublet.py
--rw-r--r--   0     1001      127     6030 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/preprocessing/_mnn_correct.py
--rw-r--r--   0     1001      127      204 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/preprocessing/__init__.py
--rw-r--r--   0     1001      127     5005 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/preprocessing/_scanorama.py
--rw-r--r--   0     1001      127     3509 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/preprocessing/_harmony.py
--rw-r--r--   0     1001      127     3031 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/preprocessing/_knn.py
--rw-r--r--   0     1001      127    37676 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/preprocessing/_basic.py
--rw-r--r--   0     1001      127     3767 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/_utils.py
--rw-r--r--   0     1001      127     6145 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/genome.py
--rw-r--r--   0     1001      127     7376 2024-05-15 16:23:08.000000 snapatac2-2.6.3/python/snapatac2/export/__init__.py
--rw-r--r--   0     1001      127       85 2024-05-15 16:23:08.000000 snapatac2-2.6.3/README.md
--rw-r--r--   0     1001      127     1080 2024-05-15 16:23:08.000000 snapatac2-2.6.3/LICENSE
--rw-r--r--   0        0        0     2271 1970-01-01 00:00:00.000000 snapatac2-2.6.3/PKG-INFO
+-rw-r--r--   0     1001      127      965 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-core/Cargo.toml
+-rw-r--r--   0     1001      127     1080 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-core/LICENSE
+-rw-r--r--   0     1001      127      724 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-core/src/embedding.rs
+-rw-r--r--   0     1001      127    12674 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-core/src/export.rs
+-rw-r--r--   0     1001      127     2687 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-core/src/knn.rs
+-rw-r--r--   0     1001      127      117 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-core/src/lib.rs
+-rw-r--r--   0     1001      127    10767 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-core/src/motif.rs
+-rw-r--r--   0     1001      127     2765 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-core/src/network.rs
+-rw-r--r--   0     1001      127    19281 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-core/src/preprocessing/bam/mark_duplicates.rs
+-rw-r--r--   0     1001      127     5170 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-core/src/preprocessing/bam.rs
+-rw-r--r--   0     1001      127    18667 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-core/src/preprocessing/count_data/coverage.rs
+-rw-r--r--   0     1001      127    31384 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-core/src/preprocessing/count_data/genome.rs
+-rw-r--r--   0     1001      127     9610 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-core/src/preprocessing/count_data/import.rs
+-rw-r--r--   0     1001      127     7610 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-core/src/preprocessing/count_data/matrix.rs
+-rw-r--r--   0     1001      127     6990 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-core/src/preprocessing/count_data.rs
+-rw-r--r--   0     1001      127      427 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-core/src/preprocessing/mod.rs
+-rw-r--r--   0     1001      127    12046 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-core/src/preprocessing/qc.rs
+-rw-r--r--   0     1001      127    13427 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-core/src/utils/similarity.rs
+-rw-r--r--   0     1001      127     5385 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-core/src/utils.rs
+-rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 snapatac2-2.6.4/snapatac2-python/Cargo.toml
+-rw-r--r--   0     1001      127     1080 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/LICENSE
+-rw-r--r--   0     1001      127       85 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/README.md
+-rw-r--r--   0     1001      127      655 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/__init__.py
+-rw-r--r--   0     1001      127     2616 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/_io.py
+-rw-r--r--   0     1001      127     3767 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/_utils.py
+-rw-r--r--   0     1001      127    11895 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/datasets.py
+-rw-r--r--   0     1001      127     7376 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/export/__init__.py
+-rw-r--r--   0     1001      127     6145 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/genome.py
+-rw-r--r--   0     1001      127     7358 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/metrics/__init__.py
+-rw-r--r--   0     1001      127    11034 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/plotting/__init__.py
+-rw-r--r--   0     1001      127    16396 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/plotting/_base.py
+-rw-r--r--   0     1001      127     2911 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/plotting/_network.py
+-rw-r--r--   0     1001      127      204 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/preprocessing/__init__.py
+-rw-r--r--   0     1001      127    38485 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/preprocessing/_basic.py
+-rw-r--r--   0     1001      127     3509 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/preprocessing/_harmony.py
+-rw-r--r--   0     1001      127     3031 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/preprocessing/_knn.py
+-rw-r--r--   0     1001      127     6030 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/preprocessing/_mnn_correct.py
+-rw-r--r--   0     1001      127     5005 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/preprocessing/_scanorama.py
+-rw-r--r--   0     1001      127    14260 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/preprocessing/_scrublet.py
+-rw-r--r--   0     1001      127      324 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/tools/__init__.py
+-rw-r--r--   0     1001      127     8737 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/tools/_call_peaks.py
+-rw-r--r--   0     1001      127    11325 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/tools/_clustering.py
+-rw-r--r--   0     1001      127     9283 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/tools/_diff.py
+-rw-r--r--   0     1001      127    19537 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/tools/_embedding.py
+-rw-r--r--   0     1001      127     1251 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/tools/_integration.py
+-rw-r--r--   0     1001      127    11022 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/tools/_misc.py
+-rw-r--r--   0     1001      127     4509 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/tools/_motif.py
+-rw-r--r--   0     1001      127    19618 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/tools/_network.py
+-rw-r--r--   0     1001      127     2078 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/python/snapatac2/tools/_smooth.py
+-rw-r--r--   0     1001      127    13935 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/src/call_peaks.rs
+-rw-r--r--   0     1001      127    15184 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/src/embedding.rs
+-rw-r--r--   0     1001      127     3156 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/src/export.rs
+-rw-r--r--   0     1001      127      748 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/src/knn.rs
+-rw-r--r--   0     1001      127     3451 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/src/lib.rs
+-rw-r--r--   0     1001      127     4759 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/src/motif.rs
+-rw-r--r--   0     1001      127     1195 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/src/network.rs
+-rw-r--r--   0     1001      127    12434 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/src/preprocessing.rs
+-rw-r--r--   0     1001      127     8189 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/src/utils/anndata.rs
+-rw-r--r--   0     1001      127    10859 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/src/utils.rs
+-rw-r--r--   0     1001      127     2015 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/tests/test_func.py
+-rw-r--r--   0     1001      127     2195 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/tests/test_pipeline.py
+-rw-r--r--   0     1001      127     4262 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/tests/test_similarity.py
+-rw-r--r--   0     1001      127      132 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/tests/test_tools/test.bam
+-rw-r--r--   0     1001      127      130 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/tests/test_tools/test.bed.gz
+-rw-r--r--   0     1001      127      131 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/tests/test_tools/test_clean.tsv.gz
+-rw-r--r--   0     1001      127     4686 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/tests/test_tools.py
+-rw-r--r--   0     1001      127    96123 2024-05-28 01:56:44.000000 snapatac2-2.6.4/snapatac2-python/Cargo.lock
+-rw-r--r--   0        0        0     1892 1970-01-01 00:00:00.000000 snapatac2-2.6.4/pyproject.toml
+-rw-r--r--   0     1001      127     3767 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/_utils.py
+-rw-r--r--   0     1001      127    11022 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/tools/_misc.py
+-rw-r--r--   0     1001      127      324 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/tools/__init__.py
+-rw-r--r--   0     1001      127     8737 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/tools/_call_peaks.py
+-rw-r--r--   0     1001      127    19618 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/tools/_network.py
+-rw-r--r--   0     1001      127    19537 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/tools/_embedding.py
+-rw-r--r--   0     1001      127     9283 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/tools/_diff.py
+-rw-r--r--   0     1001      127     1251 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/tools/_integration.py
+-rw-r--r--   0     1001      127     2078 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/tools/_smooth.py
+-rw-r--r--   0     1001      127     4509 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/tools/_motif.py
+-rw-r--r--   0     1001      127    11325 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/tools/_clustering.py
+-rw-r--r--   0     1001      127      655 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/__init__.py
+-rw-r--r--   0     1001      127    11034 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/plotting/__init__.py
+-rw-r--r--   0     1001      127     2911 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/plotting/_network.py
+-rw-r--r--   0     1001      127    16396 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/plotting/_base.py
+-rw-r--r--   0     1001      127     7376 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/export/__init__.py
+-rw-r--r--   0     1001      127     5005 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/preprocessing/_scanorama.py
+-rw-r--r--   0     1001      127      204 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/preprocessing/__init__.py
+-rw-r--r--   0     1001      127    38485 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/preprocessing/_basic.py
+-rw-r--r--   0     1001      127     3031 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/preprocessing/_knn.py
+-rw-r--r--   0     1001      127    14260 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/preprocessing/_scrublet.py
+-rw-r--r--   0     1001      127     6030 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/preprocessing/_mnn_correct.py
+-rw-r--r--   0     1001      127     3509 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/preprocessing/_harmony.py
+-rw-r--r--   0     1001      127     2616 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/_io.py
+-rw-r--r--   0     1001      127     6145 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/genome.py
+-rw-r--r--   0     1001      127     7358 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/metrics/__init__.py
+-rw-r--r--   0     1001      127    11895 2024-05-28 01:56:44.000000 snapatac2-2.6.4/python/snapatac2/datasets.py
+-rw-r--r--   0     1001      127       85 2024-05-28 01:56:44.000000 snapatac2-2.6.4/README.md
+-rw-r--r--   0     1001      127     1080 2024-05-28 01:56:44.000000 snapatac2-2.6.4/LICENSE
+-rw-r--r--   0        0        0     2280 1970-01-01 00:00:00.000000 snapatac2-2.6.4/PKG-INFO
```

### Comparing `snapatac2-2.6.3/snapatac2-core/Cargo.toml` & `snapatac2-2.6.4/snapatac2-core/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [package]
 name = "snapatac2-core"
-version = "2.0.0"
+version = "2.0.1"
 edition = "2021"
 authors = ["Kai Zhang <zhangkai33@westlake.edu.cn>"]
 description = "Rust APIs"
 license = "MIT"
 repository = "https://github.com/"
 homepage = "https://github.com/"
 keywords = ["single-cell", "biology"]
 
 [dependencies]
-anndata = "0.3.3"
+anndata = "0.4.1"
 anyhow = "1.0"
 bigtools = { version = "0.4", features = ["read", "write"] }
 bed-utils = "0.4.1"
 flate2 = "1.0"
 tokio = "1.34"
 hora = "0.1"
 kdtree = "0.7"
 itertools = "0.12"
 indexmap = "2.2"
 indicatif = {version = "0.17", features = ["rayon"] }
 lexical = "6.1"
 log = "0.4"
 ndarray = { version = "0.15", features = ["rayon"] }
 num = "0.4"
-noodles = { version = "0.70", features = ["core", "bam", "sam", "gff", "gtf"] }
+noodles = { version = "0.74", features = ["core", "bam", "sam", "gff", "gtf"] }
 nalgebra-sparse = "0.9"
-polars = { version = "0.39", features = ["ndarray", "dtype-categorical"] }
+polars = { version = "0.40", features = ["ndarray", "dtype-categorical"] }
 rayon = "1.10"
 regex = "1.6"
 serde = "1.0"
 statrs = "0.16"
 smallvec = "1.13"
 tempfile = "3.3"
 zstd = { version = "0.13", features = ["zstdmt"] }
```

### Comparing `snapatac2-2.6.3/snapatac2-core/LICENSE` & `snapatac2-2.6.4/snapatac2-core/LICENSE`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-core/src/embedding.rs` & `snapatac2-2.6.4/snapatac2-core/src/embedding.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-core/src/export.rs` & `snapatac2-2.6.4/snapatac2-core/src/export.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-core/src/knn.rs` & `snapatac2-2.6.4/snapatac2-core/src/knn.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-core/src/motif.rs` & `snapatac2-2.6.4/snapatac2-core/src/motif.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-core/src/network.rs` & `snapatac2-2.6.4/snapatac2-core/src/network.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-core/src/preprocessing/bam/mark_duplicates.rs` & `snapatac2-2.6.4/snapatac2-core/src/preprocessing/bam/mark_duplicates.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-core/src/preprocessing/bam.rs` & `snapatac2-2.6.4/snapatac2-core/src/preprocessing/bam.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-core/src/preprocessing/count_data/coverage.rs` & `snapatac2-2.6.4/snapatac2-core/src/preprocessing/count_data/coverage.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-core/src/preprocessing/count_data/genome.rs` & `snapatac2-2.6.4/snapatac2-core/src/preprocessing/count_data/genome.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-core/src/preprocessing/count_data/import.rs` & `snapatac2-2.6.4/snapatac2-core/src/preprocessing/count_data/import.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-core/src/preprocessing/count_data/matrix.rs` & `snapatac2-2.6.4/snapatac2-core/src/preprocessing/count_data/matrix.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use crate::preprocessing::count_data::{
     SnapData,
     FeatureCounter, TranscriptCount, GeneCount,
     Promoters, Transcript,
 };
 use super::coverage::CountingStrategy;
 
-use anndata::{AnnDataOp, AxisArraysOp};
+use anndata::{data::DataFrameIndex, AnnDataOp};
 use indicatif::{ProgressIterator, ProgressStyle};
 use polars::prelude::{NamedFrom, DataFrame, Series};
 use anyhow::Result;
 use bed_utils::bed::{BEDLike, tree::{GenomeRegions, SparseCoverage}};
 
 /// Create cell by bin matrix.
 /// 
@@ -37,53 +37,41 @@
     A: SnapData,
     B: AnnDataOp,
 {
     let style = ProgressStyle::with_template(
         "[{elapsed}] {bar:40.cyan/blue} {pos:>7}/{len:7} (eta: {eta})"
     ).unwrap();
 
-    if adata.obsm().keys().contains(&"contact".into()) {
-        let data_iter = adata
-            .contact_count_iter(chunk_size)?
-            .with_resolution(bin_size)
-            .into_values::<u32>().map(|x| x.0).progress_with_style(style);
-        if let Some(adata_out) =  out {
-            adata_out.set_x_from_iter(data_iter)?;
-            adata_out.set_obs_names(adata.obs_names())?;
-            adata_out.set_var_names(adata_out.n_vars().into())?;
-        } else {
-            adata.set_x_from_iter(data_iter)?;
-            adata.set_var_names(adata.n_vars().into())?;
-        }
-    } else {
-        let mut counts = adata
-            .get_count_iter(chunk_size)?
-            .with_resolution(bin_size)
-            .set_counting_strategy(counting_strategy);
+    let mut counts = adata
+        .get_count_iter(chunk_size)?
+        .with_resolution(bin_size)
+        .set_counting_strategy(counting_strategy);
 
-        if let Some(exclude_chroms) = exclude_chroms {
-            counts = counts.exclude(exclude_chroms);
-        }
-        if let Some(min_fragment_size) = min_fragment_size {
-            counts = counts.min_fragment_size(min_fragment_size);
-        }
-        if let Some(max_fragment_size) = max_fragment_size {
-            counts = counts.max_fragment_size(max_fragment_size);
-        }
+    if let Some(exclude_chroms) = exclude_chroms {
+        counts = counts.exclude(exclude_chroms);
+    }
+    if let Some(min_fragment_size) = min_fragment_size {
+        counts = counts.min_fragment_size(min_fragment_size);
+    }
+    if let Some(max_fragment_size) = max_fragment_size {
+        counts = counts.max_fragment_size(max_fragment_size);
+    }
 
-        let feature_names = counts.get_gindex().to_index().into();
-        let data_iter = counts.into_counts::<u32>().map(|x| x.0).progress_with_style(style);
-        if let Some(adata_out) =  out {
-            adata_out.set_x_from_iter(data_iter)?;
-            adata_out.set_obs_names(adata.obs_names())?;
-            adata_out.set_var_names(feature_names)?;
-        } else {
-            adata.set_x_from_iter(data_iter)?;
-            adata.set_var_names(feature_names)?;
-        }
+    let feature_names: DataFrameIndex = counts.get_gindex().to_index().into();
+    let n_feat = feature_names.len();
+    let data_iter = counts.into_counts::<u32>().map(|x| x.0).progress_with_style(style);
+    if let Some(adata_out) =  out {
+        adata_out.set_n_vars(n_feat)?;
+        adata_out.set_x_from_iter(data_iter)?;
+        adata_out.set_obs_names(adata.obs_names())?;
+        adata_out.set_var_names(feature_names)?;
+    } else {
+        adata.set_n_vars(n_feat)?;
+        adata.set_x_from_iter(data_iter)?;
+        adata.set_var_names(feature_names)?;
     }
     Ok(())
 }
 
 pub fn create_peak_matrix<A, I, D, B>(
     adata: &A,
     peaks: I,
@@ -115,41 +103,47 @@
             counts = counts.min_fragment_size(min_fragment_size);
         }
         if let Some(max_fragment_size) = max_fragment_size {
             counts = counts.max_fragment_size(max_fragment_size);
         }
         Box::new(counts.aggregate_counts_by(counter).map(|x| x.0))
     };
+    let n_feat = feature_names.len();
     if let Some(adata_out) =  out {
+        adata_out.set_n_vars(n_feat)?;
         adata_out.set_x_from_iter(data.progress_with_style(style))?;
         adata_out.set_obs_names(adata.obs_names())?;
         adata_out.set_var_names(feature_names.into())?;
     } else {
+        adata.set_n_vars(n_feat)?;
         adata.set_x_from_iter(data.progress_with_style(style))?;
         adata.set_var_names(feature_names.into())?;
     }
     Ok(())
 }
 
 pub fn create_gene_matrix<A, B>(
     adata: &A,
     transcripts: Vec<Transcript>,
     id_type: &str, 
+    upstream: u64,
+    downstream: u64,
+    include_gene_body: bool,
     chunk_size: usize,
     counting_strategy: CountingStrategy,
     min_fragment_size: Option<u64>,
     max_fragment_size: Option<u64>,
     out: Option<&B>,
     use_x: bool,
     ) -> Result<()>
 where
     A: SnapData,
     B: AnnDataOp,
 {
-    let promoters = Promoters::new(transcripts, 2000, 0, true);
+    let promoters = Promoters::new(transcripts, upstream, downstream, include_gene_body);
     let transcript_counter: TranscriptCount<'_> = TranscriptCount::new(&promoters);
     match id_type {
         "transcript" => {
             let gene_names: Vec<String> = transcript_counter.gene_names().iter().map(|x| x.clone()).collect();
             let ids = transcript_counter.get_feature_ids();
             let data: Box<dyn ExactSizeIterator<Item = _>> = if use_x {
                 Box::new(adata.read_chrom_values(chunk_size)?
@@ -199,8 +193,8 @@
                 adata.set_x_from_iter(data)?;
                 adata.set_var_names(ids.into())?;
             }
         },
         _ => panic!("id_type must be 'transcript' or 'gene'"),
     }
     Ok(())
-}
+}
```

### Comparing `snapatac2-2.6.3/snapatac2-core/src/preprocessing/count_data.rs` & `snapatac2-2.6.4/snapatac2-core/src/preprocessing/count_data.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-core/src/preprocessing/qc.rs` & `snapatac2-2.6.4/snapatac2-core/src/preprocessing/qc.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-core/src/utils/similarity.rs` & `snapatac2-2.6.4/snapatac2-core/src/utils/similarity.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-core/src/utils.rs` & `snapatac2-2.6.4/snapatac2-core/src/utils.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/Cargo.toml` & `snapatac2-2.6.4/snapatac2-python/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 [package]
 name = "snapatac2"
-version = "2.6.3"
+version = "2.6.4"
 edition = "2021"
 authors = ["Kai Zhang <kai@kzhang.org>"]
 description = "Rust APIs"
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/"
 homepage = "https://github.com/"
 keywords = ["single-cell", "biology"]
 
 [dependencies]
 snapatac2-core = { path = "../snapatac2-core" }
-anndata = "0.3.3"
-anndata-hdf5 = "0.2"
-pyanndata = "0.3.3"
+anndata = "0.4.1"
+anndata-hdf5 = "0.3"
+pyanndata = "0.4.1"
 anyhow = "1.0"
 bed-utils = "0.4.1"
 flate2 = "1.0"
 itertools = "0.12"
 indicatif = "0.17"
 linreg = "0.2"
 log = "0.4"
 linfa = "0.6"
 linfa-clustering = "0.6"
-noodles = { version = "0.70", features = ["bam", "sam"] }
+noodles = { version = "0.74", features = ["bam", "sam"] }
 numpy = "0.21.0"
 nalgebra-sparse = "0.9"
 nalgebra = "0.32"
 ndarray = "0.15"
-polars = { version = "0.39", features = ["ndarray", "dtype-categorical"] }
+polars = { version = "0.40", features = ["ndarray", "dtype-categorical"] }
 pyo3-log = "0.10"
-pyo3-polars = "0.13"
+pyo3-polars = "0.14"
 rand_isaac = "0.3"
 rand_core = "0.6"
 rand = "0.8"
 rayon = "1.10"
 statrs = "0.16"
 tempfile = "3.3"
 zstd = { version = "0.13", features = ["zstdmt"] }
```

### Comparing `snapatac2-2.6.3/snapatac2-python/LICENSE` & `snapatac2-2.6.4/snapatac2-python/LICENSE`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/__init__.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/__init__.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/_io.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/_io.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/_utils.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/_utils.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/datasets.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/datasets.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/export/__init__.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/export/__init__.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/genome.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/genome.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/metrics/__init__.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/plotting/__init__.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/plotting/_base.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/plotting/_base.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/plotting/_network.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/plotting/_network.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/preprocessing/_basic.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/preprocessing/_basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -596,28 +596,34 @@
     *,
     inplace: bool = False,
     file: Path | None = None,
     backend: Literal['hdf5'] | None = 'hdf5',
     chunk_size: int = 500,
     use_x: bool = False,
     id_type: Literal['gene', 'transcript'] = "gene",
+    upstream: int = 2000,
+    downstream: int = 0,
+    include_gene_body: bool = True,
     transcript_name_key: str = "transcript_name",
     transcript_id_key: str = "transcript_id",
     gene_name_key: str = "gene_name",
     gene_id_key: str = "gene_id",
     min_frag_size: int | None = None,
     max_frag_size: int | None = None,
     counting_strategy: Literal['fragment', 'insertion', 'paired-insertion'] = 'insertion',
 ) -> internal.AnnData:
     """Generate cell by gene activity matrix.
 
-    Generate cell by gene activity matrix by counting the TN5 insertions in gene
-    body regions. The result will be stored in a new file and a new AnnData object
+    Generate cell by gene activity matrix by counting the TN5 insertions in each gene's
+    regulatory domain. The regulatory domain is initially defined as the TSS or the
+    whole gene body (if `include_gene_body=True`). We then extends this domain
+    by `upstream` and `downstream` base pairs on both sides.
+      
+    The result will be stored in a new file and a new AnnData object
     will be created.
-
     :func:`~snapatac2.pp.import_data` must be ran first in order to use this function.
 
     Parameters
     ----------
     adata
         The (annotated) data matrix of shape `n_obs` x `n_vars`.
         Rows correspond to cells and columns to regions.
@@ -632,14 +638,21 @@
     chunk_size
         Chunk size
     use_x
         If True, use the matrix stored in `.X` to compute the gene activity.
         Otherwise the `.obsm['insertion']` is used.
     id_type
         "gene" or "transcript".
+    upstream
+        The number of base pairs upstream of the regulatory domain.
+    downstream
+        The number of base pairs downstream of the regulatory domain.
+    include_gene_body
+        Whether to include the gene body in the regulatory domain. If False, the
+        TSS is used as the regulatory domain.
     transcript_name_key
         The key of the transcript name in the gene annotation file.
     transcript_id_key
         The key of the transcript id in the gene annotation file.
     gene_name_key
         The key of the gene name in the gene annotation file.
     gene_id_key
@@ -675,28 +688,30 @@
     --------
     >>> import snapatac2 as snap
     >>> data = snap.pp.import_data(snap.datasets.pbmc500(downsample=True), chrom_sizes=snap.genome.hg38, sorted_by_barcode=False)
     >>> gene_mat = snap.pp.make_gene_matrix(data, gene_anno=snap.genome.hg38)
     >>> print(gene_mat)
     AnnData object with n_obs × n_vars = 585 × 60606
         obs: 'n_fragment', 'frac_dup', 'frac_mito'
+    >>> gene_mat = snap.pp.make_gene_matrix(data, gene_anno=snap.genome.hg38, upstream=1000, downstream=1000, include_gene_body=False)
     """
     if isinstance(gene_anno, Genome):
         gene_anno = gene_anno.annotation
 
     if inplace:
         out = None
     elif file is None:
         if adata.isbacked:
             out = AnnData(obs=adata.obs[:].to_pandas())
         else:
             out = AnnData(obs=adata.obs[:])
     else:
         out = internal.AnnData(filename=file, backend=backend, obs=adata.obs[:])
     internal.mk_gene_matrix(adata, gene_anno, chunk_size, use_x, id_type,
+        upstream, downstream, include_gene_body,
         transcript_name_key, transcript_id_key, gene_name_key, gene_id_key,
         counting_strategy, min_frag_size, max_frag_size, out)
     return out
 
 def filter_cells(
     data: internal.AnnData | list[internal.AnnData],
     min_counts: int | None = 1000,
```

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/preprocessing/_harmony.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/preprocessing/_harmony.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/preprocessing/_knn.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/preprocessing/_knn.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/preprocessing/_mnn_correct.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/preprocessing/_mnn_correct.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/preprocessing/_scanorama.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/preprocessing/_scanorama.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/preprocessing/_scrublet.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/preprocessing/_scrublet.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/tools/_call_peaks.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/tools/_call_peaks.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/tools/_clustering.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/tools/_clustering.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/tools/_diff.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/tools/_diff.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/tools/_embedding.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/tools/_embedding.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/tools/_integration.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/tools/_integration.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/tools/_misc.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/tools/_misc.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/tools/_motif.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/tools/_motif.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/tools/_network.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/tools/_network.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/python/snapatac2/tools/_smooth.py` & `snapatac2-2.6.4/snapatac2-python/python/snapatac2/tools/_smooth.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/src/call_peaks.rs` & `snapatac2-2.6.4/snapatac2-python/src/call_peaks.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/src/embedding.rs` & `snapatac2-2.6.4/snapatac2-python/src/embedding.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/src/export.rs` & `snapatac2-2.6.4/snapatac2-python/src/export.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/src/knn.rs` & `snapatac2-2.6.4/snapatac2-python/src/knn.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/src/lib.rs` & `snapatac2-2.6.4/snapatac2-python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/src/motif.rs` & `snapatac2-2.6.4/snapatac2-python/src/motif.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/src/network.rs` & `snapatac2-2.6.4/snapatac2-python/src/network.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/src/preprocessing.rs` & `snapatac2-2.6.4/snapatac2-python/src/preprocessing.rs`

 * *Files 1% similar despite different names*

```diff
@@ -291,14 +291,17 @@
 #[pyfunction]
 pub(crate) fn mk_gene_matrix(
     anndata: AnnDataLike,
     gff_file: PathBuf,
     chunk_size: usize,
     use_x: bool,
     id_type: &str,
+    upstream: u64,
+    downstream: u64,
+    include_gene_body: bool,
     transcript_name_key: String,
     transcript_id_key: String,
     gene_name_key: String,
     gene_id_key: String,
     strategy: &str,
     min_fragment_size: Option<u64>,
     max_fragment_size: Option<u64>,
@@ -314,21 +317,23 @@
     let transcripts = read_transcripts(gff_file, &options);
     let strategy = parse_strategy(strategy);
     macro_rules! run {
         ($data:expr) => {
             if let Some(out) = out {
                 macro_rules! run2 {
                     ($out_data:expr) => {
-                        preprocessing::create_gene_matrix($data, transcripts, id_type, chunk_size, strategy,
+                        preprocessing::create_gene_matrix($data, transcripts, id_type,
+                            upstream, downstream, include_gene_body, chunk_size, strategy,
                             min_fragment_size, max_fragment_size, Some($out_data), use_x)?
                     };
                 }
                 crate::with_anndata!(&out, run2);
             } else {
-                preprocessing::create_gene_matrix($data, transcripts, id_type, chunk_size, strategy,
+                preprocessing::create_gene_matrix($data, transcripts, id_type,
+                    upstream, downstream, include_gene_body, chunk_size, strategy,
                     min_fragment_size, max_fragment_size, None::<&PyAnnData>, use_x)?;
             }
         }
     }
     crate::with_anndata!(&anndata, run);
     Ok(())
 }
```

### Comparing `snapatac2-2.6.3/snapatac2-python/src/utils/anndata.rs` & `snapatac2-2.6.4/snapatac2-python/src/utils/anndata.rs`

 * *Files 10% similar despite different names*

```diff
@@ -33,97 +33,78 @@
     }
 }
 
 impl<'py> AnnDataOp for PyAnnData<'py> {
     type X = memory::ArrayElem<'py>;
     type ElemCollectionRef<'a> = memory::ElemCollection<'a> where Self: 'a;
     type AxisArraysRef<'a> = memory::AxisArrays<'a> where Self: 'a;
-
     fn x(&self) -> Self::X {
         self.0.x()
     }
-
     fn set_x_from_iter<I, D>(&self, iter: I) -> Result<()>
     where
         I: Iterator<Item = D>,
         D: ArrayChunk + Into<ArrayData>,
     {
         self.0.set_x_from_iter(iter)
     }
-
     fn set_x<D: WriteArrayData + Into<ArrayData> + HasShape>(&self, data: D) -> Result<()> {
         self.0.set_x(data)
     }
-
-    /// Delete the 'X' element.
     fn del_x(&self) -> Result<()> {
         self.0.del_x()
     }
-
-    /// Return the number of observations (rows).
     fn n_obs(&self) -> usize {
         self.0.n_obs()
     }
-    /// Return the number of variables (columns).
     fn n_vars(&self) -> usize {
         self.0.n_vars()
     }
-
-    /// Return the names of observations.
+    fn set_n_obs(&self, n: usize) -> Result<()> {
+        self.0.set_n_obs(n)
+    }
+    fn set_n_vars(&self, n: usize) -> Result<()> {
+        self.0.set_n_vars(n)
+    }
     fn obs_names(&self) -> DataFrameIndex {
         self.0.obs_names()
     }
-    /// Return the names of variables.
     fn var_names(&self) -> DataFrameIndex {
         self.0.var_names()
     }
-
-    /// Chagne the names of observations.
     fn set_obs_names(&self, index: DataFrameIndex) -> Result<()> {
         self.0.set_obs_names(index)
     }
-    /// Chagne the names of variables.
     fn set_var_names(&self, index: DataFrameIndex) -> Result<()> {
         self.0.set_var_names(index)
     }
-
     fn obs_ix<'a, I: IntoIterator<Item = &'a str>>(&self, names: I) -> Result<Vec<usize>> {
         self.0.obs_ix(names)
     }
     fn var_ix<'a, I: IntoIterator<Item = &'a str>>(&self, names: I) -> Result<Vec<usize>> {
         self.0.var_ix(names)
     }
-
     fn read_obs(&self) -> Result<DataFrame> {
         self.0.read_obs()
     }
     fn read_var(&self) -> Result<DataFrame> {
         self.0.read_var()
     }
-
-    /// Change the observation annotations.
     fn set_obs(&self, obs: DataFrame) -> Result<()> {
         self.0.set_obs(obs)
     }
-
-    /// Change the variable annotations.
     fn set_var(&self, var: DataFrame) -> Result<()> {
         self.0.set_var(var)
     }
-
-    /// Delete the observation annotations.
     fn del_obs(&self) -> Result<()> {
         self.0.del_obs()
     }
-
-    /// Delete the variable annotations.
     fn del_var(&self) -> Result<()> {
         self.0.del_var()
     }
-
     fn uns(&self) -> Self::ElemCollectionRef<'_> {
         self.0.uns()
     }
     fn obsm(&self) -> Self::AxisArraysRef<'_> {
         self.0.obsm()
     }
     fn obsp(&self) -> Self::AxisArraysRef<'_> {
@@ -131,15 +112,14 @@
     }
     fn varm(&self) -> Self::AxisArraysRef<'_> {
         self.0.varm()
     }
     fn varp(&self) -> Self::AxisArraysRef<'_> {
         self.0.varp()
     }
-
     fn del_uns(&self) -> Result<()> {
         self.0.del_uns()
     }
     fn del_obsm(&self) -> Result<()> {
         self.0.del_obsm()
     }
     fn del_obsp(&self) -> Result<()> {
@@ -147,15 +127,14 @@
     }
     fn del_varm(&self) -> Result<()> {
         self.0.del_varm()
     }
     fn del_varp(&self) -> Result<()> {
         self.0.del_varp()
     }
-
     fn layers(&self) -> Self::AxisArraysRef<'_> {
         self.0.layers()
     }
     fn del_layers(&self) -> Result<()> {
         self.0.del_layers()
     }
 }
```

### Comparing `snapatac2-2.6.3/snapatac2-python/src/utils.rs` & `snapatac2-2.6.4/snapatac2-python/src/utils.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/tests/test_func.py` & `snapatac2-2.6.4/snapatac2-python/tests/test_func.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/tests/test_pipeline.py` & `snapatac2-2.6.4/snapatac2-python/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/tests/test_similarity.py` & `snapatac2-2.6.4/snapatac2-python/tests/test_similarity.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/tests/test_tools.py` & `snapatac2-2.6.4/snapatac2-python/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/snapatac2-python/Cargo.lock` & `snapatac2-2.6.4/snapatac2-python/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -58,17 +58,17 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anndata"
-version = "0.3.3"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb25ab5522d849dda564d6807e7cd17dac43a0fd10d14770c8f8d9b39d4a12be"
+checksum = "7908551ce9d7d10e1ec90eaa697951eae25421c215c8dcb8cd8cd75270b0111f"
 dependencies = [
  "anyhow",
  "flate2",
  "indexmap 2.2.3",
  "itertools 0.12.1",
  "log",
  "nalgebra-sparse",
@@ -80,17 +80,17 @@
  "rayon",
  "replace_with",
  "smallvec",
 ]
 
 [[package]]
 name = "anndata-hdf5"
-version = "0.2.0"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7de80bddc00b2de20cafd47a662a9b0abad897742eb08cc5465348be96677f35"
+checksum = "48c189e0569819cd805ab11330bb76b83b5d35b79c9cb39b3edf35eef232400d"
 dependencies = [
  "anndata",
  "anyhow",
  "hdf5",
  "hdf5-sys",
  "libz-sys",
  "ndarray",
@@ -248,14 +248,20 @@
 [[package]]
 name = "base64"
 version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
 [[package]]
+name = "base64"
+version = "0.22.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "72b3254f16251a8381aa12e40e3c4d2f0199f8c6508fbecb9d91f575e0fbb8c6"
+
+[[package]]
 name = "bed-utils"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f67cc56ed28dac516c91085742567f9182124588b505511abf3962ec62291ae6"
 dependencies = [
  "bincode",
  "bio",
@@ -335,30 +341,30 @@
  "petgraph",
  "rand",
  "regex",
  "serde",
  "serde_derive",
  "statrs",
  "strum",
- "strum_macros",
+ "strum_macros 0.25.3",
  "thiserror",
  "triple_accel",
  "vec_map",
 ]
 
 [[package]]
 name = "bio-types"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d45749b87f21808051025e9bf714d14ff4627f9d8ca967eade6946ea769aa4a"
 dependencies = [
  "derive-new",
  "lazy_static",
  "regex",
- "strum_macros",
+ "strum_macros 0.25.3",
  "thiserror",
 ]
 
 [[package]]
 name = "bit-set"
 version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -572,15 +578,15 @@
 name = "comfy-table"
 version = "7.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c64043d6c7b7a4c58e39e7efccfdea7b93d885a795d0c054a69dbbf4dd52686"
 dependencies = [
  "crossterm",
  "strum",
- "strum_macros",
+ "strum_macros 0.25.3",
  "unicode-width",
 ]
 
 [[package]]
 name = "console"
 version = "0.15.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -748,17 +754,17 @@
 name = "editdistancek"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3e02df23d5b1c6f9e69fa603b890378123b93073df998a21e6e33b9db0a32613"
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "3dca9240753cf90908d7e4aac30f630662b02aebaa1b58a3cadabdb23385b58b"
 
 [[package]]
 name = "encode_unicode"
 version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a357d28ed41a50f9c765dbfe56cbc04a64e53e5fc58ba79fbc34c10ef3df831f"
 
@@ -1013,14 +1019,15 @@
 version = "0.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
 dependencies = [
  "ahash",
  "allocator-api2",
  "rayon",
+ "serde",
 ]
 
 [[package]]
 name = "hdf5"
 version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bdcd9b131fd67bb827b386d0dc63d3e74196a14616ef800acf87ca5fef741a10"
@@ -1755,102 +1762,105 @@
 checksum = "978fe6e6ebc0bf53de533cd456ca2d9de13de13856eda1518a285d7705a213af"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "noodles"
-version = "0.70.0"
+version = "0.74.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5c7777c4301ec50202f778c15d73b88c30f9240a074f9b9a98fe7babfa5bfc8"
+checksum = "8903a0299daf4f072f2e601c74c29c861abdfd2427366e727b8d8afbbde8cbcc"
 dependencies = [
  "noodles-bam",
  "noodles-core",
  "noodles-gff",
  "noodles-gtf",
  "noodles-sam",
 ]
 
 [[package]]
 name = "noodles-bam"
-version = "0.60.0"
+version = "0.63.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "880f71c52dab49e073361e0427610e07eccea07ff48a2ecd8f133c648cb115d8"
+checksum = "3ede0b1e0b8e0e03f21c692ad38473dfe95c3650317650205c29c9a682c4a5a6"
 dependencies = [
  "bit-vec 0.6.3",
  "bstr",
  "byteorder",
  "bytes",
  "indexmap 2.2.3",
  "noodles-bgzf",
  "noodles-core",
  "noodles-csi",
  "noodles-sam",
 ]
 
 [[package]]
 name = "noodles-bgzf"
-version = "0.28.0"
+version = "0.30.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eff82b0fb78c11947b29ef50e8ddf0093813fa9e613af0e13dc53fc12b2dc3ea"
+checksum = "13f54d4840fd26ed94103ded9524aa5fdd757255a556f24653d162c0a45c47e8"
 dependencies = [
  "byteorder",
  "bytes",
  "crossbeam-channel",
  "flate2",
 ]
 
 [[package]]
 name = "noodles-core"
-version = "0.14.0"
+version = "0.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7336c3be652de4e05444c9b12a32331beb5ba3316e8872d92bfdd8ef3b06c282"
+checksum = "c5a8c6b020d1205abef2b0fab4463a6c5ecc3c8f4d561ca8b0d1a42323376200"
+dependencies = [
+ "bstr",
+]
 
 [[package]]
 name = "noodles-csi"
-version = "0.32.0"
+version = "0.35.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "938d7d865a3fbb079c7855e76eb1ef0be5d285dc039fa7776622225c7f708411"
+checksum = "beb1618ca2aa88662d387197a188686105d6b5e25f6959c52b766276cbfc4620"
 dependencies = [
  "bit-vec 0.6.3",
  "byteorder",
  "indexmap 2.2.3",
  "noodles-bgzf",
  "noodles-core",
 ]
 
 [[package]]
 name = "noodles-gff"
-version = "0.29.0"
+version = "0.33.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9216634517bf888abb425b10f3df7857ee3f584d4e46c8d6a2bb2c84acc4e10e"
+checksum = "578b6efaf5c3f029720af4c8590e34fd38e214666971d665a52e3566830170d0"
 dependencies = [
  "indexmap 2.2.3",
  "noodles-bgzf",
  "noodles-core",
  "noodles-csi",
  "percent-encoding",
 ]
 
 [[package]]
 name = "noodles-gtf"
-version = "0.25.0"
+version = "0.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99d4fabc2e574e80c00341685e8f4df37ae0b5a00a6fecccfd7c99eb45d5a4cf"
+checksum = "126a4e1149e741808168e36fa38af871139428829d885e1ade46026ac31871c9"
 dependencies = [
  "noodles-bgzf",
  "noodles-core",
  "noodles-csi",
 ]
 
 [[package]]
 name = "noodles-sam"
-version = "0.57.0"
+version = "0.60.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6b0598e959a0e56fc60f11b3bc63bf11c332a530cb54883196c0eab1bd0d4b8a"
+checksum = "0ec6452e8ed9f20ef043dce35e09ed58f1c34834cd941e987458a66e8fa66fa0"
 dependencies = [
  "bitflags 2.4.2",
  "bstr",
  "indexmap 2.2.3",
  "lexical-core",
  "memchr",
  "noodles-bgzf",
@@ -2183,17 +2193,17 @@
 checksum = "fc1691dd09e82f428ce8d6310bd6d5da2557c82ff17694d2a32cad7242aea89f"
 dependencies = [
  "array-init-cursor",
 ]
 
 [[package]]
 name = "polars"
-version = "0.39.2"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0ea21b858b16b9c0e17a12db2800d11aa5b4bd182be6b3022eb537bbfc1f2db5"
+checksum = "e148396dca5496566880fa19374f3f789a29db94e3eb458afac1497b4bac5442"
 dependencies = [
  "getrandom",
  "polars-arrow",
  "polars-core",
  "polars-error",
  "polars-io",
  "polars-lazy",
@@ -2203,17 +2213,17 @@
  "polars-time",
  "polars-utils",
  "version_check",
 ]
 
 [[package]]
 name = "polars-arrow"
-version = "0.39.2"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "725b09f2b5ef31279b66e27bbab63c58d49d8f6696b66b1f46c7eaab95e80f75"
+checksum = "1cb5e11cd0752ae022fa6ca3afa50a14b0301b7ce53c0135828fbb0f4fa8303e"
 dependencies = [
  "ahash",
  "atoi",
  "atoi_simd",
  "bytemuck",
  "chrono",
  "chrono-tz",
@@ -2248,33 +2258,33 @@
 dependencies = [
  "planus",
  "serde",
 ]
 
 [[package]]
 name = "polars-compute"
-version = "0.39.2"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a796945b14b14fbb79b91ef0406e6fddca2be636e889f81ea5d6ee7d36efb4fe"
+checksum = "89fc4578f826234cdecb782952aa9c479dc49373f81694a7b439c70b6f609ba0"
 dependencies = [
  "bytemuck",
  "either",
  "num-traits",
  "polars-arrow",
  "polars-error",
  "polars-utils",
  "strength_reduce",
  "version_check",
 ]
 
 [[package]]
 name = "polars-core"
-version = "0.39.2"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "465f70d3e96b6d0b1a43c358ba451286b8c8bd56696feff020d65702aa33e35c"
+checksum = "e490c6bace1366a558feea33d1846f749a8ca90bd72a6748752bc65bb4710b2a"
 dependencies = [
  "ahash",
  "bitflags 2.4.2",
  "bytemuck",
  "chrono",
  "chrono-tz",
  "comfy-table",
@@ -2297,29 +2307,49 @@
  "thiserror",
  "version_check",
  "xxhash-rust",
 ]
 
 [[package]]
 name = "polars-error"
-version = "0.39.2"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5224d5d05e6b8a6f78b75951ae1b5f82c8ab1979e11ffaf5fd41941e3d5b0757"
+checksum = "08888f58e61599b00f5ea0c2ccdc796b54b9859559cc0d4582733509451fa01a"
 dependencies = [
  "polars-arrow-format",
  "regex",
  "simdutf8",
  "thiserror",
 ]
 
 [[package]]
+name = "polars-expr"
+version = "0.40.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4173591920fe56ad55af025f92eb0d08421ca85705c326a640c43856094e3484"
+dependencies = [
+ "ahash",
+ "bitflags 2.4.2",
+ "once_cell",
+ "polars-arrow",
+ "polars-core",
+ "polars-io",
+ "polars-ops",
+ "polars-plan",
+ "polars-time",
+ "polars-utils",
+ "rayon",
+ "smartstring",
+]
+
+[[package]]
 name = "polars-io"
-version = "0.39.2"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2c8589e418cbe4a48228d64b2a8a40284a82ec3c98817c0c2bcc0267701338b"
+checksum = "5842896aea46d975b425d63f156f412aed3cfde4c257b64fb1f43ceea288074e"
 dependencies = [
  "ahash",
  "atoi_simd",
  "bytes",
  "chrono",
  "fast-float",
  "flate2",
@@ -2341,44 +2371,45 @@
  "simdutf8",
  "smartstring",
  "zstd",
 ]
 
 [[package]]
 name = "polars-lazy"
-version = "0.39.2"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89b2632b1af668e2058d5f8f916d8fbde3cac63d03ae29a705f598e41dcfeb7f"
+checksum = "e805ea2ebbc6b7749b0afb31b7fc5d32b42b57ba29b984549d43d3a16114c4a5"
 dependencies = [
  "ahash",
  "bitflags 2.4.2",
  "glob",
  "once_cell",
  "polars-arrow",
  "polars-core",
+ "polars-expr",
  "polars-io",
  "polars-ops",
  "polars-pipe",
  "polars-plan",
  "polars-time",
  "polars-utils",
  "rayon",
  "smartstring",
  "version_check",
 ]
 
 [[package]]
 name = "polars-ops"
-version = "0.39.2"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "efdbdb4d9a92109bc2e0ce8e17af5ae8ab643bb5b7ee9d1d74f0aeffd1fbc95f"
+checksum = "7b0aed7e169c81b98457641cf82b251f52239a668916c2e683abd1f38df00d58"
 dependencies = [
  "ahash",
  "argminmax",
- "base64",
+ "base64 0.22.1",
  "bytemuck",
  "chrono",
  "chrono-tz",
  "either",
  "hashbrown 0.14.3",
  "hex",
  "indexmap 2.2.3",
@@ -2394,119 +2425,123 @@
  "smartstring",
  "unicode-reverse",
  "version_check",
 ]
 
 [[package]]
 name = "polars-parquet"
-version = "0.39.2"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b421d2196f786fdfe162db614c8485f8308fe41575d4de634a39bbe460d1eb6a"
+checksum = "c70670a9e51cac66d0e77fd20b5cc957dbcf9f2660d410633862bb72f846d5b8"
 dependencies = [
  "ahash",
- "base64",
+ "base64 0.22.1",
  "ethnum",
  "num-traits",
  "parquet-format-safe",
  "polars-arrow",
  "polars-error",
  "polars-utils",
  "seq-macro",
  "simdutf8",
  "streaming-decompression",
 ]
 
 [[package]]
 name = "polars-pipe"
-version = "0.39.2"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "48700f1d5bd56a15451e581f465c09541492750360f18637b196f995470a015c"
+checksum = "0a40ae1b3c74ee07e2d1f7cbf56c5d6e15969e45d9b6f0903bd2acaf783ba436"
 dependencies = [
  "crossbeam-channel",
  "crossbeam-queue",
  "enum_dispatch",
  "hashbrown 0.14.3",
  "num-traits",
  "polars-arrow",
  "polars-compute",
  "polars-core",
+ "polars-expr",
  "polars-io",
  "polars-ops",
  "polars-plan",
  "polars-row",
  "polars-utils",
  "rayon",
  "smartstring",
  "uuid",
  "version_check",
 ]
 
 [[package]]
 name = "polars-plan"
-version = "0.39.2"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2fb8e2302e20c44defd5be8cad9c96e75face63c3a5f609aced8c4ec3b3ac97d"
+checksum = "8daa3541ae7e9af311a4389bc2b21f83349c34c723cc67fa524cdefdaa172d90"
 dependencies = [
  "ahash",
  "bytemuck",
  "chrono-tz",
+ "either",
  "hashbrown 0.14.3",
  "once_cell",
  "percent-encoding",
  "polars-arrow",
  "polars-core",
  "polars-io",
  "polars-ops",
  "polars-time",
  "polars-utils",
  "rayon",
  "recursive",
  "regex",
  "smartstring",
- "strum_macros",
+ "strum_macros 0.26.2",
  "version_check",
 ]
 
 [[package]]
 name = "polars-row"
-version = "0.39.2"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a515bdc68c2ae3702e3de70d89601f3b71ca8137e282a226dddb53ee4bacfa2e"
+checksum = "deb285f2f3a65b00dd06bef16bb9f712dbb5478f941dab5cf74f9f016d382e40"
 dependencies = [
  "bytemuck",
  "polars-arrow",
  "polars-error",
  "polars-utils",
 ]
 
 [[package]]
 name = "polars-sql"
-version = "0.39.2"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b4bb7cc1c04c3023d1953b2f1dec50515e8fd8169a5a2bf4967b3b082232db7"
+checksum = "a724f699d194cb02c25124d3832f7d4d77f387f1a89ee42f6b9e88ec561d4ad9"
 dependencies = [
  "hex",
+ "once_cell",
  "polars-arrow",
  "polars-core",
  "polars-error",
  "polars-lazy",
  "polars-plan",
  "rand",
  "serde",
  "serde_json",
  "sqlparser",
 ]
 
 [[package]]
 name = "polars-time"
-version = "0.39.2"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "efc18e3ad92eec55db89d88f16c22d436559ba7030cf76f86f6ed7a754b673f1"
+checksum = "87ebec238d8b6200d9f0c3ce411c8441e950bd5a7df7806b8172d06c1d5a4b97"
 dependencies = [
  "atoi",
+ "bytemuck",
  "chrono",
  "chrono-tz",
  "now",
  "once_cell",
  "polars-arrow",
  "polars-core",
  "polars-error",
@@ -2514,17 +2549,17 @@
  "polars-utils",
  "regex",
  "smartstring",
 ]
 
 [[package]]
 name = "polars-utils"
-version = "0.39.2"
+version = "0.40.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c760b6c698cfe2fbbbd93d6cfb408db14ececfe1d92445dae2229ce1b5b21ae8"
+checksum = "34e1a907c63abf71e5f21467e2e4ff748896c28196746f631c6c25512ec6102c"
 dependencies = [
  "ahash",
  "bytemuck",
  "hashbrown 0.14.3",
  "indexmap 2.2.3",
  "num-traits",
  "once_cell",
@@ -2565,17 +2600,17 @@
 checksum = "5787f7cda34e3033a72192c018bc5883100330f362ef279a8cbccfce8bb4e874"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "pyanndata"
-version = "0.3.3"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c30551f41c9b8c2d04ad34ee5029c3db6c321a5a0297901c7bb700d3100e91f"
+checksum = "157c4c82beef68e427308fc360bdcf4bfa9dd020b3f7e0c7010d2a7d3ae72d79"
 dependencies = [
  "anndata",
  "anndata-hdf5",
  "anyhow",
  "downcast-rs",
  "flate2",
  "hdf5",
@@ -2668,17 +2703,17 @@
  "pyo3-build-config",
  "quote",
  "syn 2.0.50",
 ]
 
 [[package]]
 name = "pyo3-polars"
-version = "0.13.0"
+version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "469bd1d378fb3a34c1b182383e84741d9e7c5451a5d29a3f9c557aac161876cd"
+checksum = "8e726fef8618531b0ec1777f430a9225a909f9ffeacaad7bca7b43877fc3cd42"
 dependencies = [
  "polars",
  "polars-core",
  "pyo3",
  "thiserror",
 ]
 
@@ -2932,15 +2967,15 @@
 
 [[package]]
 name = "rustls-pemfile"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1c74cae0a4cf6ccbbf5f359f08efdf8ee7e1dc532573bf0db71968cb56b1448c"
 dependencies = [
- "base64",
+ "base64 0.21.7",
 ]
 
 [[package]]
 name = "rustls-webpki"
 version = "0.101.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b6275d1ee7a1cd780b64aca7726599a1dbc893b1e64144529e55c3c2f745765"
@@ -3123,15 +3158,15 @@
  "autocfg",
  "static_assertions",
  "version_check",
 ]
 
 [[package]]
 name = "snapatac2"
-version = "2.6.3"
+version = "2.6.4"
 dependencies = [
  "anndata",
  "anndata-hdf5",
  "anyhow",
  "bed-utils",
  "flate2",
  "indicatif",
@@ -3159,15 +3194,15 @@
  "tempfile",
  "tikv-jemallocator",
  "zstd",
 ]
 
 [[package]]
 name = "snapatac2-core"
-version = "2.0.0"
+version = "2.0.1"
 dependencies = [
  "anndata",
  "anyhow",
  "bed-utils",
  "bigtools",
  "flate2",
  "hora",
@@ -3286,14 +3321,27 @@
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "rustversion",
  "syn 2.0.50",
 ]
+
+[[package]]
+name = "strum_macros"
+version = "0.26.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c6cf59daf282c0a494ba14fd21610a0325f9f90ec9d1231dea26bcb1d696c946"
+dependencies = [
+ "heck",
+ "proc-macro2",
+ "quote",
+ "rustversion",
+ "syn 2.0.50",
+]
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
```

### Comparing `snapatac2-2.6.3/pyproject.toml` & `snapatac2-2.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     'anndata >= 0.8.0, < 0.11.0',
     'kaleido',
     'multiprocess',
     'MACS3 >= 3.0, < 3.1',
     'natsort', 
     'numpy >= 1.16.0, < 2.0.0',
     'pandas >= 1.0, < 2.1.2',
-    'plotly >= 5.6.0',
+    'plotly >= 5.19.0, < 6.0.0',
     'polars >= 0.20.0, < 0.21.0',
     'pooch >= 1.6.0, < 2.0.0',
     'igraph >= 0.10.3',
     'pyarrow',
     'pyfaidx >= 0.7.0, < 0.8.0',
     'rustworkx',
     'scipy >= 1.4, < 2.0.0',
```

### Comparing `snapatac2-2.6.3/python/snapatac2/tools/_clustering.py` & `snapatac2-2.6.4/python/snapatac2/tools/_clustering.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/python/snapatac2/tools/_integration.py` & `snapatac2-2.6.4/python/snapatac2/tools/_integration.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/python/snapatac2/tools/_call_peaks.py` & `snapatac2-2.6.4/python/snapatac2/tools/_call_peaks.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/python/snapatac2/tools/_motif.py` & `snapatac2-2.6.4/python/snapatac2/tools/_motif.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/python/snapatac2/tools/_diff.py` & `snapatac2-2.6.4/python/snapatac2/tools/_diff.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/python/snapatac2/tools/_smooth.py` & `snapatac2-2.6.4/python/snapatac2/tools/_smooth.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/python/snapatac2/tools/_embedding.py` & `snapatac2-2.6.4/python/snapatac2/tools/_embedding.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/python/snapatac2/tools/_network.py` & `snapatac2-2.6.4/python/snapatac2/tools/_network.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/python/snapatac2/tools/_misc.py` & `snapatac2-2.6.4/python/snapatac2/tools/_misc.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/python/snapatac2/plotting/_base.py` & `snapatac2-2.6.4/python/snapatac2/plotting/_base.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/python/snapatac2/plotting/__init__.py` & `snapatac2-2.6.4/python/snapatac2/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/python/snapatac2/plotting/_network.py` & `snapatac2-2.6.4/python/snapatac2/plotting/_network.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/python/snapatac2/datasets.py` & `snapatac2-2.6.4/python/snapatac2/datasets.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/python/snapatac2/metrics/__init__.py` & `snapatac2-2.6.4/python/snapatac2/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/python/snapatac2/_io.py` & `snapatac2-2.6.4/python/snapatac2/_io.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/python/snapatac2/__init__.py` & `snapatac2-2.6.4/python/snapatac2/__init__.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/python/snapatac2/preprocessing/_scrublet.py` & `snapatac2-2.6.4/python/snapatac2/preprocessing/_scrublet.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/python/snapatac2/preprocessing/_mnn_correct.py` & `snapatac2-2.6.4/python/snapatac2/preprocessing/_mnn_correct.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/python/snapatac2/preprocessing/_scanorama.py` & `snapatac2-2.6.4/python/snapatac2/preprocessing/_scanorama.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/python/snapatac2/preprocessing/_harmony.py` & `snapatac2-2.6.4/python/snapatac2/preprocessing/_harmony.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/python/snapatac2/preprocessing/_knn.py` & `snapatac2-2.6.4/python/snapatac2/preprocessing/_knn.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/python/snapatac2/preprocessing/_basic.py` & `snapatac2-2.6.4/python/snapatac2/preprocessing/_basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -596,28 +596,34 @@
     *,
     inplace: bool = False,
     file: Path | None = None,
     backend: Literal['hdf5'] | None = 'hdf5',
     chunk_size: int = 500,
     use_x: bool = False,
     id_type: Literal['gene', 'transcript'] = "gene",
+    upstream: int = 2000,
+    downstream: int = 0,
+    include_gene_body: bool = True,
     transcript_name_key: str = "transcript_name",
     transcript_id_key: str = "transcript_id",
     gene_name_key: str = "gene_name",
     gene_id_key: str = "gene_id",
     min_frag_size: int | None = None,
     max_frag_size: int | None = None,
     counting_strategy: Literal['fragment', 'insertion', 'paired-insertion'] = 'insertion',
 ) -> internal.AnnData:
     """Generate cell by gene activity matrix.
 
-    Generate cell by gene activity matrix by counting the TN5 insertions in gene
-    body regions. The result will be stored in a new file and a new AnnData object
+    Generate cell by gene activity matrix by counting the TN5 insertions in each gene's
+    regulatory domain. The regulatory domain is initially defined as the TSS or the
+    whole gene body (if `include_gene_body=True`). We then extends this domain
+    by `upstream` and `downstream` base pairs on both sides.
+      
+    The result will be stored in a new file and a new AnnData object
     will be created.
-
     :func:`~snapatac2.pp.import_data` must be ran first in order to use this function.
 
     Parameters
     ----------
     adata
         The (annotated) data matrix of shape `n_obs` x `n_vars`.
         Rows correspond to cells and columns to regions.
@@ -632,14 +638,21 @@
     chunk_size
         Chunk size
     use_x
         If True, use the matrix stored in `.X` to compute the gene activity.
         Otherwise the `.obsm['insertion']` is used.
     id_type
         "gene" or "transcript".
+    upstream
+        The number of base pairs upstream of the regulatory domain.
+    downstream
+        The number of base pairs downstream of the regulatory domain.
+    include_gene_body
+        Whether to include the gene body in the regulatory domain. If False, the
+        TSS is used as the regulatory domain.
     transcript_name_key
         The key of the transcript name in the gene annotation file.
     transcript_id_key
         The key of the transcript id in the gene annotation file.
     gene_name_key
         The key of the gene name in the gene annotation file.
     gene_id_key
@@ -675,28 +688,30 @@
     --------
     >>> import snapatac2 as snap
     >>> data = snap.pp.import_data(snap.datasets.pbmc500(downsample=True), chrom_sizes=snap.genome.hg38, sorted_by_barcode=False)
     >>> gene_mat = snap.pp.make_gene_matrix(data, gene_anno=snap.genome.hg38)
     >>> print(gene_mat)
     AnnData object with n_obs × n_vars = 585 × 60606
         obs: 'n_fragment', 'frac_dup', 'frac_mito'
+    >>> gene_mat = snap.pp.make_gene_matrix(data, gene_anno=snap.genome.hg38, upstream=1000, downstream=1000, include_gene_body=False)
     """
     if isinstance(gene_anno, Genome):
         gene_anno = gene_anno.annotation
 
     if inplace:
         out = None
     elif file is None:
         if adata.isbacked:
             out = AnnData(obs=adata.obs[:].to_pandas())
         else:
             out = AnnData(obs=adata.obs[:])
     else:
         out = internal.AnnData(filename=file, backend=backend, obs=adata.obs[:])
     internal.mk_gene_matrix(adata, gene_anno, chunk_size, use_x, id_type,
+        upstream, downstream, include_gene_body,
         transcript_name_key, transcript_id_key, gene_name_key, gene_id_key,
         counting_strategy, min_frag_size, max_frag_size, out)
     return out
 
 def filter_cells(
     data: internal.AnnData | list[internal.AnnData],
     min_counts: int | None = 1000,
```

### Comparing `snapatac2-2.6.3/python/snapatac2/_utils.py` & `snapatac2-2.6.4/python/snapatac2/_utils.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/python/snapatac2/genome.py` & `snapatac2-2.6.4/python/snapatac2/genome.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/python/snapatac2/export/__init__.py` & `snapatac2-2.6.4/python/snapatac2/export/__init__.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/LICENSE` & `snapatac2-2.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `snapatac2-2.6.3/PKG-INFO` & `snapatac2-2.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.3
 Name: snapatac2
-Version: 2.6.3
+Version: 2.6.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: anndata >=0.8.0, <0.11.0
 Requires-Dist: kaleido
 Requires-Dist: multiprocess
 Requires-Dist: macs3 >=3.0, <3.1
 Requires-Dist: natsort
 Requires-Dist: numpy >=1.16.0, <2.0.0
 Requires-Dist: pandas >=1.0, <2.1.2
-Requires-Dist: plotly >=5.6.0
+Requires-Dist: plotly >=5.19.0, <6.0.0
 Requires-Dist: polars >=0.20.0, <0.21.0
 Requires-Dist: pooch >=1.6.0, <2.0.0
 Requires-Dist: igraph >=0.10.3
 Requires-Dist: pyarrow
 Requires-Dist: pyfaidx >=0.7.0, <0.8.0
 Requires-Dist: rustworkx
 Requires-Dist: scipy >=1.4, <2.0.0
```

