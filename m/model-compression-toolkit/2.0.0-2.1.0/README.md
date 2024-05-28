# Comparing `tmp/model_compression_toolkit-2.0.0.tar.gz` & `tmp/model_compression_toolkit-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_compression_toolkit-2.0.0.tar", last modified: Tue Apr  2 13:41:43 2024, max compression
+gzip compressed data, was "model_compression_toolkit-2.1.0.tar", last modified: Tue May 28 07:59:59 2024, max compression
```

## Comparing `model_compression_toolkit-2.0.0.tar` & `model_compression_toolkit-2.1.0.tar`

### file list

```diff
@@ -1,593 +1,607 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.586365 model_compression_toolkit-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    19994 2024-04-02 13:41:43.586365 model_compression_toolkit-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17988 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.518365 model_compression_toolkit-2.0.0/model_compression_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.522365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.522365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.522365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/back2framework/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/back2framework/base_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/base_substitutions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.522365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/collectors/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/collectors/base_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/collectors/histogram_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/collectors/mean_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/collectors/statistics_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)    21152 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.522365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/fusion/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/fusion/layer_fusing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.526365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38178 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/base_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    28492 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/base_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/functional_node.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4744 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/graph_matchers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5128 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/graph_searches.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.526365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/memory_graph/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/memory_graph/cut.py
--rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.526365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/hessian/hessian_info_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/hessian/hessian_info_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/hessian/trace_hessian_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.526365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/matchers/
--rwxr-xr-x   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/matchers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3091 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/matchers/base_graph_filter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2210 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/matchers/base_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3706 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/matchers/edge_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1773 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/matchers/function.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2745 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/matchers/node_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1111 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/matchers/walk_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/memory_computation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.530365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)    37578 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.530365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    21473 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.530365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/search_methods/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
--rw-r--r--   0 runner    (1001) docker     (127)    28519 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/model_builder_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/model_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/model_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.530365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/network_editors/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/network_editors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/network_editors/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/network_editors/edit_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/network_editors/node_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.534365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/channels_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.534365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/importance_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    14027 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.534365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/mask/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/mask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)    19523 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/memory_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/prune_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/pruner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/pruning_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/pruning_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/pruning_section.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.534365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/core_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/debug_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
--rw-r--r--   0 runner    (1001) docker     (127)    26737 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.538365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18165 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
--rw-r--r--   0 runner    (1001) docker     (127)    41524 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantize_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.538365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11503 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/similarity_analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.538365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.542365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13392 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12367 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    29865 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/user_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.542365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/visualization/nn_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21951 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10100 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/graph_prep_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.542365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.542365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/back2framework/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16001 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15567 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/custom_layer_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.542365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.546365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     8158 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py
--rw-r--r--   0 runner    (1001) docker     (127)    26771 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)    11149 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.546365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)    29399 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/keras_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/keras_node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.550365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.550365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12710 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.550365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.550365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/reader/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/reader/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/reader/connectivity_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.550365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/reader/nested_model/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/reader/node_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/reader/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/resource_utilization_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.550365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/tf_tensor_numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.550365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.554365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.554365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/back2framework/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    17443 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.554365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.554365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.558365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    38459 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.558365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.558365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.558365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14648 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/pytorch_device_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27082 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.558365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.558365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/reader/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12626 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/reader/graph_builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/reader/node_holders.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/reader/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.558365 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/quantization_prep_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    11836 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/core/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.558365 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.562365 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/common/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/common/data_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/common/data_generation_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/common/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/common/image_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/common/model_info_exctractors.py
--rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/common/optimization_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.562365 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7623 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/image_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    21539 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/keras_data_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/model_info_exctractors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.562365 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/optimization_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21146 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/optimization_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.562365 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/image_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.562365 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19085 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/optimization_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20937 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/defaultdict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.562365 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.562365 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.566365 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.566365 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.566365 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.566365 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.566365 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.566365 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.566365 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/keras/builder/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.566365 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.566365 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.570365 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.570365 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/common/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/common/gptq_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/common/gptq_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/common/gptq_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    17705 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/common/gptq_training.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.570365 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    18438 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    14057 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.570365 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.570365 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.570365 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.574365 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)    15808 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    12495 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.574365 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.574365 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (127)    12347 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.574365 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8768 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.574365 model_compression_toolkit-2.0.0/model_compression_toolkit/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/pruning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.574365 model_compression_toolkit-2.0.0/model_compression_toolkit/pruning/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/pruning/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/pruning/keras/pruning_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.574365 model_compression_toolkit-2.0.0/model_compression_toolkit/pruning/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/pruning/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/pruning/pytorch/pruning_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.574365 model_compression_toolkit-2.0.0/model_compression_toolkit/ptq/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/ptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.574365 model_compression_toolkit-2.0.0/model_compression_toolkit/ptq/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/ptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9057 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/ptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.574365 model_compression_toolkit-2.0.0/model_compression_toolkit/ptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/ptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/ptq/pytorch/quantization_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/ptq/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.574365 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.574365 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/common/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/common/qat_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.578365 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.578365 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.578365 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantizer/lsq/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.578365 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13517 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.578365 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.578365 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.578365 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantizer/lsq/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10712 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.578365 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.578365 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/immutable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.582365 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
--rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.582365 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.582365 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.582365 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.582365 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.582365 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.582365 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.582365 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.582365 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.586365 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.586365 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.586365 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.586365 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.586365 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.586365 model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.586365 model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/common/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.586365 model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.586365 model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:41:43.522365 model_compression_toolkit-2.0.0/model_compression_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19994 2024-04-02 13:41:43.000000 model_compression_toolkit-2.0.0/model_compression_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    36440 2024-04-02 13:41:43.000000 model_compression_toolkit-2.0.0/model_compression_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:41:43.000000 model_compression_toolkit-2.0.0/model_compression_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-02 13:41:43.000000 model_compression_toolkit-2.0.0/model_compression_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 13:41:43.000000 model_compression_toolkit-2.0.0/model_compression_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-02 13:41:43.590365 model_compression_toolkit-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-02 13:41:14.000000 model_compression_toolkit-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.484225 model_compression_toolkit-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    20880 2024-05-28 07:59:59.484225 model_compression_toolkit-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18914 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.416225 model_compression_toolkit-2.1.0/model_compression_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.416225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.416225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.420225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/back2framework/base_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/base_substitutions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.420225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/collectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/collectors/base_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/collectors/histogram_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/collectors/mean_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/collectors/statistics_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20896 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.420225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/fusion/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/fusion/layer_fusing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.420225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38326 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/base_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29722 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/base_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/functional_node.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4744 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/graph_matchers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5128 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/graph_searches.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.420225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/memory_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/memory_graph/cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.424225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/hessian/hessian_info_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/hessian/hessian_info_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/hessian/trace_hessian_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.424225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/matchers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/matchers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3091 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/matchers/base_graph_filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2210 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/matchers/base_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3706 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/matchers/edge_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1773 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/matchers/function.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2745 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/matchers/node_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1111 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/matchers/walk_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/memory_computation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.424225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37578 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.428225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13820 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21506 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.428225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/search_methods/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28940 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/model_builder_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/model_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/model_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.428225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/network_editors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/network_editors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/network_editors/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/network_editors/edit_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/network_editors/node_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.428225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/channels_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.428225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/importance_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14027 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.432225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/mask/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/mask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19523 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/memory_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/prune_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/pruner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/pruning_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/pruning_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/pruning_section.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.432225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/core_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/debug_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26733 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7106 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.432225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23305 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8059 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41524 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8902 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantize_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.436225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/similarity_analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.436225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10478 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.436225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13392 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12367 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/remove_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29865 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/user_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.440225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/visualization/nn_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22510 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/graph_prep_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.440225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.440225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15587 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/custom_layer_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.440225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.444225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/concat_threshold_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26771 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11169 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.444225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29881 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/keras_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/keras_node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.444225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.444225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12777 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.444225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.444225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/reader/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/reader/connectivity_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.448225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/reader/nested_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/reader/node_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/reader/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/resource_utilization_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.448225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/tf_tensor_numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.448225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.448225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.448225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18258 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.448225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.448225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.452225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/concat_threshold_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38459 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/remove_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.452225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.452225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.452225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14764 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/pytorch_device_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27516 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.456225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.456225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/reader/graph_builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/reader/node_holders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/reader/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.456225 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/quantization_prep_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/core/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.456225 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.456225 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/common/data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/common/data_generation_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/common/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/common/image_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/common/model_info_exctractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19761 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/common/optimization_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.456225 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7623 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/image_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21539 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/keras_data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/model_info_exctractors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.456225 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/optimization_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21146 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/optimization_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.460225 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/image_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.460225 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19085 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/optimization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21238 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/defaultdict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.460225 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.460225 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.460225 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.460225 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11702 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.464225 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.464225 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.464225 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.464225 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.464225 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/keras/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.464225 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.464225 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.464225 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.464225 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/common/gptq_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/common/gptq_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/common/gptq_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16093 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/common/gptq_training.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.468225 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19123 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.468225 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.468225 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.468225 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.468225 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16509 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13154 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.468225 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.468225 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12347 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.468225 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8768 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.472225 model_compression_toolkit-2.1.0/model_compression_toolkit/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/pruning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.472225 model_compression_toolkit-2.1.0/model_compression_toolkit/pruning/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/pruning/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/pruning/keras/pruning_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.472225 model_compression_toolkit-2.1.0/model_compression_toolkit/pruning/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/pruning/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/pruning/pytorch/pruning_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.472225 model_compression_toolkit-2.1.0/model_compression_toolkit/ptq/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/ptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.472225 model_compression_toolkit-2.1.0/model_compression_toolkit/ptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/ptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10517 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/ptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.472225 model_compression_toolkit-2.1.0/model_compression_toolkit/ptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/ptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/ptq/pytorch/quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/ptq/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.472225 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.472225 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/common/qat_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.472225 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.472225 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.472225 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantizer/lsq/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.472225 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13517 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.472225 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.476225 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.476225 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantizer/lsq/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10712 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.476225 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.476225 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/immutable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.476225 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.476225 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9910 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.476225 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.476225 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.480225 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.480225 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.480225 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.480225 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.480225 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.480225 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.480225 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.480225 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.480225 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.484225 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.484225 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.484225 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.484225 model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.484225 model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.484225 model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.484225 model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 07:59:59.416225 model_compression_toolkit-2.1.0/model_compression_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20880 2024-05-28 07:59:58.000000 model_compression_toolkit-2.1.0/model_compression_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    37548 2024-05-28 07:59:59.000000 model_compression_toolkit-2.1.0/model_compression_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 07:59:58.000000 model_compression_toolkit-2.1.0/model_compression_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-28 07:59:58.000000 model_compression_toolkit-2.1.0/model_compression_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-28 07:59:58.000000 model_compression_toolkit-2.1.0/model_compression_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-28 07:59:59.484225 model_compression_toolkit-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-28 07:59:25.000000 model_compression_toolkit-2.1.0/setup.py
```

### Comparing `model_compression_toolkit-2.0.0/LICENSE.md` & `model_compression_toolkit-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/PKG-INFO` & `model_compression_toolkit-2.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,204 +1,185 @@
-Metadata-Version: 2.1
-Name: model_compression_toolkit
-Version: 2.0.0
-Summary: A Model Compression Toolkit for neural networks
-Home-page: UNKNOWN
-License: UNKNOWN
-Description: # Model Compression Toolkit (MCT)
-        
-        Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
-        
-        This project provides researchers, developers, and engineers tools for optimizing and deploying state-of-the-art neural networks on efficient hardware.
-        
-        Specifically, this project aims to apply quantization to compress neural networks.
-        
-        <img src="docsrc/images/mct_block_diagram.svg" width="10000">
-        
-        MCT is developed by researchers and engineers working at Sony Semiconductor Israel.
-        
-        
-        
-        ## Table of Contents
-        
-        - [Getting Started](#getting-started)
-        - [Supported features](#supported-features)
-        - [Results](#results)
-        - [Troubleshooting](#trouble-shooting)
-        - [Contributions](#contributions)
-        - [License](#license)
-        
-        
-        ## Getting Started
-        
-        This section provides an installation and a quick starting guide.
-        
-        ### Installation
-        
-        To install the latest stable release of MCT, run the following command:
-        ```
-        pip install model-compression-toolkit
-        ```
-        
-        For installing the nightly version or installing from source, refer to the [installation guide](INSTALLATION.md).
-        
-        
-        ### Quick start & tutorials 
-        
-        Explore the Model Compression Toolkit (MCT) through our tutorials, 
-        covering compression techniques for Keras and PyTorch models. Access interactive [notebooks](tutorials/README.md) 
-        for hands-on learning. For example:
-        * [Keras MobileNetV2 post training quantization](tutorials/notebooks/keras/ptq/example_keras_imagenet.ipynb)
-        * [Post training quantization with PyTorch](tutorials/notebooks/pytorch/ptq/example_pytorch_quantization_mnist.ipynb)
-        * [Data Generation for ResNet18 with PyTorch](tutorials/notebooks/pytorch/data_generation/example_pytorch_data_generation.ipynb).
-        
-        Additionally, for quick quantization of a variety of models from well-known collections,
-        visit the [quick-start page](tutorials/quick_start/README.md) and the
-        [results CSV](tutorials/quick_start/results/model_quantization_results.csv).
-        
-        ### Supported Versions
-        
-        Currently, MCT is being tested on various Python, Pytorch and TensorFlow versions:
-        
-        |             |  PyTorch 1.13                                                                                                                                                                                                               | PyTorch 2.0                                                                                                                                                                                                              | PyTorch 2.1                                                                                                                                                                                                              |
-        |-------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-        | Python 3.9  | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch113.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch113.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch20.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch20.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch21.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch21.yml)   |
-        | Python 3.10 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch112.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch112.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch113.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch113.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch20.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch20.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch21.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch21.yml) |
-        | Python 3.11 | | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch20.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch20.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch21.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch21.yml) |
-        
-        
-        |             | TensorFlow 2.12                                                                                                                                                                                                                        | TensorFlow 2.13                                                                                                                                                                                                                        | TensorFlow 2.14                                                                                                                                                                                                                        | TensorFlow 2.15                                                                                                                                                                                                        |
-        |-------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-        | Python 3.9  | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras212.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras213.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras214.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras215.yml)   |
-        | Python 3.10 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras212.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras213.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras214.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras215.yml) |
-        | Python 3.11 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras212.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras213.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras214.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras215.yml) |
-        
-        
-        ## Supported Features
-        MCT offers a range of powerful features to optimize neural network models for efficient deployment. These supported features include:
-        
-        ### Data Generation [*](#experimental-features)
-        MCT provides tools for generating synthetic images based on the statistics stored in a model's batch normalization layers. These generated images are valuable for various compression tasks where image data is required, such as quantization and pruning. 
-        You can customize data generation configurations to suit your specific needs. [Go to the Data Generation page.](model_compression_toolkit/data_generation/README.md)
-        
-        ### Quantization
-        MCT supports different quantization methods:
-        * Post-training quantization (PTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_post_training_quantization.html), [PyTorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_post_training_quantization.html)
-        * Gradient-based post-training quantization (GPTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_gradient_post_training_quantization.html), [PyTorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_gradient_post_training_quantization.html)
-        * Quantization-aware training (QAT) [*](#experimental-features)
-        
-        
-        | Quantization Method                           | Complexity | Computational Cost          |
-        |-----------------------------------------------|------------|-----------------------------|
-        | PTQ                                           | Low        | Low (order of minutes)      |
-        | GPTQ (parameters fine-tuning using gradients) | Mild       | Mild (order of 2-3 hours)   |
-        | QAT                                           | High       | High (order of 12-36 hours) |
-        
-        
-        In addition, MCT supports different quantization schemes for quantizing weights and activations:
-        
-        * Power-Of-Two (hardware-friendly quantization [1])
-        * Symmetric
-        * Uniform
-        
-        Main features:
-        * <ins>Graph optimizations:</ins> Transforming the model to an equivalent (yet, more efficient) model (for example, batch-normalization layer folding to its preceding linear layer).
-        * <ins>Quantization parameter search:</ins> Different methods can be used to minimize the expected added quantization-noise during thresholds search (by default, we use Mean-Square-Error, but other metrics can be used such as No-Clipping, Mean-Average-Error, and more).
-        * <ins>Advanced quantization algorithms:</ins> To prevent a performance degradation some algorithms are applied such as: 
-          * <ins>Shift negative correction:</ins> Symmetric activation quantization can hurt the model's performance when some layers output both negative and positive activations, but their range is asymmetric. For more details please visit [1].
-          * <ins>Outliers filtering:</ins> Computing z-score for activation statistics to detect and remove outliers.
-        * <ins>Clustering:</ins> Using non-uniform quantization grid to quantize the weights and activations to match their distributions.[*](#experimental-features)
-        * <ins>Mixed-precision search:</ins> Assigning quantization bit-width per layer (for weights/activations), based on the layer's sensitivity to different bit-widths.
-        * <ins>Visualization:</ins> You can use TensorBoard to observe useful information for troubleshooting the quantized model's performance (for example, the model in different phases of the quantization, collected statistics, similarity between layers of the float and quantized model and bit-width configuration for mixed-precision quantization). For more details, please read the [visualization documentation](https://sony.github.io/model_optimization/docs/guidelines/visualization.html).   
-        * <ins>Target Platform Capabilities:</ins> The Target Platform Capabilities (TPC) describes the target platform (an edge device with dedicated hardware). For more details, please read the [TPC README](model_compression_toolkit/target_platform_capabilities/README.md).   
-        
-        ### Enhanced Post-Training Quantization (EPTQ)
-        As part of the GPTQ we provide an advanced optimization algorithm called EPTQ.
-        
-        The specifications of the algorithm are detailed in the paper: _"**EPTQ: Enhanced Post-Training Quantization via Label-Free Hessian**"_ [4].
-        
-        More details on the how to use EPTQ via MCT can be found in the [EPTQ guidelines](model_compression_toolkit/gptq/README.md).
-        
-        
-        ### Structured Pruning [*](#experimental-features)
-        MCT introduces a structured and hardware-aware model pruning.
-        This pruning technique is designed to compress models for specific hardware architectures, 
-        taking into account the target platform's Single Instruction, Multiple Data (SIMD) capabilities. 
-        By pruning groups of channels (SIMD groups), our approach not only reduces model size 
-        and complexity, but ensures that better utilization of channels is in line with the SIMD architecture 
-        for a target Resource Utilization of weights memory footprint.
-        [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_pruning_experimental.html)
-        [Pytorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_pruning_experimental.html) 
-        
-        #### Experimental features 
-        
-        Some features are experimental and subject to future changes. 
-         
-        For more details, we highly recommend visiting our project website where experimental features are mentioned as experimental.
-        
-        
-        ## Results
-        ### Keras
-        Graph of [MobileNetV2](https://keras.io/api/applications/mobilenet/) accuracy on ImageNet vs average bit-width of weights, using 
-        single-precision quantization, mixed-precision quantization, and mixed-precision quantization with GPTQ.
-        
-        <img src="docsrc/images/mbv2_accuracy_graph.png">
-        
-        For more results, please see [1]
-        
-        ### Pytorch
-        We quantized classification networks from the torchvision library. 
-        In the following table we present the ImageNet validation results for these models:
-        
-        | Network Name              | Float Accuracy  | 8Bit Accuracy   | Data-Free 8Bit Accuracy |
-        |---------------------------|-----------------|-----------------|-------------------------|
-        | MobileNet V2 [3]          | 71.886          | 71.444          |71.29|
-        | ResNet-18 [3]             | 69.86           | 69.63           |69.53|
-        | SqueezeNet 1.1 [3]        | 58.128          | 57.678          ||
-        
-        For more results, please refer to [quick start](https://github.com/sony/model_optimization/tree/main/tutorials/quick_start).
-        
-        
-        #### Pruning Results
-        
-        Results for applying pruning to reduce the parameters of the following models by 50%:
-        
-        | Model           | Dense Model Accuracy | Pruned Model Accuracy |
-        |-----------------|----------------------|-----------------------|
-        | ResNet50 [2]    | 75.1                 | 72.4                  |
-        | DenseNet121 [3] | 74.44                | 71.71                 |
-        
-        
-        ## Trouble Shooting
-        
-        If the accuracy degradation of the quantized model is too large for your application, check out the [Quantization Troubleshooting](https://github.com/sony/model_optimization/tree/main/quantization_troubleshooting.md)
-        for common pitfalls and some tools to improve quantization accuracy.
-        
-        Check out the [FAQ](https://github.com/sony/model_optimization/tree/main/FAQ.md) for common issues.
-        
-        
-        ## Contributions
-        MCT aims at keeping a more up-to-date fork and welcomes contributions from anyone.
-        
-        *You will find more information about contributions in the [Contribution guide](CONTRIBUTING.md).
-        
-        
-        ## License
-        [Apache License 2.0](LICENSE.md).
-        
-        ## References 
-        
-        [1] Habi, H.V., Peretz, R., Cohen, E., Dikstein, L., Dror, O., Diamant, I., Jennings, R.H. and Netzer, A., 2021. [HPTQ: Hardware-Friendly Post Training Quantization. arXiv preprint](https://arxiv.org/abs/2109.09113).
-        
-        [2] [Keras Applications](https://keras.io/api/applications/)
-        
-        [3] [TORCHVISION.MODELS](https://pytorch.org/vision/stable/models.html) 
-        
-        [4] Gordon, O., Habi, H. V., & Netzer, A., 2023. [EPTQ: Enhanced Post-Training Quantization via Label-Free Hessian. arXiv preprint](https://arxiv.org/abs/2309.11531)
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+# Model Compression Toolkit (MCT)
+
+Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
+
+This project provides researchers, developers, and engineers tools for optimizing and deploying state-of-the-art neural networks on efficient hardware.
+
+Specifically, this project aims to apply quantization to compress neural networks.
+
+<img src="https://github.com/sony/model_optimization/raw/main/docsrc/images/mct_block_diagram.svg" width="10000">
+
+MCT is developed by researchers and engineers working at Sony Semiconductor Israel.
+
+
+
+## Table of Contents
+
+- [Getting Started](https://github.com/sony/model_optimization?tab=readme-ov-file#getting-started)
+- [Supported features](https://github.com/sony/model_optimization?tab=readme-ov-file#supported-features)
+- [Results](https://github.com/sony/model_optimization?tab=readme-ov-file#results)
+- [Troubleshooting](https://github.com/sony/model_optimization?tab=readme-ov-file#trouble-shooting)
+- [Contributions](https://github.com/sony/model_optimization?tab=readme-ov-file#contributions)
+- [License](https://github.com/sony/model_optimization?tab=readme-ov-file#license)
+
+
+## Getting Started
+
+This section provides an installation and a quick starting guide.
+
+### Installation
+
+To install the latest stable release of MCT, run the following command:
+```
+pip install model-compression-toolkit
+```
+
+For installing the nightly version or installing from source, refer to the [installation guide](https://github.com/sony/model_optimization/blob/main/INSTALLATION.md).
+
+
+### Quick start & tutorials 
+
+Explore the Model Compression Toolkit (MCT) through our tutorials, 
+covering compression techniques for Keras and PyTorch models. Access interactive [notebooks](https://github.com/sony/model_optimization/blob/main/tutorials/README.md) 
+for hands-on learning. For example:
+* [Keras MobileNetV2 post training quantization](https://github.com/sony/model_optimization/blob/main/tutorials/notebooks/imx500_notebooks/keras/example_keras_mobilenetv2_for_imx500.ipynb)
+* [Post training quantization with PyTorch](https://github.com/sony/model_optimization/blob/main/tutorials/notebooks/mct_features_notebooks/pytorch/example_pytorch_ptq_mnist.ipynb)
+* [Data Generation for ResNet18 with PyTorch](https://github.com/sony/model_optimization/blob/main/tutorials/notebooks/mct_features_notebooks/pytorch/example_pytorch_data_generation.ipynb).
+
+
+### Supported Versions
+
+Currently, MCT is being tested on various Python, Pytorch and TensorFlow versions:
+
+|             |  PyTorch 1.13                                                                                                                                                                                                               | PyTorch 2.0                                                                                                                                                                                                              | PyTorch 2.1                                                                                                                                                                                                              |
+|-------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Python 3.9  | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch113.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch113.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch20.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch20.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch21.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch21.yml)   |
+| Python 3.10 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch112.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch112.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch113.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch113.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch20.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch20.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch21.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch21.yml) |
+| Python 3.11 | | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch20.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch20.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch21.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch21.yml) |
+
+
+|             | TensorFlow 2.12                                                                                                                                                                                                                        | TensorFlow 2.13                                                                                                                                                                                                                        | TensorFlow 2.14                                                                                                                                                                                                                        | TensorFlow 2.15                                                                                                                                                                                                        |
+|-------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Python 3.9  | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras212.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras213.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras214.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras215.yml)   |
+| Python 3.10 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras212.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras213.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras214.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras215.yml) |
+| Python 3.11 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras212.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras213.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras214.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras215.yml) |
+
+
+## Supported Features
+MCT offers a range of powerful features to optimize neural network models for efficient deployment. These supported features include:
+
+### Data Generation [*](https://github.com/sony/model_optimization?tab=readme-ov-file#experimental-features)
+MCT provides tools for generating synthetic images based on the statistics stored in a model's batch normalization layers. These generated images are valuable for various compression tasks where image data is required, such as quantization and pruning. 
+You can customize data generation configurations to suit your specific needs. [Go to the Data Generation page.](https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/data_generation/README.md)
+
+### Quantization
+MCT supports different quantization methods:
+* Post-training quantization (PTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_post_training_quantization.html), [PyTorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_post_training_quantization.html)
+* Gradient-based post-training quantization (GPTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_gradient_post_training_quantization.html), [PyTorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_gradient_post_training_quantization.html)
+* Quantization-aware training (QAT) [*](https://github.com/sony/model_optimization?tab=readme-ov-file#experimental-features)
+
+
+| Quantization Method                           | Complexity | Computational Cost          |
+|-----------------------------------------------|------------|-----------------------------|
+| PTQ                                           | Low        | Low (order of minutes)      |
+| GPTQ (parameters fine-tuning using gradients) | Mild       | Mild (order of 2-3 hours)   |
+| QAT                                           | High       | High (order of 12-36 hours) |
+
+
+In addition, MCT supports different quantization schemes for quantizing weights and activations:
+
+* Power-Of-Two (hardware-friendly quantization [1])
+* Symmetric
+* Uniform
+
+Main features:
+* <ins>Graph optimizations:</ins> Transforming the model to an equivalent (yet, more efficient) model (for example, batch-normalization layer folding to its preceding linear layer).
+* <ins>Quantization parameter search:</ins> Different methods can be used to minimize the expected added quantization-noise during thresholds search (by default, we use Mean-Square-Error, but other metrics can be used such as No-Clipping, Mean-Average-Error, and more).
+* <ins>Advanced quantization algorithms:</ins> To prevent a performance degradation some algorithms are applied such as: 
+  * <ins>Shift negative correction:</ins> Symmetric activation quantization can hurt the model's performance when some layers output both negative and positive activations, but their range is asymmetric. For more details please visit [1].
+  * <ins>Outliers filtering:</ins> Computing z-score for activation statistics to detect and remove outliers.
+* <ins>Clustering:</ins> Using non-uniform quantization grid to quantize the weights and activations to match their distributions.[*](https://github.com/sony/model_optimization?tab=readme-ov-file#experimental-features)
+* <ins>Mixed-precision search:</ins> Assigning quantization bit-width per layer (for weights/activations), based on the layer's sensitivity to different bit-widths.
+* <ins>Visualization:</ins> You can use TensorBoard to observe useful information for troubleshooting the quantized model's performance (for example, the model in different phases of the quantization, collected statistics, similarity between layers of the float and quantized model and bit-width configuration for mixed-precision quantization). For more details, please read the [visualization documentation](https://sony.github.io/model_optimization/docs/guidelines/visualization.html).   
+* <ins>Target Platform Capabilities:</ins> The Target Platform Capabilities (TPC) describes the target platform (an edge device with dedicated hardware). For more details, please read the [TPC README](https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/target_platform_capabilities/README.md).   
+
+### Enhanced Post-Training Quantization (EPTQ)
+As part of the GPTQ we provide an advanced optimization algorithm called EPTQ.
+
+The specifications of the algorithm are detailed in the paper: _"**EPTQ: Enhanced Post-Training Quantization via Label-Free Hessian**"_ [4].
+
+More details on the how to use EPTQ via MCT can be found in the [EPTQ guidelines](https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/gptq/README.md).
+
+
+### Structured Pruning [*](https://github.com/sony/model_optimization?tab=readme-ov-file#experimental-features)
+MCT introduces a structured and hardware-aware model pruning.
+This pruning technique is designed to compress models for specific hardware architectures, 
+taking into account the target platform's Single Instruction, Multiple Data (SIMD) capabilities. 
+By pruning groups of channels (SIMD groups), our approach not only reduces model size 
+and complexity, but ensures that better utilization of channels is in line with the SIMD architecture 
+for a target Resource Utilization of weights memory footprint.
+[Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_pruning_experimental.html)
+[Pytorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_pruning_experimental.html) 
+
+#### Experimental features 
+
+Some features are experimental and subject to future changes. 
+ 
+For more details, we highly recommend visiting our project website where experimental features are mentioned as experimental.
+
+
+## Results
+### Keras
+Graph of [MobileNetV2](https://keras.io/api/applications/mobilenet/) accuracy on ImageNet vs average bit-width of weights, using 
+single-precision quantization, mixed-precision quantization, and mixed-precision quantization with GPTQ.
+
+<img src="https://github.com/sony/model_optimization/raw/main/docsrc/images/mbv2_accuracy_graph.png">
+
+For more results, please see [1]
+
+### Pytorch
+We quantized classification networks from the torchvision library. 
+In the following table we present the ImageNet validation results for these models:
+
+| Network Name              | Float Accuracy  | 8Bit Accuracy   | Data-Free 8Bit Accuracy |
+|---------------------------|-----------------|-----------------|-------------------------|
+| MobileNet V2 [3]          | 71.886          | 71.444          |71.29|
+| ResNet-18 [3]             | 69.86           | 69.63           |69.53|
+| SqueezeNet 1.1 [3]        | 58.128          | 57.678          ||
+
+
+#### Pruning Results
+
+Results for applying pruning to reduce the parameters of the following models by 50%:
+
+| Model           | Dense Model Accuracy | Pruned Model Accuracy |
+|-----------------|----------------------|-----------------------|
+| ResNet50 [2]    | 75.1                 | 72.4                  |
+| DenseNet121 [3] | 74.44                | 71.71                 |
+
+
+## Trouble Shooting
+
+If the accuracy degradation of the quantized model is too large for your application, check out the [Quantization Troubleshooting](https://github.com/sony/model_optimization/tree/main/quantization_troubleshooting.md)
+for common pitfalls and some tools to improve quantization accuracy.
+
+Check out the [FAQ](https://github.com/sony/model_optimization/tree/main/FAQ.md) for common issues.
+
+
+## Contributions
+MCT aims at keeping a more up-to-date fork and welcomes contributions from anyone.
+
+*You will find more information about contributions in the [Contribution guide](https://github.com/sony/model_optimization/blob/main/CONTRIBUTING.md).
+
+
+## License
+[Apache License 2.0](https://github.com/sony/model_optimization/blob/main/LICENSE.md).
+
+## References 
+
+[1] Habi, H.V., Peretz, R., Cohen, E., Dikstein, L., Dror, O., Diamant, I., Jennings, R.H. and Netzer, A., 2021. [HPTQ: Hardware-Friendly Post Training Quantization. arXiv preprint](https://arxiv.org/abs/2109.09113).
+
+[2] [Keras Applications](https://keras.io/api/applications/)
+
+[3] [TORCHVISION.MODELS](https://pytorch.org/vision/stable/models.html) 
+
+[4] Gordon, O., Habi, H. V., & Netzer, A., 2023. [EPTQ: Enhanced Post-Training Quantization via Label-Free Hessian. arXiv preprint](https://arxiv.org/abs/2309.11531)
```

### Comparing `model_compression_toolkit-2.0.0/README.md` & `model_compression_toolkit-2.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,190 +1,199 @@
-# Model Compression Toolkit (MCT)
-
-Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
-
-This project provides researchers, developers, and engineers tools for optimizing and deploying state-of-the-art neural networks on efficient hardware.
-
-Specifically, this project aims to apply quantization to compress neural networks.
-
-<img src="docsrc/images/mct_block_diagram.svg" width="10000">
-
-MCT is developed by researchers and engineers working at Sony Semiconductor Israel.
-
-
-
-## Table of Contents
-
-- [Getting Started](#getting-started)
-- [Supported features](#supported-features)
-- [Results](#results)
-- [Troubleshooting](#trouble-shooting)
-- [Contributions](#contributions)
-- [License](#license)
-
-
-## Getting Started
-
-This section provides an installation and a quick starting guide.
-
-### Installation
-
-To install the latest stable release of MCT, run the following command:
-```
-pip install model-compression-toolkit
-```
-
-For installing the nightly version or installing from source, refer to the [installation guide](INSTALLATION.md).
-
-
-### Quick start & tutorials 
-
-Explore the Model Compression Toolkit (MCT) through our tutorials, 
-covering compression techniques for Keras and PyTorch models. Access interactive [notebooks](tutorials/README.md) 
-for hands-on learning. For example:
-* [Keras MobileNetV2 post training quantization](tutorials/notebooks/keras/ptq/example_keras_imagenet.ipynb)
-* [Post training quantization with PyTorch](tutorials/notebooks/pytorch/ptq/example_pytorch_quantization_mnist.ipynb)
-* [Data Generation for ResNet18 with PyTorch](tutorials/notebooks/pytorch/data_generation/example_pytorch_data_generation.ipynb).
-
-Additionally, for quick quantization of a variety of models from well-known collections,
-visit the [quick-start page](tutorials/quick_start/README.md) and the
-[results CSV](tutorials/quick_start/results/model_quantization_results.csv).
-
-### Supported Versions
-
-Currently, MCT is being tested on various Python, Pytorch and TensorFlow versions:
-
-|             |  PyTorch 1.13                                                                                                                                                                                                               | PyTorch 2.0                                                                                                                                                                                                              | PyTorch 2.1                                                                                                                                                                                                              |
-|-------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| Python 3.9  | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch113.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch113.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch20.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch20.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch21.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch21.yml)   |
-| Python 3.10 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch112.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch112.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch113.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch113.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch20.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch20.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch21.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch21.yml) |
-| Python 3.11 | | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch20.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch20.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch21.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch21.yml) |
-
-
-|             | TensorFlow 2.12                                                                                                                                                                                                                        | TensorFlow 2.13                                                                                                                                                                                                                        | TensorFlow 2.14                                                                                                                                                                                                                        | TensorFlow 2.15                                                                                                                                                                                                        |
-|-------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| Python 3.9  | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras212.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras213.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras214.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras215.yml)   |
-| Python 3.10 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras212.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras213.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras214.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras215.yml) |
-| Python 3.11 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras212.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras213.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras214.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras215.yml) |
-
-
-## Supported Features
-MCT offers a range of powerful features to optimize neural network models for efficient deployment. These supported features include:
-
-### Data Generation [*](#experimental-features)
-MCT provides tools for generating synthetic images based on the statistics stored in a model's batch normalization layers. These generated images are valuable for various compression tasks where image data is required, such as quantization and pruning. 
-You can customize data generation configurations to suit your specific needs. [Go to the Data Generation page.](model_compression_toolkit/data_generation/README.md)
-
-### Quantization
-MCT supports different quantization methods:
-* Post-training quantization (PTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_post_training_quantization.html), [PyTorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_post_training_quantization.html)
-* Gradient-based post-training quantization (GPTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_gradient_post_training_quantization.html), [PyTorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_gradient_post_training_quantization.html)
-* Quantization-aware training (QAT) [*](#experimental-features)
-
-
-| Quantization Method                           | Complexity | Computational Cost          |
-|-----------------------------------------------|------------|-----------------------------|
-| PTQ                                           | Low        | Low (order of minutes)      |
-| GPTQ (parameters fine-tuning using gradients) | Mild       | Mild (order of 2-3 hours)   |
-| QAT                                           | High       | High (order of 12-36 hours) |
-
-
-In addition, MCT supports different quantization schemes for quantizing weights and activations:
-
-* Power-Of-Two (hardware-friendly quantization [1])
-* Symmetric
-* Uniform
-
-Main features:
-* <ins>Graph optimizations:</ins> Transforming the model to an equivalent (yet, more efficient) model (for example, batch-normalization layer folding to its preceding linear layer).
-* <ins>Quantization parameter search:</ins> Different methods can be used to minimize the expected added quantization-noise during thresholds search (by default, we use Mean-Square-Error, but other metrics can be used such as No-Clipping, Mean-Average-Error, and more).
-* <ins>Advanced quantization algorithms:</ins> To prevent a performance degradation some algorithms are applied such as: 
-  * <ins>Shift negative correction:</ins> Symmetric activation quantization can hurt the model's performance when some layers output both negative and positive activations, but their range is asymmetric. For more details please visit [1].
-  * <ins>Outliers filtering:</ins> Computing z-score for activation statistics to detect and remove outliers.
-* <ins>Clustering:</ins> Using non-uniform quantization grid to quantize the weights and activations to match their distributions.[*](#experimental-features)
-* <ins>Mixed-precision search:</ins> Assigning quantization bit-width per layer (for weights/activations), based on the layer's sensitivity to different bit-widths.
-* <ins>Visualization:</ins> You can use TensorBoard to observe useful information for troubleshooting the quantized model's performance (for example, the model in different phases of the quantization, collected statistics, similarity between layers of the float and quantized model and bit-width configuration for mixed-precision quantization). For more details, please read the [visualization documentation](https://sony.github.io/model_optimization/docs/guidelines/visualization.html).   
-* <ins>Target Platform Capabilities:</ins> The Target Platform Capabilities (TPC) describes the target platform (an edge device with dedicated hardware). For more details, please read the [TPC README](model_compression_toolkit/target_platform_capabilities/README.md).   
-
-### Enhanced Post-Training Quantization (EPTQ)
-As part of the GPTQ we provide an advanced optimization algorithm called EPTQ.
-
-The specifications of the algorithm are detailed in the paper: _"**EPTQ: Enhanced Post-Training Quantization via Label-Free Hessian**"_ [4].
-
-More details on the how to use EPTQ via MCT can be found in the [EPTQ guidelines](model_compression_toolkit/gptq/README.md).
-
-
-### Structured Pruning [*](#experimental-features)
-MCT introduces a structured and hardware-aware model pruning.
-This pruning technique is designed to compress models for specific hardware architectures, 
-taking into account the target platform's Single Instruction, Multiple Data (SIMD) capabilities. 
-By pruning groups of channels (SIMD groups), our approach not only reduces model size 
-and complexity, but ensures that better utilization of channels is in line with the SIMD architecture 
-for a target Resource Utilization of weights memory footprint.
-[Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_pruning_experimental.html)
-[Pytorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_pruning_experimental.html) 
-
-#### Experimental features 
-
-Some features are experimental and subject to future changes. 
- 
-For more details, we highly recommend visiting our project website where experimental features are mentioned as experimental.
-
-
-## Results
-### Keras
-Graph of [MobileNetV2](https://keras.io/api/applications/mobilenet/) accuracy on ImageNet vs average bit-width of weights, using 
-single-precision quantization, mixed-precision quantization, and mixed-precision quantization with GPTQ.
-
-<img src="docsrc/images/mbv2_accuracy_graph.png">
-
-For more results, please see [1]
-
-### Pytorch
-We quantized classification networks from the torchvision library. 
-In the following table we present the ImageNet validation results for these models:
-
-| Network Name              | Float Accuracy  | 8Bit Accuracy   | Data-Free 8Bit Accuracy |
-|---------------------------|-----------------|-----------------|-------------------------|
-| MobileNet V2 [3]          | 71.886          | 71.444          |71.29|
-| ResNet-18 [3]             | 69.86           | 69.63           |69.53|
-| SqueezeNet 1.1 [3]        | 58.128          | 57.678          ||
-
-For more results, please refer to [quick start](https://github.com/sony/model_optimization/tree/main/tutorials/quick_start).
-
-
-#### Pruning Results
-
-Results for applying pruning to reduce the parameters of the following models by 50%:
-
-| Model           | Dense Model Accuracy | Pruned Model Accuracy |
-|-----------------|----------------------|-----------------------|
-| ResNet50 [2]    | 75.1                 | 72.4                  |
-| DenseNet121 [3] | 74.44                | 71.71                 |
-
-
-## Trouble Shooting
-
-If the accuracy degradation of the quantized model is too large for your application, check out the [Quantization Troubleshooting](https://github.com/sony/model_optimization/tree/main/quantization_troubleshooting.md)
-for common pitfalls and some tools to improve quantization accuracy.
-
-Check out the [FAQ](https://github.com/sony/model_optimization/tree/main/FAQ.md) for common issues.
-
-
-## Contributions
-MCT aims at keeping a more up-to-date fork and welcomes contributions from anyone.
-
-*You will find more information about contributions in the [Contribution guide](CONTRIBUTING.md).
-
-
-## License
-[Apache License 2.0](LICENSE.md).
-
-## References 
-
-[1] Habi, H.V., Peretz, R., Cohen, E., Dikstein, L., Dror, O., Diamant, I., Jennings, R.H. and Netzer, A., 2021. [HPTQ: Hardware-Friendly Post Training Quantization. arXiv preprint](https://arxiv.org/abs/2109.09113).
-
-[2] [Keras Applications](https://keras.io/api/applications/)
-
-[3] [TORCHVISION.MODELS](https://pytorch.org/vision/stable/models.html) 
-
-[4] Gordon, O., Habi, H. V., & Netzer, A., 2023. [EPTQ: Enhanced Post-Training Quantization via Label-Free Hessian. arXiv preprint](https://arxiv.org/abs/2309.11531)
+Metadata-Version: 2.1
+Name: model_compression_toolkit
+Version: 2.1.0
+Summary: A Model Compression Toolkit for neural networks
+Home-page: UNKNOWN
+License: UNKNOWN
+Description: # Model Compression Toolkit (MCT)
+        
+        Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
+        
+        This project provides researchers, developers, and engineers tools for optimizing and deploying state-of-the-art neural networks on efficient hardware.
+        
+        Specifically, this project aims to apply quantization to compress neural networks.
+        
+        <img src="https://github.com/sony/model_optimization/raw/main/docsrc/images/mct_block_diagram.svg" width="10000">
+        
+        MCT is developed by researchers and engineers working at Sony Semiconductor Israel.
+        
+        
+        
+        ## Table of Contents
+        
+        - [Getting Started](https://github.com/sony/model_optimization?tab=readme-ov-file#getting-started)
+        - [Supported features](https://github.com/sony/model_optimization?tab=readme-ov-file#supported-features)
+        - [Results](https://github.com/sony/model_optimization?tab=readme-ov-file#results)
+        - [Troubleshooting](https://github.com/sony/model_optimization?tab=readme-ov-file#trouble-shooting)
+        - [Contributions](https://github.com/sony/model_optimization?tab=readme-ov-file#contributions)
+        - [License](https://github.com/sony/model_optimization?tab=readme-ov-file#license)
+        
+        
+        ## Getting Started
+        
+        This section provides an installation and a quick starting guide.
+        
+        ### Installation
+        
+        To install the latest stable release of MCT, run the following command:
+        ```
+        pip install model-compression-toolkit
+        ```
+        
+        For installing the nightly version or installing from source, refer to the [installation guide](https://github.com/sony/model_optimization/blob/main/INSTALLATION.md).
+        
+        
+        ### Quick start & tutorials 
+        
+        Explore the Model Compression Toolkit (MCT) through our tutorials, 
+        covering compression techniques for Keras and PyTorch models. Access interactive [notebooks](https://github.com/sony/model_optimization/blob/main/tutorials/README.md) 
+        for hands-on learning. For example:
+        * [Keras MobileNetV2 post training quantization](https://github.com/sony/model_optimization/blob/main/tutorials/notebooks/imx500_notebooks/keras/example_keras_mobilenetv2_for_imx500.ipynb)
+        * [Post training quantization with PyTorch](https://github.com/sony/model_optimization/blob/main/tutorials/notebooks/mct_features_notebooks/pytorch/example_pytorch_ptq_mnist.ipynb)
+        * [Data Generation for ResNet18 with PyTorch](https://github.com/sony/model_optimization/blob/main/tutorials/notebooks/mct_features_notebooks/pytorch/example_pytorch_data_generation.ipynb).
+        
+        
+        ### Supported Versions
+        
+        Currently, MCT is being tested on various Python, Pytorch and TensorFlow versions:
+        
+        |             |  PyTorch 1.13                                                                                                                                                                                                               | PyTorch 2.0                                                                                                                                                                                                              | PyTorch 2.1                                                                                                                                                                                                              |
+        |-------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+        | Python 3.9  | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch113.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch113.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch20.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch20.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch21.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_pytorch21.yml)   |
+        | Python 3.10 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch112.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch112.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch113.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch113.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch20.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch20.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch21.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_pytorch21.yml) |
+        | Python 3.11 | | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch20.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch20.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch21.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_pytorch21.yml) |
+        
+        
+        |             | TensorFlow 2.12                                                                                                                                                                                                                        | TensorFlow 2.13                                                                                                                                                                                                                        | TensorFlow 2.14                                                                                                                                                                                                                        | TensorFlow 2.15                                                                                                                                                                                                        |
+        |-------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+        | Python 3.9  | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras212.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras213.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras214.yml)   | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python39_keras215.yml)   |
+        | Python 3.10 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras212.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras213.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras214.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras215.yml) |
+        | Python 3.11 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras212.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras213.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras214.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras215.yml) |
+        
+        
+        ## Supported Features
+        MCT offers a range of powerful features to optimize neural network models for efficient deployment. These supported features include:
+        
+        ### Data Generation [*](https://github.com/sony/model_optimization?tab=readme-ov-file#experimental-features)
+        MCT provides tools for generating synthetic images based on the statistics stored in a model's batch normalization layers. These generated images are valuable for various compression tasks where image data is required, such as quantization and pruning. 
+        You can customize data generation configurations to suit your specific needs. [Go to the Data Generation page.](https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/data_generation/README.md)
+        
+        ### Quantization
+        MCT supports different quantization methods:
+        * Post-training quantization (PTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_post_training_quantization.html), [PyTorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_post_training_quantization.html)
+        * Gradient-based post-training quantization (GPTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_gradient_post_training_quantization.html), [PyTorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_gradient_post_training_quantization.html)
+        * Quantization-aware training (QAT) [*](https://github.com/sony/model_optimization?tab=readme-ov-file#experimental-features)
+        
+        
+        | Quantization Method                           | Complexity | Computational Cost          |
+        |-----------------------------------------------|------------|-----------------------------|
+        | PTQ                                           | Low        | Low (order of minutes)      |
+        | GPTQ (parameters fine-tuning using gradients) | Mild       | Mild (order of 2-3 hours)   |
+        | QAT                                           | High       | High (order of 12-36 hours) |
+        
+        
+        In addition, MCT supports different quantization schemes for quantizing weights and activations:
+        
+        * Power-Of-Two (hardware-friendly quantization [1])
+        * Symmetric
+        * Uniform
+        
+        Main features:
+        * <ins>Graph optimizations:</ins> Transforming the model to an equivalent (yet, more efficient) model (for example, batch-normalization layer folding to its preceding linear layer).
+        * <ins>Quantization parameter search:</ins> Different methods can be used to minimize the expected added quantization-noise during thresholds search (by default, we use Mean-Square-Error, but other metrics can be used such as No-Clipping, Mean-Average-Error, and more).
+        * <ins>Advanced quantization algorithms:</ins> To prevent a performance degradation some algorithms are applied such as: 
+          * <ins>Shift negative correction:</ins> Symmetric activation quantization can hurt the model's performance when some layers output both negative and positive activations, but their range is asymmetric. For more details please visit [1].
+          * <ins>Outliers filtering:</ins> Computing z-score for activation statistics to detect and remove outliers.
+        * <ins>Clustering:</ins> Using non-uniform quantization grid to quantize the weights and activations to match their distributions.[*](https://github.com/sony/model_optimization?tab=readme-ov-file#experimental-features)
+        * <ins>Mixed-precision search:</ins> Assigning quantization bit-width per layer (for weights/activations), based on the layer's sensitivity to different bit-widths.
+        * <ins>Visualization:</ins> You can use TensorBoard to observe useful information for troubleshooting the quantized model's performance (for example, the model in different phases of the quantization, collected statistics, similarity between layers of the float and quantized model and bit-width configuration for mixed-precision quantization). For more details, please read the [visualization documentation](https://sony.github.io/model_optimization/docs/guidelines/visualization.html).   
+        * <ins>Target Platform Capabilities:</ins> The Target Platform Capabilities (TPC) describes the target platform (an edge device with dedicated hardware). For more details, please read the [TPC README](https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/target_platform_capabilities/README.md).   
+        
+        ### Enhanced Post-Training Quantization (EPTQ)
+        As part of the GPTQ we provide an advanced optimization algorithm called EPTQ.
+        
+        The specifications of the algorithm are detailed in the paper: _"**EPTQ: Enhanced Post-Training Quantization via Label-Free Hessian**"_ [4].
+        
+        More details on the how to use EPTQ via MCT can be found in the [EPTQ guidelines](https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/gptq/README.md).
+        
+        
+        ### Structured Pruning [*](https://github.com/sony/model_optimization?tab=readme-ov-file#experimental-features)
+        MCT introduces a structured and hardware-aware model pruning.
+        This pruning technique is designed to compress models for specific hardware architectures, 
+        taking into account the target platform's Single Instruction, Multiple Data (SIMD) capabilities. 
+        By pruning groups of channels (SIMD groups), our approach not only reduces model size 
+        and complexity, but ensures that better utilization of channels is in line with the SIMD architecture 
+        for a target Resource Utilization of weights memory footprint.
+        [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_pruning_experimental.html)
+        [Pytorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_pruning_experimental.html) 
+        
+        #### Experimental features 
+        
+        Some features are experimental and subject to future changes. 
+         
+        For more details, we highly recommend visiting our project website where experimental features are mentioned as experimental.
+        
+        
+        ## Results
+        ### Keras
+        Graph of [MobileNetV2](https://keras.io/api/applications/mobilenet/) accuracy on ImageNet vs average bit-width of weights, using 
+        single-precision quantization, mixed-precision quantization, and mixed-precision quantization with GPTQ.
+        
+        <img src="https://github.com/sony/model_optimization/raw/main/docsrc/images/mbv2_accuracy_graph.png">
+        
+        For more results, please see [1]
+        
+        ### Pytorch
+        We quantized classification networks from the torchvision library. 
+        In the following table we present the ImageNet validation results for these models:
+        
+        | Network Name              | Float Accuracy  | 8Bit Accuracy   | Data-Free 8Bit Accuracy |
+        |---------------------------|-----------------|-----------------|-------------------------|
+        | MobileNet V2 [3]          | 71.886          | 71.444          |71.29|
+        | ResNet-18 [3]             | 69.86           | 69.63           |69.53|
+        | SqueezeNet 1.1 [3]        | 58.128          | 57.678          ||
+        
+        
+        #### Pruning Results
+        
+        Results for applying pruning to reduce the parameters of the following models by 50%:
+        
+        | Model           | Dense Model Accuracy | Pruned Model Accuracy |
+        |-----------------|----------------------|-----------------------|
+        | ResNet50 [2]    | 75.1                 | 72.4                  |
+        | DenseNet121 [3] | 74.44                | 71.71                 |
+        
+        
+        ## Trouble Shooting
+        
+        If the accuracy degradation of the quantized model is too large for your application, check out the [Quantization Troubleshooting](https://github.com/sony/model_optimization/tree/main/quantization_troubleshooting.md)
+        for common pitfalls and some tools to improve quantization accuracy.
+        
+        Check out the [FAQ](https://github.com/sony/model_optimization/tree/main/FAQ.md) for common issues.
+        
+        
+        ## Contributions
+        MCT aims at keeping a more up-to-date fork and welcomes contributions from anyone.
+        
+        *You will find more information about contributions in the [Contribution guide](https://github.com/sony/model_optimization/blob/main/CONTRIBUTING.md).
+        
+        
+        ## License
+        [Apache License 2.0](https://github.com/sony/model_optimization/blob/main/LICENSE.md).
+        
+        ## References 
+        
+        [1] Habi, H.V., Peretz, R., Cohen, E., Dikstein, L., Dror, O., Diamant, I., Jennings, R.H. and Netzer, A., 2021. [HPTQ: Hardware-Friendly Post Training Quantization. arXiv preprint](https://arxiv.org/abs/2109.09113).
+        
+        [2] [Keras Applications](https://keras.io/api/applications/)
+        
+        [3] [TORCHVISION.MODELS](https://pytorch.org/vision/stable/models.html) 
+        
+        [4] Gordon, O., Habi, H. V., & Netzer, A., 2023. [EPTQ: Enhanced Post-Training Quantization via Label-Free Hessian. arXiv preprint](https://arxiv.org/abs/2309.11531)
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 from model_compression_toolkit import qat
 from model_compression_toolkit import exporter
 from model_compression_toolkit import gptq
 from model_compression_toolkit import data_generation
 from model_compression_toolkit import pruning
 from model_compression_toolkit.trainable_infrastructure.keras.load_model import keras_load_quantized_model
 
-__version__ = "2.0.0"
+__version__ = "2.1.0"
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/constants.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,23 @@
 import importlib
 
 # Supported frameworks in MCT:
 TENSORFLOW = 'tensorflow'
 PYTORCH = 'pytorch'
 FOUND_TF = importlib.util.find_spec(TENSORFLOW) is not None
 FOUND_TORCH = importlib.util.find_spec("torch") is not None
+FOUND_TORCHVISION = importlib.util.find_spec("torchvision") is not None
 FOUND_ONNX = importlib.util.find_spec("onnx") is not None
 FOUND_ONNXRUNTIME = importlib.util.find_spec("onnxruntime") is not None
 FOUND_SONY_CUSTOM_LAYERS = importlib.util.find_spec('sony_custom_layers') is not None
 
+# Metadata fields
+MCT_VERSION = 'mct_version'
+TPC_VERSION = 'tpc_version'
+
 WEIGHTS_SIGNED = True
 # Minimal threshold to use for quantization ranges:
 MIN_THRESHOLD = (2 ** -16)
 EPS = 1e-8
 LUT_VALUES_BITWIDTH = 8
 FP32_BYTES_PER_PARAMETER = 4.
 
@@ -89,14 +94,16 @@
 DEFAULT_DEC_FACTOR = (1.02, 0.98)
 DEFAULT_TOL = 1e-11
 BOTTOM_FACTOR = 0.7
 UPPER_FACTOR = 1.2
 DEC_RANGE_BOTTOM = 0.97
 DEC_RANGE_UPPER = 1.03
 
+NUM_QPARAM_HESSIAN_SAMPLES = 16
+
 # Resource utilization computation parameters
 BITS_TO_BYTES = 8.0
 
 # Default threshold for Softmax layer
 SOFTMAX_THRESHOLD = 1
 
 # Substitutions node names
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/analyzer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/analyzer.py`

 * *Files 23% similar despite different names*

```diff
@@ -26,38 +26,48 @@
 
 from model_compression_toolkit.core.common.visualization.tensorboard_writer import TensorboardWriter
 from model_compression_toolkit.logger import Logger
 
 
 def analyzer_model_quantization(representative_data_gen: Callable,
                                 tb_w: TensorboardWriter,
-                                tg: Graph,
+                                float_graph: Graph,
+                                quantized_graph: Graph,
                                 fw_impl: FrameworkImplementation,
                                 fw_info: FrameworkInfo):
     """
     Plot the cosine similarity of different points on the graph between the float and quantized
     graphs. Add them to the passed TensorboardWriter object and close all tensorboard writer open
     files.
 
     Args:
         representative_data_gen: Dataset used for calibration.
         tb_w: TensorBoardWriter object to log events.
-        tg: Graph of quantized model.
+        float_graph: Graph of float model.
+        quantized_graph: Graph of quantized model.
         fw_impl: FrameworkImplementation object with a specific framework methods implementation.
         fw_info: Information needed for quantization about the specific framework.
 
     """
     if tb_w is not None:
-        visual = NNVisualizer(tg,
+        visual = NNVisualizer(float_graph,
+                              quantized_graph,
                               fw_impl=fw_impl,
                               fw_info=fw_info)
-
-        for i, _data in enumerate(representative_data_gen()):
-            if i >= NUM_SAMPLES_DISTANCE_TENSORBOARD:
-                break
-            figure = visual.plot_distance_graph(_data,
-                                                distance_fn=compute_cs,
-                                                convert_to_range=lambda a: 1 - 2 * a)
-            tb_w.add_figure(figure, f'similarity_distance_sample_{i}')
+        if not visual.has_compare_points():
+            Logger.error(f'No comparing points were found to plot analyze similarity.')
         else:
-            Logger.warning(f'Not enough batches in representative dataset to generate {NUM_SAMPLES_DISTANCE_TENSORBOARD} figures')
+            visualized_samples = 0
+            for _data in representative_data_gen():
+                batch_size = _data[0].shape[0]
+                for sample_index in range(batch_size):
+                    if visualized_samples >= NUM_SAMPLES_DISTANCE_TENSORBOARD:
+                        break
+                    figure = visual.plot_distance_graph(_data,
+                                                        sample_index=sample_index,
+                                                        distance_fn=compute_cs,
+                                                        convert_to_range=lambda a: 1 - 2 * a)
+                    tb_w.add_figure(figure, f'similarity_distance_sample_{visualized_samples}')
+                    visualized_samples += 1
+            if visualized_samples < NUM_SAMPLES_DISTANCE_TENSORBOARD:
+                Logger.error(f'Not enough batches in representative dataset to generate {NUM_SAMPLES_DISTANCE_TENSORBOARD} figures')
         tb_w.close()
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/back2framework/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/back2framework/base_model_builder.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/back2framework/base_model_builder.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/base_substitutions.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/base_substitutions.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/collectors/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/collectors/base_collector.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/collectors/base_collector.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/collectors/histogram_collector.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/collectors/histogram_collector.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/collectors/mean_collector.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/collectors/mean_collector.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/collectors/statistics_collector.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/collectors/statistics_collector.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/framework_implementation.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/framework_implementation.py`

 * *Files 4% similar despite different names*

```diff
@@ -246,23 +246,14 @@
     def get_residual_collapsing_substitution(self) -> List[common.BaseSubstitution]:
         """
         Returns: A list of the framework substitutions used for residual collapsing
         """
         raise NotImplemented(f'{self.__class__.__name__} have to implement the '
                              f'framework\'s get_residual_collapsing_substitution method.')  # pragma: no cover
 
-    @abstractmethod
-    def get_substitutions_pre_build(self) -> List[common.BaseSubstitution]:
-        """
-
-        Returns: A list of the framework substitutions used before we build a quantized model.
-
-        """
-        raise NotImplemented(f'{self.__class__.__name__} have to implement the '
-                             f'framework\'s get_substitutions_pre_build method.')  # pragma: no cover
 
     @abstractmethod
     def get_substitutions_post_statistics_collection(self, quant_config: QuantizationConfig) -> List[
         common.BaseSubstitution]:
         """
         Return a list of the framework substitutions used after we collect statistics.
 
@@ -353,34 +344,36 @@
             node: Node to indicate whether it needs to be part of the interest points set.
         Returns: True if the node should be considered an interest point, False otherwise.
         """
 
         raise NotImplemented(f'{self.__class__.__name__} have to implement the '
                              f'framework\'s count_node_for_mixed_precision_interest_points method.')  # pragma: no cover
 
-    def get_node_distance_fn(self, layer_class: type,
+    def get_mp_node_distance_fn(self, layer_class: type,
                              framework_attrs: Dict[str, Any],
                              compute_distance_fn: Callable = None,
-                             axis: int = None) -> Callable:
+                             axis: int = None,
+                             norm_mse: bool = False) -> Callable:
         """
         A mapping between layers' types and a distance function for computing the distance between
-        two tensors (for loss computation purposes). Returns a specific function if node of specific types is
+        two tensors in mixed precision (for loss computation purposes). Returns a specific function if node of specific types is
         given, or a default (normalized MSE) function otherwise.
 
         Args:
             layer_class: Class path of a model's layer.
             framework_attrs: Framework attributes the layer had which the graph node holds.
             compute_distance_fn: An optional distance function to use globally for all nodes.
             axis: The axis on which the operation is preformed (if specified).
+            norm_mse: whether to normalize mse distance function.
 
         Returns: A distance function between two tensors.
         """
 
         raise NotImplemented(f'{self.__class__.__name__} have to implement the '
-                             f'framework\'s get_node_distance_fn method.')  # pragma: no cover
+                             f'framework\'s get_mp_node_distance_fn method.')  # pragma: no cover
 
 
     @abstractmethod
     def is_output_node_compatible_for_hessian_score_computation(self,
                                                                 node: BaseNode) -> bool:
         """
         Checks and returns whether the given node is compatible as output for Hessian-based information computation.
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/framework_info.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/framework_info.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/fusion/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/fusion/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/fusion/layer_fusing.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/fusion/layer_fusing.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/base_graph.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/base_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,22 +94,23 @@
             tpc: TargetPlatformCapabilities object.
         """
         # validate graph nodes are either from the framework or a custom layer defined in the TPC
         # Validate graph nodes are either built-in layers from the framework or custom layers defined in the TPC
         tpc_layers = tpc.op_sets_to_layers.get_layers()
         tpc_filtered_layers = [layer for layer in tpc_layers if isinstance(layer, LayerFilterParams)]
         for n in self.nodes:
-            is_node_in_tpc = n.type in tpc_layers or any([n.is_match_filter_params(filtered_layer)
-                                                          for filtered_layer in tpc_filtered_layers])
+            is_node_in_tpc = any([n.is_match_type(_type) for _type in tpc_layers]) or \
+                             any([n.is_match_filter_params(filtered_layer) for filtered_layer in tpc_filtered_layers])
             if n.is_custom:
                 if not is_node_in_tpc:
                     Logger.critical(f'MCT does not support optimizing Keras custom layers. Found a layer of type {n.type}. '
-                                 f' Please add the custom layer to Target Platform Capabilities (TPC), or file a feature request or an issue if you believe this should be supported.')
+                                    ' Please add the custom layer to Target Platform Capabilities (TPC), or file a feature '
+                                    'request or an issue if you believe this should be supported.')  # pragma: no cover
                 if any([qc.default_weight_attr_config.enable_weights_quantization for qc in n.get_qco(tpc).quantization_config_list]):
-                    Logger.critical(f'Layer identified: {n.type}. MCT does not support weight quantization for Keras custom layers.')
+                    Logger.critical(f'Layer identified: {n.type}. MCT does not support weight quantization for Keras custom layers.')  # pragma: no cover
 
         self.tpc = tpc
 
     def get_topo_sorted_nodes(self):
         """
         Returns: a list of toposorted nodes.
         """
@@ -409,15 +410,15 @@
 
         Args:
             current_node: Node that (possibly) is an input node.
             new_node: New node to set as an input node if the current node is an input node.
 
         """
         if new_node is None:
-            Logger.critical("Cannot replace input node with a None value; new input node is required.")
+            Logger.critical("Cannot replace input node with a None value; new input node is required.")  # pragma: no cover
 
         graph_inputs = self.get_inputs()
         new_graph_inputs = copy(graph_inputs)
         if current_node in graph_inputs:
             new_graph_inputs.remove(current_node)
             new_graph_inputs.append(new_node)
         self.set_inputs(new_graph_inputs)
@@ -823,20 +824,20 @@
             entry_node (BaseNode): The entry node to create the section it starts.
             fw_impl (PruningFrameworkImplementation): Implementation of specific framework methods required for pruning.
 
         Returns: The pruning section that starts with node entry_node.
 
         """
         if not fw_impl.is_node_entry_node(entry_node):
-            Logger.critical(f"Node {entry_node} is not a valid entry node for creating a pruning section")
+            Logger.critical(f"Node {entry_node} is not a valid entry node for creating a pruning section")  # pragma: no cover
 
         intermediate_nodes, exit_node = self._find_intermediate_and_exit_nodes(entry_node, fw_impl)
 
         if not fw_impl.is_node_exit_node(exit_node, entry_node, self.fw_info):
-            Logger.critical(f"Node {exit_node} is not a valid exit node for the pruning section starting with {entry_node}.")
+            Logger.critical(f"Node {exit_node} is not a valid exit node for the pruning section starting with {entry_node}.")   # pragma: no cover
 
         return PruningSection(entry_node=entry_node,
                               intermediate_nodes=intermediate_nodes,
                               exit_node=exit_node)
 
     def _find_intermediate_and_exit_nodes(self, entry_node: BaseNode, fw_impl: Any) -> Tuple[List[BaseNode], BaseNode]:
         """
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/base_node.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/base_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import copy
-from typing import Dict, Any, Tuple, List, Type
+from typing import Dict, Any, Tuple, List, Type, Union
 
 import numpy as np
 
 from model_compression_toolkit.constants import WEIGHTS_NBITS_ATTRIBUTE, CORRECTED_BIAS_ATTRIBUTE, \
     ACTIVATION_NBITS_ATTRIBUTE, FP32_BYTES_PER_PARAMETER
 from model_compression_toolkit.core.common.quantization.node_quantization_config import WeightsAttrQuantizationConfig
 from model_compression_toolkit.logger import Logger
@@ -92,14 +92,24 @@
         Returns has_activation attribute.
 
         Returns: Whether the node has activation to quantize.
 
         """
         return self.has_activation
 
+    @property
+    def has_positional_weights(self):
+        """
+        Returns has_positional_weights attribute.
+
+        Returns: Whether the node has positional weights.
+
+        """
+        return any(isinstance(key, int) for key in self.weights.keys())
+
     def is_activation_quantization_enabled(self) -> bool:
         """
 
         Returns: Whether node activation quantization is enabled or not.
 
         """
         if self.final_activation_quantization_cfg:
@@ -147,27 +157,41 @@
         """
         Check whether the node is reused or not
         Returns:
             True if node is reused, else False
         """
         return self.reuse or self.reuse_group is not None
 
-    def get_weights_by_keys(self, name: str) -> np.ndarray:
+    def _get_weight_name(self, name: Union[str, int]) -> List[Union[str, int]]:
+        """
+        Get weight names that match argument name (either string weights or integer for
+        positional weights).
+        Args:
+            name: weight name
+
+        Returns:
+            A list of weight names that match input "name"
+
+        """
+        return [k for k in self.weights.keys()
+                if (isinstance(k, int) and name == k) or (isinstance(k, str) and name in k)]
+
+    def get_weights_by_keys(self, name: Union[str, int]) -> np.ndarray:
         """
         Get a node's weight by its name.
         Args:
             name: Name of the variable for a node's weight.
 
         Returns:
             A node's weight (by its name).
         """
         if name is None:
             return None
 
-        res = [k for k in self.weights.keys() if name in k]
+        res = self._get_weight_name(name)
         if len(res) == 1:  # Make sure there are no duplicates
             return self.weights[res[0]]
         else:
             return None
 
     def set_weights_by_keys(self, name: str, tensor: np.ndarray):
         """
@@ -175,15 +199,15 @@
 
         Args:
             name: Name of the weight the node holds.
             tensor: Numpy array to set as the weight.
 
         """
 
-        res = [k for k in self.weights.keys() if name in k]
+        res = self._get_weight_name(name)
         if len(res) == 1:
             self.weights[res[0]] = tensor
         else:  # Add if not exist
             self.weights[name] = tensor
             self.weights_keys = list(self.weights.keys())  # update keys
 
     def get_weights_list(self):
@@ -210,16 +234,20 @@
         Args:
             input_tensors: activation input tensors to node.
         Returns:
             Activation input tensors list with positional weights
         """
         for pos, weight in sorted((pos, weight) for pos, weight in self.weights.items()
                                   if isinstance(pos, int)):
-            assert pos <= len(input_tensors), 'Positional weight index mismatch'
-            input_tensors.insert(pos, weight)
+            if pos > len(input_tensors):
+                Logger.critical("The positional weight index cannot exceed the number of input tensors to the node.")  # pragma: no cover
+            # Insert only positional weights that are not subject to quantization. If the positional weight is
+            # subject to quantization, the quantization wrapper inserts the positional weight into the node.
+            if not self.is_weights_quantization_enabled(pos):
+                input_tensors.insert(pos, weight)
 
         return input_tensors
 
     def get_num_parameters(self, fw_info) -> Tuple[int,int]:
         """
         Compute the number of parameters the node holds.
         It returns a tuple: Number of quantized parameters, number of float parameters.
@@ -548,30 +576,33 @@
 
         if tpc is None:
             Logger.critical(f'Can not retrieve QC options for None TPC')  # pragma: no cover
 
         for fl, qco in tpc.filterlayer2qco.items():
             if self.is_match_filter_params(fl):
                 return qco
-        if self.type in tpc.layer2qco:
-            return tpc.layer2qco.get(self.type)
+        # Extract qco with is_match_type to overcome mismatch of function types in TF 2.15
+        matching_qcos = [_qco for _type, _qco in tpc.layer2qco.items() if self.is_match_type(_type)]
+        if matching_qcos:
+            if len(matching_qcos) > 1:
+                Logger.error('Found duplicate qco types!')
+            return matching_qcos[0]
         return tpc.tp_model.default_qco
 
     def is_match_type(self, _type: Type) -> bool:
         """
-        Check if input type matches the node type, either in instance type or in type name. Checking the
-        name string is required because of function types changes that occurred in TF 2.15.
+        Check if input type matches the node type, either in instance type or in type name.
 
         Args:
             _type: other node type
         Returns:
             Whether _type matches the self node type
 
         """
-        return _type == self.type or _type.__name__ == self.type.__name__
+        return _type == self.type
 
     def is_match_filter_params(self, layer_filter_params: LayerFilterParams) -> bool:
         """
         Check if the node matches a LayerFilterParams according to its
         layer, conditions and keyword-arguments.
 
         Args:
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/edge.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/edge.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/functional_node.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/functional_node.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from typing import Dict, Any, Tuple, List
+from typing import Dict, Any, Tuple, Type
 
+from model_compression_toolkit.constants import FOUND_TF
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
 import numpy as np
 
 
 class FunctionalNode(BaseNode):
     """
     Node that represents function ops with arguments to pass when building back the model.
@@ -67,7 +68,23 @@
     @property
     def type(self):
         """
         A function to get the node's function op for convenient comparison (instead of the layer_class)
         :return: the node's functional_op
         """
         return self.functional_op
+
+    def is_match_type(self, _type: Type) -> bool:
+        """
+        Check if input type matches the node type, either in instance type or in type name. Checking the
+        name string is required because of function types changes that occurred in TF 2.15, because it
+        changes the "function" attribute object (e.g. a different tf.add function that will fail the
+        equal operation).
+
+        Args:
+            _type: other node type
+        Returns:
+            Whether _type matches the self node type
+
+        """
+        names_match = _type.__name__ == self.type.__name__ if FOUND_TF else False
+        return super().is_match_type(_type) or names_match
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/graph_matchers.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/graph_matchers.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/graph_searches.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/graph_searches.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/memory_graph/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/memory_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/memory_graph/cut.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/memory_graph/cut.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/hessian/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/hessian/hessian_info_service.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/hessian/hessian_info_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 # ==============================================================================
 
 from functools import partial
 from typing import Callable, List
 
 from model_compression_toolkit.constants import HESSIAN_NUM_ITERATIONS
-from model_compression_toolkit.core.common import Graph
 from model_compression_toolkit.core.common.hessian.trace_hessian_request import TraceHessianRequest
 from model_compression_toolkit.logger import Logger
 
 
 class HessianInfoService:
     """
     A service to manage, store, and compute approximation of the Hessian-based information.
@@ -34,15 +33,15 @@
     Note:
     - The Hessian provides valuable information about the curvature of the loss function.
     - Computation can be computationally heavy and time-consuming.
     - The computed trace is an approximation.
     """
 
     def __init__(self,
-                 graph: Graph,
+                 graph,
                  representative_dataset: Callable,
                  fw_impl,
                  num_iterations_for_approximation: int = HESSIAN_NUM_ITERATIONS
                  ):
         """
 
         Args:
@@ -147,15 +146,15 @@
             The outer list is per image (thus, has the length as required_size).
             The inner list length dependent on the granularity (1 for per-tensor, 
             OC for per-output-channel when the requested node has OC output-channels, etc.)
         """
         if required_size==0:
             return []
 
-        Logger.info(f"Ensuring {required_size} Hessian-trace approximation for node {trace_hessian_request.target_node}.")
+        Logger.info(f"\nEnsuring {required_size} Hessian-trace approximation for node {trace_hessian_request.target_node}.")
 
         # Replace request of a reused target node with a request of the 'reuse group'.
         if trace_hessian_request.target_node.reuse_group:
             trace_hessian_request = self._get_request_of_reuse_group(trace_hessian_request)
 
         # Ensure the saved info has the required number of approximations
         self._populate_saved_info_to_size(trace_hessian_request, required_size)
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/hessian/hessian_info_utils.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/hessian/hessian_info_utils.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/hessian/trace_hessian_request.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/hessian/trace_hessian_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List
 
 from enum import Enum
 
-from model_compression_toolkit.core.common import BaseNode
-
 
 class HessianMode(Enum):
     """
     Enum representing the mode for Hessian information computation.
 
     This determines whether the Hessian's approximation is computed w.r.t weights or w.r.t activations.
     Note: This is not the actual Hessian but an approximation.
@@ -50,15 +48,15 @@
     It specifies the mode (weights/activations), granularity (element/channel/tensor), and the target node.
     Note: This does not compute the actual Hessian's trace but approximates it.
     """
 
     def __init__(self,
                  mode: HessianMode,
                  granularity: HessianInfoGranularity,
-                 target_node: BaseNode,
+                 target_node,
                  ):
         """
         Attributes:
             mode (HessianMode): Mode of Hessian's trace approximation (w.r.t weights or activations).
             granularity (HessianInfoGranularity): Granularity level for the approximation.
             target_node (BaseNode): The node in the float graph for which the Hessian's trace approximation is targeted.
         """
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/matchers/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/matchers/base_graph_filter.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/matchers/base_graph_filter.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/matchers/base_matcher.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/matchers/base_matcher.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/matchers/edge_matcher.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/matchers/edge_matcher.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/matchers/function.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/matchers/function.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/matchers/node_matcher.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/matchers/node_matcher.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/matchers/walk_matcher.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/matchers/walk_matcher.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/memory_computation.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/memory_computation.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
     """
 
     mp_nodes = graph.get_configurable_sorted_nodes_names(fw_info)
 
     # Go over all nodes that should be taken into consideration when computing the BOPS utilization.
     bops = []
     for n in graph.get_topo_sorted_nodes():
-        if n.has_kernel_weight_to_quantize(fw_info):
+        if n.has_kernel_weight_to_quantize(fw_info) and not n.has_positional_weights:
             # If node doesn't have weights then its MAC count is 0, and we shouldn't consider it in the BOPS count.
             incoming_edges = graph.incoming_edges(n, sort_by_attr=EDGE_SINK_INDEX)
             if len(incoming_edges) != 1:
                 Logger.critical(f"Unable to compute BOPS metric for node {n.name} due to multiple inputs.")  # pragma: no cover
             input_activation_node = incoming_edges[0].source_node
             if len(graph.out_edges(input_activation_node)) > 1:
                 # In the case where the activation node has multiple outgoing edges
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,18 +85,21 @@
 
         # Get interest points and output points set for distance measurement and set other helper datasets
         # We define a separate set of output nodes of the model for the purpose of sensitivity computation.
         self.interest_points = get_mp_interest_points(graph,
                                                       fw_impl.count_node_for_mixed_precision_interest_points,
                                                       quant_config.num_interest_points_factor)
 
-        self.ips_distance_fns, self.ips_axis = self._init_metric_points_lists(self.interest_points)
+        # We use normalized MSE when not running hessian-based. For Hessian-based normalized MSE is not needed
+        # beacause hessian weights already do normalization.
+        use_normalized_mse = self.quant_config.use_hessian_based_scores is False
+        self.ips_distance_fns, self.ips_axis = self._init_metric_points_lists(self.interest_points, use_normalized_mse)
 
         self.output_points = get_output_nodes_for_metric(graph)
-        self.out_ps_distance_fns, self.out_ps_axis = self._init_metric_points_lists(self.output_points)
+        self.out_ps_distance_fns, self.out_ps_axis = self._init_metric_points_lists(self.output_points, use_normalized_mse)
 
         # Setting lists with relative position of the interest points
         # and output points in the list of all mp model activation tensors
         graph_sorted_nodes = self.graph.get_topo_sorted_nodes()
         all_out_tensors_indices = [graph_sorted_nodes.index(n) for n in self.interest_points + self.output_points]
         global_ipts_indices = [graph_sorted_nodes.index(n) for n in self.interest_points]
         global_out_pts_indices = [graph_sorted_nodes.index(n) for n in self.output_points]
@@ -124,35 +127,37 @@
         # Computing Hessian-based scores for weighted average distance metric computation (only if requested),
         # and assigning distance_weighting method accordingly.
         self.interest_points_hessians = None
         if self.quant_config.use_hessian_based_scores is True:
             self.interest_points_hessians = self._compute_hessian_based_scores()
             self.quant_config.distance_weighting_method = lambda d: self.interest_points_hessians
 
-    def _init_metric_points_lists(self, points: List[BaseNode]) -> Tuple[List[Callable], List[int]]:
+    def _init_metric_points_lists(self, points: List[BaseNode], norm_mse: bool = False) -> Tuple[List[Callable], List[int]]:
         """
         Initiates required lists for future use when computing the sensitivity metric.
         Each point on which the metric is computed uses a dedicated distance function based on its type.
         In addition, all distance functions preform batch computation. Axis is needed only for KL Divergence computation.
 
         Args:
             points: The set of nodes in the graph for which we need to initiate the lists.
+            norm_mse: whether to normalize mse distance function.
 
         Returns: A lists with distance functions and an axis list for each node.
 
         """
         distance_fns_list = []
         axis_list = []
         for n in points:
             axis = n.framework_attr.get(AXIS) if not isinstance(n, FunctionalNode) else n.op_call_kwargs.get(AXIS)
-            distance_fn = self.fw_impl.get_node_distance_fn(
+            distance_fn = self.fw_impl.get_mp_node_distance_fn(
                 layer_class=n.layer_class,
                 framework_attrs=n.framework_attr,
                 compute_distance_fn=self.quant_config.compute_distance_fn,
-                axis=axis)
+                axis=axis,
+                norm_mse=norm_mse)
             distance_fns_list.append(distance_fn)
             # Axis is needed only for KL Divergence calculation, otherwise we use per-tensor computation
             axis_list.append(axis if distance_fn==compute_kl_divergence else None)
         return distance_fns_list, axis_list
 
     def compute_metric(self,
                        mp_model_configuration: List[int],
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/model_builder_mode.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/model_builder_mode.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/model_collector.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/model_collector.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/model_validation.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/model_validation.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/network_editors/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/network_editors/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/network_editors/actions.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/network_editors/actions.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/network_editors/edit_network.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/network_editors/edit_network.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/network_editors/node_filters.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/network_editors/node_filters.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 from typing import Any
 from model_compression_toolkit.core.common.matchers.node_matcher import BaseNodeMatcher
+from model_compression_toolkit.core.common.graph.base_node import BaseNode
 
 
 class NodeTypeFilter(BaseNodeMatcher):
     """
     Class NodeNameFilter to check if a node is of a specific type.
     """
     def __init__(self, node_type):
@@ -26,25 +27,25 @@
         Init a NodeTypeFilter object.
 
         Args:
             node_type: Node type to check.
         """
         self.node_type = node_type
 
-    def apply(self, input_object: Any) -> bool:
+    def apply(self, input_object: BaseNode) -> bool:
         """
         Check if input_object is of the type that NodeTypeFilter contains.
 
         Args:
             input_object: Node object to check for its type.
 
         Returns:
-            True if the node if of the type that was passed during the initialization of NodeTypeFilter.
+            True if the node is of the type that was passed during the initialization of NodeTypeFilter.
         """
-        if input_object.type == self.node_type:
+        if input_object.is_match_type(self.node_type):
             return True
 
 
 class NodeNameFilter(BaseNodeMatcher):
     """
     Class NodeNameFilter to check if a node's name has a specific value.
     """
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/node_prior_info.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/node_prior_info.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/channels_grouping.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/channels_grouping.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/mask/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
         Args:
             node: The prunable node to update the mask for.
             channel_idx: The index of the channel to update in the mask.
             mask_indicator: The new value to set in the mask (either PRUNED or REMAINED).
         """
         if mask_indicator not in [MaskIndicator.PRUNED, MaskIndicator.REMAINED]:
-            Logger.critical("Mask value must be either 'MaskIndicator.PRUNED' or 'MaskIndicator.REMAINED'")
+            Logger.critical("Mask value must be either 'MaskIndicator.PRUNED' or 'MaskIndicator.REMAINED'")  # pragma: no cover
         self._mask[node][channel_idx] = mask_indicator.value
 
     def has_pruned_channel(self) -> bool:
         """
         Determines if there is at least one pruned channel across all nodes in the model.
 
         Returns:
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         Args:
             node: The prunable node to update the mask for.
             group_index: The index of the SIMD group to update in the mask.
             mask_indicator: The new value to set in the mask (either PRUNED or REMAINED).
         """
         if mask_indicator not in [MaskIndicator.PRUNED, MaskIndicator.REMAINED]:
-            Logger.critical("Mask value must be either 'MaskIndicator.PRUNED' or 'MaskIndicator.REMAINED'")
+            Logger.critical("Mask value must be either 'MaskIndicator.PRUNED' or 'MaskIndicator.REMAINED'")  # pragma: no cover
 
         # Update the SIMD group mask and corresponding per-channel mask
         self._mask_simd[node][group_index] = mask_indicator.value
         node_mask_indices = self.simd_groups_indices[node][group_index]
         for idx in node_mask_indices:
             self.per_channel_mask.set_mask_value_for_simd_group(node=node,
                                                                 channel_idx=idx,
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/memory_calculator.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/memory_calculator.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/prune_graph.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/prune_graph.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/pruner.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/pruner.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                                                    self.float_graph,
                                                    self.fw_impl,
                                                    self.target_platform_capabilities,
                                                    self.simd_groups_indices)
             mask_calculator.compute_mask()
             self.per_oc_mask = mask_calculator.get_mask()
         else:
-            Logger.critical("Only GREEDY ChannelsFilteringStrategy is currently supported.")
+            Logger.critical("Only GREEDY ChannelsFilteringStrategy is currently supported.")  # pragma: no cover
 
         Logger.info("Start pruning graph...")
         _pruned_graph = build_pruned_graph(self.float_graph,
                                            self.per_oc_mask,
                                            self.fw_info,
                                            self.fw_impl)
         return _pruned_graph
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/pruning_config.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/pruning_config.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/pruning_info.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/pruning_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         simd_groups_indices (Dict[BaseNode, List[np.ndarray]]): The indices of channels in each SIMD group.
 
     Returns:
         Dict[BaseNode, np.ndarray]: Expanded scores for each individual channel.
     """
     if simd_scores is None or simd_groups_indices is None:
         Logger.critical(f"Failed to find scores and indices to create unrolled scores for pruning information."
-                        f" Scores: {simd_scores}, Group indices: {simd_groups_indices}.")
+                        f" Scores: {simd_scores}, Group indices: {simd_groups_indices}.")  # pragma: no cover
     _scores = {}
     for node, groups_indices in simd_groups_indices.items():
         node_scores = simd_scores[node]
         total_indices = sum(len(group) for group in groups_indices)
         new_node_scores = np.zeros(total_indices)
 
         for group_score, group_indices in zip(node_scores, groups_indices):
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/pruning/pruning_section.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/pruning/pruning_section.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/core_config.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/core_config.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/debug_config.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/debug_config.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/node_quantization_config.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/node_quantization_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,42 +37,40 @@
 
 
 class BaseNodeQuantizationConfig(object):
     """
     Base class for node quantization configuration
     """
 
-    def set_quant_config_attr(self, parameter_name: str, parameter_value: Any,
+    def set_quant_config_attr(self, config_parameter_name: str, config_parameter_value: Any,
                               *args: List[Any], **kwargs: Dict[str, Any]):
         """
         Changes a BaseNodeQuantizationConfig's parameter.
         Note that arg and kwargs are only to allow clean override in the child classes.
 
         Args:
-            parameter_name: parameter name to change.
-            parameter_value: parameter value to change.
+            config_parameter_name: parameter name to change.
+            config_parameter_value: parameter value to change.
             args: A list of additional arguments.
             kwargs: A dictionary with additional key arguments.
 
         """
 
-        if hasattr(self, parameter_name):
-            setattr(self, parameter_name, parameter_value)
+        if hasattr(self, config_parameter_name):
+            setattr(self, config_parameter_name, config_parameter_value)
         else:
-            Logger.warning(f"Parameter {parameter_name} could not be found in the node quantization config and "
+            Logger.warning(f"Parameter {config_parameter_name} could not be found in the node quantization config and "
                            f"was not updated!")
 
     def __repr__(self) -> str:
         """
         Returns: String to display a NodeQuantizationConfig object.
         """
-        repr_str = ''
-        for k, v in self.__dict__.items():
-            repr_str += f'{k}: {v}\n'
-        return repr_str
+        # Used for debugging, thus no cover.
+        return ''.join(f'{k}: {v}\n' for k, v in self.__dict__.items())  # pragma: no cover
 
 
 class NodeActivationQuantizationConfig(BaseNodeQuantizationConfig):
     """
     Attributes for configuring the quantization of the activations of a node.
     """
     def __init__(self,
@@ -102,14 +100,15 @@
         self.input_scaling = qc.input_scaling
         self.min_threshold = qc.min_threshold
         self.l_p_value = qc.l_p_value
         self.shift_negative_activation_correction = qc.shift_negative_activation_correction
         self.z_threshold = qc.z_threshold
         self.shift_negative_ratio = qc.shift_negative_ratio
         self.shift_negative_threshold_recalculation = qc.shift_negative_threshold_recalculation
+        self.concat_threshold_update = qc.concat_threshold_update
 
     def quantize_node_output(self,
                              tensors: Any) -> Any:
         """
 
         Args:
             tensors: framework tensor/s
@@ -215,15 +214,15 @@
                self.activation_channel_equalization == other.activation_channel_equalization and \
                self.input_scaling == other.input_scaling and \
                self.min_threshold == other.min_threshold and \
                self.l_p_value == other.l_p_value and \
                self.shift_negative_activation_correction == other.shift_negative_activation_correction and \
                self.z_threshold == other.z_threshold and \
                self.shift_negative_ratio == other.shift_negative_ratio and \
-               self.shift_negative_threshold_recalculation == other.shift_negative_threshold_recalculation
+               self.shift_negative_threshold_recalculation == other.shift_negative_threshold_recalculation 
 
     def __hash__(self):
         return hash((self.activation_quantization_fn,
                      self.activation_quantization_params_fn,
                      self.activation_error_method,
                      self.activation_quantization_method,
                      self.activation_n_bits,
@@ -260,16 +259,14 @@
         self.weights_quantization_method = weights_attr_cfg.weights_quantization_method
         self.weights_error_method = qc.weights_error_method
         self.weights_n_bits = weights_attr_cfg.weights_n_bits
         self.weights_per_channel_threshold = weights_attr_cfg.weights_per_channel_threshold
         self.enable_weights_quantization = weights_attr_cfg.enable_weights_quantization
         self.l_p_value = qc.l_p_value
 
-
-
     @property
     def weights_error_method(self) -> QuantizationErrorMethod:
         """
         weights_error_method getter.
         """
         return self._weights_error_method
 
@@ -407,17 +404,14 @@
 
         # Initialize a quantization configuration for each of the node's attributes
         self.attributes_config_mapping = {}
         self.pos_attributes_config_mapping = {}
         for attr in node_attrs_list:
             if isinstance(attr, int):
                 # this is a positional attribute, so it needs to be handled separately.
-                # we assume that a positional attribute is quantized with the default configuration provided in the TPC.
-                if op_cfg.default_weight_attr_config.enable_weights_quantization:
-                    Logger.critical(f"Quantizing constant weights is not supported.")
                 self.pos_attributes_config_mapping[attr] = WeightsAttrQuantizationConfig(qc=qc,
                                                                                          weights_attr_cfg=op_cfg.default_weight_attr_config,
                                                                                          weights_channels_axis=weights_channels_axis)
             else:
                 # In Tensorflow, the attribute name is composed of the framework attribute name and the layer name,
                 # therefore, we need to look for the attribute in the op_cfg that is contained in the node attribute's name.
                 attrs_included_in_name = {k: v for k, v in op_cfg.attr_weights_configs_mapping.items() if k in attr}
@@ -517,42 +511,43 @@
         """
         attrs_with_name = {k: v for k, v in self.attributes_config_mapping.items() if attr_name in k}
         if len(attrs_with_name) > 1:
             Logger.warning(f"Found multiple weight attributes containing the name {attr_name}: "
                            f"{list(attrs_with_name.keys())}.")
         return attrs_with_name
 
-    def set_quant_config_attr(self, parameter_name: str, parameter_value: Any, attr_name: str = None,
+    def set_quant_config_attr(self, config_parameter_name: str, config_parameter_value: Any, attr_name: str = None,
                               *args: List[Any], **kwargs: Dict[str, Any]):
         """
         This method overrides the parent class set_quant_config_attr to enable setting a specific weights
         attribute config parameter.
 
         Args:
             attr_name: attribute name to change.
-            parameter_name: parameter name to change.
-            parameter_value: parameter value to change.
+            config_parameter_name: parameter name to change.
+            config_parameter_value: parameter value to change.
             args: A list of additional arguments.
             kwargs: A dictionary with additional key arguments.
 
         """
 
         if attr_name is None:
-            super(NodeWeightsQuantizationConfig, self).set_quant_config_attr(parameter_name, parameter_value,
+            super(NodeWeightsQuantizationConfig, self).set_quant_config_attr(config_parameter_name,
+                                                                             config_parameter_value,
                                                                              *args, **kwargs)
         else:
             if self.has_attribute_config(attr_name):
                 attr_cfg = self.get_attr_config(attr_name)
-                if hasattr(attr_cfg, parameter_name):
-                    setattr(attr_cfg, parameter_name, parameter_value)
+                if hasattr(attr_cfg, config_parameter_name):
+                    setattr(attr_cfg, config_parameter_name, config_parameter_value)
                 else:
-                    Logger.warning(f"Parameter {parameter_name} could not be found in the node quantization config of "
+                    Logger.warning(f"Parameter {config_parameter_name} could not be found in the node quantization config of "
                                    f"weights attribute {attr_name} and was not updated!")
             else:
-                Logger.error(f"Weights attribute {attr_name} could not be found to set parameter {parameter_name}.")
+                Logger.error(f"Weights attribute {attr_name} could not be found to set parameter {config_parameter_name}.")
 
     def __eq__(self, other: Any) -> bool:
         """
         Compares the object to another object to find if they are equal.
 
         Args:
             other: An object to compare to.
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_config.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,29 +22,32 @@
 
 class QuantizationErrorMethod(Enum):
     """
     Method for quantization threshold selection:
 
     NOCLIPPING - Use min/max values as thresholds.
 
-    MSE - Use min square error for minimizing quantization noise.
+    MSE - Use mean square error for minimizing quantization noise.
 
-    MAE - Use min absolute error for minimizing quantization noise.
+    MAE - Use mean absolute error for minimizing quantization noise.
 
     KL - Use KL-divergence to make signals distributions to be similar as possible.
 
     Lp - Use Lp-norm to minimizing quantization noise.
 
+    HMSE - Use Hessian-based mean squared error for minimizing quantization noise. This method is using Hessian scores to factorize more valuable parameters when computing the error induced by quantization.
+
     """
 
     NOCLIPPING = 0
     MSE = 1
     MAE = 2
     KL = 4
     LP = 5
+    HMSE = 6
 
 
 class QuantizationConfig:
 
     def __init__(self,
                  activation_error_method: QuantizationErrorMethod = QuantizationErrorMethod.MSE,
                  weights_error_method: QuantizationErrorMethod = QuantizationErrorMethod.MSE,
@@ -58,15 +61,16 @@
                  z_threshold: float = math.inf,
                  min_threshold: float = MIN_THRESHOLD,
                  l_p_value: int = 2,
                  linear_collapsing: bool = True,
                  residual_collapsing: bool = True,
                  shift_negative_ratio: float = 0.05,
                  shift_negative_threshold_recalculation: bool = False,
-                 shift_negative_params_search: bool = False):
+                 shift_negative_params_search: bool = False,
+                 concat_threshold_update: bool = False):
         """
         Class to wrap all different parameters the library quantize the input model according to.
 
         Args:
             activation_error_method (QuantizationErrorMethod): Which method to use from QuantizationErrorMethod for activation quantization threshold selection.
             weights_error_method (QuantizationErrorMethod): Which method to use from QuantizationErrorMethod for activation quantization threshold selection.
             relu_bound_to_power_of_2 (bool): Whether to use relu to power of 2 scaling correction or not.
@@ -113,16 +117,18 @@
         self.z_threshold = z_threshold
         self.l_p_value = l_p_value
         self.linear_collapsing = linear_collapsing
         self.residual_collapsing = residual_collapsing
         self.shift_negative_ratio = shift_negative_ratio
         self.shift_negative_threshold_recalculation = shift_negative_threshold_recalculation
         self.shift_negative_params_search = shift_negative_params_search
+        self.concat_threshold_update = concat_threshold_update
 
     def __repr__(self):
-        return str(self.__dict__)
+        # Used for debugging, thus no cover.
+        return str(self.__dict__)  # pragma: no cover
 
 
 # Default quantization configuration the library use.
 DEFAULTCONFIG = QuantizationConfig(QuantizationErrorMethod.MSE, QuantizationErrorMethod.MSE,
                                    relu_bound_to_power_of_2=False, weights_bias_correction=True,
                                    weights_second_moment_correction=False, input_scaling=False, softmax_shift=False)
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,10 +40,10 @@
         quantizer_fn = symmetric_quantizer
     elif weights_quantization_method == QuantizationMethod.UNIFORM:
         quantizer_fn = uniform_quantizer
     elif weights_quantization_method in [QuantizationMethod.LUT_POT_QUANTIZER, QuantizationMethod.LUT_SYM_QUANTIZER]:
         quantizer_fn = lut_kmeans_quantizer
     else:
         Logger.critical(
-            f"No quantizer function found for the specified quantization method: {weights_quantization_method}")
+            f"No quantizer function found for the specified quantization method: {weights_quantization_method}")  # pragma: no cover
 
     return quantizer_fn
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,21 +9,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from copy import deepcopy
-from typing import Tuple, Callable
+from typing import Tuple, Callable, List
 import numpy as np
 import model_compression_toolkit.core.common.quantization.quantization_config as qc
+from model_compression_toolkit.core.common.hessian import TraceHessianRequest, HessianMode, HessianInfoGranularity, \
+    HessianInfoService
 from model_compression_toolkit.core.common.similarity_analyzer import compute_mse, compute_mae, compute_lp_norm
 from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
-from model_compression_toolkit.constants import FLOAT_32
-from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import uniform_quantize_tensor
+from model_compression_toolkit.constants import FLOAT_32, NUM_QPARAM_HESSIAN_SAMPLES
+from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import uniform_quantize_tensor, \
+    reshape_tensor_for_per_channel_search
 
 
 def _mse_error_histogram(q_bins: np.ndarray,
                          q_count: np.ndarray,
                          bins: np.ndarray,
                          counts: np.ndarray) -> np.float32:
     """
@@ -85,16 +88,16 @@
         The Lp-norm distance between the two histograms.
     """
 
     return np.sum((np.power(np.abs((q_bins - bins)[:-1]), p) * counts)) / np.sum(counts)
 
 
 def _kl_error_function(x: np.ndarray,
-                       range_min: float,
-                       range_max: float,
+                       range_min: np.ndarray,
+                       range_max: np.ndarray,
                        n_bins: int = 2048,
                        n_bits: int = 8) -> np.float32:
     """
     Compute the error function between a tensor to its quantized version.
     The error is computed based on the KL-divergence the distributions have.
     Number of bins to use when computing the histogram of the float tensor is passed.
     The threshold and number of bits that were used to quantize the tensor are needed to compute the
@@ -144,45 +147,50 @@
                                range_max=range_max)
 
 
 def _kl_error_function_wrapper(x: np.ndarray,
                                range_min: np.ndarray,
                                range_max: np.ndarray,
                                n_bins: int = 2048,
-                               n_bits: int = 8) -> np.ndarray:
+                               n_bits: int = 8,
+                               per_channel: int = False) -> np.ndarray:
     """
     Computes the error function between a tensor and its quantized version for each channel.
     The error is based on the KL-divergence between the distributions.
     The function uses a specified number of bins to compute the histogram of the float tensor.
     It requires the threshold and number of bits used for quantization to determine the histogram's boundaries and the number of quantized bins.
 
     Args:
         x: Float tensor.
         range_min: Array specifying the minimum bound of the quantization range for each channel.
         range_max: Array specifying the maximum bound of the quantization range for each channel.
         n_bins: Number of bins for the float histogram.
         n_bits: Number of bits used for quantization.
+        per_channel: Whether quantization is done per-channel.
 
     Returns:
         An array containing the KL-divergence between the float and quantized histograms of the tensor for each channel.
 
     """
 
     error_list = []
-    for j in range(x.shape[0]):  # iterate all channels of the tensor.
-        error_list.append(_kl_error_function(x[j], range_min[j], range_max[j], n_bins=n_bins, n_bits=n_bits))
+    if per_channel:
+        for j in range(x.shape[0]):  # iterate all channels of the tensor.
+            error_list.append(_kl_error_function(x[j], range_min[j], range_max[j], n_bins=n_bins, n_bits=n_bits))
+    else:
+        error_list.append(_kl_error_function(x, range_min, range_max, n_bins=n_bins, n_bits=n_bits))
     return np.asarray(error_list)
 
 
 def _kl_error_histogram(q_bins: np.ndarray,
                         q_count: np.ndarray,
                         bins: np.ndarray,
                         counts: np.ndarray,
-                        range_min: float,
-                        range_max: float) -> np.float32:
+                        range_min: np.ndarray,
+                        range_max: np.ndarray) -> np.float32:
     """
     Compute the error function between a histogram to its quantized version.
     The error is computed based on the KL-divergence the distributions have.
     If a threshold is not passed, the maximal quantized bin value is used. A minimal
     threshold can be passed.
 
     Args:
@@ -237,16 +245,16 @@
     p_float = counts_acc / np.sum(counts_acc)
     p_float = _smooth_distribution(p_float)
 
     return np.sum(p_float * np.log(p_float / p_fxp))
 
 
 def _get_bins_indices_from_range(bins: np.ndarray,
-                                 range_min: float,
-                                 range_max: float) -> Tuple[int, int]:
+                                 range_min: np.ndarray,
+                                 range_max: np.ndarray) -> Tuple[int, int]:
     """
     For bins and a threshold, compute the first and last bins in between the threshold
     ranges.
 
     Args:
         bins: Bins to look for its first and last bins in the range.
         range_min: min bound on the quantization range.
@@ -258,15 +266,15 @@
     assert range_min < range_max
     first_bin_idx = max(np.where(bins >= range_min)[0].min() - 1, 0)
     last_bin_idx = np.where(bins < range_max)[0].max()
     assert first_bin_idx <= last_bin_idx
     return first_bin_idx, last_bin_idx
 
 
-def _is_range_valid(bins: np.ndarray, range_min: float, range_max: float) -> bool:
+def _is_range_valid(bins: np.ndarray, range_min: np.ndarray, range_max: np.ndarray) -> bool:
     """
     Check whether there are some bins from a numpy array of bins that are in between
     a threshold range or not.
     Args:
         bins: Bins to check.
         range_min: min bound on the quantization range.
         range_max: max bound on the quantization range.
@@ -362,44 +370,125 @@
 
     bins_subset = deepcopy(bins[first_bin_idx:last_bin_idx + 1])
     counts_subset = deepcopy(counts[first_bin_idx:last_bin_idx])
 
     return bins_subset, counts_subset
 
 
+def _compute_hessian_for_hmse(node,
+                              hessian_info_service: HessianInfoService,
+                              num_hessian_samples: int = NUM_QPARAM_HESSIAN_SAMPLES) -> List[np.ndarray]:
+    """
+    Compute and retrieve Hessian-based scores for using during HMSE error computation.
+
+    Args:
+        node: The node to compute Hessian-based scores for.
+        hessian_info_service: HessianInfoService object for retrieving Hessian-based scores.
+        num_hessian_samples: Number of samples to approximate Hessian-based scores on.
+
+    Returns: A list with computed Hessian-based scores tensors for the given node.
+
+    """
+    _request = TraceHessianRequest(mode=HessianMode.WEIGHTS,
+                                   granularity=HessianInfoGranularity.PER_ELEMENT,
+                                   target_node=node)
+    _scores_for_node = hessian_info_service.fetch_hessian(_request,
+                                                          required_size=num_hessian_samples)
+
+    return _scores_for_node
+
+
+def _hmse_error_function_wrapper(float_tensor: np.ndarray,
+                                 fxp_tensor: np.ndarray,
+                                 axis: int,
+                                 norm: bool,
+                                 hessian_scores: np.ndarray):
+    """
+    This function wraps the HMSE error method to enable using it during parameters selection.
+
+    Args:
+        float_tensor: Float tensor.
+        fxp_tensor: Quantized tensor.
+        axis: Axis along which the operation has been performed. If not None, then per-channel computation is expected.
+        norm: Indicates whether to normalize the result of the error function.
+        hessian_scores: A tensor with Hessian-based scores to use for Hessian-based MSE (HMSE) error computation.
+
+    Returns: The HMSE error between the float and fixed-point tensors.
+
+    """
+    if axis is not None:
+        hessian_scores = reshape_tensor_for_per_channel_search(hessian_scores, 0)
+
+    return compute_mse(float_tensor, fxp_tensor, axis, norm, weights=hessian_scores)
+
+
 def get_threshold_selection_tensor_error_function(quantization_method: QuantizationMethod,
                                                   quant_error_method: qc.QuantizationErrorMethod,
                                                   p: int,
                                                   axis: int = None,
                                                   norm: bool = False,
                                                   n_bits: int = 8,
-                                                  signed: bool = True) -> Callable:
+                                                  signed: bool = True,
+                                                  node=None,
+                                                  hessian_info_service: HessianInfoService = None,
+                                                  num_hessian_samples: int = NUM_QPARAM_HESSIAN_SAMPLES) -> Callable:
     """
     Returns the error function compatible to the provided threshold method,
     to be used in the threshold optimization search for tensor quantization.
     Args:
         quantization_method: Method used for selecting the quantization threshold.
         quant_error_method: Type of error function requested.
         p: P-norm to use for calculating the Lp-norm distance.
         axis: Axis along which the operation has been performed.
         norm: Indicates whether to normalize the result of the error function.
         n_bits: Number of bits used to quantize the tensor.
         signed: Indicates whether the input is signed.
+        node: The node for which the quantization error is computed (used only with HMSE error method).
+        hessian_info_service: HessianInfoService object for retrieving Hessian-based scores (used only with HMSE error method).
+        num_hessian_samples: Number of samples to approximate Hessian-based scores on (used only with HMSE error method).
 
     Returns: a Callable method that calculates the error between a tensor and a quantized tensor.
     """
+    if quant_error_method == qc.QuantizationErrorMethod.KL:
+        if axis is None:
+            # per-tensor
+            if quantization_method == QuantizationMethod.UNIFORM:
+                return lambda x, y, threshold: _kl_error_function_wrapper(x, range_min=threshold[0],
+                                                                          range_max=threshold[1],
+                                                                          n_bits=n_bits,
+                                                                          per_channel=False)
+            else:
+                return lambda x, y, threshold: _kl_error_function_wrapper(x, range_min=0 if not signed else -threshold,
+                                                                          range_max=threshold,
+                                                                          n_bits=n_bits,
+                                                                          per_channel=False)
+        else:
+            # per-channel
+            if quantization_method == QuantizationMethod.UNIFORM:
+                return lambda x, y, threshold: _kl_error_function_wrapper(x, range_min=threshold[:, 0],
+                                                                          range_max=threshold[:, 1],
+                                                                          n_bits=n_bits,
+                                                                          per_channel=True)
+            else:
+                return lambda x, y, threshold: _kl_error_function_wrapper(x, range_min=0 if not signed else -threshold,
+                                                                          range_max=threshold,
+                                                                          n_bits=n_bits,
+                                                                          per_channel=True)
+
+    if quant_error_method == qc.QuantizationErrorMethod.HMSE:
+        node_hessian_scores = _compute_hessian_for_hmse(node, hessian_info_service, num_hessian_samples)
+        node_hessian_scores = np.sqrt(np.mean(node_hessian_scores, axis=0))
+
+        return lambda x, y, threshold: _hmse_error_function_wrapper(x, y, norm=norm, axis=axis,
+                                                                    hessian_scores=node_hessian_scores)
 
     quant_method_error_function_mapping = {
         qc.QuantizationErrorMethod.MSE: lambda x, y, threshold: compute_mse(x, y, norm=norm, axis=axis),
         qc.QuantizationErrorMethod.MAE: lambda x, y, threshold: compute_mae(x, y, norm=norm, axis=axis),
         qc.QuantizationErrorMethod.LP: lambda x, y, threshold: compute_lp_norm(x, y, p=p, norm=norm, axis=axis),
-        qc.QuantizationErrorMethod.KL:
-            lambda x, y, threshold: _kl_error_function_wrapper(x, range_min=threshold[:,0], range_max=threshold[:,1],
-                                                       n_bits=n_bits) if quantization_method == QuantizationMethod.UNIFORM
-            else _kl_error_function_wrapper(x, range_min=0 if not signed else -threshold, range_max=threshold, n_bits=n_bits)
     }
 
     return quant_method_error_function_mapping[quant_error_method]
 
 
 def get_threshold_selection_histogram_error_function(quantization_method: QuantizationMethod,
                                                      quant_error_method: qc.QuantizationErrorMethod,
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
+from typing import Dict
 import numpy as np
 from sklearn.cluster import KMeans
 
 import model_compression_toolkit.core.common.quantization.quantization_config as qc
 from model_compression_toolkit.constants import LUT_VALUES, MIN_THRESHOLD, SCALE_PER_CHANNEL, \
-    LUT_VALUES_BITWIDTH, THRESHOLD
+    LUT_VALUES_BITWIDTH, THRESHOLD, NUM_QPARAM_HESSIAN_SAMPLES
+from model_compression_toolkit.core.common.hessian import HessianInfoService
 from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import \
     max_power_of_two, int_quantization_with_threshold
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.symmetric_selection import \
     symmetric_selection_tensor
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.power_of_two_selection import \
     power_of_two_selection_tensor
 
@@ -33,15 +35,18 @@
                       p: int,
                       n_bits: int,
                       per_channel: bool = False,
                       channel_axis: int = 1,
                       n_iter: int = 10,
                       min_threshold: float = MIN_THRESHOLD,
                       quant_error_method: qc.QuantizationErrorMethod = None,
-                      is_symmetric=False) -> dict:
+                      is_symmetric: bool = False,
+                      node=None,
+                      hessian_info_service: HessianInfoService = None,
+                      num_hessian_samples: int = NUM_QPARAM_HESSIAN_SAMPLES) -> Dict:
     """
     The quantizer first finds the closest max value per channel of tensor_data.
     Now, we divide tensor_data with the threshold vector per channel. In addition, we scale the result to the range
     [-2^(LUT_VALUES_BITWIDTH-1), 2^(LUT_VALUES_BITWIDTH-1)-1].
     Next, we take the scaled tensor_data and perform k-means clustering with 2^nbit clusters.
     We return the rounded cluster centers, and threshold per channel. We use these to quantize the data.
     Args:
@@ -49,15 +54,18 @@
         p: p-norm to use for the Lp-norm distance.
         n_bits: Number of bits to quantize the tensor.
         per_channel: Whether the quantization should be per-channel or not.
         channel_axis: Output channel index.
         n_iter: Number of iterations to search_methods for the optimal threshold.
         min_threshold: Minimal threshold to chose when the computed one is smaller.
         quant_error_method: an error function to optimize the parameters' selection accordingly (not used for this method).
-        is_symmetric (bool): Whether to apply symmetric weight quantization (default is False, meaning power of 2 quantization)
+        is_symmetric (bool): Whether to apply symmetric weight quantization (default is False, meaning power of 2 quantization).
+        node: The node for which the quantization error is computed (not used for this method).
+        hessian_info_service: HessianInfoService object for retrieving Hessian-based scores (not used for this method).
+        num_hessian_samples: Number of samples to approximate Hessian-based scores on (not used for this method).
 
     Returns:
         A dictionary containing the cluster assignments according to the k-means algorithm,
         the thresholds per channel and the multiplier num bits.
     """
     if n_bits >= LUT_VALUES_BITWIDTH:
         Logger.critical(f'Look-Up-Table (LUT) bit configuration exceeds maximum: {n_bits} bits provided, must be less than {LUT_VALUES_BITWIDTH} bits.')  # pragma: no cover
@@ -90,15 +98,15 @@
                          p: int,
                          n_bits: int,
                          min_value: float,
                          max_value: float,
                          constrained: bool = True,
                          n_iter: int = 20,
                          min_threshold: float = MIN_THRESHOLD,
-                         quant_error_method: qc.QuantizationErrorMethod = qc.QuantizationErrorMethod.MSE) -> dict:
+                         quant_error_method: qc.QuantizationErrorMethod = qc.QuantizationErrorMethod.MSE) -> Dict:
     """
     Finds quantization cluster points for non-uniform activation quantization.
     The quantizer first finds the closest power-of-two number to the max value of the given histogram,
     and scales the bins within 8-bit quantization range.
     Next, it performs a weighted k-means clustering with 2^nbit clusters (using the histogram counts as weights).
     Returns the rounded cluster centers, and 8-bit quantization threshold.
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import numpy as np
 
 import model_compression_toolkit.core.common.quantization.quantization_config as qc
-from model_compression_toolkit.constants import MIN_THRESHOLD, THRESHOLD
+from model_compression_toolkit.constants import MIN_THRESHOLD, THRESHOLD, NUM_QPARAM_HESSIAN_SAMPLES
+from model_compression_toolkit.core.common.hessian import HessianInfoService
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.qparams_search import \
     qparams_selection_tensor_search, qparams_selection_histogram_search
 from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import max_power_of_two, get_tensor_max
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.error_functions import \
     get_threshold_selection_tensor_error_function, get_threshold_selection_histogram_error_function
 from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 
@@ -27,42 +28,51 @@
 def power_of_two_selection_tensor(tensor_data: np.ndarray,
                                   p: int,
                                   n_bits: int,
                                   per_channel: bool = False,
                                   channel_axis: int = 1,
                                   n_iter: int = 10,
                                   min_threshold: float = MIN_THRESHOLD,
-                                  quant_error_method: qc.QuantizationErrorMethod = qc.QuantizationErrorMethod.MSE) -> dict:
+                                  quant_error_method: qc.QuantizationErrorMethod = qc.QuantizationErrorMethod.MSE,
+                                  node=None,
+                                  hessian_info_service: HessianInfoService = None,
+                                  num_hessian_samples: int = NUM_QPARAM_HESSIAN_SAMPLES,
+                                  ) -> dict:
     """
     Compute the power of two threshold based on the provided QuantizationErrorMethod to quantize the tensor.
     Different search is applied, depends on the value of the selected QuantizationErrorMethod.
 
     Args:
         tensor_data: Tensor content as Numpy array.
         p: p-norm to use for the Lp-norm distance.
         n_bits: Number of bits to quantize the tensor.
         per_channel: Whether the quantization should be per-channel or not.
         channel_axis: Output channel index.
         n_iter: Number of iterations to search for the optimal threshold (not used for this method).
         min_threshold: Minimal threshold to use if threshold is too small (not used for this method).
         quant_error_method: an error function to optimize the parameters' selection accordingly.
+        node: The node for which the quantization error is computed (used only with HMSE error method).
+        hessian_info_service: HessianInfoService object for retrieving Hessian-based scores (used only with HMSE error method).
+        num_hessian_samples: Number of samples to approximate Hessian-based scores on (used only with HMSE error method).
 
     Returns:
         Power of two threshold to quantize the tensor in a power of 2 manner.
     """
 
     if quant_error_method == qc.QuantizationErrorMethod.NOCLIPPING:
         tensor_max = get_tensor_max(tensor_data, per_channel, channel_axis, n_bits)
         threshold = max_power_of_two(tensor_max, min_threshold)
     else:
         signed = True  # weights are always signed
         axis = -1 if per_channel else None
         error_function = get_threshold_selection_tensor_error_function(QuantizationMethod.POWER_OF_TWO,
-                                                                       quant_error_method, p, axis=axis, norm=False, n_bits=n_bits,
-                                                                       signed=signed)
+                                                                       quant_error_method, p, axis=axis, norm=False,
+                                                                       n_bits=n_bits, signed=signed, node=node,
+                                                                       hessian_info_service=hessian_info_service,
+                                                                       num_hessian_samples=num_hessian_samples)
         threshold = qparams_selection_tensor_search(error_function,
                                                     tensor_data,
                                                     n_bits,
                                                     per_channel=per_channel,
                                                     channel_axis=channel_axis,
                                                     n_iter=n_iter,
                                                     min_threshold=min_threshold,
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,76 +1,97 @@
-# Copyright 2021 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from tqdm import tqdm
-from typing import List
-
-from model_compression_toolkit.core.common import Graph, BaseNode
-from model_compression_toolkit.core.common.quantization.quantization_params_generation.qparams_activations_computation \
-    import get_activations_qparams
-from model_compression_toolkit.core.common.quantization.quantization_params_generation.qparams_weights_computation import \
-    get_weights_qparams
-from model_compression_toolkit.logger import Logger
-
-
-def calculate_quantization_params(graph: Graph,
-                                  nodes: List[BaseNode] = [],
-                                  specific_nodes: bool = False):
-    """
-    For a graph, go over its nodes, compute quantization params (for both weights and activations according
-    to the given framework info), and create and attach a NodeQuantizationConfig to each node (containing the
-    computed params).
-    By default, the function goes over all nodes in the graph. However, the specific_nodes flag enables
-    to compute quantization params for specific nodes if the default behavior is unnecessary. For that,
-    a list of nodes should be passed as well.
-
-    Args:
-        groups of layers by how they should be quantized, etc.)
-        graph: Graph to compute its nodes' thresholds.
-        nodes: List of nodes to compute their thresholds instead of computing it for all nodes in the graph.
-        specific_nodes: Flag to compute thresholds for only specific nodes.
-
-    """
-
-    Logger.info(f"Running quantization parameters search. "
-                f"This process might take some time, "
-                f"depending on the model size and the selected quantization methods.\n")
-
-    # Create a list of nodes to compute their thresholds
-    nodes_list: List[BaseNode] = nodes if specific_nodes else graph.nodes()
-
-    for n in tqdm(nodes_list, "Calculating quantization params"):  # iterate only nodes that we should compute their thresholds
-        for candidate_qc in n.candidates_quantization_cfg:
-            for attr in n.get_node_weights_attributes():
-                if n.is_weights_quantization_enabled(attr):
-                    # If the node's weights attribute should be quantized, we compute its quantization parameters
-                    attr_cfg = candidate_qc.weights_quantization_cfg.get_attr_config(attr)
-                    channels_axis = attr_cfg.weights_channels_axis
-                    if channels_axis is not None:
-                        output_channels_axis = channels_axis[0]
-                    else:
-                        output_channels_axis = None
-                    weights_params = get_weights_qparams(n.get_weights_by_keys(attr),
-                                                         candidate_qc.weights_quantization_cfg,
-                                                         attr_cfg,
-                                                         output_channels_axis)
-                    attr_cfg.set_weights_quantization_param(weights_params)
-
-            if n.is_activation_quantization_enabled():
-                # If node's activations should be quantized as well, we compute its activation quantization parameters
-                activation_params = get_activations_qparams(
-                    activation_quant_cfg=candidate_qc.activation_quantization_cfg,
-                    nodes_prior_info=n.prior_info,
-                    out_stats_container=graph.get_out_stats_collector(n))
-                # Create a NodeQuantizationConfig containing all quantization params and attach it to the node
-                candidate_qc.activation_quantization_cfg.set_activation_quantization_param(activation_params)
+from abc import ABC
+from typing import Dict, List
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
+
+
+class TrainableQuantizerCandidateConfig:
+
+    def __init__(self,
+                 n_bits: int,
+                 quantization_params: Dict,
+                 ):
+        """
+        Class for representing candidates of quantization configurations for trainable quantizer.
+        It can be used for weights and activation quantization configuration.
+
+        Args:
+            n_bits (int): Number of bits to use for quantization.
+            quantization_params (Dict): Dictionary that contains quantization params.
+        """
+
+        self.n_bits = n_bits
+        self.quantization_params = quantization_params
+
+
+class TrainableQuantizerActivationConfig:
+
+    def __init__(self,
+                 activation_quantization_method: QuantizationMethod,
+                 activation_n_bits: int,
+                 activation_quantization_params: Dict,
+                 enable_activation_quantization: bool,
+                 min_threshold: float,
+                 activation_quantization_candidates: List[TrainableQuantizerCandidateConfig] = None,
+                 ):
+        """
+        Attributes for configuring activations trainable quantizer.
+
+        Args:
+            activation_quantization_method (QuantizationMethod): Which method to use from QuantizationMethod for activation quantization.
+            activation_n_bits (int): Number of bits to quantize the activations.
+            activation_quantization_params (Dict): Dictionary that contains activation quantization params.
+            enable_activation_quantization (bool): Whether to quantize the layer's activations or not.
+            min_threshold (float): Minimum threshold to use during thresholds selection.
+        """
+        self.activation_quantization_method = activation_quantization_method
+        self.activation_n_bits = activation_n_bits
+        self.activation_quantization_params = activation_quantization_params
+        self.enable_activation_quantization = enable_activation_quantization
+        self.min_threshold = min_threshold
+        self.activation_bits_candidates = activation_quantization_candidates
+
+
+class TrainableQuantizerWeightsConfig:
+    def __init__(self,
+                 weights_quantization_method: QuantizationMethod,
+                 weights_n_bits: int,
+                 weights_quantization_params: Dict,
+                 enable_weights_quantization: bool,
+                 weights_channels_axis: int,
+                 weights_per_channel_threshold: bool,
+                 min_threshold: float,
+                 weights_quantization_candidates: List[TrainableQuantizerCandidateConfig] = None,
+                 ):
+        """
+        Attributes for configuring weights trainable quantizer.
+
+        Args:
+            weights_quantization_method (QuantizationMethod): Which method to use from QuantizationMethod for weights quantization.
+            weights_n_bits (int): Number of bits to quantize the coefficients.
+            weights_quantization_params (Dict): Dictionary that contains weights quantization params.
+            enable_weights_quantization (bool): Whether to quantize the layer's weights or not.
+            weights_channels_axis (int): Axis to quantize a node's kernel when quantizing per-channel.
+            weights_per_channel_threshold (bool): Whether to quantize the weights per-channel or not (per-tensor).
+            min_threshold (float): Minimum threshold to use during thresholds selection.
+        """
+        self.weights_quantization_method = weights_quantization_method
+        self.weights_n_bits = weights_n_bits
+        self.weights_quantization_params = weights_quantization_params
+        self.enable_weights_quantization = enable_weights_quantization
+        self.weights_channels_axis = weights_channels_axis
+        self.weights_per_channel_threshold = weights_per_channel_threshold
+        self.min_threshold = min_threshold
+        self.weights_bits_candidates = weights_quantization_candidates
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,54 +8,64 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import Dict, Any, Tuple
+from typing import Dict, Any
 
 import numpy as np
 
-from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.constants import NUM_QPARAM_HESSIAN_SAMPLES
+from model_compression_toolkit.core.common.hessian import HessianInfoService
 from model_compression_toolkit.defaultdict import DefaultDict
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.quantization.node_quantization_config import NodeWeightsQuantizationConfig, \
     WeightsAttrQuantizationConfig
 
 # If the quantization config does not contain kernel channel mapping or the weights
 # quantization is not per-channel, we use a dummy channel mapping.
 dummy_channel_mapping = DefaultDict(default_value=(None, None))
 
 
-def get_weights_qparams(kernel: np.ndarray,
+def get_weights_qparams(weights_attr_values: np.ndarray,
                         weights_quant_config: NodeWeightsQuantizationConfig,
                         attr_quant_config: WeightsAttrQuantizationConfig,
-                        output_channels_axis: int) -> Dict[Any, Any]:
+                        output_channels_axis: int,
+                        node=None,
+                        hessian_info_service: HessianInfoService = None,
+                        num_hessian_samples: int = NUM_QPARAM_HESSIAN_SAMPLES) -> Dict[Any, Any]:
     """
     Compute thresholds to quantize a kernel according to a NodeWeightsQuantizationConfig
     instance.
 
     Args:
-        kernel: Kernel to compute the quantization thresholds to.
+        weights_attr_values: Weights attribute parameter to compute the quantization thresholds for.
         weights_quant_config: Weights quantization configuration to define how the thresholds are computed.
         attr_quant_config: A specific weights attribute quantization configuration to get its params.
         output_channels_axis: Index of the kernel output channels dimension.
+        node: The node for which the quantization error is computed (used only with HMSE error method).
+        hessian_info_service: HessianInfoService object for retrieving Hessian-based scores (used only with HMSE error method).
+        num_hessian_samples: Number of samples to approximate Hessian-based scores on (used only with HMSE error method).
 
     Returns:
         A dictionary with the quantization threshold of the kernel.
     """
     if attr_quant_config.weights_quantization_params_fn is not None:
-        weights_params = attr_quant_config.weights_quantization_params_fn(kernel,
+        weights_params = attr_quant_config.weights_quantization_params_fn(weights_attr_values,
                                                                           p=attr_quant_config.l_p_value,
                                                                           n_bits=attr_quant_config.weights_n_bits,
                                                                           per_channel=attr_quant_config.weights_per_channel_threshold and output_channels_axis is not None,
                                                                           channel_axis=output_channels_axis,
                                                                           min_threshold=weights_quant_config.min_threshold,
-                                                                          quant_error_method=attr_quant_config.weights_error_method)
+                                                                          quant_error_method=attr_quant_config.weights_error_method,
+                                                                          node=node,
+                                                                          hessian_info_service=hessian_info_service,
+                                                                          num_hessian_samples=num_hessian_samples)
     else:
         weights_params = {}
 
     return weights_params
 
 
 def _get_kernel_channels_mapping(fw_info:FrameworkInfo,
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import numpy as np
 
 import model_compression_toolkit.core.common.quantization.quantization_config as qc
-from model_compression_toolkit.constants import MIN_THRESHOLD, THRESHOLD
+from model_compression_toolkit.constants import MIN_THRESHOLD, THRESHOLD, NUM_QPARAM_HESSIAN_SAMPLES
+from model_compression_toolkit.core.common.hessian import HessianInfoService
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.error_functions import \
     get_threshold_selection_tensor_error_function, get_threshold_selection_histogram_error_function, _kl_error_histogram
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.qparams_search import \
     qparams_symmetric_selection_tensor_search, \
     qparams_symmetric_selection_histogram_search, kl_qparams_symmetric_selection_histogram_search
 from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import \
     get_tensor_max
@@ -29,41 +30,51 @@
 def symmetric_selection_tensor(tensor_data: np.ndarray,
                                p: int,
                                n_bits: int,
                                per_channel: bool = False,
                                channel_axis: int = 1,
                                n_iter: int = 10,
                                min_threshold: float = MIN_THRESHOLD,
-                               quant_error_method: qc.QuantizationErrorMethod = qc.QuantizationErrorMethod.MSE) -> dict:
+                               quant_error_method: qc.QuantizationErrorMethod = qc.QuantizationErrorMethod.MSE,
+                               node=None,
+                               hessian_info_service: HessianInfoService = None,
+                               num_hessian_samples: int = NUM_QPARAM_HESSIAN_SAMPLES) -> dict:
     """
     Compute the optimal threshold based on the provided QuantizationErrorMethod to quantize the tensor.
     Different search is applied, depends on the value of the selected QuantizationErrorMethod.
 
     Args:
         tensor_data: Tensor content as Numpy array.
         p: p-norm to use for the Lp-norm distance.
         n_bits: Number of bits to quantize the tensor.
         per_channel: Whether the quantization should be per-channel or not.
         channel_axis: Output channel index.
         n_iter: Number of iterations to search for the optimal threshold (not used for this method).
         min_threshold: Minimal threshold to use if threshold is too small (not used for this method).
         quant_error_method: an error function to optimize the parameters' selection accordingly.
+        node: The node for which the quantization error is computed (used only with HMSE error method).
+        hessian_info_service: HessianInfoService object for retrieving Hessian-based scores (used only with HMSE error method).
+        num_hessian_samples: Number of samples to approximate Hessian-based scores on (used only with HMSE error method).
 
     Returns:
         Optimal threshold to quantize the tensor in a symmetric manner.
     """
 
     tensor_max = get_tensor_max(tensor_data, per_channel, channel_axis, n_bits)
 
     if quant_error_method == qc.QuantizationErrorMethod.NOCLIPPING:
         threshold = get_init_threshold(min_threshold, tensor_max, per_channel)
     else:
         signed = True  # weights are always signed
         axis = -1 if per_channel else None
-        error_function = get_threshold_selection_tensor_error_function(QuantizationMethod.SYMMETRIC, quant_error_method, p, axis=axis, norm=False, n_bits=n_bits, signed=signed)
+        error_function = get_threshold_selection_tensor_error_function(QuantizationMethod.SYMMETRIC, quant_error_method,
+                                                                       p, axis=axis, norm=False, n_bits=n_bits,
+                                                                       signed=signed, node=node,
+                                                                       hessian_info_service=hessian_info_service,
+                                                                       num_hessian_samples=num_hessian_samples)
         threshold = qparams_symmetric_selection_tensor_search(error_function,
                                                               tensor_data,
                                                               tensor_max,
                                                               n_bits,
                                                               per_channel,
                                                               channel_axis,
                                                               min_threshold=min_threshold,
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import numpy as np
 
 import model_compression_toolkit.core.common.quantization.quantization_config as qc
-from model_compression_toolkit.constants import MIN_THRESHOLD, RANGE_MIN, RANGE_MAX
+from model_compression_toolkit.constants import MIN_THRESHOLD, RANGE_MIN, RANGE_MAX, NUM_QPARAM_HESSIAN_SAMPLES
+from model_compression_toolkit.core.common.hessian import HessianInfoService
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.qparams_search import \
     qparams_uniform_selection_tensor_search, qparams_uniform_selection_histogram_search
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.error_functions import \
     get_threshold_selection_tensor_error_function, get_threshold_selection_histogram_error_function
 from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import get_tensor_max, \
     get_tensor_min
 from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
@@ -27,41 +28,50 @@
 def uniform_selection_tensor(tensor_data: np.ndarray,
                              p: int,
                              n_bits: int,
                              per_channel: bool = False,
                              channel_axis: int = 1,
                              n_iter: int = 10,
                              min_threshold: float = MIN_THRESHOLD,
-                             quant_error_method: qc.QuantizationErrorMethod = qc.QuantizationErrorMethod.MSE) -> dict:
+                             quant_error_method: qc.QuantizationErrorMethod = qc.QuantizationErrorMethod.MSE,
+                             node=None,
+                             hessian_info_service: HessianInfoService = None,
+                             num_hessian_samples: int = NUM_QPARAM_HESSIAN_SAMPLES) -> dict:
     """
     Compute the optimal quantization range based on the provided QuantizationErrorMethod
     to uniformly quantize the tensor.
     Different search is applied, depends on the value of the selected QuantizationErrorMethod.
 
     Args:
         tensor_data: Tensor content as Numpy array.
         p: p-norm to use for the Lp-norm distance.
         n_bits: Number of bits to quantize the tensor.
         per_channel: Whether the quantization should be per-channel or not.
         channel_axis: Output channel index.
         n_iter: Number of iterations to search for the optimal threshold (not used for this method).
         min_threshold: Minimal threshold to use if threshold is too small (not used for this method).
         quant_error_method: an error function to optimize the range parameters' selection accordingly.
+        node: The node for which the quantization error is computed (used only with HMSE error method).
+        hessian_info_service: HessianInfoService object for retrieving Hessian-based scores (used only with HMSE error method).
+        num_hessian_samples: Number of samples to approximate Hessian-based scores on (used only with HMSE error method).
 
     Returns:
         Optimal quantization range to quantize the tensor uniformly.
     """
     tensor_min = get_tensor_min(tensor_data, per_channel, channel_axis)
     tensor_max = get_tensor_max(tensor_data, per_channel, channel_axis, n_bits, is_uniform_quantization=True)
 
     if quant_error_method == qc.QuantizationErrorMethod.NOCLIPPING:
         mm = tensor_min, tensor_max
     else:
         axis = -1 if per_channel else None
-        error_function = get_threshold_selection_tensor_error_function(QuantizationMethod.UNIFORM, quant_error_method, p, axis=axis, norm=False)
+        error_function = get_threshold_selection_tensor_error_function(QuantizationMethod.UNIFORM, quant_error_method,
+                                                                       p, axis=axis, norm=False, node=node,
+                                                                       hessian_info_service=hessian_info_service,
+                                                                       num_hessian_samples=num_hessian_samples)
         mm = qparams_uniform_selection_tensor_search(error_function,
                                                      tensor_data,
                                                      tensor_min,
                                                      tensor_max,
                                                      n_bits,
                                                      per_channel,
                                                      channel_axis)
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,36 +19,37 @@
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.graph.base_graph import Graph
 from model_compression_toolkit.core.common.quantization.quantize_node import get_quantized_weights_attr_by_qc
 from model_compression_toolkit.logger import Logger
 
 
-def quantize_graph_weights(graph: Graph) -> Graph:
+def quantize_graph_weights(graph_to_quantize: Graph) -> Graph:
     """
     Get a graph representing a model, and quantize its nodes' weights.
     Each node is quantized according to the passed framework info and quantization configuration.
     If weights bias correction is enabled in the quantization configuration, a bias correction term
     is calculated and subtracted from the original node's bias. The graph is quantized in-place.
 
     Args:
-        graph: Graph to quantize its nodes.
+        graph_to_quantize: Graph to quantize its nodes.
 
     """
+    _quantized_graph = copy.deepcopy(graph_to_quantize)
     # Iterate over nodes in the graph and quantize each node's weights and activations
     # (according to operators groups in framework info).
-    for n in graph.nodes():
+    for n in _quantized_graph.nodes():
         for attr in n.get_node_weights_attributes():
             if n.is_weights_quantization_enabled(attr):
                 quantized_attr, io_channels_axes = \
                     get_quantized_weights_attr_by_qc(attr,
                                                      n,
                                                      n.final_weights_quantization_cfg.get_attr_config(attr))
 
                 Logger.debug(
                     f'Weights attribute: {attr} of node name: {n.name} has the following quantization params: '
                     f'{str(n.final_weights_quantization_cfg.get_attr_config(attr).weights_quantization_params)}')
 
                 # Set the attribute to be the quantized attribute.
                 n.set_weights_by_keys(attr, quantized_attr)
 
-    return graph
+    return _quantized_graph
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantize_node.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantize_node.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantizers/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,39 +20,52 @@
 from model_compression_toolkit.core.common import BaseNode
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.graph.base_graph import Graph
 from model_compression_toolkit.core.common.quantization.candidate_node_quantization_config import \
     CandidateNodeQuantizationConfig
 from model_compression_toolkit.core.common.quantization.node_quantization_config import NodeActivationQuantizationConfig
-from model_compression_toolkit.core.common.quantization.quantization_config import QuantizationConfig
+from model_compression_toolkit.core.common.quantization.quantization_config import QuantizationConfig, \
+    QuantizationErrorMethod
 from model_compression_toolkit.core.common.quantization.quantization_params_fn_selection import \
     get_activation_quantization_params_fn, get_weights_quantization_params_fn
 from model_compression_toolkit.core.common.quantization.quantization_fn_selection import \
     get_weights_quantization_fn
 from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework import TargetPlatformCapabilities
 from model_compression_toolkit.target_platform_capabilities.target_platform.op_quantization_config import OpQuantizationConfig, \
     QuantizationConfigOptions
 
 
 def set_quantization_configuration_to_graph(graph: Graph,
                                             quant_config: QuantizationConfig,
-                                            mixed_precision_enable: bool = False) -> Graph:
+                                            mixed_precision_enable: bool = False,
+                                            running_gptq: bool = False) -> Graph:
     """
     Add quantization configuration for each graph node.
 
     Args:
         graph: Graph for which to add quantization info to each node.
         quant_config: Quantization configuration containing parameters for how the graph should be quantized.
-        mixed_precision_enable: is mixed precision enabled
+        mixed_precision_enable: is mixed precision enabled.
+        running_gptq: Whether or not a GPTQ optimization is planned to run after the PTQ process.
 
     Returns:
         The graph with quantization configurations attached to each node in it.
     """
 
+    if quant_config.weights_error_method == QuantizationErrorMethod.HMSE:
+        if not running_gptq:
+            Logger.warning(f"The HMSE error method for parameters selection is only supported when running GPTQ "
+                           f"optimization due to long execution time that is not suitable for basic PTQ. "
+                           f"Using the default MSE error method instead.")
+            quant_config.weights_error_method = QuantizationErrorMethod.MSE
+        else:
+            Logger.warning("Using the HMSE error method for weights quantization parameters search. "
+                           "Note: This method may significantly increase runtime during the parameter search process.")
+
     for n in graph.nodes:
         set_quantization_configs_to_node(node=n,
                                          quant_config=quant_config,
                                          fw_info=graph.fw_info,
                                          tpc=graph.tpc,
                                          mixed_precision_enable=mixed_precision_enable)
     return graph
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/similarity_analyzer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/similarity_analyzer.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 # ==============================================================================
 
 from typing import Any
 
 import numpy as np
 
 from model_compression_toolkit.constants import EPS
+from model_compression_toolkit.logger import Logger
+
 
 #########################
 #  Helpful functions
 #########################
 
 
 def validate_before_compute_similarity(float_tensor: Any, fxp_tensor: Any):
@@ -83,35 +85,45 @@
 
 
 def compute_mse(float_tensor: np.ndarray,
                 fxp_tensor: np.ndarray,
                 norm: bool = False,
                 norm_eps: float = 1e-8,
                 batch: bool = False,
-                axis: int = None) -> float:
+                axis: int = None,
+                weights: np.ndarray = None) -> float:
     """
     Compute the mean square error between two numpy arrays.
 
     Args:
         float_tensor: First tensor to compare.
         fxp_tensor: Second tensor to compare.
         norm: whether to normalize the error function result.
         norm_eps: epsilon value for error normalization stability.
         batch: Whether to run batch similarity analysis or not.
         axis: Axis along which the operator has been computed.
+        weights: Weights tensor to use for computing Weighted-MSE error computation.
 
     Returns:
         The MSE distance between the two tensors.
     """
     validate_before_compute_similarity(float_tensor, fxp_tensor)
 
     float_flat = flatten_tensor(float_tensor, batch, axis)
     fxp_flat = flatten_tensor(fxp_tensor, batch, axis)
 
-    error = ((float_flat - fxp_flat) ** 2).mean(axis=-1)
+    if weights is not None:
+        w_flat = flatten_tensor(weights, batch, axis)
+        if w_flat.shape != float_flat.shape:
+            Logger.critical(f"Shape mismatch: The shape of the weights tensor {weights.shape} does not match the shape "
+                            f"of the input tensors {float_flat.shape} for Weighted-MSE computation.")  # pragma: no cover
+        error = ((w_flat * (float_flat - fxp_flat)) ** 2).mean(axis=-1)
+    else:
+        error = ((float_flat - fxp_flat) ** 2).mean(axis=-1)
+
     if norm:
         error /= ((float_flat ** 2).mean(axis=-1) + norm_eps)
 
     return error
 
 
 def compute_mae(float_tensor: np.ndarray,
@@ -142,15 +154,18 @@
 
     error = np.abs(float_flat - fxp_flat).mean(axis=-1)
     if norm:
         error /= (np.abs(float_flat).mean(axis=-1) + norm_eps)
     return error
 
 
-def compute_cs(float_tensor: np.ndarray, fxp_tensor: np.ndarray, eps: float = 1e-8, batch: bool = False,
+def compute_cs(float_tensor: np.ndarray,
+               fxp_tensor: np.ndarray,
+               eps: float = 1e-8,
+               batch: bool = False,
                axis: int = None) -> float:
     """
     Compute the similarity between two tensor using cosine similarity.
     The returned values is between 0 to 1: the smaller returned value,
     the greater similarity there is between the two tensors.
 
     Args:
@@ -216,15 +231,15 @@
     return error
 
 
 def compute_kl_divergence(float_tensor: np.ndarray, fxp_tensor: np.ndarray, batch: bool = False,
                           axis: int = None) -> float:
     """
     Compute the similarity between two tensor using KL-divergence.
-    The returned values is between 0 to 1: the smaller returned value,
+    The returned values is between 0 and 1: the smaller returned value,
     the greater similarity there is between the two tensors.
 
     Args:
         float_tensor: First tensor to compare.
         fxp_tensor: Second tensor to compare.
         batch: Whether to run batch similarity analysis or not.
         axis: Axis along which the operator has been computed.
@@ -238,10 +253,10 @@
     float_flat = flatten_tensor(float_tensor, batch, axis)
     fxp_flat = flatten_tensor(fxp_tensor, batch, axis)
 
     non_zero_fxp_tensor = fxp_flat.copy()
     non_zero_fxp_tensor[non_zero_fxp_tensor == 0] = EPS
 
     prob_distance = np.where(float_flat != 0, float_flat * np.log(float_flat / non_zero_fxp_tensor), 0)
-    # The sum is part of the KL-Divergance function.
+    # The sum is part of the KL-Divergence function.
     # The mean is to aggregate the distance between each output probability vectors.
     return np.mean(np.sum(prob_distance, axis=-1), axis=-1)
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/statistics_correction/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,19 +45,24 @@
 
     for n in graph.nodes:
         # Bias correction is computed based on the quantized kernel, so we need to get the specific kernel attribute
         # name out of all the weights attributes of the node.
         if fw_info.is_kernel_op(n.type):
             kernel_attr = fw_info.get_kernel_op_attributes(n.type)[0]
             if n.is_weights_quantization_enabled(kernel_attr):
-                _compute_bias_correction_per_candidate_qc(n,
-                                                          kernel_attr,
-                                                          fw_info,
-                                                          graph.get_in_stats_collector(n),
-                                                          fw_impl=fw_impl)
+                # Bias correction is not applied to layers with constant inputs.
+                if n.has_positional_weights:
+                    for candidate_qc in n.candidates_quantization_cfg:
+                        candidate_qc.weights_quantization_cfg.weights_bias_correction = False
+                else:
+                    _compute_bias_correction_per_candidate_qc(n,
+                                                              kernel_attr,
+                                                              fw_info,
+                                                              graph.get_in_stats_collector(n),
+                                                              fw_impl=fw_impl)
     return graph
 
 
 def _compute_bias_correction_per_candidate_qc(node: BaseNode,
                                               kernel_attr: str,
                                               fw_info: FrameworkInfo,
                                               node_in_stats_collector: BaseStatsCollector,
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/apply_substitutions.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/apply_substitutions.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/linear_collapsing.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/residual_collapsing.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/residual_collapsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,16 @@
 
         # If the linear operator is part of a reused group (it is the "base" node, or a reused node),
         # we should skip the substitution.
         if first_node.is_reused() or second_node.is_reused():
             return graph
 
         # Check if convolution and residual satisfy the collapsing conditions, otherwise skip substitution
-        if len(graph.get_next_nodes(first_node)) > 1 or len(graph.get_prev_nodes(second_node)) != 2:
+        if (len(graph.get_next_nodes(first_node)) > 1 or len(graph.get_prev_nodes(first_node)) < 1 or
+                len(graph.get_prev_nodes(second_node)) != 2):
             return graph
 
         # Check if Add is residual connection, otherwise skip substitution
         conv_prev_nodes = graph.get_prev_nodes(first_node)
         add_prev_nodes = graph.get_prev_nodes(second_node)
         add_prev_nodes.remove(first_node)
         if conv_prev_nodes[0] != add_prev_nodes[0]:
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/scale_equalization.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/softmax_shift.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/substitutions/weights_activation_split.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/user_info.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/user_info.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/visualization/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/visualization/final_config_visualizer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/visualization/final_config_visualizer.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/visualization/nn_visualizer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/visualization/nn_visualizer.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+
 from typing import Tuple, List, Callable
 
 import numpy as np
 from matplotlib import pyplot as plt
 from matplotlib.figure import Figure
 
-from model_compression_toolkit.core.common.quantization.quantize_graph_weights import quantize_graph_weights
 from model_compression_toolkit.core.common import Graph
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
 from model_compression_toolkit.core.common.model_builder_mode import ModelBuilderMode
 from model_compression_toolkit.core.common.similarity_analyzer import compute_cs
+from model_compression_toolkit.logger import Logger
 
 
 def _get_compare_points(input_graph: Graph) -> Tuple[List[BaseNode], List[str]]:
     """
     Create a list of nodes in a graph where we collect their output statistics, and a corresponding list
     of their names for tensors comparison purposes.
     Args:
@@ -53,81 +54,107 @@
     NNVisualizer can compare the two models outputs after each layer.
     The results can be displayed using plot_cs_graph by passing it an input image to use
     for inference of the models.
     """
 
     def __init__(self,
                  graph_float: Graph,
+                 graph_quantized: Graph,
                  fw_impl: FrameworkImplementation,
                  fw_info: FrameworkInfo):
         """
         Initialize a NNVisualizer object.
         Args:
             graph_float: Float version of the graph.
+            graph_quantized: Quantized version of the graph.
+            fw_impl: Framework implementation with framework-specific methods implementation.
+            fw_info: Framework info with framework-specific information.
 
         """
 
         self.graph_float = graph_float
-        self.graph_quantized = quantize_graph_weights(graph_float)
+        self.graph_quantized = graph_quantized
         self.fw_impl = fw_impl
         self.fw_info = fw_info
 
         # Get compare points of two graphs.
         self.compare_points, self.compare_points_name = _get_compare_points(self.graph_quantized)
         self.compare_points_float, self.compare_points_name_float = _get_compare_points(self.graph_float)
 
+        if len(self.compare_points) != len(self.compare_points_float):
+            Logger.critical(f"Number of compare points in float and quantized models must be equal but "
+                            f"num of quantized compare points: {len(self.compare_points)} and "
+                            f"num of float compare points: {len(self.compare_points_float)}")
+        if len(self.compare_points_name) != len(self.compare_points_name_float):
+            Logger.critical(f"Number of compare points in float and quantized models must be equal "
+                            f"but num of quantized compare points: {len(self.compare_points_name)}"
+                            f" and num of float compare points: "
+                            f"{len(self.compare_points_name_float)}")
+
         self.quantized_model, _ = self.fw_impl.model_builder(self.graph_quantized,
                                                              mode=ModelBuilderMode.QUANTIZED,
                                                              append2output=self.compare_points,
                                                              fw_info=self.fw_info)
 
         self.float_model, _ = self.fw_impl.model_builder(self.graph_float,
                                                          mode=ModelBuilderMode.FLOAT,
                                                          append2output=self.compare_points_float,
                                                          fw_info=self.fw_info)
 
+    def has_compare_points(self) -> bool:
+        """
+
+        Returns: Whether or not compare points were found.
+
+        """
+        return len(self.compare_points_float) > 0 and len(self.compare_points) > 0 and len(
+            self.compare_points_name_float) > 0 and len(self.compare_points_name) > 0
+
+
     def plot_distance_graph(self,
                             input_image: np.ndarray,
+                            sample_index: int,
                             distance_fn: Callable = compute_cs,
                             convert_to_range: Callable = lambda a: a) -> Figure:
         """
         Compare and plot the outputs of the quantized and the float versions
         of a neural network that KerasNNVisualizer has.
 
         Args:
             input_image: Image to use as input to the networks.
+            sample_index: The index of the sample from input_image to use for comparison.
             distance_fn: Distance function to calculate the distance between two tensors.
             convert_to_range: Optional function to move the distance values into a specific range, e.g., when using
                 cosine similarity for distance, use 'lambda a: 1 - 2 * a' to convert the distance values to the range
                 of [-1, 1].
 
         Returns:
             Figure of the distance per layer.
         """
 
         # To compare cosine similarity, we use a single image as input (per input),
         # to make the difference more noticeable when exists
         new_inputs = []
         for single_input in input_image:
-            img = single_input[0]
+            img = single_input[sample_index]
             new_inputs.append(np.expand_dims(img, axis=0))
 
         # Get outputs
         tensors_float = self.fw_impl.run_model_inference(self.float_model, new_inputs)
         tensors_fxp = self.fw_impl.run_model_inference(self.quantized_model, new_inputs)
 
         # Compute distance between couples of outputs.
         distance_array = np.asarray(
             [distance_fn(self.fw_impl.to_numpy(t_float), self.fw_impl.to_numpy(t_fxp)) for t_float, t_fxp in zip(tensors_float, tensors_fxp)])
 
         distance_array = convert_to_range(distance_array)
 
         # Display the result: distance at every layer's output.
         fig = plt.figure()
-        plt.plot(distance_array)
+        plt.plot(list(range(len(distance_array))), distance_array)
         eps = 0.5
         y_limits = (min(distance_array) - eps, max(distance_array) + eps)
         plt.ylim(y_limits)
         plt.grid()
         plt.xlabel('Layer')
         plt.ylabel('Distance')
         return fig
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/common/visualization/tensorboard_writer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/common/visualization/tensorboard_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     # Create protobuf for the node's output shapes
     if output_shapes is not None:
         tshape_protos = []
         for output_shape in output_shapes:  # create protobuf for each output shape
             proto_dims_list = []
             for dim in output_shape:
-                proto_dims_list.append(TensorShapeProto.Dim(size=dim))
+                proto_dims_list.append(TensorShapeProto.Dim(size=dim))  # dim is expected to be an integer
             tshape_proto = TensorShapeProto(dim=proto_dims_list)
             tshape_protos.append(tshape_proto)
         node_properties['_output_shapes'] = AttrValue(list=AttrValue.ListValue(shape=tshape_protos))
     return node_properties
 
 
 class TensorboardWriter(object):
@@ -259,15 +259,21 @@
 
             Returns:
                 A list of tuples where each tuple is an output shape of the node.
             """
 
             # For nodes with an "empty" output shape.
             output_shape = (None,) if n.output_shape == () else n.output_shape
-
+            if 'CombinedNonMaxSuppression' in str(output_shape):
+                # output_shapes is expected to be a list of tuples where each tuple is an output shape.
+                # For NMS layers, we need to align the node's output shapes before creating the node's properties.
+                output_shape = [output_shape.nmsed_boxes,
+                                output_shape.nmsed_scores,
+                                output_shape.nmsed_classes,
+                                output_shape.valid_detections]
             dims = []
             if isinstance(output_shape, list):
                 for o in output_shape:
                     shape_wo_none = (-1,) + o[1:] if o[0] is None else o
                     dims.append(shape_wo_none)
             else:
                 dims = [(-1,) + output_shape[1:] if output_shape[0] is None else output_shape]
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/graph_prep_runner.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/graph_prep_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,16 @@
 def graph_preparation_runner(in_model: Any,
                              representative_data_gen: Callable,
                              quantization_config: QuantizationConfig,
                              fw_info: FrameworkInfo,
                              fw_impl: FrameworkImplementation,
                              tpc: TargetPlatformCapabilities,
                              tb_w: TensorboardWriter = None,
-                             mixed_precision_enable: bool = False) -> Graph:
+                             mixed_precision_enable: bool = False,
+                             running_gptq: bool = False) -> Graph:
     """
     Runs all required preparations in order to build a quantization graph from the given model,
     quantization configuration and target platform specifications.
     This runner include the following steps:
         - Reading and building a graph from the given model.
         - Setting quantization config to each relevant node in the graph.
         - Apply all necessary substitutions to finalize the graph for quantization.
@@ -55,14 +56,15 @@
         fw_info: Information needed for quantization about the specific framework (e.g., kernel channels indices,
             groups of layers by how they should be quantized, etc.).
         fw_impl: FrameworkImplementation object with a specific framework methods implementation.
         tpc: TargetPlatformCapabilities object that models the inference target platform and
             the attached framework operator's information.
         tb_w: TensorboardWriter object for logging.
         mixed_precision_enable: is mixed precision enabled.
+        running_gptq: Whether or not a GPTQ optimization is planned to run after the PTQ process.
 
     Returns:
         An internal graph representation of the input model.
     """
 
     graph = read_model_to_graph(in_model,
                                 representative_data_gen,
@@ -75,40 +77,43 @@
 
     transformed_graph = get_finalized_graph(graph,
                                             tpc,
                                             quantization_config,
                                             fw_info,
                                             tb_w,
                                             fw_impl,
-                                            mixed_precision_enable=mixed_precision_enable)
+                                            mixed_precision_enable=mixed_precision_enable,
+                                            running_gptq=running_gptq)
 
     return transformed_graph
 
 
 def get_finalized_graph(initial_graph: Graph,
                         tpc: TargetPlatformCapabilities,
                         quant_config: QuantizationConfig = DEFAULTCONFIG,
                         fw_info: FrameworkInfo = None,
                         tb_w: TensorboardWriter = None,
                         fw_impl: FrameworkImplementation = None,
-                        mixed_precision_enable: bool = False) -> Graph:
+                        mixed_precision_enable: bool = False,
+                        running_gptq: bool = False) -> Graph:
     """
     Applies all edit operation (edit, substitutions, etc.) on the model's graph, to prepare it for the quantization
     process. All future graph substitutions and operations that change the graph should be added to this method.
 
     Args:
         initial_graph (Graph): Graph to apply the changes to.
         tpc (TargetPlatformCapabilities): TargetPlatformCapabilities object that describes the desired inference target platform (includes fusing patterns MCT should handle).
         quant_config (QuantizationConfig): QuantizationConfig containing parameters of how the model should be
             quantized.
         fw_info (FrameworkInfo): Information needed for quantization about the specific framework (e.g.,
             kernel channels indices, groups of layers by how they should be quantized, etc.)
         tb_w (TensorboardWriter): TensorboardWriter object to use for logging events such as graphs, histograms, etc.
         fw_impl (FrameworkImplementation): FrameworkImplementation object with a specific framework methods implementation.
         mixed_precision_enable: is mixed precision enabled.
+        running_gptq: Whether or not a GPTQ optimization is planned to run after the PTQ process.
 
     Returns: Graph object that represents the model, after applying all required modifications to it.
     """
 
     ######################################
     # Graph substitution (prepare graph)
     ######################################
@@ -138,15 +143,16 @@
         tb_w.add_graph(transformed_graph, 'pre_statistics_collection_substitutions')
 
     ######################################
     # Add quantization configurations
     ######################################
     transformed_graph = set_quantization_configuration_to_graph(graph=transformed_graph,
                                                                 quant_config=quant_config,
-                                                                mixed_precision_enable=mixed_precision_enable)
+                                                                mixed_precision_enable=mixed_precision_enable,
+                                                                running_gptq=running_gptq)
 
     ######################################
     # Layer fusing
     ######################################
     transformed_graph = fusion(transformed_graph, tpc)
 
     ######################################
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/back2framework/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/back2framework/float_model_builder.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/back2framework/instance_builder.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/back2framework/instance_builder.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,28 +21,29 @@
 from model_compression_toolkit.core.common.user_info import UserInformation
 
 if version.parse(tf.__version__) >= version.parse("2.13"):
     from keras import Input
     from keras.src.layers.core import TFOpLambda
     from keras.src.engine.base_layer import TensorFlowOpLayer, Layer
 else:
-    from keras import Input
-    from keras.layers.core import TFOpLambda
-    from keras.engine.base_layer import TensorFlowOpLayer, Layer
+    from keras import Input   # pragma: no cover
+    from keras.layers.core import TFOpLambda   # pragma: no cover
+    from keras.engine.base_layer import TensorFlowOpLayer, Layer   # pragma: no cover
 
 from typing import Any, Dict, List, Tuple, Callable
 from tensorflow.python.util.object_identity import Reference as TFReference
 from model_compression_toolkit.core.common.graph.functional_node import FunctionalNode
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.keras.default_framework_info import DEFAULT_KERAS_INFO
 from model_compression_toolkit.core.common import BaseNode
 from model_compression_toolkit.core.common.graph.edge import EDGE_SINK_INDEX
 from model_compression_toolkit.core.keras.back2framework.instance_builder import OperationHandler
 from model_compression_toolkit.core.keras.reader.connectivity_handler import OutTensor
+from mct_quantizers import KerasQuantizationWrapper
 
 # In tf2.3 fake quant node is implemented as TensorFlowOpLayer, while in tf2.4 as TFOpLambda.
 FQ_NODE_OP_V2_3 = 'FakeQuantWithMinMaxVars'
 FQ_NODE_OP_V2_4 = 'quantization.fake_quant_with_min_max_vars'
 BATCH_INPUT_SHAPE = 'batch_input_shape'
 
 
@@ -266,15 +267,17 @@
         """
         if len(input_tensors) == 0:  # Placeholder handling
             out_tensors_of_n_float = input_nodes_to_input_tensors[n]
             out_tensors_of_n = self._run_operation_activation_quantization(n,
                                                                            out_tensors_of_n_float)
         else:
             input_tensors = [tensor for tensor_list in input_tensors for tensor in tensor_list]  # flat list of lists
-            input_tensors = n.insert_positional_weights_to_input_list(input_tensors)
+            if not isinstance(op_func, KerasQuantizationWrapper):
+                # The KerasQuantizationWrapper will insert the quantized positional weights internally.
+                input_tensors = n.insert_positional_weights_to_input_list(input_tensors)
             # Build a functional node using its args
             if isinstance(n, FunctionalNode):
                 if n.inputs_as_list:  # If the first argument should be a list of tensors:
                     out_tensors_of_n_float = op_func(input_tensors, *n.op_call_args, **n.op_call_kwargs)
                 else:  # If the input tensors should not be a list but iterated:
                     out_tensors_of_n_float = op_func(*input_tensors, *n.op_call_args, **n.op_call_kwargs)
             else:
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from typing import Tuple, Any, Dict, Union, List
 
 from packaging import version
 import tensorflow as tf
 if version.parse(tf.__version__) >= version.parse("2.13"):
     from keras.src.engine.base_layer import Layer
 else:
-    from keras.engine.base_layer import Layer
+    from keras.engine.base_layer import Layer  # pragma: no cover
 
 from keras.models import Model
 from mct_quantizers import KerasQuantizationWrapper, KerasActivationQuantizationHolder, QuantizationTarget
 from mct_quantizers.common.get_quantizers import get_inferable_quantizer_class
 from mct_quantizers.keras.quantizers import BaseKerasInferableQuantizer
 
 from model_compression_toolkit.core.common import BaseNode
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/constants.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/constants.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/custom_layer_validation.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/custom_layer_validation.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/default_framework_info.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/default_framework_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from model_compression_toolkit.core.keras.quantizer.lut_fake_quant import activation_lut_kmean_quantizer
 from packaging import version
 
 if version.parse(tf.__version__) >= version.parse("2.13"):
     from keras.src.layers import Conv2D, DepthwiseConv2D, Dense, Conv2DTranspose, Softmax, ELU
 else:
-    from keras.layers import Conv2D, DepthwiseConv2D, Dense, Conv2DTranspose, Softmax, ELU
+    from keras.layers import Conv2D, DepthwiseConv2D, Dense, Conv2DTranspose, Softmax, ELU  # pragma: no cover
 
 from model_compression_toolkit.defaultdict import DefaultDict
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 from model_compression_toolkit.constants import SOFTMAX_THRESHOLD
 from model_compression_toolkit.core.keras.constants import SOFTMAX, LINEAR, RELU, SWISH, SIGMOID, IDENTITY, TANH, SELU, \
     KERNEL, DEPTHWISE_KERNEL
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         Returns:
             Graph after applying the substitution.
         """
 
         if ACTIVATION not in op2d_node.framework_attr:
             Logger.warning(f'Op2d node {op2d_node.name} of type {op2d_node.type} is missing an "{ACTIVATION}"'
                            f' attribute -> Skipping substitution ActivationDecomposition')  # pragma: no cover
-            return graph
+            return graph  # pragma: no cover
 
         activation_node_name = op2d_node.name + '_post_activation'
 
         # Softmax is a special case where we need to know the default axis parameter used
         # and for this reason we create a Softmax layer and not Activation layer.
         if op2d_node.framework_attr.get(ACTIVATION) == SOFTMAX:
             activation_fw_attr = {AXIS: SOFTMAX_AXIS_DEFAULT}
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,17 +66,17 @@
         conv_node: Convolution node to update the weight/kernel.
         kernel: The Convolution node's weight
         weights_scale: Weight scale factor in which to multiply the conv node's weight.
 
     Returns:
         The modified convolution node's weight/kernel/
     """
-    if conv_node.type == DepthwiseConv2D:
+    if conv_node.is_match_type(DepthwiseConv2D):
         kernel = kernel * weights_scale.reshape((1, 1, kernel.shape[-2], kernel.shape[-1]))
-    elif conv_node.type == Conv2DTranspose:
+    elif conv_node.is_match_type(Conv2DTranspose):
         kernel = kernel * weights_scale.reshape((1, 1, -1, 1))
     else:
         kernel = kernel * weights_scale.reshape((1, 1, 1, -1))
 
     kernel_name = DEFAULT_KERAS_INFO.get_kernel_op_attributes(conv_node.type)[0]
 
     return kernel, kernel_name
@@ -94,18 +94,18 @@
         bias: The Convolution node's bias
         weights_scale: Weight scale factor in which to multiply the conv node's weight.
         bias_factor: factor for kernel to update the bias with: (beta - moving_mean * weights_scale)
 
     Returns:
         The modified convolution node's weight/kernel/
     """
-    if conv_node.type == DepthwiseConv2D:
+    if conv_node.is_match_type(DepthwiseConv2D):
         bias_update = kernel * bias_factor.reshape((1, 1, -1, 1))
         kernel = kernel * weights_scale.reshape((1, 1, -1, 1))
-    elif conv_node.type == Conv2DTranspose:
+    elif conv_node.is_match_type(Conv2DTranspose):
         bias_update = (kernel * bias_factor.reshape((1, 1, 1, -1))).sum(3)
         kernel = kernel * weights_scale.reshape((1, 1, 1, -1))
     else:
         bias_update = (kernel * bias_factor.reshape((1, 1, -1, 1))).sum(2)
         kernel = kernel * weights_scale.reshape((1, 1, -1, 1))
 
     kernel_name = DEFAULT_KERAS_INFO.get_kernel_op_attributes(conv_node.type)[0]
@@ -129,30 +129,30 @@
     Check whether the node is a group-convolution
     Args:
         node: The Convolution node
 
     Returns:
         True if the node is a group convolution, else False
     """
-    return (node.type == Conv2D) and node.framework_attr[GROUPS] > 1
+    return (node.is_match_type(Conv2D)) and node.framework_attr[GROUPS] > 1
 
 
 def get_foldable_node_type_and_validity_fn(node: BaseNode) -> [bool, bool]:
     """
     Check whether the node to forward fold is a valid dw-convolution node or a
     batch-normalization node
     Args:
         node: The node to fold
 
     Returns:
         is_bn: True if the node is a batch norm, else False
         is_dw_valid: True if the node is a dw-convolution valid for folding or a batch-norm node, else False
     """
-    is_bn = node.type is BatchNormalization
-    is_dw = node.type is DepthwiseConv2D
+    is_bn = node.is_match_type(BatchNormalization)
+    is_dw = node.is_match_type(DepthwiseConv2D)
     is_dw_valid = is_dw and np.all(np.array(node.get_weights_by_keys(DEPTHWISE_KERNEL).shape[:2]) == 1)
     return is_bn, is_dw_valid
 
 
 def keras_batchnorm_folding() -> BatchNormalizationFolding:
     """
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         first_node: First layer node to collapse to second layer node
         second_node: Second layer node
         kernel_str: The framework specific attribute name of the convolution layer's weight/kernel.
         bias_str: The framework specific attribute name of the convolution layer's bias.
     Returns:
         The modified layer node's weights: kernel, bias
     """
-    if first_node.type == Conv2D and second_node.type == Conv2D:
+    if first_node.is_match_type(Conv2D) and second_node.is_match_type(Conv2D):
         # Get nodes attributes
         kernel1 = first_node.get_weights_by_keys(kernel_str)
         kernel2 = second_node.get_weights_by_keys(kernel_str)
         bias1 = first_node.get_weights_by_keys(bias_str)
         bias2 = second_node.get_weights_by_keys(bias_str)
         strides1 = first_node.framework_attr[STRIDES]
         strides2 = second_node.framework_attr[STRIDES]
@@ -100,15 +100,15 @@
             if bias2 is not None:
                 bias_collapsed += bias2
         elif bias2 is not None:
             bias_collapsed = bias2
 
         return kernel_collapsed, bias_collapsed
     else:
-        Logger.critical(f"Layer collapsing unsupported for combination: {first_node.type} and {second_node.type}.")
+        Logger.critical(f"Layer collapsing unsupported for combination: {first_node.type} and {second_node.type}.")  # pragma: no cover
 
 
 def keras_linear_collapsing() -> Conv2DCollapsing:
     """
     Returns:
         A Conv2DCollapsing initialized for Keras models.
     """
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,28 +45,28 @@
     Inspired by https://arxiv.org/pdf/2103.09404.pdf - Algorithm2
     Args:
         first_node: First layer node to collapse into.
         kernel_str: The framework specific attribute name of the convolution layer's weight/kernel.
     Returns:
         The modified layer node's weights: kernel
     """
-    if first_node.type == Conv2D:
+    if first_node.is_match_type(Conv2D):
         # Get nodes attributes
         kernel = first_node.get_weights_by_keys(kernel_str)
         (kH, kW, Cin, Cout) = kernel.shape
 
         # Collapsing residual by adding "1" to kernel diagonal
         idxH = (kH - 1) // 2
         idxW = (kW - 1) // 2
         for i in range(Cout):
             kernel[idxH, idxW, i, i] += 1
 
         return kernel
     else:
-        Logger.critical(f"Residual collapsing is unsupported for {first_node.type} node types.")
+        Logger.critical(f"Residual collapsing is unsupported for {first_node.type} node types.")  # pragma: no cover
 
 
 def keras_residual_collapsing() -> ResidualCollapsing:
     """
     Returns:
         A ResidualCollapsing initialized for Keras models.
     """
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import numpy as np
 
 from packaging import version
 import tensorflow as tf
 from tensorflow.python.keras.layers.core import TFOpLambda
 if version.parse(tf.__version__) >= version.parse("2.13"):
     from keras.src.layers import Activation, Conv2D, Dense, DepthwiseConv2D, ZeroPadding2D, Reshape, \
-        GlobalAveragePooling2D, Dropout, ReLU, PReLU, ELU
+        GlobalAveragePooling2D, Dropout, ReLU, PReLU, ELU  # pragma: no cover
 else:
     from tensorflow.keras.layers import Activation, Conv2D, Dense, DepthwiseConv2D, ZeroPadding2D, Reshape, \
         GlobalAveragePooling2D, Dropout, ReLU, PReLU, ELU
 
 from model_compression_toolkit.core import CoreConfig, FrameworkInfo
 from model_compression_toolkit.core.common import BaseNode, Graph
 from model_compression_toolkit.core.common.graph.functional_node import FunctionalNode
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/hessian/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,10 +70,10 @@
         _unfold_tensors = self.unfold_tensors_list(tensors_to_concate)
         _r_tensors = [tf.reshape(tensor, shape=[tensor.shape[0], -1]) for tensor in _unfold_tensors]
 
         # Ensure all tensors have the same shape for concatenation
         concat_axis_dim = [o.shape[0] for o in _r_tensors]
         if not all(d == concat_axis_dim[0] for d in concat_axis_dim):
             Logger.critical(
-                "Unable to concatenate tensors for gradient calculation due to mismatched shapes along the first axis.")# pragma: no cover
+                "Unable to concatenate tensors for gradient calculation due to mismatched shapes along the first axis.") # pragma: no cover
 
         return tf.concat(_r_tensors, axis=1)
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/keras_implementation.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/keras_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from functools import partial
-from typing import List, Any, Tuple, Callable, Dict
+from typing import List, Any, Tuple, Callable, Dict, Union
 
 import numpy as np
 import tensorflow as tf
 from mct_quantizers import KerasQuantizationWrapper, KerasActivationQuantizationHolder
 from tensorflow.keras.models import Model
 
 from model_compression_toolkit.constants import HESSIAN_NUM_ITERATIONS
 from model_compression_toolkit.core.common.hessian import TraceHessianRequest, HessianMode, HessianInfoService
+from model_compression_toolkit.core.keras.graph_substitutions.substitutions.remove_identity import RemoveIdentity
 from model_compression_toolkit.core.keras.hessian.activation_trace_hessian_calculator_keras import \
     ActivationTraceHessianCalculatorKeras
 from model_compression_toolkit.core.keras.hessian.weights_trace_hessian_calculator_keras import WeightsTraceHessianCalculatorKeras
 from model_compression_toolkit.exporter.model_wrapper.fw_agnostic.get_inferable_quantizers import \
     get_inferable_quantizers
 from model_compression_toolkit.exporter.model_wrapper.keras.builder.node_to_quantizer import \
     get_weights_quantizer_for_node, get_activations_quantizer_for_node
@@ -46,21 +47,19 @@
 from model_compression_toolkit.core.keras.mixed_precision.configurable_weights_quantizer import \
     ConfigurableWeightsQuantizer
 from model_compression_toolkit.core.keras.statistics_correction.apply_second_moment_correction import \
     keras_apply_second_moment_correction
 from packaging import version
 
 if version.parse(tf.__version__) >= version.parse("2.13"):
-    from keras.src.layers import Dense, Activation, Conv2D, DepthwiseConv2D, Conv2DTranspose, \
-        Concatenate, Add
+    from keras.src.layers import Dense, Activation, Conv2D, DepthwiseConv2D, Conv2DTranspose, Concatenate, Add
     from keras.src.layers.core import TFOpLambda
 else:
-    from keras.layers import Dense, Activation, Conv2D, DepthwiseConv2D, Conv2DTranspose, \
-        Concatenate, Add
-    from keras.layers.core import TFOpLambda
+    from keras.layers import Dense, Activation, Conv2D, DepthwiseConv2D, Conv2DTranspose, Concatenate, Add   # pragma: no cover
+    from keras.layers.core import TFOpLambda   # pragma: no cover
 
 from model_compression_toolkit.core import QuantizationConfig, FrameworkInfo, CoreConfig, MixedPrecisionQuantizationConfig
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common import Graph, BaseNode
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.common.model_builder_mode import ModelBuilderMode
 from model_compression_toolkit.core.common.node_prior_info import NodePriorInfo
@@ -76,19 +75,18 @@
 from model_compression_toolkit.core.keras.graph_substitutions.substitutions.batchnorm_refusing import \
     keras_batchnorm_refusing
 from model_compression_toolkit.core.keras.graph_substitutions.substitutions.linear_collapsing import \
     keras_linear_collapsing, keras_op2d_add_const_collapsing
 from model_compression_toolkit.core.keras.graph_substitutions.substitutions.residual_collapsing import \
     keras_residual_collapsing
 from model_compression_toolkit.core.keras.graph_substitutions.substitutions.input_scaling import InputScaling, \
-    InputScalingWithPad
+    InputScalingWithPad 
+from model_compression_toolkit.core.keras.graph_substitutions.substitutions.concat_threshold_update import ConcatThresholdUpdate
 from model_compression_toolkit.core.keras.graph_substitutions.substitutions.relu_bound_to_power_of_2 import \
     ReLUBoundToPowerOfTwo
-from model_compression_toolkit.core.keras.graph_substitutions.substitutions.remove_relu_upper_bound import \
-    RemoveReLUUpperBound
 from model_compression_toolkit.core.keras.graph_substitutions.substitutions.multi_head_attention_decomposition import \
     MultiHeadAttentionDecomposition
 from model_compression_toolkit.core.keras.graph_substitutions.substitutions.scale_equalization import \
     ScaleEqualization, ScaleEqualizationWithPad, ScaleEqualizationMidActivation, ScaleEqualizationMidActivationWithPad
 from model_compression_toolkit.core.keras.graph_substitutions.substitutions.separableconv_decomposition import \
     SeparableConvDecomposition, DEPTH_MULTIPLIER
 from model_compression_toolkit.core.keras.graph_substitutions.substitutions.shift_negative_activation import \
@@ -243,15 +241,16 @@
         Returns: A list of the framework substitutions used to prepare the graph.
 
         """
         return [SeparableConvDecomposition(),
                 MatmulToDenseSubstitution(),
                 MultiHeadAttentionDecomposition(),
                 ActivationDecomposition(),
-                DwconvToConv()]
+                DwconvToConv(),
+                RemoveIdentity()]
 
     def get_substitutions_pre_statistics_collection(self, quant_config: QuantizationConfig) -> \
             List[common.BaseSubstitution]:
         """
         Return a list of the framework substitutions used before we collect statistics.
 
         Args:
@@ -298,16 +297,16 @@
 
     def get_op2d_add_const_collapsing_substitution(self) -> common.BaseSubstitution:
         """
         Returns: Op2d add-const collapsing substitution
         """
         return keras_op2d_add_const_collapsing()
 
-    def get_substitutions_post_statistics_collection(self, quant_config: QuantizationConfig) \
-            -> List[common.BaseSubstitution]:
+    def get_substitutions_post_statistics_collection(self, 
+                                                     quant_config: QuantizationConfig) -> List[common.BaseSubstitution]:
         """
         Return a list of the framework substitutions used after we collect statistics.
 
         Args:
             quant_config: QuantizationConfig to determine which substitutions to return.
 
         Returns:
@@ -315,24 +314,18 @@
         """
         substitutions_list = []
         if quant_config.softmax_shift:
             substitutions_list.append(keras_softmax_shift())
         if quant_config.input_scaling:
             substitutions_list.append(InputScaling())
             substitutions_list.append(InputScalingWithPad())
+        if quant_config.concat_threshold_update:
+            substitutions_list.append(ConcatThresholdUpdate())
         return substitutions_list
 
-    def get_substitutions_pre_build(self) -> List[common.BaseSubstitution]:
-        """
-
-        Returns: A list of the framework substitutions used before we build a quantized model.
-
-        """
-
-        return [RemoveReLUUpperBound()]
 
     def get_substitutions_virtual_weights_activation_coupling(self) -> List[common.BaseSubstitution]:
         """
         Returns: A list of Keras substitutions used to build a virtual graph with composed activation-weights pairs.
         """
 
         return [WeightsActivationSplit(),
@@ -413,38 +406,41 @@
         """
         Returns whether a given node in considered as a potential interest point for mp metric computation purposes.
         Args:
             node: Node to indicate whether it needs to be part of the interest points set.
         Returns: True if the node should be considered an interest point, False otherwise.
         """
 
-        if node.type == Activation:
+        if node.is_match_type(Activation):
             node_type_name = node.framework_attr[keras_constants.ACTIVATION]
             if node_type_name in [keras_constants.SOFTMAX, keras_constants.SIGMOID]:
                 return True
-        elif node.type in [tf.nn.softmax, tf.keras.layers.Softmax, tf.nn.sigmoid, Conv2D, DepthwiseConv2D, Conv2DTranspose, Dense, Concatenate,
-                           tf.concat, Add, tf.add]:
+        elif any([node.is_match_type(_type) for _type in [tf.nn.softmax, tf.keras.layers.Softmax, tf.nn.sigmoid, Conv2D,
+                                                          DepthwiseConv2D, Conv2DTranspose, Dense, Concatenate, tf.concat,
+                                                          Add, tf.add]]):
             return True
 
         return False
 
-    def get_node_distance_fn(self, layer_class: type,
+    def get_mp_node_distance_fn(self, layer_class: type,
                              framework_attrs: Dict[str, Any],
                              compute_distance_fn: Callable = None,
-                             axis: int = None) -> Callable:
+                             axis: int = None,
+                             norm_mse: bool = False) -> Callable:
         """
         A mapping between layers' types and a distance function for computing the distance between
-        two tensors (for loss computation purposes). Returns a specific function if node of specific types is
+        two tensors in mixed precision (for loss computation purposes). Returns a specific function if node of specific types is
         given, or a default (normalized MSE) function otherwise.
 
         Args:
             layer_class: Class path of a model's layer.
             framework_attrs: Framework attributes the layer had which the graph node holds.
             compute_distance_fn: An optional distance function to use globally for all nodes.
             axis: The axis on which the operation is preformed (if specified).
+            norm_mse: whether to normalize mse distance function.
 
         Returns: A distance function between two tensors.
         """
 
         if compute_distance_fn is not None:
             return compute_distance_fn
 
@@ -458,15 +454,15 @@
                                    or (layer_class == TFOpLambda and
                                        SOFTMAX in framework_attrs[keras_constants.FUNCTION])):
             return compute_kl_divergence
         elif layer_class == tf.nn.sigmoid:
             return compute_cs
         elif layer_class == Dense:
             return compute_cs
-        return compute_mse
+        return partial(compute_mse, norm=norm_mse)
 
     def get_trace_hessian_calculator(self,
                                      graph: Graph,
                                      input_images: List[Any],
                                      trace_hessian_request: TraceHessianRequest,
                                      num_iterations_for_approximation: int = HESSIAN_NUM_ITERATIONS):
         """
@@ -489,15 +485,15 @@
         elif trace_hessian_request.mode == HessianMode.WEIGHTS:
             return WeightsTraceHessianCalculatorKeras(graph=graph,
                                                       trace_hessian_request=trace_hessian_request,
                                                       input_images=input_images,
                                                       fw_impl=self,
                                                       num_iterations_for_approximation=num_iterations_for_approximation)
         else:
-            Logger.critical(f"Unsupported Hessian mode for Keras: {trace_hessian_request.mode}.")
+            Logger.critical(f"Unsupported Hessian mode for Keras: {trace_hessian_request.mode}.")   # pragma: no cover
 
     def is_output_node_compatible_for_hessian_score_computation(self,
                                                                 node: BaseNode) -> Any:
         """
         Checks and returns whether the given node is compatible as output for Hessian-based information computation.
 
         Args:
@@ -530,26 +526,26 @@
         Returns: The MAC count og the operation
         """
 
         output_shape = node.output_shape
         kernel_shape = node.get_weights_by_keys(fw_info.get_kernel_op_attributes(node.type)[0]).shape
         output_channel_axis, input_channel_axis = fw_info.kernel_channels_mapping.get(node.type)
 
-        if node.type is Conv2D or node.type is Conv2DTranspose:
+        if node.is_match_type(Conv2D) or node.is_match_type(Conv2DTranspose):
             # (C_out * W_out * H_out) * C_in * (W_kernel * H_kernel)
             return np.prod([x for x in output_shape if x is not None]) * \
                    kernel_shape[input_channel_axis] * \
                    (kernel_shape[0] * kernel_shape[1])
-        elif node.type is DepthwiseConv2D:
+        elif node.is_match_type(DepthwiseConv2D):
             # Depth * (W_out * H_out) * C_in * (W_kernel * H_kernel)
             return node.framework_attr.get(DEPTH_MULTIPLIER) * \
                    np.prod([x for x in output_shape if x is not None]) / output_shape[output_channel_axis] * \
                    kernel_shape[input_channel_axis] * \
                    (kernel_shape[0] * kernel_shape[1])
-        elif node.type is Dense:
+        elif node.is_match_type(Dense):
             # IN * OUT
             return kernel_shape[0] * kernel_shape[1]
         else:
             return 0
 
     def apply_second_moment_correction(self,
                                        quantized_model: Any,
@@ -594,31 +590,30 @@
 
         Args:
            node: Node to get quantizers for.
 
         Returns:
             weight_quantizers: A dictionary between a weight's name to its quantizer.
             activation_quantizers: A list of activations quantization, one for each layer output.
-
         """
 
-        def _weight_name(w: str) -> str:
+        def _weight_name(w: Union[str, int]) -> Union[str, int]:
             """
             Extracts the weight name from the full TensorFlow variable name.
 
             For example, returns 'kernel' for 'dense_2/kernel:0'.
 
             Args:
               w: TensorFlow variable name.
 
             Returns:
               Extracted weight name.
             """
 
-            return w.split(':')[0].split('/')[-1]
+            return w.split(':')[0].split('/')[-1] if isinstance(w, str) else w
 
         attribute_names = [_weight_name(wn) for wn in node.get_node_weights_attributes()
                            if node.is_weights_quantization_enabled(wn)]
 
         return get_inferable_quantizers(node,
                                         get_weights_quantizer_for_node,
                                         get_activations_quantizer_for_node,
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/keras_model_validation.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/keras_model_validation.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/keras_node_prior_info.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/keras_node_prior_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 import tensorflow as tf
 from packaging import version
 
 if version.parse(tf.__version__) >= version.parse("2.13"):
     from keras.src.layers import Activation, ReLU, BatchNormalization
 else:
-    from keras.layers import Activation, ReLU, BatchNormalization
+    from keras.layers import Activation, ReLU, BatchNormalization  # pragma: no cover
 
 from model_compression_toolkit.core import FrameworkInfo
 from model_compression_toolkit.core.common import BaseNode
 from model_compression_toolkit.core.common.node_prior_info import NodePriorInfo
 from model_compression_toolkit.core.keras.constants import ACTIVATION, RELU_MAX_VALUE, NEGATIVE_SLOPE, THRESHOLD, \
     GAMMA, BETA, MOVING_MEAN, MOVING_VARIANCE
 from model_compression_toolkit.core.common.graph.base_graph import Graph
@@ -52,21 +52,21 @@
         fw_info: Information about a specific framework the node was generated from.
 
     Returns:
         Min/max output values if known.
     """
     min_output, max_output = None, None
 
-    if node.type == ReLU:
+    if node.is_match_type(ReLU):
         min_output = node.framework_attr[THRESHOLD] if node.framework_attr[NEGATIVE_SLOPE] == 0 else None
 
     elif fw_info.layers_has_min_max(node.type):
         min_output, max_output = fw_info.layer_min_max_mapping[node.type]
 
-    elif node.type == Activation and fw_info.activation_has_min_max(node.framework_attr[ACTIVATION]):
+    elif node.is_match_type(Activation) and fw_info.activation_has_min_max(node.framework_attr[ACTIVATION]):
         min_output, max_output = fw_info.activation_min_max_mapping[node.framework_attr[ACTIVATION]]
 
     return min_output, max_output
 
 
 def _get_mean_std_outputs(node: BaseNode,
                           graph: Graph) -> Tuple[Any, Any]:
@@ -78,24 +78,24 @@
         graph: Graph to check the next node type.
 
     Returns:
         Mean/Std output values if known.
     """
     mean_output, std_output = None, None
 
-    if node.type == BatchNormalization:
+    if node.is_match_type(BatchNormalization):
         mean_output = node.get_weights_by_keys(BETA)
         if node.get_weights_by_keys(GAMMA) is None:
             std_output = 1.0
         else:
             std_output = np.abs(node.get_weights_by_keys(GAMMA))
         if mean_output is None:
             mean_output = 0.0
     else:
         next_node_list = graph.get_next_nodes(node)
-        bn_nodes = [bn_node for bn_node in next_node_list if bn_node.type == BatchNormalization]
+        bn_nodes = [bn_node for bn_node in next_node_list if bn_node.is_match_type(BatchNormalization)]
         if len(bn_nodes) != 0:
             bn_node = bn_nodes[0]
             moving_variance = bn_node.get_weights_by_keys(MOVING_VARIANCE)
             std_output = np.sqrt(moving_variance)
             mean_output = bn_node.get_weights_by_keys(MOVING_MEAN)
     return mean_output, std_output
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/mixed_precision/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/pruning/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,18 +205,17 @@
         node (BaseNode): The node to be evaluated.
 
     Returns:
         bool: True if the node is an edge of a pruning section, False otherwise.
     """
 
     # Check if the node is a Conv2D or Conv2DTranspose layer with groups set to 1.
-    if node.type in [keras.layers.Conv2D, keras.layers.Conv2DTranspose]:
+    if node.is_match_type(keras.layers.Conv2D) or node.is_match_type(keras.layers.Conv2DTranspose):
         return node.framework_attr[GROUPS] == 1
-    return node.type == keras.layers.Dense
-
+    return node.is_match_type(keras.layers.Dense)
 
 
 def _prune_keras_edge_node(node: BaseNode,
                            mask: np.ndarray,
                            fw_info: FrameworkInfo,
                            is_exit_node: bool):
     """
@@ -246,17 +245,17 @@
         # Prune the bias if applicable and it's an entry node.
         bias = node.get_weights_by_keys(BIAS)
         pruned_bias = bias.compress(mask_bool)
         node.set_weights_by_keys(name=BIAS, tensor=pruned_bias)
 
     if not is_exit_node:
         # Update 'filters' or 'units' attributes for entry node Conv2D/Conv2DTranspose layers.
-        if node.type in [keras.layers.Conv2D, keras.layers.Conv2DTranspose]:
+        if node.is_match_type(keras.layers.Conv2D) or node.is_match_type(keras.layers.Conv2DTranspose):
             node.framework_attr[FILTERS] = int(np.sum(mask))
-        elif node.type == keras.layers.Dense:
+        elif node.is_match_type(keras.layers.Dense):
             node.framework_attr[UNITS] = int(np.sum(mask))
 
     if is_exit_node:
         # Adjust the input shape for the last node in the section.
         _edit_node_input_shape(mask_bool, node)
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/quantizer/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/quantizer/base_quantizer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/quantizer/base_quantizer.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,25 @@
 import numpy as np
 from tensorflow.python.util.object_identity import Reference as TFReference
 
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.constants import THRESHOLD, SIGNED, RANGE_MIN, RANGE_MAX
 from model_compression_toolkit.core.common.quantization.quantizers.uniform_quantizers import threshold_is_power_of_two
 
+################################################################
+################################################################
+# TODO:
+#  These quantizer functions are for internal use. They are currently
+#  used in some features like MP for activation and SNC (where
+#  inference in the framework is needed).
+#  It may worth considering removing these functions and use
+#  activation inferable quantizers in those features like we do
+#  in GPTQ.
+################################################################
+################################################################
 
 def quantizer_min_max_calculator(threshold: np.ndarray,
                                  num_bits: int,
                                  signed: bool) -> Tuple[float, float]:
     """
     Compute quantization range's min/max values given a threshold, number of bits,
      and whether it's signed or not.
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/reader/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/reader/common.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/reader/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 
 if version.parse(tf.__version__) >= version.parse("2.13"):
     from keras.src.engine.input_layer import InputLayer
     from keras.src.engine.node import Node as KerasNode
     from keras.src.engine.functional import Functional
     from keras.src.engine.sequential import Sequential
 else:
-    from keras.engine.input_layer import InputLayer
-    from keras.engine.node import Node as KerasNode
-    from keras.engine.functional import Functional
-    from keras.engine.sequential import Sequential
+    from keras.engine.input_layer import InputLayer # pragma: no cover
+    from keras.engine.node import Node as KerasNode # pragma: no cover
+    from keras.engine.functional import Functional # pragma: no cover
+    from keras.engine.sequential import Sequential # pragma: no cover
 
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
 
 
 def is_node_an_input_layer(node: BaseNode) -> bool:
     """
@@ -39,15 +39,15 @@
     Args:
         node: Node to check if its an input layer.
 
     Returns:
         Whether the node represents an input layer or not.
     """
     if isinstance(node, BaseNode):
-        return node.type == InputLayer
+        return node.is_match_type(InputLayer)
     elif isinstance(node, KerasNode):
         return isinstance(node.layer, InputLayer)
     else:
         Logger.critical('Node must be a graph node or a Keras node for input layer check.')  # pragma: no cover
 
 
 def is_node_a_model(node: BaseNode) -> bool:
@@ -56,13 +56,13 @@
     Args:
         node: Node to check if its a Keras model by itself.
 
     Returns:
         Whether the node represents a Keras model or not.
     """
     if isinstance(node, BaseNode):
-        return node.type in [Functional, Sequential]
+        return node.is_match_type(Functional) or node.is_match_type(Sequential)
     elif isinstance(node, KerasNode):
         return isinstance(node.layer, Functional) or isinstance(node.layer, Sequential)
     else:
         Logger.critical('Node must be a graph node or a Keras node.')  # pragma: no cover
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/reader/connectivity_handler.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/reader/connectivity_handler.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/reader/nested_model/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/reader/nested_model/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/reader/node_builder.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/reader/node_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from model_compression_toolkit.core.common.graph.functional_node import FunctionalNode
 
 keras = tf.keras
 layers = keras.layers
 
 REUSED_IDENTIFIER = '_reused_'
 
-is_const = lambda x: isinstance(x, (tf.Variable, tf.Tensor, np.ndarray))
+is_const = lambda x: isinstance(x, (tf.Variable, tf.Tensor, np.ndarray, float))
 is_tensor = lambda x: isinstance(x, KerasTensor)
 
 
 def get_tf_function_symbols() -> List[str]:
     """
     Create a list of tf function symbols, as they are created in the TFOpLambda layer. The
     symbols are serializations of the function names.
@@ -57,26 +57,44 @@
                                            tf.truediv, tf.pow, tf.matmul]]
 
 
 def get_kwargs2index(tfoplambda_layer: TFOpLambda) -> Dict[str, int]:
     """
     Positional weights are saved according to their index in the node's call arguments, so
     need to know the function arguments' names in case the weights are in the kwargs.
+
+    Note: the kwargs2index dictionary is initialized manually (and not with tf_inspect) so
+    it will only include the arguments that may contain constants. For example, we don't
+    want the transpose_a attribute of tf.matmul to be saved as a constant.
+
+    Every operation we add support to, needs to be added here.
+
     Args:
         tfoplambda_layer: TFOpLambda layer.
 
     Returns:
         A dictionary with argument number and index: {arg_name: arg_index}.
     """
-    if tfoplambda_layer.function in [tf.add, tf.subtract, tf.divide, tf.truediv, tf.multiply, tf.pow,
-                                     tf.matmul, tf.image.crop_and_resize, tf.image.combined_non_max_suppression] or \
-            tfoplambda_layer.symbol in ['__operators__.add', 'math.add', 'math.multiply', 'linalg.matmul', 'concat']:
-        return {arg_name: i for i, arg_name in enumerate(tf_inspect.getfullargspec(tfoplambda_layer.function).args)}
-    else:
-        return {}
+    kwargs2index = {tf.add: {'x': 0, 'y': 1},
+                    tf.subtract: {'x': 0, 'y': 1},
+                    tf.divide: {'x': 0, 'y': 1},
+                    tf.truediv: {'x': 0, 'y': 1},
+                    tf.multiply: {'x': 0, 'y': 1},
+                    tf.pow: {'x': 0, 'y': 1},
+                    tf.matmul: {'a': 0, 'b': 1}}.get(tfoplambda_layer.function)
+    if not kwargs2index:
+        # In TF 2.15 the function attribute is different and doesn't match the original
+        # operation object we use. Therefore, we extract kwargs2index with the symbol.
+        kwargs2index = {'__operators__.add': {'x': 0, 'y': 1},
+                        'math.add': {'x': 0, 'y': 1},
+                        'math.multiply': {'x': 0, 'y': 1},
+                        'linalg.matmul': {'a': 0, 'b': 1},
+                        'concat': {'values': 0}}.get(tfoplambda_layer.symbol, {})
+
+    return kwargs2index
 
 
 def build_node(node: KerasNode,
                node_name_to_node: dict) -> BaseNode:
     """
     Build a node from a Keras node. A node contains all information to reconstruct the layer it's representing
     in a model:
@@ -150,16 +168,17 @@
 
         # read weights from call kwargs
         weight_keys = []
         for k, v in op_call_kwargs.items():
             if is_const(v) or (keras_layer.function in [tf.add, tf.multiply, tf.subtract, tf.divide, tf.truediv, tf.pow,
                                                         tf.matmul] and
                                isinstance(v, (tuple, list))):
-                weights.update({kwarg2index[k]: to_numpy(v, is_single_tensor=True)})
-                weight_keys.append(k)
+                if k in kwarg2index:
+                    weights.update({kwarg2index[k]: to_numpy(v, is_single_tensor=True)})
+                    weight_keys.append(k)
         # remove weights and KerasTensors and weights from op_call_kwargs
         op_call_kwargs = {k: v for k, v in op_call_kwargs.items()
                           if not (kwarg2index.get(k) in weights or is_tensor(v))}
 
         node = FunctionalNode(node_name,
                               layer_config,
                               input_shape,
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/reader/reader.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/reader/reader.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/resource_utilization_data_facade.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/resource_utilization_data_facade.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/statistics_correction/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/tf_tensor_numpy.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/tf_tensor_numpy.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         return (to_tf_tensor(t) for t in tensor)
     elif isinstance(tensor, np.ndarray):
         return tf.convert_to_tensor(tensor.astype(np.float32))
     else:
         Logger.critical(f'Unsupported type for conversion to TF tensor: {type(tensor)}.')
 
 
-def tf_tensor_to_numpy(tensor: Union[List, Tuple, np.ndarray, tf.Tensor],
+def tf_tensor_to_numpy(tensor: Union[List, Tuple, np.ndarray, tf.Tensor, float],
                        is_single_tensor=False) -> np.ndarray:
     """
     Convert a TF tensor to a Numpy array.
     Args:
         tensor: TF tensor.
         is_single_tensor: whether input is a value to be converted to a single tensor.
                           if False, recurse the lists and tuples
@@ -61,10 +61,13 @@
             return [tf_tensor_to_numpy(t) for t in tensor]
     elif isinstance(tensor, tuple):
         if is_single_tensor:
             return np.array(tensor)
         else:
             return (tf_tensor_to_numpy(t) for t in tensor)
     elif isinstance(tensor, tf.Tensor):
-        return tensor.numpy()
+        np_tensor = tensor.numpy()
+        return np.array([np_tensor]) if np.isscalar(np_tensor) else np_tensor
+    elif isinstance(tensor, float):
+        return np.array([tensor])
     else:
         Logger.critical(f'Unsupported type for conversion to Numpy array: {type(tensor)}.')
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/keras/visualization/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/keras/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/back2framework/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py`

 * *Files 23% similar despite different names*

```diff
@@ -29,27 +29,13 @@
 
     Returns:
         Pytorch module that was built from the node.
     """
 
     framework_attr = copy.copy(n.framework_attr)
     node_instance = n.type(**framework_attr)
-    node_instance.load_state_dict({k: torch.tensor(v) for k, v in n.weights.items()}, strict=False)
+    # Positional weights act as inputs to the PyTorch layer, rather than serving as its weights.
+    node_instance.load_state_dict({k: torch.tensor(v) for k, v in n.weights.items() if isinstance(k, str)}, strict=False)
     set_model(node_instance)
     return node_instance
 
 
-# todo: remove. It is not used anymore
-def identity_wrapper(node: BaseNode,
-                     module: Module,
-                     include_activation_quantizers: bool):
-    """
-    A function which takes a computational graph node and a pytorch module and return an identity wrapping which return the layer itself
-    Args:
-        node: A node of mct graph.
-        layer: A pytorch module
-        include_activation_quantizers: bool flag.
-    Returns: pytorch module
-    """
-    return module
-
-
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,73 +23,83 @@
 from model_compression_toolkit.core import FrameworkInfo
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common import BaseNode, Graph
 from model_compression_toolkit.core.common.back2framework.base_model_builder import BaseModelBuilder
 from model_compression_toolkit.core.common.graph.edge import EDGE_SINK_INDEX
 from model_compression_toolkit.core.common.graph.functional_node import FunctionalNode
 from model_compression_toolkit.core.common.user_info import UserInformation
-from model_compression_toolkit.core.pytorch.back2framework.instance_builder import node_builder, identity_wrapper
+from model_compression_toolkit.core.pytorch.back2framework.instance_builder import node_builder
 from model_compression_toolkit.core.pytorch.default_framework_info import DEFAULT_PYTORCH_INFO
 from model_compression_toolkit.core.pytorch.pytorch_device_config import get_working_device
 from model_compression_toolkit.core.pytorch.reader.node_holders import DummyPlaceHolder
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor
 from mct_quantizers.common.constants import ACTIVATION_HOLDER_QUANTIZER
+from mct_quantizers import PytorchQuantizationWrapper
 
 
 def _build_input_tensors_list(node: BaseNode,
                               graph: Graph,
                               inputs: Tuple[Any],
-                              node_to_output_tensors_dict: Dict[BaseNode, List]) -> List[List]:
+                              node_to_output_tensors_dict: Dict[BaseNode, List],
+                              is_op_quantize_wrapper: bool) -> List[List]:
     """
-    Given a node, build a list of input tensors the node gets. The list is built
-    based on the node's incoming edges and previous nodes' output tensors.
+    Given a node, build a list of input tensors the node gets. The list is built based on the
+    node's incoming edges, previous nodes' output tensors and the node's positional weights.
+    Positional weights aren't used if the node's op is PytorchQuantizationWrapper, since it's
+    positional weights are already in the wrapper.
 
     Args:
         node: Node to build its input tensors list.
         graph: Graph the node is in.
-        inputs: list of input tensors to model
+        inputs: list of input tensors to model.
         node_to_output_tensors_dict: A dictionary from a node to its output tensors.
+        is_op_quantize_wrapper: Whether the func_op is a PytorchQuantizationWrapper or not.
 
     Returns:
         A list of the node's input tensors.
     """
-    if node.type == DummyPlaceHolder:
+    if node.is_match_type(DummyPlaceHolder):
         input_tensors = [inputs[graph.get_inputs().index(node)]]
     else:
         input_tensors = []
         # Go over a sorted list of the node's incoming edges, and for each source node get its output tensors.
         # Append them in a result list.
         for ie in graph.incoming_edges(node, sort_by_attr=EDGE_SINK_INDEX):
             _input_tensors = node_to_output_tensors_dict[ie.source_node]
             input_tensors.append(_input_tensors)
         input_tensors = [tensor for tensor_list in input_tensors for tensor in tensor_list]  # flat list of lists
         input_tensors = node.insert_positional_weights_to_input_list(input_tensors)
         # convert inputs from positional weights (numpy arrays) to tensors. Must handle each element in the
         # list separately, because in FX the tensors are FX objects and fail to_torch_tensor
-        input_tensors = [to_torch_tensor(t) if isinstance(t, np.ndarray) else t
+        input_tensors = [to_torch_tensor(t, numpy_type=t.dtype) if isinstance(t, np.ndarray) else t
                          for t in input_tensors]
     return input_tensors
 
 
-def _merge_inputs(_node, input_tensors: List, op_call_args: List) -> List:
+def _merge_inputs(_node: BaseNode, input_tensors: List, op_call_args: List,
+                  is_op_quantize_wrapper: bool) -> List:
     """
-    Merge input tensors list with op_call_args, according to correct order
+    Merge input tensors list with op_call_args, according to correct order.
 
     Args:
-        _node: The node the inputs are for
+        _node: The node the inputs are for.
         input_tensors: activation input tensors to node.
-        op_call_args: framework node call args
+        op_call_args: framework node call args.
+        is_op_quantize_wrapper: Whether the func_op is a PytorchQuantizationWrapper or not.
     Returns:
-        Combined list of input_tensors and op_call_args
+        Combined list of input_tensors and op_call_args.
     """
     if isinstance(_node, FunctionalNode) and _node.tensor_input_indices:
-        assert len(_node.tensor_input_indices) == len(input_tensors), 'Mismatch between input tensors and indices'
         _input_list = op_call_args.copy()
-        for i, t in zip(_node.tensor_input_indices, input_tensors):
-            _input_list.insert(i, t)
+        if is_op_quantize_wrapper:
+            _input_list = input_tensors + _input_list
+        else:
+            assert len(_node.tensor_input_indices) == len(input_tensors), 'Mismatch between input tensors and indices'
+            for i, t in zip(_node.tensor_input_indices, input_tensors):
+                _input_list.insert(i, t)
     else:
         _input_list = input_tensors + op_call_args
 
     return _input_list
 
 
 def _run_operation(n: BaseNode,
@@ -114,15 +124,16 @@
     """
 
     op_call_args = n.op_call_args if isinstance(n, FunctionalNode) else []
     functional_kwargs = n.op_call_kwargs if isinstance(n, FunctionalNode) else {}
     if isinstance(n, FunctionalNode) and n.inputs_as_list:
         out_tensors_of_n_float = op_func(input_tensors, *op_call_args, **functional_kwargs)
     else:
-        out_tensors_of_n_float = op_func(*_merge_inputs(n, input_tensors, op_call_args), **functional_kwargs)
+        merged_inputs = _merge_inputs(n, input_tensors, op_call_args, isinstance(op_func, PytorchQuantizationWrapper))
+        out_tensors_of_n_float = op_func(*merged_inputs, **functional_kwargs)
 
     # Add a fake quant node if the node has an activation threshold.
     out_tensors_of_n = out_tensors_of_n_float
     if use_activation_quantization:
         if isinstance(out_tensors_of_n_float, list):
             out_tensors_of_n_float = torch.cat(out_tensors_of_n_float, dim=0)
         out_tensors_of_n = quantize_node_activation_fn(out_tensors_of_n_float)
@@ -275,20 +286,20 @@
         Returns:
             torch Tensor/s which is/are the output of the model logic.
         """
         node_to_output_tensors_dict = dict()
         node_to_output_tensors_dict_float = dict()
         configurable_nodes = self.graph.get_configurable_sorted_nodes_names(DEFAULT_PYTORCH_INFO)
         for node in self.node_sort:
+            op_func = self._get_op_func(node, configurable_nodes)
             input_tensors = _build_input_tensors_list(node,
                                                       self.graph,
                                                       args,
-                                                      node_to_output_tensors_dict)
-
-            op_func = self._get_op_func(node, configurable_nodes)
+                                                      node_to_output_tensors_dict,
+                                                      isinstance(op_func, PytorchQuantizationWrapper))
             use_activation_quantization, activation_quantization_fn = self._get_activation_quantization_fn(node)
 
             # Run node operation and fetch outputs
             out_tensors_of_n, out_tensors_of_n_float = _run_operation(node,
                                                                       input_tensors,
                                                                       op_func=op_func,
                                                                       quantize_node_activation_fn=activation_quantization_fn,
@@ -322,23 +333,24 @@
             configurable_nodes_names: A list of names of configurable nodes in the quantized model.
 
         Returns: Module/functional to apply to the input tensors.
 
         """
         return getattr(self, node.name)
 
-    def _get_activation_quantization_fn(self, node) -> Tuple[bool, bool, Callable]:
+    def _get_activation_quantization_fn(self, node) -> Tuple[bool, Callable]:
         """
         Get activation quantization parameters for this node.
 
         Args:
             node: Node from which to extract the activation quantization parameters.
 
-        Returns: Flag to indicate if we quantize activations, flag to indicate if we quantize activations
-        using a quantization holder and a quantization function to use for the node's activations.
+        Returns:
+            Flag to indicate if we quantize activations using a quantization holder and a quantization
+            function to use for the node's activations.
         """
         activation_quantization_holder = self.node_to_activation_quantization_holder.get(node.name)
         use_activation_quantization = node.is_activation_quantization_enabled()
         if use_activation_quantization:
             if activation_quantization_holder is None:
                 activation_quantization_fn = partial(self._quantize_node_activations, node)
                 use_activation_quantization = self.wrapper is None
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/constants.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/constants.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/default_framework_info.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/default_framework_info.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,19 +58,19 @@
         conv_node: Convolution node to update the weight/kernel.
         kernel: The Convolution node's weight
         weights_scale: Weight scale factor in which to multiply the conv node's weight.
 
     Returns:
         The modified convolution node's weight/kernel/
     """
-    if conv_node.type == ConvTranspose2d:
+    if conv_node.is_match_type(ConvTranspose2d):
         _scale = weights_scale[None, :, None, None]
     else:
         _scale = weights_scale[:, None, None, None]
-    if conv_node.type == ConvTranspose2d and conv_node.framework_attr[GROUPS] > 1:
+    if conv_node.is_match_type(ConvTranspose2d) and conv_node.framework_attr[GROUPS] > 1:
         # PyTorch ConvTranspose2d kernel with groups stacks groups on in_channels axis, so need to reshape the kernel
         # so the groups are stacked on the out_channels axis to match the scale vector (then reshape back to original
         # shape)
         _in_channels = int(conv_node.framework_attr[IN_CHANNELS]/conv_node.framework_attr[GROUPS])
         _out_channels = conv_node.framework_attr[OUT_CHANNELS]
         return (kernel.reshape((_in_channels, _out_channels, -1, 1)) * _scale).reshape(kernel.shape), KERNEL
     else:
@@ -89,18 +89,18 @@
         bias: The Convolution node's bias
         weights_scale: Weight scale factor in which to multiply the conv node's weight.
         bias_factor: factor for kernel to update the bias with: (beta - moving_mean * weights_scale)
 
     Returns:
         The modified convolution node's weight/kernel/
     """
-    if conv_node.type == Conv2d and conv_node.framework_attr[GROUPS] > 1:
+    if conv_node.is_match_type(Conv2d) and conv_node.framework_attr[GROUPS] > 1:
         bias_update = (kernel * bias_factor[:, None, None, None]).flatten()
         _scale = weights_scale[:, None, None, None]
-    elif conv_node.type == ConvTranspose2d:
+    elif conv_node.is_match_type(ConvTranspose2d):
         bias_update = (kernel * bias_factor[:, None, None, None]).sum(axis=0).flatten()
         _scale = weights_scale[:, None, None, None]
     else:
         bias_update = (kernel * bias_factor[None, :, None, None]).sum(axis=1).flatten()
         _scale = weights_scale[None, :, None, None]
     return kernel * _scale, bias + bias_update, KERNEL
 
@@ -121,31 +121,31 @@
     Check whether the node is a group-convolution
     Args:
         node: The Convolution node
 
     Returns:
         True if the node is a group convolution, else False
     """
-    return node.type in [Conv2d, ConvTranspose2d] and \
-           node.framework_attr[GROUPS] not in [node.framework_attr[IN_CHANNELS], 1]
+    return (node.is_match_type(Conv2d) or node.is_match_type(ConvTranspose2d)) and \
+        node.framework_attr[GROUPS] not in [node.framework_attr[IN_CHANNELS], 1]
 
 
 def get_foldable_node_type_and_validity_fn(node: BaseNode) -> [bool, bool]:
     """
     Check whether the node to forward fold is a valid dw-convolution node or a
     batch-normalization node
     Args:
         node: The node to fold
 
     Returns:
         is_bn: True if the node is a batch norm, else False
         is_dw_valid: True if the node is a dw-convolution valid for folding or a batch-norm node, else False
     """
-    is_bn = node.type is BatchNorm2d
-    is_dw = node.type is Conv2d and node.framework_attr[GROUPS] == node.framework_attr[IN_CHANNELS]
+    is_bn = node.is_match_type(BatchNorm2d)
+    is_dw = node.is_match_type(Conv2d) and node.framework_attr[GROUPS] == node.framework_attr[IN_CHANNELS]
     is_dw_valid = is_dw and np.all(np.array(node.get_weights_by_keys(KERNEL).shape[2:]) == 1)
     return is_bn, is_dw_valid
 
 
 def pytorch_batchnorm_folding() -> BatchNormalizationFolding:
     """
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,17 @@
             graph: Graph we apply the substitution on.
             func_node: node that match the pattern in the substitution init.
 
         Returns:
             Graph after applying the substitution.
         """
         # Set new layer
-        if func_node.type == conv2d:
+        if func_node.is_match_type(conv2d):
             new_layer = Conv2d
-        elif func_node.type == conv_transpose2d:
+        elif func_node.is_match_type(conv_transpose2d):
             new_layer = ConvTranspose2d
         else:
             Logger.critical(f'Substitution filter mismatch. Layer {func_node.type}. Must be {type(Conv2d)} or {type(ConvTranspose2d)}.')  # pragma: no cover
 
         out_channel_index, in_channel_index = self.fw_info.kernel_channels_mapping.get(new_layer)
 
         # Create new node of layer convolution
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         first_node: First layer node to collapse to second layer node
         second_node: Second layer node
         kernel_str: The framework specific attribute name of the convolution layer's weight/kernel.
         bias_str: The framework specific attribute name of the convolution layer's bias.
     Returns:
         The modified layer node's weights: kernel, bias
     """
-    if first_node.type == Conv2d and second_node.type == Conv2d:
+    if first_node.is_match_type(Conv2d) and second_node.is_match_type(Conv2d):
         # Get nodes attributes
         kernel1 = first_node.get_weights_by_keys(kernel_str)
         kernel2 = second_node.get_weights_by_keys(kernel_str)
         bias1 = first_node.get_weights_by_keys(bias_str)
         bias2 = second_node.get_weights_by_keys(bias_str)
         strides1 = first_node.framework_attr[STRIDES]
         strides2 = second_node.framework_attr[STRIDES]
@@ -97,15 +97,15 @@
             if bias2 is not None:
                 bias_collapsed += bias2
         elif bias2 is not None:
             bias_collapsed = bias2
 
         return kernel_collapsed, bias_collapsed
     else:
-        Logger.critical(f"Layer collapsing is not supported for the combination of {first_node.type} and {second_node.type}.")
+        Logger.critical(f"Layer collapsing is not supported for the combination of {first_node.type} and {second_node.type}.")  # pragma: no cover
 
 
 def pytorch_linear_collapsing() -> Conv2DCollapsing:
     """
     Returns:
         A Conv2DCollapsing initialized for pytorch models.
     """
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,33 +72,33 @@
         """
 
         first_op2d_node = nodes_list[0]
         non_linear_node = nodes_list[1]
         second_op2d_node = nodes_list[2]
 
         # only act on bound relu with not POT max value and 0 min value
-        if non_linear_node.type == ReLU6:
+        if non_linear_node.is_match_type(ReLU6):
             scale_factor = 6.0 / self.threshold
             non_linear_node.layer_class = Hardtanh
             non_linear_node.framework_attr[INPLACE] = False
             non_linear_node.framework_attr[HARDTANH_MIN_VAL] = 0.0
             non_linear_node.framework_attr[HARDTANH_MAX_VAL] = self.threshold
-        elif non_linear_node.type == relu6:
+        elif non_linear_node.is_match_type(relu6):
             scale_factor = 6.0 / self.threshold
             non_linear_node.functional_op = hardtanh
             non_linear_node.functional_op.__defaults__ = (0.0, self.threshold, False)
-        elif non_linear_node.type == Hardtanh:
+        elif non_linear_node.is_match_type(Hardtanh):
             if (non_linear_node.framework_attr[HARDTANH_MIN_VAL] == 0.0) and not \
                     (np.log2(non_linear_node.framework_attr[HARDTANH_MAX_VAL]).astype(int) -
                      np.log2(non_linear_node.framework_attr[HARDTANH_MAX_VAL]) == 0):
                 scale_factor = non_linear_node.framework_attr[HARDTANH_MAX_VAL] / self.threshold
                 non_linear_node.framework_attr[HARDTANH_MAX_VAL] = self.threshold
             else:
                 return graph
-        elif non_linear_node.type == hardtanh:
+        elif non_linear_node.is_match_type(hardtanh):
             if (non_linear_node.framework_attr[HARDTANH_MIN_VAL] == 0.0) and not \
                     (np.log2(non_linear_node.framework_attr[HARDTANH_MAX_VAL]).astype(int) -
                      np.log2(non_linear_node.framework_attr[HARDTANH_MAX_VAL]) == 0):
                 scale_factor = non_linear_node.framework_attr[HARDTANH_MAX_VAL] / self.threshold
                 non_linear_node.functional_op.__defaults__ = (0.0, self.threshold, non_linear_node.framework_attr[INPLACE])
             else:
                 return graph
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,27 +42,27 @@
     Inspired by https://arxiv.org/pdf/2103.09404.pdf - Algorithm2
     Args:
         first_node: First layer node to collapse into.
         kernel_str: The framework specific attribute name of the convolution layer's weight/kernel.
     Returns:
         The modified layer node's weights: kernel
     """
-    if first_node.type == Conv2d:
+    if first_node.is_match_type(Conv2d):
         # Get nodes attributes
         kernel = first_node.get_weights_by_keys(kernel_str)
         (Cout, Cin, kH, kW) = kernel.shape
 
         # Collapsing residual by adding "1" to kernel diagonal
         idxH = (kH - 1) // 2
         idxW = (kW - 1) // 2
         for i in range(Cout):
             kernel[i, i, idxH, idxW] += 1
         return kernel
     else:
-        Logger.critical(f"Residual collapsing not supported for node type: {first_node.type}")
+        Logger.critical(f"Residual collapsing not supported for node type: {first_node.type}")  # pragma: no cover
 
 
 def pytorch_residual_collapsing() -> ResidualCollapsing:
     """
     Returns:
         A ResidualCollapsing initialized for pytorch models.
     """
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/hessian/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py`

 * *Files 14% similar despite different names*

```diff
@@ -61,10 +61,10 @@
         """
         _unfold_tensors = self.unfold_tensors_list(tensors_to_concate)
         _r_tensors = [torch.reshape(tensor, shape=[tensor.shape[0], -1]) for tensor in _unfold_tensors]
 
         concat_axis_dim = [o.shape[0] for o in _r_tensors]
         if not all(d == concat_axis_dim[0] for d in concat_axis_dim):
             Logger.critical(
-                "Unable to concatenate tensors for gradient calculation due to mismatched shapes along the first axis.")
+                "Unable to concatenate tensors for gradient calculation due to mismatched shapes along the first axis.")  # pragma: no cover
 
         return torch.concat(_r_tensors, dim=1)
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/pruning/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,17 +72,17 @@
         """
         # TODO (reuvenp/liord): Address handling of node parameters that can be either a single value across all channels or distinct per channel, e.g., PReLU. Consider developing a structured approach.
         pruning_en = True
         _edit_node_input_shape(node, input_mask, fw_info)
         pruned_parameters = {}
         mask_bool = output_mask.astype(bool)
         node.weights = pruned_parameters
-        if node.type == torch.nn.BatchNorm2d:
+        if node.is_match_type(torch.nn.BatchNorm2d):
             node.framework_attr[NUM_FEATURES] = int(np.sum(input_mask))
-        elif node.type == torch.nn.PReLU:
+        elif node.is_match_type(torch.nn.PReLU):
             if node.framework_attr[NUM_PARAMETERS] > 1:
                 node.framework_attr[NUM_PARAMETERS] = int(np.sum(input_mask))
             else:
                 pruning_en = False
 
         if pruning_en:
             for k, v in node.weights.items():
@@ -223,17 +223,17 @@
         node (BaseNode): The node to be evaluated.
 
     Returns:
         bool: True if the node is an edge of a pruning section, False otherwise.
     """
 
     # Check if the node is a Conv2D or Conv2DTranspose layer with groups set to 1.
-    if node.type in [torch.nn.Conv2d, torch.nn.ConvTranspose2d]:
+    if node.is_match_type(torch.nn.Conv2d) or node.is_match_type(torch.nn.ConvTranspose2d):
         return node.framework_attr[GROUPS] == 1
-    return node.type == torch.nn.Linear
+    return node.is_match_type(torch.nn.Linear)
 
 
 def _prune_pytorch_edge_node(node: BaseNode,
                              mask: np.ndarray,
                              fw_info: FrameworkInfo,
                              is_exit_node: bool):
     """
@@ -264,26 +264,26 @@
         bias = node.get_weights_by_keys(BIAS)
         pruned_bias = bias.compress(mask_bool)
         node.set_weights_by_keys(name=BIAS, tensor=pruned_bias)
 
     if not is_exit_node:
         # Update 'out_channels' or 'out_features' attributes for entry nodes
         # Conv2d,ConvTranspose2d / Linear layers.
-        if node.type in [torch.nn.Conv2d, torch.nn.ConvTranspose2d]:
+        if node.is_match_type(torch.nn.Conv2d) or node.is_match_type(torch.nn.ConvTranspose2d):
             node.framework_attr[OUT_CHANNELS] = int(np.sum(mask))
-        elif node.type == torch.nn.Linear:
+        elif node.is_match_type(torch.nn.Linear):
             node.framework_attr[OUT_FEATURES] = int(np.sum(mask))
         else:
             Logger.critical(f"{node.type} is currently not supported"
                              f"as an edge node in a pruning section")
 
     if is_exit_node:
-        if node.type in [torch.nn.Conv2d, torch.nn.ConvTranspose2d]:
+        if node.is_match_type(torch.nn.Conv2d) or node.is_match_type(torch.nn.ConvTranspose2d):
             node.framework_attr[IN_CHANNELS] = int(np.sum(mask))
-        elif node.type == torch.nn.Linear:
+        elif node.is_match_type(torch.nn.Linear):
             node.framework_attr[IN_FEATURES] = int(np.sum(mask))
         else:
             Logger.critical(f"{node.type} is currently not supported"
                              f"as an edge node in a pruning section")
         # Adjust the input shape for the last node in the section.
         _edit_node_input_shape(node, mask_bool, fw_info)
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/pytorch_device_config.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/pytorch_device_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,21 +83,24 @@
                 # 'cuda' without a specific index is valid if CUDA is available
                 return True, "Valid device"
 
             try:
                 device_index = int(device_name.split(':')[1])
                 if device_index >= torch.cuda.device_count():
                     return False, f"CUDA device index {device_index} out of range. Number of valid devices: {torch.cuda.device_count()}"
-            except IndexError:
+            except Exception:
                 # Handle cases where the device name is incorrectly formatted
                 return False, "Invalid CUDA device format. Use 'cuda' or 'cuda:x' where x is the device index."
 
             return True, "Valid device"
 
-        return True, "Valid device"
+        if CPU in device_name:
+            return True, "Valid device"
+
+        return False, "Invalid device"
 
 
 
 def set_working_device(device_name: str):
     """
     Set the device for PyTorch operations.
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/pytorch_implementation.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/pytorch_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     import MultiHeadAttentionDecomposition
 from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.permute_call_method import \
     PermuteCallMethod
 from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.const_holder_conv import \
     FunctionalConvSubstitution
 from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.relu_bound_to_power_of_2 import \
     ReLUBoundToPowerOfTwo
+from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.remove_identity import RemoveIdentity
 from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.reshape_with_static_shapes import \
     ReshapeWithStaticShapes
 from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.residual_collapsing import \
     pytorch_residual_collapsing
 from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.scale_equalization import \
     ScaleEqualization, \
     ScaleEqualizationWithPad
@@ -69,14 +70,16 @@
     pytorch_apply_shift_negative_correction
 from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.softmax_shift import \
     pytorch_softmax_shift
 from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.virtual_activation_weights_composition import \
     VirtualActivationWeightsComposition
 from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.weights_activation_split import \
     WeightsActivationSplit
+from model_compression_toolkit.core.pytorch.graph_substitutions.substitutions.concat_threshold_update import \
+    ConcatThresholdUpdate
 from model_compression_toolkit.core.pytorch.hessian.activation_trace_hessian_calculator_pytorch import \
     ActivationTraceHessianCalculatorPytorch
 from model_compression_toolkit.core.pytorch.hessian.weights_trace_hessian_calculator_pytorch import \
     WeightsTraceHessianCalculatorPytorch
 from model_compression_toolkit.core.pytorch.mixed_precision.configurable_activation_quantizer import \
     ConfigurableActivationQuantizer
 from model_compression_toolkit.core.pytorch.mixed_precision.configurable_weights_quantizer import \
@@ -232,15 +235,16 @@
 
         """
         return [ReshapeWithStaticShapes(),
                 MultiHeadAttentionDecomposition(),
                 PermuteCallMethod(),
                 FunctionalConvSubstitution(fw_info),
                 FunctionalBatchNorm(),
-                FunctionalLayerNorm()]
+                FunctionalLayerNorm(),
+                RemoveIdentity()]
 
     def get_substitutions_pre_statistics_collection(self,
                                                     quant_config: QuantizationConfig
                                                     ) -> List[common.BaseSubstitution]:
         """
         Args:
             quant_config: QuantizationConfig to determine which substitutions to return.
@@ -298,21 +302,18 @@
             A list of the framework substitutions used after we collect statistics.
         """
         substitutions_list = []
         if quant_config.softmax_shift:
             substitutions_list.append(pytorch_softmax_shift())
         if quant_config.input_scaling:
             Logger.critical('Input scaling is currently not supported for Pytorch.')
+        if quant_config.concat_threshold_update:
+            substitutions_list.append(ConcatThresholdUpdate())
         return substitutions_list
 
-    def get_substitutions_pre_build(self) -> List[common.BaseSubstitution]:
-        """
-        Returns: A list of the framework substitutions used before we build a quantized module.
-        """
-        return []
 
     def get_substitutions_virtual_weights_activation_coupling(self) -> List[common.BaseSubstitution]:
         """
         Returns: A list of Pytorch substitutions used to build a virtual graph with composed activation-weights pairs.
         """
 
         return [WeightsActivationSplit(),
@@ -393,47 +394,49 @@
         """
         Returns whether a given node in considered as a potential interest point for mp metric computation purposes.
         Args:
             node: Node to indicate whether it needs to be part of the interest points set.
         Returns: True if the node should be considered an interest point, False otherwise.
         """
 
-        if node.type in [Conv2d, Linear, ConvTranspose2d, Sigmoid, sigmoid, Softmax, softmax, operator.add, add, cat,
-                         operator.concat]:
+        if any([node.is_match_type(_type) for _type in [Conv2d, Linear, ConvTranspose2d, Sigmoid, sigmoid, Softmax,
+                                                        softmax, operator.add, add, cat, operator.concat]]):
             return True
         return False
 
-    def get_node_distance_fn(self, layer_class: type,
+    def get_mp_node_distance_fn(self, layer_class: type,
                              framework_attrs: Dict[str, Any],
                              compute_distance_fn: Callable = None,
-                             axis: int = None) -> Callable:
+                             axis: int = None,
+                             norm_mse: bool = False) -> Callable:
         """
         A mapping between layers' types and a distance function for computing the distance between
-        two tensors (for loss computation purposes). Returns a specific function if node of specific types is
+        two tensors in mixed precision (for loss computation purposes). Returns a specific function if node of specific types is
         given, or a default (normalized MSE) function otherwise.
 
         Args:
             layer_class: Class path of a model's layer.
             framework_attrs: Framework attributes the layer had which the graph node holds.
             compute_distance_fn: An optional distance function to use globally for all nodes.
             axis: The axis on which the operation is preformed (if specified).
+            norm_mse: whether to normalize mse distance function.
 
         Returns: A distance function between two tensors.
         """
 
         if compute_distance_fn is not None:
             return compute_distance_fn
 
         elif layer_class in [Softmax, softmax] and axis is not None:
             return compute_kl_divergence
         elif layer_class in [Sigmoid, sigmoid]:
             return compute_cs
         elif layer_class == Linear:
             return compute_cs
-        return compute_mse
+        return partial(compute_mse, norm=norm_mse)
 
     def is_output_node_compatible_for_hessian_score_computation(self,
                                                                 node: BaseNode) -> bool:
         """
         Checks and returns whether the given node is compatible as output for Hessian-based information computation.
 
 
@@ -459,20 +462,20 @@
         Returns: The MAC count of the operation
         """
 
         output_shape = node.output_shape[0]
         kernel_shape = node.get_weights_by_keys(fw_info.get_kernel_op_attributes(node.type)[0]).shape
         output_channel_axis, input_channel_axis = fw_info.kernel_channels_mapping.get(node.type)
 
-        if node.type is Conv2d or node.type is ConvTranspose2d:
+        if node.is_match_type(Conv2d) or node.is_match_type(ConvTranspose2d):
             # (C_out * W_out * H_out) * C_in * (W_kernel * H_kernel)
             return np.prod([x for x in output_shape if x is not None]) * \
                    kernel_shape[input_channel_axis] * \
                    (kernel_shape[0] * kernel_shape[1])
-        elif node.type is Linear:
+        elif node.is_match_type(Linear):
             # IN * OUT
             return kernel_shape[0] * kernel_shape[1]
         else:
             return 0
 
     def apply_second_moment_correction(self,
                                        quantized_model: Any,
@@ -547,14 +550,13 @@
 
         Args:
            node: Node to get quantizers for.
 
         Returns:
             weight_quantizers: A dictionary between a weight's name to its quantizer.
             activation_quantizers: A list of activations quantization, one for each layer output.
-
         """
 
         return get_inferable_quantizers(node,
                                         get_weights_quantizer_for_node,
                                         get_activations_quantizer_for_node,
                                         node.get_node_weights_attributes())
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -58,25 +58,25 @@
         graph: Graph to check the next node type.
 
     Returns:
         Mean/Std output values if known.
     """
     mean_output, std_output = None, None
 
-    if node.type == BatchNorm2d:
+    if node.is_match_type(BatchNorm2d):
         mean_output = node.get_weights_by_keys(BETA)
         if node.get_weights_by_keys(GAMMA) is None:
             std_output = 1.0
         else:
             std_output = np.abs(node.get_weights_by_keys(GAMMA))
         if mean_output is None:
             mean_output = 0.0
     else:
         next_node_list = graph.get_next_nodes(node)
-        bn_nodes = [bn_node for bn_node in next_node_list if bn_node.type == BatchNorm2d]
+        bn_nodes = [bn_node for bn_node in next_node_list if bn_node.is_match_type(BatchNorm2d)]
         if len(bn_nodes) != 0:
             bn_node = bn_nodes[0]
             moving_variance = bn_node.get_weights_by_keys(MOVING_VARIANCE)
             std_output = np.sqrt(moving_variance)
             mean_output = bn_node.get_weights_by_keys(MOVING_MEAN)
 
     return mean_output, std_output
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/quantizer/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,26 @@
 import torch
 
 from model_compression_toolkit.constants import THRESHOLD, SIGNED, RANGE_MIN, RANGE_MAX
 from model_compression_toolkit.core.common.quantization.quantizers.uniform_quantizers import threshold_is_power_of_two
 from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import fix_range_to_include_zero
 
 
+################################################################
+################################################################
+# TODO:
+#  These quantizer functions are for internal use. They are currently
+#  used in some features like MP for activation and SNC (where
+#  inference in the framework is needed).
+#  It may worth considering removing these functions and use
+#  activation inferable quantizers in those features like we do
+#  in GPTQ.
+################################################################
+################################################################
+
 def get_symmetric_quantization_range_and_scale(activation_is_signed: bool,
                                                activation_n_bits: int,
                                                activation_threshold: float):
     """
     Calculates lower and upper bounds on the quantization range, along with quantization scale,
     for symmetric quantization (used for the symmetric and power-of-two quantizers),
     according to whether the quantization is signed or unsigned.
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/reader/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/reader/graph_builders.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/reader/graph_builders.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,14 +134,15 @@
         # extract input shapes and const weights
         input_shape = []
         if node.op != PLACEHOLDER:
             for i, input_node in enumerate(node.all_input_nodes):
                 if input_node in consts_dict:
                     used_consts.add(input_node)
                     weights.update({i: consts_dict[input_node]})
+
                 tensor_meta = input_node.meta
                 if tensor_meta[TYPE] == torch.Tensor:
                     input_shape += [list(tensor_meta[TENSOR_META].shape)]
                 elif tensor_meta[TYPE] == tuple:
                     input_shape += [list(n.shape) for n in tensor_meta[TENSOR_META]]
                 elif tensor_meta[TYPE] == int:
                     input_shape += [[1]]
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/reader/node_holders.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/reader/node_holders.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/reader/reader.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/reader/reader.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/pytorch/utils.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/pytorch/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,34 +34,36 @@
     else:
         model.eval()
 
     device = get_working_device()
     model.to(device)
 
 
-def to_torch_tensor(tensor):
+def to_torch_tensor(tensor,
+                    numpy_type=np.float32):
     """
     Convert a Numpy array to a Torch tensor.
     Args:
         tensor: Numpy array.
+        numpy_type: The desired data type for the tensor. Default is np.float32.
 
     Returns:
         Torch tensor converted from the input Numpy array.
     """
     working_device = get_working_device()
     if isinstance(tensor, torch.Tensor):
         return tensor.to(working_device)
     elif isinstance(tensor, list):
         return [to_torch_tensor(t) for t in tensor]
     elif isinstance(tensor, tuple):
         return (to_torch_tensor(t) for t in tensor)
     elif isinstance(tensor, np.ndarray):
-        return torch.from_numpy(tensor.astype(np.float32)).to(working_device)
+        return torch.from_numpy(tensor.astype(numpy_type)).to(working_device)
     elif isinstance(tensor, (int, float)):
-        return torch.from_numpy(np.array(tensor).astype(np.float32)).to(working_device)
+        return torch.from_numpy(np.array(tensor).astype(numpy_type)).to(working_device)
     else:
         Logger.critical(f'Unsupported type for conversion to Torch.tensor: {type(tensor)}.')
 
 
 def torch_tensor_to_numpy(tensor: Union[torch.Tensor, list, tuple]) -> Union[np.ndarray, list, tuple]:
     """
     Convert a Pytorch tensor to a Numpy array.
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/quantization_prep_runner.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/quantization_prep_runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from typing import Callable
 
 from tqdm import tqdm
 
 from model_compression_toolkit.core.common import FrameworkInfo
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.common.graph.base_graph import Graph
+from model_compression_toolkit.core.common.hessian import HessianInfoService
 from model_compression_toolkit.core.common.model_collector import ModelCollector
 from model_compression_toolkit.core.common.network_editors.edit_network import edit_network_graph
 from model_compression_toolkit.core.common.quantization.core_config import CoreConfig
 from model_compression_toolkit.core.common.quantization.quantization_params_generation.qparams_computation import \
     calculate_quantization_params
 from model_compression_toolkit.core.common.statistics_correction.statistics_correction import \
     statistics_correction_runner
@@ -34,15 +35,16 @@
 
 
 def quantization_preparation_runner(graph: Graph,
                                     representative_data_gen: Callable,
                                     core_config: CoreConfig,
                                     fw_info: FrameworkInfo,
                                     fw_impl: FrameworkImplementation,
-                                    tb_w: TensorboardWriter = None) -> Graph:
+                                    tb_w: TensorboardWriter = None,
+                                    hessian_info_service: HessianInfoService = None,) -> Graph:
     """
     Prepares a trained model for post-training quantization.
     First, the model graph is optimized using several transformations (e.g. folding BatchNormalization to preceding layers).
     Second, statistics (e.g. min/max, histogram, etc.) are collected for each layer's output
     (and input, depends on the quantization configuration) using a given representative dataset.
     Next, quantization parameters are calculated using the collected statistics.
     Finally, more transformations (based on the statistics) are applied to increase the model's performance.
@@ -51,14 +53,15 @@
         graph: A graph representation of the model to be quantized.
         representative_data_gen: Dataset used for calibration.
         core_config: CoreConfig containing parameters of how the model should be quantized
         fw_info: Information needed for quantization about the specific framework (e.g., kernel channels indices,
             groups of layers by how they should be quantized, etc.).
         fw_impl: FrameworkImplementation object with a specific framework methods implementation.
         tb_w: TensorboardWriter object for logging
+        hessian_info_service: HessianInfoService object for retrieving Hessian-based scores.
 
     Returns:
         Graph object that represents the model, contains thresholds, and ready for quantization.
     """
 
     ######################################
     # Statistic collection
@@ -82,15 +85,16 @@
     # there are no final configurations at this stage of the optimization). For this reason we edit the graph
     # again at the end of the optimization process.
     edit_network_graph(graph, fw_info, core_config.debug_config.network_editor)
 
     ######################################
     # Calculate quantization params
     ######################################
-    calculate_quantization_params(graph)
+
+    calculate_quantization_params(graph, hessian_info_service=hessian_info_service)
 
     if tb_w is not None:
         tb_w.add_graph(graph, 'thresholds_selection')
         tb_w.add_all_statistics(graph, 'thresholds_selection')
 
     ######################################
     # Graph substitution (post statistics collection)
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/core/runner.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/core/runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 from typing import Callable, Tuple, Any, List, Dict
 
 import numpy as np
 
 from model_compression_toolkit.core.common import FrameworkInfo
 from model_compression_toolkit.core.common.hessian.hessian_info_service import HessianInfoService
+from model_compression_toolkit.core.common.mixed_precision.resource_utilization_tools.resource_utilization_data import \
+    requires_mixed_precision
 from model_compression_toolkit.core.graph_prep_runner import graph_preparation_runner
 from model_compression_toolkit.core.quantization_prep_runner import quantization_preparation_runner
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.common.graph.base_graph import Graph
 from model_compression_toolkit.core.common.mixed_precision.bit_width_setter import set_bit_widths
 from model_compression_toolkit.core.common.mixed_precision.resource_utilization_tools.resource_utilization import ResourceUtilization, RUTarget
@@ -44,14 +46,15 @@
 def core_runner(in_model: Any,
                 representative_data_gen: Callable,
                 core_config: CoreConfig,
                 fw_info: FrameworkInfo,
                 fw_impl: FrameworkImplementation,
                 tpc: TargetPlatformCapabilities,
                 target_resource_utilization: ResourceUtilization = None,
+                running_gptq: bool = False,
                 tb_w: TensorboardWriter = None):
     """
     Quantize a trained model using post-training quantization.
     First, the model graph is optimized using several transformations (e.g. folding BatchNormalization to preceding
     layers).
     Second, statistics (e.g. min/max, histogram, etc.) are collected for each layer's output
     (and input, depends on the quantization configuration) using a given representative dataset.
@@ -84,35 +87,46 @@
                        ' consider increasing the batch size')
 
     # Checking whether to run mixed precision quantization
     if target_resource_utilization is not None:
         if core_config.mixed_precision_config is None:
             Logger.critical("Provided an initialized target_resource_utilization, that means that mixed precision quantization is "
                             "enabled, but the provided MixedPrecisionQuantizationConfig is None.")
-        core_config.mixed_precision_config.set_mixed_precision_enable()
+        # Determine whether to use mixed precision or single precision based on target_resource_utilization.
+        if requires_mixed_precision(in_model,
+                                    target_resource_utilization,
+                                    representative_data_gen,
+                                    core_config,
+                                    tpc,
+                                    fw_info,
+                                    fw_impl):
+            core_config.mixed_precision_config.set_mixed_precision_enable()
+            Logger.info('Mixed precision enabled.')
 
     graph = graph_preparation_runner(in_model,
                                      representative_data_gen,
                                      core_config.quantization_config,
                                      fw_info,
                                      fw_impl,
                                      tpc,
                                      tb_w,
-                                     mixed_precision_enable=core_config.mixed_precision_enable)
+                                     mixed_precision_enable=core_config.mixed_precision_enable,
+                                     running_gptq=running_gptq)
 
     hessian_info_service = HessianInfoService(graph=graph,
                                               representative_dataset=representative_data_gen,
                                               fw_impl=fw_impl)
 
     tg = quantization_preparation_runner(graph=graph,
                                          representative_data_gen=representative_data_gen,
                                          core_config=core_config,
                                          fw_info=fw_info,
                                          fw_impl=fw_impl,
-                                         tb_w=tb_w)
+                                         tb_w=tb_w,
+                                         hessian_info_service=hessian_info_service)
 
     ######################################
     # Finalize bit widths
     ######################################
     if core_config.mixed_precision_enable:
         if core_config.mixed_precision_config.configuration_overwrite is None:
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-from model_compression_toolkit.constants import FOUND_TORCH, FOUND_TF
+from model_compression_toolkit.constants import FOUND_TORCH, FOUND_TF, FOUND_TORCHVISION
 from model_compression_toolkit.data_generation.common.data_generation_config import DataGenerationConfig
 from model_compression_toolkit.data_generation.common.enums import ImageGranularity, DataInitType, SchedulerType, BNLayerWeightingType, OutputLossType, BatchNormAlignemntLossType, ImagePipelineType, ImageNormalizationType
 
 if FOUND_TF:
     from model_compression_toolkit.data_generation.keras.keras_data_generation import (
         keras_data_generation_experimental, get_keras_data_generation_config)
 
-if FOUND_TORCH:
+if FOUND_TORCH and FOUND_TORCHVISION:
     from model_compression_toolkit.data_generation.pytorch.pytorch_data_generation import (
         pytorch_data_generation_experimental, get_pytorch_data_generation_config)
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/common/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/common/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/common/constants.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/common/constants.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/common/data_generation.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/common/data_generation.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/common/data_generation_config.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/common/data_generation_config.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/common/enums.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/common/enums.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/common/image_pipeline.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/common/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/common/model_info_exctractors.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/common/model_info_exctractors.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,16 +31,15 @@
 
         Args:
             model (Any): The framework model.
             bn_layer_types (List): List of batch normalization layer types.
         """
         self.bn_params = self.get_bn_params(model, bn_layer_types)
         if self.get_num_bn_layers() == 0:
-            Logger.critical(
-                f'Data generation requires a model with at least one BatchNorm layer.')
+            Logger.critical(f'Data generation requires a model with at least one BatchNorm layer.')
 
     def get_bn_layer_names(self) -> List[str]:
         """
         Get the names of all batch normalization layers.
 
         Returns:
             List[str]: List of batch normalization layer names.
@@ -101,15 +100,15 @@
         Args:
             model (Any): The model.
             bn_layer_types (List): List of batch normalization layer types.
 
         Returns:
             dict: Dictionary mapping batch normalization layer names to their parameters.
         """
-        raise NotImplemented
+        raise NotImplemented # pragma: no cover
 
 
 class ActivationExtractor:
     """
     Extracts activations of input tensors to layers in a model.
     """
 
@@ -119,48 +118,48 @@
         """
         Initializes the ActivationExtractor.
 
         Args:
             model (Any): The model.
             layer_types_to_extract_inputs (List): Tuple or list of layer types.
         """
-        raise NotImplemented
+        raise NotImplemented # pragma: no cover
 
     @abstractmethod
     def get_layer_input_activation(self, layer_name: str) -> Any:
         """
         Get the input activation tensor of a layer.
 
         Args:
             layer_name (str): Name of the layer.
 
         Returns:
             Any: Input activation tensor of the layer.
         """
-        raise NotImplemented
+        raise NotImplemented # pragma: no cover
 
     @abstractmethod
     def get_output_layer_input_activation(self) -> List:
         """
         Get the input activation tensors of all the output layers that are Linear or Conv2d.
 
         Returns:
             Any: Input activation tensors of all the output layers that are Linear or Conv2d.
         """
-        raise NotImplemented
+        raise NotImplemented # pragma: no cover
 
     @abstractmethod
     def get_last_linear_layers_weights(self) -> List:
         """
         Get the weight tensors of all the last linear layers.
 
         Returns:
             List: Weight tensors of all the last linear layers.
         """
-        raise NotImplemented
+        raise NotImplemented # pragma: no cover
 
     def get_num_extractor_layers(self) -> int:
         """
         Get the number of layers for which to extract input activations.
 
         Returns:
             int: Number of layers for which to extract input activations.
@@ -171,35 +170,35 @@
     def get_extractor_layer_names(self) -> List:
         """
         Get a list of the layer names for which to extract input activations.
 
         Returns:
             List: A list of layer names for which to extract input activations.
         """
-        raise NotImplemented
+        raise NotImplemented # pragma: no cover
 
     @abstractmethod
     def clear(self):
         """
         Clear the stored activation tensors.
         """
-        raise NotImplemented
+        raise NotImplemented # pragma: no cover
 
     @abstractmethod
     def remove(self):
         """
         Remove the hooks from the model.
         """
-        raise NotImplemented
+        raise NotImplemented # pragma: no cover
 
     @abstractmethod
     def run_model(self, inputs: Any) -> Any:
         """
         Run the model on the given inputs and return the output.
 
         Args:
             inputs (Any): Input tensor.
 
         Returns:
             Any: Output tensor.
         """
-        raise NotImplemented
+        raise NotImplemented # pragma: no cover
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/common/optimization_utils.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/common/optimization_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 
         Args:
             layer_name (str): the name of the layer.
 
         Returns:
             Tuple[Any, Any]: the averaged activation statistics on all the batches for the specified layer.
         """
-        raise NotImplemented
+        raise NotImplemented   # pragma: no cover
 
     def compute_bn_loss(self,
                         input_imgs: Any,
                         batch_index: int,
                         activation_extractor: ActivationExtractor,
                         orig_bn_stats_holder: OriginalBNStatsHolder,
                         bn_alignment_loss_fn: Callable,
@@ -241,35 +241,35 @@
         Perform an optimization step.
 
         Args:
             batch_index (int): Index of the batch.
             loss (Any): The loss value.
             i_ter (int): The current iteration.
         """
-        raise NotImplemented
+        raise NotImplemented   # pragma: no cover
 
     @abstractmethod
     def zero_grad(self, batch_index: int):
         """
         Zero the gradients of the optimizer for the specified batch.
 
         Args:
             batch_index (int): Index of the batch.
         """
-        raise NotImplemented
+        raise NotImplemented   # pragma: no cover
 
     @abstractmethod
     def get_finalized_images(self) -> list:
         """
         Create and return a list of the generated images.
 
         Returns:
             list: a list of the generated images.
         """
-        raise NotImplemented
+        raise NotImplemented   # pragma: no cover
 
 
 class BatchOptimizationHolder:
     """
     Holds optimization parameters for a batch of images.
 
     This class acts as a container for optimization-related parameters specific to a batch of images. It does not
@@ -287,15 +287,15 @@
 
         Args:
             images (Any): a tensor containing the input images.
             optimizer (Any): optimizer responsible for updating the image parameters during optimization.
             scheduler (Any): scheduler responsible for adjusting the learning rate of the optimizer over time.
             initial_lr (float): the initial learning rate used by the optimizer.
         """
-        raise NotImplemented
+        raise NotImplemented   # pragma: no cover
 
     def get_images(self) -> Any:
         """Returns the stored images"""
         return self.images
 
     def get_optimizer(self) -> Any:
         """Returns the optimizer"""
@@ -340,15 +340,15 @@
     def get_batches_stats_holder_list(self) -> list:
         """
         Get a list of batches stats holders.
 
         Returns:
             list: List of batches stats holders.
         """
-        raise NotImplemented
+        raise NotImplemented   # pragma: no cover
 
     def update_batch_stats(self,
                            batch_index: int,
                            input_imgs: Any,
                            activation_extractor: ActivationExtractor,
                            to_differentiate=False):
         """
@@ -438,27 +438,27 @@
 
         Args:
             bn_layer_name (str): the name of the layer.
 
         Returns:
             Any: the variance for the specified layer.
         """
-        raise NotImplemented
+        raise NotImplemented   # pragma: no cover
 
     def get_std(self, bn_layer_name: str) -> Any:
         """
         Calculate the standart deviation for the specified layer.
 
         Args:
             bn_layer_name (str): the name of the layer.
 
         Returns:
             Any: the variance for the specified layer.
         """
-        raise NotImplemented
+        raise NotImplemented   # pragma: no cover
 
     def update_layer_stats(self,
                            bn_layer_name: str,
                            mean: Any,
                            second_moment: Any):
         """
         Update the statistics for a layer.
@@ -479,15 +479,15 @@
         Calculate statistics from the input images and activation extractor.
 
         Args:
             input_imgs (Any): the input images tensor for which to calculate the statistics.
             activation_extractor (ActivationExtractor): the activation extractor object.
             to_differentiate (bool): a flag indicating whether to differentiate or not.
         """
-        raise NotImplemented
+        raise NotImplemented   # pragma: no cover
 
     def clear(self):
         """Clear the statistics."""
         self.bn_mean.clear()
         self.bn_second_moment.clear()
         self.bn_mean = {}
         self.bn_second_moment = {}
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/constants.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/constants.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/image_pipeline.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/keras_data_generation.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/keras_data_generation.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/model_info_exctractors.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/model_info_exctractors.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/keras/optimization_utils.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/keras/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/constants.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/constants.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/image_pipeline.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/optimization_utils.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 import time
 from typing import Callable, Any, Tuple, List
 
 from tqdm import tqdm
 
-from model_compression_toolkit.constants import FOUND_TORCH
+from model_compression_toolkit.constants import FOUND_TORCH, FOUND_TORCHVISION
 from model_compression_toolkit.core.pytorch.utils import set_model
 from model_compression_toolkit.data_generation.common.constants import DEFAULT_N_ITER, DEFAULT_DATA_GEN_BS
 from model_compression_toolkit.data_generation.common.data_generation import get_data_generation_classes
 from model_compression_toolkit.data_generation.common.data_generation_config import DataGenerationConfig
 from model_compression_toolkit.data_generation.common.enums import ImageGranularity, SchedulerType, \
     BatchNormAlignemntLossType, DataInitType, BNLayerWeightingType, ImagePipelineType, ImageNormalizationType, \
     OutputLossType
@@ -40,15 +40,15 @@
 from model_compression_toolkit.data_generation.pytorch.optimization_functions.output_loss_functions import \
     output_loss_function_dict
 from model_compression_toolkit.data_generation.pytorch.optimization_functions.scheduler_step_functions import \
     scheduler_step_function_dict
 from model_compression_toolkit.data_generation.pytorch.optimization_utils import PytorchImagesOptimizationHandler
 from model_compression_toolkit.logger import Logger
 
-if FOUND_TORCH:
+if FOUND_TORCH and FOUND_TORCHVISION:
     # Importing necessary libraries
     import torch
     from torch import Tensor
     from torch.nn import Module
     from torch.optim import RAdam, Optimizer
     from torch.fx import symbolic_trace
 
@@ -350,14 +350,13 @@
         finalized_imgs = all_imgs_opt_handler.get_finalized_images()
         Logger.info(f'Total time to generate {len(finalized_imgs)} images (seconds): {int(time.time() - total_time)}')
         return finalized_imgs
 else:
     # If torch is not installed,
     # we raise an exception when trying to use these functions.
     def get_pytorch_data_generation_config(*args, **kwargs):
-        Logger.critical('PyTorch must be installed to use get_pytorch_data_generation_config. '
-                        "The 'torch' package is missing.")  # pragma: no cover
-
+        msg = f"PyTorch and torchvision must be installed to use get_pytorch_data_generation_config. " + ("" if FOUND_TORCH else "The 'torch' package is missing. ") + ("" if FOUND_TORCHVISION else "The 'torchvision' package is missing. ") # pragma: no cover
+        Logger.critical(msg)  # pragma: no cover
 
     def pytorch_data_generation_experimental(*args, **kwargs):
-        Logger.critical("PyTorch must be installed to use 'pytorch_data_generation_experimental'. "
-                        "The 'torch' package is missing.")  # pragma: no cover
+        msg = f"PyTorch and torchvision must be installed to use pytorch_data_generation_experimental. " + ("" if FOUND_TORCH else "The 'torch' package is missing. ") + ("" if FOUND_TORCHVISION else "The 'torchvision' package is missing. ") # pragma: no cover
+        Logger.critical(msg)  # pragma: no cover
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/defaultdict.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/defaultdict.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/keras/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                     # Create a list of weights for the new created layer
                     if isinstance(layer.layer, layers.DepthwiseConv2D):
                         weights_list.append(layer.get_quantized_weights()['depthwise_kernel'])
                     elif isinstance(layer.layer, (layers.Conv2D, layers.Dense, layers.Conv2DTranspose)):
                         weights_list.append(layer.get_quantized_weights()['kernel'])
                     else:
                         Logger.critical(f'KerasQuantizationWrapper should wrap only DepthwiseConv2D, Conv2D, Dense'
-                                     f' and Conv2DTranspose layers but wrapped layer is {layer.layer}')
+                                        f' and Conv2DTranspose layers but wrapped layer is {layer.layer}')
 
                     if layer.layer.bias is not None:
                         weights_list.append(layer.layer.bias)
 
                     # In order to add the weights of the layer, we need to build it. To build it
                     # we need to pass its input shape. Not every layer has input_shape since some
                     # layers may have multiple inputs with different input shapes (reused layers for
@@ -117,14 +117,19 @@
                     new_layer.set_weights(weights_list)
                     new_layer.trainable = False
 
                     return new_layer
 
             return layer
 
+        # Delete metadata layer if exists
+        if hasattr(self.model, 'metadata_layer'):
+            Logger.info('Metadata is not exported to FakelyQuant models.')
+            delattr(self.model, 'metadata_layer')
+
         # clone each layer in the model and apply _unwrap_quantize_wrapper to layers wrapped with a QuantizeWrapper.
         self.exported_model = tf.keras.models.clone_model(self.model,
                                                           input_tensors=None,
                                                           clone_function=_unwrap_quantize_wrapper)
 
         # Transform the model's configuration to convert KerasActivationQuantizationHolder to fake-quant layers
         new_cfg = self.transform_model_cfg()
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,14 +52,19 @@
 
     def export(self):
         """
         Convert an exportable (fully-quantized) Keras model to a fakely-quant TFLite model
         (namely, weights that are in fake-quant format) and fake-quant layers for the activations.
 
         """
+        # Delete metadata layer if exists
+        if hasattr(self.model, 'metadata_layer'):
+            Logger.info('Metadata is not exported to TFLite models.')
+            delattr(self.model, 'metadata_layer')
+
         # Use Keras exporter to quantize model's weights before converting it to TFLite.
         # Since exporter saves the model, we use a tmp path for saving, and then we delete it.
         handle, tmp_file = tempfile.mkstemp(DEFAULT_KERAS_EXPORT_EXTENTION)
         # Close handle right away, the file is going to be reopenned by Keras exporter
         os.close(handle)
         try:
             custom_objects = FakelyQuantKerasExporter(self.model,
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,19 @@
             # point-wise convolution.
             if isinstance(layer_to_substitue, KerasQuantizationWrapper):
                 if isinstance(layer_to_substitue.layer, Dense):
                     return self._get_pointwise_layer_to_replace_dense(layer_to_substitue)
 
             return layer_to_substitue
 
+        # Delete metadata layer if exists
+        if hasattr(self.model, 'metadata_layer'):
+            Logger.info('Metadata is not exported to TFLite models.')
+            delattr(self.model, 'metadata_layer')
+
         # Transform the model to a new model that can be converted to int8 models.
         # For example: replace dense layers with point-wise layers (to support per-channel quantization)
         self.transformed_model = clone_model(self.model,
                                              clone_function=_substitute_model)
 
         # Convert model to int8 representation
         converter = tf.lite.TFLiteConverter.from_keras_model(self.transformed_model)
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,106 +9,130 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Callable
+from io import BytesIO
 
 import torch.nn
 
 from mct_quantizers import PytorchActivationQuantizationHolder, PytorchQuantizationWrapper
+from model_compression_toolkit.constants import FOUND_ONNX
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor
 from model_compression_toolkit.exporter.model_exporter.pytorch.base_pytorch_exporter import BasePyTorchExporter
 from mct_quantizers import pytorch_quantizers
 
-DEFAULT_ONNX_OPSET_VERSION=15
 
-class FakelyQuantONNXPyTorchExporter(BasePyTorchExporter):
-    """
-    Exporter for fakely-quant PyTorch models.
-    The exporter expects to receive an exportable model (where each layer's full quantization parameters
-    can be retrieved), and convert it into a fakely-quant model (namely, weights that are in fake-quant
-    format) and fake-quant layers for the activations.
-    """
-
-    def __init__(self,
-                 model: torch.nn.Module,
-                 is_layer_exportable_fn: Callable,
-                 save_model_path: str,
-                 repr_dataset: Callable,
-                 use_onnx_custom_quantizer_ops: bool = False,
-                 onnx_opset_version=DEFAULT_ONNX_OPSET_VERSION):
-        """
-
-        Args:
-            model: Model to export.
-            is_layer_exportable_fn: Callable to check whether a layer can be exported or not.
-            save_model_path: Path to save the exported model.
-            repr_dataset: Representative dataset (needed for creating torch script).
-            use_onnx_custom_quantizer_ops: Whether to export quantizers custom ops in ONNX or not.
-            onnx_opset_version: ONNX opset version to use for exported ONNX model.
-        """
-
-        super().__init__(model,
-                         is_layer_exportable_fn,
-                         save_model_path,
-                         repr_dataset)
-
-        self._use_onnx_custom_quantizer_ops = use_onnx_custom_quantizer_ops
-        self._onnx_opset_version = onnx_opset_version
-
-
-    def export(self) -> None:
-        """
-        Convert an exportable (fully-quantized) PyTorch model to a fakely-quant model
-        (namely, weights that are in fake-quant format) and fake-quant layers for the activations.
-
-        Returns:
-            Fake-quant PyTorch model.
-        """
-        for layer in self.model.children():
-            self.is_layer_exportable_fn(layer)
-
-        # Set forward that is used during onnx export.
-        # If _use_onnx_custom_quantizer_ops is set to True, the quantizer forward function will use
-        # the custom implementation when exporting the operator into onnx model. If not, it removes the
-        # wraps and quantizes the ops in place (for weights, for activation torch quantization function is
-        # exported since it's used during forward.
-        if self._use_onnx_custom_quantizer_ops:
-            self._enable_onnx_custom_ops_export()
-        else:
-            self._substitute_fully_quantized_model()
-
-        if self._use_onnx_custom_quantizer_ops:
-            Logger.info(f"Exporting onnx model with MCTQ quantizers: {self.save_model_path}")
-        else:
-            Logger.info(f"Exporting fake-quant onnx model: {self.save_model_path}")
-
-        model_input = to_torch_tensor(next(self.repr_dataset())[0])
-
-        torch.onnx.export(self.model,
-                          model_input,
-                          self.save_model_path,
-                          opset_version=self._onnx_opset_version,
-                          verbose=False,
-                          input_names=['input'],
-                          output_names=['output'],
-                          dynamic_axes={'input': {0: 'batch_size'},
-                                        'output': {0: 'batch_size'}})
-
-    def _enable_onnx_custom_ops_export(self):
-        """
-        Enable the custom implementation forward in quantizers, so it is exported
-        with custom quantizers.
-        """
-
-        for n, m in self.model.named_children():
-            if isinstance(m, PytorchActivationQuantizationHolder):
-                assert isinstance(m.activation_holder_quantizer, pytorch_quantizers.BasePyTorchInferableQuantizer)
-                m.activation_holder_quantizer.enable_custom_impl()
-
-            if isinstance(m, PytorchQuantizationWrapper):
-                for wq in m.weights_quantizers.values():
-                    assert isinstance(wq, pytorch_quantizers.BasePyTorchInferableQuantizer)
-                    wq.enable_custom_impl()
+if FOUND_ONNX:
+    import onnx
+    from mct_quantizers.pytorch.metadata import add_onnx_metadata
+
+    class FakelyQuantONNXPyTorchExporter(BasePyTorchExporter):
+        """
+        Exporter for fakely-quant PyTorch models.
+        The exporter expects to receive an exportable model (where each layer's full quantization parameters
+        can be retrieved), and convert it into a fakely-quant model (namely, weights that are in fake-quant
+        format) and fake-quant layers for the activations.
+        """
+
+        def __init__(self,
+                     model: torch.nn.Module,
+                     is_layer_exportable_fn: Callable,
+                     save_model_path: str,
+                     repr_dataset: Callable,
+                     onnx_opset_version: int,
+                     use_onnx_custom_quantizer_ops: bool = False):
+            """
+
+            Args:
+                model: Model to export.
+                is_layer_exportable_fn: Callable to check whether a layer can be exported or not.
+                save_model_path: Path to save the exported model.
+                repr_dataset: Representative dataset (needed for creating torch script).
+                onnx_opset_version: ONNX opset version to use for exported ONNX model.
+                use_onnx_custom_quantizer_ops: Whether to export quantizers custom ops in ONNX or not.
+            """
+
+            super().__init__(model,
+                             is_layer_exportable_fn,
+                             save_model_path,
+                             repr_dataset)
+
+            self._use_onnx_custom_quantizer_ops = use_onnx_custom_quantizer_ops
+            self._onnx_opset_version = onnx_opset_version
+
+        def export(self) -> None:
+            """
+            Convert an exportable (fully-quantized) PyTorch model to a fakely-quant model
+            (namely, weights that are in fake-quant format) and fake-quant layers for the activations.
+
+            Returns:
+                Fake-quant PyTorch model.
+            """
+            for layer in self.model.children():
+                self.is_layer_exportable_fn(layer)
+
+            # Set forward that is used during onnx export.
+            # If _use_onnx_custom_quantizer_ops is set to True, the quantizer forward function will use
+            # the custom implementation when exporting the operator into onnx model. If not, it removes the
+            # wraps and quantizes the ops in place (for weights, for activation torch quantization function is
+            # exported since it's used during forward).
+            if self._use_onnx_custom_quantizer_ops:
+                self._enable_onnx_custom_ops_export()
+            else:
+                self._substitute_fully_quantized_model()
+
+            if self._use_onnx_custom_quantizer_ops:
+                Logger.info(f"Exporting onnx model with MCTQ quantizers: {self.save_model_path}")
+            else:
+                Logger.info(f"Exporting fake-quant onnx model: {self.save_model_path}")
+
+            model_input = to_torch_tensor(next(self.repr_dataset())[0])
+
+            if hasattr(self.model, 'metadata'):
+                onnx_bytes = BytesIO()
+                torch.onnx.export(self.model,
+                                  model_input,
+                                  onnx_bytes,
+                                  opset_version=self._onnx_opset_version,
+                                  verbose=False,
+                                  input_names=['input'],
+                                  output_names=['output'],
+                                  dynamic_axes={'input': {0: 'batch_size'},
+                                                'output': {0: 'batch_size'}})
+                onnx_model = onnx.load_from_string(onnx_bytes.getvalue())
+                onnx_model = add_onnx_metadata(onnx_model, self.model.metadata)
+                onnx.save_model(onnx_model, self.save_model_path)
+            else:
+                torch.onnx.export(self.model,
+                                  model_input,
+                                  self.save_model_path,
+                                  opset_version=self._onnx_opset_version,
+                                  verbose=False,
+                                  input_names=['input'],
+                                  output_names=['output'],
+                                  dynamic_axes={'input': {0: 'batch_size'},
+                                                'output': {0: 'batch_size'}})
+
+        def _enable_onnx_custom_ops_export(self):
+            """
+            Enable the custom implementation forward in quantizers, so it is exported
+            with custom quantizers.
+            """
+
+            for n, m in self.model.named_modules():
+                if isinstance(m, PytorchActivationQuantizationHolder):
+                    assert isinstance(m.activation_holder_quantizer, pytorch_quantizers.BasePyTorchInferableQuantizer)
+                    m.activation_holder_quantizer.enable_custom_impl()
+
+                if isinstance(m, PytorchQuantizationWrapper):
+                    for wq in m.weights_quantizers.values():
+                        assert isinstance(wq, pytorch_quantizers.BasePyTorchInferableQuantizer)
+                        wq.enable_custom_impl()
+
+else:
+    def FakelyQuantONNXPyTorchExporter(*args, **kwargs):
+        Logger.critical("ONNX must be installed to use 'FakelyQuantONNXPyTorchExporter'. "
+                        "The 'onnx' package is missing.")  # pragma: no cover
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,36 +15,36 @@
 from typing import Callable
 
 from model_compression_toolkit.constants import FOUND_TORCH
 from model_compression_toolkit.exporter.model_exporter.fw_agonstic.quantization_format import QuantizationFormat
 from model_compression_toolkit.exporter.model_exporter.pytorch.export_serialization_format import \
     PytorchExportSerializationFormat
 from model_compression_toolkit.logger import Logger
-from model_compression_toolkit.target_platform_capabilities.target_platform import TargetPlatformCapabilities
+
+
+DEFAULT_ONNX_OPSET_VERSION = 15
 
 
 if FOUND_TORCH:
     import torch.nn
-    from model_compression_toolkit.exporter.model_exporter.pytorch.fakely_quant_onnx_pytorch_exporter import \
-    FakelyQuantONNXPyTorchExporter, DEFAULT_ONNX_OPSET_VERSION
-    from model_compression_toolkit.exporter.model_exporter.pytorch.fakely_quant_torchscript_pytorch_exporter import \
-        FakelyQuantTorchScriptPyTorchExporter
+    from model_compression_toolkit.exporter.model_exporter.pytorch.fakely_quant_onnx_pytorch_exporter import FakelyQuantONNXPyTorchExporter
+    from model_compression_toolkit.exporter.model_exporter.pytorch.fakely_quant_torchscript_pytorch_exporter import FakelyQuantTorchScriptPyTorchExporter
     from model_compression_toolkit.exporter.model_wrapper.pytorch.validate_layer import is_pytorch_layer_exportable
 
     supported_serialization_quantization_export_dict = {
         PytorchExportSerializationFormat.TORCHSCRIPT: [QuantizationFormat.FAKELY_QUANT],
         PytorchExportSerializationFormat.ONNX: [QuantizationFormat.FAKELY_QUANT, QuantizationFormat.MCTQ]
     }
 
     def pytorch_export_model(model: torch.nn.Module,
                              save_model_path: str,
                              repr_dataset: Callable,
                              is_layer_exportable_fn: Callable = is_pytorch_layer_exportable,
                              serialization_format: PytorchExportSerializationFormat = PytorchExportSerializationFormat.ONNX,
-                             quantization_format : QuantizationFormat = QuantizationFormat.MCTQ,
+                             quantization_format: QuantizationFormat = QuantizationFormat.MCTQ,
                              onnx_opset_version=DEFAULT_ONNX_OPSET_VERSION) -> None:
         """
         Export a PyTorch quantized model to a torchscript or onnx model.
         The model will be saved to the path in save_model_path.
         Currently, pytorch_export_model supports only QuantizationFormat.FAKELY_QUANT (where weights
         and activations are float fakely-quantized values) and PytorchExportSerializationFormat.TORCHSCRIPT
         (where the model will be saved to TorchScript model) or PytorchExportSerializationFormat.ONNX
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,20 @@
             layer: A keras layer
 
         Returns: Wrapped layer with weights quantizers and activation quantizers
 
         """
         weights_quantizers, _ = fw_impl.get_inferable_quantizers(node)
         if len(weights_quantizers) > 0:
+            # for positional weights we need to extract the weight's value.
+            weights_values = {attr: node.get_weights_by_keys(attr)
+                              for attr in weights_quantizers if isinstance(attr, int)}
             return KerasQuantizationWrapper(layer,
-                                            weights_quantizers)
+                                            weights_quantizers,
+                                            weights_values)
         return layer
 
 
     def get_activation_quantizer_holder(node: common.BaseNode, fw_impl) -> Callable:
         """
         Retrieve a ActivationQuantizationHolder layer to use for activation quantization for a node.
 
@@ -86,15 +90,15 @@
                                                         _get_wrapper(n, kn,
                                                                      fw_impl=C.keras.keras_implementation.KerasImplementation()),
                                                         get_activation_quantizer_holder_fn=lambda n:
                                                         get_activation_quantizer_holder(n,
                                                                                         fw_impl=C.keras.keras_implementation.KerasImplementation())).build_model()
         exportable_model.trainable = False
 
-        Logger.info("Please run your accuracy evaluation on the exported quantized model to verify it's accuracy.\n"
+        Logger.info("\nPlease run your accuracy evaluation on the exported quantized model to verify it's accuracy.\n"
                     "Checkout the FAQ and Troubleshooting pages for resolving common issues and improving the quantized model accuracy:\n"
                     "FAQ: https://github.com/sony/model_optimization/tree/main/FAQ.md\n"
                     "Quantization Troubleshooting: https://github.com/sony/model_optimization/tree/main/quantization_troubleshooting.md")
         return exportable_model, user_info
 else:
     def get_exportable_keras_model(*args, **kwargs):  # pragma: no cover
         Logger.critical("Tensorflow must be installed to use get_exportable_keras_model. "
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,49 +25,56 @@
     import torch
     from mct_quantizers import PytorchQuantizationWrapper, PytorchActivationQuantizationHolder
     from model_compression_toolkit.core.pytorch.back2framework.pytorch_model_builder import PyTorchModelBuilder
 
 
     def fully_quantized_wrapper(node: common.BaseNode,
                                 module: torch.nn.Module,
-                                fw_impl) -> Union[torch.nn.Module,PytorchQuantizationWrapper]:
+                                fw_impl) -> Union[torch.nn.Module, PytorchQuantizationWrapper]:
         """
         A function which takes a computational graph node and a pytorch module and
         perform the quantization wrapping
 
         Args:
             node: A node of mct graph.
             module: A Pytorch module
+            fw_impl: FrameworkImplementation object with a specific framework methods implementation.
         Returns: Wrapped layer
 
         """
         weight_quantizers, _ = fw_impl.get_inferable_quantizers(node)
         if len(weight_quantizers) > 0:
-            return PytorchQuantizationWrapper(module, weight_quantizers)
+            # for positional weights we need to extract the weight's value.
+            weights_values = {attr: fw_impl.to_tensor(node.get_weights_by_keys(attr))
+                              for attr in weight_quantizers if isinstance(attr, int)}
+            return PytorchQuantizationWrapper(module, weight_quantizers, weights_values)
         return module
 
+
     def get_activation_quantizer_holder(node: BaseNode, fw_impl) -> Callable:
         """
         Retrieve a PytorchActivationQuantizationHolder layer to use for activation quantization of a node.
         If the layer is not supposed to be wrapped with an activation quantizer - return None.
         Args:
             node: Node to attach a PytorchActivationQuantizationHolder to its output.
+            fw_impl: FrameworkImplementation object with a specific framework methods implementation.
         Returns:
             A PytorchActivationQuantizationHolder module for the node's activation quantization.
         """
         _, activation_quantizers = fw_impl.get_inferable_quantizers(node)
         # Holder by definition uses a single quantizer for the activation quantization
         # thus we make sure this is the only possible case (unless it's a node we no activation
         # quantization, which in this case has an empty list).
         if len(activation_quantizers) == 1:
             return PytorchActivationQuantizationHolder(activation_quantizers[0])
         Logger.critical(
             f'PytorchActivationQuantizationHolder supports a single quantizer but {len(activation_quantizers)} quantizers '
             f'were found for node {node}')
 
+
     def get_exportable_pytorch_model(graph: Graph):
         """
         Convert graph to fully quantized PyTorch model.
 
         Args:
             graph: Graph to convert to a PyTorch model.
 
@@ -78,19 +85,19 @@
                                                           wrapper=lambda n, m:
                                                           fully_quantized_wrapper(n, m,
                                                                                   fw_impl=C.pytorch.pytorch_implementation.PytorchImplementation()),
                                                           get_activation_quantizer_holder_fn=lambda n:
                                                           get_activation_quantizer_holder(n,
                                                                                           fw_impl=C.pytorch.pytorch_implementation.PytorchImplementation())).build_model()
 
-        Logger.info("Please run your accuracy evaluation on the exported quantized model to verify it's accuracy.\n"
+        Logger.info("\nPlease run your accuracy evaluation on the exported quantized model to verify it's accuracy.\n"
                     "Checkout the FAQ and Troubleshooting pages for resolving common issues and improving the quantized model accuracy:\n"
                     "FAQ: https://github.com/sony/model_optimization/tree/main/FAQ.md\n"
                     "Quantization Troubleshooting: https://github.com/sony/model_optimization/tree/main/quantization_troubleshooting.md")
 
         return exportable_model, user_info
 
 
 else:
     def get_exportable_pytorch_model(*args, **kwargs):
         Logger.critical("PyTorch must be installed to use 'get_exportable_pytorch_model'. "
-                        "The 'torch' package is missing.")  # pragma: no cover
+                        "The 'torch' package is missing.")  # pragma: no cover
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/common/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/common/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/common/gptq_config.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/common/gptq_config.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/common/gptq_constants.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/common/gptq_constants.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/common/gptq_framework_implementation.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/common/gptq_framework_implementation.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/common/gptq_graph.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/common/gptq_graph.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/common/gptq_training.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/common/gptq_training.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,15 +72,15 @@
                                                                        append2output=self.compare_points,
                                                                        fw_info=self.fw_info)
 
         self.fxp_model, self.gptq_user_info = self.build_gptq_model()
         if self.gptq_config.use_hessian_based_weights:
             if not isinstance(hessian_info_service, HessianInfoService):
                 Logger.critical(f"When using Hessian-based approximations for sensitivity evaluation, "
-                                f"an 'HessianInfoService' object must be provided, but received: {hessian_info_service}.")
+                                f"an 'HessianInfoService' object must be provided, but received: {hessian_info_service}.")   # pragma: no cover
             self.hessian_service = hessian_info_service
 
     def get_optimizer_with_param(self,
                                  flattened_trainable_weights: List[Any],
                                  flattened_bias_weights: List[Any],
                                  trainable_quantization_parameters: List[Any]) -> List[Any]:
         """
@@ -234,55 +234,20 @@
         """
         Validates the structure and length of the trace approximation.
 
         Args:
             trace_approx: Trace approximation to validate.
         """
         if not isinstance(trace_approx, list):
-            Logger.critical(f"Trace approximation was expected to be a list but is of type: {type(trace_approx)}.")
+            Logger.critical(f"Trace approximation was expected to be a list but is of type: {type(trace_approx)}.")   # pragma: no cover
         if len(trace_approx) != 1:
             Logger.critical(f"Trace approximation was expected to have a length of 1 "
                             f"(for computations with granularity set to 'HessianInfoGranularity.PER_TENSOR') "
                             f"but has a length of {len(trace_approx)}."
-            )
-
-    @staticmethod
-    def _generate_images_batch(representative_data_gen: Callable, num_samples_for_loss: int) -> np.ndarray:
-        """
-        Construct batches of image samples for inference.
-
-        Args:
-            representative_data_gen: A callable method to retrieve images from Dataset.
-            num_samples_for_loss: Num of total images for evaluation.
-
-        Returns: A tensor of images batches
-        """
-        # First, select images to use for all measurements.
-        samples_count = 0  # Number of images we used so far to compute the distance matrix.
-        images = []
-        for inference_batch_input in representative_data_gen():
-            if samples_count >= num_samples_for_loss:
-                break
-            num_images = inference_batch_input[0].shape[0]
-
-            # If we sampled more images than we should,
-            # we take only a subset of these images and use only them.
-            if num_images > num_samples_for_loss - samples_count:
-                inference_batch_input = [x[:num_samples_for_loss - samples_count] for x in inference_batch_input]
-                assert num_samples_for_loss - samples_count == inference_batch_input[0].shape[0]
-                num_images = num_samples_for_loss - samples_count
-
-            images.append(inference_batch_input[0])
-            samples_count += num_images
-        else:
-            if samples_count < num_samples_for_loss:
-                Logger.warning(f'Not enough images in representative dataset to generate {num_samples_for_loss} data points, '
-                               f'only {samples_count} were generated')
-
-        return np.concatenate(images, axis=0)
+            )   # pragma: no cover
 
 
     @abstractmethod
     def build_gptq_model(self):
         """
         Build the GPTQ model with QuantizationWrappers
         Returns:
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/gptq_loss.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/gptq_training.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/gptq_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,29 +297,31 @@
             in_optimizer_with_param: A list of optimizer classes to update with the corresponding parameters.
             n_epochs: Number of update iterations of representative dataset.
             is_training: A boolean flag stating if the network is running in training mode.
 
         Returns: None
 
         """
-        for _ in tqdm(range(n_epochs)):
-            for data in tqdm(data_function()):
-                input_data = [d * self.input_scale for d in data]
+        with tqdm(range(n_epochs), "Running GPTQ optimization") as epochs_pbar:
+            for _ in epochs_pbar:
+                with tqdm(data_function(), position=1, leave=False) as data_pbar:
+                    for data in data_pbar:
+                        input_data = [d * self.input_scale for d in data]
 
-                loss_value_step, grads = self.nano_training_step(input_data, in_compute_gradients,
-                                                                 in_optimizer_with_param, is_training)
-                # Run one step of gradient descent by updating
-                # the value of the variables to minimize the loss.
-                for i, (o, p) in enumerate(in_optimizer_with_param):
-                    o.apply_gradients(zip(grads[i], p))
-                if self.gptq_config.log_function is not None:
-                    self.gptq_config.log_function(loss_value_step, grads[0], in_optimizer_with_param[0][-1],
-                                                  self.compare_points)
-                self.loss_list.append(loss_value_step.numpy())
-                Logger.debug(f'last loss value: {self.loss_list[-1]}')
+                        loss_value_step, grads = self.nano_training_step(input_data, in_compute_gradients,
+                                                                         in_optimizer_with_param, is_training)
+                        # Run one step of gradient descent by updating
+                        # the value of the variables to minimize the loss.
+                        for i, (o, p) in enumerate(in_optimizer_with_param):
+                            o.apply_gradients(zip(grads[i], p))
+                        if self.gptq_config.log_function is not None:
+                            self.gptq_config.log_function(loss_value_step, grads[0], in_optimizer_with_param[0][-1],
+                                                          self.compare_points)
+                        self.loss_list.append(loss_value_step.numpy())
+                        Logger.debug(f'last loss value: {self.loss_list[-1]}')
 
     def update_graph(self):
         """
         Update a graph using GPTQ after minimizing the loss between the float model's output
         and the quantized model's outputs.
         Returns:
             Updated graph after GPTQ.
@@ -333,20 +335,24 @@
                     node = graph.find_node_by_name('_'.join(layer.layer.name.split('_')[3:]))
                 if len(node) != 1:
                     Logger.critical(f"Unable to update the GPTQ graph because the layer named '{layer.layer.name}' could not be found. "
                                     f"Verify that the layer names in the GPTQ model match those in the graph.")
                 node = node[0]
                 kernel_attribute = get_kernel_attribute_name_for_gptq(layer_type=node.type,
                                                                       fw_info=self.fw_info)
+                # TODO: only kernel attributes are currently trained in GPTQ, so only the kernel weights need to be updated.
+                #  To enable GPTQ for other attributes, this code needs to be modified.
                 weights, weight_quant_config, activation_quant_config = \
                     layer.weights_quantizers[kernel_attribute].update_layer_quantization_params(layer)
                 for weight_attr, weight in weights.items():
                     node.set_weights_by_keys(weight_attr, weight.numpy())
-                for config_attr, config_value in weight_quant_config.items():
-                    node.final_weights_quantization_cfg.set_quant_config_attr(config_attr, config_value)
+                for config_parameter_name, config_parameter_value in weight_quant_config.items():
+                    node.final_weights_quantization_cfg.set_quant_config_attr(config_parameter_name,
+                                                                              config_parameter_value,
+                                                                              attr_name=kernel_attribute)
                 for config_attr, config_value in activation_quant_config.items():
                     node.final_activation_quantization_cfg.set_quant_config_attr(config_attr, config_value)
                 if self.gptq_config.train_bias:
                     use_bias = layer.layer.get_config().get(USE_BIAS)
                     if use_bias is not None and use_bias:
                         new_bias = layer.layer.bias.numpy()
                         node.set_weights_by_keys(BIAS, new_bias)
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/graph_info.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/graph_info.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantization_facade.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantization_facade.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,33 +8,34 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+import copy
 
 from typing import Callable, Tuple
 from packaging import version
 
+from model_compression_toolkit.core.common.quantization.quantize_graph_weights import quantize_graph_weights
 from model_compression_toolkit.core.common.visualization.tensorboard_writer import init_tensorboard_writer
 from model_compression_toolkit.gptq.common.gptq_constants import REG_DEFAULT
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.constants import TENSORFLOW, FOUND_TF
 from model_compression_toolkit.core.common.user_info import UserInformation
 from model_compression_toolkit.gptq.common.gptq_config import GradientPTQConfig
 from model_compression_toolkit.core.common.mixed_precision.resource_utilization_tools.resource_utilization import ResourceUtilization
-from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.mixed_precision.mixed_precision_quantization_config import MixedPrecisionQuantizationConfig
 from model_compression_toolkit.core import CoreConfig
 from model_compression_toolkit.core.runner import core_runner
 from model_compression_toolkit.gptq.runner import gptq_runner
-from model_compression_toolkit.core.exporter import export_model
 from model_compression_toolkit.core.analyzer import analyzer_model_quantization
 from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework import TargetPlatformCapabilities
+from model_compression_toolkit.metadata import get_versions_dict
 
 LR_DEFAULT = 0.15
 LR_REST_DEFAULT = 1e-4
 LR_BIAS_DEFAULT = 1e-4
 LR_QUANTIZATION_PARAM_DEFAULT = 1e-3
 GPTQ_MOMENTUM = 0.9
 
@@ -44,14 +45,15 @@
     from model_compression_toolkit.gptq.keras.gptq_keras_implementation import GPTQKerasImplemantation
     from model_compression_toolkit.core.keras.keras_model_validation import KerasModelValidation
     from tensorflow.keras.models import Model
     from model_compression_toolkit.gptq.keras.gptq_loss import GPTQMultipleTensorsLoss
     from model_compression_toolkit.target_platform_capabilities.constants import DEFAULT_TP_MODEL
     from model_compression_toolkit.exporter.model_wrapper import get_exportable_keras_model
     from model_compression_toolkit import get_target_platform_capabilities
+    from mct_quantizers.keras.metadata import add_metadata
 
     # As from TF2.9 optimizers package is changed
     if version.parse(tf.__version__) < version.parse("2.9"):
         from keras.optimizer_v2.optimizer_v2 import OptimizerV2
     elif version.parse(tf.__version__) < version.parse("2.12"):
         from keras.optimizers.optimizer_v2.optimizer_v2 import OptimizerV2
     else:
@@ -206,32 +208,43 @@
         tg, bit_widths_config, hessian_info_service = core_runner(in_model=in_model,
                                                                   representative_data_gen=representative_data_gen,
                                                                   core_config=core_config,
                                                                   fw_info=DEFAULT_KERAS_INFO,
                                                                   fw_impl=fw_impl,
                                                                   tpc=target_platform_capabilities,
                                                                   target_resource_utilization=target_resource_utilization,
-                                                                  tb_w=tb_w)
+                                                                  tb_w=tb_w,
+                                                                  running_gptq=True)
+
+        float_graph = copy.deepcopy(tg)
 
         tg_gptq = gptq_runner(tg,
                               core_config,
                               gptq_config,
                               representative_data_gen,
                               gptq_representative_data_gen if gptq_representative_data_gen else representative_data_gen,
                               DEFAULT_KERAS_INFO,
                               fw_impl,
                               tb_w,
                               hessian_info_service=hessian_info_service)
 
         del hessian_info_service
 
         if core_config.debug_config.analyze_similarity:
-            analyzer_model_quantization(representative_data_gen, tb_w, tg_gptq, fw_impl, fw_info)
-
-        return get_exportable_keras_model(tg_gptq)
+            analyzer_model_quantization(representative_data_gen,
+                                        tb_w,
+                                        float_graph,
+                                        tg_gptq,
+                                        fw_impl,
+                                        DEFAULT_KERAS_INFO)
+
+        exportable_model, user_info = get_exportable_keras_model(tg_gptq)
+        if target_platform_capabilities.tp_model.add_metadata:
+            exportable_model = add_metadata(exportable_model, get_versions_dict(target_platform_capabilities))
+        return exportable_model, user_info
 
 else:
     # If tensorflow is not installed,
     # we raise an exception when trying to use these functions.
     def get_keras_gptq_config(*args, **kwargs):
         Logger.critical("Tensorflow must be installed to use get_keras_gptq_config. "
                         "The 'tensorflow' package is missing.")  # pragma: no cover
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+from tqdm import tqdm
 from typing import Callable
 
 from model_compression_toolkit.gptq import RoundingType, GradientPTQConfig, GradientPTQConfig
 from model_compression_toolkit.gptq.keras.quantizer.soft_rounding.soft_quantizer_reg import \
     SoftQuantizerRegularization
 
 
@@ -31,13 +32,13 @@
     Returns: A function for computing the regularization. If there is no regularization function defined for the given
         rounding type, then it returns a function that just returns 0.
 
     """
     if gptq_config.rounding_type == RoundingType.SoftQuantizer:
         # dry run on the representative dataset to count number of batches
         num_batches = 0
-        for _ in representative_data_gen():
+        for _ in tqdm(representative_data_gen(), "GPTQ initialization"):
             num_batches += 1
 
         return SoftQuantizerRegularization(total_gradient_steps=num_batches * gptq_config.n_epochs)
     else:
         return lambda m, e_reg: 0
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/gptq_loss.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/gptq_training.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/gptq_training.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,30 +244,32 @@
                             n_epochs: int):
         """
         This function run a micro training loop on given set of parameters.
         Args:
             data_function: A callable function that give a batch of samples.
             n_epochs: Number of update iterations of representative dataset.
         """
-        for _ in tqdm(range(n_epochs)):
-            for data in tqdm(data_function()):
-                input_data = [d * self.input_scale for d in data]
-                input_tensor = to_torch_tensor(input_data)
-                y_float = self.float_model(input_tensor)  # running float model
-                loss_value, grads = self.compute_gradients(y_float, input_tensor)
-                # Run one step of gradient descent by updating the value of the variables to minimize the loss.
-                for (optimizer, _) in self.optimizer_with_param:
-                    optimizer.step()
-                    optimizer.zero_grad()
-                if self.gptq_config.log_function is not None:
-                    self.gptq_config.log_function(loss_value.item(),
-                                                  torch_tensor_to_numpy(grads),
-                                                  torch_tensor_to_numpy(self.optimizer_with_param[0][-1]))
-                self.loss_list.append(loss_value.item())
-                Logger.debug(f'last loss value: {self.loss_list[-1]}')
+        with tqdm(range(n_epochs), "Running GPTQ optimization") as epochs_pbar:
+            for _ in epochs_pbar:
+                with tqdm(data_function(), position=1, leave=False) as data_pbar:
+                    for data in data_pbar:
+                        input_data = [d * self.input_scale for d in data]
+                        input_tensor = to_torch_tensor(input_data)
+                        y_float = self.float_model(input_tensor)  # running float model
+                        loss_value, grads = self.compute_gradients(y_float, input_tensor)
+                        # Run one step of gradient descent by updating the value of the variables to minimize the loss.
+                        for (optimizer, _) in self.optimizer_with_param:
+                            optimizer.step()
+                            optimizer.zero_grad()
+                        if self.gptq_config.log_function is not None:
+                            self.gptq_config.log_function(loss_value.item(),
+                                                          torch_tensor_to_numpy(grads),
+                                                          torch_tensor_to_numpy(self.optimizer_with_param[0][-1]))
+                        self.loss_list.append(loss_value.item())
+                        Logger.debug(f'last loss value: {self.loss_list[-1]}')
 
     def update_graph(self) -> Graph:
         """
         Update a graph using GPTQ after minimizing the loss between the float model's output
         and the quantized model's outputs.
         Returns:
             Updated graph after GPTQ.
@@ -280,20 +282,24 @@
                 node = self.graph_quant.find_node_by_name(name)
                 if len(node) != 1:
                     Logger.critical(f"Cannot update GPTQ graph: Layer with name '{name}' is missing or not unique. "
                                     f"Ensure each layer has a unique name and exists within the graph for updates.")
                 node = node[0]
                 kernel_attribute = get_kernel_attribute_name_for_gptq(layer_type=node.type,
                                                                       fw_info=self.fw_info)
+                # TODO: only kernel attributes are currently trained in GPTQ, so only the kernel weights need to be updated.
+                #  To enable GPTQ for other attributes, this code needs to be modified.
                 weights, weight_quant_config, activation_quant_config = \
                     layer.weights_quantizers[kernel_attribute].update_layer_quantization_params(layer)
                 for weight_attr, weight in weights.items():
                     node.set_weights_by_keys(weight_attr, self.fw_impl.to_numpy(weight))
-                for config_attr, config_value in weight_quant_config.items():
-                    node.final_weights_quantization_cfg.set_quant_config_attr(config_attr, config_value)
+                for config_parameter_name, config_parameter_value in weight_quant_config.items():
+                    node.final_weights_quantization_cfg.set_quant_config_attr(config_parameter_name,
+                                                                              config_parameter_value,
+                                                                              attr_name=kernel_attribute)
                 for config_attr, config_value in activation_quant_config.items():
                     node.final_activation_quantization_cfg.set_quant_config_attr(config_attr, config_value)
                 if self.gptq_config.train_bias and hasattr(layer.layer, BIAS):
                     node.set_weights_by_keys(BIAS, self.fw_impl.to_numpy(getattr(layer.layer, BIAS)))
 
         return graph_quant
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/graph_info.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/graph_info.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantization_facade.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantization_facade.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,32 +8,34 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+import copy
+
 from typing import Callable
 from model_compression_toolkit.core import common
 from model_compression_toolkit.constants import FOUND_TORCH
 from model_compression_toolkit.core.common.visualization.tensorboard_writer import init_tensorboard_writer
 from model_compression_toolkit.gptq.common.gptq_constants import REG_DEFAULT
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.constants import PYTORCH
 from model_compression_toolkit.gptq.common.gptq_config import GradientPTQConfig
 from model_compression_toolkit.target_platform_capabilities.target_platform import TargetPlatformCapabilities
 from model_compression_toolkit.core.common.mixed_precision.resource_utilization_tools.resource_utilization import ResourceUtilization
 from model_compression_toolkit.core.runner import core_runner
 from model_compression_toolkit.gptq.keras.quantization_facade import GPTQ_MOMENTUM
 from model_compression_toolkit.gptq.runner import gptq_runner
-from model_compression_toolkit.core.exporter import export_model
 from model_compression_toolkit.core.analyzer import analyzer_model_quantization
 from model_compression_toolkit.core import CoreConfig
 from model_compression_toolkit.core.common.mixed_precision.mixed_precision_quantization_config import \
     MixedPrecisionQuantizationConfig
+from model_compression_toolkit.metadata import get_versions_dict
 
 LR_DEFAULT = 1e-4
 LR_REST_DEFAULT = 1e-4
 LR_BIAS_DEFAULT = 1e-4
 LR_QUANTIZATION_PARAM_DEFAULT = 1e-4
 
 if FOUND_TORCH:
@@ -42,14 +44,15 @@
     from model_compression_toolkit.target_platform_capabilities.constants import DEFAULT_TP_MODEL
     from model_compression_toolkit.gptq.pytorch.gptq_loss import multiple_tensors_mse_loss
     from model_compression_toolkit.exporter.model_wrapper.pytorch.builder.fully_quantized_model_builder import get_exportable_pytorch_model
     import torch
     from torch.nn import Module
     from torch.optim import Adam, Optimizer
     from model_compression_toolkit import get_target_platform_capabilities
+    from mct_quantizers.pytorch.metadata import add_metadata
     DEFAULT_PYTORCH_TPC = get_target_platform_capabilities(PYTORCH, DEFAULT_TP_MODEL)
 
     def get_pytorch_gptq_config(n_epochs: int,
                                 optimizer: Optimizer = Adam([torch.Tensor([])], lr=LR_DEFAULT),
                                 optimizer_rest: Optimizer = Adam([torch.Tensor([])], lr=LR_REST_DEFAULT),
                                 loss: Callable = multiple_tensors_mse_loss,
                                 log_function: Callable = None,
@@ -173,15 +176,18 @@
         graph, bit_widths_config, hessian_info_service = core_runner(in_model=model,
                                                                      representative_data_gen=representative_data_gen,
                                                                      core_config=core_config,
                                                                      fw_info=DEFAULT_PYTORCH_INFO,
                                                                      fw_impl=fw_impl,
                                                                      tpc=target_platform_capabilities,
                                                                      target_resource_utilization=target_resource_utilization,
-                                                                     tb_w=tb_w)
+                                                                     tb_w=tb_w,
+                                                                     running_gptq=True)
+
+        float_graph = copy.deepcopy(graph)
 
         # ---------------------- #
         # GPTQ Runner
         # ---------------------- #
         graph_gptq = gptq_runner(graph,
                                  core_config,
                                  gptq_config,
@@ -189,17 +195,25 @@
                                  gptq_representative_data_gen if gptq_representative_data_gen else representative_data_gen,
                                  DEFAULT_PYTORCH_INFO,
                                  fw_impl,
                                  tb_w,
                                  hessian_info_service=hessian_info_service)
 
         if core_config.debug_config.analyze_similarity:
-            analyzer_model_quantization(representative_data_gen, tb_w, graph_gptq, fw_impl, DEFAULT_PYTORCH_INFO)
-
-        return get_exportable_pytorch_model(graph_gptq)
+            analyzer_model_quantization(representative_data_gen,
+                                        tb_w,
+                                        float_graph,
+                                        graph_gptq,
+                                        fw_impl,
+                                        DEFAULT_PYTORCH_INFO)
+
+        exportable_model, user_info = get_exportable_pytorch_model(graph_gptq)
+        if target_platform_capabilities.tp_model.add_metadata:
+            exportable_model = add_metadata(exportable_model, get_versions_dict(target_platform_capabilities))
+        return exportable_model, user_info
 
 
 else:
     # If torch is not installed,
     # we raise an exception when trying to use these functions.
     def get_pytorch_gptq_config(*args, **kwargs):
         Logger.critical("PyTorch must be installed to use 'get_pytorch_gptq_config'. "
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+from tqdm import tqdm
 from typing import Callable
 
 from model_compression_toolkit.gptq import RoundingType, GradientPTQConfig, GradientPTQConfig
 from model_compression_toolkit.gptq.pytorch.quantizer.soft_rounding.soft_quantizer_reg import \
     SoftQuantizerRegularization
 
 
@@ -31,13 +32,13 @@
     Returns: A function for computing the regularization. If there is no regularization function defined for the given
         rounding type, then it returns a function that just returns 0.
 
     """
     if gptq_config.rounding_type == RoundingType.SoftQuantizer:
         # dry run on the representative dataset to count number of batches
         num_batches = 0
-        for _ in representative_data_gen():
+        for _ in tqdm(representative_data_gen(), "GPTQ initialization"):
             num_batches += 1
 
         return SoftQuantizerRegularization(total_gradient_steps=num_batches * gptq_config.n_epochs)
     else:
         return lambda m, e_reg: 0
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/gptq/runner.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/gptq/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
     tg_bias = apply_statistics_correction(tg, representative_data_gen, core_config, fw_info, fw_impl, tb_w)
 
     if tb_w is not None:
         tb_w.add_graph(tg_bias, 'after_bias_correction')
     #############################################
     # Gradient Based Post Training Quantization
     #############################################
+    Logger.info("Running GPTQ optimization.")
     tg_gptq = _apply_gptq(gptq_config,
                           gptq_representative_data_gen,
                           tb_w,
                           tg,
                           tg_bias,
                           fw_info,
                           fw_impl,
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/logger.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/logger.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/pruning/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/pruning/keras/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/pruning/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/pruning/keras/pruning_facade.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/pruning/keras/pruning_facade.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/pruning/pytorch/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/pruning/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/pruning/pytorch/pruning_facade.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/pruning/pytorch/pruning_facade.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/ptq/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/ptq/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/ptq/keras/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/ptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/ptq/keras/quantization_facade.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/ptq/keras/quantization_facade.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,39 +8,42 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+import copy
 
 from typing import Callable
 
 from model_compression_toolkit.core import CoreConfig
 from model_compression_toolkit.core.analyzer import analyzer_model_quantization
+from model_compression_toolkit.core.common.quantization.quantize_graph_weights import quantize_graph_weights
 from model_compression_toolkit.core.common.visualization.tensorboard_writer import init_tensorboard_writer
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.constants import TENSORFLOW, FOUND_TF
 from model_compression_toolkit.core.common.mixed_precision.resource_utilization_tools.resource_utilization import ResourceUtilization
 from model_compression_toolkit.core.common.mixed_precision.mixed_precision_quantization_config import \
     MixedPrecisionQuantizationConfig
 from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework import TargetPlatformCapabilities
-from model_compression_toolkit.core.exporter import export_model
 from model_compression_toolkit.core.runner import core_runner
 from model_compression_toolkit.ptq.runner import ptq_runner
+from model_compression_toolkit.metadata import get_versions_dict
 
 if FOUND_TF:
     from model_compression_toolkit.core.keras.default_framework_info import DEFAULT_KERAS_INFO
     from model_compression_toolkit.core.keras.keras_implementation import KerasImplementation
     from model_compression_toolkit.core.keras.keras_model_validation import KerasModelValidation
     from tensorflow.keras.models import Model
     from model_compression_toolkit.target_platform_capabilities.constants import DEFAULT_TP_MODEL
     from model_compression_toolkit.exporter.model_wrapper import get_exportable_keras_model
 
     from model_compression_toolkit import get_target_platform_capabilities
+    from mct_quantizers.keras.metadata import add_metadata
     DEFAULT_KERAS_TPC = get_target_platform_capabilities(TENSORFLOW, DEFAULT_TP_MODEL)
 
 
     def keras_post_training_quantization(in_model: Model,
                                          representative_data_gen: Callable,
                                          target_resource_utilization: ResourceUtilization = None,
                                          core_config: CoreConfig = CoreConfig(),
@@ -119,16 +122,16 @@
 
         KerasModelValidation(model=in_model,
                              fw_info=fw_info).validate()
 
         if core_config.mixed_precision_enable:
             if not isinstance(core_config.mixed_precision_config, MixedPrecisionQuantizationConfig):
                 Logger.critical("Given quantization config to mixed-precision facade is not of type "
-                                    "MixedPrecisionQuantizationConfig. Please use keras_post_training_quantization "
-                                    "API, or pass a valid mixed precision configuration.")  # pragma: no cover
+                                "MixedPrecisionQuantizationConfig. Please use keras_post_training_quantization "
+                                "API, or pass a valid mixed precision configuration.")  # pragma: no cover
 
         tb_w = init_tensorboard_writer(fw_info)
 
         fw_impl = KerasImplementation()
 
         # Ignore returned hessian service as PTQ does not use it
         tg, bit_widths_config, _ = core_runner(in_model=in_model,
@@ -136,24 +139,41 @@
                                                core_config=core_config,
                                                fw_info=fw_info,
                                                fw_impl=fw_impl,
                                                tpc=target_platform_capabilities,
                                                target_resource_utilization=target_resource_utilization,
                                                tb_w=tb_w)
 
-        tg = ptq_runner(tg, representative_data_gen, core_config, fw_info, fw_impl, tb_w)
+        # At this point, tg is a graph that went through substitutions (such as BN folding) and is
+        # ready for quantization (namely, it holds quantization params, etc.) but the weights are
+        # not quantized yet. For this reason, we use it to create a graph that acts as a "float" graph
+        # for things like similarity analyzer (because the quantized and float graph should have the same
+        # architecture to find the appropriate compare points for similarity computation).
+        similarity_baseline_graph = copy.deepcopy(tg)
+
+        graph_with_stats_correction = ptq_runner(tg,
+                                                 representative_data_gen,
+                                                 core_config,
+                                                 fw_info,
+                                                 fw_impl,
+                                                 tb_w)
 
         if core_config.debug_config.analyze_similarity:
+            quantized_graph = quantize_graph_weights(graph_with_stats_correction)
             analyzer_model_quantization(representative_data_gen,
-                                        tb_w, tg,
+                                        tb_w,
+                                        similarity_baseline_graph,
+                                        quantized_graph,
                                         fw_impl,
                                         fw_info)
 
-        return get_exportable_keras_model(tg)
-
+        exportable_model, user_info = get_exportable_keras_model(graph_with_stats_correction)
+        if target_platform_capabilities.tp_model.add_metadata:
+            exportable_model = add_metadata(exportable_model, get_versions_dict(target_platform_capabilities))
+        return exportable_model, user_info
 
 
 else:
     # If tensorflow is not installed,
     # we raise an exception when trying to use these functions.
     def keras_post_training_quantization(*args, **kwargs):
         Logger.critical("Tensorflow must be installed to use keras_post_training_quantization. "
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/ptq/pytorch/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/ptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/ptq/pytorch/quantization_facade.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/ptq/pytorch/quantization_facade.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,38 +8,42 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+import copy
+
 from typing import Callable
 
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common.visualization.tensorboard_writer import init_tensorboard_writer
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.constants import PYTORCH, FOUND_TORCH
 from model_compression_toolkit.target_platform_capabilities.target_platform import TargetPlatformCapabilities
 from model_compression_toolkit.core.common.mixed_precision.resource_utilization_tools.resource_utilization import ResourceUtilization
 from model_compression_toolkit.core import CoreConfig
 from model_compression_toolkit.core.common.mixed_precision.mixed_precision_quantization_config import \
     MixedPrecisionQuantizationConfig
 from model_compression_toolkit.core.runner import core_runner
 from model_compression_toolkit.ptq.runner import ptq_runner
-from model_compression_toolkit.core.exporter import export_model
 from model_compression_toolkit.core.analyzer import analyzer_model_quantization
+from model_compression_toolkit.core.common.quantization.quantize_graph_weights import quantize_graph_weights
+from model_compression_toolkit.metadata import get_versions_dict
 
 
 if FOUND_TORCH:
     from model_compression_toolkit.core.pytorch.default_framework_info import DEFAULT_PYTORCH_INFO
     from model_compression_toolkit.core.pytorch.pytorch_implementation import PytorchImplementation
     from model_compression_toolkit.target_platform_capabilities.constants import DEFAULT_TP_MODEL
     from torch.nn import Module
     from model_compression_toolkit.exporter.model_wrapper.pytorch.builder.fully_quantized_model_builder import get_exportable_pytorch_model
     from model_compression_toolkit import get_target_platform_capabilities
+    from mct_quantizers.pytorch.metadata import add_metadata
 
     DEFAULT_PYTORCH_TPC = get_target_platform_capabilities(PYTORCH, DEFAULT_TP_MODEL)
 
     def pytorch_post_training_quantization(in_module: Module,
                                            representative_data_gen: Callable,
                                            target_resource_utilization: ResourceUtilization = None,
                                            core_config: CoreConfig = CoreConfig(),
@@ -87,45 +91,64 @@
             Set number of clibration iterations to 1:
 
             >>> import model_compression_toolkit as mct
             >>> quantized_module, quantization_info = mct.ptq.pytorch_post_training_quantization(module, repr_datagen)
 
         """
 
+        fw_info = DEFAULT_PYTORCH_INFO
+
         if core_config.mixed_precision_enable:
             if not isinstance(core_config.mixed_precision_config, MixedPrecisionQuantizationConfig):
                 Logger.critical("Given quantization config to mixed-precision facade is not of type "
-                             "MixedPrecisionQuantizationConfig. Please use "
-                             "pytorch_post_training_quantization API, or pass a valid mixed precision "
-                             "configuration.")  # pragma: no cover
+                                "MixedPrecisionQuantizationConfig. Please use "
+                                "pytorch_post_training_quantization API, or pass a valid mixed precision "
+                                "configuration.")  # pragma: no cover
 
-        tb_w = init_tensorboard_writer(DEFAULT_PYTORCH_INFO)
+        tb_w = init_tensorboard_writer(fw_info)
 
         fw_impl = PytorchImplementation()
 
         # Ignore hessian info service as it is not used here yet.
         tg, bit_widths_config, _ = core_runner(in_model=in_module,
                                                representative_data_gen=representative_data_gen,
                                                core_config=core_config,
-                                               fw_info=DEFAULT_PYTORCH_INFO,
+                                               fw_info=fw_info,
                                                fw_impl=fw_impl,
                                                tpc=target_platform_capabilities,
                                                target_resource_utilization=target_resource_utilization,
                                                tb_w=tb_w)
 
-        tg = ptq_runner(tg, representative_data_gen, core_config, DEFAULT_PYTORCH_INFO, fw_impl, tb_w)
+        # At this point, tg is a graph that went through substitutions (such as BN folding) and is
+        # ready for quantization (namely, it holds quantization params, etc.) but the weights are
+        # not quantized yet. For this reason, we use it to create a graph that acts as a "float" graph
+        # for things like similarity analyzer (because the quantized and float graph should have the same
+        # architecture to find the appropriate compare points for similarity computation).
+        similarity_baseline_graph = copy.deepcopy(tg)
+
+        graph_with_stats_correction = ptq_runner(tg,
+                                                 representative_data_gen,
+                                                 core_config,
+                                                 fw_info,
+                                                 fw_impl,
+                                                 tb_w)
 
         if core_config.debug_config.analyze_similarity:
+            quantized_graph = quantize_graph_weights(graph_with_stats_correction)
             analyzer_model_quantization(representative_data_gen,
                                         tb_w,
-                                        tg,
+                                        similarity_baseline_graph,
+                                        quantized_graph,
                                         fw_impl,
-                                        DEFAULT_PYTORCH_INFO)
+                                        fw_info)
 
-        return get_exportable_pytorch_model(tg)
+        exportable_model, user_info = get_exportable_pytorch_model(graph_with_stats_correction)
+        if target_platform_capabilities.tp_model.add_metadata:
+            exportable_model = add_metadata(exportable_model, get_versions_dict(target_platform_capabilities))
+        return exportable_model, user_info
 
 
 else:
     # If torch is not installed,
     # we raise an exception when trying to use these functions.
     def pytorch_post_training_quantization(*args, **kwargs):
         Logger.critical("PyTorch must be installed to use 'pytorch_post_training_quantization_experimental'. "
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/ptq/runner.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/ptq/runner.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/common/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/common/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/common/qat_config.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/common/qat_config.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantization_facade.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantizer/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantizer/quant_utils.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantization_facade.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantizer/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/constants.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/constants.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/immutable.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/immutable.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,15 +295,23 @@
 
         Returns:
             QuantizationConfigOptions with edited attributes names.
 
         """
         qc_options = copy.deepcopy(self)
 
-        for qc in qc_options.quantization_config_list:
+        # Extract the list of existing quantization configurations from qc_options
+
+        # Check if the base_config is already included in the quantization configuration list
+        # If not, add base_config to the list of configurations to update
+        cfgs_to_update = [cfg for cfg in qc_options.quantization_config_list]
+        if not any(qc_options.base_config is cfg for cfg in cfgs_to_update):
+            cfgs_to_update.append(qc_options.base_config)
+
+        for qc in cfgs_to_update:
             if layer_attrs_mapping is None:
                 qc.attr_weights_configs_mapping = {}
             else:
                 new_attr_mapping = {}
                 for attr in list(qc.attr_weights_configs_mapping.keys()):
                     new_key = layer_attrs_mapping.get(attr)
                     if new_key is None:
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,23 +56,26 @@
     Modeling of the hardware the quantized model will use during inference.
     The model contains definition of operators, quantization configurations of them, and
     fusing patterns so that multiple operators will be combined into a single operator.
     """
 
     def __init__(self,
                  default_qco: QuantizationConfigOptions,
+                 add_metadata: bool = False,
                  name="default_tp_model"):
         """
 
         Args:
             default_qco (QuantizationConfigOptions): Default QuantizationConfigOptions to use for operators that their QuantizationConfigOptions are not defined in the model.
+            add_metadata (bool): Whether to add metadata to the model or not.
             name (str): Name of the model.
         """
 
         super().__init__()
+        self.add_metadata = add_metadata
         self.name = name
         self.operator_set = []
         assert isinstance(default_qco, QuantizationConfigOptions)
         assert len(default_qco.quantization_config_list) == 1, \
             f'Default QuantizationConfigOptions must contain only one option'
         self.default_qco = default_qco
         self.fusing_patterns = []
@@ -187,15 +190,15 @@
 
         Assert model is valid.
         Model is invalid if, for example, it contains multiple operator sets with the same name,
         as their names should be unique.
 
         """
         opsets_names = [op.name for op in self.operator_set]
-        if (len(set(opsets_names)) != len(opsets_names)):
+        if len(set(opsets_names)) != len(opsets_names):
             Logger.critical(f'Operator Sets must have unique names.')
 
     def get_default_config(self) -> OpQuantizationConfig:
         """
 
         Returns:
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework.layer_filter_params import LayerFilterParams
 from model_compression_toolkit.target_platform_capabilities.immutable import ImmutableClass
 from model_compression_toolkit.target_platform_capabilities.target_platform.op_quantization_config import QuantizationConfigOptions, \
     OpQuantizationConfig
 from model_compression_toolkit.target_platform_capabilities.target_platform.operators import OperatorsSetBase
 from model_compression_toolkit.target_platform_capabilities.target_platform.target_platform_model import TargetPlatformModel
 from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework.current_tpc import _current_tpc
+from model_compression_toolkit.constants import MCT_VERSION, TPC_VERSION
 
 
 class TargetPlatformCapabilities(ImmutableClass):
     """
     Attach framework information to a modeled hardware.
     """
     def __init__(self,
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,36 +21,46 @@
 ###############################
 keras_tpc_models_dict = None
 if FOUND_TF:
     from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.latest import get_keras_tpc_latest
     from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v1.tpc_keras import get_keras_tpc as get_keras_tpc_v1
     from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v1_lut.tpc_keras import get_keras_tpc as get_keras_tpc_v1_lut
     from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v1_pot.tpc_keras import get_keras_tpc as get_keras_tpc_v1_pot
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v2.tpc_keras import get_keras_tpc as get_keras_tpc_v2
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v2_lut.tpc_keras import get_keras_tpc as get_keras_tpc_v2_lut
 
     # Keras: TPC versioning
     keras_tpc_models_dict = {'v1': get_keras_tpc_v1(),
                              'v1_lut': get_keras_tpc_v1_lut(),
                              'v1_pot': get_keras_tpc_v1_pot(),
+                             'v2': get_keras_tpc_v2(),
+                             'v2_lut': get_keras_tpc_v2_lut(),
                              LATEST: get_keras_tpc_latest()}
 
 ###############################
 # Build Pytorch TPC models
 ###############################
 pytorch_tpc_models_dict = None
 if FOUND_TORCH:
     from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.latest import get_pytorch_tpc_latest
     from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v1.tpc_pytorch import \
         get_pytorch_tpc as get_pytorch_tpc_v1
     from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v1_pot.tpc_pytorch import \
         get_pytorch_tpc as get_pytorch_tpc_v1_pot
-    from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v1_lut.tpc_pytorch import get_pytorch_tpc as get_pytorch_tpc_v1_lut
-
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v1_lut.tpc_pytorch import \
+        get_pytorch_tpc as get_pytorch_tpc_v1_lut
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v2.tpc_pytorch import \
+        get_pytorch_tpc as get_pytorch_tpc_v2
+    from model_compression_toolkit.target_platform_capabilities.tpc_models.imx500_tpc.v2_lut.tpc_pytorch import \
+        get_pytorch_tpc as get_pytorch_tpc_v2_lut
 
     # Pytorch: TPC versioning
     pytorch_tpc_models_dict = {'v1': get_pytorch_tpc_v1(),
                                'v1_lut': get_pytorch_tpc_v1_lut(),
                                'v1_pot': get_pytorch_tpc_v1_pot(),
+                               'v2': get_pytorch_tpc_v2(),
+                               'v2_lut': get_pytorch_tpc_v2_lut(),
                                LATEST: get_pytorch_tpc_latest()}
 
 tpc_dict = {TENSORFLOW: keras_tpc_models_dict,
             PYTORCH: pytorch_tpc_models_dict}
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     Returns: An OpQuantizationConfig config object and a list of OpQuantizationConfig objects.
 
     """
 
     # We define a default quantization config for all non-specified weights attributes.
     default_weight_attr_config = AttributeQuantizationConfig(
-        weights_quantization_method=tp.QuantizationMethod.SYMMETRIC,
+        weights_quantization_method=tp.QuantizationMethod.POWER_OF_TWO,
         weights_n_bits=8,
         weights_per_channel_threshold=False,
         enable_weights_quantization=False,
         lut_values_bitwidth=None)
 
     # We define a quantization config to quantize the kernel (for layers where there is a kernel attribute).
     kernel_base_config = AttributeQuantizationConfig(
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/common/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/common/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/common/constants.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/common/constants.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/keras/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,13 +78,10 @@
                 if quantizer_parameter.trainable and parameter_group == group:
                     quantizer_trainable.append(quantizer_parameter)
             return quantizer_trainable
 
 
 else:
     class BaseKerasTrainableQuantizer(BaseTrainableQuantizer):
-        def __init__(self,
-                     quantization_config: Union[TrainableQuantizerWeightsConfig, TrainableQuantizerActivationConfig]):
-
-            super().__init__(quantization_config)
+        def __init__(self, *args, **kwargs):
             Logger.critical("Tensorflow must be installed to use BaseKerasTrainableQuantizer. "
                             "The 'tensorflow' package is missing.")  # pragma: no cover
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/keras/load_model.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/keras/load_model.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py` & `model_compression_toolkit-2.1.0/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,13 +53,11 @@
                 quantizer_parameter, parameter_group = parameter_dict[VAR], parameter_dict[GROUP]
                 if quantizer_parameter.requires_grad and parameter_group == group:
                     quantizer_trainable.append(quantizer_parameter)
             return quantizer_trainable
 
 else:
     class BasePytorchTrainableQuantizer(BaseTrainableQuantizer):
-        def __init__(self,
-                     quantization_config: Union[TrainableQuantizerWeightsConfig, TrainableQuantizerActivationConfig]):
-            super().__init__(quantization_config)
+        def __init__(self, *args, **kwargs):
             Logger.critical("PyTorch must be installed to use 'BasePytorchTrainableQuantizer'. "
                             "The 'torch' package is missing.")  # pragma: no cover
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit.egg-info/PKG-INFO` & `model_compression_toolkit-2.1.0/model_compression_toolkit.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,60 @@
 Metadata-Version: 2.1
 Name: model-compression-toolkit
-Version: 2.0.0
+Version: 2.1.0
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
         
         This project provides researchers, developers, and engineers tools for optimizing and deploying state-of-the-art neural networks on efficient hardware.
         
         Specifically, this project aims to apply quantization to compress neural networks.
         
-        <img src="docsrc/images/mct_block_diagram.svg" width="10000">
+        <img src="https://github.com/sony/model_optimization/raw/main/docsrc/images/mct_block_diagram.svg" width="10000">
         
         MCT is developed by researchers and engineers working at Sony Semiconductor Israel.
         
         
         
         ## Table of Contents
         
-        - [Getting Started](#getting-started)
-        - [Supported features](#supported-features)
-        - [Results](#results)
-        - [Troubleshooting](#trouble-shooting)
-        - [Contributions](#contributions)
-        - [License](#license)
+        - [Getting Started](https://github.com/sony/model_optimization?tab=readme-ov-file#getting-started)
+        - [Supported features](https://github.com/sony/model_optimization?tab=readme-ov-file#supported-features)
+        - [Results](https://github.com/sony/model_optimization?tab=readme-ov-file#results)
+        - [Troubleshooting](https://github.com/sony/model_optimization?tab=readme-ov-file#trouble-shooting)
+        - [Contributions](https://github.com/sony/model_optimization?tab=readme-ov-file#contributions)
+        - [License](https://github.com/sony/model_optimization?tab=readme-ov-file#license)
         
         
         ## Getting Started
         
         This section provides an installation and a quick starting guide.
         
         ### Installation
         
         To install the latest stable release of MCT, run the following command:
         ```
         pip install model-compression-toolkit
         ```
         
-        For installing the nightly version or installing from source, refer to the [installation guide](INSTALLATION.md).
+        For installing the nightly version or installing from source, refer to the [installation guide](https://github.com/sony/model_optimization/blob/main/INSTALLATION.md).
         
         
         ### Quick start & tutorials 
         
         Explore the Model Compression Toolkit (MCT) through our tutorials, 
-        covering compression techniques for Keras and PyTorch models. Access interactive [notebooks](tutorials/README.md) 
+        covering compression techniques for Keras and PyTorch models. Access interactive [notebooks](https://github.com/sony/model_optimization/blob/main/tutorials/README.md) 
         for hands-on learning. For example:
-        * [Keras MobileNetV2 post training quantization](tutorials/notebooks/keras/ptq/example_keras_imagenet.ipynb)
-        * [Post training quantization with PyTorch](tutorials/notebooks/pytorch/ptq/example_pytorch_quantization_mnist.ipynb)
-        * [Data Generation for ResNet18 with PyTorch](tutorials/notebooks/pytorch/data_generation/example_pytorch_data_generation.ipynb).
-        
-        Additionally, for quick quantization of a variety of models from well-known collections,
-        visit the [quick-start page](tutorials/quick_start/README.md) and the
-        [results CSV](tutorials/quick_start/results/model_quantization_results.csv).
+        * [Keras MobileNetV2 post training quantization](https://github.com/sony/model_optimization/blob/main/tutorials/notebooks/imx500_notebooks/keras/example_keras_mobilenetv2_for_imx500.ipynb)
+        * [Post training quantization with PyTorch](https://github.com/sony/model_optimization/blob/main/tutorials/notebooks/mct_features_notebooks/pytorch/example_pytorch_ptq_mnist.ipynb)
+        * [Data Generation for ResNet18 with PyTorch](https://github.com/sony/model_optimization/blob/main/tutorials/notebooks/mct_features_notebooks/pytorch/example_pytorch_data_generation.ipynb).
+        
         
         ### Supported Versions
         
         Currently, MCT is being tested on various Python, Pytorch and TensorFlow versions:
         
         |             |  PyTorch 1.13                                                                                                                                                                                                               | PyTorch 2.0                                                                                                                                                                                                              | PyTorch 2.1                                                                                                                                                                                                              |
         |-------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
@@ -72,23 +69,23 @@
         | Python 3.10 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras212.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras213.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras214.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python310_keras215.yml) |
         | Python 3.11 | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras212.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras212.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras213.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras213.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras214.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras214.yml) | [![Run Tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras215.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_python311_keras215.yml) |
         
         
         ## Supported Features
         MCT offers a range of powerful features to optimize neural network models for efficient deployment. These supported features include:
         
-        ### Data Generation [*](#experimental-features)
+        ### Data Generation [*](https://github.com/sony/model_optimization?tab=readme-ov-file#experimental-features)
         MCT provides tools for generating synthetic images based on the statistics stored in a model's batch normalization layers. These generated images are valuable for various compression tasks where image data is required, such as quantization and pruning. 
-        You can customize data generation configurations to suit your specific needs. [Go to the Data Generation page.](model_compression_toolkit/data_generation/README.md)
+        You can customize data generation configurations to suit your specific needs. [Go to the Data Generation page.](https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/data_generation/README.md)
         
         ### Quantization
         MCT supports different quantization methods:
         * Post-training quantization (PTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_post_training_quantization.html), [PyTorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_post_training_quantization.html)
         * Gradient-based post-training quantization (GPTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_gradient_post_training_quantization.html), [PyTorch API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/pytorch_gradient_post_training_quantization.html)
-        * Quantization-aware training (QAT) [*](#experimental-features)
+        * Quantization-aware training (QAT) [*](https://github.com/sony/model_optimization?tab=readme-ov-file#experimental-features)
         
         
         | Quantization Method                           | Complexity | Computational Cost          |
         |-----------------------------------------------|------------|-----------------------------|
         | PTQ                                           | Low        | Low (order of minutes)      |
         | GPTQ (parameters fine-tuning using gradients) | Mild       | Mild (order of 2-3 hours)   |
         | QAT                                           | High       | High (order of 12-36 hours) |
@@ -102,28 +99,28 @@
         
         Main features:
         * <ins>Graph optimizations:</ins> Transforming the model to an equivalent (yet, more efficient) model (for example, batch-normalization layer folding to its preceding linear layer).
         * <ins>Quantization parameter search:</ins> Different methods can be used to minimize the expected added quantization-noise during thresholds search (by default, we use Mean-Square-Error, but other metrics can be used such as No-Clipping, Mean-Average-Error, and more).
         * <ins>Advanced quantization algorithms:</ins> To prevent a performance degradation some algorithms are applied such as: 
           * <ins>Shift negative correction:</ins> Symmetric activation quantization can hurt the model's performance when some layers output both negative and positive activations, but their range is asymmetric. For more details please visit [1].
           * <ins>Outliers filtering:</ins> Computing z-score for activation statistics to detect and remove outliers.
-        * <ins>Clustering:</ins> Using non-uniform quantization grid to quantize the weights and activations to match their distributions.[*](#experimental-features)
+        * <ins>Clustering:</ins> Using non-uniform quantization grid to quantize the weights and activations to match their distributions.[*](https://github.com/sony/model_optimization?tab=readme-ov-file#experimental-features)
         * <ins>Mixed-precision search:</ins> Assigning quantization bit-width per layer (for weights/activations), based on the layer's sensitivity to different bit-widths.
         * <ins>Visualization:</ins> You can use TensorBoard to observe useful information for troubleshooting the quantized model's performance (for example, the model in different phases of the quantization, collected statistics, similarity between layers of the float and quantized model and bit-width configuration for mixed-precision quantization). For more details, please read the [visualization documentation](https://sony.github.io/model_optimization/docs/guidelines/visualization.html).   
-        * <ins>Target Platform Capabilities:</ins> The Target Platform Capabilities (TPC) describes the target platform (an edge device with dedicated hardware). For more details, please read the [TPC README](model_compression_toolkit/target_platform_capabilities/README.md).   
+        * <ins>Target Platform Capabilities:</ins> The Target Platform Capabilities (TPC) describes the target platform (an edge device with dedicated hardware). For more details, please read the [TPC README](https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/target_platform_capabilities/README.md).   
         
         ### Enhanced Post-Training Quantization (EPTQ)
         As part of the GPTQ we provide an advanced optimization algorithm called EPTQ.
         
         The specifications of the algorithm are detailed in the paper: _"**EPTQ: Enhanced Post-Training Quantization via Label-Free Hessian**"_ [4].
         
-        More details on the how to use EPTQ via MCT can be found in the [EPTQ guidelines](model_compression_toolkit/gptq/README.md).
+        More details on the how to use EPTQ via MCT can be found in the [EPTQ guidelines](https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/gptq/README.md).
         
         
-        ### Structured Pruning [*](#experimental-features)
+        ### Structured Pruning [*](https://github.com/sony/model_optimization?tab=readme-ov-file#experimental-features)
         MCT introduces a structured and hardware-aware model pruning.
         This pruning technique is designed to compress models for specific hardware architectures, 
         taking into account the target platform's Single Instruction, Multiple Data (SIMD) capabilities. 
         By pruning groups of channels (SIMD groups), our approach not only reduces model size 
         and complexity, but ensures that better utilization of channels is in line with the SIMD architecture 
         for a target Resource Utilization of weights memory footprint.
         [Keras API](https://sony.github.io/model_optimization/docs/api/api_docs/methods/keras_pruning_experimental.html)
@@ -137,30 +134,28 @@
         
         
         ## Results
         ### Keras
         Graph of [MobileNetV2](https://keras.io/api/applications/mobilenet/) accuracy on ImageNet vs average bit-width of weights, using 
         single-precision quantization, mixed-precision quantization, and mixed-precision quantization with GPTQ.
         
-        <img src="docsrc/images/mbv2_accuracy_graph.png">
+        <img src="https://github.com/sony/model_optimization/raw/main/docsrc/images/mbv2_accuracy_graph.png">
         
         For more results, please see [1]
         
         ### Pytorch
         We quantized classification networks from the torchvision library. 
         In the following table we present the ImageNet validation results for these models:
         
         | Network Name              | Float Accuracy  | 8Bit Accuracy   | Data-Free 8Bit Accuracy |
         |---------------------------|-----------------|-----------------|-------------------------|
         | MobileNet V2 [3]          | 71.886          | 71.444          |71.29|
         | ResNet-18 [3]             | 69.86           | 69.63           |69.53|
         | SqueezeNet 1.1 [3]        | 58.128          | 57.678          ||
         
-        For more results, please refer to [quick start](https://github.com/sony/model_optimization/tree/main/tutorials/quick_start).
-        
         
         #### Pruning Results
         
         Results for applying pruning to reduce the parameters of the following models by 50%:
         
         | Model           | Dense Model Accuracy | Pruned Model Accuracy |
         |-----------------|----------------------|-----------------------|
@@ -175,19 +170,19 @@
         
         Check out the [FAQ](https://github.com/sony/model_optimization/tree/main/FAQ.md) for common issues.
         
         
         ## Contributions
         MCT aims at keeping a more up-to-date fork and welcomes contributions from anyone.
         
-        *You will find more information about contributions in the [Contribution guide](CONTRIBUTING.md).
+        *You will find more information about contributions in the [Contribution guide](https://github.com/sony/model_optimization/blob/main/CONTRIBUTING.md).
         
         
         ## License
-        [Apache License 2.0](LICENSE.md).
+        [Apache License 2.0](https://github.com/sony/model_optimization/blob/main/LICENSE.md).
         
         ## References 
         
         [1] Habi, H.V., Peretz, R., Cohen, E., Dikstein, L., Dror, O., Diamant, I., Jennings, R.H. and Netzer, A., 2021. [HPTQ: Hardware-Friendly Post Training Quantization. arXiv preprint](https://arxiv.org/abs/2109.09113).
         
         [2] [Keras Applications](https://keras.io/api/applications/)
```

### Comparing `model_compression_toolkit-2.0.0/model_compression_toolkit.egg-info/SOURCES.txt` & `model_compression_toolkit-2.1.0/model_compression_toolkit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 README.md
 setup.cfg
 setup.py
 model_compression_toolkit/__init__.py
 model_compression_toolkit/constants.py
 model_compression_toolkit/defaultdict.py
 model_compression_toolkit/logger.py
+model_compression_toolkit/metadata.py
 model_compression_toolkit.egg-info/PKG-INFO
 model_compression_toolkit.egg-info/SOURCES.txt
 model_compression_toolkit.egg-info/dependency_links.txt
 model_compression_toolkit.egg-info/requires.txt
 model_compression_toolkit.egg-info/top_level.txt
 model_compression_toolkit/core/__init__.py
 model_compression_toolkit/core/analyzer.py
-model_compression_toolkit/core/exporter.py
 model_compression_toolkit/core/graph_prep_runner.py
 model_compression_toolkit/core/quantization_prep_runner.py
 model_compression_toolkit/core/runner.py
 model_compression_toolkit/core/common/__init__.py
 model_compression_toolkit/core/common/base_substitutions.py
 model_compression_toolkit/core/common/framework_implementation.py
 model_compression_toolkit/core/common/framework_info.py
@@ -140,14 +140,15 @@
 model_compression_toolkit/core/common/substitutions/__init__.py
 model_compression_toolkit/core/common/substitutions/apply_substitutions.py
 model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
 model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
 model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
 model_compression_toolkit/core/common/substitutions/linear_collapsing.py
 model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
+model_compression_toolkit/core/common/substitutions/remove_identity.py
 model_compression_toolkit/core/common/substitutions/residual_collapsing.py
 model_compression_toolkit/core/common/substitutions/scale_equalization.py
 model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
 model_compression_toolkit/core/common/substitutions/softmax_shift.py
 model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
 model_compression_toolkit/core/common/substitutions/weights_activation_split.py
 model_compression_toolkit/core/common/visualization/__init__.py
@@ -172,21 +173,22 @@
 model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
 model_compression_toolkit/core/keras/graph_substitutions/__init__.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
+model_compression_toolkit/core/keras/graph_substitutions/substitutions/concat_threshold_update.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
-model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py
+model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_identity.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
 model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
@@ -235,21 +237,23 @@
 model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
 model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
 model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
+model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/concat_threshold_update.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/remove_identity.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
 model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
@@ -446,14 +450,22 @@
 model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py
 model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py
 model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py
 model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py
 model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py
 model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py
 model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/__init__.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tp_model.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_keras.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_pytorch.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/__init__.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tp_model.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_keras.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_pytorch.py
 model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
 model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
 model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
 model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
 model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
 model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
 model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
```

### Comparing `model_compression_toolkit-2.0.0/setup.py` & `model_compression_toolkit-2.1.0/setup.py`

 * *Files identical despite different names*

