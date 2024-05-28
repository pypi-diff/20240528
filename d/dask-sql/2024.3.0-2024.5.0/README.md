# Comparing `tmp/dask_sql-2024.3.0.tar.gz` & `tmp/dask_sql-2024.5.0.tar.gz`

## Comparing `dask_sql-2024.3.0.tar` & `dask_sql-2024.5.0.tar`

### file list

```diff
@@ -1,144 +1,144 @@
--rw-r--r--   0        0        0      773 1970-01-01 00:00:00.000000 dask_sql-2024.3.0/Cargo.toml
--rw-r--r--   0     1001      127     1067 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/LICENSE.txt
--rw-r--r--   0     1001      127     7970 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/README.md
--rw-r--r--   0     1001      127      472 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/__init__.py
--rw-r--r--   0     1001      127      479 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/_compat.py
--rw-r--r--   0     1001      127     9016 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/cmd.py
--rw-r--r--   0     1001      127      235 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/config.py
--rw-r--r--   0     1001      127    38110 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/context.py
--rw-r--r--   0     1001      127     9492 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/datacontainer.py
--rw-r--r--   0     1001      127      493 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/input_utils/__init__.py
--rw-r--r--   0     1001      127      312 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/input_utils/base.py
--rw-r--r--   0     1001      127     2671 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/input_utils/convert.py
--rw-r--r--   0     1001      127      982 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/input_utils/dask.py
--rw-r--r--   0     1001      127    12080 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/input_utils/hive.py
--rw-r--r--   0     1001      127     1080 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/input_utils/intake.py
--rw-r--r--   0     1001      127     1773 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/input_utils/location.py
--rw-r--r--   0     1001      127     1146 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/input_utils/pandaslike.py
--rw-r--r--   0     1001      127     1222 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/input_utils/sqlalchemy.py
--rw-r--r--   0     1001      127        0 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/integrations/__init__.py
--rw-r--r--   0     1001      127     5097 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/integrations/fugue.py
--rw-r--r--   0     1001      127     4577 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/integrations/ipython.py
--rw-r--r--   0     1001      127    12822 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/mappings.py
--rw-r--r--   0     1001      127        0 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/__init__.py
--rw-r--r--   0     1001      127       34 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/__init__.py
--rw-r--r--   0     1001      127     4400 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/base.py
--rw-r--r--   0     1001      127     2271 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/convert.py
--rw-r--r--   0     1001      127     1367 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/custom/__init__.py
--rw-r--r--   0     1001      127     2645 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/custom/alter.py
--rw-r--r--   0     1001      127     2304 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/custom/analyze_table.py
--rw-r--r--   0     1001      127     1180 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/custom/create_catalog_schema.py
--rw-r--r--   0     1001      127     9488 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/custom/create_experiment.py
--rw-r--r--   0     1001      127     2613 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/custom/create_memory_table.py
--rw-r--r--   0     1001      127     8644 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/custom/create_model.py
--rw-r--r--   0     1001      127     2433 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/custom/create_table.py
--rw-r--r--   0     1001      127     1425 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/custom/describe_model.py
--rw-r--r--   0     1001      127     1336 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/custom/distributeby.py
--rw-r--r--   0     1001      127     1039 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/custom/drop_model.py
--rw-r--r--   0     1001      127      887 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/custom/drop_schema.py
--rw-r--r--   0     1001      127     1448 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/custom/drop_table.py
--rw-r--r--   0     1001      127     3950 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/custom/export_model.py
--rw-r--r--   0     1001      127     6504 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/custom/metrics.py
--rw-r--r--   0     1001      127     3535 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/custom/predict_model.py
--rw-r--r--   0     1001      127     1470 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/custom/show_columns.py
--rw-r--r--   0     1001      127      920 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/custom/show_models.py
--rw-r--r--   0     1001      127     1513 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/custom/show_schemas.py
--rw-r--r--   0     1001      127     1532 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/custom/show_tables.py
--rw-r--r--   0     1001      127      909 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/custom/use_schema.py
--rw-r--r--   0     1001      127    28012 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/custom/wrappers.py
--rw-r--r--   0     1001      127      916 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/logical/__init__.py
--rw-r--r--   0     1001      127    22811 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/logical/aggregate.py
--rw-r--r--   0     1001      127     1738 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/logical/cross_join.py
--rw-r--r--   0     1001      127     1116 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/logical/empty.py
--rw-r--r--   0     1001      127      501 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/logical/explain.py
--rw-r--r--   0     1001      127     2234 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/logical/filter.py
--rw-r--r--   0     1001      127    14225 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/logical/join.py
--rw-r--r--   0     1001      127     4183 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/logical/limit.py
--rw-r--r--   0     1001      127     2595 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/logical/project.py
--rw-r--r--   0     1001      127     2114 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/logical/sample.py
--rw-r--r--   0     1001      127     1316 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/logical/sort.py
--rw-r--r--   0     1001      127      955 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/logical/subquery_alias.py
--rw-r--r--   0     1001      127     4113 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/logical/table_scan.py
--rw-r--r--   0     1001      127     1995 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/logical/union.py
--rw-r--r--   0     1001      127     2191 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/logical/values.py
--rw-r--r--   0     1001      127    15665 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rel/logical/window.py
--rw-r--r--   0     1001      127       34 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rex/__init__.py
--rw-r--r--   0     1001      127      812 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rex/base.py
--rw-r--r--   0     1001      127     2417 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rex/convert.py
--rw-r--r--   0     1001      127      319 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rex/core/__init__.py
--rw-r--r--   0     1001      127     1158 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rex/core/alias.py
--rw-r--r--   0     1001      127    39379 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rex/core/call.py
--rw-r--r--   0     1001      127      940 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rex/core/input_ref.py
--rw-r--r--   0     1001      127     7835 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rex/core/literal.py
--rw-r--r--   0     1001      127      993 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/rex/core/subquery.py
--rw-r--r--   0     1001      127        0 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/utils/__init__.py
--rw-r--r--   0     1001      127    20439 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/utils/filter.py
--rw-r--r--   0     1001      127     1196 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/utils/groupby.py
--rw-r--r--   0     1001      127     6509 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/utils/ml_classes.py
--rw-r--r--   0     1001      127     4155 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/utils/sort.py
--rw-r--r--   0     1001      127     7334 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/physical/utils/statistics.py
--rw-r--r--   0     1001      127        0 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/server/__init__.py
--rw-r--r--   0     1001      127     8811 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/server/app.py
--rw-r--r--   0     1001      127     4983 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/server/presto_jdbc.py
--rw-r--r--   0     1001      127     4195 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/server/responses.py
--rw-r--r--   0     1001      127     4819 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/sql-schema.yaml
--rw-r--r--   0     1001      127      476 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/sql.yaml
--rw-r--r--   0     1001      127     5834 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/dask_sql/utils.py
--rw-r--r--   0     1001      127    10523 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/dialect.rs
--rw-r--r--   0     1001      127     1617 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/error.rs
--rw-r--r--   0     1001      127    39061 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/expression.rs
--rw-r--r--   0     1001      127     1373 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/lib.rs
--rw-r--r--   0     1001      127    56283 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/parser.rs
--rw-r--r--   0     1001      127      736 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/column.rs
--rw-r--r--   0     1001      127      871 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/exceptions.rs
--rw-r--r--   0     1001      127     1086 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/function.rs
--rw-r--r--   0     1001      127     4164 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/aggregate.rs
--rw-r--r--   0     1001      127     3614 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/alter_schema.rs
--rw-r--r--   0     1001      127     4055 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/alter_table.rs
--rw-r--r--   0     1001      127     3811 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/analyze_table.rs
--rw-r--r--   0     1001      127     3859 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/create_catalog_schema.rs
--rw-r--r--   0     1001      127     4875 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/create_experiment.rs
--rw-r--r--   0     1001      127     3449 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/create_memory_table.rs
--rw-r--r--   0     1001      127     4653 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/create_model.rs
--rw-r--r--   0     1001      127     4242 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/create_table.rs
--rw-r--r--   0     1001      127     3469 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/describe_model.rs
--rw-r--r--   0     1001      127     3545 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/drop_model.rs
--rw-r--r--   0     1001      127     3229 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/drop_schema.rs
--rw-r--r--   0     1001      127      956 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/drop_table.rs
--rw-r--r--   0     1001      127     1169 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/empty_relation.rs
--rw-r--r--   0     1001      127      978 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/explain.rs
--rw-r--r--   0     1001      127     3772 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/export_model.rs
--rw-r--r--   0     1001      127      947 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/filter.rs
--rw-r--r--   0     1001      127     4400 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/join.rs
--rw-r--r--   0     1001      127     1282 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/limit.rs
--rw-r--r--   0     1001      127     3605 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/predict_model.rs
--rw-r--r--   0     1001      127     2292 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/projection.rs
--rw-r--r--   0     1001      127     1993 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/repartition_by.rs
--rw-r--r--   0     1001      127     3473 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/show_columns.rs
--rw-r--r--   0     1001      127     2942 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/show_models.rs
--rw-r--r--   0     1001      127     3382 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/show_schemas.rs
--rw-r--r--   0     1001      127     3467 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/show_tables.rs
--rw-r--r--   0     1001      127      965 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/sort.rs
--rw-r--r--   0     1001      127      871 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/subquery_alias.rs
--rw-r--r--   0     1001      127    10164 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/table_scan.rs
--rw-r--r--   0     1001      127     2983 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/use_schema.rs
--rw-r--r--   0     1001      127     6593 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical/window.rs
--rw-r--r--   0     1001      127    17390 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/logical.rs
--rw-r--r--   0     1001      127     7374 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/optimizer/decorrelate_where_exists.rs
--rw-r--r--   0     1001      127     9067 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/optimizer/decorrelate_where_in.rs
--rw-r--r--   0     1001      127    44591 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/optimizer/dynamic_partition_pruning.rs
--rw-r--r--   0     1001      127    13899 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/optimizer/join_reorder.rs
--rw-r--r--   0     1001      127    16250 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/optimizer/utils.rs
--rw-r--r--   0     1001      127     9656 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/optimizer.rs
--rw-r--r--   0     1001      127      755 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/parser_utils.rs
--rw-r--r--   0     1001      127     8568 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/preoptimizer.rs
--rw-r--r--   0     1001      127     1501 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/schema.rs
--rw-r--r--   0     1001      127      587 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/statement.rs
--rw-r--r--   0     1001      127     9700 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/table.rs
--rw-r--r--   0     1001      127     3669 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/types/rel_data_type.rs
--rw-r--r--   0     1001      127     3693 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/types/rel_data_type_field.rs
--rw-r--r--   0     1001      127    17181 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql/types.rs
--rw-r--r--   0     1001      127    36405 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/src/sql.rs
--rw-r--r--   0     1001      127    82505 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/Cargo.lock
--rw-r--r--   0     1001      127     2991 2024-03-19 16:40:50.000000 dask_sql-2024.3.0/pyproject.toml
--rw-r--r--   0        0        0    10111 1970-01-01 00:00:00.000000 dask_sql-2024.3.0/PKG-INFO
+-rw-r--r--   0        0        0      773 1970-01-01 00:00:00.000000 dask_sql-2024.5.0/Cargo.toml
+-rw-r--r--   0     1001      127     1067 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/LICENSE.txt
+-rw-r--r--   0     1001      127     7970 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/README.md
+-rw-r--r--   0     1001      127      627 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/__init__.py
+-rw-r--r--   0     1001      127      279 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/_compat.py
+-rw-r--r--   0     1001      127     9016 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/cmd.py
+-rw-r--r--   0     1001      127      235 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/config.py
+-rw-r--r--   0     1001      127    38495 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/context.py
+-rw-r--r--   0     1001      127     9492 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/datacontainer.py
+-rw-r--r--   0     1001      127      493 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/input_utils/__init__.py
+-rw-r--r--   0     1001      127      312 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/input_utils/base.py
+-rw-r--r--   0     1001      127     2671 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/input_utils/convert.py
+-rw-r--r--   0     1001      127      910 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/input_utils/dask.py
+-rw-r--r--   0     1001      127    12080 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/input_utils/hive.py
+-rw-r--r--   0     1001      127     1080 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/input_utils/intake.py
+-rw-r--r--   0     1001      127     1773 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/input_utils/location.py
+-rw-r--r--   0     1001      127     1146 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/input_utils/pandaslike.py
+-rw-r--r--   0     1001      127     1222 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/input_utils/sqlalchemy.py
+-rw-r--r--   0     1001      127        0 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/integrations/__init__.py
+-rw-r--r--   0     1001      127     5097 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/integrations/fugue.py
+-rw-r--r--   0     1001      127     4577 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/integrations/ipython.py
+-rw-r--r--   0     1001      127    12822 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/mappings.py
+-rw-r--r--   0     1001      127        0 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/__init__.py
+-rw-r--r--   0     1001      127       34 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/__init__.py
+-rw-r--r--   0     1001      127     4400 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/base.py
+-rw-r--r--   0     1001      127     2271 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/convert.py
+-rw-r--r--   0     1001      127     1367 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/custom/__init__.py
+-rw-r--r--   0     1001      127     2645 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/custom/alter.py
+-rw-r--r--   0     1001      127     2304 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/custom/analyze_table.py
+-rw-r--r--   0     1001      127     1180 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/custom/create_catalog_schema.py
+-rw-r--r--   0     1001      127     9488 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/custom/create_experiment.py
+-rw-r--r--   0     1001      127     2613 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/custom/create_memory_table.py
+-rw-r--r--   0     1001      127     8644 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/custom/create_model.py
+-rw-r--r--   0     1001      127     2433 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/custom/create_table.py
+-rw-r--r--   0     1001      127     1425 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/custom/describe_model.py
+-rw-r--r--   0     1001      127     1336 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/custom/distributeby.py
+-rw-r--r--   0     1001      127     1039 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/custom/drop_model.py
+-rw-r--r--   0     1001      127      887 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/custom/drop_schema.py
+-rw-r--r--   0     1001      127     1448 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/custom/drop_table.py
+-rw-r--r--   0     1001      127     3950 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/custom/export_model.py
+-rw-r--r--   0     1001      127     6504 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/custom/metrics.py
+-rw-r--r--   0     1001      127     3535 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/custom/predict_model.py
+-rw-r--r--   0     1001      127     1470 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/custom/show_columns.py
+-rw-r--r--   0     1001      127      920 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/custom/show_models.py
+-rw-r--r--   0     1001      127     1513 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/custom/show_schemas.py
+-rw-r--r--   0     1001      127     1532 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/custom/show_tables.py
+-rw-r--r--   0     1001      127      909 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/custom/use_schema.py
+-rw-r--r--   0     1001      127    28021 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/custom/wrappers.py
+-rw-r--r--   0     1001      127      916 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/logical/__init__.py
+-rw-r--r--   0     1001      127    22811 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/logical/aggregate.py
+-rw-r--r--   0     1001      127     1738 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/logical/cross_join.py
+-rw-r--r--   0     1001      127     1116 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/logical/empty.py
+-rw-r--r--   0     1001      127      501 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/logical/explain.py
+-rw-r--r--   0     1001      127     2326 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/logical/filter.py
+-rw-r--r--   0     1001      127    12659 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/logical/join.py
+-rw-r--r--   0     1001      127     4418 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/logical/limit.py
+-rw-r--r--   0     1001      127     2595 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/logical/project.py
+-rw-r--r--   0     1001      127     2114 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/logical/sample.py
+-rw-r--r--   0     1001      127     1316 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/logical/sort.py
+-rw-r--r--   0     1001      127      955 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/logical/subquery_alias.py
+-rw-r--r--   0     1001      127     4213 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/logical/table_scan.py
+-rw-r--r--   0     1001      127     1995 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/logical/union.py
+-rw-r--r--   0     1001      127     2191 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/logical/values.py
+-rw-r--r--   0     1001      127    15173 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rel/logical/window.py
+-rw-r--r--   0     1001      127       34 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rex/__init__.py
+-rw-r--r--   0     1001      127      812 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rex/base.py
+-rw-r--r--   0     1001      127     2417 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rex/convert.py
+-rw-r--r--   0     1001      127      319 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rex/core/__init__.py
+-rw-r--r--   0     1001      127     1158 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rex/core/alias.py
+-rw-r--r--   0     1001      127    39047 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rex/core/call.py
+-rw-r--r--   0     1001      127      940 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rex/core/input_ref.py
+-rw-r--r--   0     1001      127     7835 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rex/core/literal.py
+-rw-r--r--   0     1001      127      993 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/rex/core/subquery.py
+-rw-r--r--   0     1001      127        0 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/utils/__init__.py
+-rw-r--r--   0     1001      127    20460 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/utils/filter.py
+-rw-r--r--   0     1001      127     1196 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/utils/groupby.py
+-rw-r--r--   0     1001      127     6509 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/utils/ml_classes.py
+-rw-r--r--   0     1001      127     4155 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/utils/sort.py
+-rw-r--r--   0     1001      127     7334 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/physical/utils/statistics.py
+-rw-r--r--   0     1001      127        0 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/server/__init__.py
+-rw-r--r--   0     1001      127     8811 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/server/app.py
+-rw-r--r--   0     1001      127     4983 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/server/presto_jdbc.py
+-rw-r--r--   0     1001      127     4195 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/server/responses.py
+-rw-r--r--   0     1001      127     4819 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/sql-schema.yaml
+-rw-r--r--   0     1001      127      476 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/sql.yaml
+-rw-r--r--   0     1001      127     5834 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/dask_sql/utils.py
+-rw-r--r--   0     1001      127    10523 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/dialect.rs
+-rw-r--r--   0     1001      127     1617 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/error.rs
+-rw-r--r--   0     1001      127    39061 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/expression.rs
+-rw-r--r--   0     1001      127     1373 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/lib.rs
+-rw-r--r--   0     1001      127    56283 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/parser.rs
+-rw-r--r--   0     1001      127      736 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/column.rs
+-rw-r--r--   0     1001      127      871 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/exceptions.rs
+-rw-r--r--   0     1001      127     1086 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/function.rs
+-rw-r--r--   0     1001      127     4164 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/aggregate.rs
+-rw-r--r--   0     1001      127     3614 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/alter_schema.rs
+-rw-r--r--   0     1001      127     4055 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/alter_table.rs
+-rw-r--r--   0     1001      127     3811 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/analyze_table.rs
+-rw-r--r--   0     1001      127     3859 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/create_catalog_schema.rs
+-rw-r--r--   0     1001      127     4875 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/create_experiment.rs
+-rw-r--r--   0     1001      127     3449 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/create_memory_table.rs
+-rw-r--r--   0     1001      127     4653 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/create_model.rs
+-rw-r--r--   0     1001      127     4242 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/create_table.rs
+-rw-r--r--   0     1001      127     3469 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/describe_model.rs
+-rw-r--r--   0     1001      127     3545 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/drop_model.rs
+-rw-r--r--   0     1001      127     3229 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/drop_schema.rs
+-rw-r--r--   0     1001      127      956 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/drop_table.rs
+-rw-r--r--   0     1001      127     1169 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/empty_relation.rs
+-rw-r--r--   0     1001      127      978 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/explain.rs
+-rw-r--r--   0     1001      127     3772 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/export_model.rs
+-rw-r--r--   0     1001      127      947 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/filter.rs
+-rw-r--r--   0     1001      127     4400 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/join.rs
+-rw-r--r--   0     1001      127     1282 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/limit.rs
+-rw-r--r--   0     1001      127     3605 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/predict_model.rs
+-rw-r--r--   0     1001      127     2292 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/projection.rs
+-rw-r--r--   0     1001      127     1993 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/repartition_by.rs
+-rw-r--r--   0     1001      127     3473 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/show_columns.rs
+-rw-r--r--   0     1001      127     2942 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/show_models.rs
+-rw-r--r--   0     1001      127     3382 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/show_schemas.rs
+-rw-r--r--   0     1001      127     3467 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/show_tables.rs
+-rw-r--r--   0     1001      127      965 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/sort.rs
+-rw-r--r--   0     1001      127      871 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/subquery_alias.rs
+-rw-r--r--   0     1001      127    10164 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/table_scan.rs
+-rw-r--r--   0     1001      127     2983 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/use_schema.rs
+-rw-r--r--   0     1001      127     6593 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical/window.rs
+-rw-r--r--   0     1001      127    17390 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/logical.rs
+-rw-r--r--   0     1001      127     7374 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/optimizer/decorrelate_where_exists.rs
+-rw-r--r--   0     1001      127     9067 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/optimizer/decorrelate_where_in.rs
+-rw-r--r--   0     1001      127    44591 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/optimizer/dynamic_partition_pruning.rs
+-rw-r--r--   0     1001      127    13899 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/optimizer/join_reorder.rs
+-rw-r--r--   0     1001      127    16250 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/optimizer/utils.rs
+-rw-r--r--   0     1001      127     9656 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/optimizer.rs
+-rw-r--r--   0     1001      127      755 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/parser_utils.rs
+-rw-r--r--   0     1001      127     8568 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/preoptimizer.rs
+-rw-r--r--   0     1001      127     1501 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/schema.rs
+-rw-r--r--   0     1001      127      587 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/statement.rs
+-rw-r--r--   0     1001      127     9700 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/table.rs
+-rw-r--r--   0     1001      127     3669 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/types/rel_data_type.rs
+-rw-r--r--   0     1001      127     3693 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/types/rel_data_type_field.rs
+-rw-r--r--   0     1001      127    17181 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql/types.rs
+-rw-r--r--   0     1001      127    36405 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/src/sql.rs
+-rw-r--r--   0     1001      127    82505 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/Cargo.lock
+-rw-r--r--   0     1001      127     3084 2024-05-28 14:08:38.000000 dask_sql-2024.5.0/pyproject.toml
+-rw-r--r--   0        0        0    10111 1970-01-01 00:00:00.000000 dask_sql-2024.5.0/PKG-INFO
```

### Comparing `dask_sql-2024.3.0/Cargo.toml` & `dask_sql-2024.5.0/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "dask-sql"
 repository = "https://github.com/dask-contrib/dask-sql"
-version = "2024.3.0"
+version = "2024.5.0"
 description = "Bindings for DataFusion used by Dask-SQL"
 readme = "README.md"
 license = "Apache-2.0"
 edition = "2021"
 rust-version = "1.72"
 include = ["/src", "/dask_sql", "/LICENSE.txt", "pyproject.toml", "Cargo.toml", "Cargo.lock"]
```

### Comparing `dask_sql-2024.3.0/LICENSE.txt` & `dask_sql-2024.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/README.md` & `dask_sql-2024.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/cmd.py` & `dask_sql-2024.5.0/dask_sql/cmd.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/context.py` & `dask_sql-2024.5.0/dask_sql/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,23 +258,31 @@
         )
 
         if type(input_table) == str:
             dc.filepath = input_table
             self.schema[schema_name].filepaths[table_name.lower()] = input_table
         elif hasattr(input_table, "dask") and dd.utils.is_dataframe_like(input_table):
             try:
-                dask_filepath = hlg_layer(
-                    input_table.dask, "read-parquet"
-                ).creation_info["args"][0]
+                if dd._dask_expr_enabled():
+                    from dask_expr.io.parquet import ReadParquet
+
+                    dask_filepath = None
+                    operations = input_table.find_operations(ReadParquet)
+                    for op in operations:
+                        dask_filepath = op._args[0]
+                else:
+                    dask_filepath = hlg_layer(
+                        input_table.dask, "read-parquet"
+                    ).creation_info["args"][0]
                 dc.filepath = dask_filepath
                 self.schema[schema_name].filepaths[table_name.lower()] = dask_filepath
             except KeyError:
                 logger.debug("Expected 'read-parquet' layer")
 
-        if parquet_statistics and not statistics:
+        if parquet_statistics and not dd._dask_expr_enabled() and not statistics:
             statistics = parquet_statistics(dc.df)
             if statistics:
                 row_count = 0
                 for d in statistics:
                     row_count += d["num-rows"]
                 statistics = Statistics(row_count)
         if not statistics:
```

### Comparing `dask_sql-2024.3.0/dask_sql/datacontainer.py` & `dask_sql-2024.5.0/dask_sql/datacontainer.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/input_utils/convert.py` & `dask_sql-2024.5.0/dask_sql/input_utils/convert.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/input_utils/dask.py` & `dask_sql-2024.5.0/dask_sql/input_utils/dask.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,14 @@
         table_name: str,
         format: str = None,
         gpu: bool = False,
         **kwargs
     ):
         if gpu:  # pragma: no cover
             try:
-                import dask_cudf
+                import dask_cudf  # noqa: F401
             except ImportError:
                 raise ModuleNotFoundError(
                     "Setting `gpu=True` for table creation requires dask_cudf"
                 )
-            if not isinstance(input_item, dask_cudf.DataFrame):
-                input_item = dask_cudf.from_dask_dataframe(input_item, **kwargs)
+            return input_item.to_backend("cudf", **kwargs)
         return input_item
```

### Comparing `dask_sql-2024.3.0/dask_sql/input_utils/hive.py` & `dask_sql-2024.5.0/dask_sql/input_utils/hive.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/input_utils/intake.py` & `dask_sql-2024.5.0/dask_sql/input_utils/intake.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/input_utils/location.py` & `dask_sql-2024.5.0/dask_sql/input_utils/location.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/input_utils/pandaslike.py` & `dask_sql-2024.5.0/dask_sql/input_utils/pandaslike.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/input_utils/sqlalchemy.py` & `dask_sql-2024.5.0/dask_sql/input_utils/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/integrations/fugue.py` & `dask_sql-2024.5.0/dask_sql/integrations/fugue.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/integrations/ipython.py` & `dask_sql-2024.5.0/dask_sql/integrations/ipython.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/mappings.py` & `dask_sql-2024.5.0/dask_sql/mappings.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/base.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/base.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/convert.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/convert.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/custom/__init__.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/custom/alter.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/custom/alter.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/custom/analyze_table.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/custom/analyze_table.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/custom/create_catalog_schema.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/custom/create_catalog_schema.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/custom/create_experiment.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/custom/create_experiment.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/custom/create_memory_table.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/custom/create_memory_table.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/custom/create_model.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/custom/create_model.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/custom/create_table.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/custom/create_table.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/custom/describe_model.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/custom/describe_model.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/custom/distributeby.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/custom/distributeby.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/custom/drop_model.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/custom/drop_model.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/custom/drop_schema.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/custom/drop_schema.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/custom/drop_table.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/custom/drop_table.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/custom/export_model.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/custom/export_model.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/custom/metrics.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/custom/metrics.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/custom/predict_model.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/custom/predict_model.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/custom/show_columns.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/custom/show_columns.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/custom/show_models.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/custom/show_models.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/custom/show_schemas.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/custom/show_schemas.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/custom/show_tables.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/custom/show_tables.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/custom/use_schema.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/custom/use_schema.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/custom/wrappers.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/custom/wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,15 +203,15 @@
                     X,
                 )
             return X.map_blocks(
                 _transform,
                 estimator=self._postfit_estimator,
                 meta=output_meta,
             )
-        elif isinstance(X, dd._Frame):
+        elif isinstance(X, dd.DataFrame):
             if output_meta is None:
                 output_meta = _transform(X._meta_nonempty, self._postfit_estimator)
             try:
                 return X.map_partitions(
                     _transform,
                     self._postfit_estimator,
                     output_meta,
@@ -301,15 +301,15 @@
                 _predict,
                 estimator=self._postfit_estimator,
                 drop_axis=1,
                 meta=output_meta,
             )
             return result
 
-        elif isinstance(X, dd._Frame):
+        elif isinstance(X, dd.DataFrame):
             if output_meta is None:
                 # dask-dataframe relies on dd.core.no_default
                 # for infering meta
                 output_meta = _predict(X._meta_nonempty, self._postfit_estimator)
             try:
                 return X.map_partitions(
                     _predict,
@@ -360,15 +360,15 @@
             # XXX: multiclass
             return X.map_blocks(
                 _predict_proba,
                 estimator=self._postfit_estimator,
                 meta=output_meta,
                 chunks=(X.chunks[0], len(self._postfit_estimator.classes_)),
             )
-        elif isinstance(X, dd._Frame):
+        elif isinstance(X, dd.DataFrame):
             if output_meta is None:
                 # dask-dataframe relies on dd.core.no_default
                 # for infering meta
                 output_meta = _predict_proba(X._meta_nonempty, self._postfit_estimator)
             try:
                 return X.map_partitions(
                     _predict_proba,
```

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/logical/__init__.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/logical/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/logical/aggregate.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/logical/aggregate.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/logical/cross_join.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/logical/cross_join.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/logical/empty.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/logical/empty.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/logical/filter.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/logical/filter.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,15 +34,16 @@
             return df.head(0, compute=False)
         else:
             return df
 
     # In SQL, a NULL in a boolean is False on filtering
     filter_condition = filter_condition.fillna(False)
     out = df[filter_condition]
-    if dask_config.get("sql.predicate_pushdown"):
+    # dask-expr should implicitly handle predicate pushdown
+    if dask_config.get("sql.predicate_pushdown") and not dd._dask_expr_enabled():
         return attempt_predicate_pushdown(out, add_filters=add_filters)
     else:
         return out
 
 
 class DaskFilterPlugin(BaseRelPlugin):
     """
```

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/logical/join.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/logical/join.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 import operator
 import warnings
 from functools import reduce
 from typing import TYPE_CHECKING
 
 import dask.dataframe as dd
 from dask import config as dask_config
-from dask.base import tokenize
-from dask.highlevelgraph import HighLevelGraph
 
 from dask_sql.datacontainer import ColumnContainer, DataContainer
 from dask_sql.physical.rel.base import BaseRelPlugin
 from dask_sql.physical.rel.logical.filter import filter_or_scalar
 from dask_sql.physical.rex import RexConverter
 from dask_sql.utils import is_cudf_type
 
@@ -128,49 +126,19 @@
             # where we have no column to merge on
             # This means we have no other chance than to merge
             # everything with everything...
 
             # TODO: we should implement a shortcut
             # for filter conditions that are always false
 
-            def merge_single_partitions(lhs_partition, rhs_partition):
-                # Do a cross join with the two partitions
-                # TODO: it would be nice to apply the filter already here
-                # problem: this would mean we need to ship the rex to the
-                # workers (as this is executed on the workers),
-                # which is definitely not possible (java dependency, JVM start...)
-                lhs_partition = lhs_partition.assign(common=1)
-                rhs_partition = rhs_partition.assign(common=1)
-
-                return lhs_partition.merge(rhs_partition, on="common").drop(
-                    columns="common"
-                )
-
-            # Iterate nested over all partitions from lhs and rhs and merge them
-            name = "cross-join-" + tokenize(df_lhs_renamed, df_rhs_renamed)
-            dsk = {
-                (name, i * df_rhs_renamed.npartitions + j): (
-                    merge_single_partitions,
-                    (df_lhs_renamed._name, i),
-                    (df_rhs_renamed._name, j),
-                )
-                for i in range(df_lhs_renamed.npartitions)
-                for j in range(df_rhs_renamed.npartitions)
-            }
-
-            graph = HighLevelGraph.from_collections(
-                name, dsk, dependencies=[df_lhs_renamed, df_rhs_renamed]
-            )
-
-            meta = dd.dispatch.concat(
-                [df_lhs_renamed._meta_nonempty, df_rhs_renamed._meta_nonempty], axis=1
-            )
-            # TODO: Do we know the divisions in any way here?
-            divisions = [None] * (len(dsk) + 1)
-            df = dd.DataFrame(graph, name, meta=meta, divisions=divisions)
+            df = dd.merge(
+                df_lhs_renamed.assign(common=1),
+                df_rhs_renamed.assign(common=1),
+                on="common",
+            ).drop(columns="common")
 
             warnings.warn(
                 "Need to do a cross-join, which is typically very resource heavy",
                 ResourceWarning,
             )
 
         # 6. So the next step is to make sure
```

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/logical/limit.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/logical/limit.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         """
         # if no offset is specified we can use `head` to compute the window
         if not offset:
             # if `check-first-partition` enabled, check if we have a relatively simple Dask graph and if so,
             # check if the first partition contains our desired window
             if (
                 dask_config.get("sql.limit.check-first-partition")
+                and not dd._dask_expr_enabled()
                 and all(
                     [
                         isinstance(
                             layer, (DataFrameIOLayer, Blockwise, MaterializedLayer)
                         )
                         for layer in df.dask.layers.values()
                     ]
@@ -75,14 +76,18 @@
         # compute the size of each partition
         # TODO: compute `cumsum` here when dask#9067 is resolved
         partition_borders = df.map_partitions(lambda x: len(x))
 
         def limit_partition_func(df, partition_borders, partition_info=None):
             """Limit the partition to values contained within the specified window, returning an empty dataframe if there are none"""
 
+            # with dask-expr we may need to explicitly compute here
+            if hasattr(partition_borders, "compute"):
+                partition_borders = partition_borders.compute()
+
             # TODO: remove the `cumsum` call here when dask#9067 is resolved
             partition_borders = partition_borders.cumsum().to_dict()
             partition_index = (
                 partition_info["number"] if partition_info is not None else 0
             )
 
             partition_border_left = (
```

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/logical/project.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/logical/project.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/logical/sample.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/logical/sample.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/logical/sort.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/logical/sort.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/logical/subquery_alias.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/logical/subquery_alias.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/logical/table_scan.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/logical/table_scan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import operator
 from functools import reduce
 from typing import TYPE_CHECKING
 
+from dask.dataframe import _dask_expr_enabled
 from dask.utils_test import hlg_layer
 
 from dask_sql.datacontainer import DataContainer
 from dask_sql.physical.rel.base import BaseRelPlugin
 from dask_sql.physical.rel.logical.filter import filter_or_scalar
 from dask_sql.physical.rex import RexConverter
 
@@ -104,13 +105,15 @@
                 operator.and_,
                 [
                     RexConverter.convert(rel, rex, dc, context=context)
                     for rex in all_filters
                 ],
             )
             df = filter_or_scalar(df, df_condition)
-        try:
-            logger.debug(hlg_layer(df.dask, "read-parquet").creation_info)
-        except KeyError:
-            pass
+
+        if not _dask_expr_enabled():
+            try:
+                logger.debug(hlg_layer(df.dask, "read-parquet").creation_info)
+            except KeyError:
+                pass
 
         return DataContainer(df, cc)
```

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/logical/union.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/logical/union.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/logical/values.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/logical/values.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rel/logical/window.py` & `dask_sql-2024.5.0/dask_sql/physical/rel/logical/window.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from typing import TYPE_CHECKING, Callable, Optional
 
 import dask.dataframe as dd
 import numpy as np
 import pandas as pd
 from pandas.api.indexers import BaseIndexer
 
-from dask_sql._compat import INDEXER_WINDOW_STEP_IMPLEMENTED
 from dask_sql.datacontainer import ColumnContainer, DataContainer
 from dask_sql.physical.rel.base import BaseRelPlugin
 from dask_sql.physical.rex.convert import RexConverter
 from dask_sql.physical.utils.sort import sort_partition_func
 from dask_sql.utils import LoggableDataFrame, new_temporary_column
 
 if TYPE_CHECKING:
@@ -128,36 +127,23 @@
                 end[: -self.end] = 0
             else:  # pragma: no cover
                 raise AssertionError(
                     "This case should have been handled before! Please report this bug"
                 )
         return start, end
 
-    if INDEXER_WINDOW_STEP_IMPLEMENTED:
-
-        def get_window_bounds(
-            self,
-            num_values: int = 0,
-            min_periods: Optional[int] = None,
-            center: Optional[bool] = None,
-            closed: Optional[str] = None,
-            step: Optional[int] = None,
-        ) -> tuple[np.ndarray, np.ndarray]:
-            return self._get_window_bounds(num_values, min_periods, center, closed)
-
-    else:
-
-        def get_window_bounds(
-            self,
-            num_values: int = 0,
-            min_periods: Optional[int] = None,
-            center: Optional[bool] = None,
-            closed: Optional[str] = None,
-        ) -> tuple[np.ndarray, np.ndarray]:
-            return self._get_window_bounds(num_values, min_periods, center, closed)
+    def get_window_bounds(
+        self,
+        num_values: int = 0,
+        min_periods: Optional[int] = None,
+        center: Optional[bool] = None,
+        closed: Optional[str] = None,
+        step: Optional[int] = None,
+    ) -> tuple[np.ndarray, np.ndarray]:
+        return self._get_window_bounds(num_values, min_periods, center, closed)
 
 
 def map_on_each_group(
     partitioned_group: pd.DataFrame,
     sort_columns: list[str],
     sort_ascending: list[bool],
     sort_null_first: list[bool],
```

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rex/base.py` & `dask_sql-2024.5.0/dask_sql/physical/rex/base.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rex/convert.py` & `dask_sql-2024.5.0/dask_sql/physical/rex/convert.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rex/core/alias.py` & `dask_sql-2024.5.0/dask_sql/physical/rex/core/alias.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rex/core/call.py` & `dask_sql-2024.5.0/dask_sql/physical/rex/core/call.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 from typing import TYPE_CHECKING, Any, Callable, Union
 
 import dask.array as da
 import dask.config as dask_config
 import dask.dataframe as dd
 import numpy as np
 import pandas as pd
-from dask.base import tokenize
-from dask.dataframe.core import Series
-from dask.highlevelgraph import HighLevelGraph
 from dask.utils import random_state_data
 
 from dask_sql._datafusion_lib import SqlTypeName
 from dask_sql.datacontainer import DataContainer
 from dask_sql.mappings import (
     cast_column_to_type,
     sql_to_python_type,
@@ -824,45 +821,36 @@
 
     def random_function(self, partition, random_state, kwargs):
         """Needs to be implemented in derived classes"""
         raise NotImplementedError
 
     def random_frame(self, seed: int, dc: DataContainer, **kwargs) -> dd.Series:
         """This function - in contrast to others in this module - will only ever be called on data frames"""
-
-        random_state = np.random.RandomState(seed=seed)
-
-        # Idea taken from dask.DataFrame.sample:
-        # initialize a random state for each of the partitions
-        # separately and then create a random series
-        # for each partition
         df = dc.df
-        name = "sample-" + tokenize(df, random_state)
+        state_data = random_state_data(df.npartitions, np.random.RandomState(seed=seed))
 
-        state_data = random_state_data(df.npartitions, random_state)
-        dsk = {
-            (name, i): (
-                self.random_function,
-                (df._name, i),
-                np.random.RandomState(state),
-                kwargs,
+        def random_partition_func(df, state_data, partition_info=None):
+            """Create a random number for each partition"""
+            partition_index = (
+                partition_info["number"] if partition_info is not None else 0
             )
-            for i, state in enumerate(state_data)
-        }
 
-        graph = HighLevelGraph.from_collections(name, dsk, dependencies=[df])
-        random_series = Series(graph, name, ("random", "float64"), df.divisions)
+            state = np.random.RandomState(state_data[partition_index])
+            return self.random_function(df, state, kwargs)
+
+        random_series = df.map_partitions(
+            random_partition_func, state_data, meta=("random", "float64")
+        )
 
         # This part seems to be stupid, but helps us do a very simple
         # task without going into the (private) internals of Dask:
         # copy all meta information from the original input dataframe
         # This is important so that the returned series looks
         # exactly like coming from the input dataframe
-        return_df = df.assign(random=random_series)["random"]
-        return return_df
+        return df.assign(random=random_series)["random"]
 
 
 class RandOperation(BaseRandomOperation):
     """Create a random number between 0 and 1"""
 
     def __init__(self):
         super().__init__(f=self.rand)
```

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rex/core/input_ref.py` & `dask_sql-2024.5.0/dask_sql/physical/rex/core/input_ref.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rex/core/literal.py` & `dask_sql-2024.5.0/dask_sql/physical/rex/core/literal.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/rex/core/subquery.py` & `dask_sql-2024.5.0/dask_sql/physical/rex/core/subquery.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/utils/filter.py` & `dask_sql-2024.5.0/dask_sql/physical/utils/filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,27 +300,27 @@
     }
     | _pass_through_ops
 )
 
 # Specify functions that must be generated with
 # a different API at the dataframe-collection level
 _special_op_mappings = {
-    M.fillna: dd._Frame.fillna,
-    M.isin: dd._Frame.isin,
-    M.isna: dd._Frame.isna,
-    M.astype: dd._Frame.astype,
+    M.fillna: dd.DataFrame.fillna,
+    M.isin: dd.DataFrame.isin,
+    M.isna: dd.DataFrame.isna,
+    M.astype: dd.DataFrame.astype,
 }
 
 # Convert _pass_through_ops to respect "special" mappings
 _pass_through_ops = {_special_op_mappings.get(op, op) for op in _pass_through_ops}
 
 
 def _preprocess_layers(input_layers):
     # NOTE: This is a Layer-specific work-around to deal with
-    # the fact that `dd._Frame.isin(values)` will add a distinct
+    # the fact that `dd.DataFrame.isin(values)` will add a distinct
     # `MaterializedLayer` for the `values` argument.
     # See: https://github.com/dask-contrib/dask-sql/issues/607
     skip = set()
     layers = input_layers.copy()
     for key, layer in layers.items():
         if key.startswith("isin-") and isinstance(layer, Blockwise):
             indices = list(layer.indices)
@@ -414,17 +414,17 @@
         op = self.creation_info["func"]
         if op in _comparison_symbols.keys():
             func = _blockwise_comparison_dnf
         elif op in (operator.and_, operator.or_):
             func = _blockwise_logical_dnf
         elif op == operator.getitem:
             func = _blockwise_getitem_dnf
-        elif op == dd._Frame.isin:
+        elif op == dd.DataFrame.isin:
             func = _blockwise_isin_dnf
-        elif op == dd._Frame.isna:
+        elif op == dd.DataFrame.isna:
             func = _blockwise_isna_dnf
         elif op == operator.inv:
             func = _blockwise_inv_dnf
         elif op in _pass_through_ops:
             func = _blockwise_pass_through_dnf
         else:
             raise ValueError(f"No DNF expression for {op}")
```

### Comparing `dask_sql-2024.3.0/dask_sql/physical/utils/groupby.py` & `dask_sql-2024.5.0/dask_sql/physical/utils/groupby.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/utils/ml_classes.py` & `dask_sql-2024.5.0/dask_sql/physical/utils/ml_classes.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/utils/sort.py` & `dask_sql-2024.5.0/dask_sql/physical/utils/sort.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/physical/utils/statistics.py` & `dask_sql-2024.5.0/dask_sql/physical/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/server/app.py` & `dask_sql-2024.5.0/dask_sql/server/app.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/server/presto_jdbc.py` & `dask_sql-2024.5.0/dask_sql/server/presto_jdbc.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/server/responses.py` & `dask_sql-2024.5.0/dask_sql/server/responses.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/sql-schema.yaml` & `dask_sql-2024.5.0/dask_sql/sql-schema.yaml`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/dask_sql/utils.py` & `dask_sql-2024.5.0/dask_sql/utils.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/dialect.rs` & `dask_sql-2024.5.0/src/dialect.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/error.rs` & `dask_sql-2024.5.0/src/error.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/expression.rs` & `dask_sql-2024.5.0/src/expression.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/lib.rs` & `dask_sql-2024.5.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/parser.rs` & `dask_sql-2024.5.0/src/parser.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/column.rs` & `dask_sql-2024.5.0/src/sql/column.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/exceptions.rs` & `dask_sql-2024.5.0/src/sql/exceptions.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/function.rs` & `dask_sql-2024.5.0/src/sql/function.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/aggregate.rs` & `dask_sql-2024.5.0/src/sql/logical/aggregate.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/alter_schema.rs` & `dask_sql-2024.5.0/src/sql/logical/alter_schema.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/alter_table.rs` & `dask_sql-2024.5.0/src/sql/logical/alter_table.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/analyze_table.rs` & `dask_sql-2024.5.0/src/sql/logical/analyze_table.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/create_catalog_schema.rs` & `dask_sql-2024.5.0/src/sql/logical/create_catalog_schema.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/create_experiment.rs` & `dask_sql-2024.5.0/src/sql/logical/create_experiment.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/create_memory_table.rs` & `dask_sql-2024.5.0/src/sql/logical/create_memory_table.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/create_model.rs` & `dask_sql-2024.5.0/src/sql/logical/create_model.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/create_table.rs` & `dask_sql-2024.5.0/src/sql/logical/create_table.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/describe_model.rs` & `dask_sql-2024.5.0/src/sql/logical/describe_model.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/drop_model.rs` & `dask_sql-2024.5.0/src/sql/logical/drop_model.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/drop_schema.rs` & `dask_sql-2024.5.0/src/sql/logical/drop_schema.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/drop_table.rs` & `dask_sql-2024.5.0/src/sql/logical/drop_table.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/empty_relation.rs` & `dask_sql-2024.5.0/src/sql/logical/empty_relation.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/explain.rs` & `dask_sql-2024.5.0/src/sql/logical/explain.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/export_model.rs` & `dask_sql-2024.5.0/src/sql/logical/export_model.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/filter.rs` & `dask_sql-2024.5.0/src/sql/logical/filter.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/join.rs` & `dask_sql-2024.5.0/src/sql/logical/join.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/limit.rs` & `dask_sql-2024.5.0/src/sql/logical/limit.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/predict_model.rs` & `dask_sql-2024.5.0/src/sql/logical/predict_model.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/projection.rs` & `dask_sql-2024.5.0/src/sql/logical/projection.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/repartition_by.rs` & `dask_sql-2024.5.0/src/sql/logical/repartition_by.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/show_columns.rs` & `dask_sql-2024.5.0/src/sql/logical/show_columns.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/show_models.rs` & `dask_sql-2024.5.0/src/sql/logical/show_models.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/show_schemas.rs` & `dask_sql-2024.5.0/src/sql/logical/show_schemas.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/show_tables.rs` & `dask_sql-2024.5.0/src/sql/logical/show_tables.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/sort.rs` & `dask_sql-2024.5.0/src/sql/logical/sort.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/subquery_alias.rs` & `dask_sql-2024.5.0/src/sql/logical/subquery_alias.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/table_scan.rs` & `dask_sql-2024.5.0/src/sql/logical/table_scan.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/use_schema.rs` & `dask_sql-2024.5.0/src/sql/logical/use_schema.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical/window.rs` & `dask_sql-2024.5.0/src/sql/logical/window.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/logical.rs` & `dask_sql-2024.5.0/src/sql/logical.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/optimizer/decorrelate_where_exists.rs` & `dask_sql-2024.5.0/src/sql/optimizer/decorrelate_where_exists.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/optimizer/decorrelate_where_in.rs` & `dask_sql-2024.5.0/src/sql/optimizer/decorrelate_where_in.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/optimizer/dynamic_partition_pruning.rs` & `dask_sql-2024.5.0/src/sql/optimizer/dynamic_partition_pruning.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/optimizer/join_reorder.rs` & `dask_sql-2024.5.0/src/sql/optimizer/join_reorder.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/optimizer/utils.rs` & `dask_sql-2024.5.0/src/sql/optimizer/utils.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/optimizer.rs` & `dask_sql-2024.5.0/src/sql/optimizer.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/parser_utils.rs` & `dask_sql-2024.5.0/src/sql/parser_utils.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/preoptimizer.rs` & `dask_sql-2024.5.0/src/sql/preoptimizer.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/schema.rs` & `dask_sql-2024.5.0/src/sql/schema.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/statement.rs` & `dask_sql-2024.5.0/src/sql/statement.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/table.rs` & `dask_sql-2024.5.0/src/sql/table.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/types/rel_data_type.rs` & `dask_sql-2024.5.0/src/sql/types/rel_data_type.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/types/rel_data_type_field.rs` & `dask_sql-2024.5.0/src/sql/types/rel_data_type_field.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql/types.rs` & `dask_sql-2024.5.0/src/sql/types.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/src/sql.rs` & `dask_sql-2024.5.0/src/sql.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2024.3.0/Cargo.lock` & `dask_sql-2024.5.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -750,15 +750,15 @@
  "lock_api",
  "once_cell",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "dask-sql"
-version = "2024.3.0"
+version = "2024.5.0"
 dependencies = [
  "async-trait",
  "datafusion-python",
  "env_logger",
  "log",
  "pyo3",
  "pyo3-build-config 0.20.3",
```

### Comparing `dask_sql-2024.3.0/pyproject.toml` & `dask_sql-2024.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Topic :: System :: Distributed Computing",
 ]
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
-    "dask[dataframe]==2024.1.1",
-    "distributed==2024.1.1",
+    "dask[dataframe]>=2024.4.1",
+    "distributed>=2024.4.1",
     "pandas>=1.4.0",
     "fastapi>=0.92.0",
     "httpx>=0.24.1",
     "uvicorn>=0.14",
     "tzlocal>=2.1",
     "prompt_toolkit>=3.0.8",
     "pygments>=2.7.1",
@@ -98,9 +98,10 @@
 addopts = "-v -rsxfE --color=yes --cov dask_sql --cov-config=.coveragerc --cov-report=term-missing"
 filterwarnings = [
     "error:::dask_sql[.*]",
     "error:::dask[.*]",
     "ignore:Need to do a cross-join:ResourceWarning:dask_sql[.*]",
     "ignore:Dask doesn't support Dask frames:ResourceWarning:dask_sql[.*]",
     "ignore:Running on a single-machine scheduler:UserWarning:dask[.*]",
+    "ignore:Merging dataframes with merge column data type mismatches:UserWarning:dask[.*]",
 ]
 xfail_strict = true
```

### Comparing `dask_sql-2024.3.0/PKG-INFO` & `dask_sql-2024.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask_sql
-Version: 2024.3.0
+Version: 2024.5.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python
@@ -12,16 +12,16 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
-Requires-Dist: dask[dataframe] ==2024.1.1
-Requires-Dist: distributed ==2024.1.1
+Requires-Dist: dask[dataframe] >=2024.4.1
+Requires-Dist: distributed >=2024.4.1
 Requires-Dist: pandas >=1.4.0
 Requires-Dist: fastapi >=0.92.0
 Requires-Dist: httpx >=0.24.1
 Requires-Dist: uvicorn >=0.14
 Requires-Dist: tzlocal >=2.1
 Requires-Dist: prompt_toolkit >=3.0.8
 Requires-Dist: pygments >=2.7.1
```

