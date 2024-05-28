# Comparing `tmp/quickstats-0.7.0.4.tar.gz` & `tmp/quickstats-0.7.0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstats-0.7.0.4.tar", last modified: Thu Apr 25 03:41:34 2024, max compression
+gzip compressed data, was "quickstats-0.7.0.4.1.tar", last modified: Tue May 28 15:23:27 2024, max compression
```

## Comparing `quickstats-0.7.0.4.tar` & `quickstats-0.7.0.4.1.tar`

### file list

```diff
@@ -1,295 +1,296 @@
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:34.000000 quickstats-0.7.0.4/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4125 2024-04-25 03:41:34.000000 quickstats-0.7.0.4/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2024-03-20 05:53:30.000000 quickstats-0.7.0.4/README.md
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:18.000000 quickstats-0.7.0.4/bin/
--rwxr-xr-x   0 chlcheng (124202) zp        (1307)       93 2024-03-20 05:53:30.000000 quickstats-0.7.0.4/bin/quickstats
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:19.000000 quickstats-0.7.0.4/quickstats/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      134 2024-04-18 15:35:29.000000 quickstats-0.7.0.4/quickstats/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)       24 2024-04-25 03:40:17.000000 quickstats-0.7.0.4/quickstats/_version.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:20.000000 quickstats-0.7.0.4/quickstats/algorithms/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:30.000000 quickstats-0.7.0.4/quickstats/algorithms/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:20.000000 quickstats-0.7.0.4/quickstats/algorithms/nll_crossing/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4350 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/algorithms/nll_crossing/BaseMethod.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/algorithms/nll_crossing/BisectionMethod.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/algorithms/nll_crossing/NovelMethod.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/algorithms/nll_crossing/SteppingMethod.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/algorithms/nll_crossing/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:21.000000 quickstats-0.7.0.4/quickstats/analysis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2024-04-18 15:35:43.000000 quickstats-0.7.0.4/quickstats/analysis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9725 2024-04-18 15:35:49.000000 quickstats-0.7.0.4/quickstats/analysis/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4025 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/analysis/analysis_path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    21556 2024-04-18 15:36:06.000000 quickstats-0.7.0.4/quickstats/analysis/config_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    41208 2024-04-18 15:35:54.000000 quickstats-0.7.0.4/quickstats/analysis/data_loading.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1311 2024-04-18 15:36:08.000000 quickstats-0.7.0.4/quickstats/analysis/data_preprocessing.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    85738 2024-04-18 15:35:54.000000 quickstats-0.7.0.4/quickstats/analysis/event_categorization.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8048 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/analysis/multi_class_boundary_tree.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9238 2024-04-18 15:35:54.000000 quickstats-0.7.0.4/quickstats/analysis/ntuple_conversion_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    33252 2024-04-25 03:40:17.000000 quickstats-0.7.0.4/quickstats/analysis/ntuple_process_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8906 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/analysis/sample_poly_param_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:21.000000 quickstats-0.7.0.4/quickstats/analysis/systematics/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/analysis/systematics/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29468 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/analysis/systematics/base_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9760 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/analysis/systematics/gaussian_shape_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6753 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/analysis/systematics/normalization_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11890 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/analysis/systematics/systematics_evaluation_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:21.000000 quickstats-0.7.0.4/quickstats/clis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      237 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/clis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2816 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/clis/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1908 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/clis/inspect_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    23632 2024-04-25 03:40:17.000000 quickstats-0.7.0.4/quickstats/clis/likelihood_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15027 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/clis/limit_setting.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    19517 2024-04-18 15:43:10.000000 quickstats-0.7.0.4/quickstats/clis/nuisance_parameter_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1609 2024-03-20 05:53:31.000000 quickstats-0.7.0.4/quickstats/clis/processor_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18230 2024-03-20 05:53:32.000000 quickstats-0.7.0.4/quickstats/clis/stat_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18810 2024-03-20 05:54:19.000000 quickstats-0.7.0.4/quickstats/clis/workspace_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:22.000000 quickstats-0.7.0.4/quickstats/components/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1113 2024-04-18 15:39:11.000000 quickstats-0.7.0.4/quickstats/components/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3136 2024-03-20 05:53:32.000000 quickstats-0.7.0.4/quickstats/components/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15274 2024-04-25 03:40:17.000000 quickstats-0.7.0.4/quickstats/components/analysis_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7330 2024-03-20 05:53:32.000000 quickstats-0.7.0.4/quickstats/components/asimov_generator.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    31508 2024-03-20 05:53:32.000000 quickstats-0.7.0.4/quickstats/components/asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3273 2024-03-20 05:53:32.000000 quickstats-0.7.0.4/quickstats/components/basics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3156 2024-03-20 05:53:32.000000 quickstats-0.7.0.4/quickstats/components/caching_nll_wrapper.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10479 2024-03-20 05:53:32.000000 quickstats-0.7.0.4/quickstats/components/discrete_nuisance.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    56823 2024-04-18 15:35:32.000000 quickstats-0.7.0.4/quickstats/components/extended_minimizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)   105095 2024-03-20 05:53:32.000000 quickstats-0.7.0.4/quickstats/components/extended_model.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5859 2024-04-18 15:34:25.000000 quickstats-0.7.0.4/quickstats/components/extended_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14097 2024-04-18 15:41:02.000000 quickstats-0.7.0.4/quickstats/components/likelihood.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:23.000000 quickstats-0.7.0.4/quickstats/components/modelling/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.7.0.4/quickstats/components/modelling/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2504 2024-03-20 05:53:32.000000 quickstats-0.7.0.4/quickstats/components/modelling/component_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    20116 2024-04-18 15:35:32.000000 quickstats-0.7.0.4/quickstats/components/modelling/data_modelling.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      735 2024-03-20 05:53:33.000000 quickstats-0.7.0.4/quickstats/components/modelling/model_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4502 2024-03-20 05:53:33.000000 quickstats-0.7.0.4/quickstats/components/modelling/parameter_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5550 2024-03-20 05:53:33.000000 quickstats-0.7.0.4/quickstats/components/modelling/pdf_fit_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3483 2024-03-20 05:53:33.000000 quickstats-0.7.0.4/quickstats/components/modelling/tree_data_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10864 2024-03-20 05:53:33.000000 quickstats-0.7.0.4/quickstats/components/nuisance_parameter_harmonizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    17594 2024-03-20 05:53:33.000000 quickstats-0.7.0.4/quickstats/components/nuisance_parameter_pull.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12380 2024-04-18 15:35:32.000000 quickstats-0.7.0.4/quickstats/components/nuisance_parameter_ranking.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:23.000000 quickstats-0.7.0.4/quickstats/components/processors/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2024-04-18 15:34:50.000000 quickstats-0.7.0.4/quickstats/components/processors/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:24.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1457 2024-04-25 03:40:17.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      388 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/auxiliary.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      358 2024-04-18 15:36:38.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/formatter.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1608 2024-04-18 15:39:37.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2360 2024-04-25 03:40:17.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_as_hdf.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2037 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_as_numpy.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1589 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_as_parquet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4421 2024-04-18 15:39:37.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_base_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1049 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_cache.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      866 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_declare.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1826 2024-04-18 15:39:37.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1228 2024-04-18 15:34:47.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_export.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1903 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_filter.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1331 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_global_variables.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_helper_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_hybrid_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      755 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_if_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      763 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_if_not_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      726 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_load_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1211 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_load_macro.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_max.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      225 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_mean.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_min.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_nested_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2249 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_output_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      757 2024-04-18 15:34:47.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_progressbar.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_rdf_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      481 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_redefine.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1854 2024-04-18 15:36:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_report.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      723 2024-04-18 15:36:56.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_safe_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      539 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_safe_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1770 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_save.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      735 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_save_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1433 2024-04-18 15:39:37.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_stat.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      226 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_sum.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      606 2024-04-18 15:34:45.000000 quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_treename.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13111 2024-04-18 15:34:23.000000 quickstats-0.7.0.4/quickstats/components/processors/builtin_methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12481 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/components/processors/roo_process_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13856 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/components/processors/roo_processor.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5406 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/pvalue_toys.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2978 2024-04-18 15:35:39.000000 quickstats-0.7.0.4/quickstats/components/roo_inspector.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3103 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/root_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    21325 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/toy_limit_calculator.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:25.000000 quickstats-0.7.0.4/quickstats/components/workspaces/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      591 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/workspaces/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9877 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/workspaces/asimov_handler.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1727 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/workspaces/core_argument_sets.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/workspaces/sample.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/workspaces/settings.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8910 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/workspaces/systematic.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/workspaces/systematics_domain.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    53148 2024-04-18 15:35:32.000000 quickstats-0.7.0.4/quickstats/components/workspaces/ws_comparer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8787 2024-04-18 15:35:32.000000 quickstats-0.7.0.4/quickstats/components/workspaces/ws_decomposer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1724 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/workspaces/ws_modifier_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10827 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/workspaces/xml_ws_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    87015 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/components/workspaces/xml_ws_builder_v1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    76446 2024-04-18 15:34:27.000000 quickstats-0.7.0.4/quickstats/components/workspaces/xml_ws_builder_v2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    52888 2024-04-18 15:35:32.000000 quickstats-0.7.0.4/quickstats/components/workspaces/xml_ws_combiner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    55314 2024-04-18 15:35:32.000000 quickstats-0.7.0.4/quickstats/components/workspaces/xml_ws_modifier.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:26.000000 quickstats-0.7.0.4/quickstats/concurrent/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      372 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/concurrent/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4197 2024-04-18 15:35:40.000000 quickstats-0.7.0.4/quickstats/concurrent/abstract_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.7.0.4/quickstats/concurrent/logging.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5209 2024-03-20 05:53:34.000000 quickstats-0.7.0.4/quickstats/concurrent/nuisance_parameter_ranking_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5285 2024-04-18 15:36:29.000000 quickstats-0.7.0.4/quickstats/concurrent/parameterised_asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10852 2024-04-18 15:36:29.000000 quickstats-0.7.0.4/quickstats/concurrent/parameterised_likelihood.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5822 2024-03-20 05:54:19.000000 quickstats-0.7.0.4/quickstats/concurrent/parameterised_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7694 2024-04-18 15:41:02.000000 quickstats-0.7.0.4/quickstats/concurrent/parameterised_significance.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:27.000000 quickstats-0.7.0.4/quickstats/core/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      411 2024-04-18 15:36:36.000000 quickstats-0.7.0.4/quickstats/core/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      783 2024-03-20 05:53:35.000000 quickstats-0.7.0.4/quickstats/core/abstract_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    32252 2024-04-18 15:36:37.000000 quickstats-0.7.0.4/quickstats/core/configuration.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4546 2024-04-18 15:35:34.000000 quickstats-0.7.0.4/quickstats/core/constraints.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4603 2024-04-18 15:36:10.000000 quickstats-0.7.0.4/quickstats/core/decorators.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7569 2024-04-18 15:36:10.000000 quickstats-0.7.0.4/quickstats/core/enums.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7707 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/core/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2106 2024-04-18 15:36:02.000000 quickstats-0.7.0.4/quickstats/core/metaclasses.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7624 2024-04-18 15:39:09.000000 quickstats-0.7.0.4/quickstats/core/methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9554 2024-03-20 05:53:35.000000 quickstats-0.7.0.4/quickstats/core/path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      721 2024-04-18 15:35:28.000000 quickstats-0.7.0.4/quickstats/core/setup.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6584 2024-04-18 15:36:06.000000 quickstats-0.7.0.4/quickstats/core/type_validation.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3895 2024-04-18 15:35:28.000000 quickstats-0.7.0.4/quickstats/core/virtual_trees.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:27.000000 quickstats-0.7.0.4/quickstats/daq/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      151 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/daq/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6933 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/daq/remote_data_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3849 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/daq/servicex_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2553 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/daq/xrootd_source.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:27.000000 quickstats-0.7.0.4/quickstats/extensions/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       85 2024-03-20 05:53:35.000000 quickstats-0.7.0.4/quickstats/extensions/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4147 2024-03-20 05:53:35.000000 quickstats-0.7.0.4/quickstats/extensions/extension_dataframe.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:27.000000 quickstats-0.7.0.4/quickstats/interface/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-04-18 15:35:04.000000 quickstats-0.7.0.4/quickstats/interface/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:28.000000 quickstats-0.7.0.4/quickstats/interface/cppyy/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      198 2024-04-18 15:39:03.000000 quickstats-0.7.0.4/quickstats/interface/cppyy/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      392 2024-03-20 05:53:35.000000 quickstats-0.7.0.4/quickstats/interface/cppyy/basic_methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2023-09-01 18:55:46.000000 quickstats-0.7.0.4/quickstats/interface/cppyy/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12794 2024-03-20 05:53:35.000000 quickstats-0.7.0.4/quickstats/interface/cppyy/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4540 2024-03-20 05:53:36.000000 quickstats-0.7.0.4/quickstats/interface/cppyy/vectorize.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:28.000000 quickstats-0.7.0.4/quickstats/interface/kerberos/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      109 2024-04-18 15:39:14.000000 quickstats-0.7.0.4/quickstats/interface/kerberos/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1709 2024-04-18 15:39:14.000000 quickstats-0.7.0.4/quickstats/interface/kerberos/core.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:30.000000 quickstats-0.7.0.4/quickstats/interface/root/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3819 2024-03-20 05:53:36.000000 quickstats-0.7.0.4/quickstats/interface/root/ModelConfig.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10737 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/interface/root/RDataFrame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2306 2024-03-20 05:53:36.000000 quickstats-0.7.0.4/quickstats/interface/root/RooAbsArg.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.7.0.4/quickstats/interface/root/RooAbsData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    21668 2024-03-20 05:53:36.000000 quickstats-0.7.0.4/quickstats/interface/root/RooAbsPdf.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3531 2024-03-20 05:53:36.000000 quickstats-0.7.0.4/quickstats/interface/root/RooArgSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2024-03-20 05:53:36.000000 quickstats-0.7.0.4/quickstats/interface/root/RooCategory.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    44967 2024-03-20 05:53:36.000000 quickstats-0.7.0.4/quickstats/interface/root/RooDataSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.7.0.4/quickstats/interface/root/RooMsgService.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6728 2024-03-20 05:53:36.000000 quickstats-0.7.0.4/quickstats/interface/root/RooRealVar.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.7.0.4/quickstats/interface/root/TArrayData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2905 2024-04-18 15:34:20.000000 quickstats-0.7.0.4/quickstats/interface/root/TChain.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2024-03-20 05:53:36.000000 quickstats-0.7.0.4/quickstats/interface/root/TF1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11390 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/interface/root/TFile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2024-03-20 05:53:36.000000 quickstats-0.7.0.4/quickstats/interface/root/TH1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5813 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/interface/root/TH2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6043 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/interface/root/TH3.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      378 2024-04-18 15:34:42.000000 quickstats-0.7.0.4/quickstats/interface/root/TObject.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      748 2024-04-18 15:39:11.000000 quickstats-0.7.0.4/quickstats/interface/root/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.7.0.4/quickstats/interface/root/helper.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.7.0.4/quickstats/interface/root/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    27713 2024-03-20 05:53:36.000000 quickstats-0.7.0.4/quickstats/interface/root/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5634 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/interface/root/roofit_extension.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:30.000000 quickstats-0.7.0.4/quickstats/interface/servicex/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      163 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/interface/servicex/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5409 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/interface/servicex/config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2872 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/interface/servicex/core.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:30.000000 quickstats-0.7.0.4/quickstats/interface/tinydb/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       67 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/interface/tinydb/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      947 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/interface/tinydb/methods.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:30.000000 quickstats-0.7.0.4/quickstats/interface/xrootd/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      149 2024-04-18 15:39:06.000000 quickstats-0.7.0.4/quickstats/interface/xrootd/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      448 2024-04-18 15:39:06.000000 quickstats-0.7.0.4/quickstats/interface/xrootd/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5850 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/interface/xrootd/filesystem.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1163 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/interface/xrootd/path.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2573 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/interface/xrootd/xrd_helper.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:18.000000 quickstats-0.7.0.4/quickstats/macros/
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:30.000000 quickstats-0.7.0.4/quickstats/macros/AsymptoticCLsTool/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7366 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1591 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:30.000000 quickstats-0.7.0.4/quickstats/macros/FlexibleInterpVarMkII/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.7.0.4/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.7.0.4/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:30.000000 quickstats-0.7.0.4/quickstats/macros/QuickStatsCore/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3133 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/macros/QuickStatsCore/QStringUtils.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1259 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10312 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/macros/QuickStatsCore/RooFitExt.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3868 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/macros/QuickStatsCore/RooFitExt.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:30.000000 quickstats-0.7.0.4/quickstats/macros/ResponseFunction/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13749 2024-04-18 15:34:34.000000 quickstats-0.7.0.4/quickstats/macros/ResponseFunction/ResponseFunction.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2023-04-25 19:07:54.000000 quickstats-0.7.0.4/quickstats/macros/ResponseFunction/ResponseFunction.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:31.000000 quickstats-0.7.0.4/quickstats/macros/RooTwoSidedCBShape/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.7.0.4/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.7.0.4/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:31.000000 quickstats-0.7.0.4/quickstats/maths/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.7.0.4/quickstats/maths/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4366 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/maths/interpolation.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9053 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/maths/numerics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    40281 2024-04-18 15:41:02.000000 quickstats-0.7.0.4/quickstats/maths/statistics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3506 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/maths/statistics_jitted.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.7.0.4/quickstats/maths/symbolics.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:31.000000 quickstats-0.7.0.4/quickstats/parsers/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      187 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/parsers/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.7.0.4/quickstats/parsers/config_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16764 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/parsers/param_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5204 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/parsers/roo_param_setup_parser.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:33.000000 quickstats-0.7.0.4/quickstats/plots/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1345 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/plots/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    28606 2024-04-18 15:41:02.000000 quickstats-0.7.0.4/quickstats/plots/abstract_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14144 2024-04-18 15:38:50.000000 quickstats-0.7.0.4/quickstats/plots/bidirectional_bar_chart.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.7.0.4/quickstats/plots/collective_data_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3467 2024-04-18 15:35:22.000000 quickstats-0.7.0.4/quickstats/plots/color_schemes.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5899 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/plots/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4951 2024-03-20 05:53:37.000000 quickstats-0.7.0.4/quickstats/plots/correlation_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7581 2024-04-18 15:38:51.000000 quickstats-0.7.0.4/quickstats/plots/general_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4061 2024-04-18 15:38:51.000000 quickstats-0.7.0.4/quickstats/plots/general_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    22203 2024-04-18 15:41:03.000000 quickstats-0.7.0.4/quickstats/plots/general_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6078 2024-04-18 15:38:56.000000 quickstats-0.7.0.4/quickstats/plots/hypotest_inverter_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8981 2024-03-20 05:53:38.000000 quickstats-0.7.0.4/quickstats/plots/likelihood_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16926 2024-04-18 15:38:51.000000 quickstats-0.7.0.4/quickstats/plots/likelihood_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29155 2024-03-20 05:53:38.000000 quickstats-0.7.0.4/quickstats/plots/np_ranking_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    25684 2024-04-18 15:41:03.000000 quickstats-0.7.0.4/quickstats/plots/pdf_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5096 2024-04-18 15:38:51.000000 quickstats-0.7.0.4/quickstats/plots/sample_purity_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10353 2024-04-18 15:38:51.000000 quickstats-0.7.0.4/quickstats/plots/score_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4122 2024-03-20 05:53:38.000000 quickstats-0.7.0.4/quickstats/plots/stat_plot_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    30210 2024-04-18 15:41:03.000000 quickstats-0.7.0.4/quickstats/plots/template.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13785 2024-04-18 15:38:51.000000 quickstats-0.7.0.4/quickstats/plots/test_statistic_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5122 2024-03-20 05:53:38.000000 quickstats-0.7.0.4/quickstats/plots/two_axis_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9999 2024-04-18 15:42:16.000000 quickstats-0.7.0.4/quickstats/plots/upper_limit_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    19292 2024-04-18 15:38:51.000000 quickstats-0.7.0.4/quickstats/plots/upper_limit_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13182 2024-04-18 15:38:51.000000 quickstats-0.7.0.4/quickstats/plots/upper_limit_3D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    23223 2024-04-18 15:41:04.000000 quickstats-0.7.0.4/quickstats/plots/upper_limit_benchmark_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    34148 2024-04-18 15:41:04.000000 quickstats-0.7.0.4/quickstats/plots/variable_distribution_plot.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:33.000000 quickstats-0.7.0.4/quickstats/resources/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2024-03-20 05:53:39.000000 quickstats-0.7.0.4/quickstats/resources/default_workspace_extensions.json
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:33.000000 quickstats-0.7.0.4/quickstats/resources/mpl_stylesheets/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2024-03-20 05:53:39.000000 quickstats-0.7.0.4/quickstats/resources/mpl_stylesheets/hep.mplstyle
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2024-03-20 05:53:39.000000 quickstats-0.7.0.4/quickstats/resources/mpl_stylesheets/no_latex.mplstyle
--rw-r--r--   0 chlcheng (124202) zp        (1307)      325 2024-03-20 05:53:39.000000 quickstats-0.7.0.4/quickstats/resources/mpl_stylesheets/science.mplstyle
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4604 2024-03-20 05:53:39.000000 quickstats-0.7.0.4/quickstats/root_checker.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:34.000000 quickstats-0.7.0.4/quickstats/utils/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.7.0.4/quickstats/utils/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    19773 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/utils/common_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.7.0.4/quickstats/utils/condor_tasks.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18666 2024-04-18 15:39:08.000000 quickstats-0.7.0.4/quickstats/utils/data_conversion.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.7.0.4/quickstats/utils/hep_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3039 2024-04-25 03:40:18.000000 quickstats-0.7.0.4/quickstats/utils/path_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      563 2024-04-18 15:35:24.000000 quickstats-0.7.0.4/quickstats/utils/py_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    27521 2024-04-18 15:36:12.000000 quickstats-0.7.0.4/quickstats/utils/roofit_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10914 2024-03-20 05:53:39.000000 quickstats-0.7.0.4/quickstats/utils/roostats_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15330 2024-04-18 15:36:32.000000 quickstats-0.7.0.4/quickstats/utils/root_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15638 2024-04-18 15:39:31.000000 quickstats-0.7.0.4/quickstats/utils/string_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2321 2024-04-18 15:36:21.000000 quickstats-0.7.0.4/quickstats/utils/sys_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15128 2024-04-18 15:35:57.000000 quickstats-0.7.0.4/quickstats/utils/xml_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2024-04-25 03:41:20.000000 quickstats-0.7.0.4/quickstats.egg-info/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4125 2024-04-25 03:41:13.000000 quickstats-0.7.0.4/quickstats.egg-info/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11068 2024-04-25 03:41:16.000000 quickstats-0.7.0.4/quickstats.egg-info/SOURCES.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2024-04-25 03:41:15.000000 quickstats-0.7.0.4/quickstats.egg-info/dependency_links.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2024-04-25 03:41:15.000000 quickstats-0.7.0.4/quickstats.egg-info/requires.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2024-04-25 03:41:15.000000 quickstats-0.7.0.4/quickstats.egg-info/top_level.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2024-04-25 03:41:34.000000 quickstats-0.7.0.4/setup.cfg
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1771 2024-04-18 15:34:33.000000 quickstats-0.7.0.4/setup.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:27.057317 quickstats-0.7.0.4.1/
+-rw-r--r--   0 chlcheng (102623) chlcheng (102623)     4127 2024-05-28 15:23:27.056653 quickstats-0.7.0.4.1/PKG-INFO
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     3567 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/README.md
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:26.901513 quickstats-0.7.0.4.1/bin/
+-rwxrwx---   0 chlcheng (102623) chlcheng (102623)       93 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/bin/quickstats
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:26.903060 quickstats-0.7.0.4.1/quickstats/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      134 2024-04-02 16:59:53.000000 quickstats-0.7.0.4.1/quickstats/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)       26 2024-05-28 15:21:34.000000 quickstats-0.7.0.4.1/quickstats/_version.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:26.905986 quickstats-0.7.0.4.1/quickstats/algorithms/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2023-11-06 04:44:35.000000 quickstats-0.7.0.4.1/quickstats/algorithms/__init__.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:26.908860 quickstats-0.7.0.4.1/quickstats/algorithms/nll_crossing/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     4350 2024-02-09 19:22:50.000000 quickstats-0.7.0.4.1/quickstats/algorithms/nll_crossing/BaseMethod.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2023-11-06 04:44:35.000000 quickstats-0.7.0.4.1/quickstats/algorithms/nll_crossing/BisectionMethod.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2023-11-06 04:44:35.000000 quickstats-0.7.0.4.1/quickstats/algorithms/nll_crossing/NovelMethod.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2023-11-06 04:44:35.000000 quickstats-0.7.0.4.1/quickstats/algorithms/nll_crossing/SteppingMethod.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2023-11-06 04:44:35.000000 quickstats-0.7.0.4.1/quickstats/algorithms/nll_crossing/__init__.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:26.916787 quickstats-0.7.0.4.1/quickstats/analysis/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      428 2024-04-02 17:36:13.000000 quickstats-0.7.0.4.1/quickstats/analysis/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     9763 2024-05-18 08:43:03.000000 quickstats-0.7.0.4.1/quickstats/analysis/analysis_base.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     3881 2024-05-18 10:07:29.000000 quickstats-0.7.0.4.1/quickstats/analysis/analysis_path_manager.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    21556 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/analysis/config_templates.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    41208 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/analysis/data_loading.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1311 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/analysis/data_preprocessing.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    85738 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/analysis/event_categorization.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     8048 2024-02-09 19:22:50.000000 quickstats-0.7.0.4.1/quickstats/analysis/multi_class_boundary_tree.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     9238 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/analysis/ntuple_conversion_tool.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    33252 2024-04-23 13:33:55.000000 quickstats-0.7.0.4.1/quickstats/analysis/ntuple_process_tool.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     8906 2024-02-09 19:22:50.000000 quickstats-0.7.0.4.1/quickstats/analysis/sample_poly_param_tool.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:26.919476 quickstats-0.7.0.4.1/quickstats/analysis/systematics/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      241 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/analysis/systematics/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    29468 2024-02-09 19:22:50.000000 quickstats-0.7.0.4.1/quickstats/analysis/systematics/base_systematics.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     9760 2024-02-09 19:22:50.000000 quickstats-0.7.0.4.1/quickstats/analysis/systematics/gaussian_shape_systematics.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     6753 2024-02-09 19:22:50.000000 quickstats-0.7.0.4.1/quickstats/analysis/systematics/normalization_systematics.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    11890 2024-02-09 19:22:50.000000 quickstats-0.7.0.4.1/quickstats/analysis/systematics/systematics_evaluation_tool.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:26.923610 quickstats-0.7.0.4.1/quickstats/clis/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      237 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/clis/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     2816 2024-02-09 19:22:50.000000 quickstats-0.7.0.4.1/quickstats/clis/core.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1908 2024-03-22 01:36:00.000000 quickstats-0.7.0.4.1/quickstats/clis/inspect_rfile.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    23632 2024-04-24 20:02:12.000000 quickstats-0.7.0.4.1/quickstats/clis/likelihood_tools.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    15027 2024-03-02 09:26:25.000000 quickstats-0.7.0.4.1/quickstats/clis/limit_setting.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    19517 2024-04-02 16:59:53.000000 quickstats-0.7.0.4.1/quickstats/clis/nuisance_parameter_tools.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1609 2024-02-09 19:22:50.000000 quickstats-0.7.0.4.1/quickstats/clis/processor_tools.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    18230 2024-02-09 19:22:50.000000 quickstats-0.7.0.4.1/quickstats/clis/stat_tools.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    18810 2024-03-22 01:36:00.000000 quickstats-0.7.0.4.1/quickstats/clis/workspace_tools.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:26.933518 quickstats-0.7.0.4.1/quickstats/components/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1113 2024-04-16 04:58:47.000000 quickstats-0.7.0.4.1/quickstats/components/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     3136 2024-02-09 19:22:50.000000 quickstats-0.7.0.4.1/quickstats/components/analysis_base.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    15274 2024-04-24 20:13:29.000000 quickstats-0.7.0.4.1/quickstats/components/analysis_object.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     7330 2024-02-09 19:22:50.000000 quickstats-0.7.0.4.1/quickstats/components/asimov_generator.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    31508 2024-03-02 09:26:25.000000 quickstats-0.7.0.4.1/quickstats/components/asymptotic_cls.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     3273 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/components/basics.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     3156 2024-02-09 19:22:50.000000 quickstats-0.7.0.4.1/quickstats/components/caching_nll_wrapper.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    10479 2024-03-02 09:26:25.000000 quickstats-0.7.0.4.1/quickstats/components/discrete_nuisance.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    56823 2024-04-02 16:59:53.000000 quickstats-0.7.0.4.1/quickstats/components/extended_minimizer.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)   105095 2024-03-02 09:26:25.000000 quickstats-0.7.0.4.1/quickstats/components/extended_model.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     5859 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/quickstats/components/extended_rfile.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    14097 2024-04-24 19:51:22.000000 quickstats-0.7.0.4.1/quickstats/components/likelihood.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:26.937115 quickstats-0.7.0.4.1/quickstats/components/modelling/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      207 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/components/modelling/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     2504 2024-02-09 19:22:51.000000 quickstats-0.7.0.4.1/quickstats/components/modelling/component_source.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    20116 2024-04-02 16:59:53.000000 quickstats-0.7.0.4.1/quickstats/components/modelling/data_modelling.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      735 2024-02-09 19:22:51.000000 quickstats-0.7.0.4.1/quickstats/components/modelling/model_source.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     4502 2024-02-09 19:22:51.000000 quickstats-0.7.0.4.1/quickstats/components/modelling/parameter_templates.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     5550 2024-02-09 19:22:51.000000 quickstats-0.7.0.4.1/quickstats/components/modelling/pdf_fit_tool.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     3483 2024-02-09 19:22:51.000000 quickstats-0.7.0.4.1/quickstats/components/modelling/tree_data_source.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    10864 2024-02-09 19:22:51.000000 quickstats-0.7.0.4.1/quickstats/components/nuisance_parameter_harmonizer.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    17594 2024-02-09 19:22:51.000000 quickstats-0.7.0.4.1/quickstats/components/nuisance_parameter_pull.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    12380 2024-04-02 16:59:53.000000 quickstats-0.7.0.4.1/quickstats/components/nuisance_parameter_ranking.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:26.939383 quickstats-0.7.0.4.1/quickstats/components/processors/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      111 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/quickstats/components/processors/__init__.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:26.960140 quickstats-0.7.0.4.1/quickstats/components/processors/actions/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1457 2024-04-24 09:12:07.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      388 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/auxiliary.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      358 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/formatter.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1608 2024-04-16 12:24:10.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_alias.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     2360 2024-04-24 10:06:22.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_as_hdf.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     2037 2024-04-24 10:03:17.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_as_numpy.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1589 2024-04-24 09:17:14.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_as_parquet.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     4421 2024-04-16 12:43:49.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_base_action.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1049 2024-04-24 09:24:54.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_cache.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      866 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_declare.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1826 2024-04-16 13:51:20.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_define.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1228 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_export.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1903 2024-04-23 13:39:48.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_filter.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1331 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_global_variables.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      506 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_helper_action.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      586 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_hybrid_action.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      755 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_if_defined.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      763 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_if_not_defined.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      726 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_load_frame.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1211 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_load_macro.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      226 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_max.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      225 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_mean.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      226 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_min.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      636 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_nested_action.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     2249 2024-04-24 09:49:14.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_output_action.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      757 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_progressbar.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      462 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_rdf_action.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      481 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_redefine.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1854 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_report.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      723 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_safe_alias.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      539 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_safe_define.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1770 2024-04-24 09:17:06.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_save.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      735 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_save_frame.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1433 2024-04-16 12:24:30.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_stat.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      226 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_sum.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      606 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_treename.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    13111 2024-03-22 01:36:00.000000 quickstats-0.7.0.4.1/quickstats/components/processors/builtin_methods.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    12481 2024-04-23 14:29:19.000000 quickstats-0.7.0.4.1/quickstats/components/processors/roo_process_config.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    13843 2024-05-18 08:17:55.000000 quickstats-0.7.0.4.1/quickstats/components/processors/roo_processor.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     5406 2024-02-09 19:22:51.000000 quickstats-0.7.0.4.1/quickstats/components/pvalue_toys.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     2978 2024-04-02 17:06:13.000000 quickstats-0.7.0.4.1/quickstats/components/roo_inspector.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     3103 2024-02-09 19:22:51.000000 quickstats-0.7.0.4.1/quickstats/components/root_object.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    21325 2024-02-09 19:22:51.000000 quickstats-0.7.0.4.1/quickstats/components/toy_limit_calculator.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:26.968482 quickstats-0.7.0.4.1/quickstats/components/workspaces/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      591 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/components/workspaces/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     9877 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/components/workspaces/asimov_handler.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1727 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/components/workspaces/core_argument_sets.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1997 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/components/workspaces/sample.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1991 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/components/workspaces/settings.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     8910 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/components/workspaces/systematic.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     2303 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/components/workspaces/systematics_domain.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    53148 2024-04-02 16:59:53.000000 quickstats-0.7.0.4.1/quickstats/components/workspaces/ws_comparer.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     8787 2024-04-02 16:59:53.000000 quickstats-0.7.0.4.1/quickstats/components/workspaces/ws_decomposer.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1724 2024-02-09 19:22:51.000000 quickstats-0.7.0.4.1/quickstats/components/workspaces/ws_modifier_config.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    10827 2024-02-09 19:22:51.000000 quickstats-0.7.0.4.1/quickstats/components/workspaces/xml_ws_base.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    87015 2024-02-09 19:22:51.000000 quickstats-0.7.0.4.1/quickstats/components/workspaces/xml_ws_builder_v1.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    76446 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/quickstats/components/workspaces/xml_ws_builder_v2.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    52888 2024-04-02 16:59:53.000000 quickstats-0.7.0.4.1/quickstats/components/workspaces/xml_ws_combiner.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    55314 2024-04-02 16:59:53.000000 quickstats-0.7.0.4.1/quickstats/components/workspaces/xml_ws_modifier.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:26.972246 quickstats-0.7.0.4.1/quickstats/concurrent/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      372 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/concurrent/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     4197 2024-04-02 17:05:55.000000 quickstats-0.7.0.4.1/quickstats/concurrent/abstract_runner.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      627 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/concurrent/logging.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     5209 2024-03-22 01:36:00.000000 quickstats-0.7.0.4.1/quickstats/concurrent/nuisance_parameter_ranking_runner.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     5285 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/concurrent/parameterised_asymptotic_cls.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    10852 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/concurrent/parameterised_likelihood.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     5822 2024-03-22 01:36:00.000000 quickstats-0.7.0.4.1/quickstats/concurrent/parameterised_runner.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     7694 2024-04-18 14:43:04.000000 quickstats-0.7.0.4.1/quickstats/concurrent/parameterised_significance.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:26.978946 quickstats-0.7.0.4.1/quickstats/core/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      411 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/core/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      783 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/core/abstract_object.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    32252 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/core/configuration.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     4546 2024-04-02 16:59:53.000000 quickstats-0.7.0.4.1/quickstats/core/constraints.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     4603 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/core/decorators.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     7569 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/core/enums.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     7707 2024-04-24 20:19:23.000000 quickstats-0.7.0.4.1/quickstats/core/io.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     2106 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/core/metaclasses.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     7624 2024-04-16 04:59:38.000000 quickstats-0.7.0.4.1/quickstats/core/methods.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    18907 2024-05-27 11:31:30.000000 quickstats-0.7.0.4.1/quickstats/core/path_manager.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      721 2024-04-02 16:59:53.000000 quickstats-0.7.0.4.1/quickstats/core/setup.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     6584 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/core/type_validation.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     3895 2024-03-29 08:37:19.000000 quickstats-0.7.0.4.1/quickstats/core/virtual_trees.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:26.980869 quickstats-0.7.0.4.1/quickstats/daq/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      151 2024-04-23 12:17:50.000000 quickstats-0.7.0.4.1/quickstats/daq/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     6933 2024-04-23 13:26:47.000000 quickstats-0.7.0.4.1/quickstats/daq/remote_data_source.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     3849 2024-04-23 14:31:53.000000 quickstats-0.7.0.4.1/quickstats/daq/servicex_source.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     2553 2024-04-23 14:41:51.000000 quickstats-0.7.0.4.1/quickstats/daq/xrootd_source.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:26.981970 quickstats-0.7.0.4.1/quickstats/extensions/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)       85 2024-03-22 01:36:00.000000 quickstats-0.7.0.4.1/quickstats/extensions/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     4147 2024-03-22 01:36:00.000000 quickstats-0.7.0.4.1/quickstats/extensions/extension_dataframe.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:26.982444 quickstats-0.7.0.4.1/quickstats/interface/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/quickstats/interface/__init__.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:26.984832 quickstats-0.7.0.4.1/quickstats/interface/cppyy/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      198 2024-04-15 04:00:33.000000 quickstats-0.7.0.4.1/quickstats/interface/cppyy/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      392 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/interface/cppyy/basic_methods.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      513 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/interface/cppyy/core.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    12794 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/interface/cppyy/macros.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     4540 2024-02-09 19:22:51.000000 quickstats-0.7.0.4.1/quickstats/interface/cppyy/vectorize.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:26.985819 quickstats-0.7.0.4.1/quickstats/interface/kerberos/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      109 2024-04-15 21:52:35.000000 quickstats-0.7.0.4.1/quickstats/interface/kerberos/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1709 2024-04-15 21:56:47.000000 quickstats-0.7.0.4.1/quickstats/interface/kerberos/core.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:26.998660 quickstats-0.7.0.4.1/quickstats/interface/root/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     3819 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/interface/root/ModelConfig.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    10737 2024-04-24 09:58:20.000000 quickstats-0.7.0.4.1/quickstats/interface/root/RDataFrame.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     2306 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/interface/root/RooAbsArg.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      621 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/interface/root/RooAbsData.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    21668 2024-02-09 19:22:51.000000 quickstats-0.7.0.4.1/quickstats/interface/root/RooAbsPdf.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     3531 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/interface/root/RooArgSet.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1182 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/interface/root/RooCategory.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    44967 2024-02-09 19:22:51.000000 quickstats-0.7.0.4.1/quickstats/interface/root/RooDataSet.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      588 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/interface/root/RooMsgService.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     6728 2024-02-09 19:22:51.000000 quickstats-0.7.0.4.1/quickstats/interface/root/RooRealVar.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      130 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/interface/root/TArrayData.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     2905 2024-03-22 01:36:00.000000 quickstats-0.7.0.4.1/quickstats/interface/root/TChain.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      983 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/interface/root/TF1.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    11390 2024-04-23 03:24:44.000000 quickstats-0.7.0.4.1/quickstats/interface/root/TFile.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    13146 2024-02-09 19:22:51.000000 quickstats-0.7.0.4.1/quickstats/interface/root/TH1.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     5813 2024-04-19 22:59:06.000000 quickstats-0.7.0.4.1/quickstats/interface/root/TH2.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     6043 2024-04-19 22:51:24.000000 quickstats-0.7.0.4.1/quickstats/interface/root/TH3.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      378 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/quickstats/interface/root/TObject.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      748 2024-04-16 04:58:25.000000 quickstats-0.7.0.4.1/quickstats/interface/root/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1069 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/interface/root/helper.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      235 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/interface/root/io.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    27713 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/interface/root/macros.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     5634 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/interface/root/roofit_extension.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:27.000214 quickstats-0.7.0.4.1/quickstats/interface/servicex/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      163 2024-04-22 09:59:18.000000 quickstats-0.7.0.4.1/quickstats/interface/servicex/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     5409 2024-04-24 08:55:03.000000 quickstats-0.7.0.4.1/quickstats/interface/servicex/config.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     2872 2024-04-24 09:30:06.000000 quickstats-0.7.0.4.1/quickstats/interface/servicex/core.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:27.001247 quickstats-0.7.0.4.1/quickstats/interface/tinydb/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)       67 2024-04-24 07:55:07.000000 quickstats-0.7.0.4.1/quickstats/interface/tinydb/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      947 2024-04-24 08:54:00.000000 quickstats-0.7.0.4.1/quickstats/interface/tinydb/methods.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:27.003988 quickstats-0.7.0.4.1/quickstats/interface/xrootd/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      149 2024-04-16 06:14:52.000000 quickstats-0.7.0.4.1/quickstats/interface/xrootd/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      448 2024-04-15 05:41:21.000000 quickstats-0.7.0.4.1/quickstats/interface/xrootd/core.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     5850 2024-04-23 03:15:06.000000 quickstats-0.7.0.4.1/quickstats/interface/xrootd/filesystem.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1163 2024-04-23 03:14:39.000000 quickstats-0.7.0.4.1/quickstats/interface/xrootd/path.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     2573 2024-04-23 07:02:17.000000 quickstats-0.7.0.4.1/quickstats/interface/xrootd/xrd_helper.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:26.897614 quickstats-0.7.0.4.1/quickstats/macros/
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:27.005306 quickstats-0.7.0.4.1/quickstats/macros/AsymptoticCLsTool/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     7366 2024-02-09 19:22:51.000000 quickstats-0.7.0.4.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1591 2024-02-09 19:22:51.000000 quickstats-0.7.0.4.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:27.010429 quickstats-0.7.0.4.1/quickstats/macros/FlexibleInterpVarMkII/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    12372 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     2498 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:27.012707 quickstats-0.7.0.4.1/quickstats/macros/QuickStatsCore/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     3133 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/macros/QuickStatsCore/QStringUtils.cxx
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1259 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    10312 2024-02-23 18:55:02.000000 quickstats-0.7.0.4.1/quickstats/macros/QuickStatsCore/RooFitExt.cxx
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     3868 2024-02-23 18:55:02.000000 quickstats-0.7.0.4.1/quickstats/macros/QuickStatsCore/RooFitExt.h
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:27.013826 quickstats-0.7.0.4.1/quickstats/macros/ResponseFunction/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    13749 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/quickstats/macros/ResponseFunction/ResponseFunction.cxx
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     2982 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/macros/ResponseFunction/ResponseFunction.h
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:27.014890 quickstats-0.7.0.4.1/quickstats/macros/RooTwoSidedCBShape/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     3689 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1358 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:27.018848 quickstats-0.7.0.4.1/quickstats/maths/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/maths/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     4366 2024-03-22 01:36:00.000000 quickstats-0.7.0.4.1/quickstats/maths/interpolation.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    10394 2024-05-21 06:21:31.000000 quickstats-0.7.0.4.1/quickstats/maths/numerics.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    40281 2024-04-18 13:39:14.000000 quickstats-0.7.0.4.1/quickstats/maths/statistics.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     3506 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/maths/statistics_jitted.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      613 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/maths/symbolics.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:27.027959 quickstats-0.7.0.4.1/quickstats/parsers/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      187 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/parsers/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      337 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/parsers/config_parser.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    16764 2024-02-09 19:22:51.000000 quickstats-0.7.0.4.1/quickstats/parsers/param_parser.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     5204 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/parsers/roo_param_setup_parser.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:27.044992 quickstats-0.7.0.4.1/quickstats/plots/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1345 2024-03-22 01:36:00.000000 quickstats-0.7.0.4.1/quickstats/plots/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    27356 2024-05-07 03:52:59.000000 quickstats-0.7.0.4.1/quickstats/plots/abstract_plot.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     5196 2024-04-16 21:04:46.000000 quickstats-0.7.0.4.1/quickstats/plots/bar_chart.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    14144 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/plots/bidirectional_bar_chart.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1634 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/plots/collective_data_plot.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     3467 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/quickstats/plots/color_schemes.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     6579 2024-04-30 03:37:06.000000 quickstats-0.7.0.4.1/quickstats/plots/core.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     4951 2024-02-09 19:22:51.000000 quickstats-0.7.0.4.1/quickstats/plots/correlation_plot.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     7791 2024-04-26 23:31:28.000000 quickstats-0.7.0.4.1/quickstats/plots/general_1D_plot.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     4061 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/plots/general_2D_plot.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    22203 2024-04-17 08:14:07.000000 quickstats-0.7.0.4.1/quickstats/plots/general_distribution_plot.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     6078 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/plots/hypotest_inverter_plot.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     8981 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/plots/likelihood_1D_plot.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    16926 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/plots/likelihood_2D_plot.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    29155 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/plots/np_ranking_plot.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    25684 2024-04-17 08:14:13.000000 quickstats-0.7.0.4.1/quickstats/plots/pdf_distribution_plot.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     5096 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/plots/sample_purity_plot.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    10353 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/plots/score_distribution_plot.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     4122 2024-02-09 19:22:51.000000 quickstats-0.7.0.4.1/quickstats/plots/stat_plot_config.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    30687 2024-04-30 14:14:10.000000 quickstats-0.7.0.4.1/quickstats/plots/template.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    13785 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/plots/test_statistic_distribution_plot.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     5122 2024-03-22 01:36:00.000000 quickstats-0.7.0.4.1/quickstats/plots/two_axis_1D_plot.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     9999 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/plots/upper_limit_1D_plot.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    19292 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/plots/upper_limit_2D_plot.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    13182 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/plots/upper_limit_3D_plot.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    23227 2024-04-25 09:01:39.000000 quickstats-0.7.0.4.1/quickstats/plots/upper_limit_benchmark_plot.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    34456 2024-05-28 15:16:37.000000 quickstats-0.7.0.4.1/quickstats/plots/variable_distribution_plot.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:27.045601 quickstats-0.7.0.4.1/quickstats/resources/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)       90 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/resources/default_workspace_extensions.json
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:27.047202 quickstats-0.7.0.4.1/quickstats/resources/mpl_stylesheets/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      379 2024-03-22 01:36:00.000000 quickstats-0.7.0.4.1/quickstats/resources/mpl_stylesheets/hep.mplstyle
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2024-03-22 01:36:00.000000 quickstats-0.7.0.4.1/quickstats/resources/mpl_stylesheets/no_latex.mplstyle
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      325 2024-03-22 01:36:00.000000 quickstats-0.7.0.4.1/quickstats/resources/mpl_stylesheets/science.mplstyle
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     4604 2024-02-23 18:55:02.000000 quickstats-0.7.0.4.1/quickstats/root_checker.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:27.055823 quickstats-0.7.0.4.1/quickstats/utils/
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2024-03-22 01:35:33.000000 quickstats-0.7.0.4.1/quickstats/utils/__init__.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    19773 2024-04-23 05:00:30.000000 quickstats-0.7.0.4.1/quickstats/utils/common_utils.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)        0 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/utils/condor_tasks.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    18666 2024-04-19 21:42:21.000000 quickstats-0.7.0.4.1/quickstats/utils/data_conversion.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1187 2023-10-16 18:13:04.000000 quickstats-0.7.0.4.1/quickstats/utils/hep_utils.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     3039 2024-04-23 10:35:13.000000 quickstats-0.7.0.4.1/quickstats/utils/path_utils.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)      563 2024-03-29 07:47:20.000000 quickstats-0.7.0.4.1/quickstats/utils/py_utils.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    27521 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/utils/roofit_utils.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    10914 2024-02-09 19:22:51.000000 quickstats-0.7.0.4.1/quickstats/utils/roostats_utils.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    15330 2024-04-19 21:42:42.000000 quickstats-0.7.0.4.1/quickstats/utils/root_utils.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    15638 2024-04-16 13:51:02.000000 quickstats-0.7.0.4.1/quickstats/utils/string_utils.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     2321 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/utils/sys_utils.py
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    15128 2024-04-15 03:46:28.000000 quickstats-0.7.0.4.1/quickstats/utils/xml_tools.py
+drwxrwx---   0 chlcheng (102623) chlcheng (102623)        0 2024-05-28 15:23:26.905492 quickstats-0.7.0.4.1/quickstats.egg-info/
+-rw-r--r--   0 chlcheng (102623) chlcheng (102623)     4127 2024-05-28 15:23:26.903729 quickstats-0.7.0.4.1/quickstats.egg-info/PKG-INFO
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)    11098 2024-05-28 15:23:26.904286 quickstats-0.7.0.4.1/quickstats.egg-info/SOURCES.txt
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)        1 2024-05-28 15:23:26.904725 quickstats-0.7.0.4.1/quickstats.egg-info/dependency_links.txt
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)       39 2024-05-28 15:23:26.905139 quickstats-0.7.0.4.1/quickstats.egg-info/requires.txt
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)       11 2024-05-28 15:23:26.905571 quickstats-0.7.0.4.1/quickstats.egg-info/top_level.txt
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)       38 2024-05-28 15:23:27.057393 quickstats-0.7.0.4.1/setup.cfg
+-rw-rw----   0 chlcheng (102623) chlcheng (102623)     1771 2024-03-27 08:35:59.000000 quickstats-0.7.0.4.1/setup.py
```

### Comparing `quickstats-0.7.0.4/PKG-INFO` & `quickstats-0.7.0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.7.0.4
+Version: 0.7.0.4.1
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.7.0.4/README.md` & `quickstats-0.7.0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/algorithms/nll_crossing/BaseMethod.py` & `quickstats-0.7.0.4.1/quickstats/algorithms/nll_crossing/BaseMethod.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/analysis/analysis_base.py` & `quickstats-0.7.0.4.1/quickstats/analysis/analysis_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,22 +90,21 @@
             basename = os.path.basename(os.path.dirname(model_dir))
             if basename != study_name:
                 model_dir = os.path.join(model_dir, study_name)
                 self.path_manager.set_directory("model", model_dir)
         
     def get_study_name(self):
         return self.path_manager.study_name
-    
-    def get_directory(self, directory_name:str):
-        return self.path_manager.get_directory(directory_name)
+
+    # TODO: remove these methods
+    def get_directory(self, directory_name:str, validate:bool=False, **parameters):
+        return self.path_manager.get_directory(directory_name, check_exist=validate, **parameters)
     
     def get_file(self, file_name:str, validate:bool=False, **parameters):
-        if validate:
-            self._check_file(file_name, **parameters)
-        return self.path_manager.get_resolved_file(file_name, **parameters)
+        return self.path_manager.get_file(file_name, check_exist=validate, **parameters)
     
     def _has_directory(self, directory_name:str):
         return self.path_manager.directory_exists(directory_name)
     
     def _has_file(self, file_name:str, **parameters):
         return self.path_manager.file_exists(file_name, **parameters)
```

### Comparing `quickstats-0.7.0.4/quickstats/analysis/analysis_path_manager.py` & `quickstats-0.7.0.4.1/quickstats/analysis/analysis_path_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,17 +46,15 @@
         "likelihood_summary"                       : ("summary", "likelihood_summary.json"),
         "benchmark_significance"                   : ("summary", "benchmark_significance.json")
     }
     
     def __init__(self, study_name:Optional[str]=None, base_path:Optional[str]=None,
                  directories:Optional[Dict[str, str]]=None,
                  files:Optional[Dict[str, Union[str, Tuple[Optional[str], str]]]]=None):
-        
-        directories = combine_dict(self.DEFAULT_DIRECTORIES, directories)
-        files       = combine_dict(self.DEFAULT_FILES, files)
+
         super().__init__(base_path=base_path, directories=directories, files=files)
         
         self.study_name    = study_name
         self.base_path     = base_path
         self.update()
 
     def get_base_path(self):
```

### Comparing `quickstats-0.7.0.4/quickstats/analysis/config_templates.py` & `quickstats-0.7.0.4.1/quickstats/analysis/config_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/analysis/data_loading.py` & `quickstats-0.7.0.4.1/quickstats/analysis/data_loading.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/analysis/data_preprocessing.py` & `quickstats-0.7.0.4.1/quickstats/analysis/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/analysis/event_categorization.py` & `quickstats-0.7.0.4.1/quickstats/analysis/event_categorization.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/analysis/multi_class_boundary_tree.py` & `quickstats-0.7.0.4.1/quickstats/analysis/multi_class_boundary_tree.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/analysis/ntuple_conversion_tool.py` & `quickstats-0.7.0.4.1/quickstats/analysis/ntuple_conversion_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/analysis/ntuple_process_tool.py` & `quickstats-0.7.0.4.1/quickstats/analysis/ntuple_process_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/analysis/sample_poly_param_tool.py` & `quickstats-0.7.0.4.1/quickstats/analysis/sample_poly_param_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/analysis/systematics/base_systematics.py` & `quickstats-0.7.0.4.1/quickstats/analysis/systematics/base_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/analysis/systematics/gaussian_shape_systematics.py` & `quickstats-0.7.0.4.1/quickstats/analysis/systematics/gaussian_shape_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/analysis/systematics/normalization_systematics.py` & `quickstats-0.7.0.4.1/quickstats/analysis/systematics/normalization_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/analysis/systematics/systematics_evaluation_tool.py` & `quickstats-0.7.0.4.1/quickstats/analysis/systematics/systematics_evaluation_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/clis/core.py` & `quickstats-0.7.0.4.1/quickstats/clis/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/clis/inspect_rfile.py` & `quickstats-0.7.0.4.1/quickstats/clis/inspect_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/clis/likelihood_tools.py` & `quickstats-0.7.0.4.1/quickstats/clis/likelihood_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/clis/limit_setting.py` & `quickstats-0.7.0.4.1/quickstats/clis/limit_setting.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/clis/nuisance_parameter_tools.py` & `quickstats-0.7.0.4.1/quickstats/clis/nuisance_parameter_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/clis/processor_tools.py` & `quickstats-0.7.0.4.1/quickstats/clis/processor_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/clis/stat_tools.py` & `quickstats-0.7.0.4.1/quickstats/clis/stat_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/clis/workspace_tools.py` & `quickstats-0.7.0.4.1/quickstats/clis/workspace_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/__init__.py` & `quickstats-0.7.0.4.1/quickstats/components/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/analysis_base.py` & `quickstats-0.7.0.4.1/quickstats/components/analysis_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/analysis_object.py` & `quickstats-0.7.0.4.1/quickstats/components/analysis_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/asimov_generator.py` & `quickstats-0.7.0.4.1/quickstats/components/asimov_generator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/asymptotic_cls.py` & `quickstats-0.7.0.4.1/quickstats/components/asymptotic_cls.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/basics.py` & `quickstats-0.7.0.4.1/quickstats/components/basics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/caching_nll_wrapper.py` & `quickstats-0.7.0.4.1/quickstats/components/caching_nll_wrapper.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/discrete_nuisance.py` & `quickstats-0.7.0.4.1/quickstats/components/discrete_nuisance.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/extended_minimizer.py` & `quickstats-0.7.0.4.1/quickstats/components/extended_minimizer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/extended_model.py` & `quickstats-0.7.0.4.1/quickstats/components/extended_model.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/extended_rfile.py` & `quickstats-0.7.0.4.1/quickstats/components/extended_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/likelihood.py` & `quickstats-0.7.0.4.1/quickstats/components/likelihood.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/modelling/component_source.py` & `quickstats-0.7.0.4.1/quickstats/components/modelling/component_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/modelling/data_modelling.py` & `quickstats-0.7.0.4.1/quickstats/components/modelling/data_modelling.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/modelling/model_source.py` & `quickstats-0.7.0.4.1/quickstats/components/modelling/model_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/modelling/parameter_templates.py` & `quickstats-0.7.0.4.1/quickstats/components/modelling/parameter_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/modelling/pdf_fit_tool.py` & `quickstats-0.7.0.4.1/quickstats/components/modelling/pdf_fit_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/modelling/tree_data_source.py` & `quickstats-0.7.0.4.1/quickstats/components/modelling/tree_data_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/nuisance_parameter_harmonizer.py` & `quickstats-0.7.0.4.1/quickstats/components/nuisance_parameter_harmonizer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/nuisance_parameter_pull.py` & `quickstats-0.7.0.4.1/quickstats/components/nuisance_parameter_pull.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/nuisance_parameter_ranking.py` & `quickstats-0.7.0.4.1/quickstats/components/nuisance_parameter_ranking.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/__init__.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_alias.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_alias.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_as_hdf.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_as_hdf.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_as_numpy.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_as_numpy.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_as_parquet.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_as_parquet.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_base_action.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_base_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_cache.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_cache.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_declare.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_declare.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_define.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_define.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_export.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_export.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_filter.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_filter.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_global_variables.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_global_variables.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_hybrid_action.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_hybrid_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_if_defined.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_if_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_if_not_defined.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_if_not_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_load_frame.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_load_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_load_macro.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_load_macro.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_nested_action.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_nested_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_output_action.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_output_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_progressbar.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_progressbar.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_report.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_report.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_safe_alias.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_safe_alias.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_safe_define.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_safe_define.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_save.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_save.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_save_frame.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_save_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_stat.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_stat.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/actions/rooproc_treename.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/actions/rooproc_treename.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/builtin_methods.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/builtin_methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/roo_process_config.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/roo_process_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/processors/roo_processor.py` & `quickstats-0.7.0.4.1/quickstats/components/processors/roo_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import time
 import ROOT
 
 from .builtin_methods import BUILTIN_METHODS
 from .actions import *
 from .roo_process_config import RooProcessConfig
 
-from quickstats import timer, AbstractObject, PathManager, GeneralEnum, module_exist
+from quickstats import timer, AbstractObject, GeneralEnum, module_exist
 from quickstats.interface.root import TFile, RDataFrame, RDataFrameBackend
 from quickstats.interface.xrootd import get_cachedir, set_cachedir, switch_cachedir
 from quickstats.utils.root_utils import declare_expression, close_all_root_files, set_multithread
 from quickstats.utils.path_utils import is_remote_path
 from quickstats.utils.common_utils import get_cpu_count, combine_dict
 from quickstats.daq import DEFAULT_CACHE_DIR, XRootDSource, ServiceXSource
```

### Comparing `quickstats-0.7.0.4/quickstats/components/pvalue_toys.py` & `quickstats-0.7.0.4.1/quickstats/components/pvalue_toys.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/roo_inspector.py` & `quickstats-0.7.0.4.1/quickstats/components/roo_inspector.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/root_object.py` & `quickstats-0.7.0.4.1/quickstats/components/root_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/toy_limit_calculator.py` & `quickstats-0.7.0.4.1/quickstats/components/toy_limit_calculator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/workspaces/__init__.py` & `quickstats-0.7.0.4.1/quickstats/components/workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/workspaces/asimov_handler.py` & `quickstats-0.7.0.4.1/quickstats/components/workspaces/asimov_handler.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/workspaces/core_argument_sets.py` & `quickstats-0.7.0.4.1/quickstats/components/workspaces/core_argument_sets.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/workspaces/sample.py` & `quickstats-0.7.0.4.1/quickstats/components/workspaces/sample.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/workspaces/settings.py` & `quickstats-0.7.0.4.1/quickstats/components/workspaces/settings.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/workspaces/systematic.py` & `quickstats-0.7.0.4.1/quickstats/components/workspaces/systematic.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/workspaces/systematics_domain.py` & `quickstats-0.7.0.4.1/quickstats/components/workspaces/systematics_domain.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/workspaces/ws_comparer.py` & `quickstats-0.7.0.4.1/quickstats/components/workspaces/ws_comparer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/workspaces/ws_decomposer.py` & `quickstats-0.7.0.4.1/quickstats/components/workspaces/ws_decomposer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/workspaces/ws_modifier_config.py` & `quickstats-0.7.0.4.1/quickstats/components/workspaces/ws_modifier_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/workspaces/xml_ws_base.py` & `quickstats-0.7.0.4.1/quickstats/components/workspaces/xml_ws_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/workspaces/xml_ws_builder_v1.py` & `quickstats-0.7.0.4.1/quickstats/components/workspaces/xml_ws_builder_v1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/workspaces/xml_ws_builder_v2.py` & `quickstats-0.7.0.4.1/quickstats/components/workspaces/xml_ws_builder_v2.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/workspaces/xml_ws_combiner.py` & `quickstats-0.7.0.4.1/quickstats/components/workspaces/xml_ws_combiner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/components/workspaces/xml_ws_modifier.py` & `quickstats-0.7.0.4.1/quickstats/components/workspaces/xml_ws_modifier.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/concurrent/abstract_runner.py` & `quickstats-0.7.0.4.1/quickstats/concurrent/abstract_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/concurrent/logging.py` & `quickstats-0.7.0.4.1/quickstats/concurrent/logging.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/concurrent/nuisance_parameter_ranking_runner.py` & `quickstats-0.7.0.4.1/quickstats/concurrent/nuisance_parameter_ranking_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/concurrent/parameterised_asymptotic_cls.py` & `quickstats-0.7.0.4.1/quickstats/concurrent/parameterised_asymptotic_cls.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/concurrent/parameterised_likelihood.py` & `quickstats-0.7.0.4.1/quickstats/concurrent/parameterised_likelihood.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/concurrent/parameterised_runner.py` & `quickstats-0.7.0.4.1/quickstats/concurrent/parameterised_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/concurrent/parameterised_significance.py` & `quickstats-0.7.0.4.1/quickstats/concurrent/parameterised_significance.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/core/abstract_object.py` & `quickstats-0.7.0.4.1/quickstats/core/abstract_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/core/configuration.py` & `quickstats-0.7.0.4.1/quickstats/core/configuration.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/core/constraints.py` & `quickstats-0.7.0.4.1/quickstats/core/constraints.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/core/decorators.py` & `quickstats-0.7.0.4.1/quickstats/core/decorators.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/core/enums.py` & `quickstats-0.7.0.4.1/quickstats/core/enums.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/core/io.py` & `quickstats-0.7.0.4.1/quickstats/core/io.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/core/metaclasses.py` & `quickstats-0.7.0.4.1/quickstats/core/metaclasses.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/core/methods.py` & `quickstats-0.7.0.4.1/quickstats/core/methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/core/setup.py` & `quickstats-0.7.0.4.1/quickstats/core/setup.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/core/type_validation.py` & `quickstats-0.7.0.4.1/quickstats/core/type_validation.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/core/virtual_trees.py` & `quickstats-0.7.0.4.1/quickstats/core/virtual_trees.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/daq/remote_data_source.py` & `quickstats-0.7.0.4.1/quickstats/daq/remote_data_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/daq/servicex_source.py` & `quickstats-0.7.0.4.1/quickstats/daq/servicex_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/daq/xrootd_source.py` & `quickstats-0.7.0.4.1/quickstats/daq/xrootd_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/extensions/extension_dataframe.py` & `quickstats-0.7.0.4.1/quickstats/extensions/extension_dataframe.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/cppyy/core.py` & `quickstats-0.7.0.4.1/quickstats/interface/cppyy/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/cppyy/macros.py` & `quickstats-0.7.0.4.1/quickstats/interface/cppyy/macros.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/cppyy/vectorize.py` & `quickstats-0.7.0.4.1/quickstats/interface/cppyy/vectorize.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/kerberos/core.py` & `quickstats-0.7.0.4.1/quickstats/interface/kerberos/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/root/ModelConfig.py` & `quickstats-0.7.0.4.1/quickstats/interface/root/ModelConfig.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/root/RDataFrame.py` & `quickstats-0.7.0.4.1/quickstats/interface/root/RDataFrame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/root/RooAbsArg.py` & `quickstats-0.7.0.4.1/quickstats/interface/root/RooAbsArg.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/root/RooAbsData.py` & `quickstats-0.7.0.4.1/quickstats/interface/root/RooAbsData.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/root/RooAbsPdf.py` & `quickstats-0.7.0.4.1/quickstats/interface/root/RooAbsPdf.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/root/RooArgSet.py` & `quickstats-0.7.0.4.1/quickstats/interface/root/RooArgSet.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/root/RooCategory.py` & `quickstats-0.7.0.4.1/quickstats/interface/root/RooCategory.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/root/RooDataSet.py` & `quickstats-0.7.0.4.1/quickstats/interface/root/RooDataSet.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/root/RooMsgService.py` & `quickstats-0.7.0.4.1/quickstats/interface/root/RooMsgService.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/root/RooRealVar.py` & `quickstats-0.7.0.4.1/quickstats/interface/root/RooRealVar.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/root/TChain.py` & `quickstats-0.7.0.4.1/quickstats/interface/root/TChain.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/root/TF1.py` & `quickstats-0.7.0.4.1/quickstats/interface/root/TF1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/root/TFile.py` & `quickstats-0.7.0.4.1/quickstats/interface/root/TFile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/root/TH1.py` & `quickstats-0.7.0.4.1/quickstats/interface/root/TH1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/root/TH2.py` & `quickstats-0.7.0.4.1/quickstats/interface/root/TH2.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/root/TH3.py` & `quickstats-0.7.0.4.1/quickstats/interface/root/TH3.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/root/__init__.py` & `quickstats-0.7.0.4.1/quickstats/interface/root/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/root/helper.py` & `quickstats-0.7.0.4.1/quickstats/interface/root/helper.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/root/macros.py` & `quickstats-0.7.0.4.1/quickstats/interface/root/macros.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/root/roofit_extension.py` & `quickstats-0.7.0.4.1/quickstats/interface/root/roofit_extension.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/servicex/config.py` & `quickstats-0.7.0.4.1/quickstats/interface/servicex/config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/servicex/core.py` & `quickstats-0.7.0.4.1/quickstats/interface/servicex/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/tinydb/methods.py` & `quickstats-0.7.0.4.1/quickstats/interface/tinydb/methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/xrootd/filesystem.py` & `quickstats-0.7.0.4.1/quickstats/interface/xrootd/filesystem.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/xrootd/path.py` & `quickstats-0.7.0.4.1/quickstats/interface/xrootd/path.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/interface/xrootd/xrd_helper.py` & `quickstats-0.7.0.4.1/quickstats/interface/xrootd/xrd_helper.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx` & `quickstats-0.7.0.4.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h` & `quickstats-0.7.0.4.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx` & `quickstats-0.7.0.4.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h` & `quickstats-0.7.0.4.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/macros/QuickStatsCore/QStringUtils.cxx` & `quickstats-0.7.0.4.1/quickstats/macros/QuickStatsCore/QStringUtils.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx` & `quickstats-0.7.0.4.1/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/macros/QuickStatsCore/RooFitExt.cxx` & `quickstats-0.7.0.4.1/quickstats/macros/QuickStatsCore/RooFitExt.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/macros/QuickStatsCore/RooFitExt.h` & `quickstats-0.7.0.4.1/quickstats/macros/QuickStatsCore/RooFitExt.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/macros/ResponseFunction/ResponseFunction.cxx` & `quickstats-0.7.0.4.1/quickstats/macros/ResponseFunction/ResponseFunction.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/macros/ResponseFunction/ResponseFunction.h` & `quickstats-0.7.0.4.1/quickstats/macros/ResponseFunction/ResponseFunction.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx` & `quickstats-0.7.0.4.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h` & `quickstats-0.7.0.4.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/maths/interpolation.py` & `quickstats-0.7.0.4.1/quickstats/maths/interpolation.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/maths/numerics.py` & `quickstats-0.7.0.4.1/quickstats/maths/numerics.py`

 * *Files 10% similar despite different names*

```diff
@@ -207,22 +207,27 @@
     la = len(arrays)
     dtype = np.result_type(*arrays)
     arr = np.empty([len(a) for a in arrays] + [la], dtype=dtype)
     for i, a in enumerate(np.ix_(*arrays)):
         arr[...,i] = a
     return arr.reshape(-1, la)
 
-def get_mask(x, conditions:List[Union[Tuple[float, float], Callable]]=None):
-    mask = np.full(x.shape, False)
+def get_mask(*x, conditions:List[Union[Tuple[float, float], Callable]]=None):
+    assert len(x) > 0
+    mask = np.full(x[0].shape, False)
     for condition in conditions:
-        if isinstance(condition, (tuple, list)):
+        if isinstance(condition, tuple):
             xmin, xmax = condition
-            mask |= ((x > xmin) & (x < xmax))
+            mask |= ((x[0] > xmin) & (x[0] < xmax))
+        elif isinstance(condition, list):
+            for i, condition_i in enumerate(condition):
+                xmin, xmax = condition_i
+                mask |= ((x[i] > xmin) & (x[i] < xmax))
         else:
-            mask |= np.array(list(map(condition, x)))
+            mask |= np.array(list(map(condition, *x)))
     return mask
 
 def get_subsequences(arr, mask, min_length=1):
     """
     Finds and returns continuous subsequences of an array where the mask is True.
     
     Parameters:
@@ -256,8 +261,42 @@
     # Handle case where mask ends with True
     if mask[-1]:
         end_indices = np.append(end_indices, len(mask))
     
     # Gather and return sequences that meet the minimum length requirement
     sequences = [arr[start:end] for start, end in zip(start_indices, end_indices) if end - start >= min_length]
     
-    return sequences
+    return sequences
+
+
+def get_max_sizes_from_fraction(size1: int, size2: int, fraction: float) -> Tuple[int, int]:
+    """
+    Calculate the maximum size from each sample such that their total size 
+    is distributed according to the given fraction.
+
+    Args:
+        size1 (int): Size of the first sample.
+        size2 (int): Size of the second sample.
+        fraction (float): Desired fraction of the total size to be assigned to size1.
+
+    Returns:
+        Tuple[int, int]: Maximum sizes from each sample that maintain the desired fraction.
+    """
+
+    if size1 <= 0 or size2 <= 0:
+        raise ValueError("sizes must be positive integers.")
+    if not (0 <= fraction <= 1):
+        raise ValueError("fraction must be a number between 0 and 1.")
+
+    total_size = size1 + size2
+    
+    max_size1 = int(total_size * fraction)
+    max_size2 = total_size - max_size1
+    
+    if max_size1 > size1:
+        max_size1 = size1
+        max_size2 = int(size1 * (1 - fraction) / fraction)
+    elif max_size2 > size2:
+        max_size2 = size2
+        max_size1 = int(size2 * fraction / (1 - fraction))
+    
+    return max_size1, max_size2
```

### Comparing `quickstats-0.7.0.4/quickstats/maths/statistics.py` & `quickstats-0.7.0.4.1/quickstats/maths/statistics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/maths/statistics_jitted.py` & `quickstats-0.7.0.4.1/quickstats/maths/statistics_jitted.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/maths/symbolics.py` & `quickstats-0.7.0.4.1/quickstats/maths/symbolics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/parsers/param_parser.py` & `quickstats-0.7.0.4.1/quickstats/parsers/param_parser.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/parsers/roo_param_setup_parser.py` & `quickstats-0.7.0.4.1/quickstats/parsers/roo_param_setup_parser.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/plots/__init__.py` & `quickstats-0.7.0.4.1/quickstats/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/plots/abstract_plot.py` & `quickstats-0.7.0.4.1/quickstats/plots/abstract_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,51 +323,27 @@
         if not ylabel:
             if mode == HistComparisonMode.RATIO:
                 ylabel = "Ratio"
             elif mode == HistComparisonMode.DIFFERENCE:
                 ylabel = "Difference"
         self.draw_axis_components(ax, xlabel=xlabel, ylabel=ylabel)
 
-
-        if plot_format == PlotFormat.HIST:
-            # draw data
-            hist_y, _, handle = ax.hist(hist_data['x'], bins, range=bin_range,
-                                        weights=hist_data['y'], **styles)
-            assert np.allclose(hist_data['y'], hist_y)
-            # draw error only
-            handles = self.draw_binned_data(ax, hist_data,
-                                            bin_edges=bin_edges,
-                                            draw_data=False,
-                                            draw_error=target_show_error,
-                                            error_format=error_format,
-                                            error_styles=error_styles)
-            if not isinstance(handle, list):
-                handle = [handle]
-            handles = tuple(list(handles) + handle)
-        elif plot_format == PlotFormat.ERRORBAR:
-            handles = self.draw_binned_data(ax, hist_data,
-                                            bin_edges=bin_edges,
-                                            styles=styles,
-                                            draw_error=target_show_error,
-                                            error_format=error_format,
-                                            error_styles=error_styles)
-
     def _draw_hist_from_binned_data(self, ax, x, y,
                                     xerr=None, yerr=None,
                                     bin_edges:Optional[np.ndarray]=None,
                                     hide:Optional[Union[Tuple[float, float], Callable]]=None,
                                     styles:Optional[Dict]=None):
         styles = combine_dict(self.styles['hist'], styles)
         # assume uniform binning
         if bin_edges is None:
             bin_center = np.array(x)
             bin_edges = bin_center_to_bin_edge(bin_center)
         bins, range = bin_edges, (bin_edges[0], bin_edges[1])
         if hide is not None:
-            mask = get_mask(x, [hide])
+            mask = get_mask(x, y, [hide])
             y[mask] = 0.
         hist_y, _, handle = ax.hist(x, bins, range=range,
                                     weights=y, **styles)
         assert np.allclose(y, hist_y)
         return handle
 
     def _draw_stacked_hist_from_binned_data(self, ax, x_list, y_list,
@@ -388,15 +364,15 @@
             bin_edges = bin_edges_list[0]
         bins, range = bin_edges, (bin_edges[0], bin_edges[1])
         if hide_list is not None:
             assert len(hide_list) == len(x_list)
             for i, hide in enumerate(hide_list):
                 if hide is None:
                     continue
-                mask = get_mask(x_list[i], [hide])
+                mask = get_mask(x_list[i], y_list[i], [hide])
                 y_list[i][mask] = 0.
         hist_y, _, handles = ax.hist(x_list, bins, range=range,
                                      weights=y_list, stacked=True,
                                      **styles)
         #assert ...
         return hist_y, handles
         
@@ -421,15 +397,15 @@
         if bin_edges is None:
             bin_center = np.array(x)
             bin_edges = bin_center_to_bin_edge(bin_center)
         if yerr is None:
             yerr = 0.
         indices = np.arange(len(x))
         if hide is not None:
-            mask = ~get_mask(x, [hide])
+            mask = ~get_mask(x, y, [hide])
             sections_indices = get_subsequences(indices, mask, min_length=2)
         else:
             sections_indices = [indices]
         handles = []
         for section_indices in sections_indices:
             mask = np.full(x.shape, False)
             mask[section_indices] = True
@@ -457,15 +433,15 @@
         if bin_edges is None:
             bin_center = np.array(x)
             bin_edges = bin_center_to_bin_edge(bin_center)
         bin_widths = np.diff(bin_edges)
         if yerr is None:
             yerr = 0.
         if hide is not None:
-            mask = ~get_mask(x, [hide])
+            mask = ~get_mask(x, y, [hide])
             x, y, xerr, yerr = select_binned_data(mask, x, y, xerr, yerr)
             bin_widths = bin_widths[mask]
         if isinstance(yerr, tuple):
             height = yerr[0] + yerr[1]
             bottom = y - yerr[0]
         else:
             height = 2 * yerr
@@ -605,17 +581,17 @@
             return handles
         if handles is None:
             return error_handles
         handles = [(handle, error_handle) for handle, error_handle in zip(handles, error_handles)]
         return handles    
 
     def draw_legend(self, ax, handles=None, labels=None,
-                    handler_map=None, **kwargs):
+                    handler_map=None, idx=None, **kwargs):
         if (handles is None) and (labels is None):
-            handles, labels = self.get_legend_handles_labels()
+            handles, labels = self.get_legend_handles_labels(idx=idx)
         if handler_map is not None:
             handler_map = {**CUSTOM_HANDLER_MAP, **handler_map}
         else:
             handler_map = CUSTOM_HANDLER_MAP
         styles = {**self.styles['legend'], **kwargs}
         styles['handler_map'] = handler_map
         ax.legend(handles, labels, **styles)
```

### Comparing `quickstats-0.7.0.4/quickstats/plots/bidirectional_bar_chart.py` & `quickstats-0.7.0.4.1/quickstats/plots/bidirectional_bar_chart.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/plots/collective_data_plot.py` & `quickstats-0.7.0.4.1/quickstats/plots/collective_data_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/plots/color_schemes.py` & `quickstats-0.7.0.4.1/quickstats/plots/color_schemes.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/plots/core.py` & `quickstats-0.7.0.4.1/quickstats/plots/core.py`

 * *Files 21% similar despite different names*

```diff
@@ -149,8 +149,26 @@
 def reload_styles():
     from matplotlib import style
     style.core.USER_LIBRARY_PATHS.append(quickstats.stylesheet_path)
     style.core.reload_library()
 
 def use_style(name:str='quick_default'):
     from matplotlib import style
-    style.use(name)
+    style.use(name)
+
+def hex_to_rgba(hex_color:str, alpha:float=1.0):
+    # Ensure the hex_color starts with '#' and is the correct length
+    if hex_color.startswith('#') and len(hex_color) == 7:
+        # Convert hex to RGB
+        r = int(hex_color[1:3], 16) / 255.0
+        g = int(hex_color[3:5], 16) / 255.0
+        b = int(hex_color[5:7], 16) / 255.0
+        # Combine RGB with Alpha
+        return (r, g, b, alpha)
+    else:
+        raise ValueError("Hex color should start with '#' and be 7 characters long")
+
+def color_to_rgba(color_scheme, alpha:float=1.0):
+    import matplotlib.colors as mcolors
+    rgba = list(mcolors.to_rgba(color_scheme))
+    rgba[-1] = alpha
+    return tuple(rgba)
```

### Comparing `quickstats-0.7.0.4/quickstats/plots/correlation_plot.py` & `quickstats-0.7.0.4.1/quickstats/plots/correlation_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/plots/general_1D_plot.py` & `quickstats-0.7.0.4.1/quickstats/plots/general_1D_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Dict, Optional, Union, List, Tuple
 import pandas as pd
 import numpy as np
 
 from quickstats.plots import AbstractPlot, StatPlotConfig
+from quickstats.plots.core import color_to_rgba
 from quickstats.plots.template import create_transform, handle_has_label
 from quickstats.utils.common_utils import combine_dict
 
 class General1DPlot(AbstractPlot):
 
     STYLES = {
         'fill_between': {
              'alpha': 0.3,
              'hatch': None,
-             'linewidth': 1.0,
-             'edgecolor': 'k'
+             'linewidth': 1.0
         }
     }
     
     CONFIG = {
         'errorband_legend': True
     }
     
@@ -66,38 +66,45 @@
                          label:Optional[str]=None):
         data = data.reset_index()
         x, y = data[xattrib].values, data[yattrib].values
         indices = np.argsort(x)
         x, y = x[indices], y[indices]
         draw_styles = combine_dict(self.styles['plot'], styles)
         fill_styles = combine_dict(self.styles['fill_between'])
-        if ('color' in draw_styles) and ('color' not in fill_styles):
-            fill_styles['color'] = draw_styles['color']
             
         if (yerrloattrib is not None) and (yerrhiattrib is not None):
             yerrlo = data[yerrloattrib][indices]
             yerrhi = data[yerrhiattrib][indices]
             handle_fill = ax.fill_between(x, yerrlo, yerrhi,
                                           **fill_styles)
         else:
             handle_fill = None
         
         handle_plot = ax.plot(x, y, **draw_styles, label=label)
+        if isinstance(handle_plot, list) and (len(handle_plot) == 1):
+            handle_plot = handle_plot[0]
+
+        if handle_fill and ('color' not in fill_styles):
+            plot_color = handle_plot.get_color()
+            fill_color = color_to_rgba(plot_color)
+            handle_fill.set_color(fill_color)
+        
         if stat_configs is not None:
             stat_handles = []
             for stat_config in stat_configs:
                 stat_config.set_data(y)
                 stat_handle = stat_config.apply(ax, handle[0])
                 stat_handles.append(stat_handle)
         else:
             stat_handles = None
+
         if self.config['errorband_legend'] and (handle_fill is not None):
-            handles = (handle_plot[0], handle_fill)
+            handles = (handle_plot, handle_fill)
         else:
-            handles = handle_plot[0]
+            handles = handle_plot
         return handles, stat_handles
     
     def draw(self, xattrib:str, yattrib:str,
              yerrloattrib:Optional[str]=None,
              yerrhiattrib:Optional[str]=None,
              targets:Optional[List[str]]=None,
              xlabel:Optional[str]=None, ylabel:Optional[str]=None,
```

### Comparing `quickstats-0.7.0.4/quickstats/plots/general_2D_plot.py` & `quickstats-0.7.0.4.1/quickstats/plots/general_2D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/plots/general_distribution_plot.py` & `quickstats-0.7.0.4.1/quickstats/plots/general_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/plots/hypotest_inverter_plot.py` & `quickstats-0.7.0.4.1/quickstats/plots/hypotest_inverter_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/plots/likelihood_1D_plot.py` & `quickstats-0.7.0.4.1/quickstats/plots/likelihood_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/plots/likelihood_2D_plot.py` & `quickstats-0.7.0.4.1/quickstats/plots/likelihood_2D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/plots/np_ranking_plot.py` & `quickstats-0.7.0.4.1/quickstats/plots/np_ranking_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/plots/pdf_distribution_plot.py` & `quickstats-0.7.0.4.1/quickstats/plots/pdf_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/plots/sample_purity_plot.py` & `quickstats-0.7.0.4.1/quickstats/plots/sample_purity_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/plots/score_distribution_plot.py` & `quickstats-0.7.0.4.1/quickstats/plots/score_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/plots/stat_plot_config.py` & `quickstats-0.7.0.4.1/quickstats/plots/stat_plot_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/plots/template.py` & `quickstats-0.7.0.4.1/quickstats/plots/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,18 +262,20 @@
         if template_options is None:
             raise ValueError(f"template analysis label options `{options}` not found")
         options = combine_dict(default_options, template_options)
     else:
         options = combine_dict(default_options, options)
     return options
 
-def ratio_frame(logx:bool=False, logy:bool=False, 
+def ratio_frame(logx:bool=False, logy:bool=False,
+                logy_lower:Optional[bool]=False,
                 styles:Optional[Union[Dict, str]]=None,
                 analysis_label_options:Optional[Union[Dict, str]]=None,
                 prop_cycle:Optional[List[str]]=None,
+                prop_cycle_lower:Optional[List[str]]=None,
                 figure_index:Optional[int]=None):
     if figure_index is None:
         plt.clf()
     else:
         plt.figure(figure_index)
     styles = parse_styles(styles)
     gridspec_kw = {
@@ -282,29 +284,41 @@
     }
     fig, (ax_main, ax_ratio) = plt.subplots(nrows=2, ncols=1, gridspec_kw=gridspec_kw,
                                             sharex=True, **styles['figure'])
     
     if logx:
         ax_main.set_xscale('log')
         ax_ratio.set_xscale('log')
+
+    if logy_lower is None:
+        logy_lower = logy
         
     if logy:
         ax_main.set_yscale('log')
+
+    if logy_lower:
+        ax_ratio.set_yscale('log')
     
     ax_main_styles = combine_dict(styles['axis'], {"x_axis_styles": {"labelbottom": False}})
     format_axis_ticks(ax_main, x_axis=True, y_axis=True, xtick_styles=styles['xtick'],
                       ytick_styles=styles['ytick'], **ax_main_styles)
     format_axis_ticks(ax_ratio, x_axis=True, y_axis=True, xtick_styles=styles['xtick'],
                       ytick_styles=styles['ytick'], **styles['axis'])
     
     if analysis_label_options is not None:
-        draw_analysis_label(ax1, text_options=styles['text'], **analysis_label_options)
+        draw_analysis_label(ax_main, text_options=styles['text'], **analysis_label_options)
         
     if prop_cycle is not None:
         ax_main.set_prop_cycle(prop_cycle)
+
+    if prop_cycle_lower is None:
+        prop_cycle_lower = prop_cycle
+
+    if prop_cycle_lower is not None:
+        ax_ratio.set_prop_cycle(prop_cycle_lower)
     
     return ax_main, ax_ratio
 
 def single_frame(logx:bool=False, logy:bool=False, 
                  styles:Optional[Union[Dict, str]]=None,
                  analysis_label_options:Optional[Union[Dict, str]]=None,
                  prop_cycle:Optional[List[str]]=None,
@@ -353,29 +367,29 @@
                       xtick_styles:Optional[Dict]=None,
                       ytick_styles:Optional[Dict]=None):
     if x_axis:
         if (ax.get_xaxis().get_scale() != 'log'):
             ax.xaxis.set_minor_locator(AutoMinorLocator())
         styles = {"labelsize":labelsize}
         styles['labeltop'] = label_bothsides
-        styles['labelbottom'] = True
+        #styles['labelbottom'] = True
         styles['top'] = tick_bothsides
         styles['bottom'] = True
         styles['direction'] = direction
         if x_axis_styles is not None:
             styles.update(x_axis_styles)
         ax.tick_params(axis="x", which="major", length=major_length,
                        width=major_width, **styles)
         ax.tick_params(axis="x", which="minor", length=minor_length,
                        width=minor_width, **styles)
     if y_axis:
         if (ax.get_yaxis().get_scale() != 'log'):
             ax.yaxis.set_minor_locator(AutoMinorLocator())    
         styles = {"labelsize":labelsize}
-        styles['labelleft'] = True
+        #styles['labelleft'] = True
         styles['labelright'] = label_bothsides
         styles['left'] = True
         styles['right'] = tick_bothsides
         styles['direction'] = direction
         if y_axis_styles is not None:
             styles.update(y_axis_styles)
         ax.tick_params(axis="y", which="major", length=major_length,
@@ -388,25 +402,27 @@
         
     set_axis_tick_styles(ax.xaxis, xtick_styles)
     set_axis_tick_styles(ax.yaxis, ytick_styles)
 
     # take care of offset labels
     if offsetlabelsize is None:
         offsetlabelsize = labelsize
-    # update the offset text
-    if plt.gca().__class__.__name__ != "AxesSubplot":
-        plt.tight_layout()
-        
-    if ax.xaxis.get_offset_text().get_text():
+
+    xaxis_offset_text = ax.xaxis.get_offset_text().get_text()
+    if xaxis_offset_text:
         ax.xaxis.get_offset_text().set_fontsize(offsetlabelsize)
         ax.xaxis.labelpad = ax.xaxis.labelpad + ax.xaxis.get_offset_text().get_fontsize()
-    if ax.yaxis.get_offset_text().get_text():
+    yaxis_offset_text = ax.yaxis.get_offset_text().get_text()
+    if yaxis_offset_text:
         ax.yaxis.get_offset_text().set_fontsize(offsetlabelsize)
         ax.yaxis.labelpad = ax.yaxis.labelpad + ax.yaxis.get_offset_text().get_fontsize()
 
+    if (xaxis_offset_text or yaxis_offset_text) and (plt.gca().__class__.__name__ != "AxesSubplot"):
+        plt.tight_layout()
+
 def set_axis_tick_styles(ax, styles=None):   
     if styles is None:
         return None
   
     fmt = styles['format']
     if fmt is not None:
         formatter = None
```

### Comparing `quickstats-0.7.0.4/quickstats/plots/test_statistic_distribution_plot.py` & `quickstats-0.7.0.4.1/quickstats/plots/test_statistic_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/plots/two_axis_1D_plot.py` & `quickstats-0.7.0.4.1/quickstats/plots/two_axis_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/plots/upper_limit_1D_plot.py` & `quickstats-0.7.0.4.1/quickstats/plots/upper_limit_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/plots/upper_limit_2D_plot.py` & `quickstats-0.7.0.4.1/quickstats/plots/upper_limit_2D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/plots/upper_limit_3D_plot.py` & `quickstats-0.7.0.4.1/quickstats/plots/upper_limit_3D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/plots/upper_limit_benchmark_plot.py` & `quickstats-0.7.0.4.1/quickstats/plots/upper_limit_benchmark_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -520,13 +520,13 @@
         ax.set_xticks(np.arange(nbenchmark))
         ax.set_xticklabels(xticklabels)
         
         handles, labels = self.get_legend_handles_labels()
         handles = remake_handles(handles, polygon_to_line=False, fill_border=True,
                                  border_styles=self.styles['legend_border'])
         handler_map = {ErrorbarContainer: HandlerErrorbar(xerr_size=1)}
-        self.darw_legend(handles, labels, handler_map=handler_map)
+        self.draw_legend(ax, handles, labels, handler_map=handler_map)
         
         if comparison_options is not None:
             return ax, ax_ratio
         
         return ax
```

### Comparing `quickstats-0.7.0.4/quickstats/plots/variable_distribution_plot.py` & `quickstats-0.7.0.4.1/quickstats/plots/variable_distribution_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -479,14 +479,20 @@
                                                 hide_list=hide_list,
                                                 styles=styles,
                                                 error_styles_list=error_styles_list)
         for i, target in enumerate(components):
             self.update_legend_handles({target: handles[i]})
         self.hist_data[stack_target] = hist_data
         self.hist_bin_edges[stack_target] = bin_edges
+
+        targets = list(components)
+        from quickstats.utils.common_utils import dict_of_list_to_list_of_dict
+        hist_data_list = dict_of_list_to_list_of_dict(stacked_data)
+        for target, hist_data_i in zip(targets, hist_data_list):
+            self.hist_data[target] = hist_data_i
         #self.update_legend_handles({stack_target: handles})
 
     def draw_single_target(self, ax, target:str, samples:List[str],
                            column_name:str,
                            styles:Dict, error_styles:Dict,
                            plot_format:Union[PlotFormat, str],
                            error_format:Union[ErrorDisplayFormat, str],
@@ -678,18 +684,18 @@
             self.draw_legend(ax, handles=handles, labels=labels)
         
         if comparison_options is not None:
             components = comparison_options.pop('components')
             for component in components:
                 reference = component.pop('reference')
                 target    = component.pop('target')
-                bin_edges = target_bin_edges[target]
+                bin_edges = self.target_bin_edges[target]
                 self.draw_comparison_data(ax_ratio,
-                                          binned_data[reference],
-                                          binned_data[target],
+                                          self.hist_data[reference],
+                                          self.hist_data[target],
                                           bin_edges=bin_edges,
                                           **component)
             comparison_options['xlabel'] = ax.get_xlabel()
             self.decorate_comparison_axis(ax_ratio, **comparison_options)
             ax.set(xlabel=None)
             ax.tick_params(axis="x", labelbottom=False)
```

### Comparing `quickstats-0.7.0.4/quickstats/root_checker.py` & `quickstats-0.7.0.4.1/quickstats/root_checker.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/utils/common_utils.py` & `quickstats-0.7.0.4.1/quickstats/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/utils/data_conversion.py` & `quickstats-0.7.0.4.1/quickstats/utils/data_conversion.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/utils/hep_utils.py` & `quickstats-0.7.0.4.1/quickstats/utils/hep_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/utils/path_utils.py` & `quickstats-0.7.0.4.1/quickstats/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/utils/py_utils.py` & `quickstats-0.7.0.4.1/quickstats/utils/py_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/utils/roofit_utils.py` & `quickstats-0.7.0.4.1/quickstats/utils/roofit_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/utils/roostats_utils.py` & `quickstats-0.7.0.4.1/quickstats/utils/roostats_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/utils/root_utils.py` & `quickstats-0.7.0.4.1/quickstats/utils/root_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/utils/string_utils.py` & `quickstats-0.7.0.4.1/quickstats/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/utils/sys_utils.py` & `quickstats-0.7.0.4.1/quickstats/utils/sys_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats/utils/xml_tools.py` & `quickstats-0.7.0.4.1/quickstats/utils/xml_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.7.0.4/quickstats.egg-info/PKG-INFO` & `quickstats-0.7.0.4.1/quickstats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.7.0.4
+Version: 0.7.0.4.1
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.7.0.4/quickstats.egg-info/SOURCES.txt` & `quickstats-0.7.0.4.1/quickstats.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -209,14 +209,15 @@
 quickstats/maths/symbolics.py
 quickstats/parsers/__init__.py
 quickstats/parsers/config_parser.py
 quickstats/parsers/param_parser.py
 quickstats/parsers/roo_param_setup_parser.py
 quickstats/plots/__init__.py
 quickstats/plots/abstract_plot.py
+quickstats/plots/bar_chart.py
 quickstats/plots/bidirectional_bar_chart.py
 quickstats/plots/collective_data_plot.py
 quickstats/plots/color_schemes.py
 quickstats/plots/core.py
 quickstats/plots/correlation_plot.py
 quickstats/plots/general_1D_plot.py
 quickstats/plots/general_2D_plot.py
```

### Comparing `quickstats-0.7.0.4/setup.py` & `quickstats-0.7.0.4.1/setup.py`

 * *Files identical despite different names*

