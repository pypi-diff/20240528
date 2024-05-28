# Comparing `tmp/subgroups-0.1.6.tar.gz` & `tmp/subgroups-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subgroups-0.1.6.tar", last modified: Sat Mar 23 00:26:21 2024, max compression
+gzip compressed data, was "subgroups-0.1.7.tar", last modified: Tue May 28 09:59:41 2024, max compression
```

## Comparing `subgroups-0.1.6.tar` & `subgroups-0.1.7.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxrwxrwx   0        0        0        0 2024-03-23 00:26:21.632485 subgroups-0.1.6/
--rw-rw-rw-   0        0        0     1570 2024-03-06 17:41:16.000000 subgroups-0.1.6/LICENSE
--rw-rw-rw-   0        0        0       52 2024-03-07 16:24:46.000000 subgroups-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2554 2024-03-23 00:26:21.631484 subgroups-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1549 2024-03-23 00:26:03.000000 subgroups-0.1.6/README.md
--rw-rw-rw-   0        0        0      106 2022-12-08 11:48:51.000000 subgroups-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0     1251 2024-03-23 00:26:21.633484 subgroups-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1736 2024-03-21 17:06:11.000000 subgroups-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-23 00:26:21.445270 subgroups-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2024-03-23 00:26:21.461270 subgroups-0.1.6/src/subgroups/
--rw-rw-rw-   0        0        0      197 2024-03-23 00:26:03.000000 subgroups-0.1.6/src/subgroups/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-23 00:26:21.478270 subgroups-0.1.6/src/subgroups/algorithms/
--rw-rw-rw-   0        0        0      655 2024-03-07 16:24:46.000000 subgroups-0.1.6/src/subgroups/algorithms/__init__.py
--rw-rw-rw-   0        0        0      961 2024-03-22 13:39:35.000000 subgroups-0.1.6/src/subgroups/algorithms/algorithm.py
-drwxrwxrwx   0        0        0        0 2024-03-23 00:26:21.482270 subgroups-0.1.6/src/subgroups/algorithms/subgroup_lists/
--rw-rw-rw-   0        0        0        0 2024-03-07 16:24:46.000000 subgroups-0.1.6/src/subgroups/algorithms/subgroup_lists/__init__.py
--rw-rw-rw-   0        0        0    16624 2024-03-07 16:24:46.000000 subgroups-0.1.6/src/subgroups/algorithms/subgroup_lists/dslm.py
--rw-rw-rw-   0        0        0    19511 2024-03-22 11:03:40.000000 subgroups-0.1.6/src/subgroups/algorithms/subgroup_lists/gmsl.py
--rw-rw-rw-   0        0        0    13175 2024-03-07 16:24:46.000000 subgroups-0.1.6/src/subgroups/algorithms/subgroup_lists/psld.py
-drwxrwxrwx   0        0        0        0 2024-03-23 00:26:21.516270 subgroups-0.1.6/src/subgroups/algorithms/subgroup_sets/
--rw-rw-rw-   0        0        0        0 2024-03-07 16:24:46.000000 subgroups-0.1.6/src/subgroups/algorithms/subgroup_sets/__init__.py
--rw-rw-rw-   0        0        0    27379 2024-03-23 00:26:03.000000 subgroups-0.1.6/src/subgroups/algorithms/subgroup_sets/bsd.py
--rw-rw-rw-   0        0        0     7405 2024-03-23 00:26:03.000000 subgroups-0.1.6/src/subgroups/algorithms/subgroup_sets/cbsd.py
--rw-rw-rw-   0        0        0     7239 2024-03-23 00:26:03.000000 subgroups-0.1.6/src/subgroups/algorithms/subgroup_sets/cpbsd.py
--rw-rw-rw-   0        0        0    25173 2024-03-23 00:26:03.000000 subgroups-0.1.6/src/subgroups/algorithms/subgroup_sets/qfinder.py
--rw-rw-rw-   0        0        0    18628 2024-03-22 17:15:00.000000 subgroups-0.1.6/src/subgroups/algorithms/subgroup_sets/sdmap.py
--rw-rw-rw-   0        0        0    26268 2024-03-23 00:26:03.000000 subgroups-0.1.6/src/subgroups/algorithms/subgroup_sets/sdmapstar.py
--rw-rw-rw-   0        0        0    29284 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/algorithms/subgroup_sets/vlsd.py
-drwxrwxrwx   0        0        0        0 2024-03-23 00:26:21.525270 subgroups-0.1.6/src/subgroups/core/
--rw-rw-rw-   0        0        0      182 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/core/__init__.py
--rw-rw-rw-   0        0        0     5810 2024-03-23 00:26:03.000000 subgroups-0.1.6/src/subgroups/core/operator.py
--rw-rw-rw-   0        0        0    11365 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/core/pattern.py
--rw-rw-rw-   0        0        0    11995 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/core/selector.py
--rw-rw-rw-   0        0        0     7042 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/core/subgroup.py
-drwxrwxrwx   0        0        0        0 2024-03-23 00:26:21.561484 subgroups-0.1.6/src/subgroups/data_structures/
--rw-rw-rw-   0        0        0      650 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/data_structures/__init__.py
--rw-rw-rw-   0        0        0    12302 2024-03-23 00:26:03.000000 subgroups-0.1.6/src/subgroups/data_structures/bitset_bsd.py
--rw-rw-rw-   0        0        0     5800 2024-03-23 00:26:03.000000 subgroups-0.1.6/src/subgroups/data_structures/bitset_qfinder.py
--rw-rw-rw-   0        0        0    34798 2024-03-23 00:26:03.000000 subgroups-0.1.6/src/subgroups/data_structures/fp_tree_for_sdmap.py
--rw-rw-rw-   0        0        0    13266 2024-03-23 00:26:03.000000 subgroups-0.1.6/src/subgroups/data_structures/fp_tree_for_sdmapstar.py
--rw-rw-rw-   0        0        0     8465 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/data_structures/fp_tree_node.py
--rw-rw-rw-   0        0        0    14039 2024-03-23 00:26:03.000000 subgroups-0.1.6/src/subgroups/data_structures/subgroup_list.py
--rw-rw-rw-   0        0        0     7821 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/data_structures/vertical_list.py
--rw-rw-rw-   0        0        0    12148 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/data_structures/vertical_list_with_bitsets.py
--rw-rw-rw-   0        0        0    11011 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/data_structures/vertical_list_with_sets.py
-drwxrwxrwx   0        0        0        0 2024-03-23 00:26:21.562484 subgroups-0.1.6/src/subgroups/datasets/
--rw-rw-rw-   0        0        0     1480 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-23 00:26:21.577484 subgroups-0.1.6/src/subgroups/datasets/csv/
--rw-rw-rw-   0        0        0     2857 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/datasets/csv/balloons.csv
--rw-rw-rw-   0        0        0    53645 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/datasets/csv/car-evaluation.csv
--rw-rw-rw-   0        0        0     8716 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/datasets/csv/covid-sp.csv
--rw-rw-rw-   0        0        0   177691 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/datasets/csv/credit-g.csv
--rw-rw-rw-   0        0        0    58896 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/datasets/csv/heart-disease.csv
--rw-rw-rw-   0        0        0   106024 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/datasets/csv/income.csv
--rw-rw-rw-   0        0        0     1288 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/datasets/csv/lenses.csv
--rw-rw-rw-   0        0        0    16297 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/datasets/csv/lymph.csv
--rw-rw-rw-   0        0        0   365871 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/datasets/csv/mushroom.csv
--rw-rw-rw-   0        0        0      164 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/datasets/csv/shop.csv
--rw-rw-rw-   0        0        0   403751 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/datasets/csv/sick.csv
--rw-rw-rw-   0        0        0    27002 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/datasets/csv/tic-tac-toe.csv
--rw-rw-rw-   0        0        0    18966 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/datasets/csv/vote.csv
--rw-rw-rw-   0        0        0     1377 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-03-23 00:26:21.598484 subgroups-0.1.6/src/subgroups/quality_measures/
--rw-rw-rw-   0        0        0     1310 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/quality_measures/__init__.py
--rw-rw-rw-   0        0        0     2439 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/quality_measures/absolute_wracc.py
--rw-rw-rw-   0        0        0     3541 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/quality_measures/binomial_test.py
--rw-rw-rw-   0        0        0     3479 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/quality_measures/binomial_test_optimistic_estimate_1.py
--rw-rw-rw-   0        0        0     3295 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/quality_measures/coverage.py
--rw-rw-rw-   0        0        0     3143 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/quality_measures/f1_score.py
--rw-rw-rw-   0        0        0     3073 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/quality_measures/irr.py
--rw-rw-rw-   0        0        0     3314 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/quality_measures/npv.py
--rw-rw-rw-   0        0        0     3507 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/quality_measures/piatetsky_shapiro.py
--rw-rw-rw-   0        0        0     3861 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/quality_measures/piatetsky_shapiro_optimistic_estimate_1.py
--rw-rw-rw-   0        0        0     3626 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/quality_measures/piatetsky_shapiro_optimistic_estimate_2.py
--rw-rw-rw-   0        0        0     2789 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/quality_measures/ppv.py
--rw-rw-rw-   0        0        0     3418 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/quality_measures/qg.py
--rw-rw-rw-   0        0        0     3533 2024-03-22 13:39:53.000000 subgroups-0.1.6/src/subgroups/quality_measures/quality_measure.py
--rw-rw-rw-   0        0        0     2966 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/quality_measures/sensitivity.py
--rw-rw-rw-   0        0        0     2957 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/quality_measures/specificity.py
--rw-rw-rw-   0        0        0     3024 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/quality_measures/support.py
--rw-rw-rw-   0        0        0     3355 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/quality_measures/wracc.py
--rw-rw-rw-   0        0        0     3660 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/quality_measures/wracc_optimistic_estimate_1.py
--rw-rw-rw-   0        0        0     3304 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/quality_measures/youden.py
-drwxrwxrwx   0        0        0        0 2024-03-23 00:26:21.599483 subgroups-0.1.6/src/subgroups/tests/
--rw-rw-rw-   0        0        0     2670 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-23 00:26:21.600484 subgroups-0.1.6/src/subgroups/tests/algorithms/
--rw-rw-rw-   0        0        0        0 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/algorithms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-23 00:26:21.602484 subgroups-0.1.6/src/subgroups/tests/algorithms/subgroup_lists/
--rw-rw-rw-   0        0        0        0 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/algorithms/subgroup_lists/__init__.py
--rw-rw-rw-   0        0        0    14577 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/algorithms/subgroup_lists/test_dslm.py
--rw-rw-rw-   0        0        0    59342 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/algorithms/subgroup_lists/test_gmsl.py
-drwxrwxrwx   0        0        0        0 2024-03-23 00:26:21.610484 subgroups-0.1.6/src/subgroups/tests/algorithms/subgroup_sets/
--rw-rw-rw-   0        0        0        0 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/algorithms/subgroup_sets/__init__.py
--rw-rw-rw-   0        0        0     7502 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/algorithms/subgroup_sets/test_bsd.py
--rw-rw-rw-   0        0        0     7517 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/algorithms/subgroup_sets/test_cbsd.py
--rw-rw-rw-   0        0        0     7266 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/algorithms/subgroup_sets/test_cpbsd.py
--rw-rw-rw-   0        0        0     9750 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/algorithms/subgroup_sets/test_qfinder.py
--rw-rw-rw-   0        0        0    32790 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/algorithms/subgroup_sets/test_sdmap.py
--rw-rw-rw-   0        0        0    37583 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/algorithms/subgroup_sets/test_sdmapstar.py
--rw-rw-rw-   0        0        0    29941 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/algorithms/subgroup_sets/test_vlsd.py
-drwxrwxrwx   0        0        0        0 2024-03-23 00:26:21.615483 subgroups-0.1.6/src/subgroups/tests/core/
--rw-rw-rw-   0        0        0        0 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/core/__init__.py
--rw-rw-rw-   0        0        0     9548 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/core/test_operator.py
--rw-rw-rw-   0        0        0    15907 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/core/test_pattern.py
--rw-rw-rw-   0        0        0    22328 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/core/test_selector.py
--rw-rw-rw-   0        0        0     9584 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/core/test_subgroup.py
-drwxrwxrwx   0        0        0        0 2024-03-23 00:26:21.621484 subgroups-0.1.6/src/subgroups/tests/data_structures/
--rw-rw-rw-   0        0        0        0 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/data_structures/__init__.py
--rw-rw-rw-   0        0        0    75823 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/data_structures/test_fp_tree_for_sdmap.py
--rw-rw-rw-   0        0        0     7489 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/data_structures/test_fp_tree_node.py
--rw-rw-rw-   0        0        0    55154 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/data_structures/test_subgroup_list.py
--rw-rw-rw-   0        0        0    10503 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/data_structures/test_vertical_list_with_bitsets.py
--rw-rw-rw-   0        0        0    10137 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/data_structures/test_vertical_list_with_sets.py
-drwxrwxrwx   0        0        0        0 2024-03-23 00:26:21.622483 subgroups-0.1.6/src/subgroups/tests/quality_measures/
--rw-rw-rw-   0        0        0        0 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/quality_measures/__init__.py
--rw-rw-rw-   0        0        0    15883 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/quality_measures/test_quality_measures.py
-drwxrwxrwx   0        0        0        0 2024-03-23 00:26:21.626484 subgroups-0.1.6/src/subgroups/tests/utils/
--rw-rw-rw-   0        0        0        0 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/utils/__init__.py
--rw-rw-rw-   0        0        0     1913 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/utils/test_dataframe_filters.py
--rw-rw-rw-   0        0        0   120959 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/tests/utils/test_file_format_transformations.py
-drwxrwxrwx   0        0        0        0 2024-03-23 00:26:21.630484 subgroups-0.1.6/src/subgroups/utils/
--rw-rw-rw-   0        0        0        0 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/utils/__init__.py
--rw-rw-rw-   0        0        0     2172 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/utils/dataframe_filters.py
--rw-rw-rw-   0        0        0     1939 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/utils/file_format_transformations.py
--rw-rw-rw-   0        0        0     4548 2024-03-07 16:24:47.000000 subgroups-0.1.6/src/subgroups/utils/mdl.py
-drwxrwxrwx   0        0        0        0 2024-03-23 00:26:21.631484 subgroups-0.1.6/src/subgroups.egg-info/
--rw-rw-rw-   0        0        0     2554 2024-03-23 00:26:21.000000 subgroups-0.1.6/src/subgroups.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4877 2024-03-23 00:26:21.000000 subgroups-0.1.6/src/subgroups.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-23 00:26:21.000000 subgroups-0.1.6/src/subgroups.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-23 00:26:21.000000 subgroups-0.1.6/src/subgroups.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       50 2024-03-23 00:26:21.000000 subgroups-0.1.6/src/subgroups.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-23 00:26:21.000000 subgroups-0.1.6/src/subgroups.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 09:59:41.784426 subgroups-0.1.7/
+-rw-rw-rw-   0        0        0     1696 2024-05-28 09:42:43.000000 subgroups-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0       52 2024-03-18 09:46:34.000000 subgroups-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     6314 2024-05-28 09:59:41.784426 subgroups-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5308 2024-05-28 09:42:43.000000 subgroups-0.1.7/README.md
+-rw-rw-rw-   0        0        0      106 2023-01-23 11:41:19.000000 subgroups-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0     1252 2024-05-28 09:59:41.788454 subgroups-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1736 2024-03-18 09:46:34.000000 subgroups-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:59:41.610693 subgroups-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2024-05-28 09:59:41.632020 subgroups-0.1.7/src/subgroups/
+-rw-rw-rw-   0        0        0      197 2024-05-28 09:42:43.000000 subgroups-0.1.7/src/subgroups/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:59:41.647701 subgroups-0.1.7/src/subgroups/algorithms/
+-rw-rw-rw-   0        0        0      655 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/algorithms/__init__.py
+-rw-rw-rw-   0        0        0      961 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/algorithms/algorithm.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:59:41.647701 subgroups-0.1.7/src/subgroups/algorithms/subgroup_lists/
+-rw-rw-rw-   0        0        0        0 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/algorithms/subgroup_lists/__init__.py
+-rw-rw-rw-   0        0        0    16624 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/algorithms/subgroup_lists/dslm.py
+-rw-rw-rw-   0        0        0    19511 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/algorithms/subgroup_lists/gmsl.py
+-rw-rw-rw-   0        0        0    13175 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/algorithms/subgroup_lists/psld.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:59:41.663280 subgroups-0.1.7/src/subgroups/algorithms/subgroup_sets/
+-rw-rw-rw-   0        0        0        0 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/algorithms/subgroup_sets/__init__.py
+-rw-rw-rw-   0        0        0    27345 2024-05-28 09:42:43.000000 subgroups-0.1.7/src/subgroups/algorithms/subgroup_sets/bsd.py
+-rw-rw-rw-   0        0        0     7396 2024-05-28 09:42:43.000000 subgroups-0.1.7/src/subgroups/algorithms/subgroup_sets/cbsd.py
+-rw-rw-rw-   0        0        0     7220 2024-05-28 09:42:43.000000 subgroups-0.1.7/src/subgroups/algorithms/subgroup_sets/cpbsd.py
+-rw-rw-rw-   0        0        0    22715 2024-05-28 09:42:43.000000 subgroups-0.1.7/src/subgroups/algorithms/subgroup_sets/qfinder.py
+-rw-rw-rw-   0        0        0    18628 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/algorithms/subgroup_sets/sdmap.py
+-rw-rw-rw-   0        0        0    26246 2024-05-28 09:42:43.000000 subgroups-0.1.7/src/subgroups/algorithms/subgroup_sets/sdmapstar.py
+-rw-rw-rw-   0        0        0    29284 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/algorithms/subgroup_sets/vlsd.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:59:41.663280 subgroups-0.1.7/src/subgroups/core/
+-rw-rw-rw-   0        0        0      182 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/core/__init__.py
+-rw-rw-rw-   0        0        0     5804 2024-05-28 09:42:43.000000 subgroups-0.1.7/src/subgroups/core/operator.py
+-rw-rw-rw-   0        0        0    11365 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/core/pattern.py
+-rw-rw-rw-   0        0        0    11995 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/core/selector.py
+-rw-rw-rw-   0        0        0     7042 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/core/subgroup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:59:41.678906 subgroups-0.1.7/src/subgroups/data_structures/
+-rw-rw-rw-   0        0        0      650 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/data_structures/__init__.py
+-rw-rw-rw-   0        0        0    12246 2024-05-28 09:42:43.000000 subgroups-0.1.7/src/subgroups/data_structures/bitset_bsd.py
+-rw-rw-rw-   0        0        0     5579 2024-05-28 09:42:43.000000 subgroups-0.1.7/src/subgroups/data_structures/bitset_qfinder.py
+-rw-rw-rw-   0        0        0    34777 2024-05-28 09:42:43.000000 subgroups-0.1.7/src/subgroups/data_structures/fp_tree_for_sdmap.py
+-rw-rw-rw-   0        0        0    13104 2024-05-28 09:42:43.000000 subgroups-0.1.7/src/subgroups/data_structures/fp_tree_for_sdmapstar.py
+-rw-rw-rw-   0        0        0     8465 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/data_structures/fp_tree_node.py
+-rw-rw-rw-   0        0        0    14069 2024-05-28 09:42:43.000000 subgroups-0.1.7/src/subgroups/data_structures/subgroup_list.py
+-rw-rw-rw-   0        0        0     7821 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/data_structures/vertical_list.py
+-rw-rw-rw-   0        0        0    12148 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/data_structures/vertical_list_with_bitsets.py
+-rw-rw-rw-   0        0        0    11011 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/data_structures/vertical_list_with_sets.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:59:41.678906 subgroups-0.1.7/src/subgroups/datasets/
+-rw-rw-rw-   0        0        0     1480 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:59:41.710664 subgroups-0.1.7/src/subgroups/datasets/csv/
+-rw-rw-rw-   0        0        0     2857 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/datasets/csv/balloons.csv
+-rw-rw-rw-   0        0        0    53645 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/datasets/csv/car-evaluation.csv
+-rw-rw-rw-   0        0        0     8716 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/datasets/csv/covid-sp.csv
+-rw-rw-rw-   0        0        0   177691 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/datasets/csv/credit-g.csv
+-rw-rw-rw-   0        0        0    58896 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/datasets/csv/heart-disease.csv
+-rw-rw-rw-   0        0        0   106024 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/datasets/csv/income.csv
+-rw-rw-rw-   0        0        0     1288 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/datasets/csv/lenses.csv
+-rw-rw-rw-   0        0        0    16297 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/datasets/csv/lymph.csv
+-rw-rw-rw-   0        0        0   365871 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/datasets/csv/mushroom.csv
+-rw-rw-rw-   0        0        0      164 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/datasets/csv/shop.csv
+-rw-rw-rw-   0        0        0   403751 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/datasets/csv/sick.csv
+-rw-rw-rw-   0        0        0    27002 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/datasets/csv/tic-tac-toe.csv
+-rw-rw-rw-   0        0        0    18966 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/datasets/csv/vote.csv
+-rw-rw-rw-   0        0        0     1377 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:59:41.726302 subgroups-0.1.7/src/subgroups/quality_measures/
+-rw-rw-rw-   0        0        0     1310 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/quality_measures/__init__.py
+-rw-rw-rw-   0        0        0     2439 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/quality_measures/absolute_wracc.py
+-rw-rw-rw-   0        0        0     3541 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/quality_measures/binomial_test.py
+-rw-rw-rw-   0        0        0     3479 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/quality_measures/binomial_test_optimistic_estimate_1.py
+-rw-rw-rw-   0        0        0     3295 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/quality_measures/coverage.py
+-rw-rw-rw-   0        0        0     3143 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/quality_measures/f1_score.py
+-rw-rw-rw-   0        0        0     3073 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/quality_measures/irr.py
+-rw-rw-rw-   0        0        0     3314 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/quality_measures/npv.py
+-rw-rw-rw-   0        0        0     3507 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/quality_measures/piatetsky_shapiro.py
+-rw-rw-rw-   0        0        0     3861 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/quality_measures/piatetsky_shapiro_optimistic_estimate_1.py
+-rw-rw-rw-   0        0        0     3626 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/quality_measures/piatetsky_shapiro_optimistic_estimate_2.py
+-rw-rw-rw-   0        0        0     2789 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/quality_measures/ppv.py
+-rw-rw-rw-   0        0        0     3418 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/quality_measures/qg.py
+-rw-rw-rw-   0        0        0     3533 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/quality_measures/quality_measure.py
+-rw-rw-rw-   0        0        0     2966 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/quality_measures/sensitivity.py
+-rw-rw-rw-   0        0        0     2957 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/quality_measures/specificity.py
+-rw-rw-rw-   0        0        0     3024 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/quality_measures/support.py
+-rw-rw-rw-   0        0        0     3355 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/quality_measures/wracc.py
+-rw-rw-rw-   0        0        0     3660 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/quality_measures/wracc_optimistic_estimate_1.py
+-rw-rw-rw-   0        0        0     3304 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/quality_measures/youden.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:59:41.726302 subgroups-0.1.7/src/subgroups/tests/
+-rw-rw-rw-   0        0        0     2670 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:59:41.726302 subgroups-0.1.7/src/subgroups/tests/algorithms/
+-rw-rw-rw-   0        0        0        0 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/algorithms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:59:41.746896 subgroups-0.1.7/src/subgroups/tests/algorithms/subgroup_lists/
+-rw-rw-rw-   0        0        0        0 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/algorithms/subgroup_lists/__init__.py
+-rw-rw-rw-   0        0        0    14577 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/algorithms/subgroup_lists/test_dslm.py
+-rw-rw-rw-   0        0        0    59402 2024-05-28 09:42:43.000000 subgroups-0.1.7/src/subgroups/tests/algorithms/subgroup_lists/test_gmsl.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:59:41.756325 subgroups-0.1.7/src/subgroups/tests/algorithms/subgroup_sets/
+-rw-rw-rw-   0        0        0        0 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/algorithms/subgroup_sets/__init__.py
+-rw-rw-rw-   0        0        0     7502 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/algorithms/subgroup_sets/test_bsd.py
+-rw-rw-rw-   0        0        0     7517 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/algorithms/subgroup_sets/test_cbsd.py
+-rw-rw-rw-   0        0        0     7266 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/algorithms/subgroup_sets/test_cpbsd.py
+-rw-rw-rw-   0        0        0     9279 2024-05-28 09:42:43.000000 subgroups-0.1.7/src/subgroups/tests/algorithms/subgroup_sets/test_qfinder.py
+-rw-rw-rw-   0        0        0    32790 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/algorithms/subgroup_sets/test_sdmap.py
+-rw-rw-rw-   0        0        0    37583 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/algorithms/subgroup_sets/test_sdmapstar.py
+-rw-rw-rw-   0        0        0    29941 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/algorithms/subgroup_sets/test_vlsd.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:59:41.761327 subgroups-0.1.7/src/subgroups/tests/core/
+-rw-rw-rw-   0        0        0        0 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/core/__init__.py
+-rw-rw-rw-   0        0        0     9548 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/core/test_operator.py
+-rw-rw-rw-   0        0        0    15907 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/core/test_pattern.py
+-rw-rw-rw-   0        0        0    22328 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/core/test_selector.py
+-rw-rw-rw-   0        0        0     9584 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/core/test_subgroup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:59:41.771435 subgroups-0.1.7/src/subgroups/tests/data_structures/
+-rw-rw-rw-   0        0        0        0 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/data_structures/__init__.py
+-rw-rw-rw-   0        0        0    75823 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/data_structures/test_fp_tree_for_sdmap.py
+-rw-rw-rw-   0        0        0     7489 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/data_structures/test_fp_tree_node.py
+-rw-rw-rw-   0        0        0    57171 2024-05-28 09:42:43.000000 subgroups-0.1.7/src/subgroups/tests/data_structures/test_subgroup_list.py
+-rw-rw-rw-   0        0        0    10503 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/data_structures/test_vertical_list_with_bitsets.py
+-rw-rw-rw-   0        0        0    10137 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/data_structures/test_vertical_list_with_sets.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:59:41.771435 subgroups-0.1.7/src/subgroups/tests/quality_measures/
+-rw-rw-rw-   0        0        0        0 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/quality_measures/__init__.py
+-rw-rw-rw-   0        0        0    15883 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/quality_measures/test_quality_measures.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:59:41.771435 subgroups-0.1.7/src/subgroups/tests/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/utils/__init__.py
+-rw-rw-rw-   0        0        0     1913 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/utils/test_dataframe_filters.py
+-rw-rw-rw-   0        0        0   120959 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/tests/utils/test_file_format_transformations.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:59:41.782425 subgroups-0.1.7/src/subgroups/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/utils/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/utils/dataframe_filters.py
+-rw-rw-rw-   0        0        0     1939 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/utils/file_format_transformations.py
+-rw-rw-rw-   0        0        0     4548 2024-03-18 09:46:34.000000 subgroups-0.1.7/src/subgroups/utils/mdl.py
+drwxrwxrwx   0        0        0        0 2024-05-28 09:59:41.783426 subgroups-0.1.7/src/subgroups.egg-info/
+-rw-rw-rw-   0        0        0     6314 2024-05-28 09:59:41.000000 subgroups-0.1.7/src/subgroups.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4877 2024-05-28 09:59:41.000000 subgroups-0.1.7/src/subgroups.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 09:59:41.000000 subgroups-0.1.7/src/subgroups.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-28 09:59:41.000000 subgroups-0.1.7/src/subgroups.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       50 2024-05-28 09:59:41.000000 subgroups-0.1.7/src/subgroups.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-28 09:59:41.000000 subgroups-0.1.7/src/subgroups.egg-info/top_level.txt
```

### Comparing `subgroups-0.1.6/LICENSE` & `subgroups-0.1.7/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-BSD 3-Clause License
+BSD 4-Clause License
 
 Copyright (c) 2021, Antonio López Martínez-Carrasco
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
 
 2. Redistributions in binary form must reproduce the above copyright notice,
    this list of conditions and the following disclaimer in the documentation
    and/or other materials provided with the distribution.
 
-3. Neither the name of the copyright holder nor the names of its
+3. All materials mentioning features or use of this software must cite the
+   paper in which this software was published.
+
+4. Neither the name of the copyright holder nor the names of its
    contributors may be used to endorse or promote products derived from
    this software without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
 AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
 IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
```

### Comparing `subgroups-0.1.6/setup.cfg` & `subgroups-0.1.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -6,74 +6,74 @@
 00000050: 203d 2073 7562 6772 6f75 7073 2069 7320   = subgroups is 
 00000060: 6120 7079 7468 6f6e 206c 6962 7261 7279  a python library
 00000070: 2077 6869 6368 2063 6f6e 7461 696e 7320   which contains 
 00000080: 6120 636f 6c6c 6563 7469 6f6e 206f 6620  a collection of 
 00000090: 7375 6267 726f 7570 2064 6973 636f 7665  subgroup discove
 000000a0: 7279 2061 6c67 6f72 6974 686d 7320 616e  ry algorithms an
 000000b0: 6420 6f74 6865 7220 6461 7461 2061 6e61  d other data ana
-000000c0: 6c79 7369 7320 7574 696c 6974 6965 730d  lysis utilities.
-000000d0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-000000e0: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
-000000f0: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
-00000100: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
-00000110: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
-00000120: 776e 0d0a 6b65 7977 6f72 6473 203d 2070  wn..keywords = p
-00000130: 7974 686f 6e2c 2064 6174 612d 7363 6965  ython, data-scie
-00000140: 6e63 652c 206d 6163 6869 6e65 2d6c 6561  nce, machine-lea
-00000150: 726e 696e 672c 2064 6174 612d 616e 616c  rning, data-anal
-00000160: 7973 6973 2c20 7375 6267 726f 7570 732c  ysis, subgroups,
-00000170: 2073 7562 6772 6f75 702d 6469 7363 6f76   subgroup-discov
-00000180: 6572 790d 0a6c 6963 656e 7365 203d 2042  ery..license = B
-00000190: 5344 2d33 2d43 6c61 7573 650d 0a6c 6963  SD-3-Clause..lic
-000001a0: 656e 7365 5f66 696c 6573 203d 204c 4943  ense_files = LIC
-000001b0: 454e 5345 0d0a 706c 6174 666f 726d 7320  ENSE..platforms 
-000001c0: 3d20 616e 790d 0a63 6c61 7373 6966 6965  = any..classifie
-000001d0: 7273 203d 200d 0a09 5072 6f67 7261 6d6d  rs = ...Programm
-000001e0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000001f0: 5079 7468 6f6e 203a 3a20 330d 0a09 5072  Python :: 3...Pr
-00000200: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000210: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000220: 3320 3a3a 204f 6e6c 790d 0a09 5072 6f67  3 :: Only...Prog
-00000230: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000240: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000250: 390d 0a09 4c69 6365 6e73 6520 3a3a 204f  9...License :: O
-00000260: 5349 2041 7070 726f 7665 6420 3a3a 2042  SI Approved :: B
-00000270: 5344 204c 6963 656e 7365 0d0a 094f 7065  SD License...Ope
-00000280: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-00000290: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
-000002a0: 0a61 7574 686f 7220 3d20 416e 746f 6e69  .author = Antoni
-000002b0: 6f20 4cc3 b370 657a 204d 6172 74c3 ad6e  o L..pez Mart..n
-000002c0: 657a 2d43 6172 7261 7363 6f0d 0a61 7574  ez-Carrasco..aut
-000002d0: 686f 725f 656d 6169 6c20 3d20 616e 746f  hor_email = anto
-000002e0: 6e69 6f6c 6f70 657a 6d63 3139 3935 4067  niolopezmc1995@g
-000002f0: 6d61 696c 2e63 6f6d 0d0a 6d61 696e 7461  mail.com..mainta
-00000300: 696e 6572 203d 2041 6e74 6f6e 696f 204c  iner = Antonio L
-00000310: c3b3 7065 7a20 4d61 7274 c3ad 6e65 7a2d  ..pez Mart..nez-
-00000320: 4361 7272 6173 636f 0d0a 6d61 696e 7461  Carrasco..mainta
-00000330: 696e 6572 5f65 6d61 696c 203d 2061 6e74  iner_email = ant
-00000340: 6f6e 696f 6c6f 7065 7a6d 6331 3939 3540  oniolopezmc1995@
-00000350: 676d 6169 6c2e 636f 6d0d 0a75 726c 203d  gmail.com..url =
-00000360: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000370: 636f 6d2f 616e 746f 6e69 6f6c 6f70 657a  com/antoniolopez
-00000380: 6d63 2f73 7562 6772 6f75 7073 0d0a 0d0a  mc/subgroups....
-00000390: 5b6f 7074 696f 6e73 5d0d 0a70 7974 686f  [options]..pytho
-000003a0: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-000003b0: 2e39 2e30 0d0a 7a69 705f 7361 6665 203d  .9.0..zip_safe =
-000003c0: 2046 616c 7365 0d0a 696e 636c 7564 655f   False..include_
-000003d0: 7061 636b 6167 655f 6461 7461 203d 2054  package_data = T
-000003e0: 7275 650d 0a70 6163 6b61 6765 7320 3d20  rue..packages = 
-000003f0: 6669 6e64 3a0d 0a69 6e73 7461 6c6c 5f72  find:..install_r
-00000400: 6571 7569 7265 7320 3d20 0d0a 0970 616e  equires = ...pan
-00000410: 6461 733e 3d32 2e30 2e33 0d0a 0962 6974  das>=2.0.3...bit
-00000420: 6172 7261 793e 3d32 2e37 2e36 0d0a 0973  array>=2.7.6...s
-00000430: 7461 7473 6d6f 6465 6c73 3e3d 302e 3134  tatsmodels>=0.14
-00000440: 2e30 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .0....[options.p
-00000450: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
-00000460: 6865 7265 203d 2073 7263 0d0a 696e 636c  here = src..incl
-00000470: 7564 6520 3d20 0d0a 0973 7562 6772 6f75  ude = ...subgrou
-00000480: 7073 0d0a 0973 7562 6772 6f75 7073 2e2a  ps...subgroups.*
-00000490: 0d0a 6578 636c 7564 6520 3d20 0d0a 0962  ..exclude = ...b
-000004a0: 7569 6c64 2a0d 0a09 6469 7374 2a0d 0a09  uild*...dist*...
-000004b0: 646f 6373 2a0d 0a0d 0a5b 6567 675f 696e  docs*....[egg_in
-000004c0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-000004d0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-000004e0: 0a0d 0a                                  ...
+000000c0: 6c79 7369 7320 7574 696c 6974 6965 732e  lysis utilities.
+000000d0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+000000e0: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
+000000f0: 452e 6d64 0d0a 6c6f 6e67 5f64 6573 6372  E.md..long_descr
+00000100: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
+00000110: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
+00000120: 6f77 6e0d 0a6b 6579 776f 7264 7320 3d20  own..keywords = 
+00000130: 7079 7468 6f6e 2c20 6461 7461 2d73 6369  python, data-sci
+00000140: 656e 6365 2c20 6d61 6368 696e 652d 6c65  ence, machine-le
+00000150: 6172 6e69 6e67 2c20 6461 7461 2d61 6e61  arning, data-ana
+00000160: 6c79 7369 732c 2073 7562 6772 6f75 7073  lysis, subgroups
+00000170: 2c20 7375 6267 726f 7570 2d64 6973 636f  , subgroup-disco
+00000180: 7665 7279 0d0a 6c69 6365 6e73 6520 3d20  very..license = 
+00000190: 4253 442d 342d 436c 6175 7365 0d0a 6c69  BSD-4-Clause..li
+000001a0: 6365 6e73 655f 6669 6c65 7320 3d20 4c49  cense_files = LI
+000001b0: 4345 4e53 450d 0a70 6c61 7466 6f72 6d73  CENSE..platforms
+000001c0: 203d 2061 6e79 0d0a 636c 6173 7369 6669   = any..classifi
+000001d0: 6572 7320 3d20 0d0a 0950 726f 6772 616d  ers = ...Program
+000001e0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000001f0: 2050 7974 686f 6e20 3a3a 2033 0d0a 0950   Python :: 3...P
+00000200: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000210: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000220: 2033 203a 3a20 4f6e 6c79 0d0a 0950 726f   3 :: Only...Pro
+00000230: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000240: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000250: 2e39 0d0a 094c 6963 656e 7365 203a 3a20  .9...License :: 
+00000260: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+00000270: 4253 4420 4c69 6365 6e73 650d 0a09 4f70  BSD License...Op
+00000280: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
+00000290: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
+000002a0: 0d0a 6175 7468 6f72 203d 2041 6e74 6f6e  ..author = Anton
+000002b0: 696f 204c c3b3 7065 7a20 4d61 7274 c3ad  io L..pez Mart..
+000002c0: 6e65 7a2d 4361 7272 6173 636f 0d0a 6175  nez-Carrasco..au
+000002d0: 7468 6f72 5f65 6d61 696c 203d 2061 6e74  thor_email = ant
+000002e0: 6f6e 696f 6c6f 7065 7a6d 6331 3939 3540  oniolopezmc1995@
+000002f0: 676d 6169 6c2e 636f 6d0d 0a6d 6169 6e74  gmail.com..maint
+00000300: 6169 6e65 7220 3d20 416e 746f 6e69 6f20  ainer = Antonio 
+00000310: 4cc3 b370 657a 204d 6172 74c3 ad6e 657a  L..pez Mart..nez
+00000320: 2d43 6172 7261 7363 6f0d 0a6d 6169 6e74  -Carrasco..maint
+00000330: 6169 6e65 725f 656d 6169 6c20 3d20 616e  ainer_email = an
+00000340: 746f 6e69 6f6c 6f70 657a 6d63 3139 3935  toniolopezmc1995
+00000350: 4067 6d61 696c 2e63 6f6d 0d0a 7572 6c20  @gmail.com..url 
+00000360: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+00000370: 2e63 6f6d 2f61 6e74 6f6e 696f 6c6f 7065  .com/antoniolope
+00000380: 7a6d 632f 7375 6267 726f 7570 730d 0a0d  zmc/subgroups...
+00000390: 0a5b 6f70 7469 6f6e 735d 0d0a 7079 7468  .[options]..pyth
+000003a0: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
+000003b0: 332e 392e 300d 0a7a 6970 5f73 6166 6520  3.9.0..zip_safe 
+000003c0: 3d20 4661 6c73 650d 0a69 6e63 6c75 6465  = False..include
+000003d0: 5f70 6163 6b61 6765 5f64 6174 6120 3d20  _package_data = 
+000003e0: 5472 7565 0d0a 7061 636b 6167 6573 203d  True..packages =
+000003f0: 2066 696e 643a 0d0a 696e 7374 616c 6c5f   find:..install_
+00000400: 7265 7175 6972 6573 203d 200d 0a09 7061  requires = ...pa
+00000410: 6e64 6173 3e3d 322e 302e 330d 0a09 6269  ndas>=2.0.3...bi
+00000420: 7461 7272 6179 3e3d 322e 372e 360d 0a09  tarray>=2.7.6...
+00000430: 7374 6174 736d 6f64 656c 733e 3d30 2e31  statsmodels>=0.1
+00000440: 342e 300d 0a0d 0a5b 6f70 7469 6f6e 732e  4.0....[options.
+00000450: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
+00000460: 7768 6572 6520 3d20 7372 630d 0a69 6e63  where = src..inc
+00000470: 6c75 6465 203d 200d 0a09 7375 6267 726f  lude = ...subgro
+00000480: 7570 730d 0a09 7375 6267 726f 7570 732e  ups...subgroups.
+00000490: 2a0d 0a65 7863 6c75 6465 203d 200d 0a09  *..exclude = ...
+000004a0: 6275 696c 642a 0d0a 0964 6973 742a 0d0a  build*...dist*..
+000004b0: 0964 6f63 732a 0d0a 0d0a 5b65 6767 5f69  .docs*....[egg_i
+000004c0: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+000004d0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+000004e0: 0d0a 0d0a                                ....
```

### Comparing `subgroups-0.1.6/setup.py` & `subgroups-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/algorithms/__init__.py` & `subgroups-0.1.7/src/subgroups/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/algorithms/algorithm.py` & `subgroups-0.1.7/src/subgroups/algorithms/algorithm.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/algorithms/subgroup_lists/dslm.py` & `subgroups-0.1.7/src/subgroups/algorithms/subgroup_lists/dslm.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/algorithms/subgroup_lists/gmsl.py` & `subgroups-0.1.7/src/subgroups/algorithms/subgroup_lists/gmsl.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/algorithms/subgroup_lists/psld.py` & `subgroups-0.1.7/src/subgroups/algorithms/subgroup_lists/psld.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/algorithms/subgroup_sets/bsd.py` & `subgroups-0.1.7/src/subgroups/algorithms/subgroup_sets/bsd.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,38 +75,38 @@
         if (type(write_results_in_file) is not bool):
             raise TypeError("The type of the parameter 'write_results_in_file' must be 'bool'")
         if ((type(file_path) is not str) and (file_path is not None)):
             raise TypeError("The type of the parameter 'file_path' must be 'str' or 'NoneType'.")
         # If 'write_results_in_file' is True, 'file_path' must not be None.
         if (write_results_in_file) and (file_path is None):
             raise ValueError("If the parameter 'write_results_in_file' is True, the parameter 'file_path' must not be None.")
-         # We check whether 'optimistic_estimate' is an optimistic estimate of 'quality_measure'.
+        # We check whether 'optimistic_estimate' is an optimistic estimate of 'quality_measure'.
         if quality_measure.get_name() not in optimistic_estimate.optimistic_estimate_of():
             raise ValueError("The quality measure " + optimistic_estimate.get_name() + " is not an optimistic estimate of the quality measure " + quality_measure.get_name() + ".")
         self._maxDepth = max_depth
         self._min_support = min_support
         self._quality_measure = quality_measure
         self._optimistic_estimate = optimistic_estimate
         self._num_subgroups = num_subgroups
         # We initialize the list of subgroups with a dummy subgroup.
-                        #(quality, subgroup, bits, optimistic_estimate,(tp,fp))
+        #     (quality, subgroup, bits, optimistic_estimate, (tp,fp))
         self._k_subgroups = [(-99999,Pattern([]),bitarray(),-99999,(0,0))]
         self._TP = 0
         self._FP = 0
         self._irrelevants = []  #List of unselected subgroups.
         self._visited_subgroups = 0
         self._selected_subgroups = 0
         self._unselected_subgroups = 0
         self._additional_parameters_for_the_quality_measure = additional_parameters_for_the_quality_measure.copy()
         _delete_subgroup_parameters_from_a_dictionary(self._additional_parameters_for_the_quality_measure)
         self._additional_parameters_for_the_optimistic_estimate = additional_parameters_for_the_optimistic_estimate.copy()
         _delete_subgroup_parameters_from_a_dictionary(self._additional_parameters_for_the_optimistic_estimate)
         # We only write the results in a file if the parameter 'write_results_in_file' is True.
         if (write_results_in_file):
-                self._file_path = file_path
+            self._file_path = file_path
         else:
             self._file_path = None
         self._file = None
 
     def _get_minimum_support(self) -> Union[int,float]:
         return self._min_support
 
@@ -166,15 +166,15 @@
                     sg = selCond.copy()
                     sg.add_selector(sCurr)
                 else:
                     sg = Pattern([sCurr])
                 r= self._checkRel(self._k_subgroups, cCurrPos, cCurrNeg,quality,sg)
                 # If the subgroup is relevant, we add it to the list of k-subgroups
                 if r:
-                                        # (quality, subgroup, bits, optimistic_estimate,(tp,fp))
+                    # (quality, subgroup, bits, optimistic_estimate, (tp,fp))
                     self._k_subgroups.append((quality, sg, cCurrPos + cCurrNeg,oe,(tp,fp)))
                     self._k_subgroups = sorted(self._k_subgroups, reverse=False, key=lambda x: x[0])
                     # Check if the subgroups in k_subgroups are still relevant
                     self._checkRelevancies(cCurrPos, cCurrNeg, sg)
                     # If k_subgroups is full, remove the subgroup with the lowest quality
                     if len(self._k_subgroups) > self.num_subgroups:
                         # Remove lowest quality subgroup
```

### Comparing `subgroups-0.1.6/src/subgroups/algorithms/subgroup_sets/cbsd.py` & `subgroups-0.1.7/src/subgroups/algorithms/subgroup_sets/cbsd.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                     sg = selCond.copy()
                     sg.add_selector(sCurr)
                 else:
                     sg = Pattern([sCurr])
                 r= self._checkRel(self._k_subgroups, cCurrPos, cCurrNeg,quality,sg)
                 # If the subgroup is relevant, we add it to the list of k-subgroups
                 if r:
-                                        # (quality, subgroup, bits, optimistic_estimate,(tp,fp))
+                    # (quality, subgroup, bits, optimistic_estimate, (tp,fp))
                     self._k_subgroups.append((quality, sg, cCurrPos + cCurrNeg,oe,(tp,fp)))
                     self._k_subgroups = sorted(self._k_subgroups, reverse=False, key=lambda x: x[0])
                     # Check if the subgroups in k_subgroups are still relevant
                     self._checkRelevancies(cCurrPos + cCurrNeg, sg,quality)
                     if len(self._k_subgroups) > self.num_subgroups:
                         #Remove lowest quality subgroup
                         self._k_subgroups.pop(0)
@@ -64,14 +64,15 @@
                 self._unselected_subgroups += 1
         else:
             self._unselected_subgroups +=1
         return CcondPos,CcondNeg,newSelRel
 
     def _checkRelevancies(self,bits : bitarray,sg : Pattern,quality : float) -> None:
         """Internal method to check relevacies in _k_subgroups.
+        
         :param bits: bitarray of positive and negative instances
         :param sg: Pattern that represents a subgroup
         :param quality: sg quality
         """
         if type(quality) is not float:
             raise TypeError("Parameter 'quality' must be a float.")
         if type(bits) is not bitarray:
```

### Comparing `subgroups-0.1.6/src/subgroups/algorithms/subgroup_sets/cpbsd.py` & `subgroups-0.1.7/src/subgroups/algorithms/subgroup_sets/cpbsd.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                     sg = selCond.copy()
                     sg.add_selector(sCurr)
                 else:
                     sg = Pattern([sCurr])
                 r= self._checkRel(self._k_subgroups, cCurrPos,quality,sg)
                 # If the subgroup is relevant, we add it to the list of k-subgroups
                 if r:
-                                        # (quality, subgroup, bits, optimistic_estimate,(tp,fp))
+                    # (quality, subgroup, bits, optimistic_estimate, (tp,fp))
                     self._k_subgroups.append((quality, sg, cCurrPos + cCurrNeg,oe,(tp,fp)))
                     self._k_subgroups = sorted(self._k_subgroups, reverse=False, key=lambda x: x[0])
                     # Check if the subgroups in k_subgroups are still relevant
                     self._checkRelevancies(cCurrPos, sg,quality)
                     # If k_subgroups is full, remove the subgroup with the lowest quality
                     if len(self._k_subgroups) > self.num_subgroups:
                         # Remove lowest quality subgroup
```

### Comparing `subgroups-0.1.6/src/subgroups/algorithms/subgroup_sets/qfinder.py` & `subgroups-0.1.7/src/subgroups/algorithms/subgroup_sets/qfinder.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from pandas.api.types import is_string_dtype
 from subgroups.algorithms.algorithm import Algorithm
 from subgroups.exceptions import DatasetAttributeTypeError
 from subgroups.core.pattern import Pattern
 from subgroups.core.operator import Operator
 from subgroups.core.selector import Selector
 from subgroups.core.subgroup import Subgroup
-from bitarray import bitarray
 from subgroups.data_structures.bitset_qfinder import Bitset_QFinder
 import operator
 
 class QFinder(Algorithm):
     """This class represents the QFinder algorithm.
 
     :param cats: the number of maximum values for each column. If there is more values, we take the most frequent ones. If this value is -1, we take all the values.
@@ -28,36 +27,34 @@
     :param coverage_thld: the minimum coverage threshold.
     :param or_thld: the minimum odds ratio and adjusted odds ratio threshold.
     :param p_val_thld: the maximum p-value threshold. This threshold is used for p-values corrected for confounders and adjusted p-values.
     :param abs_contribution_thld: the minimum absolute contribution threshold.
     :param contribution_thld: the minimum contribution ratio threshold.
     :param write_results_in_file: if True, the results will be written in a file.
     :param file_path: the path of the file where the results will be written.
-    :param write_stats_in_file: if True, the statistics will be written in a HTML file.
-    :param stats_path: the path of the file where the statistics will be written.
     :param delta: minimum delta to consider that a subgroup has a higher effect size.
     :param num_subgroups: the number of top subgroups to return.
     """
 
-    __slots__ = ('_num_subgroups','_cats', '_max_complexity', '_thresholds','_credibility_values' , '_file', '_file_path', '_stats_path' , '_df','_delta', '_num_subgroups', '_top_patterns', '_candidate_patterns')
+    __slots__ = ('_num_subgroups','_cats', '_max_complexity', '_thresholds','_credibility_values' , '_file', '_file_path' , '_df','_delta', '_num_subgroups', '_top_patterns', '_candidate_patterns')
 
-    # A credibility criterion is a credibility measure and a threhosld. Here we set if the credibility measure value
+    # A credibility criterion is a credibility measure and a threshold. Here we set if the credibility measure value
     # should be greater or equal than the threshold or less or equal than the threshold.
     _credibility_criterions = {
         "coverage" :  operator.ge,
         "odds_ratio" : operator.ge,
         "p_value" : operator.le,
         "absolute_contribution" : operator.ge,
         "contribution_ratio" : operator.le,
         # "adjusted_odds_ratio" : operator.ge,
         # "corrected_p_value" : operator.le,
         "adjusted_p_value" : operator.le
     }
 
-    def __init__(self, num_subgroups :int, cats : int = -1, max_complexity: int = -1, coverage_thld: float = 0.1, or_thld: float = 1.2, p_val_thld: float = 0.05, abs_contribution_thld: float = 0.2, contribution_thld: float = 5, delta :float = 0.2, write_results_in_file: bool = False, file_path: Union[str,None] = None, write_stats_in_file: bool = False, stats_path: Union[str,None] = None) -> None:
+    def __init__(self, num_subgroups :int, cats : int = -1, max_complexity: int = -1, coverage_thld: float = 0.1, or_thld: float = 1.2, p_val_thld: float = 0.05, abs_contribution_thld: float = 0.2, contribution_thld: float = 5, delta :float = 0.2, write_results_in_file: bool = False, file_path: Union[str,None] = None) -> None:
         if type(num_subgroups) is not int:
             raise TypeError("The type of the parameter 'num_subgroups' must be 'int'.")
         if type(cats) is not int:
             raise TypeError("The type of the parameter 'cats' must be 'int'.")
         if type(max_complexity) is not int:
             raise TypeError("The type of the parameter 'max_complexity' must be 'int'.")
         if type(coverage_thld) is not float and type(coverage_thld) is not int:
@@ -84,30 +81,23 @@
         if (abs_contribution_thld < 0 or abs_contribution_thld > 1):
             raise ValueError("The parameter 'abs_contribution_thld' must be between 0 and 1.")
         if (contribution_thld < 0):
             raise ValueError("The parameter 'contribution_thld' must be greater than or equal to 0.")
         # If 'write_results_in_file' is True, 'file_path' must not be None.
         if (write_results_in_file) and (file_path is None):
             raise ValueError("If the parameter 'write_results_in_file' is True, the parameter 'file_path' must not be None.")
-        # If 'write_stats_in_file' is True, 'stats_path' must not be None.
-        if (write_stats_in_file) and (stats_path is None):
-            raise ValueError("If the parameter 'write_stats_in_file' is True, the parameter 'stats_path' must not be None.")
         self._num_subgroups = num_subgroups
         self._cats = cats
         self._max_complexity = max_complexity
         self._delta = delta
         if (write_results_in_file):
             self._file_path = file_path
         else:
             self._file_path = None
         self._file = None
-        if (write_stats_in_file):
-            self._stats_path = stats_path
-        else:
-            self._stats_path = None
         self._top_patterns = []
         self._candidate_patterns = []
         # Thresholds for each credibility measure.
         self._thresholds = {
             "coverage" : coverage_thld,
             "odds_ratio" : or_thld,
             "p_value" : p_val_thld,
@@ -131,85 +121,79 @@
         return self._top_patterns
     
     selected_subgroups = property(_get_selected_subgrouops, None, None, "The number of selected subgroups.")
     unselected_subgroups = property(_get_unselected_subgroups, None, None, "The number of unselected subgroups.")
     visited_subgroups = property(_get_visited_subgroups, None, None, "The number of visited subgroups.")
     top_patterns = property(_get_top_patterns, None, None, "The list of the selected patterns.")
 
-    def _generate_candidate_patterns(self,df : DataFrame, tuple_target_attribute_value: tuple, max_complexity : int ,cats : int = -1) -> list[Pattern]:
-        """Method to generate the set of candidate patterns for the QFinder algorithm.
+    def _generate_candidate_patterns(self,df : DataFrame, tuple_target_attribute_value: tuple) -> list[Pattern]:
+            """Method to generate the set of candidate patterns for the QFinder algorithm.
 
-        :param df: the dataset.
-        :param tuple_as_target: the tuple which contains the target attribute name and the target attribute values.
-        :param max_complexity: the maximum length of the patterns.
-        :param cats: the number of maximum values for each column. If there is more values, we take the most frequent ones. If this value is -1, we take all the values.
-        :return: the set of candidate patterns.
-        """
-        if type(df) is not DataFrame:
-            raise TypeError("The type of the parameter 'df' must be 'DataFrame'.")
-        if type(tuple_target_attribute_value) is not tuple:
-            raise TypeError("The type of the parameter 'tuple_as_target' must be 'tuple'.")
-        if type(cats) is not int:
-            raise TypeError("The type of the parameter 'cats' must be 'int'.")
-        if type(max_complexity) is not int:
-            raise TypeError("The type of the parameter 'max_complexity' must be 'int'.")
-        if (len(tuple_target_attribute_value) != 2):
-            raise ValueError("The parameter 'tuple_as_target' must contain two elements.")
-        if (not is_string_dtype(df[tuple_target_attribute_value[0]])):
-            raise DatasetAttributeTypeError("The attribute '{}' must be a string.".format(tuple_target_attribute_value[0]))
-        # We do not generate patterns with the target attribute.
-        df_without_target = df.drop(columns=[tuple_target_attribute_value[0]])
-        # We generate the list of candidate simple patterns (length 1).
-        simple_patterns = []
-        for column in df_without_target:
-            # Number of different values for the current column.
-            n_values = len(df_without_target[column].unique())
-            # If we don't have to limit the number of values, we take all of them.
-            if (n_values <= cats or cats == -1):
-                for value in df_without_target[column].unique():
-                    # We will save each selector (column = value) as a pattern.
-                    simple_patterns.append(Pattern([Selector(column, Operator.EQUAL, value)]))
-            # If we have to limit the number of values, we take the cats-1 most frequent ones and the rest of them are grouped in the "other" value.
-            else:
-                value_counts = df_without_target[column].value_counts()
-                # If the "other" value is already in the dataset, we need to make sure that the added value is different.
-                other = "other"
-                while other in value_counts.index:
-                    other += "_"
-                # Most frequent values.
-                top_values = value_counts.nlargest(cats-1).index
-                # Least frequent values. These values will be grouped in the "other" value.
-                other_values = value_counts.nsmallest(n_values - cats + 1).index
-                for value in top_values:
-                    simple_patterns.append(Pattern([Selector(column, Operator.EQUAL, value)]))
-                # We edit our copy of the dataset to set the "other" value to the rows which have a value that is not in the top_values.
-                df_without_target.loc[df_without_target[column].isin(other_values), column] = other
-                simple_patterns.append(Pattern([Selector(column, Operator.EQUAL, other)]))
-        complex_patterns = []
-        if (max_complexity == -1):
-            max_complexity = len(df_without_target.columns)
-        # We generate the list of candidate patterns by combining the simple patterns.
-        for L in range(2, max_complexity+1):
-            # We take each combination of L simple patterns.
-            for subset in itertools.combinations(simple_patterns, L):
-                column_values = [ s.get_selector(0).attribute_name for s in subset ]
-                # If we are taking twice the same column, the pattern is not valid.
-                if (len(column_values) != len(set(column_values))):
-                    continue
-                pattern = Pattern([])
-                for s in subset:
-                    pattern.add_selector(s.get_selector(0))
-                complex_patterns.append(pattern)
-        # The list of candidate patterns is the union of the list of simple patterns and the list of complex patterns.
-        return simple_patterns + complex_patterns
-
-    def _handle_individual_result(self,credibility: bitarray) -> int:
+            :param df: the dataset.
+            :param tuple_as_target: the tuple which contains the target attribute name and the target attribute values.
+            :return: the set of candidate patterns.
+            """
+            if type(df) is not DataFrame:
+                raise TypeError("The type of the parameter 'df' must be 'DataFrame'.")
+            if type(tuple_target_attribute_value) is not tuple:
+                raise TypeError("The type of the parameter 'tuple_as_target' must be 'tuple'.")
+            if (len(tuple_target_attribute_value) != 2):
+                raise ValueError("The parameter 'tuple_as_target' must contain two elements.")
+            if (not is_string_dtype(df[tuple_target_attribute_value[0]])):
+                raise DatasetAttributeTypeError("The attribute '{}' must be a string.".format(tuple_target_attribute_value[0]))
+            # We do not generate patterns with the target attribute.
+            df_without_target = df.drop(columns=[tuple_target_attribute_value[0]])
+            # We generate the list of candidate simple patterns (length 1).
+            simple_patterns = []
+            for column in df_without_target:
+                # Number of different values for the current column.
+                n_values = len(df_without_target[column].unique())
+                # If we don't have to limit the number of values, we take all of them.
+                if (n_values <= self._cats or self._cats == -1):
+                    for value in df_without_target[column].unique():
+                        # We will save each selector (column = value) as a pattern.
+                        simple_patterns.append(Pattern([Selector(column, Operator.EQUAL, value)]))
+                # If we have to limit the number of values, we take the self._cats-1 most frequent ones and the rest of them are grouped in the "other" value.
+                else:
+                    value_counts = df_without_target[column].value_counts()
+                    # If the "other" value is already in the dataset, we need to make sure that the added value is different.
+                    other = "other"
+                    while other in value_counts.index:
+                        other += "_"
+                    # Most frequent values.
+                    top_values = value_counts.nlargest(self._cats-1).index
+                    # Least frequent values. These values will be grouped in the "other" value.
+                    other_values = value_counts.nsmallest(n_values - self._cats + 1).index
+                    for value in top_values:
+                        simple_patterns.append(Pattern([Selector(column, Operator.EQUAL, value)]))
+                    # We edit our copy of the dataset to set the "other" value to the rows which have a value that is not in the top_values.
+                    df_without_target.loc[df_without_target[column].isin(other_values), column] = other
+                    simple_patterns.append(Pattern([Selector(column, Operator.EQUAL, other)]))
+            complex_patterns = []
+            if (self._max_complexity == -1):
+                self._max_complexity = len(df_without_target.columns)
+            # We generate the list of candidate patterns by combining the simple patterns.
+            for L in range(2, self._max_complexity+1):
+                # We take each combination of L simple patterns.
+                for subset in itertools.combinations(simple_patterns, L):
+                    column_values = [ s.get_selector(0).attribute_name for s in subset ]
+                    # If we are taking twice the same column, the pattern is not valid.
+                    if (len(column_values) != len(set(column_values))):
+                        continue
+                    pattern = Pattern([])
+                    for s in subset:
+                        pattern.add_selector(s.get_selector(0))
+                    complex_patterns.append(pattern)
+            # The list of candidate patterns is the union of the list of simple patterns and the list of complex patterns.
+            return simple_patterns + complex_patterns
+    
+    def _handle_individual_result(self,credibility: list[bool]) -> int:
         """Method to compute the rank of a pattern.
 
-        :param credibility: the bitarray representing the pattern's credibility.
+        :param credibility: the list of booleans representing the pattern's credibility.
         :return: the rank of the pattern.
         """
         rank = 0
         # Since most of the ranks are achieved only if the previous ones are also achieved, we can stop the loop when we find the first rank that is not achieved.
         # This won't work for the fifth rank, since it only requieres that either the third or the fourth rank are achieved (and its own criterion).
         for i in range(len(credibility)):
             # The fifth rank consists in subgroups of rank 3 OR 4 that also satisfy the fifth criterion, so we do not exit the loop if the fourth criterion is not satisfied.
@@ -235,23 +219,25 @@
         :return: the list of candidate patterns sorted by their rank.
         """
         # We first sort the patterns by their p_value. This sorting will be used in case of ties in the ranking.
         sorted_patterns = sorted(self._candidate_patterns, key=lambda pattern: self._credibility_values["p_value"][str(pattern)])
         ranks = []
         for pattern in sorted_patterns:
             # We compute the credibility of each pattern. The credibility of a pattern is a list of booleans, where each boolean represents a criterion.
-            credibility = bitarray()
+            credibility = []
             for cred in QFinder._credibility_criterions:
                 credibility.append(QFinder._credibility_criterions[cred](self._credibility_values[cred][str(pattern)],self._thresholds[cred]))
             # We compute the rank of the pattern.
             rank = self._handle_individual_result(credibility)
             ranks.append(rank)
+        sorted_patterns_ranks = list(zip(sorted_patterns,ranks))
         # We sort the patterns according to their ranks.
         # If two patterns have the same rank, we sort them according to their appearance in sorted_patterns (i.e. according to their p-values).
-        ranked_patterns = sorted(sorted_patterns, key=lambda pattern: ranks[sorted_patterns.index(pattern)], reverse=True)
+        sorted_patterns_ranks.sort(key = lambda x:x[1], reverse = True)
+        ranked_patterns = list(map(lambda x:x[0],sorted_patterns_ranks))
         return ranked_patterns
 
     def _select_top_k(self, ranked_patterns) -> list[Pattern]:
         """Method to select the top-k patterns according to the ranking and the redundancy criterion.
 
         :param ranked_patterns: the list of candidate patterns sorted by their rank.
         :return: the list of top-k patterns.
@@ -286,115 +272,79 @@
                                 self._credibility_values["p_value"][str(pattern)] < self._credibility_values["p_value"][str(top_pattern)]:
                             top_k_patterns.remove(top_pattern)
                     top_k_patterns.append(pattern)
                     # If |top_k_patterns| > k, we remove the pattern with the highest p-value.
                     if len(top_k_patterns) > self._num_subgroups:
                         max_p_val_pattern = max(top_k_patterns, key=lambda pattern: self._credibility_values["p_value"][str(pattern)])
                         top_k_patterns.remove(max_p_val_pattern)
-                    continue
-                # If we did break the first top_pattern in top_patterns loop, we continue to the next pattern.
-                break
         return top_k_patterns
     
     def fit(self, pandas_dataframe: DataFrame, tuple_target_attribute_value: tuple) -> None:
         """Main method to run the QFinder algorithm. This algorithm only supports nominal attributes (i.e., type 'str'). IMPORTANT: missing values are not supported yet.
         
         :param data: the DataFrame which is scanned. This algorithm only supports nominal attributes (i.e., type 'str'). IMPORTANT: missing values are not supported yet.
         :param target: a tuple with 2 elements: the target attribute name and the target value.
         """
-        if type(pandas_dataframe) != DataFrame:
+        if type(pandas_dataframe) is not DataFrame:
             raise TypeError("The dataset must be a pandas DataFrame.")
-        if type(tuple_target_attribute_value) != tuple:
+        if type(tuple_target_attribute_value) is not tuple:
             raise TypeError("The target must be a tuple.")
         for column in pandas_dataframe.columns:
             if not is_string_dtype(pandas_dataframe[column]):
                 raise DatasetAttributeTypeError("Error in attribute '" + str(column) + "'. This algorithm only supports nominal attributes (i.e., type 'str').")
         # We copy the DataFrame to avoid modifying the original when dealing with "other" values.
         df = pandas_dataframe.copy()
         # We generate the list of candidate patterns.
-        self._candidate_patterns = self._generate_candidate_patterns(df, tuple_target_attribute_value, self._max_complexity, self._cats)
+        self._candidate_patterns = self._generate_candidate_patterns(df, tuple_target_attribute_value)
         # We compute the credibility measures for each candidate pattern using the bitset structure.
         qfinder_bitset = Bitset_QFinder()
         qfinder_bitset.generate_bitset(df, tuple_target_attribute_value, self._candidate_patterns)
         self._candidate_patterns = qfinder_bitset.get_non_empty_patterns()
-        coverages, odds_ratios, p_values, absolute_contributions, contribution_ratios, adjusted_p_values \
-            = qfinder_bitset.compute_credibility_measures(df[tuple_target_attribute_value[0]] == tuple_target_attribute_value[1])
-        self._credibility_values = {
-            "coverage": coverages,
-            "odds_ratio": odds_ratios,
-            "p_value": p_values,
-            "absolute_contribution": absolute_contributions,
-            "contribution_ratio": contribution_ratios,
-            # "adjusted_odds_ratio": adjusted_odds_ratios,
-            # "corrected_p_value": corrected_p_values,
-            "adjusted_p_value": adjusted_p_values
-        }
+        self._credibility_values = qfinder_bitset.compute_credibility_measures(df[tuple_target_attribute_value[0]] == tuple_target_attribute_value[1])
         ranked_patterns = self._rank_patterns()
         self._top_patterns = self._select_top_k(ranked_patterns)
         if self._file_path is not None:
             self._to_file(self._file_path,tuple_target_attribute_value, self._credibility_values)
-        if self._stats_path is not None:
-            self._to_stats_file()
 
     def test_subgroups(self,test_dataframe : DataFrame, tuple_target_attribute_value: tuple, write_to_file:bool=False, file_path: Union[str,None]=None):
         """Method to test the best subgroups on a different dataset. This method can only be called after the fit method.
         
         :param test_dataframe: the DataFrame which is scanned. This algorithm only supports nominal attributes (i.e., type 'str'). IMPORTANT: missing values are not supported yet.
         :param target: a tuple with 2 elements: the target attribute name and the target value.
         :return: a dictionary with the credibility measures for each subgroup.
         """
         # We make sure that the fit method has been called before.
         if self._top_patterns is None:
             raise ValueError("The fit method must be called before testing subgroups.")
-        if type(test_dataframe) != DataFrame:
+        if type(test_dataframe) is not DataFrame:
             raise TypeError("The dataset must be a pandas DataFrame.")
-        if type(tuple_target_attribute_value) != tuple:
+        if type(tuple_target_attribute_value) is not tuple:
             raise TypeError("The target must be a tuple.")
-        if type(write_to_file) != bool:
+        if type(write_to_file) is not bool:
             raise TypeError("The write_to_file parameter must be a boolean.")
         # If wirte_to_file is True, file_path must not be None.
         if write_to_file and file_path is None:
             raise ValueError("The file path must be specified.")
-        elif write_to_file and type(file_path) != str:
+        elif write_to_file and type(file_path) is not str:
             raise TypeError("The file path must be a string.")
         # We generate a different bitset for the test dataset, which whill be used to compute the credibility measures.
         qfinder_bitset = Bitset_QFinder()
         qfinder_bitset.generate_bitset(test_dataframe, tuple_target_attribute_value, self._top_patterns)
-        coverages, odds_ratios, p_values, absolute_contributions, contribution_ratios, adjusted_p_values \
-            = qfinder_bitset.compute_credibility_measures(test_dataframe[tuple_target_attribute_value[0]] == tuple_target_attribute_value[1])
-        parameters = {
-            "coverages": coverages,
-            "odds_ratios": odds_ratios,
-            "p_values": p_values,
-            "absolute_contributions": absolute_contributions,
-            "contribution_ratios": contribution_ratios,
-            "adjusted_p_values": adjusted_p_values
-        }
+        credibility_values = qfinder_bitset.compute_credibility_measures(test_dataframe[tuple_target_attribute_value[0]] == tuple_target_attribute_value[1])
         if write_to_file:
-            self._to_file(file_path, tuple_target_attribute_value, parameters)
-        return parameters
+            self._to_file(file_path, tuple_target_attribute_value, credibility_values)
+        return credibility_values
     
     def _to_file(self, file_path, target, credibility_values):
         """Writes the top-k patterns to a file.
 
         :param target: a tuple with 2 elements: the target attribute name and the target value.
         """
         self._file = open(file_path, "w")
         for pat in self._top_patterns:
             subgroup = Subgroup(pat, Selector(target[0], Operator.EQUAL, target[1]))
             self._file.write(str(subgroup) + " ; ")
             for cred in credibility_values:
                 self._file.write(cred + ": " + str(credibility_values[cred][str(pat)]) + " ; ")
             self._file.write("\n")
         self._file.close()
-        self._file = None
-
-    def _to_stats_file(self):
-        """Write the credibility measures of each pattern to a file.
-        """
-        data = {
-                cred : list(self._credibility_values[cred].values()) for cred in self._credibility_values
-            }
-        df = DataFrame(data)
-        # Set the row names to be the patterns.
-        df.index = list(self._credibility_values["odds_ratio"].keys())
-        df.to_html(self._stats_path)
+        self._file = None
```

### Comparing `subgroups-0.1.6/src/subgroups/algorithms/subgroup_sets/sdmap.py` & `subgroups-0.1.7/src/subgroups/algorithms/subgroup_sets/sdmap.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/algorithms/subgroup_sets/sdmapstar.py` & `subgroups-0.1.7/src/subgroups/algorithms/subgroup_sets/sdmapstar.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,15 +319,14 @@
                 else:
                     # Call conditionalFPTree wihtout prune
                     conditional_fptree = fptree.generate_conditional_fp_tree(beta_as_list, minimum_tp=self.minimum_tp, minimum_fp=self.minimum_fp, minimum_n=self.minimum_n)
                 # Recursive call.
                 if not conditional_fptree.is_empty():
                     self._fpgrowth(conditional_fptree, beta_as_list, target, TP, FP)
 
-                    
     def _updateKSubgroups(self,tp:int,fp:int,TP:int,FP:int) -> None:
         """Internal method to update and sort k subgroups.
 
         :param tp: true positives
         :param fp: false positives
         """
         if (type(tp) is not int):
```

### Comparing `subgroups-0.1.6/src/subgroups/algorithms/subgroup_sets/vlsd.py` & `subgroups-0.1.7/src/subgroups/algorithms/subgroup_sets/vlsd.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/core/operator.py` & `subgroups-0.1.7/src/subgroups/core/operator.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from subgroups.exceptions import OperatorNotSupportedError
 from pandas import Series
 
 # Python annotations.
 from typing import Union
 
 class Operator(Enum):
-    
     """This enumerator provides the available operators which can be used by the selectors.
     """
     
     EQUAL = 1
     NOT_EQUAL = 2
     LESS = 3
     GREATER = 4
```

### Comparing `subgroups-0.1.6/src/subgroups/core/pattern.py` & `subgroups-0.1.7/src/subgroups/core/pattern.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/core/selector.py` & `subgroups-0.1.7/src/subgroups/core/selector.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/core/subgroup.py` & `subgroups-0.1.7/src/subgroups/core/subgroup.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/data_structures/__init__.py` & `subgroups-0.1.7/src/subgroups/data_structures/__init__.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/data_structures/bitset_bsd.py` & `subgroups-0.1.7/src/subgroups/data_structures/bitset_bsd.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,64 +3,57 @@
 # Contributors:
 #    Paco Mora Caselles <pacomoracaselles@gmail.com>
 
 """This file contains the implementation of the Bitset data structure used in the BSD algorithm and its variants.
 """
 
 from pandas import DataFrame
-
-# Python annotations.
-from typing import Union
 from subgroups.core.operator import Operator
-
 from subgroups.core.selector import Selector
 from subgroups.core.pattern import Pattern
 from bitarray import bitarray
 
 class BitsetDictionary(dict):
-    """ Internal class to implement the dicttionaries used in the bitset. This dictionary only allows to insert a Pattern or a Selector as key.
-    If a Selector is inserted, it is converted to a Pattern. Each entry must store a bitarray.
+    """ Internal class to implement the dicttionaries used in the bitset. This dictionary only allows to insert a Pattern or a Selector as key. If a Selector is inserted, it is converted to a Pattern. Each entry must store a bitarray.
     """
 
     __slots__ = ()
 
     def __iter__(self):
         for key in super().__iter__():
             yield Pattern.generate_from_str(key)
 
     def __setitem__(self, key, value) -> None:
         if (type(value) != bitarray):
             raise TypeError("The value must be a bitarray.")
-        if (type(key)==Selector):
+        if (type(key) is Selector):
             super().__setitem__(str(Pattern([key])),value)
-        elif (type(key)==Pattern):
+        elif (type(key) is Pattern):
             super().__setitem__(str(key), value)
         else:
             raise TypeError("The key must be a Selector or a Pattern.")
     
     def __getitem__(self, key) -> bitarray:
-        if (type(key)==Selector):
+        if (type(key) is Selector):
             return super().__getitem__(str(Pattern([key])))
-        elif (type(key)==Pattern):
+        elif (type(key) is Pattern):
             return super().__getitem__(str(key))
         else:
             raise TypeError("The key must be a Selector or a Pattern.")
     
     def __contains__(self, __o: object) -> bool:
-        if (type(__o)==Selector):
+        if (type(__o) is Selector):
             return super().__contains__(str(Pattern([__o])))
-        elif (type(__o)==Pattern):
+        elif (type(__o) is Pattern):
             return super().__contains__(str(__o))
         else:
             raise TypeError("The key must be a Selector or a Pattern.")
 
-
 class BitsetBSD(object):
     """This class represents a bitset used in the BSD algorithm and its variants.
-
     """
 
     __slots__ = ("_bitset_pos", "_bitset_neg")
 
     def __init__(self):
         """Method to initialize an object of type 'BitsetBSD'.
         """
@@ -96,15 +89,14 @@
         :param bitset_neg: the bitset_neg dictionary.
         """
         self._bitset_neg = bitset_neg
     
     bitset_pos = property(_get_bitset_pos, _set_bitset_pos, None, "The bitset dictionary for rows that match the target value.")
     bitset_neg = property(_get_bitset_neg, _set_bitset_neg, None, "The bitset dictionary for rows that do not match the target value.")
 
-
     def build_bitset(self, pandas_dataframe :DataFrame,set_of_frequent_selectors:list, tuple_target_attribute_value : tuple) -> None:
         """Method to build the complete tree from the root node using a set of frequent selectors.
 
         :param pandas_dataframe: Input dataset. It is VERY IMPORTANT to respect the following conditions:
           (1) the dataset must be a pandas dataframe,
           (2) the dataset must not contain missing values,
           (3) for each attribute, all its values must be of the same type.
@@ -121,15 +113,14 @@
             raise TypeError("Parameter 'set_of_frequent_selectors' must be a list.")
         if (type(tuple_target_attribute_value) is not tuple):
             raise TypeError("Parameter 'tuple_target_attribute_value' must be a tuple.")
         if (len(tuple_target_attribute_value) != 2):
             raise ValueError("Parameter 'tuple_target_attribute_value' must be of length 2.")
         if type(tuple_target_attribute_value[0]) is not str:
             raise ValueError("The name of the target attribute (first element in parameter 'tuple_target_attribute_value') must be a string.")
-
         # Initialize an empty list for selectors
         selectors = []
         # Get the columns of the dataset without the target column
         columns_without_target = pandas_dataframe.columns[pandas_dataframe.columns != tuple_target_attribute_value[0]]
         # Check that each column contains only string values
         for column in columns_without_target:
             # If the column contains only string values
@@ -148,15 +139,14 @@
             ba_pos = bitarray((df_pos[selector[0]] == selector[1]).tolist())
             # Create a bitarray from the boolean array that indicates whether the negative examples match the selector
             ba_neg = bitarray((df_neg[selector[0]] == selector[1]).tolist())
             # Add the bitarrays to the corresponding bitset dictionaries with the selector as key
             self._bitset_pos[Selector(selector[0],Operator.EQUAL, selector[1])] = ba_pos
             self._bitset_neg[Selector(selector[0],Operator.EQUAL, selector[1])] = ba_neg
 
-
     def generate_set_of_frequent_selectors(self, pandas_dataframe, tuple_target_attribute_value, min_support):
         """Method to scan the dataset (ONLY DISCRETE/NOMINAL ATTRIBUTES) and collect the sorted set of frequent selectors (L).
 
         :type pandas_dataframe: pandas.DataFrame
         :param pandas_dataframe: Input dataset. It is VERY IMPORTANT to respect the following conditions:
           (1) the dataset must be a pandas dataframe,
           (2) the dataset must not contain missing values,
```

### Comparing `subgroups-0.1.6/src/subgroups/data_structures/bitset_qfinder.py` & `subgroups-0.1.7/src/subgroups/data_structures/bitset_qfinder.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,109 +2,77 @@
 
 # Contributors:
 #    Paco Mora Caselles <pacomoracaselles@gmail.com>
 
 """This file contains the implementation of the Bitset data structure used in the QFinder to create the regression models.
 """
 
-from pandas import DataFrame, Series
-
-# Python annotations.
-from typing import Union
-from subgroups.core.operator import Operator
+from pandas import DataFrame
 import statsmodels.api as sm
 import numpy as np
-
-from subgroups.core.selector import Selector
 from subgroups.core.pattern import Pattern
 
 class Bitset_QFinder(object):
-    
-    """
-    This class represents a bitset used in the QFinder algorithm.
+    """This class represents a bitset used in the QFinder algorithm.
     """
-
-
     __slots__ = ["_df","_TP", "_FP"]
 
-
-
     def __init__(self):
         self._df = DataFrame()
 
-
-
-
     def generate_bitset(self, df : DataFrame, tuple_target_attribute_value: tuple, list_of_candidate_patterns: list[Pattern]) -> None:
-        """
-        This method generates a bitset from a dataset and a list of candidate patterns.
-        Each column of the bitset represents a candidate pattern and each row represents an instance of the dataset.
-        The value of each cell is True if the corresponding pattern appears in the corresponding instance and False otherwise.
+        """This method generates a bitset from a dataset and a list of candidate patterns. Each column of the bitset represents a candidate pattern and each row represents an instance of the dataset. The value of each cell is True if the corresponding pattern appears in the corresponding instance and False otherwise.
 
         :param df: dataset from which the bitset is generated.
         :param tuple_target_attribute_value: tuple which contains the name of the target attribute and its value.
         :param list_of_candidate_patterns: list of candidate patterns.
-
-        
         """
         self._TP = len(df[df[tuple_target_attribute_value[0]] == tuple_target_attribute_value[1]])
         self._FP = len(df) - self._TP
-        
         df_without_target = df.drop(columns=[tuple_target_attribute_value[0]])
-        
         pattern_matches = {}
         for pattern in list_of_candidate_patterns:
             entry = None
             for selector in pattern:
                 if entry is None:
                     entry = df_without_target[selector.attribute_name] == selector.value
                 else:
                     entry = entry & (df_without_target[selector.attribute_name] == selector.value)
             # If the pattern is empty (it does not appear in the dataset), we do not add it to the bitset.
             if entry.sum() != 0:
                 pattern_matches[str(pattern)] = entry
         self._df = DataFrame(pattern_matches)
 
-
     def get_non_empty_patterns(self) -> list[Pattern]:
-        """
-            Method to get the candidate patterns after removing those that do not appear in the dataset.
+        """Method to get the candidate patterns after removing those that do not appear in the dataset.
         """
         return [Pattern.generate_from_str(pattern_as_str) for pattern_as_str in self._df.columns]
 
-    
-    def compute_credibility_measures(self, target_column) -> tuple[dict, dict, dict, dict, dict, dict]:
-
-        """
-            Method to compute the credibility measures for each candidate pattern.
+    def compute_credibility_measures(self, target_column) -> DataFrame:
+        """Method to compute the credibility measures for each candidate pattern.
             
             :param target_column: target column of the dataset.
-            :return: a tuple with dictionaries with the credibility values for each candidate pattern.
-
+            :return: a pandas DataFrame with the credibility values for each candidate pattern.
         """
-
         # WARNING: Corrected measures for confounders are not implemented yet
         # We create the global model for corrected and adjusted credibility measures
         # results = sm.Logit(target_column, self._df).fit(method='nm')
         # adjusted_odds_ratios = results.params.apply(np.exp).to_dict()
         # corrected_p_values = results.pvalues.to_dict()
-        
         odds_ratios = {}
         p_values = {}
         coverages = {}
         absolute_contributions = {}
         contribution_ratios = {}
-
         # We create models to calculate the odds ratios and p-values for each pattern
         for pattern in self._df.columns:
             results = sm.GLM(target_column, self._df[pattern], family=sm.families.Binomial()).fit()
-            odds_ratios[pattern] = np.exp(results.params[0])
-            p_values[pattern] = results.pvalues[0]
+            odds_ratios[pattern] = np.exp(results.params.iloc[0])
+            p_values[pattern] = results.pvalues.iloc[0]
             coverages[pattern] = len(self._df[self._df[pattern]])/(self._TP + self._FP)
-
         # We calculate the absolute contribution and the contribution ratio for each pattern
         for pattern_as_str in self._df.columns:
             minimum_absolute_contribution = 1
             maximum_absolute_contribution = 0
             odds_ratio = odds_ratios[pattern_as_str]
             pattern = Pattern.generate_from_str(pattern_as_str)
             if len(pattern) == 1:
@@ -118,13 +86,10 @@
                     minimum_absolute_contribution = min(minimum_absolute_contribution, odds_ratio/pattern_without_selector_odds_ratio)
                     maximum_absolute_contribution = max(maximum_absolute_contribution, odds_ratio/pattern_without_selector_odds_ratio)
             absolute_contributions[pattern_as_str] = minimum_absolute_contribution
             if minimum_absolute_contribution == 0:
                 contribution_ratios[pattern_as_str] = np.inf
             else:
                 contribution_ratios[pattern_as_str] = maximum_absolute_contribution/minimum_absolute_contribution
-        
-
         # We use the Bonferroni correction for adjusted corrected p-values: each p_value is multiplied by the number of predictors
         adjusted_p_values = {pat : p_values[pat] * len(self._df.columns) for pat in p_values.keys()}
-
-        return coverages, odds_ratios, p_values, absolute_contributions, contribution_ratios, adjusted_p_values
+        return DataFrame({'coverage': coverages, 'odds_ratio': odds_ratios, 'p_value': p_values, 'absolute_contribution': absolute_contributions, 'contribution_ratio': contribution_ratios, 'adjusted_p_value': adjusted_p_values})
```

### Comparing `subgroups-0.1.6/src/subgroups/data_structures/fp_tree_for_sdmap.py` & `subgroups-0.1.7/src/subgroups/data_structures/fp_tree_for_sdmap.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 """This file contains the implementation of the FPTree data structure used in the SDMap algorithm.
 """
 
 from subgroups.data_structures.fp_tree_node import FPTreeNode
 from subgroups.core.selector import Selector
 from subgroups.core.operator import Operator
 from pandas import DataFrame
-from numpy import size, sum
 from subgroups.exceptions import InconsistentMethodParametersError
 
 # Python annotations.
 from typing import Union
 
 class FPTreeForSDMap(object):
     """This class represents the FPTree data structure used in the SDMap algorithm.
@@ -127,15 +126,15 @@
             # Result.
             final_dict_of_frequent_selectors = dict()
             # Iterate through the columns (except the target).
             insertion_order = 0 # The insertion order is necessary later in order to sort the elements which have the same 'n' in a same row.
             for column in pandas_dataframe.columns.drop(target[0]):
                 current_Series = pandas_dataframe[column]
                 # Use the 'groupby' method in order to obtain, for each value, the true positives tp and the false positives fp.
-                tp_and_fp_for_each_value = target_attribute_as_a_mask.groupby(current_Series).aggregate([size, sum]) # tp -> sum; fp -> size - sum; n -> size.
+                tp_and_fp_for_each_value = target_attribute_as_a_mask.groupby(current_Series).aggregate(["size", "sum"]) # tp -> sum; fp -> size - sum; n -> size.
                 # Filter the results according to 'minimum_tp' and 'minimum_fp'.
                 filtered = tp_and_fp_for_each_value[(tp_and_fp_for_each_value["sum"] >= minimum_tp) & ((tp_and_fp_for_each_value["size"] - tp_and_fp_for_each_value["sum"]) >= minimum_fp)]
                 # The corresponding values are the indexes of the DataFrame 'filtered'.
                 values = filtered.index
                 # We create the selectors and we add them to the final dictionary.
                 for i in values:
                     # IMPORTANT: we use 'repr' in order to add simple quotes to the values of type str, but not to the values of numeric types.
@@ -149,15 +148,15 @@
             # Result.
             final_dict_of_frequent_selectors = dict()
             # Iterate through the columns (except the target).
             insertion_order = 0 # The insertion order is necessary later in order to sort the elements which have the same 'n' in a same row.
             for column in pandas_dataframe.columns.drop(target[0]):
                 current_Series = pandas_dataframe[column]
                 # Use the 'groupby' method in order to obtain, for each value, the true positives tp and the false positives fp.
-                tp_and_fp_for_each_value = target_attribute_as_a_mask.groupby(current_Series).aggregate([size, sum]) # tp -> sum; fp -> size - sum; n -> size.
+                tp_and_fp_for_each_value = target_attribute_as_a_mask.groupby(current_Series).aggregate(["size", "sum"]) # tp -> sum; fp -> size - sum; n -> size.
                 # Filter the results according to 'minimum_tp' and 'minimum_fp'.
                 filtered = tp_and_fp_for_each_value[tp_and_fp_for_each_value["size"] >= minimum_n]
                 # The corresponding values are the indexes of the DataFrame 'filtered'.
                 values = filtered.index
                 # We create the selectors and we add them to the final dictionary.
                 for i in values:
                     # IMPORTANT: we use 'repr' in order to add simple quotes to the values of type str, but not to the values of numeric types.
```

### Comparing `subgroups-0.1.6/src/subgroups/data_structures/fp_tree_for_sdmapstar.py` & `subgroups-0.1.7/src/subgroups/data_structures/fp_tree_for_sdmapstar.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,34 +2,31 @@
 
 # Contributors:
 #    Paco Mora Caselles <pacomoracaselles@gmail.com>
 
 """This file contains the implementation of the FPTree data structure used in the SDMapStar algorithm.
 """
 
-from subgroups.data_structures.fp_tree_node import FPTreeNode
 from subgroups.core.selector import Selector
-from subgroups.core.operator import Operator
-from pandas import DataFrame
-from numpy import size, sum
 from subgroups.exceptions import InconsistentMethodParametersError
 from subgroups.data_structures.fp_tree_for_sdmap import FPTreeForSDMap
 from subgroups.quality_measures.quality_measure import QualityMeasure
 
 # Python annotations.
 from typing import Union
 
 class FPTreeForSDMapStar(FPTreeForSDMap):
     """This class represents the FPTree data structure used in the SDMapStar algorithm.
     """
 
     __slots__ = ("_TP", "_FP")
 
     def __init__(self,TP:int,FP:int) -> None:
-        """Method to initialize the FPTreeForSDMapStar
+        """Method to initialize the FPTreeForSDMapStar.
+
         :param TP: The number of true positives in the dataset.
         :param FP: The number of false positives in the dataset.
         """
         super().__init__()
         if (type(TP) is not int ):
             raise TypeError("The TP parameter must be an integer.")
         if (type(FP) is not int ):
@@ -68,15 +65,15 @@
         first_selector = list_of_selectors[0]
         # We initialize the final result.
         final_conditional_fp_tree = FPTreeForSDMapStar(self._TP,self._FP)
         ### 1. Generate the conditional pattern base and a dict of frequent selectors with their selectors. ###
         conditional_pattern_base = [] # list[list[ element 1 -> list[Selector], element 2 -> int, element 3 -> int ]]
         # If the first selector is not in the header table, return the current conditional FPTree.
         if first_selector not in self._header_table:
-            return final_conditional_fp_tree
+            return final_conditional_fp_tree, 0
         # Dictionary with all the frequent selectors (before pruning).
         dict_of_all_frequent_selectors = dict() # dict[str, tuple[Selector, list[int], int]]
         # Get the first node in the corresponding horizontal list.
         current_node_in_the_horizontal_list = self._header_table[first_selector][1]
         # Iterate through the horizontal list.
         insertion_order = 0 # The insertion order is necessary later in order to sort the elements which have the same 'n' in a same path.
         pruned_branches = 0
```

### Comparing `subgroups-0.1.6/src/subgroups/data_structures/fp_tree_node.py` & `subgroups-0.1.7/src/subgroups/data_structures/fp_tree_node.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/data_structures/subgroup_list.py` & `subgroups-0.1.7/src/subgroups/data_structures/subgroup_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 from bitarray import bitarray
 from subgroups.core.subgroup import Subgroup
 
 class SubgroupList(object):
     """This class represents a Subgroup List.
     
-    :param bitarray_of_positives: the bitarray of the dataset instances which are covered by the target (its length must be equal to the number of instances of the dataset).
-    :param bitarray_of_negatives: the bitarray of the dataset instances which are not covered by the target (its length must be equal to the number of instances of the dataset).
+    :param dataset_target_bitarray_of_positives: the bitarray of the dataset instances which are covered by the target (its length must be equal to the number of instances of the dataset).
+    :param dataset_target_bitarray_of_negatives: the bitarray of the dataset instances which are not covered by the target (its length must be equal to the number of instances of the dataset).
     :param number_of_dataset_instances: number of instances of the dataset.
     """
 
     __slots__ = ("_default_rule_bitarray_of_positives", "_default_rule_bitarray_of_negatives", "_dataset_target_distribution", "_list_of_subgroups", "_subgroups_bitarrays_of_positives", "_subgroups_bitarrays_of_negatives", "_subgroups_original_bitarrays_of_positives", "_subgroups_original_bitarrays_of_negatives")
 
     def __init__(self, dataset_target_bitarray_of_positives : bitarray, dataset_target_bitarray_of_negatives : bitarray, number_of_dataset_instances : int) -> None:
         if type(dataset_target_bitarray_of_positives) is not bitarray:
```

### Comparing `subgroups-0.1.6/src/subgroups/data_structures/vertical_list.py` & `subgroups-0.1.7/src/subgroups/data_structures/vertical_list.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/data_structures/vertical_list_with_bitsets.py` & `subgroups-0.1.7/src/subgroups/data_structures/vertical_list_with_bitsets.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/data_structures/vertical_list_with_sets.py` & `subgroups-0.1.7/src/subgroups/data_structures/vertical_list_with_sets.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/datasets/__init__.py` & `subgroups-0.1.7/src/subgroups/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/datasets/csv/balloons.csv` & `subgroups-0.1.7/src/subgroups/datasets/csv/balloons.csv`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/datasets/csv/car-evaluation.csv` & `subgroups-0.1.7/src/subgroups/datasets/csv/car-evaluation.csv`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/datasets/csv/covid-sp.csv` & `subgroups-0.1.7/src/subgroups/datasets/csv/covid-sp.csv`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/datasets/csv/credit-g.csv` & `subgroups-0.1.7/src/subgroups/datasets/csv/credit-g.csv`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/datasets/csv/heart-disease.csv` & `subgroups-0.1.7/src/subgroups/datasets/csv/heart-disease.csv`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/datasets/csv/income.csv` & `subgroups-0.1.7/src/subgroups/datasets/csv/income.csv`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/datasets/csv/lenses.csv` & `subgroups-0.1.7/src/subgroups/datasets/csv/lenses.csv`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/datasets/csv/lymph.csv` & `subgroups-0.1.7/src/subgroups/datasets/csv/lymph.csv`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/datasets/csv/mushroom.csv` & `subgroups-0.1.7/src/subgroups/datasets/csv/mushroom.csv`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/datasets/csv/sick.csv` & `subgroups-0.1.7/src/subgroups/datasets/csv/sick.csv`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/datasets/csv/tic-tac-toe.csv` & `subgroups-0.1.7/src/subgroups/datasets/csv/tic-tac-toe.csv`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/datasets/csv/vote.csv` & `subgroups-0.1.7/src/subgroups/datasets/csv/vote.csv`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/exceptions.py` & `subgroups-0.1.7/src/subgroups/exceptions.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/quality_measures/__init__.py` & `subgroups-0.1.7/src/subgroups/quality_measures/__init__.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/quality_measures/absolute_wracc.py` & `subgroups-0.1.7/src/subgroups/quality_measures/absolute_wracc.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/quality_measures/binomial_test.py` & `subgroups-0.1.7/src/subgroups/quality_measures/binomial_test.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/quality_measures/binomial_test_optimistic_estimate_1.py` & `subgroups-0.1.7/src/subgroups/quality_measures/binomial_test_optimistic_estimate_1.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/quality_measures/coverage.py` & `subgroups-0.1.7/src/subgroups/quality_measures/coverage.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/quality_measures/f1_score.py` & `subgroups-0.1.7/src/subgroups/quality_measures/f1_score.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/quality_measures/irr.py` & `subgroups-0.1.7/src/subgroups/quality_measures/irr.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/quality_measures/npv.py` & `subgroups-0.1.7/src/subgroups/quality_measures/npv.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/quality_measures/piatetsky_shapiro.py` & `subgroups-0.1.7/src/subgroups/quality_measures/piatetsky_shapiro.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/quality_measures/piatetsky_shapiro_optimistic_estimate_1.py` & `subgroups-0.1.7/src/subgroups/quality_measures/piatetsky_shapiro_optimistic_estimate_1.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/quality_measures/piatetsky_shapiro_optimistic_estimate_2.py` & `subgroups-0.1.7/src/subgroups/quality_measures/piatetsky_shapiro_optimistic_estimate_2.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/quality_measures/ppv.py` & `subgroups-0.1.7/src/subgroups/quality_measures/ppv.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/quality_measures/qg.py` & `subgroups-0.1.7/src/subgroups/quality_measures/qg.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/quality_measures/quality_measure.py` & `subgroups-0.1.7/src/subgroups/quality_measures/quality_measure.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/quality_measures/sensitivity.py` & `subgroups-0.1.7/src/subgroups/quality_measures/sensitivity.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/quality_measures/specificity.py` & `subgroups-0.1.7/src/subgroups/quality_measures/specificity.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/quality_measures/support.py` & `subgroups-0.1.7/src/subgroups/quality_measures/support.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/quality_measures/wracc.py` & `subgroups-0.1.7/src/subgroups/quality_measures/wracc.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/quality_measures/wracc_optimistic_estimate_1.py` & `subgroups-0.1.7/src/subgroups/quality_measures/wracc_optimistic_estimate_1.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/quality_measures/youden.py` & `subgroups-0.1.7/src/subgroups/quality_measures/youden.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/tests/__init__.py` & `subgroups-0.1.7/src/subgroups/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/tests/algorithms/subgroup_lists/test_dslm.py` & `subgroups-0.1.7/src/subgroups/tests/algorithms/subgroup_lists/test_dslm.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/tests/algorithms/subgroup_lists/test_gmsl.py` & `subgroups-0.1.7/src/subgroups/tests/algorithms/subgroup_lists/test_gmsl.py`

 * *Files 2% similar despite different names*

```diff
@@ -330,54 +330,54 @@
         sl = SubgroupList(bitarray(mask.tolist(), endian = "big"), bitarray((~mask).tolist(), endian = "big"), len(df))
         # Add s1 to the empty subgroup list.
         s1 = Subgroup(Pattern([Selector("doors", Operator.EQUAL, "2")]), Selector("safety", Operator.EQUAL, "unacc"))
         bitarray_of_positives = bitarray("111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000111111111000000000000000000", endian = "big")
         bitarray_of_negatives = bitarray("000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000", endian = "big")
         first_value, instances = GMSL._compute_delta_data_model_candidate(df, sl, s1, bitarray_of_positives, bitarray_of_negatives)
         second_value = GMSL._compute_delta_model_candidate(df, sl, s1)
-        self.assertEqual(first_value, 291.1768556462128)
-        self.assertEqual(second_value, -6.944025328338215)
+        self.assertAlmostEqual(first_value, 291.1768556462128)
+        self.assertAlmostEqual(second_value, -6.944025328338215)
         self.assertEqual(instances, 576)
         sl.add_subgroup(s1, bitarray_of_positives, bitarray_of_negatives)
         # Candidate s2 with only s1 in the list.
         s2 = Subgroup(Pattern([Selector("lug_boot", Operator.EQUAL, "high")]), Selector("safety", Operator.EQUAL, "unacc"))
         bitarray_of_positives = bitarray("001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000", endian = "big")
         bitarray_of_negatives = bitarray("000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001", endian = "big")
         first_value, instances = GMSL._compute_delta_data_model_candidate(df, sl, s2, bitarray_of_positives, bitarray_of_negatives)
         second_value = GMSL._compute_delta_model_candidate(df, sl, s2)
-        self.assertEqual(first_value, 265.8758204686112)
-        self.assertEqual(second_value, -6.4254579619733665)
+        self.assertAlmostEqual(first_value, 265.8758204686112)
+        self.assertAlmostEqual(second_value, -6.4254579619733665)
         self.assertEqual(instances, 384)
         # Candidate s3 with only s1 in the list.
         s3 = Subgroup(Pattern([Selector("lug_boot", Operator.EQUAL, "low")]), Selector("safety", Operator.EQUAL, "unacc"))
         bitarray_of_positives = bitarray("100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100", endian = "big")
         bitarray_of_negatives = bitarray("000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000", endian = "big")
         first_value, instances = GMSL._compute_delta_data_model_candidate(df, sl, s3, bitarray_of_positives, bitarray_of_negatives)
         second_value = GMSL._compute_delta_model_candidate(df, sl, s3)
-        self.assertEqual(first_value, 192.75576029045158)
-        self.assertEqual(second_value, -6.4254579619733665)
+        self.assertAlmostEqual(first_value, 192.75576029045158)
+        self.assertAlmostEqual(second_value, -6.4254579619733665)
         self.assertEqual(instances, 384)
         # Add s2 to the list with s1.
         s2 = Subgroup(Pattern([Selector("lug_boot", Operator.EQUAL, "high")]), Selector("safety", Operator.EQUAL, "unacc"))
         bitarray_of_positives = bitarray("001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000001001001000000000001000000001001001000000000000000000001001001000000000000000000001001001000000000000000000", endian = "big")
         bitarray_of_negatives = bitarray("000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001000000000001001001000001001000000000001001001001001001000000000001001001001001001000000000001001001001001001", endian = "big")
         first_value, instances = GMSL._compute_delta_data_model_candidate(df, sl, s2, bitarray_of_positives, bitarray_of_negatives)
         second_value = GMSL._compute_delta_model_candidate(df, sl, s2)
-        self.assertEqual(first_value, 265.8758204686112)
-        self.assertEqual(second_value, -6.4254579619733665)
+        self.assertAlmostEqual(first_value, 265.8758204686112)
+        self.assertAlmostEqual(second_value, -6.4254579619733665)
         self.assertEqual(instances, 384)
         sl.add_subgroup(s2, bitarray_of_positives, bitarray_of_negatives)
         # Add s3 to the list with s1 and s2.
         s3 = Subgroup(Pattern([Selector("lug_boot", Operator.EQUAL, "low")]), Selector("safety", Operator.EQUAL, "unacc"))
         bitarray_of_positives = bitarray("100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100100", endian = "big")
         bitarray_of_negatives = bitarray("000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000", endian = "big")
         first_value, instances = GMSL._compute_delta_data_model_candidate(df, sl, s3, bitarray_of_positives, bitarray_of_negatives)
         second_value = GMSL._compute_delta_model_candidate(df, sl, s3)
-        self.assertEqual(first_value, 192.7557602904514)
-        self.assertEqual(second_value, -6.674869170148412)
+        self.assertAlmostEqual(first_value, 192.7557602904514)
+        self.assertAlmostEqual(second_value, -6.674869170148412)
         self.assertEqual(instances, 384)
         sl.add_subgroup(s3, bitarray_of_positives, bitarray_of_negatives)
         # len(sl) equal to 3.
         self.assertEqual(len(sl), 3)
     
     def test_GMSL_load_candidates_method_1(self) -> None:
         number_of_dataset_instances = 5 # Number of instances of the original dataset (i.e., from which the subgroups were extracted).
```

### Comparing `subgroups-0.1.6/src/subgroups/tests/algorithms/subgroup_sets/test_bsd.py` & `subgroups-0.1.7/src/subgroups/tests/algorithms/subgroup_sets/test_bsd.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/tests/algorithms/subgroup_sets/test_cbsd.py` & `subgroups-0.1.7/src/subgroups/tests/algorithms/subgroup_sets/test_cbsd.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/tests/algorithms/subgroup_sets/test_cpbsd.py` & `subgroups-0.1.7/src/subgroups/tests/algorithms/subgroup_sets/test_cpbsd.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/tests/algorithms/subgroup_sets/test_qfinder.py` & `subgroups-0.1.7/src/subgroups/tests/algorithms/subgroup_sets/test_qfinder.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 class TestQFinder(unittest.TestCase):
     
     def test_QFinder_init_method1(self):
         # Test with valid parameters
         obj = QFinder(num_subgroups=5, cats=3, max_complexity=10, coverage_thld=0.5,
                            or_thld=1.0, p_val_thld=0.1, abs_contribution_thld=0.3,
                            contribution_thld=4, delta=0.1, write_results_in_file=True,
-                           file_path='results.txt', write_stats_in_file=True,
-                           stats_path='stats.txt')
+                           file_path='results.txt')
         
         # Assert that the object is created without any exceptions
         self.assertIsNotNone(obj)
         
     def test_QFinder_init_method2(self):
         # Test with invalid parameters
         with self.assertRaises(TypeError):
@@ -76,26 +75,20 @@
         
         with self.assertRaises(ValueError):
             # write_results_in_file is True but file_path is None
             QFinder(num_subgroups=5, cats=3, max_complexity=10, coverage_thld=0.5,
                           or_thld=1.0, p_val_thld=0.1, abs_contribution_thld=0.3,
                           contribution_thld=4, delta=0.1, write_results_in_file=True)
         
-        with self.assertRaises(ValueError):
-            # write_stats_in_file is True but stats_path is None
-            QFinder(num_subgroups=5, cats=3, max_complexity=10, coverage_thld=0.5,
-                          or_thld=1.0, p_val_thld=0.1, abs_contribution_thld=0.3,
-                          contribution_thld=4, delta=0.1, write_stats_in_file=True)
-                          
     def test_QFinder_generate_candidate_patterns1(self):
         df = DataFrame({'bread': {0: 'yes', 1: 'yes', 2: 'no', 3: 'yes', 4: 'yes', 5: 'yes', 6: 'yes'}, 'milk': {0: 'yes', 1: 'no', 2: 'yes', 3: 'yes', 4: 'yes', 5: 'yes', 6: 'yes'}, 'beer': {0: 'no', 1: 'yes', 2: 'yes', 3: 'yes', 4: 'no', 5: 'yes', 6: 'no'}, 'coke': {0: 'no', 1: 'no', 2: 'yes', 3: 'no', 4: 'yes', 5: 'no', 6: 'yes'}, 'diaper': {0: 'no', 1: 'yes', 2: 'yes', 3: 'yes', 4: 'yes', 5: 'yes', 6: 'yes'}})        
         target = ("diaper", "yes")
-        model = QFinder(num_subgroups=5)
         complexity = 3
-        patterns = model._generate_candidate_patterns(df,target, complexity)
+        model = QFinder(num_subgroups=5, max_complexity=complexity)
+        patterns = model._generate_candidate_patterns(df,target)
         simple_selectors = [
             Selector("bread", Operator.EQUAL, "yes"),
             Selector("milk", Operator.EQUAL, "yes"),
             Selector("beer", Operator.EQUAL, "yes"),
             Selector("coke", Operator.EQUAL, "yes"),
             Selector("bread", Operator.EQUAL, "no"),
             Selector("milk", Operator.EQUAL, "no"),
@@ -117,17 +110,16 @@
         for pat in test_complex_patterns:
             self.assertIn(pat, patterns)
         
     def test_QFinder_generate_candidate_patterns2(self):
         # Check that the value 'other' is added to the categorical variables
         df = DataFrame({'a': {0: '1', 1: '1', 2: '1', 3: '2', 4: '3'}, 'class': {0: '1', 1: '1', 2: '1', 3: '1', 4: '1'}})
         target = ("class", 1)
-        model = QFinder(num_subgroups=5)
-        complexity = 1
-        patterns = model._generate_candidate_patterns(df,target, complexity,cats=2)
+        model = QFinder(num_subgroups=5, max_complexity=1, cats=2)
+        patterns = model._generate_candidate_patterns(df,target)
         simple_selectors = [
             Selector("a", Operator.EQUAL, '1'),
             Selector("a", Operator.EQUAL, "other"),
         ]
         simple_patterns = [Pattern([sel]) for sel in simple_selectors]
         for pat in simple_patterns:
             self.assertIn(pat, patterns)
```

### Comparing `subgroups-0.1.6/src/subgroups/tests/algorithms/subgroup_sets/test_sdmap.py` & `subgroups-0.1.7/src/subgroups/tests/algorithms/subgroup_sets/test_sdmap.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/tests/algorithms/subgroup_sets/test_sdmapstar.py` & `subgroups-0.1.7/src/subgroups/tests/algorithms/subgroup_sets/test_sdmapstar.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/tests/algorithms/subgroup_sets/test_vlsd.py` & `subgroups-0.1.7/src/subgroups/tests/algorithms/subgroup_sets/test_vlsd.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/tests/core/test_operator.py` & `subgroups-0.1.7/src/subgroups/tests/core/test_operator.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/tests/core/test_pattern.py` & `subgroups-0.1.7/src/subgroups/tests/core/test_pattern.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/tests/core/test_selector.py` & `subgroups-0.1.7/src/subgroups/tests/core/test_selector.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/tests/core/test_subgroup.py` & `subgroups-0.1.7/src/subgroups/tests/core/test_subgroup.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/tests/data_structures/test_fp_tree_for_sdmap.py` & `subgroups-0.1.7/src/subgroups/tests/data_structures/test_fp_tree_for_sdmap.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/tests/data_structures/test_fp_tree_node.py` & `subgroups-0.1.7/src/subgroups/tests/data_structures/test_fp_tree_node.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/tests/data_structures/test_subgroup_list.py` & `subgroups-0.1.7/src/subgroups/tests/data_structures/test_subgroup_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from subgroups.data_structures.subgroup_list import SubgroupList
 from subgroups.core.operator import Operator
 from subgroups.core.selector import Selector
 from subgroups.core.pattern import Pattern
 from subgroups.core.subgroup import Subgroup
 from pandas import DataFrame
 from bitarray import bitarray
+from subgroups import datasets
 import unittest
 
 class TestSubgroupList(unittest.TestCase):
 
     def test_subgroup_list_1(self) -> None:
         self.assertRaises(TypeError, SubgroupList, bitarray("10110"), "a", 5)
         self.assertRaises(TypeError, SubgroupList, "a", bitarray("01001"), 5)
@@ -662,7 +663,23 @@
         self.assertEqual(sl.get_subgroup_bitarray_of_negatives(1), bitarray("00001"))
         self.assertFalse(sl.is_empty())
         self.assertNotEqual(id(bitarray_of_positives), id(sl.get_subgroup_bitarray_of_positives(1)))
         self.assertNotEqual(id(bitarray_of_negatives), id(sl.get_subgroup_bitarray_of_negatives(1)))
         self.assertRaises(IndexError, sl.get_subgroup, 2)
         self.assertRaises(IndexError, sl.get_subgroup_bitarray_of_positives, 2)
         self.assertRaises(IndexError, sl.get_subgroup_bitarray_of_negatives, 2)
+
+    def test_subgroup_list_5(self) -> None:
+        # Load the dataset.
+        df = datasets.load_ballons_csv()
+        target = ("inflated", "T")
+        # Create the subgroups.
+        sl1_s1 = Subgroup.generate_from_str("Description: [color = 'YELLOW', size = 'SMALL'], Target: inflated = 'T'")
+        sl1_s2 = Subgroup.generate_from_str("Description: [color = 'YELLOW', size = 'LARGE'], Target: inflated = 'T'")
+        sl1_s3 = Subgroup.generate_from_str("Description: [act = 'STRETCH', age = 'ADULT'], Target: inflated = 'T'")
+        sl1_s4 = Subgroup.generate_from_str("Description: [act = 'STRETCH', age = 'CHILD'], Target: inflated = 'T'")
+        # Create the subgroup list.
+        sl1 = SubgroupList(bitarray((df[target[0]] == target[1]).to_list(), endian="big"), bitarray((df[target[0]] != target[1]).to_list(), endian="big"), len(df))
+        sl1.add_subgroup(sl1_s1, bitarray((sl1_s1.description.is_contained(df) & sl1_s1.target.match(target[0], df[target[0]])).to_list(), endian="big"), bitarray((sl1_s1.description.is_contained(df) & (~ sl1_s1.target.match(target[0], df[target[0]]))).to_list(), endian="big"))
+        sl1.add_subgroup(sl1_s2, bitarray((sl1_s2.description.is_contained(df) & sl1_s2.target.match(target[0], df[target[0]])).to_list(), endian="big"), bitarray((sl1_s2.description.is_contained(df) & (~ sl1_s2.target.match(target[0], df[target[0]]))).to_list(), endian="big"))
+        sl1.add_subgroup(sl1_s3, bitarray((sl1_s3.description.is_contained(df) & sl1_s3.target.match(target[0], df[target[0]])).to_list(), endian="big"), bitarray((sl1_s3.description.is_contained(df) & (~ sl1_s3.target.match(target[0], df[target[0]]))).to_list(), endian="big"))
+        sl1.add_subgroup(sl1_s4, bitarray((sl1_s4.description.is_contained(df) & sl1_s4.target.match(target[0], df[target[0]])).to_list(), endian="big"), bitarray((sl1_s4.description.is_contained(df) & (~ sl1_s4.target.match(target[0], df[target[0]]))).to_list(), endian="big"))
```

### Comparing `subgroups-0.1.6/src/subgroups/tests/data_structures/test_vertical_list_with_bitsets.py` & `subgroups-0.1.7/src/subgroups/tests/data_structures/test_vertical_list_with_bitsets.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/tests/data_structures/test_vertical_list_with_sets.py` & `subgroups-0.1.7/src/subgroups/tests/data_structures/test_vertical_list_with_sets.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/tests/quality_measures/test_quality_measures.py` & `subgroups-0.1.7/src/subgroups/tests/quality_measures/test_quality_measures.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/tests/utils/test_dataframe_filters.py` & `subgroups-0.1.7/src/subgroups/tests/utils/test_dataframe_filters.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/tests/utils/test_file_format_transformations.py` & `subgroups-0.1.7/src/subgroups/tests/utils/test_file_format_transformations.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/utils/dataframe_filters.py` & `subgroups-0.1.7/src/subgroups/utils/dataframe_filters.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/utils/file_format_transformations.py` & `subgroups-0.1.7/src/subgroups/utils/file_format_transformations.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups/utils/mdl.py` & `subgroups-0.1.7/src/subgroups/utils/mdl.py`

 * *Files identical despite different names*

### Comparing `subgroups-0.1.6/src/subgroups.egg-info/SOURCES.txt` & `subgroups-0.1.7/src/subgroups.egg-info/SOURCES.txt`

 * *Files identical despite different names*

